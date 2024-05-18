# Comparing `tmp/pyircsdk-1.5.1.tar.gz` & `tmp/pyircsdk-1.5.2.tar.gz`

## Comparing `pyircsdk-1.5.1.tar` & `pyircsdk-1.5.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 pyircsdk-1.5.1/pyircsdk/__about__.py
--rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 pyircsdk-1.5.1/pyircsdk/__init__.py
--rw-r--r--   0        0        0     1103 2020-02-02 00:00:00.000000 pyircsdk-1.5.1/pyircsdk/command.py
--rw-r--r--   0        0        0      591 2020-02-02 00:00:00.000000 pyircsdk-1.5.1/pyircsdk/message.py
--rw-r--r--   0        0        0     9116 2020-02-02 00:00:00.000000 pyircsdk-1.5.1/pyircsdk/pyircsdk.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyircsdk-1.5.1/pyircsdk/event/__init__.py
--rw-r--r--   0        0        0      843 2020-02-02 00:00:00.000000 pyircsdk-1.5.1/pyircsdk/event/event.py
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 pyircsdk-1.5.1/.gitignore
--rw-r--r--   0        0        0     1062 2020-02-02 00:00:00.000000 pyircsdk-1.5.1/LICENSE
--rw-r--r--   0        0        0      672 2020-02-02 00:00:00.000000 pyircsdk-1.5.1/README.md
--rw-r--r--   0        0        0      825 2020-02-02 00:00:00.000000 pyircsdk-1.5.1/pyproject.toml
--rw-r--r--   0        0        0     1319 2020-02-02 00:00:00.000000 pyircsdk-1.5.1/PKG-INFO
+-rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 pyircsdk-1.5.2/pyircsdk/__about__.py
+-rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 pyircsdk-1.5.2/pyircsdk/__init__.py
+-rw-r--r--   0        0        0     1103 2020-02-02 00:00:00.000000 pyircsdk-1.5.2/pyircsdk/command.py
+-rw-r--r--   0        0        0      591 2020-02-02 00:00:00.000000 pyircsdk-1.5.2/pyircsdk/message.py
+-rw-r--r--   0        0        0     9138 2020-02-02 00:00:00.000000 pyircsdk-1.5.2/pyircsdk/pyircsdk.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyircsdk-1.5.2/pyircsdk/event/__init__.py
+-rw-r--r--   0        0        0      843 2020-02-02 00:00:00.000000 pyircsdk-1.5.2/pyircsdk/event/event.py
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 pyircsdk-1.5.2/.gitignore
+-rw-r--r--   0        0        0     1062 2020-02-02 00:00:00.000000 pyircsdk-1.5.2/LICENSE
+-rw-r--r--   0        0        0      672 2020-02-02 00:00:00.000000 pyircsdk-1.5.2/README.md
+-rw-r--r--   0        0        0      825 2020-02-02 00:00:00.000000 pyircsdk-1.5.2/pyproject.toml
+-rw-r--r--   0        0        0     1319 2020-02-02 00:00:00.000000 pyircsdk-1.5.2/PKG-INFO
```

### Comparing `pyircsdk-1.5.1/pyircsdk/command.py` & `pyircsdk-1.5.2/pyircsdk/command.py`

 * *Files identical despite different names*

### Comparing `pyircsdk-1.5.1/pyircsdk/message.py` & `pyircsdk-1.5.2/pyircsdk/message.py`

 * *Files identical despite different names*

### Comparing `pyircsdk-1.5.1/pyircsdk/pyircsdk.py` & `pyircsdk-1.5.2/pyircsdk/pyircsdk.py`

 * *Files 4% similar despite different names*

```diff
@@ -128,21 +128,26 @@
                         print("Connection closed by the remote host.")
                         break
                     self.event.emit('raw', data)
 
                 except OSError as e:
                     print(e)
                     # exit program
-                    self.irc.close()
-                    exit(1)
+                    break;
             else:
-                print("No data received for %s seconds, quiting..." % str(self.config.nodataTimeout or 120))
-                # force program to close socket and to exit
-                self.irc.close()
-                exit(1)
+                if self.config.nodataTimeout > 0:
+                    print("No data received for %s seconds, quiting..." % str(self.config.nodataTimeout or 120))
+                    break
+
+        # force program to close socket and to exit
+        self.irc.close()
+        exit(1)
+
+
+
 
 
     def log(self, data: bytes) -> None:
         # convert bytes to string
         data = data.decode('utf-8')
         # print(data)
```

### Comparing `pyircsdk-1.5.1/pyircsdk/event/event.py` & `pyircsdk-1.5.2/pyircsdk/event/event.py`

 * *Files identical despite different names*

### Comparing `pyircsdk-1.5.1/.gitignore` & `pyircsdk-1.5.2/.gitignore`

 * *Files identical despite different names*

### Comparing `pyircsdk-1.5.1/LICENSE` & `pyircsdk-1.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pyircsdk-1.5.1/README.md` & `pyircsdk-1.5.2/README.md`

 * *Files identical despite different names*

### Comparing `pyircsdk-1.5.1/pyproject.toml` & `pyircsdk-1.5.2/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "hatchling.build"
 
 [project]
 name = "pyircsdk"
 authors = [
   { name="Bludot", email="admin@floretos.com" },
 ]
-version = "1.5.1"
+version = "1.5.2"
 description = "pyIRCSDK is a Python library for creating IRC bots and clients. It is designed to provide granular access to raw mesages and to provide an event emitter like interface for handling messages."
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
```

### Comparing `pyircsdk-1.5.1/PKG-INFO` & `pyircsdk-1.5.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: pyircsdk
-Version: 1.5.1
+Version: 1.5.2
 Summary: pyIRCSDK is a Python library for creating IRC bots and clients. It is designed to provide granular access to raw mesages and to provide an event emitter like interface for handling messages.
 Project-URL: Homepage, https://github.com/bludot/pyircsdk
 Project-URL: Issues, https://github.com/bludot/pyircsdk/issues
 Author-email: Bludot <admin@floretos.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

