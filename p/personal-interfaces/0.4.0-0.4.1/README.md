# Comparing `tmp/personal_interfaces-0.4.0.tar.gz` & `tmp/personal_interfaces-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "personal_interfaces-0.4.0.tar", last modified: Mon May 13 03:15:01 2024, max compression
+gzip compressed data, was "personal_interfaces-0.4.1.tar", last modified: Sat May 18 19:04:42 2024, max compression
```

## Comparing `personal_interfaces-0.4.0.tar` & `personal_interfaces-0.4.1.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 03:15:01.125503 personal_interfaces-0.4.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-05-13 03:14:51.000000 personal_interfaces-0.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4145 2024-05-13 03:15:01.125503 personal_interfaces-0.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3362 2024-05-13 03:14:51.000000 personal_interfaces-0.4.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 03:15:01.121503 personal_interfaces-0.4.0/personal_interfaces/
--rw-r--r--   0 runner    (1001) docker     (127)      193 2024-05-13 03:14:51.000000 personal_interfaces-0.4.0/personal_interfaces/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-13 03:14:51.000000 personal_interfaces-0.4.0/personal_interfaces/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)      974 2024-05-13 03:14:51.000000 personal_interfaces-0.4.0/personal_interfaces/base_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     5217 2024-05-13 03:14:51.000000 personal_interfaces-0.4.0/personal_interfaces/database_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 03:15:01.125503 personal_interfaces-0.4.0/personal_interfaces/graphql/
--rw-r--r--   0 runner    (1001) docker     (127)      457 2024-05-13 03:14:51.000000 personal_interfaces-0.4.0/personal_interfaces/graphql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1486 2024-05-13 03:14:51.000000 personal_interfaces-0.4.0/personal_interfaces/graphql/_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 03:15:01.125503 personal_interfaces-0.4.0/personal_interfaces/graphql/connectors/
--rw-r--r--   0 runner    (1001) docker     (127)      120 2024-05-13 03:14:51.000000 personal_interfaces-0.4.0/personal_interfaces/graphql/connectors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10754 2024-05-13 03:14:51.000000 personal_interfaces-0.4.0/personal_interfaces/graphql/connectors/deta_db.py
--rw-r--r--   0 runner    (1001) docker     (127)     4865 2024-05-13 03:14:51.000000 personal_interfaces-0.4.0/personal_interfaces/graphql/connectors/template.py
--rw-r--r--   0 runner    (1001) docker     (127)    10442 2024-05-13 03:14:51.000000 personal_interfaces-0.4.0/personal_interfaces/graphql/connectors/tinydb_db.py
--rw-r--r--   0 runner    (1001) docker     (127)     1920 2024-05-13 03:14:51.000000 personal_interfaces-0.4.0/personal_interfaces/graphql/interface.py
--rw-r--r--   0 runner    (1001) docker     (127)    18682 2024-05-13 03:14:51.000000 personal_interfaces-0.4.0/personal_interfaces/graphql/models_builder.py
--rw-r--r--   0 runner    (1001) docker     (127)     7858 2024-05-13 03:14:51.000000 personal_interfaces-0.4.0/personal_interfaces/graphql/mutation_builder.py
--rw-r--r--   0 runner    (1001) docker     (127)    10829 2024-05-13 03:14:51.000000 personal_interfaces-0.4.0/personal_interfaces/graphql/query_builder.py
--rw-r--r--   0 runner    (1001) docker     (127)     3508 2024-05-13 03:14:51.000000 personal_interfaces-0.4.0/personal_interfaces/jwt_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     3591 2024-05-13 03:14:51.000000 personal_interfaces-0.4.0/personal_interfaces/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     4456 2024-05-13 03:14:51.000000 personal_interfaces-0.4.0/personal_interfaces/server_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 03:15:01.121503 personal_interfaces-0.4.0/personal_interfaces.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4145 2024-05-13 03:15:01.000000 personal_interfaces-0.4.0/personal_interfaces.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      956 2024-05-13 03:15:01.000000 personal_interfaces-0.4.0/personal_interfaces.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 03:15:01.000000 personal_interfaces-0.4.0/personal_interfaces.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-05-13 03:15:01.000000 personal_interfaces-0.4.0/personal_interfaces.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-13 03:15:01.000000 personal_interfaces-0.4.0/personal_interfaces.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      634 2024-05-13 03:14:51.000000 personal_interfaces-0.4.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-13 03:15:01.125503 personal_interfaces-0.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2280 2024-05-13 03:14:51.000000 personal_interfaces-0.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 19:04:42.826938 personal_interfaces-0.4.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-05-18 19:04:34.000000 personal_interfaces-0.4.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4145 2024-05-18 19:04:42.826938 personal_interfaces-0.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3362 2024-05-18 19:04:34.000000 personal_interfaces-0.4.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 19:04:42.822938 personal_interfaces-0.4.1/personal_interfaces/
+-rw-r--r--   0 runner    (1001) docker     (127)      193 2024-05-18 19:04:34.000000 personal_interfaces-0.4.1/personal_interfaces/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-18 19:04:34.000000 personal_interfaces-0.4.1/personal_interfaces/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)      974 2024-05-18 19:04:34.000000 personal_interfaces-0.4.1/personal_interfaces/base_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5217 2024-05-18 19:04:34.000000 personal_interfaces-0.4.1/personal_interfaces/database_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 19:04:42.826938 personal_interfaces-0.4.1/personal_interfaces/graphql/
+-rw-r--r--   0 runner    (1001) docker     (127)      457 2024-05-18 19:04:34.000000 personal_interfaces-0.4.1/personal_interfaces/graphql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1486 2024-05-18 19:04:34.000000 personal_interfaces-0.4.1/personal_interfaces/graphql/_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 19:04:42.826938 personal_interfaces-0.4.1/personal_interfaces/graphql/connectors/
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-05-18 19:04:34.000000 personal_interfaces-0.4.1/personal_interfaces/graphql/connectors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10754 2024-05-18 19:04:34.000000 personal_interfaces-0.4.1/personal_interfaces/graphql/connectors/deta_db.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4865 2024-05-18 19:04:34.000000 personal_interfaces-0.4.1/personal_interfaces/graphql/connectors/template.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10442 2024-05-18 19:04:34.000000 personal_interfaces-0.4.1/personal_interfaces/graphql/connectors/tinydb_db.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1920 2024-05-18 19:04:34.000000 personal_interfaces-0.4.1/personal_interfaces/graphql/interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18752 2024-05-18 19:04:34.000000 personal_interfaces-0.4.1/personal_interfaces/graphql/models_builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7858 2024-05-18 19:04:34.000000 personal_interfaces-0.4.1/personal_interfaces/graphql/mutation_builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10829 2024-05-18 19:04:34.000000 personal_interfaces-0.4.1/personal_interfaces/graphql/query_builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3508 2024-05-18 19:04:34.000000 personal_interfaces-0.4.1/personal_interfaces/jwt_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3591 2024-05-18 19:04:34.000000 personal_interfaces-0.4.1/personal_interfaces/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4456 2024-05-18 19:04:34.000000 personal_interfaces-0.4.1/personal_interfaces/server_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 19:04:42.826938 personal_interfaces-0.4.1/personal_interfaces.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4145 2024-05-18 19:04:42.000000 personal_interfaces-0.4.1/personal_interfaces.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      956 2024-05-18 19:04:42.000000 personal_interfaces-0.4.1/personal_interfaces.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-18 19:04:42.000000 personal_interfaces-0.4.1/personal_interfaces.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-05-18 19:04:42.000000 personal_interfaces-0.4.1/personal_interfaces.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-18 19:04:42.000000 personal_interfaces-0.4.1/personal_interfaces.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      634 2024-05-18 19:04:34.000000 personal_interfaces-0.4.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-18 19:04:42.826938 personal_interfaces-0.4.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2280 2024-05-18 19:04:34.000000 personal_interfaces-0.4.1/setup.py
```

### Comparing `personal_interfaces-0.4.0/LICENSE` & `personal_interfaces-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `personal_interfaces-0.4.0/PKG-INFO` & `personal_interfaces-0.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: personal_interfaces
-Version: 0.4.0
+Version: 0.4.1
 Home-page: https://github.com/ricardoleal20/personal_interface/
 Author: Ricardo Leal
 Author-email: ricardo.lealpz@gmail.com
 Maintainer: Ricardo Leal
 Maintainer-email: ricardo.lealpz@gmail.com
 Project-URL: Bug Reports, https://github.com/ricardoleal20/personal_interface/issues
 Keywords: development,personal_usage
```

