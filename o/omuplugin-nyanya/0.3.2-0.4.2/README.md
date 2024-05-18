# Comparing `tmp/omuplugin_nyanya-0.3.2.tar.gz` & `tmp/omuplugin_nyanya-0.4.2.tar.gz`

## Comparing `omuplugin_nyanya-0.3.2.tar` & `omuplugin_nyanya-0.4.2.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 omuplugin_nyanya-0.3.2/src/omuplugin_nyanya/__init__.py
--rw-r--r--   0        0        0      847 2020-02-02 00:00:00.000000 omuplugin_nyanya-0.3.2/src/omuplugin_nyanya/plugin.py
--rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 omuplugin_nyanya-0.3.2/src/omuplugin_nyanya/version.py
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 omuplugin_nyanya-0.3.2/.gitignore
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 omuplugin_nyanya-0.3.2/README.md
--rw-r--r--   0        0        0      537 2020-02-02 00:00:00.000000 omuplugin_nyanya-0.3.2/pyproject.toml
--rw-r--r--   0        0        0      325 2020-02-02 00:00:00.000000 omuplugin_nyanya-0.3.2/PKG-INFO
+-rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 omuplugin_nyanya-0.4.2/src/omuplugin_nyanya/__init__.py
+-rw-r--r--   0        0        0      842 2020-02-02 00:00:00.000000 omuplugin_nyanya-0.4.2/src/omuplugin_nyanya/plugin.py
+-rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 omuplugin_nyanya-0.4.2/src/omuplugin_nyanya/version.py
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 omuplugin_nyanya-0.4.2/.gitignore
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 omuplugin_nyanya-0.4.2/README.md
+-rw-r--r--   0        0        0      538 2020-02-02 00:00:00.000000 omuplugin_nyanya-0.4.2/pyproject.toml
+-rw-r--r--   0        0        0      326 2020-02-02 00:00:00.000000 omuplugin_nyanya-0.4.2/PKG-INFO
```

### Comparing `omuplugin_nyanya-0.3.2/src/omuplugin_nyanya/plugin.py` & `omuplugin_nyanya-0.4.2/src/omuplugin_nyanya/plugin.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 from __future__ import annotations
 
-from omu.identifier import Identifier
-from omuchat import App, Client, content, model
+from omu import App, Identifier, Omu
+from omu_chat import Chat, content, model
 
-IDENTIFIER = Identifier("cc.omuchat", "plugin-nyanya")
+IDENTIFIER = Identifier("com.omuapps", "plugin-nyanya")
 APP = App(
     IDENTIFIER,
     version="0.1.0",
 )
-client = Client(APP)
+omu = Omu(APP)
+chat = Chat(omu)
 replaces = {
     "な": "にゃ",
     "ナ": "ニャ",
 }
 
 
 async def translate(
@@ -21,17 +22,17 @@
     for child in component.iter():
         if not isinstance(child, content.Text):
             continue
         child.text = child.text.translate(str.maketrans(replaces))
     return component
 
 
-@client.chat.messages.proxy
+@chat.messages.proxy
 async def on_message_add(message: model.Message) -> model.Message:
     if not message.content:
         return message
     message.content = await translate(message.content)
     return message
 
 
 if __name__ == "__main__":
-    client.run()
+    omu.run()
```

### Comparing `omuplugin_nyanya-0.3.2/pyproject.toml` & `omuplugin_nyanya-0.4.2/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [project]
 name = "omuplugin_nyanya"
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
 plugin = "omuplugin_nyanya:plugin"
 
 [build-system]
```

