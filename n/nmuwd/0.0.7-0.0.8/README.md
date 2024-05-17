# Comparing `tmp/nmuwd-0.0.7.tar.gz` & `tmp/nmuwd-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nmuwd-0.0.7.tar", last modified: Fri May  3 21:39:09 2024, max compression
+gzip compressed data, was "nmuwd-0.0.8.tar", last modified: Fri May 17 22:02:16 2024, max compression
```

## Comparing `nmuwd-0.0.7.tar` & `nmuwd-0.0.8.tar`

### file list

```diff
@@ -1,24 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 21:39:09.042504 nmuwd-0.0.7/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-03 21:39:05.000000 nmuwd-0.0.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      369 2024-05-03 21:39:09.042504 nmuwd-0.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-03 21:39:05.000000 nmuwd-0.0.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 21:39:09.038504 nmuwd-0.0.7/backend/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 21:39:05.000000 nmuwd-0.0.7/backend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1677 2024-05-03 21:39:05.000000 nmuwd-0.0.7/backend/config.py
--rw-r--r--   0 runner    (1001) docker     (127)   332316 2024-05-03 21:39:05.000000 nmuwd-0.0.7/backend/geo_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2894 2024-05-03 21:39:05.000000 nmuwd-0.0.7/backend/persister.py
--rw-r--r--   0 runner    (1001) docker     (127)     2563 2024-05-03 21:39:05.000000 nmuwd-0.0.7/backend/record.py
--rw-r--r--   0 runner    (1001) docker     (127)     1550 2024-05-03 21:39:05.000000 nmuwd-0.0.7/backend/source.py
--rw-r--r--   0 runner    (1001) docker     (127)     2513 2024-05-03 21:39:05.000000 nmuwd-0.0.7/backend/transformer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 21:39:09.038504 nmuwd-0.0.7/frontend/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 21:39:05.000000 nmuwd-0.0.7/frontend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2012 2024-05-03 21:39:05.000000 nmuwd-0.0.7/frontend/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     3925 2024-05-03 21:39:05.000000 nmuwd-0.0.7/frontend/unifier.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 21:39:09.038504 nmuwd-0.0.7/nmuwd.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      369 2024-05-03 21:39:09.000000 nmuwd-0.0.7/nmuwd.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      370 2024-05-03 21:39:09.000000 nmuwd-0.0.7/nmuwd.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 21:39:09.000000 nmuwd-0.0.7/nmuwd.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-03 21:39:09.000000 nmuwd-0.0.7/nmuwd.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-03 21:39:09.000000 nmuwd-0.0.7/nmuwd.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-03 21:39:09.042504 nmuwd-0.0.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1718 2024-05-03 21:39:05.000000 nmuwd-0.0.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 22:02:16.059163 nmuwd-0.0.8/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-17 22:02:12.000000 nmuwd-0.0.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1189 2024-05-17 22:02:16.059163 nmuwd-0.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      732 2024-05-17 22:02:12.000000 nmuwd-0.0.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 22:02:16.055163 nmuwd-0.0.8/backend/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 22:02:12.000000 nmuwd-0.0.8/backend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3583 2024-05-17 22:02:12.000000 nmuwd-0.0.8/backend/bounding_polygons.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7212 2024-05-17 22:02:12.000000 nmuwd-0.0.8/backend/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1458 2024-05-17 22:02:12.000000 nmuwd-0.0.8/backend/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2683 2024-05-17 22:02:12.000000 nmuwd-0.0.8/backend/geo_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2982 2024-05-17 22:02:12.000000 nmuwd-0.0.8/backend/persister.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3923 2024-05-17 22:02:12.000000 nmuwd-0.0.8/backend/record.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6780 2024-05-17 22:02:12.000000 nmuwd-0.0.8/backend/source.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8588 2024-05-17 22:02:12.000000 nmuwd-0.0.8/backend/transformer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 22:02:16.055163 nmuwd-0.0.8/frontend/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 22:02:12.000000 nmuwd-0.0.8/frontend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4372 2024-05-17 22:02:12.000000 nmuwd-0.0.8/frontend/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3349 2024-05-17 22:02:12.000000 nmuwd-0.0.8/frontend/unifier.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 22:02:16.059163 nmuwd-0.0.8/nmuwd.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1189 2024-05-17 22:02:16.000000 nmuwd-0.0.8/nmuwd.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      448 2024-05-17 22:02:16.000000 nmuwd-0.0.8/nmuwd.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-17 22:02:16.000000 nmuwd-0.0.8/nmuwd.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-17 22:02:16.000000 nmuwd-0.0.8/nmuwd.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-17 22:02:16.000000 nmuwd-0.0.8/nmuwd.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-17 22:02:16.000000 nmuwd-0.0.8/nmuwd.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-17 22:02:16.059163 nmuwd-0.0.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1767 2024-05-17 22:02:12.000000 nmuwd-0.0.8/setup.py
```

### Comparing `nmuwd-0.0.7/LICENSE` & `nmuwd-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `nmuwd-0.0.7/backend/persister.py` & `nmuwd-0.0.8/backend/persister.py`

 * *Files 6% similar despite different names*

