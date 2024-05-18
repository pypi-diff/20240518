# Comparing `tmp/omuplugin_onecomme-0.3.2.tar.gz` & `tmp/omuplugin_onecomme-0.4.2.tar.gz`

## Comparing `omuplugin_onecomme-0.3.2.tar` & `omuplugin_onecomme-0.4.2.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 omuplugin_onecomme-0.3.2/src/omuplugin_onecomme/__init__.py
--rw-r--r--   0        0        0     1795 2020-02-02 00:00:00.000000 omuplugin_onecomme-0.3.2/src/omuplugin_onecomme/onecomme.py
--rw-r--r--   0        0        0     6015 2020-02-02 00:00:00.000000 omuplugin_onecomme-0.3.2/src/omuplugin_onecomme/plugin.py
--rw-r--r--   0        0        0      904 2020-02-02 00:00:00.000000 omuplugin_onecomme-0.3.2/src/omuplugin_onecomme/types.py
--rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 omuplugin_onecomme-0.3.2/src/omuplugin_onecomme/version.py
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 omuplugin_onecomme-0.3.2/.gitignore
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 omuplugin_onecomme-0.3.2/README.md
--rw-r--r--   0        0        0      541 2020-02-02 00:00:00.000000 omuplugin_onecomme-0.3.2/pyproject.toml
--rw-r--r--   0        0        0      327 2020-02-02 00:00:00.000000 omuplugin_onecomme-0.3.2/PKG-INFO
+-rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 omuplugin_onecomme-0.4.2/src/omuplugin_onecomme/__init__.py
+-rw-r--r--   0        0        0     1835 2020-02-02 00:00:00.000000 omuplugin_onecomme-0.4.2/src/omuplugin_onecomme/onecomme.py
+-rw-r--r--   0        0        0     6028 2020-02-02 00:00:00.000000 omuplugin_onecomme-0.4.2/src/omuplugin_onecomme/plugin.py
+-rw-r--r--   0        0        0      904 2020-02-02 00:00:00.000000 omuplugin_onecomme-0.4.2/src/omuplugin_onecomme/types.py
+-rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 omuplugin_onecomme-0.4.2/src/omuplugin_onecomme/version.py
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 omuplugin_onecomme-0.4.2/.gitignore
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 omuplugin_onecomme-0.4.2/README.md
+-rw-r--r--   0        0        0      542 2020-02-02 00:00:00.000000 omuplugin_onecomme-0.4.2/pyproject.toml
+-rw-r--r--   0        0        0      328 2020-02-02 00:00:00.000000 omuplugin_onecomme-0.4.2/PKG-INFO
```

### Comparing `omuplugin_onecomme-0.3.2/src/omuplugin_onecomme/onecomme.py` & `omuplugin_onecomme-0.4.2/src/omuplugin_onecomme/onecomme.py`

 * *Files 4% similar despite different names*

```diff
@@ -48,13 +48,13 @@
     terminate_onecomme()
     # https://onecomme.com/news/#:~:text=--disable-api-server%3A%20APIサーバーを起動しない
     bin = find_onecomme_binary()
     if bin is None:
         raise FileNotFoundError("OneComme binary not found")
     await asyncio.create_subprocess_exec(
         bin,
-        "",  # empty args for issue
+        "",  # empty args for issue https://forum.onecomme.com/t/topic/1641
         "--disable-api-server",
         stdout=asyncio.subprocess.PIPE,
         stderr=asyncio.subprocess.PIPE,
     )
     logger.info("OneComme started")
```

### Comparing `omuplugin_onecomme-0.3.2/src/omuplugin_onecomme/plugin.py` & `omuplugin_onecomme-0.4.2/src/omuplugin_onecomme/plugin.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,24 +3,26 @@
 import asyncio
 import socket
 from html import escape
 from typing import TypedDict
 
 from aiohttp import web
 from loguru import logger
-from omuchat import App, Client, events, model
-from omuchat.model import content
+from omu import App, Omu
+from omu_chat import Chat, events, model
+from omu_chat.model import content
 
 from .types import Badge, Comment, CommentData, CommentServiceData
 
 APP = App(
-    "cc.omuchat:onecomme/plugin",
+    "com.omuapps:onecomme/plugin",
     version="0.1.0",
 )
