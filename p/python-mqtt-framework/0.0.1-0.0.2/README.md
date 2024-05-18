# Comparing `tmp/python_mqtt_framework-0.0.1.tar.gz` & `tmp/python_mqtt_framework-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_mqtt_framework-0.0.1.tar", last modified: Sat May 18 19:42:57 2024, max compression
+gzip compressed data, was "python_mqtt_framework-0.0.2.tar", last modified: Sat May 18 20:00:26 2024, max compression
```

## Comparing `python_mqtt_framework-0.0.1.tar` & `python_mqtt_framework-0.0.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 19:42:57.333080 python_mqtt_framework-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-18 19:42:48.000000 python_mqtt_framework-0.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3556 2024-05-18 19:42:57.333080 python_mqtt_framework-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2132 2024-05-18 19:42:48.000000 python_mqtt_framework-0.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 19:42:57.333080 python_mqtt_framework-0.0.1/mqtt_framework/
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-18 19:42:48.000000 python_mqtt_framework-0.0.1/mqtt_framework/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2866 2024-05-18 19:42:48.000000 python_mqtt_framework-0.0.1/mqtt_framework/_topic_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     4238 2024-05-18 19:42:48.000000 python_mqtt_framework-0.0.1/mqtt_framework/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     1483 2024-05-18 19:42:48.000000 python_mqtt_framework-0.0.1/mqtt_framework/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 19:42:57.333080 python_mqtt_framework-0.0.1/python_mqtt_framework.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3556 2024-05-18 19:42:57.000000 python_mqtt_framework-0.0.1/python_mqtt_framework.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      387 2024-05-18 19:42:57.000000 python_mqtt_framework-0.0.1/python_mqtt_framework.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-18 19:42:57.000000 python_mqtt_framework-0.0.1/python_mqtt_framework.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      131 2024-05-18 19:42:57.000000 python_mqtt_framework-0.0.1/python_mqtt_framework.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-18 19:42:57.000000 python_mqtt_framework-0.0.1/python_mqtt_framework.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      109 2024-05-18 19:42:48.000000 python_mqtt_framework-0.0.1/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-18 19:42:57.333080 python_mqtt_framework-0.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1566 2024-05-18 19:42:48.000000 python_mqtt_framework-0.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 20:00:26.221308 python_mqtt_framework-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-18 20:00:15.000000 python_mqtt_framework-0.0.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3785 2024-05-18 20:00:26.221308 python_mqtt_framework-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2287 2024-05-18 20:00:15.000000 python_mqtt_framework-0.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 20:00:26.217307 python_mqtt_framework-0.0.2/mqtt_framework/
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-18 20:00:15.000000 python_mqtt_framework-0.0.2/mqtt_framework/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2866 2024-05-18 20:00:15.000000 python_mqtt_framework-0.0.2/mqtt_framework/_topic_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4238 2024-05-18 20:00:15.000000 python_mqtt_framework-0.0.2/mqtt_framework/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1483 2024-05-18 20:00:15.000000 python_mqtt_framework-0.0.2/mqtt_framework/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 20:00:26.221308 python_mqtt_framework-0.0.2/python_mqtt_framework.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3785 2024-05-18 20:00:26.000000 python_mqtt_framework-0.0.2/python_mqtt_framework.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      387 2024-05-18 20:00:26.000000 python_mqtt_framework-0.0.2/python_mqtt_framework.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-18 20:00:26.000000 python_mqtt_framework-0.0.2/python_mqtt_framework.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      131 2024-05-18 20:00:26.000000 python_mqtt_framework-0.0.2/python_mqtt_framework.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-18 20:00:26.000000 python_mqtt_framework-0.0.2/python_mqtt_framework.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      109 2024-05-18 20:00:15.000000 python_mqtt_framework-0.0.2/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-18 20:00:26.221308 python_mqtt_framework-0.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1630 2024-05-18 20:00:15.000000 python_mqtt_framework-0.0.2/setup.py
```

### Comparing `python_mqtt_framework-0.0.1/PKG-INFO` & `python_mqtt_framework-0.0.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 Metadata-Version: 2.1
 Name: python-mqtt-framework
-Version: 0.0.1
+Version: 0.0.2
+Summary: An opinionated framework to handle MQTT communication in Python.
 Home-page: https://github.com/jourdanrodrigues/python-mqtt-framework
 Author: Jourdan Rodrigues
 Author-email: thiagojourdan@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -29,23 +30,23 @@
 Requires-Dist: pydantic>=2.7.1; extra == "dev"
 Requires-Dist: pylibmc>=1.6.3; extra == "dev"
 Requires-Dist: tox>=4.15.0; extra == "dev"
 Requires-Dist: coverage>=7.5.1; extra == "dev"
 
 # Python MQTT framework
 
