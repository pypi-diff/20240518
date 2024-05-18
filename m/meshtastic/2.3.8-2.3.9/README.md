# Comparing `tmp/meshtastic-2.3.8.tar.gz` & `tmp/meshtastic-2.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "meshtastic-2.3.8.tar", last modified: Wed May  1 16:42:42 2024, max compression
+gzip compressed data, was "meshtastic-2.3.9.tar", last modified: Sat May 18 00:15:20 2024, max compression
```

## Comparing `meshtastic-2.3.8.tar` & `meshtastic-2.3.9.tar`

### file list

```diff
@@ -1,72 +1,72 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 16:42:42.605169 meshtastic-2.3.8/
--rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-05-01 16:42:37.000000 meshtastic-2.3.8/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-01 16:42:37.000000 meshtastic-2.3.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     4169 2024-05-01 16:42:42.605169 meshtastic-2.3.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3023 2024-05-01 16:42:37.000000 meshtastic-2.3.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 16:42:42.601169 meshtastic-2.3.8/meshtastic/
--rw-r--r--   0 runner    (1001) docker     (127)     9091 2024-05-01 16:42:37.000000 meshtastic-2.3.8/meshtastic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    56982 2024-05-01 16:42:37.000000 meshtastic-2.3.8/meshtastic/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6076 2024-05-01 16:42:37.000000 meshtastic-2.3.8/meshtastic/admin_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)    25228 2024-05-01 16:42:37.000000 meshtastic-2.3.8/meshtastic/admin_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1583 2024-05-01 16:42:37.000000 meshtastic-2.3.8/meshtastic/apponly_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1901 2024-05-01 16:42:37.000000 meshtastic-2.3.8/meshtastic/apponly_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3396 2024-05-01 16:42:37.000000 meshtastic-2.3.8/meshtastic/atak_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)    10359 2024-05-01 16:42:37.000000 meshtastic-2.3.8/meshtastic/atak_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     8224 2024-05-01 16:42:37.000000 meshtastic-2.3.8/meshtastic/ble_interface.py
--rw-r--r--   0 runner    (1001) docker     (127)     1383 2024-05-01 16:42:37.000000 meshtastic-2.3.8/meshtastic/cannedmessages_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)      962 2024-05-01 16:42:37.000000 meshtastic-2.3.8/meshtastic/cannedmessages_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2389 2024-05-01 16:42:37.000000 meshtastic-2.3.8/meshtastic/channel_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     9814 2024-05-01 16:42:37.000000 meshtastic-2.3.8/meshtastic/channel_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1839 2024-05-01 16:42:37.000000 meshtastic-2.3.8/meshtastic/clientonly_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3406 2024-05-01 16:42:37.000000 meshtastic-2.3.8/meshtastic/clientonly_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    10953 2024-05-01 16:42:37.000000 meshtastic-2.3.8/meshtastic/config_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)    66376 2024-05-01 16:42:37.000000 meshtastic-2.3.8/meshtastic/config_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3036 2024-05-01 16:42:37.000000 meshtastic-2.3.8/meshtastic/connection_status_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     7484 2024-05-01 16:42:37.000000 meshtastic-2.3.8/meshtastic/connection_status_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     4764 2024-05-01 16:42:37.000000 meshtastic-2.3.8/meshtastic/deviceonly_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)    14192 2024-05-01 16:42:37.000000 meshtastic-2.3.8/meshtastic/deviceonly_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3373 2024-05-01 16:42:37.000000 meshtastic-2.3.8/meshtastic/localonly_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     9543 2024-05-01 16:42:37.000000 meshtastic-2.3.8/meshtastic/localonly_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    46114 2024-05-01 16:42:37.000000 meshtastic-2.3.8/meshtastic/mesh_interface.py
--rw-r--r--   0 runner    (1001) docker     (127)    15110 2024-05-01 16:42:37.000000 meshtastic-2.3.8/meshtastic/mesh_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)    87037 2024-05-01 16:42:37.000000 meshtastic-2.3.8/meshtastic/mesh_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    11502 2024-05-01 16:42:37.000000 meshtastic-2.3.8/meshtastic/module_config_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)    48852 2024-05-01 16:42:37.000000 meshtastic-2.3.8/meshtastic/module_config_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2368 2024-05-01 16:42:37.000000 meshtastic-2.3.8/meshtastic/mqtt_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     5617 2024-05-01 16:42:37.000000 meshtastic-2.3.8/meshtastic/mqtt_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1162 2024-05-01 16:42:37.000000 meshtastic-2.3.8/meshtastic/mt_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     4551 2024-05-01 16:42:37.000000 meshtastic-2.3.8/meshtastic/nanopb_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)    16031 2024-05-01 16:42:37.000000 meshtastic-2.3.8/meshtastic/nanopb_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    31992 2024-05-01 16:42:37.000000 meshtastic-2.3.8/meshtastic/node.py
--rw-r--r--   0 runner    (1001) docker     (127)     1348 2024-05-01 16:42:37.000000 meshtastic-2.3.8/meshtastic/paxcount_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1111 2024-05-01 16:42:37.000000 meshtastic-2.3.8/meshtastic/paxcount_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2162 2024-05-01 16:42:37.000000 meshtastic-2.3.8/meshtastic/portnums_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)    13631 2024-05-01 16:42:37.000000 meshtastic-2.3.8/meshtastic/portnums_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3770 2024-05-01 16:42:37.000000 meshtastic-2.3.8/meshtastic/remote_hardware.py
--rw-r--r--   0 runner    (1001) docker     (127)     1739 2024-05-01 16:42:37.000000 meshtastic-2.3.8/meshtastic/remote_hardware_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     4500 2024-05-01 16:42:37.000000 meshtastic-2.3.8/meshtastic/remote_hardware_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1289 2024-05-01 16:42:37.000000 meshtastic-2.3.8/meshtastic/rtttl_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)      886 2024-05-01 16:42:37.000000 meshtastic-2.3.8/meshtastic/rtttl_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2638 2024-05-01 16:42:37.000000 meshtastic-2.3.8/meshtastic/serial_interface.py
--rw-r--r--   0 runner    (1001) docker     (127)     3318 2024-05-01 16:42:37.000000 meshtastic-2.3.8/meshtastic/storeforward_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)    11982 2024-05-01 16:42:37.000000 meshtastic-2.3.8/meshtastic/storeforward_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     7866 2024-05-01 16:42:37.000000 meshtastic-2.3.8/meshtastic/stream_interface.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     6140 2024-05-01 16:42:37.000000 meshtastic-2.3.8/meshtastic/supported_device.py
--rw-r--r--   0 runner    (1001) docker     (127)     2389 2024-05-01 16:42:37.000000 meshtastic-2.3.8/meshtastic/tcp_interface.py
--rw-r--r--   0 runner    (1001) docker     (127)     4108 2024-05-01 16:42:37.000000 meshtastic-2.3.8/meshtastic/telemetry_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)    14907 2024-05-01 16:42:37.000000 meshtastic-2.3.8/meshtastic/telemetry_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     6013 2024-05-01 16:42:37.000000 meshtastic-2.3.8/meshtastic/test.py
--rw-r--r--   0 runner    (1001) docker     (127)     8653 2024-05-01 16:42:37.000000 meshtastic-2.3.8/meshtastic/tunnel.py
--rw-r--r--   0 runner    (1001) docker     (127)    21571 2024-05-01 16:42:37.000000 meshtastic-2.3.8/meshtastic/util.py
--rw-r--r--   0 runner    (1001) docker     (127)      447 2024-05-01 16:42:37.000000 meshtastic-2.3.8/meshtastic/version.py
--rw-r--r--   0 runner    (1001) docker     (127)     1738 2024-05-01 16:42:37.000000 meshtastic-2.3.8/meshtastic/xmodem_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2276 2024-05-01 16:42:37.000000 meshtastic-2.3.8/meshtastic/xmodem_pb2.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 16:42:42.605169 meshtastic-2.3.8/meshtastic.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4169 2024-05-01 16:42:42.000000 meshtastic-2.3.8/meshtastic.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1803 2024-05-01 16:42:42.000000 meshtastic-2.3.8/meshtastic.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 16:42:42.000000 meshtastic-2.3.8/meshtastic.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      110 2024-05-01 16:42:42.000000 meshtastic-2.3.8/meshtastic.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      197 2024-05-01 16:42:42.000000 meshtastic-2.3.8/meshtastic.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-01 16:42:42.000000 meshtastic-2.3.8/meshtastic.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-01 16:42:42.605169 meshtastic-2.3.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1763 2024-05-01 16:42:37.000000 meshtastic-2.3.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 00:15:20.681163 meshtastic-2.3.9/
+-rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-05-18 00:15:11.000000 meshtastic-2.3.9/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-18 00:15:11.000000 meshtastic-2.3.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4235 2024-05-18 00:15:20.681163 meshtastic-2.3.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3089 2024-05-18 00:15:11.000000 meshtastic-2.3.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 00:15:20.677163 meshtastic-2.3.9/meshtastic/
+-rw-r--r--   0 runner    (1001) docker     (127)     9091 2024-05-18 00:15:11.000000 meshtastic-2.3.9/meshtastic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    57154 2024-05-18 00:15:11.000000 meshtastic-2.3.9/meshtastic/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6076 2024-05-18 00:15:11.000000 meshtastic-2.3.9/meshtastic/admin_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25228 2024-05-18 00:15:11.000000 meshtastic-2.3.9/meshtastic/admin_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1583 2024-05-18 00:15:11.000000 meshtastic-2.3.9/meshtastic/apponly_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1901 2024-05-18 00:15:11.000000 meshtastic-2.3.9/meshtastic/apponly_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3396 2024-05-18 00:15:11.000000 meshtastic-2.3.9/meshtastic/atak_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10359 2024-05-18 00:15:11.000000 meshtastic-2.3.9/meshtastic/atak_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     8274 2024-05-18 00:15:11.000000 meshtastic-2.3.9/meshtastic/ble_interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1383 2024-05-18 00:15:11.000000 meshtastic-2.3.9/meshtastic/cannedmessages_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      962 2024-05-18 00:15:11.000000 meshtastic-2.3.9/meshtastic/cannedmessages_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2389 2024-05-18 00:15:11.000000 meshtastic-2.3.9/meshtastic/channel_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9814 2024-05-18 00:15:11.000000 meshtastic-2.3.9/meshtastic/channel_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1839 2024-05-18 00:15:11.000000 meshtastic-2.3.9/meshtastic/clientonly_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3406 2024-05-18 00:15:11.000000 meshtastic-2.3.9/meshtastic/clientonly_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    10953 2024-05-18 00:15:11.000000 meshtastic-2.3.9/meshtastic/config_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    66376 2024-05-18 00:15:11.000000 meshtastic-2.3.9/meshtastic/config_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3036 2024-05-18 00:15:11.000000 meshtastic-2.3.9/meshtastic/connection_status_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7484 2024-05-18 00:15:11.000000 meshtastic-2.3.9/meshtastic/connection_status_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     4764 2024-05-18 00:15:11.000000 meshtastic-2.3.9/meshtastic/deviceonly_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14192 2024-05-18 00:15:11.000000 meshtastic-2.3.9/meshtastic/deviceonly_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3373 2024-05-18 00:15:11.000000 meshtastic-2.3.9/meshtastic/localonly_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9543 2024-05-18 00:15:11.000000 meshtastic-2.3.9/meshtastic/localonly_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    46726 2024-05-18 00:15:11.000000 meshtastic-2.3.9/meshtastic/mesh_interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15176 2024-05-18 00:15:11.000000 meshtastic-2.3.9/meshtastic/mesh_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    87517 2024-05-18 00:15:11.000000 meshtastic-2.3.9/meshtastic/mesh_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    11502 2024-05-18 00:15:11.000000 meshtastic-2.3.9/meshtastic/module_config_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    48852 2024-05-18 00:15:11.000000 meshtastic-2.3.9/meshtastic/module_config_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2368 2024-05-18 00:15:11.000000 meshtastic-2.3.9/meshtastic/mqtt_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5617 2024-05-18 00:15:11.000000 meshtastic-2.3.9/meshtastic/mqtt_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1162 2024-05-18 00:15:11.000000 meshtastic-2.3.9/meshtastic/mt_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4551 2024-05-18 00:15:11.000000 meshtastic-2.3.9/meshtastic/nanopb_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16031 2024-05-18 00:15:11.000000 meshtastic-2.3.9/meshtastic/nanopb_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    31992 2024-05-18 00:15:11.000000 meshtastic-2.3.9/meshtastic/node.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1348 2024-05-18 00:15:11.000000 meshtastic-2.3.9/meshtastic/paxcount_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1111 2024-05-18 00:15:11.000000 meshtastic-2.3.9/meshtastic/paxcount_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2162 2024-05-18 00:15:11.000000 meshtastic-2.3.9/meshtastic/portnums_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13631 2024-05-18 00:15:11.000000 meshtastic-2.3.9/meshtastic/portnums_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3770 2024-05-18 00:15:11.000000 meshtastic-2.3.9/meshtastic/remote_hardware.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1739 2024-05-18 00:15:11.000000 meshtastic-2.3.9/meshtastic/remote_hardware_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4500 2024-05-18 00:15:11.000000 meshtastic-2.3.9/meshtastic/remote_hardware_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1289 2024-05-18 00:15:11.000000 meshtastic-2.3.9/meshtastic/rtttl_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      886 2024-05-18 00:15:11.000000 meshtastic-2.3.9/meshtastic/rtttl_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2697 2024-05-18 00:15:11.000000 meshtastic-2.3.9/meshtastic/serial_interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3318 2024-05-18 00:15:11.000000 meshtastic-2.3.9/meshtastic/storeforward_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11982 2024-05-18 00:15:11.000000 meshtastic-2.3.9/meshtastic/storeforward_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     7866 2024-05-18 00:15:11.000000 meshtastic-2.3.9/meshtastic/stream_interface.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6140 2024-05-18 00:15:11.000000 meshtastic-2.3.9/meshtastic/supported_device.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2389 2024-05-18 00:15:11.000000 meshtastic-2.3.9/meshtastic/tcp_interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4133 2024-05-18 00:15:11.000000 meshtastic-2.3.9/meshtastic/telemetry_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15124 2024-05-18 00:15:11.000000 meshtastic-2.3.9/meshtastic/telemetry_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     6013 2024-05-18 00:15:11.000000 meshtastic-2.3.9/meshtastic/test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8653 2024-05-18 00:15:11.000000 meshtastic-2.3.9/meshtastic/tunnel.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21618 2024-05-18 00:15:11.000000 meshtastic-2.3.9/meshtastic/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)      447 2024-05-18 00:15:11.000000 meshtastic-2.3.9/meshtastic/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1738 2024-05-18 00:15:11.000000 meshtastic-2.3.9/meshtastic/xmodem_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2276 2024-05-18 00:15:11.000000 meshtastic-2.3.9/meshtastic/xmodem_pb2.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 00:15:20.681163 meshtastic-2.3.9/meshtastic.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4235 2024-05-18 00:15:20.000000 meshtastic-2.3.9/meshtastic.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1803 2024-05-18 00:15:20.000000 meshtastic-2.3.9/meshtastic.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-18 00:15:20.000000 meshtastic-2.3.9/meshtastic.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      110 2024-05-18 00:15:20.000000 meshtastic-2.3.9/meshtastic.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      197 2024-05-18 00:15:20.000000 meshtastic-2.3.9/meshtastic.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-18 00:15:20.000000 meshtastic-2.3.9/meshtastic.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-18 00:15:20.681163 meshtastic-2.3.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1763 2024-05-18 00:15:11.000000 meshtastic-2.3.9/setup.py
```

### Comparing `meshtastic-2.3.8/LICENSE.txt` & `meshtastic-2.3.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `meshtastic-2.3.8/PKG-INFO` & `meshtastic-2.3.9/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: meshtastic
-Version: 2.3.8
+Version: 2.3.9
 Summary: Python API & client shell for talking to Meshtastic devices
 Home-page: https://github.com/meshtastic/python
 Author: Meshtastic Developers
 Author-email: contact@meshtastic.org
 License: GPL-3.0-only
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Development Status :: 4 - Beta
@@ -57,28 +57,27 @@
 If you're interested in contributing but don't have specific things you'd like to work on, look at the roadmap below!
 
 ## Roadmap
 
 This should always be considered a list in progress and flux -- inclusion doesn't guarantee implementation, and exclusion doesn't mean something's not wanted. GitHub issues are a great place to discuss ideas.
 
 * Types
-  * type annotations throughout the codebase
-  * mypy running in CI to type-check new code
+  * type annotations throughout the codebase, and upgrading mypy running in CI to `--strict`
 * async-friendliness
 * CLI completeness & consistency
   * the CLI should support all features of the firmware
   * there should be a consistent output format available for shell scripting
 * CLI input validation & documentation
   * what arguments and options are compatible & incompatible with one another?
   * can the options be restructured in a way that is more self-documenting?
   * pubsub events should be documented clearly
 * helpers for third-party code
   * it should be easy to write a script that supports similar options to the CLI so many tools support the same ways of connecting to nodes
-* interactive client
 * data storage & processing
   * there should be a standardized way of recording packets for later use, debugging, etc.
+  * a persistence layer could also keep track of nodes beyond nodedb, as the apps do
   * a sqlite database schema and tools for writing to it may be a good starting point
   * enable maps, charts, visualizations
 
 ## Stats
 
 ![Alt](https://repobeats.axiom.co/api/embed/c71ee8fc4a79690402e5d2807a41eec5e96d9039.svg "Repobeats analytics image")
```

