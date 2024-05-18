# Comparing `tmp/model_explorer_onnx-0.1.2.tar.gz` & `tmp/model_explorer_onnx-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "model_explorer_onnx-0.1.2.tar", last modified: Fri May 17 22:23:58 2024, max compression
+gzip compressed data, was "model_explorer_onnx-0.1.3.tar", last modified: Fri May 17 23:53:18 2024, max compression
```

## Comparing `model_explorer_onnx-0.1.2.tar` & `model_explorer_onnx-0.1.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 22:23:58.053470 model_explorer_onnx-0.1.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-05-17 22:23:54.000000 model_explorer_onnx-0.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3065 2024-05-17 22:23:58.053470 model_explorer_onnx-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      837 2024-05-17 22:23:54.000000 model_explorer_onnx-0.1.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      986 2024-05-17 22:23:54.000000 model_explorer_onnx-0.1.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-17 22:23:58.053470 model_explorer_onnx-0.1.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 22:23:58.049470 model_explorer_onnx-0.1.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 22:23:58.049470 model_explorer_onnx-0.1.2/src/model_explorer_onnx/
--rw-r--r--   0 runner    (1001) docker     (127)    13378 2024-05-17 22:23:54.000000 model_explorer_onnx-0.1.2/src/model_explorer_onnx/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 22:23:58.053470 model_explorer_onnx-0.1.2/src/model_explorer_onnx.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3065 2024-05-17 22:23:58.000000 model_explorer_onnx-0.1.2/src/model_explorer_onnx.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      298 2024-05-17 22:23:58.000000 model_explorer_onnx-0.1.2/src/model_explorer_onnx.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-17 22:23:58.000000 model_explorer_onnx-0.1.2/src/model_explorer_onnx.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-05-17 22:23:58.000000 model_explorer_onnx-0.1.2/src/model_explorer_onnx.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-17 22:23:58.000000 model_explorer_onnx-0.1.2/src/model_explorer_onnx.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 23:53:18.902123 model_explorer_onnx-0.1.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-05-17 23:53:15.000000 model_explorer_onnx-0.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3283 2024-05-17 23:53:18.902123 model_explorer_onnx-0.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      979 2024-05-17 23:53:15.000000 model_explorer_onnx-0.1.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-05-17 23:53:15.000000 model_explorer_onnx-0.1.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-17 23:53:18.902123 model_explorer_onnx-0.1.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 23:53:18.902123 model_explorer_onnx-0.1.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 23:53:18.902123 model_explorer_onnx-0.1.3/src/model_explorer_onnx/
+-rw-r--r--   0 runner    (1001) docker     (127)    16832 2024-05-17 23:53:15.000000 model_explorer_onnx-0.1.3/src/model_explorer_onnx/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 23:53:18.902123 model_explorer_onnx-0.1.3/src/model_explorer_onnx.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3283 2024-05-17 23:53:18.000000 model_explorer_onnx-0.1.3/src/model_explorer_onnx.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      298 2024-05-17 23:53:18.000000 model_explorer_onnx-0.1.3/src/model_explorer_onnx.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-17 23:53:18.000000 model_explorer_onnx-0.1.3/src/model_explorer_onnx.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-05-17 23:53:18.000000 model_explorer_onnx-0.1.3/src/model_explorer_onnx.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-17 23:53:18.000000 model_explorer_onnx-0.1.3/src/model_explorer_onnx.egg-info/top_level.txt
```

### Comparing `model_explorer_onnx-0.1.2/LICENSE` & `model_explorer_onnx-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `model_explorer_onnx-0.1.2/PKG-INFO` & `model_explorer_onnx-0.1.3/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: model-explorer-onnx
-Version: 0.1.2
+Version: 0.1.3
 Summary: Adapter for ai-edge-model-explorer to support ONNX models
 Author-email: Justin Chu <justinchu@microsoft.com>
 License: MIT License
         
         Copyright (c) 2024 Justin Chu
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -21,14 +21,15 @@
         IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
         FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
         
+Project-URL: Repository, https://github.com/justinchuby/model-explorer-onnx
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Programming Language :: Python :: 3.8
@@ -67,7 +68,9 @@
 ## Screenshots
 
 <img width="1294" alt="image" src="https://github.com/justinchuby/model-explorer-onnx/assets/11205048/ed7e1eee-a693-48bd-811d-b384f784ef9b">
 
 <img width="1291" alt="image" src="https://github.com/justinchuby/model-explorer-onnx/assets/11205048/b266d8e9-9760-4860-a0a7-eda1de31e1a1">
 
 <img width="1285" alt="image" src="https://github.com/justinchuby/model-explorer-onnx/assets/11205048/b772aa13-4cc3-4034-a729-f134fa3cf818">
+
+<img width="1292" alt="image" src="https://github.com/justinchuby/model-explorer-onnx/assets/11205048/dabbad76-0ec7-43b1-b253-13b81e7dc658">
```

