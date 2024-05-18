# Comparing `tmp/oj_tools-0.0.6.tar.gz` & `tmp/oj_tools-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oj_tools-0.0.6.tar", last modified: Fri May 17 07:12:43 2024, max compression
+gzip compressed data, was "oj_tools-0.0.7.tar", last modified: Sat May 18 14:21:14 2024, max compression
```

## Comparing `oj_tools-0.0.6.tar` & `oj_tools-0.0.7.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 07:12:43.066409 oj_tools-0.0.6/
--rw-r--r--   0 runner    (1001) docker     (127)     2301 2024-05-17 07:12:43.066409 oj_tools-0.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1815 2024-05-17 07:12:27.000000 oj_tools-0.0.6/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      489 2024-05-17 07:12:27.000000 oj_tools-0.0.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-17 07:12:43.066409 oj_tools-0.0.6/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 07:12:43.062409 oj_tools-0.0.6/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 07:12:43.062409 oj_tools-0.0.6/src/oj/
--rw-r--r--   0 runner    (1001) docker     (127)      111 2024-05-17 07:12:27.000000 oj_tools-0.0.6/src/oj/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      321 2024-05-17 07:12:27.000000 oj_tools-0.0.6/src/oj/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     2100 2024-05-17 07:12:27.000000 oj_tools-0.0.6/src/oj/problem.py
--rw-r--r--   0 runner    (1001) docker     (127)     1418 2024-05-17 07:12:27.000000 oj_tools-0.0.6/src/oj/testcase.py
--rw-r--r--   0 runner    (1001) docker     (127)     1437 2024-05-17 07:12:27.000000 oj_tools-0.0.6/src/oj/validators.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 07:12:43.066409 oj_tools-0.0.6/src/oj_tools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2301 2024-05-17 07:12:43.000000 oj_tools-0.0.6/src/oj_tools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      265 2024-05-17 07:12:43.000000 oj_tools-0.0.6/src/oj_tools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-17 07:12:43.000000 oj_tools-0.0.6/src/oj_tools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        3 2024-05-17 07:12:43.000000 oj_tools-0.0.6/src/oj_tools.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 14:21:14.094656 oj_tools-0.0.7/
+-rw-r--r--   0 runner    (1001) docker     (127)     2301 2024-05-18 14:21:14.094656 oj_tools-0.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1815 2024-05-18 14:21:08.000000 oj_tools-0.0.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      489 2024-05-18 14:21:08.000000 oj_tools-0.0.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-18 14:21:14.094656 oj_tools-0.0.7/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 14:21:14.090656 oj_tools-0.0.7/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 14:21:14.094656 oj_tools-0.0.7/src/oj/
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-05-18 14:21:08.000000 oj_tools-0.0.7/src/oj/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      321 2024-05-18 14:21:08.000000 oj_tools-0.0.7/src/oj/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2100 2024-05-18 14:21:08.000000 oj_tools-0.0.7/src/oj/problem.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1418 2024-05-18 14:21:08.000000 oj_tools-0.0.7/src/oj/testcase.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3066 2024-05-18 14:21:08.000000 oj_tools-0.0.7/src/oj/validators.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 14:21:14.094656 oj_tools-0.0.7/src/oj_tools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2301 2024-05-18 14:21:14.000000 oj_tools-0.0.7/src/oj_tools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      265 2024-05-18 14:21:14.000000 oj_tools-0.0.7/src/oj_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-18 14:21:14.000000 oj_tools-0.0.7/src/oj_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        3 2024-05-18 14:21:14.000000 oj_tools-0.0.7/src/oj_tools.egg-info/top_level.txt
```

### Comparing `oj_tools-0.0.6/PKG-INFO` & `oj_tools-0.0.7/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oj-tools
-Version: 0.0.6
+Version: 0.0.7
 Summary: tools for Online Judge management
 Author-email: hepheir <hepheir@gmail.com>
 Project-URL: Homepage, https://https://github.com/hepheir/oj-tools
 Project-URL: Issues, https://https://github.com/hepheir/oj-tools/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `oj_tools-0.0.6/README.md` & `oj_tools-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `oj_tools-0.0.6/src/oj/problem.py` & `oj_tools-0.0.7/src/oj/problem.py`

 * *Files identical despite different names*

### Comparing `oj_tools-0.0.6/src/oj/testcase.py` & `oj_tools-0.0.7/src/oj/testcase.py`

 * *Files identical despite different names*

### Comparing `oj_tools-0.0.6/src/oj_tools.egg-info/PKG-INFO` & `oj_tools-0.0.7/src/oj_tools.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oj-tools
-Version: 0.0.6
+Version: 0.0.7
 Summary: tools for Online Judge management
 Author-email: hepheir <hepheir@gmail.com>
 Project-URL: Homepage, https://https://github.com/hepheir/oj-tools
 Project-URL: Issues, https://https://github.com/hepheir/oj-tools/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

