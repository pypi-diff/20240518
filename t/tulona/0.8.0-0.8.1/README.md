# Comparing `tmp/tulona-0.8.0.tar.gz` & `tmp/tulona-0.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tulona-0.8.0.tar", last modified: Thu May 16 00:39:35 2024, max compression
+gzip compressed data, was "tulona-0.8.1.tar", last modified: Sat May 18 01:54:41 2024, max compression
```

## Comparing `tulona-0.8.0.tar` & `tulona-0.8.1.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 00:39:35.033097 tulona-0.8.0/
--rw-r--r--   0 runner    (1001) docker     (127)    11356 2024-05-16 00:39:27.000000 tulona-0.8.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    14812 2024-05-16 00:39:35.033097 tulona-0.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    13105 2024-05-16 00:39:27.000000 tulona-0.8.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 00:39:35.025097 tulona-0.8.0/core/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 00:39:35.029097 tulona-0.8.0/core/tulona/
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-16 00:39:27.000000 tulona-0.8.0/core/tulona/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 00:39:35.029097 tulona-0.8.0/core/tulona/adapter/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 00:39:35.029097 tulona-0.8.0/core/tulona/adapter/base/
--rw-r--r--   0 runner    (1001) docker     (127)      123 2024-05-16 00:39:27.000000 tulona-0.8.0/core/tulona/adapter/base/connection.py
--rw-r--r--   0 runner    (1001) docker     (127)     1228 2024-05-16 00:39:27.000000 tulona-0.8.0/core/tulona/adapter/connection.py
--rw-r--r--   0 runner    (1001) docker     (127)      960 2024-05-16 00:39:27.000000 tulona-0.8.0/core/tulona/adapter/mssql.py
--rw-r--r--   0 runner    (1001) docker     (127)     1309 2024-05-16 00:39:27.000000 tulona-0.8.0/core/tulona/adapter/mysql.py
--rw-r--r--   0 runner    (1001) docker     (127)     1324 2024-05-16 00:39:27.000000 tulona-0.8.0/core/tulona/adapter/postgres.py
--rw-r--r--   0 runner    (1001) docker     (127)     2166 2024-05-16 00:39:27.000000 tulona-0.8.0/core/tulona/adapter/snowflake.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 00:39:35.029097 tulona-0.8.0/core/tulona/cli/
--rw-r--r--   0 runner    (1001) docker     (127)    18071 2024-05-16 00:39:27.000000 tulona-0.8.0/core/tulona/cli/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      930 2024-05-16 00:39:27.000000 tulona-0.8.0/core/tulona/cli/params.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 00:39:35.029097 tulona-0.8.0/core/tulona/config/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 00:39:27.000000 tulona-0.8.0/core/tulona/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1984 2024-05-16 00:39:27.000000 tulona-0.8.0/core/tulona/config/profile.py
--rw-r--r--   0 runner    (1001) docker     (127)     1931 2024-05-16 00:39:27.000000 tulona-0.8.0/core/tulona/config/project.py
--rw-r--r--   0 runner    (1001) docker     (127)     2675 2024-05-16 00:39:27.000000 tulona-0.8.0/core/tulona/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 00:39:35.033097 tulona-0.8.0/core/tulona/task/
--rw-r--r--   0 runner    (1001) docker     (127)      553 2024-05-16 00:39:27.000000 tulona-0.8.0/core/tulona/task/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    25357 2024-05-16 00:39:27.000000 tulona-0.8.0/core/tulona/task/compare.py
--rw-r--r--   0 runner    (1001) docker     (127)     4379 2024-05-16 00:39:27.000000 tulona-0.8.0/core/tulona/task/helper.py
--rw-r--r--   0 runner    (1001) docker     (127)     1462 2024-05-16 00:39:27.000000 tulona-0.8.0/core/tulona/task/ping.py
--rw-r--r--   0 runner    (1001) docker     (127)     4729 2024-05-16 00:39:27.000000 tulona-0.8.0/core/tulona/task/profile.py
--rw-r--r--   0 runner    (1001) docker     (127)    16803 2024-05-16 00:39:27.000000 tulona-0.8.0/core/tulona/task/scan.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 00:39:35.033097 tulona-0.8.0/core/tulona/util/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 00:39:27.000000 tulona-0.8.0/core/tulona/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      609 2024-05-16 00:39:27.000000 tulona-0.8.0/core/tulona/util/database.py
--rw-r--r--   0 runner    (1001) docker     (127)     1303 2024-05-16 00:39:27.000000 tulona-0.8.0/core/tulona/util/dataframe.py
--rw-r--r--   0 runner    (1001) docker     (127)     3074 2024-05-16 00:39:27.000000 tulona-0.8.0/core/tulona/util/excel.py
--rw-r--r--   0 runner    (1001) docker     (127)     1550 2024-05-16 00:39:27.000000 tulona-0.8.0/core/tulona/util/filesystem.py
--rw-r--r--   0 runner    (1001) docker     (127)      601 2024-05-16 00:39:27.000000 tulona-0.8.0/core/tulona/util/profiles.py
--rw-r--r--   0 runner    (1001) docker     (127)     5958 2024-05-16 00:39:27.000000 tulona-0.8.0/core/tulona/util/sql.py
--rw-r--r--   0 runner    (1001) docker     (127)      217 2024-05-16 00:39:27.000000 tulona-0.8.0/core/tulona/util/yaml_parser.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 00:39:35.033097 tulona-0.8.0/core/tulona.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    14812 2024-05-16 00:39:35.000000 tulona-0.8.0/core/tulona.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1020 2024-05-16 00:39:35.000000 tulona-0.8.0/core/tulona.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 00:39:35.000000 tulona-0.8.0/core/tulona.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-16 00:39:35.000000 tulona-0.8.0/core/tulona.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      261 2024-05-16 00:39:35.000000 tulona-0.8.0/core/tulona.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-16 00:39:35.000000 tulona-0.8.0/core/tulona.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3591 2024-05-16 00:39:27.000000 tulona-0.8.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-16 00:39:35.033097 tulona-0.8.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 01:54:40.994581 tulona-0.8.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    11356 2024-05-18 01:54:33.000000 tulona-0.8.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    14812 2024-05-18 01:54:40.994581 tulona-0.8.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    13105 2024-05-18 01:54:33.000000 tulona-0.8.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 01:54:40.986581 tulona-0.8.1/core/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 01:54:40.986581 tulona-0.8.1/core/tulona/
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-18 01:54:33.000000 tulona-0.8.1/core/tulona/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 01:54:40.990581 tulona-0.8.1/core/tulona/adapter/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 01:54:40.990581 tulona-0.8.1/core/tulona/adapter/base/
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-05-18 01:54:33.000000 tulona-0.8.1/core/tulona/adapter/base/connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1228 2024-05-18 01:54:33.000000 tulona-0.8.1/core/tulona/adapter/connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)      960 2024-05-18 01:54:33.000000 tulona-0.8.1/core/tulona/adapter/mssql.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1309 2024-05-18 01:54:33.000000 tulona-0.8.1/core/tulona/adapter/mysql.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1324 2024-05-18 01:54:33.000000 tulona-0.8.1/core/tulona/adapter/postgres.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2166 2024-05-18 01:54:33.000000 tulona-0.8.1/core/tulona/adapter/snowflake.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 01:54:40.990581 tulona-0.8.1/core/tulona/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)    18678 2024-05-18 01:54:33.000000 tulona-0.8.1/core/tulona/cli/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      930 2024-05-18 01:54:33.000000 tulona-0.8.1/core/tulona/cli/params.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 01:54:40.990581 tulona-0.8.1/core/tulona/config/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-18 01:54:33.000000 tulona-0.8.1/core/tulona/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2009 2024-05-18 01:54:33.000000 tulona-0.8.1/core/tulona/config/profile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1936 2024-05-18 01:54:33.000000 tulona-0.8.1/core/tulona/config/project.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2896 2024-05-18 01:54:33.000000 tulona-0.8.1/core/tulona/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 01:54:40.990581 tulona-0.8.1/core/tulona/task/
+-rw-r--r--   0 runner    (1001) docker     (127)      553 2024-05-18 01:54:33.000000 tulona-0.8.1/core/tulona/task/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25257 2024-05-18 01:54:33.000000 tulona-0.8.1/core/tulona/task/compare.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4379 2024-05-18 01:54:33.000000 tulona-0.8.1/core/tulona/task/helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1462 2024-05-18 01:54:33.000000 tulona-0.8.1/core/tulona/task/ping.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4729 2024-05-18 01:54:33.000000 tulona-0.8.1/core/tulona/task/profile.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16803 2024-05-18 01:54:33.000000 tulona-0.8.1/core/tulona/task/scan.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 01:54:40.994581 tulona-0.8.1/core/tulona/util/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-18 01:54:33.000000 tulona-0.8.1/core/tulona/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      609 2024-05-18 01:54:33.000000 tulona-0.8.1/core/tulona/util/database.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1303 2024-05-18 01:54:33.000000 tulona-0.8.1/core/tulona/util/dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3074 2024-05-18 01:54:33.000000 tulona-0.8.1/core/tulona/util/excel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1550 2024-05-18 01:54:33.000000 tulona-0.8.1/core/tulona/util/filesystem.py
+-rw-r--r--   0 runner    (1001) docker     (127)      601 2024-05-18 01:54:33.000000 tulona-0.8.1/core/tulona/util/profiles.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5997 2024-05-18 01:54:33.000000 tulona-0.8.1/core/tulona/util/sql.py
+-rw-r--r--   0 runner    (1001) docker     (127)      217 2024-05-18 01:54:33.000000 tulona-0.8.1/core/tulona/util/yaml_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 01:54:40.994581 tulona-0.8.1/core/tulona.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    14812 2024-05-18 01:54:40.000000 tulona-0.8.1/core/tulona.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1020 2024-05-18 01:54:40.000000 tulona-0.8.1/core/tulona.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-18 01:54:40.000000 tulona-0.8.1/core/tulona.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-18 01:54:40.000000 tulona-0.8.1/core/tulona.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      261 2024-05-18 01:54:40.000000 tulona-0.8.1/core/tulona.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-18 01:54:40.000000 tulona-0.8.1/core/tulona.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3591 2024-05-18 01:54:33.000000 tulona-0.8.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-18 01:54:40.994581 tulona-0.8.1/setup.cfg
```

### Comparing `tulona-0.8.0/LICENSE` & `tulona-0.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `tulona-0.8.0/PKG-INFO` & `tulona-0.8.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tulona
-Version: 0.8.0
+Version: 0.8.1
 Summary: A tool to compare data from different sources.
 Author: Mrinal Kanti Sardar
 Project-URL: Homepage, https://github.com/mrinalsardar/tulona
 Project-URL: Documentation, https://github.com/mrinalsardar/tulona
 Project-URL: Repository, https://github.com/mrinalsardar/tulona.git
 Project-URL: Issues, https://github.com/mrinalsardar/tulona/issues
 Keywords: tulona,comparison,data comparison,database scan,database profile
```

