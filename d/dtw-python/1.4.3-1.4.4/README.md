# Comparing `tmp/dtw_python-1.4.3.tar.gz` & `tmp/dtw_python-1.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dtw_python-1.4.3.tar", last modified: Sat May 18 15:54:45 2024, max compression
+gzip compressed data, was "dtw_python-1.4.4.tar", last modified: Sat May 18 16:29:50 2024, max compression
```

## Comparing `dtw_python-1.4.3.tar` & `dtw_python-1.4.4.tar`

### file list

```diff
@@ -1,57 +1,57 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 15:54:45.645433 dtw_python-1.4.3/
--rw-r--r--   0 runner    (1001) docker     (127)      149 2024-05-18 15:54:39.000000 dtw_python-1.4.3/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (127)    26255 2024-05-18 15:54:39.000000 dtw_python-1.4.3/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)     3671 2024-05-18 15:54:39.000000 dtw_python-1.4.3/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-18 15:54:39.000000 dtw_python-1.4.3/COPYING
--rw-r--r--   0 runner    (1001) docker     (127)      386 2024-05-18 15:54:39.000000 dtw_python-1.4.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     7650 2024-05-18 15:54:45.645433 dtw_python-1.4.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6202 2024-05-18 15:54:39.000000 dtw_python-1.4.3/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 15:54:45.637433 dtw_python-1.4.3/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      604 2024-05-18 15:54:39.000000 dtw_python-1.4.3/docs/Makefile
--rwxr-xr-x   0 runner    (1001) docker     (127)     7350 2024-05-18 15:54:39.000000 dtw_python-1.4.3/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-18 15:54:39.000000 dtw_python-1.4.3/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      765 2024-05-18 15:54:39.000000 dtw_python-1.4.3/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 15:54:45.641433 dtw_python-1.4.3/dtw/
--rw-r--r--   0 runner    (1001) docker     (127)     1104 2024-05-18 15:54:39.000000 dtw_python-1.4.3/dtw/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1410 2024-05-18 15:54:39.000000 dtw_python-1.4.3/dtw/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2203 2024-05-18 15:54:39.000000 dtw_python-1.4.3/dtw/_backtrack.py
--rw-r--r--   0 runner    (1001) docker     (127)  1204329 2024-05-18 15:54:45.000000 dtw_python-1.4.3/dtw/_dtw_utils.c
--rw-r--r--   0 runner    (1001) docker     (127)     2999 2024-05-18 15:54:39.000000 dtw_python-1.4.3/dtw/_dtw_utils.pyx
--rw-r--r--   0 runner    (1001) docker     (127)     1920 2024-05-18 15:54:39.000000 dtw_python-1.4.3/dtw/_globalCostMatrix.py
--rw-r--r--   0 runner    (1001) docker     (127)     2771 2024-05-18 15:54:39.000000 dtw_python-1.4.3/dtw/countPaths.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 15:54:45.641433 dtw_python-1.4.3/dtw/data/
--rw-r--r--   0 runner    (1001) docker     (127)      501 2024-05-18 15:54:39.000000 dtw_python-1.4.3/dtw/data/README.txt
--rw-r--r--   0 runner    (1001) docker     (127)   250698 2024-05-18 15:54:39.000000 dtw_python-1.4.3/dtw/data/aami3a.csv
--rw-r--r--   0 runner    (1001) docker     (127)   252781 2024-05-18 15:54:39.000000 dtw_python-1.4.3/dtw/data/aami3b.csv
--rw-r--r--   0 runner    (1001) docker     (127)    15695 2024-05-18 15:54:39.000000 dtw_python-1.4.3/dtw/dtw.py
--rw-r--r--   0 runner    (1001) docker     (127)    12039 2024-05-18 15:54:39.000000 dtw_python-1.4.3/dtw/dtwPlot.py
--rw-r--r--   0 runner    (1001) docker     (127)     8418 2024-05-18 15:54:39.000000 dtw_python-1.4.3/dtw/dtw_core.c
--rw-r--r--   0 runner    (1001) docker     (127)     1271 2024-05-18 15:54:39.000000 dtw_python-1.4.3/dtw/dtw_core.h
--rw-r--r--   0 runner    (1001) docker     (127)     3575 2024-05-18 15:54:39.000000 dtw_python-1.4.3/dtw/dtw_test_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     3073 2024-05-18 15:54:39.000000 dtw_python-1.4.3/dtw/mvm.py
--rw-r--r--   0 runner    (1001) docker     (127)    26034 2024-05-18 15:54:39.000000 dtw_python-1.4.3/dtw/stepPattern.py
--rw-r--r--   0 runner    (1001) docker     (127)     3484 2024-05-18 15:54:39.000000 dtw_python-1.4.3/dtw/warp.py
--rw-r--r--   0 runner    (1001) docker     (127)     2731 2024-05-18 15:54:39.000000 dtw_python-1.4.3/dtw/warpArea.py
--rw-r--r--   0 runner    (1001) docker     (127)     5800 2024-05-18 15:54:39.000000 dtw_python-1.4.3/dtw/window.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 15:54:45.645433 dtw_python-1.4.3/dtw_python.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7650 2024-05-18 15:54:45.000000 dtw_python-1.4.3/dtw_python.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      937 2024-05-18 15:54:45.000000 dtw_python-1.4.3/dtw_python.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-18 15:54:45.000000 dtw_python-1.4.3/dtw_python.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-18 15:54:45.000000 dtw_python-1.4.3/dtw_python.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-18 15:54:45.000000 dtw_python-1.4.3/dtw_python.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-18 15:54:45.000000 dtw_python-1.4.3/dtw_python.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-18 15:54:45.000000 dtw_python-1.4.3/dtw_python.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      223 2024-05-18 15:54:39.000000 dtw_python-1.4.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      421 2024-05-18 15:54:45.645433 dtw_python-1.4.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2408 2024-05-18 15:54:39.000000 dtw_python-1.4.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 15:54:45.645433 dtw_python-1.4.3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-05-18 15:54:39.000000 dtw_python-1.4.3/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2547 2024-05-18 15:54:39.000000 dtw_python-1.4.3/tests/query.csv
--rw-r--r--   0 runner    (1001) docker     (127)     2550 2024-05-18 15:54:39.000000 dtw_python-1.4.3/tests/reference.csv
--rw-r--r--   0 runner    (1001) docker     (127)      515 2024-05-18 15:54:39.000000 dtw_python-1.4.3/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)      747 2024-05-18 15:54:39.000000 dtw_python-1.4.3/tests/test_countPaths.py
--rw-r--r--   0 runner    (1001) docker     (127)     2660 2024-05-18 15:54:39.000000 dtw_python-1.4.3/tests/test_cran.py
--rw-r--r--   0 runner    (1001) docker     (127)      453 2024-05-18 15:54:39.000000 dtw_python-1.4.3/tests/test_doctests.py
--rw-r--r--   0 runner    (1001) docker     (127)     1033 2024-05-18 15:54:39.000000 dtw_python-1.4.3/tests/test_dtw.py
--rw-r--r--   0 runner    (1001) docker     (127)     2683 2024-05-18 15:54:39.000000 dtw_python-1.4.3/tests/test_dtw_s.py
--rw-r--r--   0 runner    (1001) docker     (127)     1477 2024-05-18 15:54:39.000000 dtw_python-1.4.3/tests/test_issues.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 16:29:50.631978 dtw_python-1.4.4/
+-rw-r--r--   0 runner    (1001) docker     (127)      149 2024-05-18 16:29:40.000000 dtw_python-1.4.4/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    26255 2024-05-18 16:29:40.000000 dtw_python-1.4.4/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3671 2024-05-18 16:29:40.000000 dtw_python-1.4.4/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-18 16:29:40.000000 dtw_python-1.4.4/COPYING
+-rw-r--r--   0 runner    (1001) docker     (127)      386 2024-05-18 16:29:40.000000 dtw_python-1.4.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     7650 2024-05-18 16:29:50.631978 dtw_python-1.4.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6202 2024-05-18 16:29:40.000000 dtw_python-1.4.4/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 16:29:50.623978 dtw_python-1.4.4/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      604 2024-05-18 16:29:40.000000 dtw_python-1.4.4/docs/Makefile
+-rwxr-xr-x   0 runner    (1001) docker     (127)     7350 2024-05-18 16:29:40.000000 dtw_python-1.4.4/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-18 16:29:40.000000 dtw_python-1.4.4/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      765 2024-05-18 16:29:40.000000 dtw_python-1.4.4/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 16:29:50.627977 dtw_python-1.4.4/dtw/
+-rw-r--r--   0 runner    (1001) docker     (127)     1104 2024-05-18 16:29:40.000000 dtw_python-1.4.4/dtw/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1410 2024-05-18 16:29:40.000000 dtw_python-1.4.4/dtw/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2203 2024-05-18 16:29:40.000000 dtw_python-1.4.4/dtw/_backtrack.py
+-rw-r--r--   0 runner    (1001) docker     (127)  1204329 2024-05-18 16:29:49.000000 dtw_python-1.4.4/dtw/_dtw_utils.c
+-rw-r--r--   0 runner    (1001) docker     (127)     2999 2024-05-18 16:29:40.000000 dtw_python-1.4.4/dtw/_dtw_utils.pyx
+-rw-r--r--   0 runner    (1001) docker     (127)     1920 2024-05-18 16:29:40.000000 dtw_python-1.4.4/dtw/_globalCostMatrix.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2771 2024-05-18 16:29:40.000000 dtw_python-1.4.4/dtw/countPaths.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 16:29:50.627977 dtw_python-1.4.4/dtw/data/
+-rw-r--r--   0 runner    (1001) docker     (127)      501 2024-05-18 16:29:40.000000 dtw_python-1.4.4/dtw/data/README.txt
+-rw-r--r--   0 runner    (1001) docker     (127)   250698 2024-05-18 16:29:40.000000 dtw_python-1.4.4/dtw/data/aami3a.csv
+-rw-r--r--   0 runner    (1001) docker     (127)   252781 2024-05-18 16:29:40.000000 dtw_python-1.4.4/dtw/data/aami3b.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    15695 2024-05-18 16:29:40.000000 dtw_python-1.4.4/dtw/dtw.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12039 2024-05-18 16:29:40.000000 dtw_python-1.4.4/dtw/dtwPlot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8418 2024-05-18 16:29:40.000000 dtw_python-1.4.4/dtw/dtw_core.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1271 2024-05-18 16:29:40.000000 dtw_python-1.4.4/dtw/dtw_core.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3575 2024-05-18 16:29:40.000000 dtw_python-1.4.4/dtw/dtw_test_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3073 2024-05-18 16:29:40.000000 dtw_python-1.4.4/dtw/mvm.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26034 2024-05-18 16:29:40.000000 dtw_python-1.4.4/dtw/stepPattern.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3484 2024-05-18 16:29:40.000000 dtw_python-1.4.4/dtw/warp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2731 2024-05-18 16:29:40.000000 dtw_python-1.4.4/dtw/warpArea.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5800 2024-05-18 16:29:40.000000 dtw_python-1.4.4/dtw/window.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 16:29:50.631978 dtw_python-1.4.4/dtw_python.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7650 2024-05-18 16:29:50.000000 dtw_python-1.4.4/dtw_python.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      937 2024-05-18 16:29:50.000000 dtw_python-1.4.4/dtw_python.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-18 16:29:50.000000 dtw_python-1.4.4/dtw_python.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-18 16:29:50.000000 dtw_python-1.4.4/dtw_python.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-18 16:29:50.000000 dtw_python-1.4.4/dtw_python.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-18 16:29:50.000000 dtw_python-1.4.4/dtw_python.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-18 16:29:50.000000 dtw_python-1.4.4/dtw_python.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      223 2024-05-18 16:29:40.000000 dtw_python-1.4.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      421 2024-05-18 16:29:50.631978 dtw_python-1.4.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2408 2024-05-18 16:29:40.000000 dtw_python-1.4.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 16:29:50.631978 dtw_python-1.4.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-05-18 16:29:40.000000 dtw_python-1.4.4/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2547 2024-05-18 16:29:40.000000 dtw_python-1.4.4/tests/query.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     2550 2024-05-18 16:29:40.000000 dtw_python-1.4.4/tests/reference.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      515 2024-05-18 16:29:40.000000 dtw_python-1.4.4/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)      747 2024-05-18 16:29:40.000000 dtw_python-1.4.4/tests/test_countPaths.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2660 2024-05-18 16:29:40.000000 dtw_python-1.4.4/tests/test_cran.py
+-rw-r--r--   0 runner    (1001) docker     (127)      453 2024-05-18 16:29:40.000000 dtw_python-1.4.4/tests/test_doctests.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1033 2024-05-18 16:29:40.000000 dtw_python-1.4.4/tests/test_dtw.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2683 2024-05-18 16:29:40.000000 dtw_python-1.4.4/tests/test_dtw_s.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1477 2024-05-18 16:29:40.000000 dtw_python-1.4.4/tests/test_issues.py
```

### Comparing `dtw_python-1.4.3/CHANGELOG.md` & `dtw_python-1.4.4/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `dtw_python-1.4.3/CONTRIBUTING.rst` & `dtw_python-1.4.4/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `dtw_python-1.4.3/COPYING` & `dtw_python-1.4.4/COPYING`

 * *Files identical despite different names*

### Comparing `dtw_python-1.4.3/PKG-INFO` & `dtw_python-1.4.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dtw-python
-Version: 1.4.3
+Version: 1.4.4
 Summary: A comprehensive implementation of dynamic time warping (DTW) algorithms. DTW computes the optimal (least cumulative distance) alignment between points of two time series. Common DTW variants covered include local (slope) and global (window) constraints, subsequence matches, arbitrary distance definitions, normalizations, minimum variance matching, and so on. Provides cumulative distances, alignments, specialized plot styles, etc.
 Home-page: https://DynamicTimeWarping.github.io
 Author: Toni Giorgino
 Author-email: toni.giorgino@gmail.com
 License: GNU General Public License v3
 Keywords: dtw,timeseries
 Classifier: Development Status :: 4 - Beta
