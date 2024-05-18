# Comparing `tmp/fastdev-0.0.2.tar.gz` & `tmp/fastdev-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastdev-0.0.2.tar", last modified: Tue May 14 00:49:09 2024, max compression
+gzip compressed data, was "fastdev-0.0.3.tar", last modified: Sat May 18 01:36:01 2024, max compression
```

## Comparing `fastdev-0.0.2.tar` & `fastdev-0.0.3.tar`

### file list

```diff
@@ -1,48 +1,51 @@
-drwxrwxr-x   0 jianglong  (1000) jianglong  (1000)        0 2024-05-14 00:49:09.307538 fastdev-0.0.2/
--rw-r--r--   0 jianglong  (1000) jianglong  (1000)      888 2024-05-14 00:49:09.307538 fastdev-0.0.2/PKG-INFO
--rw-rw-r--   0 jianglong  (1000) jianglong  (1000)       32 2024-05-13 08:49:05.000000 fastdev-0.0.2/README.md
--rw-rw-r--   0 jianglong  (1000) jianglong  (1000)      849 2024-05-14 00:43:13.000000 fastdev-0.0.2/pyproject.toml
--rw-rw-r--   0 jianglong  (1000) jianglong  (1000)       38 2024-05-14 00:49:09.307538 fastdev-0.0.2/setup.cfg
-drwxrwxr-x   0 jianglong  (1000) jianglong  (1000)        0 2024-05-14 00:49:09.304538 fastdev-0.0.2/src/
-drwxrwxr-x   0 jianglong  (1000) jianglong  (1000)        0 2024-05-14 00:49:09.305538 fastdev-0.0.2/src/fastdev/
--rw-rw-r--   0 jianglong  (1000) jianglong  (1000)       69 2024-05-13 08:49:05.000000 fastdev-0.0.2/src/fastdev/__init__.py
--rw-rw-r--   0 jianglong  (1000) jianglong  (1000)      597 2024-05-13 08:49:05.000000 fastdev-0.0.2/src/fastdev/constants.py
-drwxrwxr-x   0 jianglong  (1000) jianglong  (1000)        0 2024-05-14 00:49:09.305538 fastdev-0.0.2/src/fastdev/datasets/
--rw-rw-r--   0 jianglong  (1000) jianglong  (1000)        0 2024-05-13 08:49:05.000000 fastdev-0.0.2/src/fastdev/datasets/__init__.py
--rw-rw-r--   0 jianglong  (1000) jianglong  (1000)    17435 2024-05-13 08:49:05.000000 fastdev-0.0.2/src/fastdev/datasets/dexycb.py
-drwxrwxr-x   0 jianglong  (1000) jianglong  (1000)        0 2024-05-14 00:49:09.305538 fastdev-0.0.2/src/fastdev/fileio/
--rw-rw-r--   0 jianglong  (1000) jianglong  (1000)       69 2024-05-13 08:49:05.000000 fastdev-0.0.2/src/fastdev/fileio/__init__.py
-drwxrwxr-x   0 jianglong  (1000) jianglong  (1000)        0 2024-05-14 00:49:09.306537 fastdev-0.0.2/src/fastdev/fileio/handlers/
--rw-rw-r--   0 jianglong  (1000) jianglong  (1000)        0 2024-05-13 08:49:05.000000 fastdev-0.0.2/src/fastdev/fileio/handlers/__init__.py
--rw-rw-r--   0 jianglong  (1000) jianglong  (1000)      533 2024-05-13 08:49:05.000000 fastdev-0.0.2/src/fastdev/fileio/handlers/base_handler.py
--rw-rw-r--   0 jianglong  (1000) jianglong  (1000)      699 2024-05-13 08:49:05.000000 fastdev-0.0.2/src/fastdev/fileio/handlers/json_handler.py
--rw-rw-r--   0 jianglong  (1000) jianglong  (1000)     1737 2024-05-13 08:49:05.000000 fastdev-0.0.2/src/fastdev/fileio/handlers/yaml_handler.py
--rw-rw-r--   0 jianglong  (1000) jianglong  (1000)     3626 2024-05-13 08:49:05.000000 fastdev-0.0.2/src/fastdev/fileio/io.py
--rw-rw-r--   0 jianglong  (1000) jianglong  (1000)     1248 2024-05-13 08:49:05.000000 fastdev-0.0.2/src/fastdev/fileio/io_cli.py
-drwxrwxr-x   0 jianglong  (1000) jianglong  (1000)        0 2024-05-14 00:49:09.306537 fastdev-0.0.2/src/fastdev/robotics/
--rw-rw-r--   0 jianglong  (1000) jianglong  (1000)       90 2024-05-13 08:49:05.000000 fastdev-0.0.2/src/fastdev/robotics/__init__.py
--rw-rw-r--   0 jianglong  (1000) jianglong  (1000)      273 2024-05-13 08:49:05.000000 fastdev-0.0.2/src/fastdev/robotics/kinematics.py
--rw-rw-r--   0 jianglong  (1000) jianglong  (1000)     1028 2024-05-14 00:31:47.000000 fastdev-0.0.2/src/fastdev/robotics/urdf.py
-drwxrwxr-x   0 jianglong  (1000) jianglong  (1000)        0 2024-05-14 00:49:09.306537 fastdev-0.0.2/src/fastdev/smplx/
--rw-rw-r--   0 jianglong  (1000) jianglong  (1000)      256 2024-05-13 08:49:05.000000 fastdev-0.0.2/src/fastdev/smplx/__init__.py
--rw-rw-r--   0 jianglong  (1000) jianglong  (1000)     3778 2024-05-13 08:49:05.000000 fastdev-0.0.2/src/fastdev/smplx/smplx.py
-drwxrwxr-x   0 jianglong  (1000) jianglong  (1000)        0 2024-05-14 00:49:09.306537 fastdev-0.0.2/src/fastdev/transforms/
--rw-rw-r--   0 jianglong  (1000) jianglong  (1000)     1379 2024-05-13 08:49:05.000000 fastdev-0.0.2/src/fastdev/transforms/__init__.py
--rw-rw-r--   0 jianglong  (1000) jianglong  (1000)    17378 2024-05-13 08:49:05.000000 fastdev-0.0.2/src/fastdev/transforms/rotation.py
--rw-rw-r--   0 jianglong  (1000) jianglong  (1000)     5547 2024-05-13 08:49:05.000000 fastdev-0.0.2/src/fastdev/transforms/transforms.py
--rw-rw-r--   0 jianglong  (1000) jianglong  (1000)      469 2024-05-13 08:49:05.000000 fastdev-0.0.2/src/fastdev/transforms/utils.py
-drwxrwxr-x   0 jianglong  (1000) jianglong  (1000)        0 2024-05-14 00:49:09.306537 fastdev-0.0.2/src/fastdev/utils/
--rw-rw-r--   0 jianglong  (1000) jianglong  (1000)       59 2024-05-13 08:49:05.000000 fastdev-0.0.2/src/fastdev/utils/__init__.py
--rw-rw-r--   0 jianglong  (1000) jianglong  (1000)     1313 2024-05-13 08:49:05.000000 fastdev-0.0.2/src/fastdev/utils/timer.py
-drwxrwxr-x   0 jianglong  (1000) jianglong  (1000)        0 2024-05-14 00:49:09.306537 fastdev-0.0.2/src/fastdev/visualization/
--rw-rw-r--   0 jianglong  (1000) jianglong  (1000)       79 2024-05-13 08:49:05.000000 fastdev-0.0.2/src/fastdev/visualization/__init__.py
--rw-rw-r--   0 jianglong  (1000) jianglong  (1000)     1680 2024-05-13 08:49:05.000000 fastdev-0.0.2/src/fastdev/visualization/image.py
-drwxrwxr-x   0 jianglong  (1000) jianglong  (1000)        0 2024-05-14 00:49:09.306537 fastdev-0.0.2/src/fastdev.egg-info/
--rw-r--r--   0 jianglong  (1000) jianglong  (1000)      888 2024-05-14 00:49:09.000000 fastdev-0.0.2/src/fastdev.egg-info/PKG-INFO
--rw-rw-r--   0 jianglong  (1000) jianglong  (1000)     1050 2024-05-14 00:49:09.000000 fastdev-0.0.2/src/fastdev.egg-info/SOURCES.txt
--rw-rw-r--   0 jianglong  (1000) jianglong  (1000)        1 2024-05-14 00:49:09.000000 fastdev-0.0.2/src/fastdev.egg-info/dependency_links.txt
--rw-rw-r--   0 jianglong  (1000) jianglong  (1000)       50 2024-05-14 00:49:09.000000 fastdev-0.0.2/src/fastdev.egg-info/entry_points.txt
--rw-rw-r--   0 jianglong  (1000) jianglong  (1000)      146 2024-05-14 00:49:09.000000 fastdev-0.0.2/src/fastdev.egg-info/requires.txt
--rw-rw-r--   0 jianglong  (1000) jianglong  (1000)        8 2024-05-14 00:49:09.000000 fastdev-0.0.2/src/fastdev.egg-info/top_level.txt
-drwxrwxr-x   0 jianglong  (1000) jianglong  (1000)        0 2024-05-14 00:49:09.306537 fastdev-0.0.2/tests/
--rw-rw-r--   0 jianglong  (1000) jianglong  (1000)     1199 2024-05-13 08:49:05.000000 fastdev-0.0.2/tests/test_fileio.py
+drwxrwxr-x   0 jianglong  (1000) jianglong  (1000)        0 2024-05-18 01:36:01.245540 fastdev-0.0.3/
+-rw-r--r--   0 jianglong  (1000) jianglong  (1000)      888 2024-05-18 01:36:01.245540 fastdev-0.0.3/PKG-INFO
+-rw-rw-r--   0 jianglong  (1000) jianglong  (1000)       32 2024-05-13 08:49:05.000000 fastdev-0.0.3/README.md
+-rw-rw-r--   0 jianglong  (1000) jianglong  (1000)      849 2024-05-18 01:34:25.000000 fastdev-0.0.3/pyproject.toml
+-rw-rw-r--   0 jianglong  (1000) jianglong  (1000)       38 2024-05-18 01:36:01.245540 fastdev-0.0.3/setup.cfg
+drwxrwxr-x   0 jianglong  (1000) jianglong  (1000)        0 2024-05-18 01:36:01.242540 fastdev-0.0.3/src/
+drwxrwxr-x   0 jianglong  (1000) jianglong  (1000)        0 2024-05-18 01:36:01.243540 fastdev-0.0.3/src/fastdev/
+-rw-rw-r--   0 jianglong  (1000) jianglong  (1000)       69 2024-05-13 08:49:05.000000 fastdev-0.0.3/src/fastdev/__init__.py
+-rw-rw-r--   0 jianglong  (1000) jianglong  (1000)      597 2024-05-14 01:25:51.000000 fastdev-0.0.3/src/fastdev/constants.py
+drwxrwxr-x   0 jianglong  (1000) jianglong  (1000)        0 2024-05-18 01:36:01.243540 fastdev-0.0.3/src/fastdev/datasets/
+-rw-rw-r--   0 jianglong  (1000) jianglong  (1000)        0 2024-05-13 08:49:05.000000 fastdev-0.0.3/src/fastdev/datasets/__init__.py
+-rw-rw-r--   0 jianglong  (1000) jianglong  (1000)    17435 2024-05-13 08:49:05.000000 fastdev-0.0.3/src/fastdev/datasets/dexycb.py
+drwxrwxr-x   0 jianglong  (1000) jianglong  (1000)        0 2024-05-18 01:36:01.243540 fastdev-0.0.3/src/fastdev/fileio/
+-rw-rw-r--   0 jianglong  (1000) jianglong  (1000)       69 2024-05-13 08:49:05.000000 fastdev-0.0.3/src/fastdev/fileio/__init__.py
+drwxrwxr-x   0 jianglong  (1000) jianglong  (1000)        0 2024-05-18 01:36:01.244540 fastdev-0.0.3/src/fastdev/fileio/handlers/
+-rw-rw-r--   0 jianglong  (1000) jianglong  (1000)        0 2024-05-13 08:49:05.000000 fastdev-0.0.3/src/fastdev/fileio/handlers/__init__.py
+-rw-rw-r--   0 jianglong  (1000) jianglong  (1000)      533 2024-05-13 08:49:05.000000 fastdev-0.0.3/src/fastdev/fileio/handlers/base_handler.py
+-rw-rw-r--   0 jianglong  (1000) jianglong  (1000)      699 2024-05-13 08:49:05.000000 fastdev-0.0.3/src/fastdev/fileio/handlers/json_handler.py
+-rw-rw-r--   0 jianglong  (1000) jianglong  (1000)     1737 2024-05-13 08:49:05.000000 fastdev-0.0.3/src/fastdev/fileio/handlers/yaml_handler.py
+-rw-rw-r--   0 jianglong  (1000) jianglong  (1000)     2722 2024-05-15 08:19:43.000000 fastdev-0.0.3/src/fastdev/fileio/io.py
+drwxrwxr-x   0 jianglong  (1000) jianglong  (1000)        0 2024-05-18 01:36:01.244540 fastdev-0.0.3/src/fastdev/robotics/
+-rw-rw-r--   0 jianglong  (1000) jianglong  (1000)       90 2024-05-13 08:49:05.000000 fastdev-0.0.3/src/fastdev/robotics/__init__.py
+-rw-rw-r--   0 jianglong  (1000) jianglong  (1000)      273 2024-05-13 08:49:05.000000 fastdev-0.0.3/src/fastdev/robotics/kinematics.py
+-rw-rw-r--   0 jianglong  (1000) jianglong  (1000)     1028 2024-05-14 00:31:47.000000 fastdev-0.0.3/src/fastdev/robotics/urdf.py
+drwxrwxr-x   0 jianglong  (1000) jianglong  (1000)        0 2024-05-18 01:36:01.244540 fastdev-0.0.3/src/fastdev/smplx/
+-rw-rw-r--   0 jianglong  (1000) jianglong  (1000)      256 2024-05-13 08:49:05.000000 fastdev-0.0.3/src/fastdev/smplx/__init__.py
+-rw-rw-r--   0 jianglong  (1000) jianglong  (1000)     3778 2024-05-13 08:49:05.000000 fastdev-0.0.3/src/fastdev/smplx/smplx.py
+drwxrwxr-x   0 jianglong  (1000) jianglong  (1000)        0 2024-05-18 01:36:01.244540 fastdev-0.0.3/src/fastdev/transforms/
+-rw-rw-r--   0 jianglong  (1000) jianglong  (1000)     1421 2024-05-18 00:55:47.000000 fastdev-0.0.3/src/fastdev/transforms/__init__.py
+drwxrwxr-x   0 jianglong  (1000) jianglong  (1000)        0 2024-05-18 01:36:01.244540 fastdev-0.0.3/src/fastdev/transforms/numpy/
+-rw-rw-r--   0 jianglong  (1000) jianglong  (1000)      103 2024-05-15 07:37:41.000000 fastdev-0.0.3/src/fastdev/transforms/numpy/__init__.py
+-rw-rw-r--   0 jianglong  (1000) jianglong  (1000)     1007 2024-05-15 07:38:48.000000 fastdev-0.0.3/src/fastdev/transforms/numpy/transforms.py
+-rw-rw-r--   0 jianglong  (1000) jianglong  (1000)    17378 2024-05-13 08:49:05.000000 fastdev-0.0.3/src/fastdev/transforms/rotation.py
+-rw-rw-r--   0 jianglong  (1000) jianglong  (1000)     5547 2024-05-13 08:49:05.000000 fastdev-0.0.3/src/fastdev/transforms/transforms.py
+-rw-rw-r--   0 jianglong  (1000) jianglong  (1000)     2881 2024-05-18 00:54:56.000000 fastdev-0.0.3/src/fastdev/transforms/utils.py
+drwxrwxr-x   0 jianglong  (1000) jianglong  (1000)        0 2024-05-18 01:36:01.244540 fastdev-0.0.3/src/fastdev/utils/
+-rw-rw-r--   0 jianglong  (1000) jianglong  (1000)       59 2024-05-13 08:49:05.000000 fastdev-0.0.3/src/fastdev/utils/__init__.py
+-rw-rw-r--   0 jianglong  (1000) jianglong  (1000)     1188 2024-05-17 08:54:36.000000 fastdev-0.0.3/src/fastdev/utils/geometry.py
+-rw-rw-r--   0 jianglong  (1000) jianglong  (1000)     1313 2024-05-13 08:49:05.000000 fastdev-0.0.3/src/fastdev/utils/timer.py
+drwxrwxr-x   0 jianglong  (1000) jianglong  (1000)        0 2024-05-18 01:36:01.244540 fastdev-0.0.3/src/fastdev/visualization/
+-rw-rw-r--   0 jianglong  (1000) jianglong  (1000)       79 2024-05-13 08:49:05.000000 fastdev-0.0.3/src/fastdev/visualization/__init__.py
+-rw-rw-r--   0 jianglong  (1000) jianglong  (1000)     1680 2024-05-13 08:49:05.000000 fastdev-0.0.3/src/fastdev/visualization/image.py
+drwxrwxr-x   0 jianglong  (1000) jianglong  (1000)        0 2024-05-18 01:36:01.244540 fastdev-0.0.3/src/fastdev.egg-info/
+-rw-r--r--   0 jianglong  (1000) jianglong  (1000)      888 2024-05-18 01:36:01.000000 fastdev-0.0.3/src/fastdev.egg-info/PKG-INFO
+-rw-rw-r--   0 jianglong  (1000) jianglong  (1000)     1135 2024-05-18 01:36:01.000000 fastdev-0.0.3/src/fastdev.egg-info/SOURCES.txt
+-rw-rw-r--   0 jianglong  (1000) jianglong  (1000)        1 2024-05-18 01:36:01.000000 fastdev-0.0.3/src/fastdev.egg-info/dependency_links.txt
+-rw-rw-r--   0 jianglong  (1000) jianglong  (1000)       50 2024-05-18 01:36:01.000000 fastdev-0.0.3/src/fastdev.egg-info/entry_points.txt
+-rw-rw-r--   0 jianglong  (1000) jianglong  (1000)      146 2024-05-18 01:36:01.000000 fastdev-0.0.3/src/fastdev.egg-info/requires.txt
+-rw-rw-r--   0 jianglong  (1000) jianglong  (1000)        8 2024-05-18 01:36:01.000000 fastdev-0.0.3/src/fastdev.egg-info/top_level.txt
+drwxrwxr-x   0 jianglong  (1000) jianglong  (1000)        0 2024-05-18 01:36:01.244540 fastdev-0.0.3/tests/
+-rw-rw-r--   0 jianglong  (1000) jianglong  (1000)     1199 2024-05-13 08:49:05.000000 fastdev-0.0.3/tests/test_fileio.py
```

### Comparing `fastdev-0.0.2/PKG-INFO` & `fastdev-0.0.3/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastdev
-Version: 0.0.2
+Version: 0.0.3
 Summary: Type less, code more
 Author-email: Jianglong Ye <jianglong.yeh@gmail.com>
 License: MIT
 Project-URL: Repository, https://github.com/jianglongye/fastdev
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `fastdev-0.0.2/pyproject.toml` & `fastdev-0.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools >= 61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "fastdev"
-version = "0.0.2"
+version = "0.0.3"
 authors = [{ name = "Jianglong Ye", email = "jianglong.yeh@gmail.com" }]
 description = "Type less, code more"
 readme = "README.md"
 license = { text = "MIT" }
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
```

