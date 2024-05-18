# Comparing `tmp/docmake-0.1.3.tar.gz` & `tmp/docmake-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "docmake-0.1.3.tar", max compression
+gzip compressed data, was "docmake-0.1.4.tar", max compression
```

## Comparing `docmake-0.1.3.tar` & `docmake-0.1.4.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rwxr-xr-x   0        0        0    11358 2024-05-13 15:11:36.044304 docmake-0.1.3/LICENSE
--rwxr-xr-x   0        0        0     3953 2024-05-13 16:01:03.066258 docmake-0.1.3/README.md
--rwxr-xr-x   0        0        0      421 2024-05-13 16:06:20.232819 docmake-0.1.3/pyproject.toml
--rwxr-xr-x   0        0        0        0 2024-05-13 15:24:15.859574 docmake-0.1.3/src/__init__.py
--rwxr-xr-x   0        0        0    31507 2024-05-13 04:44:25.185511 docmake-0.1.3/src/app.py
--rw-r--r--   0        0        0     4469 1970-01-01 00:00:00.000000 docmake-0.1.3/PKG-INFO
+-rwxr-xr-x   0        0        0    11358 2024-05-13 15:11:36.044304 docmake-0.1.4/LICENSE
+-rwxr-xr-x   0        0        0     3953 2024-05-13 16:01:03.066258 docmake-0.1.4/README.md
+-rwxr-xr-x   0        0        0      421 2024-05-18 03:58:31.013203 docmake-0.1.4/pyproject.toml
+-rwxr-xr-x   0        0        0        0 2024-05-13 15:24:15.859574 docmake-0.1.4/src/__init__.py
+-rwxr-xr-x   0        0        0    31385 2024-05-18 03:54:45.639907 docmake-0.1.4/src/app.py
+-rw-r--r--   0        0        0     4469 1970-01-01 00:00:00.000000 docmake-0.1.4/PKG-INFO
```

### Comparing `docmake-0.1.3/LICENSE` & `docmake-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `docmake-0.1.3/README.md` & `docmake-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `docmake-0.1.3/src/app.py` & `docmake-0.1.4/src/app.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 import asyncio
 import uuid
 import argparse
 import mimetypes
 import qrcode
 from bs4 import BeautifulSoup
 from pyppeteer import launch
-from pypdf import PdfMerger, PdfWriter, PdfReader
+from pypdf import PdfWriter, PdfReader
 from io import BytesIO
 from Cryptodome.Hash import SHA256
 
 
 def generate_password(length=8):
     characters = string.ascii_letters + string.digits + string.punctuation
     password = ''.join(random.choice(characters) for _ in range(length))
@@ -36,15 +36,15 @@
 
 def hash_password(password, salt):
     key = SHA256.new(password.encode('utf-8') + salt).digest()
     return key
 
 def merge_pdfs(output_file, input_files):
     try:
-        merger = PdfMerger()
+        merger = PdfWriter()
         for file in input_files:
             merger.append(file)
         with open(output_file, 'wb') as merged_pdf:
             merger.write(merged_pdf)
         print('[SUCCESS] Merge operation completed.')
     except Exception as e:
         print(e)
@@ -244,15 +244,15 @@
     os.chdir(html_dir)
     browser = await launch(
         args=[
         '--headless',
         ]
     )
     page = await browser.newPage()
-    merger = PdfMerger()
+    merger = PdfWriter()
 
     md = MarkdownIt()
     try:
         for index, input_file in enumerate(input_files):
             temp_html_file = f'{tmp_file}.html'
             if input_file.lower().endswith(".md"):
                 with open(input_file, "r", encoding="utf-8") as file:
@@ -722,26 +722,24 @@
         for key, value in params.items():
             print(f'{key}: {value}')
         print('---')
 
     if args.input:
         ts, tmp_dir = Interface.get_tempdir()
         tmp_dir = f'{tmp_dir}/{ts}'
-        tmp_file = f'{tmp_dir}/{ts}'
+        tmp_file = f'{tmp_dir}/{ts}' #TODO
         os.makedirs(tmp_dir, exist_ok=True)
 
         input_files = parse_input(args.input)
         processing_files = []
 
         if args.output:
             result_file = os.path.abspath(args.output)
         else:
-            base = os.path.splitext(os.path.basename(file))[0] + f'.pdf'
-            abspath_dir = os.path.abspath(base)
-            result_file = os.path.join(abspath_dir, base)
+            result_file = os.path.join(tmp_dir, 'output.pdf')
             print(f'[INFO] Output will: {result_file}')
 
         for index, file in enumerate(input_files):
             mime_type, _ = mimetypes.guess_type(file)
             if mime_type and mime_type.startswith('application'):
                 processing_files.append(result_file)
             elif mime_type and mime_type.startswith('text'):
```

### Comparing `docmake-0.1.3/PKG-INFO` & `docmake-0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: docmake
-Version: 0.1.3
+Version: 0.1.4
 Summary: Generate pdf files from other format documents.
 Home-page: https://github.com/morisono/docmaker_webui
 Author: admin
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

