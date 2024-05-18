# Comparing `tmp/clean-alchemy-0.1.6.tar.gz` & `tmp/clean-alchemy-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clean-alchemy-0.1.6.tar", last modified: Fri May 17 08:16:59 2024, max compression
+gzip compressed data, was "clean-alchemy-0.1.7.tar", last modified: Sat May 18 13:23:02 2024, max compression
```

## Comparing `clean-alchemy-0.1.6.tar` & `clean-alchemy-0.1.7.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 swords     (501) staff       (20)        0 2024-05-17 08:16:59.097654 clean-alchemy-0.1.6/
--rw-r--r--   0 swords     (501) staff       (20)    11357 2024-05-15 18:56:06.000000 clean-alchemy-0.1.6/LICENSE
--rw-r--r--   0 swords     (501) staff       (20)     1481 2024-05-17 08:16:59.097514 clean-alchemy-0.1.6/PKG-INFO
--rw-r--r--   0 swords     (501) staff       (20)      883 2024-05-15 18:56:06.000000 clean-alchemy-0.1.6/README.md
-drwxr-xr-x   0 swords     (501) staff       (20)        0 2024-05-17 08:16:59.096697 clean-alchemy-0.1.6/clean_alchemy/
--rw-r--r--   0 swords     (501) staff       (20)      195 2024-05-17 08:13:25.000000 clean-alchemy-0.1.6/clean_alchemy/__init__.py
--rw-r--r--   0 swords     (501) staff       (20)      445 2024-05-15 20:09:20.000000 clean-alchemy-0.1.6/clean_alchemy/base.py
--rw-r--r--   0 swords     (501) staff       (20)      782 2024-05-17 08:16:17.000000 clean-alchemy-0.1.6/clean_alchemy/base_dao.py
--rw-r--r--   0 swords     (501) staff       (20)      500 2024-05-15 18:56:06.000000 clean-alchemy-0.1.6/clean_alchemy/base_ent.py
--rw-r--r--   0 swords     (501) staff       (20)     3645 2024-05-16 17:18:08.000000 clean-alchemy-0.1.6/clean_alchemy/base_rpo.py
--rw-r--r--   0 swords     (501) staff       (20)     2015 2024-05-15 20:12:10.000000 clean-alchemy-0.1.6/clean_alchemy/base_srv.py
--rw-r--r--   0 swords     (501) staff       (20)      357 2024-05-15 18:56:06.000000 clean-alchemy-0.1.6/clean_alchemy/config.py
-drwxr-xr-x   0 swords     (501) staff       (20)        0 2024-05-17 08:16:59.097336 clean-alchemy-0.1.6/clean_alchemy.egg-info/
--rw-r--r--   0 swords     (501) staff       (20)     1481 2024-05-17 08:16:59.000000 clean-alchemy-0.1.6/clean_alchemy.egg-info/PKG-INFO
--rw-r--r--   0 swords     (501) staff       (20)      386 2024-05-17 08:16:59.000000 clean-alchemy-0.1.6/clean_alchemy.egg-info/SOURCES.txt
--rw-r--r--   0 swords     (501) staff       (20)        1 2024-05-17 08:16:59.000000 clean-alchemy-0.1.6/clean_alchemy.egg-info/dependency_links.txt
--rw-r--r--   0 swords     (501) staff       (20)      516 2024-05-17 08:16:59.000000 clean-alchemy-0.1.6/clean_alchemy.egg-info/requires.txt
--rw-r--r--   0 swords     (501) staff       (20)       14 2024-05-17 08:16:59.000000 clean-alchemy-0.1.6/clean_alchemy.egg-info/top_level.txt
--rw-r--r--   0 swords     (501) staff       (20)       38 2024-05-17 08:16:59.097710 clean-alchemy-0.1.6/setup.cfg
--rw-r--r--   0 swords     (501) staff       (20)     1669 2024-05-17 08:16:53.000000 clean-alchemy-0.1.6/setup.py
+drwxr-xr-x   0 swords     (501) staff       (20)        0 2024-05-18 13:23:02.580375 clean-alchemy-0.1.7/
+-rw-r--r--   0 swords     (501) staff       (20)    11357 2024-05-15 18:56:06.000000 clean-alchemy-0.1.7/LICENSE
+-rw-r--r--   0 swords     (501) staff       (20)     1481 2024-05-18 13:23:02.580263 clean-alchemy-0.1.7/PKG-INFO
+-rw-r--r--   0 swords     (501) staff       (20)      883 2024-05-15 18:56:06.000000 clean-alchemy-0.1.7/README.md
+drwxr-xr-x   0 swords     (501) staff       (20)        0 2024-05-18 13:23:02.579408 clean-alchemy-0.1.7/clean_alchemy/
+-rw-r--r--   0 swords     (501) staff       (20)      195 2024-05-17 08:13:25.000000 clean-alchemy-0.1.7/clean_alchemy/__init__.py
+-rw-r--r--   0 swords     (501) staff       (20)      445 2024-05-15 20:09:20.000000 clean-alchemy-0.1.7/clean_alchemy/base.py
+-rw-r--r--   0 swords     (501) staff       (20)      782 2024-05-17 08:16:17.000000 clean-alchemy-0.1.7/clean_alchemy/base_dao.py
+-rw-r--r--   0 swords     (501) staff       (20)      500 2024-05-15 18:56:06.000000 clean-alchemy-0.1.7/clean_alchemy/base_ent.py
+-rw-r--r--   0 swords     (501) staff       (20)     3645 2024-05-16 17:18:08.000000 clean-alchemy-0.1.7/clean_alchemy/base_rpo.py
+-rw-r--r--   0 swords     (501) staff       (20)     2076 2024-05-18 13:17:39.000000 clean-alchemy-0.1.7/clean_alchemy/base_srv.py
+-rw-r--r--   0 swords     (501) staff       (20)      357 2024-05-15 18:56:06.000000 clean-alchemy-0.1.7/clean_alchemy/config.py
+drwxr-xr-x   0 swords     (501) staff       (20)        0 2024-05-18 13:23:02.580096 clean-alchemy-0.1.7/clean_alchemy.egg-info/
+-rw-r--r--   0 swords     (501) staff       (20)     1481 2024-05-18 13:23:02.000000 clean-alchemy-0.1.7/clean_alchemy.egg-info/PKG-INFO
+-rw-r--r--   0 swords     (501) staff       (20)      386 2024-05-18 13:23:02.000000 clean-alchemy-0.1.7/clean_alchemy.egg-info/SOURCES.txt
+-rw-r--r--   0 swords     (501) staff       (20)        1 2024-05-18 13:23:02.000000 clean-alchemy-0.1.7/clean_alchemy.egg-info/dependency_links.txt
+-rw-r--r--   0 swords     (501) staff       (20)      516 2024-05-18 13:23:02.000000 clean-alchemy-0.1.7/clean_alchemy.egg-info/requires.txt
+-rw-r--r--   0 swords     (501) staff       (20)       14 2024-05-18 13:23:02.000000 clean-alchemy-0.1.7/clean_alchemy.egg-info/top_level.txt
+-rw-r--r--   0 swords     (501) staff       (20)       38 2024-05-18 13:23:02.580421 clean-alchemy-0.1.7/setup.cfg
+-rw-r--r--   0 swords     (501) staff       (20)     1669 2024-05-18 13:22:37.000000 clean-alchemy-0.1.7/setup.py
```

### Comparing `clean-alchemy-0.1.6/LICENSE` & `clean-alchemy-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `clean-alchemy-0.1.6/PKG-INFO` & `clean-alchemy-0.1.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clean-alchemy
-Version: 0.1.6
+Version: 0.1.7
 Summary: A framework for implementing Clean Architecture using SQLAlchemy, with currently only support for FastAPI.
 Home-page: https://github.com/davidswords/clean-alchemy
 Author: David Swords
 Author-email: furuer_svette.0k@icloud.com
 License: Apache 2.0
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `clean-alchemy-0.1.6/README.md` & `clean-alchemy-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `clean-alchemy-0.1.6/clean_alchemy/base_dao.py` & `clean-alchemy-0.1.7/clean_alchemy/base_dao.py`

 * *Files identical despite different names*

