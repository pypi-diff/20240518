# Comparing `tmp/viking_log_keeper-1.0.0.tar.gz` & `tmp/viking_log_keeper-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "viking_log_keeper-1.0.0.tar", max compression
+gzip compressed data, was "viking_log_keeper-1.1.0.tar", max compression
```

## Comparing `viking_log_keeper-1.0.0.tar` & `viking_log_keeper-1.1.0.tar`

### file list

```diff
@@ -1,12 +1,14 @@
--rw-r--r--   0        0        0     3000 2024-03-29 20:20:31.918660 viking_log_keeper-1.0.0/README.md
--rw-r--r--   0        0        0     1309 2024-03-29 20:20:31.918660 viking_log_keeper-1.0.0/pyproject.toml
--rw-r--r--   0        0        0        0 2024-03-29 20:20:31.918660 viking_log_keeper-1.0.0/src/dashboard/__init__.py
--rw-r--r--   0        0        0    14527 2024-03-29 20:20:31.918660 viking_log_keeper-1.0.0/src/dashboard/main.py
--rw-r--r--   0        0        0     7385 2024-03-29 20:20:31.918660 viking_log_keeper-1.0.0/src/dashboard/plots.py
--rw-r--r--   0        0        0        0 2024-03-29 20:20:31.918660 viking_log_keeper-1.0.0/src/log_keeper/__init__.py
--rw-r--r--   0        0        0     5441 2024-03-29 20:20:31.918660 viking_log_keeper-1.0.0/src/log_keeper/get_config.py
--rw-r--r--   0        0        0     4992 2024-03-29 20:20:31.918660 viking_log_keeper-1.0.0/src/log_keeper/ingest.py
--rw-r--r--   0        0        0     2739 2024-03-29 20:20:31.918660 viking_log_keeper-1.0.0/src/log_keeper/main.py
--rw-r--r--   0        0        0     3805 2024-03-29 20:20:31.918660 viking_log_keeper-1.0.0/src/log_keeper/output.py
--rw-r--r--   0        0        0     3040 2024-03-29 20:20:31.918660 viking_log_keeper-1.0.0/src/log_keeper/utils.py
--rw-r--r--   0        0        0     4199 1970-01-01 00:00:00.000000 viking_log_keeper-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     3000 2024-05-18 08:24:21.619343 viking_log_keeper-1.1.0/README.md
+-rw-r--r--   0        0        0     1309 2024-05-18 08:24:21.619343 viking_log_keeper-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-18 08:24:21.619343 viking_log_keeper-1.1.0/src/dashboard/__init__.py
+-rw-r--r--   0        0        0     7922 2024-05-18 08:24:21.619343 viking_log_keeper-1.1.0/src/dashboard/auth.py
+-rw-r--r--   0        0        0     7124 2024-05-18 08:24:21.619343 viking_log_keeper-1.1.0/src/dashboard/main.py
+-rw-r--r--   0        0        0     7385 2024-05-18 08:24:21.619343 viking_log_keeper-1.1.0/src/dashboard/plots.py
+-rw-r--r--   0        0        0     1290 2024-05-18 08:24:21.619343 viking_log_keeper-1.1.0/src/dashboard/utils.py
+-rw-r--r--   0        0        0        0 2024-05-18 08:24:21.619343 viking_log_keeper-1.1.0/src/log_keeper/__init__.py
+-rw-r--r--   0        0        0     5441 2024-05-18 08:24:21.619343 viking_log_keeper-1.1.0/src/log_keeper/get_config.py
+-rw-r--r--   0        0        0     5000 2024-05-18 08:24:21.619343 viking_log_keeper-1.1.0/src/log_keeper/ingest.py
+-rw-r--r--   0        0        0     2739 2024-05-18 08:24:21.619343 viking_log_keeper-1.1.0/src/log_keeper/main.py
+-rw-r--r--   0        0        0     3805 2024-05-18 08:24:21.619343 viking_log_keeper-1.1.0/src/log_keeper/output.py
+-rw-r--r--   0        0        0     3040 2024-05-18 08:24:21.619343 viking_log_keeper-1.1.0/src/log_keeper/utils.py
+-rw-r--r--   0        0        0     4199 1970-01-01 00:00:00.000000 viking_log_keeper-1.1.0/PKG-INFO
```

### Comparing `viking_log_keeper-1.0.0/README.md` & `viking_log_keeper-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `viking_log_keeper-1.0.0/pyproject.toml` & `viking_log_keeper-1.1.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "viking-log-keeper"
-version = "1.0.0"
+version = "1.1.0"
 description = "661 VGS - Function to collate 2965D log sheets into a master log, database, and dashboard."
 authors = ["Michael Jennings <mjennings061@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
@@ -30,14 +30,14 @@
 
 [tool.poetry.urls]
 homepage = "https://github.com/mjennings061/viking-log-keeper"
 repository = "https://github.com/mjennings061/viking-log-keeper.git"
 
 [tool.poetry.scripts]
 update-logs = "log_keeper.main:main"
-update-config = "dashboard.main:update_credentials_wrapper"
+update-config = "dashboard.auth:update_credentials_wrapper"
 update-log-sheet-location = "log_keeper.get_config:update_log_sheets_dir_wrapper"
 viking-dashboard = "dashboard.main:display_dashboard"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `viking_log_keeper-1.0.0/src/dashboard/plots.py` & `viking_log_keeper-1.1.0/src/dashboard/plots.py`

 * *Files identical despite different names*

### Comparing `viking_log_keeper-1.0.0/src/log_keeper/get_config.py` & `viking_log_keeper-1.1.0/src/log_keeper/get_config.py`

 * *Files identical despite different names*

### Comparing `viking_log_keeper-1.0.0/src/log_keeper/ingest.py` & `viking_log_keeper-1.1.0/src/log_keeper/ingest.py`

 * *Files 0% similar despite different names*

```diff
@@ -146,15 +146,15 @@
                 # Append to the master dataframe.
                 log_sheet_df = pd.concat(
                     [log_sheet_df, this_sheet_df],
                     ignore_index=True
                 )
         except Exception:   # pylint: disable=broad-except
             if file_path.name != "2965D_YYMMDD_ZEXXX.xlsx":
