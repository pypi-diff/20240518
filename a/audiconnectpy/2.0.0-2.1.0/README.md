# Comparing `tmp/audiconnectpy-2.0.0.tar.gz` & `tmp/audiconnectpy-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "audiconnectpy-2.0.0.tar", last modified: Wed May 15 16:11:03 2024, max compression
+gzip compressed data, was "audiconnectpy-2.1.0.tar", last modified: Sat May 18 12:04:44 2024, max compression
```

## Comparing `audiconnectpy-2.0.0.tar` & `audiconnectpy-2.1.0.tar`

### file list

```diff
@@ -1,40 +1,45 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 16:11:03.065575 audiconnectpy-2.0.0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 16:11:03.061576 audiconnectpy-2.0.0/.github/
--rw-r--r--   0 runner    (1001) docker     (127)      513 2024-05-15 16:10:51.000000 audiconnectpy-2.0.0/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 16:11:03.061576 audiconnectpy-2.0.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      656 2024-05-15 16:10:51.000000 audiconnectpy-2.0.0/.github/workflows/auto-approve.yml
--rw-r--r--   0 runner    (1001) docker     (127)      659 2024-05-15 16:10:51.000000 audiconnectpy-2.0.0/.github/workflows/pythonpackage.yml
--rw-r--r--   0 runner    (1001) docker     (127)      854 2024-05-15 16:10:51.000000 audiconnectpy-2.0.0/.github/workflows/pythonpublish.yml
--rw-r--r--   0 runner    (1001) docker     (127)      843 2024-05-15 16:10:51.000000 audiconnectpy-2.0.0/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1836 2024-05-15 16:10:51.000000 audiconnectpy-2.0.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1605 2024-05-15 16:10:51.000000 audiconnectpy-2.0.0/.pre-commit-config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 16:11:03.061576 audiconnectpy-2.0.0/.vscode/
--rw-r--r--   0 runner    (1001) docker     (127)      179 2024-05-15 16:10:51.000000 audiconnectpy-2.0.0/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-15 16:10:51.000000 audiconnectpy-2.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      151 2024-05-15 16:10:51.000000 audiconnectpy-2.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3757 2024-05-15 16:11:03.065575 audiconnectpy-2.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2809 2024-05-15 16:10:51.000000 audiconnectpy-2.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 16:11:03.065575 audiconnectpy-2.0.0/audiconnectpy/
--rw-r--r--   0 runner    (1001) docker     (127)      183 2024-05-15 16:10:51.000000 audiconnectpy-2.0.0/audiconnectpy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7739 2024-05-15 16:10:51.000000 audiconnectpy-2.0.0/audiconnectpy/api.py
--rw-r--r--   0 runner    (1001) docker     (127)    22121 2024-05-15 16:10:51.000000 audiconnectpy-2.0.0/audiconnectpy/auth.py
--rw-r--r--   0 runner    (1001) docker     (127)      993 2024-05-15 16:10:51.000000 audiconnectpy-2.0.0/audiconnectpy/const.py
--rw-r--r--   0 runner    (1001) docker     (127)      392 2024-05-15 16:10:51.000000 audiconnectpy-2.0.0/audiconnectpy/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     8076 2024-05-15 16:10:51.000000 audiconnectpy-2.0.0/audiconnectpy/helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     8861 2024-05-15 16:10:51.000000 audiconnectpy-2.0.0/audiconnectpy/model.py
--rw-r--r--   0 runner    (1001) docker     (127)    26295 2024-05-15 16:10:51.000000 audiconnectpy-2.0.0/audiconnectpy/vehicle.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 16:11:03.065575 audiconnectpy-2.0.0/audiconnectpy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3757 2024-05-15 16:11:03.000000 audiconnectpy-2.0.0/audiconnectpy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      759 2024-05-15 16:11:03.000000 audiconnectpy-2.0.0/audiconnectpy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 16:11:03.000000 audiconnectpy-2.0.0/audiconnectpy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 16:11:02.000000 audiconnectpy-2.0.0/audiconnectpy.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-15 16:11:03.000000 audiconnectpy-2.0.0/audiconnectpy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-15 16:11:03.000000 audiconnectpy-2.0.0/audiconnectpy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2486 2024-05-15 16:10:51.000000 audiconnectpy-2.0.0/example.py
--rw-r--r--   0 runner    (1001) docker     (127)     1476 2024-05-15 16:10:51.000000 audiconnectpy-2.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      120 2024-05-15 16:10:51.000000 audiconnectpy-2.0.0/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-15 16:10:51.000000 audiconnectpy-2.0.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-15 16:11:03.065575 audiconnectpy-2.0.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 16:11:03.065575 audiconnectpy-2.0.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      220 2024-05-15 16:10:51.000000 audiconnectpy-2.0.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1088 2024-05-15 16:10:51.000000 audiconnectpy-2.0.0/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 12:04:44.145530 audiconnectpy-2.1.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 12:04:44.141530 audiconnectpy-2.1.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      513 2024-05-18 12:04:33.000000 audiconnectpy-2.1.0/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 12:04:44.141530 audiconnectpy-2.1.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      656 2024-05-18 12:04:33.000000 audiconnectpy-2.1.0/.github/workflows/auto-approve.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      659 2024-05-18 12:04:33.000000 audiconnectpy-2.1.0/.github/workflows/pythonpackage.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      854 2024-05-18 12:04:33.000000 audiconnectpy-2.1.0/.github/workflows/pythonpublish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      843 2024-05-18 12:04:33.000000 audiconnectpy-2.1.0/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1827 2024-05-18 12:04:33.000000 audiconnectpy-2.1.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1605 2024-05-18 12:04:33.000000 audiconnectpy-2.1.0/.pre-commit-config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 12:04:44.141530 audiconnectpy-2.1.0/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (127)      179 2024-05-18 12:04:33.000000 audiconnectpy-2.1.0/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-18 12:04:33.000000 audiconnectpy-2.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      151 2024-05-18 12:04:33.000000 audiconnectpy-2.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3757 2024-05-18 12:04:44.145530 audiconnectpy-2.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2809 2024-05-18 12:04:33.000000 audiconnectpy-2.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 12:04:44.141530 audiconnectpy-2.1.0/audiconnectpy/
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2024-05-18 12:04:33.000000 audiconnectpy-2.1.0/audiconnectpy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7395 2024-05-18 12:04:33.000000 audiconnectpy-2.1.0/audiconnectpy/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20695 2024-05-18 12:04:33.000000 audiconnectpy-2.1.0/audiconnectpy/auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)      993 2024-05-18 12:04:33.000000 audiconnectpy-2.1.0/audiconnectpy/const.py
+-rw-r--r--   0 runner    (1001) docker     (127)      392 2024-05-18 12:04:33.000000 audiconnectpy-2.1.0/audiconnectpy/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7769 2024-05-18 12:04:33.000000 audiconnectpy-2.1.0/audiconnectpy/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8916 2024-05-18 12:04:33.000000 audiconnectpy-2.1.0/audiconnectpy/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25991 2024-05-18 12:04:33.000000 audiconnectpy-2.1.0/audiconnectpy/vehicle.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 12:04:44.145530 audiconnectpy-2.1.0/audiconnectpy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3757 2024-05-18 12:04:44.000000 audiconnectpy-2.1.0/audiconnectpy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      867 2024-05-18 12:04:44.000000 audiconnectpy-2.1.0/audiconnectpy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-18 12:04:44.000000 audiconnectpy-2.1.0/audiconnectpy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-18 12:04:43.000000 audiconnectpy-2.1.0/audiconnectpy.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-18 12:04:44.000000 audiconnectpy-2.1.0/audiconnectpy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-18 12:04:44.000000 audiconnectpy-2.1.0/audiconnectpy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1816 2024-05-18 12:04:33.000000 audiconnectpy-2.1.0/example.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1547 2024-05-18 12:04:33.000000 audiconnectpy-2.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-05-18 12:04:33.000000 audiconnectpy-2.1.0/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-18 12:04:33.000000 audiconnectpy-2.1.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-18 12:04:44.145530 audiconnectpy-2.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 12:04:44.145530 audiconnectpy-2.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      220 2024-05-18 12:04:33.000000 audiconnectpy-2.1.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1089 2024-05-18 12:04:33.000000 audiconnectpy-2.1.0/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 12:04:44.145530 audiconnectpy-2.1.0/tests/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (127)     2735 2024-05-18 12:04:33.000000 audiconnectpy-2.1.0/tests/fixtures/audi0.json
+-rw-r--r--   0 runner    (1001) docker     (127)      682 2024-05-18 12:04:33.000000 audiconnectpy-2.1.0/tests/fixtures/info_vehicles.json
+-rw-r--r--   0 runner    (1001) docker     (127)    62872 2024-05-18 12:04:33.000000 audiconnectpy-2.1.0/tests/fixtures/location.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4585 2024-05-18 12:04:33.000000 audiconnectpy-2.1.0/tests/test_home.py
```

### Comparing `audiconnectpy-2.0.0/.github/dependabot.yml` & `audiconnectpy-2.1.0/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `audiconnectpy-2.0.0/.github/workflows/auto-approve.yml` & `audiconnectpy-2.1.0/.github/workflows/auto-approve.yml`

 * *Files identical despite different names*

