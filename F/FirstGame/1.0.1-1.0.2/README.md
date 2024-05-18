# Comparing `tmp/FirstGame-1.0.1.tar.gz` & `tmp/FirstGame-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FirstGame-1.0.1.tar", last modified: Sat May 18 02:08:23 2024, max compression
+gzip compressed data, was "FirstGame-1.0.2.tar", last modified: Sat May 18 02:38:22 2024, max compression
```

## Comparing `FirstGame-1.0.1.tar` & `FirstGame-1.0.2.tar`

### file list

```diff
@@ -1,23 +1,22 @@
-drwxrwxrwx   0        0        0        0 2024-05-18 02:08:23.987194 FirstGame-1.0.1/
-drwxrwxrwx   0        0        0        0 2024-05-18 02:08:23.976666 FirstGame-1.0.1/FirstGame/
--rw-rw-rw-   0        0        0        0 2024-05-17 13:32:12.000000 FirstGame-1.0.1/FirstGame/__init__.py
--rw-rw-rw-   0        0        0     4732 2024-05-17 16:32:26.000000 FirstGame-1.0.1/FirstGame/get_data.py
-drwxrwxrwx   0        0        0        0 2024-05-18 02:08:23.984943 FirstGame-1.0.1/FirstGame/get_data_dir/
--rw-rw-rw-   0        0        0        0 2024-05-17 08:58:48.000000 FirstGame-1.0.1/FirstGame/get_data_dir/__init__.py
--rw-rw-rw-   0        0        0     4732 2024-05-17 07:23:56.000000 FirstGame-1.0.1/FirstGame/get_data_dir/get_data.py
--rw-rw-rw-   0        0        0      935 2024-05-16 15:29:11.000000 FirstGame-1.0.1/FirstGame/list_mysql.py
--rw-rw-rw-   0        0        0    44130 2024-05-17 15:57:24.000000 FirstGame-1.0.1/FirstGame/main.py
--rw-rw-rw-   0        0        0     3033 2024-05-16 15:30:39.000000 FirstGame-1.0.1/FirstGame/test_mysql.py
-drwxrwxrwx   0        0        0        0 2024-05-18 02:08:23.984943 FirstGame-1.0.1/FirstGame.egg-info/
--rw-rw-rw-   0        0        0      538 2024-05-18 02:08:23.000000 FirstGame-1.0.1/FirstGame.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      452 2024-05-18 02:08:23.000000 FirstGame-1.0.1/FirstGame.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-18 02:08:23.000000 FirstGame-1.0.1/FirstGame.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       50 2024-05-18 02:08:23.000000 FirstGame-1.0.1/FirstGame.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2024-05-18 02:06:45.000000 FirstGame-1.0.1/FirstGame.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       58 2024-05-18 02:08:23.000000 FirstGame-1.0.1/FirstGame.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-05-18 02:08:23.000000 FirstGame-1.0.1/FirstGame.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1088 2024-05-17 13:43:05.000000 FirstGame-1.0.1/LICENSE.txt
--rw-rw-rw-   0        0        0      538 2024-05-18 02:08:23.987194 FirstGame-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      136 2024-05-17 13:59:41.000000 FirstGame-1.0.1/README.md
--rw-rw-rw-   0        0        0       86 2024-05-18 02:08:23.987194 FirstGame-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1304 2024-05-18 02:04:57.000000 FirstGame-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-18 02:38:22.575304 FirstGame-1.0.2/
+drwxrwxrwx   0        0        0        0 2024-05-18 02:38:22.561355 FirstGame-1.0.2/FirstGame/
+-rw-rw-rw-   0        0        0        0 2024-05-17 13:32:12.000000 FirstGame-1.0.2/FirstGame/__init__.py
+-rw-rw-rw-   0        0        0     4732 2024-05-17 16:32:26.000000 FirstGame-1.0.2/FirstGame/get_data.py
+drwxrwxrwx   0        0        0        0 2024-05-18 02:38:22.575304 FirstGame-1.0.2/FirstGame/get_data_dir/
+-rw-rw-rw-   0        0        0        0 2024-05-17 08:58:48.000000 FirstGame-1.0.2/FirstGame/get_data_dir/__init__.py
+-rw-rw-rw-   0        0        0     4732 2024-05-17 07:23:56.000000 FirstGame-1.0.2/FirstGame/get_data_dir/get_data.py
+-rw-rw-rw-   0        0        0      935 2024-05-16 15:29:11.000000 FirstGame-1.0.2/FirstGame/list_mysql.py
+-rw-rw-rw-   0        0        0    44130 2024-05-17 15:57:24.000000 FirstGame-1.0.2/FirstGame/main.py
+-rw-rw-rw-   0        0        0     3033 2024-05-16 15:30:39.000000 FirstGame-1.0.2/FirstGame/test_mysql.py
+drwxrwxrwx   0        0        0        0 2024-05-18 02:38:22.570924 FirstGame-1.0.2/FirstGame.egg-info/
+-rw-rw-rw-   0        0        0      538 2024-05-18 02:38:22.000000 FirstGame-1.0.2/FirstGame.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      416 2024-05-18 02:38:22.000000 FirstGame-1.0.2/FirstGame.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-18 02:38:22.000000 FirstGame-1.0.2/FirstGame.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2024-05-18 02:38:22.000000 FirstGame-1.0.2/FirstGame.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       58 2024-05-18 02:38:22.000000 FirstGame-1.0.2/FirstGame.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-05-18 02:38:22.000000 FirstGame-1.0.2/FirstGame.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1088 2024-05-17 13:43:05.000000 FirstGame-1.0.2/LICENSE.txt
+-rw-rw-rw-   0        0        0      538 2024-05-18 02:38:22.575304 FirstGame-1.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0      136 2024-05-17 13:59:41.000000 FirstGame-1.0.2/README.md
+-rw-rw-rw-   0        0        0       86 2024-05-18 02:38:22.575304 FirstGame-1.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1194 2024-05-18 02:37:42.000000 FirstGame-1.0.2/setup.py
```

### Comparing `FirstGame-1.0.1/FirstGame/get_data.py` & `FirstGame-1.0.2/FirstGame/get_data.py`

 * *Files identical despite different names*

### Comparing `FirstGame-1.0.1/FirstGame/get_data_dir/get_data.py` & `FirstGame-1.0.2/FirstGame/get_data_dir/get_data.py`

 * *Files identical despite different names*

### Comparing `FirstGame-1.0.1/FirstGame/list_mysql.py` & `FirstGame-1.0.2/FirstGame/list_mysql.py`

 * *Files identical despite different names*

### Comparing `FirstGame-1.0.1/FirstGame/main.py` & `FirstGame-1.0.2/FirstGame/main.py`

 * *Files identical despite different names*

### Comparing `FirstGame-1.0.1/FirstGame/test_mysql.py` & `FirstGame-1.0.2/FirstGame/test_mysql.py`

 * *Files identical despite different names*

### Comparing `FirstGame-1.0.1/FirstGame.egg-info/PKG-INFO` & `FirstGame-1.0.2/FirstGame.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FirstGame
-Version: 1.0.1
+Version: 1.0.2
 Author: spx220
 Author-email: eric2173459@gmail.com
 License: MIT
 Keywords: spx,kpop,anime,FirstGame
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `FirstGame-1.0.1/LICENSE.txt` & `FirstGame-1.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `FirstGame-1.0.1/PKG-INFO` & `FirstGame-1.0.2/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FirstGame
-Version: 1.0.1
+Version: 1.0.2
 Author: spx220
 Author-email: eric2173459@gmail.com
 License: MIT
 Keywords: spx,kpop,anime,FirstGame
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `FirstGame-1.0.1/setup.py` & `FirstGame-1.0.2/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 
 extra_files = package_files('FirstGame/resources')
 
 
 setup(
     name='FirstGame',
-    version='1.0.1',
+    version='1.0.2',
     author="spx220",
     author_email="eric2173459@gmail.com",
     long_description=long_description,
     long_description_content_type = 'text/markdown',
     packages=find_packages(),
     package_data={'': extra_files},
     license='MIT',
@@ -36,13 +36,9 @@
     ],
     classifiers=[
         'Programming Language :: Python :: 3',
         'License :: OSI Approved :: MIT License',
         'Operating System :: OS Independent',
     ],
     python_requires='>=3.6',
-    entry_points={
-        'console_scripts': [
-            'FirstGame=FirstGame.main:main',
-        ],
-    },
+    
 )
```

