# Comparing `tmp/grid2demand-0.4.4.tar.gz` & `tmp/grid2demand-0.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "grid2demand-0.4.4.tar", last modified: Thu May 16 07:48:36 2024, max compression
+gzip compressed data, was "grid2demand-0.4.5.tar", last modified: Sat May 18 02:28:44 2024, max compression
```

## Comparing `grid2demand-0.4.4.tar` & `grid2demand-0.4.5.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxrwx   0        0        0        0 2024-05-16 07:48:36.009339 grid2demand-0.4.4/
--rw-rw-rw-   0        0        0    11558 2023-09-29 02:14:48.000000 grid2demand-0.4.4/LICENSE
--rw-rw-rw-   0        0        0     7782 2024-05-16 07:48:35.996730 grid2demand-0.4.4/PKG-INFO
--rw-rw-rw-   0        0        0    34060 2024-05-16 07:46:55.000000 grid2demand-0.4.4/README.md
-drwxrwxrwx   0        0        0        0 2024-05-16 07:48:35.941416 grid2demand-0.4.4/grid2demand/
--rw-rw-rw-   0        0        0     1689 2024-05-16 07:19:09.000000 grid2demand-0.4.4/grid2demand/__init__.py
--rw-rw-rw-   0        0        0    53439 2024-05-15 21:11:09.000000 grid2demand-0.4.4/grid2demand/_grid2demand.py
-drwxrwxrwx   0        0        0        0 2024-05-16 07:48:35.993640 grid2demand-0.4.4/grid2demand/func_lib/
--rw-rw-rw-   0        0        0      282 2023-09-29 02:14:49.000000 grid2demand-0.4.4/grid2demand/func_lib/__init__.py
--rw-rw-rw-   0        0        0     2548 2024-03-31 02:03:11.000000 grid2demand-0.4.4/grid2demand/func_lib/gen_agent_demand.py
--rw-rw-rw-   0        0        0    20218 2024-05-15 19:53:14.000000 grid2demand-0.4.4/grid2demand/func_lib/gen_zone.py
--rw-rw-rw-   0        0        0     4182 2024-05-15 19:53:14.000000 grid2demand-0.4.4/grid2demand/func_lib/gravity_model.py
--rw-rw-rw-   0        0        0    18686 2024-05-15 19:53:14.000000 grid2demand-0.4.4/grid2demand/func_lib/read_node_poi.py
--rw-rw-rw-   0        0        0     6991 2024-05-15 19:53:14.000000 grid2demand-0.4.4/grid2demand/func_lib/trip_rate_production_attraction.py
-drwxrwxrwx   0        0        0        0 2024-05-16 07:48:35.996730 grid2demand-0.4.4/grid2demand/utils_lib/
--rw-rw-rw-   0        0        0      282 2023-09-29 02:14:49.000000 grid2demand-0.4.4/grid2demand/utils_lib/__init__.py
--rw-rw-rw-   0        0        0     6018 2024-03-27 02:20:39.000000 grid2demand-0.4.4/grid2demand/utils_lib/net_utils.py
--rw-rw-rw-   0        0        0     3385 2024-05-15 19:53:14.000000 grid2demand-0.4.4/grid2demand/utils_lib/pkg_settings.py
--rw-rw-rw-   0        0        0     9295 2024-05-15 19:53:14.000000 grid2demand-0.4.4/grid2demand/utils_lib/utils.py
-drwxrwxrwx   0        0        0        0 2024-05-16 07:48:35.980666 grid2demand-0.4.4/grid2demand.egg-info/
--rw-rw-rw-   0        0        0     7782 2024-05-16 07:48:35.000000 grid2demand-0.4.4/grid2demand.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      653 2024-05-16 07:48:35.000000 grid2demand-0.4.4/grid2demand.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-16 07:48:35.000000 grid2demand-0.4.4/grid2demand.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       79 2024-05-16 07:48:35.000000 grid2demand-0.4.4/grid2demand.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2024-05-16 07:48:35.000000 grid2demand-0.4.4/grid2demand.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-16 07:48:36.009925 grid2demand-0.4.4/setup.cfg
--rw-rw-rw-   0        0        0     1970 2024-05-16 07:46:29.000000 grid2demand-0.4.4/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-16 07:48:35.996730 grid2demand-0.4.4/tests/
--rw-rw-rw-   0        0        0      552 2024-03-01 23:27:53.000000 grid2demand-0.4.4/tests/test_read_node.py
+drwxrwxrwx   0        0        0        0 2024-05-18 02:28:44.586975 grid2demand-0.4.5/
+-rw-rw-rw-   0        0        0    11558 2023-09-29 02:14:50.000000 grid2demand-0.4.5/LICENSE
+-rw-rw-rw-   0        0        0     8385 2024-05-18 02:28:44.585975 grid2demand-0.4.5/PKG-INFO
+-rw-rw-rw-   0        0        0    34624 2024-05-18 02:27:14.000000 grid2demand-0.4.5/README.md
+drwxrwxrwx   0        0        0        0 2024-05-18 02:28:44.551120 grid2demand-0.4.5/grid2demand/
+-rw-rw-rw-   0        0        0     1689 2024-05-18 02:28:24.000000 grid2demand-0.4.5/grid2demand/__init__.py
+-rw-rw-rw-   0        0        0    53439 2024-05-16 17:50:59.000000 grid2demand-0.4.5/grid2demand/_grid2demand.py
+drwxrwxrwx   0        0        0        0 2024-05-18 02:28:44.567452 grid2demand-0.4.5/grid2demand/func_lib/
+-rw-rw-rw-   0        0        0      282 2023-09-29 02:14:50.000000 grid2demand-0.4.5/grid2demand/func_lib/__init__.py
+-rw-rw-rw-   0        0        0     2548 2024-05-13 22:33:57.000000 grid2demand-0.4.5/grid2demand/func_lib/gen_agent_demand.py
+-rw-rw-rw-   0        0        0    20218 2024-05-13 22:41:08.000000 grid2demand-0.4.5/grid2demand/func_lib/gen_zone.py
+-rw-rw-rw-   0        0        0     4182 2024-05-13 22:24:06.000000 grid2demand-0.4.5/grid2demand/func_lib/gravity_model.py
+-rw-rw-rw-   0        0        0    18686 2024-05-13 22:20:21.000000 grid2demand-0.4.5/grid2demand/func_lib/read_node_poi.py
+-rw-rw-rw-   0        0        0     6991 2024-05-13 22:35:49.000000 grid2demand-0.4.5/grid2demand/func_lib/trip_rate_production_attraction.py
+drwxrwxrwx   0        0        0        0 2024-05-18 02:28:44.584976 grid2demand-0.4.5/grid2demand/utils_lib/
+-rw-rw-rw-   0        0        0      282 2023-09-29 02:14:50.000000 grid2demand-0.4.5/grid2demand/utils_lib/__init__.py
+-rw-rw-rw-   0        0        0     6019 2024-05-17 23:40:00.000000 grid2demand-0.4.5/grid2demand/utils_lib/net_utils.py
+-rw-rw-rw-   0        0        0     3385 2024-05-10 20:58:54.000000 grid2demand-0.4.5/grid2demand/utils_lib/pkg_settings.py
+-rw-rw-rw-   0        0        0     9295 2024-05-13 22:38:13.000000 grid2demand-0.4.5/grid2demand/utils_lib/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-18 02:28:44.567452 grid2demand-0.4.5/grid2demand.egg-info/
+-rw-rw-rw-   0        0        0     8385 2024-05-18 02:28:44.000000 grid2demand-0.4.5/grid2demand.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      653 2024-05-18 02:28:44.000000 grid2demand-0.4.5/grid2demand.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-18 02:28:44.000000 grid2demand-0.4.5/grid2demand.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       79 2024-05-18 02:28:44.000000 grid2demand-0.4.5/grid2demand.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2024-05-18 02:28:44.000000 grid2demand-0.4.5/grid2demand.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-18 02:28:44.586975 grid2demand-0.4.5/setup.cfg
+-rw-rw-rw-   0        0        0     1970 2024-05-18 02:28:37.000000 grid2demand-0.4.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-18 02:28:44.584976 grid2demand-0.4.5/tests/
+-rw-rw-rw-   0        0        0      552 2024-03-01 23:27:54.000000 grid2demand-0.4.5/tests/test_read_node.py
```

### Comparing `grid2demand-0.4.4/LICENSE` & `grid2demand-0.4.5/LICENSE`

 * *Files identical despite different names*

### Comparing `grid2demand-0.4.4/PKG-INFO` & `grid2demand-0.4.5/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: grid2demand
-Version: 0.4.4
+Version: 0.4.5
 Summary: A tool for generating zone-to-zone travel demand based on grid cells or TAZs and gravity model
 Home-page: https://github.com/xyluo25/grid2demand
 Author: Xiangyong Luo, Dr.Xuesong(Simon) Zhou
 Author-email: luoxiangyong01@gmail.com, xzhou74@asu.edu
 Project-URL: Homepage, https://github.com/asu-trans-ai-lab/grid2demand
 Project-URL: Documentation, https://github.com/asu-trans-ai-lab/grid2demand
 Classifier: Programming Language :: Python :: 3
