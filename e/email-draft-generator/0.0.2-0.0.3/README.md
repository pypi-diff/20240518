# Comparing `tmp/email_draft_generator-0.0.2.tar.gz` & `tmp/email_draft_generator-0.0.3.tar.gz`

## Comparing `email_draft_generator-0.0.2.tar` & `email_draft_generator-0.0.3.tar`

### file list

```diff
@@ -1,24 +1,23 @@
--rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 email_draft_generator-0.0.2/.editorconfig
--rwxr-xr-x   0        0        0      186 2020-02-02 00:00:00.000000 email_draft_generator-0.0.2/run.sh
--rwxr-xr-x   0        0        0      247 2020-02-02 00:00:00.000000 email_draft_generator-0.0.2/setup.sh
--rw-r--r--   0        0        0      686 2020-02-02 00:00:00.000000 email_draft_generator-0.0.2/.github/workflows/python-build.yml
--rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 email_draft_generator-0.0.2/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 email_draft_generator-0.0.2/data/email-list.csv
--rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 email_draft_generator-0.0.2/data/email-list.txt
--rw-r--r--   0        0        0      288 2020-02-02 00:00:00.000000 email_draft_generator-0.0.2/data/template.json
--rw-r--r--   0        0        0    13503 2020-02-02 00:00:00.000000 email_draft_generator-0.0.2/data/test_image.png
--rw-r--r--   0        0        0    12586 2020-02-02 00:00:00.000000 email_draft_generator-0.0.2/data/test_pdf.pdf
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 email_draft_generator-0.0.2/src/email_draft_generator/__init__.py
--rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 email_draft_generator-0.0.2/src/email_draft_generator/__main__.py
--rw-r--r--   0        0        0      852 2020-02-02 00:00:00.000000 email_draft_generator-0.0.2/src/email_draft_generator/email_creator.py
--rw-r--r--   0        0        0     2178 2020-02-02 00:00:00.000000 email_draft_generator-0.0.2/src/email_draft_generator/gmail.py
--rw-r--r--   0        0        0      420 2020-02-02 00:00:00.000000 email_draft_generator-0.0.2/src/email_draft_generator/mail_util.py
--rw-r--r--   0        0        0     1831 2020-02-02 00:00:00.000000 email_draft_generator-0.0.2/src/email_draft_generator/main.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 email_draft_generator-0.0.2/src/email_draft_generator/file_parser/__init__.py
--rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 email_draft_generator-0.0.2/src/email_draft_generator/file_parser/__main__.py
--rw-r--r--   0        0        0      796 2020-02-02 00:00:00.000000 email_draft_generator-0.0.2/src/email_draft_generator/file_parser/main.py
--rw-r--r--   0        0        0     3204 2020-02-02 00:00:00.000000 email_draft_generator-0.0.2/.gitignore
--rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 email_draft_generator-0.0.2/LICENSE
--rw-r--r--   0        0        0     1981 2020-02-02 00:00:00.000000 email_draft_generator-0.0.2/README.md
--rw-r--r--   0        0        0     1853 2020-02-02 00:00:00.000000 email_draft_generator-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     4318 2020-02-02 00:00:00.000000 email_draft_generator-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 email_draft_generator-0.0.3/.editorconfig
+-rwxr-xr-x   0        0        0      240 2020-02-02 00:00:00.000000 email_draft_generator-0.0.3/run.sh
+-rwxr-xr-x   0        0        0      247 2020-02-02 00:00:00.000000 email_draft_generator-0.0.3/setup.sh
+-rw-r--r--   0        0        0     1686 2020-02-02 00:00:00.000000 email_draft_generator-0.0.3/.github/workflows/python-build.yml
+-rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 email_draft_generator-0.0.3/data/email-list.csv
+-rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 email_draft_generator-0.0.3/data/email-list.txt
+-rw-r--r--   0        0        0      288 2020-02-02 00:00:00.000000 email_draft_generator-0.0.3/data/template.json
+-rw-r--r--   0        0        0    13503 2020-02-02 00:00:00.000000 email_draft_generator-0.0.3/data/test_image.png
+-rw-r--r--   0        0        0    12586 2020-02-02 00:00:00.000000 email_draft_generator-0.0.3/data/test_pdf.pdf
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 email_draft_generator-0.0.3/src/email_draft_generator/__init__.py
+-rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 email_draft_generator-0.0.3/src/email_draft_generator/__main__.py
+-rw-r--r--   0        0        0      852 2020-02-02 00:00:00.000000 email_draft_generator-0.0.3/src/email_draft_generator/email_creator.py
+-rw-r--r--   0        0        0     2621 2020-02-02 00:00:00.000000 email_draft_generator-0.0.3/src/email_draft_generator/gmail.py
+-rw-r--r--   0        0        0      420 2020-02-02 00:00:00.000000 email_draft_generator-0.0.3/src/email_draft_generator/mail_util.py
+-rw-r--r--   0        0        0     2040 2020-02-02 00:00:00.000000 email_draft_generator-0.0.3/src/email_draft_generator/main.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 email_draft_generator-0.0.3/src/email_draft_generator/file_parser/__init__.py
+-rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 email_draft_generator-0.0.3/src/email_draft_generator/file_parser/__main__.py
+-rw-r--r--   0        0        0      796 2020-02-02 00:00:00.000000 email_draft_generator-0.0.3/src/email_draft_generator/file_parser/main.py
+-rw-r--r--   0        0        0     3204 2020-02-02 00:00:00.000000 email_draft_generator-0.0.3/.gitignore
+-rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 email_draft_generator-0.0.3/LICENSE
+-rw-r--r--   0        0        0     1981 2020-02-02 00:00:00.000000 email_draft_generator-0.0.3/README.md
+-rw-r--r--   0        0        0     1853 2020-02-02 00:00:00.000000 email_draft_generator-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     4318 2020-02-02 00:00:00.000000 email_draft_generator-0.0.3/PKG-INFO
```

