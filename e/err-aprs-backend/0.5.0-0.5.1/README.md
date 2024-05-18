# Comparing `tmp/err_aprs_backend-0.5.0.tar.gz` & `tmp/err_aprs_backend-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "err_aprs_backend-0.5.0.tar", max compression
+gzip compressed data, was "err_aprs_backend-0.5.1.tar", max compression
```

## Comparing `err_aprs_backend-0.5.0.tar` & `err_aprs_backend-0.5.1.tar`

### file list

```diff
@@ -1,39 +1,39 @@
--rw-r--r--   0        0        0     1063 2024-05-09 23:51:57.882527 err_aprs_backend-0.5.0/LICENSE
--rw-r--r--   0        0        0     4600 2024-05-09 23:51:57.882527 err_aprs_backend-0.5.0/README.md
--rw-r--r--   0        0        0      165 2024-05-09 23:51:57.882527 err_aprs_backend-0.5.0/aprs_backend/APRSHealth.plug
--rw-r--r--   0        0        0      161 2024-05-09 23:51:57.882527 err_aprs_backend-0.5.0/aprs_backend/APRSHelp.plug
--rw-r--r--   0        0        0      165 2024-05-09 23:51:57.882527 err_aprs_backend-0.5.0/aprs_backend/APRSWebserver.plug
--rw-r--r--   0        0        0      105 2024-05-09 23:51:57.882527 err_aprs_backend-0.5.0/aprs_backend/__init__.py
--rw-r--r--   0        0        0      138 2024-05-09 23:51:57.882527 err_aprs_backend-0.5.0/aprs_backend/aprs.plug
--rw-r--r--   0        0        0    21550 2024-05-09 23:51:57.882527 err_aprs_backend-0.5.0/aprs_backend/aprs.py
--rw-r--r--   0        0        0      188 2024-05-09 23:51:57.882527 err_aprs_backend-0.5.0/aprs_backend/aprs_core_plugins.py
--rw-r--r--   0        0        0      212 2024-05-09 23:51:57.882527 err_aprs_backend-0.5.0/aprs_backend/clients/__init__.py
--rw-r--r--   0        0        0      959 2024-05-09 23:51:57.882527 err_aprs_backend-0.5.0/aprs_backend/clients/_base.py
--rw-r--r--   0        0        0     2174 2024-05-09 23:51:57.882527 err_aprs_backend-0.5.0/aprs_backend/clients/aprs_registry.py
--rw-r--r--   0        0        0     6945 2024-05-09 23:51:57.882527 err_aprs_backend-0.5.0/aprs_backend/clients/aprsis.py
--rw-r--r--   0        0        0     1560 2024-05-09 23:51:57.882527 err_aprs_backend-0.5.0/aprs_backend/clients/beacon.py
--rw-r--r--   0        0        0       82 2024-05-09 23:51:57.882527 err_aprs_backend-0.5.0/aprs_backend/clients/kiss.py
--rw-r--r--   0        0        0      562 2024-05-09 23:51:57.882527 err_aprs_backend-0.5.0/aprs_backend/exceptions/__init__.py
--rw-r--r--   0        0        0       48 2024-05-09 23:51:57.882527 err_aprs_backend-0.5.0/aprs_backend/exceptions/base.py
--rw-r--r--   0        0        0      158 2024-05-09 23:51:57.882527 err_aprs_backend-0.5.0/aprs_backend/exceptions/client/__init__.py
--rw-r--r--   0        0        0      396 2024-05-09 23:51:57.886527 err_aprs_backend-0.5.0/aprs_backend/exceptions/client/aprsis.py
--rw-r--r--   0        0        0      118 2024-05-09 23:51:57.886527 err_aprs_backend-0.5.0/aprs_backend/exceptions/packets/__init__.py
--rw-r--r--   0        0        0      112 2024-05-09 23:51:57.886527 err_aprs_backend-0.5.0/aprs_backend/exceptions/packets/parser.py
--rw-r--r--   0        0        0      117 2024-05-09 23:51:57.886527 err_aprs_backend-0.5.0/aprs_backend/exceptions/processor.py
--rw-r--r--   0        0        0      744 2024-05-09 23:51:57.886527 err_aprs_backend-0.5.0/aprs_backend/message.py
--rw-r--r--   0        0        0     9038 2024-05-09 23:51:57.886527 err_aprs_backend-0.5.0/aprs_backend/packets/__init__.py
--rw-r--r--   0        0        0    10116 2024-05-09 23:51:57.886527 err_aprs_backend-0.5.0/aprs_backend/packets/parser.py
--rw-r--r--   0        0        0     1038 2024-05-09 23:51:57.886527 err_aprs_backend-0.5.0/aprs_backend/person.py
--rw-r--r--   0        0        0      204 2024-05-09 23:51:57.886527 err_aprs_backend-0.5.0/aprs_backend/plugins/__init__.py
--rw-r--r--   0        0        0     2099 2024-05-09 23:51:57.886527 err_aprs_backend-0.5.0/aprs_backend/plugins/health.py
--rw-r--r--   0        0        0      695 2024-05-09 23:51:57.886527 err_aprs_backend-0.5.0/aprs_backend/plugins/help.py
--rw-r--r--   0        0        0     2345 2024-05-09 23:51:57.886527 err_aprs_backend-0.5.0/aprs_backend/plugins/web.py
--rw-r--r--   0        0        0       83 2024-05-09 23:51:57.886527 err_aprs_backend-0.5.0/aprs_backend/room.py
--rw-r--r--   0        0        0      495 2024-05-09 23:51:57.886527 err_aprs_backend-0.5.0/aprs_backend/utils/__init__.py
--rw-r--r--   0        0        0      975 2024-05-09 23:51:57.886527 err_aprs_backend-0.5.0/aprs_backend/utils/counter.py
--rw-r--r--   0        0        0      118 2024-05-09 23:51:57.886527 err_aprs_backend-0.5.0/aprs_backend/utils/datetime.py
--rw-r--r--   0        0        0     8386 2024-05-09 23:51:57.886527 err_aprs_backend-0.5.0/aprs_backend/utils/plugins.py
--rw-r--r--   0        0        0      565 2024-05-09 23:51:57.886527 err_aprs_backend-0.5.0/aprs_backend/utils/position.py
--rw-r--r--   0        0        0       22 2024-05-09 23:51:57.886527 err_aprs_backend-0.5.0/aprs_backend/version.py
--rw-r--r--   0        0        0     1483 2024-05-09 23:51:57.886527 err_aprs_backend-0.5.0/pyproject.toml
--rw-r--r--   0        0        0     5272 1970-01-01 00:00:00.000000 err_aprs_backend-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0     1063 2024-05-18 16:19:51.506029 err_aprs_backend-0.5.1/LICENSE
+-rw-r--r--   0        0        0     4600 2024-05-18 16:19:51.506029 err_aprs_backend-0.5.1/README.md
+-rw-r--r--   0        0        0      165 2024-05-18 16:19:51.506029 err_aprs_backend-0.5.1/aprs_backend/APRSHealth.plug
+-rw-r--r--   0        0        0      161 2024-05-18 16:19:51.506029 err_aprs_backend-0.5.1/aprs_backend/APRSHelp.plug
+-rw-r--r--   0        0        0      165 2024-05-18 16:19:51.506029 err_aprs_backend-0.5.1/aprs_backend/APRSWebserver.plug
+-rw-r--r--   0        0        0      105 2024-05-18 16:19:51.506029 err_aprs_backend-0.5.1/aprs_backend/__init__.py
+-rw-r--r--   0        0        0      138 2024-05-18 16:19:51.506029 err_aprs_backend-0.5.1/aprs_backend/aprs.plug
+-rw-r--r--   0        0        0    21550 2024-05-18 16:19:51.506029 err_aprs_backend-0.5.1/aprs_backend/aprs.py
+-rw-r--r--   0        0        0      188 2024-05-18 16:19:51.506029 err_aprs_backend-0.5.1/aprs_backend/aprs_core_plugins.py
+-rw-r--r--   0        0        0      212 2024-05-18 16:19:51.506029 err_aprs_backend-0.5.1/aprs_backend/clients/__init__.py
+-rw-r--r--   0        0        0      959 2024-05-18 16:19:51.506029 err_aprs_backend-0.5.1/aprs_backend/clients/_base.py
+-rw-r--r--   0        0        0     2174 2024-05-18 16:19:51.506029 err_aprs_backend-0.5.1/aprs_backend/clients/aprs_registry.py
+-rw-r--r--   0        0        0     6945 2024-05-18 16:19:51.506029 err_aprs_backend-0.5.1/aprs_backend/clients/aprsis.py
+-rw-r--r--   0        0        0     1560 2024-05-18 16:19:51.506029 err_aprs_backend-0.5.1/aprs_backend/clients/beacon.py
+-rw-r--r--   0        0        0       82 2024-05-18 16:19:51.506029 err_aprs_backend-0.5.1/aprs_backend/clients/kiss.py
+-rw-r--r--   0        0        0      562 2024-05-18 16:19:51.506029 err_aprs_backend-0.5.1/aprs_backend/exceptions/__init__.py
+-rw-r--r--   0        0        0       48 2024-05-18 16:19:51.506029 err_aprs_backend-0.5.1/aprs_backend/exceptions/base.py
+-rw-r--r--   0        0        0      158 2024-05-18 16:19:51.506029 err_aprs_backend-0.5.1/aprs_backend/exceptions/client/__init__.py
+-rw-r--r--   0        0        0      396 2024-05-18 16:19:51.506029 err_aprs_backend-0.5.1/aprs_backend/exceptions/client/aprsis.py
+-rw-r--r--   0        0        0      118 2024-05-18 16:19:51.506029 err_aprs_backend-0.5.1/aprs_backend/exceptions/packets/__init__.py
+-rw-r--r--   0        0        0      112 2024-05-18 16:19:51.506029 err_aprs_backend-0.5.1/aprs_backend/exceptions/packets/parser.py
+-rw-r--r--   0        0        0      117 2024-05-18 16:19:51.506029 err_aprs_backend-0.5.1/aprs_backend/exceptions/processor.py
+-rw-r--r--   0        0        0      744 2024-05-18 16:19:51.506029 err_aprs_backend-0.5.1/aprs_backend/message.py
+-rw-r--r--   0        0        0     9038 2024-05-18 16:19:51.506029 err_aprs_backend-0.5.1/aprs_backend/packets/__init__.py
+-rw-r--r--   0        0        0    10116 2024-05-18 16:19:51.506029 err_aprs_backend-0.5.1/aprs_backend/packets/parser.py
+-rw-r--r--   0        0        0     1038 2024-05-18 16:19:51.506029 err_aprs_backend-0.5.1/aprs_backend/person.py
+-rw-r--r--   0        0        0      204 2024-05-18 16:19:51.506029 err_aprs_backend-0.5.1/aprs_backend/plugins/__init__.py
+-rw-r--r--   0        0        0     2099 2024-05-18 16:19:51.506029 err_aprs_backend-0.5.1/aprs_backend/plugins/health.py
+-rw-r--r--   0        0        0      695 2024-05-18 16:19:51.506029 err_aprs_backend-0.5.1/aprs_backend/plugins/help.py
+-rw-r--r--   0        0        0     2345 2024-05-18 16:19:51.506029 err_aprs_backend-0.5.1/aprs_backend/plugins/web.py
+-rw-r--r--   0        0        0       83 2024-05-18 16:19:51.506029 err_aprs_backend-0.5.1/aprs_backend/room.py
+-rw-r--r--   0        0        0      495 2024-05-18 16:19:51.506029 err_aprs_backend-0.5.1/aprs_backend/utils/__init__.py
+-rw-r--r--   0        0        0      975 2024-05-18 16:19:51.506029 err_aprs_backend-0.5.1/aprs_backend/utils/counter.py
+-rw-r--r--   0        0        0      118 2024-05-18 16:19:51.506029 err_aprs_backend-0.5.1/aprs_backend/utils/datetime.py
+-rw-r--r--   0        0        0     8386 2024-05-18 16:19:51.506029 err_aprs_backend-0.5.1/aprs_backend/utils/plugins.py
+-rw-r--r--   0        0        0      565 2024-05-18 16:19:51.506029 err_aprs_backend-0.5.1/aprs_backend/utils/position.py
+-rw-r--r--   0        0        0       22 2024-05-18 16:19:51.506029 err_aprs_backend-0.5.1/aprs_backend/version.py
+-rw-r--r--   0        0        0     1492 2024-05-18 16:19:51.510029 err_aprs_backend-0.5.1/pyproject.toml
+-rw-r--r--   0        0        0     5272 1970-01-01 00:00:00.000000 err_aprs_backend-0.5.1/PKG-INFO
```

### Comparing `err_aprs_backend-0.5.0/LICENSE` & `err_aprs_backend-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `err_aprs_backend-0.5.0/README.md` & `err_aprs_backend-0.5.1/README.md`

 * *Files identical despite different names*

