# Comparing `tmp/unconscious-0.0.1.tar.gz` & `tmp/unconscious-0.0.2.tar.gz`

## Comparing `unconscious-0.0.1.tar` & `unconscious-0.0.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0      501       20      548 2024-05-17 03:03:43.000000 unconscious-0.0.1/unconscious-core/Cargo.toml
--rw-r--r--   0      501       20    11564 2024-05-18 18:23:21.000000 unconscious-0.0.1/unconscious-core/src/lib.rs
--rw-r--r--   0      501       20       94 2024-05-17 01:58:19.000000 unconscious-0.0.1/unconscious-core/src/main.rs
--rw-r--r--   0        0        0      429 1970-01-01 00:00:00.000000 unconscious-0.0.1/unconscious/Cargo.toml
--rw-r--r--   0      501       20      807 2024-05-17 01:47:05.000000 unconscious-0.0.1/unconscious/.cargo/config.toml
--rw-r--r--   0      501       20      280 2024-05-15 04:49:11.000000 unconscious-0.0.1/unconscious/.env/pyvenv.cfg
--rw-r--r--   0      501       20     3526 2024-05-15 04:49:28.000000 unconscious-0.0.1/unconscious/.github/workflows/CI.yml
--rw-r--r--   0      501       20      686 2024-05-15 04:49:28.000000 unconscious-0.0.1/unconscious/.gitignore
--rw-r--r--   0      501       20       56 2024-05-16 22:13:01.000000 unconscious-0.0.1/unconscious/Makefile
--rwxr-xr-x   0      501       20      114 2024-05-17 01:32:29.000000 unconscious-0.0.1/unconscious/custom-cargo-wrapper
--rw-r--r--   0      501       20      699 2024-05-16 23:54:53.000000 unconscious-0.0.1/unconscious/demo.py
--rw-r--r--   0      501       20      430 2024-05-17 01:58:07.000000 unconscious-0.0.1/unconscious/src/lib.rs
--rw-r--r--   0      501       20     1795 2024-05-17 00:29:41.000000 unconscious-0.0.1/unconscious/unconscious/__init__.py
--rw-r--r--   0      501       20     2639 2024-05-17 00:02:16.000000 unconscious-0.0.1/unconscious/unconscious/agent.py
--rw-r--r--   0      501       20     3863 2024-05-17 00:02:21.000000 unconscious-0.0.1/unconscious/unconscious/client.py
--rw-r--r--   0      501       20    37586 2024-05-16 13:57:44.000000 unconscious-0.0.1/unconscious/Cargo.lock
--rw-r--r--   0        0        0      432 1970-01-01 00:00:00.000000 unconscious-0.0.1/pyproject.toml
--rw-r--r--   0      501       20     3863 2024-05-17 00:02:21.000000 unconscious-0.0.1/unconscious/client.py
--rw-r--r--   0      501       20     1795 2024-05-17 00:29:41.000000 unconscious-0.0.1/unconscious/__init__.py
--rw-r--r--   0      501       20     2639 2024-05-17 00:02:16.000000 unconscious-0.0.1/unconscious/agent.py
--rw-r--r--   0        0        0      260 1970-01-01 00:00:00.000000 unconscious-0.0.1/PKG-INFO
+-rw-r--r--   0      501       20      548 2024-05-17 03:03:43.000000 unconscious-0.0.2/unconscious-core/Cargo.toml
+-rw-r--r--   0      501       20    11564 2024-05-18 18:23:21.000000 unconscious-0.0.2/unconscious-core/src/lib.rs
+-rw-r--r--   0      501       20       94 2024-05-17 01:58:19.000000 unconscious-0.0.2/unconscious-core/src/main.rs
+-rw-r--r--   0        0        0      429 1970-01-01 00:00:00.000000 unconscious-0.0.2/unconscious/Cargo.toml
+-rw-r--r--   0      501       20      807 2024-05-17 01:47:05.000000 unconscious-0.0.2/unconscious/.cargo/config.toml
+-rw-r--r--   0      501       20      280 2024-05-15 04:49:11.000000 unconscious-0.0.2/unconscious/.env/pyvenv.cfg
+-rw-r--r--   0      501       20     3526 2024-05-15 04:49:28.000000 unconscious-0.0.2/unconscious/.github/workflows/CI.yml
+-rw-r--r--   0      501       20      686 2024-05-15 04:49:28.000000 unconscious-0.0.2/unconscious/.gitignore
+-rw-r--r--   0      501       20       56 2024-05-16 22:13:01.000000 unconscious-0.0.2/unconscious/Makefile
+-rwxr-xr-x   0      501       20      114 2024-05-17 01:32:29.000000 unconscious-0.0.2/unconscious/custom-cargo-wrapper
+-rw-r--r--   0      501       20      699 2024-05-16 23:54:53.000000 unconscious-0.0.2/unconscious/demo.py
+-rw-r--r--   0      501       20      427 2024-05-18 18:51:37.000000 unconscious-0.0.2/unconscious/src/lib.rs
+-rw-r--r--   0      501       20     1780 2024-05-18 18:51:20.000000 unconscious-0.0.2/unconscious/unconscious/__init__.py
+-rw-r--r--   0      501       20     2639 2024-05-17 00:02:16.000000 unconscious-0.0.2/unconscious/unconscious/agent.py
+-rw-r--r--   0      501       20     3863 2024-05-17 00:02:21.000000 unconscious-0.0.2/unconscious/unconscious/client.py
+-rw-r--r--   0      501       20    37586 2024-05-16 13:57:44.000000 unconscious-0.0.2/unconscious/Cargo.lock
+-rw-r--r--   0        0        0      432 1970-01-01 00:00:00.000000 unconscious-0.0.2/pyproject.toml
+-rw-r--r--   0      501       20     3863 2024-05-17 00:02:21.000000 unconscious-0.0.2/unconscious/client.py
+-rw-r--r--   0      501       20     1780 2024-05-18 18:51:20.000000 unconscious-0.0.2/unconscious/__init__.py
+-rw-r--r--   0      501       20     2639 2024-05-17 00:02:16.000000 unconscious-0.0.2/unconscious/agent.py
+-rw-r--r--   0        0        0      260 1970-01-01 00:00:00.000000 unconscious-0.0.2/PKG-INFO
```

### Comparing `unconscious-0.0.1/unconscious-core/Cargo.toml` & `unconscious-0.0.2/unconscious-core/Cargo.toml`

 * *Files identical despite different names*

### Comparing `unconscious-0.0.1/unconscious-core/src/lib.rs` & `unconscious-0.0.2/unconscious-core/src/lib.rs`

 * *Files identical despite different names*

### Comparing `unconscious-0.0.1/unconscious/.cargo/config.toml` & `unconscious-0.0.2/unconscious/.cargo/config.toml`

 * *Files identical despite different names*

### Comparing `unconscious-0.0.1/unconscious/.github/workflows/CI.yml` & `unconscious-0.0.2/unconscious/.github/workflows/CI.yml`

 * *Files identical despite different names*

### Comparing `unconscious-0.0.1/unconscious/.gitignore` & `unconscious-0.0.2/unconscious/.gitignore`

 * *Files identical despite different names*

### Comparing `unconscious-0.0.1/unconscious/demo.py` & `unconscious-0.0.2/unconscious/demo.py`

 * *Files identical despite different names*

### Comparing `unconscious-0.0.1/unconscious/unconscious/__init__.py` & `unconscious-0.0.2/unconscious/unconscious/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,29 +1,29 @@
-from .py_unconscious import *
+from .unconscious import *
 import asyncio
 import threading
 import asyncio
 
