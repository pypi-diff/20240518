# Comparing `tmp/pyqt5_concurrent-0.1.3.tar.gz` & `tmp/pyqt5_concurrent-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyqt5_concurrent-0.1.3.tar", last modified: Sun Apr 14 06:25:16 2024, max compression
+gzip compressed data, was "pyqt5_concurrent-0.1.4.tar", last modified: Sat May 18 14:11:31 2024, max compression
```

## Comparing `pyqt5_concurrent-0.1.3.tar` & `pyqt5_concurrent-0.1.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     5963 2024-04-14 06:25:00.974014 pyqt5_concurrent-0.1.3/README.md
--rw-r--r--   0        0        0      391 2024-04-14 06:25:16.937965 pyqt5_concurrent-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     8649 2024-04-14 06:25:00.974014 pyqt5_concurrent-0.1.3/src/pyqt5_concurrent/Future.py
--rw-r--r--   0        0        0      920 2024-04-14 06:25:00.974014 pyqt5_concurrent-0.1.3/src/pyqt5_concurrent/Qt.py
--rw-r--r--   0        0        0     2466 2024-04-14 06:25:00.974014 pyqt5_concurrent-0.1.3/src/pyqt5_concurrent/Task.py
--rw-r--r--   0        0        0     5967 2024-04-14 06:25:00.974014 pyqt5_concurrent-0.1.3/src/pyqt5_concurrent/TaskExecutor.py
--rw-r--r--   0        0        0        0 2024-04-14 06:25:00.974014 pyqt5_concurrent-0.1.3/src/pyqt5_concurrent/__init__.py
--rw-r--r--   0        0        0        0 2024-04-14 06:25:00.974014 pyqt5_concurrent-0.1.3/tests/__init__.py
--rw-r--r--   0        0        0      735 2024-04-14 06:25:00.974014 pyqt5_concurrent-0.1.3/tests/concurrent_sync_test.py
--rw-r--r--   0        0        0     1616 2024-04-14 06:25:00.974014 pyqt5_concurrent-0.1.3/tests/concurrent_test.py
--rw-r--r--   0        0        0     1061 2024-04-14 06:25:00.974014 pyqt5_concurrent-0.1.3/tests/future_cancel_test.py
--rw-r--r--   0        0        0      672 2024-04-14 06:25:00.974014 pyqt5_concurrent-0.1.3/tests/priority_test.py
--rw-r--r--   0        0        0     1026 2024-04-14 06:25:00.974014 pyqt5_concurrent-0.1.3/tests/qt.py
--rw-r--r--   0        0        0      770 2024-04-14 06:25:00.974014 pyqt5_concurrent-0.1.3/tests/task_error_test.py
--rw-r--r--   0        0        0     6218 1970-01-01 00:00:00.000000 pyqt5_concurrent-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     5963 2024-05-18 14:11:09.106145 pyqt5_concurrent-0.1.4/README.md
+-rw-r--r--   0        0        0      391 2024-05-18 14:11:31.378316 pyqt5_concurrent-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     8649 2024-05-18 14:11:09.106145 pyqt5_concurrent-0.1.4/src/pyqt5_concurrent/Future.py
+-rw-r--r--   0        0        0      920 2024-05-18 14:11:09.106145 pyqt5_concurrent-0.1.4/src/pyqt5_concurrent/Qt.py
+-rw-r--r--   0        0        0     2466 2024-05-18 14:11:09.106145 pyqt5_concurrent-0.1.4/src/pyqt5_concurrent/Task.py
+-rw-r--r--   0        0        0     5967 2024-05-18 14:11:09.106145 pyqt5_concurrent-0.1.4/src/pyqt5_concurrent/TaskExecutor.py
+-rw-r--r--   0        0        0        0 2024-05-18 14:11:09.106145 pyqt5_concurrent-0.1.4/src/pyqt5_concurrent/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-18 14:11:09.106145 pyqt5_concurrent-0.1.4/tests/__init__.py
+-rw-r--r--   0        0        0      735 2024-05-18 14:11:09.106145 pyqt5_concurrent-0.1.4/tests/concurrent_sync_test.py
+-rw-r--r--   0        0        0     1616 2024-05-18 14:11:09.106145 pyqt5_concurrent-0.1.4/tests/concurrent_test.py
+-rw-r--r--   0        0        0     1061 2024-05-18 14:11:09.106145 pyqt5_concurrent-0.1.4/tests/future_cancel_test.py
+-rw-r--r--   0        0        0      672 2024-05-18 14:11:09.106145 pyqt5_concurrent-0.1.4/tests/priority_test.py
+-rw-r--r--   0        0        0     1104 2024-05-18 14:11:09.106145 pyqt5_concurrent-0.1.4/tests/qt.py
+-rw-r--r--   0        0        0      770 2024-05-18 14:11:09.106145 pyqt5_concurrent-0.1.4/tests/task_error_test.py
+-rw-r--r--   0        0        0     6218 1970-01-01 00:00:00.000000 pyqt5_concurrent-0.1.4/PKG-INFO
```

### Comparing `pyqt5_concurrent-0.1.3/README.md` & `pyqt5_concurrent-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `pyqt5_concurrent-0.1.3/src/pyqt5_concurrent/Future.py` & `pyqt5_concurrent-0.1.4/src/pyqt5_concurrent/Future.py`

 * *Files identical despite different names*

