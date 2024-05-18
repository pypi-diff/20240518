# Comparing `tmp/omuserver-0.3.2.tar.gz` & `tmp/omuserver-0.4.2.tar.gz`

## Comparing `omuserver-0.3.2.tar` & `omuserver-0.4.2.tar`

### file list

```diff
@@ -1,59 +1,63 @@
--rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 omuserver-0.3.2/src/omuserver/__init__.py
--rw-r--r--   0        0        0     1310 2020-02-02 00:00:00.000000 omuserver-0.3.2/src/omuserver/__main__.py
--rw-r--r--   0        0        0      420 2020-02-02 00:00:00.000000 omuserver-0.3.2/src/omuserver/config.py
--rw-r--r--   0        0        0      610 2020-02-02 00:00:00.000000 omuserver-0.3.2/src/omuserver/directories.py
--rw-r--r--   0        0        0      876 2020-02-02 00:00:00.000000 omuserver-0.3.2/src/omuserver/helper.py
--rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 omuserver-0.3.2/src/omuserver/version.py
--rw-r--r--   0        0        0      375 2020-02-02 00:00:00.000000 omuserver-0.3.2/src/omuserver/extension/__init__.py
--rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 omuserver-0.3.2/src/omuserver/extension/extension.py
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 omuserver-0.3.2/src/omuserver/extension/asset/__init__.py
--rw-r--r--   0        0        0     3173 2020-02-02 00:00:00.000000 omuserver-0.3.2/src/omuserver/extension/asset/asset_extension.py
--rw-r--r--   0        0        0     2154 2020-02-02 00:00:00.000000 omuserver-0.3.2/src/omuserver/extension/asset/permissions.py
--rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 omuserver-0.3.2/src/omuserver/extension/dashboard/__init__.py
--rw-r--r--   0        0        0     7565 2020-02-02 00:00:00.000000 omuserver-0.3.2/src/omuserver/extension/dashboard/dashboard_extension.py
--rw-r--r--   0        0        0     1999 2020-02-02 00:00:00.000000 omuserver-0.3.2/src/omuserver/extension/dashboard/permission.py
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 omuserver-0.3.2/src/omuserver/extension/endpoint/__init__.py
--rw-r--r--   0        0        0     8365 2020-02-02 00:00:00.000000 omuserver-0.3.2/src/omuserver/extension/endpoint/endpoint_extension.py
--rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 omuserver-0.3.2/src/omuserver/extension/i18n/__init__.py
--rw-r--r--   0        0        0      459 2020-02-02 00:00:00.000000 omuserver-0.3.2/src/omuserver/extension/i18n/i18n_extension.py
--rw-r--r--   0        0        0      994 2020-02-02 00:00:00.000000 omuserver-0.3.2/src/omuserver/extension/i18n/permissions.py
--rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 omuserver-0.3.2/src/omuserver/extension/permission/__init__.py
--rw-r--r--   0        0        0     6544 2020-02-02 00:00:00.000000 omuserver-0.3.2/src/omuserver/extension/permission/permission_extension.py
--rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 omuserver-0.3.2/src/omuserver/extension/plugin/__init__.py
--rw-r--r--   0        0        0     1127 2020-02-02 00:00:00.000000 omuserver-0.3.2/src/omuserver/extension/plugin/plugin_connection.py
--rw-r--r--   0        0        0     3048 2020-02-02 00:00:00.000000 omuserver-0.3.2/src/omuserver/extension/plugin/plugin_extension.py
--rw-r--r--   0        0        0     9099 2020-02-02 00:00:00.000000 omuserver-0.3.2/src/omuserver/extension/plugin/plugin_loader.py
--rw-r--r--   0        0        0     1106 2020-02-02 00:00:00.000000 omuserver-0.3.2/src/omuserver/extension/plugin/plugin_session_connection.py
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 omuserver-0.3.2/src/omuserver/extension/registry/__init__.py
--rw-r--r--   0        0        0     2873 2020-02-02 00:00:00.000000 omuserver-0.3.2/src/omuserver/extension/registry/registry.py
--rw-r--r--   0        0        0     5244 2020-02-02 00:00:00.000000 omuserver-0.3.2/src/omuserver/extension/registry/registry_extension.py
--rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 omuserver-0.3.2/src/omuserver/extension/server/__init__.py
--rw-r--r--   0        0        0     1485 2020-02-02 00:00:00.000000 omuserver-0.3.2/src/omuserver/extension/server/permissions.py
--rw-r--r--   0        0        0     6020 2020-02-02 00:00:00.000000 omuserver-0.3.2/src/omuserver/extension/server/server_extension.py
--rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 omuserver-0.3.2/src/omuserver/extension/signal/__init__.py
--rw-r--r--   0        0        0     4048 2020-02-02 00:00:00.000000 omuserver-0.3.2/src/omuserver/extension/signal/signal_extension.py
--rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 omuserver-0.3.2/src/omuserver/extension/table/__init__.py
--rw-r--r--   0        0        0     8729 2020-02-02 00:00:00.000000 omuserver-0.3.2/src/omuserver/extension/table/cached_table.py
--rw-r--r--   0        0        0     6039 2020-02-02 00:00:00.000000 omuserver-0.3.2/src/omuserver/extension/table/serialized_table.py
--rw-r--r--   0        0        0     3041 2020-02-02 00:00:00.000000 omuserver-0.3.2/src/omuserver/extension/table/server_table.py
--rw-r--r--   0        0        0     2159 2020-02-02 00:00:00.000000 omuserver-0.3.2/src/omuserver/extension/table/session_table_handler.py
--rw-r--r--   0        0        0    10604 2020-02-02 00:00:00.000000 omuserver-0.3.2/src/omuserver/extension/table/table_extension.py
--rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 omuserver-0.3.2/src/omuserver/extension/table/adapters/__init__.py
--rw-r--r--   0        0        0     4884 2020-02-02 00:00:00.000000 omuserver-0.3.2/src/omuserver/extension/table/adapters/sqlitetable.py
--rw-r--r--   0        0        0     1361 2020-02-02 00:00:00.000000 omuserver-0.3.2/src/omuserver/extension/table/adapters/tableadapter.py
--rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 omuserver-0.3.2/src/omuserver/network/__init__.py
--rw-r--r--   0        0        0     6179 2020-02-02 00:00:00.000000 omuserver-0.3.2/src/omuserver/network/network.py
--rw-r--r--   0        0        0     2028 2020-02-02 00:00:00.000000 omuserver-0.3.2/src/omuserver/network/packet_dispatcher.py
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 omuserver-0.3.2/src/omuserver/security/__init__.py
--rw-r--r--   0        0        0     3692 2020-02-02 00:00:00.000000 omuserver-0.3.2/src/omuserver/security/security.py
--rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 omuserver-0.3.2/src/omuserver/server/__init__.py
--rw-r--r--   0        0        0     6964 2020-02-02 00:00:00.000000 omuserver-0.3.2/src/omuserver/server/omuserver.py
--rw-r--r--   0        0        0     2846 2020-02-02 00:00:00.000000 omuserver-0.3.2/src/omuserver/server/server.py
--rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 omuserver-0.3.2/src/omuserver/session/__init__.py
--rw-r--r--   0        0        0     2065 2020-02-02 00:00:00.000000 omuserver-0.3.2/src/omuserver/session/aiohttp_connection.py
--rw-r--r--   0        0        0     6616 2020-02-02 00:00:00.000000 omuserver-0.3.2/src/omuserver/session/session.py
--rw-r--r--   0        0        0      421 2020-02-02 00:00:00.000000 omuserver-0.3.2/test/helper_test.py
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 omuserver-0.3.2/.gitignore
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 omuserver-0.3.2/README.md
--rw-r--r--   0        0        0      585 2020-02-02 00:00:00.000000 omuserver-0.3.2/pyproject.toml
--rw-r--r--   0        0        0      520 2020-02-02 00:00:00.000000 omuserver-0.3.2/PKG-INFO
+-rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 omuserver-0.4.2/src/omuserver/__init__.py
+-rw-r--r--   0        0        0     1310 2020-02-02 00:00:00.000000 omuserver-0.4.2/src/omuserver/__main__.py
+-rw-r--r--   0        0        0      432 2020-02-02 00:00:00.000000 omuserver-0.4.2/src/omuserver/config.py
+-rw-r--r--   0        0        0      635 2020-02-02 00:00:00.000000 omuserver-0.4.2/src/omuserver/directories.py
+-rw-r--r--   0        0        0      876 2020-02-02 00:00:00.000000 omuserver-0.4.2/src/omuserver/helper.py
+-rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 omuserver-0.4.2/src/omuserver/version.py
+-rw-r--r--   0        0        0      375 2020-02-02 00:00:00.000000 omuserver-0.4.2/src/omuserver/extension/__init__.py
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 omuserver-0.4.2/src/omuserver/extension/extension.py
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 omuserver-0.4.2/src/omuserver/extension/asset/__init__.py
+-rw-r--r--   0        0        0     3180 2020-02-02 00:00:00.000000 omuserver-0.4.2/src/omuserver/extension/asset/asset_extension.py
+-rw-r--r--   0        0        0     2154 2020-02-02 00:00:00.000000 omuserver-0.4.2/src/omuserver/extension/asset/permissions.py
+-rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 omuserver-0.4.2/src/omuserver/extension/dashboard/__init__.py
+-rw-r--r--   0        0        0     7610 2020-02-02 00:00:00.000000 omuserver-0.4.2/src/omuserver/extension/dashboard/dashboard_extension.py
+-rw-r--r--   0        0        0     1999 2020-02-02 00:00:00.000000 omuserver-0.4.2/src/omuserver/extension/dashboard/permission.py
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 omuserver-0.4.2/src/omuserver/extension/endpoint/__init__.py
+-rw-r--r--   0        0        0     8312 2020-02-02 00:00:00.000000 omuserver-0.4.2/src/omuserver/extension/endpoint/endpoint_extension.py
+-rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 omuserver-0.4.2/src/omuserver/extension/i18n/__init__.py
+-rw-r--r--   0        0        0      466 2020-02-02 00:00:00.000000 omuserver-0.4.2/src/omuserver/extension/i18n/i18n_extension.py
+-rw-r--r--   0        0        0      994 2020-02-02 00:00:00.000000 omuserver-0.4.2/src/omuserver/extension/i18n/permissions.py
+-rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 omuserver-0.4.2/src/omuserver/extension/logger/__init__.py
+-rw-r--r--   0        0        0     1496 2020-02-02 00:00:00.000000 omuserver-0.4.2/src/omuserver/extension/logger/logger_extension.py
+-rw-r--r--   0        0        0      465 2020-02-02 00:00:00.000000 omuserver-0.4.2/src/omuserver/extension/logger/permissions.py
+-rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 omuserver-0.4.2/src/omuserver/extension/permission/__init__.py
+-rw-r--r--   0        0        0     3346 2020-02-02 00:00:00.000000 omuserver-0.4.2/src/omuserver/extension/permission/permission_extension.py
+-rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 omuserver-0.4.2/src/omuserver/extension/plugin/__init__.py
+-rw-r--r--   0        0        0     1127 2020-02-02 00:00:00.000000 omuserver-0.4.2/src/omuserver/extension/plugin/plugin_connection.py
+-rw-r--r--   0        0        0     3222 2020-02-02 00:00:00.000000 omuserver-0.4.2/src/omuserver/extension/plugin/plugin_extension.py
+-rw-r--r--   0        0        0     3187 2020-02-02 00:00:00.000000 omuserver-0.4.2/src/omuserver/extension/plugin/plugin_instance.py
+-rw-r--r--   0        0        0     7063 2020-02-02 00:00:00.000000 omuserver-0.4.2/src/omuserver/extension/plugin/plugin_loader.py
+-rw-r--r--   0        0        0     1106 2020-02-02 00:00:00.000000 omuserver-0.4.2/src/omuserver/extension/plugin/plugin_session_connection.py
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 omuserver-0.4.2/src/omuserver/extension/registry/__init__.py
+-rw-r--r--   0        0        0     2873 2020-02-02 00:00:00.000000 omuserver-0.4.2/src/omuserver/extension/registry/registry.py
+-rw-r--r--   0        0        0     5468 2020-02-02 00:00:00.000000 omuserver-0.4.2/src/omuserver/extension/registry/registry_extension.py
+-rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 omuserver-0.4.2/src/omuserver/extension/server/__init__.py
+-rw-r--r--   0        0        0     1017 2020-02-02 00:00:00.000000 omuserver-0.4.2/src/omuserver/extension/server/permissions.py
+-rw-r--r--   0        0        0     3924 2020-02-02 00:00:00.000000 omuserver-0.4.2/src/omuserver/extension/server/server_extension.py
+-rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 omuserver-0.4.2/src/omuserver/extension/signal/__init__.py
+-rw-r--r--   0        0        0     4029 2020-02-02 00:00:00.000000 omuserver-0.4.2/src/omuserver/extension/signal/signal_extension.py
+-rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 omuserver-0.4.2/src/omuserver/extension/table/__init__.py
+-rw-r--r--   0        0        0     8729 2020-02-02 00:00:00.000000 omuserver-0.4.2/src/omuserver/extension/table/cached_table.py
+-rw-r--r--   0        0        0     6039 2020-02-02 00:00:00.000000 omuserver-0.4.2/src/omuserver/extension/table/serialized_table.py
+-rw-r--r--   0        0        0     3041 2020-02-02 00:00:00.000000 omuserver-0.4.2/src/omuserver/extension/table/server_table.py
+-rw-r--r--   0        0        0     2159 2020-02-02 00:00:00.000000 omuserver-0.4.2/src/omuserver/extension/table/session_table_handler.py
+-rw-r--r--   0        0        0    10593 2020-02-02 00:00:00.000000 omuserver-0.4.2/src/omuserver/extension/table/table_extension.py
+-rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 omuserver-0.4.2/src/omuserver/extension/table/adapters/__init__.py
+-rw-r--r--   0        0        0     4884 2020-02-02 00:00:00.000000 omuserver-0.4.2/src/omuserver/extension/table/adapters/sqlitetable.py
+-rw-r--r--   0        0        0     1361 2020-02-02 00:00:00.000000 omuserver-0.4.2/src/omuserver/extension/table/adapters/tableadapter.py
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 omuserver-0.4.2/src/omuserver/network/__init__.py
+-rw-r--r--   0        0        0     6098 2020-02-02 00:00:00.000000 omuserver-0.4.2/src/omuserver/network/network.py
+-rw-r--r--   0        0        0     2040 2020-02-02 00:00:00.000000 omuserver-0.4.2/src/omuserver/network/packet_dispatcher.py
+-rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 omuserver-0.4.2/src/omuserver/security/__init__.py
+-rw-r--r--   0        0        0     9084 2020-02-02 00:00:00.000000 omuserver-0.4.2/src/omuserver/security/security.py
+-rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 omuserver-0.4.2/src/omuserver/server/__init__.py
+-rw-r--r--   0        0        0     7184 2020-02-02 00:00:00.000000 omuserver-0.4.2/src/omuserver/server/omuserver.py
+-rw-r--r--   0        0        0     3017 2020-02-02 00:00:00.000000 omuserver-0.4.2/src/omuserver/server/server.py
+-rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 omuserver-0.4.2/src/omuserver/session/__init__.py
+-rw-r--r--   0        0        0     2065 2020-02-02 00:00:00.000000 omuserver-0.4.2/src/omuserver/session/aiohttp_connection.py
+-rw-r--r--   0        0        0     6201 2020-02-02 00:00:00.000000 omuserver-0.4.2/src/omuserver/session/session.py
+-rw-r--r--   0        0        0      421 2020-02-02 00:00:00.000000 omuserver-0.4.2/test/helper_test.py
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 omuserver-0.4.2/.gitignore
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 omuserver-0.4.2/README.md
+-rw-r--r--   0        0        0      585 2020-02-02 00:00:00.000000 omuserver-0.4.2/pyproject.toml
+-rw-r--r--   0        0        0      520 2020-02-02 00:00:00.000000 omuserver-0.4.2/PKG-INFO
```

