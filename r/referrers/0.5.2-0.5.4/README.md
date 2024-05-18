# Comparing `tmp/referrers-0.5.2.tar.gz` & `tmp/referrers-0.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "referrers-0.5.2.tar", max compression
+gzip compressed data, was "referrers-0.5.4.tar", max compression
```

## Comparing `referrers-0.5.2.tar` & `referrers-0.5.4.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0    11357 2024-05-17 22:14:31.718328 referrers-0.5.2/LICENSE
--rw-r--r--   0        0        0     7536 2024-05-17 22:14:31.718328 referrers-0.5.2/README.md
--rw-r--r--   0        0        0      435 2024-05-17 22:14:31.718328 referrers-0.5.2/pyproject.toml
--rw-r--r--   0        0        0      130 2024-05-17 22:14:31.718328 referrers-0.5.2/src/referrers/__init__.py
--rw-r--r--   0        0        0    42056 2024-05-17 22:14:31.718328 referrers-0.5.2/src/referrers/impl.py
--rw-r--r--   0        0        0     8069 1970-01-01 00:00:00.000000 referrers-0.5.2/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-05-18 15:00:31.976243 referrers-0.5.4/LICENSE
+-rw-r--r--   0        0        0     7536 2024-05-18 15:00:31.976243 referrers-0.5.4/README.md
+-rw-r--r--   0        0        0      423 2024-05-18 15:00:31.976243 referrers-0.5.4/pyproject.toml
+-rw-r--r--   0        0        0      130 2024-05-18 15:00:31.976243 referrers-0.5.4/src/referrers/__init__.py
+-rw-r--r--   0        0        0    42056 2024-05-18 15:00:31.976243 referrers-0.5.4/src/referrers/impl.py
+-rw-r--r--   0        0        0     8177 1970-01-01 00:00:00.000000 referrers-0.5.4/PKG-INFO
```

### Comparing `referrers-0.5.2/LICENSE` & `referrers-0.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `referrers-0.5.2/README.md` & `referrers-0.5.4/README.md`

 * *Files identical despite different names*

### Comparing `referrers-0.5.2/src/referrers/impl.py` & `referrers-0.5.4/src/referrers/impl.py`

 * *Files identical despite different names*

### Comparing `referrers-0.5.2/PKG-INFO` & `referrers-0.5.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 Metadata-Version: 2.1
 Name: referrers
-Version: 0.5.2
+Version: 0.5.4
 Summary: Finds the graph of referrers for a Python object
+Home-page: https://github.com/nfergu/referrers
 Author: Neil Ferguson
 Requires-Python: >=3.8
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: networkx (>=3.1.0)
+Project-URL: Repository, https://github.com/nfergu/referrers
 Description-Content-Type: text/markdown
 
 # Referrers
 
 Referrers is a Python package that helps to answer the question **"what is holding
 a reference to this object?"**, which is useful for debugging memory leaks and other
 issues. It tries to assign a meaningful name to each reference to an object and
```

