# Comparing `tmp/lettrade-0.0.1.tar.gz` & `tmp/lettrade-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lettrade-0.0.1.tar", last modified: Sat Apr 27 15:32:40 2024, max compression
+gzip compressed data, was "lettrade-0.0.2.tar", last modified: Sat May 18 08:33:31 2024, max compression
```

## Comparing `lettrade-0.0.1.tar` & `lettrade-0.0.2.tar`

### file list

```diff
@@ -1,57 +1,77 @@
-drwxrwxrwx   0 m3        (1000) root         (0)        0 2024-04-27 15:32:40.178179 lettrade-0.0.1/
--rwxrwxrwx   0 m3        (1000) root         (0)    34523 2024-04-26 01:41:03.000000 lettrade-0.0.1/LICENSE
--rwxrwxrwx   0 m3        (1000) root         (0)     1844 2024-04-27 15:32:40.177614 lettrade-0.0.1/PKG-INFO
--rwxrwxrwx   0 m3        (1000) root         (0)     1119 2024-04-27 08:23:50.000000 lettrade-0.0.1/README.md
-drwxrwxrwx   0 m3        (1000) root         (0)        0 2024-04-27 15:32:40.146695 lettrade-0.0.1/lettrade/
-drwxrwxrwx   0 m3        (1000) root         (0)        0 2024-04-27 15:32:40.149838 lettrade-0.0.1/lettrade/base/
--rwxrwxrwx   0 m3        (1000) root         (0)       32 2024-04-27 07:43:15.000000 lettrade-0.0.1/lettrade/base/__init__.py
--rwxrwxrwx   0 m3        (1000) root         (0)      268 2024-04-27 07:51:29.000000 lettrade-0.0.1/lettrade/base/feed.py
-drwxrwxrwx   0 m3        (1000) root         (0)        0 2024-04-27 15:32:40.152047 lettrade-0.0.1/lettrade/brain/
--rwxrwxrwx   0 m3        (1000) root         (0)       25 2024-04-26 04:37:23.000000 lettrade-0.0.1/lettrade/brain/__init__.py
--rwxrwxrwx   0 m3        (1000) root         (0)    32415 2024-04-26 04:26:51.000000 lettrade-0.0.1/lettrade/brain/backtest.py
--rwxrwxrwx   0 m3        (1000) root         (0)     1343 2024-04-27 09:52:20.000000 lettrade-0.0.1/lettrade/brain/brain.py
-drwxrwxrwx   0 m3        (1000) root         (0)        0 2024-04-27 15:32:40.154066 lettrade-0.0.1/lettrade/commission/
--rwxrwxrwx   0 m3        (1000) root         (0)       70 2024-04-26 02:51:07.000000 lettrade-0.0.1/lettrade/commission/__init__.py
--rwxrwxrwx   0 m3        (1000) root         (0)      532 2024-04-26 02:55:18.000000 lettrade-0.0.1/lettrade/commission/commission.py
--rwxrwxrwx   0 m3        (1000) root         (0)      373 2024-04-26 02:50:42.000000 lettrade-0.0.1/lettrade/commission/forex.py
-drwxrwxrwx   0 m3        (1000) root         (0)        0 2024-04-27 15:32:40.158061 lettrade-0.0.1/lettrade/data/
--rwxrwxrwx   0 m3        (1000) root         (0)       87 2024-04-26 06:54:51.000000 lettrade-0.0.1/lettrade/data/__init__.py
--rwxrwxrwx   0 m3        (1000) root         (0)      335 2024-04-27 02:15:03.000000 lettrade-0.0.1/lettrade/data/csv.py
--rwxrwxrwx   0 m3        (1000) root         (0)      860 2024-04-27 11:04:27.000000 lettrade-0.0.1/lettrade/data/data.py
--rwxrwxrwx   0 m3        (1000) root         (0)      552 2024-04-27 10:26:35.000000 lettrade-0.0.1/lettrade/data/feeder.py
--rwxrwxrwx   0 m3        (1000) root         (0)        0 2024-04-26 05:17:01.000000 lettrade-0.0.1/lettrade/data/pickle.py
--rwxrwxrwx   0 m3        (1000) root         (0)        0 2024-04-26 02:43:25.000000 lettrade-0.0.1/lettrade/data/replay.py
-drwxrwxrwx   0 m3        (1000) root         (0)        0 2024-04-27 15:32:40.159546 lettrade-0.0.1/lettrade/exchange/
--rwxrwxrwx   0 m3        (1000) root         (0)       31 2024-04-26 04:58:02.000000 lettrade-0.0.1/lettrade/exchange/__init__.py
-drwxrwxrwx   0 m3        (1000) root         (0)        0 2024-04-27 15:32:40.162800 lettrade-0.0.1/lettrade/exchange/backtest/
--rwxrwxrwx   0 m3        (1000) root         (0)       98 2024-04-27 10:28:09.000000 lettrade-0.0.1/lettrade/exchange/backtest/__init__.py
--rwxrwxrwx   0 m3        (1000) root         (0)        0 2024-04-26 02:40:47.000000 lettrade-0.0.1/lettrade/exchange/backtest/commission.py
-drwxrwxrwx   0 m3        (1000) root         (0)        0 2024-04-27 15:32:40.165527 lettrade-0.0.1/lettrade/exchange/backtest/data/
--rwxrwxrwx   0 m3        (1000) root         (0)       76 2024-04-27 10:28:15.000000 lettrade-0.0.1/lettrade/exchange/backtest/data/__init__.py
--rwxrwxrwx   0 m3        (1000) root         (0)     1157 2024-04-27 11:43:57.000000 lettrade-0.0.1/lettrade/exchange/backtest/data/data.py
--rwxrwxrwx   0 m3        (1000) root         (0)     1109 2024-04-27 11:21:28.000000 lettrade-0.0.1/lettrade/exchange/backtest/data/yfinance.py
--rwxrwxrwx   0 m3        (1000) root         (0)      567 2024-04-27 08:01:38.000000 lettrade-0.0.1/lettrade/exchange/backtest/exchange.py
--rwxrwxrwx   0 m3        (1000) root         (0)      488 2024-04-27 11:14:42.000000 lettrade-0.0.1/lettrade/exchange/backtest/feeder.py
--rwxrwxrwx   0 m3        (1000) root         (0)      637 2024-04-27 08:47:37.000000 lettrade-0.0.1/lettrade/exchange/exchange.py
-drwxrwxrwx   0 m3        (1000) root         (0)        0 2024-04-27 15:32:40.167688 lettrade-0.0.1/lettrade/indicator/
--rwxrwxrwx   0 m3        (1000) root         (0)       49 2024-04-27 09:16:59.000000 lettrade-0.0.1/lettrade/indicator/__init__.py
--rwxrwxrwx   0 m3        (1000) root         (0)      930 2024-04-27 14:00:31.000000 lettrade-0.0.1/lettrade/indicator/function.py
--rwxrwxrwx   0 m3        (1000) root         (0)        0 2024-04-27 05:14:50.000000 lettrade-0.0.1/lettrade/indicator/indicator.py
-drwxrwxrwx   0 m3        (1000) root         (0)        0 2024-04-27 15:32:40.177035 lettrade-0.0.1/lettrade/lettrade.egg-info/
--rwxrwxrwx   0 m3        (1000) root         (0)     1844 2024-04-27 15:32:40.000000 lettrade-0.0.1/lettrade/lettrade.egg-info/PKG-INFO
--rwxrwxrwx   0 m3        (1000) root         (0)     1200 2024-04-27 15:32:40.000000 lettrade-0.0.1/lettrade/lettrade.egg-info/SOURCES.txt
--rwxrwxrwx   0 m3        (1000) root         (0)        1 2024-04-27 15:32:40.000000 lettrade-0.0.1/lettrade/lettrade.egg-info/dependency_links.txt
--rwxrwxrwx   0 m3        (1000) root         (0)       66 2024-04-27 15:32:40.000000 lettrade-0.0.1/lettrade/lettrade.egg-info/top_level.txt
-drwxrwxrwx   0 m3        (1000) root         (0)        0 2024-04-27 15:32:40.171692 lettrade-0.0.1/lettrade/plot/
--rwxrwxrwx   0 m3        (1000) root         (0)       26 2024-04-26 15:26:18.000000 lettrade-0.0.1/lettrade/plot/__init__.py
--rwxrwxrwx   0 m3        (1000) root         (0)     2141 2024-04-27 11:25:37.000000 lettrade-0.0.1/lettrade/plot/plot.py
-drwxrwxrwx   0 m3        (1000) root         (0)        0 2024-04-27 15:32:40.173074 lettrade-0.0.1/lettrade/strategy/
--rwxrwxrwx   0 m3        (1000) root         (0)       31 2024-04-26 02:12:21.000000 lettrade-0.0.1/lettrade/strategy/__init__.py
--rwxrwxrwx   0 m3        (1000) root         (0)     2949 2024-04-27 08:49:16.000000 lettrade-0.0.1/lettrade/strategy/strategy.py
-drwxrwxrwx   0 m3        (1000) root         (0)        0 2024-04-27 15:32:40.176083 lettrade-0.0.1/lettrade/trade/
--rwxrwxrwx   0 m3        (1000) root         (0)       81 2024-04-26 15:40:02.000000 lettrade-0.0.1/lettrade/trade/__init__.py
--rwxrwxrwx   0 m3        (1000) root         (0)     5284 2024-04-26 15:43:50.000000 lettrade-0.0.1/lettrade/trade/order.py
--rwxrwxrwx   0 m3        (1000) root         (0)     1868 2024-04-26 15:41:17.000000 lettrade-0.0.1/lettrade/trade/position.py
--rwxrwxrwx   0 m3        (1000) root         (0)     5762 2024-04-26 15:44:02.000000 lettrade-0.0.1/lettrade/trade/trade.py
--rwxrwxrwx   0 m3        (1000) root         (0)       38 2024-04-27 15:32:40.178274 lettrade-0.0.1/setup.cfg
--rwxrwxrwx   0 m3        (1000) root         (0)     1040 2024-04-27 15:30:54.000000 lettrade-0.0.1/setup.py
+drwxrwxrwx   0 m3        (1000) root         (0)        0 2024-05-18 08:33:31.045643 lettrade-0.0.2/
+-rwxrwxrwx   0 m3        (1000) root         (0)    34523 2024-04-26 01:41:03.000000 lettrade-0.0.2/LICENSE
+-rwxrwxrwx   0 m3        (1000) root         (0)     3500 2024-05-18 08:33:31.045074 lettrade-0.0.2/PKG-INFO
+-rwxrwxrwx   0 m3        (1000) root         (0)     2107 2024-05-18 06:36:47.000000 lettrade-0.0.2/README.md
+drwxrwxrwx   0 m3        (1000) root         (0)        0 2024-05-18 08:33:30.994060 lettrade-0.0.2/lettrade/
+drwxrwxrwx   0 m3        (1000) root         (0)        0 2024-05-18 08:33:30.997401 lettrade-0.0.2/lettrade/account/
+-rwxrwxrwx   0 m3        (1000) root         (0)       29 2024-05-04 12:04:30.000000 lettrade-0.0.2/lettrade/account/__init__.py
+-rwxrwxrwx   0 m3        (1000) root         (0)     1670 2024-05-18 06:14:28.000000 lettrade-0.0.2/lettrade/account/account.py
+drwxrwxrwx   0 m3        (1000) root         (0)        0 2024-05-18 08:33:30.999001 lettrade-0.0.2/lettrade/base/
+-rwxrwxrwx   0 m3        (1000) root         (0)       32 2024-04-27 07:43:15.000000 lettrade-0.0.2/lettrade/base/__init__.py
+-rwxrwxrwx   0 m3        (1000) root         (0)      311 2024-05-04 12:51:53.000000 lettrade-0.0.2/lettrade/base/feed.py
+drwxrwxrwx   0 m3        (1000) root         (0)        0 2024-05-18 08:33:31.000625 lettrade-0.0.2/lettrade/brain/
+-rwxrwxrwx   0 m3        (1000) root         (0)       25 2024-04-26 04:37:23.000000 lettrade-0.0.2/lettrade/brain/__init__.py
+-rwxrwxrwx   0 m3        (1000) root         (0)     2234 2024-05-17 06:33:46.000000 lettrade-0.0.2/lettrade/brain/brain.py
+drwxrwxrwx   0 m3        (1000) root         (0)        0 2024-05-18 08:33:31.002998 lettrade-0.0.2/lettrade/commander/
+-rwxrwxrwx   0 m3        (1000) root         (0)       33 2024-05-17 02:26:14.000000 lettrade-0.0.2/lettrade/commander/__init__.py
+-rwxrwxrwx   0 m3        (1000) root         (0)      994 2024-05-17 05:05:15.000000 lettrade-0.0.2/lettrade/commander/commander.py
+-rwxrwxrwx   0 m3        (1000) root         (0)    13385 2024-05-17 00:39:47.000000 lettrade-0.0.2/lettrade/commander/telegram.py
+drwxrwxrwx   0 m3        (1000) root         (0)        0 2024-05-18 08:33:31.007879 lettrade-0.0.2/lettrade/data/
+-rwxrwxrwx   0 m3        (1000) root         (0)       87 2024-04-26 06:54:51.000000 lettrade-0.0.2/lettrade/data/__init__.py
+-rwxrwxrwx   0 m3        (1000) root         (0)      557 2024-05-02 03:54:13.000000 lettrade-0.0.2/lettrade/data/csv.py
+-rwxrwxrwx   0 m3        (1000) root         (0)     1740 2024-05-17 08:00:18.000000 lettrade-0.0.2/lettrade/data/data.py
+drwxrwxrwx   0 m3        (1000) root         (0)        0 2024-05-18 08:33:31.009588 lettrade-0.0.2/lettrade/data/exporter/
+-rwxrwxrwx   0 m3        (1000) root         (0)       28 2024-05-18 00:44:50.000000 lettrade-0.0.2/lettrade/data/exporter/__init__.py
+-rwxrwxrwx   0 m3        (1000) root         (0)      836 2024-05-17 05:08:01.000000 lettrade-0.0.2/lettrade/data/exporter/csv.py
+-rwxrwxrwx   0 m3        (1000) root         (0)      531 2024-05-17 05:21:11.000000 lettrade-0.0.2/lettrade/data/feeder.py
+-rwxrwxrwx   0 m3        (1000) root         (0)        0 2024-04-26 05:17:01.000000 lettrade-0.0.2/lettrade/data/pickle.py
+-rwxrwxrwx   0 m3        (1000) root         (0)        0 2024-04-26 02:43:25.000000 lettrade-0.0.2/lettrade/data/replay.py
+drwxrwxrwx   0 m3        (1000) root         (0)        0 2024-05-18 08:33:31.015553 lettrade-0.0.2/lettrade/exchange/
+-rwxrwxrwx   0 m3        (1000) root         (0)      239 2024-05-17 00:39:47.000000 lettrade-0.0.2/lettrade/exchange/__init__.py
+drwxrwxrwx   0 m3        (1000) root         (0)        0 2024-05-18 08:33:31.021010 lettrade-0.0.2/lettrade/exchange/backtest/
+-rwxrwxrwx   0 m3        (1000) root         (0)      198 2024-05-17 04:24:52.000000 lettrade-0.0.2/lettrade/exchange/backtest/__init__.py
+-rwxrwxrwx   0 m3        (1000) root         (0)      552 2024-05-18 08:00:23.000000 lettrade-0.0.2/lettrade/exchange/backtest/account.py
+-rwxrwxrwx   0 m3        (1000) root         (0)      458 2024-05-17 04:24:35.000000 lettrade-0.0.2/lettrade/exchange/backtest/commander.py
+drwxrwxrwx   0 m3        (1000) root         (0)        0 2024-05-18 08:33:31.024111 lettrade-0.0.2/lettrade/exchange/backtest/data/
+-rwxrwxrwx   0 m3        (1000) root         (0)       76 2024-04-27 10:28:15.000000 lettrade-0.0.2/lettrade/exchange/backtest/data/__init__.py
+-rwxrwxrwx   0 m3        (1000) root         (0)     1358 2024-05-17 05:11:32.000000 lettrade-0.0.2/lettrade/exchange/backtest/data/data.py
+-rwxrwxrwx   0 m3        (1000) root         (0)     1111 2024-05-18 01:43:46.000000 lettrade-0.0.2/lettrade/exchange/backtest/data/yfinance.py
+-rwxrwxrwx   0 m3        (1000) root         (0)     3018 2024-05-17 23:38:42.000000 lettrade-0.0.2/lettrade/exchange/backtest/exchange.py
+-rwxrwxrwx   0 m3        (1000) root         (0)      485 2024-05-17 00:39:47.000000 lettrade-0.0.2/lettrade/exchange/backtest/feeder.py
+-rwxrwxrwx   0 m3        (1000) root         (0)     4047 2024-05-18 01:37:22.000000 lettrade-0.0.2/lettrade/exchange/backtest/trade.py
+-rwxrwxrwx   0 m3        (1000) root         (0)      857 2024-05-18 01:37:22.000000 lettrade-0.0.2/lettrade/exchange/base.py
+-rwxrwxrwx   0 m3        (1000) root         (0)     6201 2024-05-17 23:52:05.000000 lettrade-0.0.2/lettrade/exchange/exchange.py
+-rwxrwxrwx   0 m3        (1000) root         (0)     2096 2024-05-17 23:48:56.000000 lettrade-0.0.2/lettrade/exchange/execute.py
+drwxrwxrwx   0 m3        (1000) root         (0)        0 2024-05-18 08:33:31.031681 lettrade-0.0.2/lettrade/exchange/metatrader/
+-rwxrwxrwx   0 m3        (1000) root         (0)       88 2024-05-18 01:31:35.000000 lettrade-0.0.2/lettrade/exchange/metatrader/__init__.py
+-rwxrwxrwx   0 m3        (1000) root         (0)      541 2024-05-17 00:39:47.000000 lettrade-0.0.2/lettrade/exchange/metatrader/account.py
+-rwxrwxrwx   0 m3        (1000) root         (0)     6613 2024-05-17 00:39:47.000000 lettrade-0.0.2/lettrade/exchange/metatrader/api.py
+-rwxrwxrwx   0 m3        (1000) root         (0)     3540 2024-05-18 00:42:39.000000 lettrade-0.0.2/lettrade/exchange/metatrader/data.py
+-rwxrwxrwx   0 m3        (1000) root         (0)     4021 2024-05-18 01:41:36.000000 lettrade-0.0.2/lettrade/exchange/metatrader/exchange.py
+-rwxrwxrwx   0 m3        (1000) root         (0)      928 2024-05-17 00:39:47.000000 lettrade-0.0.2/lettrade/exchange/metatrader/feeder.py
+-rwxrwxrwx   0 m3        (1000) root         (0)     2122 2024-05-18 04:24:57.000000 lettrade-0.0.2/lettrade/exchange/metatrader/metatrader.py
+-rwxrwxrwx   0 m3        (1000) root         (0)     6878 2024-05-18 01:37:22.000000 lettrade-0.0.2/lettrade/exchange/metatrader/trade.py
+-rwxrwxrwx   0 m3        (1000) root         (0)     5109 2024-05-18 01:38:15.000000 lettrade-0.0.2/lettrade/exchange/order.py
+-rwxrwxrwx   0 m3        (1000) root         (0)     2361 2024-05-17 00:59:04.000000 lettrade-0.0.2/lettrade/exchange/position.py
+-rwxrwxrwx   0 m3        (1000) root         (0)     3712 2024-05-17 07:34:44.000000 lettrade-0.0.2/lettrade/exchange/trade.py
+drwxrwxrwx   0 m3        (1000) root         (0)        0 2024-05-18 08:33:31.034274 lettrade-0.0.2/lettrade/indicator/
+-rwxrwxrwx   0 m3        (1000) root         (0)       49 2024-04-27 09:16:59.000000 lettrade-0.0.2/lettrade/indicator/__init__.py
+-rwxrwxrwx   0 m3        (1000) root         (0)      862 2024-05-01 08:08:19.000000 lettrade-0.0.2/lettrade/indicator/function.py
+-rwxrwxrwx   0 m3        (1000) root         (0)        0 2024-04-27 05:14:50.000000 lettrade-0.0.2/lettrade/indicator/indicator.py
+drwxrwxrwx   0 m3        (1000) root         (0)        0 2024-05-18 08:33:31.044108 lettrade-0.0.2/lettrade/lettrade.egg-info/
+-rwxrwxrwx   0 m3        (1000) root         (0)     3500 2024-05-18 08:33:30.000000 lettrade-0.0.2/lettrade/lettrade.egg-info/PKG-INFO
+-rwxrwxrwx   0 m3        (1000) root         (0)     1810 2024-05-18 08:33:30.000000 lettrade-0.0.2/lettrade/lettrade.egg-info/SOURCES.txt
+-rwxrwxrwx   0 m3        (1000) root         (0)        1 2024-05-18 08:33:30.000000 lettrade-0.0.2/lettrade/lettrade.egg-info/dependency_links.txt
+-rwxrwxrwx   0 m3        (1000) root         (0)      143 2024-05-18 08:33:30.000000 lettrade-0.0.2/lettrade/lettrade.egg-info/requires.txt
+-rwxrwxrwx   0 m3        (1000) root         (0)       73 2024-05-18 08:33:30.000000 lettrade-0.0.2/lettrade/lettrade.egg-info/top_level.txt
+drwxrwxrwx   0 m3        (1000) root         (0)        0 2024-05-18 08:33:31.039931 lettrade-0.0.2/lettrade/plot/
+-rwxrwxrwx   0 m3        (1000) root         (0)       26 2024-04-26 15:26:18.000000 lettrade-0.0.2/lettrade/plot/__init__.py
+-rwxrwxrwx   0 m3        (1000) root         (0)     5210 2024-05-18 08:09:03.000000 lettrade-0.0.2/lettrade/plot/plot.py
+drwxrwxrwx   0 m3        (1000) root         (0)        0 2024-05-18 08:33:31.041546 lettrade-0.0.2/lettrade/stats/
+-rwxrwxrwx   0 m3        (1000) root         (0)       29 2024-04-30 00:11:14.000000 lettrade-0.0.2/lettrade/stats/__init__.py
+-rwxrwxrwx   0 m3        (1000) root         (0)     1539 2024-05-18 08:03:34.000000 lettrade-0.0.2/lettrade/stats/stats.py
+drwxrwxrwx   0 m3        (1000) root         (0)        0 2024-05-18 08:33:31.043103 lettrade-0.0.2/lettrade/strategy/
+-rwxrwxrwx   0 m3        (1000) root         (0)       31 2024-04-26 02:12:21.000000 lettrade-0.0.2/lettrade/strategy/__init__.py
+-rwxrwxrwx   0 m3        (1000) root         (0)     4486 2024-05-17 16:39:43.000000 lettrade-0.0.2/lettrade/strategy/strategy.py
+-rwxrwxrwx   0 m3        (1000) root         (0)       38 2024-05-18 08:33:31.045739 lettrade-0.0.2/setup.cfg
+-rwxrwxrwx   0 m3        (1000) root         (0)     1623 2024-05-18 08:33:27.000000 lettrade-0.0.2/setup.py
```

### Comparing `lettrade-0.0.1/LICENSE` & `lettrade-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `lettrade-0.0.1/PKG-INFO` & `lettrade-0.0.2/README.md`

 * *Files 27% similar despite different names*

