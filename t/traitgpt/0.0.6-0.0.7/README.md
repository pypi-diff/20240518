# Comparing `tmp/traitgpt-0.0.6.tar.gz` & `tmp/traitgpt-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "traitgpt-0.0.6.tar", max compression
+gzip compressed data, was "traitgpt-0.0.7.tar", max compression
```

## Comparing `traitgpt-0.0.6.tar` & `traitgpt-0.0.7.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1070 2024-05-18 12:02:55.676765 traitgpt-0.0.6/LICENSE
--rw-r--r--   0        0        0     1062 2024-05-18 12:02:55.676765 traitgpt-0.0.6/README.md
--rw-r--r--   0        0        0     1421 2024-05-18 12:02:55.680765 traitgpt-0.0.6/pyproject.toml
--rw-r--r--   0        0        0       38 2024-05-18 12:02:55.680765 traitgpt-0.0.6/tests/__init__.py
--rw-r--r--   0        0        0     4822 2024-05-18 12:02:55.680765 traitgpt-0.0.6/tests/exampledata/MeSH_test.csv
--rw-r--r--   0        0        0      202 2024-05-18 12:02:55.680765 traitgpt-0.0.6/tests/exampledata/trait.txt
--rw-r--r--   0        0        0      408 2024-05-18 12:02:55.680765 traitgpt-0.0.6/tests/exampledata/trait_map.txt
--rw-r--r--   0        0        0     2165 2024-05-18 12:02:55.680765 traitgpt-0.0.6/tests/test_traitgpt.py
--rw-r--r--   0        0        0      432 2024-05-18 12:02:55.680765 traitgpt-0.0.6/traitgpt/__init__.py
--rw-r--r--   0        0        0     2396 2024-05-18 12:02:55.680765 traitgpt-0.0.6/traitgpt/cli.py
--rw-r--r--   0        0        0      844 2024-05-18 12:02:55.680765 traitgpt-0.0.6/traitgpt/prompts.py
--rw-r--r--   0        0        0     4827 2024-05-18 12:02:55.680765 traitgpt-0.0.6/traitgpt/traitgpt.py
--rw-r--r--   0        0        0     1926 1970-01-01 00:00:00.000000 traitgpt-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0     1070 2024-05-18 12:18:45.402451 traitgpt-0.0.7/LICENSE
+-rw-r--r--   0        0        0     1062 2024-05-18 12:18:45.402451 traitgpt-0.0.7/README.md
+-rw-r--r--   0        0        0     1518 2024-05-18 12:18:45.406451 traitgpt-0.0.7/pyproject.toml
+-rw-r--r--   0        0        0       38 2024-05-18 12:18:45.406451 traitgpt-0.0.7/tests/__init__.py
+-rw-r--r--   0        0        0     4822 2024-05-18 12:18:45.406451 traitgpt-0.0.7/tests/exampledata/MeSH_test.csv
+-rw-r--r--   0        0        0      202 2024-05-18 12:18:45.406451 traitgpt-0.0.7/tests/exampledata/trait.txt
+-rw-r--r--   0        0        0      408 2024-05-18 12:18:45.406451 traitgpt-0.0.7/tests/exampledata/trait_map.txt
+-rw-r--r--   0        0        0     2165 2024-05-18 12:18:45.406451 traitgpt-0.0.7/tests/test_traitgpt.py
+-rw-r--r--   0        0        0      432 2024-05-18 12:18:45.406451 traitgpt-0.0.7/traitgpt/__init__.py
+-rw-r--r--   0        0        0     2396 2024-05-18 12:18:45.406451 traitgpt-0.0.7/traitgpt/cli.py
+-rw-r--r--   0        0        0      844 2024-05-18 12:18:45.406451 traitgpt-0.0.7/traitgpt/prompts.py
+-rw-r--r--   0        0        0     4827 2024-05-18 12:18:45.406451 traitgpt-0.0.7/traitgpt/traitgpt.py
+-rw-r--r--   0        0        0     2108 1970-01-01 00:00:00.000000 traitgpt-0.0.7/PKG-INFO
```

### Comparing `traitgpt-0.0.6/LICENSE` & `traitgpt-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `traitgpt-0.0.6/README.md` & `traitgpt-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `traitgpt-0.0.6/pyproject.toml` & `traitgpt-0.0.7/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool]
 [tool.poetry]
 name = "traitgpt"
-version = "0.0.6"
+version = "0.0.7"
 homepage = "https://github.com/Jianhua-Wang/traitgpt"
 description = "Mapping trait to ontology using GPT."
 authors = ["Jianhua Wang <jianhua.mert@gmail.com>"]
 readme = "README.md"
 license =  "MIT"
 classifiers=[
     'Development Status :: 2 - Pre-Alpha',
@@ -21,14 +21,18 @@
     { include = "traitgpt" },
     { include = "tests", format = "sdist" },
 ]
 
 [tool.poetry.dependencies]
 python = ">=3.9,<3.13"
 typer = "^0.7.0"
+rich = "^13.7.1"
+langchain-community = "^0.2.0"
+langchain-openai = "^0.1.7"
+faiss-cpu = "^1.8.0"
 
 [tool.poetry.scripts]
 traitgpt = 'traitgpt.cli:app'
 
 [tool.poetry.dev-dependencies]
 black = "^23.9.1"
 isort = "^5.12.0"
```

### Comparing `traitgpt-0.0.6/tests/exampledata/MeSH_test.csv` & `traitgpt-0.0.7/tests/exampledata/MeSH_test.csv`

 * *Files identical despite different names*

### Comparing `traitgpt-0.0.6/tests/test_traitgpt.py` & `traitgpt-0.0.7/tests/test_traitgpt.py`

 * *Files identical despite different names*

### Comparing `traitgpt-0.0.6/traitgpt/cli.py` & `traitgpt-0.0.7/traitgpt/cli.py`

 * *Files identical despite different names*

### Comparing `traitgpt-0.0.6/traitgpt/prompts.py` & `traitgpt-0.0.7/traitgpt/prompts.py`

 * *Files identical despite different names*

### Comparing `traitgpt-0.0.6/traitgpt/traitgpt.py` & `traitgpt-0.0.7/traitgpt/traitgpt.py`

 * *Files identical despite different names*

### Comparing `traitgpt-0.0.6/PKG-INFO` & `traitgpt-0.0.7/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: traitgpt
-Version: 0.0.6
+Version: 0.0.7
 Summary: Mapping trait to ontology using GPT.
 Home-page: https://github.com/Jianhua-Wang/traitgpt
 License: MIT
 Author: Jianhua Wang
 Author-email: jianhua.mert@gmail.com
 Requires-Python: >=3.9,<3.13
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -14,14 +14,18 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+Requires-Dist: faiss-cpu (>=1.8.0,<2.0.0)
+Requires-Dist: langchain-community (>=0.2.0,<0.3.0)
+Requires-Dist: langchain-openai (>=0.1.7,<0.2.0)
+Requires-Dist: rich (>=13.7.1,<14.0.0)
 Requires-Dist: typer (>=0.7.0,<0.8.0)
 Description-Content-Type: text/markdown
 
 # TraitGPT
 
 
 [![pypi](https://img.shields.io/pypi/v/traitgpt.svg)](https://pypi.org/project/traitgpt/)
```

