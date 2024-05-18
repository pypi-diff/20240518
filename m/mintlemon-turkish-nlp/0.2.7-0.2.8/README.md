# Comparing `tmp/mintlemon-turkish-nlp-0.2.7.tar.gz` & `tmp/mintlemon-turkish-nlp-0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mintlemon-turkish-nlp-0.2.7.tar", last modified: Sat May 18 17:05:15 2024, max compression
+gzip compressed data, was "mintlemon-turkish-nlp-0.2.8.tar", last modified: Sat May 18 17:11:03 2024, max compression
```

## Comparing `mintlemon-turkish-nlp-0.2.7.tar` & `mintlemon-turkish-nlp-0.2.8.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 koc        (501) staff       (20)        0 2024-05-18 17:05:15.926974 mintlemon-turkish-nlp-0.2.7/
--rw-r--r--   0 koc        (501) staff       (20)      784 2024-02-16 12:29:01.000000 mintlemon-turkish-nlp-0.2.7/AUTHORS.rst
--rw-r--r--   0 koc        (501) staff       (20)    11357 2024-02-16 12:29:01.000000 mintlemon-turkish-nlp-0.2.7/LICENSE
--rw-r--r--   0 koc        (501) staff       (20)       75 2024-02-16 12:29:01.000000 mintlemon-turkish-nlp-0.2.7/MANIFEST.in
--rw-r--r--   0 koc        (501) staff       (20)     3823 2024-05-18 17:05:15.926465 mintlemon-turkish-nlp-0.2.7/PKG-INFO
--rw-r--r--   0 koc        (501) staff       (20)     1772 2024-02-16 12:29:01.000000 mintlemon-turkish-nlp-0.2.7/README.md
-drwxr-xr-x   0 koc        (501) staff       (20)        0 2024-05-18 17:05:15.917905 mintlemon-turkish-nlp-0.2.7/mintlemon/
--rw-r--r--   0 koc        (501) staff       (20)      275 2024-02-19 23:15:49.000000 mintlemon-turkish-nlp-0.2.7/mintlemon/__init__.py
-drwxr-xr-x   0 koc        (501) staff       (20)        0 2024-05-18 17:05:15.919523 mintlemon-turkish-nlp-0.2.7/mintlemon/data/
--rw-r--r--   0 koc        (501) staff       (20)     1565 2024-02-16 12:29:01.000000 mintlemon-turkish-nlp-0.2.7/mintlemon/data/TR_non_breaking_prefixes.txt
--rw-r--r--   0 koc        (501) staff       (20)   159044 2024-02-16 12:29:01.000000 mintlemon-turkish-nlp-0.2.7/mintlemon/data/ascii_to_str_dict.pickle
--rw-r--r--   0 koc        (501) staff       (20)     4260 2024-02-16 12:29:01.000000 mintlemon-turkish-nlp-0.2.7/mintlemon/data/stop_words.txt
-drwxr-xr-x   0 koc        (501) staff       (20)        0 2024-05-18 17:05:15.921059 mintlemon-turkish-nlp-0.2.7/mintlemon/normalizer/
--rw-r--r--   0 koc        (501) staff       (20)      138 2024-02-16 12:29:01.000000 mintlemon-turkish-nlp-0.2.7/mintlemon/normalizer/__init__.py
--rw-r--r--   0 koc        (501) staff       (20)    15189 2024-02-16 12:29:01.000000 mintlemon-turkish-nlp-0.2.7/mintlemon/normalizer/_builtin.py
--rw-r--r--   0 koc        (501) staff       (20)    12341 2024-02-16 12:50:56.000000 mintlemon-turkish-nlp-0.2.7/mintlemon/normalizer/normalizer.py
--rw-r--r--   0 koc        (501) staff       (20)     3025 2024-02-16 12:29:01.000000 mintlemon-turkish-nlp-0.2.7/mintlemon/normalizer/text_to_root_dtm.py
-drwxr-xr-x   0 koc        (501) staff       (20)        0 2024-05-18 17:05:15.921762 mintlemon-turkish-nlp-0.2.7/mintlemon/sentence_splitter/
--rw-r--r--   0 koc        (501) staff       (20)       80 2024-02-16 12:29:01.000000 mintlemon-turkish-nlp-0.2.7/mintlemon/sentence_splitter/__init__.py
--rw-r--r--   0 koc        (501) staff       (20)     1592 2024-02-16 12:29:01.000000 mintlemon-turkish-nlp-0.2.7/mintlemon/sentence_splitter/sentence_splitter.py
-drwxr-xr-x   0 koc        (501) staff       (20)        0 2024-05-18 17:05:15.922512 mintlemon-turkish-nlp-0.2.7/mintlemon/turkish_spellcheck/
--rw-r--r--   0 koc        (501) staff       (20)       88 2024-02-19 23:14:58.000000 mintlemon-turkish-nlp-0.2.7/mintlemon/turkish_spellcheck/__init__.py
--rw-r--r--   0 koc        (501) staff       (20)     4263 2024-02-20 16:36:02.000000 mintlemon-turkish-nlp-0.2.7/mintlemon/turkish_spellcheck/turkish_spellchecker.py
-drwxr-xr-x   0 koc        (501) staff       (20)        0 2024-05-18 17:05:15.924783 mintlemon-turkish-nlp-0.2.7/mintlemon_turkish_nlp.egg-info/
--rw-r--r--   0 koc        (501) staff       (20)     3823 2024-05-18 17:05:15.000000 mintlemon-turkish-nlp-0.2.7/mintlemon_turkish_nlp.egg-info/PKG-INFO
--rw-r--r--   0 koc        (501) staff       (20)      750 2024-05-18 17:05:15.000000 mintlemon-turkish-nlp-0.2.7/mintlemon_turkish_nlp.egg-info/SOURCES.txt
--rw-r--r--   0 koc        (501) staff       (20)        1 2024-05-18 17:05:15.000000 mintlemon-turkish-nlp-0.2.7/mintlemon_turkish_nlp.egg-info/dependency_links.txt
--rw-r--r--   0 koc        (501) staff       (20)      133 2024-05-18 17:05:15.000000 mintlemon-turkish-nlp-0.2.7/mintlemon_turkish_nlp.egg-info/requires.txt
--rw-r--r--   0 koc        (501) staff       (20)       10 2024-05-18 17:05:15.000000 mintlemon-turkish-nlp-0.2.7/mintlemon_turkish_nlp.egg-info/top_level.txt
--rw-r--r--   0 koc        (501) staff       (20)     1087 2024-02-16 12:29:01.000000 mintlemon-turkish-nlp-0.2.7/pyproject.toml
--rw-r--r--   0 koc        (501) staff       (20)       38 2024-05-18 17:05:15.927077 mintlemon-turkish-nlp-0.2.7/setup.cfg
--rw-r--r--   0 koc        (501) staff       (20)     2272 2024-05-18 17:04:06.000000 mintlemon-turkish-nlp-0.2.7/setup.py
+drwxr-xr-x   0 koc        (501) staff       (20)        0 2024-05-18 17:11:03.027296 mintlemon-turkish-nlp-0.2.8/
+-rw-r--r--   0 koc        (501) staff       (20)      784 2024-02-16 12:29:01.000000 mintlemon-turkish-nlp-0.2.8/AUTHORS.rst
+-rw-r--r--   0 koc        (501) staff       (20)    11357 2024-02-16 12:29:01.000000 mintlemon-turkish-nlp-0.2.8/LICENSE
+-rw-r--r--   0 koc        (501) staff       (20)       75 2024-02-16 12:29:01.000000 mintlemon-turkish-nlp-0.2.8/MANIFEST.in
+-rw-r--r--   0 koc        (501) staff       (20)     3823 2024-05-18 17:11:03.026825 mintlemon-turkish-nlp-0.2.8/PKG-INFO
+-rw-r--r--   0 koc        (501) staff       (20)     1772 2024-02-16 12:29:01.000000 mintlemon-turkish-nlp-0.2.8/README.md
+drwxr-xr-x   0 koc        (501) staff       (20)        0 2024-05-18 17:11:03.018590 mintlemon-turkish-nlp-0.2.8/mintlemon/
+-rw-r--r--   0 koc        (501) staff       (20)      275 2024-02-19 23:15:49.000000 mintlemon-turkish-nlp-0.2.8/mintlemon/__init__.py
+drwxr-xr-x   0 koc        (501) staff       (20)        0 2024-05-18 17:11:03.020059 mintlemon-turkish-nlp-0.2.8/mintlemon/data/
+-rw-r--r--   0 koc        (501) staff       (20)     1565 2024-02-16 12:29:01.000000 mintlemon-turkish-nlp-0.2.8/mintlemon/data/TR_non_breaking_prefixes.txt
+-rw-r--r--   0 koc        (501) staff       (20)   159044 2024-02-16 12:29:01.000000 mintlemon-turkish-nlp-0.2.8/mintlemon/data/ascii_to_str_dict.pickle
+-rw-r--r--   0 koc        (501) staff       (20)     4260 2024-02-16 12:29:01.000000 mintlemon-turkish-nlp-0.2.8/mintlemon/data/stop_words.txt
+drwxr-xr-x   0 koc        (501) staff       (20)        0 2024-05-18 17:11:03.021544 mintlemon-turkish-nlp-0.2.8/mintlemon/normalizer/
+-rw-r--r--   0 koc        (501) staff       (20)      138 2024-02-16 12:29:01.000000 mintlemon-turkish-nlp-0.2.8/mintlemon/normalizer/__init__.py
+-rw-r--r--   0 koc        (501) staff       (20)    15189 2024-02-16 12:29:01.000000 mintlemon-turkish-nlp-0.2.8/mintlemon/normalizer/_builtin.py
+-rw-r--r--   0 koc        (501) staff       (20)    12341 2024-02-16 12:50:56.000000 mintlemon-turkish-nlp-0.2.8/mintlemon/normalizer/normalizer.py
+-rw-r--r--   0 koc        (501) staff       (20)     3025 2024-02-16 12:29:01.000000 mintlemon-turkish-nlp-0.2.8/mintlemon/normalizer/text_to_root_dtm.py
+drwxr-xr-x   0 koc        (501) staff       (20)        0 2024-05-18 17:11:03.022279 mintlemon-turkish-nlp-0.2.8/mintlemon/sentence_splitter/
+-rw-r--r--   0 koc        (501) staff       (20)       80 2024-02-16 12:29:01.000000 mintlemon-turkish-nlp-0.2.8/mintlemon/sentence_splitter/__init__.py
+-rw-r--r--   0 koc        (501) staff       (20)     1592 2024-02-16 12:29:01.000000 mintlemon-turkish-nlp-0.2.8/mintlemon/sentence_splitter/sentence_splitter.py
+drwxr-xr-x   0 koc        (501) staff       (20)        0 2024-05-18 17:11:03.023017 mintlemon-turkish-nlp-0.2.8/mintlemon/turkish_spellcheck/
+-rw-r--r--   0 koc        (501) staff       (20)       88 2024-02-19 23:14:58.000000 mintlemon-turkish-nlp-0.2.8/mintlemon/turkish_spellcheck/__init__.py
+-rw-r--r--   0 koc        (501) staff       (20)     4263 2024-02-20 16:36:02.000000 mintlemon-turkish-nlp-0.2.8/mintlemon/turkish_spellcheck/turkish_spellchecker.py
+drwxr-xr-x   0 koc        (501) staff       (20)        0 2024-05-18 17:11:03.025434 mintlemon-turkish-nlp-0.2.8/mintlemon_turkish_nlp.egg-info/
+-rw-r--r--   0 koc        (501) staff       (20)     3823 2024-05-18 17:11:02.000000 mintlemon-turkish-nlp-0.2.8/mintlemon_turkish_nlp.egg-info/PKG-INFO
+-rw-r--r--   0 koc        (501) staff       (20)      750 2024-05-18 17:11:02.000000 mintlemon-turkish-nlp-0.2.8/mintlemon_turkish_nlp.egg-info/SOURCES.txt
+-rw-r--r--   0 koc        (501) staff       (20)        1 2024-05-18 17:11:02.000000 mintlemon-turkish-nlp-0.2.8/mintlemon_turkish_nlp.egg-info/dependency_links.txt
+-rw-r--r--   0 koc        (501) staff       (20)      133 2024-05-18 17:11:02.000000 mintlemon-turkish-nlp-0.2.8/mintlemon_turkish_nlp.egg-info/requires.txt
+-rw-r--r--   0 koc        (501) staff       (20)       10 2024-05-18 17:11:02.000000 mintlemon-turkish-nlp-0.2.8/mintlemon_turkish_nlp.egg-info/top_level.txt
+-rw-r--r--   0 koc        (501) staff       (20)     1087 2024-02-16 12:29:01.000000 mintlemon-turkish-nlp-0.2.8/pyproject.toml
+-rw-r--r--   0 koc        (501) staff       (20)       38 2024-05-18 17:11:03.027394 mintlemon-turkish-nlp-0.2.8/setup.cfg
+-rw-r--r--   0 koc        (501) staff       (20)     2272 2024-05-18 17:10:47.000000 mintlemon-turkish-nlp-0.2.8/setup.py
```

### Comparing `mintlemon-turkish-nlp-0.2.7/AUTHORS.rst` & `mintlemon-turkish-nlp-0.2.8/AUTHORS.rst`

 * *Files identical despite different names*

### Comparing `mintlemon-turkish-nlp-0.2.7/LICENSE` & `mintlemon-turkish-nlp-0.2.8/LICENSE`

 * *Files identical despite different names*

### Comparing `mintlemon-turkish-nlp-0.2.7/PKG-INFO` & `mintlemon-turkish-nlp-0.2.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mintlemon-turkish-nlp
-Version: 0.2.7
+Version: 0.2.8
 Summary: Mint & Lemon Turkish NLP Library developed by Mint & Lemon Development Team.
 Home-page: https://github.com/Teknofest-Nane-Limon/mintlemon-turkish-nlp
 Author: Mint&Lemon
 License: Apache License, Version 2.0
 Project-URL: Tracker, https://github.com/Teknofest-Nane-Limon/mintlemon-turkish-nlp/issues
 Project-URL: Documentation, https://mintlemon-turkish-nlp.readthedocs.io
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `mintlemon-turkish-nlp-0.2.7/README.md` & `mintlemon-turkish-nlp-0.2.8/README.md`

 * *Files identical despite different names*

