# Comparing `tmp/bismuthsdk-0.1.8.tar.gz` & `tmp/bismuthsdk-0.1.9.tar.gz`

## Comparing `bismuthsdk-0.1.8.tar` & `bismuthsdk-0.1.9.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0      402 2020-02-02 00:00:00.000000 bismuthsdk-0.1.8/src/bismuth/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bismuthsdk-0.1.8/src/bismuth/codeblocks/__init__.py
--rw-r--r--   0        0        0     2882 2020-02-02 00:00:00.000000 bismuthsdk-0.1.8/src/bismuth/codeblocks/api_code_block.py
--rw-r--r--   0        0        0     3993 2020-02-02 00:00:00.000000 bismuthsdk-0.1.8/src/bismuth/codeblocks/api_code_block_with_storage.py
--rw-r--r--   0        0        0     1229 2020-02-02 00:00:00.000000 bismuthsdk-0.1.8/src/bismuth/codeblocks/auth_code_block.py
--rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 bismuthsdk-0.1.8/src/bismuth/codeblocks/base_code_block.py
--rw-r--r--   0        0        0     1118 2020-02-02 00:00:00.000000 bismuthsdk-0.1.8/src/bismuth/codeblocks/configuration_code_block.py
--rw-r--r--   0        0        0      968 2020-02-02 00:00:00.000000 bismuthsdk-0.1.8/src/bismuth/codeblocks/data_storage_code_block.py
--rw-r--r--   0        0        0      412 2020-02-02 00:00:00.000000 bismuthsdk-0.1.8/src/bismuth/codeblocks/function_code_block.py
--rw-r--r--   0        0        0     2436 2020-02-02 00:00:00.000000 bismuthsdk-0.1.8/src/bismuth/codeblocks/persistent_data_storage_code_block.py
--rw-r--r--   0        0        0      818 2020-02-02 00:00:00.000000 bismuthsdk-0.1.8/src/bismuth/codeblocks/test_api_code_block.py
--rw-r--r--   0        0        0      908 2020-02-02 00:00:00.000000 bismuthsdk-0.1.8/src/bismuth/codeblocks/test_api_code_block_with_storage.py
--rw-r--r--   0        0        0     1502 2020-02-02 00:00:00.000000 bismuthsdk-0.1.8/src/bismuth/codeblocks/test_configuration_code_block.py
--rw-r--r--   0        0        0     1310 2020-02-02 00:00:00.000000 bismuthsdk-0.1.8/src/bismuth/codeblocks/test_data_storage_block.py
--rw-r--r--   0        0        0     4159 2020-02-02 00:00:00.000000 bismuthsdk-0.1.8/src/bismuth/codeblocks/test_persistent_data_storage_block.py
--rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 bismuthsdk-0.1.8/.gitignore
--rw-r--r--   0        0        0      551 2020-02-02 00:00:00.000000 bismuthsdk-0.1.8/pyproject.toml
--rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 bismuthsdk-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0      410 2020-02-02 00:00:00.000000 bismuthsdk-0.1.9/src/bismuth/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bismuthsdk-0.1.9/src/bismuth/codeblocks/__init__.py
+-rw-r--r--   0        0        0     2945 2020-02-02 00:00:00.000000 bismuthsdk-0.1.9/src/bismuth/codeblocks/api_code_block.py
+-rw-r--r--   0        0        0     3993 2020-02-02 00:00:00.000000 bismuthsdk-0.1.9/src/bismuth/codeblocks/api_code_block_with_storage.py
+-rw-r--r--   0        0        0     1229 2020-02-02 00:00:00.000000 bismuthsdk-0.1.9/src/bismuth/codeblocks/auth_code_block.py
+-rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 bismuthsdk-0.1.9/src/bismuth/codeblocks/base_code_block.py
+-rw-r--r--   0        0        0     1456 2020-02-02 00:00:00.000000 bismuthsdk-0.1.9/src/bismuth/codeblocks/configuration_code_block.py
+-rw-r--r--   0        0        0      968 2020-02-02 00:00:00.000000 bismuthsdk-0.1.9/src/bismuth/codeblocks/data_storage_code_block.py
+-rw-r--r--   0        0        0      412 2020-02-02 00:00:00.000000 bismuthsdk-0.1.9/src/bismuth/codeblocks/function_code_block.py
+-rw-r--r--   0        0        0     2798 2020-02-02 00:00:00.000000 bismuthsdk-0.1.9/src/bismuth/codeblocks/persistent_data_storage_code_block.py
+-rw-r--r--   0        0        0      818 2020-02-02 00:00:00.000000 bismuthsdk-0.1.9/src/bismuth/codeblocks/test_api_code_block.py
+-rw-r--r--   0        0        0      908 2020-02-02 00:00:00.000000 bismuthsdk-0.1.9/src/bismuth/codeblocks/test_api_code_block_with_storage.py
+-rw-r--r--   0        0        0     1502 2020-02-02 00:00:00.000000 bismuthsdk-0.1.9/src/bismuth/codeblocks/test_configuration_code_block.py
+-rw-r--r--   0        0        0     1310 2020-02-02 00:00:00.000000 bismuthsdk-0.1.9/src/bismuth/codeblocks/test_data_storage_block.py
+-rw-r--r--   0        0        0     4159 2020-02-02 00:00:00.000000 bismuthsdk-0.1.9/src/bismuth/codeblocks/test_persistent_data_storage_block.py
+-rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 bismuthsdk-0.1.9/.gitignore
+-rw-r--r--   0        0        0      551 2020-02-02 00:00:00.000000 bismuthsdk-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 bismuthsdk-0.1.9/PKG-INFO
```

### Comparing `bismuthsdk-0.1.8/src/bismuth/codeblocks/api_code_block.py` & `bismuthsdk-0.1.9/src/bismuth/codeblocks/api_code_block.py`

 * *Files 3% similar despite different names*

```diff
@@ -79,9 +79,12 @@
                 if "DELETE" in methods:
                     return auth_handler("DELETE", handlers, require_auth, **kwargs)
                 else:
                     self.api.abort(404)
 
         self.api.add_resource(DynamicResource, route)
 
