# Comparing `tmp/dp-PDF-Crawler-0.2.0.tar.gz` & `tmp/dp-PDF-Crawler-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\dp-PDF-Crawler-0.2.0.tar", last modified: Sat Mar 30 05:46:42 2024, max compression
+gzip compressed data, was "dist\dp-PDF-Crawler-0.3.0.tar", last modified: Sat May 18 08:16:37 2024, max compression
```

## Comparing `dp-PDF-Crawler-0.2.0.tar` & `dp-PDF-Crawler-0.3.0.tar`

### file list

```diff
@@ -1,10 +1,10 @@
-drwxrwxrwx   0        0        0        0 2024-03-30 05:46:42.058339 dp-PDF-Crawler-0.2.0/
--rw-rw-rw-   0        0        0      832 2024-03-30 05:46:42.055336 dp-PDF-Crawler-0.2.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-03-30 05:46:42.048037 dp-PDF-Crawler-0.2.0/dp_PDF_Crawler.egg-info/
--rw-rw-rw-   0        0        0      832 2024-03-30 05:46:41.000000 dp-PDF-Crawler-0.2.0/dp_PDF_Crawler.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      197 2024-03-30 05:46:41.000000 dp-PDF-Crawler-0.2.0/dp_PDF_Crawler.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-30 05:46:41.000000 dp-PDF-Crawler-0.2.0/dp_PDF_Crawler.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      376 2024-03-30 05:46:41.000000 dp-PDF-Crawler-0.2.0/dp_PDF_Crawler.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2024-03-30 05:46:41.000000 dp-PDF-Crawler-0.2.0/dp_PDF_Crawler.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-03-30 05:46:42.062902 dp-PDF-Crawler-0.2.0/setup.cfg
--rw-rw-rw-   0        0        0      815 2024-03-30 05:46:30.000000 dp-PDF-Crawler-0.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-18 08:16:37.852204 dp-PDF-Crawler-0.3.0/
+-rw-rw-rw-   0        0        0      901 2024-05-18 08:16:37.850193 dp-PDF-Crawler-0.3.0/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-18 08:16:37.845047 dp-PDF-Crawler-0.3.0/dp_PDF_Crawler.egg-info/
+-rw-rw-rw-   0        0        0      901 2024-05-18 08:16:37.000000 dp-PDF-Crawler-0.3.0/dp_PDF_Crawler.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      201 2024-05-18 08:16:37.000000 dp-PDF-Crawler-0.3.0/dp_PDF_Crawler.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-18 08:16:37.000000 dp-PDF-Crawler-0.3.0/dp_PDF_Crawler.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      413 2024-05-18 08:16:37.000000 dp-PDF-Crawler-0.3.0/dp_PDF_Crawler.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2024-05-18 08:16:37.000000 dp-PDF-Crawler-0.3.0/dp_PDF_Crawler.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      868 2024-05-18 08:15:07.000000 dp-PDF-Crawler-0.3.0/lib-setup.py
+-rw-rw-rw-   0        0        0       42 2024-05-18 08:16:37.853206 dp-PDF-Crawler-0.3.0/setup.cfg
```

### Comparing `dp-PDF-Crawler-0.2.0/PKG-INFO` & `dp-PDF-Crawler-0.3.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dp-PDF-Crawler
-Version: 0.2.0
+Version: 0.3.0
 Summary: A custom Flask package with PDF processing tools
 Requires-Dist: fitz==0.0.1.dev2
 Requires-Dist: Flask==3.0.2
 Requires-Dist: langdetect==1.0.9
 Requires-Dist: nltk==3.6.7
 Requires-Dist: numpy==1.24.3
 Requires-Dist: openai==0.28.1
@@ -18,8 +18,10 @@
 Requires-Dist: Requests==2.31.0
 Requires-Dist: scipy==1.12.0
 Requires-Dist: sentence_transformers==2.2.2
 Requires-Dist: tensorflow==2.13.1
 Requires-Dist: timeout_decorator==0.5.0
 Requires-Dist: torch==2.1.0
 Requires-Dist: transformers==4.35.2
+Requires-Dist: ultralytics==8.0.153
+Requires-Dist: waitress==3.0.0
 Requires-Dist: Werkzeug==3.0.1
```

### Comparing `dp-PDF-Crawler-0.2.0/dp_PDF_Crawler.egg-info/PKG-INFO` & `dp-PDF-Crawler-0.3.0/dp_PDF_Crawler.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dp-PDF-Crawler
-Version: 0.2.0
+Version: 0.3.0
 Summary: A custom Flask package with PDF processing tools
 Requires-Dist: fitz==0.0.1.dev2
 Requires-Dist: Flask==3.0.2
 Requires-Dist: langdetect==1.0.9
 Requires-Dist: nltk==3.6.7
 Requires-Dist: numpy==1.24.3
 Requires-Dist: openai==0.28.1
@@ -18,8 +18,10 @@
 Requires-Dist: Requests==2.31.0
 Requires-Dist: scipy==1.12.0
 Requires-Dist: sentence_transformers==2.2.2
 Requires-Dist: tensorflow==2.13.1
 Requires-Dist: timeout_decorator==0.5.0
 Requires-Dist: torch==2.1.0
 Requires-Dist: transformers==4.35.2
+Requires-Dist: ultralytics==8.0.153
+Requires-Dist: waitress==3.0.0
 Requires-Dist: Werkzeug==3.0.1
```

### Comparing `dp-PDF-Crawler-0.2.0/setup.py` & `dp-PDF-Crawler-0.3.0/lib-setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 
 from setuptools import setup, find_packages
 
 setup(
     name='dp-PDF-Crawler',
-    version='0.2.0',  # Update version as needed
+    version='0.3.0',  # Update version as needed
     description='A custom Flask package with PDF processing tools',
     packages=find_packages(),
     install_requires=[
     'fitz==0.0.1.dev2',
     'Flask==3.0.2',
     'langdetect==1.0.9',
     'nltk==3.6.7',
@@ -23,10 +23,12 @@
     'Requests==2.31.0',
     'scipy==1.12.0',
     'sentence_transformers==2.2.2',
     'tensorflow==2.13.1',
     'timeout_decorator==0.5.0',
     'torch==2.1.0',
     'transformers==4.35.2',
+    'ultralytics==8.0.153',
+    'waitress==3.0.0',
     'Werkzeug==3.0.1'
         ],
 )
```

