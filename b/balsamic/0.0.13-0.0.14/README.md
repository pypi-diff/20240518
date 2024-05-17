# Comparing `tmp/balsamic-0.0.13.tar.gz` & `tmp/balsamic-0.0.14.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "balsamic-0.0.13.tar", last modified: Fri May 17 20:18:28 2024, max compression
+gzip compressed data, was "balsamic-0.0.14.tar", last modified: Fri May 17 20:22:06 2024, max compression
```

## Comparing `balsamic-0.0.13.tar` & `balsamic-0.0.14.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 witchdoc  (1000) witchdoc  (1001)        0 2024-05-17 20:18:28.757354 balsamic-0.0.13/
--rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)     2109 2024-05-17 20:18:28.757354 balsamic-0.0.13/PKG-INFO
--rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)     1574 2024-05-17 19:32:39.000000 balsamic-0.0.13/README.md
-drwxr-xr-x   0 witchdoc  (1000) witchdoc  (1001)        0 2024-05-17 20:18:28.757354 balsamic-0.0.13/balsamic/
--rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)        1 2024-05-17 19:32:39.000000 balsamic-0.0.13/balsamic/__innit__.py
--rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)     3503 2024-05-17 19:32:39.000000 balsamic-0.0.13/balsamic/balsamic.py
-drwxr-xr-x   0 witchdoc  (1000) witchdoc  (1001)        0 2024-05-17 20:18:28.757354 balsamic-0.0.13/balsamic.egg-info/
--rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)     2109 2024-05-17 20:18:28.000000 balsamic-0.0.13/balsamic.egg-info/PKG-INFO
--rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)      220 2024-05-17 20:18:28.000000 balsamic-0.0.13/balsamic.egg-info/SOURCES.txt
--rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)        1 2024-05-17 20:18:28.000000 balsamic-0.0.13/balsamic.egg-info/dependency_links.txt
--rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)        9 2024-05-17 20:18:28.000000 balsamic-0.0.13/balsamic.egg-info/requires.txt
--rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)        9 2024-05-17 20:18:28.000000 balsamic-0.0.13/balsamic.egg-info/top_level.txt
--rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)       38 2024-05-17 20:18:28.757354 balsamic-0.0.13/setup.cfg
--rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)     1159 2024-05-17 20:18:26.000000 balsamic-0.0.13/setup.py
+drwxr-xr-x   0 witchdoc  (1000) witchdoc  (1001)        0 2024-05-17 20:22:06.344276 balsamic-0.0.14/
+-rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)     2109 2024-05-17 20:22:06.344276 balsamic-0.0.14/PKG-INFO
+-rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)     1574 2024-05-17 19:32:39.000000 balsamic-0.0.14/README.md
+drwxr-xr-x   0 witchdoc  (1000) witchdoc  (1001)        0 2024-05-17 20:22:06.344276 balsamic-0.0.14/balsamic/
+-rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)        1 2024-05-17 19:32:39.000000 balsamic-0.0.14/balsamic/__innit__.py
+-rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)     3503 2024-05-17 19:32:39.000000 balsamic-0.0.14/balsamic/balsamic.py
+drwxr-xr-x   0 witchdoc  (1000) witchdoc  (1001)        0 2024-05-17 20:22:06.344276 balsamic-0.0.14/balsamic.egg-info/
+-rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)     2109 2024-05-17 20:22:06.000000 balsamic-0.0.14/balsamic.egg-info/PKG-INFO
+-rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)      220 2024-05-17 20:22:06.000000 balsamic-0.0.14/balsamic.egg-info/SOURCES.txt
+-rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)        1 2024-05-17 20:22:06.000000 balsamic-0.0.14/balsamic.egg-info/dependency_links.txt
+-rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)        9 2024-05-17 20:22:06.000000 balsamic-0.0.14/balsamic.egg-info/requires.txt
+-rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)        9 2024-05-17 20:22:06.000000 balsamic-0.0.14/balsamic.egg-info/top_level.txt
+-rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)       38 2024-05-17 20:22:06.344276 balsamic-0.0.14/setup.cfg
+-rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)     1144 2024-05-17 20:22:03.000000 balsamic-0.0.14/setup.py
```

### Comparing `balsamic-0.0.13/PKG-INFO` & `balsamic-0.0.14/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: balsamic
-Version: 0.0.13
+Version: 0.0.14
 Summary: Send malicious pickles via requests or sockets
 Author: Witchdoctor (malectrica)
 Keywords: python,hack,pickle,serialization,security,sockets,web
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
```

### Comparing `balsamic-0.0.13/README.md` & `balsamic-0.0.14/README.md`

 * *Files identical despite different names*

### Comparing `balsamic-0.0.13/balsamic/balsamic.py` & `balsamic-0.0.14/balsamic/balsamic.py`

 * *Files identical despite different names*

### Comparing `balsamic-0.0.13/balsamic.egg-info/PKG-INFO` & `balsamic-0.0.14/balsamic.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: balsamic
-Version: 0.0.13
+Version: 0.0.14
 Summary: Send malicious pickles via requests or sockets
 Author: Witchdoctor (malectrica)
 Keywords: python,hack,pickle,serialization,security,sockets,web
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
```

### Comparing `balsamic-0.0.13/setup.py` & `balsamic-0.0.14/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,17 +1,17 @@
-from setuptools import setup, find_packages
+from setuptools import setup
 import codecs
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '0.0.13'
+VERSION = '0.0.14'
 DESCRIPTION = 'Send malicious pickles via requests or sockets'
 LONG_DESCRIPTION = 'A package that allows the user to easily send out malicious pickles, via web requests, or a malicious server or client(currently ipv4 only)'
 
 # Setting up
 setup(
     name="balsamic",
     version=VERSION,
```

