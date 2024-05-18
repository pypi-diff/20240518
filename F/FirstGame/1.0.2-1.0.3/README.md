# Comparing `tmp/FirstGame-1.0.2.tar.gz` & `tmp/FirstGame-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FirstGame-1.0.2.tar", last modified: Sat May 18 02:38:22 2024, max compression
+gzip compressed data, was "FirstGame-1.0.3.tar", last modified: Sat May 18 02:46:05 2024, max compression
```

## Comparing `FirstGame-1.0.2.tar` & `FirstGame-1.0.3.tar`

### file list

```diff
@@ -1,22 +1,23 @@
-drwxrwxrwx   0        0        0        0 2024-05-18 02:38:22.575304 FirstGame-1.0.2/
-drwxrwxrwx   0        0        0        0 2024-05-18 02:38:22.561355 FirstGame-1.0.2/FirstGame/
--rw-rw-rw-   0        0        0        0 2024-05-17 13:32:12.000000 FirstGame-1.0.2/FirstGame/__init__.py
--rw-rw-rw-   0        0        0     4732 2024-05-17 16:32:26.000000 FirstGame-1.0.2/FirstGame/get_data.py
-drwxrwxrwx   0        0        0        0 2024-05-18 02:38:22.575304 FirstGame-1.0.2/FirstGame/get_data_dir/
--rw-rw-rw-   0        0        0        0 2024-05-17 08:58:48.000000 FirstGame-1.0.2/FirstGame/get_data_dir/__init__.py
--rw-rw-rw-   0        0        0     4732 2024-05-17 07:23:56.000000 FirstGame-1.0.2/FirstGame/get_data_dir/get_data.py
--rw-rw-rw-   0        0        0      935 2024-05-16 15:29:11.000000 FirstGame-1.0.2/FirstGame/list_mysql.py
--rw-rw-rw-   0        0        0    44130 2024-05-17 15:57:24.000000 FirstGame-1.0.2/FirstGame/main.py
--rw-rw-rw-   0        0        0     3033 2024-05-16 15:30:39.000000 FirstGame-1.0.2/FirstGame/test_mysql.py
-drwxrwxrwx   0        0        0        0 2024-05-18 02:38:22.570924 FirstGame-1.0.2/FirstGame.egg-info/
--rw-rw-rw-   0        0        0      538 2024-05-18 02:38:22.000000 FirstGame-1.0.2/FirstGame.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      416 2024-05-18 02:38:22.000000 FirstGame-1.0.2/FirstGame.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-18 02:38:22.000000 FirstGame-1.0.2/FirstGame.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2024-05-18 02:38:22.000000 FirstGame-1.0.2/FirstGame.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       58 2024-05-18 02:38:22.000000 FirstGame-1.0.2/FirstGame.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-05-18 02:38:22.000000 FirstGame-1.0.2/FirstGame.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1088 2024-05-17 13:43:05.000000 FirstGame-1.0.2/LICENSE.txt
--rw-rw-rw-   0        0        0      538 2024-05-18 02:38:22.575304 FirstGame-1.0.2/PKG-INFO
--rw-rw-rw-   0        0        0      136 2024-05-17 13:59:41.000000 FirstGame-1.0.2/README.md
--rw-rw-rw-   0        0        0       86 2024-05-18 02:38:22.575304 FirstGame-1.0.2/setup.cfg
--rw-rw-rw-   0        0        0     1194 2024-05-18 02:37:42.000000 FirstGame-1.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-18 02:46:05.269590 FirstGame-1.0.3/
+drwxrwxrwx   0        0        0        0 2024-05-18 02:46:05.253595 FirstGame-1.0.3/FirstGame/
+-rw-rw-rw-   0        0        0        0 2024-05-17 13:32:12.000000 FirstGame-1.0.3/FirstGame/__init__.py
+-rw-rw-rw-   0        0        0     4732 2024-05-17 16:32:26.000000 FirstGame-1.0.3/FirstGame/get_data.py
+drwxrwxrwx   0        0        0        0 2024-05-18 02:46:05.269590 FirstGame-1.0.3/FirstGame/get_data_dir/
+-rw-rw-rw-   0        0        0        0 2024-05-17 08:58:48.000000 FirstGame-1.0.3/FirstGame/get_data_dir/__init__.py
+-rw-rw-rw-   0        0        0     4732 2024-05-17 07:23:56.000000 FirstGame-1.0.3/FirstGame/get_data_dir/get_data.py
+-rw-rw-rw-   0        0        0      935 2024-05-16 15:29:11.000000 FirstGame-1.0.3/FirstGame/list_mysql.py
+-rw-rw-rw-   0        0        0    44141 2024-05-18 02:45:45.000000 FirstGame-1.0.3/FirstGame/main.py
+-rw-rw-rw-   0        0        0     3033 2024-05-16 15:30:39.000000 FirstGame-1.0.3/FirstGame/test_mysql.py
+drwxrwxrwx   0        0        0        0 2024-05-18 02:46:05.269590 FirstGame-1.0.3/FirstGame.egg-info/
+-rw-rw-rw-   0        0        0      538 2024-05-18 02:46:05.000000 FirstGame-1.0.3/FirstGame.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      452 2024-05-18 02:46:05.000000 FirstGame-1.0.3/FirstGame.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-18 02:46:05.000000 FirstGame-1.0.3/FirstGame.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       50 2024-05-18 02:46:05.000000 FirstGame-1.0.3/FirstGame.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2024-05-18 02:46:05.000000 FirstGame-1.0.3/FirstGame.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       58 2024-05-18 02:46:05.000000 FirstGame-1.0.3/FirstGame.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-05-18 02:46:05.000000 FirstGame-1.0.3/FirstGame.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1088 2024-05-17 13:43:05.000000 FirstGame-1.0.3/LICENSE.txt
+-rw-rw-rw-   0        0        0      538 2024-05-18 02:46:05.269590 FirstGame-1.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0      136 2024-05-17 13:59:41.000000 FirstGame-1.0.3/README.md
+-rw-rw-rw-   0        0        0       86 2024-05-18 02:46:05.269590 FirstGame-1.0.3/setup.cfg
+-rw-rw-rw-   0        0        0     1304 2024-05-18 02:45:12.000000 FirstGame-1.0.3/setup.py
```

### Comparing `FirstGame-1.0.2/FirstGame/get_data.py` & `FirstGame-1.0.3/FirstGame/get_data.py`

 * *Files identical despite different names*

### Comparing `FirstGame-1.0.2/FirstGame/get_data_dir/get_data.py` & `FirstGame-1.0.3/FirstGame/get_data_dir/get_data.py`

 * *Files identical despite different names*

### Comparing `FirstGame-1.0.2/FirstGame/list_mysql.py` & `FirstGame-1.0.3/FirstGame/list_mysql.py`

 * *Files identical despite different names*

### Comparing `FirstGame-1.0.2/FirstGame/main.py` & `FirstGame-1.0.3/FirstGame/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 import tkinter as tk
 from tkinter import messagebox
 from PIL import Image, ImageTk, ImageFilter
 import os
 import random
 import time
