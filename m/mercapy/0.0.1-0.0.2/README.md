# Comparing `tmp/mercapy-0.0.1.tar.gz` & `tmp/mercapy-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mercapy-0.0.1.tar", last modified: Fri May 17 11:31:00 2024, max compression
+gzip compressed data, was "mercapy-0.0.2.tar", last modified: Sat May 18 19:33:53 2024, max compression
```

## Comparing `mercapy-0.0.1.tar` & `mercapy-0.0.2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 11:31:00.236102 mercapy-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-05-17 11:30:55.000000 mercapy-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2426 2024-05-17 11:31:00.236102 mercapy-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1856 2024-05-17 11:30:55.000000 mercapy-0.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 11:31:00.232102 mercapy-0.0.1/mercapy/
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-17 11:30:55.000000 mercapy-0.0.1/mercapy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-17 11:30:55.000000 mercapy-0.0.1/mercapy/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 11:31:00.232102 mercapy-0.0.1/mercapy/exceptions/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 11:30:55.000000 mercapy-0.0.1/mercapy/exceptions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      342 2024-05-17 11:30:55.000000 mercapy-0.0.1/mercapy/exceptions/product.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 11:30:55.000000 mercapy-0.0.1/mercapy/merca.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 11:31:00.232102 mercapy-0.0.1/mercapy/product/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 11:30:55.000000 mercapy-0.0.1/mercapy/product/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1236 2024-05-17 11:30:55.000000 mercapy-0.0.1/mercapy/product/photo.py
--rw-r--r--   0 runner    (1001) docker     (127)     3395 2024-05-17 11:30:55.000000 mercapy-0.0.1/mercapy/product.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 11:31:00.232102 mercapy-0.0.1/mercapy/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 11:30:55.000000 mercapy-0.0.1/mercapy/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      352 2024-05-17 11:30:55.000000 mercapy-0.0.1/mercapy/utils/api.py
--rw-r--r--   0 runner    (1001) docker     (127)      231 2024-05-17 11:30:55.000000 mercapy-0.0.1/mercapy/utils/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 11:31:00.236102 mercapy-0.0.1/mercapy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2426 2024-05-17 11:31:00.000000 mercapy-0.0.1/mercapy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      440 2024-05-17 11:31:00.000000 mercapy-0.0.1/mercapy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-17 11:31:00.000000 mercapy-0.0.1/mercapy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-17 11:31:00.000000 mercapy-0.0.1/mercapy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-17 11:31:00.000000 mercapy-0.0.1/mercapy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-17 11:31:00.236102 mercapy-0.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1134 2024-05-17 11:30:55.000000 mercapy-0.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 19:33:53.372498 mercapy-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-05-18 19:33:48.000000 mercapy-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2426 2024-05-18 19:33:53.372498 mercapy-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1856 2024-05-18 19:33:48.000000 mercapy-0.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 19:33:53.368498 mercapy-0.0.2/mercapy/
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-18 19:33:48.000000 mercapy-0.0.2/mercapy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-18 19:33:48.000000 mercapy-0.0.2/mercapy/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 19:33:53.368498 mercapy-0.0.2/mercapy/exceptions/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-18 19:33:48.000000 mercapy-0.0.2/mercapy/exceptions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      342 2024-05-18 19:33:48.000000 mercapy-0.0.2/mercapy/exceptions/product.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-18 19:33:48.000000 mercapy-0.0.2/mercapy/merca.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 19:33:53.372498 mercapy-0.0.2/mercapy/product/
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-18 19:33:48.000000 mercapy-0.0.2/mercapy/product/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1236 2024-05-18 19:33:48.000000 mercapy-0.0.2/mercapy/product/photo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3391 2024-05-18 19:33:48.000000 mercapy-0.0.2/mercapy/product/product.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 19:33:53.372498 mercapy-0.0.2/mercapy/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-18 19:33:48.000000 mercapy-0.0.2/mercapy/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      352 2024-05-18 19:33:48.000000 mercapy-0.0.2/mercapy/utils/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      231 2024-05-18 19:33:48.000000 mercapy-0.0.2/mercapy/utils/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 19:33:53.372498 mercapy-0.0.2/mercapy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2426 2024-05-18 19:33:53.000000 mercapy-0.0.2/mercapy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      448 2024-05-18 19:33:53.000000 mercapy-0.0.2/mercapy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-18 19:33:53.000000 mercapy-0.0.2/mercapy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-18 19:33:53.000000 mercapy-0.0.2/mercapy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-18 19:33:53.000000 mercapy-0.0.2/mercapy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-18 19:33:53.372498 mercapy-0.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1134 2024-05-18 19:33:48.000000 mercapy-0.0.2/setup.py
```

### Comparing `mercapy-0.0.1/LICENSE` & `mercapy-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `mercapy-0.0.1/PKG-INFO` & `mercapy-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mercapy
-Version: 0.0.1
+Version: 0.0.2
 Summary: A Mercadona SDK for Python to track product prices, amounts, and more.
 Author: Joel Taylor
 Author-email: contact@joeltaylor.business
 License: MIT
 Keywords: mercadona,api,sdk,data science,prices,information
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: mercapy Version: 0.0.1 Summary: A Mercadona SDK for
+Metadata-Version: 2.1 Name: mercapy Version: 0.0.2 Summary: A Mercadona SDK for
 Python to track product prices, amounts, and more. Author: Joel Taylor Author-
 email: contact@joeltaylor.business License: MIT Keywords:
 mercadona,api,sdk,data science,prices,information Classifier: License :: OSI
 Approved :: MIT License Classifier: Programming Language :: Python Classifier:
 Programming Language :: Python :: 3.12 Classifier: Programming Language ::
 Python :: Implementation :: CPython Description-Content-Type: text/markdown
 License-File: LICENSE Requires-Dist: requests
```

