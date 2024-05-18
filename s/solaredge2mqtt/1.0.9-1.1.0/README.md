# Comparing `tmp/solaredge2mqtt-1.0.9.tar.gz` & `tmp/solaredge2mqtt-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "solaredge2mqtt-1.0.9.tar", last modified: Sun Apr 14 13:08:57 2024, max compression
+gzip compressed data, was "solaredge2mqtt-1.1.0.tar", last modified: Sat May 18 10:31:56 2024, max compression
```

## Comparing `solaredge2mqtt-1.0.9.tar` & `solaredge2mqtt-1.1.0.tar`

### file list

```diff
@@ -1,57 +1,99 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 13:08:57.374266 solaredge2mqtt-1.0.9/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-14 13:08:52.000000 solaredge2mqtt-1.0.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      356 2024-04-14 13:08:52.000000 solaredge2mqtt-1.0.9/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    14321 2024-04-14 13:08:57.374266 solaredge2mqtt-1.0.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    13061 2024-04-14 13:08:52.000000 solaredge2mqtt-1.0.9/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      823 2024-04-14 13:08:52.000000 solaredge2mqtt-1.0.9/THIRD-PARTY-NOTICES
--rw-r--r--   0 runner    (1001) docker     (127)      254 2024-04-14 13:08:52.000000 solaredge2mqtt-1.0.9/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      243 2024-04-14 13:08:57.374266 solaredge2mqtt-1.0.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1417 2024-04-14 13:08:52.000000 solaredge2mqtt-1.0.9/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 13:08:57.370267 solaredge2mqtt-1.0.9/solaredge2mqtt/
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-14 13:08:52.000000 solaredge2mqtt-1.0.9/solaredge2mqtt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-14 13:08:52.000000 solaredge2mqtt-1.0.9/solaredge2mqtt/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)      497 2024-04-14 13:08:57.374266 solaredge2mqtt-1.0.9/solaredge2mqtt/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)      376 2024-04-14 13:08:52.000000 solaredge2mqtt-1.0.9/solaredge2mqtt/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 13:08:57.370267 solaredge2mqtt-1.0.9/solaredge2mqtt/flux/
--rw-r--r--   0 runner    (1001) docker     (127)      580 2024-04-14 13:08:52.000000 solaredge2mqtt-1.0.9/solaredge2mqtt/flux/actual_unit.flux
--rw-r--r--   0 runner    (1001) docker     (127)     3381 2024-04-14 13:08:52.000000 solaredge2mqtt-1.0.9/solaredge2mqtt/flux/aggregate.flux
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 13:08:57.370267 solaredge2mqtt-1.0.9/solaredge2mqtt/flux/fixes/
--rw-r--r--   0 runner    (1001) docker     (127)     1318 2024-04-14 13:08:52.000000 solaredge2mqtt-1.0.9/solaredge2mqtt/flux/fixes/fix_0.20.1.flux
--rw-r--r--   0 runner    (1001) docker     (127)     1634 2024-04-14 13:08:52.000000 solaredge2mqtt-1.0.9/solaredge2mqtt/flux/fixes/import-historic-monitoring_data_1.0.8.flux
--rw-r--r--   0 runner    (1001) docker     (127)     1033 2024-04-14 13:08:52.000000 solaredge2mqtt-1.0.9/solaredge2mqtt/flux/fixes/refactor_money_fields_1.0.8.flux
--rw-r--r--   0 runner    (1001) docker     (127)      621 2024-04-14 13:08:52.000000 solaredge2mqtt-1.0.9/solaredge2mqtt/flux/forecast_unit.flux
--rw-r--r--   0 runner    (1001) docker     (127)      596 2024-04-14 13:08:52.000000 solaredge2mqtt-1.0.9/solaredge2mqtt/flux/historic_unit.flux
--rw-r--r--   0 runner    (1001) docker     (127)      920 2024-04-14 13:08:52.000000 solaredge2mqtt-1.0.9/solaredge2mqtt/flux/production.flux
--rw-r--r--   0 runner    (1001) docker     (127)     4573 2024-04-14 13:08:52.000000 solaredge2mqtt-1.0.9/solaredge2mqtt/flux/reduce.flux
--rw-r--r--   0 runner    (1001) docker     (127)      218 2024-04-14 13:08:52.000000 solaredge2mqtt-1.0.9/solaredge2mqtt/flux/training_data.flux
--rw-r--r--   0 runner    (1001) docker     (127)      895 2024-04-14 13:08:52.000000 solaredge2mqtt-1.0.9/solaredge2mqtt/logging.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 13:08:57.374266 solaredge2mqtt-1.0.9/solaredge2mqtt/models/
--rw-r--r--   0 runner    (1001) docker     (127)      837 2024-04-14 13:08:52.000000 solaredge2mqtt-1.0.9/solaredge2mqtt/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2409 2024-04-14 13:08:52.000000 solaredge2mqtt-1.0.9/solaredge2mqtt/models/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      939 2024-04-14 13:08:52.000000 solaredge2mqtt-1.0.9/solaredge2mqtt/models/forecast.py
--rw-r--r--   0 runner    (1001) docker     (127)     6421 2024-04-14 13:08:52.000000 solaredge2mqtt-1.0.9/solaredge2mqtt/models/historic.py
--rw-r--r--   0 runner    (1001) docker     (127)     7601 2024-04-14 13:08:52.000000 solaredge2mqtt-1.0.9/solaredge2mqtt/models/modbus.py
--rw-r--r--   0 runner    (1001) docker     (127)      747 2024-04-14 13:08:52.000000 solaredge2mqtt-1.0.9/solaredge2mqtt/models/monitoring.py
--rw-r--r--   0 runner    (1001) docker     (127)     9998 2024-04-14 13:08:52.000000 solaredge2mqtt-1.0.9/solaredge2mqtt/models/powerflow.py
--rw-r--r--   0 runner    (1001) docker     (127)      630 2024-04-14 13:08:52.000000 solaredge2mqtt-1.0.9/solaredge2mqtt/models/wallbox.py
--rw-r--r--   0 runner    (1001) docker     (127)     2753 2024-04-14 13:08:52.000000 solaredge2mqtt-1.0.9/solaredge2mqtt/models/weather.py
--rw-r--r--   0 runner    (1001) docker     (127)     1521 2024-04-14 13:08:52.000000 solaredge2mqtt-1.0.9/solaredge2mqtt/mqtt.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 13:08:57.374266 solaredge2mqtt-1.0.9/solaredge2mqtt/service/
--rw-r--r--   0 runner    (1001) docker     (127)     6414 2024-04-14 13:08:52.000000 solaredge2mqtt-1.0.9/solaredge2mqtt/service/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4297 2024-04-14 13:08:52.000000 solaredge2mqtt-1.0.9/solaredge2mqtt/service/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    23676 2024-04-14 13:08:52.000000 solaredge2mqtt-1.0.9/solaredge2mqtt/service/forecast.py
--rw-r--r--   0 runner    (1001) docker     (127)     2912 2024-04-14 13:08:52.000000 solaredge2mqtt-1.0.9/solaredge2mqtt/service/http.py
--rw-r--r--   0 runner    (1001) docker     (127)     6881 2024-04-14 13:08:52.000000 solaredge2mqtt-1.0.9/solaredge2mqtt/service/influxdb.py
--rw-r--r--   0 runner    (1001) docker     (127)     4658 2024-04-14 13:08:52.000000 solaredge2mqtt-1.0.9/solaredge2mqtt/service/modbus.py
--rw-r--r--   0 runner    (1001) docker     (127)     5496 2024-04-14 13:08:52.000000 solaredge2mqtt-1.0.9/solaredge2mqtt/service/monitoring.py
--rw-r--r--   0 runner    (1001) docker     (127)     4386 2024-04-14 13:08:52.000000 solaredge2mqtt-1.0.9/solaredge2mqtt/service/wallbox.py
--rw-r--r--   0 runner    (1001) docker     (127)     2139 2024-04-14 13:08:52.000000 solaredge2mqtt-1.0.9/solaredge2mqtt/service/weather.py
--rw-r--r--   0 runner    (1001) docker     (127)     7467 2024-04-14 13:08:52.000000 solaredge2mqtt-1.0.9/solaredge2mqtt/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 13:08:57.374266 solaredge2mqtt-1.0.9/solaredge2mqtt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    14321 2024-04-14 13:08:57.000000 solaredge2mqtt-1.0.9/solaredge2mqtt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1548 2024-04-14 13:08:57.000000 solaredge2mqtt-1.0.9/solaredge2mqtt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-14 13:08:57.000000 solaredge2mqtt-1.0.9/solaredge2mqtt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-14 13:08:57.000000 solaredge2mqtt-1.0.9/solaredge2mqtt.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      255 2024-04-14 13:08:57.000000 solaredge2mqtt-1.0.9/solaredge2mqtt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-14 13:08:57.000000 solaredge2mqtt-1.0.9/solaredge2mqtt.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)    86677 2024-04-14 13:08:52.000000 solaredge2mqtt-1.0.9/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 10:31:56.135205 solaredge2mqtt-1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-05-18 10:31:50.000000 solaredge2mqtt-1.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      356 2024-05-18 10:31:50.000000 solaredge2mqtt-1.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    14825 2024-05-18 10:31:56.135205 solaredge2mqtt-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    13538 2024-05-18 10:31:50.000000 solaredge2mqtt-1.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      823 2024-05-18 10:31:50.000000 solaredge2mqtt-1.1.0/THIRD-PARTY-NOTICES
+-rw-r--r--   0 runner    (1001) docker     (127)      267 2024-05-18 10:31:50.000000 solaredge2mqtt-1.1.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      243 2024-05-18 10:31:56.135205 solaredge2mqtt-1.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1417 2024-05-18 10:31:50.000000 solaredge2mqtt-1.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 10:31:56.123205 solaredge2mqtt-1.1.0/solaredge2mqtt/
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-05-18 10:31:50.000000 solaredge2mqtt-1.1.0/solaredge2mqtt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-05-18 10:31:50.000000 solaredge2mqtt-1.1.0/solaredge2mqtt/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      497 2024-05-18 10:31:56.135205 solaredge2mqtt-1.1.0/solaredge2mqtt/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 10:31:56.123205 solaredge2mqtt-1.1.0/solaredge2mqtt/core/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 10:31:56.123205 solaredge2mqtt-1.1.0/solaredge2mqtt/core/events/
+-rw-r--r--   0 runner    (1001) docker     (127)     2995 2024-05-18 10:31:50.000000 solaredge2mqtt-1.1.0/solaredge2mqtt/core/events/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-05-18 10:31:50.000000 solaredge2mqtt-1.1.0/solaredge2mqtt/core/events/events.py
+-rw-r--r--   0 runner    (1001) docker     (127)      376 2024-05-18 10:31:50.000000 solaredge2mqtt-1.1.0/solaredge2mqtt/core/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 10:31:56.123205 solaredge2mqtt-1.1.0/solaredge2mqtt/core/influxdb/
+-rw-r--r--   0 runner    (1001) docker     (127)     7617 2024-05-18 10:31:50.000000 solaredge2mqtt-1.1.0/solaredge2mqtt/core/influxdb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      109 2024-05-18 10:31:50.000000 solaredge2mqtt-1.1.0/solaredge2mqtt/core/influxdb/events.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 10:31:56.123205 solaredge2mqtt-1.1.0/solaredge2mqtt/core/influxdb/flux/
+-rw-r--r--   0 runner    (1001) docker     (127)      580 2024-05-18 10:31:50.000000 solaredge2mqtt-1.1.0/solaredge2mqtt/core/influxdb/flux/actual_unit.flux
+-rw-r--r--   0 runner    (1001) docker     (127)     3381 2024-05-18 10:31:50.000000 solaredge2mqtt-1.1.0/solaredge2mqtt/core/influxdb/flux/aggregate.flux
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 10:31:56.127205 solaredge2mqtt-1.1.0/solaredge2mqtt/core/influxdb/flux/fixes/
+-rw-r--r--   0 runner    (1001) docker     (127)     1318 2024-05-18 10:31:50.000000 solaredge2mqtt-1.1.0/solaredge2mqtt/core/influxdb/flux/fixes/fix_0.20.1.flux
+-rw-r--r--   0 runner    (1001) docker     (127)     1634 2024-05-18 10:31:50.000000 solaredge2mqtt-1.1.0/solaredge2mqtt/core/influxdb/flux/fixes/import-historic-monitoring_data_1.0.8.flux
+-rw-r--r--   0 runner    (1001) docker     (127)     1033 2024-05-18 10:31:50.000000 solaredge2mqtt-1.1.0/solaredge2mqtt/core/influxdb/flux/fixes/refactor_money_fields_1.0.8.flux
+-rw-r--r--   0 runner    (1001) docker     (127)      393 2024-05-18 10:31:50.000000 solaredge2mqtt-1.1.0/solaredge2mqtt/core/influxdb/flux/forecast.flux
+-rw-r--r--   0 runner    (1001) docker     (127)      596 2024-05-18 10:31:50.000000 solaredge2mqtt-1.1.0/solaredge2mqtt/core/influxdb/flux/historic_unit.flux
+-rw-r--r--   0 runner    (1001) docker     (127)      920 2024-05-18 10:31:50.000000 solaredge2mqtt-1.1.0/solaredge2mqtt/core/influxdb/flux/production.flux
+-rw-r--r--   0 runner    (1001) docker     (127)     4573 2024-05-18 10:31:50.000000 solaredge2mqtt-1.1.0/solaredge2mqtt/core/influxdb/flux/reduce.flux
+-rw-r--r--   0 runner    (1001) docker     (127)      218 2024-05-18 10:31:50.000000 solaredge2mqtt-1.1.0/solaredge2mqtt/core/influxdb/flux/training_data.flux
+-rw-r--r--   0 runner    (1001) docker     (127)      926 2024-05-18 10:31:50.000000 solaredge2mqtt-1.1.0/solaredge2mqtt/core/influxdb/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 10:31:56.127205 solaredge2mqtt-1.1.0/solaredge2mqtt/core/logging/
+-rw-r--r--   0 runner    (1001) docker     (127)      254 2024-05-18 10:31:50.000000 solaredge2mqtt-1.1.0/solaredge2mqtt/core/logging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      622 2024-05-18 10:31:50.000000 solaredge2mqtt-1.1.0/solaredge2mqtt/core/logging/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3943 2024-05-18 10:31:50.000000 solaredge2mqtt-1.1.0/solaredge2mqtt/core/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 10:31:56.127205 solaredge2mqtt-1.1.0/solaredge2mqtt/core/mqtt/
+-rw-r--r--   0 runner    (1001) docker     (127)     3228 2024-05-18 10:31:50.000000 solaredge2mqtt-1.1.0/solaredge2mqtt/core/mqtt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1741 2024-05-18 10:31:50.000000 solaredge2mqtt-1.1.0/solaredge2mqtt/core/mqtt/events.py
+-rw-r--r--   0 runner    (1001) docker     (127)      256 2024-05-18 10:31:50.000000 solaredge2mqtt-1.1.0/solaredge2mqtt/core/mqtt/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 10:31:56.127205 solaredge2mqtt-1.1.0/solaredge2mqtt/core/settings/
+-rw-r--r--   0 runner    (1001) docker     (127)      220 2024-05-18 10:31:50.000000 solaredge2mqtt-1.1.0/solaredge2mqtt/core/settings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5404 2024-05-18 10:31:50.000000 solaredge2mqtt-1.1.0/solaredge2mqtt/core/settings/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 10:31:56.127205 solaredge2mqtt-1.1.0/solaredge2mqtt/core/timer/
+-rw-r--r--   0 runner    (1001) docker     (127)      658 2024-05-18 10:31:50.000000 solaredge2mqtt-1.1.0/solaredge2mqtt/core/timer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      180 2024-05-18 10:31:50.000000 solaredge2mqtt-1.1.0/solaredge2mqtt/core/timer/events.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6723 2024-05-18 10:31:50.000000 solaredge2mqtt-1.1.0/solaredge2mqtt/service.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 10:31:56.127205 solaredge2mqtt-1.1.0/solaredge2mqtt/services/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 10:31:56.127205 solaredge2mqtt-1.1.0/solaredge2mqtt/services/energy/
+-rw-r--r--   0 runner    (1001) docker     (127)     1841 2024-05-18 10:31:50.000000 solaredge2mqtt-1.1.0/solaredge2mqtt/services/energy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      196 2024-05-18 10:31:50.000000 solaredge2mqtt-1.1.0/solaredge2mqtt/services/energy/events.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9468 2024-05-18 10:31:50.000000 solaredge2mqtt-1.1.0/solaredge2mqtt/services/energy/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)      746 2024-05-18 10:31:50.000000 solaredge2mqtt-1.1.0/solaredge2mqtt/services/energy/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)      674 2024-05-18 10:31:50.000000 solaredge2mqtt-1.1.0/solaredge2mqtt/services/events.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 10:31:56.131205 solaredge2mqtt-1.1.0/solaredge2mqtt/services/forecast/
+-rw-r--r--   0 runner    (1001) docker     (127)    15500 2024-05-18 10:31:50.000000 solaredge2mqtt-1.1.0/solaredge2mqtt/services/forecast/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7423 2024-05-18 10:31:50.000000 solaredge2mqtt-1.1.0/solaredge2mqtt/services/forecast/encoders.py
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-05-18 10:31:50.000000 solaredge2mqtt-1.1.0/solaredge2mqtt/services/forecast/events.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2785 2024-05-18 10:31:50.000000 solaredge2mqtt-1.1.0/solaredge2mqtt/services/forecast/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)      232 2024-05-18 10:31:50.000000 solaredge2mqtt-1.1.0/solaredge2mqtt/services/forecast/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 10:31:56.131205 solaredge2mqtt-1.1.0/solaredge2mqtt/services/homeassistant/
+-rw-r--r--   0 runner    (1001) docker     (127)     5457 2024-05-18 10:31:50.000000 solaredge2mqtt-1.1.0/solaredge2mqtt/services/homeassistant/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5006 2024-05-18 10:31:50.000000 solaredge2mqtt-1.1.0/solaredge2mqtt/services/homeassistant/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)      238 2024-05-18 10:31:50.000000 solaredge2mqtt-1.1.0/solaredge2mqtt/services/homeassistant/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2917 2024-05-18 10:31:50.000000 solaredge2mqtt-1.1.0/solaredge2mqtt/services/http.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 10:31:56.131205 solaredge2mqtt-1.1.0/solaredge2mqtt/services/modbus/
+-rw-r--r--   0 runner    (1001) docker     (127)     5314 2024-05-18 10:31:50.000000 solaredge2mqtt-1.1.0/solaredge2mqtt/services/modbus/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      250 2024-05-18 10:31:50.000000 solaredge2mqtt-1.1.0/solaredge2mqtt/services/modbus/events.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10456 2024-05-18 10:31:50.000000 solaredge2mqtt-1.1.0/solaredge2mqtt/services/modbus/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)      168 2024-05-18 10:31:50.000000 solaredge2mqtt-1.1.0/solaredge2mqtt/services/modbus/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1170 2024-05-18 10:31:50.000000 solaredge2mqtt-1.1.0/solaredge2mqtt/services/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 10:31:56.131205 solaredge2mqtt-1.1.0/solaredge2mqtt/services/monitoring/
+-rw-r--r--   0 runner    (1001) docker     (127)     6041 2024-05-18 10:31:50.000000 solaredge2mqtt-1.1.0/solaredge2mqtt/services/monitoring/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      747 2024-05-18 10:31:50.000000 solaredge2mqtt-1.1.0/solaredge2mqtt/services/monitoring/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)      427 2024-05-18 10:31:50.000000 solaredge2mqtt-1.1.0/solaredge2mqtt/services/monitoring/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 10:31:56.131205 solaredge2mqtt-1.1.0/solaredge2mqtt/services/powerflow/
+-rw-r--r--   0 runner    (1001) docker     (127)     4490 2024-05-18 10:31:50.000000 solaredge2mqtt-1.1.0/solaredge2mqtt/services/powerflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-05-18 10:31:50.000000 solaredge2mqtt-1.1.0/solaredge2mqtt/services/powerflow/events.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11657 2024-05-18 10:31:50.000000 solaredge2mqtt-1.1.0/solaredge2mqtt/services/powerflow/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 10:31:56.131205 solaredge2mqtt-1.1.0/solaredge2mqtt/services/wallbox/
+-rw-r--r--   0 runner    (1001) docker     (127)     4673 2024-05-18 10:31:50.000000 solaredge2mqtt-1.1.0/solaredge2mqtt/services/wallbox/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      109 2024-05-18 10:31:50.000000 solaredge2mqtt-1.1.0/solaredge2mqtt/services/wallbox/events.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2357 2024-05-18 10:31:50.000000 solaredge2mqtt-1.1.0/solaredge2mqtt/services/wallbox/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)      351 2024-05-18 10:31:50.000000 solaredge2mqtt-1.1.0/solaredge2mqtt/services/wallbox/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 10:31:56.131205 solaredge2mqtt-1.1.0/solaredge2mqtt/services/weather/
+-rw-r--r--   0 runner    (1001) docker     (127)     2774 2024-05-18 10:31:50.000000 solaredge2mqtt-1.1.0/solaredge2mqtt/services/weather/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      356 2024-05-18 10:31:50.000000 solaredge2mqtt-1.1.0/solaredge2mqtt/services/weather/events.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2753 2024-05-18 10:31:50.000000 solaredge2mqtt-1.1.0/solaredge2mqtt/services/weather/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)      253 2024-05-18 10:31:50.000000 solaredge2mqtt-1.1.0/solaredge2mqtt/services/weather/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 10:31:56.131205 solaredge2mqtt-1.1.0/solaredge2mqtt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    14825 2024-05-18 10:31:56.000000 solaredge2mqtt-1.1.0/solaredge2mqtt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3022 2024-05-18 10:31:56.000000 solaredge2mqtt-1.1.0/solaredge2mqtt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-18 10:31:56.000000 solaredge2mqtt-1.1.0/solaredge2mqtt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-18 10:31:56.000000 solaredge2mqtt-1.1.0/solaredge2mqtt.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      267 2024-05-18 10:31:56.000000 solaredge2mqtt-1.1.0/solaredge2mqtt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-18 10:31:56.000000 solaredge2mqtt-1.1.0/solaredge2mqtt.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    86677 2024-05-18 10:31:50.000000 solaredge2mqtt-1.1.0/versioneer.py
```

### Comparing `solaredge2mqtt-1.0.9/LICENSE` & `solaredge2mqtt-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `solaredge2mqtt-1.0.9/PKG-INFO` & `solaredge2mqtt-1.1.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: solaredge2mqtt
-Version: 1.0.9
+Version: 1.1.0
 Summary: Read data from SolarEdge Inverter and publish it to MQTT
 Home-page: https://github.com/deroetzi/solaredge2mqtt
 Author: Johannes Ott
 Author-email: info@johannes-ott.net
 Project-URL: Bug Reports, https://github.com/deroetzi/solaredge2mqtt/issues
 Keywords: smart home
 Classifier: Development Status :: 5 - Production/Stable
@@ -13,29 +13,30 @@
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.10, <4
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: solaredge_modbus==0.8.0
-Requires-Dist: pydantic==2.7.0
+Requires-Dist: aiocsv==1.3.2
+Requires-Dist: aiohttp==3.9.5
+Requires-Dist: aiomqtt==2.1.0
+Requires-Dist: astral==3.2
+Requires-Dist: ephem==4.1.5
+Requires-Dist: influxdb-client==1.43.0
+Requires-Dist: jsonref==1.1.0
 Requires-Dist: loguru==0.7.2
-Requires-Dist: requests==2.31.0
-Requires-Dist: influxdb-client==1.41.0
-Requires-Dist: pyjwt==2.8.0
-Requires-Dist: aiomqtt==2.0.1
 Requires-Dist: numpy==1.26.4
 Requires-Dist: pandas==2.2.2
+Requires-Dist: pydantic==2.7.1
+Requires-Dist: pyjwt==2.8.0
+Requires-Dist: requests==2.31.0
 Requires-Dist: scikit-learn==1.4.2
-Requires-Dist: scipy==1.13.0rc1
-Requires-Dist: aiohttp==3.9.4
-Requires-Dist: aiocsv==1.3.1
-Requires-Dist: astral==3.2
-Requires-Dist: ephem==4.1.5
+Requires-Dist: scipy==1.13.0
+Requires-Dist: solaredge_modbus==0.8.0
 Requires-Dist: tzlocal==5.2
 
 # SolarEdge 2 MQTT Service
 
 [![License](https://img.shields.io/github/license/DerOetzi/solaredge2mqtt)](https://github.com/DerOetzi/solaredge2mqtt/blob/main/LICENSE) [![Release](https://img.shields.io/github/v/release/DerOetzi/solaredge2mqtt)](https://github.com/DerOetzi/solaredge2mqtt/releases/latest) [![Build Status](https://img.shields.io/github/actions/workflow/status/DerOetzi/solaredge2mqtt/build_project.yml?branch=main)](https://github.com/DerOetzi/solaredge2mqtt/actions/workflows/build_project.yml) [![PyPI version](https://img.shields.io/pypi/v/solaredge2mqtt.svg)](https://pypi.org/project/solaredge2mqtt/) [![Discord Chat](https://img.shields.io/discord/1196540254686032014)](https://discord.gg/QXfghc93pY)
 
 The SolarEdge2MQTT service facilitates the retrieval of power data from SolarEdge inverters and its publication to an MQTT broker. Ideal for integrating SolarEdge inverters into home automation systems, this service supports real-time monitoring of power flow and additional parameters via Modbus.
@@ -93,14 +94,23 @@
 
 For monitoring SolarEdge Wallbox, provide:
 
 - **SE2MQTT_WALLBOX\_\_HOST**: The IP address of your Wallbox.
 - **SE2MQTT_WALLBOX\_\_PASSWORD**: The admin password for Wallbox web UI access.
 - **SE2MQTT_WALLBOX\_\_SERIAL**: The serial number of your Wallbox.
 
+### Home Assistant Auto Discovery
+
+If you want Home Assistant to auto discover the data SolarEdge2MQTT provides, you can enable this here.
+
+- **SE2MQTT_HOMEASSISTANT\_\_ENABLE**: Set to true to enable the auto discovery
+- **SE2MQTT_HOMEASSISTANT\_\_TOPIC_PREFIX**: By default Home Assistant MQTT integration listens to subtopics of homeassistant
+
+_If you want to remove things, just disable the feature, then restart SolarEdge2MQTT first and after it restart Home Assistant,_
+
 ### InfluxDB
 
 Configure your InfluxDB settings with these environment variables to store monitoring data effectively:
 
 - **SE2MQTT_INFLUXDB\_\_HOST**: Specify the host of your InfluxDB instance (e.g., http://localhost). Default is None.
 - **SE2MQTT_INFLUXDB\_\_PORT**: The port number on which your InfluxDB instance is running. The default value is 8086.
 - **SE2MQTT_INFLUXDB\_\_TOKEN**: Your access token for InfluxDB. It is imperative to use this token securely, especially when deploying with Docker. The token requires full access since the service will be managing necessary buckets and tasks. Default is None.
```

