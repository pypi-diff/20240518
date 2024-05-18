# Comparing `tmp/bluezero-0.8.0.tar.gz` & `tmp/bluezero-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bluezero-0.8.0.tar", last modified: Sun Aug  6 16:22:26 2023, max compression
+gzip compressed data, was "bluezero-0.9.0.tar", last modified: Sat May 18 18:00:30 2024, max compression
```

## Comparing `bluezero-0.8.0.tar` & `bluezero-0.9.0.tar`

### file list

```diff
@@ -1,30 +1,53 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 16:22:26.870475 bluezero-0.8.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-08-06 16:22:16.000000 bluezero-0.8.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4987 2023-08-06 16:22:26.870475 bluezero-0.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4093 2023-08-06 16:22:16.000000 bluezero-0.8.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 16:22:26.866475 bluezero-0.8.0/bluezero/
--rwxr-xr-x   0 runner    (1001) docker     (123)    15260 2023-08-06 16:22:16.000000 bluezero-0.8.0/bluezero/GATT.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-06 16:22:16.000000 bluezero-0.8.0/bluezero/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    11459 2023-08-06 16:22:16.000000 bluezero-0.8.0/bluezero/adapter.py
--rw-r--r--   0 runner    (1001) docker     (123)    11695 2023-08-06 16:22:16.000000 bluezero-0.8.0/bluezero/advertisement.py
--rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-08-06 16:22:16.000000 bluezero-0.8.0/bluezero/async_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)     2709 2023-08-06 16:22:16.000000 bluezero-0.8.0/bluezero/broadcaster.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3605 2023-08-06 16:22:16.000000 bluezero-0.8.0/bluezero/central.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1801 2023-08-06 16:22:16.000000 bluezero-0.8.0/bluezero/constants.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    14410 2023-08-06 16:22:16.000000 bluezero-0.8.0/bluezero/dbus_tools.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    10491 2023-08-06 16:22:16.000000 bluezero-0.8.0/bluezero/device.py
--rw-r--r--   0 runner    (1001) docker     (123)     1335 2023-08-06 16:22:16.000000 bluezero-0.8.0/bluezero/eddystone_beacon.py
--rw-r--r--   0 runner    (1001) docker     (123)    19355 2023-08-06 16:22:16.000000 bluezero-0.8.0/bluezero/localGATT.py
--rw-r--r--   0 runner    (1001) docker     (123)     5679 2023-08-06 16:22:16.000000 bluezero-0.8.0/bluezero/media_player.py
--rw-r--r--   0 runner    (1001) docker     (123)    36504 2023-08-06 16:22:16.000000 bluezero-0.8.0/bluezero/microbit.py
--rw-r--r--   0 runner    (1001) docker     (123)    10052 2023-08-06 16:22:16.000000 bluezero-0.8.0/bluezero/observer.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6857 2023-08-06 16:22:16.000000 bluezero-0.8.0/bluezero/peripheral.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5849 2023-08-06 16:22:16.000000 bluezero-0.8.0/bluezero/tools.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 16:22:26.870475 bluezero-0.8.0/bluezero.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4987 2023-08-06 16:22:26.000000 bluezero-0.8.0/bluezero.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      571 2023-08-06 16:22:26.000000 bluezero-0.8.0/bluezero.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-06 16:22:26.000000 bluezero-0.8.0/bluezero.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-08-06 16:22:26.000000 bluezero-0.8.0/bluezero.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-08-06 16:22:26.000000 bluezero-0.8.0/bluezero.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-08-06 16:22:26.870475 bluezero-0.8.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     4338 2023-08-06 16:22:16.000000 bluezero-0.8.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 18:00:30.311178 bluezero-0.9.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1080 2024-05-18 18:00:22.000000 bluezero-0.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5609 2024-05-18 18:00:30.311178 bluezero-0.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4093 2024-05-18 18:00:22.000000 bluezero-0.9.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 18:00:30.303178 bluezero-0.9.0/bluezero/
+-rwxr-xr-x   0 runner    (1001) docker     (127)    15260 2024-05-18 18:00:22.000000 bluezero-0.9.0/bluezero/GATT.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-18 18:00:22.000000 bluezero-0.9.0/bluezero/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    11459 2024-05-18 18:00:22.000000 bluezero-0.9.0/bluezero/adapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11869 2024-05-18 18:00:22.000000 bluezero-0.9.0/bluezero/advertisement.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1377 2024-05-18 18:00:22.000000 bluezero-0.9.0/bluezero/async_tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2709 2024-05-18 18:00:22.000000 bluezero-0.9.0/bluezero/broadcaster.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3605 2024-05-18 18:00:22.000000 bluezero-0.9.0/bluezero/central.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1801 2024-05-18 18:00:22.000000 bluezero-0.9.0/bluezero/constants.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    14410 2024-05-18 18:00:22.000000 bluezero-0.9.0/bluezero/dbus_tools.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    10491 2024-05-18 18:00:22.000000 bluezero-0.9.0/bluezero/device.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1335 2024-05-18 18:00:22.000000 bluezero-0.9.0/bluezero/eddystone_beacon.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19355 2024-05-18 18:00:22.000000 bluezero-0.9.0/bluezero/localGATT.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5679 2024-05-18 18:00:22.000000 bluezero-0.9.0/bluezero/media_player.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36504 2024-05-18 18:00:22.000000 bluezero-0.9.0/bluezero/microbit.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10052 2024-05-18 18:00:22.000000 bluezero-0.9.0/bluezero/observer.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6857 2024-05-18 18:00:22.000000 bluezero-0.9.0/bluezero/peripheral.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5849 2024-05-18 18:00:22.000000 bluezero-0.9.0/bluezero/tools.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 18:00:30.311178 bluezero-0.9.0/bluezero.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5609 2024-05-18 18:00:30.000000 bluezero-0.9.0/bluezero.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1183 2024-05-18 18:00:30.000000 bluezero-0.9.0/bluezero.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-18 18:00:30.000000 bluezero-0.9.0/bluezero.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      198 2024-05-18 18:00:30.000000 bluezero-0.9.0/bluezero.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-18 18:00:30.000000 bluezero-0.9.0/bluezero.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-05-18 18:00:30.311178 bluezero-0.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     4349 2024-05-18 18:00:22.000000 bluezero-0.9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 18:00:30.311178 bluezero-0.9.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     8400 2024-05-18 18:00:22.000000 bluezero-0.9.0/tests/test_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2337 2024-05-18 18:00:22.000000 bluezero-0.9.0/tests/test_adapter_example.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1573 2024-05-18 18:00:22.000000 bluezero-0.9.0/tests/test_adapter_example_db_mock.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2556 2024-05-18 18:00:22.000000 bluezero-0.9.0/tests/test_advertisement.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1103 2024-05-18 18:00:22.000000 bluezero-0.9.0/tests/test_async_tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1895 2024-05-18 18:00:22.000000 bluezero-0.9.0/tests/test_beacon_db_mock.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2378 2024-05-18 18:00:22.000000 bluezero-0.9.0/tests/test_broadcaster.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2495 2024-05-18 18:00:22.000000 bluezero-0.9.0/tests/test_central.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7790 2024-05-18 18:00:22.000000 bluezero-0.9.0/tests/test_dbus_tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8658 2024-05-18 18:00:22.000000 bluezero-0.9.0/tests/test_dbus_tools_mock.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6245 2024-05-18 18:00:22.000000 bluezero-0.9.0/tests/test_device.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1851 2024-05-18 18:00:22.000000 bluezero-0.9.0/tests/test_eddystone.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1507 2024-05-18 18:00:22.000000 bluezero-0.9.0/tests/test_eddystone_scanner_example.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1619 2024-05-18 18:00:22.000000 bluezero-0.9.0/tests/test_find_microbit_db_mock.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3714 2024-05-18 18:00:22.000000 bluezero-0.9.0/tests/test_gatt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2666 2024-05-18 18:00:22.000000 bluezero-0.9.0/tests/test_microbit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3159 2024-05-18 18:00:22.000000 bluezero-0.9.0/tests/test_microbit_poll_example.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2849 2024-05-18 18:00:22.000000 bluezero-0.9.0/tests/test_microbit_uart_db_mock.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5664 2024-05-18 18:00:22.000000 bluezero-0.9.0/tests/test_observer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1657 2024-05-18 18:00:22.000000 bluezero-0.9.0/tests/test_peripheral.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2157 2024-05-18 18:00:22.000000 bluezero-0.9.0/tests/test_peripheral_db_mock.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5908 2024-05-18 18:00:22.000000 bluezero-0.9.0/tests/test_tools.py
```

### Comparing `bluezero-0.8.0/LICENSE` & `bluezero-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `bluezero-0.8.0/PKG-INFO` & `bluezero-0.9.0/README.rst`

 * *Files 15% similar despite different names*

