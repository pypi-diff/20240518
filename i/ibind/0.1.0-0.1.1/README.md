# Comparing `tmp/ibind-0.1.0.tar.gz` & `tmp/ibind-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ibind-0.1.0.tar", last modified: Mon May  6 12:43:09 2024, max compression
+gzip compressed data, was "ibind-0.1.1.tar", last modified: Sat May 18 04:44:43 2024, max compression
```

## Comparing `ibind-0.1.0.tar` & `ibind-0.1.1.tar`

### file list

```diff
@@ -1,64 +1,64 @@
-drwxrwxrwx   0        0        0        0 2024-05-06 12:43:09.663785 ibind-0.1.0/
--rw-rw-rw-   0        0        0    11562 2020-10-15 10:25:32.000000 ibind-0.1.0/LICENSE
--rw-rw-rw-   0        0        0    22426 2024-05-06 12:43:09.661766 ibind-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     8341 2024-05-06 12:41:34.000000 ibind-0.1.0/README.md
-drwxrwxrwx   0        0        0        0 2024-05-06 12:43:09.461540 ibind-0.1.0/ibind/
--rw-rw-rw-   0        0        0     1062 2024-05-02 11:52:19.000000 ibind-0.1.0/ibind/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-06 12:43:09.505550 ibind-0.1.0/ibind/base/
--rw-rw-rw-   0        0        0        0 2024-04-04 04:03:06.000000 ibind-0.1.0/ibind/base/__init__.py
--rw-rw-rw-   0        0        0     5286 2024-05-02 07:49:30.000000 ibind-0.1.0/ibind/base/queue_controller.py
--rw-rw-rw-   0        0        0     8555 2024-05-03 06:26:53.000000 ibind-0.1.0/ibind/base/rest_client.py
--rw-rw-rw-   0        0        0    16433 2024-05-03 05:09:05.000000 ibind-0.1.0/ibind/base/subscription_controller.py
--rw-rw-rw-   0        0        0    18799 2024-05-02 07:52:05.000000 ibind-0.1.0/ibind/base/ws_client.py
-drwxrwxrwx   0        0        0        0 2024-05-06 12:43:09.526561 ibind-0.1.0/ibind/client/
--rw-rw-rw-   0        0        0        0 2024-04-03 12:59:53.000000 ibind-0.1.0/ibind/client/__init__.py
--rw-rw-rw-   0        0        0     3653 2024-05-03 03:15:23.000000 ibind-0.1.0/ibind/client/ibkr_client.py
-drwxrwxrwx   0        0        0        0 2024-05-06 12:43:09.568673 ibind-0.1.0/ibind/client/ibkr_client_mixins/
--rw-rw-rw-   0        0        0        0 2024-04-04 04:14:49.000000 ibind-0.1.0/ibind/client/ibkr_client_mixins/__init__.py
--rw-rw-rw-   0        0        0     3400 2024-05-02 04:33:53.000000 ibind-0.1.0/ibind/client/ibkr_client_mixins/accounts_mixin.py
--rw-rw-rw-   0        0        0    16134 2024-05-03 09:06:05.000000 ibind-0.1.0/ibind/client/ibkr_client_mixins/contract_mixin.py
--rw-rw-rw-   0        0        0    12508 2024-05-02 07:59:06.000000 ibind-0.1.0/ibind/client/ibkr_client_mixins/marketdata_mixin.py
--rw-rw-rw-   0        0        0    10477 2024-05-02 10:28:02.000000 ibind-0.1.0/ibind/client/ibkr_client_mixins/order_mixin.py
--rw-rw-rw-   0        0        0     9585 2024-05-02 10:28:35.000000 ibind-0.1.0/ibind/client/ibkr_client_mixins/portfolio_mixin.py
--rw-rw-rw-   0        0        0     4220 2024-05-02 10:28:35.000000 ibind-0.1.0/ibind/client/ibkr_client_mixins/scanner_mixin.py
--rw-rw-rw-   0        0        0     4611 2024-05-02 10:28:43.000000 ibind-0.1.0/ibind/client/ibkr_client_mixins/session_mixin.py
--rw-rw-rw-   0        0        0     2343 2024-05-02 10:30:13.000000 ibind-0.1.0/ibind/client/ibkr_client_mixins/watchlist_mixin.py
--rw-rw-rw-   0        0        0    12413 2024-04-24 12:43:26.000000 ibind-0.1.0/ibind/client/ibkr_definitions.py
--rw-rw-rw-   0        0        0    16278 2024-05-02 06:20:14.000000 ibind-0.1.0/ibind/client/ibkr_utils.py
--rw-rw-rw-   0        0        0    28501 2024-05-03 06:27:53.000000 ibind-0.1.0/ibind/client/ibkr_ws_client.py
-drwxrwxrwx   0        0        0        0 2024-05-06 12:43:09.586673 ibind-0.1.0/ibind/support/
--rw-rw-rw-   0        0        0        0 2024-04-03 13:00:28.000000 ibind-0.1.0/ibind/support/__init__.py
--rw-rw-rw-   0        0        0      227 2024-04-01 07:18:14.000000 ibind-0.1.0/ibind/support/errors.py
--rw-rw-rw-   0        0        0     5612 2024-05-02 10:37:05.000000 ibind-0.1.0/ibind/support/logs.py
--rw-rw-rw-   0        0        0    11297 2024-05-03 05:07:31.000000 ibind-0.1.0/ibind/support/py_utils.py
--rw-rw-rw-   0        0        0     2035 2024-04-25 10:00:26.000000 ibind-0.1.0/ibind/var.py
-drwxrwxrwx   0        0        0        0 2024-05-06 12:43:09.657418 ibind-0.1.0/ibind.egg-info/
--rw-rw-rw-   0        0        0    22426 2024-05-06 12:43:09.000000 ibind-0.1.0/ibind.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1595 2024-05-06 12:43:09.000000 ibind-0.1.0/ibind.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-06 12:43:09.000000 ibind-0.1.0/ibind.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       41 2024-05-06 12:43:09.000000 ibind-0.1.0/ibind.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-05-06 12:43:09.000000 ibind-0.1.0/ibind.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1038 2024-05-06 12:42:22.000000 ibind-0.1.0/pyproject.toml
--rw-rw-rw-   0        0        0       86 2024-05-06 12:43:09.665820 ibind-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0      225 2024-05-02 11:52:19.000000 ibind-0.1.0/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-06 12:43:09.594672 ibind-0.1.0/test/
--rw-rw-rw-   0        0        0        0 2024-04-01 07:47:08.000000 ibind-0.1.0/test/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-06 12:43:09.598673 ibind-0.1.0/test/integration/
--rw-rw-rw-   0        0        0        0 2024-04-01 07:47:26.000000 ibind-0.1.0/test/integration/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-06 12:43:09.615672 ibind-0.1.0/test/integration/base/
--rw-rw-rw-   0        0        0        0 2024-04-01 07:37:06.000000 ibind-0.1.0/test/integration/base/__init__.py
--rw-rw-rw-   0        0        0     3714 2024-04-03 12:45:17.000000 ibind-0.1.0/test/integration/base/test_rest_client_i.py
--rw-rw-rw-   0        0        0    11025 2024-04-24 10:05:09.000000 ibind-0.1.0/test/integration/base/test_websocket_client_i.py
--rw-rw-rw-   0        0        0     1477 2023-12-13 15:29:14.000000 ibind-0.1.0/test/integration/base/websocketapp_mock.py
-drwxrwxrwx   0        0        0        0 2024-05-06 12:43:09.639672 ibind-0.1.0/test/integration/client/
--rw-rw-rw-   0        0        0        0 2024-04-01 07:57:40.000000 ibind-0.1.0/test/integration/client/__init__.py
--rw-rw-rw-   0        0        0    39617 2024-04-01 08:07:19.000000 ibind-0.1.0/test/integration/client/ibkr_responses.py
--rw-rw-rw-   0        0        0    14441 2024-04-25 11:38:46.000000 ibind-0.1.0/test/integration/client/test_ibkr_client_i.py
--rw-rw-rw-   0        0        0    11825 2024-04-03 12:28:11.000000 ibind-0.1.0/test/integration/client/test_ibkr_utils_i.py
--rw-rw-rw-   0        0        0    19149 2024-05-03 06:23:26.000000 ibind-0.1.0/test/integration/client/test_ibkr_ws_client_i.py
--rw-rw-rw-   0        0        0     8874 2024-04-03 12:27:51.000000 ibind-0.1.0/test/test_utils.py
-drwxrwxrwx   0        0        0        0 2024-05-06 12:43:09.643687 ibind-0.1.0/test/unit/
--rw-rw-rw-   0        0        0        0 2024-04-01 07:47:26.000000 ibind-0.1.0/test/unit/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-06 12:43:09.651692 ibind-0.1.0/test/unit/support/
--rw-rw-rw-   0        0        0        0 2024-04-01 07:45:52.000000 ibind-0.1.0/test/unit/support/__init__.py
--rw-rw-rw-   0        0        0     4517 2024-04-03 12:30:12.000000 ibind-0.1.0/test/unit/support/test_py_utils_u.py
+drwxrwxrwx   0        0        0        0 2024-05-18 04:44:43.344050 ibind-0.1.1/
+-rw-rw-rw-   0        0        0    11562 2020-10-15 10:25:32.000000 ibind-0.1.1/LICENSE
+-rw-rw-rw-   0        0        0    22426 2024-05-18 04:44:43.341050 ibind-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     8341 2024-05-06 13:31:55.000000 ibind-0.1.1/README.md
+drwxrwxrwx   0        0        0        0 2024-05-18 04:44:43.166744 ibind-0.1.1/ibind/
+-rw-rw-rw-   0        0        0     1062 2024-05-02 11:52:19.000000 ibind-0.1.1/ibind/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-18 04:44:43.205834 ibind-0.1.1/ibind/base/
+-rw-rw-rw-   0        0        0        0 2024-04-04 04:03:06.000000 ibind-0.1.1/ibind/base/__init__.py
+-rw-rw-rw-   0        0        0     5286 2024-05-02 07:49:30.000000 ibind-0.1.1/ibind/base/queue_controller.py
+-rw-rw-rw-   0        0        0     8555 2024-05-03 06:26:53.000000 ibind-0.1.1/ibind/base/rest_client.py
+-rw-rw-rw-   0        0        0    16433 2024-05-03 05:09:05.000000 ibind-0.1.1/ibind/base/subscription_controller.py
+-rw-rw-rw-   0        0        0    18799 2024-05-02 07:52:05.000000 ibind-0.1.1/ibind/base/ws_client.py
+drwxrwxrwx   0        0        0        0 2024-05-18 04:44:43.224300 ibind-0.1.1/ibind/client/
+-rw-rw-rw-   0        0        0        0 2024-04-03 12:59:53.000000 ibind-0.1.1/ibind/client/__init__.py
+-rw-rw-rw-   0        0        0     3653 2024-05-03 03:15:23.000000 ibind-0.1.1/ibind/client/ibkr_client.py
+drwxrwxrwx   0        0        0        0 2024-05-18 04:44:43.261037 ibind-0.1.1/ibind/client/ibkr_client_mixins/
+-rw-rw-rw-   0        0        0        0 2024-04-04 04:14:49.000000 ibind-0.1.1/ibind/client/ibkr_client_mixins/__init__.py
+-rw-rw-rw-   0        0        0     3400 2024-05-02 04:33:53.000000 ibind-0.1.1/ibind/client/ibkr_client_mixins/accounts_mixin.py
+-rw-rw-rw-   0        0        0    16134 2024-05-03 09:06:05.000000 ibind-0.1.1/ibind/client/ibkr_client_mixins/contract_mixin.py
+-rw-rw-rw-   0        0        0    12514 2024-05-18 03:10:13.000000 ibind-0.1.1/ibind/client/ibkr_client_mixins/marketdata_mixin.py
+-rw-rw-rw-   0        0        0    10477 2024-05-02 10:28:02.000000 ibind-0.1.1/ibind/client/ibkr_client_mixins/order_mixin.py
+-rw-rw-rw-   0        0        0     9585 2024-05-02 10:28:35.000000 ibind-0.1.1/ibind/client/ibkr_client_mixins/portfolio_mixin.py
+-rw-rw-rw-   0        0        0     4220 2024-05-02 10:28:35.000000 ibind-0.1.1/ibind/client/ibkr_client_mixins/scanner_mixin.py
+-rw-rw-rw-   0        0        0     4611 2024-05-02 10:28:43.000000 ibind-0.1.1/ibind/client/ibkr_client_mixins/session_mixin.py
+-rw-rw-rw-   0        0        0     2343 2024-05-02 10:30:13.000000 ibind-0.1.1/ibind/client/ibkr_client_mixins/watchlist_mixin.py
+-rw-rw-rw-   0        0        0    12413 2024-04-24 12:43:26.000000 ibind-0.1.1/ibind/client/ibkr_definitions.py
+-rw-rw-rw-   0        0        0    16278 2024-05-02 06:20:14.000000 ibind-0.1.1/ibind/client/ibkr_utils.py
+-rw-rw-rw-   0        0        0    28501 2024-05-03 06:27:53.000000 ibind-0.1.1/ibind/client/ibkr_ws_client.py
+drwxrwxrwx   0        0        0        0 2024-05-18 04:44:43.276085 ibind-0.1.1/ibind/support/
+-rw-rw-rw-   0        0        0        0 2024-04-03 13:00:28.000000 ibind-0.1.1/ibind/support/__init__.py
+-rw-rw-rw-   0        0        0      227 2024-04-01 07:18:14.000000 ibind-0.1.1/ibind/support/errors.py
+-rw-rw-rw-   0        0        0     5612 2024-05-02 10:37:05.000000 ibind-0.1.1/ibind/support/logs.py
+-rw-rw-rw-   0        0        0    11297 2024-05-03 05:07:31.000000 ibind-0.1.1/ibind/support/py_utils.py
+-rw-rw-rw-   0        0        0     2035 2024-04-25 10:00:26.000000 ibind-0.1.1/ibind/var.py
+drwxrwxrwx   0        0        0        0 2024-05-18 04:44:43.338053 ibind-0.1.1/ibind.egg-info/
+-rw-rw-rw-   0        0        0    22426 2024-05-18 04:44:43.000000 ibind-0.1.1/ibind.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1595 2024-05-18 04:44:43.000000 ibind-0.1.1/ibind.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-18 04:44:43.000000 ibind-0.1.1/ibind.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       41 2024-05-18 04:44:43.000000 ibind-0.1.1/ibind.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-05-18 04:44:43.000000 ibind-0.1.1/ibind.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1038 2024-05-18 04:44:15.000000 ibind-0.1.1/pyproject.toml
+-rw-rw-rw-   0        0        0       86 2024-05-18 04:44:43.346049 ibind-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0      225 2024-05-02 11:52:19.000000 ibind-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-18 04:44:43.283088 ibind-0.1.1/test/
+-rw-rw-rw-   0        0        0        0 2024-04-01 07:47:08.000000 ibind-0.1.1/test/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-18 04:44:43.287609 ibind-0.1.1/test/integration/
+-rw-rw-rw-   0        0        0        0 2024-04-01 07:47:26.000000 ibind-0.1.1/test/integration/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-18 04:44:43.302129 ibind-0.1.1/test/integration/base/
+-rw-rw-rw-   0        0        0        0 2024-04-01 07:37:06.000000 ibind-0.1.1/test/integration/base/__init__.py
+-rw-rw-rw-   0        0        0     3714 2024-04-03 12:45:17.000000 ibind-0.1.1/test/integration/base/test_rest_client_i.py
+-rw-rw-rw-   0        0        0    11025 2024-04-24 10:05:09.000000 ibind-0.1.1/test/integration/base/test_websocket_client_i.py
+-rw-rw-rw-   0        0        0     1477 2023-12-13 15:29:14.000000 ibind-0.1.1/test/integration/base/websocketapp_mock.py
+drwxrwxrwx   0        0        0        0 2024-05-18 04:44:43.321709 ibind-0.1.1/test/integration/client/
+-rw-rw-rw-   0        0        0        0 2024-04-01 07:57:40.000000 ibind-0.1.1/test/integration/client/__init__.py
+-rw-rw-rw-   0        0        0    39617 2024-04-01 08:07:19.000000 ibind-0.1.1/test/integration/client/ibkr_responses.py
+-rw-rw-rw-   0        0        0    14441 2024-04-25 11:38:46.000000 ibind-0.1.1/test/integration/client/test_ibkr_client_i.py
+-rw-rw-rw-   0        0        0    11825 2024-04-03 12:28:11.000000 ibind-0.1.1/test/integration/client/test_ibkr_utils_i.py
+-rw-rw-rw-   0        0        0    19149 2024-05-03 06:23:26.000000 ibind-0.1.1/test/integration/client/test_ibkr_ws_client_i.py
+-rw-rw-rw-   0        0        0     8874 2024-04-03 12:27:51.000000 ibind-0.1.1/test/test_utils.py
+drwxrwxrwx   0        0        0        0 2024-05-18 04:44:43.325710 ibind-0.1.1/test/unit/
+-rw-rw-rw-   0        0        0        0 2024-04-01 07:47:26.000000 ibind-0.1.1/test/unit/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-18 04:44:43.331814 ibind-0.1.1/test/unit/support/
+-rw-rw-rw-   0        0        0        0 2024-04-01 07:45:52.000000 ibind-0.1.1/test/unit/support/__init__.py
+-rw-rw-rw-   0        0        0     4517 2024-04-03 12:30:12.000000 ibind-0.1.1/test/unit/support/test_py_utils_u.py
```

### Comparing `ibind-0.1.0/LICENSE` & `ibind-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ibind-0.1.0/PKG-INFO` & `ibind-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ibind
-Version: 0.1.0
+Version: 0.1.1
 Summary: IBind is a REST and WebSocket client library for Interactive Brokers Client Portal Web API.
 Author-email: Voy Zan <voy1982@yahoo.co.uk>
 License: Copyright 2020 Voy Zan
         
                                          Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
