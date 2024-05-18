# Comparing `tmp/balsamic-0.1.5.tar.gz` & `tmp/balsamic-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "balsamic-0.1.5.tar", last modified: Fri May 17 23:32:39 2024, max compression
+gzip compressed data, was "balsamic-0.1.6.tar", last modified: Fri May 17 23:34:49 2024, max compression
```

## Comparing `balsamic-0.1.5.tar` & `balsamic-0.1.6.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 witchdoc  (1000) witchdoc  (1001)        0 2024-05-17 23:32:39.417243 balsamic-0.1.5/
--rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)     2138 2024-05-17 23:32:39.417243 balsamic-0.1.5/PKG-INFO
--rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)     1604 2024-05-17 23:29:20.000000 balsamic-0.1.5/README.md
-drwxr-xr-x   0 witchdoc  (1000) witchdoc  (1001)        0 2024-05-17 23:32:39.417243 balsamic-0.1.5/balsamic/
--rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)        1 2024-05-17 19:32:39.000000 balsamic-0.1.5/balsamic/__innit__.py
--rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)     2040 2024-05-17 23:32:19.000000 balsamic-0.1.5/balsamic/__main__.py
--rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)     1482 2024-05-17 23:02:34.000000 balsamic-0.1.5/balsamic/balsamic.py
-drwxr-xr-x   0 witchdoc  (1000) witchdoc  (1001)        0 2024-05-17 23:32:39.417243 balsamic-0.1.5/balsamic.egg-info/
--rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)     2138 2024-05-17 23:32:39.000000 balsamic-0.1.5/balsamic.egg-info/PKG-INFO
--rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)      241 2024-05-17 23:32:39.000000 balsamic-0.1.5/balsamic.egg-info/SOURCES.txt
--rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)        1 2024-05-17 23:32:39.000000 balsamic-0.1.5/balsamic.egg-info/dependency_links.txt
--rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)        9 2024-05-17 23:32:39.000000 balsamic-0.1.5/balsamic.egg-info/requires.txt
--rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)        9 2024-05-17 23:32:39.000000 balsamic-0.1.5/balsamic.egg-info/top_level.txt
--rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)       38 2024-05-17 23:32:39.417243 balsamic-0.1.5/setup.cfg
--rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)     1143 2024-05-17 23:32:23.000000 balsamic-0.1.5/setup.py
+drwxr-xr-x   0 witchdoc  (1000) witchdoc  (1001)        0 2024-05-17 23:34:49.478970 balsamic-0.1.6/
+-rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)     2138 2024-05-17 23:34:49.478970 balsamic-0.1.6/PKG-INFO
+-rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)     1604 2024-05-17 23:29:20.000000 balsamic-0.1.6/README.md
+drwxr-xr-x   0 witchdoc  (1000) witchdoc  (1001)        0 2024-05-17 23:34:49.478970 balsamic-0.1.6/balsamic/
+-rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)        1 2024-05-17 19:32:39.000000 balsamic-0.1.6/balsamic/__innit__.py
+-rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)     2064 2024-05-17 23:34:22.000000 balsamic-0.1.6/balsamic/__main__.py
+-rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)     1482 2024-05-17 23:02:34.000000 balsamic-0.1.6/balsamic/balsamic.py
+drwxr-xr-x   0 witchdoc  (1000) witchdoc  (1001)        0 2024-05-17 23:34:49.478970 balsamic-0.1.6/balsamic.egg-info/
+-rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)     2138 2024-05-17 23:34:49.000000 balsamic-0.1.6/balsamic.egg-info/PKG-INFO
+-rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)      241 2024-05-17 23:34:49.000000 balsamic-0.1.6/balsamic.egg-info/SOURCES.txt
+-rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)        1 2024-05-17 23:34:49.000000 balsamic-0.1.6/balsamic.egg-info/dependency_links.txt
+-rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)        9 2024-05-17 23:34:49.000000 balsamic-0.1.6/balsamic.egg-info/requires.txt
+-rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)        9 2024-05-17 23:34:49.000000 balsamic-0.1.6/balsamic.egg-info/top_level.txt
+-rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)       38 2024-05-17 23:34:49.478970 balsamic-0.1.6/setup.cfg
+-rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)     1143 2024-05-17 23:34:33.000000 balsamic-0.1.6/setup.py
```

### Comparing `balsamic-0.1.5/PKG-INFO` & `balsamic-0.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: balsamic
-Version: 0.1.5
+Version: 0.1.6
 Summary: Send malicious pickles via requests or sockets
 Author: Witchdoctor (malectrica)
 Keywords: python,hack,pickle,serialization,security,sockets,web
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
```

### Comparing `balsamic-0.1.5/README.md` & `balsamic-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `balsamic-0.1.5/balsamic/__main__.py` & `balsamic-0.1.6/balsamic/__main__.py`

 * *Files 10% similar despite different names*

```diff
@@ -24,22 +24,22 @@
 
 		#create subparser for socksend attack
 		socksendparser=subparse.add_parser("socksend")
 		socksendparser.add_argument("-rh","--rhost",required=True)
 		socksendparser.add_argument("-rp","--rport",required=True)
 		socksendparser.add_argument("-P","--payload",required=True)
 		socksendparser.add_argument("-c","--command")
-		socksendparser.add_argument("-s","--steps")
+		socksendparser.add_argument("-s","--steps",default="0")
 
 		#create subparser for socklisten attack
 		socklistenparser=subparse.add_parser("socklisten")
 		socklistenparser.add_argument("-lp","--lport",required=True)
 		socklistenparser.add_argument("-P","--payload",required=True)
 		socklistenparser.add_argument("-c","--command")
-		socklistenparser.add_argument("-s","--steps")
+		socklistenparser.add_argument("-s","--steps",default="0")
 		
 		#return parsed arguments
 		args = parser.parse_args()
 		return args
 
 	args=parser()
 	if args.command:
```

### Comparing `balsamic-0.1.5/balsamic/balsamic.py` & `balsamic-0.1.6/balsamic/balsamic.py`

 * *Files identical despite different names*

### Comparing `balsamic-0.1.5/balsamic.egg-info/PKG-INFO` & `balsamic-0.1.6/balsamic.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: balsamic
-Version: 0.1.5
+Version: 0.1.6
 Summary: Send malicious pickles via requests or sockets
 Author: Witchdoctor (malectrica)
 Keywords: python,hack,pickle,serialization,security,sockets,web
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
```

### Comparing `balsamic-0.1.5/setup.py` & `balsamic-0.1.6/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '0.1.5'
+VERSION = '0.1.6'
 DESCRIPTION = 'Send malicious pickles via requests or sockets'
 LONG_DESCRIPTION = 'A package that allows the user to easily send out malicious pickles, via web requests, or a malicious server or client(currently ipv4 only)'
 
 # Setting up
 setup(
     name="balsamic",
     version=VERSION,
```

