# Comparing `tmp/smartpasslib-0.4.0.tar.gz` & `tmp/smartpasslib-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "smartpasslib-0.4.0.tar", last modified: Wed May 15 05:36:18 2024, max compression
+gzip compressed data, was "smartpasslib-0.4.1.tar", last modified: Sat May 18 07:47:44 2024, max compression
```

## Comparing `smartpasslib-0.4.0.tar` & `smartpasslib-0.4.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 smart     (1000) smart     (1000)        0 2024-05-15 05:36:18.067734 smartpasslib-0.4.0/
--rw-r--r--   0 smart     (1000) smart     (1000)     1498 2024-05-08 07:36:51.000000 smartpasslib-0.4.0/LICENSE
--rw-r--r--   0 smart     (1000) smart     (1000)      109 2024-05-08 07:50:33.000000 smartpasslib-0.4.0/MANIFEST.in
--rw-r--r--   0 smart     (1000) smart     (1000)     3868 2024-05-15 05:36:18.067734 smartpasslib-0.4.0/PKG-INFO
--rw-r--r--   0 smart     (1000) smart     (1000)     2635 2024-05-15 05:35:24.000000 smartpasslib-0.4.0/README.md
--rw-r--r--   0 smart     (1000) smart     (1000)       18 2024-05-15 05:13:20.000000 smartpasslib-0.4.0/requirements.txt
--rw-r--r--   0 smart     (1000) smart     (1000)     1271 2024-05-15 05:36:18.071068 smartpasslib-0.4.0/setup.cfg
--rw-r--r--   0 smart     (1000) smart     (1000)      387 2024-05-08 07:55:29.000000 smartpasslib-0.4.0/setup.py
-drwxr-xr-x   0 smart     (1000) smart     (1000)        0 2024-05-15 05:36:18.067734 smartpasslib-0.4.0/smartpasslib/
--rw-r--r--   0 smart     (1000) smart     (1000)      371 2024-05-15 05:35:24.000000 smartpasslib-0.4.0/smartpasslib/__init__.py
--rw-r--r--   0 smart     (1000) smart     (1000)     2839 2024-05-15 05:33:08.000000 smartpasslib-0.4.0/smartpasslib/generators.py
-drwxr-xr-x   0 smart     (1000) smart     (1000)        0 2024-05-15 05:36:18.067734 smartpasslib-0.4.0/smartpasslib.egg-info/
--rw-r--r--   0 smart     (1000) smart     (1000)     3868 2024-05-15 05:36:18.000000 smartpasslib-0.4.0/smartpasslib.egg-info/PKG-INFO
--rw-r--r--   0 smart     (1000) smart     (1000)      339 2024-05-15 05:36:18.000000 smartpasslib-0.4.0/smartpasslib.egg-info/SOURCES.txt
--rw-r--r--   0 smart     (1000) smart     (1000)        1 2024-05-15 05:36:18.000000 smartpasslib-0.4.0/smartpasslib.egg-info/dependency_links.txt
--rw-r--r--   0 smart     (1000) smart     (1000)        1 2024-05-15 05:36:18.000000 smartpasslib-0.4.0/smartpasslib.egg-info/not-zip-safe
--rw-r--r--   0 smart     (1000) smart     (1000)       19 2024-05-15 05:36:18.000000 smartpasslib-0.4.0/smartpasslib.egg-info/requires.txt
--rw-r--r--   0 smart     (1000) smart     (1000)       13 2024-05-15 05:36:18.000000 smartpasslib-0.4.0/smartpasslib.egg-info/top_level.txt
--rw-r--r--   0 smart     (1000) smart     (1000)      103 2024-05-08 07:56:03.000000 smartpasslib-0.4.0/tox.ini
+drwxr-xr-x   0 smart     (1000) smart     (1000)        0 2024-05-18 07:47:44.565972 smartpasslib-0.4.1/
+-rw-r--r--   0 smart     (1000) smart     (1000)     1498 2024-05-18 07:36:22.000000 smartpasslib-0.4.1/LICENSE
+-rw-r--r--   0 smart     (1000) smart     (1000)      139 2024-05-18 07:46:48.000000 smartpasslib-0.4.1/MANIFEST.in
+-rw-r--r--   0 smart     (1000) smart     (1000)     3832 2024-05-18 07:47:44.565972 smartpasslib-0.4.1/PKG-INFO
+-rw-r--r--   0 smart     (1000) smart     (1000)     2599 2024-05-18 07:44:43.000000 smartpasslib-0.4.1/README.md
+-rw-r--r--   0 smart     (1000) smart     (1000)       18 2024-05-18 07:38:01.000000 smartpasslib-0.4.1/requirements.txt
+-rw-r--r--   0 smart     (1000) smart     (1000)     1271 2024-05-18 07:47:44.569306 smartpasslib-0.4.1/setup.cfg
+-rw-r--r--   0 smart     (1000) smart     (1000)      387 2024-05-18 07:36:22.000000 smartpasslib-0.4.1/setup.py
+drwxr-xr-x   0 smart     (1000) smart     (1000)        0 2024-05-18 07:47:44.562639 smartpasslib-0.4.1/smartpasslib/
+-rw-r--r--   0 smart     (1000) smart     (1000)      371 2024-05-18 07:38:01.000000 smartpasslib-0.4.1/smartpasslib/__init__.py
+-rw-r--r--   0 smart     (1000) smart     (1000)     2866 2024-05-18 07:44:43.000000 smartpasslib-0.4.1/smartpasslib/generators.py
+drwxr-xr-x   0 smart     (1000) smart     (1000)        0 2024-05-18 07:47:44.565972 smartpasslib-0.4.1/smartpasslib.egg-info/
+-rw-r--r--   0 smart     (1000) smart     (1000)     3832 2024-05-18 07:47:44.000000 smartpasslib-0.4.1/smartpasslib.egg-info/PKG-INFO
+-rw-r--r--   0 smart     (1000) smart     (1000)      339 2024-05-18 07:47:44.000000 smartpasslib-0.4.1/smartpasslib.egg-info/SOURCES.txt
+-rw-r--r--   0 smart     (1000) smart     (1000)        1 2024-05-18 07:47:44.000000 smartpasslib-0.4.1/smartpasslib.egg-info/dependency_links.txt
+-rw-r--r--   0 smart     (1000) smart     (1000)        1 2024-05-18 07:47:44.000000 smartpasslib-0.4.1/smartpasslib.egg-info/not-zip-safe
+-rw-r--r--   0 smart     (1000) smart     (1000)       19 2024-05-18 07:47:44.000000 smartpasslib-0.4.1/smartpasslib.egg-info/requires.txt
+-rw-r--r--   0 smart     (1000) smart     (1000)       13 2024-05-18 07:47:44.000000 smartpasslib-0.4.1/smartpasslib.egg-info/top_level.txt
+-rw-r--r--   0 smart     (1000) smart     (1000)      103 2024-05-18 07:36:22.000000 smartpasslib-0.4.1/tox.ini
```

### Comparing `smartpasslib-0.4.0/LICENSE` & `smartpasslib-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `smartpasslib-0.4.0/PKG-INFO` & `smartpasslib-0.4.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smartpasslib
-Version: 0.4.0
+Version: 0.4.1
 Summary: 'Cross-platform library for generating smart passwords.'
 Home-page: https://github.com/smartlegionlab
 Author: A.A Suvorov
 Author-email: smartlegiondev@gmail.com
 License: BSD 3-Clause License
 Project-URL: Documentation, https://github.com/smartlegionlab/smartpasslib/blob/master/README.md
 Project-URL: Release notes, https://github.com/smartlegionlab/smartpasslib/releases
@@ -20,17 +20,17 @@
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Utilities
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: smartrandom~=0.1.0
+Requires-Dist: smartrandom~=0.1.1
 
-# Smart Passwords Library
+# Smart Passwords Library <sup>v0.4.1</sup>
 
 ***
 
 [![GitHub release (latest by date)](https://img.shields.io/github/v/release/smartlegionlab/smartpasslib)](https://github.com/smartlegionlab/smartpasslib/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/smartpasslib?label=pypi%20downloads)](https://pypi.org/project/smartpasslib/)
 ![GitHub top language](https://img.shields.io/github/languages/top/smartlegionlab/smartpasslib)
 [![PyPI](https://img.shields.io/pypi/v/smartpasslib)](https://pypi.org/project/smartpasslib)
@@ -49,20 +49,14 @@
 ***
 
 ## Supported:
 
 - Linux: All.
 - Windows: 7/8/10.
 - Termux (Android).
-  
-***
-
-## What's new?
-
-### ___smartpasslib v0.4.0___
 
 ***
 
 ## Requirements:
 
 [smartrandom](https://github.com/smartlegionlab/smartrandom/) - Random Data Generators.
```

