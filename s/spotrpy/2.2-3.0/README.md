# Comparing `tmp/spotrpy-2.2.tar.gz` & `tmp/spotrpy-3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spotrpy-2.2.tar", last modified: Mon Jan 15 17:02:49 2024, max compression
+gzip compressed data, was "spotrpy-3.0.tar", last modified: Sat May 18 13:48:55 2024, max compression
```

## Comparing `spotrpy-2.2.tar` & `spotrpy-3.0.tar`

### file list

```diff
@@ -1,44 +1,47 @@
-drwxr-xr-x   0 havard    (1000) havard    (1000)        0 2024-01-15 17:02:49.364420 spotrpy-2.2/
--rw-r--r--   0 havard    (1000) havard    (1000)     1065 2024-01-12 18:49:17.000000 spotrpy-2.2/LICENSE.md
--rw-r--r--   0 havard    (1000) havard    (1000)     4392 2024-01-15 17:02:49.364420 spotrpy-2.2/PKG-INFO
--rw-r--r--   0 havard    (1000) havard    (1000)     3766 2024-01-14 22:31:36.000000 spotrpy-2.2/README.md
--rw-r--r--   0 havard    (1000) havard    (1000)       38 2024-01-15 17:02:49.364420 spotrpy-2.2/setup.cfg
--rw-r--r--   0 havard    (1000) havard    (1000)     1039 2024-01-15 17:02:38.000000 spotrpy-2.2/setup.py
-drwxr-xr-x   0 havard    (1000) havard    (1000)        0 2024-01-15 17:02:49.360420 spotrpy-2.2/spotrpy/
-drwxr-xr-x   0 havard    (1000) havard    (1000)        0 2024-01-15 17:02:49.361420 spotrpy-2.2/spotrpy/Util/
--rw-r--r--   0 havard    (1000) havard    (1000)     4632 2024-01-14 22:31:36.000000 spotrpy-2.2/spotrpy/Util/API.py
--rw-r--r--   0 havard    (1000) havard    (1000)     2625 2024-01-14 22:31:36.000000 spotrpy-2.2/spotrpy/Util/ASCII.py
--rw-r--r--   0 havard    (1000) havard    (1000)     4929 2024-01-14 22:31:36.000000 spotrpy-2.2/spotrpy/Util/Configuration.py
--rw-r--r--   0 havard    (1000) havard    (1000)     4333 2024-01-15 17:00:08.000000 spotrpy-2.2/spotrpy/Util/Helpers.py
--rw-r--r--   0 havard    (1000) havard    (1000)      683 2024-01-14 22:31:36.000000 spotrpy-2.2/spotrpy/Util/Logging.py
--rw-r--r--   0 havard    (1000) havard    (1000)        0 2024-01-14 22:31:36.000000 spotrpy-2.2/spotrpy/Util/__init__.py
--rw-r--r--   0 havard    (1000) havard    (1000)        0 2024-01-12 18:49:17.000000 spotrpy-2.2/spotrpy/__init__.py
-drwxr-xr-x   0 havard    (1000) havard    (1000)        0 2024-01-15 17:02:49.363420 spotrpy-2.2/spotrpy/commands/
--rw-r--r--   0 havard    (1000) havard    (1000)        0 2024-01-14 22:31:36.000000 spotrpy-2.2/spotrpy/commands/__init__.py
--rw-r--r--   0 havard    (1000) havard    (1000)     1514 2024-01-14 22:31:36.000000 spotrpy-2.2/spotrpy/commands/ascii.py
--rw-r--r--   0 havard    (1000) havard    (1000)     4827 2024-01-15 16:43:41.000000 spotrpy-2.2/spotrpy/commands/current.py
--rw-r--r--   0 havard    (1000) havard    (1000)      667 2024-01-14 22:31:36.000000 spotrpy-2.2/spotrpy/commands/next.py
--rw-r--r--   0 havard    (1000) havard    (1000)      992 2024-01-15 16:43:34.000000 spotrpy-2.2/spotrpy/commands/playback.py
--rw-r--r--   0 havard    (1000) havard    (1000)     1425 2024-01-15 16:43:17.000000 spotrpy-2.2/spotrpy/commands/playlist.py
--rw-r--r--   0 havard    (1000) havard    (1000)     1749 2024-01-15 16:43:06.000000 spotrpy-2.2/spotrpy/commands/playlistadd.py
--rw-r--r--   0 havard    (1000) havard    (1000)      690 2024-01-14 22:31:36.000000 spotrpy-2.2/spotrpy/commands/previous.py
--rw-r--r--   0 havard    (1000) havard    (1000)     1040 2024-01-15 16:47:44.000000 spotrpy-2.2/spotrpy/commands/qsearch.py
--rw-r--r--   0 havard    (1000) havard    (1000)      821 2024-01-14 22:31:36.000000 spotrpy-2.2/spotrpy/commands/queue.py
--rw-r--r--   0 havard    (1000) havard    (1000)     1477 2024-01-15 16:38:45.000000 spotrpy-2.2/spotrpy/commands/recent.py
--rw-r--r--   0 havard    (1000) havard    (1000)     1849 2024-01-15 16:42:04.000000 spotrpy-2.2/spotrpy/commands/recommend.py
--rw-r--r--   0 havard    (1000) havard    (1000)      755 2024-01-15 16:40:53.000000 spotrpy-2.2/spotrpy/commands/replay.py
--rw-r--r--   0 havard    (1000) havard    (1000)     3975 2024-01-15 16:40:43.000000 spotrpy-2.2/spotrpy/commands/search.py
--rw-r--r--   0 havard    (1000) havard    (1000)      823 2024-01-15 16:40:17.000000 spotrpy-2.2/spotrpy/commands/seek.py
--rw-r--r--   0 havard    (1000) havard    (1000)      972 2024-01-15 16:40:01.000000 spotrpy-2.2/spotrpy/commands/shuffle.py
--rw-r--r--   0 havard    (1000) havard    (1000)      680 2024-01-15 16:39:37.000000 spotrpy-2.2/spotrpy/commands/start.py
--rw-r--r--   0 havard    (1000) havard    (1000)      673 2024-01-15 16:39:36.000000 spotrpy-2.2/spotrpy/commands/stop.py
--rw-r--r--   0 havard    (1000) havard    (1000)     1287 2024-01-15 16:44:08.000000 spotrpy-2.2/spotrpy/commands/volume.py
--rw-r--r--   0 havard    (1000) havard    (1000)      879 2024-01-15 16:44:05.000000 spotrpy-2.2/spotrpy/commands/web.py
--rwxr-xr-x   0 havard    (1000) havard    (1000)     1424 2024-01-14 22:31:36.000000 spotrpy-2.2/spotrpy/spotr.py
-drwxr-xr-x   0 havard    (1000) havard    (1000)        0 2024-01-15 17:02:49.364420 spotrpy-2.2/spotrpy.egg-info/
--rw-r--r--   0 havard    (1000) havard    (1000)     4392 2024-01-15 17:02:49.000000 spotrpy-2.2/spotrpy.egg-info/PKG-INFO
--rw-r--r--   0 havard    (1000) havard    (1000)      946 2024-01-15 17:02:49.000000 spotrpy-2.2/spotrpy.egg-info/SOURCES.txt
--rw-r--r--   0 havard    (1000) havard    (1000)        1 2024-01-15 17:02:49.000000 spotrpy-2.2/spotrpy.egg-info/dependency_links.txt
--rw-r--r--   0 havard    (1000) havard    (1000)       45 2024-01-15 17:02:49.000000 spotrpy-2.2/spotrpy.egg-info/entry_points.txt
--rw-r--r--   0 havard    (1000) havard    (1000)       77 2024-01-15 17:02:49.000000 spotrpy-2.2/spotrpy.egg-info/requires.txt
--rw-r--r--   0 havard    (1000) havard    (1000)        8 2024-01-15 17:02:49.000000 spotrpy-2.2/spotrpy.egg-info/top_level.txt
+drwxr-xr-x   0 ibanez    (1000) ibanez    (1000)        0 2024-05-18 13:48:55.132084 spotrpy-3.0/
+-rw-r--r--   0 ibanez    (1000) ibanez    (1000)     1065 2024-05-15 22:06:04.000000 spotrpy-3.0/LICENSE.md
+-rw-r--r--   0 ibanez    (1000) ibanez    (1000)     4364 2024-05-18 13:48:55.130084 spotrpy-3.0/PKG-INFO
+-rw-r--r--   0 ibanez    (1000) ibanez    (1000)     3766 2024-05-15 22:06:04.000000 spotrpy-3.0/README.md
+-rw-r--r--   0 ibanez    (1000) ibanez    (1000)       38 2024-05-18 13:48:55.132084 spotrpy-3.0/setup.cfg
+-rw-r--r--   0 ibanez    (1000) ibanez    (1000)     1011 2024-05-18 13:37:52.000000 spotrpy-3.0/setup.py
+drwxr-xr-x   0 ibanez    (1000) ibanez    (1000)        0 2024-05-18 13:48:55.125084 spotrpy-3.0/spotrpy/
+-rw-r--r--   0 ibanez    (1000) ibanez    (1000)      341 2024-05-18 13:25:20.000000 spotrpy-3.0/spotrpy/LOGO.py
+drwxr-xr-x   0 ibanez    (1000) ibanez    (1000)        0 2024-05-18 13:48:55.125084 spotrpy-3.0/spotrpy/Util/
+-rw-r--r--   0 ibanez    (1000) ibanez    (1000)     4485 2024-05-18 13:16:42.000000 spotrpy-3.0/spotrpy/Util/API.py
+-rw-r--r--   0 ibanez    (1000) ibanez    (1000)     2373 2024-05-18 13:15:25.000000 spotrpy-3.0/spotrpy/Util/ASCII.py
+-rw-r--r--   0 ibanez    (1000) ibanez    (1000)     3043 2024-05-18 13:47:09.000000 spotrpy-3.0/spotrpy/Util/Configuration.py
+-rw-r--r--   0 ibanez    (1000) ibanez    (1000)     1747 2024-05-18 13:16:02.000000 spotrpy-3.0/spotrpy/Util/Helpers.py
+-rw-r--r--   0 ibanez    (1000) ibanez    (1000)      714 2024-05-18 13:15:55.000000 spotrpy-3.0/spotrpy/Util/Logging.py
+-rw-r--r--   0 ibanez    (1000) ibanez    (1000)        0 2024-05-15 22:06:04.000000 spotrpy-3.0/spotrpy/Util/__init__.py
+-rw-r--r--   0 ibanez    (1000) ibanez    (1000)        0 2024-05-15 22:06:04.000000 spotrpy-3.0/spotrpy/__init__.py
+drwxr-xr-x   0 ibanez    (1000) ibanez    (1000)        0 2024-05-18 13:48:55.130084 spotrpy-3.0/spotrpy/commands/
+-rw-r--r--   0 ibanez    (1000) ibanez    (1000)        0 2024-05-18 13:12:56.000000 spotrpy-3.0/spotrpy/commands/__init__.py
+-rw-r--r--   0 ibanez    (1000) ibanez    (1000)     1185 2024-05-18 13:20:31.000000 spotrpy-3.0/spotrpy/commands/ascii.py
+-rw-r--r--   0 ibanez    (1000) ibanez    (1000)      580 2024-05-18 13:20:30.000000 spotrpy-3.0/spotrpy/commands/auth.py
+-rw-r--r--   0 ibanez    (1000) ibanez    (1000)     4669 2024-05-18 13:20:28.000000 spotrpy-3.0/spotrpy/commands/current.py
+-rw-r--r--   0 ibanez    (1000) ibanez    (1000)      368 2024-05-18 13:20:27.000000 spotrpy-3.0/spotrpy/commands/next.py
+-rw-r--r--   0 ibanez    (1000) ibanez    (1000)      938 2024-05-18 13:19:08.000000 spotrpy-3.0/spotrpy/commands/playback.py
+-rw-r--r--   0 ibanez    (1000) ibanez    (1000)     1122 2024-05-18 13:20:22.000000 spotrpy-3.0/spotrpy/commands/playlist.py
+-rw-r--r--   0 ibanez    (1000) ibanez    (1000)     1271 2024-05-18 13:20:34.000000 spotrpy-3.0/spotrpy/commands/playlistadd.py
+-rw-r--r--   0 ibanez    (1000) ibanez    (1000)      384 2024-05-18 13:20:35.000000 spotrpy-3.0/spotrpy/commands/previous.py
+-rw-r--r--   0 ibanez    (1000) ibanez    (1000)      839 2024-05-18 13:20:37.000000 spotrpy-3.0/spotrpy/commands/qsearch.py
+-rw-r--r--   0 ibanez    (1000) ibanez    (1000)      494 2024-05-18 13:20:39.000000 spotrpy-3.0/spotrpy/commands/queue.py
+-rw-r--r--   0 ibanez    (1000) ibanez    (1000)     1147 2024-05-18 13:20:41.000000 spotrpy-3.0/spotrpy/commands/recent.py
+-rw-r--r--   0 ibanez    (1000) ibanez    (1000)     1456 2024-05-18 13:20:43.000000 spotrpy-3.0/spotrpy/commands/recommend.py
+-rw-r--r--   0 ibanez    (1000) ibanez    (1000)      442 2024-05-18 13:20:44.000000 spotrpy-3.0/spotrpy/commands/replay.py
+-rw-r--r--   0 ibanez    (1000) ibanez    (1000)     3666 2024-05-18 13:20:46.000000 spotrpy-3.0/spotrpy/commands/search.py
+-rw-r--r--   0 ibanez    (1000) ibanez    (1000)      585 2024-05-18 13:20:49.000000 spotrpy-3.0/spotrpy/commands/seek.py
+-rw-r--r--   0 ibanez    (1000) ibanez    (1000)      924 2024-05-18 13:20:52.000000 spotrpy-3.0/spotrpy/commands/shuffle.py
+-rw-r--r--   0 ibanez    (1000) ibanez    (1000)      374 2024-05-18 13:20:54.000000 spotrpy-3.0/spotrpy/commands/start.py
+-rw-r--r--   0 ibanez    (1000) ibanez    (1000)      371 2024-05-18 13:20:56.000000 spotrpy-3.0/spotrpy/commands/stop.py
+-rw-r--r--   0 ibanez    (1000) ibanez    (1000)      965 2024-05-18 13:20:58.000000 spotrpy-3.0/spotrpy/commands/volume.py
+-rw-r--r--   0 ibanez    (1000) ibanez    (1000)      536 2024-05-18 13:20:59.000000 spotrpy-3.0/spotrpy/commands/web.py
+-rw-r--r--   0 ibanez    (1000) ibanez    (1000)     1768 2024-05-18 13:27:46.000000 spotrpy-3.0/spotrpy/main.py
+-rwxr-xr-x   0 ibanez    (1000) ibanez    (1000)      394 2024-05-18 13:25:38.000000 spotrpy-3.0/spotrpy/spotr.py
+drwxr-xr-x   0 ibanez    (1000) ibanez    (1000)        0 2024-05-18 13:48:55.130084 spotrpy-3.0/spotrpy.egg-info/
+-rw-r--r--   0 ibanez    (1000) ibanez    (1000)     4364 2024-05-18 13:48:55.000000 spotrpy-3.0/spotrpy.egg-info/PKG-INFO
+-rw-r--r--   0 ibanez    (1000) ibanez    (1000)     1003 2024-05-18 13:48:55.000000 spotrpy-3.0/spotrpy.egg-info/SOURCES.txt
+-rw-r--r--   0 ibanez    (1000) ibanez    (1000)        1 2024-05-18 13:48:55.000000 spotrpy-3.0/spotrpy.egg-info/dependency_links.txt
+-rw-r--r--   0 ibanez    (1000) ibanez    (1000)       44 2024-05-18 13:48:55.000000 spotrpy-3.0/spotrpy.egg-info/entry_points.txt
+-rw-r--r--   0 ibanez    (1000) ibanez    (1000)       77 2024-05-18 13:48:55.000000 spotrpy-3.0/spotrpy.egg-info/requires.txt
+-rw-r--r--   0 ibanez    (1000) ibanez    (1000)        8 2024-05-18 13:48:55.000000 spotrpy-3.0/spotrpy.egg-info/top_level.txt
```

### Comparing `spotrpy-2.2/LICENSE.md` & `spotrpy-3.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `spotrpy-2.2/PKG-INFO` & `spotrpy-3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 Metadata-Version: 2.1
 Name: spotrpy
-Version: 2.2
+Version: 3.0
 Summary: A simple spotify tool for the terminal
 Home-page: https://github.com/Havard03/spotr
 Author: Havard03
 Author-email: havard.buvang@gmail.com
 Keywords: cli
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: POSIX
-Classifier: Operating System :: Unix
+Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 Requires-Dist: Pillow==10.1.0
 Requires-Dist: questionary==2.0.1
 Requires-Dist: requests==2.28.1
 Requires-Dist: rich==13.6.0
```

