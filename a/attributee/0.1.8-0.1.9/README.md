# Comparing `tmp/attributee-0.1.8.tar.gz` & `tmp/attributee-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "attributee-0.1.8.tar", last modified: Thu Mar  2 15:33:16 2023, max compression
+gzip compressed data, was "attributee-0.1.9.tar", last modified: Sat May 18 21:09:25 2024, max compression
```

## Comparing `attributee-0.1.8.tar` & `attributee-0.1.9.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 lukacu    (1000) lukacu    (1000)        0 2023-03-02 15:33:16.542486 attributee-0.1.8/
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     1281 2020-11-12 14:50:57.000000 attributee-0.1.8/LICENSE.md
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     1576 2023-03-02 15:33:16.542486 attributee-0.1.8/PKG-INFO
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     1081 2020-11-12 14:50:57.000000 attributee-0.1.8/README.md
-drwxrwxr-x   0 lukacu    (1000) lukacu    (1000)        0 2023-03-02 15:33:16.542486 attributee-0.1.8/attributee/
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)    11573 2023-01-10 16:09:09.000000 attributee-0.1.8/attributee/__init__.py
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     6490 2023-01-10 16:05:01.000000 attributee-0.1.8/attributee/containers.py
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     7943 2023-01-10 16:10:53.000000 attributee-0.1.8/attributee/io.py
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     4877 2022-01-26 13:19:55.000000 attributee-0.1.8/attributee/object.py
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     4570 2023-01-10 16:09:55.000000 attributee-0.1.8/attributee/primitives.py
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     3019 2022-02-03 11:48:42.000000 attributee-0.1.8/attributee/tests.py
-drwxrwxr-x   0 lukacu    (1000) lukacu    (1000)        0 2023-03-02 15:33:16.542486 attributee-0.1.8/attributee.egg-info/
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     1576 2023-03-02 15:33:16.000000 attributee-0.1.8/attributee.egg-info/PKG-INFO
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      296 2023-03-02 15:33:16.000000 attributee-0.1.8/attributee.egg-info/SOURCES.txt
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)        1 2023-03-02 15:33:16.000000 attributee-0.1.8/attributee.egg-info/dependency_links.txt
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)       11 2023-03-02 15:33:16.000000 attributee-0.1.8/attributee.egg-info/top_level.txt
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)       38 2023-03-02 15:33:16.542486 attributee-0.1.8/setup.cfg
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     1124 2023-03-02 15:31:40.000000 attributee-0.1.8/setup.py
+drwxrwxr-x   0 lukacu    (1000) lukacu    (1000)        0 2024-05-18 21:09:25.461004 attributee-0.1.9/
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     1281 2020-11-12 14:50:57.000000 attributee-0.1.9/LICENSE.md
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     1726 2024-05-18 21:09:25.461004 attributee-0.1.9/PKG-INFO
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     1195 2024-05-18 21:09:11.000000 attributee-0.1.9/README.md
+drwxrwxr-x   0 lukacu    (1000) lukacu    (1000)        0 2024-05-18 21:09:25.461004 attributee-0.1.9/attributee/
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)    11587 2024-05-18 21:09:11.000000 attributee-0.1.9/attributee/__init__.py
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     6490 2023-01-10 16:05:01.000000 attributee-0.1.9/attributee/containers.py
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     7943 2023-01-10 16:10:53.000000 attributee-0.1.9/attributee/io.py
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     5092 2024-05-18 21:09:11.000000 attributee-0.1.9/attributee/object.py
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     5410 2024-05-18 21:09:11.000000 attributee-0.1.9/attributee/primitives.py
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     3019 2022-02-03 11:48:42.000000 attributee-0.1.9/attributee/tests.py
+drwxrwxr-x   0 lukacu    (1000) lukacu    (1000)        0 2024-05-18 21:09:25.461004 attributee-0.1.9/attributee.egg-info/
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     1726 2024-05-18 21:09:25.000000 attributee-0.1.9/attributee.egg-info/PKG-INFO
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      296 2024-05-18 21:09:25.000000 attributee-0.1.9/attributee.egg-info/SOURCES.txt
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)        1 2024-05-18 21:09:25.000000 attributee-0.1.9/attributee.egg-info/dependency_links.txt
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)       11 2024-05-18 21:09:25.000000 attributee-0.1.9/attributee.egg-info/top_level.txt
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)       38 2024-05-18 21:09:25.461004 attributee-0.1.9/setup.cfg
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     1124 2024-05-18 21:09:11.000000 attributee-0.1.9/setup.py
```

### Comparing `attributee-0.1.8/LICENSE.md` & `attributee-0.1.9/LICENSE.md`

 * *Files identical despite different names*

### Comparing `attributee-0.1.8/PKG-INFO` & `attributee-0.1.9/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,32 +1,35 @@
 Metadata-Version: 2.1
 Name: attributee
