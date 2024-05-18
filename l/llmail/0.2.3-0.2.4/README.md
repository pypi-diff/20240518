# Comparing `tmp/llmail-0.2.3.tar.gz` & `tmp/llmail-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llmail-0.2.3.tar", max compression
+gzip compressed data, was "llmail-0.2.4.tar", max compression
```

## Comparing `llmail-0.2.3.tar` & `llmail-0.2.4.tar`

### file list

```diff
@@ -1,8 +1,9 @@
--rw-r--r--   0        0        0    34516 2024-05-12 20:14:56.460155 llmail-0.2.3/LICENSE
--rw-r--r--   0        0        0     2724 2024-05-12 20:14:56.460155 llmail-0.2.3/README.md
--rw-r--r--   0        0        0        0 2024-05-12 20:14:56.460155 llmail-0.2.3/llmail/__init__.py
--rw-r--r--   0        0        0    22752 2024-05-12 20:14:56.460155 llmail-0.2.3/llmail/__main__.py
--rw-r--r--   0        0        0        0 2024-05-12 20:14:56.460155 llmail-0.2.3/llmail/utils/__init__.py
--rw-r--r--   0        0        0     5360 2024-05-12 20:14:56.460155 llmail-0.2.3/llmail/utils/cli_args.py
--rw-r--r--   0        0        0      872 2024-05-12 20:14:56.460155 llmail-0.2.3/pyproject.toml
--rw-r--r--   0        0        0     3601 1970-01-01 00:00:00.000000 llmail-0.2.3/PKG-INFO
+-rw-r--r--   0        0        0    34516 2024-04-29 23:29:15.749949 llmail-0.2.4/LICENSE
+-rw-r--r--   0        0        0        0 2024-04-29 23:31:53.519788 llmail-0.2.4/llmail/__init__.py
+-rw-r--r--   0        0        0    24205 2024-05-18 02:12:51.082069 llmail-0.2.4/llmail/__main__.py
+-rw-r--r--   0        0        0        0 2024-04-29 23:49:56.280104 llmail-0.2.4/llmail/utils/__init__.py
+-rw-r--r--   0        0        0     6044 2024-05-18 01:33:13.218763 llmail-0.2.4/llmail/utils/cli_args.py
+-rw-r--r--   0        0        0      935 2024-05-18 01:33:13.219290 llmail-0.2.4/llmail/utils/utils.py
+-rw-r--r--   0        0        0      882 2024-05-18 02:08:30.488272 llmail-0.2.4/pyproject.toml
+-rw-r--r--   0        0        0     2724 2024-05-12 20:12:58.445880 llmail-0.2.4/README.md
+-rw-r--r--   0        0        0     3656 1970-01-01 00:00:00.000000 llmail-0.2.4/PKG-INFO
```

### Comparing `llmail-0.2.3/LICENSE` & `llmail-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `llmail-0.2.3/README.md` & `llmail-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `llmail-0.2.3/llmail/__main__.py` & `llmail-0.2.4/llmail/__main__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 from email import message_from_bytes
 from email.message import Message
-from sys import stderr
 import yagmail
 import html2text
-from icecream import ic
 from imapclient import IMAPClient
 import imaplib
 from loguru import logger
 from openai import OpenAI
 from email.utils import getaddresses, parsedate_to_datetime, make_msgid
 from datetime import timezone
 import time
+import re
 
 
 from llmail.utils.cli_args import argparser
+from llmail.utils.utils import set_primary_logger
 
 
 class EmailThread:
     def __init__(self, initial_email):
         self.initial_email = initial_email
         self.replies = []
 
@@ -43,19 +43,23 @@
 
     def sort_replies(self):
         self.replies = sorted(self.replies, key=lambda x: x.timestamp)
         # Honestly, it might be better to sort by the message_id. This also goes for the get_thread_history function
         # However, this **significantly** reduces complexity so for now, it's fine
 
     def __repr__(self):
