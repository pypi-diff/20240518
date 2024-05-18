# Comparing `tmp/shared_cache-0.0.1.tar.gz` & `tmp/shared_cache-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shared_cache-0.0.1.tar", last modified: Wed May 15 05:39:14 2024, max compression
+gzip compressed data, was "shared_cache-1.0.1.tar", last modified: Sat May 18 21:20:17 2024, max compression
```

## Comparing `shared_cache-0.0.1.tar` & `shared_cache-1.0.1.tar`

### file list

```diff
@@ -1,25 +1,26 @@
-drwxrwxr-x   0 wassef    (1000) wassef    (1000)        0 2024-05-15 05:39:14.081018 shared_cache-0.0.1/
--rw-rw-r--   0 wassef    (1000) wassef    (1000)      894 2024-05-14 20:56:31.000000 shared_cache-0.0.1/.pre-commit-config.yaml
--rw-rw-r--   0 wassef    (1000) wassef    (1000)     1072 2023-09-04 18:49:49.000000 shared_cache-0.0.1/LICENSE
--rw-rw-r--   0 wassef    (1000) wassef    (1000)      136 2024-05-14 19:55:25.000000 shared_cache-0.0.1/MANIFEST.in
--rw-r--r--   0 wassef    (1000) wassef    (1000)     2812 2024-05-15 05:39:14.081018 shared_cache-0.0.1/PKG-INFO
--rw-rw-r--   0 wassef    (1000) wassef    (1000)     2035 2024-05-14 21:57:11.000000 shared_cache-0.0.1/README.md
--rw-rw-r--   0 wassef    (1000) wassef    (1000)       98 2023-08-29 13:12:41.000000 shared_cache-0.0.1/pyproject.toml
--rw-rw-r--   0 wassef    (1000) wassef    (1000)      103 2024-05-14 20:55:30.000000 shared_cache-0.0.1/requirements-dev.txt
--rw-rw-r--   0 wassef    (1000) wassef    (1000)        0 2024-05-14 19:55:47.000000 shared_cache-0.0.1/requirements.txt
--rw-rw-r--   0 wassef    (1000) wassef    (1000)      861 2024-05-15 05:39:14.081018 shared_cache-0.0.1/setup.cfg
--rw-rw-r--   0 wassef    (1000) wassef    (1000)       74 2023-09-06 16:50:45.000000 shared_cache-0.0.1/setup.py
-drwxrwxr-x   0 wassef    (1000) wassef    (1000)        0 2024-05-15 05:39:14.081018 shared_cache-0.0.1/src/
-drwxrwxr-x   0 wassef    (1000) wassef    (1000)        0 2024-05-15 05:39:14.081018 shared_cache-0.0.1/src/shared_cache/
--rw-rw-r--   0 wassef    (1000) wassef    (1000)       99 2024-05-14 21:42:51.000000 shared_cache-0.0.1/src/shared_cache/__init__.py
--rw-rw-r--   0 wassef    (1000) wassef    (1000)     1973 2024-05-14 21:56:34.000000 shared_cache-0.0.1/src/shared_cache/service.py
--rw-rw-r--   0 wassef    (1000) wassef    (1000)     3609 2024-05-14 21:32:31.000000 shared_cache-0.0.1/src/shared_cache/shared.py
-drwxrwxr-x   0 wassef    (1000) wassef    (1000)        0 2024-05-15 05:39:14.081018 shared_cache-0.0.1/src/shared_cache.egg-info/
--rw-r--r--   0 wassef    (1000) wassef    (1000)     2812 2024-05-15 05:39:14.000000 shared_cache-0.0.1/src/shared_cache.egg-info/PKG-INFO
--rw-rw-r--   0 wassef    (1000) wassef    (1000)      457 2024-05-15 05:39:14.000000 shared_cache-0.0.1/src/shared_cache.egg-info/SOURCES.txt
--rw-rw-r--   0 wassef    (1000) wassef    (1000)        1 2024-05-15 05:39:14.000000 shared_cache-0.0.1/src/shared_cache.egg-info/dependency_links.txt
--rw-rw-r--   0 wassef    (1000) wassef    (1000)       47 2024-05-15 05:39:14.000000 shared_cache-0.0.1/src/shared_cache.egg-info/requires.txt
--rw-rw-r--   0 wassef    (1000) wassef    (1000)       13 2024-05-15 05:39:14.000000 shared_cache-0.0.1/src/shared_cache.egg-info/top_level.txt
-drwxrwxr-x   0 wassef    (1000) wassef    (1000)        0 2024-05-15 05:39:14.081018 shared_cache-0.0.1/tests/
--rw-rw-r--   0 wassef    (1000) wassef    (1000)     1430 2024-05-14 21:42:51.000000 shared_cache-0.0.1/tests/test_between_workers.py
--rw-rw-r--   0 wassef    (1000) wassef    (1000)     3515 2024-05-14 21:57:04.000000 shared_cache-0.0.1/tests/test_main.py
+drwxrwxr-x   0 wassef    (1000) wassef    (1000)        0 2024-05-18 21:20:17.902540 shared_cache-1.0.1/
+-rw-rw-r--   0 wassef    (1000) wassef    (1000)      894 2024-05-14 20:56:31.000000 shared_cache-1.0.1/.pre-commit-config.yaml
+-rw-rw-r--   0 wassef    (1000) wassef    (1000)     1072 2023-09-04 18:49:49.000000 shared_cache-1.0.1/LICENSE
+-rw-rw-r--   0 wassef    (1000) wassef    (1000)      136 2024-05-14 19:55:25.000000 shared_cache-1.0.1/MANIFEST.in
+-rw-r--r--   0 wassef    (1000) wassef    (1000)     2829 2024-05-18 21:20:17.902540 shared_cache-1.0.1/PKG-INFO
+-rw-rw-r--   0 wassef    (1000) wassef    (1000)     2053 2024-05-15 05:40:48.000000 shared_cache-1.0.1/README.md
+-rw-rw-r--   0 wassef    (1000) wassef    (1000)       98 2023-08-29 13:12:41.000000 shared_cache-1.0.1/pyproject.toml
+-rw-rw-r--   0 wassef    (1000) wassef    (1000)      103 2024-05-14 20:55:30.000000 shared_cache-1.0.1/requirements-dev.txt
+-rw-rw-r--   0 wassef    (1000) wassef    (1000)       15 2024-05-18 21:18:19.000000 shared_cache-1.0.1/requirements.txt
+-rw-rw-r--   0 wassef    (1000) wassef    (1000)      860 2024-05-18 21:20:17.906540 shared_cache-1.0.1/setup.cfg
+-rw-rw-r--   0 wassef    (1000) wassef    (1000)       74 2023-09-06 16:50:45.000000 shared_cache-1.0.1/setup.py
+drwxrwxr-x   0 wassef    (1000) wassef    (1000)        0 2024-05-18 21:20:17.898540 shared_cache-1.0.1/src/
+drwxrwxr-x   0 wassef    (1000) wassef    (1000)        0 2024-05-18 21:20:17.902540 shared_cache-1.0.1/src/shared_cache/
+-rw-rw-r--   0 wassef    (1000) wassef    (1000)       99 2024-05-18 21:19:07.000000 shared_cache-1.0.1/src/shared_cache/__init__.py
+-rw-rw-r--   0 wassef    (1000) wassef    (1000)     1971 2024-05-18 21:03:33.000000 shared_cache-1.0.1/src/shared_cache/service.py
+-rw-rw-r--   0 wassef    (1000) wassef    (1000)     3838 2024-05-18 21:06:20.000000 shared_cache-1.0.1/src/shared_cache/shared.py
+drwxrwxr-x   0 wassef    (1000) wassef    (1000)        0 2024-05-18 21:20:17.902540 shared_cache-1.0.1/src/shared_cache.egg-info/
+-rw-r--r--   0 wassef    (1000) wassef    (1000)     2829 2024-05-18 21:20:17.000000 shared_cache-1.0.1/src/shared_cache.egg-info/PKG-INFO
+-rw-rw-r--   0 wassef    (1000) wassef    (1000)      482 2024-05-18 21:20:17.000000 shared_cache-1.0.1/src/shared_cache.egg-info/SOURCES.txt
+-rw-rw-r--   0 wassef    (1000) wassef    (1000)        1 2024-05-18 21:20:17.000000 shared_cache-1.0.1/src/shared_cache.egg-info/dependency_links.txt
+-rw-rw-r--   0 wassef    (1000) wassef    (1000)       47 2024-05-18 21:20:17.000000 shared_cache-1.0.1/src/shared_cache.egg-info/requires.txt
+-rw-rw-r--   0 wassef    (1000) wassef    (1000)       13 2024-05-18 21:20:17.000000 shared_cache-1.0.1/src/shared_cache.egg-info/top_level.txt
+drwxrwxr-x   0 wassef    (1000) wassef    (1000)        0 2024-05-18 21:20:17.902540 shared_cache-1.0.1/tests/
+-rw-rw-r--   0 wassef    (1000) wassef    (1000)     1430 2024-05-14 21:42:51.000000 shared_cache-1.0.1/tests/test_between_workers.py
+-rw-rw-r--   0 wassef    (1000) wassef    (1000)     3515 2024-05-14 21:57:04.000000 shared_cache-1.0.1/tests/test_main.py
+-rw-rw-r--   0 wassef    (1000) wassef    (1000)      743 2024-05-18 21:08:05.000000 shared_cache-1.0.1/tests/test_shared_mem.py
```

### Comparing `shared_cache-0.0.1/.pre-commit-config.yaml` & `shared_cache-1.0.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `shared_cache-0.0.1/LICENSE` & `shared_cache-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `shared_cache-0.0.1/PKG-INFO` & `shared_cache-1.0.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: shared_cache
-Version: 0.0.1
+Version: 1.0.1
 Summary: Across workers shared cache for python3
 Home-page: https://github.com/wassef911/shared_cache
 Author: Wassef911
 Author-email: wassef911@gmail.com
 Keywords: python3,pypi,package
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.12.0
+Requires-Python: >=3.8.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: msgpack
 Provides-Extra: dev
 Requires-Dist: check-manifest; extra == "dev"
 Provides-Extra: test
 Requires-Dist: coverage; extra == "test"