```diff
@@ -1,34 +1,7 @@
-Metadata-Version: 2.1
-Name: bluezero
-Version: 0.8.0
-Summary: Python library for Bluetooth Low Energy (BLE) on Linux
-Home-page: https://github.com/ukBaz/python-bluezero
-Author: Barry Byford
-Author-email: barry_byford@yahoo.co.uk
-Maintainer: Barry Byford
-Maintainer-email: barry_byford@yahoo.co.uk
-License: MIT
-Keywords: Bluetooth BLE development
-Classifier: Development Status :: 4 - Beta
-Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: Education
-Classifier: Topic :: System :: Hardware
-Classifier: Topic :: Software Development :: Embedded Systems
-Classifier: Topic :: Home Automation
-Classifier: Topic :: Education
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3 :: Only
-Description-Content-Type: text/x-rst
-Provides-Extra: rel
-Provides-Extra: docs
-Provides-Extra: test
-Provides-Extra: dev
-License-File: LICENSE
-
 ===============
 python-bluezero
 ===============
 .. image:: https://github.com/ukBaz/python-bluezero/workflows/bluezero-tests/badge.svg
     :target: https://github.com/ukBaz/python-bluezero/actions?query=workflow%3Abluezero-tests
     :alt: Build Status
```

### Comparing `bluezero-0.8.0/bluezero/GATT.py` & `bluezero-0.9.0/bluezero/GATT.py`

 * *Files identical despite different names*

