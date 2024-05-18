# Comparing `tmp/ncmlistdownloader-2.0.0.240516a1.tar.gz` & `tmp/ncmlistdownloader-2.0.0.240517a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ncmlistdownloader-2.0.0.240516a1.tar", last modified: Thu May 16 15:00:08 2024, max compression
+gzip compressed data, was "ncmlistdownloader-2.0.0.240517a1.tar", last modified: Fri May 17 15:02:58 2024, max compression
```

## Comparing `ncmlistdownloader-2.0.0.240516a1.tar` & `ncmlistdownloader-2.0.0.240517a1.tar`

### file list

```diff
@@ -1,38 +1,39 @@
-drwxrwxrwx   0        0        0        0 2024-05-16 15:00:08.639268 ncmlistdownloader-2.0.0.240516a1/
--rw-rw-rw-   0        0        0    35181 2024-05-16 14:27:24.000000 ncmlistdownloader-2.0.0.240516a1/LICENSE
--rw-rw-rw-   0        0        0     1297 2024-05-16 15:00:08.637937 ncmlistdownloader-2.0.0.240516a1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-16 15:00:08.583064 ncmlistdownloader-2.0.0.240516a1/ncmlistdownloader/
--rw-rw-rw-   0        0        0        0 2024-05-16 14:32:33.000000 ncmlistdownloader-2.0.0.240516a1/ncmlistdownloader/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-16 15:00:08.598671 ncmlistdownloader-2.0.0.240516a1/ncmlistdownloader/_old/
--rw-rw-rw-   0        0        0     1880 2024-05-16 14:27:24.000000 ncmlistdownloader-2.0.0.240516a1/ncmlistdownloader/_old/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-16 15:00:08.607287 ncmlistdownloader-2.0.0.240516a1/ncmlistdownloader/_old/cmd/
--rw-rw-rw-   0        0        0     1789 2024-05-16 14:27:24.000000 ncmlistdownloader-2.0.0.240516a1/ncmlistdownloader/_old/cmd/__init__.py
--rw-rw-rw-   0        0        0      651 2024-05-16 14:27:24.000000 ncmlistdownloader-2.0.0.240516a1/ncmlistdownloader/_old/cmd/common.py
--rw-rw-rw-   0        0        0     1685 2024-05-16 14:27:24.000000 ncmlistdownloader-2.0.0.240516a1/ncmlistdownloader/_old/cmd/download.py
--rw-rw-rw-   0        0        0     2689 2024-05-16 14:27:24.000000 ncmlistdownloader-2.0.0.240516a1/ncmlistdownloader/_old/cmd/find_from_id.py
--rw-rw-rw-   0        0        0     1664 2024-05-16 14:27:24.000000 ncmlistdownloader-2.0.0.240516a1/ncmlistdownloader/_old/cmd/json_io.py
-drwxrwxrwx   0        0        0        0 2024-05-16 15:00:08.617339 ncmlistdownloader-2.0.0.240516a1/ncmlistdownloader/_old/common/
--rw-rw-rw-   0        0        0     2862 2024-04-29 10:21:37.000000 ncmlistdownloader-2.0.0.240516a1/ncmlistdownloader/_old/common/__init__.py
--rw-rw-rw-   0        0        0     2161 2024-04-29 10:21:11.000000 ncmlistdownloader-2.0.0.240516a1/ncmlistdownloader/_old/common/encode_sec_key.py
--rw-rw-rw-   0        0        0     1791 2024-04-29 10:20:35.000000 ncmlistdownloader-2.0.0.240516a1/ncmlistdownloader/_old/common/thread_test.py
-drwxrwxrwx   0        0        0        0 2024-05-16 15:00:08.621712 ncmlistdownloader-2.0.0.240516a1/ncmlistdownloader/_old/downloader/
--rw-rw-rw-   0        0        0     6233 2024-04-29 10:20:23.000000 ncmlistdownloader-2.0.0.240516a1/ncmlistdownloader/_old/downloader/__init__.py
--rw-rw-rw-   0        0        0     1110 2024-04-30 04:27:30.000000 ncmlistdownloader-2.0.0.240516a1/ncmlistdownloader/_old/downloader/json_list_io.py
-drwxrwxrwx   0        0        0        0 2024-05-16 15:00:08.621712 ncmlistdownloader-2.0.0.240516a1/ncmlistdownloader/_old/editer/
--rw-rw-rw-   0        0        0     4034 2024-05-05 14:27:08.000000 ncmlistdownloader-2.0.0.240516a1/ncmlistdownloader/_old/editer/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-16 15:00:08.627972 ncmlistdownloader-2.0.0.240516a1/ncmlistdownloader/_old/playlist/
--rw-rw-rw-   0        0        0     2296 2024-04-29 10:19:56.000000 ncmlistdownloader-2.0.0.240516a1/ncmlistdownloader/_old/playlist/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-16 15:00:08.630956 ncmlistdownloader-2.0.0.240516a1/ncmlistdownloader/_old/song/
--rw-rw-rw-   0        0        0     9580 2024-05-05 14:27:08.000000 ncmlistdownloader-2.0.0.240516a1/ncmlistdownloader/_old/song/__init__.py
--rw-rw-rw-   0        0        0     1923 2024-05-16 14:59:42.000000 ncmlistdownloader-2.0.0.240516a1/ncmlistdownloader/global_args.py
-drwxrwxrwx   0        0        0        0 2024-05-16 15:00:08.634945 ncmlistdownloader-2.0.0.240516a1/ncmlistdownloader/music/
--rw-rw-rw-   0        0        0        0 2024-05-16 14:33:24.000000 ncmlistdownloader-2.0.0.240516a1/ncmlistdownloader/music/__init__.py
--rw-rw-rw-   0        0        0        0 2024-05-16 14:33:48.000000 ncmlistdownloader-2.0.0.240516a1/ncmlistdownloader/music/multiple_tools.py
-drwxrwxrwx   0        0        0        0 2024-05-16 15:00:08.636940 ncmlistdownloader-2.0.0.240516a1/ncmlistdownloader.egg-info/
--rw-rw-rw-   0        0        0     1297 2024-05-16 15:00:08.000000 ncmlistdownloader-2.0.0.240516a1/ncmlistdownloader.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      949 2024-05-16 15:00:08.000000 ncmlistdownloader-2.0.0.240516a1/ncmlistdownloader.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-16 15:00:08.000000 ncmlistdownloader-2.0.0.240516a1/ncmlistdownloader.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       37 2024-05-16 15:00:08.000000 ncmlistdownloader-2.0.0.240516a1/ncmlistdownloader.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2024-05-16 15:00:08.000000 ncmlistdownloader-2.0.0.240516a1/ncmlistdownloader.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-16 15:00:08.639268 ncmlistdownloader-2.0.0.240516a1/setup.cfg
--rw-rw-rw-   0        0        0     1811 2024-05-16 14:32:18.000000 ncmlistdownloader-2.0.0.240516a1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-17 15:02:58.261834 ncmlistdownloader-2.0.0.240517a1/
+-rw-rw-rw-   0        0        0    35181 2024-05-16 14:27:24.000000 ncmlistdownloader-2.0.0.240517a1/LICENSE
+-rw-rw-rw-   0        0        0     1297 2024-05-17 15:02:58.259837 ncmlistdownloader-2.0.0.240517a1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-17 15:02:58.086303 ncmlistdownloader-2.0.0.240517a1/ncmlistdownloader/
+-rw-rw-rw-   0        0        0        0 2024-05-17 14:52:19.000000 ncmlistdownloader-2.0.0.240517a1/ncmlistdownloader/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-17 15:02:58.181050 ncmlistdownloader-2.0.0.240517a1/ncmlistdownloader/_old/
+-rw-rw-rw-   0        0        0     1880 2024-05-17 14:52:19.000000 ncmlistdownloader-2.0.0.240517a1/ncmlistdownloader/_old/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-17 15:02:58.199002 ncmlistdownloader-2.0.0.240517a1/ncmlistdownloader/_old/cmd/
+-rw-rw-rw-   0        0        0     1789 2024-05-17 14:52:19.000000 ncmlistdownloader-2.0.0.240517a1/ncmlistdownloader/_old/cmd/__init__.py
+-rw-rw-rw-   0        0        0      651 2024-05-17 14:52:19.000000 ncmlistdownloader-2.0.0.240517a1/ncmlistdownloader/_old/cmd/common.py
+-rw-rw-rw-   0        0        0     1685 2024-05-17 14:52:19.000000 ncmlistdownloader-2.0.0.240517a1/ncmlistdownloader/_old/cmd/download.py
+-rw-rw-rw-   0        0        0     2689 2024-05-17 14:52:19.000000 ncmlistdownloader-2.0.0.240517a1/ncmlistdownloader/_old/cmd/find_from_id.py
+-rw-rw-rw-   0        0        0     1664 2024-05-17 14:52:19.000000 ncmlistdownloader-2.0.0.240517a1/ncmlistdownloader/_old/cmd/json_io.py
+drwxrwxrwx   0        0        0        0 2024-05-17 15:02:58.226926 ncmlistdownloader-2.0.0.240517a1/ncmlistdownloader/_old/common/
+-rw-rw-rw-   0        0        0     2862 2024-05-17 14:52:19.000000 ncmlistdownloader-2.0.0.240517a1/ncmlistdownloader/_old/common/__init__.py
+-rw-rw-rw-   0        0        0     2161 2024-05-17 14:52:19.000000 ncmlistdownloader-2.0.0.240517a1/ncmlistdownloader/_old/common/encode_sec_key.py
+-rw-rw-rw-   0        0        0     1791 2024-05-17 14:52:19.000000 ncmlistdownloader-2.0.0.240517a1/ncmlistdownloader/_old/common/thread_test.py
+drwxrwxrwx   0        0        0        0 2024-05-17 15:02:58.233908 ncmlistdownloader-2.0.0.240517a1/ncmlistdownloader/_old/downloader/
+-rw-rw-rw-   0        0        0     6233 2024-05-17 14:52:19.000000 ncmlistdownloader-2.0.0.240517a1/ncmlistdownloader/_old/downloader/__init__.py
+-rw-rw-rw-   0        0        0     1110 2024-05-17 14:52:19.000000 ncmlistdownloader-2.0.0.240517a1/ncmlistdownloader/_old/downloader/json_list_io.py
+drwxrwxrwx   0        0        0        0 2024-05-17 15:02:58.236900 ncmlistdownloader-2.0.0.240517a1/ncmlistdownloader/_old/editer/
+-rw-rw-rw-   0        0        0     4034 2024-05-17 14:52:19.000000 ncmlistdownloader-2.0.0.240517a1/ncmlistdownloader/_old/editer/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-17 15:02:58.241888 ncmlistdownloader-2.0.0.240517a1/ncmlistdownloader/_old/playlist/
+-rw-rw-rw-   0        0        0     2296 2024-05-17 14:52:19.000000 ncmlistdownloader-2.0.0.240517a1/ncmlistdownloader/_old/playlist/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-17 15:02:58.245875 ncmlistdownloader-2.0.0.240517a1/ncmlistdownloader/_old/song/
+-rw-rw-rw-   0        0        0     9580 2024-05-17 14:52:19.000000 ncmlistdownloader-2.0.0.240517a1/ncmlistdownloader/_old/song/__init__.py
+-rw-rw-rw-   0        0        0     2151 2024-05-17 15:02:21.000000 ncmlistdownloader-2.0.0.240517a1/ncmlistdownloader/encode.py
+-rw-rw-rw-   0        0        0     1923 2024-05-17 15:02:39.000000 ncmlistdownloader-2.0.0.240517a1/ncmlistdownloader/global_args.py
+drwxrwxrwx   0        0        0        0 2024-05-17 15:02:58.249865 ncmlistdownloader-2.0.0.240517a1/ncmlistdownloader/music/
+-rw-rw-rw-   0        0        0        0 2024-05-17 14:52:19.000000 ncmlistdownloader-2.0.0.240517a1/ncmlistdownloader/music/__init__.py
+-rw-rw-rw-   0        0        0        0 2024-05-17 14:52:19.000000 ncmlistdownloader-2.0.0.240517a1/ncmlistdownloader/music/multiple_tools.py
+drwxrwxrwx   0        0        0        0 2024-05-17 15:02:58.254853 ncmlistdownloader-2.0.0.240517a1/ncmlistdownloader.egg-info/
+-rw-rw-rw-   0        0        0     1297 2024-05-17 15:02:58.000000 ncmlistdownloader-2.0.0.240517a1/ncmlistdownloader.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      977 2024-05-17 15:02:58.000000 ncmlistdownloader-2.0.0.240517a1/ncmlistdownloader.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-17 15:02:58.000000 ncmlistdownloader-2.0.0.240517a1/ncmlistdownloader.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       37 2024-05-17 15:02:58.000000 ncmlistdownloader-2.0.0.240517a1/ncmlistdownloader.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2024-05-17 15:02:58.000000 ncmlistdownloader-2.0.0.240517a1/ncmlistdownloader.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-17 15:02:58.261834 ncmlistdownloader-2.0.0.240517a1/setup.cfg
+-rw-rw-rw-   0        0        0     1811 2024-05-17 15:02:47.000000 ncmlistdownloader-2.0.0.240517a1/setup.py
```

### Comparing `ncmlistdownloader-2.0.0.240516a1/LICENSE` & `ncmlistdownloader-2.0.0.240517a1/LICENSE`

 * *Files identical despite different names*

### Comparing `ncmlistdownloader-2.0.0.240516a1/PKG-INFO` & `ncmlistdownloader-2.0.0.240517a1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ncmlistdownloader
-Version: 2.0.0.240516a1
+Version: 2.0.0.240517a1
 Summary: 获取网易云音乐歌单数据，下载音乐，主动添加元信息。
 Home-page: https://gitee.com/Cooooldwind/163ListDownloader_NexT
 Author: CooooldWind_
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Customer Service
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: End Users/Desktop
```

### Comparing `ncmlistdownloader-2.0.0.240516a1/ncmlistdownloader/_old/__init__.py` & `ncmlistdownloader-2.0.0.240517a1/ncmlistdownloader/_old/__init__.py`

 * *Files identical despite different names*

### Comparing `ncmlistdownloader-2.0.0.240516a1/ncmlistdownloader/_old/cmd/__init__.py` & `ncmlistdownloader-2.0.0.240517a1/ncmlistdownloader/_old/cmd/__init__.py`

 * *Files identical despite different names*

### Comparing `ncmlistdownloader-2.0.0.240516a1/ncmlistdownloader/_old/cmd/common.py` & `ncmlistdownloader-2.0.0.240517a1/ncmlistdownloader/_old/cmd/common.py`

 * *Files identical despite different names*

### Comparing `ncmlistdownloader-2.0.0.240516a1/ncmlistdownloader/_old/cmd/download.py` & `ncmlistdownloader-2.0.0.240517a1/ncmlistdownloader/_old/cmd/download.py`

 * *Files identical despite different names*

### Comparing `ncmlistdownloader-2.0.0.240516a1/ncmlistdownloader/_old/cmd/find_from_id.py` & `ncmlistdownloader-2.0.0.240517a1/ncmlistdownloader/_old/cmd/find_from_id.py`

 * *Files identical despite different names*

### Comparing `ncmlistdownloader-2.0.0.240516a1/ncmlistdownloader/_old/cmd/json_io.py` & `ncmlistdownloader-2.0.0.240517a1/ncmlistdownloader/_old/cmd/json_io.py`

 * *Files identical despite different names*

### Comparing `ncmlistdownloader-2.0.0.240516a1/ncmlistdownloader/_old/common/__init__.py` & `ncmlistdownloader-2.0.0.240517a1/ncmlistdownloader/_old/common/__init__.py`

 * *Files identical despite different names*

### Comparing `ncmlistdownloader-2.0.0.240516a1/ncmlistdownloader/_old/common/encode_sec_key.py` & `ncmlistdownloader-2.0.0.240517a1/ncmlistdownloader/_old/common/encode_sec_key.py`

 * *Files identical despite different names*

### Comparing `ncmlistdownloader-2.0.0.240516a1/ncmlistdownloader/_old/common/thread_test.py` & `ncmlistdownloader-2.0.0.240517a1/ncmlistdownloader/_old/common/thread_test.py`

 * *Files identical despite different names*

### Comparing `ncmlistdownloader-2.0.0.240516a1/ncmlistdownloader/_old/downloader/__init__.py` & `ncmlistdownloader-2.0.0.240517a1/ncmlistdownloader/_old/downloader/__init__.py`

 * *Files identical despite different names*

### Comparing `ncmlistdownloader-2.0.0.240516a1/ncmlistdownloader/_old/downloader/json_list_io.py` & `ncmlistdownloader-2.0.0.240517a1/ncmlistdownloader/_old/downloader/json_list_io.py`

 * *Files identical despite different names*

### Comparing `ncmlistdownloader-2.0.0.240516a1/ncmlistdownloader/_old/editer/__init__.py` & `ncmlistdownloader-2.0.0.240517a1/ncmlistdownloader/_old/editer/__init__.py`

 * *Files identical despite different names*

### Comparing `ncmlistdownloader-2.0.0.240516a1/ncmlistdownloader/_old/playlist/__init__.py` & `ncmlistdownloader-2.0.0.240517a1/ncmlistdownloader/_old/playlist/__init__.py`

 * *Files identical despite different names*

### Comparing `ncmlistdownloader-2.0.0.240516a1/ncmlistdownloader/_old/song/__init__.py` & `ncmlistdownloader-2.0.0.240517a1/ncmlistdownloader/_old/song/__init__.py`

 * *Files identical despite different names*

### Comparing `ncmlistdownloader-2.0.0.240516a1/ncmlistdownloader/global_args.py` & `ncmlistdownloader-2.0.0.240517a1/ncmlistdownloader/global_args.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 Following GNU_AGPLV3+ License
 """
 
 _CORE_VERSION_TUPLE = (
     "2",
     "0",
     "0",
-    "240516",
+    "240517",
     "3",
     "1",
 )
 
 # Don't touch codes below if unnecessary!
 FUNC_F = "00e0b509f6259df8642dbc35662901477df22677ec152b5ff68ace615bb7b725152b3ab17a876aea8a5aa76d2e417629ec4ee341f56135fccf695280104e0312ecbda92557c93870114af6c9d05c4f7f0c3685b7a46bee255932575cce10b424d813cfe4875d3e82047b97ddef52741d546b8e289dc6935b3ece0462db0a22b8e7"
 LYRIC_API = "https://music.163.com/weapi/song/lyric?csrf_token="
```

### Comparing `ncmlistdownloader-2.0.0.240516a1/ncmlistdownloader.egg-info/PKG-INFO` & `ncmlistdownloader-2.0.0.240517a1/ncmlistdownloader.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ncmlistdownloader
-Version: 2.0.0.240516a1
+Version: 2.0.0.240517a1
 Summary: 获取网易云音乐歌单数据，下载音乐，主动添加元信息。
 Home-page: https://gitee.com/Cooooldwind/163ListDownloader_NexT
 Author: CooooldWind_
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Customer Service
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: End Users/Desktop
```

### Comparing `ncmlistdownloader-2.0.0.240516a1/ncmlistdownloader.egg-info/SOURCES.txt` & `ncmlistdownloader-2.0.0.240517a1/ncmlistdownloader.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 LICENSE
 setup.py
 ncmlistdownloader/__init__.py
+ncmlistdownloader/encode.py
 ncmlistdownloader/global_args.py
 ncmlistdownloader.egg-info/PKG-INFO
 ncmlistdownloader.egg-info/SOURCES.txt
 ncmlistdownloader.egg-info/dependency_links.txt
 ncmlistdownloader.egg-info/requires.txt
 ncmlistdownloader.egg-info/top_level.txt
 ncmlistdownloader/_old/__init__.py
```

### Comparing `ncmlistdownloader-2.0.0.240516a1/setup.py` & `ncmlistdownloader-2.0.0.240517a1/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 
 # from ncmlistdownloader.common.global_args import CORE_VERSION_SETUP
 setup(
     classifiers=[
         # 发展时期
-        'Development Status :: 3 - Alpha',
+        "Development Status :: 3 - Alpha",
         # 'Development Status :: 4 - Beta',
         # "Development Status :: 5 - Production/Stable",
         # 开发的目标用户
         "Intended Audience :: Customer Service",
         "Intended Audience :: Developers",
         "Intended Audience :: End Users/Desktop",
         # 属于什么类型
@@ -26,15 +26,15 @@
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
         "Programming Language :: Python :: 3.12",
     ],
     name="ncmlistdownloader",
-    version="2.0.0.240516a1",
+    version="2.0.0.240517a1",
     description="获取网易云音乐歌单数据，下载音乐，主动添加元信息。",
     author="CooooldWind_",
     url="https://gitee.com/Cooooldwind/163ListDownloader_NexT",
     packages=find_packages(),
     install_requires=[
         "pycryptodome",
         "pillow",
```

