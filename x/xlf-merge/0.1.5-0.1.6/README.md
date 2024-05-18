# Comparing `tmp/xlf-merge-0.1.5.tar.gz` & `tmp/xlf-merge-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xlf-merge-0.1.5.tar", last modified: Mon Jun 19 02:58:36 2023, max compression
+gzip compressed data, was "xlf-merge-0.1.6.tar", last modified: Sat May 18 17:54:27 2024, max compression
```

## Comparing `xlf-merge-0.1.5.tar` & `xlf-merge-0.1.6.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 02:58:36.065025 xlf-merge-0.1.5/
--rw-rw-rw-   0 root         (0) root         (0)    35148 2023-06-19 02:56:25.000000 xlf-merge-0.1.5/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)       69 2023-06-19 02:56:25.000000 xlf-merge-0.1.5/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2137 2023-06-19 02:58:36.065025 xlf-merge-0.1.5/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1105 2023-06-19 02:56:25.000000 xlf-merge-0.1.5/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-19 02:58:36.065025 xlf-merge-0.1.5/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1659 2023-06-19 02:56:25.000000 xlf-merge-0.1.5/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 02:58:36.065025 xlf-merge-0.1.5/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-19 02:56:25.000000 xlf-merge-0.1.5/tests/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 02:58:36.065025 xlf-merge-0.1.5/xlf_merge/
--rw-rw-rw-   0 root         (0) root         (0)     5383 2023-06-19 02:56:25.000000 xlf-merge-0.1.5/xlf_merge/XlfParser.py
--rw-rw-rw-   0 root         (0) root         (0)       21 2023-06-19 02:56:25.000000 xlf-merge-0.1.5/xlf_merge/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      138 2023-06-19 02:56:25.000000 xlf-merge-0.1.5/xlf_merge/__main__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 02:58:36.065025 xlf-merge-0.1.5/xlf_merge/bin/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-19 02:56:25.000000 xlf-merge-0.1.5/xlf_merge/bin/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5067 2023-06-19 02:56:25.000000 xlf-merge-0.1.5/xlf_merge/bin/xlf_merge.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 02:58:36.065025 xlf-merge-0.1.5/xlf_merge.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2137 2023-06-19 02:58:36.000000 xlf-merge-0.1.5/xlf_merge.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      376 2023-06-19 02:58:36.000000 xlf-merge-0.1.5/xlf_merge.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-19 02:58:36.000000 xlf-merge-0.1.5/xlf_merge.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       54 2023-06-19 02:58:36.000000 xlf-merge-0.1.5/xlf_merge.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       12 2023-06-19 02:58:36.000000 xlf-merge-0.1.5/xlf_merge.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       10 2023-06-19 02:58:36.000000 xlf-merge-0.1.5/xlf_merge.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-18 17:54:27.932426 xlf-merge-0.1.6/
+-rw-rw-rw-   0 root         (0) root         (0)    35148 2024-05-18 17:52:38.000000 xlf-merge-0.1.6/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)       69 2024-05-18 17:52:38.000000 xlf-merge-0.1.6/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2137 2024-05-18 17:54:27.932426 xlf-merge-0.1.6/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1105 2024-05-18 17:52:38.000000 xlf-merge-0.1.6/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-18 17:54:27.932426 xlf-merge-0.1.6/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1659 2024-05-18 17:52:38.000000 xlf-merge-0.1.6/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-18 17:54:27.928426 xlf-merge-0.1.6/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-18 17:52:38.000000 xlf-merge-0.1.6/tests/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-18 17:54:27.928426 xlf-merge-0.1.6/xlf_merge/
+-rw-rw-rw-   0 root         (0) root         (0)     5383 2024-05-18 17:52:38.000000 xlf-merge-0.1.6/xlf_merge/XlfParser.py
+-rw-rw-rw-   0 root         (0) root         (0)       21 2024-05-18 17:52:38.000000 xlf-merge-0.1.6/xlf_merge/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      138 2024-05-18 17:52:38.000000 xlf-merge-0.1.6/xlf_merge/__main__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-18 17:54:27.932426 xlf-merge-0.1.6/xlf_merge/bin/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-18 17:52:38.000000 xlf-merge-0.1.6/xlf_merge/bin/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5067 2024-05-18 17:52:38.000000 xlf-merge-0.1.6/xlf_merge/bin/xlf_merge.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-18 17:54:27.932426 xlf-merge-0.1.6/xlf_merge.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2137 2024-05-18 17:54:27.000000 xlf-merge-0.1.6/xlf_merge.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      376 2024-05-18 17:54:27.000000 xlf-merge-0.1.6/xlf_merge.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-18 17:54:27.000000 xlf-merge-0.1.6/xlf_merge.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       54 2024-05-18 17:54:27.000000 xlf-merge-0.1.6/xlf_merge.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2024-05-18 17:54:27.000000 xlf-merge-0.1.6/xlf_merge.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2024-05-18 17:54:27.000000 xlf-merge-0.1.6/xlf_merge.egg-info/top_level.txt
```

### Comparing `xlf-merge-0.1.5/LICENSE` & `xlf-merge-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `xlf-merge-0.1.5/PKG-INFO` & `xlf-merge-0.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xlf-merge
-Version: 0.1.5
+Version: 0.1.6
 Summary: APP for merging xlf translation files
 Home-page: https://github.com/Salamek/xlf-merge
 Author: Adam Schubert
 Author-email: adam.schubert@sg1-game.net
 License: GPL-3.0 
 Project-URL: Release notes, https://github.com/Salamek/xlf-merge/releases
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `xlf-merge-0.1.5/README.md` & `xlf-merge-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `xlf-merge-0.1.5/setup.py` & `xlf-merge-0.1.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 
 setup(
     name='xlf-merge',
-    version='0.1.5',
+    version='0.1.6',
     packages=find_packages(exclude=['tests', 'tests.*']),
     package_data={'xlf_merge': ['py.typed']},
     install_requires=[
         'docopt',
         'lxml'
     ],
     url='https://github.com/Salamek/xlf-merge',
```

### Comparing `xlf-merge-0.1.5/xlf_merge/XlfParser.py` & `xlf-merge-0.1.6/xlf_merge/XlfParser.py`

 * *Files identical despite different names*

### Comparing `xlf-merge-0.1.5/xlf_merge/bin/xlf_merge.py` & `xlf-merge-0.1.6/xlf_merge/bin/xlf_merge.py`

 * *Files identical despite different names*

### Comparing `xlf-merge-0.1.5/xlf_merge.egg-info/PKG-INFO` & `xlf-merge-0.1.6/xlf_merge.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xlf-merge
-Version: 0.1.5
+Version: 0.1.6
 Summary: APP for merging xlf translation files
 Home-page: https://github.com/Salamek/xlf-merge
 Author: Adam Schubert
 Author-email: adam.schubert@sg1-game.net
 License: GPL-3.0 
 Project-URL: Release notes, https://github.com/Salamek/xlf-merge/releases
 Classifier: Development Status :: 5 - Production/Stable
```

