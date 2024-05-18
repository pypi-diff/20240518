# Comparing `tmp/FirstGame-1.0.5.tar.gz` & `tmp/FirstGame-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FirstGame-1.0.5.tar", last modified: Sat May 18 03:02:52 2024, max compression
+gzip compressed data, was "FirstGame-1.0.6.tar", last modified: Sat May 18 03:08:56 2024, max compression
```

## Comparing `FirstGame-1.0.5.tar` & `FirstGame-1.0.6.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2024-05-18 03:02:52.278346 FirstGame-1.0.5/
-drwxrwxrwx   0        0        0        0 2024-05-18 03:02:52.264572 FirstGame-1.0.5/FirstGame/
--rw-rw-rw-   0        0        0        0 2024-05-17 13:32:12.000000 FirstGame-1.0.5/FirstGame/__init__.py
--rw-rw-rw-   0        0        0     4732 2024-05-17 16:32:26.000000 FirstGame-1.0.5/FirstGame/get_data.py
-drwxrwxrwx   0        0        0        0 2024-05-18 03:02:52.273027 FirstGame-1.0.5/FirstGame/get_data_dir/
--rw-rw-rw-   0        0        0        0 2024-05-17 08:58:48.000000 FirstGame-1.0.5/FirstGame/get_data_dir/__init__.py
--rw-rw-rw-   0        0        0     4732 2024-05-17 07:23:56.000000 FirstGame-1.0.5/FirstGame/get_data_dir/get_data.py
--rw-rw-rw-   0        0        0      935 2024-05-16 15:29:11.000000 FirstGame-1.0.5/FirstGame/list_mysql.py
--rw-rw-rw-   0        0        0    44128 2024-05-18 03:01:35.000000 FirstGame-1.0.5/FirstGame/main.py
--rw-rw-rw-   0        0        0     3033 2024-05-16 15:30:39.000000 FirstGame-1.0.5/FirstGame/test_mysql.py
-drwxrwxrwx   0        0        0        0 2024-05-18 03:02:52.273027 FirstGame-1.0.5/FirstGame.egg-info/
--rw-rw-rw-   0        0        0      538 2024-05-18 03:02:52.000000 FirstGame-1.0.5/FirstGame.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      452 2024-05-18 03:02:52.000000 FirstGame-1.0.5/FirstGame.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-18 03:02:52.000000 FirstGame-1.0.5/FirstGame.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       50 2024-05-18 03:02:52.000000 FirstGame-1.0.5/FirstGame.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2024-05-18 03:02:52.000000 FirstGame-1.0.5/FirstGame.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       58 2024-05-18 03:02:52.000000 FirstGame-1.0.5/FirstGame.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-05-18 03:02:52.000000 FirstGame-1.0.5/FirstGame.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1088 2024-05-17 13:43:05.000000 FirstGame-1.0.5/LICENSE.txt
--rw-rw-rw-   0        0        0      538 2024-05-18 03:02:52.278346 FirstGame-1.0.5/PKG-INFO
--rw-rw-rw-   0        0        0      136 2024-05-17 13:59:41.000000 FirstGame-1.0.5/README.md
--rw-rw-rw-   0        0        0       86 2024-05-18 03:02:52.278346 FirstGame-1.0.5/setup.cfg
--rw-rw-rw-   0        0        0     1304 2024-05-18 03:01:51.000000 FirstGame-1.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-18 03:08:56.116716 FirstGame-1.0.6/
+drwxrwxrwx   0        0        0        0 2024-05-18 03:08:56.106823 FirstGame-1.0.6/FirstGame/
+-rw-rw-rw-   0        0        0        0 2024-05-17 13:32:12.000000 FirstGame-1.0.6/FirstGame/__init__.py
+-rw-rw-rw-   0        0        0     4732 2024-05-17 16:32:26.000000 FirstGame-1.0.6/FirstGame/get_data.py
+drwxrwxrwx   0        0        0        0 2024-05-18 03:08:56.114376 FirstGame-1.0.6/FirstGame/get_data_dir/
+-rw-rw-rw-   0        0        0        0 2024-05-17 08:58:48.000000 FirstGame-1.0.6/FirstGame/get_data_dir/__init__.py
+-rw-rw-rw-   0        0        0     4732 2024-05-17 07:23:56.000000 FirstGame-1.0.6/FirstGame/get_data_dir/get_data.py
+-rw-rw-rw-   0        0        0      935 2024-05-16 15:29:11.000000 FirstGame-1.0.6/FirstGame/list_mysql.py
+-rw-rw-rw-   0        0        0    48595 2024-05-18 03:07:04.000000 FirstGame-1.0.6/FirstGame/main.py
+-rw-rw-rw-   0        0        0     3033 2024-05-16 15:30:39.000000 FirstGame-1.0.6/FirstGame/test_mysql.py
+drwxrwxrwx   0        0        0        0 2024-05-18 03:08:56.112469 FirstGame-1.0.6/FirstGame.egg-info/
+-rw-rw-rw-   0        0        0      538 2024-05-18 03:08:56.000000 FirstGame-1.0.6/FirstGame.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      452 2024-05-18 03:08:56.000000 FirstGame-1.0.6/FirstGame.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-18 03:08:56.000000 FirstGame-1.0.6/FirstGame.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       50 2024-05-18 03:08:56.000000 FirstGame-1.0.6/FirstGame.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2024-05-18 03:08:56.000000 FirstGame-1.0.6/FirstGame.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       58 2024-05-18 03:08:56.000000 FirstGame-1.0.6/FirstGame.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-05-18 03:08:56.000000 FirstGame-1.0.6/FirstGame.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1088 2024-05-17 13:43:05.000000 FirstGame-1.0.6/LICENSE.txt
+-rw-rw-rw-   0        0        0      538 2024-05-18 03:08:56.116716 FirstGame-1.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0      136 2024-05-17 13:59:41.000000 FirstGame-1.0.6/README.md
+-rw-rw-rw-   0        0        0       86 2024-05-18 03:08:56.118038 FirstGame-1.0.6/setup.cfg
+-rw-rw-rw-   0        0        0     1304 2024-05-18 03:08:43.000000 FirstGame-1.0.6/setup.py
```

### Comparing `FirstGame-1.0.5/FirstGame/get_data.py` & `FirstGame-1.0.6/FirstGame/get_data.py`

 * *Files identical despite different names*

### Comparing `FirstGame-1.0.5/FirstGame/get_data_dir/get_data.py` & `FirstGame-1.0.6/FirstGame/get_data_dir/get_data.py`

 * *Files identical despite different names*

### Comparing `FirstGame-1.0.5/FirstGame/list_mysql.py` & `FirstGame-1.0.6/FirstGame/list_mysql.py`

 * *Files identical despite different names*

### Comparing `FirstGame-1.0.5/FirstGame/main.py` & `FirstGame-1.0.6/FirstGame/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,160 @@
 import tkinter as tk
 from tkinter import messagebox
 from PIL import Image, ImageTk, ImageFilter
 import os
 import random
 import time
