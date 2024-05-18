# Comparing `tmp/xplainable_client-1.2.2.tar.gz` & `tmp/xplainable_client-1.2.2.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xplainable_client-1.2.2.tar", last modified: Thu May 16 09:20:25 2024, max compression
+gzip compressed data, was "xplainable_client-1.2.2.post1.tar", last modified: Fri May 17 03:17:43 2024, max compression
```

## Comparing `xplainable_client-1.2.2.tar` & `xplainable_client-1.2.2.post1.tar`

### file list

```diff
@@ -1,33 +1,36 @@
-drwxr-xr-x   0 jtuppack   (501) staff       (20)        0 2024-05-16 09:20:25.807161 xplainable_client-1.2.2/
--rw-r--r--   0 jtuppack   (501) staff       (20)     4705 2024-05-16 09:20:25.806912 xplainable_client-1.2.2/PKG-INFO
--rw-r--r--   0 jtuppack   (501) staff       (20)     3924 2024-02-21 21:39:20.000000 xplainable_client-1.2.2/README.md
--rw-r--r--   0 jtuppack   (501) staff       (20)      855 2024-05-16 09:18:33.000000 xplainable_client-1.2.2/pyproject.toml
--rw-r--r--   0 jtuppack   (501) staff       (20)       38 2024-05-16 09:20:25.807206 xplainable_client-1.2.2/setup.cfg
-drwxr-xr-x   0 jtuppack   (501) staff       (20)        0 2024-05-16 09:20:25.799899 xplainable_client-1.2.2/xplainable_client/
-drwxr-xr-x   0 jtuppack   (501) staff       (20)        0 2024-05-16 09:20:25.803639 xplainable_client-1.2.2/xplainable_client/client/
--rw-r--r--   0 jtuppack   (501) staff       (20)     1082 2024-05-16 09:16:42.000000 xplainable_client-1.2.2/xplainable_client/client/__init__.py
--rw-r--r--   0 jtuppack   (501) staff       (20)      123 2024-05-16 09:16:42.000000 xplainable_client-1.2.2/xplainable_client/client/_client_cog_base.py
--rw-r--r--   0 jtuppack   (501) staff       (20)     7365 2024-05-16 09:16:42.000000 xplainable_client-1.2.2/xplainable_client/client/_collections.py
--rw-r--r--   0 jtuppack   (501) staff       (20)     1245 2024-05-16 09:16:42.000000 xplainable_client-1.2.2/xplainable_client/client/_datasets.py
--rw-r--r--   0 jtuppack   (501) staff       (20)    14645 2024-05-16 09:16:42.000000 xplainable_client-1.2.2/xplainable_client/client/_deployments.py
--rw-r--r--   0 jtuppack   (501) staff       (20)     1219 2024-05-16 09:16:42.000000 xplainable_client-1.2.2/xplainable_client/client/_gpt.py
--rw-r--r--   0 jtuppack   (501) staff       (20)     1234 2024-05-16 09:16:42.000000 xplainable_client-1.2.2/xplainable_client/client/_inference.py
--rw-r--r--   0 jtuppack   (501) staff       (20)     8313 2024-05-16 09:16:42.000000 xplainable_client-1.2.2/xplainable_client/client/_misc.py
--rw-r--r--   0 jtuppack   (501) staff       (20)    17210 2024-05-16 09:16:42.000000 xplainable_client-1.2.2/xplainable_client/client/_models.py
--rw-r--r--   0 jtuppack   (501) staff       (20)     9371 2024-05-16 09:16:42.000000 xplainable_client-1.2.2/xplainable_client/client/_preprocessing.py
--rw-r--r--   0 jtuppack   (501) staff       (20)     3919 2024-05-16 09:16:42.000000 xplainable_client-1.2.2/xplainable_client/client/_session.py
-drwxr-xr-x   0 jtuppack   (501) staff       (20)        0 2024-05-16 09:20:25.803970 xplainable_client-1.2.2/xplainable_client/models/
--rw-r--r--   0 jtuppack   (501) staff       (20)     4057 2024-03-04 22:40:48.000000 xplainable_client-1.2.2/xplainable_client/models/ebm.py
-drwxr-xr-x   0 jtuppack   (501) staff       (20)        0 2024-05-16 09:20:25.806211 xplainable_client-1.2.2/xplainable_client/utils/
--rw-r--r--   0 jtuppack   (501) staff       (20)        0 2024-02-12 08:30:29.000000 xplainable_client-1.2.2/xplainable_client/utils/__init__.py
--rw-r--r--   0 jtuppack   (501) staff       (20)     1291 2024-02-11 21:43:09.000000 xplainable_client-1.2.2/xplainable_client/utils/encoders.py
--rw-r--r--   0 jtuppack   (501) staff       (20)      180 2024-02-11 21:51:39.000000 xplainable_client-1.2.2/xplainable_client/utils/exceptions.py
--rw-r--r--   0 jtuppack   (501) staff       (20)      980 2024-02-11 21:45:45.000000 xplainable_client-1.2.2/xplainable_client/utils/helpers.py
--rw-r--r--   0 jtuppack   (501) staff       (20)     6426 2024-02-12 08:36:49.000000 xplainable_client-1.2.2/xplainable_client/utils/metrics.py
--rw-r--r--   0 jtuppack   (501) staff       (20)     3042 2024-02-11 21:51:47.000000 xplainable_client-1.2.2/xplainable_client/utils/model_parsers.py
-drwxr-xr-x   0 jtuppack   (501) staff       (20)        0 2024-05-16 09:20:25.806607 xplainable_client-1.2.2/xplainable_client.egg-info/
--rw-r--r--   0 jtuppack   (501) staff       (20)     4705 2024-05-16 09:20:25.000000 xplainable_client-1.2.2/xplainable_client.egg-info/PKG-INFO
--rw-r--r--   0 jtuppack   (501) staff       (20)      905 2024-05-16 09:20:25.000000 xplainable_client-1.2.2/xplainable_client.egg-info/SOURCES.txt
--rw-r--r--   0 jtuppack   (501) staff       (20)        1 2024-05-16 09:20:25.000000 xplainable_client-1.2.2/xplainable_client.egg-info/dependency_links.txt
--rw-r--r--   0 jtuppack   (501) staff       (20)      138 2024-05-16 09:20:25.000000 xplainable_client-1.2.2/xplainable_client.egg-info/requires.txt
--rw-r--r--   0 jtuppack   (501) staff       (20)       29 2024-05-16 09:20:25.000000 xplainable_client-1.2.2/xplainable_client.egg-info/top_level.txt
+drwxr-xr-x   0 jtuppack   (501) staff       (20)        0 2024-05-17 03:17:43.753728 xplainable_client-1.2.2.post1/
+-rw-r--r--   0 jtuppack   (501) staff       (20)     4703 2024-05-17 03:17:43.753497 xplainable_client-1.2.2.post1/PKG-INFO
+-rw-r--r--   0 jtuppack   (501) staff       (20)     3924 2024-02-21 21:39:20.000000 xplainable_client-1.2.2.post1/README.md
+-rw-r--r--   0 jtuppack   (501) staff       (20)      849 2024-05-17 03:17:17.000000 xplainable_client-1.2.2.post1/pyproject.toml
+-rw-r--r--   0 jtuppack   (501) staff       (20)       38 2024-05-17 03:17:43.753773 xplainable_client-1.2.2.post1/setup.cfg
+drwxr-xr-x   0 jtuppack   (501) staff       (20)        0 2024-05-17 03:17:43.746352 xplainable_client-1.2.2.post1/xplainable_client/
+drwxr-xr-x   0 jtuppack   (501) staff       (20)        0 2024-05-17 03:17:43.750822 xplainable_client-1.2.2.post1/xplainable_client/client/
+-rw-r--r--   0 jtuppack   (501) staff       (20)     1099 2024-05-17 03:09:19.000000 xplainable_client-1.2.2.post1/xplainable_client/client/__init__.py
+-rw-r--r--   0 jtuppack   (501) staff       (20)      123 2024-05-16 09:16:42.000000 xplainable_client-1.2.2.post1/xplainable_client/client/_client_cog_base.py
+-rw-r--r--   0 jtuppack   (501) staff       (20)     7352 2024-05-17 03:09:19.000000 xplainable_client-1.2.2.post1/xplainable_client/client/_collections.py
+-rw-r--r--   0 jtuppack   (501) staff       (20)     1245 2024-05-16 09:16:42.000000 xplainable_client-1.2.2.post1/xplainable_client/client/_datasets.py
+-rw-r--r--   0 jtuppack   (501) staff       (20)    14623 2024-05-17 03:09:19.000000 xplainable_client-1.2.2.post1/xplainable_client/client/_deployments.py
+-rw-r--r--   0 jtuppack   (501) staff       (20)     1218 2024-05-17 03:09:19.000000 xplainable_client-1.2.2.post1/xplainable_client/client/_gpt.py
+-rw-r--r--   0 jtuppack   (501) staff       (20)     1235 2024-05-17 03:09:19.000000 xplainable_client-1.2.2.post1/xplainable_client/client/_inference.py
+-rw-r--r--   0 jtuppack   (501) staff       (20)     8265 2024-05-17 03:09:19.000000 xplainable_client-1.2.2.post1/xplainable_client/client/_misc.py
+-rw-r--r--   0 jtuppack   (501) staff       (20)    17225 2024-05-17 03:09:19.000000 xplainable_client-1.2.2.post1/xplainable_client/client/_models.py
+-rw-r--r--   0 jtuppack   (501) staff       (20)     9344 2024-05-17 03:09:19.000000 xplainable_client-1.2.2.post1/xplainable_client/client/_preprocessing.py
+-rw-r--r--   0 jtuppack   (501) staff       (20)     4051 2024-05-17 03:09:19.000000 xplainable_client-1.2.2.post1/xplainable_client/client/_session.py
+drwxr-xr-x   0 jtuppack   (501) staff       (20)        0 2024-05-17 03:17:43.751002 xplainable_client-1.2.2.post1/xplainable_client/models/
+-rw-r--r--   0 jtuppack   (501) staff       (20)     4057 2024-03-04 22:40:48.000000 xplainable_client-1.2.2.post1/xplainable_client/models/ebm.py
+drwxr-xr-x   0 jtuppack   (501) staff       (20)        0 2024-05-17 03:17:43.751469 xplainable_client-1.2.2.post1/xplainable_client/tests/
+-rw-r--r--   0 jtuppack   (501) staff       (20)      270 2024-05-17 03:09:19.000000 xplainable_client-1.2.2.post1/xplainable_client/tests/test_model.py
+-rw-r--r--   0 jtuppack   (501) staff       (20)      184 2024-05-17 03:09:19.000000 xplainable_client-1.2.2.post1/xplainable_client/tests/test_test.py
+drwxr-xr-x   0 jtuppack   (501) staff       (20)        0 2024-05-17 03:17:43.752795 xplainable_client-1.2.2.post1/xplainable_client/utils/
+-rw-r--r--   0 jtuppack   (501) staff       (20)        0 2024-02-12 08:30:29.000000 xplainable_client-1.2.2.post1/xplainable_client/utils/__init__.py
+-rw-r--r--   0 jtuppack   (501) staff       (20)     1291 2024-02-11 21:43:09.000000 xplainable_client-1.2.2.post1/xplainable_client/utils/encoders.py
+-rw-r--r--   0 jtuppack   (501) staff       (20)      218 2024-05-17 03:09:19.000000 xplainable_client-1.2.2.post1/xplainable_client/utils/exceptions.py
+-rw-r--r--   0 jtuppack   (501) staff       (20)      980 2024-02-11 21:45:45.000000 xplainable_client-1.2.2.post1/xplainable_client/utils/helpers.py
+-rw-r--r--   0 jtuppack   (501) staff       (20)     6426 2024-02-12 08:36:49.000000 xplainable_client-1.2.2.post1/xplainable_client/utils/metrics.py
+-rw-r--r--   0 jtuppack   (501) staff       (20)     3042 2024-02-11 21:51:47.000000 xplainable_client-1.2.2.post1/xplainable_client/utils/model_parsers.py
+drwxr-xr-x   0 jtuppack   (501) staff       (20)        0 2024-05-17 03:17:43.753186 xplainable_client-1.2.2.post1/xplainable_client.egg-info/
+-rw-r--r--   0 jtuppack   (501) staff       (20)     4703 2024-05-17 03:17:43.000000 xplainable_client-1.2.2.post1/xplainable_client.egg-info/PKG-INFO
+-rw-r--r--   0 jtuppack   (501) staff       (20)      980 2024-05-17 03:17:43.000000 xplainable_client-1.2.2.post1/xplainable_client.egg-info/SOURCES.txt
+-rw-r--r--   0 jtuppack   (501) staff       (20)        1 2024-05-17 03:17:43.000000 xplainable_client-1.2.2.post1/xplainable_client.egg-info/dependency_links.txt
+-rw-r--r--   0 jtuppack   (501) staff       (20)      130 2024-05-17 03:17:43.000000 xplainable_client-1.2.2.post1/xplainable_client.egg-info/requires.txt
+-rw-r--r--   0 jtuppack   (501) staff       (20)       29 2024-05-17 03:17:43.000000 xplainable_client-1.2.2.post1/xplainable_client.egg-info/top_level.txt
```

### Comparing `xplainable_client-1.2.2/PKG-INFO` & `xplainable_client-1.2.2.post1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: xplainable-client
-Version: 1.2.2
+Version: 1.2.2.post1
 Summary: The client for persisting and deploying models to Xplainable cloud.
 Author-email: xplainable pty ltd <contact@xplainable.io>
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Requires-Dist: ipywidgets==8.0.6
-Requires-Dist: numpy>=1.20.3
-Requires-Dist: pandas<=1.9.0,>=1.5.2
+Requires-Dist: numpy==1.21.1
+Requires-Dist: pandas>=1.5.2
 Requires-Dist: pyperclip==1.8.2
 Requires-Dist: Requests==2.31.0
 Requires-Dist: scikit_learn
 Requires-Dist: setuptools
 Requires-Dist: urllib3==2.2.0
 Requires-Dist: xplainable
