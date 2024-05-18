# Comparing `tmp/euc2mqtt-0.0.0.tar.gz` & `tmp/euc2mqtt-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "euc2mqtt-0.0.0.tar", last modified: Sun Apr 28 17:19:47 2024, max compression
+gzip compressed data, was "euc2mqtt-0.0.2.tar", last modified: Sat May 18 21:18:05 2024, max compression
```

## Comparing `euc2mqtt-0.0.0.tar` & `euc2mqtt-0.0.2.tar`

### file list

```diff
@@ -1,23 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 17:19:47.783068 euc2mqtt-0.0.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-04-28 17:19:43.000000 euc2mqtt-0.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3101 2024-04-28 17:19:47.783068 euc2mqtt-0.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      859 2024-04-28 17:19:43.000000 euc2mqtt-0.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1287 2024-04-28 17:19:43.000000 euc2mqtt-0.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-28 17:19:47.783068 euc2mqtt-0.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      215 2024-04-28 17:19:43.000000 euc2mqtt-0.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 17:19:47.779068 euc2mqtt-0.0.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 17:19:47.779068 euc2mqtt-0.0.0/src/euc2mqtt/
--rw-r--r--   0 runner    (1001) docker     (127)     3319 2024-04-28 17:19:43.000000 euc2mqtt-0.0.0/src/euc2mqtt/CLI.py
--rw-r--r--   0 runner    (1001) docker     (127)     3132 2024-04-28 17:19:43.000000 euc2mqtt-0.0.0/src/euc2mqtt/EatonAPI.py
--rw-r--r--   0 runner    (1001) docker     (127)     5078 2024-04-28 17:19:43.000000 euc2mqtt-0.0.0/src/euc2mqtt/HassioAPI.py
--rw-r--r--   0 runner    (1001) docker     (127)     3815 2024-04-28 17:19:43.000000 euc2mqtt-0.0.0/src/euc2mqtt/InteropE2H.py
--rw-r--r--   0 runner    (1001) docker     (127)      105 2024-04-28 17:19:43.000000 euc2mqtt-0.0.0/src/euc2mqtt/Utility.py
--rw-r--r--   0 runner    (1001) docker     (127)     4309 2024-04-28 17:19:43.000000 euc2mqtt-0.0.0/src/euc2mqtt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-04-28 17:19:43.000000 euc2mqtt-0.0.0/src/euc2mqtt/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 17:19:47.783068 euc2mqtt-0.0.0/src/euc2mqtt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3101 2024-04-28 17:19:47.000000 euc2mqtt-0.0.0/src/euc2mqtt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      431 2024-04-28 17:19:47.000000 euc2mqtt-0.0.0/src/euc2mqtt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-28 17:19:47.000000 euc2mqtt-0.0.0/src/euc2mqtt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-28 17:19:47.000000 euc2mqtt-0.0.0/src/euc2mqtt.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-28 17:19:47.000000 euc2mqtt-0.0.0/src/euc2mqtt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-28 17:19:47.000000 euc2mqtt-0.0.0/src/euc2mqtt.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 21:18:05.846962 euc2mqtt-0.0.2/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 21:18:05.842961 euc2mqtt-0.0.2/.devcontainer/
+-rw-r--r--   0 runner    (1001) docker     (127)     1199 2024-05-18 21:17:54.000000 euc2mqtt-0.0.2/.devcontainer/devcontainer.json
+-rw-r--r--   0 runner    (1001) docker     (127)      643 2024-05-18 21:17:54.000000 euc2mqtt-0.0.2/.devcontainer/docker-compose.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 21:18:05.842961 euc2mqtt-0.0.2/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      467 2024-05-18 21:17:54.000000 euc2mqtt-0.0.2/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 21:18:05.842961 euc2mqtt-0.0.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      733 2024-05-18 21:17:54.000000 euc2mqtt-0.0.2/.github/workflows/build-win.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      628 2024-05-18 21:17:54.000000 euc2mqtt-0.0.2/.github/workflows/publish-pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3095 2024-05-18 21:17:54.000000 euc2mqtt-0.0.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-05-18 21:17:54.000000 euc2mqtt-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5357 2024-05-18 21:18:05.846962 euc2mqtt-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3114 2024-05-18 21:17:54.000000 euc2mqtt-0.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-05-18 21:17:54.000000 euc2mqtt-0.0.2/build.bat
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-18 21:17:54.000000 euc2mqtt-0.0.2/entry_point.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1286 2024-05-18 21:17:54.000000 euc2mqtt-0.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)    42774 2024-05-18 21:17:54.000000 euc2mqtt-0.0.2/scr.png
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-18 21:18:05.846962 euc2mqtt-0.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      215 2024-05-18 21:17:54.000000 euc2mqtt-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 21:18:05.842961 euc2mqtt-0.0.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 21:18:05.842961 euc2mqtt-0.0.2/src/euc2mqtt/
+-rw-r--r--   0 runner    (1001) docker     (127)     3804 2024-05-18 21:17:54.000000 euc2mqtt-0.0.2/src/euc2mqtt/CLI.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3132 2024-05-18 21:17:54.000000 euc2mqtt-0.0.2/src/euc2mqtt/EatonAPI.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5105 2024-05-18 21:17:54.000000 euc2mqtt-0.0.2/src/euc2mqtt/HassioAPI.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3815 2024-05-18 21:17:54.000000 euc2mqtt-0.0.2/src/euc2mqtt/InteropE2H.py
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-05-18 21:17:54.000000 euc2mqtt-0.0.2/src/euc2mqtt/Utility.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4358 2024-05-18 21:17:54.000000 euc2mqtt-0.0.2/src/euc2mqtt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-05-18 21:17:54.000000 euc2mqtt-0.0.2/src/euc2mqtt/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 21:18:05.846962 euc2mqtt-0.0.2/src/euc2mqtt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5357 2024-05-18 21:18:05.000000 euc2mqtt-0.0.2/src/euc2mqtt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      630 2024-05-18 21:18:05.000000 euc2mqtt-0.0.2/src/euc2mqtt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-18 21:18:05.000000 euc2mqtt-0.0.2/src/euc2mqtt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-18 21:18:05.000000 euc2mqtt-0.0.2/src/euc2mqtt.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-05-18 21:18:05.000000 euc2mqtt-0.0.2/src/euc2mqtt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-18 21:18:05.000000 euc2mqtt-0.0.2/src/euc2mqtt.egg-info/top_level.txt
```

### Comparing `euc2mqtt-0.0.0/LICENSE` & `euc2mqtt-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `euc2mqtt-0.0.0/PKG-INFO` & `euc2mqtt-0.0.2/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,70 +1,75 @@
-Metadata-Version: 2.1
-Name: euc2mqtt
-Version: 0.0.0
-Summary: Eaton UPS Companion to MQTT Publisher
-Author: islandc_
-License: MIT License
-        
-        Copyright (c) 2024 islandc_
-        
-        Permission is hereby granted, free of charge, to any person obtaining a copy
-        of this software and associated documentation files (the "Software"), to deal
-        in the Software without restriction, including without limitation the rights
-        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-        copies of the Software, and to permit persons to whom the Software is
-        furnished to do so, subject to the following conditions:
-        
-        The above copyright notice and this permission notice shall be included in all
-        copies or substantial portions of the Software.
-        
-        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-        SOFTWARE.
-        
-Project-URL: Repository, https://github.com/islandcontroller/euc2mqtt.git
-Project-URL: Issues, https://github.com/islandcontroller/euc2mqtt/issues/
-Project-URL: Documentation, https://github.com/islandcontroller/euc2mqtt/wiki/
-Keywords: eaton,ups,mqtt
-Classifier: Development Status :: 3 - Alpha
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.12
-Classifier: Topic :: Communications
-Requires-Python: >=3.12
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: paho-mqtt>=2.0.0
-Requires-Dist: requests>=2.31.0
-Provides-Extra: test
-Requires-Dist: pytest>=8.1; extra == "test"
-Requires-Dist: pytest-cov>=4.1; extra == "test"
-Requires-Dist: responses>=0.25; extra == "test"
-Requires-Dist: ruff>=0.3; extra == "test"
-
 # euc2mqtt
 
 [![License](https://img.shields.io/github/license/islandcontroller/euc2mqtt)](LICENSE) ![PyPI - Version](https://img.shields.io/pypi/v/euc2mqtt)
 
 A tool for publishing status data from a local Eaton UPS Companion service to Homeassistant.
 
-## Installation
+<p align="center"><img src="scr.png"/></p>
 
-A pre-built package is hosted on [PyPI](https://pypi.org/project/euc2mqtt/) and can be installed and updated using the [`pip`](https://pip.pypa.io/en/stable/getting-started/) utility:
+## Quick Start
 
-    pip install -U euc2mqtt
+The following quick start guide should get you up and running from a blank Homeassistant installation. Feel free to skip a step if your system is already configured.
 
-Windows binaries are provided on the [GitHub Releases](https://github.com/islandcontroller/euc2mqtt/releases) page.
+### Install mosquitto
 
+1. In Homeassistant, navigate to *Settings*, *Add-ons*
+2. Click the *Add-on store* button
+3. Search for *Mosquitto broker* and select the result
+4. Click on *Install*
 
-## Usage
+### Create a new Homeassistant user for data ingest
 
-    python -m euc2mqtt --mqtt <broker hostname> --username <user> --password <password>
+As mosquitto requires authentication, I heavily suggest creating a new user for data ingest.
+
+1. In Homeassistant, navigate to *Settings*, *People*
+2. Click on *Add person*, input a user name
+3. Check *Allow person to log in*
+4. Enter all required fields
+5. Check *Can only log in from local network*
+
+### Get the application
+
+Windows binaries are provided on the [GitHub Releases](https://github.com/islandcontroller/euc2mqtt/releases) page.**
+
+If you prefer to use your own Python insallation, a pre-built package is hosted on [PyPI](https://pypi.org/project/euc2mqtt/) and can be installed and updated using the [`pip`](https://pip.pypa.io/en/stable/getting-started/) utility:
+
+    pip install -U euc2mqtt
+
+### Run it!
 
 > [!NOTE]
 > This tool needs to run on the same host as Eaton UPS Companion, as EUC in its default configuration only accepts connections on `localhost:4679`.
 
+Open a terminal and run the tool, providing the broker hostname (your Homeassistant hostname), username and the password!
+
+*Option 1: Standalone application*
+
+    .\euc2mqtt --mqtt <broker hostname> --username <user> --password <password>
+
+*Option 2: Run as Python module*
+
+    python -m euc2mqtt --mqtt <broker hostname> --username <user> --password <password>
+
+### More info
+
+A more in-depth description of available command line parameters can be viewed by appending `-h` at the end of your input. For example:
+
+```
+> .\euc2mqtt -h
+
+usage: euc2mqtt [-h] [--name NAME] [--mqtt MQTT] [--euc EUC] [--username USERNAME] [--password PASSWORD] [--interval INTERVAL] [--full-update FULL_UPDATE] [--logfile LOGFILE] [--verbose]
+
+MQTT Publisher for Eaton UPS Companion status messages to Home Assistant. See https://github.com/islandcontroller/euc2mqtt for more info!
+
+options:
+  -h, --help            show this help message and exit
+  --name NAME           Device name
+  --mqtt MQTT           MQTT broker hostname and port (hostname[:port])
+  --euc EUC             Eaton UPS Companion hostname and port (hostname[:port])
+  --username USERNAME   Username for MQTT broker authentication
+  --password PASSWORD   Password for MQTT broker authentication
+  --interval INTERVAL   Update interval in seconds
+  --full-update FULL_UPDATE
+                        Number of incremental dataset fetches between full updates
+  --logfile LOGFILE     Output log messages to a file
+  --verbose             Enable verbose logging```
```