### Comparing `meshtastic-2.3.8/README.md` & `meshtastic-2.3.9/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -24,28 +24,27 @@
 If you're interested in contributing but don't have specific things you'd like to work on, look at the roadmap below!
 
 ## Roadmap
 
 This should always be considered a list in progress and flux -- inclusion doesn't guarantee implementation, and exclusion doesn't mean something's not wanted. GitHub issues are a great place to discuss ideas.
 
 * Types
-  * type annotations throughout the codebase
-  * mypy running in CI to type-check new code
+  * type annotations throughout the codebase, and upgrading mypy running in CI to `--strict`
 * async-friendliness
 * CLI completeness & consistency
   * the CLI should support all features of the firmware
   * there should be a consistent output format available for shell scripting
 * CLI input validation & documentation
   * what arguments and options are compatible & incompatible with one another?
   * can the options be restructured in a way that is more self-documenting?
   * pubsub events should be documented clearly
 * helpers for third-party code
   * it should be easy to write a script that supports similar options to the CLI so many tools support the same ways of connecting to nodes
-* interactive client
 * data storage & processing
   * there should be a standardized way of recording packets for later use, debugging, etc.
+  * a persistence layer could also keep track of nodes beyond nodedb, as the apps do
   * a sqlite database schema and tools for writing to it may be a good starting point
   * enable maps, charts, visualizations
 
 ## Stats
 
 ![Alt](https://repobeats.axiom.co/api/embed/c71ee8fc4a79690402e5d2807a41eec5e96d9039.svg "Repobeats analytics image")
```

### Comparing `meshtastic-2.3.8/meshtastic/__init__.py` & `meshtastic-2.3.9/meshtastic/__init__.py`

 * *Files identical despite different names*

### Comparing `meshtastic-2.3.8/meshtastic/__main__.py` & `meshtastic-2.3.9/meshtastic/__main__.py`

 * *Files 0% similar despite different names*

```diff
@@ -261,15 +261,14 @@
                 print("Setting latitude, longitude, and altitude of remote nodes is not supported.")
                 return
             closeNow = True
 
             alt = 0
             lat = 0.0
             lon = 0.0
-            # TODO: use getNode(args.dest) to be able to set it for a remote node
             localConfig = interface.localNode.localConfig
             if args.setalt:
                 alt = int(args.setalt)
                 localConfig.position.fixed_position = True
                 print(f"Fixing altitude at {alt} meters")
             if args.setlat:
                 lat = float(args.setlat)
@@ -718,14 +717,18 @@
 
             channelIndex = mt_config.channel_index
             if channelIndex is None:
                 meshtastic.util.our_exit("Warning: Need to specify '--ch-index'.", 1)
             ch = interface.getNode(args.dest).channels[channelIndex]
 
             if args.ch_enable or args.ch_disable:
+                print(
+                    "Warning: --ch-enable and --ch-disable can produce noncontiguous channels, "
+                    "which can cause errors in some clients. Whenever possible, use --ch-add and --ch-del instead."
+                )
                 if channelIndex == 0:
                     meshtastic.util.our_exit(
                         "Warning: Cannot enable/disable PRIMARY channel."
                     )
 
                 enable = True  # default to enable
                 if args.ch_enable:
@@ -1347,15 +1350,15 @@
         "You need to pass the destination ID as argument with '--dest'. "
         "For repeaters, the nodeNum is required.",
         action="store_true",
     )
 
     group.add_argument(
         "--request-position",
-        help="Request the position from a nade. "
+        help="Request the position from a node. "
         "You need to pass the destination ID as an argument with '--dest'. "
         "For repeaters, the nodeNum is required.",
         action="store_true",
     )
 
     group.add_argument(
         "--ack",
```

### Comparing `meshtastic-2.3.8/meshtastic/admin_pb2.py` & `meshtastic-2.3.9/meshtastic/admin_pb2.py`

 * *Files identical despite different names*

### Comparing `meshtastic-2.3.8/meshtastic/admin_pb2.pyi` & `meshtastic-2.3.9/meshtastic/admin_pb2.pyi`

 * *Files identical despite different names*

### Comparing `meshtastic-2.3.8/meshtastic/apponly_pb2.py` & `meshtastic-2.3.9/meshtastic/apponly_pb2.py`

 * *Files identical despite different names*

### Comparing `meshtastic-2.3.8/meshtastic/apponly_pb2.pyi` & `meshtastic-2.3.9/meshtastic/apponly_pb2.pyi`

 * *Files identical despite different names*

### Comparing `meshtastic-2.3.8/meshtastic/atak_pb2.py` & `meshtastic-2.3.9/meshtastic/atak_pb2.py`

 * *Files identical despite different names*

### Comparing `meshtastic-2.3.8/meshtastic/atak_pb2.pyi` & `meshtastic-2.3.9/meshtastic/atak_pb2.pyi`

 * *Files identical despite different names*

### Comparing `meshtastic-2.3.8/meshtastic/ble_interface.py` & `meshtastic-2.3.9/meshtastic/ble_interface.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 """Bluetooth interface
 """
 import logging
 import time
 import struct
 import asyncio
 from threading import Thread, Event
+from typing import Optional
+
 from bleak import BleakScanner, BleakClient
 
 from meshtastic.mesh_interface import MeshInterface
 from meshtastic.util import our_exit
 
 SERVICE_UUID = "6ba1b218-15a8-461f-9fa8-5dcae273eafd"
 TORADIO_UUID = "f75c76d2-129e-4dad-a1dd-7866124401e7"
@@ -26,15 +28,15 @@
 
     class BLEState(): # pylint: disable=C0115
         THREADS = False
         BLE = False
         MESH = False
 
 
-    def __init__(self, address, noProto = False, debugOut = None):
+    def __init__(self, address: Optional[str], noProto: bool = False, debugOut = None):
         self.state = BLEInterface.BLEState()
 
         if not address:
             return
 
         self.should_read = False
```

### Comparing `meshtastic-2.3.8/meshtastic/cannedmessages_pb2.py` & `meshtastic-2.3.9/meshtastic/cannedmessages_pb2.py`

 * *Files identical despite different names*

### Comparing `meshtastic-2.3.8/meshtastic/cannedmessages_pb2.pyi` & `meshtastic-2.3.9/meshtastic/cannedmessages_pb2.pyi`

 * *Files identical despite different names*

### Comparing `meshtastic-2.3.8/meshtastic/channel_pb2.py` & `meshtastic-2.3.9/meshtastic/channel_pb2.py`

 * *Files identical despite different names*

### Comparing `meshtastic-2.3.8/meshtastic/channel_pb2.pyi` & `meshtastic-2.3.9/meshtastic/channel_pb2.pyi`

 * *Files identical despite different names*

### Comparing `meshtastic-2.3.8/meshtastic/clientonly_pb2.py` & `meshtastic-2.3.9/meshtastic/clientonly_pb2.py`

 * *Files identical despite different names*

### Comparing `meshtastic-2.3.8/meshtastic/clientonly_pb2.pyi` & `meshtastic-2.3.9/meshtastic/clientonly_pb2.pyi`

 * *Files identical despite different names*

### Comparing `meshtastic-2.3.8/meshtastic/config_pb2.py` & `meshtastic-2.3.9/meshtastic/config_pb2.py`

 * *Files identical despite different names*

### Comparing `meshtastic-2.3.8/meshtastic/config_pb2.pyi` & `meshtastic-2.3.9/meshtastic/config_pb2.pyi`

 * *Files identical despite different names*

### Comparing `meshtastic-2.3.8/meshtastic/connection_status_pb2.py` & `meshtastic-2.3.9/meshtastic/connection_status_pb2.py`

 * *Files identical despite different names*

### Comparing `meshtastic-2.3.8/meshtastic/connection_status_pb2.pyi` & `meshtastic-2.3.9/meshtastic/connection_status_pb2.pyi`

 * *Files identical despite different names*

### Comparing `meshtastic-2.3.8/meshtastic/deviceonly_pb2.py` & `meshtastic-2.3.9/meshtastic/deviceonly_pb2.py`

 * *Files identical despite different names*

### Comparing `meshtastic-2.3.8/meshtastic/deviceonly_pb2.pyi` & `meshtastic-2.3.9/meshtastic/deviceonly_pb2.pyi`

 * *Files identical despite different names*

### Comparing `meshtastic-2.3.8/meshtastic/localonly_pb2.py` & `meshtastic-2.3.9/meshtastic/localonly_pb2.py`

 * *Files identical despite different names*

### Comparing `meshtastic-2.3.8/meshtastic/localonly_pb2.pyi` & `meshtastic-2.3.9/meshtastic/localonly_pb2.pyi`

 * *Files identical despite different names*

### Comparing `meshtastic-2.3.8/meshtastic/mesh_interface.py` & `meshtastic-2.3.9/meshtastic/mesh_interface.py`

 * *Files 1% similar despite different names*

```diff
@@ -207,16 +207,16 @@
                             ),
                         }
                     )
 
                 row.update(
                     {
                         "SNR": formatFloat(node.get("snr"), 2, " dB"),
-                        "Hops Away": node.get("hopsAway", "unknown"),
-                        "Channel": node.get("channel"),
+                        "Hops Away": node.get("hopsAway", "0/unknown"),
+                        "Channel": node.get("channel", 0),
                         "LastHeard": getLH(node.get("lastHeard")),
                         "Since": getTimeAgo(node.get("lastHeard")),
                     }
                 )
 
                 rows.append(row)
 
