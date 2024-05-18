# Comparing `tmp/rest_solace-0.0.2.tar.gz` & `tmp/rest_solace-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rest_solace-0.0.2.tar", last modified: Fri May 10 14:18:07 2024, max compression
+gzip compressed data, was "rest_solace-0.1.0.tar", last modified: Sat May 18 13:21:01 2024, max compression
```

## Comparing `rest_solace-0.0.2.tar` & `rest_solace-0.1.0.tar`

### file list

```diff
@@ -1,46 +1,49 @@
-drwxr-xr-x   0 skyler    (1000) skyler    (1000)        0 2024-05-10 14:18:07.051106 rest_solace-0.0.2/
--rw-r--r--   0 skyler    (1000) skyler    (1000)       29 2024-05-07 12:19:34.000000 rest_solace-0.0.2/.gitignore
--rw-r--r--   0 skyler    (1000) skyler    (1000)    10178 2024-05-07 08:54:03.000000 rest_solace-0.0.2/LICENSE.txt
--rw-r--r--   0 skyler    (1000) skyler    (1000)     1260 2024-05-07 11:22:11.000000 rest_solace-0.0.2/NOTICE.txt
--rw-r--r--   0 skyler    (1000) skyler    (1000)     6617 2024-05-10 14:18:07.051106 rest_solace-0.0.2/PKG-INFO
--rw-r--r--   0 skyler    (1000) skyler    (1000)     5540 2024-05-10 14:11:26.000000 rest_solace-0.0.2/README.rst
-drwxr-xr-x   0 skyler    (1000) skyler    (1000)        0 2024-05-10 14:18:07.039106 rest_solace-0.0.2/docs/
--rw-r--r--   0 skyler    (1000) skyler    (1000)      579 2024-05-10 11:24:36.000000 rest_solace-0.0.2/docs/development_refrences.rst
--rw-r--r--   0 skyler    (1000) skyler    (1000)     1826 2024-05-10 14:17:37.000000 rest_solace-0.0.2/pyproject.toml
--rw-r--r--   0 skyler    (1000) skyler    (1000)       38 2024-05-10 14:18:07.051106 rest_solace-0.0.2/setup.cfg
-drwxr-xr-x   0 skyler    (1000) skyler    (1000)        0 2024-05-10 14:18:07.035106 rest_solace-0.0.2/src/
-drwxr-xr-x   0 skyler    (1000) skyler    (1000)        0 2024-05-10 14:18:07.039106 rest_solace-0.0.2/src/rest_solace/
--rw-r--r--   0 skyler    (1000) skyler    (1000)      520 2024-04-20 20:43:31.000000 rest_solace-0.0.2/src/rest_solace/__init__.py
-drwxr-xr-x   0 skyler    (1000) skyler    (1000)        0 2024-05-10 14:18:07.047106 rest_solace-0.0.2/src/rest_solace/__pycache__/
--rw-r--r--   0 skyler    (1000) skyler    (1000)      359 2024-04-20 20:55:30.000000 rest_solace-0.0.2/src/rest_solace/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0 skyler    (1000) skyler    (1000)     2040 2024-04-07 08:23:01.000000 rest_solace-0.0.2/src/rest_solace/__pycache__/action.cpython-311.pyc
--rw-r--r--   0 skyler    (1000) skyler    (1000)     2224 2024-04-07 06:29:02.000000 rest_solace-0.0.2/src/rest_solace/__pycache__/config.cpython-311.pyc
--rw-r--r--   0 skyler    (1000) skyler    (1000)     5734 2024-04-21 05:54:01.000000 rest_solace-0.0.2/src/rest_solace/__pycache__/consumer.cpython-311.pyc
--rw-r--r--   0 skyler    (1000) skyler    (1000)     4876 2024-04-22 07:47:41.000000 rest_solace-0.0.2/src/rest_solace/__pycache__/http_client.cpython-311.pyc
--rw-r--r--   0 skyler    (1000) skyler    (1000)     4128 2024-04-07 19:18:05.000000 rest_solace-0.0.2/src/rest_solace/__pycache__/manage.cpython-311.pyc
--rw-r--r--   0 skyler    (1000) skyler    (1000)    20533 2024-04-22 10:02:53.000000 rest_solace-0.0.2/src/rest_solace/__pycache__/manager.cpython-311.pyc
--rw-r--r--   0 skyler    (1000) skyler    (1000)     1227 2024-03-31 13:04:04.000000 rest_solace-0.0.2/src/rest_solace/__pycache__/pub_sub.cpython-311.pyc
--rw-r--r--   0 skyler    (1000) skyler    (1000)     2742 2024-04-07 20:21:55.000000 rest_solace-0.0.2/src/rest_solace/__pycache__/publish.cpython-311.pyc
--rw-r--r--   0 skyler    (1000) skyler    (1000)     4538 2024-04-21 19:21:45.000000 rest_solace-0.0.2/src/rest_solace/__pycache__/publisher.cpython-311.pyc
--rw-r--r--   0 skyler    (1000) skyler    (1000)     4246 2024-04-07 18:11:44.000000 rest_solace-0.0.2/src/rest_solace/__pycache__/semp_client.cpython-311.pyc
--rw-r--r--   0 skyler    (1000) skyler    (1000)     7341 2024-03-31 19:33:25.000000 rest_solace-0.0.2/src/rest_solace/__pycache__/semp_endpoint.cpython-311.pyc
--rw-r--r--   0 skyler    (1000) skyler    (1000)     5358 2024-04-20 19:56:40.000000 rest_solace-0.0.2/src/rest_solace/__pycache__/subscriber.cpython-311.pyc
--rw-r--r--   0 skyler    (1000) skyler    (1000)     5149 2024-05-06 18:11:03.000000 rest_solace-0.0.2/src/rest_solace/consumer.py
--rw-r--r--   0 skyler    (1000) skyler    (1000)      125 2024-05-06 18:10:17.000000 rest_solace-0.0.2/src/rest_solace/exceptions.py
--rw-r--r--   0 skyler    (1000) skyler    (1000)     3164 2024-05-05 14:53:10.000000 rest_solace-0.0.2/src/rest_solace/http_client.py
--rw-r--r--   0 skyler    (1000) skyler    (1000)    29947 2024-05-06 18:13:23.000000 rest_solace-0.0.2/src/rest_solace/manager.py
--rw-r--r--   0 skyler    (1000) skyler    (1000)    14199 2024-05-05 18:58:01.000000 rest_solace-0.0.2/src/rest_solace/publisher.py
-drwxr-xr-x   0 skyler    (1000) skyler    (1000)        0 2024-05-10 14:18:07.051106 rest_solace-0.0.2/src/rest_solace.egg-info/
--rw-r--r--   0 skyler    (1000) skyler    (1000)     6617 2024-05-10 14:18:06.000000 rest_solace-0.0.2/src/rest_solace.egg-info/PKG-INFO
--rw-r--r--   0 skyler    (1000) skyler    (1000)     1303 2024-05-10 14:18:07.000000 rest_solace-0.0.2/src/rest_solace.egg-info/SOURCES.txt
--rw-r--r--   0 skyler    (1000) skyler    (1000)        1 2024-05-10 14:18:06.000000 rest_solace-0.0.2/src/rest_solace.egg-info/dependency_links.txt
--rw-r--r--   0 skyler    (1000) skyler    (1000)       82 2024-05-10 14:18:06.000000 rest_solace-0.0.2/src/rest_solace.egg-info/requires.txt
--rw-r--r--   0 skyler    (1000) skyler    (1000)       12 2024-05-10 14:18:06.000000 rest_solace-0.0.2/src/rest_solace.egg-info/top_level.txt
-drwxr-xr-x   0 skyler    (1000) skyler    (1000)        0 2024-05-10 14:18:07.047106 rest_solace-0.0.2/tests/
-drwxr-xr-x   0 skyler    (1000) skyler    (1000)        0 2024-05-10 14:18:07.051106 rest_solace-0.0.2/tests/__pycache__/
--rw-r--r--   0 skyler    (1000) skyler    (1000)     1419 2024-04-21 18:34:05.000000 rest_solace-0.0.2/tests/__pycache__/manager_unittest.cpython-311.pyc
--rw-r--r--   0 skyler    (1000) skyler    (1000)      864 2024-05-06 18:46:43.000000 rest_solace-0.0.2/tests/consumer_test.py
--rw-r--r--   0 skyler    (1000) skyler    (1000)     2102 2024-05-06 18:46:46.000000 rest_solace-0.0.2/tests/empty_test.py
--rw-r--r--   0 skyler    (1000) skyler    (1000)     7223 2024-05-06 18:46:48.000000 rest_solace-0.0.2/tests/manager_test.py
--rw-r--r--   0 skyler    (1000) skyler    (1000)     2841 2024-05-06 18:46:50.000000 rest_solace-0.0.2/tests/pub_sub_test.py
--rw-r--r--   0 skyler    (1000) skyler    (1000)      891 2024-04-28 09:19:07.000000 rest_solace-0.0.2/tests/util.py
+drwxr-xr-x   0 skyler    (1000) skyler    (1000)        0 2024-05-18 13:21:00.997412 rest_solace-0.1.0/
+-rw-r--r--   0 skyler    (1000) skyler    (1000)      132 2024-05-14 15:14:18.000000 rest_solace-0.1.0/.gitignore
+-rw-r--r--   0 skyler    (1000) skyler    (1000)    10178 2024-05-07 08:54:03.000000 rest_solace-0.1.0/LICENSE.txt
+-rw-r--r--   0 skyler    (1000) skyler    (1000)     1260 2024-05-07 11:22:11.000000 rest_solace-0.1.0/NOTICE.txt
+-rw-r--r--   0 skyler    (1000) skyler    (1000)     8300 2024-05-18 13:21:00.997412 rest_solace-0.1.0/PKG-INFO
+-rw-r--r--   0 skyler    (1000) skyler    (1000)     7390 2024-05-14 18:08:22.000000 rest_solace-0.1.0/README.rst
+drwxr-xr-x   0 skyler    (1000) skyler    (1000)        0 2024-05-18 13:21:00.961393 rest_solace-0.1.0/docs/
+-rw-r--r--   0 skyler    (1000) skyler    (1000)      579 2024-05-10 11:24:36.000000 rest_solace-0.1.0/docs/development_refrences.rst
+-rw-r--r--   0 skyler    (1000) skyler    (1000)     1288 2024-05-10 17:40:06.000000 rest_solace-0.1.0/docs/getting_started_with_solace.rst
+-rw-r--r--   0 skyler    (1000) skyler    (1000)      276 2024-05-10 17:58:06.000000 rest_solace-0.1.0/docs/index.rst
+-rw-r--r--   0 skyler    (1000) skyler    (1000)      214 2024-05-14 15:11:52.000000 rest_solace-0.1.0/docs/semp_v2_endpoint_support.rst
+-rw-r--r--   0 skyler    (1000) skyler    (1000)     2136 2024-05-18 13:20:13.000000 rest_solace-0.1.0/pyproject.toml
+-rw-r--r--   0 skyler    (1000) skyler    (1000)       38 2024-05-18 13:21:00.997412 rest_solace-0.1.0/setup.cfg
+drwxr-xr-x   0 skyler    (1000) skyler    (1000)        0 2024-05-18 13:21:00.953388 rest_solace-0.1.0/src/
+drwxr-xr-x   0 skyler    (1000) skyler    (1000)        0 2024-05-18 13:21:00.969397 rest_solace-0.1.0/src/rest_solace/
+-rw-r--r--   0 skyler    (1000) skyler    (1000)      520 2024-04-20 20:43:31.000000 rest_solace-0.1.0/src/rest_solace/__init__.py
+drwxr-xr-x   0 skyler    (1000) skyler    (1000)        0 2024-05-18 13:21:00.981403 rest_solace-0.1.0/src/rest_solace/__pycache__/
+-rw-r--r--   0 skyler    (1000) skyler    (1000)      359 2024-04-20 20:55:30.000000 rest_solace-0.1.0/src/rest_solace/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 skyler    (1000) skyler    (1000)     2040 2024-04-07 08:23:01.000000 rest_solace-0.1.0/src/rest_solace/__pycache__/action.cpython-311.pyc
+-rw-r--r--   0 skyler    (1000) skyler    (1000)     2224 2024-04-07 06:29:02.000000 rest_solace-0.1.0/src/rest_solace/__pycache__/config.cpython-311.pyc
+-rw-r--r--   0 skyler    (1000) skyler    (1000)     5734 2024-04-21 05:54:01.000000 rest_solace-0.1.0/src/rest_solace/__pycache__/consumer.cpython-311.pyc
+-rw-r--r--   0 skyler    (1000) skyler    (1000)     4876 2024-04-22 07:47:41.000000 rest_solace-0.1.0/src/rest_solace/__pycache__/http_client.cpython-311.pyc
+-rw-r--r--   0 skyler    (1000) skyler    (1000)     4128 2024-04-07 19:18:05.000000 rest_solace-0.1.0/src/rest_solace/__pycache__/manage.cpython-311.pyc
+-rw-r--r--   0 skyler    (1000) skyler    (1000)    20533 2024-04-22 10:02:53.000000 rest_solace-0.1.0/src/rest_solace/__pycache__/manager.cpython-311.pyc
+-rw-r--r--   0 skyler    (1000) skyler    (1000)     1227 2024-03-31 13:04:04.000000 rest_solace-0.1.0/src/rest_solace/__pycache__/pub_sub.cpython-311.pyc
+-rw-r--r--   0 skyler    (1000) skyler    (1000)     2742 2024-04-07 20:21:55.000000 rest_solace-0.1.0/src/rest_solace/__pycache__/publish.cpython-311.pyc
+-rw-r--r--   0 skyler    (1000) skyler    (1000)     4538 2024-04-21 19:21:45.000000 rest_solace-0.1.0/src/rest_solace/__pycache__/publisher.cpython-311.pyc
+-rw-r--r--   0 skyler    (1000) skyler    (1000)     4246 2024-04-07 18:11:44.000000 rest_solace-0.1.0/src/rest_solace/__pycache__/semp_client.cpython-311.pyc
+-rw-r--r--   0 skyler    (1000) skyler    (1000)     7341 2024-03-31 19:33:25.000000 rest_solace-0.1.0/src/rest_solace/__pycache__/semp_endpoint.cpython-311.pyc
+-rw-r--r--   0 skyler    (1000) skyler    (1000)     5358 2024-04-20 19:56:40.000000 rest_solace-0.1.0/src/rest_solace/__pycache__/subscriber.cpython-311.pyc
+-rw-r--r--   0 skyler    (1000) skyler    (1000)     5149 2024-05-14 18:23:02.000000 rest_solace-0.1.0/src/rest_solace/consumer.py
+-rw-r--r--   0 skyler    (1000) skyler    (1000)      125 2024-05-06 18:10:17.000000 rest_solace-0.1.0/src/rest_solace/exceptions.py
+-rw-r--r--   0 skyler    (1000) skyler    (1000)     3164 2024-05-05 14:53:10.000000 rest_solace-0.1.0/src/rest_solace/http_client.py
+-rw-r--r--   0 skyler    (1000) skyler    (1000)    31091 2024-05-12 17:11:18.000000 rest_solace-0.1.0/src/rest_solace/manager.py
+-rw-r--r--   0 skyler    (1000) skyler    (1000)    17246 2024-05-18 10:07:32.000000 rest_solace-0.1.0/src/rest_solace/publisher.py
+drwxr-xr-x   0 skyler    (1000) skyler    (1000)        0 2024-05-18 13:21:00.993410 rest_solace-0.1.0/src/rest_solace.egg-info/
+-rw-r--r--   0 skyler    (1000) skyler    (1000)     8300 2024-05-18 13:21:00.000000 rest_solace-0.1.0/src/rest_solace.egg-info/PKG-INFO
+-rw-r--r--   0 skyler    (1000) skyler    (1000)     1389 2024-05-18 13:21:00.000000 rest_solace-0.1.0/src/rest_solace.egg-info/SOURCES.txt
+-rw-r--r--   0 skyler    (1000) skyler    (1000)        1 2024-05-18 13:21:00.000000 rest_solace-0.1.0/src/rest_solace.egg-info/dependency_links.txt
+-rw-r--r--   0 skyler    (1000) skyler    (1000)       17 2024-05-18 13:21:00.000000 rest_solace-0.1.0/src/rest_solace.egg-info/requires.txt
+-rw-r--r--   0 skyler    (1000) skyler    (1000)       12 2024-05-18 13:21:00.000000 rest_solace-0.1.0/src/rest_solace.egg-info/top_level.txt
+drwxr-xr-x   0 skyler    (1000) skyler    (1000)        0 2024-05-18 13:21:00.989408 rest_solace-0.1.0/tests/
+drwxr-xr-x   0 skyler    (1000) skyler    (1000)        0 2024-05-18 13:21:00.989408 rest_solace-0.1.0/tests/__pycache__/
+-rw-r--r--   0 skyler    (1000) skyler    (1000)     1419 2024-04-21 18:34:05.000000 rest_solace-0.1.0/tests/__pycache__/manager_unittest.cpython-311.pyc
+-rw-r--r--   0 skyler    (1000) skyler    (1000)      864 2024-05-06 18:46:43.000000 rest_solace-0.1.0/tests/consumer_test.py
+-rw-r--r--   0 skyler    (1000) skyler    (1000)      654 2024-05-12 08:11:53.000000 rest_solace-0.1.0/tests/empty_test.py
+-rw-r--r--   0 skyler    (1000) skyler    (1000)     6920 2024-05-12 17:08:22.000000 rest_solace-0.1.0/tests/manager_test.py
+-rw-r--r--   0 skyler    (1000) skyler    (1000)     2772 2024-05-14 18:07:29.000000 rest_solace-0.1.0/tests/pub_sub_test.py
+-rw-r--r--   0 skyler    (1000) skyler    (1000)      891 2024-04-28 09:19:07.000000 rest_solace-0.1.0/tests/util.py
```

### Comparing `rest_solace-0.0.2/LICENSE.txt` & `rest_solace-0.1.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `rest_solace-0.0.2/NOTICE.txt` & `rest_solace-0.1.0/NOTICE.txt`

 * *Files identical despite different names*

