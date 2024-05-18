# Comparing `tmp/jsrm-0.0.7.tar.gz` & `tmp/jsrm-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jsrm-0.0.7.tar", last modified: Fri May  3 09:40:00 2024, max compression
+gzip compressed data, was "jsrm-0.0.8.tar", last modified: Fri May 17 17:14:10 2024, max compression
```

## Comparing `jsrm-0.0.7.tar` & `jsrm-0.0.8.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 09:40:00.377231 jsrm-0.0.7/
--rw-r--r--   0 runner    (1001) docker     (127)     1081 2024-05-03 09:39:52.000000 jsrm-0.0.7/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     6051 2024-05-03 09:40:00.377231 jsrm-0.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2758 2024-05-03 09:39:52.000000 jsrm-0.0.7/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     6710 2024-05-03 09:39:52.000000 jsrm-0.0.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-03 09:40:00.377231 jsrm-0.0.7/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 09:40:00.369231 jsrm-0.0.7/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 09:40:00.369231 jsrm-0.0.7/src/jsrm/
--rw-r--r--   0 runner    (1001) docker     (127)      188 2024-05-03 09:39:52.000000 jsrm-0.0.7/src/jsrm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3374 2024-05-03 09:39:52.000000 jsrm-0.0.7/src/jsrm/integration.py
--rw-r--r--   0 runner    (1001) docker     (127)     1338 2024-05-03 09:39:52.000000 jsrm-0.0.7/src/jsrm/math_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 09:40:00.373231 jsrm-0.0.7/src/jsrm/parameters/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 09:39:52.000000 jsrm-0.0.7/src/jsrm/parameters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15530 2024-05-03 09:39:52.000000 jsrm-0.0.7/src/jsrm/parameters/hsa_params.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 09:40:00.373231 jsrm-0.0.7/src/jsrm/rendering/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 09:39:52.000000 jsrm-0.0.7/src/jsrm/rendering/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 09:40:00.373231 jsrm-0.0.7/src/jsrm/rendering/planar_hsa/
--rw-r--r--   0 runner    (1001) docker     (127)     9469 2024-05-03 09:39:52.000000 jsrm-0.0.7/src/jsrm/rendering/planar_hsa/opencv_renderer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 09:40:00.373231 jsrm-0.0.7/src/jsrm/symbolic_derivation/
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-05-03 09:39:52.000000 jsrm-0.0.7/src/jsrm/symbolic_derivation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5374 2024-05-03 09:39:52.000000 jsrm-0.0.7/src/jsrm/symbolic_derivation/pendulum.py
--rw-r--r--   0 runner    (1001) docker     (127)    26256 2024-05-03 09:39:52.000000 jsrm-0.0.7/src/jsrm/symbolic_derivation/planar_hsa.py
--rw-r--r--   0 runner    (1001) docker     (127)     6339 2024-05-03 09:39:52.000000 jsrm-0.0.7/src/jsrm/symbolic_derivation/planar_pcs.py
--rw-r--r--   0 runner    (1001) docker     (127)     1864 2024-05-03 09:39:52.000000 jsrm-0.0.7/src/jsrm/symbolic_derivation/symbolic_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 09:40:00.373231 jsrm-0.0.7/src/jsrm/symbolic_expressions/
--rw-r--r--   0 runner    (1001) docker     (127)     1355 2024-05-03 09:39:52.000000 jsrm-0.0.7/src/jsrm/symbolic_expressions/pendulum_nl-1.dill
--rw-r--r--   0 runner    (1001) docker     (127)     2262 2024-05-03 09:39:52.000000 jsrm-0.0.7/src/jsrm/symbolic_expressions/pendulum_nl-2.dill
--rw-r--r--   0 runner    (1001) docker     (127)     4194 2024-05-03 09:39:52.000000 jsrm-0.0.7/src/jsrm/symbolic_expressions/pendulum_nl-3.dill
--rw-r--r--   0 runner    (1001) docker     (127)    52619 2024-05-03 09:39:52.000000 jsrm-0.0.7/src/jsrm/symbolic_expressions/planar_hsa_ns-1_nrs-2.dill
--rw-r--r--   0 runner    (1001) docker     (127)    86067 2024-05-03 09:39:52.000000 jsrm-0.0.7/src/jsrm/symbolic_expressions/planar_hsa_ns-1_nrs-4.dill
--rw-r--r--   0 runner    (1001) docker     (127)     5057 2024-05-03 09:39:52.000000 jsrm-0.0.7/src/jsrm/symbolic_expressions/planar_pcs_ns-1.dill
--rw-r--r--   0 runner    (1001) docker     (127)    43433 2024-05-03 09:39:52.000000 jsrm-0.0.7/src/jsrm/symbolic_expressions/planar_pcs_ns-2.dill
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 09:40:00.377231 jsrm-0.0.7/src/jsrm/systems/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 09:39:52.000000 jsrm-0.0.7/src/jsrm/systems/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3068 2024-05-03 09:39:52.000000 jsrm-0.0.7/src/jsrm/systems/euler_lagrangian.py
--rw-r--r--   0 runner    (1001) docker     (127)     5166 2024-05-03 09:39:52.000000 jsrm-0.0.7/src/jsrm/systems/pendulum.py
--rw-r--r--   0 runner    (1001) docker     (127)    31773 2024-05-03 09:39:52.000000 jsrm-0.0.7/src/jsrm/systems/planar_hsa.py
--rw-r--r--   0 runner    (1001) docker     (127)     9233 2024-05-03 09:39:52.000000 jsrm-0.0.7/src/jsrm/systems/planar_pcs.py
--rw-r--r--   0 runner    (1001) docker     (127)     4332 2024-05-03 09:39:52.000000 jsrm-0.0.7/src/jsrm/systems/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      501 2024-05-03 09:39:52.000000 jsrm-0.0.7/src/jsrm/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 09:40:00.377231 jsrm-0.0.7/src/jsrm.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6051 2024-05-03 09:40:00.000000 jsrm-0.0.7/src/jsrm.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1238 2024-05-03 09:40:00.000000 jsrm-0.0.7/src/jsrm.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 09:40:00.000000 jsrm-0.0.7/src/jsrm.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      244 2024-05-03 09:40:00.000000 jsrm-0.0.7/src/jsrm.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-03 09:40:00.000000 jsrm-0.0.7/src/jsrm.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 09:40:00.377231 jsrm-0.0.7/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2060 2024-05-03 09:39:52.000000 jsrm-0.0.7/tests/test_planar_hsa.py
--rw-r--r--   0 runner    (1001) docker     (127)     2767 2024-05-03 09:39:52.000000 jsrm-0.0.7/tests/test_planar_pcs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 17:14:10.594300 jsrm-0.0.8/
+-rw-r--r--   0 runner    (1001) docker     (127)     1081 2024-05-17 17:14:01.000000 jsrm-0.0.8/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     6051 2024-05-17 17:14:10.594300 jsrm-0.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2758 2024-05-17 17:14:01.000000 jsrm-0.0.8/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     6710 2024-05-17 17:14:01.000000 jsrm-0.0.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-17 17:14:10.594300 jsrm-0.0.8/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 17:14:10.582301 jsrm-0.0.8/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 17:14:10.586300 jsrm-0.0.8/src/jsrm/
+-rw-r--r--   0 runner    (1001) docker     (127)      188 2024-05-17 17:14:01.000000 jsrm-0.0.8/src/jsrm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3374 2024-05-17 17:14:01.000000 jsrm-0.0.8/src/jsrm/integration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1338 2024-05-17 17:14:01.000000 jsrm-0.0.8/src/jsrm/math_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 17:14:10.586300 jsrm-0.0.8/src/jsrm/parameters/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 17:14:01.000000 jsrm-0.0.8/src/jsrm/parameters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15530 2024-05-17 17:14:01.000000 jsrm-0.0.8/src/jsrm/parameters/hsa_params.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 17:14:10.586300 jsrm-0.0.8/src/jsrm/rendering/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 17:14:01.000000 jsrm-0.0.8/src/jsrm/rendering/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 17:14:10.586300 jsrm-0.0.8/src/jsrm/rendering/planar_hsa/
+-rw-r--r--   0 runner    (1001) docker     (127)     9469 2024-05-17 17:14:01.000000 jsrm-0.0.8/src/jsrm/rendering/planar_hsa/opencv_renderer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 17:14:10.586300 jsrm-0.0.8/src/jsrm/symbolic_derivation/
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-05-17 17:14:01.000000 jsrm-0.0.8/src/jsrm/symbolic_derivation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5374 2024-05-17 17:14:01.000000 jsrm-0.0.8/src/jsrm/symbolic_derivation/pendulum.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26256 2024-05-17 17:14:01.000000 jsrm-0.0.8/src/jsrm/symbolic_derivation/planar_hsa.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6445 2024-05-17 17:14:01.000000 jsrm-0.0.8/src/jsrm/symbolic_derivation/planar_pcs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1864 2024-05-17 17:14:01.000000 jsrm-0.0.8/src/jsrm/symbolic_derivation/symbolic_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 17:14:10.590300 jsrm-0.0.8/src/jsrm/symbolic_expressions/
+-rw-r--r--   0 runner    (1001) docker     (127)     1355 2024-05-17 17:14:01.000000 jsrm-0.0.8/src/jsrm/symbolic_expressions/pendulum_nl-1.dill
+-rw-r--r--   0 runner    (1001) docker     (127)     2262 2024-05-17 17:14:01.000000 jsrm-0.0.8/src/jsrm/symbolic_expressions/pendulum_nl-2.dill
+-rw-r--r--   0 runner    (1001) docker     (127)     4194 2024-05-17 17:14:01.000000 jsrm-0.0.8/src/jsrm/symbolic_expressions/pendulum_nl-3.dill
+-rw-r--r--   0 runner    (1001) docker     (127)    52619 2024-05-17 17:14:01.000000 jsrm-0.0.8/src/jsrm/symbolic_expressions/planar_hsa_ns-1_nrs-2.dill
+-rw-r--r--   0 runner    (1001) docker     (127)    86067 2024-05-17 17:14:01.000000 jsrm-0.0.8/src/jsrm/symbolic_expressions/planar_hsa_ns-1_nrs-4.dill
+-rw-r--r--   0 runner    (1001) docker     (127)     6739 2024-05-17 17:14:01.000000 jsrm-0.0.8/src/jsrm/symbolic_expressions/planar_pcs_ns-1.dill
+-rw-r--r--   0 runner    (1001) docker     (127)    70962 2024-05-17 17:14:01.000000 jsrm-0.0.8/src/jsrm/symbolic_expressions/planar_pcs_ns-2.dill
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 17:14:10.590300 jsrm-0.0.8/src/jsrm/systems/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 17:14:01.000000 jsrm-0.0.8/src/jsrm/systems/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3068 2024-05-17 17:14:01.000000 jsrm-0.0.8/src/jsrm/systems/euler_lagrangian.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5166 2024-05-17 17:14:01.000000 jsrm-0.0.8/src/jsrm/systems/pendulum.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31773 2024-05-17 17:14:01.000000 jsrm-0.0.8/src/jsrm/systems/planar_hsa.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12146 2024-05-17 17:14:01.000000 jsrm-0.0.8/src/jsrm/systems/planar_pcs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4332 2024-05-17 17:14:01.000000 jsrm-0.0.8/src/jsrm/systems/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      501 2024-05-17 17:14:01.000000 jsrm-0.0.8/src/jsrm/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 17:14:10.590300 jsrm-0.0.8/src/jsrm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6051 2024-05-17 17:14:10.000000 jsrm-0.0.8/src/jsrm.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1238 2024-05-17 17:14:10.000000 jsrm-0.0.8/src/jsrm.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-17 17:14:10.000000 jsrm-0.0.8/src/jsrm.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      244 2024-05-17 17:14:10.000000 jsrm-0.0.8/src/jsrm.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-17 17:14:10.000000 jsrm-0.0.8/src/jsrm.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 17:14:10.590300 jsrm-0.0.8/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2060 2024-05-17 17:14:01.000000 jsrm-0.0.8/tests/test_planar_hsa.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2782 2024-05-17 17:14:01.000000 jsrm-0.0.8/tests/test_planar_pcs.py
```

### Comparing `jsrm-0.0.7/LICENSE.txt` & `jsrm-0.0.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `jsrm-0.0.7/PKG-INFO` & `jsrm-0.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jsrm
-Version: 0.0.7
+Version: 0.0.8
 Summary: Kinematic and dynamic models of continuum and articulated soft robots.
 Author-email: Maximilian Stölzle <maximilian@stoelzle.ch>
 Maintainer-email: Maximilian Stölzle <maximilian@stoelzle.ch>
 License: Copyright (c) 2016 The Python Packaging Authority (PyPA)
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of
         this software and associated documentation files (the "Software"), to deal in
```

