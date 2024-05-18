# Comparing `tmp/StdioBridge-1.0.1.tar.gz` & `tmp/StdioBridge-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "StdioBridge-1.0.1.tar", last modified: Fri May 17 15:07:36 2024, max compression
+gzip compressed data, was "StdioBridge-1.1.0.tar", last modified: Fri May 17 19:59:01 2024, max compression
```

## Comparing `StdioBridge-1.0.1.tar` & `StdioBridge-1.1.0.tar`

### file list

```diff
@@ -1,21 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 15:07:36.982055 StdioBridge-1.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-05-17 15:07:27.000000 StdioBridge-1.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3536 2024-05-17 15:07:36.982055 StdioBridge-1.0.1/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 15:07:36.982055 StdioBridge-1.0.1/StdioBridge/
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-17 15:07:27.000000 StdioBridge-1.0.1/StdioBridge/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-17 15:07:27.000000 StdioBridge-1.0.1/StdioBridge/_config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 15:07:36.982055 StdioBridge-1.0.1/StdioBridge/api/
--rw-r--r--   0 runner    (1001) docker     (127)      120 2024-05-17 15:07:27.000000 StdioBridge-1.0.1/StdioBridge/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5878 2024-05-17 15:07:27.000000 StdioBridge-1.0.1/StdioBridge/api/_api.py
--rw-r--r--   0 runner    (1001) docker     (127)      114 2024-05-17 15:07:27.000000 StdioBridge-1.0.1/StdioBridge/api/_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     1424 2024-05-17 15:07:27.000000 StdioBridge-1.0.1/StdioBridge/api/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 15:07:36.982055 StdioBridge-1.0.1/StdioBridge/client/
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-17 15:07:27.000000 StdioBridge-1.0.1/StdioBridge/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2952 2024-05-17 15:07:27.000000 StdioBridge-1.0.1/StdioBridge/client/_client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 15:07:36.982055 StdioBridge-1.0.1/StdioBridge.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3536 2024-05-17 15:07:36.000000 StdioBridge-1.0.1/StdioBridge.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      371 2024-05-17 15:07:36.000000 StdioBridge-1.0.1/StdioBridge.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-17 15:07:36.000000 StdioBridge-1.0.1/StdioBridge.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-17 15:07:36.000000 StdioBridge-1.0.1/StdioBridge.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-17 15:07:36.982055 StdioBridge-1.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1170 2024-05-17 15:07:27.000000 StdioBridge-1.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 19:59:01.249398 StdioBridge-1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-05-17 19:58:53.000000 StdioBridge-1.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3536 2024-05-17 19:59:01.249398 StdioBridge-1.1.0/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 19:59:01.249398 StdioBridge-1.1.0/StdioBridge/
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-17 19:58:53.000000 StdioBridge-1.1.0/StdioBridge/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-17 19:58:53.000000 StdioBridge-1.1.0/StdioBridge/_config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 19:59:01.249398 StdioBridge-1.1.0/StdioBridge/api/
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-05-17 19:58:53.000000 StdioBridge-1.1.0/StdioBridge/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5476 2024-05-17 19:58:53.000000 StdioBridge-1.1.0/StdioBridge/api/_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      822 2024-05-17 19:58:53.000000 StdioBridge-1.1.0/StdioBridge/api/_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2165 2024-05-17 19:58:53.000000 StdioBridge-1.1.0/StdioBridge/api/_router.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1424 2024-05-17 19:58:53.000000 StdioBridge-1.1.0/StdioBridge/api/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 19:59:01.249398 StdioBridge-1.1.0/StdioBridge/client/
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-05-17 19:58:53.000000 StdioBridge-1.1.0/StdioBridge/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4046 2024-05-17 19:58:53.000000 StdioBridge-1.1.0/StdioBridge/client/_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1334 2024-05-17 19:58:53.000000 StdioBridge-1.1.0/StdioBridge/client/_response.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 19:59:01.249398 StdioBridge-1.1.0/StdioBridge.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3536 2024-05-17 19:59:01.000000 StdioBridge-1.1.0/StdioBridge.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      464 2024-05-17 19:59:01.000000 StdioBridge-1.1.0/StdioBridge.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-17 19:59:01.000000 StdioBridge-1.1.0/StdioBridge.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-17 19:59:01.000000 StdioBridge-1.1.0/StdioBridge.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-17 19:59:01.000000 StdioBridge-1.1.0/StdioBridge.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-17 19:59:01.249398 StdioBridge-1.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1170 2024-05-17 19:58:53.000000 StdioBridge-1.1.0/setup.py
```

### Comparing `StdioBridge-1.0.1/LICENSE` & `StdioBridge-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `StdioBridge-1.0.1/PKG-INFO` & `StdioBridge-1.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: StdioBridge
-Version: 1.0.1
+Version: 1.1.0
 Summary: A StdioBridge package.
 Home-page: https://github.com/SergeiKrivko
 Author: SergeiKrivko
 License: MIT License
         
         Copyright (c) 2024 SergeiKrivko
```

### Comparing `StdioBridge-1.0.1/StdioBridge/api/errors.py` & `StdioBridge-1.1.0/StdioBridge/api/errors.py`

 * *Files identical despite different names*

### Comparing `StdioBridge-1.0.1/StdioBridge.egg-info/PKG-INFO` & `StdioBridge-1.1.0/StdioBridge.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: StdioBridge
-Version: 1.0.1
+Version: 1.1.0
 Summary: A StdioBridge package.
 Home-page: https://github.com/SergeiKrivko
 Author: SergeiKrivko
 License: MIT License
         
         Copyright (c) 2024 SergeiKrivko
```

### Comparing `StdioBridge-1.0.1/setup.py` & `StdioBridge-1.1.0/setup.py`

 * *Files identical despite different names*