### Comparing `fastdev-0.0.2/src/fastdev/constants.py` & `fastdev-0.0.3/src/fastdev/constants.py`

 * *Files identical despite different names*

### Comparing `fastdev-0.0.2/src/fastdev/datasets/dexycb.py` & `fastdev-0.0.3/src/fastdev/datasets/dexycb.py`

 * *Files identical despite different names*

### Comparing `fastdev-0.0.2/src/fastdev/fileio/handlers/base_handler.py` & `fastdev-0.0.3/src/fastdev/fileio/handlers/base_handler.py`

 * *Files identical despite different names*

### Comparing `fastdev-0.0.2/src/fastdev/fileio/handlers/json_handler.py` & `fastdev-0.0.3/src/fastdev/fileio/handlers/json_handler.py`

 * *Files identical despite different names*

### Comparing `fastdev-0.0.2/src/fastdev/fileio/handlers/yaml_handler.py` & `fastdev-0.0.3/src/fastdev/fileio/handlers/yaml_handler.py`

 * *Files identical despite different names*

### Comparing `fastdev-0.0.2/src/fastdev/robotics/urdf.py` & `fastdev-0.0.3/src/fastdev/robotics/urdf.py`

 * *Files identical despite different names*

### Comparing `fastdev-0.0.2/src/fastdev/smplx/smplx.py` & `fastdev-0.0.3/src/fastdev/smplx/smplx.py`

 * *Files identical despite different names*