### Comparing `jsrm-0.0.7/README.md` & `jsrm-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `jsrm-0.0.7/pyproject.toml` & `jsrm-0.0.8/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 name = "jsrm"  # Required
 
 # Versions should comply with PEP 440:
 # https://www.python.org/dev/peps/pep-0440/
 #
 # For a discussion on single-sourcing the version, see
 # https://packaging.python.org/guides/single-sourcing-package-version/
-version = "0.0.7"  # Required
+version = "0.0.8"  # Required
 
 # This is a one-line description or tagline of what your project does. This
 # corresponds to the "Summary" metadata field:
 # https://packaging.python.org/specifications/core-metadata/#summary
 description = "Kinematic and dynamic models of continuum and articulated soft robots."  # Optional
 
 # This is an optional longer description of your project that represents
```

### Comparing `jsrm-0.0.7/src/jsrm/integration.py` & `jsrm-0.0.8/src/jsrm/integration.py`

 * *Files identical despite different names*

### Comparing `jsrm-0.0.7/src/jsrm/math_utils.py` & `jsrm-0.0.8/src/jsrm/math_utils.py`

 * *Files identical despite different names*

### Comparing `jsrm-0.0.7/src/jsrm/parameters/hsa_params.py` & `jsrm-0.0.8/src/jsrm/parameters/hsa_params.py`

 * *Files identical despite different names*

### Comparing `jsrm-0.0.7/src/jsrm/rendering/planar_hsa/opencv_renderer.py` & `jsrm-0.0.8/src/jsrm/rendering/planar_hsa/opencv_renderer.py`

 * *Files identical despite different names*

### Comparing `jsrm-0.0.7/src/jsrm/symbolic_derivation/pendulum.py` & `jsrm-0.0.8/src/jsrm/symbolic_derivation/pendulum.py`

 * *Files identical despite different names*

### Comparing `jsrm-0.0.7/src/jsrm/symbolic_derivation/planar_hsa.py` & `jsrm-0.0.8/src/jsrm/symbolic_derivation/planar_hsa.py`

 * *Files identical despite different names*

### Comparing `jsrm-0.0.7/src/jsrm/symbolic_derivation/planar_pcs.py` & `jsrm-0.0.8/src/jsrm/symbolic_derivation/planar_pcs.py`

 * *Files 2% similar despite different names*

```diff
@@ -165,17 +165,18 @@
         "exps": {
             "chi_sms": chi_sms,  # list of pose expressions (for each segment)
             "chiee": chi_sms[-1].subs(
                 s, l[-1]
             ),  # expression for end-effector pose of shape (3, )
             "J_sms": J_sms,
             "Jee": J_sms[-1].subs(s, l[-1]),
-            "B": B,
-            "C": C,
-            "G": G,
+            "B": B,  # mass matrix
+            "C": C,  # coriolis matrix
+            "G": G,  # gravity vector
+            "U": U,  # gravitational potential energy
         },
     }
 
     if filepath is not None:
         if isinstance(filepath, str):
             filepath = Path(filepath)