```diff
@@ -1,73 +1,81 @@
-Metadata-Version: 2.1
-Name: lettrade
-Version: 0.0.1
-Summary: Lightweight trading framwork
-Home-page: https://github.com/AwesomeTrading/lettrade.git
-Author: Santatic
-Classifier: Intended Audience :: Financial and Insurance Industry
-Classifier: Intended Audience :: Science/Research
-Classifier: Framework :: Jupyter
-Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Topic :: Office/Business :: Financial :: Investment
-Classifier: Topic :: Scientific/Engineering :: Visualization
-Requires-Python: >=3.10
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # LetTrade
+
+
+[![Code Coverage](https://img.shields.io/codecov/c/gh/AwesomeTrading/lettrade.svg?style=for-the-badge)](https://codecov.io/gh/AwesomeTrading/lettrade)
+[![PyPI](https://img.shields.io/pypi/v/lettrade.svg?color=blue&style=for-the-badge)](https://pypi.org/project/lettrade)
+[![PyPI Python Version](https://img.shields.io/pypi/pyversions/lettrade.svg?color=skyblue&style=for-the-badge)](https://pypi.org/project/lettrade)
+[![PyPI Downloads](https://img.shields.io/pypi/dd/lettrade.svg?color=skyblue&style=for-the-badge)](https://pypi.org/project/lettrade)
+
 A lightweight trading framework compatible with Stock, Forex, Crypto... markets
 
 Inspired by `freqtrade`, `backtrader`, `backtesting.py`... 
 
-Let make trading simpler :)
+Let make algo trading simple :)
+
+## Installation
+
+Stable version
+```sh
+pip install lettrade
+```
+
+Developing version
+```sh
+pip install git+https://git@github.com/AwesomeTrading/lettrade.git@main
+```
 
 ## Example
 All sample are in `example/` directory
 
 ```python
 import talib.abstract as ta
 