### Comparing `fastdev-0.0.2/src/fastdev/transforms/__init__.py` & `fastdev-0.0.3/src/fastdev/transforms/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,31 +7,31 @@
     matrix_to_euler_angles,
     matrix_to_quaternion,
     matrix_to_rotation_6d,
     quaternion_real_to_first,
     quaternion_real_to_last,
     quaternion_to_axis_angle,
     quaternion_to_matrix,
+    random_rotation_matrix,
     rotation_6d_to_matrix,
     split_axis_angle,
     standardize_quaternion,
-    random_rotation_matrix,
 )
 from fastdev.transforms.transforms import (
     expand_tf_mat,
+    inverse,
     project,
+    rot_tl_to_tf_mat,
     rotate,
-    inverse,
     swap_major,
-    rot_tl_to_tf_mat,
     to_homo,
     transform,
     unproject,
 )
-from fastdev.transforms.utils import compose_intr_mat
+from fastdev.transforms.utils import compose_intr_mat, coord_conversion
 
 __all__ = [
     "transform",
     "rotate",
     "project",
     "inverse",
     "swap_major",
@@ -52,8 +52,9 @@
     "quaternion_real_to_last",
     "quaternion_real_to_first",
     "standardize_quaternion",
     "random_rotation_matrix",
     "matrix_to_rotation_6d",
     "rotation_6d_to_matrix",
     "compose_intr_mat",
+    "coord_conversion",
 ]
