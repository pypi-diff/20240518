# Comparing `tmp/data_loader_lib-0.2.tar.gz` & `tmp/data_loader_lib-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "data_loader_lib-0.2.tar", last modified: Sat May 18 16:30:17 2024, max compression
+gzip compressed data, was "data_loader_lib-0.3.tar", last modified: Sat May 18 16:47:09 2024, max compression
```

## Comparing `data_loader_lib-0.2.tar` & `data_loader_lib-0.3.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-05-18 16:30:17.013125 data_loader_lib-0.2/
--rw-rw-rw-   0        0        0      611 2024-05-18 16:30:17.012125 data_loader_lib-0.2/PKG-INFO
--rw-rw-rw-   0        0        0       42 2024-05-18 16:30:17.014124 data_loader_lib-0.2/setup.cfg
--rw-rw-rw-   0        0        0      785 2024-05-18 16:28:28.000000 data_loader_lib-0.2/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-18 16:30:16.972458 data_loader_lib-0.2/src/
-drwxrwxrwx   0        0        0        0 2024-05-18 16:30:17.010125 data_loader_lib-0.2/src/data_loader_lib.egg-info/
--rw-rw-rw-   0        0        0      611 2024-05-18 16:30:16.000000 data_loader_lib-0.2/src/data_loader_lib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      315 2024-05-18 16:30:16.000000 data_loader_lib-0.2/src/data_loader_lib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-18 16:30:16.000000 data_loader_lib-0.2/src/data_loader_lib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       83 2024-05-18 16:30:16.000000 data_loader_lib-0.2/src/data_loader_lib.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2024-05-18 16:30:16.000000 data_loader_lib-0.2/src/data_loader_lib.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-05-18 16:30:17.007030 data_loader_lib-0.2/tests/
--rw-rw-rw-   0        0        0      920 2024-05-18 16:13:12.000000 data_loader_lib-0.2/tests/test_bigquery_loader.py
--rw-rw-rw-   0        0        0     1430 2024-05-18 16:12:56.000000 data_loader_lib-0.2/tests/test_local_file_loader.py
--rw-rw-rw-   0        0        0     1457 2024-05-18 16:13:04.000000 data_loader_lib-0.2/tests/test_sftp_file_loader.py
+drwxrwxrwx   0        0        0        0 2024-05-18 16:47:09.196038 data_loader_lib-0.3/
+-rw-rw-rw-   0        0        0     3401 2024-05-18 16:47:09.194022 data_loader_lib-0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     2697 2024-05-18 16:44:38.000000 data_loader_lib-0.3/README.md
+drwxrwxrwx   0        0        0        0 2024-05-18 16:47:09.161811 data_loader_lib-0.3/data_loader/
+drwxrwxrwx   0        0        0        0 2024-05-18 16:47:09.192346 data_loader_lib-0.3/data_loader/data_loader_lib.egg-info/
+-rw-rw-rw-   0        0        0     3401 2024-05-18 16:47:08.000000 data_loader_lib-0.3/data_loader/data_loader_lib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      365 2024-05-18 16:47:09.000000 data_loader_lib-0.3/data_loader/data_loader_lib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-18 16:47:08.000000 data_loader_lib-0.3/data_loader/data_loader_lib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       83 2024-05-18 16:47:08.000000 data_loader_lib-0.3/data_loader/data_loader_lib.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2024-05-18 16:47:08.000000 data_loader_lib-0.3/data_loader/data_loader_lib.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-18 16:47:09.197033 data_loader_lib-0.3/setup.cfg
+-rw-rw-rw-   0        0        0     1299 2024-05-18 16:45:44.000000 data_loader_lib-0.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-18 16:47:09.189669 data_loader_lib-0.3/tests/
+-rw-rw-rw-   0        0        0      920 2024-05-18 16:13:12.000000 data_loader_lib-0.3/tests/test_bigquery_loader.py
+-rw-rw-rw-   0        0        0     1430 2024-05-18 16:12:56.000000 data_loader_lib-0.3/tests/test_local_file_loader.py
+-rw-rw-rw-   0        0        0     1457 2024-05-18 16:13:04.000000 data_loader_lib-0.3/tests/test_sftp_file_loader.py
```

### Comparing `data_loader_lib-0.2/tests/test_bigquery_loader.py` & `data_loader_lib-0.3/tests/test_bigquery_loader.py`

 * *Files identical despite different names*

### Comparing `data_loader_lib-0.2/tests/test_local_file_loader.py` & `data_loader_lib-0.3/tests/test_local_file_loader.py`

 * *Files identical despite different names*

### Comparing `data_loader_lib-0.2/tests/test_sftp_file_loader.py` & `data_loader_lib-0.3/tests/test_sftp_file_loader.py`

 * *Files identical despite different names*

