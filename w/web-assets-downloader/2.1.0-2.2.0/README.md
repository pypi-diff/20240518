# Comparing `tmp/web_assets_downloader-2.1.0.tar.gz` & `tmp/web_assets_downloader-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "web_assets_downloader-2.1.0.tar", last modified: Fri May 17 09:34:09 2024, max compression
+gzip compressed data, was "web_assets_downloader-2.2.0.tar", last modified: Sat May 18 13:27:24 2024, max compression
```

## Comparing `web_assets_downloader-2.1.0.tar` & `web_assets_downloader-2.2.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxr-x   0 arif      (1000) arif      (1000)        0 2024-05-17 09:34:09.832431 web_assets_downloader-2.1.0/
--rw-rw-r--   0 arif      (1000) arif      (1000)      957 2024-05-17 09:34:09.832431 web_assets_downloader-2.1.0/PKG-INFO
--rw-rw-r--   0 arif      (1000) arif      (1000)       38 2024-05-17 09:34:09.832431 web_assets_downloader-2.1.0/setup.cfg
--rw-rw-r--   0 arif      (1000) arif      (1000)     1543 2024-05-17 09:30:22.000000 web_assets_downloader-2.1.0/setup.py
-drwxrwxr-x   0 arif      (1000) arif      (1000)        0 2024-05-17 09:34:09.832431 web_assets_downloader-2.1.0/web_assets_downloader/
--rw-rw-r--   0 arif      (1000) arif      (1000)      141 2024-03-03 10:53:55.000000 web_assets_downloader-2.1.0/web_assets_downloader/__init__.py
--rw-rw-r--   0 arif      (1000) arif      (1000)     4757 2024-05-17 09:29:02.000000 web_assets_downloader-2.1.0/web_assets_downloader/web_assets_downloader.py
-drwxrwxr-x   0 arif      (1000) arif      (1000)        0 2024-05-17 09:34:09.832431 web_assets_downloader-2.1.0/web_assets_downloader.egg-info/
--rw-rw-r--   0 arif      (1000) arif      (1000)      957 2024-05-17 09:34:09.000000 web_assets_downloader-2.1.0/web_assets_downloader.egg-info/PKG-INFO
--rw-rw-r--   0 arif      (1000) arif      (1000)      361 2024-05-17 09:34:09.000000 web_assets_downloader-2.1.0/web_assets_downloader.egg-info/SOURCES.txt
--rw-rw-r--   0 arif      (1000) arif      (1000)       88 2024-05-17 09:34:09.000000 web_assets_downloader-2.1.0/web_assets_downloader.egg-info/dependency_links.txt
--rw-rw-r--   0 arif      (1000) arif      (1000)       81 2024-05-17 09:34:09.000000 web_assets_downloader-2.1.0/web_assets_downloader.egg-info/entry_points.txt
--rw-rw-r--   0 arif      (1000) arif      (1000)       59 2024-05-17 09:34:09.000000 web_assets_downloader-2.1.0/web_assets_downloader.egg-info/requires.txt
--rw-rw-r--   0 arif      (1000) arif      (1000)       22 2024-05-17 09:34:09.000000 web_assets_downloader-2.1.0/web_assets_downloader.egg-info/top_level.txt
+drwxrwxr-x   0 arif      (1000) arif      (1000)        0 2024-05-18 13:27:24.301190 web_assets_downloader-2.2.0/
+-rw-rw-r--   0 arif      (1000) arif      (1000)      957 2024-05-18 13:27:24.301190 web_assets_downloader-2.2.0/PKG-INFO
+-rw-rw-r--   0 arif      (1000) arif      (1000)       38 2024-05-18 13:27:24.301190 web_assets_downloader-2.2.0/setup.cfg
+-rw-rw-r--   0 arif      (1000) arif      (1000)     1543 2024-05-18 13:27:19.000000 web_assets_downloader-2.2.0/setup.py
+drwxrwxr-x   0 arif      (1000) arif      (1000)        0 2024-05-18 13:27:24.297191 web_assets_downloader-2.2.0/web_assets_downloader/
+-rw-rw-r--   0 arif      (1000) arif      (1000)      141 2024-03-03 10:53:55.000000 web_assets_downloader-2.2.0/web_assets_downloader/__init__.py
+-rw-rw-r--   0 arif      (1000) arif      (1000)     4925 2024-05-18 13:24:17.000000 web_assets_downloader-2.2.0/web_assets_downloader/web_assets_downloader.py
+drwxrwxr-x   0 arif      (1000) arif      (1000)        0 2024-05-18 13:27:24.301190 web_assets_downloader-2.2.0/web_assets_downloader.egg-info/
+-rw-rw-r--   0 arif      (1000) arif      (1000)      957 2024-05-18 13:27:24.000000 web_assets_downloader-2.2.0/web_assets_downloader.egg-info/PKG-INFO
+-rw-rw-r--   0 arif      (1000) arif      (1000)      361 2024-05-18 13:27:24.000000 web_assets_downloader-2.2.0/web_assets_downloader.egg-info/SOURCES.txt
+-rw-rw-r--   0 arif      (1000) arif      (1000)       88 2024-05-18 13:27:24.000000 web_assets_downloader-2.2.0/web_assets_downloader.egg-info/dependency_links.txt
+-rw-rw-r--   0 arif      (1000) arif      (1000)       81 2024-05-18 13:27:24.000000 web_assets_downloader-2.2.0/web_assets_downloader.egg-info/entry_points.txt
+-rw-rw-r--   0 arif      (1000) arif      (1000)       59 2024-05-18 13:27:24.000000 web_assets_downloader-2.2.0/web_assets_downloader.egg-info/requires.txt
+-rw-rw-r--   0 arif      (1000) arif      (1000)       22 2024-05-18 13:27:24.000000 web_assets_downloader-2.2.0/web_assets_downloader.egg-info/top_level.txt
```

### Comparing `web_assets_downloader-2.1.0/PKG-INFO` & `web_assets_downloader-2.2.0/web_assets_downloader.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: web_assets_downloader
-Version: 2.1.0
+Name: web-assets-downloader
+Version: 2.2.0
 Summary: A package for downloading web content and assets
 Home-page: https://github.com/arif-x/web-assets-downloader
 Author: Ariffudin
 Author-email: sudo.ariffudin@email.com
 License: MIT
 Project-URL: Source, https://github.com/arif-x/web-assets-downloader
 Project-URL: Source Code, https://github.com/arif-x/web-assets-downloader
