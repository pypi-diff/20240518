# Comparing `tmp/warp_python-1.1.2.tar.gz` & `tmp/warp_python-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "warp_python-1.1.2.tar", last modified: Sat May 18 14:28:27 2024, max compression
+gzip compressed data, was "warp_python-1.2.1.tar", last modified: Sat May 18 14:34:04 2024, max compression
```

## Comparing `warp_python-1.1.2.tar` & `warp_python-1.2.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 14:28:27.766344 warp_python-1.1.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-05-18 14:28:23.000000 warp_python-1.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      760 2024-05-18 14:28:27.766344 warp_python-1.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-05-18 14:28:23.000000 warp_python-1.1.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-18 14:28:27.766344 warp_python-1.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      987 2024-05-18 14:28:23.000000 warp_python-1.1.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 14:28:27.762344 warp_python-1.1.2/warp/
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-18 14:28:23.000000 warp_python-1.1.2/warp/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 14:28:27.766344 warp_python-1.1.2/warp/host/
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-18 14:28:23.000000 warp_python-1.1.2/warp/host/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4461 2024-05-18 14:28:23.000000 warp_python-1.1.2/warp/host/host.py
--rw-r--r--   0 runner    (1001) docker     (127)      812 2024-05-18 14:28:23.000000 warp_python-1.1.2/warp/resolve.py
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-18 14:28:23.000000 warp_python-1.1.2/warp/servers.py
--rw-r--r--   0 runner    (1001) docker     (127)      956 2024-05-18 14:28:23.000000 warp_python-1.1.2/warp/set_ip.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 14:28:27.766344 warp_python-1.1.2/warp_python.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      760 2024-05-18 14:28:27.000000 warp_python-1.1.2/warp_python.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      304 2024-05-18 14:28:27.000000 warp_python-1.1.2/warp_python.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-18 14:28:27.000000 warp_python-1.1.2/warp_python.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-18 14:28:27.000000 warp_python-1.1.2/warp_python.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-18 14:28:27.000000 warp_python-1.1.2/warp_python.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 14:34:04.232902 warp_python-1.2.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-05-18 14:33:58.000000 warp_python-1.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      760 2024-05-18 14:34:04.232902 warp_python-1.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-05-18 14:33:58.000000 warp_python-1.2.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-18 14:34:04.232902 warp_python-1.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      987 2024-05-18 14:33:58.000000 warp_python-1.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 14:34:04.228902 warp_python-1.2.1/warp/
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-05-18 14:33:58.000000 warp_python-1.2.1/warp/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 14:34:04.228902 warp_python-1.2.1/warp/host/
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-18 14:33:58.000000 warp_python-1.2.1/warp/host/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4461 2024-05-18 14:33:58.000000 warp_python-1.2.1/warp/host/host.py
+-rw-r--r--   0 runner    (1001) docker     (127)      812 2024-05-18 14:33:58.000000 warp_python-1.2.1/warp/resolve.py
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-18 14:33:58.000000 warp_python-1.2.1/warp/servers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      956 2024-05-18 14:33:58.000000 warp_python-1.2.1/warp/set_ip.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 14:34:04.232902 warp_python-1.2.1/warp_python.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      760 2024-05-18 14:34:04.000000 warp_python-1.2.1/warp_python.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      304 2024-05-18 14:34:04.000000 warp_python-1.2.1/warp_python.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-18 14:34:04.000000 warp_python-1.2.1/warp_python.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-18 14:34:04.000000 warp_python-1.2.1/warp_python.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-18 14:34:04.000000 warp_python-1.2.1/warp_python.egg-info/top_level.txt
```

### Comparing `warp_python-1.1.2/LICENSE` & `warp_python-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `warp_python-1.1.2/PKG-INFO` & `warp_python-1.2.1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: warp-python
-Version: 1.1.2
+Version: 1.2.1
 Summary: A python module for WARP
 Home-page: https://github.com/warp-project/warp-python
 Author: warp-project
 Author-email: simon.c.gilde@gmail.com
 Keywords: warp
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `warp_python-1.1.2/setup.py` & `warp_python-1.2.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 import os
 
 with open("README.md", encoding="utf-8") as f:
     long_description = f.read()
     
-VERSION = '1.1.2'
+VERSION = '1.2.1'
 
 setup(
     name='warp-python',
     version=VERSION,
     author='warp-project',
     author_email='simon.c.gilde@gmail.com',
     description='A python module for WARP',
```

### Comparing `warp_python-1.1.2/warp/host/host.py` & `warp_python-1.2.1/warp/host/host.py`

 * *Files identical despite different names*

### Comparing `warp_python-1.1.2/warp/resolve.py` & `warp_python-1.2.1/warp/resolve.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     domain = domain.removesuffix("<warp>").split(".")
     tld = domain.pop(-1)
     try:
         server = SERVERS[tld]
     except KeyError:
         raise ValueError("No such TLD.")
     try:
-        resp = requests.get(f"https://{server}/resolve/{".".join(domain)}.{tld}/", timeout=5).json()
+        resp = requests.get(f"https://{server}/resolve/{'.'.join(domain)}.{tld}/", timeout=5).json()
     except TimeoutError:
         raise TimeoutError("Server could not be reached.")
     try:
         assert resp.get("SUCCESS")
     except AssertionError:
         reason = resp.get("REASON")
         if reason == "Domain doesn't exist":
```

### Comparing `warp_python-1.1.2/warp/set_ip.py` & `warp_python-1.2.1/warp/set_ip.py`

 * *Files identical despite different names*

### Comparing `warp_python-1.1.2/warp_python.egg-info/PKG-INFO` & `warp_python-1.2.1/warp_python.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: warp-python
-Version: 1.1.2
+Version: 1.2.1
 Summary: A python module for WARP
 Home-page: https://github.com/warp-project/warp-python
 Author: warp-project
 Author-email: simon.c.gilde@gmail.com
 Keywords: warp
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

