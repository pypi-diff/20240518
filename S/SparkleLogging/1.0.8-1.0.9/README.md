# Comparing `tmp/SparkleLogging-1.0.8.tar.gz` & `tmp/SparkleLogging-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SparkleLogging-1.0.8.tar", last modified: Sat May  4 03:10:23 2024, max compression
+gzip compressed data, was "SparkleLogging-1.0.9.tar", last modified: Sat May 18 11:34:55 2024, max compression
```

## Comparing `SparkleLogging-1.0.8.tar` & `SparkleLogging-1.0.9.tar`

### file list

```diff
@@ -1,22 +1,24 @@
-drwxrwxrwx   0        0        0        0 2024-05-04 03:10:23.471346 SparkleLogging-1.0.8/
--rw-rw-rw-   0        0        0     3103 2024-05-04 03:10:23.470347 SparkleLogging-1.0.8/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-04 03:10:23.352981 SparkleLogging-1.0.8/SparkleLogging/
--rw-rw-rw-   0        0        0        0 2024-05-03 04:38:26.000000 SparkleLogging-1.0.8/SparkleLogging/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-04 03:10:23.415331 SparkleLogging-1.0.8/SparkleLogging/plugins/
--rw-rw-rw-   0        0        0      450 2024-05-03 04:38:26.000000 SparkleLogging-1.0.8/SparkleLogging/plugins/DecoratorsTools.py
--rw-rw-rw-   0        0        0     1160 2024-05-03 04:38:26.000000 SparkleLogging-1.0.8/SparkleLogging/plugins/HttpHander.py
--rw-rw-rw-   0        0        0        0 2024-05-03 04:38:26.000000 SparkleLogging-1.0.8/SparkleLogging/plugins/__init__.py
--rw-rw-rw-   0        0        0      954 2024-05-03 04:38:26.000000 SparkleLogging-1.0.8/SparkleLogging/plugins/websocketHander.py
-drwxrwxrwx   0        0        0        0 2024-05-04 03:10:23.442412 SparkleLogging-1.0.8/SparkleLogging/utils/
--rw-rw-rw-   0        0        0        0 2024-05-03 04:38:26.000000 SparkleLogging-1.0.8/SparkleLogging/utils/__init__.py
--rw-rw-rw-   0        0        0      498 2024-05-04 03:09:16.000000 SparkleLogging-1.0.8/SparkleLogging/utils/core.py
--rw-rw-rw-   0        0        0     4700 2024-05-04 02:57:14.000000 SparkleLogging-1.0.8/SparkleLogging/utils/getLog.py
--rw-rw-rw-   0        0        0      372 2024-05-03 04:38:26.000000 SparkleLogging-1.0.8/SparkleLogging/utils/plugins_for_core.py
-drwxrwxrwx   0        0        0        0 2024-05-04 03:10:23.469519 SparkleLogging-1.0.8/SparkleLogging.egg-info/
--rw-rw-rw-   0        0        0     3103 2024-05-04 03:10:22.000000 SparkleLogging-1.0.8/SparkleLogging.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      514 2024-05-04 03:10:22.000000 SparkleLogging-1.0.8/SparkleLogging.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-04 03:10:22.000000 SparkleLogging-1.0.8/SparkleLogging.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       35 2024-05-04 03:10:22.000000 SparkleLogging-1.0.8/SparkleLogging.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2024-05-04 03:10:22.000000 SparkleLogging-1.0.8/SparkleLogging.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-04 03:10:23.471346 SparkleLogging-1.0.8/setup.cfg
--rw-rw-rw-   0        0        0      724 2024-05-04 03:08:53.000000 SparkleLogging-1.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-18 11:34:55.254013 SparkleLogging-1.0.9/
+-rw-rw-rw-   0        0        0     3185 2024-05-18 11:34:55.251020 SparkleLogging-1.0.9/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-18 11:34:55.210128 SparkleLogging-1.0.9/SparkleLogging/
+-rw-rw-rw-   0        0        0        0 2024-05-03 04:38:26.000000 SparkleLogging-1.0.9/SparkleLogging/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-18 11:34:55.245036 SparkleLogging-1.0.9/SparkleLogging/plugins/
+-rw-rw-rw-   0        0        0      450 2024-05-03 04:38:26.000000 SparkleLogging-1.0.9/SparkleLogging/plugins/DecoratorsTools.py
+-rw-rw-rw-   0        0        0     1160 2024-05-03 04:38:26.000000 SparkleLogging-1.0.9/SparkleLogging/plugins/HttpHander.py
+-rw-rw-rw-   0        0        0        0 2024-05-03 04:38:26.000000 SparkleLogging-1.0.9/SparkleLogging/plugins/__init__.py
+-rw-rw-rw-   0        0        0     1370 2024-05-04 07:52:07.000000 SparkleLogging-1.0.9/SparkleLogging/plugins/excHandler.py
+-rw-rw-rw-   0        0        0     1193 2024-05-18 11:31:30.000000 SparkleLogging-1.0.9/SparkleLogging/plugins/exclogger.py
+-rw-rw-rw-   0        0        0      954 2024-05-03 04:38:26.000000 SparkleLogging-1.0.9/SparkleLogging/plugins/websocketHander.py
+drwxrwxrwx   0        0        0        0 2024-05-18 11:34:55.249026 SparkleLogging-1.0.9/SparkleLogging/utils/
+-rw-rw-rw-   0        0        0        0 2024-05-03 04:38:26.000000 SparkleLogging-1.0.9/SparkleLogging/utils/__init__.py
+-rw-rw-rw-   0        0        0      498 2024-05-04 03:09:16.000000 SparkleLogging-1.0.9/SparkleLogging/utils/core.py
+-rw-rw-rw-   0        0        0     4700 2024-05-18 11:32:14.000000 SparkleLogging-1.0.9/SparkleLogging/utils/getLog.py
+-rw-rw-rw-   0        0        0      434 2024-05-18 11:33:19.000000 SparkleLogging-1.0.9/SparkleLogging/utils/plugins_for_core.py
+drwxrwxrwx   0        0        0        0 2024-05-18 11:34:55.250022 SparkleLogging-1.0.9/SparkleLogging.egg-info/
+-rw-rw-rw-   0        0        0     3185 2024-05-18 11:34:53.000000 SparkleLogging-1.0.9/SparkleLogging.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      587 2024-05-18 11:34:54.000000 SparkleLogging-1.0.9/SparkleLogging.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-18 11:34:53.000000 SparkleLogging-1.0.9/SparkleLogging.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       35 2024-05-18 11:34:53.000000 SparkleLogging-1.0.9/SparkleLogging.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2024-05-18 11:34:53.000000 SparkleLogging-1.0.9/SparkleLogging.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-18 11:34:55.255010 SparkleLogging-1.0.9/setup.cfg
+-rw-rw-rw-   0        0        0      724 2024-05-18 11:23:59.000000 SparkleLogging-1.0.9/setup.py
```

### Comparing `SparkleLogging-1.0.8/PKG-INFO` & `SparkleLogging-1.0.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SparkleLogging
-Version: 1.0.8
+Version: 1.0.9
 Summary: A logging library for Python
 Home-page: https://github.com/KOKOMI12345/SparkleLogging
 Author: 花火official
 Author-email: 3072252442@qq.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -58,14 +58,18 @@
 - `setFileLevel`: 设置文件日志输出级别,默认INFO
 - `setWebLevel`: 设置websocket日志输出级别,默认INFO
 - `setHttpLevel`: 设置http日志输出级别,默认INFO
 - `custom_fomatter`: 自定义格式化函数,默认None
 
 ## 更新日志
 
