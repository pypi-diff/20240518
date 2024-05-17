# Comparing `tmp/kvalchemy-0.0.3.tar.gz` & `tmp/kvalchemy-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kvalchemy-0.0.3.tar", last modified: Fri May 17 22:42:20 2024, max compression
+gzip compressed data, was "kvalchemy-0.0.4.tar", last modified: Fri May 17 22:49:19 2024, max compression
```

## Comparing `kvalchemy-0.0.3.tar` & `kvalchemy-0.0.4.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 22:42:20.359750 kvalchemy-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-05-17 22:42:12.000000 kvalchemy-0.0.3/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)     1721 2024-05-17 22:42:20.359750 kvalchemy-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1000 2024-05-17 22:42:12.000000 kvalchemy-0.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 22:42:20.355750 kvalchemy-0.0.3/kvalchemy/
--rw-r--r--   0 runner    (1001) docker     (127)      113 2024-05-17 22:42:12.000000 kvalchemy-0.0.3/kvalchemy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9133 2024-05-17 22:42:12.000000 kvalchemy-0.0.3/kvalchemy/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     1243 2024-05-17 22:42:12.000000 kvalchemy-0.0.3/kvalchemy/models.py
--rw-r--r--   0 runner    (1001) docker     (127)     2067 2024-05-17 22:42:12.000000 kvalchemy-0.0.3/kvalchemy/proxy.py
--rw-r--r--   0 runner    (1001) docker     (127)     1379 2024-05-17 22:42:12.000000 kvalchemy-0.0.3/kvalchemy/time.py
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-17 22:42:12.000000 kvalchemy-0.0.3/kvalchemy/values.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 22:42:20.359750 kvalchemy-0.0.3/kvalchemy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1721 2024-05-17 22:42:20.000000 kvalchemy-0.0.3/kvalchemy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      378 2024-05-17 22:42:20.000000 kvalchemy-0.0.3/kvalchemy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-17 22:42:20.000000 kvalchemy-0.0.3/kvalchemy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-17 22:42:20.000000 kvalchemy-0.0.3/kvalchemy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-17 22:42:20.000000 kvalchemy-0.0.3/kvalchemy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1020 2024-05-17 22:42:12.000000 kvalchemy-0.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-17 22:42:20.359750 kvalchemy-0.0.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 22:42:20.355750 kvalchemy-0.0.3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     8236 2024-05-17 22:42:12.000000 kvalchemy-0.0.3/tests/test_client.py
--rw-r--r--   0 runner    (1001) docker     (127)      994 2024-05-17 22:42:12.000000 kvalchemy-0.0.3/tests/test_proxy.py
--rw-r--r--   0 runner    (1001) docker     (127)      779 2024-05-17 22:42:12.000000 kvalchemy-0.0.3/tests/test_time.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 22:49:19.974606 kvalchemy-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-05-17 22:49:11.000000 kvalchemy-0.0.4/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1733 2024-05-17 22:49:19.974606 kvalchemy-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1000 2024-05-17 22:49:11.000000 kvalchemy-0.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 22:49:19.970606 kvalchemy-0.0.4/kvalchemy/
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-05-17 22:49:11.000000 kvalchemy-0.0.4/kvalchemy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9133 2024-05-17 22:49:11.000000 kvalchemy-0.0.4/kvalchemy/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1243 2024-05-17 22:49:11.000000 kvalchemy-0.0.4/kvalchemy/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2067 2024-05-17 22:49:11.000000 kvalchemy-0.0.4/kvalchemy/proxy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1379 2024-05-17 22:49:11.000000 kvalchemy-0.0.4/kvalchemy/time.py
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-17 22:49:11.000000 kvalchemy-0.0.4/kvalchemy/values.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 22:49:19.974606 kvalchemy-0.0.4/kvalchemy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1733 2024-05-17 22:49:19.000000 kvalchemy-0.0.4/kvalchemy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      378 2024-05-17 22:49:19.000000 kvalchemy-0.0.4/kvalchemy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-17 22:49:19.000000 kvalchemy-0.0.4/kvalchemy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-17 22:49:19.000000 kvalchemy-0.0.4/kvalchemy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-17 22:49:19.000000 kvalchemy-0.0.4/kvalchemy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1032 2024-05-17 22:49:11.000000 kvalchemy-0.0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-17 22:49:19.974606 kvalchemy-0.0.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 22:49:19.974606 kvalchemy-0.0.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     8236 2024-05-17 22:49:11.000000 kvalchemy-0.0.4/tests/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      994 2024-05-17 22:49:11.000000 kvalchemy-0.0.4/tests/test_proxy.py
+-rw-r--r--   0 runner    (1001) docker     (127)      779 2024-05-17 22:49:11.000000 kvalchemy-0.0.4/tests/test_time.py
```

### Comparing `kvalchemy-0.0.3/LICENSE.md` & `kvalchemy-0.0.4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `kvalchemy-0.0.3/PKG-INFO` & `kvalchemy-0.0.4/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: kvalchemy
-Version: 0.0.3
-Summary: A project for kvalchemy
+Version: 0.0.4
+Summary: A SQLAlchemy based Key-Value store.
 Author-email: csm10495 <csm10495@gmail.com>
 License: MIT License
 Project-URL: homepage, https://github.com/csm10495/kvalchemy
 Project-URL: repository, https://github.com/csm10495/kvalchemy
 Project-URL: documentation, https://csm10495.github.io/kvalchemy
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
```

