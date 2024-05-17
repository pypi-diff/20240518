# Comparing `tmp/pkscreener-0.44.20240517.380.tar.gz` & `tmp/pkscreener-0.44.20240517.381.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pkscreener-0.44.20240517.380.tar", last modified: Fri May 17 03:37:14 2024, max compression
+gzip compressed data, was "pkscreener-0.44.20240517.381.tar", last modified: Fri May 17 07:37:22 2024, max compression
```

## Comparing `pkscreener-0.44.20240517.380.tar` & `pkscreener-0.44.20240517.381.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxrwxrwx   0        0        0        0 2024-05-17 03:37:14.339276 pkscreener-0.44.20240517.380/
--rw-rw-rw-   0        0        0     1086 2024-05-17 03:32:25.000000 pkscreener-0.44.20240517.380/LICENSE
--rw-rw-rw-   0        0        0     1091 2024-05-17 03:32:25.000000 pkscreener-0.44.20240517.380/LICENSE-Others
--rw-rw-rw-   0        0        0    27795 2024-05-17 03:37:14.339276 pkscreener-0.44.20240517.380/PKG-INFO
--rw-rw-rw-   0        0        0    26856 2024-05-17 03:32:25.000000 pkscreener-0.44.20240517.380/README.md
-drwxrwxrwx   0        0        0        0 2024-05-17 03:37:14.323648 pkscreener-0.44.20240517.380/pkscreener/
--rw-rw-rw-   0        0        0     1582 2024-05-17 03:32:25.000000 pkscreener-0.44.20240517.380/pkscreener/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-17 03:37:14.339276 pkscreener-0.44.20240517.380/pkscreener/classes/
--rw-rw-rw-   0        0        0    13324 2024-05-17 03:32:25.000000 pkscreener-0.44.20240517.380/pkscreener/classes/ArtTexts.py
--rw-rw-rw-   0        0        0    10156 2024-05-17 03:32:25.000000 pkscreener-0.44.20240517.380/pkscreener/classes/Backtest.py
--rw-rw-rw-   0        0        0     5705 2024-05-17 03:32:25.000000 pkscreener-0.44.20240517.380/pkscreener/classes/Barometer.py
--rw-rw-rw-   0        0        0    17333 2024-05-17 03:32:25.000000 pkscreener-0.44.20240517.380/pkscreener/classes/CandlePatterns.py
--rw-rw-rw-   0        0        0     1537 2024-05-17 03:32:25.000000 pkscreener-0.44.20240517.380/pkscreener/classes/Changelog.py
--rw-rw-rw-   0        0        0    34250 2024-05-17 03:32:25.000000 pkscreener-0.44.20240517.380/pkscreener/classes/ConfigManager.py
--rw-rw-rw-   0        0        0    10076 2024-05-17 03:32:25.000000 pkscreener-0.44.20240517.380/pkscreener/classes/Fetcher.py
--rw-rw-rw-   0        0        0    11407 2024-05-17 03:32:25.000000 pkscreener-0.44.20240517.380/pkscreener/classes/MarketMonitor.py
--rw-rw-rw-   0        0        0     3673 2024-05-17 03:32:25.000000 pkscreener-0.44.20240517.380/pkscreener/classes/MarketStatus.py
--rw-rw-rw-   0        0        0    43311 2024-05-17 03:32:25.000000 pkscreener-0.44.20240517.380/pkscreener/classes/MenuOptions.py
--rw-rw-rw-   0        0        0    12534 2024-05-17 03:32:25.000000 pkscreener-0.44.20240517.380/pkscreener/classes/OtaUpdater.py
--rw-rw-rw-   0        0        0    24598 2024-05-17 03:32:25.000000 pkscreener-0.44.20240517.380/pkscreener/classes/PKMarketOpenCloseAnalyser.py
--rw-rw-rw-   0        0        0    22369 2024-05-17 03:32:25.000000 pkscreener-0.44.20240517.380/pkscreener/classes/PKScanRunner.py
--rw-rw-rw-   0        0        0     1623 2024-05-17 03:32:25.000000 pkscreener-0.44.20240517.380/pkscreener/classes/PKScheduledTaskProgress.py
--rw-rw-rw-   0        0        0     8158 2024-05-17 03:32:25.000000 pkscreener-0.44.20240517.380/pkscreener/classes/PKScheduler.py
--rw-rw-rw-   0        0        0     8466 2024-05-17 03:32:25.000000 pkscreener-0.44.20240517.380/pkscreener/classes/PKSpreadsheets.py
--rw-rw-rw-   0        0        0     1907 2024-05-17 03:32:25.000000 pkscreener-0.44.20240517.380/pkscreener/classes/PKTask.py
--rw-rw-rw-   0        0        0    18947 2024-05-17 03:32:25.000000 pkscreener-0.44.20240517.380/pkscreener/classes/Pktalib.py
--rw-rw-rw-   0        0        0    14177 2024-05-17 03:32:25.000000 pkscreener-0.44.20240517.380/pkscreener/classes/Portfolio.py
--rw-rw-rw-   0        0        0    49043 2024-05-17 03:32:25.000000 pkscreener-0.44.20240517.380/pkscreener/classes/PortfolioXRay.py
--rw-rw-rw-   0        0        0   156140 2024-05-17 03:32:25.000000 pkscreener-0.44.20240517.380/pkscreener/classes/ScreeningStatistics.py
--rw-rw-rw-   0        0        0    56357 2024-05-17 03:32:25.000000 pkscreener-0.44.20240517.380/pkscreener/classes/StockScreener.py
--rw-rw-rw-   0        0        0     4993 2024-05-17 03:32:25.000000 pkscreener-0.44.20240517.380/pkscreener/classes/UserMenuChoicesHandler.py
--rw-rw-rw-   0        0        0    84725 2024-05-17 03:32:25.000000 pkscreener-0.44.20240517.380/pkscreener/classes/Utility.py
--rw-rw-rw-   0        0        0     3789 2024-05-17 03:32:25.000000 pkscreener-0.44.20240517.380/pkscreener/classes/WorkflowManager.py
--rw-rw-rw-   0        0        0       28 2024-05-17 03:37:04.000000 pkscreener-0.44.20240517.380/pkscreener/classes/__init__.py
--rw-rw-rw-   0        0        0     5262 2024-05-17 03:32:25.000000 pkscreener-0.44.20240517.380/pkscreener/classes/keys.py
--rw-rw-rw-   0        0        0   791436 2024-05-17 03:32:25.000000 pkscreener-0.44.20240517.380/pkscreener/courbd.ttf
--rw-rw-rw-   0        0        0   141484 2024-05-17 03:32:25.000000 pkscreener-0.44.20240517.380/pkscreener/globals.py
--rw-rw-rw-   0        0        0     1090 2024-05-17 03:32:25.000000 pkscreener-0.44.20240517.380/pkscreener/pkscreener.ini
--rw-rw-rw-   0        0        0    53036 2024-05-17 03:32:25.000000 pkscreener-0.44.20240517.380/pkscreener/pkscreenerbot.py
--rw-rw-rw-   0        0        0    33946 2024-05-17 03:32:25.000000 pkscreener-0.44.20240517.380/pkscreener/pkscreenercli.py
-drwxrwxrwx   0        0        0        0 2024-05-17 03:37:14.339276 pkscreener-0.44.20240517.380/pkscreener.egg-info/
--rw-rw-rw-   0        0        0    27795 2024-05-17 03:37:14.000000 pkscreener-0.44.20240517.380/pkscreener.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1349 2024-05-17 03:37:14.000000 pkscreener-0.44.20240517.380/pkscreener.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-17 03:37:14.000000 pkscreener-0.44.20240517.380/pkscreener.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      120 2024-05-17 03:37:14.000000 pkscreener-0.44.20240517.380/pkscreener.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2024-05-17 03:37:14.000000 pkscreener-0.44.20240517.380/pkscreener.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       11 2024-05-17 03:37:14.000000 pkscreener-0.44.20240517.380/pkscreener.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2024-05-17 03:37:14.339276 pkscreener-0.44.20240517.380/setup.cfg
--rw-rw-rw-   0        0        0     4765 2024-05-17 03:32:26.000000 pkscreener-0.44.20240517.380/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-17 07:37:22.112404 pkscreener-0.44.20240517.381/
+-rw-rw-rw-   0        0        0     1086 2024-05-17 07:34:02.000000 pkscreener-0.44.20240517.381/LICENSE
+-rw-rw-rw-   0        0        0     1091 2024-05-17 07:34:02.000000 pkscreener-0.44.20240517.381/LICENSE-Others
+-rw-rw-rw-   0        0        0    27795 2024-05-17 07:37:22.112404 pkscreener-0.44.20240517.381/PKG-INFO
+-rw-rw-rw-   0        0        0    26856 2024-05-17 07:34:02.000000 pkscreener-0.44.20240517.381/README.md
+drwxrwxrwx   0        0        0        0 2024-05-17 07:37:22.096787 pkscreener-0.44.20240517.381/pkscreener/
+-rw-rw-rw-   0        0        0     1582 2024-05-17 07:34:02.000000 pkscreener-0.44.20240517.381/pkscreener/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-17 07:37:22.112404 pkscreener-0.44.20240517.381/pkscreener/classes/
+-rw-rw-rw-   0        0        0    13324 2024-05-17 07:34:02.000000 pkscreener-0.44.20240517.381/pkscreener/classes/ArtTexts.py
+-rw-rw-rw-   0        0        0    10156 2024-05-17 07:34:02.000000 pkscreener-0.44.20240517.381/pkscreener/classes/Backtest.py
+-rw-rw-rw-   0        0        0     5705 2024-05-17 07:34:02.000000 pkscreener-0.44.20240517.381/pkscreener/classes/Barometer.py
+-rw-rw-rw-   0        0        0    17333 2024-05-17 07:34:02.000000 pkscreener-0.44.20240517.381/pkscreener/classes/CandlePatterns.py
+-rw-rw-rw-   0        0        0     1537 2024-05-17 07:34:02.000000 pkscreener-0.44.20240517.381/pkscreener/classes/Changelog.py
+-rw-rw-rw-   0        0        0    34250 2024-05-17 07:34:02.000000 pkscreener-0.44.20240517.381/pkscreener/classes/ConfigManager.py
+-rw-rw-rw-   0        0        0    10076 2024-05-17 07:34:02.000000 pkscreener-0.44.20240517.381/pkscreener/classes/Fetcher.py
+-rw-rw-rw-   0        0        0    11572 2024-05-17 07:34:02.000000 pkscreener-0.44.20240517.381/pkscreener/classes/MarketMonitor.py
+-rw-rw-rw-   0        0        0     3673 2024-05-17 07:34:02.000000 pkscreener-0.44.20240517.381/pkscreener/classes/MarketStatus.py
+-rw-rw-rw-   0        0        0    43311 2024-05-17 07:34:02.000000 pkscreener-0.44.20240517.381/pkscreener/classes/MenuOptions.py
+-rw-rw-rw-   0        0        0    12534 2024-05-17 07:34:02.000000 pkscreener-0.44.20240517.381/pkscreener/classes/OtaUpdater.py
+-rw-rw-rw-   0        0        0    24598 2024-05-17 07:34:02.000000 pkscreener-0.44.20240517.381/pkscreener/classes/PKMarketOpenCloseAnalyser.py
+-rw-rw-rw-   0        0        0    22369 2024-05-17 07:34:02.000000 pkscreener-0.44.20240517.381/pkscreener/classes/PKScanRunner.py
+-rw-rw-rw-   0        0        0     1623 2024-05-17 07:34:02.000000 pkscreener-0.44.20240517.381/pkscreener/classes/PKScheduledTaskProgress.py
+-rw-rw-rw-   0        0        0     8158 2024-05-17 07:34:02.000000 pkscreener-0.44.20240517.381/pkscreener/classes/PKScheduler.py
+-rw-rw-rw-   0        0        0     8466 2024-05-17 07:34:02.000000 pkscreener-0.44.20240517.381/pkscreener/classes/PKSpreadsheets.py
+-rw-rw-rw-   0        0        0     1907 2024-05-17 07:34:02.000000 pkscreener-0.44.20240517.381/pkscreener/classes/PKTask.py
+-rw-rw-rw-   0        0        0    18947 2024-05-17 07:34:02.000000 pkscreener-0.44.20240517.381/pkscreener/classes/Pktalib.py
+-rw-rw-rw-   0        0        0    14177 2024-05-17 07:34:02.000000 pkscreener-0.44.20240517.381/pkscreener/classes/Portfolio.py
+-rw-rw-rw-   0        0        0    49043 2024-05-17 07:34:02.000000 pkscreener-0.44.20240517.381/pkscreener/classes/PortfolioXRay.py
+-rw-rw-rw-   0        0        0   156140 2024-05-17 07:34:02.000000 pkscreener-0.44.20240517.381/pkscreener/classes/ScreeningStatistics.py
+-rw-rw-rw-   0        0        0    56357 2024-05-17 07:34:02.000000 pkscreener-0.44.20240517.381/pkscreener/classes/StockScreener.py
+-rw-rw-rw-   0        0        0     4993 2024-05-17 07:34:02.000000 pkscreener-0.44.20240517.381/pkscreener/classes/UserMenuChoicesHandler.py
+-rw-rw-rw-   0        0        0    84725 2024-05-17 07:34:02.000000 pkscreener-0.44.20240517.381/pkscreener/classes/Utility.py
+-rw-rw-rw-   0        0        0     3789 2024-05-17 07:34:02.000000 pkscreener-0.44.20240517.381/pkscreener/classes/WorkflowManager.py
+-rw-rw-rw-   0        0        0       28 2024-05-17 07:37:14.000000 pkscreener-0.44.20240517.381/pkscreener/classes/__init__.py
+-rw-rw-rw-   0        0        0     5262 2024-05-17 07:34:02.000000 pkscreener-0.44.20240517.381/pkscreener/classes/keys.py
+-rw-rw-rw-   0        0        0   791436 2024-05-17 07:34:02.000000 pkscreener-0.44.20240517.381/pkscreener/courbd.ttf
+-rw-rw-rw-   0        0        0   141484 2024-05-17 07:34:02.000000 pkscreener-0.44.20240517.381/pkscreener/globals.py
+-rw-rw-rw-   0        0        0     1090 2024-05-17 07:34:02.000000 pkscreener-0.44.20240517.381/pkscreener/pkscreener.ini
+-rw-rw-rw-   0        0        0    53036 2024-05-17 07:34:02.000000 pkscreener-0.44.20240517.381/pkscreener/pkscreenerbot.py
+-rw-rw-rw-   0        0        0    33946 2024-05-17 07:34:02.000000 pkscreener-0.44.20240517.381/pkscreener/pkscreenercli.py
+drwxrwxrwx   0        0        0        0 2024-05-17 07:37:22.112404 pkscreener-0.44.20240517.381/pkscreener.egg-info/
+-rw-rw-rw-   0        0        0    27795 2024-05-17 07:37:22.000000 pkscreener-0.44.20240517.381/pkscreener.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1349 2024-05-17 07:37:22.000000 pkscreener-0.44.20240517.381/pkscreener.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-17 07:37:22.000000 pkscreener-0.44.20240517.381/pkscreener.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      120 2024-05-17 07:37:22.000000 pkscreener-0.44.20240517.381/pkscreener.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2024-05-17 07:37:22.000000 pkscreener-0.44.20240517.381/pkscreener.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       11 2024-05-17 07:37:22.000000 pkscreener-0.44.20240517.381/pkscreener.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2024-05-17 07:37:22.128034 pkscreener-0.44.20240517.381/setup.cfg
+-rw-rw-rw-   0        0        0     4765 2024-05-17 07:34:02.000000 pkscreener-0.44.20240517.381/setup.py
```

### Comparing `pkscreener-0.44.20240517.380/LICENSE` & `pkscreener-0.44.20240517.381/LICENSE`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240517.380/LICENSE-Others` & `pkscreener-0.44.20240517.381/LICENSE-Others`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240517.380/PKG-INFO` & `pkscreener-0.44.20240517.381/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pkscreener
-Version: 0.44.20240517.380
+Version: 0.44.20240517.381
 Summary: A Python-based stock screener for NSE, India with alerts to Telegram Channel (pkscreener)
 Home-page: https://github.com/pkjmesra/pkscreener
