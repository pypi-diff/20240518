# Comparing `tmp/asyncupbit-0.1.0.tar.gz` & `tmp/asyncupbit-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "asyncupbit-0.1.0.tar", max compression
+gzip compressed data, was "asyncupbit-0.1.1.tar", max compression
```

## Comparing `asyncupbit-0.1.0.tar` & `asyncupbit-0.1.1.tar`

### file list

```diff
@@ -1,8 +1,9 @@
--rw-r--r--   0        0        0     1067 2024-05-18 16:37:01.069677 asyncupbit-0.1.0/LICENSE
--rw-r--r--   0        0        0       71 2024-05-18 16:37:01.069677 asyncupbit-0.1.0/README.md
--rw-r--r--   0        0        0       50 2024-05-18 16:37:01.069677 asyncupbit-0.1.0/asyncupbit/__init__.py
--rw-r--r--   0        0        0     8235 2024-05-18 16:37:01.069677 asyncupbit-0.1.0/asyncupbit/client.py
--rw-r--r--   0        0        0      764 2024-05-18 16:37:01.069677 asyncupbit-0.1.0/asyncupbit/errors.py
--rw-r--r--   0        0        0     6662 2024-05-18 16:37:01.069677 asyncupbit-0.1.0/asyncupbit/types.py
--rw-r--r--   0        0        0      914 2024-05-18 16:37:01.069677 asyncupbit-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      582 1970-01-01 00:00:00.000000 asyncupbit-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1067 2024-05-18 16:54:41.703177 asyncupbit-0.1.1/LICENSE
+-rw-r--r--   0        0        0      123 2024-05-18 16:54:41.703177 asyncupbit-0.1.1/README.md
+-rw-r--r--   0        0        0      274 2024-05-18 16:54:41.703177 asyncupbit-0.1.1/asyncupbit/__init__.py
+-rw-r--r--   0        0        0     8235 2024-05-18 16:54:41.703177 asyncupbit-0.1.1/asyncupbit/client.py
+-rw-r--r--   0        0        0      764 2024-05-18 16:54:41.703177 asyncupbit-0.1.1/asyncupbit/errors.py
+-rw-r--r--   0        0        0        0 2024-05-18 16:54:41.703177 asyncupbit-0.1.1/asyncupbit/py.typed
+-rw-r--r--   0        0        0     6662 2024-05-18 16:54:41.703177 asyncupbit-0.1.1/asyncupbit/types.py
+-rw-r--r--   0        0        0      916 2024-05-18 16:54:41.703177 asyncupbit-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      634 1970-01-01 00:00:00.000000 asyncupbit-0.1.1/PKG-INFO
```

### Comparing `asyncupbit-0.1.0/LICENSE` & `asyncupbit-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `asyncupbit-0.1.0/asyncupbit/client.py` & `asyncupbit-0.1.1/asyncupbit/client.py`

 * *Files identical despite different names*

### Comparing `asyncupbit-0.1.0/asyncupbit/errors.py` & `asyncupbit-0.1.1/asyncupbit/errors.py`

 * *Files identical despite different names*

### Comparing `asyncupbit-0.1.0/asyncupbit/types.py` & `asyncupbit-0.1.1/asyncupbit/types.py`

 * *Files identical despite different names*

### Comparing `asyncupbit-0.1.0/pyproject.toml` & `asyncupbit-0.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "asyncupbit"
-version = "0.1.0"
+version = "0.1.1"
 description = "비동기 기반의 파이썬 업비트 API 클라이언트"
 authors = ["sjquant <seonujang92@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
@@ -33,15 +33,15 @@
     "I",  # isort
     "B",  # flake8-bugbear
     "C4", # flake8-comprehensions
     "UP", # pyupgrade
 ]
 
 [tool.pyright]
-include = ["aioupbit"]
+include = ["asyncupbit"]
 exclude = [
     "**/__pycache__",
 ]
 pythonVersion = "3.10"
 typeCheckingMode = "strict"
```