```

### Comparing `fastdev-0.0.2/src/fastdev/transforms/rotation.py` & `fastdev-0.0.3/src/fastdev/transforms/rotation.py`

 * *Files identical despite different names*

### Comparing `fastdev-0.0.2/src/fastdev/transforms/transforms.py` & `fastdev-0.0.3/src/fastdev/transforms/transforms.py`

 * *Files identical despite different names*

### Comparing `fastdev-0.0.2/src/fastdev/utils/timer.py` & `fastdev-0.0.3/src/fastdev/utils/timer.py`

 * *Files identical despite different names*

### Comparing `fastdev-0.0.2/src/fastdev/visualization/image.py` & `fastdev-0.0.3/src/fastdev/visualization/image.py`

 * *Files identical despite different names*

### Comparing `fastdev-0.0.2/src/fastdev.egg-info/PKG-INFO` & `fastdev-0.0.3/src/fastdev.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastdev
-Version: 0.0.2
+Version: 0.0.3
 Summary: Type less, code more
 Author-email: Jianglong Ye <jianglong.yeh@gmail.com>
 License: MIT
 Project-URL: Repository, https://github.com/jianglongye/fastdev
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `fastdev-0.0.2/src/fastdev.egg-info/SOURCES.txt` & `fastdev-0.0.3/src/fastdev.egg-info/SOURCES.txt`

 * *Files 19% similar despite different names*

