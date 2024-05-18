# Comparing `tmp/pyesorm-0.4.3.tar.gz` & `tmp/pyesorm-0.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyesorm-0.4.3.tar", last modified: Tue May  7 16:03:44 2024, max compression
+gzip compressed data, was "pyesorm-0.4.4.tar", last modified: Sat May 18 15:26:29 2024, max compression
```

## Comparing `pyesorm-0.4.3.tar` & `pyesorm-0.4.4.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 wallner    (501) staff       (20)        0 2024-05-07 16:03:44.944385 pyesorm-0.4.3/
--rw-r--r--   0 wallner    (501) staff       (20)    16725 2023-10-30 16:10:12.000000 pyesorm-0.4.3/LICENSE
--rw-r--r--   0 wallner    (501) staff       (20)    23956 2024-05-07 16:03:44.944030 pyesorm-0.4.3/PKG-INFO
--rw-r--r--   0 wallner    (501) staff       (20)    22319 2024-05-07 06:59:22.000000 pyesorm-0.4.3/README.md
-drwxr-xr-x   0 wallner    (501) staff       (20)        0 2024-05-07 16:03:44.923026 pyesorm-0.4.3/docs/
--rw-r--r--   0 wallner    (501) staff       (20)        0 2024-01-17 15:06:14.000000 pyesorm-0.4.3/docs/__init__.py
--rw-r--r--   0 wallner    (501) staff       (20)     1484 2024-01-17 15:18:18.000000 pyesorm-0.4.3/docs/changelog.py
--rw-r--r--   0 wallner    (501) staff       (20)     1462 2024-01-17 15:10:11.000000 pyesorm-0.4.3/docs/conf.py
-drwxr-xr-x   0 wallner    (501) staff       (20)        0 2024-05-07 16:03:44.934487 pyesorm-0.4.3/esorm/
--rw-r--r--   0 wallner    (501) staff       (20)      728 2024-05-07 10:10:02.000000 pyesorm-0.4.3/esorm/__init__.py
--rw-r--r--   0 wallner    (501) staff       (20)     3132 2024-01-22 17:32:29.000000 pyesorm-0.4.3/esorm/aggs.py
--rw-r--r--   0 wallner    (501) staff       (20)     4447 2024-05-07 05:08:54.000000 pyesorm-0.4.3/esorm/bulk.py
--rw-r--r--   0 wallner    (501) staff       (20)     1267 2024-05-07 05:07:07.000000 pyesorm-0.4.3/esorm/error.py
--rw-r--r--   0 wallner    (501) staff       (20)     1943 2023-10-31 19:12:30.000000 pyesorm-0.4.3/esorm/esorm.py
--rw-r--r--   0 wallner    (501) staff       (20)     3500 2024-01-24 09:39:22.000000 pyesorm-0.4.3/esorm/fastapi.py
--rw-r--r--   0 wallner    (501) staff       (20)    11640 2023-10-31 19:12:30.000000 pyesorm-0.4.3/esorm/fields.py
--rw-r--r--   0 wallner    (501) staff       (20)       52 2023-10-30 16:10:12.000000 pyesorm-0.4.3/esorm/logger.py
--rw-r--r--   0 wallner    (501) staff       (20)    41642 2024-05-07 15:36:26.000000 pyesorm-0.4.3/esorm/model.py
--rw-r--r--   0 wallner    (501) staff       (20)     9605 2024-01-18 19:16:18.000000 pyesorm-0.4.3/esorm/query.py
--rw-r--r--   0 wallner    (501) staff       (20)     1315 2024-01-18 19:06:35.000000 pyesorm-0.4.3/esorm/response.py
--rw-r--r--   0 wallner    (501) staff       (20)      996 2024-01-23 07:15:23.000000 pyesorm-0.4.3/esorm/utils.py
--rw-r--r--   0 wallner    (501) staff       (20)     5538 2023-10-30 16:10:12.000000 pyesorm-0.4.3/esorm/watcher.py
-drwxr-xr-x   0 wallner    (501) staff       (20)        0 2024-05-07 16:03:44.940862 pyesorm-0.4.3/pyesorm.egg-info/
--rw-r--r--   0 wallner    (501) staff       (20)    23956 2024-05-07 16:03:44.000000 pyesorm-0.4.3/pyesorm.egg-info/PKG-INFO
--rw-r--r--   0 wallner    (501) staff       (20)      514 2024-05-07 16:03:44.000000 pyesorm-0.4.3/pyesorm.egg-info/SOURCES.txt
--rw-r--r--   0 wallner    (501) staff       (20)        1 2024-05-07 16:03:44.000000 pyesorm-0.4.3/pyesorm.egg-info/dependency_links.txt
--rw-r--r--   0 wallner    (501) staff       (20)      272 2024-05-07 16:03:44.000000 pyesorm-0.4.3/pyesorm.egg-info/requires.txt
--rw-r--r--   0 wallner    (501) staff       (20)       17 2024-05-07 16:03:44.000000 pyesorm-0.4.3/pyesorm.egg-info/top_level.txt
--rw-r--r--   0 wallner    (501) staff       (20)       87 2023-10-31 20:33:56.000000 pyesorm-0.4.3/pyproject.toml
--rw-r--r--   0 wallner    (501) staff       (20)     1306 2024-05-07 16:03:44.945228 pyesorm-0.4.3/setup.cfg
--rw-r--r--   0 wallner    (501) staff       (20)       37 2023-10-30 16:10:12.000000 pyesorm-0.4.3/setup.py
-drwxr-xr-x   0 wallner    (501) staff       (20)        0 2024-05-07 16:03:44.939551 pyesorm-0.4.3/tests/
--rw-r--r--   0 wallner    (501) staff       (20)        0 2023-10-30 16:10:12.000000 pyesorm-0.4.3/tests/__init__.py
--rw-r--r--   0 wallner    (501) staff       (20)     7758 2024-05-07 14:38:00.000000 pyesorm-0.4.3/tests/conftest.py
--rw-r--r--   0 wallner    (501) staff       (20)    31583 2024-05-07 14:58:58.000000 pyesorm-0.4.3/tests/test_esorm.py
+drwxr-xr-x   0 wallner    (501) staff       (20)        0 2024-05-18 15:26:29.526158 pyesorm-0.4.4/
+-rw-r--r--   0 wallner    (501) staff       (20)    16725 2023-10-30 16:10:12.000000 pyesorm-0.4.4/LICENSE
+-rw-r--r--   0 wallner    (501) staff       (20)    23956 2024-05-18 15:26:29.525956 pyesorm-0.4.4/PKG-INFO
+-rw-r--r--   0 wallner    (501) staff       (20)    22319 2024-05-07 06:59:22.000000 pyesorm-0.4.4/README.md
+drwxr-xr-x   0 wallner    (501) staff       (20)        0 2024-05-18 15:26:29.516506 pyesorm-0.4.4/docs/
+-rw-r--r--   0 wallner    (501) staff       (20)        0 2024-01-17 15:06:14.000000 pyesorm-0.4.4/docs/__init__.py
+-rw-r--r--   0 wallner    (501) staff       (20)     1484 2024-01-17 15:18:18.000000 pyesorm-0.4.4/docs/changelog.py
+-rw-r--r--   0 wallner    (501) staff       (20)     1462 2024-01-17 15:10:11.000000 pyesorm-0.4.4/docs/conf.py
+drwxr-xr-x   0 wallner    (501) staff       (20)        0 2024-05-18 15:26:29.520966 pyesorm-0.4.4/esorm/
+-rw-r--r--   0 wallner    (501) staff       (20)      762 2024-05-18 14:17:08.000000 pyesorm-0.4.4/esorm/__init__.py
+-rw-r--r--   0 wallner    (501) staff       (20)     3132 2024-01-22 17:32:29.000000 pyesorm-0.4.4/esorm/aggs.py
+-rw-r--r--   0 wallner    (501) staff       (20)     4447 2024-05-07 05:08:54.000000 pyesorm-0.4.4/esorm/bulk.py
+-rw-r--r--   0 wallner    (501) staff       (20)     1267 2024-05-07 05:07:07.000000 pyesorm-0.4.4/esorm/error.py
+-rw-r--r--   0 wallner    (501) staff       (20)     2144 2024-05-18 14:16:43.000000 pyesorm-0.4.4/esorm/esorm.py
+-rw-r--r--   0 wallner    (501) staff       (20)     3500 2024-01-24 09:39:22.000000 pyesorm-0.4.4/esorm/fastapi.py
+-rw-r--r--   0 wallner    (501) staff       (20)    11640 2023-10-31 19:12:30.000000 pyesorm-0.4.4/esorm/fields.py
+-rw-r--r--   0 wallner    (501) staff       (20)       52 2023-10-30 16:10:12.000000 pyesorm-0.4.4/esorm/logger.py
+-rw-r--r--   0 wallner    (501) staff       (20)    42498 2024-05-18 14:17:26.000000 pyesorm-0.4.4/esorm/model.py
+-rw-r--r--   0 wallner    (501) staff       (20)     9605 2024-01-18 19:16:18.000000 pyesorm-0.4.4/esorm/query.py
+-rw-r--r--   0 wallner    (501) staff       (20)     1315 2024-01-18 19:06:35.000000 pyesorm-0.4.4/esorm/response.py
+-rw-r--r--   0 wallner    (501) staff       (20)      996 2024-01-23 07:15:23.000000 pyesorm-0.4.4/esorm/utils.py
+-rw-r--r--   0 wallner    (501) staff       (20)     5538 2023-10-30 16:10:12.000000 pyesorm-0.4.4/esorm/watcher.py
+drwxr-xr-x   0 wallner    (501) staff       (20)        0 2024-05-18 15:26:29.524105 pyesorm-0.4.4/pyesorm.egg-info/
+-rw-r--r--   0 wallner    (501) staff       (20)    23956 2024-05-18 15:26:29.000000 pyesorm-0.4.4/pyesorm.egg-info/PKG-INFO
+-rw-r--r--   0 wallner    (501) staff       (20)      514 2024-05-18 15:26:29.000000 pyesorm-0.4.4/pyesorm.egg-info/SOURCES.txt
+-rw-r--r--   0 wallner    (501) staff       (20)        1 2024-05-18 15:26:29.000000 pyesorm-0.4.4/pyesorm.egg-info/dependency_links.txt
+-rw-r--r--   0 wallner    (501) staff       (20)      272 2024-05-18 15:26:29.000000 pyesorm-0.4.4/pyesorm.egg-info/requires.txt
+-rw-r--r--   0 wallner    (501) staff       (20)       17 2024-05-18 15:26:29.000000 pyesorm-0.4.4/pyesorm.egg-info/top_level.txt
+-rw-r--r--   0 wallner    (501) staff       (20)       87 2023-10-31 20:33:56.000000 pyesorm-0.4.4/pyproject.toml
+-rw-r--r--   0 wallner    (501) staff       (20)     1306 2024-05-18 15:26:29.526701 pyesorm-0.4.4/setup.cfg
+-rw-r--r--   0 wallner    (501) staff       (20)       37 2023-10-30 16:10:12.000000 pyesorm-0.4.4/setup.py
+drwxr-xr-x   0 wallner    (501) staff       (20)        0 2024-05-18 15:26:29.523617 pyesorm-0.4.4/tests/
+-rw-r--r--   0 wallner    (501) staff       (20)        0 2023-10-30 16:10:12.000000 pyesorm-0.4.4/tests/__init__.py
+-rw-r--r--   0 wallner    (501) staff       (20)     7993 2024-05-18 15:08:50.000000 pyesorm-0.4.4/tests/conftest.py
+-rw-r--r--   0 wallner    (501) staff       (20)    32738 2024-05-18 15:12:48.000000 pyesorm-0.4.4/tests/test_esorm.py
```

### Comparing `pyesorm-0.4.3/LICENSE` & `pyesorm-0.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pyesorm-0.4.3/PKG-INFO` & `pyesorm-0.4.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyesorm
-Version: 0.4.3
+Version: 0.4.4
 Summary: Python ElasticSearch ORM based on Pydantic
 Home-page: https://github.com/wallneradam/esorm
 Author: Adam Wallner
 Author-email: Adam.wallner@gmail.com
 License: MPL-2.0
 Project-URL: Bug Tracker, https://github.com/wallneradam/esorm/issues
 Project-URL: Documentation, https://esorm.readthedocs.io/en/latest/
