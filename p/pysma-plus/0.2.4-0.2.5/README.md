# Comparing `tmp/pysma_plus-0.2.4.tar.gz` & `tmp/pysma_plus-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pysma_plus-0.2.4.tar", last modified: Fri May  3 14:13:35 2024, max compression
+gzip compressed data, was "pysma_plus-0.2.5.tar", last modified: Sat May 18 10:44:30 2024, max compression
```

## Comparing `pysma_plus-0.2.4.tar` & `pysma_plus-0.2.5.tar`

### file list

```diff
@@ -1,45 +1,47 @@
-drwxrwxr-x   0 sven      (1001) sven      (1001)        0 2024-05-03 14:13:35.422245 pysma_plus-0.2.4/
--rw-rw-r--   0 sven      (1001) sven      (1001)     1400 2024-05-01 08:47:50.000000 pysma_plus-0.2.4/LICENSE
--rw-rw-r--   0 sven      (1001) sven      (1001)       80 2024-05-01 08:47:50.000000 pysma_plus-0.2.4/MANIFEST.in
--rw-r--r--   0 sven      (1001) sven      (1001)     3509 2024-05-03 14:13:35.422245 pysma_plus-0.2.4/PKG-INFO
--rw-rw-r--   0 sven      (1001) sven      (1001)     1085 2024-05-01 08:47:50.000000 pysma_plus-0.2.4/README.md
--rw-rw-r--   0 sven      (1001) sven      (1001)      895 2024-05-03 14:13:28.000000 pysma_plus-0.2.4/pyproject.toml
-drwxrwxr-x   0 sven      (1001) sven      (1001)        0 2024-05-03 14:13:35.422245 pysma_plus-0.2.4/pysma_plus.egg-info/
--rw-r--r--   0 sven      (1001) sven      (1001)     3509 2024-05-03 14:13:35.000000 pysma_plus-0.2.4/pysma_plus.egg-info/PKG-INFO
--rw-rw-r--   0 sven      (1001) sven      (1001)     1046 2024-05-03 14:13:35.000000 pysma_plus-0.2.4/pysma_plus.egg-info/SOURCES.txt
--rw-rw-r--   0 sven      (1001) sven      (1001)        1 2024-05-03 14:13:35.000000 pysma_plus-0.2.4/pysma_plus.egg-info/dependency_links.txt
--rw-rw-r--   0 sven      (1001) sven      (1001)       35 2024-05-03 14:13:35.000000 pysma_plus-0.2.4/pysma_plus.egg-info/requires.txt
--rw-rw-r--   0 sven      (1001) sven      (1001)       10 2024-05-03 14:13:35.000000 pysma_plus-0.2.4/pysma_plus.egg-info/top_level.txt
--rw-rw-r--   0 sven      (1001) sven      (1001)        1 2024-05-01 08:48:05.000000 pysma_plus-0.2.4/pysma_plus.egg-info/zip-safe
-drwxrwxr-x   0 sven      (1001) sven      (1001)        0 2024-05-03 14:13:35.420245 pysma_plus-0.2.4/pysmaplus/
--rw-rw-r--   0 sven      (1001) sven      (1001)     2409 2024-05-03 13:42:28.000000 pysma_plus-0.2.4/pysmaplus/__init__.py
--rw-rw-r--   0 sven      (1001) sven      (1001)    18929 2024-05-03 13:42:53.000000 pysma_plus-0.2.4/pysmaplus/const.py
--rw-rw-r--   0 sven      (1001) sven      (1001)     1283 2024-05-01 08:47:50.000000 pysma_plus-0.2.4/pysmaplus/const_webconnect.py
--rw-rw-r--   0 sven      (1001) sven      (1001)     9346 2024-05-03 13:35:20.000000 pysma_plus-0.2.4/pysmaplus/definitions_ennexos.py
--rw-rw-r--   0 sven      (1001) sven      (1001)    21600 2024-05-03 13:41:20.000000 pysma_plus-0.2.4/pysmaplus/definitions_speedwire.py
--rw-rw-r--   0 sven      (1001) sven      (1001)    21242 2024-05-03 11:25:27.000000 pysma_plus-0.2.4/pysmaplus/definitions_webconnect.py
--rw-rw-r--   0 sven      (1001) sven      (1001)      825 2024-05-02 14:56:18.000000 pysma_plus-0.2.4/pysmaplus/device.py
--rw-rw-r--   0 sven      (1001) sven      (1001)     9602 2024-05-01 08:47:50.000000 pysma_plus-0.2.4/pysmaplus/device_em.py
--rw-rw-r--   0 sven      (1001) sven      (1001)    12557 2024-05-03 13:41:56.000000 pysma_plus-0.2.4/pysmaplus/device_ennexos.py
--rw-rw-r--   0 sven      (1001) sven      (1001)    21090 2024-05-03 13:41:03.000000 pysma_plus-0.2.4/pysmaplus/device_speedwire.py
--rw-rw-r--   0 sven      (1001) sven      (1001)    17213 2024-05-02 14:59:07.000000 pysma_plus-0.2.4/pysmaplus/device_webconnect.py
--rw-rw-r--   0 sven      (1001) sven      (1001)      426 2024-05-01 08:46:05.000000 pysma_plus-0.2.4/pysmaplus/exceptions.py
--rw-rw-r--   0 sven      (1001) sven      (1001)      695 2024-05-01 08:46:05.000000 pysma_plus-0.2.4/pysmaplus/helpers.py
--rw-rw-r--   0 sven      (1001) sven      (1001)     6357 2024-05-01 08:47:50.000000 pysma_plus-0.2.4/pysmaplus/sensor.py
--rw-rw-r--   0 sven      (1001) sven      (1001)      229 2024-05-03 14:13:35.422245 pysma_plus-0.2.4/setup.cfg
--rw-rw-r--   0 sven      (1001) sven      (1001)      758 2024-05-03 14:13:28.000000 pysma_plus-0.2.4/setup.py
-drwxrwxr-x   0 sven      (1001) sven      (1001)        0 2024-05-03 14:13:35.421245 pysma_plus-0.2.4/tests/
--rw-rw-r--   0 sven      (1001) sven      (1001)   315314 2024-05-01 08:46:05.000000 pysma_plus-0.2.4/tests/__init__.py
--rw-rw-r--   0 sven      (1001) sven      (1001)     2500 2024-05-03 13:38:38.000000 pysma_plus-0.2.4/tests/test_definitions.py
--rw-rw-r--   0 sven      (1001) sven      (1001)     1668 2024-05-01 08:47:50.000000 pysma_plus-0.2.4/tests/test_em.py
--rw-rw-r--   0 sven      (1001) sven      (1001)     8246 2024-05-01 08:47:50.000000 pysma_plus-0.2.4/tests/test_ennexos.py
--rw-rw-r--   0 sven      (1001) sven      (1001)      433 2024-05-01 08:46:05.000000 pysma_plus-0.2.4/tests/test_helpers.py
--rw-rw-r--   0 sven      (1001) sven      (1001)     4807 2024-05-01 08:47:50.000000 pysma_plus-0.2.4/tests/test_sensor.py
--rw-rw-r--   0 sven      (1001) sven      (1001)    17687 2024-05-01 08:47:50.000000 pysma_plus-0.2.4/tests/test_webconnect.py
-drwxrwxr-x   0 sven      (1001) sven      (1001)        0 2024-05-03 14:13:35.422245 pysma_plus-0.2.4/tests/testdata/
--rw-rw-r--   0 sven      (1001) sven      (1001)     6266 2024-05-01 08:47:50.000000 pysma_plus-0.2.4/tests/testdata/EVCharger-measurements.json
--rw-rw-r--   0 sven      (1001) sven      (1001)      227 2024-05-01 08:47:50.000000 pysma_plus-0.2.4/tests/testdata/EVCharger-measurements.json.source
--rw-rw-r--   0 sven      (1001) sven      (1001)      831 2024-05-01 08:47:50.000000 pysma_plus-0.2.4/tests/testdata/SunnyHomeManager2.json
--rw-rw-r--   0 sven      (1001) sven      (1001)      609 2024-05-01 08:47:50.000000 pysma_plus-0.2.4/tests/testdata/TripowerX15-deviceinfo.json
--rw-rw-r--   0 sven      (1001) sven      (1001)    23412 2024-05-01 08:47:50.000000 pysma_plus-0.2.4/tests/testdata/TripowerX15-measurements.json
--rw-rw-r--   0 sven      (1001) sven      (1001)   140175 2024-05-01 08:47:50.000000 pysma_plus-0.2.4/tests/testdata/TripowerX15-parameters.json
+drwxrwxr-x   0 sven      (1001) sven      (1001)        0 2024-05-18 10:44:30.159001 pysma_plus-0.2.5/
+-rw-rw-r--   0 sven      (1001) sven      (1001)     1400 2024-05-01 08:47:50.000000 pysma_plus-0.2.5/LICENSE
+-rw-rw-r--   0 sven      (1001) sven      (1001)       80 2024-05-01 08:47:50.000000 pysma_plus-0.2.5/MANIFEST.in
+-rw-r--r--   0 sven      (1001) sven      (1001)     3551 2024-05-18 10:44:30.159001 pysma_plus-0.2.5/PKG-INFO
+-rw-rw-r--   0 sven      (1001) sven      (1001)     1089 2024-05-18 07:09:53.000000 pysma_plus-0.2.5/README.md
+-rw-rw-r--   0 sven      (1001) sven      (1001)      924 2024-05-18 10:44:14.000000 pysma_plus-0.2.5/pyproject.toml
+drwxrwxr-x   0 sven      (1001) sven      (1001)        0 2024-05-18 10:44:30.158001 pysma_plus-0.2.5/pysma_plus.egg-info/
+-rw-r--r--   0 sven      (1001) sven      (1001)     3551 2024-05-18 10:44:30.000000 pysma_plus-0.2.5/pysma_plus.egg-info/PKG-INFO
+-rw-rw-r--   0 sven      (1001) sven      (1001)     1093 2024-05-18 10:44:30.000000 pysma_plus-0.2.5/pysma_plus.egg-info/SOURCES.txt
+-rw-rw-r--   0 sven      (1001) sven      (1001)        1 2024-05-18 10:44:30.000000 pysma_plus-0.2.5/pysma_plus.egg-info/dependency_links.txt
+-rw-rw-r--   0 sven      (1001) sven      (1001)       58 2024-05-18 10:44:30.000000 pysma_plus-0.2.5/pysma_plus.egg-info/requires.txt
+-rw-rw-r--   0 sven      (1001) sven      (1001)       10 2024-05-18 10:44:30.000000 pysma_plus-0.2.5/pysma_plus.egg-info/top_level.txt
+-rw-rw-r--   0 sven      (1001) sven      (1001)        1 2024-05-01 08:48:05.000000 pysma_plus-0.2.5/pysma_plus.egg-info/zip-safe
+drwxrwxr-x   0 sven      (1001) sven      (1001)        0 2024-05-18 10:44:30.156001 pysma_plus-0.2.5/pysmaplus/
+-rw-rw-r--   0 sven      (1001) sven      (1001)     2798 2024-05-16 18:50:02.000000 pysma_plus-0.2.5/pysmaplus/__init__.py
+-rw-rw-r--   0 sven      (1001) sven      (1001)    19249 2024-05-16 19:55:39.000000 pysma_plus-0.2.5/pysmaplus/const.py
+-rw-rw-r--   0 sven      (1001) sven      (1001)     1283 2024-05-06 09:37:05.000000 pysma_plus-0.2.5/pysmaplus/const_webconnect.py
+-rw-rw-r--   0 sven      (1001) sven      (1001)    10390 2024-05-10 06:46:58.000000 pysma_plus-0.2.5/pysmaplus/definitions_ennexos.py
+-rw-rw-r--   0 sven      (1001) sven      (1001)    24349 2024-05-16 19:53:19.000000 pysma_plus-0.2.5/pysmaplus/definitions_speedwire.py
+-rw-rw-r--   0 sven      (1001) sven      (1001)    21517 2024-05-06 09:37:05.000000 pysma_plus-0.2.5/pysmaplus/definitions_webconnect.py
+-rw-rw-r--   0 sven      (1001) sven      (1001)     1345 2024-05-06 11:20:08.000000 pysma_plus-0.2.5/pysmaplus/device.py
+-rw-rw-r--   0 sven      (1001) sven      (1001)     9957 2024-05-16 19:56:05.000000 pysma_plus-0.2.5/pysmaplus/device_em.py
+-rw-rw-r--   0 sven      (1001) sven      (1001)    12167 2024-05-06 11:20:09.000000 pysma_plus-0.2.5/pysmaplus/device_ennexos.py
+-rw-rw-r--   0 sven      (1001) sven      (1001)    26526 2024-05-18 10:38:16.000000 pysma_plus-0.2.5/pysmaplus/device_speedwire.py
+-rw-rw-r--   0 sven      (1001) sven      (1001)    17330 2024-05-06 11:20:09.000000 pysma_plus-0.2.5/pysmaplus/device_webconnect.py
+-rw-rw-r--   0 sven      (1001) sven      (1001)     1880 2024-05-16 18:57:36.000000 pysma_plus-0.2.5/pysmaplus/discovery.py
+-rw-rw-r--   0 sven      (1001) sven      (1001)      426 2024-05-01 08:46:05.000000 pysma_plus-0.2.5/pysmaplus/exceptions.py
+-rw-rw-r--   0 sven      (1001) sven      (1001)      695 2024-05-01 08:46:05.000000 pysma_plus-0.2.5/pysmaplus/helpers.py
+-rw-rw-r--   0 sven      (1001) sven      (1001)     6383 2024-05-06 10:39:02.000000 pysma_plus-0.2.5/pysmaplus/sensor.py
+-rw-rw-r--   0 sven      (1001) sven      (1001)      229 2024-05-18 10:44:30.159001 pysma_plus-0.2.5/setup.cfg
+-rw-rw-r--   0 sven      (1001) sven      (1001)      758 2024-05-18 10:44:14.000000 pysma_plus-0.2.5/setup.py
+drwxrwxr-x   0 sven      (1001) sven      (1001)        0 2024-05-18 10:44:30.157001 pysma_plus-0.2.5/tests/
+-rw-rw-r--   0 sven      (1001) sven      (1001)   315314 2024-05-01 08:46:05.000000 pysma_plus-0.2.5/tests/__init__.py
+-rw-rw-r--   0 sven      (1001) sven      (1001)     2500 2024-05-03 13:38:38.000000 pysma_plus-0.2.5/tests/test_definitions.py
+-rw-rw-r--   0 sven      (1001) sven      (1001)     1668 2024-05-01 08:47:50.000000 pysma_plus-0.2.5/tests/test_em.py
+-rw-rw-r--   0 sven      (1001) sven      (1001)     8246 2024-05-01 08:47:50.000000 pysma_plus-0.2.5/tests/test_ennexos.py
+-rw-rw-r--   0 sven      (1001) sven      (1001)      433 2024-05-01 08:46:05.000000 pysma_plus-0.2.5/tests/test_helpers.py
+-rw-rw-r--   0 sven      (1001) sven      (1001)     4807 2024-05-01 08:47:50.000000 pysma_plus-0.2.5/tests/test_sensor.py
+-rw-rw-r--   0 sven      (1001) sven      (1001)      884 2024-05-03 18:21:37.000000 pysma_plus-0.2.5/tests/test_speedwire.py
+-rw-rw-r--   0 sven      (1001) sven      (1001)    17687 2024-05-01 08:47:50.000000 pysma_plus-0.2.5/tests/test_webconnect.py
+drwxrwxr-x   0 sven      (1001) sven      (1001)        0 2024-05-18 10:44:30.158001 pysma_plus-0.2.5/tests/testdata/
+-rw-rw-r--   0 sven      (1001) sven      (1001)     6266 2024-05-01 08:47:50.000000 pysma_plus-0.2.5/tests/testdata/EVCharger-measurements.json
+-rw-rw-r--   0 sven      (1001) sven      (1001)      227 2024-05-01 08:47:50.000000 pysma_plus-0.2.5/tests/testdata/EVCharger-measurements.json.source
+-rw-rw-r--   0 sven      (1001) sven      (1001)      831 2024-05-01 08:47:50.000000 pysma_plus-0.2.5/tests/testdata/SunnyHomeManager2.json
+-rw-rw-r--   0 sven      (1001) sven      (1001)      609 2024-05-01 08:47:50.000000 pysma_plus-0.2.5/tests/testdata/TripowerX15-deviceinfo.json
+-rw-rw-r--   0 sven      (1001) sven      (1001)    23412 2024-05-01 08:47:50.000000 pysma_plus-0.2.5/tests/testdata/TripowerX15-measurements.json
+-rw-rw-r--   0 sven      (1001) sven      (1001)   140175 2024-05-01 08:47:50.000000 pysma_plus-0.2.5/tests/testdata/TripowerX15-parameters.json
```

### Comparing `pysma_plus-0.2.4/LICENSE` & `pysma_plus-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pysma_plus-0.2.4/PKG-INFO` & `pysma_plus-0.2.5/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pysma-plus
-Version: 0.2.4
+Version: 0.2.5
 Summary: Library to interface SMA Devices via WebConnect, EnnexOS and Energy Meter Devices
 Home-page: https://github.com/littleyoda/pysma