-__doc__ = py_unconscious.__doc__
-if hasattr(py_unconscious, "__all__"):
-    __all__ = py_unconscious.__all__
+__doc__ = unconscious.__doc__
+if hasattr(unconscious, "__all__"):
+    __all__ = unconscious.__all__
 
 
 class Client:
     def __init__(self):
         self.loop = asyncio.new_event_loop()
         self.thread = threading.Thread(target=self.run_server)
         self.thread.start()
 
     def run_server(self):
         asyncio.set_event_loop(self.loop)
         self.loop.run_until_complete(self.main())
 
     async def main(self):
-        await py_unconscious.rust_server()
+        await unconscious.rust_server()
 
     def stop(self):
         self.loop.call_soon_threadsafe(self.loop.stop)
         self.thread.join()
 
 
 def 役人(cls=None, default_name=None, thread=None):
```

### Comparing `unconscious-0.0.1/unconscious/unconscious/agent.py` & `unconscious-0.0.2/unconscious/unconscious/agent.py`

 * *Files identical despite different names*

### Comparing `unconscious-0.0.1/unconscious/unconscious/client.py` & `unconscious-0.0.2/unconscious/unconscious/client.py`

 * *Files identical despite different names*

### Comparing `unconscious-0.0.1/unconscious/Cargo.lock` & `unconscious-0.0.2/unconscious/Cargo.lock`

 * *Files identical despite different names*

### Comparing `unconscious-0.0.1/unconscious/client.py` & `unconscious-0.0.2/unconscious/client.py`

 * *Files identical despite different names*

### Comparing `unconscious-0.0.1/unconscious/__init__.py` & `unconscious-0.0.2/unconscious/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,29 +1,29 @@
-from .py_unconscious import *
+from .unconscious import *
 import asyncio
 import threading
 import asyncio
 
-__doc__ = py_unconscious.__doc__
-if hasattr(py_unconscious, "__all__"):
-    __all__ = py_unconscious.__all__
+__doc__ = unconscious.__doc__
+if hasattr(unconscious, "__all__"):
+    __all__ = unconscious.__all__
 
 
 class Client:
     def __init__(self):
         self.loop = asyncio.new_event_loop()
         self.thread = threading.Thread(target=self.run_server)
         self.thread.start()
 
     def run_server(self):
         asyncio.set_event_loop(self.loop)
         self.loop.run_until_complete(self.main())
 
     async def main(self):
-        await py_unconscious.rust_server()
+        await unconscious.rust_server()
 
     def stop(self):
         self.loop.call_soon_threadsafe(self.loop.stop)
         self.thread.join()
 
 
 def 役人(cls=None, default_name=None, thread=None):
```

### Comparing `unconscious-0.0.1/unconscious/agent.py` & `unconscious-0.0.2/unconscious/agent.py`

 * *Files identical despite different names*

