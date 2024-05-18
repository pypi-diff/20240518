# Comparing `tmp/email_draft_generator-0.0.1.tar.gz` & `tmp/email_draft_generator-0.0.2.tar.gz`

## Comparing `email_draft_generator-0.0.1.tar` & `email_draft_generator-0.0.2.tar`

### file list

```diff
@@ -1,19 +1,24 @@
--rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 email_draft_generator-0.0.1/.editorconfig
--rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 email_draft_generator-0.0.1/email-template.txt
--rwxr-xr-x   0        0        0      185 2020-02-02 00:00:00.000000 email_draft_generator-0.0.1/run.sh
--rwxr-xr-x   0        0        0      247 2020-02-02 00:00:00.000000 email_draft_generator-0.0.1/setup.sh
--rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 email_draft_generator-0.0.1/test_data.csv
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 email_draft_generator-0.0.1/src/email_draft_generator/__init__.py
--rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 email_draft_generator-0.0.1/src/email_draft_generator/__main__.py
--rw-r--r--   0        0        0      972 2020-02-02 00:00:00.000000 email_draft_generator-0.0.1/src/email_draft_generator/email_creator.py
--rw-r--r--   0        0        0     2178 2020-02-02 00:00:00.000000 email_draft_generator-0.0.1/src/email_draft_generator/gmail.py
--rw-r--r--   0        0        0      420 2020-02-02 00:00:00.000000 email_draft_generator-0.0.1/src/email_draft_generator/mail_util.py
--rw-r--r--   0        0        0     1235 2020-02-02 00:00:00.000000 email_draft_generator-0.0.1/src/email_draft_generator/main.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 email_draft_generator-0.0.1/src/email_draft_generator/file_parser/__init__.py
--rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 email_draft_generator-0.0.1/src/email_draft_generator/file_parser/__main__.py
--rw-r--r--   0        0        0      797 2020-02-02 00:00:00.000000 email_draft_generator-0.0.1/src/email_draft_generator/file_parser/main.py
--rw-r--r--   0        0        0     3204 2020-02-02 00:00:00.000000 email_draft_generator-0.0.1/.gitignore
--rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 email_draft_generator-0.0.1/LICENSE
--rw-r--r--   0        0        0     1623 2020-02-02 00:00:00.000000 email_draft_generator-0.0.1/README.md
--rw-r--r--   0        0        0     1853 2020-02-02 00:00:00.000000 email_draft_generator-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     3960 2020-02-02 00:00:00.000000 email_draft_generator-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 email_draft_generator-0.0.2/.editorconfig
+-rwxr-xr-x   0        0        0      186 2020-02-02 00:00:00.000000 email_draft_generator-0.0.2/run.sh
+-rwxr-xr-x   0        0        0      247 2020-02-02 00:00:00.000000 email_draft_generator-0.0.2/setup.sh
+-rw-r--r--   0        0        0      686 2020-02-02 00:00:00.000000 email_draft_generator-0.0.2/.github/workflows/python-build.yml
+-rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 email_draft_generator-0.0.2/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 email_draft_generator-0.0.2/data/email-list.csv
+-rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 email_draft_generator-0.0.2/data/email-list.txt
+-rw-r--r--   0        0        0      288 2020-02-02 00:00:00.000000 email_draft_generator-0.0.2/data/template.json
+-rw-r--r--   0        0        0    13503 2020-02-02 00:00:00.000000 email_draft_generator-0.0.2/data/test_image.png
+-rw-r--r--   0        0        0    12586 2020-02-02 00:00:00.000000 email_draft_generator-0.0.2/data/test_pdf.pdf
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 email_draft_generator-0.0.2/src/email_draft_generator/__init__.py
+-rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 email_draft_generator-0.0.2/src/email_draft_generator/__main__.py
+-rw-r--r--   0        0        0      852 2020-02-02 00:00:00.000000 email_draft_generator-0.0.2/src/email_draft_generator/email_creator.py
+-rw-r--r--   0        0        0     2178 2020-02-02 00:00:00.000000 email_draft_generator-0.0.2/src/email_draft_generator/gmail.py
+-rw-r--r--   0        0        0      420 2020-02-02 00:00:00.000000 email_draft_generator-0.0.2/src/email_draft_generator/mail_util.py
+-rw-r--r--   0        0        0     1831 2020-02-02 00:00:00.000000 email_draft_generator-0.0.2/src/email_draft_generator/main.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 email_draft_generator-0.0.2/src/email_draft_generator/file_parser/__init__.py
+-rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 email_draft_generator-0.0.2/src/email_draft_generator/file_parser/__main__.py
+-rw-r--r--   0        0        0      796 2020-02-02 00:00:00.000000 email_draft_generator-0.0.2/src/email_draft_generator/file_parser/main.py
+-rw-r--r--   0        0        0     3204 2020-02-02 00:00:00.000000 email_draft_generator-0.0.2/.gitignore
+-rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 email_draft_generator-0.0.2/LICENSE
+-rw-r--r--   0        0        0     1981 2020-02-02 00:00:00.000000 email_draft_generator-0.0.2/README.md
+-rw-r--r--   0        0        0     1853 2020-02-02 00:00:00.000000 email_draft_generator-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     4318 2020-02-02 00:00:00.000000 email_draft_generator-0.0.2/PKG-INFO
```

