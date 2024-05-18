# Comparing `tmp/clean-alchemy-0.1.7.tar.gz` & `tmp/clean-alchemy-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clean-alchemy-0.1.7.tar", last modified: Sat May 18 13:23:02 2024, max compression
+gzip compressed data, was "clean-alchemy-0.1.8.tar", last modified: Sat May 18 13:41:21 2024, max compression
```

## Comparing `clean-alchemy-0.1.7.tar` & `clean-alchemy-0.1.8.tar`

### file list

```diff
@@ -1,20 +1,22 @@
-drwxr-xr-x   0 swords     (501) staff       (20)        0 2024-05-18 13:23:02.580375 clean-alchemy-0.1.7/
--rw-r--r--   0 swords     (501) staff       (20)    11357 2024-05-15 18:56:06.000000 clean-alchemy-0.1.7/LICENSE
--rw-r--r--   0 swords     (501) staff       (20)     1481 2024-05-18 13:23:02.580263 clean-alchemy-0.1.7/PKG-INFO
--rw-r--r--   0 swords     (501) staff       (20)      883 2024-05-15 18:56:06.000000 clean-alchemy-0.1.7/README.md
-drwxr-xr-x   0 swords     (501) staff       (20)        0 2024-05-18 13:23:02.579408 clean-alchemy-0.1.7/clean_alchemy/
--rw-r--r--   0 swords     (501) staff       (20)      195 2024-05-17 08:13:25.000000 clean-alchemy-0.1.7/clean_alchemy/__init__.py
--rw-r--r--   0 swords     (501) staff       (20)      445 2024-05-15 20:09:20.000000 clean-alchemy-0.1.7/clean_alchemy/base.py
--rw-r--r--   0 swords     (501) staff       (20)      782 2024-05-17 08:16:17.000000 clean-alchemy-0.1.7/clean_alchemy/base_dao.py
--rw-r--r--   0 swords     (501) staff       (20)      500 2024-05-15 18:56:06.000000 clean-alchemy-0.1.7/clean_alchemy/base_ent.py
--rw-r--r--   0 swords     (501) staff       (20)     3645 2024-05-16 17:18:08.000000 clean-alchemy-0.1.7/clean_alchemy/base_rpo.py
--rw-r--r--   0 swords     (501) staff       (20)     2076 2024-05-18 13:17:39.000000 clean-alchemy-0.1.7/clean_alchemy/base_srv.py
--rw-r--r--   0 swords     (501) staff       (20)      357 2024-05-15 18:56:06.000000 clean-alchemy-0.1.7/clean_alchemy/config.py
-drwxr-xr-x   0 swords     (501) staff       (20)        0 2024-05-18 13:23:02.580096 clean-alchemy-0.1.7/clean_alchemy.egg-info/
--rw-r--r--   0 swords     (501) staff       (20)     1481 2024-05-18 13:23:02.000000 clean-alchemy-0.1.7/clean_alchemy.egg-info/PKG-INFO
--rw-r--r--   0 swords     (501) staff       (20)      386 2024-05-18 13:23:02.000000 clean-alchemy-0.1.7/clean_alchemy.egg-info/SOURCES.txt
--rw-r--r--   0 swords     (501) staff       (20)        1 2024-05-18 13:23:02.000000 clean-alchemy-0.1.7/clean_alchemy.egg-info/dependency_links.txt
--rw-r--r--   0 swords     (501) staff       (20)      516 2024-05-18 13:23:02.000000 clean-alchemy-0.1.7/clean_alchemy.egg-info/requires.txt
--rw-r--r--   0 swords     (501) staff       (20)       14 2024-05-18 13:23:02.000000 clean-alchemy-0.1.7/clean_alchemy.egg-info/top_level.txt
--rw-r--r--   0 swords     (501) staff       (20)       38 2024-05-18 13:23:02.580421 clean-alchemy-0.1.7/setup.cfg
--rw-r--r--   0 swords     (501) staff       (20)     1669 2024-05-18 13:22:37.000000 clean-alchemy-0.1.7/setup.py
+drwxr-xr-x   0 swords     (501) staff       (20)        0 2024-05-18 13:41:21.742069 clean-alchemy-0.1.8/
+-rw-r--r--   0 swords     (501) staff       (20)    11357 2024-05-15 18:56:06.000000 clean-alchemy-0.1.8/LICENSE
+-rw-r--r--   0 swords     (501) staff       (20)     1452 2024-05-18 13:41:21.741943 clean-alchemy-0.1.8/PKG-INFO
+-rw-r--r--   0 swords     (501) staff       (20)      883 2024-05-15 18:56:06.000000 clean-alchemy-0.1.8/README.md
+drwxr-xr-x   0 swords     (501) staff       (20)        0 2024-05-18 13:41:21.740516 clean-alchemy-0.1.8/clean_alchemy.egg-info/
+-rw-r--r--   0 swords     (501) staff       (20)     1452 2024-05-18 13:41:21.000000 clean-alchemy-0.1.8/clean_alchemy.egg-info/PKG-INFO
+-rw-r--r--   0 swords     (501) staff       (20)      430 2024-05-18 13:41:21.000000 clean-alchemy-0.1.8/clean_alchemy.egg-info/SOURCES.txt
+-rw-r--r--   0 swords     (501) staff       (20)        1 2024-05-18 13:41:21.000000 clean-alchemy-0.1.8/clean_alchemy.egg-info/dependency_links.txt
+-rw-r--r--   0 swords     (501) staff       (20)      516 2024-05-18 13:41:21.000000 clean-alchemy-0.1.8/clean_alchemy.egg-info/requires.txt
+-rw-r--r--   0 swords     (501) staff       (20)        4 2024-05-18 13:41:21.000000 clean-alchemy-0.1.8/clean_alchemy.egg-info/top_level.txt
+-rw-r--r--   0 swords     (501) staff       (20)       38 2024-05-18 13:41:21.742119 clean-alchemy-0.1.8/setup.cfg
+-rw-r--r--   0 swords     (501) staff       (20)     1641 2024-05-18 13:40:55.000000 clean-alchemy-0.1.8/setup.py
+drwxr-xr-x   0 swords     (501) staff       (20)        0 2024-05-18 13:41:21.740642 clean-alchemy-0.1.8/src/
+-rw-r--r--   0 swords     (501) staff       (20)        0 2024-05-18 13:39:42.000000 clean-alchemy-0.1.8/src/__init__.py
+drwxr-xr-x   0 swords     (501) staff       (20)        0 2024-05-18 13:41:21.741606 clean-alchemy-0.1.8/src/clean_alchemy/
+-rw-r--r--   0 swords     (501) staff       (20)      195 2024-05-17 08:13:25.000000 clean-alchemy-0.1.8/src/clean_alchemy/__init__.py
+-rw-r--r--   0 swords     (501) staff       (20)      449 2024-05-18 13:39:56.000000 clean-alchemy-0.1.8/src/clean_alchemy/base.py
+-rw-r--r--   0 swords     (501) staff       (20)      786 2024-05-18 13:39:56.000000 clean-alchemy-0.1.8/src/clean_alchemy/base_dao.py
+-rw-r--r--   0 swords     (501) staff       (20)      500 2024-05-15 18:56:06.000000 clean-alchemy-0.1.8/src/clean_alchemy/base_ent.py
+-rw-r--r--   0 swords     (501) staff       (20)     3653 2024-05-18 13:39:56.000000 clean-alchemy-0.1.8/src/clean_alchemy/base_rpo.py
+-rw-r--r--   0 swords     (501) staff       (20)     2004 2024-05-18 13:39:56.000000 clean-alchemy-0.1.8/src/clean_alchemy/base_srv.py
+-rw-r--r--   0 swords     (501) staff       (20)      357 2024-05-15 18:56:06.000000 clean-alchemy-0.1.8/src/clean_alchemy/config.py
```

### Comparing `clean-alchemy-0.1.7/LICENSE` & `clean-alchemy-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `clean-alchemy-0.1.7/PKG-INFO` & `clean-alchemy-0.1.8/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: clean-alchemy
-Version: 0.1.7
-Summary: A framework for implementing Clean Architecture using SQLAlchemy, with currently only support for FastAPI.
+Version: 0.1.8
+Summary: A framework for implementing Clean Architecture using SQLAlchemy for FastAPI.
 Home-page: https://github.com/davidswords/clean-alchemy
 Author: David Swords
 Author-email: furuer_svette.0k@icloud.com
 License: Apache 2.0
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `clean-alchemy-0.1.7/README.md` & `clean-alchemy-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `clean-alchemy-0.1.7/clean_alchemy/base_dao.py` & `clean-alchemy-0.1.8/src/clean_alchemy/base_dao.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from sqlalchemy import Column, Integer, DateTime, String, Boolean
 
-from clean_alchemy.base import Base
+from src.clean_alchemy.base import Base
 
 
 class BaseDAO(Base):
     __abstract__ = True
 
     id = Column(Integer, autoincrement=True)
     key = Column(String, primary_key=True, unique=True, index=True, nullable=False)
```