### Comparing `rest_solace-0.0.2/docs/development_refrences.rst` & `rest_solace-0.1.0/docs/development_refrences.rst`

 * *Files identical despite different names*

### Comparing `rest_solace-0.0.2/src/rest_solace/__init__.py` & `rest_solace-0.1.0/src/rest_solace/__init__.py`

 * *Files identical despite different names*

### Comparing `rest_solace-0.0.2/src/rest_solace/__pycache__/action.cpython-311.pyc` & `rest_solace-0.1.0/src/rest_solace/__pycache__/action.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `rest_solace-0.0.2/src/rest_solace/__pycache__/config.cpython-311.pyc` & `rest_solace-0.1.0/src/rest_solace/__pycache__/config.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `rest_solace-0.0.2/src/rest_solace/__pycache__/consumer.cpython-311.pyc` & `rest_solace-0.1.0/src/rest_solace/__pycache__/consumer.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `rest_solace-0.0.2/src/rest_solace/__pycache__/http_client.cpython-311.pyc` & `rest_solace-0.1.0/src/rest_solace/__pycache__/http_client.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `rest_solace-0.0.2/src/rest_solace/__pycache__/manage.cpython-311.pyc` & `rest_solace-0.1.0/src/rest_solace/__pycache__/manage.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `rest_solace-0.0.2/src/rest_solace/__pycache__/manager.cpython-311.pyc` & `rest_solace-0.1.0/src/rest_solace/__pycache__/manager.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `rest_solace-0.0.2/src/rest_solace/__pycache__/pub_sub.cpython-311.pyc` & `rest_solace-0.1.0/src/rest_solace/__pycache__/pub_sub.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `rest_solace-0.0.2/src/rest_solace/__pycache__/publish.cpython-311.pyc` & `rest_solace-0.1.0/src/rest_solace/__pycache__/publish.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `rest_solace-0.0.2/src/rest_solace/__pycache__/publisher.cpython-311.pyc` & `rest_solace-0.1.0/src/rest_solace/__pycache__/publisher.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `rest_solace-0.0.2/src/rest_solace/__pycache__/semp_client.cpython-311.pyc` & `rest_solace-0.1.0/src/rest_solace/__pycache__/semp_client.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `rest_solace-0.0.2/src/rest_solace/__pycache__/semp_endpoint.cpython-311.pyc` & `rest_solace-0.1.0/src/rest_solace/__pycache__/semp_endpoint.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `rest_solace-0.0.2/src/rest_solace/__pycache__/subscriber.cpython-311.pyc` & `rest_solace-0.1.0/src/rest_solace/__pycache__/subscriber.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `rest_solace-0.0.2/src/rest_solace/consumer.py` & `rest_solace-0.1.0/src/rest_solace/consumer.py`

 * *Files identical despite different names*

