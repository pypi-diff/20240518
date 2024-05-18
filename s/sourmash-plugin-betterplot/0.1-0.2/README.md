# Comparing `tmp/sourmash_plugin_betterplot-0.1.tar.gz` & `tmp/sourmash_plugin_betterplot-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sourmash_plugin_betterplot-0.1.tar", last modified: Fri May 17 16:21:31 2024, max compression
+gzip compressed data, was "sourmash_plugin_betterplot-0.2.tar", last modified: Sat May 18 14:55:00 2024, max compression
```

## Comparing `sourmash_plugin_betterplot-0.1.tar` & `sourmash_plugin_betterplot-0.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 t          (502) staff       (20)        0 2024-05-17 16:21:31.771959 sourmash_plugin_betterplot-0.1/
--rw-r--r--   0 t          (502) staff       (20)     1540 2024-05-17 15:38:24.000000 sourmash_plugin_betterplot-0.1/LICENSE
--rw-r--r--   0 t          (502) staff       (20)     2126 2024-05-17 16:21:31.771742 sourmash_plugin_betterplot-0.1/PKG-INFO
--rw-r--r--   0 t          (502) staff       (20)     1861 2024-05-17 16:19:55.000000 sourmash_plugin_betterplot-0.1/README.md
--rw-r--r--   0 t          (502) staff       (20)      462 2024-05-17 16:19:55.000000 sourmash_plugin_betterplot-0.1/pyproject.toml
--rw-r--r--   0 t          (502) staff       (20)       38 2024-05-17 16:21:31.771997 sourmash_plugin_betterplot-0.1/setup.cfg
-drwxr-xr-x   0 t          (502) staff       (20)        0 2024-05-17 16:21:31.770027 sourmash_plugin_betterplot-0.1/src/
-drwxr-xr-x   0 t          (502) staff       (20)        0 2024-05-17 16:21:31.771519 sourmash_plugin_betterplot-0.1/src/sourmash_plugin_betterplot.egg-info/
--rw-r--r--   0 t          (502) staff       (20)     2126 2024-05-17 16:21:31.000000 sourmash_plugin_betterplot-0.1/src/sourmash_plugin_betterplot.egg-info/PKG-INFO
--rw-r--r--   0 t          (502) staff       (20)      422 2024-05-17 16:21:31.000000 sourmash_plugin_betterplot-0.1/src/sourmash_plugin_betterplot.egg-info/SOURCES.txt
--rw-r--r--   0 t          (502) staff       (20)        1 2024-05-17 16:21:31.000000 sourmash_plugin_betterplot-0.1/src/sourmash_plugin_betterplot.egg-info/dependency_links.txt
--rw-r--r--   0 t          (502) staff       (20)       79 2024-05-17 16:21:31.000000 sourmash_plugin_betterplot-0.1/src/sourmash_plugin_betterplot.egg-info/entry_points.txt
--rw-r--r--   0 t          (502) staff       (20)       19 2024-05-17 16:21:31.000000 sourmash_plugin_betterplot-0.1/src/sourmash_plugin_betterplot.egg-info/requires.txt
--rw-r--r--   0 t          (502) staff       (20)       27 2024-05-17 16:21:31.000000 sourmash_plugin_betterplot-0.1/src/sourmash_plugin_betterplot.egg-info/top_level.txt
--rw-r--r--   0 t          (502) staff       (20)     6595 2024-05-17 16:19:55.000000 sourmash_plugin_betterplot-0.1/src/sourmash_plugin_betterplot.py
-drwxr-xr-x   0 t          (502) staff       (20)        0 2024-05-17 16:21:31.771165 sourmash_plugin_betterplot-0.1/tests/
--rw-r--r--   0 t          (502) staff       (20)      446 2024-05-17 15:38:24.000000 sourmash_plugin_betterplot-0.1/tests/test_sourmash_plugin.py
+drwxr-xr-x   0 t          (502) staff       (20)        0 2024-05-18 14:55:00.242818 sourmash_plugin_betterplot-0.2/
+-rw-r--r--   0 t          (502) staff       (20)     1540 2024-05-17 15:38:24.000000 sourmash_plugin_betterplot-0.2/LICENSE
+-rw-r--r--   0 t          (502) staff       (20)     4636 2024-05-18 14:55:00.242616 sourmash_plugin_betterplot-0.2/PKG-INFO
+-rw-r--r--   0 t          (502) staff       (20)     4275 2024-05-18 14:49:39.000000 sourmash_plugin_betterplot-0.2/README.md
+-rw-r--r--   0 t          (502) staff       (20)      512 2024-05-18 14:43:24.000000 sourmash_plugin_betterplot-0.2/pyproject.toml
+-rw-r--r--   0 t          (502) staff       (20)       38 2024-05-18 14:55:00.242855 sourmash_plugin_betterplot-0.2/setup.cfg
+drwxr-xr-x   0 t          (502) staff       (20)        0 2024-05-18 14:55:00.241049 sourmash_plugin_betterplot-0.2/src/
+drwxr-xr-x   0 t          (502) staff       (20)        0 2024-05-18 14:55:00.242409 sourmash_plugin_betterplot-0.2/src/sourmash_plugin_betterplot.egg-info/
+-rw-r--r--   0 t          (502) staff       (20)     4636 2024-05-18 14:55:00.000000 sourmash_plugin_betterplot-0.2/src/sourmash_plugin_betterplot.egg-info/PKG-INFO
+-rw-r--r--   0 t          (502) staff       (20)      422 2024-05-18 14:55:00.000000 sourmash_plugin_betterplot-0.2/src/sourmash_plugin_betterplot.egg-info/SOURCES.txt
+-rw-r--r--   0 t          (502) staff       (20)        1 2024-05-18 14:55:00.000000 sourmash_plugin_betterplot-0.2/src/sourmash_plugin_betterplot.egg-info/dependency_links.txt
+-rw-r--r--   0 t          (502) staff       (20)      132 2024-05-18 14:55:00.000000 sourmash_plugin_betterplot-0.2/src/sourmash_plugin_betterplot.egg-info/entry_points.txt
+-rw-r--r--   0 t          (502) staff       (20)       55 2024-05-18 14:55:00.000000 sourmash_plugin_betterplot-0.2/src/sourmash_plugin_betterplot.egg-info/requires.txt
+-rw-r--r--   0 t          (502) staff       (20)       27 2024-05-18 14:55:00.000000 sourmash_plugin_betterplot-0.2/src/sourmash_plugin_betterplot.egg-info/top_level.txt
+-rw-r--r--   0 t          (502) staff       (20)    13099 2024-05-18 14:41:09.000000 sourmash_plugin_betterplot-0.2/src/sourmash_plugin_betterplot.py
+drwxr-xr-x   0 t          (502) staff       (20)        0 2024-05-18 14:55:00.242117 sourmash_plugin_betterplot-0.2/tests/
+-rw-r--r--   0 t          (502) staff       (20)      446 2024-05-17 15:38:24.000000 sourmash_plugin_betterplot-0.2/tests/test_sourmash_plugin.py
```

### Comparing `sourmash_plugin_betterplot-0.1/LICENSE` & `sourmash_plugin_betterplot-0.2/LICENSE`

 * *Files identical despite different names*

