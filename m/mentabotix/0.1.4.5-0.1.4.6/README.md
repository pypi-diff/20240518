# Comparing `tmp/mentabotix-0.1.4.5.tar.gz` & `tmp/mentabotix-0.1.4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mentabotix-0.1.4.5.tar", last modified: Sat May 18 02:30:51 2024, max compression
+gzip compressed data, was "mentabotix-0.1.4.6.tar", last modified: Sat May 18 04:02:35 2024, max compression
```

## Comparing `mentabotix-0.1.4.5.tar` & `mentabotix-0.1.4.6.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0     1066 2024-05-18 02:30:24.927900 mentabotix-0.1.4.5/LICENSE
--rw-r--r--   0        0        0    23799 2024-05-18 02:30:24.927900 mentabotix-0.1.4.5/README.md
--rw-r--r--   0        0        0      680 2024-05-18 02:30:51.928192 mentabotix-0.1.4.5/pyproject.toml
--rw-r--r--   0        0        0     1210 2024-05-18 02:30:24.927900 mentabotix-0.1.4.5/src/mentabotix/__init__.py
--rw-r--r--   0        0        0    70182 2024-05-18 02:30:24.927900 mentabotix-0.1.4.5/src/mentabotix/modules/botix.py
--rw-r--r--   0        0        0      225 2024-05-18 02:30:24.927900 mentabotix-0.1.4.5/src/mentabotix/modules/exceptions.py
--rw-r--r--   0        0        0      580 2024-05-18 02:30:24.927900 mentabotix-0.1.4.5/src/mentabotix/modules/logger.py
--rw-r--r--   0        0        0    21088 2024-05-18 02:30:24.931901 mentabotix-0.1.4.5/src/mentabotix/modules/menta.py
--rw-r--r--   0        0        0     9471 2024-05-18 02:30:24.931901 mentabotix-0.1.4.5/src/mentabotix/tools/composers.py
--rw-r--r--   0        0        0     2292 2024-05-18 02:30:24.931901 mentabotix-0.1.4.5/src/mentabotix/tools/generators.py
--rw-r--r--   0        0        0     9429 2024-05-18 02:30:24.931901 mentabotix-0.1.4.5/src/mentabotix/vision/tagdetector.py
--rw-r--r--   0        0        0        0 2024-05-18 02:30:24.931901 mentabotix-0.1.4.5/tests/__init__.py
--rw-r--r--   0        0        0      682 2024-05-18 02:30:24.931901 mentabotix-0.1.4.5/tests/find_tests.py
--rw-r--r--   0        0        0    15535 2024-05-18 02:30:24.931901 mentabotix-0.1.4.5/tests/test_botix.py
--rw-r--r--   0        0        0    10196 2024-05-18 02:30:24.931901 mentabotix-0.1.4.5/tests/test_composer.py
--rw-r--r--   0        0        0     8998 2024-05-18 02:30:24.931901 mentabotix-0.1.4.5/tests/test_menta.py
--rw-r--r--   0        0        0     7555 2024-05-18 02:30:24.931901 mentabotix-0.1.4.5/tests/test_moving_state.py
--rw-r--r--   0        0        0     5338 2024-05-18 02:30:24.931901 mentabotix-0.1.4.5/tests/test_moving_transition.py
--rw-r--r--   0        0        0    24235 1970-01-01 00:00:00.000000 mentabotix-0.1.4.5/PKG-INFO
+-rw-r--r--   0        0        0     1066 2024-05-18 04:02:10.273050 mentabotix-0.1.4.6/LICENSE
+-rw-r--r--   0        0        0    23799 2024-05-18 04:02:10.277050 mentabotix-0.1.4.6/README.md
+-rw-r--r--   0        0        0      680 2024-05-18 04:02:35.805260 mentabotix-0.1.4.6/pyproject.toml
+-rw-r--r--   0        0        0     1210 2024-05-18 04:02:10.277050 mentabotix-0.1.4.6/src/mentabotix/__init__.py
+-rw-r--r--   0        0        0    70194 2024-05-18 04:02:10.277050 mentabotix-0.1.4.6/src/mentabotix/modules/botix.py
+-rw-r--r--   0        0        0      225 2024-05-18 04:02:10.277050 mentabotix-0.1.4.6/src/mentabotix/modules/exceptions.py
+-rw-r--r--   0        0        0      580 2024-05-18 04:02:10.277050 mentabotix-0.1.4.6/src/mentabotix/modules/logger.py
+-rw-r--r--   0        0        0    21088 2024-05-18 04:02:10.277050 mentabotix-0.1.4.6/src/mentabotix/modules/menta.py
+-rw-r--r--   0        0        0     9471 2024-05-18 04:02:10.277050 mentabotix-0.1.4.6/src/mentabotix/tools/composers.py
+-rw-r--r--   0        0        0     2292 2024-05-18 04:02:10.277050 mentabotix-0.1.4.6/src/mentabotix/tools/generators.py
+-rw-r--r--   0        0        0     9429 2024-05-18 04:02:10.277050 mentabotix-0.1.4.6/src/mentabotix/vision/tagdetector.py
+-rw-r--r--   0        0        0        0 2024-05-18 04:02:10.277050 mentabotix-0.1.4.6/tests/__init__.py
+-rw-r--r--   0        0        0      682 2024-05-18 04:02:10.277050 mentabotix-0.1.4.6/tests/find_tests.py
+-rw-r--r--   0        0        0    15535 2024-05-18 04:02:10.277050 mentabotix-0.1.4.6/tests/test_botix.py
+-rw-r--r--   0        0        0    10196 2024-05-18 04:02:10.277050 mentabotix-0.1.4.6/tests/test_composer.py
+-rw-r--r--   0        0        0     8998 2024-05-18 04:02:10.277050 mentabotix-0.1.4.6/tests/test_menta.py
+-rw-r--r--   0        0        0     7555 2024-05-18 04:02:10.277050 mentabotix-0.1.4.6/tests/test_moving_state.py
+-rw-r--r--   0        0        0     5338 2024-05-18 04:02:10.277050 mentabotix-0.1.4.6/tests/test_moving_transition.py
+-rw-r--r--   0        0        0    24235 1970-01-01 00:00:00.000000 mentabotix-0.1.4.6/PKG-INFO
```

### Comparing `mentabotix-0.1.4.5/LICENSE` & `mentabotix-0.1.4.6/LICENSE`

 * *Files identical despite different names*

### Comparing `mentabotix-0.1.4.5/README.md` & `mentabotix-0.1.4.6/README.md`

 * *Files identical despite different names*

### Comparing `mentabotix-0.1.4.5/pyproject.toml` & `mentabotix-0.1.4.6/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "mentabotix"
-version = "0.1.4.5"
+version = "0.1.4.6"
 description = "A Bot control lib"
 authors = [
     { name = "Whth", email = "88489697+Whth@users.noreply.github.com" },
 ]
 dependencies = [
     "coloredlogs>=15.0.1",
     "numpy>=1.26.4",
```

### Comparing `mentabotix-0.1.4.5/src/mentabotix/__init__.py` & `mentabotix-0.1.4.6/src/mentabotix/__init__.py`

 * *Files identical despite different names*

### Comparing `mentabotix-0.1.4.5/src/mentabotix/modules/botix.py` & `mentabotix-0.1.4.6/src/mentabotix/modules/botix.py`

 * *Files 0% similar despite different names*

```diff
@@ -297,17 +297,17 @@
             case False, False:
                 raise ValueError(
                     f"Must provide either speeds or speed_expressions, got {speeds} and {speed_expressions}"
                 )
 
         if used_context_variables:
             self._validate_used_context_variables(used_context_variables, self._speed_expressions)
-        self._before_entering: List[Callable[[], None]] = before_entering
         self._used_context_variables: List[str] = used_context_variables
-        self._after_exiting: List[Callable[[], None]] = after_exiting
+        self._before_entering: List[Callable[[], None]] = before_entering or []
+        self._after_exiting: List[Callable[[], None]] = after_exiting or []
         self._identifier: int = MovingState.__state_id_counter__
         MovingState.__state_id_counter__ += 1
 
     @staticmethod
     def _validate_used_context_variables(
         used_context_variables: List[str], speed_expressions: IndividualExpressionPattern
     ) -> None:
```

### Comparing `mentabotix-0.1.4.5/src/mentabotix/modules/logger.py` & `mentabotix-0.1.4.6/src/mentabotix/modules/logger.py`

 * *Files identical despite different names*

### Comparing `mentabotix-0.1.4.5/src/mentabotix/modules/menta.py` & `mentabotix-0.1.4.6/src/mentabotix/modules/menta.py`

 * *Files identical despite different names*

### Comparing `mentabotix-0.1.4.5/src/mentabotix/tools/composers.py` & `mentabotix-0.1.4.6/src/mentabotix/tools/composers.py`

 * *Files identical despite different names*

### Comparing `mentabotix-0.1.4.5/src/mentabotix/tools/generators.py` & `mentabotix-0.1.4.6/src/mentabotix/tools/generators.py`

 * *Files identical despite different names*

### Comparing `mentabotix-0.1.4.5/src/mentabotix/vision/tagdetector.py` & `mentabotix-0.1.4.6/src/mentabotix/vision/tagdetector.py`

 * *Files identical despite different names*

### Comparing `mentabotix-0.1.4.5/tests/find_tests.py` & `mentabotix-0.1.4.6/tests/find_tests.py`

 * *Files identical despite different names*

### Comparing `mentabotix-0.1.4.5/tests/test_botix.py` & `mentabotix-0.1.4.6/tests/test_botix.py`

 * *Files identical despite different names*

### Comparing `mentabotix-0.1.4.5/tests/test_composer.py` & `mentabotix-0.1.4.6/tests/test_composer.py`

 * *Files identical despite different names*

### Comparing `mentabotix-0.1.4.5/tests/test_menta.py` & `mentabotix-0.1.4.6/tests/test_menta.py`

 * *Files identical despite different names*

### Comparing `mentabotix-0.1.4.5/tests/test_moving_state.py` & `mentabotix-0.1.4.6/tests/test_moving_state.py`

 * *Files identical despite different names*

### Comparing `mentabotix-0.1.4.5/tests/test_moving_transition.py` & `mentabotix-0.1.4.6/tests/test_moving_transition.py`

 * *Files identical despite different names*

### Comparing `mentabotix-0.1.4.5/PKG-INFO` & `mentabotix-0.1.4.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mentabotix
-Version: 0.1.4.5
+Version: 0.1.4.6
 Summary: A Bot control lib
 Author-Email: Whth <88489697+Whth@users.noreply.github.com>
 License: MIT
 Requires-Python: >=3.11
 Requires-Dist: coloredlogs>=15.0.1
 Requires-Dist: numpy>=1.26.4
 Requires-Dist: pyapriltags>=3.3.0.3
```