-        return f"EmailThread(initial_email={self.initial_email}, replies={self.replies})"
+        return (
+            f"EmailThread(initial_email={self.initial_email}, replies={self.replies})"
+        )
 
 
 class Email:
-    def __init__(self, imap_id, message_id, subject, sender, timestamp, body, references):
+    def __init__(
+        self, imap_id, message_id, subject, sender, timestamp, body, references
+    ):
         self.imap_id = imap_id
         self.message_id = message_id
         self.subject = subject
         self.sender = sender
         self.timestamp = timestamp
         self.body = body
         self.references = references
@@ -67,84 +71,110 @@
 
 args = None
 bot_email = None
 
 email_threads = {}
 
 
-
 def main():
     """Main entry point for the script."""
     global args
     global bot_email
     global email_threads
     args = argparser.parse_args()
 
-
     match args.subcommand:
         case "list-folders":
             with IMAPClient(args.imap_host) as client:
                 client.login(args.imap_username, args.imap_password)
                 folders = client.list_folders()
                 for folder in folders:
                     print(folder[2])
         case None:
             bot_email = args.imap_username
 
             # Set up logging
-            set_primary_logger(args.log_level)
-            ic(args)
+            set_primary_logger(args.log_level, args.redact_email_addresses)
+            logger.debug(args)
             if args.watch_interval:
-                logger.info(f"Watching for new emails every {args.watch_interval} seconds")
+                logger.info(
+                    f"Watching for new emails every {args.watch_interval} seconds"
+                )
                 while True:
                     fetch_and_process_emails(
-                        subject=args.subject_key,
+                        look_for_subject=args.subject_key,
                         alias=args.alias,
                         system_prompt=args.system_prompt,
                     )
                     time.sleep(args.watch_interval)
                     # **EMPTY THREADS**
                     email_threads = {}
             else:
                 fetch_and_process_emails(
-                    subject=args.subject_key,
+                    look_for_subject=args.subject_key,
                     alias=args.alias,
                     system_prompt=args.system_prompt,
                 )
 
+
 def fetch_and_process_emails(
-        subject: str,
-        alias: str = None,
-        system_prompt: str = None,
+    look_for_subject: str,
+    alias: str = None,
+    system_prompt: str = None,
 ):
     """Fetch and process emails from the IMAP server."""
     global email_threads
     openai = OpenAI(api_key=args.openai_api_key, base_url=args.openai_base_url)
     with IMAPClient(args.imap_host) as client:
         client.login(args.imap_username, args.imap_password)
 
         email_threads = {}
-        folders = args.folder if args.folder else [folder[2] for folder in client.list_folders()]
+        folders = (
+            args.folder
+            if args.folder
+            else [folder[2] for folder in client.list_folders()]
+        )
         # for folder in client.list_folders():
         # Disabling fetching from all folders due it not being inefficient
         # Instead, just fetch from INBOX and get the threads later
         for folder in folders:
             try:
                 client.select_folder(folder)
             # If the error is imaplib.IMAP4.error: select failed:...
             except imaplib.IMAP4.error:
                 logger.debug(f"Failed to select folder {folder[2]}. Skipping...")
                 continue
             # Might be smart to also search for forwarded emails
-            messages = client.search(["OR", "SUBJECT", subject, "SUBJECT", f"Re: {subject}"])
+            messages = client.search(
+                [
+                    "OR",
+                    "SUBJECT",
+                    look_for_subject,
+                    "SUBJECT",
+                    f"Re: {look_for_subject}",
+                ]
+            )
             for msg_id in messages:
                 # TODO: It seems this will throw a KeyError if an email is sent while this for loop is running. May have been fixed by emptying email_threads at the end of the while loop? This should be tested again to confirm
-                msg_data = client.fetch([msg_id], ["ENVELOPE", "BODY[]", "RFC822.HEADER"])
+                msg_data = client.fetch(
+                    [msg_id], ["ENVELOPE", "BODY[]", "RFC822.HEADER"]
+                )
                 envelope = msg_data[msg_id][b"ENVELOPE"]
                 subject = envelope.subject.decode()
