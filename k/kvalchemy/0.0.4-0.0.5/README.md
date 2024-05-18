# Comparing `tmp/kvalchemy-0.0.4.tar.gz` & `tmp/kvalchemy-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kvalchemy-0.0.4.tar", last modified: Fri May 17 22:49:19 2024, max compression
+gzip compressed data, was "kvalchemy-0.0.5.tar", last modified: Sat May 18 02:16:13 2024, max compression
```

## Comparing `kvalchemy-0.0.4.tar` & `kvalchemy-0.0.5.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 22:49:19.974606 kvalchemy-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-05-17 22:49:11.000000 kvalchemy-0.0.4/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)     1733 2024-05-17 22:49:19.974606 kvalchemy-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1000 2024-05-17 22:49:11.000000 kvalchemy-0.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 22:49:19.970606 kvalchemy-0.0.4/kvalchemy/
--rw-r--r--   0 runner    (1001) docker     (127)      113 2024-05-17 22:49:11.000000 kvalchemy-0.0.4/kvalchemy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9133 2024-05-17 22:49:11.000000 kvalchemy-0.0.4/kvalchemy/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     1243 2024-05-17 22:49:11.000000 kvalchemy-0.0.4/kvalchemy/models.py
--rw-r--r--   0 runner    (1001) docker     (127)     2067 2024-05-17 22:49:11.000000 kvalchemy-0.0.4/kvalchemy/proxy.py
--rw-r--r--   0 runner    (1001) docker     (127)     1379 2024-05-17 22:49:11.000000 kvalchemy-0.0.4/kvalchemy/time.py
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-17 22:49:11.000000 kvalchemy-0.0.4/kvalchemy/values.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 22:49:19.974606 kvalchemy-0.0.4/kvalchemy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1733 2024-05-17 22:49:19.000000 kvalchemy-0.0.4/kvalchemy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      378 2024-05-17 22:49:19.000000 kvalchemy-0.0.4/kvalchemy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-17 22:49:19.000000 kvalchemy-0.0.4/kvalchemy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-17 22:49:19.000000 kvalchemy-0.0.4/kvalchemy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-17 22:49:19.000000 kvalchemy-0.0.4/kvalchemy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1032 2024-05-17 22:49:11.000000 kvalchemy-0.0.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-17 22:49:19.974606 kvalchemy-0.0.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 22:49:19.974606 kvalchemy-0.0.4/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     8236 2024-05-17 22:49:11.000000 kvalchemy-0.0.4/tests/test_client.py
--rw-r--r--   0 runner    (1001) docker     (127)      994 2024-05-17 22:49:11.000000 kvalchemy-0.0.4/tests/test_proxy.py
--rw-r--r--   0 runner    (1001) docker     (127)      779 2024-05-17 22:49:11.000000 kvalchemy-0.0.4/tests/test_time.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 02:16:13.752020 kvalchemy-0.0.5/
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-05-18 02:16:05.000000 kvalchemy-0.0.5/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1733 2024-05-18 02:16:13.752020 kvalchemy-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1000 2024-05-18 02:16:05.000000 kvalchemy-0.0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 02:16:13.748020 kvalchemy-0.0.5/kvalchemy/
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-05-18 02:16:05.000000 kvalchemy-0.0.5/kvalchemy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9175 2024-05-18 02:16:05.000000 kvalchemy-0.0.5/kvalchemy/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1331 2024-05-18 02:16:05.000000 kvalchemy-0.0.5/kvalchemy/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2067 2024-05-18 02:16:05.000000 kvalchemy-0.0.5/kvalchemy/proxy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1379 2024-05-18 02:16:05.000000 kvalchemy-0.0.5/kvalchemy/time.py
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-18 02:16:05.000000 kvalchemy-0.0.5/kvalchemy/values.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 02:16:13.752020 kvalchemy-0.0.5/kvalchemy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1733 2024-05-18 02:16:13.000000 kvalchemy-0.0.5/kvalchemy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      378 2024-05-18 02:16:13.000000 kvalchemy-0.0.5/kvalchemy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-18 02:16:13.000000 kvalchemy-0.0.5/kvalchemy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-18 02:16:13.000000 kvalchemy-0.0.5/kvalchemy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-18 02:16:13.000000 kvalchemy-0.0.5/kvalchemy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1032 2024-05-18 02:16:05.000000 kvalchemy-0.0.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-18 02:16:13.752020 kvalchemy-0.0.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 02:16:13.752020 kvalchemy-0.0.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     8236 2024-05-18 02:16:05.000000 kvalchemy-0.0.5/tests/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      994 2024-05-18 02:16:05.000000 kvalchemy-0.0.5/tests/test_proxy.py
+-rw-r--r--   0 runner    (1001) docker     (127)      779 2024-05-18 02:16:05.000000 kvalchemy-0.0.5/tests/test_time.py
```

### Comparing `kvalchemy-0.0.4/LICENSE.md` & `kvalchemy-0.0.5/LICENSE.md`

 * *Files identical despite different names*

### Comparing `kvalchemy-0.0.4/PKG-INFO` & `kvalchemy-0.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kvalchemy
-Version: 0.0.4
+Version: 0.0.5
 Summary: A SQLAlchemy based Key-Value store.
 Author-email: csm10495 <csm10495@gmail.com>
 License: MIT License
 Project-URL: homepage, https://github.com/csm10495/kvalchemy
 Project-URL: repository, https://github.com/csm10495/kvalchemy
 Project-URL: documentation, https://csm10495.github.io/kvalchemy
 Classifier: Intended Audience :: Developers