-Version: 0.1.8
+Version: 0.1.9
 Summary: Declarative object initialization library
 Home-page: https://github.com/lukacu/attributee
 Author: Luka Cehovin Zajc
 Author-email: luka.cehovin@gmail.com
+License: UNKNOWN
+Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 4 - Beta
 Requires-Python: >=3.5
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 
+Attributee
+----------
 
-About
------
+[![PyPI package version](https://badge.fury.io/py/attributee.svg)](https://badge.fury.io/py/attributee)
 
 Attributee is a Python 3 library for declarative object initialization. Input arguments are defined as class attributes and are automatically processed when creating an object. It is in a way similar to Django ORM or some other ORMs, but the main purpose of this library is to simplify parsing input arguments to object constructors. 
 
 The library is a work-in-progress, I am adding stuff that I consider useful for my other projects.
 
 Simple use case
----------------
+===============
 
 ```
 from attributee import Attributee, String, Float
 
 class Model(Attributee):
 
     # Simply list the attributes of the object ...
@@ -43,20 +46,21 @@
 
 # automatic type conversion where possible
 model2 = Model(value1=10, value2="5")
 
 ```
 
 Documentation
--------------
+=============
 
 I am working on it.
 
 Authors
--------
+=======
 
 Luka Čehovin Zajc
 
 License
--------
+=======
 
 The library is available under the [simplified BSD license](LICENSE.md).
+
```

### Comparing `attributee-0.1.8/README.md` & `attributee-0.1.9/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -1,17 +1,18 @@
+Attributee
+----------
 
-About
------
+[![PyPI package version](https://badge.fury.io/py/attributee.svg)](https://badge.fury.io/py/attributee)
 
 Attributee is a Python 3 library for declarative object initialization. Input arguments are defined as class attributes and are automatically processed when creating an object. It is in a way similar to Django ORM or some other ORMs, but the main purpose of this library is to simplify parsing input arguments to object constructors. 
 
 The library is a work-in-progress, I am adding stuff that I consider useful for my other projects.
 
 Simple use case
----------------
+===============
 
 ```
 from attributee import Attributee, String, Float
 
 class Model(Attributee):
 
     # Simply list the attributes of the object ...
@@ -28,20 +29,20 @@
 
 # automatic type conversion where possible
 model2 = Model(value1=10, value2="5")
 
 ```
 
 Documentation
--------------
+=============
 
 I am working on it.
 
 Authors
--------
+=======
 
 Luka Čehovin Zajc
 
 License
--------
+=======
 
 The library is available under the [simplified BSD license](LICENSE.md).
```

### Comparing `attributee-0.1.8/attributee/__init__.py` & `attributee-0.1.9/attributee/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -337,10 +337,10 @@
         for aname, afield in attributes.items():
             if isinstance(afield, Collector) and not isinstance(afield, Unclaimed):
                 claimed.update(afield.filter(object, **kwargs).keys())
             elif aname in kwargs:
                 claimed.add(aname)
         return {k: v for k, v in kwargs.items() if k not in claimed}
 
-from attributee.primitives import Integer, Float, String, Boolean, Enumeration, Primitive, Number
+from attributee.primitives import Integer, Float, String, Boolean, Enumeration, Primitive, Number, URL, Pattern
 from attributee.object import Object, Callable, Date, Datetime
 from attributee.containers import List, Map, Tuple
```

### Comparing `attributee-0.1.8/attributee/containers.py` & `attributee-0.1.9/attributee/containers.py`

 * *Files identical despite different names*

### Comparing `attributee-0.1.8/attributee/io.py` & `attributee-0.1.9/attributee/io.py`

 * *Files identical despite different names*

### Comparing `attributee-0.1.8/attributee/object.py` & `attributee-0.1.9/attributee/object.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,18 +2,22 @@
 import inspect
 from datetime import datetime, date
 from typing import Mapping
 
 from attributee import Attributee, Attribute, AttributeException
 
 def import_class(classpath):
+    import importlib
     delimiter = classpath.rfind(".")
     classname = classpath[delimiter+1:len(classpath)]
     module = __import__(classpath[0:delimiter], globals(), locals(), [classname])
-    return getattr(module, classname)
+    try:
+        return getattr(module, classname)
+    except AttributeError:
+        raise ImportError(module, name=classname)
 
 def class_fullname(o):
     return class_string(o.__class__)
 
 def class_string(kls):
     if not inspect.isclass(kls): AttributeException("Input is not a class")
     module = kls.__module__
@@ -36,15 +40,18 @@
     if not issubclass(clstype, Attributee): raise AttributeException("Class {} is not an Attributee".format(typename))
     return clstype(**kwargs)
 
 class Object(Attribute):
 
     def __init__(self, resolver=default_object_resolver, subclass=None, **kwargs):
         super().__init__(**kwargs)
-        if subclass is not None and not inspect.isclass(subclass): raise AttributeException("Subclass constraint should be a class type")
+        if subclass is not None:
+            if isinstance(subclass, str):
+                subclass = import_class(subclass)
+            if not inspect.isclass(subclass): raise AttributeException("Subclass constraint should be a class type")
         self._resolver = resolver
         self._subclass = subclass
 
     def coerce(self, value, context=None):
         if not isinstance(value, Mapping): raise AttributeException("Value is not a key-value mapping")
         class_name = value.get("type", None)
         obj = self._resolver(class_name, context, **{k: v for k, v in value.items() if not k == "type"})
```

### Comparing `attributee-0.1.8/attributee/primitives.py` & `attributee-0.1.9/attributee/primitives.py`

 * *Files 13% similar despite different names*

```diff
@@ -107,14 +107,46 @@
         else:
             return self._transformer(to_string(value), ctx)
 
     @property
     def transformer(self):
         return self._transformer
 
+class URL(String):
+
+    def coerce(self, value, ctx):
+        from urllib.parse import urlparse 
+        value = super().coerce(value, ctx)
+        try:
+            return urlparse(value)
+        except ValueError as ve:
+            raise AttributeException("Unable to parse URL") from ve
+
+    def dump(self, value):
+        from urllib.parse import urlunparse
+        return urlunparse(value)
+
+class Pattern(String):
+
+    def coerce(self, value, ctx):
+        from re import Pattern, compile
+        value = super().coerce(value, ctx)
+        if value is None:
+            return None
+        if isinstance(value, Pattern):
+            return value
+        value = to_string(value)
+        return compile(value)
+
+    def dump(self, value):
+        if value is None:
+            return None
+
+        return value.pattern
+
 class Enumeration(Attribute):
 
     def __init__(self, options,  **kwargs):
         if inspect.isclass(options) and issubclass(options, Enum):
             self._mapping = options
         elif isinstance(options, Mapping):
             self._mapping = options
@@ -144,8 +176,8 @@
     def options(self):
         from .containers import ReadonlyMapping
         if inspect.isclass(self._mapping) and issubclass(self._mapping, Enum):
             return ReadonlyMapping([(e.value, e.name) for e in self._mapping])
         elif isinstance(self._mapping, typing.Mapping):
             return ReadonlyMapping(self._mapping) 
 
-__all__ = ["String", "Boolean", "Integer", "Float", "Enumeration", "Number"]
+__all__ = ["String", "Boolean", "Integer", "Float", "Enumeration", "Number", "URL", "Pattern"]
```

### Comparing `attributee-0.1.8/attributee/tests.py` & `attributee-0.1.9/attributee/tests.py`

 * *Files identical despite different names*

### Comparing `attributee-0.1.8/attributee.egg-info/PKG-INFO` & `attributee-0.1.9/attributee.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,32 +1,35 @@
 Metadata-Version: 2.1
 Name: attributee
-Version: 0.1.8
+Version: 0.1.9
 Summary: Declarative object initialization library
 Home-page: https://github.com/lukacu/attributee
 Author: Luka Cehovin Zajc
 Author-email: luka.cehovin@gmail.com
+License: UNKNOWN
+Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 4 - Beta
 Requires-Python: >=3.5
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 
+Attributee
+----------
 
-About
------
+[![PyPI package version](https://badge.fury.io/py/attributee.svg)](https://badge.fury.io/py/attributee)
 
 Attributee is a Python 3 library for declarative object initialization. Input arguments are defined as class attributes and are automatically processed when creating an object. It is in a way similar to Django ORM or some other ORMs, but the main purpose of this library is to simplify parsing input arguments to object constructors. 
 
 The library is a work-in-progress, I am adding stuff that I consider useful for my other projects.
 
 Simple use case
----------------
+===============
 
 ```
 from attributee import Attributee, String, Float
 
 class Model(Attributee):
 
     # Simply list the attributes of the object ...
@@ -43,20 +46,21 @@
 
 # automatic type conversion where possible
 model2 = Model(value1=10, value2="5")
 
 ```
 
 Documentation
--------------
+=============
 
 I am working on it.
 
 Authors
--------
+=======
 
 Luka Čehovin Zajc
 
 License
--------
+=======
 
 The library is available under the [simplified BSD license](LICENSE.md).
+
```

### Comparing `attributee-0.1.8/setup.py` & `attributee-0.1.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 install_requires = []
 if isfile(join(this_directory, "requirements.txt")):
     with open(join(this_directory, "requirements.txt"), encoding='utf-8') as f:
         install_requires = f.readlines()
 
 setup(name='attributee',
-    version="0.1.8",
+    version="0.1.9",
     description='Declarative object initialization library',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='Luka Cehovin Zajc',
     author_email='luka.cehovin@gmail.com',
     url='https://github.com/lukacu/attributee',
     packages=find_packages(),
```