+                # Use regex to verify that the subject optionally starts with "Fwd: " or "Re: " and then the intended subject (nothing case-sensitive)
+                # re.escape is used to escape any special characters in the subject
+                if not re.match(
+                    r"^(Fwd: ?|Re: ?)*" + re.escape(look_for_subject) + r"$",
+                    subject,
+                    re.IGNORECASE,
+                ):
+                    logger.warning(
+                        f"Skipping email with subject '{subject}' as it does not match the intended subject"
+                    )
+                    continue
                 timestamp = envelope.date
                 # Parse the headers from the email data
                 message = message_from_bytes(msg_data[msg_id][b"RFC822.HEADER"])
                 sender = get_sender(message)["email"]
                 headers = dict(message.items())
                 # Extract references from the email
                 references_header = headers.get("References", "")
@@ -197,37 +227,46 @@
                                     body=get_plain_email_content(
                                         message_from_bytes(msg_data[msg_id][b"BODY[]"])
                                     ),
                                     references=references_ids,
                                 )
                             )
                             email_threads[parent_email_id] = email_thread
-                            logger.info(
+                            logger.debug(
                                 f"Created new thread for email {message_id} sent at {timestamp}"
                             )
 
-        # ic([thread for thread in email_threads.values()])
-        ic(email_threads)
+        logger.debug(email_threads)
         # Check if there are any emails wherein the last email in the thread is a user email
         # If so, send a reply
         for message_id, email_thread in email_threads.items():
             # Check if the email only has an initial email
             # If it does, then there won't be any replies and an index error will occur
             if len(email_thread.replies) == 0:
                 logger.debug(f"No replies in thread for email {message_id}")
                 message_id = email_thread.initial_email.message_id
                 msg_id = email_thread.initial_email.imap_id
                 references_ids = email_thread.initial_email.references
-            elif len(email_thread.replies) > 0 and email_thread.replies[-1].sender != bot_email:
-                logger.debug(f"Last email in thread for email {message_id} is from {email_thread.replies[-1].sender}")
+            elif (
+                len(email_thread.replies) > 0
+                and email_thread.replies[-1].sender != bot_email
+            ):
+                logger.debug(
+                    f"Last email in thread for email {message_id} is from {email_thread.replies[-1].sender}"
+                )
                 message_id = email_thread.replies[-1].message_id
                 msg_id = email_thread.replies[-1].imap_id
                 references_ids = email_thread.replies[-1].references
-            elif len(email_thread.replies) > 0 and email_thread.replies[-1].sender == bot_email:
-                logger.debug(f"Last email in thread for email {message_id} is from the bot")
+            elif (
+                len(email_thread.replies) > 0
+                and email_thread.replies[-1].sender == bot_email
+            ):
+                logger.debug(
+                    f"Last email in thread for email {message_id} is from the bot"
+                )
                 continue
             else:
                 ValueError("Invalid email thread")
             send_reply(
                 thread=get_thread_history(client, email_thread),
                 subject=subject,
                 alias=args.alias,
@@ -236,15 +275,15 @@
                 message_id=message_id,
                 references_ids=references_ids,
                 openai=openai,
                 system_prompt=system_prompt,
                 model=args.openai_model,
             )
 
-        logger.debug(f"Keys in email_threads: {len(email_threads.keys())}")
+        logger.info (f"Current number of email threads: {len(email_threads.keys())}")
 
 
 # Function to check if an email has been read
 def is_new_email(client, msg_id):
     flags = client.get_flags([msg_id])
     return b"\\Seen" not in flags.get(msg_id, [])
 
@@ -272,15 +311,19 @@
             {
                 "sender": message_identifier.initial_email.sender,
                 "content": message_identifier.initial_email.body,
             }
         )
         for email in message_identifier.replies:
             thread_history.append(
-                {"sender": email.sender, "content": email.body, "timestamp": email.timestamp}
+                {
+                    "sender": email.sender,
+                    "content": email.body,
+                    "timestamp": email.timestamp,
+                }
             )
         return thread_history
     elif isinstance(message_identifier, int) or isinstance(message_identifier, str):
         client.select_folder("INBOX")
         if isinstance(message_identifier, str):
             message_id = message_identifier
             msg_id = get_uid_from_message_id(client, message_id)