### Comparing `email_draft_generator-0.0.2/data/test_image.png` & `email_draft_generator-0.0.3/data/test_image.png`

 * *Files identical despite different names*

### Comparing `email_draft_generator-0.0.2/data/test_pdf.pdf` & `email_draft_generator-0.0.3/data/test_pdf.pdf`

 * *Files identical despite different names*

### Comparing `email_draft_generator-0.0.2/src/email_draft_generator/email_creator.py` & `email_draft_generator-0.0.3/src/email_draft_generator/email_creator.py`

 * *Files identical despite different names*

### Comparing `email_draft_generator-0.0.2/src/email_draft_generator/gmail.py` & `email_draft_generator-0.0.3/src/email_draft_generator/gmail.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import os
+from pathlib import Path
 from google.auth.transport.requests import Request
 from google.oauth2.credentials import Credentials
 from google_auth_oauthlib.flow import InstalledAppFlow
 from googleapiclient.discovery import build
 from googleapiclient.errors import HttpError
 
 # If modifying these scopes, delete the file token.json.
@@ -19,19 +20,32 @@
 		# Refresh expired creds
 		if creds and creds.expired and creds.refresh_token:
 			creds.refresh(Request())
 		# Create new creds
 		else:
 			# If OAuth2 creds do not exist, tell the user to create them
 			if not os.path.exists(creds_path):
-				raise FileNotFoundError(f"No OAuth2 Credentials exist! Follow the guide at https://developers.google.com/gmail/api/quickstart/python#set_up_your_environment to create them, and, when you are at the step to configure the OAuth consent screen, add the `gmail.compose` scope. Download them into `.credentials/credentials.json`, and re-launch the program.")
-			# If they do, create an OAuth flow
+				creds_path_input = input("No OAuth2 Credentials exist!\nFollow the guide at https://developers.google.com/gmail/api/quickstart/python#set_up_your_environment to create them, and, when you are at the step to configure the OAuth consent screen, add the `gmail.compose` scope.\nDownload them to your device, copy the file path, and enter it here: ")
+
+				input_path = Path(creds_path_input)
+				with open(input_path, "r") as creds_input:
+					oauth_creds = creds_input.read()
+
+				flow = InstalledAppFlow.from_client_secrets_file(creds_path_input, SCOPES)
+
+				output_path = Path(creds_path)
+				output_path.parent.mkdir(parents=True, exist_ok=True)
+				with open(creds_path, "w") as creds_output:
+					creds_output.write(oauth_creds)
+
+				input_path.unlink(missing_ok=True)
 			else:
+				# If they do, create an OAuth flow
 				flow = InstalledAppFlow.from_client_secrets_file(creds_path, SCOPES)
-				creds = flow.run_local_server(port=0)
+			creds = flow.run_local_server(port=0)
 		# Save the credentials for the next run
 		with open(token_path, "w") as token:
 			token.write(creds.to_json())
 
 	return creds
 
 def create_draft(creds, body):
```

### Comparing `email_draft_generator-0.0.2/src/email_draft_generator/file_parser/main.py` & `email_draft_generator-0.0.3/src/email_draft_generator/file_parser/main.py`

 * *Files identical despite different names*

### Comparing `email_draft_generator-0.0.2/.gitignore` & `email_draft_generator-0.0.3/.gitignore`

 * *Files identical despite different names*

### Comparing `email_draft_generator-0.0.2/LICENSE` & `email_draft_generator-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `email_draft_generator-0.0.2/README.md` & `email_draft_generator-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `email_draft_generator-0.0.2/pyproject.toml` & `email_draft_generator-0.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "email_draft_generator"
-version = "0.0.2"
+version = "0.0.3"
 description = "A utility to generate E-mail drafts from a list of E-mail addresses."
 readme = "README.md"
 license = {file = "LICENSE"}
 requires-python = ">=3.8"
 keywords = ["email", "gmail", "email-template", "email-generator"]
 
 # This should be your name or the name of the organization who originally authored the project, and a valid email address corresponding to the name listed.
```

### Comparing `email_draft_generator-0.0.2/PKG-INFO` & `email_draft_generator-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: email_draft_generator
-Version: 0.0.2
+Version: 0.0.3
 Summary: A utility to generate E-mail drafts from a list of E-mail addresses.
 Project-URL: Homepage, https://github.com/fodfodfod/Email-Generator
 Project-URL: Bug Reports, https://github.com/fodfodfod/Email-Generator/issues
 Project-URL: Source, https://github.com/fodfodfod/Email-Generator
 Author-email: Brandon Clague <94200657+fodfodfod@users.noreply.github.com>, Max Nargang <CoffeeCoder1@outlook.com>
 Maintainer-email: Brandon Clague <94200657+fodfodfod@users.noreply.github.com>, Max Nargang <CoffeeCoder1@outlook.com>
 License: MIT License
```