### Comparing `omuserver-0.3.2/src/omuserver/__main__.py` & `omuserver-0.4.2/src/omuserver/__main__.py`

 * *Files identical despite different names*

### Comparing `omuserver-0.3.2/src/omuserver/directories.py` & `omuserver-0.4.2/src/omuserver/directories.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import pathlib
 from dataclasses import dataclass
 from typing import LiteralString
 
 
-@dataclass
+@dataclass(frozen=True, slots=True)
 class Directories:
     data: pathlib.Path
     assets: pathlib.Path
 
     @classmethod
     def default(cls):
         cwd = pathlib.Path.cwd()
```

### Comparing `omuserver-0.3.2/src/omuserver/helper.py` & `omuserver-0.4.2/src/omuserver/helper.py`

 * *Files identical despite different names*

### Comparing `omuserver-0.3.2/src/omuserver/extension/asset/asset_extension.py` & `omuserver-0.4.2/src/omuserver/extension/asset/asset_extension.py`

 * *Files 1% similar despite different names*

```diff
@@ -49,15 +49,15 @@
         return File(identifier, file_path.read_bytes())
 
 
 class AssetExtension:
     def __init__(self, server: Server) -> None:
         self._server = server
         self.storage = FileStorage(server.directories.assets)
-        server.permissions.register(
+        server.permission_manager.register(
             ASSET_UPLOAD_PERMISSION,
             ASSET_UPLOAD_MANY_PERMISSION,
             ASSET_DOWNLOAD_PERMISSION,
             ASSET_DOWNLOAD_MANY_PERMISSION,
         )
         server.endpoints.bind_endpoint(
             ASSET_UPLOAD_ENDPOINT,
```

### Comparing `omuserver-0.3.2/src/omuserver/extension/asset/permissions.py` & `omuserver-0.4.2/src/omuserver/extension/asset/permissions.py`

 * *Files identical despite different names*

### Comparing `omuserver-0.3.2/src/omuserver/extension/dashboard/dashboard_extension.py` & `omuserver-0.4.2/src/omuserver/extension/dashboard/dashboard_extension.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,14 +17,15 @@
     DashboardSetResponse,
 )
 from omu.extension.dashboard.packets import PluginRequestPacket
 from omu.identifier import Identifier
 
 from omuserver.server import Server
 from omuserver.session import Session
+from omuserver.session.session import SessionType
 
 from .permission import (
     DASHBOARD_OPEN_APP_PERMISSION,
     DASHBOARD_SET_PERMISSION,
     DASHOBARD_APP_EDIT_PERMISSION,
     DASHOBARD_APP_READ_PERMISSION,
 )
@@ -37,15 +38,15 @@
             DASHBOARD_PERMISSION_ACCEPT_PACKET,
             DASHBOARD_PERMISSION_DENY_PACKET,
             DASHBOARD_PLUGIN_REQUEST_PACKET,
             DASHBOARD_PLUGIN_ACCEPT_PACKET,
             DASHBOARD_PLUGIN_DENY_PACKET,
             DASHBOARD_OPEN_APP_PACKET,
         )