-**An MQTT listener and a friendly MQTT client.**
-
+![PyPI - Version](https://img.shields.io/pypi/v/python-mqtt-framework)
+![PyPI - Python Version](https://img.shields.io/pypi/pyversions/python-mqtt-framework)
 [![codecov](https://codecov.io/github/jourdanrodrigues/python-mqtt-framework/graph/badge.svg?token=L3VL6QCO77)](https://codecov.io/github/jourdanrodrigues/python-mqtt-framework)
 
 ---
 
 # Overview
 
-MQTT framework is a library that provides a simple MQTT listener and a solid client. It is built on top of the [paho-mqtt](https://pypi.org/project/paho-mqtt/) library.
+MQTT framework is a library that provides an opinionated structure for setting up message handlers and publishers for MQTT brokers. It is built on top of the [paho-mqtt](https://pypi.org/project/paho-mqtt/) library.
 
 ----
 
 # Requirements
 
 * Python 3.8+
```

### Comparing `python_mqtt_framework-0.0.1/README.md` & `python_mqtt_framework-0.0.2/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 # Python MQTT framework
 
-**An MQTT listener and a friendly MQTT client.**
-
+![PyPI - Version](https://img.shields.io/pypi/v/python-mqtt-framework)
+![PyPI - Python Version](https://img.shields.io/pypi/pyversions/python-mqtt-framework)
 [![codecov](https://codecov.io/github/jourdanrodrigues/python-mqtt-framework/graph/badge.svg?token=L3VL6QCO77)](https://codecov.io/github/jourdanrodrigues/python-mqtt-framework)
 
 ---
 
 # Overview
 
-MQTT framework is a library that provides a simple MQTT listener and a solid client. It is built on top of the [paho-mqtt](https://pypi.org/project/paho-mqtt/) library.
+MQTT framework is a library that provides an opinionated structure for setting up message handlers and publishers for MQTT brokers. It is built on top of the [paho-mqtt](https://pypi.org/project/paho-mqtt/) library.
 
 ----
 
 # Requirements
 
 * Python 3.8+
```

### Comparing `python_mqtt_framework-0.0.1/mqtt_framework/_topic_handler.py` & `python_mqtt_framework-0.0.2/mqtt_framework/_topic_handler.py`

 * *Files identical despite different names*

### Comparing `python_mqtt_framework-0.0.1/mqtt_framework/client.py` & `python_mqtt_framework-0.0.2/mqtt_framework/client.py`

 * *Files identical despite different names*

### Comparing `python_mqtt_framework-0.0.1/mqtt_framework/settings.py` & `python_mqtt_framework-0.0.2/mqtt_framework/settings.py`

 * *Files identical despite different names*

### Comparing `python_mqtt_framework-0.0.1/python_mqtt_framework.egg-info/PKG-INFO` & `python_mqtt_framework-0.0.2/python_mqtt_framework.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 Metadata-Version: 2.1
 Name: python-mqtt-framework
-Version: 0.0.1
+Version: 0.0.2
+Summary: An opinionated framework to handle MQTT communication in Python.
 Home-page: https://github.com/jourdanrodrigues/python-mqtt-framework
 Author: Jourdan Rodrigues
 Author-email: thiagojourdan@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -29,23 +30,23 @@
 Requires-Dist: pydantic>=2.7.1; extra == "dev"
 Requires-Dist: pylibmc>=1.6.3; extra == "dev"
 Requires-Dist: tox>=4.15.0; extra == "dev"
 Requires-Dist: coverage>=7.5.1; extra == "dev"
 
 # Python MQTT framework
 
-**An MQTT listener and a friendly MQTT client.**
-
+![PyPI - Version](https://img.shields.io/pypi/v/python-mqtt-framework)
+![PyPI - Python Version](https://img.shields.io/pypi/pyversions/python-mqtt-framework)
 [![codecov](https://codecov.io/github/jourdanrodrigues/python-mqtt-framework/graph/badge.svg?token=L3VL6QCO77)](https://codecov.io/github/jourdanrodrigues/python-mqtt-framework)
 
 ---
 
 # Overview
 
-MQTT framework is a library that provides a simple MQTT listener and a solid client. It is built on top of the [paho-mqtt](https://pypi.org/project/paho-mqtt/) library.
+MQTT framework is a library that provides an opinionated structure for setting up message handlers and publishers for MQTT brokers. It is built on top of the [paho-mqtt](https://pypi.org/project/paho-mqtt/) library.
 
 ----
 
 # Requirements
 
 * Python 3.8+
```

### Comparing `python_mqtt_framework-0.0.1/setup.py` & `python_mqtt_framework-0.0.2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,16 +4,16 @@
     dev_dependencies = requirements_file.read().strip().split("\n")
 
 with open("README.md") as readme_file:
     readme = readme_file.read()
 
 setup(
     name="python-mqtt-framework",
-    version="0.0.1",
-    description="",
+    version="0.0.2",
+    description="An opinionated framework to handle MQTT communication in Python.",
     long_description=readme,
     long_description_content_type="text/markdown",
     author="Jourdan Rodrigues",
     author_email="thiagojourdan@gmail.com",
     classifiers=[
         "Development Status :: 3 - Alpha",
         "Environment :: Web Environment",
```

