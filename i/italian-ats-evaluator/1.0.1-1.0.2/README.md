# Comparing `tmp/italian_ats_evaluator-1.0.1.tar.gz` & `tmp/italian_ats_evaluator-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "italian_ats_evaluator-1.0.1.tar", last modified: Sat May 18 20:42:13 2024, max compression
+gzip compressed data, was "italian_ats_evaluator-1.0.2.tar", last modified: Sat May 18 20:50:56 2024, max compression
```

## Comparing `italian_ats_evaluator-1.0.1.tar` & `italian_ats_evaluator-1.0.2.tar`

### file list

```diff
@@ -1,18 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 20:42:13.350514 italian_ats_evaluator-1.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-05-18 20:42:07.000000 italian_ats_evaluator-1.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3836 2024-05-18 20:42:13.350514 italian_ats_evaluator-1.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2141 2024-05-18 20:42:07.000000 italian_ats_evaluator-1.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 20:42:13.346513 italian_ats_evaluator-1.0.1/italian_ats_evaluator/
--rw-r--r--   0 runner    (1001) docker     (127)     2860 2024-05-18 20:42:07.000000 italian_ats_evaluator-1.0.1/italian_ats_evaluator/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 20:42:13.346513 italian_ats_evaluator-1.0.1/italian_ats_evaluator/nvdb/
--rw-r--r--   0 runner    (1001) docker     (127)    20485 2024-05-18 20:42:07.000000 italian_ats_evaluator-1.0.1/italian_ats_evaluator/nvdb/AD.txt
--rw-r--r--   0 runner    (1001) docker     (127)    27630 2024-05-18 20:42:07.000000 italian_ats_evaluator-1.0.1/italian_ats_evaluator/nvdb/AU.txt
--rw-r--r--   0 runner    (1001) docker     (127)    16107 2024-05-18 20:42:07.000000 italian_ats_evaluator-1.0.1/italian_ats_evaluator/nvdb/FO.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 20:42:13.346513 italian_ats_evaluator-1.0.1/italian_ats_evaluator.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3836 2024-05-18 20:42:13.000000 italian_ats_evaluator-1.0.1/italian_ats_evaluator.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      392 2024-05-18 20:42:13.000000 italian_ats_evaluator-1.0.1/italian_ats_evaluator.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-18 20:42:13.000000 italian_ats_evaluator-1.0.1/italian_ats_evaluator.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      115 2024-05-18 20:42:13.000000 italian_ats_evaluator-1.0.1/italian_ats_evaluator.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-18 20:42:13.000000 italian_ats_evaluator-1.0.1/italian_ats_evaluator.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1975 2024-05-18 20:42:07.000000 italian_ats_evaluator-1.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-18 20:42:13.350514 italian_ats_evaluator-1.0.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 20:50:56.255311 italian_ats_evaluator-1.0.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-05-18 20:50:50.000000 italian_ats_evaluator-1.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3836 2024-05-18 20:50:56.255311 italian_ats_evaluator-1.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2141 2024-05-18 20:50:50.000000 italian_ats_evaluator-1.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 20:50:56.251311 italian_ats_evaluator-1.0.2/italian_ats_evaluator/
+-rw-r--r--   0 runner    (1001) docker     (127)     2860 2024-05-18 20:50:50.000000 italian_ats_evaluator-1.0.2/italian_ats_evaluator/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 20:50:56.255311 italian_ats_evaluator-1.0.2/italian_ats_evaluator/analysis/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-18 20:50:50.000000 italian_ats_evaluator-1.0.2/italian_ats_evaluator/analysis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1098 2024-05-18 20:50:50.000000 italian_ats_evaluator-1.0.2/italian_ats_evaluator/analysis/basic_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1182 2024-05-18 20:50:50.000000 italian_ats_evaluator-1.0.2/italian_ats_evaluator/analysis/diff_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1829 2024-05-18 20:50:50.000000 italian_ats_evaluator-1.0.2/italian_ats_evaluator/analysis/pos_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1057 2024-05-18 20:50:50.000000 italian_ats_evaluator-1.0.2/italian_ats_evaluator/analysis/readability_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (127)      827 2024-05-18 20:50:50.000000 italian_ats_evaluator-1.0.2/italian_ats_evaluator/analysis/similarity_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1000 2024-05-18 20:50:50.000000 italian_ats_evaluator-1.0.2/italian_ats_evaluator/analysis/vdb_analysis.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 20:50:56.255311 italian_ats_evaluator-1.0.2/italian_ats_evaluator/nvdb/
+-rw-r--r--   0 runner    (1001) docker     (127)    20485 2024-05-18 20:50:50.000000 italian_ats_evaluator-1.0.2/italian_ats_evaluator/nvdb/AD.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    27630 2024-05-18 20:50:50.000000 italian_ats_evaluator-1.0.2/italian_ats_evaluator/nvdb/AU.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    16107 2024-05-18 20:50:50.000000 italian_ats_evaluator-1.0.2/italian_ats_evaluator/nvdb/FO.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 20:50:56.255311 italian_ats_evaluator-1.0.2/italian_ats_evaluator/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-18 20:50:50.000000 italian_ats_evaluator-1.0.2/italian_ats_evaluator/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      224 2024-05-18 20:50:50.000000 italian_ats_evaluator-1.0.2/italian_ats_evaluator/utils/nlp_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 20:50:56.255311 italian_ats_evaluator-1.0.2/italian_ats_evaluator.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3836 2024-05-18 20:50:56.000000 italian_ats_evaluator-1.0.2/italian_ats_evaluator.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      816 2024-05-18 20:50:56.000000 italian_ats_evaluator-1.0.2/italian_ats_evaluator.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-18 20:50:56.000000 italian_ats_evaluator-1.0.2/italian_ats_evaluator.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2024-05-18 20:50:56.000000 italian_ats_evaluator-1.0.2/italian_ats_evaluator.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-18 20:50:56.000000 italian_ats_evaluator-1.0.2/italian_ats_evaluator.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2002 2024-05-18 20:50:50.000000 italian_ats_evaluator-1.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-18 20:50:56.255311 italian_ats_evaluator-1.0.2/setup.cfg
```

### Comparing `italian_ats_evaluator-1.0.1/LICENSE` & `italian_ats_evaluator-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `italian_ats_evaluator-1.0.1/PKG-INFO` & `italian_ats_evaluator-1.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: italian-ats-evaluator
-Version: 1.0.1
+Version: 1.0.2
 Summary: Italian ATS Evaluator
 Author-email: RedHitMark <russodivito.marco@gmail.com>
 Maintainer-email: RedHitMark <russodivito.marco@gmail.com>
 License: MIT License
 Project-URL: Repository, https://github.com/RedHitMark/italian-ats-evaluator
 Project-URL: Issues, https://github.com/RedHitMark/italian-ats-evaluator/issues
 Keywords: ats,text,simplification,italian,nlp
```