#### html2text {}

```diff
@@ -1,16 +1,15 @@
-Metadata-Version: 2.1 Name: spotrpy Version: 2.2 Summary: A simple spotify tool
+Metadata-Version: 2.1 Name: spotrpy Version: 3.0 Summary: A simple spotify tool
 for the terminal Home-page: https://github.com/Havard03/spotr Author: Havard03
 Author-email: havard.buvang@gmail.com Keywords: cli Classifier: Programming
 Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: POSIX Classifier: Operating System :: Unix
-Requires-Python: >=3.6 Description-Content-Type: text/markdown License-File:
-LICENSE.md Requires-Dist: Pillow==10.1.0 Requires-Dist: questionary==2.0.1
-Requires-Dist: requests==2.28.1 Requires-Dist: rich==13.6.0 Requires-Dist:
-tqdm==4.66.1
+Classifier: Operating System :: OS Independent Requires-Python: >=3.6
+Description-Content-Type: text/markdown License-File: LICENSE.md Requires-Dist:
+Pillow==10.1.0 Requires-Dist: questionary==2.0.1 Requires-Dist:
+requests==2.28.1 Requires-Dist: rich==13.6.0 Requires-Dist: tqdm==4.66.1
              ************ SSppoottrr -- AA ssppoottiiffyy ttooooll ffoorr tthhee tteerrmmiinnaall ************
  _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_g_i_t_h_u_b_/_c_o_n_t_r_i_b_u_t_o_r_s_/_H_a_v_a_r_d_0_3_/_s_p_o_t_r_._s_v_g_?_s_t_y_l_e_=_f_o_r_-_t_h_e_-
  _b_a_d_g_e_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_g_i_t_h_u_b_/_f_o_r_k_s_/_H_a_v_a_r_d_0_3_/_s_p_o_t_r_._s_v_g_?_s_t_y_l_e_=_f_o_r_-_t_h_e_-
  _b_a_d_g_e_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_g_i_t_h_u_b_/_s_t_a_r_s_/_H_a_v_a_r_d_0_3_/_s_p_o_t_r_._s_v_g_?_s_t_y_l_e_=_f_o_r_-_t_h_e_-
  _b_a_d_g_e_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_g_i_t_h_u_b_/_i_s_s_u_e_s_/_H_a_v_a_r_d_0_3_/_s_p_o_t_r_._s_v_g_?_s_t_y_l_e_=_f_o_r_-_t_h_e_-
 _b_a_d_g_e_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_g_i_t_h_u_b_/_l_i_c_e_n_s_e_/_H_a_v_a_r_d_0_3_/_s_p_o_t_r_._s_v_g_?_s_t_y_l_e_=_f_o_r_-_t_h_e_-
                                     _b_a_d_g_e_]
```

