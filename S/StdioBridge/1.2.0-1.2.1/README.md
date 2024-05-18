# Comparing `tmp/StdioBridge-1.2.0.tar.gz` & `tmp/StdioBridge-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "StdioBridge-1.2.0.tar", last modified: Sat May 18 12:16:30 2024, max compression
+gzip compressed data, was "StdioBridge-1.2.1.tar", last modified: Sat May 18 12:55:56 2024, max compression
```

## Comparing `StdioBridge-1.2.0.tar` & `StdioBridge-1.2.1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 12:16:30.764418 StdioBridge-1.2.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-05-18 12:16:16.000000 StdioBridge-1.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3536 2024-05-18 12:16:30.764418 StdioBridge-1.2.0/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 12:16:30.764418 StdioBridge-1.2.0/StdioBridge/
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-18 12:16:16.000000 StdioBridge-1.2.0/StdioBridge/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-18 12:16:16.000000 StdioBridge-1.2.0/StdioBridge/_config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 12:16:30.764418 StdioBridge-1.2.0/StdioBridge/api/
--rw-r--r--   0 runner    (1001) docker     (127)      179 2024-05-18 12:16:16.000000 StdioBridge-1.2.0/StdioBridge/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3676 2024-05-18 12:16:16.000000 StdioBridge-1.2.0/StdioBridge/api/_api.py
--rw-r--r--   0 runner    (1001) docker     (127)      822 2024-05-18 12:16:16.000000 StdioBridge-1.2.0/StdioBridge/api/_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     5647 2024-05-18 12:16:16.000000 StdioBridge-1.2.0/StdioBridge/api/_router.py
--rw-r--r--   0 runner    (1001) docker     (127)     1424 2024-05-18 12:16:16.000000 StdioBridge-1.2.0/StdioBridge/api/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 12:16:30.764418 StdioBridge-1.2.0/StdioBridge/client/
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-05-18 12:16:16.000000 StdioBridge-1.2.0/StdioBridge/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4344 2024-05-18 12:16:16.000000 StdioBridge-1.2.0/StdioBridge/client/_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     1334 2024-05-18 12:16:16.000000 StdioBridge-1.2.0/StdioBridge/client/_response.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 12:16:30.764418 StdioBridge-1.2.0/StdioBridge.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3536 2024-05-18 12:16:30.000000 StdioBridge-1.2.0/StdioBridge.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      464 2024-05-18 12:16:30.000000 StdioBridge-1.2.0/StdioBridge.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-18 12:16:30.000000 StdioBridge-1.2.0/StdioBridge.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-18 12:16:30.000000 StdioBridge-1.2.0/StdioBridge.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-18 12:16:30.000000 StdioBridge-1.2.0/StdioBridge.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-18 12:16:30.764418 StdioBridge-1.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1170 2024-05-18 12:16:16.000000 StdioBridge-1.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 12:55:56.359239 StdioBridge-1.2.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-05-18 12:55:48.000000 StdioBridge-1.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3536 2024-05-18 12:55:56.359239 StdioBridge-1.2.1/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 12:55:56.355239 StdioBridge-1.2.1/StdioBridge/
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-18 12:55:48.000000 StdioBridge-1.2.1/StdioBridge/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-18 12:55:48.000000 StdioBridge-1.2.1/StdioBridge/_config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 12:55:56.359239 StdioBridge-1.2.1/StdioBridge/api/
+-rw-r--r--   0 runner    (1001) docker     (127)      179 2024-05-18 12:55:48.000000 StdioBridge-1.2.1/StdioBridge/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3405 2024-05-18 12:55:48.000000 StdioBridge-1.2.1/StdioBridge/api/_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      822 2024-05-18 12:55:48.000000 StdioBridge-1.2.1/StdioBridge/api/_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7232 2024-05-18 12:55:48.000000 StdioBridge-1.2.1/StdioBridge/api/_router.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1424 2024-05-18 12:55:48.000000 StdioBridge-1.2.1/StdioBridge/api/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 12:55:56.359239 StdioBridge-1.2.1/StdioBridge/client/
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-05-18 12:55:48.000000 StdioBridge-1.2.1/StdioBridge/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4344 2024-05-18 12:55:48.000000 StdioBridge-1.2.1/StdioBridge/client/_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1334 2024-05-18 12:55:48.000000 StdioBridge-1.2.1/StdioBridge/client/_response.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 12:55:56.355239 StdioBridge-1.2.1/StdioBridge.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3536 2024-05-18 12:55:56.000000 StdioBridge-1.2.1/StdioBridge.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      464 2024-05-18 12:55:56.000000 StdioBridge-1.2.1/StdioBridge.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-18 12:55:56.000000 StdioBridge-1.2.1/StdioBridge.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-18 12:55:56.000000 StdioBridge-1.2.1/StdioBridge.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-18 12:55:56.000000 StdioBridge-1.2.1/StdioBridge.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-18 12:55:56.359239 StdioBridge-1.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1170 2024-05-18 12:55:48.000000 StdioBridge-1.2.1/setup.py
```

### Comparing `StdioBridge-1.2.0/LICENSE` & `StdioBridge-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `StdioBridge-1.2.0/PKG-INFO` & `StdioBridge-1.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: StdioBridge
-Version: 1.2.0
+Version: 1.2.1
 Summary: A StdioBridge package.
 Home-page: https://github.com/SergeiKrivko
 Author: SergeiKrivko
 License: MIT License
         
         Copyright (c) 2024 SergeiKrivko
```

