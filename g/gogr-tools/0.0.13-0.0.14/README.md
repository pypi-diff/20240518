# Comparing `tmp/gogr_tools-0.0.13.tar.gz` & `tmp/gogr_tools-0.0.14.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gogr_tools-0.0.13.tar", last modified: Sat May 18 12:02:41 2024, max compression
+gzip compressed data, was "gogr_tools-0.0.14.tar", last modified: Sat May 18 12:21:15 2024, max compression
```

## Comparing `gogr_tools-0.0.13.tar` & `gogr_tools-0.0.14.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-05-18 12:02:41.262578 gogr_tools-0.0.13/
--rw-rw-rw-   0        0        0     1091 2024-05-18 10:47:16.000000 gogr_tools-0.0.13/LICENSE.txt
--rw-rw-rw-   0        0        0      702 2024-05-18 12:02:41.262578 gogr_tools-0.0.13/PKG-INFO
--rw-rw-rw-   0        0        0      122 2024-05-18 10:32:19.000000 gogr_tools-0.0.13/README.md
-drwxrwxrwx   0        0        0        0 2024-05-18 12:02:41.257580 gogr_tools-0.0.13/gogr_tools/
--rw-rw-rw-   0        0        0        0 2024-05-18 11:45:28.000000 gogr_tools-0.0.13/gogr_tools/__init__.py
--rw-rw-rw-   0        0        0     6349 2024-05-18 10:25:39.000000 gogr_tools-0.0.13/gogr_tools/visualisations.py
-drwxrwxrwx   0        0        0        0 2024-05-18 12:02:41.259579 gogr_tools-0.0.13/gogr_tools.egg-info/
--rw-rw-rw-   0        0        0      702 2024-05-18 12:02:41.000000 gogr_tools-0.0.13/gogr_tools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      233 2024-05-18 12:02:41.000000 gogr_tools-0.0.13/gogr_tools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-18 12:02:41.000000 gogr_tools-0.0.13/gogr_tools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2024-05-18 12:02:41.000000 gogr_tools-0.0.13/gogr_tools.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      626 2024-05-18 12:02:23.000000 gogr_tools-0.0.13/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-18 12:02:41.262578 gogr_tools-0.0.13/setup.cfg
--rw-rw-rw-   0        0        0      956 2024-05-18 12:02:18.000000 gogr_tools-0.0.13/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-18 12:21:15.151081 gogr_tools-0.0.14/
+-rw-rw-rw-   0        0        0     1091 2024-05-18 10:47:16.000000 gogr_tools-0.0.14/LICENSE.txt
+-rw-rw-rw-   0        0        0      702 2024-05-18 12:21:15.151081 gogr_tools-0.0.14/PKG-INFO
+-rw-rw-rw-   0        0        0      122 2024-05-18 10:32:19.000000 gogr_tools-0.0.14/README.md
+drwxrwxrwx   0        0        0        0 2024-05-18 12:21:15.146082 gogr_tools-0.0.14/gogr_tools/
+-rw-rw-rw-   0        0        0        0 2024-05-18 11:45:28.000000 gogr_tools-0.0.14/gogr_tools/__init__.py
+-rw-rw-rw-   0        0        0     6345 2024-05-18 12:19:58.000000 gogr_tools-0.0.14/gogr_tools/visualisations.py
+drwxrwxrwx   0        0        0        0 2024-05-18 12:21:15.148082 gogr_tools-0.0.14/gogr_tools.egg-info/
+-rw-rw-rw-   0        0        0      702 2024-05-18 12:21:15.000000 gogr_tools-0.0.14/gogr_tools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      233 2024-05-18 12:21:15.000000 gogr_tools-0.0.14/gogr_tools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-18 12:21:15.000000 gogr_tools-0.0.14/gogr_tools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2024-05-18 12:21:15.000000 gogr_tools-0.0.14/gogr_tools.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      626 2024-05-18 12:20:45.000000 gogr_tools-0.0.14/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-18 12:21:15.151081 gogr_tools-0.0.14/setup.cfg
+-rw-rw-rw-   0        0        0      963 2024-05-18 12:20:41.000000 gogr_tools-0.0.14/setup.py
```

### Comparing `gogr_tools-0.0.13/LICENSE.txt` & `gogr_tools-0.0.14/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `gogr_tools-0.0.13/PKG-INFO` & `gogr_tools-0.0.14/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gogr_tools
-Version: 0.0.13
+Version: 0.0.14
 Summary: Package for Personal use in DataScience
 Author: Grzegorz Gomza
 Author-email: Grzegorz Gomza <gomza.datascience@gmail.com>
 Project-URL: Homepage, https://github.com/grzegorz-gomza/GOGR-Tools
 Project-URL: Issues, https://github.com/grzegorz-gomza/GOGR-Tools/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `gogr_tools-0.0.13/gogr_tools/visualisations.py` & `gogr_tools-0.0.14/gogr_tools/visualisations.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,17 +1,17 @@
+import sys
+
 class ParcatsSankeyPlot:
     def __init__(self, df, columns, chart='sankey', w=1200, h=800):
         self.df = df
         self.columns = columns
         self.chart = chart
         self.w = w
         self.h = h
 
-    import sys
-
     def import_libraries():
         if 'plotly.graph_objects' not in sys.modules:
             print("Importing plotly.graph_objects...")
             import plotly.graph_objects as go
         else:
             print("plotly.graph_objects is already imported.")
```

### Comparing `gogr_tools-0.0.13/gogr_tools.egg-info/PKG-INFO` & `gogr_tools-0.0.14/gogr_tools.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gogr_tools
-Version: 0.0.13
+Version: 0.0.14
 Summary: Package for Personal use in DataScience
 Author: Grzegorz Gomza
 Author-email: Grzegorz Gomza <gomza.datascience@gmail.com>
 Project-URL: Homepage, https://github.com/grzegorz-gomza/GOGR-Tools
 Project-URL: Issues, https://github.com/grzegorz-gomza/GOGR-Tools/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `gogr_tools-0.0.13/pyproject.toml` & `gogr_tools-0.0.14/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "gogr_tools"
-version = "0.0.13"
+version = "0.0.14"
 authors = [
   { name="Grzegorz Gomza", email="gomza.datascience@gmail.com" },
 ]
 description = "Package for Personal use in DataScience"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `gogr_tools-0.0.13/setup.py` & `gogr_tools-0.0.14/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 from setuptools import setup, find_packages
 import codecs
 import os
 
-VERSION = '0.0.13'
+VERSION = '0.0.14'
 DESCRIPTION = 'Package for personal use in Data Science'
 LONG_DESCRIPTION = 'Package for personal use in DataS Science, Machine Learning and Deep Learning'
 
 # Setting up
 setup(
     name="gogr_tools",
     version=VERSION,
     author="Grzegorz Gomza",
     author_email="<gomza.datascience@gmail.com>",
     description=DESCRIPTION,
     long_description_content_type="text/markdown",
     long_description=LONG_DESCRIPTION,
     packages=find_packages(),
-    install_requires=['plotly', 'pandas', 'random'],
+    install_requires=['plotly', 'pandas', 'random', 'sys'],
     keywords=['python', 'Data Science'],
     classifiers=[
         "Development Status :: 1 - Planning",
         "Intended Audience :: Developers",
         "Programming Language :: Python :: 3",
         "Operating System :: Unix",
         "Operating System :: MacOS :: MacOS X",
```