@@ -871,22 +871,36 @@
             self._handleChannel(fromRadio.channel)
         elif fromRadio.HasField("packet"):
             self._handlePacketFromRadio(fromRadio.packet)
 
         elif fromRadio.HasField("queueStatus"):
             self._handleQueueStatusFromRadio(fromRadio.queueStatus)
 
-        elif fromRadio.rebooted:
+        elif fromRadio.HasField("mqttClientProxyMessage"):
+            publishingThread.queueWork(
+                lambda: pub.sendMessage(
+                    "meshtastic.mqttclientproxymessage", proxymessage=fromRadio.mqttClientProxyMessage, interface=self
+                )
+            )
+
+        elif fromRadio.HasField("xmodemPacket"):
+            publishingThread.queueWork(
+                lambda: pub.sendMessage(
+                    "meshtastic.xmodempacket", packet=fromRadio.xmodemPacket, interface=self
+                )
+            )
+
+        elif fromRadio.HasField("rebooted") and fromRadio.rebooted:
             # Tell clients the device went away.  Careful not to call the overridden
             # subclass version that closes the serial port
             MeshInterface._disconnected(self)
 
             self._startConfig()  # redownload the node db etc...
 
-        elif fromRadio.config or fromRadio.moduleConfig:
+        elif fromRadio.HasField("config") or fromRadio.HasField("moduleConfig"):
             if fromRadio.config.HasField("device"):
                 self.localNode.localConfig.device.CopyFrom(fromRadio.config.device)
             elif fromRadio.config.HasField("position"):
                 self.localNode.localConfig.position.CopyFrom(fromRadio.config.position)
             elif fromRadio.config.HasField("power"):
                 self.localNode.localConfig.power.CopyFrom(fromRadio.config.power)
             elif fromRadio.config.HasField("network"):
