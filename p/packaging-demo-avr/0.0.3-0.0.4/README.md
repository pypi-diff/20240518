# Comparing `tmp/packaging_demo_avr-0.0.3.tar.gz` & `tmp/packaging_demo_avr-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "packaging_demo_avr-0.0.3.tar", last modified: Fri May 17 06:46:04 2024, max compression
+gzip compressed data, was "packaging_demo_avr-0.0.4.tar", last modified: Sat May 18 01:57:11 2024, max compression
```

## Comparing `packaging_demo_avr-0.0.3.tar` & `packaging_demo_avr-0.0.4.tar`

### file list

```diff
@@ -1,29 +1,26 @@
-drwxr-xr-x   0 avr27     (1000) avr27     (1000)        0 2024-05-17 06:46:04.379533 packaging_demo_avr-0.0.3/
--rw-r--r--   0 avr27     (1000) avr27     (1000)    27097 2024-05-17 06:46:04.379533 packaging_demo_avr-0.0.3/PKG-INFO
--rw-r--r--   0 avr27     (1000) avr27     (1000)    26066 2024-05-17 06:36:06.000000 packaging_demo_avr-0.0.3/README.md
-drwxr-xr-x   0 avr27     (1000) avr27     (1000)        0 2024-05-17 06:46:04.379533 packaging_demo_avr-0.0.3/packaging_demo/
--rw-r--r--   0 avr27     (1000) avr27     (1000)       18 2024-05-12 11:14:18.000000 packaging_demo_avr-0.0.3/packaging_demo/__init__.py
-drwxr-xr-x   0 avr27     (1000) avr27     (1000)        0 2024-05-17 06:46:04.379533 packaging_demo_avr-0.0.3/packaging_demo/assets/
--rw-r--r--   0 avr27     (1000) avr27     (1000)        0 2024-05-17 06:00:25.000000 packaging_demo_avr-0.0.3/packaging_demo/assets/__init__.py
--rw-r--r--   0 avr27     (1000) avr27     (1000)   287499 2024-05-15 11:09:26.000000 packaging_demo_avr-0.0.3/packaging_demo/assets/dependency-graph.png
--rw-r--r--   0 avr27     (1000) avr27     (1000)     2282 2024-05-17 04:24:28.000000 packaging_demo_avr-0.0.3/packaging_demo/cities.json
--rw-r--r--   0 avr27     (1000) avr27     (1000)      134 2024-05-16 02:51:30.000000 packaging_demo_avr-0.0.3/packaging_demo/colorized_demo.py
--rw-r--r--   0 avr27     (1000) avr27     (1000)      281 2024-05-12 11:42:54.000000 packaging_demo_avr-0.0.3/packaging_demo/my_file.py
-drwxr-xr-x   0 avr27     (1000) avr27     (1000)        0 2024-05-17 06:46:04.379533 packaging_demo_avr-0.0.3/packaging_demo/my_folder/
--rw-r--r--   0 avr27     (1000) avr27     (1000)        6 2024-05-11 02:32:35.000000 packaging_demo_avr-0.0.3/packaging_demo/my_folder/__init__.py
--rw-r--r--   0 avr27     (1000) avr27     (1000)     2282 2024-05-17 04:24:28.000000 packaging_demo_avr-0.0.3/packaging_demo/my_folder/another-cities.json
--rw-r--r--   0 avr27     (1000) avr27     (1000)      196 2024-05-12 11:42:54.000000 packaging_demo_avr-0.0.3/packaging_demo/my_folder/my_nested_file.py
-drwxr-xr-x   0 avr27     (1000) avr27     (1000)        0 2024-05-17 06:46:04.379533 packaging_demo_avr-0.0.3/packaging_demo/my_folder/my_sub_package/
--rw-r--r--   0 avr27     (1000) avr27     (1000)        0 2024-05-11 06:29:23.000000 packaging_demo_avr-0.0.3/packaging_demo/my_folder/my_sub_package/__init__.py
--rw-r--r--   0 avr27     (1000) avr27     (1000)      198 2024-05-11 04:27:59.000000 packaging_demo_avr-0.0.3/packaging_demo/my_folder/my_sub_package/nested_module.py
--rw-r--r--   0 avr27     (1000) avr27     (1000)       37 2024-05-11 06:56:11.000000 packaging_demo_avr-0.0.3/packaging_demo/my_other_file.py
--rw-r--r--   0 avr27     (1000) avr27     (1000)      864 2024-05-15 04:07:16.000000 packaging_demo_avr-0.0.3/packaging_demo/states_info.py
-drwxr-xr-x   0 avr27     (1000) avr27     (1000)        0 2024-05-17 06:46:04.379533 packaging_demo_avr-0.0.3/packaging_demo_avr.egg-info/
--rw-r--r--   0 avr27     (1000) avr27     (1000)    27097 2024-05-17 06:46:04.000000 packaging_demo_avr-0.0.3/packaging_demo_avr.egg-info/PKG-INFO
--rw-r--r--   0 avr27     (1000) avr27     (1000)      728 2024-05-17 06:46:04.000000 packaging_demo_avr-0.0.3/packaging_demo_avr.egg-info/SOURCES.txt
--rw-r--r--   0 avr27     (1000) avr27     (1000)        1 2024-05-17 06:46:04.000000 packaging_demo_avr-0.0.3/packaging_demo_avr.egg-info/dependency_links.txt
--rw-r--r--   0 avr27     (1000) avr27     (1000)      255 2024-05-17 06:46:04.000000 packaging_demo_avr-0.0.3/packaging_demo_avr.egg-info/requires.txt
--rw-r--r--   0 avr27     (1000) avr27     (1000)       15 2024-05-17 06:46:04.000000 packaging_demo_avr-0.0.3/packaging_demo_avr.egg-info/top_level.txt
--rw-r--r--   0 avr27     (1000) avr27     (1000)     2612 2024-05-17 06:43:45.000000 packaging_demo_avr-0.0.3/pyproject.toml
--rw-r--r--   0 avr27     (1000) avr27     (1000)       38 2024-05-17 06:46:04.379533 packaging_demo_avr-0.0.3/setup.cfg
--rw-r--r--   0 avr27     (1000) avr27     (1000)       39 2024-05-12 13:06:35.000000 packaging_demo_avr-0.0.3/setup.py
+drwxr-xr-x   0 avr27     (1000) avr27     (1000)        0 2024-05-18 01:57:11.189787 packaging_demo_avr-0.0.4/
+-rw-r--r--   0 avr27     (1000) avr27     (1000)    27488 2024-05-18 01:57:11.189787 packaging_demo_avr-0.0.4/PKG-INFO
+-rw-r--r--   0 avr27     (1000) avr27     (1000)    26457 2024-05-18 01:55:36.000000 packaging_demo_avr-0.0.4/README.md
+drwxr-xr-x   0 avr27     (1000) avr27     (1000)        0 2024-05-18 01:57:11.179787 packaging_demo_avr-0.0.4/packaging_demo/
+-rw-r--r--   0 avr27     (1000) avr27     (1000)       18 2024-05-18 01:55:57.000000 packaging_demo_avr-0.0.4/packaging_demo/__init__.py
+-rw-r--r--   0 avr27     (1000) avr27     (1000)     2282 2024-05-17 04:24:28.000000 packaging_demo_avr-0.0.4/packaging_demo/cities.json
+-rw-r--r--   0 avr27     (1000) avr27     (1000)      134 2024-05-16 02:51:30.000000 packaging_demo_avr-0.0.4/packaging_demo/colorized_demo.py
+-rw-r--r--   0 avr27     (1000) avr27     (1000)      281 2024-05-12 11:42:54.000000 packaging_demo_avr-0.0.4/packaging_demo/my_file.py
+drwxr-xr-x   0 avr27     (1000) avr27     (1000)        0 2024-05-18 01:57:11.179787 packaging_demo_avr-0.0.4/packaging_demo/my_folder/
+-rw-r--r--   0 avr27     (1000) avr27     (1000)        6 2024-05-11 02:32:35.000000 packaging_demo_avr-0.0.4/packaging_demo/my_folder/__init__.py
+-rw-r--r--   0 avr27     (1000) avr27     (1000)     2282 2024-05-17 04:24:28.000000 packaging_demo_avr-0.0.4/packaging_demo/my_folder/another-cities.json
+-rw-r--r--   0 avr27     (1000) avr27     (1000)      196 2024-05-12 11:42:54.000000 packaging_demo_avr-0.0.4/packaging_demo/my_folder/my_nested_file.py
+drwxr-xr-x   0 avr27     (1000) avr27     (1000)        0 2024-05-18 01:57:11.179787 packaging_demo_avr-0.0.4/packaging_demo/my_folder/my_sub_package/
+-rw-r--r--   0 avr27     (1000) avr27     (1000)        0 2024-05-11 06:29:23.000000 packaging_demo_avr-0.0.4/packaging_demo/my_folder/my_sub_package/__init__.py
+-rw-r--r--   0 avr27     (1000) avr27     (1000)      198 2024-05-11 04:27:59.000000 packaging_demo_avr-0.0.4/packaging_demo/my_folder/my_sub_package/nested_module.py
+-rw-r--r--   0 avr27     (1000) avr27     (1000)       37 2024-05-11 06:56:11.000000 packaging_demo_avr-0.0.4/packaging_demo/my_other_file.py
+-rw-r--r--   0 avr27     (1000) avr27     (1000)      864 2024-05-15 04:07:16.000000 packaging_demo_avr-0.0.4/packaging_demo/states_info.py
+drwxr-xr-x   0 avr27     (1000) avr27     (1000)        0 2024-05-18 01:57:11.179787 packaging_demo_avr-0.0.4/packaging_demo_avr.egg-info/
+-rw-r--r--   0 avr27     (1000) avr27     (1000)    27488 2024-05-18 01:57:11.000000 packaging_demo_avr-0.0.4/packaging_demo_avr.egg-info/PKG-INFO
+-rw-r--r--   0 avr27     (1000) avr27     (1000)      654 2024-05-18 01:57:11.000000 packaging_demo_avr-0.0.4/packaging_demo_avr.egg-info/SOURCES.txt
+-rw-r--r--   0 avr27     (1000) avr27     (1000)        1 2024-05-18 01:57:11.000000 packaging_demo_avr-0.0.4/packaging_demo_avr.egg-info/dependency_links.txt
+-rw-r--r--   0 avr27     (1000) avr27     (1000)      255 2024-05-18 01:57:11.000000 packaging_demo_avr-0.0.4/packaging_demo_avr.egg-info/requires.txt
+-rw-r--r--   0 avr27     (1000) avr27     (1000)       15 2024-05-18 01:57:11.000000 packaging_demo_avr-0.0.4/packaging_demo_avr.egg-info/top_level.txt
+-rw-r--r--   0 avr27     (1000) avr27     (1000)     2992 2024-05-18 01:54:48.000000 packaging_demo_avr-0.0.4/pyproject.toml
+-rw-r--r--   0 avr27     (1000) avr27     (1000)       38 2024-05-18 01:57:11.189787 packaging_demo_avr-0.0.4/setup.cfg
+-rw-r--r--   0 avr27     (1000) avr27     (1000)        6 2024-05-18 01:56:05.000000 packaging_demo_avr-0.0.4/version.txt
```

### Comparing `packaging_demo_avr-0.0.3/PKG-INFO` & `packaging_demo_avr-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: packaging-demo-avr
-Version: 0.0.3
+Version: 0.0.4
 Summary: Demo for Python Packaging
 Author-email: Amit Vikram Raj <avr13405@gmail.com>
 License: MIT
 Keywords: one,two
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
@@ -495,16 +495,22 @@
 description = "Demo for Python Packaging"
 readme = "README.md"
 requires-python = ">=3.8"
 keywords = ["one", "two"]
 license = { text = "MIT" }
 classifiers = ["Programming Language :: Python :: 3"]
 dependencies = ["numpy", 'importlib-metadata; python_version<"3.10"']