-                logger.warning("Log sheet invalid: %s",
+                logger.warning("\n\nLog sheet invalid: %s\n\n",
                                file_path.name,
                                exc_info=True)
 
     sys.stdout.write("\nDone processing files.\n")
     sys.stdout.flush()
 
     # Sanitise the log sheets.
```

### Comparing `viking_log_keeper-1.0.0/src/log_keeper/main.py` & `viking_log_keeper-1.1.0/src/log_keeper/main.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 import logging
 from pathlib import Path
 
 # Get modules.
 from log_keeper.get_config import LogSheetConfig
 from log_keeper.ingest import collate_log_sheets
 from log_keeper.output import launches_to_excel, launches_to_db
-from dashboard.main import AuthConfig
+from dashboard.auth import AuthConfig
 
 # Set logging level.
 logging.basicConfig(level=logging.INFO)
 logger = logging.getLogger(__name__)
 
 
 def adjust_streamlit_logging():
```

### Comparing `viking_log_keeper-1.0.0/src/log_keeper/output.py` & `viking_log_keeper-1.1.0/src/log_keeper/output.py`

 * *Files identical despite different names*

### Comparing `viking_log_keeper-1.0.0/src/log_keeper/utils.py` & `viking_log_keeper-1.1.0/src/log_keeper/utils.py`

 * *Files identical despite different names*

### Comparing `viking_log_keeper-1.0.0/PKG-INFO` & `viking_log_keeper-1.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: viking-log-keeper
-Version: 1.0.0
+Version: 1.1.0
 Summary: 661 VGS - Function to collate 2965D log sheets into a master log, database, and dashboard.
 License: MIT
 Author: Michael Jennings
 Author-email: mjennings061@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