-        server.permissions.register(
+        server.permission_manager.register(
             DASHBOARD_SET_PERMISSION,
             DASHBOARD_OPEN_APP_PERMISSION,
             DASHOBARD_APP_READ_PERMISSION,
             DASHOBARD_APP_EDIT_PERMISSION,
         )
         server.packet_dispatcher.add_packet_handler(
             DASHBOARD_PERMISSION_ACCEPT_PACKET,
@@ -87,16 +88,16 @@
             DASHBOARD_OPEN_APP_PACKET,
             app,
         )
 
     async def handle_dashboard_set(
         self, session: Session, identifier: Identifier
     ) -> DashboardSetResponse:
-        if session.token != self.server.config.dashboard_token:
-            raise ValueError("Dashboard token does not match")
+        if session.kind != SessionType.DASHBOARD:
+            raise PermissionDenied("Session is not a dashboard")
         self.dashboard_session = session
         session.event.disconnected += self._on_dashboard_disconnected
         await self.send_pending_permission_requests()
         return {"success": True}
 
     async def _on_dashboard_disconnected(self, session: Session) -> None:
         self.dashboard_session = None
```

### Comparing `omuserver-0.3.2/src/omuserver/extension/dashboard/permission.py` & `omuserver-0.4.2/src/omuserver/extension/dashboard/permission.py`

 * *Files identical despite different names*

### Comparing `omuserver-0.3.2/src/omuserver/extension/endpoint/endpoint_extension.py` & `omuserver-0.4.2/src/omuserver/extension/endpoint/endpoint_extension.py`

 * *Files 1% similar despite different names*

```diff
@@ -165,17 +165,15 @@
             permission=type.permission_id,
         )
         self._endpoints[type.id] = endpoint
 
     def verify_permission(self, endpoint: Endpoint, session: Session):
         if endpoint.id.is_namepath_equal(session.app.id, path_length=1):
             return
