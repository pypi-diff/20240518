# Comparing `tmp/sarcharts-0.2.2.tar.gz` & `tmp/sarcharts-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sarcharts-0.2.2.tar", last modified: Thu May 16 07:33:02 2024, max compression
+gzip compressed data, was "sarcharts-0.2.3.tar", last modified: Sat May 18 13:03:03 2024, max compression
```

## Comparing `sarcharts-0.2.2.tar` & `sarcharts-0.2.3.tar`

### file list

```diff
@@ -1,54 +1,55 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 07:33:02.797346 sarcharts-0.2.2/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 07:33:02.789346 sarcharts-0.2.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 07:33:02.793346 sarcharts-0.2.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-05-16 07:32:57.000000 sarcharts-0.2.2/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3785 2024-05-16 07:32:57.000000 sarcharts-0.2.2/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-05-16 07:33:02.000000 sarcharts-0.2.2/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-16 07:33:02.000000 sarcharts-0.2.2/ChangeLog
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-16 07:32:57.000000 sarcharts-0.2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2024 2024-05-16 07:33:02.797346 sarcharts-0.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1117 2024-05-16 07:32:57.000000 sarcharts-0.2.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 07:33:02.793346 sarcharts-0.2.2/doc/
--rw-r--r--   0 runner    (1001) docker     (127)     1117 2024-05-16 07:32:57.000000 sarcharts-0.2.2/doc/README.md
--rw-r--r--   0 runner    (1001) docker     (127)   109472 2024-05-16 07:32:57.000000 sarcharts-0.2.2/doc/sarcharts.png
--rw-r--r--   0 runner    (1001) docker     (127)      295 2024-05-16 07:32:57.000000 sarcharts-0.2.2/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 07:33:02.793346 sarcharts-0.2.2/sarcharts/
--rw-r--r--   0 runner    (1001) docker     (127)     4029 2024-05-16 07:32:57.000000 sarcharts-0.2.2/sarcharts/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 07:33:02.793346 sarcharts-0.2.2/sarcharts/bin/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 07:32:57.000000 sarcharts-0.2.2/sarcharts/bin/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      204 2024-05-16 07:32:57.000000 sarcharts-0.2.2/sarcharts/bin/sarcharts.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 07:33:02.789346 sarcharts-0.2.2/sarcharts/html/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 07:33:02.793346 sarcharts-0.2.2/sarcharts/html/css/
--rw-r--r--   0 runner    (1001) docker     (127)     1939 2024-05-16 07:32:57.000000 sarcharts-0.2.2/sarcharts/html/css/sarcharts.css
--rw-r--r--   0 runner    (1001) docker     (127)     2171 2024-05-16 07:32:57.000000 sarcharts-0.2.2/sarcharts/html/css/ul-select.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 07:33:02.793346 sarcharts-0.2.2/sarcharts/html/img/
--rw-r--r--   0 runner    (1001) docker     (127)      158 2024-05-16 07:32:57.000000 sarcharts-0.2.2/sarcharts/html/img/chevron.svg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 07:33:02.797346 sarcharts-0.2.2/sarcharts/html/js/
--rw-r--r--   0 runner    (1001) docker     (127)   205214 2024-05-16 07:32:57.000000 sarcharts-0.2.2/sarcharts/html/js/chart.umd.js
--rw-r--r--   0 runner    (1001) docker     (127)    50650 2024-05-16 07:32:57.000000 sarcharts-0.2.2/sarcharts/html/js/chartjs-adapter-date-fns.bundle.min.js
--rw-r--r--   0 runner    (1001) docker     (127)    34500 2024-05-16 07:32:57.000000 sarcharts-0.2.2/sarcharts/html/js/chartjs-plugin-annotation.min.js
--rw-r--r--   0 runner    (1001) docker     (127)    12854 2024-05-16 07:32:57.000000 sarcharts-0.2.2/sarcharts/html/js/chartjs-plugin-zoom.min.js
--rw-r--r--   0 runner    (1001) docker     (127)    20765 2024-05-16 07:32:57.000000 sarcharts-0.2.2/sarcharts/html/js/hammer.min.js
--rw-r--r--   0 runner    (1001) docker     (127)   271751 2024-05-16 07:32:57.000000 sarcharts-0.2.2/sarcharts/html/js/jquery.js
--rw-r--r--   0 runner    (1001) docker     (127)     1343 2024-05-16 07:32:57.000000 sarcharts-0.2.2/sarcharts/html/js/ul-select.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 07:33:02.797346 sarcharts-0.2.2/sarcharts/lib/
--rw-r--r--   0 runner    (1001) docker     (127)     2417 2024-05-16 07:32:57.000000 sarcharts-0.2.2/sarcharts/lib/chartjs.py
--rw-r--r--   0 runner    (1001) docker     (127)     1789 2024-05-16 07:32:57.000000 sarcharts-0.2.2/sarcharts/lib/progressbar.py
--rw-r--r--   0 runner    (1001) docker     (127)    10685 2024-05-16 07:32:57.000000 sarcharts-0.2.2/sarcharts/lib/sadf.py
--rw-r--r--   0 runner    (1001) docker     (127)     2161 2024-05-16 07:32:57.000000 sarcharts-0.2.2/sarcharts/lib/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 07:33:02.797346 sarcharts-0.2.2/sarcharts/templates/
--rw-r--r--   0 runner    (1001) docker     (127)     5091 2024-05-16 07:32:57.000000 sarcharts-0.2.2/sarcharts/templates/chart.html
--rw-r--r--   0 runner    (1001) docker     (127)     1163 2024-05-16 07:32:57.000000 sarcharts-0.2.2/sarcharts/templates/header.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 07:33:02.797346 sarcharts-0.2.2/sarcharts.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2024 2024-05-16 07:33:02.000000 sarcharts-0.2.2/sarcharts.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1048 2024-05-16 07:33:02.000000 sarcharts-0.2.2/sarcharts.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 07:33:02.000000 sarcharts-0.2.2/sarcharts.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-16 07:33:02.000000 sarcharts-0.2.2/sarcharts.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 07:33:02.000000 sarcharts-0.2.2/sarcharts.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-16 07:33:02.000000 sarcharts-0.2.2/sarcharts.egg-info/pbr.json
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-16 07:33:02.000000 sarcharts-0.2.2/sarcharts.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-16 07:33:02.000000 sarcharts-0.2.2/sarcharts.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      828 2024-05-16 07:33:02.797346 sarcharts-0.2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      917 2024-05-16 07:32:57.000000 sarcharts-0.2.2/setup.py
--rw-r--r--   0 runner    (1001) docker     (127)      246 2024-05-16 07:32:57.000000 sarcharts-0.2.2/test-requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      787 2024-05-16 07:32:57.000000 sarcharts-0.2.2/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 13:03:03.508344 sarcharts-0.2.3/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 13:03:03.496344 sarcharts-0.2.3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 13:03:03.500344 sarcharts-0.2.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-05-18 13:02:57.000000 sarcharts-0.2.3/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3785 2024-05-18 13:02:57.000000 sarcharts-0.2.3/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-05-18 13:03:03.000000 sarcharts-0.2.3/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-18 13:03:03.000000 sarcharts-0.2.3/ChangeLog
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-18 13:02:57.000000 sarcharts-0.2.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2230 2024-05-18 13:03:03.508344 sarcharts-0.2.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1323 2024-05-18 13:02:57.000000 sarcharts-0.2.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 13:03:03.500344 sarcharts-0.2.3/doc/
+-rw-r--r--   0 runner    (1001) docker     (127)     1323 2024-05-18 13:02:57.000000 sarcharts-0.2.3/doc/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)   109472 2024-05-18 13:02:57.000000 sarcharts-0.2.3/doc/sarcharts.png
+-rw-r--r--   0 runner    (1001) docker     (127)      295 2024-05-18 13:02:57.000000 sarcharts-0.2.3/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 13:03:03.500344 sarcharts-0.2.3/sarcharts/
+-rw-r--r--   0 runner    (1001) docker     (127)     4373 2024-05-18 13:02:57.000000 sarcharts-0.2.3/sarcharts/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 13:03:03.504344 sarcharts-0.2.3/sarcharts/bin/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-18 13:02:57.000000 sarcharts-0.2.3/sarcharts/bin/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      204 2024-05-18 13:02:57.000000 sarcharts-0.2.3/sarcharts/bin/sarcharts.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 13:03:03.500344 sarcharts-0.2.3/sarcharts/html/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 13:03:03.504344 sarcharts-0.2.3/sarcharts/html/css/
+-rw-r--r--   0 runner    (1001) docker     (127)     2173 2024-05-18 13:02:57.000000 sarcharts-0.2.3/sarcharts/html/css/sarcharts.css
+-rw-r--r--   0 runner    (1001) docker     (127)     2171 2024-05-18 13:02:57.000000 sarcharts-0.2.3/sarcharts/html/css/ul-select.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 13:03:03.504344 sarcharts-0.2.3/sarcharts/html/img/
+-rw-r--r--   0 runner    (1001) docker     (127)      158 2024-05-18 13:02:57.000000 sarcharts-0.2.3/sarcharts/html/img/chevron.svg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 13:03:03.504344 sarcharts-0.2.3/sarcharts/html/js/
+-rw-r--r--   0 runner    (1001) docker     (127)   205214 2024-05-18 13:02:57.000000 sarcharts-0.2.3/sarcharts/html/js/chart.umd.js
+-rw-r--r--   0 runner    (1001) docker     (127)    50650 2024-05-18 13:02:57.000000 sarcharts-0.2.3/sarcharts/html/js/chartjs-adapter-date-fns.bundle.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)    34500 2024-05-18 13:02:57.000000 sarcharts-0.2.3/sarcharts/html/js/chartjs-plugin-annotation.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)    12854 2024-05-18 13:02:57.000000 sarcharts-0.2.3/sarcharts/html/js/chartjs-plugin-zoom.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)    20765 2024-05-18 13:02:57.000000 sarcharts-0.2.3/sarcharts/html/js/hammer.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)   271751 2024-05-18 13:02:57.000000 sarcharts-0.2.3/sarcharts/html/js/jquery.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1343 2024-05-18 13:02:57.000000 sarcharts-0.2.3/sarcharts/html/js/ul-select.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 13:03:03.508344 sarcharts-0.2.3/sarcharts/lib/
+-rw-r--r--   0 runner    (1001) docker     (127)     2413 2024-05-18 13:02:57.000000 sarcharts-0.2.3/sarcharts/lib/chartjs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      766 2024-05-18 13:02:57.000000 sarcharts-0.2.3/sarcharts/lib/events.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1789 2024-05-18 13:02:57.000000 sarcharts-0.2.3/sarcharts/lib/progressbar.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10660 2024-05-18 13:02:57.000000 sarcharts-0.2.3/sarcharts/lib/sadf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2541 2024-05-18 13:02:57.000000 sarcharts-0.2.3/sarcharts/lib/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 13:03:03.508344 sarcharts-0.2.3/sarcharts/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)     5588 2024-05-18 13:02:57.000000 sarcharts-0.2.3/sarcharts/templates/chart.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1162 2024-05-18 13:02:57.000000 sarcharts-0.2.3/sarcharts/templates/header.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 13:03:03.508344 sarcharts-0.2.3/sarcharts.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2230 2024-05-18 13:03:03.000000 sarcharts-0.2.3/sarcharts.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-05-18 13:03:03.000000 sarcharts-0.2.3/sarcharts.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-18 13:03:03.000000 sarcharts-0.2.3/sarcharts.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-18 13:03:03.000000 sarcharts-0.2.3/sarcharts.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-18 13:03:03.000000 sarcharts-0.2.3/sarcharts.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-18 13:03:03.000000 sarcharts-0.2.3/sarcharts.egg-info/pbr.json
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-18 13:03:03.000000 sarcharts-0.2.3/sarcharts.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-18 13:03:03.000000 sarcharts-0.2.3/sarcharts.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      828 2024-05-18 13:03:03.508344 sarcharts-0.2.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      917 2024-05-18 13:02:57.000000 sarcharts-0.2.3/setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)      246 2024-05-18 13:02:57.000000 sarcharts-0.2.3/test-requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      787 2024-05-18 13:02:57.000000 sarcharts-0.2.3/tox.ini
```

### Comparing `sarcharts-0.2.2/.github/workflows/python-publish.yml` & `sarcharts-0.2.3/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `sarcharts-0.2.2/.pylintrc` & `sarcharts-0.2.3/.pylintrc`

 * *Files identical despite different names*

