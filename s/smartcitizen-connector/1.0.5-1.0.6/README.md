# Comparing `tmp/smartcitizen_connector-1.0.5.tar.gz` & `tmp/smartcitizen_connector-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "smartcitizen_connector-1.0.5.tar", last modified: Wed May 15 10:17:39 2024, max compression
+gzip compressed data, was "smartcitizen_connector-1.0.6.tar", last modified: Sat May 18 11:05:04 2024, max compression
```

## Comparing `smartcitizen_connector-1.0.5.tar` & `smartcitizen_connector-1.0.6.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 10:17:39.856537 smartcitizen_connector-1.0.5/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-15 10:17:35.000000 smartcitizen_connector-1.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-15 10:17:35.000000 smartcitizen_connector-1.0.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2970 2024-05-15 10:17:39.856537 smartcitizen_connector-1.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1473 2024-05-15 10:17:35.000000 smartcitizen_connector-1.0.5/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-05-15 10:17:39.856537 smartcitizen_connector-1.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1894 2024-05-15 10:17:35.000000 smartcitizen_connector-1.0.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 10:17:39.852537 smartcitizen_connector-1.0.5/smartcitizen_connector/
--rw-r--r--   0 runner    (1001) docker     (127)      504 2024-05-15 10:17:35.000000 smartcitizen_connector-1.0.5/smartcitizen_connector/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 10:17:39.856537 smartcitizen_connector-1.0.5/smartcitizen_connector/_config/
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-15 10:17:35.000000 smartcitizen_connector-1.0.5/smartcitizen_connector/_config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1216 2024-05-15 10:17:35.000000 smartcitizen_connector-1.0.5/smartcitizen_connector/_config/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 10:17:39.856537 smartcitizen_connector-1.0.5/smartcitizen_connector/device/
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-05-15 10:17:35.000000 smartcitizen_connector-1.0.5/smartcitizen_connector/device/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    24676 2024-05-15 10:17:35.000000 smartcitizen_connector-1.0.5/smartcitizen_connector/device/device.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 10:17:39.856537 smartcitizen_connector-1.0.5/smartcitizen_connector/measurement/
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-15 10:17:35.000000 smartcitizen_connector-1.0.5/smartcitizen_connector/measurement/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1155 2024-05-15 10:17:35.000000 smartcitizen_connector-1.0.5/smartcitizen_connector/measurement/measurement.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 10:17:39.856537 smartcitizen_connector-1.0.5/smartcitizen_connector/models/
--rw-r--r--   0 runner    (1001) docker     (127)      160 2024-05-15 10:17:35.000000 smartcitizen_connector-1.0.5/smartcitizen_connector/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3029 2024-05-15 10:17:35.000000 smartcitizen_connector-1.0.5/smartcitizen_connector/models/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 10:17:39.856537 smartcitizen_connector-1.0.5/smartcitizen_connector/search/
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-15 10:17:35.000000 smartcitizen_connector-1.0.5/smartcitizen_connector/search/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4605 2024-05-15 10:17:35.000000 smartcitizen_connector-1.0.5/smartcitizen_connector/search/search.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 10:17:39.856537 smartcitizen_connector-1.0.5/smartcitizen_connector/sensor/
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-15 10:17:35.000000 smartcitizen_connector-1.0.5/smartcitizen_connector/sensor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-05-15 10:17:35.000000 smartcitizen_connector-1.0.5/smartcitizen_connector/sensor/sensor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 10:17:39.856537 smartcitizen_connector-1.0.5/smartcitizen_connector/tools/
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-15 10:17:35.000000 smartcitizen_connector-1.0.5/smartcitizen_connector/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8620 2024-05-15 10:17:35.000000 smartcitizen_connector-1.0.5/smartcitizen_connector/tools/tools.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 10:17:39.856537 smartcitizen_connector-1.0.5/smartcitizen_connector.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2970 2024-05-15 10:17:39.000000 smartcitizen_connector-1.0.5/smartcitizen_connector.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      945 2024-05-15 10:17:39.000000 smartcitizen_connector-1.0.5/smartcitizen_connector.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 10:17:39.000000 smartcitizen_connector-1.0.5/smartcitizen_connector.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 10:17:39.000000 smartcitizen_connector-1.0.5/smartcitizen_connector.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-05-15 10:17:39.000000 smartcitizen_connector-1.0.5/smartcitizen_connector.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-15 10:17:39.000000 smartcitizen_connector-1.0.5/smartcitizen_connector.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 11:05:04.855455 smartcitizen_connector-1.0.6/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-18 11:05:00.000000 smartcitizen_connector-1.0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-18 11:05:00.000000 smartcitizen_connector-1.0.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2970 2024-05-18 11:05:04.855455 smartcitizen_connector-1.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1473 2024-05-18 11:05:00.000000 smartcitizen_connector-1.0.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-05-18 11:05:04.855455 smartcitizen_connector-1.0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1894 2024-05-18 11:05:00.000000 smartcitizen_connector-1.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 11:05:04.851456 smartcitizen_connector-1.0.6/smartcitizen_connector/
+-rw-r--r--   0 runner    (1001) docker     (127)      504 2024-05-18 11:05:00.000000 smartcitizen_connector-1.0.6/smartcitizen_connector/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 11:05:04.851456 smartcitizen_connector-1.0.6/smartcitizen_connector/_config/
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-18 11:05:00.000000 smartcitizen_connector-1.0.6/smartcitizen_connector/_config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1216 2024-05-18 11:05:00.000000 smartcitizen_connector-1.0.6/smartcitizen_connector/_config/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 11:05:04.851456 smartcitizen_connector-1.0.6/smartcitizen_connector/device/
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-05-18 11:05:00.000000 smartcitizen_connector-1.0.6/smartcitizen_connector/device/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24662 2024-05-18 11:05:00.000000 smartcitizen_connector-1.0.6/smartcitizen_connector/device/device.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 11:05:04.851456 smartcitizen_connector-1.0.6/smartcitizen_connector/measurement/
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-18 11:05:00.000000 smartcitizen_connector-1.0.6/smartcitizen_connector/measurement/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1155 2024-05-18 11:05:00.000000 smartcitizen_connector-1.0.6/smartcitizen_connector/measurement/measurement.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 11:05:04.855455 smartcitizen_connector-1.0.6/smartcitizen_connector/models/
+-rw-r--r--   0 runner    (1001) docker     (127)      160 2024-05-18 11:05:00.000000 smartcitizen_connector-1.0.6/smartcitizen_connector/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3029 2024-05-18 11:05:00.000000 smartcitizen_connector-1.0.6/smartcitizen_connector/models/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 11:05:04.855455 smartcitizen_connector-1.0.6/smartcitizen_connector/search/
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-18 11:05:00.000000 smartcitizen_connector-1.0.6/smartcitizen_connector/search/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4605 2024-05-18 11:05:00.000000 smartcitizen_connector-1.0.6/smartcitizen_connector/search/search.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 11:05:04.855455 smartcitizen_connector-1.0.6/smartcitizen_connector/sensor/
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-18 11:05:00.000000 smartcitizen_connector-1.0.6/smartcitizen_connector/sensor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-05-18 11:05:00.000000 smartcitizen_connector-1.0.6/smartcitizen_connector/sensor/sensor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 11:05:04.855455 smartcitizen_connector-1.0.6/smartcitizen_connector/tools/
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-18 11:05:00.000000 smartcitizen_connector-1.0.6/smartcitizen_connector/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8632 2024-05-18 11:05:00.000000 smartcitizen_connector-1.0.6/smartcitizen_connector/tools/tools.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 11:05:04.855455 smartcitizen_connector-1.0.6/smartcitizen_connector.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2970 2024-05-18 11:05:04.000000 smartcitizen_connector-1.0.6/smartcitizen_connector.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      945 2024-05-18 11:05:04.000000 smartcitizen_connector-1.0.6/smartcitizen_connector.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-18 11:05:04.000000 smartcitizen_connector-1.0.6/smartcitizen_connector.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-18 11:05:04.000000 smartcitizen_connector-1.0.6/smartcitizen_connector.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-05-18 11:05:04.000000 smartcitizen_connector-1.0.6/smartcitizen_connector.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-18 11:05:04.000000 smartcitizen_connector-1.0.6/smartcitizen_connector.egg-info/top_level.txt
```

### Comparing `smartcitizen_connector-1.0.5/LICENSE` & `smartcitizen_connector-1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `smartcitizen_connector-1.0.5/PKG-INFO` & `smartcitizen_connector-1.0.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smartcitizen-connector
-Version: 1.0.5
+Version: 1.0.6
 Summary: Python connector to download information collected in SmartCitizen API
 Home-page: https://github.com/fablabbcn/smartcitizen-connector
 Author: oscgonfer
 License: GNU General Public License v3
 Project-URL: Documentation, https://docs.smartcitizen.me/
 Project-URL: Source Code, https://github.com/fablabbcn/smartcitizen-connector
 Keywords: sensors,Smart Citizen
```

