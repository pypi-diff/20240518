# Comparing `tmp/shellper-0.3.2.tar.gz` & `tmp/shellper-0.3.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shellper-0.3.2.tar", last modified: Sat May 18 01:40:38 2024, max compression
+gzip compressed data, was "shellper-0.3.2.1.tar", last modified: Sat May 18 01:49:44 2024, max compression
```

## Comparing `shellper-0.3.2.tar` & `shellper-0.3.2.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2024-05-18 01:40:38.833476 shellper-0.3.2/
--rw-rw-rw-   0        0        0    11357 2024-04-29 10:47:19.000000 shellper-0.3.2/LICENSE.txt
--rw-rw-rw-   0        0        0     1197 2024-05-18 01:40:38.832476 shellper-0.3.2/PKG-INFO
--rw-rw-rw-   0        0        0      576 2024-05-18 01:39:49.000000 shellper-0.3.2/README.md
-drwxrwxrwx   0        0        0        0 2024-05-18 01:40:38.830477 shellper-0.3.2/Shellper.egg-info/
--rw-rw-rw-   0        0        0     1197 2024-05-18 01:40:38.000000 shellper-0.3.2/Shellper.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      250 2024-05-18 01:40:38.000000 shellper-0.3.2/Shellper.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-18 01:40:38.000000 shellper-0.3.2/Shellper.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2024-05-18 01:40:38.000000 shellper-0.3.2/Shellper.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-18 01:40:38.834476 shellper-0.3.2/setup.cfg
--rw-rw-rw-   0        0        0      837 2024-05-18 01:39:49.000000 shellper-0.3.2/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-18 01:40:38.828477 shellper-0.3.2/shellper/
--rw-rw-rw-   0        0        0      376 2024-05-16 12:12:42.000000 shellper-0.3.2/shellper/__init__.py
--rw-rw-rw-   0        0        0      378 2024-05-16 12:17:03.000000 shellper-0.3.2/shellper/datas.py
--rw-rw-rw-   0        0        0     1328 2024-05-18 01:37:06.000000 shellper-0.3.2/shellper/inputs.py
--rw-rw-rw-   0        0        0     2639 2024-05-16 12:01:09.000000 shellper-0.3.2/shellper/log.py
--rw-rw-rw-   0        0        0      735 2024-05-12 07:22:51.000000 shellper-0.3.2/shellper/style.py
+drwxrwxrwx   0        0        0        0 2024-05-18 01:49:44.542623 shellper-0.3.2.1/
+-rw-rw-rw-   0        0        0    11357 2024-04-29 10:47:19.000000 shellper-0.3.2.1/LICENSE.txt
+-rw-rw-rw-   0        0        0     1268 2024-05-18 01:49:44.540624 shellper-0.3.2.1/PKG-INFO
+-rw-rw-rw-   0        0        0      645 2024-05-18 01:48:49.000000 shellper-0.3.2.1/README.md
+drwxrwxrwx   0        0        0        0 2024-05-18 01:49:44.538621 shellper-0.3.2.1/Shellper.egg-info/
+-rw-rw-rw-   0        0        0     1268 2024-05-18 01:49:44.000000 shellper-0.3.2.1/Shellper.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      250 2024-05-18 01:49:44.000000 shellper-0.3.2.1/Shellper.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-18 01:49:44.000000 shellper-0.3.2.1/Shellper.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2024-05-18 01:49:44.000000 shellper-0.3.2.1/Shellper.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-18 01:49:44.542623 shellper-0.3.2.1/setup.cfg
+-rw-rw-rw-   0        0        0      839 2024-05-18 01:48:49.000000 shellper-0.3.2.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-18 01:49:44.537620 shellper-0.3.2.1/shellper/
+-rw-rw-rw-   0        0        0      376 2024-05-16 12:12:42.000000 shellper-0.3.2.1/shellper/__init__.py
+-rw-rw-rw-   0        0        0      378 2024-05-16 12:17:03.000000 shellper-0.3.2.1/shellper/datas.py
+-rw-rw-rw-   0        0        0     1291 2024-05-18 01:45:55.000000 shellper-0.3.2.1/shellper/inputs.py
+-rw-rw-rw-   0        0        0     2639 2024-05-16 12:01:09.000000 shellper-0.3.2.1/shellper/log.py
+-rw-rw-rw-   0        0        0      735 2024-05-12 07:22:51.000000 shellper-0.3.2.1/shellper/style.py
```

### Comparing `shellper-0.3.2/LICENSE.txt` & `shellper-0.3.2.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `shellper-0.3.2/PKG-INFO` & `shellper-0.3.2.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Shellper
-Version: 0.3.2
+Version: 0.3.2.1
 Summary: A Python Library for create shell apps.
 Home-page: https://gitee.com/ShawnMerry/Shellper
 Author: ShawnMerry
 Author-email: merrybili@163.com
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
@@ -23,13 +23,14 @@
 
 #### [PyPI](https://pypi.org/project/Shellper)
 
 #### [Gitee](https://gitee.com/ShawnMerry/Shellper)
 
 ### Update Log:<br>
 
+v0.3.2.1(v0.3.2-hotfix) 24/05/18 09:49: Fix last version's bug.<br>
 v0.3.2 24/05/18 09:40: Inputs Function Add Auto Execute Functions.<br>
 v0.3.1 24/05/18 08:41: Inputs Function Add Callable Function.<br>
 v0.3 24/05/16 20:29: Update CMD Functions,Add Variable Supports,Add E_Type.<br>
 v0.2.1 24/05/12 15:45: Add CMD Functions.<br>
 v0.2 24/05/12 15:31: Removed Colorama Require.<br>
 v0.1 24/05/11: Initial Update.
```

