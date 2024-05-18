# Comparing `tmp/dp-PDF-Crawler-0.3.0.tar.gz` & `tmp/dp-PDF-Crawler-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\dp-PDF-Crawler-0.3.0.tar", last modified: Sat May 18 08:16:37 2024, max compression
+gzip compressed data, was "dist\dp-PDF-Crawler-0.4.0.tar", last modified: Sat May 18 10:01:31 2024, max compression
```

## Comparing `dp-PDF-Crawler-0.3.0.tar` & `dp-PDF-Crawler-0.4.0.tar`

### file list

```diff
@@ -1,10 +1,10 @@
-drwxrwxrwx   0        0        0        0 2024-05-18 08:16:37.852204 dp-PDF-Crawler-0.3.0/
--rw-rw-rw-   0        0        0      901 2024-05-18 08:16:37.850193 dp-PDF-Crawler-0.3.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-18 08:16:37.845047 dp-PDF-Crawler-0.3.0/dp_PDF_Crawler.egg-info/
--rw-rw-rw-   0        0        0      901 2024-05-18 08:16:37.000000 dp-PDF-Crawler-0.3.0/dp_PDF_Crawler.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      201 2024-05-18 08:16:37.000000 dp-PDF-Crawler-0.3.0/dp_PDF_Crawler.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-18 08:16:37.000000 dp-PDF-Crawler-0.3.0/dp_PDF_Crawler.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      413 2024-05-18 08:16:37.000000 dp-PDF-Crawler-0.3.0/dp_PDF_Crawler.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2024-05-18 08:16:37.000000 dp-PDF-Crawler-0.3.0/dp_PDF_Crawler.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      868 2024-05-18 08:15:07.000000 dp-PDF-Crawler-0.3.0/lib-setup.py
--rw-rw-rw-   0        0        0       42 2024-05-18 08:16:37.853206 dp-PDF-Crawler-0.3.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-18 10:01:31.781966 dp-PDF-Crawler-0.4.0/
+-rw-rw-rw-   0        0        0      946 2024-05-18 10:01:31.777968 dp-PDF-Crawler-0.4.0/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-18 10:01:31.770055 dp-PDF-Crawler-0.4.0/dp_PDF_Crawler.egg-info/
+-rw-rw-rw-   0        0        0      946 2024-05-18 10:01:30.000000 dp-PDF-Crawler-0.4.0/dp_PDF_Crawler.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      201 2024-05-18 10:01:31.000000 dp-PDF-Crawler-0.4.0/dp_PDF_Crawler.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-18 10:01:30.000000 dp-PDF-Crawler-0.4.0/dp_PDF_Crawler.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      426 2024-05-18 10:01:30.000000 dp-PDF-Crawler-0.4.0/dp_PDF_Crawler.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2024-05-18 10:01:30.000000 dp-PDF-Crawler-0.4.0/dp_PDF_Crawler.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      897 2024-05-18 10:01:21.000000 dp-PDF-Crawler-0.4.0/lib-setup.py
+-rw-rw-rw-   0        0        0       42 2024-05-18 10:01:31.782964 dp-PDF-Crawler-0.4.0/setup.cfg
```

### Comparing `dp-PDF-Crawler-0.3.0/PKG-INFO` & `dp-PDF-Crawler-0.4.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 Metadata-Version: 2.1
 Name: dp-PDF-Crawler
-Version: 0.3.0
+Version: 0.4.0
 Summary: A custom Flask package with PDF processing tools
+Requires-Dist: PyMuPDF
+Requires-Dist: fitz
 Requires-Dist: fitz==0.0.1.dev2
 Requires-Dist: Flask==3.0.2
 Requires-Dist: langdetect==1.0.9
 Requires-Dist: nltk==3.6.7
 Requires-Dist: numpy==1.24.3
 Requires-Dist: openai==0.28.1
 Requires-Dist: opencv_python==4.8.1.78
```

### Comparing `dp-PDF-Crawler-0.3.0/dp_PDF_Crawler.egg-info/PKG-INFO` & `dp-PDF-Crawler-0.4.0/dp_PDF_Crawler.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 Metadata-Version: 2.1
 Name: dp-PDF-Crawler
-Version: 0.3.0
+Version: 0.4.0
 Summary: A custom Flask package with PDF processing tools
+Requires-Dist: PyMuPDF
+Requires-Dist: fitz
 Requires-Dist: fitz==0.0.1.dev2
 Requires-Dist: Flask==3.0.2
 Requires-Dist: langdetect==1.0.9
 Requires-Dist: nltk==3.6.7
 Requires-Dist: numpy==1.24.3
 Requires-Dist: openai==0.28.1
 Requires-Dist: opencv_python==4.8.1.78
```

### Comparing `dp-PDF-Crawler-0.3.0/lib-setup.py` & `dp-PDF-Crawler-0.4.0/lib-setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 
 from setuptools import setup, find_packages
 
 setup(
     name='dp-PDF-Crawler',
-    version='0.3.0',  # Update version as needed
+    version='0.4.0',  # Update version as needed
     description='A custom Flask package with PDF processing tools',
     packages=find_packages(),
     install_requires=[
+    'PyMuPDF',
+    'fitz',
     'fitz==0.0.1.dev2',
     'Flask==3.0.2',
     'langdetect==1.0.9',
     'nltk==3.6.7',
     'numpy==1.24.3',
     'openai==0.28.1',
     'opencv_python==4.8.1.78',
```

