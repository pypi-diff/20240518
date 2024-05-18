# Comparing `tmp/shellper-0.3.tar.gz` & `tmp/shellper-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shellper-0.3.tar", last modified: Thu May 16 12:28:57 2024, max compression
+gzip compressed data, was "shellper-0.3.1.tar", last modified: Sat May 18 00:41:47 2024, max compression
```

## Comparing `shellper-0.3.tar` & `shellper-0.3.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2024-05-16 12:28:57.439381 shellper-0.3/
--rw-rw-rw-   0        0        0    11357 2024-04-29 10:47:19.000000 shellper-0.3/LICENSE.txt
--rw-rw-rw-   0        0        0     1055 2024-05-16 12:28:57.431782 shellper-0.3/PKG-INFO
--rw-rw-rw-   0        0        0      438 2024-05-16 12:28:36.000000 shellper-0.3/README.md
-drwxrwxrwx   0        0        0        0 2024-05-16 12:28:57.431782 shellper-0.3/Shellper.egg-info/
--rw-rw-rw-   0        0        0     1055 2024-05-16 12:28:57.000000 shellper-0.3/Shellper.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      250 2024-05-16 12:28:57.000000 shellper-0.3/Shellper.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-16 12:28:57.000000 shellper-0.3/Shellper.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2024-05-16 12:28:57.000000 shellper-0.3/Shellper.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-16 12:28:57.439381 shellper-0.3/setup.cfg
--rw-rw-rw-   0        0        0      833 2024-05-16 12:28:36.000000 shellper-0.3/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-16 12:28:57.421862 shellper-0.3/shellper/
--rw-rw-rw-   0        0        0      376 2024-05-16 12:12:42.000000 shellper-0.3/shellper/__init__.py
--rw-rw-rw-   0        0        0      378 2024-05-16 12:17:03.000000 shellper-0.3/shellper/datas.py
--rw-rw-rw-   0        0        0      723 2024-05-16 12:01:56.000000 shellper-0.3/shellper/inputs.py
--rw-rw-rw-   0        0        0     2639 2024-05-16 12:01:09.000000 shellper-0.3/shellper/log.py
--rw-rw-rw-   0        0        0      735 2024-05-12 07:22:51.000000 shellper-0.3/shellper/style.py
+drwxrwxrwx   0        0        0        0 2024-05-18 00:41:47.450153 shellper-0.3.1/
+-rw-rw-rw-   0        0        0    11357 2024-04-29 10:47:19.000000 shellper-0.3.1/LICENSE.txt
+-rw-rw-rw-   0        0        0     1121 2024-05-18 00:41:47.450153 shellper-0.3.1/PKG-INFO
+-rw-rw-rw-   0        0        0      500 2024-05-18 00:40:22.000000 shellper-0.3.1/README.md
+drwxrwxrwx   0        0        0        0 2024-05-18 00:41:47.450153 shellper-0.3.1/Shellper.egg-info/
+-rw-rw-rw-   0        0        0     1121 2024-05-18 00:41:47.000000 shellper-0.3.1/Shellper.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      250 2024-05-18 00:41:47.000000 shellper-0.3.1/Shellper.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-18 00:41:47.000000 shellper-0.3.1/Shellper.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2024-05-18 00:41:47.000000 shellper-0.3.1/Shellper.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-18 00:41:47.450153 shellper-0.3.1/setup.cfg
+-rw-rw-rw-   0        0        0      837 2024-05-18 00:40:22.000000 shellper-0.3.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-18 00:41:47.450153 shellper-0.3.1/shellper/
+-rw-rw-rw-   0        0        0      376 2024-05-16 12:12:42.000000 shellper-0.3.1/shellper/__init__.py
+-rw-rw-rw-   0        0        0      378 2024-05-16 12:17:03.000000 shellper-0.3.1/shellper/datas.py
+-rw-rw-rw-   0        0        0      853 2024-05-18 00:38:06.000000 shellper-0.3.1/shellper/inputs.py
+-rw-rw-rw-   0        0        0     2639 2024-05-16 12:01:09.000000 shellper-0.3.1/shellper/log.py
+-rw-rw-rw-   0        0        0      735 2024-05-12 07:22:51.000000 shellper-0.3.1/shellper/style.py
```

### Comparing `shellper-0.3/LICENSE.txt` & `shellper-0.3.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `shellper-0.3/PKG-INFO` & `shellper-0.3.1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,33 +1,34 @@
 Metadata-Version: 2.1
 Name: Shellper
-Version: 0.3
+Version: 0.3.1
 Summary: A Python Library for create shell apps.
 Home-page: https://gitee.com/ShawnMerry/Shellper
 Author: ShawnMerry
 Author-email: merrybili@163.com
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Internet
-Requires-Python: >=3
+Requires-Python: >=3.5
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # Shellper
 
 A Python Library about shells.
-<br>It can help you create the better shell apps..
+<br>It can help you create the better shell apps.
 
 #### [PyPI](https://pypi.org/project/Shellper)
 
 #### [Gitee](https://gitee.com/ShawnMerry/Shellper)
 
 ### Update Log:<br>
 
+v0.3.1 24/05/18 08:41: Inputs Function Add Callable Function.
 v0.3 24/05/16 20:29: Update CMD Functions,Add Variable Supports,Add E_Type.<br>
 v0.2.1 24/05/12 15:45: Add CMD Functions.<br>
 v0.2 24/05/12 15:31: Removed Colorama Require.<br>
 v0.1 24/05/11: Initial Update.
```