### Comparing `kvalchemy-0.0.3/README.md` & `kvalchemy-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `kvalchemy-0.0.3/kvalchemy/client.py` & `kvalchemy-0.0.4/kvalchemy/client.py`

 * *Files identical despite different names*

### Comparing `kvalchemy-0.0.3/kvalchemy/models.py` & `kvalchemy-0.0.4/kvalchemy/models.py`

 * *Files identical despite different names*

### Comparing `kvalchemy-0.0.3/kvalchemy/proxy.py` & `kvalchemy-0.0.4/kvalchemy/proxy.py`

 * *Files identical despite different names*

### Comparing `kvalchemy-0.0.3/kvalchemy/time.py` & `kvalchemy-0.0.4/kvalchemy/time.py`

 * *Files identical despite different names*

### Comparing `kvalchemy-0.0.3/kvalchemy.egg-info/PKG-INFO` & `kvalchemy-0.0.4/kvalchemy.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: kvalchemy
-Version: 0.0.3
-Summary: A project for kvalchemy
+Version: 0.0.4
+Summary: A SQLAlchemy based Key-Value store.
 Author-email: csm10495 <csm10495@gmail.com>
 License: MIT License
 Project-URL: homepage, https://github.com/csm10495/kvalchemy
 Project-URL: repository, https://github.com/csm10495/kvalchemy
 Project-URL: documentation, https://csm10495.github.io/kvalchemy
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
```

### Comparing `kvalchemy-0.0.3/pyproject.toml` & `kvalchemy-0.0.4/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "kvalchemy"
-description = "A project for kvalchemy"
+description = "A SQLAlchemy based Key-Value store."
 dynamic = ["version"]
 authors = [{name = "csm10495", email = "csm10495@gmail.com"}]
 license = {text = "MIT License"}
 classifiers = [
     "Intended Audience :: Developers",
     "Natural Language :: English",
     "Operating System :: POSIX",
```

### Comparing `kvalchemy-0.0.3/tests/test_client.py` & `kvalchemy-0.0.4/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `kvalchemy-0.0.3/tests/test_proxy.py` & `kvalchemy-0.0.4/tests/test_proxy.py`

 * *Files identical despite different names*

### Comparing `kvalchemy-0.0.3/tests/test_time.py` & `kvalchemy-0.0.4/tests/test_time.py`

 * *Files identical despite different names*