```

### Comparing `jsrm-0.0.7/src/jsrm/symbolic_derivation/symbolic_utils.py` & `jsrm-0.0.8/src/jsrm/symbolic_derivation/symbolic_utils.py`

 * *Files identical despite different names*

### Comparing `jsrm-0.0.7/src/jsrm/symbolic_expressions/pendulum_nl-1.dill` & `jsrm-0.0.8/src/jsrm/symbolic_expressions/pendulum_nl-1.dill`

 * *Files identical despite different names*

### Comparing `jsrm-0.0.7/src/jsrm/symbolic_expressions/pendulum_nl-2.dill` & `jsrm-0.0.8/src/jsrm/symbolic_expressions/pendulum_nl-2.dill`

 * *Files identical despite different names*

### Comparing `jsrm-0.0.7/src/jsrm/symbolic_expressions/pendulum_nl-3.dill` & `jsrm-0.0.8/src/jsrm/symbolic_expressions/pendulum_nl-3.dill`

 * *Files identical despite different names*

### Comparing `jsrm-0.0.7/src/jsrm/symbolic_expressions/planar_hsa_ns-1_nrs-2.dill` & `jsrm-0.0.8/src/jsrm/symbolic_expressions/planar_hsa_ns-1_nrs-2.dill`

 * *Files identical despite different names*

### Comparing `jsrm-0.0.7/src/jsrm/symbolic_expressions/planar_hsa_ns-1_nrs-4.dill` & `jsrm-0.0.8/src/jsrm/symbolic_expressions/planar_hsa_ns-1_nrs-4.dill`

 * *Files identical despite different names*

### Comparing `jsrm-0.0.7/src/jsrm/systems/euler_lagrangian.py` & `jsrm-0.0.8/src/jsrm/systems/euler_lagrangian.py`

 * *Files identical despite different names*

### Comparing `jsrm-0.0.7/src/jsrm/systems/pendulum.py` & `jsrm-0.0.8/src/jsrm/systems/pendulum.py`

 * *Files identical despite different names*

### Comparing `jsrm-0.0.7/src/jsrm/systems/planar_hsa.py` & `jsrm-0.0.8/src/jsrm/systems/planar_hsa.py`

 * *Files identical despite different names*

### Comparing `jsrm-0.0.7/src/jsrm/systems/planar_pcs.py` & `jsrm-0.0.8/src/jsrm/systems/planar_pcs.py`

 * *Files 15% similar despite different names*

```diff
@@ -21,27 +21,29 @@
 ) -> Tuple[
     Array,
     Callable[[Dict[str, Array], Array, Array], Array],
     Callable[
         [Dict[str, Array], Array, Array],
         Tuple[Array, Array, Array, Array, Array, Array],
     ],
+    Dict[str, Callable],
 ]:
     """
     Create jax functions from file containing symbolic expressions.
     Args:
         filepath: path to file containing symbolic expressions
         strain_selector: array of shape (n_xi, ) with boolean values indicating which components of the
                 strain are active / non-zero
         xi_eq: array of shape (3 * num_segments) with the rest strains of the rod
         global_eps: small number to avoid singularities (e.g., division by zero)
     Returns:
         B_xi: strain basis matrix of shape (3 * num_segments, n_q)
         forward_kinematics_fn: function that returns the p vector of shape (3, n_q) with the positions
         dynamical_matrices_fn: function that returns the B, C, G, K, D, and alpha matrices
+        auxiliary_fns: dictionary with auxiliary functions
     """
     # load saved symbolic data
     sym_exps = dill.load(open(str(filepath), "rb"))
 
     # symbols for robot parameters
     params_syms = sym_exps["params_syms"]
 