### Comparing `clean-alchemy-0.1.7/clean_alchemy/base_rpo.py` & `clean-alchemy-0.1.8/src/clean_alchemy/base_rpo.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from abc import ABC, abstractmethod
 from typing import Generic, TypeVar, List, Type
 
 from sqlalchemy.orm import Session
 
-from clean_alchemy import BaseDAO, BaseENT
-from clean_alchemy.config import ENV
+from src.clean_alchemy import BaseDAO, BaseENT
+from src.clean_alchemy.config import ENV
 
 DAO_TYPE = TypeVar("DAO_TYPE", bound=BaseDAO)
 ENT_TYPE = TypeVar("ENT_TYPE", bound=BaseENT)
 
 
 class BaseRPO(ABC, Generic[DAO_TYPE, ENT_TYPE]):
     dao_class: Type[DAO_TYPE] = None
```

### Comparing `clean-alchemy-0.1.7/clean_alchemy/base_srv.py` & `clean-alchemy-0.1.8/src/clean_alchemy/base_srv.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import string
 
 from abc import ABC, abstractmethod
 from random import sample
 from typing import Generic, List, Tuple, TypeVar
 
-from clean_alchemy import BaseRPO, BaseENT
+from src.clean_alchemy import BaseRPO, BaseENT
 
 
 RPO_TYPE = TypeVar("RPO_TYPE", bound=BaseRPO)
 ENT_TYPE = TypeVar("ENT_TYPE", bound=BaseENT)
 
 
 class BaseSRV(ABC, Generic[RPO_TYPE, ENT_TYPE]):
