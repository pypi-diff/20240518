# Comparing `tmp/model_explorer_onnx-0.1.4.tar.gz` & `tmp/model_explorer_onnx-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "model_explorer_onnx-0.1.4.tar", last modified: Sat May 18 00:15:03 2024, max compression
+gzip compressed data, was "model_explorer_onnx-0.1.5.tar", last modified: Sat May 18 05:16:12 2024, max compression
```

## Comparing `model_explorer_onnx-0.1.4.tar` & `model_explorer_onnx-0.1.5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 00:15:03.552406 model_explorer_onnx-0.1.4/
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-05-18 00:14:53.000000 model_explorer_onnx-0.1.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3283 2024-05-18 00:15:03.552406 model_explorer_onnx-0.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      979 2024-05-18 00:14:53.000000 model_explorer_onnx-0.1.4/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-05-18 00:14:53.000000 model_explorer_onnx-0.1.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-18 00:15:03.552406 model_explorer_onnx-0.1.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 00:15:03.548406 model_explorer_onnx-0.1.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 00:15:03.548406 model_explorer_onnx-0.1.4/src/model_explorer_onnx/
--rw-r--r--   0 runner    (1001) docker     (127)    16746 2024-05-18 00:14:53.000000 model_explorer_onnx-0.1.4/src/model_explorer_onnx/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 00:15:03.552406 model_explorer_onnx-0.1.4/src/model_explorer_onnx.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3283 2024-05-18 00:15:03.000000 model_explorer_onnx-0.1.4/src/model_explorer_onnx.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      298 2024-05-18 00:15:03.000000 model_explorer_onnx-0.1.4/src/model_explorer_onnx.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-18 00:15:03.000000 model_explorer_onnx-0.1.4/src/model_explorer_onnx.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-05-18 00:15:03.000000 model_explorer_onnx-0.1.4/src/model_explorer_onnx.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-18 00:15:03.000000 model_explorer_onnx-0.1.4/src/model_explorer_onnx.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 05:16:12.612696 model_explorer_onnx-0.1.5/
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-05-18 05:16:08.000000 model_explorer_onnx-0.1.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3283 2024-05-18 05:16:12.612696 model_explorer_onnx-0.1.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      979 2024-05-18 05:16:08.000000 model_explorer_onnx-0.1.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-05-18 05:16:08.000000 model_explorer_onnx-0.1.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-18 05:16:12.612696 model_explorer_onnx-0.1.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 05:16:12.608696 model_explorer_onnx-0.1.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 05:16:12.612696 model_explorer_onnx-0.1.5/src/model_explorer_onnx/
+-rw-r--r--   0 runner    (1001) docker     (127)    16776 2024-05-18 05:16:08.000000 model_explorer_onnx-0.1.5/src/model_explorer_onnx/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 05:16:12.612696 model_explorer_onnx-0.1.5/src/model_explorer_onnx.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3283 2024-05-18 05:16:12.000000 model_explorer_onnx-0.1.5/src/model_explorer_onnx.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      298 2024-05-18 05:16:12.000000 model_explorer_onnx-0.1.5/src/model_explorer_onnx.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-18 05:16:12.000000 model_explorer_onnx-0.1.5/src/model_explorer_onnx.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-05-18 05:16:12.000000 model_explorer_onnx-0.1.5/src/model_explorer_onnx.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-18 05:16:12.000000 model_explorer_onnx-0.1.5/src/model_explorer_onnx.egg-info/top_level.txt
```

### Comparing `model_explorer_onnx-0.1.4/LICENSE` & `model_explorer_onnx-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `model_explorer_onnx-0.1.4/PKG-INFO` & `model_explorer_onnx-0.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: model-explorer-onnx
-Version: 0.1.4
+Version: 0.1.5
 Summary: Adapter for ai-edge-model-explorer to support ONNX models
 Author-email: Justin Chu <justinchu@microsoft.com>
 License: MIT License
         
         Copyright (c) 2024 Justin Chu
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `model_explorer_onnx-0.1.4/README.md` & `model_explorer_onnx-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `model_explorer_onnx-0.1.4/pyproject.toml` & `model_explorer_onnx-0.1.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "model-explorer-onnx"
-version = "0.1.4"
+version = "0.1.5"
 description = "Adapter for ai-edge-model-explorer to support ONNX models"
 authors = [{ name = "Justin Chu", email = "justinchu@microsoft.com" }]
 readme = "README.md"
 requires-python = ">=3.8"
 license = { file = "LICENSE" }
 classifiers = [
   "Development Status :: 3 - Alpha",
```

### Comparing `model_explorer_onnx-0.1.4/src/model_explorer_onnx/main.py` & `model_explorer_onnx-0.1.5/src/model_explorer_onnx/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,23 +20,23 @@
 def display_tensor(tensor: ir.TensorProtocol | None) -> str:
     if tensor is None:
         return "Data not available"
     if tensor.size < _TENSOR_DISPLAY_LIMIT:
         try:
             array = tensor.numpy()
             if tensor.dtype == ir.DataType.BFLOAT16:
-                array.astype(ml_dtypes.bfloat16)
+                array = array.view(ml_dtypes.bfloat16)
             elif tensor.dtype == ir.DataType.FLOAT8E4M3FN:
-                array.astype(ml_dtypes.float8_e4m3fn)
+                array = array.view(ml_dtypes.float8_e4m3fn)
             elif tensor.dtype == ir.DataType.FLOAT8E4M3FNUZ:
-                array.astype(ml_dtypes.float8_e4m3fnuz)
+                array = array.view(ml_dtypes.float8_e4m3fnuz)
             elif tensor.dtype == ir.DataType.FLOAT8E5M2:
-                array.astype(ml_dtypes.float8_e5m2)
+                array = array.view(ml_dtypes.float8_e5m2)
             elif tensor.dtype == ir.DataType.FLOAT8E5M2FNUZ:
-                array.astype(ml_dtypes.float8_e5m2fnuz)
+                array = array.view(ml_dtypes.float8_e5m2fnuz)
             return np.array2string(array, separator=",")
         except Exception as e:
             logger.warning("Failed to display tensor: %s", e)
             return str(tensor)
     return str(tensor)
```

### Comparing `model_explorer_onnx-0.1.4/src/model_explorer_onnx.egg-info/PKG-INFO` & `model_explorer_onnx-0.1.5/src/model_explorer_onnx.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: model-explorer-onnx
-Version: 0.1.4
+Version: 0.1.5
 Summary: Adapter for ai-edge-model-explorer to support ONNX models
 Author-email: Justin Chu <justinchu@microsoft.com>
 License: MIT License
         
         Copyright (c) 2024 Justin Chu
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

