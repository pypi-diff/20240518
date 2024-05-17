# Comparing `tmp/fractal_matrix_client-0.0.5.tar.gz` & `tmp/fractal_matrix_client-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fractal_matrix_client-0.0.5.tar", max compression
+gzip compressed data, was "fractal_matrix_client-0.0.6.tar", max compression
```

## Comparing `fractal_matrix_client-0.0.5.tar` & `fractal_matrix_client-0.0.6.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0    34523 2024-02-16 23:02:46.770829 fractal_matrix_client-0.0.5/LICENSE
--rw-r--r--   0        0        0      599 2024-02-16 23:02:46.770829 fractal_matrix_client-0.0.5/README.md
--rw-r--r--   0        0        0      212 2024-02-16 23:02:46.770829 fractal_matrix_client-0.0.5/fractal/matrix/__init__.py
--rw-r--r--   0        0        0    14114 2024-02-16 23:02:46.770829 fractal_matrix_client-0.0.5/fractal/matrix/async_client.py
--rw-r--r--   0        0        0        0 2024-02-16 23:02:46.770829 fractal_matrix_client-0.0.5/fractal/matrix/controllers/__init__.py
--rw-r--r--   0        0        0      664 2024-02-16 23:02:46.770829 fractal_matrix_client-0.0.5/fractal/matrix/exceptions.py
--rw-r--r--   0        0        0     1683 2024-02-16 23:02:46.770829 fractal_matrix_client-0.0.5/fractal/matrix/utils.py
--rw-r--r--   0        0        0      432 2024-02-16 23:02:46.770829 fractal_matrix_client-0.0.5/pyproject.toml
--rw-r--r--   0        0        0     1243 1970-01-01 00:00:00.000000 fractal_matrix_client-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0    34523 2024-05-17 22:02:02.894552 fractal_matrix_client-0.0.6/LICENSE
+-rw-r--r--   0        0        0      599 2024-05-17 22:02:02.894552 fractal_matrix_client-0.0.6/README.md
+-rw-r--r--   0        0        0      212 2024-05-17 22:02:02.894552 fractal_matrix_client-0.0.6/fractal/matrix/__init__.py
+-rw-r--r--   0        0        0    14346 2024-05-17 22:02:02.894552 fractal_matrix_client-0.0.6/fractal/matrix/async_client.py
+-rw-r--r--   0        0        0        0 2024-05-17 22:02:02.894552 fractal_matrix_client-0.0.6/fractal/matrix/controllers/__init__.py
+-rw-r--r--   0        0        0      664 2024-05-17 22:02:02.894552 fractal_matrix_client-0.0.6/fractal/matrix/exceptions.py
+-rw-r--r--   0        0        0     1683 2024-05-17 22:02:02.894552 fractal_matrix_client-0.0.6/fractal/matrix/utils.py
+-rw-r--r--   0        0        0      885 2024-05-17 22:02:02.894552 fractal_matrix_client-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0     1627 1970-01-01 00:00:00.000000 fractal_matrix_client-0.0.6/PKG-INFO
```

### Comparing `fractal_matrix_client-0.0.5/LICENSE` & `fractal_matrix_client-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `fractal_matrix_client-0.0.5/README.md` & `fractal_matrix_client-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `fractal_matrix_client-0.0.5/fractal/matrix/async_client.py` & `fractal_matrix_client-0.0.6/fractal/matrix/async_client.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 from nio import (
     AsyncClient,
     AsyncClientConfig,
     DiscoveryInfoError,
     InviteInfo,
     JoinError,
     MessageDirection,
+    ProfileSetDisplayNameError,
     RoomGetStateEventError,
     RoomInviteError,
     RoomMessagesError,
     RoomPutStateError,
     RoomSendResponse,
     SyncError,
     TransferMonitor,
@@ -113,14 +114,17 @@
             user_id (str): The user id to invite to the room.
             room_id (str): The room id to invite the user to.
             admin (bool): Whether or not to set the user as an admin. FIXME: Only admin invites are supported for now.
         """
         if not admin:
             raise Exception("FIXME: Only admin invites are supported for now.")
 
+        # ensure that the provided matrix_id is a valid matrix id.
+        parse_matrix_id(user_id)
+
         # check if user_id is lowercase
         if not user_id.split("@")[1].islower():
             raise Exception("Matrix ids must be lowercase.")
 
         logger.info(f"Sending invite to {room_id} to user ({user_id})")
         res = await self.room_invite(room_id, user_id)
         if isinstance(res, RoomInviteError):
@@ -150,15 +154,14 @@
         TODO: Optionally support a custom invite filter.
         Returns:
             Dict[str, InviteInfo]: A dictionary of room ids to invite info.
         """
         # save previous next batch since sync will replace it.
         prev_next_batch = self.next_batch
         res = await self.sync(since=None, timeout=0, sync_filter=invite_filter())
-        print(f"RES IS ============== {res}")
         if isinstance(res, SyncError):
             raise Exception(res.message)
         # restore previous next batch
         self.next_batch = prev_next_batch
         return res.rooms.invite
 
     async def join_room(self, room_id: str) -> None:
@@ -238,42 +241,35 @@
             device_name (str): The device name to register. Defaults to "".
             disable_ratelimiting (bool): Whether or not to disable rate limiting for the user. Defaults to True.
 
         Returns: Access Token for registered user
         """
         matrix_id = matrix_id.lower()
         username = parse_matrix_id(matrix_id)[0]
-        access_token = self.access_token
         res = await super().register_with_token(
             username, password, registration_token, device_name=device_name
         )
         if isinstance(res, RegisterErrorResponse):
             raise Exception(res.message)
 
-        # register will replace the access token that's on the client with the one returned
-        # from a successful registration. We want to keep the original access token.
-        self.access_token = access_token
-
-        if disable_ratelimiting:
-            await self.disable_ratelimiting(matrix_id)
-
         return res.access_token
 
     async def upload_file(
         self,
         file_path: str,
         monitor: Optional[TransferMonitor] = None,
         filename: Optional[str] = None,
     ) -> str:
         """
         Uploads a file to the homeserver.
 
         Args:
             file_path (str): The path to the file to upload.
             monitor (Optional[TransferMonitor]): A transfer monitor to use. Defaults to None.
+            filename (Optional[str]): Uploads the file using this file name. Defaults to None.
 
         Returns:
             str: The content uri of the uploaded file.
         """
         file_stat = await aiofiles_os.stat(file_path)
         logger.info(f"Uploading file: {file_path}")
         async with aiofiles_open(file_path, "r+b") as f:
@@ -283,14 +279,23 @@
                 )
             else:
                 res, _ = await self.upload(f, filesize=file_stat.st_size, filename=filename)
         if isinstance(res, UploadError):
             raise Exception("Failed to upload file.")
         return res.content_uri
 
+    async def set_displayname(self, displayname: str) -> None:
+        # ensure that the provided displayname is not empty as if it is, set_displayname will fail.
+        if not self.user_id:
+            await self.whoami()
+        res = await super().set_displayname(displayname)
+        if isinstance(res, ProfileSetDisplayNameError):
+            raise Exception(res.message)
+        return None
+
 
 class MatrixClient:
     """
     Helper decorator and context manager for use with code
     that communicates with Matrix via matrix-nio's AsyncClient.
 
     Args:
```

### Comparing `fractal_matrix_client-0.0.5/fractal/matrix/exceptions.py` & `fractal_matrix_client-0.0.6/fractal/matrix/exceptions.py`

 * *Files identical despite different names*

### Comparing `fractal_matrix_client-0.0.5/fractal/matrix/utils.py` & `fractal_matrix_client-0.0.6/fractal/matrix/utils.py`

 * *Files identical despite different names*