@@ -245,9 +247,89 @@
         K = B_xi.T @ K @ (xi - xi_eq)  # evaluate K(xi) = K @ xi
         D = B_xi.T @ D @ B_xi
 
         # apply the strain basis to the actuation matrix
         alpha = B_xi.T @ jnp.identity(n_xi) @ B_xi
 
         return B, C, G, K, D, alpha
+    
 
-    return B_xi, forward_kinematics_fn, dynamical_matrices_fn
+    def kinetic_energy_fn(params: Dict[str, Array], q: Array, q_d: Array) -> Array:
+        """
+        Compute the kinetic energy of the system.
+        Args:
+            params: Dictionary of robot parameters
+            q: generalized coordinates of shape (n_q, )
+            q_d: generalized velocities of shape (n_q, )
+        Returns:
+            T: kinetic energy of shape ()
+        """
+        B, C, G, K, D, alpha = dynamical_matrices_fn(params, q=q, q_d=q_d)
+
+        # kinetic energy
+        T = (0.5 * q_d.T @ B @ q_d).squeeze()
+        
+        return T
+
+    
+    def potential_energy_fn(params: Dict[str, Array], q: Array, eps: float = 1e4 * global_eps) -> Array:
+        """
+        Compute the potential energy of the system.
+        Args:
+            params: Dictionary of robot parameters
+            q: generalized coordinates of shape (n_q, )
+            eps: small number to avoid singularities (e.g., division by zero)
+        Returns:
+            U: potential energy of shape ()
+        """
+        # map the configuration to the strains
+        xi = xi_eq + B_xi @ q
+        # add a small number to the bending strain to avoid singularities
+        xi_epsed = apply_eps_to_bend_strains(xi, eps)
+
+        # cross-sectional area and second moment of area
+        A = jnp.pi * params["r"] ** 2
+        Ib = A**2 / (4 * jnp.pi)
+
+        # elastic and shear modulus
+        E, G = params["E"], params["G"]
+        # stiffness matrix of shape (num_segments, 3, 3)
+        S = compute_stiffness_matrix_for_all_segments_fn(A, Ib, E, G)
+        # we define the elastic matrix of shape (n_xi, n_xi) as K(xi) = K @ xi where K is equal to
+        K = blk_diag(S)
+        # elastic energy
+        U_K = (xi - xi_eq).T @ K @ (xi - xi_eq)  # evaluate K(xi) = K @ xi
+
+        # gravitational potential energy
+        U_G = sp.Matrix([[0]])
+        params_for_lambdify = select_params_for_lambdify(params)
+        U_G = G_lambda(*params_for_lambdify, *xi_epsed).squeeze() @ xi_epsed
+
+        # total potential energy
+        U = (U_G + U_K).squeeze()
+
+        return U
+
+    def energy_fn(params: Dict[str, Array], q: Array, q_d: Array) -> Array:
+        """
+        Compute the total energy of the system.
+        Args:
+            params: Dictionary of robot parameters
+            q: generalized coordinates of shape (n_q, )
+            q_d: generalized velocities of shape (n_q, )
+        Returns:
+            E: total energy of shape ()
+        """
+        T = kinetic_energy_fn(params, q_d)
+        U = potential_energy_fn(params, q)
+        E = T + U
+
+        return E
+
+    auxiliary_fns = {
+        "apply_eps_to_bend_strains": apply_eps_to_bend_strains,
+        "kinetic_energy_fn": kinetic_energy_fn,
+        "potential_energy_fn": potential_energy_fn,
+        "energy_fn": energy_fn,
+    }
+
+    return B_xi, forward_kinematics_fn, dynamical_matrices_fn, auxiliary_fns
```

### Comparing `jsrm-0.0.7/src/jsrm/systems/utils.py` & `jsrm-0.0.8/src/jsrm/systems/utils.py`

 * *Files identical despite different names*

### Comparing `jsrm-0.0.7/src/jsrm.egg-info/PKG-INFO` & `jsrm-0.0.8/src/jsrm.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jsrm
-Version: 0.0.7
+Version: 0.0.8
 Summary: Kinematic and dynamic models of continuum and articulated soft robots.
 Author-email: Maximilian Stölzle <maximilian@stoelzle.ch>
 Maintainer-email: Maximilian Stölzle <maximilian@stoelzle.ch>
 License: Copyright (c) 2016 The Python Packaging Authority (PyPA)
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of
         this software and associated documentation files (the "Software"), to deal in