### Comparing `solaredge2mqtt-1.0.9/README.md` & `solaredge2mqtt-1.1.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -57,14 +57,23 @@
 
 For monitoring SolarEdge Wallbox, provide:
 
 - **SE2MQTT_WALLBOX\_\_HOST**: The IP address of your Wallbox.
 - **SE2MQTT_WALLBOX\_\_PASSWORD**: The admin password for Wallbox web UI access.
 - **SE2MQTT_WALLBOX\_\_SERIAL**: The serial number of your Wallbox.
 
+### Home Assistant Auto Discovery
+
+If you want Home Assistant to auto discover the data SolarEdge2MQTT provides, you can enable this here.
+
+- **SE2MQTT_HOMEASSISTANT\_\_ENABLE**: Set to true to enable the auto discovery
+- **SE2MQTT_HOMEASSISTANT\_\_TOPIC_PREFIX**: By default Home Assistant MQTT integration listens to subtopics of homeassistant
+
+_If you want to remove things, just disable the feature, then restart SolarEdge2MQTT first and after it restart Home Assistant,_
+
 ### InfluxDB
 
 Configure your InfluxDB settings with these environment variables to store monitoring data effectively:
 
 - **SE2MQTT_INFLUXDB\_\_HOST**: Specify the host of your InfluxDB instance (e.g., http://localhost). Default is None.
 - **SE2MQTT_INFLUXDB\_\_PORT**: The port number on which your InfluxDB instance is running. The default value is 8086.
 - **SE2MQTT_INFLUXDB\_\_TOKEN**: Your access token for InfluxDB. It is imperative to use this token securely, especially when deploying with Docker. The token requires full access since the service will be managing necessary buckets and tasks. Default is None.
```

### Comparing `solaredge2mqtt-1.0.9/THIRD-PARTY-NOTICES` & `solaredge2mqtt-1.1.0/THIRD-PARTY-NOTICES`

 * *Files identical despite different names*

### Comparing `solaredge2mqtt-1.0.9/setup.py` & `solaredge2mqtt-1.1.0/setup.py`

 * *Files identical despite different names*

### Comparing `solaredge2mqtt-1.0.9/solaredge2mqtt/flux/actual_unit.flux` & `solaredge2mqtt-1.1.0/solaredge2mqtt/core/influxdb/flux/actual_unit.flux`

 * *Files identical despite different names*

### Comparing `solaredge2mqtt-1.0.9/solaredge2mqtt/flux/aggregate.flux` & `solaredge2mqtt-1.1.0/solaredge2mqtt/core/influxdb/flux/aggregate.flux`

 * *Files identical despite different names*

### Comparing `solaredge2mqtt-1.0.9/solaredge2mqtt/flux/fixes/fix_0.20.1.flux` & `solaredge2mqtt-1.1.0/solaredge2mqtt/core/influxdb/flux/fixes/fix_0.20.1.flux`

 * *Files identical despite different names*

### Comparing `solaredge2mqtt-1.0.9/solaredge2mqtt/flux/fixes/import-historic-monitoring_data_1.0.8.flux` & `solaredge2mqtt-1.1.0/solaredge2mqtt/core/influxdb/flux/fixes/import-historic-monitoring_data_1.0.8.flux`

 * *Files identical despite different names*

### Comparing `solaredge2mqtt-1.0.9/solaredge2mqtt/flux/fixes/refactor_money_fields_1.0.8.flux` & `solaredge2mqtt-1.1.0/solaredge2mqtt/core/influxdb/flux/fixes/refactor_money_fields_1.0.8.flux`

 * *Files identical despite different names*

### Comparing `solaredge2mqtt-1.0.9/solaredge2mqtt/flux/forecast_unit.flux` & `solaredge2mqtt-1.1.0/solaredge2mqtt/core/influxdb/flux/historic_unit.flux`

 * *Files 18% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import "date"
 import "timezone"
 import "experimental/date/boundaries"
 
 option location = timezone.location(name: "{{TIMEZONE}}")
 
-week = boundaries.week(week_offset: 1)
+week = boundaries.week(week_offset: -1)
 
-startTime = if "{{UNIT}}" == "1w" then week.start else date.add(to: date.truncate(t: now(), unit: {{UNIT}}), d: {{UNIT}})
-stopTime = if "{{UNIT}}" == "1w" then week.stop else date.add(to: startTime, d: {{UNIT}})
+stopTime = if "{{UNIT}}" == "1w" then week.stop else date.truncate(t: now(), unit: {{UNIT}})
+startTime = if "{{UNIT}}" == "1w" then week.start else date.sub(from: stopTime, d: {{UNIT}})
 
 from(bucket: "{{BUCKET_NAME}}")
     |> range(start: startTime, stop: stopTime)
     |> filter(fn: (r) => r._measurement == "{{MEASUREMENT}}")
     |> sum()
     |> pivot(rowKey: ["_measurement"], columnKey: ["_field"], valueColumn: "_value")
```

### Comparing `solaredge2mqtt-1.0.9/solaredge2mqtt/flux/production.flux` & `solaredge2mqtt-1.1.0/solaredge2mqtt/core/influxdb/flux/production.flux`

 * *Files identical despite different names*

### Comparing `solaredge2mqtt-1.0.9/solaredge2mqtt/flux/reduce.flux` & `solaredge2mqtt-1.1.0/solaredge2mqtt/core/influxdb/flux/reduce.flux`

 * *Files identical despite different names*

### Comparing `solaredge2mqtt-1.0.9/solaredge2mqtt/logging.py` & `solaredge2mqtt-1.1.0/solaredge2mqtt/core/logging/models.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,15 +1,10 @@
 import logging
-import sys
 
-from loguru import logger
-
-from solaredge2mqtt.models import EnumModel
-
-LOGGING_DEVICE_INFO = "{device} ({info.manufacturer} {info.model} {info.serialnumber})"
+from solaredge2mqtt.core.models import EnumModel
 
 
 class LoggingLevelEnum(EnumModel):
     DEBUG = "DEBUG", logging.DEBUG
     INFO = "INFO", logging.INFO
     WARNING = "WARNING", logging.WARNING
     ERROR = "ERROR", logging.ERROR
@@ -23,11 +18,7 @@
     @property
     def description(self) -> str:
         return self._description
 
     @property
     def level(self) -> int:
         return self._level
-
-
-def initialize_logging(logging_level: LoggingLevelEnum) -> None:
-    logger.configure(handlers=[{"sink": sys.stdout, "level": logging_level.level}])
```

### Comparing `solaredge2mqtt-1.0.9/solaredge2mqtt/models/monitoring.py` & `solaredge2mqtt-1.1.0/solaredge2mqtt/services/monitoring/models.py`

 * *Files identical despite different names*

### Comparing `solaredge2mqtt-1.0.9/solaredge2mqtt/models/powerflow.py` & `solaredge2mqtt-1.1.0/solaredge2mqtt/services/powerflow/models.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,26 +1,147 @@
 from __future__ import annotations
 
-from typing import ClassVar, TYPE_CHECKING
+from typing import TYPE_CHECKING, ClassVar
 
 from influxdb_client import Point
 from pydantic import Field, computed_field
+from pydantic.json_schema import SkipJsonSchema
 
-from solaredge2mqtt.logging import logger
-from solaredge2mqtt.models.base import Solaredge2MQTTBaseModel
-from solaredge2mqtt.models.modbus import SunSpecBattery, SunSpecInverter, SunSpecMeter
+from solaredge2mqtt.core.logging import logger
+from solaredge2mqtt.core.models import Solaredge2MQTTBaseModel
+from solaredge2mqtt.services.homeassistant.models import (
+    HomeAssistantEntityType as EntityType,
+)
+from solaredge2mqtt.services.modbus.models import (
+    SunSpecBattery,
+    SunSpecInverter,
+    SunSpecMeter,
+)
+from solaredge2mqtt.services.models import Component
 
 if TYPE_CHECKING:
-    from solaredge2mqtt.settings import PriceSettings
+    from solaredge2mqtt.services.energy.settings import PriceSettings
+
+
+class Powerflow(Component):
+    COMPONENT = "powerflow"
+    SOURCE = None
+
+    pv_production: int = Field(0, **EntityType.POWER_W.field("PV production"))
+    inverter: InverterPowerflow = Field(title="Inverter")
+    grid: GridPowerflow = Field(title="Grid")
+    battery: BatteryPowerflow = Field(title="Battery")
+    consumer: ConsumerPowerflow = Field(title="Consumer")
+
+    last_powerflow: ClassVar[Powerflow] = None
+
+    @staticmethod
+    def from_modbus(
+        inverter_data: SunSpecInverter,
+        meters_data: dict[str, SunSpecMeter],
+        batteries_data: dict[str, SunSpecBattery],
+        evcharger: int = 0,
+    ) -> Powerflow:
+        grid = GridPowerflow.from_modbus(meters_data)
+        battery = BatteryPowerflow.from_modbus(batteries_data)
+
+        if inverter_data.ac.power.actual > 0:
+            pv_production = int(inverter_data.dc.power + battery.power)
+            if pv_production < 0:
+                pv_production = 0
+        else:
+            pv_production = 0
+
+        inverter = InverterPowerflow.from_modbus(inverter_data, battery)
+
+        consumer = ConsumerPowerflow(inverter, grid, evcharger)
+
+        return Powerflow(
+            pv_production=pv_production,
+            inverter=inverter,
+            grid=grid,
+            battery=battery,
+            consumer=consumer,
+        )
+
+    @property
+    def is_valid(self) -> bool:
+        valid = False
+
+        if self.pv_production < 0:
+            logger.warning("PV production is negative")
+        elif (
+            self.consumer.used_production + self.grid.delivery
+            != self.inverter.production
+        ):
+            logger.warning(
+                "Consumer used production + grid delivery is not equal to inverter production"
+            )
+        else:
+            valid = all(
+                [
+                    self.inverter.is_valid,
+                    self.grid.is_valid,
+                    self.battery.is_valid,
+                    self.consumer.is_valid,
+                ]
+            )
+
+        return valid
+
+    @classmethod
+    def is_not_valid_with_last(cls, powerflow: Powerflow) -> bool:
+        check = False
+
+        if cls.last_powerflow is not None:
+            check = all(
+                [
+                    cls.last_powerflow.pv_production == 0
+                    and powerflow.pv_production > 100,
+                ]
+            )
+
+        cls.last_powerflow = powerflow
+
+        return check
+
+    def prepare_point(self, measurement: str = "powerflow_raw") -> Point:
+        point = Point(measurement)
+        for key, value in self.model_dump_influxdb().items():
+            point.field(key, value)
+
+        return point
+
+    def prepare_point_energy(
+        self, measurement: str = "energy", prices: PriceSettings = None
+    ) -> Point:
+        point = Point(measurement)
+        for key, value in self.model_dump_influxdb().items():
+            energy = value / 1000
+            point.field(key, energy)
+            if prices is not None:
+                if key == "consumer_used_production":
+                    point.field("money_saved", energy * prices.price_in)
+                    point.field("money_price_in", prices.price_in)
+                elif key == "grid_delivery":
+                    point.field("money_delivered", energy * prices.price_out)
+                    point.field("money_price_out", prices.price_out)
+                elif key == "grid_consumption":
+                    point.field("money_consumed", energy * prices.price_in)
+
+        return point
+
+    def homeassistant_device_info(self) -> dict[str, any]:
+        return self._default_homeassistant_device_info("Powerflow")
 
 
 class InverterPowerflow(Solaredge2MQTTBaseModel):
-    power: int
-    dc_power: int
-    battery_discharge: int = Field(exclude=True)
+    power: SkipJsonSchema[int]
+    dc_power: int = Field(**EntityType.POWER_W.field("Power DC", "solar-power"))
+    battery_discharge: SkipJsonSchema[int] = Field(exclude=True)
 
     @staticmethod
     def from_modbus(
         inverter_data: SunSpecInverter,
         battery: BatteryPowerflow,
     ) -> InverterPowerflow:
         power = int(inverter_data.ac.power.actual)
@@ -36,34 +157,36 @@
     def battery_factor(self) -> float:
         factor = 0.0
         if self.power > 0 and self.battery_discharge > 0:
             factor = self.battery_discharge / self.dc_power
 
         return factor
 
-    @computed_field
+    @computed_field(**EntityType.POWER_W.field("Consumption"))
     @property
     def consumption(self) -> int:
         return abs(self.power) if self.power < 0 else 0
 
-    @computed_field
+    @computed_field(**EntityType.POWER_W.field("Production"))
     @property
     def production(self) -> int:
         return self.power if self.power > 0 else 0
 
-    @computed_field
+    @computed_field(
+        **EntityType.POWER_W.field("Battery production", "home-battery-outline")
+    )
     @property
     def battery_production(self) -> int:
         battery_production = 0
         if self.production > 0 and self.battery_factor > 0:
             battery_production = int(round(self.production * self.battery_factor))
             battery_production = min(battery_production, self.production)
         return battery_production
 
-    @computed_field
+    @computed_field(**EntityType.POWER_W.field("PV production", "sun-angle-outline"))
     @property
     def pv_production(self) -> int:
         return self.production - self.battery_production
 
     @property
     def is_valid(self) -> bool:
         valid = False
@@ -78,31 +201,33 @@
         else:
             valid = True
 
         return valid
 
 
 class GridPowerflow(Solaredge2MQTTBaseModel):
-    power: int
+    power: SkipJsonSchema[int]
 
     @staticmethod
     def from_modbus(meters_data: dict[str, SunSpecMeter]) -> GridPowerflow:
         grid = 0
         for meter in meters_data.values():
             if "Import" in meter.info.option and "Export" in meter.info.option:
                 grid += meter.power.actual
 
         return GridPowerflow(power=grid)
 
-    @computed_field
+    @computed_field(
+        **EntityType.POWER_W.field("Consumption", "transmission-tower-import")
+    )
     @property
     def consumption(self) -> int:
         return abs(self.power) if self.power < 0 else 0
 
-    @computed_field
+    @computed_field(**EntityType.POWER_W.field("Delivery", "transmission-tower-export"))
     @property
     def delivery(self) -> int:
         return self.power if self.power > 0 else 0
 
     @property
     def is_valid(self) -> bool:
         valid = False
@@ -113,30 +238,30 @@
         else:
             valid = True
 
         return valid
 
 
 class BatteryPowerflow(Solaredge2MQTTBaseModel):
-    power: int
+    power: SkipJsonSchema[int]
 
     @staticmethod
     def from_modbus(batteries_data: dict[str, SunSpecBattery]) -> BatteryPowerflow:
         batteries_power = 0
         for battery in batteries_data.values():
             batteries_power += battery.power
 
         return BatteryPowerflow(power=batteries_power)
 
-    @computed_field
+    @computed_field(**EntityType.POWER_W.field("Charge", "battery-plus-outline"))
     @property
     def charge(self) -> int:
         return self.power if self.power > 0 else 0
 
-    @computed_field
+    @computed_field(**EntityType.POWER_W.field("Discharge", "battery-minus-outline"))
     @property
     def discharge(self) -> int:
         return abs(self.power) if self.power < 0 else 0
 
     @property
     def is_valid(self) -> bool:
         valid = False
@@ -147,20 +272,25 @@
         else:
             valid = True
 
         return valid
 
 
 class ConsumerPowerflow(Solaredge2MQTTBaseModel):
-    house: int
-    evcharger: int = 0
-    inverter: int
+    house: int = Field(
+        **EntityType.POWER_W.field("House", "home-lightning-bolt-outline")
+    )
+
+    evcharger: int = Field(0, **EntityType.POWER_W.field("EV-Charger", "ev-station"))
 
-    used_production: int
-    battery_factor: float = Field(exclude=True)
+    inverter: int = Field(**EntityType.POWER_W.field("Inverter"))
+
+    used_production: int = Field(0, **EntityType.POWER_W.field("Used production"))
+
+    battery_factor: SkipJsonSchema[float] = Field(exclude=True)
 
     def __init__(
         self, inverter: InverterPowerflow, grid: GridPowerflow, evcharger: int
     ):
         house = int(abs(grid.power - inverter.power)) - evcharger
 
         battery_factor = inverter.battery_factor
@@ -174,29 +304,33 @@
             house=house,
             evcharger=evcharger,
             inverter=inverter.consumption,
             used_production=used_production,
             battery_factor=battery_factor,
         )
 
