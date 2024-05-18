# Comparing `tmp/ikctl-0.2.12.tar.gz` & `tmp/ikctl-0.2.14.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ikctl-0.2.12.tar", last modified: Sat May 11 21:20:08 2024, max compression
+gzip compressed data, was "ikctl-0.2.14.tar", last modified: Sat May 18 18:01:07 2024, max compression
```

## Comparing `ikctl-0.2.12.tar` & `ikctl-0.2.14.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 davidmoyalopez   (501) staff       (20)        0 2024-05-11 21:20:08.104640 ikctl-0.2.12/
--rw-r--r--   0 davidmoyalopez   (501) staff       (20)    11357 2024-05-01 15:41:01.000000 ikctl-0.2.12/LICENSE
--rw-r--r--   0 davidmoyalopez   (501) staff       (20)     2415 2024-05-11 21:20:08.104424 ikctl-0.2.12/PKG-INFO
--rw-r--r--   0 davidmoyalopez   (501) staff       (20)     2033 2024-05-11 21:14:57.000000 ikctl-0.2.12/README.md
-drwxr-xr-x   0 davidmoyalopez   (501) staff       (20)        0 2024-05-11 21:20:08.102825 ikctl-0.2.12/ikctl/
--rw-r--r--   0 davidmoyalopez   (501) staff       (20)       30 2024-05-01 15:41:01.000000 ikctl-0.2.12/ikctl/__init__.py
--rw-r--r--   0 davidmoyalopez   (501) staff       (20)     1048 2024-05-11 21:04:11.000000 ikctl-0.2.12/ikctl/commands.py
--rw-r--r--   0 davidmoyalopez   (501) staff       (20)     4427 2024-05-11 21:04:11.000000 ikctl-0.2.12/ikctl/config.py
--rw-r--r--   0 davidmoyalopez   (501) staff       (20)     1607 2024-05-01 15:41:01.000000 ikctl-0.2.12/ikctl/connect.py
--rw-r--r--   0 davidmoyalopez   (501) staff       (20)     1282 2024-05-01 15:41:01.000000 ikctl-0.2.12/ikctl/context.py
--rw-r--r--   0 davidmoyalopez   (501) staff       (20)     3514 2024-05-11 21:04:11.000000 ikctl-0.2.12/ikctl/create_config_files.py
--rw-r--r--   0 davidmoyalopez   (501) staff       (20)      970 2024-05-01 15:41:01.000000 ikctl-0.2.12/ikctl/execute.py
--rw-r--r--   0 davidmoyalopez   (501) staff       (20)      327 2024-05-01 15:41:01.000000 ikctl-0.2.12/ikctl/logs.py
--rwxr-xr-x   0 davidmoyalopez   (501) staff       (20)      794 2024-05-01 15:41:01.000000 ikctl-0.2.12/ikctl/main.py
--rw-r--r--   0 davidmoyalopez   (501) staff       (20)     3023 2024-05-01 15:41:01.000000 ikctl-0.2.12/ikctl/pipeline.py
--rw-r--r--   0 davidmoyalopez   (501) staff       (20)      927 2024-05-01 15:41:01.000000 ikctl-0.2.12/ikctl/sftp.py
--rw-r--r--   0 davidmoyalopez   (501) staff       (20)     1044 2024-05-01 15:41:01.000000 ikctl-0.2.12/ikctl/view.py
-drwxr-xr-x   0 davidmoyalopez   (501) staff       (20)        0 2024-05-11 21:20:08.104047 ikctl-0.2.12/ikctl.egg-info/
--rw-r--r--   0 davidmoyalopez   (501) staff       (20)     2415 2024-05-11 21:20:08.000000 ikctl-0.2.12/ikctl.egg-info/PKG-INFO
--rw-r--r--   0 davidmoyalopez   (501) staff       (20)      408 2024-05-11 21:20:08.000000 ikctl-0.2.12/ikctl.egg-info/SOURCES.txt
--rw-r--r--   0 davidmoyalopez   (501) staff       (20)        1 2024-05-11 21:20:08.000000 ikctl-0.2.12/ikctl.egg-info/dependency_links.txt
--rw-r--r--   0 davidmoyalopez   (501) staff       (20)       51 2024-05-11 21:20:08.000000 ikctl-0.2.12/ikctl.egg-info/entry_points.txt
--rw-r--r--   0 davidmoyalopez   (501) staff       (20)       23 2024-05-11 21:20:08.000000 ikctl-0.2.12/ikctl.egg-info/requires.txt
--rw-r--r--   0 davidmoyalopez   (501) staff       (20)        6 2024-05-11 21:20:08.000000 ikctl-0.2.12/ikctl.egg-info/top_level.txt
--rw-r--r--   0 davidmoyalopez   (501) staff       (20)       38 2024-05-11 21:20:08.104679 ikctl-0.2.12/setup.cfg
--rw-r--r--   0 davidmoyalopez   (501) staff       (20)      736 2024-05-11 21:19:18.000000 ikctl-0.2.12/setup.py
+drwxr-xr-x   0 davidmoyalopez   (501) staff       (20)        0 2024-05-18 18:01:07.502239 ikctl-0.2.14/
+-rw-r--r--   0 davidmoyalopez   (501) staff       (20)    11357 2024-05-01 15:41:01.000000 ikctl-0.2.14/LICENSE
+-rw-r--r--   0 davidmoyalopez   (501) staff       (20)     2415 2024-05-18 18:01:07.502015 ikctl-0.2.14/PKG-INFO
+-rw-r--r--   0 davidmoyalopez   (501) staff       (20)     2033 2024-05-11 21:14:57.000000 ikctl-0.2.14/README.md
+drwxr-xr-x   0 davidmoyalopez   (501) staff       (20)        0 2024-05-18 18:01:07.500775 ikctl-0.2.14/ikctl/
+-rw-r--r--   0 davidmoyalopez   (501) staff       (20)       30 2024-05-18 17:16:44.000000 ikctl-0.2.14/ikctl/__init__.py
+-rw-r--r--   0 davidmoyalopez   (501) staff       (20)     1048 2024-05-11 21:04:11.000000 ikctl-0.2.14/ikctl/commands.py
+-rw-r--r--   0 davidmoyalopez   (501) staff       (20)     4487 2024-05-18 18:01:00.000000 ikctl-0.2.14/ikctl/config.py
+-rw-r--r--   0 davidmoyalopez   (501) staff       (20)     1607 2024-05-01 15:41:01.000000 ikctl-0.2.14/ikctl/connect.py
+-rw-r--r--   0 davidmoyalopez   (501) staff       (20)     1282 2024-05-01 15:41:01.000000 ikctl-0.2.14/ikctl/context.py
+-rw-r--r--   0 davidmoyalopez   (501) staff       (20)     3514 2024-05-11 21:04:11.000000 ikctl-0.2.14/ikctl/create_config_files.py
+-rw-r--r--   0 davidmoyalopez   (501) staff       (20)      970 2024-05-01 15:41:01.000000 ikctl-0.2.14/ikctl/execute.py
+-rw-r--r--   0 davidmoyalopez   (501) staff       (20)      327 2024-05-01 15:41:01.000000 ikctl-0.2.14/ikctl/logs.py
+-rwxr-xr-x   0 davidmoyalopez   (501) staff       (20)      895 2024-05-18 18:01:00.000000 ikctl-0.2.14/ikctl/main.py
+-rw-r--r--   0 davidmoyalopez   (501) staff       (20)     3071 2024-05-18 18:01:00.000000 ikctl-0.2.14/ikctl/pipeline.py
+-rw-r--r--   0 davidmoyalopez   (501) staff       (20)      927 2024-05-01 15:41:01.000000 ikctl-0.2.14/ikctl/sftp.py
+-rw-r--r--   0 davidmoyalopez   (501) staff       (20)     1044 2024-05-01 15:41:01.000000 ikctl-0.2.14/ikctl/view.py
+drwxr-xr-x   0 davidmoyalopez   (501) staff       (20)        0 2024-05-18 18:01:07.501660 ikctl-0.2.14/ikctl.egg-info/
+-rw-r--r--   0 davidmoyalopez   (501) staff       (20)     2415 2024-05-18 18:01:07.000000 ikctl-0.2.14/ikctl.egg-info/PKG-INFO
+-rw-r--r--   0 davidmoyalopez   (501) staff       (20)      408 2024-05-18 18:01:07.000000 ikctl-0.2.14/ikctl.egg-info/SOURCES.txt
+-rw-r--r--   0 davidmoyalopez   (501) staff       (20)        1 2024-05-18 18:01:07.000000 ikctl-0.2.14/ikctl.egg-info/dependency_links.txt
+-rw-r--r--   0 davidmoyalopez   (501) staff       (20)       51 2024-05-18 18:01:07.000000 ikctl-0.2.14/ikctl.egg-info/entry_points.txt
+-rw-r--r--   0 davidmoyalopez   (501) staff       (20)       23 2024-05-18 18:01:07.000000 ikctl-0.2.14/ikctl.egg-info/requires.txt
+-rw-r--r--   0 davidmoyalopez   (501) staff       (20)        6 2024-05-18 18:01:07.000000 ikctl-0.2.14/ikctl.egg-info/top_level.txt
+-rw-r--r--   0 davidmoyalopez   (501) staff       (20)       38 2024-05-18 18:01:07.502285 ikctl-0.2.14/setup.cfg
+-rw-r--r--   0 davidmoyalopez   (501) staff       (20)     1417 2024-05-18 18:01:00.000000 ikctl-0.2.14/setup.py
```

### Comparing `ikctl-0.2.12/LICENSE` & `ikctl-0.2.14/LICENSE`

 * *Files identical despite different names*

### Comparing `ikctl-0.2.12/PKG-INFO` & `ikctl-0.2.14/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ikctl
-Version: 0.2.12
+Version: 0.2.14
 Summary: App to installer packages on remote servers
 Home-page: https://github.com/3nueves/ikctl
 Author: David Moya López
 Author-email: 3nueves@gmail.com
 License: Apache v2.0
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
```

### Comparing `ikctl-0.2.12/README.md` & `ikctl-0.2.14/README.md`

 * *Files identical despite different names*

### Comparing `ikctl-0.2.12/ikctl/commands.py` & `ikctl-0.2.14/ikctl/commands.py`

 * *Files identical despite different names*

### Comparing `ikctl-0.2.12/ikctl/config.py` & `ikctl-0.2.14/ikctl/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,22 @@
 """ Module to load configuration """
 import pathlib
 import os
 import sys
 from envyaml import EnvYAML
 from .create_config_files import CreateFolderAndConfigFile
 