### Comparing `personal_interfaces-0.4.0/README.md` & `personal_interfaces-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `personal_interfaces-0.4.0/personal_interfaces/base_api.py` & `personal_interfaces-0.4.1/personal_interfaces/base_api.py`

 * *Files identical despite different names*

### Comparing `personal_interfaces-0.4.0/personal_interfaces/database_handler.py` & `personal_interfaces-0.4.1/personal_interfaces/database_handler.py`

 * *Files identical despite different names*

### Comparing `personal_interfaces-0.4.0/personal_interfaces/graphql/_utils.py` & `personal_interfaces-0.4.1/personal_interfaces/graphql/_utils.py`

 * *Files identical despite different names*

### Comparing `personal_interfaces-0.4.0/personal_interfaces/graphql/connectors/deta_db.py` & `personal_interfaces-0.4.1/personal_interfaces/graphql/connectors/deta_db.py`

 * *Files identical despite different names*

### Comparing `personal_interfaces-0.4.0/personal_interfaces/graphql/connectors/template.py` & `personal_interfaces-0.4.1/personal_interfaces/graphql/connectors/template.py`

 * *Files identical despite different names*

### Comparing `personal_interfaces-0.4.0/personal_interfaces/graphql/connectors/tinydb_db.py` & `personal_interfaces-0.4.1/personal_interfaces/graphql/connectors/tinydb_db.py`

 * *Files identical despite different names*

