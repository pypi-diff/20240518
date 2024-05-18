# Comparing `tmp/dp-PDF-Crawler-1.0.0.tar.gz` & `tmp/dp-PDF-Crawler-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\dp-PDF-Crawler-1.0.0.tar", last modified: Sat May 18 10:45:29 2024, max compression
+gzip compressed data, was "dist\dp-PDF-Crawler-1.0.1.tar", last modified: Sat May 18 11:08:46 2024, max compression
```

## Comparing `dp-PDF-Crawler-1.0.0.tar` & `dp-PDF-Crawler-1.0.1.tar`

### file list

```diff
@@ -1,10 +1,10 @@
-drwxrwxrwx   0        0        0        0 2024-05-18 10:45:29.743680 dp-PDF-Crawler-1.0.0/
--rw-rw-rw-   0        0        0      992 2024-05-18 10:45:29.733062 dp-PDF-Crawler-1.0.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-18 10:45:29.729102 dp-PDF-Crawler-1.0.0/dp_PDF_Crawler.egg-info/
--rw-rw-rw-   0        0        0      992 2024-05-18 10:45:28.000000 dp-PDF-Crawler-1.0.0/dp_PDF_Crawler.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      201 2024-05-18 10:45:29.000000 dp-PDF-Crawler-1.0.0/dp_PDF_Crawler.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-18 10:45:28.000000 dp-PDF-Crawler-1.0.0/dp_PDF_Crawler.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      440 2024-05-18 10:45:28.000000 dp-PDF-Crawler-1.0.0/dp_PDF_Crawler.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2024-05-18 10:45:28.000000 dp-PDF-Crawler-1.0.0/dp_PDF_Crawler.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      927 2024-05-18 10:45:18.000000 dp-PDF-Crawler-1.0.0/lib-setup.py
--rw-rw-rw-   0        0        0       42 2024-05-18 10:45:29.746061 dp-PDF-Crawler-1.0.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-18 11:08:46.563822 dp-PDF-Crawler-1.0.1/
+-rw-rw-rw-   0        0        0     1039 2024-05-18 11:08:46.559875 dp-PDF-Crawler-1.0.1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-18 11:08:46.552342 dp-PDF-Crawler-1.0.1/dp_PDF_Crawler.egg-info/
+-rw-rw-rw-   0        0        0     1039 2024-05-18 11:08:45.000000 dp-PDF-Crawler-1.0.1/dp_PDF_Crawler.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      201 2024-05-18 11:08:46.000000 dp-PDF-Crawler-1.0.1/dp_PDF_Crawler.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-18 11:08:45.000000 dp-PDF-Crawler-1.0.1/dp_PDF_Crawler.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      471 2024-05-18 11:08:45.000000 dp-PDF-Crawler-1.0.1/dp_PDF_Crawler.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2024-05-18 11:08:45.000000 dp-PDF-Crawler-1.0.1/dp_PDF_Crawler.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      966 2024-05-18 11:08:32.000000 dp-PDF-Crawler-1.0.1/lib-setup.py
+-rw-rw-rw-   0        0        0       42 2024-05-18 11:08:46.565903 dp-PDF-Crawler-1.0.1/setup.cfg
```

### Comparing `dp-PDF-Crawler-1.0.0/PKG-INFO` & `dp-PDF-Crawler-1.0.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dp-PDF-Crawler
-Version: 1.0.0
+Version: 1.0.1
 Summary: A custom Flask package with PDF processing tools
 Requires-Dist: PyMuPDF
 Requires-Dist: fitz
 Requires-Dist: dotenv
 Requires-Dist: fitz==0.0.1.dev2
 Requires-Dist: Flask==3.0.2
 Requires-Dist: langdetect==1.0.9
@@ -24,8 +24,9 @@
 Requires-Dist: tensorflow==2.13.1
 Requires-Dist: timeout_decorator==0.5.0
 Requires-Dist: torch==2.1.0
 Requires-Dist: transformers==4.35.2
 Requires-Dist: ultralytics==8.0.153
 Requires-Dist: waitress==3.0.0
 Requires-Dist: Werkzeug==3.0.1
-Requires-Dist: dotenv
+Requires-Dist: python-dotenv
+Requires-Dist: deep_translator==1.11.4
```

### Comparing `dp-PDF-Crawler-1.0.0/dp_PDF_Crawler.egg-info/PKG-INFO` & `dp-PDF-Crawler-1.0.1/dp_PDF_Crawler.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dp-PDF-Crawler
-Version: 1.0.0
+Version: 1.0.1
 Summary: A custom Flask package with PDF processing tools
 Requires-Dist: PyMuPDF
 Requires-Dist: fitz
 Requires-Dist: dotenv
 Requires-Dist: fitz==0.0.1.dev2
 Requires-Dist: Flask==3.0.2
 Requires-Dist: langdetect==1.0.9
@@ -24,8 +24,9 @@
 Requires-Dist: tensorflow==2.13.1
 Requires-Dist: timeout_decorator==0.5.0
 Requires-Dist: torch==2.1.0
 Requires-Dist: transformers==4.35.2
 Requires-Dist: ultralytics==8.0.153
 Requires-Dist: waitress==3.0.0
 Requires-Dist: Werkzeug==3.0.1
-Requires-Dist: dotenv
+Requires-Dist: python-dotenv
+Requires-Dist: deep_translator==1.11.4
```

### Comparing `dp-PDF-Crawler-1.0.0/lib-setup.py` & `dp-PDF-Crawler-1.0.1/lib-setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 
 from setuptools import setup, find_packages
 
 setup(
     name='dp-PDF-Crawler',
-    version='1.0.0',  # Update version as needed
+    version='1.0.1',  # Update version as needed
     description='A custom Flask package with PDF processing tools',
     packages=find_packages(),
     install_requires=[
     'PyMuPDF',
     'fitz',
     'dotenv',
     'fitz==0.0.1.dev2',
@@ -29,10 +29,11 @@
     'tensorflow==2.13.1',
     'timeout_decorator==0.5.0',
     'torch==2.1.0',
     'transformers==4.35.2',
     'ultralytics==8.0.153',
     'waitress==3.0.0',
     'Werkzeug==3.0.1',
-    'dotenv'
+    'python-dotenv',
+    'deep_translator==1.11.4'
         ],
 )
```

