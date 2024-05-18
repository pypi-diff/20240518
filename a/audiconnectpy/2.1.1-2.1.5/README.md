# Comparing `tmp/audiconnectpy-2.1.1.tar.gz` & `tmp/audiconnectpy-2.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "audiconnectpy-2.1.1.tar", last modified: Sat May 18 14:58:23 2024, max compression
+gzip compressed data, was "audiconnectpy-2.1.5.tar", last modified: Sat May 18 17:19:04 2024, max compression
```

## Comparing `audiconnectpy-2.1.1.tar` & `audiconnectpy-2.1.5.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 14:58:23.724815 audiconnectpy-2.1.1/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 14:58:23.720815 audiconnectpy-2.1.1/.github/
--rw-r--r--   0 runner    (1001) docker     (127)      513 2024-05-18 14:58:13.000000 audiconnectpy-2.1.1/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 14:58:23.720815 audiconnectpy-2.1.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      656 2024-05-18 14:58:13.000000 audiconnectpy-2.1.1/.github/workflows/auto-approve.yml
--rw-r--r--   0 runner    (1001) docker     (127)      659 2024-05-18 14:58:13.000000 audiconnectpy-2.1.1/.github/workflows/pythonpackage.yml
--rw-r--r--   0 runner    (1001) docker     (127)      854 2024-05-18 14:58:13.000000 audiconnectpy-2.1.1/.github/workflows/pythonpublish.yml
--rw-r--r--   0 runner    (1001) docker     (127)      843 2024-05-18 14:58:13.000000 audiconnectpy-2.1.1/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1827 2024-05-18 14:58:13.000000 audiconnectpy-2.1.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1605 2024-05-18 14:58:13.000000 audiconnectpy-2.1.1/.pre-commit-config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 14:58:23.720815 audiconnectpy-2.1.1/.vscode/
--rw-r--r--   0 runner    (1001) docker     (127)      179 2024-05-18 14:58:13.000000 audiconnectpy-2.1.1/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-18 14:58:13.000000 audiconnectpy-2.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      151 2024-05-18 14:58:13.000000 audiconnectpy-2.1.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3757 2024-05-18 14:58:23.724815 audiconnectpy-2.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2809 2024-05-18 14:58:13.000000 audiconnectpy-2.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 14:58:23.720815 audiconnectpy-2.1.1/audiconnectpy/
--rw-r--r--   0 runner    (1001) docker     (127)      183 2024-05-18 14:58:13.000000 audiconnectpy-2.1.1/audiconnectpy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7395 2024-05-18 14:58:13.000000 audiconnectpy-2.1.1/audiconnectpy/api.py
--rw-r--r--   0 runner    (1001) docker     (127)    20695 2024-05-18 14:58:13.000000 audiconnectpy-2.1.1/audiconnectpy/auth.py
--rw-r--r--   0 runner    (1001) docker     (127)      993 2024-05-18 14:58:13.000000 audiconnectpy-2.1.1/audiconnectpy/const.py
--rw-r--r--   0 runner    (1001) docker     (127)      392 2024-05-18 14:58:13.000000 audiconnectpy-2.1.1/audiconnectpy/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     7769 2024-05-18 14:58:13.000000 audiconnectpy-2.1.1/audiconnectpy/helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     9119 2024-05-18 14:58:13.000000 audiconnectpy-2.1.1/audiconnectpy/model.py
--rw-r--r--   0 runner    (1001) docker     (127)    26001 2024-05-18 14:58:13.000000 audiconnectpy-2.1.1/audiconnectpy/vehicle.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 14:58:23.724815 audiconnectpy-2.1.1/audiconnectpy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3757 2024-05-18 14:58:23.000000 audiconnectpy-2.1.1/audiconnectpy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      867 2024-05-18 14:58:23.000000 audiconnectpy-2.1.1/audiconnectpy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-18 14:58:23.000000 audiconnectpy-2.1.1/audiconnectpy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-18 14:58:23.000000 audiconnectpy-2.1.1/audiconnectpy.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-18 14:58:23.000000 audiconnectpy-2.1.1/audiconnectpy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-18 14:58:23.000000 audiconnectpy-2.1.1/audiconnectpy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1816 2024-05-18 14:58:13.000000 audiconnectpy-2.1.1/example.py
--rw-r--r--   0 runner    (1001) docker     (127)     1547 2024-05-18 14:58:13.000000 audiconnectpy-2.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-05-18 14:58:13.000000 audiconnectpy-2.1.1/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-18 14:58:13.000000 audiconnectpy-2.1.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-18 14:58:23.724815 audiconnectpy-2.1.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 14:58:23.724815 audiconnectpy-2.1.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      220 2024-05-18 14:58:13.000000 audiconnectpy-2.1.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1089 2024-05-18 14:58:13.000000 audiconnectpy-2.1.1/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 14:58:23.724815 audiconnectpy-2.1.1/tests/fixtures/
--rw-r--r--   0 runner    (1001) docker     (127)     2735 2024-05-18 14:58:13.000000 audiconnectpy-2.1.1/tests/fixtures/audi0.json
--rw-r--r--   0 runner    (1001) docker     (127)      682 2024-05-18 14:58:13.000000 audiconnectpy-2.1.1/tests/fixtures/info_vehicles.json
--rw-r--r--   0 runner    (1001) docker     (127)    62872 2024-05-18 14:58:13.000000 audiconnectpy-2.1.1/tests/fixtures/location.json
--rw-r--r--   0 runner    (1001) docker     (127)     4585 2024-05-18 14:58:13.000000 audiconnectpy-2.1.1/tests/test_home.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 17:19:04.936585 audiconnectpy-2.1.5/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 17:19:04.932585 audiconnectpy-2.1.5/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      513 2024-05-18 17:18:50.000000 audiconnectpy-2.1.5/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 17:19:04.932585 audiconnectpy-2.1.5/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      656 2024-05-18 17:18:50.000000 audiconnectpy-2.1.5/.github/workflows/auto-approve.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      659 2024-05-18 17:18:50.000000 audiconnectpy-2.1.5/.github/workflows/pythonpackage.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      854 2024-05-18 17:18:50.000000 audiconnectpy-2.1.5/.github/workflows/pythonpublish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      843 2024-05-18 17:18:50.000000 audiconnectpy-2.1.5/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1827 2024-05-18 17:18:50.000000 audiconnectpy-2.1.5/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1605 2024-05-18 17:18:50.000000 audiconnectpy-2.1.5/.pre-commit-config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 17:19:04.932585 audiconnectpy-2.1.5/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (127)      179 2024-05-18 17:18:50.000000 audiconnectpy-2.1.5/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-18 17:18:50.000000 audiconnectpy-2.1.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      151 2024-05-18 17:18:50.000000 audiconnectpy-2.1.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3757 2024-05-18 17:19:04.936585 audiconnectpy-2.1.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2809 2024-05-18 17:18:50.000000 audiconnectpy-2.1.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 17:19:04.936585 audiconnectpy-2.1.5/audiconnectpy/
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2024-05-18 17:18:50.000000 audiconnectpy-2.1.5/audiconnectpy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7395 2024-05-18 17:18:50.000000 audiconnectpy-2.1.5/audiconnectpy/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20695 2024-05-18 17:18:50.000000 audiconnectpy-2.1.5/audiconnectpy/auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)      993 2024-05-18 17:18:50.000000 audiconnectpy-2.1.5/audiconnectpy/const.py
+-rw-r--r--   0 runner    (1001) docker     (127)      392 2024-05-18 17:18:50.000000 audiconnectpy-2.1.5/audiconnectpy/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7717 2024-05-18 17:18:50.000000 audiconnectpy-2.1.5/audiconnectpy/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10991 2024-05-18 17:18:50.000000 audiconnectpy-2.1.5/audiconnectpy/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26001 2024-05-18 17:18:50.000000 audiconnectpy-2.1.5/audiconnectpy/vehicle.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 17:19:04.936585 audiconnectpy-2.1.5/audiconnectpy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3757 2024-05-18 17:19:04.000000 audiconnectpy-2.1.5/audiconnectpy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      867 2024-05-18 17:19:04.000000 audiconnectpy-2.1.5/audiconnectpy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-18 17:19:04.000000 audiconnectpy-2.1.5/audiconnectpy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-18 17:19:04.000000 audiconnectpy-2.1.5/audiconnectpy.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-18 17:19:04.000000 audiconnectpy-2.1.5/audiconnectpy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-18 17:19:04.000000 audiconnectpy-2.1.5/audiconnectpy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1816 2024-05-18 17:18:50.000000 audiconnectpy-2.1.5/example.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1547 2024-05-18 17:18:50.000000 audiconnectpy-2.1.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-05-18 17:18:50.000000 audiconnectpy-2.1.5/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-18 17:18:50.000000 audiconnectpy-2.1.5/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-18 17:19:04.936585 audiconnectpy-2.1.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 17:19:04.936585 audiconnectpy-2.1.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      220 2024-05-18 17:18:50.000000 audiconnectpy-2.1.5/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1089 2024-05-18 17:18:50.000000 audiconnectpy-2.1.5/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 17:19:04.936585 audiconnectpy-2.1.5/tests/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (127)     2735 2024-05-18 17:18:50.000000 audiconnectpy-2.1.5/tests/fixtures/audi0.json
+-rw-r--r--   0 runner    (1001) docker     (127)      682 2024-05-18 17:18:50.000000 audiconnectpy-2.1.5/tests/fixtures/info_vehicles.json
+-rw-r--r--   0 runner    (1001) docker     (127)    62872 2024-05-18 17:18:50.000000 audiconnectpy-2.1.5/tests/fixtures/location.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4585 2024-05-18 17:18:50.000000 audiconnectpy-2.1.5/tests/test_home.py
```

### Comparing `audiconnectpy-2.1.1/.github/dependabot.yml` & `audiconnectpy-2.1.5/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `audiconnectpy-2.1.1/.github/workflows/auto-approve.yml` & `audiconnectpy-2.1.5/.github/workflows/auto-approve.yml`

 * *Files identical despite different names*

