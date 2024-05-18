# Comparing `tmp/qualystbx-0.2.0.tar.gz` & `tmp/qualystbx-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qualystbx-0.2.0.tar", last modified: Fri May 17 20:48:49 2024, max compression
+gzip compressed data, was "qualystbx-0.3.0.tar", last modified: Sat May 18 12:26:16 2024, max compression
```

## Comparing `qualystbx-0.2.0.tar` & `qualystbx-0.3.0.tar`

### file list

```diff
@@ -1,27 +1,28 @@
-drwxrwxr-x   0 dgregory  (1000) dgregory  (1000)        0 2024-05-17 20:48:49.138656 qualystbx-0.2.0/
--rw-rw-r--   0 dgregory  (1000) dgregory  (1000)    11359 2024-01-30 19:38:49.000000 qualystbx-0.2.0/LICENSE.txt
--rw-rw-r--   0 dgregory  (1000) dgregory  (1000)       20 2024-04-24 16:23:40.000000 qualystbx-0.2.0/MANIFEST.in
--rw-r--r--   0 dgregory  (1000) dgregory  (1000)     8578 2024-05-17 20:48:49.138656 qualystbx-0.2.0/PKG-INFO
--rw-rw-r--   0 dgregory  (1000) dgregory  (1000)     7718 2024-05-17 20:45:34.000000 qualystbx-0.2.0/README.md
--rw-rw-r--   0 dgregory  (1000) dgregory  (1000)    11359 2024-01-30 19:38:49.000000 qualystbx-0.2.0/license.txt
--rw-rw-r--   0 dgregory  (1000) dgregory  (1000)      103 2024-01-30 19:38:49.000000 qualystbx-0.2.0/pyproject.toml
-drwxrwxr-x   0 dgregory  (1000) dgregory  (1000)        0 2024-05-17 20:48:49.134656 qualystbx-0.2.0/qualys_tbx/
--rw-rw-r--   0 dgregory  (1000) dgregory  (1000)     7718 2024-05-17 20:45:34.000000 qualystbx-0.2.0/qualys_tbx/README.md
--rw-rw-r--   0 dgregory  (1000) dgregory  (1000)       21 2024-05-17 20:48:26.000000 qualystbx-0.2.0/qualys_tbx/__init__.py
-drwxrwxr-x   0 dgregory  (1000) dgregory  (1000)        0 2024-05-17 20:48:49.134656 qualystbx-0.2.0/qualys_tbx/qtbx_lib/
--rw-rw-r--   0 dgregory  (1000) dgregory  (1000)        0 2024-03-28 10:53:29.000000 qualystbx-0.2.0/qualys_tbx/qtbx_lib/__init__.py
--rw-rw-r--   0 dgregory  (1000) dgregory  (1000)     3599 2024-05-14 05:39:58.000000 qualystbx-0.2.0/qualys_tbx/qtbx_lib/qtbx_lib_argparser.py
--rw-rw-r--   0 dgregory  (1000) dgregory  (1000)    17131 2024-05-14 04:00:20.000000 qualystbx-0.2.0/qualys_tbx/qtbx_lib/qtbx_lib_authentication.py
--rw-rw-r--   0 dgregory  (1000) dgregory  (1000)     4461 2024-05-14 05:04:13.000000 qualystbx-0.2.0/qualys_tbx/qtbx_lib/qtbx_lib_config.py
--rw-rw-r--   0 dgregory  (1000) dgregory  (1000)     3131 2024-05-14 03:56:41.000000 qualystbx-0.2.0/qualys_tbx/qtbx_lib/qtbx_lib_functions.py
--rw-rw-r--   0 dgregory  (1000) dgregory  (1000)     6824 2024-05-10 03:04:01.000000 qualystbx-0.2.0/qualys_tbx/qtbx_lib/qtbx_lib_logger.py
-drwxrwxr-x   0 dgregory  (1000) dgregory  (1000)        0 2024-05-17 20:48:49.134656 qualystbx-0.2.0/qualys_tbx/qtbx_policy_merge/
--rw-rw-r--   0 dgregory  (1000) dgregory  (1000)        0 2024-04-02 10:51:14.000000 qualystbx-0.2.0/qualys_tbx/qtbx_policy_merge/__init__.py
--rw-rw-r--   0 dgregory  (1000) dgregory  (1000)    24191 2024-05-14 05:59:14.000000 qualystbx-0.2.0/qualys_tbx/qtbx_policy_merge/policy_merge_01.py
-drwxrwxr-x   0 dgregory  (1000) dgregory  (1000)        0 2024-05-17 20:48:49.134656 qualystbx-0.2.0/qualystbx.egg-info/
--rw-r--r--   0 dgregory  (1000) dgregory  (1000)     8578 2024-05-17 20:48:49.000000 qualystbx-0.2.0/qualystbx.egg-info/PKG-INFO
--rw-rw-r--   0 dgregory  (1000) dgregory  (1000)      575 2024-05-17 20:48:49.000000 qualystbx-0.2.0/qualystbx.egg-info/SOURCES.txt
--rw-rw-r--   0 dgregory  (1000) dgregory  (1000)        1 2024-05-17 20:48:49.000000 qualystbx-0.2.0/qualystbx.egg-info/dependency_links.txt
--rw-rw-r--   0 dgregory  (1000) dgregory  (1000)       11 2024-05-17 20:48:49.000000 qualystbx-0.2.0/qualystbx.egg-info/top_level.txt
--rw-rw-r--   0 dgregory  (1000) dgregory  (1000)       38 2024-05-17 20:48:49.138656 qualystbx-0.2.0/setup.cfg
--rw-rw-r--   0 dgregory  (1000) dgregory  (1000)     1718 2024-05-17 20:48:26.000000 qualystbx-0.2.0/setup.py
+drwxrwxr-x   0 dgregory  (1000) dgregory  (1000)        0 2024-05-18 12:26:16.402164 qualystbx-0.3.0/
+-rw-rw-r--   0 dgregory  (1000) dgregory  (1000)    11359 2024-01-30 19:38:49.000000 qualystbx-0.3.0/LICENSE.txt
+-rw-rw-r--   0 dgregory  (1000) dgregory  (1000)       20 2024-04-24 16:23:40.000000 qualystbx-0.3.0/MANIFEST.in
+-rw-r--r--   0 dgregory  (1000) dgregory  (1000)     8578 2024-05-18 12:26:16.402164 qualystbx-0.3.0/PKG-INFO
+-rw-rw-r--   0 dgregory  (1000) dgregory  (1000)     7718 2024-05-17 20:45:34.000000 qualystbx-0.3.0/README.md
+-rw-rw-r--   0 dgregory  (1000) dgregory  (1000)    11359 2024-01-30 19:38:49.000000 qualystbx-0.3.0/license.txt
+-rw-rw-r--   0 dgregory  (1000) dgregory  (1000)      103 2024-01-30 19:38:49.000000 qualystbx-0.3.0/pyproject.toml
+drwxrwxr-x   0 dgregory  (1000) dgregory  (1000)        0 2024-05-18 12:26:16.402164 qualystbx-0.3.0/qualys_tbx/
+-rw-rw-r--   0 dgregory  (1000) dgregory  (1000)     7718 2024-05-17 20:45:34.000000 qualystbx-0.3.0/qualys_tbx/README.md
+-rw-rw-r--   0 dgregory  (1000) dgregory  (1000)       21 2024-05-18 12:20:46.000000 qualystbx-0.3.0/qualys_tbx/__init__.py
+drwxrwxr-x   0 dgregory  (1000) dgregory  (1000)        0 2024-05-18 12:26:16.402164 qualystbx-0.3.0/qualys_tbx/qtbx_lib/
+-rw-rw-r--   0 dgregory  (1000) dgregory  (1000)        0 2024-03-28 10:53:29.000000 qualystbx-0.3.0/qualys_tbx/qtbx_lib/__init__.py
+-rw-rw-r--   0 dgregory  (1000) dgregory  (1000)     3599 2024-05-14 05:39:58.000000 qualystbx-0.3.0/qualys_tbx/qtbx_lib/qtbx_lib_argparser.py
+-rw-rw-r--   0 dgregory  (1000) dgregory  (1000)    17131 2024-05-14 04:00:20.000000 qualystbx-0.3.0/qualys_tbx/qtbx_lib/qtbx_lib_authentication.py
+-rw-rw-r--   0 dgregory  (1000) dgregory  (1000)     4462 2024-05-18 12:24:25.000000 qualystbx-0.3.0/qualys_tbx/qtbx_lib/qtbx_lib_config.py
+-rw-rw-r--   0 dgregory  (1000) dgregory  (1000)     3131 2024-05-14 03:56:41.000000 qualystbx-0.3.0/qualys_tbx/qtbx_lib/qtbx_lib_functions.py
+-rw-rw-r--   0 dgregory  (1000) dgregory  (1000)     6824 2024-05-10 03:04:01.000000 qualystbx-0.3.0/qualys_tbx/qtbx_lib/qtbx_lib_logger.py
+drwxrwxr-x   0 dgregory  (1000) dgregory  (1000)        0 2024-05-18 12:26:16.402164 qualystbx-0.3.0/qualys_tbx/qtbx_policy_merge/
+-rw-rw-r--   0 dgregory  (1000) dgregory  (1000)        0 2024-04-02 10:51:14.000000 qualystbx-0.3.0/qualys_tbx/qtbx_policy_merge/__init__.py
+-rw-rw-r--   0 dgregory  (1000) dgregory  (1000)    24191 2024-05-14 05:59:14.000000 qualystbx-0.3.0/qualys_tbx/qtbx_policy_merge/policy_merge_01.py
+-rw-rw-r--   0 dgregory  (1000) dgregory  (1000)     8352 2024-05-18 12:19:32.000000 qualystbx-0.3.0/qualys_tbx/qualystbx.py
+drwxrwxr-x   0 dgregory  (1000) dgregory  (1000)        0 2024-05-18 12:26:16.402164 qualystbx-0.3.0/qualystbx.egg-info/
+-rw-r--r--   0 dgregory  (1000) dgregory  (1000)     8578 2024-05-18 12:26:16.000000 qualystbx-0.3.0/qualystbx.egg-info/PKG-INFO
+-rw-rw-r--   0 dgregory  (1000) dgregory  (1000)      599 2024-05-18 12:26:16.000000 qualystbx-0.3.0/qualystbx.egg-info/SOURCES.txt
+-rw-rw-r--   0 dgregory  (1000) dgregory  (1000)        1 2024-05-18 12:26:16.000000 qualystbx-0.3.0/qualystbx.egg-info/dependency_links.txt
+-rw-rw-r--   0 dgregory  (1000) dgregory  (1000)       11 2024-05-18 12:26:16.000000 qualystbx-0.3.0/qualystbx.egg-info/top_level.txt
+-rw-rw-r--   0 dgregory  (1000) dgregory  (1000)       38 2024-05-18 12:26:16.402164 qualystbx-0.3.0/setup.cfg
+-rw-rw-r--   0 dgregory  (1000) dgregory  (1000)     1718 2024-05-18 12:20:46.000000 qualystbx-0.3.0/setup.py
```

### Comparing `qualystbx-0.2.0/LICENSE.txt` & `qualystbx-0.3.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `qualystbx-0.2.0/PKG-INFO` & `qualystbx-0.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qualystbx
-Version: 0.2.0
+Version: 0.3.0
 Summary: Qualys Tool Box - Tools for running various functions in Qualys.
 Home-page: https://pypi.org/project/qualystbx/
 Author: David Gregory
 Author-email: dgregory@qualys.com, dave@davidgregory.com
 License: Apache
 Project-URL: Documentation, https://dg-cafe.github.io/qualystbx/
 Keywords: qualys,qualystoolbox,qualys.com,david gregory,qualystbx,qualysapi
```

