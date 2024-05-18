# Comparing `tmp/StdioBridge-1.1.0.tar.gz` & `tmp/StdioBridge-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "StdioBridge-1.1.0.tar", last modified: Fri May 17 19:59:01 2024, max compression
+gzip compressed data, was "StdioBridge-1.2.0.tar", last modified: Sat May 18 12:16:30 2024, max compression
```

## Comparing `StdioBridge-1.1.0.tar` & `StdioBridge-1.2.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 19:59:01.249398 StdioBridge-1.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-05-17 19:58:53.000000 StdioBridge-1.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3536 2024-05-17 19:59:01.249398 StdioBridge-1.1.0/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 19:59:01.249398 StdioBridge-1.1.0/StdioBridge/
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-17 19:58:53.000000 StdioBridge-1.1.0/StdioBridge/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-17 19:58:53.000000 StdioBridge-1.1.0/StdioBridge/_config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 19:59:01.249398 StdioBridge-1.1.0/StdioBridge/api/
--rw-r--r--   0 runner    (1001) docker     (127)      120 2024-05-17 19:58:53.000000 StdioBridge-1.1.0/StdioBridge/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5476 2024-05-17 19:58:53.000000 StdioBridge-1.1.0/StdioBridge/api/_api.py
--rw-r--r--   0 runner    (1001) docker     (127)      822 2024-05-17 19:58:53.000000 StdioBridge-1.1.0/StdioBridge/api/_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     2165 2024-05-17 19:58:53.000000 StdioBridge-1.1.0/StdioBridge/api/_router.py
--rw-r--r--   0 runner    (1001) docker     (127)     1424 2024-05-17 19:58:53.000000 StdioBridge-1.1.0/StdioBridge/api/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 19:59:01.249398 StdioBridge-1.1.0/StdioBridge/client/
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-05-17 19:58:53.000000 StdioBridge-1.1.0/StdioBridge/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4046 2024-05-17 19:58:53.000000 StdioBridge-1.1.0/StdioBridge/client/_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     1334 2024-05-17 19:58:53.000000 StdioBridge-1.1.0/StdioBridge/client/_response.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 19:59:01.249398 StdioBridge-1.1.0/StdioBridge.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3536 2024-05-17 19:59:01.000000 StdioBridge-1.1.0/StdioBridge.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      464 2024-05-17 19:59:01.000000 StdioBridge-1.1.0/StdioBridge.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-17 19:59:01.000000 StdioBridge-1.1.0/StdioBridge.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-17 19:59:01.000000 StdioBridge-1.1.0/StdioBridge.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-17 19:59:01.000000 StdioBridge-1.1.0/StdioBridge.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-17 19:59:01.249398 StdioBridge-1.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1170 2024-05-17 19:58:53.000000 StdioBridge-1.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 12:16:30.764418 StdioBridge-1.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-05-18 12:16:16.000000 StdioBridge-1.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3536 2024-05-18 12:16:30.764418 StdioBridge-1.2.0/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 12:16:30.764418 StdioBridge-1.2.0/StdioBridge/
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-18 12:16:16.000000 StdioBridge-1.2.0/StdioBridge/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-18 12:16:16.000000 StdioBridge-1.2.0/StdioBridge/_config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 12:16:30.764418 StdioBridge-1.2.0/StdioBridge/api/
+-rw-r--r--   0 runner    (1001) docker     (127)      179 2024-05-18 12:16:16.000000 StdioBridge-1.2.0/StdioBridge/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3676 2024-05-18 12:16:16.000000 StdioBridge-1.2.0/StdioBridge/api/_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      822 2024-05-18 12:16:16.000000 StdioBridge-1.2.0/StdioBridge/api/_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5647 2024-05-18 12:16:16.000000 StdioBridge-1.2.0/StdioBridge/api/_router.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1424 2024-05-18 12:16:16.000000 StdioBridge-1.2.0/StdioBridge/api/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 12:16:30.764418 StdioBridge-1.2.0/StdioBridge/client/
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-05-18 12:16:16.000000 StdioBridge-1.2.0/StdioBridge/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4344 2024-05-18 12:16:16.000000 StdioBridge-1.2.0/StdioBridge/client/_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1334 2024-05-18 12:16:16.000000 StdioBridge-1.2.0/StdioBridge/client/_response.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 12:16:30.764418 StdioBridge-1.2.0/StdioBridge.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3536 2024-05-18 12:16:30.000000 StdioBridge-1.2.0/StdioBridge.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      464 2024-05-18 12:16:30.000000 StdioBridge-1.2.0/StdioBridge.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-18 12:16:30.000000 StdioBridge-1.2.0/StdioBridge.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-18 12:16:30.000000 StdioBridge-1.2.0/StdioBridge.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-18 12:16:30.000000 StdioBridge-1.2.0/StdioBridge.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-18 12:16:30.764418 StdioBridge-1.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1170 2024-05-18 12:16:16.000000 StdioBridge-1.2.0/setup.py
```

### Comparing `StdioBridge-1.1.0/LICENSE` & `StdioBridge-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `StdioBridge-1.1.0/PKG-INFO` & `StdioBridge-1.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: StdioBridge
-Version: 1.1.0
+Version: 1.2.0
 Summary: A StdioBridge package.
 Home-page: https://github.com/SergeiKrivko
 Author: SergeiKrivko
 License: MIT License
         
         Copyright (c) 2024 SergeiKrivko
```

