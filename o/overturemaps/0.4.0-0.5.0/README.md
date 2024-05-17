# Comparing `tmp/overturemaps-0.4.0.tar.gz` & `tmp/overturemaps-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "overturemaps-0.4.0.tar", max compression
+gzip compressed data, was "overturemaps-0.5.0.tar", max compression
```

## Comparing `overturemaps-0.4.0.tar` & `overturemaps-0.5.0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1070 2024-04-06 10:31:26.935857 overturemaps-0.4.0/LICENSE
--rw-r--r--   0        0        0     2507 2024-04-11 15:34:22.013871 overturemaps-0.4.0/README.md
--rw-r--r--   0        0        0       75 2024-04-11 16:40:32.681725 overturemaps-0.4.0/overturemaps/__init__.py
--rw-r--r--   0        0        0     5086 2024-04-16 03:33:02.187599 overturemaps-0.4.0/overturemaps/cli.py
--rw-r--r--   0        0        0     3246 2024-04-16 03:37:08.217413 overturemaps-0.4.0/overturemaps/core.py
--rw-r--r--   0        0        0      479 2024-04-19 20:54:04.960647 overturemaps-0.4.0/pyproject.toml
--rw-r--r--   0        0        0     3258 1970-01-01 00:00:00.000000 overturemaps-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1070 2024-04-06 10:31:26.935857 overturemaps-0.5.0/LICENSE
+-rw-r--r--   0        0        0     2515 2024-05-16 01:34:45.209954 overturemaps-0.5.0/README.md
+-rw-r--r--   0        0        0       75 2024-04-11 16:40:32.681725 overturemaps-0.5.0/overturemaps/__init__.py
+-rw-r--r--   0        0        0     5086 2024-05-16 01:34:45.212089 overturemaps-0.5.0/overturemaps/cli.py
+-rw-r--r--   0        0        0     3335 2024-05-16 01:44:07.446107 overturemaps-0.5.0/overturemaps/core.py
+-rw-r--r--   0        0        0      479 2024-05-17 23:41:16.697556 overturemaps-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0     3266 1970-01-01 00:00:00.000000 overturemaps-0.5.0/PKG-INFO
```

### Comparing `overturemaps-0.4.0/LICENSE` & `overturemaps-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `overturemaps-0.4.0/README.md` & `overturemaps-0.5.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # overturemaps-py
 
-Official Python command-line tool of the [Overture Maps Foundation](overturemaps.org)
+Official Python command-line tool of the [Overture Maps Foundation](https://overturemaps.org)
 
 Overture Maps provides free and open geospatial map data, from many different sources and normalized to a
 [common schema](https://github.com/OvertureMaps/schema). This tool helps to download Overture data
 within a region of interest and converts it to a few different file formats. For more information about accessing
 Overture Maps data, see our official documentation site https://docs.overturemaps.org.
 
 Note: This repository and project are experimental. Things are likely change including the user interface
```

### Comparing `overturemaps-0.4.0/overturemaps/cli.py` & `overturemaps-0.5.0/overturemaps/cli.py`

 * *Files identical despite different names*

### Comparing `overturemaps-0.4.0/overturemaps/core.py` & `overturemaps-0.5.0/overturemaps/core.py`

 * *Files 3% similar despite different names*

```diff
@@ -71,19 +71,22 @@
 
 type_theme_map = {
     "locality": "admins",
     "locality_area": "admins",
     "administrative_boundary": "admins",
     "building": "buildings",
     "building_part": "buildings",
+    "division": "divisions",
+    "division_area": "divisions",
     "place": "places",
     "segment": "transportation",
     "connector": "transportation",
     "infrastructure": "base",
     "land": "base",
+    "land_cover": "base",
     "land_use": "base",
     "water": "base",
 }
 
 
 def _dataset_path(overture_type: str) -> str:
     """
@@ -91,12 +94,12 @@
     been validated, e.g. by the CLI
 
     """
     # Map of sub-partition "type" to parent partition "theme" for forming the
     # complete s3 path. Could be discovered by reading from the top-level s3
     # location but this allows to only read the files in the necessary partition.
     theme = type_theme_map[overture_type]
-    return f"overturemaps-us-west-2/release/2024-04-16-beta.0/theme={theme}/type={overture_type}/"
+    return f"overturemaps-us-west-2/release/2024-05-16-beta.0/theme={theme}/type={overture_type}/"
 
 
 def get_all_overture_types() -> List[str]:
     return list(type_theme_map.keys())
```

### Comparing `overturemaps-0.4.0/PKG-INFO` & `overturemaps-0.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: overturemaps
-Version: 0.4.0
+Version: 0.5.0
 Summary: Python tools for interacting with Overture Maps (overturemaps.org) data.
 License: MIT
 Author: Jacob Wasserman
 Author-email: jwasserman@meta.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -16,15 +16,15 @@
 Requires-Dist: click (>=8.1.7,<9.0.0)
 Requires-Dist: pyarrow (>=15.0.2,<16.0.0)
 Requires-Dist: shapely (>=2.0.3,<3.0.0)
 Description-Content-Type: text/markdown
 
 # overturemaps-py
 
-Official Python command-line tool of the [Overture Maps Foundation](overturemaps.org)
+Official Python command-line tool of the [Overture Maps Foundation](https://overturemaps.org)
 
 Overture Maps provides free and open geospatial map data, from many different sources and normalized to a
 [common schema](https://github.com/OvertureMaps/schema). This tool helps to download Overture data
 within a region of interest and converts it to a few different file formats. For more information about accessing
 Overture Maps data, see our official documentation site https://docs.overturemaps.org.
 
 Note: This repository and project are experimental. Things are likely change including the user interface
```

