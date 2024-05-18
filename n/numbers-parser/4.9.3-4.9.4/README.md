# Comparing `tmp/numbers_parser-4.9.3.tar.gz` & `tmp/numbers_parser-4.9.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "numbers_parser-4.9.3.tar", max compression
+gzip compressed data, was "numbers_parser-4.9.4.tar", max compression
```

## Comparing `numbers_parser-4.9.3.tar` & `numbers_parser-4.9.4.tar`

### file list

```diff
@@ -1,59 +1,59 @@
--rw-r--r--   0        0        0     1050 2022-06-23 17:13:17.000000 numbers_parser-4.9.3/LICENSE.rst
--rw-r--r--   0        0        0    14890 2024-02-25 13:52:12.312621 numbers_parser-4.9.3/README.md
--rw-r--r--   0        0        0     3017 2024-02-25 19:45:07.827803 numbers_parser-4.9.3/pyproject.toml
--rw-r--r--   0        0        0     1950 2024-01-21 10:33:42.665265 numbers_parser-4.9.3/src/numbers_parser/__init__.py
--rw-r--r--   0        0        0     4619 2023-10-06 14:57:50.297129 numbers_parser-4.9.3/src/numbers_parser/_cat_numbers.py
--rw-r--r--   0        0        0     5689 2023-10-06 15:05:33.170136 numbers_parser-4.9.3/src/numbers_parser/_unpack_numbers.py
--rw-r--r--   0        0        0     2616 2023-10-06 11:10:41.000000 numbers_parser-4.9.3/src/numbers_parser/bullets.py
--rw-r--r--   0        0        0    38457 2024-02-25 09:36:24.697735 numbers_parser-4.9.3/src/numbers_parser/cell.py
--rw-r--r--   0        0        0    34354 2024-02-25 09:46:27.608403 numbers_parser-4.9.3/src/numbers_parser/cell_storage.py
--rw-r--r--   0        0        0     9606 2024-02-25 16:17:44.879160 numbers_parser-4.9.3/src/numbers_parser/constants.py
--rw-r--r--   0        0        0     4220 2024-02-25 15:57:58.075030 numbers_parser-4.9.3/src/numbers_parser/containers.py
--rw-r--r--   0        0        0     3767 2024-01-03 12:33:06.354196 numbers_parser-4.9.3/src/numbers_parser/currencies.py
--rwxr-xr-x   0        0        0    90316 2023-07-31 12:19:08.304273 numbers_parser-4.9.3/src/numbers_parser/data/empty.numbers
--rw-r--r--   0        0        0    55908 2024-02-25 17:44:37.445138 numbers_parser-4.9.3/src/numbers_parser/document.py
--rw-r--r--   0        0        0      670 2023-10-06 14:51:25.062892 numbers_parser-4.9.3/src/numbers_parser/exceptions.py
--rw-r--r--   0        0        0      374 2023-07-16 14:30:53.391296 numbers_parser-4.9.3/src/numbers_parser/experimental.py
--rw-r--r--   0        0        0     4111 2024-02-25 19:44:37.568600 numbers_parser-4.9.3/src/numbers_parser/file.py
--rw-r--r--   0        0        0    10572 2024-01-28 12:12:26.828534 numbers_parser-4.9.3/src/numbers_parser/formula.py
--rw-r--r--   0        0        0    16007 2023-09-22 14:45:03.344239 numbers_parser-4.9.3/src/numbers_parser/generated/TNArchives_pb2.py
--rw-r--r--   0        0        0     1215 2023-09-22 14:45:03.344533 numbers_parser-4.9.3/src/numbers_parser/generated/TNArchives_sos_pb2.py
--rw-r--r--   0        0        0    18271 2023-09-22 14:45:03.344777 numbers_parser-4.9.3/src/numbers_parser/generated/TNCommandArchives_pb2.py
--rw-r--r--   0        0        0     1857 2023-09-22 14:45:03.345248 numbers_parser-4.9.3/src/numbers_parser/generated/TNCommandArchives_sos_pb2.py
--rw-r--r--   0        0        0    19980 2023-09-22 14:45:03.345476 numbers_parser-4.9.3/src/numbers_parser/generated/TSAArchives_pb2.py
--rw-r--r--   0        0        0     2033 2023-09-22 14:45:03.345790 numbers_parser-4.9.3/src/numbers_parser/generated/TSAArchives_sos_pb2.py
--rw-r--r--   0        0        0     3907 2023-09-22 14:45:03.345971 numbers_parser-4.9.3/src/numbers_parser/generated/TSACommandArchives_sos_pb2.py
--rw-r--r--   0        0        0    64955 2023-09-22 14:45:03.346313 numbers_parser-4.9.3/src/numbers_parser/generated/TSCEArchives_pb2.py
--rw-r--r--   0        0        0    11162 2023-09-22 14:45:03.346882 numbers_parser-4.9.3/src/numbers_parser/generated/TSCH3DArchives_pb2.py
--rw-r--r--   0        0        0     8655 2023-09-22 14:45:03.347138 numbers_parser-4.9.3/src/numbers_parser/generated/TSCHArchives_Common_pb2.py
--rw-r--r--   0        0        0    46323 2023-09-22 14:45:03.347382 numbers_parser-4.9.3/src/numbers_parser/generated/TSCHArchives_GEN_pb2.py
--rw-r--r--   0        0        0    24187 2023-09-22 14:45:03.347681 numbers_parser-4.9.3/src/numbers_parser/generated/TSCHArchives_pb2.py
--rw-r--r--   0        0        0    63730 2023-09-22 14:45:03.347937 numbers_parser-4.9.3/src/numbers_parser/generated/TSCHArchives_sos_pb2.py
--rw-r--r--   0        0        0    27446 2023-09-22 14:45:03.348238 numbers_parser-4.9.3/src/numbers_parser/generated/TSCHCommandArchives_pb2.py
--rw-r--r--   0        0        0    30051 2023-09-22 14:45:03.348470 numbers_parser-4.9.3/src/numbers_parser/generated/TSCHPreUFFArchives_pb2.py
--rw-r--r--   0        0        0    40151 2023-09-22 14:45:03.348776 numbers_parser-4.9.3/src/numbers_parser/generated/TSDArchives_pb2.py
--rw-r--r--   0        0        0     6022 2023-09-22 14:45:03.349031 numbers_parser-4.9.3/src/numbers_parser/generated/TSDArchives_sos_pb2.py
--rw-r--r--   0        0        0    29192 2023-09-22 14:45:03.349425 numbers_parser-4.9.3/src/numbers_parser/generated/TSDCommandArchives_pb2.py
--rw-r--r--   0        0        0    53520 2023-09-22 14:45:03.349840 numbers_parser-4.9.3/src/numbers_parser/generated/TSKArchives_pb2.py
--rw-r--r--   0        0        0     1941 2023-09-22 14:45:03.350144 numbers_parser-4.9.3/src/numbers_parser/generated/TSKArchives_sos_pb2.py
--rw-r--r--   0        0        0    18142 2023-09-22 14:45:03.350375 numbers_parser-4.9.3/src/numbers_parser/generated/TSPArchiveMessages_pb2.py
--rw-r--r--   0        0        0     2024 2023-09-22 14:45:03.350630 numbers_parser-4.9.3/src/numbers_parser/generated/TSPDatabaseMessages_pb2.py
--rw-r--r--   0        0        0    12975 2023-09-22 14:45:03.350890 numbers_parser-4.9.3/src/numbers_parser/generated/TSPMessages_pb2.py
--rw-r--r--   0        0        0     9806 2023-09-22 14:45:03.351143 numbers_parser-4.9.3/src/numbers_parser/generated/TSSArchives_pb2.py
--rw-r--r--   0        0        0     2842 2023-09-22 14:45:03.351385 numbers_parser-4.9.3/src/numbers_parser/generated/TSSArchives_sos_pb2.py
--rw-r--r--   0        0        0    88532 2023-09-22 14:45:03.351767 numbers_parser-4.9.3/src/numbers_parser/generated/TSTArchives_pb2.py
--rw-r--r--   0        0        0    12597 2023-09-22 14:45:03.352516 numbers_parser-4.9.3/src/numbers_parser/generated/TSTArchives_sos_pb2.py
--rw-r--r--   0        0        0    59523 2023-09-22 14:45:03.352833 numbers_parser-4.9.3/src/numbers_parser/generated/TSTCommandArchives_pb2.py
--rw-r--r--   0        0        0    12644 2023-09-22 14:45:03.353148 numbers_parser-4.9.3/src/numbers_parser/generated/TSTStylePropertyArchiving_pb2.py
--rw-r--r--   0        0        0    59149 2023-09-22 14:45:03.353504 numbers_parser-4.9.3/src/numbers_parser/generated/TSWPArchives_pb2.py
--rw-r--r--   0        0        0    29114 2023-09-22 14:45:03.354254 numbers_parser-4.9.3/src/numbers_parser/generated/TSWPArchives_sos_pb2.py
--rw-r--r--   0        0        0    25441 2023-09-22 14:45:03.354496 numbers_parser-4.9.3/src/numbers_parser/generated/TSWPCommandArchives_pb2.py
--rw-r--r--   0        0        0        0 2023-09-22 14:45:03.358517 numbers_parser-4.9.3/src/numbers_parser/generated/__init__.py
--rw-r--r--   0        0        0    22748 2023-09-22 14:44:56.439021 numbers_parser-4.9.3/src/numbers_parser/generated/fontmap.py
--rw-r--r--   0        0        0     6082 2023-09-22 14:44:55.676419 numbers_parser-4.9.3/src/numbers_parser/generated/functionmap.py
--rw-r--r--   0        0        0    11833 2023-10-06 14:57:50.296152 numbers_parser-4.9.3/src/numbers_parser/iwafile.py
--rw-r--r--   0        0        0    32215 2023-10-06 11:10:41.000000 numbers_parser-4.9.3/src/numbers_parser/mapping.py
--rw-r--r--   0        0        0   103414 2024-02-25 19:29:06.390397 numbers_parser-4.9.3/src/numbers_parser/model.py
--rw-r--r--   0        0        0     1141 2024-02-24 08:45:59.061379 numbers_parser-4.9.3/src/numbers_parser/numbers_cache.py
--rw-r--r--   0        0        0     2642 2023-08-06 07:40:00.595714 numbers_parser-4.9.3/src/numbers_parser/numbers_uuid.py
--rw-r--r--   0        0        0    16197 1970-01-01 00:00:00.000000 numbers_parser-4.9.3/PKG-INFO
+-rw-r--r--   0        0        0     1050 2022-06-23 17:13:17.000000 numbers_parser-4.9.4/LICENSE.rst
+-rw-r--r--   0        0        0    14890 2024-02-25 13:52:12.312621 numbers_parser-4.9.4/README.md
+-rw-r--r--   0        0        0     3017 2024-02-25 20:34:00.451374 numbers_parser-4.9.4/pyproject.toml
+-rw-r--r--   0        0        0     1950 2024-01-21 10:33:42.665265 numbers_parser-4.9.4/src/numbers_parser/__init__.py
+-rw-r--r--   0        0        0     4619 2023-10-06 14:57:50.297129 numbers_parser-4.9.4/src/numbers_parser/_cat_numbers.py
+-rw-r--r--   0        0        0     5689 2023-10-06 15:05:33.170136 numbers_parser-4.9.4/src/numbers_parser/_unpack_numbers.py
+-rw-r--r--   0        0        0     2616 2023-10-06 11:10:41.000000 numbers_parser-4.9.4/src/numbers_parser/bullets.py
+-rw-r--r--   0        0        0    38457 2024-02-25 09:36:24.697735 numbers_parser-4.9.4/src/numbers_parser/cell.py
+-rw-r--r--   0        0        0    34354 2024-02-25 09:46:27.608403 numbers_parser-4.9.4/src/numbers_parser/cell_storage.py
+-rw-r--r--   0        0        0     9606 2024-02-25 16:17:44.879160 numbers_parser-4.9.4/src/numbers_parser/constants.py
+-rw-r--r--   0        0        0     4220 2024-02-25 15:57:58.075030 numbers_parser-4.9.4/src/numbers_parser/containers.py
+-rw-r--r--   0        0        0     3767 2024-01-03 12:33:06.354196 numbers_parser-4.9.4/src/numbers_parser/currencies.py
+-rwxr-xr-x   0        0        0    90316 2023-07-31 12:19:08.304273 numbers_parser-4.9.4/src/numbers_parser/data/empty.numbers
+-rw-r--r--   0        0        0    55908 2024-02-25 17:44:37.445138 numbers_parser-4.9.4/src/numbers_parser/document.py
+-rw-r--r--   0        0        0      670 2023-10-06 14:51:25.062892 numbers_parser-4.9.4/src/numbers_parser/exceptions.py
+-rw-r--r--   0        0        0      374 2023-07-16 14:30:53.391296 numbers_parser-4.9.4/src/numbers_parser/experimental.py
+-rw-r--r--   0        0        0     4111 2024-02-25 19:44:37.568600 numbers_parser-4.9.4/src/numbers_parser/file.py
+-rw-r--r--   0        0        0    10572 2024-01-28 12:12:26.828534 numbers_parser-4.9.4/src/numbers_parser/formula.py
+-rw-r--r--   0        0        0    16007 2023-09-22 14:45:03.344239 numbers_parser-4.9.4/src/numbers_parser/generated/TNArchives_pb2.py
+-rw-r--r--   0        0        0     1215 2023-09-22 14:45:03.344533 numbers_parser-4.9.4/src/numbers_parser/generated/TNArchives_sos_pb2.py
+-rw-r--r--   0        0        0    18271 2023-09-22 14:45:03.344777 numbers_parser-4.9.4/src/numbers_parser/generated/TNCommandArchives_pb2.py
+-rw-r--r--   0        0        0     1857 2023-09-22 14:45:03.345248 numbers_parser-4.9.4/src/numbers_parser/generated/TNCommandArchives_sos_pb2.py
+-rw-r--r--   0        0        0    19980 2023-09-22 14:45:03.345476 numbers_parser-4.9.4/src/numbers_parser/generated/TSAArchives_pb2.py
+-rw-r--r--   0        0        0     2033 2023-09-22 14:45:03.345790 numbers_parser-4.9.4/src/numbers_parser/generated/TSAArchives_sos_pb2.py
+-rw-r--r--   0        0        0     3907 2023-09-22 14:45:03.345971 numbers_parser-4.9.4/src/numbers_parser/generated/TSACommandArchives_sos_pb2.py
+-rw-r--r--   0        0        0    64955 2023-09-22 14:45:03.346313 numbers_parser-4.9.4/src/numbers_parser/generated/TSCEArchives_pb2.py
+-rw-r--r--   0        0        0    11162 2023-09-22 14:45:03.346882 numbers_parser-4.9.4/src/numbers_parser/generated/TSCH3DArchives_pb2.py
+-rw-r--r--   0        0        0     8655 2023-09-22 14:45:03.347138 numbers_parser-4.9.4/src/numbers_parser/generated/TSCHArchives_Common_pb2.py
+-rw-r--r--   0        0        0    46323 2023-09-22 14:45:03.347382 numbers_parser-4.9.4/src/numbers_parser/generated/TSCHArchives_GEN_pb2.py
+-rw-r--r--   0        0        0    24187 2023-09-22 14:45:03.347681 numbers_parser-4.9.4/src/numbers_parser/generated/TSCHArchives_pb2.py
+-rw-r--r--   0        0        0    63730 2023-09-22 14:45:03.347937 numbers_parser-4.9.4/src/numbers_parser/generated/TSCHArchives_sos_pb2.py
+-rw-r--r--   0        0        0    27446 2023-09-22 14:45:03.348238 numbers_parser-4.9.4/src/numbers_parser/generated/TSCHCommandArchives_pb2.py
+-rw-r--r--   0        0        0    30051 2023-09-22 14:45:03.348470 numbers_parser-4.9.4/src/numbers_parser/generated/TSCHPreUFFArchives_pb2.py
+-rw-r--r--   0        0        0    40151 2023-09-22 14:45:03.348776 numbers_parser-4.9.4/src/numbers_parser/generated/TSDArchives_pb2.py
+-rw-r--r--   0        0        0     6022 2023-09-22 14:45:03.349031 numbers_parser-4.9.4/src/numbers_parser/generated/TSDArchives_sos_pb2.py
+-rw-r--r--   0        0        0    29192 2023-09-22 14:45:03.349425 numbers_parser-4.9.4/src/numbers_parser/generated/TSDCommandArchives_pb2.py
+-rw-r--r--   0        0        0    53520 2023-09-22 14:45:03.349840 numbers_parser-4.9.4/src/numbers_parser/generated/TSKArchives_pb2.py
+-rw-r--r--   0        0        0     1941 2023-09-22 14:45:03.350144 numbers_parser-4.9.4/src/numbers_parser/generated/TSKArchives_sos_pb2.py
+-rw-r--r--   0        0        0    18142 2023-09-22 14:45:03.350375 numbers_parser-4.9.4/src/numbers_parser/generated/TSPArchiveMessages_pb2.py
+-rw-r--r--   0        0        0     2024 2023-09-22 14:45:03.350630 numbers_parser-4.9.4/src/numbers_parser/generated/TSPDatabaseMessages_pb2.py
+-rw-r--r--   0        0        0    12975 2023-09-22 14:45:03.350890 numbers_parser-4.9.4/src/numbers_parser/generated/TSPMessages_pb2.py
+-rw-r--r--   0        0        0     9806 2023-09-22 14:45:03.351143 numbers_parser-4.9.4/src/numbers_parser/generated/TSSArchives_pb2.py
+-rw-r--r--   0        0        0     2842 2023-09-22 14:45:03.351385 numbers_parser-4.9.4/src/numbers_parser/generated/TSSArchives_sos_pb2.py
+-rw-r--r--   0        0        0    88532 2023-09-22 14:45:03.351767 numbers_parser-4.9.4/src/numbers_parser/generated/TSTArchives_pb2.py
+-rw-r--r--   0        0        0    12597 2023-09-22 14:45:03.352516 numbers_parser-4.9.4/src/numbers_parser/generated/TSTArchives_sos_pb2.py
+-rw-r--r--   0        0        0    59523 2023-09-22 14:45:03.352833 numbers_parser-4.9.4/src/numbers_parser/generated/TSTCommandArchives_pb2.py
+-rw-r--r--   0        0        0    12644 2023-09-22 14:45:03.353148 numbers_parser-4.9.4/src/numbers_parser/generated/TSTStylePropertyArchiving_pb2.py
+-rw-r--r--   0        0        0    59149 2023-09-22 14:45:03.353504 numbers_parser-4.9.4/src/numbers_parser/generated/TSWPArchives_pb2.py
+-rw-r--r--   0        0        0    29114 2023-09-22 14:45:03.354254 numbers_parser-4.9.4/src/numbers_parser/generated/TSWPArchives_sos_pb2.py
+-rw-r--r--   0        0        0    25441 2023-09-22 14:45:03.354496 numbers_parser-4.9.4/src/numbers_parser/generated/TSWPCommandArchives_pb2.py
+-rw-r--r--   0        0        0        0 2023-09-22 14:45:03.358517 numbers_parser-4.9.4/src/numbers_parser/generated/__init__.py
+-rw-r--r--   0        0        0    22748 2023-09-22 14:44:56.439021 numbers_parser-4.9.4/src/numbers_parser/generated/fontmap.py
+-rw-r--r--   0        0        0     6082 2023-09-22 14:44:55.676419 numbers_parser-4.9.4/src/numbers_parser/generated/functionmap.py
+-rw-r--r--   0        0        0    11833 2023-10-06 14:57:50.296152 numbers_parser-4.9.4/src/numbers_parser/iwafile.py
+-rw-r--r--   0        0        0    32215 2023-10-06 11:10:41.000000 numbers_parser-4.9.4/src/numbers_parser/mapping.py
+-rw-r--r--   0        0        0   103341 2024-02-25 20:12:05.468830 numbers_parser-4.9.4/src/numbers_parser/model.py
+-rw-r--r--   0        0        0     1141 2024-02-24 08:45:59.061379 numbers_parser-4.9.4/src/numbers_parser/numbers_cache.py
+-rw-r--r--   0        0        0     2642 2023-08-06 07:40:00.595714 numbers_parser-4.9.4/src/numbers_parser/numbers_uuid.py
+-rw-r--r--   0        0        0    16197 1970-01-01 00:00:00.000000 numbers_parser-4.9.4/PKG-INFO
```

### Comparing `numbers_parser-4.9.3/LICENSE.rst` & `numbers_parser-4.9.4/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `numbers_parser-4.9.3/README.md` & `numbers_parser-4.9.4/README.md`

 * *Files identical despite different names*

