# Comparing `tmp/balsamic-0.1.93.tar.gz` & `tmp/balsamic-0.1.94.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "balsamic-0.1.93.tar", last modified: Sat May 18 02:57:28 2024, max compression
+gzip compressed data, was "balsamic-0.1.94.tar", last modified: Sat May 18 02:58:58 2024, max compression
```

## Comparing `balsamic-0.1.93.tar` & `balsamic-0.1.94.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 witchdoc  (1000) witchdoc  (1001)        0 2024-05-18 02:57:28.765761 balsamic-0.1.93/
--rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)     2139 2024-05-18 02:57:28.765761 balsamic-0.1.93/PKG-INFO
--rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)     1604 2024-05-17 23:29:20.000000 balsamic-0.1.93/README.md
-drwxr-xr-x   0 witchdoc  (1000) witchdoc  (1001)        0 2024-05-18 02:57:28.765761 balsamic-0.1.93/balsamic/
--rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)        1 2024-05-17 19:32:39.000000 balsamic-0.1.93/balsamic/__innit__.py
--rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)     2226 2024-05-18 02:50:42.000000 balsamic-0.1.93/balsamic/__main__.py
--rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)     1760 2024-05-18 02:57:03.000000 balsamic-0.1.93/balsamic/balsamic.py
-drwxr-xr-x   0 witchdoc  (1000) witchdoc  (1001)        0 2024-05-18 02:57:28.765761 balsamic-0.1.93/balsamic.egg-info/
--rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)     2139 2024-05-18 02:57:28.000000 balsamic-0.1.93/balsamic.egg-info/PKG-INFO
--rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)      241 2024-05-18 02:57:28.000000 balsamic-0.1.93/balsamic.egg-info/SOURCES.txt
--rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)        1 2024-05-18 02:57:28.000000 balsamic-0.1.93/balsamic.egg-info/dependency_links.txt
--rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)        9 2024-05-18 02:57:28.000000 balsamic-0.1.93/balsamic.egg-info/requires.txt
--rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)        9 2024-05-18 02:57:28.000000 balsamic-0.1.93/balsamic.egg-info/top_level.txt
--rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)       38 2024-05-18 02:57:28.765761 balsamic-0.1.93/setup.cfg
--rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)     1144 2024-05-18 02:57:07.000000 balsamic-0.1.93/setup.py
+drwxr-xr-x   0 witchdoc  (1000) witchdoc  (1001)        0 2024-05-18 02:58:58.342959 balsamic-0.1.94/
+-rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)     2139 2024-05-18 02:58:58.342959 balsamic-0.1.94/PKG-INFO
+-rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)     1604 2024-05-17 23:29:20.000000 balsamic-0.1.94/README.md
+drwxr-xr-x   0 witchdoc  (1000) witchdoc  (1001)        0 2024-05-18 02:58:58.342959 balsamic-0.1.94/balsamic/
+-rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)        1 2024-05-17 19:32:39.000000 balsamic-0.1.94/balsamic/__innit__.py
+-rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)     2226 2024-05-18 02:50:42.000000 balsamic-0.1.94/balsamic/__main__.py
+-rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)     1761 2024-05-18 02:58:30.000000 balsamic-0.1.94/balsamic/balsamic.py
+drwxr-xr-x   0 witchdoc  (1000) witchdoc  (1001)        0 2024-05-18 02:58:58.342959 balsamic-0.1.94/balsamic.egg-info/
+-rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)     2139 2024-05-18 02:58:58.000000 balsamic-0.1.94/balsamic.egg-info/PKG-INFO
+-rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)      241 2024-05-18 02:58:58.000000 balsamic-0.1.94/balsamic.egg-info/SOURCES.txt
+-rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)        1 2024-05-18 02:58:58.000000 balsamic-0.1.94/balsamic.egg-info/dependency_links.txt
+-rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)        9 2024-05-18 02:58:58.000000 balsamic-0.1.94/balsamic.egg-info/requires.txt
+-rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)        9 2024-05-18 02:58:58.000000 balsamic-0.1.94/balsamic.egg-info/top_level.txt
+-rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)       38 2024-05-18 02:58:58.342959 balsamic-0.1.94/setup.cfg
+-rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)     1144 2024-05-18 02:58:34.000000 balsamic-0.1.94/setup.py
```

### Comparing `balsamic-0.1.93/PKG-INFO` & `balsamic-0.1.94/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: balsamic
-Version: 0.1.93
+Version: 0.1.94
 Summary: Send malicious pickles via requests or sockets
 Author: Witchdoctor (malectrica)
 Keywords: python,hack,pickle,serialization,security,sockets,web
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
```

### Comparing `balsamic-0.1.93/README.md` & `balsamic-0.1.94/README.md`

 * *Files identical despite different names*

### Comparing `balsamic-0.1.93/balsamic/__main__.py` & `balsamic-0.1.94/balsamic/__main__.py`

 * *Files identical despite different names*

### Comparing `balsamic-0.1.93/balsamic/balsamic.py` & `balsamic-0.1.94/balsamic/balsamic.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 class utility:
 	command=""
 
 	def b64pickle(payload):
 		p=getattr(payloads,payload)
 		p=base64.b64encode(pickle.dumps(p()))
 		return p
-	def plainpickle(payload)
+	def plainpickle(payload):
 		p=getattr(payloads,payload)
 		p=p.encode("utf-8")
 		return p
 
 class payloads:
 	class oscmd:
 		def __reduce__(self):
```

### Comparing `balsamic-0.1.93/balsamic.egg-info/PKG-INFO` & `balsamic-0.1.94/balsamic.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: balsamic
-Version: 0.1.93
+Version: 0.1.94
 Summary: Send malicious pickles via requests or sockets
 Author: Witchdoctor (malectrica)
 Keywords: python,hack,pickle,serialization,security,sockets,web
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
```

### Comparing `balsamic-0.1.93/setup.py` & `balsamic-0.1.94/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '0.1.93'
+VERSION = '0.1.94'
 DESCRIPTION = 'Send malicious pickles via requests or sockets'
 LONG_DESCRIPTION = 'A package that allows the user to easily send out malicious pickles, via web requests, or a malicious server or client(currently ipv4 only)'
 
 # Setting up
 setup(
     name="balsamic",
     version=VERSION,
```