```

### Comparing `xplainable_client-1.2.2/README.md` & `xplainable_client-1.2.2.post1/README.md`

 * *Files identical despite different names*

### Comparing `xplainable_client-1.2.2/pyproject.toml` & `xplainable_client-1.2.2.post1/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "setuptools.build_meta"
 
 [tool.setuptools.packages]
 find = {} 
 
 [project]
 name = "xplainable-client"
-version = "1.2.2"
+version = "1.2.2-1"
 authors = [
   { name="xplainable pty ltd", email="contact@xplainable.io" },
 ]
 description = "The client for persisting and deploying models to Xplainable cloud."
 readme = "README.md"
 license = { file="LICENSE" }
 requires-python = ">=3.8"
@@ -22,16 +22,16 @@
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Operating System :: OS Independent"
 ]
 
 dependencies = [
 "ipywidgets==8.0.6",
-"numpy>=1.20.3",
-"pandas>=1.5.2,<=1.9.0",
+"numpy==1.21.1",
+"pandas>=1.5.2",
 "pyperclip==1.8.2",
 "Requests==2.31.0",
 "scikit_learn",
 "setuptools",
 "urllib3==2.2.0",
 "xplainable"
 ]
```

### Comparing `xplainable_client-1.2.2/xplainable_client/client/__init__.py` & `xplainable_client-1.2.2.post1/xplainable_client/client/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,25 +1,25 @@
-from .datasets import *
+from ._datasets import *
 from functools import cached_property
 
 from ._models import *
 from ._misc import *
-from requests.packages.urllib3.util.retry import Retry
+from urllib3.util.retry import Retry
 from ._session import Session
 from ._misc import Misc
 from ._models import Models
 from ._preprocessing import Preprocessing
 from ._deployments import Deployments
 from ._gpt import GPT
 from ._collections import Collections
 from ._datasets import Datasets
 from ._inference import Inference
 
 
