# Comparing `tmp/kvalchemy-0.0.5.tar.gz` & `tmp/kvalchemy-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kvalchemy-0.0.5.tar", last modified: Sat May 18 02:16:13 2024, max compression
+gzip compressed data, was "kvalchemy-0.0.6.tar", last modified: Sat May 18 02:20:03 2024, max compression
```

## Comparing `kvalchemy-0.0.5.tar` & `kvalchemy-0.0.6.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 02:16:13.752020 kvalchemy-0.0.5/
--rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-05-18 02:16:05.000000 kvalchemy-0.0.5/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)     1733 2024-05-18 02:16:13.752020 kvalchemy-0.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1000 2024-05-18 02:16:05.000000 kvalchemy-0.0.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 02:16:13.748020 kvalchemy-0.0.5/kvalchemy/
--rw-r--r--   0 runner    (1001) docker     (127)      113 2024-05-18 02:16:05.000000 kvalchemy-0.0.5/kvalchemy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9175 2024-05-18 02:16:05.000000 kvalchemy-0.0.5/kvalchemy/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     1331 2024-05-18 02:16:05.000000 kvalchemy-0.0.5/kvalchemy/models.py
--rw-r--r--   0 runner    (1001) docker     (127)     2067 2024-05-18 02:16:05.000000 kvalchemy-0.0.5/kvalchemy/proxy.py
--rw-r--r--   0 runner    (1001) docker     (127)     1379 2024-05-18 02:16:05.000000 kvalchemy-0.0.5/kvalchemy/time.py
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-18 02:16:05.000000 kvalchemy-0.0.5/kvalchemy/values.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 02:16:13.752020 kvalchemy-0.0.5/kvalchemy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1733 2024-05-18 02:16:13.000000 kvalchemy-0.0.5/kvalchemy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      378 2024-05-18 02:16:13.000000 kvalchemy-0.0.5/kvalchemy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-18 02:16:13.000000 kvalchemy-0.0.5/kvalchemy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-18 02:16:13.000000 kvalchemy-0.0.5/kvalchemy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-18 02:16:13.000000 kvalchemy-0.0.5/kvalchemy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1032 2024-05-18 02:16:05.000000 kvalchemy-0.0.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-18 02:16:13.752020 kvalchemy-0.0.5/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 02:16:13.752020 kvalchemy-0.0.5/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     8236 2024-05-18 02:16:05.000000 kvalchemy-0.0.5/tests/test_client.py
--rw-r--r--   0 runner    (1001) docker     (127)      994 2024-05-18 02:16:05.000000 kvalchemy-0.0.5/tests/test_proxy.py
--rw-r--r--   0 runner    (1001) docker     (127)      779 2024-05-18 02:16:05.000000 kvalchemy-0.0.5/tests/test_time.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 02:20:03.002776 kvalchemy-0.0.6/
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-05-18 02:19:53.000000 kvalchemy-0.0.6/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1733 2024-05-18 02:20:03.002776 kvalchemy-0.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1000 2024-05-18 02:19:53.000000 kvalchemy-0.0.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 02:20:03.002776 kvalchemy-0.0.6/kvalchemy/
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-05-18 02:19:53.000000 kvalchemy-0.0.6/kvalchemy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9226 2024-05-18 02:19:53.000000 kvalchemy-0.0.6/kvalchemy/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1331 2024-05-18 02:19:53.000000 kvalchemy-0.0.6/kvalchemy/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2067 2024-05-18 02:19:53.000000 kvalchemy-0.0.6/kvalchemy/proxy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1379 2024-05-18 02:19:53.000000 kvalchemy-0.0.6/kvalchemy/time.py
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-18 02:19:53.000000 kvalchemy-0.0.6/kvalchemy/values.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 02:20:03.002776 kvalchemy-0.0.6/kvalchemy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1733 2024-05-18 02:20:02.000000 kvalchemy-0.0.6/kvalchemy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      378 2024-05-18 02:20:02.000000 kvalchemy-0.0.6/kvalchemy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-18 02:20:02.000000 kvalchemy-0.0.6/kvalchemy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-18 02:20:02.000000 kvalchemy-0.0.6/kvalchemy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-18 02:20:02.000000 kvalchemy-0.0.6/kvalchemy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1032 2024-05-18 02:19:53.000000 kvalchemy-0.0.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-18 02:20:03.002776 kvalchemy-0.0.6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 02:20:03.002776 kvalchemy-0.0.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     8669 2024-05-18 02:19:53.000000 kvalchemy-0.0.6/tests/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      994 2024-05-18 02:19:53.000000 kvalchemy-0.0.6/tests/test_proxy.py
+-rw-r--r--   0 runner    (1001) docker     (127)      779 2024-05-18 02:19:53.000000 kvalchemy-0.0.6/tests/test_time.py
```

### Comparing `kvalchemy-0.0.5/LICENSE.md` & `kvalchemy-0.0.6/LICENSE.md`

 * *Files identical despite different names*

### Comparing `kvalchemy-0.0.5/PKG-INFO` & `kvalchemy-0.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kvalchemy
-Version: 0.0.5
+Version: 0.0.6
 Summary: A SQLAlchemy based Key-Value store.
 Author-email: csm10495 <csm10495@gmail.com>
 License: MIT License
 Project-URL: homepage, https://github.com/csm10495/kvalchemy
 Project-URL: repository, https://github.com/csm10495/kvalchemy
 Project-URL: documentation, https://csm10495.github.io/kvalchemy
 Classifier: Intended Audience :: Developers