### Comparing `audiconnectpy-2.0.0/.github/workflows/pythonpackage.yml` & `audiconnectpy-2.1.0/.github/workflows/pythonpackage.yml`

 * *Files identical despite different names*

### Comparing `audiconnectpy-2.0.0/.github/workflows/pythonpublish.yml` & `audiconnectpy-2.1.0/.github/workflows/pythonpublish.yml`

 * *Files identical despite different names*

### Comparing `audiconnectpy-2.0.0/.github/workflows/release.yml` & `audiconnectpy-2.1.0/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `audiconnectpy-2.0.0/.gitignore` & `audiconnectpy-2.1.0/.gitignore`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 # Byte-compiled / optimized / DLL files
 __pycache__/
 *.py[cod]
 *$py.class
-example_home.py
 
 # C extensions
 *.so
 
 # Distribution / packaging
 .Python
 build/
@@ -125,9 +124,9 @@
 .mypy_cache/
 .dmypy.json
 dmypy.json
 
 # Pyre type checker
 .pyre/
 
-#perso
-test_home.py
+# Secret files
+secrets.yaml
```

### Comparing `audiconnectpy-2.0.0/.pre-commit-config.yaml` & `audiconnectpy-2.1.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `audiconnectpy-2.0.0/LICENSE` & `audiconnectpy-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `audiconnectpy-2.0.0/PKG-INFO` & `audiconnectpy-2.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: audiconnectpy
-Version: 2.0.0
+Version: 2.1.0
 Summary: Provides asynchronous authentication and access to Audi Connect
 Author-email: Cyr-ius <cyr-ius@ipocus.net>
 License: GPL-3
 Keywords: connect,async,audi
 Platform: any
 Classifier: Programming Language :: Python
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `audiconnectpy-2.0.0/README.md` & `audiconnectpy-2.1.0/README.md`

 * *Files identical despite different names*

### Comparing `audiconnectpy-2.0.0/audiconnectpy/api.py` & `audiconnectpy-2.1.0/audiconnectpy/api.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """Audi connect."""
 
 from __future__ import annotations
 
 from collections import namedtuple
 import logging