-# dynamic = ["version"]
-version = "0.0.0"
+dynamic = ["version"]
+# version = "0.0.3"
+# https://setuptools.pypa.io/en/latest/userguide/pyproject_config.html#dynamic-metadata
+
+[tool.setuptools.dynamic]
+# every while making changes in package, you can change the verison in one of these files
+# version = {attr = "packaging_demo.VERSION"} # version read by 'packaging_demo/__init__.py' file
+version = {file  = ["version.txt"]} # version read by 'version.txt' file in root folder
 ```
 
 >> `python -m build --sdist --wheel .` - Runs perfectly, we got rid of another config file (`setup.cfg`)
 
 
 ## Replacing `setup.py` with `build-backend`
```

### Comparing `packaging_demo_avr-0.0.3/README.md` & `packaging_demo_avr-0.0.4/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -464,16 +464,22 @@
 description = "Demo for Python Packaging"
 readme = "README.md"
 requires-python = ">=3.8"
 keywords = ["one", "two"]
 license = { text = "MIT" }
 classifiers = ["Programming Language :: Python :: 3"]
 dependencies = ["numpy", 'importlib-metadata; python_version<"3.10"']
-# dynamic = ["version"]
-version = "0.0.0"
+dynamic = ["version"]
+# version = "0.0.3"
+# https://setuptools.pypa.io/en/latest/userguide/pyproject_config.html#dynamic-metadata
+
+[tool.setuptools.dynamic]
+# every while making changes in package, you can change the verison in one of these files
+# version = {attr = "packaging_demo.VERSION"} # version read by 'packaging_demo/__init__.py' file
+version = {file  = ["version.txt"]} # version read by 'version.txt' file in root folder
 ```
 
 >> `python -m build --sdist --wheel .` - Runs perfectly, we got rid of another config file (`setup.cfg`)
 
 
 ## Replacing `setup.py` with `build-backend`
```

