# Comparing `tmp/harken_translation_readers-0.0.4.tar.gz` & `tmp/harken_translation_readers-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "harken_translation_readers-0.0.4.tar", max compression
+gzip compressed data, was "harken_translation_readers-0.0.5.tar", max compression
```

## Comparing `harken_translation_readers-0.0.4.tar` & `harken_translation_readers-0.0.5.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0       30 2024-05-17 14:47:35.700507 harken_translation_readers-0.0.4/README.md
--rw-r--r--   0        0        0      914 2024-05-18 09:16:34.105039 harken_translation_readers-0.0.4/pyproject.toml
--rw-r--r--   0        0        0      201 2024-05-17 15:14:08.355299 harken_translation_readers-0.0.4/translation_readers/__init__.py
--rw-r--r--   0        0        0      580 2024-05-17 15:14:21.199335 harken_translation_readers-0.0.4/translation_readers/reader.py
--rw-r--r--   0        0        0     1842 2024-05-17 21:30:03.566057 harken_translation_readers-0.0.4/translation_readers/tmx_reader.py
--rw-r--r--   0        0        0     2051 2024-05-18 09:16:28.317085 harken_translation_readers-0.0.4/translation_readers/txt_reader.py
--rw-r--r--   0        0        0      915 1970-01-01 00:00:00.000000 harken_translation_readers-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0       30 2024-05-17 14:47:35.700507 harken_translation_readers-0.0.5/README.md
+-rw-r--r--   0        0        0      914 2024-05-18 09:17:22.420647 harken_translation_readers-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0      240 2024-05-18 09:17:14.088715 harken_translation_readers-0.0.5/translation_readers/__init__.py
+-rw-r--r--   0        0        0      580 2024-05-17 15:14:21.199335 harken_translation_readers-0.0.5/translation_readers/reader.py
+-rw-r--r--   0        0        0     1842 2024-05-17 21:30:03.566057 harken_translation_readers-0.0.5/translation_readers/tmx_reader.py
+-rw-r--r--   0        0        0     2051 2024-05-18 09:16:28.317085 harken_translation_readers-0.0.5/translation_readers/txt_reader.py
+-rw-r--r--   0        0        0      915 1970-01-01 00:00:00.000000 harken_translation_readers-0.0.5/PKG-INFO
```

### Comparing `harken_translation_readers-0.0.4/pyproject.toml` & `harken_translation_readers-0.0.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "harken-translation_readers"
-version = "0.0.4"
+version = "0.0.5"
 description = "..."
 authors = ["Juan Luis García <juanluis1702@gmail.com>"]
 readme = "README.md"
 packages = [{include = "translation_readers"}]
 
 [tool.poetry.dependencies]
 python = ">=3"
```

### Comparing `harken_translation_readers-0.0.4/translation_readers/reader.py` & `harken_translation_readers-0.0.5/translation_readers/reader.py`

 * *Files identical despite different names*

### Comparing `harken_translation_readers-0.0.4/translation_readers/tmx_reader.py` & `harken_translation_readers-0.0.5/translation_readers/tmx_reader.py`

 * *Files identical despite different names*

### Comparing `harken_translation_readers-0.0.4/translation_readers/txt_reader.py` & `harken_translation_readers-0.0.5/translation_readers/txt_reader.py`

 * *Files identical despite different names*

### Comparing `harken_translation_readers-0.0.4/PKG-INFO` & `harken_translation_readers-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: harken-translation_readers
-Version: 0.0.4
+Version: 0.0.5
 Summary: ...
 Author: Juan Luis García
 Author-email: juanluis1702@gmail.com
 Requires-Python: >=3
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
```