```

### Comparing `ibind-0.1.0/README.md` & `ibind-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `ibind-0.1.0/ibind/__init__.py` & `ibind-0.1.1/ibind/__init__.py`

 * *Files identical despite different names*

### Comparing `ibind-0.1.0/ibind/base/queue_controller.py` & `ibind-0.1.1/ibind/base/queue_controller.py`

 * *Files identical despite different names*

### Comparing `ibind-0.1.0/ibind/base/rest_client.py` & `ibind-0.1.1/ibind/base/rest_client.py`

 * *Files identical despite different names*

### Comparing `ibind-0.1.0/ibind/base/subscription_controller.py` & `ibind-0.1.1/ibind/base/subscription_controller.py`

 * *Files identical despite different names*

### Comparing `ibind-0.1.0/ibind/base/ws_client.py` & `ibind-0.1.1/ibind/base/ws_client.py`

 * *Files identical despite different names*

### Comparing `ibind-0.1.0/ibind/client/ibkr_client.py` & `ibind-0.1.1/ibind/client/ibkr_client.py`

 * *Files identical despite different names*

### Comparing `ibind-0.1.0/ibind/client/ibkr_client_mixins/accounts_mixin.py` & `ibind-0.1.1/ibind/client/ibkr_client_mixins/accounts_mixin.py`

 * *Files identical despite different names*