### Comparing `StdioBridge-1.1.0/StdioBridge/api/_response.py` & `StdioBridge-1.2.0/StdioBridge/api/_response.py`

 * *Files identical despite different names*

### Comparing `StdioBridge-1.1.0/StdioBridge/api/errors.py` & `StdioBridge-1.2.0/StdioBridge/api/errors.py`

 * *Files identical despite different names*

### Comparing `StdioBridge-1.1.0/StdioBridge/client/_client.py` & `StdioBridge-1.2.0/StdioBridge/client/_client.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import asyncio
 import json
 import subprocess
+import sys
 import threading
 from uuid import uuid4
 
 from StdioBridge.client._response import Response, StreamResponse
 
 
 class Client:
@@ -14,18 +15,25 @@
         self._popen: subprocess.Popen | None = None
         self._responses: dict[str: dict] = dict()
         self._streams: dict[str: list[dict]] = dict()
         self._stream_responses: dict[str: StreamResponse] = dict()
         self._thread: threading.Thread | None = None
         self._run()
 
+    def _initialize_kwargs(self):
+        if 'encoding' not in self._kwargs:
+            self._kwargs['encoding'] = 'utf-8'
+        if 'startupinfo' not in self._kwargs and sys.platform == 'win32':
+            si = subprocess.STARTUPINFO()
+            si.dwFlags |= subprocess.STARTF_USESHOWWINDOW
+            self._kwargs['startupinfo'] = si
+
     def _run(self) -> None:
         self._popen = subprocess.Popen(self._command,
                                        text=True,
-                                       encoding='utf-8',
                                        stdin=subprocess.PIPE,
                                        stdout=subprocess.PIPE,
                                        stderr=subprocess.STDOUT,
                                        **self._kwargs)
         threading.Thread(target=self._read_stdout, daemon=True).start()
 
     def terminate(self):
```

### Comparing `StdioBridge-1.1.0/StdioBridge/client/_response.py` & `StdioBridge-1.2.0/StdioBridge/client/_response.py`

 * *Files identical despite different names*

### Comparing `StdioBridge-1.1.0/StdioBridge.egg-info/PKG-INFO` & `StdioBridge-1.2.0/StdioBridge.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: StdioBridge
-Version: 1.1.0
+Version: 1.2.0
 Summary: A StdioBridge package.
 Home-page: https://github.com/SergeiKrivko
 Author: SergeiKrivko
 License: MIT License
         
         Copyright (c) 2024 SergeiKrivko
```

### Comparing `StdioBridge-1.1.0/setup.py` & `StdioBridge-1.2.0/setup.py`

 * *Files identical despite different names*