-        if endpoint.permission is not None and self._server.permissions.has_permission(
-            session, endpoint.permission
-        ):
+        if endpoint.permission and session.permission_handle.has(endpoint.permission):
             return
         logger.warning(
             f"{session.app.key()} tried to call endpoint {endpoint.id} "
             f"without permission {endpoint.permission}"
         )
         error = (
             f"Permission denied for endpoint {endpoint.id} "
```

### Comparing `omuserver-0.3.2/src/omuserver/extension/i18n/permissions.py` & `omuserver-0.4.2/src/omuserver/extension/i18n/permissions.py`

 * *Files identical despite different names*

### Comparing `omuserver-0.3.2/src/omuserver/extension/plugin/plugin_connection.py` & `omuserver-0.4.2/src/omuserver/extension/plugin/plugin_connection.py`

 * *Files identical despite different names*

### Comparing `omuserver-0.3.2/src/omuserver/extension/plugin/plugin_extension.py` & `omuserver-0.4.2/src/omuserver/extension/plugin/plugin_extension.py`

 * *Files 7% similar despite different names*

```diff
@@ -9,14 +9,15 @@
     PLUGIN_ALLOWED_PACKAGE_TABLE,
     PLUGIN_REQUIRE_PACKET,
 )
 from packaging.specifiers import SpecifierSet
 
 from omuserver.server import Server
 from omuserver.session import Session
+from omuserver.session.session import SessionType
 
 from .plugin_loader import DependencyResolver, PluginLoader
 
 
 class PluginExtension:
     def __init__(self, server: Server) -> None:
         self.server = server
@@ -41,15 +42,15 @@
         self.request_id += 1
         return f"{self.request_id}-{time.time_ns()}"
 
     async def request_plugins(
         self, session: Session, packages: dict[str, str | None]
     ) -> None:
         to_request: list[PackageInfo] = []
-        for package, version in packages.items():
+        for package in packages.keys():
             package_info = await self.dependency_resolver.get_installed_package_info(
                 package
             )
             if package_info is None:
                 package_info = await self.dependency_resolver.fetch_package_info(
                     package
                 )
@@ -68,24 +69,28 @@
             raise Exception("Request was not accepted")
 
     async def handle_require_packet(
         self, session: Session, packages: dict[str, str | None]
     ) -> None:
         if not packages:
             return
-        if not session.is_dashboard:
-            await self.request_plugins(session, packages)
 
-        changed = False
-        for package, version in packages.items():
-            specifier = None
-            if version is not None:
-                specifier = SpecifierSet(version)
-            if self.dependency_resolver.add_dependencies({package: specifier}):
-                changed = True
+        async def task():
+            if session.kind != SessionType.DASHBOARD:
+                await self.request_plugins(session, packages)
+
+            changed = False
+            for package, version in packages.items():
+                specifier = None
+                if version is not None:
+                    specifier = SpecifierSet(version)
+                if self.dependency_resolver.add_dependencies({package: specifier}):
+                    changed = True
+
+            if not changed:
+                return
+
+            async with self.lock:
+                await self.dependency_resolver.resolve()
+                await self.loader.load_updated_plugins()
 
-        if not changed:
-            return
-
-        async with self.lock:
-            await self.dependency_resolver.resolve()
-            await self.loader.load_updated_plugins()
+        session.add_ready_task(task)
```

### Comparing `omuserver-0.3.2/src/omuserver/extension/plugin/plugin_session_connection.py` & `omuserver-0.4.2/src/omuserver/extension/plugin/plugin_session_connection.py`

 * *Files identical despite different names*

### Comparing `omuserver-0.3.2/src/omuserver/extension/registry/registry.py` & `omuserver-0.4.2/src/omuserver/extension/registry/registry.py`

 * *Files identical despite different names*

### Comparing `omuserver-0.3.2/src/omuserver/extension/registry/registry_extension.py` & `omuserver-0.4.2/src/omuserver/extension/registry/registry_extension.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,15 +38,15 @@
 
 
 class RegistryExtension:
     def __init__(self, server: Server) -> None:
         self._server = server
         self.registries: dict[Identifier, ServerRegistry] = {}
         self._startup_registries: list[ServerRegistry] = []
-        server.permissions.register(REGISTRY_PERMISSION)
+        server.permission_manager.register(REGISTRY_PERMISSION)
         server.packet_dispatcher.register(
             REGISTRY_REGISTER_PACKET,
             REGISTRY_LISTEN_PACKET,
             REGISTRY_UPDATE_PACKET,
         )
         server.packet_dispatcher.add_packet_handler(
             REGISTRY_REGISTER_PACKET, self.handle_register
@@ -117,18 +117,21 @@
         registry: ServerRegistry,
         session: Session,
         get_scopes: Callable[[RegistryPermissions], list[Identifier | None]],
     ) -> None:
         if registry.id.is_namepath_equal(session.app.id, path_length=1):
             return
         require_permissions = get_scopes(registry.permissions)
-        if not any(
-            self._server.permissions.has_permission(session, permission)
-            for permission in filter(None, require_permissions)
-        ):
+        # if not any(
+        #     self._server.permissions.has_permission(session, permission)
+        #     for permission in filter(None, require_permissions)
+        # ):
+        #     msg = f"App {session.app.id=} not allowed to access {registry.id=}"
+        #     raise PermissionDenied(msg)
+        if not session.permission_handle.has_any(filter(None, require_permissions)):
             msg = f"App {session.app.id=} not allowed to access {registry.id=}"
             raise PermissionDenied(msg)
 
     def register[T](
         self,
         registry_type: RegistryType[T],
     ) -> Registry[T]:
```

### Comparing `omuserver-0.3.2/src/omuserver/extension/server/permissions.py` & `omuserver-0.4.2/src/omuserver/extension/server/permissions.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 from omu.extension.permission import PermissionType
 from omu.extension.server import (
     SERVER_APPS_READ_PERMISSION_ID,
-    SERVER_CONSOLE_PERMISSION_ID,
     SERVER_SHUTDOWN_PERMISSION_ID,
 )
 
 SERVER_SHUTDOWN_PERMISSION = PermissionType(
     id=SERVER_SHUTDOWN_PERMISSION_ID,
     metadata={
         "level": "high",
@@ -29,21 +28,7 @@
         },
         "note": {
             "en": "Permission to get a list of apps connected to the server",
             "ja": "サーバーに接続されたアプリの一覧を取得する",
         },
     },
 )
-SERVER_CONSOLE_PERMISSION = PermissionType(
-    id=SERVER_CONSOLE_PERMISSION_ID,
-    metadata={
-        "level": "low",
-        "name": {
-            "en": "Access Server Console",
-            "ja": "サーバーのコンソールアクセス",
-        },
-        "note": {
-            "en": "Permission to access the server console",
-            "ja": "サーバーのコンソールにアクセスする権限",
-        },
-    },
-)
```

### Comparing `omuserver-0.3.2/src/omuserver/extension/server/server_extension.py` & `omuserver-0.4.2/src/omuserver/extension/server/server_extension.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,38 +1,30 @@
 from __future__ import annotations
 
-import asyncio
 from asyncio import Future
 from collections import defaultdict
 from collections.abc import Callable
 from typing import TYPE_CHECKING
 
 from loguru import logger
-from omu.errors import PermissionDenied
-from omu.extension.server.packets import ConsolePacket
 from omu.extension.server.server_extension import (
     APP_TABLE_TYPE,
-    CONSOLE_GET_ENDPOINT_TYPE,
-    CONSOLE_LISTEN_PACKET_TYPE,
-    CONSOLE_PACKET_TYPE,
     REQUIRE_APPS_PACKET_TYPE,
-    SERVER_CONSOLE_PERMISSION_ID,
     SHUTDOWN_ENDPOINT_TYPE,
     VERSION_REGISTRY_TYPE,
 )
 from omu.identifier import Identifier
 
 from omuserver import __version__
 from omuserver.helper import get_launch_command
 from omuserver.server import Server
 from omuserver.session import Session
 
 from .permissions import (
     SERVER_APPS_READ_PERMISSION,
-    SERVER_CONSOLE_PERMISSION,
     SERVER_SHUTDOWN_PERMISSION,
 )
 
 if TYPE_CHECKING:
     from loguru import Message
 
 
@@ -54,80 +46,50 @@
 
 
 class ServerExtension:
     def __init__(self, server: Server) -> None:
         self._server = server
         server.packet_dispatcher.register(
             REQUIRE_APPS_PACKET_TYPE,
-            CONSOLE_LISTEN_PACKET_TYPE,
         )
-        server.permissions.register(
+        server.permission_manager.register(
             SERVER_SHUTDOWN_PERMISSION,
             SERVER_APPS_READ_PERMISSION,
-            SERVER_CONSOLE_PERMISSION,
         )
         self.version_registry = self._server.registry.register(VERSION_REGISTRY_TYPE)
         self.apps = self._server.tables.register(APP_TABLE_TYPE)
         server.network.event.connected += self.on_connected
         server.network.event.disconnected += self.on_disconnected
         server.event.start += self.on_start
         server.endpoints.bind_endpoint(
             SHUTDOWN_ENDPOINT_TYPE,
             self.handle_shutdown,
         )
         server.packet_dispatcher.add_packet_handler(
             REQUIRE_APPS_PACKET_TYPE, self.handle_require_apps
         )
-        server.endpoints.bind_endpoint(
-            CONSOLE_GET_ENDPOINT_TYPE, self.handle_console_get
-        )
-        server.packet_dispatcher.add_packet_handler(
-            CONSOLE_LISTEN_PACKET_TYPE, self.handle_console_listen
-        )
         self._app_waiters: dict[Identifier, list[WaitHandle]] = defaultdict(list)
-        self._log_lines: list[str] = []
-        self._log_listeners: list[Session] = []
-        self._log_queue: list[str] = []
-        self._log_event = asyncio.Event()
-        logger.add(LogHandler(self._on_log))
-        self._server.loop.create_task(self.log_task())
-
-    def _on_log(self, message: str) -> None:
-        self._log_queue.append(message)
-        self._log_event.set()
-
-    async def log_task(self) -> None:
-        while True:
-            await self._log_event.wait()
-            self._log_event.clear()
-            packet = ConsolePacket(self._log_queue)
-            for session in self._log_listeners:
-                if session.closed:
-                    continue
-                await session.send(CONSOLE_PACKET_TYPE, packet)
-            self._log_lines.extend(self._log_queue)
-            self._log_queue.clear()
 
     async def handle_require_apps(
         self, session: Session, app_ids: list[Identifier]
     ) -> None:
         for identifier in self._server.network._sessions.keys():
             if identifier not in app_ids:
                 continue
             app_ids.remove(identifier)
         if len(app_ids) == 0:
             return
 
-        ready_task = await session.create_ready_task(f"require_apps({app_ids})")
+        async def task():
+            waiter = WaitHandle(app_ids)
+            for app_id in app_ids:
+                self._app_waiters[app_id].append(waiter)
+            await waiter.future
 
-        waiter = WaitHandle(app_ids)
-        for app_id in app_ids:
-            self._app_waiters[app_id].append(waiter)
-        await waiter.future
-        ready_task.set()
+        session.add_ready_task(task)
 
     async def handle_shutdown(self, session: Session, restart: bool = False) -> bool:
         await self._server.shutdown()
         self._server.loop.create_task(self.shutdown(restart))
         return True
 
     async def shutdown(self, restart: bool = False) -> None:
@@ -135,32 +97,14 @@
             import os
             import sys
 
             os.execv(sys.executable, get_launch_command()["args"])
         else:
             self._server.loop.stop()
 
-    async def handle_console_get(
-        self, session: Session, line_count: int | None
-    ) -> list[str]:
-        if line_count is None:
-            return self._log_lines
-        return self._log_lines[-line_count:]
-
-    async def handle_console_listen(self, session: Session, packet: None) -> None:
-        if not self._server.permissions.has_permission(
-            session, SERVER_CONSOLE_PERMISSION_ID
-        ):
-            msg = (
-                f"Session {session} does not have permission "
-                f"{SERVER_CONSOLE_PERMISSION_ID}"
-            )
-            raise PermissionDenied(msg)
-        self._log_listeners.append(session)
-
     async def on_start(self) -> None:
         await self.version_registry.set(__version__)
         await self.apps.clear()
 
     async def on_connected(self, session: Session) -> None:
         logger.info(f"Connected: {session.app.key()}")
         await self.apps.add(session.app)
```

### Comparing `omuserver-0.3.2/src/omuserver/extension/signal/signal_extension.py` & `omuserver-0.4.2/src/omuserver/extension/signal/signal_extension.py`

 * *Files 2% similar despite different names*

```diff
@@ -55,15 +55,15 @@
         get_scopes: Callable[[SignalPermissions], list[Identifier | None]],
     ) -> None:
         if signal.id.is_namepath_equal(session.app.id, path_length=1):
             return
         for permission in get_scopes(signal.permissions):
             if permission is None:
                 continue