### Comparing `qualystbx-0.2.0/README.md` & `qualystbx-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `qualystbx-0.2.0/license.txt` & `qualystbx-0.3.0/license.txt`

 * *Files identical despite different names*

### Comparing `qualystbx-0.2.0/qualys_tbx/README.md` & `qualystbx-0.3.0/qualys_tbx/README.md`

 * *Files identical despite different names*

### Comparing `qualystbx-0.2.0/qualys_tbx/qtbx_lib/qtbx_lib_argparser.py` & `qualystbx-0.3.0/qualys_tbx/qtbx_lib/qtbx_lib_argparser.py`

 * *Files identical despite different names*

### Comparing `qualystbx-0.2.0/qualys_tbx/qtbx_lib/qtbx_lib_authentication.py` & `qualystbx-0.3.0/qualys_tbx/qtbx_lib/qtbx_lib_authentication.py`

 * *Files identical despite different names*

### Comparing `qualystbx-0.2.0/qualys_tbx/qtbx_lib/qtbx_lib_config.py` & `qualystbx-0.3.0/qualys_tbx/qtbx_lib/qtbx_lib_config.py`

 * *Files 0% similar despite different names*

```diff
@@ -84,15 +84,15 @@
     if qtbx_tool_selected_to_run is None:
         qtbx_tool_selected_to_run = "default"
 
     if not os.access(qtbx_storage_dir, os.W_OK):
         print(f"Error: The directory '{qtbx_storage_dir}' is not writable. Please update --storage_dir to a directory that is writable.\n")
         sys.exit(1)
 
-    qtbx_home_dir = Path(qtbx_storage_dir,"qualystbx", "tbx_home", qtbx_tool_selected_to_run)
+    qtbx_home_dir = Path(qtbx_storage_dir,"qualystbx", "qtbx_home", qtbx_tool_selected_to_run)
     qtbx_data_dir = Path(qtbx_home_dir, "data")
     qtbx_log_dir = Path(qtbx_home_dir, "log")
     qtbx_bin_dir = Path(qtbx_home_dir, "bin")
     qtbx_config_dir = Path(qtbx_home_dir, "config")
     qtbx_cred_dir = Path(qtbx_home_dir, "cred")
 
 def create_qtbx_directories():
```

