# Comparing `tmp/aiohttp_zip_response-1.0.1.tar.gz` & `tmp/aiohttp_zip_response-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiohttp_zip_response-1.0.1.tar", max compression
+gzip compressed data, was "aiohttp_zip_response-1.0.2.tar", max compression
```

## Comparing `aiohttp_zip_response-1.0.1.tar` & `aiohttp_zip_response-1.0.2.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1054 2024-05-16 03:13:45.883256 aiohttp_zip_response-1.0.1/LICENSE
--rw-r--r--   0        0        0     1175 2024-05-16 05:44:11.765663 aiohttp_zip_response-1.0.1/README.md
--rw-r--r--   0        0        0       65 2024-05-16 03:05:23.867378 aiohttp_zip_response-1.0.1/aiohttp_zip_response/__init__.py
--rw-r--r--   0        0        0        0 2024-05-16 05:57:50.168509 aiohttp_zip_response-1.0.1/aiohttp_zip_response/py.typed
--rw-r--r--   0        0        0     1458 2024-05-16 03:56:21.230282 aiohttp_zip_response-1.0.1/aiohttp_zip_response/zip_response.py
--rw-r--r--   0        0        0     1458 2024-05-16 05:57:50.168509 aiohttp_zip_response-1.0.1/pyproject.toml
--rw-r--r--   0        0        0     2384 1970-01-01 00:00:00.000000 aiohttp_zip_response-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1054 2024-05-16 03:13:45.883256 aiohttp_zip_response-1.0.2/LICENSE
+-rw-r--r--   0        0        0     1473 2024-05-18 16:24:15.578429 aiohttp_zip_response-1.0.2/README.md
+-rw-r--r--   0        0        0       65 2024-05-16 03:05:23.867378 aiohttp_zip_response-1.0.2/aiohttp_zip_response/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-16 05:57:50.168509 aiohttp_zip_response-1.0.2/aiohttp_zip_response/py.typed
+-rw-r--r--   0        0        0     1458 2024-05-16 03:56:21.230282 aiohttp_zip_response-1.0.2/aiohttp_zip_response/zip_response.py
+-rw-r--r--   0        0        0     1458 2024-05-18 16:24:15.578429 aiohttp_zip_response-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0     2682 1970-01-01 00:00:00.000000 aiohttp_zip_response-1.0.2/PKG-INFO
```

### Comparing `aiohttp_zip_response-1.0.1/LICENSE` & `aiohttp_zip_response-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `aiohttp_zip_response-1.0.1/aiohttp_zip_response/zip_response.py` & `aiohttp_zip_response-1.0.2/aiohttp_zip_response/zip_response.py`

 * *Files identical despite different names*

### Comparing `aiohttp_zip_response-1.0.1/pyproject.toml` & `aiohttp_zip_response-1.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "aiohttp-zip-response"
-version = "1.0.1"
+version = "1.0.2"
 description = "A AIOHTTP response class streaming a directory as ZIP archive"
 authors = ["Jonathan Ehwald <github@ehwald.info>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/DoctorJohn/aiohttp-zip-response"
 repository = "https://github.com/DoctorJohn/aiohttp-zip-response"
 documentation = "https://github.com/DoctorJohn/aiohttp-zip-response"
```

### Comparing `aiohttp_zip_response-1.0.1/PKG-INFO` & `aiohttp_zip_response-1.0.2/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiohttp-zip-response
-Version: 1.0.1
+Version: 1.0.2
 Summary: A AIOHTTP response class streaming a directory as ZIP archive
 Home-page: https://github.com/DoctorJohn/aiohttp-zip-response
 License: MIT
 Author: Jonathan Ehwald
 Author-email: github@ehwald.info
 Requires-Python: >=3.9,<4.0
 Classifier: Environment :: Web Environment
@@ -38,15 +38,18 @@
 [pypi-image]: https://img.shields.io/pypi/v/aiohttp-zip-response
 [pypi-url]: https://pypi.org/project/aiohttp-zip-response/
 [codecov-image]: https://codecov.io/gh/DoctorJohn/aiohttp-zip-response/branch/main/graph/badge.svg
 [codecov-url]: https://codecov.io/gh/DoctorJohn/aiohttp-zip-response
 [license-image]: https://img.shields.io/pypi/l/aiohttp-zip-response
 [license-url]: https://github.com/DoctorJohn/aiohttp-zip-response/blob/master/LICENSE
 
-A AIOHTTP response class streaming a directory as ZIP archive.
+A AIOHTTP response class streaming the contents of a directory as a ZIP archive.
+Thanks to [stream-zip](https://github.com/uktrade/stream-zip/), this works **without storing the entire ZIP in memory or disk**.
+
+Generally, this package is meant to complement the existing `aiohttp.web.FileResponse` class, which can already stream the contents of a single file.
 
 ## Installation
 
 ```bash
 pip install aiohttp-zip-response
 ```
```

