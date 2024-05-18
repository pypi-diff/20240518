# Comparing `tmp/matrix_reportbot-0.0.1.tar.gz` & `tmp/matrix_reportbot-0.0.2.tar.gz`

## Comparing `matrix_reportbot-0.0.1.tar` & `matrix_reportbot-0.0.2.tar`

### file list

```diff
@@ -1,15 +1,13 @@
--rw-r--r--   0        0        0     1973 2020-02-02 00:00:00.000000 matrix_reportbot-0.0.1/config.dist.ini
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 matrix_reportbot-0.0.1/pantalaimon.example.conf
--rw-r--r--   0        0        0      509 2020-02-02 00:00:00.000000 matrix_reportbot-0.0.1/pantalaimon_first_login.py
--rw-r--r--   0        0        0      304 2020-02-02 00:00:00.000000 matrix_reportbot-0.0.1/reportbot-pantalaimon.service
--rw-r--r--   0        0        0      262 2020-02-02 00:00:00.000000 matrix_reportbot-0.0.1/reportbot.service
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 matrix_reportbot-0.0.1/src/matrix_reportbot/__init__.py
--rw-r--r--   0        0        0     1338 2020-02-02 00:00:00.000000 matrix_reportbot-0.0.1/src/matrix_reportbot/__main__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 matrix_reportbot-0.0.1/src/matrix_reportbot/classes/__init__.py
--rw-r--r--   0        0        0    18187 2020-02-02 00:00:00.000000 matrix_reportbot-0.0.1/src/matrix_reportbot/classes/bot.py
--rw-r--r--   0        0        0      943 2020-02-02 00:00:00.000000 matrix_reportbot-0.0.1/src/matrix_reportbot/classes/logging.py
--rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 matrix_reportbot-0.0.1/.gitignore
--rw-r--r--   0        0        0     1087 2020-02-02 00:00:00.000000 matrix_reportbot-0.0.1/LICENSE
--rw-r--r--   0        0        0     1615 2020-02-02 00:00:00.000000 matrix_reportbot-0.0.1/README.md
--rw-r--r--   0        0        0     1003 2020-02-02 00:00:00.000000 matrix_reportbot-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     3546 2020-02-02 00:00:00.000000 matrix_reportbot-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1973 2020-02-02 00:00:00.000000 matrix_reportbot-0.0.2/config.dist.ini
+-rw-r--r--   0        0        0      509 2020-02-02 00:00:00.000000 matrix_reportbot-0.0.2/get_access_token.py
+-rw-r--r--   0        0        0      269 2020-02-02 00:00:00.000000 matrix_reportbot-0.0.2/reportbot.service
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 matrix_reportbot-0.0.2/src/matrix_reportbot/__init__.py
+-rw-r--r--   0        0        0     1338 2020-02-02 00:00:00.000000 matrix_reportbot-0.0.2/src/matrix_reportbot/__main__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 matrix_reportbot-0.0.2/src/matrix_reportbot/classes/__init__.py
+-rw-r--r--   0        0        0    19492 2020-02-02 00:00:00.000000 matrix_reportbot-0.0.2/src/matrix_reportbot/classes/bot.py
+-rw-r--r--   0        0        0      943 2020-02-02 00:00:00.000000 matrix_reportbot-0.0.2/src/matrix_reportbot/classes/logging.py
+-rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 matrix_reportbot-0.0.2/.gitignore
+-rw-r--r--   0        0        0     1087 2020-02-02 00:00:00.000000 matrix_reportbot-0.0.2/LICENSE
+-rw-r--r--   0        0        0     1615 2020-02-02 00:00:00.000000 matrix_reportbot-0.0.2/README.md
+-rw-r--r--   0        0        0      984 2020-02-02 00:00:00.000000 matrix_reportbot-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     3519 2020-02-02 00:00:00.000000 matrix_reportbot-0.0.2/PKG-INFO
```

### Comparing `matrix_reportbot-0.0.1/config.dist.ini` & `matrix_reportbot-0.0.2/config.dist.ini`

 * *Files identical despite different names*

### Comparing `matrix_reportbot-0.0.1/src/matrix_reportbot/__main__.py` & `matrix_reportbot-0.0.2/src/matrix_reportbot/__main__.py`

 * *Files identical despite different names*

### Comparing `matrix_reportbot-0.0.1/src/matrix_reportbot/classes/bot.py` & `matrix_reportbot-0.0.2/src/matrix_reportbot/classes/bot.py`

 * *Files 4% similar despite different names*

