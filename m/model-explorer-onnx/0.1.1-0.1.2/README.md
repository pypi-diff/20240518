# Comparing `tmp/model_explorer_onnx-0.1.1.tar.gz` & `tmp/model_explorer_onnx-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "model_explorer_onnx-0.1.1.tar", last modified: Fri May 17 17:21:07 2024, max compression
+gzip compressed data, was "model_explorer_onnx-0.1.2.tar", last modified: Fri May 17 22:23:58 2024, max compression
```

## Comparing `model_explorer_onnx-0.1.1.tar` & `model_explorer_onnx-0.1.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 justinc    (501) staff       (20)        0 2024-05-17 17:21:07.626413 model_explorer_onnx-0.1.1/
--rw-r--r--   0 justinc    (501) staff       (20)     1067 2024-05-17 15:12:03.000000 model_explorer_onnx-0.1.1/LICENSE
--rw-r--r--   0 justinc    (501) staff       (20)     2671 2024-05-17 17:21:07.626065 model_explorer_onnx-0.1.1/PKG-INFO
--rw-r--r--   0 justinc    (501) staff       (20)      508 2024-05-17 17:19:54.000000 model_explorer_onnx-0.1.1/README.md
--rw-r--r--   0 justinc    (501) staff       (20)      941 2024-05-17 17:20:51.000000 model_explorer_onnx-0.1.1/pyproject.toml
--rw-r--r--   0 justinc    (501) staff       (20)       38 2024-05-17 17:21:07.626488 model_explorer_onnx-0.1.1/setup.cfg
-drwxr-xr-x   0 justinc    (501) staff       (20)        0 2024-05-17 17:21:07.618393 model_explorer_onnx-0.1.1/src/
-drwxr-xr-x   0 justinc    (501) staff       (20)        0 2024-05-17 17:21:07.619169 model_explorer_onnx-0.1.1/src/model_explorer_onnx/
--rw-r--r--   0 justinc    (501) staff       (20)     9257 2024-05-17 17:20:00.000000 model_explorer_onnx-0.1.1/src/model_explorer_onnx/main.py
-drwxr-xr-x   0 justinc    (501) staff       (20)        0 2024-05-17 17:21:07.625625 model_explorer_onnx-0.1.1/src/model_explorer_onnx.egg-info/
--rw-r--r--   0 justinc    (501) staff       (20)     2671 2024-05-17 17:21:07.000000 model_explorer_onnx-0.1.1/src/model_explorer_onnx.egg-info/PKG-INFO
--rw-r--r--   0 justinc    (501) staff       (20)      298 2024-05-17 17:21:07.000000 model_explorer_onnx-0.1.1/src/model_explorer_onnx.egg-info/SOURCES.txt
--rw-r--r--   0 justinc    (501) staff       (20)        1 2024-05-17 17:21:07.000000 model_explorer_onnx-0.1.1/src/model_explorer_onnx.egg-info/dependency_links.txt
--rw-r--r--   0 justinc    (501) staff       (20)       39 2024-05-17 17:21:07.000000 model_explorer_onnx-0.1.1/src/model_explorer_onnx.egg-info/requires.txt
--rw-r--r--   0 justinc    (501) staff       (20)       20 2024-05-17 17:21:07.000000 model_explorer_onnx-0.1.1/src/model_explorer_onnx.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 22:23:58.053470 model_explorer_onnx-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-05-17 22:23:54.000000 model_explorer_onnx-0.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3065 2024-05-17 22:23:58.053470 model_explorer_onnx-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      837 2024-05-17 22:23:54.000000 model_explorer_onnx-0.1.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      986 2024-05-17 22:23:54.000000 model_explorer_onnx-0.1.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-17 22:23:58.053470 model_explorer_onnx-0.1.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 22:23:58.049470 model_explorer_onnx-0.1.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 22:23:58.049470 model_explorer_onnx-0.1.2/src/model_explorer_onnx/
+-rw-r--r--   0 runner    (1001) docker     (127)    13378 2024-05-17 22:23:54.000000 model_explorer_onnx-0.1.2/src/model_explorer_onnx/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 22:23:58.053470 model_explorer_onnx-0.1.2/src/model_explorer_onnx.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3065 2024-05-17 22:23:58.000000 model_explorer_onnx-0.1.2/src/model_explorer_onnx.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      298 2024-05-17 22:23:58.000000 model_explorer_onnx-0.1.2/src/model_explorer_onnx.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-17 22:23:58.000000 model_explorer_onnx-0.1.2/src/model_explorer_onnx.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-05-17 22:23:58.000000 model_explorer_onnx-0.1.2/src/model_explorer_onnx.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-17 22:23:58.000000 model_explorer_onnx-0.1.2/src/model_explorer_onnx.egg-info/top_level.txt
```

### Comparing `model_explorer_onnx-0.1.1/LICENSE` & `model_explorer_onnx-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `model_explorer_onnx-0.1.1/PKG-INFO` & `model_explorer_onnx-0.1.2/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: model-explorer-onnx
-Version: 0.1.1
+Version: 0.1.2
 Summary: Adapter for ai-edge-model-explorer to support ONNX models
 Author-email: Justin Chu <justinchu@microsoft.com>
 License: MIT License
         
         Copyright (c) 2024 Justin Chu
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -37,30 +37,37 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: ai-edge-model-explorer
+Requires-Dist: numpy
 Requires-Dist: onnx
-Requires-Dist: onnxscript
+Requires-Dist: onnxscript>=0.1.0.dev20240517
+Requires-Dist: ml_dtypes
 
-# model-explorer-onnx
-ONNX Adapter for model-explorer
+# Model Explorer ONNX Adapter
+
+[![PyPI - Version](https://img.shields.io/pypi/v/model-explorer-onnx.svg)](https://pypi.org/project/model-explorer-onnx)
+
+ONNX Adapter for [google-ai-edge/model-explorer](https://github.com/google-ai-edge/model-explorer)
 
 ## Installation
 
 ```bash
 pip install --upgrade model-explorer-onnx
 ```
 
 ## Usage
 
 ```bash