```

### Comparing `dtw_python-1.4.3/README.rst` & `dtw_python-1.4.4/README.rst`

 * *Files identical despite different names*

### Comparing `dtw_python-1.4.3/docs/Makefile` & `dtw_python-1.4.4/docs/Makefile`

 * *Files identical despite different names*

### Comparing `dtw_python-1.4.3/docs/conf.py` & `dtw_python-1.4.4/docs/conf.py`

 * *Files identical despite different names*

### Comparing `dtw_python-1.4.3/docs/make.bat` & `dtw_python-1.4.4/docs/make.bat`

 * *Files identical despite different names*

### Comparing `dtw_python-1.4.3/dtw/__init__.py` & `dtw_python-1.4.4/dtw/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 Please see the help for the dtw.dtw() function which is the package's
 main entry point.
 
 """
 
 __author__ = """Toni Giorgino"""
 __email__ = 'toni.giorgino@gmail.com'
-__version__ = '1.4.3'
+__version__ = '1.4.4'
 
 # There are no comments in this package because it mirrors closely the R sources.
 
 # List of things to export on "from dtw import *"
 from dtw.dtw import *
 from dtw.stepPattern import *
 from dtw.countPaths import *
```

### Comparing `dtw_python-1.4.3/dtw/__main__.py` & `dtw_python-1.4.4/dtw/__main__.py`

 * *Files identical despite different names*

### Comparing `dtw_python-1.4.3/dtw/_backtrack.py` & `dtw_python-1.4.4/dtw/_backtrack.py`

 * *Files identical despite different names*

### Comparing `dtw_python-1.4.3/dtw/_dtw_utils.c` & `dtw_python-1.4.4/dtw/_dtw_utils.c`

 * *Files 0% similar despite different names*

```diff
@@ -1697,195 +1697,195 @@
   Py_ssize_t strides[8];
   Py_ssize_t suboffsets[8];
 } __Pyx_memviewslice;
 #define __Pyx_MemoryView_Len(m)  (m.shape[0])
 
 /* #### Code section: numeric_typedefs ### */
 
-/* "../../../../../tmp/build-env-3qrhb4sw/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":732
+/* "../../../../../tmp/build-env-qv7imtqn/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":732
  * # in Cython to enable them only on the right systems.
  * 
  * ctypedef npy_int8       int8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  */
 typedef npy_int8 __pyx_t_5numpy_int8_t;
 
-/* "../../../../../tmp/build-env-3qrhb4sw/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":733
+/* "../../../../../tmp/build-env-qv7imtqn/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":733
  * 
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t
  */
 typedef npy_int16 __pyx_t_5numpy_int16_t;
 
-/* "../../../../../tmp/build-env-3qrhb4sw/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":734
+/* "../../../../../tmp/build-env-qv7imtqn/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":734
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int64      int64_t
  * #ctypedef npy_int96      int96_t
  */
 typedef npy_int32 __pyx_t_5numpy_int32_t;
 
-/* "../../../../../tmp/build-env-3qrhb4sw/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":735
+/* "../../../../../tmp/build-env-qv7imtqn/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":735
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_int96      int96_t
  * #ctypedef npy_int128     int128_t
  */
 typedef npy_int64 __pyx_t_5numpy_int64_t;
 
-/* "../../../../../tmp/build-env-3qrhb4sw/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":739
+/* "../../../../../tmp/build-env-qv7imtqn/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":739
  * #ctypedef npy_int128     int128_t
  * 
  * ctypedef npy_uint8      uint8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  */
 typedef npy_uint8 __pyx_t_5numpy_uint8_t;
 
-/* "../../../../../tmp/build-env-3qrhb4sw/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":740
+/* "../../../../../tmp/build-env-qv7imtqn/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":740
  * 
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t
  */
 typedef npy_uint16 __pyx_t_5numpy_uint16_t;
 
-/* "../../../../../tmp/build-env-3qrhb4sw/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":741
+/* "../../../../../tmp/build-env-qv7imtqn/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":741
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint64     uint64_t
  * #ctypedef npy_uint96     uint96_t
  */
 typedef npy_uint32 __pyx_t_5numpy_uint32_t;
 
-/* "../../../../../tmp/build-env-3qrhb4sw/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":742
+/* "../../../../../tmp/build-env-qv7imtqn/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":742
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_uint96     uint96_t
  * #ctypedef npy_uint128    uint128_t
  */
 typedef npy_uint64 __pyx_t_5numpy_uint64_t;
 
-/* "../../../../../tmp/build-env-3qrhb4sw/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":746
+/* "../../../../../tmp/build-env-qv7imtqn/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":746
  * #ctypedef npy_uint128    uint128_t
  * 
  * ctypedef npy_float32    float32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_float64    float64_t
  * #ctypedef npy_float80    float80_t
  */
 typedef npy_float32 __pyx_t_5numpy_float32_t;
 
-/* "../../../../../tmp/build-env-3qrhb4sw/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":747
+/* "../../../../../tmp/build-env-qv7imtqn/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":747
  * 
  * ctypedef npy_float32    float32_t
  * ctypedef npy_float64    float64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_float80    float80_t
  * #ctypedef npy_float128   float128_t
  */
 typedef npy_float64 __pyx_t_5numpy_float64_t;
 
-/* "../../../../../tmp/build-env-3qrhb4sw/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":756
+/* "../../../../../tmp/build-env-qv7imtqn/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":756
  * # The int types are mapped a bit surprising --
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longlong   long_t
  * ctypedef npy_longlong   longlong_t
  */
 typedef npy_long __pyx_t_5numpy_int_t;
 
-/* "../../../../../tmp/build-env-3qrhb4sw/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":757
+/* "../../../../../tmp/build-env-qv7imtqn/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":757
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t
  * ctypedef npy_longlong   long_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longlong   longlong_t
  * 
  */
 typedef npy_longlong __pyx_t_5numpy_long_t;
 
-/* "../../../../../tmp/build-env-3qrhb4sw/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":758
+/* "../../../../../tmp/build-env-qv7imtqn/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":758
  * ctypedef npy_long       int_t
  * ctypedef npy_longlong   long_t
  * ctypedef npy_longlong   longlong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_ulong      uint_t
  */
 typedef npy_longlong __pyx_t_5numpy_longlong_t;
 
-/* "../../../../../tmp/build-env-3qrhb4sw/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":760
+/* "../../../../../tmp/build-env-qv7imtqn/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":760
  * ctypedef npy_longlong   longlong_t
  * 
  * ctypedef npy_ulong      uint_t             # <<<<<<<<<<<<<<
  * ctypedef npy_ulonglong  ulong_t
  * ctypedef npy_ulonglong  ulonglong_t
  */
 typedef npy_ulong __pyx_t_5numpy_uint_t;
 
-/* "../../../../../tmp/build-env-3qrhb4sw/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":761
+/* "../../../../../tmp/build-env-qv7imtqn/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":761
  * 
  * ctypedef npy_ulong      uint_t
  * ctypedef npy_ulonglong  ulong_t             # <<<<<<<<<<<<<<
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  */
 typedef npy_ulonglong __pyx_t_5numpy_ulong_t;
 
-/* "../../../../../tmp/build-env-3qrhb4sw/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":762
+/* "../../../../../tmp/build-env-qv7imtqn/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":762
  * ctypedef npy_ulong      uint_t
  * ctypedef npy_ulonglong  ulong_t
  * ctypedef npy_ulonglong  ulonglong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_intp       intp_t
  */
 typedef npy_ulonglong __pyx_t_5numpy_ulonglong_t;
 
-/* "../../../../../tmp/build-env-3qrhb4sw/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":764
+/* "../../../../../tmp/build-env-qv7imtqn/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":764
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  * ctypedef npy_intp       intp_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uintp      uintp_t
  * 
  */
 typedef npy_intp __pyx_t_5numpy_intp_t;
 
-/* "../../../../../tmp/build-env-3qrhb4sw/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":765
+/* "../../../../../tmp/build-env-qv7imtqn/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":765
  * 
  * ctypedef npy_intp       intp_t
  * ctypedef npy_uintp      uintp_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_double     float_t
  */
 typedef npy_uintp __pyx_t_5numpy_uintp_t;
 
-/* "../../../../../tmp/build-env-3qrhb4sw/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":767
+/* "../../../../../tmp/build-env-qv7imtqn/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":767
  * ctypedef npy_uintp      uintp_t
  * 
  * ctypedef npy_double     float_t             # <<<<<<<<<<<<<<
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t
  */
 typedef npy_double __pyx_t_5numpy_float_t;
 
-/* "../../../../../tmp/build-env-3qrhb4sw/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":768
+/* "../../../../../tmp/build-env-qv7imtqn/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":768
  * 
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longdouble longdouble_t
  * 
  */
 typedef npy_double __pyx_t_5numpy_double_t;
 
-/* "../../../../../tmp/build-env-3qrhb4sw/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":769
+/* "../../../../../tmp/build-env-qv7imtqn/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":769
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cfloat      cfloat_t
  */
 typedef npy_longdouble __pyx_t_5numpy_longdouble_t;
@@ -1948,42 +1948,42 @@
  *     or the provided default value if no such value was found.
  */
 struct __pyx_opt_args_7cpython_11contextvars_get_value_no_default {
   int __pyx_n;
   PyObject *default_value;
 };
 
-/* "../../../../../tmp/build-env-3qrhb4sw/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":771
+/* "../../../../../tmp/build-env-qv7imtqn/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":771
  * ctypedef npy_longdouble longdouble_t
  * 
  * ctypedef npy_cfloat      cfloat_t             # <<<<<<<<<<<<<<
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t
  */
 typedef npy_cfloat __pyx_t_5numpy_cfloat_t;
 
-/* "../../../../../tmp/build-env-3qrhb4sw/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":772
+/* "../../../../../tmp/build-env-qv7imtqn/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":772
  * 
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t             # <<<<<<<<<<<<<<
  * ctypedef npy_clongdouble clongdouble_t
  * 
  */
 typedef npy_cdouble __pyx_t_5numpy_cdouble_t;
 
-/* "../../../../../tmp/build-env-3qrhb4sw/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":773
+/* "../../../../../tmp/build-env-qv7imtqn/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":773
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cdouble     complex_t
  */
 typedef npy_clongdouble __pyx_t_5numpy_clongdouble_t;
 
-/* "../../../../../tmp/build-env-3qrhb4sw/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":775
+/* "../../../../../tmp/build-env-qv7imtqn/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":775
  * ctypedef npy_clongdouble clongdouble_t
  * 
  * ctypedef npy_cdouble     complex_t             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  */
 typedef npy_cdouble __pyx_t_5numpy_complex_t;
@@ -18508,261 +18508,261 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-3qrhb4sw/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":246
+/* "../../../../../tmp/build-env-qv7imtqn/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":246
  * 
  *         @property
  *         cdef inline PyObject* base(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a borrowed reference to the object owning the data/memory.
  *             """
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_7ndarray_4base_base(PyArrayObject *__pyx_v_self) {
   PyObject *__pyx_r;
 
-  /* "../../../../../tmp/build-env-3qrhb4sw/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":249
+  /* "../../../../../tmp/build-env-qv7imtqn/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":249
  *             """Returns a borrowed reference to the object owning the data/memory.
  *             """
  *             return PyArray_BASE(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = PyArray_BASE(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-3qrhb4sw/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":246
+  /* "../../../../../tmp/build-env-qv7imtqn/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":246
  * 
  *         @property
  *         cdef inline PyObject* base(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a borrowed reference to the object owning the data/memory.
  *             """
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-3qrhb4sw/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":252
+/* "../../../../../tmp/build-env-qv7imtqn/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":252
  * 
  *         @property
  *         cdef inline dtype descr(self):             # <<<<<<<<<<<<<<
  *             """Returns an owned reference to the dtype of the array.
  *             """
  */
 
 static CYTHON_INLINE PyArray_Descr *__pyx_f_5numpy_7ndarray_5descr_descr(PyArrayObject *__pyx_v_self) {
   PyArray_Descr *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyArray_Descr *__pyx_t_1;
   __Pyx_RefNannySetupContext("descr", 1);
 
-  /* "../../../../../tmp/build-env-3qrhb4sw/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":255
+  /* "../../../../../tmp/build-env-qv7imtqn/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":255
  *             """Returns an owned reference to the dtype of the array.
  *             """
  *             return <dtype>PyArray_DESCR(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __Pyx_XDECREF((PyObject *)__pyx_r);
   __pyx_t_1 = PyArray_DESCR(__pyx_v_self);
   __Pyx_INCREF((PyObject *)((PyArray_Descr *)__pyx_t_1));
   __pyx_r = ((PyArray_Descr *)__pyx_t_1);
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-3qrhb4sw/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":252
+  /* "../../../../../tmp/build-env-qv7imtqn/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":252
  * 
  *         @property
  *         cdef inline dtype descr(self):             # <<<<<<<<<<<<<<
  *             """Returns an owned reference to the dtype of the array.
  *             """
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF((PyObject *)__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-3qrhb4sw/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":258
+/* "../../../../../tmp/build-env-qv7imtqn/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":258
  * 
  *         @property
  *         cdef inline int ndim(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns the number of dimensions in the array.
  *             """
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_7ndarray_4ndim_ndim(PyArrayObject *__pyx_v_self) {
   int __pyx_r;
 
-  /* "../../../../../tmp/build-env-3qrhb4sw/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":261
+  /* "../../../../../tmp/build-env-qv7imtqn/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":261
  *             """Returns the number of dimensions in the array.
  *             """
  *             return PyArray_NDIM(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = PyArray_NDIM(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-3qrhb4sw/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":258
+  /* "../../../../../tmp/build-env-qv7imtqn/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":258
  * 
  *         @property
  *         cdef inline int ndim(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns the number of dimensions in the array.
  *             """
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-3qrhb4sw/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":264
+/* "../../../../../tmp/build-env-qv7imtqn/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":264
  * 
  *         @property
  *         cdef inline npy_intp *shape(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a pointer to the dimensions/shape of the array.
  *             The number of elements matches the number of dimensions of the array (ndim).
  */
 
 static CYTHON_INLINE npy_intp *__pyx_f_5numpy_7ndarray_5shape_shape(PyArrayObject *__pyx_v_self) {
   npy_intp *__pyx_r;
 
-  /* "../../../../../tmp/build-env-3qrhb4sw/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":269
+  /* "../../../../../tmp/build-env-qv7imtqn/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":269
  *             Can return NULL for 0-dimensional arrays.
  *             """
  *             return PyArray_DIMS(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = PyArray_DIMS(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-3qrhb4sw/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":264
+  /* "../../../../../tmp/build-env-qv7imtqn/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":264
  * 
  *         @property
  *         cdef inline npy_intp *shape(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a pointer to the dimensions/shape of the array.
  *             The number of elements matches the number of dimensions of the array (ndim).
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-3qrhb4sw/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":272
+/* "../../../../../tmp/build-env-qv7imtqn/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":272
  * 
  *         @property
  *         cdef inline npy_intp *strides(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a pointer to the strides of the array.
  *             The number of elements matches the number of dimensions of the array (ndim).
  */
 
 static CYTHON_INLINE npy_intp *__pyx_f_5numpy_7ndarray_7strides_strides(PyArrayObject *__pyx_v_self) {
   npy_intp *__pyx_r;
 
-  /* "../../../../../tmp/build-env-3qrhb4sw/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":276
+  /* "../../../../../tmp/build-env-qv7imtqn/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":276
  *             The number of elements matches the number of dimensions of the array (ndim).
  *             """
  *             return PyArray_STRIDES(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = PyArray_STRIDES(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-3qrhb4sw/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":272
+  /* "../../../../../tmp/build-env-qv7imtqn/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":272
  * 
  *         @property
  *         cdef inline npy_intp *strides(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a pointer to the strides of the array.
  *             The number of elements matches the number of dimensions of the array (ndim).
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-3qrhb4sw/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":279
+/* "../../../../../tmp/build-env-qv7imtqn/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":279
  * 
  *         @property
  *         cdef inline npy_intp size(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns the total size (in number of elements) of the array.
  *             """
  */
 
 static CYTHON_INLINE npy_intp __pyx_f_5numpy_7ndarray_4size_size(PyArrayObject *__pyx_v_self) {
   npy_intp __pyx_r;
 
-  /* "../../../../../tmp/build-env-3qrhb4sw/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":282
+  /* "../../../../../tmp/build-env-qv7imtqn/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":282
  *             """Returns the total size (in number of elements) of the array.
  *             """
  *             return PyArray_SIZE(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = PyArray_SIZE(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-3qrhb4sw/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":279
+  /* "../../../../../tmp/build-env-qv7imtqn/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":279
  * 
  *         @property
  *         cdef inline npy_intp size(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns the total size (in number of elements) of the array.
  *             """
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-3qrhb4sw/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":285
+/* "../../../../../tmp/build-env-qv7imtqn/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":285
  * 
  *         @property
  *         cdef inline char* data(self) nogil:             # <<<<<<<<<<<<<<
  *             """The pointer to the data buffer as a char*.
  *             This is provided for legacy reasons to avoid direct struct field access.
  */
 
 static CYTHON_INLINE char *__pyx_f_5numpy_7ndarray_4data_data(PyArrayObject *__pyx_v_self) {
   char *__pyx_r;
 
-  /* "../../../../../tmp/build-env-3qrhb4sw/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":291
+  /* "../../../../../tmp/build-env-qv7imtqn/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":291
  *             of `PyArray_DATA()` instead, which returns a 'void*'.
  *             """
  *             return PyArray_BYTES(self)             # <<<<<<<<<<<<<<
  * 
  *     ctypedef unsigned char      npy_bool
  */
   __pyx_r = PyArray_BYTES(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-3qrhb4sw/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":285
+  /* "../../../../../tmp/build-env-qv7imtqn/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":285
  * 
  *         @property
  *         cdef inline char* data(self) nogil:             # <<<<<<<<<<<<<<
  *             """The pointer to the data buffer as a char*.
  *             This is provided for legacy reasons to avoid direct struct field access.
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-3qrhb4sw/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":777
+/* "../../../../../tmp/build-env-qv7imtqn/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":777
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -18771,29 +18771,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew1", 1);
 
-  /* "../../../../../tmp/build-env-3qrhb4sw/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":778
+  /* "../../../../../tmp/build-env-qv7imtqn/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":778
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  *     return PyArray_MultiIterNew(1, <void*>a)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(1, ((void *)__pyx_v_a)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 778, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-3qrhb4sw/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":777
+  /* "../../../../../tmp/build-env-qv7imtqn/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":777
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -18804,15 +18804,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-3qrhb4sw/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":780
+/* "../../../../../tmp/build-env-qv7imtqn/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":780
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -18821,29 +18821,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew2", 1);
 
-  /* "../../../../../tmp/build-env-3qrhb4sw/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":781
+  /* "../../../../../tmp/build-env-qv7imtqn/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":781
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(2, ((void *)__pyx_v_a), ((void *)__pyx_v_b)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 781, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-3qrhb4sw/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":780
+  /* "../../../../../tmp/build-env-qv7imtqn/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":780
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -18854,15 +18854,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-3qrhb4sw/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":783
+/* "../../../../../tmp/build-env-qv7imtqn/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":783
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -18871,29 +18871,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew3", 1);
 
-  /* "../../../../../tmp/build-env-3qrhb4sw/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":784
+  /* "../../../../../tmp/build-env-qv7imtqn/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":784
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(3, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 784, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-3qrhb4sw/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":783
+  /* "../../../../../tmp/build-env-qv7imtqn/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":783
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -18904,15 +18904,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-3qrhb4sw/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":786
+/* "../../../../../tmp/build-env-qv7imtqn/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":786
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -18921,29 +18921,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew4", 1);
 
-  /* "../../../../../tmp/build-env-3qrhb4sw/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":787
+  /* "../../../../../tmp/build-env-qv7imtqn/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":787
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(4, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 787, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-3qrhb4sw/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":786
+  /* "../../../../../tmp/build-env-qv7imtqn/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":786
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -18954,15 +18954,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-3qrhb4sw/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":789
+/* "../../../../../tmp/build-env-qv7imtqn/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":789
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -18971,29 +18971,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew5", 1);
 
-  /* "../../../../../tmp/build-env-3qrhb4sw/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":790
+  /* "../../../../../tmp/build-env-qv7imtqn/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":790
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)             # <<<<<<<<<<<<<<
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(5, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d), ((void *)__pyx_v_e)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 790, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-3qrhb4sw/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":789
+  /* "../../../../../tmp/build-env-qv7imtqn/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":789
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -19004,209 +19004,209 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-3qrhb4sw/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":792
+/* "../../../../../tmp/build-env-qv7imtqn/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":792
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_PyDataType_SHAPE(PyArray_Descr *__pyx_v_d) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("PyDataType_SHAPE", 1);
 
-  /* "../../../../../tmp/build-env-3qrhb4sw/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":793
+  /* "../../../../../tmp/build-env-qv7imtqn/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":793
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   __pyx_t_1 = PyDataType_HASSUBARRAY(__pyx_v_d);
   if (__pyx_t_1) {
 
-    /* "../../../../../tmp/build-env-3qrhb4sw/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":794
+    /* "../../../../../tmp/build-env-qv7imtqn/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":794
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape             # <<<<<<<<<<<<<<
  *     else:
  *         return ()
  */
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(((PyObject*)__pyx_v_d->subarray->shape));
     __pyx_r = ((PyObject*)__pyx_v_d->subarray->shape);
     goto __pyx_L0;
 
-    /* "../../../../../tmp/build-env-3qrhb4sw/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":793
+    /* "../../../../../tmp/build-env-qv7imtqn/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":793
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   }
 
-  /* "../../../../../tmp/build-env-3qrhb4sw/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":796
+  /* "../../../../../tmp/build-env-qv7imtqn/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":796
  *         return <tuple>d.subarray.shape
  *     else:
  *         return ()             # <<<<<<<<<<<<<<
  * 
  * 
  */
   /*else*/ {
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(__pyx_empty_tuple);
     __pyx_r = __pyx_empty_tuple;
     goto __pyx_L0;
   }
 
-  /* "../../../../../tmp/build-env-3qrhb4sw/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":792
+  /* "../../../../../tmp/build-env-qv7imtqn/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":792
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-3qrhb4sw/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":971
+/* "../../../../../tmp/build-env-qv7imtqn/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":971
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
 static CYTHON_INLINE void __pyx_f_5numpy_set_array_base(PyArrayObject *__pyx_v_arr, PyObject *__pyx_v_base) {
 
-  /* "../../../../../tmp/build-env-3qrhb4sw/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":972
+  /* "../../../../../tmp/build-env-qv7imtqn/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":972
  * 
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!             # <<<<<<<<<<<<<<
  *     PyArray_SetBaseObject(arr, base)
  * 
  */
   Py_INCREF(__pyx_v_base);
 
-  /* "../../../../../tmp/build-env-3qrhb4sw/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":973
+  /* "../../../../../tmp/build-env-qv7imtqn/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":973
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object get_array_base(ndarray arr):
  */
   (void)(PyArray_SetBaseObject(__pyx_v_arr, __pyx_v_base));
 
-  /* "../../../../../tmp/build-env-3qrhb4sw/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":971
+  /* "../../../../../tmp/build-env-qv7imtqn/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":971
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
   /* function exit code */
 }
 
-/* "../../../../../tmp/build-env-3qrhb4sw/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":975
+/* "../../../../../tmp/build-env-qv7imtqn/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":975
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_get_array_base(PyArrayObject *__pyx_v_arr) {
   PyObject *__pyx_v_base;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("get_array_base", 1);
 
-  /* "../../../../../tmp/build-env-3qrhb4sw/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":976
+  /* "../../../../../tmp/build-env-qv7imtqn/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":976
  * 
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)             # <<<<<<<<<<<<<<
  *     if base is NULL:
  *         return None
  */
   __pyx_v_base = PyArray_BASE(__pyx_v_arr);
 
-  /* "../../../../../tmp/build-env-3qrhb4sw/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":977
+  /* "../../../../../tmp/build-env-qv7imtqn/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":977
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   __pyx_t_1 = (__pyx_v_base == NULL);
   if (__pyx_t_1) {
 
-    /* "../../../../../tmp/build-env-3qrhb4sw/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":978
+    /* "../../../../../tmp/build-env-qv7imtqn/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":978
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  *         return None             # <<<<<<<<<<<<<<
  *     return <object>base
  * 
  */
     __Pyx_XDECREF(__pyx_r);
     __pyx_r = Py_None; __Pyx_INCREF(Py_None);
     goto __pyx_L0;
 
-    /* "../../../../../tmp/build-env-3qrhb4sw/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":977
+    /* "../../../../../tmp/build-env-qv7imtqn/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":977
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   }
 
-  /* "../../../../../tmp/build-env-3qrhb4sw/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":979
+  /* "../../../../../tmp/build-env-qv7imtqn/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":979
  *     if base is NULL:
  *         return None
  *     return <object>base             # <<<<<<<<<<<<<<
  * 
  * # Versions of the import_* functions which are more suitable for
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(((PyObject *)__pyx_v_base));
   __pyx_r = ((PyObject *)__pyx_v_base);
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-3qrhb4sw/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":975
+  /* "../../../../../tmp/build-env-qv7imtqn/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":975
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-3qrhb4sw/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":983
+/* "../../../../../tmp/build-env-qv7imtqn/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":983
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -19222,15 +19222,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_array", 1);
 
-  /* "../../../../../tmp/build-env-3qrhb4sw/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":984
+  /* "../../../../../tmp/build-env-qv7imtqn/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":984
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
   {
@@ -19238,68 +19238,68 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../../tmp/build-env-3qrhb4sw/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":985
+      /* "../../../../../tmp/build-env-qv7imtqn/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":985
  * cdef inline int import_array() except -1:
  *     try:
  *         __pyx_import_array()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")
  */
       __pyx_t_4 = _import_array(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(2, 985, __pyx_L3_error)
 
-      /* "../../../../../tmp/build-env-3qrhb4sw/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":984
+      /* "../../../../../tmp/build-env-qv7imtqn/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":984
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../../tmp/build-env-3qrhb4sw/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":986
+    /* "../../../../../tmp/build-env-qv7imtqn/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":986
  *     try:
  *         __pyx_import_array()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(2, 986, __pyx_L5_except_error)
       __Pyx_XGOTREF(__pyx_t_5);
       __Pyx_XGOTREF(__pyx_t_6);
       __Pyx_XGOTREF(__pyx_t_7);
 
-      /* "../../../../../tmp/build-env-3qrhb4sw/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":987
+      /* "../../../../../tmp/build-env-qv7imtqn/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":987
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__9, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 987, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(2, 987, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
 
-    /* "../../../../../tmp/build-env-3qrhb4sw/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":984
+    /* "../../../../../tmp/build-env-qv7imtqn/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":984
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     __pyx_L5_except_error:;
@@ -19307,15 +19307,15 @@
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../../tmp/build-env-3qrhb4sw/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":983
+  /* "../../../../../tmp/build-env-qv7imtqn/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":983
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -19330,15 +19330,15 @@
   __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-3qrhb4sw/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":989
+/* "../../../../../tmp/build-env-qv7imtqn/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":989
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -19354,15 +19354,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_umath", 1);
 
-  /* "../../../../../tmp/build-env-3qrhb4sw/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":990
+  /* "../../../../../tmp/build-env-qv7imtqn/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":990
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -19370,68 +19370,68 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../../tmp/build-env-3qrhb4sw/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":991
+      /* "../../../../../tmp/build-env-qv7imtqn/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":991
  * cdef inline int import_umath() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
       __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(2, 991, __pyx_L3_error)
 
-      /* "../../../../../tmp/build-env-3qrhb4sw/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":990
+      /* "../../../../../tmp/build-env-qv7imtqn/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":990
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../../tmp/build-env-3qrhb4sw/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":992
+    /* "../../../../../tmp/build-env-qv7imtqn/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":992
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(2, 992, __pyx_L5_except_error)
       __Pyx_XGOTREF(__pyx_t_5);
       __Pyx_XGOTREF(__pyx_t_6);
       __Pyx_XGOTREF(__pyx_t_7);
 
-      /* "../../../../../tmp/build-env-3qrhb4sw/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":993
+      /* "../../../../../tmp/build-env-qv7imtqn/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":993
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__10, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 993, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(2, 993, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
 
-    /* "../../../../../tmp/build-env-3qrhb4sw/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":990
+    /* "../../../../../tmp/build-env-qv7imtqn/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":990
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __pyx_L5_except_error:;
@@ -19439,15 +19439,15 @@
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../../tmp/build-env-3qrhb4sw/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":989
+  /* "../../../../../tmp/build-env-qv7imtqn/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":989
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -19462,15 +19462,15 @@
   __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-3qrhb4sw/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":995
+/* "../../../../../tmp/build-env-qv7imtqn/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":995
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -19486,15 +19486,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_ufunc", 1);
 
-  /* "../../../../../tmp/build-env-3qrhb4sw/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":996
+  /* "../../../../../tmp/build-env-qv7imtqn/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":996
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -19502,68 +19502,68 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../../tmp/build-env-3qrhb4sw/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":997
+      /* "../../../../../tmp/build-env-qv7imtqn/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":997
  * cdef inline int import_ufunc() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
       __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(2, 997, __pyx_L3_error)
 
-      /* "../../../../../tmp/build-env-3qrhb4sw/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":996
+      /* "../../../../../tmp/build-env-qv7imtqn/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":996
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../../tmp/build-env-3qrhb4sw/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":998
+    /* "../../../../../tmp/build-env-qv7imtqn/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":998
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(2, 998, __pyx_L5_except_error)
       __Pyx_XGOTREF(__pyx_t_5);
       __Pyx_XGOTREF(__pyx_t_6);
       __Pyx_XGOTREF(__pyx_t_7);
 
-      /* "../../../../../tmp/build-env-3qrhb4sw/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":999
+      /* "../../../../../tmp/build-env-qv7imtqn/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":999
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * 
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__10, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 999, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(2, 999, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
 
-    /* "../../../../../tmp/build-env-3qrhb4sw/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":996
+    /* "../../../../../tmp/build-env-qv7imtqn/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":996
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __pyx_L5_except_error:;
@@ -19571,15 +19571,15 @@
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../../tmp/build-env-3qrhb4sw/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":995
+  /* "../../../../../tmp/build-env-qv7imtqn/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":995
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -19594,170 +19594,170 @@
   __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-3qrhb4sw/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1002
+/* "../../../../../tmp/build-env-qv7imtqn/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1002
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_is_timedelta64_object(PyObject *__pyx_v_obj) {
   int __pyx_r;
 
-  /* "../../../../../tmp/build-env-3qrhb4sw/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1014
+  /* "../../../../../tmp/build-env-qv7imtqn/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1014
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyTimedeltaArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyTimedeltaArrType_Type));
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-3qrhb4sw/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1002
+  /* "../../../../../tmp/build-env-qv7imtqn/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1002
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-3qrhb4sw/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1017
+/* "../../../../../tmp/build-env-qv7imtqn/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1017
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_is_datetime64_object(PyObject *__pyx_v_obj) {
   int __pyx_r;
 
-  /* "../../../../../tmp/build-env-3qrhb4sw/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1029
+  /* "../../../../../tmp/build-env-qv7imtqn/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1029
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyDatetimeArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyDatetimeArrType_Type));
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-3qrhb4sw/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1017
+  /* "../../../../../tmp/build-env-qv7imtqn/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1017
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-3qrhb4sw/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1032
+/* "../../../../../tmp/build-env-qv7imtqn/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1032
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
 static CYTHON_INLINE npy_datetime __pyx_f_5numpy_get_datetime64_value(PyObject *__pyx_v_obj) {
   npy_datetime __pyx_r;
 
-  /* "../../../../../tmp/build-env-3qrhb4sw/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1039
+  /* "../../../../../tmp/build-env-qv7imtqn/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1039
  *     also needed.  That can be found using `get_datetime64_unit`.
  *     """
  *     return (<PyDatetimeScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((PyDatetimeScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-3qrhb4sw/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1032
+  /* "../../../../../tmp/build-env-qv7imtqn/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1032
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-3qrhb4sw/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1042
+/* "../../../../../tmp/build-env-qv7imtqn/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1042
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
 static CYTHON_INLINE npy_timedelta __pyx_f_5numpy_get_timedelta64_value(PyObject *__pyx_v_obj) {
   npy_timedelta __pyx_r;
 
-  /* "../../../../../tmp/build-env-3qrhb4sw/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1046
+  /* "../../../../../tmp/build-env-qv7imtqn/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1046
  *     returns the int64 value underlying scalar numpy timedelta64 object
  *     """
  *     return (<PyTimedeltaScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((PyTimedeltaScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-3qrhb4sw/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1042
+  /* "../../../../../tmp/build-env-qv7imtqn/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1042
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-3qrhb4sw/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1049
+/* "../../../../../tmp/build-env-qv7imtqn/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1049
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
 static CYTHON_INLINE NPY_DATETIMEUNIT __pyx_f_5numpy_get_datetime64_unit(PyObject *__pyx_v_obj) {
   NPY_DATETIMEUNIT __pyx_r;
 
-  /* "../../../../../tmp/build-env-3qrhb4sw/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1053
+  /* "../../../../../tmp/build-env-qv7imtqn/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1053
  *     returns the unit part of the dtype for a numpy datetime64 object.
  *     """
  *     return <NPY_DATETIMEUNIT>(<PyDatetimeScalarObject*>obj).obmeta.base             # <<<<<<<<<<<<<<
  */
   __pyx_r = ((NPY_DATETIMEUNIT)((PyDatetimeScalarObject *)__pyx_v_obj)->obmeta.base);
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-3qrhb4sw/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1049
+  /* "../../../../../tmp/build-env-qv7imtqn/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1049
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
@@ -23141,26 +23141,26 @@
  *         from pickle import PickleError as __pyx_PickleError
  *         raise __pyx_PickleError, "Incompatible checksums (0x%x vs (0x82a3537, 0x6ae9995, 0xb068931) = (name))" % __pyx_checksum
  */
   __pyx_tuple__8 = PyTuple_Pack(3, __pyx_int_136983863, __pyx_int_112105877, __pyx_int_184977713); if (unlikely(!__pyx_tuple__8)) __PYX_ERR(1, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__8);
   __Pyx_GIVEREF(__pyx_tuple__8);
 
-  /* "../../../../../tmp/build-env-3qrhb4sw/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":987
+  /* "../../../../../tmp/build-env-qv7imtqn/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":987
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
   __pyx_tuple__9 = PyTuple_Pack(1, __pyx_kp_u_numpy_core_multiarray_failed_to); if (unlikely(!__pyx_tuple__9)) __PYX_ERR(2, 987, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__9);
   __Pyx_GIVEREF(__pyx_tuple__9);
 
-  /* "../../../../../tmp/build-env-3qrhb4sw/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":993
+  /* "../../../../../tmp/build-env-qv7imtqn/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":993
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
   __pyx_tuple__10 = PyTuple_Pack(1, __pyx_kp_u_numpy_core_umath_failed_to_impor); if (unlikely(!__pyx_tuple__10)) __PYX_ERR(2, 993, __pyx_L1_error)
```

### Comparing `dtw_python-1.4.3/dtw/_dtw_utils.pyx` & `dtw_python-1.4.4/dtw/_dtw_utils.pyx`

 * *Files identical despite different names*

### Comparing `dtw_python-1.4.3/dtw/_globalCostMatrix.py` & `dtw_python-1.4.4/dtw/_globalCostMatrix.py`

 * *Files identical despite different names*

### Comparing `dtw_python-1.4.3/dtw/countPaths.py` & `dtw_python-1.4.4/dtw/countPaths.py`

 * *Files identical despite different names*

### Comparing `dtw_python-1.4.3/dtw/data/aami3a.csv` & `dtw_python-1.4.4/dtw/data/aami3a.csv`

 * *Files identical despite different names*

### Comparing `dtw_python-1.4.3/dtw/data/aami3b.csv` & `dtw_python-1.4.4/dtw/data/aami3b.csv`

 * *Files identical despite different names*

### Comparing `dtw_python-1.4.3/dtw/dtw.py` & `dtw_python-1.4.4/dtw/dtw.py`

 * *Files identical despite different names*

### Comparing `dtw_python-1.4.3/dtw/dtwPlot.py` & `dtw_python-1.4.4/dtw/dtwPlot.py`

 * *Files identical despite different names*

### Comparing `dtw_python-1.4.3/dtw/dtw_core.c` & `dtw_python-1.4.4/dtw/dtw_core.c`

 * *Files identical despite different names*

### Comparing `dtw_python-1.4.3/dtw/dtw_core.h` & `dtw_python-1.4.4/dtw/dtw_core.h`

 * *Files identical despite different names*

### Comparing `dtw_python-1.4.3/dtw/dtw_test_data.py` & `dtw_python-1.4.4/dtw/dtw_test_data.py`

 * *Files identical despite different names*

### Comparing `dtw_python-1.4.3/dtw/mvm.py` & `dtw_python-1.4.4/dtw/mvm.py`

 * *Files identical despite different names*

### Comparing `dtw_python-1.4.3/dtw/stepPattern.py` & `dtw_python-1.4.4/dtw/stepPattern.py`

 * *Files identical despite different names*

### Comparing `dtw_python-1.4.3/dtw/warp.py` & `dtw_python-1.4.4/dtw/warp.py`

 * *Files identical despite different names*

### Comparing `dtw_python-1.4.3/dtw/warpArea.py` & `dtw_python-1.4.4/dtw/warpArea.py`

 * *Files identical despite different names*

### Comparing `dtw_python-1.4.3/dtw/window.py` & `dtw_python-1.4.4/dtw/window.py`

 * *Files identical despite different names*

### Comparing `dtw_python-1.4.3/dtw_python.egg-info/PKG-INFO` & `dtw_python-1.4.4/dtw_python.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dtw-python
-Version: 1.4.3
+Version: 1.4.4
 Summary: A comprehensive implementation of dynamic time warping (DTW) algorithms. DTW computes the optimal (least cumulative distance) alignment between points of two time series. Common DTW variants covered include local (slope) and global (window) constraints, subsequence matches, arbitrary distance definitions, normalizations, minimum variance matching, and so on. Provides cumulative distances, alignments, specialized plot styles, etc.
 Home-page: https://DynamicTimeWarping.github.io
 Author: Toni Giorgino
 Author-email: toni.giorgino@gmail.com
 License: GNU General Public License v3
 Keywords: dtw,timeseries
 Classifier: Development Status :: 4 - Beta
```

### Comparing `dtw_python-1.4.3/dtw_python.egg-info/SOURCES.txt` & `dtw_python-1.4.4/dtw_python.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dtw_python-1.4.3/setup.py` & `dtw_python-1.4.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -51,10 +51,10 @@
     #    packages=find_packages(include=['dtw']),
     packages=['dtw'],
     package_data={'dtw': ['data/*.csv']},
     include_dirs=numpy.get_include(),
     ext_modules=cythonize([Extension('dtw._dtw_utils',
                  sources=['dtw/_dtw_utils.pyx', 'dtw/dtw_core.c'])]),
     url='https://DynamicTimeWarping.github.io',
-    version='1.4.3',
+    version='1.4.4',
     zip_safe=False,
 )
```

### Comparing `dtw_python-1.4.3/tests/query.csv` & `dtw_python-1.4.4/tests/query.csv`

 * *Files identical despite different names*

### Comparing `dtw_python-1.4.3/tests/reference.csv` & `dtw_python-1.4.4/tests/reference.csv`

 * *Files identical despite different names*

### Comparing `dtw_python-1.4.3/tests/test_cli.py` & `dtw_python-1.4.4/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `dtw_python-1.4.3/tests/test_countPaths.py` & `dtw_python-1.4.4/tests/test_countPaths.py`

 * *Files identical despite different names*

### Comparing `dtw_python-1.4.3/tests/test_cran.py` & `dtw_python-1.4.4/tests/test_cran.py`

 * *Files identical despite different names*

### Comparing `dtw_python-1.4.3/tests/test_dtw.py` & `dtw_python-1.4.4/tests/test_dtw.py`

 * *Files identical despite different names*

### Comparing `dtw_python-1.4.3/tests/test_dtw_s.py` & `dtw_python-1.4.4/tests/test_dtw_s.py`

 * *Files identical despite different names*

### Comparing `dtw_python-1.4.3/tests/test_issues.py` & `dtw_python-1.4.4/tests/test_issues.py`

 * *Files identical despite different names*

