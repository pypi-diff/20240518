# Comparing `tmp/data_transformation_library_ingri-0.1.0.tar.gz` & `tmp/data_transformation_library_ingri-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "data_transformation_library_ingri-0.1.0.tar", max compression
+gzip compressed data, was "data_transformation_library_ingri-0.1.1.tar", max compression
```

## Comparing `data_transformation_library_ingri-0.1.0.tar` & `data_transformation_library_ingri-0.1.1.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     2892 2024-05-18 07:16:48.292120 data_transformation_library_ingri-0.1.0/README.md
--rw-r--r--   0        0        0        0 2024-05-17 12:25:09.832766 data_transformation_library_ingri-0.1.0/data_transformation_library_ingri/__init__.py
--rw-r--r--   0        0        0     3678 2024-05-17 20:51:15.908524 data_transformation_library_ingri-0.1.0/data_transformation_library_ingri/functions.py
--rw-r--r--   0        0        0     1353 2024-05-17 19:34:12.566881 data_transformation_library_ingri-0.1.0/data_transformation_library_ingri/validate.py
--rw-r--r--   0        0        0      520 2024-05-18 10:16:25.181260 data_transformation_library_ingri-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     3473 1970-01-01 00:00:00.000000 data_transformation_library_ingri-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     2974 2024-05-18 10:23:47.752396 data_transformation_library_ingri-0.1.1/README.md
+-rw-r--r--   0        0        0        0 2024-05-17 12:25:09.832766 data_transformation_library_ingri-0.1.1/data_transformation_library_ingri/__init__.py
+-rw-r--r--   0        0        0     3712 2024-05-18 10:38:58.343557 data_transformation_library_ingri-0.1.1/data_transformation_library_ingri/functions.py
+-rw-r--r--   0        0        0     1353 2024-05-17 19:34:12.566881 data_transformation_library_ingri-0.1.1/data_transformation_library_ingri/validate.py
+-rw-r--r--   0        0        0      520 2024-05-18 10:42:51.921502 data_transformation_library_ingri-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     3555 1970-01-01 00:00:00.000000 data_transformation_library_ingri-0.1.1/PKG-INFO
```

### Comparing `data_transformation_library_ingri-0.1.0/README.md` & `data_transformation_library_ingri-0.1.1/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 
 The Data Transformation Library is a Python package designed to provide a set of functions for common data transformation tasks, such as transposing matrices, performing convolutions. This library aims to simplify data preprocessing and manipulation for machine learning and data analysis applications. There are three functions in the library:
 
 - `transpose2d`: Switches the axes of a 2D tensor.
 - `window1d`: Generates windows from a 1D time series array.
 - `convolution2d`: Computes the cross-correlation of a 2D matrix with a kernel.
 
+Library can be found: https://pypi.org/project/data-transformation-library-ingri/
 
 #### Features
 
 ##### Transpose 2D Matrix
 
 - **Signature**: `transpose2d(input_matrix: list[list[float]]) -> list`
 - **Input**: A list of lists of real numbers representing a 2D matrix.
```

### Comparing `data_transformation_library_ingri-0.1.0/data_transformation_library_ingri/functions.py` & `data_transformation_library_ingri-0.1.1/data_transformation_library_ingri/functions.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List, Union
 import numpy as np
-from validate import is_list_or_1d_numpy_array, is_2d_numpy_array, is_positive_integer
+from data_transformation_library_ingri.validate import is_list_or_1d_numpy_array, is_2d_numpy_array, is_positive_integer
 
 
 def transpose2d(input_matrix: List[List[float]]) -> List[List[float]]:
     """
     Transpose a 2D matrix.
 
     Args:
```

### Comparing `data_transformation_library_ingri-0.1.0/data_transformation_library_ingri/validate.py` & `data_transformation_library_ingri-0.1.1/data_transformation_library_ingri/validate.py`

 * *Files identical despite different names*

### Comparing `data_transformation_library_ingri-0.1.0/pyproject.toml` & `data_transformation_library_ingri-0.1.1/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "data-transformation-library-ingri"
-version = "0.1.0"
+version = "0.1.1"
 description = "The Data Transformation Library is a Python package designed to provide a set of functions for common data transformation tasks, such as transposing matrices, performing convolutions."
 authors = ["Ingrida <ingrida.vilkancaite@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.12"
 requests = "^2.31.0"
```

### Comparing `data_transformation_library_ingri-0.1.0/PKG-INFO` & `data_transformation_library_ingri-0.1.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: data-transformation-library-ingri
-Version: 0.1.0
+Version: 0.1.1
 Summary: The Data Transformation Library is a Python package designed to provide a set of functions for common data transformation tasks, such as transposing matrices, performing convolutions.
 Author: Ingrida
 Author-email: ingrida.vilkancaite@gmail.com
 Requires-Python: >=3.12,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: numpy (>=1.26.4,<2.0.0)
@@ -17,14 +17,15 @@
 
 The Data Transformation Library is a Python package designed to provide a set of functions for common data transformation tasks, such as transposing matrices, performing convolutions. This library aims to simplify data preprocessing and manipulation for machine learning and data analysis applications. There are three functions in the library:
 
 - `transpose2d`: Switches the axes of a 2D tensor.
 - `window1d`: Generates windows from a 1D time series array.
 - `convolution2d`: Computes the cross-correlation of a 2D matrix with a kernel.
 
+Library can be found: https://pypi.org/project/data-transformation-library-ingri/
 
 #### Features
 
 ##### Transpose 2D Matrix
 
 - **Signature**: `transpose2d(input_matrix: list[list[float]]) -> list`
 - **Input**: A list of lists of real numbers representing a 2D matrix.
```

