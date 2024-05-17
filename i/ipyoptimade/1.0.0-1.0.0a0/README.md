# Comparing `tmp/ipyoptimade-1.0.0.tar.gz` & `tmp/ipyoptimade-1.0.0a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ipyoptimade-1.0.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "ipyoptimade-1.0.0a0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `ipyoptimade-1.0.0.tar` & `ipyoptimade-1.0.0a0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0     7549 2024-05-17 22:05:41.971017 ipyoptimade-1.0.0/README.md
--rw-r--r--   0        0        0     2239 2024-05-17 22:05:41.979017 ipyoptimade-1.0.0/pyproject.toml
--rw-r--r--   0        0        0      584 2024-05-17 22:05:41.979017 ipyoptimade-1.0.0/src/ipyoptimade/__init__.py
--rw-r--r--   0        0        0      784 2024-05-17 22:05:41.979017 ipyoptimade-1.0.0/src/ipyoptimade/default_parameters.py
--rw-r--r--   0        0        0     4514 2024-05-17 22:05:41.979017 ipyoptimade-1.0.0/src/ipyoptimade/exceptions.py
--rw-r--r--   0        0        0    16491 2024-05-17 22:05:41.979017 ipyoptimade-1.0.0/src/ipyoptimade/informational.py
--rw-r--r--   0        0        0    10287 2024-05-17 22:05:41.979017 ipyoptimade-1.0.0/src/ipyoptimade/logger.py
--rw-r--r--   0        0        0    22047 2024-05-17 22:05:41.979017 ipyoptimade-1.0.0/src/ipyoptimade/query_filter.py
--rw-r--r--   0        0        0     3895 2024-05-17 22:05:41.979017 ipyoptimade-1.0.0/src/ipyoptimade/query_provider.py
--rw-r--r--   0        0        0   122043 2024-05-17 22:05:41.979017 ipyoptimade-1.0.0/src/ipyoptimade/statics/optimade-text-right-transparent-bg.png
--rw-r--r--   0        0        0      648 2024-05-17 22:05:41.979017 ipyoptimade-1.0.0/src/ipyoptimade/subwidgets/__init__.py
--rw-r--r--   0        0        0    22105 2024-05-17 22:05:41.979017 ipyoptimade-1.0.0/src/ipyoptimade/subwidgets/filter_inputs.py
--rw-r--r--   0        0        0      509 2024-05-17 22:05:41.979017 ipyoptimade-1.0.0/src/ipyoptimade/subwidgets/intrangeslider.py
--rw-r--r--   0        0        0     2964 2024-05-17 22:05:41.979017 ipyoptimade-1.0.0/src/ipyoptimade/subwidgets/multi_checkbox.py
--rw-r--r--   0        0        0    12316 2024-05-17 22:05:41.979017 ipyoptimade-1.0.0/src/ipyoptimade/subwidgets/output_summary.py
--rw-r--r--   0        0        0     3578 2024-05-17 22:05:41.979017 ipyoptimade-1.0.0/src/ipyoptimade/subwidgets/periodic_table.py
--rw-r--r--   0        0        0    27063 2024-05-17 22:05:41.979017 ipyoptimade-1.0.0/src/ipyoptimade/subwidgets/provider_database.py
--rw-r--r--   0        0        0    14475 2024-05-17 22:05:41.979017 ipyoptimade-1.0.0/src/ipyoptimade/subwidgets/results.py
--rw-r--r--   0        0        0     6558 2024-05-17 22:05:41.979017 ipyoptimade-1.0.0/src/ipyoptimade/subwidgets/sort_selector.py
--rw-r--r--   0        0        0    20234 2024-05-17 22:05:41.979017 ipyoptimade-1.0.0/src/ipyoptimade/summary.py
--rw-r--r--   0        0        0    24566 2024-05-17 22:05:41.979017 ipyoptimade-1.0.0/src/ipyoptimade/utils.py
--rw-r--r--   0        0        0       22 2024-05-17 22:05:41.979017 ipyoptimade-1.0.0/src/ipyoptimade/version.py
--rw-r--r--   0        0        0      635 2024-05-17 22:05:41.979017 ipyoptimade-1.0.0/src/ipyoptimade/warnings.py
--rw-r--r--   0        0        0     9606 1970-01-01 00:00:00.000000 ipyoptimade-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     7491 2024-05-16 15:28:57.575510 ipyoptimade-1.0.0a0/README.md
+-rw-r--r--   0        0        0     2218 2024-05-16 15:28:57.579510 ipyoptimade-1.0.0a0/pyproject.toml
+-rw-r--r--   0        0        0      584 2024-05-16 15:28:57.579510 ipyoptimade-1.0.0a0/src/ipyoptimade/__init__.py
+-rw-r--r--   0        0        0      784 2024-05-16 15:28:57.579510 ipyoptimade-1.0.0a0/src/ipyoptimade/default_parameters.py
+-rw-r--r--   0        0        0     4514 2024-05-16 15:28:57.579510 ipyoptimade-1.0.0a0/src/ipyoptimade/exceptions.py
+-rw-r--r--   0        0        0    16491 2024-05-16 15:28:57.579510 ipyoptimade-1.0.0a0/src/ipyoptimade/informational.py
+-rw-r--r--   0        0        0    10287 2024-05-16 15:28:57.579510 ipyoptimade-1.0.0a0/src/ipyoptimade/logger.py
+-rw-r--r--   0        0        0    22047 2024-05-16 15:28:57.579510 ipyoptimade-1.0.0a0/src/ipyoptimade/query_filter.py
+-rw-r--r--   0        0        0     3895 2024-05-16 15:28:57.579510 ipyoptimade-1.0.0a0/src/ipyoptimade/query_provider.py
+-rw-r--r--   0        0        0   122043 2024-05-16 15:28:57.579510 ipyoptimade-1.0.0a0/src/ipyoptimade/statics/optimade-text-right-transparent-bg.png
+-rw-r--r--   0        0        0      648 2024-05-16 15:28:57.579510 ipyoptimade-1.0.0a0/src/ipyoptimade/subwidgets/__init__.py
+-rw-r--r--   0        0        0    22105 2024-05-16 15:28:57.579510 ipyoptimade-1.0.0a0/src/ipyoptimade/subwidgets/filter_inputs.py
+-rw-r--r--   0        0        0      509 2024-05-16 15:28:57.579510 ipyoptimade-1.0.0a0/src/ipyoptimade/subwidgets/intrangeslider.py
+-rw-r--r--   0        0        0     2964 2024-05-16 15:28:57.579510 ipyoptimade-1.0.0a0/src/ipyoptimade/subwidgets/multi_checkbox.py
+-rw-r--r--   0        0        0    12316 2024-05-16 15:28:57.579510 ipyoptimade-1.0.0a0/src/ipyoptimade/subwidgets/output_summary.py
+-rw-r--r--   0        0        0     3578 2024-05-16 15:28:57.579510 ipyoptimade-1.0.0a0/src/ipyoptimade/subwidgets/periodic_table.py
+-rw-r--r--   0        0        0    27063 2024-05-16 15:28:57.583510 ipyoptimade-1.0.0a0/src/ipyoptimade/subwidgets/provider_database.py
+-rw-r--r--   0        0        0    14475 2024-05-16 15:28:57.583510 ipyoptimade-1.0.0a0/src/ipyoptimade/subwidgets/results.py
+-rw-r--r--   0        0        0     6558 2024-05-16 15:28:57.583510 ipyoptimade-1.0.0a0/src/ipyoptimade/subwidgets/sort_selector.py
+-rw-r--r--   0        0        0    20234 2024-05-16 15:28:57.583510 ipyoptimade-1.0.0a0/src/ipyoptimade/summary.py
+-rw-r--r--   0        0        0    24566 2024-05-16 15:28:57.583510 ipyoptimade-1.0.0a0/src/ipyoptimade/utils.py
+-rw-r--r--   0        0        0       24 2024-05-16 15:28:57.583510 ipyoptimade-1.0.0a0/src/ipyoptimade/version.py
+-rw-r--r--   0        0        0      635 2024-05-16 15:28:57.583510 ipyoptimade-1.0.0a0/src/ipyoptimade/warnings.py
+-rw-r--r--   0        0        0     9500 1970-01-01 00:00:00.000000 ipyoptimade-1.0.0a0/PKG-INFO
```

### Comparing `ipyoptimade-1.0.0/README.md` & `ipyoptimade-1.0.0a0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -135,20 +135,14 @@
 
 ```
 export ipyoptimade_DEBUG=1
 ```
 
 to automatically open and show the debug & error messages in the `OptimadeLog()` widget.
 