-            if self._server.permissions.has_permission(session, permission):
+            if session.permission_handle.has(permission):
                 return
         msg = f"App {session.app.id=} not allowed to access {signal.id=}"
         raise PermissionDenied(msg)
 
     async def handle_register(
         self, session: Session, data: SignalRegisterPacket
     ) -> None:
```

### Comparing `omuserver-0.3.2/src/omuserver/extension/table/cached_table.py` & `omuserver-0.4.2/src/omuserver/extension/table/cached_table.py`

 * *Files identical despite different names*

### Comparing `omuserver-0.3.2/src/omuserver/extension/table/serialized_table.py` & `omuserver-0.4.2/src/omuserver/extension/table/serialized_table.py`

 * *Files identical despite different names*

### Comparing `omuserver-0.3.2/src/omuserver/extension/table/server_table.py` & `omuserver-0.4.2/src/omuserver/extension/table/server_table.py`

 * *Files identical despite different names*

### Comparing `omuserver-0.3.2/src/omuserver/extension/table/session_table_handler.py` & `omuserver-0.4.2/src/omuserver/extension/table/session_table_handler.py`

 * *Files identical despite different names*

### Comparing `omuserver-0.3.2/src/omuserver/extension/table/table_extension.py` & `omuserver-0.4.2/src/omuserver/extension/table/table_extension.py`

 * *Files 1% similar despite different names*

```diff
@@ -60,15 +60,15 @@
 
 
 class TableExtension:
     def __init__(self, server: Server) -> None:
         self.server = server
         self._tables: dict[Identifier, ServerTable] = {}
         self._adapters: list[TableAdapter] = []
