# Comparing `tmp/balsamic-0.1.9.tar.gz` & `tmp/balsamic-0.1.91.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "balsamic-0.1.9.tar", last modified: Sat May 18 02:48:43 2024, max compression
+gzip compressed data, was "balsamic-0.1.91.tar", last modified: Sat May 18 02:51:07 2024, max compression
```

## Comparing `balsamic-0.1.9.tar` & `balsamic-0.1.91.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 witchdoc  (1000) witchdoc  (1001)        0 2024-05-18 02:48:43.186732 balsamic-0.1.9/
--rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)     2138 2024-05-18 02:48:43.186732 balsamic-0.1.9/PKG-INFO
--rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)     1604 2024-05-17 23:29:20.000000 balsamic-0.1.9/README.md
-drwxr-xr-x   0 witchdoc  (1000) witchdoc  (1001)        0 2024-05-18 02:48:43.186732 balsamic-0.1.9/balsamic/
--rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)        1 2024-05-17 19:32:39.000000 balsamic-0.1.9/balsamic/__innit__.py
--rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)     2202 2024-05-18 02:48:20.000000 balsamic-0.1.9/balsamic/__main__.py
--rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)     1579 2024-05-18 02:43:55.000000 balsamic-0.1.9/balsamic/balsamic.py
-drwxr-xr-x   0 witchdoc  (1000) witchdoc  (1001)        0 2024-05-18 02:48:43.186732 balsamic-0.1.9/balsamic.egg-info/
--rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)     2138 2024-05-18 02:48:43.000000 balsamic-0.1.9/balsamic.egg-info/PKG-INFO
--rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)      241 2024-05-18 02:48:43.000000 balsamic-0.1.9/balsamic.egg-info/SOURCES.txt
--rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)        1 2024-05-18 02:48:43.000000 balsamic-0.1.9/balsamic.egg-info/dependency_links.txt
--rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)        9 2024-05-18 02:48:43.000000 balsamic-0.1.9/balsamic.egg-info/requires.txt
--rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)        9 2024-05-18 02:48:43.000000 balsamic-0.1.9/balsamic.egg-info/top_level.txt
--rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)       38 2024-05-18 02:48:43.186732 balsamic-0.1.9/setup.cfg
--rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)     1143 2024-05-18 02:48:24.000000 balsamic-0.1.9/setup.py
+drwxr-xr-x   0 witchdoc  (1000) witchdoc  (1001)        0 2024-05-18 02:51:07.252658 balsamic-0.1.91/
+-rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)     2139 2024-05-18 02:51:07.252658 balsamic-0.1.91/PKG-INFO
+-rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)     1604 2024-05-17 23:29:20.000000 balsamic-0.1.91/README.md
+drwxr-xr-x   0 witchdoc  (1000) witchdoc  (1001)        0 2024-05-18 02:51:07.252658 balsamic-0.1.91/balsamic/
+-rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)        1 2024-05-17 19:32:39.000000 balsamic-0.1.91/balsamic/__innit__.py
+-rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)     2226 2024-05-18 02:50:42.000000 balsamic-0.1.91/balsamic/__main__.py
+-rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)     1579 2024-05-18 02:50:09.000000 balsamic-0.1.91/balsamic/balsamic.py
+drwxr-xr-x   0 witchdoc  (1000) witchdoc  (1001)        0 2024-05-18 02:51:07.252658 balsamic-0.1.91/balsamic.egg-info/
+-rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)     2139 2024-05-18 02:51:07.000000 balsamic-0.1.91/balsamic.egg-info/PKG-INFO
+-rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)      241 2024-05-18 02:51:07.000000 balsamic-0.1.91/balsamic.egg-info/SOURCES.txt
+-rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)        1 2024-05-18 02:51:07.000000 balsamic-0.1.91/balsamic.egg-info/dependency_links.txt
+-rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)        9 2024-05-18 02:51:07.000000 balsamic-0.1.91/balsamic.egg-info/requires.txt
+-rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)        9 2024-05-18 02:51:07.000000 balsamic-0.1.91/balsamic.egg-info/top_level.txt
+-rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)       38 2024-05-18 02:51:07.252658 balsamic-0.1.91/setup.cfg
+-rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)     1144 2024-05-18 02:50:50.000000 balsamic-0.1.91/setup.py
```

### Comparing `balsamic-0.1.9/PKG-INFO` & `balsamic-0.1.91/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: balsamic
-Version: 0.1.9
+Version: 0.1.91
 Summary: Send malicious pickles via requests or sockets
 Author: Witchdoctor (malectrica)
 Keywords: python,hack,pickle,serialization,security,sockets,web
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
```

### Comparing `balsamic-0.1.9/README.md` & `balsamic-0.1.91/README.md`

 * *Files identical despite different names*

### Comparing `balsamic-0.1.9/balsamic/__main__.py` & `balsamic-0.1.91/balsamic/__main__.py`

 * *Files 0% similar despite different names*

```diff
@@ -46,10 +46,10 @@
 	args=parser()
 	if args.command:
 		balsamic.updatecmd(args.command)
 
 	if args.attack == "webreq":
 		balsamic.webreq(args.schema,args.method,args.rhost,args.rport,args.payload,args.parameter,args.cookie)
 	elif args.attack == "socksend":
-		balsamic.socksend(args.rhost,args.rport,args.payload,args.steps)
+		balsamic.socksend(args.rhost,args.rport,args.payload,args.encode,args.steps)
 	elif args.attack == "socklisten":
-		balsamic.socklisten(args.lport,args.payload,args.steps)
+		balsamic.socklisten(args.lport,args.payload,args.encode,args.steps)
```

### Comparing `balsamic-0.1.9/balsamic/balsamic.py` & `balsamic-0.1.91/balsamic/balsamic.py`

 * *Files identical despite different names*

### Comparing `balsamic-0.1.9/balsamic.egg-info/PKG-INFO` & `balsamic-0.1.91/balsamic.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: balsamic
-Version: 0.1.9
+Version: 0.1.91
 Summary: Send malicious pickles via requests or sockets
 Author: Witchdoctor (malectrica)
 Keywords: python,hack,pickle,serialization,security,sockets,web
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
```

### Comparing `balsamic-0.1.9/setup.py` & `balsamic-0.1.91/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '0.1.9'
+VERSION = '0.1.91'
 DESCRIPTION = 'Send malicious pickles via requests or sockets'
 LONG_DESCRIPTION = 'A package that allows the user to easily send out malicious pickles, via web requests, or a malicious server or client(currently ipv4 only)'
 
 # Setting up
 setup(
     name="balsamic",
     version=VERSION,
```

