# Comparing `tmp/twinlib-0.1.6.tar.gz` & `tmp/twinlib-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "twinlib-0.1.6.tar", last modified: Sat May 18 16:14:43 2024, max compression
+gzip compressed data, was "twinlib-0.1.7.tar", last modified: Sat May 18 16:25:41 2024, max compression
```

## Comparing `twinlib-0.1.6.tar` & `twinlib-0.1.7.tar`

### file list

```diff
@@ -1,13 +1,14 @@
-drwxr-xr-x   0 gaia      (1000) gaia      (1000)        0 2024-05-18 16:14:43.889055 twinlib-0.1.6/
--rw-r--r--   0 gaia      (1000) gaia      (1000)      281 2024-05-18 16:14:43.889055 twinlib-0.1.6/PKG-INFO
--rw-r--r--   0 gaia      (1000) gaia      (1000)        0 2024-05-17 10:08:09.000000 twinlib-0.1.6/README.md
--rw-r--r--   0 gaia      (1000) gaia      (1000)       38 2024-05-18 16:14:43.889055 twinlib-0.1.6/setup.cfg
--rw-r--r--   0 gaia      (1000) gaia      (1000)      453 2024-05-18 16:11:57.000000 twinlib-0.1.6/setup.py
-drwxr-xr-x   0 gaia      (1000) gaia      (1000)        0 2024-05-18 16:14:43.889055 twinlib-0.1.6/twinlib.egg-info/
--rw-r--r--   0 gaia      (1000) gaia      (1000)      281 2024-05-18 16:14:43.000000 twinlib-0.1.6/twinlib.egg-info/PKG-INFO
--rw-r--r--   0 gaia      (1000) gaia      (1000)      186 2024-05-18 16:14:43.000000 twinlib-0.1.6/twinlib.egg-info/SOURCES.txt
--rw-r--r--   0 gaia      (1000) gaia      (1000)        1 2024-05-18 16:14:43.000000 twinlib-0.1.6/twinlib.egg-info/dependency_links.txt
--rw-r--r--   0 gaia      (1000) gaia      (1000)       12 2024-05-18 16:14:43.000000 twinlib-0.1.6/twinlib.egg-info/top_level.txt
-drwxr-xr-x   0 gaia      (1000) gaia      (1000)        0 2024-05-18 16:14:43.889055 twinlib-0.1.6/twinlib_pkg/
--rw-r--r--   0 gaia      (1000) gaia      (1000)       23 2024-05-18 16:03:24.000000 twinlib-0.1.6/twinlib_pkg/__init__.py
--rw-r--r--   0 gaia      (1000) gaia      (1000)       38 2024-05-18 16:03:05.000000 twinlib-0.1.6/twinlib_pkg/main.py
+drwxr-xr-x   0 gaia      (1000) gaia      (1000)        0 2024-05-18 16:25:41.291061 twinlib-0.1.7/
+-rw-r--r--   0 gaia      (1000) gaia      (1000)      281 2024-05-18 16:25:41.291061 twinlib-0.1.7/PKG-INFO
+-rw-r--r--   0 gaia      (1000) gaia      (1000)        0 2024-05-17 10:08:09.000000 twinlib-0.1.7/README.md
+-rw-r--r--   0 gaia      (1000) gaia      (1000)       38 2024-05-18 16:25:41.291061 twinlib-0.1.7/setup.cfg
+-rw-r--r--   0 gaia      (1000) gaia      (1000)      556 2024-05-18 16:25:18.000000 twinlib-0.1.7/setup.py
+drwxr-xr-x   0 gaia      (1000) gaia      (1000)        0 2024-05-18 16:25:41.291061 twinlib-0.1.7/twinlib.egg-info/
+-rw-r--r--   0 gaia      (1000) gaia      (1000)      281 2024-05-18 16:25:41.000000 twinlib-0.1.7/twinlib.egg-info/PKG-INFO
+-rw-r--r--   0 gaia      (1000) gaia      (1000)      220 2024-05-18 16:25:41.000000 twinlib-0.1.7/twinlib.egg-info/SOURCES.txt
+-rw-r--r--   0 gaia      (1000) gaia      (1000)        1 2024-05-18 16:25:41.000000 twinlib-0.1.7/twinlib.egg-info/dependency_links.txt
+-rw-r--r--   0 gaia      (1000) gaia      (1000)       46 2024-05-18 16:25:41.000000 twinlib-0.1.7/twinlib.egg-info/entry_points.txt
+-rw-r--r--   0 gaia      (1000) gaia      (1000)       12 2024-05-18 16:25:41.000000 twinlib-0.1.7/twinlib.egg-info/top_level.txt
+drwxr-xr-x   0 gaia      (1000) gaia      (1000)        0 2024-05-18 16:25:41.291061 twinlib-0.1.7/twinlib_pkg/
+-rw-r--r--   0 gaia      (1000) gaia      (1000)       23 2024-05-18 16:03:24.000000 twinlib-0.1.7/twinlib_pkg/__init__.py
+-rw-r--r--   0 gaia      (1000) gaia      (1000)       38 2024-05-18 16:03:05.000000 twinlib-0.1.7/twinlib_pkg/main.py
```

