# Comparing `tmp/model_explorer_onnx-0.1.3.tar.gz` & `tmp/model_explorer_onnx-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "model_explorer_onnx-0.1.3.tar", last modified: Fri May 17 23:53:18 2024, max compression
+gzip compressed data, was "model_explorer_onnx-0.1.4.tar", last modified: Sat May 18 00:15:03 2024, max compression
```

## Comparing `model_explorer_onnx-0.1.3.tar` & `model_explorer_onnx-0.1.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 23:53:18.902123 model_explorer_onnx-0.1.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-05-17 23:53:15.000000 model_explorer_onnx-0.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3283 2024-05-17 23:53:18.902123 model_explorer_onnx-0.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      979 2024-05-17 23:53:15.000000 model_explorer_onnx-0.1.3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-05-17 23:53:15.000000 model_explorer_onnx-0.1.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-17 23:53:18.902123 model_explorer_onnx-0.1.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 23:53:18.902123 model_explorer_onnx-0.1.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 23:53:18.902123 model_explorer_onnx-0.1.3/src/model_explorer_onnx/
--rw-r--r--   0 runner    (1001) docker     (127)    16832 2024-05-17 23:53:15.000000 model_explorer_onnx-0.1.3/src/model_explorer_onnx/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 23:53:18.902123 model_explorer_onnx-0.1.3/src/model_explorer_onnx.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3283 2024-05-17 23:53:18.000000 model_explorer_onnx-0.1.3/src/model_explorer_onnx.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      298 2024-05-17 23:53:18.000000 model_explorer_onnx-0.1.3/src/model_explorer_onnx.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-17 23:53:18.000000 model_explorer_onnx-0.1.3/src/model_explorer_onnx.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-05-17 23:53:18.000000 model_explorer_onnx-0.1.3/src/model_explorer_onnx.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-17 23:53:18.000000 model_explorer_onnx-0.1.3/src/model_explorer_onnx.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 00:15:03.552406 model_explorer_onnx-0.1.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-05-18 00:14:53.000000 model_explorer_onnx-0.1.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3283 2024-05-18 00:15:03.552406 model_explorer_onnx-0.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      979 2024-05-18 00:14:53.000000 model_explorer_onnx-0.1.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-05-18 00:14:53.000000 model_explorer_onnx-0.1.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-18 00:15:03.552406 model_explorer_onnx-0.1.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 00:15:03.548406 model_explorer_onnx-0.1.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 00:15:03.548406 model_explorer_onnx-0.1.4/src/model_explorer_onnx/
+-rw-r--r--   0 runner    (1001) docker     (127)    16746 2024-05-18 00:14:53.000000 model_explorer_onnx-0.1.4/src/model_explorer_onnx/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 00:15:03.552406 model_explorer_onnx-0.1.4/src/model_explorer_onnx.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3283 2024-05-18 00:15:03.000000 model_explorer_onnx-0.1.4/src/model_explorer_onnx.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      298 2024-05-18 00:15:03.000000 model_explorer_onnx-0.1.4/src/model_explorer_onnx.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-18 00:15:03.000000 model_explorer_onnx-0.1.4/src/model_explorer_onnx.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-05-18 00:15:03.000000 model_explorer_onnx-0.1.4/src/model_explorer_onnx.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-18 00:15:03.000000 model_explorer_onnx-0.1.4/src/model_explorer_onnx.egg-info/top_level.txt
```

### Comparing `model_explorer_onnx-0.1.3/LICENSE` & `model_explorer_onnx-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `model_explorer_onnx-0.1.3/PKG-INFO` & `model_explorer_onnx-0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: model-explorer-onnx
-Version: 0.1.3
+Version: 0.1.4
 Summary: Adapter for ai-edge-model-explorer to support ONNX models
 Author-email: Justin Chu <justinchu@microsoft.com>
 License: MIT License
         
         Copyright (c) 2024 Justin Chu
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `model_explorer_onnx-0.1.3/README.md` & `model_explorer_onnx-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `model_explorer_onnx-0.1.3/pyproject.toml` & `model_explorer_onnx-0.1.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "model-explorer-onnx"
-version = "0.1.3"
+version = "0.1.4"
 description = "Adapter for ai-edge-model-explorer to support ONNX models"
 authors = [{ name = "Justin Chu", email = "justinchu@microsoft.com" }]
 readme = "README.md"
 requires-python = ">=3.8"
 license = { file = "LICENSE" }
 classifiers = [
   "Development Status :: 3 - Alpha",
```