### Comparing `err_aprs_backend-0.5.0/aprs_backend/aprs.py` & `err_aprs_backend-0.5.1/aprs_backend/aprs.py`

 * *Files identical despite different names*

### Comparing `err_aprs_backend-0.5.0/aprs_backend/clients/_base.py` & `err_aprs_backend-0.5.1/aprs_backend/clients/_base.py`

 * *Files identical despite different names*

### Comparing `err_aprs_backend-0.5.0/aprs_backend/clients/aprs_registry.py` & `err_aprs_backend-0.5.1/aprs_backend/clients/aprs_registry.py`

 * *Files identical despite different names*

### Comparing `err_aprs_backend-0.5.0/aprs_backend/clients/aprsis.py` & `err_aprs_backend-0.5.1/aprs_backend/clients/aprsis.py`

 * *Files identical despite different names*

### Comparing `err_aprs_backend-0.5.0/aprs_backend/clients/beacon.py` & `err_aprs_backend-0.5.1/aprs_backend/clients/beacon.py`

 * *Files identical despite different names*

### Comparing `err_aprs_backend-0.5.0/aprs_backend/exceptions/__init__.py` & `err_aprs_backend-0.5.1/aprs_backend/exceptions/__init__.py`

 * *Files identical despite different names*

### Comparing `err_aprs_backend-0.5.0/aprs_backend/message.py` & `err_aprs_backend-0.5.1/aprs_backend/message.py`

 * *Files identical despite different names*

