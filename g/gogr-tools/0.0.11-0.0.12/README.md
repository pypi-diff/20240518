# Comparing `tmp/gogr_tools-0.0.11.tar.gz` & `tmp/gogr_tools-0.0.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gogr_tools-0.0.11.tar", last modified: Sat May 18 11:32:28 2024, max compression
+gzip compressed data, was "gogr_tools-0.0.12.tar", last modified: Sat May 18 11:48:42 2024, max compression
```

## Comparing `gogr_tools-0.0.11.tar` & `gogr_tools-0.0.12.tar`

### file list

```diff
@@ -1,15 +1,12 @@
-drwxrwxrwx   0        0        0        0 2024-05-18 11:32:28.923725 gogr_tools-0.0.11/
--rw-rw-rw-   0        0        0     1091 2024-05-18 10:47:16.000000 gogr_tools-0.0.11/LICENSE.txt
--rw-rw-rw-   0        0        0      702 2024-05-18 11:32:28.922725 gogr_tools-0.0.11/PKG-INFO
--rw-rw-rw-   0        0        0      122 2024-05-18 10:32:19.000000 gogr_tools-0.0.11/README.md
-drwxrwxrwx   0        0        0        0 2024-05-18 11:32:28.920725 gogr_tools-0.0.11/gogr_tools.egg-info/
--rw-rw-rw-   0        0        0      702 2024-05-18 11:32:28.000000 gogr_tools-0.0.11/gogr_tools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      219 2024-05-18 11:32:28.000000 gogr_tools-0.0.11/gogr_tools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-18 11:32:28.000000 gogr_tools-0.0.11/gogr_tools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        4 2024-05-18 11:32:28.000000 gogr_tools-0.0.11/gogr_tools.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      626 2024-05-18 11:31:53.000000 gogr_tools-0.0.11/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-18 11:32:28.923725 gogr_tools-0.0.11/setup.cfg
--rw-rw-rw-   0        0        0      956 2024-05-18 11:32:05.000000 gogr_tools-0.0.11/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-18 11:32:28.919726 gogr_tools-0.0.11/src/
--rw-rw-rw-   0        0        0       44 2024-05-18 10:42:32.000000 gogr_tools-0.0.11/src/__init__.py
--rw-rw-rw-   0        0        0     6349 2024-05-18 10:25:39.000000 gogr_tools-0.0.11/src/visualisations.py
+drwxrwxrwx   0        0        0        0 2024-05-18 11:48:42.060860 gogr_tools-0.0.12/
+-rw-rw-rw-   0        0        0     1091 2024-05-18 10:47:16.000000 gogr_tools-0.0.12/LICENSE.txt
+-rw-rw-rw-   0        0        0      702 2024-05-18 11:48:42.058861 gogr_tools-0.0.12/PKG-INFO
+-rw-rw-rw-   0        0        0      122 2024-05-18 10:32:19.000000 gogr_tools-0.0.12/README.md
+drwxrwxrwx   0        0        0        0 2024-05-18 11:48:42.058861 gogr_tools-0.0.12/gogr_tools.egg-info/
+-rw-rw-rw-   0        0        0      702 2024-05-18 11:48:42.000000 gogr_tools-0.0.12/gogr_tools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      181 2024-05-18 11:48:42.000000 gogr_tools-0.0.12/gogr_tools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-18 11:48:42.000000 gogr_tools-0.0.12/gogr_tools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        1 2024-05-18 11:48:42.000000 gogr_tools-0.0.12/gogr_tools.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      626 2024-05-18 11:46:44.000000 gogr_tools-0.0.12/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-18 11:48:42.060860 gogr_tools-0.0.12/setup.cfg
+-rw-rw-rw-   0        0        0      956 2024-05-18 11:46:57.000000 gogr_tools-0.0.12/setup.py
```

### Comparing `gogr_tools-0.0.11/LICENSE.txt` & `gogr_tools-0.0.12/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `gogr_tools-0.0.11/PKG-INFO` & `gogr_tools-0.0.12/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gogr_tools
-Version: 0.0.11
+Version: 0.0.12
 Summary: Package for Personal use in DataScience
 Author: Grzegorz Gomza
 Author-email: Grzegorz Gomza <gomza.datascience@gmail.com>
 Project-URL: Homepage, https://github.com/grzegorz-gomza/GOGR-Tools
 Project-URL: Issues, https://github.com/grzegorz-gomza/GOGR-Tools/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `gogr_tools-0.0.11/gogr_tools.egg-info/PKG-INFO` & `gogr_tools-0.0.12/gogr_tools.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gogr_tools
-Version: 0.0.11
+Version: 0.0.12
 Summary: Package for Personal use in DataScience
 Author: Grzegorz Gomza
 Author-email: Grzegorz Gomza <gomza.datascience@gmail.com>
 Project-URL: Homepage, https://github.com/grzegorz-gomza/GOGR-Tools
 Project-URL: Issues, https://github.com/grzegorz-gomza/GOGR-Tools/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `gogr_tools-0.0.11/pyproject.toml` & `gogr_tools-0.0.12/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "gogr_tools"
-version = "0.0.11"
+version = "0.0.12"
 authors = [
   { name="Grzegorz Gomza", email="gomza.datascience@gmail.com" },
 ]
 description = "Package for Personal use in DataScience"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `gogr_tools-0.0.11/setup.py` & `gogr_tools-0.0.12/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 import codecs
 import os
 
-VERSION = '0.0.11'
+VERSION = '0.0.12'
 DESCRIPTION = 'Package for personal use in Data Science'
 LONG_DESCRIPTION = 'Package for personal use in DataS Science, Machine Learning and Deep Learning'
 
 # Setting up
 setup(
     name="gogr_tools",
     version=VERSION,
```

