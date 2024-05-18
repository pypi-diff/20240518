# Comparing `tmp/flet_easy_static-0.1.tar.gz` & `tmp/flet_easy_static-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flet_easy_static-0.1.tar", last modified: Sat May 18 14:24:25 2024, max compression
+gzip compressed data, was "flet_easy_static-0.2.tar", last modified: Sat May 18 14:29:54 2024, max compression
```

## Comparing `flet_easy_static-0.1.tar` & `flet_easy_static-0.2.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2024-05-18 14:24:25.795995 flet_easy_static-0.1/
--rw-rw-rw-   0        0        0       61 2024-05-18 14:24:25.794998 flet_easy_static-0.1/PKG-INFO
--rw-rw-rw-   0        0        0     6461 2024-05-18 14:21:37.000000 flet_easy_static-0.1/README.md
-drwxrwxrwx   0        0        0        0 2024-05-18 14:24:25.778044 flet_easy_static-0.1/flet_easy_static/
--rw-rw-rw-   0        0        0      481 2024-05-18 13:38:21.000000 flet_easy_static-0.1/flet_easy_static/__init__.py
--rw-rw-rw-   0        0        0     1289 2024-05-18 13:38:21.000000 flet_easy_static-0.1/flet_easy_static/auto_route.py
--rw-rw-rw-   0        0        0    12267 2024-05-18 13:36:12.000000 flet_easy_static-0.1/flet_easy_static/datasy.py
--rw-rw-rw-   0        0        0      187 2024-05-05 15:12:55.000000 flet_easy_static-0.1/flet_easy_static/extra.py
--rw-rw-rw-   0        0        0     2483 2024-05-05 15:12:55.000000 flet_easy_static-0.1/flet_easy_static/extrasJwt.py
--rw-rw-rw-   0        0        0    18469 2024-05-18 13:33:23.000000 flet_easy_static-0.1/flet_easy_static/fletEasy.py
--rw-rw-rw-   0        0        0     9856 2024-05-05 15:12:55.000000 flet_easy_static-0.1/flet_easy_static/inheritance.py
--rw-rw-rw-   0        0        0     1191 2024-05-05 15:12:55.000000 flet_easy_static-0.1/flet_easy_static/job.py
--rw-rw-rw-   0        0        0     4045 2024-05-18 13:36:12.000000 flet_easy_static-0.1/flet_easy_static/jwt.py
--rw-rw-rw-   0        0        0     7526 2024-05-18 13:36:12.000000 flet_easy_static-0.1/flet_easy_static/pagesy.py
--rw-rw-rw-   0        0        0    11213 2024-05-18 13:36:12.000000 flet_easy_static-0.1/flet_easy_static/route.py
--rw-rw-rw-   0        0        0     1540 2024-05-05 15:12:55.000000 flet_easy_static-0.1/flet_easy_static/view_404.py
-drwxrwxrwx   0        0        0        0 2024-05-18 14:24:25.794001 flet_easy_static-0.1/flet_easy_static.egg-info/
--rw-rw-rw-   0        0        0       61 2024-05-18 14:24:25.000000 flet_easy_static-0.1/flet_easy_static.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      551 2024-05-18 14:24:25.000000 flet_easy_static-0.1/flet_easy_static.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-18 14:24:25.000000 flet_easy_static-0.1/flet_easy_static.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        5 2024-05-18 14:24:25.000000 flet_easy_static-0.1/flet_easy_static.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2024-05-18 14:24:25.000000 flet_easy_static-0.1/flet_easy_static.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-18 14:24:25.795995 flet_easy_static-0.1/setup.cfg
--rw-rw-rw-   0        0        0      186 2024-05-18 14:02:00.000000 flet_easy_static-0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-18 14:29:54.519062 flet_easy_static-0.2/
+-rw-rw-rw-   0        0        0     6623 2024-05-18 14:29:54.519062 flet_easy_static-0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     6461 2024-05-18 14:21:37.000000 flet_easy_static-0.2/README.md
+drwxrwxrwx   0        0        0        0 2024-05-18 14:29:54.497068 flet_easy_static-0.2/flet_easy_static/
+-rw-rw-rw-   0        0        0      481 2024-05-18 13:38:21.000000 flet_easy_static-0.2/flet_easy_static/__init__.py
+-rw-rw-rw-   0        0        0     1289 2024-05-18 13:38:21.000000 flet_easy_static-0.2/flet_easy_static/auto_route.py
+-rw-rw-rw-   0        0        0    12267 2024-05-18 13:36:12.000000 flet_easy_static-0.2/flet_easy_static/datasy.py
+-rw-rw-rw-   0        0        0      187 2024-05-05 15:12:55.000000 flet_easy_static-0.2/flet_easy_static/extra.py
+-rw-rw-rw-   0        0        0     2483 2024-05-05 15:12:55.000000 flet_easy_static-0.2/flet_easy_static/extrasJwt.py
+-rw-rw-rw-   0        0        0    18469 2024-05-18 13:33:23.000000 flet_easy_static-0.2/flet_easy_static/fletEasy.py
+-rw-rw-rw-   0        0        0     9856 2024-05-05 15:12:55.000000 flet_easy_static-0.2/flet_easy_static/inheritance.py
+-rw-rw-rw-   0        0        0     1191 2024-05-05 15:12:55.000000 flet_easy_static-0.2/flet_easy_static/job.py
+-rw-rw-rw-   0        0        0     4045 2024-05-18 13:36:12.000000 flet_easy_static-0.2/flet_easy_static/jwt.py
+-rw-rw-rw-   0        0        0     7526 2024-05-18 13:36:12.000000 flet_easy_static-0.2/flet_easy_static/pagesy.py
+-rw-rw-rw-   0        0        0    11213 2024-05-18 13:36:12.000000 flet_easy_static-0.2/flet_easy_static/route.py
+-rw-rw-rw-   0        0        0     1540 2024-05-05 15:12:55.000000 flet_easy_static-0.2/flet_easy_static/view_404.py
+drwxrwxrwx   0        0        0        0 2024-05-18 14:29:54.518065 flet_easy_static-0.2/flet_easy_static.egg-info/
+-rw-rw-rw-   0        0        0     6623 2024-05-18 14:29:54.000000 flet_easy_static-0.2/flet_easy_static.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      551 2024-05-18 14:29:54.000000 flet_easy_static-0.2/flet_easy_static.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-18 14:29:54.000000 flet_easy_static-0.2/flet_easy_static.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        5 2024-05-18 14:29:54.000000 flet_easy_static-0.2/flet_easy_static.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2024-05-18 14:29:54.000000 flet_easy_static-0.2/flet_easy_static.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-18 14:29:54.520060 flet_easy_static-0.2/setup.cfg
+-rw-rw-rw-   0        0        0      343 2024-05-18 14:29:46.000000 flet_easy_static-0.2/setup.py
```

### Comparing `flet_easy_static-0.1/README.md` & `flet_easy_static-0.2/README.md`

 * *Files identical despite different names*

### Comparing `flet_easy_static-0.1/flet_easy_static/auto_route.py` & `flet_easy_static-0.2/flet_easy_static/auto_route.py`

 * *Files identical despite different names*

### Comparing `flet_easy_static-0.1/flet_easy_static/datasy.py` & `flet_easy_static-0.2/flet_easy_static/datasy.py`

 * *Files identical despite different names*

### Comparing `flet_easy_static-0.1/flet_easy_static/extrasJwt.py` & `flet_easy_static-0.2/flet_easy_static/extrasJwt.py`

 * *Files identical despite different names*

### Comparing `flet_easy_static-0.1/flet_easy_static/fletEasy.py` & `flet_easy_static-0.2/flet_easy_static/fletEasy.py`

 * *Files identical despite different names*

### Comparing `flet_easy_static-0.1/flet_easy_static/inheritance.py` & `flet_easy_static-0.2/flet_easy_static/inheritance.py`

 * *Files identical despite different names*

### Comparing `flet_easy_static-0.1/flet_easy_static/job.py` & `flet_easy_static-0.2/flet_easy_static/job.py`

 * *Files identical despite different names*

### Comparing `flet_easy_static-0.1/flet_easy_static/jwt.py` & `flet_easy_static-0.2/flet_easy_static/jwt.py`

 * *Files identical despite different names*

### Comparing `flet_easy_static-0.1/flet_easy_static/pagesy.py` & `flet_easy_static-0.2/flet_easy_static/pagesy.py`

 * *Files identical despite different names*

### Comparing `flet_easy_static-0.1/flet_easy_static/route.py` & `flet_easy_static-0.2/flet_easy_static/route.py`

 * *Files identical despite different names*

### Comparing `flet_easy_static-0.1/flet_easy_static/view_404.py` & `flet_easy_static-0.2/flet_easy_static/view_404.py`

 * *Files identical despite different names*

### Comparing `flet_easy_static-0.1/flet_easy_static.egg-info/SOURCES.txt` & `flet_easy_static-0.2/flet_easy_static.egg-info/SOURCES.txt`

 * *Files identical despite different names*

