# Comparing `tmp/pytest_aws_apigateway-0.6.0.tar.gz` & `tmp/pytest_aws_apigateway-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest_aws_apigateway-0.6.0.tar", last modified: Thu May 16 16:10:53 2024, max compression
+gzip compressed data, was "pytest_aws_apigateway-0.7.0.tar", last modified: Sat May 18 10:15:31 2024, max compression
```

## Comparing `pytest_aws_apigateway-0.6.0.tar` & `pytest_aws_apigateway-0.7.0.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 16:10:53.868823 pytest_aws_apigateway-0.6.0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 16:10:53.860823 pytest_aws_apigateway-0.6.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 16:10:53.864823 pytest_aws_apigateway-0.6.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1284 2024-05-16 16:10:47.000000 pytest_aws_apigateway-0.6.0/.github/workflows/main.yml
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-16 16:10:47.000000 pytest_aws_apigateway-0.6.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      335 2024-05-16 16:10:47.000000 pytest_aws_apigateway-0.6.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      897 2024-05-16 16:10:47.000000 pytest_aws_apigateway-0.6.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-05-16 16:10:47.000000 pytest_aws_apigateway-0.6.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3547 2024-05-16 16:10:53.868823 pytest_aws_apigateway-0.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1342 2024-05-16 16:10:47.000000 pytest_aws_apigateway-0.6.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 16:10:53.864823 pytest_aws_apigateway-0.6.0/changes/
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-05-16 16:10:47.000000 pytest_aws_apigateway-0.6.0/changes/+.fix.md
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-16 16:10:47.000000 pytest_aws_apigateway-0.6.0/changes/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1384 2024-05-16 16:10:47.000000 pytest_aws_apigateway-0.6.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-16 16:10:47.000000 pytest_aws_apigateway-0.6.0/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-16 16:10:47.000000 pytest_aws_apigateway-0.6.0/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-16 16:10:53.868823 pytest_aws_apigateway-0.6.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 16:10:53.864823 pytest_aws_apigateway-0.6.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 16:10:53.864823 pytest_aws_apigateway-0.6.0/src/pytest_aws_apigateway/
--rw-r--r--   0 runner    (1001) docker     (127)      163 2024-05-16 16:10:47.000000 pytest_aws_apigateway-0.6.0/src/pytest_aws_apigateway/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2960 2024-05-16 16:10:47.000000 pytest_aws_apigateway-0.6.0/src/pytest_aws_apigateway/apigateway.py
--rw-r--r--   0 runner    (1001) docker     (127)      707 2024-05-16 16:10:47.000000 pytest_aws_apigateway-0.6.0/src/pytest_aws_apigateway/context.py
--rw-r--r--   0 runner    (1001) docker     (127)     2229 2024-05-16 16:10:47.000000 pytest_aws_apigateway-0.6.0/src/pytest_aws_apigateway/integration.py
--rw-r--r--   0 runner    (1001) docker     (127)      217 2024-05-16 16:10:47.000000 pytest_aws_apigateway-0.6.0/src/pytest_aws_apigateway/plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 16:10:53.868823 pytest_aws_apigateway-0.6.0/src/pytest_aws_apigateway.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3547 2024-05-16 16:10:53.000000 pytest_aws_apigateway-0.6.0/src/pytest_aws_apigateway.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      844 2024-05-16 16:10:53.000000 pytest_aws_apigateway-0.6.0/src/pytest_aws_apigateway.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 16:10:53.000000 pytest_aws_apigateway-0.6.0/src/pytest_aws_apigateway.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-05-16 16:10:53.000000 pytest_aws_apigateway-0.6.0/src/pytest_aws_apigateway.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-16 16:10:53.000000 pytest_aws_apigateway-0.6.0/src/pytest_aws_apigateway.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-16 16:10:53.000000 pytest_aws_apigateway-0.6.0/src/pytest_aws_apigateway.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 16:10:53.868823 pytest_aws_apigateway-0.6.0/tasks/
--rw-r--r--   0 runner    (1001) docker     (127)     3213 2024-05-16 16:10:47.000000 pytest_aws_apigateway-0.6.0/tasks/release.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 16:10:53.868823 pytest_aws_apigateway-0.6.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 16:10:47.000000 pytest_aws_apigateway-0.6.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-16 16:10:47.000000 pytest_aws_apigateway-0.6.0/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     3498 2024-05-16 16:10:47.000000 pytest_aws_apigateway-0.6.0/tests/test_apigateway.py
--rw-r--r--   0 runner    (1001) docker     (127)      448 2024-05-16 16:10:47.000000 pytest_aws_apigateway-0.6.0/tests/test_integration.py
--rw-r--r--   0 runner    (1001) docker     (127)      777 2024-05-16 16:10:47.000000 pytest_aws_apigateway-0.6.0/tests/test_plugin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1200 2024-05-16 16:10:47.000000 pytest_aws_apigateway-0.6.0/tests/test_powertools.py
--rw-r--r--   0 runner    (1001) docker     (127)      267 2024-05-16 16:10:47.000000 pytest_aws_apigateway-0.6.0/tests/test_response.py
--rw-r--r--   0 runner    (1001) docker     (127)      393 2024-05-16 16:10:47.000000 pytest_aws_apigateway-0.6.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 10:15:31.580045 pytest_aws_apigateway-0.7.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 10:15:31.572045 pytest_aws_apigateway-0.7.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 10:15:31.576045 pytest_aws_apigateway-0.7.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1284 2024-05-18 10:15:21.000000 pytest_aws_apigateway-0.7.0/.github/workflows/main.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-18 10:15:21.000000 pytest_aws_apigateway-0.7.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      335 2024-05-18 10:15:21.000000 pytest_aws_apigateway-0.7.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1000 2024-05-18 10:15:21.000000 pytest_aws_apigateway-0.7.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-05-18 10:15:21.000000 pytest_aws_apigateway-0.7.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3547 2024-05-18 10:15:31.580045 pytest_aws_apigateway-0.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1342 2024-05-18 10:15:21.000000 pytest_aws_apigateway-0.7.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 10:15:31.576045 pytest_aws_apigateway-0.7.0/changes/
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-05-18 10:15:21.000000 pytest_aws_apigateway-0.7.0/changes/+.fix.md
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-18 10:15:21.000000 pytest_aws_apigateway-0.7.0/changes/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1384 2024-05-18 10:15:21.000000 pytest_aws_apigateway-0.7.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-18 10:15:21.000000 pytest_aws_apigateway-0.7.0/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-18 10:15:21.000000 pytest_aws_apigateway-0.7.0/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-18 10:15:31.580045 pytest_aws_apigateway-0.7.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 10:15:31.572045 pytest_aws_apigateway-0.7.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 10:15:31.576045 pytest_aws_apigateway-0.7.0/src/pytest_aws_apigateway/
+-rw-r--r--   0 runner    (1001) docker     (127)      236 2024-05-18 10:15:21.000000 pytest_aws_apigateway-0.7.0/src/pytest_aws_apigateway/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3871 2024-05-18 10:15:21.000000 pytest_aws_apigateway-0.7.0/src/pytest_aws_apigateway/apigateway.py
+-rw-r--r--   0 runner    (1001) docker     (127)      919 2024-05-18 10:15:21.000000 pytest_aws_apigateway-0.7.0/src/pytest_aws_apigateway/context.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2229 2024-05-18 10:15:21.000000 pytest_aws_apigateway-0.7.0/src/pytest_aws_apigateway/integration.py
+-rw-r--r--   0 runner    (1001) docker     (127)      217 2024-05-18 10:15:21.000000 pytest_aws_apigateway-0.7.0/src/pytest_aws_apigateway/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 10:15:31.580045 pytest_aws_apigateway-0.7.0/src/pytest_aws_apigateway.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3547 2024-05-18 10:15:31.000000 pytest_aws_apigateway-0.7.0/src/pytest_aws_apigateway.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      844 2024-05-18 10:15:31.000000 pytest_aws_apigateway-0.7.0/src/pytest_aws_apigateway.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-18 10:15:31.000000 pytest_aws_apigateway-0.7.0/src/pytest_aws_apigateway.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-05-18 10:15:31.000000 pytest_aws_apigateway-0.7.0/src/pytest_aws_apigateway.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-18 10:15:31.000000 pytest_aws_apigateway-0.7.0/src/pytest_aws_apigateway.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-18 10:15:31.000000 pytest_aws_apigateway-0.7.0/src/pytest_aws_apigateway.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 10:15:31.576045 pytest_aws_apigateway-0.7.0/tasks/
+-rw-r--r--   0 runner    (1001) docker     (127)     3213 2024-05-18 10:15:21.000000 pytest_aws_apigateway-0.7.0/tasks/release.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 10:15:31.580045 pytest_aws_apigateway-0.7.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-18 10:15:21.000000 pytest_aws_apigateway-0.7.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-18 10:15:21.000000 pytest_aws_apigateway-0.7.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5406 2024-05-18 10:15:21.000000 pytest_aws_apigateway-0.7.0/tests/test_apigateway.py
+-rw-r--r--   0 runner    (1001) docker     (127)      448 2024-05-18 10:15:21.000000 pytest_aws_apigateway-0.7.0/tests/test_integration.py
+-rw-r--r--   0 runner    (1001) docker     (127)      777 2024-05-18 10:15:21.000000 pytest_aws_apigateway-0.7.0/tests/test_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1200 2024-05-18 10:15:21.000000 pytest_aws_apigateway-0.7.0/tests/test_powertools.py
+-rw-r--r--   0 runner    (1001) docker     (127)      267 2024-05-18 10:15:21.000000 pytest_aws_apigateway-0.7.0/tests/test_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)      393 2024-05-18 10:15:21.000000 pytest_aws_apigateway-0.7.0/tox.ini
```

### Comparing `pytest_aws_apigateway-0.6.0/.github/workflows/main.yml` & `pytest_aws_apigateway-0.7.0/.github/workflows/main.yml`

 * *Files identical despite different names*

### Comparing `pytest_aws_apigateway-0.6.0/CHANGELOG.md` & `pytest_aws_apigateway-0.7.0/CHANGELOG.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,7 +1,14 @@
+# pytest-aws-apigateway 0.7.0 (2024-05-18)
+
+### Features
+
+- Can now pass in a custom lambda context.
+
+
 # pytest-aws-apigateway 0.6.0 (2024-05-16)
 
 No significant changes.
 
 
 # pytest-aws-apigateway 0.5.1 (2024-05-16)