```

### Comparing `meshtastic-2.3.8/meshtastic/mesh_pb2.py` & `meshtastic-2.3.9/meshtastic/mesh_pb2.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,32 +15,32 @@
 from meshtastic import config_pb2 as meshtastic_dot_config__pb2
 from meshtastic import module_config_pb2 as meshtastic_dot_module__config__pb2
 from meshtastic import portnums_pb2 as meshtastic_dot_portnums__pb2
 from meshtastic import telemetry_pb2 as meshtastic_dot_telemetry__pb2
 from meshtastic import xmodem_pb2 as meshtastic_dot_xmodem__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x15meshtastic/mesh.proto\x12\nmeshtastic\x1a\x18meshtastic/channel.proto\x1a\x17meshtastic/config.proto\x1a\x1emeshtastic/module_config.proto\x1a\x19meshtastic/portnums.proto\x1a\x1ameshtastic/telemetry.proto\x1a\x17meshtastic/xmodem.proto\"\xe5\x05\n\x08Position\x12\x12\n\nlatitude_i\x18\x01 \x01(\x0f\x12\x13\n\x0blongitude_i\x18\x02 \x01(\x0f\x12\x10\n\x08\x61ltitude\x18\x03 \x01(\x05\x12\x0c\n\x04time\x18\x04 \x01(\x07\x12\x37\n\x0flocation_source\x18\x05 \x01(\x0e\x32\x1e.meshtastic.Position.LocSource\x12\x37\n\x0f\x61ltitude_source\x18\x06 \x01(\x0e\x32\x1e.meshtastic.Position.AltSource\x12\x11\n\ttimestamp\x18\x07 \x01(\x07\x12\x1f\n\x17timestamp_millis_adjust\x18\x08 \x01(\x05\x12\x14\n\x0c\x61ltitude_hae\x18\t \x01(\x11\x12#\n\x1b\x61ltitude_geoidal_separation\x18\n \x01(\x11\x12\x0c\n\x04PDOP\x18\x0b \x01(\r\x12\x0c\n\x04HDOP\x18\x0c \x01(\r\x12\x0c\n\x04VDOP\x18\r \x01(\r\x12\x14\n\x0cgps_accuracy\x18\x0e \x01(\r\x12\x14\n\x0cground_speed\x18\x0f \x01(\r\x12\x14\n\x0cground_track\x18\x10 \x01(\r\x12\x13\n\x0b\x66ix_quality\x18\x11 \x01(\r\x12\x10\n\x08\x66ix_type\x18\x12 \x01(\r\x12\x14\n\x0csats_in_view\x18\x13 \x01(\r\x12\x11\n\tsensor_id\x18\x14 \x01(\r\x12\x13\n\x0bnext_update\x18\x15 \x01(\r\x12\x12\n\nseq_number\x18\x16 \x01(\r\x12\x16\n\x0eprecision_bits\x18\x17 \x01(\r\"N\n\tLocSource\x12\r\n\tLOC_UNSET\x10\x00\x12\x0e\n\nLOC_MANUAL\x10\x01\x12\x10\n\x0cLOC_INTERNAL\x10\x02\x12\x10\n\x0cLOC_EXTERNAL\x10\x03\"b\n\tAltSource\x12\r\n\tALT_UNSET\x10\x00\x12\x0e\n\nALT_MANUAL\x10\x01\x12\x10\n\x0c\x41LT_INTERNAL\x10\x02\x12\x10\n\x0c\x41LT_EXTERNAL\x10\x03\x12\x12\n\x0e\x41LT_BAROMETRIC\x10\x04\"\xc4\x01\n\x04User\x12\n\n\x02id\x18\x01 \x01(\t\x12\x11\n\tlong_name\x18\x02 \x01(\t\x12\x12\n\nshort_name\x18\x03 \x01(\t\x12\x13\n\x07macaddr\x18\x04 \x01(\x0c\x42\x02\x18\x01\x12+\n\x08hw_model\x18\x05 \x01(\x0e\x32\x19.meshtastic.HardwareModel\x12\x13\n\x0bis_licensed\x18\x06 \x01(\x08\x12\x32\n\x04role\x18\x07 \x01(\x0e\x32$.meshtastic.Config.DeviceConfig.Role\"\x1f\n\x0eRouteDiscovery\x12\r\n\x05route\x18\x01 \x03(\x07\"\xfc\x02\n\x07Routing\x12\x33\n\rroute_request\x18\x01 \x01(\x0b\x32\x1a.meshtastic.RouteDiscoveryH\x00\x12\x31\n\x0broute_reply\x18\x02 \x01(\x0b\x32\x1a.meshtastic.RouteDiscoveryH\x00\x12\x31\n\x0c\x65rror_reason\x18\x03 \x01(\x0e\x32\x19.meshtastic.Routing.ErrorH\x00\"\xca\x01\n\x05\x45rror\x12\x08\n\x04NONE\x10\x00\x12\x0c\n\x08NO_ROUTE\x10\x01\x12\x0b\n\x07GOT_NAK\x10\x02\x12\x0b\n\x07TIMEOUT\x10\x03\x12\x10\n\x0cNO_INTERFACE\x10\x04\x12\x12\n\x0eMAX_RETRANSMIT\x10\x05\x12\x0e\n\nNO_CHANNEL\x10\x06\x12\r\n\tTOO_LARGE\x10\x07\x12\x0f\n\x0bNO_RESPONSE\x10\x08\x12\x14\n\x10\x44UTY_CYCLE_LIMIT\x10\t\x12\x0f\n\x0b\x42\x41\x44_REQUEST\x10 \x12\x12\n\x0eNOT_AUTHORIZED\x10!B\t\n\x07variant\"\xa7\x01\n\x04\x44\x61ta\x12$\n\x07portnum\x18\x01 \x01(\x0e\x32\x13.meshtastic.PortNum\x12\x0f\n\x07payload\x18\x02 \x01(\x0c\x12\x15\n\rwant_response\x18\x03 \x01(\x08\x12\x0c\n\x04\x64\x65st\x18\x04 \x01(\x07\x12\x0e\n\x06source\x18\x05 \x01(\x07\x12\x12\n\nrequest_id\x18\x06 \x01(\x07\x12\x10\n\x08reply_id\x18\x07 \x01(\x07\x12\r\n\x05\x65moji\x18\x08 \x01(\x07\"\x93\x01\n\x08Waypoint\x12\n\n\x02id\x18\x01 \x01(\r\x12\x12\n\nlatitude_i\x18\x02 \x01(\x0f\x12\x13\n\x0blongitude_i\x18\x03 \x01(\x0f\x12\x0e\n\x06\x65xpire\x18\x04 \x01(\r\x12\x11\n\tlocked_to\x18\x05 \x01(\r\x12\x0c\n\x04name\x18\x06 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x07 \x01(\t\x12\x0c\n\x04icon\x18\x08 \x01(\x07\"l\n\x16MqttClientProxyMessage\x12\r\n\x05topic\x18\x01 \x01(\t\x12\x0e\n\x04\x64\x61ta\x18\x02 \x01(\x0cH\x00\x12\x0e\n\x04text\x18\x03 \x01(\tH\x00\x12\x10\n\x08retained\x18\x04 \x01(\x08\x42\x11\n\x0fpayload_variant\"\x95\x04\n\nMeshPacket\x12\x0c\n\x04\x66rom\x18\x01 \x01(\x07\x12\n\n\x02to\x18\x02 \x01(\x07\x12\x0f\n\x07\x63hannel\x18\x03 \x01(\r\x12#\n\x07\x64\x65\x63oded\x18\x04 \x01(\x0b\x32\x10.meshtastic.DataH\x00\x12\x13\n\tencrypted\x18\x05 \x01(\x0cH\x00\x12\n\n\x02id\x18\x06 \x01(\x07\x12\x0f\n\x07rx_time\x18\x07 \x01(\x07\x12\x0e\n\x06rx_snr\x18\x08 \x01(\x02\x12\x11\n\thop_limit\x18\t \x01(\r\x12\x10\n\x08want_ack\x18\n \x01(\x08\x12\x31\n\x08priority\x18\x0b \x01(\x0e\x32\x1f.meshtastic.MeshPacket.Priority\x12\x0f\n\x07rx_rssi\x18\x0c \x01(\x05\x12\x33\n\x07\x64\x65layed\x18\r \x01(\x0e\x32\x1e.meshtastic.MeshPacket.DelayedB\x02\x18\x01\x12\x10\n\x08via_mqtt\x18\x0e \x01(\x08\x12\x11\n\thop_start\x18\x0f \x01(\r\"[\n\x08Priority\x12\t\n\x05UNSET\x10\x00\x12\x07\n\x03MIN\x10\x01\x12\x0e\n\nBACKGROUND\x10\n\x12\x0b\n\x07\x44\x45\x46\x41ULT\x10@\x12\x0c\n\x08RELIABLE\x10\x46\x12\x07\n\x03\x41\x43K\x10x\x12\x07\n\x03MAX\x10\x7f\"B\n\x07\x44\x65layed\x12\x0c\n\x08NO_DELAY\x10\x00\x12\x15\n\x11\x44\x45LAYED_BROADCAST\x10\x01\x12\x12\n\x0e\x44\x45LAYED_DIRECT\x10\x02\x42\x11\n\x0fpayload_variant\"\xfe\x01\n\x08NodeInfo\x12\x0b\n\x03num\x18\x01 \x01(\r\x12\x1e\n\x04user\x18\x02 \x01(\x0b\x32\x10.meshtastic.User\x12&\n\x08position\x18\x03 \x01(\x0b\x32\x14.meshtastic.Position\x12\x0b\n\x03snr\x18\x04 \x01(\x02\x12\x12\n\nlast_heard\x18\x05 \x01(\x07\x12\x31\n\x0e\x64\x65vice_metrics\x18\x06 \x01(\x0b\x32\x19.meshtastic.DeviceMetrics\x12\x0f\n\x07\x63hannel\x18\x07 \x01(\r\x12\x10\n\x08via_mqtt\x18\x08 \x01(\x08\x12\x11\n\thops_away\x18\t \x01(\r\x12\x13\n\x0bis_favorite\x18\n \x01(\x08\"P\n\nMyNodeInfo\x12\x13\n\x0bmy_node_num\x18\x01 \x01(\r\x12\x14\n\x0creboot_count\x18\x08 \x01(\r\x12\x17\n\x0fmin_app_version\x18\x0b \x01(\r\"\xc0\x01\n\tLogRecord\x12\x0f\n\x07message\x18\x01 \x01(\t\x12\x0c\n\x04time\x18\x02 \x01(\x07\x12\x0e\n\x06source\x18\x03 \x01(\t\x12*\n\x05level\x18\x04 \x01(\x0e\x32\x1b.meshtastic.LogRecord.Level\"X\n\x05Level\x12\t\n\x05UNSET\x10\x00\x12\x0c\n\x08\x43RITICAL\x10\x32\x12\t\n\x05\x45RROR\x10(\x12\x0b\n\x07WARNING\x10\x1e\x12\x08\n\x04INFO\x10\x14\x12\t\n\x05\x44\x45\x42UG\x10\n\x12\t\n\x05TRACE\x10\x05\"P\n\x0bQueueStatus\x12\x0b\n\x03res\x18\x01 \x01(\x05\x12\x0c\n\x04\x66ree\x18\x02 \x01(\r\x12\x0e\n\x06maxlen\x18\x03 \x01(\r\x12\x16\n\x0emesh_packet_id\x18\x04 \x01(\r\"\xdb\x04\n\tFromRadio\x12\n\n\x02id\x18\x01 \x01(\r\x12(\n\x06packet\x18\x02 \x01(\x0b\x32\x16.meshtastic.MeshPacketH\x00\x12)\n\x07my_info\x18\x03 \x01(\x0b\x32\x16.meshtastic.MyNodeInfoH\x00\x12)\n\tnode_info\x18\x04 \x01(\x0b\x32\x14.meshtastic.NodeInfoH\x00\x12$\n\x06\x63onfig\x18\x05 \x01(\x0b\x32\x12.meshtastic.ConfigH\x00\x12+\n\nlog_record\x18\x06 \x01(\x0b\x32\x15.meshtastic.LogRecordH\x00\x12\x1c\n\x12\x63onfig_complete_id\x18\x07 \x01(\rH\x00\x12\x12\n\x08rebooted\x18\x08 \x01(\x08H\x00\x12\x30\n\x0cmoduleConfig\x18\t \x01(\x0b\x32\x18.meshtastic.ModuleConfigH\x00\x12&\n\x07\x63hannel\x18\n \x01(\x0b\x32\x13.meshtastic.ChannelH\x00\x12.\n\x0bqueueStatus\x18\x0b \x01(\x0b\x32\x17.meshtastic.QueueStatusH\x00\x12*\n\x0cxmodemPacket\x18\x0c \x01(\x0b\x32\x12.meshtastic.XModemH\x00\x12.\n\x08metadata\x18\r \x01(\x0b\x32\x1a.meshtastic.DeviceMetadataH\x00\x12\x44\n\x16mqttClientProxyMessage\x18\x0e \x01(\x0b\x32\".meshtastic.MqttClientProxyMessageH\x00\x42\x11\n\x0fpayload_variant\"\x94\x02\n\x07ToRadio\x12(\n\x06packet\x18\x01 \x01(\x0b\x32\x16.meshtastic.MeshPacketH\x00\x12\x18\n\x0ewant_config_id\x18\x03 \x01(\rH\x00\x12\x14\n\ndisconnect\x18\x04 \x01(\x08H\x00\x12*\n\x0cxmodemPacket\x18\x05 \x01(\x0b\x32\x12.meshtastic.XModemH\x00\x12\x44\n\x16mqttClientProxyMessage\x18\x06 \x01(\x0b\x32\".meshtastic.MqttClientProxyMessageH\x00\x12*\n\theartbeat\x18\x07 \x01(\x0b\x32\x15.meshtastic.HeartbeatH\x00\x42\x11\n\x0fpayload_variant\"@\n\nCompressed\x12$\n\x07portnum\x18\x01 \x01(\x0e\x32\x13.meshtastic.PortNum\x12\x0c\n\x04\x64\x61ta\x18\x02 \x01(\x0c\"\x87\x01\n\x0cNeighborInfo\x12\x0f\n\x07node_id\x18\x01 \x01(\r\x12\x17\n\x0flast_sent_by_id\x18\x02 \x01(\r\x12$\n\x1cnode_broadcast_interval_secs\x18\x03 \x01(\r\x12\'\n\tneighbors\x18\x04 \x03(\x0b\x32\x14.meshtastic.Neighbor\"d\n\x08Neighbor\x12\x0f\n\x07node_id\x18\x01 \x01(\r\x12\x0b\n\x03snr\x18\x02 \x01(\x02\x12\x14\n\x0clast_rx_time\x18\x03 \x01(\x07\x12$\n\x1cnode_broadcast_interval_secs\x18\x04 \x01(\r\"\xad\x02\n\x0e\x44\x65viceMetadata\x12\x18\n\x10\x66irmware_version\x18\x01 \x01(\t\x12\x1c\n\x14\x64\x65vice_state_version\x18\x02 \x01(\r\x12\x13\n\x0b\x63\x61nShutdown\x18\x03 \x01(\x08\x12\x0f\n\x07hasWifi\x18\x04 \x01(\x08\x12\x14\n\x0chasBluetooth\x18\x05 \x01(\x08\x12\x13\n\x0bhasEthernet\x18\x06 \x01(\x08\x12\x32\n\x04role\x18\x07 \x01(\x0e\x32$.meshtastic.Config.DeviceConfig.Role\x12\x16\n\x0eposition_flags\x18\x08 \x01(\r\x12+\n\x08hw_model\x18\t \x01(\x0e\x32\x19.meshtastic.HardwareModel\x12\x19\n\x11hasRemoteHardware\x18\n \x01(\x08\"\x0b\n\tHeartbeat\"U\n\x15NodeRemoteHardwarePin\x12\x10\n\x08node_num\x18\x01 \x01(\r\x12*\n\x03pin\x18\x02 \x01(\x0b\x32\x1d.meshtastic.RemoteHardwarePin*\x95\x08\n\rHardwareModel\x12\t\n\x05UNSET\x10\x00\x12\x0c\n\x08TLORA_V2\x10\x01\x12\x0c\n\x08TLORA_V1\x10\x02\x12\x12\n\x0eTLORA_V2_1_1P6\x10\x03\x12\t\n\x05TBEAM\x10\x04\x12\x0f\n\x0bHELTEC_V2_0\x10\x05\x12\x0e\n\nTBEAM_V0P7\x10\x06\x12\n\n\x06T_ECHO\x10\x07\x12\x10\n\x0cTLORA_V1_1P3\x10\x08\x12\x0b\n\x07RAK4631\x10\t\x12\x0f\n\x0bHELTEC_V2_1\x10\n\x12\r\n\tHELTEC_V1\x10\x0b\x12\x18\n\x14LILYGO_TBEAM_S3_CORE\x10\x0c\x12\x0c\n\x08RAK11200\x10\r\x12\x0b\n\x07NANO_G1\x10\x0e\x12\x12\n\x0eTLORA_V2_1_1P8\x10\x0f\x12\x0f\n\x0bTLORA_T3_S3\x10\x10\x12\x14\n\x10NANO_G1_EXPLORER\x10\x11\x12\x11\n\rNANO_G2_ULTRA\x10\x12\x12\r\n\tLORA_TYPE\x10\x13\x12\x0e\n\nSTATION_G1\x10\x19\x12\x0c\n\x08RAK11310\x10\x1a\x12\x14\n\x10SENSELORA_RP2040\x10\x1b\x12\x10\n\x0cSENSELORA_S3\x10\x1c\x12\r\n\tCANARYONE\x10\x1d\x12\x0f\n\x0bRP2040_LORA\x10\x1e\x12\x0e\n\nSTATION_G2\x10\x1f\x12\x11\n\rLORA_RELAY_V1\x10 \x12\x0e\n\nNRF52840DK\x10!\x12\x07\n\x03PPR\x10\"\x12\x0f\n\x0bGENIEBLOCKS\x10#\x12\x11\n\rNRF52_UNKNOWN\x10$\x12\r\n\tPORTDUINO\x10%\x12\x0f\n\x0b\x41NDROID_SIM\x10&\x12\n\n\x06\x44IY_V1\x10\'\x12\x15\n\x11NRF52840_PCA10059\x10(\x12\n\n\x06\x44R_DEV\x10)\x12\x0b\n\x07M5STACK\x10*\x12\r\n\tHELTEC_V3\x10+\x12\x11\n\rHELTEC_WSL_V3\x10,\x12\x13\n\x0f\x42\x45TAFPV_2400_TX\x10-\x12\x17\n\x13\x42\x45TAFPV_900_NANO_TX\x10.\x12\x0c\n\x08RPI_PICO\x10/\x12\x1b\n\x17HELTEC_WIRELESS_TRACKER\x10\x30\x12\x19\n\x15HELTEC_WIRELESS_PAPER\x10\x31\x12\n\n\x06T_DECK\x10\x32\x12\x0e\n\nT_WATCH_S3\x10\x33\x12\x11\n\rPICOMPUTER_S3\x10\x34\x12\x0f\n\x0bHELTEC_HT62\x10\x35\x12\x12\n\x0e\x45\x42YTE_ESP32_S3\x10\x36\x12\x11\n\rESP32_S3_PICO\x10\x37\x12\r\n\tCHATTER_2\x10\x38\x12\x1e\n\x1aHELTEC_WIRELESS_PAPER_V1_0\x10\x39\x12 \n\x1cHELTEC_WIRELESS_TRACKER_V1_0\x10:\x12\x0b\n\x07UNPHONE\x10;\x12\x0c\n\x08TD_LORAC\x10<\x12\x13\n\x0f\x43\x44\x45\x42YTE_EORA_S3\x10=\x12\x0f\n\x0bTWC_MESH_V4\x10>\x12\x0f\n\nPRIVATE_HW\x10\xff\x01*,\n\tConstants\x12\x08\n\x04ZERO\x10\x00\x12\x15\n\x10\x44\x41TA_PAYLOAD_LEN\x10\xed\x01*\xee\x01\n\x11\x43riticalErrorCode\x12\x08\n\x04NONE\x10\x00\x12\x0f\n\x0bTX_WATCHDOG\x10\x01\x12\x14\n\x10SLEEP_ENTER_WAIT\x10\x02\x12\x0c\n\x08NO_RADIO\x10\x03\x12\x0f\n\x0bUNSPECIFIED\x10\x04\x12\x15\n\x11UBLOX_UNIT_FAILED\x10\x05\x12\r\n\tNO_AXP192\x10\x06\x12\x19\n\x15INVALID_RADIO_SETTING\x10\x07\x12\x13\n\x0fTRANSMIT_FAILED\x10\x08\x12\x0c\n\x08\x42ROWNOUT\x10\t\x12\x12\n\x0eSX1262_FAILURE\x10\n\x12\x11\n\rRADIO_SPI_BUG\x10\x0b\x42_\n\x13\x63om.geeksville.meshB\nMeshProtosZ\"github.com/meshtastic/go/generated\xaa\x02\x14Meshtastic.Protobufs\xba\x02\x00\x62\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x15meshtastic/mesh.proto\x12\nmeshtastic\x1a\x18meshtastic/channel.proto\x1a\x17meshtastic/config.proto\x1a\x1emeshtastic/module_config.proto\x1a\x19meshtastic/portnums.proto\x1a\x1ameshtastic/telemetry.proto\x1a\x17meshtastic/xmodem.proto\"\xe5\x05\n\x08Position\x12\x12\n\nlatitude_i\x18\x01 \x01(\x0f\x12\x13\n\x0blongitude_i\x18\x02 \x01(\x0f\x12\x10\n\x08\x61ltitude\x18\x03 \x01(\x05\x12\x0c\n\x04time\x18\x04 \x01(\x07\x12\x37\n\x0flocation_source\x18\x05 \x01(\x0e\x32\x1e.meshtastic.Position.LocSource\x12\x37\n\x0f\x61ltitude_source\x18\x06 \x01(\x0e\x32\x1e.meshtastic.Position.AltSource\x12\x11\n\ttimestamp\x18\x07 \x01(\x07\x12\x1f\n\x17timestamp_millis_adjust\x18\x08 \x01(\x05\x12\x14\n\x0c\x61ltitude_hae\x18\t \x01(\x11\x12#\n\x1b\x61ltitude_geoidal_separation\x18\n \x01(\x11\x12\x0c\n\x04PDOP\x18\x0b \x01(\r\x12\x0c\n\x04HDOP\x18\x0c \x01(\r\x12\x0c\n\x04VDOP\x18\r \x01(\r\x12\x14\n\x0cgps_accuracy\x18\x0e \x01(\r\x12\x14\n\x0cground_speed\x18\x0f \x01(\r\x12\x14\n\x0cground_track\x18\x10 \x01(\r\x12\x13\n\x0b\x66ix_quality\x18\x11 \x01(\r\x12\x10\n\x08\x66ix_type\x18\x12 \x01(\r\x12\x14\n\x0csats_in_view\x18\x13 \x01(\r\x12\x11\n\tsensor_id\x18\x14 \x01(\r\x12\x13\n\x0bnext_update\x18\x15 \x01(\r\x12\x12\n\nseq_number\x18\x16 \x01(\r\x12\x16\n\x0eprecision_bits\x18\x17 \x01(\r\"N\n\tLocSource\x12\r\n\tLOC_UNSET\x10\x00\x12\x0e\n\nLOC_MANUAL\x10\x01\x12\x10\n\x0cLOC_INTERNAL\x10\x02\x12\x10\n\x0cLOC_EXTERNAL\x10\x03\"b\n\tAltSource\x12\r\n\tALT_UNSET\x10\x00\x12\x0e\n\nALT_MANUAL\x10\x01\x12\x10\n\x0c\x41LT_INTERNAL\x10\x02\x12\x10\n\x0c\x41LT_EXTERNAL\x10\x03\x12\x12\n\x0e\x41LT_BAROMETRIC\x10\x04\"\xc4\x01\n\x04User\x12\n\n\x02id\x18\x01 \x01(\t\x12\x11\n\tlong_name\x18\x02 \x01(\t\x12\x12\n\nshort_name\x18\x03 \x01(\t\x12\x13\n\x07macaddr\x18\x04 \x01(\x0c\x42\x02\x18\x01\x12+\n\x08hw_model\x18\x05 \x01(\x0e\x32\x19.meshtastic.HardwareModel\x12\x13\n\x0bis_licensed\x18\x06 \x01(\x08\x12\x32\n\x04role\x18\x07 \x01(\x0e\x32$.meshtastic.Config.DeviceConfig.Role\"\x1f\n\x0eRouteDiscovery\x12\r\n\x05route\x18\x01 \x03(\x07\"\xfc\x02\n\x07Routing\x12\x33\n\rroute_request\x18\x01 \x01(\x0b\x32\x1a.meshtastic.RouteDiscoveryH\x00\x12\x31\n\x0broute_reply\x18\x02 \x01(\x0b\x32\x1a.meshtastic.RouteDiscoveryH\x00\x12\x31\n\x0c\x65rror_reason\x18\x03 \x01(\x0e\x32\x19.meshtastic.Routing.ErrorH\x00\"\xca\x01\n\x05\x45rror\x12\x08\n\x04NONE\x10\x00\x12\x0c\n\x08NO_ROUTE\x10\x01\x12\x0b\n\x07GOT_NAK\x10\x02\x12\x0b\n\x07TIMEOUT\x10\x03\x12\x10\n\x0cNO_INTERFACE\x10\x04\x12\x12\n\x0eMAX_RETRANSMIT\x10\x05\x12\x0e\n\nNO_CHANNEL\x10\x06\x12\r\n\tTOO_LARGE\x10\x07\x12\x0f\n\x0bNO_RESPONSE\x10\x08\x12\x14\n\x10\x44UTY_CYCLE_LIMIT\x10\t\x12\x0f\n\x0b\x42\x41\x44_REQUEST\x10 \x12\x12\n\x0eNOT_AUTHORIZED\x10!B\t\n\x07variant\"\xa7\x01\n\x04\x44\x61ta\x12$\n\x07portnum\x18\x01 \x01(\x0e\x32\x13.meshtastic.PortNum\x12\x0f\n\x07payload\x18\x02 \x01(\x0c\x12\x15\n\rwant_response\x18\x03 \x01(\x08\x12\x0c\n\x04\x64\x65st\x18\x04 \x01(\x07\x12\x0e\n\x06source\x18\x05 \x01(\x07\x12\x12\n\nrequest_id\x18\x06 \x01(\x07\x12\x10\n\x08reply_id\x18\x07 \x01(\x07\x12\r\n\x05\x65moji\x18\x08 \x01(\x07\"\x93\x01\n\x08Waypoint\x12\n\n\x02id\x18\x01 \x01(\r\x12\x12\n\nlatitude_i\x18\x02 \x01(\x0f\x12\x13\n\x0blongitude_i\x18\x03 \x01(\x0f\x12\x0e\n\x06\x65xpire\x18\x04 \x01(\r\x12\x11\n\tlocked_to\x18\x05 \x01(\r\x12\x0c\n\x04name\x18\x06 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x07 \x01(\t\x12\x0c\n\x04icon\x18\x08 \x01(\x07\"l\n\x16MqttClientProxyMessage\x12\r\n\x05topic\x18\x01 \x01(\t\x12\x0e\n\x04\x64\x61ta\x18\x02 \x01(\x0cH\x00\x12\x0e\n\x04text\x18\x03 \x01(\tH\x00\x12\x10\n\x08retained\x18\x04 \x01(\x08\x42\x11\n\x0fpayload_variant\"\x95\x04\n\nMeshPacket\x12\x0c\n\x04\x66rom\x18\x01 \x01(\x07\x12\n\n\x02to\x18\x02 \x01(\x07\x12\x0f\n\x07\x63hannel\x18\x03 \x01(\r\x12#\n\x07\x64\x65\x63oded\x18\x04 \x01(\x0b\x32\x10.meshtastic.DataH\x00\x12\x13\n\tencrypted\x18\x05 \x01(\x0cH\x00\x12\n\n\x02id\x18\x06 \x01(\x07\x12\x0f\n\x07rx_time\x18\x07 \x01(\x07\x12\x0e\n\x06rx_snr\x18\x08 \x01(\x02\x12\x11\n\thop_limit\x18\t \x01(\r\x12\x10\n\x08want_ack\x18\n \x01(\x08\x12\x31\n\x08priority\x18\x0b \x01(\x0e\x32\x1f.meshtastic.MeshPacket.Priority\x12\x0f\n\x07rx_rssi\x18\x0c \x01(\x05\x12\x33\n\x07\x64\x65layed\x18\r \x01(\x0e\x32\x1e.meshtastic.MeshPacket.DelayedB\x02\x18\x01\x12\x10\n\x08via_mqtt\x18\x0e \x01(\x08\x12\x11\n\thop_start\x18\x0f \x01(\r\"[\n\x08Priority\x12\t\n\x05UNSET\x10\x00\x12\x07\n\x03MIN\x10\x01\x12\x0e\n\nBACKGROUND\x10\n\x12\x0b\n\x07\x44\x45\x46\x41ULT\x10@\x12\x0c\n\x08RELIABLE\x10\x46\x12\x07\n\x03\x41\x43K\x10x\x12\x07\n\x03MAX\x10\x7f\"B\n\x07\x44\x65layed\x12\x0c\n\x08NO_DELAY\x10\x00\x12\x15\n\x11\x44\x45LAYED_BROADCAST\x10\x01\x12\x12\n\x0e\x44\x45LAYED_DIRECT\x10\x02\x42\x11\n\x0fpayload_variant\"\xfe\x01\n\x08NodeInfo\x12\x0b\n\x03num\x18\x01 \x01(\r\x12\x1e\n\x04user\x18\x02 \x01(\x0b\x32\x10.meshtastic.User\x12&\n\x08position\x18\x03 \x01(\x0b\x32\x14.meshtastic.Position\x12\x0b\n\x03snr\x18\x04 \x01(\x02\x12\x12\n\nlast_heard\x18\x05 \x01(\x07\x12\x31\n\x0e\x64\x65vice_metrics\x18\x06 \x01(\x0b\x32\x19.meshtastic.DeviceMetrics\x12\x0f\n\x07\x63hannel\x18\x07 \x01(\r\x12\x10\n\x08via_mqtt\x18\x08 \x01(\x08\x12\x11\n\thops_away\x18\t \x01(\r\x12\x13\n\x0bis_favorite\x18\n \x01(\x08\"P\n\nMyNodeInfo\x12\x13\n\x0bmy_node_num\x18\x01 \x01(\r\x12\x14\n\x0creboot_count\x18\x08 \x01(\r\x12\x17\n\x0fmin_app_version\x18\x0b \x01(\r\"\xc0\x01\n\tLogRecord\x12\x0f\n\x07message\x18\x01 \x01(\t\x12\x0c\n\x04time\x18\x02 \x01(\x07\x12\x0e\n\x06source\x18\x03 \x01(\t\x12*\n\x05level\x18\x04 \x01(\x0e\x32\x1b.meshtastic.LogRecord.Level\"X\n\x05Level\x12\t\n\x05UNSET\x10\x00\x12\x0c\n\x08\x43RITICAL\x10\x32\x12\t\n\x05\x45RROR\x10(\x12\x0b\n\x07WARNING\x10\x1e\x12\x08\n\x04INFO\x10\x14\x12\t\n\x05\x44\x45\x42UG\x10\n\x12\t\n\x05TRACE\x10\x05\"P\n\x0bQueueStatus\x12\x0b\n\x03res\x18\x01 \x01(\x05\x12\x0c\n\x04\x66ree\x18\x02 \x01(\r\x12\x0e\n\x06maxlen\x18\x03 \x01(\r\x12\x16\n\x0emesh_packet_id\x18\x04 \x01(\r\"\xdb\x04\n\tFromRadio\x12\n\n\x02id\x18\x01 \x01(\r\x12(\n\x06packet\x18\x02 \x01(\x0b\x32\x16.meshtastic.MeshPacketH\x00\x12)\n\x07my_info\x18\x03 \x01(\x0b\x32\x16.meshtastic.MyNodeInfoH\x00\x12)\n\tnode_info\x18\x04 \x01(\x0b\x32\x14.meshtastic.NodeInfoH\x00\x12$\n\x06\x63onfig\x18\x05 \x01(\x0b\x32\x12.meshtastic.ConfigH\x00\x12+\n\nlog_record\x18\x06 \x01(\x0b\x32\x15.meshtastic.LogRecordH\x00\x12\x1c\n\x12\x63onfig_complete_id\x18\x07 \x01(\rH\x00\x12\x12\n\x08rebooted\x18\x08 \x01(\x08H\x00\x12\x30\n\x0cmoduleConfig\x18\t \x01(\x0b\x32\x18.meshtastic.ModuleConfigH\x00\x12&\n\x07\x63hannel\x18\n \x01(\x0b\x32\x13.meshtastic.ChannelH\x00\x12.\n\x0bqueueStatus\x18\x0b \x01(\x0b\x32\x17.meshtastic.QueueStatusH\x00\x12*\n\x0cxmodemPacket\x18\x0c \x01(\x0b\x32\x12.meshtastic.XModemH\x00\x12.\n\x08metadata\x18\r \x01(\x0b\x32\x1a.meshtastic.DeviceMetadataH\x00\x12\x44\n\x16mqttClientProxyMessage\x18\x0e \x01(\x0b\x32\".meshtastic.MqttClientProxyMessageH\x00\x42\x11\n\x0fpayload_variant\"\x94\x02\n\x07ToRadio\x12(\n\x06packet\x18\x01 \x01(\x0b\x32\x16.meshtastic.MeshPacketH\x00\x12\x18\n\x0ewant_config_id\x18\x03 \x01(\rH\x00\x12\x14\n\ndisconnect\x18\x04 \x01(\x08H\x00\x12*\n\x0cxmodemPacket\x18\x05 \x01(\x0b\x32\x12.meshtastic.XModemH\x00\x12\x44\n\x16mqttClientProxyMessage\x18\x06 \x01(\x0b\x32\".meshtastic.MqttClientProxyMessageH\x00\x12*\n\theartbeat\x18\x07 \x01(\x0b\x32\x15.meshtastic.HeartbeatH\x00\x42\x11\n\x0fpayload_variant\"@\n\nCompressed\x12$\n\x07portnum\x18\x01 \x01(\x0e\x32\x13.meshtastic.PortNum\x12\x0c\n\x04\x64\x61ta\x18\x02 \x01(\x0c\"\x87\x01\n\x0cNeighborInfo\x12\x0f\n\x07node_id\x18\x01 \x01(\r\x12\x17\n\x0flast_sent_by_id\x18\x02 \x01(\r\x12$\n\x1cnode_broadcast_interval_secs\x18\x03 \x01(\r\x12\'\n\tneighbors\x18\x04 \x03(\x0b\x32\x14.meshtastic.Neighbor\"d\n\x08Neighbor\x12\x0f\n\x07node_id\x18\x01 \x01(\r\x12\x0b\n\x03snr\x18\x02 \x01(\x02\x12\x14\n\x0clast_rx_time\x18\x03 \x01(\x07\x12$\n\x1cnode_broadcast_interval_secs\x18\x04 \x01(\r\"\xad\x02\n\x0e\x44\x65viceMetadata\x12\x18\n\x10\x66irmware_version\x18\x01 \x01(\t\x12\x1c\n\x14\x64\x65vice_state_version\x18\x02 \x01(\r\x12\x13\n\x0b\x63\x61nShutdown\x18\x03 \x01(\x08\x12\x0f\n\x07hasWifi\x18\x04 \x01(\x08\x12\x14\n\x0chasBluetooth\x18\x05 \x01(\x08\x12\x13\n\x0bhasEthernet\x18\x06 \x01(\x08\x12\x32\n\x04role\x18\x07 \x01(\x0e\x32$.meshtastic.Config.DeviceConfig.Role\x12\x16\n\x0eposition_flags\x18\x08 \x01(\r\x12+\n\x08hw_model\x18\t \x01(\x0e\x32\x19.meshtastic.HardwareModel\x12\x19\n\x11hasRemoteHardware\x18\n \x01(\x08\"\x0b\n\tHeartbeat\"U\n\x15NodeRemoteHardwarePin\x12\x10\n\x08node_num\x18\x01 \x01(\r\x12*\n\x03pin\x18\x02 \x01(\x0b\x32\x1d.meshtastic.RemoteHardwarePin*\xba\x08\n\rHardwareModel\x12\t\n\x05UNSET\x10\x00\x12\x0c\n\x08TLORA_V2\x10\x01\x12\x0c\n\x08TLORA_V1\x10\x02\x12\x12\n\x0eTLORA_V2_1_1P6\x10\x03\x12\t\n\x05TBEAM\x10\x04\x12\x0f\n\x0bHELTEC_V2_0\x10\x05\x12\x0e\n\nTBEAM_V0P7\x10\x06\x12\n\n\x06T_ECHO\x10\x07\x12\x10\n\x0cTLORA_V1_1P3\x10\x08\x12\x0b\n\x07RAK4631\x10\t\x12\x0f\n\x0bHELTEC_V2_1\x10\n\x12\r\n\tHELTEC_V1\x10\x0b\x12\x18\n\x14LILYGO_TBEAM_S3_CORE\x10\x0c\x12\x0c\n\x08RAK11200\x10\r\x12\x0b\n\x07NANO_G1\x10\x0e\x12\x12\n\x0eTLORA_V2_1_1P8\x10\x0f\x12\x0f\n\x0bTLORA_T3_S3\x10\x10\x12\x14\n\x10NANO_G1_EXPLORER\x10\x11\x12\x11\n\rNANO_G2_ULTRA\x10\x12\x12\r\n\tLORA_TYPE\x10\x13\x12\x0b\n\x07WIPHONE\x10\x14\x12\x0e\n\nSTATION_G1\x10\x19\x12\x0c\n\x08RAK11310\x10\x1a\x12\x14\n\x10SENSELORA_RP2040\x10\x1b\x12\x10\n\x0cSENSELORA_S3\x10\x1c\x12\r\n\tCANARYONE\x10\x1d\x12\x0f\n\x0bRP2040_LORA\x10\x1e\x12\x0e\n\nSTATION_G2\x10\x1f\x12\x11\n\rLORA_RELAY_V1\x10 \x12\x0e\n\nNRF52840DK\x10!\x12\x07\n\x03PPR\x10\"\x12\x0f\n\x0bGENIEBLOCKS\x10#\x12\x11\n\rNRF52_UNKNOWN\x10$\x12\r\n\tPORTDUINO\x10%\x12\x0f\n\x0b\x41NDROID_SIM\x10&\x12\n\n\x06\x44IY_V1\x10\'\x12\x15\n\x11NRF52840_PCA10059\x10(\x12\n\n\x06\x44R_DEV\x10)\x12\x0b\n\x07M5STACK\x10*\x12\r\n\tHELTEC_V3\x10+\x12\x11\n\rHELTEC_WSL_V3\x10,\x12\x13\n\x0f\x42\x45TAFPV_2400_TX\x10-\x12\x17\n\x13\x42\x45TAFPV_900_NANO_TX\x10.\x12\x0c\n\x08RPI_PICO\x10/\x12\x1b\n\x17HELTEC_WIRELESS_TRACKER\x10\x30\x12\x19\n\x15HELTEC_WIRELESS_PAPER\x10\x31\x12\n\n\x06T_DECK\x10\x32\x12\x0e\n\nT_WATCH_S3\x10\x33\x12\x11\n\rPICOMPUTER_S3\x10\x34\x12\x0f\n\x0bHELTEC_HT62\x10\x35\x12\x12\n\x0e\x45\x42YTE_ESP32_S3\x10\x36\x12\x11\n\rESP32_S3_PICO\x10\x37\x12\r\n\tCHATTER_2\x10\x38\x12\x1e\n\x1aHELTEC_WIRELESS_PAPER_V1_0\x10\x39\x12 \n\x1cHELTEC_WIRELESS_TRACKER_V1_0\x10:\x12\x0b\n\x07UNPHONE\x10;\x12\x0c\n\x08TD_LORAC\x10<\x12\x13\n\x0f\x43\x44\x45\x42YTE_EORA_S3\x10=\x12\x0f\n\x0bTWC_MESH_V4\x10>\x12\x16\n\x12NRF52_PROMICRO_DIY\x10?\x12\x0f\n\nPRIVATE_HW\x10\xff\x01*,\n\tConstants\x12\x08\n\x04ZERO\x10\x00\x12\x15\n\x10\x44\x41TA_PAYLOAD_LEN\x10\xed\x01*\xee\x01\n\x11\x43riticalErrorCode\x12\x08\n\x04NONE\x10\x00\x12\x0f\n\x0bTX_WATCHDOG\x10\x01\x12\x14\n\x10SLEEP_ENTER_WAIT\x10\x02\x12\x0c\n\x08NO_RADIO\x10\x03\x12\x0f\n\x0bUNSPECIFIED\x10\x04\x12\x15\n\x11UBLOX_UNIT_FAILED\x10\x05\x12\r\n\tNO_AXP192\x10\x06\x12\x19\n\x15INVALID_RADIO_SETTING\x10\x07\x12\x13\n\x0fTRANSMIT_FAILED\x10\x08\x12\x0c\n\x08\x42ROWNOUT\x10\t\x12\x12\n\x0eSX1262_FAILURE\x10\n\x12\x11\n\rRADIO_SPI_BUG\x10\x0b\x42_\n\x13\x63om.geeksville.meshB\nMeshProtosZ\"github.com/meshtastic/go/generated\xaa\x02\x14Meshtastic.Protobufs\xba\x02\x00\x62\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'meshtastic.mesh_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'\n\023com.geeksville.meshB\nMeshProtosZ\"github.com/meshtastic/go/generated\252\002\024Meshtastic.Protobufs\272\002\000'
   _USER.fields_by_name['macaddr']._options = None
   _USER.fields_by_name['macaddr']._serialized_options = b'\030\001'
   _MESHPACKET.fields_by_name['delayed']._options = None
   _MESHPACKET.fields_by_name['delayed']._serialized_options = b'\030\001'
   _HARDWAREMODEL._serialized_start=4737
