# Comparing `tmp/traitgpt-0.0.7.tar.gz` & `tmp/traitgpt-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "traitgpt-0.0.7.tar", max compression
+gzip compressed data, was "traitgpt-0.0.8.tar", max compression
```

## Comparing `traitgpt-0.0.7.tar` & `traitgpt-0.0.8.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1070 2024-05-18 12:18:45.402451 traitgpt-0.0.7/LICENSE
--rw-r--r--   0        0        0     1062 2024-05-18 12:18:45.402451 traitgpt-0.0.7/README.md
--rw-r--r--   0        0        0     1518 2024-05-18 12:18:45.406451 traitgpt-0.0.7/pyproject.toml
--rw-r--r--   0        0        0       38 2024-05-18 12:18:45.406451 traitgpt-0.0.7/tests/__init__.py
--rw-r--r--   0        0        0     4822 2024-05-18 12:18:45.406451 traitgpt-0.0.7/tests/exampledata/MeSH_test.csv
--rw-r--r--   0        0        0      202 2024-05-18 12:18:45.406451 traitgpt-0.0.7/tests/exampledata/trait.txt
--rw-r--r--   0        0        0      408 2024-05-18 12:18:45.406451 traitgpt-0.0.7/tests/exampledata/trait_map.txt
--rw-r--r--   0        0        0     2165 2024-05-18 12:18:45.406451 traitgpt-0.0.7/tests/test_traitgpt.py
--rw-r--r--   0        0        0      432 2024-05-18 12:18:45.406451 traitgpt-0.0.7/traitgpt/__init__.py
--rw-r--r--   0        0        0     2396 2024-05-18 12:18:45.406451 traitgpt-0.0.7/traitgpt/cli.py
--rw-r--r--   0        0        0      844 2024-05-18 12:18:45.406451 traitgpt-0.0.7/traitgpt/prompts.py
--rw-r--r--   0        0        0     4827 2024-05-18 12:18:45.406451 traitgpt-0.0.7/traitgpt/traitgpt.py
--rw-r--r--   0        0        0     2108 1970-01-01 00:00:00.000000 traitgpt-0.0.7/PKG-INFO
+-rw-r--r--   0        0        0     1070 2024-05-18 12:35:21.304245 traitgpt-0.0.8/LICENSE
+-rw-r--r--   0        0        0     1062 2024-05-18 12:35:21.304245 traitgpt-0.0.8/README.md
+-rw-r--r--   0        0        0     1566 2024-05-18 12:35:21.304245 traitgpt-0.0.8/pyproject.toml
+-rw-r--r--   0        0        0       38 2024-05-18 12:35:21.304245 traitgpt-0.0.8/tests/__init__.py
+-rw-r--r--   0        0        0     4822 2024-05-18 12:35:21.304245 traitgpt-0.0.8/tests/exampledata/MeSH_test.csv
+-rw-r--r--   0        0        0      202 2024-05-18 12:35:21.304245 traitgpt-0.0.8/tests/exampledata/trait.txt
+-rw-r--r--   0        0        0      408 2024-05-18 12:35:21.304245 traitgpt-0.0.8/tests/exampledata/trait_map.txt
+-rw-r--r--   0        0        0     2165 2024-05-18 12:35:21.304245 traitgpt-0.0.8/tests/test_traitgpt.py
+-rw-r--r--   0        0        0      432 2024-05-18 12:35:21.304245 traitgpt-0.0.8/traitgpt/__init__.py
+-rw-r--r--   0        0        0     2771 2024-05-18 12:35:21.304245 traitgpt-0.0.8/traitgpt/cli.py
+-rw-r--r--   0        0        0      844 2024-05-18 12:35:21.304245 traitgpt-0.0.8/traitgpt/prompts.py
+-rw-r--r--   0        0        0     4827 2024-05-18 12:35:21.304245 traitgpt-0.0.8/traitgpt/traitgpt.py
+-rw-r--r--   0        0        0     2008 1970-01-01 00:00:00.000000 traitgpt-0.0.8/PKG-INFO
```

### Comparing `traitgpt-0.0.7/LICENSE` & `traitgpt-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `traitgpt-0.0.7/README.md` & `traitgpt-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `traitgpt-0.0.7/pyproject.toml` & `traitgpt-0.0.8/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 [tool]
 [tool.poetry]
 name = "traitgpt"
