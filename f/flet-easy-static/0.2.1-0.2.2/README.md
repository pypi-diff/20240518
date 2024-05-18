# Comparing `tmp/flet_easy_static-0.2.1.tar.gz` & `tmp/flet_easy_static-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flet_easy_static-0.2.1.tar", last modified: Sat May 18 17:04:36 2024, max compression
+gzip compressed data, was "flet_easy_static-0.2.2.tar", last modified: Sat May 18 17:09:21 2024, max compression
```

## Comparing `flet_easy_static-0.2.1.tar` & `flet_easy_static-0.2.2.tar`

### file list

```diff
@@ -1,24 +1,23 @@
-drwxrwxrwx   0        0        0        0 2024-05-18 17:04:36.740773 flet_easy_static-0.2.1/
--rw-rw-rw-   0        0        0     6625 2024-05-18 17:04:36.739776 flet_easy_static-0.2.1/PKG-INFO
--rw-rw-rw-   0        0        0     6461 2024-05-18 14:21:37.000000 flet_easy_static-0.2.1/README.md
-drwxrwxrwx   0        0        0        0 2024-05-18 17:04:36.713846 flet_easy_static-0.2.1/flet_easy_static/
--rw-rw-rw-   0        0        0      481 2024-05-18 13:38:21.000000 flet_easy_static-0.2.1/flet_easy_static/__init__.py
--rw-rw-rw-   0        0        0     1289 2024-05-18 13:38:21.000000 flet_easy_static-0.2.1/flet_easy_static/auto_route.py
--rw-rw-rw-   0        0        0    12267 2024-05-18 13:36:12.000000 flet_easy_static-0.2.1/flet_easy_static/datasy.py
--rw-rw-rw-   0        0        0      187 2024-05-05 15:12:55.000000 flet_easy_static-0.2.1/flet_easy_static/extra.py
--rw-rw-rw-   0        0        0     2483 2024-05-05 15:12:55.000000 flet_easy_static-0.2.1/flet_easy_static/extrasJwt.py
--rw-rw-rw-   0        0        0    18475 2024-05-18 17:04:32.000000 flet_easy_static-0.2.1/flet_easy_static/fletEasy.py
--rw-rw-rw-   0        0        0     9856 2024-05-05 15:12:55.000000 flet_easy_static-0.2.1/flet_easy_static/inheritance.py
--rw-rw-rw-   0        0        0     1191 2024-05-05 15:12:55.000000 flet_easy_static-0.2.1/flet_easy_static/job.py
--rw-rw-rw-   0        0        0     4045 2024-05-18 13:36:12.000000 flet_easy_static-0.2.1/flet_easy_static/jwt.py
--rw-rw-rw-   0        0        0     7526 2024-05-18 13:36:12.000000 flet_easy_static-0.2.1/flet_easy_static/pagesy.py
--rw-rw-rw-   0        0        0    11213 2024-05-18 13:36:12.000000 flet_easy_static-0.2.1/flet_easy_static/route.py
--rw-rw-rw-   0        0        0     1540 2024-05-05 15:12:55.000000 flet_easy_static-0.2.1/flet_easy_static/view_404.py
-drwxrwxrwx   0        0        0        0 2024-05-18 17:04:36.738779 flet_easy_static-0.2.1/flet_easy_static.egg-info/
--rw-rw-rw-   0        0        0     6625 2024-05-18 17:04:36.000000 flet_easy_static-0.2.1/flet_easy_static.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      551 2024-05-18 17:04:36.000000 flet_easy_static-0.2.1/flet_easy_static.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-18 17:04:36.000000 flet_easy_static-0.2.1/flet_easy_static.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        5 2024-05-18 17:04:36.000000 flet_easy_static-0.2.1/flet_easy_static.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2024-05-18 17:04:36.000000 flet_easy_static-0.2.1/flet_easy_static.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-18 17:04:36.740773 flet_easy_static-0.2.1/setup.cfg
--rw-rw-rw-   0        0        0      345 2024-05-18 17:04:32.000000 flet_easy_static-0.2.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-18 17:09:21.622442 flet_easy_static-0.2.2/
+-rw-rw-rw-   0        0        0     6625 2024-05-18 17:09:21.621444 flet_easy_static-0.2.2/PKG-INFO
+-rw-rw-rw-   0        0        0     6461 2024-05-18 14:21:37.000000 flet_easy_static-0.2.2/README.md
+drwxrwxrwx   0        0        0        0 2024-05-18 17:09:21.610472 flet_easy_static-0.2.2/flet_easy_static/
+-rw-rw-rw-   0        0        0      481 2024-05-18 13:38:21.000000 flet_easy_static-0.2.2/flet_easy_static/__init__.py
+-rw-rw-rw-   0        0        0     1289 2024-05-18 13:38:21.000000 flet_easy_static-0.2.2/flet_easy_static/auto_route.py
+-rw-rw-rw-   0        0        0    12267 2024-05-18 13:36:12.000000 flet_easy_static-0.2.2/flet_easy_static/datasy.py
+-rw-rw-rw-   0        0        0      187 2024-05-05 15:12:55.000000 flet_easy_static-0.2.2/flet_easy_static/extra.py
+-rw-rw-rw-   0        0        0     2483 2024-05-05 15:12:55.000000 flet_easy_static-0.2.2/flet_easy_static/extrasJwt.py
+-rw-rw-rw-   0        0        0    18475 2024-05-18 17:04:32.000000 flet_easy_static-0.2.2/flet_easy_static/fletEasy.py
+-rw-rw-rw-   0        0        0     9856 2024-05-05 15:12:55.000000 flet_easy_static-0.2.2/flet_easy_static/inheritance.py
+-rw-rw-rw-   0        0        0     1191 2024-05-05 15:12:55.000000 flet_easy_static-0.2.2/flet_easy_static/job.py
+-rw-rw-rw-   0        0        0     4045 2024-05-18 13:36:12.000000 flet_easy_static-0.2.2/flet_easy_static/jwt.py
+-rw-rw-rw-   0        0        0     7526 2024-05-18 13:36:12.000000 flet_easy_static-0.2.2/flet_easy_static/pagesy.py
+-rw-rw-rw-   0        0        0    11213 2024-05-18 13:36:12.000000 flet_easy_static-0.2.2/flet_easy_static/route.py
+-rw-rw-rw-   0        0        0     1540 2024-05-05 15:12:55.000000 flet_easy_static-0.2.2/flet_easy_static/view_404.py
+drwxrwxrwx   0        0        0        0 2024-05-18 17:09:21.620447 flet_easy_static-0.2.2/flet_easy_static.egg-info/
+-rw-rw-rw-   0        0        0     6625 2024-05-18 17:09:21.000000 flet_easy_static-0.2.2/flet_easy_static.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      512 2024-05-18 17:09:21.000000 flet_easy_static-0.2.2/flet_easy_static.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-18 17:09:21.000000 flet_easy_static-0.2.2/flet_easy_static.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2024-05-18 17:09:21.000000 flet_easy_static-0.2.2/flet_easy_static.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-18 17:09:21.622442 flet_easy_static-0.2.2/setup.cfg
+-rw-rw-rw-   0        0        0      347 2024-05-18 17:08:39.000000 flet_easy_static-0.2.2/setup.py
```

### Comparing `flet_easy_static-0.2.1/PKG-INFO` & `flet_easy_static-0.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flet_easy_static
-Version: 0.2.1
+Version: 0.2.2
 Description-Content-Type: text/markdown
 
 <div align="center">
     <img src="https://github.com/Daxexs/flet-easy/blob/main/media/logo.png?raw=true" alt="logo" width="250">
 </div>