### Comparing `mercapy-0.0.1/README.md` & `mercapy-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `mercapy-0.0.1/mercapy/product/photo.py` & `mercapy-0.0.2/mercapy/product/photo.py`

 * *Files identical despite different names*

### Comparing `mercapy-0.0.1/mercapy/product.py` & `mercapy-0.0.2/mercapy/product/product.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from dataclasses import dataclass
 from urllib.parse import urljoin
 
-from .exceptions.product import *
-from .constants import API_URL
-from .utils.urls import get_file_path
-from .utils.api import fetch_json
-from .product.photo import Photo
+from ..exceptions.product import *
+from ..constants import API_URL
+from ..utils.urls import get_file_path
+from ..utils.api import fetch_json
+from .photo import Photo
 
 
 @dataclass
 class Product:
     id: str
     lang: str = "es"
```

### Comparing `mercapy-0.0.1/mercapy.egg-info/PKG-INFO` & `mercapy-0.0.2/mercapy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mercapy
-Version: 0.0.1
+Version: 0.0.2
 Summary: A Mercadona SDK for Python to track product prices, amounts, and more.
 Author: Joel Taylor
 Author-email: contact@joeltaylor.business
 License: MIT
 Keywords: mercadona,api,sdk,data science,prices,information
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: mercapy Version: 0.0.1 Summary: A Mercadona SDK for
+Metadata-Version: 2.1 Name: mercapy Version: 0.0.2 Summary: A Mercadona SDK for
 Python to track product prices, amounts, and more. Author: Joel Taylor Author-
 email: contact@joeltaylor.business License: MIT Keywords:
 mercadona,api,sdk,data science,prices,information Classifier: License :: OSI
 Approved :: MIT License Classifier: Programming Language :: Python Classifier:
 Programming Language :: Python :: 3.12 Classifier: Programming Language ::
 Python :: Implementation :: CPython Description-Content-Type: text/markdown
 License-File: LICENSE Requires-Dist: requests
```

### Comparing `mercapy-0.0.1/setup.py` & `mercapy-0.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 from codecs import open
 from os import path
 
 # Read version from VERSION file
 here = path.abspath(path.dirname(__file__))
 
-VERSION = "0.0.1"
+VERSION = "0.0.2"
 DESCRIPTION = "A Mercadona SDK for Python to track product prices, amounts, and more."
 
 # Get the long description from the README file
 with open(path.join(here, "README.md"), encoding="utf-8") as f:
     LONG_DESCRIPTION = f.read()
 
 setup(
```