### Comparing `audiconnectpy-2.1.1/.github/workflows/pythonpackage.yml` & `audiconnectpy-2.1.5/.github/workflows/pythonpackage.yml`

 * *Files identical despite different names*

### Comparing `audiconnectpy-2.1.1/.github/workflows/pythonpublish.yml` & `audiconnectpy-2.1.5/.github/workflows/pythonpublish.yml`

 * *Files identical despite different names*

### Comparing `audiconnectpy-2.1.1/.github/workflows/release.yml` & `audiconnectpy-2.1.5/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `audiconnectpy-2.1.1/.gitignore` & `audiconnectpy-2.1.5/.gitignore`

 * *Files identical despite different names*

### Comparing `audiconnectpy-2.1.1/.pre-commit-config.yaml` & `audiconnectpy-2.1.5/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `audiconnectpy-2.1.1/LICENSE` & `audiconnectpy-2.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `audiconnectpy-2.1.1/PKG-INFO` & `audiconnectpy-2.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: audiconnectpy
-Version: 2.1.1
+Version: 2.1.5
 Summary: Provides asynchronous authentication and access to Audi Connect
 Author-email: Cyr-ius <cyr-ius@ipocus.net>
 License: GPL-3
 Keywords: connect,async,audi
 Platform: any
 Classifier: Programming Language :: Python
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `audiconnectpy-2.1.1/README.md` & `audiconnectpy-2.1.5/README.md`

 * *Files identical despite different names*