-  _HARDWAREMODEL._serialized_end=5782
-  _CONSTANTS._serialized_start=5784
-  _CONSTANTS._serialized_end=5828
-  _CRITICALERRORCODE._serialized_start=5831
-  _CRITICALERRORCODE._serialized_end=6069
+  _HARDWAREMODEL._serialized_end=5819
+  _CONSTANTS._serialized_start=5821
+  _CONSTANTS._serialized_end=5865
+  _CRITICALERRORCODE._serialized_start=5868
+  _CRITICALERRORCODE._serialized_end=6106
   _POSITION._serialized_start=201
   _POSITION._serialized_end=942
   _POSITION_LOCSOURCE._serialized_start=764
   _POSITION_LOCSOURCE._serialized_end=842
   _POSITION_ALTSOURCE._serialized_start=844
   _POSITION_ALTSOURCE._serialized_end=942
   _USER._serialized_start=945
```

### Comparing `meshtastic-2.3.8/meshtastic/mesh_pb2.pyi` & `meshtastic-2.3.9/meshtastic/mesh_pb2.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -108,14 +108,18 @@
     """
     B&Q Consulting Nano G2 Ultra: https://wiki.uniteng.com/en/meshtastic/nano-g2-ultra
     """
     LORA_TYPE: _HardwareModel.ValueType  # 19
     """
     LoRAType device: https://loratype.org/
     """