```diff
@@ -522,14 +522,48 @@
                         self.room_id,
                         f"Something went wrong processing reports: {e}.",
                         True,
                     )
                 except Exception as e:
                     self.logger.log(f"Error sending error message: {e}")
 
+    async def accept_pending_invites(self):
+        """Accept all pending invites."""
+
+        assert self.matrix_client, "Matrix client not set up"
+
+        invites = self.matrix_client.invited_rooms
+
+        for invite in [k for k in invites.keys()]:
+            if invite in self.room_ignore_list:
+                self.logger.log(
+                    f"Ignoring invite to room {invite} (room is in ignore list)",
+                    "debug",
+                )
+                continue
+
+            self.logger.log(f"Accepting invite to room {invite}")
+
+            response = await self.matrix_client.join(invite)
+
+            if isinstance(response, JoinError):
+                self.logger.log(
+                    f"Error joining room {invite}: {response.message}. Not trying again.",
+                    "error",
+                )
+
+                leave_response = await self.matrix_client.room_leave(invite)
+
+                if isinstance(leave_response, RoomLeaveError):
+                    self.logger.log(
+                        f"Error leaving room {invite}: {leave_response.message}",
+                        "error",
+                    )
+                    self.room_ignore_list.append(invite)
+
     async def run(self):
         """Start the bot."""
 
         # Set up the Matrix client
 
         assert self.matrix_client, "Matrix client not set up"
         assert self.matrix_client.access_token, "Access token not set up"
@@ -541,19 +575,24 @@
             self.matrix_client.device_id = await self._get_device_id()
 
         client_config = AsyncClientConfig(
             store_sync_tokens=False, encryption_enabled=False, store=None
         )
         self.matrix_client.config = client_config
 
-        # Run initial sync (includes joining rooms)
+        # Run initial sync
 
         self.logger.log("Running initial sync...", "debug")
 
-        sync = await self.matrix_client.sync(timeout=30000, full_state=True)
+        await self.matrix_client.sync(timeout=30000, full_state=True)
+
+        # Accept pending invites
+
+        self.logger.log("Joining rooms...", "debug")
+        self.accept_pending_invites()
 
         # Set custom name
 
         if self.display_name:
             self.logger.log(f"Setting display name to {self.display_name}", "debug")
             asyncio.create_task(self.matrix_client.set_displayname(self.display_name))
```

### Comparing `matrix_reportbot-0.0.1/src/matrix_reportbot/classes/logging.py` & `matrix_reportbot-0.0.2/src/matrix_reportbot/classes/logging.py`

 * *Files identical despite different names*

### Comparing `matrix_reportbot-0.0.1/LICENSE` & `matrix_reportbot-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `matrix_reportbot-0.0.1/README.md` & `matrix_reportbot-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `matrix_reportbot-0.0.1/pyproject.toml` & `matrix_reportbot-0.0.2/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "hatchling.build"
 
 [tool.hatch.metadata]
 allow-direct-references = true
 
 [project]
 name = "matrix-reportbot"
-version = "0.0.1"
+version = "0.0.2"
 
 authors = [
   { name="Private.coffee Team", email="support@private.coffee" },
 ]
 
 description = "Simple content report subscription bot for Matrix."
 readme = "README.md"
@@ -26,15 +26,14 @@
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 
 dependencies = [
     "matrix-nio",
-    "pantalaimon",
     "setuptools",
     "markdown2",
     ]
 
 [project.urls]
 "Homepage" = "https://git.private.coffee/PrivateCoffee/matrix-reportbot"
 "Bug Tracker" = "https://git.private.coffee/PrivateCoffee/matrix-reportbot/issues"
```

### Comparing `matrix_reportbot-0.0.1/PKG-INFO` & `matrix_reportbot-0.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: matrix-reportbot
-Version: 0.0.1
+Version: 0.0.2
 Summary: Simple content report subscription bot for Matrix.
 Project-URL: Homepage, https://git.private.coffee/PrivateCoffee/matrix-reportbot
 Project-URL: Bug Tracker, https://git.private.coffee/PrivateCoffee/matrix-reportbot/issues
 Author-email: "Private.coffee Team" <support@private.coffee>
 License: Copyright (c) 2024 Private.coffee Team <support@private.coffee>
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -27,15 +27,14 @@
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
 Requires-Dist: markdown2
 Requires-Dist: matrix-nio
-Requires-Dist: pantalaimon
 Requires-Dist: setuptools
 Description-Content-Type: text/markdown
 
 # Matrix-ReportBot
 
 [![Support Private.coffee!](https://shields.private.coffee/badge/private.coffee-support%20us!-pink?logo=coffeescript)](https://private.coffee)
 [![PyPI](https://shields.private.coffee/pypi/v/matrix-reportbot)](https://pypi.org/project/matrix-reportbot/)
```