-Download-URL: https://github.com/littleyoda/pysma/tarball/0.2.4
+Download-URL: https://github.com/littleyoda/pysma/tarball/0.2.5
 Author: Sven Bursch-Osewold, Johann Kellerman and other
 Author-email: Sven Bursch-Osewold <sb_pysma@bursch.com>, Johann Kellerman <kellerza@gmail.com>
 License: The webconnect Interface was created by kellerza.
         Later Engery-Meter and EnnexOS Support was added by little.yoda.
         Parts of the SMA-Query-Library (https://github.com/Wired-Square/sma-query/) by Garth Berry
         was added to this Library and modified by little.yoda
         
@@ -43,14 +43,15 @@
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: aiohttp<4,>3.3
 Requires-Dist: attrs>18
 Requires-Dist: jmespath<2
+Requires-Dist: dataclasses-struct>0.8
 
 
 # pysma-plus library
 
 Python 3 library to retrieve data from various SMA](https://www.sma.de/) devices.
 Based on a fork of the [pysma lib from kellerza](https://github.com/kellerza/pysma).
 The long-term goal is to integrate the change into the original library.
@@ -72,12 +73,12 @@
 
 | Bereich | Gerät | Methode |
 |--|--|--|
 | Wechselrichter | Tripower X (STP XX-50)<br>(15,25) | ennexos |
 | Hybrid-Wechselrichter | Sunny Tripower Smart Energy<br>(10.0)  | webconnect |
 | Hybrid-Wechselrichter | Sunny Boy Storage<br>(SBS3.7-10, SBS5.0-10) | webconnect |
 | | | |
-| Energy Meter | Energy Meter 2<br>(EMTER 20) | speedwire |
-| Energy Meter | Sunny Home Manager 2<br>(SHM2) | speedwire |
+| Energy Meter | Energy Meter 2<br>(EMTER 20) | speedwireEM |
+| Energy Meter | Sunny Home Manager 2<br>(SHM2) | speedwireEM |
 | | | |
```

### Comparing `pysma_plus-0.2.4/README.md` & `pysma_plus-0.2.5/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -22,12 +22,12 @@
 
 | Bereich | Gerät | Methode |
 |--|--|--|
 | Wechselrichter | Tripower X (STP XX-50)<br>(15,25) | ennexos |
 | Hybrid-Wechselrichter | Sunny Tripower Smart Energy<br>(10.0)  | webconnect |
 | Hybrid-Wechselrichter | Sunny Boy Storage<br>(SBS3.7-10, SBS5.0-10) | webconnect |
 | | | |
-| Energy Meter | Energy Meter 2<br>(EMTER 20) | speedwire |
-| Energy Meter | Sunny Home Manager 2<br>(SHM2) | speedwire |
+| Energy Meter | Energy Meter 2<br>(EMTER 20) | speedwireEM |
+| Energy Meter | Sunny Home Manager 2<br>(SHM2) | speedwireEM |
 | | | |
```

### Comparing `pysma_plus-0.2.4/pyproject.toml` & `pysma_plus-0.2.5/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -2,28 +2,29 @@
 
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pysma-plus"
-version = "0.2.4"
+version = "0.2.5"
 description = "Library to interface SMA Devices via WebConnect, EnnexOS and Energy Meter Devices"
 readme = "README.md"
 authors = [{ name = "Sven Bursch-Osewold", email = "sb_pysma@bursch.com" },{ name = "Johann Kellerman" , email ="kellerza@gmail.com"} ]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
 ]
 dependencies = [
     "aiohttp>3.3,<4",
     "attrs>18",
     "jmespath<2",
+    "dataclasses-struct>0.8"
 ]
 requires-python = ">=3.9"
 
 [tool.setuptools]
 include-package-data = false
 
 [tool.setuptools.packages.find]
```

### Comparing `pysma_plus-0.2.4/pysma_plus.egg-info/PKG-INFO` & `pysma_plus-0.2.5/pysma_plus.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pysma-plus
-Version: 0.2.4
+Version: 0.2.5
 Summary: Library to interface SMA Devices via WebConnect, EnnexOS and Energy Meter Devices
 Home-page: https://github.com/littleyoda/pysma
-Download-URL: https://github.com/littleyoda/pysma/tarball/0.2.4
+Download-URL: https://github.com/littleyoda/pysma/tarball/0.2.5
 Author: Sven Bursch-Osewold, Johann Kellerman and other
 Author-email: Sven Bursch-Osewold <sb_pysma@bursch.com>, Johann Kellerman <kellerza@gmail.com>
 License: The webconnect Interface was created by kellerza.
         Later Engery-Meter and EnnexOS Support was added by little.yoda.
         Parts of the SMA-Query-Library (https://github.com/Wired-Square/sma-query/) by Garth Berry
         was added to this Library and modified by little.yoda
         
@@ -43,14 +43,15 @@
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: aiohttp<4,>3.3
 Requires-Dist: attrs>18
 Requires-Dist: jmespath<2
+Requires-Dist: dataclasses-struct>0.8
 
 
 # pysma-plus library
 
 Python 3 library to retrieve data from various SMA](https://www.sma.de/) devices.
 Based on a fork of the [pysma lib from kellerza](https://github.com/kellerza/pysma).
 The long-term goal is to integrate the change into the original library.
@@ -72,12 +73,12 @@
 
 | Bereich | Gerät | Methode |
 |--|--|--|
 | Wechselrichter | Tripower X (STP XX-50)<br>(15,25) | ennexos |
 | Hybrid-Wechselrichter | Sunny Tripower Smart Energy<br>(10.0)  | webconnect |
 | Hybrid-Wechselrichter | Sunny Boy Storage<br>(SBS3.7-10, SBS5.0-10) | webconnect |
 | | | |
-| Energy Meter | Energy Meter 2<br>(EMTER 20) | speedwire |
-| Energy Meter | Sunny Home Manager 2<br>(SHM2) | speedwire |
+| Energy Meter | Energy Meter 2<br>(EMTER 20) | speedwireEM |
+| Energy Meter | Sunny Home Manager 2<br>(SHM2) | speedwireEM |
 | | | |
```

### Comparing `pysma_plus-0.2.4/pysma_plus.egg-info/SOURCES.txt` & `pysma_plus-0.2.5/pysma_plus.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -17,23 +17,25 @@
 pysmaplus/definitions_speedwire.py
 pysmaplus/definitions_webconnect.py
 pysmaplus/device.py
 pysmaplus/device_em.py
 pysmaplus/device_ennexos.py
 pysmaplus/device_speedwire.py
 pysmaplus/device_webconnect.py
+pysmaplus/discovery.py
 pysmaplus/exceptions.py
 pysmaplus/helpers.py
 pysmaplus/sensor.py
 tests/__init__.py
 tests/test_definitions.py
 tests/test_em.py
 tests/test_ennexos.py
 tests/test_helpers.py
 tests/test_sensor.py
+tests/test_speedwire.py
 tests/test_webconnect.py
 tests/testdata/EVCharger-measurements.json
 tests/testdata/EVCharger-measurements.json.source
 tests/testdata/SunnyHomeManager2.json
 tests/testdata/TripowerX15-deviceinfo.json
 tests/testdata/TripowerX15-measurements.json
 tests/testdata/TripowerX15-parameters.json
```

### Comparing `pysma_plus-0.2.4/pysmaplus/__init__.py` & `pysma_plus-0.2.5/pysmaplus/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,68 +1,91 @@
 """SMA WebConnect library for Python.
 
 See: http://www.sma.de/en/products/monitoring-control/webconnect.html
 
 Source: http://www.github.com/kellerza/pysma
 """
+
 import logging
 from typing import Optional
 import asyncio
 from aiohttp import ClientSession
 from .device_webconnect import SMAwebconnect
 from .device_ennexos import SMAennexos
 from .device_speedwire import SMAspeedwireINV
 from .device_em import SMAspeedwireEM
 from .device import Device
+from .discovery import Discovery
+
 _LOGGER = logging.getLogger(__name__)
 
 
-# Backward compatibility
 def SMA(session, url, password, group):
+    """Backward compatibility"""
+    # pylint: disable=invalid-name
     return SMAwebconnect(session, url, password=password, group=group)
 
 
-def getDevice(session: ClientSession,
-        url: str,
-        password: Optional[str] = None,
-        groupuser: str = "user",
-        accessmethod: str = "webconnect"
-    ) -> Device:
-        _LOGGER.debug(f"Device Called! Url: {url} User/Group: {groupuser} Accessmethod: {accessmethod}")
-        if (accessmethod == "webconnect"):
-            return SMAwebconnect(session, url, password=password, group=groupuser)
-        elif (accessmethod == "ennexos"):
-            return SMAennexos(session, url, password=password, group=groupuser)
-        elif (accessmethod == "speedwire") or (accessmethod == "speedwireem"):
-              return SMAspeedwireEM()
-        elif (accessmethod == "speedwireinv"):
-              return SMAspeedwireINV(host = url, password= password, group=groupuser)
-        else:
-             return None
-
-async def _runDetect(accessmethod: str, session: ClientSession, ip):
-        sma = None
-        if (accessmethod == "webconnect"):
-            sma = SMAwebconnect(session, ip, password="", group="user")
-        elif (accessmethod == "ennexos"):
-            sma = SMAennexos(session, ip, password=None, group=None)
-        elif (accessmethod == "speedwireinv"):
-            sma = SMAspeedwireINV(host=ip, password="", group="user")
-        ret = await sma.detect(ip)
-        for i in ret:
-            i["access"] = accessmethod
-        try:
-             await sma.close_session()
-        except Exception:
-             pass
-        return ret
-
-async def autoDetect(session: ClientSession, ip:str):
+def getDevice(
+    session: ClientSession,
+    url: str,
+    password: Optional[str] = None,
+    groupuser: str = "user",
+    accessmethod: str = "webconnect",
+) -> Device | None:
+    # pylint: disable=invalid-name
+    """Returns a Device object for accessing the device"""
+    _LOGGER.debug(
+        "Device Called! Url: %s User/Group: %s Accessmethod: %s",
+        url,
+        groupuser,
+        accessmethod,
+    )
+    if accessmethod == "webconnect":
+        return SMAwebconnect(session, url, password=password, group=groupuser)
+    if accessmethod == "ennexos":
+        return SMAennexos(session, url, password=password, group=groupuser)
+    if accessmethod in ["speedwire", "speedwireem"]:
+        return SMAspeedwireEM()
+    if accessmethod == "speedwireinv":
+        return SMAspeedwireINV(host=url, password=password, group=groupuser)
+    return None
+
+
+async def _run_detect(accessmethod: str, session: ClientSession, ip):
+    """Start Autodetection"""
+    sma: Device
+    if accessmethod == "webconnect":
+        sma = SMAwebconnect(session, ip, password="", group="user")
+    elif accessmethod == "ennexos":
+        sma = SMAennexos(session, ip, password=None, group=None)
+    elif accessmethod == "speedwireinv":
+        sma = SMAspeedwireINV(host=ip, password="", group="user")
+    else:
+        return None
+    ret = await sma.detect(ip)
+    for i in ret:
+        i["access"] = accessmethod
+    try:
+        await sma.close_session()
+    except Exception:  # pylint: disable=broad-exception-caught
+        pass
+    return ret
+
+
+async def autoDetect(session: ClientSession, ip: str):
+    # pylint: disable=invalid-name
+    """Runs a autodetection of all supported devices (no energy meters) on the ip-address"""
     ret = await asyncio.gather(
-        _runDetect("ennexos", session, ip),
-        _runDetect("speedwireinv", session, ip),
-        _runDetect("webconnect", session, ip)
+        _run_detect("ennexos", session, ip),
+        _run_detect("speedwireinv", session, ip),
+        _run_detect("webconnect", session, ip),
     )
     results = []
     for r in ret:
-         results.extend(r)
+        results.extend(r)
     return results
+
+
+async def discovery():
+    discover = Discovery(asyncio.get_event_loop())
+    return await discover.run()
```

### Comparing `pysma_plus-0.2.4/pysmaplus/const.py` & `pysma_plus-0.2.5/pysmaplus/const.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,136 +1,145 @@
+"""
+All Consts
+
+"""
+
 from typing import Dict
 
-class Identifier():
-    pv_power_a : str = "pv_power_a"
-    pv_power_b : str = "pv_power_b"
-    pv_power_c : str = "pv_power_c"
-    pv_voltage_a : str = "pv_voltage_a"
-    pv_voltage_b : str = "pv_voltage_b"
-    pv_voltage_c : str = "pv_voltage_c"
-    pv_current_a : str = "pv_current_a"
-    pv_current_b : str = "pv_current_b"
-    pv_current_c : str = "pv_current_c"
-    insulation_residual_current : str = "insulation_residual_current"
-    pv_power : str = "pv_power"
-    grid_power : str = "grid_power"
-    frequency : str = "frequency"
-    power_l1 : str = "power_l1"
-    power_l2 : str = "power_l2"
-    power_l3 : str = "power_l3"
-    temp_a : str = "temp_a"
-    temp_b : str = "temp_b"
-    temp_c : str = "temp_c"
-    grid_reactive_power : str = "grid_reactive_power"
-    grid_reactive_power_l1 : str = "grid_reactive_power_l1"
-    grid_reactive_power_l2 : str = "grid_reactive_power_l2"
-    grid_reactive_power_l3 : str = "grid_reactive_power_l3"
-    grid_apparent_power : str = "grid_apparent_power"
-    grid_apparent_power_l1 : str = "grid_apparent_power_l1"
-    grid_apparent_power_l2 : str = "grid_apparent_power_l2"
-    grid_apparent_power_l3 : str = "grid_apparent_power_l3"
-    grid_power_factor : str = "grid_power_factor"
-    current_l1 : str = "current_l1"
-    current_l2 : str = "current_l2"
-    current_l3 : str = "current_l3"
-    current_total : str = "current_total"
-    voltage_l1 : str = "voltage_l1"
-    voltage_l2 : str = "voltage_l2"
-    voltage_l3 : str = "voltage_l3"
-    total_yield : str = "total_yield"
-    daily_yield : str = "daily_yield"
-    metering_power_supplied : str = "metering_power_supplied"
-    metering_power_absorbed : str = "metering_power_absorbed"
-    metering_frequency : str = "metering_frequency"
-    metering_total_yield : str = "metering_total_yield"
-    metering_total_absorbed : str = "metering_total_absorbed"
-    metering_current_l1 : str = "metering_current_l1"
-    metering_current_l2 : str = "metering_current_l2"
-    metering_current_l3 : str = "metering_current_l3"
-    metering_voltage_l1 : str = "metering_voltage_l1"
-    metering_voltage_l2 : str = "metering_voltage_l2"
-    metering_voltage_l3 : str = "metering_voltage_l3"
-    metering_active_power_feed_l1 : str = "metering_active_power_feed_l1"
-    metering_active_power_feed_l2 : str = "metering_active_power_feed_l2"
-    metering_active_power_feed_l3 : str = "metering_active_power_feed_l3"
-    metering_active_power_draw_l1 : str = "metering_active_power_draw_l1"
-    metering_active_power_draw_l2 : str = "metering_active_power_draw_l2"
-    metering_active_power_draw_l3 : str = "metering_active_power_draw_l3"
-    metering_current_consumption : str = "metering_current_consumption"
-    pv_gen_meter : str = "pv_gen_meter"
-    sps_voltage : str = "sps_voltage"
-    sps_current : str = "sps_current"
-    sps_power : str = "sps_power"
-    optimizer_serial : str = "optimizer_serial"
-    optimizer_power : str = "optimizer_power"
-    optimizer_current : str = "optimizer_current"
-    optimizer_voltage : str = "optimizer_voltage"
-    optimizer_temp : str = "optimizer_temp"
-    battery_soc_total : str = "battery_soc_total"
-    battery_soc_a : str = "battery_soc_a"
-    battery_soc_b : str = "battery_soc_b"
-    battery_soc_c : str = "battery_soc_c"
-    battery_voltage_a : str = "battery_voltage_a"
-    battery_voltage_b : str = "battery_voltage_b"
-    battery_voltage_c : str = "battery_voltage_c"
-    battery_current_a : str = "battery_current_a"
-    battery_current_b : str = "battery_current_b"
-    battery_current_c : str = "battery_current_c"
-    battery_temp_a : str = "battery_temp_a"
-    battery_temp_b : str = "battery_temp_b"
-    battery_temp_c : str = "battery_temp_c"
-    battery_capacity_total : str = "battery_capacity_total"
-    battery_capacity_a : str = "battery_capacity_a"
-    battery_capacity_b : str = "battery_capacity_b"
-    battery_capacity_c : str = "battery_capacity_c"
-    battery_charging_voltage_a : str = "battery_charging_voltage_a"
-    battery_charging_voltage_b : str = "battery_charging_voltage_b"
-    battery_charging_voltage_c : str = "battery_charging_voltage_c"
-    battery_power_charge_total : str = "battery_power_charge_total"
-    battery_power_charge_a : str = "battery_power_charge_a"
-    battery_power_charge_b : str = "battery_power_charge_b"
-    battery_power_charge_c : str = "battery_power_charge_c"
-    battery_charge_total : str = "battery_charge_total"
-    battery_charge_a : str = "battery_charge_a"
-    battery_charge_b : str = "battery_charge_b"
-    battery_charge_c : str = "battery_charge_c"
-    battery_power_discharge_total : str = "battery_power_discharge_total"
-    battery_power_discharge_a : str = "battery_power_discharge_a"
-    battery_power_discharge_b : str = "battery_power_discharge_b"
-    battery_power_discharge_c : str = "battery_power_discharge_c"
-    battery_discharge_total : str = "battery_discharge_total"
-    battery_discharge_a : str = "battery_discharge_a"
-    battery_discharge_b : str = "battery_discharge_b"
-    battery_discharge_c : str = "battery_discharge_c"
-    serial_number : str = "serial_number"
-    device_name : str = "device_name"
-    device_type : str = "device_type"
-    device_manufacturer : str = "device_manufacturer"
-    device_sw_version : str = "device_sw_version"
-    inverter_power_limit : str = "inverter_power_limit"
-    energy_meter : str = "energy_meter"
+
+class Identifier:
+    # pylint: disable=too-few-public-methods
+    """All Sensor names
+    This list is considered part of the pysam interface and changes to names are considered a breaking change
+    """
+    pv_power_a: str = "pv_power_a"
+    pv_power_b: str = "pv_power_b"
+    pv_power_c: str = "pv_power_c"
+    pv_voltage_a: str = "pv_voltage_a"
+    pv_voltage_b: str = "pv_voltage_b"
+    pv_voltage_c: str = "pv_voltage_c"
+    pv_current_a: str = "pv_current_a"
+    pv_current_b: str = "pv_current_b"
+    pv_current_c: str = "pv_current_c"
+    insulation_residual_current: str = "insulation_residual_current"
+    pv_power: str = "pv_power"
+    grid_power: str = "grid_power"
+    frequency: str = "frequency"
+    power_l1: str = "power_l1"
+    power_l2: str = "power_l2"
+    power_l3: str = "power_l3"
+    temp_a: str = "temp_a"
+    temp_b: str = "temp_b"
+    temp_c: str = "temp_c"
+    grid_reactive_power: str = "grid_reactive_power"
+    grid_reactive_power_l1: str = "grid_reactive_power_l1"
+    grid_reactive_power_l2: str = "grid_reactive_power_l2"
+    grid_reactive_power_l3: str = "grid_reactive_power_l3"
+    grid_apparent_power: str = "grid_apparent_power"
+    grid_apparent_power_l1: str = "grid_apparent_power_l1"
+    grid_apparent_power_l2: str = "grid_apparent_power_l2"
+    grid_apparent_power_l3: str = "grid_apparent_power_l3"
+    grid_power_factor: str = "grid_power_factor"
+    current_l1: str = "current_l1"
+    current_l2: str = "current_l2"
+    current_l3: str = "current_l3"
+    current_total: str = "current_total"
+    voltage_l1: str = "voltage_l1"
+    voltage_l2: str = "voltage_l2"
+    voltage_l3: str = "voltage_l3"
+    total_yield: str = "total_yield"
+    daily_yield: str = "daily_yield"
+    metering_power_supplied: str = "metering_power_supplied"
+    metering_power_absorbed: str = "metering_power_absorbed"
+    metering_frequency: str = "metering_frequency"
+    metering_total_yield: str = "metering_total_yield"
+    metering_total_absorbed: str = "metering_total_absorbed"
+    metering_current_l1: str = "metering_current_l1"
+    metering_current_l2: str = "metering_current_l2"
+    metering_current_l3: str = "metering_current_l3"
+    metering_voltage_l1: str = "metering_voltage_l1"
+    metering_voltage_l2: str = "metering_voltage_l2"
+    metering_voltage_l3: str = "metering_voltage_l3"
+    metering_active_power_feed_l1: str = "metering_active_power_feed_l1"
+    metering_active_power_feed_l2: str = "metering_active_power_feed_l2"
+    metering_active_power_feed_l3: str = "metering_active_power_feed_l3"
+    metering_active_power_draw_l1: str = "metering_active_power_draw_l1"
+    metering_active_power_draw_l2: str = "metering_active_power_draw_l2"
+    metering_active_power_draw_l3: str = "metering_active_power_draw_l3"
+    metering_current_consumption: str = "metering_current_consumption"
+    pv_gen_meter: str = "pv_gen_meter"
+    sps_voltage: str = "sps_voltage"
+    sps_current: str = "sps_current"
+    sps_power: str = "sps_power"
+    optimizer_serial: str = "optimizer_serial"
+    optimizer_power: str = "optimizer_power"
+    optimizer_current: str = "optimizer_current"
+    optimizer_voltage: str = "optimizer_voltage"
+    optimizer_temp: str = "optimizer_temp"
+    battery_soc_total: str = "battery_soc_total"
+    battery_soc_a: str = "battery_soc_a"
+    battery_soc_b: str = "battery_soc_b"
+    battery_soc_c: str = "battery_soc_c"
+    battery_voltage_a: str = "battery_voltage_a"
+    battery_voltage_b: str = "battery_voltage_b"
+    battery_voltage_c: str = "battery_voltage_c"
+    battery_current_a: str = "battery_current_a"
+    battery_current_b: str = "battery_current_b"
+    battery_current_c: str = "battery_current_c"
+    battery_temp_a: str = "battery_temp_a"
+    battery_temp_b: str = "battery_temp_b"
+    battery_temp_c: str = "battery_temp_c"
+    battery_capacity_total: str = "battery_capacity_total"
+    battery_capacity_a: str = "battery_capacity_a"
+    battery_capacity_b: str = "battery_capacity_b"
+    battery_capacity_c: str = "battery_capacity_c"
+    battery_charging_voltage_a: str = "battery_charging_voltage_a"
+    battery_charging_voltage_b: str = "battery_charging_voltage_b"
+    battery_charging_voltage_c: str = "battery_charging_voltage_c"
+    battery_power_charge_total: str = "battery_power_charge_total"
+    battery_power_charge_a: str = "battery_power_charge_a"
+    battery_power_charge_b: str = "battery_power_charge_b"
+    battery_power_charge_c: str = "battery_power_charge_c"
+    battery_charge_total: str = "battery_charge_total"
+    battery_charge_a: str = "battery_charge_a"
+    battery_charge_b: str = "battery_charge_b"
+    battery_charge_c: str = "battery_charge_c"
+    battery_power_discharge_total: str = "battery_power_discharge_total"
+    battery_power_discharge_a: str = "battery_power_discharge_a"
+    battery_power_discharge_b: str = "battery_power_discharge_b"
+    battery_power_discharge_c: str = "battery_power_discharge_c"
+    battery_discharge_total: str = "battery_discharge_total"
+    battery_discharge_a: str = "battery_discharge_a"
+    battery_discharge_b: str = "battery_discharge_b"
+    battery_discharge_c: str = "battery_discharge_c"
+    serial_number: str = "serial_number"
+    device_name: str = "device_name"
+    device_type: str = "device_type"
+    device_class: str = "device_class"
+    device_manufacturer: str = "device_manufacturer"
+    device_sw_version: str = "device_sw_version"
+    inverter_power_limit: str = "inverter_power_limit"
+    energy_meter: str = "energy_meter"
     operating_status_genereal: str = "operating_status_general"
     operating_status: str = "operating_status"
     inverter_condition: str = "inverter_condition"
     inverter_system_init: str = "inverter_system_init"
     grid_connection_status: str = "grid_connection_status"
     grid_relay_status: str = "grid_relay_status"
     pv_isolation_resistance: str = "pv_isolation_resistance"
     grid_power_factor_excitation: str = "grid_power_factor_excitation"
     metering_total_consumption: str = "metering_total_consumption"
     battery_status_operating_mode: str = "battery_status_operating_mode"
     status: str = "status"
 
 
-'''
-Data-Source:
-https://www.sma.de/produkte/solar-wechselrichter/sunny-tripower-x
-Technical Information - Parameters and Measured Values STP 12-50 / STP 15-50 / STP 20-50 / STP 25-50 (Sunny Tripower X) with firmware package 03.02.07.R 
-https://github.com/sma-bluetooth/sma-bluetooth/blob/master/smatool.xml
-'''
+# Data-Source:
+# https://www.sma.de/produkte/solar-wechselrichter/sunny-tripower-x
+# Technical Information - Parameters and Measured Values STP 12-50 / STP 15-50 / STP 20-50 / STP 25-50 (Sunny Tripower X) with firmware package 03.02.07.R
+# https://github.com/sma-bluetooth/sma-bluetooth/blob/master/smatool.xml
 SMATagList: Dict[int, str] = {
     35: "Error",
     51: "Closed",
     276: "Instantaneous value",
     295: "MPP",
     303: "Off",
     307: "OK",
@@ -144,15 +153,16 @@
     336: "Contact the manufacturer",
     337: "Contact the installer",
     338: "Invalid",
     381: "Stop",
     402: "Phases L1 and L2 (phsAB)",
     403: "Phases L1 and L3 (phsAC)",
     404: "Phases L2 and L3 (phsBC)",
-    433: "Contant voltage",
+    # 433: "Contant voltage",
+    443: "Constant voltage",
     455: "Warning",
     461: "SMA",
     569: "activated",
     887: "No recommended action",
     1041: "leading / overexcited",
     1042: "lagging / underexcited",
     1069: "Reactive power / voltage characteristic curve Q(V)",
@@ -166,27 +176,28 @@
     1077: "Active power limitation P (W)",
     1078: "Active power limitation P (%) of PMAX",
     1079: "Active power limitation P via system control",
     1129: "Yes",
     1130: "No",
     1264: "Full dynamic grid support",
     1265: "Limited dynamic grid support",
-#    1295:
+    1295: "Standby",
     1387: "Reactive power Q, setpoint via analog input",
     1388: "cos φ, setpoint via analog input",
     1389: "Reactive power / voltage characteristic curve Q(U) with hysteresis and deadband",
     1390: "Active power limitation P via analog input",
     1391: "Active power limitation P via digital inputs",
     1392: "Errors",
     1393: "Wait for PV voltage",
     1394: "Wait for valid AC grid",
     1395: "DC area",
     1396: "AC grid",
     1438: "Automatic",
     1455: "Emergency stop",
+    1463: "backup",
     1466: "Waiting",
     1467: "Starting",
     1468: "MPP search",
     1469: "Shutdown",
     1470: "Event message",
     1471: "Warning/error e-mail OK",
     1472: "Warning/error e-mail not OK",
@@ -214,43 +225,40 @@
     # 2063: "Status digital inlet: DI2",
     # 2064: "Status digital inlet: DI2, DI3",
     # 2065: "Status digital inlet: DI2, DI3, DI4",
     # 2066: "Status digital inlet: DI2, DI4",
     # 2067: "Status digital inlet: DI3",
     # 2068: "Status digital inlet: DI3, DI4",
     # 2069: "Status digital inlet: DI4",
+    2119: "derating",
     2270: "cos φ or Q specification through optimum PV system control",
     2506: "Values maintained",
     2507: "Apply fallback values",
     4354: "Maximum active power export",
     4405: "Maximum active power WMax",
     4406: "Maximum reactive power VArMax",
     4433: "Zero at dead band boundary",
     4434: "Zero at origin (ZerAtZer)",
     4443: "Current power",
     4444: "Potential power",
     4450: "Q limitation",
     4562: "cos φ(V) charac. curve",
     4520: "Mean value of the phase voltages",
     4521: "Maximum phase voltage",
-    4718: "Boost Charging", # EV-Charger
-    4950: "Smart Chargig", # EV-Charger
-    5169: "Station locked", # EV-Charger
+    4718: "Boost Charging",  # EV-Charger
+    4950: "Smart Chargig",  # EV-Charger
+    5169: "Station locked",  # EV-Charger
     5249: "Potential power with characteristic curve break",
-
-
-
     # Device Classes
     8000: "All Devices",
     8001: "Solar Inverters",
     8002: "Wind Turbine Inverter",
     8007: "Batterie Inverters",
     8008: "EV Chargers",
     8009: "Hybrid Inverters",
-
     # Inverter Classes
     9000: "SWR 700",
     9001: "SWR 850",
     9002: "SWR 850E",
     9003: "SWR 1100",
     9004: "SWR 1100E",
     9005: "SWR 1100LV",
@@ -466,16 +474,16 @@
     9216: "SC 720 CP-US",
     9217: "SC 750 CP-US",
     9218: "SB 240 Dev",
     9219: "SB 240-US BTF",
     9220: "Grid Gate-20",
     9221: "SC 500 CP-US/600V",
     9222: "STP 10000TLEE-JP-10",
-    9223: "Sunny Island 6.0H",
-    9224: "Sunny Island 8.0H",
+    9223: "Sunny Island 6.0H-11",
+    9224: "Sunny Island 8.0H-11",
     9225: "SB 5000SE-10",
     9226: "SB 3600SE-10",
     9227: "SC 800CP-JP",
     9228: "SC 630CP-JP",
     9229: "WebBox-30",
     9230: "Power Reducer Box",
     9231: "Sunny Sensor Counter",
@@ -521,16 +529,16 @@
     9271: "STP 20000TLEE-JP-11",
     9272: "STP 10000TLEE-JP-11",
     9273: "SB 6000TL-21",
     9274: "SB 6000TL-US-22",
     9275: "SB 7000TL-US-22",
     9276: "SB 7600TL-US-22",
     9277: "SB 8000TL-US-22",
-    9278: "Sunny Island 3.0M",
-    9279: "Sunny Island 4.4M",
+    9278: "Sunny Island 3.0M-11",
+    9279: "Sunny Island 4.4M-11",
     9281: "STP 10000TL-20",
     9282: "STP 11000TL-20",
     9283: "STP 12000TL-20",
     9284: "STP 20000TL-30",
     9285: "STP 25000TL-30",
     9286: "Sunny Central Storage 500",
     9287: "Sunny Central Storage 630",
@@ -538,20 +546,19 @@
     9289: "Sunny Central Storage 760",
     9290: "Sunny Central Storage 800",
     9291: "Sunny Central Storage 850",
     9292: "Sunny Central Storage 900",
     9293: "SB 7700TL-US-22",
     9294: "SB20.0-3SP-40",
     9295: "SB30.0-3SP-40",
-
+    9310: "STP 30000TL-US-10",
+    9311: "STP 25000TL-JP-30",
+    9354: "STP 24500TL-JP-30",
     9489: "STP-20-50",
     9491: "STP-15-50",
     9492: "STP-12-50",
     9484: "EVC22-3AC-10",
-
-
-    200111: "Not connected", # EV-Charger
-    200112: "Sleep Mode", # EV-Charger
-    200113: "Active Mode", # EV-Charger
-    
+    200111: "Not connected",  # EV-Charger
+    200112: "Sleep Mode",  # EV-Charger
+    200113: "Active Mode",  # EV-Charger
     16777213: "Information not available",
 }
```

### Comparing `pysma_plus-0.2.4/pysmaplus/const_webconnect.py` & `pysma_plus-0.2.5/pysmaplus/const_webconnect.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Constants for SMA WebConnect library for Python."""
+
 URL_LOGIN = "/dyn/login.json"
 URL_LOGOUT = "/dyn/logout.json"
 URL_VALUES = "/dyn/getValues.json"
 URL_ALL_VALUES = "/dyn/getAllOnlValues.json"
 URL_ALL_PARAMS = "/dyn/getAllParamValues.json"
 URL_LOGGER = "/dyn/getLogger.json"
 URL_DASH_LOGGER = "/dyn/getDashLogger.json"
@@ -40,8 +41,7 @@
     "serial": "9999999999",
 }
 
 GENERIC_SENSORS = "generic"
 OPTIMIZERS_VIA_INVERTER = "optimizers"
 ENERGY_METER_VIA_INVERTER = "energy-meter"
 DEVICE_INFO = "device-info"
-
```

### Comparing `pysma_plus-0.2.4/pysmaplus/definitions_ennexos.py` & `pysma_plus-0.2.5/pysmaplus/definitions_ennexos.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,125 +1,221 @@
-from typing import Any, Dict
+"""
+Definition for all enneoxOS senosrs 
+"""
+
 from .sensor import Sensor
 from .const import Identifier
 from .const import SMATagList
 
 
 ennexosSensorProfiles = {
     "Sunny Tripower X ": [
         Sensor("Coolsys.Inverter.TmpVal.1", Identifier.temp_a, factor=1, unit="°C"),
         Sensor("Coolsys.Inverter.TmpVal.2", Identifier.temp_b, factor=1, unit="°C"),
         Sensor("Coolsys.Inverter.TmpVal.3", Identifier.temp_c, factor=1, unit="°C"),
         Sensor("DcMs.Amp.1", Identifier.pv_current_a, factor=1, unit="A"),
         Sensor("DcMs.Amp.2", Identifier.pv_current_b, factor=1, unit="A"),
         Sensor("DcMs.Amp.3", Identifier.pv_current_c, factor=1, unit="A"),
-        Sensor("DcMs.TotDcEnCntWh.1", None, factor=1, unit=None), # Energy released by string [A]
+        Sensor("DcMs.TotDcEnCntWh.1", None),  # Energy released by string [A]
         Sensor("DcMs.TotDcEnCntWh.2", None, factor=1, unit=None),
         Sensor("DcMs.TotDcEnCntWh.3", None, factor=1, unit=None),
         Sensor("DcMs.Vol.1", Identifier.pv_voltage_a, factor=1, unit="V"),
         Sensor("DcMs.Vol.2", Identifier.pv_voltage_b, factor=1, unit="V"),
         Sensor("DcMs.Vol.3", Identifier.pv_voltage_c, factor=1, unit="V"),
         Sensor("DcMs.Watt.1", Identifier.pv_power_a, factor=1, unit="W"),
         Sensor("DcMs.Watt.2", Identifier.pv_power_b, factor=1, unit="W"),
         Sensor("DcMs.Watt.3", Identifier.pv_power_c, factor=1, unit="W"),
-        Sensor("GridGuard.Cntry", None, factor=1, unit=None), # Country standard set
+        Sensor("GridGuard.Cntry", None, factor=1, unit=None),  # Country standard set
         Sensor("GridMs.A.phsA", Identifier.current_l1, factor=1, unit="A"),
         Sensor("GridMs.A.phsB", Identifier.current_l2, factor=1, unit="A"),
         Sensor("GridMs.A.phsC", Identifier.current_l3, factor=1, unit="A"),
-        Sensor("GridMs.GriTyp", None, factor=1, unit=None), # Measurement.GridMs.GriTyp
+        Sensor("GridMs.GriTyp", None, factor=1, unit=None),  # Measurement.GridMs.GriTyp
         Sensor("GridMs.Hz", Identifier.frequency, factor=1, unit="Hz"),
         Sensor("GridMs.PhV.phsA", Identifier.voltage_l1, factor=1, unit="V"),
-        Sensor("GridMs.PhV.phsA2B", None, factor=1, unit=None), # Grid voltage phase L1 against L2
+        Sensor(
+            "GridMs.PhV.phsA2B", None, factor=1, unit=None
+        ),  # Grid voltage phase L1 against L2
         Sensor("GridMs.PhV.phsB", Identifier.voltage_l2, factor=1, unit="V"),
-        Sensor("GridMs.PhV.phsB2C", None, factor=1, unit=None), # Grid voltage phase L2 against L3
+        Sensor(
+            "GridMs.PhV.phsB2C", None, factor=1, unit=None
+        ),  # Grid voltage phase L2 against L3
         Sensor("GridMs.PhV.phsC", Identifier.voltage_l3, factor=1, unit="V"),
-        Sensor("GridMs.PhV.phsC2A", None, factor=1, unit=None), # Grid voltage phase L3 against L1
+        Sensor(
+            "GridMs.PhV.phsC2A", None, factor=1, unit=None
+        ),  # Grid voltage phase L3 against L1
         Sensor("GridMs.TotA", Identifier.current_total, factor=1, unit="A"),
-        Sensor("GridMs.TotPFEEI", None, factor=1, unit=None),  # EEI displacement power factor
-        Sensor("GridMs.TotPFExt", None, factor=1, unit=None), # Excitation type of cos φ
-        Sensor("GridMs.TotPFPrc", None, factor=1, unit=None), # Displacement power factor
+        Sensor(
+            "GridMs.TotPFEEI", None, factor=1, unit=None
+        ),  # EEI displacement power factor
+        Sensor(
+            "GridMs.TotPFExt", None, factor=1, unit=None
+        ),  # Excitation type of cos φ
+        Sensor(
+            "GridMs.TotPFPrc", None, factor=1, unit=None
+        ),  # Displacement power factor
         Sensor("GridMs.TotVA", Identifier.grid_apparent_power, factor=1, unit="VA"),
         Sensor("GridMs.TotVAr", Identifier.grid_reactive_power, factor=1, unit="var"),
         Sensor("GridMs.TotW", Identifier.grid_power, factor=1, unit="W"),
         Sensor("GridMs.TotW.Pv", Identifier.pv_power, factor=1, unit="W"),
-        Sensor("GridMs.VA.phsA", Identifier.grid_apparent_power_l1, factor=1, unit="VA"),
-        Sensor("GridMs.VA.phsB", Identifier.grid_apparent_power_l2, factor=1, unit="VA"),
-        Sensor("GridMs.VA.phsC", Identifier.grid_apparent_power_l3, factor=1, unit="VA"),
-        Sensor("GridMs.VAr.phsA", Identifier.grid_reactive_power_l1, factor=1, unit="var"),
-        Sensor("GridMs.VAr.phsB", Identifier.grid_reactive_power_l2, factor=1, unit="var"),
-        Sensor("GridMs.VAr.phsC", Identifier.grid_reactive_power_l3, factor=1, unit="var"),
+        Sensor(
+            "GridMs.VA.phsA", Identifier.grid_apparent_power_l1, factor=1, unit="VA"
+        ),
+        Sensor(
+            "GridMs.VA.phsB", Identifier.grid_apparent_power_l2, factor=1, unit="VA"
+        ),
+        Sensor(
+            "GridMs.VA.phsC", Identifier.grid_apparent_power_l3, factor=1, unit="VA"
+        ),
+        Sensor(
+            "GridMs.VAr.phsA", Identifier.grid_reactive_power_l1, factor=1, unit="var"
+        ),
+        Sensor(
+            "GridMs.VAr.phsB", Identifier.grid_reactive_power_l2, factor=1, unit="var"
+        ),
+        Sensor(
+            "GridMs.VAr.phsC", Identifier.grid_reactive_power_l3, factor=1, unit="var"
+        ),
         Sensor("GridMs.W.phsA", Identifier.power_l1, factor=1, unit="W"),
         Sensor("GridMs.W.phsB", Identifier.power_l2, factor=1, unit="W"),
         Sensor("GridMs.W.phsC", Identifier.power_l3, factor=1, unit="W"),
-        Sensor("InOut.GI1", None, factor=1, unit=None), # Digital group input
+        Sensor("InOut.GI1", None, factor=1, unit=None),  # Digital group input
         Sensor("Inverter.VArModCfg.PFCtlVolCfg.Stt", None, factor=1, unit=None),
-        Sensor("Isolation.FltA", Identifier.insulation_residual_current, factor=1000, unit="mA"),
-        Sensor("Isolation.LeakRis", None, factor=1, unit="kOhm"), # TODO "pv_isolation_resistance"
-        Sensor("Metering.TotFeedTms", None, factor=1, unit=None), 
-        Sensor("Metering.TotOpTms", None, factor=1, unit=None),
+        Sensor(
+            "Isolation.FltA",
+            Identifier.insulation_residual_current,
+            factor=1000,
+            unit="mA",
+        ),
+        Sensor(
+            "Isolation.LeakRis", None, factor=1, unit="kOhm"
+        ),  # TODO "pv_isolation_resistance"
+        Sensor("Metering.TotFeedTms", None),
+        Sensor("Metering.TotOpTms", None),
         Sensor("Metering.TotWhOut", Identifier.total_yield, factor=1000, unit="kWh"),
-        Sensor("Metering.TotWhOut.Pv", Identifier.pv_gen_meter, factor=1000, unit="kWh"),
+        Sensor(
+            "Metering.TotWhOut.Pv", Identifier.pv_gen_meter, factor=1000, unit="kWh"
+        ),
         Sensor("Operation.BckStt", None, factor=1, unit=None),
         Sensor("Operation.DrtStt", None, factor=1, unit=None),
         Sensor("Operation.Evt.Dsc", None, factor=1, unit=None),
         Sensor("Operation.Evt.EvtNo", None, factor=1, unit=None),
         Sensor("Operation.Evt.Msg", None, factor=1, unit=None),
         Sensor("Operation.EvtCntIstl", None, factor=1, unit=None),
         Sensor("Operation.EvtCntUsr", None, factor=1, unit=None),
         Sensor("Operation.GriSwCnt", None, factor=1, unit=None),
-        Sensor("Operation.GriSwStt", Identifier.grid_relay_status, unit=None,  mapper=SMATagList), 
-        Sensor("Operation.Health", Identifier.status, factor=1, unit=None, mapper=SMATagList),
+        Sensor(
+            "Operation.GriSwStt",
+            Identifier.grid_relay_status,
+            unit=None,
+            mapper=SMATagList,
+        ),
+        Sensor(
+            "Operation.Health",
+            Identifier.status,
+            factor=1,
+            unit=None,
+            mapper=SMATagList,
+        ),
         Sensor("Operation.HealthStt.Alm", None, factor=1, unit=None),
         Sensor("Operation.HealthStt.Ok", None, factor=1, unit=None),
         Sensor("Operation.HealthStt.Wrn", None, factor=1, unit=None),
-        Sensor("Operation.OpStt", Identifier.operating_status_genereal, unit=None, mapper=SMATagList),
+        Sensor(
+            "Operation.OpStt",
+            Identifier.operating_status_genereal,
+            unit=None,
+            mapper=SMATagList,
+        ),
         Sensor("Operation.PvGriConn", None, factor=1, unit=None),
         Sensor("Operation.RstrLokStt", None, factor=1, unit=None),
         Sensor("Operation.RunStt", None, factor=1, unit=None),
         Sensor("Operation.StandbyStt", None, factor=1, unit=None),
         Sensor("Operation.VArCtl.VArModAct", None, factor=1, unit=None),
         Sensor("Operation.VArCtl.VArModStt", None, factor=1, unit=None),
         Sensor("Operation.WMaxLimSrc", None, factor=1, unit=None),
         Sensor("Operation.WMinLimSrc", None, factor=1, unit=None),
-        Sensor("PvGen.PvW", None, factor=1, unit=None), #  PV generation power
-        Sensor("PvGen.PvWh", None, factor=1, unit=None), # Meter count and PV gen. meter
-        Sensor("Spdwr.ComSocA.Stt", None, factor=1, unit=None), # Speedwire connection status of SMACOM A
-        Sensor("SunSpecSig.SunSpecTx.1", None, factor=1, unit=None), #SunSpec life sign [1]
+        Sensor("PvGen.PvW", None, factor=1, unit=None),  #  PV generation power
+        Sensor(
+            "PvGen.PvWh", None, factor=1, unit=None
+        ),  # Meter count and PV gen. meter
+        Sensor(
+            "Spdwr.ComSocA.Stt", None, factor=1, unit=None
+        ),  # Speedwire connection status of SMACOM A
+        Sensor(
+            "SunSpecSig.SunSpecTx.1", None, factor=1, unit=None
+        ),  # SunSpec life sign [1]
         Sensor("Upd.Stt", None, factor=1, unit=None),
-        Sensor("WebConn.Stt", None, factor=1, unit=None), #  Status of the Webconnect functionality
-        Sensor("Wl.AcqStt", None, factor=1, unit=None), # Status of WiFi scan
-        Sensor("Wl.AntMod", None, factor=1, unit=None), #  WiFi antenna type
-        Sensor("Wl.ConnStt", None, factor=1, unit=None), # WiFi connection status
-        Sensor("Wl.SigPwr", None, factor=1, unit=None), # Signal strength of the selected network
-        Sensor("Wl.SoftAcsConnStt", None, factor=1, unit=None), #Soft Access Point status
-        Sensor("Setpoint.PlantControl.InOut.GO1", None, factor=1, unit=None)
+        Sensor(
+            "WebConn.Stt", None, factor=1, unit=None
+        ),  #  Status of the Webconnect functionality
+        Sensor("Wl.AcqStt", None, factor=1, unit=None),  # Status of WiFi scan
+        Sensor("Wl.AntMod", None, factor=1, unit=None),  #  WiFi antenna type
+        Sensor("Wl.ConnStt", None, factor=1, unit=None),  # WiFi connection status
+        Sensor(
+            "Wl.SigPwr", None, factor=1, unit=None
+        ),  # Signal strength of the selected network
+        Sensor(
+            "Wl.SoftAcsConnStt", None, factor=1, unit=None
+        ),  # Soft Access Point status
+        Sensor("Setpoint.PlantControl.InOut.GO1", None, factor=1, unit=None),
     ],
     "SMA EV Charger ": [
-        Sensor("ChaSess.WhIn", None, factor=1, unit=None), # charging_session_energy
-        Sensor("Chrg.ModSw", None, factor=1, unit=None, mapper=SMATagList), # position_of_rotary_switch 4950 or 4718
-        Sensor("GridMs.A.phsA", Identifier.current_l1, factor=1, unit="A"), #Netzstrom Phase L1
+        Sensor("ChaSess.WhIn", None, factor=1, unit=None),  # charging_session_energy
+        Sensor(
+            "Chrg.ModSw", None, factor=1, unit=None, mapper=SMATagList
+        ),  # position_of_rotary_switch 4950 or 4718
+        Sensor(
+            "GridMs.A.phsA", Identifier.current_l1, factor=1, unit="A"
+        ),  # Netzstrom Phase L1
         Sensor("GridMs.A.phsB", Identifier.current_l2, factor=1, unit="A"),
         Sensor("GridMs.A.phsC", Identifier.current_l3, factor=1, unit="A"),
         Sensor("GridMs.Hz", Identifier.frequency, factor=1, unit="Hz"),
-        Sensor("GridMs.PhV.phsA", Identifier.voltage_l1, factor=1, unit="V"),#Netzspannung Phase L1
+        Sensor(
+            "GridMs.PhV.phsA", Identifier.voltage_l1, factor=1, unit="V"
+        ),  # Netzspannung Phase L1
         Sensor("GridMs.PhV.phsB", Identifier.voltage_l2, factor=1, unit="V"),
         Sensor("GridMs.PhV.phsC", Identifier.voltage_l3, factor=1, unit="V"),
         Sensor("GridMs.TotPF", None, factor=1, unit=None),
         Sensor("GridMs.TotVA", Identifier.grid_apparent_power, factor=1, unit="VA"),
         Sensor("GridMs.TotVAr", Identifier.grid_reactive_power, factor=1, unit="var"),
         Sensor("InOut.GI1", None, factor=1, unit=None),
-        Sensor("Metering.GridMs.TotWIn", Identifier.metering_power_absorbed, factor=1, unit="W"), #
-        Sensor("Metering.GridMs.TotWIn.ChaSta", None, factor=1, unit=None), # same as Metering.GridMs.TotWIn
-        Sensor("Metering.GridMs.TotWhIn", Identifier.metering_total_absorbed, factor=1000, unit="kWh"), # charging_station_meter_reading
-        Sensor("Metering.GridMs.TotWhIn.ChaSta", None, factor=1, unit=None), # same as Metering.GridMs.TotWhIn 
-        Sensor("Operation.EVeh.ChaStt", Identifier.operating_status, factor=1, unit=None, mapper=SMATagList), # charging_session_status
-        Sensor("Operation.EVeh.Health", Identifier.status, factor=1, unit=None, mapper=SMATagList), 
+        Sensor(
+            "Metering.GridMs.TotWIn",
+            Identifier.metering_power_absorbed,
+            factor=1,
+            unit="W",
+        ),  #
+        Sensor(
+            "Metering.GridMs.TotWIn.ChaSta", None, factor=1, unit=None
+        ),  # same as Metering.GridMs.TotWIn
+        Sensor(
+            "Metering.GridMs.TotWhIn",
+            Identifier.metering_total_absorbed,
+            factor=1000,
+            unit="kWh",
+        ),  # charging_station_meter_reading
+        Sensor(
+            "Metering.GridMs.TotWhIn.ChaSta", None, factor=1, unit=None
+        ),  # same as Metering.GridMs.TotWhIn
+        Sensor(
+            "Operation.EVeh.ChaStt",
+            Identifier.operating_status,
+            factor=1,
+            unit=None,
+            mapper=SMATagList,
+        ),  # charging_session_status
+        Sensor(
+            "Operation.EVeh.Health",
+            Identifier.status,
+            factor=1,
+            unit=None,
+            mapper=SMATagList,
+        ),
         Sensor("Operation.Evt.Msg", None, factor=1, unit=None),
-        Sensor("Operation.Health", None, factor=1, unit=None), # same as EVeh.Health?
+        Sensor("Operation.Health", None, factor=1, unit=None),  # same as EVeh.Health?
         Sensor("Operation.WMaxLimNom", None, factor=1, unit=None),
         Sensor("Operation.WMaxLimSrc", None, factor=1, unit=None),
         Sensor("Wl.AcqStt", None, factor=1, unit=None),
         Sensor("Wl.ConnStt", None, factor=1, unit=None),
         Sensor("Wl.SigPwr", None, factor=1, unit=None),
         Sensor("Wl.SoftAcsConnStt", None, factor=1, unit=None),
-    ]
+    ],
 }
```

### Comparing `pysma_plus-0.2.4/pysmaplus/definitions_webconnect.py` & `pysma_plus-0.2.5/pysmaplus/definitions_webconnect.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,21 +1,24 @@
 """Sensor definitions for SMA WebConnect library for Python."""
+
 from .const_webconnect import (
     DEVICE_INFO,
     ENERGY_METER_VIA_INVERTER,
     GENERIC_SENSORS,
     JMESPATHS_TAG,
     OPTIMIZERS_VIA_INVERTER,
 )
 from .sensor import Sensor
 from .const import Identifier
 
 # Status - Operation
 #: Status of the device
-status = Sensor("6180_08214800", Identifier.status, path=JMESPATHS_TAG, l10n_translate=True)
+status = Sensor(
+    "6180_08214800", Identifier.status, path=JMESPATHS_TAG, l10n_translate=True
+)
 #: General operating status
 operating_status_general = Sensor(
     "6180_08412800",
     Identifier.operating_status_genereal,
     path=JMESPATHS_TAG,
     l10n_translate=True,
     enabled=False,
@@ -108,15 +111,17 @@
 #: Current power generated by the solar panels
 pv_power = Sensor("6100_0046C200", Identifier.pv_power, unit="W", enabled=False)
 
 # AC Side - Grid measurements
 #: Power supplied to the grid. grid_power = power_l1 + power_l2 + power_l3
 grid_power = Sensor("6100_40263F00", Identifier.grid_power, unit="W")
 #: Grid frequency
-frequency = Sensor("6100_00465700", Identifier.frequency, unit="Hz", factor=100, enabled=False)
+frequency = Sensor(
+    "6100_00465700", Identifier.frequency, unit="Hz", factor=100, enabled=False
+)
 
 # AC Side - Grid measurements - Active power
 #: Power for phase 1
 power_l1 = Sensor("6100_40464000", Identifier.power_l1, unit="W", enabled=False)
 #: Power for phase 2
 power_l2 = Sensor("6100_40464100", Identifier.power_l2, unit="W", enabled=False)
 #: Power for phase 3
@@ -171,41 +176,57 @@
     path=JMESPATHS_TAG,
     l10n_translate=True,
     enabled=False,
 )
 
 # AC Side - Grid measurements - Phase Current
 #: Current for phase 1
-current_l1 = Sensor("6100_40465300", Identifier.current_l1, unit="A", factor=1000, enabled=False)
+current_l1 = Sensor(
+    "6100_40465300", Identifier.current_l1, unit="A", factor=1000, enabled=False
+)
 #: Current for phase 2
-current_l2 = Sensor("6100_40465400", Identifier.current_l2, unit="A", factor=1000, enabled=False)
+current_l2 = Sensor(
+    "6100_40465400", Identifier.current_l2, unit="A", factor=1000, enabled=False
+)
 #: Current for phase 3
-current_l3 = Sensor("6100_40465500", Identifier.current_l3, unit="A", factor=1000, enabled=False)
+current_l3 = Sensor(
+    "6100_40465500", Identifier.current_l3, unit="A", factor=1000, enabled=False
+)
 #: Total Current
 current_total = Sensor("6100_00664F00", Identifier.current_total, unit="A", factor=1000)
 
 # AC Side - Grid measurements - Phase voltage
 #: Voltage for phase 1
-voltage_l1 = Sensor("6100_00464800", Identifier.voltage_l1, unit="V", factor=100, enabled=False)
+voltage_l1 = Sensor(
+    "6100_00464800", Identifier.voltage_l1, unit="V", factor=100, enabled=False
+)
 #: Voltage for phase 2
-voltage_l2 = Sensor("6100_00464900", Identifier.voltage_l2, unit="V", factor=100, enabled=False)
+voltage_l2 = Sensor(
+    "6100_00464900", Identifier.voltage_l2, unit="V", factor=100, enabled=False
+)
 #: Voltage for phase 3
-voltage_l3 = Sensor("6100_00464A00", Identifier.voltage_l3, unit="V", factor=100, enabled=False)
+voltage_l3 = Sensor(
+    "6100_00464A00", Identifier.voltage_l3, unit="V", factor=100, enabled=False
+)
 
 # AC Side - Measured values - energy
 #: Total power yield from a solar installation
 total_yield = Sensor("6400_00260100", Identifier.total_yield, unit="kWh", factor=1000)
 #: The solar plant's yield for today
 daily_yield = Sensor("6400_00262200", Identifier.daily_yield, unit="Wh")
 
 # AC Side - Measured values - Grid measurements
 #: Power supplied to grid measured by energy meter
-metering_power_supplied = Sensor("6100_40463600", Identifier.metering_power_supplied, unit="W")
+metering_power_supplied = Sensor(
+    "6100_40463600", Identifier.metering_power_supplied, unit="W"
+)
 #: Power absorbed fromgrid measured by energy meter
-metering_power_absorbed = Sensor("6100_40463700", Identifier.metering_power_absorbed, unit="W")
+metering_power_absorbed = Sensor(
+    "6100_40463700", Identifier.metering_power_absorbed, unit="W"
+)
 #: Grid frequency measured by energy meter
 metering_frequency = Sensor(
     "6100_00468100", Identifier.metering_frequency, unit="Hz", factor=100
 )
 #: Total power supplied to the grid measured by energy meter
 metering_total_yield = Sensor(
     "6400_00462400", Identifier.metering_total_yield, unit="kWh", factor=1000
@@ -318,19 +339,25 @@
 )
 
 
 # Battery (inverter) - Battery (general parameters)
 #: Total battery state of charge
 battery_soc_total = Sensor("6100_00295A00", Identifier.battery_soc_total, unit="%")
 #: State of charge battery A
-battery_soc_a = Sensor("6100_00498F00_0", Identifier.battery_soc_a, unit="%", enabled=False)
+battery_soc_a = Sensor(
+    "6100_00498F00_0", Identifier.battery_soc_a, unit="%", enabled=False
+)
 #: State of charge battery B
-battery_soc_b = Sensor("6100_00498F00_1", Identifier.battery_soc_b, unit="%", enabled=False)
+battery_soc_b = Sensor(
+    "6100_00498F00_1", Identifier.battery_soc_b, unit="%", enabled=False
+)
 #: State of charge battery C
-battery_soc_c = Sensor("6100_00498F00_2", Identifier.battery_soc_c, unit="%", enabled=False)
+battery_soc_c = Sensor(
+    "6100_00498F00_2", Identifier.battery_soc_c, unit="%", enabled=False
+)
 #: Voltage battery A
 battery_voltage_a = Sensor(
     "6100_00495C00_0", Identifier.battery_voltage_a, unit="V", factor=100, enabled=False
 )
 #: Voltage battery B
 battery_voltage_b = Sensor(
     "6100_00495C00_1", Identifier.battery_voltage_b, unit="V", factor=100, enabled=False
@@ -348,30 +375,38 @@
     "6100_40495D00_1", Identifier.battery_current_b, unit="A", factor=1000
 )
 #: Current battery C
 battery_current_c = Sensor(
     "6100_40495D00_2", Identifier.battery_current_c, unit="A", factor=1000
 )
 #: Temperature battery A
-battery_temp_a = Sensor("6100_40495B00_0", Identifier.battery_temp_a, unit="°C", factor=10)
+battery_temp_a = Sensor(
+    "6100_40495B00_0", Identifier.battery_temp_a, unit="°C", factor=10
+)
 #: Temperature battery B
-battery_temp_b = Sensor("6100_40495B00_1", Identifier.battery_temp_b, unit="°C", factor=10)
+battery_temp_b = Sensor(
+    "6100_40495B00_1", Identifier.battery_temp_b, unit="°C", factor=10
+)
 #: Temperature battery C
-battery_temp_c = Sensor("6100_40495B00_2", Identifier.battery_temp_c, unit="°C", factor=10)
+battery_temp_c = Sensor(
+    "6100_40495B00_2", Identifier.battery_temp_c, unit="°C", factor=10
+)
 #: Battery status operating mode
 battery_status_operating_mode = Sensor(
     "6180_08495E00",
     Identifier.battery_status_operating_mode,
     path=JMESPATHS_TAG,
     l10n_translate=True,
 )
 
 # Battery (inverter) - Diagnosis
 #: Total battery capacity
-battery_capacity_total = Sensor("6100_00696E00", Identifier.battery_capacity_total, unit="%")
+battery_capacity_total = Sensor(
+    "6100_00696E00", Identifier.battery_capacity_total, unit="%"
+)
 #: Capacity battery A
 battery_capacity_a = Sensor(
     "6100_00499100_0", Identifier.battery_capacity_a, unit="%", enabled=False
 )
 #: Capacity battery B
 battery_capacity_b = Sensor(
     "6100_00499100_1", Identifier.battery_capacity_b, unit="%", enabled=False
@@ -380,23 +415,35 @@
 battery_capacity_c = Sensor(
     "6100_00499100_2", Identifier.battery_capacity_c, unit="%", enabled=False
 )
 
 # Battery (inverter) - Charge (voltage)
 #: Charging voltage battery A
 battery_charging_voltage_a = Sensor(
-    "6102_00493500_0", Identifier.battery_charging_voltage_a, unit="V", factor=100, enabled=False
+    "6102_00493500_0",
+    Identifier.battery_charging_voltage_a,
+    unit="V",
+    factor=100,
+    enabled=False,
 )
 #: Charging voltage battery B
 battery_charging_voltage_b = Sensor(
-    "6102_00493500_1", Identifier.battery_charging_voltage_b, unit="V", factor=100, enabled=False
+    "6102_00493500_1",
+    Identifier.battery_charging_voltage_b,
+    unit="V",
+    factor=100,
+    enabled=False,
 )
 #: Charging voltage battery C
 battery_charging_voltage_c = Sensor(
-    "6102_00493500_2", Identifier.battery_charging_voltage_c, unit="V", factor=100, enabled=False
+    "6102_00493500_2",
+    Identifier.battery_charging_voltage_c,
+    unit="V",
+    factor=100,
+    enabled=False,
 )
 
 # Battery (inverter) - Battery charge (power & energy)
 #: Total charging power
 battery_power_charge_total = Sensor(
     "6100_00496900", Identifier.battery_power_charge_total, unit="W"
 )
@@ -414,23 +461,35 @@
 )
 #: Total charge
 battery_charge_total = Sensor(
     "6400_00496700", Identifier.battery_charge_total, unit="kWh", factor=1000
 )
 #: Charge battery A
 battery_charge_a = Sensor(
-    "6400_00499500_0", Identifier.battery_charge_a, unit="kWh", factor=1000, enabled=False
+    "6400_00499500_0",
+    Identifier.battery_charge_a,
+    unit="kWh",
+    factor=1000,
+    enabled=False,
 )
 #: Charge battery B
 battery_charge_b = Sensor(
-    "6400_00499500_1", Identifier.battery_charge_b, unit="kWh", factor=1000, enabled=False
+    "6400_00499500_1",
+    Identifier.battery_charge_b,
+    unit="kWh",
+    factor=1000,
+    enabled=False,
 )
 #: Charge battery C
 battery_charge_c = Sensor(
-    "6400_00499500_2", Identifier.battery_charge_c, unit="kWh", factor=1000, enabled=False
+    "6400_00499500_2",
+    Identifier.battery_charge_c,
+    unit="kWh",
+    factor=1000,
+    enabled=False,
 )
 
 # Battery (inverter) - Battery discharge (power & energy)
 #: Total discharging power
 battery_power_discharge_total = Sensor(
     "6100_00496A00", Identifier.battery_power_discharge_total, unit="W"
 )
@@ -448,45 +507,62 @@
 )
 #: Total discharge
 battery_discharge_total = Sensor(
     "6400_00496800", Identifier.battery_discharge_total, unit="kWh", factor=1000
 )
 #: Discharge battery A
 battery_discharge_a = Sensor(
-    "6400_00499600_0", Identifier.battery_discharge_a, unit="kWh", factor=1000, enabled=False
+    "6400_00499600_0",
+    Identifier.battery_discharge_a,
+    unit="kWh",
+    factor=1000,
+    enabled=False,
 )
 #: Discharge battery B
 battery_discharge_b = Sensor(
-    "6400_00499600_1", Identifier.battery_discharge_b, unit="kWh", factor=1000, enabled=False
+    "6400_00499600_1",
+    Identifier.battery_discharge_b,
+    unit="kWh",
+    factor=1000,
+    enabled=False,
 )
 #: Discharge battery C
 battery_discharge_c = Sensor(
-    "6400_00499600_2", Identifier.battery_discharge_c, unit="kWh", factor=1000, enabled=False
+    "6400_00499600_2",
+    Identifier.battery_discharge_c,
+    unit="kWh",
+    factor=1000,
+    enabled=False,
 )
 
 # Device Parameters
 # Type Label - Type Label
 #: Device serial number
 serial_number = Sensor("6800_00A21E00", Identifier.serial_number)
 #: Device name
 device_name = Sensor("6800_10821E00", Identifier.device_name)
 #: Device type
 device_type = Sensor(
     "6800_08822000", Identifier.device_type, path=JMESPATHS_TAG, l10n_translate=True
 )
 #: Device manufactorer
 device_manufacturer = Sensor(
-    "6800_08822B00", Identifier.device_manufacturer, path=JMESPATHS_TAG, l10n_translate=True
+    "6800_08822B00",
+    Identifier.device_manufacturer,
+    path=JMESPATHS_TAG,
+    l10n_translate=True,
 )
 #: Device software version
 device_sw_version = Sensor("6800_00823400", Identifier.device_sw_version)
 
 # Device - Inverter
 #: Power limit of the Inverter
-inverter_power_limit = Sensor("6800_00832A00", Identifier.inverter_power_limit, unit="W")
+inverter_power_limit = Sensor(
+    "6800_00832A00", Identifier.inverter_power_limit, unit="W"
+)
 
 # System communication - Meter on Speedwire
 #: Serial number of energy meter
 energy_meter = Sensor("6800_008AA300", Identifier.energy_meter)
 
 
 sensor_map = {
```

### Comparing `pysma_plus-0.2.4/pysmaplus/device_em.py` & `pysma_plus-0.2.5/pysmaplus/device_em.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,65 +1,74 @@
+"""Interface for SMA Energy Meters and Sunny Home Manager 2 (SHM2)
+
+see https://www.unifox.at/software/sma-em-daemon/
+see https://cdn.sma.de/fileadmin/content/www.developer.sma.de/docs/EMETER-Protokoll-TI-en-10.pdf?v=1699276024
+
+"""
+
 import base64
 import socket
 import struct
 import copy
 import logging
 from typing import Any, Dict
 import datetime
 
-# https://www.unifox.at/software/sma-em-daemon/
-# https://cdn.sma.de/fileadmin/content/www.developer.sma.de/docs/EMETER-Protokoll-TI-en-10.pdf?v=1699276024
-
 
 from .sensor import Sensor
 from .const import Identifier
 
 from .exceptions import (
     SmaConnectionException,
     SmaReadException,
 )
 from .sensor import Sensors
 from .device import Device
 
-obis2sensor= [
-    Sensor("1:4:0", Identifier.metering_power_absorbed, factor=10, unit="W"), # p consume
+obis2sensor = [
+    Sensor(
+        "1:4:0", Identifier.metering_power_absorbed, factor=10, unit="W"
+    ),  # p consume
     Sensor("1:8:0", Identifier.metering_total_absorbed, factor=3600000, unit="kWh"),
-    Sensor("2:4:0", Identifier.metering_power_supplied, factor=10, unit="W"), # p supply
-    Sensor("2:8:0", Identifier.metering_total_yield, factor=3600000, unit="kWh", ),
-    Sensor("3:4:0", None), # q consume
+    Sensor(
+        "2:4:0", Identifier.metering_power_supplied, factor=10, unit="W"
+    ),  # p supply
+    Sensor(
+        "2:8:0",
+        Identifier.metering_total_yield,
+        factor=3600000,
+        unit="kWh",
+    ),
+    Sensor("3:4:0", None),  # q consume
     Sensor("3:8:0", None),
-    Sensor("4:4:0", None), # q supply
+    Sensor("4:4:0", None),  # q supply
     Sensor("4:8:0", None),
-    Sensor("9:4:0", None), # s consume
+    Sensor("9:4:0", None),  # s consume
     Sensor("9:8:0", None),
-    Sensor("10:4:0", None), # s supply
+    Sensor("10:4:0", None),  # s supply
     Sensor("10:8:0", None),
-    Sensor("13:4:0", None), # cospi
-    Sensor("14:4:0", Identifier.metering_frequency, factor=1000, unit="Hz"), # freq
-
+    Sensor("13:4:0", None),  # cospi
+    Sensor("14:4:0", Identifier.metering_frequency, factor=1000, unit="Hz"),  # freq
     # Phase 1
-
     Sensor("21:4:0", Identifier.metering_active_power_draw_l1, factor=10, unit="W"),
     Sensor("21:8:0", None),
     Sensor("22:4:0", Identifier.metering_active_power_feed_l1, factor=10, unit="W"),
     Sensor("22:8:0", None),
     Sensor("23:4:0", None),
     Sensor("23:8:0", None),
     Sensor("24:4:0", None),
     Sensor("24:8:0", None),
     Sensor("29:4:0", None),
     Sensor("29:8:0", None),
     Sensor("30:4:0", None),
     Sensor("30:8:0", None),
     Sensor("31:4:0", Identifier.metering_current_l1, factor=1000, unit="A"),
     Sensor("32:4:0", Identifier.metering_voltage_l1, factor=1000, unit="V"),
-    Sensor("33:4:0", None), #cosphi1
-
+    Sensor("33:4:0", None),  # cosphi1
     # Phase 2
-
     Sensor("41:4:0", Identifier.metering_active_power_draw_l2, factor=10, unit="W"),
     Sensor("41:8:0", None),
     Sensor("42:4:0", Identifier.metering_active_power_feed_l2, factor=10, unit="W"),
     Sensor("42:8:0", None),
     Sensor("43:4:0", None),
     Sensor("43:8:0", None),
     Sensor("44:4:0", None),
@@ -67,15 +76,14 @@
     Sensor("49:4:0", None),
     Sensor("49:8:0", None),
     Sensor("50:4:0", None),
     Sensor("50:8:0", None),
     Sensor("51:4:0", Identifier.metering_current_l2, factor=1000, unit="A"),
     Sensor("52:4:0", Identifier.metering_voltage_l2, factor=1000, unit="V"),
     Sensor("53:4:0", None),
-
     # Phase 3
     Sensor("61:4:0", Identifier.metering_active_power_draw_l3, factor=10, unit="W"),
     Sensor("61:8:0", None),
     Sensor("62:4:0", Identifier.metering_active_power_feed_l3, factor=10, unit="W"),
     Sensor("62:8:0", None),
     Sensor("63:4:0", None),
     Sensor("63:8:0", None),
@@ -83,86 +91,91 @@
     Sensor("64:8:0", None),
     Sensor("69:4:0", None),
     Sensor("69:8:0", None),
     Sensor("70:4:0", None),
     Sensor("70:8:0", None),
     Sensor("71:4:0", Identifier.metering_current_l3, factor=1000, unit="A"),
     Sensor("72:4:0", Identifier.metering_voltage_l3, factor=1000, unit="V"),
-    Sensor("73:4:0", None)
+    Sensor("73:4:0", None),
 ]
 
 
 _LOGGER = logging.getLogger(__name__)
+
+
 class SMAspeedwireEM(Device):
     """Class to connect to the ennexos based SMA inverters. (e.g. Tripower X Devices)"""
+
     _sock: socket
-    _susyid: Dict[int, Any] = {270: "Energy Meter", 349: "Energy Meter 2", 372: "Sunny Home Manager 2"}
+    _susyid: Dict[int, Any] = {
+        270: "Energy Meter",
+        349: "Energy Meter 2",
+        372: "Sunny Home Manager 2",
+    }
     _last_packet: bytes = None
 
     def __init__(self):
         """Init SMA connection.
 
         Args:
             session (ClientSession): aiohttp client session
             url (str): Url or IP address of device
             password (str, optional): Password to use during login.
-            group (str, optional): Username to use during login. 
+            group (str, optional): Username to use during login.
 
         """
-        pass
 
     async def new_session(self) -> bool:
         """Establish a new session.
 
         Returns:
             bool: authentication successful
         """
-        MCAST_GRP = '239.12.255.254'
-        MCAST_PORT = 9522
-        IPBIND = '0.0.0.0'
-
-        self._sock = socket.socket(socket.AF_INET, socket.SOCK_DGRAM, socket.IPPROTO_UDP)
+        mcast_grp = "239.12.255.254"
+        mcast_port = 9522
+        ipbind = "0.0.0.0"
+
+        self._sock = socket.socket(
+            socket.AF_INET, socket.SOCK_DGRAM, socket.IPPROTO_UDP
+        )
         self._sock.setsockopt(socket.SOL_SOCKET, socket.SO_REUSEADDR, 1)
         self._sock.settimeout(5)
-        self._sock.bind(("", MCAST_PORT))
+        self._sock.bind(("", mcast_port))
         try:
-            mreq = struct.pack("4s4s", socket.inet_aton(MCAST_GRP), socket.inet_aton(IPBIND))
+            mreq = struct.pack(
+                "4s4s", socket.inet_aton(mcast_grp), socket.inet_aton(ipbind)
+            )
             self._sock.setsockopt(socket.IPPROTO_IP, socket.IP_ADD_MEMBERSHIP, mreq)
         except BaseException as exc:
-            raise SmaConnectionException(
-                "Could not start multicast"
-            ) from exc
-
+            raise SmaConnectionException("Could not start multicast") from exc
 
         return True
 
-
     async def get_sensors(self) -> Sensors:
         """Get the sensors that are present on the device.
 
         Returns:
             Sensors: Sensors object containing Sensor objects
         """
         device_sensors = Sensors()
 
         for s in obis2sensor:
             if s.name is not None:
-                device_sensors.add(copy.copy(s)) 
+                device_sensors.add(copy.copy(s))
 
         return device_sensors
 
-
     async def close_session(self) -> None:
         """Close the session login."""
         self._sock.close()
 
     def _recv(self):
         return self._sock.recv(608)
 
-    def _getData(self):
+    def _get_data(self):
         """
 
         Hack:
             If the function is called less frequently than the device supplies data,
             the UDP packets will be stored in the buffer.
             If the read instruction (sock.recv) takes only milliseconds, I assume that
             the data came from the buffer and discard it. Otherwise outdated values would
@@ -173,17 +186,17 @@
         data = None
         tries = 50
         try:
             while tries > 0:
                 tries -= 1
                 a = datetime.datetime.now()
                 self._last_packet = self._recv()
-                data=self._decode(self._last_packet)
+                data = self._decode(self._last_packet)
                 b = datetime.datetime.now()
-                if data and (b-a).total_seconds() < 0.1:
+                if data and (b - a).total_seconds() < 0.1:
                     continue
                 if data:
                     break
         except TimeoutError as e:
             raise SmaConnectionException("No speedwire packet received!") from e
         if not data:
             raise SmaReadException("No usable data received!")
@@ -195,94 +208,102 @@
         Args:
             sensors (Sensors): Sensors object containing Sensor objects to read
 
         Returns:
             bool: reading was successful
         """
         notfound = []
-        data = self._getData()
-            
+        data = self._get_data()
+
         for sensor in sensors:
-          if (sensor.key in data):
-              value = data[sensor.key]
-              if (sensor.factor):
-                  value /= sensor.factor
-              sensor.value = value
-          else:
-              notfound.append(sensor.key)
+            if sensor.key in data:
+                value = data[sensor.key]
+                if sensor.factor:
+                    value /= sensor.factor
+                sensor.value = value
+            else:
+                notfound.append(sensor.key)
 
         if notfound:
             _LOGGER.info(
                 "No values for sensors: %s",
                 ",".join(notfound),
             )
 
         return True
 
-
     async def device_info(self) -> dict:
         """Read device info and return the results.
 
         Returns:
             dict: dict containing serial, name, type, manufacturer and sw_version
         """
-        data = self._getData()
+        data = self._get_data()
 
         device_info = {
             "serial": data["serial"],
             "name": data["device"],
             "type": data["susyid"],
             "manufacturer": "SMA",
             "sw_version": data["sw_version"],
         }
         return device_info
 
-    def _decode(self, p : bytes):
+    def _decode(self, p: bytes):
         """Decode a Speedwire-Packet
 
         Args:
             p: Network-Packet
 
         Returns:
             dict: Dict with all the decoded information
         """
         if p[0:4] != b"SMA\0":
             return None
-        protocolID = int.from_bytes(p[16:18], byteorder="big")
-        
-        if (protocolID not in [0x6069, 0x6081]):
-            _LOGGER.debug("Unknown protocoll " + str(protocolID))
+        protocol_id = int.from_bytes(p[16:18], byteorder="big")
+
+        if protocol_id not in [0x6069, 0x6081]:
+            _LOGGER.debug("Unknown protocoll %d", protocol_id)
             return None
-        
+
         data = {}
-        data["protocolID"] = protocolID
+        data["protocolID"] = protocol_id
         data["susyid"] = int.from_bytes(p[18:20], byteorder="big")
         data["device"] = self._susyid.get(data["susyid"], "unknown")
         data["serial"] = int.from_bytes(p[20:24], byteorder="big")
 
         length = int.from_bytes(p[12:14], byteorder="big") + 16
         pos = 28
         while pos < length:
             value = None
-            mchannel = int.from_bytes(p[pos: pos + 1], byteorder="big")
-            mvalueindex = int.from_bytes(p[pos + 1: pos + 2], byteorder="big")
-            mtyp = int.from_bytes(p[pos + 2: pos + 3], byteorder="big")
-            mtariff = int.from_bytes(p[pos + 3: pos + 4], byteorder="big")
-            obis = f'{mvalueindex}:{mtyp}:{mtariff}'
-            if mtyp in [4,8]:
+            mchannel = int.from_bytes(p[pos : pos + 1], byteorder="big")
+            mvalueindex = int.from_bytes(p[pos + 1 : pos + 2], byteorder="big")
+            mtyp = int.from_bytes(p[pos + 2 : pos + 3], byteorder="big")
+            mtariff = int.from_bytes(p[pos + 3 : pos + 4], byteorder="big")
+            obis = f"{mvalueindex}:{mtyp}:{mtariff}"
+            if mtyp in [4, 8]:
                 # 4 actucal / current => 8 Bytes
                 # 8 counter / sum => 12 Bytes
                 value = int.from_bytes(p[pos + 4 : pos + 4 + mtyp], byteorder="big")
                 pos += 4 + mtyp
             elif mchannel == 144 and mtyp == 0:
                 value = f"{p[pos + 4]}.{p[pos + 5]}.{p[pos + 6]}.{chr(p[pos + 7])}"
-                obis= "sw_version"
+                obis = "sw_version"
                 pos += 4 + 4
             else:
-                _LOGGER.debug("Unknown packet in speedwire: " + str(mchannel) + " " + str(mvalueindex) + " " + str(mtyp) + " " + str(mtariff))
+                _LOGGER.debug(
+                    "Unknown packet in speedwire: "
+                    + str(mchannel)
+                    + " "
+                    + str(mvalueindex)
+                    + " "
+                    + str(mtyp)
+                    + " "
+                    + str(mtariff)
+                )
                 pos += 4 + 4
             data[obis] = value
         return data
 
     async def get_debug(self) -> Dict:
         encoded = base64.b64encode(self._last_packet)
-        return { "packet": encoded.decode('ascii')}
+        return {"packet": encoded.decode("ascii")}
```

### Comparing `pysma_plus-0.2.4/pysmaplus/device_ennexos.py` & `pysma_plus-0.2.5/pysmaplus/device_ennexos.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,70 +1,75 @@
+"""
+
+Interface for SMA ennoxOS based devices. (e.g. Tripower X and maybe EV Charger)
+
+"""
+
 import asyncio
 import copy
 import json
 import logging
 from typing import Any, Dict, Optional
 
 
 from aiohttp import ClientSession, ClientTimeout, client_exceptions, hdrs
-from .sensor import Sensor
 from .const_webconnect import (
     DEFAULT_TIMEOUT,
 )
 from .exceptions import (
     SmaAuthenticationException,
     SmaConnectionException,
     SmaReadException,
 )
 from .sensor import Sensors
 from .device import Device
-from .const import Identifier
 from .definitions_ennexos import ennexosSensorProfiles
 from .const import SMATagList
 
 
 _LOGGER = logging.getLogger(__name__)
+
+
 class SMAennexos(Device):
     """Class to connect to the ennexos based SMA inverters. (e.g. Tripower X Devices)"""
 
     # pylint: disable=too-many-instance-attributes
     _aio_session: ClientSession
     _new_session_data: Optional[dict]
     _url: str
     _token: str
-    _authorization_header: str
+    _authorization_header: dict[str, str]
     _last_parameters: Any
     _last_measurements: Any
     _last_device: Any
     _device_info: Dict = None
-    _jsessionid: str = None    
+    _jsessionid: str = None
+
     def __init__(
         self,
         session: ClientSession,
         url: str,
         password: Optional[str],
         group: str,
     ):
         """Init SMA connection.
 
         Args:
             session (ClientSession): aiohttp client session
             url (str): Url or IP address of device
             password (str, optional): Password to use during login.
-            group (str, optional): Username to use during login. 
+            group (str, optional): Username to use during login.
 
         """
         self._url = url.rstrip("/")
         if not url.startswith("http"):
             self._url = "https://" + self._url
         self._new_session_data = {"user": group, "pass": password}
         self._aio_session = session
 
-
-
     async def _jsonrequest(
         self, url: str, parameters: Dict[str, Any], method: str = hdrs.METH_POST
     ) -> dict:
         """Request json data for requests.
 
         Args:
             url (str): URL to do request to
@@ -75,32 +80,27 @@
             SmaConnectionException: Connection to device failed
             SmaAuthenticationException: Authentication failed
 
         Returns:
             dict: json returned by device
         """
 
-        #_LOGGER.debug("Sending Request to %s: %s", url, parameters)
+        # _LOGGER.debug("Sending Request to %s: %s", url, parameters)
 
         try:
-                async with self._aio_session.request(
-                    method,
-                    url,
-                    timeout=ClientTimeout(total=DEFAULT_TIMEOUT),
-                    **parameters
-                ) as res:
-                    if (res.status == 401):
-                        raise SmaAuthenticationException(
-                            "Token failed!"
-                        )
-                    res = await res.json()
-                   # _LOGGER.debug("Received reply %s", res)
-                    return res
+            async with self._aio_session.request(
+                method, url, timeout=ClientTimeout(total=DEFAULT_TIMEOUT), **parameters
+            ) as res:
+                if res.status == 401:
+                    raise SmaAuthenticationException("Token failed!")
+                res = await res.json()
+                # _LOGGER.debug("Received reply %s", res)
+                return res
         except SmaAuthenticationException as e:
-                raise e
+            raise e
         except (client_exceptions.ContentTypeError, json.decoder.JSONDecodeError):
             _LOGGER.warning("Request to %s did not return a valid json.", url)
         except client_exceptions.ServerDisconnectedError as exc:
             raise SmaConnectionException(
                 f"Server at {self._url} disconnected."
             ) from exc
         except (
@@ -108,124 +108,117 @@
             asyncio.exceptions.TimeoutError,
         ) as exc:
             raise SmaConnectionException(
                 f"Could not connect to SMA at {self._url}: {exc}"
             ) from exc
         return {}
 
-
     async def new_session(self) -> bool:
         """Establish a new session.
 
         Returns:
             bool: authentication successful
         """
-        loginurl = self._url + '/api/v1/token'
-        postdata = {'data':{'grant_type': 'password',
-                'username': self._new_session_data["user"],
-                'password': self._new_session_data["pass"],
-                }}
-        ret = await self._jsonrequest(loginurl,postdata)
+        loginurl = self._url + "/api/v1/token"
+        postdata = {
+            "data": {
+                "grant_type": "password",
+                "username": self._new_session_data["user"],
+                "password": self._new_session_data["pass"],
+            }
+        }
+        ret = await self._jsonrequest(loginurl, postdata)
         if "access_token" not in ret:
             raise SmaAuthenticationException("Login failed!")
         self._token = ret["access_token"]
-#        self._refreshtoken = ret["refresh_token"]
-        self._authorization_header = { "Authorization" : "Bearer " + self._token,
-                                       "Content-Type": "application/json"
-                                       }
+        #        self._refreshtoken = ret["refresh_token"]
+        self._authorization_header = {
+            "Authorization": "Bearer " + self._token,
+            "Content-Type": "application/json",
+        }
         _LOGGER.debug("Login successfull")
         return True
 
     async def _get_parameter(self) -> Dict:
         """Get all parameters from the device
 
         Returns:
             Dict: Return a dict with all parameters
 
         """
-        url = self._url + '/api/v1/parameters/search'
+        url = self._url + "/api/v1/parameters/search"
         postdata = {
-             'data': '{"queryItems":[{"componentId":"IGULD:SELF"}]}',
-             'headers': self._authorization_header
+            "data": '{"queryItems":[{"componentId":"IGULD:SELF"}]}',
+            "headers": self._authorization_header,
         }
         ret = await self._jsonrequest(url, postdata)
         data = {}
-        if (len(ret) != 1):
-            _LOGGER.warning("Uncommon length of array in parameters request: %d", len(ret))
+        if len(ret) != 1:
+            _LOGGER.warning(
+                "Uncommon length of array in parameters request: %d", len(ret)
+            )
 
         for d in ret[0]["values"]:
-            dname = d["channelId"].replace("Parameter.","").replace("[]", "")
+            dname = d["channelId"].replace("Parameter.", "").replace("[]", "")
             if "value" in d:
                 v = d["value"]
-                data[dname] = {
-                        "name": dname,
-                        "value": v,
-                        "origname": d["channelId"]
-                    }
+                data[dname] = {"name": dname, "value": v, "origname": d["channelId"]}
             elif "values" in d:
                 # Split Value-Arrays
                 for idx in range(0, len(d["values"])):
                     v = d["values"][idx]
                     idxname = dname + "." + str(idx + 1)
                     data[idxname] = {
-                            "name": idxname,
-                            "value": v,
-                            "origname": d["channelId"]
+                        "name": idxname,
+                        "value": v,
+                        "origname": d["channelId"],
                     }
             else:
                 # Value current not available // night?
-                # TODO
                 pass
         return data
 
     async def _get_livedata(self) -> Dict:
         """Get the sensors reading from the device
 
         Returns:
             Dict: Return a dict with all measurements
 
         """
-        liveurl = self._url + '/api/v1/measurements/live'
-        postdata = { 
-             'data': '[{"componentId":"IGULD:SELF"}]',
-             'headers': self._authorization_header
+        liveurl = self._url + "/api/v1/measurements/live"
+        postdata = {
+            "data": '[{"componentId":"IGULD:SELF"}]',
+            "headers": self._authorization_header,
         }
-        ret = await self._jsonrequest(liveurl,postdata)
+        ret = await self._jsonrequest(liveurl, postdata)
         self._last_measurements = ret
         data = {}
         for d in ret:
-            dname = d["channelId"].replace("Measurement.","").replace("[]", "")
+            dname = d["channelId"].replace("Measurement.", "").replace("[]", "")
             if "value" in d["values"][0]:
                 v = d["values"][0]["value"]
                 if self._isfloat(v):
-                     v = round(v,2)
-                data[dname] = {
-                        "name": dname,
-                        "value": v,
-                        "origname": d["channelId"]
-                    }
+                    v = round(v, 2)
+                data[dname] = {"name": dname, "value": v, "origname": d["channelId"]}
             elif "values" in d["values"][0]:
                 # Split Value-Arrays
                 for idx in range(0, len(d["values"][0]["values"])):
                     v = d["values"][0]["values"][idx]
                     if self._isfloat(v):
-                        v = round(v,2)
+                        v = round(v, 2)
                     idxname = dname + "." + str(idx + 1)
                     data[idxname] = {
-                            "name": idxname,
-                            "value": v,
-                            "origname": d["channelId"]
+                        "name": idxname,
+                        "value": v,
+                        "origname": d["channelId"],
                     }
             else:
                 # Value current not available // night?
-                # TODO
                 pass
         return data
-    
-
 
     async def get_sensors(self) -> Sensors:
         """Get the sensors that are present on the device.
 
         Returns:
             Sensors: Sensors object containing Sensor objects
         """
@@ -235,56 +228,56 @@
         ret = await self._get_livedata()
         _LOGGER.debug("Found Sensors: %s", ret)
 
         device_sensors = Sensors()
         sensors = []
 
         # Search for matiching profile
-        for devname in ennexosSensorProfiles.keys():
-            if (self._device_info["name"].startswith(devname)):
-                sensors = ennexosSensorProfiles[devname]
-        if (len(sensors) == 0):
-            _LOGGER.warning(f'Unknown Device: {self._device_info["name"]} {self._device_info["type"]}')
-        
+        for dev in ennexosSensorProfiles.items():
+            if self._device_info["name"].startswith(dev[0]):
+                sensors = dev[1]
+        if len(sensors) == 0:
+            _LOGGER.warning(
+                f'Unknown Device: {self._device_info["name"]} {self._device_info["type"]}'
+            )
+
         # Add Sensors from profile
         for s in sensors:
-             if s.name:
-                 device_sensors.add(copy.copy(s))
+            if s.name:
+                device_sensors.add(copy.copy(s))
         return device_sensors
 
-
     async def close_session(self) -> None:
         pass
 
-    def _isfloat(self,num: Any):
+    def _isfloat(self, num: Any):
         """Test if num is a float
-            
+
             Tests for type float or a string with a dot is is float
-        
+
         Args:
             num: number to check
 
         Returns:
             bool: true, if num is from type float or a string with a dot
         """
         if isinstance(num, float):
             return True
         if isinstance(num, int):
             return False
         if not isinstance(num, str):
             raise TypeError("Value is not a string, float or int!")
-        if ("." not in num):
+        if "." not in num:
             return False
         try:
             float(num)
             return True
         except ValueError:
             return False
 
-
     async def read(self, sensors: Sensors) -> bool:
         """Read a set of keys.
 
         Args:
             sensors (Sensors): Sensors object containing Sensor objects to read
 
         Returns:
@@ -300,79 +293,76 @@
             await self.new_session()
             data = await self._get_livedata()
 
         for sen in sensors:
             if sen.enabled:
                 if sen.key in data:
                     value = data[sen.key]["value"]
-                    if (sen.mapper):
+                    if sen.mapper:
                         sen.mapped_value = sen.mapper.get(value, str(value))
-                    if (sen.factor and sen.factor != 1):
-                        value = round(value/sen.factor,4)
+                    if sen.factor and sen.factor != 1:
+                        value = round(value / sen.factor, 4)
                     sen.value = value
                     continue
                 notfound.append(f"{sen.name} [{sen.key}]")
 
         if notfound:
             _LOGGER.info(
                 "No values for sensors: %s",
                 ",".join(notfound),
             )
 
         return True
 
-
-
     async def device_info(self) -> dict:
         """Read device info and return the results.
 
         Returns:
             dict: dict containing serial, name, type, manufacturer and sw_version
         """
-        url = self._url + '/api/v1/plants/Plant:1/devices/IGULD:SELF'
-        requestdata = { 
-             'headers': self._authorization_header
-        }
-        dev = await self._jsonrequest(url,requestdata, hdrs.METH_GET)
+        url = self._url + "/api/v1/plants/Plant:1/devices/IGULD:SELF"
+        requestdata = {"headers": self._authorization_header}
+        dev = await self._jsonrequest(url, requestdata, hdrs.METH_GET)
         self._last_device = dev
         self._last_parameters = await self._get_parameter()
         _LOGGER.debug("Found Device: %s", dev)
         self._device_info = {
             "serial": dev["serial"],
             "name": dev["product"],
             "type": dev["name"],
             "manufacturer": dev["vendor"],
             "sw_version": dev["firmwareVersion"],
         }
         return self._device_info
 
     async def get_debug(self) -> Dict:
-        """ Collect all Debug Information """
+        """Collect all Debug Information"""
         return {
             "device": self._last_device,
             "measurements": self._last_measurements,
             "parameters": self._last_parameters,
-            "device_info": self._device_info
+            "device_info": self._device_info,
         }
 
     async def detect(self, ip):
         rets = []
         for prefix in ["https", "http"]:
             url = f"{prefix}://{ip}/api/v1/system/info"
             ret = (await super().detect(ip))[0]
             rets.append(ret)
             ret["testedEndpoints"] = url
             ret["remark"] = prefix
             try:
-                dev = await self._jsonrequest(url,{}, hdrs.METH_GET)
-                if ("productFriendlyNameTagId" in dev):
-                    fallback = "Unkown: "+ str(dev["productFriendlyNameTagId"])
-                    ret["device"] = SMATagList.get(dev["productFriendlyNameTagId"], fallback)
+                dev = await self._jsonrequest(url, {}, hdrs.METH_GET)
+                if "productFriendlyNameTagId" in dev:
+                    fallback = "Unkown: " + str(dev["productFriendlyNameTagId"])
+                    ret["device"] = SMATagList.get(
+                        dev["productFriendlyNameTagId"], fallback
+                    )
                     ret["status"] = "found"
                     break
-                else:
-                    ret["status"] = "failed"
-                    ret["exception"] = dev
+                ret["status"] = "failed"
+                ret["exception"] = dev
             except Exception as e:
                 ret["status"] = "failed"
                 ret["exception"] = e
         return rets
```

### Comparing `pysma_plus-0.2.4/pysmaplus/device_speedwire.py` & `pysma_plus-0.2.5/pysmaplus/device_speedwire.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,51 +1,53 @@
-# based on https://github.com/Wired-Square/sma-query/blob/main/src/sma_query_sw/protocol.py
+"""
+Implementation for SMA Speedwire
+
+Originally based on https://github.com/Wired-Square/sma-query/blob/main/src/sma_query_sw/commands.py
+Improved with Information from https://github.com/mhop/fhem-mirror/blob/master/fhem/FHEM/76_SMAInverter.pm
+Receiver classes completely reimplemented by little.yoda
+
+"""
 import logging
 import time
 import ctypes
 import binascii
 import copy
 import collections
 import struct
-
-from typing import Any, Dict, Optional,List
+import asyncio
+from typing import Any, Dict, Optional, List, Annotated
 from ctypes import LittleEndianStructure
-from asyncio import DatagramProtocol
+from asyncio import DatagramProtocol, Future
 
 from .helpers import version_int_to_string
-from .definitions_speedwire import commands
+from .definitions_speedwire import commands, responseDef, speedwireHeader, speedwireHeader6065
 
-from .sensor import Sensor
-from .const import Identifier
+from .sensor import Sensors, Sensor
+from .device import Device
 from .const import SMATagList
 
 from .exceptions import (
     SmaConnectionException,
     SmaReadException,
-    SmaAuthenticationException
+    SmaAuthenticationException,
 )
-from .sensor import Sensors
-from .device import Device
-import asyncio
+
 
 _LOGGER = logging.getLogger(__name__)
 
 APP_ID = 125
 ANY_SERIAL = 0xFFFFFFFF
 ANY_SUSYID = 0xFFFF
 
 # Login Timeout in seconds
 LOGIN_TIMEOUT = 900
 
-# Create a reverse index based command lookup
-ril_index = {f"ril-{value['first']:X}": value for (key, value) in commands.items() if "first" in value}
-
 
 def get_encoded_pw(password, installer=False):
-    # user=0x88, installer=0xBB
+    """Encodes the password"""
     byte_password = bytearray(password.encode("ascii"))
 
     if installer:
         login_code = 0xBB
     else:
         login_code = 0x88
 
@@ -57,505 +59,680 @@
         else:
             encodedpw[index] = login_code
 
     return encodedpw
 
 
 class SpeedwireFrame:
+    """Class for the send speedwire messages"""
+
     _frame_sequence = 1
     _id = (ctypes.c_ubyte * 4).from_buffer(bytearray(b"SMA\x00"))
     _tag0 = (ctypes.c_ubyte * 4).from_buffer(bytearray(b"\x00\x04\x02\xA0"))
     _group1 = (ctypes.c_ubyte * 4).from_buffer(bytearray(b"\x00\x00\x00\x01"))
     _eth_sig = (ctypes.c_ubyte * 4).from_buffer(bytearray(b"\x00\x10\x60\x65"))
     _ctrl2_1 = (ctypes.c_ubyte * 2).from_buffer(bytearray(b"\x00\x01"))
     _ctrl2_2 = (ctypes.c_ubyte * 2).from_buffer(bytearray(b"\x00\x01"))
 
     _data_length = 0  # Placeholder value
     _longwords = 0  # Placeholder value
     _ctrl = 0  # Placeholder value
 
     class FrameHeader(LittleEndianStructure):
+        """Frame Header"""
+
         _pack_ = 1
         _fields_ = [
             ("id", ctypes.c_ubyte * 4),
             ("tag0", ctypes.c_ubyte * 4),
             ("group1", ctypes.c_ubyte * 4),
             ("data_length", ctypes.c_uint16),
             ("eth_sig", ctypes.c_ubyte * 4),
             ("longwords", ctypes.c_ubyte),
             ("ctrl", ctypes.c_ubyte),
         ]
 
     class DataHeader(LittleEndianStructure):
+        # pylint: disable=too-few-public-methods
+        """Data header"""
         _pack_ = 1
         _fields_ = [
             ("dst_sysyid", ctypes.c_uint16),
             ("dst_serial", ctypes.c_uint32),
             ("ctrl2_1", ctypes.c_ubyte * 2),
             ("app_id", ctypes.c_uint16),
             ("app_serial", ctypes.c_uint32),
             ("ctrl2_2", ctypes.c_ubyte * 2),
             ("preamble", ctypes.c_uint32),
             ("sequence", ctypes.c_uint16),
         ]
 
     class LogoutFrame(LittleEndianStructure):
+        # pylint: disable=too-few-public-methods
+        """Logout"""
         _pack_ = 1
         _fields_ = [
             ("command", ctypes.c_uint32),
             ("data_start", ctypes.c_uint32),
             ("data_end", ctypes.c_uint32),
         ]
 
     class LoginFrame(LittleEndianStructure):
+        # pylint: disable=too-few-public-methods
+        """Login"""
         _pack_ = 1
         _fields_ = [
             ("command", ctypes.c_uint32),
             ("login_type", ctypes.c_uint32),
             ("timeout", ctypes.c_uint32),
             ("time", ctypes.c_uint32),
             ("data_start", ctypes.c_uint32),
             ("user_password", ctypes.c_ubyte * 12),
             ("data_end", ctypes.c_uint32),
         ]
 
     class QueryFrame(LittleEndianStructure):
+        # pylint: disable=too-few-public-methods
+        """Query Frame"""
+
         _pack_ = 1
         _fields_ = [
             ("command", ctypes.c_uint32),
             ("first", ctypes.c_uint32),
             ("last", ctypes.c_uint32),
-            ("data_end", ctypes.c_uint32)
+            ("data_end", ctypes.c_uint32),
         ]
 
-    def getLogoutFrame(self, inverter):
-        frame_header = self.getFrameHeader()
-        frame_data_header = self.getDataHeader(inverter)
-        frame_data = self.LogoutFrame()
+    # def getLogoutFrame(self, inverter):
+    #     frame_header = self.getFrameHeader()
+    #     frame_data_header = self.getDataHeader(inverter)
+    #     frame_data = self.LogoutFrame()
 
-        frame_header.ctrl = 0xA0
-        frame_data_header.dst_sysyid = 0xFFFF
-        frame_data_header.ctrl2_1 = (ctypes.c_ubyte * 2).from_buffer(bytearray(b"\x00\x03"))
-        frame_data_header.ctrl2_2 = (ctypes.c_ubyte * 2).from_buffer(bytearray(b"\x00\x03"))
+    #     frame_header.ctrl = 0xA0
+    #     frame_data_header.dst_sysyid = 0xFFFF
+    #     frame_data_header.ctrl2_1 = (ctypes.c_ubyte * 2).from_buffer(bytearray(b"\x00\x03"))
+    #     frame_data_header.ctrl2_2 = (ctypes.c_ubyte * 2).from_buffer(bytearray(b"\x00\x03"))
 
-        frame_data.command = commands["logoff"]["command"]
-        frame_data.data_start = 0xFFFFFFFF
-        frame_data.data_end = 0x00000000
+    #     frame_data.command = commands["logoff"]["command"]
+    #     frame_data.data_start = 0xFFFFFFFF
+    #     frame_data.data_end = 0x00000000
 
-        data_length = ctypes.sizeof(frame_data_header) + ctypes.sizeof(frame_data)
+    #     data_length = ctypes.sizeof(frame_data_header) + ctypes.sizeof(frame_data)
 
-        frame_header.data_length = int.from_bytes(data_length.to_bytes(2, "big"), "little")
+    #     frame_header.data_length = int.from_bytes(data_length.to_bytes(2, "big"), "little")
 
-        frame_header.longwords = (data_length // 4)
+    #     frame_header.longwords = (data_length // 4)
 
-        return bytes(frame_header) + bytes(frame_data_header) + bytes(frame_data)
+    #     return bytes(frame_header) + bytes(frame_data_header) + bytes(frame_data)
 
-    def getLoginFrame(self, inverter, installer):
+    def getLoginFrame(self, password, serial: int, installer: bool):
+        # pylint: disable=too-few-public-methods
+        """Returns a Login Frame"""
         frame_header = self.getFrameHeader()
-        frame_data_header = self.getDataHeader(inverter)
+        frame_data_header = self.getDataHeader(password, serial)
         frame_data = self.LoginFrame()
 
         frame_header.ctrl = 0xA0
         frame_data_header.dst_sysyid = 0xFFFF
-        frame_data_header.ctrl2_1 = (ctypes.c_ubyte * 2).from_buffer(bytearray(b"\x00\x01"))
-        frame_data_header.ctrl2_2 = (ctypes.c_ubyte * 2).from_buffer(bytearray(b"\x00\x01"))
+        frame_data_header.ctrl2_1 = (ctypes.c_ubyte * 2).from_buffer(
+            bytearray(b"\x00\x01")
+        )
+        frame_data_header.ctrl2_2 = (ctypes.c_ubyte * 2).from_buffer(
+            bytearray(b"\x00\x01")
+        )
 
         frame_data.command = commands["login"]["command"]
         frame_data.login_type = (0x07, 0x0A)[installer]
         frame_data.timeout = LOGIN_TIMEOUT
         frame_data.time = int(time.time())
         frame_data.data_start = 0x00000000  # Data Start
-        frame_data.user_password = (ctypes.c_ubyte * 12).from_buffer(get_encoded_pw(inverter["user_password"], installer))
-        frame_data.date_end = 0x00000000 # Packet End
+        frame_data.user_password = (ctypes.c_ubyte * 12).from_buffer(
+            get_encoded_pw(password, installer)
+        )
+        frame_data.date_end = 0x00000000  # Packet End
 
         data_length = ctypes.sizeof(frame_data_header) + ctypes.sizeof(frame_data)
 
-        frame_header.data_length = int.from_bytes(data_length.to_bytes(2, "big"), "little")
+        frame_header.data_length = int.from_bytes(
+            data_length.to_bytes(2, "big"), "little"
+        )
 
-        frame_header.longwords = (data_length // 4)
+        frame_header.longwords = data_length // 4
 
         return bytes(frame_header) + bytes(frame_data_header) + bytes(frame_data)
 
-    def getQueryFrame(self, inverter, command_name):
+    def getQueryFrame(self, password, serial: int, command_name: str):
+        """Return Query Frame"""
         frame_header = self.getFrameHeader()
-        frame_data_header = self.getDataHeader(inverter)
+        frame_data_header = self.getDataHeader(password, serial)
         frame_data = self.QueryFrame()
 
         command = commands[command_name]
 
         frame_header.ctrl = 0xA0
         frame_data_header.dst_sysyid = 0xFFFF
-        frame_data_header.ctrl2_1 = (ctypes.c_ubyte * 2).from_buffer(bytearray(b"\x00\x00"))
-        frame_data_header.ctrl2_2 = (ctypes.c_ubyte * 2).from_buffer(bytearray(b"\x00\x00"))
+        frame_data_header.ctrl2_1 = (ctypes.c_ubyte * 2).from_buffer(
+            bytearray(b"\x00\x00")
+        )
+        frame_data_header.ctrl2_2 = (ctypes.c_ubyte * 2).from_buffer(
+            bytearray(b"\x00\x00")
+        )
 
         frame_data.command = command["command"]
         frame_data.first = command["first"]
         frame_data.last = command["last"]
         frame_data.date_end = 0x00000000
 
         data_length = ctypes.sizeof(frame_data_header) + ctypes.sizeof(frame_data)
 
-        frame_header.data_length = int.from_bytes(data_length.to_bytes(2, "big"), "little")
+        frame_header.data_length = int.from_bytes(
+            data_length.to_bytes(2, "big"), "little"
+        )
 
-        frame_header.longwords = (data_length // 4)
+        frame_header.longwords = data_length // 4
 
         return bytes(frame_header) + bytes(frame_data_header) + bytes(frame_data)
 
     def getFrameHeader(self):
+        """Return Frame Header"""
         newFrameHeader = self.FrameHeader()
         newFrameHeader.id = self._id
         newFrameHeader.tag0 = self._tag0
         newFrameHeader.group1 = self._group1
         newFrameHeader.data_length = self._data_length
         newFrameHeader.eth_sig = self._eth_sig
         newFrameHeader.longwords = self._longwords
         newFrameHeader.ctrl = self._ctrl
 
         return newFrameHeader
 
-    def getDataHeader(self, inverter):
+    def getDataHeader(self, password, serial):
+        """Return Data Header"""
         newDataHeader = self.DataHeader()
 
         newDataHeader.dst_susyid = ANY_SUSYID
         newDataHeader.dst_serial = ANY_SERIAL
         newDataHeader.ctrl2_1 = self._ctrl2_1
         newDataHeader.app_id = APP_ID
-        newDataHeader.app_serial = (inverter["serial"])
+        newDataHeader.app_serial = serial
         newDataHeader.ctrl2_2 = self._ctrl2_2
         newDataHeader.preamble = 0
-        newDataHeader.sequence = (self._frame_sequence | 0x8000)
+        newDataHeader.sequence = self._frame_sequence | 0x8000
 
         self._frame_sequence += 1
 
         return newDataHeader
 
 
 class SMAClientProtocol(DatagramProtocol):
+    """Basic Class for communication"""
+
+    _commandFuture: Future[Any] = None
 
-    useDummyData = False
-    debug = {
-        "msg": collections.deque(maxlen=30),
+    debug: Dict[str, Any] = {
+        "msg": collections.deque(maxlen=len(commands) * 10),
         "data": {},
-        "unfinished": set()
+        "unfinished": set(),
+        "ids": set(),
+        "sendcounter": 0,
+        "resondcounter": 0,
+        "failedCounter": 0
     }
 
-    def __init__(self, inverter, on_connection_lost):
+    def __init__(self, password, on_connection_lost):
         self.speedwire = SpeedwireFrame()
         self.transport = None
-        self.inverter = inverter
+        self.password = password
         self.on_connection_lost = on_connection_lost
         self.cmds = []
         self.cmdidx = 0
         self.future = None
+        self.data_values = {}
+        self.sensors = {}
+        self._group = None
+        self._resendcounter = 0
+        self._failedCounter = 0
+        self._sendCounter = 0
 
         self.allCmds = []
         self.allCmds.extend(commands.keys())
         self.allCmds.remove("login")
         self.allCmds.remove("logoff")
 
     def connection_made(self, transport):
         self.transport = transport
 
-    def start_query(self, cmds: List, future, group: str):
-        self.cmds = cmds
+    async def controller(self):
+        try:
+            if self._resendcounter == 0:
+                self.debug["sendcounter"] += 1
+                self._sendCounter += 1
+
+            await asyncio.wait_for(self._commandFuture, timeout=0.5)
+            self.cmdidx += 1
+            self._resendcounter = 0
+        except asyncio.TimeoutError:
+            _LOGGER.debug(f"Timeout in command. Resendcounter: {self._resendcounter}")
+            self._resendcounter += 1
+            self.debug["resendcounter"] += 1
+            if (self._resendcounter > 2):
+                # Giving up. Next Command
+                _LOGGER.debug(f"Timeout in command")
+                self.cmdidx += 1
+                self._resendcounter = 0
+                self._failedCounter += 1
+                self.debug["failedcounter"] += 1
+
+        await self._send_next_command()
+
+
+    def _confirm_repsonse(self, code=-1):
+        if self._commandFuture.done():
+            _LOGGER.debug(f"unexpected message {code:08X}")
+            return
+        self._commandFuture.set_result(True)
+
+    async def start_query(self, cmds: List, future, group: str):
+        self.cmds = ["login"]
+        self.cmds.extend(cmds)
         self.future = future
         self.cmdidx = 0
-        self.inverter["data"] = {}
-        self.inverter["sensors"] = {}
-        _LOGGER.debug(f"""Sending login for {self.inverter["serial"]:#08X}""")
-        if self.useDummyData:
-            self.inverter["data"] = {}
-            self.inverter["sensors"] = {}
-            self.cmds = []
-            self._send_next_command()
-        else:
-            groupidx = ["user", "installer"].index(group)
-            self._send_command(self.speedwire.getLoginFrame(self.inverter, groupidx))
-    
+        self._failedCounter = 0
+        self._sendCounter = 0
+        self._group = group
+        self.data_values = {}
+        self.sensors = {}
+        _LOGGER.debug("Sending login")
+        self.debug["msg"].append(["SEND", "login"])
+        await self._send_next_command()
+
     def connection_lost(self, exc):
         _LOGGER.debug(f"Connection lost: {exc}")
         self.on_connection_lost.set_result(True)
 
     def _send_command(self, cmd):
-        _LOGGER.debug(f"Sending command [{len(cmd)}] -- {binascii.hexlify(cmd).upper()}")
+        """Send the Command"""
+        _LOGGER.debug(
+            f"Sending command [{len(cmd)}] -- {binascii.hexlify(cmd).upper()}"
+        )
+        self._commandFuture = asyncio.get_running_loop().create_future()
+        asyncio.get_running_loop().create_task(self.controller())
         self.transport.sendto(cmd)
 
-    def _get_code(self, data):
-        code = int.from_bytes(data[42:46], "little")
-        return code
-
-    def _get_ril(self, data):
-        code = int.from_bytes(data[54:58], "little")
-        return code & 0x00FFFF00
-
-    def _get_value(self, data, offset, format, invalid):
-        if format == "int":
-            format = "<l"
-        elif format == "uint":
-            format = "<L"
-        size = struct.calcsize(format)
-        if (size + offset >= len(data)):
-            return None
-        v = struct.unpack(format, data[offset:offset+size])[0]
-        if (v in [0x80000000, 0xFFFFFFFF, -0x80000000 ] or (invalid and invalid == v)):
-            v = None
-        return v
-
-    def _get_long_value(self, data, offset):
-         value = int.from_bytes(data[offset:offset + 4], "little")
-         return value
-
-    def _send_next_command(self):
+    async def _send_next_command(self):
+        """Send the next command in the list"""
         if not self.future:
             return
         if self.cmdidx >= len(self.cmds):
-            if self.useDummyData:
-                f = self.future
-                self.future = None
-                self.addDummyData()
-                self.future = f
-            self.debug["data"] = self.inverter["data"]
-            self.future.set_result(True)
+            # All commands send. Clean up.
+            f = self.future
+            self.future = None
+            await asyncio.sleep(0.1)  # Wait for delayed respones
+            self.debug["data"] = self.data_values
             self.cmds = []
             self.cmdidx = 0
-            self.future = None
+            f.set_result(True)
         else:
+            # Send the next command
             self.debug["msg"].append(["SEND", self.cmds[self.cmdidx]])
-            _LOGGER.debug("Sending "+ self.cmds[self.cmdidx])
-            self._send_command(self.speedwire.getQueryFrame(self.inverter,
-                                               self.cmds[self.cmdidx]))
-            self.cmdidx += 1
+            _LOGGER.debug("Sending " + self.cmds[self.cmdidx])
+            if (self.cmds[self.cmdidx]) == "login":
+                groupidx = ["user", "installer"].index(self._group)
+                self._send_command(
+                    self.speedwire.getLoginFrame(self.password, 0, groupidx)
+                )
+            else:
+                self._send_command(
+                    self.speedwire.getQueryFrame(
+                        self.password, 0, self.cmds[self.cmdidx]
+                    )
+                )
+
+    def _getFormat(self, handler):
+        """Return the necessary information for extracting the information"""
+        converter = None
+        format = handler.get("format", "")
+        if format == "int":
+            format = "<l"
+        elif format == "" or format == "uint":
+            format = "<L"
+        elif format == "version":
+            format = "<L"
+            converter = version_int_to_string
+        else:
+            raise ValueError(f"Unknown Format {format}")
+        size = struct.calcsize(format)
+        return (format, size, converter)
 
-    def _getvalue(self, register, data):
-            format = register.get("format", "uint")
-            value = None
-            if format == "list":
-                i = register.get("offset")
-                while (int.from_bytes(data[i:i+4], byteorder="little") != 0x00FFFFFE) and i+4 <= len(data):
-                        temp = int.from_bytes(data[i:i+4], byteorder="little")
-                        if (temp & 0xFF000000) == 0x01000000:
-                                value = temp & 0x00FFFFFF
-                        i += 4
-            elif format == "version":
-#                        value = self._get_value(data, register["offset"], format, register.get("invalid"))
-                value = self._get_long_value(data, register["offset"])
-                value = version_int_to_string(value)
+    def handle_login(self, msg):
+        """Is called if a login repsonse is received"""
+        _LOGGER.debug("Login repsonse received!")
+        self.sensors = {}
+        self.data_values = {"error": msg.error}
+        if msg.error == 256:
+            _LOGGER.error("Login failed!")
+            self.future.set_exception(
+                SmaAuthenticationException(
+                    "Login failed! Credentials wrong (user/install or password)"
+                )
+            )
+
+    def handle_newvalue(self, sensor: Sensor, value: Any):
+        """Set the new value to the sensor"""
+        if value is None:
+            return
+        sen = copy.copy(sensor)
+        if sen.factor and sen.factor != 1:
+            value /= sen.factor
+        sen.value = value
+        if sen.key in self.sensors:
+            oldValue = self.sensors[sen.key].value
+            if oldValue != value:
+                _LOGGER.warning(
+                    f"Overwriting sensors {sen.key} {sen.name} {oldValue} with new values {sen.value}"
+                )
+        self.sensors[sen.key] = sen
+        self.data_values[sen.key] = value
+
+    def extractvalues(self, handler: Dict, subdata):
+        (formatdef, size, converter) = self._getFormat(handler)
+        values = []
+        for idx in range(8, len(subdata), size):
+            v = struct.unpack(formatdef, subdata[idx : idx + size])[0]
+            if v in [0xFFFFFFFF, 0x80000000, 0xFFFFFFEC]:
+                v = None
             else:
-                if register["offset"] >= len(data):
-                    _LOGGER.debug(f'Value for {register["name"]} not found in this message type')
-                    return None
-                value = self._get_value(data, register["offset"], format, register.get("invalid"))
-                if value and register.get("mask"):
-                    value = value & register.get("mask")
-            return value
+                if converter:
+                    v = converter(v)
+                if "mask" in handler:
+                    v = v & handler["mask"]
+            values.append(v)
+        return values
+
+    def handle_register(self, subdata, register_idx: int):
+        """Handle the payload with all the registers"""
+        code = int.from_bytes(subdata[0:4], "little")
+        # c = f"{(code & 0xFFFFFFFF):08X}"
+        c = f"{code:08X}"
+        msec = int.from_bytes(subdata[4:8], "little")  # noqa: F841
+
+        # Fix for strange response codes
+        self.debug["ids"].add(c[6:])
+        if c.endswith("07"):
+            c = c[:7] + "1"
+
+        # Handle unknown Responses
+        if c not in responseDef:
+            values = []
+            valuesPos = []
+            for idx in range(8, len(subdata), 4):
+                v = struct.unpack("<l", subdata[idx : idx + 4])[0]
+                values.append(v)
+                valuesPos.append(f"{idx + 54}")
+            _LOGGER.warning(f"No Handler for {c}: {values} @ {valuesPos}")
+            self.debug["unfinished"].add(f"{c}")
+            return
 
+        # Handle known repsones
+        for handler in responseDef[c]:
+            values = self.extractvalues(handler, subdata)
+            if "sensor" not in handler:
+                continue
+            v = values[handler["idx"]]
+
+            sensor = handler["sensor"]
+
+            # Special handling for a response that returns two values under the same code
+            if isinstance(sensor, List):
+                if register_idx >= len(sensor):
+                    _LOGGER.warning(
+                        f"No Handler for {c} at register idx {register_idx}: {values}"
+                    )
+                    continue
+                _LOGGER.debug(
+                    f"Special Handler for {c} at register idx {register_idx}: {values}"
+                )
+                sensor = sensor[register_idx]
+            self.handle_newvalue(sensor, v)
+
+    # Unfortunately, there is no known method of determining the size of the registers
+    # from the message. Therefore, the register size is determined from the number of
+    # registers and the size of the payload.
+    def calc_register(self, data, msg: speedwireHeader6065):
+        cnt_registers = msg.lastRegister - msg.firstRegister + 1
+        size_datapayload = len(data) - 54 - 4
+        size_registers = (
+            size_datapayload // cnt_registers
+            if size_datapayload % cnt_registers == 0
+            else -1
+        )
+        return (cnt_registers, size_registers)
+
+    # Main routine for processing received messages.
     def datagram_received(self, data, addr):
-        code = self._get_code(data)
-        ril = self._get_ril(data)
-        ril_key = f"ril-{ril:X}"
-        shortcode = (f"{ril:X}")[0:4]
-
-        _LOGGER.debug(f"{addr} -- [{len(data)}] [{code:X}] [{ril:X}] -- {binascii.hexlify(data).upper()}")
-        self.debug["msg"].append(["RECV", len(data), (f"{ril:X}")[0:4], binascii.hexlify(data).upper().decode("utf-8")])
-
-        if code == commands["login"]["response"]:
-            _LOGGER.debug("Login repsonse received!")
-            self.inverter["data"] = {}
-            self.inverter["sensors"] = {}
-            for r in commands["login"]["registers"]:
-                value = self._getvalue(r, data)
-                self.inverter["data"][r['name']] = value
-            if (self.inverter["data"]["error"] == 256):
-                _LOGGER.error("Login failed!")
-                self.future.set_exception(SmaAuthenticationException("Login failed! Credentials wrong (user/install or password)"))
-
-        if len(data) <= 58:
-            _LOGGER.debug(f"Short datagram received: [{len(data)}] -- {data}")
-            self._send_next_command()
+        _LOGGER.debug(f"RECV: {addr} Len:{len(data)} {binascii.hexlify(data).upper()}")
+        self.debug["msg"].append(
+            ["RECV", len(data), binascii.hexlify(data).upper().decode("utf-8")]
+        )
+
+        # Check if message is a 6065 protocol
+        msg = speedwireHeader.from_packed(data[0:18])
+        if not msg.check6065():
+            _LOGGER.debug("Ignoring non 6065 Response. %d", msg.protokoll)
             return
-        
-        if ril_key not in ril_index:
-            shortcode = (f"{ril:X}")[0:4]
-            _LOGGER.debug(f"No Definition for {ril_key} {code:X} {shortcode}")
-            self.debug["unfinished"].add(f"No Definition for {ril_key} {code:X} {shortcode}")
-            self._send_next_command()
+
+        # If the requested information is not available, send the next command,
+        if len(data) < 58:
+            _LOGGER.debug(f"NACK [{len(data)}] -- {data}")
+            self._confirm_repsonse()
+            return
+
+        # Handle Login Responses
+        msg6065 = speedwireHeader6065.from_packed(data[18 : 18 + 36])
+        if msg6065.isLoginResponse():
+            self.handle_login(msg6065)
+            self._confirm_repsonse()
             return
-        
-        if ril_key in ril_index:
-            command = ril_index[ril_key]
-            short = f"{command['first']:#08X}"[2:6]
-            if "registers" in command:
-                if len(command["registers"]) == 0:
-                    self.debug["unfinished"].add(f"Command Response: {ril_key} {short} {code:X}")
-                    _LOGGER.error(f"Message but no registers definied. {command}")
-                for register in command["registers"]:
-                    value = self._getvalue(register, data)
-                    if value is not None:
-                        if "sensor" in register:
-                            sen = copy.copy(register["sensor"])
-                            v = value
-                            if (sen.factor and sen.factor != 1):
-                                v /= sen.factor
-                            sen.value = v
-                            self.inverter["sensors"][sen.key] = sen
-                        else:
-                             _LOGGER.debug(f'Value but no sensor: {register["name"]} {value}')
-                             pass
-                    self.inverter["data"][register["name"]] = value
-            else:
-                if self.useDummyData:
-                    _LOGGER.debug(f" {shortcode} [{len(data)}] [{code:X}] [{ril:X}]")
-                    print("======================================================================================================")
-                    print("======================================================================================================")
-                    raise RuntimeError()
-            self._send_next_command()
-
-    def addDummyData(self):
-        for pp in []:
-            self.datagram_received(bytes.fromhex(pp), ('10.10.10.10', 9522))
+
+
+        # Filter out non matching responses
+        (cnt_registers, size_registers) = self.calc_register(data, msg6065)
+        code = int.from_bytes(data[54:58], "little")
+        codem = code & 0x00FFFF00
+        if len(data) == 58 and codem == 0:
+            _LOGGER.debug(f"NACK [{len(data)}] -- {data}")
+            self._confirm_repsonse()
+            return
+        if size_registers <= 0 or size_registers not in [16, 28, 40]:
+            _LOGGER.warning(
+                f"Skipping message. --- Len {data} Ril {codem} {cnt_registers} x {size_registers} bytes"
+            )
+            self._confirm_repsonse(code)
+            return
+
+        # Extract the values for each register
+        for idx in range(0, cnt_registers):
+            start = idx * size_registers + 54
+            self.handle_register(data[start : start + size_registers], idx)
+
+        self._confirm_repsonse(code)
 
 
 class SMAspeedwireINV(Device):
+    """Adapter between Device-Class and SMAClientProtocol"""
 
     _transport = None
     _protocol = None
-    _deviceinfo = {}
+    _deviceinfo: Dict[str, Any] = {}
+    _debug: Dict[str, Any] = {
+        "overalltimeout": 0
+    }
 
-    def __init__(
-        self,
-        host: str,
-        group: str,
-        password: Optional[str]
-    ):
+    def __init__(self, host: str, group: str, password: Optional[str]):
         self._host = host
         self._group = group
+        self._password = password
         if group not in ["user", "installer"]:
             raise KeyError(f"Invalid user type: {group} (user or installer)")
 
-        self._inverter = {
-            "serial": 0,
-            "user_password": password,
-        }
-    #     self.check()
-
-    # def check(self) -> None:
-    #     keysname = {}
-    #     sensorname = {}
-    #     for x in commands.items():
-    #         if "registers" in x[1]:
-    #             for r in x[1]["registers"]:
-    #                 if "name" in r:
-    #                     name = r["name"]
-    #                     if (name in keysname):
-    #                         print("Doppelter Keyname " + name)
-    #                         raise RuntimeError("Doppelter Keyname " + name)
-    #                     keysname[name] = 1
-    #                 if "sensor" in r:
-    #                     sensor = r["sensor"]
-    #                     if (sensor.key in sensorname):
-    #                         print("Doppelter Sensorname " + sensor.key)
-    #                         raise RuntimeError("Doppelter Sensorname " + sensor.key)
+        self.check()
 
-    #                     sensorname[name] = 1
+    def check(self) -> None:
+        keysname = {}
+        sensorname = {}
+        for responses in responseDef.values():
+            for response in responses:
+                if "sensor" not in response or not isinstance(
+                    response["sensor"], Sensor
+                ):
+                    continue
+                sensor = response["sensor"]
+                if sensor.key in keysname:
+                    print("Doppelter SensorKey " + sensor.key)
+                    raise RuntimeError("Doppelter SensorKey " + sensor.key)
+                keysname[sensor.key] = 1
+                if sensor.name in sensorname:
+                    print("Doppelter SensorName " + sensor.name)
+                    raise RuntimeError("Doppelter Sensorname " + sensor.name)
+                sensorname[sensor.name] = 1
+
+        keysname = {}
+        sensorname = {}
+        for x in commands.items():
+            if "registers" not in x[1]:
+                continue
+            for r in x[1]["registers"]:
+                if "name" in r:
+                    name = r["name"]
+                    if name in keysname:
+                        print("Doppelter Keyname " + name)
+                        raise RuntimeError("Doppelter Keyname " + name)
+                    keysname[name] = 1
+                if "sensor" in r:
+                    sensor = r["sensor"]
+                    if isinstance(sensor, Sensor) and sensor.key in sensorname:
+                        print("Doppelter Sensorname " + sensor.key)
+                        raise RuntimeError("Doppelter Sensorname " + sensor.key)
+                    sensorname[name] = 1
 
-
-    async def get_sensors(self) -> Sensors:
-        fut = asyncio.get_running_loop().create_future()
-        c = self._protocol.allCmds
-        if self._protocol.useDummyData:
-            c = []
-        self._protocol.start_query(c, fut, self._group)
-        await asyncio.wait_for(fut, timeout=5)
-        device_sensors = Sensors()
-        for s in self._inverter["sensors"].values():
-            device_sensors.add(s)
-        return device_sensors
-    
     async def new_session(self) -> bool:
         loop = asyncio.get_running_loop()
         on_connection_lost = loop.create_future()
 
         self._transport, self._protocol = await loop.create_datagram_endpoint(
-             lambda: SMAClientProtocol(self._inverter, on_connection_lost), 
-             remote_addr=(self._host, 9522))
+            lambda: SMAClientProtocol(self._password, on_connection_lost),
+            remote_addr=(self._host, 9522),
+        )
+        # Test with device_info if the ip and user/pwd are correct
+        await self.device_info()
+        if (self._protocol._failedCounter >= self._protocol._sendCounter):
+            raise SmaConnectionException("No connection to device: %s:9522",self._host)
 
     async def device_info(self) -> dict:
         fut = asyncio.get_running_loop().create_future()
-        self._protocol.start_query(["TypeLabel", "Firmware"], fut, self._group)
+        await self._protocol.start_query(["TypeLabel", "Firmware"], fut, self._group)
         try:
             await asyncio.wait_for(fut, timeout=5)
         except TimeoutError:
+            self._debug["overalltimeout"] += 1
             _LOGGER.warning("Timeout in device_info")
-            if "error" in self._protocol.inverter["data"] and self._protocol.inverter["data"]["error"] == 0:
-                raise SmaReadException("Reply for request not received")
-            else:
-                raise SmaConnectionException("No connection to device")
-        print(self._protocol.inverter["data"])
-        data = self._inverter["data"]
+            if (
+                "error" in self._protocol.data_values
+                and self._protocol.data_values["error"] == 0
+            ):
+                raise SmaReadException(
+                    "Reply for request not received"
+                )  # Recheck Logic
+            raise SmaConnectionException("No connection to device")
+        data = self._protocol.data_values
 
-        invcnr = self._inverter["data"].get("inverter_class",0)
+        invcnr = data.get("inverter_class", 0)
         invc = SMATagList.get(invcnr, "Unknown device")
 
-        invtnr = self._inverter["data"].get("inverter_type",0)
+        invtnr = data.get("inverter_type", 0)
         invt = SMATagList.get(invtnr, "Unknown type")
         self._deviceinfo = {
             "serial": data.get("serial", ""),
             "name": str(invt) + " (" + str(invtnr) + ")",
             "type": str(invc) + " (" + str(invcnr) + ")",
             "manufacturer": "SMA",
-            "sw_version": data.get("Firmware",""),
+            "sw_version": data.get("Firmware", ""),
         }
         return self._deviceinfo
 
+    async def get_sensors(self) -> Sensors:
+        fut = asyncio.get_running_loop().create_future()
+        c = self._protocol.allCmds
+        device_sensors = Sensors()
+        try:
+            await self._protocol.start_query(c, fut, self._group)
+            await asyncio.wait_for(fut, timeout=5)
+            for s in self._protocol.sensors.values():
+                device_sensors.add(s)
+        except asyncio.TimeoutError as e:
+            self._debug["overalltimeout"] += 1
+            raise e
+        return device_sensors
+
 
     async def read(self, sensors: Sensors) -> bool:
         fut = asyncio.get_running_loop().create_future()
         c = self._protocol.allCmds
-        if self._protocol.useDummyData:
-            c = []
-        self._protocol.start_query(c, fut, self._group)
-        await asyncio.wait_for(fut, timeout=5)
-        sensorReadings = self._inverter["sensors"]
+        await self._protocol.start_query(c, fut, self._group)
+        try:
+            await asyncio.wait_for(fut, timeout=5)
+            self._update_sensors(sensors, self._protocol.sensors)
+            return True
+        except asyncio.TimeoutError as e:
+            self._debug["overalltimeout"] += 1
+            raise e
+
+    def _update_sensors(self, sensors, sensorReadings):
+        """Update a sensor with the sensor reading"""
+        _LOGGER.debug("Received %d sensor readings", len(sensorReadings))
         for sen in sensors:
-            if sen.enabled:
-                if sen.key in sensorReadings:
-                    value = sensorReadings[sen.key].value
-                    if (sen.mapper):
-                        sen.mapped_value = sen.mapper.get(value, str(value))
-                    sen.value = value
-
+            if sen.enabled and sen.key in sensorReadings:
+                value = sensorReadings[sen.key].value
+                if sen.mapper:
+                    sen.mapped_value = sen.mapper.get(value, str(value))
+                sen.value = value
 
     async def close_session(self) -> None:
         self._transport.close()
 
     async def get_debug(self) -> Dict:
-        return {
-            "msg": list(self._protocol.debug["msg"]),
-            "data": self._protocol.debug["data"],
-            "device_info": self._deviceinfo,
-            "unfinished": list(self._protocol.debug["unfinished"])
-       }
-
+        ret = self._protocol.debug.copy()
+        ret["unfinished"] = list(ret["unfinished"])
+        ret["msg"] = list(ret["msg"])
+        ret["ids"] = list(ret["ids"])
+        ret["device_info"] = self._deviceinfo
+        ret["overalltimeout"] = self._debug["overalltimeout"]
+        return ret
 
+    # wait for a response or a timeout
     async def detect(self, ip) -> bool:
         ret = await super().detect(ip)
         try:
             ret[0]["testedEndpoints"] = str(ip) + ":9522"
             await self.new_session()
             fut = asyncio.get_running_loop().create_future()
-            self._protocol.start_query(["TypeLabel"], fut, self._group)
+            await self._protocol.start_query(["TypeLabel"], fut, self._group)
             try:
                 await asyncio.wait_for(fut, timeout=5)
             except TimeoutError:
-                _LOGGER.warning("Timeout in device_info")
-            if "error" in self._protocol.inverter["data"] and self._protocol.inverter["data"]["error"] == 0:
-                raise SmaReadException("Reply for request not received")
-            else:
-                raise SmaConnectionException("No connection to device")
+                _LOGGER.warning("Timeout in detect")
+            if (
+                "error" in self._protocol.data_values
+                and self._protocol.dataValuess["error"] == 0
+            ):
+                raise SmaReadException(
+                    "Reply for request not received"
+                )  ## TODO recheck logic
+            raise SmaConnectionException("No connection to device")
         except SmaAuthenticationException as e:
             ret[0]["status"] = "maybe"
             ret[0]["exception"] = e
             ret[0]["remark"] = "only unencrypted Speedwire is supported"
         except Exception as e:
             ret[0]["status"] = "failed"
             ret[0]["exception"] = e
-        return ret
+        return ret
```

### Comparing `pysma_plus-0.2.4/pysmaplus/device_webconnect.py` & `pysma_plus-0.2.5/pysmaplus/device_webconnect.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 """SMA WebConnect library for Python.
 
 See: http://www.sma.de/en/products/monitoring-control/webconnect.html
 
 Source: http://www.github.com/kellerza/pysma
 """
+
 import asyncio
 import copy
 import json
 import logging
-from typing import Any, Dict, Optional
+from typing import Any, Dict, Optional, List
 
 import jmespath  # type: ignore
 from aiohttp import ClientSession, ClientTimeout, client_exceptions, hdrs
 from . import definitions_webconnect
 from .const_webconnect import (
     DEFAULT_LANG,
     DEFAULT_TIMEOUT,
@@ -35,14 +36,15 @@
     SmaAuthenticationException,
     SmaConnectionException,
     SmaReadException,
 )
 from .helpers import version_int_to_string
 from .sensor import Sensors
 from .device import Device
+
 _LOGGER = logging.getLogger(__name__)
 
 
 class SMAwebconnect(Device):
     """Class to connect to the SMA webconnect module and read parameters."""
 
     # pylint: disable=too-many-instance-attributes
@@ -92,15 +94,17 @@
             self._url = "http://" + self._url
         self._aio_session = session
         self._sid = None
         self._uid = uid
         self._lang = lang
         self._l10n = None
         self._devclass = None
-        self._device_info_sensors = Sensors(definitions_webconnect.sensor_map[DEVICE_INFO])
+        self._device_info_sensors = Sensors(
+            definitions_webconnect.sensor_map[DEVICE_INFO]
+        )
 
     async def _request_json(
         self, method: str, url: str, **kwargs: Dict[str, Any]
     ) -> dict:
         """Request json data for requests.
 
         Args:
@@ -442,15 +446,17 @@
             _LOGGER.debug(
                 "Energy Meter with serial %s detected. Adding extra sensors.",
                 em_sensor.value,
             )
             device_sensors.add(
                 [
                     sensor
-                    for sensor in definitions_webconnect.sensor_map[ENERGY_METER_VIA_INVERTER]
+                    for sensor in definitions_webconnect.sensor_map[
+                        ENERGY_METER_VIA_INVERTER
+                    ]
                     if sensor not in device_sensors
                 ]
             )
 
         _LOGGER.debug("Finding connected optimizers...")
         # Detect and add Optimizer Sensors
         optimizers = all_sensors.get(definitions_webconnect.optimizer_serial.key)
@@ -473,16 +479,15 @@
                         device_sensors.add(new_sensor)
 
         return device_sensors
 
     async def get_debug(self) -> Dict:
         return {}
 
-
-    async def detect(self, ip) -> bool:
+    async def detect(self, ip) -> List:
         results = []
         for urls in ["https://" + ip, "http://" + ip]:
             self._url = urls
             ret = await super().detect(ip)
             ret[0]["remark"] = urls
             try:
                 ret[0]["testedEndpoints"] = self._url
@@ -490,12 +495,12 @@
             except SmaAuthenticationException as e:
                 if self._sid:
                     ret[0]["status"] = "found"
                     ret[0]["exception"] = e
                 else:
                     ret[0]["status"] = "failed"
                     ret[0]["exception"] = e
-            except Exception as e:
+            except Exception as e:  # pylint: disable=broad-exception-caught
                 ret[0]["status"] = "failed"
                 ret[0]["exception"] = e
             results.extend(ret)
         return results
```

### Comparing `pysma_plus-0.2.4/pysmaplus/helpers.py` & `pysma_plus-0.2.5/pysmaplus/helpers.py`

 * *Files identical despite different names*

### Comparing `pysma_plus-0.2.4/pysmaplus/sensor.py` & `pysma_plus-0.2.5/pysmaplus/sensor.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Sensor classes for SMA WebConnect library for Python."""
+
 import copy
 import logging
 from typing import Any, Iterator, List, Optional, Union
 
 import attr
 import jmespath  # type: ignore
 
@@ -193,15 +194,15 @@
             for sss in sensor:
                 self.add(sss)
             return
 
         if isinstance(sensor, Sensor):
             sensor = copy.copy(sensor)
         else:
-            raise TypeError("pysma.Sensor expected")
+            raise TypeError(f"pysma.Sensor expected {type(sensor)} {sensor}")
 
         if sensor.name in self:
             old = self[sensor.name]
             self.__s.remove(old)
             _LOGGER.warning("Replacing sensor %s with %s", old, sensor)
 
         if sensor.key in self and self[sensor.key].key_idx == sensor.key_idx:
```

### Comparing `pysma_plus-0.2.4/setup.py` & `pysma_plus-0.2.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #!/usr/bin/env python
 """pysma library setup."""
 from pathlib import Path
 
 from setuptools import setup
 
-VERSION = "0.2.4"
+VERSION = "0.2.5"
 URL = "https://github.com/littleyoda/pysma"
 
 setup(
     name="pysma-plus",
     version=VERSION,
     description="Library to interface SMA Devices via WebConnect, EnnexOS and Energy Meter Devices",
     long_description=Path("README.md").read_text(),
```

### Comparing `pysma_plus-0.2.4/tests/__init__.py` & `pysma_plus-0.2.5/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `pysma_plus-0.2.4/tests/test_definitions.py` & `pysma_plus-0.2.5/tests/test_definitions.py`

 * *Files identical despite different names*

### Comparing `pysma_plus-0.2.4/tests/test_em.py` & `pysma_plus-0.2.5/tests/test_em.py`

 * *Files identical despite different names*

### Comparing `pysma_plus-0.2.4/tests/test_ennexos.py` & `pysma_plus-0.2.5/tests/test_ennexos.py`

 * *Files identical despite different names*

### Comparing `pysma_plus-0.2.4/tests/test_sensor.py` & `pysma_plus-0.2.5/tests/test_sensor.py`

 * *Files identical despite different names*

### Comparing `pysma_plus-0.2.4/tests/test_webconnect.py` & `pysma_plus-0.2.5/tests/test_webconnect.py`

 * *Files identical despite different names*

### Comparing `pysma_plus-0.2.4/tests/testdata/EVCharger-measurements.json` & `pysma_plus-0.2.5/tests/testdata/EVCharger-measurements.json`

 * *Files identical despite different names*

### Comparing `pysma_plus-0.2.4/tests/testdata/SunnyHomeManager2.json` & `pysma_plus-0.2.5/tests/testdata/SunnyHomeManager2.json`

 * *Files identical despite different names*

### Comparing `pysma_plus-0.2.4/tests/testdata/TripowerX15-deviceinfo.json` & `pysma_plus-0.2.5/tests/testdata/TripowerX15-deviceinfo.json`

 * *Files identical despite different names*

### Comparing `pysma_plus-0.2.4/tests/testdata/TripowerX15-measurements.json` & `pysma_plus-0.2.5/tests/testdata/TripowerX15-measurements.json`

 * *Files identical despite different names*

### Comparing `pysma_plus-0.2.4/tests/testdata/TripowerX15-parameters.json` & `pysma_plus-0.2.5/tests/testdata/TripowerX15-parameters.json`

 * *Files identical despite different names*

