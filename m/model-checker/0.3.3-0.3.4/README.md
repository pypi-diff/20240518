# Comparing `tmp/model_checker-0.3.3.tar.gz` & `tmp/model_checker-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "model_checker-0.3.3.tar", last modified: Sat May 18 15:09:29 2024, max compression
+gzip compressed data, was "model_checker-0.3.4.tar", last modified: Sat May 18 15:31:16 2024, max compression
```

## Comparing `model_checker-0.3.3.tar` & `model_checker-0.3.4.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 benjamin  (1000) users      (100)        0 2024-05-18 15:09:29.239747 model_checker-0.3.3/
--rw-r--r--   0 benjamin  (1000) users      (100)     1064 2024-05-08 20:11:06.000000 model_checker-0.3.3/LICENCE
--rw-r--r--   0 benjamin  (1000) users      (100)     5371 2024-05-18 15:09:29.239747 model_checker-0.3.3/PKG-INFO
--rw-r--r--   0 benjamin  (1000) users      (100)     4662 2024-05-12 17:17:50.000000 model_checker-0.3.3/README.md
--rw-r--r--   0 benjamin  (1000) users      (100)      925 2024-05-18 15:09:21.000000 model_checker-0.3.3/pyproject.toml
--rw-r--r--   0 benjamin  (1000) users      (100)       38 2024-05-18 15:09:29.239747 model_checker-0.3.3/setup.cfg
-drwxr-xr-x   0 benjamin  (1000) users      (100)        0 2024-05-18 15:09:29.238747 model_checker-0.3.3/src/
-drwxr-xr-x   0 benjamin  (1000) users      (100)        0 2024-05-18 15:09:29.238747 model_checker-0.3.3/src/model_checker/
--rw-r--r--   0 benjamin  (1000) users      (100)       86 2024-05-08 21:34:17.000000 model_checker-0.3.3/src/model_checker/__init__.py
--rw-r--r--   0 benjamin  (1000) users      (100)     9602 2024-05-18 15:08:34.000000 model_checker-0.3.3/src/model_checker/__main__.py
--rw-r--r--   0 benjamin  (1000) users      (100)    19680 2024-05-18 15:02:56.000000 model_checker-0.3.3/src/model_checker/model_definitions.py
--rw-r--r--   0 benjamin  (1000) users      (100)    26125 2024-05-18 15:08:46.000000 model_checker-0.3.3/src/model_checker/model_structure.py
--rw-r--r--   0 benjamin  (1000) users      (100)    18152 2024-05-13 15:43:10.000000 model_checker-0.3.3/src/model_checker/semantics.py
--rw-r--r--   0 benjamin  (1000) users      (100)     7686 2024-05-17 23:03:51.000000 model_checker-0.3.3/src/model_checker/syntax.py
--rw-r--r--   0 benjamin  (1000) users      (100)     1864 2024-05-08 20:49:46.000000 model_checker-0.3.3/src/model_checker/temp.py
--rw-r--r--   0 benjamin  (1000) users      (100)     2985 2024-05-16 20:27:14.000000 model_checker-0.3.3/src/model_checker/test.py
-drwxr-xr-x   0 benjamin  (1000) users      (100)        0 2024-05-18 15:09:29.239747 model_checker-0.3.3/src/model_checker.egg-info/
--rw-r--r--   0 benjamin  (1000) users      (100)     5371 2024-05-18 15:09:29.000000 model_checker-0.3.3/src/model_checker.egg-info/PKG-INFO
--rw-r--r--   0 benjamin  (1000) users      (100)      549 2024-05-18 15:09:29.000000 model_checker-0.3.3/src/model_checker.egg-info/SOURCES.txt
--rw-r--r--   0 benjamin  (1000) users      (100)        1 2024-05-18 15:09:29.000000 model_checker-0.3.3/src/model_checker.egg-info/dependency_links.txt
--rw-r--r--   0 benjamin  (1000) users      (100)       62 2024-05-18 15:09:29.000000 model_checker-0.3.3/src/model_checker.egg-info/entry_points.txt
--rw-r--r--   0 benjamin  (1000) users      (100)       10 2024-05-18 15:09:29.000000 model_checker-0.3.3/src/model_checker.egg-info/requires.txt
--rw-r--r--   0 benjamin  (1000) users      (100)       14 2024-05-18 15:09:29.000000 model_checker-0.3.3/src/model_checker.egg-info/top_level.txt
-drwxr-xr-x   0 benjamin  (1000) users      (100)        0 2024-05-18 15:09:29.239747 model_checker-0.3.3/test/
--rw-r--r--   0 benjamin  (1000) users      (100)      330 2024-05-13 22:46:42.000000 model_checker-0.3.3/test/test_examples.py
+drwxr-xr-x   0 benjamin  (1000) users      (100)        0 2024-05-18 15:31:16.091332 model_checker-0.3.4/
+-rw-r--r--   0 benjamin  (1000) users      (100)     1064 2024-05-08 20:11:06.000000 model_checker-0.3.4/LICENCE
+-rw-r--r--   0 benjamin  (1000) users      (100)     5371 2024-05-18 15:31:16.090332 model_checker-0.3.4/PKG-INFO
+-rw-r--r--   0 benjamin  (1000) users      (100)     4662 2024-05-12 17:17:50.000000 model_checker-0.3.4/README.md
+-rw-r--r--   0 benjamin  (1000) users      (100)      925 2024-05-18 15:27:08.000000 model_checker-0.3.4/pyproject.toml
+-rw-r--r--   0 benjamin  (1000) users      (100)       38 2024-05-18 15:31:16.091332 model_checker-0.3.4/setup.cfg
+drwxr-xr-x   0 benjamin  (1000) users      (100)        0 2024-05-18 15:31:16.090332 model_checker-0.3.4/src/
+drwxr-xr-x   0 benjamin  (1000) users      (100)        0 2024-05-18 15:31:16.090332 model_checker-0.3.4/src/model_checker/
+-rw-r--r--   0 benjamin  (1000) users      (100)       86 2024-05-08 21:34:17.000000 model_checker-0.3.4/src/model_checker/__init__.py
+-rw-r--r--   0 benjamin  (1000) users      (100)     9602 2024-05-18 15:29:17.000000 model_checker-0.3.4/src/model_checker/__main__.py
+-rw-r--r--   0 benjamin  (1000) users      (100)    19680 2024-05-18 15:02:56.000000 model_checker-0.3.4/src/model_checker/model_definitions.py
+-rw-r--r--   0 benjamin  (1000) users      (100)    26125 2024-05-18 15:29:14.000000 model_checker-0.3.4/src/model_checker/model_structure.py
+-rw-r--r--   0 benjamin  (1000) users      (100)    18152 2024-05-13 15:43:10.000000 model_checker-0.3.4/src/model_checker/semantics.py
+-rw-r--r--   0 benjamin  (1000) users      (100)     7686 2024-05-17 23:03:51.000000 model_checker-0.3.4/src/model_checker/syntax.py
+-rw-r--r--   0 benjamin  (1000) users      (100)     1864 2024-05-08 20:49:46.000000 model_checker-0.3.4/src/model_checker/temp.py
+-rw-r--r--   0 benjamin  (1000) users      (100)     2985 2024-05-16 20:27:14.000000 model_checker-0.3.4/src/model_checker/test.py
+drwxr-xr-x   0 benjamin  (1000) users      (100)        0 2024-05-18 15:31:16.090332 model_checker-0.3.4/src/model_checker.egg-info/
+-rw-r--r--   0 benjamin  (1000) users      (100)     5371 2024-05-18 15:31:16.000000 model_checker-0.3.4/src/model_checker.egg-info/PKG-INFO
+-rw-r--r--   0 benjamin  (1000) users      (100)      549 2024-05-18 15:31:16.000000 model_checker-0.3.4/src/model_checker.egg-info/SOURCES.txt
+-rw-r--r--   0 benjamin  (1000) users      (100)        1 2024-05-18 15:31:16.000000 model_checker-0.3.4/src/model_checker.egg-info/dependency_links.txt
+-rw-r--r--   0 benjamin  (1000) users      (100)       62 2024-05-18 15:31:16.000000 model_checker-0.3.4/src/model_checker.egg-info/entry_points.txt
+-rw-r--r--   0 benjamin  (1000) users      (100)       10 2024-05-18 15:31:16.000000 model_checker-0.3.4/src/model_checker.egg-info/requires.txt
+-rw-r--r--   0 benjamin  (1000) users      (100)       14 2024-05-18 15:31:16.000000 model_checker-0.3.4/src/model_checker.egg-info/top_level.txt
+drwxr-xr-x   0 benjamin  (1000) users      (100)        0 2024-05-18 15:31:16.090332 model_checker-0.3.4/test/
+-rw-r--r--   0 benjamin  (1000) users      (100)      330 2024-05-13 22:46:42.000000 model_checker-0.3.4/test/test_examples.py
```

### Comparing `model_checker-0.3.3/LICENCE` & `model_checker-0.3.4/LICENCE`

 * *Files identical despite different names*

### Comparing `model_checker-0.3.3/PKG-INFO` & `model_checker-0.3.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: model-checker
-Version: 0.3.3
+Version: 0.3.4
 Summary: A hyperintensional model checker for counterfactual conditionals
 Author-email: Benjamin Brast-McKie <benbrastmckie@gmail.com>, Miguel Buitrago <mbuit82@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/benbrastmckie/ModelChecker
 Project-URL: Issues, https://github.com/benbrastmckie/ModelChecker/issues
 Keywords: semantics,Z3,counterfactuals,model checker,theorem prover,hyperintensionality
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `model_checker-0.3.3/README.md` & `model_checker-0.3.4/README.md`

 * *Files identical despite different names*

