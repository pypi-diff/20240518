# Comparing `tmp/baosight-0.0.2.tar.gz` & `tmp/baosight-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "baosight-0.0.2.tar", last modified: Sat May 18 18:16:11 2024, max compression
+gzip compressed data, was "baosight-0.0.3.tar", last modified: Sat May 18 18:19:11 2024, max compression
```

## Comparing `baosight-0.0.2.tar` & `baosight-0.0.3.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxrwx   0        0        0        0 2024-05-18 18:16:11.763516 baosight-0.0.2/
--rw-rw-rw-   0        0        0     1064 2023-10-25 05:23:47.000000 baosight-0.0.2/LICENSE
--rw-rw-rw-   0        0        0      126 2024-05-18 18:14:34.000000 baosight-0.0.2/MANIFEST.in
--rw-rw-rw-   0        0        0     4904 2024-05-18 18:16:11.762517 baosight-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     4225 2024-02-20 09:06:02.000000 baosight-0.0.2/README.md
-drwxrwxrwx   0        0        0        0 2024-05-18 18:16:11.722895 baosight-0.0.2/baosight/
--rw-rw-rw-   0        0        0        0 2024-05-18 17:41:58.000000 baosight-0.0.2/baosight/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-18 18:16:11.754482 baosight-0.0.2/baosight/cli/
--rw-rw-rw-   0        0        0        0 2023-10-25 05:23:47.000000 baosight-0.0.2/baosight/cli/__init__.py
--rw-rw-rw-   0        0        0     1100 2024-05-18 18:04:07.000000 baosight-0.0.2/baosight/cli/gl_runner.py
--rw-rw-rw-   0        0        0     1418 2024-05-18 18:01:43.000000 baosight-0.0.2/baosight/cli/main.py
-drwxrwxrwx   0        0        0        0 2024-05-18 18:16:11.758484 baosight-0.0.2/baosight/tools/
--rw-rw-rw-   0        0        0        0 2024-05-18 17:42:50.000000 baosight-0.0.2/baosight/tools/__init__.py
--rw-rw-rw-   0        0        0     4563 2024-05-18 17:44:00.000000 baosight-0.0.2/baosight/tools/gitlab_runner.py
--rw-rw-rw-   0        0        0     7139 2024-05-18 17:36:06.000000 baosight-0.0.2/baosight/tools/gitlab_runner_gui.py
-drwxrwxrwx   0        0        0        0 2024-05-18 18:16:11.760487 baosight-0.0.2/baosight.egg-info/
--rw-rw-rw-   0        0        0     4904 2024-05-18 18:16:11.000000 baosight-0.0.2/baosight.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      461 2024-05-18 18:16:11.000000 baosight-0.0.2/baosight.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-18 18:16:11.000000 baosight-0.0.2/baosight.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       52 2024-05-18 18:16:11.000000 baosight-0.0.2/baosight.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2024-05-18 18:16:11.000000 baosight-0.0.2/baosight.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       57 2024-05-18 18:16:11.000000 baosight-0.0.2/baosight.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-05-18 18:16:11.000000 baosight-0.0.2/baosight.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      666 2024-05-18 18:16:11.766487 baosight-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0      171 2024-05-18 18:10:58.000000 baosight-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-18 18:19:11.100153 baosight-0.0.3/
+-rw-rw-rw-   0        0        0     1064 2023-10-25 05:23:47.000000 baosight-0.0.3/LICENSE
+-rw-rw-rw-   0        0        0      126 2024-05-18 18:14:34.000000 baosight-0.0.3/MANIFEST.in
+-rw-rw-rw-   0        0        0      783 2024-05-18 18:19:11.099154 baosight-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0      199 2024-05-18 18:18:59.000000 baosight-0.0.3/README.md
+drwxrwxrwx   0        0        0        0 2024-05-18 18:19:11.067151 baosight-0.0.3/baosight/
+-rw-rw-rw-   0        0        0        0 2024-05-18 17:41:58.000000 baosight-0.0.3/baosight/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-18 18:19:11.093151 baosight-0.0.3/baosight/cli/
+-rw-rw-rw-   0        0        0        0 2023-10-25 05:23:47.000000 baosight-0.0.3/baosight/cli/__init__.py
+-rw-rw-rw-   0        0        0     1100 2024-05-18 18:04:07.000000 baosight-0.0.3/baosight/cli/gl_runner.py
+-rw-rw-rw-   0        0        0     1418 2024-05-18 18:01:43.000000 baosight-0.0.3/baosight/cli/main.py
+drwxrwxrwx   0        0        0        0 2024-05-18 18:19:11.096151 baosight-0.0.3/baosight/tools/
+-rw-rw-rw-   0        0        0        0 2024-05-18 17:42:50.000000 baosight-0.0.3/baosight/tools/__init__.py
+-rw-rw-rw-   0        0        0     4563 2024-05-18 17:44:00.000000 baosight-0.0.3/baosight/tools/gitlab_runner.py
+-rw-rw-rw-   0        0        0     7139 2024-05-18 17:36:06.000000 baosight-0.0.3/baosight/tools/gitlab_runner_gui.py
+drwxrwxrwx   0        0        0        0 2024-05-18 18:19:11.098159 baosight-0.0.3/baosight.egg-info/
+-rw-rw-rw-   0        0        0      783 2024-05-18 18:19:11.000000 baosight-0.0.3/baosight.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      461 2024-05-18 18:19:11.000000 baosight-0.0.3/baosight.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-18 18:19:11.000000 baosight-0.0.3/baosight.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       52 2024-05-18 18:19:11.000000 baosight-0.0.3/baosight.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2024-05-18 18:19:10.000000 baosight-0.0.3/baosight.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       57 2024-05-18 18:19:11.000000 baosight-0.0.3/baosight.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-05-18 18:19:11.000000 baosight-0.0.3/baosight.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      666 2024-05-18 18:19:11.102154 baosight-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      171 2024-05-18 18:10:58.000000 baosight-0.0.3/setup.py
```

### Comparing `baosight-0.0.2/LICENSE` & `baosight-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `baosight-0.0.2/baosight/cli/gl_runner.py` & `baosight-0.0.3/baosight/cli/gl_runner.py`

 * *Files identical despite different names*

