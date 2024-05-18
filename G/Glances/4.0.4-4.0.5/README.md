# Comparing `tmp/glances-4.0.4.tar.gz` & `tmp/glances-4.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "glances-4.0.4.tar", last modified: Wed May 15 09:25:11 2024, max compression
+gzip compressed data, was "glances-4.0.5.tar", last modified: Sat May 18 09:31:20 2024, max compression
```

## Comparing `glances-4.0.4.tar` & `glances-4.0.5.tar`

### file list

```diff
@@ -1,406 +1,408 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 09:25:11.852857 glances-4.0.4/
--rw-r--r--   0 runner    (1001) docker     (127)     1861 2024-05-15 09:25:06.000000 glances-4.0.4/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (127)     6086 2024-05-15 09:25:06.000000 glances-4.0.4/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)    42098 2024-05-15 09:25:06.000000 glances-4.0.4/COPYING
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 09:25:11.848857 glances-4.0.4/Glances.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    20541 2024-05-15 09:25:11.000000 glances-4.0.4/Glances.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     9997 2024-05-15 09:25:11.000000 glances-4.0.4/Glances.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 09:25:11.000000 glances-4.0.4/Glances.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-15 09:25:11.000000 glances-4.0.4/Glances.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      728 2024-05-15 09:25:11.000000 glances-4.0.4/Glances.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-15 09:25:11.000000 glances-4.0.4/Glances.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      217 2024-05-15 09:25:06.000000 glances-4.0.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    72575 2024-05-15 09:25:06.000000 glances-4.0.4/NEWS.rst
--rw-r--r--   0 runner    (1001) docker     (127)    20541 2024-05-15 09:25:11.852857 glances-4.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    16704 2024-05-15 09:25:06.000000 glances-4.0.4/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 09:25:11.788856 glances-4.0.4/conf/
--rw-r--r--   0 runner    (1001) docker     (127)    23758 2024-05-15 09:25:06.000000 glances-4.0.4/conf/glances.conf
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 09:25:11.788856 glances-4.0.4/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     7769 2024-05-15 09:25:06.000000 glances-4.0.4/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)      281 2024-05-15 09:25:06.000000 glances-4.0.4/docs/README.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 09:25:11.808857 glances-4.0.4/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (127)     5175 2024-05-15 09:25:06.000000 glances-4.0.4/docs/_static/Glances Logo dark.svg
--rw-r--r--   0 runner    (1001) docker     (127)     5185 2024-05-15 09:25:06.000000 glances-4.0.4/docs/_static/Glances Logo.svg
--rw-r--r--   0 runner    (1001) docker     (127)    10756 2024-05-15 09:25:06.000000 glances-4.0.4/docs/_static/Glances Text Logo dark.svg
--rw-r--r--   0 runner    (1001) docker     (127)    10775 2024-05-15 09:25:06.000000 glances-4.0.4/docs/_static/Glances Text Logo.svg
--rw-r--r--   0 runner    (1001) docker     (127)    29273 2024-05-15 09:25:06.000000 glances-4.0.4/docs/_static/amp-dropbox.png
--rw-r--r--   0 runner    (1001) docker     (127)     9474 2024-05-15 09:25:06.000000 glances-4.0.4/docs/_static/amp-python-warning.png
--rw-r--r--   0 runner    (1001) docker     (127)     9362 2024-05-15 09:25:06.000000 glances-4.0.4/docs/_static/amp-python.png
--rw-r--r--   0 runner    (1001) docker     (127)    80498 2024-05-15 09:25:06.000000 glances-4.0.4/docs/_static/amps.png
--rw-r--r--   0 runner    (1001) docker     (127)    13916 2024-05-15 09:25:06.000000 glances-4.0.4/docs/_static/aws.png
--rw-r--r--   0 runner    (1001) docker     (127)    44160 2024-05-15 09:25:06.000000 glances-4.0.4/docs/_static/browser.png
--rw-r--r--   0 runner    (1001) docker     (127)    21111 2024-05-15 09:25:06.000000 glances-4.0.4/docs/_static/cloud.png
--rw-r--r--   0 runner    (1001) docker     (127)     9442 2024-05-15 09:25:06.000000 glances-4.0.4/docs/_static/connected.png
--rw-r--r--   0 runner    (1001) docker     (127)    29245 2024-05-15 09:25:06.000000 glances-4.0.4/docs/_static/connections.png
--rw-r--r--   0 runner    (1001) docker     (127)    34093 2024-05-15 09:25:06.000000 glances-4.0.4/docs/_static/containers.png
--rw-r--r--   0 runner    (1001) docker     (127)    11799 2024-05-15 09:25:06.000000 glances-4.0.4/docs/_static/cpu-wide.png
--rw-r--r--   0 runner    (1001) docker     (127)     4504 2024-05-15 09:25:06.000000 glances-4.0.4/docs/_static/cpu.png
--rw-r--r--   0 runner    (1001) docker     (127)    10031 2024-05-15 09:25:06.000000 glances-4.0.4/docs/_static/disconnected.png
--rw-r--r--   0 runner    (1001) docker     (127)     9638 2024-05-15 09:25:06.000000 glances-4.0.4/docs/_static/diskio.png
--rw-r--r--   0 runner    (1001) docker     (127)    24808 2024-05-15 09:25:06.000000 glances-4.0.4/docs/_static/events.png
--rw-r--r--   0 runner    (1001) docker     (127)    13715 2024-05-15 09:25:06.000000 glances-4.0.4/docs/_static/folders.png
--rw-r--r--   0 runner    (1001) docker     (127)    10950 2024-05-15 09:25:06.000000 glances-4.0.4/docs/_static/fs.png
--rw-r--r--   0 runner    (1001) docker     (127)    56273 2024-05-15 09:25:06.000000 glances-4.0.4/docs/_static/glances-architecture.excalidraw
--rw-r--r--   0 runner    (1001) docker     (127)   123499 2024-05-15 09:25:06.000000 glances-4.0.4/docs/_static/glances-architecture.png
--rw-r--r--   0 runner    (1001) docker     (127)    92793 2024-05-15 09:25:06.000000 glances-4.0.4/docs/_static/glances-cgraph.svg
--rw-r--r--   0 runner    (1001) docker     (127)   114983 2024-05-15 09:25:06.000000 glances-4.0.4/docs/_static/glances-flame.svg
--rw-r--r--   0 runner    (1001) docker     (127)     9404 2024-05-15 09:25:06.000000 glances-4.0.4/docs/_static/glances-influxdb.png
--rw-r--r--   0 runner    (1001) docker     (127)    33567 2024-05-15 09:25:06.000000 glances-4.0.4/docs/_static/glances-memory-profiling-with-history.png
--rw-r--r--   0 runner    (1001) docker     (127)    31797 2024-05-15 09:25:06.000000 glances-4.0.4/docs/_static/glances-memory-profiling-without-history.png
--rw-r--r--   0 runner    (1001) docker     (127)    29500 2024-05-15 09:25:06.000000 glances-4.0.4/docs/_static/glances-pyinstrument.html
--rw-r--r--   0 runner    (1001) docker     (127)   295283 2024-05-15 09:25:06.000000 glances-4.0.4/docs/_static/glances-responsive-webdesign.png
--rw-r--r--   0 runner    (1001) docker     (127)   435038 2024-05-15 09:25:06.000000 glances-4.0.4/docs/_static/glances-summary.png
--rw-r--r--   0 runner    (1001) docker     (127)     3865 2024-05-15 09:25:06.000000 glances-4.0.4/docs/_static/gpu.png
--rw-r--r--   0 runner    (1001) docker     (127)   141657 2024-05-15 09:25:06.000000 glances-4.0.4/docs/_static/grafana.png
--rw-r--r--   0 runner    (1001) docker     (127)   187140 2024-05-15 09:25:06.000000 glances-4.0.4/docs/_static/graph-load.svg
--rw-r--r--   0 runner    (1001) docker     (127)    14415 2024-05-15 09:25:06.000000 glances-4.0.4/docs/_static/hddtemp.png
--rw-r--r--   0 runner    (1001) docker     (127)    19879 2024-05-15 09:25:06.000000 glances-4.0.4/docs/_static/header.png
--rw-r--r--   0 runner    (1001) docker     (127)    12750 2024-05-15 09:25:06.000000 glances-4.0.4/docs/_static/ip.png
--rw-r--r--   0 runner    (1001) docker     (127)     3980 2024-05-15 09:25:06.000000 glances-4.0.4/docs/_static/irq.png
--rw-r--r--   0 runner    (1001) docker     (127)     6923 2024-05-15 09:25:06.000000 glances-4.0.4/docs/_static/load.png
--rw-r--r--   0 runner    (1001) docker     (127)    20009 2024-05-15 09:25:06.000000 glances-4.0.4/docs/_static/loadpercent.png
--rw-r--r--   0 runner    (1001) docker     (127)     9404 2024-05-15 09:25:06.000000 glances-4.0.4/docs/_static/mem-wide.png
--rw-r--r--   0 runner    (1001) docker     (127)     5994 2024-05-15 09:25:06.000000 glances-4.0.4/docs/_static/mem.png
--rw-r--r--   0 runner    (1001) docker     (127)    12190 2024-05-15 09:25:06.000000 glances-4.0.4/docs/_static/monitored.png
--rw-r--r--   0 runner    (1001) docker     (127)    10211 2024-05-15 09:25:06.000000 glances-4.0.4/docs/_static/network.png
--rw-r--r--   0 runner    (1001) docker     (127)    21132 2024-05-15 09:25:06.000000 glances-4.0.4/docs/_static/per-cpu.png
--rw-r--r--   0 runner    (1001) docker     (127)     3809 2024-05-15 09:25:06.000000 glances-4.0.4/docs/_static/pergpu.png
--rw-r--r--   0 runner    (1001) docker     (127)    11041 2024-05-15 09:25:06.000000 glances-4.0.4/docs/_static/ports.png
--rw-r--r--   0 runner    (1001) docker     (127)    63154 2024-05-15 09:25:06.000000 glances-4.0.4/docs/_static/processlist-extended.png
--rw-r--r--   0 runner    (1001) docker     (127)   160408 2024-05-15 09:25:06.000000 glances-4.0.4/docs/_static/processlist-filter.png
--rw-r--r--   0 runner    (1001) docker     (127)    53684 2024-05-15 09:25:06.000000 glances-4.0.4/docs/_static/processlist-top.png
--rw-r--r--   0 runner    (1001) docker     (127)   227401 2024-05-15 09:25:06.000000 glances-4.0.4/docs/_static/processlist-wide.png
--rw-r--r--   0 runner    (1001) docker     (127)   151590 2024-05-15 09:25:06.000000 glances-4.0.4/docs/_static/processlist.png
--rw-r--r--   0 runner    (1001) docker     (127)    25081 2024-05-15 09:25:06.000000 glances-4.0.4/docs/_static/prometheus_exporter.png
--rw-r--r--   0 runner    (1001) docker     (127)    91914 2024-05-15 09:25:06.000000 glances-4.0.4/docs/_static/prometheus_server.png
--rw-r--r--   0 runner    (1001) docker     (127)    27582 2024-05-15 09:25:06.000000 glances-4.0.4/docs/_static/quicklook-percpu.png
--rw-r--r--   0 runner    (1001) docker     (127)    17789 2024-05-15 09:25:06.000000 glances-4.0.4/docs/_static/quicklook.png
--rw-r--r--   0 runner    (1001) docker     (127)     5585 2024-05-15 09:25:06.000000 glances-4.0.4/docs/_static/raid.png
--rw-r--r--   0 runner    (1001) docker     (127)     6362 2024-05-15 09:25:06.000000 glances-4.0.4/docs/_static/reddit.png
--rw-r--r--   0 runner    (1001) docker     (127)  1089975 2024-05-15 09:25:06.000000 glances-4.0.4/docs/_static/screencast.gif
--rw-r--r--   0 runner    (1001) docker     (127)   265567 2024-05-15 09:25:06.000000 glances-4.0.4/docs/_static/screenshot-web.png
--rw-r--r--   0 runner    (1001) docker     (127)    36097 2024-05-15 09:25:06.000000 glances-4.0.4/docs/_static/screenshot-web2.png
--rw-r--r--   0 runner    (1001) docker     (127)  1098062 2024-05-15 09:25:06.000000 glances-4.0.4/docs/_static/screenshot-wide.png
--rw-r--r--   0 runner    (1001) docker     (127)   508044 2024-05-15 09:25:06.000000 glances-4.0.4/docs/_static/screenshot.png
--rw-r--r--   0 runner    (1001) docker     (127)    16125 2024-05-15 09:25:06.000000 glances-4.0.4/docs/_static/sensors.png
--rw-r--r--   0 runner    (1001) docker     (127)    21500 2024-05-15 09:25:06.000000 glances-4.0.4/docs/_static/smart.png
--rw-r--r--   0 runner    (1001) docker     (127)    41952 2024-05-15 09:25:06.000000 glances-4.0.4/docs/_static/sparkline.png
--rw-r--r--   0 runner    (1001) docker     (127)    23021 2024-05-15 09:25:06.000000 glances-4.0.4/docs/_static/trend.png
--rw-r--r--   0 runner    (1001) docker     (127)     6395 2024-05-15 09:25:06.000000 glances-4.0.4/docs/_static/twitter-icon.png
--rw-r--r--   0 runner    (1001) docker     (127)     4741 2024-05-15 09:25:06.000000 glances-4.0.4/docs/_static/wifi.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 09:25:11.808857 glances-4.0.4/docs/_templates/
--rw-r--r--   0 runner    (1001) docker     (127)      357 2024-05-15 09:25:06.000000 glances-4.0.4/docs/_templates/links.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 09:25:11.812857 glances-4.0.4/docs/aoa/
--rw-r--r--   0 runner    (1001) docker     (127)     2457 2024-05-15 09:25:06.000000 glances-4.0.4/docs/aoa/actions.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3690 2024-05-15 09:25:06.000000 glances-4.0.4/docs/aoa/amps.rst
--rw-r--r--   0 runner    (1001) docker     (127)      407 2024-05-15 09:25:06.000000 glances-4.0.4/docs/aoa/cloud.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1059 2024-05-15 09:25:06.000000 glances-4.0.4/docs/aoa/connections.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2179 2024-05-15 09:25:06.000000 glances-4.0.4/docs/aoa/containers.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3406 2024-05-15 09:25:06.000000 glances-4.0.4/docs/aoa/cpu.rst
--rw-r--r--   0 runner    (1001) docker     (127)      975 2024-05-15 09:25:06.000000 glances-4.0.4/docs/aoa/diskio.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1034 2024-05-15 09:25:06.000000 glances-4.0.4/docs/aoa/events.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1144 2024-05-15 09:25:06.000000 glances-4.0.4/docs/aoa/folders.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1584 2024-05-15 09:25:06.000000 glances-4.0.4/docs/aoa/fs.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1288 2024-05-15 09:25:06.000000 glances-4.0.4/docs/aoa/gpu.rst
--rw-r--r--   0 runner    (1001) docker     (127)      925 2024-05-15 09:25:06.000000 glances-4.0.4/docs/aoa/hddtemp.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2828 2024-05-15 09:25:06.000000 glances-4.0.4/docs/aoa/header.rst
--rw-r--r--   0 runner    (1001) docker     (127)      629 2024-05-15 09:25:06.000000 glances-4.0.4/docs/aoa/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      556 2024-05-15 09:25:06.000000 glances-4.0.4/docs/aoa/irq.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2227 2024-05-15 09:25:06.000000 glances-4.0.4/docs/aoa/load.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2526 2024-05-15 09:25:06.000000 glances-4.0.4/docs/aoa/memory.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1963 2024-05-15 09:25:06.000000 glances-4.0.4/docs/aoa/network.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1991 2024-05-15 09:25:06.000000 glances-4.0.4/docs/aoa/ports.rst
--rw-r--r--   0 runner    (1001) docker     (127)     9688 2024-05-15 09:25:06.000000 glances-4.0.4/docs/aoa/ps.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1266 2024-05-15 09:25:06.000000 glances-4.0.4/docs/aoa/quicklook.rst
--rw-r--r--   0 runner    (1001) docker     (127)      344 2024-05-15 09:25:06.000000 glances-4.0.4/docs/aoa/raid.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1349 2024-05-15 09:25:06.000000 glances-4.0.4/docs/aoa/sensors.rst
--rw-r--r--   0 runner    (1001) docker     (127)      572 2024-05-15 09:25:06.000000 glances-4.0.4/docs/aoa/smart.rst
--rw-r--r--   0 runner    (1001) docker     (127)      623 2024-05-15 09:25:06.000000 glances-4.0.4/docs/aoa/wifi.rst
--rw-r--r--   0 runner    (1001) docker     (127)    50249 2024-05-15 09:25:06.000000 glances-4.0.4/docs/api.rst
--rwxr-xr-x   0 runner    (1001) docker     (127)       28 2024-05-15 09:25:06.000000 glances-4.0.4/docs/build.sh
--rw-r--r--   0 runner    (1001) docker     (127)     7977 2024-05-15 09:25:06.000000 glances-4.0.4/docs/cmds.rst
--rw-r--r--   0 runner    (1001) docker     (127)     9804 2024-05-15 09:25:06.000000 glances-4.0.4/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)     6715 2024-05-15 09:25:06.000000 glances-4.0.4/docs/config.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 09:25:11.812857 glances-4.0.4/docs/dev/
--rw-r--r--   0 runner    (1001) docker     (127)      457 2024-05-15 09:25:06.000000 glances-4.0.4/docs/dev/README.txt
--rw-r--r--   0 runner    (1001) docker     (127)   328258 2024-05-15 09:25:07.000000 glances-4.0.4/docs/dev/glances-cprofile.png
--rw-r--r--   0 runner    (1001) docker     (127)     8376 2024-05-15 09:25:07.000000 glances-4.0.4/docs/docker.rst
--rw-r--r--   0 runner    (1001) docker     (127)      137 2024-05-15 09:25:07.000000 glances-4.0.4/docs/faq.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1755 2024-05-15 09:25:07.000000 glances-4.0.4/docs/glances.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 09:25:11.816857 glances-4.0.4/docs/gw/
--rw-r--r--   0 runner    (1001) docker     (127)      756 2024-05-15 09:25:07.000000 glances-4.0.4/docs/gw/cassandra.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1094 2024-05-15 09:25:07.000000 glances-4.0.4/docs/gw/couchdb.rst
--rw-r--r--   0 runner    (1001) docker     (127)      843 2024-05-15 09:25:07.000000 glances-4.0.4/docs/gw/csv.rst
--rw-r--r--   0 runner    (1001) docker     (127)      500 2024-05-15 09:25:07.000000 glances-4.0.4/docs/gw/elastic.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1141 2024-05-15 09:25:07.000000 glances-4.0.4/docs/gw/graph.rst
--rw-r--r--   0 runner    (1001) docker     (127)      836 2024-05-15 09:25:07.000000 glances-4.0.4/docs/gw/graphite.rst
--rw-r--r--   0 runner    (1001) docker     (127)      401 2024-05-15 09:25:07.000000 glances-4.0.4/docs/gw/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     4597 2024-05-15 09:25:07.000000 glances-4.0.4/docs/gw/influxdb.rst
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-15 09:25:07.000000 glances-4.0.4/docs/gw/json.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1460 2024-05-15 09:25:07.000000 glances-4.0.4/docs/gw/kafka.rst
--rw-r--r--   0 runner    (1001) docker     (127)      851 2024-05-15 09:25:07.000000 glances-4.0.4/docs/gw/mongodb.rst
--rw-r--r--   0 runner    (1001) docker     (127)      700 2024-05-15 09:25:07.000000 glances-4.0.4/docs/gw/mqtt.rst
--rw-r--r--   0 runner    (1001) docker     (127)      386 2024-05-15 09:25:07.000000 glances-4.0.4/docs/gw/opentsdb.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1196 2024-05-15 09:25:07.000000 glances-4.0.4/docs/gw/prometheus.rst
--rw-r--r--   0 runner    (1001) docker     (127)      415 2024-05-15 09:25:07.000000 glances-4.0.4/docs/gw/rabbitmq.rst
--rw-r--r--   0 runner    (1001) docker     (127)      845 2024-05-15 09:25:07.000000 glances-4.0.4/docs/gw/restful.rst
--rw-r--r--   0 runner    (1001) docker     (127)      333 2024-05-15 09:25:07.000000 glances-4.0.4/docs/gw/riemann.rst
--rw-r--r--   0 runner    (1001) docker     (127)      580 2024-05-15 09:25:07.000000 glances-4.0.4/docs/gw/statsd.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1196 2024-05-15 09:25:07.000000 glances-4.0.4/docs/gw/zeromq.rst
--rw-r--r--   0 runner    (1001) docker     (127)      805 2024-05-15 09:25:07.000000 glances-4.0.4/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-05-15 09:25:07.000000 glances-4.0.4/docs/install.rst
--rw-r--r--   0 runner    (1001) docker     (127)     7251 2024-05-15 09:25:07.000000 glances-4.0.4/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 09:25:11.816857 glances-4.0.4/docs/man/
--rwxr-xr-x   0 runner    (1001) docker     (127)    19253 2024-05-15 09:25:07.000000 glances-4.0.4/docs/man/glances.1
--rw-r--r--   0 runner    (1001) docker     (127)     1909 2024-05-15 09:25:07.000000 glances-4.0.4/docs/objects.inv
--rw-r--r--   0 runner    (1001) docker     (127)     6081 2024-05-15 09:25:07.000000 glances-4.0.4/docs/quickstart.rst
--rw-r--r--   0 runner    (1001) docker     (127)      326 2024-05-15 09:25:07.000000 glances-4.0.4/docs/support.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 09:25:11.820857 glances-4.0.4/glances/
--rw-r--r--   0 runner    (1001) docker     (127)     5475 2024-05-15 09:25:07.000000 glances-4.0.4/glances/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      333 2024-05-15 09:25:07.000000 glances-4.0.4/glances/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3090 2024-05-15 09:25:07.000000 glances-4.0.4/glances/actions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 09:25:11.820857 glances-4.0.4/glances/amps/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 09:25:07.000000 glances-4.0.4/glances/amps/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6445 2024-05-15 09:25:07.000000 glances-4.0.4/glances/amps/amp.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 09:25:11.820857 glances-4.0.4/glances/amps/default/
--rw-r--r--   0 runner    (1001) docker     (127)     2262 2024-05-15 09:25:07.000000 glances-4.0.4/glances/amps/default/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 09:25:11.820857 glances-4.0.4/glances/amps/nginx/
--rw-r--r--   0 runner    (1001) docker     (127)     2599 2024-05-15 09:25:07.000000 glances-4.0.4/glances/amps/nginx/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 09:25:11.820857 glances-4.0.4/glances/amps/systemd/
--rw-r--r--   0 runner    (1001) docker     (127)     2575 2024-05-15 09:25:07.000000 glances-4.0.4/glances/amps/systemd/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 09:25:11.820857 glances-4.0.4/glances/amps/systemv/
--rw-r--r--   0 runner    (1001) docker     (127)     2401 2024-05-15 09:25:07.000000 glances-4.0.4/glances/amps/systemv/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5437 2024-05-15 09:25:07.000000 glances-4.0.4/glances/amps_list.py
--rw-r--r--   0 runner    (1001) docker     (127)     3399 2024-05-15 09:25:07.000000 glances-4.0.4/glances/attribute.py
--rw-r--r--   0 runner    (1001) docker     (127)     9593 2024-05-15 09:25:07.000000 glances-4.0.4/glances/autodiscover.py
--rw-r--r--   0 runner    (1001) docker     (127)     8973 2024-05-15 09:25:07.000000 glances-4.0.4/glances/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    10101 2024-05-15 09:25:07.000000 glances-4.0.4/glances/client_browser.py
--rw-r--r--   0 runner    (1001) docker     (127)    12385 2024-05-15 09:25:07.000000 glances-4.0.4/glances/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     5012 2024-05-15 09:25:07.000000 glances-4.0.4/glances/cpu_percent.py
--rw-r--r--   0 runner    (1001) docker     (127)     2263 2024-05-15 09:25:07.000000 glances-4.0.4/glances/event.py
--rw-r--r--   0 runner    (1001) docker     (127)    15798 2024-05-15 09:25:07.000000 glances-4.0.4/glances/events_list.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 09:25:11.820857 glances-4.0.4/glances/exports/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 09:25:07.000000 glances-4.0.4/glances/exports/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7751 2024-05-15 09:25:07.000000 glances-4.0.4/glances/exports/export.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 09:25:11.824857 glances-4.0.4/glances/exports/glances_cassandra/
--rw-r--r--   0 runner    (1001) docker     (127)     4428 2024-05-15 09:25:07.000000 glances-4.0.4/glances/exports/glances_cassandra/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 09:25:11.824857 glances-4.0.4/glances/exports/glances_couchdb/
--rw-r--r--   0 runner    (1001) docker     (127)     2714 2024-05-15 09:25:07.000000 glances-4.0.4/glances/exports/glances_couchdb/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 09:25:11.824857 glances-4.0.4/glances/exports/glances_csv/
--rw-r--r--   0 runner    (1001) docker     (127)     4047 2024-05-15 09:25:07.000000 glances-4.0.4/glances/exports/glances_csv/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 09:25:11.824857 glances-4.0.4/glances/exports/glances_elasticsearch/
--rw-r--r--   0 runner    (1001) docker     (127)     2927 2024-05-15 09:25:07.000000 glances-4.0.4/glances/exports/glances_elasticsearch/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 09:25:11.824857 glances-4.0.4/glances/exports/glances_graph/
--rw-r--r--   0 runner    (1001) docker     (127)     4410 2024-05-15 09:25:07.000000 glances-4.0.4/glances/exports/glances_graph/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 09:25:11.824857 glances-4.0.4/glances/exports/glances_graphite/
--rw-r--r--   0 runner    (1001) docker     (127)     3288 2024-05-15 09:25:07.000000 glances-4.0.4/glances/exports/glances_graphite/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 09:25:11.824857 glances-4.0.4/glances/exports/glances_influxdb/
--rw-r--r--   0 runner    (1001) docker     (127)     5991 2024-05-15 09:25:07.000000 glances-4.0.4/glances/exports/glances_influxdb/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 09:25:11.824857 glances-4.0.4/glances/exports/glances_influxdb2/
--rw-r--r--   0 runner    (1001) docker     (127)     6694 2024-05-15 09:25:07.000000 glances-4.0.4/glances/exports/glances_influxdb2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 09:25:11.824857 glances-4.0.4/glances/exports/glances_json/
--rw-r--r--   0 runner    (1001) docker     (127)     1847 2024-05-15 09:25:07.000000 glances-4.0.4/glances/exports/glances_json/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 09:25:11.824857 glances-4.0.4/glances/exports/glances_kafka/
--rw-r--r--   0 runner    (1001) docker     (127)     2848 2024-05-15 09:25:07.000000 glances-4.0.4/glances/exports/glances_kafka/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 09:25:11.824857 glances-4.0.4/glances/exports/glances_mongodb/
--rw-r--r--   0 runner    (1001) docker     (127)     2276 2024-05-15 09:25:07.000000 glances-4.0.4/glances/exports/glances_mongodb/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 09:25:11.824857 glances-4.0.4/glances/exports/glances_mqtt/
--rwxr-xr-x   0 runner    (1001) docker     (127)     5011 2024-05-15 09:25:07.000000 glances-4.0.4/glances/exports/glances_mqtt/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 09:25:11.824857 glances-4.0.4/glances/exports/glances_opentsdb/
--rw-r--r--   0 runner    (1001) docker     (127)     2475 2024-05-15 09:25:07.000000 glances-4.0.4/glances/exports/glances_opentsdb/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 09:25:11.824857 glances-4.0.4/glances/exports/glances_prometheus/
--rw-r--r--   0 runner    (1001) docker     (127)     3196 2024-05-15 09:25:07.000000 glances-4.0.4/glances/exports/glances_prometheus/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 09:25:11.824857 glances-4.0.4/glances/exports/glances_rabbitmq/
--rw-r--r--   0 runner    (1001) docker     (127)     2846 2024-05-15 09:25:07.000000 glances-4.0.4/glances/exports/glances_rabbitmq/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 09:25:11.824857 glances-4.0.4/glances/exports/glances_restful/
--rw-r--r--   0 runner    (1001) docker     (127)     2158 2024-05-15 09:25:07.000000 glances-4.0.4/glances/exports/glances_restful/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 09:25:11.824857 glances-4.0.4/glances/exports/glances_riemann/
--rw-r--r--   0 runner    (1001) docker     (127)     2034 2024-05-15 09:25:07.000000 glances-4.0.4/glances/exports/glances_riemann/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 09:25:11.824857 glances-4.0.4/glances/exports/glances_statsd/
--rw-r--r--   0 runner    (1001) docker     (127)     2263 2024-05-15 09:25:07.000000 glances-4.0.4/glances/exports/glances_statsd/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 09:25:11.824857 glances-4.0.4/glances/exports/glances_zeromq/
--rw-r--r--   0 runner    (1001) docker     (127)     2911 2024-05-15 09:25:07.000000 glances-4.0.4/glances/exports/glances_zeromq/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5858 2024-05-15 09:25:07.000000 glances-4.0.4/glances/filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     5913 2024-05-15 09:25:07.000000 glances-4.0.4/glances/folder_list.py
--rw-r--r--   0 runner    (1001) docker     (127)    12259 2024-05-15 09:25:07.000000 glances-4.0.4/glances/globals.py
--rw-r--r--   0 runner    (1001) docker     (127)     1408 2024-05-15 09:25:07.000000 glances-4.0.4/glances/history.py
--rw-r--r--   0 runner    (1001) docker     (127)     3270 2024-05-15 09:25:07.000000 glances-4.0.4/glances/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)    30810 2024-05-15 09:25:07.000000 glances-4.0.4/glances/main.py
--rw-r--r--   0 runner    (1001) docker     (127)     6008 2024-05-15 09:25:07.000000 glances-4.0.4/glances/outdated.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 09:25:11.828857 glances-4.0.4/glances/outputs/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 09:25:07.000000 glances-4.0.4/glances/outputs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3735 2024-05-15 09:25:07.000000 glances-4.0.4/glances/outputs/glances_bars.py
--rw-r--r--   0 runner    (1001) docker     (127)    48721 2024-05-15 09:25:07.000000 glances-4.0.4/glances/outputs/glances_curses.py
--rw-r--r--   0 runner    (1001) docker     (127)    12659 2024-05-15 09:25:07.000000 glances-4.0.4/glances/outputs/glances_curses_browser.py
--rw-r--r--   0 runner    (1001) docker     (127)    29836 2024-05-15 09:25:07.000000 glances-4.0.4/glances/outputs/glances_restful_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     2768 2024-05-15 09:25:07.000000 glances-4.0.4/glances/outputs/glances_sparklines.py
--rw-r--r--   0 runner    (1001) docker     (127)     3034 2024-05-15 09:25:07.000000 glances-4.0.4/glances/outputs/glances_stdout.py
--rw-r--r--   0 runner    (1001) docker     (127)    11649 2024-05-15 09:25:07.000000 glances-4.0.4/glances/outputs/glances_stdout_apidoc.py
--rw-r--r--   0 runner    (1001) docker     (127)     3619 2024-05-15 09:25:07.000000 glances-4.0.4/glances/outputs/glances_stdout_csv.py
--rw-r--r--   0 runner    (1001) docker     (127)     4451 2024-05-15 09:25:07.000000 glances-4.0.4/glances/outputs/glances_stdout_issue.py
--rw-r--r--   0 runner    (1001) docker     (127)     1435 2024-05-15 09:25:07.000000 glances-4.0.4/glances/outputs/glances_stdout_json.py
--rw-r--r--   0 runner    (1001) docker     (127)      799 2024-05-15 09:25:07.000000 glances-4.0.4/glances/outputs/glances_unicode.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 09:25:11.828857 glances-4.0.4/glances/outputs/static/
--rw-r--r--   0 runner    (1001) docker     (127)      245 2024-05-15 09:25:07.000000 glances-4.0.4/glances/outputs/static/.eslintrc.js
--rw-r--r--   0 runner    (1001) docker     (127)      182 2024-05-15 09:25:07.000000 glances-4.0.4/glances/outputs/static/.prettierrc.js
--rw-r--r--   0 runner    (1001) docker     (127)     1122 2024-05-15 09:25:07.000000 glances-4.0.4/glances/outputs/static/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 09:25:11.828857 glances-4.0.4/glances/outputs/static/css/
--rw-r--r--   0 runner    (1001) docker     (127)     1991 2024-05-15 09:25:07.000000 glances-4.0.4/glances/outputs/static/css/bootstrap.less
--rw-r--r--   0 runner    (1001) docker     (127)     5635 2024-05-15 09:25:07.000000 glances-4.0.4/glances/outputs/static/css/style.scss
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-15 09:25:07.000000 glances-4.0.4/glances/outputs/static/css/variables.less
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 09:25:11.828857 glances-4.0.4/glances/outputs/static/images/
--rw-r--r--   0 runner    (1001) docker     (127)     4286 2024-05-15 09:25:07.000000 glances-4.0.4/glances/outputs/static/images/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (127)    50295 2024-05-15 09:25:07.000000 glances-4.0.4/glances/outputs/static/images/glances.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 09:25:11.832857 glances-4.0.4/glances/outputs/static/js/
--rw-r--r--   0 runner    (1001) docker     (127)    15387 2024-05-15 09:25:07.000000 glances-4.0.4/glances/outputs/static/js/App.vue
--rw-r--r--   0 runner    (1001) docker     (127)      326 2024-05-15 09:25:07.000000 glances-4.0.4/glances/outputs/static/js/app.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 09:25:11.836857 glances-4.0.4/glances/outputs/static/js/components/
--rw-r--r--   0 runner    (1001) docker     (127)    11318 2024-05-15 09:25:07.000000 glances-4.0.4/glances/outputs/static/js/components/help.vue
--rw-r--r--   0 runner    (1001) docker     (127)     3485 2024-05-15 09:25:07.000000 glances-4.0.4/glances/outputs/static/js/components/plugin-alert.vue
--rw-r--r--   0 runner    (1001) docker     (127)     1656 2024-05-15 09:25:07.000000 glances-4.0.4/glances/outputs/static/js/components/plugin-amps.vue
--rw-r--r--   0 runner    (1001) docker     (127)      717 2024-05-15 09:25:07.000000 glances-4.0.4/glances/outputs/static/js/components/plugin-cloud.vue
--rw-r--r--   0 runner    (1001) docker     (127)     2382 2024-05-15 09:25:07.000000 glances-4.0.4/glances/outputs/static/js/components/plugin-connections.vue
--rw-r--r--   0 runner    (1001) docker     (127)     7663 2024-05-15 09:25:07.000000 glances-4.0.4/glances/outputs/static/js/components/plugin-containers.vue
--rw-r--r--   0 runner    (1001) docker     (127)     7350 2024-05-15 09:25:07.000000 glances-4.0.4/glances/outputs/static/js/components/plugin-cpu.vue
--rw-r--r--   0 runner    (1001) docker     (127)     2526 2024-05-15 09:25:07.000000 glances-4.0.4/glances/outputs/static/js/components/plugin-diskio.vue
--rw-r--r--   0 runner    (1001) docker     (127)     1985 2024-05-15 09:25:07.000000 glances-4.0.4/glances/outputs/static/js/components/plugin-folders.vue
--rw-r--r--   0 runner    (1001) docker     (127)     2577 2024-05-15 09:25:07.000000 glances-4.0.4/glances/outputs/static/js/components/plugin-fs.vue
--rw-r--r--   0 runner    (1001) docker     (127)     4633 2024-05-15 09:25:07.000000 glances-4.0.4/glances/outputs/static/js/components/plugin-gpu.vue
--rw-r--r--   0 runner    (1001) docker     (127)      979 2024-05-15 09:25:07.000000 glances-4.0.4/glances/outputs/static/js/components/plugin-ip.vue
--rw-r--r--   0 runner    (1001) docker     (127)     1048 2024-05-15 09:25:07.000000 glances-4.0.4/glances/outputs/static/js/components/plugin-irq.vue
--rw-r--r--   0 runner    (1001) docker     (127)     1864 2024-05-15 09:25:07.000000 glances-4.0.4/glances/outputs/static/js/components/plugin-load.vue
--rw-r--r--   0 runner    (1001) docker     (127)     1518 2024-05-15 09:25:07.000000 glances-4.0.4/glances/outputs/static/js/components/plugin-mem-more.vue
--rw-r--r--   0 runner    (1001) docker     (127)     1742 2024-05-15 09:25:07.000000 glances-4.0.4/glances/outputs/static/js/components/plugin-mem.vue
--rw-r--r--   0 runner    (1001) docker     (127)     1752 2024-05-15 09:25:07.000000 glances-4.0.4/glances/outputs/static/js/components/plugin-memswap.vue
--rw-r--r--   0 runner    (1001) docker     (127)     4138 2024-05-15 09:25:07.000000 glances-4.0.4/glances/outputs/static/js/components/plugin-network.vue
--rw-r--r--   0 runner    (1001) docker     (127)      525 2024-05-15 09:25:07.000000 glances-4.0.4/glances/outputs/static/js/components/plugin-now.vue
--rw-r--r--   0 runner    (1001) docker     (127)     2659 2024-05-15 09:25:07.000000 glances-4.0.4/glances/outputs/static/js/components/plugin-percpu.vue
--rw-r--r--   0 runner    (1001) docker     (127)     2192 2024-05-15 09:25:07.000000 glances-4.0.4/glances/outputs/static/js/components/plugin-ports.vue
--rw-r--r--   0 runner    (1001) docker     (127)     2869 2024-05-15 09:25:07.000000 glances-4.0.4/glances/outputs/static/js/components/plugin-process.vue
--rw-r--r--   0 runner    (1001) docker     (127)     1347 2024-05-15 09:25:07.000000 glances-4.0.4/glances/outputs/static/js/components/plugin-processcount.vue
--rw-r--r--   0 runner    (1001) docker     (127)     9459 2024-05-15 09:25:07.000000 glances-4.0.4/glances/outputs/static/js/components/plugin-processlist.vue
--rw-r--r--   0 runner    (1001) docker     (127)     5094 2024-05-15 09:25:07.000000 glances-4.0.4/glances/outputs/static/js/components/plugin-quicklook.vue
--rw-r--r--   0 runner    (1001) docker     (127)     3082 2024-05-15 09:25:07.000000 glances-4.0.4/glances/outputs/static/js/components/plugin-raid.vue
--rw-r--r--   0 runner    (1001) docker     (127)     2125 2024-05-15 09:25:07.000000 glances-4.0.4/glances/outputs/static/js/components/plugin-sensors.vue
--rw-r--r--   0 runner    (1001) docker     (127)     1738 2024-05-15 09:25:07.000000 glances-4.0.4/glances/outputs/static/js/components/plugin-smart.vue
--rw-r--r--   0 runner    (1001) docker     (127)      810 2024-05-15 09:25:07.000000 glances-4.0.4/glances/outputs/static/js/components/plugin-system.vue
--rw-r--r--   0 runner    (1001) docker     (127)      326 2024-05-15 09:25:07.000000 glances-4.0.4/glances/outputs/static/js/components/plugin-uptime.vue
--rw-r--r--   0 runner    (1001) docker     (127)     1776 2024-05-15 09:25:07.000000 glances-4.0.4/glances/outputs/static/js/components/plugin-wifi.vue
--rw-r--r--   0 runner    (1001) docker     (127)     3362 2024-05-15 09:25:07.000000 glances-4.0.4/glances/outputs/static/js/filters.js
--rw-r--r--   0 runner    (1001) docker     (127)     4000 2024-05-15 09:25:07.000000 glances-4.0.4/glances/outputs/static/js/services.js
--rw-r--r--   0 runner    (1001) docker     (127)      153 2024-05-15 09:25:07.000000 glances-4.0.4/glances/outputs/static/js/store.js
--rw-r--r--   0 runner    (1001) docker     (127)      235 2024-05-15 09:25:07.000000 glances-4.0.4/glances/outputs/static/js/uiconfig.json
--rw-r--r--   0 runner    (1001) docker     (127)   452411 2024-05-15 09:25:07.000000 glances-4.0.4/glances/outputs/static/package-lock.json
--rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-05-15 09:25:07.000000 glances-4.0.4/glances/outputs/static/package.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 09:25:11.836857 glances-4.0.4/glances/outputs/static/public/
--rw-r--r--   0 runner    (1001) docker     (127)    50295 2024-05-15 09:25:07.000000 glances-4.0.4/glances/outputs/static/public/1272f6e9e8f9d6bfd6de.png
--rw-r--r--   0 runner    (1001) docker     (127)     4286 2024-05-15 09:25:07.000000 glances-4.0.4/glances/outputs/static/public/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (127)   448748 2024-05-15 09:25:07.000000 glances-4.0.4/glances/outputs/static/public/glances.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 09:25:11.840857 glances-4.0.4/glances/outputs/static/templates/
--rw-r--r--   0 runner    (1001) docker     (127)      477 2024-05-15 09:25:07.000000 glances-4.0.4/glances/outputs/static/templates/index.html
--rw-r--r--   0 runner    (1001) docker     (127)     2651 2024-05-15 09:25:07.000000 glances-4.0.4/glances/outputs/static/webpack.config.js
--rw-r--r--   0 runner    (1001) docker     (127)     4862 2024-05-15 09:25:07.000000 glances-4.0.4/glances/password.py
--rw-r--r--   0 runner    (1001) docker     (127)     2205 2024-05-15 09:25:07.000000 glances-4.0.4/glances/password_list.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 09:25:11.840857 glances-4.0.4/glances/plugins/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 09:25:07.000000 glances-4.0.4/glances/plugins/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 09:25:11.840857 glances-4.0.4/glances/plugins/__pycache__/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 09:25:07.000000 glances-4.0.4/glances/plugins/__pycache__/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 09:25:11.840857 glances-4.0.4/glances/plugins/alert/
--rw-r--r--   0 runner    (1001) docker     (127)     6273 2024-05-15 09:25:07.000000 glances-4.0.4/glances/plugins/alert/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 09:25:11.840857 glances-4.0.4/glances/plugins/amps/
--rw-r--r--   0 runner    (1001) docker     (127)     5074 2024-05-15 09:25:07.000000 glances-4.0.4/glances/plugins/amps/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 09:25:11.840857 glances-4.0.4/glances/plugins/cloud/
--rw-r--r--   0 runner    (1001) docker     (127)     6779 2024-05-15 09:25:07.000000 glances-4.0.4/glances/plugins/cloud/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 09:25:11.840857 glances-4.0.4/glances/plugins/connections/
--rw-r--r--   0 runner    (1001) docker     (127)     8252 2024-05-15 09:25:07.000000 glances-4.0.4/glances/plugins/connections/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 09:25:11.840857 glances-4.0.4/glances/plugins/containers/
--rw-r--r--   0 runner    (1001) docker     (127)    18361 2024-05-15 09:25:07.000000 glances-4.0.4/glances/plugins/containers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 09:25:11.840857 glances-4.0.4/glances/plugins/containers/engines/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 09:25:07.000000 glances-4.0.4/glances/plugins/containers/engines/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13975 2024-05-15 09:25:07.000000 glances-4.0.4/glances/plugins/containers/engines/docker.py
--rw-r--r--   0 runner    (1001) docker     (127)    13308 2024-05-15 09:25:07.000000 glances-4.0.4/glances/plugins/containers/engines/podman.py
--rw-r--r--   0 runner    (1001) docker     (127)     2648 2024-05-15 09:25:07.000000 glances-4.0.4/glances/plugins/containers/stats_streamer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 09:25:11.840857 glances-4.0.4/glances/plugins/core/
--rw-r--r--   0 runner    (1001) docker     (127)     2361 2024-05-15 09:25:07.000000 glances-4.0.4/glances/plugins/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 09:25:11.840857 glances-4.0.4/glances/plugins/cpu/
--rw-r--r--   0 runner    (1001) docker     (127)    15556 2024-05-15 09:25:07.000000 glances-4.0.4/glances/plugins/cpu/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 09:25:11.840857 glances-4.0.4/glances/plugins/diskio/
--rw-r--r--   0 runner    (1001) docker     (127)     8212 2024-05-15 09:25:07.000000 glances-4.0.4/glances/plugins/diskio/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 09:25:11.840857 glances-4.0.4/glances/plugins/folders/
--rw-r--r--   0 runner    (1001) docker     (127)     5165 2024-05-15 09:25:07.000000 glances-4.0.4/glances/plugins/folders/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 09:25:11.840857 glances-4.0.4/glances/plugins/fs/
--rw-r--r--   0 runner    (1001) docker     (127)    11833 2024-05-15 09:25:07.000000 glances-4.0.4/glances/plugins/fs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 09:25:11.840857 glances-4.0.4/glances/plugins/gpu/
--rw-r--r--   0 runner    (1001) docker     (127)     9805 2024-05-15 09:25:07.000000 glances-4.0.4/glances/plugins/gpu/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 09:25:11.840857 glances-4.0.4/glances/plugins/gpu/cards/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 09:25:07.000000 glances-4.0.4/glances/plugins/gpu/cards/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5033 2024-05-15 09:25:07.000000 glances-4.0.4/glances/plugins/gpu/cards/amd.py
--rw-r--r--   0 runner    (1001) docker     (127)     3561 2024-05-15 09:25:07.000000 glances-4.0.4/glances/plugins/gpu/cards/nvidia.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 09:25:11.840857 glances-4.0.4/glances/plugins/help/
--rw-r--r--   0 runner    (1001) docker     (127)    10295 2024-05-15 09:25:07.000000 glances-4.0.4/glances/plugins/help/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 09:25:11.844857 glances-4.0.4/glances/plugins/ip/
--rw-r--r--   0 runner    (1001) docker     (127)     9149 2024-05-15 09:25:07.000000 glances-4.0.4/glances/plugins/ip/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 09:25:11.844857 glances-4.0.4/glances/plugins/irq/
--rw-r--r--   0 runner    (1001) docker     (127)     6913 2024-05-15 09:25:07.000000 glances-4.0.4/glances/plugins/irq/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 09:25:11.844857 glances-4.0.4/glances/plugins/load/
--rw-r--r--   0 runner    (1001) docker     (127)     6856 2024-05-15 09:25:07.000000 glances-4.0.4/glances/plugins/load/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 09:25:11.844857 glances-4.0.4/glances/plugins/mem/
--rw-r--r--   0 runner    (1001) docker     (127)    10971 2024-05-15 09:25:07.000000 glances-4.0.4/glances/plugins/mem/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 09:25:11.844857 glances-4.0.4/glances/plugins/memswap/
--rw-r--r--   0 runner    (1001) docker     (127)     7512 2024-05-15 09:25:07.000000 glances-4.0.4/glances/plugins/memswap/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 09:25:11.844857 glances-4.0.4/glances/plugins/network/
--rw-r--r--   0 runner    (1001) docker     (127)    11852 2024-05-15 09:25:07.000000 glances-4.0.4/glances/plugins/network/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 09:25:11.844857 glances-4.0.4/glances/plugins/now/
--rw-r--r--   0 runner    (1001) docker     (127)     2623 2024-05-15 09:25:07.000000 glances-4.0.4/glances/plugins/now/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 09:25:11.844857 glances-4.0.4/glances/plugins/percpu/
--rw-r--r--   0 runner    (1001) docker     (127)     7548 2024-05-15 09:25:07.000000 glances-4.0.4/glances/plugins/percpu/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 09:25:11.844857 glances-4.0.4/glances/plugins/plugin/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 09:25:07.000000 glances-4.0.4/glances/plugins/plugin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    47262 2024-05-15 09:25:07.000000 glances-4.0.4/glances/plugins/plugin/model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 09:25:11.844857 glances-4.0.4/glances/plugins/ports/
--rw-r--r--   0 runner    (1001) docker     (127)    12956 2024-05-15 09:25:07.000000 glances-4.0.4/glances/plugins/ports/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 09:25:11.844857 glances-4.0.4/glances/plugins/processcount/
--rw-r--r--   0 runner    (1001) docker     (127)     5561 2024-05-15 09:25:07.000000 glances-4.0.4/glances/plugins/processcount/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 09:25:11.844857 glances-4.0.4/glances/plugins/processlist/
--rw-r--r--   0 runner    (1001) docker     (127)    36694 2024-05-15 09:25:07.000000 glances-4.0.4/glances/plugins/processlist/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 09:25:11.844857 glances-4.0.4/glances/plugins/psutilversion/
--rw-r--r--   0 runner    (1001) docker     (127)     1230 2024-05-15 09:25:07.000000 glances-4.0.4/glances/plugins/psutilversion/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 09:25:11.844857 glances-4.0.4/glances/plugins/quicklook/
--rw-r--r--   0 runner    (1001) docker     (127)    11876 2024-05-15 09:25:07.000000 glances-4.0.4/glances/plugins/quicklook/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 09:25:11.844857 glances-4.0.4/glances/plugins/raid/
--rw-r--r--   0 runner    (1001) docker     (127)     6537 2024-05-15 09:25:07.000000 glances-4.0.4/glances/plugins/raid/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 09:25:11.844857 glances-4.0.4/glances/plugins/sensors/
--rw-r--r--   0 runner    (1001) docker     (127)    14710 2024-05-15 09:25:07.000000 glances-4.0.4/glances/plugins/sensors/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 09:25:11.844857 glances-4.0.4/glances/plugins/sensors/sensor/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 09:25:07.000000 glances-4.0.4/glances/plugins/sensors/sensor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4403 2024-05-15 09:25:07.000000 glances-4.0.4/glances/plugins/sensors/sensor/glances_batpercent.py
--rw-r--r--   0 runner    (1001) docker     (127)     4932 2024-05-15 09:25:07.000000 glances-4.0.4/glances/plugins/sensors/sensor/glances_hddtemp.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 09:25:11.844857 glances-4.0.4/glances/plugins/smart/
--rw-r--r--   0 runner    (1001) docker     (127)     6411 2024-05-15 09:25:07.000000 glances-4.0.4/glances/plugins/smart/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 09:25:11.844857 glances-4.0.4/glances/plugins/system/
--rw-r--r--   0 runner    (1001) docker     (127)     8261 2024-05-15 09:25:07.000000 glances-4.0.4/glances/plugins/system/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 09:25:11.848857 glances-4.0.4/glances/plugins/uptime/
--rw-r--r--   0 runner    (1001) docker     (127)     2535 2024-05-15 09:25:07.000000 glances-4.0.4/glances/plugins/uptime/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 09:25:11.848857 glances-4.0.4/glances/plugins/version/
--rw-r--r--   0 runner    (1001) docker     (127)     1214 2024-05-15 09:25:07.000000 glances-4.0.4/glances/plugins/version/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 09:25:11.848857 glances-4.0.4/glances/plugins/wifi/
--rw-r--r--   0 runner    (1001) docker     (127)     6943 2024-05-15 09:25:07.000000 glances-4.0.4/glances/plugins/wifi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4862 2024-05-15 09:25:07.000000 glances-4.0.4/glances/ports_list.py
--rw-r--r--   0 runner    (1001) docker     (127)    26474 2024-05-15 09:25:07.000000 glances-4.0.4/glances/processes.py
--rw-r--r--   0 runner    (1001) docker     (127)     2668 2024-05-15 09:25:07.000000 glances-4.0.4/glances/programs.py
--rw-r--r--   0 runner    (1001) docker     (127)     2277 2024-05-15 09:25:07.000000 glances-4.0.4/glances/secure.py
--rw-r--r--   0 runner    (1001) docker     (127)     8281 2024-05-15 09:25:07.000000 glances-4.0.4/glances/server.py
--rw-r--r--   0 runner    (1001) docker     (127)     3937 2024-05-15 09:25:07.000000 glances-4.0.4/glances/snmp.py
--rw-r--r--   0 runner    (1001) docker     (127)     8000 2024-05-15 09:25:07.000000 glances-4.0.4/glances/standalone.py
--rw-r--r--   0 runner    (1001) docker     (127)     3210 2024-05-15 09:25:07.000000 glances-4.0.4/glances/static_list.py
--rw-r--r--   0 runner    (1001) docker     (127)    15179 2024-05-15 09:25:07.000000 glances-4.0.4/glances/stats.py
--rw-r--r--   0 runner    (1001) docker     (127)     2047 2024-05-15 09:25:07.000000 glances-4.0.4/glances/stats_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     3592 2024-05-15 09:25:07.000000 glances-4.0.4/glances/stats_client_snmp.py
--rw-r--r--   0 runner    (1001) docker     (127)     1693 2024-05-15 09:25:07.000000 glances-4.0.4/glances/stats_server.py
--rw-r--r--   0 runner    (1001) docker     (127)     2644 2024-05-15 09:25:07.000000 glances-4.0.4/glances/thresholds.py
--rw-r--r--   0 runner    (1001) docker     (127)     1589 2024-05-15 09:25:07.000000 glances-4.0.4/glances/timer.py
--rw-r--r--   0 runner    (1001) docker     (127)     4406 2024-05-15 09:25:07.000000 glances-4.0.4/glances/web_list.py
--rw-r--r--   0 runner    (1001) docker     (127)     1183 2024-05-15 09:25:07.000000 glances-4.0.4/glances/webserver.py
--rw-r--r--   0 runner    (1001) docker     (127)     1240 2024-05-15 09:25:07.000000 glances-4.0.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-15 09:25:11.852857 glances-4.0.4/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)     4418 2024-05-15 09:25:07.000000 glances-4.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 09:31:20.349850 glances-4.0.5/
+-rw-r--r--   0 runner    (1001) docker     (127)     1958 2024-05-18 09:31:15.000000 glances-4.0.5/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (127)     6148 2024-05-18 09:31:15.000000 glances-4.0.5/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)    42098 2024-05-18 09:31:15.000000 glances-4.0.5/COPYING
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 09:31:20.341850 glances-4.0.5/Glances.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    20468 2024-05-18 09:31:20.000000 glances-4.0.5/Glances.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    10026 2024-05-18 09:31:20.000000 glances-4.0.5/Glances.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-18 09:31:20.000000 glances-4.0.5/Glances.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-18 09:31:20.000000 glances-4.0.5/Glances.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      719 2024-05-18 09:31:20.000000 glances-4.0.5/Glances.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-18 09:31:20.000000 glances-4.0.5/Glances.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      262 2024-05-18 09:31:15.000000 glances-4.0.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    73130 2024-05-18 09:31:15.000000 glances-4.0.5/NEWS.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    20468 2024-05-18 09:31:20.349850 glances-4.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    16655 2024-05-18 09:31:15.000000 glances-4.0.5/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1515 2024-05-18 09:31:15.000000 glances-4.0.5/SECURITY.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 09:31:20.289849 glances-4.0.5/conf/
+-rw-r--r--   0 runner    (1001) docker     (127)    23757 2024-05-18 09:31:15.000000 glances-4.0.5/conf/glances.conf
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 09:31:20.293849 glances-4.0.5/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     7769 2024-05-18 09:31:15.000000 glances-4.0.5/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)      281 2024-05-18 09:31:15.000000 glances-4.0.5/docs/README.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 09:31:20.309849 glances-4.0.5/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)     5175 2024-05-18 09:31:15.000000 glances-4.0.5/docs/_static/Glances Logo dark.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     5185 2024-05-18 09:31:15.000000 glances-4.0.5/docs/_static/Glances Logo.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    10756 2024-05-18 09:31:15.000000 glances-4.0.5/docs/_static/Glances Text Logo dark.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    10775 2024-05-18 09:31:15.000000 glances-4.0.5/docs/_static/Glances Text Logo.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    29273 2024-05-18 09:31:15.000000 glances-4.0.5/docs/_static/amp-dropbox.png
+-rw-r--r--   0 runner    (1001) docker     (127)     9474 2024-05-18 09:31:15.000000 glances-4.0.5/docs/_static/amp-python-warning.png
+-rw-r--r--   0 runner    (1001) docker     (127)     9362 2024-05-18 09:31:15.000000 glances-4.0.5/docs/_static/amp-python.png
+-rw-r--r--   0 runner    (1001) docker     (127)    80498 2024-05-18 09:31:15.000000 glances-4.0.5/docs/_static/amps.png
+-rw-r--r--   0 runner    (1001) docker     (127)    13916 2024-05-18 09:31:15.000000 glances-4.0.5/docs/_static/aws.png
+-rw-r--r--   0 runner    (1001) docker     (127)    44160 2024-05-18 09:31:15.000000 glances-4.0.5/docs/_static/browser.png
+-rw-r--r--   0 runner    (1001) docker     (127)    21111 2024-05-18 09:31:15.000000 glances-4.0.5/docs/_static/cloud.png
+-rw-r--r--   0 runner    (1001) docker     (127)     9442 2024-05-18 09:31:15.000000 glances-4.0.5/docs/_static/connected.png
+-rw-r--r--   0 runner    (1001) docker     (127)    29245 2024-05-18 09:31:15.000000 glances-4.0.5/docs/_static/connections.png
+-rw-r--r--   0 runner    (1001) docker     (127)    34093 2024-05-18 09:31:15.000000 glances-4.0.5/docs/_static/containers.png
+-rw-r--r--   0 runner    (1001) docker     (127)    11799 2024-05-18 09:31:15.000000 glances-4.0.5/docs/_static/cpu-wide.png
+-rw-r--r--   0 runner    (1001) docker     (127)     4504 2024-05-18 09:31:15.000000 glances-4.0.5/docs/_static/cpu.png
+-rw-r--r--   0 runner    (1001) docker     (127)    10031 2024-05-18 09:31:15.000000 glances-4.0.5/docs/_static/disconnected.png
+-rw-r--r--   0 runner    (1001) docker     (127)     9638 2024-05-18 09:31:15.000000 glances-4.0.5/docs/_static/diskio.png
+-rw-r--r--   0 runner    (1001) docker     (127)    24808 2024-05-18 09:31:15.000000 glances-4.0.5/docs/_static/events.png
+-rw-r--r--   0 runner    (1001) docker     (127)    13715 2024-05-18 09:31:15.000000 glances-4.0.5/docs/_static/folders.png
+-rw-r--r--   0 runner    (1001) docker     (127)    10950 2024-05-18 09:31:15.000000 glances-4.0.5/docs/_static/fs.png
+-rw-r--r--   0 runner    (1001) docker     (127)    56273 2024-05-18 09:31:15.000000 glances-4.0.5/docs/_static/glances-architecture.excalidraw
+-rw-r--r--   0 runner    (1001) docker     (127)   123499 2024-05-18 09:31:15.000000 glances-4.0.5/docs/_static/glances-architecture.png
+-rw-r--r--   0 runner    (1001) docker     (127)    92793 2024-05-18 09:31:15.000000 glances-4.0.5/docs/_static/glances-cgraph.svg
+-rw-r--r--   0 runner    (1001) docker     (127)   114983 2024-05-18 09:31:15.000000 glances-4.0.5/docs/_static/glances-flame.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     9404 2024-05-18 09:31:15.000000 glances-4.0.5/docs/_static/glances-influxdb.png
+-rw-r--r--   0 runner    (1001) docker     (127)    33567 2024-05-18 09:31:15.000000 glances-4.0.5/docs/_static/glances-memory-profiling-with-history.png
+-rw-r--r--   0 runner    (1001) docker     (127)    31797 2024-05-18 09:31:15.000000 glances-4.0.5/docs/_static/glances-memory-profiling-without-history.png
+-rw-r--r--   0 runner    (1001) docker     (127)    29500 2024-05-18 09:31:15.000000 glances-4.0.5/docs/_static/glances-pyinstrument.html
+-rw-r--r--   0 runner    (1001) docker     (127)   295283 2024-05-18 09:31:15.000000 glances-4.0.5/docs/_static/glances-responsive-webdesign.png
+-rw-r--r--   0 runner    (1001) docker     (127)   435038 2024-05-18 09:31:15.000000 glances-4.0.5/docs/_static/glances-summary.png
+-rw-r--r--   0 runner    (1001) docker     (127)     3865 2024-05-18 09:31:15.000000 glances-4.0.5/docs/_static/gpu.png
+-rw-r--r--   0 runner    (1001) docker     (127)   141657 2024-05-18 09:31:15.000000 glances-4.0.5/docs/_static/grafana.png
+-rw-r--r--   0 runner    (1001) docker     (127)   187140 2024-05-18 09:31:15.000000 glances-4.0.5/docs/_static/graph-load.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    14415 2024-05-18 09:31:15.000000 glances-4.0.5/docs/_static/hddtemp.png
+-rw-r--r--   0 runner    (1001) docker     (127)    19879 2024-05-18 09:31:15.000000 glances-4.0.5/docs/_static/header.png
+-rw-r--r--   0 runner    (1001) docker     (127)    12750 2024-05-18 09:31:15.000000 glances-4.0.5/docs/_static/ip.png
+-rw-r--r--   0 runner    (1001) docker     (127)     3980 2024-05-18 09:31:15.000000 glances-4.0.5/docs/_static/irq.png
+-rw-r--r--   0 runner    (1001) docker     (127)     6923 2024-05-18 09:31:15.000000 glances-4.0.5/docs/_static/load.png
+-rw-r--r--   0 runner    (1001) docker     (127)    20009 2024-05-18 09:31:15.000000 glances-4.0.5/docs/_static/loadpercent.png
+-rw-r--r--   0 runner    (1001) docker     (127)     9404 2024-05-18 09:31:15.000000 glances-4.0.5/docs/_static/mem-wide.png
+-rw-r--r--   0 runner    (1001) docker     (127)     5994 2024-05-18 09:31:15.000000 glances-4.0.5/docs/_static/mem.png
+-rw-r--r--   0 runner    (1001) docker     (127)    12190 2024-05-18 09:31:15.000000 glances-4.0.5/docs/_static/monitored.png
+-rw-r--r--   0 runner    (1001) docker     (127)    10211 2024-05-18 09:31:15.000000 glances-4.0.5/docs/_static/network.png
+-rw-r--r--   0 runner    (1001) docker     (127)    21132 2024-05-18 09:31:15.000000 glances-4.0.5/docs/_static/per-cpu.png
+-rw-r--r--   0 runner    (1001) docker     (127)     3809 2024-05-18 09:31:15.000000 glances-4.0.5/docs/_static/pergpu.png
+-rw-r--r--   0 runner    (1001) docker     (127)    11041 2024-05-18 09:31:15.000000 glances-4.0.5/docs/_static/ports.png
+-rw-r--r--   0 runner    (1001) docker     (127)    63154 2024-05-18 09:31:15.000000 glances-4.0.5/docs/_static/processlist-extended.png
+-rw-r--r--   0 runner    (1001) docker     (127)   160408 2024-05-18 09:31:15.000000 glances-4.0.5/docs/_static/processlist-filter.png
+-rw-r--r--   0 runner    (1001) docker     (127)    53684 2024-05-18 09:31:15.000000 glances-4.0.5/docs/_static/processlist-top.png
+-rw-r--r--   0 runner    (1001) docker     (127)   227401 2024-05-18 09:31:15.000000 glances-4.0.5/docs/_static/processlist-wide.png
+-rw-r--r--   0 runner    (1001) docker     (127)   151590 2024-05-18 09:31:15.000000 glances-4.0.5/docs/_static/processlist.png
+-rw-r--r--   0 runner    (1001) docker     (127)    25081 2024-05-18 09:31:15.000000 glances-4.0.5/docs/_static/prometheus_exporter.png
+-rw-r--r--   0 runner    (1001) docker     (127)    91914 2024-05-18 09:31:15.000000 glances-4.0.5/docs/_static/prometheus_server.png
+-rw-r--r--   0 runner    (1001) docker     (127)    27582 2024-05-18 09:31:15.000000 glances-4.0.5/docs/_static/quicklook-percpu.png
+-rw-r--r--   0 runner    (1001) docker     (127)    17789 2024-05-18 09:31:15.000000 glances-4.0.5/docs/_static/quicklook.png
+-rw-r--r--   0 runner    (1001) docker     (127)     5585 2024-05-18 09:31:15.000000 glances-4.0.5/docs/_static/raid.png
+-rw-r--r--   0 runner    (1001) docker     (127)     6362 2024-05-18 09:31:15.000000 glances-4.0.5/docs/_static/reddit.png
+-rw-r--r--   0 runner    (1001) docker     (127)  1089975 2024-05-18 09:31:15.000000 glances-4.0.5/docs/_static/screencast.gif
+-rw-r--r--   0 runner    (1001) docker     (127)   265567 2024-05-18 09:31:15.000000 glances-4.0.5/docs/_static/screenshot-web.png
+-rw-r--r--   0 runner    (1001) docker     (127)    36097 2024-05-18 09:31:15.000000 glances-4.0.5/docs/_static/screenshot-web2.png
+-rw-r--r--   0 runner    (1001) docker     (127)  1098062 2024-05-18 09:31:15.000000 glances-4.0.5/docs/_static/screenshot-wide.png
+-rw-r--r--   0 runner    (1001) docker     (127)   508044 2024-05-18 09:31:15.000000 glances-4.0.5/docs/_static/screenshot.png
+-rw-r--r--   0 runner    (1001) docker     (127)    16125 2024-05-18 09:31:15.000000 glances-4.0.5/docs/_static/sensors.png
+-rw-r--r--   0 runner    (1001) docker     (127)    21500 2024-05-18 09:31:15.000000 glances-4.0.5/docs/_static/smart.png
+-rw-r--r--   0 runner    (1001) docker     (127)    41952 2024-05-18 09:31:15.000000 glances-4.0.5/docs/_static/sparkline.png
+-rw-r--r--   0 runner    (1001) docker     (127)    23021 2024-05-18 09:31:15.000000 glances-4.0.5/docs/_static/trend.png
+-rw-r--r--   0 runner    (1001) docker     (127)     6395 2024-05-18 09:31:15.000000 glances-4.0.5/docs/_static/twitter-icon.png
+-rw-r--r--   0 runner    (1001) docker     (127)     4741 2024-05-18 09:31:15.000000 glances-4.0.5/docs/_static/wifi.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 09:31:20.309849 glances-4.0.5/docs/_templates/
+-rw-r--r--   0 runner    (1001) docker     (127)      357 2024-05-18 09:31:15.000000 glances-4.0.5/docs/_templates/links.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 09:31:20.313850 glances-4.0.5/docs/aoa/
+-rw-r--r--   0 runner    (1001) docker     (127)     2457 2024-05-18 09:31:15.000000 glances-4.0.5/docs/aoa/actions.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3690 2024-05-18 09:31:15.000000 glances-4.0.5/docs/aoa/amps.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      407 2024-05-18 09:31:15.000000 glances-4.0.5/docs/aoa/cloud.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1059 2024-05-18 09:31:15.000000 glances-4.0.5/docs/aoa/connections.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2179 2024-05-18 09:31:15.000000 glances-4.0.5/docs/aoa/containers.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3406 2024-05-18 09:31:15.000000 glances-4.0.5/docs/aoa/cpu.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      975 2024-05-18 09:31:15.000000 glances-4.0.5/docs/aoa/diskio.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1034 2024-05-18 09:31:15.000000 glances-4.0.5/docs/aoa/events.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1144 2024-05-18 09:31:15.000000 glances-4.0.5/docs/aoa/folders.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1584 2024-05-18 09:31:15.000000 glances-4.0.5/docs/aoa/fs.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1288 2024-05-18 09:31:15.000000 glances-4.0.5/docs/aoa/gpu.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      925 2024-05-18 09:31:15.000000 glances-4.0.5/docs/aoa/hddtemp.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2828 2024-05-18 09:31:15.000000 glances-4.0.5/docs/aoa/header.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      629 2024-05-18 09:31:15.000000 glances-4.0.5/docs/aoa/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      556 2024-05-18 09:31:15.000000 glances-4.0.5/docs/aoa/irq.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2227 2024-05-18 09:31:15.000000 glances-4.0.5/docs/aoa/load.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2526 2024-05-18 09:31:15.000000 glances-4.0.5/docs/aoa/memory.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1963 2024-05-18 09:31:15.000000 glances-4.0.5/docs/aoa/network.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1991 2024-05-18 09:31:15.000000 glances-4.0.5/docs/aoa/ports.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     9688 2024-05-18 09:31:15.000000 glances-4.0.5/docs/aoa/ps.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1266 2024-05-18 09:31:15.000000 glances-4.0.5/docs/aoa/quicklook.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      551 2024-05-18 09:31:15.000000 glances-4.0.5/docs/aoa/raid.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1349 2024-05-18 09:31:15.000000 glances-4.0.5/docs/aoa/sensors.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      572 2024-05-18 09:31:15.000000 glances-4.0.5/docs/aoa/smart.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      623 2024-05-18 09:31:15.000000 glances-4.0.5/docs/aoa/wifi.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    53003 2024-05-18 09:31:15.000000 glances-4.0.5/docs/api.rst
+-rwxr-xr-x   0 runner    (1001) docker     (127)       28 2024-05-18 09:31:15.000000 glances-4.0.5/docs/build.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     7977 2024-05-18 09:31:15.000000 glances-4.0.5/docs/cmds.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     9768 2024-05-18 09:31:15.000000 glances-4.0.5/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6715 2024-05-18 09:31:15.000000 glances-4.0.5/docs/config.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 09:31:20.313850 glances-4.0.5/docs/dev/
+-rw-r--r--   0 runner    (1001) docker     (127)      457 2024-05-18 09:31:15.000000 glances-4.0.5/docs/dev/README.txt
+-rw-r--r--   0 runner    (1001) docker     (127)   328258 2024-05-18 09:31:15.000000 glances-4.0.5/docs/dev/glances-cprofile.png
+-rw-r--r--   0 runner    (1001) docker     (127)     8376 2024-05-18 09:31:15.000000 glances-4.0.5/docs/docker.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      137 2024-05-18 09:31:15.000000 glances-4.0.5/docs/faq.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1755 2024-05-18 09:31:15.000000 glances-4.0.5/docs/glances.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 09:31:20.317849 glances-4.0.5/docs/gw/
+-rw-r--r--   0 runner    (1001) docker     (127)      756 2024-05-18 09:31:15.000000 glances-4.0.5/docs/gw/cassandra.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1094 2024-05-18 09:31:15.000000 glances-4.0.5/docs/gw/couchdb.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      843 2024-05-18 09:31:15.000000 glances-4.0.5/docs/gw/csv.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      500 2024-05-18 09:31:15.000000 glances-4.0.5/docs/gw/elastic.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1141 2024-05-18 09:31:15.000000 glances-4.0.5/docs/gw/graph.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      836 2024-05-18 09:31:15.000000 glances-4.0.5/docs/gw/graphite.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      401 2024-05-18 09:31:15.000000 glances-4.0.5/docs/gw/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4597 2024-05-18 09:31:15.000000 glances-4.0.5/docs/gw/influxdb.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-18 09:31:15.000000 glances-4.0.5/docs/gw/json.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1460 2024-05-18 09:31:15.000000 glances-4.0.5/docs/gw/kafka.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      851 2024-05-18 09:31:15.000000 glances-4.0.5/docs/gw/mongodb.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      700 2024-05-18 09:31:15.000000 glances-4.0.5/docs/gw/mqtt.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      386 2024-05-18 09:31:15.000000 glances-4.0.5/docs/gw/opentsdb.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1196 2024-05-18 09:31:15.000000 glances-4.0.5/docs/gw/prometheus.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      415 2024-05-18 09:31:15.000000 glances-4.0.5/docs/gw/rabbitmq.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      845 2024-05-18 09:31:15.000000 glances-4.0.5/docs/gw/restful.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      333 2024-05-18 09:31:15.000000 glances-4.0.5/docs/gw/riemann.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      580 2024-05-18 09:31:15.000000 glances-4.0.5/docs/gw/statsd.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1196 2024-05-18 09:31:15.000000 glances-4.0.5/docs/gw/zeromq.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      805 2024-05-18 09:31:15.000000 glances-4.0.5/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-05-18 09:31:15.000000 glances-4.0.5/docs/install.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     7251 2024-05-18 09:31:15.000000 glances-4.0.5/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 09:31:20.317849 glances-4.0.5/docs/man/
+-rw-r--r--   0 runner    (1001) docker     (127)    19253 2024-05-18 09:31:15.000000 glances-4.0.5/docs/man/glances.1
+-rw-r--r--   0 runner    (1001) docker     (127)     1909 2024-05-18 09:31:15.000000 glances-4.0.5/docs/objects.inv
+-rw-r--r--   0 runner    (1001) docker     (127)     6081 2024-05-18 09:31:15.000000 glances-4.0.5/docs/quickstart.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      326 2024-05-18 09:31:15.000000 glances-4.0.5/docs/support.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 09:31:20.321850 glances-4.0.5/glances/
+-rw-r--r--   0 runner    (1001) docker     (127)     5223 2024-05-18 09:31:15.000000 glances-4.0.5/glances/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      309 2024-05-18 09:31:15.000000 glances-4.0.5/glances/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3022 2024-05-18 09:31:15.000000 glances-4.0.5/glances/actions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 09:31:20.321850 glances-4.0.5/glances/amps/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-18 09:31:15.000000 glances-4.0.5/glances/amps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6255 2024-05-18 09:31:15.000000 glances-4.0.5/glances/amps/amp.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 09:31:20.321850 glances-4.0.5/glances/amps/default/
+-rw-r--r--   0 runner    (1001) docker     (127)     2219 2024-05-18 09:31:15.000000 glances-4.0.5/glances/amps/default/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 09:31:20.321850 glances-4.0.5/glances/amps/nginx/
+-rw-r--r--   0 runner    (1001) docker     (127)     2575 2024-05-18 09:31:15.000000 glances-4.0.5/glances/amps/nginx/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 09:31:20.321850 glances-4.0.5/glances/amps/systemd/
+-rw-r--r--   0 runner    (1001) docker     (127)     2531 2024-05-18 09:31:15.000000 glances-4.0.5/glances/amps/systemd/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 09:31:20.321850 glances-4.0.5/glances/amps/systemv/
+-rw-r--r--   0 runner    (1001) docker     (127)     2357 2024-05-18 09:31:15.000000 glances-4.0.5/glances/amps/systemv/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5357 2024-05-18 09:31:15.000000 glances-4.0.5/glances/amps_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3349 2024-05-18 09:31:15.000000 glances-4.0.5/glances/attribute.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9449 2024-05-18 09:31:15.000000 glances-4.0.5/glances/autodiscover.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8791 2024-05-18 09:31:15.000000 glances-4.0.5/glances/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9967 2024-05-18 09:31:15.000000 glances-4.0.5/glances/client_browser.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12332 2024-05-18 09:31:15.000000 glances-4.0.5/glances/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4949 2024-05-18 09:31:15.000000 glances-4.0.5/glances/cpu_percent.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2430 2024-05-18 09:31:15.000000 glances-4.0.5/glances/event.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15722 2024-05-18 09:31:15.000000 glances-4.0.5/glances/events_list.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 09:31:20.321850 glances-4.0.5/glances/exports/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-18 09:31:15.000000 glances-4.0.5/glances/exports/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7620 2024-05-18 09:31:15.000000 glances-4.0.5/glances/exports/export.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 09:31:20.321850 glances-4.0.5/glances/exports/glances_cassandra/
+-rw-r--r--   0 runner    (1001) docker     (127)     4311 2024-05-18 09:31:15.000000 glances-4.0.5/glances/exports/glances_cassandra/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 09:31:20.325850 glances-4.0.5/glances/exports/glances_couchdb/
+-rw-r--r--   0 runner    (1001) docker     (127)     2646 2024-05-18 09:31:15.000000 glances-4.0.5/glances/exports/glances_couchdb/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 09:31:20.325850 glances-4.0.5/glances/exports/glances_csv/
+-rw-r--r--   0 runner    (1001) docker     (127)     3969 2024-05-18 09:31:15.000000 glances-4.0.5/glances/exports/glances_csv/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 09:31:20.325850 glances-4.0.5/glances/exports/glances_elasticsearch/
+-rw-r--r--   0 runner    (1001) docker     (127)     2779 2024-05-18 09:31:15.000000 glances-4.0.5/glances/exports/glances_elasticsearch/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 09:31:20.325850 glances-4.0.5/glances/exports/glances_graph/
+-rw-r--r--   0 runner    (1001) docker     (127)     4331 2024-05-18 09:31:15.000000 glances-4.0.5/glances/exports/glances_graph/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 09:31:20.325850 glances-4.0.5/glances/exports/glances_graphite/
+-rw-r--r--   0 runner    (1001) docker     (127)     3195 2024-05-18 09:31:15.000000 glances-4.0.5/glances/exports/glances_graphite/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 09:31:20.325850 glances-4.0.5/glances/exports/glances_influxdb/
+-rw-r--r--   0 runner    (1001) docker     (127)     5865 2024-05-18 09:31:15.000000 glances-4.0.5/glances/exports/glances_influxdb/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 09:31:20.325850 glances-4.0.5/glances/exports/glances_influxdb2/
+-rw-r--r--   0 runner    (1001) docker     (127)     6482 2024-05-18 09:31:15.000000 glances-4.0.5/glances/exports/glances_influxdb2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 09:31:20.325850 glances-4.0.5/glances/exports/glances_json/
+-rw-r--r--   0 runner    (1001) docker     (127)     1799 2024-05-18 09:31:15.000000 glances-4.0.5/glances/exports/glances_json/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 09:31:20.325850 glances-4.0.5/glances/exports/glances_kafka/
+-rw-r--r--   0 runner    (1001) docker     (127)     2764 2024-05-18 09:31:15.000000 glances-4.0.5/glances/exports/glances_kafka/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 09:31:20.325850 glances-4.0.5/glances/exports/glances_mongodb/
+-rw-r--r--   0 runner    (1001) docker     (127)     2204 2024-05-18 09:31:15.000000 glances-4.0.5/glances/exports/glances_mongodb/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 09:31:20.325850 glances-4.0.5/glances/exports/glances_mqtt/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4955 2024-05-18 09:31:15.000000 glances-4.0.5/glances/exports/glances_mqtt/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 09:31:20.325850 glances-4.0.5/glances/exports/glances_opentsdb/
+-rw-r--r--   0 runner    (1001) docker     (127)     2393 2024-05-18 09:31:15.000000 glances-4.0.5/glances/exports/glances_opentsdb/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 09:31:20.325850 glances-4.0.5/glances/exports/glances_prometheus/
+-rw-r--r--   0 runner    (1001) docker     (127)     3130 2024-05-18 09:31:15.000000 glances-4.0.5/glances/exports/glances_prometheus/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 09:31:20.325850 glances-4.0.5/glances/exports/glances_rabbitmq/
+-rw-r--r--   0 runner    (1001) docker     (127)     2749 2024-05-18 09:31:15.000000 glances-4.0.5/glances/exports/glances_rabbitmq/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 09:31:20.325850 glances-4.0.5/glances/exports/glances_restful/
+-rw-r--r--   0 runner    (1001) docker     (127)     2089 2024-05-18 09:31:15.000000 glances-4.0.5/glances/exports/glances_restful/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 09:31:20.325850 glances-4.0.5/glances/exports/glances_riemann/
+-rw-r--r--   0 runner    (1001) docker     (127)     1925 2024-05-18 09:31:15.000000 glances-4.0.5/glances/exports/glances_riemann/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 09:31:20.325850 glances-4.0.5/glances/exports/glances_statsd/
+-rw-r--r--   0 runner    (1001) docker     (127)     2182 2024-05-18 09:31:15.000000 glances-4.0.5/glances/exports/glances_statsd/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 09:31:20.325850 glances-4.0.5/glances/exports/glances_zeromq/
+-rw-r--r--   0 runner    (1001) docker     (127)     2812 2024-05-18 09:31:15.000000 glances-4.0.5/glances/exports/glances_zeromq/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5779 2024-05-18 09:31:15.000000 glances-4.0.5/glances/filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5818 2024-05-18 09:31:15.000000 glances-4.0.5/glances/folder_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12176 2024-05-18 09:31:15.000000 glances-4.0.5/glances/globals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1376 2024-05-18 09:31:15.000000 glances-4.0.5/glances/history.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3231 2024-05-18 09:31:15.000000 glances-4.0.5/glances/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30679 2024-05-18 09:31:15.000000 glances-4.0.5/glances/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5879 2024-05-18 09:31:15.000000 glances-4.0.5/glances/outdated.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 09:31:20.329850 glances-4.0.5/glances/outputs/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-18 09:31:15.000000 glances-4.0.5/glances/outputs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3678 2024-05-18 09:31:15.000000 glances-4.0.5/glances/outputs/glances_bars.py
+-rw-r--r--   0 runner    (1001) docker     (127)    48469 2024-05-18 09:31:15.000000 glances-4.0.5/glances/outputs/glances_curses.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12555 2024-05-18 09:31:15.000000 glances-4.0.5/glances/outputs/glances_curses_browser.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29542 2024-05-18 09:31:15.000000 glances-4.0.5/glances/outputs/glances_restful_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2657 2024-05-18 09:31:15.000000 glances-4.0.5/glances/outputs/glances_sparklines.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2942 2024-05-18 09:31:15.000000 glances-4.0.5/glances/outputs/glances_stdout.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11392 2024-05-18 09:31:15.000000 glances-4.0.5/glances/outputs/glances_stdout_apidoc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3513 2024-05-18 09:31:15.000000 glances-4.0.5/glances/outputs/glances_stdout_csv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4229 2024-05-18 09:31:15.000000 glances-4.0.5/glances/outputs/glances_stdout_issue.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1393 2024-05-18 09:31:15.000000 glances-4.0.5/glances/outputs/glances_stdout_json.py
+-rw-r--r--   0 runner    (1001) docker     (127)      745 2024-05-18 09:31:15.000000 glances-4.0.5/glances/outputs/glances_unicode.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 09:31:20.329850 glances-4.0.5/glances/outputs/static/
+-rw-r--r--   0 runner    (1001) docker     (127)      245 2024-05-18 09:31:15.000000 glances-4.0.5/glances/outputs/static/.eslintrc.js
+-rw-r--r--   0 runner    (1001) docker     (127)      182 2024-05-18 09:31:15.000000 glances-4.0.5/glances/outputs/static/.prettierrc.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1122 2024-05-18 09:31:15.000000 glances-4.0.5/glances/outputs/static/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 09:31:20.329850 glances-4.0.5/glances/outputs/static/css/
+-rw-r--r--   0 runner    (1001) docker     (127)     1991 2024-05-18 09:31:15.000000 glances-4.0.5/glances/outputs/static/css/bootstrap.less
+-rw-r--r--   0 runner    (1001) docker     (127)     5635 2024-05-18 09:31:15.000000 glances-4.0.5/glances/outputs/static/css/style.scss
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-18 09:31:15.000000 glances-4.0.5/glances/outputs/static/css/variables.less
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 09:31:20.329850 glances-4.0.5/glances/outputs/static/images/
+-rw-r--r--   0 runner    (1001) docker     (127)     4286 2024-05-18 09:31:15.000000 glances-4.0.5/glances/outputs/static/images/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (127)    50295 2024-05-18 09:31:15.000000 glances-4.0.5/glances/outputs/static/images/glances.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 09:31:20.329850 glances-4.0.5/glances/outputs/static/js/
+-rw-r--r--   0 runner    (1001) docker     (127)    15387 2024-05-18 09:31:15.000000 glances-4.0.5/glances/outputs/static/js/App.vue
+-rw-r--r--   0 runner    (1001) docker     (127)      326 2024-05-18 09:31:15.000000 glances-4.0.5/glances/outputs/static/js/app.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 09:31:20.333850 glances-4.0.5/glances/outputs/static/js/components/
+-rw-r--r--   0 runner    (1001) docker     (127)    11318 2024-05-18 09:31:15.000000 glances-4.0.5/glances/outputs/static/js/components/help.vue
+-rw-r--r--   0 runner    (1001) docker     (127)     3485 2024-05-18 09:31:15.000000 glances-4.0.5/glances/outputs/static/js/components/plugin-alert.vue
+-rw-r--r--   0 runner    (1001) docker     (127)     1656 2024-05-18 09:31:15.000000 glances-4.0.5/glances/outputs/static/js/components/plugin-amps.vue
+-rw-r--r--   0 runner    (1001) docker     (127)      717 2024-05-18 09:31:15.000000 glances-4.0.5/glances/outputs/static/js/components/plugin-cloud.vue
+-rw-r--r--   0 runner    (1001) docker     (127)     2382 2024-05-18 09:31:15.000000 glances-4.0.5/glances/outputs/static/js/components/plugin-connections.vue
+-rw-r--r--   0 runner    (1001) docker     (127)     7663 2024-05-18 09:31:15.000000 glances-4.0.5/glances/outputs/static/js/components/plugin-containers.vue
+-rw-r--r--   0 runner    (1001) docker     (127)     7350 2024-05-18 09:31:15.000000 glances-4.0.5/glances/outputs/static/js/components/plugin-cpu.vue
+-rw-r--r--   0 runner    (1001) docker     (127)     2526 2024-05-18 09:31:15.000000 glances-4.0.5/glances/outputs/static/js/components/plugin-diskio.vue
+-rw-r--r--   0 runner    (1001) docker     (127)     1985 2024-05-18 09:31:15.000000 glances-4.0.5/glances/outputs/static/js/components/plugin-folders.vue
+-rw-r--r--   0 runner    (1001) docker     (127)     2577 2024-05-18 09:31:15.000000 glances-4.0.5/glances/outputs/static/js/components/plugin-fs.vue
+-rw-r--r--   0 runner    (1001) docker     (127)     4633 2024-05-18 09:31:15.000000 glances-4.0.5/glances/outputs/static/js/components/plugin-gpu.vue
+-rw-r--r--   0 runner    (1001) docker     (127)      979 2024-05-18 09:31:15.000000 glances-4.0.5/glances/outputs/static/js/components/plugin-ip.vue
+-rw-r--r--   0 runner    (1001) docker     (127)     1048 2024-05-18 09:31:15.000000 glances-4.0.5/glances/outputs/static/js/components/plugin-irq.vue
+-rw-r--r--   0 runner    (1001) docker     (127)     1864 2024-05-18 09:31:15.000000 glances-4.0.5/glances/outputs/static/js/components/plugin-load.vue
+-rw-r--r--   0 runner    (1001) docker     (127)     1518 2024-05-18 09:31:15.000000 glances-4.0.5/glances/outputs/static/js/components/plugin-mem-more.vue
+-rw-r--r--   0 runner    (1001) docker     (127)     1742 2024-05-18 09:31:15.000000 glances-4.0.5/glances/outputs/static/js/components/plugin-mem.vue
+-rw-r--r--   0 runner    (1001) docker     (127)     1752 2024-05-18 09:31:15.000000 glances-4.0.5/glances/outputs/static/js/components/plugin-memswap.vue
+-rw-r--r--   0 runner    (1001) docker     (127)     4138 2024-05-18 09:31:15.000000 glances-4.0.5/glances/outputs/static/js/components/plugin-network.vue
+-rw-r--r--   0 runner    (1001) docker     (127)      525 2024-05-18 09:31:15.000000 glances-4.0.5/glances/outputs/static/js/components/plugin-now.vue
+-rw-r--r--   0 runner    (1001) docker     (127)     2659 2024-05-18 09:31:15.000000 glances-4.0.5/glances/outputs/static/js/components/plugin-percpu.vue
+-rw-r--r--   0 runner    (1001) docker     (127)     2192 2024-05-18 09:31:15.000000 glances-4.0.5/glances/outputs/static/js/components/plugin-ports.vue
+-rw-r--r--   0 runner    (1001) docker     (127)     2869 2024-05-18 09:31:15.000000 glances-4.0.5/glances/outputs/static/js/components/plugin-process.vue
+-rw-r--r--   0 runner    (1001) docker     (127)     1347 2024-05-18 09:31:15.000000 glances-4.0.5/glances/outputs/static/js/components/plugin-processcount.vue
+-rw-r--r--   0 runner    (1001) docker     (127)     9459 2024-05-18 09:31:15.000000 glances-4.0.5/glances/outputs/static/js/components/plugin-processlist.vue
+-rw-r--r--   0 runner    (1001) docker     (127)     5094 2024-05-18 09:31:15.000000 glances-4.0.5/glances/outputs/static/js/components/plugin-quicklook.vue
+-rw-r--r--   0 runner    (1001) docker     (127)     3082 2024-05-18 09:31:15.000000 glances-4.0.5/glances/outputs/static/js/components/plugin-raid.vue
+-rw-r--r--   0 runner    (1001) docker     (127)     2125 2024-05-18 09:31:15.000000 glances-4.0.5/glances/outputs/static/js/components/plugin-sensors.vue
+-rw-r--r--   0 runner    (1001) docker     (127)     1738 2024-05-18 09:31:15.000000 glances-4.0.5/glances/outputs/static/js/components/plugin-smart.vue
+-rw-r--r--   0 runner    (1001) docker     (127)      810 2024-05-18 09:31:15.000000 glances-4.0.5/glances/outputs/static/js/components/plugin-system.vue
+-rw-r--r--   0 runner    (1001) docker     (127)      326 2024-05-18 09:31:15.000000 glances-4.0.5/glances/outputs/static/js/components/plugin-uptime.vue
+-rw-r--r--   0 runner    (1001) docker     (127)     1776 2024-05-18 09:31:15.000000 glances-4.0.5/glances/outputs/static/js/components/plugin-wifi.vue
+-rw-r--r--   0 runner    (1001) docker     (127)     3362 2024-05-18 09:31:15.000000 glances-4.0.5/glances/outputs/static/js/filters.js
+-rw-r--r--   0 runner    (1001) docker     (127)     4000 2024-05-18 09:31:15.000000 glances-4.0.5/glances/outputs/static/js/services.js
+-rw-r--r--   0 runner    (1001) docker     (127)      153 2024-05-18 09:31:15.000000 glances-4.0.5/glances/outputs/static/js/store.js
+-rw-r--r--   0 runner    (1001) docker     (127)      235 2024-05-18 09:31:15.000000 glances-4.0.5/glances/outputs/static/js/uiconfig.json
+-rw-r--r--   0 runner    (1001) docker     (127)   452411 2024-05-18 09:31:15.000000 glances-4.0.5/glances/outputs/static/package-lock.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-05-18 09:31:15.000000 glances-4.0.5/glances/outputs/static/package.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 09:31:20.337850 glances-4.0.5/glances/outputs/static/public/
+-rw-r--r--   0 runner    (1001) docker     (127)    50295 2024-05-18 09:31:15.000000 glances-4.0.5/glances/outputs/static/public/1272f6e9e8f9d6bfd6de.png
+-rw-r--r--   0 runner    (1001) docker     (127)     4286 2024-05-18 09:31:15.000000 glances-4.0.5/glances/outputs/static/public/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (127)   448748 2024-05-18 09:31:15.000000 glances-4.0.5/glances/outputs/static/public/glances.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 09:31:20.337850 glances-4.0.5/glances/outputs/static/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)      477 2024-05-18 09:31:15.000000 glances-4.0.5/glances/outputs/static/templates/index.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2651 2024-05-18 09:31:15.000000 glances-4.0.5/glances/outputs/static/webpack.config.js
+-rw-r--r--   0 runner    (1001) docker     (127)     4770 2024-05-18 09:31:15.000000 glances-4.0.5/glances/password.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2109 2024-05-18 09:31:15.000000 glances-4.0.5/glances/password_list.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 09:31:20.337850 glances-4.0.5/glances/plugins/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-18 09:31:15.000000 glances-4.0.5/glances/plugins/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 09:31:20.337850 glances-4.0.5/glances/plugins/__pycache__/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-18 09:31:15.000000 glances-4.0.5/glances/plugins/__pycache__/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 09:31:20.337850 glances-4.0.5/glances/plugins/alert/
+-rw-r--r--   0 runner    (1001) docker     (127)     6184 2024-05-18 09:31:15.000000 glances-4.0.5/glances/plugins/alert/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 09:31:20.337850 glances-4.0.5/glances/plugins/amps/
+-rw-r--r--   0 runner    (1001) docker     (127)     4926 2024-05-18 09:31:15.000000 glances-4.0.5/glances/plugins/amps/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 09:31:20.337850 glances-4.0.5/glances/plugins/cloud/
+-rw-r--r--   0 runner    (1001) docker     (127)     6672 2024-05-18 09:31:15.000000 glances-4.0.5/glances/plugins/cloud/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 09:31:20.337850 glances-4.0.5/glances/plugins/connections/
+-rw-r--r--   0 runner    (1001) docker     (127)     8133 2024-05-18 09:31:15.000000 glances-4.0.5/glances/plugins/connections/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 09:31:20.337850 glances-4.0.5/glances/plugins/containers/
+-rw-r--r--   0 runner    (1001) docker     (127)    18169 2024-05-18 09:31:15.000000 glances-4.0.5/glances/plugins/containers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 09:31:20.337850 glances-4.0.5/glances/plugins/containers/engines/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-18 09:31:15.000000 glances-4.0.5/glances/plugins/containers/engines/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13849 2024-05-18 09:31:15.000000 glances-4.0.5/glances/plugins/containers/engines/docker.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13212 2024-05-18 09:31:15.000000 glances-4.0.5/glances/plugins/containers/engines/podman.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2616 2024-05-18 09:31:15.000000 glances-4.0.5/glances/plugins/containers/stats_streamer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 09:31:20.337850 glances-4.0.5/glances/plugins/core/
+-rw-r--r--   0 runner    (1001) docker     (127)     2320 2024-05-18 09:31:15.000000 glances-4.0.5/glances/plugins/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 09:31:20.337850 glances-4.0.5/glances/plugins/cpu/
+-rw-r--r--   0 runner    (1001) docker     (127)    15498 2024-05-18 09:31:15.000000 glances-4.0.5/glances/plugins/cpu/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 09:31:20.337850 glances-4.0.5/glances/plugins/diskio/
+-rw-r--r--   0 runner    (1001) docker     (127)     8072 2024-05-18 09:31:15.000000 glances-4.0.5/glances/plugins/diskio/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 09:31:20.337850 glances-4.0.5/glances/plugins/folders/
+-rw-r--r--   0 runner    (1001) docker     (127)     5053 2024-05-18 09:31:15.000000 glances-4.0.5/glances/plugins/folders/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 09:31:20.337850 glances-4.0.5/glances/plugins/fs/
+-rw-r--r--   0 runner    (1001) docker     (127)    11663 2024-05-18 09:31:15.000000 glances-4.0.5/glances/plugins/fs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 09:31:20.337850 glances-4.0.5/glances/plugins/gpu/
+-rw-r--r--   0 runner    (1001) docker     (127)     9684 2024-05-18 09:31:15.000000 glances-4.0.5/glances/plugins/gpu/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 09:31:20.337850 glances-4.0.5/glances/plugins/gpu/cards/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-18 09:31:15.000000 glances-4.0.5/glances/plugins/gpu/cards/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5059 2024-05-18 09:31:15.000000 glances-4.0.5/glances/plugins/gpu/cards/amd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3517 2024-05-18 09:31:15.000000 glances-4.0.5/glances/plugins/gpu/cards/nvidia.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 09:31:20.337850 glances-4.0.5/glances/plugins/help/
+-rw-r--r--   0 runner    (1001) docker     (127)    10081 2024-05-18 09:31:15.000000 glances-4.0.5/glances/plugins/help/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 09:31:20.341850 glances-4.0.5/glances/plugins/ip/
+-rw-r--r--   0 runner    (1001) docker     (127)     9024 2024-05-18 09:31:15.000000 glances-4.0.5/glances/plugins/ip/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 09:31:20.341850 glances-4.0.5/glances/plugins/irq/
+-rw-r--r--   0 runner    (1001) docker     (127)     6797 2024-05-18 09:31:15.000000 glances-4.0.5/glances/plugins/irq/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 09:31:20.341850 glances-4.0.5/glances/plugins/load/
+-rw-r--r--   0 runner    (1001) docker     (127)     6699 2024-05-18 09:31:15.000000 glances-4.0.5/glances/plugins/load/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 09:31:20.341850 glances-4.0.5/glances/plugins/mem/
+-rw-r--r--   0 runner    (1001) docker     (127)    10913 2024-05-18 09:31:15.000000 glances-4.0.5/glances/plugins/mem/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 09:31:20.341850 glances-4.0.5/glances/plugins/memswap/
+-rw-r--r--   0 runner    (1001) docker     (127)     7454 2024-05-18 09:31:15.000000 glances-4.0.5/glances/plugins/memswap/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 09:31:20.341850 glances-4.0.5/glances/plugins/network/
+-rw-r--r--   0 runner    (1001) docker     (127)    11704 2024-05-18 09:31:15.000000 glances-4.0.5/glances/plugins/network/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 09:31:20.341850 glances-4.0.5/glances/plugins/now/
+-rw-r--r--   0 runner    (1001) docker     (127)     2561 2024-05-18 09:31:15.000000 glances-4.0.5/glances/plugins/now/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 09:31:20.341850 glances-4.0.5/glances/plugins/percpu/
+-rw-r--r--   0 runner    (1001) docker     (127)     7467 2024-05-18 09:31:15.000000 glances-4.0.5/glances/plugins/percpu/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 09:31:20.341850 glances-4.0.5/glances/plugins/plugin/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-18 09:31:15.000000 glances-4.0.5/glances/plugins/plugin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    46696 2024-05-18 09:31:15.000000 glances-4.0.5/glances/plugins/plugin/model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 09:31:20.341850 glances-4.0.5/glances/plugins/ports/
+-rw-r--r--   0 runner    (1001) docker     (127)    12756 2024-05-18 09:31:15.000000 glances-4.0.5/glances/plugins/ports/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 09:31:20.341850 glances-4.0.5/glances/plugins/processcount/
+-rw-r--r--   0 runner    (1001) docker     (127)     5480 2024-05-18 09:31:15.000000 glances-4.0.5/glances/plugins/processcount/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 09:31:20.341850 glances-4.0.5/glances/plugins/processlist/
+-rw-r--r--   0 runner    (1001) docker     (127)    36550 2024-05-18 09:31:15.000000 glances-4.0.5/glances/plugins/processlist/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 09:31:20.341850 glances-4.0.5/glances/plugins/psutilversion/
+-rw-r--r--   0 runner    (1001) docker     (127)     1189 2024-05-18 09:31:15.000000 glances-4.0.5/glances/plugins/psutilversion/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 09:31:20.341850 glances-4.0.5/glances/plugins/quicklook/
+-rw-r--r--   0 runner    (1001) docker     (127)    11764 2024-05-18 09:31:15.000000 glances-4.0.5/glances/plugins/quicklook/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 09:31:20.341850 glances-4.0.5/glances/plugins/raid/
+-rw-r--r--   0 runner    (1001) docker     (127)     6458 2024-05-18 09:31:15.000000 glances-4.0.5/glances/plugins/raid/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 09:31:20.341850 glances-4.0.5/glances/plugins/sensors/
+-rw-r--r--   0 runner    (1001) docker     (127)    15060 2024-05-18 09:31:15.000000 glances-4.0.5/glances/plugins/sensors/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 09:31:20.341850 glances-4.0.5/glances/plugins/sensors/sensor/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-18 09:31:15.000000 glances-4.0.5/glances/plugins/sensors/sensor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4423 2024-05-18 09:31:15.000000 glances-4.0.5/glances/plugins/sensors/sensor/glances_batpercent.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4863 2024-05-18 09:31:15.000000 glances-4.0.5/glances/plugins/sensors/sensor/glances_hddtemp.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 09:31:20.341850 glances-4.0.5/glances/plugins/smart/
+-rw-r--r--   0 runner    (1001) docker     (127)     6326 2024-05-18 09:31:15.000000 glances-4.0.5/glances/plugins/smart/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 09:31:20.341850 glances-4.0.5/glances/plugins/system/
+-rw-r--r--   0 runner    (1001) docker     (127)     8214 2024-05-18 09:31:15.000000 glances-4.0.5/glances/plugins/system/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 09:31:20.341850 glances-4.0.5/glances/plugins/uptime/
+-rw-r--r--   0 runner    (1001) docker     (127)     2467 2024-05-18 09:31:15.000000 glances-4.0.5/glances/plugins/uptime/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 09:31:20.341850 glances-4.0.5/glances/plugins/version/
+-rw-r--r--   0 runner    (1001) docker     (127)     1173 2024-05-18 09:31:15.000000 glances-4.0.5/glances/plugins/version/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 09:31:20.341850 glances-4.0.5/glances/plugins/wifi/
+-rw-r--r--   0 runner    (1001) docker     (127)     6851 2024-05-18 09:31:15.000000 glances-4.0.5/glances/plugins/wifi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4831 2024-05-18 09:31:15.000000 glances-4.0.5/glances/ports_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26258 2024-05-18 09:31:15.000000 glances-4.0.5/glances/processes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2644 2024-05-18 09:31:15.000000 glances-4.0.5/glances/programs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2243 2024-05-18 09:31:15.000000 glances-4.0.5/glances/secure.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8072 2024-05-18 09:31:15.000000 glances-4.0.5/glances/server.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3884 2024-05-18 09:31:15.000000 glances-4.0.5/glances/snmp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7903 2024-05-18 09:31:15.000000 glances-4.0.5/glances/standalone.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3172 2024-05-18 09:31:15.000000 glances-4.0.5/glances/static_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14920 2024-05-18 09:31:15.000000 glances-4.0.5/glances/stats.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1945 2024-05-18 09:31:15.000000 glances-4.0.5/glances/stats_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3522 2024-05-18 09:31:15.000000 glances-4.0.5/glances/stats_client_snmp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1621 2024-05-18 09:31:15.000000 glances-4.0.5/glances/stats_server.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2557 2024-05-18 09:31:15.000000 glances-4.0.5/glances/thresholds.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1549 2024-05-18 09:31:15.000000 glances-4.0.5/glances/timer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4366 2024-05-18 09:31:15.000000 glances-4.0.5/glances/web_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1151 2024-05-18 09:31:15.000000 glances-4.0.5/glances/webserver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1794 2024-05-18 09:31:15.000000 glances-4.0.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-18 09:31:15.000000 glances-4.0.5/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-18 09:31:20.349850 glances-4.0.5/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4531 2024-05-18 09:31:15.000000 glances-4.0.5/setup.py
```

### Comparing `glances-4.0.4/AUTHORS` & `glances-4.0.5/AUTHORS`

 * *Files 3% similar despite different names*

```diff
@@ -60,7 +60,11 @@
 Frederic Aoustin (https://github.com/fraoustin) and Nicolas Bourges (installer) for the Windows port
 
 Aljaž Srebrnič for the MacPorts package
 http://www.macports.org/ports.php?by=name&substr=glances
 
 John Kirkham for the conda package (at conda-forge)
 https://github.com/conda-forge/glances-feedstock
+
+Rui Chen for the Homebrew package
+https://chenrui.dev/
+https://formulae.brew.sh/formula/glances
```

### Comparing `glances-4.0.4/CONTRIBUTING.md` & `glances-4.0.5/CONTRIBUTING.md`

 * *Files 2% similar despite different names*

```diff
@@ -6,29 +6,27 @@
 process easy and effective for everyone involved.
 
 Following these guidelines helps to communicate that you respect the time of
 the developers managing and developing this open source project. In return,
 they should reciprocate that respect in addressing your issue or assessing
 patches and features.
 
-
 ## Using the issue tracker
 
 The [issue tracker](https://github.com/nicolargo/glances/issues) is
 the preferred channel for [bug reports](#bug-reports), [features requests](#feature-requests)
 and [submitting pull requests](#pull-requests), but please respect the following
 restrictions:
 
 * Please **do not** use the issue tracker for personal support requests. An
   official Q&A exist. [Use it](https://groups.google.com/forum/?hl=en#!forum/glances-users)!
 
 * Please **do not** derail or troll issues. Keep the discussion on topic and
   respect the opinions of others.
 
-
 ## Bug reports
 
 A bug is a _demonstrable problem_ that is caused by the code in the repository.
 Good bug reports are extremely helpful, so thanks!
 
 Guidelines for bug reports:
 
@@ -61,27 +59,25 @@
 > Screenshot (if useful)
 >
 > Any other information you want to share that is relevant to the issue being
 > reported. This might include the lines of code that you have identified as
 > causing the bug, and potential solutions (and your opinions on their
 > merits).
 >
-> You can also run Glances in debug mode (-d) and paste/bin the glances.conf file (https://glances.readthedocs.io/en/latest/config.html).
+> You can also run Glances in debug mode (-d) and paste/bin the glances.conf file (<https://glances.readthedocs.io/en/latest/config.html>).
 >
 > Glances 3.2.0 or higher have also a --issue option to run a simple test. Please use it and copy/paste the output.
 
-
 ## Feature requests
 
 Feature requests are welcome. But take a moment to find out whether your idea
-fits with the scope and aims of the project. It's up to *you* to make a strong
+fits with the scope and aims of the project. It's up to _you* to make a strong
 case to convince the project's developers of the merits of this feature. Please
 provide as much detail and context as possible.
 
-
 ## Pull requests
 
 Good pull requests—patches, improvements, new features—are a fantastic
 help. They should remain focused in scope and avoid containing unrelated
 commits.
 
 **Please ask first** before embarking on any significant pull request (e.g.
@@ -129,14 +125,15 @@
    ```
 
 4. It's coding time !
    Please respect the following coding convention: [Elements of Python Style](https://github.com/amontalenti/elements-of-python-style)
 
 5. Test you code using the Makefile:
 
+   * make format ==> Format your code thanks to the Ruff linter
    * make run ==> Run Glances
    * make run-webserver ==> Run a Glances Web Server
    * make test ==> Run unit tests
    * make docs ==> Update docs
    * make webui ==> Compile a new Web UI
 
 6. Commit your changes in logical chunks. Please adhere to these [git commit
```

### Comparing `glances-4.0.4/COPYING` & `glances-4.0.5/COPYING`

 * *Files identical despite different names*

### Comparing `glances-4.0.4/Glances.egg-info/PKG-INFO` & `glances-4.0.5/Glances.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Glances
-Version: 4.0.4
+Version: 4.0.5
 Summary: A cross-platform curses-based monitoring tool
 Home-page: https://github.com/nicolargo/glances
 Author: Nicolas Hennion
 Author-email: nicolas@nicolargo.com
 License: LGPLv3
 Keywords: cli curses monitoring system
 Classifier: Development Status :: 5 - Production/Stable
@@ -22,19 +22,18 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: System :: Monitoring
 Requires-Python: >=3.8
 License-File: COPYING
 License-File: AUTHORS
-Requires-Dist: psutil>=5.6.7
 Requires-Dist: defusedxml
 Requires-Dist: packaging
+Requires-Dist: psutil>=5.6.7
 Requires-Dist: ujson>=5.4.0
-Requires-Dist: pydantic
 Provides-Extra: action
 Requires-Dist: chevron; extra == "action"
 Provides-Extra: browser
 Requires-Dist: zeroconf>=0.19.1; extra == "browser"
 Provides-Extra: cloud
 Requires-Dist: requests; extra == "cloud"
 Provides-Extra: containers
@@ -184,15 +183,14 @@
 ============
 
 - ``python>=3.8`` (use Glances 3.4.x for lower Python version)
 - ``psutil`` (better with latest version)
 - ``defusedxml`` (in order to monkey patch xmlrpc)
 - ``packaging`` (for the version comparison)
 - ``ujson`` (an optimized alternative to the standard json module)
-- ``pydantic`` (for the data validation support)
 
 *Note for Python 2 users*
 
 Glances version 4 or higher do not support Python 2 (and Python 3 < 3.8).
 Please uses Glances version 3.4.x if you need Python 2 support.
 
 Optional dependencies:
```

### Comparing `glances-4.0.4/Glances.egg-info/SOURCES.txt` & `glances-4.0.5/Glances.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 AUTHORS
 CONTRIBUTING.md
 COPYING
 MANIFEST.in
 NEWS.rst
 README.rst
+SECURITY.md
 pyproject.toml
+requirements.txt
 setup.py
 Glances.egg-info/PKG-INFO
 Glances.egg-info/SOURCES.txt
 Glances.egg-info/dependency_links.txt
 Glances.egg-info/entry_points.txt
 Glances.egg-info/requires.txt
 Glances.egg-info/top_level.txt
```

### Comparing `glances-4.0.4/Glances.egg-info/requires.txt` & `glances-4.0.5/Glances.egg-info/requires.txt`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,11 @@
-psutil>=5.6.7
 defusedxml
 packaging
+psutil>=5.6.7
 ujson>=5.4.0
-pydantic
 
 [action]
 chevron
 
 [all]
 chevron
 zeroconf>=0.19.1
```

### Comparing `glances-4.0.4/NEWS.rst` & `glances-4.0.5/NEWS.rst`

 * *Files 0% similar despite different names*

```diff
@@ -1,28 +1,43 @@
 ==============================================================================
                                 Glances ChangeLog
 ==============================================================================
 
 ===============
+Version 4.0.5
+===============
+
+* SensorType change in REST API breaks compatibility in 4.0.4 #2788
+* Please make pydantic optional dependency, not required one #2777
+* Update the Grafana dashboard #2780
+* 4.0.4 - On Glances startup "ERROR -- Can not init battery class #2776
+* In codeSpace (with Python 3.8), an error occurs in ./unittest-restful.py #2773
+
+Use Ruff as default Linter.
+
+===============
 Version 4.0.4
 ===============
 
-Hostfix release for support sensors on python3.8
+Hostfix release for support sensors plugin on python 3.8
 
 ===============
 Version 4.0.3
 ===============
 
-Additional fixes for Sensor plugin.
+Additional fixes for Sensor plugin
 
 ===============
 Version 4.0.2
 ===============
 
-Fix: Sensor plugin buggy due to race conditions.
+* hotfix: plugin(sensors) - race conditions btw fan_speed & temperature… #2766
+* fix: include requirements.txt and SECURITY.md for pypi dist #2761
+
+Thanks to RazCrimson for the sensors patch !
 
 ===============
 Version 4.0.1
 ===============
 
 Correct issue with CI (miss pydantic dep).
```

### Comparing `glances-4.0.4/PKG-INFO` & `glances-4.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Glances
-Version: 4.0.4
+Version: 4.0.5
 Summary: A cross-platform curses-based monitoring tool
 Home-page: https://github.com/nicolargo/glances
 Author: Nicolas Hennion
 Author-email: nicolas@nicolargo.com
 License: LGPLv3
 Keywords: cli curses monitoring system
 Classifier: Development Status :: 5 - Production/Stable
@@ -22,19 +22,18 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: System :: Monitoring
 Requires-Python: >=3.8
 License-File: COPYING
 License-File: AUTHORS
-Requires-Dist: psutil>=5.6.7
 Requires-Dist: defusedxml
 Requires-Dist: packaging
+Requires-Dist: psutil>=5.6.7
 Requires-Dist: ujson>=5.4.0
-Requires-Dist: pydantic
 Provides-Extra: action
 Requires-Dist: chevron; extra == "action"
 Provides-Extra: browser
 Requires-Dist: zeroconf>=0.19.1; extra == "browser"
 Provides-Extra: cloud
 Requires-Dist: requests; extra == "cloud"
 Provides-Extra: containers
@@ -184,15 +183,14 @@
 ============
 
 - ``python>=3.8`` (use Glances 3.4.x for lower Python version)
 - ``psutil`` (better with latest version)
 - ``defusedxml`` (in order to monkey patch xmlrpc)
 - ``packaging`` (for the version comparison)
 - ``ujson`` (an optimized alternative to the standard json module)
-- ``pydantic`` (for the data validation support)
 
 *Note for Python 2 users*
 
 Glances version 4 or higher do not support Python 2 (and Python 3 < 3.8).
 Please uses Glances version 3.4.x if you need Python 2 support.
 
 Optional dependencies:
```

### Comparing `glances-4.0.4/README.rst` & `glances-4.0.5/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -83,15 +83,14 @@
 ============
 
 - ``python>=3.8`` (use Glances 3.4.x for lower Python version)
 - ``psutil`` (better with latest version)
 - ``defusedxml`` (in order to monkey patch xmlrpc)
 - ``packaging`` (for the version comparison)
 - ``ujson`` (an optimized alternative to the standard json module)
-- ``pydantic`` (for the data validation support)
 
 *Note for Python 2 users*
 
 Glances version 4 or higher do not support Python 2 (and Python 3 < 3.8).
 Please uses Glances version 3.4.x if you need Python 2 support.
 
 Optional dependencies:
```

### Comparing `glances-4.0.4/conf/glances.conf` & `glances-4.0.5/conf/glances.conf`

 * *Files 0% similar despite different names*

```diff
@@ -313,15 +313,15 @@
 # Documentation: https://glances.readthedocs.io/en/latest/aoa/cloud.html
 # This plugin is disabled by default
 disable=True
 
 [raid]
 # Documentation: https://glances.readthedocs.io/en/latest/aoa/raid.html
 # This plugin is disabled by default
-disable=False
+disable=True
 
 [smart]
 # Documentation: https://glances.readthedocs.io/en/latest/aoa/smart.html
 # This plugin is disabled by default
 disable=True
 
 [hddtemp]
```

### Comparing `glances-4.0.4/docs/Makefile` & `glances-4.0.5/docs/Makefile`

 * *Files identical despite different names*

### Comparing `glances-4.0.4/docs/_static/Glances Logo dark.svg` & `glances-4.0.5/docs/_static/Glances Logo dark.svg`

 * *Files identical despite different names*

### Comparing `glances-4.0.4/docs/_static/Glances Logo.svg` & `glances-4.0.5/docs/_static/Glances Logo.svg`

 * *Files identical despite different names*

### Comparing `glances-4.0.4/docs/_static/Glances Text Logo dark.svg` & `glances-4.0.5/docs/_static/Glances Text Logo dark.svg`

 * *Files identical despite different names*

### Comparing `glances-4.0.4/docs/_static/Glances Text Logo.svg` & `glances-4.0.5/docs/_static/Glances Text Logo.svg`

 * *Files identical despite different names*

### Comparing `glances-4.0.4/docs/_static/amp-dropbox.png` & `glances-4.0.5/docs/_static/amp-dropbox.png`

 * *Files identical despite different names*

### Comparing `glances-4.0.4/docs/_static/amp-python-warning.png` & `glances-4.0.5/docs/_static/amp-python-warning.png`

 * *Files identical despite different names*

### Comparing `glances-4.0.4/docs/_static/amp-python.png` & `glances-4.0.5/docs/_static/amp-python.png`

 * *Files identical despite different names*

### Comparing `glances-4.0.4/docs/_static/amps.png` & `glances-4.0.5/docs/_static/amps.png`

 * *Files identical despite different names*

### Comparing `glances-4.0.4/docs/_static/aws.png` & `glances-4.0.5/docs/_static/aws.png`

 * *Files identical despite different names*

### Comparing `glances-4.0.4/docs/_static/browser.png` & `glances-4.0.5/docs/_static/browser.png`

 * *Files identical despite different names*

### Comparing `glances-4.0.4/docs/_static/cloud.png` & `glances-4.0.5/docs/_static/cloud.png`

 * *Files identical despite different names*

### Comparing `glances-4.0.4/docs/_static/connected.png` & `glances-4.0.5/docs/_static/connected.png`

 * *Files identical despite different names*

### Comparing `glances-4.0.4/docs/_static/connections.png` & `glances-4.0.5/docs/_static/connections.png`

 * *Files identical despite different names*

### Comparing `glances-4.0.4/docs/_static/containers.png` & `glances-4.0.5/docs/_static/containers.png`

 * *Files identical despite different names*

### Comparing `glances-4.0.4/docs/_static/cpu-wide.png` & `glances-4.0.5/docs/_static/cpu-wide.png`

 * *Files identical despite different names*

### Comparing `glances-4.0.4/docs/_static/cpu.png` & `glances-4.0.5/docs/_static/cpu.png`

 * *Files identical despite different names*

### Comparing `glances-4.0.4/docs/_static/disconnected.png` & `glances-4.0.5/docs/_static/disconnected.png`

 * *Files identical despite different names*

### Comparing `glances-4.0.4/docs/_static/diskio.png` & `glances-4.0.5/docs/_static/diskio.png`

 * *Files identical despite different names*

### Comparing `glances-4.0.4/docs/_static/events.png` & `glances-4.0.5/docs/_static/events.png`

 * *Files identical despite different names*

### Comparing `glances-4.0.4/docs/_static/folders.png` & `glances-4.0.5/docs/_static/folders.png`

 * *Files identical despite different names*

### Comparing `glances-4.0.4/docs/_static/fs.png` & `glances-4.0.5/docs/_static/fs.png`

 * *Files identical despite different names*

### Comparing `glances-4.0.4/docs/_static/glances-architecture.excalidraw` & `glances-4.0.5/docs/_static/glances-architecture.excalidraw`

 * *Files identical despite different names*

### Comparing `glances-4.0.4/docs/_static/glances-architecture.png` & `glances-4.0.5/docs/_static/glances-architecture.png`

 * *Files identical despite different names*

### Comparing `glances-4.0.4/docs/_static/glances-cgraph.svg` & `glances-4.0.5/docs/_static/glances-cgraph.svg`

 * *Files identical despite different names*

### Comparing `glances-4.0.4/docs/_static/glances-flame.svg` & `glances-4.0.5/docs/_static/glances-flame.svg`

 * *Files identical despite different names*

### Comparing `glances-4.0.4/docs/_static/glances-influxdb.png` & `glances-4.0.5/docs/_static/glances-influxdb.png`

 * *Files identical despite different names*

### Comparing `glances-4.0.4/docs/_static/glances-memory-profiling-with-history.png` & `glances-4.0.5/docs/_static/glances-memory-profiling-with-history.png`

 * *Files identical despite different names*

### Comparing `glances-4.0.4/docs/_static/glances-memory-profiling-without-history.png` & `glances-4.0.5/docs/_static/glances-memory-profiling-without-history.png`

 * *Files identical despite different names*

### Comparing `glances-4.0.4/docs/_static/glances-pyinstrument.html` & `glances-4.0.5/docs/_static/glances-pyinstrument.html`

 * *Files identical despite different names*

### Comparing `glances-4.0.4/docs/_static/glances-responsive-webdesign.png` & `glances-4.0.5/docs/_static/glances-responsive-webdesign.png`

 * *Files identical despite different names*

### Comparing `glances-4.0.4/docs/_static/glances-summary.png` & `glances-4.0.5/docs/_static/glances-summary.png`

 * *Files identical despite different names*

### Comparing `glances-4.0.4/docs/_static/gpu.png` & `glances-4.0.5/docs/_static/gpu.png`

 * *Files identical despite different names*

### Comparing `glances-4.0.4/docs/_static/grafana.png` & `glances-4.0.5/docs/_static/grafana.png`

 * *Files identical despite different names*

### Comparing `glances-4.0.4/docs/_static/graph-load.svg` & `glances-4.0.5/docs/_static/graph-load.svg`

 * *Files identical despite different names*

### Comparing `glances-4.0.4/docs/_static/hddtemp.png` & `glances-4.0.5/docs/_static/hddtemp.png`

 * *Files identical despite different names*

### Comparing `glances-4.0.4/docs/_static/header.png` & `glances-4.0.5/docs/_static/header.png`

 * *Files identical despite different names*

### Comparing `glances-4.0.4/docs/_static/ip.png` & `glances-4.0.5/docs/_static/ip.png`

 * *Files identical despite different names*

### Comparing `glances-4.0.4/docs/_static/irq.png` & `glances-4.0.5/docs/_static/irq.png`

 * *Files identical despite different names*

### Comparing `glances-4.0.4/docs/_static/load.png` & `glances-4.0.5/docs/_static/load.png`

 * *Files identical despite different names*

### Comparing `glances-4.0.4/docs/_static/loadpercent.png` & `glances-4.0.5/docs/_static/loadpercent.png`

 * *Files identical despite different names*

### Comparing `glances-4.0.4/docs/_static/mem-wide.png` & `glances-4.0.5/docs/_static/mem-wide.png`

 * *Files identical despite different names*

### Comparing `glances-4.0.4/docs/_static/mem.png` & `glances-4.0.5/docs/_static/mem.png`

 * *Files identical despite different names*

### Comparing `glances-4.0.4/docs/_static/monitored.png` & `glances-4.0.5/docs/_static/monitored.png`

 * *Files identical despite different names*

### Comparing `glances-4.0.4/docs/_static/network.png` & `glances-4.0.5/docs/_static/network.png`

 * *Files identical despite different names*

### Comparing `glances-4.0.4/docs/_static/per-cpu.png` & `glances-4.0.5/docs/_static/per-cpu.png`

 * *Files identical despite different names*

### Comparing `glances-4.0.4/docs/_static/pergpu.png` & `glances-4.0.5/docs/_static/pergpu.png`

 * *Files identical despite different names*

### Comparing `glances-4.0.4/docs/_static/ports.png` & `glances-4.0.5/docs/_static/ports.png`

 * *Files identical despite different names*

### Comparing `glances-4.0.4/docs/_static/processlist-extended.png` & `glances-4.0.5/docs/_static/processlist-extended.png`

 * *Files identical despite different names*

### Comparing `glances-4.0.4/docs/_static/processlist-filter.png` & `glances-4.0.5/docs/_static/processlist-filter.png`

 * *Files identical despite different names*

### Comparing `glances-4.0.4/docs/_static/processlist-top.png` & `glances-4.0.5/docs/_static/processlist-top.png`

 * *Files identical despite different names*

### Comparing `glances-4.0.4/docs/_static/processlist-wide.png` & `glances-4.0.5/docs/_static/processlist-wide.png`

 * *Files identical despite different names*

### Comparing `glances-4.0.4/docs/_static/processlist.png` & `glances-4.0.5/docs/_static/processlist.png`

 * *Files identical despite different names*

### Comparing `glances-4.0.4/docs/_static/prometheus_exporter.png` & `glances-4.0.5/docs/_static/prometheus_exporter.png`

 * *Files identical despite different names*

### Comparing `glances-4.0.4/docs/_static/prometheus_server.png` & `glances-4.0.5/docs/_static/prometheus_server.png`

 * *Files identical despite different names*

### Comparing `glances-4.0.4/docs/_static/quicklook-percpu.png` & `glances-4.0.5/docs/_static/quicklook-percpu.png`

 * *Files identical despite different names*

### Comparing `glances-4.0.4/docs/_static/quicklook.png` & `glances-4.0.5/docs/_static/quicklook.png`

 * *Files identical despite different names*

### Comparing `glances-4.0.4/docs/_static/raid.png` & `glances-4.0.5/docs/_static/raid.png`

 * *Files identical despite different names*

### Comparing `glances-4.0.4/docs/_static/reddit.png` & `glances-4.0.5/docs/_static/reddit.png`

 * *Files identical despite different names*

### Comparing `glances-4.0.4/docs/_static/screencast.gif` & `glances-4.0.5/docs/_static/screencast.gif`

 * *Files identical despite different names*

### Comparing `glances-4.0.4/docs/_static/screenshot-web.png` & `glances-4.0.5/docs/_static/screenshot-web.png`

 * *Files identical despite different names*

### Comparing `glances-4.0.4/docs/_static/screenshot-web2.png` & `glances-4.0.5/docs/_static/screenshot-web2.png`

 * *Files identical despite different names*

### Comparing `glances-4.0.4/docs/_static/screenshot-wide.png` & `glances-4.0.5/docs/_static/screenshot-wide.png`

 * *Files identical despite different names*

### Comparing `glances-4.0.4/docs/_static/screenshot.png` & `glances-4.0.5/docs/_static/screenshot.png`

 * *Files identical despite different names*

### Comparing `glances-4.0.4/docs/_static/sensors.png` & `glances-4.0.5/docs/_static/sensors.png`

 * *Files identical despite different names*

### Comparing `glances-4.0.4/docs/_static/smart.png` & `glances-4.0.5/docs/_static/smart.png`

 * *Files identical despite different names*

### Comparing `glances-4.0.4/docs/_static/sparkline.png` & `glances-4.0.5/docs/_static/sparkline.png`

 * *Files identical despite different names*

### Comparing `glances-4.0.4/docs/_static/trend.png` & `glances-4.0.5/docs/_static/trend.png`

 * *Files identical despite different names*

### Comparing `glances-4.0.4/docs/_static/twitter-icon.png` & `glances-4.0.5/docs/_static/twitter-icon.png`

 * *Files identical despite different names*

### Comparing `glances-4.0.4/docs/_static/wifi.png` & `glances-4.0.5/docs/_static/wifi.png`

 * *Files identical despite different names*

### Comparing `glances-4.0.4/docs/aoa/actions.rst` & `glances-4.0.5/docs/aoa/actions.rst`

 * *Files identical despite different names*

### Comparing `glances-4.0.4/docs/aoa/amps.rst` & `glances-4.0.5/docs/aoa/amps.rst`

 * *Files identical despite different names*

### Comparing `glances-4.0.4/docs/aoa/connections.rst` & `glances-4.0.5/docs/aoa/connections.rst`

 * *Files identical despite different names*

### Comparing `glances-4.0.4/docs/aoa/containers.rst` & `glances-4.0.5/docs/aoa/containers.rst`

 * *Files identical despite different names*

### Comparing `glances-4.0.4/docs/aoa/cpu.rst` & `glances-4.0.5/docs/aoa/cpu.rst`

 * *Files identical despite different names*

### Comparing `glances-4.0.4/docs/aoa/diskio.rst` & `glances-4.0.5/docs/aoa/diskio.rst`

 * *Files identical despite different names*

### Comparing `glances-4.0.4/docs/aoa/events.rst` & `glances-4.0.5/docs/aoa/events.rst`

 * *Files identical despite different names*

### Comparing `glances-4.0.4/docs/aoa/folders.rst` & `glances-4.0.5/docs/aoa/folders.rst`

 * *Files identical despite different names*

### Comparing `glances-4.0.4/docs/aoa/fs.rst` & `glances-4.0.5/docs/aoa/fs.rst`

 * *Files identical despite different names*

### Comparing `glances-4.0.4/docs/aoa/gpu.rst` & `glances-4.0.5/docs/aoa/gpu.rst`

 * *Files identical despite different names*

### Comparing `glances-4.0.4/docs/aoa/hddtemp.rst` & `glances-4.0.5/docs/aoa/hddtemp.rst`

 * *Files identical despite different names*

### Comparing `glances-4.0.4/docs/aoa/header.rst` & `glances-4.0.5/docs/aoa/header.rst`

 * *Files identical despite different names*

### Comparing `glances-4.0.4/docs/aoa/index.rst` & `glances-4.0.5/docs/aoa/index.rst`

 * *Files identical despite different names*

### Comparing `glances-4.0.4/docs/aoa/irq.rst` & `glances-4.0.5/docs/aoa/irq.rst`

 * *Files identical despite different names*

### Comparing `glances-4.0.4/docs/aoa/load.rst` & `glances-4.0.5/docs/aoa/load.rst`

 * *Files identical despite different names*

### Comparing `glances-4.0.4/docs/aoa/memory.rst` & `glances-4.0.5/docs/aoa/memory.rst`

 * *Files identical despite different names*

### Comparing `glances-4.0.4/docs/aoa/network.rst` & `glances-4.0.5/docs/aoa/network.rst`

 * *Files identical despite different names*

### Comparing `glances-4.0.4/docs/aoa/ports.rst` & `glances-4.0.5/docs/aoa/ports.rst`

 * *Files identical despite different names*

### Comparing `glances-4.0.4/docs/aoa/ps.rst` & `glances-4.0.5/docs/aoa/ps.rst`

 * *Files identical despite different names*

### Comparing `glances-4.0.4/docs/aoa/quicklook.rst` & `glances-4.0.5/docs/aoa/quicklook.rst`

 * *Files identical despite different names*

### Comparing `glances-4.0.4/docs/aoa/sensors.rst` & `glances-4.0.5/docs/aoa/sensors.rst`

 * *Files identical despite different names*

### Comparing `glances-4.0.4/docs/aoa/smart.rst` & `glances-4.0.5/docs/aoa/smart.rst`

 * *Files identical despite different names*

### Comparing `glances-4.0.4/docs/aoa/wifi.rst` & `glances-4.0.5/docs/aoa/wifi.rst`

 * *Files identical despite different names*

### Comparing `glances-4.0.4/docs/api.rst` & `glances-4.0.5/docs/api.rst`

 * *Files 8% similar despite different names*

```diff
@@ -137,24 +137,24 @@
       "countmax": None,
       "countmin": 1.0,
       "key": "name",
       "name": "Dropbox",
       "refresh": 3.0,
       "regex": True,
       "result": None,
-      "timer": 1.4603652954101562},
+      "timer": 0.1488208770751953},
      {"count": 0,
       "countmax": 20.0,
       "countmin": None,
       "key": "name",
       "name": "Python",
       "refresh": 3.0,
       "regex": True,
       "result": None,
-      "timer": 1.4599840641021729}]
+      "timer": 0.14876770973205566}]
 
 Fields descriptions:
 
 * **name**: AMP name (unit is *None*)
 * **result**: AMP result (a string) (unit is *None*)
 * **refresh**: AMP refresh interval (unit is *second*)
 * **timer**: Time until next refresh (unit is *second*)
@@ -174,15 +174,15 @@
                   "countmax": None,
                   "countmin": 1.0,
                   "key": "name",
                   "name": "Dropbox",
                   "refresh": 3.0,
                   "regex": True,
                   "result": None,
-                  "timer": 1.4603652954101562}]}
+                  "timer": 0.1488208770751953}]}
 
 GET cloud
 ---------
 
 Get plugin stats::
 
     # curl http://localhost:61208/api/4/cloud
@@ -215,29 +215,15 @@
 
 GET containers
 --------------
 
 Get plugin stats::
 
     # curl http://localhost:61208/api/4/containers
-    [{"command": "/portainer",
-      "cpu": {"total": 0.0},
-      "cpu_percent": 0.0,
-      "created": "2022-10-29T14:59:10.266701439Z",
-      "engine": "docker",
-      "id": "3abd51c615968482d9ccff5afc629f267f6dda113ed68b75b432615fae3b49fb",
-      "image": ["portainer/portainer-ce:2.9.3"],
-      "io": {"cumulative_ior": 28909568, "cumulative_iow": 593920},
-      "key": "name",
-      "memory": {"inactive_file": 13643776, "limit": 7823511552, "usage": 33411072},
-      "memory_usage": 33411072,
-      "name": "portainer",
-      "network": {"cumulative_rx": 165757, "cumulative_tx": 0},
-      "status": "running",
-      "uptime": "39 mins"}]
+    []
 
 Fields descriptions:
 
 * **name**: Container name (unit is *None*)
 * **id**: Container ID (unit is *None*)
 * **image**: Container image (unit is *None*)
 * **status**: Container status (unit is *None*)
@@ -250,77 +236,51 @@
 * **network_rx**: Container network RX bitrate (unit is *bitpersecond*)
 * **network_tx**: Container network TX bitrate (unit is *bitpersecond*)
 * **uptime**: Container uptime (unit is *None*)
 * **engine**: Container engine (Docker and Podman are currently supported) (unit is *None*)
 * **pod_name**: Pod name (only with Podman) (unit is *None*)
 * **pod_id**: Pod ID (only with Podman) (unit is *None*)
 
-Get a specific field::
-
-    # curl http://localhost:61208/api/4/containers/name
-    {"name": ["portainer"]}
-
-Get a specific item when field matches the given value::
-
-    # curl http://localhost:61208/api/4/containers/name/portainer
-    {"portainer": [{"command": "/portainer",
-                    "cpu": {"total": 0.0},
-                    "cpu_percent": 0.0,
-                    "created": "2022-10-29T14:59:10.266701439Z",
-                    "engine": "docker",
-                    "id": "3abd51c615968482d9ccff5afc629f267f6dda113ed68b75b432615fae3b49fb",
-                    "image": ["portainer/portainer-ce:2.9.3"],
-                    "io": {"cumulative_ior": 28909568, "cumulative_iow": 593920},
-                    "key": "name",
-                    "memory": {"inactive_file": 13643776,
-                               "limit": 7823511552,
-                               "usage": 33411072},
-                    "memory_usage": 33411072,
-                    "name": "portainer",
-                    "network": {"cumulative_rx": 165757, "cumulative_tx": 0},
-                    "status": "running",
-                    "uptime": "39 mins"}]}
-
 GET core
 --------
 
 Get plugin stats::
 
     # curl http://localhost:61208/api/4/core
-    {"log": 4, "phys": 2}
+    {"log": 16, "phys": 10}
 
 Fields descriptions:
 
 * **phys**: Number of physical cores (hyper thread CPUs are excluded) (unit is *number*)
 * **log**: Number of logical CPU cores. A logical CPU is the number of physical cores multiplied by the number of threads that can run on each core (unit is *number*)
 
 Get a specific field::
 
     # curl http://localhost:61208/api/4/core/phys
-    {"phys": 2}
+    {"phys": 10}
 
 GET cpu
 -------
 
 Get plugin stats::
 
     # curl http://localhost:61208/api/4/cpu
-    {"cpucore": 4,
-     "ctx_switches": 9640228,
+    {"cpucore": 16,
+     "ctx_switches": 26785017,
      "guest": 0.0,
-     "idle": 0.0,
-     "interrupts": 4408812,
+     "idle": 1.0,
+     "interrupts": 31606155,
      "iowait": 0.0,
      "irq": 0.0,
      "nice": 0.0,
-     "soft_interrupts": 2938886,
+     "soft_interrupts": 7987786,
      "steal": 0.0,
      "syscalls": 0,
      "system": 0.0,
-     "total": 33.3,
+     "total": 0.0,
      "user": 0.0}
 
 Fields descriptions:
 
 * **total**: Sum of all CPU percentages (except idle) (unit is *percent*)
 * **system**: Percent time spent in kernel space. System CPU time is the time spent running code in the Operating System kernel (unit is *percent*)
 * **user**: CPU percent time spent in user space. User CPU time is the time spent on the processor running your program's code (or code in libraries) (unit is *percent*)
@@ -346,34 +306,34 @@
 * **cpucore**: Total number of CPU core (unit is *number*)
 * **time_since_update**: Number of seconds since last update (unit is *seconds*)
 * **time_since_update**: Number of seconds since last update (unit is *seconds*)
 
 Get a specific field::
 
     # curl http://localhost:61208/api/4/cpu/total
-    {"total": 33.3}
+    {"total": 0.0}
 
 GET diskio
 ----------
 
 Get plugin stats::
 
     # curl http://localhost:61208/api/4/diskio
-    [{"disk_name": "sda",
+    [{"disk_name": "nvme0n1",
       "key": "disk_name",
-      "read_bytes": 4421953024,
-      "read_count": 193359,
-      "write_bytes": 3038687232,
-      "write_count": 55949},
-     {"disk_name": "sda1",
+      "read_bytes": 3989510656,
+      "read_count": 136457,
+      "write_bytes": 4117681152,
+      "write_count": 166108},
+     {"disk_name": "nvme0n1p1",
       "key": "disk_name",
-      "read_bytes": 3551232,
-      "read_count": 107,
-      "write_bytes": 0,
-      "write_count": 11}]
+      "read_bytes": 7476224,
+      "read_count": 576,
+      "write_bytes": 1024,
+      "write_count": 2}]
 
 Fields descriptions:
 
 * **disk_name**: Disk name (unit is *None*)
 * **read_count**: Number of reads (unit is *number*)
 * **read_count_rate_per_sec**: Number of reads per second (unit is *number* per second)
 * **read_count_gauge**: Number of reads (cumulative) (unit is *number*)
@@ -387,25 +347,30 @@
 * **write_bytes_rate_per_sec**: Number of bytes written per second (unit is *byte* per second)
 * **write_bytes_gauge**: Number of bytes written (cumulative) (unit is *byte*)
 * **time_since_update**: Number of seconds since last update (unit is *seconds*)
 
 Get a specific field::
 
     # curl http://localhost:61208/api/4/diskio/disk_name
-    {"disk_name": ["sda", "sda1", "sda2", "sda5", "dm-0", "dm-1"]}
+    {"disk_name": ["nvme0n1",
+                   "nvme0n1p1",
+                   "nvme0n1p2",
+                   "nvme0n1p3",
+                   "dm-0",
+                   "dm-1"]}
 
 Get a specific item when field matches the given value::
 
-    # curl http://localhost:61208/api/4/diskio/disk_name/sda
-    {"sda": [{"disk_name": "sda",
-              "key": "disk_name",
-              "read_bytes": 4421953024,
-              "read_count": 193359,
-              "write_bytes": 3038687232,
-              "write_count": 55949}]}
+    # curl http://localhost:61208/api/4/diskio/disk_name/nvme0n1
+    {"nvme0n1": [{"disk_name": "nvme0n1",
+                  "key": "disk_name",
+                  "read_bytes": 3989510656,
+                  "read_count": 136457,
+                  "write_bytes": 4117681152,
+                  "write_count": 166108}]}
 
 GET folders
 -----------
 
 Get plugin stats::
 
     # curl http://localhost:61208/api/4/folders
@@ -423,113 +388,83 @@
 
 GET fs
 ------
 
 Get plugin stats::
 
     # curl http://localhost:61208/api/4/fs
-    [{"device_name": "/dev/mapper/ubuntu--gnome--vg-root",
-      "free": 117916065792,
+    [{"device_name": "/dev/mapper/ubuntu--vg-ubuntu--lv",
+      "free": 905288650752,
       "fs_type": "ext4",
       "key": "mnt_point",
       "mnt_point": "/",
-      "percent": 48.9,
-      "size": 243334156288,
-      "used": 113030635520},
-     {"device_name": "zsfpool",
-      "free": 31195136,
-      "fs_type": "zfs",
-      "key": "mnt_point",
-      "mnt_point": "/zsfpool",
-      "percent": 25.4,
-      "size": 41811968,
-      "used": 10616832}]
+      "percent": 5.0,
+      "size": 1003736440832,
+      "used": 47385284608}]
 
 Fields descriptions:
 
 * **device_name**: Device name (unit is *None*)
 * **fs_type**: File system type (unit is *None*)
 * **mnt_point**: Mount point (unit is *None*)
 * **size**: Total size (unit is *byte*)
 * **used**: Used size (unit is *byte*)
 * **free**: Free size (unit is *byte*)
 * **percent**: File system usage in percent (unit is *percent*)
 
 Get a specific field::
 
     # curl http://localhost:61208/api/4/fs/mnt_point
-    {"mnt_point": ["/", "/zsfpool"]}
+    {"mnt_point": ["/"]}
 
 Get a specific item when field matches the given value::
 
     # curl http://localhost:61208/api/4/fs/mnt_point//
-    {"/": [{"device_name": "/dev/mapper/ubuntu--gnome--vg-root",
-            "free": 117916065792,
+    {"/": [{"device_name": "/dev/mapper/ubuntu--vg-ubuntu--lv",
+            "free": 905288650752,
             "fs_type": "ext4",
             "key": "mnt_point",
             "mnt_point": "/",
-            "percent": 48.9,
-            "size": 243334156288,
-            "used": 113030635520}]}
+            "percent": 5.0,
+            "size": 1003736440832,
+            "used": 47385284608}]}
 
 GET gpu
 -------
 
 Get plugin stats::
 
     # curl http://localhost:61208/api/4/gpu
-    [{"fan_speed": 29,
-      "gpu_id": "nvidia0",
-      "key": "gpu_id",
-      "mem": 46.144612630208336,
-      "name": "NVIDIA GeForce GTX 1060 3GB",
-      "proc": 2,
-      "temperature": 57}]
+    []
 
 Fields descriptions:
 
 * **gpu_id**: GPU identification (unit is *None*)
 * **name**: GPU name (unit is *None*)
 * **mem**: Memory consumption (unit is *percent*)
 * **proc**: GPU processor consumption (unit is *percent*)
 * **temperature**: GPU temperature (unit is *celsius*)
 * **fan_speed**: GPU fan speed (unit is *roundperminute*)
 
-Get a specific field::
-
-    # curl http://localhost:61208/api/4/gpu/gpu_id
-    {"gpu_id": ["nvidia0"]}
-
-Get a specific item when field matches the given value::
-
-    # curl http://localhost:61208/api/4/gpu/gpu_id/nvidia0
-    {"nvidia0": [{"fan_speed": 29,
-                  "gpu_id": "nvidia0",
-                  "key": "gpu_id",
-                  "mem": 46.144612630208336,
-                  "name": "NVIDIA GeForce GTX 1060 3GB",
-                  "proc": 2,
-                  "temperature": 57}]}
-
 GET help
 --------
 
 Get plugin stats::
 
     # curl http://localhost:61208/api/4/help
     None
 
 GET ip
 ------
 
 Get plugin stats::
 
     # curl http://localhost:61208/api/4/ip
-    {"address": "192.168.0.32",
-     "gateway": "192.168.0.254",
+    {"address": "192.168.1.26",
+     "gateway": "192.168.1.1",
      "mask": "255.255.255.0",
      "mask_cidr": 24,
      "public_address": "",
      "public_info_human": ""}
 
 Fields descriptions:
 
@@ -539,15 +474,15 @@
 * **gateway**: Private IP gateway (unit is *None*)
 * **public_address**: Public IP address (unit is *None*)
 * **public_info_human**: Public IP information (unit is *None*)
 
 Get a specific field::
 
     # curl http://localhost:61208/api/4/ip/gateway
-    {"gateway": "192.168.0.254"}
+    {"gateway": "192.168.1.1"}
 
 GET irq
 -------
 
 Get plugin stats::
 
     # curl http://localhost:61208/api/4/irq
@@ -560,47 +495,44 @@
 
 GET load
 --------
 
 Get plugin stats::
 
     # curl http://localhost:61208/api/4/load
-    {"cpucore": 4,
-     "min1": 2.2197265625,
-     "min15": 2.08154296875,
-     "min5": 2.44287109375}
+    {"cpucore": 16, "min1": 0.748046875, "min15": 0.57373046875, "min5": 0.7265625}
 
 Fields descriptions:
 
 * **min1**: Average sum of the number of processes waiting in the run-queue plus the number currently executing over 1 minute (unit is *float*)
 * **min5**: Average sum of the number of processes waiting in the run-queue plus the number currently executing over 5 minutes (unit is *float*)
 * **min15**: Average sum of the number of processes waiting in the run-queue plus the number currently executing over 15 minutes (unit is *float*)
 * **cpucore**: Total number of CPU core (unit is *number*)
 
 Get a specific field::
 
     # curl http://localhost:61208/api/4/load/min1
-    {"min1": 2.2197265625}
+    {"min1": 0.748046875}
 
 GET mem
 -------
 
 Get plugin stats::
 
     # curl http://localhost:61208/api/4/mem
-    {"active": 2232004608,
-     "available": 3969384448,
-     "buffers": 600408064,
-     "cached": 3533656064,
-     "free": 3969384448,
-     "inactive": 4194328576,
-     "percent": 49.3,
-     "shared": 349536256,
-     "total": 7823511552,
-     "used": 3854127104}
+    {"active": 5833261056,
+     "available": 10653102080,
+     "buffers": 250515456,
+     "cached": 5880537088,
+     "free": 10653102080,
+     "inactive": 3567583232,
+     "percent": 35.1,
+     "shared": 705511424,
+     "total": 16422486016,
+     "used": 5769383936}
 
 Fields descriptions:
 
 * **total**: Total physical memory available (unit is *bytes*)
 * **available**: The actual amount of available memory that can be given instantly to processes that request more memory in bytes; this is calculated by summing different memory values depending on the platform (e.g. free + buffers + cached on Linux) and it is supposed to be used to monitor actual memory usage in a cross platform fashion (unit is *bytes*)
 * **percent**: The percentage usage calculated as (total - available) / total * 100 (unit is *percent*)
 * **used**: Memory used, calculated differently depending on the platform and designed for informational purposes only (unit is *bytes*)
@@ -611,73 +543,62 @@
 * **cached**: *(Linux, BSD)*: cache for various things (unit is *bytes*)
 * **wired**: *(BSD, macOS)*: memory that is marked to always stay in RAM. It is never moved to disk (unit is *bytes*)
 * **shared**: *(BSD)*: memory that may be simultaneously accessed by multiple processes (unit is *bytes*)
 
 Get a specific field::
 
     # curl http://localhost:61208/api/4/mem/total
-    {"total": 7823511552}
+    {"total": 16422486016}
 
 GET memswap
 -----------
 
 Get plugin stats::
 
     # curl http://localhost:61208/api/4/memswap
-    {"free": 8070361088,
-     "percent": 0.1,
-     "sin": 180224,
-     "sout": 11976704,
+    {"free": 4294963200,
+     "percent": 0.0,
+     "sin": 0,
+     "sout": 0,
      "time_since_update": 1,
-     "total": 8082419712,
-     "used": 12058624}
+     "total": 4294963200,
+     "used": 0}
 
 Fields descriptions:
 
 * **total**: Total swap memory (unit is *bytes*)
 * **used**: Used swap memory (unit is *bytes*)
 * **free**: Free swap memory (unit is *bytes*)
 * **percent**: Used swap memory in percentage (unit is *percent*)
 * **sin**: The number of bytes the system has swapped in from disk (cumulative) (unit is *bytes*)
 * **sout**: The number of bytes the system has swapped out from disk (cumulative) (unit is *bytes*)
 * **time_since_update**: Number of seconds since last update (unit is *seconds*)
 
 Get a specific field::
 
     # curl http://localhost:61208/api/4/memswap/total
-    {"total": 8082419712}
+    {"total": 4294963200}
 
 GET network
 -----------
 
 Get plugin stats::
 
     # curl http://localhost:61208/api/4/network
     [{"alias": None,
       "bytes_all": 0,
-      "bytes_all_gauge": 233342069,
+      "bytes_all_gauge": 451852439,
       "bytes_recv": 0,
-      "bytes_recv_gauge": 216683314,
+      "bytes_recv_gauge": 428042038,
       "bytes_sent": 0,
-      "bytes_sent_gauge": 16658755,
-      "interface_name": "wlp2s0",
+      "bytes_sent_gauge": 23810401,
+      "interface_name": "wlp0s20f3",
       "key": "interface_name",
       "speed": 0,
-      "time_since_update": 1.0833158493041992},
-     {"alias": None,
-      "bytes_all": 0,
-      "bytes_all_gauge": 165757,
-      "bytes_recv": 0,
-      "bytes_recv_gauge": 0,
-      "bytes_sent": 0,
-      "bytes_sent_gauge": 165757,
-      "interface_name": "veth1d38654",
-      "key": "interface_name",
-      "speed": 10485760000,
-      "time_since_update": 1.0833158493041992}]
+      "time_since_update": 0.15277767181396484}]
 
 Fields descriptions:
 
 * **interface_name**: Interface name (unit is *None*)
 * **alias**: Interface alias name (optional) (unit is *None*)
 * **bytes_recv**: Number of bytes received (unit is *byte*)
 * **bytes_recv_rate_per_sec**: Number of bytes received per second (unit is *byte* per second)
@@ -691,85 +612,80 @@
 * **speed**: Maximum interface speed (in bit per second). Can return 0 on some operating-system (unit is *bitpersecond*)
 * **is_up**: Is the interface up ? (unit is *bool*)
 * **time_since_update**: Number of seconds since last update (unit is *seconds*)
 
 Get a specific field::
 
     # curl http://localhost:61208/api/4/network/interface_name
-    {"interface_name": ["wlp2s0",
-                        "veth1d38654",
-                        "mpqemubr0",
-                        "lxdbr0",
-                        "veth377a0b53",
-                        "veth9a7e77b5"]}
+    {"interface_name": ["wlp0s20f3"]}
 
 Get a specific item when field matches the given value::
 
-    # curl http://localhost:61208/api/4/network/interface_name/wlp2s0
-    {"wlp2s0": [{"alias": None,
-                 "bytes_all": 0,
-                 "bytes_all_gauge": 233342069,
-                 "bytes_recv": 0,
-                 "bytes_recv_gauge": 216683314,
-                 "bytes_sent": 0,
-                 "bytes_sent_gauge": 16658755,
-                 "interface_name": "wlp2s0",
-                 "key": "interface_name",
-                 "speed": 0,
-                 "time_since_update": 1.0833158493041992}]}
+    # curl http://localhost:61208/api/4/network/interface_name/wlp0s20f3
+    {"wlp0s20f3": [{"alias": None,
+                    "bytes_all": 0,
+                    "bytes_all_gauge": 451852439,
+                    "bytes_recv": 0,
+                    "bytes_recv_gauge": 428042038,
+                    "bytes_sent": 0,
+                    "bytes_sent_gauge": 23810401,
+                    "interface_name": "wlp0s20f3",
+                    "key": "interface_name",
+                    "speed": 0,
+                    "time_since_update": 0.15277767181396484}]}
 
 GET now
 -------
 
 Get plugin stats::
 
     # curl http://localhost:61208/api/4/now
-    {"custom": "2024-05-14 01:49:24 IST", "iso": "2024-05-14T01:49:24+05:30"}
+    {"custom": "2024-05-18 11:03:48 CEST", "iso": "2024-05-18T11:03:48+02:00"}
 
 Fields descriptions:
 
 * **custom**: Current date in custom format (unit is *None*)
 * **iso**: Current date in ISO 8601 format (unit is *None*)
 
 Get a specific field::
 
     # curl http://localhost:61208/api/4/now/iso
-    {"iso": "2024-05-14T01:49:24+05:30"}
+    {"iso": "2024-05-18T11:03:48+02:00"}
 
 GET percpu
 ----------
 
 Get plugin stats::
 
     # curl http://localhost:61208/api/4/percpu
     [{"cpu_number": 0,
       "guest": 0.0,
       "guest_nice": 0.0,
-      "idle": 0.0,
+      "idle": 1.0,
       "iowait": 0.0,
       "irq": 0.0,
       "key": "cpu_number",
       "nice": 0.0,
       "softirq": 0.0,
       "steal": 0.0,
       "system": 0.0,
-      "total": 100.0,
+      "total": 99.0,
       "user": 0.0},
      {"cpu_number": 1,
       "guest": 0.0,
       "guest_nice": 0.0,
-      "idle": 1.0,
+      "idle": 0.0,
       "iowait": 0.0,
       "irq": 0.0,
       "key": "cpu_number",
       "nice": 0.0,
       "softirq": 0.0,
       "steal": 0.0,
       "system": 0.0,
-      "total": 99.0,
+      "total": 100.0,
       "user": 0.0}]
 
 Fields descriptions:
 
 * **cpu_number**: CPU number (unit is *None*)
 * **total**: Sum of CPU percentages (except idle) for current CPU number (unit is *percent*)
 * **system**: Percent time spent in kernel space. System CPU time is the time spent running code in the Operating System kernel (unit is *percent*)
@@ -782,29 +698,29 @@
 * **guest**: *(Linux)*: percent of time spent running a virtual CPU for guest operating systems under the control of the Linux kernel (unit is *percent*)
 * **guest_nice**: *(Linux)*: percent of time spent running a niced guest (virtual CPU) (unit is *percent*)
 * **softirq**: *(Linux)*: percent of time spent handling software interrupts (unit is *percent*)
 
 Get a specific field::
 
     # curl http://localhost:61208/api/4/percpu/cpu_number
-    {"cpu_number": [0, 1, 2, 3]}
+    {"cpu_number": [0, 1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12, 13, 14, 15]}
 
 GET ports
 ---------
 
 Get plugin stats::
 
     # curl http://localhost:61208/api/4/ports
     [{"description": "DefaultGateway",
-      "host": "192.168.0.254",
+      "host": "192.168.1.1",
       "indice": "port_0",
       "port": 0,
       "refresh": 30,
       "rtt_warning": None,
-      "status": 0.012202,
+      "status": 0.004889,
       "timeout": 3}]
 
 Fields descriptions:
 
 * **host**: Measurement is be done on this host (or IP address) (unit is *None*)
 * **port**: Measurement is be done on this port (0 for ICMP) (unit is *None*)
 * **description**: Human readable description for the host/port (unit is *None*)
@@ -813,48 +729,48 @@
 * **status**: Measurement result (in seconds) (unit is *second*)
 * **rtt_warning**: Warning threshold (in seconds) for the measurement (unit is *second*)
 * **indice**: Unique indice for the host/port (unit is *None*)
 
 Get a specific field::
 
     # curl http://localhost:61208/api/4/ports/host
-    {"host": ["192.168.0.254"]}
+    {"host": ["192.168.1.1"]}
 
 Get a specific item when field matches the given value::
 
-    # curl http://localhost:61208/api/4/ports/host/192.168.0.254
-    {"192.168.0.254": [{"description": "DefaultGateway",
-                        "host": "192.168.0.254",
-                        "indice": "port_0",
-                        "port": 0,
-                        "refresh": 30,
-                        "rtt_warning": None,
-                        "status": 0.012202,
-                        "timeout": 3}]}
+    # curl http://localhost:61208/api/4/ports/host/192.168.1.1
+    {"192.168.1.1": [{"description": "DefaultGateway",
+                      "host": "192.168.1.1",
+                      "indice": "port_0",
+                      "port": 0,
+                      "refresh": 30,
+                      "rtt_warning": None,
+                      "status": 0.004889,
+                      "timeout": 3}]}
 
 GET processcount
 ----------------
 
 Get plugin stats::
 
     # curl http://localhost:61208/api/4/processcount
-    {"pid_max": 0, "running": 0, "sleeping": 303, "thread": 1250, "total": 373}
+    {"pid_max": 0, "running": 0, "sleeping": 276, "thread": 1568, "total": 407}
 
 Fields descriptions:
 
 * **total**: Total number of processes (unit is *number*)
 * **running**: Total number of running processes (unit is *number*)
 * **sleeping**: Total number of sleeping processes (unit is *number*)
 * **thread**: Total number of threads (unit is *number*)
 * **pid_max**: Maximum number of processes (unit is *number*)
 
 Get a specific field::
 
     # curl http://localhost:61208/api/4/processcount/total
-    {"total": 373}
+    {"total": 407}
 
 GET processlist
 ---------------
 
 Get plugin stats::
 
     # curl http://localhost:61208/api/4/processlist
@@ -886,75 +802,231 @@
 
 GET quicklook
 -------------
 
 Get plugin stats::
 
     # curl http://localhost:61208/api/4/quicklook
-    {"cpu": 33.3,
-     "cpu_hz": 3000000000.0,
-     "cpu_hz_current": 1348638750.0,
-     "cpu_log_core": 4,
-     "cpu_name": "Intel(R) Core(TM) i7-4500U CPU @ 1.80GHz",
-     "cpu_phys_core": 2,
-     "load": 52.0,
-     "mem": 49.3,
+    {"cpu": 0.0,
+     "cpu_hz": 4475000000.0,
+     "cpu_hz_current": 1871619687.4999998,
+     "cpu_log_core": 16,
+     "cpu_name": "13th Gen Intel(R) Core(TM) i7-13620H",
+     "cpu_phys_core": 10,
+     "load": 3.6,
+     "mem": 35.1,
      "percpu": [{"cpu_number": 0,
                  "guest": 0.0,
                  "guest_nice": 0.0,
+                 "idle": 1.0,
+                 "iowait": 0.0,
+                 "irq": 0.0,
+                 "key": "cpu_number",
+                 "nice": 0.0,
+                 "softirq": 0.0,
+                 "steal": 0.0,
+                 "system": 0.0,
+                 "total": 99.0,
+                 "user": 0.0},
+                {"cpu_number": 1,
+                 "guest": 0.0,
+                 "guest_nice": 0.0,
                  "idle": 0.0,
                  "iowait": 0.0,
                  "irq": 0.0,
                  "key": "cpu_number",
                  "nice": 0.0,
                  "softirq": 0.0,
                  "steal": 0.0,
                  "system": 0.0,
                  "total": 100.0,
                  "user": 0.0},
-                {"cpu_number": 1,
+                {"cpu_number": 2,
+                 "guest": 0.0,
+                 "guest_nice": 0.0,
+                 "idle": 0.0,
+                 "iowait": 0.0,
+                 "irq": 0.0,
+                 "key": "cpu_number",
+                 "nice": 0.0,
+                 "softirq": 0.0,
+                 "steal": 0.0,
+                 "system": 0.0,
+                 "total": 100.0,
+                 "user": 0.0},
+                {"cpu_number": 3,
+                 "guest": 0.0,
+                 "guest_nice": 0.0,
+                 "idle": 0.0,
+                 "iowait": 0.0,
+                 "irq": 0.0,
+                 "key": "cpu_number",
+                 "nice": 0.0,
+                 "softirq": 0.0,
+                 "steal": 0.0,
+                 "system": 0.0,
+                 "total": 100.0,
+                 "user": 0.0},
+                {"cpu_number": 4,
+                 "guest": 0.0,
+                 "guest_nice": 0.0,
+                 "idle": 0.0,
+                 "iowait": 0.0,
+                 "irq": 0.0,
+                 "key": "cpu_number",
+                 "nice": 0.0,
+                 "softirq": 0.0,
+                 "steal": 0.0,
+                 "system": 0.0,
+                 "total": 100.0,
+                 "user": 0.0},
+                {"cpu_number": 5,
                  "guest": 0.0,
                  "guest_nice": 0.0,
                  "idle": 1.0,
                  "iowait": 0.0,
                  "irq": 0.0,
                  "key": "cpu_number",
                  "nice": 0.0,
                  "softirq": 0.0,
                  "steal": 0.0,
                  "system": 0.0,
                  "total": 99.0,
                  "user": 0.0},
-                {"cpu_number": 2,
+                {"cpu_number": 6,
                  "guest": 0.0,
                  "guest_nice": 0.0,
                  "idle": 0.0,
                  "iowait": 0.0,
                  "irq": 0.0,
                  "key": "cpu_number",
                  "nice": 0.0,
                  "softirq": 0.0,
                  "steal": 0.0,
                  "system": 1.0,
                  "total": 100.0,
                  "user": 0.0},
-                {"cpu_number": 3,
+                {"cpu_number": 7,
+                 "guest": 0.0,
+                 "guest_nice": 0.0,
+                 "idle": 1.0,
+                 "iowait": 0.0,
+                 "irq": 0.0,
+                 "key": "cpu_number",
+                 "nice": 0.0,
+                 "softirq": 0.0,
+                 "steal": 0.0,
+                 "system": 0.0,
+                 "total": 99.0,
+                 "user": 0.0},
+                {"cpu_number": 8,
+                 "guest": 0.0,
+                 "guest_nice": 0.0,
+                 "idle": 1.0,
+                 "iowait": 0.0,
+                 "irq": 0.0,
+                 "key": "cpu_number",
+                 "nice": 0.0,
+                 "softirq": 0.0,
+                 "steal": 0.0,
+                 "system": 0.0,
+                 "total": 99.0,
+                 "user": 0.0},
+                {"cpu_number": 9,
+                 "guest": 0.0,
+                 "guest_nice": 0.0,
+                 "idle": 1.0,
+                 "iowait": 0.0,
+                 "irq": 0.0,
+                 "key": "cpu_number",
+                 "nice": 0.0,
+                 "softirq": 0.0,
+                 "steal": 0.0,
+                 "system": 0.0,
+                 "total": 99.0,
+                 "user": 0.0},
+                {"cpu_number": 10,
                  "guest": 0.0,
                  "guest_nice": 0.0,
                  "idle": 0.0,
                  "iowait": 0.0,
                  "irq": 0.0,
                  "key": "cpu_number",
                  "nice": 0.0,
                  "softirq": 0.0,
                  "steal": 0.0,
-                 "system": 1.0,
+                 "system": 0.0,
+                 "total": 100.0,
+                 "user": 0.0},
+                {"cpu_number": 11,
+                 "guest": 0.0,
+                 "guest_nice": 0.0,
+                 "idle": 1.0,
+                 "iowait": 0.0,
+                 "irq": 0.0,
+                 "key": "cpu_number",
+                 "nice": 0.0,
+                 "softirq": 0.0,
+                 "steal": 0.0,
+                 "system": 0.0,
+                 "total": 99.0,
+                 "user": 0.0},
+                {"cpu_number": 12,
+                 "guest": 0.0,
+                 "guest_nice": 0.0,
+                 "idle": 0.0,
+                 "iowait": 0.0,
+                 "irq": 0.0,
+                 "key": "cpu_number",
+                 "nice": 0.0,
+                 "softirq": 0.0,
+                 "steal": 0.0,
+                 "system": 0.0,
+                 "total": 100.0,
+                 "user": 0.0},
+                {"cpu_number": 13,
+                 "guest": 0.0,
+                 "guest_nice": 0.0,
+                 "idle": 0.0,
+                 "iowait": 0.0,
+                 "irq": 0.0,
+                 "key": "cpu_number",
+                 "nice": 0.0,
+                 "softirq": 0.0,
+                 "steal": 0.0,
+                 "system": 0.0,
+                 "total": 100.0,
+                 "user": 0.0},
+                {"cpu_number": 14,
+                 "guest": 0.0,
+                 "guest_nice": 0.0,
+                 "idle": 1.0,
+                 "iowait": 0.0,
+                 "irq": 0.0,
+                 "key": "cpu_number",
+                 "nice": 0.0,
+                 "softirq": 0.0,
+                 "steal": 0.0,
+                 "system": 0.0,
+                 "total": 99.0,
+                 "user": 0.0},
+                {"cpu_number": 15,
+                 "guest": 0.0,
+                 "guest_nice": 0.0,
+                 "idle": 0.0,
+                 "iowait": 0.0,
+                 "irq": 0.0,
+                 "key": "cpu_number",
+                 "nice": 0.0,
+                 "softirq": 0.0,
+                 "steal": 0.0,
+                 "system": 0.0,
                  "total": 100.0,
                  "user": 0.0}],
-     "swap": 0.1}
+     "swap": 0.0}
 
 Fields descriptions:
 
 * **cpu**: CPU percent usage (unit is *percent*)
 * **mem**: MEM percent usage (unit is *percent*)
 * **swap**: SWAP percent usage (unit is *percent*)
 * **load**: LOAD percent usage (unit is *percent*)
@@ -963,15 +1035,15 @@
 * **cpu_name**: CPU name (unit is *None*)
 * **cpu_hz_current**: CPU current frequency (unit is *hertz*)
 * **cpu_hz**: CPU max frequency (unit is *hertz*)
 
 Get a specific field::
 
     # curl http://localhost:61208/api/4/quicklook/cpu_name
-    {"cpu_name": "Intel(R) Core(TM) i7-4500U CPU @ 1.80GHz"}
+    {"cpu_name": "13th Gen Intel(R) Core(TM) i7-13620H"}
 
 GET raid
 --------
 
 Get plugin stats::
 
     # curl http://localhost:61208/api/4/raid
@@ -982,58 +1054,86 @@
 
 Get plugin stats::
 
     # curl http://localhost:61208/api/4/sensors
     [{"critical": None,
       "key": "label",
       "label": "Ambient",
-      "type": "temperature_core",
+      "type": "SensorType.CPU_TEMP",
       "unit": "C",
-      "value": 48,
-      "warning": None},
+      "value": 38,
+      "warning": 0},
      {"critical": None,
       "key": "label",
-      "label": "CPU",
-      "type": "temperature_core",
+      "label": "Ambient 3",
+      "type": "SensorType.CPU_TEMP",
       "unit": "C",
-      "value": 58,
-      "warning": None}]
+      "value": 33,
+      "warning": 0}]
 
 Fields descriptions:
 
 * **label**: Sensor label (unit is *None*)
 * **unit**: Sensor unit (unit is *None*)
 * **value**: Sensor value (unit is *number*)
 * **warning**: Warning threshold (unit is *number*)
 * **critical**: Critical threshold (unit is *number*)
 * **type**: Sensor type (one of battery, temperature_core, fan_speed) (unit is *None*)
 
 Get a specific field::
 
     # curl http://localhost:61208/api/4/sensors/label
     {"label": ["Ambient",
+               "Ambient 3",
+               "Ambient 5",
+               "Ambient 6",
                "CPU",
+               "Composite",
                "Core 0",
-               "Core 1",
+               "Core 12",
+               "Core 16",
+               "Core 20",
+               "Core 28",
+               "Core 29",
+               "Core 30",
+               "Core 31",
+               "Core 4",
+               "Core 8",
+               "HDD",
                "Package id 0",
                "SODIMM",
-               "acpitz 0",
-               "acpitz 1",
+               "Sensor 1",
+               "Sensor 2",
+               "dell_smm 0",
+               "dell_smm 1",
+               "dell_smm 2",
+               "dell_smm 3",
+               "dell_smm 4",
+               "dell_smm 5",
+               "dell_smm 6",
+               "dell_smm 7",
+               "dell_smm 8",
+               "dell_smm 9",
+               "iwlwifi_1 0",
+               "CPU Fan",
+               "Video Fan",
+               "dell_smm 0",
+               "dell_smm 1",
                "BAT BAT0"]}
 
 Get a specific item when field matches the given value::
 
     # curl http://localhost:61208/api/4/sensors/label/Ambient
     {"Ambient": [{"critical": None,
                   "key": "label",
                   "label": "Ambient",
-                  "type": "temperature_core",
+                  "type": "SensorType.CPU_TEMP",
                   "unit": "C",
-                  "value": 48,
-                  "warning": None}]}
+                  "value": 38,
+                  "warning": 0}]}
 
 GET smart
 ---------
 
 Get plugin stats::
 
     # curl http://localhost:61208/api/4/smart
@@ -1041,19 +1141,19 @@
 
 GET system
 ----------
 
 Get plugin stats::
 
     # curl http://localhost:61208/api/4/system
-    {"hostname": "XPS13-9333",
-     "hr_name": "Ubuntu 22.04 64bit / Linux 5.15.0-105-generic",
-     "linux_distro": "Ubuntu 22.04",
+    {"hostname": "nicolargo-xps15",
+     "hr_name": "Ubuntu 24.04 64bit / Linux 6.8.0-31-generic",
+     "linux_distro": "Ubuntu 24.04",
      "os_name": "Linux",
-     "os_version": "5.15.0-105-generic",
+     "os_version": "6.8.0-31-generic",
      "platform": "64bit"}
 
 Fields descriptions:
 
 * **os_name**: Operating system name (unit is *None*)
 * **hostname**: Hostname (unit is *None*)
 * **platform**: Platform (32 or 64 bits) (unit is *None*)
@@ -1068,47 +1168,47 @@
 
 GET uptime
 ----------
 
 Get plugin stats::
 
     # curl http://localhost:61208/api/4/uptime
-    "0:40:05"
+    "4 days, 11:56:37"
 
 GET version
 -----------
 
 Get plugin stats::
 
     # curl http://localhost:61208/api/4/version
-    "4.0.4"
+    "4.0.5"
 
 GET wifi
 --------
 
 Get plugin stats::
 
     # curl http://localhost:61208/api/4/wifi
     [{"key": "ssid",
-      "quality_level": -73.0,
-      "quality_link": 37.0,
-      "ssid": "wlp2s0"}]
+      "quality_level": -60.0,
+      "quality_link": 50.0,
+      "ssid": "wlp0s20f3"}]
 
 Get a specific field::
 
     # curl http://localhost:61208/api/4/wifi/ssid
-    {"ssid": ["wlp2s0"]}
+    {"ssid": ["wlp0s20f3"]}
 
 Get a specific item when field matches the given value::
 
-    # curl http://localhost:61208/api/4/wifi/ssid/wlp2s0
-    {"wlp2s0": [{"key": "ssid",
-                 "quality_level": -73.0,
-                 "quality_link": 37.0,
-                 "ssid": "wlp2s0"}]}
+    # curl http://localhost:61208/api/4/wifi/ssid/wlp0s20f3
+    {"wlp0s20f3": [{"key": "ssid",
+                    "quality_level": -60.0,
+                    "quality_link": 50.0,
+                    "ssid": "wlp0s20f3"}]}
 
 GET all stats
 -------------
 
 Get all Glances stats::
 
     # curl http://localhost:61208/api/4/all
@@ -1144,63 +1244,63 @@
 
 GET stats history
 -----------------
 
 History of a plugin::
 
     # curl http://localhost:61208/api/4/cpu/history
-    {"system": [["2024-05-12T19:00:53.344171", 0.0],
-                ["2024-05-12T19:00:54.388941", 0.0],
-                ["2024-05-12T19:00:55.807295", 0.0]],
-     "user": [["2024-05-12T19:00:53.344145", 0.0],
-              ["2024-05-12T19:00:54.388924", 0.0],
-              ["2024-05-12T19:00:55.807269", 0.0]]}
+    {"system": [["2024-05-18T11:03:49.609837", 0.0],
+                ["2024-05-18T11:03:50.653488", 1.0],
+                ["2024-05-18T11:03:51.701403", 1.0]],
+     "user": [["2024-05-18T11:03:49.609825", 0.0],
+              ["2024-05-18T11:03:50.653484", 0.0],
+              ["2024-05-18T11:03:51.701393", 0.0]]}
 
 Limit history to last 2 values::
 
     # curl http://localhost:61208/api/4/cpu/history/2
-    {"system": [["2024-05-12T19:00:54.388941", 0.0],
-                ["2024-05-12T19:00:55.807295", 0.0]],
-     "user": [["2024-05-12T19:00:54.388924", 0.0],
-              ["2024-05-12T19:00:55.807269", 0.0]]}
+    {"system": [["2024-05-18T11:03:50.653488", 1.0],
+                ["2024-05-18T11:03:51.701403", 1.0]],
+     "user": [["2024-05-18T11:03:50.653484", 0.0],
+              ["2024-05-18T11:03:51.701393", 0.0]]}
 
 History for a specific field::
 
     # curl http://localhost:61208/api/4/cpu/system/history
-    {"system": [["2024-05-12T19:00:51.692893", 0.0],
-                ["2024-05-12T19:00:53.344171", 0.0],
-                ["2024-05-12T19:00:54.388941", 0.0],
-                ["2024-05-12T19:00:55.807295", 0.0]]}
+    {"system": [["2024-05-18T11:03:48.519990", 0.0],
+                ["2024-05-18T11:03:49.609837", 0.0],
+                ["2024-05-18T11:03:50.653488", 1.0],
+                ["2024-05-18T11:03:51.701403", 1.0]]}
 
 Limit history for a specific field to last 2 values::
 
     # curl http://localhost:61208/api/4/cpu/system/history
-    {"system": [["2024-05-12T19:00:54.388941", 0.0],
-                ["2024-05-12T19:00:55.807295", 0.0]]}
+    {"system": [["2024-05-18T11:03:50.653488", 1.0],
+                ["2024-05-18T11:03:51.701403", 1.0]]}
 
 GET limits (used for thresholds)
 --------------------------------
 
 All limits/thresholds::
 
     # curl http://localhost:61208/api/4/all/limits
     {"alert": {"alert_disable": ["False"], "history_size": 1200.0},
      "amps": {"amps_disable": ["False"], "history_size": 1200.0},
      "containers": {"containers_all": ["False"],
                     "containers_disable": ["False"],
                     "containers_max_name_size": 20.0,
                     "history_size": 1200.0},
      "core": {"history_size": 1200.0},
-     "cpu": {"cpu_ctx_switches_careful": 160000.0,
-             "cpu_ctx_switches_critical": 200000.0,
-             "cpu_ctx_switches_warning": 180000.0,
+     "cpu": {"cpu_ctx_switches_careful": 640000.0,
+             "cpu_ctx_switches_critical": 800000.0,
+             "cpu_ctx_switches_warning": 720000.0,
              "cpu_disable": ["False"],
-             "cpu_iowait_careful": 20.0,
-             "cpu_iowait_critical": 25.0,
-             "cpu_iowait_warning": 22.5,
+             "cpu_iowait_careful": 5.0,
+             "cpu_iowait_critical": 6.25,
+             "cpu_iowait_warning": 5.625,
              "cpu_steal_careful": 50.0,
              "cpu_steal_critical": 90.0,
              "cpu_steal_warning": 70.0,
              "cpu_system_careful": 50.0,
              "cpu_system_critical": 90.0,
              "cpu_system_log": ["False"],
              "cpu_system_warning": 70.0,
@@ -1345,15 +1445,14 @@
                    "quicklook_load_warning": 100.0,
                    "quicklook_mem_careful": 50.0,
                    "quicklook_mem_critical": 90.0,
                    "quicklook_mem_warning": 70.0,
                    "quicklook_swap_careful": 50.0,
                    "quicklook_swap_critical": 90.0,
                    "quicklook_swap_warning": 70.0},
-     "raid": {"history_size": 1200.0, "raid_disable": ["False"]},
      "sensors": {"history_size": 1200.0,
                  "sensors_battery_careful": 80.0,
                  "sensors_battery_critical": 95.0,
                  "sensors_battery_warning": 90.0,
                  "sensors_disable": ["False"],
                  "sensors_hide": ["unknown.*"],
                  "sensors_refresh": 6.0,
@@ -1373,21 +1472,21 @@
               "wifi_critical": -85.0,
               "wifi_disable": ["False"],
               "wifi_warning": -75.0}}
 
 Limits/thresholds for the cpu plugin::
 
     # curl http://localhost:61208/api/4/cpu/limits
-    {"cpu_ctx_switches_careful": 160000.0,
-     "cpu_ctx_switches_critical": 200000.0,
-     "cpu_ctx_switches_warning": 180000.0,
+    {"cpu_ctx_switches_careful": 640000.0,
+     "cpu_ctx_switches_critical": 800000.0,
+     "cpu_ctx_switches_warning": 720000.0,
      "cpu_disable": ["False"],
-     "cpu_iowait_careful": 20.0,
-     "cpu_iowait_critical": 25.0,
-     "cpu_iowait_warning": 22.5,
+     "cpu_iowait_careful": 5.0,
+     "cpu_iowait_critical": 6.25,
+     "cpu_iowait_warning": 5.625,
      "cpu_steal_careful": 50.0,
      "cpu_steal_critical": 90.0,
      "cpu_steal_warning": 70.0,
      "cpu_system_careful": 50.0,
      "cpu_system_critical": 90.0,
      "cpu_system_log": ["False"],
      "cpu_system_warning": 70.0,
```

### Comparing `glances-4.0.4/docs/cmds.rst` & `glances-4.0.5/docs/cmds.rst`

 * *Files identical despite different names*

### Comparing `glances-4.0.4/docs/conf.py` & `glances-4.0.5/docs/conf.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,37 +1,35 @@
-# -*- coding: utf-8 -*-
 #
 # Glances documentation build configuration file, created by
 # sphinx-quickstart on Tue Mar  1 10:53:59 2016.
 #
 # This file is execfile()d with the current directory set to its
 # containing dir.
 #
 # Note that not all possible configuration values are present in this
 # autogenerated file.
 #
 # All configuration values have a default; values that are commented out
 # serve to show the default.
 
-import sys
 import os
+import sys
 from datetime import datetime
 
 # If extensions (or modules to document with autodoc) are in another directory,
 # add these directories to sys.path here. If the directory is relative to the
 # documentation root, use os.path.abspath to make it absolute, like shown here.
 # sys.path.insert(0, os.path.abspath('.'))
 
 # Insert Glances' path into the system.
 sys.path.insert(0, os.path.abspath('..'))
 
 # WARNING: Do not move this import before the sys.path.insert() call.
 from glances import __version__
 
-
 # -- General configuration ------------------------------------------------
 
 # If your documentation needs a minimal Sphinx version, state it here.
 # needs_sphinx = '1.0'
 
 # Add any Sphinx extension module names here, as strings. They can be
 # extensions coming with Sphinx (named 'sphinx.ext.*') or your custom
@@ -121,16 +119,15 @@
 # The theme to use for HTML and HTML Help pages.  See the documentation for
 # a list of builtin themes.
 html_theme = 'sphinx_rtd_theme'
 
 # Theme options are theme-specific and customize the look and feel of a theme
 # further.  For a list of options available for each theme, see the
 # documentation.
-html_theme_options = {
-}
+html_theme_options = {}
 
 # Add any paths that contain custom themes here, relative to this directory.
 # html_theme_path = []
 
 # The name for this set of Sphinx documents.  If None, it defaults to
 # "<project> v<release> documentation".
 # html_title = None
@@ -162,22 +159,15 @@
 # html_last_updated_fmt = '%b %d, %Y'
 
 # If true, SmartyPants will be used to convert quotes and dashes to
 # typographically correct entities.
 # html_use_smartypants = True
 
 # Custom sidebar templates, maps document names to template names.
-html_sidebars = {
-    '**': [
-        'about.html',
-        'navigation.html',
-        'links.html',
-        'searchbox.html'
-    ]
-}
+html_sidebars = {'**': ['about.html', 'navigation.html', 'links.html', 'searchbox.html']}
 
 # Additional templates that should be rendered to pages, maps page names to
 # template names.
 # html_additional_pages = {}
 
 # If false, no module index is generated.
 # html_domain_indices = True
@@ -223,31 +213,27 @@
 htmlhelp_basename = 'Glancesdoc'
 
 # -- Options for LaTeX output ---------------------------------------------
 
 latex_elements = {
     # The paper size ('letterpaper' or 'a4paper').
     # 'papersize': 'letterpaper',
-
     # The font size ('10pt', '11pt' or '12pt').
     # 'pointsize': '10pt',
-
     # Additional stuff for the LaTeX preamble.
     # 'preamble': '',
-
     # Latex figure (float) alignment
     # 'figure_align': 'htbp',
 }
 
 # Grouping the document tree into LaTeX files. List of tuples
 # (source start file, target name, title,
 #  author, documentclass [howto, manual, or own class]).
 latex_documents = [
-    (master_doc, 'Glances.tex', 'Glances Documentation',
-     'Nicolas Hennion', 'manual'),
+    (master_doc, 'Glances.tex', 'Glances Documentation', 'Nicolas Hennion', 'manual'),
 ]
 
 # The name of an image file (relative to this directory) to place at the top of
 # the title page.
 # latex_logo = None
 
 # For "manual" documents, if this is true, then toplevel headings are parts,
@@ -267,32 +253,35 @@
 # latex_domain_indices = True
 
 
 # -- Options for manual page output ---------------------------------------
 
 # One entry per manual page. List of tuples
 # (source start file, name, description, authors, manual section).
-man_pages = [
-    ('glances', 'glances', 'An eye on your system',
-     '', 1)
-]
+man_pages = [('glances', 'glances', 'An eye on your system', '', 1)]
 
 # If true, show URL addresses after external links.
 # man_show_urls = False
 
 
 # -- Options for Texinfo output -------------------------------------------
 
 # Grouping the document tree into Texinfo files. List of tuples
 # (source start file, target name, title, author,
 #  dir menu entry, description, category)
 texinfo_documents = [
-    (master_doc, 'Glances', 'Glances Documentation',
-     author, 'Glances', 'One line description of project.',
-     'Miscellaneous'),
+    (
+        master_doc,
+        'Glances',
+        'Glances Documentation',
+        author,
+        'Glances',
+        'One line description of project.',
+        'Miscellaneous',
+    ),
 ]
 
 # Documents to append as an appendix to all manuals.
 # texinfo_appendices = []
 
 # If false, no module index is generated.
 # texinfo_domain_indices = True
```

### Comparing `glances-4.0.4/docs/config.rst` & `glances-4.0.5/docs/config.rst`

 * *Files identical despite different names*

### Comparing `glances-4.0.4/docs/dev/glances-cprofile.png` & `glances-4.0.5/docs/dev/glances-cprofile.png`

 * *Files identical despite different names*

### Comparing `glances-4.0.4/docs/docker.rst` & `glances-4.0.5/docs/docker.rst`

 * *Files identical despite different names*

### Comparing `glances-4.0.4/docs/glances.rst` & `glances-4.0.5/docs/glances.rst`

 * *Files identical despite different names*

### Comparing `glances-4.0.4/docs/gw/cassandra.rst` & `glances-4.0.5/docs/gw/cassandra.rst`

 * *Files identical despite different names*

### Comparing `glances-4.0.4/docs/gw/couchdb.rst` & `glances-4.0.5/docs/gw/couchdb.rst`

 * *Files identical despite different names*

### Comparing `glances-4.0.4/docs/gw/csv.rst` & `glances-4.0.5/docs/gw/csv.rst`

 * *Files identical despite different names*

### Comparing `glances-4.0.4/docs/gw/graph.rst` & `glances-4.0.5/docs/gw/graph.rst`

 * *Files identical despite different names*

### Comparing `glances-4.0.4/docs/gw/graphite.rst` & `glances-4.0.5/docs/gw/graphite.rst`

 * *Files identical despite different names*

### Comparing `glances-4.0.4/docs/gw/influxdb.rst` & `glances-4.0.5/docs/gw/influxdb.rst`

 * *Files identical despite different names*

### Comparing `glances-4.0.4/docs/gw/kafka.rst` & `glances-4.0.5/docs/gw/kafka.rst`

 * *Files identical despite different names*

### Comparing `glances-4.0.4/docs/gw/mongodb.rst` & `glances-4.0.5/docs/gw/mongodb.rst`

 * *Files identical despite different names*

### Comparing `glances-4.0.4/docs/gw/mqtt.rst` & `glances-4.0.5/docs/gw/mqtt.rst`

 * *Files identical despite different names*

### Comparing `glances-4.0.4/docs/gw/prometheus.rst` & `glances-4.0.5/docs/gw/prometheus.rst`

 * *Files identical despite different names*

### Comparing `glances-4.0.4/docs/gw/restful.rst` & `glances-4.0.5/docs/gw/restful.rst`

 * *Files identical despite different names*

### Comparing `glances-4.0.4/docs/gw/statsd.rst` & `glances-4.0.5/docs/gw/statsd.rst`

 * *Files identical despite different names*

### Comparing `glances-4.0.4/docs/gw/zeromq.rst` & `glances-4.0.5/docs/gw/zeromq.rst`

 * *Files identical despite different names*

### Comparing `glances-4.0.4/docs/index.rst` & `glances-4.0.5/docs/index.rst`

 * *Files identical despite different names*

### Comparing `glances-4.0.4/docs/install.rst` & `glances-4.0.5/docs/install.rst`

 * *Files identical despite different names*

### Comparing `glances-4.0.4/docs/make.bat` & `glances-4.0.5/docs/make.bat`

 * *Files identical despite different names*

### Comparing `glances-4.0.4/docs/man/glances.1` & `glances-4.0.5/docs/man/glances.1`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 . RE
 .\" indent \\n[an-margin]
 .\" old: \\n[rst2man-indent\\n[rst2man-indent-level]]
 .nr rst2man-indent-level -1
 .\" new: \\n[rst2man-indent\\n[rst2man-indent-level]]
 .in \\n[rst2man-indent\\n[rst2man-indent-level]]u
 ..
-.TH "GLANCES" "1" "May 15, 2024" "4.0.4" "Glances"
+.TH "GLANCES" "1" "May 18, 2024" "4.0.5" "Glances"
 .SH NAME
 glances \- An eye on your system
 .SH SYNOPSIS
 .sp
 \fBglances\fP [OPTIONS]
 .SH DESCRIPTION
 .sp
```

### Comparing `glances-4.0.4/docs/objects.inv` & `glances-4.0.5/docs/objects.inv`

 * *Files identical despite different names*

### Comparing `glances-4.0.4/docs/quickstart.rst` & `glances-4.0.5/docs/quickstart.rst`

 * *Files identical despite different names*

### Comparing `glances-4.0.4/glances/__init__.py` & `glances-4.0.5/glances/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,30 +1,29 @@
-# -*- coding: utf-8 -*-
 #
 # This file is part of Glances.
 #
 # SPDX-FileCopyrightText: 2024 Nicolas Hennion <nicolas@nicolargo.com>
 #
 # SPDX-License-Identifier: LGPL-3.0-only
 #
 #
 
 """Init the Glances software."""
 
 # Import system libs
-import tracemalloc
 import locale
 import platform
 import signal
 import sys
+import tracemalloc
 
 # Global name
 # Version should start and end with a numerical char
 # See https://packaging.python.org/specifications/core-metadata/#version
-__version__ = '4.0.4'
+__version__ = '4.0.5'
 __apiversion__ = '4'
 __author__ = 'Nicolas Hennion <nicolas@nicolargo.com>'
 __license__ = 'LGPLv3'
 
 # Import psutil
 try:
     from psutil import __version__ as psutil_version
@@ -40,31 +39,27 @@
 
 # Check locale
 try:
     locale.setlocale(locale.LC_ALL, '')
 except locale.Error:
     print("Warning: Unable to set locale. Expect encoding problems.")
 
-# Check Python version
-if sys.version_info < (3, 4):
-    print('Glances requires at least Python 3.4 to run.')
-    sys.exit(1)
-
 # Check psutil version
 psutil_min_version = (5, 3, 0)
 psutil_version_info = tuple([int(num) for num in psutil_version.split('.')])
 if psutil_version_info < psutil_min_version:
     print('psutil 5.3.0 or higher is needed. Glances cannot start.')
     sys.exit(1)
 
+
 # Trac malloc is only available on Python 3.4 or higher
 
 
 def __signal_handler(signal, frame):
-    logger.debug("Signal {} catched".format(signal))
+    logger.debug(f"Signal {signal} catched")
     end()
 
 
 def end():
     """Stop Glances."""
     try:
         mode.end()
@@ -99,28 +94,24 @@
             from glances.client import GlancesClient as GlancesMode
     elif core.is_server():
         from glances.server import GlancesServer as GlancesMode
     elif core.is_webserver():
         from glances.webserver import GlancesWebServer as GlancesMode
 
     # Init the mode
-    logger.info("Start {} mode".format(GlancesMode.__name__))
+    logger.info(f"Start {GlancesMode.__name__} mode")
     mode = GlancesMode(config=config, args=args)
 
     # Start the main loop
-    logger.debug("Glances started in {} seconds".format(start_duration.get()))
+    logger.debug(f"Glances started in {start_duration.get()} seconds")
     if args.stop_after:
-        logger.info('Glances will be stopped in ~{} seconds'.format(args.stop_after * args.time))
+        logger.info(f'Glances will be stopped in ~{args.stop_after * args.time} seconds')
 
     if args.memory_leak:
-        print(
-            'Memory leak detection, please wait ~{} seconds...'.format(
-                args.stop_after * args.time * args.memory_leak * 2
-            )
-        )
+        print(f'Memory leak detection, please wait ~{args.stop_after * args.time * args.memory_leak * 2} seconds...')
         # First run without dump to fill the memory
         mode.serve_n(args.stop_after)
         # Then start the memory-leak loop
         snapshot_begin = tracemalloc.take_snapshot()
 
     if args.stdout_issue or args.stdout_apidoc:
         # Serve once for issue/test mode
@@ -129,15 +120,15 @@
         # Serve forever
         mode.serve_forever()
 
     if args.memory_leak:
         snapshot_end = tracemalloc.take_snapshot()
         snapshot_diff = snapshot_end.compare_to(snapshot_begin, 'filename')
         memory_leak = sum([s.size_diff for s in snapshot_diff])
-        print("Memory consumption: {0:.1f}KB (see log for details)".format(memory_leak / 1000))
+        print(f"Memory consumption: {memory_leak / 1000:.1f}KB (see log for details)")
         logger.info("Memory consumption (top 5):")
         for stat in snapshot_diff[:5]:
             logger.info(stat)
     elif args.trace_malloc:
         # See more options here: https://docs.python.org/3/library/tracemalloc.html
         snapshot = tracemalloc.take_snapshot()
         top_stats = snapshot.statistics("filename")
@@ -161,20 +152,18 @@
     else:
         signal_list = (signal.SIGTERM, signal.SIGINT, signal.SIGHUP)
     # Catch the kill signal
     for sig in signal_list:
         signal.signal(sig, __signal_handler)
 
     # Log Glances and psutil version
-    logger.info('Start Glances {}'.format(__version__))
-    logger.info(
-        '{} {} ({}) and psutil {} detected'.format(
-            platform.python_implementation(), platform.python_version(), sys.executable, psutil_version
-        )
-    )
+    logger.info(f'Start Glances {__version__}')
+    python_impl = platform.python_implementation()
+    python_ver = platform.python_version()
+    logger.info(f'{python_impl} {python_ver} ({sys.executable}) and psutil {psutil_version} detected')
 
     # Share global var
     global core
 
     # Create the Glances main instance
     # Glances options from the command line are read first (in __init__)
     # then the options from the config file (in parse_args)
```

### Comparing `glances-4.0.4/glances/actions.py` & `glances-4.0.5/glances/actions.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,32 +1,31 @@
-# -*- coding: utf-8 -*-
 #
 # This file is part of Glances.
 #
 # SPDX-FileCopyrightText: 2022 Nicolas Hennion <nicolas@nicolargo.com>
 #
 # SPDX-License-Identifier: LGPL-3.0-only
 #
 
 """Manage on alert actions."""
 
 from glances.logger import logger
-from glances.timer import Timer
 from glances.secure import secure_popen
+from glances.timer import Timer
 
 try:
     import chevron
 except ImportError:
     logger.debug("Chevron library not found (action scripts won't work)")
     chevron_tag = False
 else:
     chevron_tag = True
 
 
-class GlancesActions(object):
+class GlancesActions:
     """This class manage action if an alert is reached."""
 
     def __init__(self, args=None):
         """Init GlancesActions class."""
         # Dict with the criticality status
         # - key: stat_name
         # - value: criticality
@@ -76,18 +75,18 @@
         for cmd in commands:
             # Replace {{arg}} by the dict one (Thk to {Mustache})
             if chevron_tag:
                 cmd_full = chevron.render(cmd, mustache_dict)
             else:
                 cmd_full = cmd
             # Execute the action
-            logger.info("Action triggered for {} ({}): {}".format(stat_name, criticality, cmd_full))
+            logger.info(f"Action triggered for {stat_name} ({criticality}): {cmd_full}")
             try:
                 ret = secure_popen(cmd_full)
             except OSError as e:
-                logger.error("Action error for {} ({}): {}".format(stat_name, criticality, e))
+                logger.error(f"Action error for {stat_name} ({criticality}): {e}")
             else:
-                logger.debug("Action result for {} ({}): {}".format(stat_name, criticality, ret))
+                logger.debug(f"Action result for {stat_name} ({criticality}): {ret}")
 
         self.set(stat_name, criticality)
 
         return True
```

### Comparing `glances-4.0.4/glances/amps/amp.py` & `glances-4.0.5/glances/amps/amp.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 #
 # This file is part of Glances.
 #
 # SPDX-FileCopyrightText: 2024 Nicolas Hennion <nicolas@nicolargo.com>
 #
 # SPDX-License-Identifier: LGPL-3.0-only
 #
@@ -19,30 +18,30 @@
 The script should define a Amp (GlancesAmp) class with, at least, an update method.
 The update method should call the set_result method to set the AMP return string.
 The return string is a string with one or more line (\n between lines).
 If the *one_line* var is true then the AMP will be displayed in one line.
 """
 
 from glances.globals import u
-from glances.timer import Timer
 from glances.logger import logger
+from glances.timer import Timer
 
 
-class GlancesAmp(object):
+class GlancesAmp:
     """Main class for Glances AMP."""
 
     NAME = '?'
     VERSION = '?'
     DESCRIPTION = '?'
     AUTHOR = '?'
     EMAIL = '?'
 
     def __init__(self, name=None, args=None):
         """Init AMP class."""
-        logger.debug("AMP - Init {} version {}".format(self.NAME, self.VERSION))
+        logger.debug(f"AMP - Init {self.NAME} version {self.VERSION}")
 
         # AMP name (= module name without glances_)
         if name is None:
             self.amp_name = self.__class__.__module__
         else:
             self.amp_name = name
 
@@ -70,75 +69,71 @@
         # and optionally:
         #
         # one_line=false
         # option1=opt1
 
         amp_section = 'amp_' + self.amp_name
         if hasattr(config, 'has_section') and config.has_section(amp_section):
-            logger.debug("AMP - {}: Load configuration".format(self.NAME))
+            logger.debug(f"AMP - {self.NAME}: Load configuration")
             for param, _ in config.items(amp_section):
                 try:
                     self.configs[param] = config.get_float_value(amp_section, param)
                 except ValueError:
                     self.configs[param] = config.get_value(amp_section, param).split(',')
                     if len(self.configs[param]) == 1:
                         self.configs[param] = self.configs[param][0]
-                logger.debug("AMP - {}: Load parameter: {} = {}".format(self.NAME, param, self.configs[param]))
+                logger.debug(f"AMP - {self.NAME}: Load parameter: {param} = {self.configs[param]}")
         else:
-            logger.debug("AMP - {}: Can not find section {} in the configuration file".format(self.NAME, self.amp_name))
+            logger.debug(f"AMP - {self.NAME}: Can not find section {self.amp_name} in the configuration file")
             return False
 
         if self.enable():
             # Refresh option is mandatory
             for k in ['refresh']:
                 if k not in self.configs:
                     logger.warning(
-                        "AMP - {}: Can not find configuration key {} in section {} (the AMP will be disabled)".format(
-                            self.NAME, k, self.amp_name
-                        )
+                        f"AMP - {self.NAME}: Can not find configuration key {k} in section {self.amp_name} "
+                        f"(the AMP will be disabled)"
                     )
                     self.configs['enable'] = 'false'
         else:
-            logger.debug("AMP - {} is disabled".format(self.NAME))
+            logger.debug(f"AMP - {self.NAME} is disabled")
 
         # Init the count to 0
         self.configs['count'] = 0
 
         return self.enable()
 
     def get(self, key):
         """Generic method to get the item in the AMP configuration"""
         if key in self.configs:
             return self.configs[key]
-        else:
-            return None
+        return None
 
     def enable(self):
         """Return True|False if the AMP is enabled in the configuration file (enable=true|false)."""
         ret = self.get('enable')
         if ret is None:
             return False
-        else:
-            return ret.lower().startswith('true')
+        return ret.lower().startswith('true')
 
     def regex(self):
         """Return regular expression used to identified the current application."""
         return self.get('regex')
 
     def refresh(self):
         """Return refresh time in seconds for the current application monitoring process."""
         return self.get('refresh')
 
     def one_line(self):
         """Return True|False if the AMP should be displayed in one line (one_line=true|false)."""
         ret = self.get('one_line')
         if ret is None:
             return False
-        else:
-            return ret.lower().startswith('true')
+        return ret.lower().startswith('true')
 
     def time_until_refresh(self):
         """Return time in seconds until refresh."""
         return self.timer.get()
 
     def should_update(self):
         """Return True is the AMP should be updated
@@ -189,9 +184,8 @@
     def update_wrapper(self, process_list):
         """Wrapper for the children update"""
         # Set the number of running process
         self.set_count(len(process_list))
         # Call the children update method
         if self.should_update():
             return self.update(process_list)
-        else:
-            return self.result()
+        return self.result()
```

### Comparing `glances-4.0.4/glances/amps/default/__init__.py` & `glances-4.0.5/glances/amps/default/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 #
 # This file is part of Glances.
 #
 # SPDX-FileCopyrightText: 2022 Nicolas Hennion <nicolas@nicolargo.com>
 #
 # SPDX-License-Identifier: LGPL-3.0-only
 #
@@ -21,44 +20,44 @@
 enable=true
 regex=\/usr\/bin\/foo
 refresh=10
 one_line=false
 command=foo status
 """
 
-from subprocess import check_output, STDOUT, CalledProcessError
+from subprocess import STDOUT, CalledProcessError, check_output
 
-from glances.globals import u, to_ascii
-from glances.logger import logger
 from glances.amps.amp import GlancesAmp
+from glances.globals import to_ascii, u
+from glances.logger import logger
 
 
 class Amp(GlancesAmp):
     """Glances' Default AMP."""
 
     NAME = ''
     VERSION = '1.1'
     DESCRIPTION = ''
     AUTHOR = 'Nicolargo'
     EMAIL = 'contact@nicolargo.com'
 
     def __init__(self, name=None, args=None):
         """Init the AMP."""
         self.NAME = name.capitalize()
-        super(Amp, self).__init__(name=name, args=args)
+        super().__init__(name=name, args=args)
 
     def update(self, process_list):
         """Update the AMP"""
         # Get the systemctl status
         logger.debug('{}: Update AMP stats using command {}'.format(self.NAME, self.get('service_cmd')))
         # Get command to execute
         try:
             res = self.get('command')
         except OSError as e:
-            logger.debug('{}: Error while executing command ({})'.format(self.NAME, e))
+            logger.debug(f'{self.NAME}: Error while executing command ({e})')
             return self.result()
         # No command found, use default message
         if res is None:
             # Set the default message if command return None
             # Default sum of CPU and MEM for the matching regex
             self.set_result(
                 'CPU: {:.1f}% | MEM: {:.1f}%'.format(
```

### Comparing `glances-4.0.4/glances/amps/nginx/__init__.py` & `glances-4.0.5/glances/amps/nginx/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 #
 # This file is part of Glances.
 #
 # SPDX-FileCopyrightText: 2022 Nicolas Hennion <nicolas@nicolargo.com>
 #
 # SPDX-License-Identifier: LGPL-3.0-only
 #
@@ -42,16 +41,16 @@
 refresh=60
 one_line=false
 status_url=http://localhost/nginx_status
 """
 
 import requests
 
-from glances.logger import logger
 from glances.amps.amp import GlancesAmp
+from glances.logger import logger
 
 
 class Amp(GlancesAmp):
     """Glances' Nginx AMP."""
 
     NAME = 'Nginx'
     VERSION = '1.0'
```

### Comparing `glances-4.0.4/glances/amps/systemd/__init__.py` & `glances-4.0.5/glances/amps/systemd/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 #
 # This file is part of Glances.
 #
 # SPDX-FileCopyrightText: 2022 Nicolas Hennion <nicolas@nicolargo.com>
 #
 # SPDX-License-Identifier: LGPL-3.0-only
 #
@@ -31,19 +30,19 @@
 enable=true
 regex=\/usr\/lib\/systemd\/systemd
 refresh=60
 one_line=true
 systemctl_cmd=/usr/bin/systemctl --plain
 """
 
-from subprocess import check_output, CalledProcessError
+from subprocess import CalledProcessError, check_output
 
-from glances.logger import logger
-from glances.globals import iteritems, to_ascii
 from glances.amps.amp import GlancesAmp
+from glances.globals import iteritems, to_ascii
+from glances.logger import logger
 
 
 class Amp(GlancesAmp):
     """Glances' Systemd AMP."""
 
     NAME = 'Systemd'
     VERSION = '1.0'
@@ -58,15 +57,15 @@
     def update(self, process_list):
         """Update the AMP"""
         # Get the systemctl status
         logger.debug('{}: Update stats using systemctl {}'.format(self.NAME, self.get('systemctl_cmd')))
         try:
             res = check_output(self.get('systemctl_cmd').split())
         except (OSError, CalledProcessError) as e:
-            logger.debug('{}: Error while executing systemctl ({})'.format(self.NAME, e))
+            logger.debug(f'{self.NAME}: Error while executing systemctl ({e})')
         else:
             status = {}
             # For each line
             for r in to_ascii(res).split('\n')[1:-8]:
                 # Split per space .*
                 column = r.split()
                 if len(column) > 3:
@@ -75,11 +74,11 @@
                         try:
                             status[column[c]] += 1
                         except KeyError:
                             status[column[c]] = 1
             # Build the output (string) message
             output = 'Services\n'
             for k, v in iteritems(status):
-                output += '{}: {}\n'.format(k, v)
+                output += f'{k}: {v}\n'
             self.set_result(output, separator=' ')
 
         return self.result()
```

### Comparing `glances-4.0.4/glances/amps/systemv/__init__.py` & `glances-4.0.5/glances/amps/systemv/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 #
 # This file is part of Glances.
 #
 # SPDX-FileCopyrightText: 2022 Nicolas Hennion <nicolas@nicolargo.com>
 #
 # SPDX-License-Identifier: LGPL-3.0-only
 #
@@ -30,19 +29,19 @@
 enable=true
 regex=\/sbin\/init
 refresh=60
 one_line=true
 service_cmd=/usr/bin/service --status-all
 """
 
-from subprocess import check_output, STDOUT
+from subprocess import STDOUT, check_output
 
-from glances.logger import logger
-from glances.globals import iteritems
 from glances.amps.amp import GlancesAmp
+from glances.globals import iteritems
+from glances.logger import logger
 
 
 class Amp(GlancesAmp):
     """Glances' Systemd AMP."""
 
     NAME = 'SystemV'
     VERSION = '1.0'
@@ -57,15 +56,15 @@
     def update(self, process_list):
         """Update the AMP"""
         # Get the systemctl status
         logger.debug('{}: Update stats using service {}'.format(self.NAME, self.get('service_cmd')))
         try:
             res = check_output(self.get('service_cmd').split(), stderr=STDOUT).decode('utf-8')
         except OSError as e:
-            logger.debug('{}: Error while executing service ({})'.format(self.NAME, e))
+            logger.debug(f'{self.NAME}: Error while executing service ({e})')
         else:
             status = {'running': 0, 'stopped': 0, 'upstart': 0}
             # For each line
             for r in res.split('\n'):
                 # Split per space .*
                 line = r.split()
                 if len(line) < 4:
@@ -75,11 +74,11 @@
                 elif line[1] == '-':
                     status['stopped'] += 1
                 elif line[1] == '?':
                     status['upstart'] += 1
             # Build the output (string) message
             output = 'Services\n'
             for k, v in iteritems(status):
-                output += '{}: {}\n'.format(k, v)
+                output += f'{k}: {v}\n'
             self.set_result(output, separator=' ')
 
         return self.result()
```

### Comparing `glances-4.0.4/glances/amps_list.py` & `glances-4.0.5/glances/amps_list.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,28 +1,27 @@
-# -*- coding: utf-8 -*-
 #
 # This file is part of Glances.
 #
 # SPDX-FileCopyrightText: 2022 Nicolas Hennion <nicolas@nicolargo.com>
 #
 # SPDX-License-Identifier: LGPL-3.0-only
 #
 
 """Manage the AMPs list."""
 
 import os
 import re
 import threading
 
-from glances.globals import listkeys, iteritems, amps_path
+from glances.globals import amps_path, iteritems, listkeys
 from glances.logger import logger
 from glances.processes import glances_processes
 
 
-class AmpsList(object):
+class AmpsList:
     """This class describes the optional application monitoring process list.
 
     The AMP list is a list of processes with a specific monitoring action.
 
     The list (Python list) is composed of items (Python dict).
     An item is defined (dict keys):
     *...
@@ -53,27 +52,27 @@
                 amp_module = os.path.join(amps_path, amp_name)
                 if not os.path.exists(amp_module):
                     # If not, use the default script
                     amp_module = os.path.join(amps_path, "default")
                 try:
                     amp = __import__(os.path.basename(amp_module))
                 except ImportError as e:
-                    logger.warning("Missing Python Lib ({}), cannot load AMP {}".format(e, amp_name))
+                    logger.warning(f"Missing Python Lib ({e}), cannot load AMP {amp_name}")
                 except Exception as e:
-                    logger.warning("Cannot load AMP {} ({})".format(amp_name, e))
+                    logger.warning(f"Cannot load AMP {amp_name} ({e})")
                 else:
                     # Add the AMP to the dictionary
                     # The key is the AMP name
                     # for example, the file glances_xxx.py
                     # generate self._amps_list["xxx"] = ...
                     self.__amps_dict[amp_name] = amp.Amp(name=amp_name, args=self.args)
                     # Load the AMP configuration
                     self.__amps_dict[amp_name].load_config(self.config)
         # Log AMPs list
-        logger.debug("AMPs list: {}".format(self.getList()))
+        logger.debug(f"AMPs list: {self.getList()}")
 
         return True
 
     def __str__(self):
         return str(self.__amps_dict)
 
     def __repr__(self):
@@ -104,15 +103,15 @@
                 thread.start()
                 continue
 
             amps_list = self._build_amps_list(v, processlist)
 
             if len(amps_list) > 0:
                 # At least one process is matching the regex
-                logger.debug("AMPS: {} processes {} detected ({})".format(len(amps_list), k, amps_list))
+                logger.debug(f"AMPS: {len(amps_list)} processes {k} detected ({amps_list})")
                 # Call the AMP update method
                 thread = threading.Thread(target=v.update_wrapper, args=[amps_list])
                 thread.start()
             else:
                 # Set the process number to 0
                 v.set_count(0)
                 if v.count_min() is not None and v.count_min() > 0:
@@ -136,15 +135,15 @@
                     and re.search(amp_value.regex(), ' '.join(p['cmdline'])) is not None
                 ):
                     ret.append(
                         {'pid': p['pid'], 'cpu_percent': p['cpu_percent'], 'memory_percent': p['memory_percent']}
                     )
 
         except (TypeError, KeyError) as e:
-            logger.debug("Can not build AMPS list ({})".format(e))
+            logger.debug(f"Can not build AMPS list ({e})")
 
         return ret
 
     def getList(self):
         """Return the AMPs list."""
         return listkeys(self.__amps_dict)
```

### Comparing `glances-4.0.4/glances/attribute.py` & `glances-4.0.5/glances/attribute.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,21 @@
-# -*- coding: utf-8 -*-
 #
 # This file is part of Glances.
 #
 # SPDX-FileCopyrightText: 2022 Nicolas Hennion <nicolas@nicolargo.com>
 #
 # SPDX-License-Identifier: LGPL-3.0-only
 #
 
 """Attribute class."""
 
 from datetime import datetime
 
 
-class GlancesAttribute(object):
+class GlancesAttribute:
     def __init__(self, name, description='', history_max_size=None):
         """Init the attribute
 
         :param name: Attribute name (string)
         :param description: Attribute human reading description (string)
         :param history_max_size: Maximum size of the history list (default is no limit)
 
@@ -62,16 +61,15 @@
     Properties for the attribute value
     """
 
     @property
     def value(self):
         if self.history_len() > 0:
             return (self._value[1] - self.history_value()[1]) / (self._value[0] - self.history_value()[0])
-        else:
-            return None
+        return None
 
     @value.setter
     def value(self, new_value):
         """Set a value.
 
         Value is a tuple: (<timestamp>, <new_value>)
         """
```

### Comparing `glances-4.0.4/glances/autodiscover.py` & `glances-4.0.5/glances/autodiscover.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 #
 # This file is part of Glances.
 #
 # SPDX-FileCopyrightText: 2022 Nicolas Hennion <nicolas@nicolargo.com>
 #
 # SPDX-License-Identifier: LGPL-3.0-only
 #
@@ -12,36 +11,37 @@
 import socket
 import sys
 
 from glances.globals import BSD
 from glances.logger import logger
 
 try:
-    from zeroconf import __version__ as __zeroconf_version, ServiceBrowser, ServiceInfo, Zeroconf
+    from zeroconf import ServiceBrowser, ServiceInfo, Zeroconf
+    from zeroconf import __version__ as __zeroconf_version
 
     zeroconf_tag = True
 except ImportError:
     zeroconf_tag = False
 
 # Zeroconf 0.17 or higher is needed
 if zeroconf_tag:
     zeroconf_min_version = (0, 17, 0)
     zeroconf_version = tuple([int(num) for num in __zeroconf_version.split('.')])
-    logger.debug("Zeroconf version {} detected.".format(__zeroconf_version))
+    logger.debug(f"Zeroconf version {__zeroconf_version} detected.")
     if zeroconf_version < zeroconf_min_version:
         logger.critical("Please install zeroconf 0.17 or higher.")
         sys.exit(1)
 
 # Global var
 # Recent versions of the zeroconf python package doesn't like a zeroconf type that ends with '._tcp.'.
 # Correct issue: zeroconf problem with zeroconf_type = "_%s._tcp." % 'glances' #888
-zeroconf_type = "_%s._tcp.local." % 'glances'
+zeroconf_type = "_{}._tcp.local.".format('glances')
 
 
-class AutoDiscovered(object):
+class AutoDiscovered:
     """Class to manage the auto discovered servers dict."""
 
     def __init__(self):
         # server_dict is a list of dict (JSON compliant)
         # [ {'key': 'zeroconf name', ip': '172.1.2.3', 'port': 61209, 'cpu': 3, 'mem': 34 ...} ... ]
         self._server_list = []
 
@@ -62,29 +62,29 @@
             'port': port,  # TCP port
             'username': 'glances',  # Default username
             'password': '',  # Default password
             'status': 'UNKNOWN',  # Server status: 'UNKNOWN', 'OFFLINE', 'ONLINE', 'PROTECTED'
             'type': 'DYNAMIC',
         }  # Server type: 'STATIC' or 'DYNAMIC'
         self._server_list.append(new_server)
-        logger.debug("Updated servers list (%s servers): %s" % (len(self._server_list), self._server_list))
+        logger.debug(f"Updated servers list ({len(self._server_list)} servers): {self._server_list}")
 
     def remove_server(self, name):
         """Remove a server from the dict."""
         for i in self._server_list:
             if i['key'] == name:
                 try:
                     self._server_list.remove(i)
-                    logger.debug("Remove server %s from the list" % name)
-                    logger.debug("Updated servers list (%s servers): %s" % (len(self._server_list), self._server_list))
+                    logger.debug(f"Remove server {name} from the list")
+                    logger.debug(f"Updated servers list ({len(self._server_list)} servers): {self._server_list}")
                 except ValueError:
-                    logger.error("Cannot remove server %s from the list" % name)
+                    logger.error(f"Cannot remove server {name} from the list")
 
 
-class GlancesAutoDiscoverListener(object):
+class GlancesAutoDiscoverListener:
     """Zeroconf listener for Glances server."""
 
     def __init__(self):
         # Create an instance of the servers list
         self.servers = AutoDiscovered()
 
     def get_servers_list(self):
@@ -100,80 +100,79 @@
 
         Note: the return code will never be used
 
         :return: True if the zeroconf client is a Glances server
         """
         if srv_type != zeroconf_type:
             return False
-        logger.debug("Check new Zeroconf server: %s / %s" % (srv_type, srv_name))
+        logger.debug(f"Check new Zeroconf server: {srv_type} / {srv_name}")
         info = zeroconf.get_service_info(srv_type, srv_name)
         if info and (info.addresses or info.parsed_addresses):
             address = info.addresses[0] if info.addresses else info.parsed_addresses[0]
             new_server_ip = socket.inet_ntoa(address)
             new_server_port = info.port
 
             # Add server to the global dict
             self.servers.add_server(srv_name, new_server_ip, new_server_port)
-            logger.info("New Glances server detected (%s from %s:%s)" % (srv_name, new_server_ip, new_server_port))
+            logger.info(f"New Glances server detected ({srv_name} from {new_server_ip}:{new_server_port})")
         else:
             logger.warning("New Glances server detected, but failed to be get Zeroconf ServiceInfo ")
         return True
 
     def remove_service(self, zeroconf, srv_type, srv_name):
         """Remove the server from the list."""
         self.servers.remove_server(srv_name)
-        logger.info("Glances server %s removed from the autodetect list" % srv_name)
+        logger.info(f"Glances server {srv_name} removed from the autodetect list")
 
 
-class GlancesAutoDiscoverServer(object):
+class GlancesAutoDiscoverServer:
     """Implementation of the Zeroconf protocol (server side for the Glances client)."""
 
     def __init__(self, args=None):
         if zeroconf_tag:
             logger.info("Init autodiscover mode (Zeroconf protocol)")
             try:
                 self.zeroconf = Zeroconf()
-            except socket.error as e:
-                logger.error("Cannot start Zeroconf (%s)" % e)
+            except OSError as e:
+                logger.error(f"Cannot start Zeroconf ({e})")
                 self.zeroconf_enable_tag = False
             else:
                 self.listener = GlancesAutoDiscoverListener()
                 self.browser = ServiceBrowser(self.zeroconf, zeroconf_type, self.listener)
                 self.zeroconf_enable_tag = True
         else:
             logger.error("Cannot start autodiscover mode (Zeroconf lib is not installed)")
             self.zeroconf_enable_tag = False
 
     def get_servers_list(self):
         """Return the current server list (dict of dict)."""
         if zeroconf_tag and self.zeroconf_enable_tag:
             return self.listener.get_servers_list()
-        else:
-            return []
+        return []
 
     def set_server(self, server_pos, key, value):
         """Set the key to the value for the server_pos (position in the list)."""
         if zeroconf_tag and self.zeroconf_enable_tag:
             self.listener.set_server(server_pos, key, value)
 
     def close(self):
         if zeroconf_tag and self.zeroconf_enable_tag:
             self.zeroconf.close()
 
 
-class GlancesAutoDiscoverClient(object):
+class GlancesAutoDiscoverClient:
     """Implementation of the zeroconf protocol (client side for the Glances server)."""
 
     def __init__(self, hostname, args=None):
         if zeroconf_tag:
             zeroconf_bind_address = args.bind_address
             try:
                 self.zeroconf = Zeroconf()
-            except socket.error as e:
-                logger.error("Cannot start zeroconf: {}".format(e))
+            except OSError as e:
+                logger.error(f"Cannot start zeroconf: {e}")
 
             # XXX *BSDs: Segmentation fault (core dumped)
             # -- https://bitbucket.org/al45tair/netifaces/issues/15
             if not BSD:
                 try:
                     # -B @ overwrite the dynamic IPv4 choice
                     if zeroconf_bind_address == '0.0.0.0':
@@ -188,41 +187,41 @@
             # Check IP v4/v6
             address_family = socket.getaddrinfo(zeroconf_bind_address, args.port)[0][0]
 
             # Start the zeroconf service
             try:
                 self.info = ServiceInfo(
                     zeroconf_type,
-                    '{}:{}.{}'.format(hostname, args.port, zeroconf_type),
+                    f'{hostname}:{args.port}.{zeroconf_type}',
                     address=socket.inet_pton(address_family, zeroconf_bind_address),
                     port=args.port,
                     weight=0,
                     priority=0,
                     properties={},
                     server=hostname,
                 )
             except TypeError:
                 # Manage issue 1663 with breaking change on ServiceInfo method
                 # address (only one address) is replaced by addresses (list of addresses)
                 self.info = ServiceInfo(
                     zeroconf_type,
-                    name='{}:{}.{}'.format(hostname, args.port, zeroconf_type),
+                    name=f'{hostname}:{args.port}.{zeroconf_type}',
                     addresses=[socket.inet_pton(address_family, zeroconf_bind_address)],
                     port=args.port,
                     weight=0,
                     priority=0,
                     properties={},
                     server=hostname,
                 )
             try:
                 self.zeroconf.register_service(self.info)
             except Exception as e:
-                logger.error("Error while announcing Glances server: {}".format(e))
+                logger.error(f"Error while announcing Glances server: {e}")
             else:
-                print("Announce the Glances server on the LAN (using {} IP address)".format(zeroconf_bind_address))
+                print(f"Announce the Glances server on the LAN (using {zeroconf_bind_address} IP address)")
         else:
             logger.error("Cannot announce Glances server on the network: zeroconf library not found.")
 
     @staticmethod
     def find_active_ip_address():
         """Try to find the active IP addresses."""
         import netifaces
```

### Comparing `glances-4.0.4/glances/client.py` & `glances-4.0.5/glances/client.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,39 +1,38 @@
-# -*- coding: utf-8 -*-
 #
 # This file is part of Glances.
 #
 # SPDX-FileCopyrightText: 2022 Nicolas Hennion <nicolas@nicolargo.com>
 #
 # SPDX-License-Identifier: LGPL-3.0-only
 #
 
 """Manage the Glances client."""
 
-import ujson
-import socket
 import sys
 import time
 
+import ujson
+
 from glances import __version__
 from glances.globals import Fault, ProtocolError, ServerProxy, Transport
 from glances.logger import logger
-from glances.stats_client import GlancesStatsClient
 from glances.outputs.glances_curses import GlancesCursesClient
+from glances.stats_client import GlancesStatsClient
 from glances.timer import Counter
 
 
 class GlancesClientTransport(Transport):
     """This class overwrite the default XML-RPC transport and manage timeout."""
 
     def set_timeout(self, timeout):
         self.timeout = timeout
 
 
-class GlancesClient(object):
+class GlancesClient:
     """This class creates and manages the TCP client."""
 
     def __init__(self, config=None, args=None, timeout=7, return_to_browser=False):
         # Store the arg/config
         self.args = args
         self.config = config
 
@@ -44,27 +43,29 @@
         self._client_mode = 'glances'
 
         # Return to browser or exit
         self.return_to_browser = return_to_browser
 
         # Build the URI
         if args.password != "":
-            self.uri = 'http://{}:{}@{}:{}'.format(args.username, args.password, args.client, args.port)
+            self.uri = f'http://{args.username}:{args.password}@{args.client}:{args.port}'
         else:
-            self.uri = 'http://{}:{}'.format(args.client, args.port)
-        logger.debug("Try to connect to {}".format(self.uri))
+            self.uri = f'http://{args.client}:{args.port}'
+
+        # Avoid logging user credentials
+        logger.debug(f"Try to connect to 'http://{args.client}:{args.port}'")
 
         # Try to connect to the URI
         transport = GlancesClientTransport()
         # Configure the server timeout
         transport.set_timeout(timeout)
         try:
             self.client = ServerProxy(self.uri, transport=transport)
         except Exception as e:
-            self.log_and_exit("Client couldn't create socket {}: {}".format(self.uri, e))
+            self.log_and_exit(f"Client couldn't create socket {self.uri}: {e}")
 
     @property
     def quiet(self):
         return self._quiet
 
     def log_and_exit(self, msg=''):
         """Log and exit."""
@@ -89,46 +90,44 @@
         self._client_mode = mode
 
     def _login_glances(self):
         """Login to a Glances server"""
         client_version = None
         try:
             client_version = self.client.init()
-        except socket.error as err:
+        except OSError as err:
             # Fallback to SNMP
             self.client_mode = 'snmp'
-            logger.error("Connection to Glances server failed ({} {})".format(err.errno, err.strerror))
+            logger.error(f"Connection to Glances server failed ({err.errno} {err.strerror})")
             fall_back_msg = 'No Glances server found. Trying fallback to SNMP...'
             if not self.return_to_browser:
                 print(fall_back_msg)
             else:
                 logger.info(fall_back_msg)
         except ProtocolError as err:
             # Other errors
-            msg = "Connection to server {} failed".format(self.uri)
+            msg = f"Connection to server {self.uri} failed"
             if err.errcode == 401:
                 msg += " (Bad username/password)"
             else:
-                msg += " ({} {})".format(err.errcode, err.errmsg)
+                msg += f" ({err.errcode} {err.errmsg})"
             self.log_and_exit(msg)
             return False
 
         if self.client_mode == 'glances':
             # Check that both client and server are in the same major version
             if __version__.split('.')[0] == client_version.split('.')[0]:
                 # Init stats
                 self.stats = GlancesStatsClient(config=self.config, args=self.args)
                 self.stats.set_plugins(ujson.loads(self.client.getAllPlugins()))
-                logger.debug("Client version: {} / Server version: {}".format(__version__, client_version))
+                logger.debug(f"Client version: {__version__} / Server version: {client_version}")
             else:
                 self.log_and_exit(
-                    (
-                        'Client and server not compatible: '
-                        'Client version: {} / Server version: {}'.format(__version__, client_version)
-                    )
+                    'Client and server not compatible: '
+                    f'Client version: {__version__} / Server version: {client_version}'
                 )
                 return False
 
         return True
 
     def _login_snmp(self):
         """Login to a SNMP server"""
@@ -176,32 +175,32 @@
         # Return True: OK
         return True
 
     def update(self):
         """Update stats from Glances/SNMP server."""
         if self.client_mode == 'glances':
             return self.update_glances()
-        elif self.client_mode == 'snmp':
+        if self.client_mode == 'snmp':
             return self.update_snmp()
-        else:
-            self.end()
-            logger.critical("Unknown server mode: {}".format(self.client_mode))
-            sys.exit(2)
+
+        self.end()
+        logger.critical(f"Unknown server mode: {self.client_mode}")
+        sys.exit(2)
 
     def update_glances(self):
         """Get stats from Glances server.
 
         Return the client/server connection status:
         - Connected: Connection OK
         - Disconnected: Connection NOK
         """
         # Update the stats
         try:
             server_stats = ujson.loads(self.client.getAll())
-        except socket.error:
+        except OSError:
             # Client cannot get server stats
             return "Disconnected"
         except Fault:
             # Client cannot get server stats (issue #375)
             return "Disconnected"
         else:
             # Put it in the internal dict
@@ -236,20 +235,20 @@
 
         exit_key = False
         try:
             while True and not exit_key:
                 # Update the stats
                 counter = Counter()
                 cs_status = self.update()
-                logger.debug('Stats updated duration: {} seconds'.format(counter.get()))
+                logger.debug(f'Stats updated duration: {counter.get()} seconds')
 
                 # Export stats using export modules
                 counter_export = Counter()
                 self.stats.export(self.stats)
-                logger.debug('Stats exported duration: {} seconds'.format(counter_export.get()))
+                logger.debug(f'Stats exported duration: {counter_export.get()} seconds')
 
                 # Patch for issue1326 to avoid < 0 refresh
                 adapted_refresh = self.refresh_time - counter.get()
                 adapted_refresh = adapted_refresh if adapted_refresh > 0 else 0
 
                 # Update the screen
                 if not self.quiet:
```

### Comparing `glances-4.0.4/glances/client_browser.py` & `glances-4.0.5/glances/client_browser.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,32 +1,31 @@
-# -*- coding: utf-8 -*-
 #
 # This file is part of Glances.
 #
 # SPDX-FileCopyrightText: 2022 Nicolas Hennion <nicolas@nicolargo.com>
 #
 # SPDX-License-Identifier: LGPL-3.0-only
 #
 
 """Manage the Glances client browser (list of Glances server)."""
 
-import ujson
-import socket
 import threading
 
-from glances.globals import Fault, ProtocolError, ServerProxy
+import ujson
+
+from glances.autodiscover import GlancesAutoDiscoverServer
 from glances.client import GlancesClient, GlancesClientTransport
-from glances.logger import logger, LOG_FILENAME
+from glances.globals import Fault, ProtocolError, ServerProxy
+from glances.logger import LOG_FILENAME, logger
+from glances.outputs.glances_curses_browser import GlancesCursesBrowser
 from glances.password_list import GlancesPasswordList as GlancesPassword
 from glances.static_list import GlancesStaticServer
-from glances.autodiscover import GlancesAutoDiscoverServer
-from glances.outputs.glances_curses_browser import GlancesCursesBrowser
 
 
-class GlancesClientBrowser(object):
+class GlancesClientBrowser:
     """This class creates and manages the TCP client browser (servers list)."""
 
     def __init__(self, config=None, args=None):
         # Store the arg/config
         self.args = args
         self.config = config
         self.static_server = None
@@ -72,71 +71,70 @@
         if server['password'] != "":
             if server['status'] == 'PROTECTED':
                 # Try with the preconfigure password (only if status is PROTECTED)
                 clear_password = self.password.get_password(server['name'])
                 if clear_password is not None:
                     server['password'] = self.password.get_hash(clear_password)
             return 'http://{}:{}@{}:{}'.format(server['username'], server['password'], server['ip'], server['port'])
-        else:
-            return 'http://{}:{}'.format(server['ip'], server['port'])
+        return 'http://{}:{}'.format(server['ip'], server['port'])
 
     def __update_stats(self, server):
         """Update stats for the given server (picked from the server list)"""
         # Get the server URI
         uri = self.__get_uri(server)
 
         # Try to connect to the server
         t = GlancesClientTransport()
         t.set_timeout(3)
 
         # Get common stats
         try:
             s = ServerProxy(uri, transport=t)
         except Exception as e:
-            logger.warning("Client browser couldn't create socket ({})".format(e))
+            logger.warning(f"Client browser couldn't create socket ({e})")
         else:
             # Mandatory stats
             try:
                 # CPU%
                 cpu_percent = 100 - ujson.loads(s.getCpu())['idle']
-                server['cpu_percent'] = '{:.1f}'.format(cpu_percent)
+                server['cpu_percent'] = f'{cpu_percent:.1f}'
                 # MEM%
                 server['mem_percent'] = ujson.loads(s.getMem())['percent']
                 # OS (Human Readable name)
                 server['hr_name'] = ujson.loads(s.getSystem())['hr_name']
-            except (socket.error, Fault, KeyError) as e:
-                logger.debug("Error while grabbing stats form server ({})".format(e))
+            except (OSError, Fault, KeyError) as e:
+                logger.debug(f"Error while grabbing stats form server ({e})")
                 server['status'] = 'OFFLINE'
             except ProtocolError as e:
                 if e.errcode == 401:
                     # Error 401 (Authentication failed)
                     # Password is not the good one...
                     server['password'] = None
                     server['status'] = 'PROTECTED'
                 else:
                     server['status'] = 'OFFLINE'
-                logger.debug("Cannot grab stats from server ({} {})".format(e.errcode, e.errmsg))
+                logger.debug(f"Cannot grab stats from server ({e.errcode} {e.errmsg})")
             else:
                 # Status
                 server['status'] = 'ONLINE'
 
                 # Optional stats (load is not available on Windows OS)
                 try:
                     # LOAD
                     load_min5 = ujson.loads(s.getLoad())['min5']
-                    server['load_min5'] = '{:.2f}'.format(load_min5)
+                    server['load_min5'] = f'{load_min5:.2f}'
                 except Exception as e:
-                    logger.warning("Error while grabbing stats form server ({})".format(e))
+                    logger.warning(f"Error while grabbing stats form server ({e})")
 
         return server
 
     def __display_server(self, server):
         """Connect and display the given server"""
         # Display the Glances client for the selected server
-        logger.debug("Selected server {}".format(server))
+        logger.debug(f"Selected server {server}")
 
         # Connection can take time
         # Display a popup
         self.screen.display_popup('Connect to {}:{}'.format(server['name'], server['port']), duration=1)
 
         # A password is needed to access to the server's stats
         if server['password'] is None:
@@ -197,15 +195,15 @@
         """Main client loop."""
         # No need to update the server list
         # It's done by the GlancesAutoDiscoverListener class (autodiscover.py)
         # Or define statically in the configuration file (module static_list.py)
         # For each server in the list, grab elementary stats (CPU, LOAD, MEM, OS...)
         thread_list = {}
         while not self.screen.is_end:
-            logger.debug("Iter through the following server list: {}".format(self.get_servers_list()))
+            logger.debug(f"Iter through the following server list: {self.get_servers_list()}")
             for v in self.get_servers_list():
                 key = v["key"]
                 thread = thread_list.get(key, None)
                 if thread is None or thread.is_alive() is False:
                     thread = threading.Thread(target=self.__update_stats, args=[v])
                     thread_list[key] = thread
                     thread.start()
```

### Comparing `glances-4.0.4/glances/config.py` & `glances-4.0.5/glances/config.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,25 +1,24 @@
-# -*- coding: utf-8 -*-
 #
 # This file is part of Glances.
 #
 # SPDX-FileCopyrightText: 2022 Nicolas Hennion <nicolas@nicolargo.com>
 #
 # SPDX-License-Identifier: LGPL-3.0-only
 #
 
 """Manage the configuration file."""
 
-import os
-import sys
+import builtins
 import multiprocessing
-from io import open
+import os
 import re
+import sys
 
-from glances.globals import ConfigParser, NoOptionError, NoSectionError, system_exec, BSD, LINUX, MACOS, SUNOS, WINDOWS
+from glances.globals import BSD, LINUX, MACOS, SUNOS, WINDOWS, ConfigParser, NoOptionError, NoSectionError, system_exec
 from glances.logger import logger
 
 
 def user_config_dir():
     r"""Return a list of per-user config dir (full path).
 
     - Linux, *BSD, SunOS: ~/.config/glances
@@ -90,15 +89,15 @@
         path = ''
     else:
         path = os.path.join(path, 'glances')
 
     return [path]
 
 
-class Config(object):
+class Config:
     """This class is used to access/read config file, if it exists.
 
     :param config_dir: the path to search for config file
     :type config_dir: str or None
     """
 
     def __init__(self, config_dir=None):
@@ -149,23 +148,23 @@
         paths.extend([os.path.join(path, self.config_filename) for path in default_config_dir()])
 
         return paths
 
     def read(self):
         """Read the config file, if it exists. Using defaults otherwise."""
         for config_file in self.config_file_paths():
-            logger.debug('Search glances.conf file in {}'.format(config_file))
+            logger.debug(f'Search glances.conf file in {config_file}')
             if os.path.exists(config_file):
                 try:
-                    with open(config_file, encoding='utf-8') as f:
+                    with builtins.open(config_file, encoding='utf-8') as f:
                         self.parser.read_file(f)
                         self.parser.read(f)
-                    logger.info("Read configuration file '{}'".format(config_file))
+                    logger.info(f"Read configuration file '{config_file}'")
                 except UnicodeDecodeError as err:
-                    logger.error("Can not read configuration file '{}': {}".format(config_file, err))
+                    logger.error(f"Can not read configuration file '{config_file}': {err}")
                     sys.exit(1)
                 # Save the loaded configuration file path (issue #374)
                 self._loaded_config_file = config_file
                 break
 
         # Set the default values for section not configured
         self.sections_set_default()
```

### Comparing `glances-4.0.4/glances/cpu_percent.py` & `glances-4.0.5/glances/cpu_percent.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,24 @@
-# -*- coding: utf-8 -*-
 #
 # This file is part of Glances.
 #
 # SPDX-FileCopyrightText: 2022 Nicolas Hennion <nicolas@nicolargo.com>
 #
 # SPDX-License-Identifier: LGPL-3.0-only
 #
 
 """CPU percent stats shared between CPU and Quicklook plugins."""
 
+import psutil
+
 from glances.logger import logger
 from glances.timer import Timer
 
-import psutil
-
 
-class CpuPercent(object):
+class CpuPercent:
     """Get and store the CPU percent."""
 
     def __init__(self, cached_timer_cpu=3):
         self.cpu_info = {'cpu_name': None, 'cpu_hz_current': None, 'cpu_hz': None}
         self.cpu_percent = 0
         self.percpu_percent = []
 
@@ -42,26 +41,25 @@
         return 'cpu_number'
 
     def get(self, percpu=False):
         """Update and/or return the CPU using the psutil library.
         If percpu, return the percpu stats"""
         if percpu:
             return self.__get_percpu()
-        else:
-            return self.__get_cpu()
+        return self.__get_cpu()
 
     def get_info(self):
         """Get additional information about the CPU"""
         # Never update more than 1 time per cached_timer_cpu_info
         if self.timer_cpu_info.finished() and hasattr(psutil, 'cpu_freq'):
             # Get the CPU freq current/max
             try:
                 cpu_freq = psutil.cpu_freq()
             except Exception as e:
-                logger.debug('Can not grab CPU information ({})'.format(e))
+                logger.debug(f'Can not grab CPU information ({e})')
             else:
                 if hasattr(cpu_freq, 'current'):
                     self.cpu_info['cpu_hz_current'] = cpu_freq.current
                 else:
                     self.cpu_info['cpu_hz_current'] = None
                 if hasattr(cpu_freq, 'max'):
                     self.cpu_info['cpu_hz'] = cpu_freq.max
@@ -71,15 +69,15 @@
                 self.timer_cpu_info.reset(duration=self.cached_timer_cpu_info)
         return self.cpu_info
 
     def __get_cpu_name(self):
         # Get the CPU name once from the /proc/cpuinfo file
         # TODO: Multisystem...
         try:
-            self.cpu_info['cpu_name'] = open('/proc/cpuinfo', 'r').readlines()[4].split(':')[1].strip()
+            self.cpu_info['cpu_name'] = open('/proc/cpuinfo').readlines()[4].split(':')[1].strip()
         except (FileNotFoundError, PermissionError, IndexError, KeyError, AttributeError):
             self.cpu_info['cpu_name'] = 'CPU'
         return self.cpu_info['cpu_name']
 
     def __get_cpu(self):
         """Update and/or return the CPU using the psutil library."""
         # Never update more than 1 time per cached_timer_cpu
```

### Comparing `glances-4.0.4/glances/event.py` & `glances-4.0.5/glances/event.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,18 @@
-# -*- coding: utf-8 -*-
 #
 # This file is part of Glances.
 #
 # SPDX-FileCopyrightText: 2022 Nicolas Hennion <nicolas@nicolargo.com>
 #
 # SPDX-License-Identifier: LGPL-3.0-only
 #
 
 """Manage Glances event class
-This class is a Pydantic data class for the Glances event.
+
+This class is a data class for the Glances event.
 
 event_state = "OK|CAREFUL|WARNING|CRITICAL"
 event_type = "CPU*|LOAD|MEM|MON"
 event_value = value
 
 Item (or event) is defined by:
     {
@@ -28,15 +28,21 @@
         "top": [top 3 process name],
         "desc": "Processes description",
         "sort": "top sort key",
         "global": "global alert message"
     }
 """
 
-from pydantic.dataclasses import dataclass
+from glances.logger import logger
+
+try:
+    from pydantic.dataclasses import dataclass
+except ImportError as e:
+    logger.warning(f"Missing Python Lib ({e}), EventList will be skipping data validation")
+    from dataclasses import dataclass
 
 from glances.processes import sort_stats
 
 
 @dataclass
 class GlancesEvent:
     begin: int
```

### Comparing `glances-4.0.4/glances/events_list.py` & `glances-4.0.5/glances/events_list.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,24 @@
-# -*- coding: utf-8 -*-
 #
 # This file is part of Glances.
 #
 # SPDX-FileCopyrightText: 2022 Nicolas Hennion <nicolas@nicolargo.com>
 #
 # SPDX-License-Identifier: LGPL-3.0-only
 #
 
 """Manage Glances events list (previously Glances logs in Glances < 3.1)."""
 
 import time
+from dataclasses import asdict
 from datetime import datetime
-from pydantic import RootModel
 
+from glances.event import GlancesEvent
 from glances.processes import glances_processes
 from glances.thresholds import glances_thresholds
-from glances.event import GlancesEvent
 
 # Static decision tree for the global alert message
 # - msg: Message to be displayed (result of the decision tree)
 # - thresholds: a list of stats to take into account
 # - thresholds_min: minimal value of the thresholds sum
 # -                 0: OK
 # -                 1: CAREFUL
@@ -154,19 +153,18 @@
     current_thresholds = glances_thresholds.get()
     for i in tree:
         i['weight'] = sum([current_thresholds[t].value() for t in i['thresholds'] if t in current_thresholds])
     themax = max(tree, key=lambda d: d['weight'])
     if themax['weight'] >= themax['thresholds_min']:
         # Check if the weight is > to the minimal threshold value
         return themax['msg']
-    else:
-        return tree[0]['msg']
+    return tree[0]['msg']
 
 
-class GlancesEventsList(object):
+class GlancesEventsList:
     """This class manages events inside the Glances software.
     GlancesEventsList is a list of GlancesEvent.
     GlancesEvent is defined in the event.py file
     """
 
     def __init__(self, max_events=10, min_duration=6, min_interval=6):
         """Init the events class.
@@ -197,15 +195,15 @@
 
     def set_min_interval(self, min_interval):
         """Set the minimum interval between same kind of alert (in seconds)."""
         self.min_interval = min_interval
 
     def get(self):
         """Return the RAW events list."""
-        return [RootModel[GlancesEvent](e).model_dump() for e in self.events_list]
+        return [asdict(e) for e in self.events_list]
 
     def len(self):
         """Return the number of events in the logs list."""
         return self.events_list.__len__()
 
     def __event_exist(self, event_time, event_type):
         """Return the event position in the events list if:
```

### Comparing `glances-4.0.4/glances/exports/export.py` & `glances-4.0.5/glances/exports/export.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,29 +1,27 @@
-# -*- coding: utf-8 -*-
 #
 # This file is part of Glances.
 #
 # SPDX-FileCopyrightText: 2022 Nicolas Hennion <nicolas@nicolargo.com>
 #
 # SPDX-License-Identifier: LGPL-3.0-only
 #
 
 """
 I am your father...
 
 ...for all Glances exports IF.
 """
 
-from glances.globals import json_dumps
-from glances.globals import NoOptionError, NoSectionError, iteritems, iterkeys
-from glances.timer import Counter
+from glances.globals import NoOptionError, NoSectionError, iteritems, iterkeys, json_dumps
 from glances.logger import logger
+from glances.timer import Counter
 
 
-class GlancesExport(object):
+class GlancesExport:
     """Main class for Glances export IF."""
 
     # List of non exportable plugins
     # @TODO: remove this part and make all plugins exportable (see issue #1556)
     # @TODO: also make this list configurable by the user (see issue #1443)
     non_exportable_plugins = [
         'alert',
@@ -36,15 +34,15 @@
         'version',
     ]
 
     def __init__(self, config=None, args=None):
         """Init the export class."""
         # Export name
         self.export_name = self.__class__.__module__
-        logger.debug("Init export module %s" % self.export_name)
+        logger.debug(f"Init export module {self.export_name}")
 
         # Init the config & args
         self.config = config
         self.args = args
 
         # By default export is disabled
         # Needs to be set to True in the __init__ class of child
@@ -60,26 +58,24 @@
     def _log_result_decorator(fct):
         """Log (DEBUG) the result of the function fct."""
 
         def wrapper(*args, **kw):
             counter = Counter()
             ret = fct(*args, **kw)
             duration = counter.get()
-            logger.debug(
-                "{} {} {} return {} in {} seconds".format(
-                    args[0].__class__.__name__, args[0].__class__.__module__, fct.__name__, ret, duration
-                )
-            )
+            class_name = args[0].__class__.__name__
+            class_module = args[0].__class__.__module__
+            logger.debug(f"{class_name} {class_module} {fct.__name__} return {ret} in {duration} seconds")
             return ret
 
         return wrapper
 
     def exit(self):
         """Close the export module."""
-        logger.debug("Finalise export interface %s" % self.export_name)
+        logger.debug(f"Finalise export interface {self.export_name}")
 
     def load_conf(self, section, mandatories=['host', 'port'], options=None):
         """Load the export <section> configuration in the Glances configuration file.
 
         :param section: name of the export section to load
         :param mandatories: a list of mandatory parameters to load
         :param options: a list of optional parameters to load
@@ -92,43 +88,42 @@
             return False
 
         # By default read the mandatory host:port items
         try:
             for opt in mandatories:
                 setattr(self, opt, self.config.get_value(section, opt))
         except NoSectionError:
-            logger.error("No {} configuration found".format(section))
+            logger.error(f"No {section} configuration found")
             return False
         except NoOptionError as e:
-            logger.error("Error in the {} configuration ({})".format(section, e))
+            logger.error(f"Error in the {section} configuration ({e})")
             return False
 
         # Load options
         for opt in options:
             try:
                 setattr(self, opt, self.config.get_value(section, opt))
             except NoOptionError:
                 pass
 
-        logger.debug("Load {} from the Glances configuration file".format(section))
-        logger.debug("{} parameters: {}".format(section, {opt: getattr(self, opt) for opt in mandatories + options}))
+        logger.debug(f"Load {section} from the Glances configuration file")
+        logger.debug(f"{section} parameters: {({opt: getattr(self, opt) for opt in mandatories + options})}")
 
         return True
 
     def get_item_key(self, item):
         """Return the value of the item 'key'."""
         ret = None
         try:
             ret = item[item['key']]
         except KeyError:
-            logger.error("No 'key' available in {}".format(item))
+            logger.error(f"No 'key' available in {item}")
         if isinstance(ret, list):
             return ret[0]
-        else:
-            return ret
+        return ret
 
     def parse_tags(self, tags):
         """Parse tags into a dict.
 
         :param tags: a comma-separated list of 'key:value' pairs. Example: foo:bar,spam:eggs
         :return: a dict of tags. Example: {'foo': 'bar', 'spam': 'eggs'}
         """
```

### Comparing `glances-4.0.4/glances/exports/glances_cassandra/__init__.py` & `glances-4.0.5/glances/exports/glances_cassandra/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,37 +1,36 @@
-# -*- coding: utf-8 -*-
 #
 # This file is part of Glances.
 #
 # SPDX-FileCopyrightText: 2022 Nicolas Hennion <nicolas@nicolargo.com>
 #
 # SPDX-License-Identifier: LGPL-3.0-only
 #
 
 """Cassandra/Scylla interface class."""
 
 import sys
 from datetime import datetime
 from numbers import Number
 
-from glances.logger import logger
-from glances.exports.export import GlancesExport
-
+from cassandra import InvalidRequest
 from cassandra.auth import PlainTextAuthProvider
 from cassandra.cluster import Cluster
 from cassandra.util import uuid_from_time
-from cassandra import InvalidRequest
+
+from glances.exports.export import GlancesExport
+from glances.logger import logger
 
 
 class Export(GlancesExport):
     """This class manages the Cassandra/Scylla export module."""
 
     def __init__(self, config=None, args=None):
         """Init the Cassandra export IF."""
-        super(Export, self).__init__(config=config, args=args)
+        super().__init__(config=config, args=args)
 
         # Mandatory configuration keys (additional to host and port)
         self.keyspace = None
 
         # Optional configuration keys
         self.protocol_version = 3
         self.replication_factor = 2
@@ -65,62 +64,61 @@
                 [self.host],
                 port=int(self.port),
                 protocol_version=int(self.protocol_version),
                 auth_provider=auth_provider,
             )
             session = cluster.connect()
         except Exception as e:
-            logger.critical("Cannot connect to Cassandra cluster '%s:%s' (%s)" % (self.host, self.port, e))
+            logger.critical(f"Cannot connect to Cassandra cluster '{self.host}:{self.port}' ({e})")
             sys.exit(2)
 
         # Keyspace
         try:
             session.set_keyspace(self.keyspace)
         except InvalidRequest:
-            logger.info("Create keyspace {} on the Cassandra cluster".format(self.keyspace))
-            c = "CREATE KEYSPACE %s WITH replication = { 'class': 'SimpleStrategy', 'replication_factor': '%s' }" % (
-                self.keyspace,
-                self.replication_factor,
+            logger.info(f"Create keyspace {self.keyspace} on the Cassandra cluster")
+            c = (
+                f"CREATE KEYSPACE {self.keyspace} WITH "
+                f"replication = {{ 'class': 'SimpleStrategy', 'replication_factor': '{self.replication_factor}' }}"
             )
             session.execute(c)
             session.set_keyspace(self.keyspace)
 
         logger.info(
-            "Stats will be exported to Cassandra cluster {} ({}) in keyspace {}".format(
-                cluster.metadata.cluster_name, cluster.metadata.all_hosts(), self.keyspace
-            )
+            f"Stats will be exported to Cassandra cluster {cluster.metadata.cluster_name} "
+            f"({cluster.metadata.all_hosts()}) in keyspace {self.keyspace}"
         )
 
         # Table
         try:
             session.execute(
-                "CREATE TABLE %s (plugin text, time timeuuid, stat map<text,float>, PRIMARY KEY (plugin, time)) \
-                    WITH CLUSTERING ORDER BY (time DESC)"
-                % self.table
+                f"CREATE TABLE {self.table} "
+                f"(plugin text, time timeuuid, stat map<text,float>, PRIMARY KEY (plugin, time)) "
+                f"WITH CLUSTERING ORDER BY (time DESC)"
             )
         except Exception:
-            logger.debug("Cassandra table %s already exist" % self.table)
+            logger.debug(f"Cassandra table {self.table} already exist")
 
         return cluster, session
 
     def export(self, name, columns, points):
         """Write the points to the Cassandra cluster."""
-        logger.debug("Export {} stats to Cassandra".format(name))
+        logger.debug(f"Export {name} stats to Cassandra")
 
         # Remove non number stats and convert all to float (for Boolean)
         data = {k: float(v) for (k, v) in dict(zip(columns, points)).iteritems() if isinstance(v, Number)}
 
         # Write input to the Cassandra table
         try:
-            stmt = "INSERT INTO {} (plugin, time, stat) VALUES (?, ?, ?)".format(self.table)
+            stmt = f"INSERT INTO {self.table} (plugin, time, stat) VALUES (?, ?, ?)"
             query = self.session.prepare(stmt)
             self.session.execute(query, (name, uuid_from_time(datetime.now()), data))
         except Exception as e:
-            logger.error("Cannot export {} stats to Cassandra ({})".format(name, e))
+            logger.error(f"Cannot export {name} stats to Cassandra ({e})")
 
     def exit(self):
         """Close the Cassandra export module."""
         # To ensure all connections are properly closed
         self.session.shutdown()
         self.cluster.shutdown()
         # Call the father method
-        super(Export, self).exit()
+        super().exit()
```

### Comparing `glances-4.0.4/glances/exports/glances_couchdb/__init__.py` & `glances-4.0.5/glances/exports/glances_couchdb/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 #
 # This file is part of Glances.
 #
 # SPDX-FileCopyrightText: 2022 Nicolas Hennion <nicolas@nicolargo.com>
 #
 # SPDX-License-Identifier: LGPL-3.0-only
 #
@@ -16,26 +15,26 @@
 # 2) ./venv/bin/python -m glances -C ./conf/glances.conf --export couchdb --quiet
 # 3) Result can be seen at: http://127.0.0.1:5984/_utils
 #
 
 import sys
 from datetime import datetime
 
-from glances.logger import logger
-from glances.exports.export import GlancesExport
-
 import pycouchdb
 
+from glances.exports.export import GlancesExport
+from glances.logger import logger
+
 
 class Export(GlancesExport):
     """This class manages the CouchDB export module."""
 
     def __init__(self, config=None, args=None):
         """Init the CouchDB export IF."""
-        super(Export, self).__init__(config=config, args=args)
+        super().__init__(config=config, args=args)
 
         # Load the CouchDB configuration file section
         # User and Password are mandatory with CouchDB 3.0 and higher
         self.export_enable = self.load_conf('couchdb', mandatories=['host', 'port', 'db', 'user', 'password'])
         if not self.export_enable:
             sys.exit(2)
 
@@ -44,45 +43,45 @@
 
     def init(self):
         """Init the connection to the CouchDB server."""
         if not self.export_enable:
             return None
 
         # @TODO: https
-        server_uri = 'http://{}:{}@{}:{}/'.format(self.user, self.password, self.host, self.port)
+        server_uri = f'http://{self.user}:{self.password}@{self.host}:{self.port}/'
 
         try:
             s = pycouchdb.Server(server_uri)
         except Exception as e:
-            logger.critical("Cannot connect to CouchDB server (%s)" % e)
+            logger.critical(f"Cannot connect to CouchDB server ({e})")
             sys.exit(2)
         else:
-            logger.info("Connected to the CouchDB server version %s" % s.info()['version'])
+            logger.info("Connected to the CouchDB server version {}".format(s.info()['version']))
 
         try:
             s.database(self.db)
         except Exception:
             # Database did not exist
             # Create it...
             s.create(self.db)
-            logger.info("Create CouchDB database %s" % self.db)
+            logger.info(f"Create CouchDB database {self.db}")
         else:
-            logger.info("CouchDB database %s already exist" % self.db)
+            logger.info(f"CouchDB database {self.db} already exist")
 
         return s.database(self.db)
 
     def export(self, name, columns, points):
         """Write the points to the CouchDB server."""
-        logger.debug("Export {} stats to CouchDB".format(name))
+        logger.debug(f"Export {name} stats to CouchDB")
 
         # Create DB input
         data = dict(zip(columns, points))
 
         # Add the type and the timestamp in ISO format
         data['type'] = name
         data['time'] = datetime.now().isoformat()[:-3] + 'Z'
 
         # Write data to the CouchDB database
         try:
             self.client.save(data)
         except Exception as e:
-            logger.error("Cannot export {} stats to CouchDB ({})".format(name, e))
+            logger.error(f"Cannot export {name} stats to CouchDB ({e})")
```

### Comparing `glances-4.0.4/glances/exports/glances_csv/__init__.py` & `glances-4.0.5/glances/exports/glances_csv/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,33 +1,32 @@
-# -*- coding: utf-8 -*-
 #
 # This file is part of Glances.
 #
 # SPDX-FileCopyrightText: 2022 Nicolas Hennion <nicolas@nicolargo.com>
 #
 # SPDX-License-Identifier: LGPL-3.0-only
 #
 
 """CSV interface class."""
 
-import os.path
 import csv
+import os.path
 import sys
 import time
 
-from glances.logger import logger
 from glances.exports.export import GlancesExport
+from glances.logger import logger
 
 
 class Export(GlancesExport):
     """This class manages the CSV export module."""
 
     def __init__(self, config=None, args=None):
         """Init the CSV export IF."""
-        super(Export, self).__init__(config=config, args=args)
+        super().__init__(config=config, args=args)
 
         # CSV file name
         self.csv_filename = args.export_csv_file
 
         # Set the CSV output file
         # (see https://github.com/nicolargo/glances/issues/1525)
         if not os.path.isfile(self.csv_filename) or args.export_csv_overwrite:
@@ -38,36 +37,36 @@
             # A CSV file already exit, append new data
             file_mode = 'a'
             # Header will be checked later
             # Get the existing one
             try:
                 self.csv_file = open_csv_file(self.csv_filename, 'r')
                 reader = csv.reader(self.csv_file)
-            except IOError as e:
-                logger.critical("Cannot open existing CSV file: {}".format(e))
+            except OSError as e:
+                logger.critical(f"Cannot open existing CSV file: {e}")
                 sys.exit(2)
             self.old_header = next(reader, None)
             self.csv_file.close()
 
         try:
             self.csv_file = open_csv_file(self.csv_filename, file_mode)
             self.writer = csv.writer(self.csv_file)
-        except IOError as e:
-            logger.critical("Cannot create the CSV file: {}".format(e))
+        except OSError as e:
+            logger.critical(f"Cannot create the CSV file: {e}")
             sys.exit(2)
 
-        logger.info("Stats exported to CSV file: {}".format(self.csv_filename))
+        logger.info(f"Stats exported to CSV file: {self.csv_filename}")
 
         self.export_enable = True
 
         self.first_line = True
 
     def exit(self):
         """Close the CSV file."""
-        logger.debug("Finalise export interface %s" % self.export_name)
+        logger.debug(f"Finalise export interface {self.export_name}")
         self.csv_file.close()
 
     def update(self, stats):
         """Update stats in the CSV output file.
         Note: This class overwrite the one in the parent class because we need to manage the header.
         """
         # Get the stats
@@ -91,16 +90,16 @@
             if self.old_header is None:
                 # New file, write the header on top on the CSV file
                 self.writer.writerow(csv_header)
             # File already exist, check if header are compatible
             if self.old_header != csv_header and self.old_header is not None:
                 # Header are different, log an error and do not write data
                 logger.error("Cannot append data to existing CSV file. Headers are different.")
-                logger.debug("Old header: {}".format(self.old_header))
-                logger.debug("New header: {}".format(csv_header))
+                logger.debug(f"Old header: {self.old_header}")
+                logger.debug(f"New header: {csv_header}")
             else:
                 # Header are equals, ready to write data
                 self.old_header = None
             # Only do this once
             self.first_line = False
         # Manage data
         if self.old_header is None:
```

### Comparing `glances-4.0.4/glances/exports/glances_elasticsearch/__init__.py` & `glances-4.0.5/glances/exports/glances_elasticsearch/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,33 +1,32 @@
-# -*- coding: utf-8 -*-
 #
 # This file is part of Glances.
 #
 # SPDX-FileCopyrightText: 2022 Nicolas Hennion <nicolas@nicolargo.com>
 #
 # SPDX-License-Identifier: LGPL-3.0-only
 #
 
 """ElasticSearch interface class."""
 
 import sys
 from datetime import datetime
 
-from glances.logger import logger
-from glances.exports.export import GlancesExport
-
 from elasticsearch import Elasticsearch, helpers
 
+from glances.exports.export import GlancesExport
+from glances.logger import logger
+
 
 class Export(GlancesExport):
     """This class manages the ElasticSearch (ES) export module."""
 
     def __init__(self, config=None, args=None):
         """Init the ES export IF."""
-        super(Export, self).__init__(config=config, args=args)
+        super().__init__(config=config, args=args)
 
         # Mandatory configuration keys (additional to host and port)
         self.index = None
 
         # Load the ES configuration file
         self.export_enable = self.load_conf(
             'elasticsearch', mandatories=['scheme', 'host', 'port', 'index'], options=[]
@@ -40,49 +39,47 @@
 
     def init(self):
         """Init the connection to the ES server."""
         if not self.export_enable:
             return None
 
         try:
-            es = Elasticsearch(hosts=['{}://{}:{}'.format(self.scheme, self.host, self.port)])
+            es = Elasticsearch(hosts=[f'{self.scheme}://{self.host}:{self.port}'])
         except Exception as e:
-            logger.critical(
-                "Cannot connect to ElasticSearch server %s://%s:%s (%s)" % (self.scheme, self.host, self.port, e)
-            )
+            logger.critical(f"Cannot connect to ElasticSearch server {self.scheme}://{self.host}:{self.port} ({e})")
             sys.exit(2)
 
         if not es.ping():
-            logger.critical("Cannot ping the ElasticSearch server %s://%s:%s" % (self.scheme, self.host, self.port))
+            logger.critical(f"Cannot ping the ElasticSearch server {self.scheme}://{self.host}:{self.port}")
             sys.exit(2)
         else:
-            logger.info("Connected to the ElasticSearch server %s://%s:%s" % (self.scheme, self.host, self.port))
+            logger.info(f"Connected to the ElasticSearch server {self.scheme}://{self.host}:{self.port}")
 
         return es
 
     def export(self, name, columns, points):
         """Write the points to the ES server."""
-        logger.debug("Export {} stats to ElasticSearch".format(name))
+        logger.debug(f"Export {name} stats to ElasticSearch")
 
         # Generate index name with the index field + current day
         index = '{}-{}'.format(self.index, datetime.utcnow().strftime("%Y.%m.%d"))
 
         # Create DB input
         # https://elasticsearch-py.readthedocs.io/en/master/helpers.html
         actions = []
         dt_now = datetime.utcnow().isoformat('T')
         action = {
             "_index": index,
-            "_id": '{}.{}'.format(name, dt_now),
-            "_type": 'glances-{}'.format(name),
+            "_id": f'{name}.{dt_now}',
+            "_type": f'glances-{name}',
             "_source": {"plugin": name, "timestamp": dt_now},
         }
         action['_source'].update(zip(columns, [str(p) for p in points]))
         actions.append(action)
 
-        logger.debug("Exporting the following object to elasticsearch: {}".format(action))
+        logger.debug(f"Exporting the following object to elasticsearch: {action}")
 
         # Write input to the ES index
         try:
             helpers.bulk(self.client, actions)
         except Exception as e:
-            logger.error("Cannot export {} stats to ElasticSearch ({})".format(name, e))
+            logger.error(f"Cannot export {name} stats to ElasticSearch ({e})")
```

### Comparing `glances-4.0.4/glances/exports/glances_graph/__init__.py` & `glances-4.0.5/glances/exports/glances_graph/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,37 +1,37 @@
-# -*- coding: utf-8 -*-
 #
 # This file is part of Glances.
 #
 # SPDX-FileCopyrightText: 2022 Nicolas Hennion <nicolas@nicolargo.com>
 #
 # SPDX-License-Identifier: LGPL-3.0-only
 #
 
 """Graph exporter interface class."""
 
-from pygal import DateTimeLine
-import pygal.style
-import sys
+import errno
 import os
+import sys
 import tempfile
-import errno
 
+import pygal.style
+from pygal import DateTimeLine
+
+from glances.exports.export import GlancesExport
+from glances.globals import iteritems, time_serie_subsample
 from glances.logger import logger
 from glances.timer import Timer
-from glances.globals import iteritems, time_serie_subsample
-from glances.exports.export import GlancesExport
 
 
 class Export(GlancesExport):
     """This class manages the Graph export module."""
 
     def __init__(self, config=None, args=None):
         """Init the export IF."""
-        super(Export, self).__init__(config=config, args=args)
+        super().__init__(config=config, args=args)
 
         # Load the Graph configuration file section (is exists)
         self.export_enable = self.load_conf('graph', options=['path', 'generate_every', 'width', 'height', 'style'])
 
         # Manage options (command line arguments overwrite configuration file)
         self.path = args.export_graph_path or self.path
         self.generate_every = int(getattr(self, 'generate_every', 0))
@@ -40,37 +40,37 @@
         self.style = getattr(pygal.style, getattr(self, 'style', 'DarkStyle'), pygal.style.DarkStyle)
 
         # Create export folder
         try:
             os.makedirs(self.path)
         except OSError as e:
             if e.errno != errno.EEXIST:
-                logger.critical("Cannot create the Graph output folder {} ({})".format(self.path, e))
+                logger.critical(f"Cannot create the Graph output folder {self.path} ({e})")
                 sys.exit(2)
 
         # Check if output folder is writeable
         try:
             tempfile.TemporaryFile(dir=self.path)
         except OSError:
-            logger.critical("Graph output folder {} is not writeable".format(self.path))
+            logger.critical(f"Graph output folder {self.path} is not writeable")
             sys.exit(2)
 
-        logger.info("Graphs will be created in the {} folder".format(self.path))
+        logger.info(f"Graphs will be created in the {self.path} folder")
         if self.generate_every != 0:
-            logger.info("Graphs will be created automatically every {} seconds".format(self.generate_every))
+            logger.info(f"Graphs will be created automatically every {self.generate_every} seconds")
             logger.info("or when 'g' key is pressed (only through the CLI interface)")
             # Start the timer
             self._timer = Timer(self.generate_every)
         else:
             logger.info("Graphs will be created  when 'g' key is pressed (in the CLI interface)")
             self._timer = None
 
     def exit(self):
         """Close the files."""
-        logger.debug("Finalise export interface %s" % self.export_name)
+        logger.debug(f"Finalise export interface {self.export_name}")
 
     def update(self, stats):
         """Generate Graph file in the output folder."""
 
         if self.generate_every != 0 and self._timer.finished():
             self.args.generate_graph = True
             self._timer.reset()
@@ -80,15 +80,15 @@
 
         plugins = stats.getPluginsList()
         for plugin_name in plugins:
             plugin = stats._plugins[plugin_name]
             if plugin_name in self.plugins_to_export(stats):
                 self.export(plugin_name, plugin.get_export_history())
 
-        logger.info("Graphs created in {}".format(self.path))
+        logger.info(f"Graphs created in {self.path}")
         self.args.generate_graph = False
 
     def export(self, title, data):
         """Generate graph from the data.
 
         Example for the mem plugin:
         {'percent': [
```

### Comparing `glances-4.0.4/glances/exports/glances_graphite/__init__.py` & `glances-4.0.5/glances/exports/glances_graphite/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,33 +1,32 @@
-# -*- coding: utf-8 -*-
 #
 # This file is part of Glances.
 #
 # SPDX-FileCopyrightText: 2022 Nicolas Hennion <nicolas@nicolargo.com>
 #
 # SPDX-License-Identifier: LGPL-3.0-only
 #
 
 """Graphite interface class."""
 
 import sys
 from numbers import Number
 
-from glances.logger import logger
-from glances.exports.export import GlancesExport
-
 from graphitesend import GraphiteClient
 
+from glances.exports.export import GlancesExport
+from glances.logger import logger
+
 
 class Export(GlancesExport):
     """This class manages the Graphite export module."""
 
     def __init__(self, config=None, args=None):
         """Init the Graphite export IF."""
-        super(Export, self).__init__(config=config, args=args)
+        super().__init__(config=config, args=args)
 
         # Mandatory configuration keys (additional to host and port)
         # N/A
 
         # Optional configuration keys
         self.debug = False
         self.prefix = None
@@ -70,36 +69,34 @@
                     graphite_port=self.port,
                     prefix=self.prefix,
                     system_name=self.system_name,
                     lowercase_metric_names=True,
                     debug=self.debug,
                 )
         except Exception as e:
-            logger.error("Can not write data to Graphite server: {}:{} ({})".format(self.host, self.port, e))
+            logger.error(f"Can not write data to Graphite server: {self.host}:{self.port} ({e})")
             client = None
         else:
-            logger.info("Stats will be exported to Graphite server: {}:{}".format(self.host, self.port))
+            logger.info(f"Stats will be exported to Graphite server: {self.host}:{self.port}")
         return client
 
     def export(self, name, columns, points):
         """Export the stats to the Graphite server."""
         if self.client is None:
             return False
-        before_filtering_dict = dict(zip([normalize('{}.{}'.format(name, i)) for i in columns], points))
+        before_filtering_dict = dict(zip([normalize(f'{name}.{i}') for i in columns], points))
         after_filtering_dict = dict(filter(lambda i: isinstance(i[1], Number), before_filtering_dict.items()))
         try:
             self.client.send_dict(after_filtering_dict)
         except Exception as e:
-            logger.error("Can not export stats to Graphite (%s)" % e)
+            logger.error(f"Can not export stats to Graphite ({e})")
             return False
         else:
-            logger.debug("Export {} stats to Graphite".format(name))
+            logger.debug(f"Export {name} stats to Graphite")
         return True
 
 
 def normalize(name):
     """Normalize name for the Graphite convention"""
 
     # Name should not contain space
-    ret = name.replace(' ', '_')
-
-    return ret
+    return name.replace(' ', '_')
```

### Comparing `glances-4.0.4/glances/exports/glances_influxdb/__init__.py` & `glances-4.0.5/glances/exports/glances_influxdb/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,36 +1,35 @@
-# -*- coding: utf-8 -*-
 #
 # This file is part of Glances.
 #
 # SPDX-FileCopyrightText: 2022 Nicolas Hennion <nicolas@nicolargo.com>
 #
 # SPDX-License-Identifier: LGPL-3.0-only
 #
 
 """InfluxDB (up to InfluxDB 1.7.x) interface class."""
 
 import sys
 from platform import node
 
-from glances.logger import logger
-from glances.exports.export import GlancesExport
-
 from influxdb import InfluxDBClient
 from influxdb.client import InfluxDBClientError
 
-FIELD_TO_TAG = ['name', 'cmdline']
+from glances.exports.export import GlancesExport
+from glances.logger import logger
+
+FIELD_TO_TAG = ['name', 'cmdline', 'type']
 
 
 class Export(GlancesExport):
     """This class manages the InfluxDB export module."""
 
     def __init__(self, config=None, args=None):
         """Init the InfluxDB export IF."""
-        super(Export, self).__init__(config=config, args=args)
+        super().__init__(config=config, args=args)
 
         # Mandatory configuration keys (additional to host and port)
         self.user = None
         self.password = None
         self.db = None
 
         # Optional configuration keys
@@ -71,21 +70,21 @@
                 verify_ssl=False,
                 username=self.user,
                 password=self.password,
                 database=self.db,
             )
             get_all_db = [i['name'] for i in db.get_list_database()]
         except InfluxDBClientError as e:
-            logger.critical("Cannot connect to InfluxDB database '%s' (%s)" % (self.db, e))
+            logger.critical(f"Cannot connect to InfluxDB database '{self.db}' ({e})")
             sys.exit(2)
 
         if self.db in get_all_db:
-            logger.info("Stats will be exported to InfluxDB server: {}".format(db._baseurl))
+            logger.info(f"Stats will be exported to InfluxDB server: {db._baseurl}")
         else:
-            logger.critical("InfluxDB database '%s' did not exist. Please create it" % self.db)
+            logger.critical(f"InfluxDB database '{self.db}' did not exist. Please create it")
             sys.exit(2)
 
         return db
 
     def _normalize(self, name, columns, points):
         """Normalize data for the InfluxDB's data model.
 
@@ -102,17 +101,15 @@
         if len(keys_list) == 0:
             keys_list = [None]
 
         for measurement in keys_list:
             # Manage field
             if measurement is not None:
                 fields = {
-                    k.replace('{}.'.format(measurement), ''): data_dict[k]
-                    for k in data_dict
-                    if k.startswith('{}.'.format(measurement))
+                    k.replace(f'{measurement}.', ''): data_dict[k] for k in data_dict if k.startswith(f'{measurement}.')
                 }
             else:
                 fields = data_dict
             # Transform to InfluxDB data model
             # https://docs.influxdata.com/influxdb/v1.8/write_protocols/line_protocol_reference/
             for k in fields:
                 #  Do not export empty (None) value
@@ -151,16 +148,16 @@
     def export(self, name, columns, points):
         """Write the points to the InfluxDB server."""
         # Manage prefix
         if self.prefix is not None:
             name = self.prefix + '.' + name
         # Write input to the InfluxDB database
         if len(points) == 0:
-            logger.debug("Cannot export empty {} stats to InfluxDB".format(name))
+            logger.debug(f"Cannot export empty {name} stats to InfluxDB")
         else:
             try:
                 self.client.write_points(self._normalize(name, columns, points), time_precision="s")
             except Exception as e:
                 # Log level set to debug instead of error (see: issue #1561)
-                logger.debug("Cannot export {} stats to InfluxDB ({})".format(name, e))
+                logger.debug(f"Cannot export {name} stats to InfluxDB ({e})")
             else:
-                logger.debug("Export {} stats to InfluxDB".format(name))
+                logger.debug(f"Export {name} stats to InfluxDB")
```

### Comparing `glances-4.0.4/glances/exports/glances_influxdb2/__init__.py` & `glances-4.0.5/glances/exports/glances_influxdb2/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,35 +1,34 @@
-# -*- coding: utf-8 -*-
 #
 # This file is part of Glances.
 #
 # SPDX-FileCopyrightText: 2022 Nicolas Hennion <nicolas@nicolargo.com>
 #
 # SPDX-License-Identifier: LGPL-3.0-only
 #
 
 """InfluxDB (from to InfluxDB 1.8+) interface class."""
 
 import sys
 from platform import node
 
-from glances.logger import logger
-from glances.exports.export import GlancesExport
-
 from influxdb_client import InfluxDBClient, WriteOptions
 
-FIELD_TO_TAG = ['name', 'cmdline']
+from glances.exports.export import GlancesExport
+from glances.logger import logger
+
+FIELD_TO_TAG = ['name', 'cmdline', 'type']
 
 
 class Export(GlancesExport):
     """This class manages the InfluxDB export module."""
 
     def __init__(self, config=None, args=None):
         """Init the InfluxDB export IF."""
-        super(Export, self).__init__(config=config, args=args)
+        super().__init__(config=config, args=args)
 
         # Mandatory configuration keys (additional to host and port)
         self.org = None
         self.bucket = None
         self.token = None
 
         # Optional configuration keys
@@ -54,52 +53,49 @@
         try:
             self.interval = int(self.interval)
         except ValueError:
             logger.warning("InfluxDB export interval is not an integer, use default value")
             self.interval = 0
         # and should be set to the Glances refresh time if the value is 0
         self.interval = self.interval if self.interval > 0 else self.args.time
-        logger.debug("InfluxDB export interval is set to {} seconds".format(self.interval))
+        logger.debug(f"InfluxDB export interval is set to {self.interval} seconds")
 
         # The hostname is always add as a tag
         self.hostname = node().split('.')[0]
 
         # Init the InfluxDB client
         self.client = self.init()
 
     def init(self):
         """Init the connection to the InfluxDB server."""
         if not self.export_enable:
             return None
 
-        url = '{}://{}:{}'.format(self.protocol, self.host, self.port)
+        url = f'{self.protocol}://{self.host}:{self.port}'
         try:
             # See docs: https://influxdb-client.readthedocs.io/en/stable/api.html#influxdbclient
             client = InfluxDBClient(url=url, enable_gzip=False, verify_ssl=False, org=self.org, token=self.token)
         except Exception as e:
-            logger.critical("Cannot connect to InfluxDB server '%s' (%s)" % (url, e))
+            logger.critical(f"Cannot connect to InfluxDB server '{url}' ({e})")
             sys.exit(2)
         else:
-            logger.info(
-                "Connected to InfluxDB server version {} ({})".format(client.health().version, client.health().message)
-            )
+            logger.info(f"Connected to InfluxDB server version {client.health().version} ({client.health().message})")
 
         # Create the write client
-        write_client = client.write_api(
+        return client.write_api(
             write_options=WriteOptions(
                 batch_size=500,
                 flush_interval=self.interval * 1000,
                 jitter_interval=2000,
                 retry_interval=5000,
                 max_retries=5,
                 max_retry_delay=30000,
                 exponential_base=2,
             )
         )
-        return write_client
 
     def _normalize(self, name, columns, points):
         """Normalize data for the InfluxDB's data model.
 
         :return: a list of measurements.
         """
         ret = []
@@ -113,17 +109,15 @@
         if len(keys_list) == 0:
             keys_list = [None]
 
         for measurement in keys_list:
             # Manage field
             if measurement is not None:
                 fields = {
-                    k.replace('{}.'.format(measurement), ''): data_dict[k]
-                    for k in data_dict
-                    if k.startswith('{}.'.format(measurement))
+                    k.replace(f'{measurement}.', ''): data_dict[k] for k in data_dict if k.startswith(f'{measurement}.')
                 }
             else:
                 fields = data_dict
             # Transform to InfluxDB datamodel
             # https://docs.influxdata.com/influxdb/v2.0/reference/syntax/line-protocol/
             for k in fields:
                 #  Do not export empty (None) value
@@ -162,16 +156,16 @@
     def export(self, name, columns, points):
         """Write the points to the InfluxDB server."""
         # Manage prefix
         if self.prefix is not None:
             name = self.prefix + '.' + name
         # Write input to the InfluxDB database
         if len(points) == 0:
-            logger.debug("Cannot export empty {} stats to InfluxDB".format(name))
+            logger.debug(f"Cannot export empty {name} stats to InfluxDB")
         else:
             try:
                 self.client.write(self.bucket, self.org, self._normalize(name, columns, points), time_precision="s")
             except Exception as e:
                 # Log level set to debug instead of error (see: issue #1561)
-                logger.debug("Cannot export {} stats to InfluxDB ({})".format(name, e))
+                logger.debug(f"Cannot export {name} stats to InfluxDB ({e})")
             else:
-                logger.debug("Export {} stats to InfluxDB".format(name))
+                logger.debug(f"Export {name} stats to InfluxDB")
```

### Comparing `glances-4.0.4/glances/exports/glances_json/__init__.py` & `glances-4.0.5/glances/exports/glances_json/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,57 +1,57 @@
 """JSON interface class."""
 
 import sys
 
-from glances.globals import listkeys, json_dumps
-from glances.logger import logger
 from glances.exports.export import GlancesExport
+from glances.globals import json_dumps, listkeys
+from glances.logger import logger
 
 
 class Export(GlancesExport):
     """This class manages the JSON export module."""
 
     def __init__(self, config=None, args=None):
         """Init the JSON export IF."""
-        super(Export, self).__init__(config=config, args=args)
+        super().__init__(config=config, args=args)
 
         # JSON file name
         self.json_filename = args.export_json_file
 
         # Set the JSON output file
         try:
             self.json_file = open(self.json_filename, 'w')
             self.json_file.close()
-        except IOError as e:
-            logger.critical("Cannot create the JSON file: {}".format(e))
+        except OSError as e:
+            logger.critical(f"Cannot create the JSON file: {e}")
             sys.exit(2)
 
-        logger.info("Exporting stats to file: {}".format(self.json_filename))
+        logger.info(f"Exporting stats to file: {self.json_filename}")
 
         self.export_enable = True
 
         # Buffer for dict of stats
         self.buffer = {}
 
     def exit(self):
         """Close the JSON file."""
-        logger.debug("Finalise export interface %s" % self.export_name)
+        logger.debug(f"Finalise export interface {self.export_name}")
         self.json_file.close()
 
     def export(self, name, columns, points):
         """Export the stats to the JSON file."""
 
         # Check for completion of loop for all exports
         if name == self.last_exported_list()[0] and self.buffer != {}:
             # One whole loop has been completed
             # Flush stats to file
-            logger.debug("Exporting stats ({}) to JSON file ({})".format(listkeys(self.buffer), self.json_filename))
+            logger.debug(f"Exporting stats ({listkeys(self.buffer)}) to JSON file ({self.json_filename})")
 
             # Export stats to JSON file
             with open(self.json_filename, "w") as self.json_file:
-                self.json_file.write("{}\n".format(json_dumps(self.buffer)))
+                self.json_file.write(f"{json_dumps(self.buffer)}\n")
 
             # Reset buffer
             self.buffer = {}
 
         # Add current stat to the buffer
         self.buffer[name] = dict(zip(columns, points))
```

### Comparing `glances-4.0.4/glances/exports/glances_kafka/__init__.py` & `glances-4.0.5/glances/exports/glances_kafka/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,33 +1,32 @@
-# -*- coding: utf-8 -*-
 #
 # This file is part of Glances.
 #
 # SPDX-FileCopyrightText: 2022 Nicolas Hennion <nicolas@nicolargo.com>
 #
 # SPDX-License-Identifier: LGPL-3.0-only
 #
 
 """Kafka interface class."""
 
 import sys
 
-from glances.logger import logger
-from glances.globals import json_dumps
-from glances.exports.export import GlancesExport
-
 from kafka import KafkaProducer
 
+from glances.exports.export import GlancesExport
+from glances.globals import json_dumps
+from glances.logger import logger
+
 
 class Export(GlancesExport):
     """This class manages the Kafka export module."""
 
     def __init__(self, config=None, args=None):
         """Init the Kafka export IF."""
-        super(Export, self).__init__(config=config, args=args)
+        super().__init__(config=config, args=args)
 
         # Mandatory configuration keys (additional to host and port)
         self.topic = None
 
         # Optional configuration keys
         self.compression = None
         self.tags = None
@@ -44,33 +43,33 @@
 
     def init(self):
         """Init the connection to the Kafka server."""
         if not self.export_enable:
             return None
 
         # Build the server URI with host and port
-        server_uri = '{}:{}'.format(self.host, self.port)
+        server_uri = f'{self.host}:{self.port}'
 
         try:
             s = KafkaProducer(
                 bootstrap_servers=server_uri,
                 value_serializer=lambda v: json_dumps(v).encode('utf-8'),
                 compression_type=self.compression,
             )
         except Exception as e:
-            logger.critical("Cannot connect to Kafka server %s (%s)" % (server_uri, e))
+            logger.critical(f"Cannot connect to Kafka server {server_uri} ({e})")
             sys.exit(2)
         else:
-            logger.info("Connected to the Kafka server %s" % server_uri)
+            logger.info(f"Connected to the Kafka server {server_uri}")
 
         return s
 
     def export(self, name, columns, points):
         """Write the points to the kafka server."""
-        logger.debug("Export {} stats to Kafka".format(name))
+        logger.debug(f"Export {name} stats to Kafka")
 
         # Create DB input
         data = dict(zip(columns, points))
         if self.tags is not None:
             data.update(self.parse_tags(self.tags))
 
         # Send stats to the kafka topic
@@ -80,16 +79,16 @@
             self.client.send(
                 self.topic,
                 # Kafka key name needs to be bytes #1593
                 key=name.encode('utf-8'),
                 value=data,
             )
         except Exception as e:
-            logger.error("Cannot export {} stats to Kafka ({})".format(name, e))
+            logger.error(f"Cannot export {name} stats to Kafka ({e})")
 
     def exit(self):
         """Close the Kafka export module."""
         # To ensure all connections are properly closed
         self.client.flush()
         self.client.close()
         # Call the father method
-        super(Export, self).exit()
+        super().exit()
```

### Comparing `glances-4.0.4/glances/exports/glances_mongodb/__init__.py` & `glances-4.0.5/glances/exports/glances_mongodb/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,33 +1,32 @@
-# -*- coding: utf-8 -*-
 #
 # This file is part of Glances.
 #
 # SPDX-FileCopyrightText: 2024 Nicolas Hennion <nicolas@nicolargo.com>
 #
 # SPDX-License-Identifier: LGPL-3.0-only
 #
 
 """MongoDB interface class."""
 
 import sys
-
-from glances.logger import logger
-from glances.exports.export import GlancesExport
+from urllib.parse import quote_plus
 
 import pymongo
-from urllib.parse import quote_plus
+
+from glances.exports.export import GlancesExport
+from glances.logger import logger
 
 
 class Export(GlancesExport):
     """This class manages the MongoDB export module."""
 
     def __init__(self, config=None, args=None):
         """Init the MongoDB export IF."""
-        super(Export, self).__init__(config=config, args=args)
+        super().__init__(config=config, args=args)
 
         # Mandatory configuration keys (additional to host and port)
         self.db = None
 
         # Optional configuration keys
         self.user = None
         self.password = None
@@ -41,36 +40,36 @@
         self.client = self.init()
 
     def init(self):
         """Init the connection to the CouchDB server."""
         if not self.export_enable:
             return None
 
-        server_uri = 'mongodb://%s:%s@%s:%s' % (quote_plus(self.user), quote_plus(self.password), self.host, self.port)
+        server_uri = f'mongodb://{quote_plus(self.user)}:{quote_plus(self.password)}@{self.host}:{self.port}'
 
         try:
             client = pymongo.MongoClient(server_uri)
             client.admin.command('ping')
         except Exception as e:
-            logger.critical("Cannot connect to MongoDB server %s:%s (%s)" % (self.host, self.port, e))
+            logger.critical(f"Cannot connect to MongoDB server {self.host}:{self.port} ({e})")
             sys.exit(2)
         else:
             logger.info("Connected to the MongoDB server")
 
         return client
 
     def database(self):
         """Return the CouchDB database object"""
         return self.client[self.db]
 
     def export(self, name, columns, points):
         """Write the points to the MongoDB server."""
-        logger.debug("Export {} stats to MongoDB".format(name))
+        logger.debug(f"Export {name} stats to MongoDB")
 
         # Create DB input
         data = dict(zip(columns, points))
 
         # Write data to the MongoDB database
         try:
             self.database()[name].insert_one(data)
         except Exception as e:
-            logger.error("Cannot export {} stats to MongoDB ({})".format(name, e))
+            logger.error(f"Cannot export {name} stats to MongoDB ({e})")
```

### Comparing `glances-4.0.4/glances/exports/glances_mqtt/__init__.py` & `glances-4.0.5/glances/exports/glances_mqtt/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,37 +1,36 @@
-# -*- coding: utf-8 -*-
 #
 # This file is part of Glances.
 #
 # SPDX-FileCopyrightText: 2022 Nicolas Hennion <nicolas@nicolargo.com>
 #
 # SPDX-License-Identifier: LGPL-3.0-only
 #
 
 """MQTT interface class."""
 
 import socket
 import string
 import sys
 
-from glances.logger import logger
-from glances.exports.export import GlancesExport
-from glances.globals import json_dumps
-
 # Import paho for MQTT
 import certifi
 import paho.mqtt.client as paho
 
+from glances.exports.export import GlancesExport
+from glances.globals import json_dumps
+from glances.logger import logger
+
 
 class Export(GlancesExport):
     """This class manages the MQTT export module."""
 
     def __init__(self, config=None, args=None):
         """Init the MQTT export IF."""
-        super(Export, self).__init__(config=config, args=args)
+        super().__init__(config=config, args=args)
 
         # Mandatory configuration keys (additional to host and port)
         self.user = None
         self.password = None
         self.topic = None
         self.tls = 'true'
 
@@ -83,15 +82,15 @@
             client.username_pw_set(username=self.user, password=self.password)
             if self.tls:
                 client.tls_set(certifi.where())
             client.connect(host=self.host, port=self.port)
             client.loop_start()
             return client
         except Exception as e:
-            logger.critical("Connection to MQTT server %s:%s failed with error: %s " % (self.host, self.port, e))
+            logger.critical(f"Connection to MQTT server {self.host}:{self.port} failed with error: {e} ")
             return None
 
     def export(self, name, columns, points):
         """Write the points in MQTT."""
 
         WHITELIST = '_-' + string.ascii_letters + string.digits
         SUBSTITUTE = '_'
@@ -105,32 +104,32 @@
                     sensor = [whitelisted(name) for name in sensor.split('.')]
                     to_export = [self.topic, self.devicename, name]
                     to_export.extend(sensor)
                     topic = '/'.join(to_export)
 
                     self.client.publish(topic, value)
                 except Exception as e:
-                    logger.error("Can not export stats to MQTT server (%s)" % e)
+                    logger.error(f"Can not export stats to MQTT server ({e})")
         elif self.topic_structure == 'per-plugin':
             try:
                 topic = '/'.join([self.topic, self.devicename, name])
                 sensor_values = dict(zip(columns, points))
 
                 # Build the value to output
-                output_value = dict()
+                output_value = {}
                 for key in sensor_values:
                     split_key = key.split('.')
 
                     # Add the parent keys if they don't exist
                     current_level = output_value
                     for depth in range(len(split_key) - 1):
                         if split_key[depth] not in current_level:
-                            current_level[split_key[depth]] = dict()
+                            current_level[split_key[depth]] = {}
                         current_level = current_level[split_key[depth]]
 
                     # Add the value
                     current_level[split_key[len(split_key) - 1]] = sensor_values[key]
 
                 json_value = json_dumps(output_value)
                 self.client.publish(topic, json_value)
             except Exception as e:
-                logger.error("Can not export stats to MQTT server (%s)" % e)
+                logger.error(f"Can not export stats to MQTT server ({e})")
```

### Comparing `glances-4.0.4/glances/exports/glances_opentsdb/__init__.py` & `glances-4.0.5/glances/exports/glances_opentsdb/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,33 +1,32 @@
-# -*- coding: utf-8 -*-
 #
 # This file is part of Glances.
 #
 # SPDX-FileCopyrightText: 2022 Nicolas Hennion <nicolas@nicolargo.com>
 #
 # SPDX-License-Identifier: LGPL-3.0-only
 #
 
 """OpenTSDB interface class."""
 
 import sys
 from numbers import Number
 
-from glances.logger import logger
-from glances.exports.export import GlancesExport
-
 import potsdb
 
+from glances.exports.export import GlancesExport
+from glances.logger import logger
+
 
 class Export(GlancesExport):
     """This class manages the OpenTSDB export module."""
 
     def __init__(self, config=None, args=None):
         """Init the OpenTSDB export IF."""
-        super(Export, self).__init__(config=config, args=args)
+        super().__init__(config=config, args=args)
 
         # Mandatory configuration keys (additional to host and port)
         # N/A
 
         # Optionals configuration keys
         self.prefix = None
         self.tags = None
@@ -48,32 +47,32 @@
         """Init the connection to the OpenTSDB server."""
         if not self.export_enable:
             return None
 
         try:
             db = potsdb.Client(self.host, port=int(self.port), check_host=True)
         except Exception as e:
-            logger.critical("Cannot connect to OpenTSDB server %s:%s (%s)" % (self.host, self.port, e))
+            logger.critical(f"Cannot connect to OpenTSDB server {self.host}:{self.port} ({e})")
             sys.exit(2)
 
         return db
 
     def export(self, name, columns, points):
         """Export the stats to the Statsd server."""
         for i in range(len(columns)):
             if not isinstance(points[i], Number):
                 continue
-            stat_name = '{}.{}.{}'.format(self.prefix, name, columns[i])
+            stat_name = f'{self.prefix}.{name}.{columns[i]}'
             stat_value = points[i]
             tags = self.parse_tags(self.tags)
             try:
                 self.client.send(stat_name, stat_value, **tags)
             except Exception as e:
-                logger.error("Can not export stats %s to OpenTSDB (%s)" % (name, e))
-        logger.debug("Export {} stats to OpenTSDB".format(name))
+                logger.error(f"Can not export stats {name} to OpenTSDB ({e})")
+        logger.debug(f"Export {name} stats to OpenTSDB")
 
     def exit(self):
         """Close the OpenTSDB export module."""
         # Waits for all outstanding metrics to be sent and background thread closes
         self.client.wait()
         # Call the father method
-        super(Export, self).exit()
+        super().exit()
```

### Comparing `glances-4.0.4/glances/exports/glances_prometheus/__init__.py` & `glances-4.0.5/glances/exports/glances_prometheus/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,36 +1,35 @@
-# -*- coding: utf-8 -*-
 #
 # This file is part of Glances.
 #
 # SPDX-FileCopyrightText: 2022 Nicolas Hennion <nicolas@nicolargo.com>
 #
 # SPDX-License-Identifier: LGPL-3.0-only
 #
 
 """Prometheus interface class."""
 
 import sys
 from numbers import Number
 
-from glances.logger import logger
+from prometheus_client import Gauge, start_http_server
+
 from glances.exports.export import GlancesExport
 from glances.globals import iteritems, listkeys
-
-from prometheus_client import start_http_server, Gauge
+from glances.logger import logger
 
 
 class Export(GlancesExport):
     """This class manages the Prometheus export module."""
 
     METRIC_SEPARATOR = '_'
 
     def __init__(self, config=None, args=None):
         """Init the Prometheus export IF."""
-        super(Export, self).__init__(config=config, args=args)
+        super().__init__(config=config, args=args)
 
         # Load the Prometheus configuration file section
         self.export_enable = self.load_conf('prometheus', mandatories=['host', 'port', 'labels'], options=['prefix'])
         if not self.export_enable:
             exit('Missing PROMETHEUS config')
 
         # Optionals configuration keys
@@ -48,22 +47,22 @@
         self.init()
 
     def init(self):
         """Init the Prometheus Exporter"""
         try:
             start_http_server(port=int(self.port), addr=self.host)
         except Exception as e:
-            logger.critical("Can not start Prometheus exporter on {}:{} ({})".format(self.host, self.port, e))
+            logger.critical(f"Can not start Prometheus exporter on {self.host}:{self.port} ({e})")
             sys.exit(2)
         else:
-            logger.info("Start Prometheus exporter on {}:{}".format(self.host, self.port))
+            logger.info(f"Start Prometheus exporter on {self.host}:{self.port}")
 
     def export(self, name, columns, points):
         """Write the points to the Prometheus exporter using Gauge."""
-        logger.debug("Export {} stats to Prometheus exporter".format(name))
+        logger.debug(f"Export {name} stats to Prometheus exporter")
 
         # Remove non number stats and convert all to float (for Boolean)
         data = {k: float(v) for (k, v) in iteritems(dict(zip(columns, points))) if isinstance(v, Number)}
 
         # Write metrics to the Prometheus exporter
         for k, v in iteritems(data):
             # Prometheus metric name: prefix_<glances stats name>
```

### Comparing `glances-4.0.4/glances/exports/glances_rabbitmq/__init__.py` & `glances-4.0.5/glances/exports/glances_rabbitmq/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 #
 # This file is part of Glances.
 #
 # SPDX-FileCopyrightText: 2022 Nicolas Hennion <nicolas@nicolargo.com>
 #
 # SPDX-License-Identifier: LGPL-3.0-only
 #
@@ -10,27 +9,27 @@
 """JMS interface class."""
 
 import datetime
 import socket
 import sys
 from numbers import Number
 
-from glances.logger import logger
-from glances.exports.export import GlancesExport
-
 # Import pika for RabbitMQ
 import pika
 
+from glances.exports.export import GlancesExport
+from glances.logger import logger
+
 
 class Export(GlancesExport):
     """This class manages the rabbitMQ export module."""
 
     def __init__(self, config=None, args=None):
         """Init the RabbitMQ export IF."""
-        super(Export, self).__init__(config=config, args=args)
+        super().__init__(config=config, args=args)
 
         # Mandatory configuration keys (additional to host and port)
         self.user = None
         self.password = None
         self.queue = None
         self.protocol = None
 
@@ -63,26 +62,25 @@
             self.protocol = 'amqp'
 
         try:
             parameters = pika.URLParameters(
                 self.protocol + '://' + self.user + ':' + self.password + '@' + self.host + ':' + self.port + '/'
             )
             connection = pika.BlockingConnection(parameters)
-            channel = connection.channel()
-            return channel
+            return connection.channel()
         except Exception as e:
-            logger.critical("Connection to rabbitMQ server %s:%s failed. %s" % (self.host, self.port, e))
+            logger.critical(f"Connection to rabbitMQ server {self.host}:{self.port} failed. {e}")
             sys.exit(2)
 
     def export(self, name, columns, points):
         """Write the points in RabbitMQ."""
         data = 'hostname=' + self.hostname + ', name=' + name + ', dateinfo=' + datetime.datetime.utcnow().isoformat()
         for i in range(len(columns)):
             if not isinstance(points[i], Number):
                 continue
-            else:
-                data += ", " + columns[i] + "=" + str(points[i])
+            data += ", " + columns[i] + "=" + str(points[i])
+
         logger.debug(data)
         try:
             self.client.basic_publish(exchange='', routing_key=self.queue, body=data)
         except Exception as e:
-            logger.error("Can not export stats to RabbitMQ (%s)" % e)
+            logger.error(f"Can not export stats to RabbitMQ ({e})")
```

### Comparing `glances-4.0.4/glances/exports/glances_restful/__init__.py` & `glances-4.0.5/glances/exports/glances_restful/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,33 +1,31 @@
-# -*- coding: utf-8 -*-
 #
 # This file is part of Glances.
 #
 # SPDX-FileCopyrightText: 2022 Nicolas Hennion <nicolas@nicolargo.com>
 #
 # SPDX-License-Identifier: LGPL-3.0-only
 #
 
 """RESTful interface class."""
 
+from requests import post
 
+from glances.exports.export import GlancesExport
 from glances.globals import listkeys
 from glances.logger import logger
-from glances.exports.export import GlancesExport
-
-from requests import post
 
 
 class Export(GlancesExport):
     """This class manages the RESTful export module.
     Be aware that stats will be exported in one big POST request"""
 
     def __init__(self, config=None, args=None):
         """Init the RESTful export IF."""
-        super(Export, self).__init__(config=config, args=args)
+        super().__init__(config=config, args=args)
 
         # Mandatory configuration keys (additional to host and port)
         self.protocol = None
         self.path = None
 
         # Load the RESTful section in the configuration file
         self.export_enable = self.load_conf('restful', mandatories=['host', 'port', 'protocol', 'path'])
@@ -42,23 +40,23 @@
         self.client = self.init()
 
     def init(self):
         """Init the connection to the RESTful server."""
         if not self.export_enable:
             return None
         # Build the RESTful URL where the stats will be posted
-        url = '{}://{}:{}{}'.format(self.protocol, self.host, self.port, self.path)
-        logger.info("Stats will be exported to the RESTful endpoint {}".format(url))
+        url = f'{self.protocol}://{self.host}:{self.port}{self.path}'
+        logger.info(f"Stats will be exported to the RESTful endpoint {url}")
         return url
 
     def export(self, name, columns, points):
         """Export the stats to the Statsd server."""
         if name == self.last_exported_list()[0] and self.buffer != {}:
             # One complete loop have been done
-            logger.debug("Export stats ({}) to RESTful endpoint ({})".format(listkeys(self.buffer), self.client))
+            logger.debug(f"Export stats ({listkeys(self.buffer)}) to RESTful endpoint ({self.client})")
             # Export stats
             post(self.client, json=self.buffer, allow_redirects=True)
             # Reset buffer
             self.buffer = {}
 
         # Add current stat to the buffer
         self.buffer[name] = dict(zip(columns, points))
```

### Comparing `glances-4.0.4/glances/exports/glances_riemann/__init__.py` & `glances-4.0.5/glances/exports/glances_riemann/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,34 +1,33 @@
-# -*- coding: utf-8 -*-
 #
 # This file is part of Glances.
 #
 # SPDX-FileCopyrightText: 2022 Nicolas Hennion <nicolas@nicolargo.com>
 #
 # SPDX-License-Identifier: LGPL-3.0-only
 #
 
 """Riemann interface class."""
 
 import socket
 from numbers import Number
 
-from glances.logger import logger
-from glances.exports.export import GlancesExport
-
 # Import bernhard for Riemann
 import bernhard
 
+from glances.exports.export import GlancesExport
+from glances.logger import logger
+
 
 class Export(GlancesExport):
     """This class manages the Riemann export module."""
 
     def __init__(self, config=None, args=None):
         """Init the Riemann export IF."""
-        super(Export, self).__init__(config=config, args=args)
+        super().__init__(config=config, args=args)
 
         # Mandatory configuration keys (additional to host and port)
         # N/A
 
         # Optional configuration keys
         # N/A
 
@@ -44,25 +43,24 @@
         self.client = self.init()
 
     def init(self):
         """Init the connection to the Riemann server."""
         if not self.export_enable:
             return None
         try:
-            client = bernhard.Client(host=self.host, port=self.port)
-            return client
+            return bernhard.Client(host=self.host, port=self.port)
         except Exception as e:
-            logger.critical("Connection to Riemann failed : %s " % e)
+            logger.critical(f"Connection to Riemann failed : {e} ")
             return None
 
     def export(self, name, columns, points):
         """Write the points in Riemann."""
         for i in range(len(columns)):
             if not isinstance(points[i], Number):
                 continue
-            else:
-                data = {'host': self.hostname, 'service': name + " " + columns[i], 'metric': points[i]}
-                logger.debug(data)
-                try:
-                    self.client.send(data)
-                except Exception as e:
-                    logger.error("Cannot export stats to Riemann (%s)" % e)
+
+            data = {'host': self.hostname, 'service': name + " " + columns[i], 'metric': points[i]}
+            logger.debug(data)
+            try:
+                self.client.send(data)
+            except Exception as e:
+                logger.error(f"Cannot export stats to Riemann ({e})")
```

### Comparing `glances-4.0.4/glances/exports/glances_statsd/__init__.py` & `glances-4.0.5/glances/exports/glances_statsd/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,32 +1,31 @@
-# -*- coding: utf-8 -*-
 #
 # This file is part of Glances.
 #
 # SPDX-FileCopyrightText: 2022 Nicolas Hennion <nicolas@nicolargo.com>
 #
 # SPDX-License-Identifier: LGPL-3.0-only
 #
 
 """Statsd interface class."""
 
 from numbers import Number
 
-from glances.logger import logger
-from glances.exports.export import GlancesExport
-
 from statsd import StatsClient
 
+from glances.exports.export import GlancesExport
+from glances.logger import logger
+
 
 class Export(GlancesExport):
     """This class manages the Statsd export module."""
 
     def __init__(self, config=None, args=None):
         """Init the Statsd export IF."""
-        super(Export, self).__init__(config=config, args=args)
+        super().__init__(config=config, args=args)
 
         # Mandatory configuration keys (additional to host and port)
         # N/A
 
         # Optional configuration keys
         self.prefix = None
 
@@ -42,33 +41,31 @@
         # Init the Statsd client
         self.client = self.init()
 
     def init(self):
         """Init the connection to the Statsd server."""
         if not self.export_enable:
             return None
-        logger.info("Stats will be exported to StatsD server: {}:{}".format(self.host, self.port))
+        logger.info(f"Stats will be exported to StatsD server: {self.host}:{self.port}")
         return StatsClient(self.host, int(self.port), prefix=self.prefix)
 
     def export(self, name, columns, points):
         """Export the stats to the Statsd server."""
         for i in range(len(columns)):
             if not isinstance(points[i], Number):
                 continue
-            stat_name = '{}.{}'.format(name, columns[i])
+            stat_name = f'{name}.{columns[i]}'
             stat_value = points[i]
             try:
                 self.client.gauge(normalize(stat_name), stat_value)
             except Exception as e:
-                logger.error("Can not export stats to Statsd (%s)" % e)
-        logger.debug("Export {} stats to Statsd".format(name))
+                logger.error(f"Can not export stats to Statsd ({e})")
+        logger.debug(f"Export {name} stats to Statsd")
 
 
 def normalize(name):
     """Normalize name for the Statsd convention"""
 
     # Name should not contain some specials chars (issue #1068)
     ret = name.replace(':', '')
     ret = ret.replace('%', '')
-    ret = ret.replace(' ', '_')
-
-    return ret
+    return ret.replace(' ', '_')
```

### Comparing `glances-4.0.4/glances/exports/glances_zeromq/__init__.py` & `glances-4.0.5/glances/exports/glances_zeromq/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,35 +1,33 @@
-# -*- coding: utf-8 -*-
 #
 # This file is part of Glances.
 #
 # SPDX-FileCopyrightText: 2022 Nicolas Hennion <nicolas@nicolargo.com>
 #
 # SPDX-License-Identifier: LGPL-3.0-only
 #
 
 """ZeroMQ interface class."""
 
 import sys
 
-from glances.globals import b
-from glances.logger import logger
-from glances.exports.export import GlancesExport
-from glances.globals import json_dumps
-
 import zmq
 from zmq.utils.strtypes import asbytes
 
+from glances.exports.export import GlancesExport
+from glances.globals import b, json_dumps
+from glances.logger import logger
+
 
 class Export(GlancesExport):
     """This class manages the ZeroMQ export module."""
 
     def __init__(self, config=None, args=None):
         """Init the ZeroMQ export IF."""
-        super(Export, self).__init__(config=config, args=args)
+        super().__init__(config=config, args=args)
 
         # Mandatory configuration keys (additional to host and port)
         self.prefix = None
 
         # Optionals configuration keys
         # N/A
 
@@ -43,38 +41,38 @@
         self.client = self.init()
 
     def init(self):
         """Init the connection to the CouchDB server."""
         if not self.export_enable:
             return None
 
-        server_uri = 'tcp://{}:{}'.format(self.host, self.port)
+        server_uri = f'tcp://{self.host}:{self.port}'
 
         try:
             self.context = zmq.Context()
             publisher = self.context.socket(zmq.PUB)
             publisher.bind(server_uri)
         except Exception as e:
-            logger.critical("Cannot connect to ZeroMQ server %s (%s)" % (server_uri, e))
+            logger.critical(f"Cannot connect to ZeroMQ server {server_uri} ({e})")
             sys.exit(2)
         else:
-            logger.info("Connected to the ZeroMQ server %s" % server_uri)
+            logger.info(f"Connected to the ZeroMQ server {server_uri}")
 
         return publisher
 
     def exit(self):
         """Close the socket and context"""
         if self.client is not None:
             self.client.close()
         if self.context is not None:
             self.context.destroy()
 
     def export(self, name, columns, points):
         """Write the points to the ZeroMQ server."""
-        logger.debug("Export {} stats to ZeroMQ".format(name))
+        logger.debug(f"Export {name} stats to ZeroMQ")
 
         # Create DB input
         data = dict(zip(columns, points))
 
         # Do not publish empty stats
         if data == {}:
             return False
@@ -86,10 +84,10 @@
         message = [b(self.prefix), b(name), asbytes(json_dumps(data))]
 
         # Write data to the ZeroMQ bus
         # Result can be view: tcp://host:port
         try:
             self.client.send_multipart(message)
         except Exception as e:
-            logger.error("Cannot export {} stats to ZeroMQ ({})".format(name, e))
+            logger.error(f"Cannot export {name} stats to ZeroMQ ({e})")
 
         return True
```

### Comparing `glances-4.0.4/glances/filter.py` & `glances-4.0.5/glances/filter.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,21 @@
-# -*- coding: utf-8 -*-
 #
 # This file is part of Glances.
 #
 # SPDX-FileCopyrightText: 2022 Nicolas Hennion <nicolas@nicolargo.com>
 #
 # SPDX-License-Identifier: LGPL-3.0-only
 #
 
 import re
 
 from glances.logger import logger
 
 
-class GlancesFilterList(object):
+class GlancesFilterList:
     """Manage a lis of GlancesFilter objects
 
     >>> fl = GlancesFilterList()
     >>> fl.filter = '.*python.*,user:nicolargo'
     >>> fl.is_filtered({'name': 'python is in the place'})
     True
     >>> fl.is_filtered({'name': 'snake is in the place'})
@@ -51,15 +50,15 @@
         """Return True if the process is filtered by at least one filter"""
         for f in self._filter:
             if f.is_filtered(process):
                 return True
         return False
 
 
-class GlancesFilter(object):
+class GlancesFilter:
     """Allow Glances to filter processes
 
     >>> f = GlancesFilter()
     >>> f.filter = '.*python.*'
     >>> f.filter
     '.*python.*'
     >>> f.filter_key
@@ -123,17 +122,17 @@
         if self.filter is not None:
             logger.debug(
                 "Set filter to {} on {}".format(self.filter, self.filter_key if self.filter_key else 'name or cmdline')
             )
             # Compute the regular expression
             try:
                 self._filter_re = re.compile(self.filter)
-                logger.debug("Filter regex compilation OK: {}".format(self.filter))
+                logger.debug(f"Filter regex compilation OK: {self.filter}")
             except Exception as e:
-                logger.error("Cannot compile filter regex: {} ({})".format(self.filter, e))
+                logger.error(f"Cannot compile filter regex: {self.filter} ({e})")
                 self._filter = None
                 self._filter_re = None
                 self._filter_key = None
 
     @property
     def filter_re(self):
         """Return the filter regular expression"""
@@ -152,17 +151,17 @@
         if self.filter is None:
             # No filter => Not filtered
             return False
 
         if self.filter_key is None:
             # Apply filter on command line and process name
             return self._is_process_filtered(process, key='name') or self._is_process_filtered(process, key='cmdline')
-        else:
-            # Apply filter on <key>
-            return self._is_process_filtered(process)
+
+        # Apply filter on <key>
+        return self._is_process_filtered(process)
 
     def _is_process_filtered(self, process, key=None):
         """Return True if the process[key] should be filtered according to the current filter"""
         if key is None:
             key = self.filter_key
         try:
             # If the item process[key] is a list, convert it to a string
```

### Comparing `glances-4.0.4/glances/folder_list.py` & `glances-4.0.5/glances/folder_list.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,26 +1,23 @@
-# -*- coding: utf-8 -*-
 #
 # This file is part of Glances.
 #
 # SPDX-FileCopyrightText: 2024 Nicolas Hennion <nicolas@nicolargo.com>
 #
 # SPDX-License-Identifier: LGPL-3.0-only
 #
 
 """Manage the folder list."""
-from __future__ import unicode_literals
 
-
-from glances.timer import Timer
-from glances.globals import nativestr, folder_size
+from glances.globals import folder_size, nativestr
 from glances.logger import logger
+from glances.timer import Timer
 
 
-class FolderList(object):
+class FolderList:
     """This class describes the optional monitored folder list.
 
     The folder list is a list of 'important' folder to monitor.
 
     The list (Python list) is composed of items (Python dict).
     An item is defined (dict keys):
     * path: Path to the folder
@@ -63,16 +60,15 @@
             key = 'folder_' + str(line) + '_'
 
             # Path is mandatory
             value['indice'] = str(line)
             value['path'] = self.config.get_value(section, key + 'path')
             if value['path'] is None:
                 continue
-            else:
-                value['path'] = nativestr(value['path'])
+            value['path'] = nativestr(value['path'])
 
             # Optional conf keys
             # Refresh time
             value['refresh'] = int(self.config.get_value(section, key + 'refresh', default=self.__default_refresh))
             self.timer_folders.append(Timer(value['refresh']))
             # Thresholds
             for i in ['careful', 'warning', 'critical']:
```

### Comparing `glances-4.0.4/glances/globals.py` & `glances-4.0.5/glances/globals.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,45 +1,43 @@
-# -*- coding: utf-8 -*-
+# ruff: noqa: F401
 #
 # This file is part of Glances.
 #
 # SPDX-FileCopyrightText: 2024 Nicolas Hennion <nicolas@nicolargo.com>
 #
 # SPDX-License-Identifier: LGPL-3.0-only
 #
 
 """Common objects shared by all Glances modules."""
 
 ################
 # GLOBAL IMPORTS
 ################
 
+import base64
 import errno
+import functools
 import os
-import sys
 import platform
-import ujson
-from operator import itemgetter, methodcaller
-import unicodedata
-import types
-import subprocess
-from datetime import datetime
+import queue
 import re
-import base64
-import functools
+import subprocess
+import sys
 import weakref
-
-import queue
 from configparser import ConfigParser, NoOptionError, NoSectionError
+from datetime import datetime
+from operator import itemgetter, methodcaller
 from statistics import mean
-from xmlrpc.client import Fault, ProtocolError, ServerProxy, Transport, Server
-from xmlrpc.server import SimpleXMLRPCRequestHandler, SimpleXMLRPCServer
-from urllib.request import urlopen, Request
 from urllib.error import HTTPError, URLError
 from urllib.parse import urlparse
+from urllib.request import Request, urlopen
+from xmlrpc.client import Fault, ProtocolError, Server, ServerProxy, Transport
+from xmlrpc.server import SimpleXMLRPCRequestHandler, SimpleXMLRPCServer
+
+import ujson
 
 # Correct issue #1025 by monkey path the xmlrpc lib
 from defusedxml.xmlrpc import monkey_patch
 
 monkey_patch()
 
 ##############
@@ -132,26 +130,25 @@
         return s
     return s.encode('utf-8', errors=errors)
 
 
 def nativestr(s, errors='replace'):
     if isinstance(s, text_type):
         return s
-    elif isinstance(s, (int, float)):
+    if isinstance(s, (int, float)):
         return s.__str__()
-    else:
-        return s.decode('utf-8', errors=errors)
+    return s.decode('utf-8', errors=errors)
 
 
 def system_exec(command):
     """Execute a system command and return the result as a str"""
     try:
         res = subprocess.run(command.split(' '), stdout=subprocess.PIPE).stdout.decode('utf-8')
     except Exception as e:
-        res = 'ERROR: {}'.format(e)
+        res = f'ERROR: {e}'
     return res.rstrip()
 
 
 def subsample(data, sampling):
     """Compute a simple mean subsampling.
 
     Data should be a list of numerical itervalues
@@ -200,15 +197,15 @@
         import ctypes
         import traceback
 
         # WARNING: requires Windows XP SP2 or higher!
         try:
             return ctypes.windll.shell32.IsUserAnAdmin()
         except Exception as e:
-            print("Admin check failed with error: %s" % e)
+            print(f"Admin check failed with error: {e}")
             traceback.print_exc()
             return False
     else:
         # Check for root on Posix
         return os.getuid() == 0
 
 
@@ -297,15 +294,15 @@
 
 
 def urlopen_auth(url, username, password):
     """Open a url with basic auth"""
     return urlopen(
         Request(
             url,
-            headers={'Authorization': 'Basic ' + base64.b64encode(('%s:%s' % (username, password)).encode()).decode()},
+            headers={'Authorization': 'Basic ' + base64.b64encode((f'{username}:{password}').encode()).decode()},
         )
     )
 
 
 def json_dumps(data):
     """Return the object data in a JSON format.
 
@@ -335,16 +332,15 @@
         return None
 
 
 def json_dumps_dictlist(data, item):
     dl = dictlist(data, item)
     if dl is None:
         return None
-    else:
-        return json_dumps(dl)
+    return json_dumps(dl)
 
 
 def string_value_to_float(s):
     """Convert a string with a value and an unit to a float.
     Example:
     '12.5 MB' -> 12500000.0
     '32.5 GB' -> 32500000000.0
```

### Comparing `glances-4.0.4/glances/history.py` & `glances-4.0.5/glances/history.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,21 @@
-# -*- coding: utf-8 -*-
 #
 # This file is part of Glances.
 #
 # SPDX-FileCopyrightText: 2022 Nicolas Hennion <nicolas@nicolargo.com>
 #
 # SPDX-License-Identifier: LGPL-3.0-only
 #
 
 """Manage stats history"""
 
 from glances.attribute import GlancesAttribute
 
 
-class GlancesHistory(object):
+class GlancesHistory:
     """This class manage a dict of GlancesAttribute
     - key: stats name
     - value: GlancesAttribute"""
 
     def __init__(self):
         """
         items_history_list: list of stats to historized (define inside plugins)
```

### Comparing `glances-4.0.4/glances/logger.py` & `glances-4.0.5/glances/logger.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,23 @@
-# -*- coding: utf-8 -*-
 #
 # This file is part of Glances.
 #
 # SPDX-FileCopyrightText: 2022 Nicolas Hennion <nicolas@nicolargo.com>
 #
 # SPDX-License-Identifier: LGPL-3.0-only
 #
 
 """Custom logger class."""
 
-import os
-import json
 import getpass
-import tempfile
-
+import json
 import logging
 import logging.config
+import os
+import tempfile
 
 from glances.globals import safe_makedirs
 
 # Choose the good place for the log file (see issue #1575)
 # Default root path
 if 'HOME' in os.environ:
     _XDG_CACHE_HOME = os.path.join(os.environ['HOME'], '.local', 'share')
@@ -33,15 +31,15 @@
 ):
     safe_makedirs(os.path.join(os.environ['XDG_CACHE_HOME'], 'glances'))
     LOG_FILENAME = os.path.join(os.environ['XDG_CACHE_HOME'], 'glances', 'glances.log')
 elif os.path.isdir(_XDG_CACHE_HOME) and os.access(_XDG_CACHE_HOME, os.W_OK):
     safe_makedirs(os.path.join(_XDG_CACHE_HOME, 'glances'))
     LOG_FILENAME = os.path.join(_XDG_CACHE_HOME, 'glances', 'glances.log')
 else:
-    LOG_FILENAME = os.path.join(tempfile.gettempdir(), 'glances-{}.log'.format(getpass.getuser()))
+    LOG_FILENAME = os.path.join(tempfile.gettempdir(), f'glances-{getpass.getuser()}.log')
 
 # Define the logging configuration
 LOGGING_CFG = {
     "version": 1,
     "disable_existing_loggers": "False",
     "root": {"level": "INFO", "handlers": ["file", "console"]},
     "formatters": {
@@ -85,15 +83,15 @@
     # By default, use the LOGGING_CFG logger configuration
     config = LOGGING_CFG
 
     # Check if a specific configuration is available
     user_file = os.getenv(env_key, None)
     if user_file and os.path.exists(user_file):
         # A user file as been defined. Use it...
-        with open(user_file, 'rt') as f:
+        with open(user_file) as f:
             config = json.load(f)
 
     # Load the configuration
     logging.config.dictConfig(config)
 
     return _logger
```

### Comparing `glances-4.0.4/glances/main.py` & `glances-4.0.5/glances/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 #
 # This file is part of Glances.
 #
 # SPDX-FileCopyrightText: 2024 Nicolas Hennion <nicolas@nicolargo.com>
 #
 # SPDX-License-Identifier: LGPL-3.0-only
 #
@@ -11,22 +10,22 @@
 
 import argparse
 import sys
 import tempfile
 from logging import DEBUG
 from warnings import simplefilter
 
-from glances import __version__, psutil_version, __apiversion__
-from glances.globals import WINDOWS, disable, enable
+from glances import __apiversion__, __version__, psutil_version
 from glances.config import Config
+from glances.globals import WINDOWS, disable, enable
+from glances.logger import LOG_FILENAME, logger
 from glances.processes import sort_processes_key_list
-from glances.logger import logger, LOG_FILENAME
 
 
-class GlancesMain(object):
+class GlancesMain:
     """Main class to manage Glances instance."""
 
     # Default stats' minimum refresh time is 2 seconds
     DEFAULT_REFRESH_TIME = 2
     # Set the default cache lifetime to 1 second (only for server)
     cached_time = 1
     # By default, Glances is ran in standalone mode (no client/server)
@@ -97,18 +96,18 @@
     def __init__(self):
         """Manage the command line arguments."""
         # Read the command line arguments
         self.args = self.parse_args()
 
     def version_msg(self):
         """Return the version message."""
-        version = 'Glances version:\t{}\n'.format(__version__)
-        version += 'Glances API version:\t{}\n'.format(__apiversion__)
-        version += 'PsUtil version:\t\t{}\n'.format(psutil_version)
-        version += 'Log file:\t\t{}\n'.format(LOG_FILENAME)
+        version = f'Glances version:\t{__version__}\n'
+        version += f'Glances API version:\t{__apiversion__}\n'
+        version += f'PsUtil version:\t\t{psutil_version}\n'
+        version += f'Log file:\t\t{LOG_FILENAME}\n'
         return version
 
     def init_args(self):
         """Init all the command line arguments."""
         parser = argparse.ArgumentParser(
             prog='glances',
             conflict_handler='resolve',
@@ -237,36 +236,36 @@
             action='store_true',
             default=False,
             dest='disable_bg',
             help='disable background colors in the terminal',
         )
         parser.add_argument(
             '--enable-irq', action='store_true', default=False, dest='enable_irq', help='enable IRQ module'
-        ),
+        )
         parser.add_argument(
             '--enable-process-extended',
             action='store_true',
             default=False,
             dest='enable_process_extended',
             help='enable extended stats on top process',
         )
         parser.add_argument(
             '--disable-separator',
             action='store_false',
             default=True,
             dest='enable_separator',
             help='disable separator in the UI (between top and others modules)',
-        ),
+        )
         parser.add_argument(
             '--disable-cursor',
             action='store_true',
             default=False,
             dest='disable_cursor',
             help='disable cursor (process selection) in the UI',
-        ),
+        )
         # Sort processes list
         parser.add_argument(
             '--sort-processes',
             dest='sort_processes_key',
             choices=sort_processes_key_list,
             help='Sort processes by: {}'.format(', '.join(sort_processes_key_list)),
         )
@@ -330,15 +329,15 @@
         )
         parser.add_argument(
             '-p',
             '--port',
             default=None,
             type=int,
             dest='port',
-            help='define the client/server TCP port [default: {}]'.format(self.server_port),
+            help=f'define the client/server TCP port [default: {self.server_port}]',
         )
         parser.add_argument(
             '-B',
             '--bind',
             default='0.0.0.0',
             dest='bind_address',
             help='bind server to the given IPv4/IPv6 address or hostname',
@@ -370,30 +369,30 @@
         )
         parser.add_argument(
             '-t',
             '--time',
             default=self.DEFAULT_REFRESH_TIME,
             type=float,
             dest='time',
-            help='set minimum refresh rate in seconds [default: {} sec]'.format(self.DEFAULT_REFRESH_TIME),
+            help=f'set minimum refresh rate in seconds [default: {self.DEFAULT_REFRESH_TIME} sec]',
         )
         parser.add_argument(
             '-w',
             '--webserver',
             action='store_true',
             default=False,
             dest='webserver',
             help='run Glances in web server mode (FastAPI, Uvicorn, Jinja2 libs needed)',
         )
         parser.add_argument(
             '--cached-time',
             default=self.cached_time,
             type=int,
             dest='cached_time',
-            help='set the server cache time [default: {} sec]'.format(self.cached_time),
+            help=f'set the server cache time [default: {self.cached_time} sec]',
         )
         parser.add_argument(
             '--stop-after',
             default=None,
             type=int,
             dest='stop_after',
             help='stop Glances after n refresh',
@@ -573,23 +572,23 @@
         else:
             global_refresh = self.DEFAULT_REFRESH_TIME
 
         # The configuration key can be overwrite from the command line (-t <time>)
         if args.time == self.DEFAULT_REFRESH_TIME:
             args.time = global_refresh
 
-        logger.debug('Global refresh rate is set to {} seconds'.format(args.time))
+        logger.debug(f'Global refresh rate is set to {args.time} seconds')
 
     def init_plugins(self, args):
         """Init Glances plugins"""
         # Allow users to disable plugins from the glances.conf (issue #1378)
         for s in self.config.sections():
             if self.config.has_section(s) and (self.config.get_bool_value(s, 'disable', False)):
                 disable(args, s)
-                logger.debug('{} disabled by the configuration file'.format(s))
+                logger.debug(f'{s} disabled by the configuration file')
         # The configuration key can be overwrite from the command line
         if args and args.disable_plugin and 'all' in args.disable_plugin.split(','):
             if not args.enable_plugin:
                 logger.critical("'all' key in --disable-plugin needs to be used with --enable-plugin")
                 sys.exit(2)
             else:
                 logger.info(
@@ -660,27 +659,27 @@
                 # Default user name is 'glances'
                 args.username = self.username
 
         if args.password_prompt or args.username_used:
             # Interactive or file password
             if args.server:
                 args.password = self.__get_password(
-                    description='Define the Glances server password ({} username): '.format(args.username),
+                    description=f'Define the Glances server password ({args.username} username): ',
                     confirm=True,
                     username=args.username,
                 )
             elif args.webserver:
                 args.password = self.__get_password(
-                    description='Define the Glances webserver password ({} username): '.format(args.username),
+                    description=f'Define the Glances webserver password ({args.username} username): ',
                     confirm=True,
                     username=args.username,
                 )
             elif args.client:
                 args.password = self.__get_password(
-                    description='Enter the Glances server password ({} username): '.format(args.username),
+                    description=f'Enter the Glances server password ({args.username} username): ',
                     clear=True,
                     username=args.username,
                 )
         else:
             # Default is no password
             args.password = self.password
```

### Comparing `glances-4.0.4/glances/outdated.py` & `glances-4.0.5/glances/outdated.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,78 +1,77 @@
-# -*- coding: utf-8 -*-
 #
 # This file is part of Glances.
 #
 # SPDX-FileCopyrightText: 2022 Nicolas Hennion <nicolas@nicolargo.com>
 #
 # SPDX-License-Identifier: LGPL-3.0-only
 #
 
 """Manage Glances update."""
 
-from datetime import datetime, timedelta
-import threading
 import json
-import pickle
 import os
+import pickle
+import threading
+from datetime import datetime, timedelta
 from ssl import CertificateError
 
 from glances import __version__
-from glances.globals import nativestr, urlopen, HTTPError, URLError, safe_makedirs
 from glances.config import user_cache_dir
+from glances.globals import HTTPError, URLError, nativestr, safe_makedirs, urlopen
 from glances.logger import logger
 
 try:
     from packaging.version import Version
 
     PACKAGING_IMPORT = True
 except Exception as e:
-    logger.warning("Unable to import 'packaging' module ({}). Glances cannot check for updates.".format(e))
+    logger.warning(f"Unable to import 'packaging' module ({e}). Glances cannot check for updates.")
     PACKAGING_IMPORT = False
 
 PYPI_API_URL = 'https://pypi.python.org/pypi/Glances/json'
 
 
-class Outdated(object):
+class Outdated:
     """
     This class aims at providing methods to warn the user when a new Glances
     version is available on the PyPI repository (https://pypi.python.org/pypi/Glances/).
     """
 
     def __init__(self, args, config):
         """Init the Outdated class"""
         self.args = args
         self.config = config
         self.cache_dir = user_cache_dir()[0]
         self.cache_file = os.path.join(self.cache_dir, 'glances-version.db')
 
         # Set default value...
-        self.data = {u'installed_version': __version__, u'latest_version': '0.0', u'refresh_date': datetime.now()}
+        self.data = {'installed_version': __version__, 'latest_version': '0.0', 'refresh_date': datetime.now()}
 
         # Disable update check if `packaging` is not installed
         if not PACKAGING_IMPORT:
             self.args.disable_check_update = True
 
         # Read the configuration file only if update check is not explicitly disabled
         if not self.args.disable_check_update:
             self.load_config(config)
 
-        logger.debug("Check Glances version up-to-date: {}".format(not self.args.disable_check_update))
+        logger.debug(f"Check Glances version up-to-date: {not self.args.disable_check_update}")
 
         # And update !
         self.get_pypi_version()
 
     def load_config(self, config):
         """Load outdated parameter in the global section of the configuration file."""
 
         global_section = 'global'
         if hasattr(config, 'has_section') and config.has_section(global_section):
             self.args.disable_check_update = config.get_value(global_section, 'check_update').lower() == 'false'
         else:
-            logger.debug("Cannot find section {} in the configuration file".format(global_section))
+            logger.debug(f"Cannot find section {global_section} in the configuration file")
             return False
 
         return True
 
     def installed_version(self):
         return self.data['installed_version']
 
@@ -106,29 +105,27 @@
 
     def is_outdated(self):
         """Return True if a new version is available"""
         if self.args.disable_check_update:
             # Check is disabled by configuration
             return False
 
-        logger.debug(
-            "Check Glances version (installed: {} / latest: {})".format(self.installed_version(), self.latest_version())
-        )
+        logger.debug(f"Check Glances version (installed: {self.installed_version()} / latest: {self.latest_version()})")
         return Version(self.latest_version()) > Version(self.installed_version())
 
     def _load_cache(self):
         """Load cache file and return cached data"""
         # If the cached file exist, read-it
         max_refresh_date = timedelta(days=7)
         cached_data = {}
         try:
             with open(self.cache_file, 'rb') as f:
                 cached_data = pickle.load(f)
         except Exception as e:
-            logger.debug("Cannot read version from cache file: {} ({})".format(self.cache_file, e))
+            logger.debug(f"Cannot read version from cache file: {self.cache_file} ({e})")
         else:
             logger.debug("Read version from cache file")
             if (
                 cached_data['installed_version'] != self.installed_version()
                 or datetime.now() - cached_data['refresh_date'] > max_refresh_date
             ):
                 # Reset the cache if:
@@ -143,29 +140,29 @@
         safe_makedirs(self.cache_dir)
 
         # Create/overwrite the cache file
         try:
             with open(self.cache_file, 'wb') as f:
                 pickle.dump(self.data, f)
         except Exception as e:
-            logger.error("Cannot write version to cache file {} ({})".format(self.cache_file, e))
+            logger.error(f"Cannot write version to cache file {self.cache_file} ({e})")
 
     def _update_pypi_version(self):
         """Get the latest PyPI version (as a string) via the RESTful JSON API"""
-        logger.debug("Get latest Glances version from the PyPI RESTful API ({})".format(PYPI_API_URL))
+        logger.debug(f"Get latest Glances version from the PyPI RESTful API ({PYPI_API_URL})")
 
         # Update the current time
-        self.data[u'refresh_date'] = datetime.now()
+        self.data['refresh_date'] = datetime.now()
 
         try:
             res = urlopen(PYPI_API_URL, timeout=3).read()
         except (HTTPError, URLError, CertificateError) as e:
-            logger.debug("Cannot get Glances version from the PyPI RESTful API ({})".format(e))
+            logger.debug(f"Cannot get Glances version from the PyPI RESTful API ({e})")
         else:
-            self.data[u'latest_version'] = json.loads(nativestr(res))['info']['version']
+            self.data['latest_version'] = json.loads(nativestr(res))['info']['version']
             logger.debug("Save Glances version to the cache file")
 
         # Save result to the cache file
         # Note: also saved if the Glances PyPI version cannot be grabbed
         self._save_cache()
 
         return self.data
```

### Comparing `glances-4.0.4/glances/outputs/glances_bars.py` & `glances-4.0.5/glances/outputs/glances_bars.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,21 @@
-# -*- coding: utf-8 -*-
 #
 # This file is part of Glances.
 #
 # SPDX-FileCopyrightText: 2022 Nicolas Hennion <nicolas@nicolargo.com>
 #
 # SPDX-License-Identifier: LGPL-3.0-only
 #
 
 """Manage bars for Glances output."""
 
-from __future__ import division
-
 from math import modf
 
 
-class Bar(object):
+class Bar:
     """Manage bar (progression or status).
 
     import sys
     import time
     b = Bar(10)
     for p in range(0, 100):
         b.percent = p
@@ -72,14 +69,15 @@
     @property
     def size(self, with_decoration=False):
         # Return the bar size, with or without decoration
         if with_decoration:
             return self.__size
         if self.__display_value:
             return self.__size - 6
+        return None
 
     @property
     def percent(self):
         return self.__percent
 
     @percent.setter
     def percent(self, value):
@@ -110,15 +108,15 @@
         # Add the value
         if self.__display_value:
             if self.percent >= self.max_value:
                 ret = '{} {}{:3.0f}{}'.format(
                     ret, '>' if self.percent > self.max_value else ' ', self.max_value, self.__unit_char
                 )
             else:
-                ret = '{}{:5.1f}{}'.format(ret, self.percent, self.__unit_char)
+                ret = f'{ret}{self.percent:5.1f}{self.__unit_char}'
 
         # Add overlay
         if overlay and len(overlay) < len(ret) - 6:
             ret = overlay + ret[len(overlay) :]
 
         return ret
```

### Comparing `glances-4.0.4/glances/outputs/glances_curses.py` & `glances-4.0.5/glances/outputs/glances_curses.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,42 +1,40 @@
-# -*- coding: utf-8 -*-
 #
 # This file is part of Glances.
 #
 # SPDX-FileCopyrightText: 2024 Nicolas Hennion <nicolas@nicolargo.com>
 #
 # SPDX-License-Identifier: LGPL-3.0-only
 #
 
 """Curses interface class."""
-from __future__ import unicode_literals
 
-import sys
 import getpass
+import sys
 
-from glances.globals import MACOS, WINDOWS, nativestr, u, itervalues, enable, disable
-from glances.logger import logger
 from glances.events_list import glances_events
-from glances.processes import glances_processes, sort_processes_key_list
+from glances.globals import MACOS, WINDOWS, disable, enable, itervalues, nativestr, u
+from glances.logger import logger
 from glances.outputs.glances_unicode import unicode_message
+from glances.processes import glances_processes, sort_processes_key_list
 from glances.timer import Timer
 
 # Import curses library for "normal" operating system
 try:
     import curses
     import curses.panel
     from curses.textpad import Textbox
 except ImportError:
     logger.critical("Curses module not found. Glances cannot start in standalone mode.")
     if WINDOWS:
         logger.critical("For Windows you can try installing windows-curses with pip install.")
     sys.exit(1)
 
 
-class _GlancesCurses(object):
+class _GlancesCurses:
     """This class manages the curses display (and key pressed).
 
     Note: It is a private class, use GlancesCursesClient or GlancesCursesBrowser.
     """
 
     _hotkeys = {
         '\n': {'handler': '_handle_enter'},
@@ -143,23 +141,23 @@
         # Init the curses screen
         try:
             self.screen = curses.initscr()
             if not self.screen:
                 logger.critical("Cannot init the curses library.\n")
                 sys.exit(1)
             else:
-                logger.debug("Curses library initialized with term: {}".format(curses.longname()))
+                logger.debug(f"Curses library initialized with term: {curses.longname()}")
         except Exception as e:
             if args.export:
                 logger.info("Cannot init the curses library, quiet mode on and export.")
                 args.quiet = True
                 return
-            else:
-                logger.critical("Cannot init the curses library ({})".format(e))
-                sys.exit(1)
+
+            logger.critical(f"Cannot init the curses library ({e})")
+            sys.exit(1)
 
         # Load configuration file
         self.load_config(config)
 
         # Init cursor
         self._init_cursor()
 
@@ -219,19 +217,19 @@
     def _init_colors(self):
         """Init the Curses color layout."""
 
         # Set curses options
         try:
             if hasattr(curses, 'start_color'):
                 curses.start_color()
-                logger.debug('Curses interface compatible with {} colors'.format(curses.COLORS))
+                logger.debug(f'Curses interface compatible with {curses.COLORS} colors')
             if hasattr(curses, 'use_default_colors'):
                 curses.use_default_colors()
         except Exception as e:
-            logger.warning('Error initializing terminal color ({})'.format(e))
+            logger.warning(f'Error initializing terminal color ({e})')
 
         # Init colors
         if self.args.disable_bold:
             A_BOLD = 0
             self.args.disable_bg = True
         else:
             A_BOLD = curses.A_BOLD
@@ -283,18 +281,21 @@
                     try:
                         curses.init_pair(i + 9, colors_list[i], -1)
                     except Exception:
                         curses.init_pair(i + 9, -1, -1)
                 self.filter_color = curses.color_pair(9) | A_BOLD
                 self.selected_color = curses.color_pair(10) | A_BOLD
                 # Define separator line style
-                curses.init_color(11, 500, 500, 500)
-                curses.init_pair(11, curses.COLOR_BLACK, -1)
-                self.separator = curses.color_pair(11)
-
+                try:
+                    curses.init_color(11, 500, 500, 500)
+                    curses.init_pair(11, curses.COLOR_BLACK, -1)
+                    self.separator = curses.color_pair(11)
+                except Exception:
+                    # Catch exception in TMUX
+                    pass
         else:
             # The screen is NOT compatible with a colored design
             # switch to B&W text styles
             # ex: export TERM=xterm-mono
             self.no_color = -1
             self.default_color = -1
             self.nice_color = A_BOLD
@@ -351,25 +352,24 @@
             try:
                 curses.curs_set(value)
             except Exception:
                 pass
 
     def get_key(self, window):
         # TODO: Check issue #163
-        ret = window.getch()
-        return ret
+        return window.getch()
 
     def __catch_key(self, return_to_browser=False):
         # Catch the pressed key
         self.pressedkey = self.get_key(self.term_window)
         if self.pressedkey == -1:
             return -1
 
         # Actions (available in the global hotkey dict)...
-        logger.debug("Keypressed (code: {})".format(self.pressedkey))
+        logger.debug(f"Keypressed (code: {self.pressedkey})")
         for hotkey in self._hotkeys:
             if self.pressedkey == ord(hotkey) and 'switch' in self._hotkeys[hotkey]:
                 self._handle_switch(hotkey)
             elif self.pressedkey == ord(hotkey) and 'sort_key' in self._hotkeys[hotkey]:
                 self._handle_sort_key(hotkey)
             if self.pressedkey == ord(hotkey) and 'handler' in self._hotkeys[hotkey]:
                 action = getattr(self, self._hotkeys[hotkey]['handler'])
@@ -488,15 +488,15 @@
         if self.args.cursor_position < glances_processes.processes_count:
             self.args.cursor_position += 1
 
     def _handle_quit(self, return_to_browser):
         if return_to_browser:
             logger.info("Stop Glances client and return to the browser")
         else:
-            logger.info("Stop Glances (keypressed: {})".format(self.pressedkey))
+            logger.info(f"Stop Glances (keypressed: {self.pressedkey})")
 
     def _handle_refresh(self):
         pass
 
     def loop_position(self):
         """Return the current sort in the loop"""
         for i, v in enumerate(self._sort_loop):
@@ -709,15 +709,15 @@
         elif self.kill_process and cs_status is not None:
             self.display_popup('Kill process only available for local processes')
         self.kill_process = False
 
         # Display graph generation popup
         if self.args.generate_graph:
             if 'graph' in stats.getExportsList():
-                self.display_popup('Generate graph in {}'.format(self.args.export_graph_path))
+                self.display_popup(f'Generate graph in {self.args.export_graph_path}')
             else:
                 logger.warning('Graph export module is disable. Run Glances with --export graph to enable it.')
                 self.args.generate_graph = False
 
         return True
 
     def nice_increase(self, process):
@@ -728,15 +728,15 @@
 
     def kill(self, process):
         """Kill a process, or a list of process if the process has a childrens field.
 
         :param process
         :return: None
         """
-        logger.debug("Selected process to kill: {}".format(process))
+        logger.debug(f"Selected process to kill: {process}")
 
         if 'childrens' in process:
             pid_to_kill = process['childrens']
         else:
             pid_to_kill = [process['pid']]
 
         confirm = self.display_popup(
@@ -748,17 +748,17 @@
         )
 
         if confirm.lower().startswith('y'):
             for pid in pid_to_kill:
                 try:
                     ret_kill = glances_processes.kill(pid)
                 except Exception as e:
-                    logger.error('Can not kill process {} ({})'.format(pid, e))
+                    logger.error(f'Can not kill process {pid} ({e})')
                 else:
-                    logger.info('Kill signal has been sent to process {} (return code: {})'.format(pid, ret_kill))
+                    logger.info(f'Kill signal has been sent to process {pid} (return code: {ret_kill})')
 
     def __display_header(self, stat_display):
         """Display the firsts lines (header) in the Curses interface.
 
         system + ip + uptime
         (cloud)
         """
@@ -822,15 +822,15 @@
                     self._quicklook_max_width - 5,
                 )
             try:
                 stat_display["quicklook"] = stats.get_plugin('quicklook').get_stats_display(
                     max_width=quicklook_width, args=self.args
                 )
             except AttributeError as e:
-                logger.debug("Quicklook plugin not available (%s)" % e)
+                logger.debug(f"Quicklook plugin not available ({e})")
             else:
                 plugin_widths['quicklook'] = self.get_stats_display_width(stat_display["quicklook"])
                 stats_width = sum(itervalues(plugin_widths)) + 1
             self.space_between_column = 1
             self.display_plugin(stat_display["quicklook"])
             self.new_column()
 
@@ -982,15 +982,16 @@
                 popup.addnstr(2 + y, 2, m, len(m))
 
         if popup_type == 'info':
             # Display the popup
             popup.refresh()
             self.wait(duration * 1000)
             return True
-        elif popup_type == 'input':
+
+        if popup_type == 'input':
             logger.info(popup_type)
             logger.info(is_password)
             # Create a sub-window for the text field
             sub_pop = popup.derwin(1, input_size, 2, 2 + len(m))
             sub_pop.attron(self.colors_list['FILTER'])
             # Init the field with the current value
             if input_value is not None:
@@ -1002,25 +1003,25 @@
             self.set_cursor(2)
             self.term_window.keypad(1)
             if is_password:
                 textbox = getpass.getpass('')
                 self.set_cursor(0)
                 if textbox != '':
                     return textbox
-                else:
-                    return None
-            else:
-                textbox = GlancesTextbox(sub_pop, insert_mode=True)
-                textbox.edit()
-                self.set_cursor(0)
-                if textbox.gather() != '':
-                    return textbox.gather()[:-1]
-                else:
-                    return None
-        elif popup_type == 'yesno':
+                return None
+
+            # No password
+            textbox = GlancesTextbox(sub_pop, insert_mode=True)
+            textbox.edit()
+            self.set_cursor(0)
+            if textbox.gather() != '':
+                return textbox.gather()[:-1]
+            return None
+
+        if popup_type == 'yesno':
             # # Create a sub-window for the text field
             sub_pop = popup.derwin(1, 2, len(sentence_list) + 1, len(m) + 2)
             sub_pop.attron(self.colors_list['FILTER'])
             # Init the field with the current value
             sub_pop.addnstr(0, 0, '', 0)
             # Display the popup
             popup.refresh()
@@ -1030,14 +1031,16 @@
             self.term_window.keypad(1)
             textbox = GlancesTextboxYesNo(sub_pop, insert_mode=False)
             textbox.edit()
             self.set_cursor(0)
             # self.term_window.keypad(0)
             return textbox.gather()
 
+        return None
+
     def display_plugin(self, plugin_stats, display_optional=True, display_additional=True, max_y=65535, add_space=0):
         """Display the plugin_stats on the screen.
 
         :param plugin_stats:
         :param display_optional: display the optional stats if True
         :param display_additional: display additional stats if True
         :param max_y: do not display line > max_y
@@ -1124,14 +1127,15 @@
 
         # Compute the next Glances column/line position
         self.next_column = max(self.next_column, x_max + self.space_between_column)
         self.next_line = max(self.next_line, y + self.space_between_line)
 
         # Have empty lines after the plugins
         self.next_line += add_space
+        return None
 
     def clear(self):
         """Erase the content of the screen.
         The difference is that clear() also calls clearok(). clearok()
         basically tells ncurses to forget whatever it knows about the current
         terminal contents, so that when refresh() is called, it will actually
         begin by clearing the entire terminal screen before redrawing any of it."""
@@ -1206,16 +1210,15 @@
                 # Up of won key pressed, reset the countdown
                 # Better for user experience
                 countdown.reset()
 
             if isexitkey and self.args.help_tag:
                 # Quit from help should return to main screen, not exit #1874
                 self.args.help_tag = not self.args.help_tag
-                isexitkey = False
-                return isexitkey
+                return False
 
             if not isexitkey and pressedkey > -1:
                 # Redraw display
                 self.flush(stats, cs_status=cs_status)
                 # Overwrite the timeout with the countdown
                 self.wait(delay=int(countdown.get() * 1000))
 
@@ -1248,52 +1251,52 @@
                         ''.join(
                             [u(u(nativestr(i['msg'])).encode('ascii', 'replace')) for i in curse_msg['msgdict']]
                         ).split('\n'),
                         key=len,
                     )
                 )
         except Exception as e:
-            logger.debug('ERROR: Can not compute plugin width ({})'.format(e))
+            logger.debug(f'ERROR: Can not compute plugin width ({e})')
             return 0
         else:
             return c
 
     def get_stats_display_height(self, curse_msg):
         """Return the height of the formatted curses message.
 
         The height is defined by the number of '\n' (new line).
         """
         try:
             c = [i['msg'] for i in curse_msg['msgdict']].count('\n')
         except Exception as e:
-            logger.debug('ERROR: Can not compute plugin height ({})'.format(e))
+            logger.debug(f'ERROR: Can not compute plugin height ({e})')
             return 0
         else:
             return c + 1
 
 
 class GlancesCursesStandalone(_GlancesCurses):
     """Class for the Glances curse standalone."""
 
 
 class GlancesCursesClient(_GlancesCurses):
     """Class for the Glances curse client."""
 
 
-class GlancesTextbox(Textbox, object):
+class GlancesTextbox(Textbox):
     def __init__(self, *args, **kwargs):
-        super(GlancesTextbox, self).__init__(*args, **kwargs)
+        super().__init__(*args, **kwargs)
 
     def do_command(self, ch):
         if ch == 10:  # Enter
             return 0
         if ch == 127:  # Back
             return 8
-        return super(GlancesTextbox, self).do_command(ch)
+        return super().do_command(ch)
 
 
-class GlancesTextboxYesNo(Textbox, object):
+class GlancesTextboxYesNo(Textbox):
     def __init__(self, *args, **kwargs):
-        super(GlancesTextboxYesNo, self).__init__(*args, **kwargs)
+        super().__init__(*args, **kwargs)
 
     def do_command(self, ch):
-        return super(GlancesTextboxYesNo, self).do_command(ch)
+        return super().do_command(ch)
```

### Comparing `glances-4.0.4/glances/outputs/glances_curses_browser.py` & `glances-4.0.5/glances/outputs/glances_curses_browser.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,32 +1,31 @@
-# -*- coding: utf-8 -*-
 #
 # This file is part of Glances.
 #
 # SPDX-FileCopyrightText: 2022 Nicolas Hennion <nicolas@nicolargo.com>
 #
 # SPDX-License-Identifier: LGPL-3.0-only
 #
 
 """Curses browser interface class ."""
 
-import math
 import curses
-from glances.outputs.glances_curses import _GlancesCurses
+import math
 
 from glances.logger import logger
+from glances.outputs.glances_curses import _GlancesCurses
 from glances.timer import Timer
 
 
 class GlancesCursesBrowser(_GlancesCurses):
     """Class for the Glances curse client browser."""
 
     def __init__(self, args=None):
         """Init the father class."""
-        super(GlancesCursesBrowser, self).__init__(args=args)
+        super().__init__(args=args)
 
         _colors_list = {
             'UNKNOWN': self.no_color,
             'SNMP': self.default_color2,
             'ONLINE': self.default_color2,
             'OFFLINE': self.ifCRITICAL_color2,
             'PROTECTED': self.ifWARNING_color2,
@@ -147,43 +146,43 @@
         self.cursor_position = 0
 
     def __catch_key(self, stats):
         # Catch the browser pressed key
         self.pressedkey = self.get_key(self.term_window)
         refresh = False
         if self.pressedkey != -1:
-            logger.debug("Key pressed. Code=%s" % self.pressedkey)
+            logger.debug(f"Key pressed. Code={self.pressedkey}")
 
         # Actions...
         if self.pressedkey == ord('\x1b') or self.pressedkey == ord('q'):
             # 'ESC'|'q' > Quit
             self.end()
             logger.info("Stop Glances client browser")
             # sys.exit(0)
             self.is_end = True
         elif self.pressedkey == 10:
             # 'ENTER' > Run Glances on the selected server
             self.active_server = self._current_page * self._page_max_lines + self.cursor_position
-            logger.debug("Server {}/{} selected".format(self.active_server, len(stats)))
+            logger.debug(f"Server {self.active_server}/{len(stats)} selected")
         elif self.pressedkey == curses.KEY_UP or self.pressedkey == 65:
             # 'UP' > Up in the server list
             self.cursor_up(stats)
-            logger.debug("Server {}/{} selected".format(self.cursor + 1, len(stats)))
+            logger.debug(f"Server {self.cursor + 1}/{len(stats)} selected")
         elif self.pressedkey == curses.KEY_DOWN or self.pressedkey == 66:
             # 'DOWN' > Down in the server list
             self.cursor_down(stats)
-            logger.debug("Server {}/{} selected".format(self.cursor + 1, len(stats)))
+            logger.debug(f"Server {self.cursor + 1}/{len(stats)} selected")
         elif self.pressedkey == curses.KEY_PPAGE:
             # 'Page UP' > Prev page in the server list
             self.cursor_pageup(stats)
-            logger.debug("PageUP: Server ({}/{}) pages.".format(self._current_page + 1, self._page_max))
+            logger.debug(f"PageUP: Server ({self._current_page + 1}/{self._page_max}) pages.")
         elif self.pressedkey == curses.KEY_NPAGE:
             # 'Page Down' > Next page in the server list
             self.cursor_pagedown(stats)
-            logger.debug("PageDown: Server {}/{} pages".format(self._current_page + 1, self._page_max))
+            logger.debug(f"PageDown: Server {self._current_page + 1}/{self._page_max} pages")
         elif self.pressedkey == ord('1'):
             self._stats_list = None
             refresh = True
         elif self.pressedkey == ord('2'):
             self._revesed_sorting = False
             self._stats_list = stats.copy()
             refresh = True
@@ -207,15 +206,15 @@
 
         :param stats: Dict of dict with servers stats
         :param cs_status:
         :param duration:
         :param return_to_browser:
         """
         # Flush display
-        logger.debug('Servers list: {}'.format(stats))
+        logger.debug(f'Servers list: {stats}')
         self.flush(stats)
 
         # Wait
         exitkey = False
         countdown = Timer(self.__refresh_time)
         while not countdown.finished() and not exitkey:
             # Getkey
@@ -264,27 +263,27 @@
                 msg = 'Glances is scanning your network. Please wait...'
                 self.first_scan = False
             else:
                 msg = 'No Glances server available'
         elif len(stats) == 1:
             msg = 'One Glances server available'
         else:
-            msg = '{} Glances servers available'.format(stats_len)
+            msg = f'{stats_len} Glances servers available'
         if self.args.disable_autodiscover:
             msg += ' (auto discover is disabled)'
         if screen_y > 1:
             self.term_window.addnstr(y, x, msg, screen_x - x, self.colors_list['TITLE'])
 
-            msg = '{}'.format(self._get_status_count(stats))
+            msg = f'{self._get_status_count(stats)}'
             self.term_window.addnstr(y + 1, x, msg, screen_x - x)
 
         if stats_len > stats_max and screen_y > 2:
-            msg = '{} servers displayed.({}/{}) {}'.format(
-                self.get_pagelines(stats), self._current_page + 1, self._page_max, self._get_status_count(stats)
-            )
+            page_lines = self.get_pagelines(stats)
+            status_count = self._get_status_count(stats)
+            msg = f'{page_lines} servers displayed.({self._current_page + 1}/{self._page_max}) {status_count}'
             self.term_window.addnstr(y + 1, x, msg, screen_x - x)
 
         if stats_len == 0:
             return False
 
         # Display the Glances server list
         # ================================
@@ -331,15 +330,15 @@
                 continue
             # Get server stats
             server_stat = {}
             for c in column_def:
                 try:
                     server_stat[c[0]] = v[c[0]]
                 except KeyError as e:
-                    logger.debug("Cannot grab stats {} from server (KeyError: {})".format(c[0], e))
+                    logger.debug(f"Cannot grab stats {c[0]} from server (KeyError: {e})")
                     server_stat[c[0]] = '?'
                 # Display alias instead of name
                 try:
                     if c[0] == 'alias' and v[c[0]] is not None:
                         server_stat['name'] = v[c[0]]
                 except KeyError:
                     pass
```

### Comparing `glances-4.0.4/glances/outputs/glances_restful_api.py` & `glances-4.0.5/glances/outputs/glances_restful_api.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,51 +1,54 @@
-# -*- coding: utf-8 -*-
 #
 # This file is part of Glances.
 #
 # SPDX-FileCopyrightText: 2024 Nicolas Hennion <nicolas@nicolargo.com>
 #
 # SPDX-License-Identifier: LGPL-3.0-only
 #
 
 """RestFull API interface class."""
 
 import os
 import sys
 import tempfile
-from io import open
 import webbrowser
 from urllib.parse import urljoin
 
-# Replace typing_extensions by typing when Python 3.8 support will be dropped
-from typing import Annotated
+try:
+    from typing import Annotated
+except ImportError:
+    # Only for Python 3.8
+    # To be removed when Python 3.8 support will be dropped
+    from typing_extensions import Annotated
 
-from glances import __version__, __apiversion__
+from glances import __apiversion__, __version__
+from glances.logger import logger
 from glances.password import GlancesPassword
 from glances.timer import Timer
-from glances.logger import logger
 
 # FastAPI import
 try:
-    from fastapi import FastAPI, Depends, HTTPException, status, APIRouter, Request
-    from fastapi.security import HTTPBasic, HTTPBasicCredentials
+    from fastapi import APIRouter, Depends, FastAPI, HTTPException, Request, status
     from fastapi.middleware.cors import CORSMiddleware
     from fastapi.middleware.gzip import GZipMiddleware
     from fastapi.responses import HTMLResponse, ORJSONResponse
-    from fastapi.templating import Jinja2Templates
+    from fastapi.security import HTTPBasic, HTTPBasicCredentials
     from fastapi.staticfiles import StaticFiles
+    from fastapi.templating import Jinja2Templates
 except ImportError:
     logger.critical('FastAPI import error. Glances cannot start in web server mode.')
     sys.exit(2)
 
 try:
     import uvicorn
 except ImportError:
     logger.critical('Uvicorn import error. Glances cannot start in web server mode.')
     sys.exit(2)
+import builtins
 import contextlib
 import threading
 import time
 
 security = HTTPBasic()
 
 
@@ -69,15 +72,15 @@
                 thread.join()
             yield
         finally:
             self.should_exit = True
             thread.join()
 
 
-class GlancesRestfulApi(object):
+class GlancesRestfulApi:
     """This class manages the Restful API server."""
 
     API_VERSION = __apiversion__
 
     def __init__(self, config=None, args=None):
         # Init config
         self.config = config
@@ -94,15 +97,15 @@
         # since last update is passed (will retrieve old cached info instead)
         self.timer = Timer(0)
 
         # Load configuration file
         self.load_config(config)
 
         # Set the bind URL
-        self.bind_url = urljoin('http://{}:{}/'.format(self.args.bind_address, self.args.port), self.url_prefix)
+        self.bind_url = urljoin(f'http://{self.args.bind_address}:{self.args.port}/', self.url_prefix)
 
         # FastAPI Init
         if self.args.password:
             self._app = FastAPI(dependencies=[Depends(self.authentication)])
             self._password = GlancesPassword(username=args.username, config=config)
 
         else:
@@ -143,17 +146,17 @@
 
     def load_config(self, config):
         """Load the outputs section of the configuration file."""
         # Limit the number of processes to display in the WebUI
         self.url_prefix = '/'
         if config is not None and config.has_section('outputs'):
             n = config.get_value('outputs', 'max_processes_display', default=None)
-            logger.debug('Number of processes to display in the WebUI: {}'.format(n))
+            logger.debug(f'Number of processes to display in the WebUI: {n}')
             self.url_prefix = config.get_value('outputs', 'url_prefix', default='/')
-            logger.debug('URL prefix: {}'.format(self.url_prefix))
+            logger.debug(f'URL prefix: {self.url_prefix}')
 
     def __update__(self):
         # Never update more than 1 time per cached_time
         if self.timer.finished():
             self.stats.update()
             self.timer = Timer(self.args.cached_time)
 
@@ -176,113 +179,113 @@
 
     def _router(self):
         """Define a custom router for Glances path."""
         router = APIRouter()
 
         # REST API
         router.add_api_route(
-            '/api/%s/status' % self.API_VERSION,
+            f'/api/{self.API_VERSION}/status',
             status_code=status.HTTP_200_OK,
             response_class=ORJSONResponse,
             endpoint=self._api_status,
         )
 
         router.add_api_route(
-            '/api/%s/config' % self.API_VERSION, response_class=ORJSONResponse, endpoint=self._api_config
+            f'/api/{self.API_VERSION}/config', response_class=ORJSONResponse, endpoint=self._api_config
         )
         router.add_api_route(
-            '/api/%s/config/{section}' % self.API_VERSION,
+            f'/api/{self.API_VERSION}/config/{{section}}',
             response_class=ORJSONResponse,
             endpoint=self._api_config_section,
         )
         router.add_api_route(
-            '/api/%s/config/{section}/{item}' % self.API_VERSION,
+            f'/api/{self.API_VERSION}/config/{{section}}/{{item}}',
             response_class=ORJSONResponse,
             endpoint=self._api_config_section_item,
         )
 
-        router.add_api_route('/api/%s/args' % self.API_VERSION, response_class=ORJSONResponse, endpoint=self._api_args)
+        router.add_api_route(f'/api/{self.API_VERSION}/args', response_class=ORJSONResponse, endpoint=self._api_args)
         router.add_api_route(
-            '/api/%s/args/{item}' % self.API_VERSION, response_class=ORJSONResponse, endpoint=self._api_args_item
+            f'/api/{self.API_VERSION}/args/{{item}}', response_class=ORJSONResponse, endpoint=self._api_args_item
         )
 
         router.add_api_route(
-            '/api/%s/pluginslist' % self.API_VERSION, response_class=ORJSONResponse, endpoint=self._api_plugins
+            f'/api/{self.API_VERSION}/pluginslist', response_class=ORJSONResponse, endpoint=self._api_plugins
         )
-        router.add_api_route('/api/%s/all' % self.API_VERSION, response_class=ORJSONResponse, endpoint=self._api_all)
+        router.add_api_route(f'/api/{self.API_VERSION}/all', response_class=ORJSONResponse, endpoint=self._api_all)
         router.add_api_route(
-            '/api/%s/all/limits' % self.API_VERSION, response_class=ORJSONResponse, endpoint=self._api_all_limits
+            f'/api/{self.API_VERSION}/all/limits', response_class=ORJSONResponse, endpoint=self._api_all_limits
         )
         router.add_api_route(
-            '/api/%s/all/views' % self.API_VERSION, response_class=ORJSONResponse, endpoint=self._api_all_views
+            f'/api/{self.API_VERSION}/all/views', response_class=ORJSONResponse, endpoint=self._api_all_views
         )
 
-        router.add_api_route('/api/%s/help' % self.API_VERSION, response_class=ORJSONResponse, endpoint=self._api_help)
-        router.add_api_route('/api/%s/{plugin}' % self.API_VERSION, response_class=ORJSONResponse, endpoint=self._api)
+        router.add_api_route(f'/api/{self.API_VERSION}/help', response_class=ORJSONResponse, endpoint=self._api_help)
+        router.add_api_route(f'/api/{self.API_VERSION}/{{plugin}}', response_class=ORJSONResponse, endpoint=self._api)
         router.add_api_route(
-            '/api/%s/{plugin}/history' % self.API_VERSION, response_class=ORJSONResponse, endpoint=self._api_history
+            f'/api/{self.API_VERSION}/{{plugin}}/history', response_class=ORJSONResponse, endpoint=self._api_history
         )
         router.add_api_route(
-            '/api/%s/{plugin}/history/{nb}' % self.API_VERSION,
+            f'/api/{self.API_VERSION}/{{plugin}}/history/{{nb}}',
             response_class=ORJSONResponse,
             endpoint=self._api_history,
         )
         router.add_api_route(
-            '/api/%s/{plugin}/top/{nb}' % self.API_VERSION, response_class=ORJSONResponse, endpoint=self._api_top
+            f'/api/{self.API_VERSION}/{{plugin}}/top/{{nb}}', response_class=ORJSONResponse, endpoint=self._api_top
         )
         router.add_api_route(
-            '/api/%s/{plugin}/limits' % self.API_VERSION, response_class=ORJSONResponse, endpoint=self._api_limits
+            f'/api/{self.API_VERSION}/{{plugin}}/limits', response_class=ORJSONResponse, endpoint=self._api_limits
         )
         router.add_api_route(
-            '/api/%s/{plugin}/views' % self.API_VERSION, response_class=ORJSONResponse, endpoint=self._api_views
+            f'/api/{self.API_VERSION}/{{plugin}}/views', response_class=ORJSONResponse, endpoint=self._api_views
         )
         router.add_api_route(
-            '/api/%s/{plugin}/{item}' % self.API_VERSION, response_class=ORJSONResponse, endpoint=self._api_item
+            f'/api/{self.API_VERSION}/{{plugin}}/{{item}}', response_class=ORJSONResponse, endpoint=self._api_item
         )
         router.add_api_route(
-            '/api/%s/{plugin}/{item}/history' % self.API_VERSION,
+            f'/api/{self.API_VERSION}/{{plugin}}/{{item}}/history',
             response_class=ORJSONResponse,
             endpoint=self._api_item_history,
         )
         router.add_api_route(
-            '/api/%s/{plugin}/{item}/history/{nb}' % self.API_VERSION,
+            f'/api/{self.API_VERSION}/{{plugin}}/{{item}}/history/{{nb}}',
             response_class=ORJSONResponse,
             endpoint=self._api_item_history,
         )
         router.add_api_route(
-            '/api/%s/{plugin}/{item}/description' % self.API_VERSION,
+            f'/api/{self.API_VERSION}/{{plugin}}/{{item}}/description',
             response_class=ORJSONResponse,
             endpoint=self._api_item_description,
         )
         router.add_api_route(
-            '/api/%s/{plugin}/{item}/unit' % self.API_VERSION,
+            f'/api/{self.API_VERSION}/{{plugin}}/{{item}}/unit',
             response_class=ORJSONResponse,
             endpoint=self._api_item_unit,
         )
         router.add_api_route(
-            '/api/%s/{plugin}/{item}/{value}' % self.API_VERSION,
+            f'/api/{self.API_VERSION}/{{plugin}}/{{item}}/{{value}}',
             response_class=ORJSONResponse,
             endpoint=self._api_value,
         )
 
         # Restful API
-        bindmsg = 'Glances RESTful API Server started on {}api/{}'.format(self.bind_url, self.API_VERSION)
+        bindmsg = f'Glances RESTful API Server started on {self.bind_url}api/{self.API_VERSION}'
         logger.info(bindmsg)
 
         # WEB UI
         if not self.args.disable_webui:
             # Template for the root index.html file
             router.add_api_route('/', response_class=HTMLResponse, endpoint=self._index)
 
             # Statics files
             self._app.mount("/static", StaticFiles(directory=self.STATIC_PATH), name="static")
 
-            logger.info("Get WebUI in {}".format(self.STATIC_PATH))
+            logger.info(f"Get WebUI in {self.STATIC_PATH}")
 
-            bindmsg = 'Glances Web User Interface started on {}'.format(self.bind_url)
+            bindmsg = f'Glances Web User Interface started on {self.bind_url}'
         else:
             bindmsg = 'The WebUI is disable (--disable-webui)'
 
         logger.info(bindmsg)
         print(bindmsg)
 
         return router
@@ -309,15 +312,15 @@
         # Run the Uvicorn Web server
         uvicorn_config = uvicorn.Config(
             self._app, host=self.args.bind_address, port=self.args.port, access_log=self.args.debug
         )
         try:
             self.uvicorn_server = GlancesUvicornServer(config=uvicorn_config)
         except Exception as e:
-            logger.critical('Error: Can not ran Glances Web server ({})'.format(e))
+            logger.critical(f'Error: Can not ran Glances Web server ({e})')
             self.uvicorn_server = None
         else:
             with self.uvicorn_server.run_in_thread():
                 while not self.uvicorn_server.should_exit:
                     time.sleep(1)
 
     def end(self):
@@ -361,15 +364,15 @@
         """Glances API RESTful implementation.
 
         Return the help data or 404 error.
         """
         try:
             plist = self.stats.get_plugin("help").get_view_data()
         except Exception as e:
-            raise HTTPException(status_code=status.HTTP_404_NOT_FOUND, detail="Cannot get help view data (%s)" % str(e))
+            raise HTTPException(status_code=status.HTTP_404_NOT_FOUND, detail=f"Cannot get help view data ({str(e)})")
 
         return ORJSONResponse(plist)
 
     def _api_plugins(self):
         """Glances API RESTFul implementation.
 
         @api {get} /api/%s/pluginslist Get plugins list
@@ -397,42 +400,42 @@
         """
         # Update the stat
         self.__update__()
 
         try:
             plist = self.plugins_list
         except Exception as e:
-            raise HTTPException(status_code=status.HTTP_404_NOT_FOUND, detail="Cannot get plugin list (%s)" % str(e))
+            raise HTTPException(status_code=status.HTTP_404_NOT_FOUND, detail=f"Cannot get plugin list ({str(e)})")
 
         return ORJSONResponse(plist)
 
     def _api_all(self):
         """Glances API RESTful implementation.
 
         Return the JSON representation of all the plugins
         HTTP/200 if OK
         HTTP/400 if plugin is not found
         HTTP/404 if others error
         """
         if self.args.debug:
             fname = os.path.join(tempfile.gettempdir(), 'glances-debug.json')
             try:
-                with open(fname) as f:
+                with builtins.open(fname) as f:
                     return f.read()
-            except IOError:
-                logger.debug("Debug file (%s) not found" % fname)
+            except OSError:
+                logger.debug(f"Debug file ({fname}) not found")
 
         # Update the stat
         self.__update__()
 
         try:
             # Get the RAW value of the stat ID
             statval = self.stats.getAllAsDict()
         except Exception as e:
-            raise HTTPException(status_code=status.HTTP_404_NOT_FOUND, detail="Cannot get stats (%s)" % str(e))
+            raise HTTPException(status_code=status.HTTP_404_NOT_FOUND, detail=f"Cannot get stats ({str(e)})")
 
         return ORJSONResponse(statval)
 
     def _api_all_limits(self):
         """Glances API RESTful implementation.
 
         Return the JSON representation of all the plugins limits
@@ -440,15 +443,15 @@
         HTTP/400 if plugin is not found
         HTTP/404 if others error
         """
         try:
             # Get the RAW value of the stat limits
             limits = self.stats.getAllLimitsAsDict()
         except Exception as e:
-            raise HTTPException(status_code=status.HTTP_404_NOT_FOUND, detail="Cannot get limits (%s)" % str(e))
+            raise HTTPException(status_code=status.HTTP_404_NOT_FOUND, detail=f"Cannot get limits ({str(e)})")
 
         return ORJSONResponse(limits)
 
     def _api_all_views(self):
         """Glances API RESTful implementation.
 
         Return the JSON representation of all the plugins views
@@ -456,42 +459,40 @@
         HTTP/400 if plugin is not found
         HTTP/404 if others error
         """
         try:
             # Get the RAW value of the stat view
             limits = self.stats.getAllViewsAsDict()
         except Exception as e:
-            raise HTTPException(status_code=status.HTTP_404_NOT_FOUND, detail="Cannot get views (%s)" % str(e))
+            raise HTTPException(status_code=status.HTTP_404_NOT_FOUND, detail=f"Cannot get views ({str(e)})")
 
         return ORJSONResponse(limits)
 
     def _api(self, plugin):
         """Glances API RESTful implementation.
 
         Return the JSON representation of a given plugin
         HTTP/200 if OK
         HTTP/400 if plugin is not found
         HTTP/404 if others error
         """
         if plugin not in self.plugins_list:
             raise HTTPException(
                 status_code=status.HTTP_400_BAD_REQUEST,
-                detail="Unknown plugin %s (available plugins: %s)" % (plugin, self.plugins_list),
+                detail=f"Unknown plugin {plugin} (available plugins: {self.plugins_list})",
             )
 
         # Update the stat
         self.__update__()
 
         try:
             # Get the RAW value of the stat ID
             statval = self.stats.get_plugin(plugin).get_raw()
         except Exception as e:
-            raise HTTPException(
-                status_code=status.HTTP_404_NOT_FOUND, detail="Cannot get plugin %s (%s)" % (plugin, str(e))
-            )
+            raise HTTPException(status_code=status.HTTP_404_NOT_FOUND, detail=f"Cannot get plugin {plugin} ({str(e)})")
 
         return ORJSONResponse(statval)
 
     def _api_top(self, plugin, nb: int = 0):
         """Glances API RESTful implementation.
 
         Return the JSON representation of a given plugin limited to the top nb items.
@@ -500,27 +501,25 @@
         HTTP/200 if OK
         HTTP/400 if plugin is not found
         HTTP/404 if others error
         """
         if plugin not in self.plugins_list:
             raise HTTPException(
                 status_code=status.HTTP_400_BAD_REQUEST,
-                detail="Unknown plugin %s (available plugins: %s)" % (plugin, self.plugins_list),
+                detail=f"Unknown plugin {plugin} (available plugins: {self.plugins_list})",
             )
 
         # Update the stat
         self.__update__()
 
         try:
             # Get the RAW value of the stat ID
             statval = self.stats.get_plugin(plugin).get_raw()
         except Exception as e:
-            raise HTTPException(
-                status_code=status.HTTP_404_NOT_FOUND, detail="Cannot get plugin %s (%s)" % (plugin, str(e))
-            )
+            raise HTTPException(status_code=status.HTTP_404_NOT_FOUND, detail=f"Cannot get plugin {plugin} ({str(e)})")
 
         print(statval)
 
         if isinstance(statval, list):
             statval = statval[:nb]
 
         return ORJSONResponse(statval)
@@ -533,26 +532,26 @@
         HTTP/200 if OK
         HTTP/400 if plugin is not found
         HTTP/404 if others error
         """
         if plugin not in self.plugins_list:
             raise HTTPException(
                 status_code=status.HTTP_400_BAD_REQUEST,
-                detail="Unknown plugin %s (available plugins: %s)" % (plugin, self.plugins_list),
+                detail=f"Unknown plugin {plugin} (available plugins: {self.plugins_list})",
             )
 
         # Update the stat
         self.__update__()
 
         try:
             # Get the RAW value of the stat ID
             statval = self.stats.get_plugin(plugin).get_raw_history(nb=int(nb))
         except Exception as e:
             raise HTTPException(
-                status_code=status.HTTP_404_NOT_FOUND, detail="Cannot get plugin history %s (%s)" % (plugin, str(e))
+                status_code=status.HTTP_404_NOT_FOUND, detail=f"Cannot get plugin history {plugin} ({str(e)})"
             )
 
         return statval
 
     def _api_limits(self, plugin):
         """Glances API RESTful implementation.
 
@@ -560,23 +559,23 @@
         HTTP/200 if OK
         HTTP/400 if plugin is not found
         HTTP/404 if others error
         """
         if plugin not in self.plugins_list:
             raise HTTPException(
                 status_code=status.HTTP_400_BAD_REQUEST,
-                detail="Unknown plugin %s (available plugins: %s)" % (plugin, self.plugins_list),
+                detail=f"Unknown plugin {plugin} (available plugins: {self.plugins_list})",
             )
 
         try:
             # Get the RAW value of the stat limits
             ret = self.stats.get_plugin(plugin).limits
         except Exception as e:
             raise HTTPException(
-                status_code=status.HTTP_404_NOT_FOUND, detail="Cannot get limits for plugin %s (%s)" % (plugin, str(e))
+                status_code=status.HTTP_404_NOT_FOUND, detail=f"Cannot get limits for plugin {plugin} ({str(e)})"
             )
 
         return ORJSONResponse(ret)
 
     def _api_views(self, plugin):
         """Glances API RESTful implementation.
 
@@ -584,23 +583,23 @@
         HTTP/200 if OK
         HTTP/400 if plugin is not found
         HTTP/404 if others error
         """
         if plugin not in self.plugins_list:
             raise HTTPException(
                 status_code=status.HTTP_400_BAD_REQUEST,
-                detail="Unknown plugin %s (available plugins: %s)" % (plugin, self.plugins_list),
+                detail=f"Unknown plugin {plugin} (available plugins: {self.plugins_list})",
             )
 
         try:
             # Get the RAW value of the stat views
             ret = self.stats.get_plugin(plugin).get_views()
         except Exception as e:
             raise HTTPException(
-                status_code=status.HTTP_404_NOT_FOUND, detail="Cannot get views for plugin %s (%s)" % (plugin, str(e))
+                status_code=status.HTTP_404_NOT_FOUND, detail=f"Cannot get views for plugin {plugin} ({str(e)})"
             )
 
         return ORJSONResponse(ret)
 
     def _api_item(self, plugin, item):
         """Glances API RESTful implementation.
 
@@ -608,27 +607,27 @@
         HTTP/200 if OK
         HTTP/400 if plugin is not found
         HTTP/404 if others error
         """
         if plugin not in self.plugins_list:
             raise HTTPException(
                 status_code=status.HTTP_400_BAD_REQUEST,
-                detail="Unknown plugin %s (available plugins: %s)" % (plugin, self.plugins_list),
+                detail=f"Unknown plugin {plugin} (available plugins: {self.plugins_list})",
             )
 
         # Update the stat
         self.__update__()
 
         try:
             # Get the RAW value of the stat views
             ret = self.stats.get_plugin(plugin).get_raw_stats_item(item)
         except Exception as e:
             raise HTTPException(
                 status_code=status.HTTP_404_NOT_FOUND,
-                detail="Cannot get item %s in plugin %s (%s)" % (item, plugin, str(e)),
+                detail=f"Cannot get item {item} in plugin {plugin} ({str(e)})",
             )
 
         return ORJSONResponse(ret)
 
     def _api_item_history(self, plugin, item, nb: int = 0):
         """Glances API RESTful implementation.
 
@@ -637,26 +636,26 @@
         HTTP/400 if plugin is not found
         HTTP/404 if others error
 
         """
         if plugin not in self.plugins_list:
             raise HTTPException(
                 status_code=status.HTTP_400_BAD_REQUEST,
-                detail="Unknown plugin %s (available plugins: %s)" % (plugin, self.plugins_list),
+                detail=f"Unknown plugin {plugin} (available plugins: {self.plugins_list})",
             )
 
         # Update the stat
         self.__update__()
 
         try:
             # Get the RAW value of the stat history
             ret = self.stats.get_plugin(plugin).get_raw_history(item, nb=nb)
         except Exception as e:
             raise HTTPException(
-                status_code=status.HTTP_404_NOT_FOUND, detail="Cannot get history for plugin %s (%s)" % (plugin, str(e))
+                status_code=status.HTTP_404_NOT_FOUND, detail=f"Cannot get history for plugin {plugin} ({str(e)})"
             )
         else:
             return ORJSONResponse(ret)
 
     def _api_item_description(self, plugin, item):
         """Glances API RESTful implementation.
 
@@ -664,24 +663,24 @@
         HTTP/200 if OK
         HTTP/400 if plugin is not found
         HTTP/404 if others error
         """
         if plugin not in self.plugins_list:
             raise HTTPException(
                 status_code=status.HTTP_400_BAD_REQUEST,
-                detail="Unknown plugin %s (available plugins: %s)" % (plugin, self.plugins_list),
+                detail=f"Unknown plugin {plugin} (available plugins: {self.plugins_list})",
             )
 
         try:
             # Get the description
             ret = self.stats.get_plugin(plugin).get_item_info(item, 'description')
         except Exception as e:
             raise HTTPException(
                 status_code=status.HTTP_404_NOT_FOUND,
-                detail="Cannot get %s description for plugin %s (%s)" % (item, plugin, str(e)),
+                detail=f"Cannot get {item} description for plugin {plugin} ({str(e)})",
             )
         else:
             return ORJSONResponse(ret)
 
     def _api_item_unit(self, plugin, item):
         """Glances API RESTful implementation.
 
@@ -689,24 +688,24 @@
         HTTP/200 if OK
         HTTP/400 if plugin is not found
         HTTP/404 if others error
         """
         if plugin not in self.plugins_list:
             raise HTTPException(
                 status_code=status.HTTP_400_BAD_REQUEST,
-                detail="Unknown plugin %s (available plugins: %s)" % (plugin, self.plugins_list),
+                detail=f"Unknown plugin {plugin} (available plugins: {self.plugins_list})",
             )
 
         try:
             # Get the unit
             ret = self.stats.get_plugin(plugin).get_item_info(item, 'unit')
         except Exception as e:
             raise HTTPException(
                 status_code=status.HTTP_404_NOT_FOUND,
-                detail="Cannot get %s unit for plugin %s (%s)" % (item, plugin, str(e)),
+                detail=f"Cannot get {item} unit for plugin {plugin} ({str(e)})",
             )
         else:
             return ORJSONResponse(ret)
 
     def _api_value(self, plugin, item, value):
         """Glances API RESTful implementation.
 
@@ -714,27 +713,27 @@
         HTTP/200 if OK
         HTTP/400 if plugin is not found
         HTTP/404 if others error
         """
         if plugin not in self.plugins_list:
             raise HTTPException(
                 status_code=status.HTTP_400_BAD_REQUEST,
-                detail="Unknown plugin %s (available plugins: %s)" % (plugin, self.plugins_list),
+                detail=f"Unknown plugin {plugin} (available plugins: {self.plugins_list})",
             )
 
         # Update the stat
         self.__update__()
 
         try:
             # Get the RAW value
             ret = self.stats.get_plugin(plugin).get_raw_stats_value(item, value)
         except Exception as e:
             raise HTTPException(
                 status_code=status.HTTP_404_NOT_FOUND,
-                detail="Cannot get %s = %s for plugin %s (%s)" % (item, value, plugin, str(e)),
+                detail=f"Cannot get {item} = {value} for plugin {plugin} ({str(e)})",
             )
         else:
             return ORJSONResponse(ret)
 
     def _api_config(self):
         """Glances API RESTful implementation.
 
@@ -742,71 +741,67 @@
         HTTP/200 if OK
         HTTP/404 if others error
         """
         try:
             # Get the RAW value of the config' dict
             args_json = self.config.as_dict()
         except Exception as e:
-            raise HTTPException(status_code=status.HTTP_404_NOT_FOUND, detail="Cannot get config (%s)" % str(e))
+            raise HTTPException(status_code=status.HTTP_404_NOT_FOUND, detail=f"Cannot get config ({str(e)})")
         else:
             return ORJSONResponse(args_json)
 
     def _api_config_section(self, section):
         """Glances API RESTful implementation.
 
         Return the JSON representation of the Glances configuration section
         HTTP/200 if OK
         HTTP/400 if item is not found
         HTTP/404 if others error
         """
         config_dict = self.config.as_dict()
         if section not in config_dict:
-            raise HTTPException(
-                status_code=status.HTTP_400_BAD_REQUEST, detail="Unknown configuration item %s" % section
-            )
+            raise HTTPException(status_code=status.HTTP_400_BAD_REQUEST, detail=f"Unknown configuration item {section}")
 
         try:
             # Get the RAW value of the config' dict
             ret_section = config_dict[section]
         except Exception as e:
             raise HTTPException(
-                status_code=status.HTTP_404_NOT_FOUND, detail="Cannot get config section %s (%s)" % (section, str(e))
+                status_code=status.HTTP_404_NOT_FOUND, detail=f"Cannot get config section {section} ({str(e)})"
             )
 
         return ORJSONResponse(ret_section)
 
     def _api_config_section_item(self, section, item):
         """Glances API RESTful implementation.
 
         Return the JSON representation of the Glances configuration section/item
         HTTP/200 if OK
         HTTP/400 if item is not found
         HTTP/404 if others error
         """
         config_dict = self.config.as_dict()
         if section not in config_dict:
-            raise HTTPException(
-                status_code=status.HTTP_400_BAD_REQUEST, detail="Unknown configuration item %s" % section
-            )
+            raise HTTPException(status_code=status.HTTP_400_BAD_REQUEST, detail=f"Unknown configuration item {section}")
 
         try:
             # Get the RAW value of the config' dict section
             ret_section = config_dict[section]
         except Exception as e:
             raise HTTPException(
-                status_code=status.HTTP_404_NOT_FOUND, detail="Cannot get config section %s (%s)" % (section, str(e))
+                status_code=status.HTTP_404_NOT_FOUND, detail=f"Cannot get config section {section} ({str(e)})"
             )
 
         try:
             # Get the RAW value of the config' dict item
             ret_item = ret_section[item]
         except Exception as e:
             raise HTTPException(
                 status_code=status.HTTP_404_NOT_FOUND,
-                detail="Cannot get item %s in config section %s (%s)" % (item, section, str(e)),
+                detail=f"Cannot get item {item} in config section {section} ({str(e)})",
             )
 
         return ORJSONResponse(ret_item)
 
     def _api_args(self):
         """Glances API RESTful implementation.
 
@@ -816,31 +811,31 @@
         """
         try:
             # Get the RAW value of the args' dict
             # Use vars to convert namespace to dict
             # Source: https://docs.python.org/%s/library/functions.html#vars
             args_json = vars(self.args)
         except Exception as e:
-            raise HTTPException(status_code=status.HTTP_404_NOT_FOUND, detail="Cannot get args (%s)" % str(e))
+            raise HTTPException(status_code=status.HTTP_404_NOT_FOUND, detail=f"Cannot get args ({str(e)})")
 
         return ORJSONResponse(args_json)
 
     def _api_args_item(self, item):
         """Glances API RESTful implementation.
 
         Return the JSON representation of the Glances command line arguments item
         HTTP/200 if OK
         HTTP/400 if item is not found
         HTTP/404 if others error
         """
         if item not in self.args:
-            raise HTTPException(status_code=status.HTTP_400_BAD_REQUEST, detail="Unknown argument item %s" % item)
+            raise HTTPException(status_code=status.HTTP_400_BAD_REQUEST, detail=f"Unknown argument item {item}")
 
         try:
             # Get the RAW value of the args' dict
             # Use vars to convert namespace to dict
             # Source: https://docs.python.org/%s/library/functions.html#vars
             args_json = vars(self.args)[item]
         except Exception as e:
-            raise HTTPException(status_code=status.HTTP_404_NOT_FOUND, detail="Cannot get args item (%s)" % str(e))
+            raise HTTPException(status_code=status.HTTP_404_NOT_FOUND, detail=f"Cannot get args item ({str(e)})")
 
         return ORJSONResponse(args_json)
```

### Comparing `glances-4.0.4/glances/outputs/glances_sparklines.py` & `glances-4.0.5/glances/outputs/glances_sparklines.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,40 +1,38 @@
-# -*- coding: utf-8 -*-
 #
 # This file is part of Glances.
 #
 # SPDX-FileCopyrightText: 2022 Nicolas Hennion <nicolas@nicolargo.com>
 #
 # SPDX-License-Identifier: LGPL-3.0-only
 #
 
 """Manage sparklines for Glances output."""
 
-from __future__ import unicode_literals
-from __future__ import division
 import sys
-from glances.logger import logger
+
 from glances.globals import nativestr
+from glances.logger import logger
 
 sparklines_module = True
 
 try:
     from sparklines import sparklines
 except ImportError as e:
-    logger.warning("Sparklines module not found ({})".format(e))
+    logger.warning(f"Sparklines module not found ({e})")
     sparklines_module = False
 
 try:
     '┌┬┐╔╦╗╒╤╕╓╥╖│║─═├┼┤╠╬╣╞╪╡╟╫╢└┴┘╚╩╝╘╧╛╙╨╜'.encode(sys.stdout.encoding)
 except (UnicodeEncodeError, TypeError) as e:
-    logger.warning("UTF-8 is mandatory for sparklines ({})".format(e))
+    logger.warning(f"UTF-8 is mandatory for sparklines ({e})")
     sparklines_module = False
 
 
-class Sparkline(object):
+class Sparkline:
     """Manage sparklines (see https://pypi.org/project/sparklines/)."""
 
     def __init__(self, size, pre_char='[', post_char=']', unit_char='%', display_value=True):
         # If the sparklines python module available ?
         self.__available = sparklines_module
         # Sparkline size
         self.__size = size
@@ -54,14 +52,15 @@
     @property
     def size(self, with_decoration=False):
         # Return the sparkline size, with or without decoration
         if with_decoration:
             return self.__size
         if self.__display_value:
             return self.__size - 6
+        return None
 
     @property
     def percents(self):
         return self.__percent
 
     @percents.setter
     def percents(self, value):
@@ -77,15 +76,15 @@
 
     def get(self, overwrite=''):
         """Return the sparkline."""
         ret = sparklines(self.percents, minimum=0, maximum=100)[0]
         if self.__display_value:
             percents_without_none = [x for x in self.percents if x is not None]
             if len(percents_without_none) > 0:
-                ret = '{}{:5.1f}{}'.format(ret, percents_without_none[-1], self.__unit_char)
+                ret = f'{ret}{percents_without_none[-1]:5.1f}{self.__unit_char}'
         ret = nativestr(ret)
         if overwrite and len(overwrite) < len(ret) - 6:
             ret = overwrite + ret[len(overwrite) :]
         return ret
 
     def __str__(self):
         """Return the sparkline."""
```

### Comparing `glances-4.0.4/glances/outputs/glances_stdout.py` & `glances-4.0.5/glances/outputs/glances_stdout.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,25 +1,24 @@
-# -*- coding: utf-8 -*-
 #
 # This file is part of Glances.
 #
 # SPDX-FileCopyrightText: 2024 Nicolas Hennion <nicolas@nicolargo.com>
 #
 # SPDX-License-Identifier: LGPL-3.0-only
 #
 
 """Stdout interface class."""
 
 import time
 
-from glances.logger import logger
 from glances.globals import printandflush
+from glances.logger import logger
 
 
-class GlancesStdout(object):
+class GlancesStdout:
     """This class manages the Stdout display."""
 
     def __init__(self, config=None, args=None):
         # Init
         self.config = config
         self.args = args
 
@@ -61,29 +60,29 @@
             else:
                 continue
             # Display stats
             if attribute is not None:
                 # With attribute
                 if isinstance(stat, dict):
                     try:
-                        printandflush("{}.{}: {}".format(plugin, attribute, stat[attribute]))
+                        printandflush(f"{plugin}.{attribute}: {stat[attribute]}")
                     except KeyError as err:
-                        logger.error("Can not display stat {}.{} ({})".format(plugin, attribute, err))
+                        logger.error(f"Can not display stat {plugin}.{attribute} ({err})")
                 elif isinstance(stat, list):
                     for i in stat:
                         if key is None:
                             i_key = i[i['key']]
                         elif str(key) == str(i[i['key']]):
                             i_key = key
                         else:
                             continue
                         try:
-                            printandflush("{}.{}.{}: {}".format(plugin, i_key, attribute, i[attribute]))
+                            printandflush(f"{plugin}.{i_key}.{attribute}: {i[attribute]}")
                         except KeyError as err:
-                            logger.error("Can not display stat {}.{} ({})".format(plugin, attribute, err))
+                            logger.error(f"Can not display stat {plugin}.{attribute} ({err})")
             else:
                 # Without attribute
-                printandflush("{}: {}".format(plugin, stat))
+                printandflush(f"{plugin}: {stat}")
 
         # Wait until next refresh
         if duration > 0:
             time.sleep(duration)
```

### Comparing `glances-4.0.4/glances/outputs/glances_stdout_apidoc.py` & `glances-4.0.5/glances/outputs/glances_stdout_apidoc.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,36 +1,34 @@
-# -*- coding: utf-8 -*-
 #
 # This file is part of Glances.
 #
 # SPDX-FileCopyrightText: 2024 Nicolas Hennion <nicolas@nicolargo.com>
 #
 # SPDX-License-Identifier: LGPL-3.0-only
 #
 
 """Fields description interface class."""
 
-from pprint import pformat
 import json
 import time
+from pprint import pformat
 
 from glances import __apiversion__
-from glances.logger import logger
 from glances.globals import iteritems
+from glances.logger import logger
 
+API_URL = f"http://localhost:61208/api/{__apiversion__}"
 
-API_URL = "http://localhost:61208/api/{api_version}".format(api_version=__apiversion__)
-
-APIDOC_HEADER = """\
+APIDOC_HEADER = f"""\
 .. _api:
 
 API (Restfull/JSON) documentation
 =================================
 
-This documentation describes the Glances API version {api_version} (Restfull/JSON) interface.
+This documentation describes the Glances API version {__apiversion__} (Restfull/JSON) interface.
 
 For Glances version 3, please have a look on:
 ``https://github.com/nicolargo/glances/blob/support/glancesv3/docs/api.rst``
 
 Run the Glances API server
 --------------------------
 
@@ -41,94 +39,91 @@
     # glances -w --disable-webui
 
 It is also ran automatically when Glances is started in Web server mode (-w).
 
 API URL
 -------
 
-The default root API URL is ``http://localhost:61208/api/{api_version}``.
+The default root API URL is ``http://localhost:61208/api/{__apiversion__}``.
 
 The bind address and port could be changed using the ``--bind`` and ``--port`` command line options.
 
 It is also possible to define an URL prefix using the ``url_prefix`` option from the [outputs] section
 of the Glances configuration file.
 
 Note: The url_prefix should always end with a slash (``/``).
 
 For example:
 
 .. code-block:: ini
     [outputs]
     url_prefix = /glances/
 
-will change the root API URL to ``http://localhost:61208/glances/api/{api_version}`` and the Web UI URL to
+will change the root API URL to ``http://localhost:61208/glances/api/{__apiversion__}`` and the Web UI URL to
 ``http://localhost:61208/glances/``
 
 API documentation URL
 ---------------------
 
 The API documentation is embeded in the server and available at the following URL:
 ``http://localhost:61208/docs#/``.
 
 WebUI refresh
 -------------
 
 It is possible to change the Web UI refresh rate (default is 2 seconds) using the following option in the URL:
 ``http://localhost:61208/glances/?refresh=5``
 
-""".format(
-    api_version=__apiversion__
-)
+"""
 
 
 def indent_stat(stat, indent='    '):
     # Indent stats to pretty print it
     if isinstance(stat, list) and len(stat) > 1 and isinstance(stat[0], dict):
         # Only display two first items
         return indent + pformat(stat[0:2]).replace('\n', '\n' + indent).replace("'", '"')
-    else:
-        return indent + pformat(stat).replace('\n', '\n' + indent).replace("'", '"')
+    return indent + pformat(stat).replace('\n', '\n' + indent).replace("'", '"')
 
 
 def print_api_status():
     sub_title = 'GET API status'
     print(sub_title)
     print('-' * len(sub_title))
     print('')
     print('This entry point should be used to check the API status.')
     print('It will the Glances version and a 200 return code if everything is OK.')
     print('')
     print('Get the Rest API status::')
     print('')
-    print('    # curl -I {}/status'.format(API_URL))
+    print(f'    # curl -I {API_URL}/status')
     print(indent_stat('HTTP/1.0 200 OK'))
     print('')
 
 
 def print_plugins_list(stat):
     sub_title = 'GET plugins list'
     print(sub_title)
     print('-' * len(sub_title))
     print('')
     print('Get the plugins list::')
     print('')
-    print('    # curl {}/pluginslist'.format(API_URL))
+    print(f'    # curl {API_URL}/pluginslist')
     print(indent_stat(stat))
     print('')
 
 
 def print_plugin_stats(plugin, stat):
-    sub_title = 'GET {}'.format(plugin)
+    sub_title = f'GET {plugin}'
     print(sub_title)
     print('-' * len(sub_title))
     print('')
 
     print('Get plugin stats::')
     print('')
-    print('    # curl {}/{}'.format(API_URL, plugin))
+    print(f'    # curl {API_URL}/{plugin}')
     print(indent_stat(json.loads(stat.get_stats())))
     print('')
 
 
 def print_plugin_description(plugin, stat):
     if stat.fields_description:
         # For each plugins with a description
@@ -179,15 +174,15 @@
                 '* **{}**: {} (unit is *{}*)'.format(
                     'time_since_update', 'Number of seconds since last update', 'seconds'
                 )
             )
 
         print('')
     else:
-        logger.error('No fields_description variable defined for plugin {}'.format(plugin))
+        logger.error(f'No fields_description variable defined for plugin {plugin}')
 
 
 def print_plugin_item_value(plugin, stat, stat_export):
     item = None
     value = None
     if isinstance(stat_export, dict):
         item = list(stat_export.keys())[0]
@@ -201,70 +196,70 @@
         stat_item = json.loads(stat.get_stats_item(item))
         if isinstance(stat_item[item], list):
             value = stat_item[item][0]
         else:
             value = stat_item[item]
         print('Get a specific field::')
         print('')
-        print('    # curl {}/{}/{}'.format(API_URL, plugin, item))
+        print(f'    # curl {API_URL}/{plugin}/{item}')
         print(indent_stat(stat_item))
         print('')
     if item and value and stat.get_stats_value(item, value):
         print('Get a specific item when field matches the given value::')
         print('')
-        print('    # curl {}/{}/{}/{}'.format(API_URL, plugin, item, value))
+        print(f'    # curl {API_URL}/{plugin}/{item}/{value}')
         print(indent_stat(json.loads(stat.get_stats_value(item, value))))
         print('')
 
 
 def print_all():
     sub_title = 'GET all stats'
     print(sub_title)
     print('-' * len(sub_title))
     print('')
     print('Get all Glances stats::')
     print('')
-    print('    # curl {}/all'.format(API_URL))
+    print(f'    # curl {API_URL}/all')
     print('    Return a very big dictionary (avoid using this request, performances will be poor)...')
     print('')
 
 
 def print_top(stats):
     time.sleep(1)
     stats.update()
     sub_title = 'GET top n items of a specific plugin'
     print(sub_title)
     print('-' * len(sub_title))
     print('')
     print('Get top 2 processes of the processlist plugin::')
     print('')
-    print('    # curl {}/processlist/top/2'.format(API_URL))
+    print(f'    # curl {API_URL}/processlist/top/2')
     print(indent_stat(stats.get_plugin('processlist').get_export()[:2]))
     print('')
     print('Note: Only work for plugin with a list of items')
     print('')
 
 
 def print_fields_info(stats):
     sub_title = 'GET item description'
     print(sub_title)
     print('-' * len(sub_title))
     print('Get item description (human readable) for a specific plugin/item::')
     print('')
-    print('    # curl {}/diskio/read_bytes/description'.format(API_URL))
+    print(f'    # curl {API_URL}/diskio/read_bytes/description')
     print(indent_stat(stats.get_plugin('diskio').get_item_info('read_bytes', 'description')))
     print('')
     print('Note: the description is defined in the fields_description variable of the plugin.')
     print('')
     sub_title = 'GET item unit'
     print(sub_title)
     print('-' * len(sub_title))
     print('Get item unit for a specific plugin/item::')
     print('')
-    print('    # curl {}/diskio/read_bytes/unit'.format(API_URL))
+    print(f'    # curl {API_URL}/diskio/read_bytes/unit')
     print(indent_stat(stats.get_plugin('diskio').get_item_info('read_bytes', 'unit')))
     print('')
     print('Note: the description is defined in the fields_description variable of the plugin.')
     print('')
 
 
 def print_history(stats):
@@ -274,52 +269,52 @@
     stats.update()
     sub_title = 'GET stats history'
     print(sub_title)
     print('-' * len(sub_title))
     print('')
     print('History of a plugin::')
     print('')
-    print('    # curl {}/cpu/history'.format(API_URL))
+    print(f'    # curl {API_URL}/cpu/history')
     print(indent_stat(json.loads(stats.get_plugin('cpu').get_stats_history(nb=3))))
     print('')
     print('Limit history to last 2 values::')
     print('')
-    print('    # curl {}/cpu/history/2'.format(API_URL))
+    print(f'    # curl {API_URL}/cpu/history/2')
     print(indent_stat(json.loads(stats.get_plugin('cpu').get_stats_history(nb=2))))
     print('')
     print('History for a specific field::')
     print('')
-    print('    # curl {}/cpu/system/history'.format(API_URL))
+    print(f'    # curl {API_URL}/cpu/system/history')
     print(indent_stat(json.loads(stats.get_plugin('cpu').get_stats_history('system'))))
     print('')
     print('Limit history for a specific field to last 2 values::')
     print('')
-    print('    # curl {}/cpu/system/history'.format(API_URL))
+    print(f'    # curl {API_URL}/cpu/system/history')
     print(indent_stat(json.loads(stats.get_plugin('cpu').get_stats_history('system', nb=2))))
     print('')
 
 
 def print_limits(stats):
     sub_title = 'GET limits (used for thresholds)'
     print(sub_title)
     print('-' * len(sub_title))
     print('')
     print('All limits/thresholds::')
     print('')
-    print('    # curl {}/all/limits'.format(API_URL))
+    print(f'    # curl {API_URL}/all/limits')
     print(indent_stat(stats.getAllLimitsAsDict()))
     print('')
     print('Limits/thresholds for the cpu plugin::')
     print('')
-    print('    # curl {}/cpu/limits'.format(API_URL))
+    print(f'    # curl {API_URL}/cpu/limits')
     print(indent_stat(stats.get_plugin('cpu').limits))
     print('')
 
 
-class GlancesStdoutApiDoc(object):
+class GlancesStdoutApiDoc:
     """This class manages the fields description display."""
 
     def __init__(self, config=None, args=None):
         # Init
         self.config = config
         self.args = args
```

### Comparing `glances-4.0.4/glances/outputs/glances_stdout_csv.py` & `glances-4.0.5/glances/outputs/glances_stdout_csv.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 #
 # This file is part of Glances.
 #
 # SPDX-FileCopyrightText: 2022 Nicolas Hennion <nicolas@nicolargo.com>
 #
 # SPDX-License-Identifier: LGPL-3.0-only
 #
@@ -10,15 +9,15 @@
 """StdoutCsv interface class."""
 
 import time
 
 from glances.globals import printandflush
 
 
-class GlancesStdoutCsv(object):
+class GlancesStdoutCsv:
     """This class manages the StdoutCsv display."""
 
     separator = ','
     na = 'N/A'
 
     def __init__(self, config=None, args=None):
         # Init
@@ -49,46 +48,46 @@
         pass
 
     def build_header(self, plugin, attribute, stat):
         """Build and return the header line"""
         line = ''
 
         if attribute is not None:
-            line += '{}.{}{}'.format(plugin, attribute, self.separator)
+            line += f'{plugin}.{attribute}{self.separator}'
         else:
             if isinstance(stat, dict):
                 for k in stat.keys():
-                    line += '{}.{}{}'.format(plugin, str(k), self.separator)
+                    line += f'{plugin}.{str(k)}{self.separator}'
             elif isinstance(stat, list):
                 for i in stat:
                     if isinstance(i, dict) and 'key' in i:
                         for k in i.keys():
                             line += '{}.{}.{}{}'.format(plugin, str(i[i['key']]), str(k), self.separator)
             else:
-                line += '{}{}'.format(plugin, self.separator)
+                line += f'{plugin}{self.separator}'
 
         return line
 
     def build_data(self, plugin, attribute, stat):
         """Build and return the data line"""
         line = ''
 
         if attribute is not None:
-            line += '{}{}'.format(str(stat.get(attribute, self.na)), self.separator)
+            line += f'{str(stat.get(attribute, self.na))}{self.separator}'
         else:
             if isinstance(stat, dict):
                 for v in stat.values():
-                    line += '{}{}'.format(str(v), self.separator)
+                    line += f'{str(v)}{self.separator}'
             elif isinstance(stat, list):
                 for i in stat:
                     if isinstance(i, dict) and 'key' in i:
                         for v in i.values():
-                            line += '{}{}'.format(str(v), self.separator)
+                            line += f'{str(v)}{self.separator}'
             else:
-                line += '{}{}'.format(str(stat), self.separator)
+                line += f'{str(stat)}{self.separator}'
 
         return line
 
     def update(self, stats, duration=3):
         """Display stats to stdout.
 
         Refresh every duration second.
```

### Comparing `glances-4.0.4/glances/outputs/glances_stdout_issue.py` & `glances-4.0.5/glances/outputs/glances_stdout_issue.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,29 +1,28 @@
-# -*- coding: utf-8 -*-
 #
 # This file is part of Glances.
 #
 # SPDX-FileCopyrightText: 2024 Nicolas Hennion <nicolas@nicolargo.com>
 #
 # SPDX-License-Identifier: LGPL-3.0-only
 #
 
 """Issue interface class."""
 
 import os
-import sys
 import platform
-import time
 import pprint
-
-from glances.timer import Counter
-from glances import __version__, psutil_version
+import sys
+import time
 
 import psutil
+
 import glances
+from glances import __version__, psutil_version
+from glances.timer import Counter
 
 TERMINAL_WIDTH = 79
 
 
 class colors:
     RED = '\033[91m'
     GREEN = '\033[92m'
@@ -35,39 +34,35 @@
         self.RED = ''
         self.GREEN = ''
         self.BLUE = ''
         self.ORANGE = ''
         self.NO = ''
 
 
-class GlancesStdoutIssue(object):
+class GlancesStdoutIssue:
     """This class manages the Issue display."""
 
     def __init__(self, config=None, args=None):
         # Init
         self.config = config
         self.args = args
 
     def end(self):
         pass
 
     def print_version(self):
         sys.stdout.write('=' * TERMINAL_WIDTH + '\n')
-        sys.stdout.write(
-            'Glances {} ({})\n'.format(colors.BLUE + __version__ + colors.NO, os.path.realpath(glances.__file__))
-        )
-        sys.stdout.write('Python {} ({})\n'.format(colors.BLUE + platform.python_version() + colors.NO, sys.executable))
-        sys.stdout.write(
-            'PsUtil {} ({})\n'.format(colors.BLUE + psutil_version + colors.NO, os.path.realpath(psutil.__file__))
-        )
+        sys.stdout.write(f'Glances {colors.BLUE + __version__ + colors.NO} ({os.path.realpath(glances.__file__)})\n')
+        sys.stdout.write(f'Python {colors.BLUE + platform.python_version() + colors.NO} ({sys.executable})\n')
+        sys.stdout.write(f'PsUtil {colors.BLUE + psutil_version + colors.NO} ({os.path.realpath(psutil.__file__)})\n')
         sys.stdout.write('=' * TERMINAL_WIDTH + '\n')
         sys.stdout.flush()
 
     def print_issue(self, plugin, result, message):
-        sys.stdout.write('{}{}{}'.format(colors.BLUE + plugin, result, message))
+        sys.stdout.write(f'{colors.BLUE + plugin}{result}{message}')
         sys.stdout.write(colors.NO + '\n')
         sys.stdout.flush()
 
     def update(self, stats, duration=3):
         """Display issue"""
         self.print_version()
 
@@ -104,32 +99,28 @@
                 # Hide private information
                 if plugin == 'ip':
                     for key in stat.keys():
                         stat[key] = '***'
             except Exception as e:
                 stat_error = e
             if stat_error is None:
-                result = (colors.GREEN + '[OK]   ' + colors.BLUE + ' {:.5f}s '.format(counter.get())).rjust(
-                    41 - len(plugin)
-                )
+                result = (colors.GREEN + '[OK]   ' + colors.BLUE + f' {counter.get():.5f}s ').rjust(41 - len(plugin))
                 if isinstance(stat, list) and len(stat) > 0 and 'key' in stat[0]:
                     key = 'key={} '.format(stat[0]['key'])
                     stat_output = pprint.pformat([stat[0]], compact=True, width=120, depth=3)
                     message = colors.ORANGE + key + colors.NO + '\n' + stat_output[0:-1] + ', ...' + stat_output[-1]
                 else:
                     message = '\n' + colors.NO + pprint.pformat(stat, compact=True, width=120, depth=2)
             else:
-                result = (colors.RED + '[ERROR]' + colors.BLUE + ' {:.5f}s '.format(counter.get())).rjust(
-                    41 - len(plugin)
-                )
+                result = (colors.RED + '[ERROR]' + colors.BLUE + f' {counter.get():.5f}s ').rjust(41 - len(plugin))
                 message = colors.NO + str(stat_error)[0 : TERMINAL_WIDTH - 41]
 
             # Display the result
             self.print_issue(plugin, result, message)
 
         # Display total time need to update all plugins
         sys.stdout.write('=' * TERMINAL_WIDTH + '\n')
-        print("Total time to update all stats: {}{:.5f}s{}".format(colors.BLUE, counter_total.get(), colors.NO))
+        print(f"Total time to update all stats: {colors.BLUE}{counter_total.get():.5f}s{colors.NO}")
         sys.stdout.write('=' * TERMINAL_WIDTH + '\n')
 
         # Return True to exit directly (no refresh)
         return True
```

### Comparing `glances-4.0.4/glances/outputs/glances_stdout_json.py` & `glances-4.0.5/glances/outputs/glances_stdout_json.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 #
 # This file is part of Glances.
 #
 # SPDX-FileCopyrightText: 2022 Nicolas Hennion <nicolas@nicolargo.com>
 #
 # SPDX-License-Identifier: LGPL-3.0-only
 #
@@ -10,15 +9,15 @@
 """Stdout interface class."""
 
 import time
 
 from glances.globals import printandflush
 
 
-class GlancesStdoutJson(object):
+class GlancesStdoutJson:
     """This class manages the Stdout JSON display."""
 
     def __init__(self, config=None, args=None):
         # Init
         self.config = config
         self.args = args
 
@@ -43,12 +42,12 @@
         for plugin in self.plugins_list:
             # Check if the plugin exist and is enable
             if plugin in stats.getPluginsList() and stats.get_plugin(plugin).is_enabled():
                 stat = stats.get_plugin(plugin).get_json()
             else:
                 continue
             # Display stats
-            printandflush('{}: {}'.format(plugin, stat))
+            printandflush(f'{plugin}: {stat}')
 
         # Wait until next refresh
         if duration > 0:
             time.sleep(duration)
```

### Comparing `glances-4.0.4/glances/outputs/glances_unicode.py` & `glances-4.0.5/glances/outputs/glances_unicode.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,29 +1,27 @@
-# -*- coding: utf-8 -*-
 #
 # This file is part of Glances.
 #
 # SPDX-FileCopyrightText: 2022 Nicolas Hennion <nicolas@nicolargo.com>
 #
 # SPDX-License-Identifier: LGPL-3.0-only
 #
 
 """Manage unicode message for Glances output."""
 
 _unicode_message = {
-    'ARROW_LEFT': [u'\u2190', u'<'],
-    'ARROW_RIGHT': [u'\u2192', u'>'],
-    'ARROW_UP': [u'\u2191', u'^'],
-    'ARROW_DOWN': [u'\u2193', u'v'],
-    'CHECK': [u'\u2713', u''],
-    'PROCESS_SELECTOR': [u'>', u'>'],
-    'MEDIUM_LINE': [u'\u23AF', u'-'],
-    'LOW_LINE': [u'\u2581', u'_'],
+    'ARROW_LEFT': ['\u2190', '<'],
+    'ARROW_RIGHT': ['\u2192', '>'],
+    'ARROW_UP': ['\u2191', '^'],
+    'ARROW_DOWN': ['\u2193', 'v'],
+    'CHECK': ['\u2713', ''],
+    'PROCESS_SELECTOR': ['>', '>'],
+    'MEDIUM_LINE': ['\u23af', '-'],
+    'LOW_LINE': ['\u2581', '_'],
 }
 
 
 def unicode_message(key, args=None):
     """Return the unicode message for the given key."""
     if args and hasattr(args, 'disable_unicode') and args.disable_unicode:
         return _unicode_message[key][1]
-    else:
-        return _unicode_message[key][0]
+    return _unicode_message[key][0]
```

### Comparing `glances-4.0.4/glances/outputs/static/README.md` & `glances-4.0.5/glances/outputs/static/README.md`

 * *Files identical despite different names*

### Comparing `glances-4.0.4/glances/outputs/static/css/bootstrap.less` & `glances-4.0.5/glances/outputs/static/css/bootstrap.less`

 * *Files identical despite different names*

### Comparing `glances-4.0.4/glances/outputs/static/css/style.scss` & `glances-4.0.5/glances/outputs/static/css/style.scss`

 * *Files identical despite different names*

### Comparing `glances-4.0.4/glances/outputs/static/images/favicon.ico` & `glances-4.0.5/glances/outputs/static/images/favicon.ico`

 * *Files identical despite different names*

### Comparing `glances-4.0.4/glances/outputs/static/images/glances.png` & `glances-4.0.5/glances/outputs/static/images/glances.png`

 * *Files identical despite different names*

### Comparing `glances-4.0.4/glances/outputs/static/js/App.vue` & `glances-4.0.5/glances/outputs/static/js/App.vue`

 * *Files identical despite different names*

### Comparing `glances-4.0.4/glances/outputs/static/js/components/help.vue` & `glances-4.0.5/glances/outputs/static/js/components/help.vue`

 * *Files identical despite different names*

### Comparing `glances-4.0.4/glances/outputs/static/js/components/plugin-alert.vue` & `glances-4.0.5/glances/outputs/static/js/components/plugin-alert.vue`

 * *Files identical despite different names*

### Comparing `glances-4.0.4/glances/outputs/static/js/components/plugin-amps.vue` & `glances-4.0.5/glances/outputs/static/js/components/plugin-amps.vue`

 * *Files identical despite different names*

### Comparing `glances-4.0.4/glances/outputs/static/js/components/plugin-cloud.vue` & `glances-4.0.5/glances/outputs/static/js/components/plugin-cloud.vue`

 * *Files identical despite different names*

### Comparing `glances-4.0.4/glances/outputs/static/js/components/plugin-connections.vue` & `glances-4.0.5/glances/outputs/static/js/components/plugin-connections.vue`

 * *Files identical despite different names*

### Comparing `glances-4.0.4/glances/outputs/static/js/components/plugin-containers.vue` & `glances-4.0.5/glances/outputs/static/js/components/plugin-containers.vue`

 * *Files identical despite different names*

### Comparing `glances-4.0.4/glances/outputs/static/js/components/plugin-cpu.vue` & `glances-4.0.5/glances/outputs/static/js/components/plugin-cpu.vue`

 * *Files identical despite different names*

### Comparing `glances-4.0.4/glances/outputs/static/js/components/plugin-diskio.vue` & `glances-4.0.5/glances/outputs/static/js/components/plugin-diskio.vue`

 * *Files identical despite different names*

### Comparing `glances-4.0.4/glances/outputs/static/js/components/plugin-folders.vue` & `glances-4.0.5/glances/outputs/static/js/components/plugin-folders.vue`

 * *Files identical despite different names*

### Comparing `glances-4.0.4/glances/outputs/static/js/components/plugin-fs.vue` & `glances-4.0.5/glances/outputs/static/js/components/plugin-fs.vue`

 * *Files identical despite different names*

### Comparing `glances-4.0.4/glances/outputs/static/js/components/plugin-gpu.vue` & `glances-4.0.5/glances/outputs/static/js/components/plugin-gpu.vue`

 * *Files identical despite different names*

### Comparing `glances-4.0.4/glances/outputs/static/js/components/plugin-ip.vue` & `glances-4.0.5/glances/outputs/static/js/components/plugin-ip.vue`

 * *Files identical despite different names*

### Comparing `glances-4.0.4/glances/outputs/static/js/components/plugin-irq.vue` & `glances-4.0.5/glances/outputs/static/js/components/plugin-irq.vue`

 * *Files identical despite different names*

### Comparing `glances-4.0.4/glances/outputs/static/js/components/plugin-load.vue` & `glances-4.0.5/glances/outputs/static/js/components/plugin-load.vue`

 * *Files identical despite different names*

### Comparing `glances-4.0.4/glances/outputs/static/js/components/plugin-mem-more.vue` & `glances-4.0.5/glances/outputs/static/js/components/plugin-mem-more.vue`

 * *Files identical despite different names*

### Comparing `glances-4.0.4/glances/outputs/static/js/components/plugin-mem.vue` & `glances-4.0.5/glances/outputs/static/js/components/plugin-mem.vue`

 * *Files identical despite different names*

### Comparing `glances-4.0.4/glances/outputs/static/js/components/plugin-memswap.vue` & `glances-4.0.5/glances/outputs/static/js/components/plugin-memswap.vue`

 * *Files identical despite different names*

### Comparing `glances-4.0.4/glances/outputs/static/js/components/plugin-network.vue` & `glances-4.0.5/glances/outputs/static/js/components/plugin-network.vue`

 * *Files identical despite different names*

### Comparing `glances-4.0.4/glances/outputs/static/js/components/plugin-now.vue` & `glances-4.0.5/glances/outputs/static/js/components/plugin-now.vue`

 * *Files identical despite different names*

### Comparing `glances-4.0.4/glances/outputs/static/js/components/plugin-percpu.vue` & `glances-4.0.5/glances/outputs/static/js/components/plugin-percpu.vue`

 * *Files identical despite different names*

### Comparing `glances-4.0.4/glances/outputs/static/js/components/plugin-ports.vue` & `glances-4.0.5/glances/outputs/static/js/components/plugin-ports.vue`

 * *Files identical despite different names*

### Comparing `glances-4.0.4/glances/outputs/static/js/components/plugin-process.vue` & `glances-4.0.5/glances/outputs/static/js/components/plugin-process.vue`

 * *Files identical despite different names*

### Comparing `glances-4.0.4/glances/outputs/static/js/components/plugin-processcount.vue` & `glances-4.0.5/glances/outputs/static/js/components/plugin-processcount.vue`

 * *Files identical despite different names*

### Comparing `glances-4.0.4/glances/outputs/static/js/components/plugin-processlist.vue` & `glances-4.0.5/glances/outputs/static/js/components/plugin-processlist.vue`

 * *Files identical despite different names*

### Comparing `glances-4.0.4/glances/outputs/static/js/components/plugin-quicklook.vue` & `glances-4.0.5/glances/outputs/static/js/components/plugin-quicklook.vue`

 * *Files identical despite different names*

### Comparing `glances-4.0.4/glances/outputs/static/js/components/plugin-raid.vue` & `glances-4.0.5/glances/outputs/static/js/components/plugin-raid.vue`

 * *Files identical despite different names*

### Comparing `glances-4.0.4/glances/outputs/static/js/components/plugin-sensors.vue` & `glances-4.0.5/glances/outputs/static/js/components/plugin-sensors.vue`

 * *Files identical despite different names*

### Comparing `glances-4.0.4/glances/outputs/static/js/components/plugin-smart.vue` & `glances-4.0.5/glances/outputs/static/js/components/plugin-smart.vue`

 * *Files identical despite different names*

### Comparing `glances-4.0.4/glances/outputs/static/js/components/plugin-system.vue` & `glances-4.0.5/glances/outputs/static/js/components/plugin-system.vue`

 * *Files identical despite different names*

### Comparing `glances-4.0.4/glances/outputs/static/js/components/plugin-wifi.vue` & `glances-4.0.5/glances/outputs/static/js/components/plugin-wifi.vue`

 * *Files identical despite different names*

### Comparing `glances-4.0.4/glances/outputs/static/js/filters.js` & `glances-4.0.5/glances/outputs/static/js/filters.js`

 * *Files identical despite different names*

### Comparing `glances-4.0.4/glances/outputs/static/js/services.js` & `glances-4.0.5/glances/outputs/static/js/services.js`

 * *Files identical despite different names*

### Comparing `glances-4.0.4/glances/outputs/static/package-lock.json` & `glances-4.0.5/glances/outputs/static/package-lock.json`

 * *Files identical despite different names*

### Comparing `glances-4.0.4/glances/outputs/static/package.json` & `glances-4.0.5/glances/outputs/static/package.json`

 * *Files identical despite different names*

### Comparing `glances-4.0.4/glances/outputs/static/public/1272f6e9e8f9d6bfd6de.png` & `glances-4.0.5/glances/outputs/static/public/1272f6e9e8f9d6bfd6de.png`

 * *Files identical despite different names*

### Comparing `glances-4.0.4/glances/outputs/static/public/favicon.ico` & `glances-4.0.5/glances/outputs/static/public/favicon.ico`

 * *Files identical despite different names*

### Comparing `glances-4.0.4/glances/outputs/static/public/glances.js` & `glances-4.0.5/glances/outputs/static/public/glances.js`

 * *Files identical despite different names*

### Comparing `glances-4.0.4/glances/outputs/static/webpack.config.js` & `glances-4.0.5/glances/outputs/static/webpack.config.js`

 * *Files identical despite different names*

### Comparing `glances-4.0.4/glances/password.py` & `glances-4.0.5/glances/password.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,31 +1,30 @@
-# -*- coding: utf-8 -*-
 #
 # This file is part of Glances.
 #
 # SPDX-FileCopyrightText: 2024 Nicolas Hennion <nicolas@nicolargo.com>
 #
 # SPDX-License-Identifier: LGPL-3.0-only
 #
 
 """Manage password."""
 
+import builtins
 import getpass
 import hashlib
 import os
 import sys
 import uuid
-from io import open
 
-from glances.globals import b, safe_makedirs, weak_lru_cache
 from glances.config import user_config_dir
+from glances.globals import b, safe_makedirs, weak_lru_cache
 from glances.logger import logger
 
 
-class GlancesPassword(object):
+class GlancesPassword:
     """This class contains all the methods relating to password."""
 
     def __init__(self, username='glances', config=None):
         self.username = username
 
         self.config = config
         self.password_dir = self.local_password_path()
@@ -34,16 +33,15 @@
 
     def local_password_path(self):
         """Return the local password path.
         Related to issue: Password files in same configuration dir in effect #2143
         """
         if self.config is None:
             return user_config_dir()[0]
-        else:
-            return self.config.get_value('passwords', 'local_password_path', default=user_config_dir()[0])
+        return self.config.get_value('passwords', 'local_password_path', default=user_config_dir()[0])
 
     @weak_lru_cache(maxsize=32)
     def get_hash(self, plain_password, salt=''):
         """Return the hashed password, salt + pbkdf2_hmac."""
         return hashlib.pbkdf2_hmac('sha256', plain_password.encode(), salt.encode(), 100000, dklen=128).hex()
 
     @weak_lru_cache(maxsize=32)
@@ -74,15 +72,15 @@
         For Glances client, get the password (confirm=False, clear=True):
             1) from the CLI
             2) the password is hashed with SHA-pbkdf2_hmac (only SHA string transit
                through the network)
         """
         if os.path.exists(self.password_file) and not clear:
             # If the password file exist then use it
-            logger.info("Read password from file {}".format(self.password_file))
+            logger.info(f"Read password from file {self.password_file}")
             password = self.load_password()
         else:
             # password_hash is the plain SHA-pbkdf2_hmac password
             # password_hashed is the salt + SHA-pbkdf2_hmac password
             password_hash = self.get_hash(getpass.getpass(description))
             password_hashed = self.hash_password(password_hash)
             if confirm:
@@ -109,17 +107,15 @@
 
     def save_password(self, hashed_password):
         """Save the hashed password to the Glances folder."""
         # Create the glances directory
         safe_makedirs(self.password_dir)
 
         # Create/overwrite the password file
-        with open(self.password_file, 'wb') as file_pwd:
+        with builtins.open(self.password_file, 'wb') as file_pwd:
             file_pwd.write(b(hashed_password))
 
     def load_password(self):
         """Load the hashed password from the Glances folder."""
         # Read the password file, if it exists
-        with open(self.password_file, 'r') as file_pwd:
-            hashed_password = file_pwd.read()
-
-        return hashed_password
+        with builtins.open(self.password_file) as file_pwd:
+            return file_pwd.read()
```

### Comparing `glances-4.0.4/glances/password_list.py` & `glances-4.0.5/glances/password_list.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 #
 # This file is part of Glances.
 #
 # SPDX-FileCopyrightText: 2022 Nicolas Hennion <nicolas@nicolargo.com>
 #
 # SPDX-License-Identifier: LGPL-3.0-only
 #
@@ -15,51 +14,51 @@
 
 class GlancesPasswordList(GlancesPassword):
     """Manage the Glances passwords list for the client|browser/server."""
 
     _section = "passwords"
 
     def __init__(self, config=None, args=None):
-        super(GlancesPasswordList, self).__init__()
+        super().__init__()
         # password_dict is a dict (JSON compliant)
         # {'host': 'password', ... }
         # Load the configuration file
         self._password_dict = self.load(config)
 
     def load(self, config):
         """Load the password from the configuration file."""
         password_dict = {}
 
         if config is None:
             logger.warning("No configuration file available. Cannot load password list.")
         elif not config.has_section(self._section):
-            logger.warning("No [%s] section in the configuration file. Cannot load password list." % self._section)
+            logger.warning(f"No [{self._section}] section in the configuration file. Cannot load password list.")
         else:
-            logger.info("Start reading the [%s] section in the configuration file" % self._section)
+            logger.info(f"Start reading the [{self._section}] section in the configuration file")
 
             password_dict = dict(config.items(self._section))
 
             # Password list loaded
-            logger.info("%s password(s) loaded from the configuration file" % len(password_dict))
+            logger.info(f"{len(password_dict)} password(s) loaded from the configuration file")
 
         return password_dict
 
     def get_password(self, host=None):
         """Get the password from a Glances client or server.
 
         If host=None, return the current server list (dict).
         Else, return the host's password (or the default one if defined or None)
         """
         if host is None:
             return self._password_dict
-        else:
+
+        try:
+            return self._password_dict[host]
+        except (KeyError, TypeError):
             try:
-                return self._password_dict[host]
+                return self._password_dict['default']
             except (KeyError, TypeError):
-                try:
-                    return self._password_dict['default']
-                except (KeyError, TypeError):
-                    return None
+                return None
 
     def set_password(self, host, password):
         """Set a password for a specific host."""
         self._password_dict[host] = password
```

### Comparing `glances-4.0.4/glances/plugins/alert/__init__.py` & `glances-4.0.5/glances/plugins/alert/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 #
 # This file is part of Glances.
 #
 # SPDX-FileCopyrightText: 2024 Nicolas Hennion <nicolas@nicolargo.com>
 #
 # SPDX-License-Identifier: LGPL-3.0-only
 #
@@ -97,17 +96,15 @@
     """Glances alert plugin.
 
     Only for display.
     """
 
     def __init__(self, args=None, config=None):
         """Init the plugin."""
-        super(PluginModel, self).__init__(
-            args=args, config=config, stats_init_value=[], fields_description=fields_description
-        )
+        super().__init__(args=args, config=config, stats_init_value=[], fields_description=fields_description)
 
         # We want to display the stat in the curse interface
         self.display_curse = True
 
         # Set the message position
         self.align = 'bottom'
 
@@ -170,18 +167,17 @@
                 msg = ' ({:.1f})'.format(alert['avg'])
             else:
                 msg = ' (Min:{:.1f} Mean:{:.1f} Max:{:.1f})'.format(alert['min'], alert['avg'], alert['max'])
             ret.append(self.curse_add_line(msg))
             # Top processes
             top_process = ', '.join(alert['top'])
             if top_process != '':
-                msg = ': {}'.format(top_process)
+                msg = f': {top_process}'
                 ret.append(self.curse_add_line(msg))
 
         return ret
 
     def approx_equal(self, a, b, tolerance=0.0):
         """Compare a with b using the tolerance (if numerical)."""
         if str(int(a)).isdigit() and str(int(b)).isdigit():
             return abs(a - b) <= max(abs(a), abs(b)) * tolerance
-        else:
-            return a == b
+        return a == b
```

### Comparing `glances-4.0.4/glances/plugins/amps/__init__.py` & `glances-4.0.5/glances/plugins/amps/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,19 @@
-# -*- coding: utf-8 -*-
 #
 # This file is part of Glances.
 #
 # SPDX-FileCopyrightText: 2024 Nicolas Hennion <nicolas@nicolargo.com>
 #
 # SPDX-License-Identifier: LGPL-3.0-only
 #
 
 """Monitor plugin."""
 
-from glances.globals import iteritems
 from glances.amps_list import AmpsList as glancesAmpsList
+from glances.globals import iteritems
 from glances.plugins.plugin.model import GlancesPluginModel
 
 # Fields description
 # description: human readable description
 # short_name: shortname to use un UI
 # unit: unit type
 # rate: is it a rate ? If yes, // by time_since_update when displayed,
@@ -31,17 +30,15 @@
 
 
 class PluginModel(GlancesPluginModel):
     """Glances AMPs plugin."""
 
     def __init__(self, args=None, config=None):
         """Init the plugin."""
-        super(PluginModel, self).__init__(
-            args=args, config=config, stats_init_value=[], fields_description=fields_description
-        )
+        super().__init__(args=args, config=config, stats_init_value=[], fields_description=fields_description)
         self.args = args
         self.config = config
 
         # We want to display the stat in the curse interface
         self.display_curse = True
 
         # Init the list of AMP (classes define in the glances/amps_list.py script)
@@ -89,21 +86,19 @@
         if countmin is None:
             countmin = nbprocess
         if countmax is None:
             countmax = nbprocess
         if nbprocess > 0:
             if int(countmin) <= int(nbprocess) <= int(countmax):
                 return 'OK'
-            else:
-                return 'WARNING'
-        else:
-            if int(countmin) == 0:
-                return 'OK'
-            else:
-                return 'CRITICAL'
+            return 'WARNING'
+
+        if int(countmin) == 0:
+            return 'OK'
+        return 'CRITICAL'
 
     def msg_curse(self, args=None, max_width=None):
         """Return the dict to display in the curse interface."""
         # Init the return message
         # Only process if stats exist and display plugin enable...
         ret = []
 
@@ -117,18 +112,18 @@
                 continue
             # Display AMP
             first_column = '{}'.format(m['name'])
             first_column_style = self.get_alert(m['count'], m['countmin'], m['countmax'])
             second_column = '{}'.format(m['count'] if m['regex'] else '')
             for line in m['result'].split('\n'):
                 # Display first column with the process name...
-                msg = '{:<16} '.format(first_column)
+                msg = f'{first_column:<16} '
                 ret.append(self.curse_add_line(msg, first_column_style))
                 # ... and second column with the number of matching processes...
-                msg = '{:<4} '.format(second_column)
+                msg = f'{second_column:<4} '
                 ret.append(self.curse_add_line(msg))
                 # ... only on the first line
                 first_column = second_column = ''
                 # Display AMP result in the third column
                 ret.append(self.curse_add_line(line, splittable=True))
                 ret.append(self.curse_new_line())
```

### Comparing `glances-4.0.4/glances/plugins/cloud/__init__.py` & `glances-4.0.5/glances/plugins/cloud/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 #
 # This file is part of Glances.
 #
 # SPDX-FileCopyrightText: 2022 Nicolas Hennion <nicolas@nicolargo.com>
 #
 # SPDX-License-Identifier: LGPL-3.0-only
 #
@@ -13,24 +12,24 @@
 - OpenStack meta data (class ThreadOpenStack) - Vanilla OpenStack
 - OpenStackEC2 meta data (class ThreadOpenStackEC2) - Amazon EC2 compatible
 """
 
 import threading
 
 from glances.globals import iteritems, to_ascii
-from glances.plugins.plugin.model import GlancesPluginModel
 from glances.logger import logger
+from glances.plugins.plugin.model import GlancesPluginModel
 
 # Import plugin specific dependency
 try:
     import requests
 except ImportError as e:
     import_error_tag = True
     # Display debug message if import error
-    logger.warning("Missing Python Lib ({}), Cloud plugin is disabled".format(e))
+    logger.warning(f"Missing Python Lib ({e}), Cloud plugin is disabled")
 else:
     import_error_tag = False
 
 
 class PluginModel(GlancesPluginModel):
     """Glances' cloud plugin.
 
@@ -40,15 +39,15 @@
     See https://github.com/nicolargo/glances/issues/1029
 
     stats is a dict
     """
 
     def __init__(self, args=None, config=None):
         """Init the plugin."""
-        super(PluginModel, self).__init__(args=args, config=config)
+        super().__init__(args=args, config=config)
 
         # We want to display the stat in the curse interface
         self.display_curse = True
 
         # Init the stats
         self.reset()
 
@@ -61,15 +60,15 @@
         self.OPENSTACKEC2.start()
 
     def exit(self):
         """Overwrite the exit method to close threads."""
         self.OPENSTACK.stop()
         self.OPENSTACKEC2.stop()
         # Call the father class
-        super(PluginModel, self).exit()
+        super().exit()
 
     @GlancesPluginModel._check_decorator
     @GlancesPluginModel._log_result_decorator
     def update(self):
         """Update the cloud stats.
 
         Return the stats (dict)
@@ -141,15 +140,15 @@
         'type': 'meta/role',
         'region': 'availability_zone',
     }
 
     def __init__(self):
         """Init the class."""
         logger.debug("cloud plugin - Create thread for OpenStack metadata")
-        super(ThreadOpenStack, self).__init__()
+        super().__init__()
         # Event needed to stop properly the thread
         self._stopper = threading.Event()
         # The class return the stats as a dict
         self._stats = {}
 
     def run(self):
         """Grab plugin's stats.
@@ -157,20 +156,20 @@
         Infinite loop, should be stopped by calling the stop() method
         """
         if import_error_tag:
             self.stop()
             return False
 
         for k, v in iteritems(self.OPENSTACK_API_METADATA):
-            r_url = '{}/{}'.format(self.OPENSTACK_API_URL, v)
+            r_url = f'{self.OPENSTACK_API_URL}/{v}'
             try:
                 # Local request, a timeout of 3 seconds is OK
                 r = requests.get(r_url, timeout=3)
             except Exception as e:
-                logger.debug('cloud plugin - Cannot connect to the OpenStack metadata API {}: {}'.format(r_url, e))
+                logger.debug(f'cloud plugin - Cannot connect to the OpenStack metadata API {r_url}: {e}')
                 break
             else:
                 if r.ok:
                     self._stats[k] = to_ascii(r.content)
         else:
             # No break during the loop, so we can set the platform
             self._stats['platform'] = self.OPENSTACK_PLATFORM
```

### Comparing `glances-4.0.4/glances/plugins/connections/__init__.py` & `glances-4.0.5/glances/plugins/connections/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,22 @@
-# -*- coding: utf-8 -*-
 #
 # This file is part of Glances.
 #
 # SPDX-FileCopyrightText: 2024 Nicolas Hennion <nicolas@nicolargo.com>
 #
 # SPDX-License-Identifier: LGPL-3.0-only
 #
 
 """Connections plugin."""
-from __future__ import unicode_literals
 
+import psutil
+
+from glances.globals import nativestr
 from glances.logger import logger
 from glances.plugins.plugin.model import GlancesPluginModel
-from glances.globals import nativestr
-
-import psutil
 
 # Fields description
 # description: human readable description
 # short_name: shortname to use un UI
 # unit: unit type
 # rate: is it a rate ? If yes, // by time_since_update when displayed,
 # min_symbol: Auto unit should be used if value > than 1 'X' (K, M, G)...
@@ -89,15 +87,15 @@
     conntrack = {
         'nf_conntrack_count': '/proc/sys/net/netfilter/nf_conntrack_count',
         'nf_conntrack_max': '/proc/sys/net/netfilter/nf_conntrack_max',
     }
 
     def __init__(self, args=None, config=None):
         """Init the plugin."""
-        super(PluginModel, self).__init__(
+        super().__init__(
             args=args,
             config=config,
             # items_history_list=items_history_list,
             stats_init_value={'net_connections_enabled': True, 'nf_conntrack_enabled': True},
             fields_description=fields_description,
         )
 
@@ -118,15 +116,15 @@
             # Update stats using the PSUtils lib
 
             # Grab network interface stat using the psutil net_connections method
             if stats['net_connections_enabled']:
                 try:
                     net_connections = psutil.net_connections(kind="tcp")
                 except Exception as e:
-                    logger.warning('Can not get network connections stats ({})'.format(e))
+                    logger.warning(f'Can not get network connections stats ({e})')
                     logger.info('Disable connections stats')
                     stats['net_connections_enabled'] = False
                     self.stats = stats
                     return self.stats
 
                 for s in self.status_list:
                     stats[s] = len([c for c in net_connections if c.status == s])
@@ -141,18 +139,18 @@
                     terminated += stats[s]
                 stats['terminated'] = terminated
 
             if stats['nf_conntrack_enabled']:
                 # Grab connections track directly from the /proc file
                 for i in self.conntrack:
                     try:
-                        with open(self.conntrack[i], 'r') as f:
+                        with open(self.conntrack[i]) as f:
                             stats[i] = float(f.readline().rstrip("\n"))
-                    except (IOError, FileNotFoundError) as e:
-                        logger.warning('Can not get network connections track ({})'.format(e))
+                    except (OSError, FileNotFoundError) as e:
+                        logger.warning(f'Can not get network connections track ({e})')
                         logger.info('Disable connections track')
                         stats['nf_conntrack_enabled'] = False
                         self.stats = stats
                         return self.stats
                 if 'nf_conntrack_max' in stats and 'nf_conntrack_count' in stats:
                     stats['nf_conntrack_percent'] = stats['nf_conntrack_count'] * 100 / stats['nf_conntrack_max']
                 else:
@@ -167,15 +165,15 @@
         # Update the stats
         self.stats = stats
         return self.stats
 
     def update_views(self):
         """Update stats views."""
         # Call the father's method
-        super(PluginModel, self).update_views()
+        super().update_views()
 
         # Add specific information
         try:
             # Alert and log
             if self.stats['nf_conntrack_enabled']:
                 self.views['nf_conntrack_percent']['decoration'] = self.get_alert(header='nf_conntrack_percent')
         except KeyError:
```

### Comparing `glances-4.0.4/glances/plugins/containers/__init__.py` & `glances-4.0.5/glances/plugins/containers/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 #
 # This file is part of Glances.
 #
 # SPDX-FileCopyrightText: 2022 Nicolas Hennion <nicolas@nicolargo.com>
 #
 # SPDX-License-Identifier: LGPL-3.0-only
 #
@@ -123,15 +122,15 @@
     """Glances Docker plugin.
 
     stats is a dict: {'version': {...}, 'containers': [{}, {}]}
     """
 
     def __init__(self, args=None, config=None):
         """Init the plugin."""
-        super(PluginModel, self).__init__(
+        super().__init__(
             args=args, config=config, items_history_list=items_history_list, fields_description=fields_description
         )
 
         # The plugin can be disabled using: args.disable_docker
         self.args = args
 
         # Default config keys
@@ -160,40 +159,39 @@
         """Return the podman sock.
         Could be desfined in the [docker] section thanks to the podman_sock option.
         Default value: unix:///run/user/1000/podman/podman.sock
         """
         conf_podman_sock = self.get_conf_value('podman_sock')
         if len(conf_podman_sock) == 0:
             return "unix:///run/user/1000/podman/podman.sock"
-        else:
-            return conf_podman_sock[0]
+        return conf_podman_sock[0]
 
     def exit(self):
         """Overwrite the exit method to close threads."""
         if self.docker_extension:
             self.docker_extension.stop()
         if self.podman_extension:
             self.podman_extension.stop()
         # Call the father class
-        super(PluginModel, self).exit()
+        super().exit()
 
     def get_key(self):
         """Return the key of the list."""
         return 'name'
 
     def get_export(self):
         """Overwrite the default export method.
 
         - Only exports containers
         - The key is the first container name
         """
         try:
             ret = deepcopy(self.stats)
         except KeyError as e:
-            logger.debug("docker plugin - Docker export error {}".format(e))
+            logger.debug(f"docker plugin - Docker export error {e}")
             ret = []
 
         # Remove fields uses to compute rate
         for container in ret:
             for i in export_exclude_list:
                 container.pop(i)
 
@@ -205,16 +203,15 @@
         # By default, Glances only display running containers
         # Set the following key to True to display all containers
         all=True
         """
         all_tag = self.get_conf_value('all')
         if len(all_tag) == 0:
             return False
-        else:
-            return all_tag[0].lower() == 'true'
+        return all_tag[0].lower() == 'true'
 
     @GlancesPluginModel._check_decorator
     @GlancesPluginModel._log_result_decorator
     def update(self):
         """Update Docker and podman stats using the input method."""
         # Connection should be ok
         if self.docker_extension is None and self.podman_extension is None:
@@ -258,15 +255,15 @@
         """Return the 'real' memory usage by removing inactive_file to usage"""
         # Ref: https://github.com/docker/docker-py/issues/3210
         return mem['usage'] - (mem['inactive_file'] if 'inactive_file' in mem else 0)
 
     def update_views(self):
         """Update stats views."""
         # Call the father's method
-        super(PluginModel, self).update_views()
+        super().update_views()
 
         if not self.stats:
             return False
 
         # Add specifics information
         # Alert
         for i in self.stats:
@@ -298,15 +295,15 @@
 
         # Display Engine and Pod name ?
         show_pod_name = False
         if any(ct.get("pod_name") for ct in self.stats):
             show_pod_name = True
         self.views['show_pod_name'] = show_pod_name
         show_engine_name = False
-        if len(set(ct["engine"] for ct in self.stats)) > 1:
+        if len({ct["engine"] for ct in self.stats}) > 1:
             show_engine_name = True
         self.views['show_engine_name'] = show_engine_name
 
         return True
 
     def msg_curse(self, args=None, max_width=None):
         """Return the dict to display in the curse interface."""
@@ -317,17 +314,17 @@
         if not self.stats or len(self.stats) == 0 or self.is_disabled():
             return ret
 
         # Build the string message
         # Title
         msg = '{}'.format('CONTAINERS')
         ret.append(self.curse_add_line(msg, "TITLE"))
-        msg = ' {}'.format(len(self.stats))
+        msg = f' {len(self.stats)}'
         ret.append(self.curse_add_line(msg))
-        msg = ' sorted by {}'.format(sort_for_human[self.sort_key])
+        msg = f' sorted by {sort_for_human[self.sort_key]}'
         ret.append(self.curse_add_line(msg))
         ret.append(self.curse_new_line())
         # Header
         ret.append(self.curse_new_line())
         # Get the maximum containers name
         # Max size is configurable. See feature request #1723.
         name_max_width = min(
@@ -400,42 +397,42 @@
             except (KeyError, TypeError):
                 msg = '/{:<7}'.format('_')
             ret.append(self.curse_add_line(msg))
             # IO R/W
             unit = 'B'
             try:
                 value = self.auto_unit(int(container['io_rx'])) + unit
-                msg = '{:>7}'.format(value)
+                msg = f'{value:>7}'
             except (KeyError, TypeError):
                 msg = '{:>7}'.format('_')
             ret.append(self.curse_add_line(msg))
             try:
                 value = self.auto_unit(int(container['io_wx'])) + unit
-                msg = ' {:<7}'.format(value)
+                msg = f' {value:<7}'
             except (KeyError, TypeError):
                 msg = ' {:<7}'.format('_')
             ret.append(self.curse_add_line(msg))
             # NET RX/TX
             if args.byte:
                 # Bytes per second (for dummy)
                 to_bit = 1
                 unit = ''
             else:
                 # Bits per second (for real network administrator | Default)
                 to_bit = 8
                 unit = 'b'
             try:
                 value = self.auto_unit(int(container['network_rx'] * to_bit)) + unit
-                msg = '{:>7}'.format(value)
+                msg = f'{value:>7}'
             except (KeyError, TypeError):
                 msg = '{:>7}'.format('_')
             ret.append(self.curse_add_line(msg))
             try:
                 value = self.auto_unit(int(container['network_tx'] * to_bit)) + unit
-                msg = ' {:<7}'.format(value)
+                msg = f' {value:<7}'
             except (KeyError, TypeError):
                 msg = ' {:<7}'.format('_')
             ret.append(self.curse_add_line(msg))
             # Command
             if container['command'] is not None:
                 msg = ' {}'.format(container['command'])
             else:
@@ -449,20 +446,19 @@
         name = container['name'][:max_width]
         return ' {:{width}}'.format(name, width=max_width)
 
     def container_alert(self, status):
         """Analyse the container status."""
         if status == 'running':
             return 'OK'
-        elif status == 'exited':
+        if status == 'exited':
             return 'WARNING'
-        elif status == 'dead':
+        if status == 'dead':
             return 'CRITICAL'
-        else:
-            return 'CAREFUL'
+        return 'CAREFUL'
 
 
 def sort_docker_stats(stats):
     # Sort Docker stats using the same function than processes
     sort_by = glances_processes.sort_key
     sort_by_secondary = 'memory_usage'
     if sort_by == 'memory_percent':
```

### Comparing `glances-4.0.4/glances/plugins/containers/engines/docker.py` & `glances-4.0.5/glances/plugins/containers/engines/docker.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,33 +1,33 @@
-# -*- coding: utf-8 -*-
 #
 # This file is part of Glances.
 #
 # SPDX-FileCopyrightText: 2024 Nicolas Hennion <nicolas@nicolargo.com>
 #
 # SPDX-License-Identifier: LGPL-3.0-only
 #
 
 """Docker Extension unit for Glances' Containers plugin."""
+
 import time
 
 from glances.globals import iterkeys, itervalues, nativestr, pretty_date, replace_special_chars
 from glances.logger import logger
 from glances.plugins.containers.stats_streamer import StatsStreamer
 
 # Docker-py library (optional and Linux-only)
 # https://github.com/docker/docker-py
 try:
-    import requests
     import docker
+    import requests
     from dateutil import parser, tz
 except Exception as e:
     import_docker_error_tag = True
     # Display debug message if import KeyError
-    logger.warning("Error loading Docker deps Lib. Docker plugin is disabled ({})".format(e))
+    logger.warning(f"Error loading Docker deps Lib. Docker plugin is disabled ({e})")
 else:
     import_docker_error_tag = False
 
 
 class DockerStatsFetcher:
     MANDATORY_MEMORY_FIELDS = ['usage', 'limit']
 
@@ -42,15 +42,15 @@
         self._last_stats_computed_time = 0
 
         # Threaded Streamer
         stats_iterable = container.stats(decode=True)
         self._streamer = StatsStreamer(stats_iterable, initial_stream_value={})
 
     def _log_debug(self, msg, exception=None):
-        logger.debug("containers (Docker) ID: {} - {} ({}) ".format(self._container.id, msg, exception))
+        logger.debug(f"containers (Docker) ID: {self._container.id} - {msg} ({exception}) ")
         logger.debug(self._streamer.stats)
 
     def stop(self):
         self._streamer.stop()
 
     @property
     def activity_stats(self):
@@ -66,21 +66,20 @@
     def _compute_activity_stats(self):
         with self._streamer.result_lock:
             io_stats = self._get_io_stats()
             cpu_stats = self._get_cpu_stats()
             memory_stats = self._get_memory_stats()
             network_stats = self._get_network_stats()
 
-        computed_stats = {
+        return {
             "io": io_stats or {},
             "memory": memory_stats or {},
             "network": network_stats or {},
             "cpu": cpu_stats or {"total": 0.0},
         }
-        return computed_stats
 
     @property
     def time_since_update(self):
         # In case no update, default to 1
         return max(1, self._streamer.last_update_time - self._last_stats_computed_time)
 
     def _get_cpu_stats(self):
@@ -225,15 +224,15 @@
     def connect(self):
         """Connect to the Docker server."""
         # Init the Docker API Client
         try:
             # Do not use the timeout option (see issue #1878)
             self.client = docker.from_env()
         except Exception as e:
-            logger.error("{} plugin - Can't connect to Docker ({})".format(self.ext_name, e))
+            logger.error(f"{self.ext_name} plugin - Can't connect to Docker ({e})")
             self.client = None
 
     def update_version(self):
         # Long and not useful anymore because the information is no more displayed in UIs
         # return self.client.version()
         return {}
 
@@ -252,30 +251,30 @@
 
         # Update current containers list
         try:
             # Issue #1152: Docker module doesn't export details about stopped containers
             # The Containers/all key of the configuration file should be set to True
             containers = self.client.containers.list(all=all_tag)
         except Exception as e:
-            logger.error("{} plugin - Can't get containers list ({})".format(self.ext_name, e))
+            logger.error(f"{self.ext_name} plugin - Can't get containers list ({e})")
             return version_stats, []
 
         # Start new thread for new container
         for container in containers:
             if container.id not in self.stats_fetchers:
                 # StatsFetcher did not exist in the internal dict
                 # Create it, add it to the internal dict
-                logger.debug("{} plugin - Create thread for container {}".format(self.ext_name, container.id[:12]))
+                logger.debug(f"{self.ext_name} plugin - Create thread for container {container.id[:12]}")
                 self.stats_fetchers[container.id] = DockerStatsFetcher(container)
 
         # Stop threads for non-existing containers
-        absent_containers = set(iterkeys(self.stats_fetchers)) - set(c.id for c in containers)
+        absent_containers = set(iterkeys(self.stats_fetchers)) - {c.id for c in containers}
         for container_id in absent_containers:
             # Stop the StatsFetcher
-            logger.debug("{} plugin - Stop thread for old container {}".format(self.ext_name, container_id[:12]))
+            logger.debug(f"{self.ext_name} plugin - Stop thread for old container {container_id[:12]}")
             self.stats_fetchers[container_id].stop()
             # Delete the StatsFetcher from the dict
             del self.stats_fetchers[container_id]
 
         # Get stats for all containers
         container_stats = [self.generate_stats(container) for container in containers]
         return version_stats, container_stats
```

### Comparing `glances-4.0.4/glances/plugins/containers/engines/podman.py` & `glances-4.0.5/glances/plugins/containers/engines/podman.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,30 +1,30 @@
-# -*- coding: utf-8 -*-
 #
 # This file is part of Glances.
 #
 # SPDX-FileCopyrightText: 2022 Nicolas Hennion <nicolas@nicolargo.com>
 #
 # SPDX-License-Identifier: LGPL-3.0-only
 
 """Podman Extension unit for Glances' Containers plugin."""
+
 from datetime import datetime
 
-from glances.globals import iterkeys, itervalues, nativestr, pretty_date, string_value_to_float, replace_special_chars
+from glances.globals import iterkeys, itervalues, nativestr, pretty_date, replace_special_chars, string_value_to_float
 from glances.logger import logger
 from glances.plugins.containers.stats_streamer import StatsStreamer
 
 # Podman library (optional and Linux-only)
 # https://pypi.org/project/podman/
 try:
     from podman import PodmanClient
 except Exception as e:
     import_podman_error_tag = True
     # Display debug message if import KeyError
-    logger.warning("Error loading Podman deps Lib. Podman feature in the Containers plugin is disabled ({})".format(e))
+    logger.warning(f"Error loading Podman deps Lib. Podman feature in the Containers plugin is disabled ({e})")
 else:
     import_podman_error_tag = False
 
 
 class PodmanContainerStatsFetcher:
     MANDATORY_FIELDS = ["CPU", "MemUsage", "MemLimit", "NetInput", "NetOutput", "BlockInput", "BlockOutput"]
 
@@ -32,15 +32,15 @@
         self._container = container
 
         # Threaded Streamer
         stats_iterable = container.stats(decode=True)
         self._streamer = StatsStreamer(stats_iterable, initial_stream_value={})
 
     def _log_debug(self, msg, exception=None):
-        logger.debug("containers (Podman) ID: {} - {} ({})".format(self._container.id, msg, exception))
+        logger.debug(f"containers (Podman) ID: {self._container.id} - {msg} ({exception})")
         logger.debug(self._streamer.stats)
 
     def stop(self):
         self._streamer.stop()
 
     @property
     def stats(self):
@@ -91,15 +91,15 @@
 
         # Threaded Streamer
         # Temporary patch to get podman extension working
         stats_iterable = (pod_manager.stats(decode=True) for _ in iter(int, 1))
         self._streamer = StatsStreamer(stats_iterable, initial_stream_value={}, sleep_duration=2)
 
     def _log_debug(self, msg, exception=None):
-        logger.debug("containers (Podman): Pod Manager - {} ({})".format(msg, exception))
+        logger.debug(f"containers (Podman): Pod Manager - {msg} ({exception})")
         logger.debug(self._streamer.stats)
 
     def stop(self):
         self._streamer.stop()
 
     @property
     def activity_stats(self):
@@ -230,15 +230,15 @@
     def connect(self):
         """Connect to Podman."""
         try:
             self.client = PodmanClient(base_url=self.podman_sock)
             # PodmanClient works lazily, so make a ping to determine if socket is open
             self.client.ping()
         except Exception as e:
-            logger.debug("{} plugin - Can't connect to Podman ({})".format(self.ext_name, e))
+            logger.debug(f"{self.ext_name} plugin - Can't connect to Podman ({e})")
             self.client = None
 
     def update_version(self):
         # Long and not useful anymore because the information is no more displayed in UIs
         # return self.client.version()
         return {}
 
@@ -262,30 +262,30 @@
         try:
             # Issue #1152: Podman module doesn't export details about stopped containers
             # The Containers/all key of the configuration file should be set to True
             containers = self.client.containers.list(all=all_tag)
             if not self.pods_stats_fetcher:
                 self.pods_stats_fetcher = PodmanPodStatsFetcher(self.client.pods)
         except Exception as e:
-            logger.error("{} plugin - Can't get containers list ({})".format(self.ext_name, e))
+            logger.error(f"{self.ext_name} plugin - Can't get containers list ({e})")
             return version_stats, []
 
         # Start new thread for new container
         for container in containers:
             if container.id not in self.container_stats_fetchers:
                 # StatsFetcher did not exist in the internal dict
                 # Create it, add it to the internal dict
-                logger.debug("{} plugin - Create thread for container {}".format(self.ext_name, container.id[:12]))
+                logger.debug(f"{self.ext_name} plugin - Create thread for container {container.id[:12]}")
                 self.container_stats_fetchers[container.id] = PodmanContainerStatsFetcher(container)
 
         # Stop threads for non-existing containers
-        absent_containers = set(iterkeys(self.container_stats_fetchers)) - set(c.id for c in containers)
+        absent_containers = set(iterkeys(self.container_stats_fetchers)) - {c.id for c in containers}
         for container_id in absent_containers:
             # Stop the StatsFetcher
-            logger.debug("{} plugin - Stop thread for old container {}".format(self.ext_name, container_id[:12]))
+            logger.debug(f"{self.ext_name} plugin - Stop thread for old container {container_id[:12]}")
             self.container_stats_fetchers[container_id].stop()
             # Delete the StatsFetcher from the dict
             del self.container_stats_fetchers[container_id]
 
         # Get stats for all containers
         container_stats = [self.generate_stats(container) for container in containers]
```

### Comparing `glances-4.0.4/glances/plugins/containers/stats_streamer.py` & `glances-4.0.5/glances/plugins/containers/stats_streamer.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 #
 # This file is part of Glances.
 #
 # SPDX-FileCopyrightText: 2022 Nicolas Hennion <nicolas@nicolargo.com>
 #
 # SPDX-License-Identifier: LGPL-3.0-only
 
@@ -59,15 +58,15 @@
                 self._post_update_hook()
 
                 time.sleep(self._sleep_duration)
                 if self.stopped():
                     break
 
         except Exception as e:
-            logger.debug("docker plugin - Exception thrown during run ({})".format(e))
+            logger.debug(f"docker plugin - Exception thrown during run ({e})")
             self.stop()
 
     def _pre_update_hook(self):
         """Hook that runs before worker thread updates the raw_stats"""
         self.result_lock.acquire()
 
     def _post_update_hook(self):
```

### Comparing `glances-4.0.4/glances/plugins/core/__init__.py` & `glances-4.0.5/glances/plugins/core/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,22 +1,21 @@
-# -*- coding: utf-8 -*-
 #
 # This file is part of Glances.
 #
 # SPDX-FileCopyrightText: 2022 Nicolas Hennion <nicolas@nicolargo.com>
 #
 # SPDX-License-Identifier: LGPL-3.0-only
 #
 
 """CPU core plugin."""
 
-from glances.plugins.plugin.model import GlancesPluginModel
-
 import psutil
 
+from glances.plugins.plugin.model import GlancesPluginModel
+
 # Fields description
 fields_description = {
     'phys': {'description': 'Number of physical cores (hyper thread CPUs are excluded).', 'unit': 'number'},
     'log': {
         'description': 'Number of logical CPU cores. A logical CPU is the number of \
 physical cores multiplied by the number of threads that can run on each core.',
         'unit': 'number',
@@ -30,15 +29,15 @@
     Get stats about CPU core number.
 
     stats is integer (number of core)
     """
 
     def __init__(self, args=None, config=None):
         """Init the plugin."""
-        super(PluginModel, self).__init__(args=args, config=config, fields_description=fields_description)
+        super().__init__(args=args, config=config, fields_description=fields_description)
 
         # We dot not want to display the stat in the curse interface
         # The core number is displayed by the load plugin
         self.display_curse = False
 
     # Do *NOT* uncomment the following line
     # @GlancesPluginModel._check_decorator
```

### Comparing `glances-4.0.4/glances/plugins/cpu/__init__.py` & `glances-4.0.5/glances/plugins/cpu/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,24 @@
-# -*- coding: utf-8 -*-
 #
 # This file is part of Glances.
 #
 # SPDX-FileCopyrightText: 2022 Nicolas Hennion <nicolas@nicolargo.com>
 #
 # SPDX-License-Identifier: LGPL-3.0-only
 #
 
 """CPU plugin."""
 
-from glances.globals import LINUX, WINDOWS, SUNOS, iterkeys
+import psutil
+
 from glances.cpu_percent import cpu_percent
+from glances.globals import LINUX, SUNOS, WINDOWS, iterkeys
 from glances.plugins.core import PluginModel as CorePluginModel
 from glances.plugins.plugin.model import GlancesPluginModel
 
-import psutil
-
 # Fields description
 # description: human readable description
 # short_name: shortname to use un UI
 # unit: unit type
 # rate: if True then compute and add *_gauge and *_rate_per_is fields
 # min_symbol: Auto unit should be used if value > than 1 'X' (K, M, G)...
 fields_description = {
@@ -140,15 +139,15 @@
 
     'stats' is a dictionary that contains the system-wide CPU utilization as a
     percentage.
     """
 
     def __init__(self, args=None, config=None):
         """Init the CPU plugin."""
-        super(PluginModel, self).__init__(
+        super().__init__(
             args=args, config=config, items_history_list=items_history_list, fields_description=fields_description
         )
 
         # We want to display the stat in the curse interface
         self.display_curse = True
 
         # Call CorePluginModel in order to display the core number
@@ -269,15 +268,15 @@
             stats['total'] = 100 - stats['idle']
 
         return stats
 
     def update_views(self):
         """Update stats views."""
         # Call the father's method
-        super(PluginModel, self).update_views()
+        super().update_views()
 
         # Add specifics information
         # Alert and log
         for key in ['user', 'system', 'iowait', 'dpc', 'total']:
             if key in self.stats:
                 self.views[key]['decoration'] = self.get_alert_log(self.stats[key], header=key)
         # Alert only
```

### Comparing `glances-4.0.4/glances/plugins/diskio/__init__.py` & `glances-4.0.5/glances/plugins/diskio/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,25 +1,23 @@
-# -*- coding: utf-8 -*-
 #
 # This file is part of Glances.
 #
 # SPDX-FileCopyrightText: 2024 Nicolas Hennion <nicolas@nicolargo.com>
 #
 # SPDX-License-Identifier: LGPL-3.0-only
 #
 
 """Disk I/O plugin."""
-from __future__ import unicode_literals
 
-from glances.logger import logger
+import psutil
+
 from glances.globals import nativestr
+from glances.logger import logger
 from glances.plugins.plugin.model import GlancesPluginModel
 
-import psutil
-
 # Fields description
 # description: human readable description
 # short_name: shortname to use un UI
 # unit: unit type
 # rate: if True then compute and add *_gauge and *_rate_per_is fields
 # min_symbol: Auto unit should be used if value > than 1 'X' (K, M, G)...
 fields_description = {
@@ -57,15 +55,15 @@
     """Glances disks I/O plugin.
 
     stats is a list
     """
 
     def __init__(self, args=None, config=None):
         """Init the plugin."""
-        super(PluginModel, self).__init__(
+        super().__init__(
             args=args,
             config=config,
             items_history_list=items_history_list,
             stats_init_value=[],
             fields_description=fields_description,
         )
 
@@ -137,15 +135,15 @@
             stats.append(stat)
 
         return stats
 
     def update_views(self):
         """Update stats views."""
         # Call the father's method
-        super(PluginModel, self).update_views()
+        super().update_views()
 
         # Check if the stats should be hidden
         self.update_views_hidden()
 
         # Add specifics information
         # Alert
         for i in self.get_raw():
@@ -167,15 +165,15 @@
             return ret
 
         # Max size for the interface name
         if max_width:
             name_max_width = max_width - 13
         else:
             # No max_width defined, return an emptu curse message
-            logger.debug("No max_width defined for the {} plugin, it will not be displayed.".format(self.plugin_name))
+            logger.debug(f"No max_width defined for the {self.plugin_name} plugin, it will not be displayed.")
             return ret
 
         # Header
         msg = '{:{width}}'.format('DISK I/O', width=name_max_width)
         ret.append(self.curse_add_line(msg, "TITLE"))
         if args.diskio_iops:
             msg = '{:>8}'.format('IOR/s')
@@ -186,52 +184,52 @@
             msg = '{:>8}'.format('R/s')
             ret.append(self.curse_add_line(msg))
             msg = '{:>7}'.format('W/s')
             ret.append(self.curse_add_line(msg))
         # Disk list (sorted by name)
         for i in self.sorted_stats():
             # Hide stats if never be different from 0 (issue #1787)
-            if all([self.get_views(item=i[self.get_key()], key=f, option='hidden') for f in self.hide_zero_fields]):
+            if all(self.get_views(item=i[self.get_key()], key=f, option='hidden') for f in self.hide_zero_fields):
                 continue
             # Is there an alias for the disk name ?
             disk_name = i['alias'] if 'alias' in i else i['disk_name']
             # New line
             ret.append(self.curse_new_line())
             if len(disk_name) > name_max_width:
                 # Cut disk name if it is too long
                 disk_name = disk_name[:name_max_width] + '_'
             msg = '{:{width}}'.format(nativestr(disk_name), width=name_max_width + 1)
             ret.append(self.curse_add_line(msg))
             if args.diskio_iops:
                 # count
                 txps = self.auto_unit(i.get('read_count_rate_per_sec', None))
                 rxps = self.auto_unit(i.get('write_count_rate_per_sec', None))
-                msg = '{:>7}'.format(txps)
+                msg = f'{txps:>7}'
                 ret.append(
                     self.curse_add_line(
                         msg, self.get_views(item=i[self.get_key()], key='read_count', option='decoration')
                     )
                 )
-                msg = '{:>7}'.format(rxps)
+                msg = f'{rxps:>7}'
                 ret.append(
                     self.curse_add_line(
                         msg, self.get_views(item=i[self.get_key()], key='write_count', option='decoration')
                     )
                 )
             else:
                 # Bitrate
                 txps = self.auto_unit(i.get('read_bytes_rate_per_sec', None))
                 rxps = self.auto_unit(i.get('write_bytes_rate_per_sec', None))
-                msg = '{:>7}'.format(txps)
+                msg = f'{txps:>7}'
                 ret.append(
                     self.curse_add_line(
                         msg, self.get_views(item=i[self.get_key()], key='read_bytes', option='decoration')
                     )
                 )
-                msg = '{:>7}'.format(rxps)
+                msg = f'{rxps:>7}'
                 ret.append(
                     self.curse_add_line(
                         msg, self.get_views(item=i[self.get_key()], key='write_bytes', option='decoration')
                     )
                 )
 
         return ret
```

### Comparing `glances-4.0.4/glances/plugins/folders/__init__.py` & `glances-4.0.5/glances/plugins/folders/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,22 @@
-# -*- coding: utf-8 -*-
 #
 # This file is part of Glances.
 #
 # SPDX-FileCopyrightText: 2022 Nicolas Hennion <nicolas@nicolargo.com>
 #
 # SPDX-License-Identifier: LGPL-3.0-only
 #
 
 """Folder plugin."""
-from __future__ import unicode_literals
 
-from glances.logger import logger
-from glances.globals import nativestr
 from glances.folder_list import FolderList as glancesFolderList
+from glances.globals import nativestr
+from glances.logger import logger
 from glances.plugins.plugin.model import GlancesPluginModel
 
-
 # Fields description
 # description: human readable description
 # short_name: shortname to use un UI
 # unit: unit type
 # rate: is it a rate ? If yes, // by time_since_update when displayed,
 # min_symbol: Auto unit should be used if value > than 1 'X' (K, M, G)...
 fields_description = {
@@ -52,17 +49,15 @@
 
 
 class PluginModel(GlancesPluginModel):
     """Glances folder plugin."""
 
     def __init__(self, args=None, config=None):
         """Init the plugin."""
-        super(PluginModel, self).__init__(
-            args=args, config=config, stats_init_value=[], fields_description=fields_description
-        )
+        super().__init__(args=args, config=config, stats_init_value=[], fields_description=fields_description)
 
         self.args = args
         self.config = config
 
         # We want to display the stat in the curse interface
         self.display_curse = True
 
@@ -134,15 +129,15 @@
             return ret
 
         # Max size for the interface name
         if max_width:
             name_max_width = max_width - 7
         else:
             # No max_width defined, return an emptu curse message
-            logger.debug("No max_width defined for the {} plugin, it will not be displayed.".format(self.plugin_name))
+            logger.debug(f"No max_width defined for the {self.plugin_name} plugin, it will not be displayed.")
             return ret
 
         # Header
         msg = '{:{width}}'.format('FOLDERS', width=name_max_width)
         ret.append(self.curse_add_line(msg, "TITLE"))
 
         # Data
```

### Comparing `glances-4.0.4/glances/plugins/fs/__init__.py` & `glances-4.0.5/glances/plugins/fs/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,25 @@
-# -*- coding: utf-8 -*-
 #
 # This file is part of Glances.
 #
 # SPDX-FileCopyrightText: 2024 Nicolas Hennion <nicolas@nicolargo.com>
 #
 # SPDX-License-Identifier: LGPL-3.0-only
 #
 
 """File system plugin."""
-from __future__ import unicode_literals
 
 import operator
 
-from glances.globals import u, nativestr, PermissionError
+import psutil
+
+from glances.globals import PermissionError, nativestr, u
 from glances.logger import logger
 from glances.plugins.plugin.model import GlancesPluginModel
 
-import psutil
-
 # Fields description
 # description: human readable description
 # short_name: shortname to use un UI
 # unit: unit type
 # rate: is it a rate ? If yes, // by time_since_update when displayed,
 # min_symbol: Auto unit should be used if value > than 1 'X' (K, M, G)...
 fields_description = {
@@ -93,15 +91,15 @@
     """Glances file system plugin.
 
     stats is a list
     """
 
     def __init__(self, args=None, config=None):
         """Init the plugin."""
-        super(PluginModel, self).__init__(
+        super().__init__(
             args=args,
             config=config,
             items_history_list=items_history_list,
             stats_init_value=[],
             fields_description=fields_description,
         )
 
@@ -137,15 +135,15 @@
                 # Avoid Psutil call unless mounts need to be allowed
                 try:
                     all_mounted_fs = psutil.disk_partitions(all=True)
                 except (UnicodeDecodeError, PermissionError):
                     logger.debug("Plugin - fs: PsUtil extended fetch failed")
                 else:
                     # Discard duplicates (#2299) and add entries matching allowed fs types
-                    tracked_mnt_points = set(f.mountpoint for f in fs_stat)
+                    tracked_mnt_points = {f.mountpoint for f in fs_stat}
                     for f in all_mounted_fs:
                         if (
                             any(f.fstype.find(fs_type) >= 0 for fs_type in allowed_fs_types)
                             and f.mountpoint not in tracked_mnt_points
                         ):
                             fs_stat.append(f)
 
@@ -162,15 +160,15 @@
                     # Correct issue #346
                     # Disk is ejected during the command
                     continue
                 fs_current = {
                     'device_name': fs.device,
                     'fs_type': fs.fstype,
                     # Manage non breaking space (see issue #1065)
-                    'mnt_point': u(fs.mountpoint).replace(u'\u00A0', ' '),
+                    'mnt_point': u(fs.mountpoint).replace('\u00a0', ' '),
                     'size': fs_usage.total,
                     'used': fs_usage.used,
                     'free': fs_usage.free,
                     'percent': fs_usage.percent,
                     'key': self.get_key(),
                 }
 
@@ -211,42 +209,40 @@
                         'used': used,
                         'percent': percent,
                         'key': self.get_key(),
                     }
                     # Do not take hidden file system into account
                     if self.is_hide(fs_current['mnt_point']):
                         continue
-                    else:
-                        stats.append(fs_current)
+                    stats.append(fs_current)
             else:
                 # Default behavior
                 for fs in fs_stat:
                     fs_current = {
                         'device_name': fs_stat[fs]['device_name'],
                         'mnt_point': fs,
                         'size': int(fs_stat[fs]['size']) * 1024,
                         'used': int(fs_stat[fs]['used']) * 1024,
                         'percent': float(fs_stat[fs]['percent']),
                         'key': self.get_key(),
                     }
                     # Do not take hidden file system into account
                     if self.is_hide(fs_current['mnt_point']) or self.is_hide(fs_current['device_name']):
                         continue
-                    else:
-                        stats.append(fs_current)
+                    stats.append(fs_current)
 
         # Update the stats
         self.stats = stats
 
         return self.stats
 
     def update_views(self):
         """Update stats views."""
         # Call the father's method
-        super(PluginModel, self).update_views()
+        super().update_views()
 
         # Add specifics information
         # Alert
         for i in self.stats:
             self.views[i[self.get_key()]]['used']['decoration'] = self.get_alert(
                 current=i['size'] - i['free'], maximum=i['size'], header=i['mnt_point']
             )
@@ -261,15 +257,15 @@
             return ret
 
         # Max size for the interface name
         if max_width:
             name_max_width = max_width - 13
         else:
             # No max_width defined, return an emptu curse message
-            logger.debug("No max_width defined for the {} plugin, it will not be displayed.".format(self.plugin_name))
+            logger.debug(f"No max_width defined for the {self.plugin_name} plugin, it will not be displayed.")
             return ret
 
         # Build the string message
         # Header
         msg = '{:{width}}'.format('FILE SYS', width=name_max_width)
         ret.append(self.curse_add_line(msg, "TITLE"))
         if args.fs_free_space:
```

### Comparing `glances-4.0.4/glances/plugins/gpu/__init__.py` & `glances-4.0.5/glances/plugins/gpu/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 #
 # This file is part of Glances.
 #
 # Copyright (C) 2020 Kirby Banman <kirby.banman@gmail.com>
 # Copyright (C) 2024 Nicolas Hennion <nicolashennion@gmail.com>
 #
 # SPDX-License-Identifier: LGPL-3.0-only
@@ -12,16 +11,16 @@
 
 Currently supported:
 - NVIDIA GPU (need pynvml lib)
 - AMD GPU (no lib needed)
 """
 
 from glances.globals import to_fahrenheit
-from glances.plugins.gpu.cards.nvidia import NvidiaGPU
 from glances.plugins.gpu.cards.amd import AmdGPU
+from glances.plugins.gpu.cards.nvidia import NvidiaGPU
 from glances.plugins.plugin.model import GlancesPluginModel
 
 # Fields description
 # description: human readable description
 # short_name: shortname to use un UI
 # unit: unit type
 # rate: is it a rate ? If yes, // by time_since_update when displayed,
@@ -63,15 +62,15 @@
     """Glances GPU plugin.
 
     stats is a list of dictionaries with one entry per GPU
     """
 
     def __init__(self, args=None, config=None):
         """Init the plugin."""
-        super(PluginModel, self).__init__(
+        super().__init__(
             args=args,
             config=config,
             items_history_list=items_history_list,
             stats_init_value=[],
             fields_description=fields_description,
         )
         # Init the GPU API
@@ -85,15 +84,15 @@
 
     def exit(self):
         """Overwrite the exit method to close the GPU API."""
         self.nvidia.exit()
         self.amd.exit()
 
         # Call the father exit method
-        super(PluginModel, self).exit()
+        super().exit()
 
     def get_key(self):
         """Return the key of the list."""
         return 'gpu_id'
 
     @GlancesPluginModel._check_decorator
     @GlancesPluginModel._log_result_decorator
@@ -146,15 +145,15 @@
         self.stats = stats
 
         return self.stats
 
     def update_views(self):
         """Update stats views."""
         # Call the father's method
-        super(PluginModel, self).update_views()
+        super().update_views()
 
         # Add specifics information
         # Alert
         for i in self.stats:
             # Init the views for the current GPU
             self.views[i[self.get_key()]] = {'proc': {}, 'mem': {}, 'temperature': {}}
             # Processor alert
@@ -186,15 +185,15 @@
 
         # gpu_stats contain the first GPU in the list
         gpu_stats = self.stats[0]
 
         # Header
         header = ''
         if len(self.stats) > 1:
-            header += '{}'.format(len(self.stats))
+            header += f'{len(self.stats)}'
             if same_name:
                 header += ' {}'.format(gpu_stats['name'])
             else:
                 header += ' GPUs'
         elif same_name:
             header += '{}'.format(gpu_stats['name'])
         else:
@@ -209,15 +208,15 @@
             ret.append(self.curse_new_line())
             # GPU PROC
             try:
                 mean_proc = sum(s['proc'] for s in self.stats if s is not None) / len(self.stats)
             except TypeError:
                 mean_proc_msg = '{:>4}'.format('N/A')
             else:
-                mean_proc_msg = '{:>3.0f}%'.format(mean_proc)
+                mean_proc_msg = f'{mean_proc:>3.0f}%'
             if len(self.stats) > 1:
                 msg = '{:13}'.format('proc mean:')
             else:
                 msg = '{:13}'.format('proc:')
             ret.append(self.curse_add_line(msg))
             ret.append(
                 self.curse_add_line(
@@ -228,15 +227,15 @@
             ret.append(self.curse_new_line())
             # GPU MEM
             try:
                 mean_mem = sum(s['mem'] for s in self.stats if s is not None) / len(self.stats)
             except TypeError:
                 mean_mem_msg = '{:>4}'.format('N/A')
             else:
-                mean_mem_msg = '{:>3.0f}%'.format(mean_mem)
+                mean_mem_msg = f'{mean_mem:>3.0f}%'
             if len(self.stats) > 1:
                 msg = '{:13}'.format('mem mean:')
             else:
                 msg = '{:13}'.format('mem:')
             ret.append(self.curse_add_line(msg))
             ret.append(
                 self.curse_add_line(
@@ -251,15 +250,15 @@
             except TypeError:
                 mean_temperature_msg = '{:>4}'.format('N/A')
             else:
                 unit = 'C'
                 if args.fahrenheit:
                     mean_temperature = to_fahrenheit(mean_temperature)
                     unit = 'F'
-                mean_temperature_msg = '{:>3.0f}{}'.format(mean_temperature, unit)
+                mean_temperature_msg = f'{mean_temperature:>3.0f}{unit}'
             if len(self.stats) > 1:
                 msg = '{:13}'.format('temp mean:')
             else:
                 msg = '{:13}'.format('temperature:')
             ret.append(self.curse_add_line(msg))
             ret.append(
                 self.curse_add_line(
@@ -279,11 +278,11 @@
                     proc_msg = '{:>3.0f}%'.format(gpu_stats['proc'])
                 except (ValueError, TypeError):
                     proc_msg = '{:>4}'.format('N/A')
                 try:
                     mem_msg = '{:>3.0f}%'.format(gpu_stats['mem'])
                 except (ValueError, TypeError):
                     mem_msg = '{:>4}'.format('N/A')
-                msg = '{} {} mem {}'.format(id_msg, proc_msg, mem_msg)
+                msg = f'{id_msg} {proc_msg} mem {mem_msg}'
                 ret.append(self.curse_add_line(msg))
 
         return ret
```

### Comparing `glances-4.0.4/glances/plugins/gpu/cards/amd.py` & `glances-4.0.5/glances/plugins/gpu/cards/amd.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 #
 # This file is part of Glances.
 #
 # SPDX-FileCopyrightText: 2024 Nicolas Hennion <nicolas@nicolargo.com>
 #
 # SPDX-License-Identifier: LGPL-3.0-only
 #
@@ -31,16 +30,17 @@
 #     │               └── pp_dpm_sclk
 #     └── kernel
 #         └── debug
 #             └── dri
 #                 └── 0
 #                     └── amdgpu_pm_info
 
-import re
 import os
+import re
+from typing import Optional
 
 DRM_ROOT_FOLDER: str = '/sys/class/drm'
 CARD_REGEX: str = r"^card\d$"
 DEVICE_FOLDER: str = 'device'
 GPU_PROC_PERCENT: str = 'gpu_busy_percent'
 GPU_MEM_TOTAL: str = 'mem_info_vram_total'
 GPU_MEM_USED: str = 'mem_info_vram_used'
@@ -60,15 +60,15 @@
         """Close AMD GPU class."""
 
     def get_device_stats(self):
         """Get AMD GPU stats."""
         stats = []
 
         for index, device in enumerate(self.device_folders):
-            device_stats = dict()
+            device_stats = {}
             # Dictionary key is the GPU_ID
             device_stats['key'] = 'gpu_id'
             # GPU id (for multiple GPU, start at 0)
             device_stats['gpu_id'] = f'amd{index}'
             # GPU name
             device_stats['name'] = get_device_name(device)
             # Memory consumption in % (not available on all GPU)
@@ -100,50 +100,49 @@
 
 
 def get_device_name(device_folder: str) -> str:
     """Return the GPU name."""
     return 'AMD GPU'
 
 
-def get_mem(device_folder: str) -> int:
+def get_mem(device_folder: str) -> Optional[int]:
     """Return the memory consumption in %."""
     mem_info_vram_total = os.path.join(device_folder, GPU_MEM_TOTAL)
     mem_info_vram_used = os.path.join(device_folder, GPU_MEM_USED)
     if os.path.isfile(mem_info_vram_total) and os.path.isfile(mem_info_vram_used):
         with open(mem_info_vram_total) as f:
             mem_info_vram_total = int(f.read())
         with open(mem_info_vram_used) as f:
             mem_info_vram_used = int(f.read())
         if mem_info_vram_total > 0:
             return round(mem_info_vram_used / mem_info_vram_total * 100)
     return None
 
 
-def get_proc(device_folder: str) -> int:
+def get_proc(device_folder: str) -> Optional[int]:
     """Return the processor consumption in %."""
     gpu_busy_percent = os.path.join(device_folder, GPU_PROC_PERCENT)
     if os.path.isfile(gpu_busy_percent):
         with open(gpu_busy_percent) as f:
             return int(f.read())
     return None
 
 
-def get_temperature(device_folder: str) -> int:
+def get_temperature(device_folder: str) -> Optional[int]:
     """Return the processor temperature in °C (mean of all HWMON)"""
     temp_input = []
     for root, dirs, _ in os.walk(device_folder):
         for d in dirs:
             if re.match(HWMON_REGEXP, d):
                 for _, _, files in os.walk(os.path.join(root, d)):
                     for f in files:
                         if re.match(GPU_TEMPERATURE_REGEXP, f):
                             with open(os.path.join(root, d, f)) as f:
                                 temp_input.append(int(f.read()))
     if len(temp_input) > 0:
         return round(sum(temp_input) / len(temp_input) / 1000)
-    else:
-        return None
+    return None
 
 
-def get_fan_speed(device_folder: str) -> int:
+def get_fan_speed(device_folder: str) -> Optional[int]:
     """Return the fan speed in %."""
     return None
```

### Comparing `glances-4.0.4/glances/plugins/gpu/cards/nvidia.py` & `glances-4.0.5/glances/plugins/gpu/cards/nvidia.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,27 +1,26 @@
-# -*- coding: utf-8 -*-
 #
 # This file is part of Glances.
 #
 # SPDX-FileCopyrightText: 2024 Nicolas Hennion <nicolas@nicolargo.com>
 #
 # SPDX-License-Identifier: LGPL-3.0-only
 #
 
 """NVidia Extension unit for Glances' GPU plugin."""
 
-from glances.logger import logger
 from glances.globals import nativestr
+from glances.logger import logger
 
 try:
     import pynvml
 except Exception as e:
     nvidia_gpu_enable = False
     # Display debug message if import KeyError
-    logger.warning("Missing Python Lib ({}), Nvidia GPU plugin is disabled".format(e))
+    logger.warning(f"Missing Python Lib ({e}), Nvidia GPU plugin is disabled")
 else:
     nvidia_gpu_enable = True
 
 
 class NvidiaGPU:
     """GPU card class."""
 
@@ -39,22 +38,22 @@
 
     def exit(self):
         """Close NVidia GPU class."""
         if self.device_handles != []:
             try:
                 pynvml.nvmlShutdown()
             except Exception as e:
-                logger.debug("pynvml failed to shutdown correctly ({})".format(e))
+                logger.debug(f"pynvml failed to shutdown correctly ({e})")
 
     def get_device_stats(self):
         """Get Nvidia GPU stats."""
         stats = []
 
         for index, device_handle in enumerate(self.device_handles):
-            device_stats = dict()
+            device_stats = {}
             # Dictionary key is the GPU_ID
             device_stats['key'] = 'gpu_id'
             # GPU id (for multiple GPU, start at 0)
             device_stats['gpu_id'] = f'nvidia{index}'
             # GPU name
             device_stats['name'] = get_device_name(device_handle)
             # Memory consumption in % (not available on all GPU)
```

### Comparing `glances-4.0.4/glances/plugins/help/__init__.py` & `glances-4.0.5/glances/plugins/help/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,64 +1,59 @@
-# -*- coding: utf-8 -*-
 #
 # This file is part of Glances.
 #
 # SPDX-FileCopyrightText: 2022 Nicolas Hennion <nicolas@nicolargo.com>
 #
 # SPDX-License-Identifier: LGPL-3.0-only
 #
 
 """
 Help plugin.
 
 Just a stupid plugin to display the help screen.
 """
-import sys
-from glances.globals import iteritems
+
+from itertools import chain
+
 from glances import __version__, psutil_version
+from glances.globals import iteritems
 from glances.plugins.plugin.model import GlancesPluginModel
-from itertools import chain
 
 
 class PluginModel(GlancesPluginModel):
     """Glances help plugin."""
 
     def __init__(self, args=None, config=None):
         """Init the plugin."""
-        super(PluginModel, self).__init__(args=args, config=config)
+        super().__init__(args=args, config=config)
 
         # Set the config instance
         self.config = config
         self.args = args
 
         # We want to display the stat in the curse interface
         self.display_curse = True
 
         # init data dictionary, to preserve insertion order
-        if sys.version_info < (3, 6):
-            from collections import OrderedDict
-
-            self.view_data = OrderedDict()
-        else:
-            self.view_data = {}
+        self.view_data = {}
         self.generate_view_data()
 
     def reset(self):
         """No stats. It is just a plugin to display the help."""
 
     def update(self):
         """No stats. It is just a plugin to display the help."""
 
     def generate_view_data(self):
         """Generate the views."""
         self.view_data['version'] = '{} {}'.format('Glances', __version__)
-        self.view_data['psutil_version'] = ' with psutil {}'.format(psutil_version)
+        self.view_data['psutil_version'] = f' with psutil {psutil_version}'
 
         try:
-            self.view_data['configuration_file'] = 'Configuration file: {}'.format(self.config.loaded_config_file)
+            self.view_data['configuration_file'] = f'Configuration file: {self.config.loaded_config_file}'
         except AttributeError:
             pass
 
         msg_col = '  {0:1}  {1:34}'
         msg_header = '{0:39}'
 
         self.view_data.update(
```

### Comparing `glances-4.0.4/glances/plugins/ip/__init__.py` & `glances-4.0.5/glances/plugins/ip/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,33 +1,32 @@
-# -*- coding: utf-8 -*-
 #
 # This file is part of Glances.
 #
 # SPDX-FileCopyrightText: 2024 Nicolas Hennion <nicolas@nicolargo.com>
 #
 # SPDX-License-Identifier: LGPL-3.0-only
 #
 
 """IP plugin."""
 
 import threading
+
 from ujson import loads
 
 from glances.globals import queue, urlopen_auth
 from glances.logger import logger
-from glances.timer import Timer
-from glances.timer import getTimeSinceLastUpdate
 from glances.plugins.plugin.model import GlancesPluginModel
+from glances.timer import Timer, getTimeSinceLastUpdate
 
 # Import plugin specific dependency
 try:
     import netifaces
 except ImportError as e:
     import_error_tag = True
-    logger.warning("Missing Python Lib ({}), IP plugin is disabled".format(e))
+    logger.warning(f"Missing Python Lib ({e}), IP plugin is disabled")
 else:
     import_error_tag = False
 
 # Fields description
 # description: human readable description
 # short_name: shortname to use un UI
 # unit: unit type
@@ -62,15 +61,15 @@
     stats is a dict
     """
 
     _default_public_refresh_interval = 300
 
     def __init__(self, args=None, config=None):
         """Init the plugin."""
-        super(PluginModel, self).__init__(args=args, config=config, fields_description=fields_description)
+        super().__init__(args=args, config=config, fields_description=fields_description)
 
         # We want to display the stat in the curse interface
         self.display_curse = True
 
         # Public information (see issue #2732)
         self.public_address = ""
         self.public_info = ""
@@ -100,24 +99,24 @@
 
         if self.input_method == 'local' and not import_error_tag:
             # Private IP address
             # Get the default gateway thanks to the netifaces lib
             try:
                 default_gw = netifaces.gateways()['default'][netifaces.AF_INET]
             except (KeyError, AttributeError) as e:
-                logger.debug("Cannot grab default gateway IP address ({})".format(e))
+                logger.debug(f"Cannot grab default gateway IP address ({e})")
                 return self.get_init_value()
             else:
                 stats['gateway'] = default_gw[0]
             # If multiple IP addresses are available, only the one with the default gateway is returned
             try:
                 address = netifaces.ifaddresses(default_gw[1])[netifaces.AF_INET][0]['addr']
                 mask = netifaces.ifaddresses(default_gw[1])[netifaces.AF_INET][0]['netmask']
             except (KeyError, AttributeError) as e:
-                logger.debug("Cannot grab private IP address ({})".format(e))
+                logger.debug(f"Cannot grab private IP address ({e})")
                 return self.get_init_value()
             else:
                 stats['address'] = address
                 stats['mask'] = mask
                 stats['mask_cidr'] = self.ip_to_cidr(stats['mask'])
 
             # Public IP address
@@ -125,15 +124,15 @@
             try:
                 if not self.public_disabled and (
                     self.public_address == "" or time_since_update > self.public_address_refresh_interval
                 ):
                     self.public_info = PublicIpInfo(self.public_api, self.public_username, self.public_password).get()
                     self.public_address = self.public_info['ip']
             except (KeyError, AttributeError, TypeError) as e:
-                logger.debug("Cannot grab public IP information ({})".format(e))
+                logger.debug(f"Cannot grab public IP information ({e})")
             else:
                 stats['public_address'] = (
                     self.public_address if not self.args.hide_public_info else self.__hide_ip(self.public_address)
                 )
                 stats['public_info_human'] = self.public_info_for_human(self.public_info)
 
         elif self.input_method == 'snmp':
@@ -207,15 +206,15 @@
         # See https://github.com/nicolargo/glances/issues/1417#issuecomment-469894399
         if ip is None:
             # Correct issue #1528
             return 0
         return sum(bin(int(x)).count('1') for x in ip.split('.'))
 
 
-class PublicIpInfo(object):
+class PublicIpInfo:
     """Get public IP information from online service."""
 
     def __init__(self, url, username, password, timeout=2):
         """Init the class."""
         self.url = url
         self.username = username
         self.password = password
@@ -238,15 +237,15 @@
         return info
 
     def _get_ip_public_info(self, queue_target, url, username, password):
         """Request the url service and put the result in the queue_target."""
         try:
             response = urlopen_auth(url, username, password).read()
         except Exception as e:
-            logger.debug("IP plugin - Cannot get public IP information from {} ({})".format(url, e))
+            logger.debug(f"IP plugin - Cannot get public IP information from {url} ({e})")
             queue_target.put(None)
         else:
             try:
                 queue_target.put(loads(response))
             except (ValueError, KeyError) as e:
-                logger.debug("IP plugin - Cannot load public IP information from {} ({})".format(url, e))
+                logger.debug(f"IP plugin - Cannot load public IP information from {url} ({e})")
                 queue_target.put(None)
```

### Comparing `glances-4.0.4/glances/plugins/irq/__init__.py` & `glances-4.0.5/glances/plugins/irq/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,26 +1,24 @@
-# -*- coding: utf-8 -*-
 #
 # This file is part of Glances.
 #
 # Copyright (C) 2018 Angelo Poerio <angelo.poerio@gmail.com>
 #
 # SPDX-License-Identifier: LGPL-3.0-only
 #
 
 """IRQ plugin."""
 
-import os
 import operator
+import os
 
-from glances.logger import logger
 from glances.globals import LINUX
-from glances.timer import getTimeSinceLastUpdate
+from glances.logger import logger
 from glances.plugins.plugin.model import GlancesPluginModel
-
+from glances.timer import getTimeSinceLastUpdate
 
 # Fields description
 # description: human readable description
 # short_name: shortname to use un UI
 # unit: unit type
 # rate: is it a rate ? If yes, // by time_since_update when displayed,
 # min_symbol: Auto unit should be used if value > than 1 'X' (K, M, G)...
@@ -39,17 +37,15 @@
     """Glances IRQ plugin.
 
     stats is a list
     """
 
     def __init__(self, args=None, config=None):
         """Init the plugin."""
-        super(PluginModel, self).__init__(
-            args=args, config=config, stats_init_value=[], fields_description=fields_description
-        )
+        super().__init__(args=args, config=config, stats_init_value=[], fields_description=fields_description)
 
         # We want to display the stat in the curse interface
         self.display_curse = True
 
         # Init the stats
         self.irq = GlancesIRQ()
 
@@ -83,15 +79,15 @@
         self.stats = stats
 
         return self.stats
 
     def update_views(self):
         """Update stats views."""
         # Call the father's method
-        super(PluginModel, self).update_views()
+        super().update_views()
 
     def msg_curse(self, args=None, max_width=None):
         """Return the dict to display in the curse interface."""
         # Init the return message
         ret = []
 
         # Only available on GNU/Linux
@@ -100,15 +96,15 @@
             return ret
 
         # Max size for the interface name
         if max_width:
             name_max_width = max_width - 7
         else:
             # No max_width defined, return an emptu curse message
-            logger.debug("No max_width defined for the {} plugin, it will not be displayed.".format(self.plugin_name))
+            logger.debug(f"No max_width defined for the {self.plugin_name} plugin, it will not be displayed.")
             return ret
 
         # Build the string message
         # Header
         msg = '{:{width}}'.format('IRQ', width=name_max_width)
         ret.append(self.curse_add_line(msg, "TITLE"))
         msg = '{:>9}'.format('Rate/s')
@@ -120,15 +116,15 @@
             ret.append(self.curse_add_line(msg))
             msg = '{:>9}'.format(str(i['irq_rate']))
             ret.append(self.curse_add_line(msg))
 
         return ret
 
 
-class GlancesIRQ(object):
+class GlancesIRQ:
     """This class manages the IRQ file."""
 
     IRQ_FILE = '/proc/interrupts'
 
     def __init__(self):
         """Init the class.
 
@@ -166,15 +162,15 @@
         1:      44487        341         44         72   IO-APIC   1-edge      i8042
         LOC:   33549868   22394684   32474570   21855077   Local timer interrupts
         """
         splitted_line = line.split()
         irq_line = splitted_line[0].replace(':', '')
         if irq_line.isdigit():
             # If the first column is a digit, use the alias (last column)
-            irq_line += '_{}'.format(splitted_line[-1])
+            irq_line += f'_{splitted_line[-1]}'
         return irq_line
 
     def __sum(self, line):
         """Return the IRQ sum number.
 
         IRQ line samples:
         1:     44487        341         44         72   IO-APIC   1-edge      i8042
@@ -213,11 +209,11 @@
                         'irq_line': irq_line,
                         'irq_rate': irq_rate,
                         'key': self.get_key(),
                         'time_since_update': time_since_update,
                     }
                     self.stats.append(irq_current)
                     self.lasts[irq_line] = current_irqs
-        except (OSError, IOError):
+        except OSError:
             pass
 
         return self.stats
```

### Comparing `glances-4.0.4/glances/plugins/load/__init__.py` & `glances-4.0.5/glances/plugins/load/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,25 +1,25 @@
-# -*- coding: utf-8 -*-
 #
 # This file is part of Glances.
 #
 # SPDX-FileCopyrightText: 2022 Nicolas Hennion <nicolas@nicolargo.com>
 #
 # SPDX-License-Identifier: LGPL-3.0-only
 #
 
 """Load plugin."""
 
 import os
+
 import psutil
 
 from glances.globals import iteritems
+from glances.logger import logger
 from glances.plugins.core import PluginModel as CorePluginModel
 from glances.plugins.plugin.model import GlancesPluginModel
-from glances.logger import logger
 
 # Fields description
 fields_description = {
     'min1': {
         'description': 'Average sum of the number of processes \
 waiting in the run-queue plus the number currently executing \
 over 1 minute.',
@@ -61,15 +61,15 @@
 # Get the number of logical CPU core only once
 # the variable is also shared with the QuickLook plugin
 nb_log_core = 1
 nb_phys_core = 1
 try:
     core = CorePluginModel().update()
 except Exception as e:
-    logger.warning('Error: Can not retrieve the CPU core number (set it to 1) ({})'.format(e))
+    logger.warning(f'Error: Can not retrieve the CPU core number (set it to 1) ({e})')
 else:
     if 'log' in core:
         nb_log_core = core['log']
     if 'phys' in core:
         nb_phys_core = core['phys']
 
 
@@ -77,15 +77,15 @@
     """Glances load plugin.
 
     stats is a dict
     """
 
     def __init__(self, args=None, config=None):
         """Init the plugin."""
-        super(PluginModel, self).__init__(
+        super().__init__(
             args=args, config=config, items_history_list=items_history_list, fields_description=fields_description
         )
 
         # We want to display the stat in the curse interface
         self.display_curse = True
 
     @GlancesPluginModel._check_decorator
@@ -106,16 +106,15 @@
                 stats = {'min1': load[0], 'min5': load[1], 'min15': load[2], 'cpucore': get_nb_log_core()}
 
         elif self.input_method == 'snmp':
             # Update stats using SNMP
             stats = self.get_stats_snmp(snmp_oid=snmp_oid)
 
             if stats['min1'] == '':
-                stats = self.get_init_value()
-                return stats
+                return self.get_init_value()
 
             # Python 3 return a dict like:
             # {'min1': "b'0.08'", 'min5': "b'0.12'", 'min15': "b'0.15'"}
             for k, v in iteritems(stats):
                 stats[k] = float(v)
 
             stats['cpucore'] = get_nb_log_core()
@@ -124,15 +123,15 @@
         self.stats = stats
 
         return self.stats
 
     def update_views(self):
         """Update stats views."""
         # Call the father's method
-        super(PluginModel, self).update_views()
+        super().update_views()
 
         # Add specifics information
         try:
             # Alert and log
             self.views['min15']['decoration'] = self.get_alert_log(
                 self.stats['min15'], maximum=100 * self.stats['cpucore']
             )
@@ -160,25 +159,25 @@
         # Core number
         if 'cpucore' in self.stats and self.stats['cpucore'] > 0:
             msg = '{:3}core'.format(int(self.stats['cpucore']))
             ret.append(self.curse_add_line(msg))
         # Loop over 1min, 5min and 15min load
         for load_time in ['1', '5', '15']:
             ret.append(self.curse_new_line())
-            msg = '{:7}'.format('{} min'.format(load_time))
+            msg = '{:7}'.format(f'{load_time} min')
             ret.append(self.curse_add_line(msg))
             if args.disable_irix and get_nb_log_core() != 0:
                 # Enable Irix mode for load (see issue #1554)
-                load_stat = self.stats['min{}'.format(load_time)] / get_nb_log_core() * 100
-                msg = '{:>5.1f}%'.format(load_stat)
+                load_stat = self.stats[f'min{load_time}'] / get_nb_log_core() * 100
+                msg = f'{load_stat:>5.1f}%'
             else:
                 # Default mode for load
-                load_stat = self.stats['min{}'.format(load_time)]
-                msg = '{:>6.2f}'.format(load_stat)
-            ret.append(self.curse_add_line(msg, self.get_views(key='min{}'.format(load_time), option='decoration')))
+                load_stat = self.stats[f'min{load_time}']
+                msg = f'{load_stat:>6.2f}'
+            ret.append(self.curse_add_line(msg, self.get_views(key=f'min{load_time}', option='decoration')))
 
         return ret
 
 
 def get_nb_log_core():
     """Get the number of logical CPU core."""
     return nb_log_core
@@ -201,9 +200,8 @@
         try:
             load_average = os.getloadavg()
         except (AttributeError, OSError):
             pass
 
     if load_average and percent:
         return tuple([round(i / get_nb_log_core() * 100, 1) for i in load_average])
-    else:
-        return load_average
+    return load_average
```

### Comparing `glances-4.0.4/glances/plugins/mem/__init__.py` & `glances-4.0.5/glances/plugins/mem/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,21 @@
-# -*- coding: utf-8 -*-
 #
 # This file is part of Glances.
 #
 # SPDX-FileCopyrightText: 2022 Nicolas Hennion <nicolas@nicolargo.com>
 #
 # SPDX-License-Identifier: LGPL-3.0-only
 #
 
 """Virtual memory plugin."""
 
-from glances.plugins.plugin.model import GlancesPluginModel
-
 import psutil
 
+from glances.plugins.plugin.model import GlancesPluginModel
+
 # Fields description
 fields_description = {
     'total': {'description': 'Total physical memory available.', 'unit': 'bytes', 'min_symbol': 'K'},
     'available': {
         'description': 'The actual amount of available memory that can be given instantly \
 to processes that request more memory in bytes; this is calculated by summing \
 different memory values depending on the platform (e.g. free + buffers + cached on Linux) \
@@ -109,15 +108,15 @@
     """Glances' memory plugin.
 
     stats is a dict
     """
 
     def __init__(self, args=None, config=None):
         """Init the plugin."""
-        super(PluginModel, self).__init__(
+        super().__init__(
             args=args, config=config, items_history_list=items_history_list, fields_description=fields_description
         )
 
         # We want to display the stat in the curse interface
         self.display_curse = True
 
     @GlancesPluginModel._check_decorator
@@ -215,15 +214,15 @@
         self.stats = stats
 
         return self.stats
 
     def update_views(self):
         """Update stats views."""
         # Call the father's method
-        super(PluginModel, self).update_views()
+        super().update_views()
 
         # Add specifics information
         # Alert and log
         self.views['percent']['decoration'] = self.get_alert_log(self.stats['used'], maximum=self.stats['total'])
         # Optional
         for key in ['active', 'inactive', 'buffers', 'cached']:
             if key in self.stats:
```

### Comparing `glances-4.0.4/glances/plugins/memswap/__init__.py` & `glances-4.0.5/glances/plugins/memswap/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,22 @@
-# -*- coding: utf-8 -*-
 #
 # This file is part of Glances.
 #
 # SPDX-FileCopyrightText: 2022 Nicolas Hennion <nicolas@nicolargo.com>
 #
 # SPDX-License-Identifier: LGPL-3.0-only
 #
 
 """Swap memory plugin."""
 
+import psutil
+
 from glances.globals import iterkeys
-from glances.timer import getTimeSinceLastUpdate
 from glances.plugins.plugin.model import GlancesPluginModel
-
-import psutil
+from glances.timer import getTimeSinceLastUpdate
 
 # Fields description
 fields_description = {
     'total': {'description': 'Total swap memory.', 'unit': 'bytes', 'min_symbol': 'K'},
     'used': {'description': 'Used swap memory.', 'unit': 'bytes', 'min_symbol': 'K'},
     'free': {'description': 'Free swap memory.', 'unit': 'bytes', 'min_symbol': 'K'},
     'percent': {'description': 'Used swap memory in percentage.', 'unit': 'percent'},
@@ -56,15 +55,15 @@
     """Glances swap memory plugin.
 
     stats is a dict
     """
 
     def __init__(self, args=None, config=None):
         """Init the plugin."""
-        super(PluginModel, self).__init__(
+        super().__init__(
             args=args, config=config, items_history_list=items_history_list, fields_description=fields_description
         )
 
         # We want to display the stat in the curse interface
         self.display_curse = True
 
     @GlancesPluginModel._check_decorator
@@ -141,15 +140,15 @@
         self.stats = stats
 
         return self.stats
 
     def update_views(self):
         """Update stats views."""
         # Call the father's method
-        super(PluginModel, self).update_views()
+        super().update_views()
 
         # Add specifics information
         # Alert and log
         if 'used' in self.stats and 'total' in self.stats and 'percent' in self.stats:
             self.views['percent']['decoration'] = self.get_alert_log(self.stats['used'], maximum=self.stats['total'])
 
     def msg_curse(self, args=None, max_width=None):
```

### Comparing `glances-4.0.4/glances/plugins/network/__init__.py` & `glances-4.0.5/glances/plugins/network/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,22 @@
-# -*- coding: utf-8 -*-
 #
 # This file is part of Glances.
 #
 # SPDX-FileCopyrightText: 2022 Nicolas Hennion <nicolas@nicolargo.com>
 #
 # SPDX-License-Identifier: LGPL-3.0-only
 #
 
 """Network plugin."""
-from __future__ import unicode_literals
-
-from glances.plugins.plugin.model import GlancesPluginModel
-from glances.logger import logger
 
 import psutil
 
+from glances.logger import logger
+from glances.plugins.plugin.model import GlancesPluginModel
+
 # Fields description
 # description: human readable description
 # short_name: shortname to use un UI
 # unit: unit type
 # rate: if True then compute and add *_gauge and *_rate_per_is fields
 # min_symbol: Auto unit should be used if value > than 1 'X' (K, M, G)...
 fields_description = {
@@ -68,15 +66,15 @@
     """Glances network plugin.
 
     stats is a list
     """
 
     def __init__(self, args=None, config=None):
         """Init the plugin."""
-        super(PluginModel, self).__init__(
+        super().__init__(
             args=args,
             config=config,
             items_history_list=items_history_list,
             fields_description=fields_description,
             stats_init_value=[],
         )
 
@@ -126,29 +124,29 @@
         # { 'veth4cbf8f0a': snetio(
         #   bytes_sent=102038421, bytes_recv=1263258,
         #   packets_sent=25046, packets_recv=14114,
         #   errin=0, errout=0, dropin=0, dropout=0), ... }
         try:
             net_io_counters = psutil.net_io_counters(pernic=True)
         except UnicodeDecodeError as e:
-            logger.debug('Can not get network interface counters ({})'.format(e))
+            logger.debug(f'Can not get network interface counters ({e})')
             return self.stats
 
         # Grab interface's status (issue #765)
         # Grab interface's speed (issue #718)
         # Example:
         # { 'veth4cbf8f0a': snicstats(
         #   isup=True, duplex=<NicDuplex.NIC_DUPLEX_FULL: 2>,
         #   speed=10000, mtu=1500, flags='up,broadcast,running,multicast'), ... }
         net_status = {}
         try:
             net_status = psutil.net_if_stats()
         except OSError as e:
             # see psutil #797/glances #1106
-            logger.debug('Can not get network interface status ({})'.format(e))
+            logger.debug(f'Can not get network interface status ({e})')
 
         for interface_name, interface_stat in net_io_counters.items():
             # Do not take hidden interface into account
             # or KeyError: 'eth0' when interface is not connected #1348
             if not self.is_display(interface_name) or interface_name not in net_status:
                 continue
 
@@ -176,15 +174,15 @@
             stats.append(stat)
 
         return stats
 
     def update_views(self):
         """Update stats views."""
         # Call the father's method
-        super(PluginModel, self).update_views()
+        super().update_views()
 
         # Check if the stats should be hidden
         self.update_views_hidden()
 
         # Add specifics information
         # Alert
         for i in self.get_raw():
@@ -222,15 +220,15 @@
             return ret
 
         # Max size for the interface name
         if max_width:
             name_max_width = max_width - 12
         else:
             # No max_width defined, return an emptu curse message
-            logger.debug("No max_width defined for the {} plugin, it will not be displayed.".format(self.plugin_name))
+            logger.debug(f"No max_width defined for the {self.plugin_name} plugin, it will not be displayed.")
             return ret
 
         # Header
         msg = '{:{width}}'.format('NETWORK', width=name_max_width)
         ret.append(self.curse_add_line(msg, "TITLE"))
         if args.network_cumul:
             # Cumulative stats
@@ -257,15 +255,15 @@
                 ret.append(self.curse_add_line(msg))
         # Interface list (sorted by name)
         for i in self.sorted_stats():
             # Do not display interface in down state (issue #765)
             if ('is_up' in i) and (i['is_up'] is False):
                 continue
             # Hide stats if never be different from 0 (issue #1787)
-            if all([self.get_views(item=i[self.get_key()], key=f, option='hidden') for f in self.hide_zero_fields]):
+            if all(self.get_views(item=i[self.get_key()], key=f, option='hidden') for f in self.hide_zero_fields):
                 continue
             # Format stats
             # Is there an alias for the interface name ?
             if i['alias'] is None:
                 if_name = i['interface_name'].split(':')[0]
             else:
                 if_name = i['alias']
@@ -296,24 +294,24 @@
                 continue
 
             # New line
             ret.append(self.curse_new_line())
             msg = '{:{width}}'.format(if_name, width=name_max_width)
             ret.append(self.curse_add_line(msg))
             if args.network_sum:
-                msg = '{:>14}'.format(ax)
+                msg = f'{ax:>14}'
                 ret.append(self.curse_add_line(msg))
             else:
-                msg = '{:>7}'.format(rx)
+                msg = f'{rx:>7}'
                 ret.append(
                     self.curse_add_line(
                         msg, self.get_views(item=i[self.get_key()], key='bytes_recv', option='decoration')
                     )
                 )
-                msg = '{:>7}'.format(tx)
+                msg = f'{tx:>7}'
                 ret.append(
                     self.curse_add_line(
                         msg, self.get_views(item=i[self.get_key()], key='bytes_sent', option='decoration')
                     )
                 )
 
         return ret
```

### Comparing `glances-4.0.4/glances/plugins/now/__init__.py` & `glances-4.0.5/glances/plugins/now/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-# -*- coding: utf-8 -*-
 #
 # This file is part of Glances.
 #
 # SPDX-FileCopyrightText: 2024 Nicolas Hennion <nicolas@nicolargo.com>
 #
 # SPDX-License-Identifier: LGPL-3.0-only
 #
 
 """Now (current date) plugin."""
 
-from time import tzname, strftime
 import datetime
+from time import strftime, tzname
+
 from glances.plugins.plugin.model import GlancesPluginModel
 
 # Fields description
 # description: human readable description
 # short_name: shortname to use un UI
 # unit: unit type
 # rate: if True then compute and add *_gauge and *_rate_per_is fields
@@ -33,17 +33,15 @@
         "custom": "2024-04-27 16:43:52 CEST",
         "iso": "2024-04-27T16:28:23.382748"
     }
     """
 
     def __init__(self, args=None, config=None):
         """Init the plugin."""
-        super(PluginModel, self).__init__(
-            args=args, config=config, fields_description=fields_description, stats_init_value={}
-        )
+        super().__init__(args=args, config=config, fields_description=fields_description, stats_init_value={})
 
         # We want to display the stat in the curse interface
         self.display_curse = True
 
         # Set the message position
         self.align = 'bottom'
```

### Comparing `glances-4.0.4/glances/plugins/percpu/__init__.py` & `glances-4.0.5/glances/plugins/percpu/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 #
 # This file is part of Glances.
 #
 # SPDX-FileCopyrightText: 2022 Nicolas Hennion <nicolas@nicolargo.com>
 #
 # SPDX-License-Identifier: LGPL-3.0-only
 #
@@ -92,15 +91,15 @@
 
     'stats' is a list of dictionaries that contain the utilization percentages
     for each CPU.
     """
 
     def __init__(self, args=None, config=None):
         """Init the plugin."""
-        super(PluginModel, self).__init__(
+        super().__init__(
             args=args,
             config=config,
             items_history_list=items_history_list,
             stats_init_value=[],
             fields_description=fields_description,
         )
 
@@ -155,15 +154,15 @@
             ret.append(self.curse_add_line(msg, "TITLE"))
             header.insert(0, 'total')
 
         # Per CPU stats displayed per line
         for stat in header:
             if stat not in self.stats[0]:
                 continue
-            msg = '{:>7}'.format(stat)
+            msg = f'{stat:>7}'
             ret.append(self.curse_add_line(msg))
 
         # Manage the maximum number of CPU to display (related to enhancement request #2734)
         if len(self.stats) > self.max_cpu_display:
             # If the number of CPU is > max_cpu_display then sort and display top 'n'
             percpu_list = sorted(self.stats, key=lambda x: x['total'], reverse=True)
         else:
@@ -172,26 +171,26 @@
         # Per CPU stats displayed per column
         for cpu in percpu_list[0 : self.max_cpu_display]:
             ret.append(self.curse_new_line())
             if self.is_disabled('quicklook'):
                 try:
                     cpu_id = cpu[cpu['key']]
                     if cpu_id < 10:
-                        msg = 'CPU{:1} '.format(cpu_id)
+                        msg = f'CPU{cpu_id:1} '
                     else:
-                        msg = '{:4} '.format(cpu_id)
+                        msg = f'{cpu_id:4} '
                 except TypeError:
                     # TypeError: string indices must be integers (issue #1027)
                     msg = '{:4} '.format('?')
                 ret.append(self.curse_add_line(msg))
             for stat in header:
                 if stat not in self.stats[0]:
                     continue
                 try:
-                    msg = '{:6.1f}%'.format(cpu[stat])
+                    msg = f'{cpu[stat]:6.1f}%'
                 except TypeError:
                     msg = '{:>6}%'.format('?')
                 ret.append(self.curse_add_line(msg, self.get_alert(cpu[stat], header=stat)))
 
         # Add a new line with sum of all others CPU
         if len(self.stats) > self.max_cpu_display:
             ret.append(self.curse_new_line())
@@ -200,13 +199,13 @@
             for stat in header:
                 if stat not in self.stats[0]:
                     continue
                 cpu_stat = sum([i[stat] for i in percpu_list[0 : self.max_cpu_display]]) / len(
                     [i[stat] for i in percpu_list[0 : self.max_cpu_display]]
                 )
                 try:
-                    msg = '{:6.1f}%'.format(cpu_stat)
+                    msg = f'{cpu_stat:6.1f}%'
                 except TypeError:
                     msg = '{:>6}%'.format('?')
                 ret.append(self.curse_add_line(msg, self.get_alert(cpu_stat, header=stat)))
 
         return ret
```

### Comparing `glances-4.0.4/glances/plugins/plugin/model.py` & `glances-4.0.5/glances/plugins/plugin/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,34 +1,32 @@
-# -*- coding: utf-8 -*-
 #
 # This file is part of Glances.
 #
 # SPDX-FileCopyrightText: 2024 Nicolas Hennion <nicolas@nicolargo.com>
 #
 # SPDX-License-Identifier: LGPL-3.0-only
 #
 
 """
 I am your father...
 
 ...of all Glances model plugins.
 """
 
-import re
 import copy
+import re
 
-from glances.globals import iterkeys, itervalues, listkeys, mean, nativestr, json_dumps, json_dumps_dictlist, dictlist
 from glances.actions import GlancesActions
+from glances.events_list import glances_events
+from glances.globals import dictlist, iterkeys, itervalues, json_dumps, json_dumps_dictlist, listkeys, mean, nativestr
 from glances.history import GlancesHistory
 from glances.logger import logger
-from glances.events_list import glances_events
+from glances.outputs.glances_unicode import unicode_message
 from glances.thresholds import glances_thresholds
 from glances.timer import Counter, Timer, getTimeSinceLastUpdate
-from glances.outputs.glances_unicode import unicode_message
-
 
 fields_unit_short = {'percent': '%'}
 
 fields_unit_type = {
     'percent': 'float',
     'percents': 'float',
     'number': 'int',
@@ -40,15 +38,15 @@
     'second': 'int',
     'seconds': 'int',
     'byte': 'int',
     'bytes': 'int',
 }
 
 
-class GlancesPluginModel(object):
+class GlancesPluginModel:
     """Main class for Glances plugin model."""
 
     def __init__(self, args=None, config=None, items_history_list=None, stats_init_value={}, fields_description=None):
         """Init the plugin of plugins model class.
 
         All Glances' plugins model should inherit from this class. Most of the
         methods are already implemented in the father classes.
@@ -74,15 +72,15 @@
         # Build the plugin name
         # Internal or external module (former prefixed by 'glances.plugins')
         _mod = self.__class__.__module__.replace('glances.plugins.', '')
         self.plugin_name = _mod.split('.')[0]
 
         if self.plugin_name.startswith('glances_'):
             self.plugin_name = self.plugin_name.split('glances_')[1]
-        logger.debug("Init {} plugin".format(self.plugin_name))
+        logger.debug(f"Init {self.plugin_name} plugin")
 
         # Init the args
         self.args = args
 
         # Init the default alignment (for curses)
         self._align = 'left'
 
@@ -91,27 +89,27 @@
         self._short_system_name = None
 
         # Init the history list
         self.items_history_list = items_history_list
         self.stats_history = self.init_stats_history()
 
         # Init the limits (configuration keys) dictionary
-        self._limits = dict()
+        self._limits = {}
         if config is not None:
-            logger.debug('Load section {} in {}'.format(self.plugin_name, config.config_file_paths()))
+            logger.debug(f'Load section {self.plugin_name} in {config.config_file_paths()}')
             self.load_limits(config=config)
 
         # Init the alias (dictionnary)
         self.alias = self.read_alias()
 
         # Init the actions
         self.actions = GlancesActions(args=args)
 
         # Init the views
-        self.views = dict()
+        self.views = {}
 
         # Hide stats if all the hide_zero_fields has never been != 0
         # Default is False, always display stats
         self.hide_zero = False
         self.hide_zero_fields = []
 
         # Set the initial refresh time to display stats the first time
@@ -144,19 +142,19 @@
 
         This method should be overwritten by child classes.
         """
         self.stats = self.get_init_value()
 
     def exit(self):
         """Just log an event when Glances exit."""
-        logger.debug("Stop the {} plugin".format(self.plugin_name))
+        logger.debug(f"Stop the {self.plugin_name} plugin")
 
     def get_key(self):
         """Return the key of the list."""
-        return None
+        return
 
     def is_enabled(self, plugin_name=None):
         """Return true if plugin is enabled."""
         if not plugin_name:
             plugin_name = self.plugin_name
         try:
             d = getattr(self.args, 'disable_' + plugin_name)
@@ -171,22 +169,22 @@
     def history_enable(self):
         return self.args is not None and not self.args.disable_history and self.get_items_history_list() is not None
 
     def init_stats_history(self):
         """Init the stats history (dict of GlancesAttribute)."""
         if self.history_enable():
             init_list = [a['name'] for a in self.get_items_history_list()]
-            logger.debug("Stats history activated for plugin {} (items: {})".format(self.plugin_name, init_list))
+            logger.debug(f"Stats history activated for plugin {self.plugin_name} (items: {init_list})")
         return GlancesHistory()
 
     def reset_stats_history(self):
         """Reset the stats history (dict of GlancesAttribute)."""
         if self.history_enable():
             reset_list = [a['name'] for a in self.get_items_history_list()]
-            logger.debug("Reset history for plugin {} (items: {})".format(self.plugin_name, reset_list))
+            logger.debug(f"Reset history for plugin {self.plugin_name} (items: {reset_list})")
             self.stats_history.reset()
 
     def update_stats_history(self):
         """Update stats history."""
         # Build the history
         if not (self.get_export() and self.history_enable()):
             return
@@ -224,19 +222,17 @@
         - the stats history (dict of list) if item is None
         - the stats history for the given item (list) instead
         - None if item did not exist in the history
         """
         s = self.stats_history.get(nb=nb)
         if item is None:
             return s
-        else:
-            if item in s:
-                return s[item]
-            else:
-                return None
+        if item in s:
+            return s[item]
+        return None
 
     def get_export_history(self, item=None):
         """Return the stats history object to export."""
         return self.get_raw_history(item=item)
 
     def get_stats_history(self, item=None, nb=0):
         """Return the stats history (JSON format)."""
@@ -284,26 +280,24 @@
         key = self.get_key()
         if key is None:
             return self.stats
         try:
             return sorted(
                 self.stats,
                 key=lambda stat: tuple(
-                    map(
-                        lambda part: int(part) if part.isdigit() else part.lower(),
-                        re.split(r"(\d+|\D+)", self.has_alias(stat[key]) or stat[key]),
-                    )
+                    int(part) if part.isdigit() else part.lower()
+                    for part in re.split(r"(\d+|\D+)", self.has_alias(stat[key]) or stat[key])
                 ),
             )
         except TypeError:
             # Correct "Starting an alias with a number causes a crash #1885"
             return sorted(
                 self.stats,
                 key=lambda stat: tuple(
-                    map(lambda part: part.lower(), re.split(r"(\d+|\D+)", self.has_alias(stat[key]) or stat[key]))
+                    part.lower() for part in re.split(r"(\d+|\D+)", self.has_alias(stat[key]) or stat[key])
                 ),
             )
 
     @short_system_name.setter
     def short_system_name(self, short_name):
         """Set the short detected OS name (SNMP)."""
         self._short_system_name = short_name
@@ -407,40 +401,38 @@
         """Return the stats object for a specific item=value.
 
         Return None if the item=value does not exist
         Return None if the item is not a list of dict
         """
         if not isinstance(self.get_raw(), list):
             return None
-        else:
-            if (not isinstance(value, int) and not isinstance(value, float)) and value.isdigit():
-                value = int(value)
-            try:
-                return {value: [i for i in self.get_raw() if i[item] == value]}
-            except (KeyError, ValueError) as e:
-                logger.error("Cannot get item({})=value({}) ({})".format(item, value, e))
-                return None
+
+        if (not isinstance(value, int) and not isinstance(value, float)) and value.isdigit():
+            value = int(value)
+        try:
+            return {value: [i for i in self.get_raw() if i[item] == value]}
+        except (KeyError, ValueError) as e:
+            logger.error(f"Cannot get item({item})=value({value}) ({e})")
+            return None
 
     def get_stats_value(self, item, value):
         """Return the stats object for a specific item=value in JSON format.
 
         Stats should be a list of dict (processlist, network...)
         """
         rsv = self.get_raw_stats_value(item, value)
         if rsv is None:
             return None
-        else:
-            return json_dumps(rsv)
+        return json_dumps(rsv)
 
     def get_item_info(self, item, key, default=None):
         """Return the item info grabbed into self.fields_description."""
         if self.fields_description is None or item not in self.fields_description:
             return default
-        else:
-            return self.fields_description[item].get(key, default)
+        return self.fields_description[item].get(key, default)
 
     def update_views_hidden(self):
         """Update the hidden views
 
         If the self.hide_zero is set then update the hidden field of the view
         It will check if all fields values are already be different from 0
         In this case, the hidden field is set to True
@@ -455,27 +447,27 @@
             self.update_views_hidden()
         """
         if not self.hide_zero:
             return False
         if isinstance(self.get_raw(), list) and self.get_raw() is not None and self.get_key() is not None:
             # Stats are stored in a list of dict (ex: NETWORK, FS...)
             for i in self.get_raw():
-                if any([i[f] for f in self.hide_zero_fields]):
+                if any(i[f] for f in self.hide_zero_fields):
                     for f in self.hide_zero_fields:
                         self.views[i[self.get_key()]][f]['_zero'] = self.views[i[self.get_key()]][f]['hidden']
                 for f in self.hide_zero_fields:
                     self.views[i[self.get_key()]][f]['hidden'] = self.views[i[self.get_key()]][f]['_zero'] and i[f] == 0
         elif isinstance(self.get_raw(), dict) and self.get_raw() is not None:
             #
             # Warning: This code has never been tested because
             # no plugin with dict instance use the hidden function...
             #
             # Stats are stored in a dict (ex: CPU, LOAD...)
             for key in listkeys(self.get_raw()):
-                if any([self.get_raw()[f] for f in self.hide_zero_fields]):
+                if any(self.get_raw()[f] for f in self.hide_zero_fields):
                     for f in self.hide_zero_fields:
                         self.views[f]['_zero'] = self.views[f]['hidden']
                 for f in self.hide_zero_fields:
                     self.views[f]['hidden'] = self.views['_zero'] and self.views[f] == 0
         return True
 
     def update_views(self):
@@ -532,15 +524,15 @@
 
     def set_views(self, input_views):
         """Set the views to input_views."""
         self.views = input_views
 
     def reset_views(self):
         """Reset the views to input_views."""
-        self.views = dict()
+        self.views = {}
 
     def get_views(self, item=None, key=None, option=None):
         """Return the views object.
 
         If key is None, return all the view for the current plugin
         else if option is None return the view for the specific key (all option)
         else return the view of the specific key/option
@@ -550,22 +542,19 @@
         if item is None:
             item_views = self.views
         else:
             item_views = self.views[item]
 
         if key is None:
             return item_views
-        else:
-            if option is None:
-                return item_views[key]
-            else:
-                if option in item_views[key]:
-                    return item_views[key][option]
-                else:
-                    return 'DEFAULT'
+        if option is None:
+            return item_views[key]
+        if option in item_views[key]:
+            return item_views[key][option]
+        return 'DEFAULT'
 
     def get_json_views(self, item=None, key=None, option=None):
         """Return the views (in JSON)."""
         return json_dumps(self.get_views(item, key, option))
 
     def load_limits(self, config):
         """Load limits from the configuration file, if it exists."""
@@ -586,15 +575,15 @@
             for level, _ in config.items(self.plugin_name):
                 # Read limits
                 limit = '_'.join([self.plugin_name, level])
                 try:
                     self._limits[limit] = config.get_float_value(self.plugin_name, level)
                 except ValueError:
                     self._limits[limit] = config.get_value(self.plugin_name, level).split(",")
-                logger.debug("Load limit: {} = {}".format(limit, self._limits[limit]))
+                logger.debug(f"Load limit: {limit} = {self._limits[limit]}")
 
         return True
 
     @property
     def limits(self):
         """Return the limits object."""
         return self._limits
@@ -617,22 +606,21 @@
 
     def get_refresh_time(self):
         """Return the plugin refresh time"""
         return self.get_refresh()
 
     def set_limits(self, item, value):
         """Set the limits object."""
-        self._limits['{}_{}'.format(self.plugin_name, item)] = value
+        self._limits[f'{self.plugin_name}_{item}'] = value
 
     def get_limits(self, item=None):
         """Return the limits object."""
         if item is None:
             return self._limits
-        else:
-            return self._limits.get('{}_{}'.format(self.plugin_name, item), None)
+        return self._limits.get(f'{self.plugin_name}_{item}', None)
 
     def get_stats_action(self):
         """Return stats for the action.
 
         By default return all the stats.
         Can be overwrite by plugins implementation.
         For example, Docker will return self.stats['containers']
@@ -739,20 +727,19 @@
         # Default is 'OK'
         return ret + log_str
 
     def filter_stats(self, stats):
         """Filter the stats to keep only the fields we want (the one defined in fields_description)."""
         if hasattr(stats, '_asdict'):
             return {k: v for k, v in stats._asdict().items() if k in self.fields_description}
-        elif isinstance(stats, dict):
+        if isinstance(stats, dict):
             return {k: v for k, v in stats.items() if k in self.fields_description}
-        elif isinstance(stats, list):
+        if isinstance(stats, list):
             return [self.filter_stats(s) for s in stats]
-        else:
-            return stats
+        return stats
 
     def manage_threshold(self, stat_name, trigger):
         """Manage the threshold for the current stat."""
         glances_thresholds.add(stat_name, trigger)
 
     def manage_action(self, stat_name, trigger, header, action_key):
         """Manage the action for the current stat."""
@@ -790,28 +777,27 @@
             current=current, minimum=minimum, maximum=maximum, header=header, action_key=action_key, log=True
         )
 
     def is_limit(self, criticality, stat_name=""):
         """Return true if the criticality limit exist for the given stat_name"""
         if stat_name == "":
             return self.plugin_name + '_' + criticality in self._limits
-        else:
-            return stat_name + '_' + criticality in self._limits
+        return stat_name + '_' + criticality in self._limits
 
     def get_limit(self, criticality=None, stat_name=""):
         """Return the limit value for the given criticality.
         If criticality is None, return the dict of all the limits."""
         if criticality is None:
             return self._limits
 
         # Get the limit for stat + header
         # Example: network_wlan0_rx_careful
         if stat_name + '_' + criticality in self._limits:
             return self._limits[stat_name + '_' + criticality]
-        elif self.plugin_name + '_' + criticality in self._limits:
+        if self.plugin_name + '_' + criticality in self._limits:
             return self._limits[self.plugin_name + '_' + criticality]
 
         # No key found, the raise an error
         raise KeyError
 
     def get_limit_action(self, criticality, stat_name=""):
         """Return the tuple (action, repeat) for the alert.
@@ -837,18 +823,17 @@
 
     def get_limit_log(self, stat_name, default_action=False):
         """Return the log tag for the alert."""
         # Get the log tag for stat + header
         # Example: network_wlan0_rx_log
         if stat_name + '_log' in self._limits:
             return self._limits[stat_name + '_log'][0].lower() == 'true'
-        elif self.plugin_name + '_log' in self._limits:
+        if self.plugin_name + '_log' in self._limits:
             return self._limits[self.plugin_name + '_log'][0].lower() == 'true'
-        else:
-            return default_action
+        return default_action
 
     def get_conf_value(self, value, header="", plugin_name=None, default=[]):
         """Return the configuration (header_) value for the current plugin.
 
         ...or the one given by the plugin_name var.
         """
         if plugin_name is None:
@@ -892,22 +877,20 @@
             j for j in [re.fullmatch(i.lower(), value.lower()) for i in self.get_conf_value('hide', header=header)]
         )
 
     def is_display(self, value, header=""):
         """Return True if the value should be displayed in the UI"""
         if self.get_conf_value('show', header=header) != []:
             return self.is_show(value, header=header)
-        else:
-            return not self.is_hide(value, header=header)
+        return not self.is_hide(value, header=header)
 
     def read_alias(self):
         if self.plugin_name + '_' + 'alias' in self._limits:
             return {i.split(':')[0].lower(): i.split(':')[1] for i in self._limits[self.plugin_name + '_' + 'alias']}
-        else:
-            return dict()
+        return {}
 
     def has_alias(self, header):
         """Return the alias name for the relative header it it exists otherwise None."""
         return self.alias.get(header, None)
 
     def msg_curse(self, args=None, max_width=None):
         """Return default string to display in the curse interface."""
@@ -1035,15 +1018,15 @@
             and self.fields_description[key]['rate'] is True
         ):
             value = self.stats.get(key + '_rate_per_sec', None)
         else:
             value = self.stats.get(key, None)
 
         if width is None:
-            msg_item = header + '{}'.format(key_name) + separator
+            msg_item = header + f'{key_name}' + separator
             msg_template_float = '{:.1f}{}'
             msg_template = '{}{}'
         else:
             # Define the size of the message
             # item will be on the left
             # value will be on the right
             msg_item = header + '{:{width}}'.format(key_name, width=width - 7) + separator
@@ -1134,15 +1117,15 @@
                     if symbol in 'MK':
                         decimal_precision = 0
                     else:
                         decimal_precision = min(1, decimal_precision)
                 elif symbol in 'K':
                     decimal_precision = 0
                 return '{:.{decimal}f}{symbol}'.format(value, decimal=decimal_precision, symbol=symbol)
-        return '{!s}'.format(number)
+        return f'{number!s}'
 
     def trend_msg(self, trend, significant=1):
         """Return the trend message.
 
         Do not take into account if trend < significant
         """
         ret = '-'
@@ -1180,19 +1163,17 @@
     def _log_result_decorator(fct):
         """Log (DEBUG) the result of the function fct."""
 
         def wrapper(*args, **kw):
             counter = Counter()
             ret = fct(*args, **kw)
             duration = counter.get()
-            logger.debug(
-                "{} {} {} return {} in {} seconds".format(
-                    args[0].__class__.__name__, args[0].__class__.__module__, fct.__name__, ret, duration
-                )
-            )
+            class_name = args[0].__class__.__name__
+            class_module = args[0].__class__.__module__
+            logger.debug(f"{class_name} {class_module} {fct.__name__} return {ret} in {duration} seconds")
             return ret
 
         return wrapper
 
     def _manage_rate(fct):
         """Manage rate decorator for update method."""
```

### Comparing `glances-4.0.4/glances/plugins/ports/__init__.py` & `glances-4.0.5/glances/plugins/ports/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,39 +1,38 @@
-# -*- coding: utf-8 -*-
 #
 # This file is part of Glances.
 #
 # SPDX-FileCopyrightText: 2022 Nicolas Hennion <nicolas@nicolargo.com>
 #
 # SPDX-License-Identifier: LGPL-3.0-only
 #
 
 """Ports scanner plugin."""
 
+import numbers
 import os
+import socket
 import subprocess
 import threading
-import socket
 import time
-import numbers
 
-from glances.globals import WINDOWS, MACOS, BSD, bool_type
-from glances.ports_list import GlancesPortsList
-from glances.web_list import GlancesWebList
-from glances.timer import Counter
+from glances.globals import BSD, MACOS, WINDOWS, bool_type
 from glances.logger import logger
 from glances.plugins.plugin.model import GlancesPluginModel
+from glances.ports_list import GlancesPortsList
+from glances.timer import Counter
+from glances.web_list import GlancesWebList
 
 try:
     import requests
 
     requests_tag = True
 except ImportError as e:
     requests_tag = False
-    logger.warning("Missing Python Lib ({}), Ports plugin is limited to port scanning".format(e))
+    logger.warning(f"Missing Python Lib ({e}), Ports plugin is limited to port scanning")
 
 # Fields description
 # description: human readable description
 # short_name: shortname to use un UI
 # unit: unit type
 # rate: is it a rate ? If yes, // by time_since_update when displayed,
 # min_symbol: Auto unit should be used if value > than 1 'X' (K, M, G)...
@@ -68,17 +67,15 @@
 
 
 class PluginModel(GlancesPluginModel):
     """Glances ports scanner plugin."""
 
     def __init__(self, args=None, config=None):
         """Init the plugin."""
-        super(PluginModel, self).__init__(
-            args=args, config=config, stats_init_value=[], fields_description=fields_description
-        )
+        super().__init__(args=args, config=config, stats_init_value=[], fields_description=fields_description)
         self.args = args
         self.config = config
 
         # We want to display the stat in the curse interface
         self.display_curse = True
 
         # Init stats
@@ -91,15 +88,15 @@
         self._thread = None
 
     def exit(self):
         """Overwrite the exit method to close threads."""
         if self._thread is not None:
             self._thread.stop()
         # Call the father class
-        super(PluginModel, self).exit()
+        super().exit()
 
     def get_key(self):
         """Return the key of the list."""
         return 'indice'
 
     @GlancesPluginModel._check_decorator
     @GlancesPluginModel._log_result_decorator
@@ -179,15 +176,15 @@
             return ret
 
         # Max size for the interface name
         if max_width:
             name_max_width = max_width - 7
         else:
             # No max_width defined, return an emptu curse message
-            logger.debug("No max_width defined for the {} plugin, it will not be displayed.".format(self.plugin_name))
+            logger.debug(f"No max_width defined for the {self.plugin_name} plugin, it will not be displayed.")
             return ret
 
         # Build the string message
         for p in self.stats:
             if 'host' in p:
                 if p['host'] is None:
                     status = 'None'
@@ -195,31 +192,31 @@
                     status = 'Scanning'
                 elif isinstance(p['status'], bool_type) and p['status'] is True:
                     status = 'Open'
                 elif p['status'] == 0:
                     status = 'Timeout'
                 else:
                     # Convert second to ms
-                    status = '{0:.0f}ms'.format(p['status'] * 1000.0)
+                    status = '{:.0f}ms'.format(p['status'] * 1000.0)
 
                 msg = '{:{width}}'.format(p['description'][0:name_max_width], width=name_max_width)
                 ret.append(self.curse_add_line(msg))
-                msg = '{:>9}'.format(status)
+                msg = f'{status:>9}'
                 ret.append(self.curse_add_line(msg, self.get_ports_alert(p, header=p['indice'] + '_rtt')))
                 ret.append(self.curse_new_line())
             elif 'url' in p:
                 msg = '{:{width}}'.format(p['description'][0:name_max_width], width=name_max_width)
                 ret.append(self.curse_add_line(msg))
                 if isinstance(p['status'], numbers.Number):
                     status = 'Code {}'.format(p['status'])
                 elif p['status'] is None:
                     status = 'Scanning'
                 else:
                     status = p['status']
-                msg = '{:>9}'.format(status)
+                msg = f'{status:>9}'
                 ret.append(self.curse_add_line(msg, self.get_web_alert(p, header=p['indice'] + '_rtt')))
                 ret.append(self.curse_new_line())
 
         # Delete the last empty line
         try:
             ret.pop()
         except IndexError:
@@ -233,16 +230,16 @@
     Specific thread for the port/web scanner.
 
     stats is a list of dict
     """
 
     def __init__(self, stats):
         """Init the class."""
-        logger.debug("ports plugin - Create thread for scan list {}".format(stats))
-        super(ThreadScanner, self).__init__()
+        logger.debug(f"ports plugin - Create thread for scan list {stats}")
+        super().__init__()
         # Event needed to stop properly the thread
         self._stopper = threading.Event()
         # The class return the stats as a list of dict
         self._stats = stats
         # Is part of Ports plugin
         self.plugin_name = "ports"
 
@@ -279,15 +276,15 @@
     @stats.setter
     def stats(self, value):
         """Stats setter."""
         self._stats = value
 
     def stop(self, timeout=None):
         """Stop the thread."""
-        logger.debug("ports plugin - Close thread for scan list {}".format(self._stats))
+        logger.debug(f"ports plugin - Close thread for scan list {self._stats}")
         self._stopper.set()
 
     def stopped(self):
         """Return True is the thread is stopped."""
         return self._stopper.is_set()
 
     def _web_scan(self, web):
@@ -309,24 +306,23 @@
             web['elapsed'] = req.elapsed.total_seconds()
         return web
 
     def _port_scan(self, port):
         """Scan the port structure (dict) and update the status key."""
         if int(port['port']) == 0:
             return self._port_scan_icmp(port)
-        else:
-            return self._port_scan_tcp(port)
+        return self._port_scan_tcp(port)
 
     def _resolv_name(self, hostname):
         """Convert hostname to IP address."""
         ip = hostname
         try:
             ip = socket.gethostbyname(hostname)
         except Exception as e:
-            logger.debug("{}: Cannot convert {} to IP address ({})".format(self.plugin_name, hostname, e))
+            logger.debug(f"{self.plugin_name}: Cannot convert {hostname} to IP address ({e})")
         return ip
 
     def _port_scan_icmp(self, port):
         """Scan the (ICMP) port structure (dict) and update the status key."""
         ret = None
 
         # Create the ping command
@@ -376,23 +372,23 @@
         ret = None
 
         # Create and configure the scanning socket
         try:
             socket.setdefaulttimeout(port['timeout'])
             _socket = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
         except Exception as e:
-            logger.debug("{}: Error while creating scanning socket ({})".format(self.plugin_name, e))
+            logger.debug(f"{self.plugin_name}: Error while creating scanning socket ({e})")
 
         # Scan port
         ip = self._resolv_name(port['host'])
         counter = Counter()
         try:
             ret = _socket.connect_ex((ip, int(port['port'])))
         except Exception as e:
-            logger.debug("{}: Error while scanning port {} ({})".format(self.plugin_name, port, e))
+            logger.debug(f"{self.plugin_name}: Error while scanning port {port} ({e})")
         else:
             if ret == 0:
                 port['status'] = counter.get()
             else:
                 port['status'] = False
         finally:
             _socket.close()
```

### Comparing `glances-4.0.4/glances/plugins/processcount/__init__.py` & `glances-4.0.5/glances/plugins/processcount/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,19 @@
-# -*- coding: utf-8 -*-
 #
 # This file is part of Glances.
 #
 # SPDX-FileCopyrightText: 2022 Nicolas Hennion <nicolas@nicolargo.com>
 #
 # SPDX-License-Identifier: LGPL-3.0-only
 #
 
 """Process count plugin."""
 
-from glances.processes import glances_processes, sort_for_human
 from glances.plugins.plugin.model import GlancesPluginModel
+from glances.processes import glances_processes, sort_for_human
 
 # Fields description
 # description: human readable description
 # short_name: shortname to use un UI
 # unit: unit type
 # rate: if True then compute and add *_gauge and *_rate_per_is fields
 # min_symbol: Auto unit should be used if value > than 1 'X' (K, M, G)...
@@ -54,15 +53,15 @@
     """Glances process count plugin.
 
     stats is a list
     """
 
     def __init__(self, args=None, config=None):
         """Init the plugin."""
-        super(PluginModel, self).__init__(
+        super().__init__(
             args=args, config=config, items_history_list=items_history_list, fields_description=fields_description
         )
 
         # We want to display the stat in the curse interface
         self.display_curse = True
 
         # Note: 'glances_processes' is already init in the glances_processes.py script
@@ -109,17 +108,17 @@
         if not self.stats:
             return ret
 
         # Display the filter (if it exists)
         if glances_processes.process_filter is not None:
             msg = 'Processes filter:'
             ret.append(self.curse_add_line(msg, "TITLE"))
-            msg = ' {} '.format(glances_processes.process_filter)
+            msg = f' {glances_processes.process_filter} '
             if glances_processes.process_filter_key is not None:
-                msg += 'on column {} '.format(glances_processes.process_filter_key)
+                msg += f'on column {glances_processes.process_filter_key} '
             ret.append(self.curse_add_line(msg, "FILTER"))
             msg = '(\'ENTER\' to edit, \'E\' to reset)'
             ret.append(self.curse_add_line(msg))
             ret.append(self.curse_new_line())
 
         # Build the string message
         # Header
@@ -140,26 +139,26 @@
             ret.append(self.curse_add_line(msg))
 
         if 'sleeping' in self.stats:
             other -= self.stats['sleeping']
             msg = ' {} slp,'.format(self.stats['sleeping'])
             ret.append(self.curse_add_line(msg))
 
-        msg = ' {} oth '.format(other)
+        msg = f' {other} oth '
         ret.append(self.curse_add_line(msg))
 
         # Display sort information
         msg = 'Programs' if self.args.programs else 'Threads'
         try:
             sort_human = sort_for_human[glances_processes.sort_key]
         except KeyError:
             sort_human = glances_processes.sort_key
         if glances_processes.auto_sort:
             msg += ' sorted automatically'
             ret.append(self.curse_add_line(msg))
-            msg = ' by {}'.format(sort_human)
+            msg = f' by {sort_human}'
         else:
-            msg += ' sorted by {}'.format(sort_human)
+            msg += f' sorted by {sort_human}'
         ret.append(self.curse_add_line(msg))
 
         # Return the message with decoration
         return ret
```

### Comparing `glances-4.0.4/glances/plugins/processlist/__init__.py` & `glances-4.0.5/glances/plugins/processlist/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,27 +1,26 @@
-# -*- coding: utf-8 -*-
 #
 # This file is part of Glances.
 #
 # SPDX-FileCopyrightText: 2024 Nicolas Hennion <nicolas@nicolargo.com>
 #
 # SPDX-License-Identifier: LGPL-3.0-only
 #
 
 """Process list plugin."""
 
-import os
 import copy
+import os
 
-from glances.logger import logger
 from glances.globals import WINDOWS, key_exist_value_not_none_not_v, replace_special_chars
-from glances.processes import glances_processes, sort_stats
+from glances.logger import logger
 from glances.outputs.glances_unicode import unicode_message
 from glances.plugins.core import PluginModel as CorePluginModel
 from glances.plugins.plugin.model import GlancesPluginModel
+from glances.processes import glances_processes, sort_stats
 
 # Fields description
 # description: human readable description
 # short_name: shortname to use un UI
 # unit: unit type
 # rate: if True then compute and add *_gauge and *_rate_per_is fields
 # min_symbol: Auto unit should be used if value > than 1 'X' (K, M, G)...
@@ -151,17 +150,15 @@
         'iow': '{:<4} ',
         'command': '{}',
         'name': '[{}]',
     }
 
     def __init__(self, args=None, config=None):
         """Init the plugin."""
-        super(PluginModel, self).__init__(
-            args=args, config=config, fields_description=fields_description, stats_init_value=[]
-        )
+        super().__init__(args=args, config=config, fields_description=fields_description, stats_init_value=[])
 
         # We want to display the stat in the curse interface
         self.display_curse = True
 
         # Trying to display proc time
         self.tag_proc_time = True
 
@@ -337,19 +334,19 @@
             # See: https://github.com/nicolargo/glances/issues/622
             # logger.debug("Cannot get TIME+ ({})".format(e))
             msg = self.layout_header['time'].format('?')
             ret = self.curse_add_line(msg, optional=True)
         else:
             hours, minutes, seconds = seconds_to_hms(user_system_time)
             if hours > 99:
-                msg = '{:<7}h'.format(hours)
+                msg = f'{hours:<7}h'
             elif 0 < hours < 100:
-                msg = '{}h{}:{}'.format(hours, minutes, seconds)
+                msg = f'{hours}h{minutes}:{seconds}'
             else:
-                msg = '{}:{}'.format(minutes, seconds)
+                msg = f'{minutes}:{seconds}'
             msg = self.layout_stat['time'].format(msg)
             if hours > 0:
                 ret = self.curse_add_line(msg, decoration='CPU_TIME', optional=True)
             else:
                 ret = self.curse_add_line(msg, optional=True)
         return ret
 
@@ -498,15 +495,15 @@
                     msg = ' ' + self.layout_stat['command'].format(arguments)
                     ret.append(self.curse_add_line(msg, splittable=True))
             else:
                 msg = self.layout_stat['name'].format(bare_process_name)
                 ret.append(self.curse_add_line(msg, decoration=process_decoration, splittable=True))
         except (TypeError, UnicodeEncodeError) as e:
             # Avoid crash after running fine for several hours #1335
-            logger.debug("Can not decode command line '{}' ({})".format(cmdline, e))
+            logger.debug(f"Can not decode command line '{cmdline}' ({e})")
             ret.append(self.curse_add_line('', splittable=True))
 
         return ret
 
     def is_selected_process(self, args):
         return (
             args.is_standalone
@@ -639,15 +636,15 @@
                 elif v == 3:
                     msg += k + 'IDLE'
                 else:
                     msg += k + str(v)
             #  value is a number which goes from 0 to 7.
             # The higher the value, the lower the I/O priority of the process.
             if hasattr(p['ionice'], 'value') and p['ionice'].value != 0:
-                msg += ' (value %s/7)' % str(p['ionice'].value)
+                msg += ' (value {}/7)'.format(str(p['ionice'].value))
             ret.append(self.curse_add_line(msg, splittable=True))
 
         # Second line is memory info
         ret.append(self.curse_new_line())
         ret.append(self.curse_add_line(' MEM Min/Max/Mean: '))
         msg = '{: >7.1f}{: >7.1f}{: >7.1f}%'.format(p['memory_min'], p['memory_max'], p['memory_mean'])
         ret.append(self.curse_add_line(msg, decoration='INFO'))
@@ -822,25 +819,24 @@
             ret.append(self.curse_add_line(msg, optional=True, additional=True))
             msg = self.layout_header['iow'].format('')
             ret.append(self.curse_add_line(msg, optional=True, additional=True))
         if mmm is None:
             msg = ' < {}'.format('current')
             ret.append(self.curse_add_line(msg, optional=True))
         else:
-            msg = ' < {}'.format(mmm)
+            msg = f' < {mmm}'
             ret.append(self.curse_add_line(msg, optional=True))
             msg = ' (\'M\' to reset)'
             ret.append(self.curse_add_line(msg, optional=True))
 
     def __mmm_deco(self, mmm):
         """Return the decoration string for the current mmm status."""
         if mmm is not None:
             return 'DEFAULT'
-        else:
-            return 'FILTER'
+        return 'FILTER'
 
     def __mmm_reset(self):
         """Reset the MMM stats."""
         self.mmm_min = {}
         self.mmm_max = {}
 
     def __sum_stats(self, key, sub_key=None, mmm=None):
@@ -898,10 +894,10 @@
         """Return the stats (dict) sorted by (sorted_by)."""
         return sort_stats(self.stats, sorted_by, reverse=glances_processes.sort_reverse)
 
     def __max_pid_size(self):
         """Return the maximum PID size in number of char."""
         if self.pid_max is not None:
             return len(str(self.pid_max))
-        else:
-            # By default return 5 (corresponding to 99999 PID number)
-            return 5
+
+        # By default return 5 (corresponding to 99999 PID number)
+        return 5
```

### Comparing `glances-4.0.4/glances/plugins/psutilversion/__init__.py` & `glances-4.0.5/glances/plugins/psutilversion/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 #
 # This file is part of Glances.
 #
 # SPDX-FileCopyrightText: 2022 Nicolas Hennion <nicolas@nicolargo.com>
 #
 # SPDX-License-Identifier: LGPL-3.0-only
 #
@@ -18,15 +17,15 @@
     """Get the Psutil version.
 
     stats is a string
     """
 
     def __init__(self, args=None, config=None):
         """Init the plugin."""
-        super(PluginModel, self).__init__(args=args, config=config)
+        super().__init__(args=args, config=config)
 
         self.reset()
 
     def reset(self):
         """Reset/init the stats."""
         self.stats = None
```

### Comparing `glances-4.0.4/glances/plugins/quicklook/__init__.py` & `glances-4.0.5/glances/plugins/quicklook/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,26 @@
-# -*- coding: utf-8 -*-
 #
 # This file is part of Glances.
 #
 # SPDX-FileCopyrightText: 2024 Nicolas Hennion <nicolas@nicolargo.com>
 #
 # SPDX-License-Identifier: LGPL-3.0-only
 #
 
 """Quicklook plugin."""
 
-from glances.logger import logger
+import psutil
+
 from glances.cpu_percent import cpu_percent
-from glances.plugins.load import get_load_average, get_nb_log_core, get_nb_phys_core
+from glances.logger import logger
 from glances.outputs.glances_bars import Bar
 from glances.outputs.glances_sparklines import Sparkline
+from glances.plugins.load import get_load_average, get_nb_log_core, get_nb_phys_core
 from glances.plugins.plugin.model import GlancesPluginModel
 
-import psutil
-
 # Fields description
 # description: human readable description
 # short_name: shortname to use un UI
 # unit: unit type
 # rate: is it a rate ? If yes, // by time_since_update when displayed,
 # min_symbol: Auto unit should be used if value > than 1 'X' (K, M, G)...
 fields_description = {
@@ -80,28 +79,28 @@
     """
 
     AVAILABLE_STATS_LIST = ['cpu', 'mem', 'swap', 'load']
     DEFAULT_STATS_LIST = ['cpu', 'mem', 'load']
 
     def __init__(self, args=None, config=None):
         """Init the quicklook plugin."""
-        super(PluginModel, self).__init__(
+        super().__init__(
             args=args, config=config, items_history_list=items_history_list, fields_description=fields_description
         )
 
         # We want to display the stat in the curse interface
         self.display_curse = True
 
         # Manage the maximum number of CPU to display (related to enhancement request #2734)
         self.max_cpu_display = config.get_int_value('percpu', 'max_cpu_display', 4) if config else 4
 
         # Define the stats list
         self.stats_list = self.get_conf_value('list', default=self.DEFAULT_STATS_LIST)
         if not set(self.stats_list).issubset(self.AVAILABLE_STATS_LIST):
-            logger.warning('Quicklook plugin: Invalid stats list: {}'.format(self.stats_list))
+            logger.warning(f'Quicklook plugin: Invalid stats list: {self.stats_list}')
             self.stats_list = self.AVAILABLE_STATS_LIST
 
     @GlancesPluginModel._check_decorator
     @GlancesPluginModel._log_result_decorator
     def update(self):
         """Update quicklook stats using the input method."""
         # Init new stats
@@ -148,15 +147,15 @@
         self.stats = stats
 
         return self.stats
 
     def update_views(self):
         """Update stats views."""
         # Call the father's method
-        super(PluginModel, self).update_views()
+        super().update_views()
 
         # Alert for CPU, MEM and SWAP
         for key in self.stats_list:
             if key in self.stats:
                 self.views[key]['decoration'] = self.get_alert(self.stats[key], header=key)
 
         # Alert for LOAD
@@ -172,19 +171,19 @@
 
         # Only process if stats exist...
         if not self.stats or self.is_disabled():
             return ret
 
         if not max_width:
             # No max_width defined, return an empty message
-            logger.debug("No max_width defined for the {} plugin, it will not be displayed.".format(self.plugin_name))
+            logger.debug(f"No max_width defined for the {self.plugin_name} plugin, it will not be displayed.")
             return ret
 
         # Define the data: Bar (default behavior) or Sparkline
-        data = dict()
+        data = {}
         for key in self.stats_list:
             if self.args.sparkline and self.history_enable() and not self.args.client:
                 data[key] = Sparkline(max_width)
             else:
                 # Fallback to bar if Sparkline module is not installed
                 data[key] = Bar(max_width, bar_char=self.get_conf_value('bar_char', default=['|'])[0])
 
@@ -217,15 +216,15 @@
                     # Sparkline display an history
                     data[key].percents = [i[1] for i in self.get_raw_history(item=key, nb=data[key].size)]
                     # A simple padding in order to align metrics to the right
                     data[key].percents += [None] * (data[key].size - len(data[key].percents))
                 else:
                     # Bar only the last value
                     data[key].percent = self.stats[key]
-                msg = '{:4} '.format(key.upper())
+                msg = f'{key.upper():4} '
                 ret.extend(self._msg_create_line(msg, data[key], key))
                 ret.append(self.curse_new_line())
 
         # Remove the last new line
         ret.pop()
 
         # Return the message with decoration
@@ -254,17 +253,17 @@
                 data[key].percents = [i[1][cpu_id]['total'] for i in raw_cpu]
                 # A simple padding in order to align metrics to the right
                 data[key].percents += [None] * (data[key].size - len(data[key].percents))
             else:
                 # Bar will only display the last value
                 data[key].percent = cpu['total']
             if cpu_id < 10:
-                msg = '{:3}{} '.format(key.upper(), cpu_id)
+                msg = f'{key.upper():3}{cpu_id} '
             else:
-                msg = '{:4} '.format(cpu_id)
+                msg = f'{cpu_id:4} '
             ret.extend(self._msg_create_line(msg, data[key], key))
             ret.append(self.curse_new_line())
 
         # Add a new line with sum of all others CPU
         if len(self.stats['percpu']) > self.max_cpu_display:
             if type(data[key]).__name__ == 'Sparkline':
                 sum_other = Sparkline(max_width)
@@ -278,15 +277,15 @@
                 sum_other.percents += [None] * (sum_other.size - len(sum_other.percents))
             else:
                 # Bar will only display the last value
                 sum_other = Bar(max_width, bar_char=self.get_conf_value('bar_char', default=['|'])[0])
                 sum_other.percent = sum([i['total'] for i in percpu_list[self.max_cpu_display :]]) / len(
                     percpu_list[self.max_cpu_display :]
                 )
-            msg = msg = '{:3}* '.format(key.upper())
+            msg = msg = f'{key.upper():3}* '
             ret.extend(self._msg_create_line(msg, sum_other, key))
             ret.append(self.curse_new_line())
 
         return ret
 
     def _msg_create_line(self, msg, data, key):
         """Create a new line to the Quick view."""
```

### Comparing `glances-4.0.4/glances/plugins/raid/__init__.py` & `glances-4.0.5/glances/plugins/raid/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 #
 # This file is part of Glances.
 #
 # SPDX-FileCopyrightText: 2022 Nicolas Hennion <nicolas@nicolargo.com>
 #
 # SPDX-License-Identifier: LGPL-3.0-only
 #
@@ -14,28 +13,28 @@
 from glances.plugins.plugin.model import GlancesPluginModel
 
 # Import plugin specific dependency
 try:
     from pymdstat import MdStat
 except ImportError as e:
     import_error_tag = True
-    logger.warning("Missing Python Lib ({}), Raid plugin is disabled".format(e))
+    logger.warning(f"Missing Python Lib ({e}), Raid plugin is disabled")
 else:
     import_error_tag = False
 
 
 class PluginModel(GlancesPluginModel):
     """Glances RAID plugin.
 
     stats is a dict (see pymdstat documentation)
     """
 
     def __init__(self, args=None, config=None):
         """Init the plugin."""
-        super(PluginModel, self).__init__(args=args, config=config)
+        super().__init__(args=args, config=config)
 
         # We want to display the stat in the curse interface
         self.display_curse = True
 
     @GlancesPluginModel._check_decorator
     @GlancesPluginModel._log_result_decorator
     def update(self):
@@ -50,15 +49,15 @@
             # Update stats using the PyMDstat lib (https://github.com/nicolargo/pymdstat)
             try:
                 mds = MdStat()
                 # Just for test: uncomment the following line to use a local file
                 # mds = MdStat(path='/home/nicolargo/dev/pymdstat/tests/mdstat.10')
                 stats = mds.get_stats()['arrays']
             except Exception as e:
-                logger.debug("Can not grab RAID stats (%s)" % e)
+                logger.debug(f"Can not grab RAID stats ({e})")
                 return self.stats
 
         elif self.input_method == 'snmp':
             # Update stats using SNMP
             # No standard way for the moment...
             pass
 
@@ -77,15 +76,15 @@
             return ret
 
         # Max size for the interface name
         if max_width:
             name_max_width = max_width - 12
         else:
             # No max_width defined, return an emptu curse message
-            logger.debug("No max_width defined for the {} plugin, it will not be displayed.".format(self.plugin_name))
+            logger.debug(f"No max_width defined for the {self.plugin_name} plugin, it will not be displayed.")
             return ret
 
         # Header
         msg = '{:{width}}'.format('RAID disks', width=name_max_width)
         ret.append(self.curse_add_line(msg, "TITLE"))
         msg = '{:>7}'.format('Used')
         ret.append(self.curse_add_line(msg))
@@ -104,15 +103,15 @@
                 self.stats[array]['used'],
                 self.stats[array]['available'],
                 self.stats[array]['type'],
             )
             # Data: RAID type name | disk used | disk available
             array_type = self.stats[array]['type'].upper() if self.stats[array]['type'] is not None else 'UNKNOWN'
             # Build the full name = array type + array name
-            full_name = '{} {}'.format(array_type, array)
+            full_name = f'{array_type} {array}'
             msg = '{:{width}}'.format(full_name, width=name_max_width)
             ret.append(self.curse_add_line(msg))
             if self.stats[array]['type'] == 'raid0' and self.stats[array]['status'] == 'active':
                 msg = '{:>7}'.format(len(self.stats[array]['components']))
                 ret.append(self.curse_add_line(msg, status))
                 msg = '{:>7}'.format('-')
                 ret.append(self.curse_add_line(msg, status))
@@ -130,15 +129,15 @@
                     if i == len(components) - 1:
                         tree_char = '└─'
                     else:
                         tree_char = '├─'
                     ret.append(self.curse_new_line())
                     msg = '   {} disk {}: '.format(tree_char, self.stats[array]['components'][component])
                     ret.append(self.curse_add_line(msg))
-                    msg = '{}'.format(component)
+                    msg = f'{component}'
                     ret.append(self.curse_add_line(msg))
             if self.stats[array]['type'] != 'raid0' and (self.stats[array]['used'] < self.stats[array]['available']):
                 # Display current array configuration
                 ret.append(self.curse_new_line())
                 msg = '└─ Degraded mode'
                 ret.append(self.curse_add_line(msg, status))
                 if len(self.stats[array]['config']) < 17:
@@ -157,10 +156,10 @@
         """
         if type == 'raid0':
             return 'OK'
         if status == 'inactive':
             return 'CRITICAL'
         if used is None or available is None:
             return 'DEFAULT'
-        elif used < available:
+        if used < available:
             return 'WARNING'
         return 'OK'
```

### Comparing `glances-4.0.4/glances/plugins/sensors/__init__.py` & `glances-4.0.5/glances/plugins/sensors/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,34 +1,35 @@
-# -*- coding: utf-8 -*-
 #
 # This file is part of Glances.
 #
 # SPDX-FileCopyrightText: 2024 Nicolas Hennion <nicolas@nicolargo.com>
 #
 # SPDX-License-Identifier: LGPL-3.0-only
 #
 
 """Sensors plugin."""
-from enum import Enum
+
+import warnings
 from concurrent.futures import ThreadPoolExecutor
-from typing import List, Dict, Literal, Any
+from enum import Enum
+from typing import Any, Dict, List, Literal
 
 import psutil
-import warnings
 
-from glances.logger import logger
 from glances.globals import to_fahrenheit
-from glances.timer import Counter
-from glances.plugins.sensors.sensor.glances_batpercent import PluginModel as BatPercentPluginModel
-from glances.plugins.sensors.sensor.glances_hddtemp import PluginModel as HddTempPluginModel
+from glances.logger import logger
 from glances.outputs.glances_unicode import unicode_message
 from glances.plugins.plugin.model import GlancesPluginModel
+from glances.plugins.sensors.sensor.glances_batpercent import PluginModel as BatPercentPluginModel
+from glances.plugins.sensors.sensor.glances_hddtemp import PluginModel as HddTempPluginModel
+from glances.timer import Counter
 
 
 class SensorType(str, Enum):
+    # Switch to `enum.StrEnum` when we only support py311+
     CPU_TEMP = 'temperature_core'
     FAN_SPEED = 'fan_speed'
     HDD_TEMP = 'temperature_hdd'
     BATTERY = 'battery'
 
 
 CPU_TEMP_UNIT = 'C'
@@ -78,37 +79,46 @@
     The stats list includes both sensors and hard disks stats, if any.
     The sensors are already grouped by chip type and then sorted by label.
     The hard disks are already sorted by label.
     """
 
     def __init__(self, args=None, config=None):
         """Init the plugin."""
-        super(PluginModel, self).__init__(
-            args=args, config=config, stats_init_value=[], fields_description=fields_description
-        )
+        super().__init__(args=args, config=config, stats_init_value=[], fields_description=fields_description)
         start_duration = Counter()
 
         # Init the sensor class
         start_duration.reset()
         glances_grab_sensors_cpu_temp = GlancesGrabSensors(SensorType.CPU_TEMP)
-        logger.debug("CPU Temp sensor plugin init duration: {} seconds".format(start_duration.get()))
+        logger.debug(f"CPU Temp sensor plugin init duration: {start_duration.get()} seconds")
 
         start_duration.reset()
         glances_grab_sensors_fan_speed = GlancesGrabSensors(SensorType.FAN_SPEED)
-        logger.debug("Fan speed sensor plugin init duration: {} seconds".format(start_duration.get()))
+        logger.debug(f"Fan speed sensor plugin init duration: {start_duration.get()} seconds")
 
         # Instance for the HDDTemp Plugin in order to display the hard disks temperatures
         start_duration.reset()
         hddtemp_plugin = HddTempPluginModel(args=args, config=config)
-        logger.debug("HDDTemp sensor plugin init duration: {} seconds".format(start_duration.get()))
+        logger.debug(f"HDDTemp sensor plugin init duration: {start_duration.get()} seconds")
 
         # Instance for the BatPercent in order to display the batteries capacities
         start_duration.reset()
         batpercent_plugin = BatPercentPluginModel(args=args, config=config)
-        logger.debug("Battery sensor plugin init duration: {} seconds".format(start_duration.get()))
+        logger.debug(f"Battery sensor plugin init duration: {start_duration.get()} seconds")
+
+        self.sensors_grab_map: Dict[SensorType, Any] = {}
+
+        if glances_grab_sensors_cpu_temp.init:
+            self.sensors_grab_map[SensorType.CPU_TEMP] = glances_grab_sensors_cpu_temp
+
+        if glances_grab_sensors_fan_speed.init:
+            self.sensors_grab_map[SensorType.FAN_SPEED] = glances_grab_sensors_fan_speed
+
+        self.sensors_grab_map[SensorType.HDD_TEMP] = hddtemp_plugin
+        self.sensors_grab_map[SensorType.BATTERY] = batpercent_plugin
 
         self.sensors_grab_map: Dict[SensorType, Any] = {}
 
         if glances_grab_sensors_cpu_temp.init:
             self.sensors_grab_map[SensorType.CPU_TEMP] = glances_grab_sensors_cpu_temp
 
         if glances_grab_sensors_fan_speed.init:
@@ -148,16 +158,15 @@
             # Set alias for sensors
             stat["label"] = self.__get_alias(stat)
             # Add the stat to the stats_transformed list
             stats_transformed.append(stat)
         # Remove duplicates thanks to https://stackoverflow.com/a/9427216/1919431
         stats_transformed = [dict(t) for t in {tuple(d.items()) for d in stats_transformed}]
         # Sort by label
-        stats_transformed = sorted(stats_transformed, key=lambda d: d['label'])
-        return stats_transformed
+        return sorted(stats_transformed, key=lambda d: d['label'])
 
     @GlancesPluginModel._check_decorator
     @GlancesPluginModel._log_result_decorator
     def update(self):
         """Update sensors stats using the input method."""
         # Init new stats
         stats = self.get_init_value()
@@ -186,20 +195,19 @@
         return self.stats
 
     def __get_alias(self, stats):
         """Return the alias of the sensor."""
         # Get the alias for each stat
         if self.has_alias(stats["label"].lower()):
             return self.has_alias(stats["label"].lower())
-        elif self.has_alias("{}_{}".format(stats["label"], stats["type"]).lower()):
+        if self.has_alias("{}_{}".format(stats["label"], stats["type"]).lower()):
             return self.has_alias("{}_{}".format(stats["label"], stats["type"]).lower())
-        else:
-            return stats["label"]
+        return stats["label"]
 
-    def __set_type(self, stats, sensor_type):
+    def __set_type(self, stats: List[Dict[str, Any]], sensor_type: SensorType) -> List[Dict[str, Any]]:
         """Set the plugin type.
 
         4 types of stats is possible in the sensors plugin:
         - Core temperature: SENSOR_TEMP_TYPE
         - Fan speed: SENSOR_FAN_TYPE
         - HDD temperature: 'temperature_hdd'
         - Battery capacity: 'battery'
@@ -211,15 +219,15 @@
             i.update({'key': self.get_key()})
 
         return stats
 
     def update_views(self):
         """Update stats views."""
         # Call the father's method
-        super(PluginModel, self).update_views()
+        super().update_views()
 
         # Add specifics information
         # Alert
         for i in self.stats:
             if not i['value']:
                 continue
             # Alert processing
@@ -249,17 +257,17 @@
 
     def battery_trend(self, stats):
         """Return the trend character for the battery"""
         if 'status' not in stats:
             return ''
         if stats['status'].startswith('Charg'):
             return unicode_message('ARROW_UP')
-        elif stats['status'].startswith('Discharg'):
+        if stats['status'].startswith('Discharg'):
             return unicode_message('ARROW_DOWN')
-        elif stats['status'].startswith('Full'):
+        if stats['status'].startswith('Full'):
             return unicode_message('CHECK')
         return ''
 
     def msg_curse(self, args=None, max_width=None):
         """Return the dict to display in the curse interface."""
         # Init the return message
         ret = []
@@ -269,15 +277,15 @@
             return ret
 
         # Max size for the interface name
         if max_width:
             name_max_width = max_width - 12
         else:
             # No max_width defined, return an emptu curse message
-            logger.debug("No max_width defined for the {} plugin, it will not be displayed.".format(self.plugin_name))
+            logger.debug(f"No max_width defined for the {self.plugin_name} plugin, it will not be displayed.")
             return ret
 
         # Header
         msg = '{:{width}}'.format('SENSORS', width=name_max_width)
         ret.append(self.curse_add_line(msg, "TITLE"))
 
         # Stats
@@ -300,28 +308,28 @@
                     value = to_fahrenheit(i['value'])
                     unit = 'F'
                 else:
                     trend = self.battery_trend(i)
                     value = i['value']
                     unit = i['unit']
                 try:
-                    msg = '{:.0f}{}{}'.format(value, unit, trend)
-                    msg = '{:>14}'.format(msg)
+                    msg = f'{value:.0f}{unit}{trend}'
+                    msg = f'{msg:>14}'
                     ret.append(
                         self.curse_add_line(
                             msg, self.get_views(item=i[self.get_key()], key='value', option='decoration')
                         )
                     )
                 except (TypeError, ValueError):
                     pass
 
         return ret
 
 
-class GlancesGrabSensors(object):
+class GlancesGrabSensors:
     """Get sensors stats."""
 
     def __init__(self, sensor_type: Literal[SensorType.FAN_SPEED, SensorType.CPU_TEMP]):
         """Init sensors stats."""
         self.sensor_type = sensor_type
         self.sensor_unit = CPU_TEMP_UNIT if self.sensor_type == SensorType.CPU_TEMP else FAN_SPEED_UNIT
 
@@ -365,16 +373,15 @@
                 elif feature.label in [i['label'] for i in ret]:
                     sensors_current['label'] = feature.label + ' ' + str(label_index)
                     label_index += 1
                 else:
                     sensors_current['label'] = feature.label
                 # Sensors value, limit and unit
                 sensors_current['unit'] = self.sensor_unit
-                sensors_current['value'] = int(
-                    getattr(feature, 'current', 0) if getattr(feature, 'current', 0) else 0)
+                sensors_current['value'] = int(getattr(feature, 'current', 0) if getattr(feature, 'current', 0) else 0)
                 system_warning = getattr(feature, 'high', None)
                 system_critical = getattr(feature, 'critical', None)
                 sensors_current['warning'] = int(system_warning) if system_warning is not None else None
                 sensors_current['critical'] = int(system_critical) if system_critical is not None else None
                 # Add sensor to the list
                 ret.append(sensors_current)
         return ret
```

### Comparing `glances-4.0.4/glances/plugins/sensors/sensor/glances_batpercent.py` & `glances-4.0.5/glances/plugins/sensors/sensor/glances_batpercent.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,57 +1,58 @@
-# -*- coding: utf-8 -*-
 #
 # This file is part of Glances.
 #
 # SPDX-FileCopyrightText: 2022 Nicolas Hennion <nicolas@nicolargo.com>
 #
 # SPDX-License-Identifier: LGPL-3.0-only
 #
 
 """Battery plugin."""
 
 import psutil
 
+from glances.globals import LINUX
 from glances.logger import logger
 from glances.plugins.plugin.model import GlancesPluginModel
 
 # Batinfo library (optional; Linux-only)
-batinfo_tag = True
-try:
-    import batinfo
-except ImportError:
-    logger.debug("batinfo library not found. Fallback to psutil.")
+if LINUX:
+    batinfo_tag = True
+    try:
+        import batinfo
+    except ImportError:
+        logger.debug("batinfo library not found. Fallback to psutil.")
+        batinfo_tag = False
+else:
     batinfo_tag = False
 
-# Availability:
-# Linux, Windows, FreeBSD (psutil>=5.1.0)
-# macOS (psutil>=5.4.2)
+# PsUtil Sensors_battery available on Linux, Windows, FreeBSD, macOS
 psutil_tag = True
 try:
     psutil.sensors_battery()
 except Exception as e:
-    logger.error("Cannot grab battery status {}.".format(e))
+    logger.error(f"Cannot grab battery status {e}.")
     psutil_tag = False
 
 
 class PluginModel(GlancesPluginModel):
     """Glances battery capacity plugin.
 
     stats is a list
     """
 
     def __init__(self, args=None, config=None):
         """Init the plugin."""
-        super(PluginModel, self).__init__(args=args, config=config, stats_init_value=[])
+        super().__init__(args=args, config=config, stats_init_value=[])
 
         # Init the sensor class
         try:
             self.glances_grab_bat = GlancesGrabBat()
         except Exception as e:
-            logger.error("Can not init battery class ({})".format(e))
+            logger.error(f"Can not init battery class ({e})")
             global batinfo_tag
             global psutil_tag
             batinfo_tag = False
             psutil_tag = False
 
         # We do not want to display the stat in a dedicated area
         # The HDD temp is displayed within the sensors plugin
@@ -76,15 +77,15 @@
 
         # Update the stats
         self.stats = stats
 
         return self.stats
 
 
-class GlancesGrabBat(object):
+class GlancesGrabBat:
     """Get batteries stats using the batinfo library."""
 
     def __init__(self):
         """Init batteries stats."""
         self.bat_list = []
 
         if batinfo_tag:
```

### Comparing `glances-4.0.4/glances/plugins/sensors/sensor/glances_hddtemp.py` & `glances-4.0.5/glances/plugins/sensors/sensor/glances_hddtemp.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 #
 # This file is part of Glances.
 #
 # SPDX-FileCopyrightText: 2022 Nicolas Hennion <nicolas@nicolargo.com>
 #
 # SPDX-License-Identifier: LGPL-3.0-only
 #
@@ -21,15 +20,15 @@
     """Glances HDD temperature sensors plugin.
 
     stats is a list
     """
 
     def __init__(self, args=None, config=None):
         """Init the plugin."""
-        super(PluginModel, self).__init__(args=args, config=config, stats_init_value=[])
+        super().__init__(args=args, config=config, stats_init_value=[])
 
         # Init the sensor class
         hddtemp_host = self.get_conf_value("host", default=["127.0.0.1"])[0]
         hddtemp_port = int(self.get_conf_value("port", default="7634"))
         self.hddtemp = GlancesGrabHDDTemp(args=args, host=hddtemp_host, port=hddtemp_port)
 
         # We do not want to display the stat in a dedicated area
@@ -54,15 +53,15 @@
 
         # Update the stats
         self.stats = stats
 
         return self.stats
 
 
-class GlancesGrabHDDTemp(object):
+class GlancesGrabHDDTemp:
     """Get hddtemp stats using a socket connection."""
 
     def __init__(self, host='127.0.0.1', port=7634, args=None):
         """Init hddtemp stats."""
         self.args = args
         self.host = host
         self.port = port
@@ -129,23 +128,23 @@
             data = b''
             while True:
                 received = sck.recv(4096)
                 if not received:
                     break
                 data += received
         except Exception as e:
-            logger.debug("Cannot connect to an HDDtemp server ({}:{} => {})".format(self.host, self.port, e))
+            logger.debug(f"Cannot connect to an HDDtemp server ({self.host}:{self.port} => {e})")
             logger.debug("Disable the HDDtemp module. Use the --disable-hddtemp to hide the previous message.")
             if self.args is not None:
                 self.args.disable_hddtemp = True
             data = ""
         finally:
             sck.close()
             if data != "":
-                logger.debug("Received data from the HDDtemp server: {}".format(data))
+                logger.debug(f"Received data from the HDDtemp server: {data}")
 
         return data
 
     def get(self):
         """Get HDDs list."""
         self.__update__()
         return self.hddtemp_list
```

### Comparing `glances-4.0.4/glances/plugins/smart/__init__.py` & `glances-4.0.5/glances/plugins/smart/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 #
 # This file is part of Glances.
 #
 # Copyright (C) 2018 Tim Nibert <docz2a@gmail.com>
 #
 # SPDX-License-Identifier: LGPL-3.0-only
 #
@@ -30,25 +29,25 @@
 
 So, here is what we are going to do:
 Check for admin access.  If no admin access, disable SMART plugin.
 
 If smartmontools is not installed, we should catch the error upstream in plugin initialization.
 """
 
-from glances.plugins.plugin.model import GlancesPluginModel
+from glances.globals import is_admin
 from glances.logger import logger
 from glances.main import disable
-from glances.globals import is_admin
+from glances.plugins.plugin.model import GlancesPluginModel
 
 # Import plugin specific dependency
 try:
     from pySMART import DeviceList
 except ImportError as e:
     import_error_tag = True
-    logger.warning("Missing Python Lib ({}), HDD Smart plugin is disabled".format(e))
+    logger.warning(f"Missing Python Lib ({e}), HDD Smart plugin is disabled")
 else:
     import_error_tag = False
 
 
 def convert_attribute_to_dict(attr):
     return {
         'name': attr.name,
@@ -85,38 +84,38 @@
     """
     stats = []
     # get all devices
     try:
         devlist = DeviceList()
     except TypeError as e:
         # Catch error  (see #1806)
-        logger.debug('Smart plugin error - Can not grab device list ({})'.format(e))
+        logger.debug(f'Smart plugin error - Can not grab device list ({e})')
         global import_error_tag
         import_error_tag = True
         return stats
 
     for dev in devlist.devices:
         stats.append(
             {
-                'DeviceName': '{} {}'.format(dev.name, dev.model),
+                'DeviceName': f'{dev.name} {dev.model}',
             }
         )
         for attribute in dev.attributes:
             if attribute is None:
                 pass
             else:
                 attrib_dict = convert_attribute_to_dict(attribute)
 
                 # we will use the attribute number as the key
                 num = attrib_dict.pop('num', None)
                 try:
                     assert num is not None
                 except Exception as e:
                     # we should never get here, but if we do, continue to next iteration and skip this attribute
-                    logger.debug('Smart plugin error - Skip the attribute {} ({})'.format(attribute, e))
+                    logger.debug(f'Smart plugin error - Skip the attribute {attribute} ({e})')
                     continue
 
                 stats[-1][num] = attrib_dict
     return stats
 
 
 class PluginModel(GlancesPluginModel):
@@ -125,15 +124,15 @@
     def __init__(self, args=None, config=None, stats_init_value=[]):
         """Init the plugin."""
         # check if user is admin
         if not is_admin() and args:
             disable(args, "smart")
             logger.debug("Current user is not admin, HDD SMART plugin disabled.")
 
-        super(PluginModel, self).__init__(args=args, config=config)
+        super().__init__(args=args, config=config)
 
         # We want to display the stat in the curse interface
         self.display_curse = True
 
     @GlancesPluginModel._check_decorator
     @GlancesPluginModel._log_result_decorator
     def update(self):
@@ -168,15 +167,15 @@
             return ret
 
         # Max size for the interface name
         if max_width:
             name_max_width = max_width - 6
         else:
             # No max_width defined, return an emptu curse message
-            logger.debug("No max_width defined for the {} plugin, it will not be displayed.".format(self.plugin_name))
+            logger.debug(f"No max_width defined for the {self.plugin_name} plugin, it will not be displayed.")
             return ret
 
         # Header
         msg = '{:{width}}'.format('SMART disks', width=name_max_width)
         ret.append(self.curse_add_line(msg, "TITLE"))
         # Data
         for device_stat in self.stats:
```

### Comparing `glances-4.0.4/glances/plugins/system/__init__.py` & `glances-4.0.5/glances/plugins/system/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,25 +1,24 @@
-# -*- coding: utf-8 -*-
 #
 # This file is part of Glances.
 #
 # SPDX-FileCopyrightText: 2022 Nicolas Hennion <nicolas@nicolargo.com>
 #
 # SPDX-License-Identifier: LGPL-3.0-only
 #
 
 """System plugin."""
 
+import builtins
 import os
 import platform
 import re
-from io import open
 
-from glances.logger import logger
 from glances.globals import iteritems
+from glances.logger import logger
 from glances.plugins.plugin.model import GlancesPluginModel
 
 # {
 #   "os_name": "Linux",
 #   "hostname": "XPS13-9333",
 #   "platform": "64bit",
 #   "linux_distro": "Ubuntu 22.04",
@@ -88,20 +87,20 @@
     It takes the name from the 'NAME' field and the version from 'VERSION_ID'.
     An empty string is returned if the above values cannot be determined.
     """
     pretty_name = ''
     ashtray = {}
     keys = ['NAME', 'VERSION_ID']
     try:
-        with open(os.path.join('/etc', 'os-release')) as f:
+        with builtins.open(os.path.join('/etc', 'os-release')) as f:
             for line in f:
                 for key in keys:
                     if line.startswith(key):
                         ashtray[key] = re.sub(r'^"|"$', '', line.strip().split('=')[1])
-    except (OSError, IOError):
+    except OSError:
         return pretty_name
 
     if ashtray:
         if 'NAME' in ashtray:
             pretty_name = ashtray['NAME']
         if 'VERSION_ID' in ashtray:
             pretty_name += ' {}'.format(ashtray['VERSION_ID'])
@@ -113,15 +112,15 @@
     """Glances' host/system plugin.
 
     stats is a dict
     """
 
     def __init__(self, args=None, config=None):
         """Init the plugin."""
-        super(PluginModel, self).__init__(args=args, config=config, fields_description=fields_description)
+        super().__init__(args=args, config=config, fields_description=fields_description)
 
         # We want to display the stat in the curse interface
         self.display_curse = True
 
         # Set default rate to 60 seconds
         if self.get_refresh():
             self.set_refresh(60)
```

### Comparing `glances-4.0.4/glances/plugins/uptime/__init__.py` & `glances-4.0.5/glances/plugins/uptime/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,37 +1,36 @@
-# -*- coding: utf-8 -*-
 #
 # This file is part of Glances.
 #
 # SPDX-FileCopyrightText: 2022 Nicolas Hennion <nicolas@nicolargo.com>
 #
 # SPDX-License-Identifier: LGPL-3.0-only
 #
 
 """Uptime plugin."""
 
 from datetime import datetime, timedelta
 
-from glances.plugins.plugin.model import GlancesPluginModel
-
 import psutil
 
+from glances.plugins.plugin.model import GlancesPluginModel
+
 # SNMP OID
 snmp_oid = {'_uptime': '1.3.6.1.2.1.1.3.0'}
 
 
 class PluginModel(GlancesPluginModel):
     """Glances uptime plugin.
 
     stats is date (string)
     """
 
     def __init__(self, args=None, config=None):
         """Init the plugin."""
-        super(PluginModel, self).__init__(args=args, config=config)
+        super().__init__(args=args, config=config)
 
         # We want to display the stat in the curse interface
         self.display_curse = True
 
         # Set the message position
         self.align = 'right'
 
@@ -79,10 +78,8 @@
         # Init the return message
         ret = []
 
         # Only process if stats exist and plugin not disabled
         if not self.stats or self.is_disabled():
             return ret
 
-        ret = [self.curse_add_line('Uptime: {}'.format(self.stats))]
-
-        return ret
+        return [self.curse_add_line(f'Uptime: {self.stats}')]
```

### Comparing `glances-4.0.4/glances/plugins/version/__init__.py` & `glances-4.0.5/glances/plugins/version/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 #
 # This file is part of Glances.
 #
 # SPDX-FileCopyrightText: 2024 Nicolas Hennion <nicolas@nicolargo.com>
 #
 # SPDX-License-Identifier: LGPL-3.0-only
 #
@@ -19,15 +18,15 @@
     """Get the Glances versions.
 
     stats is a string
     """
 
     def __init__(self, args=None, config=None):
         """Init the plugin."""
-        super(PluginModel, self).__init__(args=args, config=config)
+        super().__init__(args=args, config=config)
 
         self.reset()
 
     def reset(self):
         """Reset/init the stats."""
         self.stats = None
```

### Comparing `glances-4.0.4/glances/plugins/wifi/__init__.py` & `glances-4.0.5/glances/plugins/wifi/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 #
 # This file is part of Glances.
 #
 # SPDX-FileCopyrightText: 2024 Nicolas Hennion <nicolas@nicolargo.com>
 #
 # SPDX-License-Identifier: LGPL-3.0-only
 #
@@ -15,25 +14,25 @@
 Inter-| sta-|   Quality        |   Discarded packets               | Missed | WE
  face | tus | link level noise |  nwid  crypt   frag  retry   misc | beacon | 22
 wlp2s0: 0000   51.  -59.  -256        0      0      0      0   5881        0
 """
 
 import operator
 
-from glances.globals import nativestr, file_exists
-from glances.plugins.plugin.model import GlancesPluginModel
+from glances.globals import file_exists, nativestr
 from glances.logger import logger
+from glances.plugins.plugin.model import GlancesPluginModel
 
 # Backup solution is to use the /proc/net/wireless file
 # but it only give signal information about the current hotspot
 WIRELESS_FILE = '/proc/net/wireless'
 wireless_file_exists = file_exists(WIRELESS_FILE)
 
 if not wireless_file_exists:
-    logger.debug("Wifi plugin is disabled (no %s file found)" % (WIRELESS_FILE))
+    logger.debug(f"Wifi plugin is disabled (no {WIRELESS_FILE} file found)")
 
 # Fields description
 # description: human readable description
 # short_name: shortname to use un UI
 # unit: unit type
 # rate: if True then compute and add *_gauge and *_rate_per_is fields
 # min_symbol: Auto unit should be used if value > than 1 'X' (K, M, G)...
@@ -54,28 +53,28 @@
     """Glances Wifi plugin.
 
     Get stats of the current Wifi hotspots.
     """
 
     def __init__(self, args=None, config=None):
         """Init the plugin."""
-        super(PluginModel, self).__init__(args=args, config=config, stats_init_value=[])
+        super().__init__(args=args, config=config, stats_init_value=[])
 
         # We want to display the stat in the curse interface
         self.display_curse = True
 
         # Global Thread running all the scans
         self._thread = None
 
     def exit(self):
         """Overwrite the exit method to close threads."""
         if self._thread is not None:
             self._thread.stop()
         # Call the father class
-        super(PluginModel, self).exit()
+        super().exit()
 
     def get_key(self):
         """Return the key of the list.
 
         :returns: string -- SSID is the dict key
         """
         return 'ssid'
@@ -94,15 +93,15 @@
 
         # Exist if we can not grab the stats
         if not wireless_file_exists:
             return stats
 
         if self.input_method == 'local' and wireless_file_exists:
             # As a backup solution, use the /proc/net/wireless file
-            with open(WIRELESS_FILE, 'r') as f:
+            with open(WIRELESS_FILE) as f:
                 # The first two lines are header
                 f.readline()
                 f.readline()
                 # Others lines are Wifi stats
                 wifi_stats = f.readline()
                 while wifi_stats != '':
                     # Extract the stats
@@ -150,15 +149,15 @@
             ret = 'DEFAULT'
 
         return ret
 
     def update_views(self):
         """Update stats views."""
         # Call the father's method
-        super(PluginModel, self).update_views()
+        super().update_views()
 
         # Add specifics information
         # Alert on quality_level thresholds
         for i in self.stats:
             self.views[i[self.get_key()]]['quality_level']['decoration'] = self.get_alert(i['quality_level'])
 
     def msg_curse(self, args=None, max_width=None):
@@ -171,15 +170,15 @@
             return ret
 
         # Max size for the interface name
         if max_width:
             if_name_max_width = max_width - 5
         else:
             # No max_width defined, return an emptu curse message
-            logger.debug("No max_width defined for the {} plugin, it will not be displayed.".format(self.plugin_name))
+            logger.debug(f"No max_width defined for the {self.plugin_name} plugin, it will not be displayed.")
             return ret
 
         # Build the string message
         # Header
         msg = '{:{width}}'.format('WIFI', width=if_name_max_width)
         ret.append(self.curse_add_line(msg, "TITLE"))
         msg = '{:>7}'.format('dBm')
```

### Comparing `glances-4.0.4/glances/ports_list.py` & `glances-4.0.5/glances/ports_list.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,19 @@
-# -*- coding: utf-8 -*-
 #
 # This file is part of Glances.
 #
 # SPDX-FileCopyrightText: 2022 Nicolas Hennion <nicolas@nicolargo.com>
 #
 # SPDX-License-Identifier: LGPL-3.0-only
 #
 
 """Manage the Glances ports list (Ports plugin)."""
 
-from glances.logger import logger
 from glances.globals import BSD
+from glances.logger import logger
 
 # XXX *BSDs: Segmentation fault (core dumped)
 # -- https://bitbucket.org/al45tair/netifaces/issues/15
 # Also used in the glances_ip plugin
 if not BSD:
     try:
         import netifaces
@@ -22,15 +21,15 @@
         netifaces_tag = True
     except ImportError:
         netifaces_tag = False
 else:
     netifaces_tag = False
 
 
-class GlancesPortsList(object):
+class GlancesPortsList:
     """Manage the ports list for the ports plugin."""
 
     _section = "ports"
     _default_refresh = 60
     _default_timeout = 3
 
     def __init__(self, config=None, args=None):
@@ -42,17 +41,17 @@
     def load(self, config):
         """Load the ports list from the configuration file."""
         ports_list = []
 
         if config is None:
             logger.debug("No configuration file available. Cannot load ports list.")
         elif not config.has_section(self._section):
-            logger.debug("No [%s] section in the configuration file. Cannot load ports list." % self._section)
+            logger.debug(f"No [{self._section}] section in the configuration file. Cannot load ports list.")
         else:
-            logger.debug("Start reading the [%s] section in the configuration file" % self._section)
+            logger.debug(f"Start reading the [{self._section}] section in the configuration file")
 
             refresh = int(config.get_value(self._section, 'refresh', default=self._default_refresh))
             timeout = int(config.get_value(self._section, 'timeout', default=self._default_timeout))
 
             # Add default gateway on top of the ports_list lists
             default_gateway = config.get_value(self._section, 'port_default_gateway', default='False')
             if default_gateway.lower().startswith('true') and netifaces_tag:
@@ -64,60 +63,60 @@
                 # ICMP
                 new_port['port'] = 0
                 new_port['description'] = 'DefaultGateway'
                 new_port['refresh'] = refresh
                 new_port['timeout'] = timeout
                 new_port['status'] = None
                 new_port['rtt_warning'] = None
-                new_port['indice'] = str('port_0')
-                logger.debug("Add default gateway %s to the static list" % (new_port['host']))
+                new_port['indice'] = 'port_0'
+                logger.debug("Add default gateway {} to the static list".format(new_port['host']))
                 ports_list.append(new_port)
 
             # Read the scan list
             for i in range(1, 256):
                 new_port = {}
-                postfix = 'port_%s_' % str(i)
+                postfix = f'port_{str(i)}_'
 
                 # Read mandatory configuration key: host
-                new_port['host'] = config.get_value(self._section, '%s%s' % (postfix, 'host'))
+                new_port['host'] = config.get_value(self._section, '{}{}'.format(postfix, 'host'))
 
                 if new_port['host'] is None:
                     continue
 
                 # Read optionals configuration keys
                 # Port is set to 0 by default. 0 mean ICMP check instead of TCP check
-                new_port['port'] = config.get_value(self._section, '%s%s' % (postfix, 'port'), 0)
+                new_port['port'] = config.get_value(self._section, '{}{}'.format(postfix, 'port'), 0)
                 new_port['description'] = config.get_value(
-                    self._section, '%sdescription' % postfix, default="%s:%s" % (new_port['host'], new_port['port'])
+                    self._section, f'{postfix}description', default="{}:{}".format(new_port['host'], new_port['port'])
                 )
 
                 # Default status
                 new_port['status'] = None
 
                 # Refresh rate in second
                 new_port['refresh'] = refresh
 
                 # Timeout in second
-                new_port['timeout'] = int(config.get_value(self._section, '%stimeout' % postfix, default=timeout))
+                new_port['timeout'] = int(config.get_value(self._section, f'{postfix}timeout', default=timeout))
 
                 # RTT warning
-                new_port['rtt_warning'] = config.get_value(self._section, '%srtt_warning' % postfix, default=None)
+                new_port['rtt_warning'] = config.get_value(self._section, f'{postfix}rtt_warning', default=None)
                 if new_port['rtt_warning'] is not None:
                     # Convert to second
                     new_port['rtt_warning'] = int(new_port['rtt_warning']) / 1000.0
 
                 # Indice
                 new_port['indice'] = 'port_' + str(i)
 
                 # Add the server to the list
-                logger.debug("Add port %s:%s to the static list" % (new_port['host'], new_port['port']))
+                logger.debug("Add port {}:{} to the static list".format(new_port['host'], new_port['port']))
                 ports_list.append(new_port)
 
             # Ports list loaded
-            logger.debug("Ports list loaded: %s" % ports_list)
+            logger.debug(f"Ports list loaded: {ports_list}")
 
         return ports_list
 
     def get_ports_list(self):
         """Return the current server list (dict of dict)."""
         return self._ports_list
```

### Comparing `glances-4.0.4/glances/processes.py` & `glances-4.0.5/glances/processes.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,25 @@
-# -*- coding: utf-8 -*-
 #
 # This file is part of Glances.
 #
 # SPDX-FileCopyrightText: 2024 Nicolas Hennion <nicolas@nicolargo.com>
 #
 # SPDX-License-Identifier: LGPL-3.0-only
 #
 
 import os
 
-from glances.globals import BSD, LINUX, MACOS, WINDOWS, iterkeys
-from glances.globals import namedtuple_to_dict, list_of_namedtuple_to_list_of_dict
-from glances.timer import Timer, getTimeSinceLastUpdate
-from glances.filter import GlancesFilterList, GlancesFilter
-from glances.programs import processes_to_programs
-from glances.logger import logger
-
 import psutil
 
+from glances.filter import GlancesFilter, GlancesFilterList
+from glances.globals import BSD, LINUX, MACOS, WINDOWS, iterkeys, list_of_namedtuple_to_list_of_dict, namedtuple_to_dict
+from glances.logger import logger
+from glances.programs import processes_to_programs
+from glances.timer import Timer, getTimeSinceLastUpdate
+
 psutil_version_info = tuple([int(num) for num in psutil.__version__.split('.')])
 
 # This constant defines the list of available processes sort key
 sort_processes_key_list = ['cpu_percent', 'memory_percent', 'username', 'cpu_times', 'io_counters', 'name']
 
 # Sort dictionary for human
 sort_for_human = {
@@ -31,15 +29,15 @@
     'cpu_times': 'process time',
     'username': 'user name',
     'name': 'processs name',
     None: 'None',
 }
 
 
-class GlancesProcesses(object):
+class GlancesProcesses:
     """Get processed stats using the psutil library."""
 
     def __init__(self, cache_timeout=60):
         """Init the class to collect stats about processes."""
         # Init the args, coming from the GlancesStandalone class
         # Should be set by the set_args method
         self.args = None
@@ -80,26 +78,26 @@
         self.extended_process = None
 
         # Test if the system can grab io_counters
         try:
             p = psutil.Process()
             p.io_counters()
         except Exception as e:
-            logger.warning('PsUtil can not grab processes io_counters ({})'.format(e))
+            logger.warning(f'PsUtil can not grab processes io_counters ({e})')
             self.disable_io_counters = True
         else:
             logger.debug('PsUtil can grab processes io_counters')
             self.disable_io_counters = False
 
         # Test if the system can grab gids
         try:
             p = psutil.Process()
             p.gids()
         except Exception as e:
-            logger.warning('PsUtil can not grab processes gids ({})'.format(e))
+            logger.warning(f'PsUtil can not grab processes gids ({e})')
             self.disable_gids = True
         else:
             logger.debug('PsUtil can grab processes gids')
             self.disable_gids = False
 
         # Maximum number of processes showed in the UI (None if no limit)
         self._max_processes = None
@@ -180,15 +178,15 @@
         :returns: int or None
         """
         if LINUX:
             # XXX: waiting for https://github.com/giampaolo/psutil/issues/720
             try:
                 with open('/proc/sys/kernel/pid_max', 'rb') as f:
                     return int(f.read())
-            except (OSError, IOError):
+            except OSError:
                 return None
         else:
             return None
 
     @property
     def processes_count(self):
         """Get the current number of processes showed in the UI."""
@@ -307,15 +305,15 @@
 
             # Get memory swap for the selected process (Linux Only)
             ret['memory_swap'] = self.__get_extended_memory_swap(selected_process)
 
             # Get number of TCP and UDP network connections for the selected process
             ret['tcp'], ret['udp'] = self.__get_extended_connections(selected_process)
         except (psutil.NoSuchProcess, ValueError, AttributeError) as e:
-            logger.error('Can not grab extended stats ({})'.format(e))
+            logger.error(f'Can not grab extended stats ({e})')
             self.extended_process = None
             ret['extended_stats'] = False
         else:
             # Compute CPU and MEM min/max/mean
             # Merge the returned dict with the current on
             ret.update(self.__get_min_max_mean(proc))
             self.extended_process = ret
@@ -565,16 +563,15 @@
 
     def get_list(self, sorted_by=None, as_programs=False):
         """Get the processlist.
         By default, return the list of threads.
         If as_programs is True, return the list of programs."""
         if as_programs:
             return processes_to_programs(self.processlist)
-        else:
-            return self.processlist
+        return self.processlist
 
     def get_export(self):
         """Return the processlist for export."""
         return self.processlist_export
 
     @property
     def sort_key(self):
@@ -593,38 +590,34 @@
     def nice_decrease(self, pid):
         """Decrease nice level
         On UNIX this is a number which usually goes from -20 to 20.
         The higher the nice value, the lower the priority of the process."""
         p = psutil.Process(pid)
         try:
             p.nice(p.nice() - 1)
-            logger.info('Set nice level of process {} to {} (higher the priority)'.format(pid, p.nice()))
+            logger.info(f'Set nice level of process {pid} to {p.nice()} (higher the priority)')
         except psutil.AccessDenied:
-            logger.warning(
-                'Can not decrease (higher the priority) the nice level of process {} (access denied)'.format(pid)
-            )
+            logger.warning(f'Can not decrease (higher the priority) the nice level of process {pid} (access denied)')
 
     def nice_increase(self, pid):
         """Increase nice level
         On UNIX this is a number which usually goes from -20 to 20.
         The higher the nice value, the lower the priority of the process."""
         p = psutil.Process(pid)
         try:
             p.nice(p.nice() + 1)
-            logger.info('Set nice level of process {} to {} (lower the priority)'.format(pid, p.nice()))
+            logger.info(f'Set nice level of process {pid} to {p.nice()} (lower the priority)')
         except psutil.AccessDenied:
-            logger.warning(
-                'Can not increase (lower the priority) the nice level of process {} (access denied)'.format(pid)
-            )
+            logger.warning(f'Can not increase (lower the priority) the nice level of process {pid} (access denied)')
 
     def kill(self, pid, timeout=3):
         """Kill process with pid"""
         assert pid != os.getpid(), "Glances can kill itself..."
         p = psutil.Process(pid)
-        logger.debug('Send kill signal to process: {}'.format(p))
+        logger.debug(f'Send kill signal to process: {p}')
         p.kill()
         return p.wait(timeout)
 
 
 def weighted(value):
     """Manage None value in dict value."""
     return -float('inf') if value is None else value
```

### Comparing `glances-4.0.4/glances/programs.py` & `glances-4.0.5/glances/programs.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 #
 # This file is part of Glances.
 #
 # SPDX-FileCopyrightText: 2024 Nicolas Hennion <nicolas@nicolargo.com>
 #
 # SPDX-License-Identifier: LGPL-3.0-only
 #
```

### Comparing `glances-4.0.4/glances/secure.py` & `glances-4.0.5/glances/secure.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,20 +1,19 @@
-# -*- coding: utf-8 -*-
 #
 # This file is part of Glances.
 #
 # SPDX-FileCopyrightText: 2022 Nicolas Hennion <nicolas@nicolargo.com>
 #
 # SPDX-License-Identifier: LGPL-3.0-only
 #
 
 """Secures functions for Glances"""
 
-from subprocess import Popen, PIPE
 import re
+from subprocess import PIPE, Popen
 
 from glances.globals import nativestr
 
 
 def secure_popen(cmd):
     """A more or less secure way to execute system commands
 
@@ -35,16 +34,16 @@
     """A more or less secure way to execute system command
 
     Manage redirection (>) and pipes (|)
     """
     # Split by redirection '>'
     cmd_split_redirect = cmd.split('>')
     if len(cmd_split_redirect) > 2:
-        return 'Glances error: Only one file redirection allowed ({})'.format(cmd)
-    elif len(cmd_split_redirect) == 2:
+        return f'Glances error: Only one file redirection allowed ({cmd})'
+    if len(cmd_split_redirect) == 2:
         stdout_redirect = cmd_split_redirect[1].strip()
         cmd = cmd_split_redirect[0]
     else:
         stdout_redirect = None
 
     sub_cmd_stdin = None
     p_last = None
```

### Comparing `glances-4.0.4/glances/server.py` & `glances-4.0.5/glances/server.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,41 +1,39 @@
-# -*- coding: utf-8 -*-
 #
 # This file is part of Glances.
 #
 # SPDX-FileCopyrightText: 2022 Nicolas Hennion <nicolas@nicolargo.com>
 #
 # SPDX-License-Identifier: LGPL-3.0-only
 #
 
 """Manage the Glances server."""
 
-from glances.globals import json_dumps
 import socket
 import sys
 from base64 import b64decode
 
 from glances import __version__
-from glances.globals import SimpleXMLRPCRequestHandler, SimpleXMLRPCServer
 from glances.autodiscover import GlancesAutoDiscoverClient
+from glances.globals import SimpleXMLRPCRequestHandler, SimpleXMLRPCServer, json_dumps
 from glances.logger import logger
 from glances.stats_server import GlancesStatsServer
 from glances.timer import Timer
 
 
-class GlancesXMLRPCHandler(SimpleXMLRPCRequestHandler, object):
+class GlancesXMLRPCHandler(SimpleXMLRPCRequestHandler):
     """Main XML-RPC handler."""
 
     rpc_paths = ('/RPC2',)
 
     def end_headers(self):
         # Hack to add a specific header
         # Thk to: https://gist.github.com/rca/4063325
         self.send_my_headers()
-        super(GlancesXMLRPCHandler, self).end_headers()
+        super().end_headers()
 
     def send_my_headers(self):
         # Specific header is here (solved the issue #227)
         self.send_header("Access-Control-Allow-Origin", "*")
 
     def authenticate(self, headers):
         # auth = headers.get('Authorization')
@@ -65,61 +63,59 @@
         # Check username and password in the dictionary
         if username in self.server.user_dict:
             from glances.password import GlancesPassword
 
             # TODO: config is not taken into account: it may be a problem ?
             pwd = GlancesPassword(username=username, config=None)
             return pwd.check_password(self.server.user_dict[username], password)
-        else:
-            return False
+        return False
 
     def parse_request(self):
         if SimpleXMLRPCRequestHandler.parse_request(self):
             # Next we authenticate
             if self.authenticate(self.headers):
                 return True
-            else:
-                # if authentication fails, tell the client
-                self.send_error(401, 'Authentication failed')
+            # if authentication fails, tell the client
+            self.send_error(401, 'Authentication failed')
         return False
 
     def log_message(self, log_format, *args):
         # No message displayed on the server side
         pass
 
 
-class GlancesXMLRPCServer(SimpleXMLRPCServer, object):
+class GlancesXMLRPCServer(SimpleXMLRPCServer):
     """Init a SimpleXMLRPCServer instance (IPv6-ready)."""
 
     finished = False
 
     def __init__(self, bind_address, bind_port=61209, requestHandler=GlancesXMLRPCHandler, config=None):
         self.bind_address = bind_address
         self.bind_port = bind_port
         self.config = config
         try:
             self.address_family = socket.getaddrinfo(bind_address, bind_port)[0][0]
-        except socket.error as e:
-            logger.error("Couldn't open socket: {}".format(e))
+        except OSError as e:
+            logger.error(f"Couldn't open socket: {e}")
             sys.exit(1)
 
-        super(GlancesXMLRPCServer, self).__init__((bind_address, bind_port), requestHandler)
+        super().__init__((bind_address, bind_port), requestHandler)
 
     def end(self):
         """Stop the server"""
         self.server_close()
         self.finished = True
 
     def serve_forever(self):
         """Main loop"""
         while not self.finished:
             self.handle_request()
 
 
-class GlancesInstance(object):
+class GlancesInstance:
     """All the methods of this class are published as XML-RPC methods."""
 
     def __init__(self, config=None, args=None):
         # Init stats
         self.stats = GlancesStatsServer(config=config, args=args)
 
         # Initial update
@@ -175,29 +171,29 @@
                 # The method is not found for the plugin
                 raise AttributeError(item)
         else:
             # Default behavior
             raise AttributeError(item)
 
 
-class GlancesServer(object):
+class GlancesServer:
     """This class creates and manages the TCP server."""
 
     def __init__(self, requestHandler=GlancesXMLRPCHandler, config=None, args=None):
         # Args
         self.args = args
 
         # Init the XML RPC server
         try:
             self.server = GlancesXMLRPCServer(args.bind_address, args.port, requestHandler, config=config)
         except Exception as e:
-            logger.critical("Cannot start Glances server: {}".format(e))
+            logger.critical(f"Cannot start Glances server: {e}")
             sys.exit(2)
         else:
-            print('Glances XML-RPC server is running on {}:{}'.format(args.bind_address, args.port))
+            print(f'Glances XML-RPC server is running on {args.bind_address}:{args.port}')
 
         # The users dict
         # username / password couple
         # By default, no auth is needed
         self.server.user_dict = {}
         self.server.isAuth = False
```

### Comparing `glances-4.0.4/glances/snmp.py` & `glances-4.0.5/glances/snmp.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 #
 # This file is part of Glances.
 #
 # SPDX-FileCopyrightText: 2022 Nicolas Hennion <nicolas@nicolargo.com>
 #
 # SPDX-License-Identifier: LGPL-3.0-only
 #
@@ -15,19 +14,19 @@
 try:
     from pysnmp.entity.rfc3413.oneliner import cmdgen
 except ImportError:
     logger.critical("PySNMP library not found. To install it: pip install pysnmp")
     sys.exit(2)
 
 
-class GlancesSNMPClient(object):
+class GlancesSNMPClient:
     """SNMP client class (based on pysnmp library)."""
 
     def __init__(self, host='localhost', port=161, version='2c', community='public', user='private', auth=''):
-        super(GlancesSNMPClient, self).__init__()
+        super().__init__()
         self.cmdGen = cmdgen.CommandGenerator()
 
         self.version = version
 
         self.host = host
         self.port = port
 
@@ -93,21 +92,21 @@
         """
         if self.version.startswith('3'):
             errorIndication, errorStatus, errorIndex, varBinds = self.cmdGen.getCmd(
                 cmdgen.UsmUserData(self.user, self.auth),
                 cmdgen.UdpTransportTarget((self.host, self.port)),
                 non_repeaters,
                 max_repetitions,
-                *oid
+                *oid,
             )
         if self.version.startswith('2'):
             errorIndication, errorStatus, errorIndex, varBindTable = self.cmdGen.bulkCmd(
                 cmdgen.CommunityData(self.community),
                 cmdgen.UdpTransportTarget((self.host, self.port)),
                 non_repeaters,
                 max_repetitions,
-                *oid
+                *oid,
             )
         else:
             # Bulk request are not available with SNMP version 1
             return []
         return self.__bulk_result__(errorIndication, errorStatus, errorIndex, varBindTable)
```

### Comparing `glances-4.0.4/glances/standalone.py` & `glances-4.0.5/glances/standalone.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,52 +1,50 @@
-# -*- coding: utf-8 -*-
 #
 # This file is part of Glances.
 #
 # SPDX-FileCopyrightText: 2022 Nicolas Hennion <nicolas@nicolargo.com>
 #
 # SPDX-License-Identifier: LGPL-3.0-only
 #
 
 """Manage the Glances standalone session."""
 
 import sys
 import time
 
-from glances.logger import logger
-
 from glances.globals import WINDOWS
-from glances.processes import glances_processes
-from glances.stats import GlancesStats
+from glances.logger import logger
+from glances.outdated import Outdated
 from glances.outputs.glances_curses import GlancesCursesStandalone
 from glances.outputs.glances_stdout import GlancesStdout
-from glances.outputs.glances_stdout_json import GlancesStdoutJson
+from glances.outputs.glances_stdout_apidoc import GlancesStdoutApiDoc
 from glances.outputs.glances_stdout_csv import GlancesStdoutCsv
 from glances.outputs.glances_stdout_issue import GlancesStdoutIssue
-from glances.outputs.glances_stdout_apidoc import GlancesStdoutApiDoc
-from glances.outdated import Outdated
+from glances.outputs.glances_stdout_json import GlancesStdoutJson
+from glances.processes import glances_processes
+from glances.stats import GlancesStats
 from glances.timer import Counter
 
 
-class GlancesStandalone(object):
+class GlancesStandalone:
     """This class creates and manages the Glances standalone session."""
 
     def __init__(self, config=None, args=None):
         self.config = config
         self.args = args
 
         # Quiet mode
         self._quiet = args.quiet
         self.refresh_time = args.time
 
         # Init stats
         start_duration = Counter()
         start_duration.reset()
         self.stats = GlancesStats(config=config, args=args)
-        logger.debug("Plugins initialisation duration: {} seconds".format(start_duration.get()))
+        logger.debug(f"Plugins initialisation duration: {start_duration.get()} seconds")
 
         # Modules (plugins and exporters) are loaded at this point
         # Glances can display the list if asked...
         if args.modules_list:
             self.display_modules_list()
             sys.exit(0)
 
@@ -59,52 +57,52 @@
             glances_processes.disable_extended()
         else:
             logger.debug("Extended stats for top process are enabled")
             glances_processes.enable_extended()
 
         # Manage optional process filter
         if args.process_filter is not None:
-            logger.info("Process filter is set to: {}".format(args.process_filter))
+            logger.info(f"Process filter is set to: {args.process_filter}")
             glances_processes.process_filter = args.process_filter
 
         if (args.export or args.stdout) and args.export_process_filter is not None:
-            logger.info("Export process filter is set to: {}".format(args.export_process_filter))
+            logger.info(f"Export process filter is set to: {args.export_process_filter}")
             glances_processes.export_process_filter = args.export_process_filter
 
         if (not WINDOWS) and args.no_kernel_threads:
             # Ignore kernel threads in process list
             glances_processes.disable_kernel_threads()
 
         # Initial system information update
         start_duration.reset()
         self.stats.update()
-        logger.debug("First stats update duration: {} seconds".format(start_duration.get()))
+        logger.debug(f"First stats update duration: {start_duration.get()} seconds")
 
         if self.quiet:
             logger.info("Quiet mode is ON, nothing will be displayed")
             # In quiet mode, nothing is displayed
             glances_processes.max_processes = 0
         elif args.stdout_issue:
             logger.info("Issue mode is ON")
             # Init screen
             self.screen = GlancesStdoutIssue(config=config, args=args)
         elif args.stdout_apidoc:
             logger.info("Fields descriptions mode is ON")
             # Init screen
             self.screen = GlancesStdoutApiDoc(config=config, args=args)
         elif args.stdout:
-            logger.info("Stdout mode is ON, following stats will be displayed: {}".format(args.stdout))
+            logger.info(f"Stdout mode is ON, following stats will be displayed: {args.stdout}")
             # Init screen
             self.screen = GlancesStdout(config=config, args=args)
         elif args.stdout_json:
-            logger.info("Stdout JSON mode is ON, following stats will be displayed: {}".format(args.stdout_json))
+            logger.info(f"Stdout JSON mode is ON, following stats will be displayed: {args.stdout_json}")
             # Init screen
             self.screen = GlancesStdoutJson(config=config, args=args)
         elif args.stdout_csv:
-            logger.info("Stdout CSV mode is ON, following stats will be displayed: {}".format(args.stdout_csv))
+            logger.info(f"Stdout CSV mode is ON, following stats will be displayed: {args.stdout_csv}")
             # Init screen
             self.screen = GlancesStdoutCsv(config=config, args=args)
         else:
             # Default number of processes to displayed is set to 50
             glances_processes.max_processes = 50
 
             # Init screen
@@ -140,38 +138,38 @@
 
         :return: True if we should continue (no exit key has been pressed)
         """
         # Update stats
         # Start a counter used to compute the time needed
         counter = Counter()
         self.stats.update()
-        logger.debug('Stats updated duration: {} seconds'.format(counter.get()))
+        logger.debug(f'Stats updated duration: {counter.get()} seconds')
 
         # Patch for issue1326 to avoid < 0 refresh
         adapted_refresh = (self.refresh_time - counter.get()) if (self.refresh_time - counter.get()) > 0 else 0
 
         # Display stats
         # and wait refresh_time - counter
         if not self.quiet:
             # The update function return True if an exit key 'q' or 'ESC'
             # has been pressed.
             counter_display = Counter()
             ret = not self.screen.update(self.stats, duration=adapted_refresh)
-            logger.debug('Stats display duration: {} seconds'.format(counter_display.get() - adapted_refresh))
+            logger.debug(f'Stats display duration: {counter_display.get() - adapted_refresh} seconds')
         else:
             # Nothing is displayed
             # Break should be done via a signal (CTRL-C)
             time.sleep(adapted_refresh)
             ret = True
 
         # Export stats
         # Start a counter used to compute the time needed
         counter_export = Counter()
         self.stats.export(self.stats)
-        logger.debug('Stats exported duration: {} seconds'.format(counter_export.get()))
+        logger.debug(f'Stats exported duration: {counter_export.get()} seconds')
 
         return ret
 
     def serve_n(self, n=1):
         """Serve n time."""
         for _ in range(n):
             if not self.__serve_once():
@@ -193,18 +191,16 @@
             self.screen.end()
 
         # Exit from export modules
         self.stats.end()
 
         # Check Glances version versus PyPI one
         if self.outdated.is_outdated():
-            print(
-                "You are using Glances version {}, however version {} is available.".format(
-                    self.outdated.installed_version(), self.outdated.latest_version()
-                )
-            )
+            latest_version = self.outdated.latest_version()
+            installed_version = self.outdated.installed_version()
+            print(f"You are using Glances version {installed_version}, however version {latest_version} is available.")
             print("You should consider upgrading using: pip install --upgrade glances")
             print("Disable this warning temporarily using: glances --disable-check-update")
             print(
                 "To disable it permanently, refer config reference at "
                 "https://glances.readthedocs.io/en/latest/config.html#syntax"
             )
```

### Comparing `glances-4.0.4/glances/static_list.py` & `glances-4.0.5/glances/static_list.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 #
 # This file is part of Glances.
 #
 # SPDX-FileCopyrightText: 2022 Nicolas Hennion <nicolas@nicolargo.com>
 #
 # SPDX-License-Identifier: LGPL-3.0-only
 #
@@ -10,15 +9,15 @@
 """Manage the Glances server static list."""
 
 from socket import gaierror, gethostbyname
 
 from glances.logger import logger
 
 
-class GlancesStaticServer(object):
+class GlancesStaticServer:
     """Manage the static servers list for the client browser."""
 
     _section = "serverlist"
 
     def __init__(self, config=None, args=None):
         # server_list is a list of dict (JSON compliant)
         # [ {'key': 'zeroconf name', ip': '172.1.2.3', 'port': 61209, 'cpu': 3, 'mem': 34 ...} ... ]
@@ -28,50 +27,50 @@
     def load(self, config):
         """Load the server list from the configuration file."""
         server_list = []
 
         if config is None:
             logger.debug("No configuration file available. Cannot load server list.")
         elif not config.has_section(self._section):
-            logger.warning("No [%s] section in the configuration file. Cannot load server list." % self._section)
+            logger.warning(f"No [{self._section}] section in the configuration file. Cannot load server list.")
         else:
-            logger.info("Start reading the [%s] section in the configuration file" % self._section)
+            logger.info(f"Start reading the [{self._section}] section in the configuration file")
             for i in range(1, 256):
                 new_server = {}
-                postfix = 'server_%s_' % str(i)
+                postfix = f'server_{str(i)}_'
                 # Read the server name (mandatory)
                 for s in ['name', 'port', 'alias']:
-                    new_server[s] = config.get_value(self._section, '%s%s' % (postfix, s))
+                    new_server[s] = config.get_value(self._section, f'{postfix}{s}')
                 if new_server['name'] is not None:
                     # Manage optional information
                     if new_server['port'] is None:
                         new_server['port'] = '61209'
                     new_server['username'] = 'glances'
                     # By default, try empty (aka no) password
                     new_server['password'] = ''
                     try:
                         new_server['ip'] = gethostbyname(new_server['name'])
                     except gaierror as e:
-                        logger.error("Cannot get IP address for server %s (%s)" % (new_server['name'], e))
+                        logger.error("Cannot get IP address for server {} ({})".format(new_server['name'], e))
                         continue
                     new_server['key'] = new_server['name'] + ':' + new_server['port']
 
                     # Default status is 'UNKNOWN'
                     new_server['status'] = 'UNKNOWN'
 
                     # Server type is 'STATIC'
                     new_server['type'] = 'STATIC'
 
                     # Add the server to the list
-                    logger.debug("Add server %s to the static list" % new_server['name'])
+                    logger.debug("Add server {} to the static list".format(new_server['name']))
                     server_list.append(new_server)
 
             # Server list loaded
-            logger.info("%s server(s) loaded from the configuration file" % len(server_list))
-            logger.debug("Static server list: %s" % server_list)
+            logger.info(f"{len(server_list)} server(s) loaded from the configuration file")
+            logger.debug(f"Static server list: {server_list}")
 
         return server_list
 
     def get_servers_list(self):
         """Return the current server list (list of dict)."""
         return self._server_list
```

### Comparing `glances-4.0.4/glances/stats.py` & `glances-4.0.5/glances/stats.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,32 +1,31 @@
-# -*- coding: utf-8 -*-
 #
 # This file is part of Glances.
 #
 # SPDX-FileCopyrightText: 2022 Nicolas Hennion <nicolas@nicolargo.com>
 #
 # SPDX-License-Identifier: LGPL-3.0-only
 #
 
 """The stats manager."""
 
 import collections
 import os
+import pathlib
 import sys
 import threading
 import traceback
 from importlib import import_module
-import pathlib
 
-from glances.logger import logger
 from glances.globals import exports_path, plugins_path, sys_path
+from glances.logger import logger
 from glances.timer import Counter
 
 
-class GlancesStats(object):
+class GlancesStats:
     """This class stores, updates and gives stats."""
 
     # Script header constant
     header = "glances_"
 
     def __init__(self, config=None, args=None):
         # Set the config instance
@@ -51,31 +50,28 @@
             # Get the plugin name
             plugname = item[len('getViews') :].lower()
             # Get the plugin instance
             plugin = self._plugins[plugname]
             if hasattr(plugin, 'get_json_views'):
                 # The method get_views exist, return it
                 return getattr(plugin, 'get_json_views')
-            else:
-                # The method get_views is not found for the plugin
-                raise AttributeError(item)
-        elif item.startswith('get'):
+            # The method get_views is not found for the plugin
+            raise AttributeError(item)
+        if item.startswith('get'):
             # Get the plugin name
             plugname = item[len('get') :].lower()
             # Get the plugin instance
             plugin = self._plugins[plugname]
             if hasattr(plugin, 'get_stats'):
                 # The method get_stats exist, return it
                 return getattr(plugin, 'get_stats')
-            else:
-                # The method get_stats is not found for the plugin
-                raise AttributeError(item)
-        else:
-            # Default behavior
+            # The method get_stats is not found for the plugin
             raise AttributeError(item)
+        # Default behavior
+        raise AttributeError(item)
 
     def load_modules(self, args):
         """Wrapper to load: plugins and export modules."""
 
         # Init the plugins dict
         # Active plugins dictionary
         self._plugins = collections.defaultdict(dict)
@@ -103,15 +99,15 @@
             # Import the plugin
             plugin = import_module('glances.plugins.' + plugin_path)
             # Init and add the plugin to the dictionary
             self._plugins[plugin_path] = plugin.PluginModel(args=args, config=config)
         except Exception as e:
             # If a plugin can not be loaded, display a critical message
             # on the console but do not crash
-            logger.critical("Error while initializing the {} plugin ({})".format(plugin_path, e))
+            logger.critical(f"Error while initializing the {plugin_path} plugin ({e})")
             logger.error(traceback.format_exc())
             # An error occurred, disable the plugin
             if args is not None:
                 setattr(args, 'disable_' + plugin_path, False)
         else:
             # Manage the default status of the plugin (enable or disable)
             if args is not None:
@@ -127,18 +123,18 @@
         start_duration = Counter()
 
         for item in os.listdir(plugins_path):
             if os.path.isdir(os.path.join(plugins_path, item)) and not item.startswith('__') and item != 'plugin':
                 # Load the plugin
                 start_duration.reset()
                 self._load_plugin(os.path.basename(item), args=args, config=self.config)
-                logger.debug("Plugin {} started in {} seconds".format(item, start_duration.get()))
+                logger.debug(f"Plugin {item} started in {start_duration.get()} seconds")
 
         # Log plugins list
-        logger.debug("Active plugins list: {}".format(self.getPluginsList()))
+        logger.debug(f"Active plugins list: {self.getPluginsList()}")
 
     def load_additional_plugins(self, args=None, config=None):
         """Load additional plugins if defined"""
 
         def get_addl_plugins(self, plugin_path):
             """Get list of additonal plugins"""
             _plugin_list = []
@@ -173,27 +169,27 @@
                 if plugin in sys.modules:
                     logger.warn(f"Pugin {plugin} already in sys.modules, skipping (workaround: rename plugin)")
                 else:
                     start_duration.reset()
                     try:
                         _mod_loaded = import_module(plugin + '.model')
                         self._plugins[plugin] = _mod_loaded.PluginModel(args=args, config=config)
-                        logger.debug("Plugin {} started in {} seconds".format(plugin, start_duration.get()))
+                        logger.debug(f"Plugin {plugin} started in {start_duration.get()} seconds")
                     except Exception as e:
                         # If a plugin can not be loaded, display a critical message
                         # on the console but do not crash
-                        logger.critical("Error while initializing the {} plugin ({})".format(plugin, e))
+                        logger.critical(f"Error while initializing the {plugin} plugin ({e})")
                         logger.error(traceback.format_exc())
                         # An error occurred, disable the plugin
                         if args:
                             setattr(args, 'disable_' + plugin, False)
 
             sys.path = _sys_path
             # Log plugins list
-            logger.debug("Active additional plugins list: {}".format(self.getPluginsList()))
+            logger.debug(f"Active additional plugins list: {self.getPluginsList()}")
 
     def load_exports(self, args=None):
         """Load all exporters in the 'exports' folder."""
         start_duration = Counter()
 
         if args is None:
             return False
@@ -217,45 +213,43 @@
                     # Add the exporter instance to the active exporters dictionary
                     self._exports[exporter_name] = export_module.Export(args=args, config=self.config)
                     # Add the exporter instance to the available exporters dictionary
                     self._exports_all[exporter_name] = self._exports[exporter_name]
                 else:
                     # Add the exporter name to the available exporters dictionary
                     self._exports_all[exporter_name] = exporter_name
-                logger.debug("Exporter {} started in {} seconds".format(exporter_name, start_duration.get()))
+                logger.debug(f"Exporter {exporter_name} started in {start_duration.get()} seconds")
 
         # Log plugins list
-        logger.debug("Active exports modules list: {}".format(self.getExportsList()))
+        logger.debug(f"Active exports modules list: {self.getExportsList()}")
         return True
 
     def getPluginsList(self, enable=True):
         """Return the plugins list.
 
         if enable is True, only return the active plugins (default)
         if enable is False, return all the plugins
 
         Return: list of plugin name
         """
         if enable:
             return [p for p in self._plugins if self._plugins[p].is_enabled()]
-        else:
-            return [p for p in self._plugins]
+        return list(self._plugins)
 
     def getExportsList(self, enable=True):
         """Return the exports list.
 
         if enable is True, only return the active exporters (default)
         if enable is False, return all the exporters
 
         :return: list of export module names
         """
         if enable:
-            return [e for e in self._exports]
-        else:
-            return [e for e in self._exports_all]
+            return list(self._exports)
+        return list(self._exports_all)
 
     def load_limits(self, config=None):
         """Load the stats limits (except the one in the exclude list)."""
         # For each plugins, call the load_limits method
         for p in self._plugins:
             self._plugins[p].load_limits(config)
 
@@ -289,15 +283,15 @@
             logger.debug("Do not export stats during the first iteration because some information are missing")
             self.first_export = False
             return False
 
         input_stats = input_stats or {}
 
         for e in self.getExportsList(enable=True):
-            logger.debug("Export stats using the %s module" % e)
+            logger.debug(f"Export stats using the {e} module")
             thread = threading.Thread(target=self._exports[e].update, args=(input_stats,))
             thread.start()
 
         return True
 
     def getAll(self):
         """Return all the stats (list)."""
@@ -363,16 +357,15 @@
         """Return the plugin list."""
         return self._plugins
 
     def get_plugin(self, plugin_name):
         """Return the plugin name."""
         if plugin_name in self._plugins:
             return self._plugins[plugin_name]
-        else:
-            return None
+        return None
 
     def end(self):
         """End of the Glances stats."""
         # Close export modules
         for e in self._exports:
             self._exports[e].exit()
         # Close plugins
```

### Comparing `glances-4.0.4/glances/stats_client.py` & `glances-4.0.5/glances/stats_client.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,31 +1,30 @@
-# -*- coding: utf-8 -*-
 #
 # This file is part of Glances.
 #
 # SPDX-FileCopyrightText: 2022 Nicolas Hennion <nicolas@nicolargo.com>
 #
 # SPDX-License-Identifier: LGPL-3.0-only
 #
 
 """The stats server manager."""
 
 import sys
 
-from glances.stats import GlancesStats
 from glances.globals import sys_path
 from glances.logger import logger
+from glances.stats import GlancesStats
 
 
 class GlancesStatsClient(GlancesStats):
     """This class stores, updates and gives stats for the client."""
 
     def __init__(self, config=None, args=None):
         """Init the GlancesStatsClient class."""
-        super(GlancesStatsClient, self).__init__(config=config, args=args)
+        super().__init__(config=config, args=args)
 
         # Init the configuration
         self.config = config
 
         # Init the arguments
         self.args = args
 
@@ -34,23 +33,21 @@
         header = "glances_"
         for item in input_plugins:
             # Import the plugin
             try:
                 plugin = __import__(header + item)
             except ImportError:
                 # Server plugin can not be imported from the client side
-                logger.error(
-                    "Can not import {} plugin. Please upgrade your Glances client/server version.".format(item)
-                )
+                logger.error(f"Can not import {item} plugin. Please upgrade your Glances client/server version.")
             else:
                 # Add the plugin to the dictionary
                 # The key is the plugin name
                 # for example, the file glances_xxx.py
                 # generate self._plugins_list["xxx"] = ...
-                logger.debug("Server uses {} plugin".format(item))
+                logger.debug(f"Server uses {item} plugin")
                 self._plugins[item] = plugin.Plugin(args=self.args)
         # Restoring system path
         sys.path = sys_path
 
     def update(self, input_stats):
         """Update all the stats."""
         # For Glances client mode
```

### Comparing `glances-4.0.4/glances/stats_client_snmp.py` & `glances-4.0.5/glances/stats_client_snmp.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,22 @@
-# -*- coding: utf-8 -*-
 #
 # This file is part of Glances.
 #
 # SPDX-FileCopyrightText: 2022 Nicolas Hennion <nicolas@nicolargo.com>
 #
 # SPDX-License-Identifier: LGPL-3.0-only
 #
 
 """The stats manager."""
 
 import re
 
-from glances.stats import GlancesStats
 from glances.globals import iteritems
 from glances.logger import logger
+from glances.stats import GlancesStats
 
 # SNMP OID regexp pattern to short system name dict
 oid_to_short_system_name = {
     '.*Linux.*': 'linux',
     '.*Darwin.*': 'mac',
     '.*BSD.*': 'bsd',
     '.*Windows.*': 'windows',
@@ -27,15 +26,15 @@
 }
 
 
 class GlancesStatsClientSNMP(GlancesStats):
     """This class stores, updates and gives stats for the SNMP client."""
 
     def __init__(self, config=None, args=None):
-        super(GlancesStatsClientSNMP, self).__init__()
+        super().__init__()
 
         # Init the configuration
         self.config = config
 
         # Init the arguments
         self.args = args
 
@@ -63,15 +62,15 @@
         # If we cannot grab the hostname, then exit...
         ret = snmp_client.get_by_oid("1.3.6.1.2.1.1.5.0") != {}
         if ret:
             # Get the OS name (need to grab the good OID...)
             oid_os_name = snmp_client.get_by_oid("1.3.6.1.2.1.1.1.0")
             try:
                 self.system_name = self.get_system_name(oid_os_name['1.3.6.1.2.1.1.1.0'])
-                logger.info("SNMP system name detected: {}".format(self.system_name))
+                logger.info(f"SNMP system name detected: {self.system_name}")
             except KeyError:
                 self.system_name = None
                 logger.warning("Cannot detect SNMP system name")
 
         return ret
 
     def get_system_name(self, oid_system_name):
@@ -102,13 +101,13 @@
             self._plugins[p].input_method = 'snmp'
             self._plugins[p].short_system_name = self.system_name
 
             # Update the stats...
             try:
                 self._plugins[p].update()
             except Exception as e:
-                logger.error("Update {} failed: {}".format(p, e))
+                logger.error(f"Update {p} failed: {e}")
             else:
                 # ... the history
                 self._plugins[p].update_stats_history()
                 # ... and the views
                 self._plugins[p].update_views()
```

### Comparing `glances-4.0.4/glances/stats_server.py` & `glances-4.0.5/glances/stats_server.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,44 +1,43 @@
-# -*- coding: utf-8 -*-
 #
 # This file is part of Glances.
 #
 # SPDX-FileCopyrightText: 2022 Nicolas Hennion <nicolas@nicolargo.com>
 #
 # SPDX-License-Identifier: LGPL-3.0-only
 #
 
 """The stats server manager."""
 
 import collections
 
-from glances.stats import GlancesStats
 from glances.logger import logger
+from glances.stats import GlancesStats
 
 
 class GlancesStatsServer(GlancesStats):
     """This class stores, updates and gives stats for the server."""
 
     def __init__(self, config=None, args=None):
         # Init the stats
-        super(GlancesStatsServer, self).__init__(config=config, args=args)
+        super().__init__(config=config, args=args)
 
         # Init the all_stats dict used by the server
         # all_stats is a dict of dicts filled by the server
         self.all_stats = collections.defaultdict(dict)
 
         # In the update method, disable extended process stats
         logger.info("Disable extended processes stats in server mode")
 
     def update(self, input_stats=None):
         """Update the stats."""
         input_stats = input_stats or {}
 
         # Force update of all the stats
-        super(GlancesStatsServer, self).update()
+        super().update()
 
         # Disable the extended processes stats because it cause an high CPU load
         self._plugins['processcount'].disable_extended()
 
         # Build all_stats variable (concatenation of all the stats)
         self.all_stats = self._set_stats(input_stats)
```

### Comparing `glances-4.0.4/glances/thresholds.py` & `glances-4.0.5/glances/thresholds.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 #
 # This file is part of Glances.
 #
 # SPDX-FileCopyrightText: 2022 Nicolas Hennion <nicolas@nicolargo.com>
 #
 # SPDX-License-Identifier: LGPL-3.0-only
 #
@@ -11,15 +10,15 @@
 Thresholds classes: OK, CAREFUL, WARNING, CRITICAL
 """
 
 import sys
 from functools import total_ordering
 
 
-class GlancesThresholds(object):
+class GlancesThresholds:
     """Class to manage thresholds dict for all Glances plugins:
 
     key: Glances stats (example: cpu_user)
     value: Threshold instance
     """
 
     threshold_list = ['OK', 'CAREFUL', 'WARNING', 'CRITICAL']
@@ -34,34 +33,33 @@
         Else return the Threshold* instance for the given plugin
         """
         if stat_name is None:
             return self._thresholds
 
         if stat_name in self._thresholds:
             return self._thresholds[stat_name]
-        else:
-            return {}
+        return {}
 
     def add(self, stat_name, threshold_description):
         """Add a new threshold to the dict (key = stat_name)"""
         if threshold_description not in self.threshold_list:
             return False
-        else:
-            self._thresholds[stat_name] = getattr(
-                self.current_module, 'GlancesThreshold' + threshold_description.capitalize()
-            )()
-            return True
+
+        self._thresholds[stat_name] = getattr(
+            self.current_module, 'GlancesThreshold' + threshold_description.capitalize()
+        )()
+        return True
 
 
 # Global variable uses to share thresholds between Glances components
 glances_thresholds = GlancesThresholds()
 
 
 @total_ordering
-class _GlancesThreshold(object):
+class _GlancesThreshold:
     """Father class for all other Thresholds"""
 
     def description(self):
         return self._threshold['description']
 
     def value(self):
         return self._threshold['value']
```

### Comparing `glances-4.0.4/glances/timer.py` & `glances-4.0.5/glances/timer.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,19 @@
-# -*- coding: utf-8 -*-
 #
 # This file is part of Glances.
 #
 # SPDX-FileCopyrightText: 2022 Nicolas Hennion <nicolas@nicolargo.com>
 #
 # SPDX-License-Identifier: LGPL-3.0-only
 #
 
 """The timer manager."""
 
-from time import time
 from datetime import datetime
+from time import time
 
 # Global list to manage the elapsed time
 last_update_times = {}
 
 
 def getTimeSinceLastUpdate(IOType):
     """Return the elapsed time since last update."""
@@ -26,15 +25,15 @@
         time_since_update = 1
     else:
         time_since_update = current_time - last_time
     last_update_times[IOType] = current_time
     return time_since_update
 
 
-class Timer(object):
+class Timer:
     """The timer class. A simple chronometer."""
 
     def __init__(self, duration):
         self.duration = duration
         self.start()
 
     def start(self):
@@ -51,15 +50,15 @@
     def set(self, duration):
         self.duration = duration
 
     def finished(self):
         return time() > self.target
 
 
-class Counter(object):
+class Counter:
     """The counter class."""
 
     def __init__(self):
         self.start()
 
     def start(self):
         self.target = datetime.now()
```

### Comparing `glances-4.0.4/glances/web_list.py` & `glances-4.0.5/glances/web_list.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,23 +1,22 @@
-# -*- coding: utf-8 -*-
 #
 # This file is part of Glances.
 #
 # SPDX-FileCopyrightText: 2022 Nicolas Hennion <nicolas@nicolargo.com>
 #
 # SPDX-License-Identifier: LGPL-3.0-only
 #
 
 """Manage the Glances web/url list (Ports plugin)."""
 
 from glances.globals import urlparse
 from glances.logger import logger
 
 
-class GlancesWebList(object):
+class GlancesWebList:
     """Manage the Web/Url list for the ports plugin."""
 
     _section = "ports"
     _default_refresh = 60
     _default_timeout = 3
 
     def __init__(self, config=None, args=None):
@@ -32,80 +31,80 @@
     def load(self, config):
         """Load the web list from the configuration file."""
         web_list = []
 
         if config is None:
             logger.debug("No configuration file available. Cannot load ports list.")
         elif not config.has_section(self._section):
-            logger.debug("No [%s] section in the configuration file. Cannot load ports list." % self._section)
+            logger.debug(f"No [{self._section}] section in the configuration file. Cannot load ports list.")
         else:
-            logger.debug("Start reading the [%s] section in the configuration file" % self._section)
+            logger.debug(f"Start reading the [{self._section}] section in the configuration file")
 
             refresh = int(config.get_value(self._section, 'refresh', default=self._default_refresh))
             timeout = int(config.get_value(self._section, 'timeout', default=self._default_timeout))
 
             # Read the web/url list
             for i in range(1, 256):
                 new_web = {}
-                postfix = 'web_%s_' % str(i)
+                postfix = f'web_{str(i)}_'
 
                 # Read mandatory configuration key: host
-                new_web['url'] = config.get_value(self._section, '%s%s' % (postfix, 'url'))
+                new_web['url'] = config.get_value(self._section, '{}{}'.format(postfix, 'url'))
                 if new_web['url'] is None:
                     continue
                 url_parse = urlparse(new_web['url'])
                 if not bool(url_parse.scheme) or not bool(url_parse.netloc):
                     logger.error(
-                        'Bad URL (%s) in the [%s] section of configuration file.' % (new_web['url'], self._section)
+                        'Bad URL ({}) in the [{}] section of configuration file.'.format(new_web['url'], self._section)
                     )
                     continue
 
                 # Read optionals configuration keys
                 # Default description is the URL without the http://
                 new_web['description'] = config.get_value(
-                    self._section, '%sdescription' % postfix, default="%s" % url_parse.netloc
+                    self._section, f'{postfix}description', default=f"{url_parse.netloc}"
                 )
 
                 # Default status
                 new_web['status'] = None
                 new_web['elapsed'] = 0
 
                 # Refresh rate in second
                 new_web['refresh'] = refresh
 
                 # Timeout in second
-                new_web['timeout'] = int(config.get_value(self._section, '%stimeout' % postfix, default=timeout))
+                new_web['timeout'] = int(config.get_value(self._section, f'{postfix}timeout', default=timeout))
 
                 # RTT warning
-                new_web['rtt_warning'] = config.get_value(self._section, '%srtt_warning' % postfix, default=None)
+                new_web['rtt_warning'] = config.get_value(self._section, f'{postfix}rtt_warning', default=None)
                 if new_web['rtt_warning'] is not None:
                     # Convert to second
                     new_web['rtt_warning'] = int(new_web['rtt_warning']) / 1000.0
 
                 # Indice
                 new_web['indice'] = 'web_' + str(i)
 
                 # ssl_verify
-                new_web['ssl_verify'] = config.get_value(self._section, '%sssl_verify' % postfix, default=True)
+                new_web['ssl_verify'] = config.get_value(self._section, f'{postfix}ssl_verify', default=True)
                 # Proxy
-                http_proxy = config.get_value(self._section, '%shttp_proxy' % postfix, default=None)
+                http_proxy = config.get_value(self._section, f'{postfix}http_proxy', default=None)
 
-                https_proxy = config.get_value(self._section, '%shttps_proxy' % postfix, default=None)
+                https_proxy = config.get_value(self._section, f'{postfix}https_proxy', default=None)
 
                 if https_proxy is None and http_proxy is None:
                     new_web['proxies'] = None
                 else:
                     new_web['proxies'] = {'http': http_proxy, 'https': https_proxy}
 
                 # Add the server to the list
-                logger.debug("Add Web URL %s to the static list" % new_web['url'])
+                logger.debug("Add Web URL {} to the static list".format(new_web['url']))
                 web_list.append(new_web)
 
             # Ports list loaded
-            logger.debug("Web list loaded: %s" % web_list)
+            logger.debug(f"Web list loaded: {web_list}")
 
         return web_list
 
     def get_web_list(self):
         """Return the current server list (dict of dict)."""
         return self._web_list
```

### Comparing `glances-4.0.4/glances/webserver.py` & `glances-4.0.5/glances/webserver.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,25 +1,24 @@
-# -*- coding: utf-8 -*-
 #
 # This file is part of Glances.
 #
 # SPDX-FileCopyrightText: 2024 Nicolas Hennion <nicolas@nicolargo.com>
 #
 # SPDX-License-Identifier: LGPL-3.0-only
 #
 
 """Glances Restful/API and Web based interface."""
 
 from glances.globals import WINDOWS
+from glances.outputs.glances_restful_api import GlancesRestfulApi
 from glances.processes import glances_processes
 from glances.stats import GlancesStats
-from glances.outputs.glances_restful_api import GlancesRestfulApi
 
 
-class GlancesWebServer(object):
+class GlancesWebServer:
     """This class creates and manages the Glances Web server session."""
 
     def __init__(self, config=None, args=None):
         # Init stats
         self.stats = GlancesStats(config, args)
 
         if not WINDOWS and args.no_kernel_threads:
```

### Comparing `glances-4.0.4/pyproject.toml` & `glances-4.0.5/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,16 +1,40 @@
 [tool.black]
 line-length = 120
 skip-string-normalization = true
 exclude = '\./glances/outputs/static/*'
 
 [tool.ruff]
+line-length = 120
+target-version = "py38"
+
+[tool.ruff.format]
+quote-style = "preserve"
+
+[tool.ruff.lint]
 # Enable pycodestyle (`E`) and Pyflakes (`F`) codes by default.
-select = ["E", "F"]
-ignore = []
+select = [
+#    "A",
+#    "B",
+#    "S",
+    "C90", # mccabe
+    "E", # pycodestyle
+    "F", # Pyflakes
+    "I", # isort
+    "N", # pep8-naming
+    "W", # pycodestyle
+    "UP", # pyupgrde
+    "C4", # flake8-comprehensions
+    "RET", # flake8-return
+#    "PL",
+#    "FBT", # flake8-boolean-trap
+#    "RUF", # Ruff-specific rules
+#    "PERF", # Perflint
+]
+ignore = ["N801", "N802", "N803", "N805", "N806", "N807", "N811", "N812", "N813", "N814", "N815", "N816", "N817", "N818"]
 
 # Allow autofix for all enabled rules (when `--fix`) is provided.
 fixable = ["A", "B", "C", "D", "E", "F", "G", "I", "N", "Q", "S", "T", "W", "ANN", "ARG", "BLE", "COM", "DJ", "DTZ", "EM", "ERA", "EXE", "FBT", "ICN", "INP", "ISC", "NPY", "PD", "PGH", "PIE", "PL", "PT", "PTH", "PYI", "RET", "RSE", "RUF", "SIM", "SLF", "TCH", "TID", "TRY", "UP", "YTT"]
 unfixable = []
 
 # Exclude a variety of commonly ignored directories.
 exclude = [
@@ -30,22 +54,20 @@
     "__pypackages__",
     "_build",
     "buck-out",
     "build",
     "dist",
     "node_modules",
     "venv",
-    "docs"
+    "venv-dev",
+    "venv-min",
+    "docs",
+    "test-data",
+    "./glances/outputs/static/*"
 ]
 
-# Same as Black.
-line-length = 120
-
 # Allow unused variables when underscore-prefixed.
 dummy-variable-rgx = "^(_+|(_+[a-zA-Z0-9_]*[a-zA-Z0-9]+?))$"
 
-# Assume Python 3.11
-target-version = "py311"
-
-[tool.ruff.mccabe]
+[tool.ruff.lint.mccabe]
 # Unlike Flake8, default to a complexity level of 10.
-max-complexity = 10
+max-complexity = 21
```

### Comparing `glances-4.0.4/setup.py` & `glances-4.0.5/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,81 +1,94 @@
 #!/usr/bin/env python
 
+import builtins
 import glob
 import os
 import re
 import sys
-from io import open
 
-from setuptools import setup, Command
+from setuptools import Command, setup
 
-# Predication warning
-# Glances version 4 will only be compatible with Python 3.7 and above
-if sys.version_info < (3, 7):
-    print('WARNING: Glances version 4 will only be compatible with Python 3.7 and above.')
-
-if sys.version_info < (3, 8):
+# If the minimal Python version is changed then do not forget to change it in:
+# - ./pyproject.toml
+# - .github/workflows/test.yml
+if not (sys.version_info >= (3, 8)):
     print('Glances requires at least Python 3.8 to run.')
     sys.exit(1)
 
 # Global functions
 ##################
 
-with open(os.path.join('glances', '__init__.py'), encoding='utf-8') as f:
+with builtins.open(os.path.join('glances', '__init__.py'), encoding='utf-8') as f:
     version = re.search(r"^__version__ = ['\"]([^'\"]*)['\"]", f.read(), re.M).group(1)
 
 if not version:
     raise RuntimeError('Cannot find Glances version information.')
 
-with open('README.rst', encoding='utf-8') as f:
+with builtins.open('README.rst', encoding='utf-8') as f:
     long_description = f.read()
 
 
 def get_data_files():
-    data_files = [
-        ('share/doc/glances', ['AUTHORS', 'COPYING', 'NEWS.rst', 'README.rst',
-                               'CONTRIBUTING.md', 'conf/glances.conf']),
-        ('share/man/man1', ['docs/man/glances.1'])
+    return [
+        (
+            'share/doc/glances',
+            ['AUTHORS', 'COPYING', 'NEWS.rst', 'README.rst', "SECURITY.md", 'CONTRIBUTING.md', 'conf/glances.conf'],
+        ),
+        ('share/man/man1', ['docs/man/glances.1']),
     ]
 
-    return data_files
-
-with open('requirements.txt') as f:
-    required = f.read().splitlines()
 
 def get_install_requires():
-    requires = required
+    required = []
+    with open('requirements.txt') as f:
+        required = f.read().splitlines()
+
+    # On Windows, install WebUI by default
     if sys.platform.startswith('win'):
-        requires.append('fastapi')
-        requires.append('uvicorn')
-        requires.append('jinja2')
-        requires.append('requests')
+        required.append('fastapi')
+        required.append('uvicorn')
+        required.append('jinja2')
+        required.append('requests')
 
-    return requires
+    return required
 
 
 def get_install_extras_require():
     extras_require = {
         'action': ['chevron'],
         'browser': ['zeroconf>=0.19.1'],
         'cloud': ['requests'],
         'containers': ['docker>=6.1.1', 'python-dateutil', 'six', 'podman', 'packaging'],
-        'export': ['bernhard', 'cassandra-driver', 'elasticsearch', 'graphitesender',
-                   'ibmcloudant', 'influxdb>=1.0.0', 'influxdb-client', 'pymongo',
-                   'kafka-python', 'pika', 'paho-mqtt', 'potsdb', 'prometheus_client',
-                   'pyzmq', 'statsd'],
+        'export': [
+            'bernhard',
+            'cassandra-driver',
+            'elasticsearch',
+            'graphitesender',
+            'ibmcloudant',
+            'influxdb>=1.0.0',
+            'influxdb-client',
+            'pymongo',
+            'kafka-python',
+            'pika',
+            'paho-mqtt',
+            'potsdb',
+            'prometheus_client',
+            'pyzmq',
+            'statsd',
+        ],
         'gpu': ['nvidia-ml-py'],
         'graph': ['pygal'],
         'ip': ['netifaces'],
         'raid': ['pymdstat'],
         'smart': ['pySMART.smartx'],
         'snmp': ['pysnmp'],
         'sparklines': ['sparklines'],
         'web': ['fastapi', 'uvicorn', 'jinja2', 'requests'],
-        'wifi': ['wifi']
+        'wifi': ['wifi'],
     }
     if sys.platform.startswith('linux'):
         extras_require['sensors'] = ['batinfo']
 
     # Add automatically the 'all' target
     extras_require.update({'all': [i[0] for i in extras_require.values()]})
 
@@ -90,14 +103,15 @@
 
     def finalize_options(self):
         pass
 
     def run(self):
         import subprocess
         import sys
+
         for t in glob.glob('unittest-core.py'):
             ret = subprocess.call([sys.executable, t]) != 0
             if ret != 0:
                 raise SystemExit(ret)
         raise SystemExit(0)
 
 
@@ -134,10 +148,10 @@
         'Operating System :: OS Independent',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
         'Programming Language :: Python :: 3.11',
         'Programming Language :: Python :: 3.12',
-        'Topic :: System :: Monitoring'
-    ]
+        'Topic :: System :: Monitoring',
+    ],
 )
```

