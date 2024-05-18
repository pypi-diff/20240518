# Comparing `tmp/link-shorteners-1.0.7.tar.gz` & `tmp/link-shorteners-1.10.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "link-shorteners-1.0.7.tar", last modified: Sun Feb 11 18:50:39 2024, max compression
+gzip compressed data, was "link-shorteners-1.10.0.tar", last modified: Sun Mar 10 05:55:55 2024, max compression
```

## Comparing `link-shorteners-1.0.7.tar` & `link-shorteners-1.10.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 samikshagarg   (501) staff       (20)        0 2024-02-11 18:50:39.897846 link-shorteners-1.0.7/
--rw-r--r--   0 samikshagarg   (501) staff       (20)     3528 2024-02-11 18:50:39.897649 link-shorteners-1.0.7/PKG-INFO
--rw-r--r--   0 samikshagarg   (501) staff       (20)     3252 2024-02-11 18:49:36.000000 link-shorteners-1.0.7/README.md
-drwxr-xr-x   0 samikshagarg   (501) staff       (20)        0 2024-02-11 18:50:39.896899 link-shorteners-1.0.7/link_shorteners/
--rw-r--r--   0 samikshagarg   (501) staff       (20)       49 2024-01-16 18:24:09.000000 link-shorteners-1.0.7/link_shorteners/__init__.py
--rw-r--r--   0 samikshagarg   (501) staff       (20)     1135 2024-02-11 18:49:36.000000 link-shorteners-1.0.7/link_shorteners/link-shorteners.txt
--rw-r--r--   0 samikshagarg   (501) staff       (20)      580 2024-01-16 18:24:09.000000 link-shorteners-1.0.7/link_shorteners/link_shorteners.py
-drwxr-xr-x   0 samikshagarg   (501) staff       (20)        0 2024-02-11 18:50:39.897420 link-shorteners-1.0.7/link_shorteners.egg-info/
--rw-r--r--   0 samikshagarg   (501) staff       (20)     3528 2024-02-11 18:50:39.000000 link-shorteners-1.0.7/link_shorteners.egg-info/PKG-INFO
--rw-r--r--   0 samikshagarg   (501) staff       (20)      273 2024-02-11 18:50:39.000000 link-shorteners-1.0.7/link_shorteners.egg-info/SOURCES.txt
--rw-r--r--   0 samikshagarg   (501) staff       (20)        1 2024-02-11 18:50:39.000000 link-shorteners-1.0.7/link_shorteners.egg-info/dependency_links.txt
--rw-r--r--   0 samikshagarg   (501) staff       (20)       16 2024-02-11 18:50:39.000000 link-shorteners-1.0.7/link_shorteners.egg-info/top_level.txt
--rw-r--r--   0 samikshagarg   (501) staff       (20)       38 2024-02-11 18:50:39.897883 link-shorteners-1.0.7/setup.cfg
--rw-r--r--   0 samikshagarg   (501) staff       (20)      545 2024-02-11 18:49:36.000000 link-shorteners-1.0.7/setup.py
+drwxr-xr-x   0 samikshagarg   (501) staff       (20)        0 2024-03-10 05:55:55.586185 link-shorteners-1.10.0/
+-rw-r--r--   0 samikshagarg   (501) staff       (20)     3529 2024-03-10 05:55:55.585991 link-shorteners-1.10.0/PKG-INFO
+-rw-r--r--   0 samikshagarg   (501) staff       (20)     3252 2024-03-10 05:52:50.000000 link-shorteners-1.10.0/README.md
+drwxr-xr-x   0 samikshagarg   (501) staff       (20)        0 2024-03-10 05:55:55.585023 link-shorteners-1.10.0/link_shorteners/
+-rw-r--r--   0 samikshagarg   (501) staff       (20)       49 2024-03-10 05:52:50.000000 link-shorteners-1.10.0/link_shorteners/__init__.py
+-rw-r--r--   0 samikshagarg   (501) staff       (20)    20183 2024-03-10 05:52:50.000000 link-shorteners-1.10.0/link_shorteners/link-shorteners.txt
+-rw-r--r--   0 samikshagarg   (501) staff       (20)      580 2024-03-10 05:52:50.000000 link-shorteners-1.10.0/link_shorteners/link_shorteners.py
+drwxr-xr-x   0 samikshagarg   (501) staff       (20)        0 2024-03-10 05:55:55.585815 link-shorteners-1.10.0/link_shorteners.egg-info/
+-rw-r--r--   0 samikshagarg   (501) staff       (20)     3529 2024-03-10 05:55:55.000000 link-shorteners-1.10.0/link_shorteners.egg-info/PKG-INFO
+-rw-r--r--   0 samikshagarg   (501) staff       (20)      273 2024-03-10 05:55:55.000000 link-shorteners-1.10.0/link_shorteners.egg-info/SOURCES.txt
+-rw-r--r--   0 samikshagarg   (501) staff       (20)        1 2024-03-10 05:55:55.000000 link-shorteners-1.10.0/link_shorteners.egg-info/dependency_links.txt
+-rw-r--r--   0 samikshagarg   (501) staff       (20)       16 2024-03-10 05:55:55.000000 link-shorteners-1.10.0/link_shorteners.egg-info/top_level.txt
+-rw-r--r--   0 samikshagarg   (501) staff       (20)       38 2024-03-10 05:55:55.586225 link-shorteners-1.10.0/setup.cfg
+-rw-r--r--   0 samikshagarg   (501) staff       (20)      546 2024-03-10 05:52:50.000000 link-shorteners-1.10.0/setup.py
```

### Comparing `link-shorteners-1.0.7/PKG-INFO` & `link-shorteners-1.10.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: link-shorteners
-Version: 1.0.7
+Version: 1.10.0
 Summary: List of all URL shorteners, such as bitly, tinyurl, shorturl, and many others.
 Home-page: https://github.com/mayakyler/link-shorteners/py-link-shorteners
 License: MIT
 Description-Content-Type: text/markdown
 
 # link-shorteners Package
 
 This package exposes a list of all known link shorteners (also known as URL shorteners). 
 This can help you block or filter link shorteners. We are promoting responsible link shortening practices and trying to cut down on spam.
 Built by [Maya](https://mayakyler.com) from [y.gy](https://app.y.gy).
 
-**Latest Version**: 1.0.7 released on 2024-Feb-11
+**Latest Version**: 1.10.0 released on 2024-Mar-8
 
 ## Table of Contents
 - [Key Features](#key-features)
 - [Installation](#installation)
 - [Usage](#usage)
 - [Contribution](#contribution)
 - [License](#license)
```

### Comparing `link-shorteners-1.0.7/README.md` & `link-shorteners-1.10.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # link-shorteners Package
 
 This package exposes a list of all known link shorteners (also known as URL shorteners). 
 This can help you block or filter link shorteners. We are promoting responsible link shortening practices and trying to cut down on spam.
 Built by [Maya](https://mayakyler.com) from [y.gy](https://app.y.gy).
 
-**Latest Version**: 1.0.7 released on 2024-Feb-11
+**Latest Version**: 1.10.0 released on 2024-Mar-8
 
 ## Table of Contents
 - [Key Features](#key-features)
 - [Installation](#installation)
 - [Usage](#usage)
 - [Contribution](#contribution)
 - [License](#license)
```

### Comparing `link-shorteners-1.0.7/link_shorteners/link_shorteners.py` & `link-shorteners-1.10.0/link_shorteners/link_shorteners.py`

 * *Files identical despite different names*

### Comparing `link-shorteners-1.0.7/link_shorteners.egg-info/PKG-INFO` & `link-shorteners-1.10.0/link_shorteners.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: link-shorteners
-Version: 1.0.7
+Version: 1.10.0
 Summary: List of all URL shorteners, such as bitly, tinyurl, shorturl, and many others.
 Home-page: https://github.com/mayakyler/link-shorteners/py-link-shorteners
 License: MIT
 Description-Content-Type: text/markdown
 
 # link-shorteners Package
 
 This package exposes a list of all known link shorteners (also known as URL shorteners). 
 This can help you block or filter link shorteners. We are promoting responsible link shortening practices and trying to cut down on spam.
 Built by [Maya](https://mayakyler.com) from [y.gy](https://app.y.gy).
 
-**Latest Version**: 1.0.7 released on 2024-Feb-11
+**Latest Version**: 1.10.0 released on 2024-Mar-8
 
 ## Table of Contents
 - [Key Features](#key-features)
 - [Installation](#installation)
 - [Usage](#usage)
 - [Contribution](#contribution)
 - [License](#license)
```

### Comparing `link-shorteners-1.0.7/setup.py` & `link-shorteners-1.10.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 setup(
     name="link-shorteners",
-    version="1.0.7",
+    version="1.10.0",
     description="List of all URL shorteners, such as bitly, tinyurl, shorturl, and many others.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=find_packages(),
     package_data={'link_shorteners': ['link-shorteners.txt']},
     url="https://github.com/mayakyler/link-shorteners/py-link-shorteners",
     license="MIT",
```