+    def __call__(self, *args):
+        return self.app(*args)
+
     def run(self, host="0.0.0.0", port=5000, debug=False):
         self.app.run(host=host, port=port, debug=debug)
```

### Comparing `bismuthsdk-0.1.8/src/bismuth/codeblocks/api_code_block_with_storage.py` & `bismuthsdk-0.1.9/src/bismuth/codeblocks/api_code_block_with_storage.py`

 * *Files identical despite different names*

### Comparing `bismuthsdk-0.1.8/src/bismuth/codeblocks/auth_code_block.py` & `bismuthsdk-0.1.9/src/bismuth/codeblocks/auth_code_block.py`

 * *Files identical despite different names*

### Comparing `bismuthsdk-0.1.8/src/bismuth/codeblocks/configuration_code_block.py` & `bismuthsdk-0.1.9/src/bismuth/codeblocks/configuration_code_block.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import os
 import requests
+from flask import request
 from http import HTTPStatus
 from typing import Optional
 from urllib.parse import urljoin
 
 from .base_code_block import BaseCodeBlock
 
 
@@ -16,14 +17,24 @@
 
     def __init__(self, api_url="http://169.254.169.254:9000/secrets/v1/"):
         if 'BISMUTH_AUTH' not in os.environ:
             raise Exception("Missing BISMUTH_AUTH token in environment.")
         self.auth = {"Authorization": "Bearer " + os.environ['BISMUTH_AUTH']}
         self.api_url = api_url
 
+    def _headers(self):
+        hdrs = self.auth.copy()
+        try:
+            for tracehdr in ["traceparent", "tracestate"]:
+                if tracehdr in request.headers:
+                    hdrs[tracehdr] = request.headers[tracehdr]
+        except RuntimeError:
+            pass
+        return hdrs
+
     def get(self, key) -> Optional[str]:
-        resp = requests.get(urljoin(self.api_url, key), headers=self.auth)
+        resp = requests.get(urljoin(self.api_url, key), headers=self._headers())
         if resp.status_code == HTTPStatus.NOT_FOUND:
             raise AttributeError(f"Configuration key {key} not set")
         elif not resp.ok:
             raise Exception(f"Server error {resp}")
         return resp.text
```

### Comparing `bismuthsdk-0.1.8/src/bismuth/codeblocks/data_storage_code_block.py` & `bismuthsdk-0.1.9/src/bismuth/codeblocks/data_storage_code_block.py`

 * *Files identical despite different names*

### Comparing `bismuthsdk-0.1.8/src/bismuth/codeblocks/persistent_data_storage_code_block.py` & `bismuthsdk-0.1.9/src/bismuth/codeblocks/persistent_data_storage_code_block.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import json
 import os
 import requests