### Comparing `StdioBridge-1.2.0/StdioBridge/api/_api.py` & `StdioBridge-1.2.1/StdioBridge/api/_api.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,27 +1,18 @@
 import asyncio
-import functools
 import json
 from urllib.parse import urlparse, parse_qs
 
 from aioconsole import ainput
 
 from StdioBridge.api._response import Response, StreamResponse
 from StdioBridge.api._router import Router
 from StdioBridge.api.errors import *
 
 
-def async_slot(func):
-    @functools.wraps(func)
-    def _run(*args, **kwargs):
-        loop = asyncio.get_event_loop()
-        loop.create_task(func(*args, **kwargs)).done()
-    return _run
-
-
 class Api:
     def __init__(self):
         self._root_router = Router()
 
     def get(self, url: str):
         return self._root_router.get(url)
 
@@ -36,15 +27,14 @@
 
     def patch(self, url: str):
         return self._root_router.patch(url)
 
     def add_router(self, url: str, router: Router):
         self._root_router.add_router(url, router)
 
-    @async_slot
     async def _process_request(self, request: dict):
         resp_id = request.get('id')
         try:
             try:
                 url = request['url']
                 method = request['method']
                 data = request['data']
@@ -89,14 +79,12 @@
     def run(self):
         asyncio.run(self._run())
 
     async def _run(self):
         while True:
             try:
                 inp = await ainput()
-                # inp = input()
                 data = json.loads(inp)
-                resp_id = data.get('id')
             except json.JSONDecodeError:
                 print("Invalid JSON")
             else:
-                self._process_request(data)
+                asyncio.create_task(self._process_request(data)).done()
```

### Comparing `StdioBridge-1.2.0/StdioBridge/api/_response.py` & `StdioBridge-1.2.1/StdioBridge/api/_response.py`

 * *Files identical despite different names*

### Comparing `StdioBridge-1.2.0/StdioBridge/api/_router.py` & `StdioBridge-1.2.1/StdioBridge/api/_router.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from inspect import isasyncgen, isgenerator, iscoroutine
-from types import FunctionType
-from typing import Callable, Any
+from types import FunctionType, GenericAlias
+from typing import Callable, Any, Type
 
 from StdioBridge.api._response import Response, StreamResponse
 from StdioBridge.api.errors import *
 
 
 class _Router:
     def __init__(self, name):
@@ -69,49 +69,95 @@
                     path_params.pop(self._routes[None].name)
                     method_not_found = True
         if method_not_found:
             raise ErrorMethodNotAllowed()
         raise ErrorNotFound()
 
 
+def _convert_param(param_type: Type, param):
+    try:
+        return param_type(param)
+    except Exception:
+        raise ErrorUnprocessableEntity(f"Cannot convert {param} to {param_type.__name__}")
+
+
+def _result_to_json(result):
+    if isinstance(result, dict):
+        return {key: _result_to_json(value) for key, value in result.items()}
+    if isinstance(result, list):
+        return [_result_to_json(el) for el in result]
+    if hasattr(result, 'dict'):
+        return result.dict()
+    return result
+
+
 class Router:
     def __init__(self):
         self._router = _Router('/')
 