-from lettrade import DataFeed, LetTrade, Strategy
-from lettrade.indicator import crossover
+from lettrade import DataFeed, LetTrade, Strategy, let_backtest
+from lettrade.indicator import crossover, crossunder
 
 
 class SmaCross(Strategy):
     ema1_period = 9
     ema2_period = 21
 
     def indicators(self, df: DataFeed):
         df["ema1"] = ta.EMA(df, timeperiod=self.ema1_period)
         df["ema2"] = ta.EMA(df, timeperiod=self.ema2_period)
-        return df
+
+        df["crossover"] = crossover(df.ema1, df.ema2)
+        df["crossunder"] = crossunder(df.ema1, df.ema2)
 
     def next(self, df: DataFeed):
-        if crossover(df.ema1, df.ema2):
+        if df.crossover[-1]:
             self.buy(1)
-        elif crossover(df.ema2, df.ema1):
+        elif df.crossunder[-1]:
             self.sell(1)
 
-    def end(self):
-        print(self.data.tail(10))
+    def end(self, df: DataFeed):
+        print(df.tail(10))
 
 
-lt = LetTrade(
+lt = let_backtest(
     strategy=SmaCross,
-    csv="data/EURUSD=X_1h.csv",
+    datas="data/EURUSD=X_1h.csv",
 )
 
 lt.run()
 lt.plot()
 
 ```
 
+## Live Trading
+### Official
+- `MetaTrader`: Support MetaTrader 5 Terminal trading
+- `CCXT`: Support most of cryptocurrency exchange from CCXT library
+
 ## Development
 
 Set up conda environment
 ```sh
 conda create -y -n LetTrade python=3.10
 conda activate LetTrade
 conda install -c conda-forge ta-lib
 pip install -r requirements-dev.txt
-```
+```
```

### Comparing `lettrade-0.0.1/lettrade/brain/brain.py` & `lettrade-0.0.2/lettrade/brain/brain.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,54 +1,77 @@
+from lettrade.commander import Commander
+from lettrade.data import DataFeed, DataFeeder
+from lettrade.exchange import Exchange, Execute, Order, Position, Trade
 from lettrade.strategy import Strategy
 
-from ..commission import Commission
-from ..data import DataFeed, DataFeeder
-from ..exchange import Exchange
-from ..strategy import Strategy
-
 
 class Brain:
     """Brain of lettrade"""
 
     def __init__(
         self,
         strategy: Strategy,
+        exchange: Exchange,
         feeder: DataFeeder,
-        commission: Commission = None,
-        cash=10_000,
-        hedging=True,
+        commander: "Commander",
         *args,
         **kwargs,
     ) -> None:
         self.strategy: Strategy = strategy
-        self.exchange: Exchange = strategy.exchange
+        self.exchange: Exchange = exchange
         self.feeder: DataFeeder = feeder
-        self.datas: list[DataFeed] = self.exchange.datas
-        self.data: DataFeed = self.exchange.data
+        self.datas: list[DataFeed] = self.feeder.datas
+        self.data: DataFeed = self.feeder.data
 
-        self._cash = cash
-        self._commission = commission
-        self._hedging = hedging
+        self.commander: "Commander" = commander
 
     def run(self):
         self.strategy.init()
 
-        self.feeder.pre_feed()
+        self.feeder.start()
+        self.exchange.start()
         self.strategy.indicators(self.data)
+        self.strategy.start(self.data)
 
         while self.feeder.alive():
-            # Load feader next data
+            # Load feeder next data
             self.feeder.next()
+            self.exchange.next()
 
             # Realtime continous update data, then rebuild indicator data
             if self.feeder.is_continous:
                 self.strategy.indicators(self.data)
 
             self.strategy.next(self.data)
 
-        self.strategy.end()
+        self.strategy.end(self.data)
 
-    def run_until(self, index=0, next=0):
-        pass
+    def stop(self):
+        self.feeder.stop()
+        self.exchange.stop()
+
+    # Events
+    def on_execute(self, execute: Execute):
+        self.on_transaction(execute)
+        self.strategy.on_execute(execute)
+
+    def on_order(self, order: Order):
+        self.on_transaction(order)
+        self.strategy.on_order(order)
+
+    def on_trade(self, trade: Trade):
+        self.on_transaction(trade)
+        self.strategy.on_trade(trade)
+
+    def on_position(self, position: Position):
+        self.on_transaction(position)
+        self.strategy.on_position(position)
+
+    def on_notify(self, *args, **kwargs):
+        self.strategy.on_notify(*args, **kwargs)
+
+    def on_transaction(self, transaction):
+        if self.commander is not None:
+            # TODO: send message to commander when new transaction
+            self.commander.send_message(f"New transaction: {str(transaction)}")
 
-    def shutdown(self):
-        pass
+        self.strategy.on_transaction(transaction)
```

### Comparing `lettrade-0.0.1/lettrade/exchange/backtest/data/data.py` & `lettrade-0.0.2/lettrade/exchange/backtest/data/data.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,21 +1,24 @@
 import pandas as pd
-import yfinance as yf
-
 from lettrade.data import CSVDataFeed, DataFeed
 
-from .yfinance import yf_parse
-
 
 class BackTestDataFeed(DataFeed):
     def alive(self):
-        return self.index[-1] > 0
+        return self.index.stop > 1
+
+    def bar(self, i=0):
+        return -self.index.start + i, self.datetime[i]
 
     def next(self, size=1) -> bool:
-        self.index -= size
+        self.index = pd.RangeIndex(
+            self.index.start - size,
+            self.index.stop - size,
+            1,
+        )
         return True
 
 
 class CSVBackTestDataFeed(CSVDataFeed, BackTestDataFeed):
     pass
 
 
@@ -36,25 +39,29 @@
             start=start,
             end=end,
             period=period,
             interval=interval,
         )
 
         # Download