```diff
@@ -8,26 +8,28 @@
 src/fastdev.egg-info/entry_points.txt
 src/fastdev.egg-info/requires.txt
 src/fastdev.egg-info/top_level.txt
 src/fastdev/datasets/__init__.py
 src/fastdev/datasets/dexycb.py
 src/fastdev/fileio/__init__.py
 src/fastdev/fileio/io.py
-src/fastdev/fileio/io_cli.py
 src/fastdev/fileio/handlers/__init__.py
 src/fastdev/fileio/handlers/base_handler.py
 src/fastdev/fileio/handlers/json_handler.py
 src/fastdev/fileio/handlers/yaml_handler.py
 src/fastdev/robotics/__init__.py
 src/fastdev/robotics/kinematics.py
 src/fastdev/robotics/urdf.py
 src/fastdev/smplx/__init__.py
 src/fastdev/smplx/smplx.py
 src/fastdev/transforms/__init__.py
 src/fastdev/transforms/rotation.py
 src/fastdev/transforms/transforms.py
 src/fastdev/transforms/utils.py
+src/fastdev/transforms/numpy/__init__.py
+src/fastdev/transforms/numpy/transforms.py
 src/fastdev/utils/__init__.py
+src/fastdev/utils/geometry.py
 src/fastdev/utils/timer.py
 src/fastdev/visualization/__init__.py
 src/fastdev/visualization/image.py
 tests/test_fileio.py
```

### Comparing `fastdev-0.0.2/tests/test_fileio.py` & `fastdev-0.0.3/tests/test_fileio.py`

 * *Files identical despite different names*

