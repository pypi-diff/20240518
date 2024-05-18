# Comparing `tmp/omuplugin_translator-0.3.2.tar.gz` & `tmp/omuplugin_translator-0.4.2.tar.gz`

## Comparing `omuplugin_translator-0.3.2.tar` & `omuplugin_translator-0.4.2.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 omuplugin_translator-0.3.2/src/omuplugin_translator/__init__.py
--rw-r--r--   0        0        0     3051 2020-02-02 00:00:00.000000 omuplugin_translator-0.3.2/src/omuplugin_translator/plugin.py
--rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 omuplugin_translator-0.3.2/src/omuplugin_translator/version.py
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 omuplugin_translator-0.3.2/.gitignore
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 omuplugin_translator-0.3.2/README.md
--rw-r--r--   0        0        0      565 2020-02-02 00:00:00.000000 omuplugin_translator-0.3.2/pyproject.toml
--rw-r--r--   0        0        0      361 2020-02-02 00:00:00.000000 omuplugin_translator-0.3.2/PKG-INFO
+-rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 omuplugin_translator-0.4.2/src/omuplugin_translator/__init__.py
+-rw-r--r--   0        0        0     2998 2020-02-02 00:00:00.000000 omuplugin_translator-0.4.2/src/omuplugin_translator/plugin.py
+-rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 omuplugin_translator-0.4.2/src/omuplugin_translator/version.py
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 omuplugin_translator-0.4.2/.gitignore
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 omuplugin_translator-0.4.2/README.md
+-rw-r--r--   0        0        0      566 2020-02-02 00:00:00.000000 omuplugin_translator-0.4.2/pyproject.toml
+-rw-r--r--   0        0        0      362 2020-02-02 00:00:00.000000 omuplugin_translator-0.4.2/PKG-INFO
```

### Comparing `omuplugin_translator-0.3.2/src/omuplugin_translator/plugin.py` & `omuplugin_translator-0.4.2/src/omuplugin_translator/plugin.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,38 +1,38 @@
 from __future__ import annotations
 
 from typing import TypedDict
 
 from edgetrans import EdgeTranslator, Language, Translator
 from loguru import logger
-from omu.identifier import Identifier
-from omuchat import App, Client, model
-from omuchat.event.event_types import events
-from omuchat.model.content import Component, Root, System, Text
+from omu import App, Identifier, Omu
+from omu_chat import Chat, model
+from omu_chat.model.content import Component, Root, System, Text
 
-IDENTIFIER = Identifier("cc.omuchat", "translator", "plugin")
+IDENTIFIER = Identifier("com.omuapps", "translator", "plugin")
 APP = App(
     IDENTIFIER,
     version="0.1.0",
 )
-client = Client(APP)
+omu = Omu(APP)
+chat = Chat(omu)
 
 translator: Translator | None = None
 
 
 class TrasnlatorConfig(TypedDict):
     active: bool
     languages: list[Language]
 
 
 config = TrasnlatorConfig(
     active=False,
     languages=["ja", "en"],
 )
-CONFIG_REGISTRY_TYPE = client.registry.create("config", config)
+CONFIG_REGISTRY_TYPE = omu.registry.create("config", config)
 
 
 @CONFIG_REGISTRY_TYPE.listen
 async def on_config_change(new_config: TrasnlatorConfig):
     global config
     config = new_config
     logger.info(f"translator config updated: {config}")
@@ -58,15 +58,15 @@
     ]
     texts_b = [
         sibling.text.lower() for sibling in b.iter() if isinstance(sibling, Text)
     ]
     return all(a == b for a, b in zip(texts_a, texts_b, strict=False))
 
 
-@client.chat.messages.proxy
+@chat.messages.proxy
 async def on_message_add(message: model.Message) -> model.Message:
     if not config["active"]:
         return message
     if not message.content:
         return message
     translations: dict[str, Component] = {}
     if len(config["languages"]) == 1:
@@ -90,16 +90,16 @@
             translated,
         ]
         content.add(System(lines))
     message.content = content
     return message
 
 
-@client.on(events.ready)
+@omu.event.ready.listen
 async def on_ready():
     global translator, config
     config = await CONFIG_REGISTRY_TYPE.get()
     translator = await EdgeTranslator.create()
 
 
 if __name__ == "__main__":
-    client.run()
+    omu.run()
```

### Comparing `omuplugin_translator-0.3.2/pyproject.toml` & `omuplugin_translator-0.4.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [project]
 name = "omuplugin_translator"
-version = "0.3.2"
+version = "0.4.2"
 description = "Add your description here"
 authors = [
     { name = "am230", email = "111672334+am230@users.noreply.github.com" },
 ]
-dependencies = ["loguru>=0.7.2", "edgetrans>=0.2.3", "omuchat>=0.1.9"]
+dependencies = ["loguru>=0.7.2", "edgetrans>=0.2.3", "omu_chat>=0.1.9"]
 readme = "README.md"
 requires-python = ">= 3.12"
 
 [project.entry-points."omu.plugins"]
 plugin = "omuplugin_translator:plugin"
 
 [build-system]
```

