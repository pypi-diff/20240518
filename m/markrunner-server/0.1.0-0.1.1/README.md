# Comparing `tmp/markrunner_server-0.1.0.tar.gz` & `tmp/markrunner_server-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "markrunner_server-0.1.0.tar", max compression
+gzip compressed data, was "markrunner_server-0.1.1.tar", max compression
```

## Comparing `markrunner_server-0.1.0.tar` & `markrunner_server-0.1.1.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0       20 2024-05-18 08:40:20.585620 markrunner_server-0.1.0/README.md
--rw-r--r--   0        0        0     2135 2024-05-18 08:39:31.956874 markrunner_server-0.1.0/main.py
--rw-r--r--   0        0        0      458 2024-05-18 08:44:15.634536 markrunner_server-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      453 1970-01-01 00:00:00.000000 markrunner_server-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0       20 2024-05-18 08:40:20.585620 markrunner_server-0.1.1/README.md
+-rw-r--r--   0        0        0     2160 2024-05-18 09:04:50.843275 markrunner_server-0.1.1/main.py
+-rw-r--r--   0        0        0      463 2024-05-18 09:05:04.100668 markrunner_server-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      453 1970-01-01 00:00:00.000000 markrunner_server-0.1.1/PKG-INFO
```

### Comparing `markrunner_server-0.1.0/main.py` & `markrunner_server-0.1.1/main.py`

 * *Files 6% similar despite different names*

```diff
@@ -53,12 +53,16 @@
     }
 
     def initialize_handlers(self):
         self.handlers.append(("/info", InfoHandler))
         self.handlers.append(("/stop", StopHandler))
 
 
-if __name__ == "__main__":
+def main():
     if os.environ.get("MARKRUNNER_SERVER_VERSION") != __version__:
         raise ValueError("Version mismatch")
 
     MarkrunnerApp.launch_instance()
+
+
+if __name__ == "__main__":
+    main()
```