-class Client(Misc, Models, Preprocessing, GPT, Collections):
+class Client(Misc, Models, Preprocessing, GPT, Collections, Datasets, Inference, Deployments):
 
     def __init__(self, api_key=None, hostname='https://api.xplainable.io', silent_mode=False):
         self.session = Session(api_key=api_key, hostname=hostname, silent_mode=silent_mode)
         Misc.__init__(self, self.session)
         Models.__init__(self, self.session)
         Preprocessing.__init__(self, self.session)
         Deployments.__init__(self, self.session)
```

### Comparing `xplainable_client-1.2.2/xplainable_client/client/_collections.py` & `xplainable_client-1.2.2.post1/xplainable_client/client/_collections.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,41 +15,41 @@
         """
         payload = {
             "name": name,
             "description": description
         }
         
         response = self.session._session.put(
-            url=f"{self.session.hostname}/v1/{self.session.__ext}/models/{model_id}/create-collection",
+            url=f"{self.session.hostname}/v1/{self.session._ext}/models/{model_id}/create-collection",
             json=payload
             )
         data = self.session.get_response_content(response)
         return data
     
     
     def get_model_collections(self, model_id: str):
         """ Gets all collections of a model.
         Args:
             model_id (str): The model id.
         Returns:
             dict: Dictionary of collections.
         """
         response = self.session._session.get(
-            url=f"{self.session.hostname}/v1/{self.session.__ext}/models/{model_id}/collections"
+            url=f"{self.session.hostname}/v1/{self.session._ext}/models/{model_id}/collections"
             )
         data = self.session.get_response_content(response)
         return data
     
     def get_team_collections(self):
         """ Gets all collections of a team.
         Returns:
             dict: Dictionary of collections.
         """
         response = self.session._session.get(
-            url=f"{self.session.hostname}/v1/{self.session.__ext}/collections"
+            url=f"{self.session.hostname}/v1/{self.session._ext}/collections"
             )
         data = self.session.get_response_content(response)
         return data
     
 
     def edit_collection_name(self, model_id: str, collections_id: str, name: str):
         """ Edits the name of a collection.
@@ -61,15 +61,15 @@
             json: A json payload.
         """
         payload = {
             "name": name
         }
 
         response = self.session._session.patch(
-            url=f"{self.session.hostname}/v1/{self.session.__ext}/models/{model_id}/collections/{collections_id}/name",
+            url=f"{self.session.hostname}/v1/{self.session._ext}/models/{model_id}/collections/{collections_id}/name",
             json=payload
             )
         return response
     
 
     def edit_collection_description(self, model_id: str, collections_id: str, description: str):
         """ Edits the description of a collection.
@@ -81,81 +81,81 @@
             json: A json payload.
         """
         payload = {
             "description": description
         }
 
         response = self.session._session.patch(
-            url=f"{self.session.hostname}/v1/{self.session.__ext}/models/{model_id}/collections/{collections_id}/description",
+            url=f"{self.session.hostname}/v1/{self.session._ext}/models/{model_id}/collections/{collections_id}/description",
             json=payload
             )
         return response
     
 
     def delete_collection(self, model_id: str, collections_id: str):
         """ Deletes a collection.
         Args:
             model_id (str): The model id.
             collections_id (str): The collection id.
         Returns:
             json: A json payload.
         """
         response = self.session._session.delete(
-            url=f"{self.session.hostname}/v1/{self.session.__ext}/models/{model_id}/collections/{collections_id}"
+            url=f"{self.session.hostname}/v1/{self.session._ext}/models/{model_id}/collections/{collections_id}"
             )
         return response
     
 
     def delete_model_collections(self, model_id: str):
         """ Deletes all collections of a model.
         Args:
             model_id (str): The model id.
         Returns:
             json: A json payload.
         """
         response = self.session._session.delete(
-            url=f"{self.session.hostname}/v1/{self.session.__ext}/models/{model_id}/collections"
+            url=f"{self.session.hostname}/v1/{self.session._ext}/models/{model_id}/collections"
             )
         return response
     
     
     def restore_collection(self, model_id: str, collection_id: str):
         """ Restores a collection.
         Args:
             model_id (str): The model id.
             collections_id (str): The collection id.
         Returns:
             json: A json payload.
         """
         response = self.session._session.patch(
-            url=f"{self.session.hostname}/v1/{self.session.__ext}/models/{model_id}/collections/{collection_id}/restore"
+            url=f"{self.session.hostname}/v1/{self.session._ext}/models/{model_id}/collections/{collection_id}/restore"
             )
         return response
     
 
     def get_collection(self, model_id: str, collection_id: str):
         """ Gets a collection.
         Args:
             model_id (str): The model id.
             collections_id (str): The collection id.
         Returns:
             dict: Dictionary of collection.
         """
         response = self.session._session.get(
-            url=f"{self.session.hostname}/v1/{self.session.__ext}/models/{model_id}/collections/{collection_id}"
+            url=f"{self.session.hostname}/v1/{self.session._ext}/models/{model_id}/collections/{collection_id}"
             )
         data = self.session.get_response_content(response)
         return data
     
 
     #TODO: Implement.
     # def add_scenario(self, model_id: str, version_id: str, collection_id: str):
     #     try:
     #         response = self.session._session.get(
-    #             url=f'{self.session.hostname}/v1/{self.session.__ext}/models/{model_id}/versions/{version_id}'
+    #             url=f'{self.session.hostname}/v1/{self.session._ext}/models/{model_id}/versions/{version_id}'
     #         )
     #         return self.session.get_response_content(response)
     #     except Exception as e:
     #         raise ValueError(f'Model with ID {model_id}:{version_id} does not exist')
     #     return
 
     # add_scenario
@@ -172,15 +172,15 @@
             json: A json payload.
         """
         payload = {
             "notes": notes
         }
 
         response = self.session._session.patch(
-            url=f"{self.session.hostname}/v1/{self.session.__ext}/models/{model_id}/collections/{collection_id}/scenarios/{scenario_id}/notes",
+            url=f"{self.session.hostname}/v1/{self.session._ext}/models/{model_id}/collections/{collection_id}/scenarios/{scenario_id}/notes",
             json=payload
             )
         return response
     
 
     def delete_scenario(self, model_id: str, collection_id: str, scenario_id: str):
         """" Deletes a scenario.
@@ -189,25 +189,25 @@
             collections_id (str): The collection id.
             scenario_id (str): The scenario id.
         Returns:
             json: A json payload.
         """
 
         response = self.session._session.delete(
-            url=f"{self.session.hostname}/v1/{self.session.__ext}/models/{model_id}/collections/{collection_id}/scenarios/{scenario_id}"
+            url=f"{self.session.hostname}/v1/{self.session._ext}/models/{model_id}/collections/{collection_id}/scenarios/{scenario_id}"
             )
         return response
     
 
     def restore_scenario(self, model_id: str, collection_id: str, scenario_id: str):
         """ Restores a scenario.
         Args:
             model_id (str): The model id.
             collections_id (str): The collection id.
             scenario_id (str): The scenario id.
         Returns:
             json: A json payload.
         """
         response = self.session._session.patch(
-            url=f"{self.session.hostname}/v1/{self.session.__ext}/models/{model_id}/collections/{collection_id}/scenarios/{scenario_id}/restore"
+            url=f"{self.session.hostname}/v1/{self.session._ext}/models/{model_id}/collections/{collection_id}/scenarios/{scenario_id}/restore"
             )
         return response