### Comparing `rest_solace-0.0.2/src/rest_solace/http_client.py` & `rest_solace-0.1.0/src/rest_solace/http_client.py`

 * *Files identical despite different names*

### Comparing `rest_solace-0.0.2/src/rest_solace/manager.py` & `rest_solace-0.1.0/src/rest_solace/manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,55 +1,55 @@
 from .http_client import HttpClient
 from urllib.parse import urlsplit, urlunsplit
 
 class Manager():
     
     def __init__(self, user_name:str, password:str,
-                 host:str, SEMP_port:str= "8080", verify_ssl=False) -> None:
+                 host:str, semp_port:str= "8080", verify_ssl=False) -> None:
         """Class for creating a Manage object for communicating with a broker regarding management stuff.
 
         Args:
             username (str): Username of user with admin level access to the broker.
             password (str): Password for the username provided.
             host (str): Broker address (IPv4)
             SEMP_port (str): Management port used for management stuff on the broker side using Solace Element Management Protocol v2.
         """
 
         self.http_client = HttpClient(host= host,
-                                      port= SEMP_port,
+                                      port= semp_port,
                                       user_name= user_name,
                                       password= password,
                                       verify_ssl= verify_ssl)
 
 
     #info
     
-    def get_about(self, throw_exception= True)->dict:
+    def get_about_api(self, throw_exception= True)->dict:
+        """This provides metadata about the SEMP API, such as the version of the API supported by the broker.
 
-        endpoint = "/SEMP/v2/config/about"
+        Args:
+            throw_exception (bool, optional): Throw exception incase request error code indicates an error. 
+                                              Defaults to True.
 
-        res = self.http_client.http_get(endpoint= endpoint)
-        
-        if throw_exception:
-            res.raise_for_status()
-        return res.json()
-    
-    def get_about_api(self, throw_exception= True)->dict:
+        Returns:
+            dict: Requested data.
+        """
 
         endpoint = "/SEMP/v2/config/about/api"
 
         res = self.http_client.http_get(endpoint= endpoint)
 
         if throw_exception:
             res.raise_for_status()
         return res.json()
 
 
     #client profile
 