```

### Comparing `flet_easy_static-0.2.1/README.md` & `flet_easy_static-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `flet_easy_static-0.2.1/flet_easy_static/auto_route.py` & `flet_easy_static-0.2.2/flet_easy_static/auto_route.py`

 * *Files identical despite different names*

### Comparing `flet_easy_static-0.2.1/flet_easy_static/datasy.py` & `flet_easy_static-0.2.2/flet_easy_static/datasy.py`

 * *Files identical despite different names*

### Comparing `flet_easy_static-0.2.1/flet_easy_static/extrasJwt.py` & `flet_easy_static-0.2.2/flet_easy_static/extrasJwt.py`

 * *Files identical despite different names*

### Comparing `flet_easy_static-0.2.1/flet_easy_static/fletEasy.py` & `flet_easy_static-0.2.2/flet_easy_static/fletEasy.py`

 * *Files identical despite different names*

### Comparing `flet_easy_static-0.2.1/flet_easy_static/inheritance.py` & `flet_easy_static-0.2.2/flet_easy_static/inheritance.py`

 * *Files identical despite different names*

### Comparing `flet_easy_static-0.2.1/flet_easy_static/job.py` & `flet_easy_static-0.2.2/flet_easy_static/job.py`

 * *Files identical despite different names*

### Comparing `flet_easy_static-0.2.1/flet_easy_static/jwt.py` & `flet_easy_static-0.2.2/flet_easy_static/jwt.py`

 * *Files identical despite different names*

### Comparing `flet_easy_static-0.2.1/flet_easy_static/pagesy.py` & `flet_easy_static-0.2.2/flet_easy_static/pagesy.py`

 * *Files identical despite different names*

### Comparing `flet_easy_static-0.2.1/flet_easy_static/route.py` & `flet_easy_static-0.2.2/flet_easy_static/route.py`

 * *Files identical despite different names*

### Comparing `flet_easy_static-0.2.1/flet_easy_static/view_404.py` & `flet_easy_static-0.2.2/flet_easy_static/view_404.py`

 * *Files identical despite different names*

### Comparing `flet_easy_static-0.2.1/flet_easy_static.egg-info/PKG-INFO` & `flet_easy_static-0.2.2/flet_easy_static.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flet-easy-static
-Version: 0.2.1
+Version: 0.2.2
 Description-Content-Type: text/markdown
 
 <div align="center">
     <img src="https://github.com/Daxexs/flet-easy/blob/main/media/logo.png?raw=true" alt="logo" width="250">
 </div>
```

### Comparing `flet_easy_static-0.2.1/flet_easy_static.egg-info/SOURCES.txt` & `flet_easy_static-0.2.2/flet_easy_static.egg-info/SOURCES.txt`

 * *Files 13% similar despite different names*

```diff
@@ -11,9 +11,8 @@
 flet_easy_static/jwt.py
 flet_easy_static/pagesy.py
 flet_easy_static/route.py
 flet_easy_static/view_404.py
 flet_easy_static.egg-info/PKG-INFO
 flet_easy_static.egg-info/SOURCES.txt
 flet_easy_static.egg-info/dependency_links.txt
-flet_easy_static.egg-info/requires.txt
 flet_easy_static.egg-info/top_level.txt
```

