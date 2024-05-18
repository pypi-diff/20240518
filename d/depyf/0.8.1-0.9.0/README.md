# Comparing `tmp/depyf-0.8.1.tar.gz` & `tmp/depyf-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "depyf-0.8.1.tar", last modified: Wed Oct 18 09:04:43 2023, max compression
+gzip compressed data, was "depyf-0.9.0.tar", last modified: Sun Oct 22 09:13:50 2023, max compression
```

## Comparing `depyf-0.8.1.tar` & `depyf-0.9.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 youkaichao   (501) staff       (20)        0 2023-10-18 09:04:43.572082 depyf-0.8.1/
--rw-r--r--   0 youkaichao   (501) staff       (20)     1067 2023-08-28 04:06:29.000000 depyf-0.8.1/LICENSE
--rw-r--r--   0 youkaichao   (501) staff       (20)       26 2023-10-18 00:44:03.000000 depyf-0.8.1/MANIFEST.in
--rw-r--r--   0 youkaichao   (501) staff       (20)    11770 2023-10-18 09:04:43.571829 depyf-0.8.1/PKG-INFO
--rw-r--r--   0 youkaichao   (501) staff       (20)    11438 2023-10-18 07:47:08.000000 depyf-0.8.1/README.md
-drwxr-xr-x   0 youkaichao   (501) staff       (20)        0 2023-10-18 09:04:43.569440 depyf-0.8.1/depyf/
--rw-r--r--   0 youkaichao   (501) staff       (20)        5 2023-10-18 09:02:08.000000 depyf-0.8.1/depyf/VERSION.txt
--rw-r--r--   0 youkaichao   (501) staff       (20)     1460 2023-10-17 08:46:19.000000 depyf-0.8.1/depyf/__init__.py
--rw-r--r--   0 youkaichao   (501) staff       (20)    10910 2023-10-06 01:18:00.000000 depyf-0.8.1/depyf/code_transform.py
--rw-r--r--   0 youkaichao   (501) staff       (20)    39532 2023-10-09 22:58:05.000000 depyf-0.8.1/depyf/decompiler.py
-drwxr-xr-x   0 youkaichao   (501) staff       (20)        0 2023-10-18 09:04:43.570765 depyf-0.8.1/depyf/explain/
--rw-r--r--   0 youkaichao   (501) staff       (20)      582 2023-10-18 06:42:40.000000 depyf-0.8.1/depyf/explain/__init__.py
--rw-r--r--   0 youkaichao   (501) staff       (20)     7446 2023-10-18 06:42:25.000000 depyf-0.8.1/depyf/explain/utils.py
--rw-r--r--   0 youkaichao   (501) staff       (20)     2368 2023-10-05 05:06:05.000000 depyf-0.8.1/depyf/utils.py
-drwxr-xr-x   0 youkaichao   (501) staff       (20)        0 2023-10-18 09:04:43.570326 depyf-0.8.1/depyf.egg-info/
--rw-r--r--   0 youkaichao   (501) staff       (20)    11770 2023-10-18 09:04:43.000000 depyf-0.8.1/depyf.egg-info/PKG-INFO
--rw-r--r--   0 youkaichao   (501) staff       (20)      363 2023-10-18 09:04:43.000000 depyf-0.8.1/depyf.egg-info/SOURCES.txt
--rw-r--r--   0 youkaichao   (501) staff       (20)        1 2023-10-18 09:04:43.000000 depyf-0.8.1/depyf.egg-info/dependency_links.txt
--rw-r--r--   0 youkaichao   (501) staff       (20)       20 2023-10-18 09:04:43.000000 depyf-0.8.1/depyf.egg-info/requires.txt
--rw-r--r--   0 youkaichao   (501) staff       (20)        6 2023-10-18 09:04:43.000000 depyf-0.8.1/depyf.egg-info/top_level.txt
--rw-r--r--   0 youkaichao   (501) staff       (20)       38 2023-10-18 09:04:43.572122 depyf-0.8.1/setup.cfg
--rw-r--r--   0 youkaichao   (501) staff       (20)      673 2023-10-18 09:02:02.000000 depyf-0.8.1/setup.py
-drwxr-xr-x   0 youkaichao   (501) staff       (20)        0 2023-10-18 09:04:43.571465 depyf-0.8.1/tests/
--rw-r--r--   0 youkaichao   (501) staff       (20)    21047 2023-10-09 22:33:41.000000 depyf-0.8.1/tests/test.py
--rw-r--r--   0 youkaichao   (501) staff       (20)     1714 2023-10-05 07:51:44.000000 depyf-0.8.1/tests/test_advanced.py
+drwxr-xr-x   0 youkaichao   (501) staff       (20)        0 2023-10-22 09:13:50.463765 depyf-0.9.0/
+-rw-r--r--   0 youkaichao   (501) staff       (20)     1067 2023-08-28 04:06:29.000000 depyf-0.9.0/LICENSE
+-rw-r--r--   0 youkaichao   (501) staff       (20)       26 2023-10-18 00:44:03.000000 depyf-0.9.0/MANIFEST.in
+-rw-r--r--   0 youkaichao   (501) staff       (20)    13092 2023-10-22 09:13:50.463567 depyf-0.9.0/PKG-INFO
+-rw-r--r--   0 youkaichao   (501) staff       (20)    12760 2023-10-22 08:48:06.000000 depyf-0.9.0/README.md
+drwxr-xr-x   0 youkaichao   (501) staff       (20)        0 2023-10-22 09:13:50.461079 depyf-0.9.0/depyf/
+-rw-r--r--   0 youkaichao   (501) staff       (20)        5 2023-10-22 09:12:16.000000 depyf-0.9.0/depyf/VERSION.txt
+-rw-r--r--   0 youkaichao   (501) staff       (20)     3276 2023-10-22 06:12:11.000000 depyf-0.9.0/depyf/__init__.py
+-rw-r--r--   0 youkaichao   (501) staff       (20)    11972 2023-10-22 06:12:11.000000 depyf-0.9.0/depyf/code_transform.py
+-rw-r--r--   0 youkaichao   (501) staff       (20)    39532 2023-10-09 22:58:05.000000 depyf-0.9.0/depyf/decompiler.py
+drwxr-xr-x   0 youkaichao   (501) staff       (20)        0 2023-10-22 09:13:50.462358 depyf-0.9.0/depyf/explain/
+-rw-r--r--   0 youkaichao   (501) staff       (20)      582 2023-10-18 06:42:40.000000 depyf-0.9.0/depyf/explain/__init__.py
+-rw-r--r--   0 youkaichao   (501) staff       (20)     8014 2023-10-22 06:12:11.000000 depyf-0.9.0/depyf/explain/utils.py
+-rw-r--r--   0 youkaichao   (501) staff       (20)     2368 2023-10-05 05:06:05.000000 depyf-0.9.0/depyf/utils.py
+drwxr-xr-x   0 youkaichao   (501) staff       (20)        0 2023-10-22 09:13:50.461961 depyf-0.9.0/depyf.egg-info/
+-rw-r--r--   0 youkaichao   (501) staff       (20)    13092 2023-10-22 09:13:50.000000 depyf-0.9.0/depyf.egg-info/PKG-INFO
+-rw-r--r--   0 youkaichao   (501) staff       (20)      363 2023-10-22 09:13:50.000000 depyf-0.9.0/depyf.egg-info/SOURCES.txt
+-rw-r--r--   0 youkaichao   (501) staff       (20)        1 2023-10-22 09:13:50.000000 depyf-0.9.0/depyf.egg-info/dependency_links.txt
+-rw-r--r--   0 youkaichao   (501) staff       (20)       20 2023-10-22 09:13:50.000000 depyf-0.9.0/depyf.egg-info/requires.txt
+-rw-r--r--   0 youkaichao   (501) staff       (20)        6 2023-10-22 09:13:50.000000 depyf-0.9.0/depyf.egg-info/top_level.txt
+-rw-r--r--   0 youkaichao   (501) staff       (20)       38 2023-10-22 09:13:50.463809 depyf-0.9.0/setup.cfg
+-rw-r--r--   0 youkaichao   (501) staff       (20)      673 2023-10-18 09:02:02.000000 depyf-0.9.0/setup.py
+drwxr-xr-x   0 youkaichao   (501) staff       (20)        0 2023-10-22 09:13:50.463135 depyf-0.9.0/tests/
+-rw-r--r--   0 youkaichao   (501) staff       (20)    21047 2023-10-09 22:33:41.000000 depyf-0.9.0/tests/test.py
+-rw-r--r--   0 youkaichao   (501) staff       (20)     1714 2023-10-05 07:51:44.000000 depyf-0.9.0/tests/test_advanced.py
```

### Comparing `depyf-0.8.1/LICENSE` & `depyf-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `depyf-0.8.1/PKG-INFO` & `depyf-0.9.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,27 +1,70 @@
 Metadata-Version: 2.1
 Name: depyf
-Version: 0.8.1
+Version: 0.9.0
 Summary: Decompile python functions, from bytecode to source code!
 Home-page: https://github.com/thuml/depyf
 Author: Kaichao You
 Author-email: youkaichao@gmail.com
 License: MIT
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
-# `torch.compile`, explained!
+# Understand and Deubg `torch.compile`!
 
 Have you ever felt overwhelmed by the complexities of `torch.compile`? Diving into its workings can feel like black magic, with bytecode and Python internal details that many users fail to understand, hindering them from understanding and debugging `torch.compile`.
 
 We are excited to announce `depyf`, a new tool to pull out all the artifacts of `torch.compile`, and to decompile all the bytecode into source code so that every user understands it.
 
-# Example usage:
+# Installation
+
+Stable release: `pip install depyf`
+
+Nightly version (recommended): `pip install git+https://github.com/thuml/depyf.git`
+
+# Usage
+
+<details>
+<summary><h2>Debug <code>torch.compile</code> with your favorite debugger.</h2></summary>
+
+```diff
+import torch
+from torch import _dynamo as torchdynamo
+from typing import List
+
++ @torch.compile(backend="eager")
+- @torch.compile
+def toy_example(a, b):
+    x = a / (torch.abs(a) + 1)
+    if b.sum() < 0:
+        b = b * -1
+    return x * b
+
++ import depyf
++ with depyf.prepare_debug(toy_example, "./dump_src_dir"):
++     # run your code long enough under `depyf.prepare_debug` to prepare all the source code for debugging
++     for _ in range(100):
++         toy_example(torch.randn(10), torch.randn(10))
++ # the program will pause here for you to set breakpoints
++ with depyf.debug():
++     # then you can hit breakpoints when running the function
++     toy_example(torch.randn(10), torch.randn(10))
+- toy_example(torch.randn(10), torch.randn(10))
+```
+
+Run the above program with your favorite debugger, and debug the compiled code as you like. The UI looks like the following:
+
+![](https://raw.githubusercontent.com/thuml/depyf/master/imgs/debug.png)
+
+</details>
+
+<details>
+<summary><h2>Explain <code>torch.compile</code> in source code</h2></summary>
 
 ```diff
 import torch
 + @torch.compile(backend="eager")
 - @torch.compile
 def toy_example(a, b):
     x = a / (torch.abs(a) + 1)
@@ -155,55 +198,29 @@
     return toy_example(a, b)
 
 #============ end of toy_example ============#
 ```
 
 You can explore the code with your favorite IDE. Start from the `toy_example` function, and pay attention to the `compiled_toy_example` function below, walk through all the details of guards/compiled code/compiled subgraph/resume functions. It's all in readable source code format!
 
-# Installation
-
-Stable release: `pip install depyf`
-
-Nightly version (recommended): `pip install git+https://github.com/thuml/depyf.git`
-
-# Other usages:
-
-## General Usage:
-
-`depyf` is a general-purpose tool to decompile Python bytecode into source code.
-
-```python
-# obtain a callable object or codeobject
-def func():
-    print("hello, world!")
-# import the `decompile` function
-from depyf import decompile
-# and decompile it into source code!
-print(decompile(func))
-```
-
-Example output:
+</details>
 
-```python
-def func():
-    print('hello, world!')
-    return None
-```
-
-The output source code is semantically equivalent to the function, but not syntactically the same. It verbosely adds many details that are hidden in the Python code. For example, the above output code explicitly returns `None`, which is typically ignored.
-
-## Interactively explore artifacts of `torch.compile`
+<details>
+<summary><h2>Interactively explore artifacts of <code>torch.compile</code></h2></summary>
 
 Please run the [Jupyter Lab Notebook](https://github.com/thuml/depyf/blob/master/explain_pt2.ipynb).
 
 In the notebook, you can interactively select the content you want to explore. The UI looks like the following:
 
 ![](https://raw.githubusercontent.com/thuml/depyf/master/imgs/ui.png)
 
-## Enhance `torch.compile` logging
+</details>
+
+<details>
+<summary><h2>Enhance <code>torch.compile</code> logging</h2></summary>
 
 `depyf` works closely with PyTorch. If you have a PyTorch program with `torch.compile`, you only need to add a single line to enable the decompilation of PyTorch bytecode.
 
 ```diff
 + import depyf
 + depyf.install()
 from typing import List
@@ -285,14 +302,43 @@
 +     if __temp_1[1]:
 +         return __resume_at_30_1(b, x)
 +     return __resume_at_38_2(b, x)
 + 
 + If you find the decompiled code is wrong,please submit an issue at https://github.com/thuml/depyf/issues.
 ```
 
+</details>
+
+<details>
+<summary><h2>General Usage</h2></summary>
+
+`depyf` is a general-purpose tool to decompile Python bytecode into source code.
+
+```python
+# obtain a callable object or codeobject
+def func():
+    print("hello, world!")
+# import the `decompile` function
+from depyf import decompile
+# and decompile it into source code!
+print(decompile(func))
+```
+
+Example output:
+
+```python
+def func():
+    print('hello, world!')
+    return None
+```
+
+The output source code is semantically equivalent to the function, but not syntactically the same. It verbosely adds many details that are hidden in the Python code. For example, the above output code explicitly returns `None`, which is typically ignored.
+
+</details>
+
 :warning: We recommend running the above examples with PyTorch nightly.
 
 # Python Version Coverage
 
 The following python major versions are tested:
 
 - Python 3.12
```

### Comparing `depyf-0.8.1/README.md` & `depyf-0.9.0/depyf.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,70 @@
-# `torch.compile`, explained!
+Metadata-Version: 2.1
+Name: depyf
+Version: 0.9.0
+Summary: Decompile python functions, from bytecode to source code!
+Home-page: https://github.com/thuml/depyf
+Author: Kaichao You
+Author-email: youkaichao@gmail.com
+License: MIT
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+Provides-Extra: dev
+License-File: LICENSE
+
+# Understand and Deubg `torch.compile`!
 
 Have you ever felt overwhelmed by the complexities of `torch.compile`? Diving into its workings can feel like black magic, with bytecode and Python internal details that many users fail to understand, hindering them from understanding and debugging `torch.compile`.
 
 We are excited to announce `depyf`, a new tool to pull out all the artifacts of `torch.compile`, and to decompile all the bytecode into source code so that every user understands it.
 
-# Example usage:
+# Installation
+
+Stable release: `pip install depyf`
+
+Nightly version (recommended): `pip install git+https://github.com/thuml/depyf.git`
+
+# Usage
+
+<details>
+<summary><h2>Debug <code>torch.compile</code> with your favorite debugger.</h2></summary>
+
+```diff
+import torch
+from torch import _dynamo as torchdynamo
+from typing import List
+
++ @torch.compile(backend="eager")
+- @torch.compile
+def toy_example(a, b):
+    x = a / (torch.abs(a) + 1)
+    if b.sum() < 0:
+        b = b * -1
+    return x * b
+
++ import depyf
++ with depyf.prepare_debug(toy_example, "./dump_src_dir"):
++     # run your code long enough under `depyf.prepare_debug` to prepare all the source code for debugging
++     for _ in range(100):
++         toy_example(torch.randn(10), torch.randn(10))
++ # the program will pause here for you to set breakpoints
++ with depyf.debug():
++     # then you can hit breakpoints when running the function
++     toy_example(torch.randn(10), torch.randn(10))
+- toy_example(torch.randn(10), torch.randn(10))
+```
+
+Run the above program with your favorite debugger, and debug the compiled code as you like. The UI looks like the following:
+
+![](https://raw.githubusercontent.com/thuml/depyf/master/imgs/debug.png)
+
+</details>
+
+<details>
+<summary><h2>Explain <code>torch.compile</code> in source code</h2></summary>
 
 ```diff
 import torch
 + @torch.compile(backend="eager")
 - @torch.compile
 def toy_example(a, b):
     x = a / (torch.abs(a) + 1)
@@ -142,55 +198,29 @@
     return toy_example(a, b)
 
 #============ end of toy_example ============#
 ```
 
 You can explore the code with your favorite IDE. Start from the `toy_example` function, and pay attention to the `compiled_toy_example` function below, walk through all the details of guards/compiled code/compiled subgraph/resume functions. It's all in readable source code format!
 
-# Installation
+</details>
 
-Stable release: `pip install depyf`
-
-Nightly version (recommended): `pip install git+https://github.com/thuml/depyf.git`
-
-# Other usages:
-
-## General Usage:
-
-`depyf` is a general-purpose tool to decompile Python bytecode into source code.
-
-```python
-# obtain a callable object or codeobject
-def func():
-    print("hello, world!")
-# import the `decompile` function
-from depyf import decompile
-# and decompile it into source code!
-print(decompile(func))
-```
-
-Example output:
-
-```python
-def func():
-    print('hello, world!')
-    return None
-```
-
-The output source code is semantically equivalent to the function, but not syntactically the same. It verbosely adds many details that are hidden in the Python code. For example, the above output code explicitly returns `None`, which is typically ignored.
-
-## Interactively explore artifacts of `torch.compile`
+<details>
+<summary><h2>Interactively explore artifacts of <code>torch.compile</code></h2></summary>
 
 Please run the [Jupyter Lab Notebook](https://github.com/thuml/depyf/blob/master/explain_pt2.ipynb).
 
 In the notebook, you can interactively select the content you want to explore. The UI looks like the following:
 
 ![](https://raw.githubusercontent.com/thuml/depyf/master/imgs/ui.png)
 
-## Enhance `torch.compile` logging
+</details>
+
+<details>
+<summary><h2>Enhance <code>torch.compile</code> logging</h2></summary>
 
 `depyf` works closely with PyTorch. If you have a PyTorch program with `torch.compile`, you only need to add a single line to enable the decompilation of PyTorch bytecode.
 
 ```diff
 + import depyf
 + depyf.install()
 from typing import List
@@ -272,14 +302,43 @@
 +     if __temp_1[1]:
 +         return __resume_at_30_1(b, x)
 +     return __resume_at_38_2(b, x)
 + 
 + If you find the decompiled code is wrong,please submit an issue at https://github.com/thuml/depyf/issues.
 ```
 
+</details>
+
+<details>
+<summary><h2>General Usage</h2></summary>
+
+`depyf` is a general-purpose tool to decompile Python bytecode into source code.
+
+```python
+# obtain a callable object or codeobject
+def func():
+    print("hello, world!")
+# import the `decompile` function
+from depyf import decompile
+# and decompile it into source code!
+print(decompile(func))
+```
+
+Example output:
+
+```python
+def func():
+    print('hello, world!')
+    return None
+```
+
+The output source code is semantically equivalent to the function, but not syntactically the same. It verbosely adds many details that are hidden in the Python code. For example, the above output code explicitly returns `None`, which is typically ignored.
+
+</details>
+
 :warning: We recommend running the above examples with PyTorch nightly.
 
 # Python Version Coverage
 
 The following python major versions are tested:
 
 - Python 3.12
```

### Comparing `depyf-0.8.1/depyf/code_transform.py` & `depyf-0.9.0/depyf/code_transform.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 from typing import List, Tuple, Union, Optional, Callable, Any, Dict, Set
 from types import CodeType
 import ast
 import astor
 from collections import defaultdict
 import dataclasses
 import sys
+import hashlib
 
 py311 = sys.version_info >= (3, 11)
 all_jump_opcode_set = set(dis.hasjabs) | set(dis.hasjrel)
 
 
 @dataclasses.dataclass
 class Instruction:
@@ -277,7 +278,38 @@
             can_merge = not isinstance(assignment_parent, indentation_nodes)
             temp_occurrences[key].append(can_merge)
         tree = RemoveAssignmentTransformer(key, temp_occurrences).visit(tree)
         tree = RemoveAssignment2Transformer(key, temp_occurrences).visit(tree)
 
     reconstructed_code = astor.to_source(tree, indent_with=" " * indentation)
     return reconstructed_code
+
+class IdentifierReplacer(ast.NodeTransformer):
+
+    # def visit_Name(self, node):
+    #     return ast.copy_location(ast.Name(id='PLACEHOLDER', ctx=node.ctx), node)
+
+    def visit_FunctionDef(self, node):
+        node.name = 'PLACEHOLDER'
+        return self.generic_visit(node)
+
+    # def visit_AsyncFunctionDef(self, node):
+    #     node.name = 'PLACEHOLDER'
+    #     return self.generic_visit(node)
+
+    # def visit_ClassDef(self, node):
+    #     node.name = 'PLACEHOLDER'
+    #     return self.generic_visit(node)
+
+    # def visit_Attribute(self, node):
+    #     node.attr = 'PLACEHOLDER'
+    #     return self.generic_visit(node)
+
+def structure_hash(source_code: str) -> str:
+    """Compute the hash of code structure, ignore the function name difference.
+    This is because PyTorch dynamically generates function names.
+    """
+    tree = ast.parse(source_code)
+    tree = IdentifierReplacer().visit(tree)
+    modified_code = astor.to_source(tree)
+    hash_value = hashlib.md5(modified_code.encode()).hexdigest()
+    return hash_value
```

### Comparing `depyf-0.8.1/depyf/decompiler.py` & `depyf-0.9.0/depyf/decompiler.py`

 * *Files identical despite different names*

### Comparing `depyf-0.8.1/depyf/explain/__init__.py` & `depyf-0.9.0/depyf/explain/__init__.py`

 * *Files identical despite different names*

### Comparing `depyf-0.8.1/depyf/utils.py` & `depyf-0.9.0/depyf/utils.py`

 * *Files identical despite different names*

### Comparing `depyf-0.8.1/depyf.egg-info/PKG-INFO` & `depyf-0.9.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,27 +1,57 @@
-Metadata-Version: 2.1
-Name: depyf
-Version: 0.8.1
-Summary: Decompile python functions, from bytecode to source code!
-Home-page: https://github.com/thuml/depyf
-Author: Kaichao You
-Author-email: youkaichao@gmail.com
-License: MIT
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-Provides-Extra: dev
-License-File: LICENSE
-
-# `torch.compile`, explained!
+# Understand and Deubg `torch.compile`!
 
 Have you ever felt overwhelmed by the complexities of `torch.compile`? Diving into its workings can feel like black magic, with bytecode and Python internal details that many users fail to understand, hindering them from understanding and debugging `torch.compile`.
 
 We are excited to announce `depyf`, a new tool to pull out all the artifacts of `torch.compile`, and to decompile all the bytecode into source code so that every user understands it.
 
-# Example usage:
+# Installation
+
+Stable release: `pip install depyf`
+
+Nightly version (recommended): `pip install git+https://github.com/thuml/depyf.git`
+
+# Usage
+
+<details>
+<summary><h2>Debug <code>torch.compile</code> with your favorite debugger.</h2></summary>
+
+```diff
+import torch
+from torch import _dynamo as torchdynamo
+from typing import List
+
++ @torch.compile(backend="eager")
+- @torch.compile
+def toy_example(a, b):
+    x = a / (torch.abs(a) + 1)
+    if b.sum() < 0:
+        b = b * -1
+    return x * b
+
++ import depyf
++ with depyf.prepare_debug(toy_example, "./dump_src_dir"):
++     # run your code long enough under `depyf.prepare_debug` to prepare all the source code for debugging
++     for _ in range(100):
++         toy_example(torch.randn(10), torch.randn(10))
++ # the program will pause here for you to set breakpoints
++ with depyf.debug():
++     # then you can hit breakpoints when running the function
++     toy_example(torch.randn(10), torch.randn(10))
+- toy_example(torch.randn(10), torch.randn(10))
+```
+
+Run the above program with your favorite debugger, and debug the compiled code as you like. The UI looks like the following:
+
+![](https://raw.githubusercontent.com/thuml/depyf/master/imgs/debug.png)
+
+</details>
+
+<details>
+<summary><h2>Explain <code>torch.compile</code> in source code</h2></summary>
 
 ```diff
 import torch
 + @torch.compile(backend="eager")
 - @torch.compile
 def toy_example(a, b):
     x = a / (torch.abs(a) + 1)
@@ -155,55 +185,29 @@
     return toy_example(a, b)
 
 #============ end of toy_example ============#
 ```
 
 You can explore the code with your favorite IDE. Start from the `toy_example` function, and pay attention to the `compiled_toy_example` function below, walk through all the details of guards/compiled code/compiled subgraph/resume functions. It's all in readable source code format!
 
-# Installation
+</details>
 
-Stable release: `pip install depyf`
-
-Nightly version (recommended): `pip install git+https://github.com/thuml/depyf.git`
-
-# Other usages:
-
-## General Usage:
-
-`depyf` is a general-purpose tool to decompile Python bytecode into source code.
-
-```python
-# obtain a callable object or codeobject
-def func():
-    print("hello, world!")
-# import the `decompile` function
-from depyf import decompile
-# and decompile it into source code!
-print(decompile(func))
-```
-
-Example output:
-
-```python
-def func():
-    print('hello, world!')
-    return None
-```
-
-The output source code is semantically equivalent to the function, but not syntactically the same. It verbosely adds many details that are hidden in the Python code. For example, the above output code explicitly returns `None`, which is typically ignored.
-
-## Interactively explore artifacts of `torch.compile`
+<details>
+<summary><h2>Interactively explore artifacts of <code>torch.compile</code></h2></summary>
 
 Please run the [Jupyter Lab Notebook](https://github.com/thuml/depyf/blob/master/explain_pt2.ipynb).
 
 In the notebook, you can interactively select the content you want to explore. The UI looks like the following:
 
 ![](https://raw.githubusercontent.com/thuml/depyf/master/imgs/ui.png)
 
-## Enhance `torch.compile` logging
+</details>
+
+<details>
+<summary><h2>Enhance <code>torch.compile</code> logging</h2></summary>
 
 `depyf` works closely with PyTorch. If you have a PyTorch program with `torch.compile`, you only need to add a single line to enable the decompilation of PyTorch bytecode.
 
 ```diff
 + import depyf
 + depyf.install()
 from typing import List
@@ -285,14 +289,43 @@
 +     if __temp_1[1]:
 +         return __resume_at_30_1(b, x)
 +     return __resume_at_38_2(b, x)
 + 
 + If you find the decompiled code is wrong,please submit an issue at https://github.com/thuml/depyf/issues.
 ```
 
+</details>
+
+<details>
+<summary><h2>General Usage</h2></summary>
+
+`depyf` is a general-purpose tool to decompile Python bytecode into source code.
+
+```python
+# obtain a callable object or codeobject
+def func():
+    print("hello, world!")
+# import the `decompile` function
+from depyf import decompile
+# and decompile it into source code!
+print(decompile(func))
+```
+
+Example output:
+
+```python
+def func():
+    print('hello, world!')
+    return None
+```
+
+The output source code is semantically equivalent to the function, but not syntactically the same. It verbosely adds many details that are hidden in the Python code. For example, the above output code explicitly returns `None`, which is typically ignored.
+
+</details>
+
 :warning: We recommend running the above examples with PyTorch nightly.
 
 # Python Version Coverage
 
 The following python major versions are tested:
 
 - Python 3.12
```

### Comparing `depyf-0.8.1/setup.py` & `depyf-0.9.0/setup.py`

 * *Files identical despite different names*

### Comparing `depyf-0.8.1/tests/test.py` & `depyf-0.9.0/tests/test.py`

 * *Files identical despite different names*

### Comparing `depyf-0.8.1/tests/test_advanced.py` & `depyf-0.9.0/tests/test_advanced.py`

 * *Files identical despite different names*

