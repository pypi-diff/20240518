# Comparing `tmp/statedict2pytree-0.3.0.tar.gz` & `tmp/statedict2pytree-0.4.0.tar.gz`

## Comparing `statedict2pytree-0.3.0.tar` & `statedict2pytree-0.4.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0      427 2020-02-02 00:00:00.000000 statedict2pytree-0.3.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0    50334 2020-02-02 00:00:00.000000 statedict2pytree-0.3.0/package-lock.json
--rw-r--r--   0        0        0      267 2020-02-02 00:00:00.000000 statedict2pytree-0.3.0/package.json
--rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 statedict2pytree-0.3.0/pyrightconfig.json
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 statedict2pytree-0.3.0/tailwind.config.js
--rw-r--r--   0        0        0   336449 2020-02-02 00:00:00.000000 statedict2pytree-0.3.0/torch2jax.png
--rw-r--r--   0        0        0      450 2020-02-02 00:00:00.000000 statedict2pytree-0.3.0/examples/convert_resnet.py
--rw-r--r--   0        0        0    97404 2020-02-02 00:00:00.000000 statedict2pytree-0.3.0/examples/doggo.jpeg
--rw-r--r--   0        0        0    10628 2020-02-02 00:00:00.000000 statedict2pytree-0.3.0/examples/resnet.py
--rw-r--r--   0        0        0     2071 2020-02-02 00:00:00.000000 statedict2pytree-0.3.0/examples/test_resnet_inference.py
--rw-r--r--   0        0        0      240 2020-02-02 00:00:00.000000 statedict2pytree-0.3.0/statedict2pytree/__init__.py
--rw-r--r--   0        0        0     7103 2020-02-02 00:00:00.000000 statedict2pytree-0.3.0/statedict2pytree/statedict2pytree.py
--rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 statedict2pytree-0.3.0/statedict2pytree/static/input.css
--rw-r--r--   0        0        0    40813 2020-02-02 00:00:00.000000 statedict2pytree-0.3.0/statedict2pytree/static/output.css
--rw-r--r--   0        0        0     7506 2020-02-02 00:00:00.000000 statedict2pytree-0.3.0/statedict2pytree/templates/index.html
--rw-r--r--   0        0        0     1585 2020-02-02 00:00:00.000000 statedict2pytree-0.3.0/tests/test_conv.py
--rw-r--r--   0        0        0     1116 2020-02-02 00:00:00.000000 statedict2pytree-0.3.0/tests/test_linear.py
--rw-r--r--   0        0        0     3092 2020-02-02 00:00:00.000000 statedict2pytree-0.3.0/.gitignore
--rw-r--r--   0        0        0     3555 2020-02-02 00:00:00.000000 statedict2pytree-0.3.0/README.md
--rw-r--r--   0        0        0     1110 2020-02-02 00:00:00.000000 statedict2pytree-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     4232 2020-02-02 00:00:00.000000 statedict2pytree-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0      427 2020-02-02 00:00:00.000000 statedict2pytree-0.4.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0    50334 2020-02-02 00:00:00.000000 statedict2pytree-0.4.0/package-lock.json
+-rw-r--r--   0        0        0      267 2020-02-02 00:00:00.000000 statedict2pytree-0.4.0/package.json
+-rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 statedict2pytree-0.4.0/pyrightconfig.json
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 statedict2pytree-0.4.0/tailwind.config.js
+-rw-r--r--   0        0        0   336449 2020-02-02 00:00:00.000000 statedict2pytree-0.4.0/torch2jax.png
+-rw-r--r--   0        0        0      619 2020-02-02 00:00:00.000000 statedict2pytree-0.4.0/examples/convert_resnet.py
+-rw-r--r--   0        0        0    97404 2020-02-02 00:00:00.000000 statedict2pytree-0.4.0/examples/doggo.jpeg
+-rw-r--r--   0        0        0    11256 2020-02-02 00:00:00.000000 statedict2pytree-0.4.0/examples/resnet.py
+-rw-r--r--   0        0        0     2104 2020-02-02 00:00:00.000000 statedict2pytree-0.4.0/examples/test_resnet_inference.py
+-rw-r--r--   0        0        0      240 2020-02-02 00:00:00.000000 statedict2pytree-0.4.0/statedict2pytree/__init__.py
+-rw-r--r--   0        0        0     7175 2020-02-02 00:00:00.000000 statedict2pytree-0.4.0/statedict2pytree/statedict2pytree.py
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 statedict2pytree-0.4.0/statedict2pytree/static/input.css
+-rw-r--r--   0        0        0    40813 2020-02-02 00:00:00.000000 statedict2pytree-0.4.0/statedict2pytree/static/output.css
+-rw-r--r--   0        0        0     7506 2020-02-02 00:00:00.000000 statedict2pytree-0.4.0/statedict2pytree/templates/index.html
+-rw-r--r--   0        0        0     1585 2020-02-02 00:00:00.000000 statedict2pytree-0.4.0/tests/test_conv.py
+-rw-r--r--   0        0        0     1116 2020-02-02 00:00:00.000000 statedict2pytree-0.4.0/tests/test_linear.py
+-rw-r--r--   0        0        0     3092 2020-02-02 00:00:00.000000 statedict2pytree-0.4.0/.gitignore
+-rw-r--r--   0        0        0     3555 2020-02-02 00:00:00.000000 statedict2pytree-0.4.0/README.md
+-rw-r--r--   0        0        0     1110 2020-02-02 00:00:00.000000 statedict2pytree-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     4232 2020-02-02 00:00:00.000000 statedict2pytree-0.4.0/PKG-INFO
```

### Comparing `statedict2pytree-0.3.0/package-lock.json` & `statedict2pytree-0.4.0/package-lock.json`

 * *Files identical despite different names*

### Comparing `statedict2pytree-0.3.0/torch2jax.png` & `statedict2pytree-0.4.0/torch2jax.png`

 * *Files identical despite different names*

### Comparing `statedict2pytree-0.3.0/examples/doggo.jpeg` & `statedict2pytree-0.4.0/examples/doggo.jpeg`

 * *Files identical despite different names*

### Comparing `statedict2pytree-0.3.0/examples/resnet.py` & `statedict2pytree-0.4.0/examples/resnet.py`

 * *Files 6% similar despite different names*

```diff
@@ -329,20 +329,30 @@
     else:
         return ResNet(
             BasicBlock, layers, image_channels, num_classes, **kwargs, key=key
         )
 
 
 def resnet34(
-    image_channels: int = 3, num_classes: int = 1000, *, key: PRNGKeyArray, **kwargs
+    image_channels: int = 3,
+    num_classes: int = 1000,
+    *,
+    key: PRNGKeyArray,
+    make_with_state: bool = True,
+    **kwargs,
 ):
     layers = [3, 4, 6, 3]