```

### Comparing `pytest_aws_apigateway-0.6.0/LICENSE` & `pytest_aws_apigateway-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pytest_aws_apigateway-0.6.0/PKG-INFO` & `pytest_aws_apigateway-0.7.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-aws-apigateway
-Version: 0.6.0
+Version: 0.7.0
 Summary: pytest plugin for AWS ApiGateway
 Author-email: Felix Scherz <felixwscherz@gmail.com>
 License: MIT License
         
         Copyright (c) 2024-present Felix Scherz <felixwscherz@gmail.com>
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
```

### Comparing `pytest_aws_apigateway-0.6.0/README.md` & `pytest_aws_apigateway-0.7.0/README.md`

 * *Files identical despite different names*

### Comparing `pytest_aws_apigateway-0.6.0/pyproject.toml` & `pytest_aws_apigateway-0.7.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pytest_aws_apigateway-0.6.0/src/pytest_aws_apigateway/integration.py` & `pytest_aws_apigateway-0.7.0/src/pytest_aws_apigateway/integration.py`

 * *Files identical despite different names*

### Comparing `pytest_aws_apigateway-0.6.0/src/pytest_aws_apigateway.egg-info/PKG-INFO` & `pytest_aws_apigateway-0.7.0/src/pytest_aws_apigateway.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-aws-apigateway
-Version: 0.6.0
+Version: 0.7.0
 Summary: pytest plugin for AWS ApiGateway
 Author-email: Felix Scherz <felixwscherz@gmail.com>
 License: MIT License
         
         Copyright (c) 2024-present Felix Scherz <felixwscherz@gmail.com>
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
```

### Comparing `pytest_aws_apigateway-0.6.0/src/pytest_aws_apigateway.egg-info/SOURCES.txt` & `pytest_aws_apigateway-0.7.0/src/pytest_aws_apigateway.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pytest_aws_apigateway-0.6.0/tasks/release.py` & `pytest_aws_apigateway-0.7.0/tasks/release.py`

 * *Files identical despite different names*

### Comparing `pytest_aws_apigateway-0.6.0/tests/test_plugin.py` & `pytest_aws_apigateway-0.7.0/tests/test_plugin.py`

 * *Files identical despite different names*

### Comparing `pytest_aws_apigateway-0.6.0/tests/test_powertools.py` & `pytest_aws_apigateway-0.7.0/tests/test_powertools.py`

 * *Files identical despite different names*