### Comparing `audiconnectpy-2.1.1/audiconnectpy/api.py` & `audiconnectpy-2.1.5/audiconnectpy/api.py`

 * *Files identical despite different names*

### Comparing `audiconnectpy-2.1.1/audiconnectpy/auth.py` & `audiconnectpy-2.1.5/audiconnectpy/auth.py`

 * *Files identical despite different names*

### Comparing `audiconnectpy-2.1.1/audiconnectpy/const.py` & `audiconnectpy-2.1.5/audiconnectpy/const.py`

 * *Files identical despite different names*

### Comparing `audiconnectpy-2.1.1/audiconnectpy/helpers.py` & `audiconnectpy-2.1.5/audiconnectpy/helpers.py`

 * *Files 18% similar despite different names*

```diff
@@ -123,53 +123,55 @@
     status = map_name_status(attrs)
     left_open = "closed" not in status.get("frontLeft", [])
     left_rear_open = "closed" not in status.get("rearLeft", [])
     right_open = "closed" not in status.get("frontRight", [])
     right_rear_open = "closed" not in status.get("rearRight", [])
     windows_open = [left_open, left_rear_open, right_rear_open, right_rear_open]
     metadatas = {
-        "open_left_front_window": left_open,
-        "open_left_rear_window": left_rear_open,
-        "open_right_front_window": right_open,
-        "open_right_rear_window": right_rear_open,
-        "open_any_window": any(windows_open),
+        "left_front": left_open,
+        "left_rear": left_rear_open,
+        "right_front": right_open,
+        "right_rear": right_rear_open,
+        "any_status": any(windows_open),
     }
 
     if "unsupported" not in status.get("roofCover", {}):
         open_roof_cover = "closed" not in status.get("roofCover", [])
-        metadatas.update({"open_roof_cover": open_roof_cover})
+        metadatas.update({"roof_cover": open_roof_cover})
         windows_open.append(open_roof_cover)
 
     if "unsupported" not in status.get("sunRoof", {}):
         open_sun_roof = "closed" not in status.get("sunRoof", [])
-        metadatas.update({"open_sun_roof": open_sun_roof})
+        metadatas.update({"sun_roof": open_sun_roof})
         windows_open.append(open_sun_roof)
 
-    metadatas.update({"open_any_window": any(windows_open)})
+    metadatas.update({"any_status": any(windows_open)})
 
     return metadatas
 
 
 def doors_status(attrs: list[dict[str, Any]]) -> dict[str, bool]:
     """Doors lock status."""
     status = map_name_status(attrs)
     left_unlock = "locked" not in status.get("frontLeft", [])
     left_rear_unlock = "locked" not in status.get("rearLeft", [])
     right_unlock = "locked" not in status.get("frontRight", [])
     right_rear_unlock = "locked" not in status.get("rearRight", [])
     trunk_unlock = "locked" not in status.get("trunk", [])
     doors_unlock = [left_unlock, left_rear_unlock, right_unlock, right_rear_unlock]
     metadatas = {
-        "lock_left_front_door": left_unlock,
-        "lock_left_rear_door": left_rear_unlock,
-        "lock_right_front_door": right_unlock,
-        "lock_right_rear_door": right_rear_unlock,
-        "lock_trunk": trunk_unlock,
-        "lock_any_door": any(doors_unlock),
-        "lock_doors_trunk": any(doors_unlock) and trunk_unlock,
+        "locked": {
+            "left_front": left_unlock,
+            "left_rear": left_rear_unlock,
+            "right_front": right_unlock,
+            "right_rear": right_rear_unlock,
+            "trunk": trunk_unlock,
+            "any_doors": any(doors_unlock),
+            "doors_trunk": any(doors_unlock) and trunk_unlock,
+        }
     }
 
     # Doors open status
     left_open = "closed" not in status.get("frontLeft", [])
     left_rear_open = "closed" not in status.get("rearLeft", [])
     right_open = "closed" not in status.get("frontRight", [])
     right_rear_open = "closed" not in status.get("rearRight", [])
@@ -182,21 +184,23 @@
         right_rear_open,
         trunk_open,
         bonnet_open,
     ]
 
     metadatas.update(
         {
-            "open_left_front_door": left_open,
-            "open_left_rear_door": left_rear_open,
-            "open_right_front_door": right_open,
-            "open_right_rear_door": right_rear_open,
-            "open_trunk": trunk_open,
-            "open_bonnet": bonnet_open,
-            "open_any_door": any(doors_open),
+            "opened": {
+                "left_front": left_open,
+                "left_rear": left_rear_open,
+                "right_front": right_open,
+                "right_rear": right_rear_open,
+                "trunk": trunk_open,
+                "bonnet": bonnet_open,
+                "any_doors": any(doors_open),
+            }
         }
     )
 
     return metadatas
 
 
 def lights_status(attrs: list[dict[str, Any]]) -> dict[str, bool]:
```