### Comparing `err_aprs_backend-0.5.0/aprs_backend/packets/__init__.py` & `err_aprs_backend-0.5.1/aprs_backend/packets/__init__.py`

 * *Files identical despite different names*

### Comparing `err_aprs_backend-0.5.0/aprs_backend/packets/parser.py` & `err_aprs_backend-0.5.1/aprs_backend/packets/parser.py`

 * *Files identical despite different names*

### Comparing `err_aprs_backend-0.5.0/aprs_backend/person.py` & `err_aprs_backend-0.5.1/aprs_backend/person.py`

 * *Files identical despite different names*

### Comparing `err_aprs_backend-0.5.0/aprs_backend/plugins/health.py` & `err_aprs_backend-0.5.1/aprs_backend/plugins/health.py`

 * *Files identical despite different names*

### Comparing `err_aprs_backend-0.5.0/aprs_backend/plugins/help.py` & `err_aprs_backend-0.5.1/aprs_backend/plugins/help.py`

 * *Files identical despite different names*

### Comparing `err_aprs_backend-0.5.0/aprs_backend/plugins/web.py` & `err_aprs_backend-0.5.1/aprs_backend/plugins/web.py`

 * *Files identical despite different names*

### Comparing `err_aprs_backend-0.5.0/aprs_backend/utils/counter.py` & `err_aprs_backend-0.5.1/aprs_backend/utils/counter.py`

 * *Files identical despite different names*

