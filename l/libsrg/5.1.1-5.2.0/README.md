# Comparing `tmp/libsrg-5.1.1.tar.gz` & `tmp/libsrg-5.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "libsrg-5.1.1.tar", max compression
+gzip compressed data, was "libsrg-5.2.0.tar", max compression
```

## Comparing `libsrg-5.1.1.tar` & `libsrg-5.2.0.tar`

### file list

```diff
@@ -1,79 +1,79 @@
--rw-r--r--   0        0        0     1069 2022-02-24 22:12:03.211633 libsrg-5.1.1/LICENSE.txt
--rw-r--r--   0        0        0     2620 2024-05-03 23:47:01.671722 libsrg-5.1.1/README.md
--rw-r--r--   0        0        0     1464 2024-05-03 23:47:01.853721 libsrg-5.1.1/libsrg/AppTemplate.py
--rw-r--r--   0        0        0    11933 2024-05-06 15:12:41.996241 libsrg-5.1.1/libsrg/Config.py
--rwxr-xr-x   0        0        0     2603 2024-05-04 14:04:12.419228 libsrg-5.1.1/libsrg/ElapsedTime.py
--rwxr-xr-x   0        0        0     8969 2024-05-10 00:36:18.128675 libsrg-5.1.1/libsrg/Info.py
--rwxr-xr-x   0        0        0     4027 2024-05-03 23:47:01.866721 libsrg-5.1.1/libsrg/LevelBanner.py
--rwxr-xr-x   0        0        0     1514 2024-05-03 23:47:01.870721 libsrg-5.1.1/libsrg/LoggerGUIProxy.py
--rwxr-xr-x   0        0        0     6135 2024-05-03 23:47:01.873721 libsrg-5.1.1/libsrg/LoggingAppBase.py
--rwxr-xr-x   0        0        0     8167 2024-05-03 23:47:01.876721 libsrg-5.1.1/libsrg/LoggingCounter.py
--rwxr-xr-x   0        0        0      593 2024-05-03 23:47:01.880721 libsrg-5.1.1/libsrg/LoggingUtils.py
--rwxr-xr-x   0        0        0     1854 2024-05-03 23:47:01.884721 libsrg-5.1.1/libsrg/LoggingWatcher.py
--rwxr-xr-x   0        0        0     3644 2024-05-03 23:47:01.888721 libsrg-5.1.1/libsrg/NagiosBase.py
--rwxr-xr-x   0        0        0     7209 2024-05-04 13:52:43.434938 libsrg-5.1.1/libsrg/Runner.py
--rwxr-xr-x   0        0        0     4903 2024-05-03 23:47:01.898721 libsrg-5.1.1/libsrg/Runner2.py
--rw-r--r--   0        0        0     4523 2024-05-06 14:42:50.143127 libsrg-5.1.1/libsrg/Statistics/ADStatsBase.py
--rw-r--r--   0        0        0     2275 2024-04-11 13:40:23.574158 libsrg-5.1.1/libsrg/Statistics/AnalogStatsBase.py
--rw-r--r--   0        0        0     1436 2024-04-08 17:02:20.928118 libsrg-5.1.1/libsrg/Statistics/AnalogStatsCumulative.py
--rw-r--r--   0        0        0     2302 2024-05-06 14:43:05.792050 libsrg-5.1.1/libsrg/Statistics/AnalogStatsFading.py
--rw-r--r--   0        0        0     1590 2024-04-12 18:46:46.468186 libsrg-5.1.1/libsrg/Statistics/AnalogStatsSlidingWindow.py
--rw-r--r--   0        0        0     1593 2024-04-11 13:40:23.559158 libsrg-5.1.1/libsrg/Statistics/DiscreteStatsBase.py
--rw-r--r--   0        0        0      774 2024-04-08 17:02:20.912118 libsrg-5.1.1/libsrg/Statistics/DiscreteStatsCumulative.py
--rw-r--r--   0        0        0     1583 2024-04-11 13:02:36.159113 libsrg-5.1.1/libsrg/Statistics/DiscreteStatsSlidingWindow.py
--rw-r--r--   0        0        0     1839 2024-04-11 13:46:23.627270 libsrg-5.1.1/libsrg/Statistics/UnitTests/ADStatsBase_test.py
--rw-r--r--   0        0        0     2784 2024-04-17 20:08:12.373031 libsrg-5.1.1/libsrg/Statistics/UnitTests/AnalogStatsBase_test.py
--rw-r--r--   0        0        0     2344 2024-04-11 13:56:04.322214 libsrg-5.1.1/libsrg/Statistics/UnitTests/AnalogStatsCumulative_test.py
--rw-r--r--   0        0        0     3915 2024-04-11 13:59:27.002140 libsrg-5.1.1/libsrg/Statistics/UnitTests/AnalogStatsFading_test.py
--rw-r--r--   0        0        0     2933 2024-04-12 18:46:46.483186 libsrg-5.1.1/libsrg/Statistics/UnitTests/AnalogStatsSlidingWindow_test.py
--rw-r--r--   0        0        0     1605 2024-04-09 15:09:14.481097 libsrg-5.1.1/libsrg/Statistics/UnitTests/DiscteteStatsBase_test.py
--rw-r--r--   0        0        0     2607 2024-04-11 00:45:26.519787 libsrg-5.1.1/libsrg/Statistics/UnitTests/DiscteteStatsSlidingWindow_test.py
--rw-r--r--   0        0        0        0 2024-04-07 19:48:22.511124 libsrg-5.1.1/libsrg/Statistics/UnitTests/__init__.py
--rw-r--r--   0        0        0     5150 2024-04-11 13:46:23.848269 libsrg-5.1.1/libsrg/Statistics/UnitTests/__pycache__/ADStatsBase_test.cpython-311-pytest-7.2.0.pyc
--rw-r--r--   0        0        0     5015 2024-04-24 16:16:17.446580 libsrg-5.1.1/libsrg/Statistics/UnitTests/__pycache__/ADStatsBase_test.cpython-311.pyc
--rw-r--r--   0        0        0     7026 2024-04-17 20:08:12.643029 libsrg-5.1.1/libsrg/Statistics/UnitTests/__pycache__/AnalogStatsBase_test.cpython-311-pytest-7.2.0.pyc
--rw-r--r--   0        0        0     6891 2024-04-24 16:16:17.454580 libsrg-5.1.1/libsrg/Statistics/UnitTests/__pycache__/AnalogStatsBase_test.cpython-311.pyc
--rw-r--r--   0        0        0     5527 2024-04-11 13:56:04.579212 libsrg-5.1.1/libsrg/Statistics/UnitTests/__pycache__/AnalogStatsCumulative_test.cpython-311-pytest-7.2.0.pyc
--rw-r--r--   0        0        0     5392 2024-04-24 16:16:17.459580 libsrg-5.1.1/libsrg/Statistics/UnitTests/__pycache__/AnalogStatsCumulative_test.cpython-311.pyc
--rw-r--r--   0        0        0     9207 2024-04-11 14:18:27.440094 libsrg-5.1.1/libsrg/Statistics/UnitTests/__pycache__/AnalogStatsFading_test.cpython-311-pytest-7.2.0.pyc
--rw-r--r--   0        0        0     9072 2024-04-24 16:16:17.471580 libsrg-5.1.1/libsrg/Statistics/UnitTests/__pycache__/AnalogStatsFading_test.cpython-311.pyc
--rw-r--r--   0        0        0     7000 2024-04-17 20:02:03.807004 libsrg-5.1.1/libsrg/Statistics/UnitTests/__pycache__/AnalogStatsSlidingWindow_test.cpython-311-pytest-7.2.0.pyc
--rw-r--r--   0        0        0     6865 2024-04-24 16:16:17.481580 libsrg-5.1.1/libsrg/Statistics/UnitTests/__pycache__/AnalogStatsSlidingWindow_test.cpython-311.pyc
--rw-r--r--   0        0        0     4310 2024-04-11 13:37:57.025926 libsrg-5.1.1/libsrg/Statistics/UnitTests/__pycache__/DiscteteStatsBase_test.cpython-311-pytest-7.2.0.pyc
--rw-r--r--   0        0        0     4175 2024-04-24 16:16:17.492580 libsrg-5.1.1/libsrg/Statistics/UnitTests/__pycache__/DiscteteStatsBase_test.cpython-311.pyc
--rw-r--r--   0        0        0     6751 2024-04-11 00:45:26.752786 libsrg-5.1.1/libsrg/Statistics/UnitTests/__pycache__/DiscteteStatsSlidingWindow_test.cpython-311-pytest-7.2.0.pyc
--rw-r--r--   0        0        0     6616 2024-04-24 16:16:17.500579 libsrg-5.1.1/libsrg/Statistics/UnitTests/__pycache__/DiscteteStatsSlidingWindow_test.cpython-311.pyc
--rw-r--r--   0        0        0     4185 2024-04-11 13:37:57.059926 libsrg-5.1.1/libsrg/Statistics/UnitTests/__pycache__/RunStatsBase_test.cpython-311-pytest-7.2.0.pyc
--rw-r--r--   0        0        0      182 2024-04-08 17:02:46.936966 libsrg-5.1.1/libsrg/Statistics/UnitTests/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0        0 2024-04-07 19:48:22.512123 libsrg-5.1.1/libsrg/Statistics/__init__.py
--rw-r--r--   0        0        0     7810 2024-04-21 12:42:50.605797 libsrg-5.1.1/libsrg/Statistics/__pycache__/ADStatsBase.cpython-311.pyc
--rw-r--r--   0        0        0     5538 2024-04-11 13:40:23.849156 libsrg-5.1.1/libsrg/Statistics/__pycache__/AnalogStatsBase.cpython-311.pyc
--rw-r--r--   0        0        0     3209 2024-04-08 17:03:01.079883 libsrg-5.1.1/libsrg/Statistics/__pycache__/AnalogStatsCumulative.cpython-311.pyc
--rw-r--r--   0        0        0     4475 2024-04-08 17:03:01.094884 libsrg-5.1.1/libsrg/Statistics/__pycache__/AnalogStatsFading.cpython-311.pyc
--rw-r--r--   0        0        0     3619 2024-04-17 20:02:03.812004 libsrg-5.1.1/libsrg/Statistics/__pycache__/AnalogStatsSlidingWindow.cpython-311.pyc
--rw-r--r--   0        0        0     4439 2024-04-11 13:40:23.886156 libsrg-5.1.1/libsrg/Statistics/__pycache__/DiscreteStatsBase.cpython-311.pyc
--rw-r--r--   0        0        0     2252 2024-04-24 18:48:49.375379 libsrg-5.1.1/libsrg/Statistics/__pycache__/DiscreteStatsCumulative.cpython-311.pyc
--rw-r--r--   0        0        0     3785 2024-04-11 13:37:57.049926 libsrg-5.1.1/libsrg/Statistics/__pycache__/DiscreteStatsSlidingWindow.cpython-311.pyc
--rw-r--r--   0        0        0      172 2024-04-08 17:02:46.932966 libsrg-5.1.1/libsrg/Statistics/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     2222 2024-04-09 15:09:14.520097 libsrg-5.1.1/libsrg/TKGUI/GuiBase.py
--rw-r--r--   0        0        0      448 2024-04-09 15:09:14.568096 libsrg-5.1.1/libsrg/TKGUI/GuiRequest.py
--rw-r--r--   0        0        0     3424 2024-04-09 15:09:14.527097 libsrg-5.1.1/libsrg/TKGUI/GuiRequestQueue.py
--rw-r--r--   0        0        0    10694 2024-04-09 15:09:14.560097 libsrg-5.1.1/libsrg/TKGUI/LoggerGUI.py
--rw-r--r--   0        0        0        1 2023-01-31 17:16:02.479077 libsrg-5.1.1/libsrg/TKGUI/__init__.py
--rw-r--r--   0        0        0     4464 2024-04-24 18:48:47.930388 libsrg-5.1.1/libsrg/TKGUI/__pycache__/GuiBase.cpython-311.pyc
--rw-r--r--   0        0        0     1129 2024-04-24 18:48:47.938388 libsrg-5.1.1/libsrg/TKGUI/__pycache__/GuiRequest.cpython-311.pyc
--rw-r--r--   0        0        0     7736 2024-04-24 18:48:47.949388 libsrg-5.1.1/libsrg/TKGUI/__pycache__/GuiRequestQueue.cpython-311.pyc
--rw-r--r--   0        0        0    21932 2024-04-24 18:48:49.869376 libsrg-5.1.1/libsrg/TKGUI/__pycache__/LoggerGUI.cpython-311.pyc
--rw-r--r--   0        0        0      167 2023-02-05 15:38:41.630152 libsrg-5.1.1/libsrg/TKGUI/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     5498 2024-04-17 20:14:51.866892 libsrg-5.1.1/libsrg/UnitTests/Config_test.py
--rw-r--r--   0        0        0      470 2024-05-06 14:29:21.184142 libsrg-5.1.1/libsrg/UnitTests/Info_test.py
--rw-r--r--   0        0        0     1259 2024-04-17 20:14:51.874892 libsrg-5.1.1/libsrg/UnitTests/RolloverTest_filename.py
--rw-r--r--   0        0        0     1309 2024-04-17 20:14:51.850892 libsrg-5.1.1/libsrg/UnitTests/RolloverTest_logfile.py
--rw-r--r--   0        0        0       33 2024-04-08 13:15:42.414708 libsrg-5.1.1/libsrg/UnitTests/Sample.env
--rw-r--r--   0        0        0       82 2024-04-08 14:36:33.524107 libsrg-5.1.1/libsrg/UnitTests/Sample.ini
--rw-r--r--   0        0        0       60 2024-04-09 14:56:25.134524 libsrg-5.1.1/libsrg/UnitTests/Sample.json
--rw-r--r--   0        0        0        0 2024-05-06 14:46:32.169025 libsrg-5.1.1/libsrg/UnitTests/__init__.py
--rw-r--r--   0        0        0    12397 2024-04-16 16:38:28.280498 libsrg-5.1.1/libsrg/UnitTests/__pycache__/Config_test.cpython-311-pytest-7.2.0.pyc
--rwxr-xr-x   0        0        0      114 2024-05-03 23:47:01.900721 libsrg-5.1.1/libsrg/__init__.py
--rw-r--r--   0        0        0     1168 2024-05-10 00:36:30.486614 libsrg-5.1.1/pyproject.toml
--rw-r--r--   0        0        0     3633 1970-01-01 00:00:00.000000 libsrg-5.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1069 2022-02-24 22:12:03.211633 libsrg-5.2.0/LICENSE.txt
+-rw-r--r--   0        0        0     2620 2024-05-03 23:47:01.671722 libsrg-5.2.0/README.md
+-rw-r--r--   0        0        0     1703 2024-05-18 01:01:00.461508 libsrg-5.2.0/libsrg/AppTemplate.py
+-rw-r--r--   0        0        0    12172 2024-05-18 01:01:00.447508 libsrg-5.2.0/libsrg/Config.py
+-rwxr-xr-x   0        0        0     2842 2024-05-18 01:01:00.459508 libsrg-5.2.0/libsrg/ElapsedTime.py
+-rwxr-xr-x   0        0        0     9552 2024-05-18 01:11:35.933634 libsrg-5.2.0/libsrg/Info.py
+-rwxr-xr-x   0        0        0     4266 2024-05-18 01:01:00.454508 libsrg-5.2.0/libsrg/LevelBanner.py
+-rwxr-xr-x   0        0        0     1753 2024-05-18 01:01:00.444508 libsrg-5.2.0/libsrg/LoggerGUIProxy.py
+-rwxr-xr-x   0        0        0     6374 2024-05-18 01:01:00.442508 libsrg-5.2.0/libsrg/LoggingAppBase.py
+-rwxr-xr-x   0        0        0     8406 2024-05-18 01:01:00.451508 libsrg-5.2.0/libsrg/LoggingCounter.py
+-rwxr-xr-x   0        0        0      832 2024-05-18 01:01:00.431508 libsrg-5.2.0/libsrg/LoggingUtils.py
+-rwxr-xr-x   0        0        0     2093 2024-05-18 01:01:00.439508 libsrg-5.2.0/libsrg/LoggingWatcher.py
+-rwxr-xr-x   0        0        0     3883 2024-05-18 01:01:00.435508 libsrg-5.2.0/libsrg/NagiosBase.py
+-rwxr-xr-x   0        0        0     7448 2024-05-18 01:01:00.456508 libsrg-5.2.0/libsrg/Runner.py
+-rwxr-xr-x   0        0        0     5142 2024-05-18 01:01:00.433508 libsrg-5.2.0/libsrg/Runner2.py
+-rw-r--r--   0        0        0     4762 2024-05-18 01:01:00.503508 libsrg-5.2.0/libsrg/Statistics/ADStatsBase.py
+-rw-r--r--   0        0        0     2514 2024-05-18 01:01:00.501508 libsrg-5.2.0/libsrg/Statistics/AnalogStatsBase.py
+-rw-r--r--   0        0        0     1675 2024-05-18 01:01:00.498508 libsrg-5.2.0/libsrg/Statistics/AnalogStatsCumulative.py
+-rw-r--r--   0        0        0     2541 2024-05-18 01:01:00.486508 libsrg-5.2.0/libsrg/Statistics/AnalogStatsFading.py
+-rw-r--r--   0        0        0     1829 2024-05-18 01:01:00.496508 libsrg-5.2.0/libsrg/Statistics/AnalogStatsSlidingWindow.py
+-rw-r--r--   0        0        0     1832 2024-05-18 01:01:00.494508 libsrg-5.2.0/libsrg/Statistics/DiscreteStatsBase.py
+-rw-r--r--   0        0        0     1013 2024-05-18 01:01:00.492508 libsrg-5.2.0/libsrg/Statistics/DiscreteStatsCumulative.py
+-rw-r--r--   0        0        0     1822 2024-05-18 01:01:00.488508 libsrg-5.2.0/libsrg/Statistics/DiscreteStatsSlidingWindow.py
+-rw-r--r--   0        0        0     2078 2024-05-18 01:01:00.511508 libsrg-5.2.0/libsrg/Statistics/UnitTests/ADStatsBase_test.py
+-rw-r--r--   0        0        0     3023 2024-05-18 01:01:00.514508 libsrg-5.2.0/libsrg/Statistics/UnitTests/AnalogStatsBase_test.py
+-rw-r--r--   0        0        0     2583 2024-05-18 01:01:00.509508 libsrg-5.2.0/libsrg/Statistics/UnitTests/AnalogStatsCumulative_test.py
+-rw-r--r--   0        0        0     4154 2024-05-18 01:01:00.507508 libsrg-5.2.0/libsrg/Statistics/UnitTests/AnalogStatsFading_test.py
+-rw-r--r--   0        0        0     3172 2024-05-18 01:01:00.519508 libsrg-5.2.0/libsrg/Statistics/UnitTests/AnalogStatsSlidingWindow_test.py
+-rw-r--r--   0        0        0     1844 2024-05-18 01:01:00.521508 libsrg-5.2.0/libsrg/Statistics/UnitTests/DiscteteStatsBase_test.py
+-rw-r--r--   0        0        0     2846 2024-05-18 01:01:00.517508 libsrg-5.2.0/libsrg/Statistics/UnitTests/DiscteteStatsSlidingWindow_test.py
+-rw-r--r--   0        0        0      239 2024-05-18 01:01:00.515508 libsrg-5.2.0/libsrg/Statistics/UnitTests/__init__.py
+-rw-r--r--   0        0        0     5150 2024-04-11 13:46:23.848269 libsrg-5.2.0/libsrg/Statistics/UnitTests/__pycache__/ADStatsBase_test.cpython-311-pytest-7.2.0.pyc
+-rw-r--r--   0        0        0     5015 2024-04-24 16:16:17.446580 libsrg-5.2.0/libsrg/Statistics/UnitTests/__pycache__/ADStatsBase_test.cpython-311.pyc
+-rw-r--r--   0        0        0     7026 2024-04-17 20:08:12.643029 libsrg-5.2.0/libsrg/Statistics/UnitTests/__pycache__/AnalogStatsBase_test.cpython-311-pytest-7.2.0.pyc
+-rw-r--r--   0        0        0     6891 2024-04-24 16:16:17.454580 libsrg-5.2.0/libsrg/Statistics/UnitTests/__pycache__/AnalogStatsBase_test.cpython-311.pyc
+-rw-r--r--   0        0        0     5527 2024-04-11 13:56:04.579212 libsrg-5.2.0/libsrg/Statistics/UnitTests/__pycache__/AnalogStatsCumulative_test.cpython-311-pytest-7.2.0.pyc
+-rw-r--r--   0        0        0     5392 2024-04-24 16:16:17.459580 libsrg-5.2.0/libsrg/Statistics/UnitTests/__pycache__/AnalogStatsCumulative_test.cpython-311.pyc
+-rw-r--r--   0        0        0     9207 2024-04-11 14:18:27.440094 libsrg-5.2.0/libsrg/Statistics/UnitTests/__pycache__/AnalogStatsFading_test.cpython-311-pytest-7.2.0.pyc
+-rw-r--r--   0        0        0     9072 2024-04-24 16:16:17.471580 libsrg-5.2.0/libsrg/Statistics/UnitTests/__pycache__/AnalogStatsFading_test.cpython-311.pyc
+-rw-r--r--   0        0        0     7000 2024-04-17 20:02:03.807004 libsrg-5.2.0/libsrg/Statistics/UnitTests/__pycache__/AnalogStatsSlidingWindow_test.cpython-311-pytest-7.2.0.pyc
+-rw-r--r--   0        0        0     6865 2024-04-24 16:16:17.481580 libsrg-5.2.0/libsrg/Statistics/UnitTests/__pycache__/AnalogStatsSlidingWindow_test.cpython-311.pyc
+-rw-r--r--   0        0        0     4310 2024-04-11 13:37:57.025926 libsrg-5.2.0/libsrg/Statistics/UnitTests/__pycache__/DiscteteStatsBase_test.cpython-311-pytest-7.2.0.pyc
+-rw-r--r--   0        0        0     4175 2024-04-24 16:16:17.492580 libsrg-5.2.0/libsrg/Statistics/UnitTests/__pycache__/DiscteteStatsBase_test.cpython-311.pyc
+-rw-r--r--   0        0        0     6751 2024-04-11 00:45:26.752786 libsrg-5.2.0/libsrg/Statistics/UnitTests/__pycache__/DiscteteStatsSlidingWindow_test.cpython-311-pytest-7.2.0.pyc
+-rw-r--r--   0        0        0     6616 2024-04-24 16:16:17.500579 libsrg-5.2.0/libsrg/Statistics/UnitTests/__pycache__/DiscteteStatsSlidingWindow_test.cpython-311.pyc
+-rw-r--r--   0        0        0     4185 2024-04-11 13:37:57.059926 libsrg-5.2.0/libsrg/Statistics/UnitTests/__pycache__/RunStatsBase_test.cpython-311-pytest-7.2.0.pyc
+-rw-r--r--   0        0        0      182 2024-04-08 17:02:46.936966 libsrg-5.2.0/libsrg/Statistics/UnitTests/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0      239 2024-05-18 01:01:00.490508 libsrg-5.2.0/libsrg/Statistics/__init__.py
+-rw-r--r--   0        0        0     7810 2024-04-21 12:42:50.605797 libsrg-5.2.0/libsrg/Statistics/__pycache__/ADStatsBase.cpython-311.pyc
+-rw-r--r--   0        0        0     5538 2024-04-11 13:40:23.849156 libsrg-5.2.0/libsrg/Statistics/__pycache__/AnalogStatsBase.cpython-311.pyc
+-rw-r--r--   0        0        0     3209 2024-04-08 17:03:01.079883 libsrg-5.2.0/libsrg/Statistics/__pycache__/AnalogStatsCumulative.cpython-311.pyc
+-rw-r--r--   0        0        0     4475 2024-04-08 17:03:01.094884 libsrg-5.2.0/libsrg/Statistics/__pycache__/AnalogStatsFading.cpython-311.pyc
+-rw-r--r--   0        0        0     3619 2024-04-17 20:02:03.812004 libsrg-5.2.0/libsrg/Statistics/__pycache__/AnalogStatsSlidingWindow.cpython-311.pyc
+-rw-r--r--   0        0        0     4439 2024-04-11 13:40:23.886156 libsrg-5.2.0/libsrg/Statistics/__pycache__/DiscreteStatsBase.cpython-311.pyc
+-rw-r--r--   0        0        0     2252 2024-04-24 18:48:49.375379 libsrg-5.2.0/libsrg/Statistics/__pycache__/DiscreteStatsCumulative.cpython-311.pyc
+-rw-r--r--   0        0        0     3785 2024-04-11 13:37:57.049926 libsrg-5.2.0/libsrg/Statistics/__pycache__/DiscreteStatsSlidingWindow.cpython-311.pyc
+-rw-r--r--   0        0        0      172 2024-04-08 17:02:46.932966 libsrg-5.2.0/libsrg/Statistics/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     2461 2024-05-18 01:01:00.535508 libsrg-5.2.0/libsrg/TKGUI/GuiBase.py
+-rw-r--r--   0        0        0      687 2024-05-18 01:01:00.533508 libsrg-5.2.0/libsrg/TKGUI/GuiRequest.py
+-rw-r--r--   0        0        0     3663 2024-05-18 01:01:00.537508 libsrg-5.2.0/libsrg/TKGUI/GuiRequestQueue.py
+-rw-r--r--   0        0        0    10933 2024-05-18 01:01:00.539508 libsrg-5.2.0/libsrg/TKGUI/LoggerGUI.py
+-rw-r--r--   0        0        0      239 2024-05-18 01:01:00.531508 libsrg-5.2.0/libsrg/TKGUI/__init__.py
+-rw-r--r--   0        0        0     4464 2024-04-24 18:48:47.930388 libsrg-5.2.0/libsrg/TKGUI/__pycache__/GuiBase.cpython-311.pyc
+-rw-r--r--   0        0        0     1129 2024-04-24 18:48:47.938388 libsrg-5.2.0/libsrg/TKGUI/__pycache__/GuiRequest.cpython-311.pyc
+-rw-r--r--   0        0        0     7736 2024-04-24 18:48:47.949388 libsrg-5.2.0/libsrg/TKGUI/__pycache__/GuiRequestQueue.cpython-311.pyc
+-rw-r--r--   0        0        0    21932 2024-04-24 18:48:49.869376 libsrg-5.2.0/libsrg/TKGUI/__pycache__/LoggerGUI.cpython-311.pyc
+-rw-r--r--   0        0        0      167 2023-02-05 15:38:41.630152 libsrg-5.2.0/libsrg/TKGUI/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     5737 2024-05-18 01:01:00.472508 libsrg-5.2.0/libsrg/UnitTests/Config_test.py
+-rw-r--r--   0        0        0      709 2024-05-18 01:01:00.464508 libsrg-5.2.0/libsrg/UnitTests/Info_test.py
+-rw-r--r--   0        0        0     1497 2024-05-18 01:01:00.468508 libsrg-5.2.0/libsrg/UnitTests/RolloverTest_filename.py
+-rw-r--r--   0        0        0     1547 2024-05-18 01:01:00.466508 libsrg-5.2.0/libsrg/UnitTests/RolloverTest_logfile.py
+-rw-r--r--   0        0        0       33 2024-04-08 13:15:42.414708 libsrg-5.2.0/libsrg/UnitTests/Sample.env
+-rw-r--r--   0        0        0       82 2024-04-08 14:36:33.524107 libsrg-5.2.0/libsrg/UnitTests/Sample.ini
+-rw-r--r--   0        0        0       60 2024-04-09 14:56:25.134524 libsrg-5.2.0/libsrg/UnitTests/Sample.json
+-rw-r--r--   0        0        0      239 2024-05-18 01:01:00.470508 libsrg-5.2.0/libsrg/UnitTests/__init__.py
+-rw-r--r--   0        0        0    12397 2024-04-16 16:38:28.280498 libsrg-5.2.0/libsrg/UnitTests/__pycache__/Config_test.cpython-311-pytest-7.2.0.pyc
+-rwxr-xr-x   0        0        0      353 2024-05-18 01:01:00.437508 libsrg-5.2.0/libsrg/__init__.py
+-rw-r--r--   0        0        0     1168 2024-05-18 01:11:45.989573 libsrg-5.2.0/pyproject.toml
+-rw-r--r--   0        0        0     3633 1970-01-01 00:00:00.000000 libsrg-5.2.0/PKG-INFO
```

### Comparing `libsrg-5.1.1/LICENSE.txt` & `libsrg-5.2.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `libsrg-5.1.1/README.md` & `libsrg-5.2.0/README.md`

 * *Files identical despite different names*