### Comparing `packaging_demo_avr-0.0.3/packaging_demo/cities.json` & `packaging_demo_avr-0.0.4/packaging_demo/cities.json`

 * *Files identical despite different names*

### Comparing `packaging_demo_avr-0.0.3/packaging_demo/my_folder/another-cities.json` & `packaging_demo_avr-0.0.4/packaging_demo/my_folder/another-cities.json`

 * *Files identical despite different names*

### Comparing `packaging_demo_avr-0.0.3/packaging_demo/states_info.py` & `packaging_demo_avr-0.0.4/packaging_demo/states_info.py`

 * *Files identical despite different names*

### Comparing `packaging_demo_avr-0.0.3/packaging_demo_avr.egg-info/PKG-INFO` & `packaging_demo_avr-0.0.4/packaging_demo_avr.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: packaging-demo-avr
-Version: 0.0.3
+Version: 0.0.4
 Summary: Demo for Python Packaging
 Author-email: Amit Vikram Raj <avr13405@gmail.com>
 License: MIT
 Keywords: one,two
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
@@ -495,16 +495,22 @@
 description = "Demo for Python Packaging"
 readme = "README.md"
 requires-python = ">=3.8"
 keywords = ["one", "two"]
 license = { text = "MIT" }
 classifiers = ["Programming Language :: Python :: 3"]
 dependencies = ["numpy", 'importlib-metadata; python_version<"3.10"']
