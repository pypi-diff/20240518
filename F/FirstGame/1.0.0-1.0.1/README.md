# Comparing `tmp/FirstGame-1.0.0.tar.gz` & `tmp/FirstGame-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FirstGame-1.0.0.tar", last modified: Fri May 17 14:35:53 2024, max compression
+gzip compressed data, was "FirstGame-1.0.1.tar", last modified: Sat May 18 02:08:23 2024, max compression
```

## Comparing `FirstGame-1.0.0.tar` & `FirstGame-1.0.1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2024-05-17 14:35:53.846214 FirstGame-1.0.0/
-drwxrwxrwx   0        0        0        0 2024-05-17 14:35:53.838711 FirstGame-1.0.0/FirstGame/
--rw-rw-rw-   0        0        0        0 2024-05-17 13:32:12.000000 FirstGame-1.0.0/FirstGame/__init__.py
--rw-rw-rw-   0        0        0      200 2024-05-10 04:50:44.000000 FirstGame-1.0.0/FirstGame/find_all_font.py
--rw-rw-rw-   0        0        0     4732 2024-05-17 11:34:08.000000 FirstGame-1.0.0/FirstGame/get_data.py
--rw-rw-rw-   0        0        0      935 2024-05-16 15:29:11.000000 FirstGame-1.0.0/FirstGame/list_mysql.py
--rw-rw-rw-   0        0        0    44082 2024-05-17 13:21:51.000000 FirstGame-1.0.0/FirstGame/main.py
--rw-rw-rw-   0        0        0     1334 2024-05-14 05:14:38.000000 FirstGame-1.0.0/FirstGame/play_music.py
--rw-rw-rw-   0        0        0      966 2024-05-14 02:24:46.000000 FirstGame-1.0.0/FirstGame/pygame_test.py
--rw-rw-rw-   0        0        0     3033 2024-05-16 15:30:39.000000 FirstGame-1.0.0/FirstGame/test_mysql.py
-drwxrwxrwx   0        0        0        0 2024-05-17 14:35:53.846214 FirstGame-1.0.0/FirstGame.egg-info/
--rw-rw-rw-   0        0        0      487 2024-05-17 14:35:53.000000 FirstGame-1.0.0/FirstGame.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      458 2024-05-17 14:35:53.000000 FirstGame-1.0.0/FirstGame.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-17 14:35:53.000000 FirstGame-1.0.0/FirstGame.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       41 2024-05-17 14:35:53.000000 FirstGame-1.0.0/FirstGame.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2024-05-17 14:35:32.000000 FirstGame-1.0.0/FirstGame.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       58 2024-05-17 14:35:53.000000 FirstGame-1.0.0/FirstGame.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-05-17 14:35:53.000000 FirstGame-1.0.0/FirstGame.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1088 2024-05-17 13:43:05.000000 FirstGame-1.0.0/LICENSE.txt
--rw-rw-rw-   0        0        0      487 2024-05-17 14:35:53.846214 FirstGame-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0      136 2024-05-17 13:59:41.000000 FirstGame-1.0.0/README.md
--rw-rw-rw-   0        0        0       86 2024-05-17 14:35:53.854215 FirstGame-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0      716 2024-05-17 14:27:46.000000 FirstGame-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-18 02:08:23.987194 FirstGame-1.0.1/
+drwxrwxrwx   0        0        0        0 2024-05-18 02:08:23.976666 FirstGame-1.0.1/FirstGame/
+-rw-rw-rw-   0        0        0        0 2024-05-17 13:32:12.000000 FirstGame-1.0.1/FirstGame/__init__.py
+-rw-rw-rw-   0        0        0     4732 2024-05-17 16:32:26.000000 FirstGame-1.0.1/FirstGame/get_data.py
+drwxrwxrwx   0        0        0        0 2024-05-18 02:08:23.984943 FirstGame-1.0.1/FirstGame/get_data_dir/
+-rw-rw-rw-   0        0        0        0 2024-05-17 08:58:48.000000 FirstGame-1.0.1/FirstGame/get_data_dir/__init__.py
+-rw-rw-rw-   0        0        0     4732 2024-05-17 07:23:56.000000 FirstGame-1.0.1/FirstGame/get_data_dir/get_data.py
+-rw-rw-rw-   0        0        0      935 2024-05-16 15:29:11.000000 FirstGame-1.0.1/FirstGame/list_mysql.py
+-rw-rw-rw-   0        0        0    44130 2024-05-17 15:57:24.000000 FirstGame-1.0.1/FirstGame/main.py
+-rw-rw-rw-   0        0        0     3033 2024-05-16 15:30:39.000000 FirstGame-1.0.1/FirstGame/test_mysql.py
+drwxrwxrwx   0        0        0        0 2024-05-18 02:08:23.984943 FirstGame-1.0.1/FirstGame.egg-info/
+-rw-rw-rw-   0        0        0      538 2024-05-18 02:08:23.000000 FirstGame-1.0.1/FirstGame.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      452 2024-05-18 02:08:23.000000 FirstGame-1.0.1/FirstGame.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-18 02:08:23.000000 FirstGame-1.0.1/FirstGame.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       50 2024-05-18 02:08:23.000000 FirstGame-1.0.1/FirstGame.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2024-05-18 02:06:45.000000 FirstGame-1.0.1/FirstGame.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       58 2024-05-18 02:08:23.000000 FirstGame-1.0.1/FirstGame.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-05-18 02:08:23.000000 FirstGame-1.0.1/FirstGame.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1088 2024-05-17 13:43:05.000000 FirstGame-1.0.1/LICENSE.txt
+-rw-rw-rw-   0        0        0      538 2024-05-18 02:08:23.987194 FirstGame-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0      136 2024-05-17 13:59:41.000000 FirstGame-1.0.1/README.md
+-rw-rw-rw-   0        0        0       86 2024-05-18 02:08:23.987194 FirstGame-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0     1304 2024-05-18 02:04:57.000000 FirstGame-1.0.1/setup.py
```

### Comparing `FirstGame-1.0.0/FirstGame/get_data.py` & `FirstGame-1.0.1/FirstGame/get_data.py`

 * *Files identical despite different names*

### Comparing `FirstGame-1.0.0/FirstGame/list_mysql.py` & `FirstGame-1.0.1/FirstGame/list_mysql.py`

 * *Files identical despite different names*

### Comparing `FirstGame-1.0.0/FirstGame/main.py` & `FirstGame-1.0.1/FirstGame/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 import tkinter as tk
 from tkinter import messagebox
 from PIL import Image, ImageTk, ImageFilter
 import os
 import random
 import time
