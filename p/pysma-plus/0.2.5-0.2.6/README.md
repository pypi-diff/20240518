# Comparing `tmp/pysma_plus-0.2.5.tar.gz` & `tmp/pysma_plus-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pysma_plus-0.2.5.tar", last modified: Sat May 18 10:44:30 2024, max compression
+gzip compressed data, was "pysma_plus-0.2.6.tar", last modified: Sat May 18 15:00:36 2024, max compression
```

## Comparing `pysma_plus-0.2.5.tar` & `pysma_plus-0.2.6.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxrwxr-x   0 sven      (1001) sven      (1001)        0 2024-05-18 10:44:30.159001 pysma_plus-0.2.5/
--rw-rw-r--   0 sven      (1001) sven      (1001)     1400 2024-05-01 08:47:50.000000 pysma_plus-0.2.5/LICENSE
--rw-rw-r--   0 sven      (1001) sven      (1001)       80 2024-05-01 08:47:50.000000 pysma_plus-0.2.5/MANIFEST.in
--rw-r--r--   0 sven      (1001) sven      (1001)     3551 2024-05-18 10:44:30.159001 pysma_plus-0.2.5/PKG-INFO
--rw-rw-r--   0 sven      (1001) sven      (1001)     1089 2024-05-18 07:09:53.000000 pysma_plus-0.2.5/README.md
--rw-rw-r--   0 sven      (1001) sven      (1001)      924 2024-05-18 10:44:14.000000 pysma_plus-0.2.5/pyproject.toml
-drwxrwxr-x   0 sven      (1001) sven      (1001)        0 2024-05-18 10:44:30.158001 pysma_plus-0.2.5/pysma_plus.egg-info/
--rw-r--r--   0 sven      (1001) sven      (1001)     3551 2024-05-18 10:44:30.000000 pysma_plus-0.2.5/pysma_plus.egg-info/PKG-INFO
--rw-rw-r--   0 sven      (1001) sven      (1001)     1093 2024-05-18 10:44:30.000000 pysma_plus-0.2.5/pysma_plus.egg-info/SOURCES.txt
--rw-rw-r--   0 sven      (1001) sven      (1001)        1 2024-05-18 10:44:30.000000 pysma_plus-0.2.5/pysma_plus.egg-info/dependency_links.txt
--rw-rw-r--   0 sven      (1001) sven      (1001)       58 2024-05-18 10:44:30.000000 pysma_plus-0.2.5/pysma_plus.egg-info/requires.txt
--rw-rw-r--   0 sven      (1001) sven      (1001)       10 2024-05-18 10:44:30.000000 pysma_plus-0.2.5/pysma_plus.egg-info/top_level.txt
--rw-rw-r--   0 sven      (1001) sven      (1001)        1 2024-05-01 08:48:05.000000 pysma_plus-0.2.5/pysma_plus.egg-info/zip-safe
-drwxrwxr-x   0 sven      (1001) sven      (1001)        0 2024-05-18 10:44:30.156001 pysma_plus-0.2.5/pysmaplus/
--rw-rw-r--   0 sven      (1001) sven      (1001)     2798 2024-05-16 18:50:02.000000 pysma_plus-0.2.5/pysmaplus/__init__.py
--rw-rw-r--   0 sven      (1001) sven      (1001)    19249 2024-05-16 19:55:39.000000 pysma_plus-0.2.5/pysmaplus/const.py
--rw-rw-r--   0 sven      (1001) sven      (1001)     1283 2024-05-06 09:37:05.000000 pysma_plus-0.2.5/pysmaplus/const_webconnect.py
--rw-rw-r--   0 sven      (1001) sven      (1001)    10390 2024-05-10 06:46:58.000000 pysma_plus-0.2.5/pysmaplus/definitions_ennexos.py
--rw-rw-r--   0 sven      (1001) sven      (1001)    24349 2024-05-16 19:53:19.000000 pysma_plus-0.2.5/pysmaplus/definitions_speedwire.py
--rw-rw-r--   0 sven      (1001) sven      (1001)    21517 2024-05-06 09:37:05.000000 pysma_plus-0.2.5/pysmaplus/definitions_webconnect.py
--rw-rw-r--   0 sven      (1001) sven      (1001)     1345 2024-05-06 11:20:08.000000 pysma_plus-0.2.5/pysmaplus/device.py
--rw-rw-r--   0 sven      (1001) sven      (1001)     9957 2024-05-16 19:56:05.000000 pysma_plus-0.2.5/pysmaplus/device_em.py
--rw-rw-r--   0 sven      (1001) sven      (1001)    12167 2024-05-06 11:20:09.000000 pysma_plus-0.2.5/pysmaplus/device_ennexos.py
--rw-rw-r--   0 sven      (1001) sven      (1001)    26526 2024-05-18 10:38:16.000000 pysma_plus-0.2.5/pysmaplus/device_speedwire.py
--rw-rw-r--   0 sven      (1001) sven      (1001)    17330 2024-05-06 11:20:09.000000 pysma_plus-0.2.5/pysmaplus/device_webconnect.py
--rw-rw-r--   0 sven      (1001) sven      (1001)     1880 2024-05-16 18:57:36.000000 pysma_plus-0.2.5/pysmaplus/discovery.py
--rw-rw-r--   0 sven      (1001) sven      (1001)      426 2024-05-01 08:46:05.000000 pysma_plus-0.2.5/pysmaplus/exceptions.py
--rw-rw-r--   0 sven      (1001) sven      (1001)      695 2024-05-01 08:46:05.000000 pysma_plus-0.2.5/pysmaplus/helpers.py
--rw-rw-r--   0 sven      (1001) sven      (1001)     6383 2024-05-06 10:39:02.000000 pysma_plus-0.2.5/pysmaplus/sensor.py
--rw-rw-r--   0 sven      (1001) sven      (1001)      229 2024-05-18 10:44:30.159001 pysma_plus-0.2.5/setup.cfg
--rw-rw-r--   0 sven      (1001) sven      (1001)      758 2024-05-18 10:44:14.000000 pysma_plus-0.2.5/setup.py
-drwxrwxr-x   0 sven      (1001) sven      (1001)        0 2024-05-18 10:44:30.157001 pysma_plus-0.2.5/tests/
--rw-rw-r--   0 sven      (1001) sven      (1001)   315314 2024-05-01 08:46:05.000000 pysma_plus-0.2.5/tests/__init__.py
--rw-rw-r--   0 sven      (1001) sven      (1001)     2500 2024-05-03 13:38:38.000000 pysma_plus-0.2.5/tests/test_definitions.py
--rw-rw-r--   0 sven      (1001) sven      (1001)     1668 2024-05-01 08:47:50.000000 pysma_plus-0.2.5/tests/test_em.py
--rw-rw-r--   0 sven      (1001) sven      (1001)     8246 2024-05-01 08:47:50.000000 pysma_plus-0.2.5/tests/test_ennexos.py
--rw-rw-r--   0 sven      (1001) sven      (1001)      433 2024-05-01 08:46:05.000000 pysma_plus-0.2.5/tests/test_helpers.py
--rw-rw-r--   0 sven      (1001) sven      (1001)     4807 2024-05-01 08:47:50.000000 pysma_plus-0.2.5/tests/test_sensor.py
--rw-rw-r--   0 sven      (1001) sven      (1001)      884 2024-05-03 18:21:37.000000 pysma_plus-0.2.5/tests/test_speedwire.py
--rw-rw-r--   0 sven      (1001) sven      (1001)    17687 2024-05-01 08:47:50.000000 pysma_plus-0.2.5/tests/test_webconnect.py
-drwxrwxr-x   0 sven      (1001) sven      (1001)        0 2024-05-18 10:44:30.158001 pysma_plus-0.2.5/tests/testdata/
--rw-rw-r--   0 sven      (1001) sven      (1001)     6266 2024-05-01 08:47:50.000000 pysma_plus-0.2.5/tests/testdata/EVCharger-measurements.json
--rw-rw-r--   0 sven      (1001) sven      (1001)      227 2024-05-01 08:47:50.000000 pysma_plus-0.2.5/tests/testdata/EVCharger-measurements.json.source
--rw-rw-r--   0 sven      (1001) sven      (1001)      831 2024-05-01 08:47:50.000000 pysma_plus-0.2.5/tests/testdata/SunnyHomeManager2.json
--rw-rw-r--   0 sven      (1001) sven      (1001)      609 2024-05-01 08:47:50.000000 pysma_plus-0.2.5/tests/testdata/TripowerX15-deviceinfo.json
--rw-rw-r--   0 sven      (1001) sven      (1001)    23412 2024-05-01 08:47:50.000000 pysma_plus-0.2.5/tests/testdata/TripowerX15-measurements.json
--rw-rw-r--   0 sven      (1001) sven      (1001)   140175 2024-05-01 08:47:50.000000 pysma_plus-0.2.5/tests/testdata/TripowerX15-parameters.json
+drwxrwxr-x   0 sven      (1001) sven      (1001)        0 2024-05-18 15:00:36.384836 pysma_plus-0.2.6/
+-rw-rw-r--   0 sven      (1001) sven      (1001)     1400 2024-05-01 08:47:50.000000 pysma_plus-0.2.6/LICENSE
+-rw-rw-r--   0 sven      (1001) sven      (1001)       80 2024-05-01 08:47:50.000000 pysma_plus-0.2.6/MANIFEST.in
+-rw-r--r--   0 sven      (1001) sven      (1001)     3551 2024-05-18 15:00:36.384836 pysma_plus-0.2.6/PKG-INFO
+-rw-rw-r--   0 sven      (1001) sven      (1001)     1089 2024-05-18 07:09:53.000000 pysma_plus-0.2.6/README.md
+-rw-rw-r--   0 sven      (1001) sven      (1001)      924 2024-05-18 15:00:27.000000 pysma_plus-0.2.6/pyproject.toml
+drwxrwxr-x   0 sven      (1001) sven      (1001)        0 2024-05-18 15:00:36.383836 pysma_plus-0.2.6/pysma_plus.egg-info/
+-rw-r--r--   0 sven      (1001) sven      (1001)     3551 2024-05-18 15:00:36.000000 pysma_plus-0.2.6/pysma_plus.egg-info/PKG-INFO
+-rw-rw-r--   0 sven      (1001) sven      (1001)     1093 2024-05-18 15:00:36.000000 pysma_plus-0.2.6/pysma_plus.egg-info/SOURCES.txt
+-rw-rw-r--   0 sven      (1001) sven      (1001)        1 2024-05-18 15:00:36.000000 pysma_plus-0.2.6/pysma_plus.egg-info/dependency_links.txt
+-rw-rw-r--   0 sven      (1001) sven      (1001)       58 2024-05-18 15:00:36.000000 pysma_plus-0.2.6/pysma_plus.egg-info/requires.txt
+-rw-rw-r--   0 sven      (1001) sven      (1001)       10 2024-05-18 15:00:36.000000 pysma_plus-0.2.6/pysma_plus.egg-info/top_level.txt
+-rw-rw-r--   0 sven      (1001) sven      (1001)        1 2024-05-01 08:48:05.000000 pysma_plus-0.2.6/pysma_plus.egg-info/zip-safe
+drwxrwxr-x   0 sven      (1001) sven      (1001)        0 2024-05-18 15:00:36.381836 pysma_plus-0.2.6/pysmaplus/
+-rw-rw-r--   0 sven      (1001) sven      (1001)     2798 2024-05-16 18:50:02.000000 pysma_plus-0.2.6/pysmaplus/__init__.py
+-rw-rw-r--   0 sven      (1001) sven      (1001)    19249 2024-05-16 19:55:39.000000 pysma_plus-0.2.6/pysmaplus/const.py
+-rw-rw-r--   0 sven      (1001) sven      (1001)     1283 2024-05-06 09:37:05.000000 pysma_plus-0.2.6/pysmaplus/const_webconnect.py
+-rw-rw-r--   0 sven      (1001) sven      (1001)    10390 2024-05-10 06:46:58.000000 pysma_plus-0.2.6/pysmaplus/definitions_ennexos.py
+-rw-rw-r--   0 sven      (1001) sven      (1001)    32364 2024-05-18 14:47:57.000000 pysma_plus-0.2.6/pysmaplus/definitions_speedwire.py
+-rw-rw-r--   0 sven      (1001) sven      (1001)    21517 2024-05-06 09:37:05.000000 pysma_plus-0.2.6/pysmaplus/definitions_webconnect.py
+-rw-rw-r--   0 sven      (1001) sven      (1001)     1437 2024-05-18 14:17:32.000000 pysma_plus-0.2.6/pysmaplus/device.py
+-rw-rw-r--   0 sven      (1001) sven      (1001)     9957 2024-05-16 19:56:05.000000 pysma_plus-0.2.6/pysmaplus/device_em.py
+-rw-rw-r--   0 sven      (1001) sven      (1001)    12168 2024-05-18 13:46:36.000000 pysma_plus-0.2.6/pysmaplus/device_ennexos.py
+-rw-rw-r--   0 sven      (1001) sven      (1001)    19389 2024-05-18 14:59:42.000000 pysma_plus-0.2.6/pysmaplus/device_speedwire.py
+-rw-rw-r--   0 sven      (1001) sven      (1001)    17330 2024-05-06 11:20:09.000000 pysma_plus-0.2.6/pysmaplus/device_webconnect.py
+-rw-rw-r--   0 sven      (1001) sven      (1001)     1880 2024-05-16 18:57:36.000000 pysma_plus-0.2.6/pysmaplus/discovery.py
+-rw-rw-r--   0 sven      (1001) sven      (1001)      426 2024-05-01 08:46:05.000000 pysma_plus-0.2.6/pysmaplus/exceptions.py
+-rw-rw-r--   0 sven      (1001) sven      (1001)      695 2024-05-01 08:46:05.000000 pysma_plus-0.2.6/pysmaplus/helpers.py
+-rw-rw-r--   0 sven      (1001) sven      (1001)     6383 2024-05-06 10:39:02.000000 pysma_plus-0.2.6/pysmaplus/sensor.py
+-rw-rw-r--   0 sven      (1001) sven      (1001)      229 2024-05-18 15:00:36.385836 pysma_plus-0.2.6/setup.cfg
+-rw-rw-r--   0 sven      (1001) sven      (1001)      758 2024-05-18 15:00:27.000000 pysma_plus-0.2.6/setup.py
+drwxrwxr-x   0 sven      (1001) sven      (1001)        0 2024-05-18 15:00:36.382836 pysma_plus-0.2.6/tests/
+-rw-rw-r--   0 sven      (1001) sven      (1001)   315314 2024-05-01 08:46:05.000000 pysma_plus-0.2.6/tests/__init__.py
+-rw-rw-r--   0 sven      (1001) sven      (1001)     2500 2024-05-03 13:38:38.000000 pysma_plus-0.2.6/tests/test_definitions.py
+-rw-rw-r--   0 sven      (1001) sven      (1001)     1668 2024-05-01 08:47:50.000000 pysma_plus-0.2.6/tests/test_em.py
+-rw-rw-r--   0 sven      (1001) sven      (1001)     8246 2024-05-01 08:47:50.000000 pysma_plus-0.2.6/tests/test_ennexos.py
+-rw-rw-r--   0 sven      (1001) sven      (1001)      433 2024-05-01 08:46:05.000000 pysma_plus-0.2.6/tests/test_helpers.py
+-rw-rw-r--   0 sven      (1001) sven      (1001)     4807 2024-05-01 08:47:50.000000 pysma_plus-0.2.6/tests/test_sensor.py
+-rw-rw-r--   0 sven      (1001) sven      (1001)      884 2024-05-03 18:21:37.000000 pysma_plus-0.2.6/tests/test_speedwire.py
+-rw-rw-r--   0 sven      (1001) sven      (1001)    17687 2024-05-01 08:47:50.000000 pysma_plus-0.2.6/tests/test_webconnect.py
+drwxrwxr-x   0 sven      (1001) sven      (1001)        0 2024-05-18 15:00:36.383836 pysma_plus-0.2.6/tests/testdata/
+-rw-rw-r--   0 sven      (1001) sven      (1001)     6266 2024-05-01 08:47:50.000000 pysma_plus-0.2.6/tests/testdata/EVCharger-measurements.json
+-rw-rw-r--   0 sven      (1001) sven      (1001)      227 2024-05-01 08:47:50.000000 pysma_plus-0.2.6/tests/testdata/EVCharger-measurements.json.source
+-rw-rw-r--   0 sven      (1001) sven      (1001)      831 2024-05-01 08:47:50.000000 pysma_plus-0.2.6/tests/testdata/SunnyHomeManager2.json
+-rw-rw-r--   0 sven      (1001) sven      (1001)      609 2024-05-01 08:47:50.000000 pysma_plus-0.2.6/tests/testdata/TripowerX15-deviceinfo.json
+-rw-rw-r--   0 sven      (1001) sven      (1001)    23412 2024-05-01 08:47:50.000000 pysma_plus-0.2.6/tests/testdata/TripowerX15-measurements.json
+-rw-rw-r--   0 sven      (1001) sven      (1001)   140175 2024-05-01 08:47:50.000000 pysma_plus-0.2.6/tests/testdata/TripowerX15-parameters.json
```

### Comparing `pysma_plus-0.2.5/LICENSE` & `pysma_plus-0.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pysma_plus-0.2.5/PKG-INFO` & `pysma_plus-0.2.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pysma-plus
-Version: 0.2.5
+Version: 0.2.6
 Summary: Library to interface SMA Devices via WebConnect, EnnexOS and Energy Meter Devices
 Home-page: https://github.com/littleyoda/pysma
