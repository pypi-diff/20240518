# Comparing `tmp/warp_python-1.2.7.tar.gz` & `tmp/warp_python-1.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "warp_python-1.2.7.tar", last modified: Sat May 18 15:29:02 2024, max compression
+gzip compressed data, was "warp_python-1.2.8.tar", last modified: Sat May 18 15:31:06 2024, max compression
```

## Comparing `warp_python-1.2.7.tar` & `warp_python-1.2.8.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 15:29:02.325871 warp_python-1.2.7/
--rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-05-18 15:28:58.000000 warp_python-1.2.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      796 2024-05-18 15:29:02.325871 warp_python-1.2.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-05-18 15:28:58.000000 warp_python-1.2.7/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-18 15:29:02.325871 warp_python-1.2.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1023 2024-05-18 15:28:58.000000 warp_python-1.2.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 15:29:02.321871 warp_python-1.2.7/warp/
--rw-r--r--   0 runner    (1001) docker     (127)      116 2024-05-18 15:28:58.000000 warp_python-1.2.7/warp/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 15:29:02.325871 warp_python-1.2.7/warp/host/
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-18 15:28:58.000000 warp_python-1.2.7/warp/host/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4461 2024-05-18 15:28:58.000000 warp_python-1.2.7/warp/host/host.py
--rw-r--r--   0 runner    (1001) docker     (127)      813 2024-05-18 15:28:58.000000 warp_python-1.2.7/warp/resolve.py
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-05-18 15:28:58.000000 warp_python-1.2.7/warp/servers.py
--rw-r--r--   0 runner    (1001) docker     (127)      957 2024-05-18 15:28:58.000000 warp_python-1.2.7/warp/set_ip.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 15:29:02.325871 warp_python-1.2.7/warp_python.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      796 2024-05-18 15:29:02.000000 warp_python-1.2.7/warp_python.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      304 2024-05-18 15:29:02.000000 warp_python-1.2.7/warp_python.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-18 15:29:02.000000 warp_python-1.2.7/warp_python.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-18 15:29:02.000000 warp_python-1.2.7/warp_python.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-18 15:29:02.000000 warp_python-1.2.7/warp_python.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 15:31:06.790283 warp_python-1.2.8/
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-05-18 15:31:01.000000 warp_python-1.2.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      796 2024-05-18 15:31:06.790283 warp_python-1.2.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-05-18 15:31:01.000000 warp_python-1.2.8/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-18 15:31:06.790283 warp_python-1.2.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1023 2024-05-18 15:31:01.000000 warp_python-1.2.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 15:31:06.786283 warp_python-1.2.8/warp/
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-05-18 15:31:01.000000 warp_python-1.2.8/warp/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 15:31:06.786283 warp_python-1.2.8/warp/host/
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-18 15:31:01.000000 warp_python-1.2.8/warp/host/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4463 2024-05-18 15:31:01.000000 warp_python-1.2.8/warp/host/host.py
+-rw-r--r--   0 runner    (1001) docker     (127)      813 2024-05-18 15:31:01.000000 warp_python-1.2.8/warp/resolve.py
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-05-18 15:31:01.000000 warp_python-1.2.8/warp/servers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      957 2024-05-18 15:31:01.000000 warp_python-1.2.8/warp/set_ip.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 15:31:06.790283 warp_python-1.2.8/warp_python.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      796 2024-05-18 15:31:06.000000 warp_python-1.2.8/warp_python.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      304 2024-05-18 15:31:06.000000 warp_python-1.2.8/warp_python.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-18 15:31:06.000000 warp_python-1.2.8/warp_python.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-18 15:31:06.000000 warp_python-1.2.8/warp_python.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-18 15:31:06.000000 warp_python-1.2.8/warp_python.egg-info/top_level.txt
```

### Comparing `warp_python-1.2.7/LICENSE` & `warp_python-1.2.8/LICENSE`

 * *Files identical despite different names*

### Comparing `warp_python-1.2.7/PKG-INFO` & `warp_python-1.2.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: warp-python
-Version: 1.2.7
+Version: 1.2.8
 Summary: A python module for WARP
 Home-page: https://github.com/warp-project/warp-python
 Author: warp-project, Ryan_shamu
 Author-email: simon.c.gilde@gmail.com, ryanshamu418@gmail.com
 Keywords: warp
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `warp_python-1.2.7/setup.py` & `warp_python-1.2.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 import os
 
 with open("README.md", encoding="utf-8") as f:
     long_description = f.read()
     
-VERSION = '1.2.7'
+VERSION = '1.2.8'
 
 setup(
     name='warp-python',
     version=VERSION,
     author='warp-project, Ryan_shamu',
     author_email='simon.c.gilde@gmail.com, ryanshamu418@gmail.com',
     description='A python module for WARP',
```

### Comparing `warp_python-1.2.7/warp/host/host.py` & `warp_python-1.2.8/warp/host/host.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
     tlds : list[str]
     events : dict[str, list[FunctionType]]
     
     def __init__(self, *, app : Flask, tld : str = None, tlds : list[str] = None, domains : dict[str, dict[str, Union[str, int]]] = None):
         self.app = app
         self.domains = domains or {}
         self.tlds = tlds or [tld]
-        self.tlds = [tld.strip(".") for tld in self.tlds]
+        self.tlds = [_tld.strip(".") for _tld in self.tlds]
         try:
             assert tld or tlds
         except AssertionError:
             raise ValueError("Pass either tld or tlds")
         @app.get("/resolve/<domain_name>/")
         def resolve_domain(domain_name : str):
             if not domain_name.endswith("."+tld):
```

### Comparing `warp_python-1.2.7/warp/resolve.py` & `warp_python-1.2.8/warp/resolve.py`

 * *Files identical despite different names*

### Comparing `warp_python-1.2.7/warp/set_ip.py` & `warp_python-1.2.8/warp/set_ip.py`

 * *Files identical despite different names*

### Comparing `warp_python-1.2.7/warp_python.egg-info/PKG-INFO` & `warp_python-1.2.8/warp_python.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: warp-python
-Version: 1.2.7
+Version: 1.2.8
 Summary: A python module for WARP
 Home-page: https://github.com/warp-project/warp-python
 Author: warp-project, Ryan_shamu
 Author-email: simon.c.gilde@gmail.com, ryanshamu418@gmail.com
 Keywords: warp
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