```

### Comparing `pyesorm-0.4.3/README.md` & `pyesorm-0.4.4/README.md`

 * *Files identical despite different names*

### Comparing `pyesorm-0.4.3/docs/changelog.py` & `pyesorm-0.4.4/docs/changelog.py`

 * *Files identical despite different names*

### Comparing `pyesorm-0.4.3/docs/conf.py` & `pyesorm-0.4.4/docs/conf.py`

 * *Files identical despite different names*

### Comparing `pyesorm-0.4.3/esorm/__init__.py` & `pyesorm-0.4.4/esorm/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,26 +5,26 @@
 from .error import (
     InvalidResponseError,
     InvalidModelError,
     NotFoundError,
 )
 from .model import (TModel, ESBaseModel, ESModel, ESModelTimestamp, Pagination, Sort, setup_mappings,
                     lazy_property, retry_on_conflict)
-from .esorm import es, connect
+from .esorm import es, connect, get_es_version
 from .fields import Field
 from .bulk import ESBulk
 from . import fields
 
 __all__ = [
     "TModel", "ESBaseModel", "ESModel", "ESModelTimestamp", "ESBulk",
     'lazy_property', 'retry_on_conflict',
     "es",
     "NotFoundError",
     "InvalidModelError",
     "InvalidResponseError",
-    "connect",
+    "connect", "get_es_version",
     "setup_mappings",
     "Field",
     "fields",
     "error",
     "Pagination", "Sort",
 ]