### Comparing `qualystbx-0.2.0/qualys_tbx/qtbx_lib/qtbx_lib_functions.py` & `qualystbx-0.3.0/qualys_tbx/qtbx_lib/qtbx_lib_functions.py`

 * *Files identical despite different names*

### Comparing `qualystbx-0.2.0/qualys_tbx/qtbx_lib/qtbx_lib_logger.py` & `qualystbx-0.3.0/qualys_tbx/qtbx_lib/qtbx_lib_logger.py`

 * *Files identical despite different names*

### Comparing `qualystbx-0.2.0/qualys_tbx/qtbx_policy_merge/policy_merge_01.py` & `qualystbx-0.3.0/qualys_tbx/qtbx_policy_merge/policy_merge_01.py`

 * *Files identical despite different names*

### Comparing `qualystbx-0.2.0/qualystbx.egg-info/PKG-INFO` & `qualystbx-0.3.0/qualystbx.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qualystbx
-Version: 0.2.0
+Version: 0.3.0
 Summary: Qualys Tool Box - Tools for running various functions in Qualys.
 Home-page: https://pypi.org/project/qualystbx/
 Author: David Gregory
 Author-email: dgregory@qualys.com, dave@davidgregory.com
 License: Apache
 Project-URL: Documentation, https://dg-cafe.github.io/qualystbx/
 Keywords: qualys,qualystoolbox,qualys.com,david gregory,qualystbx,qualysapi