-Download-URL: https://github.com/littleyoda/pysma/tarball/0.2.5
+Download-URL: https://github.com/littleyoda/pysma/tarball/0.2.6
 Author: Sven Bursch-Osewold, Johann Kellerman and other
 Author-email: Sven Bursch-Osewold <sb_pysma@bursch.com>, Johann Kellerman <kellerza@gmail.com>
 License: The webconnect Interface was created by kellerza.
         Later Engery-Meter and EnnexOS Support was added by little.yoda.
         Parts of the SMA-Query-Library (https://github.com/Wired-Square/sma-query/) by Garth Berry
         was added to this Library and modified by little.yoda
```

### Comparing `pysma_plus-0.2.5/README.md` & `pysma_plus-0.2.6/README.md`

 * *Files identical despite different names*

### Comparing `pysma_plus-0.2.5/pyproject.toml` & `pysma_plus-0.2.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pysma-plus"
-version = "0.2.5"
+version = "0.2.6"
 description = "Library to interface SMA Devices via WebConnect, EnnexOS and Energy Meter Devices"
 readme = "README.md"
 authors = [{ name = "Sven Bursch-Osewold", email = "sb_pysma@bursch.com" },{ name = "Johann Kellerman" , email ="kellerza@gmail.com"} ]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
```

### Comparing `pysma_plus-0.2.5/pysma_plus.egg-info/PKG-INFO` & `pysma_plus-0.2.6/pysma_plus.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pysma-plus
-Version: 0.2.5
+Version: 0.2.6
 Summary: Library to interface SMA Devices via WebConnect, EnnexOS and Energy Meter Devices
 Home-page: https://github.com/littleyoda/pysma
-Download-URL: https://github.com/littleyoda/pysma/tarball/0.2.5
+Download-URL: https://github.com/littleyoda/pysma/tarball/0.2.6
 Author: Sven Bursch-Osewold, Johann Kellerman and other
 Author-email: Sven Bursch-Osewold <sb_pysma@bursch.com>, Johann Kellerman <kellerza@gmail.com>
 License: The webconnect Interface was created by kellerza.
         Later Engery-Meter and EnnexOS Support was added by little.yoda.
         Parts of the SMA-Query-Library (https://github.com/Wired-Square/sma-query/) by Garth Berry
         was added to this Library and modified by little.yoda
```

### Comparing `pysma_plus-0.2.5/pysma_plus.egg-info/SOURCES.txt` & `pysma_plus-0.2.6/pysma_plus.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pysma_plus-0.2.5/pysmaplus/__init__.py` & `pysma_plus-0.2.6/pysmaplus/__init__.py`

 * *Files identical despite different names*

### Comparing `pysma_plus-0.2.5/pysmaplus/const.py` & `pysma_plus-0.2.6/pysmaplus/const.py`

 * *Files identical despite different names*

### Comparing `pysma_plus-0.2.5/pysmaplus/const_webconnect.py` & `pysma_plus-0.2.6/pysmaplus/const_webconnect.py`

 * *Files identical despite different names*

### Comparing `pysma_plus-0.2.5/pysmaplus/definitions_ennexos.py` & `pysma_plus-0.2.6/pysmaplus/definitions_ennexos.py`

 * *Files identical despite different names*

### Comparing `pysma_plus-0.2.5/pysmaplus/definitions_webconnect.py` & `pysma_plus-0.2.6/pysmaplus/definitions_webconnect.py`

 * *Files identical despite different names*

### Comparing `pysma_plus-0.2.5/pysmaplus/device.py` & `pysma_plus-0.2.6/pysmaplus/device.py`

 * *Files 4% similar despite different names*

```diff
@@ -43,7 +43,11 @@
                 "ip": ip,
             }
         ]
 
     @abstractmethod
     async def get_debug(self) -> Dict[str, Any]:
         """Return a dict with all debug information."""
