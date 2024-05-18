# Comparing `tmp/my_road-1.0.1.tar.gz` & `tmp/my_road-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "my_road-1.0.1.tar", last modified: Sat May 18 20:38:32 2024, max compression
+gzip compressed data, was "my_road-1.0.2.tar", last modified: Sat May 18 21:05:52 2024, max compression
```

## Comparing `my_road-1.0.1.tar` & `my_road-1.0.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2024-05-18 20:38:32.556113 my_road-1.0.1/
--rw-rw-rw-   0        0        0     1088 2024-05-13 21:55:30.000000 my_road-1.0.1/LICENSE
--rw-rw-rw-   0        0        0    26063 2024-05-18 20:38:32.555115 my_road-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0    25852 2024-05-13 22:08:39.000000 my_road-1.0.1/README.md
-drwxrwxrwx   0        0        0        0 2024-05-18 20:38:32.554114 my_road-1.0.1/my_road.egg-info/
--rw-rw-rw-   0        0        0    26063 2024-05-18 20:38:32.000000 my_road-1.0.1/my_road.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      158 2024-05-18 20:38:32.000000 my_road-1.0.1/my_road.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-18 20:38:32.000000 my_road-1.0.1/my_road.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        5 2024-05-18 20:38:32.000000 my_road-1.0.1/my_road.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      621 2024-05-13 22:08:39.000000 my_road-1.0.1/road.py
--rw-rw-rw-   0        0        0       42 2024-05-18 20:38:32.556113 my_road-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0      349 2024-05-18 20:38:26.000000 my_road-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-18 21:05:52.562731 my_road-1.0.2/
+-rw-rw-rw-   0        0        0     1088 2024-05-13 21:55:30.000000 my_road-1.0.2/LICENSE
+-rw-rw-rw-   0        0        0     2126 2024-05-18 21:05:52.561732 my_road-1.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1915 2024-05-18 21:05:47.000000 my_road-1.0.2/README.md
+-rw-rw-rw-   0        0        0       61 2024-05-18 21:03:21.000000 my_road-1.0.2/my_decimal.py
+drwxrwxrwx   0        0        0        0 2024-05-18 21:05:52.560731 my_road-1.0.2/my_road.egg-info/
+-rw-rw-rw-   0        0        0     2126 2024-05-18 21:05:52.000000 my_road-1.0.2/my_road.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      164 2024-05-18 21:05:52.000000 my_road-1.0.2/my_road.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-18 21:05:52.000000 my_road-1.0.2/my_road.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2024-05-18 21:05:52.000000 my_road-1.0.2/my_road.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-18 21:05:52.562731 my_road-1.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      355 2024-05-18 21:03:21.000000 my_road-1.0.2/setup.py
```

### Comparing `my_road-1.0.1/LICENSE` & `my_road-1.0.2/LICENSE`

 * *Files identical despite different names*

