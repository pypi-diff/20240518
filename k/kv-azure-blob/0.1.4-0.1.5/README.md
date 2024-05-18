# Comparing `tmp/kv_azure_blob-0.1.4.tar.gz` & `tmp/kv_azure_blob-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kv_azure_blob-0.1.4.tar", last modified: Sun May 12 08:59:26 2024, max compression
+gzip compressed data, was "kv_azure_blob-0.1.5.tar", last modified: Sat May 18 18:55:04 2024, max compression
```

## Comparing `kv_azure_blob-0.1.4.tar` & `kv_azure_blob-0.1.5.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-12 08:59:26.656930 kv_azure_blob-0.1.4/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1471 2024-05-12 08:59:26.656930 kv_azure_blob-0.1.4/PKG-INFO
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1063 2024-05-12 08:47:51.000000 kv_azure_blob-0.1.4/README.md
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      608 2024-05-12 08:59:18.000000 kv_azure_blob-0.1.4/pyproject.toml
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       38 2024-05-12 08:59:26.656930 kv_azure_blob-0.1.4/setup.cfg
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-12 08:59:26.646930 kv_azure_blob-0.1.4/src/
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-12 08:59:26.636930 kv_azure_blob-0.1.4/src/kv/
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-12 08:59:26.636930 kv_azure_blob-0.1.4/src/kv/azure/
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-12 08:59:26.646930 kv_azure_blob-0.1.4/src/kv/azure/blob/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      167 2024-05-12 07:36:23.000000 kv_azure_blob-0.1.4/src/kv/azure/blob/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      104 2024-05-12 08:28:05.000000 kv_azure_blob-0.1.4/src/kv/azure/blob/__init__.pyi
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     3673 2024-05-12 08:59:04.000000 kv_azure_blob-0.1.4/src/kv/azure/blob/blob.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     2979 2024-05-12 08:41:36.000000 kv_azure_blob-0.1.4/src/kv/azure/blob/container.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      569 2024-05-12 08:38:57.000000 kv_azure_blob-0.1.4/src/kv/azure/blob/util.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-12 08:59:26.656930 kv_azure_blob-0.1.4/src/kv_azure_blob.egg-info/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1471 2024-05-12 08:59:26.000000 kv_azure_blob-0.1.4/src/kv_azure_blob.egg-info/PKG-INFO
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      372 2024-05-12 08:59:26.000000 kv_azure_blob-0.1.4/src/kv_azure_blob.egg-info/SOURCES.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)        1 2024-05-12 08:59:26.000000 kv_azure_blob-0.1.4/src/kv_azure_blob.egg-info/dependency_links.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       50 2024-05-12 08:59:26.000000 kv_azure_blob-0.1.4/src/kv_azure_blob.egg-info/requires.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)        3 2024-05-12 08:59:26.000000 kv_azure_blob-0.1.4/src/kv_azure_blob.egg-info/top_level.txt
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-18 18:55:04.484403 kv_azure_blob-0.1.5/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1471 2024-05-18 18:55:04.474402 kv_azure_blob-0.1.5/PKG-INFO
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1063 2024-05-12 08:47:51.000000 kv_azure_blob-0.1.5/README.md
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      608 2024-05-18 18:55:01.000000 kv_azure_blob-0.1.5/pyproject.toml
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       38 2024-05-18 18:55:04.484403 kv_azure_blob-0.1.5/setup.cfg
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-18 18:55:04.464402 kv_azure_blob-0.1.5/src/
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-18 18:55:04.464402 kv_azure_blob-0.1.5/src/kv/
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-18 18:55:04.464402 kv_azure_blob-0.1.5/src/kv/azure/
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-18 18:55:04.474402 kv_azure_blob-0.1.5/src/kv/azure/blob/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      167 2024-05-12 07:36:23.000000 kv_azure_blob-0.1.5/src/kv/azure/blob/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      104 2024-05-12 08:28:05.000000 kv_azure_blob-0.1.5/src/kv/azure/blob/__init__.pyi
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     3845 2024-05-18 18:54:50.000000 kv_azure_blob-0.1.5/src/kv/azure/blob/blob.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     2979 2024-05-12 08:41:36.000000 kv_azure_blob-0.1.5/src/kv/azure/blob/container.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      569 2024-05-12 08:38:57.000000 kv_azure_blob-0.1.5/src/kv/azure/blob/util.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-18 18:55:04.474402 kv_azure_blob-0.1.5/src/kv_azure_blob.egg-info/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1471 2024-05-18 18:55:04.000000 kv_azure_blob-0.1.5/src/kv_azure_blob.egg-info/PKG-INFO
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      372 2024-05-18 18:55:04.000000 kv_azure_blob-0.1.5/src/kv_azure_blob.egg-info/SOURCES.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)        1 2024-05-18 18:55:04.000000 kv_azure_blob-0.1.5/src/kv_azure_blob.egg-info/dependency_links.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       50 2024-05-18 18:55:04.000000 kv_azure_blob-0.1.5/src/kv_azure_blob.egg-info/requires.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)        3 2024-05-18 18:55:04.000000 kv_azure_blob-0.1.5/src/kv_azure_blob.egg-info/top_level.txt
```

### Comparing `kv_azure_blob-0.1.4/PKG-INFO` & `kv_azure_blob-0.1.5/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kv-azure-blob
-Version: 0.1.4
+Version: 0.1.5
 Summary: KV API implementation on Azure Blob Storage
 Author-email: Marcel Claramunt <marcel@moveread.com>
 Project-URL: repo, https://github.com/marciclabas/python-storage.git
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Requires-Dist: azure-storage-blob
 Requires-Dist: aiohttp