-    @computed_field
+    @computed_field(**EntityType.POWER_W.field("Total"))
     @property
     def total(self) -> int:
         return self.house + self.evcharger + self.inverter
 
-    @computed_field
+    @computed_field(
+        **EntityType.POWER_W.field("Used consumption"),
+    )
     @property
     def used_battery_production(self) -> int:
         battery_production = 0
         if self.used_production > 0 and self.battery_factor > 0:
             battery_production = int(round(self.used_production * self.battery_factor))
             battery_production = min(battery_production, self.used_production)
         return battery_production
 
-    @computed_field
+    @computed_field(
+        **EntityType.POWER_W.field("Used PV production"),
+    )
     @property
     def used_pv_production(self) -> int:
         return self.used_production - self.used_battery_production
 
     @property
     def is_valid(self) -> bool:
         valid = False
@@ -216,113 +350,7 @@
             logger.warning("Consumer total is negative")
         elif self.total < self.used_production:
             logger.warning("Consumer total is less than used production")
         else:
             valid = True
 
         return valid
-
-
-class Powerflow(Solaredge2MQTTBaseModel):
-    pv_production: int
-    inverter: InverterPowerflow
-    grid: GridPowerflow
-    battery: BatteryPowerflow
-    consumer: ConsumerPowerflow
-
-    last_powerflow: ClassVar[Powerflow] = None
-
-    @staticmethod
-    def from_modbus(
-        inverter_data: SunSpecInverter,
-        meters_data: dict[str, SunSpecMeter],
-        batteries_data: dict[str, SunSpecBattery],
-        evcharger: int = 0,
-    ) -> Powerflow:
-        grid = GridPowerflow.from_modbus(meters_data)
-        battery = BatteryPowerflow.from_modbus(batteries_data)
-
-        if inverter_data.ac.power.actual > 0:
-            pv_production = int(inverter_data.dc.power + battery.power)
-            if pv_production < 0:
-                pv_production = 0
-        else:
-            pv_production = 0
-
-        inverter = InverterPowerflow.from_modbus(inverter_data, battery)
-
-        consumer = ConsumerPowerflow(inverter, grid, evcharger)
-
-        return Powerflow(
-            pv_production=pv_production,
-            inverter=inverter,
-            grid=grid,
-            battery=battery,
-            consumer=consumer,
-        )
-
-    @property
-    def is_valid(self) -> bool:
-        valid = False
-
-        if self.pv_production < 0:
-            logger.warning("PV production is negative")
-        elif (
-            self.consumer.used_production + self.grid.delivery
-            != self.inverter.production
-        ):
-            logger.warning(
-                "Consumer used production + grid delivery is not equal to inverter production"
-            )
-        else:
-            valid = all(
-                [
-                    self.inverter.is_valid,
-                    self.grid.is_valid,
-                    self.battery.is_valid,
-                    self.consumer.is_valid,
-                ]
-            )
-
-        return valid
-
-    @classmethod
-    def is_not_valid_with_last(cls, powerflow: Powerflow) -> bool:
-        check = False
-
-        if cls.last_powerflow is not None:
-            check = all(
-                [
-                    cls.last_powerflow.pv_production == 0
-                    and powerflow.pv_production > 100,
-                ]
-            )
-
-        cls.last_powerflow = powerflow
-
-        return check
-
-    def prepare_point(self, measurement: str = "powerflow_raw") -> Point:
-        point = Point(measurement)
-        for key, value in self.model_dump_influxdb().items():
-            point.field(key, value)
-
-        return point
-
-    def prepare_point_energy(
-        self, measurement: str = "energy", prices: PriceSettings = None
-    ) -> Point:
-        point = Point(measurement)
-        for key, value in self.model_dump_influxdb().items():
-            energy = value / 1000
-            point.field(key, energy)
-            if prices is not None:
-                if key == "consumer_used_production":
-                    point.field("money_saved", energy * prices.price_in)
-                    point.field("money_price_in", prices.price_in)
-                elif key == "grid_delivery":
-                    point.field("money_delivered", energy * prices.price_out)
-                    point.field("money_price_out", prices.price_out)
-                elif key == "grid_consumption":
-                    point.field("money_consumed", energy * prices.price_out)
-
-        return point
```

### Comparing `solaredge2mqtt-1.0.9/solaredge2mqtt/models/weather.py` & `solaredge2mqtt-1.1.0/solaredge2mqtt/services/weather/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,26 @@
 from __future__ import annotations
 
 from datetime import datetime
 
 from pydantic import Field, field_serializer, model_serializer
 