@@ -39,15 +39,15 @@
 
 ```python
 # main.py
 from fastapi import FastAPI, HTTPException
 from pydantic import BaseModel
 from typing import Any, Hashable
 import asyncio
-from .models
+from .models import Item
 
 from shared_cache import Cache
 
 app = FastAPI()
 cache = Cache(maxsize=1_280_000) # in mb
 
 @app.on_event("startup")
@@ -83,15 +83,15 @@
 
 ### Testing the Package
 
 To test the `Cache` package, you can use the provided test suite. The tests include inter-process communication scenarios to ensure that the cache works correctly across multiple processes.
 
 1. **Run the Tests**:
    ```bash
-   pytest test_between_workers.py
+   pytest tests/test_between_workers.py
    ```
 
 ### Contributing
 
 Contributions are welcome! Please open an issue or submit a pull request on the [GitHub repository](https://github.com/wassef911/shared_cache).
 
 ### License
```

### Comparing `shared_cache-0.0.1/README.md` & `shared_cache-1.0.1/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 ```python
 # main.py
 from fastapi import FastAPI, HTTPException
 from pydantic import BaseModel
 from typing import Any, Hashable
 import asyncio
-from .models
+from .models import Item
 
 from shared_cache import Cache
 
 app = FastAPI()
 cache = Cache(maxsize=1_280_000) # in mb
 
 @app.on_event("startup")
