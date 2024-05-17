# Comparing `tmp/glidergun-0.5.5.tar.gz` & `tmp/glidergun-0.5.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "glidergun-0.5.5.tar", last modified: Fri May 17 02:44:31 2024, max compression
+gzip compressed data, was "glidergun-0.5.6.tar", last modified: Fri May 17 11:44:34 2024, max compression
```

## Comparing `glidergun-0.5.5.tar` & `glidergun-0.5.6.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2024-05-17 02:44:31.473601 glidergun-0.5.5/
--rw-rw-rw-   0        0        0     2832 2024-05-17 02:44:31.472300 glidergun-0.5.5/PKG-INFO
--rw-rw-rw-   0        0        0     2148 2024-04-24 03:01:21.000000 glidergun-0.5.5/README.md
-drwxrwxrwx   0        0        0        0 2024-05-17 02:44:31.442190 glidergun-0.5.5/glidergun/
--rw-rw-rw-   0        0        0      438 2024-05-17 02:12:31.000000 glidergun-0.5.5/glidergun/__init__.py
--rw-rw-rw-   0        0        0    50020 2024-05-17 02:12:30.000000 glidergun-0.5.5/glidergun/_grid.py
--rw-rw-rw-   0        0        0     4200 2024-05-17 02:40:30.000000 glidergun-0.5.5/glidergun/_ipython.py
--rw-rw-rw-   0        0        0     1783 2024-04-24 03:01:21.000000 glidergun-0.5.5/glidergun/_literals.py
--rw-rw-rw-   0        0        0    10367 2024-05-17 02:12:25.000000 glidergun-0.5.5/glidergun/_stack.py
-drwxrwxrwx   0        0        0        0 2024-05-17 02:44:31.471025 glidergun-0.5.5/glidergun.egg-info/
--rw-rw-rw-   0        0        0     2832 2024-05-17 02:44:31.000000 glidergun-0.5.5/glidergun.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      294 2024-05-17 02:44:31.000000 glidergun-0.5.5/glidergun.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-17 02:44:31.000000 glidergun-0.5.5/glidergun.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       68 2024-05-17 02:44:31.000000 glidergun-0.5.5/glidergun.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-05-17 02:44:31.000000 glidergun-0.5.5/glidergun.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      746 2024-05-17 02:36:03.000000 glidergun-0.5.5/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-17 02:44:31.474621 glidergun-0.5.5/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-17 11:44:34.257897 glidergun-0.5.6/
+-rw-rw-rw-   0        0        0     2832 2024-05-17 11:44:34.255452 glidergun-0.5.6/PKG-INFO
+-rw-rw-rw-   0        0        0     2148 2024-04-24 03:01:21.000000 glidergun-0.5.6/README.md
+drwxrwxrwx   0        0        0        0 2024-05-17 11:44:34.226870 glidergun-0.5.6/glidergun/
+-rw-rw-rw-   0        0        0      438 2024-05-17 02:12:31.000000 glidergun-0.5.6/glidergun/__init__.py
+-rw-rw-rw-   0        0        0    50020 2024-05-17 02:12:30.000000 glidergun-0.5.6/glidergun/_grid.py
+-rw-rw-rw-   0        0        0     4200 2024-05-17 11:42:12.000000 glidergun-0.5.6/glidergun/_ipython.py
+-rw-rw-rw-   0        0        0     1783 2024-04-24 03:01:21.000000 glidergun-0.5.6/glidergun/_literals.py
+-rw-rw-rw-   0        0        0    10367 2024-05-17 02:12:25.000000 glidergun-0.5.6/glidergun/_stack.py
+drwxrwxrwx   0        0        0        0 2024-05-17 11:44:34.255187 glidergun-0.5.6/glidergun.egg-info/
+-rw-rw-rw-   0        0        0     2832 2024-05-17 11:44:34.000000 glidergun-0.5.6/glidergun.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      294 2024-05-17 11:44:34.000000 glidergun-0.5.6/glidergun.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-17 11:44:34.000000 glidergun-0.5.6/glidergun.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       68 2024-05-17 11:44:34.000000 glidergun-0.5.6/glidergun.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-05-17 11:44:34.000000 glidergun-0.5.6/glidergun.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      746 2024-05-17 11:43:31.000000 glidergun-0.5.6/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-17 11:44:34.257897 glidergun-0.5.6/setup.cfg
```

### Comparing `glidergun-0.5.5/PKG-INFO` & `glidergun-0.5.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: glidergun
-Version: 0.5.5
+Version: 0.5.6
 Summary: Map Algebra with NumPy
 Author-email: Jiro Shirota <jshirota@gmail.com>
 Project-URL: Homepage, https://github.com/jshirota/glidergun
 Project-URL: Bug Tracker, https://github.com/jshirota/glidergun/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `glidergun-0.5.5/README.md` & `glidergun-0.5.6/README.md`

 * *Files identical despite different names*

### Comparing `glidergun-0.5.5/glidergun/_grid.py` & `glidergun-0.5.6/glidergun/_grid.py`

 * *Files identical despite different names*

### Comparing `glidergun-0.5.5/glidergun/_ipython.py` & `glidergun-0.5.6/glidergun/_ipython.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,25 +2,25 @@
 from io import BytesIO
 from typing import Optional, Union
 
 import IPython
 import matplotlib.pyplot as plt
 import numpy as np
 
-from glidergun._grid import Grid, Extent
+from glidergun._grid import Extent, Grid
 from glidergun._stack import Stack
 
 
 def _thumbnail(obj: Union[Grid, Stack], color, figsize=None):
     with BytesIO() as buffer:
         figure = plt.figure(figsize=figsize, frameon=False)
         axes = figure.add_axes((0, 0, 1, 1))
         axes.axis("off")
 
-        n = 2000 / max(obj.width, obj.height)
+        n = 4000 / max(obj.width, obj.height)
 
         if n < 1:
             obj = obj.resample(obj.cell_size / n)
 
         obj = obj.to_uint8_range()
 
         if isinstance(obj, Grid):
```

### Comparing `glidergun-0.5.5/glidergun/_literals.py` & `glidergun-0.5.6/glidergun/_literals.py`

 * *Files identical despite different names*

### Comparing `glidergun-0.5.5/glidergun/_stack.py` & `glidergun-0.5.6/glidergun/_stack.py`

 * *Files identical despite different names*

### Comparing `glidergun-0.5.5/glidergun.egg-info/PKG-INFO` & `glidergun-0.5.6/glidergun.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: glidergun
-Version: 0.5.5
+Version: 0.5.6
 Summary: Map Algebra with NumPy
 Author-email: Jiro Shirota <jshirota@gmail.com>
 Project-URL: Homepage, https://github.com/jshirota/glidergun
 Project-URL: Bug Tracker, https://github.com/jshirota/glidergun/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `glidergun-0.5.5/pyproject.toml` & `glidergun-0.5.6/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "glidergun"
-version = "0.5.5"
+version = "0.5.6"
 authors = [
   { name="Jiro Shirota", email="jshirota@gmail.com" },
 ]
 description = "Map Algebra with NumPy"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

