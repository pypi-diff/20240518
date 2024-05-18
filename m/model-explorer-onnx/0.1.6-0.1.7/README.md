# Comparing `tmp/model_explorer_onnx-0.1.6.tar.gz` & `tmp/model_explorer_onnx-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "model_explorer_onnx-0.1.6.tar", last modified: Sat May 18 15:52:50 2024, max compression
+gzip compressed data, was "model_explorer_onnx-0.1.7.tar", last modified: Sat May 18 16:41:25 2024, max compression
```

## Comparing `model_explorer_onnx-0.1.6.tar` & `model_explorer_onnx-0.1.7.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 15:52:50.639682 model_explorer_onnx-0.1.6/
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-05-18 15:52:47.000000 model_explorer_onnx-0.1.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3568 2024-05-18 15:52:50.639682 model_explorer_onnx-0.1.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1264 2024-05-18 15:52:47.000000 model_explorer_onnx-0.1.6/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-05-18 15:52:47.000000 model_explorer_onnx-0.1.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-18 15:52:50.639682 model_explorer_onnx-0.1.6/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 15:52:50.639682 model_explorer_onnx-0.1.6/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 15:52:50.639682 model_explorer_onnx-0.1.6/src/model_explorer_onnx/
--rw-r--r--   0 runner    (1001) docker     (127)    18823 2024-05-18 15:52:47.000000 model_explorer_onnx-0.1.6/src/model_explorer_onnx/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 15:52:50.639682 model_explorer_onnx-0.1.6/src/model_explorer_onnx.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3568 2024-05-18 15:52:50.000000 model_explorer_onnx-0.1.6/src/model_explorer_onnx.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      298 2024-05-18 15:52:50.000000 model_explorer_onnx-0.1.6/src/model_explorer_onnx.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-18 15:52:50.000000 model_explorer_onnx-0.1.6/src/model_explorer_onnx.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-05-18 15:52:50.000000 model_explorer_onnx-0.1.6/src/model_explorer_onnx.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-18 15:52:50.000000 model_explorer_onnx-0.1.6/src/model_explorer_onnx.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 16:41:25.833750 model_explorer_onnx-0.1.7/
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-05-18 16:41:22.000000 model_explorer_onnx-0.1.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3568 2024-05-18 16:41:25.829749 model_explorer_onnx-0.1.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1264 2024-05-18 16:41:22.000000 model_explorer_onnx-0.1.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-05-18 16:41:22.000000 model_explorer_onnx-0.1.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-18 16:41:25.833750 model_explorer_onnx-0.1.7/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 16:41:25.829749 model_explorer_onnx-0.1.7/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 16:41:25.829749 model_explorer_onnx-0.1.7/src/model_explorer_onnx/
+-rw-r--r--   0 runner    (1001) docker     (127)    18673 2024-05-18 16:41:22.000000 model_explorer_onnx-0.1.7/src/model_explorer_onnx/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 16:41:25.829749 model_explorer_onnx-0.1.7/src/model_explorer_onnx.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3568 2024-05-18 16:41:25.000000 model_explorer_onnx-0.1.7/src/model_explorer_onnx.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      298 2024-05-18 16:41:25.000000 model_explorer_onnx-0.1.7/src/model_explorer_onnx.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-18 16:41:25.000000 model_explorer_onnx-0.1.7/src/model_explorer_onnx.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-05-18 16:41:25.000000 model_explorer_onnx-0.1.7/src/model_explorer_onnx.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-18 16:41:25.000000 model_explorer_onnx-0.1.7/src/model_explorer_onnx.egg-info/top_level.txt
```

### Comparing `model_explorer_onnx-0.1.6/LICENSE` & `model_explorer_onnx-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `model_explorer_onnx-0.1.6/PKG-INFO` & `model_explorer_onnx-0.1.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: model-explorer-onnx
-Version: 0.1.6
+Version: 0.1.7
 Summary: Adapter for ai-edge-model-explorer to support ONNX models
 Author-email: Justin Chu <justinchu@microsoft.com>
 License: MIT License
         
         Copyright (c) 2024 Justin Chu
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `model_explorer_onnx-0.1.6/README.md` & `model_explorer_onnx-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `model_explorer_onnx-0.1.6/pyproject.toml` & `model_explorer_onnx-0.1.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "model-explorer-onnx"
-version = "0.1.6"
+version = "0.1.7"
 description = "Adapter for ai-edge-model-explorer to support ONNX models"
 authors = [{ name = "Justin Chu", email = "justinchu@microsoft.com" }]
 readme = "README.md"
 requires-python = ">=3.8"
 license = { file = "LICENSE" }
 classifiers = [
   "Development Status :: 3 - Alpha",
```

### Comparing `model_explorer_onnx-0.1.6/src/model_explorer_onnx/main.py` & `model_explorer_onnx-0.1.7/src/model_explorer_onnx/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -301,15 +301,14 @@
                 )
             )
         if type_ == "Input":
             metadata = graph_builder.MetadataItem(id="0", attrs=[])
             set_attr(metadata, "__tensor_tag", value.name or "")
             set_type_shape_metadata(metadata, value)
             node.outputsMetadata.append(metadata)
-        set_attr(node, "category", type_)
         set_attr(node, "name", value.name or "")
         set_attr(node, "index", str(i))
         graph.nodes.append(node)
         # Record nodes for quick lookup
         all_nodes[node.id] = node
 
 
@@ -375,16 +374,14 @@
             set_attr(metadata, "value", display_tensor(initializer.const_value))
             continue
         node = graph_builder.GraphNode(
             id=initializer_node_name,
             label="Initializer",
             namespace=get_initializer_namespace(initializer, namespace),
         )
-        # Annotate the initializer node as an initializer
-        set_attr(node, "category", "Initializer")
         # Add metadata for the output tensor
         if initializer.const_value is None:
             logger.warning(
                 "Initializer %s does not have a const value. Skipping.", initializer
             )
             graph.nodes.append(node)
             continue
```

### Comparing `model_explorer_onnx-0.1.6/src/model_explorer_onnx.egg-info/PKG-INFO` & `model_explorer_onnx-0.1.7/src/model_explorer_onnx.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: model-explorer-onnx
-Version: 0.1.6
+Version: 0.1.7
 Summary: Adapter for ai-edge-model-explorer to support ONNX models
 Author-email: Justin Chu <justinchu@microsoft.com>
 License: MIT License
         
         Copyright (c) 2024 Justin Chu
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

