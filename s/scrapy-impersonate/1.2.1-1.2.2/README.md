# Comparing `tmp/scrapy_impersonate-1.2.1.tar.gz` & `tmp/scrapy_impersonate-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scrapy_impersonate-1.2.1.tar", last modified: Mon Apr 22 01:29:34 2024, max compression
+gzip compressed data, was "scrapy_impersonate-1.2.2.tar", last modified: Sat May 18 03:04:10 2024, max compression
```

## Comparing `scrapy_impersonate-1.2.1.tar` & `scrapy_impersonate-1.2.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 01:29:34.962652 scrapy_impersonate-1.2.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-04-22 01:29:27.000000 scrapy_impersonate-1.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5923 2024-04-22 01:29:34.962652 scrapy_impersonate-1.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5244 2024-04-22 01:29:27.000000 scrapy_impersonate-1.2.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-22 01:29:27.000000 scrapy_impersonate-1.2.1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 01:29:34.962652 scrapy_impersonate-1.2.1/scrapy_impersonate/
--rw-r--r--   0 runner    (1001) docker     (127)      177 2024-04-22 01:29:27.000000 scrapy_impersonate-1.2.1/scrapy_impersonate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2485 2024-04-22 01:29:27.000000 scrapy_impersonate-1.2.1/scrapy_impersonate/handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     3039 2024-04-22 01:29:27.000000 scrapy_impersonate-1.2.1/scrapy_impersonate/parser.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 01:29:34.962652 scrapy_impersonate-1.2.1/scrapy_impersonate.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5923 2024-04-22 01:29:34.000000 scrapy_impersonate-1.2.1/scrapy_impersonate.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      340 2024-04-22 01:29:34.000000 scrapy_impersonate-1.2.1/scrapy_impersonate.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-22 01:29:34.000000 scrapy_impersonate-1.2.1/scrapy_impersonate.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-22 01:29:34.000000 scrapy_impersonate-1.2.1/scrapy_impersonate.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-22 01:29:34.000000 scrapy_impersonate-1.2.1/scrapy_impersonate.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-22 01:29:34.962652 scrapy_impersonate-1.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      963 2024-04-22 01:29:27.000000 scrapy_impersonate-1.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 03:04:10.226354 scrapy_impersonate-1.2.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-05-18 03:04:02.000000 scrapy_impersonate-1.2.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5923 2024-05-18 03:04:10.226354 scrapy_impersonate-1.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5244 2024-05-18 03:04:02.000000 scrapy_impersonate-1.2.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-18 03:04:02.000000 scrapy_impersonate-1.2.2/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 03:04:10.222353 scrapy_impersonate-1.2.2/scrapy_impersonate/
+-rw-r--r--   0 runner    (1001) docker     (127)      177 2024-05-18 03:04:02.000000 scrapy_impersonate-1.2.2/scrapy_impersonate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2005 2024-05-18 03:04:02.000000 scrapy_impersonate-1.2.2/scrapy_impersonate/handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3039 2024-05-18 03:04:02.000000 scrapy_impersonate-1.2.2/scrapy_impersonate/parser.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 03:04:10.226354 scrapy_impersonate-1.2.2/scrapy_impersonate.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5923 2024-05-18 03:04:10.000000 scrapy_impersonate-1.2.2/scrapy_impersonate.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      340 2024-05-18 03:04:10.000000 scrapy_impersonate-1.2.2/scrapy_impersonate.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-18 03:04:10.000000 scrapy_impersonate-1.2.2/scrapy_impersonate.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-18 03:04:10.000000 scrapy_impersonate-1.2.2/scrapy_impersonate.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-18 03:04:10.000000 scrapy_impersonate-1.2.2/scrapy_impersonate.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-18 03:04:10.226354 scrapy_impersonate-1.2.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      963 2024-05-18 03:04:02.000000 scrapy_impersonate-1.2.2/setup.py
```

### Comparing `scrapy_impersonate-1.2.1/LICENSE` & `scrapy_impersonate-1.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `scrapy_impersonate-1.2.1/PKG-INFO` & `scrapy_impersonate-1.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scrapy-impersonate
-Version: 1.2.1
+Version: 1.2.2
 Summary: Scrapy download handler that can impersonate browser fingerprints
 Home-page: https://github.com/jxlil/scrapy-impersonate
 Author: Jalil SA (jxlil)
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `scrapy_impersonate-1.2.1/README.md` & `scrapy_impersonate-1.2.2/README.md`

 * *Files identical despite different names*

### Comparing `scrapy_impersonate-1.2.1/scrapy_impersonate/handler.py` & `scrapy_impersonate-1.2.2/scrapy_impersonate/handler.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,51 +1,45 @@
-from typing import Optional, Type, TypeVar
+from typing import Type, TypeVar
 
 from curl_cffi.requests import AsyncSession