### Comparing `sarcharts-0.2.2/LICENSE` & `sarcharts-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `sarcharts-0.2.2/README.md` & `sarcharts-0.2.3/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -5,30 +5,33 @@
 `sadf` command is needed to read sar files. Hence [sysstat](https://sysstat.github.io/) package is required.
 
 ### Installation
 `pip install sarcharts`
 
 ### Usage
 ~~~
-usage: sarcharts.py [-h] [-d {D,I,W,E}] [-f FROMDATE] [-o OUTPUTPATH] [-t TODATE] [sarfilespaths ...]
+usage: sarcharts [-h] [-d {D,I,W,E}] [-e EVENTFILE] [-f FROMDATE] [-o OUTPUTPATH] [-t TODATE] [-q] [sarfilespaths ...]
 
 SarCharts gets "sysstat" files from provided `sarfilespaths` and generates dynamic HTML Charts.
 
 positional arguments:
   sarfilespaths         `sa` file/s to parse. Default: `./sa??`.
 
-options:
+optional arguments:
   -h, --help            show this help message and exit
   -d {D,I,W,E}, --debug {D,I,W,E}
                         Set debug level. Default `W`.
+  -e EVENTFILE, --eventfile EVENTFILE
+                        Add events csv file. Header: # date;hostname;event_name;event_description
   -f FROMDATE, --fromdate FROMDATE
-                        Read metric starting on this date.
+                        Include metrics from this date.
   -o OUTPUTPATH, --outputpath OUTPUTPATH
                         Path to put output files. Default `./sarcharts`.
   -t TODATE, --todate TODATE
                         Discard metrics after this date.
+  -q, --quiet           Don't show progress.
 ~~~
 
 | Example Chart |
 | --- |
 | ![](/doc/sarcharts.png) |
```

### Comparing `sarcharts-0.2.2/doc/README.md` & `sarcharts-0.2.3/doc/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -5,30 +5,33 @@
 `sadf` command is needed to read sar files. Hence [sysstat](https://sysstat.github.io/) package is required.
 
 ### Installation
 `pip install sarcharts`
 
 ### Usage
 ~~~
-usage: sarcharts.py [-h] [-d {D,I,W,E}] [-f FROMDATE] [-o OUTPUTPATH] [-t TODATE] [sarfilespaths ...]
+usage: sarcharts [-h] [-d {D,I,W,E}] [-e EVENTFILE] [-f FROMDATE] [-o OUTPUTPATH] [-t TODATE] [-q] [sarfilespaths ...]
 
 SarCharts gets "sysstat" files from provided `sarfilespaths` and generates dynamic HTML Charts.
 
 positional arguments:
   sarfilespaths         `sa` file/s to parse. Default: `./sa??`.
 
-options:
+optional arguments:
   -h, --help            show this help message and exit
   -d {D,I,W,E}, --debug {D,I,W,E}
                         Set debug level. Default `W`.
+  -e EVENTFILE, --eventfile EVENTFILE
+                        Add events csv file. Header: # date;hostname;event_name;event_description
   -f FROMDATE, --fromdate FROMDATE
-                        Read metric starting on this date.
+                        Include metrics from this date.
   -o OUTPUTPATH, --outputpath OUTPUTPATH
                         Path to put output files. Default `./sarcharts`.
   -t TODATE, --todate TODATE
                         Discard metrics after this date.
+  -q, --quiet           Don't show progress.
 ~~~
 
 | Example Chart |
 | --- |
 | ![](/doc/sarcharts.png) |
```

### Comparing `sarcharts-0.2.2/doc/sarcharts.png` & `sarcharts-0.2.3/doc/sarcharts.png`

 * *Files identical despite different names*

### Comparing `sarcharts-0.2.2/sarcharts/__init__.py` & `sarcharts-0.2.3/sarcharts/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 
 import argparse
 import fnmatch
 import shutil
 import webbrowser
 
 from sarcharts.lib.chartjs import ChartJS
+from sarcharts.lib.events import Events
 from sarcharts.lib.sadf import Sadf
 from sarcharts.lib import util
 
 
 class SarCharts:
     args = ()
     cwd = os.getcwd()
@@ -53,14 +54,21 @@
             '-d',
             '--debug',
             help='Set debug level. Default `W`.',
             default='W',
             choices=['D', 'I', 'W', 'E']
             )
         self.parser.add_argument(
+            '-e',
+            '--eventfile',
+            help='Add events csv file. Header: '
+                 + '# date;hostname;event_name;event_description',
+            type=self.valid_path
+            )
+        self.parser.add_argument(
             '-f',
             '--fromdate',
             help='Include metrics from this date.',
             default=datetime.datetime.strptime('1970-01-01', '%Y-%m-%d'),
             type=self.valid_date
             )
         self.parser.add_argument(
@@ -105,14 +113,15 @@
 
     def main(self):
         if len(self.args.sarfilespaths) > 0:
             sarfiles = util.get_filelist(self.args.sarfilespaths)
             if len(sarfiles) > 0:
                 util.debug(self.args, 'D', "sarfiles: " + str(sarfiles))
                 charts = Sadf().sar_to_chartjs(self.args, sarfiles)
+                charts = Events.getCSVdata(self.args, charts)
                 ChartJS().write_files(self.args, charts)
                 util.debug(self.args, '', "Open SarCharts in default browser.")
                 webbrowser.open(self.args.outputpath, 0, True)
             else:
                 self.parser.print_help()
                 util.debug(
                     self.args, 'E',
```

### Comparing `sarcharts-0.2.2/sarcharts/html/css/sarcharts.css` & `sarcharts-0.2.3/sarcharts/html/css/sarcharts.css`

 * *Files 9% similar despite different names*

```diff
@@ -56,15 +56,26 @@
     display: inline;
     padding: 0.3em;
     border: 1px solid #ccc;    
     border-radius: 5px;
     margin-bottom: 5px;
     margin-left: 0.2em;
   }
-
+  #popup {
+    display: none;
+    position: absolute;
+    min-width: 80%;
+    max-width: 80%;
+    margin: 0.7em;
+    padding: 0.3em;
+    background: #eee;
+    border: solid 1px #000;
+    border-radius: 5px;
+    margin-bottom: 5px;
+  }
   a:link, a:visited,  a:active {
     color: #5685bc;
     text-decoration: none;
   }
   a:hover {
     color:rgba(255, 0, 0, 0.650);
     text-decoration: none;
```

### Comparing `sarcharts-0.2.2/sarcharts/html/css/ul-select.css` & `sarcharts-0.2.3/sarcharts/html/css/ul-select.css`

 * *Files identical despite different names*

### Comparing `sarcharts-0.2.2/sarcharts/html/js/chart.umd.js` & `sarcharts-0.2.3/sarcharts/html/js/chart.umd.js`

 * *Files identical despite different names*

### Comparing `sarcharts-0.2.2/sarcharts/html/js/chartjs-adapter-date-fns.bundle.min.js` & `sarcharts-0.2.3/sarcharts/html/js/chartjs-adapter-date-fns.bundle.min.js`

 * *Files identical despite different names*

### Comparing `sarcharts-0.2.2/sarcharts/html/js/chartjs-plugin-annotation.min.js` & `sarcharts-0.2.3/sarcharts/html/js/chartjs-plugin-annotation.min.js`

 * *Files identical despite different names*

### Comparing `sarcharts-0.2.2/sarcharts/html/js/chartjs-plugin-zoom.min.js` & `sarcharts-0.2.3/sarcharts/html/js/chartjs-plugin-zoom.min.js`

 * *Files identical despite different names*

### Comparing `sarcharts-0.2.2/sarcharts/html/js/hammer.min.js` & `sarcharts-0.2.3/sarcharts/html/js/hammer.min.js`

 * *Files identical despite different names*

### Comparing `sarcharts-0.2.2/sarcharts/html/js/jquery.js` & `sarcharts-0.2.3/sarcharts/html/js/jquery.js`

 * *Files identical despite different names*

### Comparing `sarcharts-0.2.2/sarcharts/html/js/ul-select.js` & `sarcharts-0.2.3/sarcharts/html/js/ul-select.js`

 * *Files identical despite different names*

### Comparing `sarcharts-0.2.2/sarcharts/lib/chartjs.py` & `sarcharts-0.2.3/sarcharts/lib/chartjs.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,15 +45,15 @@
                     "xlabels": sorted(nodecharts['xlabels']),
                     "sysname": nodecharts['sysname'],
                     "release": nodecharts['release'],
                     "machine": nodecharts['machine'],
                     "numberofcpus": nodecharts['number-of-cpus'],
                     "timezone": nodecharts['timezone'],
                     "details": csvdata,
-                    "restarts": nodecharts['restarts'],
+                    "events": nodecharts['events'],
                     "pages": sorted(nodecharts['activities'].keys()),
                     "colors": self.colors,
                     "hostname": nodename,
                     "hostnames": charts.keys()
                     }
                 parent = (
                     os.path.dirname(
```

### Comparing `sarcharts-0.2.2/sarcharts/lib/progressbar.py` & `sarcharts-0.2.3/sarcharts/lib/progressbar.py`

 * *Files identical despite different names*

### Comparing `sarcharts-0.2.2/sarcharts/lib/sadf.py` & `sarcharts-0.2.3/sarcharts/lib/sadf.py`

 * *Files 4% similar despite different names*

```diff
@@ -60,22 +60,25 @@
                         "sysname": hdata['sysname'],
                         "release": hdata['release'],
                         "machine": hdata['machine'],
                         "number-of-cpus": hdata['number-of-cpus'],
                         "timezone": hdata['timezone'],
                         "xlabels": [],
                         "activities": {},
-                        "restarts": []
+                        "events": {'Restart': []}
                         }
                 for istats in range(len(hdata['restarts'])):
                     for r in hdata['restarts'][istats].values():
                         date = f"{r['date']} {r['time']}"
                         if util.in_date_range(args, date):
-                            charts[nodename]['restarts'].append(date)
                             charts[nodename]['xlabels'].append(date)
+                            charts[nodename]['events']['Restart'].append(
+                                {'date': date,
+                                 'text': f'Restarted at {date}'
+                                 })
                 for istats in range(len(hdata['statistics'])):
                     for act, adata in hdata['statistics'][istats].items():
                         pbi += 1
                         pb.print_bar(pbi, f"data {act}.")
                         if act == "timestamp":
                             date = f"{adata['date']} {adata['time']}"
                             if (date not in charts[nodename]['xlabels']
@@ -95,61 +98,58 @@
                                 for d in adata:
                                     line = linedet
                                     for v in d.values():
                                         line += f";{str(v)}"
                                     charts[nodename]['activities'][act][
                                         'content'].append(line.split(";"))
                             elif isinstance(adata, dict):
-                                d = adata[list(adata.keys())[0]]
-                                if isinstance(d, float) or isinstance(d, int):
-                                    if (act not in charts[nodename][
-                                            'activities'].keys()):
-                                        line = linehead
-                                        for h in adata.keys():
-                                            line += f";{str(h)}"
-                                        charts[nodename]['activities'][act] = {
-                                            "content": [line.split(";")],
-                                            "multiple": False
-                                            }
-                                    line = linedet
-                                    for v in adata.values():
-                                        line += f";{str(v)}"
-                                    charts[nodename]['activities'][act][
-                                        'content'].append(line.split(";"))
-                                else:
-                                    for subact, subdata in adata.items():
-                                        nact = f"{act}_{subact}"
-                                        if isinstance(subdata, list):
-                                            if (nact not in charts[nodename][
-                                                    'activities'].keys()):
-                                                line = linehead
-                                                for h in subdata[0].keys():
-                                                    line += f";{str(h)}"
-                                                charts[nodename]['activities'][nact] = {
-                                                    "content": [line.split(";")],
-                                                    "multiple": True
-                                                    }
-                                            for sv in subdata:
-                                                line = linedet
-                                                for v in sv.values():
-                                                    line += f";{str(v)}"
-                                                charts[nodename]['activities'][nact]['content'].append(line.split(";"))                                        
-                                        else:
-                                            if nact not in charts[nodename]['activities'].keys():
-                                                line = linehead
-                                                for h in subdata.keys():
-                                                    line += f";{str(h)}"
-                                                charts[nodename]['activities'][nact] = {
-                                                    "content": [line.split(";")],
-                                                    "multiple": False
-                                                    }
+                                for subact, subdata in adata.items():
+                                    nact = f"{act}_{subact}"
+                                    if isinstance(subdata, float) or isinstance(subdata, int):
+                                        if (act not in charts[nodename][
+                                                'activities'].keys()):
+                                            line = linehead
+                                            for h in adata.keys():
+                                                line += f";{str(h)}"
+                                            charts[nodename]['activities'][act] = {
+                                                "content": [line.split(";")],
+                                                "multiple": False
+                                                }
+                                        line = linedet
+                                        line += f";{str(subdata)}"
+                                        charts[nodename]['activities'][act][
+                                            'content'].append(line.split(";"))
+                                    elif isinstance(subdata, list):
+                                        if (nact not in charts[nodename][
+                                                'activities'].keys()):
+                                            line = linehead
+                                            for h in subdata[0].keys():
+                                                line += f";{str(h)}"
+                                            charts[nodename]['activities'][nact] = {
+                                                "content": [line.split(";")],
+                                                "multiple": True
+                                                }
+                                        for sv in subdata:
                                             line = linedet
-                                            for v in subdata.values():
+                                            for v in sv.values():
                                                 line += f";{str(v)}"
                                             charts[nodename]['activities'][nact]['content'].append(line.split(";"))                                        
+                                    else:
+                                        if nact not in charts[nodename]['activities'].keys():
+                                            line = linehead
+                                            for h in subdata.keys():
+                                                line += f";{str(h)}"
+                                            charts[nodename]['activities'][nact] = {
+                                                "content": [line.split(";")],
+                                                "multiple": False
+                                                }
+                                        line = linedet
+                                        for v in subdata.values():
+                                            line += f";{str(v)}"
+                                        charts[nodename]['activities'][nact]['content'].append(line.split(";"))                                        
 
         pb.finish("  Get data.")
         # write csv files
         for nodename, nodecharts in charts.items():
             for activity, csvdata in charts[nodename]['activities'].items():
                 with open(f"{args.outputpath}/sar/{nodename}_{activity}.csv", "w") as f:
                     f.write(";".join(csvdata['content'][0]) + "\n")
@@ -182,13 +182,14 @@
                         if item not in charts[nodename]['activities'][activity]['datasets'].keys():
                             charts[nodename]['activities'][activity]['datasets'][item] = []
                             for h in headers:
                                 charts[nodename]['activities'][activity]['datasets'][item].append({
                                     "label": h,
                                     "values": []
                                     })
+                        
                         for f in range(len(fields[datastart:])):
                             charts[nodename]['activities'][activity]['datasets'][item][f]['values'].append({
                                     'x': fields[2],
                                     'y': fields[f+datastart]
                                     })
         return charts
```

### Comparing `sarcharts-0.2.2/sarcharts/lib/util.py` & `sarcharts-0.2.3/sarcharts/lib/util.py`

 * *Files 17% similar despite different names*

```diff
@@ -66,19 +66,30 @@
         details[mtime] = f
     # 'sorted' returns a 'set' hence no duplicates
     # but it should be converted to a list
     return list(dict(sorted(details.items())).values())
 
 
 def valid_date(args, d):
-    format = "%Y-%m-%d %H:%M:%S"
-    try:
-        return datetime.datetime.strptime(d, format)
-    except ValueError:
-        debug(args, 'E', f"ERROR: date '{d}' doesn't match {format}.")
+    outformat = "%Y-%m-%d %H:%M:%S"
+    # put sar 'sar' default format as first helps performance
+    valid = ["%Y-%m-%d %H:%M:%S",
+             "%Y-%m-%dT%H:%M:%S%z",
+             "%Y-%m-%dT%H:%M:%S",
+             "%Y-%m-%d %H",
+             "%Y-%m-%d %H:%M",
+             "%Y-%m-%d"
+             ]
+    for v in valid:
+        try:
+            o = datetime.datetime.strptime(d, v)
+            return datetime.datetime.strptime(str(o), outformat)
+        except ValueError:
+            pass
+    debug(args, 'E', f"not a valid date: {d!r}. Valid formats: {str(valid)}")
 
 
 def in_date_range(args, d):
     d = valid_date(args, d)
     if d >= args.fromdate and d <= args.todate:
         return True
     else:
```

### Comparing `sarcharts-0.2.2/sarcharts/templates/chart.html` & `sarcharts-0.2.3/sarcharts/templates/chart.html`

 * *Files 24% similar despite different names*

```diff
@@ -24,57 +24,63 @@
     {% if item != "" %}
       <li class="i_inactive"><a href='#'>{{ item }}</a></li>
     {% endif %}
   {% endfor %}
     </ul>
   </div>
 </section>
+<div id="popup"></div>
     <div class="chart">
       <canvas id="chartcanvas"></canvas>
     </div>
 <script>
 $('.i_inactive').click(function() {
   $(".i_active").attr("class","i_inactive");
   $(this).attr("class","i_active");
   showChart($(this).text());
 });
-
-
-{% for i in range(restarts|length) %}
-const restart{{ i }} = {
-  type: 'line',
-  enter: function({element}) {
-    element.label.options.color = 'rgba(255, 0, 0)',
-    element.label.options.font.size = 13;
-    element.label.options.content = 'restarted at {{ restarts[i] }}';
-    return true;
-  },
-  leave: function({element}) {
-    element.label.options.color = 'rgba(255, 0, 0, 0.4)',
-    element.label.options.font.size = 10;
-    element.label.options.content = 'restarted';
-    return true;
-  },
-  borderColor: 'rgba(255, 0, 0, 0.4)',
-  borderWidth: 1,
-  display: (ctx) => ctx.chart.isDatasetVisible(1),
-  label: {
-    display: true,
-    position: 'start',
-    content: 'restart',
-    backgroundColor: 'transparent',
-    opacity: 0,
-    rotation: 90,
-    xAdjust: 5,
-    font: { size: 10 },
-    color: 'rgba(255, 0, 0, 0.4)'
-  },
-  scaleID: 'x',
-  value: '{{ restarts[i] }}'
-};
+{% for c in range(events|length) %}
+  {% set event = (events.keys()|list)[c] %}
+  {% for i in range(events[event]|length) %}
+  {% set eventdata = events[event][i] %}
+  const event{{ c }}_{{ i }} = {
+    type: 'line',
+    enter: function({element}) {
+      element.label.options.color = "rgba({{ colors[c] }})",
+      element.label.options.content = ["{{ event }}", "{{ eventdata['date'] }}"];
+      return true;
+    },
+    leave: function({element}) {
+      element.label.options.color = "rgba({{ colors[c] }}, 0.4)",
+      element.label.options.content = "{{ event }}";
+      return true;
+    },
+    click: function({element}) {
+      $("#popup").show();
+      $("#popup").text("{{ eventdata['text'] }}");
+    },
+    borderColor: "rgba({{ colors[c] }}, 0.4)",
+    borderWidth: 1,
+    display: (ctx) => ctx.chart.isDatasetVisible(1),
+    label: {
+      display: true,
+      position: 'start',
+      content: "{{ event }}",
+      backgroundColor: 'transparent',
+      opacity: 0,
+      rotation: 90,
+      xAdjust: 5,
+      yAdjust: 15,
+      font: { size: 11 },
+      color: 'rgba({{ colors[c] }}, 0.4)'
+    },
+    scaleID: 'x',
+    value: "{{ eventdata['date'] }}"
+  };
+  {% endfor %}
 {% endfor %}
 
 function showChart(name) {
   myChart.destroy();
   myChart = new Chart(ctx, {
     type: 'line',
       data: {
@@ -100,28 +106,27 @@
               'quarter': 'yyyy LL:dd HH:mm:ss',
               'year': 'yyyy:LL:dd HH:mm:ss'
             }
           }
         },
         y: {
           title: {
-            display: true,
+            display: false,
             text: 'value'
           }
         }
       },
       plugins: {
         legend: {
           position: 'top'
         },
-        annotation: {
-          annotations: {
-            {% for i in range(restarts|length) %}
-              restart{{ i }}{{ ", " if not loop.last else "" }}
-            {% endfor %}
+        annotation: { annotations: { 
+          {% for c in range(events|length) %}
+            {% set event = (events.keys()|list)[c] %}{% for i in range(events[event]|length) %}event{{c}}_{{i}},{% endfor %}
+          {% endfor %}
           }
         },
         zoom: {
           limits: {
             x: { min:'original', max:'original' }
           },
           zoom: {
@@ -141,15 +146,14 @@
     }
   });
 }
 
 var myCharts = {
   {% for item, data in details['datasets'].items() %}
   '{{ item }}': {
-    // 'labels': {{ xlabels }},
     'datasets': [
     {% for i in range(data|length) %}
       {
       {{ "hidden: true," if data[i]['label'] in details['hidden'] else "" }}
       label: '{{ data[i]['label'] }}',
       data: {{ data[i]['values'] }},
       borderColor: 'rgb({{ colors[i] }} 0.3)',
@@ -159,15 +163,16 @@
     ]
   }{{ ", " if not loop.last else "" }}
   {% endfor %}
 }
 
 var ctx = document.getElementById('chartcanvas').getContext('2d');
 var myChart = new Chart(ctx);
-
+var mousex = 0;
+var mousey = 0;
 $(document).ready(function () {
   showChart($('.i_inactive').first().text());
   $('.i_inactive').first().attr("class", "i_active");
 
   selhost="{{ hostname }}"
   $('#hostlist').ulSelect(function(elem) {
     if (selhost != $(elem).text()) {
@@ -176,13 +181,17 @@
     }
   });
   selchart="{{ chart }}"
   $('#chartlist').ulSelect(function(elem) {
       selchart=$(elem).text().replace(/\s+/g, "");
       window.location = selhost+"_"+selchart+".html"
   });
-
+  $("body").on("click",function(e) {
+    if (!$(e.target).closest('#popup').length) {
+        $('#popup').hide();
+    }
+  });
 });
 
 </script>
 </body>
 </html>
```

### Comparing `sarcharts-0.2.2/sarcharts/templates/header.html` & `sarcharts-0.2.3/sarcharts/templates/header.html`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,12 @@
     <div class="info">
         <ul>
             <li><b>Start:</b> {{ xlabels[0] }} {{ timezone }}</li>
             <li><b>End:</b> {{ xlabels[-1] }} {{ timezone }}</li>
-            <li><b>Hostname:</b> {{ sysname }}</li>
+            <li><b>Sysname:</b> {{ sysname }}</li>
             <li><b>Release:</b> {{ release }}</li>
             <li><b>Architecture:</b> {{ machine}}</li>
             <li><b>CPU:</b> {{ numberofcpus }}</li>
         </ul><!--
         {% for r in restarts %}
             <br> {{r}}
         {% endfor %}
```

### Comparing `sarcharts-0.2.2/sarcharts.egg-info/SOURCES.txt` & `sarcharts-0.2.3/sarcharts.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -29,12 +29,13 @@
 sarcharts/html/js/chartjs-adapter-date-fns.bundle.min.js
 sarcharts/html/js/chartjs-plugin-annotation.min.js
 sarcharts/html/js/chartjs-plugin-zoom.min.js
 sarcharts/html/js/hammer.min.js
 sarcharts/html/js/jquery.js
 sarcharts/html/js/ul-select.js
 sarcharts/lib/chartjs.py
+sarcharts/lib/events.py
 sarcharts/lib/progressbar.py
 sarcharts/lib/sadf.py
 sarcharts/lib/util.py
 sarcharts/templates/chart.html
 sarcharts/templates/header.html
```

### Comparing `sarcharts-0.2.2/setup.cfg` & `sarcharts-0.2.3/setup.cfg`

 * *Files identical despite different names*

### Comparing `sarcharts-0.2.2/setup.py` & `sarcharts-0.2.3/setup.py`

 * *Files identical despite different names*

### Comparing `sarcharts-0.2.2/tox.ini` & `sarcharts-0.2.3/tox.ini`

 * *Files identical despite different names*