### Comparing `email_draft_generator-0.0.1/src/email_draft_generator/email_creator.py` & `email_draft_generator-0.0.2/src/email_draft_generator/email_creator.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,29 +1,23 @@
 import base64
 from email.message import EmailMessage
 
-def create_email_body(company, attachments):
-	"""Generates an E-mail with the provided company name and attachments"""
+def create_email_body(template, company, attachments):
+	"""Generates an E-mail with the provided template, company data, and attachments"""
 	mime_message = EmailMessage()
 
-	# headers
-	# TODO: Pull these from a configuration file
+	# Add headers
 	mime_message["To"] = company['email']
 	# Doesn't seem to be required for Gmail
 	# mime_message["From"] = ""
-	mime_message["Subject"] = "sample with attachment"
+	if 'subject' in template:
+		mime_message["Subject"] = str(template['subject']).format_map(company)
 
-	# text
-	mime_message.set_content(f"""Dear {company['name']},
-
-We are pleased to inform you that your company has been selected for a special offer.
-Please find attached the details of the offer.
-
-Best regards,
-Your Company""")
+	# Add text
+	mime_message.set_content(str(template['body']).format_map(company))
 
 	# Add attachments
 	for attachment in attachments:
 		mime_message.add_attachment(attachment['data'], maintype=attachment['maintype'], subtype=attachment['subtype'], filename=attachment['name'])
 
 	encoded_message = base64.urlsafe_b64encode(mime_message.as_bytes()).decode()
```

### Comparing `email_draft_generator-0.0.1/src/email_draft_generator/gmail.py` & `email_draft_generator-0.0.2/src/email_draft_generator/gmail.py`

 * *Files identical despite different names*

### Comparing `email_draft_generator-0.0.1/src/email_draft_generator/file_parser/main.py` & `email_draft_generator-0.0.2/src/email_draft_generator/file_parser/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,13 +21,13 @@
 			chars.append(char)
 		lines = ''.join(chars).split('\n')
 		companies = []
 		with concurrent.futures.ProcessPoolExecutor() as executor:
 			for i in range(0, len(lines), 2):
 				companies.append({
 					'name': lines[i].strip(),
-						'email': lines[i+1].strip()
+					'email': lines[i+1].strip()
 				})
 	except:
 		raise ValueError("Invalid input file")
 
 	json.dump(companies, sys.stdout, indent="\t")
```

### Comparing `email_draft_generator-0.0.1/.gitignore` & `email_draft_generator-0.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `email_draft_generator-0.0.1/LICENSE` & `email_draft_generator-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `email_draft_generator-0.0.1/README.md` & `email_draft_generator-0.0.2/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,26 +1,37 @@
 # Email Generator
 
 ## Installation
 Download the latest release as a `tar.gz` file.
 
 ## Setup
+### Build program
+Run `setup.sh` (can be run by simply double-clicking on the file).
+
 ### Set up the Google API
 Follow the guide at https://developers.google.com/gmail/api/quickstart/python#set_up_your_environment to generate OAuth2 credentials, and, when you are at the step to configure the OAuth consent screen, add the `gmail.compose` scope so the script can edit drafts. Download them into `.credentials/credentials.json` (you will have to create this directory yourself, and show hidden files to see it on MacOS).
+
 ### Set up the template
-- update the email template in `email_generator/email_creator.py`
-- put the file paths to any attachments in the `attachment_paths` list in `email_generator/main.py`
-### Build program
-Run `setup.sh` (can be run by simply double-clicking on the file)
-If you make any changes to the template after this, run `setup.sh` again.
+Update the email template in `data/template.json`.
+
+#### Template Format
+| Key                      | Value                                            |
+|--------------------------|--------------------------------------------------|
+| `subject` (formatted)    | E-mail subject                                   |
+| `body` (formatted)       | E-mail body                                      |
+| `attachments` (optional) | Paths to any attachments that should be included |
+
+Formatted fields can include the following variables
+| Variable  | Data           |
+|-----------|----------------|
+| `{name}`  | Company name   |
+| `{email}` | Company E-mail |
 
 ## Usage
 ### Prepare data