```

### Comparing `jsrm-0.0.7/src/jsrm.egg-info/SOURCES.txt` & `jsrm-0.0.8/src/jsrm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `jsrm-0.0.7/tests/test_planar_hsa.py` & `jsrm-0.0.8/tests/test_planar_hsa.py`

 * *Files identical despite different names*

### Comparing `jsrm-0.0.7/tests/test_planar_pcs.py` & `jsrm-0.0.8/tests/test_planar_pcs.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,15 +23,15 @@
         "g": jnp.array([0.0, -9.81]),
         "E": 1e7 * jnp.ones((1,)),  # Elastic modulus [Pa]
         "G": 1e6 * jnp.ones((1,)),  # Shear modulus [Pa]
     }
     # activate all strains (i.e. bending, shear, and axial)
     strain_selector = jnp.ones((3,), dtype=bool)
 
-    strain_basis, forward_kinematics_fn, dynamical_matrices_fn = planar_pcs.factory(
+    strain_basis, forward_kinematics_fn, dynamical_matrices_fn, auxiliary_fns = planar_pcs.factory(
         sym_exp_filepath, strain_selector
     )
     forward_dynamics_fn = partial(
         euler_lagrangian.forward_dynamics, dynamical_matrices_fn
     )
     nonlinear_state_space_fn = partial(
         euler_lagrangian.nonlinear_state_space, dynamical_matrices_fn
```

