# Comparing `tmp/shellper-0.3.1.tar.gz` & `tmp/shellper-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shellper-0.3.1.tar", last modified: Sat May 18 00:41:47 2024, max compression
+gzip compressed data, was "shellper-0.3.2.tar", last modified: Sat May 18 01:40:38 2024, max compression
```

## Comparing `shellper-0.3.1.tar` & `shellper-0.3.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2024-05-18 00:41:47.450153 shellper-0.3.1/
--rw-rw-rw-   0        0        0    11357 2024-04-29 10:47:19.000000 shellper-0.3.1/LICENSE.txt
--rw-rw-rw-   0        0        0     1121 2024-05-18 00:41:47.450153 shellper-0.3.1/PKG-INFO
--rw-rw-rw-   0        0        0      500 2024-05-18 00:40:22.000000 shellper-0.3.1/README.md
-drwxrwxrwx   0        0        0        0 2024-05-18 00:41:47.450153 shellper-0.3.1/Shellper.egg-info/
--rw-rw-rw-   0        0        0     1121 2024-05-18 00:41:47.000000 shellper-0.3.1/Shellper.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      250 2024-05-18 00:41:47.000000 shellper-0.3.1/Shellper.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-18 00:41:47.000000 shellper-0.3.1/Shellper.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2024-05-18 00:41:47.000000 shellper-0.3.1/Shellper.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-18 00:41:47.450153 shellper-0.3.1/setup.cfg
--rw-rw-rw-   0        0        0      837 2024-05-18 00:40:22.000000 shellper-0.3.1/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-18 00:41:47.450153 shellper-0.3.1/shellper/
--rw-rw-rw-   0        0        0      376 2024-05-16 12:12:42.000000 shellper-0.3.1/shellper/__init__.py
--rw-rw-rw-   0        0        0      378 2024-05-16 12:17:03.000000 shellper-0.3.1/shellper/datas.py
--rw-rw-rw-   0        0        0      853 2024-05-18 00:38:06.000000 shellper-0.3.1/shellper/inputs.py
--rw-rw-rw-   0        0        0     2639 2024-05-16 12:01:09.000000 shellper-0.3.1/shellper/log.py
--rw-rw-rw-   0        0        0      735 2024-05-12 07:22:51.000000 shellper-0.3.1/shellper/style.py
+drwxrwxrwx   0        0        0        0 2024-05-18 01:40:38.833476 shellper-0.3.2/
+-rw-rw-rw-   0        0        0    11357 2024-04-29 10:47:19.000000 shellper-0.3.2/LICENSE.txt
+-rw-rw-rw-   0        0        0     1197 2024-05-18 01:40:38.832476 shellper-0.3.2/PKG-INFO
+-rw-rw-rw-   0        0        0      576 2024-05-18 01:39:49.000000 shellper-0.3.2/README.md
+drwxrwxrwx   0        0        0        0 2024-05-18 01:40:38.830477 shellper-0.3.2/Shellper.egg-info/
+-rw-rw-rw-   0        0        0     1197 2024-05-18 01:40:38.000000 shellper-0.3.2/Shellper.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      250 2024-05-18 01:40:38.000000 shellper-0.3.2/Shellper.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-18 01:40:38.000000 shellper-0.3.2/Shellper.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2024-05-18 01:40:38.000000 shellper-0.3.2/Shellper.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-18 01:40:38.834476 shellper-0.3.2/setup.cfg
+-rw-rw-rw-   0        0        0      837 2024-05-18 01:39:49.000000 shellper-0.3.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-18 01:40:38.828477 shellper-0.3.2/shellper/
+-rw-rw-rw-   0        0        0      376 2024-05-16 12:12:42.000000 shellper-0.3.2/shellper/__init__.py
+-rw-rw-rw-   0        0        0      378 2024-05-16 12:17:03.000000 shellper-0.3.2/shellper/datas.py
+-rw-rw-rw-   0        0        0     1328 2024-05-18 01:37:06.000000 shellper-0.3.2/shellper/inputs.py
+-rw-rw-rw-   0        0        0     2639 2024-05-16 12:01:09.000000 shellper-0.3.2/shellper/log.py
+-rw-rw-rw-   0        0        0      735 2024-05-12 07:22:51.000000 shellper-0.3.2/shellper/style.py
```

### Comparing `shellper-0.3.1/LICENSE.txt` & `shellper-0.3.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `shellper-0.3.1/PKG-INFO` & `shellper-0.3.2/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Shellper
-Version: 0.3.1
+Version: 0.3.2
 Summary: A Python Library for create shell apps.
 Home-page: https://gitee.com/ShawnMerry/Shellper
 Author: ShawnMerry
 Author-email: merrybili@163.com
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
@@ -23,12 +23,13 @@
 
 #### [PyPI](https://pypi.org/project/Shellper)
 
 #### [Gitee](https://gitee.com/ShawnMerry/Shellper)
 
 ### Update Log:<br>
 
-v0.3.1 24/05/18 08:41: Inputs Function Add Callable Function.
+v0.3.2 24/05/18 09:40: Inputs Function Add Auto Execute Functions.<br>
+v0.3.1 24/05/18 08:41: Inputs Function Add Callable Function.<br>
 v0.3 24/05/16 20:29: Update CMD Functions,Add Variable Supports,Add E_Type.<br>
 v0.2.1 24/05/12 15:45: Add CMD Functions.<br>
 v0.2 24/05/12 15:31: Removed Colorama Require.<br>
 v0.1 24/05/11: Initial Update.
```

### Comparing `shellper-0.3.1/Shellper.egg-info/PKG-INFO` & `shellper-0.3.2/Shellper.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Shellper
-Version: 0.3.1
+Version: 0.3.2
 Summary: A Python Library for create shell apps.
 Home-page: https://gitee.com/ShawnMerry/Shellper
 Author: ShawnMerry
 Author-email: merrybili@163.com
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
@@ -23,12 +23,13 @@
 
 #### [PyPI](https://pypi.org/project/Shellper)
 
 #### [Gitee](https://gitee.com/ShawnMerry/Shellper)
 
 ### Update Log:<br>
 
-v0.3.1 24/05/18 08:41: Inputs Function Add Callable Function.
+v0.3.2 24/05/18 09:40: Inputs Function Add Auto Execute Functions.<br>
+v0.3.1 24/05/18 08:41: Inputs Function Add Callable Function.<br>
 v0.3 24/05/16 20:29: Update CMD Functions,Add Variable Supports,Add E_Type.<br>
 v0.2.1 24/05/12 15:45: Add CMD Functions.<br>
 v0.2 24/05/12 15:31: Removed Colorama Require.<br>
 v0.1 24/05/11: Initial Update.
```

### Comparing `shellper-0.3.1/setup.py` & `shellper-0.3.2/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="Shellper",
-    version="0.3.1",
+    version="0.3.2",
     author="ShawnMerry",
     author_email="merrybili@163.com",
     description="A Python Library for create shell apps.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://gitee.com/ShawnMerry/Shellper",
     packages=find_packages(),
```

### Comparing `shellper-0.3.1/shellper/log.py` & `shellper-0.3.2/shellper/log.py`

 * *Files identical despite different names*

### Comparing `shellper-0.3.1/shellper/style.py` & `shellper-0.3.2/shellper/style.py`

 * *Files identical despite different names*

