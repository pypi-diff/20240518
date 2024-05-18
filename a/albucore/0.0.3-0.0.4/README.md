# Comparing `tmp/albucore-0.0.3.tar.gz` & `tmp/albucore-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "albucore-0.0.3.tar", last modified: Thu May 16 02:11:02 2024, max compression
+gzip compressed data, was "albucore-0.0.4.tar", last modified: Sat May 18 00:36:35 2024, max compression
```

## Comparing `albucore-0.0.3.tar` & `albucore-0.0.4.tar`

### file list

```diff
@@ -1,20 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 02:11:02.332960 albucore-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-05-16 02:10:53.000000 albucore-0.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3940 2024-05-16 02:11:02.332960 albucore-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2230 2024-05-16 02:10:53.000000 albucore-0.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 02:11:02.328960 albucore-0.0.3/albucore/
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-16 02:10:53.000000 albucore-0.0.3/albucore/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1732 2024-05-16 02:10:53.000000 albucore-0.0.3/albucore/functions.py
--rw-r--r--   0 runner    (1001) docker     (127)     3824 2024-05-16 02:10:53.000000 albucore-0.0.3/albucore/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 02:11:02.332960 albucore-0.0.3/albucore.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3940 2024-05-16 02:11:02.000000 albucore-0.0.3/albucore.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      316 2024-05-16 02:11:02.000000 albucore-0.0.3/albucore.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 02:11:02.000000 albucore-0.0.3/albucore.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 02:11:02.000000 albucore-0.0.3/albucore.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-16 02:11:02.000000 albucore-0.0.3/albucore.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-16 02:11:02.000000 albucore-0.0.3/albucore.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2611 2024-05-16 02:10:53.000000 albucore-0.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-16 02:11:02.332960 albucore-0.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3671 2024-05-16 02:10:53.000000 albucore-0.0.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 02:11:02.332960 albucore-0.0.3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1515 2024-05-16 02:10:53.000000 albucore-0.0.3/tests/test_functions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 00:36:35.343985 albucore-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-05-18 00:36:26.000000 albucore-0.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3940 2024-05-18 00:36:35.343985 albucore-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2230 2024-05-18 00:36:26.000000 albucore-0.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 00:36:35.339985 albucore-0.0.4/albucore/
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-18 00:36:26.000000 albucore-0.0.4/albucore/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3412 2024-05-18 00:36:26.000000 albucore-0.0.4/albucore/functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4763 2024-05-18 00:36:26.000000 albucore-0.0.4/albucore/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 00:36:35.343985 albucore-0.0.4/albucore.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3940 2024-05-18 00:36:35.000000 albucore-0.0.4/albucore.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      336 2024-05-18 00:36:35.000000 albucore-0.0.4/albucore.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-18 00:36:35.000000 albucore-0.0.4/albucore.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-18 00:36:35.000000 albucore-0.0.4/albucore.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-18 00:36:35.000000 albucore-0.0.4/albucore.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-18 00:36:35.000000 albucore-0.0.4/albucore.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2611 2024-05-18 00:36:26.000000 albucore-0.0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-18 00:36:35.343985 albucore-0.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3671 2024-05-18 00:36:26.000000 albucore-0.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 00:36:35.343985 albucore-0.0.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    11832 2024-05-18 00:36:26.000000 albucore-0.0.4/tests/test_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1582 2024-05-18 00:36:26.000000 albucore-0.0.4/tests/test_utils.py
```

### Comparing `albucore-0.0.3/LICENSE` & `albucore-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `albucore-0.0.3/PKG-INFO` & `albucore-0.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: albucore
-Version: 0.0.3
+Version: 0.0.4
 Summary: A high-performance image processing library designed to optimize and extend the Albumentations library with specialized functions for advanced image transformations. Perfect for developers working in computer vision who require efficient and scalable image augmentation.
 Home-page: https://github.com/albumentations-team/albucore
 Author: Vladimir I. Iglovikov
 License: MIT
 Keywords: Image Processing,Computer Vision,Image Augmentation,Albumentations,Optimization,Machine Learning,Deep Learning,Python Imaging,Data Augmentation,Performance,Efficiency,High-Performance,CV,OpenCV,Automation
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -24,15 +24,15 @@
 Classifier: Topic :: Scientific/Engineering :: Image Processing
 Classifier: Typing :: Typed
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy>=1.24.4
 Requires-Dist: tomli>=2.0.1
-Requires-Dist: opencv-python-headless>=4.5.5.64
+Requires-Dist: opencv-python-headless>=4.9.0.80
 
 # Albucore
 
 Albucore is a high-performance image processing library designed to optimize operations on images using Python and OpenCV, building upon the foundations laid by the popular Albumentations library. It offers specialized optimizations for different image data types and aims to provide faster processing times through efficient algorithm implementations.
 
 ## Features
```

### Comparing `albucore-0.0.3/README.md` & `albucore-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `albucore-0.0.3/albucore/utils.py` & `albucore-0.0.4/albucore/utils.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from functools import wraps
-from typing import Any, Callable
+from typing import Any, Callable, Union
 
 import cv2
 import numpy as np
 from typing_extensions import Concatenate, ParamSpec
 
+NUM_RGB_CHANNELS = 3
 MONO_CHANNEL_DIMENSIONS = 2
 NUM_MULTI_CHANNEL_DIMENSIONS = 3
 FOUR = 4
 TWO = 2
 
 MAX_OPENCV_WORKING_CHANNELS = 4
 
@@ -23,26 +24,28 @@
     np.dtype("float64"): 1.0,
     np.uint8: 255,
     np.uint16: 65535,
     np.uint32: 4294967295,
     np.float16: 1.0,
     np.float32: 1.0,
     np.float64: 1.0,