-version = "0.0.7"
+version = "0.0.8"
 homepage = "https://github.com/Jianhua-Wang/traitgpt"
 description = "Mapping trait to ontology using GPT."
 authors = ["Jianhua Wang <jianhua.mert@gmail.com>"]
 readme = "README.md"
 license =  "MIT"
 classifiers=[
     'Development Status :: 2 - Pre-Alpha',
     'Intended Audience :: Developers',
     'License :: OSI Approved :: MIT License',
     'Natural Language :: English',
     'Programming Language :: Python :: 3',
-    'Programming Language :: Python :: 3.7',
-    'Programming Language :: Python :: 3.8',
     'Programming Language :: Python :: 3.9',
+    'Programming Language :: Python :: 3.10',
+    'Programming Language :: Python :: 3.11',
+    'Programming Language :: Python :: 3.12',
 ]
 packages = [
     { include = "traitgpt" },
     { include = "tests", format = "sdist" },
 ]
 
 [tool.poetry.dependencies]
```

### Comparing `traitgpt-0.0.7/tests/exampledata/MeSH_test.csv` & `traitgpt-0.0.8/tests/exampledata/MeSH_test.csv`

 * *Files identical despite different names*

### Comparing `traitgpt-0.0.7/tests/test_traitgpt.py` & `traitgpt-0.0.8/tests/test_traitgpt.py`

 * *Files identical despite different names*

### Comparing `traitgpt-0.0.7/traitgpt/cli.py` & `traitgpt-0.0.8/traitgpt/cli.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """Console script for traitgpt."""
 
 import logging
 
 import typer
+from langchain_community.callbacks import get_openai_callback
 from rich.console import Console
 
 from . import __version__
 
 CONTEXT_SETTINGS = dict(help_option_names=["-h", "--help"])
 app = typer.Typer(context_settings=CONTEXT_SETTINGS, add_completion=False)
 
@@ -60,18 +61,23 @@
     ),
 ):
     """Search the vocabulary."""
     from traitgpt import TraitGPT
 
     tg = TraitGPT(index_path=index_path)
     out_write = open(outfile, "w")
-    with open(infile, "r") as f:
-        for line in f:
-            res = tg.map_trait(line.strip())
-            term_name, term_id = res.get("term_name"), res.get("term_id")
-            logging.info(f"{line.strip()} -> {term_name} | {term_id}")
-            out_write.write(f"{line.strip()}\t{term_name}\t{term_id}\n")
-    out_write.close()
+    with get_openai_callback() as cb:
+        with open(infile, "r") as f:
+            for line in f:
+                res = tg.map_trait(line.strip())
+                term_name, term_id = res.get("term_name"), res.get("term_id")
+                logging.info(f"{line.strip()} -> {term_name} | {term_id}")
+                out_write.write(f"{line.strip()}\t{term_name}\t{term_id}\n")
+        out_write.close()
+        console.print(f"Prompt Tokens: {cb.prompt_tokens}")
+        console.print(f"Completion Tokens: {cb.completion_tokens}")
+        console.print(f"Total Tokens: {cb.total_tokens}")
+        console.print(f"Total Cost (USD): ${cb.total_cost}")
 
 
 if __name__ == "__main__":
     app()
```

### Comparing `traitgpt-0.0.7/traitgpt/prompts.py` & `traitgpt-0.0.8/traitgpt/prompts.py`

 * *Files identical despite different names*

### Comparing `traitgpt-0.0.7/traitgpt/traitgpt.py` & `traitgpt-0.0.8/traitgpt/traitgpt.py`

 * *Files identical despite different names*

### Comparing `traitgpt-0.0.7/PKG-INFO` & `traitgpt-0.0.8/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: traitgpt
-Version: 0.0.7
+Version: 0.0.8
 Summary: Mapping trait to ontology using GPT.
 Home-page: https://github.com/Jianhua-Wang/traitgpt
 License: MIT
 Author: Jianhua Wang
 Author-email: jianhua.mert@gmail.com
 Requires-Python: >=3.9,<3.13
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -12,16 +12,14 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
 Requires-Dist: faiss-cpu (>=1.8.0,<2.0.0)
 Requires-Dist: langchain-community (>=0.2.0,<0.3.0)
 Requires-Dist: langchain-openai (>=0.1.7,<0.2.0)
 Requires-Dist: rich (>=13.7.1,<14.0.0)
 Requires-Dist: typer (>=0.7.0,<0.8.0)
 Description-Content-Type: text/markdown
```

