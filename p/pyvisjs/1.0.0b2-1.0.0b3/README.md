# Comparing `tmp/pyvisjs-1.0.0b2.tar.gz` & `tmp/pyvisjs-1.0.0b3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyvisjs-1.0.0b2.tar", last modified: Fri May 17 09:42:44 2024, max compression
+gzip compressed data, was "pyvisjs-1.0.0b3.tar", last modified: Fri May 17 19:45:58 2024, max compression
```

## Comparing `pyvisjs-1.0.0b2.tar` & `pyvisjs-1.0.0b3.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 09:42:44.515450 pyvisjs-1.0.0b2/
--rw-rw-rw-   0 root         (0) root         (0)     1396 2024-05-17 09:42:28.000000 pyvisjs-1.0.0b2/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)      979 2024-05-17 09:42:28.000000 pyvisjs-1.0.0b2/.gitlab-ci.yml
--rw-rw-rw-   0 root         (0) root         (0)     4169 2024-05-17 09:42:28.000000 pyvisjs-1.0.0b2/CONTRIBUTING.md
--rw-rw-rw-   0 root         (0) root         (0)     1091 2024-05-17 09:42:28.000000 pyvisjs-1.0.0b2/LICENSE
--rw-r--r--   0 root         (0) root         (0)     3331 2024-05-17 09:42:44.515450 pyvisjs-1.0.0b2/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1404 2024-05-17 09:42:28.000000 pyvisjs-1.0.0b2/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 09:42:44.508450 pyvisjs-1.0.0b2/examples/
--rw-rw-rw-   0 root         (0) root         (0)     8970 2024-05-17 09:42:28.000000 pyvisjs-1.0.0b2/examples/bluor.py
--rw-rw-rw-   0 root         (0) root         (0)      481 2024-05-17 09:42:28.000000 pyvisjs-1.0.0b2/examples/readme.py
--rw-rw-rw-   0 root         (0) root         (0)      959 2024-05-17 09:42:28.000000 pyvisjs-1.0.0b2/folder_structure.txt
--rw-rw-rw-   0 root         (0) root         (0)      890 2024-05-17 09:42:28.000000 pyvisjs-1.0.0b2/pyproject.toml
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 09:42:44.509450 pyvisjs-1.0.0b2/pyvisjs/
--rw-rw-rw-   0 root         (0) root         (0)      103 2024-05-17 09:42:28.000000 pyvisjs-1.0.0b2/pyvisjs/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      103 2024-05-17 09:42:28.000000 pyvisjs-1.0.0b2/pyvisjs/_version.py
--rw-rw-rw-   0 root         (0) root         (0)     2018 2024-05-17 09:42:28.000000 pyvisjs-1.0.0b2/pyvisjs/base_dictable.py
--rw-rw-rw-   0 root         (0) root         (0)     1274 2024-05-17 09:42:28.000000 pyvisjs-1.0.0b2/pyvisjs/edge.py
--rw-rw-rw-   0 root         (0) root         (0)    10718 2024-05-17 09:42:28.000000 pyvisjs-1.0.0b2/pyvisjs/network.py
--rw-rw-rw-   0 root         (0) root         (0)      590 2024-05-17 09:42:28.000000 pyvisjs-1.0.0b2/pyvisjs/node.py
--rw-rw-rw-   0 root         (0) root         (0)    13394 2024-05-17 09:42:28.000000 pyvisjs-1.0.0b2/pyvisjs/options.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 09:42:44.512450 pyvisjs-1.0.0b2/pyvisjs/templates/
--rw-rw-rw-   0 root         (0) root         (0)      966 2024-05-17 09:42:28.000000 pyvisjs-1.0.0b2/pyvisjs/templates/base.html
--rw-rw-rw-   0 root         (0) root         (0)      153 2024-05-17 09:42:28.000000 pyvisjs-1.0.0b2/pyvisjs/templates/basic.html
--rw-rw-rw-   0 root         (0) root         (0)     1193 2024-05-17 09:42:28.000000 pyvisjs-1.0.0b2/pyvisjs/templates/bs-container.html
--rw-rw-rw-   0 root         (0) root         (0)     1058 2024-05-17 09:42:28.000000 pyvisjs-1.0.0b2/pyvisjs/templates/create_network.js
--rw-rw-rw-   0 root         (0) root         (0)      926 2024-05-17 09:42:28.000000 pyvisjs-1.0.0b2/pyvisjs/templates/draw_title.js
--rw-rw-rw-   0 root         (0) root         (0)     7594 2024-05-17 09:42:28.000000 pyvisjs-1.0.0b2/pyvisjs/templates/functions.js
--rw-rw-rw-   0 root         (0) root         (0)      516 2024-05-17 09:42:28.000000 pyvisjs-1.0.0b2/pyvisjs/templates/init_tomSelect.js
--rw-rw-rw-   0 root         (0) root         (0)      840 2024-05-17 09:42:28.000000 pyvisjs-1.0.0b2/pyvisjs/templates/select-edge-filter.html
--rw-rw-rw-   0 root         (0) root         (0)     1704 2024-05-17 09:42:28.000000 pyvisjs-1.0.0b2/pyvisjs/templates/tom-select.html
--rw-rw-rw-   0 root         (0) root         (0)     1051 2024-05-17 09:42:28.000000 pyvisjs-1.0.0b2/pyvisjs/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 09:42:44.514450 pyvisjs-1.0.0b2/pyvisjs.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3331 2024-05-17 09:42:44.000000 pyvisjs-1.0.0b2/pyvisjs.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      907 2024-05-17 09:42:44.000000 pyvisjs-1.0.0b2/pyvisjs.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-17 09:42:44.000000 pyvisjs-1.0.0b2/pyvisjs.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       43 2024-05-17 09:42:44.000000 pyvisjs-1.0.0b2/pyvisjs.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       28 2024-05-17 09:42:44.000000 pyvisjs-1.0.0b2/pyvisjs.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      109 2024-05-17 09:42:28.000000 pyvisjs-1.0.0b2/requirements.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-05-17 09:42:44.515450 pyvisjs-1.0.0b2/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 09:42:44.514450 pyvisjs-1.0.0b2/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-17 09:42:28.000000 pyvisjs-1.0.0b2/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1921 2024-05-17 09:42:28.000000 pyvisjs-1.0.0b2/tests/test_base_dictable.py
--rw-rw-rw-   0 root         (0) root         (0)     1006 2024-05-17 09:42:28.000000 pyvisjs-1.0.0b2/tests/test_edge.py
--rw-rw-rw-   0 root         (0) root         (0)    11958 2024-05-17 09:42:28.000000 pyvisjs-1.0.0b2/tests/test_network.py
--rw-rw-rw-   0 root         (0) root         (0)     2399 2024-05-17 09:42:28.000000 pyvisjs-1.0.0b2/tests/test_node.py
--rw-rw-rw-   0 root         (0) root         (0)     3863 2024-05-17 09:42:28.000000 pyvisjs-1.0.0b2/tests/test_options.py
--rw-rw-rw-   0 root         (0) root         (0)     2561 2024-05-17 09:42:28.000000 pyvisjs-1.0.0b2/tests/test_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 19:45:58.830309 pyvisjs-1.0.0b3/
+-rw-rw-rw-   0 root         (0) root         (0)     1396 2024-05-17 19:45:42.000000 pyvisjs-1.0.0b3/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)     1578 2024-05-17 19:45:42.000000 pyvisjs-1.0.0b3/.gitlab-ci.yml
+-rw-rw-rw-   0 root         (0) root         (0)     5120 2024-05-17 19:45:42.000000 pyvisjs-1.0.0b3/CONTRIBUTING.md
+-rw-rw-rw-   0 root         (0) root         (0)     1091 2024-05-17 19:45:42.000000 pyvisjs-1.0.0b3/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     3331 2024-05-17 19:45:58.830309 pyvisjs-1.0.0b3/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1404 2024-05-17 19:45:42.000000 pyvisjs-1.0.0b3/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 19:45:58.823309 pyvisjs-1.0.0b3/examples/
+-rw-rw-rw-   0 root         (0) root         (0)     8970 2024-05-17 19:45:42.000000 pyvisjs-1.0.0b3/examples/bluor.py
+-rw-rw-rw-   0 root         (0) root         (0)      481 2024-05-17 19:45:42.000000 pyvisjs-1.0.0b3/examples/readme.py
+-rw-rw-rw-   0 root         (0) root         (0)      959 2024-05-17 19:45:42.000000 pyvisjs-1.0.0b3/folder_structure.txt
+-rw-rw-rw-   0 root         (0) root         (0)      890 2024-05-17 19:45:42.000000 pyvisjs-1.0.0b3/pyproject.toml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 19:45:58.825309 pyvisjs-1.0.0b3/pyvisjs/
+-rw-rw-rw-   0 root         (0) root         (0)      103 2024-05-17 19:45:42.000000 pyvisjs-1.0.0b3/pyvisjs/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      103 2024-05-17 19:45:42.000000 pyvisjs-1.0.0b3/pyvisjs/_version.py
+-rw-rw-rw-   0 root         (0) root         (0)     2018 2024-05-17 19:45:42.000000 pyvisjs-1.0.0b3/pyvisjs/base_dictable.py
+-rw-rw-rw-   0 root         (0) root         (0)     1274 2024-05-17 19:45:42.000000 pyvisjs-1.0.0b3/pyvisjs/edge.py
+-rw-rw-rw-   0 root         (0) root         (0)    10718 2024-05-17 19:45:42.000000 pyvisjs-1.0.0b3/pyvisjs/network.py
+-rw-rw-rw-   0 root         (0) root         (0)      590 2024-05-17 19:45:42.000000 pyvisjs-1.0.0b3/pyvisjs/node.py
+-rw-rw-rw-   0 root         (0) root         (0)    13394 2024-05-17 19:45:42.000000 pyvisjs-1.0.0b3/pyvisjs/options.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 19:45:58.828309 pyvisjs-1.0.0b3/pyvisjs/templates/
+-rw-rw-rw-   0 root         (0) root         (0)      966 2024-05-17 19:45:42.000000 pyvisjs-1.0.0b3/pyvisjs/templates/base.html
+-rw-rw-rw-   0 root         (0) root         (0)      153 2024-05-17 19:45:42.000000 pyvisjs-1.0.0b3/pyvisjs/templates/basic.html
+-rw-rw-rw-   0 root         (0) root         (0)     1193 2024-05-17 19:45:42.000000 pyvisjs-1.0.0b3/pyvisjs/templates/bs-container.html
+-rw-rw-rw-   0 root         (0) root         (0)     1058 2024-05-17 19:45:42.000000 pyvisjs-1.0.0b3/pyvisjs/templates/create_network.js
+-rw-rw-rw-   0 root         (0) root         (0)      926 2024-05-17 19:45:42.000000 pyvisjs-1.0.0b3/pyvisjs/templates/draw_title.js
+-rw-rw-rw-   0 root         (0) root         (0)     7594 2024-05-17 19:45:42.000000 pyvisjs-1.0.0b3/pyvisjs/templates/functions.js
+-rw-rw-rw-   0 root         (0) root         (0)      516 2024-05-17 19:45:42.000000 pyvisjs-1.0.0b3/pyvisjs/templates/init_tomSelect.js
+-rw-rw-rw-   0 root         (0) root         (0)      840 2024-05-17 19:45:42.000000 pyvisjs-1.0.0b3/pyvisjs/templates/select-edge-filter.html
+-rw-rw-rw-   0 root         (0) root         (0)     1704 2024-05-17 19:45:42.000000 pyvisjs-1.0.0b3/pyvisjs/templates/tom-select.html
+-rw-rw-rw-   0 root         (0) root         (0)     1051 2024-05-17 19:45:42.000000 pyvisjs-1.0.0b3/pyvisjs/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 19:45:58.829309 pyvisjs-1.0.0b3/pyvisjs.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3331 2024-05-17 19:45:58.000000 pyvisjs-1.0.0b3/pyvisjs.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      907 2024-05-17 19:45:58.000000 pyvisjs-1.0.0b3/pyvisjs.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-17 19:45:58.000000 pyvisjs-1.0.0b3/pyvisjs.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       43 2024-05-17 19:45:58.000000 pyvisjs-1.0.0b3/pyvisjs.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       28 2024-05-17 19:45:58.000000 pyvisjs-1.0.0b3/pyvisjs.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      109 2024-05-17 19:45:42.000000 pyvisjs-1.0.0b3/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-17 19:45:58.830309 pyvisjs-1.0.0b3/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 19:45:58.829309 pyvisjs-1.0.0b3/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-17 19:45:42.000000 pyvisjs-1.0.0b3/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1921 2024-05-17 19:45:42.000000 pyvisjs-1.0.0b3/tests/test_base_dictable.py
+-rw-rw-rw-   0 root         (0) root         (0)     1006 2024-05-17 19:45:42.000000 pyvisjs-1.0.0b3/tests/test_edge.py
+-rw-rw-rw-   0 root         (0) root         (0)    11958 2024-05-17 19:45:42.000000 pyvisjs-1.0.0b3/tests/test_network.py
+-rw-rw-rw-   0 root         (0) root         (0)     2399 2024-05-17 19:45:42.000000 pyvisjs-1.0.0b3/tests/test_node.py
+-rw-rw-rw-   0 root         (0) root         (0)     3863 2024-05-17 19:45:42.000000 pyvisjs-1.0.0b3/tests/test_options.py
+-rw-rw-rw-   0 root         (0) root         (0)     2561 2024-05-17 19:45:42.000000 pyvisjs-1.0.0b3/tests/test_utils.py
```

### Comparing `pyvisjs-1.0.0b2/.gitignore` & `pyvisjs-1.0.0b3/.gitignore`

 * *Files identical despite different names*

### Comparing `pyvisjs-1.0.0b2/CONTRIBUTING.md` & `pyvisjs-1.0.0b3/CONTRIBUTING.md`

 * *Files 18% similar despite different names*

```diff
@@ -77,14 +77,35 @@
 git add .
 git commit -m "Fixes issue #12"
 git push origin feature-name
 << create a Pull Request >>
 
 ```
 
+## Branching Strategy
+```main```:
+
+- **Purpose**: This branch holds the production-released code.
+- **Protection**: Set as a protected branch to prevent direct commits. Only allow merge requests (MRs) from ```dev``` after code reviews and CI checks.
+- **Deployment**: Deployments to production are triggered from this branch.
+
+```dev```:
+
+- **Purpose**: This branch holds the current or in-progress code.
+- **Protection**: Also set as a protected branch to prevent direct commits. Similar to the ```main``` branch, only allow MRs.
+- **Integration**: Regularly integrated from ```feature-branches``` to keep it up-to-date with the latest changes.
+
+
+```feature-branches```:
+
+ - **Purpose**: For developing new features, bug fixes, or any changes.
+- **Naming Convention**: Use a consistent naming convention like feature-name or bug-description.
+- **Lifecycle**: These branches are short-lived and should be merged back into ```dev``` upon completion.
+
+
 ## Community Guidelines
 
 We value a respectful and inclusive community. Please adhere to the following guidelines when interacting with others in the pyvisjs community:
 
 - Be respectful and considerate of others' opinions and contributions.
 - Avoid offensive language, harassment, or discrimination of any kind.
 - Help create a welcoming and inclusive environment for all community members.
```

