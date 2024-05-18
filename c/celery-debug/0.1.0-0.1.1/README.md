# Comparing `tmp/celery-debug-0.1.0.tar.gz` & `tmp/celery-debug-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "celery-debug-0.1.0.tar", last modified: Fri May 17 13:16:15 2024, max compression
+gzip compressed data, was "celery-debug-0.1.1.tar", last modified: Fri May 17 23:34:46 2024, max compression
```

## Comparing `celery-debug-0.1.0.tar` & `celery-debug-0.1.1.tar`

### file list

```diff
@@ -1,16 +1,19 @@
-drwxr-xr-x   0 test       (501) staff       (20)        0 2024-05-17 13:16:15.741422 celery-debug-0.1.0/
--rw-r--r--   0 test       (501) staff       (20)     1036 2024-05-17 12:58:21.000000 celery-debug-0.1.0/LICENSE
--rw-r--r--   0 test       (501) staff       (20)      136 2024-05-17 12:58:40.000000 celery-debug-0.1.0/MANIFEST.in
--rw-r--r--   0 test       (501) staff       (20)     1390 2024-05-17 13:16:15.741301 celery-debug-0.1.0/PKG-INFO
--rw-r--r--   0 test       (501) staff       (20)      793 2024-05-17 13:07:07.000000 celery-debug-0.1.0/README.md
-drwxr-xr-x   0 test       (501) staff       (20)        0 2024-05-17 13:16:15.741143 celery-debug-0.1.0/celery_debug.egg-info/
--rw-r--r--   0 test       (501) staff       (20)     1390 2024-05-17 13:16:15.000000 celery-debug-0.1.0/celery_debug.egg-info/PKG-INFO
--rw-r--r--   0 test       (501) staff       (20)      285 2024-05-17 13:16:15.000000 celery-debug-0.1.0/celery_debug.egg-info/SOURCES.txt
--rw-r--r--   0 test       (501) staff       (20)        1 2024-05-17 13:16:15.000000 celery-debug-0.1.0/celery_debug.egg-info/dependency_links.txt
--rw-r--r--   0 test       (501) staff       (20)        1 2024-05-17 13:16:15.000000 celery-debug-0.1.0/celery_debug.egg-info/not-zip-safe
--rw-r--r--   0 test       (501) staff       (20)        7 2024-05-17 13:16:15.000000 celery-debug-0.1.0/celery_debug.egg-info/requires.txt
--rw-r--r--   0 test       (501) staff       (20)       13 2024-05-17 13:16:15.000000 celery-debug-0.1.0/celery_debug.egg-info/top_level.txt
--rw-r--r--   0 test       (501) staff       (20)      430 2024-05-17 13:11:18.000000 celery-debug-0.1.0/celery_debug.py
--rw-r--r--   0 test       (501) staff       (20)        7 2024-05-17 12:58:30.000000 celery-debug-0.1.0/requirements.txt
--rw-r--r--   0 test       (501) staff       (20)       38 2024-05-17 13:16:15.741476 celery-debug-0.1.0/setup.cfg
--rw-r--r--   0 test       (501) staff       (20)     1234 2024-05-17 13:00:43.000000 celery-debug-0.1.0/setup.py
+drwxr-xr-x   0 test       (501) staff       (20)        0 2024-05-17 23:34:46.751643 celery-debug-0.1.1/
+-rw-r--r--   0 test       (501) staff       (20)     1036 2024-05-17 12:58:21.000000 celery-debug-0.1.1/LICENSE
+-rw-r--r--   0 test       (501) staff       (20)      156 2024-05-17 23:15:59.000000 celery-debug-0.1.1/MANIFEST.in
+-rw-r--r--   0 test       (501) staff       (20)     1565 2024-05-17 23:34:46.751527 celery-debug-0.1.1/PKG-INFO
+-rw-r--r--   0 test       (501) staff       (20)      968 2024-05-17 23:34:40.000000 celery-debug-0.1.1/README.md
+drwxr-xr-x   0 test       (501) staff       (20)        0 2024-05-17 23:34:46.750506 celery-debug-0.1.1/celery_debug/
+-rw-r--r--   0 test       (501) staff       (20)      110 2024-05-17 22:43:08.000000 celery-debug-0.1.1/celery_debug/__init__.py
+-rw-r--r--   0 test       (501) staff       (20)      397 2024-05-17 22:45:53.000000 celery-debug-0.1.1/celery_debug/tasks.py
+-rw-r--r--   0 test       (501) staff       (20)     1483 2024-05-17 23:33:44.000000 celery-debug-0.1.1/celery_debug/utils.py
+drwxr-xr-x   0 test       (501) staff       (20)        0 2024-05-17 23:34:46.751363 celery-debug-0.1.1/celery_debug.egg-info/
+-rw-r--r--   0 test       (501) staff       (20)     1565 2024-05-17 23:34:46.000000 celery-debug-0.1.1/celery_debug.egg-info/PKG-INFO
+-rw-r--r--   0 test       (501) staff       (20)      338 2024-05-17 23:34:46.000000 celery-debug-0.1.1/celery_debug.egg-info/SOURCES.txt
+-rw-r--r--   0 test       (501) staff       (20)        1 2024-05-17 23:34:46.000000 celery-debug-0.1.1/celery_debug.egg-info/dependency_links.txt
+-rw-r--r--   0 test       (501) staff       (20)        1 2024-05-17 23:34:46.000000 celery-debug-0.1.1/celery_debug.egg-info/not-zip-safe
+-rw-r--r--   0 test       (501) staff       (20)        7 2024-05-17 23:34:46.000000 celery-debug-0.1.1/celery_debug.egg-info/requires.txt
+-rw-r--r--   0 test       (501) staff       (20)       13 2024-05-17 23:34:46.000000 celery-debug-0.1.1/celery_debug.egg-info/top_level.txt
+-rw-r--r--   0 test       (501) staff       (20)        7 2024-05-17 12:58:30.000000 celery-debug-0.1.1/requirements.txt
+-rw-r--r--   0 test       (501) staff       (20)       38 2024-05-17 23:34:46.751699 celery-debug-0.1.1/setup.cfg
+-rw-r--r--   0 test       (501) staff       (20)     1186 2024-05-17 23:34:37.000000 celery-debug-0.1.1/setup.py
```

### Comparing `celery-debug-0.1.0/LICENSE` & `celery-debug-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `celery-debug-0.1.0/PKG-INFO` & `celery-debug-0.1.1/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: celery-debug
-Version: 0.1.0
+Version: 0.1.1
 Summary: celery debug tasks.
 Home-page: UNKNOWN
 Author: Chen YuBo
 Maintainer: Chen YuBo
 License: MIT
 Keywords: celery debug tasks
 Platform: UNKNOWN
@@ -43,23 +43,29 @@
     result_backend = "redis://redis/1"
     accept_content = ["application/json"]
     task_serializer = "json"
     result_accept_content = ["application/json"]
     result_serializer = "json"
     timezone = "Asia/Shanghai"
     broker_connection_retry_on_startup = True
-    task_routes = {}
+    # 额外新增的配置项
+    # 配置后所有任务都使用不同的队列
+    use_different_queue = True
     ```
 
 2. 使用以下命令启动celery worker
 
     ```shell
     celery -A celery_debug:app worker -Q debug -l DEBUG
     ```
 
 ## 版本记录
 
 ### v0.1.0
 
 - 版本首发。
 
