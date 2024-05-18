# Comparing `tmp/pydatagenerator-0.0.0.tar.gz` & `tmp/pydatagenerator-0.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydatagenerator-0.0.0.tar", last modified: Fri May  3 07:25:48 2024, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `pydatagenerator-0.0.0.tar` & `pydatagenerator-0.0.1.tar`

### file list

```diff
@@ -1,13 +1,32 @@
-drwxrwxrwx   0        0        0        0 2024-05-03 07:25:48.739529 pydatagenerator-0.0.0/
--rw-rw-rw-   0        0        0     1100 2024-05-03 07:16:54.000000 pydatagenerator-0.0.0/LICENSE
--rw-rw-rw-   0        0        0      167 2024-05-03 07:25:48.734421 pydatagenerator-0.0.0/PKG-INFO
--rw-rw-rw-   0        0        0       17 2024-05-03 07:16:54.000000 pydatagenerator-0.0.0/README.md
--rw-rw-rw-   0        0        0      165 2024-05-03 07:22:57.000000 pydatagenerator-0.0.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-03 07:25:48.740516 pydatagenerator-0.0.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-05-03 07:25:48.699750 pydatagenerator-0.0.0/src/
--rw-rw-rw-   0        0        0        0 2024-05-03 07:22:36.000000 pydatagenerator-0.0.0/src/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-03 07:25:48.726704 pydatagenerator-0.0.0/src/pydatagenerator.egg-info/
--rw-rw-rw-   0        0        0      167 2024-05-03 07:25:48.000000 pydatagenerator-0.0.0/src/pydatagenerator.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      220 2024-05-03 07:25:48.000000 pydatagenerator-0.0.0/src/pydatagenerator.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-03 07:25:48.000000 pydatagenerator-0.0.0/src/pydatagenerator.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2024-05-03 07:25:48.000000 pydatagenerator-0.0.0/src/pydatagenerator.egg-info/top_level.txt
+-rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 pydatagenerator-0.0.1/CHANGELOG.md
+-rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 pydatagenerator-0.0.1/mkdocs.yml
+-rw-r--r--   0        0        0     3308 2020-02-02 00:00:00.000000 pydatagenerator-0.0.1/.github/workflows/publish.yml
+-rw-r--r--   0        0        0     1103 2020-02-02 00:00:00.000000 pydatagenerator-0.0.1/.vscode/launch.json
+-rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 pydatagenerator-0.0.1/.vscode/settings.json
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 pydatagenerator-0.0.1/docs/index.md
+-rw-r--r--   0        0        0      472 2020-02-02 00:00:00.000000 pydatagenerator-0.0.1/docs/reference/reference.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pydatagenerator-0.0.1/src/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pydatagenerator-0.0.1/src/pydatagenerator/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pydatagenerator-0.0.1/src/pydatagenerator/data/__init__.py
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 pydatagenerator-0.0.1/src/pydatagenerator/data/abstract/__init__.py
+-rw-r--r--   0        0        0     3401 2020-02-02 00:00:00.000000 pydatagenerator-0.0.1/src/pydatagenerator/data/abstract/abstract_dataset.py
+-rw-r--r--   0        0        0      561 2020-02-02 00:00:00.000000 pydatagenerator-0.0.1/src/pydatagenerator/data/abstract/abstract_dataset_handler_factory.py
+-rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 pydatagenerator-0.0.1/src/pydatagenerator/data/impl/__init__.py
+-rw-r--r--   0        0        0     1036 2020-02-02 00:00:00.000000 pydatagenerator-0.0.1/src/pydatagenerator/data/impl/dataset_handler_factory.py
+-rw-r--r--   0        0        0     1149 2020-02-02 00:00:00.000000 pydatagenerator-0.0.1/src/pydatagenerator/data/impl/random_number_data_set.py
+-rw-r--r--   0        0        0     1214 2020-02-02 00:00:00.000000 pydatagenerator-0.0.1/src/pydatagenerator/data/impl/sequence_data_set.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pydatagenerator-0.0.1/src/pydatagenerator/xml/__init__.py
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 pydatagenerator-0.0.1/src/pydatagenerator/xml/abstract/__init__.py
+-rw-r--r--   0        0        0      792 2020-02-02 00:00:00.000000 pydatagenerator-0.0.1/src/pydatagenerator/xml/abstract/abstract_xml_parser.py
+-rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 pydatagenerator-0.0.1/src/pydatagenerator/xml/impl/__init__.py
+-rw-r--r--   0        0        0     3374 2020-02-02 00:00:00.000000 pydatagenerator-0.0.1/src/pydatagenerator/xml/impl/xml_parser.py
+-rw-r--r--   0        0        0      513 2020-02-02 00:00:00.000000 pydatagenerator-0.0.1/src/pydatagenerator/xml/impl/xml_parser_util.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pydatagenerator-0.0.1/tests/__init__.py
+-rw-r--r--   0        0        0     3358 2020-02-02 00:00:00.000000 pydatagenerator-0.0.1/tests/pydatagenerator/data/random_number_data_set_test.py
+-rw-r--r--   0        0        0      459 2020-02-02 00:00:00.000000 pydatagenerator-0.0.1/tests/pydatagenerator/data/sequence_data_set_test.py
+-rw-r--r--   0        0        0     1725 2020-02-02 00:00:00.000000 pydatagenerator-0.0.1/tests/pydatagenerator/xml/xml_parser_test.py
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 pydatagenerator-0.0.1/.gitignore
+-rw-r--r--   0        0        0     1079 2020-02-02 00:00:00.000000 pydatagenerator-0.0.1/LICENSE
+-rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 pydatagenerator-0.0.1/README.md
+-rw-r--r--   0        0        0     1820 2020-02-02 00:00:00.000000 pydatagenerator-0.0.1/pyproject.toml
+-rw-r--r--   0        0        0     2666 2020-02-02 00:00:00.000000 pydatagenerator-0.0.1/PKG-INFO
```

### Comparing `pydatagenerator-0.0.0/LICENSE` & `pydatagenerator-0.0.1/LICENSE`

 * *Ordering differences only*

 * *Files 13% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-MIT License
-
-Copyright (c) 2024 Ionut-Alexandru Prodan
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+MIT License
+
+Copyright (c) 2024 Ionut-Alexandru Prodan
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
```

