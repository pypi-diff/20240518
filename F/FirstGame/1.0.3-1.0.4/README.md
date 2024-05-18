# Comparing `tmp/FirstGame-1.0.3.tar.gz` & `tmp/FirstGame-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FirstGame-1.0.3.tar", last modified: Sat May 18 02:46:05 2024, max compression
+gzip compressed data, was "FirstGame-1.0.4.tar", last modified: Sat May 18 02:54:25 2024, max compression
```

## Comparing `FirstGame-1.0.3.tar` & `FirstGame-1.0.4.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2024-05-18 02:46:05.269590 FirstGame-1.0.3/
-drwxrwxrwx   0        0        0        0 2024-05-18 02:46:05.253595 FirstGame-1.0.3/FirstGame/
--rw-rw-rw-   0        0        0        0 2024-05-17 13:32:12.000000 FirstGame-1.0.3/FirstGame/__init__.py
--rw-rw-rw-   0        0        0     4732 2024-05-17 16:32:26.000000 FirstGame-1.0.3/FirstGame/get_data.py
-drwxrwxrwx   0        0        0        0 2024-05-18 02:46:05.269590 FirstGame-1.0.3/FirstGame/get_data_dir/
--rw-rw-rw-   0        0        0        0 2024-05-17 08:58:48.000000 FirstGame-1.0.3/FirstGame/get_data_dir/__init__.py
--rw-rw-rw-   0        0        0     4732 2024-05-17 07:23:56.000000 FirstGame-1.0.3/FirstGame/get_data_dir/get_data.py
--rw-rw-rw-   0        0        0      935 2024-05-16 15:29:11.000000 FirstGame-1.0.3/FirstGame/list_mysql.py
--rw-rw-rw-   0        0        0    44141 2024-05-18 02:45:45.000000 FirstGame-1.0.3/FirstGame/main.py
--rw-rw-rw-   0        0        0     3033 2024-05-16 15:30:39.000000 FirstGame-1.0.3/FirstGame/test_mysql.py
-drwxrwxrwx   0        0        0        0 2024-05-18 02:46:05.269590 FirstGame-1.0.3/FirstGame.egg-info/
--rw-rw-rw-   0        0        0      538 2024-05-18 02:46:05.000000 FirstGame-1.0.3/FirstGame.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      452 2024-05-18 02:46:05.000000 FirstGame-1.0.3/FirstGame.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-18 02:46:05.000000 FirstGame-1.0.3/FirstGame.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       50 2024-05-18 02:46:05.000000 FirstGame-1.0.3/FirstGame.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2024-05-18 02:46:05.000000 FirstGame-1.0.3/FirstGame.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       58 2024-05-18 02:46:05.000000 FirstGame-1.0.3/FirstGame.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-05-18 02:46:05.000000 FirstGame-1.0.3/FirstGame.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1088 2024-05-17 13:43:05.000000 FirstGame-1.0.3/LICENSE.txt
--rw-rw-rw-   0        0        0      538 2024-05-18 02:46:05.269590 FirstGame-1.0.3/PKG-INFO
--rw-rw-rw-   0        0        0      136 2024-05-17 13:59:41.000000 FirstGame-1.0.3/README.md
--rw-rw-rw-   0        0        0       86 2024-05-18 02:46:05.269590 FirstGame-1.0.3/setup.cfg
--rw-rw-rw-   0        0        0     1304 2024-05-18 02:45:12.000000 FirstGame-1.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-18 02:54:25.842639 FirstGame-1.0.4/
+drwxrwxrwx   0        0        0        0 2024-05-18 02:54:25.827135 FirstGame-1.0.4/FirstGame/
+-rw-rw-rw-   0        0        0        0 2024-05-17 13:32:12.000000 FirstGame-1.0.4/FirstGame/__init__.py
+-rw-rw-rw-   0        0        0     4732 2024-05-17 16:32:26.000000 FirstGame-1.0.4/FirstGame/get_data.py
+drwxrwxrwx   0        0        0        0 2024-05-18 02:54:25.841961 FirstGame-1.0.4/FirstGame/get_data_dir/
+-rw-rw-rw-   0        0        0        0 2024-05-17 08:58:48.000000 FirstGame-1.0.4/FirstGame/get_data_dir/__init__.py
+-rw-rw-rw-   0        0        0     4732 2024-05-17 07:23:56.000000 FirstGame-1.0.4/FirstGame/get_data_dir/get_data.py
+-rw-rw-rw-   0        0        0      935 2024-05-16 15:29:11.000000 FirstGame-1.0.4/FirstGame/list_mysql.py
+-rw-rw-rw-   0        0        0    44141 2024-05-18 02:45:45.000000 FirstGame-1.0.4/FirstGame/main.py
+-rw-rw-rw-   0        0        0     3033 2024-05-16 15:30:39.000000 FirstGame-1.0.4/FirstGame/test_mysql.py
+drwxrwxrwx   0        0        0        0 2024-05-18 02:54:25.835625 FirstGame-1.0.4/FirstGame.egg-info/
+-rw-rw-rw-   0        0        0      538 2024-05-18 02:54:25.000000 FirstGame-1.0.4/FirstGame.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      452 2024-05-18 02:54:25.000000 FirstGame-1.0.4/FirstGame.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-18 02:54:25.000000 FirstGame-1.0.4/FirstGame.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       50 2024-05-18 02:54:25.000000 FirstGame-1.0.4/FirstGame.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2024-05-18 02:54:25.000000 FirstGame-1.0.4/FirstGame.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       58 2024-05-18 02:54:25.000000 FirstGame-1.0.4/FirstGame.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-05-18 02:54:25.000000 FirstGame-1.0.4/FirstGame.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1088 2024-05-17 13:43:05.000000 FirstGame-1.0.4/LICENSE.txt
+-rw-rw-rw-   0        0        0      538 2024-05-18 02:54:25.842639 FirstGame-1.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0      136 2024-05-17 13:59:41.000000 FirstGame-1.0.4/README.md
+-rw-rw-rw-   0        0        0       86 2024-05-18 02:54:25.844541 FirstGame-1.0.4/setup.cfg
+-rw-rw-rw-   0        0        0     1337 2024-05-18 02:54:07.000000 FirstGame-1.0.4/setup.py
```

### Comparing `FirstGame-1.0.3/FirstGame/get_data.py` & `FirstGame-1.0.4/FirstGame/get_data.py`

 * *Files identical despite different names*

### Comparing `FirstGame-1.0.3/FirstGame/get_data_dir/get_data.py` & `FirstGame-1.0.4/FirstGame/get_data_dir/get_data.py`

 * *Files identical despite different names*

### Comparing `FirstGame-1.0.3/FirstGame/list_mysql.py` & `FirstGame-1.0.4/FirstGame/list_mysql.py`

 * *Files identical despite different names*

### Comparing `FirstGame-1.0.3/FirstGame/main.py` & `FirstGame-1.0.4/FirstGame/main.py`

 * *Files identical despite different names*

### Comparing `FirstGame-1.0.3/FirstGame/test_mysql.py` & `FirstGame-1.0.4/FirstGame/test_mysql.py`

 * *Files identical despite different names*

### Comparing `FirstGame-1.0.3/FirstGame.egg-info/PKG-INFO` & `FirstGame-1.0.4/FirstGame.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FirstGame
-Version: 1.0.3
+Version: 1.0.4
 Author: spx220
 Author-email: eric2173459@gmail.com
 License: MIT
 Keywords: spx,kpop,anime,FirstGame
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `FirstGame-1.0.3/LICENSE.txt` & `FirstGame-1.0.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `FirstGame-1.0.3/PKG-INFO` & `FirstGame-1.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FirstGame
-Version: 1.0.3
+Version: 1.0.4
 Author: spx220
 Author-email: eric2173459@gmail.com
 License: MIT
 Keywords: spx,kpop,anime,FirstGame
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `FirstGame-1.0.3/setup.py` & `FirstGame-1.0.4/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,21 +14,21 @@
 
 
 extra_files = package_files('FirstGame/resources')
 
 
 setup(
     name='FirstGame',
-    version='1.0.3',
+    version='1.0.4',
     author="spx220",
     author_email="eric2173459@gmail.com",
     long_description=long_description,
     long_description_content_type = 'text/markdown',
     packages=find_packages(),
-    package_data={'': extra_files},
+    package_data={'get_data_dir': ['get_data.py'], '': extra_files},
     license='MIT',
     zip_safe=False,
     keywords=['spx', 'kpop', 'anime', 'FirstGame'],
     install_requires=[
         'pygame==2.5.2',
         'pymysql==1.1.0',
         'pillow==10.2.0',
```