@@ -66,18 +66,21 @@
     net.load_network()
 
     # Generate zone dictionary from node dictionary by specifying number of x blocks and y blocks
     net.net2zone(num_x_blocks=10, num_y_blocks=10)
     # net.net2zone(cell_width=10, cell_height=10, unit="km")
 
     # Synchronize geometry info between zone, node and poi
+    # if you want to save updated node, poi, zone without demand,
+    # you can skip net.run_gravity_model()
+    # and run net.save_results_to_csv(overwrite_file=True) directly
     net.sync_geometry_between_zone_and_node_poi()
 
     # Calculate demand by running gravity model
-    net.run_gravity_model(zone_prod_attr, zone_od_distance_matrix)
+    net.run_gravity_model()
 
     # Save demand, zone, updated node, updated poi to csv
     net.save_results_to_csv(overwrite_file=True)
 ```
 
 # Generate Demand with node.csv, poi.csv and zone.csv (geometry filed in zone.csv)
 
@@ -98,18 +101,21 @@
     # load network: node and poi
     net.load_network()
 
     # Generate zone
     net.taz2zone()
 
     # Synchronize geometry info between zone, node and poi
+    # if you want to save updated node, poi, zone without demand,
+    # you can skip net.run_gravity_model()
+    # and run net.save_results_to_csv(overwrite_file=True) directly
     net.sync_geometry_between_zone_and_node_poi()
 
     # Calculate demand by running gravity model
-    net.run_gravity_model(zone_prod_attr, zone_od_distance_matrix)
+    net.run_gravity_model()
 
     # Save demand, zone, updated node, updated poi to csv
     net.save_results_to_csv(overwrite_file=True)
 ```
 
 # Generate Demand with node.csv, poi.csv and zone.csv (x_coord, y_coord fields represent zone centroids)
 