+# 2024/5/18 19:24
+
+更新了不同的堆栈格式和方便使用的装饰器
+
 # 2024/2/20 1:01
 
 更新了自定义格式功能,修复了少量bug
 
 # 2024/5/2 20:10
 
 更新了可以自定义设置日志等级的功能
```

### Comparing `SparkleLogging-1.0.8/SparkleLogging/plugins/HttpHander.py` & `SparkleLogging-1.0.9/SparkleLogging/plugins/HttpHander.py`

 * *Files identical despite different names*

### Comparing `SparkleLogging-1.0.8/SparkleLogging/plugins/websocketHander.py` & `SparkleLogging-1.0.9/SparkleLogging/plugins/websocketHander.py`

 * *Files identical despite different names*

### Comparing `SparkleLogging-1.0.8/SparkleLogging/utils/getLog.py` & `SparkleLogging-1.0.9/SparkleLogging/utils/getLog.py`

 * *Files identical despite different names*

### Comparing `SparkleLogging-1.0.8/SparkleLogging.egg-info/PKG-INFO` & `SparkleLogging-1.0.9/SparkleLogging.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SparkleLogging
-Version: 1.0.8
+Version: 1.0.9
 Summary: A logging library for Python
 Home-page: https://github.com/KOKOMI12345/SparkleLogging
 Author: 花火official
 Author-email: 3072252442@qq.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -58,14 +58,18 @@
 - `setFileLevel`: 设置文件日志输出级别,默认INFO
 - `setWebLevel`: 设置websocket日志输出级别,默认INFO
 - `setHttpLevel`: 设置http日志输出级别,默认INFO
 - `custom_fomatter`: 自定义格式化函数,默认None
 
 ## 更新日志
 
+# 2024/5/18 19:24
+
+更新了不同的堆栈格式和方便使用的装饰器
+
 # 2024/2/20 1:01
 
 更新了自定义格式功能,修复了少量bug
 
 # 2024/5/2 20:10
 
 更新了可以自定义设置日志等级的功能
```

### Comparing `SparkleLogging-1.0.8/SparkleLogging.egg-info/SOURCES.txt` & `SparkleLogging-1.0.9/SparkleLogging.egg-info/SOURCES.txt`

 * *Files 19% similar despite different names*

```diff
@@ -4,12 +4,14 @@
 SparkleLogging.egg-info/SOURCES.txt
 SparkleLogging.egg-info/dependency_links.txt
 SparkleLogging.egg-info/requires.txt
 SparkleLogging.egg-info/top_level.txt
 SparkleLogging/plugins/DecoratorsTools.py
 SparkleLogging/plugins/HttpHander.py
 SparkleLogging/plugins/__init__.py
+SparkleLogging/plugins/excHandler.py
+SparkleLogging/plugins/exclogger.py
 SparkleLogging/plugins/websocketHander.py
 SparkleLogging/utils/__init__.py
 SparkleLogging/utils/core.py
 SparkleLogging/utils/getLog.py
 SparkleLogging/utils/plugins_for_core.py
```

