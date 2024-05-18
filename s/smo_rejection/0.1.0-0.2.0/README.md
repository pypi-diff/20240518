# Comparing `tmp/smo_rejection-0.1.0.tar.gz` & `tmp/smo_rejection-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "smo_rejection-0.1.0.tar", max compression
+gzip compressed data, was "smo_rejection-0.2.0.tar", max compression
```

## Comparing `smo_rejection-0.1.0.tar` & `smo_rejection-0.2.0.tar`

### file list

```diff
@@ -1,8 +1,9 @@
--rw-r--r--   0        0        0      283 2024-05-18 08:23:57.461799 smo_rejection-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     2061 2024-05-18 08:07:37.781285 smo_rejection-0.1.0/README.md
--rw-r--r--   0        0        0     1709 2024-05-18 08:07:37.784352 smo_rejection-0.1.0/smo_rejection/exception.py
--rw-r--r--   0        0        0     1628 2024-05-18 08:07:37.785364 smo_rejection-0.1.0/smo_rejection/models.py
--rw-r--r--   0        0        0     4417 2024-05-18 08:27:53.620739 smo_rejection-0.1.0/smo_rejection/processing.py
--rw-r--r--   0        0        0     4304 2024-05-18 08:30:20.844396 smo_rejection-0.1.0/smo_rejection/simulation.py
--rw-r--r--   0        0        0     2471 2024-05-18 08:09:14.671502 smo_rejection-0.1.0/smo_rejection/utils.py
--rw-r--r--   0        0        0     2357 1970-01-01 00:00:00.000000 smo_rejection-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      283 2024-05-18 09:16:32.071334 smo_rejection-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     2061 2024-05-18 09:16:32.069301 smo_rejection-0.2.0/README.md
+-rw-r--r--   0        0        0      101 2024-05-18 09:17:07.279398 smo_rejection-0.2.0/smo_rejection/__init__.py
+-rw-r--r--   0        0        0     1709 2024-05-18 09:16:32.075303 smo_rejection-0.2.0/smo_rejection/exception.py
+-rw-r--r--   0        0        0     1628 2024-05-18 09:16:32.076302 smo_rejection-0.2.0/smo_rejection/models.py
+-rw-r--r--   0        0        0     4417 2024-05-18 09:17:38.463921 smo_rejection-0.2.0/smo_rejection/processing.py
+-rw-r--r--   0        0        0     4304 2024-05-18 09:16:32.077303 smo_rejection-0.2.0/smo_rejection/simulation.py
+-rw-r--r--   0        0        0     2471 2024-05-18 09:16:32.077303 smo_rejection-0.2.0/smo_rejection/utils.py
+-rw-r--r--   0        0        0     2357 1970-01-01 00:00:00.000000 smo_rejection-0.2.0/PKG-INFO
```

### Comparing `smo_rejection-0.1.0/README.md` & `smo_rejection-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `smo_rejection-0.1.0/smo_rejection/exception.py` & `smo_rejection-0.2.0/smo_rejection/exception.py`

 * *Files identical despite different names*

### Comparing `smo_rejection-0.1.0/smo_rejection/models.py` & `smo_rejection-0.2.0/smo_rejection/models.py`

 * *Files identical despite different names*

### Comparing `smo_rejection-0.1.0/smo_rejection/processing.py` & `smo_rejection-0.2.0/smo_rejection/processing.py`

 * *Files identical despite different names*

### Comparing `smo_rejection-0.1.0/smo_rejection/simulation.py` & `smo_rejection-0.2.0/smo_rejection/simulation.py`

 * *Files identical despite different names*

### Comparing `smo_rejection-0.1.0/smo_rejection/utils.py` & `smo_rejection-0.2.0/smo_rejection/utils.py`

 * *Files identical despite different names*

### Comparing `smo_rejection-0.1.0/PKG-INFO` & `smo_rejection-0.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smo_rejection
-Version: 0.1.0
+Version: 0.2.0
 Summary: 
 Author: mbtmrw
 Author-email: keks2324098@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
```