+    WIPHONE: _HardwareModel.ValueType  # 20
+    """
+    wiphone https://www.wiphone.io/
+    """
     STATION_G1: _HardwareModel.ValueType  # 25
     """
     B&Q Consulting Station Edition G1: https://uniteng.com/wiki/doku.php?id=meshtastic:station
     """
     RAK11310: _HardwareModel.ValueType  # 26
     """
     RAK11310 (RP2040 + SX1262)
@@ -272,14 +276,19 @@
     CDEBYTE EoRa-S3 board using their own MM modules, clone of LILYGO T3S3
     """
     TWC_MESH_V4: _HardwareModel.ValueType  # 62
     """
     TWC_MESH_V4 
     Adafruit NRF52840 feather express with SX1262, SSD1306 OLED and NEO6M GPS
     """
+    NRF52_PROMICRO_DIY: _HardwareModel.ValueType  # 63
+    """
+    NRF52_PROMICRO_DIY
+    Promicro NRF52840 with SX1262/LLCC68, SSD1306 OLED and NEO6M GPS
+    """
     PRIVATE_HW: _HardwareModel.ValueType  # 255
     """
     ------------------------------------------------------------------------------------------------------------------------------------------
     Reserved ID For developing private Ports. These will show up in live traffic sparsely, so we can use a high number. Keep it within 8 bits.
     ------------------------------------------------------------------------------------------------------------------------------------------
     """
 