```

### Comparing `kv_azure_blob-0.1.4/README.md` & `kv_azure_blob-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `kv_azure_blob-0.1.4/pyproject.toml` & `kv_azure_blob-0.1.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "kv-azure-blob"
-version = "0.1.4"
+version = "0.1.5"
 authors = [
   {name="Marcel Claramunt", email="marcel@moveread.com"}
 ]
 description = "KV API implementation on Azure Blob Storage"
 dependencies = [
   "azure-storage-blob", "aiohttp", "haskellian", "lazy-loader"
 ]
```

### Comparing `kv_azure_blob-0.1.4/src/kv/azure/blob/blob.py` & `kv_azure_blob-0.1.5/src/kv/azure/blob/blob.py`

 * *Files 13% similar despite different names*

```diff
@@ -4,19 +4,20 @@
 from kv.api import LocatableKV, InvalidData, DBError
 from kv.azure.blob import BlobContainerKV
 from azure.storage.blob.aio import BlobServiceClient
 
 A = TypeVar('A')
 
 def default_split(key: str) -> tuple[str, str]:
-  return key.split('/', 1) # type: ignore
+  parts = key.split('/', 1)
+  return (parts[0], parts[1]) if len(parts) > 1 else ('container', parts[0])
 
 @dataclass
 class BlobKV(LocatableKV[A], Generic[A]):
-  client: BlobServiceClient
+  client: Callable[[], BlobServiceClient]
   split_key: Callable[[str], tuple[str, str]] = default_split
   """Split a key into container + blob. Defaults to `{container}/{blob/with/slashes}`"""
   parse: Callable[[bytes], Either[InvalidData, A]] = Right # type: ignore
   dump: Callable[[A], bytes | str] = lambda x: x # type: ignore
 
   @overload
   @classmethod
@@ -24,43 +25,46 @@
     cls, Type: type[A], conn_str: str, /,
     split_key: Callable[[str], tuple[str, str]] = default_split
   ) -> 'BlobKV[A]':
     ...
   @overload
   @classmethod
   def validated(
-    cls, Type: type[A], client: BlobServiceClient, /,
+    cls, Type: type[A], client_supplier: Callable[[], BlobServiceClient], /,
     split_key: Callable[[str], tuple[str, str]] = default_split
   ) -> 'BlobKV[A]':
     ...
 
   @classmethod
   def validated(
-    cls, Type: type[A], client: BlobServiceClient | str,
+    cls, Type: type[A], client: Callable[[], BlobServiceClient] | str,
     split_key: Callable[[str], tuple[str, str]] = default_split
   ) -> 'BlobKV[A]':
-    client = BlobServiceClient.from_connection_string(client) if isinstance(client, str) else client
+    if isinstance(client, str):
+      client_fn = (lambda: BlobServiceClient.from_connection_string(client))
+    else:
+      client_fn = client
     from pydantic import RootModel
     Model = RootModel[Type]
     return BlobKV(
-      client=client, split_key=split_key,
+      client=client_fn, split_key=split_key,
       parse=lambda b: E.validate_json(b, Model).fmap(lambda x: x.root).mapl(InvalidData),
       dump=lambda x: Model(x).model_dump_json(exclude_none=True)
     )
   
   @classmethod
   def from_conn_str(
     cls, conn_str: str,
     split_key: Callable[[str], tuple[str, str]] = default_split
   ) -> 'BlobKV[A]':
-    return BlobKV(client=BlobServiceClient.from_connection_string(conn_str), split_key=split_key)
+    return BlobKV(client=lambda: BlobServiceClient.from_connection_string(conn_str), split_key=split_key)
 
   def _kv(self, container: str) -> BlobContainerKV:
     return BlobContainerKV(
-      client=lambda: self.client.get_container_client(container),
+      client=lambda: self.client().get_container_client(container),
       parse=self.parse, dump=self.dump
     )
 
   def _delete(self, key: str):
     container, blob = self.split_key(key)
     return self._kv(container)._delete(blob)
   
@@ -69,15 +73,15 @@
     return self._kv(container)._insert(blob, value)
   
   def _read(self, key: str):
     container, blob = self.split_key(key)
     return self._kv(container)._read(blob)
   
   async def _containers(self) -> Sequence[str]:
-    containers = await AI.syncify(self.client.list_containers())
+    containers = await AI.syncify(self.client().list_containers())
     return [c.name for c in containers] # type: ignore (mr azure isn't very good at python types, it seems)
   
   @E.do[DBError]()
   async def _container_keys(self, container: str):
     keys = (await self._kv(container).keys()).unsafe()
     return [f"{container}/{k}" for k in keys]
```

### Comparing `kv_azure_blob-0.1.4/src/kv/azure/blob/container.py` & `kv_azure_blob-0.1.5/src/kv/azure/blob/container.py`

 * *Files identical despite different names*

### Comparing `kv_azure_blob-0.1.4/src/kv/azure/blob/util.py` & `kv_azure_blob-0.1.5/src/kv/azure/blob/util.py`

 * *Files identical despite different names*

### Comparing `kv_azure_blob-0.1.4/src/kv_azure_blob.egg-info/PKG-INFO` & `kv_azure_blob-0.1.5/src/kv_azure_blob.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kv-azure-blob
-Version: 0.1.4
+Version: 0.1.5
 Summary: KV API implementation on Azure Blob Storage
 Author-email: Marcel Claramunt <marcel@moveread.com>
 Project-URL: repo, https://github.com/marciclabas/python-storage.git
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Requires-Dist: azure-storage-blob
 Requires-Dist: aiohttp
```