### Comparing `audiconnectpy-2.1.1/audiconnectpy/model.py` & `audiconnectpy-2.1.5/audiconnectpy/model.py`

 * *Files 16% similar despite different names*

```diff
@@ -24,14 +24,38 @@
     def serialize(self, value: str) -> str:
         return value
 
     def deserialize(self, value: str) -> bool:
         return value != "off"
 
 
+class WindowsStrategy(SerializationStrategy):  # type: ignore
+    def serialize(self, value: str) -> str:
+        return value
+
+    def deserialize(self, value: str) -> bool:
+        return Window.from_dict(windows_status(value))
+
+
+class DoorsStrategy(SerializationStrategy):  # type: ignore
+    def serialize(self, value: str) -> str:
+        return value
+
+    def deserialize(self, value: str) -> bool:
+        return Doors.from_dict(doors_status(value))
+
+
+class LightsStrategy(SerializationStrategy):  # type: ignore
+    def serialize(self, value: str) -> str:
+        return value
+
+    def deserialize(self, value: str) -> bool:
+        return Lights.from_dict(lights_status(value))
+
+
 @dataclass
 class Base(DataClassDictMixin):  # type: ignore
     @classmethod
     def __pre_deserialize__(cls, d: dict[Any, Any]) -> dict[Any, Any]:
         return {camel2snake(k): v for k, v in d.items()}
 
 
@@ -64,22 +88,67 @@
 
     car_captured_timestamp: datetime
     overall_status: str | None = None
     door_lock_status: bool | None = field(
         metadata=field_options(serialization_strategy=Locked()),
         default=None,
     )
-    doors: dict[str, Any] | None = field(
-        metadata=field_options(deserialize=doors_status), default=None
+    doors: Doors | None = field(
+        metadata=field_options(serialization_strategy=DoorsStrategy()), default=None
     )
-    windows: dict[str, Any] | None = field(
-        metadata=field_options(deserialize=windows_status), default=None
+    windows: Window | None = field(
+        metadata=field_options(serialization_strategy=WindowsStrategy()), default=None
     )
 
 
+@dataclass
+class Doors(DataClassDictMixin):
+    locked: DoorLocked | None = None
+    opened: DoorOpened | None = None
+
+
+@dataclass
+class DoorLocked(DataClassDictMixin):
+    """Windows status."""
+
+    left_front: bool | None = None
+    right_front: bool | None = None
+    left_rear: bool | None = None
+    right_rear: bool | None = None
+    trunk: bool | None = None
+    any_doors: bool | None = None
+    doors_trunk: bool | None = None
+
+
+@dataclass
+class DoorOpened(DataClassDictMixin):
+    """Windows status."""
+
+    left_front: bool | None = None
+    right_front: bool | None = None
+    left_rear: bool | None = None
+    right_rear: bool | None = None
+    trunk: bool | None = None
+    bonnet: bool | None = None
+    any_doors: bool | None = None
+
+
+@dataclass
+class Window(DataClassDictMixin):
+    """Windows status."""
+
+    left_front: bool | None = None
+    right_front: bool | None = None
+    left_rear: bool | None = None
+    right_rear: bool | None = None
+    roof_cover: bool | None = None
+    sun_roof: bool | None = None
+    any_status: bool | None = None
+
+
 # SECTION
 @dataclass
 class Charging(Base):
     battery_status: BatteryStatus | None = None
     charging_status: ChargingStatus | None = None
     charging_settings: ChargingSettings | None = None
     plug_status: PlugStatus | None = None
@@ -247,19 +316,25 @@
 @dataclass
 class VehicleLights(Base):
     lights_status: LightsStatus | None = None
 
 
 @dataclass
 class LightsStatus(Base):
-    lights: dict[str, Any] | None = field(
-        metadata=field_options(deserialize=lights_status), default=None
+    lights: Lights | None = field(
+        metadata=field_options(serialization_strategy=LightsStrategy()), default=None
     )
 
 
+@dataclass
+class Lights(Base):
+    left: bool | None = None
+    right: bool | None = None
+
+
 # SECTION
 @dataclass
 class VehicleHealthInspection(Base):
     maintenance_status: MaintenanceStatus | None = None
 
 
 @dataclass
@@ -311,16 +386,16 @@
 @dataclass
 class VehicleHealthWarnings(Base):
     warning_lights: WarningLights | None = None
 
 
 @dataclass
 class WarningLights(Base):
-    lights: dict[str, Any] | None = field(
-        metadata=field_options(deserialize=lights_status), default=None
+    lights: Lights | None = field(
+        metadata=field_options(serialization_strategy=LightsStrategy()), default=None
     )
 
 
 @dataclass
 class UserCapabilities(Base):
     capabilities_status: list[dict[str, Any]] | None = None
```

