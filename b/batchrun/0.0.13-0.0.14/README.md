# Comparing `tmp/batchrun-0.0.13.tar.gz` & `tmp/batchrun-0.0.14.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "batchrun-0.0.13.tar", max compression
+gzip compressed data, was "batchrun-0.0.14.tar", max compression
```

## Comparing `batchrun-0.0.13.tar` & `batchrun-0.0.14.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     2017 2024-02-12 02:06:41.797467 batchrun-0.0.13/README.md
--rw-r--r--   0        0        0       29 2024-01-23 14:36:10.370721 batchrun-0.0.13/batchrun/__init__.py
--rwxr-xr-x   0        0        0     8657 2024-02-12 01:29:03.786086 batchrun-0.0.13/batchrun/cli.py
--rw-r--r--   0        0        0     2055 2023-01-18 00:03:16.169422 batchrun-0.0.13/batchrun/spec.py
--rw-r--r--   0        0        0      643 2024-02-12 02:08:39.894018 batchrun-0.0.13/pyproject.toml
--rw-r--r--   0        0        0     2677 1970-01-01 00:00:00.000000 batchrun-0.0.13/PKG-INFO
+-rw-r--r--   0        0        0     2017 2024-02-12 02:06:41.797467 batchrun-0.0.14/README.md
+-rw-r--r--   0        0        0       29 2024-01-23 14:36:10.370721 batchrun-0.0.14/batchrun/__init__.py
+-rwxr-xr-x   0        0        0     8657 2024-02-12 01:29:03.786086 batchrun-0.0.14/batchrun/cli.py
+-rw-r--r--   0        0        0     2407 2024-05-18 09:51:27.198248 batchrun-0.0.14/batchrun/spec.py
+-rw-r--r--   0        0        0      643 2024-05-18 09:54:34.991342 batchrun-0.0.14/pyproject.toml
+-rw-r--r--   0        0        0     2677 1970-01-01 00:00:00.000000 batchrun-0.0.14/PKG-INFO
```

### Comparing `batchrun-0.0.13/README.md` & `batchrun-0.0.14/README.md`

 * *Files identical despite different names*

### Comparing `batchrun-0.0.13/batchrun/cli.py` & `batchrun-0.0.14/batchrun/cli.py`

 * *Files identical despite different names*

### Comparing `batchrun-0.0.13/pyproject.toml` & `batchrun-0.0.14/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "batchrun"
-version = "0.0.13"
+version = "0.0.14"
 description = "A simple workflow for executing scripts in parallel with varying argument values"
 authors = ["Bogdan Kulynych <bogdan@kulyny.ch>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `batchrun-0.0.13/PKG-INFO` & `batchrun-0.0.14/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: batchrun
-Version: 0.0.13
+Version: 0.0.14
 Summary: A simple workflow for executing scripts in parallel with varying argument values
 License: MIT
 Author: Bogdan Kulynych
 Author-email: bogdan@kulyny.ch
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