@@ -130,18 +136,21 @@
     # load network: node and poi
     net.load_network()
 
     # Generate zone
     net.taz2zone()
 
     # Synchronize geometry info between zone, node and poi
+    # if you want to save updated node, poi, zone without demand,
+    # you can skip net.run_gravity_model()
+    # and run net.save_results_to_csv(overwrite_file=True) directly
     net.sync_geometry_between_zone_and_node_poi()
 
     # Calculate demand by running gravity model
-    net.run_gravity_model(zone_prod_attr, zone_od_distance_matrix)
+    net.run_gravity_model()
 
     # Save demand, zone, updated node, updated poi to csv
     net.save_results_to_csv(overwrite_file=True)
 ```
 
 # Generate Demand with node.csv (if zone_id field exist, generated zone boundary cover zone_id that are not empty) and poi.csv
 
@@ -162,14 +171,17 @@
     net.load_network()
 
     # Generate zone dictionary from node dictionary by specifying number of x blocks and y blocks
     net.net2zone(num_x_blocks=10, num_y_blocks=10)
     # net.net2zone(cell_width=10, cell_height=10, unit="km")
 
     # Synchronize geometry info between zone, node and poi
+    # if you want to save updated node, poi, zone without demand,
+    # you can skip net.run_gravity_model()
+    # and run net.save_results_to_csv(overwrite_file=True) directly
     net.sync_geometry_between_zone_and_node_poi()
 
     # Calculate demand by running gravity model
     net.run_gravity_model(zone_prod_attr, zone_od_distance_matrix)
 
     # Save demand, zone, updated node, updated poi to csv
     net.save_results_to_csv(overwrite_file=True)
```