### Comparing `smartcitizen_connector-1.0.5/README.md` & `smartcitizen_connector-1.0.6/README.md`

 * *Files identical despite different names*

### Comparing `smartcitizen_connector-1.0.5/setup.py` & `smartcitizen_connector-1.0.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 PROJECT_URLS = {
     "Documentation": "https://docs.smartcitizen.me/",
     "Source Code": "https://github.com/fablabbcn/smartcitizen-connector",
 }
 
 setup(
     name="smartcitizen-connector",
-    version="1.0.5",
+    version="1.0.6",
     description="Python connector to download information collected in SmartCitizen API",
     author="oscgonfer",
     license="GNU General Public License v3",
     keywords=['sensors', 'Smart Citizen'],
     long_description = open('README.md').read(),
     long_description_content_type="text/markdown",
     url="https://github.com/fablabbcn/smartcitizen-connector",
```

### Comparing `smartcitizen_connector-1.0.5/smartcitizen_connector/_config/config.py` & `smartcitizen_connector-1.0.6/smartcitizen_connector/_config/config.py`

 * *Files identical despite different names*

### Comparing `smartcitizen_connector-1.0.5/smartcitizen_connector/device/device.py` & `smartcitizen_connector-1.0.6/smartcitizen_connector/device/device.py`

 * *Files 1% similar despite different names*

```diff
@@ -54,15 +54,15 @@
 
     # Check the url in hardware
     urls = url_checker(_postprocessing.hardware_url)
     # If URL is empty, try prepending base url from config
     if not urls:
         tentative_url = f"{config.BASE_POSTPROCESSING_URL}hardware/{_postprocessing.hardware_url}.json"
     else:
-        if len(urls)>1: logger('URLs for postprocessing recipe are more than one, trying first', 'WARNING')
+        if len(urls)>1: logger.warning('URLs for postprocessing recipe are more than one, trying first')
         tentative_url = urls[0]
 
     logger.info(f'Device has postprocessing information:\n{_postprocessing}')
 
     _ok = True
     # Make hardware postprocessing
     if url_checker(tentative_url):
@@ -281,15 +281,15 @@
             if max_date > self.json.last_reading_at:
                 logger.warning('Trimming max_date to last reading')
                 max_date = self.json.last_reading_at
 
         logger.info(f'Device {self.id} timezone: {self.timezone}')
 
         if not self.json.data.sensors:
-            logger.info(f'Device {self.id} is empty', 'WARNING')
+            logger.info(f'Device {self.id} is empty')
             return self.data
         else: logger.info(f"Sensor IDs: {[f'{sensor.name}: {sensor.id}' for sensor in self.json.data.sensors]}")
 
         df = DataFrame()
         logger.info(f'Requesting device {self.id} from {min_date} to {max_date}')
 
         semaphore = asyncio.Semaphore(config._max_concurrent_requests)
```

### Comparing `smartcitizen_connector-1.0.5/smartcitizen_connector/measurement/measurement.py` & `smartcitizen_connector-1.0.6/smartcitizen_connector/measurement/measurement.py`

 * *Files identical despite different names*

### Comparing `smartcitizen_connector-1.0.5/smartcitizen_connector/models/models.py` & `smartcitizen_connector-1.0.6/smartcitizen_connector/models/models.py`

 * *Files identical despite different names*

### Comparing `smartcitizen_connector-1.0.5/smartcitizen_connector/search/search.py` & `smartcitizen_connector-1.0.6/smartcitizen_connector/search/search.py`

 * *Files identical despite different names*

### Comparing `smartcitizen_connector-1.0.5/smartcitizen_connector/sensor/sensor.py` & `smartcitizen_connector-1.0.6/smartcitizen_connector/sensor/sensor.py`

 * *Files identical despite different names*

### Comparing `smartcitizen_connector-1.0.5/smartcitizen_connector/tools/tools.py` & `smartcitizen_connector-1.0.6/smartcitizen_connector/tools/tools.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 from typing import Optional
 from termcolor import colored
 from requests.exceptions import HTTPError
 from requests import get
 import re
 import logging
 import sys
+import time
 
 tf = TimezoneFinder()
 
 freq_2_rollup_lut = (
     ['A', 'y'],
     ['M', 'M'],
     ['W', 'w'],
```

### Comparing `smartcitizen_connector-1.0.5/smartcitizen_connector.egg-info/PKG-INFO` & `smartcitizen_connector-1.0.6/smartcitizen_connector.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smartcitizen-connector
-Version: 1.0.5
+Version: 1.0.6
 Summary: Python connector to download information collected in SmartCitizen API
 Home-page: https://github.com/fablabbcn/smartcitizen-connector
 Author: oscgonfer
 License: GNU General Public License v3
 Project-URL: Documentation, https://docs.smartcitizen.me/
 Project-URL: Source Code, https://github.com/fablabbcn/smartcitizen-connector
 Keywords: sensors,Smart Citizen
```

### Comparing `smartcitizen_connector-1.0.5/smartcitizen_connector.egg-info/SOURCES.txt` & `smartcitizen_connector-1.0.6/smartcitizen_connector.egg-info/SOURCES.txt`

 * *Files identical despite different names*

