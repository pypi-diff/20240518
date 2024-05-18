# Comparing `tmp/dp-PDF-Crawler-0.4.0.tar.gz` & `tmp/dp-PDF-Crawler-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\dp-PDF-Crawler-0.4.0.tar", last modified: Sat May 18 10:01:31 2024, max compression
+gzip compressed data, was "dist\dp-PDF-Crawler-1.0.0.tar", last modified: Sat May 18 10:45:29 2024, max compression
```

## Comparing `dp-PDF-Crawler-0.4.0.tar` & `dp-PDF-Crawler-1.0.0.tar`

### file list

```diff
@@ -1,10 +1,10 @@
-drwxrwxrwx   0        0        0        0 2024-05-18 10:01:31.781966 dp-PDF-Crawler-0.4.0/
--rw-rw-rw-   0        0        0      946 2024-05-18 10:01:31.777968 dp-PDF-Crawler-0.4.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-18 10:01:31.770055 dp-PDF-Crawler-0.4.0/dp_PDF_Crawler.egg-info/
--rw-rw-rw-   0        0        0      946 2024-05-18 10:01:30.000000 dp-PDF-Crawler-0.4.0/dp_PDF_Crawler.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      201 2024-05-18 10:01:31.000000 dp-PDF-Crawler-0.4.0/dp_PDF_Crawler.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-18 10:01:30.000000 dp-PDF-Crawler-0.4.0/dp_PDF_Crawler.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      426 2024-05-18 10:01:30.000000 dp-PDF-Crawler-0.4.0/dp_PDF_Crawler.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2024-05-18 10:01:30.000000 dp-PDF-Crawler-0.4.0/dp_PDF_Crawler.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      897 2024-05-18 10:01:21.000000 dp-PDF-Crawler-0.4.0/lib-setup.py
--rw-rw-rw-   0        0        0       42 2024-05-18 10:01:31.782964 dp-PDF-Crawler-0.4.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-18 10:45:29.743680 dp-PDF-Crawler-1.0.0/
+-rw-rw-rw-   0        0        0      992 2024-05-18 10:45:29.733062 dp-PDF-Crawler-1.0.0/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-18 10:45:29.729102 dp-PDF-Crawler-1.0.0/dp_PDF_Crawler.egg-info/
+-rw-rw-rw-   0        0        0      992 2024-05-18 10:45:28.000000 dp-PDF-Crawler-1.0.0/dp_PDF_Crawler.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      201 2024-05-18 10:45:29.000000 dp-PDF-Crawler-1.0.0/dp_PDF_Crawler.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-18 10:45:28.000000 dp-PDF-Crawler-1.0.0/dp_PDF_Crawler.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      440 2024-05-18 10:45:28.000000 dp-PDF-Crawler-1.0.0/dp_PDF_Crawler.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2024-05-18 10:45:28.000000 dp-PDF-Crawler-1.0.0/dp_PDF_Crawler.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      927 2024-05-18 10:45:18.000000 dp-PDF-Crawler-1.0.0/lib-setup.py
+-rw-rw-rw-   0        0        0       42 2024-05-18 10:45:29.746061 dp-PDF-Crawler-1.0.0/setup.cfg
```

### Comparing `dp-PDF-Crawler-0.4.0/PKG-INFO` & `dp-PDF-Crawler-1.0.0/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 Metadata-Version: 2.1
 Name: dp-PDF-Crawler
-Version: 0.4.0
+Version: 1.0.0
 Summary: A custom Flask package with PDF processing tools
 Requires-Dist: PyMuPDF
 Requires-Dist: fitz
+Requires-Dist: dotenv
 Requires-Dist: fitz==0.0.1.dev2
 Requires-Dist: Flask==3.0.2
 Requires-Dist: langdetect==1.0.9
 Requires-Dist: nltk==3.6.7
 Requires-Dist: numpy==1.24.3
 Requires-Dist: openai==0.28.1
 Requires-Dist: opencv_python==4.8.1.78
@@ -23,7 +24,8 @@
 Requires-Dist: tensorflow==2.13.1
 Requires-Dist: timeout_decorator==0.5.0
 Requires-Dist: torch==2.1.0
 Requires-Dist: transformers==4.35.2
 Requires-Dist: ultralytics==8.0.153
 Requires-Dist: waitress==3.0.0
 Requires-Dist: Werkzeug==3.0.1
+Requires-Dist: dotenv
```

### Comparing `dp-PDF-Crawler-0.4.0/dp_PDF_Crawler.egg-info/PKG-INFO` & `dp-PDF-Crawler-1.0.0/dp_PDF_Crawler.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 Metadata-Version: 2.1
 Name: dp-PDF-Crawler
-Version: 0.4.0
+Version: 1.0.0
 Summary: A custom Flask package with PDF processing tools
 Requires-Dist: PyMuPDF
 Requires-Dist: fitz
+Requires-Dist: dotenv
 Requires-Dist: fitz==0.0.1.dev2
 Requires-Dist: Flask==3.0.2
 Requires-Dist: langdetect==1.0.9
 Requires-Dist: nltk==3.6.7
 Requires-Dist: numpy==1.24.3
 Requires-Dist: openai==0.28.1
 Requires-Dist: opencv_python==4.8.1.78
@@ -23,7 +24,8 @@
 Requires-Dist: tensorflow==2.13.1
 Requires-Dist: timeout_decorator==0.5.0
 Requires-Dist: torch==2.1.0
 Requires-Dist: transformers==4.35.2
 Requires-Dist: ultralytics==8.0.153
 Requires-Dist: waitress==3.0.0
 Requires-Dist: Werkzeug==3.0.1
+Requires-Dist: dotenv
```

### Comparing `dp-PDF-Crawler-0.4.0/lib-setup.py` & `dp-PDF-Crawler-1.0.0/lib-setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 
 from setuptools import setup, find_packages
 
 setup(
     name='dp-PDF-Crawler',
-    version='0.4.0',  # Update version as needed
+    version='1.0.0',  # Update version as needed
     description='A custom Flask package with PDF processing tools',
     packages=find_packages(),
     install_requires=[
     'PyMuPDF',
     'fitz',
+    'dotenv',
     'fitz==0.0.1.dev2',
     'Flask==3.0.2',
     'langdetect==1.0.9',
     'nltk==3.6.7',
     'numpy==1.24.3',
     'openai==0.28.1',
     'opencv_python==4.8.1.78',
@@ -27,10 +28,11 @@
     'sentence_transformers==2.2.2',
     'tensorflow==2.13.1',
     'timeout_decorator==0.5.0',
     'torch==2.1.0',
     'transformers==4.35.2',
     'ultralytics==8.0.153',
     'waitress==3.0.0',
-    'Werkzeug==3.0.1'
+    'Werkzeug==3.0.1',
+    'dotenv'
         ],
 )
```

