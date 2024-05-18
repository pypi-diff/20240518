# Comparing `tmp/synthetic_home-0.0.1.tar.gz` & `tmp/synthetic_home-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "synthetic_home-0.0.1.tar", last modified: Mon May 13 03:54:59 2024, max compression
+gzip compressed data, was "synthetic_home-0.1.0.tar", last modified: Sat May 18 05:49:11 2024, max compression
```

## Comparing `synthetic_home-0.0.1.tar` & `synthetic_home-0.1.0.tar`

### file list

```diff
@@ -1,21 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 03:54:59.593345 synthetic_home-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-13 03:54:52.000000 synthetic_home-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      893 2024-05-13 03:54:59.593345 synthetic_home-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      354 2024-05-13 03:54:52.000000 synthetic_home-0.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      593 2024-05-13 03:54:52.000000 synthetic_home-0.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      791 2024-05-13 03:54:59.597345 synthetic_home-0.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-05-13 03:54:52.000000 synthetic_home-0.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 03:54:59.593345 synthetic_home-0.0.1/synthetic_home/
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-05-13 03:54:52.000000 synthetic_home-0.0.1/synthetic_home/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7050 2024-05-13 03:54:52.000000 synthetic_home-0.0.1/synthetic_home/device_types.py
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-05-13 03:54:52.000000 synthetic_home-0.0.1/synthetic_home/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 03:54:59.593345 synthetic_home-0.0.1/synthetic_home/registry/
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-13 03:54:52.000000 synthetic_home-0.0.1/synthetic_home/registry/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 03:54:59.593345 synthetic_home-0.0.1/synthetic_home.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      893 2024-05-13 03:54:59.000000 synthetic_home-0.0.1/synthetic_home.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      398 2024-05-13 03:54:59.000000 synthetic_home-0.0.1/synthetic_home.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 03:54:59.000000 synthetic_home-0.0.1/synthetic_home.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-13 03:54:59.000000 synthetic_home-0.0.1/synthetic_home.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-13 03:54:59.000000 synthetic_home-0.0.1/synthetic_home.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 03:54:59.593345 synthetic_home-0.0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      571 2024-05-13 03:54:52.000000 synthetic_home-0.0.1/tests/test_device_types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 05:49:11.857648 synthetic_home-0.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-18 05:49:07.000000 synthetic_home-0.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4768 2024-05-18 05:49:11.857648 synthetic_home-0.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4229 2024-05-18 05:49:07.000000 synthetic_home-0.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      593 2024-05-18 05:49:07.000000 synthetic_home-0.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      803 2024-05-18 05:49:11.861648 synthetic_home-0.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-05-18 05:49:07.000000 synthetic_home-0.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 05:49:11.857648 synthetic_home-0.1.0/synthetic_home/
+-rw-r--r--   0 runner    (1001) docker     (127)      125 2024-05-18 05:49:07.000000 synthetic_home-0.1.0/synthetic_home/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6900 2024-05-18 05:49:07.000000 synthetic_home-0.1.0/synthetic_home/device_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-05-18 05:49:07.000000 synthetic_home-0.1.0/synthetic_home/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-18 05:49:07.000000 synthetic_home-0.1.0/synthetic_home/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 05:49:11.857648 synthetic_home-0.1.0/synthetic_home/registry/
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-18 05:49:07.000000 synthetic_home-0.1.0/synthetic_home/registry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4922 2024-05-18 05:49:07.000000 synthetic_home-0.1.0/synthetic_home/synthetic_home.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 05:49:11.857648 synthetic_home-0.1.0/synthetic_home.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4768 2024-05-18 05:49:11.000000 synthetic_home-0.1.0/synthetic_home.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      488 2024-05-18 05:49:11.000000 synthetic_home-0.1.0/synthetic_home.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-18 05:49:11.000000 synthetic_home-0.1.0/synthetic_home.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-18 05:49:11.000000 synthetic_home-0.1.0/synthetic_home.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-18 05:49:11.000000 synthetic_home-0.1.0/synthetic_home.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 05:49:11.857648 synthetic_home-0.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      571 2024-05-18 05:49:07.000000 synthetic_home-0.1.0/tests/test_device_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)      647 2024-05-18 05:49:07.000000 synthetic_home-0.1.0/tests/test_synthetic_home.py
```

### Comparing `synthetic_home-0.0.1/LICENSE` & `synthetic_home-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `synthetic_home-0.0.1/pyproject.toml` & `synthetic_home-0.1.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `synthetic_home-0.0.1/setup.cfg` & `synthetic_home-0.1.0/setup.cfg`

 * *Files 14% similar despite different names*

```diff
@@ -1,38 +1,40 @@
 [metadata]
 name = synthetic_home
-version = 0.0.1
+version = 0.1.0
 description = Library for managing synthetic home device registry
 long_description = file: README.md
 long_description_content_type = text/markdown