### Comparing `pyvisjs-1.0.0b2/LICENSE` & `pyvisjs-1.0.0b3/LICENSE`

 * *Files identical despite different names*

### Comparing `pyvisjs-1.0.0b2/PKG-INFO` & `pyvisjs-1.0.0b3/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyvisjs
-Version: 1.0.0b2
+Version: 1.0.0b3
 Summary: A Python wrapper for vis.js Network
 Author-email: Andrey Morozov <andrey@morozov.lv>
 License: MIT License
         
         Copyright (c) 2024 Andrey Morozov (andrey@morozov.lv)
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `pyvisjs-1.0.0b2/README.md` & `pyvisjs-1.0.0b3/README.md`

 * *Files identical despite different names*

### Comparing `pyvisjs-1.0.0b2/examples/bluor.py` & `pyvisjs-1.0.0b3/examples/bluor.py`

 * *Files 0% similar despite different names*

```diff
@@ -78,15 +78,15 @@
 
     return (color, shape, size, second_line)
 
 ####################
 try_gummy = True  
 ####################
 springConstant = (0.05 if try_gummy else 0)
-damping = (0.05 if try_gummy else 0)
+damping = (0.05 if try_gummy else 1)
 
 options = Options("800px", "1300px")
 options \
     .set_configure(enabled=False) \
     .set_interaction(dragNodes=True, hideEdgesOnDrag=False, hideNodesOnDrag=False)
 options.nodes \
     .set_font(face="JetBrains Mono")
```

