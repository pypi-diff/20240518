# Comparing `tmp/adb-tool-py-0.0.4.tar.gz` & `tmp/adb-tool-py-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adb-tool-py-0.0.4.tar", last modified: Tue May 14 13:50:53 2024, max compression
+gzip compressed data, was "adb-tool-py-0.1.0.tar", last modified: Fri May 17 23:28:24 2024, max compression
```

## Comparing `adb-tool-py-0.0.4.tar` & `adb-tool-py-0.1.0.tar`

### file list

```diff
@@ -1,21 +1,22 @@
-drwxr-xr-x   0 iuchi      (501) staff       (20)        0 2024-05-14 13:50:53.754391 adb-tool-py-0.0.4/
--rw-r--r--   0 iuchi      (501) staff       (20)     1068 2024-05-14 11:56:34.000000 adb-tool-py-0.0.4/LICENSE
--rw-r--r--   0 iuchi      (501) staff       (20)       34 2024-05-12 13:08:55.000000 adb-tool-py-0.0.4/MANIFEST.in
--rw-r--r--   0 iuchi      (501) staff       (20)     1310 2024-05-14 13:50:53.754252 adb-tool-py-0.0.4/PKG-INFO
--rw-r--r--   0 iuchi      (501) staff       (20)      878 2024-05-14 13:36:26.000000 adb-tool-py-0.0.4/README.md
-drwxr-xr-x   0 iuchi      (501) staff       (20)        0 2024-05-14 13:50:53.753182 adb-tool-py-0.0.4/adb_tool_py/
--rw-r--r--   0 iuchi      (501) staff       (20)      175 2024-05-13 13:35:05.000000 adb-tool-py-0.0.4/adb_tool_py/__init__.py
--rw-r--r--   0 iuchi      (501) staff       (20)     1906 2024-05-14 13:14:27.000000 adb-tool-py-0.0.4/adb_tool_py/adb_command.py
--rw-r--r--   0 iuchi      (501) staff       (20)       91 2024-05-13 13:07:27.000000 adb-tool-py-0.0.4/adb_tool_py/adb_device.py
--rw-r--r--   0 iuchi      (501) staff       (20)     3347 2024-05-14 13:35:03.000000 adb-tool-py-0.0.4/adb_tool_py/adb_tool.py
--rw-r--r--   0 iuchi      (501) staff       (20)     4313 2024-05-14 13:12:28.000000 adb-tool-py-0.0.4/adb_tool_py/adb_view_tree.py
--rw-r--r--   0 iuchi      (501) staff       (20)      468 2024-05-12 12:33:36.000000 adb-tool-py-0.0.4/adb_tool_py/command.py
--rw-r--r--   0 iuchi      (501) staff       (20)     2371 2024-05-14 13:13:37.000000 adb-tool-py-0.0.4/adb_tool_py/ui_node.py
-drwxr-xr-x   0 iuchi      (501) staff       (20)        0 2024-05-14 13:50:53.753801 adb-tool-py-0.0.4/adb_tool_py.egg-info/
--rw-r--r--   0 iuchi      (501) staff       (20)     1310 2024-05-14 13:50:53.000000 adb-tool-py-0.0.4/adb_tool_py.egg-info/PKG-INFO
--rw-r--r--   0 iuchi      (501) staff       (20)      388 2024-05-14 13:50:53.000000 adb-tool-py-0.0.4/adb_tool_py.egg-info/SOURCES.txt
--rw-r--r--   0 iuchi      (501) staff       (20)        1 2024-05-14 13:50:53.000000 adb-tool-py-0.0.4/adb_tool_py.egg-info/dependency_links.txt
--rw-r--r--   0 iuchi      (501) staff       (20)        8 2024-05-14 13:50:53.000000 adb-tool-py-0.0.4/adb_tool_py.egg-info/requires.txt
--rw-r--r--   0 iuchi      (501) staff       (20)       12 2024-05-14 13:50:53.000000 adb-tool-py-0.0.4/adb_tool_py.egg-info/top_level.txt
--rw-r--r--   0 iuchi      (501) staff       (20)       38 2024-05-14 13:50:53.754436 adb-tool-py-0.0.4/setup.cfg
--rw-r--r--   0 iuchi      (501) staff       (20)      677 2024-05-14 13:18:17.000000 adb-tool-py-0.0.4/setup.py
+drwxr-xr-x   0 iuchi      (501) staff       (20)        0 2024-05-17 23:28:24.512888 adb-tool-py-0.1.0/
+-rw-r--r--   0 iuchi      (501) staff       (20)     1068 2024-05-14 11:56:34.000000 adb-tool-py-0.1.0/LICENSE
+-rw-r--r--   0 iuchi      (501) staff       (20)       34 2024-05-12 13:08:55.000000 adb-tool-py-0.1.0/MANIFEST.in
+-rw-r--r--   0 iuchi      (501) staff       (20)     1310 2024-05-17 23:28:24.512773 adb-tool-py-0.1.0/PKG-INFO
+-rw-r--r--   0 iuchi      (501) staff       (20)      878 2024-05-14 13:55:58.000000 adb-tool-py-0.1.0/README.md
+drwxr-xr-x   0 iuchi      (501) staff       (20)        0 2024-05-17 23:28:24.511972 adb-tool-py-0.1.0/adb_tool_py/
+-rw-r--r--   0 iuchi      (501) staff       (20)      212 2024-05-17 12:42:08.000000 adb-tool-py-0.1.0/adb_tool_py/__init__.py
+-rw-r--r--   0 iuchi      (501) staff       (20)     4502 2024-05-17 13:03:28.000000 adb-tool-py-0.1.0/adb_tool_py/adb_command.py
+-rw-r--r--   0 iuchi      (501) staff       (20)      334 2024-05-17 13:03:43.000000 adb-tool-py-0.1.0/adb_tool_py/adb_device.py
+-rw-r--r--   0 iuchi      (501) staff       (20)     8684 2024-05-17 14:12:06.000000 adb-tool-py-0.1.0/adb_tool_py/adb_image_cv.py
+-rw-r--r--   0 iuchi      (501) staff       (20)    13311 2024-05-17 14:09:24.000000 adb-tool-py-0.1.0/adb_tool_py/adb_tool.py
+-rw-r--r--   0 iuchi      (501) staff       (20)     8759 2024-05-17 13:15:51.000000 adb-tool-py-0.1.0/adb_tool_py/adb_view_tree.py
+-rw-r--r--   0 iuchi      (501) staff       (20)     1170 2024-05-17 13:04:06.000000 adb-tool-py-0.1.0/adb_tool_py/command.py
+-rw-r--r--   0 iuchi      (501) staff       (20)     3544 2024-05-17 12:37:04.000000 adb-tool-py-0.1.0/adb_tool_py/ui_node.py
+drwxr-xr-x   0 iuchi      (501) staff       (20)        0 2024-05-17 23:28:24.512630 adb-tool-py-0.1.0/adb_tool_py.egg-info/
+-rw-r--r--   0 iuchi      (501) staff       (20)     1310 2024-05-17 23:28:24.000000 adb-tool-py-0.1.0/adb_tool_py.egg-info/PKG-INFO
+-rw-r--r--   0 iuchi      (501) staff       (20)      416 2024-05-17 23:28:24.000000 adb-tool-py-0.1.0/adb_tool_py.egg-info/SOURCES.txt
+-rw-r--r--   0 iuchi      (501) staff       (20)        1 2024-05-17 23:28:24.000000 adb-tool-py-0.1.0/adb_tool_py.egg-info/dependency_links.txt
+-rw-r--r--   0 iuchi      (501) staff       (20)       22 2024-05-17 23:28:24.000000 adb-tool-py-0.1.0/adb_tool_py.egg-info/requires.txt
+-rw-r--r--   0 iuchi      (501) staff       (20)       12 2024-05-17 23:28:24.000000 adb-tool-py-0.1.0/adb_tool_py.egg-info/top_level.txt
+-rw-r--r--   0 iuchi      (501) staff       (20)       38 2024-05-17 23:28:24.512923 adb-tool-py-0.1.0/setup.cfg
+-rw-r--r--   0 iuchi      (501) staff       (20)      702 2024-05-17 23:28:04.000000 adb-tool-py-0.1.0/setup.py
```

### Comparing `adb-tool-py-0.0.4/LICENSE` & `adb-tool-py-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `adb-tool-py-0.0.4/PKG-INFO` & `adb-tool-py-0.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adb-tool-py
-Version: 0.0.4
+Version: 0.1.0
 Summary: adb-tool-py is a tool for Android Debug Bridge (adb).
 Home-page: https://github.com/ShotaIuchi/adb-tool-py
 Author: Shota Iuchi
 Author-email: shotaiuchi.develop@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `adb-tool-py-0.0.4/README.md` & `adb-tool-py-0.1.0/README.md`

 * *Files identical despite different names*

### Comparing `adb-tool-py-0.0.4/adb_tool_py.egg-info/PKG-INFO` & `adb-tool-py-0.1.0/adb_tool_py.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adb-tool-py
-Version: 0.0.4
+Version: 0.1.0
 Summary: adb-tool-py is a tool for Android Debug Bridge (adb).
 Home-page: https://github.com/ShotaIuchi/adb-tool-py
 Author: Shota Iuchi
 Author-email: shotaiuchi.develop@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `adb-tool-py-0.0.4/setup.py` & `adb-tool-py-0.1.0/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='adb-tool-py',
-    version='0.0.4',
+    version='0.1.0',
     author='Shota Iuchi',
     author_email='shotaiuchi.develop@gmail.com',
     description='adb-tool-py is a tool for Android Debug Bridge (adb).',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/ShotaIuchi/adb-tool-py',
     license='MIT',
@@ -14,10 +14,11 @@
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
     ],
     python_requires='>=3.6',
     install_requires=[
         'chardet',
+        'opencv-python',
     ],
     include_package_data=True
 )
```

