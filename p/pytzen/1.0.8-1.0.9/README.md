# Comparing `tmp/pytzen-1.0.8.tar.gz` & `tmp/pytzen-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytzen-1.0.8.tar", last modified: Fri May 10 15:32:24 2024, max compression
+gzip compressed data, was "pytzen-1.0.9.tar", last modified: Sat May 18 15:58:23 2024, max compression
```

## Comparing `pytzen-1.0.8.tar` & `pytzen-1.0.9.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 15:32:24.313382 pytzen-1.0.8/
--rw-r--r--   0 runner    (1001) docker     (127)     1078 2024-05-10 15:32:10.000000 pytzen-1.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    22948 2024-05-10 15:32:24.313382 pytzen-1.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    22454 2024-05-10 15:32:10.000000 pytzen-1.0.8/README.md
--rwxr-xr-x   0 runner    (1001) docker     (127)       84 2024-05-10 15:32:10.000000 pytzen-1.0.8/pyproject.toml
--rwxr-xr-x   0 runner    (1001) docker     (127)      571 2024-05-10 15:32:24.313382 pytzen-1.0.8/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 15:32:24.309382 pytzen-1.0.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 15:32:24.309382 pytzen-1.0.8/src/pytzen/
--rw-r--r--   0 runner    (1001) docker     (127)    22440 2024-05-10 15:32:10.000000 pytzen-1.0.8/src/pytzen/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 15:32:24.313382 pytzen-1.0.8/src/pytzen.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    22948 2024-05-10 15:32:24.000000 pytzen-1.0.8/src/pytzen.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      201 2024-05-10 15:32:24.000000 pytzen-1.0.8/src/pytzen.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 15:32:24.000000 pytzen-1.0.8/src/pytzen.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-10 15:32:24.000000 pytzen-1.0.8/src/pytzen.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 15:58:23.349414 pytzen-1.0.9/
+-rw-r--r--   0 runner    (1001) docker     (127)     1078 2024-05-18 15:58:12.000000 pytzen-1.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5482 2024-05-18 15:58:23.349414 pytzen-1.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4988 2024-05-18 15:58:12.000000 pytzen-1.0.9/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (127)       84 2024-05-18 15:58:12.000000 pytzen-1.0.9/pyproject.toml
+-rwxr-xr-x   0 runner    (1001) docker     (127)      571 2024-05-18 15:58:23.353414 pytzen-1.0.9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 15:58:23.349414 pytzen-1.0.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 15:58:23.349414 pytzen-1.0.9/src/pytzen/
+-rw-r--r--   0 runner    (1001) docker     (127)     4974 2024-05-18 15:58:12.000000 pytzen-1.0.9/src/pytzen/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 15:58:23.349414 pytzen-1.0.9/src/pytzen.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5482 2024-05-18 15:58:23.000000 pytzen-1.0.9/src/pytzen.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      201 2024-05-18 15:58:23.000000 pytzen-1.0.9/src/pytzen.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-18 15:58:23.000000 pytzen-1.0.9/src/pytzen.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-18 15:58:23.000000 pytzen-1.0.9/src/pytzen.egg-info/top_level.txt
```

### Comparing `pytzen-1.0.8/LICENSE` & `pytzen-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pytzen-1.0.8/setup.cfg` & `pytzen-1.0.9/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = pytzen
-version = 1.0.8
+version = 1.0.9
 author = PYTZEN
 description = PYTZEN is designed to sketch out data pipelines
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://pytzen.com
 project_urls = 
 	Source Code = https://github.com/pytzen/pytzen
```

