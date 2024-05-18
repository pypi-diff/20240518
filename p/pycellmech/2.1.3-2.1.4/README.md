# Comparing `tmp/pycellmech-2.1.3.tar.gz` & `tmp/pycellmech-2.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pycellmech-2.1.3.tar", last modified: Sat May 18 00:52:57 2024, max compression
+gzip compressed data, was "dist/pycellmech-2.1.4.tar", last modified: Sat May 18 01:01:49 2024, max compression
```

## Comparing `pycellmech-2.1.3.tar` & `pycellmech-2.1.4.tar`

### file list

```diff
@@ -1,12 +1,14 @@
-drwxr-xr-x   0 janan.arslan (31680)    10513        0 2024-05-18 00:52:57.547329 pycellmech-2.1.3/
--rw-rw-r--   0 janan.arslan (31680)    10513       34 2024-05-18 00:12:55.000000 pycellmech-2.1.3/MANIFEST.in
--rw-r--r--   0 janan.arslan (31680)    10513      508 2024-05-18 00:52:57.547605 pycellmech-2.1.3/PKG-INFO
-drwxr-xr-x   0 janan.arslan (31680)    10513        0 2024-05-18 00:52:57.546617 pycellmech-2.1.3/pycellmech.egg-info/
--rw-r--r--   0 janan.arslan (31680)    10513      508 2024-05-18 00:52:57.000000 pycellmech-2.1.3/pycellmech.egg-info/PKG-INFO
--rw-r--r--   0 janan.arslan (31680)    10513      236 2024-05-18 00:52:57.000000 pycellmech-2.1.3/pycellmech.egg-info/SOURCES.txt
--rw-r--r--   0 janan.arslan (31680)    10513        1 2024-05-18 00:52:57.000000 pycellmech-2.1.3/pycellmech.egg-info/dependency_links.txt
--rw-r--r--   0 janan.arslan (31680)    10513       52 2024-05-18 00:52:57.000000 pycellmech-2.1.3/pycellmech.egg-info/entry_points.txt
--rw-r--r--   0 janan.arslan (31680)    10513       51 2024-05-18 00:52:57.000000 pycellmech-2.1.3/pycellmech.egg-info/requires.txt
--rw-r--r--   0 janan.arslan (31680)    10513        1 2024-05-18 00:52:57.000000 pycellmech-2.1.3/pycellmech.egg-info/top_level.txt
--rw-rw-r--   0 janan.arslan (31680)    10513       79 2024-05-18 00:52:57.551549 pycellmech-2.1.3/setup.cfg
--rw-rw-r--   0 janan.arslan (31680)    10513     1131 2024-05-18 00:52:51.000000 pycellmech-2.1.3/setup.py
+drwxr-xr-x   0 janan.arslan (31680)    10513        0 2024-05-18 01:01:49.320421 pycellmech-2.1.4/
+-rw-rw-r--   0 janan.arslan (31680)    10513    14649 2024-05-18 00:12:55.000000 pycellmech-2.1.4/LICENSE.txt
+-rw-rw-r--   0 janan.arslan (31680)    10513       38 2024-05-18 00:59:30.000000 pycellmech-2.1.4/MANIFEST.in
+-rw-r--r--   0 janan.arslan (31680)    10513      508 2024-05-18 01:01:49.320759 pycellmech-2.1.4/PKG-INFO
+-rw-rw-r--   0 janan.arslan (31680)    10513     5873 2024-05-18 00:12:55.000000 pycellmech-2.1.4/README.md
+drwxr-xr-x   0 janan.arslan (31680)    10513        0 2024-05-18 01:01:49.319710 pycellmech-2.1.4/pycellmech.egg-info/
+-rw-r--r--   0 janan.arslan (31680)    10513      508 2024-05-18 01:01:49.000000 pycellmech-2.1.4/pycellmech.egg-info/PKG-INFO
+-rw-r--r--   0 janan.arslan (31680)    10513      258 2024-05-18 01:01:49.000000 pycellmech-2.1.4/pycellmech.egg-info/SOURCES.txt
+-rw-r--r--   0 janan.arslan (31680)    10513        1 2024-05-18 01:01:49.000000 pycellmech-2.1.4/pycellmech.egg-info/dependency_links.txt
+-rw-r--r--   0 janan.arslan (31680)    10513       52 2024-05-18 01:01:49.000000 pycellmech-2.1.4/pycellmech.egg-info/entry_points.txt
+-rw-r--r--   0 janan.arslan (31680)    10513       51 2024-05-18 01:01:49.000000 pycellmech-2.1.4/pycellmech.egg-info/requires.txt
+-rw-r--r--   0 janan.arslan (31680)    10513        1 2024-05-18 01:01:49.000000 pycellmech-2.1.4/pycellmech.egg-info/top_level.txt
+-rw-rw-r--   0 janan.arslan (31680)    10513       79 2024-05-18 01:01:49.323679 pycellmech-2.1.4/setup.cfg
+-rw-rw-r--   0 janan.arslan (31680)    10513     1130 2024-05-18 01:01:34.000000 pycellmech-2.1.4/setup.py
```

### Comparing `pycellmech-2.1.3/setup.py` & `pycellmech-2.1.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 import os
 from setuptools import setup, find_packages
 
 # Get the directory where setup.py is located
 current_directory = os.path.abspath(os.path.dirname(__file__))
 
 # Read the README.md file
-with open(os.path.join(current_directory, '../README.md'), encoding='utf-8') as f:
+with open(os.path.join(current_directory, './README.md'), encoding='utf-8') as f:
     long_description = f.read()    
 
 setup(
     name="pycellmech",
-    version="2.1.3",
+    version="2.1.4",
     author="Janan Arslan",
     author_email="janan.arslan@icm-institute.org",
     description="A shape-based feature extractor for medical and biological studies",
     long_description_content_type="text/markdown",
     url="https://github.com/icm-dac/pycellmech",
     packages=find_packages(),
     classifiers=[
```