### Comparing `smartpasslib-0.4.0/README.md` & `smartpasslib-0.4.1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Smart Passwords Library
+# Smart Passwords Library <sup>v0.4.1</sup>
 
 ***
 
 [![GitHub release (latest by date)](https://img.shields.io/github/v/release/smartlegionlab/smartpasslib)](https://github.com/smartlegionlab/smartpasslib/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/smartpasslib?label=pypi%20downloads)](https://pypi.org/project/smartpasslib/)
 ![GitHub top language](https://img.shields.io/github/languages/top/smartlegionlab/smartpasslib)
 [![PyPI](https://img.shields.io/pypi/v/smartpasslib)](https://pypi.org/project/smartpasslib)
@@ -21,20 +21,14 @@
 ***
 
 ## Supported:
 
 - Linux: All.
 - Windows: 7/8/10.
 - Termux (Android).
-  
-***
-
-## What's new?
-
-### ___smartpasslib v0.4.0___
 
 ***
 
 ## Requirements:
 
 [smartrandom](https://github.com/smartlegionlab/smartrandom/) - Random Data Generators.
```

### Comparing `smartpasslib-0.4.0/setup.cfg` & `smartpasslib-0.4.1/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -32,13 +32,13 @@
 
 [options]
 python_requires = >=3.6
 packages = find:
 include_package_data = true
 zip_safe = false
 install_requires = 
-	smartrandom~=0.1.0
+	smartrandom~=0.1.1
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `smartpasslib-0.4.0/smartpasslib/generators.py` & `smartpasslib-0.4.1/smartpasslib/generators.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,24 +1,17 @@
 # --------------------------------------------------------
 # Licensed under the terms of the BSD 3-Clause License
 # (see LICENSE for details).
 # Copyright © 2018-2024, A.A Suvorov
 # All rights reserved.
 # --------------------------------------------------------
 """Smart Random Generators"""
-import os
 import random
 
-from smartrandom.random_master import RandomStringMaster, HashMaster
-
-
-class UrandomGen:
-    @classmethod
-    def generate(cls, size=32):
-        return os.urandom(size)
+from smartrandom.random_master import RandomStringMaster, HashMaster, UrandomGen
 
 
 class SmartKeyGen:
     _hash_master = HashMaster()
 
     @classmethod
     def __make_key(cls, login='', secret='', public_step=15):
@@ -78,14 +71,17 @@
     key_gen = SmartKeyGen()
     smart_pass_gen = BaseSmartPassGen()
 
     @classmethod
     def get_password(cls, length=10):
         return cls.random_master.create_string(length)
 
+    def get_default_password(cls, secret='', length=10):
+        return cls.get_smart_password(secret=secret, length=length)
+
     @classmethod
     def get_smart_password(cls, login='', secret='', length=10):
         seed = cls.key_gen.get_private_key(login, secret)
         return cls.smart_pass_gen.generate(seed, length=length)
 
     @classmethod
     def get_public_key(cls, login='', secret=''):
```

### Comparing `smartpasslib-0.4.0/smartpasslib.egg-info/PKG-INFO` & `smartpasslib-0.4.1/smartpasslib.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smartpasslib
-Version: 0.4.0
+Version: 0.4.1
 Summary: 'Cross-platform library for generating smart passwords.'
 Home-page: https://github.com/smartlegionlab
 Author: A.A Suvorov
 Author-email: smartlegiondev@gmail.com
 License: BSD 3-Clause License
 Project-URL: Documentation, https://github.com/smartlegionlab/smartpasslib/blob/master/README.md
 Project-URL: Release notes, https://github.com/smartlegionlab/smartpasslib/releases
@@ -20,17 +20,17 @@
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Utilities
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: smartrandom~=0.1.0
+Requires-Dist: smartrandom~=0.1.1
 
-# Smart Passwords Library
+# Smart Passwords Library <sup>v0.4.1</sup>
 
 ***
 
 [![GitHub release (latest by date)](https://img.shields.io/github/v/release/smartlegionlab/smartpasslib)](https://github.com/smartlegionlab/smartpasslib/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/smartpasslib?label=pypi%20downloads)](https://pypi.org/project/smartpasslib/)
 ![GitHub top language](https://img.shields.io/github/languages/top/smartlegionlab/smartpasslib)
 [![PyPI](https://img.shields.io/pypi/v/smartpasslib)](https://pypi.org/project/smartpasslib)
@@ -49,20 +49,14 @@
 ***
 
 ## Supported:
 
 - Linux: All.
 - Windows: 7/8/10.
 - Termux (Android).
-  
-***
-
-## What's new?
-
-### ___smartpasslib v0.4.0___
 
 ***
 
 ## Requirements:
 
 [smartrandom](https://github.com/smartlegionlab/smartrandom/) - Random Data Generators.
```

