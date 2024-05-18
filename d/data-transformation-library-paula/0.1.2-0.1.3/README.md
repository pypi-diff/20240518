# Comparing `tmp/data_transformation_library_paula-0.1.2.tar.gz` & `tmp/data_transformation_library_paula-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "data_transformation_library_paula-0.1.2.tar", max compression
+gzip compressed data, was "data_transformation_library_paula-0.1.3.tar", max compression
```

## Comparing `data_transformation_library_paula-0.1.2.tar` & `data_transformation_library_paula-0.1.3.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0        0 2024-05-16 11:33:25.380607 data_transformation_library_paula-0.1.2/data_transformation_library_paula/__init__.py
--rw-r--r--   0        0        0     4959 2024-05-16 12:35:24.095538 data_transformation_library_paula-0.1.2/data_transformation_library_paula/transformation_functions.py
--rw-r--r--   0        0        0     2851 2024-05-16 12:13:56.543951 data_transformation_library_paula-0.1.2/data_transformation_library_paula/validators.py
--rw-r--r--   0        0        0      607 2024-05-16 12:35:51.216026 data_transformation_library_paula-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     2604 2024-05-16 12:14:41.243043 data_transformation_library_paula-0.1.2/README.md
--rw-r--r--   0        0        0     3160 1970-01-01 00:00:00.000000 data_transformation_library_paula-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-05-16 11:33:25.380607 data_transformation_library_paula-0.1.3/data_transformation_library_paula/__init__.py
+-rw-r--r--   0        0        0     4959 2024-05-16 12:35:24.095538 data_transformation_library_paula-0.1.3/data_transformation_library_paula/transformation_functions.py
+-rw-r--r--   0        0        0     2851 2024-05-16 12:13:56.543951 data_transformation_library_paula-0.1.3/data_transformation_library_paula/validators.py
+-rw-r--r--   0        0        0      607 2024-05-18 11:45:17.161525 data_transformation_library_paula-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     2779 2024-05-18 11:41:24.644075 data_transformation_library_paula-0.1.3/README.md
+-rw-r--r--   0        0        0     3335 1970-01-01 00:00:00.000000 data_transformation_library_paula-0.1.3/PKG-INFO
```

### Comparing `data_transformation_library_paula-0.1.2/data_transformation_library_paula/transformation_functions.py` & `data_transformation_library_paula-0.1.3/data_transformation_library_paula/transformation_functions.py`

 * *Files identical despite different names*

### Comparing `data_transformation_library_paula-0.1.2/data_transformation_library_paula/validators.py` & `data_transformation_library_paula-0.1.3/data_transformation_library_paula/validators.py`

 * *Files identical despite different names*

### Comparing `data_transformation_library_paula-0.1.2/README.md` & `data_transformation_library_paula-0.1.3/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -48,29 +48,30 @@
 ```
 
 ## Usage
 After installation, the functions can be imported and used in Python scripts or Jupyter notebooks.
 
 Example usage:
 ```
-from data_transformation_library_paula import transpose2d, window1d, convolution2d
+from data_transformation_library_paula import transformation_functions
+import numpy as np
 
 # example for transpose2d
 matrix = [[1, 2, 3], [4, 5, 6]]
-transpose2d(matrix)
+transformation_functions.transpose2d(matrix)
 
 # example for window1d
 input_array = [1, 2, 3, 4, 5, 6]
 size = 3
 shift = 2
-window1d(input_array, size, shift)
+transformation_functions.window1d(input_array, size, shift)
 
 # example for convolution2d
-input_matrix = [[1, 2, 3], [4, 5, 6], [7, 8, 9]]
-kernel = [[1, 0], [0, -1]]
+input_matrix = np.array([[1, 2, 3], [4, 5, 6]])
+kernel = np.array([[1, 0], [0, -1]])
 stride = 2
-convolution2d(input_matrix, kernel, stride)
+transformation_functions.convolution2d(input_matrix, kernel, stride)
 ```
 
+## Link
 
-
-
+Find package here: https://pypi.org/project/data-transformation-library-paula/
```

### Comparing `data_transformation_library_paula-0.1.2/PKG-INFO` & `data_transformation_library_paula-0.1.3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: data-transformation-library-paula
-Version: 0.1.2
+Version: 0.1.3
 Summary: The `data-transformation-library-paula` is a Python package focused on providing essential tools for matrix operations and data transformations. These functions are fundamental for handling and processing data in areas like machine learning, signal processing, and image processing.
 Author: Paula
 Author-email: paula.valaityte@gmail.com
 Requires-Python: >=3.12,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: numpy (>=1.26.4,<2.0.0)
@@ -60,30 +60,30 @@
 ```
 
 ## Usage
 After installation, the functions can be imported and used in Python scripts or Jupyter notebooks.
 
 Example usage:
 ```
-from data_transformation_library_paula import transpose2d, window1d, convolution2d
+from data_transformation_library_paula import transformation_functions
+import numpy as np
 
 # example for transpose2d
 matrix = [[1, 2, 3], [4, 5, 6]]
-transpose2d(matrix)
+transformation_functions.transpose2d(matrix)
 
 # example for window1d
 input_array = [1, 2, 3, 4, 5, 6]
 size = 3
 shift = 2
-window1d(input_array, size, shift)
+transformation_functions.window1d(input_array, size, shift)
 
 # example for convolution2d
-input_matrix = [[1, 2, 3], [4, 5, 6], [7, 8, 9]]
-kernel = [[1, 0], [0, -1]]
+input_matrix = np.array([[1, 2, 3], [4, 5, 6]])
+kernel = np.array([[1, 0], [0, -1]])
 stride = 2
-convolution2d(input_matrix, kernel, stride)
+transformation_functions.convolution2d(input_matrix, kernel, stride)
 ```
 
+## Link
 
-
-
-
+Find package here: https://pypi.org/project/data-transformation-library-paula/
```