```

### Comparing `web_assets_downloader-2.1.0/setup.py` & `web_assets_downloader-2.2.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='web_assets_downloader',
-    version='2.1.0',
+    version='2.2.0',
     packages=find_packages(),
     install_requires=[
         'requests',
         'beautifulsoup4',
         'pillow',
         'PyPDF2',
         'python-docx',
```

### Comparing `web_assets_downloader-2.1.0/web_assets_downloader/web_assets_downloader.py` & `web_assets_downloader-2.2.0/web_assets_downloader/web_assets_downloader.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from bs4 import BeautifulSoup
 from urllib.parse import urljoin, unquote
 from PIL import Image
 import PyPDF2
 from docx import Document
 from openpyxl import load_workbook
 
-def download_asset(asset_urls, save_folder, headers):
+def download_asset(asset_urls, save_folder, headers, img=True, pdf=True, doc=True, xlx=True):
     for url in asset_urls:
         print(url)
         response = requests.get(url, headers=headers)
         if response.status_code == 200:
             # Parse the asset URL to extract the path
             parsed_url = urlparse(url)
             asset_path = unquote(parsed_url.path)
@@ -24,29 +24,33 @@
             os.makedirs(os.path.dirname(asset_filepath), exist_ok=True)
 
             # Download the asset
             with open(asset_filepath, 'wb') as f:
                 f.write(response.content)
                 print(f"Downloaded {asset_path}.")
 
-            # Resize images if it's an image file
-            if asset_path.lower().endswith(('.png', '.jpg', '.jpeg', '.gif')):
-                resize_image(asset_filepath, (100, 100))  # Specify desired dimensions
-
-            # Extract text from PDF files
-            if asset_path.lower().endswith('.pdf'):
-                extract_text_from_pdf(asset_filepath)
-
-            # Extract text from Word files
-            if asset_path.lower().endswith('.docx'):
-                extract_text_from_docx(asset_filepath)
-
-            # Extract text from Excel files
-            if asset_path.lower().endswith('.xlsx'):
-                extract_text_from_excel(asset_filepath)
+            if img:
+                # Resize images if it's an image file
+                if asset_path.lower().endswith(('.png', '.jpg', '.jpeg', '.gif')):
+                    resize_image(asset_filepath, (100, 100))  # Specify desired dimensions
+
+            if pdf:
+                # Extract text from PDF files
+                if asset_path.lower().endswith('.pdf'):
+                    extract_text_from_pdf(asset_filepath)
+
+            if doc:
+                # Extract text from Word files
+                if asset_path.lower().endswith('.docx'):
+                    extract_text_from_docx(asset_filepath)
+
+            if xlx:
+                # Extract text from Excel files
+                if asset_path.lower().endswith('.xlsx'):
+                    extract_text_from_excel(asset_filepath)
 
 def resize_image(image_path, dimensions):
     img = Image.open(image_path)
     img_resized = img.resize(dimensions, Image.ANTIALIAS)
     img_resized.save(image_path)
 
 def extract_text_from_pdf(pdf_path):
```

### Comparing `web_assets_downloader-2.1.0/web_assets_downloader.egg-info/PKG-INFO` & `web_assets_downloader-2.2.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: web-assets-downloader
-Version: 2.1.0
+Name: web_assets_downloader
+Version: 2.2.0
 Summary: A package for downloading web content and assets
 Home-page: https://github.com/arif-x/web-assets-downloader
 Author: Ariffudin
 Author-email: sudo.ariffudin@email.com
 License: MIT
 Project-URL: Source, https://github.com/arif-x/web-assets-downloader
 Project-URL: Source Code, https://github.com/arif-x/web-assets-downloader
```

