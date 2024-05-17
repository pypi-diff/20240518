# Comparing `tmp/balsamic-0.1.1.tar.gz` & `tmp/balsamic-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "balsamic-0.1.1.tar", last modified: Fri May 17 23:16:45 2024, max compression
+gzip compressed data, was "balsamic-0.1.2.tar", last modified: Fri May 17 23:24:27 2024, max compression
```

## Comparing `balsamic-0.1.1.tar` & `balsamic-0.1.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 witchdoc  (1000) witchdoc  (1001)        0 2024-05-17 23:16:45.008512 balsamic-0.1.1/
--rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)     2108 2024-05-17 23:16:45.008512 balsamic-0.1.1/PKG-INFO
--rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)     1574 2024-05-17 19:32:39.000000 balsamic-0.1.1/README.md
-drwxr-xr-x   0 witchdoc  (1000) witchdoc  (1001)        0 2024-05-17 23:16:45.008512 balsamic-0.1.1/balsamic/
--rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)        1 2024-05-17 19:32:39.000000 balsamic-0.1.1/balsamic/__innit__.py
--rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)     2026 2024-05-17 23:15:11.000000 balsamic-0.1.1/balsamic/__main__.py
--rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)     1482 2024-05-17 23:02:34.000000 balsamic-0.1.1/balsamic/balsamic.py
-drwxr-xr-x   0 witchdoc  (1000) witchdoc  (1001)        0 2024-05-17 23:16:45.008512 balsamic-0.1.1/balsamic.egg-info/
--rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)     2108 2024-05-17 23:16:44.000000 balsamic-0.1.1/balsamic.egg-info/PKG-INFO
--rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)      241 2024-05-17 23:16:44.000000 balsamic-0.1.1/balsamic.egg-info/SOURCES.txt
--rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)        1 2024-05-17 23:16:44.000000 balsamic-0.1.1/balsamic.egg-info/dependency_links.txt
--rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)        9 2024-05-17 23:16:44.000000 balsamic-0.1.1/balsamic.egg-info/requires.txt
--rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)        9 2024-05-17 23:16:44.000000 balsamic-0.1.1/balsamic.egg-info/top_level.txt
--rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)       38 2024-05-17 23:16:45.008512 balsamic-0.1.1/setup.cfg
--rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)     1143 2024-05-17 23:16:22.000000 balsamic-0.1.1/setup.py
+drwxr-xr-x   0 witchdoc  (1000) witchdoc  (1001)        0 2024-05-17 23:24:27.246689 balsamic-0.1.2/
+-rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)     2138 2024-05-17 23:24:27.246689 balsamic-0.1.2/PKG-INFO
+-rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)     1604 2024-05-17 23:23:51.000000 balsamic-0.1.2/README.md
+drwxr-xr-x   0 witchdoc  (1000) witchdoc  (1001)        0 2024-05-17 23:24:27.246689 balsamic-0.1.2/balsamic/
+-rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)        1 2024-05-17 19:32:39.000000 balsamic-0.1.2/balsamic/__innit__.py
+-rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)     2026 2024-05-17 23:20:54.000000 balsamic-0.1.2/balsamic/__main__.py
+-rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)     1482 2024-05-17 23:02:34.000000 balsamic-0.1.2/balsamic/balsamic.py
+drwxr-xr-x   0 witchdoc  (1000) witchdoc  (1001)        0 2024-05-17 23:24:27.246689 balsamic-0.1.2/balsamic.egg-info/
+-rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)     2138 2024-05-17 23:24:27.000000 balsamic-0.1.2/balsamic.egg-info/PKG-INFO
+-rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)      241 2024-05-17 23:24:27.000000 balsamic-0.1.2/balsamic.egg-info/SOURCES.txt
+-rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)        1 2024-05-17 23:24:27.000000 balsamic-0.1.2/balsamic.egg-info/dependency_links.txt
+-rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)        9 2024-05-17 23:24:27.000000 balsamic-0.1.2/balsamic.egg-info/requires.txt
+-rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)        9 2024-05-17 23:24:27.000000 balsamic-0.1.2/balsamic.egg-info/top_level.txt
+-rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)       38 2024-05-17 23:24:27.246689 balsamic-0.1.2/setup.cfg
+-rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)     1143 2024-05-17 23:24:23.000000 balsamic-0.1.2/setup.py
```

### Comparing `balsamic-0.1.1/PKG-INFO` & `balsamic-0.1.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: balsamic
-Version: 0.1.1
+Version: 0.1.2
 Summary: Send malicious pickles via requests or sockets
 Author: Witchdoctor (malectrica)
 Keywords: python,hack,pickle,serialization,security,sockets,web
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
@@ -54,12 +54,13 @@
   -lp LPORT, --lport LPORT
   -P PAYLOAD, --payload PAYLOAD
   -c COMMAND, --command COMMAND
 ```
 
 ## useage (library)
 ```
+from balsamic import balsamic
 balsamic.utility.command="command"
 balsamic.webreq("schema","method","rhost","rport","payload","parameter","cookie")
 balsamic.socksend("ip",port,"payload",steps)
 balsamic.socklisten(port,"payload",steps)
 ```
```

### Comparing `balsamic-0.1.1/README.md` & `balsamic-0.1.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -39,12 +39,13 @@
   -lp LPORT, --lport LPORT
   -P PAYLOAD, --payload PAYLOAD
   -c COMMAND, --command COMMAND
 ```
 
 ## useage (library)
 ```
+from balsamic import balsamic
 balsamic.utility.command="command"
 balsamic.webreq("schema","method","rhost","rport","payload","parameter","cookie")
 balsamic.socksend("ip",port,"payload",steps)
 balsamic.socklisten(port,"payload",steps)
 ```
```

### Comparing `balsamic-0.1.1/balsamic/__main__.py` & `balsamic-0.1.2/balsamic/__main__.py`

 * *Files identical despite different names*

### Comparing `balsamic-0.1.1/balsamic/balsamic.py` & `balsamic-0.1.2/balsamic/balsamic.py`

 * *Files identical despite different names*

### Comparing `balsamic-0.1.1/balsamic.egg-info/PKG-INFO` & `balsamic-0.1.2/balsamic.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: balsamic
-Version: 0.1.1
+Version: 0.1.2
 Summary: Send malicious pickles via requests or sockets
 Author: Witchdoctor (malectrica)
 Keywords: python,hack,pickle,serialization,security,sockets,web
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
@@ -54,12 +54,13 @@
   -lp LPORT, --lport LPORT
   -P PAYLOAD, --payload PAYLOAD
   -c COMMAND, --command COMMAND
 ```
 
 ## useage (library)
 ```
+from balsamic import balsamic
 balsamic.utility.command="command"
 balsamic.webreq("schema","method","rhost","rport","payload","parameter","cookie")
 balsamic.socksend("ip",port,"payload",steps)
 balsamic.socklisten(port,"payload",steps)
 ```
```

### Comparing `balsamic-0.1.1/setup.py` & `balsamic-0.1.2/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '0.1.1'
+VERSION = '0.1.2'
 DESCRIPTION = 'Send malicious pickles via requests or sockets'
 LONG_DESCRIPTION = 'A package that allows the user to easily send out malicious pickles, via web requests, or a malicious server or client(currently ipv4 only)'
 
 # Setting up
 setup(
     name="balsamic",
     version=VERSION,
```

