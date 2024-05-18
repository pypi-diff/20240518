# Comparing `tmp/packaging_demo_avr-0.0.2.tar.gz` & `tmp/packaging_demo_avr-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "packaging_demo_avr-0.0.2.tar", last modified: Fri May 17 06:34:44 2024, max compression
+gzip compressed data, was "packaging_demo_avr-0.0.3.tar", last modified: Fri May 17 06:46:04 2024, max compression
```

## Comparing `packaging_demo_avr-0.0.2.tar` & `packaging_demo_avr-0.0.3.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 avr27     (1000) avr27     (1000)        0 2024-05-17 06:34:44.809688 packaging_demo_avr-0.0.2/
--rw-r--r--   0 avr27     (1000) avr27     (1000)    26955 2024-05-17 06:34:44.809688 packaging_demo_avr-0.0.2/PKG-INFO
--rw-r--r--   0 avr27     (1000) avr27     (1000)    25924 2024-05-17 06:30:57.000000 packaging_demo_avr-0.0.2/README.md
-drwxr-xr-x   0 avr27     (1000) avr27     (1000)        0 2024-05-17 06:34:44.809688 packaging_demo_avr-0.0.2/packaging_demo/
--rw-r--r--   0 avr27     (1000) avr27     (1000)       18 2024-05-12 11:14:18.000000 packaging_demo_avr-0.0.2/packaging_demo/__init__.py
-drwxr-xr-x   0 avr27     (1000) avr27     (1000)        0 2024-05-17 06:34:44.809688 packaging_demo_avr-0.0.2/packaging_demo/assets/
--rw-r--r--   0 avr27     (1000) avr27     (1000)        0 2024-05-17 06:00:25.000000 packaging_demo_avr-0.0.2/packaging_demo/assets/__init__.py
--rw-r--r--   0 avr27     (1000) avr27     (1000)   287499 2024-05-15 11:09:26.000000 packaging_demo_avr-0.0.2/packaging_demo/assets/dependency-graph.png
--rw-r--r--   0 avr27     (1000) avr27     (1000)     2282 2024-05-17 04:24:28.000000 packaging_demo_avr-0.0.2/packaging_demo/cities.json
--rw-r--r--   0 avr27     (1000) avr27     (1000)      134 2024-05-16 02:51:30.000000 packaging_demo_avr-0.0.2/packaging_demo/colorized_demo.py
--rw-r--r--   0 avr27     (1000) avr27     (1000)      281 2024-05-12 11:42:54.000000 packaging_demo_avr-0.0.2/packaging_demo/my_file.py
-drwxr-xr-x   0 avr27     (1000) avr27     (1000)        0 2024-05-17 06:34:44.809688 packaging_demo_avr-0.0.2/packaging_demo/my_folder/
--rw-r--r--   0 avr27     (1000) avr27     (1000)        6 2024-05-11 02:32:35.000000 packaging_demo_avr-0.0.2/packaging_demo/my_folder/__init__.py
--rw-r--r--   0 avr27     (1000) avr27     (1000)     2282 2024-05-17 04:24:28.000000 packaging_demo_avr-0.0.2/packaging_demo/my_folder/another-cities.json
--rw-r--r--   0 avr27     (1000) avr27     (1000)      196 2024-05-12 11:42:54.000000 packaging_demo_avr-0.0.2/packaging_demo/my_folder/my_nested_file.py
-drwxr-xr-x   0 avr27     (1000) avr27     (1000)        0 2024-05-17 06:34:44.809688 packaging_demo_avr-0.0.2/packaging_demo/my_folder/my_sub_package/
--rw-r--r--   0 avr27     (1000) avr27     (1000)        0 2024-05-11 06:29:23.000000 packaging_demo_avr-0.0.2/packaging_demo/my_folder/my_sub_package/__init__.py
--rw-r--r--   0 avr27     (1000) avr27     (1000)      198 2024-05-11 04:27:59.000000 packaging_demo_avr-0.0.2/packaging_demo/my_folder/my_sub_package/nested_module.py
--rw-r--r--   0 avr27     (1000) avr27     (1000)       37 2024-05-11 06:56:11.000000 packaging_demo_avr-0.0.2/packaging_demo/my_other_file.py
--rw-r--r--   0 avr27     (1000) avr27     (1000)      864 2024-05-15 04:07:16.000000 packaging_demo_avr-0.0.2/packaging_demo/states_info.py
-drwxr-xr-x   0 avr27     (1000) avr27     (1000)        0 2024-05-17 06:34:44.809688 packaging_demo_avr-0.0.2/packaging_demo_avr.egg-info/
--rw-r--r--   0 avr27     (1000) avr27     (1000)    26955 2024-05-17 06:34:44.000000 packaging_demo_avr-0.0.2/packaging_demo_avr.egg-info/PKG-INFO
--rw-r--r--   0 avr27     (1000) avr27     (1000)      728 2024-05-17 06:34:44.000000 packaging_demo_avr-0.0.2/packaging_demo_avr.egg-info/SOURCES.txt
--rw-r--r--   0 avr27     (1000) avr27     (1000)        1 2024-05-17 06:34:44.000000 packaging_demo_avr-0.0.2/packaging_demo_avr.egg-info/dependency_links.txt
--rw-r--r--   0 avr27     (1000) avr27     (1000)      255 2024-05-17 06:34:44.000000 packaging_demo_avr-0.0.2/packaging_demo_avr.egg-info/requires.txt
--rw-r--r--   0 avr27     (1000) avr27     (1000)       15 2024-05-17 06:34:44.000000 packaging_demo_avr-0.0.2/packaging_demo_avr.egg-info/top_level.txt
--rw-r--r--   0 avr27     (1000) avr27     (1000)     2540 2024-05-17 06:34:36.000000 packaging_demo_avr-0.0.2/pyproject.toml
--rw-r--r--   0 avr27     (1000) avr27     (1000)       38 2024-05-17 06:34:44.809688 packaging_demo_avr-0.0.2/setup.cfg
--rw-r--r--   0 avr27     (1000) avr27     (1000)       39 2024-05-12 13:06:35.000000 packaging_demo_avr-0.0.2/setup.py
+drwxr-xr-x   0 avr27     (1000) avr27     (1000)        0 2024-05-17 06:46:04.379533 packaging_demo_avr-0.0.3/
+-rw-r--r--   0 avr27     (1000) avr27     (1000)    27097 2024-05-17 06:46:04.379533 packaging_demo_avr-0.0.3/PKG-INFO
+-rw-r--r--   0 avr27     (1000) avr27     (1000)    26066 2024-05-17 06:36:06.000000 packaging_demo_avr-0.0.3/README.md
+drwxr-xr-x   0 avr27     (1000) avr27     (1000)        0 2024-05-17 06:46:04.379533 packaging_demo_avr-0.0.3/packaging_demo/
+-rw-r--r--   0 avr27     (1000) avr27     (1000)       18 2024-05-12 11:14:18.000000 packaging_demo_avr-0.0.3/packaging_demo/__init__.py
+drwxr-xr-x   0 avr27     (1000) avr27     (1000)        0 2024-05-17 06:46:04.379533 packaging_demo_avr-0.0.3/packaging_demo/assets/
+-rw-r--r--   0 avr27     (1000) avr27     (1000)        0 2024-05-17 06:00:25.000000 packaging_demo_avr-0.0.3/packaging_demo/assets/__init__.py
+-rw-r--r--   0 avr27     (1000) avr27     (1000)   287499 2024-05-15 11:09:26.000000 packaging_demo_avr-0.0.3/packaging_demo/assets/dependency-graph.png
+-rw-r--r--   0 avr27     (1000) avr27     (1000)     2282 2024-05-17 04:24:28.000000 packaging_demo_avr-0.0.3/packaging_demo/cities.json
+-rw-r--r--   0 avr27     (1000) avr27     (1000)      134 2024-05-16 02:51:30.000000 packaging_demo_avr-0.0.3/packaging_demo/colorized_demo.py
+-rw-r--r--   0 avr27     (1000) avr27     (1000)      281 2024-05-12 11:42:54.000000 packaging_demo_avr-0.0.3/packaging_demo/my_file.py
+drwxr-xr-x   0 avr27     (1000) avr27     (1000)        0 2024-05-17 06:46:04.379533 packaging_demo_avr-0.0.3/packaging_demo/my_folder/
+-rw-r--r--   0 avr27     (1000) avr27     (1000)        6 2024-05-11 02:32:35.000000 packaging_demo_avr-0.0.3/packaging_demo/my_folder/__init__.py
+-rw-r--r--   0 avr27     (1000) avr27     (1000)     2282 2024-05-17 04:24:28.000000 packaging_demo_avr-0.0.3/packaging_demo/my_folder/another-cities.json
+-rw-r--r--   0 avr27     (1000) avr27     (1000)      196 2024-05-12 11:42:54.000000 packaging_demo_avr-0.0.3/packaging_demo/my_folder/my_nested_file.py
+drwxr-xr-x   0 avr27     (1000) avr27     (1000)        0 2024-05-17 06:46:04.379533 packaging_demo_avr-0.0.3/packaging_demo/my_folder/my_sub_package/
+-rw-r--r--   0 avr27     (1000) avr27     (1000)        0 2024-05-11 06:29:23.000000 packaging_demo_avr-0.0.3/packaging_demo/my_folder/my_sub_package/__init__.py
+-rw-r--r--   0 avr27     (1000) avr27     (1000)      198 2024-05-11 04:27:59.000000 packaging_demo_avr-0.0.3/packaging_demo/my_folder/my_sub_package/nested_module.py
+-rw-r--r--   0 avr27     (1000) avr27     (1000)       37 2024-05-11 06:56:11.000000 packaging_demo_avr-0.0.3/packaging_demo/my_other_file.py
+-rw-r--r--   0 avr27     (1000) avr27     (1000)      864 2024-05-15 04:07:16.000000 packaging_demo_avr-0.0.3/packaging_demo/states_info.py
+drwxr-xr-x   0 avr27     (1000) avr27     (1000)        0 2024-05-17 06:46:04.379533 packaging_demo_avr-0.0.3/packaging_demo_avr.egg-info/
+-rw-r--r--   0 avr27     (1000) avr27     (1000)    27097 2024-05-17 06:46:04.000000 packaging_demo_avr-0.0.3/packaging_demo_avr.egg-info/PKG-INFO
+-rw-r--r--   0 avr27     (1000) avr27     (1000)      728 2024-05-17 06:46:04.000000 packaging_demo_avr-0.0.3/packaging_demo_avr.egg-info/SOURCES.txt
+-rw-r--r--   0 avr27     (1000) avr27     (1000)        1 2024-05-17 06:46:04.000000 packaging_demo_avr-0.0.3/packaging_demo_avr.egg-info/dependency_links.txt
+-rw-r--r--   0 avr27     (1000) avr27     (1000)      255 2024-05-17 06:46:04.000000 packaging_demo_avr-0.0.3/packaging_demo_avr.egg-info/requires.txt
+-rw-r--r--   0 avr27     (1000) avr27     (1000)       15 2024-05-17 06:46:04.000000 packaging_demo_avr-0.0.3/packaging_demo_avr.egg-info/top_level.txt
+-rw-r--r--   0 avr27     (1000) avr27     (1000)     2612 2024-05-17 06:43:45.000000 packaging_demo_avr-0.0.3/pyproject.toml
+-rw-r--r--   0 avr27     (1000) avr27     (1000)       38 2024-05-17 06:46:04.379533 packaging_demo_avr-0.0.3/setup.cfg
+-rw-r--r--   0 avr27     (1000) avr27     (1000)       39 2024-05-12 13:06:35.000000 packaging_demo_avr-0.0.3/setup.py
```

### Comparing `packaging_demo_avr-0.0.2/PKG-INFO` & `packaging_demo_avr-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: packaging-demo-avr
-Version: 0.0.2
+Version: 0.0.3
 Summary: Demo for Python Packaging
 Author-email: Amit Vikram Raj <avr13405@gmail.com>
 License: MIT
 Keywords: one,two
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
@@ -664,15 +664,17 @@
 
 sudo apt-get install graphviz  
 
 # generate the dependency graph
 pipdeptree -p packaging-demo --graph-output png > dependency-graph.png
 ```
 
-<img href='https://raw.githubusercontent.com/avr2002/python-packaging/main/packaging_demo/assets/dependency-graph.png' alt='Dependency Graph of packaging-demo package' title='Dependency Graph of packaging-demo package'>
+<a href='https://raw.githubusercontent.com/avr2002/python-packaging/main/packaging_demo/assets/dependency-graph.png' target='_blank'>
+    <img src='https://raw.githubusercontent.com/avr2002/python-packaging/main/packaging_demo/assets/dependency-graph.png' alt='Dependency Graph of packaging-demo package' title='Dependency Graph of packaging-demo package'>
+</a>
 
 * **
 
 ## Adding Optional/Extra Dependencies to our Project
 
 ```toml
 [project.optional-dependencies]