-from get_data import get_ranking, ok_user_id, register_user, get_random_jpg
+#from get_data import get_ranking, ok_user_id, register_user, get_random_jpg
 import pygame
 import io
 import sys
+import pymysql
+import re
+import yaml
 
 #打包指令:
 #pyinstaller --icon=icon.ico --add-data="icon.ico:." --add-data="C:\Users\eric2\Desktop\git_repos\PLAY\FirstGame\get_data.py:." --add-data="start.png:." --add-data="sign_up.jpg:." --add-data="topic_menu.jpg:." --add-data="anime_menu.jpg:." --add-data="kpop_menu.jpg:." --add-data="anime_bg.jpg:." --add-data="anime_bg2.jpg:." --add-data="anime_bg3.jpg:." --add-data="anime_result.jpg:." --add-data="anime_result2.jpg:." --add-data="anime_result3.jpg:." --add-data="anime_result4.jpg:." --add-data="anime_result5.jpg:." --add-data="kpop_bg.jpg:." --add-data="kpop_result.jpg:." --add-data="kpop_result2.jpg:." --add-data="database.yml:." --add-data="Better Day.mp3:." --add-data="Ethereal Vistas.mp3:." --add-data="Host.mp3:." --add-data="Mellow Future Bass.mp3:." --add-data="Midnight Forest.mp3:." --add-data="Movement.mp3:." --add-data="Sad Soul.mp3:." --add-data="Separation.mp3:." C:\Users\eric2\Desktop\git_repos\PLAY\FirstGame\main.py -F -w
 
+"""get_data"""
+# 連結database
+def connect_to_database():
+    with open(resource_path('database.yml'), 'r') as file:
+        config = yaml.safe_load(file)
 