### Comparing `tulona-0.8.0/README.rst` & `tulona-0.8.1/README.rst`

 * *Files identical despite different names*

### Comparing `tulona-0.8.0/core/tulona/adapter/connection.py` & `tulona-0.8.1/core/tulona/adapter/connection.py`

 * *Files identical despite different names*

### Comparing `tulona-0.8.0/core/tulona/adapter/mssql.py` & `tulona-0.8.1/core/tulona/adapter/mssql.py`

 * *Files identical despite different names*

### Comparing `tulona-0.8.0/core/tulona/adapter/mysql.py` & `tulona-0.8.1/core/tulona/adapter/mysql.py`

 * *Files identical despite different names*

### Comparing `tulona-0.8.0/core/tulona/adapter/postgres.py` & `tulona-0.8.1/core/tulona/adapter/postgres.py`

 * *Files identical despite different names*

### Comparing `tulona-0.8.0/core/tulona/adapter/snowflake.py` & `tulona-0.8.1/core/tulona/adapter/snowflake.py`

 * *Files identical despite different names*

### Comparing `tulona-0.8.0/core/tulona/cli/base.py` & `tulona-0.8.1/core/tulona/cli/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -28,28 +28,29 @@
 log_dir = Path(Path().absolute(), "log")
 log_dir.mkdir(parents=True, exist_ok=True)
 log_file_fqn = Path(log_dir, f"tulona_{datetime.now().strftime('%Y%m%d%H%M%S')}.log")
 file_handler = logging.FileHandler(log_file_fqn)
 file_handler.setFormatter(log_formatter)
 file_handler.setLevel(logging.DEBUG)
 log.addHandler(file_handler)