+    
     def fetch_all_client_profiles(self, msgVpnName= "default", select= "*"):
 
 
         endpoint = f"/SEMP/v2/config/msgVpns/{msgVpnName}/clientProfiles?count=1&select={select}"
 
         data= list()
         links= list()
@@ -137,38 +137,54 @@
             res.raise_for_status()
         return res.json()
 
 
 
     # VPNs
 
-    def request_vpn_objects(self, count:int= 10, select= '*',throw_exception= True)->dict:
+    #Finished. Now need to give same options to fetch.
+    def request_vpn_objects(self, count:int= 10, where= None, 
+                            select= '*', opaquePassword= None,
+                            throw_exception= True)->dict:
         """Get list of message VPNs and info regarding them based on specified parameters.
         
         Note: 
             This function directly passes parameters to an endpoint and could require the use of pagination to access all values.
             It is recommended that you use get_all_vpn_objects() function instead which grantees all info, but uses more bandwidth.
 
         For more info: 
-            https://docs.solace.com/Admin/SEMP/SEMP-Features.htm
             https://docs.solace.com/API-Developer-Online-Ref-Documentation/swagger-ui/software-broker/config/index.html#/msgVpn/getMsgVpns
 
         Args:
             count (int): Limits the number of objects in the response. default is 10.
-                         Ideally applications should always be written to handle pagination instead of massive counts.
-            select (str): Select only certain attributes to return. Give value 'msgVpnName,enabled' to see only names and enabled status.
-
-            throw_exception (bool, optional): _description_. Defaults to True.
+                         Ideally your applications should always be written to handle pagination instead of massive counts.
+            where (str): Specify that a response should include only objects that satisfy certain conditions.
+                         Expects comma-separated list of expressions. 
+                         All expressions must be true for the object to be included in the response.
+                         For more info, consult: https://docs.solace.com/Admin/SEMP/SEMP-Features.htm#Filtering
+            select (str): Select only certain attributes to return. 
+                          Expects comma-separated list of attribute names.
+                          Give value 'msgVpnName,enabled' to see only names and enabled status.
+                          For more info, consult: https://docs.solace.com/Admin/SEMP/SEMP-Features.htm#Select
+            opaquePassword (str): Password to retrieve attributes with the opaque property. 
+            throw_exception (bool, optional): Throw exception incase request error code indicates an error. 
+                                              Defaults to True.
 
         Returns:
-            _type_: _description_
+            dict: Requested data.
         """
 
         endpoint = f"/SEMP/v2/config/msgVpns?count={str(count)}&select={select}"
 