### Comparing `mintlemon-turkish-nlp-0.2.7/mintlemon/data/TR_non_breaking_prefixes.txt` & `mintlemon-turkish-nlp-0.2.8/mintlemon/data/TR_non_breaking_prefixes.txt`

 * *Files identical despite different names*

### Comparing `mintlemon-turkish-nlp-0.2.7/mintlemon/data/ascii_to_str_dict.pickle` & `mintlemon-turkish-nlp-0.2.8/mintlemon/data/ascii_to_str_dict.pickle`

 * *Files identical despite different names*

### Comparing `mintlemon-turkish-nlp-0.2.7/mintlemon/data/stop_words.txt` & `mintlemon-turkish-nlp-0.2.8/mintlemon/data/stop_words.txt`

 * *Files identical despite different names*

### Comparing `mintlemon-turkish-nlp-0.2.7/mintlemon/normalizer/_builtin.py` & `mintlemon-turkish-nlp-0.2.8/mintlemon/normalizer/_builtin.py`

 * *Files identical despite different names*

### Comparing `mintlemon-turkish-nlp-0.2.7/mintlemon/normalizer/normalizer.py` & `mintlemon-turkish-nlp-0.2.8/mintlemon/normalizer/normalizer.py`

 * *Files identical despite different names*

### Comparing `mintlemon-turkish-nlp-0.2.7/mintlemon/normalizer/text_to_root_dtm.py` & `mintlemon-turkish-nlp-0.2.8/mintlemon/normalizer/text_to_root_dtm.py`

 * *Files identical despite different names*