-from typing import Any, Tuple
+from typing import Any, NamedTuple
 
 from aiohttp import ClientSession
 
 from .auth import Auth
 from .const import (
     CLIENT_ID,
     MARKET_URL,
@@ -43,15 +43,15 @@
         Globals(unit_system)
         self.auth = Auth(session)
         self.country = country.upper()
         self._password = password
         self._username = username
         self._spin = spin
         self.is_connected: bool = False
-        self.vehicles: list[Vehicle] = None
+        self.vehicles: list[Vehicle] = []
         self.uris: dict[str, str] = {}
 
     async def async_login(self, vinlist: list[str] | None = None) -> None:
         """Login and retrieve tokens."""
 
         # Retrieve urls
         try:
@@ -68,25 +68,27 @@
                 self.is_connected = True
 
         # Update the state of all vehicles.
         if self.is_connected:
             try:
                 vehicles_response = await self.async_get_information_vehicles()
             except AudiException as error:
-                raise ("Error to get information vehicles (%s)", error) from error
+                raise AudiException(
+                    "Error to get information vehicles ({error})"
+                ) from error
             else:
                 obj_vehicles = Vehicles.from_dict(vehicles_response.get("data", []))
                 self.vehicles = obj_vehicles.user_vehicles
                 for vehicle in self.vehicles:
                     fill_region = await self._async_fill_url(vehicle.vin)
                     self.uris.update(fill_region._asdict())
                     # Add attributes to vehicle
                     vehicle.uris = self.uris
                     vehicle.auth = self.auth
-                    vehicle.spin = self._spin
+                    vehicle.spin = str(self._spin)
 
                     if vinlist is None or vehicle.vin.upper() in vinlist:
                         try:
                             # Fetch data for a vehicle
                             await vehicle.async_update()
                         except AudiException as error:
                             _LOGGER.error(
@@ -101,96 +103,92 @@
             token_type="audi",
             headers={
                 "Accept-Language": f"{self.uris['language']}-{self.country}",
                 "Content-Type": "application/json",
                 "X-User-Country": self.country,
             },
         )
-        query = {
+        data = {
             "query": "query vehicleList {\n userVehicles {\n vin\n mappingVin\n vehicle { core { modelYear\n }\n media { shortName\n longName }\n }\n csid\n commissionNumber\n type\n devicePlatform\n mbbConnect\n userRole {\n role\n }\n vehicle {\n classification {\n driveTrain\n }\n }\n nickname\n }\n}"
         }
         url = URL_INFO_VEHICLE if self.country != "US" else URL_INFO_VEHICLE_US
 
-        response = await self.auth.post(
-            url, data=query, headers=headers, allow_redirects=False
+        response = await self.auth.request(
+            "POST", url, json=data, headers=headers, allow_redirects=False
         )
         if "data" not in response:
             raise AudiException("Invalid json in vehicle information")
 
         return response
 
     async def _async_retrieve_url_service(self) -> None:
         """Get urls for request."""
         # Get markets to get language
         global URL_SERVICES
         country = self.country.upper()
-        markets_json = await self.auth.request("GET", f"{MARKET_URL}/markets", None)
+        markets_json = await self.auth.request("GET", f"{MARKET_URL}/markets")
 
-        country_spec = markets_json.getr("countries.countrySpecifications")
+        country_spec = ExtendedDict(markets_json).getr(
+            "countries.countrySpecifications"
+        )
         if country not in country_spec:
             raise AudiException("Country not found")
 
         language = country_spec[country].get("defaultLanguage")
 
-        # Get market config to get client_id , Authorization base url and mbbOAuth base url
+        # Get market config
         services = await self.auth.request(
-            "GET", f"{MARKET_URL}/market/{country}/{language}", None
+            "GET", f"{MARKET_URL}/market/{country}/{language}"
         )
 
         client_id = services.get("idkClientIDAndroidLive", CLIENT_ID)
         audi_baseurl = services.get(
             "myAudiAuthorizationServerProxyServiceURLProduction"
         )
         profil_url = (
             services.get("idkCustomerProfileMicroserviceBaseURLLive", "") + "/v3"
         )
         mbb_baseurl = services.get("mbbOAuthBaseURLLive", MBB_URL)
         cvvsb_base_url = services.get("connectedVehicleVehicleServiceBaseURLProduction")
 
-        _LOGGER.debug("Client id: %s", client_id)
-        _LOGGER.debug("Audi Base Url: %s", audi_baseurl)
-        _LOGGER.debug("Profil Base Url: %s", profil_url)
-        _LOGGER.debug("MBB Base Url: %s", mbb_baseurl)
-        _LOGGER.debug("ConnectedVehicle Base Url: %s", cvvsb_base_url)
-
-        # Get openId config to get authorizationEndpoint, tokenEndpoint, RevocationEndpoint
+        # Get openId config
         openid_url = services.get("idkLoginServiceConfigurationURLProduction")
         _LOGGER.debug("IDK Base Url: %s", openid_url)
-        openid_json = await self.auth.request("GET", openid_url, None)
+        openid_json = await self.auth.request("GET", openid_url)
 
         authorization_endpoint_url = openid_json.get("authorization_endpoint", "")
         token_endpoint_url = openid_json.get("token_endpoint", "")
         revocation_endpoint_url = openid_json.get("revocation_endpoint", "")
 
-        _LOGGER.debug("AuthEndpoint: %s", authorization_endpoint_url)
-        _LOGGER.debug("TokenEndpoint: %s", token_endpoint_url)
-        _LOGGER.debug("RevocationEndpoint: %s", revocation_endpoint_url)
-
         self.uris = {
             "client_id": client_id,
             "audi_url": audi_baseurl,
             "profil_url": profil_url,
             "mbb_url": mbb_baseurl,
             "here_url": URL_HERE_COM,
             "cv_url": cvvsb_base_url,
             "user_url": URL_INFO_USER,
             "authorization_endpoint": authorization_endpoint_url,
             "token_endpoint": token_endpoint_url,
+            "revocation_endpoint": revocation_endpoint_url,
             "language": language,
             "country": country,
         }
 
-    async def _async_fill_url(self, vin: str) -> Tuple[str, str]:
+        _LOGGER.debug("Urls of service: %s", self.uris)
+
+    async def _async_fill_url(self, vin: str) -> NamedTuple:
         """Fill region."""
         url = URL_HOME_REGION
         url_setter = URL_HOME_REGION_SETTER
-
-        rsp = await self.auth.get(f"{url_setter}/cs/vds/v1/vehicles/{vin}/homeRegion")
-        rsp = rsp if rsp else ExtendedDict()
-        uri = rsp.getr("homeRegion.baseUri.content")
+        headers = await self.auth.async_get_headers(token_type="mbb")
+        rsp = await self.auth.request(
+            "GET", f"{url_setter}/cs/vds/v1/vehicles/{vin}/homeRegion", headers=headers
+        )
+        uri = ExtendedDict(rsp).getr("homeRegion.baseUri.content")
         if uri and uri != url_setter:
             url = uri.replace("mal-", "fal-").replace("/api", "/fs-car")
             url_setter = uri
 
         FillRegion = namedtuple("FillRegion", ("url", "url_setter"))
 
         return FillRegion(url, url_setter)
```

### Comparing `audiconnectpy-2.0.0/audiconnectpy/auth.py` & `audiconnectpy-2.1.0/audiconnectpy/auth.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,26 +12,24 @@
 import re
 import socket
 from typing import Any, Literal
 from urllib.parse import parse_qs, urlencode, urlparse
 import uuid
 
 import aiohttp
-from aiohttp.hdrs import METH_GET, METH_POST, METH_PUT
 import async_timeout
 from bs4 import BeautifulSoup
 
 from .exceptions import (
     AudiException,
     AuthorizationError,
     HttpRequestError,
     ServiceNotFoundError,
     TimeoutExceededError,
 )
-from .helpers import ExtendedDict, json_loads
 
 TIMEOUT = 120
 DELAY = 10
 HDR_XAPP_VERSION = "4.24.2"
 HDR_USER_AGENT = "Android/4.24.2 (Build 800240338.root project 'onetouch-android'.ext.buildTime) Android/11"
 MARKET_URL = "https://content.app.my.audi.com/service/mobileapp/configurations"
 CLIENT_ID = "09b6cbec-cd19-4589-82fd-363dfa8c24da@apps_vw-dilab_com"
@@ -61,29 +59,25 @@
         self._audi_token: dict[str, str] = {}
         self.uris: dict[str, str] = {}
 
     async def request(
         self,
         method: str,
         url: str,
-        data: Any | None = None,
-        headers: dict[str, str] | None = None,
         raw_reply: bool = False,
         raw_rsp: bool = False,
         **kwargs: Any,
     ) -> Any:
         """Request url with method."""
         try:
             async with async_timeout.timeout(TIMEOUT):
-                _LOGGER.debug("REQUEST HEADERS: %s", headers)
+                _LOGGER.debug("REQUEST HEADERS: %s", kwargs.get("headers"))
                 _LOGGER.debug("REQUEST: %s", url)
-                _LOGGER.debug("REQUEST DATA:%s", data)
-                response = await self._session.request(
-                    method, url, headers=headers, data=data, **kwargs
-                )
+                _LOGGER.debug("REQUEST DATA:%s", kwargs.get("data"))
+                response = await self._session.request(method, url, **kwargs)
         except (asyncio.CancelledError, asyncio.TimeoutError) as error:
             raise TimeoutExceededError(
                 "Timeout occurred while connecting to Audi Connect."
             ) from error
         except (aiohttp.ClientError, socket.gaierror) as error:
             raise HttpRequestError(
                 "Error occurred while communicating with Audi Connect."
@@ -101,58 +95,29 @@
                 raise ServiceNotFoundError(response.status, json.loads(contents))
             raise ServiceNotFoundError(response.status, contents)
 
         if raw_reply and raw_rsp is False:
             return response
 
         if "application/json" in content_type:
-            rsp = await response.json(loads=json_loads)
+            rsp = await response.json()
         elif (
-            headers
+            (headers := kwargs.get("headers"))
             and "application/json" in headers.get("Accept", "")
             and contents == ""
         ):
             _LOGGER.debug("JSON FIX: Accept is JSON but Response is None")
-            rsp = ExtendedDict()
+            rsp = {}
         else:
             rsp = await response.text()
 
         if raw_reply and raw_rsp:
             return response, rsp
         return rsp
 
-    async def get(self, url: str, **kwargs: Any) -> Any:
-        """GET request."""
-        if (headers := kwargs.pop("headers", None)) is None:
-            headers = await self.async_get_headers(token_type="mbb")
-        response = await self.request(METH_GET, url, headers=headers, **kwargs)
-        return response
-
-    async def put(self, url: str, data: Any = None, **kwargs: Any) -> Any:
-        """PUT request."""
-        if (headers := kwargs.pop("headers", None)) is None:
-            headers = await self.async_get_headers(token_type="mbb")
-        response = await self.request(
-            METH_PUT, url, headers=headers, data=data, **kwargs
-        )
-        return response
-
-    async def post(
-        self, url: str, data: Any = None, use_json: bool = True, **kwargs: Any
-    ) -> Any:
-        """POST request."""
-        if (headers := kwargs.pop("headers", None)) is None:
-            headers = await self.async_get_headers(token_type="mbb")
-        if use_json and data:
-            data = json.dumps(data)
-        response = await self.request(
-            METH_POST, url, headers=headers, data=data, **kwargs
-        )
-        return response
-
     async def async_connect(
         self, username: str, password: str, uris: dict[str, str], tries: int = 3
     ) -> None:
         """Connect to API."""
         try:
             self.uris = uris
             await self._async_login(username, password)
@@ -196,29 +161,28 @@
             "code_challenge": code_challenge,
             "code_challenge_method": code_challenge_method,
             "ui_locales": f"{self.uris['language']}-{self.uris['language']} {self.uris['language']}",
         }
         idk_rsp, idk_rsptxt = await self.request(
             "GET",
             self.uris["authorization_endpoint"],
-            None,
             headers=headers,
             params=idk_data,
             raw_reply=True,
             raw_rsp=True,
         )
 
         # form_data with email
         submit_data = self._get_hidden_html_input_form_data(idk_rsptxt, {"email": user})
         submit_url = self._get_post_url(idk_rsptxt, self.uris["authorization_endpoint"])
         # send email
         email_rsptxt = await self.request(
             "POST",
             submit_url,
-            submit_data,
+            data=submit_data,
             headers=headers,
             cookies=idk_rsp.cookies,
             allow_redirects=True,
         )
 
         # form_data with password
         # 2022-01-29: new HTML response uses a js two build the html form data + button.
@@ -235,15 +199,15 @@
             )
             submit_url = self._get_post_url(email_rsptxt, submit_url)
 
         # send password
         pw_rsp = await self.request(
             "POST",
             submit_url,
-            submit_data,
+            data=submit_data,
             headers=headers,
             cookies=idk_rsp.cookies,
             allow_redirects=False,
             raw_reply=True,
         )
 
         pw_strings = parse_qs(urlparse(pw_rsp.headers.get("Location", {}))[4]).get(
@@ -251,37 +215,34 @@
         )
         self.user_id = pw_strings[0] if pw_strings else ""
 
         # forward1 after pwd
         fwd1_rsp = await self.request(
             "GET",
             pw_rsp.headers.get("Location", {}),
-            None,
             headers=headers,
             cookies=idk_rsp.cookies,
             allow_redirects=False,
             raw_reply=True,
         )
 
         # forward2 after pwd
         fwd2_rsp = await self.request(
             "GET",
             fwd1_rsp.headers.get("Location", {}),
-            None,
             headers=headers,
             cookies=idk_rsp.cookies,
             allow_redirects=False,
             raw_reply=True,
         )
 
         # get tokens
         codeauth_rsp = await self.request(
             "GET",
             fwd2_rsp.headers.get("Location", {}),
-            None,
             headers=headers,
             cookies=fwd2_rsp.cookies,
             allow_redirects=False,
             raw_reply=True,
         )
 
         authcode_parsed = urlparse(
@@ -475,15 +436,15 @@
             "token": kwargs.get("id_token"),
             "stage": "live",
             "config": "myaudi",
         }
         azs_token_json = await self.request(
             "POST",
             self.uris["audi_url"] + "/token",
-            json.dumps(asz_req_data),
+            json=asz_req_data,
             headers=headers,
             allow_redirects=False,
         )
         _LOGGER.debug("AZS Token: %s", azs_token_json)
         return azs_token_json
 
     async def _async_get_idk_token(self, **kwargs: Any) -> Any:
@@ -511,20 +472,20 @@
                 "response_type": "token id_token",
                 "code_verifier": kwargs.get("code_verifier"),
             }
 
         # IDK token request
         encoded_idk_data = urlencode(idk_data, encoding="utf-8").replace("+", "%20")
 
-        idk_token_json = await self.post(
+        idk_token_json = await self.request(
+            "POST",
             self.uris["token_endpoint"],
-            encoded_idk_data,
+            data=encoded_idk_data,
             headers=headers,
             allow_redirects=False,
-            use_json=False,
         )
         _LOGGER.debug("IDK Token: %s", idk_token_json)
 
         return idk_token_json
 
     async def _async_register_idk(self) -> str:
         """Register IDK.
@@ -542,17 +503,18 @@
             "client_name": "SM-A405FN",
             "platform": "google",
             "client_brand": "Audi",
             "appName": "myAudi",
             "appVersion": HDR_XAPP_VERSION,
             "appId": "de.myaudi.mobile.assistant",
         }
-        mbboauth_client_reg_json = await self.post(
+        mbboauth_client_reg_json = await self.request(
+            "POST",
             self.uris["mbb_url"] + "/mobile/register/v1",
-            mbboauth_reg_data,
+            json=mbboauth_reg_data,
             headers=headers,
             allow_redirects=False,
         )
         return str(mbboauth_client_reg_json.get("client_id", ""))
 
     async def _async_get_mbb_token(self, **kwargs: Any) -> Any:
         """Authentication to mbboauth-1d.prd.ece.vwg-connect.com."""
@@ -577,20 +539,20 @@
                 "grant_type": "id_token",
                 "token": kwargs.get("id_token"),
                 "scope": "sc2:fal",
             }
         encoded_mbboauth_data = urlencode(mbboauth_data, encoding="utf-8").replace(
             "+", "%20"
         )
-        mbboauth_json = await self.post(
+        mbboauth_json = await self.request(
+            "POST",
             self.uris["mbb_url"] + "/mobile/oauth2/v1/token",
-            encoded_mbboauth_data,
+            data=encoded_mbboauth_data,
             headers=headers,
             allow_redirects=False,
-            use_json=False,
         )
         _LOGGER.debug("MBB Token: %s", mbboauth_json)
         return mbboauth_json
 
     async def _async_get_here_token(self, **kwargs: Any) -> Any:
         """Authentication to Here.com."""
         headers = {
@@ -612,16 +574,16 @@
                 "token": kwargs.get("id_token"),
                 "scope": "sc2:here_a_t21-s",
             }
 
         encoded_hereoauth_data = urlencode(hereoauth_data, encoding="utf-8").replace(
             "+", "%20"
         )
-        hereoauth_json = await self.post(
+        hereoauth_json = await self.request(
+            "POST",
             self.uris["mbb_url"] + "/mobile/oauth2/v1/token",
-            encoded_hereoauth_data,
+            data=encoded_hereoauth_data,
             headers=headers,
             allow_redirects=False,
-            use_json=False,
         )
         _LOGGER.debug("Here Token: %s", hereoauth_json)
         return hereoauth_json
```

### Comparing `audiconnectpy-2.0.0/audiconnectpy/const.py` & `audiconnectpy-2.1.0/audiconnectpy/const.py`

 * *Files identical despite different names*

### Comparing `audiconnectpy-2.0.0/audiconnectpy/helpers.py` & `audiconnectpy-2.1.0/audiconnectpy/helpers.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 from __future__ import annotations
 
 from collections.abc import Callable
 from datetime import datetime
 import functools
 from functools import reduce
 from hashlib import sha512
-import json
 import logging
 import random
 import re
 import time
 from typing import Any
 
 from .exceptions import TimeoutExceededError
@@ -49,20 +48,14 @@
         try:
             obj[key] = datetime.strptime(val, "%Y-%m-%dT%H:%M:%S%z")
         except (TypeError, ValueError):
             pass
     return obj
 
 
-def json_loads(jsload: str | bytes) -> ExtendedDict:
-    """Json load."""
-    data_dict = json.loads(jsload)
-    return ExtendedDict(data_dict)
-
-
 def retry(
     exceptions: Any = Exception,
     tries: int = -1,
     delay: float = 0,
     max_delay: int | None = None,
     backoff: int = 1,
     jitter: int | tuple[int, int] = 0,
@@ -121,77 +114,71 @@
     """Generate security pin hash."""
     pin = to_byte_array(str(spin))
     byte_challenge = to_byte_array(challenge)
     b_pin = bytes(pin + byte_challenge)
     return sha512(b_pin).hexdigest().upper()
 
 
-def windows_status(attrs: ExtendedDict) -> ExtendedDict:
+def windows_status(attrs: list[dict[str, Any]]) -> dict[str, bool]:
     """Windows open status."""
-    attrs = map_name_status(attrs)
-    metadatas = ExtendedDict({})
-    left_open = "closed" not in attrs.get("frontLeft", [])
-    left_rear_open = "closed" not in attrs.get("rearLeft", [])
-    right_open = "closed" not in attrs.get("frontRight", [])
-    right_rear_open = "closed" not in attrs.get("rearRight", [])
+    status = map_name_status(attrs)
+    left_open = "closed" not in status.get("frontLeft", [])
+    left_rear_open = "closed" not in status.get("rearLeft", [])
+    right_open = "closed" not in status.get("frontRight", [])
+    right_rear_open = "closed" not in status.get("rearRight", [])
     windows_open = [left_open, left_rear_open, right_rear_open, right_rear_open]
-    metadatas.update(
-        {
-            "open_left_front_window": left_open,
-            "open_left_rear_window": left_rear_open,
-            "open_right_front_window": right_open,
-            "open_right_rear_window": right_rear_open,
-            "open_any_window": any(windows_open),
-        }
-    )
+    metadatas = {
+        "open_left_front_window": left_open,
+        "open_left_rear_window": left_rear_open,
+        "open_right_front_window": right_open,
+        "open_right_rear_window": right_rear_open,
+        "open_any_window": any(windows_open),
+    }
 
-    if "unsupported" not in attrs.get("roofCover", {}):
-        open_roof_cover = "closed" not in attrs.get("roofCover", [])
+    if "unsupported" not in status.get("roofCover", {}):
+        open_roof_cover = "closed" not in status.get("roofCover", [])
         metadatas.update({"open_roof_cover": open_roof_cover})
         windows_open.append(open_roof_cover)
 
-    if "unsupported" not in attrs.get("sunRoof", {}):
-        open_sun_roof = "closed" not in attrs.get("sunRoof", [])
+    if "unsupported" not in status.get("sunRoof", {}):
+        open_sun_roof = "closed" not in status.get("sunRoof", [])
         metadatas.update({"open_sun_roof": open_sun_roof})
         windows_open.append(open_sun_roof)
 
     metadatas.update({"open_any_window": any(windows_open)})
 
     return metadatas
 
 
-def doors_status(attrs: ExtendedDict) -> ExtendedDict:
+def doors_status(attrs: list[dict[str, Any]]) -> dict[str, bool]:
     """Doors lock status."""
-    attrs = map_name_status(attrs)
-    metadatas = ExtendedDict({})
-    left_unlock = "locked" not in attrs.get("frontLeft", [])
-    left_rear_unlock = "locked" not in attrs.get("rearLeft", [])
-    right_unlock = "locked" not in attrs.get("frontRight", [])
-    right_rear_unlock = "locked" not in attrs.get("rearRight", [])
-    trunk_unlock = "locked" not in attrs.get("trunk", [])
+    status = map_name_status(attrs)
+    left_unlock = "locked" not in status.get("frontLeft", [])
+    left_rear_unlock = "locked" not in status.get("rearLeft", [])
+    right_unlock = "locked" not in status.get("frontRight", [])
+    right_rear_unlock = "locked" not in status.get("rearRight", [])
+    trunk_unlock = "locked" not in status.get("trunk", [])
     doors_unlock = [left_unlock, left_rear_unlock, right_unlock, right_rear_unlock]
-    metadatas.update(
-        {
-            "lock_left_front_door": left_unlock,
-            "lock_left_rear_door": left_rear_unlock,
-            "lock_right_front_door": right_unlock,
-            "lock_right_rear_door": right_rear_unlock,
-            "lock_trunk": trunk_unlock,
-            "lock_any_door": any(doors_unlock),
-            "lock_doors_trunk": any(doors_unlock) and trunk_unlock,
-        }
-    )
+    metadatas = {
+        "lock_left_front_door": left_unlock,
+        "lock_left_rear_door": left_rear_unlock,
+        "lock_right_front_door": right_unlock,
+        "lock_right_rear_door": right_rear_unlock,
+        "lock_trunk": trunk_unlock,
+        "lock_any_door": any(doors_unlock),
+        "lock_doors_trunk": any(doors_unlock) and trunk_unlock,
+    }
 
     # Doors open status
-    left_open = "closed" not in attrs.get("frontLeft", [])
-    left_rear_open = "closed" not in attrs.get("rearLeft", [])
-    right_open = "closed" not in attrs.get("frontRight", [])
-    right_rear_open = "closed" not in attrs.get("rearRight", [])
-    trunk_open = "closed" not in attrs.get("trunk", [])
-    bonnet_open = "closed" not in attrs.get("bonnet", [])
+    left_open = "closed" not in status.get("frontLeft", [])
+    left_rear_open = "closed" not in status.get("rearLeft", [])
+    right_open = "closed" not in status.get("frontRight", [])
+    right_rear_open = "closed" not in status.get("rearRight", [])
+    trunk_open = "closed" not in status.get("trunk", [])
+    bonnet_open = "closed" not in status.get("bonnet", [])
     doors_open = [
         left_open,
         left_rear_open,
         right_open,
         right_rear_open,
         trunk_open,
         bonnet_open,
@@ -208,39 +195,36 @@
             "open_any_door": any(doors_open),
         }
     )
 
     return metadatas
 
 
-def lights_status(attrs: ExtendedDict) -> ExtendedDict:
-    attrs = map_name_status(attrs)
-    metadatas = ExtendedDict(
-        {
-            "left": attrs.get("left") != "off",
-            "right": attrs.get("right") != "off",
-        }
-    )
+def lights_status(attrs: list[dict[str, Any]]) -> dict[str, bool]:
+    status = map_name_status(attrs)
+    metadatas = {
+        "left": status.get("left") != "off",
+        "right": status.get("right") != "off",
+    }
 
     return metadatas
 
 
-def camel2snake(name):
+def camel2snake(name: str) -> str:
     """Camel case to Snake case."""
     return re.sub(r"(?<=[a-z])(?=[A-Z])|(?<=[A-Z])(?=[A-Z][a-z])", "_", name).lower()
 
 
-def remove_value(obj=dict[str, Any]) -> dict[str, Any]:
+def remove_value(obj: dict[str, Any]) -> dict[str, Any]:
     """Remove 'value' key in dictionary."""
     for k in obj.copy():
         if isinstance(obj[k], dict):
             for a, b in obj[k].items():
                 if data := b.pop("value", None):
                     obj[k][a] = data
 
     return obj
 
 
-def map_name_status(array: list[dict[str, Any]]) -> ExtendedDict:
+def map_name_status(array: list[dict[str, Any]]) -> dict[str, Any]:
     """Convert name/status to dictionary."""
-
-    return ExtendedDict({item.get("name"): item.get("status") for item in array})
+    return {item["name"]: item.get("status") for item in array}
```

### Comparing `audiconnectpy-2.0.0/audiconnectpy/model.py` & `audiconnectpy-2.1.0/audiconnectpy/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,32 +8,32 @@
 
 from mashumaro import DataClassDictMixin, field_options
 from mashumaro.types import SerializationStrategy
 
 from .helpers import camel2snake, doors_status, lights_status, windows_status
 
 
-class Locked(SerializationStrategy):
+class Locked(SerializationStrategy):  # type: ignore
     def serialize(self, value: str) -> str:
         return value
 
     def deserialize(self, value: str) -> bool:
         return value == "locked"
 
 
-class OnOff(SerializationStrategy):
+class OnOff(SerializationStrategy):  # type: ignore
     def serialize(self, value: str) -> str:
         return value
 
     def deserialize(self, value: str) -> bool:
         return value != "off"
 
 
 @dataclass
-class Base(DataClassDictMixin):
+class Base(DataClassDictMixin):  # type: ignore
     @classmethod
     def __pre_deserialize__(cls, d: dict[Any, Any]) -> dict[Any, Any]:
         return {camel2snake(k): v for k, v in d.items()}
 
 
 # SECTION
 @dataclass
@@ -223,15 +223,15 @@
     remaining_range_km: int | None = None
     current_fuel_level_pct: int | None = None
 
 
 @dataclass
 class SecondaryEngine(Base):
     type: str | None = None
-    current_soc_pct: str = None
+    current_soc_pct: int | None = None
     remaining_range_km: int | None = None
     current_fuel_level_pct: int | None = None
 
 
 # SECTION
 @dataclass
 class OilLevel(Base):
```

### Comparing `audiconnectpy-2.0.0/audiconnectpy/vehicle.py` & `audiconnectpy-2.1.0/audiconnectpy/vehicle.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 """Vehicle class."""
 
 from __future__ import annotations
 
 import asyncio
 from dataclasses import dataclass, field
 from datetime import datetime
+import json
 import logging
-from typing import Any, Literal
+from typing import Any, Iterable, Literal, cast
 
 from mashumaro import DataClassDictMixin, field_options
 
 from .const import (
     BRAND,
     FAILED,
     MAX_RESPONSE_ATTEMPTS,
@@ -28,42 +29,42 @@
 
 
 class Globals:
     """Global variables."""
 
     def __init__(self, unit: str) -> None:
         """Initilaze."""
-        global UNIT_SYSTEM  # pylint: disable=global-variable-undefined
+        global UNIT_SYSTEM
         UNIT_SYSTEM = f"{unit}"  # type: ignore
 
 
 @dataclass
-class Vehicles(DataClassDictMixin):
+class Vehicles(DataClassDictMixin):  # type: ignore
     """Vehicles."""
 
     user_vehicles: list[Vehicle] = field(
-        metadata=field_options(alias="userVehicles"), default=None
+        metadata=field_options(alias="userVehicles"), default_factory=list
     )
 
 
 @dataclass
-class Vehicle(DataClassDictMixin):
+class Vehicle(DataClassDictMixin):  # type: ignore
     """Vehicle class."""
 
     vin: str
     csid: str
     nickname: str | None = None
     last_access: datetime | None = None
     uris: dict[str, str] = field(init=False)
     spin: str = field(init=False)
-    auth: str = field(init=False)
+    auth: Any = field(init=False)
     infos: dict[str, Any] | None = field(
         metadata=field_options(alias="vehicle"), default=None
     )
-    capabilities: dict[str, Any] | None = field(init=False, default=None)
+    capabilities: list[str] | None = field(init=False, default=None)
     position: Position | None = field(init=False, default=None)
     location: Location | None = field(init=False, default=None)
 
     @property
     def api_level(self) -> dict[str, int]:
         """Return API Level."""
         return {
@@ -117,60 +118,62 @@
                     item
                     for item in location.get("data", [])
                     if "proprietaryData" in item
                 ],
             }
         )
 
-    async def async_get_location(self) -> ExtendedDict:
+    async def async_get_location(self) -> Any:
         """Get destination data."""
         headers = await self.auth.async_get_headers(token_type="here")
-        data = await self.auth.get(f"{self.uris['here_url']}/location", headers=headers)
+        data = await self.auth.request(
+            "GET", f"{self.uris['here_url']}/location", headers=headers
+        )
         return data
 
-    async def async_get_position(self) -> ExtendedDict:
+    async def async_get_position(self) -> Any:
         """Get position data."""
         headers = await self.auth.async_get_headers(token_type="idk")
-        data = await self.auth.get(
+        data = await self.auth.request(
+            "GET",
             f"{self.uris['cv_url']}/vehicles/{self.vin}/parkingposition",
             headers=headers,
         )
         return data
 
-    async def async_get_capabilities(self) -> ExtendedDict:
+    async def async_get_capabilities(self) -> Any:
         """Get capabilities."""
         headers = await self.auth.async_get_headers(token_type="idk")
-        data = await self.auth.get(
+        data = await self.auth.request(
+            "GET",
             f"{self.uris['cv_url']}/vehicles/{self.vin}/capabilities",
             headers=headers,
         )
         return data
 
-    async def async_get_selectivestatus(
-        self, jobs: list[str] | None = None
-    ) -> ExtendedDict:
+    async def async_get_selectivestatus(self, jobs: Iterable[str] | None = None) -> Any:
         """Get capabilities."""
-        if not jobs:
+        if jobs is None:
             headers = await self.auth.async_get_headers(token_type="idk")
-            capabilities = await self.auth.get(
+            capabilities = await self.auth.request(
+                "GET",
                 f"{self.uris['cv_url']}/vehicles/{self.vin}/selectivestatus?jobs=userCapabilities",
                 headers=headers,
             )
-            dict_values = (
-                capabilities.get("userCapabilities", {})
-                .get("capabilitiesStatus", {})
-                .get("value", [])
+            values: list[dict[str, Any]] = ExtendedDict(capabilities).getr(
+                "userCapabilities.capabilitiesStatus.value", []
             )
-            self.capabilities = [
-                d for capability in dict_values if (d := capability.get("id"))
+            self.capabilities: list[str] = [
+                str(d) for capability in values if (d := capability.get("id"))
             ]
 
-        str_jobs = ",".join(self.capabilities)
+        str_jobs = ",".join(self.capabilities)  # type: ignore
         headers = await self.auth.async_get_headers(token_type="idk")
-        data = await self.auth.get(
+        data = await self.auth.request(
+            "GET",
             f"{self.uris['cv_url']}/vehicles/{self.vin}/selectivestatus?jobs={str_jobs},userCapabilities",
             headers=headers,
         )
         return data
 
     async def async_set_lock(self, lock: bool) -> None:
         """Set lock."""
@@ -182,22 +185,21 @@
             security_token,
         )
         data: str | dict[str, Any] = (
             '<?xml version="1.0" encoding= "UTF-8" ?>'
             + f'<rluAction xmlns="http://audi.de/connect/rlu"><action>{"lock" if lock else "unlock"}</action></rluAction>'
         )
 
-        rsp = await self.auth.post(
+        rsp = await self.auth.request(
+            "POST",
             f"{self.uris['url']}/bs/rlu/v1/{BRAND}/{self.uris['country']}/vehicles/{self.vin}/actions",
             headers=headers,
             data=data,
-            use_json=False,
         )
-        rsp = rsp if rsp else ExtendedDict()
-        request_id = rsp.getr("rluActionResponse.requestId")
+        request_id = ExtendedDict(rsp).getr("rluActionResponse.requestId", "")
         await self._async_check_request(
             f"{self.uris['url']}/bs/rlu/v1/{BRAND}/{self.uris['country']}/vehicles/{self.vin}/requests/{request_id}/status",
             "lock vehicle" if lock else "unlock vehicle",
             REQUEST_SUCCESSFUL,
             REQUEST_FAILED,
             "requestStatusResponse.status",
         )
@@ -224,15 +226,14 @@
                 heater_source != "electric",
             )
             data: str | dict[str, Any] = (
                 f'<?xml version="1.0" encoding="UTF-8"?><action><type>{"startClimatisation" if start else "stopClimatisation"}</type><settings><heaterSource>'
                 + heater_source
                 + "</heaterSource></settings></action>"
             )
-            use_json = False
         else:
             headers = await self.auth.async_get_action_headers(
                 "application/json",
                 security_token,
                 heater_source != "electric",
             )
             data = (
@@ -249,24 +250,23 @@
                             },
                         },
                     }
                 }
                 if start
                 else {"action": {"type": "stopClimatisation"}}
             )
-            use_json = True
+            data = json.dumps(data)
 
-        rsp = await self.auth.post(
+        rsp = await self.auth.request(
+            "POST",
             f"{self.uris['url']}/bs/climatisation/v1/{BRAND}/{self.uris['country']}/vehicles/{self.vin}/climater/actions",
             headers=headers,
             data=data,
-            use_json=use_json,
         )
-        rsp = rsp if rsp else ExtendedDict()
-        actionid = rsp.getr("action.actionId")
+        actionid = ExtendedDict(rsp).getr("action.actionId", "")
         await self._async_check_request(
             f"{self.uris['url']}/bs/climatisation/v1/{BRAND}/{self.uris['country']}/vehicles/{self.vin}/climater/actions/{actionid}",
             "start climatisation" if start else "stop climatisation",
             SUCCEEDED,
             FAILED,
             "action.actionState",
         )
@@ -302,15 +302,14 @@
             data: str | dict[str, Any] = (
                 '<?xml version="1.0" encoding="UTF-8"?><action><type>setSettings</type><settings>'
                 + f"<targetTemperature>{temperature}</targetTemperature>"
                 + "<climatisationWithoutHVpower>false</climatisationWithoutHVpower>"
                 + f"<heaterSource>{heater_source}</heaterSource>"
                 + "</settings></action>"
             )
-            use_json = False
         else:
             headers = await self.auth.async_get_action_headers("application/json", None)
             data = {
                 "action": {
                     "type": "setSettings",
                     "settings": {
                         "targetTemperature": temperature,
@@ -320,23 +319,22 @@
                             "isClimatisationAtUnlock": False,
                             "isMirrorHeatingEnabled": glass_heating,
                             "zoneSettings": {"zoneSetting": zone_settings},
                         },
                     },
                 }
             }
-            use_json = True
-        rsp = await self.auth.post(
+            data = json.dumps(data)
+        rsp = await self.auth.request(
+            "POST",
             f"{self.uris['url']}/bs/climatisation/v1/{BRAND}/{self.uris['country']}/vehicles/{self.vin}/climater/actions",
             headers=headers,
             data=data,
-            use_json=use_json,
         )
-        rsp = rsp if rsp else ExtendedDict()
-        actionid = rsp.getr("action.actionId")
+        actionid = ExtendedDict(rsp).getr("action.actionId", "")
         await self._async_check_request(
             f"{self.uris['url']}/bs/climatisation/v1/{BRAND}/{self.uris['country']}/vehicles/{self.vin}/climater/actions/{actionid}",
             "set target temperature",
             SUCCEEDED,
             FAILED,
             "action.actionState",
         )
@@ -350,15 +348,14 @@
             headers = await self.auth.async_get_action_headers(
                 "application/vnd.vwg.mbb.RemoteStandheizung_v2_0_0+xml", security_token
             )
             data: str | dict[str, Any] = (
                 '<?xml version="1.0" encoding= "UTF-8" ?><performAction xmlns="http://audi.de/connect/rs">'
                 + f'<quickstart><active>{"true" if start else "false"}</active></quickstart></performAction>'
             )
-            use_json = False
         else:
             headers = await self.auth.async_get_action_headers(
                 "application/json", security_token
             )
             data = (
                 {
                     "performAction": {
@@ -368,21 +365,21 @@
                             "climatisationDuration": duration,
                         }
                     }
                 }
                 if start
                 else {"performAction": {"quickstop": {"active": False}}}
             )
-            use_json = True
+            data = json.dumps(data)
 
-        await self.auth.post(
+        await self.auth.request(
+            "POST",
             f"{self.uris['url']}/bs/rs/v1/{BRAND}/{self.uris['country']}/vehicles/{self.vin}/action",
             headers=headers,
             data=data,
-            use_json=use_json,
         )
 
     async def async_set_ventilation(self, start: bool, duration: int = 60) -> None:
         """Set ventilation."""
         security_token = await self._async_get_security_token(
             "rheating_v1/operations/" + ("P_QSACT" if start else "P_QSTOPACT")
         )
@@ -399,15 +396,14 @@
                 if start
                 else "<active>false</active>"
             )
             data: str | dict[str, Any] = (
                 '<?xml version="1.0" encoding="UTF-8" ?><performAction xmlns="http://audi.de/connect/rs">'
                 f"<quickstart>{content}</quickstart></performAction>"
             )
-            use_json = False
         else:
             headers = await self.auth.async_get_action_headers(
                 "application/vnd.vwg.mbb.RemoteStandheizung_v2_0_2+json", security_token
             )
             data = (
                 {
                     "performAction": {
@@ -417,21 +413,21 @@
                             "climatisationDuration": duration,
                         }
                     }
                 }
                 if start
                 else {"performAction": {"quickstop": {"active": False}}}
             )
-            use_json = True
+            data = json.dumps(data)
 
-        await self.auth.post(
+        await self.auth.request(
+            "POST",
             f"{self.uris['url']}/bs/rs/v1/{BRAND}/{self.uris['country']}/vehicles/{self.vin}/action",
             headers=headers,
             data=data,
-            use_json=use_json,
         )
 
     async def async_set_battery_charger(self, start: bool, timer: bool = False) -> None:
         """Set battery charger."""
         if self.api_level["charger"] == 2:
             headers = await self.auth.async_get_action_headers("application/json", None)
             if start and timer:
@@ -443,38 +439,36 @@
                         },
                     }
                 }
             elif start:
                 data = {"action": {"type": "start"}}
             else:
                 data = {"action": {"type": "stop"}}
-            use_json = True
+            data = json.dumps(data)
         elif self.api_level["charger"] == 3:
             headers = await self.auth.async_get_action_headers("application/json", None)
             data = {
                 "action": {
                     "type": "startBatteryCharging" if start else "stopBatteryCharging"
                 }
             }
-            use_json = True
+            data = json.dumps(data)
         else:
             headers = await self.auth.async_get_action_headers(
                 "application/vnd.vwg.mbb.ChargerAction_v1_0_0+xml", None
             )
             data = f'<?xml version="1.0" encoding="UTF-8" ?><action><type>{"start" if start else "stop"}</type></action>'
-            use_json = False
 
-        rsp = await self.auth.post(
+        rsp = await self.auth.request(
+            "POST",
             f"{self.uris['url']}/bs/batterycharge/v1/{BRAND}/{self.uris['country']}/vehicles/{self.vin}/charger/actions",
             headers=headers,
             data=data,
-            use_json=use_json,
         )
-        rsp = rsp if rsp else ExtendedDict()
-        actionid = rsp.getr("action.actionId")
+        actionid = ExtendedDict(rsp).getr("action.actionId", "")
         await self._async_check_request(
             f"{self.uris['url']}/bs/batterycharge/v1/{BRAND}/{self.uris['country']}/vehicles/{self.vin}/charger/actions/{actionid}",
             "start charger" if start else "stop charger",
             SUCCEEDED,
             FAILED,
             "action.actionState",
         )
@@ -485,33 +479,32 @@
             headers = await self.auth.async_get_action_headers("application/json", None)
             data: str | dict[str, Any] = {
                 "action": {
                     "settings": {"maxChargeCurrent": int(current)},
                     "type": "setSettings",
                 }
             }
-            use_json = True
+            data = json.dumps(data)
+
         else:
             headers = await self.auth.async_get_action_headers(
                 "application/vnd.vwg.mbb.ChargerAction_v1_0_0+xml", None
             )
             data = (
                 '<?xml version="1.0" encoding="UTF-8" ?><action><type>setSettings</type>'
                 + f"<settings><maxChargeCurrent>{current}</maxChargeCurrent></settings></action>"
             )
-            use_json = False
 
-        rsp = await self.auth.post(
+        rsp = await self.auth.request(
+            "POST",
             f"{self.uris['url']}/bs/batterycharge/v1/{BRAND}/{self.uris['country']}/vehicles/{self.vin}/charger/actions",
             headers=headers,
             data=data,
-            use_json=use_json,
         )
-        rsp = rsp if rsp else ExtendedDict()
-        actionid = rsp.getr("action.actionId")
+        actionid = ExtendedDict(rsp).getr("action.actionId", "")
         await self._async_check_request(
             f"{self.uris['url']}/bs/batterycharge/v1/{BRAND}/{self.uris['country']}/vehicles/{self.vin}/charger/actions/{actionid}",
             "set charger max current",
             SUCCEEDED,
             FAILED,
             "action.actionState",
         )
@@ -521,77 +514,72 @@
         if self.api_level["windows_heating"] == 2:
             headers = await self.auth.async_get_action_headers("application/json", None)
             data: str | dict[str, Any] = {
                 "action": {
                     "type": "startWindowHeating" if start else "stopWindowHeating"
                 }
             }
-            use_json = True
+            data = json.dumps(data)
         else:
             headers = await self.auth.async_get_action_headers(
                 "application/vnd.vwg.mbb.ClimaterAction_v1_0_0+xml", None
             )
             data = (
                 '<?xml version="1.0" encoding= "UTF-8" ?>'
                 + f"<action><type>{'startWindowHeating' if start else 'stopWindowHeating'}</type></action>"
             )
-            use_json = False
-        rsp = await self.auth.post(
+        rsp = await self.auth.request(
+            "POST",
             f"{self.uris['url']}/bs/climatisation/v1/{BRAND}/{self.uris['country']}/vehicles/{self.vin}/climater/actions",
             headers=headers,
             data=data,
-            use_json=use_json,
         )
-        rsp = rsp if rsp else ExtendedDict()
-        actionid = rsp.getr("action.actionId")
+        actionid = ExtendedDict(rsp).getr("action.actionId", "")
         await self._async_check_request(
             f"{self.uris['url']}/bs/climatisation/v1/{BRAND}/{self.uris['country']}/vehicles/{self.vin}/climater/actions/{actionid}",
             "start window heating" if start else "stop window heating",
             SUCCEEDED,
             FAILED,
             "action.actionState",
         )
 
     async def async_set_honkflash(
         self, mode: Literal["honk", "flash"], duration: int = 15
     ) -> None:
         """Set honk and flash light."""
-        rsp_position = await self.auth.get(
-            f"{self.uris['url']}/bs/cf/v1/{BRAND}/{self.uris['country']}/vehicles/{self.vin}/position"
-        )
-        rsp_position = rsp_position if rsp_position else ExtendedDict()
-        position = rsp_position.getr("findCarResponse.Position.carCoordinate")
-        headers = await self.auth.async_get_action_headers("application/json", None)
-        data: str | dict[str, Any] = {
-            "honkAndFlashRequest": {
-                "serviceOperationCode": "HONK_AND_FLASH"
-                if mode == "honk"
-                else "FLASH_ONLY",
-                "serviceDuration": duration,
-                "userPosition": {
-                    "latitude": position["latitude"],
-                    "longitude": position["longitude"],
-                },
+        if self.position:
+            headers = await self.auth.async_get_action_headers("application/json", None)
+            data: dict[str, Any] = {
+                "honkAndFlashRequest": {
+                    "serviceOperationCode": "HONK_AND_FLASH"
+                    if mode == "honk"
+                    else "FLASH_ONLY",
+                    "serviceDuration": duration,
+                    "userPosition": {
+                        "latitude": self.position.latitude,
+                        "longitude": self.position.longitude,
+                    },
+                }
             }
-        }
-        await self.auth.post(
-            f"{self.uris['url']}/bs/rhf/v1/{BRAND}/{self.uris['country']}/vehicles/{self.vin}/honkAndFlash",
-            headers=headers,
-            data=data,
-        )
+            await self.auth.request(
+                "POST",
+                f"{self.uris['url']}/bs/rhf/v1/{BRAND}/{self.uris['country']}/vehicles/{self.vin}/honkAndFlash",
+                headers=headers,
+                json=data,
+            )
 
     async def async_refresh_vehicle_data(self) -> None:
         """Refresh vehicle data."""
         headers = await self.auth.async_get_headers(token_type="idk")
-        data = await self.auth.post(
+        rsp = await self.auth.request(
+            "POST",
             f"{self.uris['cv_url']}/vehicles/{self.vin}/vehiclewakeup",
             headers=headers,
         )
-        data = data if data else ExtendedDict()
-        request_id: str = data.getr("data.requestID")
+        request_id: str = ExtendedDict(rsp).getr("data.requestID", "")
         await self._async_pending_request(
             f"{self.uris['cv_url']}/vehicles/{self.vin}/pendingrequests",
             "refresh vehicle data",
             SUCCESSFUL,
             FAILED,
             request_id,
         )
@@ -601,15 +589,15 @@
     ) -> None:
         """Check request succeeded."""
         stauts_good = False
         for _ in range(MAX_RESPONSE_ATTEMPTS):
             await asyncio.sleep(REQUEST_STATUS_SLEEP)
 
             headers = await self.auth.async_get_headers(token_type="idk")
-            rsp = await self.auth.get(url, headers=headers)
+            rsp = await self.auth.request("GET", url, headers=headers)
 
             status = None
             if rsp and (data := rsp.get("data")):
                 for item in data:
                     if item.get("id") == request_id:
                         status = item.get("status")
                         break
@@ -628,56 +616,57 @@
         self, url: str, action: str, success: str, failed: str, path: str
     ) -> None:
         """Check request succeeded."""
         stauts_good = False
         for _ in range(MAX_RESPONSE_ATTEMPTS):
             await asyncio.sleep(REQUEST_STATUS_SLEEP)
 
-            rsp = await self.auth.get(url)
+            headers = await self.auth.async_get_headers(token_type="mbb")
+            rsp = await self.auth.request("GET", url, headers=headers)
 
-            status = rsp.getr(path)
+            status = ExtendedDict(rsp).getr(path)
 
             if status is None or (failed is not None and status == failed):
                 raise HttpRequestError(("Cannot %s, return code '%s'", action, status))
 
             if status == success:
                 stauts_good = True
                 break
 
         if stauts_good is False:
             raise TimeoutExceededError(("Cannot %s, operation timed out", action))
 
-    async def _async_get_security_token(self, action: str) -> Any:
+    async def _async_get_security_token(self, action: str) -> str:
         """Get security token."""
         self.spin = "" if self.spin is None else self.spin
 
         # Challenge
         headers = await self.auth.async_get_headers(token_type="mbb", okhttp=True)
-        rsp = await self.auth.get(
+        rsp = await self.auth.request(
+            "GET",
             f"{self.uris['url_setter']}/rolesrights/authorization/v2/vehicles/{self.vin}/services/{action}/security-pin-auth-requested",
             headers=headers,
         )
-        rsp = rsp if rsp else ExtendedDict()
-        sec_token = rsp.getr("securityPinAuthInfo.securityToken")
+        rsp = ExtendedDict(rsp)
+        sec_token: str = rsp.getr("securityPinAuthInfo.securityToken")
         challenge: str = rsp.getr(
             "securityPinAuthInfo.securityPinTransmission.challenge"
         )
 
         # Response
-        security_pin_hash = spin_hash(self.spin, challenge)
+        headers["Content-Type"] = "application/json"
         data = {
             "securityPinAuthentication": {
                 "securityPin": {
                     "challenge": challenge,
-                    "securityPinHash": security_pin_hash,
+                    "securityPinHash": spin_hash(self.spin, challenge),
                 },
                 "securityToken": sec_token,
             }
         }
-
-        headers["Content-Type"] = "application/json"
-        body = await self.auth.post(
+        response = await self.auth.request(
+            "POST",
             f"{self.uris['url_setter']}/rolesrights/authorization/v2/security-pin-auth-completed",
             headers=headers,
-            data=data,
+            json=data,
         )
-        return body["securityToken"]
+        return cast(str, response.get("securityToken", ""))
```

### Comparing `audiconnectpy-2.0.0/audiconnectpy.egg-info/PKG-INFO` & `audiconnectpy-2.1.0/audiconnectpy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: audiconnectpy
-Version: 2.0.0
+Version: 2.1.0
 Summary: Provides asynchronous authentication and access to Audi Connect
 Author-email: Cyr-ius <cyr-ius@ipocus.net>
 License: GPL-3
 Keywords: connect,async,audi
 Platform: any
 Classifier: Programming Language :: Python
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `audiconnectpy-2.0.0/audiconnectpy.egg-info/SOURCES.txt` & `audiconnectpy-2.1.0/audiconnectpy.egg-info/SOURCES.txt`

 * *Files 19% similar despite different names*

```diff
@@ -24,8 +24,12 @@
 audiconnectpy.egg-info/PKG-INFO
 audiconnectpy.egg-info/SOURCES.txt
 audiconnectpy.egg-info/dependency_links.txt
 audiconnectpy.egg-info/not-zip-safe
 audiconnectpy.egg-info/requires.txt
 audiconnectpy.egg-info/top_level.txt
 tests/__init__.py
-tests/conftest.py
+tests/conftest.py
+tests/test_home.py
+tests/fixtures/audi0.json
+tests/fixtures/info_vehicles.json
+tests/fixtures/location.json
```

### Comparing `audiconnectpy-2.0.0/pyproject.toml` & `audiconnectpy-2.1.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -46,7 +46,11 @@
 "async_timeout".msg = "use asyncio.timeout instead"
 "pytz".msg = "use zoneinfo instead"
 
 [tool.ruff.lint.isort]
 force-sort-within-sections = true
 combine-as-imports = true
 split-on-trailing-comma = false
+
+[[tool.mypy.overrides]]
+module = "yaml"
+ignore_missing_imports = true
```

### Comparing `audiconnectpy-2.0.0/tests/conftest.py` & `audiconnectpy-2.1.0/tests/conftest.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,16 +39,16 @@
     return json.loads(load_fixture("audi2.json"))
 
 
 @pytest.fixture
 def position():
     return {
         "data": {
-            "lon": -0.020479,
-            "lat": 47.928315,
+            "lon": -10.020479,
+            "lat": 87.928315,
             "carCapturedTimestamp": "2024-05-14T17:42:22Z",
         }
     }
 
 
 @pytest.fixture
 def fill_region():
```