+        if where != None:
+            endpoint+="&where={where}"
+
+        if opaquePassword != None:
+            endpoint+="&opaquePassword={opaquePassword}"
+
         res = self.http_client.http_get(endpoint= endpoint)
         
         if throw_exception:
             res.raise_for_status()
         return res.json()
 
     def fetch_all_vpn_objects(self, select= "*")->dict[list, list]:
```

### Comparing `rest_solace-0.0.2/src/rest_solace/publisher.py` & `rest_solace-0.1.0/src/rest_solace/publisher.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,247 +1,314 @@
 from .http_client import HttpClient
 from requests.exceptions import ReadTimeout
 
 class MessagingPublisher():
     
     def __init__(self, user_name:str, password:str,
-                 host:str, REST_VPNport:str, verify_ssl=False) -> None:
+                 host:str, rest_vpn_port:str, verify_ssl=False) -> None:
         """Class for creating a Publisher object for communicating with a broker to publish a message in Messaging mode.
 
         Args:
             username (str): Username of user with admin level access to the broker.
             password (str): Password for the username provided.
             host (str): Broker address (IPv4)
-            REST_VPNport (str): The port assigned on your vpn of interest where you wish to send messages through REST messaging.
+            rest_vpn_port (str): The port assigned on your vpn of interest where you wish to send messages through REST messaging.
                                 We use this port so specify which VPN we wish to send our messages to.
         """
 
         self.http_client = HttpClient(host= host,
-                                      port= REST_VPNport,
+                                      port= rest_vpn_port,
                                       user_name= user_name,
                                       password= password,
                                       verify_ssl= verify_ssl)
         
     def update_parameters(self, user_name:str, password:str,
-                          host:str, REST_VPNport:str, verify_ssl=False):
+                          host:str, rest_vpn_port:str, verify_ssl=False):
         """Update parameters used to connect with the broker.
 
         Args:
             username (str): Username of user with admin level access to the broker.
             password (str): Password for the username provided.
             host (str): Broker address (IPv4)
-            REST_VPNport (str): The port assigned on your vpn of interest where you wish to send messages through REST messaging.
+            rest_vpn_port (str): The port assigned on your vpn of interest where you wish to send messages through REST messaging.
                                 We use this port so specify which VPN we wish to send our messages to.        """
         
         self.http_client = HttpClient(host= host,
-                                      port= REST_VPNport,
+                                      port= rest_vpn_port,
                                       user_name= user_name,
                                       password= password,
                                       verify_ssl= verify_ssl)
 
-    def publishToQueueEndpoint(self, queue_name:str, message:str, delivery_mode:str= "direct", 
-                                reply_to_queue:str|None= None, reply_for_topic:str|None= None, 
-                                time_to_live:int|None= None, DMQ_eligible:bool= False,
-                                timeout:str|None= 120, throw_exception:bool= False)->dict:
+    def direct_message_to_queue(self, queue_name:str, message:str, 
+                             reply_to_queue:str|None= None, reply_for_topic:str|None= None, 
+                             timeout:str|None= 120, throw_exception:bool= False)->dict:
         
-        """Publish a message to a queue endpoint.
+        """Publish a message to a queue endpoint in direct mode.
+        'direct' mode is for sending messages without expecting a reply.
 
         Args:
             queue_name (str): Name of the queue endpoint you wish to publish to.
             message (str): The message you wish to send.
-            delivery_mode (str, optional): Mode of delivery for sending a message. 
-                                           'direct' for sending messages without expecting a reply.
-                                           'persistent' for getting a reply from the consumer to confirm if the message was received.
-                                           Defaults to "direct".
             reply_to_queue (str | None, optional): After the message is received by the consumer, 
                                                    chose which queue the consumer reply will go to if provided.
                                                    The value must be the name of a queue.
-                                                   Only works in 'direct' delivery_mode.
+                                                   Only works in 'direct' delivery mode.
                                                    Defaults to None.
             reply_for_topic (str | None, optional): After the message is received by the consumer, 
                                                     chose which topic string the consumer reply will go to if provided.
                                                     The value must be a topic string (NOT the name of a topic endpoint).
-                                                    Only works in 'direct' delivery_mode.
+                                                    Only works in 'direct' delivery mode.
                                                     Defaults to None.
-            time_to_live (int | None, optional): Lifetime for a guaranteed message (in milliseconds). 
-                                                 If the message is not delivered by this time limit,
-                                                 it is either discarded from the queue or moved to dead message queue if eligible.
-                                                 Only works in 'persistent' delivery_mode.
-                                                 Defaults to None.
-            DMQ_eligible (bool, optional): Set the message as eligible for a Dead Message Queues (DMQ). 
-                                           Only works in 'persistent' delivery_mode.
-                                           Defaults to False.
             timeout (str | None, optional): http/https request timeout set on the client side. Defaults to 120.
             throw_exception (bool, optional): Throw exception incase request error code indicates an error or timeout has been reached.
                                               Defaults to False.
 
         Raises:
             ValueError: Can only select either 'reply_to_queue' or 'reply_for_topic', not both.