+### v0.1.1
+
+- 提供配置项，快速让所有任务都使用不同的队列。
+
```

### Comparing `celery-debug-0.1.0/celery_debug.egg-info/PKG-INFO` & `celery-debug-0.1.1/celery_debug.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: celery-debug
-Version: 0.1.0
+Version: 0.1.1
 Summary: celery debug tasks.
 Home-page: UNKNOWN
 Author: Chen YuBo
 Maintainer: Chen YuBo
 License: MIT
 Keywords: celery debug tasks
 Platform: UNKNOWN
@@ -43,23 +43,29 @@
     result_backend = "redis://redis/1"
     accept_content = ["application/json"]
     task_serializer = "json"
     result_accept_content = ["application/json"]
     result_serializer = "json"
     timezone = "Asia/Shanghai"
     broker_connection_retry_on_startup = True
-    task_routes = {}
+    # 额外新增的配置项
+    # 配置后所有任务都使用不同的队列
+    use_different_queue = True
     ```
 
 2. 使用以下命令启动celery worker
 
     ```shell
     celery -A celery_debug:app worker -Q debug -l DEBUG
     ```
 
 ## 版本记录
 
 ### v0.1.0
 
 - 版本首发。
 
+### v0.1.1
+
+- 提供配置项，快速让所有任务都使用不同的队列。
+
```

### Comparing `celery-debug-0.1.0/setup.py` & `celery-debug-0.1.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     long_description = fobj.read()
 
 with open(os.path.join(here, "requirements.txt"), "r", encoding="utf-8") as fobj:
     requires = [x.strip() for x in fobj.readlines() if x.strip()]
 
 setup(
     name="celery-debug",
-    version="0.1.0",
+    version="0.1.1",
     description="celery debug tasks.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="Chen YuBo",
     maintainer="Chen YuBo",
     license="MIT",
     classifiers=[
@@ -28,13 +28,10 @@
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3 :: Only",
     ],
     keywords=["celery debug tasks"],
     install_requires=requires,
     packages=find_packages("."),
-    py_modules=[
-        "celery_debug",
-    ],
     zip_safe=False,
     include_package_data=True,
 )
```