### Comparing `pyvisjs-1.0.0b2/folder_structure.txt` & `pyvisjs-1.0.0b3/folder_structure.txt`

 * *Files identical despite different names*

### Comparing `pyvisjs-1.0.0b2/pyproject.toml` & `pyvisjs-1.0.0b3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pyvisjs-1.0.0b2/pyvisjs/base_dictable.py` & `pyvisjs-1.0.0b3/pyvisjs/base_dictable.py`

 * *Files identical despite different names*

### Comparing `pyvisjs-1.0.0b2/pyvisjs/edge.py` & `pyvisjs-1.0.0b3/pyvisjs/edge.py`

 * *Files identical despite different names*

### Comparing `pyvisjs-1.0.0b2/pyvisjs/network.py` & `pyvisjs-1.0.0b3/pyvisjs/network.py`

 * *Files identical despite different names*

### Comparing `pyvisjs-1.0.0b2/pyvisjs/node.py` & `pyvisjs-1.0.0b3/pyvisjs/node.py`

 * *Files identical despite different names*

### Comparing `pyvisjs-1.0.0b2/pyvisjs/options.py` & `pyvisjs-1.0.0b3/pyvisjs/options.py`

 * *Files identical despite different names*

### Comparing `pyvisjs-1.0.0b2/pyvisjs/templates/base.html` & `pyvisjs-1.0.0b3/pyvisjs/templates/base.html`

 * *Files identical despite different names*

