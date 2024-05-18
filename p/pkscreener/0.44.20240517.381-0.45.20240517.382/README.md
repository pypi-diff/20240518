# Comparing `tmp/pkscreener-0.44.20240517.381.tar.gz` & `tmp/pkscreener-0.45.20240517.382.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pkscreener-0.44.20240517.381.tar", last modified: Fri May 17 07:37:22 2024, max compression
+gzip compressed data, was "pkscreener-0.45.20240517.382.tar", last modified: Fri May 17 23:46:12 2024, max compression
```

## Comparing `pkscreener-0.44.20240517.381.tar` & `pkscreener-0.45.20240517.382.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxrwxrwx   0        0        0        0 2024-05-17 07:37:22.112404 pkscreener-0.44.20240517.381/
--rw-rw-rw-   0        0        0     1086 2024-05-17 07:34:02.000000 pkscreener-0.44.20240517.381/LICENSE
--rw-rw-rw-   0        0        0     1091 2024-05-17 07:34:02.000000 pkscreener-0.44.20240517.381/LICENSE-Others
--rw-rw-rw-   0        0        0    27795 2024-05-17 07:37:22.112404 pkscreener-0.44.20240517.381/PKG-INFO
--rw-rw-rw-   0        0        0    26856 2024-05-17 07:34:02.000000 pkscreener-0.44.20240517.381/README.md
-drwxrwxrwx   0        0        0        0 2024-05-17 07:37:22.096787 pkscreener-0.44.20240517.381/pkscreener/
--rw-rw-rw-   0        0        0     1582 2024-05-17 07:34:02.000000 pkscreener-0.44.20240517.381/pkscreener/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-17 07:37:22.112404 pkscreener-0.44.20240517.381/pkscreener/classes/
--rw-rw-rw-   0        0        0    13324 2024-05-17 07:34:02.000000 pkscreener-0.44.20240517.381/pkscreener/classes/ArtTexts.py
--rw-rw-rw-   0        0        0    10156 2024-05-17 07:34:02.000000 pkscreener-0.44.20240517.381/pkscreener/classes/Backtest.py
--rw-rw-rw-   0        0        0     5705 2024-05-17 07:34:02.000000 pkscreener-0.44.20240517.381/pkscreener/classes/Barometer.py
--rw-rw-rw-   0        0        0    17333 2024-05-17 07:34:02.000000 pkscreener-0.44.20240517.381/pkscreener/classes/CandlePatterns.py
--rw-rw-rw-   0        0        0     1537 2024-05-17 07:34:02.000000 pkscreener-0.44.20240517.381/pkscreener/classes/Changelog.py
--rw-rw-rw-   0        0        0    34250 2024-05-17 07:34:02.000000 pkscreener-0.44.20240517.381/pkscreener/classes/ConfigManager.py
--rw-rw-rw-   0        0        0    10076 2024-05-17 07:34:02.000000 pkscreener-0.44.20240517.381/pkscreener/classes/Fetcher.py
--rw-rw-rw-   0        0        0    11572 2024-05-17 07:34:02.000000 pkscreener-0.44.20240517.381/pkscreener/classes/MarketMonitor.py
--rw-rw-rw-   0        0        0     3673 2024-05-17 07:34:02.000000 pkscreener-0.44.20240517.381/pkscreener/classes/MarketStatus.py
--rw-rw-rw-   0        0        0    43311 2024-05-17 07:34:02.000000 pkscreener-0.44.20240517.381/pkscreener/classes/MenuOptions.py
--rw-rw-rw-   0        0        0    12534 2024-05-17 07:34:02.000000 pkscreener-0.44.20240517.381/pkscreener/classes/OtaUpdater.py
--rw-rw-rw-   0        0        0    24598 2024-05-17 07:34:02.000000 pkscreener-0.44.20240517.381/pkscreener/classes/PKMarketOpenCloseAnalyser.py
--rw-rw-rw-   0        0        0    22369 2024-05-17 07:34:02.000000 pkscreener-0.44.20240517.381/pkscreener/classes/PKScanRunner.py
--rw-rw-rw-   0        0        0     1623 2024-05-17 07:34:02.000000 pkscreener-0.44.20240517.381/pkscreener/classes/PKScheduledTaskProgress.py
--rw-rw-rw-   0        0        0     8158 2024-05-17 07:34:02.000000 pkscreener-0.44.20240517.381/pkscreener/classes/PKScheduler.py
--rw-rw-rw-   0        0        0     8466 2024-05-17 07:34:02.000000 pkscreener-0.44.20240517.381/pkscreener/classes/PKSpreadsheets.py
--rw-rw-rw-   0        0        0     1907 2024-05-17 07:34:02.000000 pkscreener-0.44.20240517.381/pkscreener/classes/PKTask.py
--rw-rw-rw-   0        0        0    18947 2024-05-17 07:34:02.000000 pkscreener-0.44.20240517.381/pkscreener/classes/Pktalib.py
--rw-rw-rw-   0        0        0    14177 2024-05-17 07:34:02.000000 pkscreener-0.44.20240517.381/pkscreener/classes/Portfolio.py
--rw-rw-rw-   0        0        0    49043 2024-05-17 07:34:02.000000 pkscreener-0.44.20240517.381/pkscreener/classes/PortfolioXRay.py
--rw-rw-rw-   0        0        0   156140 2024-05-17 07:34:02.000000 pkscreener-0.44.20240517.381/pkscreener/classes/ScreeningStatistics.py
--rw-rw-rw-   0        0        0    56357 2024-05-17 07:34:02.000000 pkscreener-0.44.20240517.381/pkscreener/classes/StockScreener.py
--rw-rw-rw-   0        0        0     4993 2024-05-17 07:34:02.000000 pkscreener-0.44.20240517.381/pkscreener/classes/UserMenuChoicesHandler.py
--rw-rw-rw-   0        0        0    84725 2024-05-17 07:34:02.000000 pkscreener-0.44.20240517.381/pkscreener/classes/Utility.py
--rw-rw-rw-   0        0        0     3789 2024-05-17 07:34:02.000000 pkscreener-0.44.20240517.381/pkscreener/classes/WorkflowManager.py
--rw-rw-rw-   0        0        0       28 2024-05-17 07:37:14.000000 pkscreener-0.44.20240517.381/pkscreener/classes/__init__.py
--rw-rw-rw-   0        0        0     5262 2024-05-17 07:34:02.000000 pkscreener-0.44.20240517.381/pkscreener/classes/keys.py
--rw-rw-rw-   0        0        0   791436 2024-05-17 07:34:02.000000 pkscreener-0.44.20240517.381/pkscreener/courbd.ttf
--rw-rw-rw-   0        0        0   141484 2024-05-17 07:34:02.000000 pkscreener-0.44.20240517.381/pkscreener/globals.py
--rw-rw-rw-   0        0        0     1090 2024-05-17 07:34:02.000000 pkscreener-0.44.20240517.381/pkscreener/pkscreener.ini
--rw-rw-rw-   0        0        0    53036 2024-05-17 07:34:02.000000 pkscreener-0.44.20240517.381/pkscreener/pkscreenerbot.py
--rw-rw-rw-   0        0        0    33946 2024-05-17 07:34:02.000000 pkscreener-0.44.20240517.381/pkscreener/pkscreenercli.py
-drwxrwxrwx   0        0        0        0 2024-05-17 07:37:22.112404 pkscreener-0.44.20240517.381/pkscreener.egg-info/
--rw-rw-rw-   0        0        0    27795 2024-05-17 07:37:22.000000 pkscreener-0.44.20240517.381/pkscreener.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1349 2024-05-17 07:37:22.000000 pkscreener-0.44.20240517.381/pkscreener.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-17 07:37:22.000000 pkscreener-0.44.20240517.381/pkscreener.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      120 2024-05-17 07:37:22.000000 pkscreener-0.44.20240517.381/pkscreener.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2024-05-17 07:37:22.000000 pkscreener-0.44.20240517.381/pkscreener.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       11 2024-05-17 07:37:22.000000 pkscreener-0.44.20240517.381/pkscreener.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2024-05-17 07:37:22.128034 pkscreener-0.44.20240517.381/setup.cfg
--rw-rw-rw-   0        0        0     4765 2024-05-17 07:34:02.000000 pkscreener-0.44.20240517.381/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-17 23:46:12.124395 pkscreener-0.45.20240517.382/
+-rw-rw-rw-   0        0        0     1086 2024-05-17 23:42:19.000000 pkscreener-0.45.20240517.382/LICENSE
+-rw-rw-rw-   0        0        0     1091 2024-05-17 23:42:19.000000 pkscreener-0.45.20240517.382/LICENSE-Others
+-rw-rw-rw-   0        0        0    27795 2024-05-17 23:46:12.124395 pkscreener-0.45.20240517.382/PKG-INFO
+-rw-rw-rw-   0        0        0    26856 2024-05-17 23:42:19.000000 pkscreener-0.45.20240517.382/README.md
+drwxrwxrwx   0        0        0        0 2024-05-17 23:46:12.108778 pkscreener-0.45.20240517.382/pkscreener/
+-rw-rw-rw-   0        0        0     1582 2024-05-17 23:42:19.000000 pkscreener-0.45.20240517.382/pkscreener/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-17 23:46:12.124395 pkscreener-0.45.20240517.382/pkscreener/classes/
+-rw-rw-rw-   0        0        0    13324 2024-05-17 23:42:19.000000 pkscreener-0.45.20240517.382/pkscreener/classes/ArtTexts.py
+-rw-rw-rw-   0        0        0    10156 2024-05-17 23:42:19.000000 pkscreener-0.45.20240517.382/pkscreener/classes/Backtest.py
+-rw-rw-rw-   0        0        0     5705 2024-05-17 23:42:19.000000 pkscreener-0.45.20240517.382/pkscreener/classes/Barometer.py
+-rw-rw-rw-   0        0        0    17333 2024-05-17 23:42:19.000000 pkscreener-0.45.20240517.382/pkscreener/classes/CandlePatterns.py
+-rw-rw-rw-   0        0        0     1537 2024-05-17 23:42:19.000000 pkscreener-0.45.20240517.382/pkscreener/classes/Changelog.py
+-rw-rw-rw-   0        0        0    34249 2024-05-17 23:42:19.000000 pkscreener-0.45.20240517.382/pkscreener/classes/ConfigManager.py
+-rw-rw-rw-   0        0        0    10076 2024-05-17 23:42:19.000000 pkscreener-0.45.20240517.382/pkscreener/classes/Fetcher.py
+-rw-rw-rw-   0        0        0    13424 2024-05-17 23:42:19.000000 pkscreener-0.45.20240517.382/pkscreener/classes/MarketMonitor.py
+-rw-rw-rw-   0        0        0     3673 2024-05-17 23:42:19.000000 pkscreener-0.45.20240517.382/pkscreener/classes/MarketStatus.py
+-rw-rw-rw-   0        0        0    45625 2024-05-17 23:42:19.000000 pkscreener-0.45.20240517.382/pkscreener/classes/MenuOptions.py
+-rw-rw-rw-   0        0        0    12534 2024-05-17 23:42:19.000000 pkscreener-0.45.20240517.382/pkscreener/classes/OtaUpdater.py
+-rw-rw-rw-   0        0        0    24598 2024-05-17 23:42:19.000000 pkscreener-0.45.20240517.382/pkscreener/classes/PKMarketOpenCloseAnalyser.py
+-rw-rw-rw-   0        0        0    22819 2024-05-17 23:42:19.000000 pkscreener-0.45.20240517.382/pkscreener/classes/PKScanRunner.py
+-rw-rw-rw-   0        0        0     1623 2024-05-17 23:42:19.000000 pkscreener-0.45.20240517.382/pkscreener/classes/PKScheduledTaskProgress.py
+-rw-rw-rw-   0        0        0     8158 2024-05-17 23:42:19.000000 pkscreener-0.45.20240517.382/pkscreener/classes/PKScheduler.py
+-rw-rw-rw-   0        0        0     8466 2024-05-17 23:42:19.000000 pkscreener-0.45.20240517.382/pkscreener/classes/PKSpreadsheets.py
+-rw-rw-rw-   0        0        0     1907 2024-05-17 23:42:19.000000 pkscreener-0.45.20240517.382/pkscreener/classes/PKTask.py
+-rw-rw-rw-   0        0        0    18947 2024-05-17 23:42:19.000000 pkscreener-0.45.20240517.382/pkscreener/classes/Pktalib.py
+-rw-rw-rw-   0        0        0    14177 2024-05-17 23:42:19.000000 pkscreener-0.45.20240517.382/pkscreener/classes/Portfolio.py
+-rw-rw-rw-   0        0        0    49043 2024-05-17 23:42:19.000000 pkscreener-0.45.20240517.382/pkscreener/classes/PortfolioXRay.py
+-rw-rw-rw-   0        0        0   156140 2024-05-17 23:42:19.000000 pkscreener-0.45.20240517.382/pkscreener/classes/ScreeningStatistics.py
+-rw-rw-rw-   0        0        0    56423 2024-05-17 23:42:19.000000 pkscreener-0.45.20240517.382/pkscreener/classes/StockScreener.py
+-rw-rw-rw-   0        0        0     4993 2024-05-17 23:42:19.000000 pkscreener-0.45.20240517.382/pkscreener/classes/UserMenuChoicesHandler.py
+-rw-rw-rw-   0        0        0    84899 2024-05-17 23:42:19.000000 pkscreener-0.45.20240517.382/pkscreener/classes/Utility.py
+-rw-rw-rw-   0        0        0     3789 2024-05-17 23:42:19.000000 pkscreener-0.45.20240517.382/pkscreener/classes/WorkflowManager.py
+-rw-rw-rw-   0        0        0       28 2024-05-17 23:46:03.000000 pkscreener-0.45.20240517.382/pkscreener/classes/__init__.py
+-rw-rw-rw-   0        0        0     5262 2024-05-17 23:42:19.000000 pkscreener-0.45.20240517.382/pkscreener/classes/keys.py
+-rw-rw-rw-   0        0        0   791436 2024-05-17 23:42:19.000000 pkscreener-0.45.20240517.382/pkscreener/courbd.ttf
+-rw-rw-rw-   0        0        0   144916 2024-05-17 23:42:19.000000 pkscreener-0.45.20240517.382/pkscreener/globals.py
+-rw-rw-rw-   0        0        0     1089 2024-05-17 23:42:19.000000 pkscreener-0.45.20240517.382/pkscreener/pkscreener.ini
+-rw-rw-rw-   0        0        0    53056 2024-05-17 23:42:19.000000 pkscreener-0.45.20240517.382/pkscreener/pkscreenerbot.py
+-rw-rw-rw-   0        0        0    34360 2024-05-17 23:42:19.000000 pkscreener-0.45.20240517.382/pkscreener/pkscreenercli.py
+drwxrwxrwx   0        0        0        0 2024-05-17 23:46:12.108778 pkscreener-0.45.20240517.382/pkscreener.egg-info/
+-rw-rw-rw-   0        0        0    27795 2024-05-17 23:46:12.000000 pkscreener-0.45.20240517.382/pkscreener.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1349 2024-05-17 23:46:12.000000 pkscreener-0.45.20240517.382/pkscreener.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-17 23:46:12.000000 pkscreener-0.45.20240517.382/pkscreener.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      120 2024-05-17 23:46:12.000000 pkscreener-0.45.20240517.382/pkscreener.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2024-05-17 23:46:12.000000 pkscreener-0.45.20240517.382/pkscreener.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       11 2024-05-17 23:46:12.000000 pkscreener-0.45.20240517.382/pkscreener.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2024-05-17 23:46:12.124395 pkscreener-0.45.20240517.382/setup.cfg
+-rw-rw-rw-   0        0        0     4765 2024-05-17 23:42:19.000000 pkscreener-0.45.20240517.382/setup.py
```

### Comparing `pkscreener-0.44.20240517.381/LICENSE` & `pkscreener-0.45.20240517.382/LICENSE`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240517.381/LICENSE-Others` & `pkscreener-0.45.20240517.382/LICENSE-Others`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240517.381/PKG-INFO` & `pkscreener-0.45.20240517.382/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pkscreener
-Version: 0.44.20240517.381
+Version: 0.45.20240517.382
 Summary: A Python-based stock screener for NSE, India with alerts to Telegram Channel (pkscreener)
 Home-page: https://github.com/pkjmesra/pkscreener
