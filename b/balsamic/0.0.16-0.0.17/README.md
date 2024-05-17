# Comparing `tmp/balsamic-0.0.16.tar.gz` & `tmp/balsamic-0.0.17.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "balsamic-0.0.16.tar", last modified: Fri May 17 22:48:26 2024, max compression
+gzip compressed data, was "balsamic-0.0.17.tar", last modified: Fri May 17 22:51:16 2024, max compression
```

## Comparing `balsamic-0.0.16.tar` & `balsamic-0.0.17.tar`

### file list

```diff
@@ -1,15 +1,14 @@
-drwxr-xr-x   0 witchdoc  (1000) witchdoc  (1001)        0 2024-05-17 22:48:26.429875 balsamic-0.0.16/
--rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)     2109 2024-05-17 22:48:26.429875 balsamic-0.0.16/PKG-INFO
--rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)     1574 2024-05-17 19:32:39.000000 balsamic-0.0.16/README.md
-drwxr-xr-x   0 witchdoc  (1000) witchdoc  (1001)        0 2024-05-17 22:48:26.429875 balsamic-0.0.16/balsamic/
--rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)        1 2024-05-17 19:32:39.000000 balsamic-0.0.16/balsamic/__innit__.py
--rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)     2017 2024-05-17 22:47:27.000000 balsamic-0.0.16/balsamic/__main__.py
--rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)     1483 2024-05-17 22:47:40.000000 balsamic-0.0.16/balsamic/balsamic.py
-drwxr-xr-x   0 witchdoc  (1000) witchdoc  (1001)        0 2024-05-17 22:48:26.429875 balsamic-0.0.16/balsamic.egg-info/
--rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)     2109 2024-05-17 22:48:26.000000 balsamic-0.0.16/balsamic.egg-info/PKG-INFO
--rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)      241 2024-05-17 22:48:26.000000 balsamic-0.0.16/balsamic.egg-info/SOURCES.txt
--rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)        1 2024-05-17 22:48:26.000000 balsamic-0.0.16/balsamic.egg-info/dependency_links.txt
--rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)        9 2024-05-17 22:48:26.000000 balsamic-0.0.16/balsamic.egg-info/requires.txt
--rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)        9 2024-05-17 22:48:26.000000 balsamic-0.0.16/balsamic.egg-info/top_level.txt
--rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)       38 2024-05-17 22:48:26.429875 balsamic-0.0.16/setup.cfg
--rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)     1144 2024-05-17 22:47:58.000000 balsamic-0.0.16/setup.py
+drwxr-xr-x   0 witchdoc  (1000) witchdoc  (1001)        0 2024-05-17 22:51:16.428136 balsamic-0.0.17/
+-rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)     2109 2024-05-17 22:51:16.428136 balsamic-0.0.17/PKG-INFO
+-rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)     1574 2024-05-17 19:32:39.000000 balsamic-0.0.17/README.md
+drwxr-xr-x   0 witchdoc  (1000) witchdoc  (1001)        0 2024-05-17 22:51:16.428136 balsamic-0.0.17/balsamic/
+-rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)        1 2024-05-17 19:32:39.000000 balsamic-0.0.17/balsamic/__innit__.py
+-rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)     3503 2024-05-17 22:50:44.000000 balsamic-0.0.17/balsamic/__main__.py
+drwxr-xr-x   0 witchdoc  (1000) witchdoc  (1001)        0 2024-05-17 22:51:16.428136 balsamic-0.0.17/balsamic.egg-info/
+-rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)     2109 2024-05-17 22:51:16.000000 balsamic-0.0.17/balsamic.egg-info/PKG-INFO
+-rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)      220 2024-05-17 22:51:16.000000 balsamic-0.0.17/balsamic.egg-info/SOURCES.txt
+-rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)        1 2024-05-17 22:51:16.000000 balsamic-0.0.17/balsamic.egg-info/dependency_links.txt
+-rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)        9 2024-05-17 22:51:16.000000 balsamic-0.0.17/balsamic.egg-info/requires.txt
+-rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)        9 2024-05-17 22:51:16.000000 balsamic-0.0.17/balsamic.egg-info/top_level.txt
+-rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)       38 2024-05-17 22:51:16.428136 balsamic-0.0.17/setup.cfg
+-rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)     1144 2024-05-17 22:50:50.000000 balsamic-0.0.17/setup.py
```

### Comparing `balsamic-0.0.16/PKG-INFO` & `balsamic-0.0.17/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: balsamic
-Version: 0.0.16
+Version: 0.0.17
 Summary: Send malicious pickles via requests or sockets
 Author: Witchdoctor (malectrica)
 Keywords: python,hack,pickle,serialization,security,sockets,web
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
```

### Comparing `balsamic-0.0.16/README.md` & `balsamic-0.0.17/README.md`

 * *Files identical despite different names*

### Comparing `balsamic-0.0.16/balsamic.egg-info/PKG-INFO` & `balsamic-0.0.17/balsamic.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: balsamic
-Version: 0.0.16
+Version: 0.0.17
 Summary: Send malicious pickles via requests or sockets
 Author: Witchdoctor (malectrica)
 Keywords: python,hack,pickle,serialization,security,sockets,web
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
```

### Comparing `balsamic-0.0.16/setup.py` & `balsamic-0.0.17/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '0.0.16'
+VERSION = '0.0.17'
 DESCRIPTION = 'Send malicious pickles via requests or sockets'
 LONG_DESCRIPTION = 'A package that allows the user to easily send out malicious pickles, via web requests, or a malicious server or client(currently ipv4 only)'
 
 # Setting up
 setup(
     name="balsamic",
     version=VERSION,
```