### Comparing `personal_interfaces-0.4.0/personal_interfaces/graphql/interface.py` & `personal_interfaces-0.4.1/personal_interfaces/graphql/interface.py`

 * *Files identical despite different names*

### Comparing `personal_interfaces-0.4.0/personal_interfaces/graphql/models_builder.py` & `personal_interfaces-0.4.1/personal_interfaces/graphql/models_builder.py`

 * *Files 0% similar despite different names*

```diff
@@ -45,17 +45,19 @@
         # Also, define the GraphQL scalars equivalences
         self._scalars = {
             'ID': strawberry.ID,
             'Boolean': bool,
             'String': str,
             'Int': int,
             'Integer': int,
+            'Float': float,
             'Date': date,
             'DateTime': datetime,
             'Text': str,
+            'Private': strawberry.Private
         }
 
         self._defaults = {
             'UNDEFINED': 'FunctionType.UNDEFINED',
             'UNINITIALIZED': 'ProgramStatus.UNINITIALIZED',
             'PENDING': 'PlanStatus.PENDING',
             'LIMITED': 'LotType.LIMITED',
```

### Comparing `personal_interfaces-0.4.0/personal_interfaces/graphql/mutation_builder.py` & `personal_interfaces-0.4.1/personal_interfaces/graphql/mutation_builder.py`

 * *Files identical despite different names*

### Comparing `personal_interfaces-0.4.0/personal_interfaces/graphql/query_builder.py` & `personal_interfaces-0.4.1/personal_interfaces/graphql/query_builder.py`

 * *Files identical despite different names*

### Comparing `personal_interfaces-0.4.0/personal_interfaces/jwt_handler.py` & `personal_interfaces-0.4.1/personal_interfaces/jwt_handler.py`

 * *Files identical despite different names*

### Comparing `personal_interfaces-0.4.0/personal_interfaces/logger.py` & `personal_interfaces-0.4.1/personal_interfaces/logger.py`

 * *Files identical despite different names*

### Comparing `personal_interfaces-0.4.0/personal_interfaces/server_handler.py` & `personal_interfaces-0.4.1/personal_interfaces/server_handler.py`

 * *Files identical despite different names*

### Comparing `personal_interfaces-0.4.0/personal_interfaces.egg-info/PKG-INFO` & `personal_interfaces-0.4.1/personal_interfaces.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: personal-interfaces
-Version: 0.4.0
+Version: 0.4.1
 Home-page: https://github.com/ricardoleal20/personal_interface/
 Author: Ricardo Leal
 Author-email: ricardo.lealpz@gmail.com
 Maintainer: Ricardo Leal
 Maintainer-email: ricardo.lealpz@gmail.com
 Project-URL: Bug Reports, https://github.com/ricardoleal20/personal_interface/issues
 Keywords: development,personal_usage
```

### Comparing `personal_interfaces-0.4.0/personal_interfaces.egg-info/SOURCES.txt` & `personal_interfaces-0.4.1/personal_interfaces.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `personal_interfaces-0.4.0/pyproject.toml` & `personal_interfaces-0.4.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "personal_interfaces"
-version = "0.4.0"
+version = "0.4.1"
 description = "Interface for personal usage. Is intended to be used in personal projects"
 authors = ["ricardoleal20 <rick.leal420@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `personal_interfaces-0.4.0/setup.py` & `personal_interfaces-0.4.1/setup.py`

 * *Files identical despite different names*

