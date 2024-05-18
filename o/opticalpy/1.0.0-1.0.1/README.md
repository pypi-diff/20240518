# Comparing `tmp/opticalpy-1.0.0.tar.gz` & `tmp/opticalpy-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "opticalpy-1.0.0.tar", last modified: Sat May 18 08:53:13 2024, max compression
+gzip compressed data, was "opticalpy-1.0.1.tar", last modified: Sat May 18 09:00:16 2024, max compression
```

## Comparing `opticalpy-1.0.0.tar` & `opticalpy-1.0.1.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxrwx   0        0        0        0 2024-05-18 08:53:12.000000 opticalpy-1.0.0/
--rw-rw-rw-   0        0        0    35823 2024-05-18 07:43:32.000000 opticalpy-1.0.0/LICENSE
--rw-rw-rw-   0        0        0    44148 2024-05-18 08:53:13.000000 opticalpy-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     2277 2024-05-18 08:53:00.000000 opticalpy-1.0.0/README.md
--rw-rw-rw-   0        0        0      719 2024-05-18 08:49:39.000000 opticalpy-1.0.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-18 08:53:13.000000 opticalpy-1.0.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-05-18 08:53:12.000000 opticalpy-1.0.0/src/
-drwxrwxrwx   0        0        0        0 2024-05-18 08:53:12.000000 opticalpy-1.0.0/src/opticalpy/
--rw-rw-rw-   0        0        0      190 2024-05-18 08:33:11.000000 opticalpy-1.0.0/src/opticalpy/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-18 08:53:12.000000 opticalpy-1.0.0/src/opticalpy/elems/
--rw-rw-rw-   0        0        0      644 2024-05-18 08:19:58.000000 opticalpy-1.0.0/src/opticalpy/elems/__init__.py
--rw-rw-rw-   0        0        0     4311 2024-05-18 08:43:55.000000 opticalpy-1.0.0/src/opticalpy/elems/beam.py
--rw-rw-rw-   0        0        0     3751 2024-05-18 08:40:50.000000 opticalpy-1.0.0/src/opticalpy/elems/grating.py
--rw-rw-rw-   0        0        0    12887 2024-05-18 08:34:25.000000 opticalpy-1.0.0/src/opticalpy/elems/lens.py
--rw-rw-rw-   0        0        0     2158 2024-05-18 08:01:04.000000 opticalpy-1.0.0/src/opticalpy/elems/material.py
--rw-rw-rw-   0        0        0     7303 2024-05-18 08:34:43.000000 opticalpy-1.0.0/src/opticalpy/elems/mirror.py
--rw-rw-rw-   0        0        0     2749 2024-05-18 08:34:53.000000 opticalpy-1.0.0/src/opticalpy/elems/telescope.py
--rw-rw-rw-   0        0        0     2818 2024-05-18 08:40:00.000000 opticalpy-1.0.0/src/opticalpy/optgroup.py
--rw-rw-rw-   0        0        0     3329 2024-05-18 07:56:43.000000 opticalpy-1.0.0/src/opticalpy/optic.py
--rw-rw-rw-   0        0        0     4867 2024-05-18 08:08:09.000000 opticalpy-1.0.0/src/opticalpy/ray.py
--rw-rw-rw-   0        0        0     1568 2024-05-18 08:39:13.000000 opticalpy-1.0.0/src/opticalpy/scene.py
--rw-rw-rw-   0        0        0     1285 2024-05-18 07:50:30.000000 opticalpy-1.0.0/src/opticalpy/utils.py
--rw-rw-rw-   0        0        0     1139 2024-05-18 08:29:09.000000 opticalpy-1.0.0/src/opticalpy/visualization.py
-drwxrwxrwx   0        0        0        0 2024-05-18 08:53:12.000000 opticalpy-1.0.0/src/opticalpy.egg-info/
--rw-rw-rw-   0        0        0    44148 2024-05-18 08:53:12.000000 opticalpy-1.0.0/src/opticalpy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      603 2024-05-18 08:53:12.000000 opticalpy-1.0.0/src/opticalpy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-18 08:53:12.000000 opticalpy-1.0.0/src/opticalpy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       34 2024-05-18 08:53:12.000000 opticalpy-1.0.0/src/opticalpy.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-05-18 08:53:12.000000 opticalpy-1.0.0/src/opticalpy.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-18 09:00:16.000000 opticalpy-1.0.1/
+-rw-rw-rw-   0        0        0    35823 2024-05-18 07:43:32.000000 opticalpy-1.0.1/LICENSE
+-rw-rw-rw-   0        0        0    44369 2024-05-18 09:00:16.000000 opticalpy-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0     2498 2024-05-18 08:59:30.000000 opticalpy-1.0.1/README.md
+-rw-rw-rw-   0        0        0      719 2024-05-18 08:59:47.000000 opticalpy-1.0.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-18 09:00:16.000000 opticalpy-1.0.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-18 09:00:16.000000 opticalpy-1.0.1/src/
+drwxrwxrwx   0        0        0        0 2024-05-18 09:00:16.000000 opticalpy-1.0.1/src/opticalpy/
+-rw-rw-rw-   0        0        0      190 2024-05-18 08:33:11.000000 opticalpy-1.0.1/src/opticalpy/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-18 09:00:16.000000 opticalpy-1.0.1/src/opticalpy/elems/
+-rw-rw-rw-   0        0        0      644 2024-05-18 08:19:58.000000 opticalpy-1.0.1/src/opticalpy/elems/__init__.py
+-rw-rw-rw-   0        0        0     4311 2024-05-18 08:43:55.000000 opticalpy-1.0.1/src/opticalpy/elems/beam.py
+-rw-rw-rw-   0        0        0     3751 2024-05-18 08:40:50.000000 opticalpy-1.0.1/src/opticalpy/elems/grating.py
+-rw-rw-rw-   0        0        0    12887 2024-05-18 08:34:25.000000 opticalpy-1.0.1/src/opticalpy/elems/lens.py
+-rw-rw-rw-   0        0        0     2158 2024-05-18 08:01:04.000000 opticalpy-1.0.1/src/opticalpy/elems/material.py
+-rw-rw-rw-   0        0        0     7303 2024-05-18 08:34:43.000000 opticalpy-1.0.1/src/opticalpy/elems/mirror.py
+-rw-rw-rw-   0        0        0     2749 2024-05-18 08:34:53.000000 opticalpy-1.0.1/src/opticalpy/elems/telescope.py
+-rw-rw-rw-   0        0        0     2818 2024-05-18 08:40:00.000000 opticalpy-1.0.1/src/opticalpy/optgroup.py
+-rw-rw-rw-   0        0        0     3329 2024-05-18 07:56:43.000000 opticalpy-1.0.1/src/opticalpy/optic.py
+-rw-rw-rw-   0        0        0     4867 2024-05-18 08:08:09.000000 opticalpy-1.0.1/src/opticalpy/ray.py
+-rw-rw-rw-   0        0        0     1568 2024-05-18 08:39:13.000000 opticalpy-1.0.1/src/opticalpy/scene.py
+-rw-rw-rw-   0        0        0     1285 2024-05-18 07:50:30.000000 opticalpy-1.0.1/src/opticalpy/utils.py
+-rw-rw-rw-   0        0        0     1139 2024-05-18 08:29:09.000000 opticalpy-1.0.1/src/opticalpy/visualization.py
+drwxrwxrwx   0        0        0        0 2024-05-18 09:00:16.000000 opticalpy-1.0.1/src/opticalpy.egg-info/
+-rw-rw-rw-   0        0        0    44369 2024-05-18 09:00:16.000000 opticalpy-1.0.1/src/opticalpy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      603 2024-05-18 09:00:16.000000 opticalpy-1.0.1/src/opticalpy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-18 09:00:16.000000 opticalpy-1.0.1/src/opticalpy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       34 2024-05-18 09:00:16.000000 opticalpy-1.0.1/src/opticalpy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-05-18 09:00:16.000000 opticalpy-1.0.1/src/opticalpy.egg-info/top_level.txt
```

### Comparing `opticalpy-1.0.0/LICENSE` & `opticalpy-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `opticalpy-1.0.0/PKG-INFO` & `opticalpy-1.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opticalpy
-Version: 1.0.0
+Version: 1.0.1
 Summary: Exact geometrical optics including dispersion to learn and design optical instruments
 Author-email: Aurélien Genin <aurelien.genin@polytechnique.org>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -686,15 +686,17 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: autograd
 Requires-Dist: matplotlib
 Requires-Dist: astropy
 Requires-Dist: scipy
 
-# Optical raytracing in Python
+# Opticalpy - Optical raytracing in Python
+
+[![PyPI - Version](https://img.shields.io/pypi/v/opticalpy)](https://pypi.org/project/opticalpy/)
 
 This package in the making offers the possibility to **create optical setup** and **visualize the light rays going through it**.
 
 It originated as a way to better understand how instruments in astronomy worked, and allow to design them for amateur scientific endeavours. However, this package can be used in very different fields !
 
 ![Czerny-Turner spectrograph](images/Czerny-Turner%20spectrograph.png)
 
@@ -702,14 +704,20 @@
 
 1. It allows for modeling setup that use **dispersive elements** (gratings, prism, *grism*), and soon will also take dispersion in lenses into account.
 
 2. The optical elements geometry are **described by parameterized curves** allowing for exact interaction bewteen light rays and optical elements. This gives way better results than using discretized elements. To make this easy to use, each optical element is defined by one set of equations, that are automatically modified to place it where and in the orientation you want. The most common optical elements are already implemented, but you can add whatever you want with the method !
 
 ![Cassegrain telescope](images/Cassegrain.png)
 
+## Installation
+
+This package can be very easily installed using pip :
+
+ ```pip install opticalpy```
+
 ## Optical elements
 
 This package integrates the following optical elements. The elements in *italic* aren't developed yet but should be added soon.
 
 * **Mirror**:
     * Flat
     * Parabolic
```

