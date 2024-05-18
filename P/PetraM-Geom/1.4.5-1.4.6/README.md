# Comparing `tmp/petram_geom-1.4.5.tar.gz` & `tmp/petram_geom-1.4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "petram_geom-1.4.5.tar", last modified: Thu Apr 25 14:23:19 2024, max compression
+gzip compressed data, was "petram_geom-1.4.6.tar", last modified: Sat May 18 14:57:39 2024, max compression
```

## Comparing `petram_geom-1.4.5.tar` & `petram_geom-1.4.6.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 14:23:19.327198 petram_geom-1.4.5/
--rw-r--r--   0 runner    (1001) docker     (127)    35148 2024-04-25 14:23:11.000000 petram_geom-1.4.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      948 2024-04-25 14:23:19.327198 petram_geom-1.4.5/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 14:23:19.327198 petram_geom-1.4.5/PetraM_Geom.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      948 2024-04-25 14:23:19.000000 petram_geom-1.4.5/PetraM_Geom.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1006 2024-04-25 14:23:19.000000 petram_geom-1.4.5/PetraM_Geom.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 14:23:19.000000 petram_geom-1.4.5/PetraM_Geom.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-25 14:23:19.000000 petram_geom-1.4.5/PetraM_Geom.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      176 2024-04-25 14:23:11.000000 petram_geom-1.4.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 14:23:19.319198 petram_geom-1.4.5/petram/
--rw-r--r--   0 runner    (1001) docker     (127)      249 2024-04-25 14:23:11.000000 petram_geom-1.4.5/petram/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 14:23:19.323198 petram_geom-1.4.5/petram/geom/
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-25 14:23:11.000000 petram_geom-1.4.5/petram/geom/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1899 2024-04-25 14:23:11.000000 petram_geom-1.4.5/petram/geom/geom_id.py
--rw-r--r--   0 runner    (1001) docker     (127)     6233 2024-04-25 14:23:11.000000 petram_geom-1.4.5/petram/geom/geom_info_palette.py
--rw-r--r--   0 runner    (1001) docker     (127)     1460 2024-04-25 14:23:11.000000 petram_geom-1.4.5/petram/geom/geom_model.py
--rw-r--r--   0 runner    (1001) docker     (127)   106477 2024-04-25 14:23:11.000000 petram_geom-1.4.5/petram/geom/geom_primitives.py
--rw-r--r--   0 runner    (1001) docker     (127)     6295 2024-04-25 14:23:11.000000 petram_geom-1.4.5/petram/geom/geom_sel_buttons.py
--rw-r--r--   0 runner    (1001) docker     (127)    10313 2024-04-25 14:23:11.000000 petram_geom-1.4.5/petram/geom/geom_sequence_operator.py
--rw-r--r--   0 runner    (1001) docker     (127)    21288 2024-04-25 14:23:11.000000 petram_geom-1.4.5/petram/geom/geom_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-04-25 14:23:11.000000 petram_geom-1.4.5/petram/geom/gmsh_config.py
--rw-r--r--   0 runner    (1001) docker     (127)    31394 2024-04-25 14:23:11.000000 petram_geom-1.4.5/petram/geom/gmsh_geom_model.py
--rw-r--r--   0 runner    (1001) docker     (127)   101674 2024-04-25 14:23:11.000000 petram_geom-1.4.5/petram/geom/gmsh_geom_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-04-25 14:23:11.000000 petram_geom-1.4.5/petram/geom/gmsh_primitives.py
--rw-r--r--   0 runner    (1001) docker     (127)    32106 2024-04-25 14:23:11.000000 petram_geom-1.4.5/petram/geom/occ_cbook.py
--rw-r--r--   0 runner    (1001) docker     (127)    16603 2024-04-25 14:23:11.000000 petram_geom-1.4.5/petram/geom/occ_geom_model.py
--rw-r--r--   0 runner    (1001) docker     (127)   204117 2024-04-25 14:23:11.000000 petram_geom-1.4.5/petram/geom/occ_geom_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (127)     7139 2024-04-25 14:23:11.000000 petram_geom-1.4.5/petram/geom/occ_heal_extra.py
--rw-r--r--   0 runner    (1001) docker     (127)    11334 2024-04-25 14:23:11.000000 petram_geom-1.4.5/petram/geom/occ_heal_shape.py
--rw-r--r--   0 runner    (1001) docker     (127)    13298 2024-04-25 14:23:11.000000 petram_geom-1.4.5/petram/geom/occ_inspect.py
--rw-r--r--   0 runner    (1001) docker     (127)    15549 2024-04-25 14:23:11.000000 petram_geom-1.4.5/petram/geom/read_brep_occ.py
--rw-r--r--   0 runner    (1001) docker     (127)    14807 2024-04-25 14:23:11.000000 petram_geom-1.4.5/petram/geom/read_gmsh.py
--rw-r--r--   0 runner    (1001) docker     (127)    18808 2024-04-25 14:23:11.000000 petram_geom-1.4.5/petram/geom/vtable_geom.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 14:23:19.327198 petram_geom-1.4.5/petram/mesh/
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-04-25 14:23:11.000000 petram_geom-1.4.5/petram/mesh/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14488 2024-04-25 14:23:11.000000 petram_geom-1.4.5/petram/mesh/gmsh2mfem.py
--rw-r--r--   0 runner    (1001) docker     (127)     3784 2024-04-25 14:23:11.000000 petram_geom-1.4.5/petram/mesh/gmsh_helper.py
--rw-r--r--   0 runner    (1001) docker     (127)    30212 2024-04-25 14:23:11.000000 petram_geom-1.4.5/petram/mesh/gmsh_mesh_actions.py
--rw-r--r--   0 runner    (1001) docker     (127)    31106 2024-04-25 14:23:11.000000 petram_geom-1.4.5/petram/mesh/gmsh_mesh_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    94896 2024-04-25 14:23:11.000000 petram_geom-1.4.5/petram/mesh/gmsh_mesh_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (127)     5164 2024-04-25 14:23:11.000000 petram_geom-1.4.5/petram/mesh/mesh_sequence_operator.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-25 14:23:19.327198 petram_geom-1.4.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1472 2024-04-25 14:23:11.000000 petram_geom-1.4.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 14:57:39.157317 petram_geom-1.4.6/
+-rw-r--r--   0 runner    (1001) docker     (127)    35148 2024-05-18 14:57:31.000000 petram_geom-1.4.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      706 2024-05-18 14:57:39.157317 petram_geom-1.4.6/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 14:57:39.157317 petram_geom-1.4.6/PetraM_Geom.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      706 2024-05-18 14:57:39.000000 petram_geom-1.4.6/PetraM_Geom.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1006 2024-05-18 14:57:39.000000 petram_geom-1.4.6/PetraM_Geom.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-18 14:57:39.000000 petram_geom-1.4.6/PetraM_Geom.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-18 14:57:39.000000 petram_geom-1.4.6/PetraM_Geom.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      176 2024-05-18 14:57:31.000000 petram_geom-1.4.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 14:57:39.149317 petram_geom-1.4.6/petram/
+-rw-r--r--   0 runner    (1001) docker     (127)      249 2024-05-18 14:57:31.000000 petram_geom-1.4.6/petram/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 14:57:39.153317 petram_geom-1.4.6/petram/geom/
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-18 14:57:31.000000 petram_geom-1.4.6/petram/geom/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1899 2024-05-18 14:57:31.000000 petram_geom-1.4.6/petram/geom/geom_id.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6233 2024-05-18 14:57:31.000000 petram_geom-1.4.6/petram/geom/geom_info_palette.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1460 2024-05-18 14:57:31.000000 petram_geom-1.4.6/petram/geom/geom_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)   106477 2024-05-18 14:57:31.000000 petram_geom-1.4.6/petram/geom/geom_primitives.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6295 2024-05-18 14:57:31.000000 petram_geom-1.4.6/petram/geom/geom_sel_buttons.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10313 2024-05-18 14:57:31.000000 petram_geom-1.4.6/petram/geom/geom_sequence_operator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21288 2024-05-18 14:57:31.000000 petram_geom-1.4.6/petram/geom/geom_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-05-18 14:57:31.000000 petram_geom-1.4.6/petram/geom/gmsh_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31394 2024-05-18 14:57:31.000000 petram_geom-1.4.6/petram/geom/gmsh_geom_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)   101674 2024-05-18 14:57:31.000000 petram_geom-1.4.6/petram/geom/gmsh_geom_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-05-18 14:57:31.000000 petram_geom-1.4.6/petram/geom/gmsh_primitives.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32106 2024-05-18 14:57:31.000000 petram_geom-1.4.6/petram/geom/occ_cbook.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16603 2024-05-18 14:57:31.000000 petram_geom-1.4.6/petram/geom/occ_geom_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)   204117 2024-05-18 14:57:31.000000 petram_geom-1.4.6/petram/geom/occ_geom_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7139 2024-05-18 14:57:31.000000 petram_geom-1.4.6/petram/geom/occ_heal_extra.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11334 2024-05-18 14:57:31.000000 petram_geom-1.4.6/petram/geom/occ_heal_shape.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13298 2024-05-18 14:57:31.000000 petram_geom-1.4.6/petram/geom/occ_inspect.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15549 2024-05-18 14:57:31.000000 petram_geom-1.4.6/petram/geom/read_brep_occ.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14807 2024-05-18 14:57:31.000000 petram_geom-1.4.6/petram/geom/read_gmsh.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18808 2024-05-18 14:57:31.000000 petram_geom-1.4.6/petram/geom/vtable_geom.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 14:57:39.157317 petram_geom-1.4.6/petram/mesh/
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-05-18 14:57:31.000000 petram_geom-1.4.6/petram/mesh/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14488 2024-05-18 14:57:31.000000 petram_geom-1.4.6/petram/mesh/gmsh2mfem.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3784 2024-05-18 14:57:31.000000 petram_geom-1.4.6/petram/mesh/gmsh_helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30212 2024-05-18 14:57:31.000000 petram_geom-1.4.6/petram/mesh/gmsh_mesh_actions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31106 2024-05-18 14:57:31.000000 petram_geom-1.4.6/petram/mesh/gmsh_mesh_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    94902 2024-05-18 14:57:31.000000 petram_geom-1.4.6/petram/mesh/gmsh_mesh_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5164 2024-05-18 14:57:31.000000 petram_geom-1.4.6/petram/mesh/mesh_sequence_operator.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-18 14:57:39.157317 petram_geom-1.4.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1221 2024-05-18 14:57:31.000000 petram_geom-1.4.6/setup.py
```

### Comparing `petram_geom-1.4.5/LICENSE` & `petram_geom-1.4.6/LICENSE`

 * *Files identical despite different names*

### Comparing `petram_geom-1.4.5/PetraM_Geom.egg-info/SOURCES.txt` & `petram_geom-1.4.6/PetraM_Geom.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `petram_geom-1.4.5/petram/geom/geom_id.py` & `petram_geom-1.4.6/petram/geom/geom_id.py`

 * *Files identical despite different names*