### Comparing `spotrpy-2.2/README.md` & `spotrpy-3.0/README.md`

 * *Files identical despite different names*

### Comparing `spotrpy-2.2/setup.py` & `spotrpy-3.0/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding = "utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='spotrpy',
-    version='2.2',
+    version='3.0',
     packages=find_packages(),
     python_requires = ">=3.6",
     author = "Havard03",
     author_email = "havard.buvang@gmail.com",
     description = "A simple spotify tool for the terminal",
     long_description = long_description,
     long_description_content_type = "text/markdown",
@@ -22,17 +22,16 @@
         'questionary==2.0.1',
         'requests==2.28.1',
         'rich==13.6.0',
         'tqdm==4.66.1',
     ],
     entry_points={
         'console_scripts': [
-            'spotr=spotrpy.spotr:main',
+            'spotr=spotrpy.main:main',
         ],
     },
     classifiers=[
         'Programming Language :: Python :: 3',
         'License :: OSI Approved :: MIT License',
-        'Operating System :: POSIX',
-        'Operating System :: Unix',
+        'Operating System :: OS Independent',
     ],
 )
```

### Comparing `spotrpy-2.2/spotrpy/Util/API.py` & `spotrpy-3.0/spotrpy/Util/API.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,117 +1,109 @@
-"""API class"""
-
 import base64
 import sys
-import time
-import webbrowser
 import requests
+
 from urllib.parse import urljoin
 
 class API:
-    """API class for sending all requests"""
+    """ API """
 
     def __initAPI__(self):
-        self.SPOTIFY_LIMIT = 50
-        self.QUSTIONARY_LIMIT = 36
-        self.API_VERSION = "v1"
-        self.API_BASE = "api.spotify.com"
-        self.ACCOUNT_URL = "https://accounts.spotify.com" 
-        self.API_PLAYER = urljoin("https://api.spotify.com", f"{self.API_VERSION}/me/player/")
-        self.API_BASE_VERSION = urljoin("https://api.spotify.com", f"{self.API_VERSION}/")
+        self.SPOTIFY_LIMIT      = 50
+        self.QUSTIONARY_LIMIT   = 36
+        self.API_VERSION        = "v1"
+        self.API_BASE           = "api.spotify.com"
+        self.ACCOUNT_URL        = "https://accounts.spotify.com" 
+        self.API_PLAYER         = urljoin("https://api.spotify.com", f"{self.API_VERSION}/me/player/")
+        self.API_BASE_VERSION   = urljoin("https://api.spotify.com", f"{self.API_VERSION}/")
 
     def request(
         self, 
         method,
         url,
         headers=None,
         json=None
     ):
-        """Spotr request, with deafult headers"""
-        if headers is None:
-            headers = {"Authorization": f"Bearer {self.CONFIG['key']}"}
+        """ Spotify API request """
 
