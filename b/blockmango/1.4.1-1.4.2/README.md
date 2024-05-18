# Comparing `tmp/blockmango-1.4.1.tar.gz` & `tmp/blockmango-1.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "blockmango-1.4.1.tar", last modified: Thu May 16 20:29:39 2024, max compression
+gzip compressed data, was "blockmango-1.4.2.tar", last modified: Fri May 17 15:55:13 2024, max compression
```

## Comparing `blockmango-1.4.1.tar` & `blockmango-1.4.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwx------   0 userland  (2000) userland  (2000)        0 2024-05-16 20:29:39.433166 blockmango-1.4.1/
--rw-------   0 userland  (2000) userland  (2000)     1061 2024-05-16 17:46:17.000000 blockmango-1.4.1/LICENSE.md
--rw-------   0 userland  (2000) userland  (2000)      430 2024-05-16 20:29:39.429166 blockmango-1.4.1/PKG-INFO
--rw-------   0 userland  (2000) userland  (2000)      834 2024-05-16 17:43:12.000000 blockmango-1.4.1/README.md
-drwx------   0 userland  (2000) userland  (2000)        0 2024-05-16 20:29:39.409166 blockmango-1.4.1/blockmango/
--rw-------   0 userland  (2000) userland  (2000)      172 2024-05-16 20:23:50.000000 blockmango-1.4.1/blockmango/__init__.py
--rw-------   0 userland  (2000) userland  (2000)     5961 2024-05-16 20:24:58.000000 blockmango-1.4.1/blockmango/clan.py
--rw-------   0 userland  (2000) userland  (2000)      747 2024-05-16 20:23:50.000000 blockmango-1.4.1/blockmango/constants.py
--rw-------   0 userland  (2000) userland  (2000)     1856 2024-05-16 20:27:18.000000 blockmango-1.4.1/blockmango/decoration.py
--rw-------   0 userland  (2000) userland  (2000)     3616 2024-05-16 20:27:59.000000 blockmango-1.4.1/blockmango/friends.py
--rw-------   0 userland  (2000) userland  (2000)     4336 2024-05-16 20:28:32.000000 blockmango-1.4.1/blockmango/groupchat.py
--rw-------   0 userland  (2000) userland  (2000)     3391 2024-05-16 20:28:52.000000 blockmango-1.4.1/blockmango/user.py
-drwx------   0 userland  (2000) userland  (2000)        0 2024-05-16 20:29:39.425166 blockmango-1.4.1/blockmango.egg-info/
--rw-------   0 userland  (2000) userland  (2000)      430 2024-05-16 20:29:38.000000 blockmango-1.4.1/blockmango.egg-info/PKG-INFO
--rw-------   0 userland  (2000) userland  (2000)      354 2024-05-16 20:29:38.000000 blockmango-1.4.1/blockmango.egg-info/SOURCES.txt
--rw-------   0 userland  (2000) userland  (2000)        1 2024-05-16 20:29:38.000000 blockmango-1.4.1/blockmango.egg-info/dependency_links.txt
--rw-------   0 userland  (2000) userland  (2000)        9 2024-05-16 20:29:38.000000 blockmango-1.4.1/blockmango.egg-info/requires.txt
--rw-------   0 userland  (2000) userland  (2000)       11 2024-05-16 20:29:38.000000 blockmango-1.4.1/blockmango.egg-info/top_level.txt
--rw-------   0 userland  (2000) userland  (2000)       38 2024-05-16 20:29:39.433166 blockmango-1.4.1/setup.cfg
--rw-------   0 userland  (2000) userland  (2000)      503 2024-05-16 20:29:22.000000 blockmango-1.4.1/setup.py
+drwx------   0 userland  (2000) userland  (2000)        0 2024-05-17 15:55:13.911391 blockmango-1.4.2/
+-rw-------   0 userland  (2000) userland  (2000)     1061 2024-05-16 17:46:17.000000 blockmango-1.4.2/LICENSE.md
+-rw-------   0 userland  (2000) userland  (2000)      430 2024-05-17 15:55:13.911391 blockmango-1.4.2/PKG-INFO
+-rw-------   0 userland  (2000) userland  (2000)      834 2024-05-16 17:43:12.000000 blockmango-1.4.2/README.md
+drwx------   0 userland  (2000) userland  (2000)        0 2024-05-17 15:55:13.895391 blockmango-1.4.2/blockmango/
+-rw-------   0 userland  (2000) userland  (2000)      200 2024-05-17 15:51:17.000000 blockmango-1.4.2/blockmango/__init__.py
+-rw-------   0 userland  (2000) userland  (2000)     4628 2024-05-17 15:51:44.000000 blockmango-1.4.2/blockmango/clan.py
+-rw-------   0 userland  (2000) userland  (2000)     1477 2024-05-17 15:52:40.000000 blockmango-1.4.2/blockmango/decoration.py
+-rw-------   0 userland  (2000) userland  (2000)     2505 2024-05-17 15:53:00.000000 blockmango-1.4.2/blockmango/friends.py
+-rw-------   0 userland  (2000) userland  (2000)     3520 2024-05-17 15:53:21.000000 blockmango-1.4.2/blockmango/groupchat.py
+-rw-------   0 userland  (2000) userland  (2000)     3674 2024-05-17 15:53:39.000000 blockmango-1.4.2/blockmango/http.py
+-rw-------   0 userland  (2000) userland  (2000)     2375 2024-05-17 15:53:55.000000 blockmango-1.4.2/blockmango/user.py
+drwx------   0 userland  (2000) userland  (2000)        0 2024-05-17 15:55:13.907391 blockmango-1.4.2/blockmango.egg-info/
+-rw-------   0 userland  (2000) userland  (2000)      430 2024-05-17 15:55:13.000000 blockmango-1.4.2/blockmango.egg-info/PKG-INFO
+-rw-------   0 userland  (2000) userland  (2000)      349 2024-05-17 15:55:13.000000 blockmango-1.4.2/blockmango.egg-info/SOURCES.txt
+-rw-------   0 userland  (2000) userland  (2000)        1 2024-05-17 15:55:13.000000 blockmango-1.4.2/blockmango.egg-info/dependency_links.txt
+-rw-------   0 userland  (2000) userland  (2000)        9 2024-05-17 15:55:13.000000 blockmango-1.4.2/blockmango.egg-info/requires.txt
+-rw-------   0 userland  (2000) userland  (2000)       11 2024-05-17 15:55:13.000000 blockmango-1.4.2/blockmango.egg-info/top_level.txt
+-rw-------   0 userland  (2000) userland  (2000)       38 2024-05-17 15:55:13.911391 blockmango-1.4.2/setup.cfg
+-rw-------   0 userland  (2000) userland  (2000)      503 2024-05-17 15:54:55.000000 blockmango-1.4.2/setup.py
```

### Comparing `blockmango-1.4.1/LICENSE.md` & `blockmango-1.4.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `blockmango-1.4.1/README.md` & `blockmango-1.4.2/README.md`

 * *Files identical despite different names*

