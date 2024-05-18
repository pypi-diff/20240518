# Comparing `tmp/lukasdata-1.3.5.tar.gz` & `tmp/lukasdata-1.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lukasdata-1.3.5.tar", last modified: Sun May 12 15:20:48 2024, max compression
+gzip compressed data, was "lukasdata-1.3.6.tar", last modified: Sat May 18 14:39:32 2024, max compression
```

## Comparing `lukasdata-1.3.5.tar` & `lukasdata-1.3.6.tar`

### file list

```diff
@@ -1,42 +1,53 @@
-drwxrwxrwx   0        0        0        0 2024-05-12 15:20:48.699483 lukasdata-1.3.5/
--rw-rw-rw-   0        0        0      128 2024-05-12 15:20:48.696172 lukasdata-1.3.5/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-12 15:20:48.595635 lukasdata-1.3.5/cleaning/
--rw-rw-rw-   0        0        0        0 2024-05-11 10:17:58.000000 lukasdata-1.3.5/cleaning/__init__.py
--rw-rw-rw-   0        0        0      416 2024-05-03 13:24:44.000000 lukasdata-1.3.5/cleaning/check_for_all_zeroes.py
--rw-rw-rw-   0        0        0      387 2024-04-26 08:28:12.000000 lukasdata-1.3.5/cleaning/drop_column_with_na.py
--rw-rw-rw-   0        0        0      129 2024-04-26 08:32:10.000000 lukasdata-1.3.5/cleaning/mean_impute.py
--rw-rw-rw-   0        0        0      160 2024-04-26 08:29:44.000000 lukasdata-1.3.5/cleaning/na_counts.py
-drwxrwxrwx   0        0        0        0 2024-05-12 15:20:48.619620 lukasdata-1.3.5/datahandler/
--rw-rw-rw-   0        0        0        0 2024-05-11 10:17:58.000000 lukasdata-1.3.5/datahandler/__init__.py
--rw-rw-rw-   0        0        0      616 2024-04-22 22:29:19.000000 lukasdata-1.3.5/datahandler/change_directory.py
--rw-rw-rw-   0        0        0      178 2024-04-22 22:29:19.000000 lukasdata-1.3.5/datahandler/del_jpg.py
--rw-rw-rw-   0        0        0      334 2024-04-22 22:29:19.000000 lukasdata-1.3.5/datahandler/determine_file_type.py
--rw-rw-rw-   0        0        0      334 2024-04-22 22:29:19.000000 lukasdata-1.3.5/datahandler/dict_to_json.py
--rw-rw-rw-   0        0        0      255 2024-04-22 22:29:19.000000 lukasdata-1.3.5/datahandler/json_to_dict.py
--rw-rw-rw-   0        0        0      132 2024-04-30 10:39:24.000000 lukasdata-1.3.5/datahandler/order_dict.py
--rw-rw-rw-   0        0        0      160 2024-04-22 22:29:19.000000 lukasdata-1.3.5/datahandler/string_to_text.py
-drwxrwxrwx   0        0        0        0 2024-05-12 15:20:48.633611 lukasdata-1.3.5/exploration/
--rw-rw-rw-   0        0        0        0 2024-05-11 10:17:58.000000 lukasdata-1.3.5/exploration/__init__.py
--rw-rw-rw-   0        0        0      440 2024-05-04 13:56:10.000000 lukasdata-1.3.5/exploration/analyze_datasets.py
--rw-rw-rw-   0        0        0      351 2024-04-22 22:29:19.000000 lukasdata-1.3.5/exploration/count_nans.py
--rw-rw-rw-   0        0        0      385 2024-04-26 08:43:39.000000 lukasdata-1.3.5/exploration/get_list_intersection.py
-drwxrwxrwx   0        0        0        0 2024-05-12 15:20:48.694626 lukasdata-1.3.5/lukasdata.egg-info/
--rw-rw-rw-   0        0        0      128 2024-05-12 15:20:48.000000 lukasdata-1.3.5/lukasdata.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      972 2024-05-12 15:20:48.000000 lukasdata-1.3.5/lukasdata.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-12 15:20:48.000000 lukasdata-1.3.5/lukasdata.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       24 2024-05-12 15:20:48.000000 lukasdata-1.3.5/lukasdata.egg-info/requires.txt
--rw-rw-rw-   0        0        0       63 2024-05-12 15:20:48.000000 lukasdata-1.3.5/lukasdata.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-05-12 15:20:48.676811 lukasdata-1.3.5/machine_learning/
--rw-rw-rw-   0        0        0        0 2024-05-11 10:17:58.000000 lukasdata-1.3.5/machine_learning/__init__.py
--rw-rw-rw-   0        0        0      322 2024-05-08 17:36:02.000000 lukasdata-1.3.5/machine_learning/drop_columns_permutation_score.py
--rw-rw-rw-   0        0        0     2005 2024-05-11 09:53:36.000000 lukasdata-1.3.5/machine_learning/keras_input.py
--rw-rw-rw-   0        0        0     1166 2024-05-11 09:53:38.000000 lukasdata-1.3.5/machine_learning/ml_model.py
--rw-rw-rw-   0        0        0     2400 2024-05-09 08:33:54.000000 lukasdata-1.3.5/machine_learning/permutation_importance.py
-drwxrwxrwx   0        0        0        0 2024-05-12 15:20:48.691121 lukasdata-1.3.5/manipulation/
--rw-rw-rw-   0        0        0        0 2024-05-11 10:17:58.000000 lukasdata-1.3.5/manipulation/__init__.py
--rw-rw-rw-   0        0        0      260 2024-04-29 20:51:11.000000 lukasdata-1.3.5/manipulation/concat_dfs.py
--rw-rw-rw-   0        0        0      332 2024-04-22 22:29:19.000000 lukasdata-1.3.5/manipulation/create_mask.py
--rw-rw-rw-   0        0        0      447 2024-04-22 22:29:19.000000 lukasdata-1.3.5/manipulation/int_columns.py
--rw-rw-rw-   0        0        0      144 2024-04-22 22:29:19.000000 lukasdata-1.3.5/manipulation/list_to_string.py
--rw-rw-rw-   0        0        0       42 2024-05-12 15:20:48.700000 lukasdata-1.3.5/setup.cfg
--rw-rw-rw-   0        0        0      192 2024-05-12 15:20:41.000000 lukasdata-1.3.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-18 14:39:32.048454 lukasdata-1.3.6/
+-rw-rw-rw-   0        0        0      128 2024-05-18 14:39:32.046454 lukasdata-1.3.6/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-18 14:39:31.951066 lukasdata-1.3.6/cleaning/
+-rw-rw-rw-   0        0        0        0 2024-05-11 10:17:58.000000 lukasdata-1.3.6/cleaning/__init__.py
+-rw-rw-rw-   0        0        0      416 2024-05-03 13:24:44.000000 lukasdata-1.3.6/cleaning/check_for_all_zeroes.py
+-rw-rw-rw-   0        0        0      177 2024-05-18 14:37:26.000000 lukasdata-1.3.6/cleaning/clean_multiple_space.py
+-rw-rw-rw-   0        0        0      387 2024-04-26 08:28:12.000000 lukasdata-1.3.6/cleaning/drop_column_with_na.py
+-rw-rw-rw-   0        0        0      129 2024-04-26 08:32:10.000000 lukasdata-1.3.6/cleaning/mean_impute.py
+-rw-rw-rw-   0        0        0      160 2024-04-26 08:29:44.000000 lukasdata-1.3.6/cleaning/na_counts.py
+drwxrwxrwx   0        0        0        0 2024-05-18 14:39:31.979049 lukasdata-1.3.6/datahandling/
+-rw-rw-rw-   0        0        0        0 2024-05-11 10:17:58.000000 lukasdata-1.3.6/datahandling/__init__.py
+-rw-rw-rw-   0        0        0      616 2024-04-22 22:29:19.000000 lukasdata-1.3.6/datahandling/change_directory.py
+-rw-rw-rw-   0        0        0      184 2023-09-18 11:41:48.000000 lukasdata-1.3.6/datahandling/check_for_mismatches_in_list.py
+-rw-rw-rw-   0        0        0      704 2023-10-29 15:04:54.000000 lukasdata-1.3.6/datahandling/create_text_for_all_files_in_pdf_dir.py
+-rw-rw-rw-   0        0        0      503 2023-10-28 19:49:49.000000 lukasdata-1.3.6/datahandling/deconstruct_file_name.py
+-rw-rw-rw-   0        0        0      178 2024-04-22 22:29:19.000000 lukasdata-1.3.6/datahandling/del_jpg.py
+-rw-rw-rw-   0        0        0      334 2024-04-22 22:29:19.000000 lukasdata-1.3.6/datahandling/determine_file_type.py
+-rw-rw-rw-   0        0        0      334 2024-04-22 22:29:19.000000 lukasdata-1.3.6/datahandling/dict_to_json.py
+-rw-rw-rw-   0        0        0      257 2024-05-14 19:58:00.000000 lukasdata-1.3.6/datahandling/json_to_dict.py
+-rw-rw-rw-   0        0        0      132 2024-04-30 10:39:24.000000 lukasdata-1.3.6/datahandling/order_dict.py
+-rw-rw-rw-   0        0        0     1171 2023-10-29 14:47:29.000000 lukasdata-1.3.6/datahandling/pdf_to_txt.py
+-rw-rw-rw-   0        0        0      193 2024-05-17 17:01:50.000000 lukasdata-1.3.6/datahandling/read_txt.py
+-rw-rw-rw-   0        0        0      160 2024-04-22 22:29:19.000000 lukasdata-1.3.6/datahandling/string_to_text.py
+drwxrwxrwx   0        0        0        0 2024-05-18 14:39:31.983046 lukasdata-1.3.6/errorhandling/
+-rw-rw-rw-   0        0        0        0 2024-05-11 10:17:58.000000 lukasdata-1.3.6/errorhandling/__init__.py
+-rw-rw-rw-   0        0        0      587 2024-05-17 15:57:45.000000 lukasdata-1.3.6/errorhandling/custom_errors.py
+drwxrwxrwx   0        0        0        0 2024-05-18 14:39:31.995281 lukasdata-1.3.6/exploration/
+-rw-rw-rw-   0        0        0        0 2024-05-11 10:17:58.000000 lukasdata-1.3.6/exploration/__init__.py
+-rw-rw-rw-   0        0        0      440 2024-05-04 13:56:10.000000 lukasdata-1.3.6/exploration/analyze_datasets.py
+-rw-rw-rw-   0        0        0      351 2024-04-22 22:29:19.000000 lukasdata-1.3.6/exploration/count_nans.py
+-rw-rw-rw-   0        0        0     3566 2024-05-14 10:55:38.000000 lukasdata-1.3.6/exploration/desciptive_statistics.py
+-rw-rw-rw-   0        0        0      385 2024-04-26 08:43:39.000000 lukasdata-1.3.6/exploration/get_list_intersection.py
+-rw-rw-rw-   0        0        0        0 2024-05-14 10:08:25.000000 lukasdata-1.3.6/exploration/kernel_density_estimation.py
+drwxrwxrwx   0        0        0        0 2024-05-18 14:39:32.044456 lukasdata-1.3.6/lukasdata.egg-info/
+-rw-rw-rw-   0        0        0      128 2024-05-18 14:39:31.000000 lukasdata-1.3.6/lukasdata.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1336 2024-05-18 14:39:31.000000 lukasdata-1.3.6/lukasdata.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-18 14:39:31.000000 lukasdata-1.3.6/lukasdata.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       24 2024-05-18 14:39:31.000000 lukasdata-1.3.6/lukasdata.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       78 2024-05-18 14:39:31.000000 lukasdata-1.3.6/lukasdata.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-18 14:39:32.030464 lukasdata-1.3.6/machine_learning/
+-rw-rw-rw-   0        0        0        0 2024-05-11 10:17:58.000000 lukasdata-1.3.6/machine_learning/__init__.py
+-rw-rw-rw-   0        0        0      322 2024-05-08 17:36:02.000000 lukasdata-1.3.6/machine_learning/drop_columns_permutation_score.py
+-rw-rw-rw-   0        0        0     2005 2024-05-11 09:53:36.000000 lukasdata-1.3.6/machine_learning/keras_input.py
+-rw-rw-rw-   0        0        0     1746 2024-05-14 10:55:46.000000 lukasdata-1.3.6/machine_learning/ml_model.py
+-rw-rw-rw-   0        0        0     2400 2024-05-09 08:33:54.000000 lukasdata-1.3.6/machine_learning/permutation_importance.py
+drwxrwxrwx   0        0        0        0 2024-05-18 14:39:32.042457 lukasdata-1.3.6/manipulation/
+-rw-rw-rw-   0        0        0        0 2024-05-11 10:17:58.000000 lukasdata-1.3.6/manipulation/__init__.py
+-rw-rw-rw-   0        0        0      260 2024-04-29 20:51:11.000000 lukasdata-1.3.6/manipulation/concat_dfs.py
+-rw-rw-rw-   0        0        0      332 2024-04-22 22:29:19.000000 lukasdata-1.3.6/manipulation/create_mask.py
+-rw-rw-rw-   0        0        0      466 2024-05-13 11:10:36.000000 lukasdata-1.3.6/manipulation/int_columns.py
+-rw-rw-rw-   0        0        0      144 2024-04-22 22:29:19.000000 lukasdata-1.3.6/manipulation/list_to_string.py
+-rw-rw-rw-   0        0        0       42 2024-05-18 14:39:32.049454 lukasdata-1.3.6/setup.cfg
+-rw-rw-rw-   0        0        0      192 2024-05-18 14:39:24.000000 lukasdata-1.3.6/setup.py
```

### Comparing `lukasdata-1.3.5/datahandler/change_directory.py` & `lukasdata-1.3.6/datahandling/change_directory.py`

 * *Files identical despite different names*

### Comparing `lukasdata-1.3.5/machine_learning/keras_input.py` & `lukasdata-1.3.6/machine_learning/keras_input.py`

 * *Files identical despite different names*

### Comparing `lukasdata-1.3.5/machine_learning/permutation_importance.py` & `lukasdata-1.3.6/machine_learning/permutation_importance.py`

 * *Files identical despite different names*

