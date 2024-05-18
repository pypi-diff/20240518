# Comparing `tmp/coherent_build-0.7.0.tar.gz` & `tmp/coherent_build-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "coherent_build-0.7.0.tar", last modified: Sat May 18 18:26:52 2024, max compression
+gzip compressed data, was "coherent_build-0.8.0.tar", last modified: Sat May 18 18:46:43 2024, max compression
```

## Comparing `coherent_build-0.7.0.tar` & `coherent_build-0.8.0.tar`

### file list

```diff
@@ -1,10 +1,10 @@
-drwxr-xr-x   0 jaraco     (501) staff       (20)        0 2024-05-18 18:21:00.880212 coherent_build-0.7.0/
--rw-r--r--   0 jaraco     (501) staff       (20)       84 2024-05-05 14:27:21.911766 coherent_build-0.7.0/README.md
--rw-r--r--   0 jaraco     (501) staff       (20)      268 2024-05-18 18:04:29.832212 coherent_build-0.7.0/__init__.py
--rw-r--r--   0 jaraco     (501) staff       (20)     8550 2024-05-07 20:37:24.092828 coherent_build-0.7.0/__init__.py.orig
--rw-r--r--   0 jaraco     (501) staff       (20)      492 2024-05-09 19:24:41.199168 coherent_build-0.7.0/__main__.py
--rw-r--r--   0 jaraco     (501) staff       (20)     5482 2024-05-18 18:04:29.832430 coherent_build-0.7.0/backend.py
--rw-r--r--   0 jaraco     (501) staff       (20)     4363 2024-05-18 18:23:06.275278 coherent_build-0.7.0/discovery.py
--rw-r--r--   0 jaraco     (501) staff       (20)       78 2024-05-18 18:20:50.401743 coherent_build-0.7.0/pyproject.toml
--rw-r--r--   0 jaraco     (501) staff       (20)       78 2024-05-02 15:12:07.306572 coherent_build-0.7.0/system.toml
--rw-r--r--   0        0        0      611 2024-05-18 18:26:52.048515 coherent_build-0.7.0/PKG-INFO
+drwxr-xr-x   0 jaraco     (501) staff       (20)        0 2024-05-18 18:46:42.502695 coherent_build-0.8.0/
+-rw-r--r--   0 jaraco     (501) staff       (20)       84 2024-05-05 14:27:21.911766 coherent_build-0.8.0/README.md
+-rw-r--r--   0 jaraco     (501) staff       (20)      268 2024-05-18 18:04:29.832212 coherent_build-0.8.0/__init__.py
+-rw-r--r--   0 jaraco     (501) staff       (20)     8550 2024-05-07 20:37:24.092828 coherent_build-0.8.0/__init__.py.orig
+-rw-r--r--   0 jaraco     (501) staff       (20)      533 2024-05-18 18:41:00.726383 coherent_build-0.8.0/__main__.py
+-rw-r--r--   0 jaraco     (501) staff       (20)     5482 2024-05-18 18:04:29.832430 coherent_build-0.8.0/backend.py
+-rw-r--r--   0 jaraco     (501) staff       (20)     4436 2024-05-18 18:44:04.428362 coherent_build-0.8.0/discovery.py
+-rw-r--r--   0 jaraco     (501) staff       (20)       78 2024-05-18 18:46:42.502769 coherent_build-0.8.0/pyproject.toml
+-rw-r--r--   0 jaraco     (501) staff       (20)       78 2024-05-02 15:12:07.306572 coherent_build-0.8.0/system.toml
+-rw-r--r--   0        0        0      611 2024-05-18 18:46:43.826281 coherent_build-0.8.0/PKG-INFO
```

### Comparing `coherent_build-0.7.0/__init__.py.orig` & `coherent_build-0.8.0/__init__.py.orig`

 * *Files identical despite different names*

### Comparing `coherent_build-0.7.0/backend.py` & `coherent_build-0.8.0/backend.py`

 * *Files identical despite different names*

### Comparing `coherent_build-0.7.0/discovery.py` & `coherent_build-0.8.0/discovery.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,26 @@
 import contextlib
 import functools
 import json
+import logging
 import pathlib
 import subprocess
 import types
 import mimetypes
 from collections.abc import Mapping
 
 import jaraco.functools
 import requests
 import setuptools_scm
 from jaraco.context import suppress
 from pip_run import scripts
 
 
+log = logging.getLogger(__name__)
+
 mimetypes.add_type('text/plain', '', strict=True)
 mimetypes.add_type('text/markdown', '.md', strict=True)
 mimetypes.add_type('text/x-rst', '.rst', strict=True)
 
 
 @suppress(subprocess.CalledProcessError)
 def name_from_vcs():
@@ -99,17 +102,19 @@
     """
     owner = 'python'
     repo = 'cpython'
     url = f'https://api.github.com/repos/{owner}/{repo}/branches'
     branches = requests.get(url).json()
     # cheat and grab the first branch, which is the oldest supported Python version
     try:
-        return f'>= {branches[0]["name"]}'
-    except KeyError as err:
-        raise RuntimeError(f"Unexpected {branches=}") from err
+        min_ver = branches[0]["name"]
+    except KeyError:
+        log.warning(f"Unexpected {branches=}")
+        min_ver = "3.8"
+    return f'>= {min_ver}'
 
 
 def read_deps():
     """
     Read deps from ``__init__.py``.
     """
     return scripts.DepsReader.search(['__init__.py'])
```

### Comparing `coherent_build-0.7.0/PKG-INFO` & `coherent_build-0.8.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: coherent.build
-Version: 0.7.0
+Version: 0.8.0
 Author-Email: "Jason R. Coombs" <jaraco@jaraco.com>
 Summary: A zero-config Python project build backend
 Requires-Python: >= 3.8
 Requires-Dist: wheel
 Requires-Dist: pip-run
 Requires-Dist: setuptools_scm
 Requires-Dist: build
```