### Comparing `bluezero-0.8.0/bluezero/adapter.py` & `bluezero-0.9.0/bluezero/adapter.py`

 * *Files identical despite different names*

### Comparing `bluezero-0.8.0/bluezero/advertisement.py` & `bluezero-0.9.0/bluezero/advertisement.py`

 * *Files 2% similar despite different names*

```diff
@@ -75,15 +75,15 @@
         self.props = {
             constants.LE_ADVERTISEMENT_IFACE: {
                 'Type': ad_type,
                 'ServiceUUIDs': None,
                 'ManufacturerData': None,
                 'SolicitUUIDs': None,
                 'ServiceData': None,
-                'IncludeTxPower': False,
+                'Includes': set(),
                 'Appearance': None,
                 'LocalName': None
             }
         }
 
     def start(self):
         """Start GLib event loop"""
@@ -146,21 +146,27 @@
             self.Set(constants.LE_ADVERTISEMENT_IFACE,
                      'ServiceData',
                      {uuid: dbus.Array(data[uuid], signature='y')})
 
     @property
     def include_tx_power(self):
         """Include TX power in advert (Different from beacon packet)"""
-        return self.Get(constants.LE_ADVERTISEMENT_IFACE,
-                        'IncludeTxPower')
+        includes = self.Get(constants.LE_ADVERTISEMENT_IFACE, 'Includes')
+        return 'tx-power' in includes
 
     @include_tx_power.setter
     def include_tx_power(self, state):
-        return self.Set(constants.LE_ADVERTISEMENT_IFACE,
-                        'IncludeTxPower', state)
+        if state:
+            self.props[
+                constants.LE_ADVERTISEMENT_IFACE][
+                'Includes'].add('tx-power')
+        else:
+            self.props[
+                constants.LE_ADVERTISEMENT_IFACE][
+                'Includes'].discard('tx-power')
 
     @property
     def local_name(self):
         """Local name of the device included in Advertisement."""
         return self.Get(constants.LE_ADVERTISEMENT_IFACE, 'LocalName')
 
     @local_name.setter
@@ -213,16 +219,16 @@
                 signature='s')
         if self.props[interface_name]['LocalName'] is not None:
             response['LocalName'] = dbus.String(
                     self.props[interface_name]['LocalName'])
         if self.props[interface_name]['Appearance'] is not None:
             response['Appearance'] = dbus.UInt16(
                     self.props[interface_name]['Appearance'])
-        response['IncludeTxPower'] = dbus.Boolean(
-            self.props[interface_name]['IncludeTxPower'])
+        response['Includes'] = dbus.Array(
+            self.props[interface_name]['Includes'], signature='s')
 
         return response
 
     @dbus.service.method(dbus.PROPERTIES_IFACE,
                          in_signature='ss', out_signature='v')
     def Get(self, interface_name,  # pylint: disable=invalid-name
             property_name):
```