+        import yfinance as yf
+
         df = yf.download(ticker, **params)
 
         # Parse to lettrade datafeed
+        from .yfinance import yf_parse
+
         df = yf_parse(df)
 
         # Reindex to 0,1,2,3...
         df.reset_index(inplace=True)
 
-        # Information
-        info = dict(ticker=ticker, **params)
+        # Metadata
+        meta = dict(yf=dict(ticker=ticker, **params))
 
         super().__init__(
             name=name,
-            info=dict(yf=info),
+            meta=meta,
             data=df,
             *args,
             **kwargs,
         )
```

### Comparing `lettrade-0.0.1/lettrade/exchange/backtest/data/yfinance.py` & `lettrade-0.0.2/lettrade/exchange/backtest/data/yfinance.py`

 * *Files 9% similar despite different names*

```diff
@@ -12,26 +12,26 @@
 def yf_download(tickers, path=None, force=False, interval="1d", *args, **kwargs):
     # path validate
     if path is None:
         path = f"data/{tickers}_{interval}.csv"
 
     path = Path(path)
     if not force and path.exists():
-        print(f"File {path} existed")
+        logger.error("File %s existed", path)
         return
 
     # Download
     df: pd.DataFrame = yf.download(tickers=tickers, interval=interval, *args, **kwargs)
     logger.info("YFinance downloaded:\n%s", df)
 
     # Parse
     df = yf_parse(df)
 
     # Save to csv
