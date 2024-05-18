# Comparing `tmp/promplate_recipes-0.2.2.1.tar.gz` & `tmp/promplate_recipes-0.2.2.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "promplate_recipes-0.2.2.1.tar", last modified: Sat May 18 10:55:29 2024, max compression
+gzip compressed data, was "promplate_recipes-0.2.2.post1.tar", last modified: Sat May 18 02:58:03 2024, max compression
```

## Comparing `promplate_recipes-0.2.2.1.tar` & `promplate_recipes-0.2.2.post1.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0      405 2024-05-18 02:37:49.089513 promplate_recipes-0.2.2.1/README.md
--rw-r--r--   0        0        0      200 2024-04-10 06:40:35.413855 promplate_recipes-0.2.2.1/promplate_recipes/__init__.py
--rw-r--r--   0        0        0     2191 2024-05-16 12:21:26.190215 promplate_recipes-0.2.2.1/promplate_recipes/context.py
--rw-r--r--   0        0        0      388 2024-05-18 02:56:21.209051 promplate_recipes-0.2.2.1/promplate_recipes/functional/_common.py
--rw-r--r--   0        0        0      927 2024-05-18 02:56:55.070071 promplate_recipes-0.2.2.1/promplate_recipes/functional/component.py
--rw-r--r--   0        0        0     2689 2024-05-18 10:52:38.896492 promplate_recipes-0.2.2.1/promplate_recipes/functional/node.py
--rw-r--r--   0        0        0       50 2024-05-18 10:53:13.375568 promplate_recipes-0.2.2.1/promplate_recipes/version.py
--rw-r--r--   0        0        0      714 2024-05-18 10:55:29.493576 promplate_recipes-0.2.2.1/pyproject.toml
--rw-r--r--   0        0        0      647 1970-01-01 00:00:00.000000 promplate_recipes-0.2.2.1/PKG-INFO
+-rw-r--r--   0        0        0      405 2024-05-18 02:37:49.089513 promplate_recipes-0.2.2.post1/README.md
+-rw-r--r--   0        0        0      200 2024-04-10 06:40:35.413855 promplate_recipes-0.2.2.post1/promplate_recipes/__init__.py
+-rw-r--r--   0        0        0     2191 2024-05-16 12:21:26.190215 promplate_recipes-0.2.2.post1/promplate_recipes/context.py
+-rw-r--r--   0        0        0      388 2024-05-18 02:56:21.209051 promplate_recipes-0.2.2.post1/promplate_recipes/functional/_common.py
+-rw-r--r--   0        0        0      927 2024-05-18 02:56:55.070071 promplate_recipes-0.2.2.post1/promplate_recipes/functional/component.py
+-rw-r--r--   0        0        0     2694 2024-05-18 02:54:44.379680 promplate_recipes-0.2.2.post1/promplate_recipes/functional/node.py
+-rw-r--r--   0        0        0       54 2024-05-18 02:57:56.486031 promplate_recipes-0.2.2.post1/promplate_recipes/version.py
+-rw-r--r--   0        0        0      718 2024-05-18 02:58:03.238697 promplate_recipes-0.2.2.post1/pyproject.toml
+-rw-r--r--   0        0        0      651 1970-01-01 00:00:00.000000 promplate_recipes-0.2.2.post1/PKG-INFO
```

### Comparing `promplate_recipes-0.2.2.1/promplate_recipes/context.py` & `promplate_recipes-0.2.2.post1/promplate_recipes/context.py`

 * *Files identical despite different names*

### Comparing `promplate_recipes-0.2.2.1/promplate_recipes/functional/component.py` & `promplate_recipes-0.2.2.post1/promplate_recipes/functional/component.py`

 * *Files identical despite different names*

### Comparing `promplate_recipes-0.2.2.1/promplate_recipes/functional/node.py` & `promplate_recipes-0.2.2.post1/promplate_recipes/functional/node.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-from inspect import isgenerator
 from typing import TYPE_CHECKING, Any, Callable, Optional, TypeVar
 
 from promplate.chain.node import Context, Interruptable, resolve
 
 from ._common import CallableWrapper
 
 Function = TypeVar("Function", bound=Callable[[Context], Any])
@@ -24,15 +23,15 @@
             ...
 
     def _stream(self, context, /, generate, callbacks, **config):
         self._apply_pre_processes(context, callbacks)
 
         ret = self.__call__(context)
 
-        if isgenerator(ret):
+        if "__iter__" in dir(ret):
             for i in ret:
                 context.result = i
                 self._apply_mid_processes(context, callbacks)
                 yield
         else:
             context.result = ret
             self._apply_mid_processes(context, callbacks)
@@ -41,20 +40,20 @@
         self._apply_end_processes(context, callbacks)
 
     async def _astream(self, context, /, generate, callbacks, **config):
         await self._apply_async_pre_processes(context, callbacks)
 
         ret = await resolve(resolve(self.__call__(context)))
 
-        if "__aiter__" in dir(ret):
+        if "__aiter__" in dir(ret) or "__iter__" in dir(ret):
             async for i in ret:
                 context.result = i
                 await self._apply_async_mid_processes(context, callbacks)
                 yield
-        elif isgenerator(ret):
+        elif "__iter__" in dir(ret):
             for i in ret:
                 context.result = i
                 await self._apply_async_mid_processes(context, callbacks)
                 yield
         else:
             context.result = ret
             await self._apply_async_mid_processes(context, callbacks)
```

### Comparing `promplate_recipes-0.2.2.1/pyproject.toml` & `promplate_recipes-0.2.2.post1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 ]
 dependencies = [
     "promplate~=0.3.4",
     "python-box~=7.1.1",
 ]
 requires-python = ">=3.10"
 readme = "README.md"
-version = "0.2.2.1"
+version = "0.2.2.post1"
 
 [project.license]
 text = "MIT"
 
 [tool.pdm]
 distribution = true
```

### Comparing `promplate_recipes-0.2.2.1/PKG-INFO` & `promplate_recipes-0.2.2.post1/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: promplate-recipes
-Version: 0.2.2.1
+Version: 0.2.2.post1
 Author-Email: Muspi Merol <me@promplate.dev>
 License: MIT
 Requires-Python: >=3.10
 Requires-Dist: promplate~=0.3.4
 Requires-Dist: python-box~=7.1.1
 Description-Content-Type: text/markdown
```