+        if headers is None: headers = {"Authorization": f"Bearer {self.CONFIG['key']}"}
+        
         response = requests.request(method, url, headers=headers, json=json, timeout=10)
 
-        if response.status_code in (401, 400):
-            self.refresh_key()
-            headers = {"Authorization": f"Bearer {self.CONFIG['key']}"}
-            response = requests.request(method, url, headers=headers, json=json, timeout=10)
-
-        if not response.ok:
-            self.log.warning("[bold red]request error - status-code: %d", response.status_code)
-            self.log.info(response.json())
-            sys.exit()
-
         try:
             data = response.json()
         except ValueError:
-            return None
+            data = None
+
+        if not response.ok:
+            status_code = response.status_code
+
+            self.log.error(f"Requst error - {status_code}")
+            if data: self.log.debug(f"Request response - {data}")
+
+            if status_code in (401, 400):                
+                self.refresh_token()
+                
+                headers     = {"Authorization": f"Bearer {self.CONFIG['key']}"}
+                response    = requests.request(method, url, headers=headers, json=json, timeout=10)
 
         return data
-    
-    def play(self, json=None):
-        """Play song or collection of songs"""
-        self.request("PUT", str(urljoin(self.API_PLAYER, "play")), json=json)
 
-    def refresh_key(self):
-        """Refresh API key"""
+    def refresh_token(self):
+        """ Refresh Spotify API token """
+
+        self.log.debug(f"Refreshing API-Token")
         url = urljoin(self.ACCOUNT_URL, "api/token")
         
         response = requests.post(
             url,
             data={
                 "grant_type": "refresh_token",
                 "refresh_token": self.CONFIG["refresh_token"],
             },
             headers={"Authorization": "Basic " + self.CONFIG["base_64"]},
             timeout=10,
         )
+
         if not response.ok:
-            self.log.warning(
-                "[bold red]request error - status-code: %d",
-                response.status_code,
-            )
-            self.log.info(
-                "[bold blue]Most likely something wrong with base_64 or refresh_token, try running 'spotr authorise'"
-            )
+            self.log.critical(f"Request error - status-code: {response.status_code}")
+            self.log.critical("Indication of invalid refresh_token, or base_64")
+
             sys.exit()
+
         data = response.json()
         self.CONFIG["key"] = data["access_token"]
         self.write_config()
 
-    def authorise(self):
-        """Authenticate with Spotify API"""
-        auth_url = urljoin(self.ACCOUNT_URL, "authorize")
+    def authorise(self, client_id=None, client_secret=None):
+        """ Authorise CLI with Spotify API """
+
+        auth_url  = urljoin(self.ACCOUNT_URL, "authorize")
         token_url = urljoin(self.ACCOUNT_URL, "api/token")
 
-        client_id = str(input("Spotify-App Client id: "))
-        client_secret = str(input("Spotify-App Client secret: "))
+        if not client_id: client_id         = str(input("Spotify-App Client id: "))
+        if not client_secret: client_secret = str(input("Spotify-App Client secret: "))
 
         auth_request = requests.get(
             auth_url,
             {
                 "client_id": client_id,
                 "response_type": "code",
                 "redirect_uri": "https://www.google.com/",
                 "scope": "playlist-read-collaborative playlist-read-private user-read-playback-state user-modify-playback-state user-read-currently-playing user-read-recently-played playlist-modify-private playlist-modify-public",
             },
             timeout=10,
         )
 
-        print(
-            "URL will open in 5 seconds, Accept the terms, Copy the code in the redirected URL, Then paste the code into the terminal"
-        )
-        time.sleep(5)
-        webbrowser.open_new_tab(auth_request.url)
-
-        auth_code = str(input("Enter code from the URL: "))
+        print("\nGo to the Following URL, Accept the terms, Copy the code in the redirected URL, Then paste the code into the terminal\n")
+        print(f"\n{auth_request.url}\n")
 
-        client_creds = f"{client_id}:{client_secret}"
-        client_creds_b64 = base64.b64encode(client_creds.encode())
+        auth_code           = str(input("Enter code from the URL: "))
+        client_creds        = f"{client_id}:{client_secret}"
+        client_creds_b64    = base64.b64encode(client_creds.encode())
 
         headers = {
             "Content-Type": "application/x-www-form-urlencoded",
             "Authorization": "Basic %s" % client_creds_b64.decode(),
         }
         payload = {
             "grant_type": "authorization_code",
@@ -123,13 +115,13 @@
             url=token_url, data=payload, headers=headers, timeout=10
         )
 
         if not access_token_request.ok:
             self.log.warning("Request error: %d", access_token_request.status_code)
             sys.exit()
 
-        access_token_response_data = access_token_request.json()
+        access_token_response_data      = access_token_request.json()
+        self.CONFIG["refresh_token"]    = access_token_response_data["refresh_token"]
+        self.CONFIG["base_64"]          = client_creds_b64.decode()
 
-        self.CONFIG["refresh_token"] = access_token_response_data["refresh_token"]
-        self.CONFIG["base_64"] = client_creds_b64.decode()
         self.write_config()
         print("All done!")
```

### Comparing `spotrpy-2.2/spotrpy/Util/ASCII.py` & `spotrpy-3.0/spotrpy/Util/ASCII.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,75 +1,69 @@
-""" ASCII """
+import requests
 
 from io import BytesIO
 from PIL import Image
-import requests
 
 class ASCII:
-    """ASCII class"""
+    """ ASCII class """
 
     def resize_image(self, image, new_width=100):
-        """Rezise image"""
-        width, height = image.size
-        ratio = height / width / 2.25
-        new_height = int(new_width * ratio)
-        resized_image = image.resize((new_width, new_height))
+        """ Rezise image """
+        
+        width, height   = image.size
+        ratio           = height / width / 2.25
+        new_height      = int(new_width * ratio)
+        resized_image   = image.resize((new_width, new_height))
+
         return resized_image
 
     def image_to_ascii(self, image_url, desired_width=75):
-        """Convert image to ascii"""
-
-        response = requests.get(image_url, timeout=10)
-        image_data = response.content
+        """ Convert image to ascii """
 
-        image = Image.open(BytesIO(image_data))
-        image = self.resize_image(image, desired_width)
+        response    = requests.get(image_url, timeout=10)
+        image_data  = response.content
+        image       = Image.open(BytesIO(image_data))
+        image       = self.resize_image(image, desired_width)
+        image       = image.convert("L")
+        pixels      = image.getdata()
+        ascii_str   = ""
+        ascii_art   = ""
 