### Comparing `audiconnectpy-2.1.1/audiconnectpy/vehicle.py` & `audiconnectpy-2.1.5/audiconnectpy/vehicle.py`

 * *Files identical despite different names*

### Comparing `audiconnectpy-2.1.1/audiconnectpy.egg-info/PKG-INFO` & `audiconnectpy-2.1.5/audiconnectpy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: audiconnectpy
-Version: 2.1.1
+Version: 2.1.5
 Summary: Provides asynchronous authentication and access to Audi Connect
 Author-email: Cyr-ius <cyr-ius@ipocus.net>
 License: GPL-3
 Keywords: connect,async,audi
 Platform: any
 Classifier: Programming Language :: Python
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `audiconnectpy-2.1.1/audiconnectpy.egg-info/SOURCES.txt` & `audiconnectpy-2.1.5/audiconnectpy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `audiconnectpy-2.1.1/example.py` & `audiconnectpy-2.1.5/example.py`

 * *Files identical despite different names*

### Comparing `audiconnectpy-2.1.1/pyproject.toml` & `audiconnectpy-2.1.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `audiconnectpy-2.1.1/tests/conftest.py` & `audiconnectpy-2.1.5/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `audiconnectpy-2.1.1/tests/fixtures/audi0.json` & `audiconnectpy-2.1.5/tests/fixtures/audi0.json`

 * *Files identical despite different names*

### Comparing `audiconnectpy-2.1.1/tests/fixtures/info_vehicles.json` & `audiconnectpy-2.1.5/tests/fixtures/info_vehicles.json`

 * *Files identical despite different names*

### Comparing `audiconnectpy-2.1.1/tests/fixtures/location.json` & `audiconnectpy-2.1.5/tests/fixtures/location.json`

 * *Files identical despite different names*

### Comparing `audiconnectpy-2.1.1/tests/test_home.py` & `audiconnectpy-2.1.5/tests/test_home.py`

 * *Files identical despite different names*

