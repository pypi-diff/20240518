# Comparing `tmp/warp_python-1.2.3.tar.gz` & `tmp/warp_python-1.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "warp_python-1.2.3.tar", last modified: Sat May 18 14:42:32 2024, max compression
+gzip compressed data, was "warp_python-1.2.4.tar", last modified: Sat May 18 14:47:41 2024, max compression
```

## Comparing `warp_python-1.2.3.tar` & `warp_python-1.2.4.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 14:42:32.719762 warp_python-1.2.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-05-18 14:42:29.000000 warp_python-1.2.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      760 2024-05-18 14:42:32.719762 warp_python-1.2.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-05-18 14:42:29.000000 warp_python-1.2.3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-18 14:42:32.719762 warp_python-1.2.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      987 2024-05-18 14:42:29.000000 warp_python-1.2.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 14:42:32.719762 warp_python-1.2.3/warp/
--rw-r--r--   0 runner    (1001) docker     (127)      116 2024-05-18 14:42:29.000000 warp_python-1.2.3/warp/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 14:42:32.719762 warp_python-1.2.3/warp/host/
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-18 14:42:29.000000 warp_python-1.2.3/warp/host/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4461 2024-05-18 14:42:29.000000 warp_python-1.2.3/warp/host/host.py
--rw-r--r--   0 runner    (1001) docker     (127)      812 2024-05-18 14:42:29.000000 warp_python-1.2.3/warp/resolve.py
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-18 14:42:29.000000 warp_python-1.2.3/warp/servers.py
--rw-r--r--   0 runner    (1001) docker     (127)      957 2024-05-18 14:42:29.000000 warp_python-1.2.3/warp/set_ip.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 14:42:32.719762 warp_python-1.2.3/warp_python.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      760 2024-05-18 14:42:32.000000 warp_python-1.2.3/warp_python.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      304 2024-05-18 14:42:32.000000 warp_python-1.2.3/warp_python.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-18 14:42:32.000000 warp_python-1.2.3/warp_python.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-18 14:42:32.000000 warp_python-1.2.3/warp_python.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-18 14:42:32.000000 warp_python-1.2.3/warp_python.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 14:47:41.780461 warp_python-1.2.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-05-18 14:47:38.000000 warp_python-1.2.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      760 2024-05-18 14:47:41.780461 warp_python-1.2.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-05-18 14:47:38.000000 warp_python-1.2.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-18 14:47:41.780461 warp_python-1.2.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      987 2024-05-18 14:47:38.000000 warp_python-1.2.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 14:47:41.780461 warp_python-1.2.4/warp/
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-05-18 14:47:38.000000 warp_python-1.2.4/warp/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 14:47:41.780461 warp_python-1.2.4/warp/host/
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-18 14:47:38.000000 warp_python-1.2.4/warp/host/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4461 2024-05-18 14:47:38.000000 warp_python-1.2.4/warp/host/host.py
+-rw-r--r--   0 runner    (1001) docker     (127)      812 2024-05-18 14:47:38.000000 warp_python-1.2.4/warp/resolve.py
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-18 14:47:38.000000 warp_python-1.2.4/warp/servers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      957 2024-05-18 14:47:38.000000 warp_python-1.2.4/warp/set_ip.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 14:47:41.780461 warp_python-1.2.4/warp_python.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      760 2024-05-18 14:47:41.000000 warp_python-1.2.4/warp_python.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      304 2024-05-18 14:47:41.000000 warp_python-1.2.4/warp_python.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-18 14:47:41.000000 warp_python-1.2.4/warp_python.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-18 14:47:41.000000 warp_python-1.2.4/warp_python.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-18 14:47:41.000000 warp_python-1.2.4/warp_python.egg-info/top_level.txt
```

### Comparing `warp_python-1.2.3/LICENSE` & `warp_python-1.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `warp_python-1.2.3/PKG-INFO` & `warp_python-1.2.4/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: warp-python
-Version: 1.2.3
+Version: 1.2.4
 Summary: A python module for WARP
 Home-page: https://github.com/warp-project/warp-python
 Author: warp-project
 Author-email: simon.c.gilde@gmail.com
 Keywords: warp
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `warp_python-1.2.3/setup.py` & `warp_python-1.2.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 import os
 
 with open("README.md", encoding="utf-8") as f:
     long_description = f.read()
     
-VERSION = '1.2.3'
+VERSION = '1.2.4'
 
 setup(
     name='warp-python',
     version=VERSION,
     author='warp-project',
     author_email='simon.c.gilde@gmail.com',
     description='A python module for WARP',
```

### Comparing `warp_python-1.2.3/warp/host/host.py` & `warp_python-1.2.4/warp/host/host.py`

 * *Files identical despite different names*

### Comparing `warp_python-1.2.3/warp/resolve.py` & `warp_python-1.2.4/warp/resolve.py`

 * *Files identical despite different names*

### Comparing `warp_python-1.2.3/warp/set_ip.py` & `warp_python-1.2.4/warp/set_ip.py`

 * *Files identical despite different names*

### Comparing `warp_python-1.2.3/warp_python.egg-info/PKG-INFO` & `warp_python-1.2.4/warp_python.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: warp-python
-Version: 1.2.3
+Version: 1.2.4
 Summary: A python module for WARP
 Home-page: https://github.com/warp-project/warp-python
 Author: warp-project
 Author-email: simon.c.gilde@gmail.com
 Keywords: warp
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

