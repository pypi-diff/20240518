# Comparing `tmp/referrers-0.5.1.tar.gz` & `tmp/referrers-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "referrers-0.5.1.tar", max compression
+gzip compressed data, was "referrers-0.5.2.tar", max compression
```

## Comparing `referrers-0.5.1.tar` & `referrers-0.5.2.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0    11357 2024-05-17 22:02:23.190553 referrers-0.5.1/LICENSE
--rw-r--r--   0        0        0     7536 2024-05-17 22:02:23.190553 referrers-0.5.1/README.md
--rw-r--r--   0        0        0      372 2024-05-17 22:02:23.190553 referrers-0.5.1/pyproject.toml
--rw-r--r--   0        0        0      130 2024-05-17 22:02:23.190553 referrers-0.5.1/src/referrers/__init__.py
--rw-r--r--   0        0        0    42056 2024-05-17 22:02:23.190553 referrers-0.5.1/src/referrers/impl.py
--rw-r--r--   0        0        0     8069 1970-01-01 00:00:00.000000 referrers-0.5.1/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-05-17 22:14:31.718328 referrers-0.5.2/LICENSE
+-rw-r--r--   0        0        0     7536 2024-05-17 22:14:31.718328 referrers-0.5.2/README.md
+-rw-r--r--   0        0        0      435 2024-05-17 22:14:31.718328 referrers-0.5.2/pyproject.toml
+-rw-r--r--   0        0        0      130 2024-05-17 22:14:31.718328 referrers-0.5.2/src/referrers/__init__.py
+-rw-r--r--   0        0        0    42056 2024-05-17 22:14:31.718328 referrers-0.5.2/src/referrers/impl.py
+-rw-r--r--   0        0        0     8069 1970-01-01 00:00:00.000000 referrers-0.5.2/PKG-INFO
```

### Comparing `referrers-0.5.1/LICENSE` & `referrers-0.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `referrers-0.5.1/README.md` & `referrers-0.5.2/README.md`

 * *Files identical despite different names*

### Comparing `referrers-0.5.1/src/referrers/impl.py` & `referrers-0.5.2/src/referrers/impl.py`

 * *Files identical despite different names*

### Comparing `referrers-0.5.1/PKG-INFO` & `referrers-0.5.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: referrers
-Version: 0.5.1
+Version: 0.5.2
 Summary: Finds the graph of referrers for a Python object
 Author: Neil Ferguson
 Requires-Python: >=3.8
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