-    return eqx.nn.make_with_state(ResNet)(
-        BasicBlock, layers, image_channels, num_classes, **kwargs, key=key
-    )
+    if make_with_state:
+        return eqx.nn.make_with_state(ResNet)(
+            BasicBlock, layers, image_channels, num_classes, **kwargs, key=key
+        )
+    else:
+        return ResNet(
+            BasicBlock, layers, image_channels, num_classes, **kwargs, key=key
+        )
 
 
 def resnet50(
     image_channels: int = 3,
     num_classes: int = 1000,
     *,
     key: PRNGKeyArray,
@@ -357,22 +367,43 @@
     else:
         return ResNet(
             Bottleneck, layers, image_channels, num_classes, **kwargs, key=key
         )
 
 
 def resnet101(
-    image_channels: int = 3, num_classes: int = 1000, *, key: PRNGKeyArray, **kwargs
+    image_channels: int = 3,
+    num_classes: int = 1000,
+    *,
+    key: PRNGKeyArray,
+    make_with_state: bool = True,
+    **kwargs,
 ):
     layers = [3, 4, 23, 3]
-    return eqx.nn.make_with_state(ResNet)(
-        Bottleneck, layers, image_channels, num_classes, **kwargs, key=key
-    )
+
+    if make_with_state:
+        return eqx.nn.make_with_state(ResNet)(
+            Bottleneck, layers, image_channels, num_classes, **kwargs, key=key
+        )
+    else:
+        return ResNet(
+            Bottleneck, layers, image_channels, num_classes, **kwargs, key=key
+        )
 
 
 def resnet152(
-    image_channels: int = 3, num_classes: int = 1000, *, key: PRNGKeyArray, **kwargs
+    image_channels: int = 3,
+    num_classes: int = 1000,
+    *,
+    key: PRNGKeyArray,
+    make_with_state: bool = True,
+    **kwargs,
 ):
     layers = [3, 8, 36, 3]
-    return eqx.nn.make_with_state(ResNet)(
-        Bottleneck, layers, image_channels, num_classes, **kwargs, key=key
-    )
+    if make_with_state:
+        return eqx.nn.make_with_state(ResNet)(
+            Bottleneck, layers, image_channels, num_classes, **kwargs, key=key
+        )
+    else:
+        return ResNet(
+            Bottleneck, layers, image_channels, num_classes, **kwargs, key=key
+        )
```

### Comparing `statedict2pytree-0.3.0/examples/test_resnet_inference.py` & `statedict2pytree-0.4.0/examples/test_resnet_inference.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,23 +2,23 @@
 import json
 import urllib
 
 import equinox as eqx
 import jax
 import jax.numpy as jnp
 import torch
+from examples.resnet import resnet152
 from PIL import Image
-from tests.resnet import resnet50
 from torchvision import transforms
-from torchvision.models import resnet50 as t_resnet50, ResNet50_Weights
+from torchvision.models import resnet152 as t_resnet152, ResNet152_Weights
 
 
 def test_resnet():
-    resnet_jax = resnet50(key=jax.random.PRNGKey(33), make_with_state=False)
-    resnet_torch = t_resnet50(weights=ResNet50_Weights.DEFAULT)
+    resnet_jax = resnet152(key=jax.random.PRNGKey(33), make_with_state=False)
+    resnet_torch = t_resnet152(weights=ResNet152_Weights.DEFAULT)
 
     img_name = "doggo.jpeg"
 
     transform = transforms.Compose(
         [
             transforms.Resize(256),
             transforms.CenterCrop(224),
@@ -38,25 +38,25 @@
         _, predicted = torch.max(output, 1)
 
     print(
         f"Predicted: {predicted.item()}"
     )  # Outputs the ImageNet class index of the prediction
 
     url = "https://storage.googleapis.com/download.tensorflow.org/data/imagenet_class_index.json"
-    with urllib.request.urlopen(url) as url:
+    with urllib.request.urlopen(url) as url:  # pyright: ignore
         imagenet_labels = json.loads(url.read().decode())
 
     label = imagenet_labels[str(predicted.item())][1]
     print(f"Label for index {predicted.item()}: {label}")
 
     identity = lambda x: x
     model_callable = ft.partial(identity, resnet_jax)
     model, state = eqx.nn.make_with_state(model_callable)()
 
-    model, state = eqx.tree_deserialise_leaves("model.eqx", (model, state))
+    model, state = eqx.tree_deserialise_leaves("resnet152.eqx", (model, state))
 
     jax_batch = jnp.array(batch_t.numpy())
     out, state = eqx.filter_vmap(
         model, in_axes=(0, None), out_axes=(0, None), axis_name="batch"
     )(jax_batch, state)
     print(f"{out.shape}")
```

### Comparing `statedict2pytree-0.3.0/statedict2pytree/statedict2pytree.py` & `statedict2pytree-0.4.0/statedict2pytree/statedict2pytree.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,15 +42,15 @@
 def get_node(
     tree: PyTree, targets: list[str], log_when_not_found: bool = False
 ) -> PyTree | None:
     if len(targets) == 0 or tree is None:
         return tree
     else:
         next_target: str = targets[0]
-        if bool(re.search(r"\[\d\]", next_target)):
+        if bool(re.search(r"\[\d+\]", next_target)):
             split_index = next_target.rfind("[")
             name, index = next_target[:split_index], next_target[split_index:]
             index = index[1:-1]
             if hasattr(tree, name):
                 subtree = getattr(tree, name)[int(index)]
             else:
                 subtree = None
@@ -153,14 +153,17 @@
         torch_fields=state_dict_to_fields(STATE_DICT),
     )
 
 
 def autoconvert(pytree: PyTree, state_dict: dict) -> tuple[PyTree, eqx.nn.State]:
     jax_fields = pytree_to_fields(pytree)
     torch_fields = state_dict_to_fields(state_dict)
+
+    for k, v in state_dict.items():
+        state_dict[k] = v.numpy()
     return convert(jax_fields, torch_fields, pytree, state_dict)
 
 
 def convert(
     jax_fields: list[JaxField],
     torch_fields: list[TorchField],
     pytree: PyTree,
```

### Comparing `statedict2pytree-0.3.0/statedict2pytree/static/output.css` & `statedict2pytree-0.4.0/statedict2pytree/static/output.css`

 * *Files identical despite different names*

### Comparing `statedict2pytree-0.3.0/statedict2pytree/templates/index.html` & `statedict2pytree-0.4.0/statedict2pytree/templates/index.html`

 * *Files identical despite different names*

### Comparing `statedict2pytree-0.3.0/tests/test_conv.py` & `statedict2pytree-0.4.0/tests/test_conv.py`

 * *Files identical despite different names*

### Comparing `statedict2pytree-0.3.0/tests/test_linear.py` & `statedict2pytree-0.4.0/tests/test_linear.py`

 * *Files identical despite different names*

### Comparing `statedict2pytree-0.3.0/.gitignore` & `statedict2pytree-0.4.0/.gitignore`

 * *Files identical despite different names*

### Comparing `statedict2pytree-0.3.0/README.md` & `statedict2pytree-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `statedict2pytree-0.3.0/pyproject.toml` & `statedict2pytree-0.4.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "statedict2pytree"
-version = "0.3.0"
+version = "0.4.0"
 description = "Converts torch models into PyTrees for Equinox"
 readme = "README.md"
 requires-python = "~=3.10"
 authors = [{ name = "Artur A. Galstyan", email = "mail@arturgalstyan.dev" }]
 dependencies = [
     "jax",
     "equinox>=0.11.4",
```

### Comparing `statedict2pytree-0.3.0/PKG-INFO` & `statedict2pytree-0.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: statedict2pytree
-Version: 0.3.0
+Version: 0.4.0
 Summary: Converts torch models into PyTrees for Equinox
 Author-email: "Artur A. Galstyan" <mail@arturgalstyan.dev>
 Requires-Python: ~=3.10
 Requires-Dist: beartype
 Requires-Dist: equinox>=0.11.4
 Requires-Dist: flask
 Requires-Dist: jax
```

