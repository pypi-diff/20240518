# Comparing `tmp/way3-0.0.27.tar.gz` & `tmp/way3-0.0.28.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "way3-0.0.27.tar", last modified: Sat May 18 09:37:03 2024, max compression
+gzip compressed data, was "way3-0.0.28.tar", last modified: Sat May 18 09:39:58 2024, max compression
```

## Comparing `way3-0.0.27.tar` & `way3-0.0.28.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 09:37:03.036747 way3-0.0.27/
--rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-05-18 09:36:54.000000 way3-0.0.27/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3977 2024-05-18 09:37:03.036747 way3-0.0.27/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3548 2024-05-18 09:36:54.000000 way3-0.0.27/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-18 09:37:03.036747 way3-0.0.27/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      638 2024-05-18 09:36:54.000000 way3-0.0.27/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 09:37:03.032747 way3-0.0.27/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-18 09:36:54.000000 way3-0.0.27/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2020 2024-05-18 09:36:54.000000 way3-0.0.27/tests/test_file_find.py
--rw-r--r--   0 runner    (1001) docker     (127)      839 2024-05-18 09:36:54.000000 way3-0.0.27/tests/test_file_op.py
--rw-r--r--   0 runner    (1001) docker     (127)     1547 2024-05-18 09:36:54.000000 way3-0.0.27/tests/test_folder_op.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 09:37:03.032747 way3-0.0.27/way3/
--rw-r--r--   0 runner    (1001) docker     (127)     1322 2024-05-18 09:36:54.000000 way3-0.0.27/way3/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 09:37:03.036747 way3-0.0.27/way3/file_find/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-18 09:36:54.000000 way3-0.0.27/way3/file_find/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      106 2024-05-18 09:36:54.000000 way3-0.0.27/way3/file_find/current_dir.py
--rw-r--r--   0 runner    (1001) docker     (127)     2120 2024-05-18 09:36:54.000000 way3-0.0.27/way3/file_find/traverse_files_from_folder.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 09:37:03.036747 way3-0.0.27/way3/file_op/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-18 09:36:54.000000 way3-0.0.27/way3/file_op/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1735 2024-05-18 09:36:54.000000 way3-0.0.27/way3/file_op/create_file.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 09:37:03.036747 way3-0.0.27/way3/folder_op/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-18 09:36:54.000000 way3-0.0.27/way3/folder_op/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2681 2024-05-18 09:36:54.000000 way3-0.0.27/way3/folder_op/create_folder.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 09:37:03.036747 way3-0.0.27/way3.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3977 2024-05-18 09:37:03.000000 way3-0.0.27/way3.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      457 2024-05-18 09:37:03.000000 way3-0.0.27/way3.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-18 09:37:03.000000 way3-0.0.27/way3.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-18 09:37:03.000000 way3-0.0.27/way3.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 09:39:58.679025 way3-0.0.28/
+-rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-05-18 09:39:53.000000 way3-0.0.28/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4888 2024-05-18 09:39:58.679025 way3-0.0.28/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4459 2024-05-18 09:39:53.000000 way3-0.0.28/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-18 09:39:58.679025 way3-0.0.28/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      638 2024-05-18 09:39:53.000000 way3-0.0.28/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 09:39:58.675025 way3-0.0.28/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-18 09:39:53.000000 way3-0.0.28/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2020 2024-05-18 09:39:53.000000 way3-0.0.28/tests/test_file_find.py
+-rw-r--r--   0 runner    (1001) docker     (127)      839 2024-05-18 09:39:53.000000 way3-0.0.28/tests/test_file_op.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1547 2024-05-18 09:39:53.000000 way3-0.0.28/tests/test_folder_op.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 09:39:58.675025 way3-0.0.28/way3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1322 2024-05-18 09:39:53.000000 way3-0.0.28/way3/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 09:39:58.675025 way3-0.0.28/way3/file_find/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-18 09:39:53.000000 way3-0.0.28/way3/file_find/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-05-18 09:39:53.000000 way3-0.0.28/way3/file_find/current_dir.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2120 2024-05-18 09:39:53.000000 way3-0.0.28/way3/file_find/traverse_files_from_folder.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 09:39:58.675025 way3-0.0.28/way3/file_op/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-18 09:39:53.000000 way3-0.0.28/way3/file_op/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1735 2024-05-18 09:39:53.000000 way3-0.0.28/way3/file_op/create_file.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 09:39:58.679025 way3-0.0.28/way3/folder_op/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-18 09:39:53.000000 way3-0.0.28/way3/folder_op/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2681 2024-05-18 09:39:53.000000 way3-0.0.28/way3/folder_op/create_folder.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 09:39:58.679025 way3-0.0.28/way3.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4888 2024-05-18 09:39:58.000000 way3-0.0.28/way3.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      457 2024-05-18 09:39:58.000000 way3-0.0.28/way3.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-18 09:39:58.000000 way3-0.0.28/way3.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-18 09:39:58.000000 way3-0.0.28/way3.egg-info/top_level.txt
```

### Comparing `way3-0.0.27/LICENSE` & `way3-0.0.28/LICENSE`

 * *Files identical despite different names*

### Comparing `way3-0.0.27/PKG-INFO` & `way3-0.0.28/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,20 +1,7 @@
-Metadata-Version: 2.1
-Name: way3
-Version: 0.0.27
-Summary: Simplified file path management for Python developers
-Home-page: https://github.com/aboutmydreams/way3
-Author: aboutmydreams
-Author-email: aboutmydreams@163.com
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # Way3: A Python Module for File Operations
 
 [![Auto CI and Build Tools](https://github.com/aboutmydreams/way3/actions/workflows/ci-test.yml/badge.svg)](https://github.com/aboutmydreams/way3/actions/workflows/ci-test.yml)
 [![Auto Publish to PyPI and GitHub Release](https://github.com/aboutmydreams/way3/actions/workflows/release.yml/badge.svg)](https://github.com/aboutmydreams/way3/actions/workflows/release.yml)
 [![label](https://img.shields.io/badge/%E4%B8%AD%E6%96%87%E6%96%87%E6%A1%A3-ZH-brightgreen)](https://github.com/aboutmydreams/way3/blob/main/README_ZH.md)
 [![label](https://img.shields.io/badge/English-EN-brightgreen)](https://github.com/aboutmydreams/way3/blob/main/README.md)
 [![Release Version](https://img.shields.io/github/release/aboutmydreams/way3.svg)](https://github.com/aboutmydreams/way3/releases)
@@ -87,20 +74,61 @@
 ```python
 import way3
 
 result = way3.get_current_dir()
 print(result)  # prints the current working directory
 ```
 
+### create_directory(directory_name: str, directory_path: Union[str, os.PathLike] = ".") -> str
+
+Creates a new directory with the given name.
+
+Example:
+
+```python
+import way3
+
+result = way3.create_directory("my_directory")
+print(result)  # prints the absolute path of the created directory
+```
+
+### rename_directory(original_name: str, new_name: str) -> str
+
+Renames a directory with a new name.
+
+Example:
+
+```python
+import way3
+
+result = way3.rename_directory("old_directory", "new_directory")
+print(result)  # prints the absolute path of the renamed directory
+```
+
+### delete_directory(directory_name: str, directory_path: Union[str, os.PathLike] = ".") -> str
+
+Deletes a directory and all its contents.
+
+Example:
+
+```python
+import way3
+
+result = way3.delete_directory("my_directory")
+print(result)  # prints the absolute path of the deleted directory
+```
+
+Let me know if you need any further modifications!
+
 ## Testing
 
 To run the tests, you can use the following command:
 
 ```bash
 python3 -m unittest discover -s tests
 ```
 
 ## License
 
 Way3 is released under the MIT License. See [LICENSE](LICENSE) for details.
 
-I hope you find Way3 useful! If you have any questions or feedback, please open an issue or pull request.
+I hope you find Way3 useful! If you have any questions or feedback, please open an issue or pull request.
```

### Comparing `way3-0.0.27/setup.py` & `way3-0.0.28/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="way3",
-    version="0.0.27",
+    version="0.0.28",
     author="aboutmydreams",
     author_email="aboutmydreams@163.com",
     description="Simplified file path management for Python developers",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/aboutmydreams/way3",
     packages=setuptools.find_packages(),
```

### Comparing `way3-0.0.27/tests/test_file_find.py` & `way3-0.0.28/tests/test_file_find.py`

 * *Files identical despite different names*

### Comparing `way3-0.0.27/tests/test_file_op.py` & `way3-0.0.28/tests/test_file_op.py`

 * *Files identical despite different names*

### Comparing `way3-0.0.27/tests/test_folder_op.py` & `way3-0.0.28/tests/test_folder_op.py`

 * *Files identical despite different names*

### Comparing `way3-0.0.27/way3/__init__.py` & `way3-0.0.28/way3/__init__.py`

 * *Files identical despite different names*

### Comparing `way3-0.0.27/way3/file_find/traverse_files_from_folder.py` & `way3-0.0.28/way3/file_find/traverse_files_from_folder.py`

 * *Files identical despite different names*

### Comparing `way3-0.0.27/way3/file_op/create_file.py` & `way3-0.0.28/way3/file_op/create_file.py`

 * *Files identical despite different names*

### Comparing `way3-0.0.27/way3/folder_op/create_folder.py` & `way3-0.0.28/way3/folder_op/create_folder.py`

 * *Files identical despite different names*

### Comparing `way3-0.0.27/way3.egg-info/PKG-INFO` & `way3-0.0.28/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: way3
-Version: 0.0.27
+Version: 0.0.28
 Summary: Simplified file path management for Python developers
 Home-page: https://github.com/aboutmydreams/way3
 Author: aboutmydreams
 Author-email: aboutmydreams@163.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -87,14 +87,55 @@
 ```python
 import way3
 
 result = way3.get_current_dir()
 print(result)  # prints the current working directory
 ```
 
+### create_directory(directory_name: str, directory_path: Union[str, os.PathLike] = ".") -> str
+
+Creates a new directory with the given name.
+
+Example:
+
+```python
+import way3
+
+result = way3.create_directory("my_directory")
+print(result)  # prints the absolute path of the created directory
+```
+
+### rename_directory(original_name: str, new_name: str) -> str
+
+Renames a directory with a new name.
+
+Example:
+
+```python
+import way3
+
+result = way3.rename_directory("old_directory", "new_directory")
+print(result)  # prints the absolute path of the renamed directory
+```
+
+### delete_directory(directory_name: str, directory_path: Union[str, os.PathLike] = ".") -> str
+
+Deletes a directory and all its contents.
+
+Example:
+
+```python
+import way3
+
+result = way3.delete_directory("my_directory")
+print(result)  # prints the absolute path of the deleted directory
+```
+
+Let me know if you need any further modifications!
+
 ## Testing
 
 To run the tests, you can use the following command:
 
 ```bash
 python3 -m unittest discover -s tests
 ```
```

