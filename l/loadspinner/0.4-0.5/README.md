# Comparing `tmp/loadspinner-0.4.tar.gz` & `tmp/loadspinner-0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "loadspinner-0.4.tar", last modified: Sun May 12 09:18:13 2024, max compression
+gzip compressed data, was "loadspinner-0.5.tar", last modified: Sat May 18 04:56:41 2024, max compression
```

## Comparing `loadspinner-0.4.tar` & `loadspinner-0.5.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 xyz       (1000) xyz       (1000)        0 2024-05-12 09:18:13.539399 loadspinner-0.4/
--rw-r--r--   0 xyz       (1000) xyz       (1000)     1061 2024-05-01 16:53:43.000000 loadspinner-0.4/LICENSE
--rw-r--r--   0 xyz       (1000) xyz       (1000)     1675 2024-05-12 09:18:13.539399 loadspinner-0.4/PKG-INFO
--rw-r--r--   0 xyz       (1000) xyz       (1000)      940 2024-05-12 09:08:44.000000 loadspinner-0.4/README.md
-drwxr-xr-x   0 xyz       (1000) xyz       (1000)        0 2024-05-12 09:18:13.538399 loadspinner-0.4/loadspinner/
--rw-r--r--   0 xyz       (1000) xyz       (1000)     3311 2024-05-12 09:17:57.000000 loadspinner-0.4/loadspinner/__init__.py
--rw-r--r--   0 xyz       (1000) xyz       (1000)     5640 2024-05-12 08:59:13.000000 loadspinner-0.4/loadspinner/_spinners.py
-drwxr-xr-x   0 xyz       (1000) xyz       (1000)        0 2024-05-12 09:18:13.538399 loadspinner-0.4/loadspinner/tools/
--rw-r--r--   0 xyz       (1000) xyz       (1000)      476 2024-04-29 18:02:17.000000 loadspinner-0.4/loadspinner/tools/demo.py
--rw-r--r--   0 xyz       (1000) xyz       (1000)      284 2024-05-08 23:02:02.000000 loadspinner-0.4/loadspinner/tools/preview.py
-drwxr-xr-x   0 xyz       (1000) xyz       (1000)        0 2024-05-12 09:18:13.538399 loadspinner-0.4/loadspinner.egg-info/
--rw-r--r--   0 xyz       (1000) xyz       (1000)     1675 2024-05-12 09:18:13.000000 loadspinner-0.4/loadspinner.egg-info/PKG-INFO
--rw-r--r--   0 xyz       (1000) xyz       (1000)      270 2024-05-12 09:18:13.000000 loadspinner-0.4/loadspinner.egg-info/SOURCES.txt
--rw-r--r--   0 xyz       (1000) xyz       (1000)        1 2024-05-12 09:18:13.000000 loadspinner-0.4/loadspinner.egg-info/dependency_links.txt
--rw-r--r--   0 xyz       (1000) xyz       (1000)       12 2024-05-12 09:18:13.000000 loadspinner-0.4/loadspinner.egg-info/top_level.txt
--rw-r--r--   0 xyz       (1000) xyz       (1000)       38 2024-05-12 09:18:13.539399 loadspinner-0.4/setup.cfg
--rw-r--r--   0 xyz       (1000) xyz       (1000)     1060 2024-05-01 07:28:17.000000 loadspinner-0.4/setup.py
+drwxr-xr-x   0 xyz       (1000) xyz       (1000)        0 2024-05-18 04:56:41.885583 loadspinner-0.5/
+-rw-r--r--   0 xyz       (1000) xyz       (1000)     1061 2024-05-01 16:53:43.000000 loadspinner-0.5/LICENSE
+-rw-r--r--   0 xyz       (1000) xyz       (1000)     2163 2024-05-18 04:56:41.885583 loadspinner-0.5/PKG-INFO
+-rw-r--r--   0 xyz       (1000) xyz       (1000)     1428 2024-05-18 04:53:05.000000 loadspinner-0.5/README.md
+drwxr-xr-x   0 xyz       (1000) xyz       (1000)        0 2024-05-18 04:56:41.884584 loadspinner-0.5/loadspinner/
+-rw-r--r--   0 xyz       (1000) xyz       (1000)     3927 2024-05-18 04:34:14.000000 loadspinner-0.5/loadspinner/__init__.py
+-rw-r--r--   0 xyz       (1000) xyz       (1000)     5640 2024-05-12 08:59:13.000000 loadspinner-0.5/loadspinner/_spinners.py
+drwxr-xr-x   0 xyz       (1000) xyz       (1000)        0 2024-05-18 04:56:41.885583 loadspinner-0.5/loadspinner/tools/
+-rw-r--r--   0 xyz       (1000) xyz       (1000)      476 2024-04-29 18:02:17.000000 loadspinner-0.5/loadspinner/tools/demo.py
+-rw-r--r--   0 xyz       (1000) xyz       (1000)      284 2024-05-08 23:02:02.000000 loadspinner-0.5/loadspinner/tools/preview.py
+drwxr-xr-x   0 xyz       (1000) xyz       (1000)        0 2024-05-18 04:56:41.885583 loadspinner-0.5/loadspinner.egg-info/
+-rw-r--r--   0 xyz       (1000) xyz       (1000)     2163 2024-05-18 04:56:41.000000 loadspinner-0.5/loadspinner.egg-info/PKG-INFO
+-rw-r--r--   0 xyz       (1000) xyz       (1000)      270 2024-05-18 04:56:41.000000 loadspinner-0.5/loadspinner.egg-info/SOURCES.txt
+-rw-r--r--   0 xyz       (1000) xyz       (1000)        1 2024-05-18 04:56:41.000000 loadspinner-0.5/loadspinner.egg-info/dependency_links.txt
+-rw-r--r--   0 xyz       (1000) xyz       (1000)       12 2024-05-18 04:56:41.000000 loadspinner-0.5/loadspinner.egg-info/top_level.txt
+-rw-r--r--   0 xyz       (1000) xyz       (1000)       38 2024-05-18 04:56:41.885583 loadspinner-0.5/setup.cfg
+-rw-r--r--   0 xyz       (1000) xyz       (1000)     1060 2024-05-01 07:28:17.000000 loadspinner-0.5/setup.py
```

### Comparing `loadspinner-0.4/LICENSE` & `loadspinner-0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `loadspinner-0.4/README.md` & `loadspinner-0.5/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 # loadspinner
 ![Pepy Total Downlods](https://img.shields.io/pepy/dt/loadspinner)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/loadspinner)
 ![GitHub repo size](https://img.shields.io/github/repo-size/xyzpw/loadspinner)
 
-A CLI based loading spinner.
+A CLI based loading spinner which is used to tell the user work is being done in the background.
+
+**Loadspinner** contains more than 20 spinners to choose from, and you can even create your own spinner.
 
 ## Prerequisites
 - Terminal that accepts ANSI codes
 
 ## Usage
 Creating a spinner:
 ```python
