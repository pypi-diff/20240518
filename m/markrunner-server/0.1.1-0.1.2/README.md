# Comparing `tmp/markrunner_server-0.1.1.tar.gz` & `tmp/markrunner_server-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "markrunner_server-0.1.1.tar", max compression
+gzip compressed data, was "markrunner_server-0.1.2.tar", max compression
```

## Comparing `markrunner_server-0.1.1.tar` & `markrunner_server-0.1.2.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0       20 2024-05-18 08:40:20.585620 markrunner_server-0.1.1/README.md
--rw-r--r--   0        0        0     2160 2024-05-18 09:04:50.843275 markrunner_server-0.1.1/main.py
--rw-r--r--   0        0        0      463 2024-05-18 09:05:04.100668 markrunner_server-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      453 1970-01-01 00:00:00.000000 markrunner_server-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0       20 2024-05-18 08:40:20.585620 markrunner_server-0.1.2/README.md
+-rw-r--r--   0        0        0     2160 2024-05-18 09:14:23.202459 markrunner_server-0.1.2/main.py
+-rw-r--r--   0        0        0      408 2024-05-18 09:14:17.139402 markrunner_server-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      453 1970-01-01 00:00:00.000000 markrunner_server-0.1.2/PKG-INFO
```

### Comparing `markrunner_server-0.1.1/main.py` & `markrunner_server-0.1.2/main.py`

 * *Files 5% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 
 import os
 
 from jupyter_server.base.handlers import JupyterHandler
 from jupyter_server.extension.handler import ExtensionHandlerMixin
 from jupyterlab_server import LabServerApp
 
-__version__ = "1.0.0"
+__version__ = "0.1.2"
 
 
 def _jupyter_server_extension_points():
     return [{"module": __name__, "app": MarkrunnerApp}]
 
 
 class InfoHandler(ExtensionHandlerMixin, JupyterHandler):
```

