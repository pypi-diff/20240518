# Comparing `tmp/vaers-0.0.3.tar.gz` & `tmp/vaers-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/vaers-0.0.3.tar", last modified: Thu Mar 17 07:10:03 2022, max compression
+gzip compressed data, was "vaers-0.0.4.tar", last modified: Sat May 18 07:50:14 2024, max compression
```

## Comparing `vaers-0.0.3.tar` & `vaers-0.0.4.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 takefuji  (1000) takefuji  (1000)        0 2022-03-17 07:10:03.648084 vaers-0.0.3/
--rw-r--r--   0 takefuji  (1000) takefuji  (1000)     2147 2022-03-17 07:10:03.648084 vaers-0.0.3/PKG-INFO
--rw-r--r--   0 takefuji  (1000) takefuji  (1000)     1608 2022-03-17 07:09:17.000000 vaers-0.0.3/README.md
--rw-r--r--   0 takefuji  (1000) takefuji  (1000)       38 2022-03-17 07:10:03.648084 vaers-0.0.3/setup.cfg
--rw-r--r--   0 takefuji  (1000) takefuji  (1000)      950 2022-03-17 07:05:04.000000 vaers-0.0.3/setup.py
-drwxr-xr-x   0 takefuji  (1000) takefuji  (1000)        0 2022-03-17 07:10:03.629990 vaers-0.0.3/src/
-drwxr-xr-x   0 takefuji  (1000) takefuji  (1000)        0 2022-03-17 07:10:03.648084 vaers-0.0.3/src/vaers.egg-info/
--rw-r--r--   0 takefuji  (1000) takefuji  (1000)     2147 2022-03-17 07:10:03.000000 vaers-0.0.3/src/vaers.egg-info/PKG-INFO
--rw-r--r--   0 takefuji  (1000) takefuji  (1000)      199 2022-03-17 07:10:03.000000 vaers-0.0.3/src/vaers.egg-info/SOURCES.txt
--rw-r--r--   0 takefuji  (1000) takefuji  (1000)        1 2022-03-17 07:10:03.000000 vaers-0.0.3/src/vaers.egg-info/dependency_links.txt
--rw-r--r--   0 takefuji  (1000) takefuji  (1000)       38 2022-03-17 07:10:03.000000 vaers-0.0.3/src/vaers.egg-info/entry_points.txt
--rw-r--r--   0 takefuji  (1000) takefuji  (1000)        6 2022-03-17 07:10:03.000000 vaers-0.0.3/src/vaers.egg-info/top_level.txt
--rw-r--r--   0 takefuji  (1000) takefuji  (1000)     3801 2022-03-17 07:04:25.000000 vaers-0.0.3/src/vaers.py
+drwxr-xr-x   0 takefuji  (1000) takefuji  (1000)        0 2024-05-18 07:50:14.437413 vaers-0.0.4/
+-rw-r--r--   0 takefuji  (1000) takefuji  (1000)     3420 2024-05-18 07:50:14.437413 vaers-0.0.4/PKG-INFO
+-rw-r--r--   0 takefuji  (1000) takefuji  (1000)     2879 2024-05-18 07:48:51.000000 vaers-0.0.4/README.md
+-rw-r--r--   0 takefuji  (1000) takefuji  (1000)       38 2024-05-18 07:50:14.437413 vaers-0.0.4/setup.cfg
+-rw-r--r--   0 takefuji  (1000) takefuji  (1000)      952 2024-05-18 07:49:37.000000 vaers-0.0.4/setup.py
+drwxr-xr-x   0 takefuji  (1000) takefuji  (1000)        0 2024-05-18 07:50:14.437413 vaers-0.0.4/src/
+drwxr-xr-x   0 takefuji  (1000) takefuji  (1000)        0 2024-05-18 07:50:14.437413 vaers-0.0.4/src/vaers.egg-info/
+-rw-r--r--   0 takefuji  (1000) takefuji  (1000)     3420 2024-05-18 07:50:14.000000 vaers-0.0.4/src/vaers.egg-info/PKG-INFO
+-rw-r--r--   0 takefuji  (1000) takefuji  (1000)      199 2024-05-18 07:50:14.000000 vaers-0.0.4/src/vaers.egg-info/SOURCES.txt
+-rw-r--r--   0 takefuji  (1000) takefuji  (1000)        1 2024-05-18 07:50:14.000000 vaers-0.0.4/src/vaers.egg-info/dependency_links.txt
+-rw-r--r--   0 takefuji  (1000) takefuji  (1000)       38 2024-05-18 07:50:14.000000 vaers-0.0.4/src/vaers.egg-info/entry_points.txt
+-rw-r--r--   0 takefuji  (1000) takefuji  (1000)        6 2024-05-18 07:50:14.000000 vaers-0.0.4/src/vaers.egg-info/top_level.txt
+-rw-r--r--   0 takefuji  (1000) takefuji  (1000)     3801 2022-03-17 07:04:25.000000 vaers-0.0.4/src/vaers.py
```

### Comparing `vaers-0.0.3/src/vaers.py` & `vaers-0.0.4/src/vaers.py`

 * *Files identical despite different names*