-# TODO: Logs of this file are not getting out (-_-)
+
+nlog = logging.getLogger(__name__)
 
 
 # command: tulona
 @click.group(
     context_settings={"help_option_names": ["-h", "--help"]},
     no_args_is_help=True,
     epilog="Execute: tulona <command> -h/--help for more help with specific commands",
 )
 @click.pass_context
 def cli(ctx):
     """Tulona compares data sources to find out differences"""
     logging.getLogger("tulona").setLevel(logging.DEBUG)
-    logging.getLogger(__name__).info(f"Writing debug log into: {log_file_fqn}")
+    nlog.info(f"Writing debug log into: {log_file_fqn}")
 
     prof = Profile()
     proj = Project()
     ctx.obj = ctx.obj or {}
     ctx.obj["project"] = proj.load_project_config()
     ctx.obj["profile"] = prof.load_profile_config()[ctx.obj["project"]["name"]]
     ctx.obj["project"]["run_result_dir"] = get_run_result_dir(
@@ -76,18 +77,18 @@
         ping_tasks = [t for t in ctx.obj["project"]["task_config"] if t["task"] == "ping"]
 
     if len(ping_tasks) == 0:
         raise RuntimeError(
             "Nothing to execute. Either define tasks in task_config section of the"
             " project config file or pass --datasources argument with values."
         )
-    log.debug(f"Number of ping tasks to execute: {len(ping_tasks)}")
+    nlog.debug(f"Number of ping tasks to execute: {len(ping_tasks)}")
 
     for tconf in ping_tasks:
-        log.debug(f"Executing ping with task profile: {tconf}")
+        nlog.info(f"Executing ping with task profile: {tconf}")
         PingTask(
             profile=ctx.obj["profile"],
             project=ctx.obj["project"],
             datasources=tconf["datasources"],
         ).execute()
 
 
@@ -121,22 +122,23 @@
         scan_tasks = [t for t in ctx.obj["project"]["task_config"] if t["task"] == "scan"]
 
     if len(scan_tasks) == 0:
         raise RuntimeError(
             "Nothing to execute. Either define tasks in task_config section of the"
             " project config file or pass --datasources argument with values."
         )
-    log.debug(f"Number of scan tasks to execute: {len(scan_tasks)}")
+    nlog.debug(f"Number of scan tasks to execute: {len(scan_tasks)}")
 
     for tconf in scan_tasks:
-        log.debug(f"Executing scan with task profile: {tconf}")
+        nlog.info(f"Executing scan with task profile: {tconf}")
         final_outdir = get_task_outdir(
             run_dir=ctx.obj["project"]["run_result_dir"],
             task_conf=tconf,
         )
+        nlog.debug(f"Output will be stored in: {final_outdir}")
 
         ScanTask(
             profile=ctx.obj["profile"],
             project=ctx.obj["project"],
             datasources=tconf["datasources"],
             final_outdir=final_outdir,
             compare=tconf["compare"] if "compare" in tconf else None,
@@ -171,23 +173,24 @@
         ]
 
     if len(profile_tasks) == 0:
         raise RuntimeError(
             "Nothing to execute. Either define tasks in task_config section of the"
             " project config file or pass --datasources argument with values."
         )
-    log.debug(f"Number of profile tasks to execute: {len(profile_tasks)}")
+    nlog.debug(f"Number of profile tasks to execute: {len(profile_tasks)}")
 
     for tconf in profile_tasks:
-        log.debug(f"Executing profile with task profile: {tconf}")
+        nlog.info(f"Executing profile with task profile: {tconf}")
         final_outdir = get_task_outdir(
             run_dir=ctx.obj["project"]["run_result_dir"],
             task_conf=tconf,
         )
         outfile_fqn = Path(final_outdir, "profile_metadata.xlsx")
+        nlog.debug(f"Output will be stored in: {final_outdir}")
 
         ProfileTask(
             profile=ctx.obj["profile"],
             project=ctx.obj["project"],
             datasources=tconf["datasources"],
             outfile_fqn=outfile_fqn,
             compare=tconf["compare"] if "compare" in tconf else None,
@@ -220,23 +223,24 @@
         ]
 
     if len(compare_row_tasks) == 0:
         raise RuntimeError(
             "Nothing to execute. Either define tasks in task_config section of the"
             " project config file or pass --datasources argument with values."
         )
-    log.debug(f"Number compare-row tasks to execute: {len(compare_row_tasks)}")
+    nlog.debug(f"Number compare-row tasks to execute: {len(compare_row_tasks)}")
 
     for tconf in compare_row_tasks:
-        log.debug(f"Executing compare-row with task profile: {tconf}")
+        nlog.info(f"Executing compare-row with task profile: {tconf}")
         final_outdir = get_task_outdir(
             run_dir=ctx.obj["project"]["run_result_dir"],
             task_conf=tconf,
         )
         outfile_fqn = Path(final_outdir, "row_comparison.xlsx")
+        nlog.debug(f"Output will be stored in: {final_outdir}")
 
         CompareRowTask(
             profile=ctx.obj["profile"],
             project=ctx.obj["project"],
             datasources=tconf["datasources"],
             outfile_fqn=outfile_fqn,
             sample_count=tconf["sample_count"] if "sample_count" in tconf else None,
@@ -277,23 +281,24 @@
         ]
 
     if len(compare_column_tasks) == 0:
         raise RuntimeError(
             "Nothing to execute. Either define tasks in task_config section of the"
             " project config file or pass --datasources argument with values."
         )
-    log.debug(f"Number compare-column tasks to execute: {len(compare_column_tasks)}")
+    nlog.debug(f"Number compare-column tasks to execute: {len(compare_column_tasks)}")
 
     for tconf in compare_column_tasks:
-        log.debug(f"Executing compare-column with task profile: {tconf}")
+        nlog.info(f"Executing compare-column with task profile: {tconf}")
         final_outdir = get_task_outdir(
             run_dir=ctx.obj["project"]["run_result_dir"],
             task_conf=tconf,
         )
         outfile_fqn = Path(final_outdir, "column_comparison.xlsx")
+        nlog.debug(f"Output will be stored in: {final_outdir}")
 
         CompareColumnTask(
             profile=ctx.obj["profile"],
             project=ctx.obj["project"],
             datasources=tconf["datasources"],
             outfile_fqn=outfile_fqn,
             composite=tconf["composite"] if "composite" in tconf else None,
@@ -334,23 +339,24 @@
         ]
 
     if len(compare_tasks) == 0:
         raise RuntimeError(
             "Nothing to execute. Either define tasks in task_config section of the"
             " project config file or pass --datasources argument with values."
         )
-    log.debug(f"Number compare tasks to execute: {len(compare_tasks)}")
+    nlog.debug(f"Number compare tasks to execute: {len(compare_tasks)}")
 
     for tconf in compare_tasks:
-        log.debug(f"Executing compare with task profile: {tconf}")
+        nlog.info(f"Executing compare with task profile: {tconf}")
         final_outdir = get_task_outdir(
             run_dir=ctx.obj["project"]["run_result_dir"],
             task_conf=tconf,
         )
         outfile_fqn = Path(final_outdir, "comparison.xlsx")
+        nlog.debug(f"Output will be stored in: {final_outdir}")
 
         CompareTask(
             profile=ctx.obj["profile"],
             project=ctx.obj["project"],
             datasources=tconf["datasources"],
             outfile_fqn=outfile_fqn,
             sample_count=tconf["sample_count"] if "sample_count" in tconf else None,
@@ -386,49 +392,51 @@
     compare_tasks = [
         t for t in ctx.obj["project"]["task_config"] if t["task"] == "compare"
     ]
     scan_tasks = [t for t in ctx.obj["project"]["task_config"] if t["task"] == "scan"]
 
     # PingTask
     for tconf in ping_tasks:
-        log.debug(f"Executing ping with task profile: {tconf}")
+        nlog.info(f"Executing ping with task profile: {tconf}")
         PingTask(
             profile=ctx.obj["profile"],
             project=ctx.obj["project"],
             datasources=tconf["datasources"],
         ).execute()
 
     # ProfileTask
     for tconf in profile_tasks:
-        log.debug(f"Executing profile with task profile: {tconf}")
+        nlog.info(f"Executing profile with task profile: {tconf}")
         final_outdir = get_task_outdir(
             run_dir=ctx.obj["project"]["run_result_dir"],
             task_conf=tconf,
         )
         outfile_fqn = Path(final_outdir, "profile_metadata.xlsx")
+        nlog.debug(f"Output will be stored in: {final_outdir}")
 
         try:
             ProfileTask(
                 profile=ctx.obj["profile"],
                 project=ctx.obj["project"],
                 datasources=tconf["datasources"],
                 outfile_fqn=outfile_fqn,
                 compare=tconf["compare"] if "compare" in tconf else None,
             ).execute()
         except Exception:
             log.error(f"Profiling failed with error: {traceback.format_exc()}")
 
     # CompareRowTask
     for tconf in compare_row_tasks:
-        log.debug(f"Executing compare-row with task profile: {tconf}")
+        nlog.info(f"Executing compare-row with task profile: {tconf}")
         final_outdir = get_task_outdir(
             run_dir=ctx.obj["project"]["run_result_dir"],
             task_conf=tconf,
         )
         outfile_fqn = Path(final_outdir, "row_comparison.xlsx")
+        nlog.debug(f"Output will be stored in: {final_outdir}")
 
         try:
             CompareRowTask(
                 profile=ctx.obj["profile"],
                 project=ctx.obj["project"],
                 datasources=tconf["datasources"],
                 outfile_fqn=outfile_fqn,
@@ -438,20 +446,21 @@
                 ),
             ).execute()
         except Exception:
             log.error(f"Row comparison failed with error: {traceback.format_exc()}")
 
     # CompareColumnTask
     for tconf in compare_column_tasks:
-        log.debug(f"Executing compare-column with task profile: {tconf}")
+        nlog.info(f"Executing compare-column with task profile: {tconf}")
         final_outdir = get_task_outdir(
             run_dir=ctx.obj["project"]["run_result_dir"],
             task_conf=tconf,
         )
         outfile_fqn = Path(final_outdir, "column_comparison.xlsx")
+        nlog.debug(f"Output will be stored in: {final_outdir}")
 
         try:
             CompareColumnTask(
                 profile=ctx.obj["profile"],
                 project=ctx.obj["project"],
                 datasources=tconf["datasources"],
                 outfile_fqn=outfile_fqn,
@@ -461,20 +470,21 @@
                 ),
             ).execute()
         except Exception:
             log.error(f"Column comparison failed with errorr: {traceback.format_exc()}")
 
     # CompareTask
     for tconf in compare_tasks:
-        log.debug(f"Executing compare with task profile: {tconf}")
+        nlog.info(f"Executing compare with task profile: {tconf}")
         final_outdir = get_task_outdir(
             run_dir=ctx.obj["project"]["run_result_dir"],
             task_conf=tconf,
         )
         outfile_fqn = Path(final_outdir, "comparison.xlsx")
+        nlog.debug(f"Output will be stored in: {final_outdir}")
 
         CompareTask(
             profile=ctx.obj["profile"],
             project=ctx.obj["project"],
             datasources=tconf["datasources"],
             outfile_fqn=outfile_fqn,
             sample_count=tconf["sample_count"] if "sample_count" in tconf else None,
@@ -482,19 +492,20 @@
             case_insensitive=(
                 tconf["case_insensitive"] if "case_insensitive" in tconf else False
             ),
         ).execute()
 
     # ScanTask
     for tconf in scan_tasks:
-        log.debug(f"Executing scan with task profile: {tconf}")
+        nlog.info(f"Executing scan with task profile: {tconf}")
         final_outdir = get_task_outdir(
             run_dir=ctx.obj["project"]["run_result_dir"],
             task_conf=tconf,
         )
+        nlog.debug(f"Output will be stored in: {final_outdir}")
 
         ScanTask(
             profile=ctx.obj["profile"],
             project=ctx.obj["project"],
             datasources=tconf["datasources"],
             final_outdir=final_outdir,
             compare=tconf["compare"] if "compare" in tconf else None,
```

### Comparing `tulona-0.8.0/core/tulona/cli/params.py` & `tulona-0.8.1/core/tulona/cli/params.py`

 * *Files identical despite different names*

### Comparing `tulona-0.8.0/core/tulona/config/profile.py` & `tulona-0.8.1/core/tulona/config/profile.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import logging
 from pathlib import Path
-from typing import Dict
+from typing import Dict, Union
 
 from tulona.exceptions import TulonaMissingPropertyError, TulonaProfileException
 from tulona.util.filesystem import path_exists
 from tulona.util.yaml_parser import read_yaml
 
 log = logging.getLogger(__name__)
 
@@ -14,15 +14,15 @@
 
 class Profile:
     @property
     def get_profile_root(self):
         return Path(Path.home(), ".tulona")
 
     @property
-    def profile_conf_path(self) -> str:
+    def profile_conf_path(self) -> Union[str, Path]:
         return Path(self.get_profile_root, PROFILE_FILE_NAME)
 
     def validate_profile_config(self, profile_dict_raw: dict) -> None:
         for proj in profile_dict_raw:
             proj_dict = profile_dict_raw[proj]
             if "profiles" not in proj_dict:
                 raise TulonaMissingPropertyError(
@@ -41,15 +41,15 @@
         log.debug(f"Attempting to load profile config from {profile_file_uri}")
 
         if not path_exists(profile_file_uri):
             raise TulonaProfileException(
                 f"Profile file {profile_file_uri} does not exist."
             )
 
-        profile_dict_raw = read_yaml(profile_file_uri)
+        profile_dict_raw = read_yaml(str(profile_file_uri))
 
         if not isinstance(profile_dict_raw, dict):
             raise TulonaProfileException(
                 f"{profile_file_uri} could not be parsed to a python dictionary."
             )
 
         log.debug(f"Profile config is successfully loaded from {profile_file_uri}")
```

### Comparing `tulona-0.8.0/core/tulona/config/project.py` & `tulona-0.8.1/core/tulona/config/project.py`

 * *Files 5% similar despite different names*

```diff
@@ -44,15 +44,15 @@
         log.debug(f"Attempting to load project config from {project_file_uri}")
 
         if not path_exists(project_file_uri):
             raise TulonaProjectException(
                 f"Project file {project_file_uri} does not exist."
             )
 
-        project_dict_raw = read_yaml(project_file_uri)
+        project_dict_raw = read_yaml(str(project_file_uri))
 
         if not isinstance(project_dict_raw, dict):
             raise TulonaProjectException(
                 f"{project_file_uri} could not be parsed to a python dictionary."
             )
 
         log.debug(f"Project config is successfully loaded from {project_file_uri}")
```

### Comparing `tulona-0.8.0/core/tulona/exceptions.py` & `tulona-0.8.1/core/tulona/exceptions.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,14 +29,21 @@
 class TulonaProfileException(Exception):
     def __init__(self, message: str):
         self.message = message
         self.formatted_message = f"ERROR: {self.message}"
         super().__init__(self.formatted_message)
 
 
+class TulonaInvalidConfigError(Exception):
+    def __init__(self, message: str):
+        self.message = message
+        self.formatted_message = f"ERROR: {self.message}"
+        super().__init__(self.formatted_message)
+
+
 class TulonaInvalidProfileConfigError(Exception):
     def __init__(self, message: str):
         self.message = message
         self.formatted_message = f"ERROR: {self.message}"
         super().__init__(self.formatted_message)
```

### Comparing `tulona-0.8.0/core/tulona/task/base.py` & `tulona-0.8.1/core/tulona/task/base.py`

 * *Files identical despite different names*

### Comparing `tulona-0.8.0/core/tulona/task/compare.py` & `tulona-0.8.1/core/tulona/task/compare.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 from dataclasses import _MISSING_TYPE, dataclass, fields
 from pathlib import Path
 from typing import Dict, List
 
 import pandas as pd
 
 from tulona.exceptions import (
+    TulonaInvalidConfigError,
     TulonaMissingPrimaryKeyError,
     TulonaMissingPropertyError,
     TulonaUnsupportedQueryError,
 )
 from tulona.task.base import BaseTask
 from tulona.task.helper import perform_comparison
 from tulona.task.profile import ProfileTask
@@ -56,18 +57,47 @@
             if (
                 not isinstance(field.default, _MISSING_TYPE)
                 and getattr(self, field.name) is None
             ):
                 setattr(self, field.name, field.default)
 
     def extract_confs(self):
+        def validate_conjunct_configs(econf_dict: Dict):
+            if len(econf_dict["queries"]) > 0 and len(econf_dict["queries"]) != len(
+                self.datasources
+            ):
+                raise TulonaInvalidConfigError(
+                    "If `query` is used for a datasource, it must be used"
+                    " for all datasources."
+                )
+            if len(econf_dict["queries"]) == 0 and len(econf_dict["table_fqns"]) != len(
+                self.datasources
+            ):
+                raise TulonaInvalidConfigError(
+                    "If `query` is not used, `table` must be used" " for all datasources."
+                )
+
+            # Validate primary key
+            if (
+                len(
+                    {
+                        tuple(map(lambda x: x.lower(), k))
+                        for k in econf_dict["primary_keys"]
+                    }
+                )
+                > 1
+            ):
+                raise ValueError(
+                    "Primary key must be same in all candidate tables for comparison"
+                )
+
         # TODO: Add support for different names of primary keys in different tables
         # Check if primary key[s] is[are] specified for row comparison
         econf_dict = {}
-        primary_keys = []
+        econf_dict["primary_keys"] = []
         econf_dict["ds_names"] = []
         econf_dict["ds_name_compressed_list"] = []
         econf_dict["ds_configs"] = []
         econf_dict["dbtypes"] = []
         econf_dict["table_fqns"] = []
         econf_dict["queries"] = []
         econf_dict["connection_managers"] = []
@@ -94,26 +124,16 @@
                 if "database" in ds_config and dbtype.lower() != "mysql":
                     database = ds_config["database"]
                 else:
                     database = None
                 schema = ds_config["schema"]
                 table = ds_config["table"]
 
-                table_fqn = get_table_fqn(
-                    database,
-                    schema,
-                    table,
-                )
-
+                table_fqn = get_table_fqn(database, schema, table)
                 econf_dict["table_fqns"].append(table_fqn)
-            if "query" not in ds_config and "table" not in ds_config:
-                raise TulonaMissingPropertyError(
-                    "Either 'table' or 'query' must be specified"
-                    "in datasource config for row comparison."
-                )
 
             exclude_columns = (
                 ds_config["exclude_columns"] if "exclude_columns" in ds_config else []
             )
             if isinstance(exclude_columns, str):
                 exclude_columns = [exclude_columns]
             econf_dict["exclude_columns_lol"].append(exclude_columns)
@@ -128,170 +148,155 @@
                     (ds_config["primary_key"],)
                     if isinstance(ds_config["primary_key"], str)
                     else tuple(sorted(ds_config["primary_key"]))
                 )
                 log.debug(f"Provided primary key for datasource {ds_name}: {ds_pk}")
             else:
                 log.debug(
-                    f"Primary key not provided for datasource {ds_name}"
+                    f"Primary key not provided for datasource {ds_name}."
                     " Tulona will try to extract it from table metadata"
                 )
                 ds_pk = tuple(get_table_primary_keys(conman.engine, schema, table))
-                log.debug(f"Extracted primary key for datasource {ds_name}: {ds_pk}")
-
-            if len(ds_pk) > 0:
-                primary_keys.append(ds_pk)
+                if not ds_pk:
+                    raise TulonaMissingPrimaryKeyError(
+                        "Primary key[s] is[are] not available"
+                        f" for {table_fqn}[{ds_name}]. Abort!"
+                    )
+                else:
+                    log.debug(f"Extracted primary key for datasource {ds_name}: {ds_pk}")
 
-        pk_ci_set = {tuple(map(lambda x: x.lower(), k)) for k in primary_keys}
+            if ds_pk:
+                econf_dict["primary_keys"].append(ds_pk)
 
-        if len(primary_keys) == 0:
-            raise TulonaMissingPrimaryKeyError(
-                "Primary key[s] is[are] not available. Abort!"
-            )
-        elif len(primary_keys) > 0:
-            if len(primary_keys) != len(primary_keys):
-                raise TulonaMissingPrimaryKeyError(
-                    "If primary key is provided, it must be provided for all datasources"
-                )
+        # Validate the config counterparts
+        validate_conjunct_configs(econf_dict)
 
-            if len(pk_ci_set) > 1:
-                raise ValueError(
-                    "Primary key must be same in all candidate tables for comparison"
-                )
-            econf_dict["primary_key"] = primary_keys[0]
-            log.debug(f"Final primary key: {econf_dict['primary_key']}")
-        else:
-            raise TulonaMissingPrimaryKeyError(
-                f"Primary key for {table_fqn}[{ds_name}] could not be found."
-                " Row comparison without primary key has not been implemented yet."
-                " Abort!"
-            )
+        econf_dict["primary_key"] = econf_dict["primary_keys"][0]
+        log.debug(f"Final primary key: {econf_dict['primary_key']}")
 
         return econf_dict
 
     def execute(self):
         log.info("------------------------ Starting task: compare-row")
         start_time = time.time()
 
         if len(self.datasources) != 2:
             raise ValueError("Data comparison needs two data sources.")
+        log.info(f"Comparing {self.datasources}")
 
         # Config extraction
         econf_dict = self.extract_confs()
         dbtype1, dbtype2 = econf_dict["dbtypes"]
-        if "table_fqns" in econf_dict and len(econf_dict["table_fqns"]) > 0:
-            table_fqn1, table_fqn2 = econf_dict["table_fqns"]
-            log.debug(f"Sample count: {self.sample_count}")
-        else:
-            query1, query2 = econf_dict["queries"]
         exclude_columns1, exclude_columns2 = econf_dict["exclude_columns_lol"]
         conman1, conman2 = econf_dict["connection_managers"]
 
+        if len(econf_dict["queries"]) > 0:
+            data_container1 = "(" + econf_dict["queries"][0] + ") t"
+            data_container2 = "(" + econf_dict["queries"][1] + ") t"
+        else:
+            table_fqn1, table_fqn2 = econf_dict["table_fqns"]
+            data_container1 = table_fqn1
+            data_container2 = table_fqn2
+            log.debug(f"Sample count: {self.sample_count}")
+
         # TODO: push column exclusion down to the database/query
         # TODO: We probably don't need to create pk tuple out of pk
         # lists as that is already happening while extracting pks
         primary_key = tuple([k for k in econf_dict["primary_key"]])
         query_expr = None
 
-        log.info(f"Comparing {self.datasources}")
         df1 = df2 = pd.DataFrame()
-        num_try = 1 if "queries" in econf_dict else 5
+        num_try = 5
         i = 0
         while i < num_try:
             log.debug(f"Extraction iteration: {i + 1}/{num_try}")
 
-            if "table_fqns" in econf_dict and len(econf_dict["table_fqns"]) > 0:
-                query1 = get_table_data_query(
-                    dbtype1, table_fqn1, self.sample_count, query_expr
-                )
+            query1 = get_table_data_query(
+                dbtype=dbtype1,
+                data_container=data_container1,
+                sample_count=self.sample_count,
+                query_expr=query_expr,
+            )
 
             sanitized_query1 = re.sub(r"where(.*)\(.*\)", r"where\g<1>(...)", query1)
             log.debug(f"Executing query: {sanitized_query1}")
 
             try:
                 df1 = get_query_output_as_df(
                     connection_manager=conman1, query_text=query1
                 )
             except Exception as exc:
                 log.warning(f"Previous query failed with error: {exc}")
-                if "table_fqns" not in econf_dict:
+                if len(econf_dict["queries"]) > 0:
                     raise TulonaUnsupportedQueryError(
                         "The provided query is unsupported!"
                         " Please try to execute it in the database platform first."
+                        f" Query: {econf_dict['queries'][0]}"
                     )
-                log.debug(
-                    "Trying query with quoted column names for the filter expression"
-                )
+
                 if query_expr and i > 0:
+                    log.debug(
+                        "Trying query with quoted column names for the filter expression"
+                    )
                     query_expr = build_filter_query_expression(
                         df1, primary_key, quoted=True, positive=False
                     )
                 else:
                     raise TulonaUnsupportedQueryError(
                         "Something is wrong with following query,"
                         " please try to execute it in the database platform first."
                         f" Query: {query1}"
                     )
-                if "table_fqns" in econf_dict and len(econf_dict["table_fqns"]) > 0:
-                    query1 = get_table_data_query(
-                        dbtype1, table_fqn1, self.sample_count, query_expr
-                    )
-                sanitized_query1 = re.sub(r"where(.*)\(.*\)", r"where\g<1>(...)", query1)
-                log.debug(f"Executing query: {sanitized_query1}")
-                df1 = get_query_output_as_df(
-                    connection_manager=conman1, query_text=query1
-                )
 
-            if df1.shape[0] == 0:
-                log.warning(f"Couldn't extract rows from {table_fqn1}")
-                i += 1
-                continue
+            if df1.empty:
+                raise ValueError(f"Couldn't extract rows from {data_container1}")
 
             df1 = df1.rename(columns={c: c.lower() for c in df1.columns})
             for k in primary_key:
                 if k.lower() not in df1.columns.tolist():
-                    raise ValueError(f"Primary key {k} not present in {table_fqn1}")
+                    raise ValueError(f"Primary key {k} not present in {data_container1}")
 
             # Exclude columns
             if len(exclude_columns1) > 0:
                 log.debug(
                     f"Excluding columns from {econf_dict['ds_names'][0]}: {exclude_columns1}"
                 )
                 exclude_columns1 = [c.lower() for c in exclude_columns1]
                 df1 = apply_column_exclusion(
                     df1, primary_key, exclude_columns1, econf_dict["ds_names"][0]
                 )
-            if "table_fqns" in econf_dict and len(econf_dict["table_fqns"]) > 0:
-                query2 = get_table_data_query(
-                    dbtype2,
-                    table_fqn2,
-                    self.sample_count,
-                    query_expr=build_filter_query_expression(df1, primary_key),
-                )
+
+            query2 = get_table_data_query(
+                dbtype=dbtype2,
+                data_container=data_container2,
+                sample_count=self.sample_count,
+                query_expr=build_filter_query_expression(df1, primary_key),
+            )
             sanitized_query2 = re.sub(r"where(.*)\(.*\)", r"where\g<1>(...)", query2)
             log.debug(f"Executing query: {sanitized_query2}")
 
             try:
                 df2 = get_query_output_as_df(
                     connection_manager=conman2, query_text=query2
                 )
             except Exception as exc:
                 log.warning(f"Previous query failed with error: {exc}")
-                if "table_fqns" not in econf_dict:
+                if len(econf_dict["queries"]) > 0:
                     raise TulonaUnsupportedQueryError(
                         "The provided query is unsupported!"
                         " Please try to execute it in the database platform first."
+                        f" Query: {econf_dict['queries'][1]}"
                     )
                 log.debug(
                     "Trying query with quoted column names for the filter expression"
                 )
                 query2 = get_table_data_query(
-                    dbtype2,
-                    table_fqn2,
-                    self.sample_count,
+                    dbtype=dbtype2,
+                    data_container=data_container2,
+                    sample_count=self.sample_count,
                     query_expr=build_filter_query_expression(
                         df1, primary_key, quoted=True
                     ),
                 )
                 sanitized_query2 = re.sub(r"where(.*)\(.*\)", r"where\g<1>(...)", query2)
                 log.debug(f"Executing query: {sanitized_query2}")
                 df2 = get_query_output_as_df(
@@ -325,15 +330,15 @@
                     df1, primary_key, positive=False
                 )
 
             i += 1
 
         if df2.empty:
             raise ValueError(
-                f"Could not find common rows between {table_fqn1} and {table_fqn2}"
+                f"Could not find common rows between {data_container1} and {data_container2}"
             )
 
         log.debug(
             f"Preparing row comparison for: {econf_dict['ds_name_compressed_list']}"
         )
         df_row_comp = perform_comparison(
             ds_compressed_names=econf_dict["ds_name_compressed_list"],
```

### Comparing `tulona-0.8.0/core/tulona/task/helper.py` & `tulona-0.8.1/core/tulona/task/helper.py`

 * *Files identical despite different names*

### Comparing `tulona-0.8.0/core/tulona/task/ping.py` & `tulona-0.8.1/core/tulona/task/ping.py`

 * *Files identical despite different names*

### Comparing `tulona-0.8.0/core/tulona/task/profile.py` & `tulona-0.8.1/core/tulona/task/profile.py`

 * *Files identical despite different names*

### Comparing `tulona-0.8.0/core/tulona/task/scan.py` & `tulona-0.8.1/core/tulona/task/scan.py`

 * *Files identical despite different names*

### Comparing `tulona-0.8.0/core/tulona/util/database.py` & `tulona-0.8.1/core/tulona/util/database.py`

 * *Files identical despite different names*

### Comparing `tulona-0.8.0/core/tulona/util/dataframe.py` & `tulona-0.8.1/core/tulona/util/dataframe.py`

 * *Files identical despite different names*

### Comparing `tulona-0.8.0/core/tulona/util/excel.py` & `tulona-0.8.1/core/tulona/util/excel.py`

 * *Files identical despite different names*

### Comparing `tulona-0.8.0/core/tulona/util/filesystem.py` & `tulona-0.8.1/core/tulona/util/filesystem.py`

 * *Files identical despite different names*

### Comparing `tulona-0.8.0/core/tulona/util/profiles.py` & `tulona-0.8.1/core/tulona/util/profiles.py`

 * *Files identical despite different names*

### Comparing `tulona-0.8.0/core/tulona/util/sql.py` & `tulona-0.8.1/core/tulona/util/sql.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,28 +6,28 @@
 
 
 def get_table_fqn(database: Optional[str], schema: str, table: str) -> str:
     table_fqn = f"{database + '.' if database else ''}{schema}.{table}"
     return table_fqn
 
 
-def get_sample_row_query(dbtype: str, table_name: str, sample_count: int):
+def get_sample_row_query(dbtype: str, data_container: str, sample_count: int):
     dbtype = dbtype.lower()
 
     # TODO: validate sampling mechanism for maximum possible randomness
     if dbtype == "snowflake":
-        query = f"select * from {table_name} tablesample ({sample_count} rows)"
+        query = f"select * from {data_container} tablesample ({sample_count} rows)"
     elif dbtype == "mssql":
-        query = f"select top {sample_count} * from {table_name}"
+        query = f"select top {sample_count} * from {data_container}"
     elif dbtype == "postgres":
         # TODO: system_rows method not implemented, tablesample works for percentage selection
         # query = f"select * from {table_name} tablesample system_rows({sample_count})"
-        query = f"select * from {table_name} limit {sample_count}"
+        query = f"select * from {data_container} limit {sample_count}"
     elif dbtype == "mysql":
-        query = f"select * from {table_name} limit {sample_count}"
+        query = f"select * from {data_container} limit {sample_count}"
     else:
         raise TulonaNotImplementedError(
             f"Extracting sample rows from adapter type {dbtype} is not implemented."
         )
 
     return query
 
@@ -178,16 +178,16 @@
     from {table_fqn}
     """
 
     return query
 
 
 def get_table_data_query(
-    dbtype, table_fqn, sample_count, query_expr: Optional[str] = None
+    dbtype, data_container, sample_count, query_expr: Optional[str] = None
 ):
     if query_expr:
-        query = f"select * from {table_fqn} where {query_expr}"
+        query = f"select * from {data_container} where {query_expr}"
     else:
         query = get_sample_row_query(
-            dbtype=dbtype, table_name=table_fqn, sample_count=sample_count
+            dbtype=dbtype, data_container=data_container, sample_count=sample_count
         )
     return query
```

### Comparing `tulona-0.8.0/core/tulona.egg-info/PKG-INFO` & `tulona-0.8.1/core/tulona.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tulona
-Version: 0.8.0
+Version: 0.8.1
 Summary: A tool to compare data from different sources.
 Author: Mrinal Kanti Sardar
 Project-URL: Homepage, https://github.com/mrinalsardar/tulona
 Project-URL: Documentation, https://github.com/mrinalsardar/tulona
 Project-URL: Repository, https://github.com/mrinalsardar/tulona.git
 Project-URL: Issues, https://github.com/mrinalsardar/tulona/issues
 Keywords: tulona,comparison,data comparison,database scan,database profile
```

### Comparing `tulona-0.8.0/core/tulona.egg-info/SOURCES.txt` & `tulona-0.8.1/core/tulona.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tulona-0.8.0/pyproject.toml` & `tulona-0.8.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "tulona"
-version = "0.8.0"
+version = "0.8.1"
 description = "A tool to compare data from different sources."
 dependencies = [
   "click~=8.1",
   "ruamel.yaml~=0.18",
   "psycopg2-binary~=2.9",
   "pymysql~=1.1",
   "cryptography~=42.0",
@@ -125,15 +125,15 @@
 
 [tool.isort]
 profile = "black"
 line_length = 90
 skip = [".gitignore"]
 
 [tool.bumpversion]
-current_version = "0.8.0"
+current_version = "0.8.1"
 parse = "(?P<major>\\d+)\\.(?P<minor>\\d+)\\.(?P<patch>\\d+)"
 serialize = ["{major}.{minor}.{patch}"]
 search = "{current_version}"
 replace = "{new_version}"
 regex = false
 ignore_missing_version = false
 tag = false
```