-from scrapy import signals
 from scrapy.core.downloader.handlers.http import HTTPDownloadHandler
 from scrapy.crawler import Crawler
 from scrapy.http import Headers, Request, Response
 from scrapy.responsetypes import responsetypes
 from scrapy.spiders import Spider
-from scrapy.utils.defer import deferred_f_from_coro_f, deferred_from_coro
+from scrapy.utils.defer import deferred_f_from_coro_f
 from scrapy.utils.reactor import verify_installed_reactor
 from twisted.internet.defer import Deferred
 
 from scrapy_impersonate.parser import RequestParser
 
 ImpersonateHandler = TypeVar("ImpersonateHandler", bound="ImpersonateDownloadHandler")
 
 
 class ImpersonateDownloadHandler(HTTPDownloadHandler):
     def __init__(self, crawler) -> None:
         settings = crawler.settings
         super().__init__(settings=settings, crawler=crawler)
 
         verify_installed_reactor("twisted.internet.asyncioreactor.AsyncioSelectorReactor")
-        crawler.signals.connect(self._engine_started, signals.engine_started)
-
-        self.client: Optional[AsyncSession] = None
 
     @classmethod
     def from_crawler(cls: Type[ImpersonateHandler], crawler: Crawler) -> ImpersonateHandler:
         return cls(crawler)
 
-    @deferred_f_from_coro_f
-    async def _engine_started(self, signal, sender) -> None:
-        self.client = await AsyncSession().__aenter__()
-
     def download_request(self, request: Request, spider: Spider) -> Deferred:
         if request.meta.get("impersonate"):
-            return deferred_from_coro(self._download_request(request, spider))
+            return self._download_request(request, spider)
 
         return super().download_request(request, spider)
 
+    @deferred_f_from_coro_f
     async def _download_request(self, request: Request, spider: Spider) -> Response:
-        response = await self.client.request(**RequestParser(request).as_dict())  # type: ignore
+        async with AsyncSession() as client:
+            response = await client.request(**RequestParser(request).as_dict())  # type: ignore
 
         headers = Headers(response.headers)
         headers.pop("Content-Encoding", None)
 
         respcls = responsetypes.from_args(
             headers=headers,
             url=response.url,
@@ -56,15 +50,7 @@
             url=response.url,
             status=response.status_code,
             headers=headers,
             body=response.content,
             flags=["impersonate"],
             request=request,
         )
-
-    def close(self):
-        yield super().close()
-        yield self._close()
-
-    @deferred_f_from_coro_f
-    async def _close(self) -> None:
-        await self.client.__aexit__()  # type: ignore
```

### Comparing `scrapy_impersonate-1.2.1/scrapy_impersonate/parser.py` & `scrapy_impersonate-1.2.2/scrapy_impersonate/parser.py`

 * *Files identical despite different names*

### Comparing `scrapy_impersonate-1.2.1/scrapy_impersonate.egg-info/PKG-INFO` & `scrapy_impersonate-1.2.2/scrapy_impersonate.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scrapy-impersonate
-Version: 1.2.1
+Version: 1.2.2
 Summary: Scrapy download handler that can impersonate browser fingerprints
 Home-page: https://github.com/jxlil/scrapy-impersonate
 Author: Jalil SA (jxlil)
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `scrapy_impersonate-1.2.1/setup.py` & `scrapy_impersonate-1.2.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     long_description = f.read()
 
 with open("requirements.txt", "r") as f:
     requirements = f.read().splitlines()
 
 setup(
     name="scrapy-impersonate",
-    version="1.2.1",
+    version="1.2.2",
     author="Jalil SA (jxlil)",
     description="Scrapy download handler that can impersonate browser fingerprints",
     license="MIT",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/jxlil/scrapy-impersonate",
     packages=find_packages(),
```

