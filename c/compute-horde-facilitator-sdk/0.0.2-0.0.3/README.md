# Comparing `tmp/compute_horde_facilitator_sdk-0.0.2.tar.gz` & `tmp/compute_horde_facilitator_sdk-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "compute_horde_facilitator_sdk-0.0.2.tar", last modified: Thu Apr 18 07:18:45 2024, max compression
+gzip compressed data, was "compute_horde_facilitator_sdk-0.0.3.tar", last modified: Sat May 18 21:56:03 2024, max compression
```

## Comparing `compute_horde_facilitator_sdk-0.0.2.tar` & `compute_horde_facilitator_sdk-0.0.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1079 2024-04-18 07:18:38.892714 compute_horde_facilitator_sdk-0.0.2/LICENSE
--rw-r--r--   0        0        0       32 2024-04-18 07:18:38.892714 compute_horde_facilitator_sdk-0.0.2/README.md
--rw-r--r--   0        0        0     1074 2024-04-18 07:18:45.300788 compute_horde_facilitator_sdk-0.0.2/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-18 07:18:38.892714 compute_horde_facilitator_sdk-0.0.2/src/compute_horde_facilitator_sdk/__init__.py
--rw-r--r--   0        0        0        0 2024-04-18 07:18:38.892714 compute_horde_facilitator_sdk-0.0.2/src/compute_horde_facilitator_sdk/_internal/__init__.py
--rw-r--r--   0        0        0     3418 2024-04-18 07:18:38.892714 compute_horde_facilitator_sdk-0.0.2/src/compute_horde_facilitator_sdk/_internal/sdk.py
--rw-r--r--   0        0        0      139 2024-04-18 07:18:38.892714 compute_horde_facilitator_sdk-0.0.2/src/compute_horde_facilitator_sdk/v1.py
--rw-r--r--   0        0        0        0 2024-04-18 07:18:38.892714 compute_horde_facilitator_sdk-0.0.2/tests/__init__.py
--rw-r--r--   0        0        0     4137 2024-04-18 07:18:38.892714 compute_horde_facilitator_sdk-0.0.2/tests/conftest.py
--rw-r--r--   0        0        0     3465 2024-04-18 07:18:38.892714 compute_horde_facilitator_sdk-0.0.2/tests/test_sdk.py
--rw-r--r--   0        0        0        0 2024-04-18 07:18:38.892714 compute_horde_facilitator_sdk-0.0.2/tests/v1/__init__.py
--rw-r--r--   0        0        0        0 2024-04-18 07:18:38.892714 compute_horde_facilitator_sdk-0.0.2/tests/v1/apiver/__init__.py
--rw-r--r--   0        0        0       62 2024-04-18 07:18:38.892714 compute_horde_facilitator_sdk-0.0.2/tests/v1/apiver/apiver_deps.py
--rw-r--r--   0        0        0      309 1970-01-01 00:00:00.000000 compute_horde_facilitator_sdk-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1079 2024-05-18 21:55:52.587234 compute_horde_facilitator_sdk-0.0.3/LICENSE
+-rw-r--r--   0        0        0     1173 2024-05-18 21:55:52.587234 compute_horde_facilitator_sdk-0.0.3/README.md
+-rw-r--r--   0        0        0     1074 2024-05-18 21:56:03.927334 compute_horde_facilitator_sdk-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-18 21:55:52.587234 compute_horde_facilitator_sdk-0.0.3/src/compute_horde_facilitator_sdk/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-18 21:55:52.587234 compute_horde_facilitator_sdk-0.0.3/src/compute_horde_facilitator_sdk/_internal/__init__.py
+-rw-r--r--   0        0        0     3498 2024-05-18 21:55:52.587234 compute_horde_facilitator_sdk-0.0.3/src/compute_horde_facilitator_sdk/_internal/sdk.py
+-rw-r--r--   0        0        0      139 2024-05-18 21:55:52.587234 compute_horde_facilitator_sdk-0.0.3/src/compute_horde_facilitator_sdk/v1.py
+-rw-r--r--   0        0        0        0 2024-05-18 21:55:52.587234 compute_horde_facilitator_sdk-0.0.3/tests/__init__.py
+-rw-r--r--   0        0        0     4137 2024-05-18 21:55:52.587234 compute_horde_facilitator_sdk-0.0.3/tests/conftest.py
+-rw-r--r--   0        0        0     3465 2024-05-18 21:55:52.587234 compute_horde_facilitator_sdk-0.0.3/tests/test_sdk.py
+-rw-r--r--   0        0        0        0 2024-05-18 21:55:52.587234 compute_horde_facilitator_sdk-0.0.3/tests/v1/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-18 21:55:52.587234 compute_horde_facilitator_sdk-0.0.3/tests/v1/apiver/__init__.py
+-rw-r--r--   0        0        0       62 2024-05-18 21:55:52.587234 compute_horde_facilitator_sdk-0.0.3/tests/v1/apiver/apiver_deps.py
+-rw-r--r--   0        0        0     1450 1970-01-01 00:00:00.000000 compute_horde_facilitator_sdk-0.0.3/PKG-INFO
```

### Comparing `compute_horde_facilitator_sdk-0.0.2/LICENSE` & `compute_horde_facilitator_sdk-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `compute_horde_facilitator_sdk-0.0.2/pyproject.toml` & `compute_horde_facilitator_sdk-0.0.3/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "compute-horde-facilitator-sdk"
-version = "0.0.2"
+version = "0.0.3"
 description = "SDK library to communicate with ComputeHorde Facilitator"
 authors = [
     { name = "Backend Developers LTD" },
 ]
 dependencies = [
     "httpx>=0.27.0",
 ]
```

### Comparing `compute_horde_facilitator_sdk-0.0.2/src/compute_horde_facilitator_sdk/_internal/sdk.py` & `compute_horde_facilitator_sdk-0.0.3/src/compute_horde_facilitator_sdk/_internal/sdk.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 from typing import Any
 
 import httpx
 
+BASE_URL = 'https://facilitator.computehorde.io/api/v1/'
+
 
 class FacilitatorClient:
-    def __init__(self, base_url: str, token: str):
+    def __init__(self, token: str, base_url: str = BASE_URL):
         self.base_url = base_url
         self.token = token
         self.client = httpx.Client(base_url=base_url, headers={"Authorization": f"Token {token}"})
 
     def __enter__(self):
         return self
 
@@ -51,15 +53,15 @@
         return response.json()
 
     def close(self):
         self.client.close()
 
 
 class AsyncFacilitatorClient:
-    def __init__(self, base_url: str, token: str):
+    def __init__(self, token: str, base_url: str = BASE_URL):
         self.base_url = base_url
         self.token = token
         self.client = httpx.AsyncClient(
             base_url=base_url, headers={"Authorization": f"Token {token}"}
         )
 
     async def __aenter__(self):
```

### Comparing `compute_horde_facilitator_sdk-0.0.2/tests/conftest.py` & `compute_horde_facilitator_sdk-0.0.3/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `compute_horde_facilitator_sdk-0.0.2/tests/test_sdk.py` & `compute_horde_facilitator_sdk-0.0.3/tests/test_sdk.py`

 * *Files identical despite different names*

