# Comparing `tmp/markrunner_server-0.1.5.tar.gz` & `tmp/markrunner_server-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "markrunner_server-0.1.5.tar", max compression
+gzip compressed data, was "markrunner_server-0.1.6.tar", max compression
```

## Comparing `markrunner_server-0.1.5.tar` & `markrunner_server-0.1.6.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0       20 2024-05-18 08:40:20.585620 markrunner_server-0.1.5/README.md
--rw-r--r--   0        0        0     2120 2024-05-18 09:44:44.872792 markrunner_server-0.1.5/main.py
--rw-r--r--   0        0        0      463 2024-05-18 09:44:47.776804 markrunner_server-0.1.5/pyproject.toml
--rw-r--r--   0        0        0      453 1970-01-01 00:00:00.000000 markrunner_server-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0       20 2024-05-18 08:40:20.585620 markrunner_server-0.1.6/README.md
+-rw-r--r--   0        0        0     2160 2024-05-18 09:55:27.267088 markrunner_server-0.1.6/__main__.py
+-rw-r--r--   0        0        0      412 2024-05-18 09:55:17.463620 markrunner_server-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0      453 1970-01-01 00:00:00.000000 markrunner_server-0.1.6/PKG-INFO
```

### Comparing `markrunner_server-0.1.5/main.py` & `markrunner_server-0.1.6/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 
 import os
 
 from jupyter_server.base.handlers import JupyterHandler
 from jupyter_server.extension.handler import ExtensionHandlerMixin
 from jupyterlab_server import LabServerApp
 
-__version__ = "0.1.5"
+__version__ = "0.1.6"
 
 
 def _jupyter_server_extension_points():
     return [{"module": __name__, "app": MarkrunnerApp}]
 
 
 class InfoHandler(ExtensionHandlerMixin, JupyterHandler):
@@ -58,7 +58,11 @@
 
 
 def main():
     if os.environ.get("MARKRUNNER_SERVER_VERSION") != __version__:
         raise ValueError("Version mismatch")
 
     MarkrunnerApp.launch_instance()
+
+
+if __name__ == "__main__":
+    main()
```