+
+    def set_options(self, options: Dict[str, Any]):
+        """Set options"""
+        pass
```

### Comparing `pysma_plus-0.2.5/pysmaplus/device_em.py` & `pysma_plus-0.2.6/pysmaplus/device_em.py`

 * *Files identical despite different names*

### Comparing `pysma_plus-0.2.5/pysmaplus/device_ennexos.py` & `pysma_plus-0.2.6/pysmaplus/device_ennexos.py`

 * *Files 0% similar despite different names*

```diff
@@ -362,7 +362,8 @@
                     break
                 ret["status"] = "failed"
                 ret["exception"] = dev
             except Exception as e:
                 ret["status"] = "failed"
                 ret["exception"] = e
         return rets
+
```

### Comparing `pysma_plus-0.2.5/pysmaplus/device_webconnect.py` & `pysma_plus-0.2.6/pysmaplus/device_webconnect.py`

 * *Files identical despite different names*

### Comparing `pysma_plus-0.2.5/pysmaplus/discovery.py` & `pysma_plus-0.2.6/pysmaplus/discovery.py`

 * *Files identical despite different names*

### Comparing `pysma_plus-0.2.5/pysmaplus/helpers.py` & `pysma_plus-0.2.6/pysmaplus/helpers.py`

 * *Files identical despite different names*

### Comparing `pysma_plus-0.2.5/pysmaplus/sensor.py` & `pysma_plus-0.2.6/pysmaplus/sensor.py`

 * *Files identical despite different names*

### Comparing `pysma_plus-0.2.5/setup.py` & `pysma_plus-0.2.6/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #!/usr/bin/env python
 """pysma library setup."""
 from pathlib import Path
 
 from setuptools import setup
 