### Comparing `numbers_parser-4.9.3/pyproject.toml` & `numbers_parser-4.9.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 description = "Read and write Apple Numbers spreadsheets"
 documentation = "https://github.com/masaccio/numbers-parser/blob/main/README.md"
 license = "MIT"
 name = "numbers-parser"
 packages = [{include = "numbers_parser", from = "src"}]
 readme = "README.md"
 repository = "https://github.com/masaccio/numbers-parser"
-version = "4.9.3"
+version = "4.9.4"
 
 [tool.poetry.scripts]
 cat-numbers = "numbers_parser._cat_numbers:main"
 unpack-numbers = "numbers_parser._unpack_numbers:main"
 
 [tool.poetry.dependencies]
 compact-json = "^1.1.3"
```

### Comparing `numbers_parser-4.9.3/src/numbers_parser/__init__.py` & `numbers_parser-4.9.4/src/numbers_parser/__init__.py`

 * *Files identical despite different names*

### Comparing `numbers_parser-4.9.3/src/numbers_parser/_cat_numbers.py` & `numbers_parser-4.9.4/src/numbers_parser/_cat_numbers.py`

 * *Files identical despite different names*

### Comparing `numbers_parser-4.9.3/src/numbers_parser/_unpack_numbers.py` & `numbers_parser-4.9.4/src/numbers_parser/_unpack_numbers.py`

 * *Files identical despite different names*

### Comparing `numbers_parser-4.9.3/src/numbers_parser/bullets.py` & `numbers_parser-4.9.4/src/numbers_parser/bullets.py`

 * *Files identical despite different names*

### Comparing `numbers_parser-4.9.3/src/numbers_parser/cell.py` & `numbers_parser-4.9.4/src/numbers_parser/cell.py`

 * *Files identical despite different names*

### Comparing `numbers_parser-4.9.3/src/numbers_parser/cell_storage.py` & `numbers_parser-4.9.4/src/numbers_parser/cell_storage.py`

 * *Files identical despite different names*

### Comparing `numbers_parser-4.9.3/src/numbers_parser/constants.py` & `numbers_parser-4.9.4/src/numbers_parser/constants.py`

 * *Files identical despite different names*

### Comparing `numbers_parser-4.9.3/src/numbers_parser/containers.py` & `numbers_parser-4.9.4/src/numbers_parser/containers.py`

 * *Files identical despite different names*

### Comparing `numbers_parser-4.9.3/src/numbers_parser/currencies.py` & `numbers_parser-4.9.4/src/numbers_parser/currencies.py`

 * *Files identical despite different names*

### Comparing `numbers_parser-4.9.3/src/numbers_parser/data/empty.numbers` & `numbers_parser-4.9.4/src/numbers_parser/data/empty.numbers`

 * *Files identical despite different names*

### Comparing `numbers_parser-4.9.3/src/numbers_parser/document.py` & `numbers_parser-4.9.4/src/numbers_parser/document.py`

 * *Files identical despite different names*

### Comparing `numbers_parser-4.9.3/src/numbers_parser/exceptions.py` & `numbers_parser-4.9.4/src/numbers_parser/exceptions.py`

 * *Files identical despite different names*

### Comparing `numbers_parser-4.9.3/src/numbers_parser/file.py` & `numbers_parser-4.9.4/src/numbers_parser/file.py`

 * *Files identical despite different names*

### Comparing `numbers_parser-4.9.3/src/numbers_parser/formula.py` & `numbers_parser-4.9.4/src/numbers_parser/formula.py`

 * *Files identical despite different names*

### Comparing `numbers_parser-4.9.3/src/numbers_parser/generated/TNArchives_pb2.py` & `numbers_parser-4.9.4/src/numbers_parser/generated/TNArchives_pb2.py`

 * *Files identical despite different names*

### Comparing `numbers_parser-4.9.3/src/numbers_parser/generated/TNArchives_sos_pb2.py` & `numbers_parser-4.9.4/src/numbers_parser/generated/TNArchives_sos_pb2.py`

 * *Files identical despite different names*

### Comparing `numbers_parser-4.9.3/src/numbers_parser/generated/TNCommandArchives_pb2.py` & `numbers_parser-4.9.4/src/numbers_parser/generated/TNCommandArchives_pb2.py`

 * *Files identical despite different names*

### Comparing `numbers_parser-4.9.3/src/numbers_parser/generated/TNCommandArchives_sos_pb2.py` & `numbers_parser-4.9.4/src/numbers_parser/generated/TNCommandArchives_sos_pb2.py`

 * *Files identical despite different names*

### Comparing `numbers_parser-4.9.3/src/numbers_parser/generated/TSAArchives_pb2.py` & `numbers_parser-4.9.4/src/numbers_parser/generated/TSAArchives_pb2.py`

 * *Files identical despite different names*

### Comparing `numbers_parser-4.9.3/src/numbers_parser/generated/TSAArchives_sos_pb2.py` & `numbers_parser-4.9.4/src/numbers_parser/generated/TSAArchives_sos_pb2.py`

 * *Files identical despite different names*

### Comparing `numbers_parser-4.9.3/src/numbers_parser/generated/TSACommandArchives_sos_pb2.py` & `numbers_parser-4.9.4/src/numbers_parser/generated/TSACommandArchives_sos_pb2.py`

 * *Files identical despite different names*

### Comparing `numbers_parser-4.9.3/src/numbers_parser/generated/TSCEArchives_pb2.py` & `numbers_parser-4.9.4/src/numbers_parser/generated/TSCEArchives_pb2.py`

 * *Files identical despite different names*

### Comparing `numbers_parser-4.9.3/src/numbers_parser/generated/TSCH3DArchives_pb2.py` & `numbers_parser-4.9.4/src/numbers_parser/generated/TSCH3DArchives_pb2.py`

 * *Files identical despite different names*

### Comparing `numbers_parser-4.9.3/src/numbers_parser/generated/TSCHArchives_Common_pb2.py` & `numbers_parser-4.9.4/src/numbers_parser/generated/TSCHArchives_Common_pb2.py`

 * *Files identical despite different names*

### Comparing `numbers_parser-4.9.3/src/numbers_parser/generated/TSCHArchives_GEN_pb2.py` & `numbers_parser-4.9.4/src/numbers_parser/generated/TSCHArchives_GEN_pb2.py`

 * *Files identical despite different names*

### Comparing `numbers_parser-4.9.3/src/numbers_parser/generated/TSCHArchives_pb2.py` & `numbers_parser-4.9.4/src/numbers_parser/generated/TSCHArchives_pb2.py`

 * *Files identical despite different names*

### Comparing `numbers_parser-4.9.3/src/numbers_parser/generated/TSCHArchives_sos_pb2.py` & `numbers_parser-4.9.4/src/numbers_parser/generated/TSCHArchives_sos_pb2.py`

 * *Files identical despite different names*

### Comparing `numbers_parser-4.9.3/src/numbers_parser/generated/TSCHCommandArchives_pb2.py` & `numbers_parser-4.9.4/src/numbers_parser/generated/TSCHCommandArchives_pb2.py`

 * *Files identical despite different names*

### Comparing `numbers_parser-4.9.3/src/numbers_parser/generated/TSCHPreUFFArchives_pb2.py` & `numbers_parser-4.9.4/src/numbers_parser/generated/TSCHPreUFFArchives_pb2.py`

 * *Files identical despite different names*

### Comparing `numbers_parser-4.9.3/src/numbers_parser/generated/TSDArchives_pb2.py` & `numbers_parser-4.9.4/src/numbers_parser/generated/TSDArchives_pb2.py`

 * *Files identical despite different names*

### Comparing `numbers_parser-4.9.3/src/numbers_parser/generated/TSDArchives_sos_pb2.py` & `numbers_parser-4.9.4/src/numbers_parser/generated/TSDArchives_sos_pb2.py`

 * *Files identical despite different names*

### Comparing `numbers_parser-4.9.3/src/numbers_parser/generated/TSDCommandArchives_pb2.py` & `numbers_parser-4.9.4/src/numbers_parser/generated/TSDCommandArchives_pb2.py`

 * *Files identical despite different names*

### Comparing `numbers_parser-4.9.3/src/numbers_parser/generated/TSKArchives_pb2.py` & `numbers_parser-4.9.4/src/numbers_parser/generated/TSKArchives_pb2.py`

 * *Files identical despite different names*

### Comparing `numbers_parser-4.9.3/src/numbers_parser/generated/TSKArchives_sos_pb2.py` & `numbers_parser-4.9.4/src/numbers_parser/generated/TSKArchives_sos_pb2.py`

 * *Files identical despite different names*

### Comparing `numbers_parser-4.9.3/src/numbers_parser/generated/TSPArchiveMessages_pb2.py` & `numbers_parser-4.9.4/src/numbers_parser/generated/TSPArchiveMessages_pb2.py`

 * *Files identical despite different names*

### Comparing `numbers_parser-4.9.3/src/numbers_parser/generated/TSPDatabaseMessages_pb2.py` & `numbers_parser-4.9.4/src/numbers_parser/generated/TSPDatabaseMessages_pb2.py`

 * *Files identical despite different names*

### Comparing `numbers_parser-4.9.3/src/numbers_parser/generated/TSPMessages_pb2.py` & `numbers_parser-4.9.4/src/numbers_parser/generated/TSPMessages_pb2.py`

 * *Files identical despite different names*

### Comparing `numbers_parser-4.9.3/src/numbers_parser/generated/TSSArchives_pb2.py` & `numbers_parser-4.9.4/src/numbers_parser/generated/TSSArchives_pb2.py`

 * *Files identical despite different names*

### Comparing `numbers_parser-4.9.3/src/numbers_parser/generated/TSSArchives_sos_pb2.py` & `numbers_parser-4.9.4/src/numbers_parser/generated/TSSArchives_sos_pb2.py`

 * *Files identical despite different names*

### Comparing `numbers_parser-4.9.3/src/numbers_parser/generated/TSTArchives_pb2.py` & `numbers_parser-4.9.4/src/numbers_parser/generated/TSTArchives_pb2.py`

 * *Files identical despite different names*

### Comparing `numbers_parser-4.9.3/src/numbers_parser/generated/TSTArchives_sos_pb2.py` & `numbers_parser-4.9.4/src/numbers_parser/generated/TSTArchives_sos_pb2.py`

 * *Files identical despite different names*

### Comparing `numbers_parser-4.9.3/src/numbers_parser/generated/TSTCommandArchives_pb2.py` & `numbers_parser-4.9.4/src/numbers_parser/generated/TSTCommandArchives_pb2.py`

 * *Files identical despite different names*

### Comparing `numbers_parser-4.9.3/src/numbers_parser/generated/TSTStylePropertyArchiving_pb2.py` & `numbers_parser-4.9.4/src/numbers_parser/generated/TSTStylePropertyArchiving_pb2.py`

 * *Files identical despite different names*

### Comparing `numbers_parser-4.9.3/src/numbers_parser/generated/TSWPArchives_pb2.py` & `numbers_parser-4.9.4/src/numbers_parser/generated/TSWPArchives_pb2.py`

 * *Files identical despite different names*

### Comparing `numbers_parser-4.9.3/src/numbers_parser/generated/TSWPArchives_sos_pb2.py` & `numbers_parser-4.9.4/src/numbers_parser/generated/TSWPArchives_sos_pb2.py`

 * *Files identical despite different names*

### Comparing `numbers_parser-4.9.3/src/numbers_parser/generated/TSWPCommandArchives_pb2.py` & `numbers_parser-4.9.4/src/numbers_parser/generated/TSWPCommandArchives_pb2.py`

 * *Files identical despite different names*

### Comparing `numbers_parser-4.9.3/src/numbers_parser/generated/fontmap.py` & `numbers_parser-4.9.4/src/numbers_parser/generated/fontmap.py`

 * *Files identical despite different names*

### Comparing `numbers_parser-4.9.3/src/numbers_parser/generated/functionmap.py` & `numbers_parser-4.9.4/src/numbers_parser/generated/functionmap.py`

 * *Files identical despite different names*

### Comparing `numbers_parser-4.9.3/src/numbers_parser/iwafile.py` & `numbers_parser-4.9.4/src/numbers_parser/iwafile.py`

 * *Files identical despite different names*

### Comparing `numbers_parser-4.9.3/src/numbers_parser/mapping.py` & `numbers_parser-4.9.4/src/numbers_parser/mapping.py`

 * *Files identical despite different names*

### Comparing `numbers_parser-4.9.3/src/numbers_parser/model.py` & `numbers_parser-4.9.4/src/numbers_parser/model.py`

 * *Files 0% similar despite different names*

```diff
@@ -1735,17 +1735,15 @@
             value = pack("<d", float(cell.value))
         elif isinstance(cell, DurationCell):
             flags = 2
             length += 8
             cell_type = TSTArchives.durationCellType
             value = value = pack("<d", float(cell.value.total_seconds()))
         elif isinstance(cell, EmptyCell):
-            if cell._style is not None or (
-                cell._storage is not None and cell._storage.control_id is not None
-            ):
+            if cell._style is not None or cell._storage is not None:
                 flags = 0
                 cell_type = TSTArchives.emptyCellValueType
                 value = b""
             else:
                 return None
         elif isinstance(cell, MergedCell):
             return None
```

### Comparing `numbers_parser-4.9.3/src/numbers_parser/numbers_cache.py` & `numbers_parser-4.9.4/src/numbers_parser/numbers_cache.py`

 * *Files identical despite different names*

### Comparing `numbers_parser-4.9.3/src/numbers_parser/numbers_uuid.py` & `numbers_parser-4.9.4/src/numbers_parser/numbers_uuid.py`

 * *Files identical despite different names*

### Comparing `numbers_parser-4.9.3/PKG-INFO` & `numbers_parser-4.9.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: numbers-parser
-Version: 4.9.3
+Version: 4.9.4
 Summary: Read and write Apple Numbers spreadsheets
 Home-page: https://github.com/masaccio/numbers-parser
 License: MIT
 Author: Jon Connell
 Author-email: python@figsandfudge.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