```

### Comparing `kvalchemy-0.0.4/README.md` & `kvalchemy-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `kvalchemy-0.0.4/kvalchemy/client.py` & `kvalchemy-0.0.5/kvalchemy/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import contextlib
 import logging
 from typing import Any, Callable, Iterable, Union
 
 from sqlalchemy import create_engine
 from sqlalchemy.orm import Session, scoped_session, sessionmaker
 
-from kvalchemy.models import Base, KVStore, ValueMixIn
+from kvalchemy.models import KEY_MAX_LENGTH, TAG_MAX_LENGTH, Base, KVStore, ValueMixIn
 from kvalchemy.proxy import Proxy
 from kvalchemy.time import ExpirationType, to_expire
 from kvalchemy.values import ENOVAL
 
 log = logging.getLogger(__name__)
 
 MEMOIZE_TAG = "__memoize__"
@@ -175,22 +175,20 @@
 
     def get_proxy(self, key: str, default: Any = ENOVAL, tag: str = "") -> Proxy:
         """
         Returns a Proxy object for the given key, tag, default.
         """
         return Proxy(self, key, default, tag)
 
-    def _delete_startswith(self, key: str, tag: str):
+    def delete_tag(self, tag: str) -> None:
         """
-        Deletes all keys that start with the given key but fall under the given tag.
+        Deletes all keys under a given tag.
         """
         with self.session() as session:
-            session.query(KVStore).filter(
-                KVStore.key.startswith(key), KVStore.tag == tag
-            ).delete()
+            session.query(KVStore).filter(KVStore.tag == tag).delete()
 
     def memoize(
         self,
         expire: ExpirationType = None,
         expire_if: Union[bool, Callable] = False,
         skip_saving_to_cache_if: Union[bool, Callable] = False,
     ):
@@ -214,33 +212,37 @@
             # without () at the end
             func = expire
             expire = None
         else:
             func = None
 
         def inner(func):
-            base_key = f"memoize.{func.__module__}_{func.__qualname__}_{expire!s}"
+            # Warning: we're truncating to fit the tag
+            tag = f"memoize.{func.__module__}_{func.__qualname__}_{expire!s}"[
+                :TAG_MAX_LENGTH
+            ]
 
             def wrapper(*args, **kwargs):
-                key = f"{base_key}_{args!s}_{kwargs!s}"
+                # Warning: we're truncating to fit the key
+                key = f"{args!s}_{kwargs!s}"[:KEY_MAX_LENGTH]
 
                 # if you overwrite inner.expire_if then the callable would only get evaluated once
                 # ... so don't do that.
                 expire_if = inner.expire_if
 
                 if callable(expire_if):
                     expire_if = expire_if()
 
                 try_cache = not bool(expire_if)
 
                 NO_RESULT = object()
                 result = NO_RESULT
                 if try_cache:
                     try:
-                        result = self.get(key, tag=MEMOIZE_TAG)
+                        result = self.get(key, tag=tag)
                     except KeyError:
                         pass
                 else:
                     log.debug(f"expire_if is forcing us to ignore cache: {key}")
 
                 if result == NO_RESULT:
                     result = func(*args, **kwargs)
@@ -253,19 +255,19 @@
                         skip_saving_to_cache = skip_saving_to_cache_if
 
                     if skip_saving_to_cache:
                         log.debug(
                             f"skip_saving_to_cache_if is forcing us to not save to cache the value for key: {key}"
                         )
                     else:
-                        self.set(key, result, tag=MEMOIZE_TAG, expire=expire)
+                        self.set(key, result, tag=tag, expire=expire)
 
                 return result
 
-            wrapper.cache_clear = lambda: self._delete_startswith(base_key, MEMOIZE_TAG)
+            wrapper.cache_clear = lambda: self.delete_tag(tag)
             return wrapper
 
         inner.expire_if = expire_if
 
         if func:
             return inner(func)
         else:
```