### Comparing `err_aprs_backend-0.5.0/aprs_backend/utils/plugins.py` & `err_aprs_backend-0.5.1/aprs_backend/utils/plugins.py`

 * *Files identical despite different names*

### Comparing `err_aprs_backend-0.5.0/aprs_backend/utils/position.py` & `err_aprs_backend-0.5.1/aprs_backend/utils/position.py`

 * *Files identical despite different names*

### Comparing `err_aprs_backend-0.5.0/pyproject.toml` & `err_aprs_backend-0.5.1/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "err-aprs-backend"
-version = "0.5.0"
+version = "0.5.1"
 description = "Errbot APRS backend plugin"
 authors = ["Andrew Herrington <andrew.the.techie@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "aprs_backend"}]
 include = ["*.plug"]
 
@@ -25,20 +25,20 @@
 [tool.poetry.plugins."errbot.plugins"]
 help = "aprs_backend:APRSHelp"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^8.1.1"
 coverage = {extras = ["toml"], version = ">=6.5,<8.0"}
 pre-commit = ">=2.12.1"
-pep8-naming = "^0.13.2"
+pep8-naming = ">=0.13.2,<0.15.0"
 reorder-python-imports = "^3.9.0"
 pre-commit-hooks = "^4.2.0"
 pyupgrade = "^3.15.2"
 pytest-xdist = "^3.1.0"
-ruff = ">=0.0.249,<0.4.4"
+ruff = ">=0.0.249,<0.4.5"
 bandit = "^1.7.8"
 pytest-subtests = "^0.12.1"
 pytest-cov = "^5.0.0"
 pytest-asyncio = "^0.23.6"
 pytest-httpx = "^0.30.0"
```

### Comparing `err_aprs_backend-0.5.0/PKG-INFO` & `err_aprs_backend-0.5.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: err-aprs-backend
-Version: 0.5.0
+Version: 0.5.1
 Summary: Errbot APRS backend plugin
 License: MIT
 Author: Andrew Herrington
 Author-email: andrew.the.techie@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