-            ValueError: Cannot select 'reply_to_queue' or 'reply_for_topic' options when delivery_mode = 'persistent'
-            ValueError: 'delivery_mode' parameter can only be 'direct' or 'persistent'
             HTTPError: Return code for request indicates an error
 
         Returns:
             dict: Dictionary containing request information and {'timeout':False}.
                   Incase timeout is reached, returned dictionary only contains {'timeout':True}.
         """
 
         endpoint = f"/QUEUE/{queue_name}"
 
-        headers = {'Content-Type': 'text/plain'}
-
-        if delivery_mode == 'direct':
-
-            headers['Solace-Delivery-Mode'] = 'direct'
-
-            if reply_to_queue == None and reply_for_topic == None:
-                pass
-            elif reply_to_queue != None and reply_for_topic != None:
-                raise ValueError("Can only select either 'reply_to_queue' or 'reply_for_topic', not both.")
-            elif reply_to_queue != None:
-                headers['Solace-Reply-To-Destination'] = f"/QUEUE/{reply_to_queue}"
-            else:
-                headers['Solace-Reply-To-Destination'] = f"/TOPIC/{reply_for_topic}"
-
-        elif delivery_mode == 'persistent':
-
-            headers['Solace-Delivery-Mode'] = 'persistent'
-            headers['Solace-Reply-Wait-Time-In-ms'] = "FOREVER" #specifies to broker that reply is expected
-
-            if time_to_live != None:
-                headers['Solace-Time-To-Live-In-ms'] = str(time_to_live) #Time after which the message is removed from queue.
-
-            if DMQ_eligible != None:
-                headers['Solace-DMQ-Eligible'] = 'true' if DMQ_eligible == True else 'false'
+        headers = {'Content-Type': 'text/plain',
+                   'Solace-Delivery-Mode': 'direct'}
 
-            if (reply_to_queue != None) or (reply_for_topic != None):
-                raise ValueError("Cannot select 'reply_to_queue' or 'reply_for_topic' options when delivery_mode = 'persistent'")
-        
+        if reply_to_queue == None and reply_for_topic == None:
+            pass
+        elif reply_to_queue != None and reply_for_topic != None:
+            raise ValueError("Can only select either 'reply_to_queue' or 'reply_for_topic', not both.")
+        elif reply_to_queue != None:
+            headers['Solace-Reply-To-Destination'] = f"/QUEUE/{reply_to_queue}"
         else:
-            raise ValueError("'delivery_mode' parameter can only be 'direct' or 'persistent'")
+            headers['Solace-Reply-To-Destination'] = f"/TOPIC/{reply_for_topic}"
             
         res = None
         try:
             res = self.http_client.http_post(endpoint= endpoint, payload= message, headers= headers, timeout=timeout)
         except ReadTimeout as e:
             if throw_exception == True:
                 raise e
             else:
                 return {'timeout':True} 
         
-
         if res != None:
             if throw_exception:
                 res.raise_for_status()
             return {"status_code":res.status_code, "headers":res.headers, 
                     "content":res.content, 'timeout':False}
-        
-
-    def publishForTopic(self, topic_string:str, message:str, delivery_mode:str= "direct", 
+       
+    def direct_message_for_topic(self, topic_string:str, message:str, 
                         reply_to_queue:str|None= None, reply_for_topic:str|None= None, 
-                        time_to_live:int|None= None, DMQ_eligible:bool= False,
                         timeout:str|None= 120, throw_exception:bool= False)->dict:
 
         """Publish a message for a specific topic. 
+        'direct' mode is for sending messages without expecting a reply.
         A topic is a string that allows for attracting specific messages to specific endpoints.
-        Endpoints subscribe to a specific topic string and messages with matching strings go to those endpoints.
+        Endpoints subscribe to a specific topic string, and messages with matching strings go to those endpoints.
         Learn more at: https://docs.solace.com/Get-Started/what-are-topics.htm   
 
         Note: 
             This is not to be confused with publishing to a topic endpoint.
             Publishing directly to a topic endpoint is not possible anyway,
             and topic endpoints only receive messages through the topic they are subscribed to.
             Also, the topic-string a topic endpoint is subscribed to cannot be configured manually and
             is defined by the subscriber subscribing to the topic endpoint.
             This library does not support subscribing to a topic endpoint.
 
         Args:
-            topic_string (str): A string used to attract published messages. It can contain wildcards to match with multiple sub topic-strings.
+            topic_string (str): A string used by an endpoint to attract published messages. 
+                                It can contain wildcards to match with multiple sub topic-strings.
             message (str): The message you wish to send.
-            delivery_mode (str, optional): Mode of delivery for sending a message. 
-                                           'direct' for sending messages without expecting a reply.
-                                           'persistent' for getting a reply from the consumer to confirm if the message was received.
-                                           Defaults to "direct".
             reply_to_queue (str | None, optional): After the message is received by the consumer, 
                                                    chose which queue the consumer reply will go to if provided.
                                                    The value must be the name of a queue.
-                                                   Only works in 'direct' delivery_mode.
+                                                   Only works in 'direct' delivery mode.
                                                    Defaults to None.
             reply_for_topic (str | None, optional): After the message is received by the consumer, 
                                                     chose which topic string the consumer reply will go to if provided.
                                                     The value must be a topic string (NOT the name of a topic endpoint).
-                                                    Only works in 'direct' delivery_mode.
+                                                    Only works in 'direct' delivery mode.
                                                     Defaults to None.
+            timeout (str | None, optional): http/https request timeout set on the client side. Defaults to 120.
+            throw_exception (bool, optional): Throw exception incase request error code indicates an error or timeout has been reached.
+                                              Defaults to False.
+
+        Raises:
+            ValueError: Can only select either 'reply_to_queue' or 'reply_for_topic', not both.
+            HTTPError: Return code for request indicates an error
+
+        Returns:
+            dict: Dictionary containing request information and {'timeout':False}.
+                  Incase timeout is reached, returned dictionary only contains {'timeout':True}.
+        """
+
+        endpoint = f"/TOPIC/{topic_string}"
+
+        headers = {'Content-Type': 'text/plain',
+                   'Solace-Delivery-Mode': 'direct'}
+
+        if reply_to_queue == None and reply_for_topic == None:
+            pass
+        elif reply_to_queue != None and reply_for_topic != None:
+            raise ValueError("Can only select either 'reply_to_queue' or 'reply_for_topic', not both.")
+        elif reply_to_queue != None:
+            headers['Solace-Reply-To-Destination'] = f"/QUEUE/{reply_to_queue}"
+        else:
+            headers['Solace-Reply-To-Destination'] = f"/TOPIC/{reply_for_topic}"
+            
+        res = None
+        try:
+            res = self.http_client.http_post(endpoint= endpoint, payload= message, headers= headers, timeout=timeout)
+        except ReadTimeout as e:
+            if throw_exception == True:
+                raise e
+            else:
+                return {'timeout':True} 
+        
+        if res != None:
+            if throw_exception:
+                res.raise_for_status()
+            return {"status_code":res.status_code, "headers":res.headers, 
+                    "content":res.content, 'timeout':False}
+       
+    def persistent_message_to_queue(self, queue_name:str, message:str, 
+                                time_to_live:int|None= None, DMQ_eligible:bool= False,
+                                timeout:str|None= 120, throw_exception:bool= False)->dict:
+        
+        """Publish a message to a queue endpoint in persistent mode.
+        'persistent' mode is for getting a reply from the consumer to confirm if the message was received.
+
+        Args:
+            queue_name (str): Name of the queue endpoint you wish to publish to.
+            message (str): The message you wish to send.
             time_to_live (int | None, optional): Lifetime for a guaranteed message (in milliseconds). 
                                                  If the message is not delivered by this time limit,
                                                  it is either discarded from the queue or moved to dead message queue if eligible.