### Comparing `pyvisjs-1.0.0b2/pyvisjs/templates/bs-container.html` & `pyvisjs-1.0.0b3/pyvisjs/templates/bs-container.html`

 * *Files identical despite different names*

### Comparing `pyvisjs-1.0.0b2/pyvisjs/templates/create_network.js` & `pyvisjs-1.0.0b3/pyvisjs/templates/create_network.js`

 * *Files identical despite different names*

### Comparing `pyvisjs-1.0.0b2/pyvisjs/templates/draw_title.js` & `pyvisjs-1.0.0b3/pyvisjs/templates/draw_title.js`

 * *Files identical despite different names*

### Comparing `pyvisjs-1.0.0b2/pyvisjs/templates/functions.js` & `pyvisjs-1.0.0b3/pyvisjs/templates/functions.js`

 * *Files identical despite different names*

### Comparing `pyvisjs-1.0.0b2/pyvisjs/templates/init_tomSelect.js` & `pyvisjs-1.0.0b3/pyvisjs/templates/init_tomSelect.js`

 * *Files identical despite different names*

### Comparing `pyvisjs-1.0.0b2/pyvisjs/templates/select-edge-filter.html` & `pyvisjs-1.0.0b3/pyvisjs/templates/select-edge-filter.html`

 * *Files identical despite different names*