-Test voila with
-
-```bash
-voila optimade-client.ipynb
-```
-
 ### Making a new release
 
 To create a new release, clone the repository, install development dependencies with `pip install -e '.[dev]'`, and then execute `bumpver update [--major|--minor|--patch] [--tag-num --tag [alpha|beta|rc]]`.
 This will:
 
 1. Create a tagged release with bumped version and push it to the repository.
 2. Trigger a GitHub actions workflow that creates a GitHub release and publishes it on PyPI.
```

### Comparing `ipyoptimade-1.0.0/pyproject.toml` & `ipyoptimade-1.0.0a0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 ]
 requires-python = ">=3.9"
 dynamic = ["version"] # read version from src/ipyoptimade/__init__.py
 dependencies = [
   "appdirs~=1.4.4",
   "cachecontrol[filecache]~=0.13.1",
   "ipywidgets~=8.1",
-  "nglview~=3.0.8",
+  "nglview~=3.0",
   "optimade~=1.0.0",
   "ase~=3.22",
   "pandas~=2.1",
   "requests~=2.31",
   "widget_periodictable~=4.1",
   "semver~=3.0",
 ]
@@ -48,28 +48,27 @@
 [project.optional-dependencies]
 dev = [
   "pre-commit~=3.6",
   "pytest~=7.4",
   "pytest-cov~=4.1",
   "bumpver>=2023.1129",
   "pip-tools~=7.4",
-  "jupyterlab~=4.0",
 ]
