# Comparing `tmp/dp-PDF-Crawler-1.0.1.tar.gz` & `tmp/dp-PDF-Crawler-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\dp-PDF-Crawler-1.0.1.tar", last modified: Sat May 18 11:08:46 2024, max compression
+gzip compressed data, was "dist\dp-PDF-Crawler-1.0.2.tar", last modified: Sat May 18 11:21:02 2024, max compression
```

## Comparing `dp-PDF-Crawler-1.0.1.tar` & `dp-PDF-Crawler-1.0.2.tar`

### file list

```diff
@@ -1,10 +1,10 @@
-drwxrwxrwx   0        0        0        0 2024-05-18 11:08:46.563822 dp-PDF-Crawler-1.0.1/
--rw-rw-rw-   0        0        0     1039 2024-05-18 11:08:46.559875 dp-PDF-Crawler-1.0.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-18 11:08:46.552342 dp-PDF-Crawler-1.0.1/dp_PDF_Crawler.egg-info/
--rw-rw-rw-   0        0        0     1039 2024-05-18 11:08:45.000000 dp-PDF-Crawler-1.0.1/dp_PDF_Crawler.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      201 2024-05-18 11:08:46.000000 dp-PDF-Crawler-1.0.1/dp_PDF_Crawler.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-18 11:08:45.000000 dp-PDF-Crawler-1.0.1/dp_PDF_Crawler.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      471 2024-05-18 11:08:45.000000 dp-PDF-Crawler-1.0.1/dp_PDF_Crawler.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2024-05-18 11:08:45.000000 dp-PDF-Crawler-1.0.1/dp_PDF_Crawler.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      966 2024-05-18 11:08:32.000000 dp-PDF-Crawler-1.0.1/lib-setup.py
--rw-rw-rw-   0        0        0       42 2024-05-18 11:08:46.565903 dp-PDF-Crawler-1.0.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-18 11:21:02.840496 dp-PDF-Crawler-1.0.2/
+-rw-rw-rw-   0        0        0     1016 2024-05-18 11:21:02.836527 dp-PDF-Crawler-1.0.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-18 11:21:02.828489 dp-PDF-Crawler-1.0.2/dp_PDF_Crawler.egg-info/
+-rw-rw-rw-   0        0        0     1016 2024-05-18 11:21:02.000000 dp-PDF-Crawler-1.0.2/dp_PDF_Crawler.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      201 2024-05-18 11:21:02.000000 dp-PDF-Crawler-1.0.2/dp_PDF_Crawler.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-18 11:21:02.000000 dp-PDF-Crawler-1.0.2/dp_PDF_Crawler.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      464 2024-05-18 11:21:02.000000 dp-PDF-Crawler-1.0.2/dp_PDF_Crawler.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2024-05-18 11:21:02.000000 dp-PDF-Crawler-1.0.2/dp_PDF_Crawler.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      951 2024-05-18 11:20:57.000000 dp-PDF-Crawler-1.0.2/lib-setup.py
+-rw-rw-rw-   0        0        0       42 2024-05-18 11:21:02.842483 dp-PDF-Crawler-1.0.2/setup.cfg
```

### Comparing `dp-PDF-Crawler-1.0.1/PKG-INFO` & `dp-PDF-Crawler-1.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 Metadata-Version: 2.1
 Name: dp-PDF-Crawler
-Version: 1.0.1
+Version: 1.0.2
 Summary: A custom Flask package with PDF processing tools
 Requires-Dist: PyMuPDF
 Requires-Dist: fitz
-Requires-Dist: dotenv
 Requires-Dist: fitz==0.0.1.dev2
 Requires-Dist: Flask==3.0.2
 Requires-Dist: langdetect==1.0.9
 Requires-Dist: nltk==3.6.7
 Requires-Dist: numpy==1.24.3
 Requires-Dist: openai==0.28.1
 Requires-Dist: opencv_python==4.8.1.78
```

### Comparing `dp-PDF-Crawler-1.0.1/dp_PDF_Crawler.egg-info/PKG-INFO` & `dp-PDF-Crawler-1.0.2/dp_PDF_Crawler.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 Metadata-Version: 2.1
 Name: dp-PDF-Crawler
-Version: 1.0.1
+Version: 1.0.2
 Summary: A custom Flask package with PDF processing tools
 Requires-Dist: PyMuPDF
 Requires-Dist: fitz
-Requires-Dist: dotenv
 Requires-Dist: fitz==0.0.1.dev2
 Requires-Dist: Flask==3.0.2
 Requires-Dist: langdetect==1.0.9
 Requires-Dist: nltk==3.6.7
 Requires-Dist: numpy==1.24.3
 Requires-Dist: openai==0.28.1
 Requires-Dist: opencv_python==4.8.1.78
```

### Comparing `dp-PDF-Crawler-1.0.1/lib-setup.py` & `dp-PDF-Crawler-1.0.2/lib-setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 
 from setuptools import setup, find_packages
 
 setup(
     name='dp-PDF-Crawler',
-    version='1.0.1',  # Update version as needed
+    version='1.0.2',  # Update version as needed
     description='A custom Flask package with PDF processing tools',
     packages=find_packages(),
     install_requires=[
     'PyMuPDF',
     'fitz',
-    'dotenv',
     'fitz==0.0.1.dev2',
     'Flask==3.0.2',
     'langdetect==1.0.9',
     'nltk==3.6.7',
     'numpy==1.24.3',
     'openai==0.28.1',
     'opencv_python==4.8.1.78',
```

