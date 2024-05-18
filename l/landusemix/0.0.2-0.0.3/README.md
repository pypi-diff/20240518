# Comparing `tmp/landusemix-0.0.2.tar.gz` & `tmp/landusemix-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "landusemix-0.0.2.tar", last modified: Thu May 16 10:14:45 2024, max compression
+gzip compressed data, was "landusemix-0.0.3.tar", last modified: Sat May 18 00:30:01 2024, max compression
```

## Comparing `landusemix-0.0.2.tar` & `landusemix-0.0.3.tar`

### file list

```diff
@@ -1,15 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 10:14:45.245608 landusemix-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-05-16 10:14:41.000000 landusemix-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4281 2024-05-16 10:14:45.241608 landusemix-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3735 2024-05-16 10:14:41.000000 landusemix-0.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 10:14:45.241608 landusemix-0.0.2/landusemix.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4281 2024-05-16 10:14:45.000000 landusemix-0.0.2/landusemix.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      238 2024-05-16 10:14:45.000000 landusemix-0.0.2/landusemix.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 10:14:45.000000 landusemix-0.0.2/landusemix.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-16 10:14:45.000000 landusemix-0.0.2/landusemix.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-16 10:14:45.000000 landusemix-0.0.2/landusemix.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-16 10:14:45.245608 landusemix-0.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      750 2024-05-16 10:14:41.000000 landusemix-0.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 10:14:45.241608 landusemix-0.0.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 10:14:41.000000 landusemix-0.0.2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      832 2024-05-16 10:14:41.000000 landusemix-0.0.2/tests/test_landusemix.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 00:30:01.245154 landusemix-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-05-18 00:29:54.000000 landusemix-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4281 2024-05-18 00:30:01.245154 landusemix-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3735 2024-05-18 00:29:54.000000 landusemix-0.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 00:30:01.245154 landusemix-0.0.3/landusemix/
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-18 00:29:54.000000 landusemix-0.0.3/landusemix/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      650 2024-05-18 00:29:54.000000 landusemix-0.0.3/landusemix/indices.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1265 2024-05-18 00:29:54.000000 landusemix-0.0.3/landusemix/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 00:30:01.245154 landusemix-0.0.3/landusemix.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4281 2024-05-18 00:30:01.000000 landusemix-0.0.3/landusemix.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      303 2024-05-18 00:30:01.000000 landusemix-0.0.3/landusemix.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-18 00:30:01.000000 landusemix-0.0.3/landusemix.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-18 00:30:01.000000 landusemix-0.0.3/landusemix.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-18 00:30:01.000000 landusemix-0.0.3/landusemix.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-18 00:30:01.245154 landusemix-0.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      750 2024-05-18 00:29:54.000000 landusemix-0.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 00:30:01.245154 landusemix-0.0.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-18 00:29:54.000000 landusemix-0.0.3/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      832 2024-05-18 00:29:54.000000 landusemix-0.0.3/tests/test_landusemix.py
```

### Comparing `landusemix-0.0.2/LICENSE` & `landusemix-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `landusemix-0.0.2/PKG-INFO` & `landusemix-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: landusemix
-Version: 0.0.2
+Version: 0.0.3
 Summary: A package for calculating land use mix indices
 Home-page: https://github.com/makyol/landusemix
 Author: Mehmet Ali Akyol
 Author-email: akyol.mehmet@metu.edu.tr
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `landusemix-0.0.2/README.md` & `landusemix-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `landusemix-0.0.2/landusemix.egg-info/PKG-INFO` & `landusemix-0.0.3/landusemix.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: landusemix
-Version: 0.0.2
+Version: 0.0.3
 Summary: A package for calculating land use mix indices
 Home-page: https://github.com/makyol/landusemix
 Author: Mehmet Ali Akyol
 Author-email: akyol.mehmet@metu.edu.tr
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `landusemix-0.0.2/setup.py` & `landusemix-0.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="landusemix",
-    version="0.0.2",
+    version="0.0.3",
     author="Mehmet Ali Akyol",
     author_email="akyol.mehmet@metu.edu.tr",
     description="A package for calculating land use mix indices",
     long_description=open('README.md').read(),
     long_description_content_type="text/markdown",
     url="https://github.com/makyol/landusemix",
     packages=find_packages(),
```

### Comparing `landusemix-0.0.2/tests/test_landusemix.py` & `landusemix-0.0.3/tests/test_landusemix.py`

 * *Files identical despite different names*