-        image = image.convert("L")
-        pixels = image.getdata()
-        ascii_str = ""
-        ascii_art = ""
         for pixel_value in pixels:
             ascii_str += self.CONFIG["ASCII_IMAGE_CHARS"][
                 max(
                     0, min(pixel_value // 16, len(self.CONFIG["ASCII_IMAGE_CHARS"]) - 1)
                 )
             ]
+
         for i in range(0, len(ascii_str), int(desired_width)):
-            row = ascii_str[i : i + int(desired_width)]
-            ascii_art += row + "\n"
+            row         = ascii_str[i : i + int(desired_width)]
+            ascii_art   += row + "\n"
+
         return ascii_art
 
     def rgb_to_ansi(self, r, g, b):
-        """Convert RGB color values to ANSI color codes for console."""
+        """ Convert RGB color values to ANSI color codes for console """
+
         return f"\x1b[38;2;{r};{g};{b}m"
 
     def image_to_ascii_color(self, image_url, width=75):
-        """Convert image to ASCII art with color."""
+        """ Convert image to ASCII art with color """
         
-        response = requests.get(image_url, timeout=10)
-        image = Image.open(BytesIO(response.content))
-
-        aspect_ratio = image.height / image.width
-        new_height = int(width * aspect_ratio * 0.5)
-        resized_image = image.resize((width, new_height))
-        pixels = resized_image.convert("RGB").load()
+        response        = requests.get(image_url, timeout=10)
+        image           = Image.open(BytesIO(response.content))
+        aspect_ratio    = image.height / image.width
+        new_height      = int(width * aspect_ratio * 0.5)
+        resized_image   = image.resize((width, new_height))
+        pixels          = resized_image.convert("RGB").load()
+        ascii_art       = ""
 
-        ascii_art = ""
         for y in range(resized_image.height):
             for x in range(resized_image.width):
-                try:
-                    r, g, b, *_ = pixels[x, y]
-                except TypeError:
-                    LOG = (
-                        log.exception("Something went wrong with image convertion")
-                        if eval(self.CONFIG["DEBUG"])
-                        else log.error("Something went wrong with image convertion")
-                    )
-                    exit()
+                r, g, b, *_ = pixels[x, y]
                 char = "\u2588" if eval(self.CONFIG["ASCII_IMAGE_UNICODE"]) else "@"
                 ascii_art += self.rgb_to_ansi(r, g, b) + char
             if y != resized_image.height - 1:
                 ascii_art += "\n"
 
         ascii_art += "\x1b[0m"
```

### Comparing `spotrpy-2.2/spotrpy/Util/Logging.py` & `spotrpy-3.0/spotrpy/Util/Logging.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 import logging
 
 from rich.console import Console
 from rich.logging import RichHandler
 
 class Logging:
+    """ Logging """
 
     def __initLogging__(self):
         self.log = logging.getLogger()
         self.console = Console()
 
-        if eval(self.CONFIG["DEBUG"]):
+        if self.args.debug:
             logging.basicConfig(
                 level="NOTSET",
                 format="%(message)s",
                 datefmt="[%X]",
                 handlers=[RichHandler(markup=True, rich_tracebacks=True)],
             )
         else:
             logging.basicConfig(
                 level="INFO",
                 datefmt="[%X]",
                 format="%(message)s",
-                handlers=[RichHandler(markup=True)],
+                handlers=[RichHandler(markup=True, rich_tracebacks=True)],
             )
```

### Comparing `spotrpy-2.2/spotrpy/commands/current.py` & `spotrpy-3.0/spotrpy/commands/current.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,64 +1,52 @@
 import re
-import textwrap
 import time
+import textwrap
+
+from ..spotr import Spotr
 from urllib.parse import urljoin
 
-class Current():
-    """ Current class """
+class Current(Spotr):
+    """ Current """
+
+    description = "Display information about the currently playing track"
 
-    def __init__(self, spotr):
-        # Command info
-        self.info = {
-            'name': 'Current',
-            'description': 'Display information about the currently playing track',
-            'arguments': [],
-            'min_args': 0,
-            'max_args': 0,
-        }
-
-        # Data URL
-        self.URL = str(urljoin(spotr.API_PLAYER, "currently-playing"))
-
-        # Arguments passed
-        self.args = spotr.args
-
-        # Unpack form spotr instance
-        self.CONFIG = spotr.CONFIG
-        self.request = spotr.request
-        self.log = spotr.log
-        self.image_to_ascii = spotr.image_to_ascii
-        self.image_to_ascii_color = spotr.image_to_ascii_color
+    def __init__(self, args):
+        self.args = args
+        Spotr.__init__(self)
+
+    @staticmethod
+    def add_arguments(parser):
+        pass
 
     def execute(self):
-        """Display information about the currently playing track"""
-        data = self.request("GET", self.URL)
+        data = self.request("GET", urljoin(self.API_PLAYER, "currently-playing"))
 
         if data is None or data["item"] is None:
-            self.log.error("No data")
+            self.log.error(f'No data - {data}')
             return
 
         if data["currently_playing_type"] not in ("track"):
             self.log.error("Playing unsupported type - %s", data['currently_playing_type'])
             return
 
-        current_track = data["item"]
-        album_data = current_track["album"]
-        artist_names = ", ".join([artist["name"] for artist in current_track["artists"]])
-        track_duration_ms = current_track["duration_ms"]
-        track_duration_m, track_duration_s = divmod(track_duration_ms // 1000, 60)
-        progress_ms = data["progress_ms"]
-        progress_m, progress_s = divmod(progress_ms // 1000, 60)
-        track_id = current_track["id"]
-        track_name = current_track["name"]
-        track_type = album_data["album_type"]
-        album_name = album_data["name"]
-        track_release_date = album_data["release_date"]
-        track_url = current_track["external_urls"]["spotify"]
-        track_image = album_data["images"][0]["url"]
+        current_track                       = data["item"]
+        album_data                          = current_track["album"]
+        artist_names                        = ", ".join([artist["name"] for artist in current_track["artists"]])
+        track_duration_ms                   = current_track["duration_ms"]
+        track_duration_m, track_duration_s  = divmod(track_duration_ms // 1000, 60)
+        progress_ms                         = data["progress_ms"]
+        progress_m, progress_s              = divmod(progress_ms // 1000, 60)
+        track_id                            = current_track["id"]
+        track_name                          = current_track["name"]
+        track_type                          = album_data["album_type"]
+        album_name                          = album_data["name"]
+        track_release_date                  = album_data["release_date"]
+        track_url                           = current_track["external_urls"]["spotify"]
+        track_image                         = album_data["images"][0]["url"]
 
         color_start = "\x1b[{}m".format
         color_end = "\x1b[0m"
 
         strings = textwrap.dedent(
             f"""
         {color_start('31')}Current track{color_end}
@@ -67,17 +55,17 @@
         {color_start('37')}Artits{color_end}{color_start('32')}        -  {artist_names}{color_end}
         {color_start('37')}Duration{color_end}{color_start('32')}      -  {track_duration_m} minutes {track_duration_s} seconds{color_end}
         {color_start('37')}Progress{color_end}{color_start('32')}      -  {progress_m} minutes {progress_s} seconds{color_end}
         {color_start('37')}Release date{color_end}{color_start('32')}  -  {track_release_date}{color_end}
         {color_start('37')}From{color_end}{color_start('32')}          -  {track_type} - {album_name}{color_end}
         {color_start('31')}Track details{color_end}
         {color_start('32')}------------------------------{color_end}
-        {color_start('37')}Id{color_end}{color_start('32')}  - {track_id}{color_end}
-        {color_start('37')}URL{color_end}{color_start('32')} - {track_url}{color_end}
-        {color_start('37')}Image{color_end}{color_start('32')} - {track_image}{color_end}
+        {color_start('37')}Id{color_end}{color_start('32')}     - {track_id}{color_end}
+        {color_start('37')}URL{color_end}{color_start('32')}    - {track_url}{color_end}
+        {color_start('37')}Image{color_end}{color_start('32')}  - {track_image}{color_end}
         """
         )
 
         ansi_color_escape = re.compile(r"\x1b\[\d{1,2}m")
         strings_no_color = ansi_color_escape.sub("", strings)
         if not eval(self.CONFIG["ANSI_COLORS"]):
             strings = strings_no_color
```

### Comparing `spotrpy-2.2/spotrpy/commands/playback.py` & `spotrpy-3.0/spotrpy/commands/playback.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,39 +1,35 @@
 import questionary
+
+from ..spotr import Spotr
 from urllib.parse import urljoin, urlencode
 
-class Playback():
-    """ Playback class """
+class Playback(Spotr):
+    """ Playback """
+
+    description = "Set playback state"
 
-    def __init__(self, spotr):
-        # Command info
-        self.info = {
-            'name': 'Playback',
-            'description': 'Set playback state',
-            'arguments': [],
-            'min_args': 0,
-            'max_args': 0,
-        }
-
-        # Arguments passed
-        self.args = spotr.args
-
-        # Unpack form spotr instance
-        self.CONFIG = spotr.CONFIG
-        self.request = spotr.request
-        self.API_PLAYER = spotr.API_PLAYER
+    def __init__(self, args):
+        self.args = args
+        Spotr.__init__(self)
+
+    @staticmethod
+    def add_arguments(parser):
+        parser.add_argument(
+            '-s', '--state', type=str, choices=["track", "context", "off"], help="playback state"
+        )
 
     def execute(self):
-        """Set playback state"""
-        state = questionary.select(
-            "Choose a play state",
-            choices=["track", "context", "off"],
-            erase_when_done=True,
-            use_shortcuts=True,
-        ).ask()
+        if not self.args.state:
+            state = questionary.select(
+                "Choose a play state",
+                choices=["track", "context", "off"],
+                erase_when_done=True,
+                use_shortcuts=True,
+            ).ask()
+        else:
+            state = self.args.state
 
         if state is None:
             return
         
         self.request("PUT", str(f"{urljoin(self.API_PLAYER, 'repeat')}?{urlencode({'state': state})}"))
-
-
```

### Comparing `spotrpy-2.2/spotrpy/commands/playlist.py` & `spotrpy-3.0/spotrpy/commands/recent.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,53 +1,43 @@
 import questionary
+
+from ..spotr import Spotr
 from urllib.parse import urljoin, urlencode
 
-class Playlist():
-    """ Playlist class """
+class Recent(Spotr):
+    """ Recent """
+
+    description = "Select one of recently played tracks"
 
-    def __init__(self, spotr):
-        # Command info
-        self.info = {
-            'name': 'Playlist',
-            'description': 'Choose a playlist',
-            'arguments': [],
-            'min_args': 0,
-            'max_args': 0,
-        }
-
-        # Data URL
-        self.URL = str(f"{urljoin(spotr.API_BASE_VERSION, 'me/playlists')}?{urlencode({'limit': spotr.SPOTIFY_LIMIT})}")
-
-        # Arguments passed
-        self.args = spotr.args
-
-        # Unpack form spotr instance
-        self.CONFIG = spotr.CONFIG
-        self.request = spotr.request
-        self.parse_items = spotr.parse_items
-        self.play = spotr.play
+    def __init__(self, args):
+        self.args = args
+        Spotr.__init__(self)
+
+    @staticmethod
+    def add_arguments(parser):
+        pass
 
     def execute(self):
-        """Choose a playlist"""
-        data = self.request("GET", self.URL)
+        data = self.request("GET", f"{urljoin(self.API_PLAYER, 'recently-played')}?{urlencode({'limit' : self.QUSTIONARY_LIMIT})}")
 
         choices = self.parse_items(
             data,
             accessor=["items"],
-            return_value=["uri"],
-            name_value=["name"],
-            artists_value=False,
+            return_value=["track", "uri"],
+            name_value=["track", "name"],
+            artists_value=["track", "artists"],
         )
 
         selected = questionary.select(
-            "What playlist do you want to play?",
+            "What song do you want to play?",
             choices=choices,
             erase_when_done=True,
+            use_shortcuts=True,
             use_arrow_keys=True,
             use_jk_keys=False,
         ).ask()
+
         if selected is None:
             return
 
-        json = {"context_uri": selected, "offset": {"position": "0"}}
-        self.play(json=json)
-
+        json = {"uris": [selected]}
+        self.request("PUT", str(urljoin(self.API_PLAYER, "play")), json=json)
```

### Comparing `spotrpy-2.2/spotrpy/commands/playlistadd.py` & `spotrpy-3.0/spotrpy/commands/playlistadd.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,40 +1,28 @@
 import questionary
+
+from ..spotr import Spotr
 from urllib.parse import urljoin, urlencode
 
-class Playlistadd():
-    """ Playlistadd class """
+class Playlistadd(Spotr):
+    """ Playlistadd """
+
+    description = "Add currently playing track to a playlist"
 
-    def __init__(self, spotr):
-        # Command info
-        self.info = {
-            'name': 'PlaylistAdd',
-            'description': 'Add currently playing track to playlist',
-            'arguments': [],
-            'min_args': 0,
-            'max_args': 0,
-        }
-
-        # Data URL
-        self.DATA_URL = str(f"{urljoin(spotr.API_BASE_VERSION, 'me/playlists')}?{urlencode({'limit': spotr.SPOTIFY_LIMIT})}")
-        self.CURRENT_URL = str(urljoin(spotr.API_PLAYER, "currently-playing"))
-
-        # Arguments passed
-        self.args = spotr.args
-
-        # Unpack form spotr instance
-        self.CONFIG = spotr.CONFIG
-        self.request = spotr.request
-        self.parse_items = spotr.parse_items
-        self.API_BASE_VERSION = spotr.API_BASE_VERSION
+    def __init__(self, args):
+        self.args = args
+        Spotr.__init__(self)
+
+    @staticmethod
+    def add_arguments(parser):
+        pass
 
     def execute(self):
-        """Add currently playing track to playlist"""
-        data = self.request("GET", self.DATA_URL)
-        current_song = self.request("GET", self.CURRENT_URL)
+        data = self.request("GET", f"{urljoin(self.API_BASE_VERSION, 'me/playlists')}?{urlencode({'limit': self.SPOTIFY_LIMIT})}")
+        current_song = self.request("GET", urljoin(self.API_PLAYER, "currently-playing"))
 
         choices = self.parse_items(
             data,
             accessor=["items"],
             return_value=["id"],
             name_value=["name"],
             artists_value=False,
@@ -50,9 +38,8 @@
 
         if selected is None:
             return
 
         self.request(
             "POST",
             str(f"{urljoin(self.API_BASE_VERSION, f"playlists/{selected}/tracks")}?{urlencode({"uris": current_song["item"]["uri"]})}")
-        )
-
+        )
```

### Comparing `spotrpy-2.2/spotrpy/commands/qsearch.py` & `spotrpy-3.0/spotrpy/commands/qsearch.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,37 +1,29 @@
+from ..spotr import Spotr
 from urllib.parse import urljoin, urlencode
 
-class Qsearch():
-    """ Qsearch class """
+class Qsearch(Spotr):
+    """ Qsearch """
 
-    def __init__(self, spotr):
-        # Command info
-        self.info = {
-            'name': 'Qsearch (Quicksearch)',
-            'description': 'Quicksearch for tracks',
-            'arguments': ['Query...'],
-            'min_args': 1,
-            'max_args': 999,
-        }
-
-        # Arguments passed
-        self.args = spotr.args
-
-        # Unpack form spotr instance
-        self.CONFIG = spotr.CONFIG
-        self.request = spotr.request
-        self.play = spotr.play
-        self.API_BASE_VERSION = spotr.API_BASE_VERSION
+    description = "Quicksearch for tracks"
 
+    def __init__(self, args):
+        self.args = args
+        Spotr.__init__(self)
+
+    @staticmethod
+    def add_arguments(parser):
+        parser.add_argument(
+            'query', type=str, help="Search query", nargs='*'
+        )
 
-    def execute(self, *query):
-        """ Info """
+    def execute(self):
         data = self.request(
             "GET",
             str(
-                f"{urljoin(self.API_BASE_VERSION, 'search')}?{urlencode({'q': ' '.join(query), 'type': 'track', 'limit': 1})}"
+                f"{urljoin(self.API_BASE_VERSION, 'search')}?{urlencode({'q': ' '.join(self.args.query), 'type': 'track', 'limit': 1})}"
             ),
         )
-
         json_id = [data['tracks']['items'][0]['uri']]
         json = {"uris": json_id, "offset": {"position": "0"}}
-        self.play(json=json)
+
+        self.request("PUT", str(urljoin(self.API_PLAYER, "play")), json=json)
```

### Comparing `spotrpy-2.2/spotrpy/commands/recommend.py` & `spotrpy-3.0/spotrpy/commands/recommend.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,38 +1,26 @@
+from ..spotr import Spotr
 from urllib.parse import urljoin, urlencode
 
-class Recommend():
-    """ Recommend class """
+class Recommend(Spotr):
+    """ Recommend """
 
-    def __init__(self, spotr):
-        # Command info
-        self.info = {
-            'name': 'Recommend',
-            'description': 'Play random / recommended tracks based on recent tracks',
-            'arguments': [],
-            'min_args': 0,
-            'max_args': 0,
-        }
-
-        # Data URL
-        self.URL = str(f"{urljoin(spotr.API_PLAYER, 'recently-played')}?{urlencode({'limit': 5})}")
-
-        # Arguments passed
-        self.args = spotr.args
-
-        # Unpack form spotr instance
-        self.CONFIG = spotr.CONFIG
-        self.request = spotr.request
-        self.play = spotr.play
-        self.API_BASE_VERSION = spotr.API_BASE_VERSION
+    description = "Play random / recommended tracks based on recent tracks"
+
+    def __init__(self, args):
+        self.args = args
+        Spotr.__init__(self)
+
+    @staticmethod
+    def add_arguments(parser):
+        pass
 
     def execute(self):
-        """Play random / recommended tracks based on recent tracks"""
         recent = self.request(
-            "GET", self.URL
+            "GET", f"{urljoin(self.API_PLAYER, 'recently-played')}?{urlencode({'limit': 5})}"
         )
 
         seed_arists = []
         seed_generes = ["all"]
         seed_tracks = []
 
         for track in recent["items"]:
@@ -52,10 +40,8 @@
                 )}"
             ),
         )
         results = []
         for track in recommended["tracks"]:
             results.append(track["uri"])
         json = {"uris": results, "offset": {"position": "0"}}
-
-        self.play(json=json)
-        self.current()
+        self.request("PUT", str(urljoin(self.API_PLAYER, "play")), json=json)
```

### Comparing `spotrpy-2.2/spotrpy/commands/search.py` & `spotrpy-3.0/spotrpy/commands/search.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,37 +1,31 @@
 import questionary
-from urllib.parse import urljoin, urlencode
-
-class Search():
-    """ Search class """
 
-    def __init__(self, spotr):
-        # Command info
-        self.info = {
-            'name': 'Search',
-            'description': 'Search for anything on spotify, Types - track, playlist, album',
-            'arguments': [['Query...'],['Type', 'Query...']],
-            'min_args': 1,
-            'max_args': 999,
-        }
+from ..spotr import Spotr
+from urllib.parse import urljoin, urlencode
 
-        # Arguments passed
-        self.args = spotr.args
+class Search(Spotr):
+    """ Search """
 
-        # Unpack form spotr instance
-        self.CONFIG = spotr.CONFIG
-        self.request = spotr.request
-        self.play = spotr.play
-        self.parse_items = spotr.parse_items
-        self.API_BASE_VERSION = spotr.API_BASE_VERSION
-        self.QUSTIONARY_LIMIT = spotr.QUSTIONARY_LIMIT
+    description = "Search for anything on spotify, Types - track, playlist, album"
 
+    def __init__(self, args):
+        self.args = args
+        Spotr.__init__(self)
+
+    @staticmethod
+    def add_arguments(parser):
+        parser.add_argument(
+            'query', type=str, help="Search query", nargs='*'
+        )
+        parser.add_argument(
+            '-t', '--type', type=str, choices=["track", "playlist", "album"], help="Search type"
+        )
 
-    def execute(self, *query):
-        """Search for anything on spotify, Types - track, playlist, album"""
+    def execute(self):
         search_types = {
             "track": {
                 "accessor": ["tracks", "items"],
                 "return_value": ["uri"],
                 "name_value": ["name"],
                 "artists_value": ["artists"],
                 "artists_array": True,
@@ -57,35 +51,33 @@
                 "artists_array": True,
                 "json_value": "context_uri",
                 "json_value_array": False,
                 "json": {"context_uri": [], "offset": {"position": "0"}},
             },
         }
 
-        if query[0] not in ["track", "playlist", "album"]:
+        if not self.args.type:
             available_types = ["track", "playlist", "album"]
             search_type = questionary.select(
                 "Select search type",
                 choices=available_types,
                 erase_when_done=True,
                 use_shortcuts=True,
                 use_arrow_keys=True,
                 use_jk_keys=False,
             ).ask()
             if search_type is None:
                 return
         else:
-            query = list(query)
-            search_type = query[0]
-            query.pop(0)
+            search_type = self.args.type
 
         data = self.request(
             "GET",
             str(
-                f"{urljoin(self.API_BASE_VERSION, 'search')}?{urlencode({'q': ' '.join(query), 'type': search_type, 'limit': self.QUSTIONARY_LIMIT})}"
+                f"{urljoin(self.API_BASE_VERSION, 'search')}?{urlencode({'q': ' '.join(self.args.query), 'type': search_type, 'limit': self.QUSTIONARY_LIMIT})}"
             )
         )
 
         choices = self.parse_items(
             data,
             accessor=search_types[search_type]["accessor"],
             return_value=search_types[search_type]["return_value"],
@@ -108,11 +100,9 @@
 
         json = search_types[search_type]["json"]
         if search_types[search_type]["json_value_array"]:
             json[search_types[search_type]["json_value"]] = [selected]
         else:
             json[search_types[search_type]["json_value"]] = selected
 
-        self.play(json=json)
-
-
+        self.request("PUT", str(urljoin(self.API_PLAYER, "play")), json=json)
```

### Comparing `spotrpy-2.2/spotrpy/commands/shuffle.py` & `spotrpy-3.0/spotrpy/commands/playlist.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,34 +1,41 @@
 import questionary
+
+from ..spotr import Spotr
 from urllib.parse import urljoin, urlencode
 
-class Shuffle():
-    """ Shuffle class """
+class Playlist(Spotr):
+    """ Playlist """
+
+    description = "Start playing one of your playlists"
+
+    def __init__(self, args):
+        self.args = args
+        Spotr.__init__(self)
 
-    def __init__(self, spotr):
-        # Command info
-        self.info = {
-            'name': 'Shuffle',
-            'description': 'Display ASCII art for the currently playing track.',
-            'arguments': [],
-            'min_args': 0,
-            'max_args': 0,
-        }
-
-        # Arguments passed
-        self.args = spotr.args
-
-        # Unpack form spotr instance
-        self.CONFIG = spotr.CONFIG
-        self.request = spotr.request
-        self.API_PLAYER = spotr.API_PLAYER
+    @staticmethod
+    def add_arguments(parser):
+        pass
 
     def execute(self):
-        """Toggle shuffle, on / off"""
-        state = questionary.select(
-            "Choose playback state",
-            choices=["true", "false"],
+        data = self.request("GET", f"{urljoin(self.API_BASE_VERSION, 'me/playlists')}?{urlencode({'limit': self.SPOTIFY_LIMIT})}")
+
+        choices = self.parse_items(
+            data,
+            accessor=["items"],
+            return_value=["uri"],
+            name_value=["name"],
+            artists_value=False,
+        )
+
+        selected = questionary.select(
+            "What playlist do you want to play?",
+            choices=choices,
             erase_when_done=True,
-            use_shortcuts=True,
+            use_arrow_keys=True,
+            use_jk_keys=False,
         ).ask()
-        
-        self.request("PUT", str(f"{urljoin(self.API_PLAYER, 'shuffle')}?{urlencode({'state': state})}"))
+        if selected is None:
+            return
+
+        json = {"context_uri": selected, "offset": {"position": "0"}}
+        self.request("PUT", str(urljoin(self.API_PLAYER, "play")), json=json)
```

### Comparing `spotrpy-2.2/spotrpy/commands/volume.py` & `spotrpy-3.0/spotrpy/commands/volume.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,45 +1,37 @@
 import questionary
+
+from ..spotr import Spotr
 from urllib.parse import urljoin, urlencode
 
-class Volume():
-    """ Volume class """
+class Volume(Spotr):
+    """ Volume """
+
+    description = "Ajust volume"
+
+    def __init__(self, args):
+        self.args = args
+        Spotr.__init__(self)
+
+    @staticmethod
+    def add_arguments(parser):
+        parser.add_argument(
+            '-p', '--percentage', type=str, help="Volume percentage"
+        )
 
-    def __init__(self, spotr):
-        # Command info
-        self.info = {
-            'name': 'Volume',
-            'description': 'Display ASCII art for the currently playing track.',
-            'arguments': ['Volume (in percentage)'],
-            'min_args': 0,
-            'max_args': 1,
-        }
-
-        # Arguments passed
-        self.args = spotr.args
-
-        # Unpack form spotr instance
-        self.CONFIG = spotr.CONFIG
-        self.request = spotr.request
-        self.API_PLAYER = spotr.API_PLAYER
-
-    def execute(self, volume=None):
-        """Ajust volume"""
-        if volume is None:
+    def execute(self):
+        if self.args.percentage is None:
             volume = questionary.select(
                 "Choose volume precentage",
                 choices=["25%", "50%", "75%", "100%"],
                 erase_when_done=True,
                 use_shortcuts=True,
             ).ask()
         else:
-            if int(volume) < 0:
-                volume = 0
-            elif int(volume) > 100:
-                volume = 100
+            volume = self.args.percentage
+
         self.request(
             "PUT",
             str(
                 f"{urljoin(self.API_PLAYER, 'volume')}?{urlencode({'volume_percent': str(volume).replace('%', '')})}"
             ),
         )
-
```

### Comparing `spotrpy-2.2/spotrpy.egg-info/PKG-INFO` & `spotrpy-3.0/spotrpy.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 Metadata-Version: 2.1
 Name: spotrpy
-Version: 2.2
+Version: 3.0
 Summary: A simple spotify tool for the terminal
 Home-page: https://github.com/Havard03/spotr
 Author: Havard03
 Author-email: havard.buvang@gmail.com
 Keywords: cli
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: POSIX
-Classifier: Operating System :: Unix
+Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 Requires-Dist: Pillow==10.1.0
 Requires-Dist: questionary==2.0.1
 Requires-Dist: requests==2.28.1
 Requires-Dist: rich==13.6.0
```

#### html2text {}

```diff
@@ -1,16 +1,15 @@
-Metadata-Version: 2.1 Name: spotrpy Version: 2.2 Summary: A simple spotify tool
+Metadata-Version: 2.1 Name: spotrpy Version: 3.0 Summary: A simple spotify tool
 for the terminal Home-page: https://github.com/Havard03/spotr Author: Havard03
 Author-email: havard.buvang@gmail.com Keywords: cli Classifier: Programming
 Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: POSIX Classifier: Operating System :: Unix
-Requires-Python: >=3.6 Description-Content-Type: text/markdown License-File:
-LICENSE.md Requires-Dist: Pillow==10.1.0 Requires-Dist: questionary==2.0.1
-Requires-Dist: requests==2.28.1 Requires-Dist: rich==13.6.0 Requires-Dist:
-tqdm==4.66.1
+Classifier: Operating System :: OS Independent Requires-Python: >=3.6
+Description-Content-Type: text/markdown License-File: LICENSE.md Requires-Dist:
+Pillow==10.1.0 Requires-Dist: questionary==2.0.1 Requires-Dist:
+requests==2.28.1 Requires-Dist: rich==13.6.0 Requires-Dist: tqdm==4.66.1
              ************ SSppoottrr -- AA ssppoottiiffyy ttooooll ffoorr tthhee tteerrmmiinnaall ************
  _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_g_i_t_h_u_b_/_c_o_n_t_r_i_b_u_t_o_r_s_/_H_a_v_a_r_d_0_3_/_s_p_o_t_r_._s_v_g_?_s_t_y_l_e_=_f_o_r_-_t_h_e_-
  _b_a_d_g_e_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_g_i_t_h_u_b_/_f_o_r_k_s_/_H_a_v_a_r_d_0_3_/_s_p_o_t_r_._s_v_g_?_s_t_y_l_e_=_f_o_r_-_t_h_e_-
  _b_a_d_g_e_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_g_i_t_h_u_b_/_s_t_a_r_s_/_H_a_v_a_r_d_0_3_/_s_p_o_t_r_._s_v_g_?_s_t_y_l_e_=_f_o_r_-_t_h_e_-
  _b_a_d_g_e_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_g_i_t_h_u_b_/_i_s_s_u_e_s_/_H_a_v_a_r_d_0_3_/_s_p_o_t_r_._s_v_g_?_s_t_y_l_e_=_f_o_r_-_t_h_e_-
 _b_a_d_g_e_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_g_i_t_h_u_b_/_l_i_c_e_n_s_e_/_H_a_v_a_r_d_0_3_/_s_p_o_t_r_._s_v_g_?_s_t_y_l_e_=_f_o_r_-_t_h_e_-
                                     _b_a_d_g_e_]
```

### Comparing `spotrpy-2.2/spotrpy.egg-info/SOURCES.txt` & `spotrpy-3.0/spotrpy.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 LICENSE.md
 README.md
 setup.py
+spotrpy/LOGO.py
 spotrpy/__init__.py
+spotrpy/main.py
 spotrpy/spotr.py
 spotrpy.egg-info/PKG-INFO
 spotrpy.egg-info/SOURCES.txt
 spotrpy.egg-info/dependency_links.txt
 spotrpy.egg-info/entry_points.txt
 spotrpy.egg-info/requires.txt
 spotrpy.egg-info/top_level.txt
@@ -13,14 +15,15 @@
 spotrpy/Util/ASCII.py
 spotrpy/Util/Configuration.py
 spotrpy/Util/Helpers.py
 spotrpy/Util/Logging.py
 spotrpy/Util/__init__.py
 spotrpy/commands/__init__.py
 spotrpy/commands/ascii.py
+spotrpy/commands/auth.py
 spotrpy/commands/current.py
 spotrpy/commands/next.py
 spotrpy/commands/playback.py
 spotrpy/commands/playlist.py
 spotrpy/commands/playlistadd.py
 spotrpy/commands/previous.py
 spotrpy/commands/qsearch.py
```