@@ -17,18 +17,14 @@
 
     @staticmethod
     def _generate_key(prefix: str = "", postfix: str = "", length: int = 24) -> str:
         characters = string.ascii_letters + string.digits
         return f"{prefix}{''.join(sample(characters, k=length))}{postfix}"
 
     @abstractmethod
-    def _generate_metadata(self) -> dict:
-        pass
-
-    @abstractmethod
     def _create_ent_from_doc(self, doc: dict) -> ENT_TYPE:
         pass
 
     @abstractmethod
     def _update_ent_from_doc(self, ent: ENT_TYPE, doc: dict) -> ENT_TYPE:
         pass
```

### Comparing `clean-alchemy-0.1.7/clean_alchemy.egg-info/PKG-INFO` & `clean-alchemy-0.1.8/clean_alchemy.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: clean-alchemy
-Version: 0.1.7
-Summary: A framework for implementing Clean Architecture using SQLAlchemy, with currently only support for FastAPI.
+Version: 0.1.8
+Summary: A framework for implementing Clean Architecture using SQLAlchemy for FastAPI.
 Home-page: https://github.com/davidswords/clean-alchemy
 Author: David Swords
 Author-email: furuer_svette.0k@icloud.com
 License: Apache 2.0
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `clean-alchemy-0.1.7/clean_alchemy.egg-info/requires.txt` & `clean-alchemy-0.1.8/clean_alchemy.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `clean-alchemy-0.1.7/setup.py` & `clean-alchemy-0.1.8/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="clean-alchemy",
-    version="0.1.7",
+    version="0.1.8",
     packages=find_packages(exclude=["tests*", "build*"]),
     install_requires=[
         "annotated-types==0.6.0",
         "black==24.4.2",
         "click==8.1.7",
         "exceptiongroup==1.2.1",
         "factory-boy==3.3.0",
@@ -36,19 +36,19 @@
             "pytest-mock==3.14.0",
             "factory-boy==3.3.0",
             "pytest-sugar==1.0.0",
         ],
     },
     author="David Swords",
     author_email="furuer_svette.0k@icloud.com",
-    description="A framework for implementing Clean Architecture using SQLAlchemy, with currently only support for FastAPI.",
+    description="A framework for implementing Clean Architecture using SQLAlchemy for FastAPI.",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     license="Apache 2.0",
     url="https://github.com/davidswords/clean-alchemy",
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: OS Independent",
     ],
     python_requires=">=3.9.6",
-)
+)
```

