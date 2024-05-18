# Comparing `tmp/aiocmcapi-0.5.tar.gz` & `tmp/aiocmcapi-0.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiocmcapi-0.5.tar", last modified: Sat May 11 22:08:36 2024, max compression
+gzip compressed data, was "aiocmcapi-0.6.3.tar", last modified: Sat May 18 11:35:16 2024, max compression
```

## Comparing `aiocmcapi-0.5.tar` & `aiocmcapi-0.6.3.tar`

### file list

```diff
@@ -1,17 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-05-11 22:08:36.552824 aiocmcapi-0.5/
--rw-rw-rw-   0        0        0     1083 2024-05-11 19:33:44.000000 aiocmcapi-0.5/LICENSE
--rw-rw-rw-   0        0        0     2045 2024-05-11 22:08:36.552824 aiocmcapi-0.5/PKG-INFO
--rw-rw-rw-   0        0        0     1777 2024-05-11 21:20:54.000000 aiocmcapi-0.5/README.md
-drwxrwxrwx   0        0        0        0 2024-05-11 22:08:36.546824 aiocmcapi-0.5/aiocmcapi/
--rw-rw-rw-   0        0        0       61 2024-05-11 21:41:23.000000 aiocmcapi-0.5/aiocmcapi/__init__.py
--rw-rw-rw-   0        0        0      748 2024-05-11 19:22:47.000000 aiocmcapi-0.5/aiocmcapi/client.py
--rw-rw-rw-   0        0        0      922 2024-05-11 21:33:51.000000 aiocmcapi-0.5/aiocmcapi/currency.py
-drwxrwxrwx   0        0        0        0 2024-05-11 22:08:36.551824 aiocmcapi-0.5/aiocmcapi.egg-info/
--rw-rw-rw-   0        0        0     2045 2024-05-11 22:08:36.000000 aiocmcapi-0.5/aiocmcapi.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      269 2024-05-11 22:08:36.000000 aiocmcapi-0.5/aiocmcapi.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-11 22:08:36.000000 aiocmcapi-0.5/aiocmcapi.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2024-05-11 22:08:36.000000 aiocmcapi-0.5/aiocmcapi.egg-info/requires.txt
--rw-rw-rw-   0        0        0       26 2024-05-11 22:08:36.000000 aiocmcapi-0.5/aiocmcapi.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      410 2024-05-11 22:08:00.000000 aiocmcapi-0.5/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-11 22:08:36.553824 aiocmcapi-0.5/setup.cfg
--rw-rw-rw-   0        0        0      129 2024-05-11 22:08:31.000000 aiocmcapi-0.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-18 11:35:16.096276 aiocmcapi-0.6.3/
+-rw-rw-rw-   0        0        0     1083 2024-05-11 19:33:44.000000 aiocmcapi-0.6.3/LICENSE
+-rw-rw-rw-   0        0        0     2047 2024-05-18 11:35:16.095275 aiocmcapi-0.6.3/PKG-INFO
+-rw-rw-rw-   0        0        0     1777 2024-05-11 21:20:54.000000 aiocmcapi-0.6.3/README.md
+drwxrwxrwx   0        0        0        0 2024-05-18 11:35:16.094272 aiocmcapi-0.6.3/aiocmcapi.egg-info/
+-rw-rw-rw-   0        0        0     2047 2024-05-18 11:35:16.000000 aiocmcapi-0.6.3/aiocmcapi.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      218 2024-05-18 11:35:16.000000 aiocmcapi-0.6.3/aiocmcapi.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-18 11:35:16.000000 aiocmcapi-0.6.3/aiocmcapi.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2024-05-18 11:35:16.000000 aiocmcapi-0.6.3/aiocmcapi.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2024-05-18 11:35:16.000000 aiocmcapi-0.6.3/aiocmcapi.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      738 2024-05-12 15:05:54.000000 aiocmcapi-0.6.3/client.py
+-rw-rw-rw-   0        0        0     1057 2024-05-13 02:36:18.000000 aiocmcapi-0.6.3/currency.py
+-rw-rw-rw-   0        0        0      412 2024-05-18 11:34:02.000000 aiocmcapi-0.6.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-18 11:35:16.096276 aiocmcapi-0.6.3/setup.cfg
```

### Comparing `aiocmcapi-0.5/LICENSE` & `aiocmcapi-0.6.3/LICENSE`

 * *Files identical despite different names*

### Comparing `aiocmcapi-0.5/PKG-INFO` & `aiocmcapi-0.6.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiocmcapi
-Version: 0.5
+Version: 0.6.3
 Summary: Async wrapper for CoinMarketCap API
 Author-email: alobuzy <amozebus@gmail.com>
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: aiohttp>=3.9.5
```

### Comparing `aiocmcapi-0.5/README.md` & `aiocmcapi-0.6.3/README.md`

 * *Files identical despite different names*

### Comparing `aiocmcapi-0.5/aiocmcapi/client.py` & `aiocmcapi-0.6.3/client.py`

 * *Files 10% similar despite different names*

```diff
@@ -10,16 +10,16 @@
         )
     
     async def close_session(self):
         await self._session.connector.close()
         await self._session.close()
 
 class APIClient(BaseClient):
-    async def get(self, endpoint_path: str, params: dict = None) -> dict:
+    async def get(self, endpoint: str, params: dict = None) -> dict:
         async with self._session.get(
-            url=endpoint_path,
+            url=endpoint,
             params=params
         ) as r:
             json = await r.json()
             await self.close_session()
             
             return json
```

### Comparing `aiocmcapi-0.5/aiocmcapi/currency.py` & `aiocmcapi-0.6.3/currency.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,30 +1,38 @@
 from .client import APIClient
 
 class Currency:
     def __init__(self, cmc_id: int):
         self.name: str
+        self.slug: str
+        self.symbol: str
+
         self.price: float
         self.market_cap: float
+
         self.change_periods: dict
 
         self.data: dict
         self.cmc_id: int = cmc_id
 
     async def update(self, client: APIClient):
         json = await client.get(
-            endpoint_path="/v2/cryptocurrency/quotes/latest",
+            endpoint="/v2/cryptocurrency/quotes/latest",
             params={'id': self.cmc_id}
         )
         
         self.data = json['data'][str(self.cmc_id)]
         root = self.data['quote']['USD']
 
         self.name = self.data['name']
+        self.slug = self.data['slug']
+        self.symbol = self.data['symbol']
+
         self.price = root['price']
         self.market_cap = root['market_cap']
+
         self.change_periods = {
             '1h': root['percent_change_1h'],
             '24h': root['percent_change_24h'],
             '7d': root['percent_change_7d'],
             '30d': root['percent_change_30d']
         }
```

### Comparing `aiocmcapi-0.5/aiocmcapi.egg-info/PKG-INFO` & `aiocmcapi-0.6.3/aiocmcapi.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiocmcapi
-Version: 0.5
+Version: 0.6.3
 Summary: Async wrapper for CoinMarketCap API
 Author-email: alobuzy <amozebus@gmail.com>
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: aiohttp>=3.9.5
```