```

### Comparing `kvalchemy-0.0.5/README.md` & `kvalchemy-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `kvalchemy-0.0.5/kvalchemy/client.py` & `kvalchemy-0.0.6/kvalchemy/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -175,20 +175,22 @@
 
     def get_proxy(self, key: str, default: Any = ENOVAL, tag: str = "") -> Proxy:
         """
         Returns a Proxy object for the given key, tag, default.
         """
         return Proxy(self, key, default, tag)
 
-    def delete_tag(self, tag: str) -> None:
+    def delete_tag(self, tag: str) -> int:
         """
         Deletes all keys under a given tag.
+
+        Returns the number of keys deleted.
         """
         with self.session() as session:
-            session.query(KVStore).filter(KVStore.tag == tag).delete()
+            return session.query(KVStore).filter(KVStore.tag == tag).delete()
 
     def memoize(
         self,
         expire: ExpirationType = None,
         expire_if: Union[bool, Callable] = False,
         skip_saving_to_cache_if: Union[bool, Callable] = False,
     ):
```

### Comparing `kvalchemy-0.0.5/kvalchemy/models.py` & `kvalchemy-0.0.6/kvalchemy/models.py`

 * *Files identical despite different names*

### Comparing `kvalchemy-0.0.5/kvalchemy/proxy.py` & `kvalchemy-0.0.6/kvalchemy/proxy.py`

 * *Files identical despite different names*

### Comparing `kvalchemy-0.0.5/kvalchemy/time.py` & `kvalchemy-0.0.6/kvalchemy/time.py`

 * *Files identical despite different names*

### Comparing `kvalchemy-0.0.5/kvalchemy.egg-info/PKG-INFO` & `kvalchemy-0.0.6/kvalchemy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kvalchemy
-Version: 0.0.5
+Version: 0.0.6
 Summary: A SQLAlchemy based Key-Value store.
 Author-email: csm10495 <csm10495@gmail.com>
 License: MIT License
 Project-URL: homepage, https://github.com/csm10495/kvalchemy
 Project-URL: repository, https://github.com/csm10495/kvalchemy
 Project-URL: documentation, https://csm10495.github.io/kvalchemy
 Classifier: Intended Audience :: Developers
```

### Comparing `kvalchemy-0.0.5/pyproject.toml` & `kvalchemy-0.0.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `kvalchemy-0.0.5/tests/test_client.py` & `kvalchemy-0.0.6/tests/test_client.py`

 * *Files 8% similar despite different names*

```diff
@@ -227,14 +227,28 @@
     proxy = kvalchemy.get_proxy("key", "default", "tag")
     assert proxy.kva is kvalchemy
     assert proxy.key == "key"
     assert proxy.default == "default"
     assert proxy.tag == "tag"
 
 
+def test_delete_tag(kvalchemy):
+    kvalchemy.set("key", "value", "tag")
+    kvalchemy.set("key2", "value2", "tag")
+    assert len(kvalchemy) == 2
+    kvalchemy.set("key", "value", "tag2")
+    assert len(kvalchemy) == 3
+
+    assert kvalchemy.delete_tag("tag") == 2
+    assert len(kvalchemy) == 1
+    assert kvalchemy.delete_tag("tag2") == 1
+    assert len(kvalchemy) == 0
+    assert kvalchemy.delete_tag("tag3") == 0
+
+
 def test_memoize_simple(kvalchemy):
     global ret_val
 
     # with parenthesis
     ret_val = True
 
     @kvalchemy.memoize()
```

### Comparing `kvalchemy-0.0.5/tests/test_proxy.py` & `kvalchemy-0.0.6/tests/test_proxy.py`

 * *Files identical despite different names*

### Comparing `kvalchemy-0.0.5/tests/test_time.py` & `kvalchemy-0.0.6/tests/test_time.py`

 * *Files identical despite different names*

