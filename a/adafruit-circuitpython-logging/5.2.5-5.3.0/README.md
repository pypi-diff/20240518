# Comparing `tmp/adafruit-circuitpython-logging-5.2.5.tar.gz` & `tmp/adafruit_circuitpython_logging-5.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adafruit-circuitpython-logging-5.2.5.tar", last modified: Sat Dec  9 17:45:19 2023, max compression
+gzip compressed data, was "adafruit_circuitpython_logging-5.3.0.tar", last modified: Sat May 18 16:07:49 2024, max compression
```

## Comparing `adafruit-circuitpython-logging-5.2.5.tar` & `adafruit_circuitpython_logging-5.3.0.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-09 17:45:19.227008 adafruit-circuitpython-logging-5.2.5/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-09 17:45:19.219008 adafruit-circuitpython-logging-5.2.5/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-09 17:45:19.223008 adafruit-circuitpython-logging-5.2.5/.github/PULL_REQUEST_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)      880 2023-12-09 17:45:05.000000 adafruit-circuitpython-logging-5.2.5/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-09 17:45:19.223008 adafruit-circuitpython-logging-5.2.5/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      303 2023-12-09 17:45:05.000000 adafruit-circuitpython-logging-5.2.5/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (127)      479 2023-12-09 17:45:05.000000 adafruit-circuitpython-logging-5.2.5/.github/workflows/failure-help-text.yml
--rw-r--r--   0 runner    (1001) docker     (127)      482 2023-12-09 17:45:05.000000 adafruit-circuitpython-logging-5.2.5/.github/workflows/release_gh.yml
--rw-r--r--   0 runner    (1001) docker     (127)      475 2023-12-09 17:45:05.000000 adafruit-circuitpython-logging-5.2.5/.github/workflows/release_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1654 2023-12-09 17:45:05.000000 adafruit-circuitpython-logging-5.2.5/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1238 2023-12-09 17:45:05.000000 adafruit-circuitpython-logging-5.2.5/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    13078 2023-12-09 17:45:05.000000 adafruit-circuitpython-logging-5.2.5/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (127)      388 2023-12-09 17:45:05.000000 adafruit-circuitpython-logging-5.2.5/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     6147 2023-12-09 17:45:05.000000 adafruit-circuitpython-logging-5.2.5/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (127)     1102 2023-12-09 17:45:05.000000 adafruit-circuitpython-logging-5.2.5/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-09 17:45:19.223008 adafruit-circuitpython-logging-5.2.5/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (127)    16814 2023-12-09 17:45:05.000000 adafruit-circuitpython-logging-5.2.5/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1108 2023-12-09 17:45:05.000000 adafruit-circuitpython-logging-5.2.5/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1211 2023-12-09 17:45:05.000000 adafruit-circuitpython-logging-5.2.5/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2742 2023-12-09 17:45:19.227008 adafruit-circuitpython-logging-5.2.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1952 2023-12-09 17:45:05.000000 adafruit-circuitpython-logging-5.2.5/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)      108 2023-12-09 17:45:05.000000 adafruit-circuitpython-logging-5.2.5/README.rst.license
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-09 17:45:19.227008 adafruit-circuitpython-logging-5.2.5/adafruit_circuitpython_logging.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2742 2023-12-09 17:45:19.000000 adafruit-circuitpython-logging-5.2.5/adafruit_circuitpython_logging.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1029 2023-12-09 17:45:19.000000 adafruit-circuitpython-logging-5.2.5/adafruit_circuitpython_logging.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-09 17:45:19.000000 adafruit-circuitpython-logging-5.2.5/adafruit_circuitpython_logging.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       46 2023-12-09 17:45:19.000000 adafruit-circuitpython-logging-5.2.5/adafruit_circuitpython_logging.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2023-12-09 17:45:19.000000 adafruit-circuitpython-logging-5.2.5/adafruit_circuitpython_logging.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)    12262 2023-12-09 17:45:12.000000 adafruit-circuitpython-logging-5.2.5/adafruit_logging.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-09 17:45:19.227008 adafruit-circuitpython-logging-5.2.5/docs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-09 17:45:19.227008 adafruit-circuitpython-logging-5.2.5/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (127)     4414 2023-12-09 17:45:05.000000 adafruit-circuitpython-logging-5.2.5/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (127)      105 2023-12-09 17:45:05.000000 adafruit-circuitpython-logging-5.2.5/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (127)      266 2023-12-09 17:45:05.000000 adafruit-circuitpython-logging-5.2.5/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (127)       96 2023-12-09 17:45:05.000000 adafruit-circuitpython-logging-5.2.5/docs/api.rst.license
--rw-r--r--   0 runner    (1001) docker     (127)     5390 2023-12-09 17:45:05.000000 adafruit-circuitpython-logging-5.2.5/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)      188 2023-12-09 17:45:05.000000 adafruit-circuitpython-logging-5.2.5/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (127)       96 2023-12-09 17:45:05.000000 adafruit-circuitpython-logging-5.2.5/docs/examples.rst.license
--rw-r--r--   0 runner    (1001) docker     (127)      971 2023-12-09 17:45:05.000000 adafruit-circuitpython-logging-5.2.5/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)       96 2023-12-09 17:45:05.000000 adafruit-circuitpython-logging-5.2.5/docs/index.rst.license
--rw-r--r--   0 runner    (1001) docker     (127)      154 2023-12-09 17:45:05.000000 adafruit-circuitpython-logging-5.2.5/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-09 17:45:19.227008 adafruit-circuitpython-logging-5.2.5/examples/
--rw-r--r--   0 runner    (1001) docker     (127)      934 2023-12-09 17:45:12.000000 adafruit-circuitpython-logging-5.2.5/examples/logging_filehandler.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2449 2023-12-09 17:45:12.000000 adafruit-circuitpython-logging-5.2.5/examples/logging_mqtt_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     1210 2023-12-09 17:45:12.000000 adafruit-circuitpython-logging-5.2.5/examples/logging_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (127)      108 2023-12-09 17:45:05.000000 adafruit-circuitpython-logging-5.2.5/optional_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1173 2023-12-09 17:45:12.000000 adafruit-circuitpython-logging-5.2.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      143 2023-12-09 17:45:05.000000 adafruit-circuitpython-logging-5.2.5/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-09 17:45:19.227008 adafruit-circuitpython-logging-5.2.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 16:07:49.455763 adafruit_circuitpython_logging-5.3.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 16:07:49.447763 adafruit_circuitpython_logging-5.3.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 16:07:49.451763 adafruit_circuitpython_logging-5.3.0/.github/PULL_REQUEST_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      880 2024-05-18 16:07:40.000000 adafruit_circuitpython_logging-5.3.0/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 16:07:49.451763 adafruit_circuitpython_logging-5.3.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      303 2024-05-18 16:07:40.000000 adafruit_circuitpython_logging-5.3.0/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      479 2024-05-18 16:07:40.000000 adafruit_circuitpython_logging-5.3.0/.github/workflows/failure-help-text.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      482 2024-05-18 16:07:40.000000 adafruit_circuitpython_logging-5.3.0/.github/workflows/release_gh.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      475 2024-05-18 16:07:40.000000 adafruit_circuitpython_logging-5.3.0/.github/workflows/release_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1654 2024-05-18 16:07:40.000000 adafruit_circuitpython_logging-5.3.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1238 2024-05-18 16:07:40.000000 adafruit_circuitpython_logging-5.3.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    13078 2024-05-18 16:07:40.000000 adafruit_circuitpython_logging-5.3.0/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (127)      388 2024-05-18 16:07:40.000000 adafruit_circuitpython_logging-5.3.0/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     6147 2024-05-18 16:07:40.000000 adafruit_circuitpython_logging-5.3.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-05-18 16:07:40.000000 adafruit_circuitpython_logging-5.3.0/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 16:07:49.451763 adafruit_circuitpython_logging-5.3.0/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (127)    16814 2024-05-18 16:07:40.000000 adafruit_circuitpython_logging-5.3.0/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1108 2024-05-18 16:07:40.000000 adafruit_circuitpython_logging-5.3.0/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-05-18 16:07:40.000000 adafruit_circuitpython_logging-5.3.0/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2742 2024-05-18 16:07:49.455763 adafruit_circuitpython_logging-5.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1952 2024-05-18 16:07:40.000000 adafruit_circuitpython_logging-5.3.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-05-18 16:07:40.000000 adafruit_circuitpython_logging-5.3.0/README.rst.license
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 16:07:49.455763 adafruit_circuitpython_logging-5.3.0/adafruit_circuitpython_logging.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2742 2024-05-18 16:07:49.000000 adafruit_circuitpython_logging-5.3.0/adafruit_circuitpython_logging.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1029 2024-05-18 16:07:49.000000 adafruit_circuitpython_logging-5.3.0/adafruit_circuitpython_logging.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-18 16:07:49.000000 adafruit_circuitpython_logging-5.3.0/adafruit_circuitpython_logging.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-18 16:07:49.000000 adafruit_circuitpython_logging-5.3.0/adafruit_circuitpython_logging.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-18 16:07:49.000000 adafruit_circuitpython_logging-5.3.0/adafruit_circuitpython_logging.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    16622 2024-05-18 16:07:47.000000 adafruit_circuitpython_logging-5.3.0/adafruit_logging.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 16:07:49.451763 adafruit_circuitpython_logging-5.3.0/docs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 16:07:49.455763 adafruit_circuitpython_logging-5.3.0/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)     4414 2024-05-18 16:07:40.000000 adafruit_circuitpython_logging-5.3.0/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-05-18 16:07:40.000000 adafruit_circuitpython_logging-5.3.0/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (127)      266 2024-05-18 16:07:40.000000 adafruit_circuitpython_logging-5.3.0/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-05-18 16:07:40.000000 adafruit_circuitpython_logging-5.3.0/docs/api.rst.license
+-rw-r--r--   0 runner    (1001) docker     (127)     5390 2024-05-18 16:07:40.000000 adafruit_circuitpython_logging-5.3.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      188 2024-05-18 16:07:40.000000 adafruit_circuitpython_logging-5.3.0/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-05-18 16:07:40.000000 adafruit_circuitpython_logging-5.3.0/docs/examples.rst.license
+-rw-r--r--   0 runner    (1001) docker     (127)      971 2024-05-18 16:07:40.000000 adafruit_circuitpython_logging-5.3.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-05-18 16:07:40.000000 adafruit_circuitpython_logging-5.3.0/docs/index.rst.license
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-05-18 16:07:40.000000 adafruit_circuitpython_logging-5.3.0/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 16:07:49.455763 adafruit_circuitpython_logging-5.3.0/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)      934 2024-05-18 16:07:47.000000 adafruit_circuitpython_logging-5.3.0/examples/logging_filehandler.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2449 2024-05-18 16:07:47.000000 adafruit_circuitpython_logging-5.3.0/examples/logging_mqtt_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1210 2024-05-18 16:07:47.000000 adafruit_circuitpython_logging-5.3.0/examples/logging_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-05-18 16:07:40.000000 adafruit_circuitpython_logging-5.3.0/optional_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1173 2024-05-18 16:07:47.000000 adafruit_circuitpython_logging-5.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      143 2024-05-18 16:07:40.000000 adafruit_circuitpython_logging-5.3.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-18 16:07:49.455763 adafruit_circuitpython_logging-5.3.0/setup.cfg
```

### Comparing `adafruit-circuitpython-logging-5.2.5/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md` & `adafruit_circuitpython_logging-5.3.0/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-logging-5.2.5/.gitignore` & `adafruit_circuitpython_logging-5.3.0/.gitignore`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-logging-5.2.5/.pre-commit-config.yaml` & `adafruit_circuitpython_logging-5.3.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-logging-5.2.5/.pylintrc` & `adafruit_circuitpython_logging-5.3.0/.pylintrc`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-logging-5.2.5/CODE_OF_CONDUCT.md` & `adafruit_circuitpython_logging-5.3.0/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-logging-5.2.5/LICENSE` & `adafruit_circuitpython_logging-5.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-logging-5.2.5/LICENSES/CC-BY-4.0.txt` & `adafruit_circuitpython_logging-5.3.0/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-logging-5.2.5/LICENSES/MIT.txt` & `adafruit_circuitpython_logging-5.3.0/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-logging-5.2.5/LICENSES/Unlicense.txt` & `adafruit_circuitpython_logging-5.3.0/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-logging-5.2.5/PKG-INFO` & `adafruit_circuitpython_logging-5.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-logging
-Version: 5.2.5
+Version: 5.3.0
 Summary: Logging module for CircuitPython
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_Logging
 Keywords: adafruit,blinka,circuitpython,micropython,logging,logger
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-logging-5.2.5/README.rst` & `adafruit_circuitpython_logging-5.3.0/README.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-logging-5.2.5/adafruit_circuitpython_logging.egg-info/PKG-INFO` & `adafruit_circuitpython_logging-5.3.0/adafruit_circuitpython_logging.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-logging
-Version: 5.2.5
+Version: 5.3.0
 Summary: Logging module for CircuitPython
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_Logging
 Keywords: adafruit,blinka,circuitpython,micropython,logging,logger
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-logging-5.2.5/adafruit_circuitpython_logging.egg-info/SOURCES.txt` & `adafruit_circuitpython_logging-5.3.0/adafruit_circuitpython_logging.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-logging-5.2.5/adafruit_logging.py` & `adafruit_circuitpython_logging-5.3.0/adafruit_logging.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 # SPDX-FileCopyrightText: 2019 Dave Astels for Adafruit Industries
+# SPDX-FileCopyrightText: 2024 Pat Satyshur
 #
 # SPDX-License-Identifier: MIT
 
 """
 `adafruit_logging`
 ==================
 
@@ -54,17 +55,19 @@
 
 """
 
 # pylint: disable=invalid-name,undefined-variable
 
 import time
 import sys