-Download-URL: https://github.com/pkjmesra/pkscreener/archive/v0.44.20240517.380.zip
+Download-URL: https://github.com/pkjmesra/pkscreener/archive/v0.44.20240517.381.zip
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
-[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240516.379/pkscreenercli.exe
+[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240517.380/pkscreenercli.exe
 [Linux-badge]: https://img.shields.io/badge/Linux-FCC624?logo=linux&logoColor=black
-[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240516.379/pkscreenercli.bin
+[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240517.380/pkscreenercli.bin
 [Mac OS-badge]: https://img.shields.io/badge/mac%20os-D3D3D3?logo=apple&logoColor=000000
-[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240516.379/pkscreenercli.run
+[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240517.380/pkscreenercli.run
 [GitHub release (latest by date)-badge]: https://img.shields.io/github/v/release/pkjmesra/PKScreener
 [GitHub release (latest by date)]: https://github.com/pkjmesra/PKScreener/releases/latest
 [pypi-badge]: https://img.shields.io/pypi/v/pkscreener.svg?style=flat-square
 [pypi]: https://pypi.python.org/pypi/pkscreener
 [wheel-badge]: https://img.shields.io/pypi/wheel/pkscreener.svg?style=flat-square
 [GitHub all releases]: https://img.shields.io/github/downloads/pkjmesra/PKScreener/total?color=Green&label=Downloads&style=for-the-badge
 [License-badge]: https://img.shields.io/github/license/pkjmesra/PKScreener?style=for-the-badge
```

### Comparing `pkscreener-0.44.20240517.380/README.md` & `pkscreener-0.44.20240517.381/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -247,19 +247,19 @@
 * Always backtest and analyze the stocks manually before you trade.
 * The Author(s), the software and any related/unrelated entity will not be held liable for your own investing decisions or losses. The authors or this softfware does not make any claim about the correctness of the results.
 * This screener began as a [fork](https://github.com/pranjal-joshi/Screeni-py) but has since added a lot of additional scanners, backtesting, Telegram bots, Alerts and a number of modifications and improvements.
 
 [MADE-IN-INDIA-badge]: https://img.shields.io/badge/MADE%20WITH%20%E2%9D%A4%20IN-INDIA-orange
 [MADE-IN-INDIA]: https://en.wikipedia.org/wiki/India
 [Windows-badge]: https://img.shields.io/badge/Windows-0078D6?logo=windows&logoColor=white
-[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240516.379/pkscreenercli.exe
+[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240517.380/pkscreenercli.exe
 [Linux-badge]: https://img.shields.io/badge/Linux-FCC624?logo=linux&logoColor=black
-[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240516.379/pkscreenercli.bin
+[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240517.380/pkscreenercli.bin
 [Mac OS-badge]: https://img.shields.io/badge/mac%20os-D3D3D3?logo=apple&logoColor=000000
-[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240516.379/pkscreenercli.run
+[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240517.380/pkscreenercli.run
 [GitHub release (latest by date)-badge]: https://img.shields.io/github/v/release/pkjmesra/PKScreener
 [GitHub release (latest by date)]: https://github.com/pkjmesra/PKScreener/releases/latest
 [pypi-badge]: https://img.shields.io/pypi/v/pkscreener.svg?style=flat-square
 [pypi]: https://pypi.python.org/pypi/pkscreener
 [wheel-badge]: https://img.shields.io/pypi/wheel/pkscreener.svg?style=flat-square
 [GitHub all releases]: https://img.shields.io/github/downloads/pkjmesra/PKScreener/total?color=Green&label=Downloads&style=for-the-badge
 [License-badge]: https://img.shields.io/github/license/pkjmesra/PKScreener?style=for-the-badge
```

### Comparing `pkscreener-0.44.20240517.380/pkscreener/__init__.py` & `pkscreener-0.44.20240517.381/pkscreener/__init__.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240517.380/pkscreener/classes/ArtTexts.py` & `pkscreener-0.44.20240517.381/pkscreener/classes/ArtTexts.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240517.380/pkscreener/classes/Backtest.py` & `pkscreener-0.44.20240517.381/pkscreener/classes/Backtest.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240517.380/pkscreener/classes/Barometer.py` & `pkscreener-0.44.20240517.381/pkscreener/classes/Barometer.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240517.380/pkscreener/classes/CandlePatterns.py` & `pkscreener-0.44.20240517.381/pkscreener/classes/CandlePatterns.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240517.380/pkscreener/classes/Changelog.py` & `pkscreener-0.44.20240517.381/pkscreener/classes/Changelog.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240517.380/pkscreener/classes/ConfigManager.py` & `pkscreener-0.44.20240517.381/pkscreener/classes/ConfigManager.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240517.380/pkscreener/classes/Fetcher.py` & `pkscreener-0.44.20240517.381/pkscreener/classes/Fetcher.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240517.380/pkscreener/classes/MarketMonitor.py` & `pkscreener-0.44.20240517.381/pkscreener/classes/MarketMonitor.py`

 * *Files 5% similar despite different names*

```diff
@@ -197,15 +197,17 @@
                             telegram_df,
                             headers="keys",
                             tablefmt=colorText.No_Pad_GridFormat,
                             showindex=False,
                             maxcolwidths=[None,None,4,3]
                         ).encode("utf-8").decode(STD_ENCODING).replace("-K-----S-----C-----R","-K-----S----C---R").replace("%  ","% ").replace("=K=====S=====C=====R","=K=====S====C===R").replace("Vol  |","Vol|").replace("x  ","x")
             telegram_df_tabulated = telegram_df_tabulated.replace("-E-----N-----E-----R","-E-----N----E---R").replace("=E=====N=====E=====R","=E=====N====E===R")
-            result_output = f"Latest data as of:{dbTimestamp}\n<b>{chosenMenu.split('>')[-1]}</b> [{screenOptions}]\n<pre>{telegram_df_tabulated}</pre>"
+            choiceSegments = chosenMenu.split(">")
+            chosenMenu = f"{choiceSegments[-2]} > {choiceSegments[-1]}" if len(choiceSegments)>=4 else f"{choiceSegments[-1]}"
+            result_output = f"Latest data as of:{dbTimestamp}\n<b>{chosenMenu}</b> [{screenOptions}]\n<pre>{telegram_df_tabulated}</pre>"
             try:
                 filePath = os.path.join(Archiver.get_user_outputs_dir(), f"monitor_outputs_{self.monitorIndex}.txt")
                 f = open(filePath, "w")
                 f.write(result_output)
                 f.close()
             except:
                 pass
```

### Comparing `pkscreener-0.44.20240517.380/pkscreener/classes/MarketStatus.py` & `pkscreener-0.44.20240517.381/pkscreener/classes/MarketStatus.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240517.380/pkscreener/classes/MenuOptions.py` & `pkscreener-0.44.20240517.381/pkscreener/classes/MenuOptions.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240517.380/pkscreener/classes/OtaUpdater.py` & `pkscreener-0.44.20240517.381/pkscreener/classes/OtaUpdater.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240517.380/pkscreener/classes/PKMarketOpenCloseAnalyser.py` & `pkscreener-0.44.20240517.381/pkscreener/classes/PKMarketOpenCloseAnalyser.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240517.380/pkscreener/classes/PKScanRunner.py` & `pkscreener-0.44.20240517.381/pkscreener/classes/PKScanRunner.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240517.380/pkscreener/classes/PKScheduledTaskProgress.py` & `pkscreener-0.44.20240517.381/pkscreener/classes/PKScheduledTaskProgress.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240517.380/pkscreener/classes/PKScheduler.py` & `pkscreener-0.44.20240517.381/pkscreener/classes/PKScheduler.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240517.380/pkscreener/classes/PKSpreadsheets.py` & `pkscreener-0.44.20240517.381/pkscreener/classes/PKSpreadsheets.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240517.380/pkscreener/classes/PKTask.py` & `pkscreener-0.44.20240517.381/pkscreener/classes/PKTask.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240517.380/pkscreener/classes/Pktalib.py` & `pkscreener-0.44.20240517.381/pkscreener/classes/Pktalib.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240517.380/pkscreener/classes/Portfolio.py` & `pkscreener-0.44.20240517.381/pkscreener/classes/Portfolio.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240517.380/pkscreener/classes/PortfolioXRay.py` & `pkscreener-0.44.20240517.381/pkscreener/classes/PortfolioXRay.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240517.380/pkscreener/classes/ScreeningStatistics.py` & `pkscreener-0.44.20240517.381/pkscreener/classes/ScreeningStatistics.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240517.380/pkscreener/classes/StockScreener.py` & `pkscreener-0.44.20240517.381/pkscreener/classes/StockScreener.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240517.380/pkscreener/classes/UserMenuChoicesHandler.py` & `pkscreener-0.44.20240517.381/pkscreener/classes/UserMenuChoicesHandler.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240517.380/pkscreener/classes/Utility.py` & `pkscreener-0.44.20240517.381/pkscreener/classes/Utility.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240517.380/pkscreener/classes/WorkflowManager.py` & `pkscreener-0.44.20240517.381/pkscreener/classes/WorkflowManager.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240517.380/pkscreener/classes/keys.py` & `pkscreener-0.44.20240517.381/pkscreener/classes/keys.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240517.380/pkscreener/courbd.ttf` & `pkscreener-0.44.20240517.381/pkscreener/courbd.ttf`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240517.380/pkscreener/globals.py` & `pkscreener-0.44.20240517.381/pkscreener/globals.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240517.380/pkscreener/pkscreener.ini` & `pkscreener-0.44.20240517.381/pkscreener/pkscreener.ini`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240517.380/pkscreener/pkscreenerbot.py` & `pkscreener-0.44.20240517.381/pkscreener/pkscreenerbot.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240517.380/pkscreener/pkscreenercli.py` & `pkscreener-0.44.20240517.381/pkscreener/pkscreenercli.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240517.380/pkscreener.egg-info/PKG-INFO` & `pkscreener-0.44.20240517.381/pkscreener.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pkscreener
-Version: 0.44.20240517.380
+Version: 0.44.20240517.381
 Summary: A Python-based stock screener for NSE, India with alerts to Telegram Channel (pkscreener)
 Home-page: https://github.com/pkjmesra/pkscreener
-Download-URL: https://github.com/pkjmesra/pkscreener/archive/v0.44.20240517.380.zip
+Download-URL: https://github.com/pkjmesra/pkscreener/archive/v0.44.20240517.381.zip
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
-[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240516.379/pkscreenercli.exe
+[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240517.380/pkscreenercli.exe
 [Linux-badge]: https://img.shields.io/badge/Linux-FCC624?logo=linux&logoColor=black
-[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240516.379/pkscreenercli.bin
+[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240517.380/pkscreenercli.bin
 [Mac OS-badge]: https://img.shields.io/badge/mac%20os-D3D3D3?logo=apple&logoColor=000000
-[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240516.379/pkscreenercli.run
+[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240517.380/pkscreenercli.run
 [GitHub release (latest by date)-badge]: https://img.shields.io/github/v/release/pkjmesra/PKScreener
 [GitHub release (latest by date)]: https://github.com/pkjmesra/PKScreener/releases/latest
 [pypi-badge]: https://img.shields.io/pypi/v/pkscreener.svg?style=flat-square
 [pypi]: https://pypi.python.org/pypi/pkscreener
 [wheel-badge]: https://img.shields.io/pypi/wheel/pkscreener.svg?style=flat-square
 [GitHub all releases]: https://img.shields.io/github/downloads/pkjmesra/PKScreener/total?color=Green&label=Downloads&style=for-the-badge
 [License-badge]: https://img.shields.io/github/license/pkjmesra/PKScreener?style=for-the-badge
```

### Comparing `pkscreener-0.44.20240517.380/pkscreener.egg-info/SOURCES.txt` & `pkscreener-0.44.20240517.381/pkscreener.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240517.380/setup.py` & `pkscreener-0.44.20240517.381/setup.py`

 * *Files identical despite different names*