### Comparing `pyvisjs-1.0.0b2/pyvisjs/templates/tom-select.html` & `pyvisjs-1.0.0b3/pyvisjs/templates/tom-select.html`

 * *Files identical despite different names*

### Comparing `pyvisjs-1.0.0b2/pyvisjs/utils.py` & `pyvisjs-1.0.0b3/pyvisjs/utils.py`

 * *Files identical despite different names*

### Comparing `pyvisjs-1.0.0b2/pyvisjs.egg-info/PKG-INFO` & `pyvisjs-1.0.0b3/pyvisjs.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyvisjs
-Version: 1.0.0b2
+Version: 1.0.0b3
 Summary: A Python wrapper for vis.js Network
 Author-email: Andrey Morozov <andrey@morozov.lv>
 License: MIT License
         
         Copyright (c) 2024 Andrey Morozov (andrey@morozov.lv)
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `pyvisjs-1.0.0b2/pyvisjs.egg-info/SOURCES.txt` & `pyvisjs-1.0.0b3/pyvisjs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyvisjs-1.0.0b2/tests/test_base_dictable.py` & `pyvisjs-1.0.0b3/tests/test_base_dictable.py`

 * *Files identical despite different names*

### Comparing `pyvisjs-1.0.0b2/tests/test_edge.py` & `pyvisjs-1.0.0b3/tests/test_edge.py`

 * *Files identical despite different names*

### Comparing `pyvisjs-1.0.0b2/tests/test_network.py` & `pyvisjs-1.0.0b3/tests/test_network.py`

 * *Files identical despite different names*

### Comparing `pyvisjs-1.0.0b2/tests/test_node.py` & `pyvisjs-1.0.0b3/tests/test_node.py`

 * *Files identical despite different names*

### Comparing `pyvisjs-1.0.0b2/tests/test_options.py` & `pyvisjs-1.0.0b3/tests/test_options.py`

 * *Files identical despite different names*

### Comparing `pyvisjs-1.0.0b2/tests/test_utils.py` & `pyvisjs-1.0.0b3/tests/test_utils.py`

 * *Files identical despite different names*