-from solaredge2mqtt.models.base import Solaredge2MQTTBaseModel
+from solaredge2mqtt.core.models import Solaredge2MQTTBaseModel
 
 
-class OpenWeatherMapCondition(Solaredge2MQTTBaseModel):
-    id: int
-    main: str
-    description: str
-    icon: str = Field(exclude=True)
+class OpenWeatherMapOneCallBase(Solaredge2MQTTBaseModel):
+    lat: float
+    lon: float
+    timezone: str
+    timezone_offset: int
+
+
+class OpenWeatherMapOneCall(OpenWeatherMapOneCallBase):
+    current: OpenWeatherMapCurrentData
+    hourly: list[OpenWeatherMapForecastData]
 
 
 class OpenWeatherMapRain(Solaredge2MQTTBaseModel):
     one_hour: float = Field(0.0, alias="1h")
 
     @model_serializer
     def ser_model(self) -> float:
@@ -85,17 +90,12 @@
     sunset: datetime = Field(exclude=True)
 
 
 class OpenWeatherMapForecastData(OpenWeatherMapBaseData):
     pop: float
 
 
-class OpenWeatherMapOneCallBase(Solaredge2MQTTBaseModel):
-    lat: float
-    lon: float
-    timezone: str
-    timezone_offset: int
-
-
-class OpenWeatherMapOneCall(OpenWeatherMapOneCallBase):
-    current: OpenWeatherMapCurrentData
-    hourly: list[OpenWeatherMapForecastData]
+class OpenWeatherMapCondition(Solaredge2MQTTBaseModel):
+    id: int
+    main: str
+    description: str
+    icon: str = Field(exclude=True)
```

### Comparing `solaredge2mqtt-1.0.9/solaredge2mqtt/service/__init__.py` & `solaredge2mqtt-1.1.0/solaredge2mqtt/service.py`

 * *Files 17% similar despite different names*

```diff
@@ -2,93 +2,117 @@
     This module, service.py, is part of the SolarEdge2MQTT service, which reads data 
     from a SolarEdge inverter and publishes it to an MQTT broker. It uses the asyncio 
     library for asynchronous I/O and the aiomqtt library for MQTT communication. 
     The module also includes a run function to initialize and start the service.
 """
 
 import asyncio as aio
-import signal
 import platform
+import signal
 from time import time
 from typing import Callable
 
 from aiomqtt import MqttError
+from tzlocal import get_localzone_name
 
 from solaredge2mqtt import __version__
-from solaredge2mqtt.exceptions import ConfigurationException, InvalidDataException
-from solaredge2mqtt.logging import initialize_logging, logger
-from solaredge2mqtt.mqtt import MQTTClient
-from solaredge2mqtt.service.base import BaseLoops
-from solaredge2mqtt.service.forecast import Forecast
-from solaredge2mqtt.service.influxdb import InfluxDB
-from solaredge2mqtt.service.monitoring import MonitoringSite
-from solaredge2mqtt.service.weather import WeatherClient
-from solaredge2mqtt.settings import LOCAL_TZ, service_settings
+from solaredge2mqtt.core.events import EventBus
+from solaredge2mqtt.core.exceptions import ConfigurationException
+from solaredge2mqtt.core.influxdb import InfluxDB
+from solaredge2mqtt.core.logging import initialize_logging, logger
+from solaredge2mqtt.core.mqtt import MQTTClient
+from solaredge2mqtt.core.settings import service_settings
+from solaredge2mqtt.core.timer import Timer
+from solaredge2mqtt.services.energy import EnergyService
+from solaredge2mqtt.services.forecast import ForecastService
+from solaredge2mqtt.services.homeassistant import HomeAssistantDiscovery
+from solaredge2mqtt.services.monitoring import MonitoringSite
+from solaredge2mqtt.services.powerflow import PowerflowService
+from solaredge2mqtt.services.weather import WeatherClient
+
+LOCAL_TZ = get_localzone_name()
 
 
 def run():
     try:
         service = Service()
         loop = aio.get_event_loop()
         loop.add_signal_handler(signal.SIGINT, service.cancel)
         loop.add_signal_handler(signal.SIGTERM, service.cancel)
         loop.run_until_complete(service.main_loop())
-        loop.close()
     except ConfigurationException:
         logger.error("Configuration error")
+    except aio.exceptions.CancelledError:
+        logger.debug("Service cancelled")
+    finally:
+        loop.close()
 
 
 class Service:
     def __init__(self):
         self.settings = service_settings()
         initialize_logging(self.settings.logging_level)
         logger.debug(self.settings)
 
-        self.mqtt = MQTTClient(self.settings.mqtt)
+        self.event_bus = EventBus()
+        self.timer = Timer(self.event_bus, self.settings.interval)
+
+        self.mqtt = MQTTClient(self.settings.mqtt, self.event_bus)
 
         self.cancel_request = aio.Event()
         self.loops: set[aio.Task] = set()
 
         self.influxdb: InfluxDB | None = (
-            InfluxDB(self.settings.influxdb, self.settings.prices)
+            InfluxDB(self.settings.influxdb, self.settings.prices, self.event_bus)
             if self.settings.is_influxdb_configured
             else None
         )
 
-        self.basics = BaseLoops(self.settings, self.mqtt, self.influxdb)
+        self.energy: EnergyService | None = (
+            EnergyService(self.event_bus, self.influxdb)
+            if self.settings.is_influxdb_configured
+            else None
+        )
+
+        self.powerflow = PowerflowService(self.settings, self.event_bus, self.influxdb)
 
         self.monitoring: MonitoringSite | None = (
-            MonitoringSite(self.settings.monitoring, self.mqtt)
+            MonitoringSite(self.settings.monitoring, self.event_bus)
             if self.settings.is_monitoring_configured
             else None
         )
 
         self.weather: WeatherClient | None = (
-            WeatherClient(self.settings, self.mqtt)
+            WeatherClient(self.settings, self.event_bus)
             if self.settings.is_weather_configured
             else None
         )
 
-        self.forecast: Forecast | None = (
-            Forecast(
+        self.forecast: ForecastService | None = (
+            ForecastService(
                 self.settings.forecast,
                 self.settings.location,
-                self.mqtt,
+                self.event_bus,
                 self.influxdb,
-                self.weather,
             )
             if self.settings.is_forecast_configured
             else None
         )
 
+        self.homeassistant: HomeAssistantDiscovery | None = (
+            HomeAssistantDiscovery(self.settings, self.event_bus)
+            if self.settings.is_homeassistant_configured
+            else None
+        )
+
     def cancel(self):
         logger.info("Stopping SolarEdge2MQTT service...")
         self.cancel_request.set()
-        for loop in self.loops:
-            loop.cancel()
+        for tasks in aio.all_tasks():
+            tasks.cancel()
 
     async def main_loop(self):
         logger.info("Starting SolarEdge2MQTT service...")
         logger.info("Version: {version}", version=__version__)
         logger.info(
             f"Operationg system: {platform.platform()} ({platform.system()}/{platform.machine()})"
         )
@@ -99,91 +123,81 @@
             self.influxdb.initialize_buckets()
 
         while not self.cancel_request.is_set():
             try:
                 async with self.mqtt:
                     await self.mqtt.publish_status_online()
 
-                    self.schedule_loop(
-                        self.settings.interval, self.basics.powerflow_loop
-                    )
-
-                    self.schedule_influxdb_loops()
+                    if self.settings.is_homeassistant_configured:
+                        await self.homeassistant.async_init()
 
-                    self.schedule_monitoring_loop()
-
-                    await self.schedule_weather_loops()
+                    self._start_mqtt_listener()
+                    self.schedule_loop(1, self.timer.loop)
 
                     await aio.gather(*self.loops)
-
-                    await self.mqtt.publish_status_offline()
-
             except MqttError:
                 logger.error("MQTT error, reconnecting in 5 seconds...")
                 await aio.sleep(5)
             except aio.exceptions.CancelledError:
                 logger.debug("Loops cancelled")
                 return
             finally:
-                for loop in self.loops:
-                    loop.cancel()
+                await self.finalize()
 
-    def schedule_monitoring_loop(self):
-        if self.settings.is_monitoring_configured:
-            self.monitoring.login()
-            self.schedule_loop(300, self.monitoring.loop)
+    async def finalize(self):
+        try:
+            await self.mqtt.publish_status_offline()
+        except MqttError:
+            pass
+
+        try:
+            self.event_bus.cancel_tasks()
+        finally:
+            pass
 
-    def schedule_influxdb_loops(self):
-        if self.settings.is_influxdb_configured:
-            loop_handles = [self.influxdb.loop, self.basics.energy_loop]
-            if self.settings.is_forecast_configured:
-                loop_handles.append(self.forecast.training_loop)
-
-            self.schedule_loop(600, loop_handles)
-
-    async def schedule_weather_loops(self):
-        if self.settings.is_weather_configured:
-            self.schedule_loop(600, self.weather.loop)
+        for task in self.loops:
+            try:
+                task.cancel()
+            finally:
+                pass
 
-            if self.settings.is_forecast_configured:
-                self.schedule_loop(600, self.forecast.forecast_loop, True)
+    def _start_mqtt_listener(self):
+        task = aio.create_task(self.mqtt.listen())
+        self.loops.add(task)
+        task.add_done_callback(self.loops.remove)
 
     def schedule_loop(
         self,
         interval_in_seconds: int,
         handles: Callable | list[Callable],
-        delay_start: bool = False,
+        delay_start: int = 0,
         args: list[any] = None,
     ):
         loop = aio.create_task(
             self.run_loop(interval_in_seconds, handles, delay_start, args)
         )
         self.loops.add(loop)
         loop.add_done_callback(self.loops.remove)
 
     async def run_loop(
         self,
         interval_in_seconds: int,
         handles: Callable | list[Callable],
-        delay_start: bool = False,
+        delay_start: int = 0,
         args: list[any] = None,
     ):
         if not isinstance(handles, list):
             handles = [handles]
 
-        if delay_start:
-            await aio.sleep(interval_in_seconds)
+        await aio.sleep(delay_start)
 
         while not self.cancel_request.is_set():
             execution_time = 0
-            try:
-                start_time = time()
-                for handle in handles:
-                    await handle(*args or [])
-                execution_time = time() - start_time
-            except InvalidDataException as error:
-                logger.warning("{message}, skipping this loop", message=error.message)
+            start_time = time()
+            for handle in handles:
+                await handle(*args or [])
+            execution_time = time() - start_time
 
             if execution_time < interval_in_seconds:
                 await aio.sleep(interval_in_seconds - execution_time)
             else:
                 await aio.sleep(interval_in_seconds)
```

### Comparing `solaredge2mqtt-1.0.9/solaredge2mqtt/service/http.py` & `solaredge2mqtt-1.1.0/solaredge2mqtt/services/http.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from json import loads as json_loads
 from typing import Callable
 
 from requests import session
 from requests.exceptions import ConnectionError as RequestsConnectionError
 from requests.exceptions import Timeout, HTTPError
 
-from solaredge2mqtt.logging import logger
+from solaredge2mqtt.core.logging import logger
 
 
 class HTTPClient:
     def __init__(self, service: str) -> None:
         self.session = session()
         self.service = service
```

### Comparing `solaredge2mqtt-1.0.9/solaredge2mqtt/service/influxdb.py` & `solaredge2mqtt-1.1.0/solaredge2mqtt/core/influxdb/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,30 +1,52 @@
+from __future__ import annotations
+
 from datetime import datetime, timedelta, timezone
+from typing import TYPE_CHECKING
 
 import pkg_resources
 from influxdb_client import BucketRetentionRules, InfluxDBClient, Point
 from influxdb_client.client.exceptions import InfluxDBError
 from influxdb_client.client.influxdb_client_async import (
     InfluxDBClientAsync,
     QueryApiAsync,
 )
 from pandas import DataFrame
+from tzlocal import get_localzone_name
+
+from solaredge2mqtt.core.events import EventBus
+from solaredge2mqtt.core.influxdb.events import InfluxDBAggregatedEvent
+from solaredge2mqtt.core.influxdb.settings import InfluxDBSettings
+from solaredge2mqtt.core.logging import logger
+from solaredge2mqtt.core.timer.events import Interval10MinTriggerEvent
+
+if TYPE_CHECKING:
+    from solaredge2mqtt.services.energy.models import HistoricPeriod
+    from solaredge2mqtt.services.energy.settings import PriceSettings
+
 
-from solaredge2mqtt.logging import logger
-from solaredge2mqtt.models import ForecastPeriod, HistoricPeriod
-from solaredge2mqtt.settings import LOCAL_TZ, InfluxDBSettings, PriceSettings
+LOCAL_TZ = get_localzone_name()
 
 
 class InfluxDB:
-    def __init__(self, settings: InfluxDBSettings, prices: PriceSettings) -> None:
+    def __init__(
+        self,
+        settings: InfluxDBSettings,
+        prices: PriceSettings,
+        event_bus: EventBus | None = None,
+    ) -> None:
         self.settings: InfluxDBSettings = settings
         self.prices: PriceSettings = prices
 
+        self.event_bus = event_bus
+        if self.event_bus:
+            self._subscribe_events()
+
         self.client: InfluxDBClient = InfluxDBClient(
-            url=f"{settings.host}:{settings.port}",
+            url=settings.url,
             token=settings.token.get_secret_value(),
             org=settings.org,
         )
 
         self.write_api = self.client.write_api(
             success_callback=self.write_success_callback,
             error_callback=self.write_error_callback,
@@ -35,14 +57,17 @@
         self.delete_api = self.client.delete_api()
 
         self.client_async: InfluxDBClientAsync | None = None
         self.query_api_async: QueryApiAsync | None = None
 
         self.flux_cache: dict[str, str] = {}
 
+    def _subscribe_events(self) -> None:
+        self.event_bus.subscribe(Interval10MinTriggerEvent, self.loop)
+
     def initialize_buckets(self) -> None:
         buckets_api = self.client.buckets_api()
         bucket = buckets_api.find_bucket_by_name(self.bucket_name)
         retention_rules = BucketRetentionRules(
             type="expire", every_seconds=self.settings.retention
         )
 
@@ -57,15 +82,15 @@
                 logger.info(
                     f"Updating retention rules for bucket '{self.bucket_name}' "
                     + f"to {self.settings.retention} seconds."
                 )
                 bucket.retention_rules[0] = retention_rules
                 buckets_api.update_bucket(bucket=bucket)
 
-    async def loop(self) -> None:
+    async def loop(self, _) -> None:
         now = datetime.now(tz=timezone.utc).replace(minute=0, second=0, microsecond=0)
 
         logger.info("Aggregate powerflow and energy raw data")
         aggregate_query = self._get_flux_query(
             "aggregate",
             {"PRICE_IN": self.prices.price_in, "PRICE_OUT": self.prices.price_out},
         )
@@ -75,14 +100,17 @@
         retention_time = now - timedelta(hours=self.settings.retention_raw)
         self.delete_from_measurements(
             datetime(1970, 1, 1, tzinfo=timezone.utc),
             retention_time,
             ["powerflow_raw", "battery_raw"],
         )
 
+        if self.event_bus:
+            await self.event_bus.emit(InfluxDBAggregatedEvent())
+
     def delete_from_measurements(
         self, start: datetime, stop: datetime, measurements: list[str]
     ) -> None:
         for measurement in measurements:
             self.delete_from_measurement(start, stop, measurement)
 
     def delete_from_measurement(
@@ -115,15 +143,15 @@
     def write_error_callback(
         self, conf: tuple[str, str, str], data: str, error: InfluxDBError
     ) -> None:
         logger.error(f"InfluxDB error while writting: {conf} {error}")
         logger.debug(data)
 
     def query_timeunit(
-        self, period: HistoricPeriod | ForecastPeriod, measurement: str
+        self, period: HistoricPeriod, measurement: str
     ) -> dict[str, any] | None:
         return self.query_first(
             period.query.query, {"UNIT": period.unit, "MEASUREMENT": measurement}
         )
 
     def query_first(
         self, query_name: str, additional_replacements: dict[str, any] | None = None
@@ -147,26 +175,26 @@
         async with self.client_async:
             return await self.query_api_async.query_data_frame(
                 self._get_flux_query(query_name, additional_replacements)
             )
 
     async def init_client_async(self) -> None:
         self.client_async = InfluxDBClientAsync(
-            url=f"{self.settings.host}:{self.settings.port}",
+            url=self.settings.url,
             token=self.settings.token.get_secret_value(),
             org=self.settings.org,
         )
         self.query_api_async = self.client_async.query_api()
 
     def _get_flux_query(
         self, query_name: str, additional_replacements: dict[str, any] | None = None
     ) -> str:
         if query_name not in self.flux_cache:
             flux = pkg_resources.resource_string(
-                __name__, f"../flux/{query_name}.flux"
+                __name__, f"./flux/{query_name}.flux"
             ).decode("utf-8")
             flux = (
                 flux.replace("{{BUCKET_AGGREGATED}}", self.bucket_name)
                 .replace("{{BUCKET_NAME}}", self.bucket_name)
                 .replace("{{TIMEZONE}}", LOCAL_TZ)
             )
             self.flux_cache[query_name] = flux
```

### Comparing `solaredge2mqtt-1.0.9/solaredge2mqtt/service/modbus.py` & `solaredge2mqtt-1.1.0/solaredge2mqtt/services/modbus/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,38 +1,52 @@
 import json
 
 from pymodbus.exceptions import ModbusException
 from solaredge_modbus import Inverter
 
-from solaredge2mqtt.exceptions import InvalidDataException
-from solaredge2mqtt.logging import LOGGING_DEVICE_INFO, logger
-from solaredge2mqtt.models import SunSpecBattery, SunSpecInverter, SunSpecMeter
-from solaredge2mqtt.settings import ModbusSettings
+from solaredge2mqtt.core.events import EventBus
+from solaredge2mqtt.core.exceptions import InvalidDataException
+from solaredge2mqtt.core.logging import logger
+from solaredge2mqtt.services.modbus.events import (
+    ModbusBatteriesReadEvent,
+    ModbusInverterReadEvent,
+    ModbusMetersReadEvent,
+)
+from solaredge2mqtt.services.modbus.models import (
+    SunSpecBattery,
+    SunSpecInverter,
+    SunSpecMeter,
+)
+from solaredge2mqtt.services.modbus.settings import ModbusSettings
 
 SunSpecRawData = dict[str, str | int]
 
+LOGGING_DEVICE_INFO = "{device} ({info.manufacturer} {info.model} {info.serialnumber})"
+
 
 class Modbus:
     inverter: Inverter
 
-    def __init__(self, settings: ModbusSettings):
+    def __init__(self, settings: ModbusSettings, event_bus: EventBus):
         self.inverter = Inverter(
             host=settings.host,
             port=settings.port,
             timeout=settings.timeout,
             unit=settings.unit,
         )
 
         logger.info(
             "Using SolarEdge inverter via modbus: {host}:{port}",
             host=settings.host,
             port=settings.port,
         )
 
-    async def loop(
+        self.event_bus = event_bus
+
+    async def get_data(
         self,
     ) -> (
         tuple[
             SunSpecInverter | None,
             dict[str, SunSpecMeter] | None,
             dict[str, SunSpecBattery | None],
         ]
@@ -47,14 +61,20 @@
 
             inverter_data = self._map_inverter(inverter_raw)
             meters_data = self._map_meters(meters_raw)
             batteries_data = self._map_batteries(batteries_raw)
         except (ModbusException, KeyError) as error:
             raise InvalidDataException("Invalid modbus data") from error
 
+        await self.event_bus.emit(ModbusInverterReadEvent(inverter_data))
+        if meters_data:
+            await self.event_bus.emit(ModbusMetersReadEvent(meters_data))
+        if batteries_data:
+            await self.event_bus.emit(ModbusBatteriesReadEvent(batteries_data))
+
         return inverter_data, meters_data, batteries_data
 
     def _get_raw_data(
         self,
     ) -> tuple[SunSpecRawData, dict[str, SunSpecRawData], dict[str, SunSpecRawData]]:
         inverter_raw = self.inverter.read_all()
         meters_raw = {
```

### Comparing `solaredge2mqtt-1.0.9/solaredge2mqtt/service/monitoring.py` & `solaredge2mqtt-1.1.0/solaredge2mqtt/services/monitoring/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,33 +1,39 @@
 from requests.exceptions import HTTPError
 
-from solaredge2mqtt.exceptions import ConfigurationException, InvalidDataException
-from solaredge2mqtt.logging import logger
-from solaredge2mqtt.models import (
+from solaredge2mqtt.core.events import EventBus
+from solaredge2mqtt.core.exceptions import ConfigurationException, InvalidDataException
+from solaredge2mqtt.core.logging import logger
+from solaredge2mqtt.core.mqtt.events import MQTTPublishEvent
+from solaredge2mqtt.core.timer.events import Interval10MinTriggerEvent
+from solaredge2mqtt.services.http import HTTPClient
+from solaredge2mqtt.services.monitoring.models import (
     LogicalInfo,
     LogicalInverter,
     LogicalModule,
     LogicalString,
 )
-from solaredge2mqtt.mqtt import MQTTClient
-from solaredge2mqtt.service.http import HTTPClient
-from solaredge2mqtt.settings import MonitoringSettings
+from solaredge2mqtt.services.monitoring.settings import MonitoringSettings
 
 LOGIN_URL = "https://monitoring.solaredge.com/solaredge-apigw/api/login"
 LOGICAL_URL = "https://monitoring.solaredge.com/solaredge-apigw/api/sites/{site_id}/layout/logical"
 
 
 class MonitoringSite(HTTPClient):
-    def __init__(self, settings: MonitoringSettings, mqtt: MQTTClient) -> None:
+    def __init__(self, settings: MonitoringSettings, event_bus: EventBus) -> None:
         super().__init__("Monitoring Site")
         self.settings = settings
 
-        self.mqtt = mqtt
+        self.event_bus = event_bus
+        self._subscribe_events()
 
-    async def loop(self):
+    def _subscribe_events(self) -> None:
+        self.event_bus.subscribe(Interval10MinTriggerEvent, self.get_data)
+
+    async def get_data(self, _):
         modules = self.get_module_energies()
 
         if modules is None:
             logger.warning("Invalid monitoring data, skipping this loop")
             return
 
         energy_total = 0
@@ -39,19 +45,24 @@
 
         logger.info(
             "Read from monitoring total energy: {energy_total} kWh from {count_modules} modules",
             energy_total=energy_total / 1000,
             count_modules=count_modules,
         )
 
-        await self.mqtt.publish_to("monitoring/pv_energy_today", energy_total)
+        await self.event_bus.emit(
+            MQTTPublishEvent("monitoring/pv_energy_today", energy_total)
+        )
+
         for module in modules:
-            await self.mqtt.publish_to(
-                f"monitoring/module/{module.info.serialnumber}",
-                module,
+            await self.event_bus.emit(
+                MQTTPublishEvent(
+                    f"monitoring/module/{module.info.serialnumber}",
+                    module,
+                )
             )
 
     def login(self) -> None:
         try:
             self._post(
                 LOGIN_URL,
                 headers={"Content-Type": "application/x-www-form-urlencoded"},
@@ -62,15 +73,15 @@
                 timeout=10,
                 expect_json=False,
             )
 
             logger.info("Login to monitoring site successful")
         except HTTPError as error:
             raise ConfigurationException(
-                "Monitoring","Unable to login to monitoring account"
+                "Monitoring", "Unable to login to monitoring account"
             ) from error
 
     def get_module_energies(self) -> list[LogicalInverter] | None:
         modules = None
         logical = self._get_logical()
 
         if logical is None:
@@ -93,14 +104,17 @@
                     modules.append(module)
 
         return modules
 
     def _get_logical(self) -> dict | None:
         result = None
         try:
+            if "CSRF-TOKEN" not in self.session.cookies:
+                self.login()
+
             result = self._get(
                 LOGICAL_URL.format(site_id=self.settings.site_id),
                 headers={
                     "Content-Type": "application/x-www-form-urlencoded",
                     "X-CSRF-TOKEN": self.session.cookies["CSRF-TOKEN"],
                 },
                 timeout=10,
```

### Comparing `solaredge2mqtt-1.0.9/solaredge2mqtt/service/wallbox.py` & `solaredge2mqtt-1.1.0/solaredge2mqtt/services/wallbox/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 import time
 
 import jwt
 import urllib3
 from pydantic import BaseModel, Field
 from requests.exceptions import HTTPError
 
-from solaredge2mqtt.exceptions import ConfigurationException, InvalidDataException
-from solaredge2mqtt.logging import logger
-from solaredge2mqtt.models import WallboxAPI
-from solaredge2mqtt.settings import WallboxSettings
-from solaredge2mqtt.service.http import HTTPClient
+from solaredge2mqtt.core.events import EventBus
+from solaredge2mqtt.core.exceptions import ConfigurationException, InvalidDataException
+from solaredge2mqtt.services.http import HTTPClient
+from solaredge2mqtt.core.logging import logger
+from solaredge2mqtt.services.wallbox.events import WallboxReadEvent
+from solaredge2mqtt.services.wallbox.models import WallboxAPI
+from solaredge2mqtt.services.wallbox.settings import WallboxSettings
 
 urllib3.disable_warnings()
 
 LOGIN_URL = "https://{host}:8443/v2/jwt/login"
 REFRESH_URL = "https://{host}:8443/v2/jwt/refresh"
 WALLBOX_URL = "https://{host}:8443/v2/wallboxes/{serial}"
 
@@ -32,26 +34,27 @@
     def refresh_token_expires(self) -> int:
         payload = jwt.decode(self.refresh_token, options={"verify_signature": False})
         logger.debug("Refresh token expires at: {expires}", expires=payload["exp"])
         return payload["exp"]
 
 
 class WallboxClient(HTTPClient):
-    def __init__(self, settings: WallboxSettings):
+    def __init__(self, settings: WallboxSettings, event_bus: EventBus):
         super().__init__("Wallbox API")
         self.settings = settings
 
         logger.info(
             "Using Wallbox charger: {host}",
             host=settings.host,
         )
 
+        self.event_bus = event_bus
         self.authorization: AuthorizationTokens | None = None
 
-    async def loop(self) -> WallboxAPI | None:
+    async def get_data(self) -> WallboxAPI | None:
         wallbox = None
         try:
             self._get_access()
 
             response = self._get(
                 WALLBOX_URL.format(
                     host=self.settings.host, serial=self.settings.serial
@@ -65,14 +68,16 @@
                 raise InvalidDataException("Invalid Wallbox data")
 
             wallbox = WallboxAPI(response)
             logger.info(
                 f"Wallbox: {wallbox.state}, {wallbox.power / 1000} kW",
                 wallbox=wallbox,
             )
+
+            await self.event_bus.emit(WallboxReadEvent(wallbox))
         except HTTPError as error:
             raise InvalidDataException(f"Cannot read Wallbox data: {error}") from error
 
         return wallbox
 
     def _get_access(self) -> None:
         current_timestamp = int(time.time())
```

### Comparing `solaredge2mqtt-1.0.9/solaredge2mqtt/service/weather.py` & `solaredge2mqtt-1.1.0/solaredge2mqtt/services/weather/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,35 +1,50 @@
+from __future__ import annotations
+
+from typing import TYPE_CHECKING
+
 from requests.exceptions import HTTPError
 
-from solaredge2mqtt.exceptions import InvalidDataException
-from solaredge2mqtt.logging import logger
-from solaredge2mqtt.models import OpenWeatherMapOneCall
-from solaredge2mqtt.mqtt import MQTTClient
-from solaredge2mqtt.service.http import HTTPClient
-from solaredge2mqtt.settings import ServiceSettings
+from solaredge2mqtt.core.events import EventBus
+from solaredge2mqtt.core.exceptions import InvalidDataException
+from solaredge2mqtt.services.http import HTTPClient
+from solaredge2mqtt.core.logging import logger
+from solaredge2mqtt.core.mqtt.events import MQTTPublishEvent
+from solaredge2mqtt.core.timer.events import Interval10MinTriggerEvent
+from solaredge2mqtt.services.weather.events import WeatherUpdateEvent
+from solaredge2mqtt.services.weather.models import OpenWeatherMapOneCall
+
+if TYPE_CHECKING:
+    from solaredge2mqtt.core.settings import ServiceSettings
 
 ONECALL_URL = "https://api.openweathermap.org/data/3.0/onecall"
 TIMEMACHINE_URL = "https://api.openweathermap.org/data/3.0/onecall/timemachine"
 
 
 class WeatherClient(HTTPClient):
-    def __init__(self, settings: ServiceSettings, mqtt: MQTTClient) -> None:
+    def __init__(self, settings: ServiceSettings, event_bus: EventBus) -> None:
         super().__init__("Weather API")
 
         self.location = settings.location
         self.settings = settings.weather
 
-        self.mqtt = mqtt
+        self.event_bus = event_bus
+        self._subscribe_events()
+
+    def _subscribe_events(self):
+        self.event_bus.subscribe(Interval10MinTriggerEvent, self.loop)
 
-    async def loop(self):
+    async def loop(self, _):
         weather = self.get_weather()
-        await self.mqtt.publish_to("weather/current", weather.current)
+        await self.event_bus.emit(WeatherUpdateEvent(weather))
+        await self.event_bus.emit(MQTTPublishEvent("weather/current", weather.current))
 
     def get_weather(self) -> OpenWeatherMapOneCall:
         try:
+            logger.info("Reading weather data from OpenWeatherMap")
             result = self._get(
                 ONECALL_URL,
                 params={
                     "lat": self.location.latitude,
                     "lon": self.location.longitude,
                     "exclude": "minutely,daily,alerts",
                     "units": "metric",
```

### Comparing `solaredge2mqtt-1.0.9/solaredge2mqtt.egg-info/PKG-INFO` & `solaredge2mqtt-1.1.0/solaredge2mqtt.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: solaredge2mqtt
-Version: 1.0.9
+Version: 1.1.0
 Summary: Read data from SolarEdge Inverter and publish it to MQTT
 Home-page: https://github.com/deroetzi/solaredge2mqtt
 Author: Johannes Ott
 Author-email: info@johannes-ott.net
 Project-URL: Bug Reports, https://github.com/deroetzi/solaredge2mqtt/issues
 Keywords: smart home
 Classifier: Development Status :: 5 - Production/Stable
@@ -13,29 +13,30 @@
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.10, <4
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: solaredge_modbus==0.8.0
-Requires-Dist: pydantic==2.7.0
+Requires-Dist: aiocsv==1.3.2
+Requires-Dist: aiohttp==3.9.5
+Requires-Dist: aiomqtt==2.1.0
+Requires-Dist: astral==3.2
+Requires-Dist: ephem==4.1.5
+Requires-Dist: influxdb-client==1.43.0
+Requires-Dist: jsonref==1.1.0
 Requires-Dist: loguru==0.7.2
-Requires-Dist: requests==2.31.0
-Requires-Dist: influxdb-client==1.41.0
-Requires-Dist: pyjwt==2.8.0
-Requires-Dist: aiomqtt==2.0.1
 Requires-Dist: numpy==1.26.4
 Requires-Dist: pandas==2.2.2
+Requires-Dist: pydantic==2.7.1
+Requires-Dist: pyjwt==2.8.0
+Requires-Dist: requests==2.31.0
 Requires-Dist: scikit-learn==1.4.2
-Requires-Dist: scipy==1.13.0rc1
-Requires-Dist: aiohttp==3.9.4
-Requires-Dist: aiocsv==1.3.1
-Requires-Dist: astral==3.2
-Requires-Dist: ephem==4.1.5
+Requires-Dist: scipy==1.13.0
+Requires-Dist: solaredge_modbus==0.8.0
 Requires-Dist: tzlocal==5.2
 
 # SolarEdge 2 MQTT Service
 
 [![License](https://img.shields.io/github/license/DerOetzi/solaredge2mqtt)](https://github.com/DerOetzi/solaredge2mqtt/blob/main/LICENSE) [![Release](https://img.shields.io/github/v/release/DerOetzi/solaredge2mqtt)](https://github.com/DerOetzi/solaredge2mqtt/releases/latest) [![Build Status](https://img.shields.io/github/actions/workflow/status/DerOetzi/solaredge2mqtt/build_project.yml?branch=main)](https://github.com/DerOetzi/solaredge2mqtt/actions/workflows/build_project.yml) [![PyPI version](https://img.shields.io/pypi/v/solaredge2mqtt.svg)](https://pypi.org/project/solaredge2mqtt/) [![Discord Chat](https://img.shields.io/discord/1196540254686032014)](https://discord.gg/QXfghc93pY)
 
 The SolarEdge2MQTT service facilitates the retrieval of power data from SolarEdge inverters and its publication to an MQTT broker. Ideal for integrating SolarEdge inverters into home automation systems, this service supports real-time monitoring of power flow and additional parameters via Modbus.
@@ -93,14 +94,23 @@
 
 For monitoring SolarEdge Wallbox, provide:
 
 - **SE2MQTT_WALLBOX\_\_HOST**: The IP address of your Wallbox.
 - **SE2MQTT_WALLBOX\_\_PASSWORD**: The admin password for Wallbox web UI access.
 - **SE2MQTT_WALLBOX\_\_SERIAL**: The serial number of your Wallbox.
 
+### Home Assistant Auto Discovery
+
+If you want Home Assistant to auto discover the data SolarEdge2MQTT provides, you can enable this here.
+
+- **SE2MQTT_HOMEASSISTANT\_\_ENABLE**: Set to true to enable the auto discovery
+- **SE2MQTT_HOMEASSISTANT\_\_TOPIC_PREFIX**: By default Home Assistant MQTT integration listens to subtopics of homeassistant
+
+_If you want to remove things, just disable the feature, then restart SolarEdge2MQTT first and after it restart Home Assistant,_
+
 ### InfluxDB
 
 Configure your InfluxDB settings with these environment variables to store monitoring data effectively:
 
 - **SE2MQTT_INFLUXDB\_\_HOST**: Specify the host of your InfluxDB instance (e.g., http://localhost). Default is None.
 - **SE2MQTT_INFLUXDB\_\_PORT**: The port number on which your InfluxDB instance is running. The default value is 8086.
 - **SE2MQTT_INFLUXDB\_\_TOKEN**: Your access token for InfluxDB. It is imperative to use this token securely, especially when deploying with Docker. The token requires full access since the service will be managing necessary buckets and tasks. Default is None.
```

### Comparing `solaredge2mqtt-1.0.9/versioneer.py` & `solaredge2mqtt-1.1.0/versioneer.py`

 * *Files identical despite different names*

