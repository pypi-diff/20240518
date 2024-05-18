# Comparing `tmp/pyaogmaneo-2.6.1.tar.gz` & `tmp/pyaogmaneo-2.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyaogmaneo-2.6.1.tar", last modified: Sat May 11 20:51:58 2024, max compression
+gzip compressed data, was "pyaogmaneo-2.6.2.tar", last modified: Fri May 17 23:34:17 2024, max compression
```

## Comparing `pyaogmaneo-2.6.1.tar` & `pyaogmaneo-2.6.2.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 20:51:58.444482 pyaogmaneo-2.6.1/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 20:51:58.444482 pyaogmaneo-2.6.1/CMake/
--rw-r--r--   0 runner    (1001) docker     (127)     1250 2024-05-11 20:51:47.000000 pyaogmaneo-2.6.1/CMake/FindAOgmaNeo.cmake
--rw-r--r--   0 runner    (1001) docker     (127)     2237 2024-05-11 20:51:47.000000 pyaogmaneo-2.6.1/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (127)    17842 2024-05-11 20:51:47.000000 pyaogmaneo-2.6.1/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-05-11 20:51:47.000000 pyaogmaneo-2.6.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      785 2024-05-11 20:51:58.444482 pyaogmaneo-2.6.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2415 2024-05-11 20:51:47.000000 pyaogmaneo-2.6.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 20:51:58.444482 pyaogmaneo-2.6.1/pyaogmaneo.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      785 2024-05-11 20:51:58.000000 pyaogmaneo-2.6.1/pyaogmaneo.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      505 2024-05-11 20:51:58.000000 pyaogmaneo-2.6.1/pyaogmaneo.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-11 20:51:58.000000 pyaogmaneo-2.6.1/pyaogmaneo.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-11 20:51:58.000000 pyaogmaneo-2.6.1/pyaogmaneo.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-11 20:51:58.000000 pyaogmaneo-2.6.1/pyaogmaneo.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-05-11 20:51:47.000000 pyaogmaneo-2.6.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-11 20:51:58.444482 pyaogmaneo-2.6.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     4253 2024-05-11 20:51:47.000000 pyaogmaneo-2.6.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 20:51:58.440482 pyaogmaneo-2.6.1/source/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 20:51:58.444482 pyaogmaneo-2.6.1/source/pyaogmaneo/
--rw-r--r--   0 runner    (1001) docker     (127)     1153 2024-05-11 20:51:47.000000 pyaogmaneo-2.6.1/source/pyaogmaneo/py_helpers.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1953 2024-05-11 20:51:47.000000 pyaogmaneo-2.6.1/source/pyaogmaneo/py_helpers.h
--rw-r--r--   0 runner    (1001) docker     (127)    12736 2024-05-11 20:51:47.000000 pyaogmaneo-2.6.1/source/pyaogmaneo/py_hierarchy.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     6861 2024-05-11 20:51:47.000000 pyaogmaneo-2.6.1/source/pyaogmaneo/py_hierarchy.h
--rw-r--r--   0 runner    (1001) docker     (127)     7846 2024-05-11 20:51:47.000000 pyaogmaneo-2.6.1/source/pyaogmaneo/py_image_encoder.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     3209 2024-05-11 20:51:47.000000 pyaogmaneo-2.6.1/source/pyaogmaneo/py_image_encoder.h
--rw-r--r--   0 runner    (1001) docker     (127)    11773 2024-05-11 20:51:47.000000 pyaogmaneo-2.6.1/source/pyaogmaneo/py_module.cpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 23:34:17.280911 pyaogmaneo-2.6.2/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 23:34:17.276911 pyaogmaneo-2.6.2/CMake/
+-rw-r--r--   0 runner    (1001) docker     (127)     1250 2024-05-17 23:34:08.000000 pyaogmaneo-2.6.2/CMake/FindAOgmaNeo.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)     2237 2024-05-17 23:34:08.000000 pyaogmaneo-2.6.2/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    17842 2024-05-17 23:34:08.000000 pyaogmaneo-2.6.2/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-05-17 23:34:08.000000 pyaogmaneo-2.6.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      785 2024-05-17 23:34:17.280911 pyaogmaneo-2.6.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2415 2024-05-17 23:34:08.000000 pyaogmaneo-2.6.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 23:34:17.280911 pyaogmaneo-2.6.2/pyaogmaneo.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      785 2024-05-17 23:34:17.000000 pyaogmaneo-2.6.2/pyaogmaneo.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      505 2024-05-17 23:34:17.000000 pyaogmaneo-2.6.2/pyaogmaneo.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-17 23:34:17.000000 pyaogmaneo-2.6.2/pyaogmaneo.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-17 23:34:17.000000 pyaogmaneo-2.6.2/pyaogmaneo.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-17 23:34:17.000000 pyaogmaneo-2.6.2/pyaogmaneo.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-05-17 23:34:08.000000 pyaogmaneo-2.6.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-17 23:34:17.280911 pyaogmaneo-2.6.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     4253 2024-05-17 23:34:08.000000 pyaogmaneo-2.6.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 23:34:17.276911 pyaogmaneo-2.6.2/source/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 23:34:17.280911 pyaogmaneo-2.6.2/source/pyaogmaneo/
+-rw-r--r--   0 runner    (1001) docker     (127)     1153 2024-05-17 23:34:08.000000 pyaogmaneo-2.6.2/source/pyaogmaneo/py_helpers.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1953 2024-05-17 23:34:08.000000 pyaogmaneo-2.6.2/source/pyaogmaneo/py_helpers.h
+-rw-r--r--   0 runner    (1001) docker     (127)    12736 2024-05-17 23:34:08.000000 pyaogmaneo-2.6.2/source/pyaogmaneo/py_hierarchy.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     6861 2024-05-17 23:34:08.000000 pyaogmaneo-2.6.2/source/pyaogmaneo/py_hierarchy.h
+-rw-r--r--   0 runner    (1001) docker     (127)     7846 2024-05-17 23:34:08.000000 pyaogmaneo-2.6.2/source/pyaogmaneo/py_image_encoder.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3209 2024-05-17 23:34:08.000000 pyaogmaneo-2.6.2/source/pyaogmaneo/py_image_encoder.h
+-rw-r--r--   0 runner    (1001) docker     (127)    11641 2024-05-17 23:34:08.000000 pyaogmaneo-2.6.2/source/pyaogmaneo/py_module.cpp
```

### Comparing `pyaogmaneo-2.6.1/CMake/FindAOgmaNeo.cmake` & `pyaogmaneo-2.6.2/CMake/FindAOgmaNeo.cmake`

 * *Files identical despite different names*

### Comparing `pyaogmaneo-2.6.1/CMakeLists.txt` & `pyaogmaneo-2.6.2/CMakeLists.txt`

 * *Files 6% similar despite different names*

```diff
@@ -32,15 +32,15 @@
     find_package(AOgmaNeo)
 else()
     message(STATUS "Not using system installation of AOgmaNeo, will download from repository")
 
     FetchContent_Declare(
         AOgmaNeo
         GIT_REPOSITORY https://github.com/ogmacorp/AOgmaNeo.git
-        GIT_TAG 280df76544e206e9c585cfecbefb1707392cfadb
+        GIT_TAG bf753760db4b130b735f65571ad23e532d9861b9
     )
 
     FetchContent_MakeAvailable(AOgmaNeo)
 endif()
 
 FetchContent_Declare(
     pybind11
```

### Comparing `pyaogmaneo-2.6.1/LICENSE.md` & `pyaogmaneo-2.6.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pyaogmaneo-2.6.1/PKG-INFO` & `pyaogmaneo-2.6.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyaogmaneo
-Version: 2.6.1
+Version: 2.6.2
 Summary: Python bindings for the AOgmaNeo library
 Home-page: https://ogmacorp.com/
 Author: Ogma Intelligent Systems Corp
 Author-email: info@ogmacorp.com
 License: Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International License
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
```

### Comparing `pyaogmaneo-2.6.1/README.md` & `pyaogmaneo-2.6.2/README.md`

 * *Files identical despite different names*

### Comparing `pyaogmaneo-2.6.1/pyaogmaneo.egg-info/PKG-INFO` & `pyaogmaneo-2.6.2/pyaogmaneo.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyaogmaneo
-Version: 2.6.1
+Version: 2.6.2
 Summary: Python bindings for the AOgmaNeo library
 Home-page: https://ogmacorp.com/
 Author: Ogma Intelligent Systems Corp
 Author-email: info@ogmacorp.com
 License: Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International License
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
```

### Comparing `pyaogmaneo-2.6.1/setup.py` & `pyaogmaneo-2.6.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -84,15 +84,15 @@
             os.makedirs(self.build_temp)
 
         subprocess.check_call([ 'cmake', ext.sourcedir ] + cmake_args, cwd=self.build_temp, env=env)
         subprocess.check_call([ 'cmake', '--build', '.' ] + build_args, cwd=self.build_temp)
 
 setup(
     name="pyaogmaneo",
-    version="2.6.1",
+    version="2.6.2",
     description="Python bindings for the AOgmaNeo library",
     long_description='https://github.com/ogmacorp/PyAOgmaNeo',
     author='Ogma Intelligent Systems Corp',
     author_email='info@ogmacorp.com',
     url='https://ogmacorp.com/',
     license='Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International License',
     classifiers=[
```

### Comparing `pyaogmaneo-2.6.1/source/pyaogmaneo/py_helpers.cpp` & `pyaogmaneo-2.6.2/source/pyaogmaneo/py_helpers.cpp`

 * *Files identical despite different names*

### Comparing `pyaogmaneo-2.6.1/source/pyaogmaneo/py_helpers.h` & `pyaogmaneo-2.6.2/source/pyaogmaneo/py_helpers.h`

 * *Files identical despite different names*

### Comparing `pyaogmaneo-2.6.1/source/pyaogmaneo/py_hierarchy.cpp` & `pyaogmaneo-2.6.2/source/pyaogmaneo/py_hierarchy.cpp`

 * *Files identical despite different names*

### Comparing `pyaogmaneo-2.6.1/source/pyaogmaneo/py_hierarchy.h` & `pyaogmaneo-2.6.2/source/pyaogmaneo/py_hierarchy.h`

 * *Files identical despite different names*

### Comparing `pyaogmaneo-2.6.1/source/pyaogmaneo/py_image_encoder.cpp` & `pyaogmaneo-2.6.2/source/pyaogmaneo/py_image_encoder.cpp`

 * *Files identical despite different names*

### Comparing `pyaogmaneo-2.6.1/source/pyaogmaneo/py_image_encoder.h` & `pyaogmaneo-2.6.2/source/pyaogmaneo/py_image_encoder.h`

 * *Files identical despite different names*

### Comparing `pyaogmaneo-2.6.1/source/pyaogmaneo/py_module.cpp` & `pyaogmaneo-2.6.2/source/pyaogmaneo/py_module.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -94,19 +94,17 @@
                 return other;
             }
         );
 
     // bind params
     py::class_<aon::Encoder::Params>(m, "EncoderParams")
         .def(py::init<>())
-        .def_readwrite("choice", &aon::Encoder::Params::choice)
-        .def_readwrite("vigilance", &aon::Encoder::Params::vigilance)
+        .def_readwrite("scale", &aon::Encoder::Params::scale)
         .def_readwrite("lr", &aon::Encoder::Params::lr)
-        .def_readwrite("active_ratio", &aon::Encoder::Params::active_ratio)
-        .def_readwrite("l_radius", &aon::Encoder::Params::l_radius);
+        .def_readwrite("early_stop_cells", &aon::Encoder::Params::early_stop_cells);
 
     py::class_<aon::Decoder::Params>(m, "DecoderParams")
         .def(py::init<>())
         .def_readwrite("scale", &aon::Decoder::Params::scale)
         .def_readwrite("lr", &aon::Decoder::Params::lr)
         .def_readwrite("leak", &aon::Decoder::Params::leak);
```