### Comparing `ibind-0.1.0/ibind/client/ibkr_client_mixins/contract_mixin.py` & `ibind-0.1.1/ibind/client/ibkr_client_mixins/contract_mixin.py`

 * *Files identical despite different names*

### Comparing `ibind-0.1.0/ibind/client/ibkr_client_mixins/marketdata_mixin.py` & `ibind-0.1.1/ibind/client/ibkr_client_mixins/marketdata_mixin.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,15 +34,15 @@
             - The endpoint /iserver/accounts must be called prior to /iserver/marketdata/snapshot.
             - For derivative contracts, the endpoint /iserver/secdef/search must be called first.
         """
         params = {
             'conids': ','.join(conids),
             'fields': ','.join(fields)
         }
-        return self.get(f'iserver/secdef/search', params)
+        return self.get(f'iserver/marketdata/snapshot', params)
 
     def regulatory_snapshot(self: 'IbkrClient', conid: str) -> Result:  # pragma: no cover
         """
         Send a request for a regulatory snapshot. This will cost $0.01 USD per request unless you are subscribed to the direct exchange market data already.
 
         WARNING: Each regulatory snapshot made will incur a fee of $0.01 USD to the account. This applies to both live and paper accounts.
```

### Comparing `ibind-0.1.0/ibind/client/ibkr_client_mixins/order_mixin.py` & `ibind-0.1.1/ibind/client/ibkr_client_mixins/order_mixin.py`

 * *Files identical despite different names*

### Comparing `ibind-0.1.0/ibind/client/ibkr_client_mixins/portfolio_mixin.py` & `ibind-0.1.1/ibind/client/ibkr_client_mixins/portfolio_mixin.py`

 * *Files identical despite different names*

### Comparing `ibind-0.1.0/ibind/client/ibkr_client_mixins/scanner_mixin.py` & `ibind-0.1.1/ibind/client/ibkr_client_mixins/scanner_mixin.py`

 * *Files identical despite different names*

### Comparing `ibind-0.1.0/ibind/client/ibkr_client_mixins/session_mixin.py` & `ibind-0.1.1/ibind/client/ibkr_client_mixins/session_mixin.py`

 * *Files identical despite different names*

### Comparing `ibind-0.1.0/ibind/client/ibkr_client_mixins/watchlist_mixin.py` & `ibind-0.1.1/ibind/client/ibkr_client_mixins/watchlist_mixin.py`

 * *Files identical despite different names*

### Comparing `ibind-0.1.0/ibind/client/ibkr_definitions.py` & `ibind-0.1.1/ibind/client/ibkr_definitions.py`

 * *Files identical despite different names*

### Comparing `ibind-0.1.0/ibind/client/ibkr_utils.py` & `ibind-0.1.1/ibind/client/ibkr_utils.py`

 * *Files identical despite different names*

### Comparing `ibind-0.1.0/ibind/client/ibkr_ws_client.py` & `ibind-0.1.1/ibind/client/ibkr_ws_client.py`

 * *Files identical despite different names*

### Comparing `ibind-0.1.0/ibind/support/logs.py` & `ibind-0.1.1/ibind/support/logs.py`

 * *Files identical despite different names*

### Comparing `ibind-0.1.0/ibind/support/py_utils.py` & `ibind-0.1.1/ibind/support/py_utils.py`

 * *Files identical despite different names*

### Comparing `ibind-0.1.0/ibind/var.py` & `ibind-0.1.1/ibind/var.py`

 * *Files identical despite different names*

### Comparing `ibind-0.1.0/ibind.egg-info/PKG-INFO` & `ibind-0.1.1/ibind.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ibind
-Version: 0.1.0
+Version: 0.1.1
 Summary: IBind is a REST and WebSocket client library for Interactive Brokers Client Portal Web API.
 Author-email: Voy Zan <voy1982@yahoo.co.uk>
 License: Copyright 2020 Voy Zan
         
                                          Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