@@ -369,14 +378,18 @@
 """
 B&Q Consulting Nano G2 Ultra: https://wiki.uniteng.com/en/meshtastic/nano-g2-ultra
 """
 LORA_TYPE: HardwareModel.ValueType  # 19
 """
 LoRAType device: https://loratype.org/
 """
+WIPHONE: HardwareModel.ValueType  # 20
+"""
+wiphone https://www.wiphone.io/
+"""
 STATION_G1: HardwareModel.ValueType  # 25
 """
 B&Q Consulting Station Edition G1: https://uniteng.com/wiki/doku.php?id=meshtastic:station
 """
 RAK11310: HardwareModel.ValueType  # 26
 """
 RAK11310 (RP2040 + SX1262)
@@ -533,14 +546,19 @@
 CDEBYTE EoRa-S3 board using their own MM modules, clone of LILYGO T3S3
 """
 TWC_MESH_V4: HardwareModel.ValueType  # 62
 """
 TWC_MESH_V4 
 Adafruit NRF52840 feather express with SX1262, SSD1306 OLED and NEO6M GPS
 """
+NRF52_PROMICRO_DIY: HardwareModel.ValueType  # 63
+"""
+NRF52_PROMICRO_DIY
+Promicro NRF52840 with SX1262/LLCC68, SSD1306 OLED and NEO6M GPS
+"""
 PRIVATE_HW: HardwareModel.ValueType  # 255
 """
 ------------------------------------------------------------------------------------------------------------------------------------------
 Reserved ID For developing private Ports. These will show up in live traffic sparsely, so we can use a high number. Keep it within 8 bits.
 ------------------------------------------------------------------------------------------------------------------------------------------
 """
 global___HardwareModel = HardwareModel
```

### Comparing `meshtastic-2.3.8/meshtastic/module_config_pb2.py` & `meshtastic-2.3.9/meshtastic/module_config_pb2.py`

 * *Files identical despite different names*

### Comparing `meshtastic-2.3.8/meshtastic/module_config_pb2.pyi` & `meshtastic-2.3.9/meshtastic/module_config_pb2.pyi`

 * *Files identical despite different names*

### Comparing `meshtastic-2.3.8/meshtastic/mqtt_pb2.py` & `meshtastic-2.3.9/meshtastic/mqtt_pb2.py`

 * *Files identical despite different names*

### Comparing `meshtastic-2.3.8/meshtastic/mqtt_pb2.pyi` & `meshtastic-2.3.9/meshtastic/mqtt_pb2.pyi`

 * *Files identical despite different names*

### Comparing `meshtastic-2.3.8/meshtastic/mt_config.py` & `meshtastic-2.3.9/meshtastic/mt_config.py`

 * *Files identical despite different names*

### Comparing `meshtastic-2.3.8/meshtastic/nanopb_pb2.py` & `meshtastic-2.3.9/meshtastic/nanopb_pb2.py`

 * *Files identical despite different names*

### Comparing `meshtastic-2.3.8/meshtastic/nanopb_pb2.pyi` & `meshtastic-2.3.9/meshtastic/nanopb_pb2.pyi`

 * *Files identical despite different names*

### Comparing `meshtastic-2.3.8/meshtastic/node.py` & `meshtastic-2.3.9/meshtastic/node.py`

 * *Files identical despite different names*

### Comparing `meshtastic-2.3.8/meshtastic/paxcount_pb2.py` & `meshtastic-2.3.9/meshtastic/paxcount_pb2.py`

 * *Files identical despite different names*

### Comparing `meshtastic-2.3.8/meshtastic/paxcount_pb2.pyi` & `meshtastic-2.3.9/meshtastic/paxcount_pb2.pyi`

 * *Files identical despite different names*

### Comparing `meshtastic-2.3.8/meshtastic/portnums_pb2.py` & `meshtastic-2.3.9/meshtastic/portnums_pb2.py`

 * *Files identical despite different names*

### Comparing `meshtastic-2.3.8/meshtastic/portnums_pb2.pyi` & `meshtastic-2.3.9/meshtastic/portnums_pb2.pyi`

 * *Files identical despite different names*

### Comparing `meshtastic-2.3.8/meshtastic/remote_hardware.py` & `meshtastic-2.3.9/meshtastic/remote_hardware.py`

 * *Files identical despite different names*

### Comparing `meshtastic-2.3.8/meshtastic/remote_hardware_pb2.py` & `meshtastic-2.3.9/meshtastic/remote_hardware_pb2.py`

 * *Files identical despite different names*

### Comparing `meshtastic-2.3.8/meshtastic/remote_hardware_pb2.pyi` & `meshtastic-2.3.9/meshtastic/remote_hardware_pb2.pyi`

 * *Files identical despite different names*

### Comparing `meshtastic-2.3.8/meshtastic/rtttl_pb2.py` & `meshtastic-2.3.9/meshtastic/rtttl_pb2.py`

 * *Files identical despite different names*

### Comparing `meshtastic-2.3.8/meshtastic/rtttl_pb2.pyi` & `meshtastic-2.3.9/meshtastic/rtttl_pb2.pyi`

 * *Files identical despite different names*

### Comparing `meshtastic-2.3.8/meshtastic/serial_interface.py` & `meshtastic-2.3.9/meshtastic/serial_interface.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,36 +1,38 @@
 """ Serial interface class
 """
 import logging
 import platform
 import time
 
+from typing import Optional
+
 import serial # type: ignore[import-untyped]
 
 import meshtastic.util
 from meshtastic.stream_interface import StreamInterface
 
 if platform.system() != "Windows":
     import termios
 
 
 class SerialInterface(StreamInterface):
     """Interface class for meshtastic devices over a serial link"""
 
-    def __init__(self, devPath=None, debugOut=None, noProto=False, connectNow=True):
+    def __init__(self, devPath: Optional[str]=None, debugOut=None, noProto=False, connectNow=True):
         """Constructor, opens a connection to a specified serial port, or if unspecified try to
         find one Meshtastic device by probing
 
         Keyword Arguments:
             devPath {string} -- A filepath to a device, i.e. /dev/ttyUSB0 (default: {None})
             debugOut {stream} -- If a stream is provided, any debug serial output from the device will be emitted to that stream. (default: {None})
         """
         self.noProto = noProto
 
-        self.devPath = devPath
+        self.devPath: Optional[str] = devPath
 
         if self.devPath is None:
             ports = meshtastic.util.findPorts(True)
             logging.debug(f"ports:{ports}")
             if len(ports) == 0:
                 print("No Serial Meshtastic device detected, attempting TCP connection on localhost.")
                 return