-    csv_export(df, path=path, index=False)
+    return csv_export(df, path=path)
 
 
 def yf_parse(df: pd.DataFrame):
     df = df[df.High != df.Low]
     df.index = df.index.rename("datetime")
     df = df.rename(
         columns={
```

### Comparing `lettrade-0.0.1/lettrade/indicator/function.py` & `lettrade-0.0.2/lettrade/indicator/function.py`

 * *Files 25% similar despite different names*

```diff
@@ -15,14 +15,14 @@
     diffed = diff(series1, series2)
     return diffed.apply(lambda v: True if v < 0 else False).astype(bool)
 
 
 def crossover(series1: pd.Series, series2: pd.Series) -> pd.Series:
     below1 = below(series1.shift(1), series2.shift(1))
     above0 = above(series1, series2)
-    return above0.add(below1, fill_value=False).astype(bool)
+    return below1 & above0
 
 
 def crossunder(series1: pd.Series, series2: pd.Series) -> pd.Series:
     above1 = above(series1.shift(1), series2.shift(1))
     below0 = below(series1, series2)
-    return above1.add(below0, fill_value=False).astype(bool)
+    return below0 & above1
```

### Comparing `lettrade-0.0.1/lettrade/strategy/strategy.py` & `lettrade-0.0.2/lettrade/exchange/execute.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,123 +1,74 @@
-from abc import ABCMeta, abstractmethod
-from typing import Optional, Tuple
+from .base import BaseTransaction
 
-from ..data import DataFeed
-from ..exchange import Exchange
-from ..trade import Order, Position, Trade
 
+class Execute(BaseTransaction):
+    """
+    Place new orders through `Strategy.buy()` and `Strategy.sell()`.
+    Query existing orders through `Strategy.orders`.
 
-class Strategy(metaclass=ABCMeta):
-    def __init__(self, exchange):
-        self._exchange: Exchange = exchange
+    When an order is executed or [filled], it results in a `Trade`.
 
-    def init(self):
-        pass
+    If you wish to modify aspects of a placed but not yet filled order,
+    cancel it and place a new one instead.
 
-    def indicators(self):
-        """
-        All indicator and signal should implement here to cacheable
-        Because of lettrade will cache/pre-load DataFeeds
-        """
-
-    @abstractmethod
-    def next(self):
-        pass
+    All placed orders are [Good 'Til Canceled].
 
-    def end(self):
-        pass
+    [filled]: https://www.investopedia.com/terms/f/fill.asp
+    [Good 'Til Canceled]: https://www.investopedia.com/terms/g/gtc.asp
+    """
 
-    def buy(
+    def __init__(
         self,
-        *,
+        id: str,
+        exchange: "Exchange",
+        data: "DataFeed",
         size: float,
-        limit: Optional[float] = None,
-        stop: Optional[float] = None,
-        sl: Optional[float] = None,
-        tp: Optional[float] = None,
-        tag: object = None,
-        **kwargs,
+        price: float,
+        at: float,
+        order_id: str = None,
+        order: "Order" = None,
+        trade_id: str = None,
+        trade: "Trade" = None,
     ):
-        """
-        Place a new long order. For explanation of parameters, see `Order` and its properties.
-
-        See `Position.close()` and `Trade.close()` for closing existing positions.
-
-        See also `Strategy.sell()`.
-        """
-        assert (
-            0 < size < 1 or round(size) == size
-        ), "size must be a positive fraction of equity, or a positive whole number of units"
-        return self._exchange.new_order(
-            size,
-            limit,
-            stop,
-            sl,
-            tp,
-            tag,
-            **kwargs,
+        super().__init__(
+            id=id,
+            exchange=exchange,
+            data=data,
+            size=size,
         )
-
-    def sell(
-        self,
-        *,
-        size: float,
-        limit: Optional[float] = None,
-        stop: Optional[float] = None,
-        sl: Optional[float] = None,
-        tp: Optional[float] = None,
-        tag: object = None,
-        **kwargs,
-    ):
-        """
-        Place a new short order. For explanation of parameters, see `Order` and its properties.
-
-        See also `Strategy.buy()`.
-
-        .. note::
-            If you merely want to close an existing long position,
-            use `Position.close()` or `Trade.close()`.
-        """
-        assert (
-            0 < size < 1 or round(size) == size
-        ), "size must be a positive fraction of equity, or a positive whole number of units"
-        return self._exchange.new_order(
-            -size,
-            limit,
-            stop,
-            sl,
-            tp,
-            tag,
-            **kwargs,
-        )
-
-    @property
-    def equity(self) -> float:
-        return 0.0
-
-    @property
-    def exchange(self) -> Exchange:
-        return self._exchange
-
-    @property
-    def data(self) -> DataFeed:
-        return self._exchange.data
-
-    @property
-    def datas(self) -> list[DataFeed]:
-        return self._exchange.datas
-
-    @property
-    def position(self) -> Position:
-        return None
-
-    @property
-    def orders(self) -> Tuple[Order, ...]:
-        return ()
-
-    @property
-    def trades(self) -> Tuple[Trade, ...]:
-        return ()
-
-    @property
-    def closed_trades(self) -> Tuple[Trade, ...]:
-        return ()
+        self.order_id = order_id
+        self.order: "Order" = order
+        self.trade_id = trade_id
+        self.trade: "Trade" = trade
+        self.price = price
+        self.at = at
+
+    def __repr__(self):
+        return f"<Execute id={self.id} size={self.size}>"
+
+    def execute(self):
+        self.exchange.on_execute(self)
+
+    def merge(self, other: "Execute"):
+        """
+        Merge to keep object handler but not overwrite for Strategy using when Strategy want to store object and object will be automatic update directly
+        """
+        if other is self:
+            return
+
+        if self.id != other.id:
+            raise RuntimeError(f"Merge difference id {self.id} != {other.id} execute")
+
+        self.price = other.price
+        self.size = other.size
+
+        if other.at:
+            self.at = other.at
+        if other.order_id:
+            self.order_id = other.order_id
+        if other.order:
+            self.order = other.order
+        if other.trade_id:
+            self.trade_id = other.trade_id
+        if other.trade:
+            self.trade = other.trade
```

### Comparing `lettrade-0.0.1/lettrade/trade/trade.py` & `lettrade-0.0.2/lettrade/exchange/order.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,187 +1,171 @@
-from typing import Optional, Tuple, Union
+from typing import Optional, Type
 
-import numpy as np
-import pandas as pd
+from .base import BaseTransaction, OrderState, OrderType
 
-from .order import Order
 
-
-class Trade:
-    """
-    When an `Order` is filled, it results in an active `Trade`.
-    Find active trades in `Strategy.trades` and closed, settled trades in `Strategy.closed_trades`.
-    """
+class Order(BaseTransaction):
+    _trade_cls: Type["Trade"] = None
+    _execute_cls: Type["Execute"] = None
 
     def __init__(
-        self, broker: "_Broker", size: int, entry_price: float, entry_bar, tag
+        self,
+        id: str,
+        exchange: "Exchange",
+        data: "DataFeed",
+        size: float,
+        state: OrderState = OrderState.Pending,
+        type: OrderType = OrderType.Market,
+        limit_price: Optional[float] = None,
+        stop_price: Optional[float] = None,
+        sl_price: Optional[float] = None,
+        tp_price: Optional[float] = None,
+        trade: Optional["Trade"] = None,
+        tag: object = None,
+        open_at: int = None,
+        open_price: int = None,
     ):
-        self.__broker = broker
-        self.__size = size
-        self.__entry_price = entry_price
-        self.__exit_price: Optional[float] = None
-        self.__entry_bar: int = entry_bar
-        self.__exit_bar: Optional[int] = None
-        self.__sl_order: Optional[Order] = None
-        self.__tp_order: Optional[Order] = None
-        self.__tag = tag
+        super().__init__(
+            id=id,
+            exchange=exchange,
+            data=data,
+            size=size,
+        )
+
+        self.type: OrderType = type
+        self.state: OrderState = state
+        self.limit_price: Optional[float] = limit_price
+        self.stop_price: Optional[float] = stop_price
+        self.sl_price: Optional[float] = sl_price
+        self.tp_price: Optional[float] = tp_price
+        self.trade: Optional["Trade"] = trade
+        self.tag: object = tag
+
+        self.open_at: int = open_at
+        self.open_price: int = open_price
+        self.entry_at: int = None
+        self.entry_price: int = None
 
     def __repr__(self):
-        return (
-            f'<Trade size={self.__size} time={self.__entry_bar}-{self.__exit_bar or ""} '
-            f'price={self.__entry_price}-{self.__exit_price or ""} pl={self.pl:.0f}'
-            f'{" tag="+str(self.__tag) if self.__tag is not None else ""}>'
+        return "<Order {}>".format(
+            ", ".join(
+                f"{param}={value if isinstance(value, str) else round(value, 5)}"
+                for param, value in (
+                    ("id", self.id),
+                    ("type", self.type),
+                    ("state", self.state),
+                    ("size", self.size),
+                    ("limit", self.limit_price),
+                    ("stop", self.stop_price),
+                    ("sl", self.sl_price),
+                    ("tp", self.tp_price),
+                    ("tag", self.tag),
+                )
+                if value is not None
+            )
         )
 
-    def _replace(self, **kwargs):
-        for k, v in kwargs.items():
-            setattr(self, f"_{self.__class__.__qualname__}__{k}", v)
-        return self
-
-    def _copy(self, **kwargs):
-        return copy(self)._replace(**kwargs)
-
-    def close(self, portion: float = 1.0):
-        """Place new `Order` to close `portion` of the trade at next market price."""
-        assert 0 < portion <= 1, "portion must be a fraction between 0 and 1"
-        size = copysign(max(1, round(abs(self.__size) * portion)), -self.__size)
-        order = Order(self.__broker, size, parent_trade=self, tag=self.__tag)
-        self.__broker.orders.insert(0, order)
+    def place(self):
+        if self.state != OrderState.Pending:
+            raise RuntimeError(f"Order {self.id} state {self.state} is not Pending")
+
+        self.state = OrderState.Placed
+        self.exchange.on_order(self)
+        return OrderResultOk(order=self)
+
+    def execute(self, price, at):
+        if self.state != OrderState.Placed:
+            raise RuntimeError(f"Order {self.id} state {self.state} is not Placed")
+
+        self.entry_at = at
+        self.entry_price = price
+        self.state = OrderState.Executed
+        self.exchange.on_order(self)
+
+    def cancel(self):
+        if self.state != OrderState.Placed:
+            raise RuntimeError(f"Order {self.id} state {self.state} is not Placed")
+
+        self.state = OrderState.Canceled
+        self.exchange.on_order(self)
+        return OrderResultOk(order=self)
+
+    def merge(self, other: "Order"):
+        if other is self:
+            return
+
+        if self.id != other.id:
+            raise RuntimeError(f"Merge difference id {self.id} != {other.id} order")
+
+        self.size = other.size
+        self.sl_price = other.sl_price
+        self.tp_price = other.tp_price
+
+        if other.open_price:
+            self.open_price = other.open_price
+        if other.open_at:
+            self.open_at = other.open_at
+        if other.entry_price:
+            self.entry_price = other.entry_price
+        if other.entry_at:
+            self.entry_at = other.entry_at
+        if other.trade:
+            self.trade = other.trade
 
     # Fields getters
-
     @property
-    def size(self):
-        """Trade size (volume; negative for short trades)."""
-        return self.__size
+    def limit(self) -> Optional[float]:
+        return self.limit_price
 
     @property
-    def entry_price(self) -> float:
-        """Trade entry price."""
-        return self.__entry_price
+    def stop(self) -> Optional[float]:
+        return self.stop_price
 
     @property
-    def exit_price(self) -> Optional[float]:
-        """Trade exit price (or None if the trade is still active)."""
-        return self.__exit_price
+    def sl(self) -> Optional[float]:
+        return self.sl_price
 
     @property
-    def entry_bar(self) -> int:
-        """Candlestick bar index of when the trade was entered."""
-        return self.__entry_bar
+    def tp(self) -> Optional[float]:
+        return self.tp_price
 
+    # Extra properties
     @property
-    def exit_bar(self) -> Optional[int]:
-        """
-        Candlestick bar index of when the trade was exited
-        (or None if the trade is still active).
-        """
-        return self.__exit_bar
+    def is_long(self):
+        """True if the order is long (order size is positive)."""
+        return self.size > 0
 
     @property
-    def tag(self):
-        """
-        A tag value inherited from the `Order` that opened
-        this trade.
-
-        This can be used to track trades and apply conditional
-        logic / subgroup analysis.
+    def is_short(self):
+        """True if the order is short (order size is negative)."""
+        return self.size < 0
 
-        See also `Order.tag`.
-        """
-        return self.__tag
+    @property
+    def is_sl_order(self):
+        return self.trade and self is self.trade.sl_order
 
     @property
-    def _sl_order(self):
-        return self.__sl_order
+    def is_tp_order(self):
+        return self.trade and self is self.trade.tp_order
 
     @property
-    def _tp_order(self):
-        return self.__tp_order
+    def is_alive(self) -> bool:
+        return self.state in [OrderState.Pending, OrderState.Placed]
 
-    # Extra properties
 
-    @property
-    def entry_time(self) -> Union[pd.Timestamp, int]:
-        """Datetime of when the trade was entered."""
-        return self.__broker._data.index[self.__entry_bar]
+class OrderResult:
+    def __init__(self, ok=True, order: "Order" = None, code=0, raw=None) -> None:
+        self.ok: bool = ok
+        self.order: "Order" = order
+        self.code: int = code
+        self.raw: object = raw
 
-    @property
-    def exit_time(self) -> Optional[Union[pd.Timestamp, int]]:
-        """Datetime of when the trade was exited."""
-        if self.__exit_bar is None:
-            return None
-        return self.__broker._data.index[self.__exit_bar]
 
-    @property
-    def is_long(self):
-        """True if the trade is long (trade size is positive)."""
-        return self.__size > 0
+class OrderResultOk(OrderResult):
+    def __init__(self, order: Order = None, raw=None) -> None:
+        super().__init__(ok=True, order=order, raw=raw)
 
-    @property
-    def is_short(self):
-        """True if the trade is short (trade size is negative)."""
-        return not self.is_long
 
-    @property
-    def pl(self):
-        """Trade profit (positive) or loss (negative) in cash units."""
-        price = self.__exit_price or self.__broker.last_price
-        return self.__size * (price - self.__entry_price)
-
-    @property
-    def pl_pct(self):
-        """Trade profit (positive) or loss (negative) in percent."""
-        price = self.__exit_price or self.__broker.last_price
-        return copysign(1, self.__size) * (price / self.__entry_price - 1)
-
-    @property
-    def value(self):
-        """Trade total value in cash (volume × price)."""
-        price = self.__exit_price or self.__broker.last_price
-        return abs(self.__size) * price
-
-    # SL/TP management API
-
-    @property
-    def sl(self):
-        """
-        Stop-loss price at which to close the trade.
-
-        This variable is writable. By assigning it a new price value,
-        you create or modify the existing SL order.
-        By assigning it `None`, you cancel it.
-        """
-        return self.__sl_order and self.__sl_order.stop
-
-    @sl.setter
-    def sl(self, price: float):
-        self.__set_contingent("sl", price)
-
-    @property
-    def tp(self):
-        """
-        Take-profit price at which to close the trade.
-
-        This property is writable. By assigning it a new price value,
-        you create or modify the existing TP order.
-        By assigning it `None`, you cancel it.
-        """
-        return self.__tp_order and self.__tp_order.limit
-
-    @tp.setter
-    def tp(self, price: float):
-        self.__set_contingent("tp", price)
-
-    def __set_contingent(self, type, price):
-        assert type in ("sl", "tp")
-        assert price is None or 0 < price < np.inf
-        attr = f"_{self.__class__.__qualname__}__{type}_order"
-        order: Order = getattr(self, attr)
-        if order:
-            order.cancel()
-        if price:
-            kwargs = {"stop": price} if type == "sl" else {"limit": price}
-            order = self.__broker.new_order(
-                -self.size, trade=self, tag=self.tag, **kwargs
-            )
-            setattr(self, attr, order)
+class OrderResultError(OrderResult):
+    def __init__(self, error, code, order: Order = None, raw=None) -> None:
+        super().__init__(ok=False, order=order, code=code, raw=raw)
+        self.error: str = error
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

