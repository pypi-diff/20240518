# Comparing `tmp/wrg-0.1.1rc1.tar.gz` & `tmp/wrg-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wrg-0.1.1rc1.tar", last modified: Sun Dec 10 21:24:29 2023, max compression
+gzip compressed data, was "wrg-0.1.2.tar", last modified: Fri May 17 22:49:25 2024, max compression
```

## Comparing `wrg-0.1.1rc1.tar` & `wrg-0.1.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 goyo      (1000) goyo      (1000)        0 2023-12-10 21:24:29.350779 wrg-0.1.1rc1/
--rw-rw-r--   0 goyo      (1000) goyo      (1000)    17988 2020-10-11 23:09:56.000000 wrg-0.1.1rc1/LICENSE.txt
--rw-rw-r--   0 goyo      (1000) goyo      (1000)       40 2020-10-11 23:09:56.000000 wrg-0.1.1rc1/MANIFEST.in
--rw-r--r--   0 goyo      (1000) goyo      (1000)      573 2023-12-10 21:24:29.350779 wrg-0.1.1rc1/PKG-INFO
--rw-rw-r--   0 goyo      (1000) goyo      (1000)        0 2020-10-11 23:10:14.000000 wrg-0.1.1rc1/README.txt
--rw-r--r--   0 goyo      (1000) goyo      (1000)      583 2023-12-10 21:24:29.350779 wrg-0.1.1rc1/setup.cfg
--rw-rw-r--   0 goyo      (1000) goyo      (1000)      907 2023-12-03 23:24:09.000000 wrg-0.1.1rc1/setup.py
-drwxr-xr-x   0 goyo      (1000) goyo      (1000)        0 2023-12-10 21:24:29.350779 wrg-0.1.1rc1/wrg.egg-info/
--rw-r--r--   0 goyo      (1000) goyo      (1000)      573 2023-12-10 21:24:29.000000 wrg-0.1.1rc1/wrg.egg-info/PKG-INFO
--rw-r--r--   0 goyo      (1000) goyo      (1000)      194 2023-12-10 21:24:29.000000 wrg-0.1.1rc1/wrg.egg-info/SOURCES.txt
--rw-r--r--   0 goyo      (1000) goyo      (1000)        1 2023-12-10 21:24:29.000000 wrg-0.1.1rc1/wrg.egg-info/dependency_links.txt
--rw-r--r--   0 goyo      (1000) goyo      (1000)       24 2023-12-10 21:24:29.000000 wrg-0.1.1rc1/wrg.egg-info/requires.txt
--rw-r--r--   0 goyo      (1000) goyo      (1000)        4 2023-12-10 21:24:29.000000 wrg-0.1.1rc1/wrg.egg-info/top_level.txt
--rw-rw-r--   0 goyo      (1000) goyo      (1000)     7665 2023-12-10 21:23:08.000000 wrg-0.1.1rc1/wrg.py
+drwxr-xr-x   0 goyo      (1000) goyo      (1000)        0 2024-05-17 22:49:25.967261 wrg-0.1.2/
+-rw-rw-r--   0 goyo      (1000) goyo      (1000)    17988 2020-10-11 23:09:56.000000 wrg-0.1.2/LICENSE.txt
+-rw-rw-r--   0 goyo      (1000) goyo      (1000)       40 2020-10-11 23:09:56.000000 wrg-0.1.2/MANIFEST.in
+-rw-r--r--   0 goyo      (1000) goyo      (1000)      568 2024-05-17 22:49:25.967261 wrg-0.1.2/PKG-INFO
+-rw-rw-r--   0 goyo      (1000) goyo      (1000)        0 2020-10-11 23:10:14.000000 wrg-0.1.2/README.txt
+-rw-r--r--   0 goyo      (1000) goyo      (1000)      579 2024-05-17 22:49:25.967261 wrg-0.1.2/setup.cfg
+-rw-rw-r--   0 goyo      (1000) goyo      (1000)      907 2023-12-03 23:24:09.000000 wrg-0.1.2/setup.py
+drwxr-xr-x   0 goyo      (1000) goyo      (1000)        0 2024-05-17 22:49:25.967261 wrg-0.1.2/wrg.egg-info/
+-rw-r--r--   0 goyo      (1000) goyo      (1000)      568 2024-05-17 22:49:25.000000 wrg-0.1.2/wrg.egg-info/PKG-INFO
+-rw-r--r--   0 goyo      (1000) goyo      (1000)      194 2024-05-17 22:49:25.000000 wrg-0.1.2/wrg.egg-info/SOURCES.txt
+-rw-r--r--   0 goyo      (1000) goyo      (1000)        1 2024-05-17 22:49:25.000000 wrg-0.1.2/wrg.egg-info/dependency_links.txt
+-rw-r--r--   0 goyo      (1000) goyo      (1000)       24 2024-05-17 22:49:25.000000 wrg-0.1.2/wrg.egg-info/requires.txt
+-rw-r--r--   0 goyo      (1000) goyo      (1000)        4 2024-05-17 22:49:25.000000 wrg-0.1.2/wrg.egg-info/top_level.txt
+-rw-rw-r--   0 goyo      (1000) goyo      (1000)     7661 2024-05-17 22:47:30.000000 wrg-0.1.2/wrg.py
```

### Comparing `wrg-0.1.1rc1/LICENSE.txt` & `wrg-0.1.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `wrg-0.1.1rc1/PKG-INFO` & `wrg-0.1.2/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: wrg
-Version: 0.1.1rc1
-Summary: Work with WRG files
+Version: 0.1.2
+Summary: Work with WRG files in python.
 Author: Goyo
 Author-email: goyodiaz@gmail.com
 License: OSI Approved :: GNU General Public License v2 or later (GPLv2+)
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Provides: wind
-Requires-Python: <3.13,>=3.9
+Classifier: Programming Language :: Python :: 3.13
+Requires-Python: <3.14,>=3.10
 License-File: LICENSE.txt
 Requires-Dist: numpy<2,>=1
 Requires-Dist: scipy<2,>=1
```

