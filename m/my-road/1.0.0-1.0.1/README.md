# Comparing `tmp/my_road-1.0.0.tar.gz` & `tmp/my_road-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "my_road-1.0.0.tar", last modified: Mon May 13 22:08:58 2024, max compression
+gzip compressed data, was "my_road-1.0.1.tar", last modified: Sat May 18 20:38:32 2024, max compression
```

## Comparing `my_road-1.0.0.tar` & `my_road-1.0.1.tar`

### file list

```diff
@@ -1,11 +1,12 @@
-drwxrwxrwx   0        0        0        0 2024-05-13 22:08:58.032717 my_road-1.0.0/
--rw-rw-rw-   0        0        0     1088 2024-05-13 21:55:30.000000 my_road-1.0.0/LICENSE
--rw-rw-rw-   0        0        0    26063 2024-05-13 22:08:58.031718 my_road-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0    25852 2024-05-13 22:08:39.000000 my_road-1.0.0/README.md
-drwxrwxrwx   0        0        0        0 2024-05-13 22:08:58.030715 my_road-1.0.0/my_road.egg-info/
--rw-rw-rw-   0        0        0    26063 2024-05-13 22:08:57.000000 my_road-1.0.0/my_road.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      150 2024-05-13 22:08:58.000000 my_road-1.0.0/my_road.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-13 22:08:57.000000 my_road-1.0.0/my_road.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        5 2024-05-13 22:08:57.000000 my_road-1.0.0/my_road.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-13 22:08:58.032717 my_road-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0      349 2024-05-13 21:59:34.000000 my_road-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-18 20:38:32.556113 my_road-1.0.1/
+-rw-rw-rw-   0        0        0     1088 2024-05-13 21:55:30.000000 my_road-1.0.1/LICENSE
+-rw-rw-rw-   0        0        0    26063 2024-05-18 20:38:32.555115 my_road-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0    25852 2024-05-13 22:08:39.000000 my_road-1.0.1/README.md
+drwxrwxrwx   0        0        0        0 2024-05-18 20:38:32.554114 my_road-1.0.1/my_road.egg-info/
+-rw-rw-rw-   0        0        0    26063 2024-05-18 20:38:32.000000 my_road-1.0.1/my_road.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      158 2024-05-18 20:38:32.000000 my_road-1.0.1/my_road.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-18 20:38:32.000000 my_road-1.0.1/my_road.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        5 2024-05-18 20:38:32.000000 my_road-1.0.1/my_road.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      621 2024-05-13 22:08:39.000000 my_road-1.0.1/road.py
+-rw-rw-rw-   0        0        0       42 2024-05-18 20:38:32.556113 my_road-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0      349 2024-05-18 20:38:26.000000 my_road-1.0.1/setup.py
```

### Comparing `my_road-1.0.0/LICENSE` & `my_road-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `my_road-1.0.0/PKG-INFO` & `my_road-1.0.1/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: my_road
-Version: 1.0.0
+Version: 1.0.1
 Summary: Look at the road
 Author: k0ng999
 Author-email: baydar_14@mail.ru
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `my_road-1.0.0/README.md` & `my_road-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `my_road-1.0.0/my_road.egg-info/PKG-INFO` & `my_road-1.0.1/my_road.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: my_road
-Version: 1.0.0
+Version: 1.0.1
 Summary: Look at the road
 Author: k0ng999
 Author-email: baydar_14@mail.ru
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