```

### Comparing `pyesorm-0.4.3/esorm/aggs.py` & `pyesorm-0.4.4/esorm/aggs.py`

 * *Files identical despite different names*

### Comparing `pyesorm-0.4.3/esorm/bulk.py` & `pyesorm-0.4.4/esorm/bulk.py`

 * *Files identical despite different names*

### Comparing `pyesorm-0.4.3/esorm/error.py` & `pyesorm-0.4.4/esorm/error.py`

 * *Files identical despite different names*

### Comparing `pyesorm-0.4.3/esorm/esorm.py` & `pyesorm-0.4.4/esorm/esorm.py`

 * *Files 9% similar despite different names*

```diff
@@ -27,15 +27,15 @@
             raise ValueError(f"ElasticSearch client has not been set yet, please call connect! ({name})")
         return getattr(self.__client__, name)
 
 
 # Global client proxy
 es = cast(AsyncElasticsearch, _ESProxy())
 
-__all__ = ['es', 'connect']
+__all__ = ['es', 'connect', 'get_es_version']
 
 
 async def connect(hosts: Union[str, List[Union[str, Mapping[str, Union[str, int]], NodeConfig]]],
                   *args, wait=False, **kwargs) -> Optional[AsyncElasticsearch]:
     """
     Connect to ElasticSearch
 
@@ -58,7 +58,17 @@
                 else:
                     break
 
         return es
 
     except asyncio.CancelledError:
         return None
+
+
+async def get_es_version() -> str:
+    """
+    Get ElasticSearch version
+
+    :return: ElasticSearch version
+    """
+    info = await es.info()
+    return info['version']['number']
```

### Comparing `pyesorm-0.4.3/esorm/fastapi.py` & `pyesorm-0.4.4/esorm/fastapi.py`

 * *Files identical despite different names*

### Comparing `pyesorm-0.4.3/esorm/fields.py` & `pyesorm-0.4.4/esorm/fields.py`

 * *Files identical despite different names*

### Comparing `pyesorm-0.4.3/esorm/model.py` & `pyesorm-0.4.4/esorm/model.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 # noinspection PyProtectedMember
 from pydantic.fields import FieldInfo  # It is just not in __all__ of pydantic.fields, but we strongly need it
 
 from .utils import snake_case, utcnow
 from .aggs import ESAggs, ESAggsResponse
 
 from .error import InvalidResponseError, NotFoundError
-from .esorm import es
+from .esorm import es, get_es_version
 from .query import ESQuery
 from .response import ESResponse
 
 from .logger import logger
 
 __all__ = [
     'TModel',
@@ -50,15 +50,15 @@
 # Global variables and types
 #
 
 # noinspection PyProtectedMember
 _model_construction = getattr(pydantic_main, '_model_construction')
 ModelMetaclass = _model_construction.ModelMetaclass
 
-_default_index_prefix = 'esorm'
+_default_index_prefix = 'esorm_'
 
 # Map python types to ES type
 _pydantic_type_map = {
     str: 'keyword',  # Str is defaulted to keyword
     int: 'long',
     float: 'double',
     bool: 'boolean',
@@ -178,15 +178,15 @@
 
             # Create (new) ESConfig class inside the class
             model.ESConfig = type('ESConfig', (object,), dict(m_dict))
 
             # Set default index name if not already set
             if is_model and not getattr(model.ESConfig, 'index', None):
                 # Default index is the name of the class in snake_case
-                model.ESConfig.index = _default_index_prefix + '-' + snake_case(name)
+                model.ESConfig.index = _default_index_prefix + snake_case(name)
 
             # If there is an 'id' field, set it as id_field
             if is_model and 'id' in model.model_fields.keys():
                 model.ESConfig.id_field = 'id'
 
             # Add to models
             if is_model:
@@ -514,15 +514,15 @@
         :param id: Document id
         :param routing: Shard routing value
         :raises esorm.error.NotFoundError: Returned if document not found
         :return: ESModel object
         """
         kwargs = {'id': id}
         try:
-            es_res = await cls.call('get', **kwargs)
+            es_res = await cls.call('get', routing=routing, **kwargs)
             return await _lazy_process_results(cls.from_es(es_res))
         except ElasticNotFoundError:
             raise NotFoundError(f"Document with id {id} not found")
 
     async def delete(self, *, wait_for=False, routing: Optional[str] = None):
         """
         Deletes document from ElasticSearch.
@@ -1021,28 +1021,51 @@
                                 **other_settings: Any) -> object:
     """
     Create index template
 
     :param name: The name of the template
     :param prefix_name: The prefix of index pattern
     :param shards: Number of shards
-    :param replicas: Nuber of replicas
+    :param replicas: Number of replicas
     :param other_settings: Other settings
     :return: The result object from ES
     """
-    return await es.indices.put_template(
-        name=name,
-        index_patterns=[f'{prefix_name}-*'],
-        settings=dict(
-            number_of_shards=shards,
-            number_of_replicas=replicas,
-            **other_settings
-        ),
-        request_timeout=90
-    )
+    es_version = await get_es_version()
+    major, minor, _ = map(int, es_version.split('.'))
+
+    if major > 7 or (major == 7 and minor >= 8):
+        # Use composable template for ES 7.8 and above
+        return await es.indices.put_index_template(
+            name=name,
+            body={
+                "index_patterns": [f'{prefix_name}*'],
+                "template": {
+                    "settings": {
+                        "number_of_shards": shards,
+                        "number_of_replicas": replicas,
+                        **other_settings
+                    }
+                }
+            },
+            request_timeout=90
+        )
+    else:
+        # Use legacy template for ES versions below 7.8
+        return await es.indices.put_template(
+            name=name,
+            body={
+                "index_patterns": [f'{prefix_name}*'],
+                "settings": {
+                    "number_of_shards": shards,
+                    "number_of_replicas": replicas,
+                    **other_settings
+                }
+            },
+            request_timeout=90
+        )
 
 
 async def setup_mappings(*_, debug=False):
     """
     Create mappings for indices or try to extend it if there are new fields
     """
```

### Comparing `pyesorm-0.4.3/esorm/query.py` & `pyesorm-0.4.4/esorm/query.py`

 * *Files identical despite different names*

### Comparing `pyesorm-0.4.3/esorm/response.py` & `pyesorm-0.4.4/esorm/response.py`

 * *Files identical despite different names*

### Comparing `pyesorm-0.4.3/esorm/utils.py` & `pyesorm-0.4.4/esorm/utils.py`

 * *Files identical despite different names*

### Comparing `pyesorm-0.4.3/esorm/watcher.py` & `pyesorm-0.4.4/esorm/watcher.py`

 * *Files identical despite different names*

### Comparing `pyesorm-0.4.3/pyesorm.egg-info/PKG-INFO` & `pyesorm-0.4.4/pyesorm.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyesorm
-Version: 0.4.3
+Version: 0.4.4
 Summary: Python ElasticSearch ORM based on Pydantic
 Home-page: https://github.com/wallneradam/esorm
 Author: Adam Wallner
 Author-email: Adam.wallner@gmail.com
 License: MPL-2.0
 Project-URL: Bug Tracker, https://github.com/wallneradam/esorm/issues
 Project-URL: Documentation, https://esorm.readthedocs.io/en/latest/
```

### Comparing `pyesorm-0.4.3/pyesorm.egg-info/SOURCES.txt` & `pyesorm-0.4.4/pyesorm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyesorm-0.4.3/setup.cfg` & `pyesorm-0.4.4/setup.cfg`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = pyesorm
-version = 0.4.3
+version = 0.4.4
 author = Adam Wallner
 author_email = Adam.wallner@gmail.com
 description = Python ElasticSearch ORM based on Pydantic
 long_description = file: README.md
 long_description_content_type = text/markdown
 keywords = ElasticSearch, ORM, Pydantic
 license = MPL-2.0
```

### Comparing `pyesorm-0.4.3/tests/conftest.py` & `pyesorm-0.4.4/tests/conftest.py`

 * *Files 10% similar despite different names*

```diff
@@ -50,57 +50,63 @@
     esorm.model._ESModelMeta.__models__.clear()
     for module_name in list(sys.modules):
         if module_name.startswith('esorm'):
             del sys.modules[module_name]
 
 
 @pytest.fixture(scope="class")  # Test both ES 8.x and 7.x
-def docker_es(service):
+async def docker_es(service):
     compose_file = os.path.join(os.path.dirname(__file__), 'docker-compose.yml')
     res = subprocess.run(['docker', 'compose', '-f', compose_file, 'up', '-d', service], check=True)
     logger.info(f"Started service: {service}")
     assert res.returncode == 0
     yield
     subprocess.run(['docker', 'compose', '-f', compose_file, 'down', service, '-v'], check=True)
     logger.info(f"Stopped service: {service}")
 
 
 # noinspection PyUnresolvedReferences
 @pytest.fixture(scope="class")
-async def es(docker_es, esorm):
+async def es(docker_es, esorm, service):
     """
     ElasticSearch fixture for version 8.x
     """
     es = await esorm.connect(hosts=["http://localhost:9200"], wait=True)
+
+    es_version = await esorm.get_es_version()
+    major, _, _ = map(int, es_version.split('.'))
+    if service == 'es7x':
+        assert major == 7
+    elif service == 'es8x':
+        assert major == 8
+
+    major, minor, _ = map(int, es_version.split('.'))
     assert es is not None
     yield es
     await es.close()
 
 
 # noinspection PyUnresolvedReferences
 @pytest.fixture(scope="class")
 def model_python(esorm):
     """
     Model to test python types
     """
-
     from datetime import datetime, date, time
 
     class PythonFieldModel(esorm.ESModel):
         f_str: str
         f_int: int
         f_float: float
         f_bool: bool
         f_datetime: datetime
         f_date: date
         f_time: time
 
-    yield PythonFieldModel
-
-    del PythonFieldModel
+    return PythonFieldModel
 
 
 # noinspection PyUnresolvedReferences
 @pytest.fixture(scope="class")
 def model_es(esorm):
     """
     Model to test ES types