+import os
 from collections import namedtuple
 
 try:
+    # pylint: disable=deprecated-class
     from typing import Optional, Hashable
     from typing_extensions import Protocol
 
     class WriteableStream(Protocol):
         """Any stream that can ``write`` strings"""
 
         def write(self, buf: str) -> int:
@@ -72,15 +75,15 @@
 
             :param str buf: The string data to write to the stream
             """
 
 except ImportError:
     pass
 
-__version__ = "5.2.5"
+__version__ = "5.3.0"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_Logger.git"
 
 # pylint:disable=undefined-all-variable
 __all__ = [
     "LEVELS",
     "NOTSET",
     "DEBUG",
@@ -210,14 +213,16 @@
 
     :param str filename: The filename of the log file
     :param str mode: Whether to write ('w') or append ('a'); default is to append
     """
 
     def __init__(self, filename: str, mode: str = "a") -> None:
         # pylint: disable=consider-using-with
+        if mode == "r":
+            raise ValueError("Can't write to a read only file")
         super().__init__(open(filename, mode=mode))
 
     def close(self) -> None:
         """Closes the file"""
         self.stream.flush()
         self.stream.close()
 
@@ -225,21 +230,120 @@
         """Generate a string to log
 
         :param record: The record (message object) to be logged
         """
         return super().format(record) + "\r\n"
 
     def emit(self, record: LogRecord) -> None:
-        """Generate the message and write it to the UART.
+        """Generate the message and write it to the file.
 
         :param record: The record (message object) to be logged
         """
         self.stream.write(self.format(record))
 
 
+class RotatingFileHandler(FileHandler):
+    """File handler for writing log files to flash memory or external memory such as an SD card.
+    This handler implements a very simple log rotating system similar to the python function of the
+    same name (https://docs.python.org/3/library/logging.handlers.html#rotatingfilehandler)
+
+    If maxBytes is set, the handler will check to see if the log file is larger than the given
+    limit. If the log file is larger than the limit, it is renamed and a new file is started.
+    The old log file will be renamed with a numerical appendix '.1', '.2', etc... The variable
+    backupCount controls how many old log files to keep. For example, if the filename is 'log.txt'
+    and backupCount is 5, you will end up with six log files: 'log.txt', 'log.txt.1', 'log.txt.3',
+    up to 'log.txt.5' Therefore, the maximum amount of disk space the logs can use is
+    maxBytes*(backupCount+1).
+
+    If either maxBytes or backupCount is not set, or set to zero, the log rotation is disabled.
+    This will result in a single log file with a name `filename` that will grow without bound.
+
+    :param str filename: The filename of the log file
+    :param str mode: Whether to write ('w') or append ('a'); default is to append
+    :param int maxBytes: The max allowable size of the log file in bytes.
+    :param int backupCount: The number of old log files to keep.
+    """
+
+    def __init__(
+        self,
+        filename: str,
+        mode: str = "a",
+        maxBytes: int = 0,
+        backupCount: int = 0,
+    ) -> None:
+        if maxBytes < 0:
+            raise ValueError("maxBytes must be a positive number")
+        if backupCount < 0:
+            raise ValueError("backupCount must be a positive number")
+
+        self._LogFileName = filename
+        self._WriteMode = mode
+        self._maxBytes = maxBytes
+        self._backupCount = backupCount
+
+        # Open the file and save the handle to self.stream
+        super().__init__(self._LogFileName, mode=self._WriteMode)
+
+    def doRollover(self) -> None:
+        """Roll over the log files. This should not need to be called directly"""
+        # At this point, we have already determined that we need to roll the log files.
+        # Close the log file. Probably needed if we want to delete/rename files.
+        self.close()
+
+        for i in range(self._backupCount, 0, -1):
+            CurrentFileName = self._LogFileName + "." + str(i)
+            CurrentFileNamePlus = self._LogFileName + "." + str(i + 1)
+            try:
+                if i == self._backupCount:
+                    # This is the oldest log file. Delete this one.
+                    os.remove(CurrentFileName)
+                else:
+                    # Rename the current file to the next number in the sequence.
+                    os.rename(CurrentFileName, CurrentFileNamePlus)
+            except OSError as e:
+                if e.args[0] == 2:
+                    # File does not exsist. This is okay.
+                    pass
+                else:
+                    raise e
+
+        # Rename the current log to the first backup
+        os.rename(self._LogFileName, CurrentFileName)
+
+        # Reopen the file.
+        # pylint: disable=consider-using-with
+        self.stream = open(self._LogFileName, mode=self._WriteMode)
+
+    def GetLogSize(self) -> int:
+        """Check the size of the log file."""
+        try:
+            self.stream.flush()  # We need to call this or the file size is always zero.
+            LogFileSize = os.stat(self._LogFileName)[6]
+        except OSError as e:
+            if e.args[0] == 2:
+                # Log file does not exsist. This is okay.
+                LogFileSize = None
+            else:
+                raise e
+        return LogFileSize
+
+    def emit(self, record: LogRecord) -> None:
+        """Generate the message and write it to the file.
+
+        :param record: The record (message object) to be logged
+        """
+        if (
+            (self.GetLogSize() >= self._maxBytes)
+            and (self._maxBytes > 0)
+            and (self._backupCount > 0)
+        ):
+            self.doRollover()
+        self.stream.write(self.format(record))
+
+
 class NullHandler(Handler):
     """Provide an empty log handler.
 
     This can be used in place of a real log handler to more efficiently disable
     logging.
     """
```

### Comparing `adafruit-circuitpython-logging-5.2.5/docs/_static/favicon.ico` & `adafruit_circuitpython_logging-5.3.0/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-logging-5.2.5/docs/conf.py` & `adafruit_circuitpython_logging-5.3.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-logging-5.2.5/docs/index.rst` & `adafruit_circuitpython_logging-5.3.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-logging-5.2.5/examples/logging_filehandler.py` & `adafruit_circuitpython_logging-5.3.0/examples/logging_filehandler.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-logging-5.2.5/examples/logging_mqtt_handler.py` & `adafruit_circuitpython_logging-5.3.0/examples/logging_mqtt_handler.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-logging-5.2.5/examples/logging_simpletest.py` & `adafruit_circuitpython_logging-5.3.0/examples/logging_simpletest.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-logging-5.2.5/pyproject.toml` & `adafruit_circuitpython_logging-5.3.0/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     "wheel",
     "setuptools-scm",
 ]
 
 [project]
 name = "adafruit-circuitpython-logging"
 description = "Logging module for CircuitPython"
-version = "5.2.5"
+version = "5.3.0"
 readme = "README.rst"
 authors = [
     {name = "Adafruit Industries", email = "circuitpython@adafruit.com"}
 ]
 urls = {Homepage = "https://github.com/adafruit/Adafruit_CircuitPython_Logging"}
 keywords = [
     "adafruit",
```