-VERSION = "0.2.5"
+VERSION = "0.2.6"
 URL = "https://github.com/littleyoda/pysma"
 
 setup(
     name="pysma-plus",
     version=VERSION,
     description="Library to interface SMA Devices via WebConnect, EnnexOS and Energy Meter Devices",
     long_description=Path("README.md").read_text(),
```

### Comparing `pysma_plus-0.2.5/tests/__init__.py` & `pysma_plus-0.2.6/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `pysma_plus-0.2.5/tests/test_definitions.py` & `pysma_plus-0.2.6/tests/test_definitions.py`

 * *Files identical despite different names*

### Comparing `pysma_plus-0.2.5/tests/test_em.py` & `pysma_plus-0.2.6/tests/test_em.py`

 * *Files identical despite different names*

### Comparing `pysma_plus-0.2.5/tests/test_ennexos.py` & `pysma_plus-0.2.6/tests/test_ennexos.py`

 * *Files identical despite different names*

### Comparing `pysma_plus-0.2.5/tests/test_sensor.py` & `pysma_plus-0.2.6/tests/test_sensor.py`

 * *Files identical despite different names*

### Comparing `pysma_plus-0.2.5/tests/test_speedwire.py` & `pysma_plus-0.2.6/tests/test_speedwire.py`

 * *Files identical despite different names*

### Comparing `pysma_plus-0.2.5/tests/test_webconnect.py` & `pysma_plus-0.2.6/tests/test_webconnect.py`

 * *Files identical despite different names*

### Comparing `pysma_plus-0.2.5/tests/testdata/EVCharger-measurements.json` & `pysma_plus-0.2.6/tests/testdata/EVCharger-measurements.json`

 * *Files identical despite different names*

### Comparing `pysma_plus-0.2.5/tests/testdata/SunnyHomeManager2.json` & `pysma_plus-0.2.6/tests/testdata/SunnyHomeManager2.json`

 * *Files identical despite different names*

### Comparing `pysma_plus-0.2.5/tests/testdata/TripowerX15-deviceinfo.json` & `pysma_plus-0.2.6/tests/testdata/TripowerX15-deviceinfo.json`

 * *Files identical despite different names*

### Comparing `pysma_plus-0.2.5/tests/testdata/TripowerX15-measurements.json` & `pysma_plus-0.2.6/tests/testdata/TripowerX15-measurements.json`

 * *Files identical despite different names*

### Comparing `pysma_plus-0.2.5/tests/testdata/TripowerX15-parameters.json` & `pysma_plus-0.2.6/tests/testdata/TripowerX15-parameters.json`

 * *Files identical despite different names*