+    @staticmethod
+    def _check_data_param(data, param_type):
+        if param_type == dict:
+            return dict(data)
+        if isinstance(param_type, GenericAlias) and param_type.__origin__ == dict:
+            return dict(data)
+        try:
+            import pydantic
+            if issubclass(param_type, pydantic.BaseModel):
+                return param_type(**data)
+        except Exception:
+            pass
+        return None
+
+    @staticmethod
+    def _check_query_param(param_list, param_type):
+        if param_type == list:
+            return list(param_list)
+        elif isinstance(param_type, GenericAlias) and param_type.__origin__ == list:
+            if len(param_type.__args__) != 1:
+                raise ErrorUnprocessableEntity(f"Invalid param type: {param_type}")
+            return [_convert_param(param_type.__args__[0], el) for el in param_list]
+        else:
+            if len(param_list) == 1:
+                return _convert_param(param_type, param_list[0])
+            else:
+                raise ErrorUnprocessableEntity("Only one param is allowed")
+
     def _method(self, method: str, url: str):
         def decorator(func: FunctionType) -> Callable:
             async def wrapper(data: dict[str: Any],
-                              path_params: dict[str: str] = None,
-                              query_params: dict[str: list[str]] = None) -> Response | StreamResponse:
+                              path_params: dict[str: str],
+                              query_params: dict[str: list[str]]) -> Response | StreamResponse:
                 params = dict()
-                try:
-                    for param_name, param_type in func.__annotations__.items():
-                        if param_type == dict:
-                            if data is not None:
-                                params[param_name] = param_type(data)
-                        elif path_params and param_name in path_params:
-                            params[param_name] = param_type(path_params[param_name])
-                        elif query_params and param_name in query_params:
-                            if param_type != list:
-                                if len(query_params[param_name]) == 1:
-                                    params[param_name] = param_type(query_params[param_name][0])
-                                else:
-                                    raise InternalServerError
-                            else:
-                                params[param_name] = param_type(query_params[param_name])
-                except ValueError:
-                    raise ErrorUnprocessableEntity()
+
+                for param_name, param in path_params.items():
+                    param_type = func.__annotations__.get(param_name, Any)
+                    params[param_name] = _convert_param(param_type, param)
+
+                for param_name, param in query_params.items():
+                    if param_name in path_params:
+                        raise ErrorUnprocessableEntity(f"Duplicate param name: '{param_name}'")
+                    param_type = func.__annotations__.get(param_name, Any)
+                    params[param_name] = self._check_query_param(param, param_type)
+
+                for param_name, param_type in func.__annotations__.items():
+                    if param_name in path_params or param_name in query_params:
+                        continue
+                    elif (p := self._check_data_param(data, param_type)) is not None:
+                        params[param_name] = p
+                    # else:
+                    #     raise ErrorUnprocessableEntity
 
                 try:
                     res = func(**params)
                     if isasyncgen(res) or isgenerator(res):
                         return StreamResponse(res)
                     elif iscoroutine(res):
                         res = await res
-                    return Response(200, res)
+                    return Response(200, _result_to_json(res))
                 except ApiError as e:
                     raise e
                 except Exception as e:
                     raise InternalServerError(f"{e.__class__.__name__}: {e}")
 
             self._add(method, url, wrapper)
```

### Comparing `StdioBridge-1.2.0/StdioBridge/api/errors.py` & `StdioBridge-1.2.1/StdioBridge/api/errors.py`

 * *Files identical despite different names*

### Comparing `StdioBridge-1.2.0/StdioBridge/client/_client.py` & `StdioBridge-1.2.1/StdioBridge/client/_client.py`

 * *Files identical despite different names*

### Comparing `StdioBridge-1.2.0/StdioBridge/client/_response.py` & `StdioBridge-1.2.1/StdioBridge/client/_response.py`

 * *Files identical despite different names*

### Comparing `StdioBridge-1.2.0/StdioBridge.egg-info/PKG-INFO` & `StdioBridge-1.2.1/StdioBridge.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: StdioBridge
-Version: 1.2.0
+Version: 1.2.1
 Summary: A StdioBridge package.
 Home-page: https://github.com/SergeiKrivko
 Author: SergeiKrivko
 License: MIT License
         
         Copyright (c) 2024 SergeiKrivko
```

### Comparing `StdioBridge-1.2.0/setup.py` & `StdioBridge-1.2.1/setup.py`

 * *Files identical despite different names*