@@ -60,15 +60,15 @@
 
 ### Testing the Package
 
 To test the `Cache` package, you can use the provided test suite. The tests include inter-process communication scenarios to ensure that the cache works correctly across multiple processes.
 
 1. **Run the Tests**:
    ```bash
-   pytest test_between_workers.py
+   pytest tests/test_between_workers.py
    ```
 
 ### Contributing
 
 Contributions are welcome! Please open an issue or submit a pull request on the [GitHub repository](https://github.com/wassef911/shared_cache).
 
 ### License
```

### Comparing `shared_cache-0.0.1/setup.cfg` & `shared_cache-1.0.1/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 [options]
 package_dir = 
 	= src
 packages = find:
 install_requires = 
 	msgpack
-python_requires = >=3.12.0
+python_requires = >=3.8.0
 
 [options.packages.find]
 where = src
 
 [options.extras_require]
 dev = 
 	check-manifest
```

### Comparing `shared_cache-0.0.1/src/shared_cache/service.py` & `shared_cache-1.0.1/src/shared_cache/service.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,10 @@
 from __future__ import annotations
-
 from typing import Any
 from typing import Hashable
-
 from .shared import SharedMemoryBackend
 
 
 class Cache:
     def __init__(
         self,
         maxsize=1024,
```

### Comparing `shared_cache-0.0.1/src/shared_cache/shared.py` & `shared_cache-1.0.1/src/shared_cache/shared.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from __future__ import annotations
-
+import collections
 import time
 from multiprocessing.shared_memory import SharedMemory
 from typing import Any
 from typing import Dict
 from typing import Hashable
 
 import msgpack
@@ -11,15 +11,15 @@
 
 class CacheItem:
     def __init__(self, value: Any, timestamp: float):
         self.value = value
         self.timestamp = timestamp
 
 
-class SharedMemoryBackend:
+class SharedMemoryBackend(collections.abc.MutableMapping[Hashable, Any]):
     _is_creator = False
 
     def __init__(self, maxsize=1024, shm_name="caching_service_memory"):
         self.memory_size = maxsize * 1024  # 1KB = 1024 bytes
         self.shm_name = shm_name
         try:
             self.shm = SharedMemory(
@@ -101,7 +101,16 @@
         except KeyError:
             return self.__missing__(key)
 
     def __setitem__(self, key: Hashable, value: Any):
         data = self.data
         data[key] = CacheItem(value, time.time())
         self.data = data
+
+    def __iter__(self):
+        return iter(self.data)
+
+    def __len__(self):
+        return len(self.data)
+
+    def __str__(self):
+        return str(self.data)
```

### Comparing `shared_cache-0.0.1/src/shared_cache.egg-info/PKG-INFO` & `shared_cache-1.0.1/src/shared_cache.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: shared_cache
-Version: 0.0.1
+Version: 1.0.1
 Summary: Across workers shared cache for python3
 Home-page: https://github.com/wassef911/shared_cache
 Author: Wassef911
 Author-email: wassef911@gmail.com
 Keywords: python3,pypi,package
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.12.0
+Requires-Python: >=3.8.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: msgpack
 Provides-Extra: dev
 Requires-Dist: check-manifest; extra == "dev"
 Provides-Extra: test
 Requires-Dist: coverage; extra == "test"
@@ -39,15 +39,15 @@
 
 ```python
 # main.py
 from fastapi import FastAPI, HTTPException
 from pydantic import BaseModel
 from typing import Any, Hashable
 import asyncio
-from .models
+from .models import Item
 
 from shared_cache import Cache
 
 app = FastAPI()
 cache = Cache(maxsize=1_280_000) # in mb
 
 @app.on_event("startup")
@@ -83,15 +83,15 @@
 
 ### Testing the Package
 
 To test the `Cache` package, you can use the provided test suite. The tests include inter-process communication scenarios to ensure that the cache works correctly across multiple processes.
 
 1. **Run the Tests**:
    ```bash
-   pytest test_between_workers.py
+   pytest tests/test_between_workers.py
    ```
 
 ### Contributing
 
 Contributions are welcome! Please open an issue or submit a pull request on the [GitHub repository](https://github.com/wassef911/shared_cache).
 
 ### License
```

### Comparing `shared_cache-0.0.1/tests/test_between_workers.py` & `shared_cache-1.0.1/tests/test_between_workers.py`

 * *Files identical despite different names*

### Comparing `shared_cache-0.0.1/tests/test_main.py` & `shared_cache-1.0.1/tests/test_main.py`

 * *Files identical despite different names*