+__version__ = "v0.2.14"
+
 class Config():
     """ Manage path kits """
 
     def __init__(self):
         self.config = ""
+        self.version = __version__
         self.home = pathlib.Path.home()
         self.path_config_file = self.home.joinpath('.ikctl/config')
         self.create_config_file = CreateFolderAndConfigFile()
         self.__create_folder_and_config_file()
         self.__load_config_file_where_are_kits()
         self.context = self.config['context']
```

### Comparing `ikctl-0.2.12/ikctl/connect.py` & `ikctl-0.2.14/ikctl/connect.py`

 * *Files identical despite different names*

### Comparing `ikctl-0.2.12/ikctl/context.py` & `ikctl-0.2.14/ikctl/context.py`

 * *Files identical despite different names*

### Comparing `ikctl-0.2.12/ikctl/create_config_files.py` & `ikctl-0.2.14/ikctl/create_config_files.py`

 * *Files identical despite different names*

### Comparing `ikctl-0.2.12/ikctl/execute.py` & `ikctl-0.2.14/ikctl/execute.py`

 * *Files identical despite different names*

### Comparing `ikctl-0.2.12/ikctl/main.py` & `ikctl-0.2.14/ikctl/main.py`

 * *Files 20% similar despite different names*

```diff
@@ -2,16 +2,18 @@
 import argparse
 
 from .pipeline import Pipeline
 
 def create_parser():
     """ CLI class """
     parser = argparse.ArgumentParser(description="tool for install software in remote servers", prog="ikctl")