```

### Comparing `meshtastic-2.3.8/meshtastic/storeforward_pb2.py` & `meshtastic-2.3.9/meshtastic/storeforward_pb2.py`

 * *Files identical despite different names*

### Comparing `meshtastic-2.3.8/meshtastic/storeforward_pb2.pyi` & `meshtastic-2.3.9/meshtastic/storeforward_pb2.pyi`

 * *Files identical despite different names*

### Comparing `meshtastic-2.3.8/meshtastic/stream_interface.py` & `meshtastic-2.3.9/meshtastic/stream_interface.py`

 * *Files identical despite different names*

### Comparing `meshtastic-2.3.8/meshtastic/supported_device.py` & `meshtastic-2.3.9/meshtastic/supported_device.py`

 * *Files identical despite different names*

### Comparing `meshtastic-2.3.8/meshtastic/tcp_interface.py` & `meshtastic-2.3.9/meshtastic/tcp_interface.py`

 * *Files identical despite different names*

### Comparing `meshtastic-2.3.8/meshtastic/telemetry_pb2.py` & `meshtastic-2.3.9/meshtastic/telemetry_pb2.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,24 +9,24 @@
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1ameshtastic/telemetry.proto\x12\nmeshtastic\"\x81\x01\n\rDeviceMetrics\x12\x15\n\rbattery_level\x18\x01 \x01(\r\x12\x0f\n\x07voltage\x18\x02 \x01(\x02\x12\x1b\n\x13\x63hannel_utilization\x18\x03 \x01(\x02\x12\x13\n\x0b\x61ir_util_tx\x18\x04 \x01(\x02\x12\x16\n\x0euptime_seconds\x18\x05 \x01(\r\"\xba\x01\n\x12\x45nvironmentMetrics\x12\x13\n\x0btemperature\x18\x01 \x01(\x02\x12\x19\n\x11relative_humidity\x18\x02 \x01(\x02\x12\x1b\n\x13\x62\x61rometric_pressure\x18\x03 \x01(\x02\x12\x16\n\x0egas_resistance\x18\x04 \x01(\x02\x12\x0f\n\x07voltage\x18\x05 \x01(\x02\x12\x0f\n\x07\x63urrent\x18\x06 \x01(\x02\x12\x0b\n\x03iaq\x18\x07 \x01(\r\x12\x10\n\x08\x64istance\x18\x08 \x01(\x02\"\x8c\x01\n\x0cPowerMetrics\x12\x13\n\x0b\x63h1_voltage\x18\x01 \x01(\x02\x12\x13\n\x0b\x63h1_current\x18\x02 \x01(\x02\x12\x13\n\x0b\x63h2_voltage\x18\x03 \x01(\x02\x12\x13\n\x0b\x63h2_current\x18\x04 \x01(\x02\x12\x13\n\x0b\x63h3_voltage\x18\x05 \x01(\x02\x12\x13\n\x0b\x63h3_current\x18\x06 \x01(\x02\"\xbf\x02\n\x11\x41irQualityMetrics\x12\x15\n\rpm10_standard\x18\x01 \x01(\r\x12\x15\n\rpm25_standard\x18\x02 \x01(\r\x12\x16\n\x0epm100_standard\x18\x03 \x01(\r\x12\x1a\n\x12pm10_environmental\x18\x04 \x01(\r\x12\x1a\n\x12pm25_environmental\x18\x05 \x01(\r\x12\x1b\n\x13pm100_environmental\x18\x06 \x01(\r\x12\x16\n\x0eparticles_03um\x18\x07 \x01(\r\x12\x16\n\x0eparticles_05um\x18\x08 \x01(\r\x12\x16\n\x0eparticles_10um\x18\t \x01(\r\x12\x16\n\x0eparticles_25um\x18\n \x01(\r\x12\x16\n\x0eparticles_50um\x18\x0b \x01(\r\x12\x17\n\x0fparticles_100um\x18\x0c \x01(\r\"\x89\x02\n\tTelemetry\x12\x0c\n\x04time\x18\x01 \x01(\x07\x12\x33\n\x0e\x64\x65vice_metrics\x18\x02 \x01(\x0b\x32\x19.meshtastic.DeviceMetricsH\x00\x12=\n\x13\x65nvironment_metrics\x18\x03 \x01(\x0b\x32\x1e.meshtastic.EnvironmentMetricsH\x00\x12<\n\x13\x61ir_quality_metrics\x18\x04 \x01(\x0b\x32\x1d.meshtastic.AirQualityMetricsH\x00\x12\x31\n\rpower_metrics\x18\x05 \x01(\x0b\x32\x18.meshtastic.PowerMetricsH\x00\x42\t\n\x07variant*\xee\x01\n\x13TelemetrySensorType\x12\x10\n\x0cSENSOR_UNSET\x10\x00\x12\n\n\x06\x42ME280\x10\x01\x12\n\n\x06\x42ME680\x10\x02\x12\x0b\n\x07MCP9808\x10\x03\x12\n\n\x06INA260\x10\x04\x12\n\n\x06INA219\x10\x05\x12\n\n\x06\x42MP280\x10\x06\x12\t\n\x05SHTC3\x10\x07\x12\t\n\x05LPS22\x10\x08\x12\x0b\n\x07QMC6310\x10\t\x12\x0b\n\x07QMI8658\x10\n\x12\x0c\n\x08QMC5883L\x10\x0b\x12\t\n\x05SHT31\x10\x0c\x12\x0c\n\x08PMSA003I\x10\r\x12\x0b\n\x07INA3221\x10\x0e\x12\n\n\x06\x42MP085\x10\x0f\x12\x0c\n\x08RCWL9620\x10\x10\x42\x64\n\x13\x63om.geeksville.meshB\x0fTelemetryProtosZ\"github.com/meshtastic/go/generated\xaa\x02\x14Meshtastic.Protobufs\xba\x02\x00\x62\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1ameshtastic/telemetry.proto\x12\nmeshtastic\"\x81\x01\n\rDeviceMetrics\x12\x15\n\rbattery_level\x18\x01 \x01(\r\x12\x0f\n\x07voltage\x18\x02 \x01(\x02\x12\x1b\n\x13\x63hannel_utilization\x18\x03 \x01(\x02\x12\x13\n\x0b\x61ir_util_tx\x18\x04 \x01(\x02\x12\x16\n\x0euptime_seconds\x18\x05 \x01(\r\"\xba\x01\n\x12\x45nvironmentMetrics\x12\x13\n\x0btemperature\x18\x01 \x01(\x02\x12\x19\n\x11relative_humidity\x18\x02 \x01(\x02\x12\x1b\n\x13\x62\x61rometric_pressure\x18\x03 \x01(\x02\x12\x16\n\x0egas_resistance\x18\x04 \x01(\x02\x12\x0f\n\x07voltage\x18\x05 \x01(\x02\x12\x0f\n\x07\x63urrent\x18\x06 \x01(\x02\x12\x0b\n\x03iaq\x18\x07 \x01(\r\x12\x10\n\x08\x64istance\x18\x08 \x01(\x02\"\x8c\x01\n\x0cPowerMetrics\x12\x13\n\x0b\x63h1_voltage\x18\x01 \x01(\x02\x12\x13\n\x0b\x63h1_current\x18\x02 \x01(\x02\x12\x13\n\x0b\x63h2_voltage\x18\x03 \x01(\x02\x12\x13\n\x0b\x63h2_current\x18\x04 \x01(\x02\x12\x13\n\x0b\x63h3_voltage\x18\x05 \x01(\x02\x12\x13\n\x0b\x63h3_current\x18\x06 \x01(\x02\"\xbf\x02\n\x11\x41irQualityMetrics\x12\x15\n\rpm10_standard\x18\x01 \x01(\r\x12\x15\n\rpm25_standard\x18\x02 \x01(\r\x12\x16\n\x0epm100_standard\x18\x03 \x01(\r\x12\x1a\n\x12pm10_environmental\x18\x04 \x01(\r\x12\x1a\n\x12pm25_environmental\x18\x05 \x01(\r\x12\x1b\n\x13pm100_environmental\x18\x06 \x01(\r\x12\x16\n\x0eparticles_03um\x18\x07 \x01(\r\x12\x16\n\x0eparticles_05um\x18\x08 \x01(\r\x12\x16\n\x0eparticles_10um\x18\t \x01(\r\x12\x16\n\x0eparticles_25um\x18\n \x01(\r\x12\x16\n\x0eparticles_50um\x18\x0b \x01(\r\x12\x17\n\x0fparticles_100um\x18\x0c \x01(\r\"\x89\x02\n\tTelemetry\x12\x0c\n\x04time\x18\x01 \x01(\x07\x12\x33\n\x0e\x64\x65vice_metrics\x18\x02 \x01(\x0b\x32\x19.meshtastic.DeviceMetricsH\x00\x12=\n\x13\x65nvironment_metrics\x18\x03 \x01(\x0b\x32\x1e.meshtastic.EnvironmentMetricsH\x00\x12<\n\x13\x61ir_quality_metrics\x18\x04 \x01(\x0b\x32\x1d.meshtastic.AirQualityMetricsH\x00\x12\x31\n\rpower_metrics\x18\x05 \x01(\x0b\x32\x18.meshtastic.PowerMetricsH\x00\x42\t\n\x07variant*\xf9\x01\n\x13TelemetrySensorType\x12\x10\n\x0cSENSOR_UNSET\x10\x00\x12\n\n\x06\x42ME280\x10\x01\x12\n\n\x06\x42ME680\x10\x02\x12\x0b\n\x07MCP9808\x10\x03\x12\n\n\x06INA260\x10\x04\x12\n\n\x06INA219\x10\x05\x12\n\n\x06\x42MP280\x10\x06\x12\t\n\x05SHTC3\x10\x07\x12\t\n\x05LPS22\x10\x08\x12\x0b\n\x07QMC6310\x10\t\x12\x0b\n\x07QMI8658\x10\n\x12\x0c\n\x08QMC5883L\x10\x0b\x12\t\n\x05SHT31\x10\x0c\x12\x0c\n\x08PMSA003I\x10\r\x12\x0b\n\x07INA3221\x10\x0e\x12\n\n\x06\x42MP085\x10\x0f\x12\x0c\n\x08RCWL9620\x10\x10\x12\t\n\x05SHT4X\x10\x11\x42\x64\n\x13\x63om.geeksville.meshB\x0fTelemetryProtosZ\"github.com/meshtastic/go/generated\xaa\x02\x14Meshtastic.Protobufs\xba\x02\x00\x62\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'meshtastic.telemetry_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'\n\023com.geeksville.meshB\017TelemetryProtosZ\"github.com/meshtastic/go/generated\252\002\024Meshtastic.Protobufs\272\002\000'
   _TELEMETRYSENSORTYPE._serialized_start=1097
-  _TELEMETRYSENSORTYPE._serialized_end=1335
+  _TELEMETRYSENSORTYPE._serialized_end=1346
   _DEVICEMETRICS._serialized_start=43
   _DEVICEMETRICS._serialized_end=172
   _ENVIRONMENTMETRICS._serialized_start=175
   _ENVIRONMENTMETRICS._serialized_end=361
   _POWERMETRICS._serialized_start=364
   _POWERMETRICS._serialized_end=504
   _AIRQUALITYMETRICS._serialized_start=507
```

### Comparing `meshtastic-2.3.8/meshtastic/telemetry_pb2.pyi` & `meshtastic-2.3.9/meshtastic/telemetry_pb2.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -86,14 +86,18 @@
     """
     BMP085/BMP180 High accuracy temperature and pressure (older Version of BMP280)
     """
     RCWL9620: _TelemetrySensorType.ValueType  # 16
     """
     RCWL-9620 Doppler Radar Distance Sensor, used for water level detection
     """
+    SHT4X: _TelemetrySensorType.ValueType  # 17
+    """
+    Sensirion High accuracy temperature and humidity
+    """
 
 class TelemetrySensorType(_TelemetrySensorType, metaclass=_TelemetrySensorTypeEnumTypeWrapper):
     """
     Supported I2C Sensors for telemetry in Meshtastic
     """
 
 SENSOR_UNSET: TelemetrySensorType.ValueType  # 0
@@ -160,14 +164,18 @@
 """
 BMP085/BMP180 High accuracy temperature and pressure (older Version of BMP280)
 """
 RCWL9620: TelemetrySensorType.ValueType  # 16
 """
 RCWL-9620 Doppler Radar Distance Sensor, used for water level detection
 """
+SHT4X: TelemetrySensorType.ValueType  # 17
+"""
+Sensirion High accuracy temperature and humidity
+"""
 global___TelemetrySensorType = TelemetrySensorType
 
 @typing_extensions.final
 class DeviceMetrics(google.protobuf.message.Message):
     """
     Key native device metrics such as battery level
     """
```

### Comparing `meshtastic-2.3.8/meshtastic/test.py` & `meshtastic-2.3.9/meshtastic/test.py`

 * *Files identical despite different names*

### Comparing `meshtastic-2.3.8/meshtastic/tunnel.py` & `meshtastic-2.3.9/meshtastic/tunnel.py`

 * *Files identical despite different names*

### Comparing `meshtastic-2.3.8/meshtastic/util.py` & `meshtastic-2.3.9/meshtastic/util.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 import re
 import subprocess
 import sys
 import threading
 import time
 import traceback
 from queue import Queue
-from typing import Union
+from typing import List, NoReturn, Union
 
 from google.protobuf.json_format import MessageToJson
 
 import packaging.version as pkg_version
 import requests
 import serial # type: ignore[import-untyped]
 import serial.tools.list_ports # type: ignore[import-untyped]
@@ -118,15 +118,15 @@
     """Call a closure but if it throws an exception print it and continue"""
     try:
         closure()
     except BaseException as ex:
         logging.error(f"Exception thrown in {reason}: {ex}")
 
 
-def findPorts(eliminate_duplicates=False):
+def findPorts(eliminate_duplicates: bool=False) -> List[str]:
     """Find all ports that might have meshtastic devices
        eliminate_duplicates will run the eliminate_duplicate_port() on the collection
 
     Returns:
         list -- a list of device paths
     """
     l = list(
@@ -259,15 +259,15 @@
             except:
                 logging.error(
                     f"Unexpected error in deferred execution {sys.exc_info()[0]}"
                 )
                 print(traceback.format_exc())
 
 
-def our_exit(message, return_value=1):
+def our_exit(message, return_value=1) -> NoReturn:
     """Print the message and return a value.
     return_value defaults to 1 (non-successful)
     """
     print(message)
     sys.exit(return_value)
```

### Comparing `meshtastic-2.3.8/meshtastic/xmodem_pb2.py` & `meshtastic-2.3.9/meshtastic/xmodem_pb2.py`

 * *Files identical despite different names*

### Comparing `meshtastic-2.3.8/meshtastic/xmodem_pb2.pyi` & `meshtastic-2.3.9/meshtastic/xmodem_pb2.pyi`

 * *Files identical despite different names*

### Comparing `meshtastic-2.3.8/meshtastic.egg-info/PKG-INFO` & `meshtastic-2.3.9/meshtastic.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: meshtastic
-Version: 2.3.8
+Version: 2.3.9
 Summary: Python API & client shell for talking to Meshtastic devices
 Home-page: https://github.com/meshtastic/python
 Author: Meshtastic Developers
 Author-email: contact@meshtastic.org
 License: GPL-3.0-only
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Development Status :: 4 - Beta
@@ -57,28 +57,27 @@
 If you're interested in contributing but don't have specific things you'd like to work on, look at the roadmap below!
 
 ## Roadmap
 
 This should always be considered a list in progress and flux -- inclusion doesn't guarantee implementation, and exclusion doesn't mean something's not wanted. GitHub issues are a great place to discuss ideas.
 
 * Types
-  * type annotations throughout the codebase
-  * mypy running in CI to type-check new code
+  * type annotations throughout the codebase, and upgrading mypy running in CI to `--strict`
 * async-friendliness
 * CLI completeness & consistency
   * the CLI should support all features of the firmware
   * there should be a consistent output format available for shell scripting
 * CLI input validation & documentation
   * what arguments and options are compatible & incompatible with one another?
   * can the options be restructured in a way that is more self-documenting?
   * pubsub events should be documented clearly
 * helpers for third-party code
   * it should be easy to write a script that supports similar options to the CLI so many tools support the same ways of connecting to nodes
-* interactive client
 * data storage & processing
   * there should be a standardized way of recording packets for later use, debugging, etc.
+  * a persistence layer could also keep track of nodes beyond nodedb, as the apps do
   * a sqlite database schema and tools for writing to it may be a good starting point
   * enable maps, charts, visualizations
 
 ## Stats
 
 ![Alt](https://repobeats.axiom.co/api/embed/c71ee8fc4a79690402e5d2807a41eec5e96d9039.svg "Repobeats analytics image")
```

### Comparing `meshtastic-2.3.8/meshtastic.egg-info/SOURCES.txt` & `meshtastic-2.3.9/meshtastic.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `meshtastic-2.3.8/setup.py` & `meshtastic-2.3.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 # This call to setup() does all the work
 setup(
     name="meshtastic",
-    version="2.3.8",
+    version="2.3.9",
     description="Python API & client shell for talking to Meshtastic devices",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/meshtastic/python",
     author="Meshtastic Developers",
     author_email="contact@meshtastic.org",
     license="GPL-3.0-only",
```