```diff
@@ -29,26 +29,29 @@
     def log(self, msg, fg="yellow"):
         click.secho(f"{self.__class__.__name__:30s}{msg}", fg=fg)
 
 
 class BasePersister(Loggable):
     extension = None
 
-    def __init__(self, record_klass):
+    def __init__(self):
         self.records = []
 
-        self.keys = record_klass.keys
+        # self.keys = record_klass.keys
 
     def load(self, records):
         self.records.extend(records)
 
     def save(self, path):
         path = self.add_extension(path)
-        self.log(f"saving to {path}")
-        self._save(path)
+        if self.records:
+            self.log(f"saving to {path}")
+            self._save(path)
+        else:
+            self.log("no records to save", fg="red")
 
     def add_extension(self, path):
         if not self.extension:
             raise NotImplementedError
 
         if not path.endswith(self.extension):
             path = f"{path}.{self.extension}"
@@ -58,18 +61,19 @@
         raise NotImplementedError
 
 
 class CSVPersister(BasePersister):
     extension = "csv"
 
     def _save(self, path):
-        path = self.add_extension(path)
         with open(path, "w") as f:
             writer = csv.writer(f)
-            writer.writerow(self.keys)
+
+            record = self.records[0]
+            writer.writerow(record.keys)
             for record in self.records:
                 writer.writerow(record.to_row())
 
 
 class GeoJSONPersister(BasePersister):
     extension = "geojson"
```

### Comparing `nmuwd-0.0.7/backend/record.py` & `nmuwd-0.0.8/backend/record.py`

 * *Files 26% similar despite different names*

```diff
@@ -21,54 +21,101 @@
 
     def __init__(self, payload):
         self._payload = payload
 
     def to_row(self):
 
         def get(attr):
-            v = self._payload.get(attr)
-            if attr == "elevation" and v is not None:
-                v = round(v, 2)
-
-            if v is None:
-                v = self.defaults.get(attr)
+            # v = self._payload.get(attr)
+            # if v is None and self.defaults:
+            #     v = self.defaults.get(attr)
+            v = self.__getattr__(attr)
+            for key, sigfigs in (
+                ("elevation", 2),
+                ("depth_to_water_ft_below_ground_surface", 2),
+                ("surface_elevation_ft", 2),
+                ("well_depth_ft_below_ground_surface", 2),
+                ("well_depth", 2),
+                ("latitude", 6),
+                ("longitude", 6),
+                ("min", 2),
+                ("max", 2),
+                ("mean", 2),
+            ):
+                if v is not None and key == attr:
+                    try:
+                        v = round(v, sigfigs)
+                    except TypeError as e:
+                        print(key, attr)
+                        raise e
+                    break
             return v
 
         return [get(k) for k in self.keys]
 
     def update(self, **kw):
         self._payload.update(kw)
 
-    def __getattr__(self, k):
-        return self._payload.get(k)
+    def __getattr__(self, attr):
+        v = self._payload.get(attr)
+        if v is None and self.defaults:
+            v = self.defaults.get(attr)
+        return v
 
 
 class WaterLevelRecord(BaseRecord):
     keys = (
         "source",
         "id",
+        "location",
+        "latitude",
+        "longitude",
         "surface_elevation_ft",
         "well_depth_ft_below_ground_surface",
         "depth_to_water_ft_below_ground_surface",
         "date_measured",
         "time_measured",
     )
+
     defaults = {}
 
 
-class AnalyteRecord(BaseRecord):
+class SummaryRecord(BaseRecord):
     keys = (
         "source",
         "id",
-        "date_measured",
-        "time_measured",
-        "analyte",
-        "result",
-        "units"
+        "location",
+        "usgs_site_id",
+        "alternate_site_id",
+        "latitude",
+        "longitude",
+        "elevation",
+        "elevation_units",
+        "well_depth",
+        "well_depth_units",
+        "parameter",
+        "parameter_units",
+        "nrecords",
+        "min",
+        "max",
+        "mean",
+        "most_recent_date",
+        "most_recent_time",
+        "most_recent_value",
+        "most_recent_units",
     )
+    defaults = {}
+
+
+class WaterLevelSummaryRecord(SummaryRecord):
+    pass
+
+
+class AnalyteSummaryRecord(SummaryRecord):
+    pass
 
 
 class SiteRecord(BaseRecord):
     keys = (
         "source",
         "id",
         "name",
@@ -78,26 +125,29 @@
         "elevation_units",
         "horizontal_datum",
         "vertical_datum",
         "usgs_site_id",
         "alternate_site_id",
         "formation",
         "aquifer",
+        "well_depth",
     )
 
     defaults = {
         "source": None,
         "id": None,
         "name": "",
         "latitude": None,
         "longitude": None,
         "elevation": None,
         "elevation_units": "feet",
-        "horizontal_datum": "",
+        "horizontal_datum": "WGS84",
         "vertical_datum": "",
         "usgs_site_id": "",
         "alternate_site_id": "",
         "formation": "",
         "aquifer": "",
+        "well_depth": None,
     }
 
+
 # ============= EOF =============================================
```

### Comparing `nmuwd-0.0.7/setup.py` & `nmuwd-0.0.8/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,25 +17,25 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="nmuwd",
-    version="0.0.7",
+    version="0.0.8",
     author="Jake Ross",
     description="New Mexico Water Data Integration Engine",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/DataIntegrationGroup/PyWeaver",
     classifiers=[
         "Programming Language :: Python :: 3",
         "Operating System :: OS Independent",
     ],
-    install_requires=[],
+    install_requires=["click", "httpx", "geopandas", "frost_sta_client"],
     entry_points={
         "console_scripts": [
             "weave = frontend.cli:cli",
         ],
     },
     packages=["frontend", "backend"],
     python_requires=">=3.6",
```