+    db_settings = {
+        "host": config['database']['host'],
+        "port": config['database']['port'],
+        "user": config['database']['user'],
+        "password": config['database']['password'],
+        "db": config['database']['db'],
+        "charset": config['database']['charset']
+    }
+
+    try:
+        # 建立Connection物件
+        conn = pymysql.connect(**db_settings)
+        return conn
+    except Exception as ex:
+        print(ex)
+        return None
+
+# 判定是否註冊過
+def ok_user_id(user_id):
+    conn = connect_to_database()
+    if conn:
+        try:
+            # 建立Cursor物件
+            with conn.cursor() as cursor:
+                # 查詢資料SQL語法
+                command = "SELECT username, password FROM user WHERE username=%s"
+                # 執行指令
+                cursor.execute(command,(user_id,))
+                # 取得所有資料
+                result = cursor.fetchall()
+                print(result)
+        except Exception as ex:
+            print(ex)
+
+        if result:
+            # 在result中找到了user_id
+            password = result[0][1]
+        else:
+            # result為空，沒有找到匹配的user_id
+            password = ''
+        return password
+
+# 取得前10排名
+def get_ranking(now, user_id, score, total, level, topic):
+    conn = connect_to_database()
+    if conn:
+        try:
+            # 建立Cursor物件
+            with conn.cursor() as cursor:
+                # 新增資料SQL語法
+                command = "INSERT INTO charts(time, name, score, total, level, topic)VALUES(%s, %s, %s, %s, %s, %s)"
+                # 新增"結束時間", "使用者名稱", "遊戲分數", "題數", "難易度", "主題"給資料庫
+                cursor.execute(command, (now, user_id, score, total, level, topic))
+                # 儲存變更
+                conn.commit()
+
+                # 查詢資料SQL語法
+                command = "SELECT DISTINCT name, score, time FROM charts WHERE level = %s AND total = %s AND topic = %s ORDER BY score DESC LIMIT 10"
+                # 執行指令
+                cursor.execute(command, (level, total, topic))
+                # 取得所有資料
+                result = cursor.fetchall()
+                
+        except Exception as ex:
+            print(ex)
+
+        return result
+
+# 註冊帳號資料
+def register_user(username, password):
+    conn = connect_to_database()
+    try:
+        # 建立Cursor物件
+        with conn.cursor() as cursor:
+            # 新增資料SQL語法
+            command = "INSERT INTO user(username, password)VALUES(%s, %s)"
+            cursor.execute(command, (username, password))
+            # 儲存變更
+            conn.commit()
+    except Exception as ex:
+        print(ex)
+
+# 取得圖片二進制資料
+def get_picture_data(selected_topic, group_name):
+    global selected_pictures
+    conn = connect_to_database()
+    try: 
+        # 建立Cursor物件
+        with conn.cursor() as cursor:
+            if selected_topic == 'anime':
+                command = "SELECT picture, name, group_name FROM anime WHERE group_name=%s"
+            elif selected_topic == 'kpop':
+                command = "SELECT picture, name, group_name FROM kpop WHERE group_name=%s"
+            cursor.execute(command, (group_name))
+            result = cursor.fetchall()
+            selected_pictures += result
+        # 儲存
+        conn.commit()
+    except Exception as ex:
+        print(ex)
+
+# 取得選取圖檔的二進制
+def get_random_jpg(selected_topic, groups):
+    global selected_pictures
+    selected_pictures = []
+    pictures = []
+    answers = []
+    group_names = []
+
+    for group_name in groups:
+        get_picture_data(selected_topic, group_name)
+
+    random.shuffle(selected_pictures)
+
+    for i in selected_pictures:
+        picture = i[0]
+        name = i[1]
+        group = i[2]
+        # 將尾巴數字去掉變成答案
+        answer = re.sub(r'\d+', '', name)
+
+        pictures.append(picture)
+        answers.append(answer)
+        group_names.append(group)
+    return answers, pictures, group_names
+
+
+
+
+"""宣告"""
 names = []
 backgrounds = []
 result_bgs = []
 
 animes = ['蠟筆小新', '鏈鋸人', '藍色監獄', '獵人', '實力至上', '間諜家家酒', '棍勇',
           '鬼滅之刃', '海賊王', '果青', '咒術迴戰', '我英', '死神', '死亡筆記本',
           '火影', '刀劍神域']
```

### Comparing `FirstGame-1.0.5/FirstGame/test_mysql.py` & `FirstGame-1.0.6/FirstGame/test_mysql.py`

 * *Files identical despite different names*

### Comparing `FirstGame-1.0.5/FirstGame.egg-info/PKG-INFO` & `FirstGame-1.0.6/FirstGame.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FirstGame
-Version: 1.0.5
+Version: 1.0.6
 Author: spx220
 Author-email: eric2173459@gmail.com
 License: MIT
 Keywords: spx,kpop,anime,FirstGame
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `FirstGame-1.0.5/LICENSE.txt` & `FirstGame-1.0.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `FirstGame-1.0.5/PKG-INFO` & `FirstGame-1.0.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FirstGame
-Version: 1.0.5
+Version: 1.0.6
 Author: spx220
 Author-email: eric2173459@gmail.com
 License: MIT
 Keywords: spx,kpop,anime,FirstGame
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `FirstGame-1.0.5/setup.py` & `FirstGame-1.0.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 
 extra_files = package_files('FirstGame/resources')
 
 
 setup(
     name='FirstGame',
-    version='1.0.5',
+    version='1.0.6',
     author="spx220",
     author_email="eric2173459@gmail.com",
     long_description=long_description,
     long_description_content_type = 'text/markdown',
     packages=find_packages(),
     package_data={'': extra_files},
     license='MIT',
```