### Comparing `wrg-0.1.1rc1/setup.cfg` & `wrg-0.1.2/setup.cfg`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 [metadata]
 name = wrg
 version = attr: wrg.__version__
 author = Goyo
 author_email = goyodiaz@gmail.com
-description = Work with WRG files
-provides = wind,
+description = Work with WRG files in python.
 license = OSI Approved :: GNU General Public License v2 or later (GPLv2+)
 classifiers = 
 	Programming Language :: Python :: 3
-	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
 	Programming Language :: Python :: 3.11
 	Programming Language :: Python :: 3.12
+	Programming Language :: Python :: 3.13
 
 [options]
-python_requires = >=3.9, <3.13
+python_requires = >=3.10, <3.14
 install_requires = 
 	numpy>=1,<2
 	scipy>=1,<2
 py_modules = wrg,
 
 [egg_info]
 tag_build =
```

### Comparing `wrg-0.1.1rc1/setup.py` & `wrg-0.1.2/setup.py`

 * *Files identical despite different names*

### Comparing `wrg-0.1.1rc1/wrg.egg-info/PKG-INFO` & `wrg-0.1.2/wrg.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: wrg
-Version: 0.1.1rc1
-Summary: Work with WRG files
+Version: 0.1.2
+Summary: Work with WRG files in python.
 Author: Goyo
 Author-email: goyodiaz@gmail.com
 License: OSI Approved :: GNU General Public License v2 or later (GPLv2+)
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Provides: wind
-Requires-Python: <3.13,>=3.9
+Classifier: Programming Language :: Python :: 3.13
+Requires-Python: <3.14,>=3.10
 License-File: LICENSE.txt
 Requires-Dist: numpy<2,>=1
 Requires-Dist: scipy<2,>=1
```

### Comparing `wrg-0.1.1rc1/wrg.py` & `wrg-0.1.2/wrg.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8 -*-
 #
 # wrg.py
 #
-# Copyright 2017 - 2023 Goyo <goyodiaz@gmail.com>
+# Copyright 2017 - 2024 Goyo <goyodiaz@gmail.com>
 #
 # This program is free software; you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation; either version 2 of the License, or
 # (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful,
@@ -23,15 +23,15 @@
 """Module wrg"""
 
 import itertools
 
 import numpy as np
 from scipy.special import gamma
 
-__version__ = "0.1.1.rc1"
+__version__ = "0.1.2"
 
 
 # return (start, end) pairs from iterable of widths
 def _widths2slices(widths):
     cuts = itertools.accumulate(itertools.chain([0], widths))
     a, b = itertools.tee(cuts)
     return tuple(zip(a, itertools.islice(b, 1, None)))
```

