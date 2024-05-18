# Comparing `tmp/qdrant_txtai-1.0.1.tar.gz` & `tmp/qdrant_txtai-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qdrant_txtai-1.0.1.tar", max compression
+gzip compressed data, was "qdrant_txtai-2.0.0.tar", max compression
```

## Comparing `qdrant_txtai-1.0.1.tar` & `qdrant_txtai-2.0.0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0    11357 2023-04-12 11:25:58.610895 qdrant_txtai-1.0.1/LICENSE
--rw-r--r--   0        0        0     4044 2023-04-12 11:25:58.610895 qdrant_txtai-1.0.1/README.md
--rw-r--r--   0        0        0      676 2023-04-12 11:25:58.614895 qdrant_txtai-1.0.1/pyproject.toml
--rw-r--r--   0        0        0        0 2023-04-12 11:25:58.614895 qdrant_txtai-1.0.1/src/qdrant_txtai/__init__.py
--rw-r--r--   0        0        0        0 2023-04-12 11:25:58.614895 qdrant_txtai-1.0.1/src/qdrant_txtai/ann/__init__.py
--rw-r--r--   0        0        0     4721 2023-04-12 11:25:58.614895 qdrant_txtai-1.0.1/src/qdrant_txtai/ann/qdrant.py
--rw-r--r--   0        0        0     4764 1970-01-01 00:00:00.000000 qdrant_txtai-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-05-18 09:22:16.576105 qdrant_txtai-2.0.0/LICENSE
+-rw-r--r--   0        0        0     3988 2024-05-18 09:22:16.576105 qdrant_txtai-2.0.0/README.md
+-rw-r--r--   0        0        0      677 2024-05-18 09:22:16.580105 qdrant_txtai-2.0.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-18 09:22:16.580105 qdrant_txtai-2.0.0/src/qdrant_txtai/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-18 09:22:16.580105 qdrant_txtai-2.0.0/src/qdrant_txtai/ann/__init__.py
+-rw-r--r--   0        0        0     4229 2024-05-18 09:22:16.580105 qdrant_txtai-2.0.0/src/qdrant_txtai/ann/qdrant.py
+-rw-r--r--   0        0        0     4702 1970-01-01 00:00:00.000000 qdrant_txtai-2.0.0/PKG-INFO
```

### Comparing `qdrant_txtai-1.0.1/LICENSE` & `qdrant_txtai-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `qdrant_txtai-1.0.1/README.md` & `qdrant_txtai-2.0.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 # qdrant-txtai
 
 [txtai](https://github.com/neuml/txtai) simplifies building AI-powered semantic 
 search applications using Transformers. It leverages the neural embeddings and
 their properties to encode high-dimensional data in a lower-dimensional space 
 and allows to find similar objects based on their embeddings' proximity. 
 
-Implementing such application in real-world use cases requires storing the
-embeddings in an efficient way though, namely in a vector database like 
+Implementing such applications in real-world use cases requires storing the
+embeddings efficiently, namely in a vector database like 
 [Qdrant](https://qdrant.tech). It offers not only a powerful engine for neural
 search, but also allows setting up a whole cluster if your data does not fit
-a single machine anymore. It is production grade and can be launched easily
+a single machine anymore. It is production-grade and can be launched easily
 with Docker.
 
 Combining the easiness of txtai with Qdrant's performance enables you to build
 production-ready semantic search applications way faster than before.
 
 ## Installation
 
@@ -21,19 +21,19 @@
 
 ```bash
 pip install qdrant-txtai
 ```
 
 ## Usage
 
-Running the txtai application with Qdrant as a vector storage requires launching
+Running the txtai application with Qdrant as vector storage requires launching
 a Qdrant instance. That might be done easily with Docker:
 
 ```bash
-docker run -p 6333:6333 -p:6334:6334 qdrant/qdrant:v1.0.1
+docker run -p 6333:6333 -p:6334:6334 qdrant/qdrant:latest
 ```
 
 Running the txtai application might be done either programmatically or by 
 providing configuration in a YAML file.
 
 ### Programmatically
 
@@ -61,72 +61,69 @@
 ```bash
 CONFIG=app.yml uvicorn "txtai.api:app"
 curl -X GET "http://localhost:8000/search?query=positive"
 ```
 
 ## Configuration properties
 
-*qdrant-txtai* allows you to configure both the connection details, and some 
-internal properties of the vector collection which may impact both speed and
+*qdrant-txtai* allows you to configure both the connection details and some 
+internal properties of the vector collection, which may impact both speed and
 accuracy. Please refer to [Qdrant docs](https://qdrant.github.io/qdrant/redoc/index.html#tag/collections/operation/create_collection)
 if you are interested in the meaning of each property.
 
 The example below presents all the available options, if we connect to Qdrant server:
 
 ```yaml
 embeddings:
   path: sentence-transformers/all-MiniLM-L6-v2
   backend: qdrant_txtai.ann.qdrant.Qdrant