### Comparing `libsrg-5.1.1/libsrg/AppTemplate.py` & `libsrg-5.2.0/libsrg/AppTemplate.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+# libsrg (Code and Documentation) is published under an MIT License
+# Copyright (c) 2023,2024 Steven Goncalo
+# The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
+
 # 2024 Steven Goncalo
 import logging
 
 from libsrg.LoggingAppBase import LoggingAppBase
 
 """
 This module is a sample application template for libsrg application logging
```

### Comparing `libsrg-5.1.1/libsrg/Config.py` & `libsrg-5.2.0/libsrg/Config.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+# libsrg (Code and Documentation) is published under an MIT License
+# Copyright (c) 2023,2024 Steven Goncalo
+# The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
+
 import configparser
 import json
 import os
 import re
 from collections import ChainMap
 from pathlib import Path
 from typing import Any, Optional, Tuple, Union
```

### Comparing `libsrg-5.1.1/libsrg/ElapsedTime.py` & `libsrg-5.2.0/libsrg/ElapsedTime.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+# libsrg (Code and Documentation) is published under an MIT License
+# Copyright (c) 2023,2024 Steven Goncalo
+# The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
+
 # 2024 Steven Goncalo
 """
 ElapsedTime is a class to measure elapsed time between start and stop events.
 It can be operated directly using start and stop methods, or it can
 act as a context manager in a "with" statement block.
 """
 import logging
```

### Comparing `libsrg-5.1.1/libsrg/Info.py` & `libsrg-5.2.0/libsrg/Info.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,12 @@
 #! /usr/bin/env python3
+# libsrg (Code and Documentation) is published under an MIT License
+# Copyright (c) 2023,2024 Steven Goncalo
+# The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
+
 # 2024 Steven Goncalo
 import configparser
 import logging
 import os
 import platform
 import sys
 from importlib.metadata import version
@@ -87,14 +91,17 @@
 
         rm = Runner("uname -m", userat=self.userat, rethrow=True, timeout=timeout, throw=True, retries=retries)
         self.machine = rm.so_lines[-1]
 
         rk = Runner("uname -r", userat=self.userat, rethrow=True, timeout=timeout, throw=True, retries=retries)
         self.kernel = rk.so_lines[-1]
 
+        rs = Runner("uname -s", userat=self.userat, rethrow=True, timeout=timeout, throw=True, retries=retries)
+        self.kernel_name = rs.so_lines[-1]
+
         rfqdn = Runner("hostname -f", userat=self.userat, rethrow=True, timeout=timeout, throw=True, retries=retries)
         self.fqdn = rfqdn.so_lines[-1]
 
         rshort = Runner("hostname -s", userat=self.userat, rethrow=True, timeout=timeout, throw=True, retries=retries)
         self.short = rshort.so_lines[-1]
 
         rip = Runner("hostname -i", userat=self.userat, rethrow=True, timeout=timeout, throw=True, retries=retries)
@@ -172,14 +179,21 @@
     def is_root(self) -> bool:
         """
         Checks if the user calling Info is root or not.
         :return: true if the user calling Info is root
         """
         return self.uid == 0
 
+    def is_linux(self) -> bool:
+        """
+        Checks if uname -s reported Linux.
+        :return: true if the system is Linux
+        """
+        return self.kernel_name == "Linux"
+
     def exit_if_not_root(self):
         """
         Checks if the user calling Info is root and calls exit if not root.
         :return: None or exit without explicit return
         """
         if not self.is_root():
             self.logger.critical("Must run as root, uid={self.uid}, hostname={self.hostname}")
```

### Comparing `libsrg-5.1.1/libsrg/LevelBanner.py` & `libsrg-5.2.0/libsrg/LevelBanner.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,12 @@
 #!/usr/bin/env  python3
+# libsrg (Code and Documentation) is published under an MIT License
+# Copyright (c) 2023,2024 Steven Goncalo
+# The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
+
 # 2024 Steven Goncalo
 
 import logging
 
 from libsrg.LoggingUtils import level2int
 from libsrg.Runner import Runner
```

### Comparing `libsrg-5.1.1/libsrg/LoggerGUIProxy.py` & `libsrg-5.2.0/libsrg/LoggerGUIProxy.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+# libsrg (Code and Documentation) is published under an MIT License
+# Copyright (c) 2023,2024 Steven Goncalo
+# The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
+
 # 2024 Steven Goncalo
 import logging
 
 GUI_NEW_LINE = "GUI_NEW_LINE"
 GUI_FREEZE_LINE = "GUI_FREEZE_LINE"
 GUI_CONFIGURE = "GUI_CONFIGURE"
```

### Comparing `libsrg-5.1.1/libsrg/LoggingAppBase.py` & `libsrg-5.2.0/libsrg/LoggingAppBase.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,12 @@
 #!/usr/bin/env  python3
+# libsrg (Code and Documentation) is published under an MIT License
+# Copyright (c) 2023,2024 Steven Goncalo
+# The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
+
 # 2024 Steven Goncalo
 
 import argparse
 import logging
 from importlib.metadata import version
 from typing import Optional
```

### Comparing `libsrg-5.1.1/libsrg/LoggingCounter.py` & `libsrg-5.2.0/libsrg/LoggingCounter.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,12 @@
 #!/usr/bin/env  python3
+# libsrg (Code and Documentation) is published under an MIT License
+# Copyright (c) 2023,2024 Steven Goncalo
+# The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
+
 # 2024 Steven Goncalo
 
 import atexit
 import logging
 import sys
 import time
 from collections import Counter
```

### Comparing `libsrg-5.1.1/libsrg/LoggingWatcher.py` & `libsrg-5.2.0/libsrg/LoggingWatcher.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,8 +1,12 @@
 #!/usr/bin/env  python3
+# libsrg (Code and Documentation) is published under an MIT License
+# Copyright (c) 2023,2024 Steven Goncalo
+# The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
+
 # 2024 Steven Goncalo
 
 import logging
 from queue import Queue
 
 log = logging.getLogger("libsrg.LoggingWatcher")
```

### Comparing `libsrg-5.1.1/libsrg/NagiosBase.py` & `libsrg-5.2.0/libsrg/NagiosBase.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,12 @@
 #!/usr/bin/env  python3
+# libsrg (Code and Documentation) is published under an MIT License
+# Copyright (c) 2023,2024 Steven Goncalo
+# The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
+
 # 2024 Steven Goncalo
 
 # from optparse import OptionParser
 import sys
 from enum import Enum
 
 from libsrg.LoggingAppBase import LoggingAppBase
```

### Comparing `libsrg-5.1.1/libsrg/Runner.py` & `libsrg-5.2.0/libsrg/Runner.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+# libsrg (Code and Documentation) is published under an MIT License
+# Copyright (c) 2023,2024 Steven Goncalo
+# The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
+
 # 2024 Steven Goncalo
 """
 Module before includes
 """
 import logging
 import os
 import subprocess
```

### Comparing `libsrg-5.1.1/libsrg/Runner2.py` & `libsrg-5.2.0/libsrg/Runner2.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+# libsrg (Code and Documentation) is published under an MIT License
+# Copyright (c) 2023,2024 Steven Goncalo
+# The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
+
 # 2024 Steven Goncalo
 import logging
 import subprocess
 from typing import List, Optional, Union
 
 from libsrg.LoggingAppBase import LoggingAppBase
```

### Comparing `libsrg-5.1.1/libsrg/Statistics/ADStatsBase.py` & `libsrg-5.2.0/libsrg/Statistics/ADStatsBase.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+# libsrg (Code and Documentation) is published under an MIT License
+# Copyright (c) 2023,2024 Steven Goncalo
+# The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
+
 from abc import ABC, abstractmethod
 from dataclasses import dataclass
 from time import time
 from typing import Optional, Callable, Any
 
 
 @dataclass
```

### Comparing `libsrg-5.1.1/libsrg/Statistics/AnalogStatsBase.py` & `libsrg-5.2.0/libsrg/Statistics/AnalogStatsBase.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+# libsrg (Code and Documentation) is published under an MIT License
+# Copyright (c) 2023,2024 Steven Goncalo
+# The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
+
 import math
 from abc import ABC, abstractmethod
 from dataclasses import dataclass
 from typing import Optional, Callable, Any
 
 from libsrg.Statistics.ADStatsBase import ADStatsBase, ADStatsRecord
```

### Comparing `libsrg-5.1.1/libsrg/Statistics/AnalogStatsFading.py` & `libsrg-5.2.0/libsrg/Statistics/AnalogStatsFading.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+# libsrg (Code and Documentation) is published under an MIT License
+# Copyright (c) 2023,2024 Steven Goncalo
+# The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
+
 import math
 from typing import Optional, Callable
 
 from libsrg.Statistics.AnalogStatsBase import AnalogStatsBase
 
 
 class AnalogStatsFading(AnalogStatsBase):
```

### Comparing `libsrg-5.1.1/libsrg/Statistics/AnalogStatsSlidingWindow.py` & `libsrg-5.2.0/libsrg/Statistics/AnalogStatsSlidingWindow.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+# libsrg (Code and Documentation) is published under an MIT License
+# Copyright (c) 2023,2024 Steven Goncalo
+# The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
+
 from typing import Optional, Callable
 
 from libsrg.Statistics.AnalogStatsCumulative import AnalogStatsCumulative
 
 
 class AnalogStatsSlidingWindow(AnalogStatsCumulative):
```

### Comparing `libsrg-5.1.1/libsrg/Statistics/DiscreteStatsBase.py` & `libsrg-5.2.0/libsrg/Statistics/DiscreteStatsBase.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+# libsrg (Code and Documentation) is published under an MIT License
+# Copyright (c) 2023,2024 Steven Goncalo
+# The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
+
 from collections import Counter
 from dataclasses import dataclass
 from typing import Optional, Callable, Any
 
 from libsrg.Statistics.ADStatsBase import ADStatsBase, ADStatsRecord
```

### Comparing `libsrg-5.1.1/libsrg/Statistics/DiscreteStatsSlidingWindow.py` & `libsrg-5.2.0/libsrg/Statistics/DiscreteStatsSlidingWindow.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+# libsrg (Code and Documentation) is published under an MIT License
+# Copyright (c) 2023,2024 Steven Goncalo
+# The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
+
 from typing import Optional, Callable, Any
 
 from libsrg.Statistics.DiscreteStatsBase import DiscreteStatsBase
 
 
 class DiscreteStatsSlidingWindow(DiscreteStatsBase):
     class_callbacks: list[Callable] = []
```

### Comparing `libsrg-5.1.1/libsrg/Statistics/UnitTests/ADStatsBase_test.py` & `libsrg-5.2.0/libsrg/Statistics/UnitTests/ADStatsBase_test.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+# libsrg (Code and Documentation) is published under an MIT License
+# Copyright (c) 2023,2024 Steven Goncalo
+# The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
+
 import unittest
 from dataclasses import dataclass
 from typing import Optional, Callable, Any
 
 from libsrg.Statistics.ADStatsBase import ADStatsBase, ADStatsRecord
```

### Comparing `libsrg-5.1.1/libsrg/Statistics/UnitTests/AnalogStatsBase_test.py` & `libsrg-5.2.0/libsrg/Statistics/UnitTests/AnalogStatsBase_test.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+# libsrg (Code and Documentation) is published under an MIT License
+# Copyright (c) 2023,2024 Steven Goncalo
+# The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
+
 import unittest
 from typing import Any
 
 from libsrg.Statistics.AnalogStatsBase import AnalogStatsBase
 from libsrg.Statistics.ADStatsBase import ADStatsBase, ADStatsRecord
```

### Comparing `libsrg-5.1.1/libsrg/Statistics/UnitTests/AnalogStatsCumulative_test.py` & `libsrg-5.2.0/libsrg/Statistics/UnitTests/AnalogStatsCumulative_test.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+# libsrg (Code and Documentation) is published under an MIT License
+# Copyright (c) 2023,2024 Steven Goncalo
+# The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
+
 import random
 import unittest
 from time import time, ctime
 
 from libsrg.Statistics.AnalogStatsBase import AStatsRecord
 from libsrg.Statistics.AnalogStatsCumulative import AnalogStatsCumulative
```

### Comparing `libsrg-5.1.1/libsrg/Statistics/UnitTests/AnalogStatsFading_test.py` & `libsrg-5.2.0/libsrg/Statistics/UnitTests/AnalogStatsFading_test.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+# libsrg (Code and Documentation) is published under an MIT License
+# Copyright (c) 2023,2024 Steven Goncalo
+# The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
+
 import random
 import unittest
 from time import time
 
 from libsrg.Statistics.AnalogStatsBase import AStatsRecord
 from libsrg.Statistics.AnalogStatsCumulative import AnalogStatsCumulative
 from libsrg.Statistics.AnalogStatsFading import AnalogStatsFading
```

### Comparing `libsrg-5.1.1/libsrg/Statistics/UnitTests/AnalogStatsSlidingWindow_test.py` & `libsrg-5.2.0/libsrg/Statistics/UnitTests/AnalogStatsSlidingWindow_test.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+# libsrg (Code and Documentation) is published under an MIT License
+# Copyright (c) 2023,2024 Steven Goncalo
+# The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
+
 import math
 import random
 import unittest
 from time import time, ctime
 
 from libsrg.Statistics.AnalogStatsBase import AStatsRecord
 from libsrg.Statistics.AnalogStatsSlidingWindow import AnalogStatsSlidingWindow
```

### Comparing `libsrg-5.1.1/libsrg/Statistics/UnitTests/DiscteteStatsSlidingWindow_test.py` & `libsrg-5.2.0/libsrg/Statistics/UnitTests/DiscteteStatsSlidingWindow_test.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+# libsrg (Code and Documentation) is published under an MIT License
+# Copyright (c) 2023,2024 Steven Goncalo
+# The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
+
 import unittest
 
 from enum import Enum
 from libsrg.Statistics.DiscreteStatsSlidingWindow import DiscreteStatsSlidingWindow
 
 
 class Status(Enum):
```

### Comparing `libsrg-5.1.1/libsrg/Statistics/UnitTests/__pycache__/ADStatsBase_test.cpython-311-pytest-7.2.0.pyc` & `libsrg-5.2.0/libsrg/Statistics/UnitTests/__pycache__/ADStatsBase_test.cpython-311-pytest-7.2.0.pyc`

 * *Files identical despite different names*

### Comparing `libsrg-5.1.1/libsrg/Statistics/UnitTests/__pycache__/ADStatsBase_test.cpython-311.pyc` & `libsrg-5.2.0/libsrg/Statistics/UnitTests/__pycache__/ADStatsBase_test.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `libsrg-5.1.1/libsrg/Statistics/UnitTests/__pycache__/AnalogStatsBase_test.cpython-311-pytest-7.2.0.pyc` & `libsrg-5.2.0/libsrg/Statistics/UnitTests/__pycache__/AnalogStatsBase_test.cpython-311-pytest-7.2.0.pyc`

 * *Files identical despite different names*

### Comparing `libsrg-5.1.1/libsrg/Statistics/UnitTests/__pycache__/AnalogStatsBase_test.cpython-311.pyc` & `libsrg-5.2.0/libsrg/Statistics/UnitTests/__pycache__/AnalogStatsBase_test.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `libsrg-5.1.1/libsrg/Statistics/UnitTests/__pycache__/AnalogStatsCumulative_test.cpython-311-pytest-7.2.0.pyc` & `libsrg-5.2.0/libsrg/Statistics/UnitTests/__pycache__/AnalogStatsCumulative_test.cpython-311-pytest-7.2.0.pyc`

 * *Files identical despite different names*

### Comparing `libsrg-5.1.1/libsrg/Statistics/UnitTests/__pycache__/AnalogStatsCumulative_test.cpython-311.pyc` & `libsrg-5.2.0/libsrg/Statistics/UnitTests/__pycache__/AnalogStatsCumulative_test.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `libsrg-5.1.1/libsrg/Statistics/UnitTests/__pycache__/AnalogStatsFading_test.cpython-311-pytest-7.2.0.pyc` & `libsrg-5.2.0/libsrg/Statistics/UnitTests/__pycache__/AnalogStatsFading_test.cpython-311-pytest-7.2.0.pyc`

 * *Files identical despite different names*

### Comparing `libsrg-5.1.1/libsrg/Statistics/UnitTests/__pycache__/AnalogStatsFading_test.cpython-311.pyc` & `libsrg-5.2.0/libsrg/Statistics/UnitTests/__pycache__/AnalogStatsFading_test.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `libsrg-5.1.1/libsrg/Statistics/UnitTests/__pycache__/AnalogStatsSlidingWindow_test.cpython-311-pytest-7.2.0.pyc` & `libsrg-5.2.0/libsrg/Statistics/UnitTests/__pycache__/AnalogStatsSlidingWindow_test.cpython-311-pytest-7.2.0.pyc`

 * *Files identical despite different names*

### Comparing `libsrg-5.1.1/libsrg/Statistics/UnitTests/__pycache__/AnalogStatsSlidingWindow_test.cpython-311.pyc` & `libsrg-5.2.0/libsrg/Statistics/UnitTests/__pycache__/AnalogStatsSlidingWindow_test.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `libsrg-5.1.1/libsrg/Statistics/UnitTests/__pycache__/DiscteteStatsBase_test.cpython-311-pytest-7.2.0.pyc` & `libsrg-5.2.0/libsrg/Statistics/UnitTests/__pycache__/DiscteteStatsBase_test.cpython-311-pytest-7.2.0.pyc`

 * *Files identical despite different names*

### Comparing `libsrg-5.1.1/libsrg/Statistics/UnitTests/__pycache__/DiscteteStatsBase_test.cpython-311.pyc` & `libsrg-5.2.0/libsrg/Statistics/UnitTests/__pycache__/DiscteteStatsBase_test.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `libsrg-5.1.1/libsrg/Statistics/UnitTests/__pycache__/DiscteteStatsSlidingWindow_test.cpython-311-pytest-7.2.0.pyc` & `libsrg-5.2.0/libsrg/Statistics/UnitTests/__pycache__/DiscteteStatsSlidingWindow_test.cpython-311-pytest-7.2.0.pyc`

 * *Files identical despite different names*

### Comparing `libsrg-5.1.1/libsrg/Statistics/UnitTests/__pycache__/DiscteteStatsSlidingWindow_test.cpython-311.pyc` & `libsrg-5.2.0/libsrg/Statistics/UnitTests/__pycache__/DiscteteStatsSlidingWindow_test.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `libsrg-5.1.1/libsrg/Statistics/UnitTests/__pycache__/RunStatsBase_test.cpython-311-pytest-7.2.0.pyc` & `libsrg-5.2.0/libsrg/Statistics/UnitTests/__pycache__/RunStatsBase_test.cpython-311-pytest-7.2.0.pyc`

 * *Files identical despite different names*

### Comparing `libsrg-5.1.1/libsrg/Statistics/__pycache__/ADStatsBase.cpython-311.pyc` & `libsrg-5.2.0/libsrg/Statistics/__pycache__/ADStatsBase.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `libsrg-5.1.1/libsrg/Statistics/__pycache__/AnalogStatsBase.cpython-311.pyc` & `libsrg-5.2.0/libsrg/Statistics/__pycache__/AnalogStatsBase.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `libsrg-5.1.1/libsrg/Statistics/__pycache__/AnalogStatsCumulative.cpython-311.pyc` & `libsrg-5.2.0/libsrg/Statistics/__pycache__/AnalogStatsCumulative.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `libsrg-5.1.1/libsrg/Statistics/__pycache__/AnalogStatsFading.cpython-311.pyc` & `libsrg-5.2.0/libsrg/Statistics/__pycache__/AnalogStatsFading.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `libsrg-5.1.1/libsrg/Statistics/__pycache__/AnalogStatsSlidingWindow.cpython-311.pyc` & `libsrg-5.2.0/libsrg/Statistics/__pycache__/AnalogStatsSlidingWindow.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `libsrg-5.1.1/libsrg/Statistics/__pycache__/DiscreteStatsBase.cpython-311.pyc` & `libsrg-5.2.0/libsrg/Statistics/__pycache__/DiscreteStatsBase.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `libsrg-5.1.1/libsrg/Statistics/__pycache__/DiscreteStatsCumulative.cpython-311.pyc` & `libsrg-5.2.0/libsrg/Statistics/__pycache__/DiscreteStatsCumulative.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `libsrg-5.1.1/libsrg/Statistics/__pycache__/DiscreteStatsSlidingWindow.cpython-311.pyc` & `libsrg-5.2.0/libsrg/Statistics/__pycache__/DiscreteStatsSlidingWindow.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `libsrg-5.1.1/libsrg/TKGUI/GuiBase.py` & `libsrg-5.2.0/libsrg/TKGUI/GuiBase.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+# libsrg (Code and Documentation) is published under an MIT License
+# Copyright (c) 2023,2024 Steven Goncalo
+# The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
+
 import logging
 import sys
 import threading
 import tkinter as tk
 from pathlib import Path
 
 from libsrg.LoggingAppBase import LoggingAppBase
```

### Comparing `libsrg-5.1.1/libsrg/TKGUI/GuiRequestQueue.py` & `libsrg-5.2.0/libsrg/TKGUI/GuiRequestQueue.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+# libsrg (Code and Documentation) is published under an MIT License
+# Copyright (c) 2023,2024 Steven Goncalo
+# The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
+
 import logging
 import queue
 import random
 import tkinter as tk
 from tkinter import ttk
 
 from libsrg.TKGUI.GuiRequest import GuiRequest
```

### Comparing `libsrg-5.1.1/libsrg/TKGUI/LoggerGUI.py` & `libsrg-5.2.0/libsrg/TKGUI/LoggerGUI.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+# libsrg (Code and Documentation) is published under an MIT License
+# Copyright (c) 2023,2024 Steven Goncalo
+# The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
+
 import logging
 import sys
 import threading
 import tkinter as tk
 from collections import Counter
 from concurrent.futures import ThreadPoolExecutor
 from logging import LogRecord
```

### Comparing `libsrg-5.1.1/libsrg/TKGUI/__pycache__/GuiBase.cpython-311.pyc` & `libsrg-5.2.0/libsrg/TKGUI/__pycache__/GuiBase.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `libsrg-5.1.1/libsrg/TKGUI/__pycache__/GuiRequest.cpython-311.pyc` & `libsrg-5.2.0/libsrg/TKGUI/__pycache__/GuiRequest.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `libsrg-5.1.1/libsrg/TKGUI/__pycache__/GuiRequestQueue.cpython-311.pyc` & `libsrg-5.2.0/libsrg/TKGUI/__pycache__/GuiRequestQueue.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `libsrg-5.1.1/libsrg/TKGUI/__pycache__/LoggerGUI.cpython-311.pyc` & `libsrg-5.2.0/libsrg/TKGUI/__pycache__/LoggerGUI.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `libsrg-5.1.1/libsrg/UnitTests/Config_test.py` & `libsrg-5.2.0/libsrg/UnitTests/Config_test.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+# libsrg (Code and Documentation) is published under an MIT License
+# Copyright (c) 2023,2024 Steven Goncalo
+# The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
+
 import unittest
 from collections import ChainMap
 from pathlib import Path
 
 from libsrg.Config import Config
 
 dir_path: Path = Path(__file__).parent
```

### Comparing `libsrg-5.1.1/libsrg/UnitTests/RolloverTest_logfile.py` & `libsrg-5.2.0/libsrg/UnitTests/RolloverTest_logfile.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,11 @@
 #!/usr/bin/env  python3
+# libsrg (Code and Documentation) is published under an MIT License
+# Copyright (c) 2023,2024 Steven Goncalo
+# The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
 
 import os
 from pathlib import Path
 
 from libsrg.LoggingAppBase import LoggingAppBase
 from libsrg.LoggingCounter import LoggingCounter
 from libsrg.Runner import Runner
```

### Comparing `libsrg-5.1.1/libsrg/UnitTests/__pycache__/Config_test.cpython-311-pytest-7.2.0.pyc` & `libsrg-5.2.0/libsrg/UnitTests/__pycache__/Config_test.cpython-311-pytest-7.2.0.pyc`

 * *Files identical despite different names*

### Comparing `libsrg-5.1.1/pyproject.toml` & `libsrg-5.2.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "libsrg"
-version = "5.1.1"
+version = "5.2.0"
 description = "Utility lib logging, statistics, subprocesses"
 authors = ["Steve Goncalo <steven@goncalo.us>"]
 readme = "README.md"
 classifiers = [
     "Programming Language :: Python :: 3.9",
     "Development Status :: 5 - Production/Stable",
     "License :: OSI Approved :: MIT License",
```

### Comparing `libsrg-5.1.1/PKG-INFO` & `libsrg-5.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: libsrg
-Version: 5.1.1
+Version: 5.2.0
 Summary: Utility lib logging, statistics, subprocesses
 Author: Steve Goncalo
 Author-email: steven@goncalo.us
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

