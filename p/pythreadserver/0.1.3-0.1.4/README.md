# Comparing `tmp/pythreadserver-0.1.3.tar.gz` & `tmp/pythreadserver-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pythreadserver-0.1.3.tar", last modified: Sat May 11 10:58:44 2024, max compression
+gzip compressed data, was "pythreadserver-0.1.4.tar", last modified: Sat May 18 16:34:59 2024, max compression
```

## Comparing `pythreadserver-0.1.3.tar` & `pythreadserver-0.1.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-05-11 10:58:44.634315 pythreadserver-0.1.3/
--rw-rw-rw-   0        0        0      512 2024-05-11 10:58:44.634315 pythreadserver-0.1.3/PKG-INFO
--rw-rw-rw-   0        0        0      192 2024-05-11 10:23:05.000000 pythreadserver-0.1.3/README.md
-drwxrwxrwx   0        0        0        0 2024-05-11 10:58:44.618297 pythreadserver-0.1.3/pythreadserver/
--rw-rw-rw-   0        0        0       60 2024-05-11 10:43:35.000000 pythreadserver-0.1.3/pythreadserver/__init__.py
--rw-rw-rw-   0        0        0     3371 2024-05-11 10:43:35.000000 pythreadserver-0.1.3/pythreadserver/client.py
--rw-rw-rw-   0        0        0      115 2024-05-11 10:43:35.000000 pythreadserver-0.1.3/pythreadserver/constants.py
--rw-rw-rw-   0        0        0     4995 2024-05-11 10:43:35.000000 pythreadserver-0.1.3/pythreadserver/server.py
--rw-rw-rw-   0        0        0      561 2024-05-11 10:43:35.000000 pythreadserver-0.1.3/pythreadserver/textlog.py
-drwxrwxrwx   0        0        0        0 2024-05-11 10:58:44.633315 pythreadserver-0.1.3/pythreadserver.egg-info/
--rw-rw-rw-   0        0        0      512 2024-05-11 10:58:44.000000 pythreadserver-0.1.3/pythreadserver.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      301 2024-05-11 10:58:44.000000 pythreadserver-0.1.3/pythreadserver.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-11 10:58:44.000000 pythreadserver-0.1.3/pythreadserver.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2024-05-11 10:58:44.000000 pythreadserver-0.1.3/pythreadserver.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-11 10:58:44.634315 pythreadserver-0.1.3/setup.cfg
--rw-rw-rw-   0        0        0      781 2024-05-11 10:57:35.000000 pythreadserver-0.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-18 16:34:59.644030 pythreadserver-0.1.4/
+-rw-rw-rw-   0        0        0      512 2024-05-18 16:34:59.644030 pythreadserver-0.1.4/PKG-INFO
+-rw-rw-rw-   0        0        0      192 2024-05-11 10:23:05.000000 pythreadserver-0.1.4/README.md
+drwxrwxrwx   0        0        0        0 2024-05-18 16:34:59.634147 pythreadserver-0.1.4/pythreadserver/
+-rw-rw-rw-   0        0        0       60 2024-05-11 10:43:35.000000 pythreadserver-0.1.4/pythreadserver/__init__.py
+-rw-rw-rw-   0        0        0     3312 2024-05-17 17:27:10.000000 pythreadserver-0.1.4/pythreadserver/client.py
+-rw-rw-rw-   0        0        0      115 2024-05-17 17:38:09.000000 pythreadserver-0.1.4/pythreadserver/constants.py
+-rw-rw-rw-   0        0        0     4994 2024-05-17 20:19:39.000000 pythreadserver-0.1.4/pythreadserver/server.py
+-rw-rw-rw-   0        0        0      561 2024-05-11 10:43:35.000000 pythreadserver-0.1.4/pythreadserver/textlog.py
+drwxrwxrwx   0        0        0        0 2024-05-18 16:34:59.643030 pythreadserver-0.1.4/pythreadserver.egg-info/
+-rw-rw-rw-   0        0        0      512 2024-05-18 16:34:59.000000 pythreadserver-0.1.4/pythreadserver.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      301 2024-05-18 16:34:59.000000 pythreadserver-0.1.4/pythreadserver.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-18 16:34:59.000000 pythreadserver-0.1.4/pythreadserver.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2024-05-18 16:34:59.000000 pythreadserver-0.1.4/pythreadserver.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-18 16:34:59.644030 pythreadserver-0.1.4/setup.cfg
+-rw-rw-rw-   0        0        0      781 2024-05-18 16:32:02.000000 pythreadserver-0.1.4/setup.py
```

### Comparing `pythreadserver-0.1.3/PKG-INFO` & `pythreadserver-0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pythreadserver
-Version: 0.1.3
+Version: 0.1.4
 Summary: Socket-based server package
 Author: rain1107
 Author-email: ryanbays@icloud.com
 Keywords: python,socket,threading
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pythreadserver-0.1.3/pythreadserver/client.py` & `pythreadserver-0.1.4/pythreadserver/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,41 +2,40 @@
 import threading
 import time
 from .textlog import Log
 from .constants import *
 
 
 class Client:
-    def __init__(self, ip, **kwargs):
+    def __init__(self, **kwargs):
         output_to_console = True
         log_path = ""
         if "console" in kwargs:
             output_to_console = kwargs["console"]
         if "log_path" in kwargs:
             log_path = kwargs["log_path"]
 
-        self.ip = ip
-        if self.ip == "" or self.ip == "localhost":
-            self.ip = socket.gethostname()
         self.__listeners = []
         self.packets = []
         self.log = Log(output_to_console, log_path)
         self.socket_out = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
         self.socket_in = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
         self.send_loop_thread = None
         self.recv_loop_thread = None
         self.connected = False
 
         self.runtime = time.time()
 
-    def connect(self):
+    def connect(self, ip):
+        if ip == "localhost":
+            ip = socket.gethostname()
         self.log.log("Connecting to server...")
         try:
-            self.socket_in.connect((self.ip, PORT_S_TO_C))
-            self.socket_out.connect((self.ip, PORT_C_TO_S))
+            self.socket_in.connect((ip, PORT_S_TO_C))
+            self.socket_out.connect((ip, PORT_C_TO_S))
         except ConnectionRefusedError:
             self.log.log("Error: Connection refused")
             return 1
         self.log.log("Connected to server.")
         self.connected = True
         self.log.log("Initialising handling threads...")
         self.send_loop_thread = threading.Thread(target=self.send_loop)
```

### Comparing `pythreadserver-0.1.3/pythreadserver/server.py` & `pythreadserver-0.1.4/pythreadserver/server.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 
     def run(self):
         self.send_loop_thread = threading.Thread(target=self.send_loop)
         self.send_loop_thread.start()
         self.recv_loop_thread = threading.Thread(target=self.recv_loop)
         self.recv_loop_thread.start()
 
-    def send_loop(self,):
+    def send_loop(self):
         while self.connected:
             try:
                 self.server.client_send(self)
             except ConnectionResetError:
                 self.connected = False
                 self.close()
                 break
```

### Comparing `pythreadserver-0.1.3/pythreadserver/textlog.py` & `pythreadserver-0.1.4/pythreadserver/textlog.py`

 * *Files identical despite different names*

### Comparing `pythreadserver-0.1.3/pythreadserver.egg-info/PKG-INFO` & `pythreadserver-0.1.4/pythreadserver.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pythreadserver
-Version: 0.1.3
+Version: 0.1.4
 Summary: Socket-based server package
 Author: rain1107
 Author-email: ryanbays@icloud.com
 Keywords: python,socket,threading
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pythreadserver-0.1.3/setup.py` & `pythreadserver-0.1.4/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.1.3'
+VERSION = '0.1.4'
 DESCRIPTION = 'Socket-based server package'
 LONG_DESCRIPTION = ''
 
 # Setting up
 setup(
     name="pythreadserver",
     version=VERSION,
```

