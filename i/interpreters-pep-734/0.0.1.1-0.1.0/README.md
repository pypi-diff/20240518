# Comparing `tmp/interpreters_pep_734-0.0.1.1.tar.gz` & `tmp/interpreters_pep_734-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "interpreters_pep_734-0.0.1.1.tar", last modified: Thu Apr 11 22:08:42 2024, max compression
+gzip compressed data, was "interpreters_pep_734-0.1.0.tar", last modified: Sat May 18 11:54:11 2024, max compression
```

## Comparing `interpreters_pep_734-0.0.1.1.tar` & `interpreters_pep_734-0.1.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 esnow     (1000) esnow     (1000)        0 2024-04-11 22:08:42.923631 interpreters_pep_734-0.0.1.1/
--rw-rw-r--   0 esnow     (1000) esnow     (1000)     1298 2023-12-18 22:41:56.000000 interpreters_pep_734-0.0.1.1/LICENSE
--rw-r--r--   0 esnow     (1000) esnow     (1000)     1966 2024-04-11 22:08:42.923631 interpreters_pep_734-0.0.1.1/PKG-INFO
--rw-rw-r--   0 esnow     (1000) esnow     (1000)     1315 2024-01-18 00:03:36.000000 interpreters_pep_734-0.0.1.1/README.md
--rw-rw-r--   0 esnow     (1000) esnow     (1000)     1393 2024-04-11 22:08:38.000000 interpreters_pep_734-0.0.1.1/pyproject.toml
--rw-rw-r--   0 esnow     (1000) esnow     (1000)       38 2024-04-11 22:08:42.923631 interpreters_pep_734-0.0.1.1/setup.cfg
-drwxrwxr-x   0 esnow     (1000) esnow     (1000)        0 2024-04-11 22:08:42.919631 interpreters_pep_734-0.0.1.1/src/
-drwxrwxr-x   0 esnow     (1000) esnow     (1000)        0 2024-04-11 22:08:42.919631 interpreters_pep_734-0.0.1.1/src/interpreters/
--rw-rw-r--   0 esnow     (1000) esnow     (1000)     6310 2024-04-11 22:03:35.000000 interpreters_pep_734-0.0.1.1/src/interpreters/__init__.py
--rw-rw-r--   0 esnow     (1000) esnow     (1000)     5153 2024-04-11 22:03:35.000000 interpreters_pep_734-0.0.1.1/src/interpreters/channels.py
--rw-rw-r--   0 esnow     (1000) esnow     (1000)     6539 2024-04-11 22:03:35.000000 interpreters_pep_734-0.0.1.1/src/interpreters/queues.py
-drwxrwxr-x   0 esnow     (1000) esnow     (1000)        0 2024-04-11 22:08:42.923631 interpreters_pep_734-0.0.1.1/src/interpreters_pep_734.egg-info/
--rw-r--r--   0 esnow     (1000) esnow     (1000)     1966 2024-04-11 22:08:42.000000 interpreters_pep_734-0.0.1.1/src/interpreters_pep_734.egg-info/PKG-INFO
--rw-rw-r--   0 esnow     (1000) esnow     (1000)      309 2024-04-11 22:08:42.000000 interpreters_pep_734-0.0.1.1/src/interpreters_pep_734.egg-info/SOURCES.txt
--rw-rw-r--   0 esnow     (1000) esnow     (1000)        1 2024-04-11 22:08:42.000000 interpreters_pep_734-0.0.1.1/src/interpreters_pep_734.egg-info/dependency_links.txt
--rw-rw-r--   0 esnow     (1000) esnow     (1000)       13 2024-04-11 22:08:42.000000 interpreters_pep_734-0.0.1.1/src/interpreters_pep_734.egg-info/top_level.txt
+drwxrwxr-x   0 esnow     (1000) esnow     (1000)        0 2024-05-18 11:54:11.552497 interpreters_pep_734-0.1.0/
+-rw-rw-r--   0 esnow     (1000) esnow     (1000)     1298 2023-04-19 20:43:12.000000 interpreters_pep_734-0.1.0/LICENSE
+-rw-r--r--   0 esnow     (1000) esnow     (1000)      778 2024-05-18 11:54:11.552497 interpreters_pep_734-0.1.0/PKG-INFO
+-rw-rw-r--   0 esnow     (1000) esnow     (1000)      125 2024-05-18 11:23:59.000000 interpreters_pep_734-0.1.0/README.md
+-rw-rw-r--   0 esnow     (1000) esnow     (1000)     1395 2024-05-18 11:31:15.000000 interpreters_pep_734-0.1.0/pyproject.toml
+-rw-rw-r--   0 esnow     (1000) esnow     (1000)       38 2024-05-18 11:54:11.552497 interpreters_pep_734-0.1.0/setup.cfg
+drwxrwxr-x   0 esnow     (1000) esnow     (1000)        0 2024-05-18 11:54:11.548497 interpreters_pep_734-0.1.0/src/
+drwxrwxr-x   0 esnow     (1000) esnow     (1000)        0 2024-05-18 11:54:11.552497 interpreters_pep_734-0.1.0/src/interpreters/
+-rw-rw-r--   0 esnow     (1000) esnow     (1000)     7673 2024-05-18 11:38:55.000000 interpreters_pep_734-0.1.0/src/interpreters/__init__.py
+-rw-rw-r--   0 esnow     (1000) esnow     (1000)     5149 2024-05-18 11:39:17.000000 interpreters_pep_734-0.1.0/src/interpreters/channels.py
+-rw-rw-r--   0 esnow     (1000) esnow     (1000)     6535 2024-05-18 11:39:24.000000 interpreters_pep_734-0.1.0/src/interpreters/queues.py
+drwxrwxr-x   0 esnow     (1000) esnow     (1000)        0 2024-05-18 11:54:11.552497 interpreters_pep_734-0.1.0/src/interpreters_pep_734.egg-info/
+-rw-r--r--   0 esnow     (1000) esnow     (1000)      778 2024-05-18 11:54:11.000000 interpreters_pep_734-0.1.0/src/interpreters_pep_734.egg-info/PKG-INFO
+-rw-rw-r--   0 esnow     (1000) esnow     (1000)      309 2024-05-18 11:54:11.000000 interpreters_pep_734-0.1.0/src/interpreters_pep_734.egg-info/SOURCES.txt
+-rw-rw-r--   0 esnow     (1000) esnow     (1000)        1 2024-05-18 11:54:11.000000 interpreters_pep_734-0.1.0/src/interpreters_pep_734.egg-info/dependency_links.txt
+-rw-rw-r--   0 esnow     (1000) esnow     (1000)       13 2024-05-18 11:54:11.000000 interpreters_pep_734-0.1.0/src/interpreters_pep_734.egg-info/top_level.txt
```

### Comparing `interpreters_pep_734-0.0.1.1/LICENSE` & `interpreters_pep_734-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `interpreters_pep_734-0.0.1.1/pyproject.toml` & `interpreters_pep_734-0.1.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 [build-system]
 # We use setuptools because hatchling doesn't build extension modules.
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "interpreters_pep_734"
-version = "0.0.1.1"
+version = "0.1.0"
 authors = [
   { name="Eric Snow", email="ericsnowcurrently@gmail.com" },
 ]
-description = "Use this module to try out multiple interpreters and a per-interpreter GIL in Python 3.12+.  Do not use this for anything important."
+description = "Use this module to try out multiple interpreters and a per-interpreter GIL in Python 3.13+.  Do not use this for anything important yet."
 readme = "README.md"
-requires-python = ">=3.12"
+requires-python = ">=3.13"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: BSD License",
     "Operating System :: OS Independent",
 ]
 
 [project.urls]
```

