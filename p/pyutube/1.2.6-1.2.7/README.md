# Comparing `tmp/pyutube-1.2.6.tar.gz` & `tmp/pyutube-1.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyutube-1.2.6.tar", last modified: Sun May 12 13:30:06 2024, max compression
+gzip compressed data, was "pyutube-1.2.7.tar", last modified: Sat May 18 21:03:54 2024, max compression
```

## Comparing `pyutube-1.2.6.tar` & `pyutube-1.2.7.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0 brhoom    (1000) brhoom    (1000)        0 2024-05-12 13:30:06.923330 pyutube-1.2.6/
--rwxrwxrwx   0 brhoom    (1000) brhoom    (1000)     1078 2024-04-27 12:45:59.000000 pyutube-1.2.6/LICENSE.md
--rwxrwxrwx   0 brhoom    (1000) brhoom    (1000)     8619 2024-05-12 13:30:06.920975 pyutube-1.2.6/PKG-INFO
--rwxrwxrwx   0 brhoom    (1000) brhoom    (1000)     7795 2024-05-12 13:29:54.000000 pyutube-1.2.6/README.md
-drwxrwxrwx   0 brhoom    (1000) brhoom    (1000)        0 2024-05-12 13:30:06.907234 pyutube-1.2.6/pyutube/
--rwxrwxrwx   0 brhoom    (1000) brhoom    (1000)      399 2024-04-07 04:16:19.000000 pyutube-1.2.6/pyutube/__init__.py
--rwxrwxrwx   0 brhoom    (1000) brhoom    (1000)      184 2024-03-31 03:14:16.000000 pyutube-1.2.6/pyutube/__main__.py
--rwxrwxrwx   0 brhoom    (1000) brhoom    (1000)     6728 2024-04-30 18:17:01.000000 pyutube-1.2.6/pyutube/cli.py
--rwxrwxrwx   0 brhoom    (1000) brhoom    (1000)    14111 2024-05-12 13:19:01.000000 pyutube-1.2.6/pyutube/downloader.py
-drwxrwxrwx   0 brhoom    (1000) brhoom    (1000)        0 2024-05-12 13:30:06.917039 pyutube-1.2.6/pyutube/tests/
--rwxrwxrwx   0 brhoom    (1000) brhoom    (1000)       30 2024-02-14 23:03:00.000000 pyutube-1.2.6/pyutube/tests/__init__.py
--rwxrwxrwx   0 brhoom    (1000) brhoom    (1000)     4676 2024-04-12 09:09:48.000000 pyutube-1.2.6/pyutube/tests/test_utils.py
--rwxrwxrwx   0 brhoom    (1000) brhoom    (1000)    11218 2024-05-12 13:20:14.000000 pyutube-1.2.6/pyutube/utils.py
-drwxrwxrwx   0 brhoom    (1000) brhoom    (1000)        0 2024-05-12 13:30:06.918258 pyutube-1.2.6/pyutube.egg-info/
--rwxrwxrwx   0 brhoom    (1000) brhoom    (1000)     8619 2024-05-12 13:30:06.000000 pyutube-1.2.6/pyutube.egg-info/PKG-INFO
--rwxrwxrwx   0 brhoom    (1000) brhoom    (1000)      365 2024-05-12 13:30:06.000000 pyutube-1.2.6/pyutube.egg-info/SOURCES.txt
--rwxrwxrwx   0 brhoom    (1000) brhoom    (1000)        1 2024-05-12 13:30:06.000000 pyutube-1.2.6/pyutube.egg-info/dependency_links.txt
--rwxrwxrwx   0 brhoom    (1000) brhoom    (1000)       44 2024-05-12 13:30:06.000000 pyutube-1.2.6/pyutube.egg-info/entry_points.txt
--rwxrwxrwx   0 brhoom    (1000) brhoom    (1000)       70 2024-05-12 13:30:06.000000 pyutube-1.2.6/pyutube.egg-info/requires.txt
--rwxrwxrwx   0 brhoom    (1000) brhoom    (1000)        8 2024-05-12 13:30:06.000000 pyutube-1.2.6/pyutube.egg-info/top_level.txt
--rwxrwxrwx   0 brhoom    (1000) brhoom    (1000)       38 2024-05-12 13:30:06.923832 pyutube-1.2.6/setup.cfg
--rwxrwxrwx   0 brhoom    (1000) brhoom    (1000)     1439 2024-05-12 13:08:51.000000 pyutube-1.2.6/setup.py
+drwxrwxrwx   0 brhoom    (1000) brhoom    (1000)        0 2024-05-18 21:03:54.398934 pyutube-1.2.7/
+-rwxrwxrwx   0 brhoom    (1000) brhoom    (1000)     1078 2024-04-27 12:45:59.000000 pyutube-1.2.7/LICENSE.md
+-rwxrwxrwx   0 brhoom    (1000) brhoom    (1000)     8622 2024-05-18 21:03:54.395975 pyutube-1.2.7/PKG-INFO
+-rwxrwxrwx   0 brhoom    (1000) brhoom    (1000)     7795 2024-05-18 21:03:06.000000 pyutube-1.2.7/README.md
+drwxrwxrwx   0 brhoom    (1000) brhoom    (1000)        0 2024-05-18 21:03:54.299979 pyutube-1.2.7/pyutube/
+-rwxrwxrwx   0 brhoom    (1000) brhoom    (1000)      399 2024-04-07 04:16:19.000000 pyutube-1.2.7/pyutube/__init__.py
+-rwxrwxrwx   0 brhoom    (1000) brhoom    (1000)      184 2024-03-31 03:14:16.000000 pyutube-1.2.7/pyutube/__main__.py
+-rwxrwxrwx   0 brhoom    (1000) brhoom    (1000)     6728 2024-04-30 18:17:01.000000 pyutube-1.2.7/pyutube/cli.py
+-rwxrwxrwx   0 brhoom    (1000) brhoom    (1000)    14111 2024-05-12 13:19:01.000000 pyutube-1.2.7/pyutube/downloader.py
+drwxrwxrwx   0 brhoom    (1000) brhoom    (1000)        0 2024-05-18 21:03:54.376758 pyutube-1.2.7/pyutube/tests/
+-rwxrwxrwx   0 brhoom    (1000) brhoom    (1000)       30 2024-02-14 23:03:00.000000 pyutube-1.2.7/pyutube/tests/__init__.py
+-rwxrwxrwx   0 brhoom    (1000) brhoom    (1000)     4676 2024-04-12 09:09:48.000000 pyutube-1.2.7/pyutube/tests/test_utils.py
+-rwxrwxrwx   0 brhoom    (1000) brhoom    (1000)    11218 2024-05-18 21:03:21.000000 pyutube-1.2.7/pyutube/utils.py
+drwxrwxrwx   0 brhoom    (1000) brhoom    (1000)        0 2024-05-18 21:03:54.382954 pyutube-1.2.7/pyutube.egg-info/
+-rwxrwxrwx   0 brhoom    (1000) brhoom    (1000)     8622 2024-05-18 21:03:53.000000 pyutube-1.2.7/pyutube.egg-info/PKG-INFO
+-rwxrwxrwx   0 brhoom    (1000) brhoom    (1000)      365 2024-05-18 21:03:53.000000 pyutube-1.2.7/pyutube.egg-info/SOURCES.txt
+-rwxrwxrwx   0 brhoom    (1000) brhoom    (1000)        1 2024-05-18 21:03:53.000000 pyutube-1.2.7/pyutube.egg-info/dependency_links.txt
+-rwxrwxrwx   0 brhoom    (1000) brhoom    (1000)       44 2024-05-18 21:03:53.000000 pyutube-1.2.7/pyutube.egg-info/entry_points.txt
+-rwxrwxrwx   0 brhoom    (1000) brhoom    (1000)       73 2024-05-18 21:03:53.000000 pyutube-1.2.7/pyutube.egg-info/requires.txt
+-rwxrwxrwx   0 brhoom    (1000) brhoom    (1000)        8 2024-05-18 21:03:53.000000 pyutube-1.2.7/pyutube.egg-info/top_level.txt
+-rwxrwxrwx   0 brhoom    (1000) brhoom    (1000)       38 2024-05-18 21:03:54.399407 pyutube-1.2.7/setup.cfg
+-rwxrwxrwx   0 brhoom    (1000) brhoom    (1000)     1442 2024-05-18 21:02:28.000000 pyutube-1.2.7/setup.py
```

### Comparing `pyutube-1.2.6/LICENSE.md` & `pyutube-1.2.7/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pyutube-1.2.6/PKG-INFO` & `pyutube-1.2.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyutube
-Version: 1.2.6
+Version: 1.2.7
 Summary: Awesome CLI to download YouTube videos (as video or audio)/shorts/playlists from the terminal
 Author: Ebraheem Alhetari
 Author-email: hetari4all@gmail.com
 License: MIT
 Project-URL: Homepage, https://github.com/Hetari/pyutube
 Keywords: youtube,download,cli,pyutube,pytubefix
 Platform: Windows