### Comparing `grid2demand-0.4.4/README.md` & `grid2demand-0.4.5/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -63,18 +63,21 @@
     net.load_network()
 
     # Generate zone dictionary from node dictionary by specifying number of x blocks and y blocks
     net.net2zone(num_x_blocks=10, num_y_blocks=10)
     # net.net2zone(cell_width=10, cell_height=10, unit="km")
 
     # Synchronize geometry info between zone, node and poi
+    # if you want to save updated node, poi, zone without demand,
+    # you can skip net.run_gravity_model()
+    # and run net.save_results_to_csv(overwrite_file=True) directly
     net.sync_geometry_between_zone_and_node_poi()
 
     # Calculate demand by running gravity model
-    net.run_gravity_model(zone_prod_attr, zone_od_distance_matrix)
+    net.run_gravity_model()
 
     # Save demand, zone, updated node, updated poi to csv
     net.save_results_to_csv(overwrite_file=True)
 ```
 
 #### **Generate Demand with node.csv, poi.csv and zone.csv (geometry filed in zone.csv)**
 
@@ -95,18 +98,21 @@
     # load network: node and poi
     net.load_network()
 
     # Generate zone
     net.taz2zone()
 
     # Synchronize geometry info between zone, node and poi
+    # if you want to save updated node, poi, zone without demand,
+    # you can skip net.run_gravity_model()
+    # and run net.save_results_to_csv(overwrite_file=True) directly
     net.sync_geometry_between_zone_and_node_poi()
 
     # Calculate demand by running gravity model
-    net.run_gravity_model(zone_prod_attr, zone_od_distance_matrix)
+    net.run_gravity_model()
 
     # Save demand, zone, updated node, updated poi to csv
     net.save_results_to_csv(overwrite_file=True)
 ```
 
 #### **Generate Demand with node.csv, poi.csv and zone.csv (x_coord, y_coord fields represent zone centroids)**
 
@@ -127,18 +133,21 @@
     # load network: node and poi
     net.load_network()
 
     # Generate zone
     net.taz2zone()
 
     # Synchronize geometry info between zone, node and poi
+    # if you want to save updated node, poi, zone without demand,
+    # you can skip net.run_gravity_model()
+    # and run net.save_results_to_csv(overwrite_file=True) directly
     net.sync_geometry_between_zone_and_node_poi()
 
     # Calculate demand by running gravity model
-    net.run_gravity_model(zone_prod_attr, zone_od_distance_matrix)
+    net.run_gravity_model()
 
     # Save demand, zone, updated node, updated poi to csv
     net.save_results_to_csv(overwrite_file=True)
 ```
 
 #### **Generate Demand with node.csv (if zone_id field exist, generated zone boundary cover zone_id that are not empty) and poi.csv**
 
@@ -159,18 +168,21 @@
     net.load_network()
 
     # Generate zone dictionary from node dictionary by specifying number of x blocks and y blocks
     net.net2zone(num_x_blocks=10, num_y_blocks=10)
     # net.net2zone(cell_width=10, cell_height=10, unit="km")
 
     # Synchronize geometry info between zone, node and poi
+    # if you want to save updated node, poi, zone without demand,
+    # you can skip net.run_gravity_model()
+    # and run net.save_results_to_csv(overwrite_file=True) directly
     net.sync_geometry_between_zone_and_node_poi()
 
     # Calculate demand by running gravity model
-    net.run_gravity_model(zone_prod_attr, zone_od_distance_matrix)
+    net.run_gravity_model()
 
     # Save demand, zone, updated node, updated poi to csv
     net.save_results_to_csv(overwrite_file=True)
 ```
 
 ### **Call for Contributions**