### Comparing `opticalpy-1.0.0/README.md` & `opticalpy-1.0.1/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,10 @@
-# Optical raytracing in Python
+# Opticalpy - Optical raytracing in Python
+
+[![PyPI - Version](https://img.shields.io/pypi/v/opticalpy)](https://pypi.org/project/opticalpy/)
 
 This package in the making offers the possibility to **create optical setup** and **visualize the light rays going through it**.
 
 It originated as a way to better understand how instruments in astronomy worked, and allow to design them for amateur scientific endeavours. However, this package can be used in very different fields !
 
 ![Czerny-Turner spectrograph](images/Czerny-Turner%20spectrograph.png)
 
@@ -10,14 +12,20 @@
 
 1. It allows for modeling setup that use **dispersive elements** (gratings, prism, *grism*), and soon will also take dispersion in lenses into account.
 
 2. The optical elements geometry are **described by parameterized curves** allowing for exact interaction bewteen light rays and optical elements. This gives way better results than using discretized elements. To make this easy to use, each optical element is defined by one set of equations, that are automatically modified to place it where and in the orientation you want. The most common optical elements are already implemented, but you can add whatever you want with the method !
 
 ![Cassegrain telescope](images/Cassegrain.png)
 
+## Installation
+
+This package can be very easily installed using pip :
+
+ ```pip install opticalpy```
+
 ## Optical elements
 
 This package integrates the following optical elements. The elements in *italic* aren't developed yet but should be added soon.
 
 * **Mirror**:
     * Flat
     * Parabolic
```

### Comparing `opticalpy-1.0.0/pyproject.toml` & `opticalpy-1.0.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "opticalpy"
-version = "1.0.0"
+version = "1.0.1"
 authors = [
     {name="Aurélien Genin", email="aurelien.genin@polytechnique.org"}
 ]
 description = "Exact geometrical optics including dispersion to learn and design optical instruments"
 readme = "README.md"
 license = {file = "LICENSE"}
 requires-python = ">=3.10"
```

### Comparing `opticalpy-1.0.0/src/opticalpy/elems/__init__.py` & `opticalpy-1.0.1/src/opticalpy/elems/__init__.py`

 * *Files identical despite different names*

### Comparing `opticalpy-1.0.0/src/opticalpy/elems/beam.py` & `opticalpy-1.0.1/src/opticalpy/elems/beam.py`

 * *Files identical despite different names*

### Comparing `opticalpy-1.0.0/src/opticalpy/elems/grating.py` & `opticalpy-1.0.1/src/opticalpy/elems/grating.py`

 * *Files identical despite different names*

### Comparing `opticalpy-1.0.0/src/opticalpy/elems/lens.py` & `opticalpy-1.0.1/src/opticalpy/elems/lens.py`

 * *Files identical despite different names*

### Comparing `opticalpy-1.0.0/src/opticalpy/elems/material.py` & `opticalpy-1.0.1/src/opticalpy/elems/material.py`

 * *Files identical despite different names*

### Comparing `opticalpy-1.0.0/src/opticalpy/elems/mirror.py` & `opticalpy-1.0.1/src/opticalpy/elems/mirror.py`

 * *Files identical despite different names*

### Comparing `opticalpy-1.0.0/src/opticalpy/elems/telescope.py` & `opticalpy-1.0.1/src/opticalpy/elems/telescope.py`

 * *Files identical despite different names*

### Comparing `opticalpy-1.0.0/src/opticalpy/optgroup.py` & `opticalpy-1.0.1/src/opticalpy/optgroup.py`

 * *Files identical despite different names*

### Comparing `opticalpy-1.0.0/src/opticalpy/optic.py` & `opticalpy-1.0.1/src/opticalpy/optic.py`

 * *Files identical despite different names*

### Comparing `opticalpy-1.0.0/src/opticalpy/ray.py` & `opticalpy-1.0.1/src/opticalpy/ray.py`

 * *Files identical despite different names*

### Comparing `opticalpy-1.0.0/src/opticalpy/scene.py` & `opticalpy-1.0.1/src/opticalpy/scene.py`

 * *Files identical despite different names*

### Comparing `opticalpy-1.0.0/src/opticalpy/utils.py` & `opticalpy-1.0.1/src/opticalpy/utils.py`

 * *Files identical despite different names*

### Comparing `opticalpy-1.0.0/src/opticalpy/visualization.py` & `opticalpy-1.0.1/src/opticalpy/visualization.py`

 * *Files identical despite different names*

### Comparing `opticalpy-1.0.0/src/opticalpy.egg-info/PKG-INFO` & `opticalpy-1.0.1/src/opticalpy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opticalpy
-Version: 1.0.0
+Version: 1.0.1
 Summary: Exact geometrical optics including dispersion to learn and design optical instruments
 Author-email: Aurélien Genin <aurelien.genin@polytechnique.org>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -686,15 +686,17 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: autograd
 Requires-Dist: matplotlib
 Requires-Dist: astropy
 Requires-Dist: scipy
 
-# Optical raytracing in Python
+# Opticalpy - Optical raytracing in Python
+
+[![PyPI - Version](https://img.shields.io/pypi/v/opticalpy)](https://pypi.org/project/opticalpy/)
 
 This package in the making offers the possibility to **create optical setup** and **visualize the light rays going through it**.
 
 It originated as a way to better understand how instruments in astronomy worked, and allow to design them for amateur scientific endeavours. However, this package can be used in very different fields !
 
 ![Czerny-Turner spectrograph](images/Czerny-Turner%20spectrograph.png)
 
@@ -702,14 +704,20 @@
 
 1. It allows for modeling setup that use **dispersive elements** (gratings, prism, *grism*), and soon will also take dispersion in lenses into account.
 
 2. The optical elements geometry are **described by parameterized curves** allowing for exact interaction bewteen light rays and optical elements. This gives way better results than using discretized elements. To make this easy to use, each optical element is defined by one set of equations, that are automatically modified to place it where and in the orientation you want. The most common optical elements are already implemented, but you can add whatever you want with the method !
 
 ![Cassegrain telescope](images/Cassegrain.png)
 
+## Installation
+
+This package can be very easily installed using pip :
+
+ ```pip install opticalpy```
+
 ## Optical elements
 
 This package integrates the following optical elements. The elements in *italic* aren't developed yet but should be added soon.
 
 * **Mirror**:
     * Flat
     * Parabolic
```

### Comparing `opticalpy-1.0.0/src/opticalpy.egg-info/SOURCES.txt` & `opticalpy-1.0.1/src/opticalpy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