@@ -35,7 +37,18 @@
 ```python
 from loadspinner import functionSpinner
 @functionSpinner("building")
 def doWork():
     # code...
 doWork()
 ```
+
+Spinners can be made or customized:
+```python
+import loadspinner
+loadspinner.makeSpinner(
+    name="myCustomSpinner",
+    frames=["a", "b", "c", "1", "2", "3"],
+    interval=200,
+)
+```
+The above code will create its own spinner which can be accessed as its own name, e.g. `loadspinner.Spinner("myCustomSpinner")`
```

### Comparing `loadspinner-0.4/loadspinner/__init__.py` & `loadspinner-0.5/loadspinner/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -4,17 +4,18 @@
 from time import sleep
 from time import time as getEpoch
 import multiprocessing
 
 __all__ = [
     "Spinner",
     "functionSpinner",
+    "makeSpinner",
 ]
 
-__version__ = "0.4"
+__version__ = "0.5"
 __description__ = "a CLI based loading spinner."
 __author__ = "xyzpw"
 __license__ = "MIT"
 
 class Spinner:
     def __init__(self, spinner_type: str = "classic"):
         self.spinner_type = spinner_type
@@ -81,7 +82,20 @@
 def functionSpinner(spinner_type: str):
     def func_wrapper(func):
         def wrapper(*args, **kwargs):
             with Spinner(spinner_type):
                 return func(*args, **kwargs)
         return wrapper
     return func_wrapper
+
+def makeSpinner(name: str, frames: list, interval: int):
+    """Creates a custom spinner which can be used with specified name.
+
+    :param name: the name of which the spinner will be given
+    :param frames: the frames of which each will be printed to display the spinner
+    :param interval: the interval in milliseconds between each frame being printed"""
+    if not (isinstance(name, str) and isinstance(frames, list) and isinstance(interval, int)):
+        raise TypeError("invalid variable type")
+    all_spinners[name] = {
+        "frames": frames,
+        "interval": interval/1e3,
+    }
```

### Comparing `loadspinner-0.4/loadspinner/_spinners.py` & `loadspinner-0.5/loadspinner/_spinners.py`

 * *Files identical despite different names*

### Comparing `loadspinner-0.4/setup.py` & `loadspinner-0.5/setup.py`

 * *Files identical despite different names*

