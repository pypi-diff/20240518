# Comparing `tmp/decorator_retry-0.1.5.tar.gz` & `tmp/decorator_retry-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "decorator_retry-0.1.5.tar", max compression
+gzip compressed data, was "decorator_retry-0.1.6.tar", max compression
```

## Comparing `decorator_retry-0.1.5.tar` & `decorator_retry-0.1.6.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0      980 2023-10-06 13:34:26.318166 decorator_retry-0.1.5/README.md
--rw-r--r--   0        0        0     2350 2023-10-06 13:35:07.466730 decorator_retry-0.1.5/decorator_retry/__init__.py
--rw-r--r--   0        0        0      535 2023-10-06 12:08:23.430016 decorator_retry-0.1.5/pyproject.toml
--rw-r--r--   0        0        0     1324 1970-01-01 00:00:00.000000 decorator_retry-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0      980 2023-10-06 13:34:26.318166 decorator_retry-0.1.6/README.md
+-rw-r--r--   0        0        0     2518 2024-05-17 10:11:17.507600 decorator_retry-0.1.6/decorator_retry/__init__.py
+-rw-r--r--   0        0        0      564 2024-05-17 10:12:33.864837 decorator_retry-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0     1474 1970-01-01 00:00:00.000000 decorator_retry-0.1.6/PKG-INFO
```

### Comparing `decorator_retry-0.1.5/README.md` & `decorator_retry-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `decorator_retry-0.1.5/decorator_retry/__init__.py` & `decorator_retry-0.1.6/decorator_retry/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,19 @@
-import logging
+import sys
 import time
+import logging
 from typing import Callable, TypeVar, Type
 from typing import ParamSpec
 
+if sys.version_info >= (3, 10):  # pragma: no cover
+    from typing import ParamSpec
+else:  # pragma: no cover
+    from typing_extensions import ParamSpec
+
+
 P = ParamSpec('P')
 R = TypeVar('R')
 OF = Callable[P, R]
 DF = Callable[P, None | R]
 
 
 def retry(*exceptions: Type[Exception],
```

### Comparing `decorator_retry-0.1.5/pyproject.toml` & `decorator_retry-0.1.6/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 [tool.poetry]
 name = "decorator-retry"
-version = "0.1.5"
+version = "0.1.6"
 description = ""
 authors = ["Yibo Mao <yibo.mao@genscript.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
-python = "^3.10"
+python = "^3.8"
+typing-extensions = "^4.11.0"
 
 
 [[tool.poetry.source]]
 name = "aliyun"
 url = "https://mirrors.aliyun.com/pypi/simple/"
 priority = "primary"
```

### Comparing `decorator_retry-0.1.5/PKG-INFO` & `decorator_retry-0.1.6/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,20 @@
 Metadata-Version: 2.1
 Name: decorator-retry
-Version: 0.1.5
+Version: 0.1.6
 Summary: 
 Author: Yibo Mao
 Author-email: yibo.mao@genscript.com
-Requires-Python: >=3.10,<4.0
+Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: typing-extensions (>=4.11.0,<5.0.0)
 Description-Content-Type: text/markdown
 
 # A simple decorator for retry functions  
 
 ```python
 @retry(ValueError, KeyError,
          retry = True,
```