@@ -12,15 +12,15 @@
 Platform: Linux
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
-Requires-Dist: pytube
+Requires-Dist: pytubefix
 Requires-Dist: inquirer
 Requires-Dist: yaspin
 Requires-Dist: typer
 Requires-Dist: requests
 Requires-Dist: rich
 Requires-Dist: inquirer
 Requires-Dist: termcolor
@@ -79,15 +79,16 @@
 
 Pyutube is very easy to use, here are examples of its uses:
 
 ```bash
 pyutube YOUTUBE_LINK [PATH]
 ```
 
-> [!NOTE] > `[PATH]` is an optional input, the default value is the `terminal` path where the CLI is running (the current working directory in your terminal).
+> [!NOTE]
+> `[PATH]` is an optional input, the default value is the `terminal` path where the CLI is running (the current working directory in your terminal).
 
 ## 👨‍💻 Usage
 
 #### Arguments
 
 | Arguments | Description                                                                                                          |
 | --------- | -------------------------------------------------------------------------------------------------------------------- |
```

#### html2text {}

```diff
@@ -1,17 +1,17 @@
-Metadata-Version: 2.1 Name: pyutube Version: 1.2.6 Summary: Awesome CLI to
+Metadata-Version: 2.1 Name: pyutube Version: 1.2.7 Summary: Awesome CLI to
 download YouTube videos (as video or audio)/shorts/playlists from the terminal
 Author: Ebraheem Alhetari Author-email: hetari4all@gmail.com License: MIT
 Project-URL: Homepage, https://github.com/Hetari/pyutube Keywords:
 youtube,download,cli,pyutube,pytubefix Platform: Windows Platform: MacOS
 Platform: Linux Classifier: License :: OSI Approved :: MIT License Classifier:
 Operating System :: OS Independent Classifier: Programming Language :: Python
 :: 3 Requires-Python: >=3.6 Description-Content-Type: text/markdown License-