-voila = ["voila~=0.4.0"]
+voila = ["voila~=0.5.0"]
 
 [project.urls]
 Documentation = "https://github.com/aiidalab/ipyoptimade#readme"
 Source = "https://github.com/aiidalab/ipyoptimade"
 Tracker = "https://github.com/aiidalab/ipyoptimade/issues"
 
 [tool.flit.module]
 name = "ipyoptimade"
 
 [tool.bumpver]
-current_version = "v1.0.0"
+current_version = "v1.0.0a0"
 version_pattern = "vMAJOR.MINOR.PATCH[PYTAGNUM]"
 commit_message = "Bump version: {old_version} -> {new_version}"
 commit = true
 tag = true
 push = true
 
 [tool.bumpver.file_patterns]
```

### Comparing `ipyoptimade-1.0.0/src/ipyoptimade/__init__.py` & `ipyoptimade-1.0.0a0/src/ipyoptimade/__init__.py`

 * *Files identical despite different names*

### Comparing `ipyoptimade-1.0.0/src/ipyoptimade/default_parameters.py` & `ipyoptimade-1.0.0a0/src/ipyoptimade/default_parameters.py`

 * *Files identical despite different names*

### Comparing `ipyoptimade-1.0.0/src/ipyoptimade/exceptions.py` & `ipyoptimade-1.0.0a0/src/ipyoptimade/exceptions.py`

 * *Files identical despite different names*

### Comparing `ipyoptimade-1.0.0/src/ipyoptimade/informational.py` & `ipyoptimade-1.0.0a0/src/ipyoptimade/informational.py`

 * *Files identical despite different names*

### Comparing `ipyoptimade-1.0.0/src/ipyoptimade/logger.py` & `ipyoptimade-1.0.0a0/src/ipyoptimade/logger.py`

 * *Files identical despite different names*

### Comparing `ipyoptimade-1.0.0/src/ipyoptimade/query_filter.py` & `ipyoptimade-1.0.0a0/src/ipyoptimade/query_filter.py`

 * *Files identical despite different names*

### Comparing `ipyoptimade-1.0.0/src/ipyoptimade/query_provider.py` & `ipyoptimade-1.0.0a0/src/ipyoptimade/query_provider.py`

 * *Files identical despite different names*

### Comparing `ipyoptimade-1.0.0/src/ipyoptimade/statics/optimade-text-right-transparent-bg.png` & `ipyoptimade-1.0.0a0/src/ipyoptimade/statics/optimade-text-right-transparent-bg.png`

 * *Files identical despite different names*

### Comparing `ipyoptimade-1.0.0/src/ipyoptimade/subwidgets/__init__.py` & `ipyoptimade-1.0.0a0/src/ipyoptimade/subwidgets/__init__.py`

 * *Files identical despite different names*

### Comparing `ipyoptimade-1.0.0/src/ipyoptimade/subwidgets/filter_inputs.py` & `ipyoptimade-1.0.0a0/src/ipyoptimade/subwidgets/filter_inputs.py`

 * *Files identical despite different names*

### Comparing `ipyoptimade-1.0.0/src/ipyoptimade/subwidgets/multi_checkbox.py` & `ipyoptimade-1.0.0a0/src/ipyoptimade/subwidgets/multi_checkbox.py`

 * *Files identical despite different names*

### Comparing `ipyoptimade-1.0.0/src/ipyoptimade/subwidgets/output_summary.py` & `ipyoptimade-1.0.0a0/src/ipyoptimade/subwidgets/output_summary.py`

 * *Files identical despite different names*

### Comparing `ipyoptimade-1.0.0/src/ipyoptimade/subwidgets/periodic_table.py` & `ipyoptimade-1.0.0a0/src/ipyoptimade/subwidgets/periodic_table.py`

 * *Files identical despite different names*

### Comparing `ipyoptimade-1.0.0/src/ipyoptimade/subwidgets/provider_database.py` & `ipyoptimade-1.0.0a0/src/ipyoptimade/subwidgets/provider_database.py`

 * *Files identical despite different names*

### Comparing `ipyoptimade-1.0.0/src/ipyoptimade/subwidgets/results.py` & `ipyoptimade-1.0.0a0/src/ipyoptimade/subwidgets/results.py`

 * *Files identical despite different names*

### Comparing `ipyoptimade-1.0.0/src/ipyoptimade/subwidgets/sort_selector.py` & `ipyoptimade-1.0.0a0/src/ipyoptimade/subwidgets/sort_selector.py`

 * *Files identical despite different names*

### Comparing `ipyoptimade-1.0.0/src/ipyoptimade/summary.py` & `ipyoptimade-1.0.0a0/src/ipyoptimade/summary.py`

 * *Files identical despite different names*

### Comparing `ipyoptimade-1.0.0/src/ipyoptimade/utils.py` & `ipyoptimade-1.0.0a0/src/ipyoptimade/utils.py`

 * *Files identical despite different names*

### Comparing `ipyoptimade-1.0.0/src/ipyoptimade/warnings.py` & `ipyoptimade-1.0.0a0/src/ipyoptimade/warnings.py`

 * *Files identical despite different names*

### Comparing `ipyoptimade-1.0.0/PKG-INFO` & `ipyoptimade-1.0.0a0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ipyoptimade
-Version: 1.0.0
+Version: 1.0.0a0
 Summary: Jupyter client for searching structures through OPTIMADE API
 Author-email: Casper Welzel Andersen <casper+github@welzel.nu>, Kristjan Eimre <kristan.eimre@epfl.ch>, Jusong Yu <jusong.yu@psi.ch>
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: AiiDA
 Classifier: Framework :: Jupyter