-                                                 Only works in 'persistent' delivery_mode.
+                                                 Only works in 'persistent' delivery mode.
                                                  Defaults to None.
             DMQ_eligible (bool, optional): Set the message as eligible for a Dead Message Queues (DMQ). 
-                                           Only works in 'persistent' delivery_mode.
+                                           Only works in 'persistent' delivery mode.
                                            Defaults to False.
             timeout (str | None, optional): http/https request timeout set on the client side. Defaults to 120.
             throw_exception (bool, optional): Throw exception incase request error code indicates an error or timeout has been reached.
                                               Defaults to False.
 
         Raises:
-            ValueError: Can only select either 'reply_to_queue' or 'reply_for_topic', not both.
-            ValueError: Cannot select 'reply_to_queue' or 'reply_for_topic' options when delivery_mode = 'persistent'
-            ValueError: 'delivery_mode' parameter can only be 'direct' or 'persistent'
             HTTPError: Return code for request indicates an error
 
         Returns:
             dict: Dictionary containing request information and {'timeout':False}.
                   Incase timeout is reached, returned dictionary only contains {'timeout':True}.
         """
 
-        endpoint = f"/TOPIC/{topic_string}"
-
-        headers = {'Content-Type': 'text/plain'}
+        endpoint = f"/QUEUE/{queue_name}"
 
-        if delivery_mode == 'direct':
+        headers = {'Content-Type': 'text/plain',
+                   'Solace-Delivery-Mode': 'persistent',
+                   'Solace-Reply-Wait-Time-In-ms': "FOREVER" #specifies to broker that reply is expected
+                   }
 
-            headers['Solace-Delivery-Mode'] = 'direct'
+        if time_to_live != None:
+            headers['Solace-Time-To-Live-In-ms'] = str(time_to_live) #Time after which the message is removed from queue.
 
-            if reply_to_queue == None and reply_for_topic == None:
-                pass
-            elif reply_to_queue != None and reply_for_topic != None:
-                raise ValueError("Can only select either 'reply_to_queue' or 'reply_for_topic', not both.")
-            elif reply_to_queue != None:
-                headers['Solace-Reply-To-Destination'] = f"/QUEUE/{reply_to_queue}"
+        if DMQ_eligible != None:
+            headers['Solace-DMQ-Eligible'] = 'true' if DMQ_eligible == True else 'false'
+    
+        res = None
+        try:
+            res = self.http_client.http_post(endpoint= endpoint, payload= message, headers= headers, timeout=timeout)
+        except ReadTimeout as e:
+            if throw_exception == True:
+                raise e
             else:
-                headers['Solace-Reply-To-Destination'] = f"/TOPIC/{reply_for_topic}"
+                return {'timeout':True} 
+        
+        if res != None:
+            if throw_exception:
+                res.raise_for_status()
+            return {"status_code":res.status_code, "headers":res.headers, 
+                    "content":res.content, 'timeout':False}
+
+    def persistent_message_for_topic(self, topic_string:str, message:str,
+                        time_to_live:int|None= None, DMQ_eligible:bool= False,
+                        timeout:str|None= 120, throw_exception:bool= False)->dict:
+
+        """Publish a message for a specific topic. 
+        'persistent' mode is for getting a reply from the consumer to confirm if the message was received.
+        A topic is a string that allows for attracting specific messages to specific endpoints.
+        Endpoints subscribe to a specific topic string, and messages with matching strings go to those endpoints.
+        Learn more at: https://docs.solace.com/Get-Started/what-are-topics.htm   
+
+        Note: 
+            This is not to be confused with publishing to a topic endpoint.
+            Publishing directly to a topic endpoint is not possible anyway,
+            and topic endpoints only receive messages through the topic they are subscribed to.
+            Also, the topic-string a topic endpoint is subscribed to cannot be configured manually and
+            is defined by the subscriber subscribing to the topic endpoint.
+            This library does not support subscribing to a topic endpoint.
+
+        Args:
+            topic_string (str): A string used by an endpoint to attract published messages. 
+            It can contain wildcards to match with multiple sub topic-strings.
+            message (str): The message you wish to send.
+            time_to_live (int | None, optional): Lifetime for a guaranteed message (in milliseconds). 
+                                                 If the message is not delivered by this time limit,
+                                                 it is either discarded from the queue or moved to dead message queue if eligible.
+                                                 Only works in 'persistent' delivery mode.
+                                                 Defaults to None.
+            DMQ_eligible (bool, optional): Set the message as eligible for a Dead Message Queues (DMQ). 
+                                           Only works in 'persistent' delivery mode.
+                                           Defaults to False.
+            timeout (str | None, optional): http/https request timeout set on the client side. Defaults to 120.
+            throw_exception (bool, optional): Throw exception incase request error code indicates an error or timeout has been reached.
+                                              Defaults to False.
+
+        Raises:
+            HTTPError: Return code for request indicates an error
 
