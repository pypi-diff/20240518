# Comparing `tmp/psgr-0.1.2.tar.gz` & `tmp/psgr-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "psgr-0.1.2.tar", last modified: Fri May 17 15:47:47 2024, max compression
+gzip compressed data, was "psgr-0.1.3.tar", last modified: Fri May 17 15:53:49 2024, max compression
```

## Comparing `psgr-0.1.2.tar` & `psgr-0.1.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 nareshkarthigeyan  (1000) nareshkarthigeyan  (1000)        0 2024-05-17 15:47:47.629034 psgr-0.1.2/
--rw-r--r--   0 nareshkarthigeyan  (1000) nareshkarthigeyan  (1000)      161 2024-05-17 15:47:47.629034 psgr-0.1.2/PKG-INFO
-drwxr-xr-x   0 nareshkarthigeyan  (1000) nareshkarthigeyan  (1000)        0 2024-05-17 15:47:47.629034 psgr-0.1.2/psgr/
--rw-r--r--   0 nareshkarthigeyan  (1000) nareshkarthigeyan  (1000)       19 2024-04-28 12:52:49.000000 psgr-0.1.2/psgr/__init__.py
--rw-r--r--   0 nareshkarthigeyan  (1000) nareshkarthigeyan  (1000)     8511 2024-05-17 15:32:22.000000 psgr-0.1.2/psgr/main.py
-drwxr-xr-x   0 nareshkarthigeyan  (1000) nareshkarthigeyan  (1000)        0 2024-05-17 15:47:47.629034 psgr-0.1.2/psgr.egg-info/
--rw-r--r--   0 nareshkarthigeyan  (1000) nareshkarthigeyan  (1000)      161 2024-05-17 15:47:47.000000 psgr-0.1.2/psgr.egg-info/PKG-INFO
--rw-r--r--   0 nareshkarthigeyan  (1000) nareshkarthigeyan  (1000)      208 2024-05-17 15:47:47.000000 psgr-0.1.2/psgr.egg-info/SOURCES.txt
--rw-r--r--   0 nareshkarthigeyan  (1000) nareshkarthigeyan  (1000)        1 2024-05-17 15:47:47.000000 psgr-0.1.2/psgr.egg-info/dependency_links.txt
--rw-r--r--   0 nareshkarthigeyan  (1000) nareshkarthigeyan  (1000)       46 2024-05-17 15:47:47.000000 psgr-0.1.2/psgr.egg-info/entry_points.txt
--rw-r--r--   0 nareshkarthigeyan  (1000) nareshkarthigeyan  (1000)       24 2024-05-17 15:47:47.000000 psgr-0.1.2/psgr.egg-info/requires.txt
--rw-r--r--   0 nareshkarthigeyan  (1000) nareshkarthigeyan  (1000)        5 2024-05-17 15:47:47.000000 psgr-0.1.2/psgr.egg-info/top_level.txt
--rw-r--r--   0 nareshkarthigeyan  (1000) nareshkarthigeyan  (1000)       38 2024-05-17 15:47:47.629034 psgr-0.1.2/setup.cfg
--rw-r--r--   0 nareshkarthigeyan  (1000) nareshkarthigeyan  (1000)      452 2024-05-17 15:47:42.000000 psgr-0.1.2/setup.py
+drwxr-xr-x   0 nareshkarthigeyan  (1000) nareshkarthigeyan  (1000)        0 2024-05-17 15:53:49.103437 psgr-0.1.3/
+-rw-r--r--   0 nareshkarthigeyan  (1000) nareshkarthigeyan  (1000)      161 2024-05-17 15:53:49.103437 psgr-0.1.3/PKG-INFO
+drwxr-xr-x   0 nareshkarthigeyan  (1000) nareshkarthigeyan  (1000)        0 2024-05-17 15:53:49.099437 psgr-0.1.3/psgr/
+-rw-r--r--   0 nareshkarthigeyan  (1000) nareshkarthigeyan  (1000)       19 2024-04-28 12:52:49.000000 psgr-0.1.3/psgr/__init__.py
+-rw-r--r--   0 nareshkarthigeyan  (1000) nareshkarthigeyan  (1000)     8511 2024-05-17 15:49:16.000000 psgr-0.1.3/psgr/main.py
+drwxr-xr-x   0 nareshkarthigeyan  (1000) nareshkarthigeyan  (1000)        0 2024-05-17 15:53:49.103437 psgr-0.1.3/psgr.egg-info/
+-rw-r--r--   0 nareshkarthigeyan  (1000) nareshkarthigeyan  (1000)      161 2024-05-17 15:53:49.000000 psgr-0.1.3/psgr.egg-info/PKG-INFO
+-rw-r--r--   0 nareshkarthigeyan  (1000) nareshkarthigeyan  (1000)      208 2024-05-17 15:53:49.000000 psgr-0.1.3/psgr.egg-info/SOURCES.txt
+-rw-r--r--   0 nareshkarthigeyan  (1000) nareshkarthigeyan  (1000)        1 2024-05-17 15:53:49.000000 psgr-0.1.3/psgr.egg-info/dependency_links.txt
+-rw-r--r--   0 nareshkarthigeyan  (1000) nareshkarthigeyan  (1000)       65 2024-05-17 15:53:49.000000 psgr-0.1.3/psgr.egg-info/entry_points.txt
+-rw-r--r--   0 nareshkarthigeyan  (1000) nareshkarthigeyan  (1000)       24 2024-05-17 15:53:49.000000 psgr-0.1.3/psgr.egg-info/requires.txt
+-rw-r--r--   0 nareshkarthigeyan  (1000) nareshkarthigeyan  (1000)        5 2024-05-17 15:53:49.000000 psgr-0.1.3/psgr.egg-info/top_level.txt
+-rw-r--r--   0 nareshkarthigeyan  (1000) nareshkarthigeyan  (1000)       38 2024-05-17 15:53:49.103437 psgr-0.1.3/setup.cfg
+-rw-r--r--   0 nareshkarthigeyan  (1000) nareshkarthigeyan  (1000)      485 2024-05-17 15:52:50.000000 psgr-0.1.3/setup.py
```

### Comparing `psgr-0.1.2/psgr/main.py` & `psgr-0.1.3/psgr/main.py`

 * *Files identical despite different names*

