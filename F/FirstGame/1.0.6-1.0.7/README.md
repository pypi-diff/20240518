# Comparing `tmp/FirstGame-1.0.6.tar.gz` & `tmp/FirstGame-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FirstGame-1.0.6.tar", last modified: Sat May 18 03:08:56 2024, max compression
+gzip compressed data, was "FirstGame-1.0.7.tar", last modified: Sat May 18 03:19:41 2024, max compression
```

## Comparing `FirstGame-1.0.6.tar` & `FirstGame-1.0.7.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2024-05-18 03:08:56.116716 FirstGame-1.0.6/
-drwxrwxrwx   0        0        0        0 2024-05-18 03:08:56.106823 FirstGame-1.0.6/FirstGame/
--rw-rw-rw-   0        0        0        0 2024-05-17 13:32:12.000000 FirstGame-1.0.6/FirstGame/__init__.py
--rw-rw-rw-   0        0        0     4732 2024-05-17 16:32:26.000000 FirstGame-1.0.6/FirstGame/get_data.py
-drwxrwxrwx   0        0        0        0 2024-05-18 03:08:56.114376 FirstGame-1.0.6/FirstGame/get_data_dir/
--rw-rw-rw-   0        0        0        0 2024-05-17 08:58:48.000000 FirstGame-1.0.6/FirstGame/get_data_dir/__init__.py
--rw-rw-rw-   0        0        0     4732 2024-05-17 07:23:56.000000 FirstGame-1.0.6/FirstGame/get_data_dir/get_data.py
--rw-rw-rw-   0        0        0      935 2024-05-16 15:29:11.000000 FirstGame-1.0.6/FirstGame/list_mysql.py
--rw-rw-rw-   0        0        0    48595 2024-05-18 03:07:04.000000 FirstGame-1.0.6/FirstGame/main.py
--rw-rw-rw-   0        0        0     3033 2024-05-16 15:30:39.000000 FirstGame-1.0.6/FirstGame/test_mysql.py
-drwxrwxrwx   0        0        0        0 2024-05-18 03:08:56.112469 FirstGame-1.0.6/FirstGame.egg-info/
--rw-rw-rw-   0        0        0      538 2024-05-18 03:08:56.000000 FirstGame-1.0.6/FirstGame.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      452 2024-05-18 03:08:56.000000 FirstGame-1.0.6/FirstGame.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-18 03:08:56.000000 FirstGame-1.0.6/FirstGame.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       50 2024-05-18 03:08:56.000000 FirstGame-1.0.6/FirstGame.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2024-05-18 03:08:56.000000 FirstGame-1.0.6/FirstGame.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       58 2024-05-18 03:08:56.000000 FirstGame-1.0.6/FirstGame.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-05-18 03:08:56.000000 FirstGame-1.0.6/FirstGame.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1088 2024-05-17 13:43:05.000000 FirstGame-1.0.6/LICENSE.txt
--rw-rw-rw-   0        0        0      538 2024-05-18 03:08:56.116716 FirstGame-1.0.6/PKG-INFO
--rw-rw-rw-   0        0        0      136 2024-05-17 13:59:41.000000 FirstGame-1.0.6/README.md
--rw-rw-rw-   0        0        0       86 2024-05-18 03:08:56.118038 FirstGame-1.0.6/setup.cfg
--rw-rw-rw-   0        0        0     1304 2024-05-18 03:08:43.000000 FirstGame-1.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-18 03:19:41.084742 FirstGame-1.0.7/
+drwxrwxrwx   0        0        0        0 2024-05-18 03:19:41.076735 FirstGame-1.0.7/FirstGame/
+-rw-rw-rw-   0        0        0        0 2024-05-17 13:32:12.000000 FirstGame-1.0.7/FirstGame/__init__.py
+-rw-rw-rw-   0        0        0     4732 2024-05-17 16:32:26.000000 FirstGame-1.0.7/FirstGame/get_data.py
+drwxrwxrwx   0        0        0        0 2024-05-18 03:19:41.084742 FirstGame-1.0.7/FirstGame/get_data_dir/
+-rw-rw-rw-   0        0        0        0 2024-05-17 08:58:48.000000 FirstGame-1.0.7/FirstGame/get_data_dir/__init__.py
+-rw-rw-rw-   0        0        0     4732 2024-05-17 07:23:56.000000 FirstGame-1.0.7/FirstGame/get_data_dir/get_data.py
+-rw-rw-rw-   0        0        0      935 2024-05-16 15:29:11.000000 FirstGame-1.0.7/FirstGame/list_mysql.py
+-rw-rw-rw-   0        0        0    48595 2024-05-18 03:07:04.000000 FirstGame-1.0.7/FirstGame/main.py
+-rw-rw-rw-   0        0        0     3033 2024-05-16 15:30:39.000000 FirstGame-1.0.7/FirstGame/test_mysql.py
+drwxrwxrwx   0        0        0        0 2024-05-18 03:19:41.084742 FirstGame-1.0.7/FirstGame.egg-info/
+-rw-rw-rw-   0        0        0      400 2024-05-18 03:19:40.000000 FirstGame-1.0.7/FirstGame.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      452 2024-05-18 03:19:41.000000 FirstGame-1.0.7/FirstGame.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-18 03:19:40.000000 FirstGame-1.0.7/FirstGame.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       50 2024-05-18 03:19:41.000000 FirstGame-1.0.7/FirstGame.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2024-05-18 03:19:40.000000 FirstGame-1.0.7/FirstGame.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       58 2024-05-18 03:19:41.000000 FirstGame-1.0.7/FirstGame.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-05-18 03:19:41.000000 FirstGame-1.0.7/FirstGame.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1088 2024-05-17 13:43:05.000000 FirstGame-1.0.7/LICENSE.txt
+-rw-rw-rw-   0        0        0      400 2024-05-18 03:19:41.084742 FirstGame-1.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0      136 2024-05-17 13:59:41.000000 FirstGame-1.0.7/README.md
+-rw-rw-rw-   0        0        0       86 2024-05-18 03:19:41.084742 FirstGame-1.0.7/setup.cfg
+-rw-rw-rw-   0        0        0     1171 2024-05-18 03:19:35.000000 FirstGame-1.0.7/setup.py
```

### Comparing `FirstGame-1.0.6/FirstGame/get_data.py` & `FirstGame-1.0.7/FirstGame/get_data.py`

 * *Files identical despite different names*

### Comparing `FirstGame-1.0.6/FirstGame/get_data_dir/get_data.py` & `FirstGame-1.0.7/FirstGame/get_data_dir/get_data.py`

 * *Files identical despite different names*

### Comparing `FirstGame-1.0.6/FirstGame/list_mysql.py` & `FirstGame-1.0.7/FirstGame/list_mysql.py`

 * *Files identical despite different names*

### Comparing `FirstGame-1.0.6/FirstGame/main.py` & `FirstGame-1.0.7/FirstGame/main.py`

 * *Files identical despite different names*

### Comparing `FirstGame-1.0.6/FirstGame/test_mysql.py` & `FirstGame-1.0.7/FirstGame/test_mysql.py`

 * *Files identical despite different names*

### Comparing `FirstGame-1.0.6/LICENSE.txt` & `FirstGame-1.0.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `FirstGame-1.0.6/setup.py` & `FirstGame-1.0.7/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,34 +1,30 @@
 from setuptools import setup, find_packages
 import os
 
-with open("README.md", "r", encoding='utf-8') as f:
-    long_description = f.read()
-
 # 列出資源文件，如圖片、音頻等
 def package_files(directory):
     paths = []
     for (path, directories, filenames) in os.walk(directory):
         for filename in filenames:
             paths.append(os.path.join(path, filename))
     return paths
 
 
 extra_files = package_files('FirstGame/resources')
 
 
 setup(
     name='FirstGame',
-    version='1.0.6',
+    version='1.0.7',
     author="spx220",
     author_email="eric2173459@gmail.com",
-    long_description=long_description,
     long_description_content_type = 'text/markdown',
     packages=find_packages(),
-    package_data={'': extra_files},
+    include_package_data=True,
     license='MIT',
     zip_safe=False,
     keywords=['spx', 'kpop', 'anime', 'FirstGame'],
     install_requires=[
         'pygame==2.5.2',
         'pymysql==1.1.0',
         'pillow==10.2.0',
```

