# Comparing `tmp/warp_python-1.2.6.tar.gz` & `tmp/warp_python-1.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "warp_python-1.2.6.tar", last modified: Sat May 18 15:25:44 2024, max compression
+gzip compressed data, was "warp_python-1.2.7.tar", last modified: Sat May 18 15:29:02 2024, max compression
```

## Comparing `warp_python-1.2.6.tar` & `warp_python-1.2.7.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 15:25:44.187384 warp_python-1.2.6/
--rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-05-18 15:25:40.000000 warp_python-1.2.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      760 2024-05-18 15:25:44.187384 warp_python-1.2.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-05-18 15:25:40.000000 warp_python-1.2.6/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-18 15:25:44.187384 warp_python-1.2.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      987 2024-05-18 15:25:40.000000 warp_python-1.2.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 15:25:44.183384 warp_python-1.2.6/warp/
--rw-r--r--   0 runner    (1001) docker     (127)      116 2024-05-18 15:25:40.000000 warp_python-1.2.6/warp/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 15:25:44.187384 warp_python-1.2.6/warp/host/
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-18 15:25:40.000000 warp_python-1.2.6/warp/host/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4461 2024-05-18 15:25:40.000000 warp_python-1.2.6/warp/host/host.py
--rw-r--r--   0 runner    (1001) docker     (127)      813 2024-05-18 15:25:40.000000 warp_python-1.2.6/warp/resolve.py
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-05-18 15:25:40.000000 warp_python-1.2.6/warp/servers.py
--rw-r--r--   0 runner    (1001) docker     (127)      957 2024-05-18 15:25:40.000000 warp_python-1.2.6/warp/set_ip.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 15:25:44.187384 warp_python-1.2.6/warp_python.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      760 2024-05-18 15:25:44.000000 warp_python-1.2.6/warp_python.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      304 2024-05-18 15:25:44.000000 warp_python-1.2.6/warp_python.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-18 15:25:44.000000 warp_python-1.2.6/warp_python.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-18 15:25:44.000000 warp_python-1.2.6/warp_python.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-18 15:25:44.000000 warp_python-1.2.6/warp_python.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 15:29:02.325871 warp_python-1.2.7/
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-05-18 15:28:58.000000 warp_python-1.2.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      796 2024-05-18 15:29:02.325871 warp_python-1.2.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-05-18 15:28:58.000000 warp_python-1.2.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-18 15:29:02.325871 warp_python-1.2.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1023 2024-05-18 15:28:58.000000 warp_python-1.2.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 15:29:02.321871 warp_python-1.2.7/warp/
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-05-18 15:28:58.000000 warp_python-1.2.7/warp/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 15:29:02.325871 warp_python-1.2.7/warp/host/
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-18 15:28:58.000000 warp_python-1.2.7/warp/host/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4461 2024-05-18 15:28:58.000000 warp_python-1.2.7/warp/host/host.py
+-rw-r--r--   0 runner    (1001) docker     (127)      813 2024-05-18 15:28:58.000000 warp_python-1.2.7/warp/resolve.py
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-05-18 15:28:58.000000 warp_python-1.2.7/warp/servers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      957 2024-05-18 15:28:58.000000 warp_python-1.2.7/warp/set_ip.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 15:29:02.325871 warp_python-1.2.7/warp_python.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      796 2024-05-18 15:29:02.000000 warp_python-1.2.7/warp_python.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      304 2024-05-18 15:29:02.000000 warp_python-1.2.7/warp_python.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-18 15:29:02.000000 warp_python-1.2.7/warp_python.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-18 15:29:02.000000 warp_python-1.2.7/warp_python.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-18 15:29:02.000000 warp_python-1.2.7/warp_python.egg-info/top_level.txt
```

### Comparing `warp_python-1.2.6/LICENSE` & `warp_python-1.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `warp_python-1.2.6/PKG-INFO` & `warp_python-1.2.7/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: warp-python
-Version: 1.2.6
+Version: 1.2.7
 Summary: A python module for WARP
 Home-page: https://github.com/warp-project/warp-python
-Author: warp-project
-Author-email: simon.c.gilde@gmail.com
+Author: warp-project, Ryan_shamu
+Author-email: simon.c.gilde@gmail.com, ryanshamu418@gmail.com
 Keywords: warp
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `warp_python-1.2.6/setup.py` & `warp_python-1.2.7/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 from setuptools import setup, find_packages
 import os
 
 with open("README.md", encoding="utf-8") as f:
     long_description = f.read()
     
-VERSION = '1.2.6'
+VERSION = '1.2.7'
 
 setup(
     name='warp-python',
     version=VERSION,
-    author='warp-project',
-    author_email='simon.c.gilde@gmail.com',
+    author='warp-project, Ryan_shamu',
+    author_email='simon.c.gilde@gmail.com, ryanshamu418@gmail.com',
     description='A python module for WARP',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/warp-project/warp-python',
     packages=find_packages(exclude=[]),
     classifiers=[
         'Development Status :: 4 - Beta',
```

### Comparing `warp_python-1.2.6/warp/host/host.py` & `warp_python-1.2.7/warp/host/host.py`

 * *Files identical despite different names*

### Comparing `warp_python-1.2.6/warp/resolve.py` & `warp_python-1.2.7/warp/resolve.py`

 * *Files identical despite different names*

### Comparing `warp_python-1.2.6/warp/set_ip.py` & `warp_python-1.2.7/warp/set_ip.py`

 * *Files identical despite different names*

### Comparing `warp_python-1.2.6/warp_python.egg-info/PKG-INFO` & `warp_python-1.2.7/warp_python.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: warp-python
-Version: 1.2.6
+Version: 1.2.7
 Summary: A python module for WARP
 Home-page: https://github.com/warp-project/warp-python
-Author: warp-project
-Author-email: simon.c.gilde@gmail.com
+Author: warp-project, Ryan_shamu
+Author-email: simon.c.gilde@gmail.com, ryanshamu418@gmail.com
 Keywords: warp
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