@@ -115,17 +121,15 @@
         f_int32: esorm.fields.int32
         f_long: esorm.fields.long
         f_float16: esorm.fields.float16
         f_float32: esorm.fields.float32
         f_double: esorm.fields.double
         f_geo_point: esorm.fields.geo_point
 
-    yield ESFieldModel
-
-    del ESFieldModel
+    return ESFieldModel
 
 
 @pytest.fixture(scope="class")
 def model_es_optional(esorm):
     """
     Model to test optional ES types
     """
@@ -139,33 +143,29 @@
         f_int32: Optional[esorm.fields.int32] = None
         f_long: Optional[esorm.fields.long] = None
         f_float16: Optional[esorm.fields.float16] = None
         f_float32: Optional[esorm.fields.float32] = None
         f_double: Optional[esorm.fields.double] = None
         f_geo_point: Optional[esorm.fields.geo_point] = None
 
-    yield ESOptionalFieldModel
-
-    del ESOptionalFieldModel
+    return ESOptionalFieldModel
 
 
 # noinspection PyUnresolvedReferences
 @pytest.fixture(scope="class")
 def model_timestamp(esorm):
     """
     Model to test timestamp
     """
 
     class TimestampModel(esorm.ESModelTimestamp):
         f_str: str
         f_int: int = 1
 
