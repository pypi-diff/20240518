# Comparing `tmp/vuc3-0.0.2.tar.gz` & `tmp/vuc3-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vuc3-0.0.2.tar", last modified: Mon Apr 22 08:11:46 2024, max compression
+gzip compressed data, was "vuc3-0.0.3.tar", last modified: Fri May 17 22:35:13 2024, max compression
```

## Comparing `vuc3-0.0.2.tar` & `vuc3-0.0.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 takefuji  (1000) takefuji  (1000)        0 2024-04-22 08:11:46.009386 vuc3-0.0.2/
--rw-r--r--   0 takefuji  (1000) takefuji  (1000)     1459 2024-04-22 08:11:46.009386 vuc3-0.0.2/PKG-INFO
--rw-r--r--   0 takefuji  (1000) takefuji  (1000)      931 2024-04-22 08:11:16.000000 vuc3-0.0.2/README.md
--rw-r--r--   0 takefuji  (1000) takefuji  (1000)       38 2024-04-22 08:11:46.009386 vuc3-0.0.2/setup.cfg
--rw-r--r--   0 takefuji  (1000) takefuji  (1000)      936 2024-04-22 08:10:38.000000 vuc3-0.0.2/setup.py
-drwxr-xr-x   0 takefuji  (1000) takefuji  (1000)        0 2024-04-22 08:11:46.009386 vuc3-0.0.2/src/
-drwxr-xr-x   0 takefuji  (1000) takefuji  (1000)        0 2024-04-22 08:11:46.009386 vuc3-0.0.2/src/vuc3.egg-info/
--rw-r--r--   0 takefuji  (1000) takefuji  (1000)     1459 2024-04-22 08:11:45.000000 vuc3-0.0.2/src/vuc3.egg-info/PKG-INFO
--rw-r--r--   0 takefuji  (1000) takefuji  (1000)      193 2024-04-22 08:11:45.000000 vuc3-0.0.2/src/vuc3.egg-info/SOURCES.txt
--rw-r--r--   0 takefuji  (1000) takefuji  (1000)        1 2024-04-22 08:11:45.000000 vuc3-0.0.2/src/vuc3.egg-info/dependency_links.txt
--rw-r--r--   0 takefuji  (1000) takefuji  (1000)       36 2024-04-22 08:11:45.000000 vuc3-0.0.2/src/vuc3.egg-info/entry_points.txt
--rw-r--r--   0 takefuji  (1000) takefuji  (1000)        5 2024-04-22 08:11:45.000000 vuc3-0.0.2/src/vuc3.egg-info/top_level.txt
--rwxr-xr-x   0 takefuji  (1000) takefuji  (1000)     2198 2023-03-04 01:53:17.000000 vuc3-0.0.2/src/vuc3.py
+drwxr-xr-x   0 takefuji  (1000) takefuji  (1000)        0 2024-05-17 22:35:13.374696 vuc3-0.0.3/
+-rw-r--r--   0 takefuji  (1000) takefuji  (1000)     1456 2024-05-17 22:35:13.374696 vuc3-0.0.3/PKG-INFO
+-rw-r--r--   0 takefuji  (1000) takefuji  (1000)      931 2024-05-17 22:34:37.000000 vuc3-0.0.3/README.md
+-rw-r--r--   0 takefuji  (1000) takefuji  (1000)       38 2024-05-17 22:35:13.374696 vuc3-0.0.3/setup.cfg
+-rw-r--r--   0 takefuji  (1000) takefuji  (1000)      933 2024-05-17 22:13:18.000000 vuc3-0.0.3/setup.py
+drwxr-xr-x   0 takefuji  (1000) takefuji  (1000)        0 2024-05-17 22:35:13.374696 vuc3-0.0.3/src/
+drwxr-xr-x   0 takefuji  (1000) takefuji  (1000)        0 2024-05-17 22:35:13.374696 vuc3-0.0.3/src/vuc3.egg-info/
+-rw-r--r--   0 takefuji  (1000) takefuji  (1000)     1456 2024-05-17 22:35:13.000000 vuc3-0.0.3/src/vuc3.egg-info/PKG-INFO
+-rw-r--r--   0 takefuji  (1000) takefuji  (1000)      193 2024-05-17 22:35:13.000000 vuc3-0.0.3/src/vuc3.egg-info/SOURCES.txt
+-rw-r--r--   0 takefuji  (1000) takefuji  (1000)        1 2024-05-17 22:35:13.000000 vuc3-0.0.3/src/vuc3.egg-info/dependency_links.txt
+-rw-r--r--   0 takefuji  (1000) takefuji  (1000)       36 2024-05-17 22:35:13.000000 vuc3-0.0.3/src/vuc3.egg-info/entry_points.txt
+-rw-r--r--   0 takefuji  (1000) takefuji  (1000)        5 2024-05-17 22:35:13.000000 vuc3-0.0.3/src/vuc3.egg-info/top_level.txt
+-rwxr-xr-x   0 takefuji  (1000) takefuji  (1000)     2198 2023-03-04 01:53:17.000000 vuc3-0.0.3/src/vuc3.py
```

### Comparing `vuc3-0.0.2/PKG-INFO` & `vuc3-0.0.3/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: vuc3
-Version: 0.0.2
+Version: 0.0.3
 Summary: effects of vaccines on COVID-19 infection and mortality
-Home-page: https://github.com/y-takefuji/patient
+Home-page: https://github.com/y-takefuji/vuc3
 Author: yoshiyasu takefuji
 Author-email: takefuji@keio.jp
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/y-takefuji/vuc3
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `vuc3-0.0.2/README.md` & `vuc3-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `vuc3-0.0.2/setup.py` & `vuc3-0.0.3/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="vuc3",
-    version="0.0.2",
+    version="0.0.3",
     author="yoshiyasu takefuji",
     author_email="takefuji@keio.jp",
     description="effects of vaccines on COVID-19 infection and mortality",
     long_description=long_description,
     long_description_content_type="text/markdown",
-    url="https://github.com/y-takefuji/patient",
+    url="https://github.com/y-takefuji/vuc3",
     project_urls={
         "Bug Tracker": "https://github.com/y-takefuji/vuc3",
     },
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
```

### Comparing `vuc3-0.0.2/src/vuc3.egg-info/PKG-INFO` & `vuc3-0.0.3/src/vuc3.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: vuc3
-Version: 0.0.2
+Version: 0.0.3
 Summary: effects of vaccines on COVID-19 infection and mortality
-Home-page: https://github.com/y-takefuji/patient
+Home-page: https://github.com/y-takefuji/vuc3
 Author: yoshiyasu takefuji
 Author-email: takefuji@keio.jp
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/y-takefuji/vuc3
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `vuc3-0.0.2/src/vuc3.py` & `vuc3-0.0.3/src/vuc3.py`

 * *Files identical despite different names*

