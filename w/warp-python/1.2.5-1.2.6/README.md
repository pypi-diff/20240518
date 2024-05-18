# Comparing `tmp/warp_python-1.2.5.tar.gz` & `tmp/warp_python-1.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "warp_python-1.2.5.tar", last modified: Sat May 18 15:23:16 2024, max compression
+gzip compressed data, was "warp_python-1.2.6.tar", last modified: Sat May 18 15:25:44 2024, max compression
```

## Comparing `warp_python-1.2.5.tar` & `warp_python-1.2.6.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 15:23:16.214152 warp_python-1.2.5/
--rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-05-18 15:23:12.000000 warp_python-1.2.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      760 2024-05-18 15:23:16.214152 warp_python-1.2.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-05-18 15:23:12.000000 warp_python-1.2.5/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-18 15:23:16.214152 warp_python-1.2.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      987 2024-05-18 15:23:12.000000 warp_python-1.2.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 15:23:16.214152 warp_python-1.2.5/warp/
--rw-r--r--   0 runner    (1001) docker     (127)      116 2024-05-18 15:23:12.000000 warp_python-1.2.5/warp/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 15:23:16.214152 warp_python-1.2.5/warp/host/
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-18 15:23:12.000000 warp_python-1.2.5/warp/host/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4461 2024-05-18 15:23:12.000000 warp_python-1.2.5/warp/host/host.py
--rw-r--r--   0 runner    (1001) docker     (127)      812 2024-05-18 15:23:12.000000 warp_python-1.2.5/warp/resolve.py
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-05-18 15:23:12.000000 warp_python-1.2.5/warp/servers.py
--rw-r--r--   0 runner    (1001) docker     (127)      956 2024-05-18 15:23:12.000000 warp_python-1.2.5/warp/set_ip.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 15:23:16.214152 warp_python-1.2.5/warp_python.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      760 2024-05-18 15:23:16.000000 warp_python-1.2.5/warp_python.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      304 2024-05-18 15:23:16.000000 warp_python-1.2.5/warp_python.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-18 15:23:16.000000 warp_python-1.2.5/warp_python.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-18 15:23:16.000000 warp_python-1.2.5/warp_python.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-18 15:23:16.000000 warp_python-1.2.5/warp_python.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 15:25:44.187384 warp_python-1.2.6/
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-05-18 15:25:40.000000 warp_python-1.2.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      760 2024-05-18 15:25:44.187384 warp_python-1.2.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-05-18 15:25:40.000000 warp_python-1.2.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-18 15:25:44.187384 warp_python-1.2.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      987 2024-05-18 15:25:40.000000 warp_python-1.2.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 15:25:44.183384 warp_python-1.2.6/warp/
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-05-18 15:25:40.000000 warp_python-1.2.6/warp/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 15:25:44.187384 warp_python-1.2.6/warp/host/
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-18 15:25:40.000000 warp_python-1.2.6/warp/host/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4461 2024-05-18 15:25:40.000000 warp_python-1.2.6/warp/host/host.py
+-rw-r--r--   0 runner    (1001) docker     (127)      813 2024-05-18 15:25:40.000000 warp_python-1.2.6/warp/resolve.py
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-05-18 15:25:40.000000 warp_python-1.2.6/warp/servers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      957 2024-05-18 15:25:40.000000 warp_python-1.2.6/warp/set_ip.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 15:25:44.187384 warp_python-1.2.6/warp_python.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      760 2024-05-18 15:25:44.000000 warp_python-1.2.6/warp_python.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      304 2024-05-18 15:25:44.000000 warp_python-1.2.6/warp_python.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-18 15:25:44.000000 warp_python-1.2.6/warp_python.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-18 15:25:44.000000 warp_python-1.2.6/warp_python.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-18 15:25:44.000000 warp_python-1.2.6/warp_python.egg-info/top_level.txt
```

### Comparing `warp_python-1.2.5/LICENSE` & `warp_python-1.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `warp_python-1.2.5/PKG-INFO` & `warp_python-1.2.6/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: warp-python
-Version: 1.2.5
+Version: 1.2.6
 Summary: A python module for WARP
 Home-page: https://github.com/warp-project/warp-python
 Author: warp-project
 Author-email: simon.c.gilde@gmail.com
 Keywords: warp
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `warp_python-1.2.5/setup.py` & `warp_python-1.2.6/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 import os
 
 with open("README.md", encoding="utf-8") as f:
     long_description = f.read()
     
-VERSION = '1.2.5'
+VERSION = '1.2.6'
 
 setup(
     name='warp-python',
     version=VERSION,
     author='warp-project',
     author_email='simon.c.gilde@gmail.com',
     description='A python module for WARP',
```

### Comparing `warp_python-1.2.5/warp/host/host.py` & `warp_python-1.2.6/warp/host/host.py`

 * *Files identical despite different names*

### Comparing `warp_python-1.2.5/warp/resolve.py` & `warp_python-1.2.6/warp/resolve.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
 For resolving domains
 """
 import requests
-from servers import SERVERS
+from .servers import SERVERS
 
 def resolve(domain : str) -> list[tuple[str, int]]:
     domain = domain.removesuffix("<warp>").split(".")
     tld = domain.pop(-1)
     try:
         server = SERVERS[tld]
     except KeyError:
```

### Comparing `warp_python-1.2.5/warp/set_ip.py` & `warp_python-1.2.6/warp/set_ip.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
 Set an ip of a domain
 """
 import requests
-from servers import SERVERS
+from .servers import SERVERS
 
 def set_ip(*, domain_name, ip, key):
     domain = domain_name
     domain = domain.removesuffix("<warp>").split(".")
     tld = domain.pop(-1)
     try:
         server = SERVERS[tld]
```

### Comparing `warp_python-1.2.5/warp_python.egg-info/PKG-INFO` & `warp_python-1.2.6/warp_python.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: warp-python
-Version: 1.2.5
+Version: 1.2.6
 Summary: A python module for WARP
 Home-page: https://github.com/warp-project/warp-python
 Author: warp-project
 Author-email: simon.c.gilde@gmail.com
 Keywords: warp
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