-from get_data.get_data import get_ranking, ok_user_id, register_user, get_random_jpg
+from get_data import get_ranking, ok_user_id, register_user, get_random_jpg
 import pygame
 import io
 import sys
 
 
-
 #打包指令:
-#pyinstaller --icon=icon.ico --add-data="C:\Users\eric2\Desktop\git_repos\PLAY\get_data.py:." --add-data="start.png:." --add-data="sign_up.jpg:." --add-data="topic_menu.jpg:." --add-data="anime_menu.jpg:." --add-data="kpop_menu.jpg:." --add-data="anime_bg.jpg:." --add-data="anime_bg2.jpg:." --add-data="anime_bg3.jpg:." --add-data="anime_result.jpg:." --add-data="anime_result2.jpg:." --add-data="anime_result3.jpg:." --add-data="anime_result4.jpg:." --add-data="anime_result5.jpg:." --add-data="kpop_bg.jpg:." --add-data="kpop_result.jpg:." --add-data="kpop_result2.jpg:." --add-data="database.yml:." --add-data="Better Day.mp3:." --add-data="Ethereal Vistas.mp3:." --add-data="Host.mp3:." --add-data="Mellow Future Bass.mp3:." --add-data="Midnight Forest.mp3:." --add-data="Movement.mp3:." --add-data="Sad Soul.mp3:." --add-data="Separation.mp3:." C:\Users\eric2\Desktop\git_repos\PLAY\main.py -F -w
+#pyinstaller --icon=icon.ico --add-data="icon.ico:." --add-data="C:\Users\eric2\Desktop\git_repos\PLAY\FirstGame\get_data.py:." --add-data="start.png:." --add-data="sign_up.jpg:." --add-data="topic_menu.jpg:." --add-data="anime_menu.jpg:." --add-data="kpop_menu.jpg:." --add-data="anime_bg.jpg:." --add-data="anime_bg2.jpg:." --add-data="anime_bg3.jpg:." --add-data="anime_result.jpg:." --add-data="anime_result2.jpg:." --add-data="anime_result3.jpg:." --add-data="anime_result4.jpg:." --add-data="anime_result5.jpg:." --add-data="kpop_bg.jpg:." --add-data="kpop_result.jpg:." --add-data="kpop_result2.jpg:." --add-data="database.yml:." --add-data="Better Day.mp3:." --add-data="Ethereal Vistas.mp3:." --add-data="Host.mp3:." --add-data="Mellow Future Bass.mp3:." --add-data="Midnight Forest.mp3:." --add-data="Movement.mp3:." --add-data="Sad Soul.mp3:." --add-data="Separation.mp3:." C:\Users\eric2\Desktop\git_repos\PLAY\FirstGame\main.py -F -w
 
 
 names = []
 backgrounds = []
 result_bgs = []
 
 animes = ['蠟筆小新', '鏈鋸人', '藍色監獄', '獵人', '實力至上', '間諜家家酒', '棍勇',
@@ -280,15 +279,15 @@
 # 開啟tkinter介面
 def tkinter() -> None:
     global root
     
     # 建立tkinter介面
     root = tk.Tk()
     root.title('Anime_Guess')
-    root.iconbitmap('icon.ico')
+    root.iconbitmap(resource_path('icon.ico'))
     root.geometry(f'{bg_width}x{bg_height}+100+0')
     # 禁用視窗縮放功能
     root.resizable(False, False)
     try:
         # 建立主題選擇
         topic_menu()
         # 建立主選單背景
```

### Comparing `FirstGame-1.0.0/FirstGame/test_mysql.py` & `FirstGame-1.0.1/FirstGame/test_mysql.py`

 * *Files identical despite different names*

### Comparing `FirstGame-1.0.0/LICENSE.txt` & `FirstGame-1.0.1/LICENSE.txt`

 * *Files identical despite different names*