-    yield TimestampModel
-
-    del TimestampModel
+    return TimestampModel
 
 
 # noinspection PyUnresolvedReferences
 @pytest.fixture(scope="class")
 def model_config(esorm):
     """
     Model to test config
@@ -188,33 +188,44 @@
         f_str: str
         """ Field to test """
 
         @property
         def __routing__(self) -> str:
             return self.custom_id + '_routing'
 
-    yield ConfigModel
+    return ConfigModel
 
-    del ConfigModel
+
+@pytest.fixture(scope="class")
+def model_index_template(esorm):
+    """
+    Model to test index template
+    """
+
+    class IndexTemplateModel(esorm.ESModel):
+        class ESConfig:
+            index = 'custom_index_template'
+
+        f_str: str
+
+    return IndexTemplateModel
 
 
 # noinspection PyUnresolvedReferences
 @pytest.fixture(scope="class")
 def model_with_id(esorm):
     """
     Model to test id field
     """
 
     class IdModel(esorm.ESModel):
         id: str
         f_str: str
 
-    yield IdModel
-
-    del IdModel
+    return IdModel
 
 
 # noinspection PyUnresolvedReferences
 @pytest.fixture(scope="class")
 def model_with_int_id(esorm):
     """
     Model to test int id field
@@ -223,17 +234,15 @@
     class IntIdModel(esorm.ESModel):
         class ESConfig:
             id_field = 'custom_id'
 
         custom_id: int
         f_str: str
 
