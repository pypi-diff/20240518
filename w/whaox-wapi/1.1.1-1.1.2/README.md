# Comparing `tmp/whaox-wapi-1.1.1.tar.gz` & `tmp/whaox-wapi-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "whaox-wapi-1.1.1.tar", last modified: Thu May 16 18:16:55 2024, max compression
+gzip compressed data, was "whaox-wapi-1.1.2.tar", last modified: Sat May 18 05:05:52 2024, max compression
```

## Comparing `whaox-wapi-1.1.1.tar` & `whaox-wapi-1.1.2.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxrwxrwx   0        0        0        0 2024-05-16 18:16:55.268086 whaox-wapi-1.1.1/
--rw-rw-rw-   0        0        0     1083 2024-04-11 20:02:10.000000 whaox-wapi-1.1.1/LICENSE
--rw-rw-rw-   0        0        0     3072 2024-05-16 18:16:55.265296 whaox-wapi-1.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     2663 2024-05-16 18:13:06.000000 whaox-wapi-1.1.1/README.md
--rw-rw-rw-   0        0        0       42 2024-05-16 18:16:55.268704 whaox-wapi-1.1.1/setup.cfg
--rw-rw-rw-   0        0        0      932 2024-05-16 18:16:35.000000 whaox-wapi-1.1.1/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-16 18:16:55.223611 whaox-wapi-1.1.1/wapi/
--rw-rw-rw-   0        0        0       27 2024-04-15 09:31:56.000000 whaox-wapi-1.1.1/wapi/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-16 18:16:55.229885 whaox-wapi-1.1.1/wapi/features/
--rw-rw-rw-   0        0        0      669 2024-05-16 17:54:49.000000 whaox-wapi-1.1.1/wapi/features/DELETE.py
--rw-rw-rw-   0        0        0      663 2024-05-16 18:00:57.000000 whaox-wapi-1.1.1/wapi/features/GET.py
--rw-rw-rw-   0        0        0      667 2024-05-16 17:54:49.000000 whaox-wapi-1.1.1/wapi/features/PATCH.py
--rw-rw-rw-   0        0        0      659 2024-05-16 18:00:57.000000 whaox-wapi-1.1.1/wapi/features/POST.py
--rw-rw-rw-   0        0        0      663 2024-05-16 17:54:49.000000 whaox-wapi-1.1.1/wapi/features/PUT.py
--rw-rw-rw-   0        0        0      837 2024-05-09 11:47:35.000000 whaox-wapi-1.1.1/wapi/features/Route.py
--rw-rw-rw-   0        0        0      148 2024-05-16 18:00:57.000000 whaox-wapi-1.1.1/wapi/features/__init__.py
--rw-rw-rw-   0        0        0     1291 2024-05-16 18:16:35.000000 whaox-wapi-1.1.1/wapi/features/request.py
-drwxrwxrwx   0        0        0        0 2024-05-16 18:16:55.234255 whaox-wapi-1.1.1/wapi/static/
--rw-rw-rw-   0        0        0       48 2024-04-11 20:01:35.000000 whaox-wapi-1.1.1/wapi/static/T.py
--rw-rw-rw-   0        0        0        0 2024-04-15 09:20:58.000000 whaox-wapi-1.1.1/wapi/static/__init__.py
--rw-rw-rw-   0        0        0      118 2024-05-16 16:57:54.000000 whaox-wapi-1.1.1/wapi/static/methods.py
--rw-rw-rw-   0        0        0      440 2024-05-16 17:01:19.000000 whaox-wapi-1.1.1/wapi/static/params.py
-drwxrwxrwx   0        0        0        0 2024-05-16 18:16:55.242139 whaox-wapi-1.1.1/wapi/utils/
--rw-rw-rw-   0        0        0        0 2024-04-15 09:21:14.000000 whaox-wapi-1.1.1/wapi/utils/__init__.py
--rw-rw-rw-   0        0        0      299 2024-05-14 15:31:03.000000 whaox-wapi-1.1.1/wapi/utils/get_path.py
--rw-rw-rw-   0        0        0      252 2024-05-16 17:25:56.000000 whaox-wapi-1.1.1/wapi/utils/get_used_vars.py
--rw-rw-rw-   0        0        0       54 2024-05-09 11:47:35.000000 whaox-wapi-1.1.1/wapi/utils/is_class.py
--rw-rw-rw-   0        0        0      124 2024-04-11 20:01:35.000000 whaox-wapi-1.1.1/wapi/utils/is_dataclass.py
--rw-rw-rw-   0        0        0       59 2024-05-09 09:32:44.000000 whaox-wapi-1.1.1/wapi/utils/is_object.py
--rw-rw-rw-   0        0        0      311 2024-05-14 15:31:03.000000 whaox-wapi-1.1.1/wapi/utils/merge_paths.py
--rw-rw-rw-   0        0        0      242 2024-05-14 15:31:57.000000 whaox-wapi-1.1.1/wapi/utils/set_path.py
-drwxrwxrwx   0        0        0        0 2024-05-16 18:16:55.263139 whaox-wapi-1.1.1/whaox_wapi.egg-info/
--rw-rw-rw-   0        0        0     3072 2024-05-16 18:16:55.000000 whaox-wapi-1.1.1/whaox_wapi.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      680 2024-05-16 18:16:55.000000 whaox-wapi-1.1.1/whaox_wapi.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-16 18:16:55.000000 whaox-wapi-1.1.1/whaox_wapi.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2024-05-16 18:16:55.000000 whaox-wapi-1.1.1/whaox_wapi.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2024-05-16 18:16:55.000000 whaox-wapi-1.1.1/whaox_wapi.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-18 05:05:52.424246 whaox-wapi-1.1.2/
+-rw-rw-rw-   0        0        0     1083 2024-04-11 20:02:10.000000 whaox-wapi-1.1.2/LICENSE
+-rw-rw-rw-   0        0        0     3072 2024-05-18 05:05:52.328704 whaox-wapi-1.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0     2663 2024-05-16 18:13:06.000000 whaox-wapi-1.1.2/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-18 05:05:52.428868 whaox-wapi-1.1.2/setup.cfg
+-rw-rw-rw-   0        0        0      932 2024-05-18 05:05:38.000000 whaox-wapi-1.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-18 05:05:52.042439 whaox-wapi-1.1.2/wapi/
+-rw-rw-rw-   0        0        0       27 2024-04-15 09:31:56.000000 whaox-wapi-1.1.2/wapi/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-18 05:05:52.103013 whaox-wapi-1.1.2/wapi/features/
+-rw-rw-rw-   0        0        0      669 2024-05-16 17:54:49.000000 whaox-wapi-1.1.2/wapi/features/DELETE.py
+-rw-rw-rw-   0        0        0      663 2024-05-16 18:00:57.000000 whaox-wapi-1.1.2/wapi/features/GET.py
+-rw-rw-rw-   0        0        0      667 2024-05-16 17:54:49.000000 whaox-wapi-1.1.2/wapi/features/PATCH.py
+-rw-rw-rw-   0        0        0      659 2024-05-16 18:00:57.000000 whaox-wapi-1.1.2/wapi/features/POST.py
+-rw-rw-rw-   0        0        0      663 2024-05-16 17:54:49.000000 whaox-wapi-1.1.2/wapi/features/PUT.py
+-rw-rw-rw-   0        0        0      837 2024-05-09 11:47:35.000000 whaox-wapi-1.1.2/wapi/features/Route.py
+-rw-rw-rw-   0        0        0      148 2024-05-16 18:00:57.000000 whaox-wapi-1.1.2/wapi/features/__init__.py
+-rw-rw-rw-   0        0        0     1291 2024-05-16 18:16:35.000000 whaox-wapi-1.1.2/wapi/features/request.py
+drwxrwxrwx   0        0        0        0 2024-05-18 05:05:52.179128 whaox-wapi-1.1.2/wapi/static/
+-rw-rw-rw-   0        0        0       48 2024-04-11 20:01:35.000000 whaox-wapi-1.1.2/wapi/static/T.py
+-rw-rw-rw-   0        0        0        0 2024-04-15 09:20:58.000000 whaox-wapi-1.1.2/wapi/static/__init__.py
+-rw-rw-rw-   0        0        0      118 2024-05-16 16:57:54.000000 whaox-wapi-1.1.2/wapi/static/methods.py
+-rw-rw-rw-   0        0        0      440 2024-05-16 17:01:19.000000 whaox-wapi-1.1.2/wapi/static/params.py
+drwxrwxrwx   0        0        0        0 2024-05-18 05:05:52.256322 whaox-wapi-1.1.2/wapi/utils/
+-rw-rw-rw-   0        0        0        0 2024-04-15 09:21:14.000000 whaox-wapi-1.1.2/wapi/utils/__init__.py
+-rw-rw-rw-   0        0        0      299 2024-05-14 15:31:03.000000 whaox-wapi-1.1.2/wapi/utils/get_path.py
+-rw-rw-rw-   0        0        0      252 2024-05-16 17:25:56.000000 whaox-wapi-1.1.2/wapi/utils/get_used_vars.py
+-rw-rw-rw-   0        0        0       54 2024-05-09 11:47:35.000000 whaox-wapi-1.1.2/wapi/utils/is_class.py
+-rw-rw-rw-   0        0        0      124 2024-04-11 20:01:35.000000 whaox-wapi-1.1.2/wapi/utils/is_dataclass.py
+-rw-rw-rw-   0        0        0       59 2024-05-09 09:32:44.000000 whaox-wapi-1.1.2/wapi/utils/is_object.py
+-rw-rw-rw-   0        0        0      311 2024-05-14 15:31:03.000000 whaox-wapi-1.1.2/wapi/utils/merge_paths.py
+-rw-rw-rw-   0        0        0      242 2024-05-14 15:31:57.000000 whaox-wapi-1.1.2/wapi/utils/set_path.py
+drwxrwxrwx   0        0        0        0 2024-05-18 05:05:52.326584 whaox-wapi-1.1.2/whaox_wapi.egg-info/
+-rw-rw-rw-   0        0        0     3072 2024-05-18 05:05:51.000000 whaox-wapi-1.1.2/whaox_wapi.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      680 2024-05-18 05:05:51.000000 whaox-wapi-1.1.2/whaox_wapi.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-18 05:05:51.000000 whaox-wapi-1.1.2/whaox_wapi.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2024-05-18 05:05:51.000000 whaox-wapi-1.1.2/whaox_wapi.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2024-05-18 05:05:51.000000 whaox-wapi-1.1.2/whaox_wapi.egg-info/top_level.txt
```

### Comparing `whaox-wapi-1.1.1/LICENSE` & `whaox-wapi-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `whaox-wapi-1.1.1/PKG-INFO` & `whaox-wapi-1.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: whaox-wapi
-Version: 1.1.1
+Version: 1.1.2
 Summary: Web-Library for Python
 Home-page: https://github.com/topanim/WApi
 Author: WHAOX
 Author-email: gorogannisan641@gmail.com
 License: MIT LICENSE, see LICENSE file
 Keywords: python,web,api,requests,post,get,put,patch,delete,rest
 Description-Content-Type: text/markdown
```