@@ -318,23 +361,27 @@
             prev_msg_data = client.fetch([prev_msg_id], ["RFC822"])
             prev_raw_message = prev_msg_data[prev_msg_id][b"RFC822"]
             prev_message = message_from_bytes(prev_raw_message)
             thread_history.append(
                 {
                     "sender": get_sender(message)["email"],
                     "content": get_plain_email_content(message),
-                    "timestamp": make_tz_aware(parsedate_to_datetime(message.get("Date"))),
+                    "timestamp": make_tz_aware(
+                        parsedate_to_datetime(message.get("Date"))
+                    ),
                 }
             )
             message = prev_message
         # Sort the thread history by timestamp
         thread_history = sorted(thread_history, key=lambda x: x["timestamp"])
         return thread_history
     else:
-        raise TypeError("Invalid type for message. Must be an int, str, or EmailThread object.")
+        raise TypeError(
+            "Invalid type for message. Must be an int, str, or EmailThread object."
+        )
 
 
 def get_sender(message: Message) -> dict:
     """Extract the sender information from an email message."""
     sender = message.get("From", "")
     sender_name, sender_email = getaddresses([sender])[0]
     return {"name": sender_name, "email": sender_email}
@@ -348,15 +395,17 @@
 
     # Parse the headers using the email library
     msg = message_from_bytes(headers_bytes)
     headers = dict(msg.items())
 
     # Extract the References header and split it into individual message IDs
     references_header = headers.get("References", "")
-    references_ids = [m_id.strip() for m_id in references_header.split() if m_id.strip()]
+    references_ids = [
+        m_id.strip() for m_id in references_header.split() if m_id.strip()
+    ]
 
     # Extract the first message ID, which represents the top-level email in the thread
     # If it doesn't exist, use the current message ID. Not msg_id since msg_id is only for IMAP
     top_level_email_id = references_ids[0] if references_ids else message_id
     return top_level_email_id
 
 
@@ -396,22 +445,14 @@
             return uid
     logger.warning(
         f"UID of message with Message-ID {message_id} not found. Trying to check all headers and text."
     )
     return None
 
 
-def set_primary_logger(log_level):
-    """Set up the primary logger with the specified log level. Output to stderr and use the format specified."""
-    logger.remove()
-    # ^10 is a formatting directive to center with a padding of 10
-    logger_format = "<green>{time:YYYY-MM-DD HH:mm:ss}</green> |<level>{level: ^10}</level>| <level>{message}</level>"
-    logger.add(stderr, format=logger_format, colorize=True, level=log_level)
-
-
 def send_reply(
     thread: list[dict],
     subject: str,
     alias: str,
     client: IMAPClient,
     msg_id: int,
     message_id: str,
@@ -420,45 +461,48 @@
     system_prompt: str,
     model: str,
 ):
     """Send a reply to the email with the specified message ID."""
     # Set roles deletes the sender key so we need to store the sender before calling it
     sender = thread[-1]["sender"]
     thread = set_roles(thread)
-    if system_prompt:   
+    if system_prompt:
         thread.insert(0, {"role": "system", "content": system_prompt})
     references_ids.append(message_id)