### Comparing `shellper-0.3.2/README.md` & `shellper-0.3.2.1/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -5,13 +5,14 @@
 
 #### [PyPI](https://pypi.org/project/Shellper)
 
 #### [Gitee](https://gitee.com/ShawnMerry/Shellper)
 
 ### Update Log:<br>
 
+v0.3.2.1(v0.3.2-hotfix) 24/05/18 09:49: Fix last version's bug.<br>
 v0.3.2 24/05/18 09:40: Inputs Function Add Auto Execute Functions.<br>
 v0.3.1 24/05/18 08:41: Inputs Function Add Callable Function.<br>
 v0.3 24/05/16 20:29: Update CMD Functions,Add Variable Supports,Add E_Type.<br>
 v0.2.1 24/05/12 15:45: Add CMD Functions.<br>
 v0.2 24/05/12 15:31: Removed Colorama Require.<br>
 v0.1 24/05/11: Initial Update.
```

### Comparing `shellper-0.3.2/Shellper.egg-info/PKG-INFO` & `shellper-0.3.2.1/Shellper.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Shellper
-Version: 0.3.2
+Version: 0.3.2.1
 Summary: A Python Library for create shell apps.
 Home-page: https://gitee.com/ShawnMerry/Shellper
 Author: ShawnMerry
 Author-email: merrybili@163.com
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
@@ -23,13 +23,14 @@
 
 #### [PyPI](https://pypi.org/project/Shellper)
 
 #### [Gitee](https://gitee.com/ShawnMerry/Shellper)
 
 ### Update Log:<br>
 
+v0.3.2.1(v0.3.2-hotfix) 24/05/18 09:49: Fix last version's bug.<br>
 v0.3.2 24/05/18 09:40: Inputs Function Add Auto Execute Functions.<br>
 v0.3.1 24/05/18 08:41: Inputs Function Add Callable Function.<br>
 v0.3 24/05/16 20:29: Update CMD Functions,Add Variable Supports,Add E_Type.<br>
 v0.2.1 24/05/12 15:45: Add CMD Functions.<br>
 v0.2 24/05/12 15:31: Removed Colorama Require.<br>
 v0.1 24/05/11: Initial Update.
```

### Comparing `shellper-0.3.2/setup.py` & `shellper-0.3.2.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="Shellper",
-    version="0.3.2",
+    version="0.3.2.1",
     author="ShawnMerry",
     author_email="merrybili@163.com",
     description="A Python Library for create shell apps.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://gitee.com/ShawnMerry/Shellper",
     packages=find_packages(),
```

### Comparing `shellper-0.3.2/shellper/inputs.py` & `shellper-0.3.2.1/shellper/inputs.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,15 +23,14 @@
     elif func is not None:
         func(text.split(spilt_text))
     elif func_word is not None:
         text = text.split(spilt_text)
         command = text[0]
         for i in func_word:
             if command == i:
-                print(func_word[i])
                 command = func_word[i]
                 command(text[1:])
                 return True
             else:
                 error("System", f"The command '{command}' is not valid", e_type="Function Undefined")
                 return False
     else:
```

### Comparing `shellper-0.3.2/shellper/log.py` & `shellper-0.3.2.1/shellper/log.py`

 * *Files identical despite different names*

### Comparing `shellper-0.3.2/shellper/style.py` & `shellper-0.3.2.1/shellper/style.py`

 * *Files identical despite different names*