+    parser.version = Pipeline().version
     parser.add_argument("-l", "--list", choices=["kits", "servers", "context"], help="option to list kits, servers or context")
     parser.add_argument("-i", "--install", help="Select kit to use")
     parser.add_argument("-n", "--name", help="Name of the groups servers")
     parser.add_argument("-p", "--parameter", nargs = '*', help="Add parameters")
     parser.add_argument("-s", "--sudo", choices=["sudo"], help="exec from sudo")
     parser.add_argument("-c", "--context", help="Select context")
+    parser.add_argument("-v", "--version", action='version')
     return parser.parse_args()
 
 Pipeline().init(create_parser())
```

### Comparing `ikctl-0.2.12/ikctl/pipeline.py` & `ikctl-0.2.14/ikctl/pipeline.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 from .context import Context
 
 class Pipeline:
     """ Class where we will initiation the process to install kits on remote servers """
 
     def __init__(self):
 
+        self.version = Config().version
         self.path = []
         self.files = []
         self.log = Log()
         self.exe = Exec()
         self.sftp = Sftp()
         self.data = Config()
         self.connection = []
@@ -45,15 +46,15 @@
         # Manage context
         if options.context:
             self.context.change_context(options.context)
                 
         # Show configuration
         if options.list:
             self.view.show_config(options.list)
-
+        
         # Install kits in servers
         if options.install:
 
             # Load kit
             kits = self.data.extrac_config_kits(self.config_kits, options.install)
             if kits is None:
                 print("Kit not found")
```

### Comparing `ikctl-0.2.12/ikctl/sftp.py` & `ikctl-0.2.14/ikctl/sftp.py`

 * *Files identical despite different names*

### Comparing `ikctl-0.2.12/ikctl/view.py` & `ikctl-0.2.14/ikctl/view.py`

 * *Files identical despite different names*

### Comparing `ikctl-0.2.12/ikctl.egg-info/PKG-INFO` & `ikctl-0.2.14/ikctl.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ikctl
-Version: 0.2.12
+Version: 0.2.14
 Summary: App to installer packages on remote servers
 Home-page: https://github.com/3nueves/ikctl
 Author: David Moya López
 Author-email: 3nueves@gmail.com
 License: Apache v2.0
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
```