### Comparing `kvalchemy-0.0.4/kvalchemy/models.py` & `kvalchemy-0.0.5/kvalchemy/models.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,18 +1,21 @@
 """
 Home to models for KVAlchemy.
 """
 from datetime import datetime
 
 from sqlalchemy import Column, ColumnElement, UniqueConstraint, or_
 from sqlalchemy.orm import DeclarativeBase, Mapped, mapped_column
-from sqlalchemy.types import PickleType
+from sqlalchemy.types import PickleType, Unicode
 
 from kvalchemy.time import db_now
 
+KEY_MAX_LENGTH = 256
+TAG_MAX_LENGTH = 256
+
 
 class Base(DeclarativeBase):
     """
     The base class for all models.
     """
 
     pass
@@ -34,16 +37,16 @@
     The table for storing key-value pairs.
     """
 
     __tablename__ = "kvstore"
 
     __table_args__ = (UniqueConstraint("key", "tag", name="key_tag_unique"),)
 
-    key: Mapped[str] = mapped_column(primary_key=True)
-    tag: Mapped[str] = mapped_column(primary_key=True)
+    key: Mapped[str] = Column(Unicode(KEY_MAX_LENGTH), primary_key=True)
+    tag: Mapped[str] = Column(Unicode(TAG_MAX_LENGTH), primary_key=True)
 
     # Naive datetime (though expected to be UTC)
     expire: Mapped[datetime] = mapped_column(nullable=True)
 
     @classmethod
     def non_expired_filter(cls) -> ColumnElement[bool]:
         """
```

### Comparing `kvalchemy-0.0.4/kvalchemy/proxy.py` & `kvalchemy-0.0.5/kvalchemy/proxy.py`

 * *Files identical despite different names*

### Comparing `kvalchemy-0.0.4/kvalchemy/time.py` & `kvalchemy-0.0.5/kvalchemy/time.py`

 * *Files identical despite different names*

### Comparing `kvalchemy-0.0.4/kvalchemy.egg-info/PKG-INFO` & `kvalchemy-0.0.5/kvalchemy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kvalchemy
-Version: 0.0.4
+Version: 0.0.5
 Summary: A SQLAlchemy based Key-Value store.
 Author-email: csm10495 <csm10495@gmail.com>
 License: MIT License
 Project-URL: homepage, https://github.com/csm10495/kvalchemy
 Project-URL: repository, https://github.com/csm10495/kvalchemy
 Project-URL: documentation, https://csm10495.github.io/kvalchemy
 Classifier: Intended Audience :: Developers
```

### Comparing `kvalchemy-0.0.4/pyproject.toml` & `kvalchemy-0.0.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `kvalchemy-0.0.4/tests/test_client.py` & `kvalchemy-0.0.5/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `kvalchemy-0.0.4/tests/test_proxy.py` & `kvalchemy-0.0.5/tests/test_proxy.py`

 * *Files identical despite different names*

### Comparing `kvalchemy-0.0.4/tests/test_time.py` & `kvalchemy-0.0.5/tests/test_time.py`

 * *Files identical despite different names*