-  metric: l2 # allowed values: l2 / cosine / ip
+  metric: l2 # allowed values: l1 / l2 / cosine / ip
   qdrant:
     url: qdrant.host
     port: 6333
     grpc_port: 6334
     prefer_grpc: true
     collection: CustomCollectionName
     https: true # for Qdrant Cloud
     api_key: XYZ # for Qdrant Cloud
-    hnsw:
-      m: 8
-      ef_construct: 256
-      full_scan_threshold:
-      ef_search: 512
+    search_params:
+      hnsw_ef: 100
 ```
 
 ### Local in-memory/disk-persisted mode
 
 Qdrant Python client, from version 1.1.1, supports local in-memory/disk-persisted mode. 
 That's a good choice for any test scenarios and quick experiments in which you do not 
-plan to store lots of vectors. In such a case spinning a Docker container might be even 
+plan to store lots of vectors. In such a case, spinning a Docker container might be even
 not required.
 
 #### In-memory storage
 
-In case you want to have a transient storage, for example in case of automated tests 
+In case you want to have transient storage, for example, in the case of automated tests 
 launched during your CI/CD pipeline, using Qdrant Local mode with in-memory storage 
 might be a preferred option.
 
 ```yaml
 embeddings:
   path: sentence-transformers/all-MiniLM-L6-v2
   backend: qdrant_txtai.ann.qdrant.Qdrant
-  metric: l2 # allowed values: l2 / cosine / ip
+  metric: l2 # allowed values: l1 / l2 / cosine / ip
   qdrant:
     location: ':memory:'
     prefer_grpc: true
 ```
 
 #### On disk storage
 
 However, if you prefer to keep the vectors between different runs of your application, 
-it might be better to use on disk storage and pass the path that should be used to 
+it might be better to use disk storage and pass the path that should be used to 
 persist the data.
 
 ```yaml
 embeddings:
   path: sentence-transformers/all-MiniLM-L6-v2
   backend: qdrant_txtai.ann.qdrant.Qdrant
-  metric: l2 # allowed values: l2 / cosine / ip
+  metric: l2 # allowed values: l1 / l2 / cosine / ip
   qdrant:
     path: '/home/qdrant/storage_local'
     prefer_grpc: true
 ```
```

### Comparing `qdrant_txtai-1.0.1/src/qdrant_txtai/ann/qdrant.py` & `qdrant_txtai-2.0.0/src/qdrant_txtai/ann/qdrant.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,97 +1,75 @@
 import warnings
+from txtai.ann import ANN
 
 from grpc import RpcError
 from qdrant_client import QdrantClient
 from qdrant_client.http.exceptions import UnexpectedResponse
 from qdrant_client.http.models import (
-    PointIdsList,
-    VectorParams,
-    Distance,
-    HnswConfigDiff,
-    SearchRequest,
-    SearchParams,
-)
-from txtai.ann import ANN
+        PointIdsList,
+        VectorParams,
+        Distance,
+        SearchRequest,
+        SearchParams,
+    )
+
 
 
 class Qdrant(ANN):
     """
-    ANN implementation using Qdrant server as a backend.
+    ANN implementation using Qdrant - https://qdrant.tech as a backend.
     """
 