### Comparing `model_explorer_onnx-0.1.3/src/model_explorer_onnx/main.py` & `model_explorer_onnx-0.1.4/src/model_explorer_onnx/main.py`

 * *Files 7% similar despite different names*

```diff
@@ -210,20 +210,16 @@
             if input_node is None:
                 logger.debug(
                     "Input value %s does not have a producer. Treating as initializer.",
                     input_value,
                 )
                 source_node_id = get_initializer_node_name(input_value)
                 source_node_output_id = "0"
-            elif not input_node.name:
-                logger.debug(
-                    "Node %s does not have a name. Skipping incoming edge.", input_node
-                )
-                continue
             else:
+                assert input_node.name, "Bug: Node name is required"
                 source_node_id = input_node.name
                 source_node_output_id = str(input_value.index())
         assert source_node_id is not None
         node.incomingEdges.append(
             graph_builder.IncomingEdge(
                 sourceNodeId=source_node_id,
                 sourceNodeOutputId=source_node_output_id,
@@ -250,17 +246,15 @@
     Args:
         onnx_node: The ONNX node to convert.
         graph_inputs: The set of graph inputs.
         namespace: The namespace of the node.
         all_function_ids: The set of all function identifiers.
         opset_version: The current ONNX opset version.
     """
-    if onnx_node.name is None:
-        logger.warning("Node does not have a name. Skipping node %s.", onnx_node)
-        return None
+    assert onnx_node.name, "Bug: Node name is required"
 
     embedded_namespace = onnx_node.name.lstrip("/").split("/")[0:-1]
     embedded_namespace = [ns or "<anonymous>" for ns in embedded_namespace]
     if embedded_namespace:
         namespace = namespace + "/" + "/".join(embedded_namespace)
     node = graph_builder.GraphNode(
         id=onnx_node.name,
@@ -284,15 +278,16 @@
 ):
     for value in input_or_outputs:
         node = graph_builder.GraphNode(
             id=get_graph_io_node_name(value),
             label=value.name,  # type: ignore
         )
         producer = value.producer()
-        if producer is not None and producer.name is not None:
+        if producer is not None:
+            assert producer.name, "Bug: Node name is required"
             node.incomingEdges.append(
                 graph_builder.IncomingEdge(
                     sourceNodeId=producer.name,
                     sourceNodeOutputId=str(value.index()),
                     targetNodeInputId="0",
                 )
             )
@@ -379,15 +374,17 @@
     else:
         graph_name = onnx_graph.name
     graph = graph_builder.Graph(id=graph_name, nodes=[])
     graph_inputs = set(onnx_graph.inputs)
     all_nodes = {}
     add_graph_io(graph, onnx_graph.inputs, type="Input", all_nodes=all_nodes)
 
-    for onnx_node in onnx_graph:
+    for i, onnx_node in enumerate(onnx_graph):
+        if not onnx_node.name:
+            onnx_node.name = f"<node_{i}>"
         node = create_node(
             onnx_node,
             graph_inputs,  # type: ignore
             namespace=graph_name,
             all_function_ids=all_function_ids,
             opset_version=opset_version,
         )  # type: ignore
```

### Comparing `model_explorer_onnx-0.1.3/src/model_explorer_onnx.egg-info/PKG-INFO` & `model_explorer_onnx-0.1.4/src/model_explorer_onnx.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: model-explorer-onnx
-Version: 0.1.3
+Version: 0.1.4
 Summary: Adapter for ai-edge-model-explorer to support ONNX models
 Author-email: Justin Chu <justinchu@microsoft.com>
 License: MIT License
         
         Copyright (c) 2024 Justin Chu
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

