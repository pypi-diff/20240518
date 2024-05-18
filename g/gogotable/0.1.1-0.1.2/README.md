# Comparing `tmp/gogotable-0.1.1.tar.gz` & `tmp/gogotable-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gogotable-0.1.1.tar", max compression
+gzip compressed data, was "gogotable-0.1.2.tar", max compression
```

## Comparing `gogotable-0.1.1.tar` & `gogotable-0.1.2.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1211 2024-04-27 14:32:31.956850 gogotable-0.1.1/LICENSE
--rw-r--r--   0        0        0     1178 2024-04-27 14:32:31.957569 gogotable-0.1.1/README.md
--rw-r--r--   0        0        0      848 2024-05-17 14:40:27.759263 gogotable-0.1.1/pyproject.toml
--rw-r--r--   0        0        0       41 2024-04-27 14:32:31.961336 gogotable-0.1.1/src/gogotable/__init__.py
--rw-r--r--   0        0        0     1455 2024-05-17 14:39:24.799795 gogotable-0.1.1/src/gogotable/gogotable.py
--rw-r--r--   0        0        0     1704 1970-01-01 00:00:00.000000 gogotable-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1211 2024-04-27 14:32:31.956850 gogotable-0.1.2/LICENSE
+-rw-r--r--   0        0        0     1178 2024-04-27 14:32:31.957569 gogotable-0.1.2/README.md
+-rw-r--r--   0        0        0      848 2024-05-18 17:26:51.724721 gogotable-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0       41 2024-04-27 14:32:31.961336 gogotable-0.1.2/src/gogotable/__init__.py
+-rw-r--r--   0        0        0     1390 2024-05-18 17:24:18.721199 gogotable-0.1.2/src/gogotable/gogotable.py
+-rw-r--r--   0        0        0     1704 1970-01-01 00:00:00.000000 gogotable-0.1.2/PKG-INFO
```

### Comparing `gogotable-0.1.1/LICENSE` & `gogotable-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `gogotable-0.1.1/README.md` & `gogotable-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `gogotable-0.1.1/pyproject.toml` & `gogotable-0.1.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 [tool.isort]
 profile = "black"
 multi_line_output = 3
 
 [tool.poetry]
 name = "gogotable"
-version = "0.1.1"
+version = "0.1.2"
 description = "Convert structured data to a table"
 authors = ["Luís Miranda <luistm@gmail.com>"]
 license = "The Unlicense"
 readme = "README.md"
 packages = [{ include = "gogotable", from = "src" }]
 exclude = ["**/*_test.py"]
```

### Comparing `gogotable-0.1.1/PKG-INFO` & `gogotable-0.1.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gogotable
-Version: 0.1.1
+Version: 0.1.2
 Summary: Convert structured data to a table
 License: Unlicense
 Author: Luís Miranda
 Author-email: luistm@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved
 Classifier: Programming Language :: Python :: 3
```

