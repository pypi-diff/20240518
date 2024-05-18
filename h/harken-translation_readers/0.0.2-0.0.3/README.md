# Comparing `tmp/harken_translation_readers-0.0.2.tar.gz` & `tmp/harken_translation_readers-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "harken_translation_readers-0.0.2.tar", max compression
+gzip compressed data, was "harken_translation_readers-0.0.3.tar", max compression
```

## Comparing `harken_translation_readers-0.0.2.tar` & `harken_translation_readers-0.0.3.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0       30 2024-05-17 14:47:35.700507 harken_translation_readers-0.0.2/README.md
--rw-r--r--   0        0        0      914 2024-05-17 15:14:28.083353 harken_translation_readers-0.0.2/pyproject.toml
--rw-r--r--   0        0        0      201 2024-05-17 15:14:08.355299 harken_translation_readers-0.0.2/translation_readers/__init__.py
--rw-r--r--   0        0        0      580 2024-05-17 15:14:21.199335 harken_translation_readers-0.0.2/translation_readers/reader.py
--rw-r--r--   0        0        0     1813 2024-05-17 14:57:19.929813 harken_translation_readers-0.0.2/translation_readers/tmx_reader.py
--rw-r--r--   0        0        0      915 1970-01-01 00:00:00.000000 harken_translation_readers-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0       30 2024-05-17 14:47:35.700507 harken_translation_readers-0.0.3/README.md
+-rw-r--r--   0        0        0      914 2024-05-17 21:30:10.946065 harken_translation_readers-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0      201 2024-05-17 15:14:08.355299 harken_translation_readers-0.0.3/translation_readers/__init__.py
+-rw-r--r--   0        0        0      580 2024-05-17 15:14:21.199335 harken_translation_readers-0.0.3/translation_readers/reader.py
+-rw-r--r--   0        0        0     1842 2024-05-17 21:30:03.566057 harken_translation_readers-0.0.3/translation_readers/tmx_reader.py
+-rw-r--r--   0        0        0      915 1970-01-01 00:00:00.000000 harken_translation_readers-0.0.3/PKG-INFO
```

### Comparing `harken_translation_readers-0.0.2/pyproject.toml` & `harken_translation_readers-0.0.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "harken-translation_readers"
-version = "0.0.2"
+version = "0.0.3"
 description = "..."
 authors = ["Juan Luis García <juanluis1702@gmail.com>"]
 readme = "README.md"
 packages = [{include = "translation_readers"}]
 
 [tool.poetry.dependencies]
 python = ">=3"
```

### Comparing `harken_translation_readers-0.0.2/translation_readers/reader.py` & `harken_translation_readers-0.0.3/translation_readers/reader.py`

 * *Files identical despite different names*

### Comparing `harken_translation_readers-0.0.2/translation_readers/tmx_reader.py` & `harken_translation_readers-0.0.3/translation_readers/tmx_reader.py`

 * *Files 10% similar despite different names*

```diff
@@ -12,25 +12,25 @@
 
 
 class TmxReader(Reader):
 
     def __init__(self, input_path, src_lang, tgt_lang, **kwargs):
         super().__init__(input_path, src_lang, tgt_lang, **kwargs)
         self.switch_lang = False
+        self.factor=kwargs.get("factor",0.01)
         self.parse_data()
 
     def parse_data(self):
         try:
             with open(self.input_path, 'r', encoding='utf-16') as reader:
                 self.tmx_file = tmxfile(reader, self.src_lang, self.tgt_lang)
         except:
             with open(self.input_path, 'rb') as reader:
                 self.tmx_file = tmxfile(reader, self.src_lang, self.tgt_lang)
-        factor = 0.01
-        patience = int(factor * len(self.tmx_file.units))
+        patience = int(self.factor * len(self.tmx_file.units))
         patience = patience if len(self.tmx_file.units) <= 1000 else 100
         for node in self.tmx_file.unit_iter():
             src_tmp = detect_language_code(node.source, iso=ISO_639_2)
             tgt_tmp = detect_language_code(node.target, iso=ISO_639_2)
             if src_tmp == self.src_lang and \
                     tgt_tmp == self.tgt_lang:
                 break
```

### Comparing `harken_translation_readers-0.0.2/PKG-INFO` & `harken_translation_readers-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: harken-translation_readers
-Version: 0.0.2
+Version: 0.0.3
 Summary: ...
 Author: Juan Luis García
 Author-email: juanluis1702@gmail.com
 Requires-Python: >=3
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
```