### Comparing `mintlemon-turkish-nlp-0.2.7/mintlemon/sentence_splitter/sentence_splitter.py` & `mintlemon-turkish-nlp-0.2.8/mintlemon/sentence_splitter/sentence_splitter.py`

 * *Files identical despite different names*

### Comparing `mintlemon-turkish-nlp-0.2.7/mintlemon/turkish_spellcheck/turkish_spellchecker.py` & `mintlemon-turkish-nlp-0.2.8/mintlemon/turkish_spellcheck/turkish_spellchecker.py`

 * *Files identical despite different names*

### Comparing `mintlemon-turkish-nlp-0.2.7/mintlemon_turkish_nlp.egg-info/PKG-INFO` & `mintlemon-turkish-nlp-0.2.8/mintlemon_turkish_nlp.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mintlemon-turkish-nlp
-Version: 0.2.7
+Version: 0.2.8
 Summary: Mint & Lemon Turkish NLP Library developed by Mint & Lemon Development Team.
 Home-page: https://github.com/Teknofest-Nane-Limon/mintlemon-turkish-nlp
 Author: Mint&Lemon
 License: Apache License, Version 2.0
 Project-URL: Tracker, https://github.com/Teknofest-Nane-Limon/mintlemon-turkish-nlp/issues
 Project-URL: Documentation, https://mintlemon-turkish-nlp.readthedocs.io
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `mintlemon-turkish-nlp-0.2.7/mintlemon_turkish_nlp.egg-info/SOURCES.txt` & `mintlemon-turkish-nlp-0.2.8/mintlemon_turkish_nlp.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mintlemon-turkish-nlp-0.2.7/pyproject.toml` & `mintlemon-turkish-nlp-0.2.8/pyproject.toml`

 * *Files identical despite different names*

### Comparing `mintlemon-turkish-nlp-0.2.7/setup.py` & `mintlemon-turkish-nlp-0.2.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 def get_long_description():
     with open("README.md", "r", encoding="utf-8") as f:
         return f.read()
 
 setup(
     name="mintlemon-turkish-nlp",
-    version = "0.2.7",
+    version = "0.2.8",
     description="Mint & Lemon Turkish NLP Library developed by Mint & Lemon Development Team.",
     author="Mint&Lemon",
     license="Apache License, Version 2.0",
     long_description=get_long_description(),
     long_description_content_type="text/markdown",
     url="https://github.com/Teknofest-Nane-Limon/mintlemon-turkish-nlp",
     project_urls={
```

