# Comparing `tmp/omuplugin_chat-0.3.2.tar.gz` & `tmp/omuplugin_chat-0.4.2.tar.gz`

## Comparing `omuplugin_chat-0.3.2.tar` & `omuplugin_chat-0.4.2.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 omuplugin_chat-0.3.2/src/omuplugin_chat/__init__.py
--rw-r--r--   0        0        0     3922 2020-02-02 00:00:00.000000 omuplugin_chat-0.3.2/src/omuplugin_chat/plugin.py
--rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 omuplugin_chat-0.3.2/src/omuplugin_chat/version.py
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 omuplugin_chat-0.3.2/.gitignore
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 omuplugin_chat-0.3.2/README.md
--rw-r--r--   0        0        0      550 2020-02-02 00:00:00.000000 omuplugin_chat-0.3.2/pyproject.toml
--rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 omuplugin_chat-0.3.2/PKG-INFO
+-rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 omuplugin_chat-0.4.2/src/omuplugin_chat/__init__.py
+-rw-r--r--   0        0        0     3894 2020-02-02 00:00:00.000000 omuplugin_chat-0.4.2/src/omuplugin_chat/plugin.py
+-rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 omuplugin_chat-0.4.2/src/omuplugin_chat/version.py
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 omuplugin_chat-0.4.2/.gitignore
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 omuplugin_chat-0.4.2/README.md
+-rw-r--r--   0        0        0      551 2020-02-02 00:00:00.000000 omuplugin_chat-0.4.2/pyproject.toml
+-rw-r--r--   0        0        0      353 2020-02-02 00:00:00.000000 omuplugin_chat-0.4.2/PKG-INFO
```

### Comparing `omuplugin_chat-0.3.2/src/omuplugin_chat/plugin.py` & `omuplugin_chat-0.4.2/src/omuplugin_chat/plugin.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,37 +1,36 @@
 import re
 
 import iwashi
-from omu import Address, OmuClient
+from omu import Address, App, Omu
 from omu.extension.permission import PermissionType
-from omuchat import App
-from omuchat.chat import (
+from omu_chat.chat import (
     AUTHOR_TABLE,
     CHANNEL_TABLE,
     CREATE_CHANNEL_TREE_ENDPOINT,
     IDENTIFIER,
     MESSAGE_TABLE,
     PROVIDER_TABLE,
     ROOM_TABLE,
 )
-from omuchat.model.channel import Channel
-from omuchat.permissions import (
+from omu_chat.model.channel import Channel
+from omu_chat.permissions import (
     CHAT_CHANNEL_TREE_PERMISSION_ID,
     CHAT_PERMISSION_ID,
     CHAT_READ_PERMISSION_ID,
     CHAT_SEND_PERMISSION_ID,
     CHAT_WRITE_PERMISSION_ID,
 )
 
 app = App(
     IDENTIFIER,
     version="0.1.0",
 )
 address = Address("127.0.0.1", 26423)
-client = OmuClient(app, address=address)
+client = Omu(app, address=address)
 
 client.permissions.register(
     PermissionType(
         CHAT_PERMISSION_ID,
         metadata={
             "level": "medium",
             "name": {
```

### Comparing `omuplugin_chat-0.3.2/pyproject.toml` & `omuplugin_chat-0.4.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [project]
 name = "omuplugin_chat"
-version = "0.3.2"
+version = "0.4.2"
 description = "Add your description here"
 authors = [
     { name = "am230", email = "111672334+am230@users.noreply.github.com" },
 ]
-dependencies = ["loguru>=0.7.2", "omuchat>=0.1.9", "iwashi>=3.0.2"]
+dependencies = ["loguru>=0.7.2", "omu_chat>=0.1.9", "iwashi>=3.0.4"]
 readme = "README.md"
 requires-python = ">= 3.12"
 
 [project.entry-points."omu.plugins"]
 plugin = "omuplugin_chat:plugin"
 
 [build-system]
```