-File: LICENSE.md Requires-Dist: pytube Requires-Dist: inquirer Requires-Dist:
-yaspin Requires-Dist: typer Requires-Dist: requests Requires-Dist: rich
+File: LICENSE.md Requires-Dist: pytubefix Requires-Dist: inquirer Requires-
+Dist: yaspin Requires-Dist: typer Requires-Dist: requests Requires-Dist: rich
 Requires-Dist: inquirer Requires-Dist: termcolor Requires-Dist: moviepy # ð¹
 YouTube Downloader CLI ### Enjoying my project? Please show your appreciation
 by starring it on GitHub! â­ [![Version](https://img.shields.io/pypi/v/
 pyutube.svg?style=flat)](https://pypi.org/project/pyutube/) [![Downloads]
 (https://static.pepy.tech/badge/pyutube)](https://pepy.tech/project/pyutube) >
 [!NOTE] > Have a new feature? Please don't hesitate to [tell me](https://
 github.com/Hetari/pyutube/issues/new)! _[_P_y_u_t_u_b_e_]## ð Description This
```

### Comparing `pyutube-1.2.6/README.md` & `pyutube-1.2.7/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -51,15 +51,16 @@
 
 Pyutube is very easy to use, here are examples of its uses:
 
 ```bash
 pyutube YOUTUBE_LINK [PATH]
 ```
 
-> [!NOTE] > `[PATH]` is an optional input, the default value is the `terminal` path where the CLI is running (the current working directory in your terminal).
+> [!NOTE]
+> `[PATH]` is an optional input, the default value is the `terminal` path where the CLI is running (the current working directory in your terminal).
 
 ## 👨‍💻 Usage
 
 #### Arguments
 
 | Arguments | Description                                                                                                          |
 | --------- | -------------------------------------------------------------------------------------------------------------------- |
```

### Comparing `pyutube-1.2.6/pyutube/cli.py` & `pyutube-1.2.7/pyutube/cli.py`

 * *Files identical despite different names*

### Comparing `pyutube-1.2.6/pyutube/downloader.py` & `pyutube-1.2.7/pyutube/downloader.py`

 * *Files identical despite different names*

### Comparing `pyutube-1.2.6/pyutube/tests/test_utils.py` & `pyutube-1.2.7/pyutube/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `pyutube-1.2.6/pyutube/utils.py` & `pyutube-1.2.7/pyutube/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 from yaspin import yaspin
 from yaspin.spinners import Spinners
 from rich.console import Console
 from rich.theme import Theme
 from termcolor import colored
 
 
-__version__ = "1.2.6"
+__version__ = "1.2.7"
 __app__ = "pyutube"
 ABORTED_PREFIX = "aborted"
 CANCEL_PREFIX = "cancel"
 
 
 # Set up the console
 custom_theme = Theme({
```

### Comparing `pyutube-1.2.6/pyutube.egg-info/PKG-INFO` & `pyutube-1.2.7/pyutube.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyutube
-Version: 1.2.6
+Version: 1.2.7
 Summary: Awesome CLI to download YouTube videos (as video or audio)/shorts/playlists from the terminal
 Author: Ebraheem Alhetari
 Author-email: hetari4all@gmail.com
 License: MIT
 Project-URL: Homepage, https://github.com/Hetari/pyutube
 Keywords: youtube,download,cli,pyutube,pytubefix
 Platform: Windows
@@ -12,15 +12,15 @@
 Platform: Linux
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
-Requires-Dist: pytube
+Requires-Dist: pytubefix
 Requires-Dist: inquirer
 Requires-Dist: yaspin
 Requires-Dist: typer
 Requires-Dist: requests
 Requires-Dist: rich
 Requires-Dist: inquirer
 Requires-Dist: termcolor
@@ -79,15 +79,16 @@
 
 Pyutube is very easy to use, here are examples of its uses:
 
 ```bash
 pyutube YOUTUBE_LINK [PATH]
 ```
 
-> [!NOTE] > `[PATH]` is an optional input, the default value is the `terminal` path where the CLI is running (the current working directory in your terminal).
+> [!NOTE]
+> `[PATH]` is an optional input, the default value is the `terminal` path where the CLI is running (the current working directory in your terminal).
 
 ## 👨‍💻 Usage
 
 #### Arguments
 
 | Arguments | Description                                                                                                          |
 | --------- | -------------------------------------------------------------------------------------------------------------------- |
```

#### html2text {}

```diff
@@ -1,17 +1,17 @@
-Metadata-Version: 2.1 Name: pyutube Version: 1.2.6 Summary: Awesome CLI to
+Metadata-Version: 2.1 Name: pyutube Version: 1.2.7 Summary: Awesome CLI to
 download YouTube videos (as video or audio)/shorts/playlists from the terminal
 Author: Ebraheem Alhetari Author-email: hetari4all@gmail.com License: MIT
 Project-URL: Homepage, https://github.com/Hetari/pyutube Keywords:
 youtube,download,cli,pyutube,pytubefix Platform: Windows Platform: MacOS
 Platform: Linux Classifier: License :: OSI Approved :: MIT License Classifier:
 Operating System :: OS Independent Classifier: Programming Language :: Python
 :: 3 Requires-Python: >=3.6 Description-Content-Type: text/markdown License-
-File: LICENSE.md Requires-Dist: pytube Requires-Dist: inquirer Requires-Dist:
-yaspin Requires-Dist: typer Requires-Dist: requests Requires-Dist: rich
+File: LICENSE.md Requires-Dist: pytubefix Requires-Dist: inquirer Requires-
+Dist: yaspin Requires-Dist: typer Requires-Dist: requests Requires-Dist: rich
 Requires-Dist: inquirer Requires-Dist: termcolor Requires-Dist: moviepy # ð¹
 YouTube Downloader CLI ### Enjoying my project? Please show your appreciation
 by starring it on GitHub! â­ [![Version](https://img.shields.io/pypi/v/
 pyutube.svg?style=flat)](https://pypi.org/project/pyutube/) [![Downloads]
 (https://static.pepy.tech/badge/pyutube)](https://pepy.tech/project/pyutube) >
 [!NOTE] > Have a new feature? Please don't hesitate to [tell me](https://
 github.com/Hetari/pyutube/issues/new)! _[_P_y_u_t_u_b_e_]## ð Description This
```

### Comparing `pyutube-1.2.6/setup.py` & `pyutube-1.2.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -39,15 +39,15 @@
 
 
     include_package_data=True,
 
     python_requires=">=3.6",
 
     install_requires=[
-        "pytube",
+        "pytubefix",
         "inquirer",
         "yaspin",
         "typer",
         "requests",
         "rich",
         "inquirer",
         "termcolor",
```