-Download-URL: https://github.com/pkjmesra/pkscreener/archive/v0.44.20240517.381.zip
+Download-URL: https://github.com/pkjmesra/pkscreener/archive/v0.45.20240517.382.zip
 Author: pkjmesra
 Author-email: pkjmesra@gmail.com
 License: OSI Approved (MIT)
 Keywords: NSE,Technical Indicators,Scanning,Stock Scanners
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS
@@ -269,19 +269,19 @@
 * Always backtest and analyze the stocks manually before you trade.
 * The Author(s), the software and any related/unrelated entity will not be held liable for your own investing decisions or losses. The authors or this softfware does not make any claim about the correctness of the results.
 * This screener began as a [fork](https://github.com/pranjal-joshi/Screeni-py) but has since added a lot of additional scanners, backtesting, Telegram bots, Alerts and a number of modifications and improvements.
 
 [MADE-IN-INDIA-badge]: https://img.shields.io/badge/MADE%20WITH%20%E2%9D%A4%20IN-INDIA-orange
 [MADE-IN-INDIA]: https://en.wikipedia.org/wiki/India
 [Windows-badge]: https://img.shields.io/badge/Windows-0078D6?logo=windows&logoColor=white
-[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240517.380/pkscreenercli.exe
+[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240517.381/pkscreenercli.exe
 [Linux-badge]: https://img.shields.io/badge/Linux-FCC624?logo=linux&logoColor=black
-[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240517.380/pkscreenercli.bin
+[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240517.381/pkscreenercli.bin
 [Mac OS-badge]: https://img.shields.io/badge/mac%20os-D3D3D3?logo=apple&logoColor=000000
-[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240517.380/pkscreenercli.run
+[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240517.381/pkscreenercli.run
 [GitHub release (latest by date)-badge]: https://img.shields.io/github/v/release/pkjmesra/PKScreener
 [GitHub release (latest by date)]: https://github.com/pkjmesra/PKScreener/releases/latest
 [pypi-badge]: https://img.shields.io/pypi/v/pkscreener.svg?style=flat-square
 [pypi]: https://pypi.python.org/pypi/pkscreener
 [wheel-badge]: https://img.shields.io/pypi/wheel/pkscreener.svg?style=flat-square
 [GitHub all releases]: https://img.shields.io/github/downloads/pkjmesra/PKScreener/total?color=Green&label=Downloads&style=for-the-badge
 [License-badge]: https://img.shields.io/github/license/pkjmesra/PKScreener?style=for-the-badge
```

### Comparing `pkscreener-0.44.20240517.381/README.md` & `pkscreener-0.45.20240517.382/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -247,19 +247,19 @@
 * Always backtest and analyze the stocks manually before you trade.
 * The Author(s), the software and any related/unrelated entity will not be held liable for your own investing decisions or losses. The authors or this softfware does not make any claim about the correctness of the results.
 * This screener began as a [fork](https://github.com/pranjal-joshi/Screeni-py) but has since added a lot of additional scanners, backtesting, Telegram bots, Alerts and a number of modifications and improvements.
 
 [MADE-IN-INDIA-badge]: https://img.shields.io/badge/MADE%20WITH%20%E2%9D%A4%20IN-INDIA-orange
 [MADE-IN-INDIA]: https://en.wikipedia.org/wiki/India
 [Windows-badge]: https://img.shields.io/badge/Windows-0078D6?logo=windows&logoColor=white
-[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240517.380/pkscreenercli.exe
+[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240517.381/pkscreenercli.exe
 [Linux-badge]: https://img.shields.io/badge/Linux-FCC624?logo=linux&logoColor=black
-[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240517.380/pkscreenercli.bin
+[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240517.381/pkscreenercli.bin
 [Mac OS-badge]: https://img.shields.io/badge/mac%20os-D3D3D3?logo=apple&logoColor=000000
-[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240517.380/pkscreenercli.run
+[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240517.381/pkscreenercli.run
 [GitHub release (latest by date)-badge]: https://img.shields.io/github/v/release/pkjmesra/PKScreener
 [GitHub release (latest by date)]: https://github.com/pkjmesra/PKScreener/releases/latest
 [pypi-badge]: https://img.shields.io/pypi/v/pkscreener.svg?style=flat-square
 [pypi]: https://pypi.python.org/pypi/pkscreener
 [wheel-badge]: https://img.shields.io/pypi/wheel/pkscreener.svg?style=flat-square
 [GitHub all releases]: https://img.shields.io/github/downloads/pkjmesra/PKScreener/total?color=Green&label=Downloads&style=for-the-badge
 [License-badge]: https://img.shields.io/github/license/pkjmesra/PKScreener?style=for-the-badge
```

### Comparing `pkscreener-0.44.20240517.381/pkscreener/__init__.py` & `pkscreener-0.45.20240517.382/pkscreener/__init__.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240517.381/pkscreener/classes/ArtTexts.py` & `pkscreener-0.45.20240517.382/pkscreener/classes/ArtTexts.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240517.381/pkscreener/classes/Backtest.py` & `pkscreener-0.45.20240517.382/pkscreener/classes/Backtest.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240517.381/pkscreener/classes/Barometer.py` & `pkscreener-0.45.20240517.382/pkscreener/classes/Barometer.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240517.381/pkscreener/classes/CandlePatterns.py` & `pkscreener-0.45.20240517.382/pkscreener/classes/CandlePatterns.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240517.381/pkscreener/classes/Changelog.py` & `pkscreener-0.45.20240517.382/pkscreener/classes/Changelog.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240517.381/pkscreener/classes/ConfigManager.py` & `pkscreener-0.45.20240517.382/pkscreener/classes/ConfigManager.py`

 * *Files 0% similar despite different names*

```diff
@@ -75,15 +75,15 @@
         # This determines how many days apart the backtest calculations are run.
         # For example, for weekly backtest calculations, set this to 5 (5 days = 1 week)
         # For fortnightly, set this to 10 and so on (10 trading sessions = 2 weeks)
         self.backtestPeriodFactor = 1
         self.maxDashboardWidgetsPerRow = 5
         self.maxNumResultRowsInMonitor = 3
         self.calculatersiintraday = False
-        self.defaultMonitorOptions = " X:12:9:2.5,X:12:23,X:12:28,X:12:31,|{1}X:0:23:>|X:0:27:>|X:0:31:,|{2}X:0:31:,|{3}X:0:27:,X:12:7:3:.01:1,|{5}X:0:5:0:40:,X:12:7:6:1,X:12:11:,X:12:12:i 5m,X:12:17,X:12:24,X:12:6:7:1,X:12:6:3,X:12:6:8,X:12:6:9,X:12:6:10:1,X:12:7:3:.02:1,X:12:13:i 1m,X:12:2,|{1}X:0:29:"
+        self.defaultMonitorOptions = "X:12:9:2.5~X:12:23~X:12:28~X:12:31~|{1}X:0:23:>|X:0:27:>|X:0:31:~|{2}X:0:31:~|{3}X:0:27:~X:12:7:3:.01:1~|{5}X:0:5:0:40:~X:12:7:6:1~X:12:11:~X:12:12:i 5m~X:12:17~X:12:24~X:12:6:7:1~X:12:6:3~X:12:6:8~X:12:6:9~X:12:6:10:1~X:12:7:3:.02:1~X:12:13:i 1m~X:12:2~|{1}X:0:29:"
         self.minimumChangePercentage = 0
         self.daysToLookback = 22 * self.backtestPeriodFactor  # 1 month
         self.periods = [1,2,3,4,5,10,15,22,30]
         if self.maxBacktestWindow > self.periods[-1]:
             self.periods.extend(self.maxBacktestWindow)
 
     @property
```

### Comparing `pkscreener-0.44.20240517.381/pkscreener/classes/Fetcher.py` & `pkscreener-0.45.20240517.382/pkscreener/classes/Fetcher.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240517.381/pkscreener/classes/MarketStatus.py` & `pkscreener-0.45.20240517.382/pkscreener/classes/MarketStatus.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240517.381/pkscreener/classes/MenuOptions.py` & `pkscreener-0.45.20240517.382/pkscreener/classes/MenuOptions.py`

 * *Files 2% similar despite different names*

```diff
@@ -54,44 +54,47 @@
     "L": "Collect Logs for Debugging",
     "H": "Help / About Developer",
     "Z": "Exit (Ctrl + C)",
 }
 level1_P_MenuDict = {
     "1": "Predefined Piped Scanners",
     "2": "Define my custom Piped Scanner",
+    "3": "Run Piped Scans Saved So Far",
     "M": "Back to the Top/Main menu",
 }
-PREDEFINED_SCAN_MENU_KEYS = ["1","2","3","4","5","6","7","8","9","10"]
+PREDEFINED_SCAN_MENU_KEYS = ["1","2","3","4","5","6","7","8","9","10","11"]
 PREDEFINED_SCAN_MENU_TEXTS = [
     "Volume Scanners | High Momentum | Breaking Out Now | ATR Cross     ",
     "Volume Scanners | High Momentum | ATR Cross",
     "Volume Scanners | High Momentum                                    ",
     "Volume Scanners | ATR Cross",
     "Volume Scanners | High Bid/Ask Build Up                            ",
     "High Momentum | ATR Cross",
     "High Momentum | ATR Trailing Stop                                  ",
     "ATR Cross | ATR Trailing Stop",
     "TTM Sqeeze Buy | Intraday RSI b/w 0 to 54                          ",
-    "Volume Scanners | ATR Cross | Intraday RSI b/w 0 to 54",
+    "Volume Scanners | High Momentum | Breaking Out Now | ATR Cross | Intraday RSI b/w 0 to 54",
+    "Volume Scanners | ATR Cross | Intraday RSI b/w 0 to 54             ",
 ]
 level2_P_MenuDict = {}
 for key in PREDEFINED_SCAN_MENU_KEYS:
     level2_P_MenuDict[key] = PREDEFINED_SCAN_MENU_TEXTS[int(key)-1]
 level2_P_MenuDict["M"] = "Back to the Top/Main menu"
 PREDEFINED_SCAN_MENU_VALUES =[
-    "-a y -e -o 'X:12:9:2.5:>|X:0:31:>|X:0:23:>|X:0:27:'",
-    "-a y -e -o 'X:12:9:2.5:>|X:0:31:>|X:0:27:'",
-    "-a y -e -o 'X:12:9:2.5:>|X:0:31:'",
-    "-a y -e -o 'X:12:9:2.5:>|X:0:27:'",
-    "-a y -e -o 'X:12:9:2.5:>|X:0:29:'",
-    "-a y -e -o 'X:12:31:>|X:0:27:'",
-    "-a y -e -o 'X:12:31:>|X:0:30:1:'",
-    "-a y -e -o 'X:12:27:>|X:0:30:1:'",
-    "-a y -e -o 'X:12:7:6:1:>|X:0:5:0:54:i 1m'",
-    "-a y -e -o 'X:12:9:2.5:>|X:0:27:>|X:0:5:0:54:i 1m'"
+    "--systemlaunched -a y -e -o 'X:12:9:2.5:>|X:0:31:>|X:0:23:>|X:0:27:'",
+    "--systemlaunched -a y -e -o 'X:12:9:2.5:>|X:0:31:>|X:0:27:'",
+    "--systemlaunched -a y -e -o 'X:12:9:2.5:>|X:0:31:'",
+    "--systemlaunched -a y -e -o 'X:12:9:2.5:>|X:0:27:'",
+    "--systemlaunched -a y -e -o 'X:12:9:2.5:>|X:0:29:'",
+    "--systemlaunched -a y -e -o 'X:12:31:>|X:0:27:'",
+    "--systemlaunched -a y -e -o 'X:12:31:>|X:0:30:1:'",
+    "--systemlaunched -a y -e -o 'X:12:27:>|X:0:30:1:'",
+    "--systemlaunched -a y -e -o 'X:12:7:6:1:>|X:0:5:0:54:i 1m'",
+    "--systemlaunched -a y -e -o 'X:12:9:2.5:>|X:0:31:>|X:0:23:>|X:0:27:>|X:0:5:0:54:i 1m'",
+    "--systemlaunched -a y -e -o 'X:12:9:2.5:>|X:0:27:>|X:0:5:0:54:i 1m'",
 ]
 PIPED_SCANNERS = {}
 for key in PREDEFINED_SCAN_MENU_KEYS:
     PIPED_SCANNERS[key] = PREDEFINED_SCAN_MENU_VALUES[int(key)-1]
 
 level1_T_MenuDict = {
     "L": "Long Term",
@@ -246,15 +249,19 @@
 
 level4_X_Lorenzian_MenuDict = {
     "1": "Buy",
     "2": "Sell",
     "3": "Any/All",
     "0": "Cancel",
 }
-
+Pin_MenuDict = {
+    "1": "Pin this scan category or piped scan {0}",
+    "2": "Pin these {0} stocks in the scan results (Just keep tracking only these {0} stocks)",
+    "M": "Back to the Top/Main menu",
+}
 
 class MenuRenderStyle(Enum):
     STANDALONE = 1
     TWO_PER_ROW = 2
     THREE_PER_ROW = 3
 
 
@@ -384,25 +391,31 @@
     def fromDictionary(
         self,
         rawDictionary={},
         renderStyle=MenuRenderStyle.STANDALONE,
         renderExceptionKeys=[],
         skip=[],
         parent=None,
+        substitutes=[]
     ):
         tabLevel = 0
         self.menuDict = {}
         line = 0
         lineIndex = 1
+        substituteIndex = 0
         for key in rawDictionary:
             if skip is not None and key in skip:
                 continue
             m = menu()
+            menuText = rawDictionary[key]
+            if "{0}" in menuText and len(substitutes) > 0:
+                menuText = menuText.format(f"{colorText.WARN}{substitutes[substituteIndex]}{colorText.END}")
+                substituteIndex += 1
             m.create(
-                str(key).upper(), rawDictionary[key], level=self.level, parent=parent
+                str(key).upper(), menuText, level=self.level, parent=parent
             )
             if key in renderExceptionKeys:
                 m.isException = True
                 line += 2
                 lineIndex = 1
                 m.line = line
                 m.lineIndex = lineIndex
@@ -430,14 +443,17 @@
             m = self.menuDict[k]
             if asList:
                 menuText.append(m)
             else:
                 menuText = menuText + m.render(coloredValues=([] if asList else coloredValues))
         return menuText
 
+    def renderPinnedMenu(self,substitutes=[]):
+        return self.renderPinSubmenus(substitutes=substitutes)
+    
     def renderForMenu(self, selectedMenu:menu=None, skip=[], asList=False, renderStyle=None):
         if selectedMenu is None and self.level == 0:
             # Top level Application Main menu
             return self.renderLevel0Menus(
                 skip=skip, asList=asList, renderStyle=renderStyle, parent=selectedMenu
             )
         elif selectedMenu is not None:
@@ -573,14 +589,48 @@
             try:
                 return self.menuDict[str(key).upper()]
             except Exception as e:  # pragma: no cover
                 default_logger().debug(e, exc_info=True)
                 return None
         return None
 
+    def renderPinSubmenus(self, asList=False, renderStyle=None, parent=None, skip=None, substitutes=[]):
+        menuText = self.fromDictionary(
+            Pin_MenuDict,
+            renderExceptionKeys=["M"],
+            renderStyle=renderStyle
+            if renderStyle is not None
+            else MenuRenderStyle.STANDALONE,
+            skip=skip,
+            parent=parent,
+            substitutes = substitutes
+        ).render(asList=asList,coloredValues=["M"])
+        if asList:
+            return menuText
+        else:
+            if OutputControls().enableMultipleLineOutput:
+                OutputControls().printOutput(
+                    colorText.BOLD
+                    + colorText.WARN
+                    + "[+] Select a menu option:"
+                    + colorText.END
+                )
+                OutputControls().printOutput(
+                    colorText.BOLD
+                    + menuText
+                    + """
+
+    Enter your choice > (default is """
+                    + colorText.WARN
+                    + (self.find("M") or menu().create('?','?')).keyTextLabel().strip()
+                    + ") "
+                    "" + colorText.END
+                )
+            return menuText
+        
     def renderLevel0Menus(self, asList=False, renderStyle=None, parent=None, skip=None):
         menuText = self.fromDictionary(
             level0MenuDict,
             renderExceptionKeys=["P", "T", "E", "U", "Z", "L", "D"],
             renderStyle=renderStyle
             if renderStyle is not None
             else MenuRenderStyle.STANDALONE,
```

### Comparing `pkscreener-0.44.20240517.381/pkscreener/classes/OtaUpdater.py` & `pkscreener-0.45.20240517.382/pkscreener/classes/OtaUpdater.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240517.381/pkscreener/classes/PKMarketOpenCloseAnalyser.py` & `pkscreener-0.45.20240517.382/pkscreener/classes/PKMarketOpenCloseAnalyser.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240517.381/pkscreener/classes/PKScanRunner.py` & `pkscreener-0.45.20240517.382/pkscreener/classes/PKScanRunner.py`

 * *Files 7% similar despite different names*

```diff
@@ -98,19 +98,19 @@
         return screenResults, saveResults
 
     def initQueues(minimumCount=0,userPassedArgs=None):
         tasks_queue = multiprocessing.JoinableQueue()
         results_queue = multiprocessing.Queue()
         logging_queue = multiprocessing.Queue()
 
-        totalConsumers = 1 if (userPassedArgs is not None and userPassedArgs.singlethread is not None) else min(minimumCount, multiprocessing.cpu_count())
+        totalConsumers = 1 if (userPassedArgs is not None and userPassedArgs.singlethread) else min(minimumCount, multiprocessing.cpu_count())
         if totalConsumers == 1:
             totalConsumers = 2  # This is required for single core machine
-        if PKScanRunner.configManager.cacheEnabled is True and multiprocessing.cpu_count() > 2:
-            totalConsumers -= 1
+        # if PKScanRunner.configManager.cacheEnabled is True and multiprocessing.cpu_count() > 2:
+        #     totalConsumers -= 1
         return tasks_queue, results_queue, totalConsumers, logging_queue
 
     def populateQueues(items, tasks_queue, exit=False,userPassedArgs=None):
         # default_logger().debug(f"Unfinished items in task_queue: {tasks_queue.qsize()}")
         for item in items:
             tasks_queue.put(item)
         mayBePiped = userPassedArgs is not None and (userPassedArgs.monitor is not None or "|" in userPassedArgs.options)
@@ -287,14 +287,18 @@
 
         OutputControls().printOutput(colorText.END)
         if userPassedArgs is not None and (userPassedArgs.monitor is None and "|" not in userPassedArgs.options) and not userPassedArgs.options.upper().startswith("C"):
             # Don't terminate the multiprocessing clients if we're 
             # going to pipe the results from an earlier run
             # or we're running in monitoring mode
             PKScanRunner.terminateAllWorkers(userPassedArgs,consumers, tasks_queue, testing)
+        else:
+            for worker in consumers:
+                worker.paused = True
+                worker._clear()
         return screenResults, saveResults,backtest_df,tasks_queue, results_queue, consumers, logging_queue
 
     @exit_after(180) # Should not remain stuck starting the multiprocessing clients beyond this time
     def prepareToRunScan(menuOption,keyboardInterruptEvent, screenCounter, screenResultsCounter, stockDictPrimary,stockDictSecondary, items, executeOption,userPassedArgs):
         tasks_queue, results_queue, totalConsumers, logging_queue = PKScanRunner.initQueues(len(items),userPassedArgs)
         scr = ScreeningStatistics.ScreeningStatistics(PKScanRunner.configManager, default_logger())
         exists, cache_file = Utility.tools.afterMarketStockDataExists(intraday=PKScanRunner.configManager.isIntradayConfig())
@@ -322,15 +326,19 @@
                         # None
                         (cache_file if (exists and menuOption in ["C"]) else None),
                         (sec_cache_file if (exists and menuOption in ["C"]) else None),
                     )
                     for _ in range(totalConsumers)
                 ]
         # if executeOption == 29: # Intraday Bid/Ask, for which we need to fetch data from NSE instead of yahoo
-        intradayFetcher = Intra_Day("SBINEQN") # This will initialise the cookies etc.
+        try:
+            intradayFetcher = None
+            intradayFetcher = Intra_Day("SBINEQN") # This will initialise the cookies etc.
+        except:
+            pass
         for consumer in consumers:
             consumer.intradayNSEFetcher = intradayFetcher
         PKScanRunner.startWorkers(consumers)
         return tasks_queue,results_queue,consumers,logging_queue
 
     @exit_after(120) # Should not remain stuck starting the multiprocessing clients beyond this time
     def startWorkers(consumers):
@@ -436,14 +444,19 @@
             
             if resultsReceivedCb is not None:
                 shouldContinue, backtest_df = resultsReceivedCb(result, numStocks, backtest_df,*otherArgs)
             counter += 1
             # If it's being run under unit testing, let's wrap up if we find at least 1
             # stock or if we've already tried screening through 5% of the list.
             if (not shouldContinue) or (testing and counter >= int(numStocksPerIteration * 0.05)):
+                if PKScanRunner.consumers is not None:
+                    consumers = PKScanRunner.consumers
+                    for worker in consumers:
+                        worker.paused = True
+                        worker._clear()
                 break
             # Add to the queue when we're through 75% of the previously added items already
             if counter >= numStocksPerIteration: #int(numStocksPerIteration * 0.75):
                 queueCounter += 1
                 counter = 0
         
         return backtest_df, lastNonNoneResult
```

### Comparing `pkscreener-0.44.20240517.381/pkscreener/classes/PKScheduledTaskProgress.py` & `pkscreener-0.45.20240517.382/pkscreener/classes/PKScheduledTaskProgress.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240517.381/pkscreener/classes/PKScheduler.py` & `pkscreener-0.45.20240517.382/pkscreener/classes/PKScheduler.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240517.381/pkscreener/classes/PKSpreadsheets.py` & `pkscreener-0.45.20240517.382/pkscreener/classes/PKSpreadsheets.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240517.381/pkscreener/classes/PKTask.py` & `pkscreener-0.45.20240517.382/pkscreener/classes/PKTask.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240517.381/pkscreener/classes/Pktalib.py` & `pkscreener-0.45.20240517.382/pkscreener/classes/Pktalib.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240517.381/pkscreener/classes/Portfolio.py` & `pkscreener-0.45.20240517.382/pkscreener/classes/Portfolio.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240517.381/pkscreener/classes/PortfolioXRay.py` & `pkscreener-0.45.20240517.382/pkscreener/classes/PortfolioXRay.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240517.381/pkscreener/classes/ScreeningStatistics.py` & `pkscreener-0.45.20240517.382/pkscreener/classes/ScreeningStatistics.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240517.381/pkscreener/classes/StockScreener.py` & `pkscreener-0.45.20240517.382/pkscreener/classes/StockScreener.py`

 * *Files 0% similar despite different names*

```diff
@@ -551,15 +551,15 @@
                         or (executeOption == 21 and (mfiStake > 0 and reversalOption in [3,5]))
                         or (executeOption == 21 and (mfiStake < 0 and reversalOption in [6,7]))
                         or (executeOption == 21 and (fairValueDiff > 0 and reversalOption in [8]))
                         or (executeOption == 21 and (fairValueDiff < 0 and reversalOption in [9]))
                         or (executeOption == 26)
                         or (executeOption == 29) and bidGreaterThanAsk
                     ):
-                        isNotMonitoringDashboard = userArgs.monitor is None
+                        isNotMonitoringDashboard = userArgs.monitor is None or (userArgs.monitor is not None and "~" not in userArgs.monitor)
                         # Now screen for common ones to improve performance
                         if isNotMonitoringDashboard and not (executeOption == 6 and reversalOption == 7):
                             if sys.version_info >= (3, 11):
                                 with SuppressOutput(suppress_stderr=True, suppress_stdout=True):
                                     screener.validateLorentzian(
                                         fullData,
                                         screeningDictionary,
```

### Comparing `pkscreener-0.44.20240517.381/pkscreener/classes/UserMenuChoicesHandler.py` & `pkscreener-0.45.20240517.382/pkscreener/classes/UserMenuChoicesHandler.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240517.381/pkscreener/classes/Utility.py` & `pkscreener-0.45.20240517.382/pkscreener/classes/Utility.py`

 * *Files 0% similar despite different names*

```diff
@@ -836,14 +836,15 @@
                 if task.result is not None:
                     for stock in task.userData:
                         taskResult = task.result.get(f"{stock}{exchangeSuffix}")
                         if taskResult is not None:
                             stockDict[stock] = taskResult.to_dict("split")
                             processedStocks.append(stock)
         leftOutStocks = list(set(stockCodes)-set(processedStocks))
+        default_logger().debug(f"Attempted fresh download of {len(stockCodes)} stocks and downloaded {len(processedStocks)} stocks. {len(leftOutStocks)} stocks remaining.")
         return stockDict, leftOutStocks
 
     def loadStockData(
         stockDict,
         configManager,
         downloadOnly=False,
         defaultAnswer=None,
```

### Comparing `pkscreener-0.44.20240517.381/pkscreener/classes/WorkflowManager.py` & `pkscreener-0.45.20240517.382/pkscreener/classes/WorkflowManager.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240517.381/pkscreener/classes/keys.py` & `pkscreener-0.45.20240517.382/pkscreener/classes/keys.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240517.381/pkscreener/courbd.ttf` & `pkscreener-0.45.20240517.382/pkscreener/courbd.ttf`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240517.381/pkscreener/globals.py` & `pkscreener-0.45.20240517.382/pkscreener/globals.py`

 * *Files 2% similar despite different names*

```diff
@@ -450,17 +450,24 @@
 
 def showSendHelpInfo(defaultAnswer=None, user=None):
     helpData = Utility.tools.showDevInfo(defaultAnswer=('Y' if user is not None else defaultAnswer))
     if user is not None:
         sendMessageToTelegramChannel(message=Utility.tools.removeAllColorStyles(helpData), user=user)
 
 def initExecution(menuOption=None):
-    global selectedChoice
+    global selectedChoice, userPassedArgs
     Utility.tools.clearScreen()
-
+    if (userPassedArgs is not None and userPassedArgs.pipedmenus is not None):
+        OutputControls().printOutput(
+        colorText.BOLD
+        + colorText.FAIL
+        + "[+] You chose: "
+        + f" (Piped Scan Mode) [{userPassedArgs.pipedmenus}]"
+        + colorText.END
+    )
     m0.renderForMenu(selectedMenu=None)
     try:
         if menuOption is None:
             if "PKDevTools_Default_Log_Level" in os.environ.keys():
                 from PKDevTools.classes import Archiver
                 log_file_path = os.path.join(Archiver.get_user_outputs_dir(), "pkscreener-logs.txt")
                 OutputControls().printOutput(colorText.FAIL + "\n    [+] Logs will be written to:"+colorText.END)
@@ -497,24 +504,25 @@
     showOptionErrorMessage()
     return initExecution()
 
 
 def initPostLevel0Execution(
     menuOption=None, indexOption=None, executeOption=None, skip=[], retrial=False
 ):
-    global newlyListedOnly, selectedChoice
+    global newlyListedOnly, selectedChoice, userPassedArgs
     Utility.tools.clearScreen()
     if menuOption is None:
         OutputControls().printOutput('You must choose an option from the previous menu! Defaulting to "X"...')
         menuOption = "X"
     OutputControls().printOutput(
         colorText.BOLD
         + colorText.FAIL
         + "[+] You chose: "
-        + level0MenuDict[menuOption].strip()
+        + level0MenuDict[menuOption].strip() 
+        + (f" (Piped Scan Mode) [{userPassedArgs.pipedmenus}]" if (userPassedArgs is not None and userPassedArgs.pipedmenus is not None) else "")
         + colorText.END
     )
     if indexOption is None:
         selectedMenu = m0.find(menuOption)
         m1.renderForMenu(selectedMenu=selectedMenu, skip=skip)
     try:
         if indexOption is None:
@@ -554,25 +562,26 @@
             sleep(2)
             Utility.tools.clearScreen()
             return initPostLevel0Execution(retrial=True)
     return indexOption, executeOption
 
 
 def initPostLevel1Execution(indexOption, executeOption=None, skip=[], retrial=False):
-    global selectedChoice
+    global selectedChoice, userPassedArgs
     if executeOption is None:
         if indexOption is not None and indexOption != "W":
             Utility.tools.clearScreen()
             OutputControls().printOutput(
                 colorText.BOLD
                 + colorText.FAIL
                 + "[+] You chose: "
                 + level0MenuDict[selectedChoice["0"]].strip()
                 + " > "
                 + level1_X_MenuDict[selectedChoice["1"]].strip()
+                + (f" (Piped Scan Mode) [{userPassedArgs.pipedmenus}]" if (userPassedArgs is not None and userPassedArgs.pipedmenus is not None) else "")
                 + colorText.END
             )
             selectedMenu = m1.find(indexOption)
             m2.renderForMenu(selectedMenu=selectedMenu, skip=skip)
     try:
         if indexOption is not None and indexOption != "W":
             if executeOption is None:
@@ -749,14 +758,16 @@
     maxRSI = 100
     insideBarToLookback = 7
     respChartPattern = None
     daysForLowestVolume = 30
     backtestPeriod = 0
     reversalOption = None
     listStockCodes = None
+    if userPassedArgs.log:
+        default_logger().debug(f"User Passed args: {userPassedArgs}")
     screenResults, saveResults = PKScanRunner.initDataframes()
     options, menuOption, indexOption, executeOption = getTopLevelMenuChoices(
         startupoptions, testBuild, downloadOnly, defaultAnswer=defaultAnswer
     )
     # Print Level 1 menu options
     selectedMenu = initExecution(menuOption=menuOption)
     menuOption = selectedMenu.menuKey
@@ -777,30 +788,30 @@
             os.system(f"{launcher} -a Y -e -d -i 1m")
         elif menuOption in ["L"]:
             OutputControls().printOutput(f"{colorText.GREEN}Launching PKScreener to collect logs. If it does not launch, please try with the following:{colorText.END}\n{colorText.FAIL}{launcher} -a Y -l{colorText.END}\n{colorText.WARN}Press Ctrl + C to exit at any time.{colorText.END}")
             sleep(2)
             os.system(f"{launcher} -a Y -l")
         sys.exit(0)
     if menuOption in ["P"]:
-        Utility.tools.clearScreen(forceTop=True)
+        updateMenuChoiceHierarchy()
         selectedMenu = m0.find(menuOption)
         m1.renderForMenu(selectedMenu)
         predefinedOption = input(colorText.BOLD + colorText.FAIL + "[+] Select option: ") or "1"
         OutputControls().printOutput(colorText.END, end="")
-        if predefinedOption not in ["1","2"]:
+        if predefinedOption not in ["1","2","3"]:
             return None, None
         if predefinedOption == "1":
-            Utility.tools.clearScreen(forceTop=True)
+            updateMenuChoiceHierarchy()
             selectedMenu = m1.find(predefinedOption)
             m2.renderForMenu(selectedMenu=selectedMenu)
             selPredefinedOption = input(colorText.BOLD + colorText.FAIL + "[+] Select option: ") or "1"
             OutputControls().printOutput(colorText.END, end="")
             if selPredefinedOption in PREDEFINED_SCAN_MENU_KEYS:
                 scannerOption = PIPED_SCANNERS[selPredefinedOption]
-                Utility.tools.clearScreen(forceTop=True)
+                updateMenuChoiceHierarchy()
                 if userPassedArgs.pipedmenus is not None:
                     chosenOptions = scannerOption.split("-o ")[1]
                     userPassedArgs.options = chosenOptions.replace("'","")
                     return addOrRunPipedMenus()
                 launcher = sys.argv[0]
                 launcher = f"python3.11 {launcher}" if launcher.endswith(".py") else launcher
                 OutputControls().printOutput(f"{colorText.GREEN}Launching PKScreener with piped scanners. If it does not launch, please try with the following:{colorText.END}\n{colorText.FAIL}{launcher} {scannerOption}{colorText.END}")
@@ -819,14 +830,17 @@
         elif predefinedOption == "2":
             # User chose custom
             menuOption = "X" # Let's have the user choose various scan options
             selectedMenu = m0.find(menuOption)
             selectedChoice["0"] = selectedMenu.menuKey
             if userPassedArgs.pipedmenus is None:
                 userPassedArgs.pipedmenus = ""
+        elif predefinedOption == "3":
+            if userPassedArgs.pipedmenus is not None:
+                return addOrRunPipedMenus()
     if menuOption in ["X", "T", "E", "Y", "U", "H", "C"]:
         # Print Level 2 menu options
         menuOption, indexOption, executeOption, selectedChoice = getScannerMenuChoices(
             testBuild or testing,
             downloadOnly,
             startupoptions,
             menuOption=menuOption,
@@ -1524,14 +1538,38 @@
                 runOption = PKScanRunner.getFormattedChoices(userPassedArgs,selectedChoice)
                 df = saveResults.copy()
                 df["LastTradeDate"], df["LastTradeTime"] = getLatestTradeDateTime(stockDictPrimary)
                 gClient.df_to_sheet(df=df,sheetName=runOption)
                 OutputControls().printOutput(f"{colorText.GREEN} => Done in {round(time.time()-begin,2)}s{colorText.END}")
     except:
         pass
+    if userPassedArgs is None or (userPassedArgs is not None and (userPassedArgs.answerdefault is None or userPassedArgs.systemlaunched)):
+        prevOutput_results = saveResults.index if (saveResults is not None and not saveResults.empty) else []
+        hasFoundStocks = len(prevOutput_results) > 0 and (("|" not in userPassedArgs.options) if (userPassedArgs is not None and userPassedArgs.options is not None) else True)
+        if hasFoundStocks:
+            monitorOption = userPassedArgs.systemlaunched if (userPassedArgs is not None and isinstance(userPassedArgs.systemlaunched,str) and userPassedArgs.systemlaunched is not None) else (userPassedArgs.options if (userPassedArgs is not None and userPassedArgs.options is not None) else "")
+            if len(monitorOption) == 0:
+                for choice in selectedChoice.keys():
+                    monitorOption = (f"{monitorOption}:" if len(monitorOption) > 0  else '') + f"{selectedChoice[choice]}"
+            m0.renderPinnedMenu(substitutes=[monitorOption,len(prevOutput_results)])
+            pinOption = input(
+                    colorText.BOLD + colorText.FAIL + "[+] Select option: "
+                ) or 'M'
+            OutputControls().printOutput(colorText.END, end="")
+            if pinOption in ["1","2"]:
+                if pinOption in ["2"]:
+                    monitorOption = "X:0:0"
+                    prevOutput_results = ",".join(prevOutput_results)
+                    monitorOption = f"{monitorOption}:{prevOutput_results}"
+                launcher = sys.argv[0]
+                launcher = f"python3.11 {launcher}" if launcher.endswith(".py") else launcher
+                OutputControls().printOutput(f"{colorText.GREEN}Launching PKScreener with pinned scan option. If it does not launch, please try with the following:{colorText.END}\n{colorText.FAIL}{launcher} -a Y -m '{monitorOption}'{colorText.END}")
+                sleep(2)
+                os.system(f"{launcher} -a Y -m '{monitorOption}'")
+
     if userPassedArgs is not None:
         if userPassedArgs.runintradayanalysis:
             analysis_df = screenResults.copy()
             analysis_df.reset_index(inplace=True)
             if 'index' in analysis_df.columns:
                 analysis_df.drop('index', axis=1, inplace=True, errors="ignore")
             if optionalFinalOutcome_df is None:
@@ -1638,26 +1676,27 @@
 def addOrRunPipedMenus():
     global userPassedArgs
     # User must have selected menu "P" earlier
     savedPipes = f"{userPassedArgs.pipedmenus}:>|" if len(userPassedArgs.pipedmenus) > 0 else ""
     userPassedArgs.pipedmenus = f"{savedPipes}{userPassedArgs.options}"
     userPassedArgs.pipedmenus = userPassedArgs.pipedmenus.replace("::",":D:")
     userPassedArgs.pipedmenus = f"{userPassedArgs.pipedmenus}{('i '+configManager.duration) if configManager.isIntradayConfig() else ''}"
+    updateMenuChoiceHierarchy()
     OutputControls().printOutput(
             colorText.GREEN
             + f"[+] {len(userPassedArgs.pipedmenus.split('|'))} Scanners piped so far: {colorText.END}{colorText.WARN+userPassedArgs.pipedmenus+colorText.END}\n{colorText.GREEN}[+] Do you want to add any more scanners into the pipe?"
             + colorText.END
         )
     shouldAddMoreIntoPipe = input(colorText.FAIL + "[+] Select [Y/N] (Default:N): " + colorText.END) or 'n'
     if shouldAddMoreIntoPipe.lower() != 'y':
         launcher = sys.argv[0]
         launcher = f"python3.11 {launcher}" if launcher.endswith(".py") else launcher
         OutputControls().printOutput(f"{colorText.GREEN}Launching PKScreener with piped scanners. If it does not launch, please try with the following:{colorText.END}\n{colorText.FAIL}{launcher} -a Y -e -o '{userPassedArgs.pipedmenus}'{colorText.END}")
         sleep(2)
-        os.system(f"{launcher} -a Y -e -o '{userPassedArgs.pipedmenus}'")
+        os.system(f"{launcher} --systemlaunched -a Y -e -o '{userPassedArgs.pipedmenus}'")
         userPassedArgs.pipedmenus = None
         OutputControls().printOutput(
                 colorText.GREEN
                 + f"[+] Finished running all piped scanners!"
                 + colorText.END
             )
         if defaultAnswer is None:
@@ -1891,61 +1930,65 @@
             if executeOption is not None:
                 selMenu = m2.find(executeOption)
                 m3.renderForMenu(selMenu, asList=True)
 
 
 def updateMenuChoiceHierarchy():
     global userPassedArgs, selectedChoice, menuChoiceHierarchy
-    menuChoiceHierarchy = f'{level0MenuDict[selectedChoice["0"]].strip()}>{level1_X_MenuDict[selectedChoice["1"]].strip()}>{level2_X_MenuDict[selectedChoice["2"]].strip()}'
-    if selectedChoice["2"] == "6":
-        menuChoiceHierarchy = (
-            menuChoiceHierarchy
-            + f'>{level3_X_Reversal_MenuDict[selectedChoice["3"]].strip()}'
-        )
-        if len(selectedChoice) >= 5 and selectedChoice["3"] in ["7","10"]:
-            menuChoiceHierarchy = (
-            menuChoiceHierarchy
-            + f'>{level4_X_Lorenzian_MenuDict[selectedChoice["4"]].strip()}'
-        )
-    elif selectedChoice["2"] in ["30"]:
-        if len(selectedChoice) >= 3:
+    try:
+        menuChoiceHierarchy = f'{level0MenuDict[selectedChoice["0"]].strip()}>{level1_X_MenuDict[selectedChoice["1"]].strip()}>{level2_X_MenuDict[selectedChoice["2"]].strip()}'
+        if selectedChoice["2"] == "6":
             menuChoiceHierarchy = (
-            menuChoiceHierarchy
-            + f'>{level4_X_Lorenzian_MenuDict[selectedChoice["3"]].strip()}'
-        )
-    elif selectedChoice["2"] == "7":
-        menuChoiceHierarchy = (
-            menuChoiceHierarchy
-            + f'>{level3_X_ChartPattern_MenuDict[selectedChoice["3"]].strip()}'
-        )
-        if len(selectedChoice) >= 5 and selectedChoice["3"] == "3":
+                menuChoiceHierarchy
+                + f'>{level3_X_Reversal_MenuDict[selectedChoice["3"]].strip()}'
+            )
+            if len(selectedChoice) >= 5 and selectedChoice["3"] in ["7","10"]:
+                menuChoiceHierarchy = (
+                menuChoiceHierarchy
+                + f'>{level4_X_Lorenzian_MenuDict[selectedChoice["4"]].strip()}'
+            )
+        elif selectedChoice["2"] in ["30"]:
+            if len(selectedChoice) >= 3:
+                menuChoiceHierarchy = (
+                menuChoiceHierarchy
+                + f'>{level4_X_Lorenzian_MenuDict[selectedChoice["3"]].strip()}'
+            )
+        elif selectedChoice["2"] == "7":
             menuChoiceHierarchy = (
-            menuChoiceHierarchy
-            + f'>{level4_X_ChartPattern_Confluence_MenuDict[selectedChoice["4"]].strip()}'
-        )
-        elif len(selectedChoice) >= 5 and selectedChoice["3"] == "6":
+                menuChoiceHierarchy
+                + f'>{level3_X_ChartPattern_MenuDict[selectedChoice["3"]].strip()}'
+            )
+            if len(selectedChoice) >= 5 and selectedChoice["3"] == "3":
+                menuChoiceHierarchy = (
+                menuChoiceHierarchy
+                + f'>{level4_X_ChartPattern_Confluence_MenuDict[selectedChoice["4"]].strip()}'
+            )
+            elif len(selectedChoice) >= 5 and selectedChoice["3"] == "6":
+                menuChoiceHierarchy = (
+                menuChoiceHierarchy
+                + f'>{level4_X_ChartPattern_BBands_SQZ_MenuDict[selectedChoice["4"]].strip()}'
+            )
+        elif selectedChoice["2"] == "21":
             menuChoiceHierarchy = (
-            menuChoiceHierarchy
-            + f'>{level4_X_ChartPattern_BBands_SQZ_MenuDict[selectedChoice["4"]].strip()}'
-        )
-    elif selectedChoice["2"] == "21":
-        menuChoiceHierarchy = (
-            menuChoiceHierarchy
-            + f'>{level3_X_PopularStocks_MenuDict[selectedChoice["3"]].strip()}'
-        )
-    intraday = "(Intraday)" if (userPassedArgs is not None and userPassedArgs.intraday) or configManager.isIntradayConfig() else ""
-    menuChoiceHierarchy = f"{menuChoiceHierarchy}{intraday}"
-    global nValueForMenu
-    menuChoiceHierarchy = menuChoiceHierarchy.replace("N-",f"{nValueForMenu}-")
-    Utility.tools.clearScreen()
+                menuChoiceHierarchy
+                + f'>{level3_X_PopularStocks_MenuDict[selectedChoice["3"]].strip()}'
+            )
+        intraday = "(Intraday)" if (userPassedArgs is not None and userPassedArgs.intraday) or configManager.isIntradayConfig() else ""
+        menuChoiceHierarchy = f"{menuChoiceHierarchy}{intraday}"
+        global nValueForMenu
+        menuChoiceHierarchy = menuChoiceHierarchy.replace("N-",f"{nValueForMenu}-")
+    except:
+        pass
+    Utility.tools.clearScreen(forceTop=True)
     OutputControls().printOutput(
         colorText.BOLD
         + colorText.FAIL
         + "[+] You chose: "
         + menuChoiceHierarchy
+        + (f" (Piped Scan Mode) [{userPassedArgs.pipedmenus}]" if (userPassedArgs is not None and userPassedArgs.pipedmenus is not None) else "")
         + colorText.END
     )
     default_logger().info(menuChoiceHierarchy)
     return menuChoiceHierarchy
 
 def printNotifySaveScreenedResults(
     screenResults, saveResults, selectedChoice, menuChoiceHierarchy, testing, user=None
@@ -1955,28 +1998,29 @@
         return
     MAX_ALLOWED = (100 if userPassedArgs.maxdisplayresults is None else min(int(userPassedArgs.maxdisplayresults),100)) if not testing else 1
     tabulated_backtest_summary = ""
     tabulated_backtest_detail = ""
     recordDate = PKDateUtilities.tradingDate().strftime('%Y-%m-%d') if (userPassedArgs.backtestdaysago is None) else (PKDateUtilities.nthPastTradingDateStringFromFutureDate(int(userPassedArgs.backtestdaysago)))
     if user is None and userPassedArgs.user is not None:
         user = userPassedArgs.user
-    Utility.tools.clearScreen()
+    Utility.tools.clearScreen(forceTop=True)
     if screenResults is not None and len(screenResults) > 0:
         screenResults = screenResults[~screenResults.index.duplicated(keep='first')]
         saveResults = saveResults[~saveResults.index.duplicated(keep='first')]
         if "Stock" in screenResults.columns:
             screenResults.drop_duplicates(keep="first", inplace=True)
         if "Stock" in saveResults.columns:
             saveResults.drop_duplicates(keep="first", inplace=True)
-
+    
     reportTitle = f"{userPassedArgs.pipedtitle}|" if userPassedArgs is not None and userPassedArgs.pipedtitle is not None else ""
     OutputControls().printOutput(
         colorText.BOLD
         + colorText.FAIL
         + f"[+] You chose: {reportTitle}{menuChoiceHierarchy}"
+        + (f" (Piped Scan Mode) [{userPassedArgs.pipedmenus}]" if (userPassedArgs is not None and userPassedArgs.pipedmenus is not None) else "")
         + colorText.END
         , enableMultipleLineOutput=True
     )
     pngName = f'PKS_{PKScanRunner.getFormattedChoices(userPassedArgs,selectedChoice)}_{PKDateUtilities.currentDateTime().strftime("%d-%m-%y_%H.%M.%S")}'
     pngExtension = ".png"
     eligible = is_token_telegram_configured()
     targetDateG10k = prepareGrowthOf10kResults(saveResults, selectedChoice, menuChoiceHierarchy, testing, user, pngName, pngExtension, eligible)
```

### Comparing `pkscreener-0.44.20240517.381/pkscreener/pkscreener.ini` & `pkscreener-0.45.20240517.382/pkscreener/pkscreener.ini`

 * *Files 14% similar despite different names*

```diff
@@ -10,60 +10,60 @@
 00000090: 6f72 203d 2031 0d0a 6361 6368 6573 746f  or = 1..cachesto
 000000a0: 636b 6461 7461 203d 2079 0d0a 6361 6c63  ckdata = y..calc
 000000b0: 756c 6174 6572 7369 696e 7472 6164 6179  ulatersiintraday
 000000c0: 203d 206e 0d0a 6461 7973 746f 6c6f 6f6b   = n..daystolook
 000000d0: 6261 636b 203d 2032 320d 0a64 6566 6175  back = 22..defau
 000000e0: 6c74 696e 6465 7820 3d20 3132 0d0a 6465  ltindex = 12..de
 000000f0: 6661 756c 746d 6f6e 6974 6f72 6f70 7469  faultmonitoropti
-00000100: 6f6e 7320 3d20 2058 3a31 323a 393a 322e  ons =  X:12:9:2.
-00000110: 352c 583a 3132 3a32 332c 583a 3132 3a32  5,X:12:23,X:12:2
-00000120: 382c 583a 3132 3a33 312c 7c7b 317d 583a  8,X:12:31,|{1}X:
-00000130: 3132 3a32 333a 3e7c 583a 303a 3237 3a3e  12:23:>|X:0:27:>
-00000140: 7c58 3a30 3a33 313a 2c7c 7b32 7d58 3a30  |X:0:31:,|{2}X:0
-00000150: 3a33 313a 2c7c 7b33 7d58 3a30 3a32 373a  :31:,|{3}X:0:27:
-00000160: 2c58 3a31 323a 373a 333a 2e30 313a 312c  ,X:12:7:3:.01:1,
-00000170: 7c7b 357d 583a 303a 353a 303a 3430 3a2c  |{5}X:0:5:0:40:,
-00000180: 583a 3132 3a37 3a36 3a31 2c58 3a31 323a  X:12:7:6:1,X:12:
-00000190: 3131 3a2c 583a 3132 3a31 323a 6920 356d  11:,X:12:12:i 5m
-000001a0: 2c58 3a31 323a 3137 2c58 3a31 323a 3234  ,X:12:17,X:12:24
-000001b0: 2c58 3a31 323a 363a 373a 312c 583a 3132  ,X:12:6:7:1,X:12
-000001c0: 3a36 3a33 2c58 3a31 323a 363a 382c 583a  :6:3,X:12:6:8,X:
-000001d0: 3132 3a36 3a39 2c58 3a31 323a 363a 3130  12:6:9,X:12:6:10
-000001e0: 3a31 2c58 3a31 323a 373a 333a 2e30 323a  :1,X:12:7:3:.02:
-000001f0: 312c 583a 3132 3a31 333a 6920 316d 2c58  1,X:12:13:i 1m,X
-00000200: 3a31 323a 322c 7c7b 317d 583a 303a 3239  :12:2,|{1}X:0:29
-00000210: 3a0d 0a64 7572 6174 696f 6e20 3d20 3164  :..duration = 1d
-00000220: 0d0a 656e 6162 6c65 706f 7274 666f 6c69  ..enableportfoli
-00000230: 6f63 616c 6375 6c61 7469 6f6e 7320 3d20  ocalculations = 
-00000240: 6e0d 0a67 656e 6572 616c 7469 6d65 6f75  n..generaltimeou
-00000250: 7420 3d20 322e 300d 0a6c 6f67 7365 6e61  t = 2.0..logsena
-00000260: 626c 6564 203d 206e 0d0a 6c6f 6e67 7469  bled = n..longti
-00000270: 6d65 6f75 7420 3d20 342e 300d 0a6d 6178  meout = 4.0..max
-00000280: 6261 636b 7465 7374 7769 6e64 6f77 203d  backtestwindow =
-00000290: 2033 300d 0a6d 6178 6461 7368 626f 6172   30..maxdashboar
-000002a0: 6477 6964 6765 7473 7065 7272 6f77 203d  dwidgetsperrow =
-000002b0: 2035 0d0a 6d61 786e 6574 776f 726b 7265   5..maxnetworkre
-000002c0: 7472 7963 6f75 6e74 203d 2031 300d 0a6d  trycount = 10..m
-000002d0: 6178 6e75 6d72 6573 756c 7472 6f77 7369  axnumresultrowsi
-000002e0: 6e6d 6f6e 6974 6f72 203d 2033 0d0a 6d6f  nmonitor = 3..mo
-000002f0: 726e 696e 6761 6e61 6c79 7369 7363 616e  rninganalysiscan
-00000300: 646c 656e 756d 6265 7220 3d20 3235 0d0a  dlenumber = 25..
-00000310: 6d6f 726e 696e 6761 6e61 6c79 7369 7363  morninganalysisc
-00000320: 616e 646c 6564 7572 6174 696f 6e20 3d20  andleduration = 
-00000330: 316d 0d0a 6f6e 6c79 7374 6167 6574 776f  1m..onlystagetwo
-00000340: 7374 6f63 6b73 203d 2079 0d0a 7065 7269  stocks = y..peri
-00000350: 6f64 203d 2032 3830 640d 0a73 686f 7770  od = 280d..showp
-00000360: 6173 7473 7472 6174 6567 7964 6174 6120  aststrategydata 
-00000370: 3d20 6e0d 0a73 686f 7775 6e6b 6e6f 776e  = n..showunknown
-00000380: 7472 656e 6473 203d 2079 0d0a 7368 7566  trends = y..shuf
-00000390: 666c 6520 3d20 790d 0a75 7365 656d 6120  fle = y..useema 
-000003a0: 3d20 6e0d 0a0d 0a5b 6669 6c74 6572 735d  = n....[filters]
-000003b0: 0d0a 636f 6e73 6f6c 6964 6174 696f 6e70  ..consolidationp
-000003c0: 6572 6365 6e74 6167 6520 3d20 3130 2e30  ercentage = 10.0
-000003d0: 0d0a 6d61 7870 7269 6365 203d 2035 3030  ..maxprice = 500
-000003e0: 3030 2e30 0d0a 6d69 6e69 6d75 6d63 6861  00.0..minimumcha
-000003f0: 6e67 6570 6572 6365 6e74 6167 6520 3d20  ngepercentage = 
-00000400: 302e 300d 0a6d 696e 696d 756d 766f 6c75  0.0..minimumvolu
-00000410: 6d65 203d 2031 3030 3030 0d0a 6d69 6e70  me = 10000..minp
-00000420: 7269 6365 203d 2032 302e 300d 0a76 6f6c  rice = 20.0..vol
-00000430: 756d 6572 6174 696f 203d 2032 2e35 0d0a  umeratio = 2.5..
-00000440: 0d0a                                     ..
+00000100: 6f6e 7320 3d20 583a 3132 3a39 3a32 2e35  ons = X:12:9:2.5
+00000110: 7e58 3a31 323a 3233 7e58 3a31 323a 3238  ~X:12:23~X:12:28
+00000120: 7e58 3a31 323a 3331 7e7c 7b31 7d58 3a31  ~X:12:31~|{1}X:1
+00000130: 323a 3233 3a3e 7c58 3a30 3a32 373a 3e7c  2:23:>|X:0:27:>|
+00000140: 583a 303a 3331 3a7e 7c7b 327d 583a 303a  X:0:31:~|{2}X:0:
+00000150: 3331 3a7e 7c7b 337d 583a 303a 3237 3a7e  31:~|{3}X:0:27:~
+00000160: 583a 3132 3a37 3a33 3a2e 3031 3a31 7e7c  X:12:7:3:.01:1~|
+00000170: 7b35 7d58 3a30 3a35 3a30 3a34 303a 7e58  {5}X:0:5:0:40:~X
+00000180: 3a31 323a 373a 363a 317e 583a 3132 3a31  :12:7:6:1~X:12:1
+00000190: 313a 7e58 3a31 323a 3132 3a69 2035 6d7e  1:~X:12:12:i 5m~
+000001a0: 583a 3132 3a31 377e 583a 3132 3a32 347e  X:12:17~X:12:24~
+000001b0: 583a 3132 3a36 3a37 3a31 7e58 3a31 323a  X:12:6:7:1~X:12:
+000001c0: 363a 337e 583a 3132 3a36 3a38 7e58 3a31  6:3~X:12:6:8~X:1
+000001d0: 323a 363a 397e 583a 3132 3a36 3a31 303a  2:6:9~X:12:6:10:
+000001e0: 317e 583a 3132 3a37 3a33 3a2e 3032 3a31  1~X:12:7:3:.02:1
+000001f0: 7e58 3a31 323a 3133 3a69 2031 6d7e 583a  ~X:12:13:i 1m~X:
+00000200: 3132 3a32 7e7c 7b31 7d58 3a30 3a32 393a  12:2~|{1}X:0:29:
+00000210: 0d0a 6475 7261 7469 6f6e 203d 2031 640d  ..duration = 1d.
+00000220: 0a65 6e61 626c 6570 6f72 7466 6f6c 696f  .enableportfolio
+00000230: 6361 6c63 756c 6174 696f 6e73 203d 206e  calculations = n
+00000240: 0d0a 6765 6e65 7261 6c74 696d 656f 7574  ..generaltimeout
+00000250: 203d 2032 2e30 0d0a 6c6f 6773 656e 6162   = 2.0..logsenab
+00000260: 6c65 6420 3d20 6e0d 0a6c 6f6e 6774 696d  led = n..longtim
+00000270: 656f 7574 203d 2034 2e30 0d0a 6d61 7862  eout = 4.0..maxb
+00000280: 6163 6b74 6573 7477 696e 646f 7720 3d20  acktestwindow = 
+00000290: 3330 0d0a 6d61 7864 6173 6862 6f61 7264  30..maxdashboard
+000002a0: 7769 6467 6574 7370 6572 726f 7720 3d20  widgetsperrow = 
+000002b0: 350d 0a6d 6178 6e65 7477 6f72 6b72 6574  5..maxnetworkret
+000002c0: 7279 636f 756e 7420 3d20 3130 0d0a 6d61  rycount = 10..ma
+000002d0: 786e 756d 7265 7375 6c74 726f 7773 696e  xnumresultrowsin
+000002e0: 6d6f 6e69 746f 7220 3d20 330d 0a6d 6f72  monitor = 3..mor
+000002f0: 6e69 6e67 616e 616c 7973 6973 6361 6e64  ninganalysiscand
+00000300: 6c65 6e75 6d62 6572 203d 2032 350d 0a6d  lenumber = 25..m
+00000310: 6f72 6e69 6e67 616e 616c 7973 6973 6361  orninganalysisca
+00000320: 6e64 6c65 6475 7261 7469 6f6e 203d 2031  ndleduration = 1
+00000330: 6d0d 0a6f 6e6c 7973 7461 6765 7477 6f73  m..onlystagetwos
+00000340: 746f 636b 7320 3d20 790d 0a70 6572 696f  tocks = y..perio
+00000350: 6420 3d20 3238 3064 0d0a 7368 6f77 7061  d = 280d..showpa
+00000360: 7374 7374 7261 7465 6779 6461 7461 203d  ststrategydata =
+00000370: 206e 0d0a 7368 6f77 756e 6b6e 6f77 6e74   n..showunknownt
+00000380: 7265 6e64 7320 3d20 790d 0a73 6875 6666  rends = y..shuff
+00000390: 6c65 203d 2079 0d0a 7573 6565 6d61 203d  le = y..useema =
+000003a0: 206e 0d0a 0d0a 5b66 696c 7465 7273 5d0d   n....[filters].
+000003b0: 0a63 6f6e 736f 6c69 6461 7469 6f6e 7065  .consolidationpe
+000003c0: 7263 656e 7461 6765 203d 2031 302e 300d  rcentage = 10.0.
+000003d0: 0a6d 6178 7072 6963 6520 3d20 3530 3030  .maxprice = 5000
+000003e0: 302e 300d 0a6d 696e 696d 756d 6368 616e  0.0..minimumchan
+000003f0: 6765 7065 7263 656e 7461 6765 203d 2030  gepercentage = 0
+00000400: 2e30 0d0a 6d69 6e69 6d75 6d76 6f6c 756d  .0..minimumvolum
+00000410: 6520 3d20 3130 3030 300d 0a6d 696e 7072  e = 10000..minpr
+00000420: 6963 6520 3d20 3230 2e30 0d0a 766f 6c75  ice = 20.0..volu
+00000430: 6d65 7261 7469 6f20 3d20 322e 350d 0a0d  meratio = 2.5...
+00000440: 0a                                       .
```

### Comparing `pkscreener-0.44.20240517.381/pkscreener/pkscreenerbot.py` & `pkscreener-0.45.20240517.382/pkscreener/pkscreenerbot.py`

 * *Files 0% similar despite different names*

```diff
@@ -496,15 +496,15 @@
                 elif selection[2] in SCANNER_MENUS_WITH_NO_SUBMENUS:  # Vol gainer ratio
                     selection.extend(["", ""])
     elif len(selection) == 4:
         preSelection = (
             query.data.upper().replace("CX", "X").replace("CB", "B").replace("CG", "G")
         )
     optionChoices = ""
-    if len(selection) <= 3:
+    if len(selection) <= 3 and mns is not None:
         for mnu in mns:
             inlineMenus.append(
                 InlineKeyboardButton(
                     mnu.menuKey,
                     callback_data="C" + str(f"{preSelection}_{mnu.menuKey}"),
                 )
             )
```

### Comparing `pkscreener-0.44.20240517.381/pkscreener/pkscreenercli.py` & `pkscreener-0.45.20240517.382/pkscreener/pkscreenercli.py`

 * *Files 4% similar despite different names*

```diff
@@ -161,14 +161,17 @@
     help="Use Intraday configurations and use the candlestick duration that is passed. Acceptable values 1m, 5m, 10m, 15m, 1h etc.",
     required=False,
 )
 argParser.add_argument(
     "-m",
     "--monitor",
     help="Monitor for intraday scanners and their results.",
+    nargs='?',
+    const='X',
+    type=str,
     required=False,
 )
 argParser.add_argument(
     "--maxdisplayresults",
     help="Maximum number of results to display.",
     required=False,
 )
@@ -210,14 +213,20 @@
 argParser.add_argument(
     "--singlethread",
     action="store_true",
     help="Run analysis for debugging purposes in a single process, single threaded environment",
     required=False,
 )
 argParser.add_argument(
+    "--systemlaunched",
+    action="store_true",
+    help="Indicator to show that this is a system launched screener, using os.system",
+    required=False,
+)
+argParser.add_argument(
     "-t",
     "--testbuild",
     action="store_true",
     help="Run in test-build mode",
     required=False,
 )
 argParser.add_argument(
@@ -259,34 +268,35 @@
 resultStocks = None
 plainResults = None
 start_time = None
 dbTimestamp = None
 elapsed_time = None
 configManager = ConfigManager.tools()
 
-def removeMonitorFile():
+def exitGracefully():
     from PKDevTools.classes import Archiver
     from pkscreener.globals import resetConfigToDefault
     filePath = os.path.join(Archiver.get_user_outputs_dir(), "monitor_outputs")
     index = 0
     while index < configManager.maxDashboardWidgetsPerRow*configManager.maxNumResultRowsInMonitor:
         try:
             os.remove(f"{filePath}_{index}.txt")
         except:
             pass
         index += 1
+
     argsv = argParser.parse_known_args()
     args = argsv[0]
     if args is not None and args.options is not None and not args.options.upper().startswith("T"):
         resetConfigToDefault()
-    if args.monitor is not None:
-        if "PKDevTools_Default_Log_Level" in os.environ.keys():
-            if args is None or (args is not None and args.options is not None and "|" not in args.options):
-                del os.environ['PKDevTools_Default_Log_Level']
-        configManager.logsEnabled = False
+        
+    if "PKDevTools_Default_Log_Level" in os.environ.keys():
+        if args is None or (args is not None and args.options is not None and "|" not in args.options):
+            del os.environ['PKDevTools_Default_Log_Level']
+    configManager.logsEnabled = False
     configManager.setConfig(ConfigManager.parser,default=True,showFileCreatedText=False)
 
 def logFilePath():
     try:
         from PKDevTools.classes import Archiver
 
         filePath = os.path.join(Archiver.get_user_outputs_dir(), "pkscreener-logs.txt")
@@ -355,14 +365,16 @@
     try:
         savedPipedArgs = None
         savedPipedArgs = args.pipedmenus if args is not None and args.pipedmenus is not None else None
     except:
         pass
     argsv = argParser.parse_known_args()
     args = argsv[0]
+    if args.systemlaunched:
+        args.systemlaunched = args.options
     # if sys.argv[0].endswith(".py"):
     #     args.monitor = 'X'
     #     args.answerdefault = 'Y'
     args.pipedmenus = savedPipedArgs
     if args.options is not None:
         args.options = args.options.replace("::",":")
     if args.runintradayanalysis:
@@ -481,15 +493,15 @@
                 results, plainResults = main(userArgs=args)
                 if args.pipedmenus is not None:
                     while args.pipedmenus is not None:
                         results, plainResults = main(userArgs=args)
                     sys.exit(0)
                 if isInterrupted():
                     closeWorkersAndExit()
-                    removeMonitorFile()
+                    exitGracefully()
                     sys.exit(0)
                 runPipedScans = True
                 while runPipedScans:
                     runPipedScans = pipeResults(plainResults,args)
                     if runPipedScans:
                         results, plainResults = main(userArgs=args)
                     else:
@@ -499,36 +511,37 @@
                                     + f"[+] Pipe Results Found: {args.pipedtitle}. {'Reduce number of piped scans if no stocks could be found.' if '[0]' in args.pipedtitle else ''}"
                                     + colorText.END
                                 )
                             if args.answerdefault is None:
                                 input("Press <Enter> to continue...")
             except SystemExit:
                 closeWorkersAndExit()
-                removeMonitorFile()
+                exitGracefully()
                 sys.exit(0)
             except Exception as e:
                 default_logger().debug(e, exc_info=True)
                 # Probably user cancelled an operation by choosing a cancel sub-menu somewhere
                 pass
             if plainResults is not None and not plainResults.empty:
                 try:
                     plainResults.set_index("Stock", inplace=True)
                 except:
                     pass
                 try:
                     results.set_index("Stock", inplace=True)
                 except:
                     pass
-                # plainResults = plainResults[~plainResults.index.duplicated(keep='first')]
-                # results = results[~results.index.duplicated(keep='first')]
+                plainResults = plainResults[~plainResults.index.duplicated(keep='first')]
+                results = results[~results.index.duplicated(keep='first')]
                 resultStocks = plainResults.index
             if args.monitor is not None:
                 MarketMonitor().saveMonitorResultStocks(plainResults)
                 if results is not None and len(monitorOption_org) > 0:
-                    MarketMonitor().refresh(screen_df=results,screenOptions=monitorOption_org, chosenMenu=updateMenuChoiceHierarchy(),dbTimestamp=f"{dbTimestamp} | CycleTime:{elapsed_time}s",telegram=args.telegram)
+                    chosenMenu = args.pipedtitle if args.pipedtitle is not None else updateMenuChoiceHierarchy()
+                    MarketMonitor().refresh(screen_df=results,screenOptions=monitorOption_org, chosenMenu=chosenMenu[:120],dbTimestamp=f"{dbTimestamp} | CycleTime:{elapsed_time}s",telegram=args.telegram)
 
 def checkIntradayComponent(args, monitorOption):
     lastComponent = monitorOption.split(":")[-1]
                 # previousCandleDuration = configManager.duration
     if "i" in lastComponent:
                     # We need to switch to intraday scan
         monitorOption = monitorOption.replace(lastComponent,"")
@@ -567,16 +580,16 @@
                 monitorOption = ":".join(monitorOptions)
             # We need to pipe the output from previous run into the next one
             if prevOutput is not None and not prevOutput.empty:
                 try:
                     prevOutput.set_index("Stock", inplace=True)
                 except:
                     pass
-                # prevOutput_results = prevOutput[~prevOutput.index.duplicated(keep='first')]
-                prevOutput_results = prevOutput.index
+                prevOutput_results = prevOutput[~prevOutput.index.duplicated(keep='first')]
+                prevOutput_results = prevOutput_results.index
                 hasFoundStocks = len(prevOutput_results) > 0
                 prevOutput_results = ",".join(prevOutput_results)
                 monitorOption = monitorOption.replace(":D:",":")
                 monitorOption = f"{monitorOption}:{prevOutput_results}"
         args.options = monitorOption.replace("::",":")
         args.options = args.options + ":D:>" + ":D:>".join(nextOnes[2:])
         args.options = args.options.replace("::",":")
@@ -594,20 +607,22 @@
                     "[+] RuntimeError with 'multiprocessing'.\n[+] Please contact the Developer, if this does not work!"
                 )
                 OutputControls().printOutput(e)
                 traceback.print_exc()
             pass
 
     OutputControls(enableMultipleLineOutput=(args.monitor is None)).printOutput("",end="\r")
-        
+    
     configManager.getConfig(ConfigManager.parser)
+    import atexit
+    atexit.register(exitGracefully)
     # configManager.restartRequestsCache()
     # args.monitor = configManager.defaultMonitorOptions
     if args.monitor is not None:
-        MarketMonitor(monitors=args.monitor.split(",") if len(args.monitor)>5 else configManager.defaultMonitorOptions.split(","),
+        MarketMonitor(monitors=args.monitor.split("~") if len(args.monitor)>5 else configManager.defaultMonitorOptions.split("~"),
                       maxNumResultsPerRow=configManager.maxDashboardWidgetsPerRow,
                       maxNumColsInEachResult=6,
                       maxNumRowsInEachResult=10,
                       maxNumResultRowsInMonitor=configManager.maxNumResultRowsInMonitor)
 
     if args.log or configManager.logsEnabled:
         setupLogger(shouldLog=True, trace=args.testbuild)
@@ -634,25 +649,26 @@
     if args.prodbuild:
         disableSysOut()
 
     if not configManager.checkConfigFile():
         configManager.setConfig(
             ConfigManager.parser, default=True, showFileCreatedText=False
         )
+    if args.systemlaunched:
+        args.systemlaunched = args.options
+        
     if args.telegram:
         # Launched by bot for intraday monitor?
         if (PKDateUtilities.isTradingTime() and not PKDateUtilities.isTodayHoliday()[0]) or ("PKDevTools_Default_Log_Level" in os.environ.keys()):
             from PKDevTools.classes import Archiver
             filePath = os.path.join(Archiver.get_user_outputs_dir(), "monitor_outputs_0.txt")
             if os.path.exists(filePath):
                 default_logger().info("monitor_outputs_0.txt already exists! This means an instance may already be running. Exiting now...")
                 # Since the file exists, it means, there is another instance running
                 sys.exit(0)
-            import atexit
-            atexit.register(removeMonitorFile)
         else:
             # It should have been launched only during the trading hours
             default_logger().info("--telegram option must be launched ONLY during NSE trading hours. Exiting now...")
             sys.exit(0)
     # Check and see if we're running only the telegram bot
     if args.bot:
         from pkscreener import pkscreenerbot
@@ -691,15 +707,15 @@
             + colorText.END
         )
         if args.intraday is None:
             configManager.toggleConfig(candleDuration="1d", clearCache=False)
         runApplication()
         from pkscreener.globals import closeWorkersAndExit
         closeWorkersAndExit()
-        removeMonitorFile()
+        exitGracefully()
         sys.exit(0)
     else:
         runApplicationForScreening()
 
 def runLoopOnScheduleOrStdApplication(hasCronInterval):
     if hasCronInterval:
         scheduleNextRun()
@@ -716,34 +732,34 @@
             if shouldBreak:
                 break
             runLoopOnScheduleOrStdApplication(hasCronInterval)
         if args.v:
             disableSysOut(disable=False)
             return
         closeWorkersAndExit()
-        removeMonitorFile()
+        exitGracefully()
         sys.exit(0)
     except SystemExit:
         closeWorkersAndExit()
-        removeMonitorFile()
+        exitGracefully()
         sys.exit(0)
     except (RuntimeError, Exception) as e:  # pragma: no cover
         default_logger().debug(e, exc_info=True)
         if args.prodbuild:
             disableSysOut(disable=False)
         OutputControls().printOutput(
             f"{e}\n[+] An error occurred! Please run with '-l' option to collect the logs.\n[+] For example, 'pkscreener -l' and then contact the developer!"
         )
         if "RUNNER" in os.environ.keys() or ('PKDevTools_Default_Log_Level' in os.environ.keys() and os.environ["PKDevTools_Default_Log_Level"] != str(log.logging.NOTSET)):
             traceback.print_exc()
         if args.v:
             disableSysOut(disable=False)
             return
         closeWorkersAndExit()
-        removeMonitorFile()
+        exitGracefully()
         sys.exit(0)
 
 
 def scheduleNextRun():
     sleepUntilNextExecution = not PKDateUtilities.isTradingTime()
     while sleepUntilNextExecution:
         OutputControls().printOutput(
```

### Comparing `pkscreener-0.44.20240517.381/pkscreener.egg-info/PKG-INFO` & `pkscreener-0.45.20240517.382/pkscreener.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pkscreener
-Version: 0.44.20240517.381
+Version: 0.45.20240517.382
 Summary: A Python-based stock screener for NSE, India with alerts to Telegram Channel (pkscreener)
 Home-page: https://github.com/pkjmesra/pkscreener
-Download-URL: https://github.com/pkjmesra/pkscreener/archive/v0.44.20240517.381.zip
+Download-URL: https://github.com/pkjmesra/pkscreener/archive/v0.45.20240517.382.zip
 Author: pkjmesra
 Author-email: pkjmesra@gmail.com
 License: OSI Approved (MIT)
 Keywords: NSE,Technical Indicators,Scanning,Stock Scanners
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS
@@ -269,19 +269,19 @@
 * Always backtest and analyze the stocks manually before you trade.
 * The Author(s), the software and any related/unrelated entity will not be held liable for your own investing decisions or losses. The authors or this softfware does not make any claim about the correctness of the results.
 * This screener began as a [fork](https://github.com/pranjal-joshi/Screeni-py) but has since added a lot of additional scanners, backtesting, Telegram bots, Alerts and a number of modifications and improvements.
 
 [MADE-IN-INDIA-badge]: https://img.shields.io/badge/MADE%20WITH%20%E2%9D%A4%20IN-INDIA-orange
 [MADE-IN-INDIA]: https://en.wikipedia.org/wiki/India
 [Windows-badge]: https://img.shields.io/badge/Windows-0078D6?logo=windows&logoColor=white
-[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240517.380/pkscreenercli.exe
+[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240517.381/pkscreenercli.exe
 [Linux-badge]: https://img.shields.io/badge/Linux-FCC624?logo=linux&logoColor=black
-[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240517.380/pkscreenercli.bin
+[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240517.381/pkscreenercli.bin
 [Mac OS-badge]: https://img.shields.io/badge/mac%20os-D3D3D3?logo=apple&logoColor=000000
-[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240517.380/pkscreenercli.run
+[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240517.381/pkscreenercli.run
 [GitHub release (latest by date)-badge]: https://img.shields.io/github/v/release/pkjmesra/PKScreener
 [GitHub release (latest by date)]: https://github.com/pkjmesra/PKScreener/releases/latest
 [pypi-badge]: https://img.shields.io/pypi/v/pkscreener.svg?style=flat-square
 [pypi]: https://pypi.python.org/pypi/pkscreener
 [wheel-badge]: https://img.shields.io/pypi/wheel/pkscreener.svg?style=flat-square
 [GitHub all releases]: https://img.shields.io/github/downloads/pkjmesra/PKScreener/total?color=Green&label=Downloads&style=for-the-badge
 [License-badge]: https://img.shields.io/github/license/pkjmesra/PKScreener?style=for-the-badge
```

### Comparing `pkscreener-0.44.20240517.381/pkscreener.egg-info/SOURCES.txt` & `pkscreener-0.45.20240517.382/pkscreener.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240517.381/setup.py` & `pkscreener-0.45.20240517.382/setup.py`

 * *Files identical despite different names*