-- copy and paste the table into `email-template.txt`
-- make sure there is nothing else in the file
-- save it
+Copy and paste the table into `data/email-list.txt`.
 ### Run the program
 Run `run.sh` (can be run by double-clicking as well)
 The first time it is run, you will need to authenticate with the account that you want to upload the drafts to. A browser window should be opened automatically to do this in (if it is not, copy and paste the URL from the terminal window into your browser). The authentication flow may not work in Firefox or other Gecko-based browsers, so try Chrome, Safari, or another Chromium- or Webkit-based browser if it doesn't work for you.
 
 ## Building from source
 Install the `build` tool with pip and run `python3 -m build` to build the package.
```

### Comparing `email_draft_generator-0.0.1/pyproject.toml` & `email_draft_generator-0.0.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "email_draft_generator"
-version = "0.0.1"
+version = "0.0.2"
 description = "A utility to generate E-mail drafts from a list of E-mail addresses."
 readme = "README.md"
 license = {file = "LICENSE"}
 requires-python = ">=3.8"
 keywords = ["email", "gmail", "email-template", "email-generator"]
 
 # This should be your name or the name of the organization who originally authored the project, and a valid email address corresponding to the name listed.
```

### Comparing `email_draft_generator-0.0.1/PKG-INFO` & `email_draft_generator-0.0.2/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: email_draft_generator
-Version: 0.0.1
+Version: 0.0.2
 Summary: A utility to generate E-mail drafts from a list of E-mail addresses.
 Project-URL: Homepage, https://github.com/fodfodfod/Email-Generator
 Project-URL: Bug Reports, https://github.com/fodfodfod/Email-Generator/issues
 Project-URL: Source, https://github.com/fodfodfod/Email-Generator
 Author-email: Brandon Clague <94200657+fodfodfod@users.noreply.github.com>, Max Nargang <CoffeeCoder1@outlook.com>
 Maintainer-email: Brandon Clague <94200657+fodfodfod@users.noreply.github.com>, Max Nargang <CoffeeCoder1@outlook.com>
 License: MIT License
@@ -43,27 +43,38 @@
 
 # Email Generator
 
 ## Installation
 Download the latest release as a `tar.gz` file.
 
 ## Setup
+### Build program
+Run `setup.sh` (can be run by simply double-clicking on the file).
+
 ### Set up the Google API
 Follow the guide at https://developers.google.com/gmail/api/quickstart/python#set_up_your_environment to generate OAuth2 credentials, and, when you are at the step to configure the OAuth consent screen, add the `gmail.compose` scope so the script can edit drafts. Download them into `.credentials/credentials.json` (you will have to create this directory yourself, and show hidden files to see it on MacOS).
+
 ### Set up the template
-- update the email template in `email_generator/email_creator.py`
-- put the file paths to any attachments in the `attachment_paths` list in `email_generator/main.py`
-### Build program
-Run `setup.sh` (can be run by simply double-clicking on the file)
-If you make any changes to the template after this, run `setup.sh` again.
+Update the email template in `data/template.json`.
+
+#### Template Format
+| Key                      | Value                                            |
+|--------------------------|--------------------------------------------------|
+| `subject` (formatted)    | E-mail subject                                   |
+| `body` (formatted)       | E-mail body                                      |
+| `attachments` (optional) | Paths to any attachments that should be included |
+
+Formatted fields can include the following variables
+| Variable  | Data           |
+|-----------|----------------|
+| `{name}`  | Company name   |
+| `{email}` | Company E-mail |
 
 ## Usage
 ### Prepare data
-- copy and paste the table into `email-template.txt`
-- make sure there is nothing else in the file
-- save it
+Copy and paste the table into `data/email-list.txt`.
 ### Run the program
 Run `run.sh` (can be run by double-clicking as well)
 The first time it is run, you will need to authenticate with the account that you want to upload the drafts to. A browser window should be opened automatically to do this in (if it is not, copy and paste the URL from the terminal window into your browser). The authentication flow may not work in Firefox or other Gecko-based browsers, so try Chrome, Safari, or another Chromium- or Webkit-based browser if it doesn't work for you.
 
 ## Building from source
 Install the `build` tool with pip and run `python3 -m build` to build the package.
```