-    # thread_from_msg_id = get_thread_history(client, msg_id)
-    # logger.debug(f"Thread history (message_identifier): {thread_from_msg_id}")
-    # logger.debug(f"Thread history length (message_identifier): {len(thread_from_msg_id)}")
-    # thread_from_object = get_thread_history(client, email_threads[list(email_threads.keys())[-1]])
-    # logger.debug(f"Thread history (EmailThread object): {thread_from_object}")
-    # logger.debug(f"Thread history length (EmailThread object): {len(thread_from_object)}")
-    logger.info(f"Sending reply to email {message_id} to {sender}")
-    logger.debug(f"Thread history: {thread}")
-    logger.debug(f"Thread history length: {len(thread)}")
     generated_response = openai.chat.completions.create(
         model=model,
         messages=thread,
     )
     generated_response = generated_response.choices[0].message.content
     logger.debug(f"Generated response: {generated_response}")
     yag = yagmail.SMTP(
         user={args.smtp_username: alias} if alias else args.smtp_username,
         password=args.smtp_password,
         host=args.smtp_host,
         port=int(args.smtp_port),
     )
     yag.send(
         to=sender,
+        # subject=f"Re: {subject}" if not subject.startswith("Re: ") else subject,
         subject=f"Re: {subject}",
         headers={"In-Reply-To": message_id, "References": " ".join(references_ids)},
         contents=generated_response,
-        message_id=make_msgid(domain=args.message_id_domain if args.message_id_domain else "llmail"),
+        message_id=make_msgid(
+            domain=args.message_id_domain if args.message_id_domain else "llmail"
+        ),
     )
+    # thread_from_msg_id = get_thread_history(client, msg_id)
+    # logger.debug(f"Thread history (message_identifier): {thread_from_msg_id}")
+    # logger.debug(f"Thread history length (message_identifier): {len(thread_from_msg_id)}")
+    # thread_from_object = get_thread_history(client, email_threads[list(email_threads.keys())[-1]])
+    # logger.debug(f"Thread history (EmailThread object): {thread_from_object}")
+    # logger.debug(f"Thread history length (EmailThread object): {len(thread_from_object)}")
+    logger.info(f"Sending reply to email {message_id} to {sender}")
+    logger.debug(f"Thread history: {thread}")
+    logger.debug(f"Thread history length: {len(thread)}")
 
 
 def get_plain_email_content(message: Message | str) -> str:
     """Get the content of the email message. If a  message object is provided, it will be parsed
     Otherwise, it is assumed that the content is already a string and will be converted to markdown.
     """
     if isinstance(message, str):
@@ -466,23 +510,33 @@
     else:
         if message.is_multipart():
             for part in message.walk():
                 content_type = part.get_content_type()
                 try:
                     body = part.get_payload(decode=True)
                 except UnicodeDecodeError:
-                    logger.debug("UnicodeDecodeError occurred. Trying to get payload as string.")
+                    logger.debug(
+                        "UnicodeDecodeError occurred. Trying to get payload as string."
+                    )
                     body = str(part.get_payload())
                 if content_type == "text/plain":
-                    markdown = html2text.html2text(str(body.decode("unicode_escape"))).strip()
+                    markdown = html2text.html2text(
+                        str(body.decode("unicode_escape"))
+                    ).strip()
                     # logger.debug(f"Converted to markdown: {markdown}")
+                    # if len(markdown) < 5:
+                    #     logger.warning(
+                    #         f"Content is less than 5 characters | Content: {markdown}"
+                    #     )
                     return markdown
         else:
             logger.debug("Message is not multipart. Getting payload as string.")
             body = message.get_payload(decode=True).decode()
+            # if len(body) < 5:
+            #     logger.warning(f"Content is less than 5 characters | Content: {body}")
             return html2text.html2text(str(body.decode("unicode_escape")))
 
 
 def set_roles(thread_history: list[dict]) -> list[dict]:
     """Change all email senders to roles (assistant or user)"""
     # Change email senders to roles
     for email in thread_history:
```

### Comparing `llmail-0.2.3/llmail/utils/cli_args.py` & `llmail-0.2.4/llmail/utils/cli_args.py`

 * *Files 9% similar despite different names*

```diff
@@ -11,15 +11,14 @@
 - Hostname: imap.gmail.com
 - Port: 993
 - Username: Your full Gmail address
 - Password: App token (when using 2FA) or perhaps your regular password (if not using 2FA ?)
 """
 
 
-
 def set_argparse():
     global argparser
 
     if Path(".env").is_file():
         dotenv.load_dotenv()
         print("Loaded .env file")
     else:
@@ -32,45 +31,67 @@
         epilog=":)",
     )
     # Subcommands
     subparsers = argparser.add_subparsers(
         # Dest means that the current subcommand can be accessed via args.subcommand
         dest="subcommand",
         title="Subcommands",
-        )
+    )
     # Subcommand: list-folders
-    _ = subparsers.add_parser("list-folders", help="List all folders in the IMAP account and exit")
+    _ = subparsers.add_parser(
+        "list-folders", help="List all folders in the IMAP account and exit"
+    )
     # General arguments
     argparser.add_argument(
         "--log-level",
         "-l",
         help="Log level",
         default=os.getenv("LOG_LEVEL") if os.getenv("LOG_LEVEL") else "INFO",
     )
     argparser.add_argument(
+        "--redact-email-addresses",
+        help="Replace email addresses with '[redacted]' in logs",
+        action="store_true",
+        default=(
+            True
+            if (
+                os.getenv("REDACT_EMAIL_ADDRESSES")
+                and os.getenv("REDACT_EMAIL_ADDRESSES").lower() == "true"
+                and os.getenv("REDACT_EMAIL_ADDRESSES").lower() != "false"
+            )
+            else False
+        ),
+    )
+    argparser.add_argument(
         "--watch-interval",
         "-w",
         help="Interval in seconds to check for new emails. If not set, will only check once.",
         type=int,
-        default=int(os.getenv("WATCH_INTERVAL")) if os.getenv("WATCH_INTERVAL") else None,
+        default=(
+            int(os.getenv("WATCH_INTERVAL")) if os.getenv("WATCH_INTERVAL") else None
+        ),
     )
     # OpenAI-compatible API arguments
     ai_api = argparser.add_argument_group("OpenAI-compatible API")
     ai_api.add_argument(
         "--openai-api-key", help="OpenAI API key", default=os.getenv("OPENAI_API_KEY")
     )
     ai_api.add_argument(
         "--openai-base-url",
         help="OpenAI API endpoint",
         default=os.getenv("OPENAI_BASE_URL"),
     )
     ai_api.add_argument(
         "--openai-model",
         help="Model to use for the LLM",
-        default=os.getenv("OPENAI_MODEL") if os.getenv("OPENAI_MODEL") else "mistralai/mistral-7b-instruct:free",
+        default=(
+            os.getenv("OPENAI_MODEL")
+            if os.getenv("OPENAI_MODEL")
+            else "mistralai/mistral-7b-instruct:free"
+        ),
     )
     ai_api.add_argument(
         "--system-prompt",
         help="Prepend this to the message history sent to the LLM as a message from the system role",
         default=os.getenv("SYSTEM_PROMPT") if os.getenv("SYSTEM_PROMPT") else None,
     )
     # Email arguments
@@ -83,51 +104,63 @@
         default=os.getenv("FOLDER").split(",") if os.getenv("FOLDER") else None,
         action="append",
     )
     email.add_argument(
         "--subject-key",
         "-s",
         help="Emails with this subject will be replied to",
-        default=os.getenv("SUBJECT_KEY") if os.getenv("SUBJECT_KEY") else "llmail autoreply",
+        default=(
+            os.getenv("SUBJECT_KEY") if os.getenv("SUBJECT_KEY") else "llmail autoreply"
+        ),
     )
     email.add_argument(
         "--alias",
         help="Name to use in the 'From' in addition to the email address",
         default=os.getenv("ALIAS") if os.getenv("ALIAS") else "LLMail",
     )
     imap = email.add_argument_group("IMAP")
-    imap.add_argument("--imap-host", help="IMAP server hostname", default=os.getenv("IMAP_HOST"))
-    imap.add_argument("--imap-port", help="IMAP server port", default=os.getenv("IMAP_PORT"))
+    imap.add_argument(
+        "--imap-host", help="IMAP server hostname", default=os.getenv("IMAP_HOST")
+    )
+    imap.add_argument(
+        "--imap-port", help="IMAP server port", default=os.getenv("IMAP_PORT")
+    )
     imap.add_argument(
         "--imap-username",
         help="IMAP server username",
         default=os.getenv("IMAP_USERNAME"),
     )
     imap.add_argument(
         "--imap-password",
         help="IMAP server password",
         default=os.getenv("IMAP_PASSWORD"),
     )
     smtp = email.add_argument_group("SMTP")
-    smtp.add_argument("--smtp-host", help="SMTP server hostname", default=os.getenv("SMTP_HOST"))
-    smtp.add_argument("--smtp-port", help="SMTP server port", default=os.getenv("SMTP_PORT"))
+    smtp.add_argument(
+        "--smtp-host", help="SMTP server hostname", default=os.getenv("SMTP_HOST")
+    )
+    smtp.add_argument(
+        "--smtp-port", help="SMTP server port", default=os.getenv("SMTP_PORT")
+    )
     smtp.add_argument(
         "--smtp-username",
         help="SMTP server username",
         default=os.getenv("SMTP_USERNAME"),
     )
     smtp.add_argument(
         "--smtp-password",
         help="SMTP server password",
         default=os.getenv("SMTP_PASSWORD"),
     )
     smtp.add_argument(
         "--message-id-domain",
         help="Domain to use for Message-ID header",
-        default=os.getenv("MESSAGE_ID_DOMAIN") if os.getenv("MESSAGE_ID_DOMAIN") else None,
+        default=(
+            os.getenv("MESSAGE_ID_DOMAIN") if os.getenv("MESSAGE_ID_DOMAIN") else None
+        ),
     )
 
     check_required_args(
         [
             "imap_host",
             "imap_port",
             "imap_username",
```

### Comparing `llmail-0.2.3/pyproject.toml` & `llmail-0.2.4/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 [tool.poetry]
 name = "llmail"
-version = "0.2.3"
+version = "0.2.4"
 description = "Interact with LLMs via email"
 authors = ["slashtechno <77907286+slashtechno@users.noreply.github.com>"]
 repository = "https://github.com/slashtechno/llmail"
 keywords = ["llm", "email", "ai", "openai"]
 license = "GNU Affero General Public License v3"
 readme = "README.md"
 
 [tool.poetry.dependencies]
-python = "^3.11"
+python = ">=3.10.0,<4.0.0"
 loguru = "^0.7.2"
 python-dotenv = "^1.0.1"
 imapclient = "^3.0.1"
 icecream = "^2.1.3"
 yagmail = {extras = ["all"], version = "^0.15.293"}
 html2text = "^2024.2.26"
 openai = "^1.25.1"
```

### Comparing `llmail-0.2.3/PKG-INFO` & `llmail-0.2.4/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: llmail
-Version: 0.2.3
+Version: 0.2.4
 Summary: Interact with LLMs via email
 Home-page: https://github.com/slashtechno/llmail
 License: GNU Affero General Public License v3
 Keywords: llm,email,ai,openai
 Author: slashtechno
 Author-email: 77907286+slashtechno@users.noreply.github.com
-Requires-Python: >=3.11,<4.0
+Requires-Python: >=3.10.0,<4.0.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: html2text (>=2024.2.26,<2025.0.0)
 Requires-Dist: icecream (>=2.1.3,<3.0.0)
 Requires-Dist: imapclient (>=3.0.1,<4.0.0)
 Requires-Dist: loguru (>=0.7.2,<0.8.0)
 Requires-Dist: openai (>=1.25.1,<2.0.0)
```

