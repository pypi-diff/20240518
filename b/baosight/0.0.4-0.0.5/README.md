# Comparing `tmp/baosight-0.0.4.tar.gz` & `tmp/baosight-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "baosight-0.0.4.tar", last modified: Sat May 18 18:25:08 2024, max compression
+gzip compressed data, was "baosight-0.0.5.tar", last modified: Sat May 18 18:54:28 2024, max compression
```

## Comparing `baosight-0.0.4.tar` & `baosight-0.0.5.tar`

### file list

```diff
@@ -1,25 +1,26 @@
-drwxrwxrwx   0        0        0        0 2024-05-18 18:25:08.489935 baosight-0.0.4/
--rw-rw-rw-   0        0        0     1064 2023-10-25 05:23:47.000000 baosight-0.0.4/LICENSE
--rw-rw-rw-   0        0        0      126 2024-05-18 18:14:34.000000 baosight-0.0.4/MANIFEST.in
--rw-rw-rw-   0        0        0      783 2024-05-18 18:25:08.489935 baosight-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0      199 2024-05-18 18:18:59.000000 baosight-0.0.4/README.md
-drwxrwxrwx   0        0        0        0 2024-05-18 18:25:08.457938 baosight-0.0.4/baosight/
--rw-rw-rw-   0        0        0        0 2024-05-18 17:41:58.000000 baosight-0.0.4/baosight/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-18 18:25:08.483935 baosight-0.0.4/baosight/cli/
--rw-rw-rw-   0        0        0        0 2023-10-25 05:23:47.000000 baosight-0.0.4/baosight/cli/__init__.py
--rw-rw-rw-   0        0        0     1100 2024-05-18 18:04:07.000000 baosight-0.0.4/baosight/cli/gl_runner.py
--rw-rw-rw-   0        0        0     1418 2024-05-18 18:01:43.000000 baosight-0.0.4/baosight/cli/main.py
-drwxrwxrwx   0        0        0        0 2024-05-18 18:25:08.486935 baosight-0.0.4/baosight/tools/
--rw-rw-rw-   0        0        0        0 2024-05-18 17:42:50.000000 baosight-0.0.4/baosight/tools/__init__.py
--rw-rw-rw-   0        0        0     4563 2024-05-18 17:44:00.000000 baosight-0.0.4/baosight/tools/gitlab_runner.py
--rw-rw-rw-   0        0        0     7201 2024-05-18 18:24:21.000000 baosight-0.0.4/baosight/tools/gitlab_runner_gui.py
-drwxrwxrwx   0        0        0        0 2024-05-18 18:25:08.487935 baosight-0.0.4/baosight.egg-info/
--rw-rw-rw-   0        0        0      783 2024-05-18 18:25:08.000000 baosight-0.0.4/baosight.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      461 2024-05-18 18:25:08.000000 baosight-0.0.4/baosight.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-18 18:25:08.000000 baosight-0.0.4/baosight.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       52 2024-05-18 18:25:08.000000 baosight-0.0.4/baosight.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2024-05-18 18:25:07.000000 baosight-0.0.4/baosight.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       57 2024-05-18 18:25:08.000000 baosight-0.0.4/baosight.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-05-18 18:25:08.000000 baosight-0.0.4/baosight.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      666 2024-05-18 18:25:08.492936 baosight-0.0.4/setup.cfg
--rw-rw-rw-   0        0        0      171 2024-05-18 18:10:58.000000 baosight-0.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-18 18:54:28.675547 baosight-0.0.5/
+-rw-rw-rw-   0        0        0     1064 2023-10-25 05:23:47.000000 baosight-0.0.5/LICENSE
+-rw-rw-rw-   0        0        0      126 2024-05-18 18:14:34.000000 baosight-0.0.5/MANIFEST.in
+-rw-rw-rw-   0        0        0     1296 2024-05-18 18:54:28.675547 baosight-0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0      689 2024-05-18 18:35:53.000000 baosight-0.0.5/README.md
+drwxrwxrwx   0        0        0        0 2024-05-18 18:54:28.641611 baosight-0.0.5/baosight/
+-rw-rw-rw-   0        0        0        0 2024-05-18 17:41:58.000000 baosight-0.0.5/baosight/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-18 18:54:28.667611 baosight-0.0.5/baosight/cli/
+-rw-rw-rw-   0        0        0        0 2023-10-25 05:23:47.000000 baosight-0.0.5/baosight/cli/__init__.py
+-rw-rw-rw-   0        0        0     1415 2024-05-18 18:53:44.000000 baosight-0.0.5/baosight/cli/gl_runner.py
+-rw-rw-rw-   0        0        0     1418 2024-05-18 18:01:43.000000 baosight-0.0.5/baosight/cli/main.py
+drwxrwxrwx   0        0        0        0 2024-05-18 18:54:28.672546 baosight-0.0.5/baosight/tools/
+-rw-rw-rw-   0        0        0        0 2024-05-18 17:42:50.000000 baosight-0.0.5/baosight/tools/__init__.py
+-rw-rw-rw-   0        0        0     4563 2024-05-18 17:44:00.000000 baosight-0.0.5/baosight/tools/gitlab_runner.py
+-rw-rw-rw-   0        0        0     1526 2024-05-18 18:52:57.000000 baosight-0.0.5/baosight/tools/gitlab_runner_config_generator.py
+-rw-rw-rw-   0        0        0     7201 2024-05-18 18:24:21.000000 baosight-0.0.5/baosight/tools/gitlab_runner_gui.py
+drwxrwxrwx   0        0        0        0 2024-05-18 18:54:28.673545 baosight-0.0.5/baosight.egg-info/
+-rw-rw-rw-   0        0        0     1296 2024-05-18 18:54:28.000000 baosight-0.0.5/baosight.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      510 2024-05-18 18:54:28.000000 baosight-0.0.5/baosight.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-18 18:54:28.000000 baosight-0.0.5/baosight.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       52 2024-05-18 18:54:28.000000 baosight-0.0.5/baosight.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2024-05-18 18:54:28.000000 baosight-0.0.5/baosight.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       57 2024-05-18 18:54:28.000000 baosight-0.0.5/baosight.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-05-18 18:54:28.000000 baosight-0.0.5/baosight.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      666 2024-05-18 18:54:28.677549 baosight-0.0.5/setup.cfg
+-rw-rw-rw-   0        0        0      171 2024-05-18 18:10:58.000000 baosight-0.0.5/setup.py
```

### Comparing `baosight-0.0.4/LICENSE` & `baosight-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `baosight-0.0.4/baosight/cli/gl_runner.py` & `baosight-0.0.5/baosight/cli/gl_runner.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 from argparse import ArgumentParser
 from baosight.tools.gitlab_runner import deploy
 from baosight.tools.gitlab_runner_gui import create_installation_ui
+from baosight.tools.gitlab_runner_config_generator import generator
+
 
 class CLICommand:
     """
     安装gitlab runner,配置文件格式如下：
     {
       "gitlab_url": "http://127.0.0.1",
       "gitlab_api_token": "xxxxxxx",
@@ -22,15 +24,20 @@
       ],
     }
     """
 
     @staticmethod
     def add_arguments(parser: ArgumentParser):
         add = parser.add_argument
-        add("--quite", help="静默安装当前目录下的config.json")
+        add("--quite", action='store_true', help="静默安装当前目录下的config.json")
+        add("--create-config", dest="config", action='store_true', help="静默安装当前目录下的config.json")
 
     @staticmethod
     def run(args, parser):
+        if args.config:
+            generator()
+            deploy("config.json")
+            return
         if args.quite:
             deploy("config.json")
         else:
             create_installation_ui()
```

### Comparing `baosight-0.0.4/baosight/cli/main.py` & `baosight-0.0.5/baosight/cli/main.py`

 * *Files identical despite different names*

### Comparing `baosight-0.0.4/baosight/tools/gitlab_runner.py` & `baosight-0.0.5/baosight/tools/gitlab_runner.py`

 * *Files identical despite different names*

### Comparing `baosight-0.0.4/baosight/tools/gitlab_runner_gui.py` & `baosight-0.0.5/baosight/tools/gitlab_runner_gui.py`

 * *Files identical despite different names*