### Comparing `petram_geom-1.4.5/petram/geom/geom_info_palette.py` & `petram_geom-1.4.6/petram/geom/geom_info_palette.py`

 * *Files identical despite different names*

### Comparing `petram_geom-1.4.5/petram/geom/geom_model.py` & `petram_geom-1.4.6/petram/geom/geom_model.py`

 * *Files identical despite different names*

### Comparing `petram_geom-1.4.5/petram/geom/geom_primitives.py` & `petram_geom-1.4.6/petram/geom/geom_primitives.py`

 * *Files identical despite different names*

### Comparing `petram_geom-1.4.5/petram/geom/geom_sel_buttons.py` & `petram_geom-1.4.6/petram/geom/geom_sel_buttons.py`

 * *Files identical despite different names*

### Comparing `petram_geom-1.4.5/petram/geom/geom_sequence_operator.py` & `petram_geom-1.4.6/petram/geom/geom_sequence_operator.py`

 * *Files identical despite different names*

### Comparing `petram_geom-1.4.5/petram/geom/geom_utils.py` & `petram_geom-1.4.6/petram/geom/geom_utils.py`

 * *Files identical despite different names*

### Comparing `petram_geom-1.4.5/petram/geom/gmsh_geom_model.py` & `petram_geom-1.4.6/petram/geom/gmsh_geom_model.py`

 * *Files identical despite different names*