-url = https://github.com/allenporter/synthetic_home
+url = https://github.com/allenporter/synthetic-home
 author = Allen Porter
 author_email = allen.porter@gmail.com
 license = Apache-2.0
 license_files = LICENSE
 classifiers = 
 	License :: OSI Approved :: Apache Software License
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3 :: Only
 
 [options]
 packages = find:
 install_requires = 
 	mashumaro>=3.13
-python_requires = >=3.11
+python_requires = >=3.12
 include_package_data = True
 package_dir = 
 	= .
 
 [options.packages.find]
 where = .
 exclude = 
 	tests
 	tests.*
 
 [options.package_data]
-synthetic_home = py.typed
+synthetic_home = 
+	py.typed
+	registry
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `synthetic_home-0.0.1/synthetic_home/device_types.py` & `synthetic_home-0.1.0/synthetic_home/device_types.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,16 +14,16 @@
 from .exceptions import SyntheticHomeError
 
 __all__ = [
     "DeviceTypeRegistry",
     "DeviceType",
     "load_device_type_registry",
     "EntityEntry",
-    "load_restorable_attributes",
-    "RestorableAttributes"
+    "load_predefined_states",
+    "PredefinedStates"
 ]
 
 
 _LOGGER = logging.getLogger(__name__)
 
 
 DEVICE_TYPES_RESOURCE_PATH = resources.files().joinpath("registry")
@@ -54,20 +54,20 @@
                 parts = attribute.split("=")
                 entity_attribute_key = parts[0]
                 device_attribute_key = parts[1]
             yield device_attribute_key, entity_attribute_key
 
 
 @dataclass
-class RestorableAttributes:
+class PredefinedState:
     """Represents a device state that can be used to save a pre-canned restore state.
 
     This is used as a grouping of state values representing the "interesting"
     states of the device that can be enumerated during evaluation. For example,
-    instead of explicitly specifying specific temperature values, a restorable
+    instead of explicitly specifying specific temperature values, a predefined
     state could implement "warm" and "cool".
     """
 
     key: str
     """An identifier for this set of attributes used for labeling"""
 
     attributes: dict[str, Any] = field(default_factory=dict)
@@ -89,15 +89,15 @@
 
     supported_attributes: list[str] = field(default_factory=list)
     """Attributes supported by this device, mapped to entity attributes."""
 
     supported_state_attributes: list[str] = field(default_factory=list)
     """State values that can be set on this device, mapped to entity attributes."""
 
-    restorable_attributes: list[RestorableAttributes] = field(default_factory=list)
+    predefined_states: list[PredefinedState] = field(default_factory=list)
     """A series of different attribute values that are most interesting to use during evaluation."""
 
     @property
     def entity_entries(self) -> dict[str, list[EntityEntry]]:
         """Return the parsed entitty attributes for consumption."""
         result: dict[str, list[EntityEntry]] = {}
         for key, entity_entries in self.entities.items():
@@ -112,25 +112,23 @@
                     raise SyntheticHomeError(
                         f"Unknown Entity Entry type {entity_entry}"
                     )
             result[key] = updated_entries
         return result
 
     @property
-    def all_restore_attribute_keys(self) -> list[str]:
-        """Return all restorable attribute keys supported."""
-        return [state.key for state in self.restorable_attributes]
-
-    def get_restorable_attributes_by_key(
-        self, restore_attribute_key: str
-    ) -> RestorableAttributes | None:
-        """Get the set of restorable attributes by the specified key."""
-        for restore_attribute in self.restorable_attributes:
-            if restore_attribute.key == restore_attribute_key:
-                return restore_attribute
+    def all_predefined_state_keys(self) -> list[str]:
+        """Return all predefined state keys supported."""
+        return [state.key for state in self.predefined_states]
+
+    def get_predefined_states_by_key(self, key: str) -> PredefinedState | None:
+        """Get the predefined state by the specified key."""
+        for state in self.predefined_states:
+            if state.key == key:
+                return state
         return None
 
 
 @dataclass
 class DeviceTypeRegistry:
     """The registry of all DeviceType objects."""
 
@@ -177,12 +175,12 @@
             raise SyntheticHomeError(
                 f"Device registry contains duplicate device type '{device_type.device_type}"
             )
         device_types[device_type.device_type] = device_type
     return DeviceTypeRegistry(device_types=device_types)
 
 
-def load_restorable_attributes(device_type: str) -> list[str]:
+def load_predefined_states(device_type: str) -> list[str]:
     """Enumerate the evaluation states for the specified device type."""
     device_type_registry = load_device_type_registry()
     camera_device_type = device_type_registry.device_types[device_type]
-    return [eval_state.key for eval_state in camera_device_type.restorable_attributes]
+    return [eval_state.key for eval_state in camera_device_type.predefined_states]
```

### Comparing `synthetic_home-0.0.1/tests/test_device_types.py` & `synthetic_home-0.1.0/tests/test_device_types.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-"""Test for devife_types."""
+"""Test for device_types."""
 
 from synthetic_home import device_types
 
 def test_load_device_type_registry() -> None:
     """Test loading the device type registry."""
 
     reg = device_types.load_device_type_registry()
```