```

### Comparing `packaging_demo_avr-0.0.2/README.md` & `packaging_demo_avr-0.0.3/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -633,15 +633,17 @@
 
 sudo apt-get install graphviz  
 
 # generate the dependency graph
 pipdeptree -p packaging-demo --graph-output png > dependency-graph.png
 ```
 
-<img href='https://raw.githubusercontent.com/avr2002/python-packaging/main/packaging_demo/assets/dependency-graph.png' alt='Dependency Graph of packaging-demo package' title='Dependency Graph of packaging-demo package'>
+<a href='https://raw.githubusercontent.com/avr2002/python-packaging/main/packaging_demo/assets/dependency-graph.png' target='_blank'>
+    <img src='https://raw.githubusercontent.com/avr2002/python-packaging/main/packaging_demo/assets/dependency-graph.png' alt='Dependency Graph of packaging-demo package' title='Dependency Graph of packaging-demo package'>
+</a>
 
 * **
 
 ## Adding Optional/Extra Dependencies to our Project
 
 ```toml
 [project.optional-dependencies]
```

### Comparing `packaging_demo_avr-0.0.2/packaging_demo/assets/dependency-graph.png` & `packaging_demo_avr-0.0.3/packaging_demo/assets/dependency-graph.png`

 * *Files identical despite different names*

### Comparing `packaging_demo_avr-0.0.2/packaging_demo/cities.json` & `packaging_demo_avr-0.0.3/packaging_demo/cities.json`

 * *Files identical despite different names*

### Comparing `packaging_demo_avr-0.0.2/packaging_demo/my_folder/another-cities.json` & `packaging_demo_avr-0.0.3/packaging_demo/my_folder/another-cities.json`

 * *Files identical despite different names*

### Comparing `packaging_demo_avr-0.0.2/packaging_demo/states_info.py` & `packaging_demo_avr-0.0.3/packaging_demo/states_info.py`

 * *Files identical despite different names*

### Comparing `packaging_demo_avr-0.0.2/packaging_demo_avr.egg-info/PKG-INFO` & `packaging_demo_avr-0.0.3/packaging_demo_avr.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: packaging-demo-avr
-Version: 0.0.2
+Version: 0.0.3
 Summary: Demo for Python Packaging
 Author-email: Amit Vikram Raj <avr13405@gmail.com>
 License: MIT
 Keywords: one,two
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
@@ -664,15 +664,17 @@
 
 sudo apt-get install graphviz  
 
 # generate the dependency graph
 pipdeptree -p packaging-demo --graph-output png > dependency-graph.png
 ```
 
-<img href='https://raw.githubusercontent.com/avr2002/python-packaging/main/packaging_demo/assets/dependency-graph.png' alt='Dependency Graph of packaging-demo package' title='Dependency Graph of packaging-demo package'>
+<a href='https://raw.githubusercontent.com/avr2002/python-packaging/main/packaging_demo/assets/dependency-graph.png' target='_blank'>
+    <img src='https://raw.githubusercontent.com/avr2002/python-packaging/main/packaging_demo/assets/dependency-graph.png' alt='Dependency Graph of packaging-demo package' title='Dependency Graph of packaging-demo package'>
+</a>
 
 * **
 
 ## Adding Optional/Extra Dependencies to our Project
 
 ```toml
 [project.optional-dependencies]