### Comparing `euc2mqtt-0.0.0/pyproject.toml` & `euc2mqtt-0.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [build-system]
 requires = [
     "setuptools>=61.0",
-#    "setuptools-scm>=8.0"
+    "setuptools-scm>=8.0"
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "euc2mqtt"
 authors = [
     {name = "islandc_"},
```

### Comparing `euc2mqtt-0.0.0/src/euc2mqtt/CLI.py` & `euc2mqtt-0.0.2/src/euc2mqtt/CLI.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,23 +6,25 @@
 
 class DefaultConfig:
     EUC_HOST: str = 'localhost'
     EUC_PORT: int = 4679
     HASSIO_HOST: str = 'homeassistant.local'
     HASSIO_PORT: int = 1883
     INTERVAL: int = 30
+    FULL_UPDATE_INTERVAL: int = 9
 
 def main():
     parser = argparse.ArgumentParser(prog='euc2mqtt', description='MQTT Publisher for Eaton UPS Companion status messages to Home Assistant. See https://github.com/islandcontroller/euc2mqtt for more info!')
     parser.add_argument('--name', help='Device name', type=str, default=None)
     parser.add_argument('--mqtt', help='MQTT broker hostname and port (hostname[:port])', type=str, default=f"{DefaultConfig.HASSIO_HOST}:{DefaultConfig.HASSIO_PORT}")
     parser.add_argument('--euc', help='Eaton UPS Companion hostname and port (hostname[:port])', type=str, default=f"{DefaultConfig.EUC_HOST}:{DefaultConfig.EUC_PORT}")
     parser.add_argument('--username', help='Username for MQTT broker authentication', type=str, default=None)
-    parser.add_argument('--password', help='Password fpr MQTT broker authentication', type=str, default=None)
+    parser.add_argument('--password', help='Password for MQTT broker authentication', type=str, default=None)
     parser.add_argument('--interval', help='Update interval in seconds', type=int, default=DefaultConfig.INTERVAL)
+    parser.add_argument('--full-update', help='Number of incremental dataset fetches between full updates', type=int, default=DefaultConfig.FULL_UPDATE_INTERVAL)
     parser.add_argument('--logfile', help='Output log messages to a file', type=str, default=None)
     parser.add_argument('--verbose', help='Enable verbose logging', action='store_true')
     args = parser.parse_args()
 
     logging.basicConfig(filename=args.logfile,
                         level=logging.DEBUG if args.verbose else logging.INFO,
                         format='%(asctime)s %(levelname)-8s %(message)s',
@@ -44,16 +46,22 @@
     handler.on_com_lost = [lambda: logging.log(logging.WARNING, 'EUC lost communication with UPS')]
     handler.on_register = [lambda e: logging.log(logging.DEBUG, f"Entity registered: {e.unique_id}")]
     handler.on_update = [lambda e, v: logging.log(logging.DEBUG, f"Entity updated: {e.unique_id} = {v}")]
     handler.on_unregister = [lambda e: logging.log(logging.DEBUG, f"Entity unregistered: {e.unique_id}")]
 
     logging.log(logging.INFO, f"Starting update loop ({args.interval}s update interval)...")
     handler.start()
+    update_count = 0
     while True:
         try:
-            handler.update()
+            logging.log(logging.DEBUG, f"Fetching {'full' if update_count == 0 else 'incremental'} dataset")
+            handler.update(update_count == 0)
+            if update_count == 0:
+                update_count = max(args.full_update, 0)
+            else:
+                update_count -= 1
             time.sleep(args.interval)
         except KeyboardInterrupt:
             logging.log(logging.WARNING, 'Caught KeyboardInterrupt, exiting...')
             break
     logging.log(logging.INFO, 'Stopping update loop...')
     handler.stop()
```

### Comparing `euc2mqtt-0.0.0/src/euc2mqtt/EatonAPI.py` & `euc2mqtt-0.0.2/src/euc2mqtt/EatonAPI.py`

 * *Files identical despite different names*

### Comparing `euc2mqtt-0.0.0/src/euc2mqtt/HassioAPI.py` & `euc2mqtt-0.0.2/src/euc2mqtt/HassioAPI.py`

 * *Files 1% similar despite different names*

```diff
@@ -120,17 +120,17 @@
             "availability_topic": self._availability_topic(entity),
             "device": {
                 "identifiers": entity.device.identifiers
             } if device_ident_only else {
                 **entity.device.discovery_data
             }
         })
-        self._mqtt.publish(self._discovery_topic(entity), payload).wait_for_publish()
+        self._mqtt.publish(self._discovery_topic(entity), payload, qos=1, retain=True).wait_for_publish()
 
     def unregister(self, entity: HassioEntity) -> None:
-        self._mqtt.publish(self._discovery_topic(entity), '').wait_for_publish()
+        self._mqtt.publish(self._discovery_topic(entity), '', qos=1).wait_for_publish()
 
     def update_availability(self, entity: HassioEntity, available: bool) -> None:
         self._mqtt.publish(self._availability_topic(entity), 'online' if available else 'offline').wait_for_publish()
 
     def update_state(self, entity: HassioEntity, payload) -> None:
         self._mqtt.publish(self._state_topic(entity), payload).wait_for_publish()
```

### Comparing `euc2mqtt-0.0.0/src/euc2mqtt/InteropE2H.py` & `euc2mqtt-0.0.2/src/euc2mqtt/InteropE2H.py`

 * *Files identical despite different names*

### Comparing `euc2mqtt-0.0.0/src/euc2mqtt/__init__.py` & `euc2mqtt-0.0.2/src/euc2mqtt/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -70,16 +70,16 @@
         self._add_sensors()
         # Start MQTT and register entities with Hassio
         self._hassio_client.start()
         self._register_entities()
         # Prepare update loop
         self._last_update = 0
 
-    def update(self):
-        data = self._eaton_client.get_data(self._last_update)
+    def update(self, full_update: bool = False):
+        data = self._eaton_client.get_data(0 if full_update else self._last_update)
         if 'lastUpdate' in data:
             # Update reference timestamp
             self._last_update = data['lastUpdate']
         if ('status' in data) and ('comLost' in data['status']) and bool(data['status']['comLost']):
             # Communication loss
             for e in self._collection.entities:
                 self._hassio_client.update_availability(e, False)
```

