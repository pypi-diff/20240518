# Comparing `tmp/python_http_request-0.0.1.tar.gz` & `tmp/python_http_request-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_http_request-0.0.1.tar", max compression
+gzip compressed data, was "python_http_request-0.0.2.tar", max compression
```

## Comparing `python_http_request-0.0.1.tar` & `python_http_request-0.0.2.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rwxr-xr-x   0        0        0     1100 2024-01-29 04:51:11.346824 python_http_request-0.0.1/LICENSE
--rwxr-xr-x   0        0        0     3992 2024-05-17 14:53:01.589521 python_http_request-0.0.1/http_request/__init__.py
--rw-r--r--   0        0        0        0 2024-01-30 04:55:37.590943 python_http_request-0.0.1/http_request/py.typed
--rw-r--r--   0        0        0     1234 2024-05-17 15:05:41.841003 python_http_request-0.0.1/pyproject.toml
--rw-r--r--   0        0        0      219 2024-05-17 15:05:56.280517 python_http_request-0.0.1/readme.md
--rw-r--r--   0        0        0     1457 1970-01-01 00:00:00.000000 python_http_request-0.0.1/PKG-INFO
+-rwxr-xr-x   0        0        0     1100 2024-01-29 04:51:11.346824 python_http_request-0.0.2/LICENSE
+-rwxr-xr-x   0        0        0     4690 2024-05-18 16:18:51.151968 python_http_request-0.0.2/http_request/__init__.py
+-rw-r--r--   0        0        0        0 2024-01-30 04:55:37.590943 python_http_request-0.0.2/http_request/py.typed
+-rw-r--r--   0        0        0     1234 2024-05-18 16:19:30.790986 python_http_request-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0      219 2024-05-17 15:05:56.280517 python_http_request-0.0.2/readme.md
+-rw-r--r--   0        0        0     1457 1970-01-01 00:00:00.000000 python_http_request-0.0.2/PKG-INFO
```

### Comparing `python_http_request-0.0.1/LICENSE` & `python_http_request-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `python_http_request-0.0.1/http_request/__init__.py` & `python_http_request-0.0.2/http_request/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,25 +1,32 @@
 #!/usr/bin/env python3
 # encoding: utf-8
 
 __author__ = "ChenyangGao <https://chenyanggao.github.io>"
-__version__ = (0, 0, 1)
-__all__ = ["encode_multipart_data", "encode_multipart_data_async"]
+__version__ = (0, 0, 2)
+__all__ = ["SupportsGeturl", "encode_multipart_data", "encode_multipart_data_async"]
 
 from itertools import chain
 from collections.abc import AsyncIterable, AsyncIterator, ItemsView, Iterable, Iterator, Mapping
-from typing import Any
+from typing import Any, Protocol, TypeVar
 from urllib.parse import quote
 from uuid import uuid4
 
 from asynctools import ensure_aiter, async_chain
 from filewrap import bio_chunk_iter, bio_chunk_async_iter, SupportsRead
 from integer_tool import int_to_bytes
 
 
+AnyStr = TypeVar("AnyStr", bytes, str, covariant=True)
+
+
+class SupportsGeturl(Protocol[AnyStr]):
+    def geturl(self) -> AnyStr: ...
+
+
 def ensure_bytes(s, /) -> bytes | bytearray | memoryview:
     if isinstance(s, (bytes, bytearray, memoryview)):
         return s
     if isinstance(s, int):
         return int_to_bytes(s)
     elif isinstance(s, str):
         return bytes(s, "utf-8")
@@ -27,31 +34,33 @@
         return bytes(s)
     except TypeError:
         return bytes(str(s), "utf-8")
 
 
 def encode_multipart_data(
     data: Mapping[str, Any], 
-    files: Mapping[str, bytes | bytearray | memoryview | SupportsRead[bytes] | Iterable[bytes]], 
+    files: Mapping[str, bytes | bytearray | memoryview | 
+                        SupportsRead[bytes] | SupportsRead[bytearray] | SupportsRead[memoryview] | 
+                        Iterable[bytes] | Iterable[bytearray] | Iterable[memoryview]], 
     boundary: None | str = None, 
-) -> tuple[dict, Iterator[bytes]]:
+) -> tuple[dict, Iterator[bytes | bytearray | memoryview]]:
     if not boundary:
         boundary = uuid4().bytes.hex()
     headers = {"Content-Type": f"multipart/form-data; boundary={boundary}"}
 
-    def encode_data(data) -> Iterator[bytes]:
+    def encode_data(data) -> Iterator[bytes | bytearray | memoryview]:
         if isinstance(data, Mapping):
             data = ItemsView(data)
         for name, value in data:
             yield boundary_line
             yield b'Content-Disposition: form-data; name="%s"\r\n\r\n' % bytes(quote(name), "ascii")
             yield ensure_bytes(value)
             yield b"\r\n"
 
-    def encode_files(files) -> Iterator[bytes]:
+    def encode_files(files) -> Iterator[bytes | bytearray | memoryview]:
         if isinstance(files, Mapping):
             files = ItemsView(files)
         for name, file in files:
             yield boundary_line
             yield b'Content-Disposition: form-data; name="%s"\r\nContent-Type: application/octet-stream\r\n\r\n' % bytes(quote(name), "ascii")
             if isinstance(file, (bytes, bytearray, memoryview)):
                 yield file
@@ -63,31 +72,34 @@
 
     boundary_line = b"--%s\r\n" % boundary.encode("utf-8")
     return headers, chain(encode_data(data), encode_files(files), (b'--%s--\r\n' % boundary.encode("ascii"),))
 
 
 def encode_multipart_data_async(
     data: Mapping[str, Any], 
-    files: Mapping[str, bytes | bytearray | memoryview | SupportsRead[bytes] | Iterable[bytes] | AsyncIterable[bytes]], 
+    files: Mapping[str, bytes | bytearray | memoryview | 
+                        SupportsRead[bytes] | SupportsRead[bytearray] | SupportsRead[memoryview] | 
+                        Iterable[bytes] | Iterable[bytearray] | Iterable[memoryview] | 
+                        AsyncIterable[bytes] | AsyncIterable[bytearray] | AsyncIterable[memoryview]], 
     boundary: None | str = None, 
-) -> tuple[dict, AsyncIterator[bytes]]:
+) -> tuple[dict, AsyncIterator[bytes | bytearray | memoryview]]:
     if not boundary:
         boundary = uuid4().bytes.hex()
     headers = {"Content-Type": f"multipart/form-data; boundary={boundary}"}
 
-    async def encode_data(data) -> AsyncIterator[bytes]:
+    async def encode_data(data) -> AsyncIterator[bytes | bytearray | memoryview]:
         if isinstance(data, Mapping):
             data = ItemsView(data)
         for name, value in data:
             yield boundary_line
             yield b'Content-Disposition: form-data; name="%s"\r\n\r\n' % bytes(quote(name), "ascii")
             yield ensure_bytes(value)
             yield b"\r\n"
 
-    async def encode_files(files) -> AsyncIterator[bytes]:
+    async def encode_files(files) -> AsyncIterator[bytes | bytearray | memoryview]:
         if isinstance(files, Mapping):
             files = ItemsView(files)
         for name, file in files:
             yield boundary_line
             yield b'Content-Disposition: form-data; name="%s"\r\nContent-Type: application/octet-stream\r\n\r\n' % bytes(quote(name), "ascii")
             if isinstance(file, (bytes, bytearray, memoryview)):
                 yield file
```

### Comparing `python_http_request-0.0.1/pyproject.toml` & `python_http_request-0.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "python-http_request"
-version = "0.0.1"
+version = "0.0.2"
 description = "Python http response utils."
 authors = ["ChenyangGao <wosiwujm@gmail.com>"]
 license = "MIT"
 readme = "readme.md"
 homepage = "https://github.com/ChenyangGao/web-mount-packs/tree/main/python-module/python-http_request"
 repository = "https://github.com/ChenyangGao/web-mount-packs/tree/main/python-module/python-http_request"
 keywords = ["http", "request"]
```

### Comparing `python_http_request-0.0.1/PKG-INFO` & `python_http_request-0.0.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-http_request
-Version: 0.0.1
+Version: 0.0.2
 Summary: Python http response utils.
 Home-page: https://github.com/ChenyangGao/web-mount-packs/tree/main/python-module/python-http_request
 License: MIT
 Keywords: http,request
 Author: ChenyangGao
 Author-email: wosiwujm@gmail.com
 Requires-Python: >=3.10,<4.0
```