```

### Comparing `ibind-0.1.0/ibind.egg-info/SOURCES.txt` & `ibind-0.1.1/ibind.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ibind-0.1.0/pyproject.toml` & `ibind-0.1.1/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "ibind"
-version = "0.1.0"
+version = "0.1.1"
 authors = [
     { name="Voy Zan", email="voy1982@yahoo.co.uk" },
 ]
 description = "IBind is a REST and WebSocket client library for Interactive Brokers Client Portal Web API."
 readme = "README.md"
 requires-python = ">=3.8"
 license={ file = "LICENSE" }
```

### Comparing `ibind-0.1.0/test/integration/base/test_rest_client_i.py` & `ibind-0.1.1/test/integration/base/test_rest_client_i.py`

 * *Files identical despite different names*

### Comparing `ibind-0.1.0/test/integration/base/test_websocket_client_i.py` & `ibind-0.1.1/test/integration/base/test_websocket_client_i.py`

 * *Files identical despite different names*

### Comparing `ibind-0.1.0/test/integration/base/websocketapp_mock.py` & `ibind-0.1.1/test/integration/base/websocketapp_mock.py`

 * *Files identical despite different names*

### Comparing `ibind-0.1.0/test/integration/client/ibkr_responses.py` & `ibind-0.1.1/test/integration/client/ibkr_responses.py`

 * *Files identical despite different names*

### Comparing `ibind-0.1.0/test/integration/client/test_ibkr_client_i.py` & `ibind-0.1.1/test/integration/client/test_ibkr_client_i.py`

 * *Files identical despite different names*

### Comparing `ibind-0.1.0/test/integration/client/test_ibkr_utils_i.py` & `ibind-0.1.1/test/integration/client/test_ibkr_utils_i.py`

 * *Files identical despite different names*

### Comparing `ibind-0.1.0/test/integration/client/test_ibkr_ws_client_i.py` & `ibind-0.1.1/test/integration/client/test_ibkr_ws_client_i.py`

 * *Files identical despite different names*

### Comparing `ibind-0.1.0/test/test_utils.py` & `ibind-0.1.1/test/test_utils.py`

 * *Files identical despite different names*

### Comparing `ibind-0.1.0/test/unit/support/test_py_utils_u.py` & `ibind-0.1.1/test/unit/support/test_py_utils_u.py`

 * *Files identical despite different names*