-    yield IntIdModel
-
-    del IntIdModel
+    return IntIdModel
 
 
 # noinspection PyUnresolvedReferences
 @pytest.fixture(scope="class")
 def model_with_prop_id(esorm):
     """
     Model to test property id field
@@ -243,33 +252,29 @@
         @property
         def __id__(self) -> int:
             return self.custom_id + 1000
 
         custom_id: int
         f_str: str
 
-    yield PropIdModel
-
-    del PropIdModel
+    return PropIdModel
 
 
 # noinspection PyUnresolvedReferences
 @pytest.fixture(scope="class")
 def model_nested(esorm, model_timestamp):
     """
     Model to test nested fields
     """
 
     class NestedFieldModel(esorm.ESModel):
         f_nested: model_timestamp
         f_float: float = 0.5
 
-    yield NestedFieldModel
-
-    del NestedFieldModel
+    return NestedFieldModel
 
 
 # noinspection PyUnresolvedReferences
 @pytest.fixture(scope="class")
 def model_lazy_prop(esorm):
     """
     Model to test lazy properties
@@ -282,17 +287,15 @@
         f_str: str
 
         # noinspection PyUnresolvedReferences
         @esorm.lazy_property
         async def same_f_strs(self) -> List['LazyPropModel']:
             return await self.search_by_fields({'f_str': self.f_str})
 