-        server.permissions.register(TABLE_PERMISSION)
+        server.permission_manager.register(TABLE_PERMISSION)
         server.packet_dispatcher.register(
             TABLE_SET_PERMISSION_PACKET,
             TABLE_SET_CONFIG_PACKET,
             TABLE_LISTEN_PACKET,
             TABLE_PROXY_LISTEN_PACKET,
             TABLE_PROXY_PACKET,
             TABLE_ITEM_ADD_PACKET,
@@ -302,15 +302,15 @@
             return
         if table.permissions is None:
             raise PermissionDenied(f"Table {table.id} does not have a permission set")
         permissions: list[Identifier | None] = get_scopes(table.permissions)
         for permission in permissions:
             if permission is None:
                 continue
-            if self.server.permissions.has_permission(session, permission):
+            if session.permission_handle.has(permission):
                 return
 
         raise PermissionDenied(
             f"Table {table.id} does not have permission {table.permissions}"
         )
 
     def register[T: Keyable](self, table_type: TableType[T]) -> Table[T]:
```

### Comparing `omuserver-0.3.2/src/omuserver/extension/table/adapters/sqlitetable.py` & `omuserver-0.4.2/src/omuserver/extension/table/adapters/sqlitetable.py`

 * *Files identical despite different names*

### Comparing `omuserver-0.3.2/src/omuserver/extension/table/adapters/tableadapter.py` & `omuserver-0.4.2/src/omuserver/extension/table/adapters/tableadapter.py`

 * *Files identical despite different names*

### Comparing `omuserver-0.3.2/src/omuserver/network/network.py` & `omuserver-0.4.2/src/omuserver/network/network.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 from __future__ import annotations
 
-import asyncio
 import socket
 
 import psutil
 from aiohttp import web
 from loguru import logger
 from omu import App, Identifier
 from omu.event_emitter import EventEmitter
 from omu.helper import Coro
 from omu.network.packet import PACKET_TYPES, PacketType
 from omu.network.packet.packet_types import DisconnectType
 
 from omuserver.network.packet_dispatcher import ServerPacketDispatcher
 from omuserver.server import Server
-from omuserver.session import Session
+from omuserver.session import Session, SessionType
 from omuserver.session.aiohttp_connection import WebsocketsConnection
 
 
 class Network:
     def __init__(
         self, server: Server, packet_dispatcher: ServerPacketDispatcher
     ) -> None:
@@ -29,15 +28,15 @@
         self._app = web.Application()
         self.add_websocket_route("/ws")
         self.register_packet(PACKET_TYPES.CONNECT, PACKET_TYPES.READY)
         self.add_packet_handler(PACKET_TYPES.READY, self._handle_ready)
         self.event.connected += self._packet_dispatcher.process_connection
 
     async def _handle_ready(self, session: Session, packet: None) -> None:
-        await session.wait_for_tasks()
+        await session.process_ready_tasks()
         if session.closed:
             return
         await session.send(PACKET_TYPES.READY, None)
         logger.info(f"Ready: {session.app.key()}")
 
     def register_packet(self, *packet_types: PacketType) -> None:
         self._packet_dispatcher.register(*packet_types)
@@ -78,15 +77,15 @@
             await ws.prepare(request)
             connection = WebsocketsConnection(ws)
             session = await Session.from_connection(
                 self._server,
                 self._packet_dispatcher.packet_mapper,
                 connection,
             )
-            if not session.is_dashboard:
+            if session.kind != SessionType.DASHBOARD:
                 await self._validate_origin(request, session)
             await self.process_session(session)
             return ws
 
         self._app.router.add_get(path, websocket_handler)
 
     async def process_session(self, session: Session) -> None:
@@ -108,17 +107,14 @@
 
     async def handle_disconnection(self, session: Session) -> None:
         if session.app.id not in self._sessions:
             return
         del self._sessions[session.app.id]
         await self._event.disconnected.emit(session)
 
-    async def _handle_start(self, app: web.Application) -> None:
-        asyncio.create_task(self._event.start.emit())
-
     def is_port_free(self) -> bool:
         try:
             with socket.socket(socket.AF_INET, socket.SOCK_STREAM) as s:
                 s.bind(
                     (
                         self._server.address.host or "127.0.0.1",
                         self._server.address.port,
@@ -142,21 +138,23 @@
             port = self._server.address.port
             name = process.name()
             pid = process.pid
             raise OSError(f"Port {port} already in use by {name} ({pid=})")
 
     async def start(self) -> None:
         self.check_port_availability()
-        self._app.on_startup.append(self._handle_start)
         runner = web.AppRunner(self._app)
         await runner.setup()
         site = web.TCPSite(
-            runner, host=self._server.address.host, port=self._server.address.port
+            runner,
+            host=self._server.address.host or "127.0.0.1",
+            port=self._server.address.port,
         )
         await site.start()
+        await self._event.start.emit()
 
     @property
     def event(self) -> NetworkEvents:
         return self._event
 
 
 class NetworkEvents:
```

### Comparing `omuserver-0.3.2/src/omuserver/network/packet_dispatcher.py` & `omuserver-0.4.2/src/omuserver/network/packet_dispatcher.py`

 * *Files 12% similar despite different names*

```diff
@@ -48,11 +48,11 @@
             self._packet_listeners[packet_type.id].handler = func
 
         if handler:
             decorator(handler)
         return decorator
 
 
-@dataclass
+@dataclass(slots=True)
 class PacketHandler[T]:
     packet_type: PacketType[T]
     handler: Coro[[Session, T], None] | None = None
```

### Comparing `omuserver-0.3.2/src/omuserver/server/omuserver.py` & `omuserver-0.4.2/src/omuserver/server/omuserver.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,24 +11,25 @@
 from omuserver import __version__
 from omuserver.config import Config
 from omuserver.directories import Directories
 from omuserver.extension.asset import AssetExtension
 from omuserver.extension.dashboard import DashboardExtension
 from omuserver.extension.endpoint import EndpointExtension
 from omuserver.extension.i18n import I18nExtension
+from omuserver.extension.logger import LoggerExtension
 from omuserver.extension.permission import PermissionExtension
 from omuserver.extension.plugin import PluginExtension
 from omuserver.extension.registry import RegistryExtension
 from omuserver.extension.server import ServerExtension
 from omuserver.extension.signal import SignalExtension
 from omuserver.extension.table import TableExtension
 from omuserver.helper import safe_path_join
 from omuserver.network import Network
 from omuserver.network.packet_dispatcher import ServerPacketDispatcher
-from omuserver.security.security import Security, ServerAuthenticator
+from omuserver.security.security import PermissionManager, ServerPermissionManager
 
 from .server import Server, ServerEvents
 
 client = aiohttp.ClientSession(
     headers={
         "User-Agent": json.dumps(
             [
@@ -56,26 +57,27 @@
         self._directories = config.directories
         self._directories.mkdir()
         self._packet_dispatcher = ServerPacketDispatcher()
         self._network = Network(self, self._packet_dispatcher)
         self._network.event.start += self._handle_network_start
         self._network.add_http_route("/proxy", self._handle_proxy)
         self._network.add_http_route("/asset", self._handle_assets)
-        self._security = ServerAuthenticator(self)
+        self._security = ServerPermissionManager(self)
         self._running = False
         self._endpoints = EndpointExtension(self)
         self._permissions = PermissionExtension(self)
         self._tables = TableExtension(self)
         self._dashboard = DashboardExtension(self)
         self._registry = RegistryExtension(self)
         self._server = ServerExtension(self)
         self._signal = SignalExtension(self)
         self._plugins = PluginExtension(self)
         self._assets = AssetExtension(self)
         self._i18n = I18nExtension(self)
+        self._logger = LoggerExtension(self)
 
     async def _handle_proxy(self, request: web.Request) -> web.StreamResponse:
         url = request.query.get("url")
         no_cache = bool(request.query.get("no_cache"))
         if not url:
             return web.Response(status=400)
         try:
@@ -163,15 +165,15 @@
         return self._loop
 
     @property
     def address(self) -> Address:
         return self._address
 
     @property
-    def security(self) -> Security:
+    def permission_manager(self) -> PermissionManager:
         return self._security
 
     @property
     def directories(self) -> Directories:
         return self._directories
 
     @property
@@ -215,13 +217,17 @@
         return self._assets
 
     @property
     def i18n(self) -> I18nExtension:
         return self._i18n
 
     @property
+    def logger(self) -> LoggerExtension:
+        return self._logger
+
+    @property
     def running(self) -> bool:
         return self._running
 
     @property
     def event(self) -> ServerEvents:
         return self._event
```

### Comparing `omuserver-0.3.2/src/omuserver/server/server.py` & `omuserver-0.4.2/src/omuserver/server/server.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,22 +10,23 @@
 if TYPE_CHECKING:
     from omuserver.config import Config
     from omuserver.directories import Directories
     from omuserver.extension.asset import AssetExtension
     from omuserver.extension.dashboard import DashboardExtension
     from omuserver.extension.endpoint import EndpointExtension
     from omuserver.extension.i18n import I18nExtension
+    from omuserver.extension.logger import LoggerExtension
     from omuserver.extension.permission import PermissionExtension
     from omuserver.extension.plugin import PluginExtension
     from omuserver.extension.registry import RegistryExtension
     from omuserver.extension.signal import SignalExtension
     from omuserver.extension.table import TableExtension
     from omuserver.network import Network
     from omuserver.network.packet_dispatcher import ServerPacketDispatcher
-    from omuserver.security import Security
+    from omuserver.security import PermissionManager
 
 
 class ServerEvents:
     def __init__(self) -> None:
         self.start = EventEmitter[[]]()
         self.stop = EventEmitter[[]]()
 
@@ -45,15 +46,15 @@
 
     @property
     @abc.abstractmethod
     def directories(self) -> Directories: ...
 
     @property
     @abc.abstractmethod
-    def security(self) -> Security: ...
+    def permission_manager(self) -> PermissionManager: ...
 
     @property
     @abc.abstractmethod
     def network(self) -> Network: ...
 
     @property
     @abc.abstractmethod
@@ -93,14 +94,18 @@
 
     @property
     @abc.abstractmethod
     def i18n(self) -> I18nExtension: ...
 
     @property
     @abc.abstractmethod
+    def logger(self) -> LoggerExtension: ...
+
+    @property
+    @abc.abstractmethod
     def running(self) -> bool: ...
 
     @abc.abstractmethod
     def run(self) -> None: ...
 
     @abc.abstractmethod
     async def start(self) -> None: ...
```

### Comparing `omuserver-0.3.2/src/omuserver/session/aiohttp_connection.py` & `omuserver-0.4.2/src/omuserver/session/aiohttp_connection.py`

 * *Files identical despite different names*

### Comparing `omuserver-0.3.2/src/omuserver/session/session.py` & `omuserver-0.4.2/src/omuserver/session/session.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,27 +1,34 @@
 from __future__ import annotations
 
 import abc
 import asyncio
 from dataclasses import dataclass
+from enum import Enum
+from typing import TYPE_CHECKING
 
 from loguru import logger
 from omu import App
 from omu.errors import DisconnectReason
 from omu.event_emitter import EventEmitter
+from omu.helper import Coro
 from omu.network.packet import PACKET_TYPES, Packet, PacketType
 from omu.network.packet.packet_types import (
     ConnectPacket,
     DisconnectPacket,
     DisconnectType,
 )
 from omu.network.packet_mapper import PacketMapper
+from result import Err, Ok
 
 from omuserver.server import Server
 
+if TYPE_CHECKING:
+    from omuserver.security import PermissionHandle
+
 
 class SessionConnection(abc.ABC):
     @abc.abstractmethod
     async def send(self, packet: Packet, packet_mapper: PacketMapper) -> None: ...
 
     @abc.abstractmethod
     async def receive(self, packet_mapper: PacketMapper) -> Packet | None: ...
@@ -37,43 +44,40 @@
 class SessionEvents:
     def __init__(self) -> None:
         self.packet = EventEmitter[Session, Packet]()
         self.disconnected = EventEmitter[Session]()
         self.ready = EventEmitter[Session]()
 
 
-@dataclass
+@dataclass(frozen=True, slots=True)
 class SessionTask:
     session: Session
-    start_future: asyncio.Future[None]
-    future: asyncio.Future[None]
+    coro: Coro[[], None]
     name: str
 
-    def set(self) -> None:
-        self.future.set_result(None)
 
-    def __repr__(self) -> str:
-        return f"SessionTask({self.name})"
+class SessionType(Enum):
+    APP = "app"
+    PLUGIN = "plugin"
+    DASHBOARD = "dashboard"
 
 
 class Session:
     def __init__(
         self,
         packet_mapper: PacketMapper,
         app: App,
-        token: str,
-        is_dashboard: bool,
-        is_plugin: bool,
+        permission_handle: PermissionHandle,
+        kind: SessionType,
         connection: SessionConnection,
     ) -> None:
         self.packet_mapper = packet_mapper
         self.app = app
-        self.token = token
-        self.is_dashboard = is_dashboard
-        self.is_plugin = is_plugin
+        self.permission_handle = permission_handle
+        self.kind = kind
         self.connection = connection
         self.event = SessionEvents()
         self.ready_tasks: list[SessionTask] = []
         self.ready = False
 
     @classmethod
     async def from_connection(
@@ -112,50 +116,36 @@
             )
             await connection.close()
             raise RuntimeError(f"Invalid packet data: {packet.data}")
         event = packet.data
         app = event.app
         token = event.token
 
-        if token and await server.security.is_plugin_token(token):
-            session = Session(
-                packet_mapper=packet_mapper,
-                app=app,
-                token=token,
-                is_dashboard=False,
-                is_plugin=True,
-                connection=connection,
-            )
-            return session
-
-        is_dashboard = False
-        if server.config.dashboard_token and server.config.dashboard_token == token:
-            is_dashboard = True
-        else:
-            token = await server.security.verify_app_token(app, token)
-        if token is None:
-            await connection.send(
-                Packet(
-                    PACKET_TYPES.DISCONNECT,
-                    DisconnectPacket(DisconnectType.INVALID_TOKEN, "Invalid token"),
-                ),
-                packet_mapper,
-            )
-            await connection.close()
-            raise RuntimeError("Invalid token")
-        session = Session(
-            packet_mapper=packet_mapper,
-            app=app,
-            token=token,
-            is_dashboard=is_dashboard,
-            is_plugin=False,
-            connection=connection,
-        )
-        await session.send(PACKET_TYPES.TOKEN, token)
-        return session
+        match await server.permission_manager.verify_app_token(app, token):
+            case Ok((kind, permission_handle, new_token)):
+                session = Session(
+                    packet_mapper=packet_mapper,
+                    app=app,
+                    permission_handle=permission_handle,
+                    kind=kind,
+                    connection=connection,
+                )
+                if session.kind != SessionType.PLUGIN:
+                    await session.send(PACKET_TYPES.TOKEN, new_token)
+                return session
+            case Err(error):
+                await connection.send(
+                    Packet(
+                        PACKET_TYPES.DISCONNECT,
+                        DisconnectPacket(DisconnectType.INVALID_TOKEN, error),
+                    ),
+                    packet_mapper,
+                )
+                await connection.close()
+                raise RuntimeError(f"Invalid token: {error}")
 
     @property
     def closed(self) -> bool:
         return self.connection.closed
 
     async def disconnect(
         self, disconnect_type: DisconnectType, message: str | None = None
@@ -181,31 +171,25 @@
         except DisconnectReason as reason:
             logger.opt(exception=reason).error("Disconnecting session")
             await self.disconnect(reason.type, reason.message)
 
     async def send[T](self, packet_type: PacketType[T], data: T) -> None:
         await self.connection.send(Packet(packet_type, data), self.packet_mapper)
 
-    async def create_ready_task(self, name: str) -> SessionTask:
+    def add_ready_task(self, coro: Coro[[], None]):
         if self.ready:
             raise RuntimeError("Session is already ready")
-        start_future = asyncio.Future()
-        future = asyncio.Future()
         task = SessionTask(
             session=self,
-            start_future=start_future,
-            future=future,
-            name=name,
+            coro=coro,
+            name=coro.__name__,
         )
         self.ready_tasks.append(task)
-        await start_future
-        return task
 
-    async def wait_for_tasks(self) -> None:
+    async def process_ready_tasks(self) -> None:
         if self.ready:
             raise RuntimeError("Session is already ready")
         for task in self.ready_tasks:
-            task.start_future.set_result(None)
-            await task.future
+            await task.coro()
         self.ready_tasks.clear()
         self.ready = True
         await self.event.ready.emit(self)
```

### Comparing `omuserver-0.3.2/pyproject.toml` & `omuserver-0.4.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "omuserver"
-version = "0.3.2"
+version = "0.4.2"
 description = "Add your description here"
 authors = [
     { name = "am230", email = "111672334+am230@users.noreply.github.com" },
 ]
 dependencies = [
     "loguru>=0.7.2",
     "aiohttp>=3.9.3",
```

### Comparing `omuserver-0.3.2/PKG-INFO` & `omuserver-0.4.2/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: omuserver
-Version: 0.3.2
+Version: 0.4.2
 Summary: Add your description here
 Author-email: am230 <111672334+am230@users.noreply.github.com>
 Requires-Python: >=3.12
 Requires-Dist: aiohttp>=3.9.3
 Requires-Dist: click>=8.1.7
 Requires-Dist: loguru>=0.7.2
 Requires-Dist: omu>=0.1.4
```