### Comparing `whaox-wapi-1.1.1/README.md` & `whaox-wapi-1.1.2/README.md`

 * *Files identical despite different names*

### Comparing `whaox-wapi-1.1.1/setup.py` & `whaox-wapi-1.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 """
 :authors: WHAOX
 :license: MIT License, see LICENSE file
 :copyright: (c) 2024 WHAOX
 """
 
-version = '1.1.1'
+version = '1.1.2'
 
 with open('README.md', encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='whaox-wapi',
     version=version,
```

### Comparing `whaox-wapi-1.1.1/wapi/features/DELETE.py` & `whaox-wapi-1.1.2/wapi/features/DELETE.py`

 * *Files identical despite different names*

### Comparing `whaox-wapi-1.1.1/wapi/features/GET.py` & `whaox-wapi-1.1.2/wapi/features/GET.py`

 * *Files identical despite different names*

### Comparing `whaox-wapi-1.1.1/wapi/features/PATCH.py` & `whaox-wapi-1.1.2/wapi/features/PATCH.py`

 * *Files identical despite different names*

### Comparing `whaox-wapi-1.1.1/wapi/features/POST.py` & `whaox-wapi-1.1.2/wapi/features/POST.py`

 * *Files identical despite different names*

### Comparing `whaox-wapi-1.1.1/wapi/features/PUT.py` & `whaox-wapi-1.1.2/wapi/features/PUT.py`

 * *Files identical despite different names*

### Comparing `whaox-wapi-1.1.1/wapi/features/Route.py` & `whaox-wapi-1.1.2/wapi/features/Route.py`

 * *Files identical despite different names*

### Comparing `whaox-wapi-1.1.1/wapi/features/request.py` & `whaox-wapi-1.1.2/wapi/features/request.py`

 * *Files identical despite different names*

### Comparing `whaox-wapi-1.1.1/whaox_wapi.egg-info/PKG-INFO` & `whaox-wapi-1.1.2/whaox_wapi.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: whaox-wapi
-Version: 1.1.1
+Version: 1.1.2
 Summary: Web-Library for Python
 Home-page: https://github.com/topanim/WApi
 Author: WHAOX
 Author-email: gorogannisan641@gmail.com
 License: MIT LICENSE, see LICENSE file
 Keywords: python,web,api,requests,post,get,put,patch,delete,rest
 Description-Content-Type: text/markdown
```

### Comparing `whaox-wapi-1.1.1/whaox_wapi.egg-info/SOURCES.txt` & `whaox-wapi-1.1.2/whaox_wapi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