```

### Comparing `qualystbx-0.2.0/qualystbx.egg-info/SOURCES.txt` & `qualystbx-0.3.0/qualystbx.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 MANIFEST.in
 README.md
 license.txt
 pyproject.toml
 setup.py
 qualys_tbx/README.md
 qualys_tbx/__init__.py
+qualys_tbx/qualystbx.py
 qualys_tbx/qtbx_lib/__init__.py
 qualys_tbx/qtbx_lib/qtbx_lib_argparser.py
 qualys_tbx/qtbx_lib/qtbx_lib_authentication.py
 qualys_tbx/qtbx_lib/qtbx_lib_config.py
 qualys_tbx/qtbx_lib/qtbx_lib_functions.py
 qualys_tbx/qtbx_lib/qtbx_lib_logger.py
 qualys_tbx/qtbx_policy_merge/__init__.py
```

### Comparing `qualystbx-0.2.0/setup.py` & `qualystbx-0.3.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 # Get the long description from the README file
 long_description = (here_qualys_tbx / 'README.md').read_text(encoding='utf-8')
 
 
 setup(
     name='qualystbx',
-    version='0.2.0',
+    version='0.3.0',
     packages=find_packages(include=[
         'qualys_tbx',
         'qualys_tbx.qtbx_lib',
         'qualys_tbx.qtbx_policy_merge',
         'qualys_tbx.*',
         'qualys_tbx.qtbx_lib.*',
         'qualys_tbx.qtbx_policy_merge.*',
```