### Comparing `model_explorer_onnx-0.1.2/README.md` & `model_explorer_onnx-0.1.3/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -19,7 +19,9 @@
 ## Screenshots
 
 <img width="1294" alt="image" src="https://github.com/justinchuby/model-explorer-onnx/assets/11205048/ed7e1eee-a693-48bd-811d-b384f784ef9b">
 
 <img width="1291" alt="image" src="https://github.com/justinchuby/model-explorer-onnx/assets/11205048/b266d8e9-9760-4860-a0a7-eda1de31e1a1">
 
 <img width="1285" alt="image" src="https://github.com/justinchuby/model-explorer-onnx/assets/11205048/b772aa13-4cc3-4034-a729-f134fa3cf818">
+
+<img width="1292" alt="image" src="https://github.com/justinchuby/model-explorer-onnx/assets/11205048/dabbad76-0ec7-43b1-b253-13b81e7dc658">
```

### Comparing `model_explorer_onnx-0.1.2/pyproject.toml` & `model_explorer_onnx-0.1.3/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "model-explorer-onnx"
-version = "0.1.2"
+version = "0.1.3"
 description = "Adapter for ai-edge-model-explorer to support ONNX models"
 authors = [{ name = "Justin Chu", email = "justinchu@microsoft.com" }]
 readme = "README.md"
 requires-python = ">=3.8"
 license = { file = "LICENSE" }
 classifiers = [
   "Development Status :: 3 - Alpha",
@@ -28,7 +28,10 @@
 dependencies = [
   "ai-edge-model-explorer",
   "numpy",
   "onnx",
   "onnxscript>=0.1.0.dev20240517",
   "ml_dtypes",
 ]
+
+[project.urls]
+Repository = "https://github.com/justinchuby/model-explorer-onnx"
```

### Comparing `model_explorer_onnx-0.1.2/src/model_explorer_onnx/main.py` & `model_explorer_onnx-0.1.3/src/model_explorer_onnx/main.py`

 * *Files 16% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 import onnx
 from model_explorer import graph_builder
 from onnxscript import ir
 
 logger = logging.getLogger(__name__)
 
 _TENSOR_DISPLAY_LIMIT = 1024
+_DEFAULT_OPSET_VERSION = 18
 
 
 def display_tensor(tensor: ir.TensorProtocol | None) -> str:
     if tensor is None:
         return "Data not available"
     if tensor.size < _TENSOR_DISPLAY_LIMIT:
         try:
@@ -64,52 +65,127 @@
 def get_function_graph_name(identifier: ir.OperatorIdentifier) -> str:
     name = f"[function]{identifier[0]}::{identifier[1]}"
     if identifier[2]:
         name += f"::{identifier[2]}"
     return name
 
 
-def add_inputs_metadata(onnx_node: ir.Node, node: graph_builder.GraphNode):
+def get_node_input_param_name(
+    schema: onnx.defs.OpSchema, input_index: int
+) -> str | None:
+    """Get the name of the input parameter of the node from OpSchema."""
+    try:
+        if len(schema.inputs) == 0:
+            # Invalid schema.
+            return None
+        if input_index < len(schema.inputs):
+            return schema.inputs[input_index].name
+        if (
+            schema.inputs[-1].option
+            == onnx.defs.OpSchema.FormalParameterOption.Variadic
+        ):
+            # The last input is variadic. Return the name of the last input.
+            return schema.inputs[-1].name
+        return None
+    except Exception as e:
+        logger.warning("Failed to get input schema name: %s", e)
+    return None
+
+
+def get_node_output_param_name(
+    schema: onnx.defs.OpSchema, output_index: int
+) -> str | None:
+    """Get the name of the output parameter of the node from OpSchema."""
+    try:
+        if len(schema.outputs) == 0:
+            # Invalid schema. Return the output index as a fallback.
+            return None
+        if output_index < len(schema.outputs):
+            return schema.outputs[output_index].name
+        if (
+            schema.outputs[-1].option
+            == onnx.defs.OpSchema.FormalParameterOption.Variadic
+        ):
+            # The last input is variadic. Return the name of the last input.
+            return schema.outputs[-1].name
+        return None
+    except Exception as e:
+        logger.warning("Failed to get output schema name: %s", e)
+
+
+def add_inputs_metadata(
+    onnx_node: ir.Node, node: graph_builder.GraphNode, opset_version: int
+):
+    if onnx.defs.has(onnx_node.op_type, max_inclusive_version=opset_version):
+        schema = onnx.defs.get_schema(
+            onnx_node.op_type, max_inclusive_version=opset_version
+        )
+    else:
+        schema = None
     for i, input_value in enumerate(onnx_node.inputs):
         metadata = graph_builder.MetadataItem(id=str(i), attrs=[])
         if input_value is None:
             metadata.attrs.append(graph_builder.KeyValue(key="__tensor_tag", value=""))
         else:
             metadata.attrs.append(
                 graph_builder.KeyValue(key="__tensor_tag", value=input_value.name or "")
             )
             # tensor_shape is a special key that is used to display the type and shape of the tensor
             metadata.attrs.append(
                 graph_builder.KeyValue(
                     key="tensor_shape", value=format_tensor_shape(input_value)
                 )
             )
+        if schema is not None:
+            if (param_name := get_node_input_param_name(schema, i)) is not None:
+                metadata.attrs.append(
+                    graph_builder.KeyValue(key="param_name", value=param_name)
+                )
         node.inputsMetadata.append(metadata)
 
 
-def add_outputs_metadata(onnx_node: ir.Node, node: graph_builder.GraphNode):
+def add_outputs_metadata(
+    onnx_node: ir.Node, node: graph_builder.GraphNode, opset_version: int
+):
+    if onnx.defs.has(onnx_node.op_type, max_inclusive_version=opset_version):
+        schema = onnx.defs.get_schema(
+            onnx_node.op_type, max_inclusive_version=opset_version
+        )
+    else:
+        schema = None
     for output in onnx_node.outputs:
         metadata = graph_builder.MetadataItem(id=str(output.index()), attrs=[])
         metadata.attrs.append(
             graph_builder.KeyValue(key="__tensor_tag", value=output.name or "")
         )
         # tensor_shape is a special key that is used to display the type and shape of the tensor
         metadata.attrs.append(
             graph_builder.KeyValue(
                 key="tensor_shape", value=format_tensor_shape(output)
             )
         )
+        if schema is not None:
+            output_index = output.index()
+            assert output_index is not None
+            if (
+                param_name := get_node_output_param_name(schema, output_index)
+            ) is not None:
+                metadata.attrs.append(
+                    graph_builder.KeyValue(key="param_name", value=param_name)
+                )
         node.outputsMetadata.append(metadata)
 
 
 def add_node_attrs(onnx_node: ir.Node, node: graph_builder.GraphNode):
     for attr in onnx_node.attributes.values():
         if isinstance(attr, ir.Attr):
             if attr.type == ir.AttributeType.TENSOR:
                 attr_value = display_tensor(attr.value)
+            elif onnx_node.op_type == "Cast" and attr.name == "to":
+                attr_value = str(ir.DataType(attr.value))
             else:
                 attr_value = str(attr.value)
             node.attrs.append(graph_builder.KeyValue(key=attr.name, value=attr_value))
         elif isinstance(attr, ir.RefAttr):
             node.attrs.append(
                 graph_builder.KeyValue(
                     key=attr.name, value=f"Ref({attr.ref_attr_name})"
@@ -163,15 +239,25 @@
 
 
 def create_node(
     onnx_node: ir.Node,
     graph_inputs: set[ir.Value],
     namespace: str,
     all_function_ids: set[ir.OperatorIdentifier],
+    opset_version: int,
 ) -> graph_builder.GraphNode | None:
+    """Create a GraphNode from an ONNX node.
+
+    Args:
+        onnx_node: The ONNX node to convert.
+        graph_inputs: The set of graph inputs.
+        namespace: The namespace of the node.
+        all_function_ids: The set of all function identifiers.
+        opset_version: The current ONNX opset version.
+    """
     if onnx_node.name is None:
         logger.warning("Node does not have a name. Skipping node %s.", onnx_node)
         return None
 
     embedded_namespace = onnx_node.name.lstrip("/").split("/")[0:-1]
     embedded_namespace = [ns or "<anonymous>" for ns in embedded_namespace]
     if embedded_namespace:
@@ -179,16 +265,16 @@
     node = graph_builder.GraphNode(
         id=onnx_node.name,
         label=create_op_label(onnx_node.domain, onnx_node.op_type),
         namespace=namespace,
     )
     add_incoming_edges(onnx_node, node, graph_inputs)
     add_node_attrs(onnx_node, node)
-    add_inputs_metadata(onnx_node, node)
-    add_outputs_metadata(onnx_node, node)
+    add_inputs_metadata(onnx_node, node, opset_version=opset_version)
+    add_outputs_metadata(onnx_node, node, opset_version=opset_version)
     if onnx_node.op_identifier() in all_function_ids:
         node.subgraphIds.append(get_function_graph_name(onnx_node.op_identifier()))
     return node
 
 
 def add_graph_io(
     graph: graph_builder.Graph,
@@ -277,15 +363,17 @@
             )
         )
         node.outputsMetadata.append(metadata)
         graph.nodes.append(node)
 
 
 def create_graph(
-    onnx_graph: ir.Graph | ir.Function, all_function_ids: set[ir.OperatorIdentifier]
+    onnx_graph: ir.Graph | ir.Function,
+    all_function_ids: set[ir.OperatorIdentifier],
+    opset_version: int,
 ) -> graph_builder.Graph | None:
     if isinstance(onnx_graph, ir.Function):
         graph_name = get_function_graph_name(onnx_graph.identifier())
     elif onnx_graph.name is None:
         logger.warning("Graph does not have a name. skipping graph: %s", onnx_graph)
         return None
     else:
@@ -297,14 +385,15 @@
 
     for onnx_node in onnx_graph:
         node = create_node(
             onnx_node,
             graph_inputs,  # type: ignore
             namespace=graph_name,
             all_function_ids=all_function_ids,
+            opset_version=opset_version,
         )  # type: ignore
         if node is None:
             continue
         graph.nodes.append(node)
         all_nodes[node.id] = node
 
     # Add initializers
@@ -350,17 +439,22 @@
         base_dir = os.path.dirname(model_filepath)
         onnx.load_external_data_for_model(onnx_model, base_dir)
 
         # Convert to ONNX IR
         model = ir.serde.deserialize_model(onnx_model)
         all_function_ids = set(model.functions)
         graphs = []
+        opset_version = model.opset_imports.get("", _DEFAULT_OPSET_VERSION)
         # TODO: Better support subgraphs in nodes
-        main_graph = create_graph(model.graph, all_function_ids)
+        main_graph = create_graph(
+            model.graph, all_function_ids, opset_version=opset_version
+        )
         assert main_graph is not None
         graphs.append(main_graph)
 
         for function in model.functions.values():
-            function_graph = create_graph(function, all_function_ids)
+            function_graph = create_graph(
+                function, all_function_ids, opset_version=opset_version
+            )
             assert function_graph is not None
             graphs.append(function_graph)
         return {"graphs": graphs}
```

### Comparing `model_explorer_onnx-0.1.2/src/model_explorer_onnx.egg-info/PKG-INFO` & `model_explorer_onnx-0.1.3/src/model_explorer_onnx.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: model-explorer-onnx
-Version: 0.1.2
+Version: 0.1.3
 Summary: Adapter for ai-edge-model-explorer to support ONNX models
 Author-email: Justin Chu <justinchu@microsoft.com>
 License: MIT License
         
         Copyright (c) 2024 Justin Chu
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -21,14 +21,15 @@
         IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
         FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
         
+Project-URL: Repository, https://github.com/justinchuby/model-explorer-onnx
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Programming Language :: Python :: 3.8
@@ -67,7 +68,9 @@
 ## Screenshots
 
 <img width="1294" alt="image" src="https://github.com/justinchuby/model-explorer-onnx/assets/11205048/ed7e1eee-a693-48bd-811d-b384f784ef9b">
 
 <img width="1291" alt="image" src="https://github.com/justinchuby/model-explorer-onnx/assets/11205048/b266d8e9-9760-4860-a0a7-eda1de31e1a1">
 
 <img width="1285" alt="image" src="https://github.com/justinchuby/model-explorer-onnx/assets/11205048/b772aa13-4cc3-4034-a729-f134fa3cf818">
+
+<img width="1292" alt="image" src="https://github.com/justinchuby/model-explorer-onnx/assets/11205048/dabbad76-0ec7-43b1-b253-13b81e7dc658">
```