### Comparing `italian_ats_evaluator-1.0.1/README.md` & `italian_ats_evaluator-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `italian_ats_evaluator-1.0.1/italian_ats_evaluator/__init__.py` & `italian_ats_evaluator-1.0.2/italian_ats_evaluator/__init__.py`

 * *Files identical despite different names*

### Comparing `italian_ats_evaluator-1.0.1/italian_ats_evaluator/nvdb/AD.txt` & `italian_ats_evaluator-1.0.2/italian_ats_evaluator/nvdb/AD.txt`

 * *Files identical despite different names*

### Comparing `italian_ats_evaluator-1.0.1/italian_ats_evaluator/nvdb/AU.txt` & `italian_ats_evaluator-1.0.2/italian_ats_evaluator/nvdb/AU.txt`

 * *Files identical despite different names*

### Comparing `italian_ats_evaluator-1.0.1/italian_ats_evaluator/nvdb/FO.txt` & `italian_ats_evaluator-1.0.2/italian_ats_evaluator/nvdb/FO.txt`

 * *Files identical despite different names*

### Comparing `italian_ats_evaluator-1.0.1/italian_ats_evaluator.egg-info/PKG-INFO` & `italian_ats_evaluator-1.0.2/italian_ats_evaluator.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: italian-ats-evaluator
-Version: 1.0.1
+Version: 1.0.2
 Summary: Italian ATS Evaluator
 Author-email: RedHitMark <russodivito.marco@gmail.com>
 Maintainer-email: RedHitMark <russodivito.marco@gmail.com>
 License: MIT License
 Project-URL: Repository, https://github.com/RedHitMark/italian-ats-evaluator
 Project-URL: Issues, https://github.com/RedHitMark/italian-ats-evaluator/issues
 Keywords: ats,text,simplification,italian,nlp
```

### Comparing `italian_ats_evaluator-1.0.1/pyproject.toml` & `italian_ats_evaluator-1.0.2/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "italian-ats-evaluator"
-version = "1.0.1"
+version = "1.0.2"
 description = "Italian ATS Evaluator"
 readme = {file = "README.md", content-type = "text/markdown"}
 license = {text = "MIT License"}
 authors = [{"name" = "RedHitMark", "email"= "russodivito.marco@gmail.com"}]
 maintainers = [{"name" = "RedHitMark", "email"= "russodivito.marco@gmail.com"}]
 keywords = ["ats", 'text', 'simplification', 'italian', 'nlp']
 classifiers=[
@@ -52,9 +52,9 @@
 [tool.setuptools]
 include-package-data = true
 
 [tool.setuptools.package-data]
 italian_ats_evaluator = ["nvdb/*.txt"]
 
 [tool.setuptools.packages.find]
-include = ["italian_ats_evaluator"]
+include = ["italian_ats_evaluator", "italian_ats_evaluator.*"]
 exclude = ["docs*", "tests*"]
```

