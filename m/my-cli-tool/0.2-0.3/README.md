# Comparing `tmp/my_cli_tool-0.2.tar.gz` & `tmp/my_cli_tool-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "my_cli_tool-0.2.tar", last modified: Sat May 18 08:21:21 2024, max compression
+gzip compressed data, was "my_cli_tool-0.3.tar", last modified: Sat May 18 08:23:09 2024, max compression
```

## Comparing `my_cli_tool-0.2.tar` & `my_cli_tool-0.3.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 zengbobo   (501) staff       (20)        0 2024-05-18 08:21:21.113567 my_cli_tool-0.2/
--rw-r--r--   0 zengbobo   (501) staff       (20)      565 2024-05-18 08:21:21.113307 my_cli_tool-0.2/PKG-INFO
--rw-r--r--   0 zengbobo   (501) staff       (20)       65 2024-05-18 07:55:10.000000 my_cli_tool-0.2/README.md
-drwxr-xr-x   0 zengbobo   (501) staff       (20)        0 2024-05-18 08:21:21.112695 my_cli_tool-0.2/my_cli_tool.egg-info/
--rw-r--r--   0 zengbobo   (501) staff       (20)      565 2024-05-18 08:21:21.000000 my_cli_tool-0.2/my_cli_tool.egg-info/PKG-INFO
--rw-r--r--   0 zengbobo   (501) staff       (20)      196 2024-05-18 08:21:21.000000 my_cli_tool-0.2/my_cli_tool.egg-info/SOURCES.txt
--rw-r--r--   0 zengbobo   (501) staff       (20)        1 2024-05-18 08:21:21.000000 my_cli_tool-0.2/my_cli_tool.egg-info/dependency_links.txt
--rw-r--r--   0 zengbobo   (501) staff       (20)       48 2024-05-18 08:21:21.000000 my_cli_tool-0.2/my_cli_tool.egg-info/entry_points.txt
--rw-r--r--   0 zengbobo   (501) staff       (20)        1 2024-05-18 08:21:21.000000 my_cli_tool-0.2/my_cli_tool.egg-info/top_level.txt
--rw-r--r--   0 zengbobo   (501) staff       (20)       38 2024-05-18 08:21:21.113667 my_cli_tool-0.2/setup.cfg
--rw-r--r--   0 zengbobo   (501) staff       (20)      978 2024-05-18 08:21:01.000000 my_cli_tool-0.2/setup.py
+drwxr-xr-x   0 zengbobo   (501) staff       (20)        0 2024-05-18 08:23:09.595481 my_cli_tool-0.3/
+-rw-r--r--   0 zengbobo   (501) staff       (20)      565 2024-05-18 08:23:09.595149 my_cli_tool-0.3/PKG-INFO
+-rw-r--r--   0 zengbobo   (501) staff       (20)       65 2024-05-18 07:55:10.000000 my_cli_tool-0.3/README.md
+drwxr-xr-x   0 zengbobo   (501) staff       (20)        0 2024-05-18 08:23:09.594593 my_cli_tool-0.3/my_cli_tool.egg-info/
+-rw-r--r--   0 zengbobo   (501) staff       (20)      565 2024-05-18 08:23:09.000000 my_cli_tool-0.3/my_cli_tool.egg-info/PKG-INFO
+-rw-r--r--   0 zengbobo   (501) staff       (20)      196 2024-05-18 08:23:09.000000 my_cli_tool-0.3/my_cli_tool.egg-info/SOURCES.txt
+-rw-r--r--   0 zengbobo   (501) staff       (20)        1 2024-05-18 08:23:09.000000 my_cli_tool-0.3/my_cli_tool.egg-info/dependency_links.txt
+-rw-r--r--   0 zengbobo   (501) staff       (20)       48 2024-05-18 08:23:09.000000 my_cli_tool-0.3/my_cli_tool.egg-info/entry_points.txt
+-rw-r--r--   0 zengbobo   (501) staff       (20)        1 2024-05-18 08:23:09.000000 my_cli_tool-0.3/my_cli_tool.egg-info/top_level.txt
+-rw-r--r--   0 zengbobo   (501) staff       (20)       38 2024-05-18 08:23:09.595708 my_cli_tool-0.3/setup.cfg
+-rw-r--r--   0 zengbobo   (501) staff       (20)      978 2024-05-18 08:23:02.000000 my_cli_tool-0.3/setup.py
```

### Comparing `my_cli_tool-0.2/PKG-INFO` & `my_cli_tool-0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: my_cli_tool
-Version: 0.2
+Version: 0.3
 Summary: A simple CLI tool to add two numbers.
 Home-page: https://github.com/yourusername/my_cli_tool
 Author: Your Name
 Author-email: your.email@example.com
 License: UNKNOWN
 Description: # My CLI Tool
```

### Comparing `my_cli_tool-0.2/my_cli_tool.egg-info/PKG-INFO` & `my_cli_tool-0.3/my_cli_tool.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: my-cli-tool
-Version: 0.2
+Version: 0.3
 Summary: A simple CLI tool to add two numbers.
 Home-page: https://github.com/yourusername/my_cli_tool
 Author: Your Name
 Author-email: your.email@example.com
 License: UNKNOWN
 Description: # My CLI Tool
```

### Comparing `my_cli_tool-0.2/setup.py` & `my_cli_tool-0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 long_description = ""
 if os.path.exists("README.md"):
     with open("README.md", "r", encoding="utf-8") as fh:
         long_description = fh.read()
 
 setup(
     name="my_cli_tool",
-    version="0.2",
+    version="0.3",
     packages=find_packages(),
     entry_points={
         "console_scripts": [
             "mycli=my_cli_tool.cli:main",
         ],
     },
     install_requires=[
```