### Comparing `bluezero-0.8.0/bluezero/async_tools.py` & `bluezero-0.9.0/bluezero/async_tools.py`

 * *Files identical despite different names*

### Comparing `bluezero-0.8.0/bluezero/broadcaster.py` & `bluezero-0.9.0/bluezero/broadcaster.py`

 * *Files identical despite different names*

### Comparing `bluezero-0.8.0/bluezero/central.py` & `bluezero-0.9.0/bluezero/central.py`

 * *Files identical despite different names*

### Comparing `bluezero-0.8.0/bluezero/constants.py` & `bluezero-0.9.0/bluezero/constants.py`

 * *Files identical despite different names*

### Comparing `bluezero-0.8.0/bluezero/dbus_tools.py` & `bluezero-0.9.0/bluezero/dbus_tools.py`

 * *Files identical despite different names*

### Comparing `bluezero-0.8.0/bluezero/device.py` & `bluezero-0.9.0/bluezero/device.py`

 * *Files identical despite different names*

### Comparing `bluezero-0.8.0/bluezero/eddystone_beacon.py` & `bluezero-0.9.0/bluezero/eddystone_beacon.py`

 * *Files identical despite different names*

### Comparing `bluezero-0.8.0/bluezero/localGATT.py` & `bluezero-0.9.0/bluezero/localGATT.py`

 * *Files identical despite different names*

### Comparing `bluezero-0.8.0/bluezero/media_player.py` & `bluezero-0.9.0/bluezero/media_player.py`

 * *Files identical despite different names*

### Comparing `bluezero-0.8.0/bluezero/microbit.py` & `bluezero-0.9.0/bluezero/microbit.py`

 * *Files identical despite different names*

### Comparing `bluezero-0.8.0/bluezero/observer.py` & `bluezero-0.9.0/bluezero/observer.py`

 * *Files identical despite different names*

### Comparing `bluezero-0.8.0/bluezero/peripheral.py` & `bluezero-0.9.0/bluezero/peripheral.py`

 * *Files identical despite different names*

### Comparing `bluezero-0.8.0/bluezero/tools.py` & `bluezero-0.9.0/bluezero/tools.py`

 * *Files identical despite different names*

### Comparing `bluezero-0.8.0/setup.py` & `bluezero-0.9.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from setuptools import setup
 # To use a consistent encoding
 from codecs import open
 from os import path
 
 here = path.abspath(path.dirname(__file__))
 
-required_packages = []
+required_packages = ['PyGObject']
 extras_rel = ['bumpversion', 'twine']
 extras_doc = ['sphinx', 'sphinx_rtd_theme']
 extras_test = ['coverage', 'pycodestyle', 'python-dbusmock']
 extras_dev = extras_rel + extras_doc + extras_test
 
 # Get the long description from the README file
 with open(path.join(here, 'README.rst'), encoding='utf-8') as f:
@@ -25,15 +25,15 @@
 
 setup(
     name='bluezero',
 
     # Versions should comply with PEP440.  For a discussion on single-sourcing
     # the version across setup.py and the project code, see
     # https://packaging.python.org/en/latest/single_source_version.html
-    version='0.8.0',
+    version='0.9.0',
 
     description='Python library for Bluetooth Low Energy (BLE) on Linux',
     long_description=long_description,
     long_description_content_type='text/x-rst',
 
     # The project's main homepage.
     url='https://github.com/ukBaz/python-bluezero',
```