```

### Comparing `xplainable_client-1.2.2/xplainable_client/client/_datasets.py` & `xplainable_client-1.2.2.post1/xplainable_client/client/_datasets.py`

 * *Files identical despite different names*

### Comparing `xplainable_client-1.2.2/xplainable_client/client/_deployments.py` & `xplainable_client-1.2.2.post1/xplainable_client/client/_deployments.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
             partition_id (int): The partition id
             raw_output (bool, optional): returns a dictionary
         Returns:
             dict: deployment status and details.
         """
 
         url = (
-            f'{self.session.hostname}/v1/{self.session.__ext}/models/{model_id}/versions/'
+            f'{self.session.hostname}/v1/{self.session._ext}/models/{model_id}/versions/'
             f'{version_id}/deploy'
         )
         body = {
             "location": location
         }
         response = self.session._session.put(url, json=body)
 
@@ -48,15 +48,15 @@
 
     def list_deployments(self):
         """ Lists all deployments of the active user's team.
         Returns:
             dict: Dictionary of deployments.
         """
         response = self.session._session.get(
-            url=f'{self.session.hostname}/v1/{self.session.__ext}/deployments'
+            url=f'{self.session.hostname}/v1/{self.session._ext}/deployments'
             )
         deployments = self.session.get_response_content(response)
         return deployments
     
     
     def generate_deploy_key(
             self, description: str, deployment_id: str,
@@ -66,15 +66,15 @@
         Args:
             description (str): Description of the deploy key use case.
             deployment_id (str): The deployment id.
             days_until_expiry (float): The number of days until the key expires.
         Returns:
             str: The deploy key.
         """