```

### Comparing `grid2demand-0.4.4/grid2demand/__init__.py` & `grid2demand-0.4.5/grid2demand/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
                                 calc_zone_od_matrix)
 from .func_lib.gravity_model import (run_gravity_model,
                                      calc_zone_production_attraction)
 from .func_lib.gen_agent_demand import gen_agent_based_demand
 from .utils_lib.pkg_settings import pkg_settings
 from ._grid2demand import GRID2DEMAND
 
-print('grid2demand, version 0.4.3')
+print('grid2demand, version 0.4.5')
 print("Python version for running the model is 3.10 or higher")
 
 
 __all__ = ["read_node", "read_poi", "read_network",
            "read_zone_by_geometry", "read_zone_by_centroid",
            "gen_poi_trip_rate", "gen_node_prod_attr",
            "net2zone",
```

### Comparing `grid2demand-0.4.4/grid2demand/_grid2demand.py` & `grid2demand-0.4.5/grid2demand/_grid2demand.py`

 * *Files identical despite different names*

### Comparing `grid2demand-0.4.4/grid2demand/func_lib/gen_agent_demand.py` & `grid2demand-0.4.5/grid2demand/func_lib/gen_agent_demand.py`

 * *Files identical despite different names*

### Comparing `grid2demand-0.4.4/grid2demand/func_lib/gen_zone.py` & `grid2demand-0.4.5/grid2demand/func_lib/gen_zone.py`

 * *Files identical despite different names*

### Comparing `grid2demand-0.4.4/grid2demand/func_lib/gravity_model.py` & `grid2demand-0.4.5/grid2demand/func_lib/gravity_model.py`

 * *Files identical despite different names*

### Comparing `grid2demand-0.4.4/grid2demand/func_lib/read_node_poi.py` & `grid2demand-0.4.5/grid2demand/func_lib/read_node_poi.py`

 * *Files identical despite different names*

### Comparing `grid2demand-0.4.4/grid2demand/func_lib/trip_rate_production_attraction.py` & `grid2demand-0.4.5/grid2demand/func_lib/trip_rate_production_attraction.py`

 * *Files identical despite different names*

### Comparing `grid2demand-0.4.4/grid2demand/utils_lib/net_utils.py` & `grid2demand-0.4.5/grid2demand/utils_lib/net_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -66,15 +66,15 @@
     x_coord: float = 0
     y_coord: float = 0
     count: int = 1
     area: list = field(default_factory=list)
     poi_type: str = ''
     trip_rate: dict = field(default_factory=dict)
     geometry: str = ''
-    zone_id: int = 0
+    zone_id: int = -1
 
     @property
     def as_dict(self):
         return asdict(self)
 
 
 @dataclass
```

### Comparing `grid2demand-0.4.4/grid2demand/utils_lib/pkg_settings.py` & `grid2demand-0.4.5/grid2demand/utils_lib/pkg_settings.py`

 * *Files identical despite different names*

### Comparing `grid2demand-0.4.4/grid2demand/utils_lib/utils.py` & `grid2demand-0.4.5/grid2demand/utils_lib/utils.py`

 * *Files identical despite different names*

### Comparing `grid2demand-0.4.4/grid2demand.egg-info/PKG-INFO` & `grid2demand-0.4.5/grid2demand.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: grid2demand
-Version: 0.4.4
+Version: 0.4.5
 Summary: A tool for generating zone-to-zone travel demand based on grid cells or TAZs and gravity model
 Home-page: https://github.com/xyluo25/grid2demand
 Author: Xiangyong Luo, Dr.Xuesong(Simon) Zhou
 Author-email: luoxiangyong01@gmail.com, xzhou74@asu.edu
 Project-URL: Homepage, https://github.com/asu-trans-ai-lab/grid2demand
 Project-URL: Documentation, https://github.com/asu-trans-ai-lab/grid2demand
 Classifier: Programming Language :: Python :: 3
@@ -66,18 +66,21 @@
     net.load_network()
 
     # Generate zone dictionary from node dictionary by specifying number of x blocks and y blocks
     net.net2zone(num_x_blocks=10, num_y_blocks=10)
     # net.net2zone(cell_width=10, cell_height=10, unit="km")
 
     # Synchronize geometry info between zone, node and poi
+    # if you want to save updated node, poi, zone without demand,
+    # you can skip net.run_gravity_model()
+    # and run net.save_results_to_csv(overwrite_file=True) directly
     net.sync_geometry_between_zone_and_node_poi()
 
     # Calculate demand by running gravity model
-    net.run_gravity_model(zone_prod_attr, zone_od_distance_matrix)
+    net.run_gravity_model()
 
     # Save demand, zone, updated node, updated poi to csv
     net.save_results_to_csv(overwrite_file=True)
 ```
 
 # Generate Demand with node.csv, poi.csv and zone.csv (geometry filed in zone.csv)
 
@@ -98,18 +101,21 @@
     # load network: node and poi
     net.load_network()
 
     # Generate zone
     net.taz2zone()
 
     # Synchronize geometry info between zone, node and poi
+    # if you want to save updated node, poi, zone without demand,
+    # you can skip net.run_gravity_model()
+    # and run net.save_results_to_csv(overwrite_file=True) directly
     net.sync_geometry_between_zone_and_node_poi()
 
     # Calculate demand by running gravity model
-    net.run_gravity_model(zone_prod_attr, zone_od_distance_matrix)
+    net.run_gravity_model()
 
     # Save demand, zone, updated node, updated poi to csv
     net.save_results_to_csv(overwrite_file=True)
 ```
 
 # Generate Demand with node.csv, poi.csv and zone.csv (x_coord, y_coord fields represent zone centroids)
 
@@ -130,18 +136,21 @@
     # load network: node and poi
     net.load_network()
 
     # Generate zone
     net.taz2zone()
 
     # Synchronize geometry info between zone, node and poi
+    # if you want to save updated node, poi, zone without demand,
+    # you can skip net.run_gravity_model()
+    # and run net.save_results_to_csv(overwrite_file=True) directly
     net.sync_geometry_between_zone_and_node_poi()
 
     # Calculate demand by running gravity model
-    net.run_gravity_model(zone_prod_attr, zone_od_distance_matrix)
+    net.run_gravity_model()
 
     # Save demand, zone, updated node, updated poi to csv
     net.save_results_to_csv(overwrite_file=True)
 ```
 
 # Generate Demand with node.csv (if zone_id field exist, generated zone boundary cover zone_id that are not empty) and poi.csv
 
@@ -162,14 +171,17 @@
     net.load_network()
 
     # Generate zone dictionary from node dictionary by specifying number of x blocks and y blocks
     net.net2zone(num_x_blocks=10, num_y_blocks=10)
     # net.net2zone(cell_width=10, cell_height=10, unit="km")
 
     # Synchronize geometry info between zone, node and poi
+    # if you want to save updated node, poi, zone without demand,
+    # you can skip net.run_gravity_model()
+    # and run net.save_results_to_csv(overwrite_file=True) directly
     net.sync_geometry_between_zone_and_node_poi()
 
     # Calculate demand by running gravity model
     net.run_gravity_model(zone_prod_attr, zone_od_distance_matrix)
 
     # Save demand, zone, updated node, updated poi to csv
     net.save_results_to_csv(overwrite_file=True)
```

### Comparing `grid2demand-0.4.4/grid2demand.egg-info/SOURCES.txt` & `grid2demand-0.4.5/grid2demand.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `grid2demand-0.4.4/setup.py` & `grid2demand-0.4.5/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     with open("requirements.txt", "r", encoding="utf-8") as f:
         modules_needed = [i.strip() for i in f.readlines()]
 except Exception:
     modules_needed = []
 
 setuptools.setup(
     name="grid2demand",  # Replace with your own username
-    version="0.4.4",
+    version="0.4.5",
     author="Xiangyong Luo, Dr.Xuesong(Simon) Zhou",
     author_email="luoxiangyong01@gmail.com, xzhou74@asu.edu",
     description="A tool for generating zone-to-zone travel demand based on grid cells or TAZs and gravity model",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/xyluo25/grid2demand",
```

### Comparing `grid2demand-0.4.4/tests/test_read_node.py` & `grid2demand-0.4.5/tests/test_read_node.py`

 * *Files identical despite different names*