### Comparing `baosight-0.0.2/baosight/cli/main.py` & `baosight-0.0.3/baosight/cli/main.py`

 * *Files identical despite different names*

### Comparing `baosight-0.0.2/baosight/tools/gitlab_runner.py` & `baosight-0.0.3/baosight/tools/gitlab_runner.py`

 * *Files identical despite different names*

### Comparing `baosight-0.0.2/baosight/tools/gitlab_runner_gui.py` & `baosight-0.0.3/baosight/tools/gitlab_runner_gui.py`

 * *Files identical despite different names*

### Comparing `baosight-0.0.2/setup.cfg` & `baosight-0.0.3/setup.cfg`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2062 616f 7369 6768 740d 0a76 6572   = baosight..ver
-00000020: 7369 6f6e 203d 2030 2e30 2e32 0d0a 6465  sion = 0.0.2..de
+00000020: 7369 6f6e 203d 2030 2e30 2e33 0d0a 6465  sion = 0.0.3..de
 00000030: 7363 7269 7074 696f 6e20 3d20 6261 6f73  scription = baos
 00000040: 6967 6874 2074 6f6f 6c73 0d0a 6c6f 6e67  ight tools..long
 00000050: 5f64 6573 6372 6970 7469 6f6e 203d 2066  _description = f
 00000060: 696c 653a 2052 4541 444d 452e 6d64 0d0a  ile: README.md..
 00000070: 6c6f 6e67 5f64 6573 6372 6970 7469 6f6e  long_description
 00000080: 5f63 6f6e 7465 6e74 5f74 7970 6520 3d20  _content_type = 
 00000090: 7465 7874 2f6d 6172 6b64 6f77 6e0d 0a61  text/markdown..a
```