### Comparing `model_checker-0.3.3/pyproject.toml` & `model_checker-0.3.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=42", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "model-checker"
-version = "0.3.3"
+version = "0.3.4"
 description = "A hyperintensional model checker for counterfactual conditionals"
 authors = [
     { name = "Benjamin Brast-McKie", email = "benbrastmckie@gmail.com" },
     { name = "Miguel Buitrago", email = "mbuit82@gmail.com" },
 ]
 license = { text = "MIT" }
 readme = "README.md"
```

### Comparing `model_checker-0.3.3/src/model_checker/__main__.py` & `model_checker-0.3.4/src/model_checker/__main__.py`

 * *Files identical despite different names*

### Comparing `model_checker-0.3.3/src/model_checker/model_definitions.py` & `model_checker-0.3.4/src/model_checker/model_definitions.py`

 * *Files identical despite different names*

### Comparing `model_checker-0.3.3/src/model_checker/model_structure.py` & `model_checker-0.3.4/src/model_checker/model_structure.py`

 * *Files identical despite different names*

### Comparing `model_checker-0.3.3/src/model_checker/semantics.py` & `model_checker-0.3.4/src/model_checker/semantics.py`

 * *Files identical despite different names*

### Comparing `model_checker-0.3.3/src/model_checker/syntax.py` & `model_checker-0.3.4/src/model_checker/syntax.py`

 * *Files identical despite different names*

### Comparing `model_checker-0.3.3/src/model_checker/temp.py` & `model_checker-0.3.4/src/model_checker/temp.py`

 * *Files identical despite different names*

### Comparing `model_checker-0.3.3/src/model_checker/test.py` & `model_checker-0.3.4/src/model_checker/test.py`

 * *Files identical despite different names*

### Comparing `model_checker-0.3.3/src/model_checker.egg-info/PKG-INFO` & `model_checker-0.3.4/src/model_checker.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: model-checker
-Version: 0.3.3
+Version: 0.3.4
 Summary: A hyperintensional model checker for counterfactual conditionals
 Author-email: Benjamin Brast-McKie <benbrastmckie@gmail.com>, Miguel Buitrago <mbuit82@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/benbrastmckie/ModelChecker
 Project-URL: Issues, https://github.com/benbrastmckie/ModelChecker/issues
 Keywords: semantics,Z3,counterfactuals,model checker,theorem prover,hyperintensionality
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `model_checker-0.3.3/src/model_checker.egg-info/SOURCES.txt` & `model_checker-0.3.4/src/model_checker.egg-info/SOURCES.txt`

 * *Files identical despite different names*