-client = Client(APP)
+client = Omu(APP)
+chat = Chat(client)
 app = web.Application()
 
 
 def format_content(*components: content.Component | None) -> str:
     if components is None:
         return ""
     if len(components) == 0:
@@ -47,18 +49,18 @@
             parts.append(f"<span>{format_content(*component.get_children())}</span>")
         else:
             raise ValueError(f"Unknown component type: {component}")
     return "".join(parts)
 
 
 async def to_comment(message: model.Message) -> Comment | None:
-    room = await client.chat.rooms.get(message.room_id.key())
+    room = await chat.rooms.get(message.room_id.key())
     author: model.Author | None = None
     if message.author_id:
-        author = await client.chat.authors.get(message.author_id.key())
+        author = await chat.authors.get(message.author_id.key())
     if not room or not author:
         return None
     metadata = room.metadata or {}
     badges = []
     for badge in author.roles:
         if badge.icon_url:
             badges.append(
@@ -114,15 +116,15 @@
 
 
 async def handle(request: web.Request) -> web.WebSocketResponse:
     ws = web.WebSocketResponse()
     await ws.prepare(request)
     messages = [
         await to_comment(message)
-        for message in (await client.chat.messages.fetch_items(before=35)).values()
+        for message in (await chat.messages.fetch_items(before=35)).values()
     ]
     await ws.send_json(
         {
             "type": "connected",
             "data": CommentsData(
                 comments=list(reversed(tuple(filter(None, messages))))
             ),
@@ -136,15 +138,15 @@
             elif msg.type == web.WSMsgType.ERROR:
                 logger.error("ws connection closed with exception %s", ws.exception())
     finally:
         sessions.remove(ws)
     return ws
 
 
-@client.on(events.message.add)
+@chat.on(events.message.add)
 async def on_message_add(message: model.Message) -> None:
     comment = await to_comment(message)
     if not comment:
         return
     for ws in sessions:
         await ws.send_json(
             {
@@ -152,15 +154,15 @@
                 "data": CommentsData(
                     comments=[comment],
                 ),
             }
         )
 
 
-@client.on(events.message.update)
+@chat.on(events.message.update)
 async def on_message_update(message: model.Message) -> None:
     comment = await to_comment(message)
     if comment is None:
         return
     for ws in sessions:
         await ws.send_json(
             {
@@ -168,15 +170,15 @@
                 "data": CommentsData(
                     comments=[comment],
                 ),
             }
         )
 
 
-@client.on(events.message.remove)
+@chat.on(events.message.remove)
 async def on_message_delete(message: model.Message) -> None:
     for ws in sessions:
         await ws.send_json({"type": "deleted", "data": [message.key()]})
 
 
 def is_port_free() -> bool:
     try:
@@ -188,15 +190,15 @@
                 )
             )
             return True
     except OSError:
         return False
 
 
-@client.on(events.ready)
+@client.event.ready.listen
 async def on_ready():
     port_free = is_port_free()
     if not port_free:
         raise OSError("Port 11180 already in use")
     app.add_routes([web.get("/sub", handle)])
     runner = web.AppRunner(app)
     await runner.setup()
```

### Comparing `omuplugin_onecomme-0.3.2/src/omuplugin_onecomme/types.py` & `omuplugin_onecomme-0.4.2/src/omuplugin_onecomme/types.py`

 * *Files identical despite different names*

### Comparing `omuplugin_onecomme-0.3.2/pyproject.toml` & `omuplugin_onecomme-0.4.2/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [project]
 name = "omuplugin_onecomme"
-version = "0.3.2"
+version = "0.4.2"
 description = "Add your description here"
 authors = [
     { name = "am230", email = "111672334+am230@users.noreply.github.com" },
 ]
-dependencies = ["loguru>=0.7.2", "omuchat>=0.1.9"]
+dependencies = ["loguru>=0.7.2", "omu_chat>=0.1.9"]
 readme = "README.md"
 requires-python = ">= 3.12"
 
 [project.entry-points."omu.plugins"]
 plugin = "omuplugin_onecomme:plugin"
 
 [build-system]
```

