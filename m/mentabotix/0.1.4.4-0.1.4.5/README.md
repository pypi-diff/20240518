# Comparing `tmp/mentabotix-0.1.4.4.tar.gz` & `tmp/mentabotix-0.1.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mentabotix-0.1.4.4.tar", last modified: Fri May 17 16:49:15 2024, max compression
+gzip compressed data, was "mentabotix-0.1.4.5.tar", last modified: Sat May 18 02:30:51 2024, max compression
```

## Comparing `mentabotix-0.1.4.4.tar` & `mentabotix-0.1.4.5.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0     1066 2024-05-17 16:48:50.872905 mentabotix-0.1.4.4/LICENSE
--rw-r--r--   0        0        0    23799 2024-05-17 16:48:50.872905 mentabotix-0.1.4.4/README.md
--rw-r--r--   0        0        0      680 2024-05-17 16:49:15.237063 mentabotix-0.1.4.4/pyproject.toml
--rw-r--r--   0        0        0     1210 2024-05-17 16:48:50.872905 mentabotix-0.1.4.4/src/mentabotix/__init__.py
--rw-r--r--   0        0        0    69823 2024-05-17 16:48:50.876905 mentabotix-0.1.4.4/src/mentabotix/modules/botix.py
--rw-r--r--   0        0        0      225 2024-05-17 16:48:50.876905 mentabotix-0.1.4.4/src/mentabotix/modules/exceptions.py
--rw-r--r--   0        0        0      580 2024-05-17 16:48:50.876905 mentabotix-0.1.4.4/src/mentabotix/modules/logger.py
--rw-r--r--   0        0        0    21088 2024-05-17 16:48:50.876905 mentabotix-0.1.4.4/src/mentabotix/modules/menta.py
--rw-r--r--   0        0        0     9471 2024-05-17 16:48:50.876905 mentabotix-0.1.4.4/src/mentabotix/tools/composers.py
--rw-r--r--   0        0        0     2292 2024-05-17 16:48:50.876905 mentabotix-0.1.4.4/src/mentabotix/tools/generators.py
--rw-r--r--   0        0        0     9429 2024-05-17 16:48:50.876905 mentabotix-0.1.4.4/src/mentabotix/vision/tagdetector.py
--rw-r--r--   0        0        0        0 2024-05-17 16:48:50.876905 mentabotix-0.1.4.4/tests/__init__.py
--rw-r--r--   0        0        0      682 2024-05-17 16:48:50.876905 mentabotix-0.1.4.4/tests/find_tests.py
--rw-r--r--   0        0        0    15535 2024-05-17 16:48:50.876905 mentabotix-0.1.4.4/tests/test_botix.py
--rw-r--r--   0        0        0    10196 2024-05-17 16:48:50.876905 mentabotix-0.1.4.4/tests/test_composer.py
--rw-r--r--   0        0        0     8998 2024-05-17 16:48:50.876905 mentabotix-0.1.4.4/tests/test_menta.py
--rw-r--r--   0        0        0     7061 2024-05-17 16:48:50.876905 mentabotix-0.1.4.4/tests/test_moving_state.py
--rw-r--r--   0        0        0     5338 2024-05-17 16:48:50.876905 mentabotix-0.1.4.4/tests/test_moving_transition.py
--rw-r--r--   0        0        0    24235 1970-01-01 00:00:00.000000 mentabotix-0.1.4.4/PKG-INFO
+-rw-r--r--   0        0        0     1066 2024-05-18 02:30:24.927900 mentabotix-0.1.4.5/LICENSE
+-rw-r--r--   0        0        0    23799 2024-05-18 02:30:24.927900 mentabotix-0.1.4.5/README.md
+-rw-r--r--   0        0        0      680 2024-05-18 02:30:51.928192 mentabotix-0.1.4.5/pyproject.toml
+-rw-r--r--   0        0        0     1210 2024-05-18 02:30:24.927900 mentabotix-0.1.4.5/src/mentabotix/__init__.py
+-rw-r--r--   0        0        0    70182 2024-05-18 02:30:24.927900 mentabotix-0.1.4.5/src/mentabotix/modules/botix.py
+-rw-r--r--   0        0        0      225 2024-05-18 02:30:24.927900 mentabotix-0.1.4.5/src/mentabotix/modules/exceptions.py
+-rw-r--r--   0        0        0      580 2024-05-18 02:30:24.927900 mentabotix-0.1.4.5/src/mentabotix/modules/logger.py
+-rw-r--r--   0        0        0    21088 2024-05-18 02:30:24.931901 mentabotix-0.1.4.5/src/mentabotix/modules/menta.py
+-rw-r--r--   0        0        0     9471 2024-05-18 02:30:24.931901 mentabotix-0.1.4.5/src/mentabotix/tools/composers.py
+-rw-r--r--   0        0        0     2292 2024-05-18 02:30:24.931901 mentabotix-0.1.4.5/src/mentabotix/tools/generators.py
+-rw-r--r--   0        0        0     9429 2024-05-18 02:30:24.931901 mentabotix-0.1.4.5/src/mentabotix/vision/tagdetector.py
+-rw-r--r--   0        0        0        0 2024-05-18 02:30:24.931901 mentabotix-0.1.4.5/tests/__init__.py
+-rw-r--r--   0        0        0      682 2024-05-18 02:30:24.931901 mentabotix-0.1.4.5/tests/find_tests.py
+-rw-r--r--   0        0        0    15535 2024-05-18 02:30:24.931901 mentabotix-0.1.4.5/tests/test_botix.py
+-rw-r--r--   0        0        0    10196 2024-05-18 02:30:24.931901 mentabotix-0.1.4.5/tests/test_composer.py
+-rw-r--r--   0        0        0     8998 2024-05-18 02:30:24.931901 mentabotix-0.1.4.5/tests/test_menta.py
+-rw-r--r--   0        0        0     7555 2024-05-18 02:30:24.931901 mentabotix-0.1.4.5/tests/test_moving_state.py
+-rw-r--r--   0        0        0     5338 2024-05-18 02:30:24.931901 mentabotix-0.1.4.5/tests/test_moving_transition.py
+-rw-r--r--   0        0        0    24235 1970-01-01 00:00:00.000000 mentabotix-0.1.4.5/PKG-INFO
```

### Comparing `mentabotix-0.1.4.4/LICENSE` & `mentabotix-0.1.4.5/LICENSE`

 * *Files identical despite different names*

### Comparing `mentabotix-0.1.4.4/README.md` & `mentabotix-0.1.4.5/README.md`

 * *Files identical despite different names*

### Comparing `mentabotix-0.1.4.4/pyproject.toml` & `mentabotix-0.1.4.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "mentabotix"
-version = "0.1.4.4"
+version = "0.1.4.5"
 description = "A Bot control lib"
 authors = [
     { name = "Whth", email = "88489697+Whth@users.noreply.github.com" },
 ]
 dependencies = [
     "coloredlogs>=15.0.1",
     "numpy>=1.26.4",
```

### Comparing `mentabotix-0.1.4.4/src/mentabotix/__init__.py` & `mentabotix-0.1.4.5/src/mentabotix/__init__.py`

 * *Files identical despite different names*

### Comparing `mentabotix-0.1.4.4/src/mentabotix/modules/botix.py` & `mentabotix-0.1.4.5/src/mentabotix/modules/botix.py`

 * *Files 0% similar despite different names*

```diff
@@ -491,22 +491,30 @@
     def clone(self) -> Self:
         """
         Creates a clone of the current `MovingState` object.
 
         Returns:
             Self: A new `MovingState` object with the same speeds as the current object.
         """
+        if self._speeds is not None:
 
-        return MovingState(
-            *tuple(self._speeds.tolist()),
-            speed_expressions=self._speed_expressions,
-            used_context_variables=self._used_context_variables,
-            before_entering=self._before_entering,
-            after_exiting=self._after_exiting,
-        )
+            return MovingState(
+                *tuple(self._speeds.tolist()),
+                speed_expressions=self._speed_expressions,
+                used_context_variables=self._used_context_variables,
+                before_entering=self._before_entering,
+                after_exiting=self._after_exiting,
+            )
+        else:
+            return MovingState(
+                speed_expressions=self._speed_expressions,
+                used_context_variables=self._used_context_variables,
+                before_entering=self._before_entering,
+                after_exiting=self._after_exiting,
+            )
 
     def tokenize(self, con: Optional[CloseLoopController]) -> Tuple[List[str], Context]:
         """
         Converts the current state into a list of tokens and a context dictionary.
 
         Parameters:
         - con: Optional[CloseLoopController] - The closed-loop controller required if speed expressions exist.
```

### Comparing `mentabotix-0.1.4.4/src/mentabotix/modules/logger.py` & `mentabotix-0.1.4.5/src/mentabotix/modules/logger.py`

 * *Files identical despite different names*

### Comparing `mentabotix-0.1.4.4/src/mentabotix/modules/menta.py` & `mentabotix-0.1.4.5/src/mentabotix/modules/menta.py`

 * *Files identical despite different names*

### Comparing `mentabotix-0.1.4.4/src/mentabotix/tools/composers.py` & `mentabotix-0.1.4.5/src/mentabotix/tools/composers.py`

 * *Files identical despite different names*

### Comparing `mentabotix-0.1.4.4/src/mentabotix/tools/generators.py` & `mentabotix-0.1.4.5/src/mentabotix/tools/generators.py`

 * *Files identical despite different names*

### Comparing `mentabotix-0.1.4.4/src/mentabotix/vision/tagdetector.py` & `mentabotix-0.1.4.5/src/mentabotix/vision/tagdetector.py`

 * *Files identical despite different names*

### Comparing `mentabotix-0.1.4.4/tests/find_tests.py` & `mentabotix-0.1.4.5/tests/find_tests.py`

 * *Files identical despite different names*

### Comparing `mentabotix-0.1.4.4/tests/test_botix.py` & `mentabotix-0.1.4.5/tests/test_botix.py`

 * *Files identical despite different names*

### Comparing `mentabotix-0.1.4.4/tests/test_composer.py` & `mentabotix-0.1.4.5/tests/test_composer.py`

 * *Files identical despite different names*

### Comparing `mentabotix-0.1.4.4/tests/test_menta.py` & `mentabotix-0.1.4.5/tests/test_menta.py`

 * *Files identical despite different names*

### Comparing `mentabotix-0.1.4.4/tests/test_moving_state.py` & `mentabotix-0.1.4.5/tests/test_moving_state.py`

 * *Files 3% similar despite different names*

```diff
@@ -90,18 +90,32 @@
         state_applied = state.apply(1.5)
 
         self.assertEqual(state_applied.unwrap(), (30, 45, 60, 75))
 
     def test_clone(self):
         original_state = MovingState(10, 20, 30, 40)
         cloned_state = original_state.clone()
+        print()
 
+        print(cloned_state)
+        print(original_state)
+        print()
         self.assertEqual(cloned_state.unwrap(), (10, 20, 30, 40))
         self.assertIsNot(cloned_state, original_state)  # Ensure a new instance is returned
 
+        original_state = MovingState(speed_expressions="var1", used_context_variables=["var1"])
+
+        cloned_state = original_state.clone()
+        print(cloned_state)
+        print(original_state)
+        print()
+
+        self.assertEqual(cloned_state.speed_expressions, ("var1", "var1", "var1", "var1"))
+        self.assertIsNot(cloned_state, original_state)  # Ensure a new instance is returned()
+
     def test_tokenize(self):
 
         con_mock = Mock(
             spec=CloseLoopController(
                 [MotorInfo(1), MotorInfo(2), MotorInfo(3), MotorInfo(4)], port="COM4", context={"var1": 10, "var2": 20}
             )
         )
```

### Comparing `mentabotix-0.1.4.4/tests/test_moving_transition.py` & `mentabotix-0.1.4.5/tests/test_moving_transition.py`

 * *Files identical despite different names*

### Comparing `mentabotix-0.1.4.4/PKG-INFO` & `mentabotix-0.1.4.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mentabotix
-Version: 0.1.4.4
+Version: 0.1.4.5
 Summary: A Bot control lib
 Author-Email: Whth <88489697+Whth@users.noreply.github.com>
 License: MIT
 Requires-Python: >=3.11
 Requires-Dist: coloredlogs>=15.0.1
 Requires-Dist: numpy>=1.26.4
 Requires-Dist: pyapriltags>=3.3.0.3
```

