# Comparing `tmp/bdmc-0.1.5.8.tar.gz` & `tmp/bdmc-0.1.5.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bdmc-0.1.5.8.tar", last modified: Fri May 17 16:06:13 2024, max compression
+gzip compressed data, was "bdmc-0.1.5.9.tar", last modified: Sat May 18 15:54:57 2024, max compression
```

## Comparing `bdmc-0.1.5.8.tar` & `bdmc-0.1.5.9.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     5466 2024-05-17 16:05:54.868493 bdmc-0.1.5.8/README.md
--rw-r--r--   0        0        0      547 2024-05-17 16:06:13.764532 bdmc-0.1.5.8/pyproject.toml
--rw-r--r--   0        0        0      556 2024-05-17 16:05:54.868493 bdmc-0.1.5.8/src/bdmc/__init__.py
--rw-r--r--   0        0        0      419 2024-05-17 16:05:54.868493 bdmc-0.1.5.8/src/bdmc/modules/cmd.py
--rw-r--r--   0        0        0    15509 2024-05-17 16:05:54.868493 bdmc-0.1.5.8/src/bdmc/modules/controller.py
--rw-r--r--   0        0        0     2266 2024-05-17 16:05:54.868493 bdmc-0.1.5.8/src/bdmc/modules/debug.py
--rw-r--r--   0        0        0      574 2024-05-17 16:05:54.868493 bdmc-0.1.5.8/src/bdmc/modules/logger.py
--rw-r--r--   0        0        0     1356 2024-05-17 16:05:54.868493 bdmc-0.1.5.8/src/bdmc/modules/port.py
--rw-r--r--   0        0        0     7529 2024-05-17 16:05:54.872493 bdmc-0.1.5.8/src/bdmc/modules/seriald.py
--rw-r--r--   0        0        0      682 2024-05-17 16:05:54.872493 bdmc-0.1.5.8/tests/find_tests.py
--rw-r--r--   0        0        0     4380 2024-05-17 16:05:54.872493 bdmc-0.1.5.8/tests/test_context.py
--rw-r--r--   0        0        0     1989 2024-05-17 16:05:54.872493 bdmc-0.1.5.8/tests/test_controller.py
--rw-r--r--   0        0        0     5782 1970-01-01 00:00:00.000000 bdmc-0.1.5.8/PKG-INFO
+-rw-r--r--   0        0        0     5466 2024-05-18 15:54:39.180903 bdmc-0.1.5.9/README.md
+-rw-r--r--   0        0        0      547 2024-05-18 15:54:57.080996 bdmc-0.1.5.9/pyproject.toml
+-rw-r--r--   0        0        0      556 2024-05-18 15:54:39.180903 bdmc-0.1.5.9/src/bdmc/__init__.py
+-rw-r--r--   0        0        0      419 2024-05-18 15:54:39.180903 bdmc-0.1.5.9/src/bdmc/modules/cmd.py
+-rw-r--r--   0        0        0    15671 2024-05-18 15:54:39.180903 bdmc-0.1.5.9/src/bdmc/modules/controller.py
+-rw-r--r--   0        0        0     2266 2024-05-18 15:54:39.180903 bdmc-0.1.5.9/src/bdmc/modules/debug.py
+-rw-r--r--   0        0        0      574 2024-05-18 15:54:39.180903 bdmc-0.1.5.9/src/bdmc/modules/logger.py
+-rw-r--r--   0        0        0     1356 2024-05-18 15:54:39.180903 bdmc-0.1.5.9/src/bdmc/modules/port.py
+-rw-r--r--   0        0        0     7529 2024-05-18 15:54:39.180903 bdmc-0.1.5.9/src/bdmc/modules/seriald.py
+-rw-r--r--   0        0        0      682 2024-05-18 15:54:39.180903 bdmc-0.1.5.9/tests/find_tests.py
+-rw-r--r--   0        0        0     4380 2024-05-18 15:54:39.180903 bdmc-0.1.5.9/tests/test_context.py
+-rw-r--r--   0        0        0     1989 2024-05-18 15:54:39.180903 bdmc-0.1.5.9/tests/test_controller.py
+-rw-r--r--   0        0        0     5782 1970-01-01 00:00:00.000000 bdmc-0.1.5.9/PKG-INFO
```

### Comparing `bdmc-0.1.5.8/README.md` & `bdmc-0.1.5.9/README.md`

 * *Files identical despite different names*

### Comparing `bdmc-0.1.5.8/pyproject.toml` & `bdmc-0.1.5.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "bdmc"
-version = "0.1.5.8"
+version = "0.1.5.9"
 description = "An api wrapper lib designed for the uptech BDMC divers"
 authors = [
     { name = "Whth", email = "88489697+Whth@users.noreply.github.com" },
 ]
 dependencies = [
     "pyserial>=3.5",
     "coloredlogs>=15.0.1",
```

### Comparing `bdmc-0.1.5.8/src/bdmc/__init__.py` & `bdmc-0.1.5.9/src/bdmc/__init__.py`

 * *Files identical despite different names*

### Comparing `bdmc-0.1.5.8/src/bdmc/modules/controller.py` & `bdmc-0.1.5.9/src/bdmc/modules/controller.py`

 * *Files 1% similar despite different names*

```diff
@@ -241,14 +241,21 @@
     def motor_dirs(self) -> List[DIRECTION]:
         """
         Return the list of directions for each motor in the motor_infos.
         """
         return [motor_info.direction for motor_info in self._motor_infos]
 
     @property
+    def motor_infos(self) -> Sequence[MotorInfo]:
+        """
+        Return the list of motor infos.
+        """
+        return self._motor_infos
+
+    @property
     def cmd_queue(self) -> Queue[ByteString]:
         """
         Return the message queue.
         """
         return self._cmd_queue
 
     @property
```

### Comparing `bdmc-0.1.5.8/src/bdmc/modules/debug.py` & `bdmc-0.1.5.9/src/bdmc/modules/debug.py`

 * *Files identical despite different names*

### Comparing `bdmc-0.1.5.8/src/bdmc/modules/logger.py` & `bdmc-0.1.5.9/src/bdmc/modules/logger.py`

 * *Files identical despite different names*

### Comparing `bdmc-0.1.5.8/src/bdmc/modules/port.py` & `bdmc-0.1.5.9/src/bdmc/modules/port.py`

 * *Files identical despite different names*

### Comparing `bdmc-0.1.5.8/src/bdmc/modules/seriald.py` & `bdmc-0.1.5.9/src/bdmc/modules/seriald.py`

 * *Files identical despite different names*

### Comparing `bdmc-0.1.5.8/tests/find_tests.py` & `bdmc-0.1.5.9/tests/find_tests.py`

 * *Files identical despite different names*

### Comparing `bdmc-0.1.5.8/tests/test_context.py` & `bdmc-0.1.5.9/tests/test_context.py`

 * *Files identical despite different names*

### Comparing `bdmc-0.1.5.8/tests/test_controller.py` & `bdmc-0.1.5.9/tests/test_controller.py`

 * *Files identical despite different names*

### Comparing `bdmc-0.1.5.8/PKG-INFO` & `bdmc-0.1.5.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bdmc
-Version: 0.1.5.8
+Version: 0.1.5.9
 Summary: An api wrapper lib designed for the uptech BDMC divers
 Author-Email: Whth <88489697+Whth@users.noreply.github.com>
 License: MIT
 Requires-Python: >=3.11
 Requires-Dist: pyserial>=3.5
 Requires-Dist: coloredlogs>=15.0.1
 Description-Content-Type: text/markdown
```