### Comparing `petram_geom-1.4.5/petram/geom/gmsh_geom_wrapper.py` & `petram_geom-1.4.6/petram/geom/gmsh_geom_wrapper.py`

 * *Files identical despite different names*

### Comparing `petram_geom-1.4.5/petram/geom/occ_cbook.py` & `petram_geom-1.4.6/petram/geom/occ_cbook.py`

 * *Files identical despite different names*

### Comparing `petram_geom-1.4.5/petram/geom/occ_geom_model.py` & `petram_geom-1.4.6/petram/geom/occ_geom_model.py`

 * *Files identical despite different names*

### Comparing `petram_geom-1.4.5/petram/geom/occ_geom_wrapper.py` & `petram_geom-1.4.6/petram/geom/occ_geom_wrapper.py`

 * *Files identical despite different names*

### Comparing `petram_geom-1.4.5/petram/geom/occ_heal_extra.py` & `petram_geom-1.4.6/petram/geom/occ_heal_extra.py`

 * *Files identical despite different names*

### Comparing `petram_geom-1.4.5/petram/geom/occ_heal_shape.py` & `petram_geom-1.4.6/petram/geom/occ_heal_shape.py`

 * *Files identical despite different names*

### Comparing `petram_geom-1.4.5/petram/geom/occ_inspect.py` & `petram_geom-1.4.6/petram/geom/occ_inspect.py`

 * *Files identical despite different names*