### Comparing `blockmango-1.4.1/blockmango/decoration.py` & `blockmango-1.4.2/blockmango/decoration.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,46 +1,36 @@
-import requests
-import constants
-from constants import BASE_URL_DECORATION, BASE_URL_SHOP, BASE_URL_USER, HEADERS_TEMPLATE
-
-class Decoration:
-    def __init__(self, user_id, access_token):
-        self.headers = {
-            **HEADERS_TEMPLATE,
-            "userId": user_id,
-            "Access-Token": access_token
-        }
-
-    def _handle_response(self, response):
-        return response.json()
-
-    def _get(self, base_url, endpoint, params=None):
-        response = requests.get(f"{base_url}{endpoint}", headers=self.headers, params=params)
-        return self._handle_response(response)
-
-    def _post(self, base_url, endpoint, json_data=None, params=None):
-        response = requests.post(f"{base_url}{endpoint}", headers=self.headers, json=json_data, params=params)
-        return self._handle_response(response)
-
-    def see_skins(self, uid):
-        endpoint = f"/new/decorations/users/{uid}/classify/all"
-        params = {"engineVersion": "10105", "os": "android", "showVip": 1}
-        return self._get(BASE_URL_DECORATION, endpoint, params)
-
-    def current_price(self, skin_id, is_suit):
-        endpoint = "/decoration/current/price"
-        payload = [{"id": skin_id, "isSuit": is_suit}]
-        return self._post(BASE_URL_DECORATION, endpoint, json_data=payload)
-
-    def buy_skin(self, diamond, cloth_voucher, paytype):
-        endpoint = "/new/shop/decorations/buy"
-        params = {"diamond": diamond, "gold": 0, "clothVoucher": cloth_voucher, "payType": paytype}
-        return self._post(BASE_URL_SHOP, endpoint, params=params)
-
-    def shop_info(self):
-        endpoint = "/user/shop/info"
-        return self._get(BASE_URL_USER, endpoint)
-
-    def equip_skin(self, skin_id):
-        endpoint = "/decorations/using/new"
-        params = {"ids": skin_id}
-        return self._post(BASE_URL_DECORATION, endpoint, params=params)
+from .http import HTTPMixin
+
+
+BASE_URL_DECORATION = "http://modsgs.sandboxol.com/decoration/api/v1"
+BASE_URL_SHOP = "http://modsgs.sandboxol.com/shop/api/v1"
+BASE_URL_USER = "http://modsgs.sandboxol.com/user/api/v1"
+
+
+class Decoration(HTTPMixin):
+  __slots__ = ("headers",)
+
+  def __init__(self, user_id, access_token):
+    self.headers = { "userId": user_id, "Access-Token": access_token, "User-Agent": "okhttp/3.12.1" }
+
+  def skins(self, uid):
+    endpoint = f"{BASE_URL_DECORATION}/new/decorations/users/{uid}/classify/all"
+    params = { "engineVersion": "10105", "os": "android", "showVip": 1 }
+    return self._get(endpoint, headers=self.headers, params=params)
+
+  def current_price(self, skin_id, is_suit):
+    endpoint = f"{BASE_URL_DECORATION}/decoration/current/price"
+    payload = [{ "id": skin_id, "isSuit": is_suit }]
+    return self._post(endpoint, headers=self.headers, json_data=payload)
+
+  def buy(self, diamond, cloth_voucher, paytype):
+    endpoint = f"{BASE_URL_SHOP}/new/shop/decorations/buy"
+    params = { "diamond": diamond, "gold": 0, "clothVoucher": cloth_voucher, "payType": paytype }
+    return self._post(endpoint, headers=self.headers, params=params)
+
+  def shop_info(self):
+    return self._get(f"{BASE_URL_USER}/user/shop/info", headers=self.headers)
+
+  def equip(self, skin_id):
+    endpoint = f"{BASE_URL_DECORATION}/decorations/using/new"
+    params = { "ids": skin_id }
+    return self._post(endpoint, headers=self.headers, params=params)
```

