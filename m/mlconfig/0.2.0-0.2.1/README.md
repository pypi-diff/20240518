# Comparing `tmp/mlconfig-0.2.0-py3-none-any.whl.zip` & `tmp/mlconfig-0.2.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 3412 bytes, number of entries: 7
+Zip file size: 3369 bytes, number of entries: 7
 -rw-r--r--  2.0 unx      105 b- defN 80-Jan-01 00:00 mlconfig/__init__.py
--rw-r--r--  2.0 unx     1961 b- defN 80-Jan-01 00:00 mlconfig/conf.py
--rw-r--r--  2.0 unx     1001 b- defN 80-Jan-01 00:00 mlconfig/torch/__init__.py
--rw-r--r--  2.0 unx     1066 b- defN 80-Jan-01 00:00 mlconfig-0.2.0.dist-info/LICENSE
--rw-r--r--  2.0 unx      457 b- defN 80-Jan-01 00:00 mlconfig-0.2.0.dist-info/METADATA
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 mlconfig-0.2.0.dist-info/WHEEL
-?rw-r--r--  2.0 unx      529 b- defN 16-Jan-01 00:00 mlconfig-0.2.0.dist-info/RECORD
-7 files, 5207 bytes uncompressed, 2482 bytes compressed:  52.3%
+-rw-r--r--  2.0 unx     1916 b- defN 80-Jan-01 00:00 mlconfig/conf.py
+-rw-r--r--  2.0 unx     1005 b- defN 80-Jan-01 00:00 mlconfig/torch/__init__.py
+-rw-r--r--  2.0 unx     1066 b- defN 80-Jan-01 00:00 mlconfig-0.2.1.dist-info/LICENSE
+-rw-r--r--  2.0 unx      505 b- defN 80-Jan-01 00:00 mlconfig-0.2.1.dist-info/METADATA
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 mlconfig-0.2.1.dist-info/WHEEL
+?rw-r--r--  2.0 unx      529 b- defN 16-Jan-01 00:00 mlconfig-0.2.1.dist-info/RECORD
+7 files, 5214 bytes uncompressed, 2439 bytes compressed:  53.2%
```

## zipnote {}

```diff
@@ -3,20 +3,20 @@
 
 Filename: mlconfig/conf.py
 Comment: 
 
 Filename: mlconfig/torch/__init__.py
 Comment: 
 
-Filename: mlconfig-0.2.0.dist-info/LICENSE
+Filename: mlconfig-0.2.1.dist-info/LICENSE
 Comment: 
 
-Filename: mlconfig-0.2.0.dist-info/METADATA
+Filename: mlconfig-0.2.1.dist-info/METADATA
 Comment: 
 
-Filename: mlconfig-0.2.0.dist-info/WHEEL
+Filename: mlconfig-0.2.1.dist-info/WHEEL
 Comment: 
 
-Filename: mlconfig-0.2.0.dist-info/RECORD
+Filename: mlconfig-0.2.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## mlconfig/conf.py

```diff
@@ -1,14 +1,14 @@
 import copy
 import functools
 
 from omegaconf import OmegaConf
 
-_REGISTRY = {}
-_KEY_OF_FUNC_OR_CLS = 'name'
+_registry = {}
+_key = "name"
 
 
 def load(f=None, obj=None) -> OmegaConf:
     """Load configuration file or structured object.
     If both are provided, then the configuration from file
     will override the configuration from structured object.
 
@@ -25,15 +25,15 @@
         configs.append(OmegaConf.structured(obj))
 
     if f is not None:
         configs.append(OmegaConf.load(f))
 
     length = len(configs)
     if length == 0:
-        raise ValueError('No configuration file or structured object provided.')
+        raise ValueError("No configuration file or structured object provided.")
     elif length == 1:
         return configs[0]
 
     return OmegaConf.merge(*configs)
 
 
 def register(func_or_cls=None, name: str = None):
@@ -46,34 +46,34 @@
     if isinstance(func_or_cls, str) and name is None:
         func_or_cls, name = None, func_or_cls
 
     def _register(func_or_cls, name=None):
         if name is None:
             name = func_or_cls.__name__
 
-        if name not in _REGISTRY:
-            _REGISTRY[name] = func_or_cls
+        if name not in _registry:
+            _registry[name] = func_or_cls
         else:
-            raise ValueError('duplicate name {} found'.format(name))
+            raise ValueError("duplicate name {} found".format(name))
 
         return func_or_cls
 
     if func_or_cls is None:
         return functools.partial(_register, name=name)
 
     return _register(func_or_cls, name=name)
 
 
 def getcls(conf):
-    return _REGISTRY[conf[_KEY_OF_FUNC_OR_CLS]]
+    return _registry[conf[_key]]
 
 
 def instantiate(conf, *args, **kwargs):
     kwargs = copy.deepcopy(kwargs)
 
     for k, v in conf.items():
-        if k not in kwargs and k != _KEY_OF_FUNC_OR_CLS:
+        if k not in kwargs and k != _key:
             kwargs[k] = v
 
     func_or_cls = getcls(conf)
 
     return func_or_cls(*args, **kwargs)
```

## mlconfig/torch/__init__.py

```diff
@@ -1,34 +1,34 @@
 import functools
 
 import mlconfig
 
 try:
     from torch import optim
 except ImportError:
-    print('Failed to import torch.')
+    print("Failed to import torch.")
 
 
-def _register_classes(module, superclass, prefix=None, sep='.'):
+def _register_classes(module, superclass, prefix=None, sep="."):
     for name in dir(module):
         attr = getattr(module, name)
 
         if isinstance(attr, type) and issubclass(attr, superclass):
             if attr is superclass:
                 continue
 
             if prefix is not None:
                 name = prefix + sep + name
 
-            mlconfig.conf(attr, name=name)
+            mlconfig.register(attr, name=name)
 
 
 def get_lr_scheduler_class():
     # PyTorch 2.0 renamed LRScheduler to _LRScheduler
-    name = 'LRScheduler' if hasattr(optim.lr_scheduler, 'LRScheduler') else '_LRScheduler'
+    name = "LRScheduler" if hasattr(optim.lr_scheduler, "LRScheduler") else "_LRScheduler"
     return getattr(optim.lr_scheduler, name)
 
 
 register_torch_optimizers = functools.partial(
     _register_classes,
     module=optim,
     superclass=optim.Optimizer,
```

## Comparing `mlconfig-0.2.0.dist-info/LICENSE` & `mlconfig-0.2.1.dist-info/LICENSE`

 * *Files identical despite different names*

