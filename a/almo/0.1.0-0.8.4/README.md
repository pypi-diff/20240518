# Comparing `tmp/almo-0.1.0.tar.gz` & `tmp/almo-0.8.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "almo-0.1.0.tar", last modified: Sat May 18 09:47:41 2024, max compression
+gzip compressed data, was "almo-0.8.4.tar", last modified: Sat May 18 14:25:28 2024, max compression
```

## Comparing `almo-0.1.0.tar` & `almo-0.8.4.tar`

### file list

```diff
@@ -1,13 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 09:47:41.608703 almo-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1081 2024-05-18 09:47:30.000000 almo-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4997 2024-05-18 09:47:41.608703 almo-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4810 2024-05-18 09:47:30.000000 almo-0.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 09:47:41.608703 almo-0.1.0/almo.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4997 2024-05-18 09:47:41.000000 almo-0.1.0/almo.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      180 2024-05-18 09:47:41.000000 almo-0.1.0/almo.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-18 09:47:41.000000 almo-0.1.0/almo.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-18 09:47:41.000000 almo-0.1.0/almo.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-18 09:47:41.000000 almo-0.1.0/almo.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      116 2024-05-18 09:47:30.000000 almo-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-18 09:47:41.608703 almo-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      700 2024-05-18 09:47:30.000000 almo-0.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 14:25:28.338556 almo-0.8.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1081 2024-05-18 14:25:14.000000 almo-0.8.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-18 14:25:14.000000 almo-0.8.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4997 2024-05-18 14:25:28.338556 almo-0.8.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4810 2024-05-18 14:25:14.000000 almo-0.8.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 14:25:28.338556 almo-0.8.4/almo.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4997 2024-05-18 14:25:28.000000 almo-0.8.4/almo.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      334 2024-05-18 14:25:28.000000 almo-0.8.4/almo.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-18 14:25:28.000000 almo-0.8.4/almo.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-18 14:25:28.000000 almo-0.8.4/almo.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-18 14:25:28.000000 almo-0.8.4/almo.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-05-18 14:25:14.000000 almo-0.8.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-18 14:25:28.338556 almo-0.8.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      700 2024-05-18 14:25:14.000000 almo-0.8.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 14:25:28.338556 almo-0.8.4/src/
+-rw-r--r--   0 runner    (1001) docker     (127)     6258 2024-05-18 14:25:14.000000 almo-0.8.4/src/almo.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    37825 2024-05-18 14:25:14.000000 almo-0.8.4/src/ast.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     6645 2024-05-18 14:25:14.000000 almo-0.8.4/src/dark.css
+-rw-r--r--   0 runner    (1001) docker     (127)     6583 2024-05-18 14:25:14.000000 almo-0.8.4/src/light.css
+-rw-r--r--   0 runner    (1001) docker     (127)    43762 2024-05-18 14:25:14.000000 almo-0.8.4/src/parse.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)      954 2024-05-18 14:25:14.000000 almo-0.8.4/src/pyalmo.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3188 2024-05-18 14:25:14.000000 almo-0.8.4/src/render.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     4896 2024-05-18 14:25:14.000000 almo-0.8.4/src/runner.js
+-rw-r--r--   0 runner    (1001) docker     (127)     5558 2024-05-18 14:25:14.000000 almo-0.8.4/src/template.html
+-rw-r--r--   0 runner    (1001) docker     (127)     6869 2024-05-18 14:25:14.000000 almo-0.8.4/src/utils.hpp
```

### Comparing `almo-0.1.0/LICENSE` & `almo-0.8.4/LICENSE`

 * *Files identical despite different names*

### Comparing `almo-0.1.0/PKG-INFO` & `almo-0.8.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: almo
-Version: 0.1.0
+Version: 0.8.4
 Home-page: https://github.com/abap34/ALMO
 Author: abap34, ebi-fly13, noya2
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # ALMO
```

### Comparing `almo-0.1.0/README.md` & `almo-0.8.4/README.md`

 * *Files identical despite different names*

### Comparing `almo-0.1.0/almo.egg-info/PKG-INFO` & `almo-0.8.4/almo.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: almo
-Version: 0.1.0
+Version: 0.8.4
 Home-page: https://github.com/abap34/ALMO
 Author: abap34, ebi-fly13, noya2
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # ALMO
```

### Comparing `almo-0.1.0/setup.py` & `almo-0.8.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import os
 from pybind11.setup_helpers import Pybind11Extension, build_ext
 from setuptools import setup
 
 os.system("bash scripts/setup.sh")
-__version__ = "0.1.0"
+__version__ = "0.8.4"
 
 ext_modules = [
     Pybind11Extension(
         "almo",
         ["build/pyalmo.cpp"],
         cxx_std=20,
         define_macros=[("VERSION_INFO", "\"" + __version__ + "\"")],
```

