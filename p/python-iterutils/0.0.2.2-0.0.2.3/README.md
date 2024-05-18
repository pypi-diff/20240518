# Comparing `tmp/python_iterutils-0.0.2.2.tar.gz` & `tmp/python_iterutils-0.0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_iterutils-0.0.2.2.tar", max compression
+gzip compressed data, was "python_iterutils-0.0.2.3.tar", max compression
```

## Comparing `python_iterutils-0.0.2.2.tar` & `python_iterutils-0.0.2.3.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rwxr-xr-x   0        0        0     1100 2024-01-29 04:51:11.346824 python_iterutils-0.0.2.2/LICENSE
--rwxr-xr-x   0        0        0     3119 2024-05-17 10:07:08.653887 python_iterutils-0.0.2.2/iterutils/__init__.py
--rw-r--r--   0        0        0        0 2024-01-30 04:55:37.590943 python_iterutils-0.0.2.2/iterutils/py.typed
--rw-r--r--   0        0        0     1187 2024-05-17 10:08:11.963854 python_iterutils-0.0.2.2/pyproject.toml
--rw-r--r--   0        0        0      208 2024-05-15 13:48:16.668636 python_iterutils-0.0.2.2/readme.md
--rw-r--r--   0        0        0     1384 1970-01-01 00:00:00.000000 python_iterutils-0.0.2.2/PKG-INFO
+-rwxr-xr-x   0        0        0     1100 2024-01-29 04:51:11.346824 python_iterutils-0.0.2.3/LICENSE
+-rwxr-xr-x   0        0        0     3505 2024-05-18 18:01:04.033354 python_iterutils-0.0.2.3/iterutils/__init__.py
+-rw-r--r--   0        0        0        0 2024-01-30 04:55:37.590943 python_iterutils-0.0.2.3/iterutils/py.typed
+-rw-r--r--   0        0        0     1187 2024-05-18 18:13:11.493431 python_iterutils-0.0.2.3/pyproject.toml
+-rw-r--r--   0        0        0      208 2024-05-15 13:48:16.668636 python_iterutils-0.0.2.3/readme.md
+-rw-r--r--   0        0        0     1384 1970-01-01 00:00:00.000000 python_iterutils-0.0.2.3/PKG-INFO
```

### Comparing `python_iterutils-0.0.2.2/LICENSE` & `python_iterutils-0.0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `python_iterutils-0.0.2.2/iterutils/__init__.py` & `python_iterutils-0.0.2.3/iterutils/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -72,35 +72,47 @@
 ) -> Iterator[T]:
     if not callable(callprev):
         callprev = None
     if not callable(callnext):
         callnext = None
     for e in it:
         if callprev:
-            callprev(e)
+            try:
+                callprev(e)
+            except (StopIteration, GeneratorExit):
+                break
         yield e
         if callnext:
-            callnext(e)
+            try:
+                callnext(e)
+            except (StopIteration, GeneratorExit):
+                break
 
 
 async def wrap_aiter(
     it: Iterable[T] | AsyncIterable[T], 
     /, 
     callprev: None | Callable[[T], Any] = None, 
     callnext: None | Callable[[T], Any] = None,  
     threaded: bool = True, 
 ) -> AsyncIterator[T]:
     callprev = ensure_async(callprev) if callable(callprev) else None
     callnext = ensure_async(callnext) if callable(callnext) else None
     async for e in ensure_aiter(it, threaded=threaded):
         if callprev:
-            await callprev(e)
+            try:
+                await callprev(e)
+            except (StopAsyncIteration, GeneratorExit):
+                break
         yield e
         if callnext:
-            await callnext(e)
+            try:
+                await callnext(e)
+            except (StopAsyncIteration, GeneratorExit):
+                break
 
 
 def acc_step(
     start: int, 
     stop: None | int = None, 
     step: int = 1, 
 ) -> Iterator[tuple[int, int, int]]:
```

### Comparing `python_iterutils-0.0.2.2/pyproject.toml` & `python_iterutils-0.0.2.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "python-iterutils"
-version = "0.0.2.2"
+version = "0.0.2.3"
 description = "Python another itertools."
 authors = ["ChenyangGao <wosiwujm@gmail.com>"]
 license = "MIT"
 readme = "readme.md"
 homepage = "https://github.com/ChenyangGao/web-mount-packs/tree/main/python-module/python-iterutils"
 repository = "https://github.com/ChenyangGao/web-mount-packs/tree/main/python-module/python-iterutils"
 keywords = ["iterable", "iterutils"]
```

### Comparing `python_iterutils-0.0.2.2/PKG-INFO` & `python_iterutils-0.0.2.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-iterutils
-Version: 0.0.2.2
+Version: 0.0.2.3
 Summary: Python another itertools.
 Home-page: https://github.com/ChenyangGao/web-mount-packs/tree/main/python-module/python-iterutils
 License: MIT
 Keywords: iterable,iterutils
 Author: ChenyangGao
 Author-email: wosiwujm@gmail.com
 Requires-Python: >=3.10,<4.0
```