-    yield LazyPropModel
-
-    del LazyPropModel
+    return LazyPropModel
 
 
 # noinspection PyUnresolvedReferences
 @pytest.fixture(scope="class")
 async def model_nested_binary(esorm):
     """
     Model to test nested binary fields
@@ -302,17 +305,15 @@
         f_binary: Optional[esorm.fields.binary] = esorm.Field(None, index=False)
 
     class NestedBinaryModel(esorm.ESModel):
         f_nested: BinaryModel
 
     await esorm.setup_mappings()
 
-    yield BinaryModel, NestedBinaryModel
-    del BinaryModel
-    del NestedBinaryModel
+    return BinaryModel, NestedBinaryModel
 
 
 @pytest.fixture(scope="class")
 async def model_nested_base_model(esorm):
     """
     Model to test nested base model
     """
@@ -328,10 +329,8 @@
             return f'lazy(f_str={self.f_str}, f_int={self.f_int})'
 
     class NestedBaseModelModel(esorm.ESModel):
         f_nested: NestedBaseModel
 
     await esorm.setup_mappings()
 
-    yield NestedBaseModel, NestedBaseModelModel
-    del NestedBaseModel
-    del NestedBaseModelModel
+    return NestedBaseModel, NestedBaseModelModel
```

### Comparing `pyesorm-0.4.3/tests/test_esorm.py` & `pyesorm-0.4.4/tests/test_esorm.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from typing import TYPE_CHECKING
 import pytest
 
 
-@pytest.mark.parametrize('service', ['es7x', 'es8x'], scope='class')
+@pytest.mark.parametrize('service', ['es8x', 'es7x'], scope='class')
 class TestBaseTests:
     """
     Base tests
     """
 
     doc_id: str = None
 
@@ -35,83 +35,95 @@
         assert not hasattr(BaseChild.ESConfig, 'index')
 
     async def test_create_model_with_python_fields(self, es, esorm, model_python):
         """
         Test model with python fields
         """
         assert model_python is not None
-        assert model_python.ESConfig.index == 'esorm-python_field_model'
+        assert model_python.ESConfig.index == 'esorm_python_field_model'
 
     async def test_create_model_with_es_fields(self, es, esorm, model_es):
         """
         Test model with ES fields
         """
         assert model_es is not None
-        assert model_es.ESConfig.index == 'esorm-es_field_model'
+        assert model_es.ESConfig.index == 'esorm_es_field_model'
 
     async def test_create_model_with_es_optional_fields(self, es, esorm, model_es_optional):
         """
         Test model with ES fields
         """
         assert model_es_optional is not None
-        assert model_es_optional.ESConfig.index == 'esorm-es_optional_field_model'
+        assert model_es_optional.ESConfig.index == 'esorm_es_optional_field_model'
 
     async def test_create_timestamp_models(self, es, esorm, model_timestamp):
         """
         Test timestamp models
         """
         assert model_timestamp is not None
-        assert model_timestamp.ESConfig.index == 'esorm-timestamp_model'
+        assert model_timestamp.ESConfig.index == 'esorm_timestamp_model'
         assert 'created_at' in model_timestamp.model_fields
         assert 'modified_at' in model_timestamp.model_fields
 
     async def test_create_model_config(self, es, esorm, model_config):
         """
         Test model config
         """
         assert model_config is not None
         assert model_config.ESConfig.index == 'custom_index'
 
+    async def test_model_template(self, es, esorm, model_index_template):
+        """
+        Test model config
+        """
+        assert model_index_template is not None
+        assert model_index_template.ESConfig.index == 'custom_index_template'
+
     async def test_create_model_with_id(self, es, esorm, model_with_id):
         """
         Test model with config
         """
         assert model_with_id is not None
-        assert model_with_id.ESConfig.index == 'esorm-id_model'
+        assert model_with_id.ESConfig.index == 'esorm_id_model'
         assert model_with_id.ESConfig.id_field == 'id'
 
     async def test_create_model_with_int_id(self, es, esorm, model_with_int_id):
         """
         Test model with int id
         """
         assert model_with_int_id is not None
-        assert model_with_int_id.ESConfig.index == 'esorm-int_id_model'
+        assert model_with_int_id.ESConfig.index == 'esorm_int_id_model'
         assert model_with_int_id.ESConfig.id_field == 'custom_id'
 
     async def test_create_model_with_prop_id(self, es, esorm, model_with_prop_id):
         """
         Test model with property id
         """
         assert model_with_prop_id is not None
-        assert model_with_prop_id.ESConfig.index == 'esorm-prop_id_model'
+        assert model_with_prop_id.ESConfig.index == 'esorm_prop_id_model'
         assert model_with_prop_id.ESConfig.id_field is None
 
     async def test_create_nested_model(self, es, esorm, model_nested):
         """
         Test nested model
         """
         assert model_nested is not None
-        assert model_nested.ESConfig.index == 'esorm-nested_field_model'
+        assert model_nested.ESConfig.index == 'esorm_nested_field_model'
 
     async def test_create_mappings(self, es, esorm, model_python, model_es, model_es_optional,
                                    model_timestamp, model_config, model_with_id, model_with_int_id,
-                                   model_with_prop_id, model_nested, model_lazy_prop):
+                                   model_with_prop_id, model_nested, model_lazy_prop,
+                                   model_index_template):
         """
         Test create mappings
         """
+        # Create index template
+        await esorm.model.create_index_template('custom_index_template', prefix_name='custom_index_',
+                                                shards=5, auto_expand_replicas="1-2")
+
         await esorm.setup_mappings()
         # Check if index exists
         assert await es.indices.exists(index=model_python.ESConfig.index)
 
         # Check if mappings are correct for python fields
         mappings = await es.indices.get_mapping(index=model_python.ESConfig.index)
         assert mappings[model_python.ESConfig.index]['mappings']['properties']['f_str']['type'] == 'keyword'
@@ -161,14 +173,22 @@
             "Id fields should not be in mappings"
         # Check index settings
         settings = await es.indices.get_settings(index=model_config.ESConfig.index)
         assert settings[model_config.ESConfig.index]['settings']['index']['number_of_shards'] == '6'
         assert settings[model_config.ESConfig.index]['settings']['index']['number_of_replicas'] == '1'
         assert settings[model_config.ESConfig.index]['settings']['index']['refresh_interval'] == '5s'
 
+        # Check if mappings are correct for model with index template
+        mappings = await es.indices.get_mapping(index=model_index_template.ESConfig.index)
+        assert mappings[model_index_template.ESConfig.index]['mappings']['properties']['f_str']['type'] == 'keyword'
+        # Check index settings
+        settings = await es.indices.get_settings(index=model_index_template.ESConfig.index)
+        assert settings[model_index_template.ESConfig.index]['settings']['index']['number_of_shards'] == '5'
+        assert settings[model_index_template.ESConfig.index]['settings']['index']['auto_expand_replicas'] == '1-2'
+
         # Check if mappings are correct for model with id
         mappings = await es.indices.get_mapping(index=model_with_id.ESConfig.index)
         assert mappings[model_with_id.ESConfig.index]['mappings']['properties']['f_str']['type'] == 'keyword'
         assert 'id' not in mappings[model_with_id.ESConfig.index]['mappings']['properties'], \
             "Id fields should not be in mappings"
 
         # Check if mappings are correct for model with int id
```

