# Comparing `tmp/fast_version-1.1.0.tar.gz` & `tmp/fast_version-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fast_version-1.1.0.tar", max compression
+gzip compressed data, was "fast_version-1.2.0.tar", max compression
```

## Comparing `fast_version-1.1.0.tar` & `fast_version-1.2.0.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1070 2024-03-30 10:36:32.829777 fast_version-1.1.0/LICENSE
--rw-r--r--   0        0        0     1107 2024-03-30 10:36:32.830511 fast_version-1.1.0/README.md
--rw-r--r--   0        0        0      177 2023-09-10 19:49:22.104243 fast_version-1.1.0/fast_version/__init__.py
--rw-r--r--   0        0        0     4511 2024-03-31 09:14:00.747145 fast_version-1.1.0/fast_version/app.py
--rw-r--r--   0        0        0      800 2023-09-04 07:12:34.000000 fast_version-1.1.0/fast_version/helpers.py
--rw-r--r--   0        0        0        0 2023-08-28 10:48:35.000000 fast_version-1.1.0/fast_version/py.typed
--rw-r--r--   0        0        0     2351 2024-03-30 10:36:37.772924 fast_version-1.1.0/fast_version/router.py
--rw-r--r--   0        0        0     1392 2024-04-29 08:00:34.410728 fast_version-1.1.0/pyproject.toml
--rw-r--r--   0        0        0     1759 1970-01-01 00:00:00.000000 fast_version-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1070 2024-03-30 10:36:32.829777 fast_version-1.2.0/LICENSE
+-rw-r--r--   0        0        0     1928 2024-05-18 04:54:16.978187 fast_version-1.2.0/README.md
+-rw-r--r--   0        0        0      177 2023-09-10 19:49:22.104243 fast_version-1.2.0/fast_version/__init__.py
+-rw-r--r--   0        0        0     4511 2024-03-31 09:14:00.747145 fast_version-1.2.0/fast_version/app.py
+-rw-r--r--   0        0        0      800 2023-09-04 07:12:34.000000 fast_version-1.2.0/fast_version/helpers.py
+-rw-r--r--   0        0        0        0 2023-08-28 10:48:35.000000 fast_version-1.2.0/fast_version/py.typed
+-rw-r--r--   0        0        0     2351 2024-03-30 10:36:37.772924 fast_version-1.2.0/fast_version/router.py
+-rw-r--r--   0        0        0     1393 2024-05-18 04:56:14.257000 fast_version-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0     2481 1970-01-01 00:00:00.000000 fast_version-1.2.0/PKG-INFO
```

### Comparing `fast_version-1.1.0/LICENSE` & `fast_version-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `fast_version-1.1.0/fast_version/app.py` & `fast_version-1.2.0/fast_version/app.py`

 * *Files identical despite different names*

### Comparing `fast_version-1.1.0/fast_version/helpers.py` & `fast_version-1.2.0/fast_version/helpers.py`

 * *Files identical despite different names*

### Comparing `fast_version-1.1.0/fast_version/router.py` & `fast_version-1.2.0/fast_version/router.py`

 * *Files identical despite different names*

### Comparing `fast_version-1.1.0/pyproject.toml` & `fast_version-1.2.0/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 [tool.poetry]
 name = "fast-version"
-version = "1.1.0"
+version = "1.2.0"
 description = "Fastapi versioning package with accept header"
 authors = ["Artur Shiriev <me@shiriev.ru>"]
 readme = "README.md"
 classifiers = ["Programming Language :: Python :: 3.11", "Framework :: Pytest"]
 homepage = "https://github.com/modern-python/fast-version"
 packages = [
     { include = "fast_version" },
 ]
 
 [tool.poetry.dependencies]
-python = ">=3.8,<4"
+python = ">=3.10,<4"
 fastapi = ">=0.100"
 
 [tool.poetry.dev-dependencies]
 pytest = "*"
 pytest-asyncio = "*"
 pytest-cov = "*"
 httpx = "*"
```