+    np.int32: 2147483647,
 }
 
 NPDTYPE_TO_OPENCV_DTYPE = {
     np.uint8: cv2.CV_8U,
     np.uint16: cv2.CV_16U,
     np.float32: cv2.CV_32F,
     np.float64: cv2.CV_64F,
+    np.int32: cv2.CV_32S,
     np.dtype("uint8"): cv2.CV_8U,
     np.dtype("uint16"): cv2.CV_16U,
-    np.dtype("float16"): cv2.CV_16F,
     np.dtype("float32"): cv2.CV_32F,
     np.dtype("float64"): cv2.CV_64F,
+    np.dtype("int32"): cv2.CV_32S,
 }
 
 
 def maybe_process_in_chunks(
     process_fn: Callable[Concatenate[np.ndarray, P], np.ndarray], **kwargs: Any
 ) -> Callable[[np.ndarray], np.ndarray]:
     """Wrap OpenCV function to enable processing images with more than 4 channels.
@@ -93,18 +96,14 @@
     def wrapped_function(img: np.ndarray, *args: P.args, **kwargs: P.kwargs) -> np.ndarray:
         dtype = img.dtype
         return clip(func(img, *args, **kwargs), dtype)
 
     return wrapped_function
 
 
-def get_num_channels(image: np.ndarray) -> int:
-    return image.shape[2] if image.ndim == NUM_MULTI_CHANNEL_DIMENSIONS else 1
-
-
 def preserve_channel_dim(
     func: Callable[Concatenate[np.ndarray, P], np.ndarray],
 ) -> Callable[Concatenate[np.ndarray, P], np.ndarray]:
     """Preserve dummy channel dim."""
 
     @wraps(func)
     def wrapped_function(img: np.ndarray, *args: P.args, **kwargs: P.kwargs) -> np.ndarray:
@@ -116,9 +115,41 @@
         if len(shape) == MONO_CHANNEL_DIMENSIONS and result.ndim == NUM_MULTI_CHANNEL_DIMENSIONS:
             return result[:, :, 0]
         return result
 
     return wrapped_function
 
 
+def get_num_channels(image: np.ndarray) -> int:
+    return image.shape[2] if image.ndim == NUM_MULTI_CHANNEL_DIMENSIONS else 1
+
+
 def is_grayscale_image(image: np.ndarray) -> bool:
     return get_num_channels(image) == 1
+
+
+def get_opencv_dtype_from_numpy(value: Union[np.ndarray, int, np.dtype, object]) -> int:
+    if isinstance(value, np.ndarray):
+        value = value.dtype
+    return NPDTYPE_TO_OPENCV_DTYPE[value]
+
+
+def is_rgb_image(image: np.ndarray) -> bool:
+    return get_num_channels(image) == NUM_RGB_CHANNELS
+
+
+def is_multispectral_image(image: np.ndarray) -> bool:
+    num_channels = get_num_channels(image)
+    return num_channels not in {1, 3}
+
+
+def contiguous(
+    func: Callable[Concatenate[np.ndarray, P], np.ndarray],
+) -> Callable[Concatenate[np.ndarray, P], np.ndarray]:
+    """Ensure that input img is contiguous."""
+
+    @wraps(func)
+    def wrapped_function(img: np.ndarray, *args: P.args, **kwargs: P.kwargs) -> np.ndarray:
+        img = np.require(img, requirements=["C_CONTIGUOUS"])
+        return func(img, *args, **kwargs)
+
+    return wrapped_function
```

### Comparing `albucore-0.0.3/albucore.egg-info/PKG-INFO` & `albucore-0.0.4/albucore.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: albucore
-Version: 0.0.3
+Version: 0.0.4
 Summary: A high-performance image processing library designed to optimize and extend the Albumentations library with specialized functions for advanced image transformations. Perfect for developers working in computer vision who require efficient and scalable image augmentation.
 Home-page: https://github.com/albumentations-team/albucore
 Author: Vladimir I. Iglovikov
 License: MIT
 Keywords: Image Processing,Computer Vision,Image Augmentation,Albumentations,Optimization,Machine Learning,Deep Learning,Python Imaging,Data Augmentation,Performance,Efficiency,High-Performance,CV,OpenCV,Automation
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -24,15 +24,15 @@
 Classifier: Topic :: Scientific/Engineering :: Image Processing
 Classifier: Typing :: Typed
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy>=1.24.4
 Requires-Dist: tomli>=2.0.1
-Requires-Dist: opencv-python-headless>=4.5.5.64
+Requires-Dist: opencv-python-headless>=4.9.0.80
 
 # Albucore
 
 Albucore is a high-performance image processing library designed to optimize operations on images using Python and OpenCV, building upon the foundations laid by the popular Albumentations library. It offers specialized optimizations for different image data types and aims to provide faster processing times through efficient algorithm implementations.
 
 ## Features
```

### Comparing `albucore-0.0.3/pyproject.toml` & `albucore-0.0.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `albucore-0.0.3/setup.py` & `albucore-0.0.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from setuptools import find_packages, setup
 
 INSTALL_REQUIRES = [
     "numpy>=1.24.4",
     "tomli>=2.0.1",
 ]
 
-MIN_OPENCV_VERSION = "4.5.5.64"
+MIN_OPENCV_VERSION = "4.9.0.80"
 
 CHOOSE_INSTALL_REQUIRES = [
     (
         (f"opencv-python>={MIN_OPENCV_VERSION}", f"opencv-contrib-python>={MIN_OPENCV_VERSION}", f"opencv-contrib-python-headless>={MIN_OPENCV_VERSION}"),
         f"opencv-python-headless>={MIN_OPENCV_VERSION}",
     ),
 ]
```

