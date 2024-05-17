# Comparing `tmp/balsamic-0.1.0.tar.gz` & `tmp/balsamic-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "balsamic-0.1.0.tar", last modified: Fri May 17 23:11:43 2024, max compression
+gzip compressed data, was "balsamic-0.1.1.tar", last modified: Fri May 17 23:16:45 2024, max compression
```

## Comparing `balsamic-0.1.0.tar` & `balsamic-0.1.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 witchdoc  (1000) witchdoc  (1001)        0 2024-05-17 23:11:43.244483 balsamic-0.1.0/
--rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)     2108 2024-05-17 23:11:43.244483 balsamic-0.1.0/PKG-INFO
--rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)     1574 2024-05-17 19:32:39.000000 balsamic-0.1.0/README.md
-drwxr-xr-x   0 witchdoc  (1000) witchdoc  (1001)        0 2024-05-17 23:11:43.244483 balsamic-0.1.0/balsamic/
--rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)        1 2024-05-17 19:32:39.000000 balsamic-0.1.0/balsamic/__innit__.py
--rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)     2026 2024-05-17 23:11:06.000000 balsamic-0.1.0/balsamic/__main__.py
--rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)     1482 2024-05-17 23:02:34.000000 balsamic-0.1.0/balsamic/balsamic.py
-drwxr-xr-x   0 witchdoc  (1000) witchdoc  (1001)        0 2024-05-17 23:11:43.244483 balsamic-0.1.0/balsamic.egg-info/
--rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)     2108 2024-05-17 23:11:43.000000 balsamic-0.1.0/balsamic.egg-info/PKG-INFO
--rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)      241 2024-05-17 23:11:43.000000 balsamic-0.1.0/balsamic.egg-info/SOURCES.txt
--rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)        1 2024-05-17 23:11:43.000000 balsamic-0.1.0/balsamic.egg-info/dependency_links.txt
--rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)        9 2024-05-17 23:11:43.000000 balsamic-0.1.0/balsamic.egg-info/requires.txt
--rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)        9 2024-05-17 23:11:43.000000 balsamic-0.1.0/balsamic.egg-info/top_level.txt
--rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)       38 2024-05-17 23:11:43.244483 balsamic-0.1.0/setup.cfg
--rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)     1143 2024-05-17 23:11:17.000000 balsamic-0.1.0/setup.py
+drwxr-xr-x   0 witchdoc  (1000) witchdoc  (1001)        0 2024-05-17 23:16:45.008512 balsamic-0.1.1/
+-rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)     2108 2024-05-17 23:16:45.008512 balsamic-0.1.1/PKG-INFO
+-rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)     1574 2024-05-17 19:32:39.000000 balsamic-0.1.1/README.md
+drwxr-xr-x   0 witchdoc  (1000) witchdoc  (1001)        0 2024-05-17 23:16:45.008512 balsamic-0.1.1/balsamic/
+-rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)        1 2024-05-17 19:32:39.000000 balsamic-0.1.1/balsamic/__innit__.py
+-rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)     2026 2024-05-17 23:15:11.000000 balsamic-0.1.1/balsamic/__main__.py
+-rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)     1482 2024-05-17 23:02:34.000000 balsamic-0.1.1/balsamic/balsamic.py
+drwxr-xr-x   0 witchdoc  (1000) witchdoc  (1001)        0 2024-05-17 23:16:45.008512 balsamic-0.1.1/balsamic.egg-info/
+-rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)     2108 2024-05-17 23:16:44.000000 balsamic-0.1.1/balsamic.egg-info/PKG-INFO
+-rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)      241 2024-05-17 23:16:44.000000 balsamic-0.1.1/balsamic.egg-info/SOURCES.txt
+-rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)        1 2024-05-17 23:16:44.000000 balsamic-0.1.1/balsamic.egg-info/dependency_links.txt
+-rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)        9 2024-05-17 23:16:44.000000 balsamic-0.1.1/balsamic.egg-info/requires.txt
+-rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)        9 2024-05-17 23:16:44.000000 balsamic-0.1.1/balsamic.egg-info/top_level.txt
+-rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)       38 2024-05-17 23:16:45.008512 balsamic-0.1.1/setup.cfg
+-rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)     1143 2024-05-17 23:16:22.000000 balsamic-0.1.1/setup.py
```

### Comparing `balsamic-0.1.0/PKG-INFO` & `balsamic-0.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: balsamic
-Version: 0.1.0
+Version: 0.1.1
 Summary: Send malicious pickles via requests or sockets
 Author: Witchdoctor (malectrica)
 Keywords: python,hack,pickle,serialization,security,sockets,web
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
```

### Comparing `balsamic-0.1.0/README.md` & `balsamic-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `balsamic-0.1.0/balsamic/__main__.py` & `balsamic-0.1.1/balsamic/__main__.py`

 * *Files identical despite different names*

### Comparing `balsamic-0.1.0/balsamic/balsamic.py` & `balsamic-0.1.1/balsamic/balsamic.py`

 * *Files identical despite different names*

### Comparing `balsamic-0.1.0/balsamic.egg-info/PKG-INFO` & `balsamic-0.1.1/balsamic.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: balsamic
-Version: 0.1.0
+Version: 0.1.1
 Summary: Send malicious pickles via requests or sockets
 Author: Witchdoctor (malectrica)
 Keywords: python,hack,pickle,serialization,security,sockets,web
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
```

### Comparing `balsamic-0.1.0/setup.py` & `balsamic-0.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '0.1.0'
+VERSION = '0.1.1'
 DESCRIPTION = 'Send malicious pickles via requests or sockets'
 LONG_DESCRIPTION = 'A package that allows the user to easily send out malicious pickles, via web requests, or a malicious server or client(currently ipv4 only)'
 
 # Setting up
 setup(
     name="balsamic",
     version=VERSION,
```