+from flask import request
 from http import HTTPStatus
 from typing import Optional, Dict, Any
 from urllib.parse import urljoin
 
 from .data_storage_code_block import DataStorageCodeBlock
 
 
@@ -14,46 +15,56 @@
     """
     def __init__(self, api_url="http://169.254.169.254:9000/blob/v1/"):
         if 'BISMUTH_AUTH' not in os.environ:
             raise Exception("Missing BISMUTH_AUTH token in environment.")
         self.auth = {"Authorization": os.environ['BISMUTH_AUTH']}
         self.api_url = api_url
 
+    def _headers(self):
+        hdrs = self.auth.copy()
+        try:
+            for tracehdr in ["traceparent", "tracestate"]:
+                if tracehdr in request.headers:
+                    hdrs[tracehdr] = request.headers[tracehdr]
+        except RuntimeError:
+            pass
+        return hdrs
+
     def create(self, key, value) -> None:
         """Create a new item in the datastore."""
-        resp = requests.post(urljoin(self.api_url, key), data=json.dumps(value), headers=self.auth)
+        resp = requests.post(urljoin(self.api_url, key), data=json.dumps(value), headers=self._headers())
         if resp.status_code == HTTPStatus.CONFLICT:
             raise ValueError("Key already exists.")
         elif not resp.ok:
             raise Exception(f"Server error {resp}")
 
     def retrieve(self, key) -> Optional[Any]:
         """Retrieve an item from the datastore."""
-        resp = requests.get(urljoin(self.api_url, key), headers=self.auth)
+        resp = requests.get(urljoin(self.api_url, key), headers=self._headers())
         if resp.status_code == HTTPStatus.NOT_FOUND:
             return None
         elif not resp.ok:
             raise Exception(f"Server error {resp}")
         return resp.json()
 
     def update(self, key, value) -> None:
         """Update an existing item in the datastore."""
-        resp = requests.put(urljoin(self.api_url, key), data=json.dumps(value), headers=self.auth)
+        resp = requests.put(urljoin(self.api_url, key), data=json.dumps(value), headers=self._headers())
         if resp.status_code == HTTPStatus.NOT_FOUND:
             raise ValueError("Key does not exist.")
         elif not resp.ok:
             raise Exception(f"Server error {resp}")
 
     def delete(self, key) -> None:
         """Delete an item from the datastore."""
-        resp = requests.delete(urljoin(self.api_url, key), headers=self.auth)
+        resp = requests.delete(urljoin(self.api_url, key), headers=self._headers())
         if resp.status_code == HTTPStatus.NOT_FOUND:
             raise ValueError("Key does not exist.")
         elif not resp.ok:
             raise Exception(f"Server error {resp}")
 
     def list_all(self) -> Dict[str, Any]:
         """List all items in the datastore."""
-        resp = requests.get(self.api_url, headers=self.auth)
+        resp = requests.get(self.api_url, headers=self._headers())
         if not resp.ok:
             raise Exception(f"Server error {resp}")
         return dict((k, json.loads(bytes(v))) for k, v in resp.json().items())
```

### Comparing `bismuthsdk-0.1.8/src/bismuth/codeblocks/test_api_code_block.py` & `bismuthsdk-0.1.9/src/bismuth/codeblocks/test_api_code_block.py`

 * *Files identical despite different names*

### Comparing `bismuthsdk-0.1.8/src/bismuth/codeblocks/test_api_code_block_with_storage.py` & `bismuthsdk-0.1.9/src/bismuth/codeblocks/test_api_code_block_with_storage.py`

 * *Files identical despite different names*

### Comparing `bismuthsdk-0.1.8/src/bismuth/codeblocks/test_configuration_code_block.py` & `bismuthsdk-0.1.9/src/bismuth/codeblocks/test_configuration_code_block.py`

 * *Files identical despite different names*

### Comparing `bismuthsdk-0.1.8/src/bismuth/codeblocks/test_data_storage_block.py` & `bismuthsdk-0.1.9/src/bismuth/codeblocks/test_data_storage_block.py`

 * *Files identical despite different names*

### Comparing `bismuthsdk-0.1.8/src/bismuth/codeblocks/test_persistent_data_storage_block.py` & `bismuthsdk-0.1.9/src/bismuth/codeblocks/test_persistent_data_storage_block.py`

 * *Files identical despite different names*

### Comparing `bismuthsdk-0.1.8/pyproject.toml` & `bismuthsdk-0.1.9/pyproject.toml`

 * *Files identical despite different names*

