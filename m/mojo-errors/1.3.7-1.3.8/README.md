# Comparing `tmp/mojo_errors-1.3.7.tar.gz` & `tmp/mojo_errors-1.3.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mojo_errors-1.3.7.tar", max compression
+gzip compressed data, was "mojo_errors-1.3.8.tar", max compression
```

## Comparing `mojo_errors-1.3.7.tar` & `mojo_errors-1.3.8.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1083 2024-01-26 02:55:15.327504 mojo_errors-1.3.7/LICENSE.txt
--rw-r--r--   0        0        0      154 2024-01-29 05:14:53.461749 mojo_errors-1.3.7/README.rst
--rw-r--r--   0        0        0      663 2024-05-05 22:47:35.143495 mojo_errors-1.3.7/pyproject.toml
--rw-r--r--   0        0        0     5105 2024-05-02 02:53:05.622002 mojo_errors-1.3.7/source/packages/mojo/errors/exceptions.py
--rw-r--r--   0        0        0    11609 2024-05-02 02:53:23.372760 mojo_errors-1.3.7/source/packages/mojo/errors/xtraceback.py
--rw-r--r--   0        0        0      751 1970-01-01 00:00:00.000000 mojo_errors-1.3.7/setup.py
--rw-r--r--   0        0        0      739 1970-01-01 00:00:00.000000 mojo_errors-1.3.7/PKG-INFO
+-rw-r--r--   0        0        0     1557 2024-05-14 05:02:15.201200 mojo_errors-1.3.8/LICENSE.txt
+-rw-r--r--   0        0        0      154 2024-01-29 05:14:53.461749 mojo_errors-1.3.8/README.rst
+-rw-r--r--   0        0        0      663 2024-05-18 17:36:01.991513 mojo_errors-1.3.8/pyproject.toml
+-rw-r--r--   0        0        0     5227 2024-05-18 17:35:51.684869 mojo_errors-1.3.8/source/packages/mojo/errors/exceptions.py
+-rw-r--r--   0        0        0    11609 2024-05-02 02:53:23.372760 mojo_errors-1.3.8/source/packages/mojo/errors/xtraceback.py
+-rw-r--r--   0        0        0      751 1970-01-01 00:00:00.000000 mojo_errors-1.3.8/setup.py
+-rw-r--r--   0        0        0      739 1970-01-01 00:00:00.000000 mojo_errors-1.3.8/PKG-INFO
```

### Comparing `mojo_errors-1.3.7/pyproject.toml` & `mojo_errors-1.3.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "mojo-errors"
 description = "Automation Mojo Errors Module"
-version = "1.3.7"
+version = "1.3.8"
 authors = []
 readme = "README.rst"
 license = "LICENSE.txt"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: POSIX"
```

### Comparing `mojo_errors-1.3.7/source/packages/mojo/errors/exceptions.py` & `mojo_errors-1.3.8/source/packages/mojo/errors/exceptions.py`

 * *Files 2% similar despite different names*

```diff
@@ -81,14 +81,19 @@
     """
 
 class NotSupportedError(RuntimeError):
     """
         This error is raised when a method that must be overloaded has not been overridden.
     """
 
+class PublishError(RuntimeError):
+    """
+        This error is raised when the publishing of an artifact fails.
+    """
+
 class SemanticError(BaseException):
     """
         The base error object for errors that indicate that there is an issue with
         a piece of automation code and with the way the Automation Kit code is being
         utilized.
     """
```

### Comparing `mojo_errors-1.3.7/source/packages/mojo/errors/xtraceback.py` & `mojo_errors-1.3.8/source/packages/mojo/errors/xtraceback.py`

 * *Files identical despite different names*

### Comparing `mojo_errors-1.3.7/setup.py` & `mojo_errors-1.3.8/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 ['mojo', 'mojo.errors']
 
 package_data = \
 {'': ['*']}
 
 setup_kwargs = {
     'name': 'mojo-errors',
-    'version': '1.3.7',
+    'version': '1.3.8',
     'description': 'Automation Mojo Errors Module',
     'long_description': '==============================\nAutomation Mojo Errors Package\n==============================\nPython package that provides a common source of error types.\n',
     'author': 'None',
     'author_email': 'None',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `mojo_errors-1.3.7/PKG-INFO` & `mojo_errors-1.3.8/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mojo-errors
-Version: 1.3.7
+Version: 1.3.8
 Summary: Automation Mojo Errors Module
 License: LICENSE.txt
 Keywords: python
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: POSIX
```