-        url = f'{self.session.hostname}/v1/{self.session.__ext}/deployments/{deployment_id}/create-deploy-key'
+        url = f'{self.session.hostname}/v1/{self.session._ext}/deployments/{deployment_id}/create-deploy-key'
 
         params = {
             'description': description,
             'days_until_expiry': days_until_expiry
         }
 
         response = self.session._session.put(
@@ -91,15 +91,15 @@
     def list_deploy_keys(self, deployment_id: str):
         """ Lists all deploy keys for a deployment.
         Args:
             deployment_id (str): The deployment id.
         Returns:
             dict: Dictionary of deploy keys.
         """
-        url = f'{self.session.hostname}/v1/{self.session.__ext}/deployments/{deployment_id}/deploy-keys'
+        url = f'{self.session.hostname}/v1/{self.session._ext}/deployments/{deployment_id}/deploy-keys'
         response = self.session._session.get(url)
         deploy_keys = self.session.get_response_content(response)
         return deploy_keys
 
     def list_active_team_deploy_keys(self, team_id: str):
         """ Lists all active team deploy keys.
         Args:
@@ -116,94 +116,94 @@
         """ Revokes a deploy key for a deployment.
         Args:
             deployment_id (str): The deployment id.
             deploy_key_id (str): The deploy key id.
         Returns:
             dict: Dictionary of deploy keys.
         """
-        url = f'{self.session.hostname}/v1/{self.session.__ext}/deployments/{deployment_id}/revoke-deploy-key/{deploy_key_id}'
+        url = f'{self.session.hostname}/v1/{self.session._ext}/deployments/{deployment_id}/revoke-deploy-key/{deploy_key_id}'
         response = self.session._session.patch(url)
         return response.json()
 
     def delete_deployment(self, deployment_id: str):
         """ Deletes a model deployment.
         Args:
             deployment_id (str): The deployment id
         """
         url = (
-            f'{self.session.hostname}/v1/{self.session.__ext}/deployments/{deployment_id}'
+            f'{self.session.hostname}/v1/{self.session._ext}/deployments/{deployment_id}'
         )
         response = self.session._session.delete(url)
         return response.json()
     
 
     def add_allowed_ip_address(self, deployment_id: str):
         """ Add allowed ip address to a deployment.
         Args:
             deployment_id (str): The deployment id
         Return:
             json: The json response if the ip is added.
         """
         url = (
-            f'{self.session.hostname}/v1/{self.session.__ext}/deployments/{deployment_id}/add-allowed-ip'
+            f'{self.session.hostname}/v1/{self.session._ext}/deployments/{deployment_id}/add-allowed-ip'
 
         )
         response = self.session._session.put(url)
         return response.json()
 
     def list_allowed_ip_addresses(self, deployment_id: str):
         """ List allowed ip addresses for a deployment.
         Args:
             deployment_id (str): The deployment id
         Return:
             json: The json response of the allowed ip addresses.
         """
         url = (
-            f'{self.session.hostname}/v1/{self.session.__ext}/deployments/{deployment_id}/get-firewall'
+            f'{self.session.hostname}/v1/{self.session._ext}/deployments/{deployment_id}/get-firewall'
         )
         response = self.session._session.get(url)
         firewall = self.session.get_response_content(response)
         return firewall['allowed_ips']
 
     def list_allowed_ip_address_and_description(self, deployment_id: str):
         """ List allowed ip addresses and their descriptions for a deployment.
         Args:
             deployment_id (str): The deployment id
         Return:
             json: The json response of the allowed ip addresses and descriptions.
         """
         url = (
-            f'{self.session.hostname}/v1/{self.session.__ext}/deployments/{deployment_id}/get-firewall-descriptions'
+            f'{self.session.hostname}/v1/{self.session._ext}/deployments/{deployment_id}/get-firewall-descriptions'
         )
         response = self.session._session.get(url)
         firewall = self.session.get_response_content(response)
         return firewall
 
     def delete_allowed_ip_address(self, deployment_id: str, ip_id: str):
         """ Delete an allowed ip address from a deployment.
         Args:
             deployment_id (str): The deployment id
             ip_id (str): The ip id
         Return:
             json: The json response if the ip is deleted.
         """
         url = (
-            f'{self.session.hostname}/v1/{self.session.__ext}/deployments/{deployment_id}/ips/{ip_id}'
+            f'{self.session.hostname}/v1/{self.session._ext}/deployments/{deployment_id}/ips/{ip_id}'
         )
         response = self.session._session.delete(url)
         message = self.session.get_response_content(response)
         return message.get('message')
 
     def activate_deployment(self, deployment_id):
         """ Activates a model deployment.
         Args:
             deployment_id (str): The deployment id
         """
         url = (
-            f'{self.session.hostname}/v1/{self.session.__ext}/deployments/{deployment_id}/activate'
+            f'{self.session.hostname}/v1/{self.session._ext}/deployments/{deployment_id}/activate'
         )
         response = self.session._session.patch(url)
         if response.status_code == 200:
             return response.json()
         else:
             return {
                 "message": f"Failed with status code {response.status_code}"}
@@ -211,15 +211,15 @@
 
     def deactivate_deployment(self, deployment_id):
         """ Deactivates a model deployment.
         Args:
             deployment_id (str): The deployment id
         """
         url = (
-            f'{self.session.hostname}/v1/{self.session.__ext}/deployments/{deployment_id}/deactivate'
+            f'{self.session.hostname}/v1/{self.session._ext}/deployments/{deployment_id}/deactivate'
         )
         response = self.session._session.patch(url)
         if response.status_code == 200:
             return response.json()
         else:
             return {
                 "message": f"Failed with status code {response.status_code}"}
@@ -228,15 +228,15 @@
         """ Enables explain for a deployment.
         Args:
             deployment_id (str): The deployment id
         Return:
             str: The message if explain is enabled.
         """
         url = (
-            f'{self.session.hostname}/v1/{self.session.__ext}/deployments/{deployment_id}/enable-explain'
+            f'{self.session.hostname}/v1/{self.session._ext}/deployments/{deployment_id}/enable-explain'
         )
         response = self.session._session.patch(url)
         try:
             message = self.session.get_response_content(response)
             return message.get('message')
         except:
             return {"Explain for this deployment could not be enabled. Status code: ", response.status_code}
@@ -246,15 +246,15 @@
         """ Disables explain for a deployment.
         Args:
             deployment_id (str): The deployment id
         Return:
             str: The message if explain is disabled.
         """
         url = (
-            f'{self.session.hostname}/v1/{self.session.__ext}/deployments/{deployment_id}/disable-explain'
+            f'{self.session.hostname}/v1/{self.session._ext}/deployments/{deployment_id}/disable-explain'
         )
         response = self.session._session.patch(url)
         try:
             message = self.session.get_response_content(response)
             return message.get('message')
         except:
             return {"Explain for this deployment could not be disabled. Status code: ", response.status_code}
@@ -263,15 +263,15 @@
         """ Activates ip blocking for a deployment.
         Args:
             deployment_id (str): The deployment id
         Return:
             str: The message if ip blocking is activated.
         """
         url = (
-            f'{self.session.hostname}/v1/{self.session.__ext}/deployments/{deployment_id}/activate-deployment-ip-blocking'
+            f'{self.session.hostname}/v1/{self.session._ext}/deployments/{deployment_id}/activate-deployment-ip-blocking'
         )
         response = self.session._session.patch(url)
         try:
             message = self.session.get_response_content(response)
             return message.get('message')
         except:
             return {"Ip blocking for this deployment could not be activated. Status code: ", response.status_code}
@@ -280,15 +280,15 @@
         """ Deactivates ip blocking for a deployment.
         Args:
             deployment_id (str): The deployment id
         Return:
             str: The message if ip blocking is deactivated.
         """
         url = (
-            f'{self.session.hostname}/v1/{self.session.__ext}/deployments/{deployment_id}/deactivate-deployment-ip-blocking'
+            f'{self.session.hostname}/v1/{self.session._ext}/deployments/{deployment_id}/deactivate-deployment-ip-blocking'
         )
         response = self.session._session.patch(url)
         try:
             message = self.session.get_response_content(response)
             return message.get('message')
         except:
             return {"Ip blocking for this deployment could not be deactivated. Status code: ", response.status_code}
@@ -297,15 +297,15 @@
         """ Revokes all deploy keys for a deployment.
         Args:
             deployment_id (str): The deployment id
         Return:
             str: The message if all deploy keys are revoked.
         """
         url = (
-            f'{self.session.hostname}/v1/{self.session.__ext}/deployments/{deployment_id}/revoke-all-user-deploy-keys'
+            f'{self.session.hostname}/v1/{self.session._ext}/deployments/{deployment_id}/revoke-all-user-deploy-keys'
         )
         response = self.session._session.patch(url)
         try:
             message = self.session.get_response_content(response)
             return message.get('message')
         except:
             return {"All deploy keys for this deployment could not be revoked. Status code: ", response.status_code}
@@ -315,43 +315,43 @@
         Args:
             deployment_id (str): The deployment id
             key_id (str): The key id
         Return:
             str: The message if the key is deleted.
         """
         url = (
-            f'{self.session.hostname}/v1/{self.session.__ext}/deployments/{deployment_id}/deploy-keys/{key_id}'
+            f'{self.session.hostname}/v1/{self.session._ext}/deployments/{deployment_id}/deploy-keys/{key_id}'
         )
         response = self.session._session.delete(url)
         try:
             message = self.session.get_response_content(response)
             return message.get('message')
         except:
             return {"Deploy key could not be deleted. Status code: ", response.status_code}
 
 
     def generate_example_deployment_payload(self, deployment_id):
         """ Generates an example deployment payload for a deployment.
         Args:
             deployment_id (str): The deployment id.
         """
-        url = f'{self.session.hostname}/v1/{self.session.__ext}/deployments/{deployment_id}/payload'
+        url = f'{self.session.hostname}/v1/{self.session._ext}/deployments/{deployment_id}/payload'
         response = self.session._session.get(url)
         return response.json()
     
 
     def add_deployment_middleware(
         self, deployment_id, func, name, description=None):
         """ Adds or replaces a middleware function to a deployment.
         Args:
             deployment_id (str): The deployment id
             func (function): The middleware function
         """
         url = (
-            f'{self.session.hostname}/v1/{self.session.__ext}/deployments/{deployment_id}/add-middleware'
+            f'{self.session.hostname}/v1/{self.session._ext}/deployments/{deployment_id}/add-middleware'
         )
         # Convert function to expected name
         if func.__name__ != 'middleware':
             func = self.__parse_function(func)
             source_code = func.source
 
         else:
@@ -369,22 +369,22 @@
     
     def get_middleware(self, deployment_id):
         """ Gets the middleware function from a deployment.
         Args:
             deployment_id (str): The deployment id
         """
         url = (
-            f'{self.session.hostname}/v1/{self.session.__ext}/deployments/{deployment_id}/middleware'
+            f'{self.session.hostname}/v1/{self.session._ext}/deployments/{deployment_id}/middleware'
         )
         response = self.session._session.get(url)
         return self.session.get_response_content(response)
 
     def delete_deployment_middleware(self, deployment_id):
         """ Deletes a middleware function from a deployment.
         Args:
             deployment_id (str): The deployment id
         """
         url = (
-            f'{self.session.hostname}/v1/{self.session.__ext}/deployments/{deployment_id}/middleware'
+            f'{self.session.hostname}/v1/{self.session._ext}/deployments/{deployment_id}/middleware'
         )
         response = self.session._session.delete(url)
         return {"status_code": response.status_code}
```

### Comparing `xplainable_client-1.2.2/xplainable_client/client/_gpt.py` & `xplainable_client-1.2.2.post1/xplainable_client/client/_gpt.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
             max_features (int): The maximum number of features
             temperature (float): The temperature
         Return:
             dict: The report
         """
 
         url = (
-            f'{self.session.hostname}/v1/{self.session.__ext}/models/{model_id}/versions/'
+            f'{self.session.hostname}/v1/{self.session._ext}/models/{model_id}/versions/'
             f'{version_id}/generate-report'
         )
         params = {
             'target_description': target_description,
             'project_objective': project_objective,
             'max_features': max_features,
             'temperature': temperature
```

### Comparing `xplainable_client-1.2.2/xplainable_client/client/_inference.py` & `xplainable_client-1.2.2.post1/xplainable_client/client/_inference.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from _client_cog_base import *
+from ._client_cog_base import *
 
 class Inference(Client_Cog):
     
     def predict(self, filename: str, model_id: str, version_id: str, threshold: float = 0.5, delimiter: str = ","):
         """ Predicts the target column of a dataset.
         Args:
             filename (str): The name of the file.
```

### Comparing `xplainable_client-1.2.2/xplainable_client/client/_misc.py` & `xplainable_client-1.2.2.post1/xplainable_client/client/_misc.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,17 +12,17 @@
 from requests.adapters import HTTPAdapter
 
 from xplainable.preprocessing.pipeline import XPipeline
 from xplainable.preprocessing import transformers as xtf
 from xplainable.utils.model_parsers import *
 from xplainable.quality.scanner import XScan
 
-from xplainable_client.utils.exceptions import AuthenticationError
-from xplainable_client.utils.encoders import NpEncoder, force_json_compliant
-from xplainable_client.utils.metrics import evaluate_classification, evaluate_regression
+from ..utils.exceptions import AuthenticationError
+from ..utils.encoders import NpEncoder, force_json_compliant
+from ..utils.metrics import evaluate_classification, evaluate_regression
 
 import ipywidgets
 from ._client_cog_base import *
 
 
 class Misc(Client_Cog):
```

### Comparing `xplainable_client-1.2.2/xplainable_client/client/_models.py` & `xplainable_client-1.2.2.post1/xplainable_client/client/_models.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-from ._client_cog_base import *
+from ._client_cog_base import Client_Cog
 import pandas as pd
-from xplainable_client.utils.encoders import force_json_compliant
+from ..utils.encoders import force_json_compliant
 
 
 class Models(Client_Cog):
 
     def create_model(self, model_name: str, model_description: str, model, x: pd.DataFrame, y: pd.Series):
         """ Creates a new model if the model does not already exist.
 
@@ -46,18 +46,18 @@
             "model_description": model_description,
             "model_type": model_type,
             "target_name": target,
             "algorithm": model.__class__.__name__
         }
 
         response = self.session._session.post(
-            url=f'{self.session.hostname}/v1/{self.session.__ext}/create-model',
+            url=f'{self.session.hostname}/v1/{self.session._ext}/create-model',
             json=payoad
         )
-
+        print(response.content)
         model_id = self.session.get_response_content(response)
 
         return model_id
 
     
     #TODO: Refactor this based on notion instructions.
     def create_model_version(self, model, model_id: str, x: pd.DataFrame, y: pd.Series) -> str:
@@ -69,16 +69,16 @@
             health_info (dict): Feature health information
             versions (dict): Versions of current environment
         Returns:
             int: The model version id
         """
         # Get current versions
         versions = {
-                "xplainable_version": self.xplainable_version,
-                "python_version": self.python_version
+                "xplainable_version": self.session.xplainable_version,
+                "python_version": self.session.python_version
             }
         partition_on = model.partition_on if 'Partitioned' in \
             model.__class__.__name__ else None
         payload = {
             "partition_on": partition_on,
             "versions": versions,
             "partitions": []
@@ -98,30 +98,30 @@
                 payload['partitions'].append(pdata)
 
         elif model.__class__.__name__ in independent_models:
             pdata = self._get_partition_data(model, '__dataset__', x, y)
             payload['partitions'].append(pdata)
 
         # Create a new version and fetch id
-        url = f'{self.session.hostname}/v1/{self.session.__ext}/models/{model_id}/add-version'
+        url = f'{self.session.hostname}/v1/{self.session._ext}/models/{model_id}/add-version'
         response = self.session._session.post(
             url=url, json=force_json_compliant(payload))
         version_id = self.session.get_response_content(response)
         return version_id
         
 
     def list_models(self) -> list:
         """ Lists all models of the active user's team.
 
         Returns:
             dict: Dictionary of saved models.
         """
 
         response = self.session._session.get(
-            url=f'{self.session.hostname}/v1/{self.session.__ext}/models'
+            url=f'{self.session.hostname}/v1/{self.session._ext}/models'
             )
 
         data = self.session.get_response_content(response)
 
         # For better readability
         [i.pop('user') for i in data]
         [i.pop('contributors') for i in data]
@@ -140,15 +140,15 @@
             dict: The model information
 
         Raises:
             ValueError: If the model does not exist.
         """
         try:
             response = self.session._session.get(
-                url=f'{self.session.hostname}/v1/{self.session.__ext}/models/{model_id}/versions/{version_id}'
+                url=f'{self.session.hostname}/v1/{self.session._ext}/models/{model_id}/versions/{version_id}'
             )
             return self.session.get_response_content(response)
         except Exception as e:
             raise ValueError(f'Model with ID {model_id}:{version_id} does not exist')
 
     #TODO: Refactor this based on notion instructions.
     def _detect_model_type(self, model):
@@ -181,15 +181,15 @@
         """ Lists all versions of a model.
         Args:
             model_id (int): The model id
         Returns:
             dict: Dictionary of model versions.
         """
         response = self.session._session.get(
-            url=f'{self.session.hostname}/v1/{self.session.__ext}/models/{model_id}/versions'
+            url=f'{self.session.hostname}/v1/{self.session._ext}/models/{model_id}/versions'
             )
         data = self.session.get_response_content(response)
         [i.pop('user') for i in data]
         return data
     
     def list_model_version_partitions(self, model_id: str, version_id: str):
         """ Lists all partitions of a model version.
@@ -199,15 +199,15 @@
             version_id (str): The version id.
         
         Return:
             dict: Dictionary of model partitions.
 
         """
         response = self.session._session.get(
-            url=f'{self.session.hostname}/v1/{self.session.__ext}/models/{model_id}/versions/{version_id}'
+            url=f'{self.session.hostname}/v1/{self.session._ext}/models/{model_id}/versions/{version_id}'
         )
         partitions = self.session.get_response_content(response)
         return partitions
 
 
     def get_model_version_partition(self, model_id: str, version_id: str, partition_id: str):
         """ Gets a partition of a model version.
@@ -215,142 +215,142 @@
             model_id (str): The model id.
             version_id (str): The version id.
             partition_id (str): The partition id.
         Returns:
             json: A json payload.
         """
         response = self.session._session.get(
-            url=f'{self.session.hostname}/v1/{self.session.__ext}/models/{model_id}/versions/{version_id}/partitions/{partition_id}'
+            url=f'{self.session.hostname}/v1/{self.session._ext}/models/{model_id}/versions/{version_id}/partitions/{partition_id}'
         )
         partition_data = self.session.get_response_content(response)
         return partition_data
 
 
     def delete_model_version(self, model_id: str, version_id: str):
         """ Deletes a model version.
         Args:
             model_id (str): The model id.
             version_id (str): The version id.
         Return:
             json: A json payload.
         """
         response = self.session._session.delete(
-            url=f'{self.session.hostname}/v1/{self.session.__ext}/models/{model_id}/versions/{version_id}'
+            url=f'{self.session.hostname}/v1/{self.session._ext}/models/{model_id}/versions/{version_id}'
         )
         return response
 
     def restore_model_version(self, model_id: str, version_id: str):
         """ Restores a model version.
         Args:
             model_id (str): The model id.
             version_id (str): The version id.
         Return:
             json: A json payload.
         """
         response = self.session._session.post(
-            url=f'{self.session.hostname}/v1/{self.session.__ext}/models/{model_id}/versions/{version_id}/restore'
+            url=f'{self.session.hostname}/v1/{self.session._ext}/models/{model_id}/versions/{version_id}/restore'
         )
         return response
 
     def delete_model(self, model_id: str):
         """ Deletes an existing model.
         Args:
             model_id (str): The id of the model to be deleted.
         Return:
             json: A json payload
         """
         response = self.session._session.delete(
-            url=f'{self.session.hostname}/v1/{self.session.__ext}/models/{model_id}'
+            url=f'{self.session.hostname}/v1/{self.session._ext}/models/{model_id}'
         )
         return response
     
     def restore_deleted_model(self, model_id: str):
         """ Restores a deleted model.
         Args:
             model_id (str): The id of the model to be restored.
         Return:
             json: A json payload
         """
         response = self.session._session.patch(
-            url=f'{self.session.hostname}/v1/{self.session.__ext}/models/{model_id}/restore-deleted'
+            url=f'{self.session.hostname}/v1/{self.session._ext}/models/{model_id}/restore-deleted'
         )
         return response
 
     def activate_model(self, model_id: str):
         """ Activates a model.
         Args:
             model_id (str): The id of the model to be activated.
         Return:
             json: A json payload
         """
         response = self.session._session.patch(
-            url=f'{self.session.hostname}/v1/{self.session.__ext}/models/{model_id}/activate'
+            url=f'{self.session.hostname}/v1/{self.session._ext}/models/{model_id}/activate'
         )
         return response
 
     def deactivate_model(self, model_id: str):
         """ Deactivates a model.
         Args:
             model_id (str): The id of the model to be deactivated.
         Return:
             json: A json payload
         """
         response = self.session._session.patch(
-            url=f'{self.session.hostname}/v1/{self.session.__ext}/models/{model_id}/deactivate'
+            url=f'{self.session.hostname}/v1/{self.session._ext}/models/{model_id}/deactivate'
         )
         return response
 
     def archive_model(self, model_id: str):
         """ Archives a model.
         Args:
             model_id (str): The id of the model to be archived.
         Return:
             json: A json payload
         """
         response = self.session._session.patch(
-            url=f'{self.session.hostname}/v1/{self.session.__ext}/models/{model_id}/archive'
+            url=f'{self.session.hostname}/v1/{self.session._ext}/models/{model_id}/archive'
         )
         return response
 
     def restore_archived_model(self, model_id: str):
         """ Restores an archived model.
         Args:
             model_id (str): The id of the model to be restored.
         Return:
             json: A json payload
         """
         response = self.session._session.patch(
-            url=f'{self.session.hostname}/v1/{self.session.__ext}/models/{model_id}/restore-archived'
+            url=f'{self.session.hostname}/v1/{self.session._ext}/models/{model_id}/restore-archived'
         )
         return response
 
     def publish_model_version(self, model_id: str, version_id: str):
         """ Publishes a model version.
         Args:
             model_id (str): The model id.
             version_id (str): The version id.
         Return:
             json: A json payload.
         """
         response = self.session._session.post(
-            url=f'{self.session.hostname}/v1/{self.session.__ext}/models/{model_id}/versions/{version_id}/publish'
+            url=f'{self.session.hostname}/v1/{self.session._ext}/models/{model_id}/versions/{version_id}/publish'
         )
         return response
 
 
     def unpublish_model_version(self, model_id: str, version_id: str):
         """ Unpublishes a model version.
         Args:
             model_id (str): The model id.
             version_id (str): The version id.
         Return:
             json: A json payload.
         """
         response = self.session._session.post(
-            url=f'{self.session.hostname}/v1/{self.session.__ext}/models/{model_id}/versions/{version_id}/unpublish'
+            url=f'{self.session.hostname}/v1/{self.session._ext}/models/{model_id}/versions/{version_id}/unpublish'
         )
         return response
 
     def update_model_description(self, model_id: str, description: str):
         """ Updates the description of a model.
         Args:
             model_id (str): The model id.
@@ -359,15 +359,15 @@
             json: A json payload.
         """
         payload = {
             "description": description
         }
 
         response = self.session._session.patch(
-            url=f'{self.session.hostname}/v1/{self.session.__ext}/models/{model_id}/description',
+            url=f'{self.session.hostname}/v1/{self.session._ext}/models/{model_id}/description',
             json=payload
         )
         return response
 
     def update_model_name(self, model_id: str, name: str):
         """ Updates the name of a model.
         Args:
@@ -377,44 +377,44 @@
             json: A json payload.
         """
         payload = {
             "name": name
         }
 
         response = self.session._session.patch(
-            url=f'{self.session.hostname}/v1/{self.session.__ext}/models/{model_id}/name',
+            url=f'{self.session.hostname}/v1/{self.session._ext}/models/{model_id}/name',
             json=payload
         )
         return response
 
     def get_model_profile(self, model_id: str, version_id: str):
         """ Gets the profile of a model.
         Args:
             model_id (str): The model id.
             version_id (str): The version id.
         Return:
             list: A list of model profiles.
         """
         response = self.session._session.get(
-            url=f'{self.session.hostname}/v1/{self.session.__ext}/models/{model_id}/versions/{version_id}/profile'
+            url=f'{self.session.hostname}/v1/{self.session._ext}/models/{model_id}/versions/{version_id}/profile'
         )
         profile = self.session.get_response_content(response)
         return profile
 
     def get_model_evaluation_data(self, model_id: str, version_id: str, partition_id: str):
         """ Gets the evaluation data of a model.
         Args:
             model_id (str): The model id.
             version_id (str): The version id.
             partition_id (str): The partition id.
         Return:
             dict: A dictionary of model evaluation data.
         """
         response = self.session._session.get(
-            url=f'{self.session.hostname}/v1/{self.session.__ext}/models/{model_id}/versions/{version_id}/partitions/{partition_id}/evaluation'
+            url=f'{self.session.hostname}/v1/{self.session._ext}/models/{model_id}/versions/{version_id}/partitions/{partition_id}/evaluation'
         )
         evaluation_data = self.session.get_response_content(response)
         return evaluation_data
 
     def link_model_preprocessor(self, model_id: str, version_id: str, preprocessor_id: str, preprocessor_version_id: str):
         """ Links a model to a preprocessor.
         Args:
@@ -428,29 +428,29 @@
         payload = {
             "preprocessor_id": preprocessor_id,
             "preprocessor_version_id": preprocessor_version_id
 
         }
 
         response = self.session._session.put(
-            url=f'{self.session.hostname}/v1/{self.session.__ext}/models/{model_id}/versions/{version_id}/preprocessor',
+            url=f'{self.session.hostname}/v1/{self.session._ext}/models/{model_id}/versions/{version_id}/preprocessor',
             json=payload
         )
         return response
 
     def get_model_preprocessor(self, model_id: str, version_id: str):
         """ Gets the preprocessor of a model.
         Args:
             model_id (str): The model id.
             version_id (str): The version id.
         Return:
             dict: A dictionary of model preprocessor.
         """
         response = self.session._session.get(
-            url=f'{self.session.hostname}/v1/{self.session.__ext}/models/{model_id}/versions/{version_id}/preprocessor'
+            url=f'{self.session.hostname}/v1/{self.session._ext}/models/{model_id}/versions/{version_id}/preprocessor'
         )
         preprocessor = self.session.get_response_content(response)
         return preprocessor
 
     def set_active_version(self, model_id: str, version_id: str):
         """ Sets the active version of a model.
         Args:
@@ -460,15 +460,15 @@
             json: A json payload.
         """
         payload = {
             "version_id": version_id
         }
 
         response = self.session._session.patch(
-            url=f'{self.session.hostname}/v1/{self.session.__ext}/models/{model_id}/active-version',
+            url=f'{self.session.hostname}/v1/{self.session._ext}/models/{model_id}/active-version',
             json=payload
         )
         return response
 
     def move_model(self, model_id: str, new_team_id: str):
         """ Moves a model to a new team.
         Args:
@@ -478,15 +478,15 @@
             json: A json payload.
         """
         payload = {
             "new_team_id": new_team_id
         }
 
         response = self.session._session.patch(
-            url=f'{self.session.hostname}/v1/{self.session.__ext}/models/{model_id}/move',
+            url=f'{self.session.hostname}/v1/{self.session._ext}/models/{model_id}/move',
             json=payload
         )
         return response
```

### Comparing `xplainable_client-1.2.2/xplainable_client/client/_preprocessing.py` & `xplainable_client-1.2.2.post1/xplainable_client/client/_preprocessing.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from ._client_cog_base import *
 import pandas as pd
 import json
-from xplainable_client.utils.helpers import get_df_delta
+from ..utils.helpers import get_df_delta
 from xplainable.preprocessing.pipeline import XPipeline
 
 
 class Preprocessing(Client_Cog):
 
     def create_preprocessor_id(
         self, preprocessor_name: str, preprocessor_description: str) -> str:
@@ -17,15 +17,15 @@
             int: The preprocessor id
         """
         payoad = {
             "preprocessor_name": preprocessor_name,
             "preprocessor_description": preprocessor_description
         }
         response = self.session._session.post(
-            url=f'{self.session.hostname}/v1/{self.session.__ext}/create-preprocessor',
+            url=f'{self.session.hostname}/v1/{self.session._ext}/create-preprocessor',
             json=payoad
         )
 
         preprocessor_id = self.session.get_response_content(response)
 
         return preprocessor_id
     
@@ -70,29 +70,29 @@
             "stages": stages,
             "deltas": deltas,
             "versions": versions
             }
 
         # Create a new version and fetch id
         url = (
-            f'{self.session.hostname}/v1/{self.session.__ext}/preprocessors/'
+            f'{self.session.hostname}/v1/{self.session._ext}/preprocessors/'
             f'{preprocessor_id}/add-version'
             )
 
         response = self.session._session.post(url=url, json=payload)
         version_id = self.session.get_response_content(response)
         return version_id
 
     def list_preprocessors(self) -> list:
         """ Lists all preprocessors of the active user's team.
         Returns:
             dict: Dictionary of preprocessors.
         """
         response = self.session._session.get(
-            url=f'{self.session.hostname}/v1/{self.session.__ext}/preprocessors'
+            url=f'{self.session.hostname}/v1/{self.session._ext}/preprocessors'
             )
         data = self.session.get_response_content(response)
         [i.pop('user') for i in data]
         return data
     
     # get_preprocessor
     
@@ -102,15 +102,15 @@
         """ Lists all versions of a preprocessor.
         Args:
             preprocessor_id (int): The preprocessor id
         Returns:
             dict: Dictionary of preprocessor versions.
         """
         response = self.session._session.get(
-            url=f'{self.session.hostname}/v1/{self.session.__ext}/preprocessors/{preprocessor_id}/versions'
+            url=f'{self.session.hostname}/v1/{self.session._ext}/preprocessors/{preprocessor_id}/versions'
             )
 
         data = self.session.get_response_content(response)
         [i.pop('user') for i in data]
         return data
 
     def load_preprocessor(
@@ -130,15 +130,15 @@
                 raise ValueError(f"{stage['name']} does not exist in the transformers module")
             # Get transformer function
             func = getattr(xtf, stage["name"])
             return func(**stage['params'])
 
         try:
             preprocessor_response = self.session._session.get(
-                url=f'{self.session.hostname}/v1/{self.session.__ext}/preprocessors/{preprocessor_id}/versions/{version_id}'
+                url=f'{self.session.hostname}/v1/{self.session._ext}/preprocessors/{preprocessor_id}/versions/{version_id}'
                 )
             response = self.session.get_response_content(preprocessor_response)
             if response_only:
                 return response
         except Exception as e:
             raise ValueError(
             f'Preprocessor with ID {preprocessor_id}:{version_id} does not exist')
@@ -165,66 +165,66 @@
         Args:
             preprocessor_id (int): The preprocessor id
             version_id (int): The version id
         Returns:
             xplainable.preprocessing.pipeline.Pipeline: The pipeline
         """
         response = self.session._session.get(
-            url=f'{self.session.hostname}/v1/{self.session.__ext}/preprocessors/{preprocessor_id}/versions/{version_id}/pipeline'
+            url=f'{self.session.hostname}/v1/{self.session._ext}/preprocessors/{preprocessor_id}/versions/{version_id}/pipeline'
             )
         data = self.session.get_response_content(response)
         return data
 
     def delete_preprocessor_version(self, preprocessor_id: str, version_id: str):
         """ Deletes a preprocessor version.
         Args:
             preprocessor_id (int): The preprocessor id
             version_id (int): The version id
         Return:
             json: A json response
         """
         response = self.session._session.delete(
-            url=f'{self.session.hostname}/v1/{self.session.__ext}/preprocessors/{preprocessor_id}/versions/{version_id}'
+            url=f'{self.session.hostname}/v1/{self.session._ext}/preprocessors/{preprocessor_id}/versions/{version_id}'
             )
         return response
 
     def restore_preprocessor_version(self, preprocessor_id: str, version_id: str):
         """ Restores a preprocessor version.
         Args:
             preprocessor_id (int): The preprocessor id
             version_id (int): The version id
         Return:
             json: A json response. 
         """
         response = self.session._session.put(
-            url=f'{self.session.hostname}/v1/{self.session.__ext}/preprocessors/{preprocessor_id}/versions/{version_id}/restore'
+            url=f'{self.session.hostname}/v1/{self.session._ext}/preprocessors/{preprocessor_id}/versions/{version_id}/restore'
             )
         return response
 
     def delete_preprocessor(self, preprocessor_id: str):
         """ Deletes a preprocessor.
         Args:
             preprocessor_id (int): The preprocessor id
         Return:
             json: A json response
         """
         response = self.session._session.delete(
-            url=f'{self.session.hostname}/v1/{self.session.__ext}/preprocessors/{preprocessor_id}'
+            url=f'{self.session.hostname}/v1/{self.session._ext}/preprocessors/{preprocessor_id}'
             )
         return response
 
     def restore_preprocessor(self, preprocessor_id: str):
         """ Restores a preprocessor.
         Args:
             preprocessor_id (int): The preprocessor id
         Return:
             json: A json response
         """
         response = self.session._session.post(
-            url=f'{self.session.hostname}/v1/{self.session.__ext}/preprocessors/{preprocessor_id}/restore'
+            url=f'{self.session.hostname}/v1/{self.session._ext}/preprocessors/{preprocessor_id}/restore'
             )
         return response
 
     def check_signature(self, preprocessor_id: str, preprocessor_version_id: str, model_id: str, model_version_id: str):
         """ Checks the signature of a preprocessor version.
         Args:
             preprocessor_id (int): The preprocessor id
@@ -236,15 +236,15 @@
         """
         
         payload = {
             'model_id': model_id,
             'version_id': model_version_id
         }
         response = self.session._session.post(
-            url=f'{self.session.hostname}/v1/{self.session.__ext}/preprocessors/{preprocessor_id}/versions/{preprocessor_version_id}/check-signature',
+            url=f'{self.session.hostname}/v1/{self.session._ext}/preprocessors/{preprocessor_id}/versions/{preprocessor_version_id}/check-signature',
             json=payload
         )
         output = self.session.get_response_content(response)
         return output
```

### Comparing `xplainable_client-1.2.2/xplainable_client/client/_session.py` & `xplainable_client-1.2.2.post1/xplainable_client/client/_session.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,19 @@
-from .datasets import *
+from ._datasets import *
+from ..utils.exceptions import *
 from functools import cached_property
+import xplainable
+import json
+from requests.adapters import HTTPAdapter
+import ipywidgets
+import sys
+from IPython.display import display
 
-from ._models import *
-from ._misc import *
-from requests.packages.urllib3.util.retry import Retry
+from urllib3.util import Retry
+import requests
 
 
 class Session:
     """ A client for interfacing with the xplainable web api (xplainable cloud).
 
     Access models, preprocessors and user data from xplainable cloud. API keys
     can be generated at https://beta.xplainable.io.
@@ -20,31 +26,32 @@
         if not api_key:
             raise ValueError('A valid API Key is required. Generate one from the xplainable app.')
 
         self.api_key = api_key
         self.hostname = hostname
         self._setup_session()  # Set up the session and other initialization steps
 
-        self.__ext = f"organisations/{self.user_data['organisation_id']}/teams/{self.user_data['team_id']}"
+
+        self._ext = f"organisations/{self.user_data['organisation_id']}/teams/{self.user_data['team_id']}"
 
         # You can still use the _render_init_table here if you want to display it,
         # or you can return the data dict for a more script-friendly approach.
         data = self._gather_initialization_data()
         if not silent_mode:
             self._render_init_table(data)
 
     @cached_property
     def user_data(self):
         """ Retrieves the user data for the active user.
         Returns:
             dict: User data
         """
-
         response = self._session.get(
-            url=f'{self.hostname}/v1/client-connect'
+            url=f'{self.hostname}/v1/client-connect',
+            
         )
         if response.status_code == 200:
             return self.get_response_content(response)
 
         else:
             raise AuthenticationError(
                 f"{response.status_code} Unauthenticated. "
```

### Comparing `xplainable_client-1.2.2/xplainable_client/models/ebm.py` & `xplainable_client-1.2.2.post1/xplainable_client/models/ebm.py`

 * *Files identical despite different names*

### Comparing `xplainable_client-1.2.2/xplainable_client/utils/encoders.py` & `xplainable_client-1.2.2.post1/xplainable_client/utils/encoders.py`

 * *Files identical despite different names*

### Comparing `xplainable_client-1.2.2/xplainable_client/utils/helpers.py` & `xplainable_client-1.2.2.post1/xplainable_client/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `xplainable_client-1.2.2/xplainable_client/utils/metrics.py` & `xplainable_client-1.2.2.post1/xplainable_client/utils/metrics.py`

 * *Files identical despite different names*

### Comparing `xplainable_client-1.2.2/xplainable_client/utils/model_parsers.py` & `xplainable_client-1.2.2.post1/xplainable_client/utils/model_parsers.py`

 * *Files identical despite different names*

### Comparing `xplainable_client-1.2.2/xplainable_client.egg-info/PKG-INFO` & `xplainable_client-1.2.2.post1/xplainable_client.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: xplainable-client
-Version: 1.2.2
+Version: 1.2.2.post1
 Summary: The client for persisting and deploying models to Xplainable cloud.
 Author-email: xplainable pty ltd <contact@xplainable.io>
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Requires-Dist: ipywidgets==8.0.6
-Requires-Dist: numpy>=1.20.3
-Requires-Dist: pandas<=1.9.0,>=1.5.2
+Requires-Dist: numpy==1.21.1
+Requires-Dist: pandas>=1.5.2
 Requires-Dist: pyperclip==1.8.2
 Requires-Dist: Requests==2.31.0
 Requires-Dist: scikit_learn
 Requires-Dist: setuptools
 Requires-Dist: urllib3==2.2.0
 Requires-Dist: xplainable
```

### Comparing `xplainable_client-1.2.2/xplainable_client.egg-info/SOURCES.txt` & `xplainable_client-1.2.2.post1/xplainable_client.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -13,13 +13,15 @@
 xplainable_client/client/_gpt.py
 xplainable_client/client/_inference.py
 xplainable_client/client/_misc.py
 xplainable_client/client/_models.py
 xplainable_client/client/_preprocessing.py
 xplainable_client/client/_session.py
 xplainable_client/models/ebm.py
+xplainable_client/tests/test_model.py
+xplainable_client/tests/test_test.py
 xplainable_client/utils/__init__.py
 xplainable_client/utils/encoders.py
 xplainable_client/utils/exceptions.py
 xplainable_client/utils/helpers.py
 xplainable_client/utils/metrics.py
 xplainable_client/utils/model_parsers.py
```