-model-explorer model.onnx --extensions=model_explorer_onnx
+model-explorer --extensions=model_explorer_onnx
 ```
 
 ## Screenshots
 
 <img width="1294" alt="image" src="https://github.com/justinchuby/model-explorer-onnx/assets/11205048/ed7e1eee-a693-48bd-811d-b384f784ef9b">
 
 <img width="1291" alt="image" src="https://github.com/justinchuby/model-explorer-onnx/assets/11205048/b266d8e9-9760-4860-a0a7-eda1de31e1a1">
+
+<img width="1285" alt="image" src="https://github.com/justinchuby/model-explorer-onnx/assets/11205048/b772aa13-4cc3-4034-a729-f134fa3cf818">
```

### Comparing `model_explorer_onnx-0.1.1/pyproject.toml` & `model_explorer_onnx-0.1.2/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "model-explorer-onnx"
-version = "0.1.1"
+version = "0.1.2"
 description = "Adapter for ai-edge-model-explorer to support ONNX models"
 authors = [{ name = "Justin Chu", email = "justinchu@microsoft.com" }]
 readme = "README.md"
 requires-python = ">=3.8"
 license = { file = "LICENSE" }
 classifiers = [
   "Development Status :: 3 - Alpha",
@@ -23,10 +23,12 @@
   "Programming Language :: Python :: 3.11",
   "Programming Language :: Python :: 3.12",
   "License :: OSI Approved :: MIT License",
 ]
 
 dependencies = [
   "ai-edge-model-explorer",
+  "numpy",
   "onnx",
-  "onnxscript",
+  "onnxscript>=0.1.0.dev20240517",
+  "ml_dtypes",
 ]
```

### Comparing `model_explorer_onnx-0.1.1/src/model_explorer_onnx.egg-info/PKG-INFO` & `model_explorer_onnx-0.1.2/src/model_explorer_onnx.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: model-explorer-onnx
-Version: 0.1.1
+Version: 0.1.2
 Summary: Adapter for ai-edge-model-explorer to support ONNX models
 Author-email: Justin Chu <justinchu@microsoft.com>
 License: MIT License
         
         Copyright (c) 2024 Justin Chu
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -37,30 +37,37 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: ai-edge-model-explorer
+Requires-Dist: numpy
 Requires-Dist: onnx
-Requires-Dist: onnxscript
+Requires-Dist: onnxscript>=0.1.0.dev20240517
+Requires-Dist: ml_dtypes
 
-# model-explorer-onnx
-ONNX Adapter for model-explorer
+# Model Explorer ONNX Adapter
+
+[![PyPI - Version](https://img.shields.io/pypi/v/model-explorer-onnx.svg)](https://pypi.org/project/model-explorer-onnx)
+
+ONNX Adapter for [google-ai-edge/model-explorer](https://github.com/google-ai-edge/model-explorer)
 
 ## Installation
 
 ```bash
 pip install --upgrade model-explorer-onnx
 ```
 
 ## Usage
 
 ```bash
-model-explorer model.onnx --extensions=model_explorer_onnx
+model-explorer --extensions=model_explorer_onnx
 ```
 
 ## Screenshots
 
 <img width="1294" alt="image" src="https://github.com/justinchuby/model-explorer-onnx/assets/11205048/ed7e1eee-a693-48bd-811d-b384f784ef9b">
 
 <img width="1291" alt="image" src="https://github.com/justinchuby/model-explorer-onnx/assets/11205048/b266d8e9-9760-4860-a0a7-eda1de31e1a1">
+
+<img width="1285" alt="image" src="https://github.com/justinchuby/model-explorer-onnx/assets/11205048/b772aa13-4cc3-4034-a729-f134fa3cf818">
```