### Comparing `clean-alchemy-0.1.6/clean_alchemy/base_rpo.py` & `clean-alchemy-0.1.7/clean_alchemy/base_rpo.py`

 * *Files identical despite different names*

### Comparing `clean-alchemy-0.1.6/clean_alchemy/base_srv.py` & `clean-alchemy-0.1.7/clean_alchemy/base_srv.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 import string
 
 from abc import ABC, abstractmethod
-from random import choice
+from random import sample
 from typing import Generic, List, Tuple, TypeVar
 
 from clean_alchemy import BaseRPO, BaseENT
 
 
 RPO_TYPE = TypeVar("RPO_TYPE", bound=BaseRPO)
 ENT_TYPE = TypeVar("ENT_TYPE", bound=BaseENT)
 
 
 class BaseSRV(ABC, Generic[RPO_TYPE, ENT_TYPE]):
-    def __init__(cls, rpo: RPO_TYPE) -> None:
-        cls.rpo = rpo
+    def __init__(self, rpo: RPO_TYPE) -> None:
+        self.rpo = rpo
 
     @staticmethod
-    def _generate_key(length: int = 24) -> str:
+    def _generate_key(prefix: str = "", postfix: str = "", length: int = 24) -> str:
         characters = string.ascii_letters + string.digits
-        return "".join(choice(characters, k=length))
+        return f"{prefix}{''.join(sample(characters, k=length))}{postfix}"
 
     @abstractmethod
     def _generate_metadata(self) -> dict:
         pass
 
     @abstractmethod
     def _create_ent_from_doc(self, doc: dict) -> ENT_TYPE:
```

### Comparing `clean-alchemy-0.1.6/clean_alchemy.egg-info/PKG-INFO` & `clean-alchemy-0.1.7/clean_alchemy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clean-alchemy
-Version: 0.1.6
+Version: 0.1.7
 Summary: A framework for implementing Clean Architecture using SQLAlchemy, with currently only support for FastAPI.
 Home-page: https://github.com/davidswords/clean-alchemy
 Author: David Swords
 Author-email: furuer_svette.0k@icloud.com
 License: Apache 2.0
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `clean-alchemy-0.1.6/clean_alchemy.egg-info/requires.txt` & `clean-alchemy-0.1.7/clean_alchemy.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `clean-alchemy-0.1.6/setup.py` & `clean-alchemy-0.1.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="clean-alchemy",
-    version="0.1.6",
+    version="0.1.7",
     packages=find_packages(exclude=["tests*", "build*"]),
     install_requires=[
         "annotated-types==0.6.0",
         "black==24.4.2",
         "click==8.1.7",
         "exceptiongroup==1.2.1",
         "factory-boy==3.3.0",
```

