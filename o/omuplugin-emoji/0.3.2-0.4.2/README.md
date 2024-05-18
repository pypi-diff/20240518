# Comparing `tmp/omuplugin_emoji-0.3.2.tar.gz` & `tmp/omuplugin_emoji-0.4.2.tar.gz`

## Comparing `omuplugin_emoji-0.3.2.tar` & `omuplugin_emoji-0.4.2.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 omuplugin_emoji-0.3.2/src/omuplugin_emoji/__init__.py
--rw-r--r--   0        0        0     5581 2020-02-02 00:00:00.000000 omuplugin_emoji-0.3.2/src/omuplugin_emoji/plugin.py
--rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 omuplugin_emoji-0.3.2/src/omuplugin_emoji/version.py
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 omuplugin_emoji-0.3.2/.gitignore
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 omuplugin_emoji-0.3.2/README.md
--rw-r--r--   0        0        0      535 2020-02-02 00:00:00.000000 omuplugin_emoji-0.3.2/pyproject.toml
--rw-r--r--   0        0        0      324 2020-02-02 00:00:00.000000 omuplugin_emoji-0.3.2/PKG-INFO
+-rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 omuplugin_emoji-0.4.2/src/omuplugin_emoji/__init__.py
+-rw-r--r--   0        0        0     5505 2020-02-02 00:00:00.000000 omuplugin_emoji-0.4.2/src/omuplugin_emoji/plugin.py
+-rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 omuplugin_emoji-0.4.2/src/omuplugin_emoji/version.py
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 omuplugin_emoji-0.4.2/.gitignore
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 omuplugin_emoji-0.4.2/README.md
+-rw-r--r--   0        0        0      536 2020-02-02 00:00:00.000000 omuplugin_emoji-0.4.2/pyproject.toml
+-rw-r--r--   0        0        0      325 2020-02-02 00:00:00.000000 omuplugin_emoji-0.4.2/PKG-INFO
```

### Comparing `omuplugin_emoji-0.3.2/src/omuplugin_emoji/plugin.py` & `omuplugin_emoji-0.4.2/src/omuplugin_emoji/plugin.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,40 +1,39 @@
 import re
 from collections.abc import Mapping
 from dataclasses import dataclass
 from typing import Literal, TypedDict
 
 from loguru import logger
-from omu.extension.table.table import TableType
-from omu.identifier import Identifier
+from omu import App, Identifier, Omu
+from omu.extension.table import TableType
 from omu.interface.keyable import Keyable
 from omu.model import Model
-from omuchat import App, Client
-from omuchat.event.event_types import events
-from omuchat.model import content
-from omuchat.model.message import Message
+from omu_chat import Chat
+from omu_chat.model import Message, content
 
-IDENTIFIER = Identifier("cc.omuchat", "emoji", "plugin")
+IDENTIFIER = Identifier("com.omuapps", "emoji", "plugin")
 APP = App(
     IDENTIFIER,
     version="0.1.0",
 )
-client = Client(APP)
+omu = Omu(APP)
+chat = Chat(omu)
 
 
 class EmojiConfig(TypedDict):
     active: bool
 
 
 config = EmojiConfig(
     active=False,
 )
 
 
-@client.registry.create("config", config).listen
+@omu.registry.create("config", config).listen
 async def on_config_change(new_config: EmojiConfig):
     global config
     config = new_config
     logger.info(f"emoji config updated: {config}")
 
 
 class TextPattern(TypedDict):
@@ -92,15 +91,15 @@
 
 
 EMOJI_TABLE_TYPE = TableType.create_model(
     IDENTIFIER,
     name="emoji",
     model_type=Emoji,
 )
-emoji_table = client.tables.get(EMOJI_TABLE_TYPE)
+emoji_table = omu.tables.get(EMOJI_TABLE_TYPE)
 emoji_table.set_cache_size(1000)
 
 
 class Patterns:
     text: list[tuple[TextPattern, Emoji]] = []
     image: list[tuple[ImagePattern, Emoji]] = []
     regex: list[tuple[RegexPattern, Emoji]] = []
@@ -118,15 +117,15 @@
                 Patterns.text.append((pattern, emoji))
             elif pattern["type"] == "image":
                 Patterns.image.append((pattern, emoji))
             elif pattern["type"] == "regex":
                 Patterns.regex.append((pattern, emoji))
 
 
-@dataclass
+@dataclass(frozen=True, slots=True)
 class EmojiMatch:
     start: int
     end: int
     emoji: Emoji
 
 
 def transform(component: content.Component) -> content.Component:
@@ -135,15 +134,15 @@
         if len(parts) == 1:
             return parts[0]
         return content.Root(parts)
     if isinstance(component, content.Image):
         for pattern, emoji in Patterns.image:
             if component.id == pattern["id"]:
                 return content.Image.of(
-                    url=client.assets.url(emoji.asset),
+                    url=omu.assets.url(emoji.asset),
                     id=emoji.id,
                 )
     if isinstance(component, content.Parent):
         component.set_children(
             [transform(sibling) for sibling in component.get_children()]
         )
     return component
@@ -159,15 +158,15 @@
         if not match:
             parts.append(content.Text.of(text))
             break
         if match.start > 0:
             parts.append(content.Text.of(text[: match.start]))
         parts.append(
             content.Image.of(
-                url=client.assets.url(match.emoji.asset),
+                url=omu.assets.url(match.emoji.asset),
                 id=match.emoji.id,
             )
         )
         text = text[match.end :]
     return parts
 
 
@@ -199,24 +198,24 @@
         if not match or result.start() < match.start:
             match = EmojiMatch(result.start(), result.end(), asset)
         if match.start == 0:
             break
     return match
 
 
-@client.chat.messages.proxy
+@chat.messages.proxy
 async def on_message(message: Message):
     if not config["active"]:
         return message
     if not message.content:
         return message
     message.content = transform(message.content)
     return message
 
 
-@client.on(events.ready)
+@omu.event.ready.listen
 async def ready():
     await emoji_table.fetch_all()
 
 
 if __name__ == "__main__":
-    client.run()
+    omu.run()
```

### Comparing `omuplugin_emoji-0.3.2/pyproject.toml` & `omuplugin_emoji-0.4.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [project]
 name = "omuplugin_emoji"
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
 plugin = "omuplugin_emoji:plugin"
 
 [build-system]
```