```

### Comparing `packaging_demo_avr-0.0.2/packaging_demo_avr.egg-info/SOURCES.txt` & `packaging_demo_avr-0.0.3/packaging_demo_avr.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `packaging_demo_avr-0.0.2/pyproject.toml` & `packaging_demo_avr-0.0.3/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 [build-system]
 # Minimum requirements for the build system to execute
 requires = ["setuptools>=61.0.0", "wheel"]
 # default value of build-backend is "setuptools.build_meta"
 build-backend = "setuptools.build_meta"
 
+# include-package-data defaults to true, not needed to add in toml file
 [tool.setuptools]
 include-package-data = true
 
 [tool.setuptools.package-data]
 packaging_demo = ["**/*.json", "**/*png"]
 
 [project]
@@ -17,15 +18,15 @@
 readme = "README.md"
 requires-python = ">=3.8"
 keywords = ["one", "two"]
 license = { text = "MIT" }
 classifiers = ["Programming Language :: Python :: 3"]
 dependencies = ["numpy", "fastapi", 'importlib-metadata; python_version<"3.10"']
 # dynamic = ["version"]
-version = "0.0.2"
+version = "0.0.3"
 
 [project.optional-dependencies]
 test = ["pytest", "pytest-cov"]
 release = ["build", "twine"]
 static-code-qa = ["pre-commit"]
 # for developement
 dev = ["ruff", "mypy", "black", "packaging-demo[test, release, static-code-qa]"]
```