### Comparing `pyqt5_concurrent-0.1.3/src/pyqt5_concurrent/Qt.py` & `pyqt5_concurrent-0.1.4/src/pyqt5_concurrent/Qt.py`

 * *Files identical despite different names*

### Comparing `pyqt5_concurrent-0.1.3/src/pyqt5_concurrent/Task.py` & `pyqt5_concurrent-0.1.4/src/pyqt5_concurrent/Task.py`

 * *Files identical despite different names*

### Comparing `pyqt5_concurrent-0.1.3/src/pyqt5_concurrent/TaskExecutor.py` & `pyqt5_concurrent-0.1.4/src/pyqt5_concurrent/TaskExecutor.py`

 * *Files identical despite different names*

### Comparing `pyqt5_concurrent-0.1.3/tests/concurrent_sync_test.py` & `pyqt5_concurrent-0.1.4/tests/concurrent_sync_test.py`

 * *Files identical despite different names*

### Comparing `pyqt5_concurrent-0.1.3/tests/concurrent_test.py` & `pyqt5_concurrent-0.1.4/tests/concurrent_test.py`

 * *Files identical despite different names*

### Comparing `pyqt5_concurrent-0.1.3/tests/future_cancel_test.py` & `pyqt5_concurrent-0.1.4/tests/future_cancel_test.py`

 * *Files identical despite different names*

### Comparing `pyqt5_concurrent-0.1.3/tests/priority_test.py` & `pyqt5_concurrent-0.1.4/tests/priority_test.py`

 * *Files identical despite different names*

### Comparing `pyqt5_concurrent-0.1.3/tests/qt.py` & `pyqt5_concurrent-0.1.4/tests/qt.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,16 +3,19 @@
 QT_BINDINGS = None
 
 qt_bindings = ["PySide6.QtCore", "PyQt6.QtCore", "PySide2.QtCore", "PyQt5.QtCore"]
 
 
 def find_qt_bindings():
     for binding in qt_bindings:
-        if importlib.util.find_spec(binding) is not None:
-            return binding
+        try:
+            if importlib.util.find_spec(binding) is not None:
+                return binding
+        except ModuleNotFoundError:
+            continue
     raise ModuleNotFoundError("No python Qt bindings found.")
 
 
 qt_binding = find_qt_bindings()
 QT_BINDINGS = qt_binding.split(".")[0]
```

### Comparing `pyqt5_concurrent-0.1.3/tests/task_error_test.py` & `pyqt5_concurrent-0.1.4/tests/task_error_test.py`

 * *Files identical despite different names*

### Comparing `pyqt5_concurrent-0.1.3/PKG-INFO` & `pyqt5_concurrent-0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyqt5-concurrent
-Version: 0.1.3
+Version: 0.1.4
 Summary: QThreadPool based task concurrency library in pyqt5
 Author-Email: AresConnor <aresconnor867@gmail.com>
 License: MIT
 Requires-Python: <3.13,>=3.7
 Description-Content-Type: text/markdown
 
 # PyQt5-Concurrent
```