-        elif delivery_mode == 'persistent':
+        Returns:
+            dict: Dictionary containing request information and {'timeout':False}.
+                  Incase timeout is reached, returned dictionary only contains {'timeout':True}.
+        """
 
-            headers['Solace-Delivery-Mode'] = 'persistent'
-            headers['Solace-Reply-Wait-Time-In-ms'] = "FOREVER" #specifies to broker that reply is expected
+        endpoint = f"/TOPIC/{topic_string}"
 
-            if time_to_live != None:
-                headers['Solace-Time-To-Live-In-ms'] = str(time_to_live) #Time after which the message is removed from queue.
+        headers = {'Content-Type': 'text/plain',
+                   'Solace-Delivery-Mode': 'persistent',
+                   'Solace-Reply-Wait-Time-In-ms': "FOREVER" #specifies to broker that reply is expected
+                   }
 
-            if DMQ_eligible != None:
-                headers['Solace-DMQ-Eligible'] = 'true' if DMQ_eligible == True else 'false'
+        if time_to_live != None:
+            headers['Solace-Time-To-Live-In-ms'] = str(time_to_live) #Time after which the message is removed from queue.
 
-            if (reply_to_queue != None) or (reply_for_topic != None):
-                raise ValueError("Cannot select 'reply_to_queue' or 'reply_for_topic' options when delivery_mode = 'persistent'")
-        
-        else:
-            raise ValueError("'delivery_mode' parameter can only be 'direct' or 'persistent'")
-            
+        if DMQ_eligible != None:
+            headers['Solace-DMQ-Eligible'] = 'true' if DMQ_eligible == True else 'false'
+    
         res = None
         try:
             res = self.http_client.http_post(endpoint= endpoint, payload= message, headers= headers, timeout=timeout)
         except ReadTimeout as e:
             if throw_exception == True:
                 raise e
             else:
                 return {'timeout':True} 
         
-
         if res != None:
             if throw_exception:
                 res.raise_for_status()
             return {"status_code":res.status_code, "headers":res.headers, 
                     "content":res.content, 'timeout':False}
 
+    #Async functions of the above 4 functions. (you will have to remake each one and with aiohttp)
+    
+
+    #A single sync function to send many messages based on parameters from list of dictionary (That you could import from a CSV)
+    #Should have flag to turn on and off async
+    #https://www.geeksforgeeks.org/load-csv-data-into-list-and-dictionary-using-python/
+
 
+#Add a class to validate inputs for the different functions.
+#this would validate input for all functions. Also makes it so you can validate all the input for the multi message function first.
```

### Comparing `rest_solace-0.0.2/src/rest_solace.egg-info/SOURCES.txt` & `rest_solace-0.1.0/src/rest_solace.egg-info/SOURCES.txt`

 * *Files 19% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 .gitignore
 LICENSE.txt
 NOTICE.txt
 README.rst
 pyproject.toml
 docs/development_refrences.rst
+docs/getting_started_with_solace.rst
+docs/index.rst
+docs/semp_v2_endpoint_support.rst
 src/rest_solace/__init__.py
 src/rest_solace/consumer.py
 src/rest_solace/exceptions.py
 src/rest_solace/http_client.py
 src/rest_solace/manager.py
 src/rest_solace/publisher.py
 src/rest_solace.egg-info/PKG-INFO
```

### Comparing `rest_solace-0.0.2/tests/__pycache__/manager_unittest.cpython-311.pyc` & `rest_solace-0.1.0/tests/__pycache__/manager_unittest.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `rest_solace-0.0.2/tests/consumer_test.py` & `rest_solace-0.1.0/tests/consumer_test.py`

 * *Files identical despite different names*

### Comparing `rest_solace-0.0.2/tests/manager_test.py` & `rest_solace-0.1.0/tests/manager_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,38 +24,26 @@
 
 #Testing getting an instance of manager class
 try:
     count.add_count()
     manager = Manager(user_name= SEMP_USERNAME, 
                       password= SEMP_PASSWORD, 
                       host= SEMP_HOST, 
-                      SEMP_port= SEMP_PORT)
+                      semp_port= SEMP_PORT)
     log.info("Testing the creation of manager instance: PASS\n")
     count.passed()
 except Exception as e:
     count.failed()
     log.error("Testing the creation of manager instance: FAIL")
     print("Stopping test early as unable to create instance of manager class")
     print(count.get_stats())
     log.error("Error str: "+str(e))
     exit(1)
 
 
-#Testing "get_about" function
-try:
-    count.add_count()
-    res = manager.get_about()
-    log.info("Function 'get_about': PASS")  
-    log.info(str(res)+'\n')
-    count.passed()
-except Exception as e:
-    count.failed()
-    log.info("Function 'get_about': FAIL")  
-    log.error("Error str: "+str(e))
-
 
 #Testing "get_about_api" function
 try:
     count.add_count()
     res = manager.get_about_api()
     log.info("Function 'get_about_api': PASS")  
     log.info(str(res)+'\n')
```

### Comparing `rest_solace-0.0.2/tests/pub_sub_test.py` & `rest_solace-0.1.0/tests/pub_sub_test.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,18 +16,18 @@
 
 INPUT_MESSAGE= "hello world!!"
 EXPECTED_OUTPUT_MESSAGE= bytes("HELLO WORLD!!", 'utf-8')
 
 manager = Manager(user_name= SEMP_USERNAME, 
                       password= SEMP_PASSWORD, 
                       host= SEMP_HOST, 
-                      SEMP_port= SEMP_PORT)
+                      semp_port= SEMP_PORT)
 
-publish_obj = MessagingPublisher(user_name="admin", password="admin", 
-                                 host= SEMP_HOST, REST_VPNport=NEW_VPN_PORT)
+publish = MessagingPublisher(user_name="admin", password="admin", 
+                             host= SEMP_HOST, rest_vpn_port=NEW_VPN_PORT)
 
 consumer_obj = Consumer()
 
 #Step1: setup broker to send and receive messages
 print("Setting up Message VPN, queue endpoint, and RDP.")
 
 res = manager.create_message_vpn(msgVpnName= NEW_VPN_NAME,
@@ -50,19 +50,18 @@
 
 manager.restart_rest_delivery_point(restDeliveryPointName= "myRDP", 
                                     msgVpnName= NEW_VPN_NAME)
 
 #Step4: setup publisher, publish a message, and get response
 print("\nPublishing a message and waiting for uppercase response\nSending message:", INPUT_MESSAGE)
 
-res = publish_obj.publishToQueueEndpoint(queue_name="queue_rest_consumer", 
-                                        message= INPUT_MESSAGE,
-                                        delivery_mode="persistent",
-                                        time_to_live= 10000 #waits 1 min
-                                        )
+res = publish.persistent_message_to_queue(queue_name="queue_rest_consumer", 
+                                          message= INPUT_MESSAGE,
+                                          time_to_live= 10000 #waits 1 min
+                                         )
 
 print("\nResponse:\n",res)
 
 if res.get('content') == EXPECTED_OUTPUT_MESSAGE:
     print("\nTest was a Success")
 else:
     print("\nTest was a Failure")
```

### Comparing `rest_solace-0.0.2/tests/util.py` & `rest_solace-0.1.0/tests/util.py`

 * *Files identical despite different names*