@@ -21,28 +21,27 @@
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Chemistry
 Classifier: Topic :: Scientific/Engineering :: Physics
 Classifier: Topic :: Software Development :: Widget Sets
 Requires-Dist: appdirs~=1.4.4
 Requires-Dist: cachecontrol[filecache]~=0.13.1
 Requires-Dist: ipywidgets~=8.1
-Requires-Dist: nglview~=3.0.8
+Requires-Dist: nglview~=3.0
 Requires-Dist: optimade~=1.0.0
 Requires-Dist: ase~=3.22
 Requires-Dist: pandas~=2.1
 Requires-Dist: requests~=2.31
 Requires-Dist: widget_periodictable~=4.1
 Requires-Dist: semver~=3.0
 Requires-Dist: pre-commit~=3.6 ; extra == "dev"
 Requires-Dist: pytest~=7.4 ; extra == "dev"
 Requires-Dist: pytest-cov~=4.1 ; extra == "dev"
 Requires-Dist: bumpver>=2023.1129 ; extra == "dev"
 Requires-Dist: pip-tools~=7.4 ; extra == "dev"
-Requires-Dist: jupyterlab~=4.0 ; extra == "dev"
-Requires-Dist: voila~=0.4.0 ; extra == "voila"
+Requires-Dist: voila~=0.5.0 ; extra == "voila"
 Project-URL: Documentation, https://github.com/aiidalab/ipyoptimade#readme
 Project-URL: Source, https://github.com/aiidalab/ipyoptimade
 Project-URL: Tracker, https://github.com/aiidalab/ipyoptimade/issues
 Provides-Extra: dev
 Provides-Extra: voila
 
 # OPTIMADE Jupyter widgets and Voilà application
@@ -182,20 +181,14 @@
 
 ```
 export ipyoptimade_DEBUG=1
 ```
 
 to automatically open and show the debug & error messages in the `OptimadeLog()` widget.
 
-Test voila with
-
-```bash
-voila optimade-client.ipynb
-```
-
 ### Making a new release
 
 To create a new release, clone the repository, install development dependencies with `pip install -e '.[dev]'`, and then execute `bumpver update [--major|--minor|--patch] [--tag-num --tag [alpha|beta|rc]]`.
 This will:
 
 1. Create a tagged release with bumped version and push it to the repository.
 2. Trigger a GitHub actions workflow that creates a GitHub release and publishes it on PyPI.
```