-    DISTANCE = {
+    DISTANCE_MAPPING = {
         "cosine": Distance.COSINE,
         "l2": Distance.EUCLID,
         "ip": Distance.DOT,
+        "l1": Distance.MANHATTAN,
     }
 
     def __init__(self, config):
         super().__init__(config)
 
-        # Load Qdrant specific configuration from the nested configuration dict
         self.qdrant_config = self.config.get("qdrant", {})
-        location = self.qdrant_config.get("location")
-        url = self.qdrant_config.get("url")
-        port = self.qdrant_config.get("port", 6333)
-        grpc_port = self.qdrant_config.get("grpc_port", 6334)
-        prefer_grpc = self.qdrant_config.get("prefer_grpc", False)
-        https = self.qdrant_config.get("https")
-        api_key = self.qdrant_config.get("api_key")
-        prefix = self.qdrant_config.get("prefix")
-        timeout = self.qdrant_config.get("timeout")
-        host = self.qdrant_config.get("host")
-        path = self.qdrant_config.get("path")
+        self.collection_name = self.qdrant_config.get("collection", "txtai-embeddings")
         self.qdrant_client = QdrantClient(
-            location=location,
-            url=url,
-            port=port,
-            grpc_port=grpc_port,
-            prefer_grpc=prefer_grpc,
-            https=https,
-            api_key=api_key,
-            prefix=prefix,
-            timeout=timeout,
-            host=host,
-            path=path,
+            location=self.qdrant_config.get("location"),
+            url=self.qdrant_config.get("url"),
+            port=self.qdrant_config.get("port", 6333),
+            grpc_port=self.qdrant_config.get("grpc_port", 6334),
+            prefer_grpc=self.qdrant_config.get("prefer_grpc", False),
+            https=self.qdrant_config.get("https"),
+            api_key=self.qdrant_config.get("api_key"),
+            prefix=self.qdrant_config.get("prefix"),
+            timeout=self.qdrant_config.get("timeout"),
+            host=self.qdrant_config.get("host"),
+            path=self.qdrant_config.get("path"),
+            grpc_options=self.qdrant_config.get("grpc_options"),
         )
-        self.collection_name = self.qdrant_config.get("collection", "embeddings")
 
         # Initial offset is set to the number of existing rows
         try:
             self.config["offset"] = self.count()
         except (UnexpectedResponse, RpcError, ValueError):
             self.config["offset"] = 0
 
-    def load(self, path):
-        # Since Qdrant does not rely on files, there is no need to load anything
-        # from given path. Instead, the file path is used as a collection name,
-        # effectively allowing to use different embeddings.
-        warnings.warn(
-            "Trying to call .load method on Qdrant ANN backend. "
-            "It won't have any effect.",
-            UserWarning,
-        )
-
     def index(self, embeddings):
         vector_size = self.config.get("dimensions")
         metric_name = self.config.get("metric", "cosine")
-        hnsw_config = self.qdrant_config.get("hnsw", {})
+        if metric_name not in self.DISTANCE_MAPPING:
+            raise ValueError(f"Unsupported Qdrant similarity metric: {metric_name}")
+        collection_config = self.qdrant_config.get("collection_config", {})
 
         self.qdrant_client.recreate_collection(
             collection_name=self.collection_name,
             vectors_config=VectorParams(
                 size=vector_size,
-                distance=self.DISTANCE[metric_name],
-            ),
-            hnsw_config=HnswConfigDiff(
-                m=hnsw_config.get("m"),
-                ef_construct=hnsw_config.get("ef_construct"),
-                full_scan_threshold=hnsw_config.get("full_scan_threshold"),
+                distance=self.DISTANCE_MAPPING[metric_name],
             ),
+            **collection_config,
         )
 
         self.config["offset"] = 0
         self.append(embeddings)
 
     def append(self, embeddings):
         offset = self.config.get("offset", 0)
@@ -107,22 +85,21 @@
     def delete(self, ids):
         self.qdrant_client.delete(
             collection_name=self.collection_name,
             points_selector=PointIdsList(points=ids),
         )
 
     def search(self, queries, limit):
-        hnsw_config = self.qdrant_config.get("hnsw", {})
-        ef_search = hnsw_config.get("ef_search")
+        search_params = self.qdrant_config.get("search_params", {})
         search_results = self.qdrant_client.search_batch(
             collection_name=self.collection_name,
             requests=[
                 SearchRequest(
                     vector=query.tolist(),
-                    params=SearchParams(hnsw_ef=ef_search),
+                    params=SearchParams(**search_params),
                     limit=limit,
                 )
                 for query in queries
             ],
         )
 
         results = []
@@ -132,11 +109,18 @@
 
     def count(self):
         result = self.qdrant_client.count(
             collection_name=self.collection_name,
         )
         return result.count
 
+    def load(self, path):
+        warnings.warn(
+            "Trying to call .load method on Qdrant ANN backend. " "This is redundant and won't have any effect.",
+            UserWarning,
+        )
+
     def save(self, path):
-        # All the indexed embeddings are already saved in a Qdrant collection,
-        # so there is no further need to perform any other action.
-        pass
+        warnings.warn(
+            "Trying to call .save method on Qdrant ANN backend. " "This is redundant and won't have any effect.",
+            UserWarning,
+        )
```

### Comparing `qdrant_txtai-1.0.1/PKG-INFO` & `qdrant_txtai-2.0.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,38 +1,38 @@
 Metadata-Version: 2.1
 Name: qdrant-txtai
-Version: 1.0.1
+Version: 2.0.0
 Summary: An integration of Qdrant ANN vector database backend with txtai
 License: Apache 2.0
 Author: Kacper Łukawski
 Author-email: kacper.lukawski@qdrant.com
-Requires-Python: >=3.7,<=3.11
+Requires-Python: >=3.8,<=3.13
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: qdrant-client (>=1.1.4,<2.0.0)
-Requires-Dist: txtai (>=5.0.0,<6.0.0)
+Classifier: Programming Language :: Python :: 3.12
+Requires-Dist: qdrant-client (>=1.9.1,<2.0.0)
+Requires-Dist: txtai (>=5.0.0)
 Description-Content-Type: text/markdown
 
 # qdrant-txtai
 
 [txtai](https://github.com/neuml/txtai) simplifies building AI-powered semantic 
 search applications using Transformers. It leverages the neural embeddings and
 their properties to encode high-dimensional data in a lower-dimensional space 
 and allows to find similar objects based on their embeddings' proximity. 
 
-Implementing such application in real-world use cases requires storing the
-embeddings in an efficient way though, namely in a vector database like 
+Implementing such applications in real-world use cases requires storing the
+embeddings efficiently, namely in a vector database like 
 [Qdrant](https://qdrant.tech). It offers not only a powerful engine for neural
 search, but also allows setting up a whole cluster if your data does not fit
-a single machine anymore. It is production grade and can be launched easily
+a single machine anymore. It is production-grade and can be launched easily
 with Docker.
 
 Combining the easiness of txtai with Qdrant's performance enables you to build
 production-ready semantic search applications way faster than before.
 
 ## Installation
 
@@ -40,19 +40,19 @@
 
 ```bash
 pip install qdrant-txtai
 ```
 
 ## Usage
 
-Running the txtai application with Qdrant as a vector storage requires launching
+Running the txtai application with Qdrant as vector storage requires launching
 a Qdrant instance. That might be done easily with Docker:
 
 ```bash
-docker run -p 6333:6333 -p:6334:6334 qdrant/qdrant:v1.0.1
+docker run -p 6333:6333 -p:6334:6334 qdrant/qdrant:latest
 ```
 
 Running the txtai application might be done either programmatically or by 
 providing configuration in a YAML file.
 
 ### Programmatically
 
@@ -80,73 +80,70 @@
 ```bash
 CONFIG=app.yml uvicorn "txtai.api:app"
 curl -X GET "http://localhost:8000/search?query=positive"
 ```
 
 ## Configuration properties
 
-*qdrant-txtai* allows you to configure both the connection details, and some 
-internal properties of the vector collection which may impact both speed and
+*qdrant-txtai* allows you to configure both the connection details and some 
+internal properties of the vector collection, which may impact both speed and
 accuracy. Please refer to [Qdrant docs](https://qdrant.github.io/qdrant/redoc/index.html#tag/collections/operation/create_collection)
 if you are interested in the meaning of each property.
 
 The example below presents all the available options, if we connect to Qdrant server:
 
 ```yaml
 embeddings:
   path: sentence-transformers/all-MiniLM-L6-v2
   backend: qdrant_txtai.ann.qdrant.Qdrant
-  metric: l2 # allowed values: l2 / cosine / ip
+  metric: l2 # allowed values: l1 / l2 / cosine / ip
   qdrant:
     url: qdrant.host
     port: 6333
     grpc_port: 6334
     prefer_grpc: true
     collection: CustomCollectionName
     https: true # for Qdrant Cloud
     api_key: XYZ # for Qdrant Cloud
-    hnsw:
-      m: 8
-      ef_construct: 256
-      full_scan_threshold:
-      ef_search: 512
+    search_params:
+      hnsw_ef: 100
 ```
 
 ### Local in-memory/disk-persisted mode
 
 Qdrant Python client, from version 1.1.1, supports local in-memory/disk-persisted mode. 
 That's a good choice for any test scenarios and quick experiments in which you do not 
-plan to store lots of vectors. In such a case spinning a Docker container might be even 
+plan to store lots of vectors. In such a case, spinning a Docker container might be even
 not required.
 
 #### In-memory storage
 
-In case you want to have a transient storage, for example in case of automated tests 
+In case you want to have transient storage, for example, in the case of automated tests 
 launched during your CI/CD pipeline, using Qdrant Local mode with in-memory storage 
 might be a preferred option.
 
 ```yaml
 embeddings:
   path: sentence-transformers/all-MiniLM-L6-v2
   backend: qdrant_txtai.ann.qdrant.Qdrant
-  metric: l2 # allowed values: l2 / cosine / ip
+  metric: l2 # allowed values: l1 / l2 / cosine / ip
   qdrant:
     location: ':memory:'
     prefer_grpc: true
 ```
 
 #### On disk storage
 
 However, if you prefer to keep the vectors between different runs of your application, 
-it might be better to use on disk storage and pass the path that should be used to 
+it might be better to use disk storage and pass the path that should be used to 
 persist the data.
 
 ```yaml
 embeddings:
   path: sentence-transformers/all-MiniLM-L6-v2
   backend: qdrant_txtai.ann.qdrant.Qdrant
-  metric: l2 # allowed values: l2 / cosine / ip
+  metric: l2 # allowed values: l1 / l2 / cosine / ip
   qdrant:
     path: '/home/qdrant/storage_local'
     prefer_grpc: true
 ```
```