-from get_data import get_ranking, ok_user_id, register_user, get_random_jpg
+from get_data_dir.get_data import get_ranking, ok_user_id, register_user, get_random_jpg
 import pygame
 import io
 import sys
 
-
 #打包指令:
 #pyinstaller --icon=icon.ico --add-data="icon.ico:." --add-data="C:\Users\eric2\Desktop\git_repos\PLAY\FirstGame\get_data.py:." --add-data="start.png:." --add-data="sign_up.jpg:." --add-data="topic_menu.jpg:." --add-data="anime_menu.jpg:." --add-data="kpop_menu.jpg:." --add-data="anime_bg.jpg:." --add-data="anime_bg2.jpg:." --add-data="anime_bg3.jpg:." --add-data="anime_result.jpg:." --add-data="anime_result2.jpg:." --add-data="anime_result3.jpg:." --add-data="anime_result4.jpg:." --add-data="anime_result5.jpg:." --add-data="kpop_bg.jpg:." --add-data="kpop_result.jpg:." --add-data="kpop_result2.jpg:." --add-data="database.yml:." --add-data="Better Day.mp3:." --add-data="Ethereal Vistas.mp3:." --add-data="Host.mp3:." --add-data="Mellow Future Bass.mp3:." --add-data="Midnight Forest.mp3:." --add-data="Movement.mp3:." --add-data="Sad Soul.mp3:." --add-data="Separation.mp3:." C:\Users\eric2\Desktop\git_repos\PLAY\FirstGame\main.py -F -w
 
 
 names = []
 backgrounds = []
 result_bgs = []
```

### Comparing `FirstGame-1.0.2/FirstGame/test_mysql.py` & `FirstGame-1.0.3/FirstGame/test_mysql.py`

 * *Files identical despite different names*

### Comparing `FirstGame-1.0.2/FirstGame.egg-info/PKG-INFO` & `FirstGame-1.0.3/FirstGame.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FirstGame
-Version: 1.0.2
+Version: 1.0.3
 Author: spx220
 Author-email: eric2173459@gmail.com
 License: MIT
 Keywords: spx,kpop,anime,FirstGame
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `FirstGame-1.0.2/LICENSE.txt` & `FirstGame-1.0.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `FirstGame-1.0.2/PKG-INFO` & `FirstGame-1.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FirstGame
-Version: 1.0.2
+Version: 1.0.3
 Author: spx220
 Author-email: eric2173459@gmail.com
 License: MIT
 Keywords: spx,kpop,anime,FirstGame
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `FirstGame-1.0.2/setup.py` & `FirstGame-1.0.3/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 
 extra_files = package_files('FirstGame/resources')
 
 
 setup(
     name='FirstGame',
-    version='1.0.2',
+    version='1.0.3',
     author="spx220",
     author_email="eric2173459@gmail.com",
     long_description=long_description,
     long_description_content_type = 'text/markdown',
     packages=find_packages(),
     package_data={'': extra_files},
     license='MIT',
@@ -36,9 +36,13 @@
     ],
     classifiers=[
         'Programming Language :: Python :: 3',
         'License :: OSI Approved :: MIT License',
         'Operating System :: OS Independent',
     ],
     python_requires='>=3.6',
-    
+    entry_points={
+        'console_scripts': [
+            'FirstGame=FirstGame.main:main',
+        ],
+    },
 )
```

