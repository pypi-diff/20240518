# Comparing `tmp/numpytransforms-0.0.0.tar.gz` & `tmp/numpytransforms-0.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "numpytransforms-0.0.0.tar", last modified: Thu May 16 16:47:17 2024, max compression
+gzip compressed data, was "numpytransforms-0.0.1.tar", last modified: Sat May 18 21:38:02 2024, max compression
```

## Comparing `numpytransforms-0.0.0.tar` & `numpytransforms-0.0.1.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxrwxrwx   0        0        0        0 2024-05-16 16:47:17.293352 numpytransforms-0.0.0/
--rw-rw-rw-   0        0        0    35823 2022-09-12 17:26:44.000000 numpytransforms-0.0.0/LICENSE
--rw-rw-rw-   0        0        0    41676 2024-05-16 16:47:17.292353 numpytransforms-0.0.0/PKG-INFO
--rw-rw-rw-   0        0        0      476 2024-05-16 16:46:25.000000 numpytransforms-0.0.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-16 16:47:17.293352 numpytransforms-0.0.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-05-16 16:47:17.268353 numpytransforms-0.0.0/src/
-drwxrwxrwx   0        0        0        0 2024-05-16 16:47:17.271353 numpytransforms-0.0.0/src/NumpyTransforms/
--rw-rw-rw-   0        0        0     1838 2024-05-16 16:32:17.000000 numpytransforms-0.0.0/src/NumpyTransforms/Affine.py
--rw-rw-rw-   0        0        0     1375 2024-05-16 16:38:01.000000 numpytransforms-0.0.0/src/NumpyTransforms/Bezier.py
--rw-rw-rw-   0        0        0       69 2024-05-16 16:32:17.000000 numpytransforms-0.0.0/src/NumpyTransforms/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-16 16:47:17.289354 numpytransforms-0.0.0/src/NumpyTransforms.egg-info/
--rw-rw-rw-   0        0        0    41676 2024-05-16 16:47:17.000000 numpytransforms-0.0.0/src/NumpyTransforms.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      302 2024-05-16 16:47:17.000000 numpytransforms-0.0.0/src/NumpyTransforms.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-16 16:47:17.000000 numpytransforms-0.0.0/src/NumpyTransforms.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       25 2024-05-16 16:47:17.000000 numpytransforms-0.0.0/src/NumpyTransforms.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        0 2024-05-16 15:09:19.000000 numpytransforms-0.0.0/src/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-18 21:38:02.866344 numpytransforms-0.0.1/
+-rw-rw-rw-   0        0        0    35823 2022-09-12 17:26:44.000000 numpytransforms-0.0.1/LICENSE
+-rw-rw-rw-   0        0        0    41739 2024-05-18 21:38:02.865343 numpytransforms-0.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0       61 2024-05-16 16:59:24.000000 numpytransforms-0.0.1/README.md
+-rw-rw-rw-   0        0        0      476 2024-05-18 21:37:53.000000 numpytransforms-0.0.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-18 21:38:02.866344 numpytransforms-0.0.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-18 21:38:02.827343 numpytransforms-0.0.1/src/
+drwxrwxrwx   0        0        0        0 2024-05-18 21:38:02.845342 numpytransforms-0.0.1/src/NumpyTransforms/
+-rw-rw-rw-   0        0        0     1838 2024-05-16 16:32:17.000000 numpytransforms-0.0.1/src/NumpyTransforms/Affine.py
+-rw-rw-rw-   0        0        0     1375 2024-05-16 16:38:01.000000 numpytransforms-0.0.1/src/NumpyTransforms/Bezier.py
+-rw-rw-rw-   0        0        0       71 2024-05-18 21:37:32.000000 numpytransforms-0.0.1/src/NumpyTransforms/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-18 21:38:02.863343 numpytransforms-0.0.1/src/NumpyTransforms.egg-info/
+-rw-rw-rw-   0        0        0    41739 2024-05-18 21:38:02.000000 numpytransforms-0.0.1/src/NumpyTransforms.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      312 2024-05-18 21:38:02.000000 numpytransforms-0.0.1/src/NumpyTransforms.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-18 21:38:02.000000 numpytransforms-0.0.1/src/NumpyTransforms.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       25 2024-05-18 21:38:02.000000 numpytransforms-0.0.1/src/NumpyTransforms.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        0 2024-05-16 15:09:19.000000 numpytransforms-0.0.1/src/__init__.py
```

### Comparing `numpytransforms-0.0.0/LICENSE` & `numpytransforms-0.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `numpytransforms-0.0.0/PKG-INFO` & `numpytransforms-0.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: NumpyTransforms
-Version: 0.0.0
+Version: 0.0.1
 Summary: Library of helpful transformations for numpy arrays
 Author-email: Carter Bodinger <carterallenbodinger@yahoo.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -680,7 +680,10 @@
         
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
+
+# NumpyTransforms
+Helpful transformations for numpy arrays
```

### Comparing `numpytransforms-0.0.0/src/NumpyTransforms/Affine.py` & `numpytransforms-0.0.1/src/NumpyTransforms/Affine.py`

 * *Files identical despite different names*

### Comparing `numpytransforms-0.0.0/src/NumpyTransforms/Bezier.py` & `numpytransforms-0.0.1/src/NumpyTransforms/Bezier.py`

 * *Files identical despite different names*

### Comparing `numpytransforms-0.0.0/src/NumpyTransforms.egg-info/PKG-INFO` & `numpytransforms-0.0.1/src/NumpyTransforms.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: NumpyTransforms
-Version: 0.0.0
+Version: 0.0.1
 Summary: Library of helpful transformations for numpy arrays
 Author-email: Carter Bodinger <carterallenbodinger@yahoo.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -680,7 +680,10 @@
         
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
+
+# NumpyTransforms
+Helpful transformations for numpy arrays
```