### Comparing `interpreters_pep_734-0.0.1.1/src/interpreters/__init__.py` & `interpreters_pep_734-0.1.0/src/interpreters/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Subinterpreters High Level Module."""
 
 import threading
 import weakref
-import _xxsubinterpreters as _interpreters
+import _interpreters
 
 # aliases:
-from _xxsubinterpreters import (
+from _interpreters import (
     InterpreterError, InterpreterNotFoundError, NotShareableError,
     is_shareable,
 )
 
 
 __all__ = [
     'get_current', 'get_main', 'create', 'list_all', 'is_shareable',
@@ -70,59 +70,85 @@
                 formatted=formatted,
             )
 
 
 def create():
     """Return a new (idle) Python interpreter."""
     id = _interpreters.create(reqrefs=True)
-    return Interpreter(id)
+    return Interpreter(id, _ownsref=True)
 
 
 def list_all():
     """Return all existing interpreters."""
-    return [Interpreter(id)
-            for id, in _interpreters.list_all()]
+    return [Interpreter(id, _whence=whence)
+            for id, whence in _interpreters.list_all(require_ready=True)]
 
 
 def get_current():
     """Return the currently running interpreter."""
-    id, = _interpreters.get_current()
-    return Interpreter(id)
+    id, whence = _interpreters.get_current()
+    return Interpreter(id, _whence=whence)
 
 
 def get_main():
     """Return the main interpreter."""
-    id, = _interpreters.get_main()
-    return Interpreter(id)
+    id, whence = _interpreters.get_main()
+    assert whence == _interpreters.WHENCE_RUNTIME, repr(whence)
+    return Interpreter(id, _whence=whence)
 
 
 _known = weakref.WeakValueDictionary()
 
 class Interpreter:
-    """A single Python interpreter."""
+    """A single Python interpreter.
 
-    def __new__(cls, id, /):
+    Attributes:
+
+    "id" - the unique process-global ID number for the interpreter
+    "whence" - indicates where the interpreter was created
+
+    If the interpreter wasn't created by this module
+    then any method that modifies the interpreter will fail,
+    i.e. .close(), .prepare_main(), .exec(), and .call()
+    """
+
+    _WHENCE_TO_STR = {
+       _interpreters.WHENCE_UNKNOWN: 'unknown',
+       _interpreters.WHENCE_RUNTIME: 'runtime init',
+       _interpreters.WHENCE_LEGACY_CAPI: 'legacy C-API',
+       _interpreters.WHENCE_CAPI: 'C-API',
+       _interpreters.WHENCE_XI: 'cross-interpreter C-API',
+       _interpreters.WHENCE_STDLIB: '_interpreters module',
+    }
+
+    def __new__(cls, id, /, _whence=None, _ownsref=None):
         # There is only one instance for any given ID.
         if not isinstance(id, int):
             raise TypeError(f'id must be an int, got {id!r}')
         id = int(id)
+        if _whence is None:
+            if _ownsref:
+                _whence = _interpreters.WHENCE_STDLIB
+            else:
+                _whence = _interpreters.whence(id)
+        assert _whence in cls._WHENCE_TO_STR, repr(_whence)
+        if _ownsref is None:
+            _ownsref = (_whence == _interpreters.WHENCE_STDLIB)
         try:
             self = _known[id]
             assert hasattr(self, '_ownsref')
         except KeyError:
-            # This may raise InterpreterNotFoundError:
-            _interpreters.incref(id)
-            try:
-                self = super().__new__(cls)
-                self._id = id
-                self._ownsref = True
-            except BaseException:
-                _interpreters.decref(id)
-                raise
+            self = super().__new__(cls)
             _known[id] = self
+            self._id = id
+            self._whence = _whence
+            self._ownsref = _ownsref
+            if _ownsref:
+                # This may raise InterpreterNotFoundError:
+                _interpreters.incref(id)
         return self
 
     def __repr__(self):
         return f'{type(self).__name__}({self.id})'
 
     def __hash__(self):
         return hash(self._id)
@@ -139,41 +165,48 @@
         return None
 
     def _decref(self):
         if not self._ownsref:
             return
         self._ownsref = False
         try:
-            _interpreters.decref(self.id)
+            _interpreters.decref(self._id)
         except InterpreterNotFoundError:
             pass
 
     @property
     def id(self):
         return self._id
 
+    @property
+    def whence(self):
+        return self._WHENCE_TO_STR[self._whence]
+
     def is_running(self):
         """Return whether or not the identified interpreter is running."""
         return _interpreters.is_running(self._id)
 
+    # Everything past here is available only to interpreters created by
+    # interpreters.create().
+
     def close(self):
         """Finalize and destroy the interpreter.
 
         Attempting to destroy the current interpreter results
         in an InterpreterError.
         """
-        return _interpreters.destroy(self._id)
+        return _interpreters.destroy(self._id, restrict=True)
 
     def prepare_main(self, ns=None, /, **kwargs):
         """Bind the given values into the interpreter's __main__.
 
         The values must be shareable.
         """
         ns = dict(ns, **kwargs) if ns is not None else kwargs
-        _interpreters.set___main___attrs(self._id, ns)
+        _interpreters.set___main___attrs(self._id, ns, restrict=True)
 
     def exec(self, code, /):
         """Run the given source code in the interpreter.
 
         This is essentially the same as calling the builtin "exec"
         with this interpreter, using the __dict__ of its __main__
         module as both globals and locals.
@@ -185,15 +218,15 @@
         The actual exception is discarded because objects cannot be
         shared between interpreters.
 
         This blocks the current Python thread until done.  During
         that time, the previous interpreter is allowed to run
         in other threads.
         """
-        excinfo = _interpreters.exec(self._id, code)
+        excinfo = _interpreters.exec(self._id, code, restrict=True)
         if excinfo is not None:
             raise ExecutionFailed(excinfo)
 
     def call(self, callable, /):
         """Call the object in the interpreter with given args/kwargs.
 
         Only functions that take no arguments and have no closure
@@ -205,15 +238,15 @@
         (including full traceback) is send back between the interpreters
         and an ExecutionFailed exception is raised, much like what
         happens with Interpreter.exec().
         """
         # XXX Support args and kwargs.
         # XXX Support arbitrary callables.
         # XXX Support returning the return value (e.g. via pickle).
-        excinfo = _interpreters.call(self._id, callable)
+        excinfo = _interpreters.call(self._id, callable, restrict=True)
         if excinfo is not None:
             raise ExecutionFailed(excinfo)
 
     def call_in_thread(self, callable, /):
         """Return a new thread that calls the object in the interpreter.
 
         The return value and any raised exception are discarded.
```

### Comparing `interpreters_pep_734-0.0.1.1/src/interpreters/channels.py` & `interpreters_pep_734-0.1.0/src/interpreters/channels.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """Cross-interpreter Channels High Level Module."""
 
 import time
-import _xxinterpchannels as _channels
+import _interpchannels as _channels
 
 # aliases:
-from _xxinterpchannels import (
+from _interpchannels import (
     ChannelError, ChannelNotFoundError, ChannelClosedError,
     ChannelEmptyError, ChannelNotEmptyError,
 )
 
 
 __all__ = [
     'create', 'list_all',
```

### Comparing `interpreters_pep_734-0.0.1.1/src/interpreters/queues.py` & `interpreters_pep_734-0.1.0/src/interpreters/queues.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 """Cross-interpreter Queues High Level Module."""
 
 import pickle
 import queue
 import time
 import weakref
-import _xxinterpqueues as _queues
+import _interpqueues as _queues
 
 # aliases:
-from _xxinterpqueues import (
+from _interpqueues import (
     QueueError, QueueNotFoundError,
 )
 
 __all__ = [
     'create', 'list_all',
     'Queue',
     'QueueError', 'QueueNotFoundError', 'QueueEmpty', 'QueueFull',
```