-# dynamic = ["version"]
-version = "0.0.0"
+dynamic = ["version"]
+# version = "0.0.3"
+# https://setuptools.pypa.io/en/latest/userguide/pyproject_config.html#dynamic-metadata
+
+[tool.setuptools.dynamic]
+# every while making changes in package, you can change the verison in one of these files
+# version = {attr = "packaging_demo.VERSION"} # version read by 'packaging_demo/__init__.py' file
+version = {file  = ["version.txt"]} # version read by 'version.txt' file in root folder
 ```
 
 >> `python -m build --sdist --wheel .` - Runs perfectly, we got rid of another config file (`setup.cfg`)
 
 
 ## Replacing `setup.py` with `build-backend`
```

### Comparing `packaging_demo_avr-0.0.3/pyproject.toml` & `packaging_demo_avr-0.0.4/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -5,28 +5,34 @@
 build-backend = "setuptools.build_meta"
 
 # include-package-data defaults to true, not needed to add in toml file
 [tool.setuptools]
 include-package-data = true
 
 [tool.setuptools.package-data]
-packaging_demo = ["**/*.json", "**/*png"]
+packaging_demo = ["**/*.json"]
 
 [project]
 name = "packaging-demo-avr"
 authors = [{ name = "Amit Vikram Raj", email = "avr13405@gmail.com" }]
 description = "Demo for Python Packaging"
 readme = "README.md"
 requires-python = ">=3.8"
 keywords = ["one", "two"]
 license = { text = "MIT" }
 classifiers = ["Programming Language :: Python :: 3"]
 dependencies = ["numpy", "fastapi", 'importlib-metadata; python_version<"3.10"']
-# dynamic = ["version"]
-version = "0.0.3"
+dynamic = ["version"]
+# version = "0.0.3"
+# https://setuptools.pypa.io/en/latest/userguide/pyproject_config.html#dynamic-metadata
+
+[tool.setuptools.dynamic]
+# every while making changes in package, you can change the verison in one of these files
+# version = {attr = "packaging_demo.VERSION"} # version read by 'packaging_demo/__init__.py' file
+version = {file  = ["version.txt"]} # version read by 'version.txt' file in root folder
 
 [project.optional-dependencies]
 test = ["pytest", "pytest-cov"]
 release = ["build", "twine"]
 static-code-qa = ["pre-commit"]
 # for developement
 dev = ["ruff", "mypy", "black", "packaging-demo[test, release, static-code-qa]"]
```