### Comparing `petram_geom-1.4.5/petram/geom/read_brep_occ.py` & `petram_geom-1.4.6/petram/geom/read_brep_occ.py`

 * *Files identical despite different names*

### Comparing `petram_geom-1.4.5/petram/geom/read_gmsh.py` & `petram_geom-1.4.6/petram/geom/read_gmsh.py`

 * *Files identical despite different names*

### Comparing `petram_geom-1.4.5/petram/geom/vtable_geom.py` & `petram_geom-1.4.6/petram/geom/vtable_geom.py`

 * *Files identical despite different names*

### Comparing `petram_geom-1.4.5/petram/mesh/gmsh2mfem.py` & `petram_geom-1.4.6/petram/mesh/gmsh2mfem.py`

 * *Files identical despite different names*

### Comparing `petram_geom-1.4.5/petram/mesh/gmsh_helper.py` & `petram_geom-1.4.6/petram/mesh/gmsh_helper.py`

 * *Files identical despite different names*

### Comparing `petram_geom-1.4.5/petram/mesh/gmsh_mesh_actions.py` & `petram_geom-1.4.6/petram/mesh/gmsh_mesh_actions.py`

 * *Files identical despite different names*

### Comparing `petram_geom-1.4.5/petram/mesh/gmsh_mesh_model.py` & `petram_geom-1.4.6/petram/mesh/gmsh_mesh_model.py`

 * *Files identical despite different names*

### Comparing `petram_geom-1.4.5/petram/mesh/gmsh_mesh_wrapper.py` & `petram_geom-1.4.6/petram/mesh/gmsh_mesh_wrapper.py`

 * *Files 0% similar despite different names*

```diff
@@ -775,15 +775,15 @@
 
     def check_algorith_dim(self):
         dims = {'cl': 0,
                 'freevolume': 3,
                 'freeface': 2,
                 'freeedge': 1,
                 'transfinite_volume': 3,
-                'transfinite_face': 2,
+                'transfinite_surface': 2,
                 'transfinite_edge': 1,
                 'recombine_surface': 0,
                 'copyface': 2,
                 'extrude_face': 2,
                 'revolve_face': 2,
                 'mergetxt': 0,
                 }
@@ -796,15 +796,15 @@
 
     def check_need_optimize(self):
         dims = {'cl': 0,
                 'freevolume': 1,
                 'freeface': 1,
                 'freeedge': 1,
                 'transfinite_volume': 0,
-                'transfinite_face': 0,
+                'transfinite_surface': 0,
                 'transfinite_edge': 0,
                 'recombine_surface': 0,
                 'copyface': 0,
                 'extrude_face': 0,
                 'revolve_face': 0,
                 'mergetxt': 0,
                 }
```

### Comparing `petram_geom-1.4.5/petram/mesh/mesh_sequence_operator.py` & `petram_geom-1.4.6/petram/mesh/mesh_sequence_operator.py`

 * *Files identical despite different names*

### Comparing `petram_geom-1.4.5/setup.py` & `petram_geom-1.4.6/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -13,37 +13,32 @@
 
 with open(path.join(here, 'README.md')) as f:
     long_description = f.read()
 
 setup(
     name='PetraM_Geom',
 
-    version='1.4.5',
+    version='1.4.6',
 
     description='PetraM Geometry Package',
     long_description=long_description,
-    long_description_content_type = 'text/markdown',
     url='https://github.com/piScope/PetraM',
     author='S. Sihraiwa',
     author_email='shiraiwa@psfc.mit.edu',
     license='GNUv3',
 
     classifiers=[
         #   3 - Alpha
         #   4 - Beta
         #   5 - Production/Stable
         'Development Status :: 3 - Alpha',
         'Intended Audience :: Developers',
         'Topic :: Scientific/Engineering :: Physics',
         'License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)',
-        'Programming Language :: Python :: 3.7',
-        'Programming Language :: Python :: 3.8',
-        'Programming Language :: Python :: 3.9',
-        'Programming Language :: Python :: 3.10',
-        'Programming Language :: Python :: 3.11',
+        'Programming Language :: Python :: 2.7',
     ],
 
     keywords='MFEM physics',
     packages=find_packages(exclude=['contrib', 'docs', 'tests']),
     install_requires=[],
     extras_require={},
     data_files=[],
```