### Comparing `shellper-0.3/Shellper.egg-info/PKG-INFO` & `shellper-0.3.1/Shellper.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,33 +1,34 @@
 Metadata-Version: 2.1
 Name: Shellper
-Version: 0.3
+Version: 0.3.1
 Summary: A Python Library for create shell apps.
 Home-page: https://gitee.com/ShawnMerry/Shellper
 Author: ShawnMerry
 Author-email: merrybili@163.com
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Internet
-Requires-Python: >=3
+Requires-Python: >=3.5
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # Shellper
 
 A Python Library about shells.
-<br>It can help you create the better shell apps..
+<br>It can help you create the better shell apps.
 
 #### [PyPI](https://pypi.org/project/Shellper)
 
 #### [Gitee](https://gitee.com/ShawnMerry/Shellper)
 
 ### Update Log:<br>
 
+v0.3.1 24/05/18 08:41: Inputs Function Add Callable Function.
 v0.3 24/05/16 20:29: Update CMD Functions,Add Variable Supports,Add E_Type.<br>
 v0.2.1 24/05/12 15:45: Add CMD Functions.<br>
 v0.2 24/05/12 15:31: Removed Colorama Require.<br>
 v0.1 24/05/11: Initial Update.
```

### Comparing `shellper-0.3/setup.py` & `shellper-0.3.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="Shellper",
-    version="0.3",
+    version="0.3.1",
     author="ShawnMerry",
     author_email="merrybili@163.com",
     description="A Python Library for create shell apps.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://gitee.com/ShawnMerry/Shellper",
     packages=find_packages(),
@@ -18,9 +18,9 @@
         "Environment :: Console",
         "Intended Audience :: Developers",
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: OS Independent",
         "Topic :: Internet"
     ],
-    python_requires=">=3"
+    python_requires=">=3.5"
 )
```

### Comparing `shellper-0.3/shellper/inputs.py` & `shellper-0.3.1/shellper/inputs.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,22 +1,26 @@
 from .log import *
 from .style import *
 from os import system as cmd
+from typing import Callable
 
 
-def inputs(word=Style.BRIGHT + ">>> " + Style.NORMAL, spilt_text=None, end_symbol: str = None, is_cmd: bool = False):
+def inputs(word=Style.BRIGHT + ">>> " + Style.NORMAL, spilt_text=None, func: Callable = None,
+           end_symbol: str = None, is_cmd: bool = False):
     try:
         word = str(word)
     except TypeError:
         raise ConvertError("Name or message must can convert to string")
     text = input(word)
     if end_symbol is not None:
         if text[-1] == end_symbol:
             text = text[:-1]
         else:
             error("System", f"The last character of your command must be '{end_symbol}'.{Style.RESET}",
                   e_type="Symbol Error")
             return False
     if is_cmd:
         cmd(text)
+    elif func is not None:
+        func(text.split(spilt_text))
     else:
         return text.split(spilt_text)
```

### Comparing `shellper-0.3/shellper/log.py` & `shellper-0.3.1/shellper/log.py`

 * *Files identical despite different names*

### Comparing `shellper-0.3/shellper/style.py` & `shellper-0.3.1/shellper/style.py`

 * *Files identical despite different names*

