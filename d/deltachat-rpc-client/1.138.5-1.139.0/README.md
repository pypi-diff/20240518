# Comparing `tmp/deltachat_rpc_client-1.138.5.tar.gz` & `tmp/deltachat_rpc_client-1.139.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deltachat_rpc_client-1.138.5.tar", last modified: Thu May 16 15:33:23 2024, max compression
+gzip compressed data, was "deltachat_rpc_client-1.139.0.tar", last modified: Sat May 18 19:50:26 2024, max compression
```

## Comparing `deltachat_rpc_client-1.138.5.tar` & `deltachat_rpc_client-1.139.0.tar`

### file list

```diff
@@ -1,34 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 15:33:23.166738 deltachat_rpc_client-1.138.5/
--rw-r--r--   0 runner    (1001) docker     (127)    16726 2024-05-16 15:33:17.000000 deltachat_rpc_client-1.138.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2018 2024-05-16 15:33:23.166738 deltachat_rpc_client-1.138.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1190 2024-05-16 15:33:17.000000 deltachat_rpc_client-1.138.5/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1763 2024-05-16 15:33:17.000000 deltachat_rpc_client-1.138.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-16 15:33:23.166738 deltachat_rpc_client-1.138.5/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 15:33:23.162738 deltachat_rpc_client-1.138.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 15:33:23.162738 deltachat_rpc_client-1.138.5/src/deltachat_rpc_client/
--rw-r--r--   0 runner    (1001) docker     (127)      566 2024-05-16 15:33:17.000000 deltachat_rpc_client-1.138.5/src/deltachat_rpc_client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6304 2024-05-16 15:33:17.000000 deltachat_rpc_client-1.138.5/src/deltachat_rpc_client/_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    13369 2024-05-16 15:33:17.000000 deltachat_rpc_client-1.138.5/src/deltachat_rpc_client/account.py
--rw-r--r--   0 runner    (1001) docker     (127)    10279 2024-05-16 15:33:17.000000 deltachat_rpc_client-1.138.5/src/deltachat_rpc_client/chat.py
--rw-r--r--   0 runner    (1001) docker     (127)     7043 2024-05-16 15:33:17.000000 deltachat_rpc_client-1.138.5/src/deltachat_rpc_client/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     5292 2024-05-16 15:33:17.000000 deltachat_rpc_client-1.138.5/src/deltachat_rpc_client/const.py
--rw-r--r--   0 runner    (1001) docker     (127)     1735 2024-05-16 15:33:17.000000 deltachat_rpc_client-1.138.5/src/deltachat_rpc_client/contact.py
--rw-r--r--   0 runner    (1001) docker     (127)     1538 2024-05-16 15:33:17.000000 deltachat_rpc_client-1.138.5/src/deltachat_rpc_client/deltachat.py
--rw-r--r--   0 runner    (1001) docker     (127)     7808 2024-05-16 15:33:17.000000 deltachat_rpc_client-1.138.5/src/deltachat_rpc_client/direct_imap.py
--rw-r--r--   0 runner    (1001) docker     (127)     9877 2024-05-16 15:33:17.000000 deltachat_rpc_client-1.138.5/src/deltachat_rpc_client/events.py
--rw-r--r--   0 runner    (1001) docker     (127)     2516 2024-05-16 15:33:17.000000 deltachat_rpc_client-1.138.5/src/deltachat_rpc_client/message.py
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-16 15:33:17.000000 deltachat_rpc_client-1.138.5/src/deltachat_rpc_client/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     4059 2024-05-16 15:33:17.000000 deltachat_rpc_client-1.138.5/src/deltachat_rpc_client/pytestplugin.py
--rw-r--r--   0 runner    (1001) docker     (127)     6714 2024-05-16 15:33:17.000000 deltachat_rpc_client-1.138.5/src/deltachat_rpc_client/rpc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 15:33:23.166738 deltachat_rpc_client-1.138.5/src/deltachat_rpc_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2018 2024-05-16 15:33:23.000000 deltachat_rpc_client-1.138.5/src/deltachat_rpc_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      924 2024-05-16 15:33:23.000000 deltachat_rpc_client-1.138.5/src/deltachat_rpc_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 15:33:23.000000 deltachat_rpc_client-1.138.5/src/deltachat_rpc_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-05-16 15:33:23.000000 deltachat_rpc_client-1.138.5/src/deltachat_rpc_client.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-16 15:33:23.000000 deltachat_rpc_client-1.138.5/src/deltachat_rpc_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-16 15:33:23.000000 deltachat_rpc_client-1.138.5/src/deltachat_rpc_client.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 15:33:23.166738 deltachat_rpc_client-1.138.5/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     7581 2024-05-16 15:33:17.000000 deltachat_rpc_client-1.138.5/tests/test_chatlist_events.py
--rw-r--r--   0 runner    (1001) docker     (127)    24172 2024-05-16 15:33:17.000000 deltachat_rpc_client-1.138.5/tests/test_securejoin.py
--rw-r--r--   0 runner    (1001) docker     (127)    22129 2024-05-16 15:33:17.000000 deltachat_rpc_client-1.138.5/tests/test_something.py
--rw-r--r--   0 runner    (1001) docker     (127)     1995 2024-05-16 15:33:17.000000 deltachat_rpc_client-1.138.5/tests/test_webxdc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 19:50:26.836506 deltachat_rpc_client-1.139.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    16726 2024-05-18 19:50:17.000000 deltachat_rpc_client-1.139.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2018 2024-05-18 19:50:26.836506 deltachat_rpc_client-1.139.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1190 2024-05-18 19:50:17.000000 deltachat_rpc_client-1.139.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1763 2024-05-18 19:50:17.000000 deltachat_rpc_client-1.139.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-18 19:50:26.836506 deltachat_rpc_client-1.139.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 19:50:26.832506 deltachat_rpc_client-1.139.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 19:50:26.836506 deltachat_rpc_client-1.139.0/src/deltachat_rpc_client/
+-rw-r--r--   0 runner    (1001) docker     (127)      566 2024-05-18 19:50:17.000000 deltachat_rpc_client-1.139.0/src/deltachat_rpc_client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6304 2024-05-18 19:50:17.000000 deltachat_rpc_client-1.139.0/src/deltachat_rpc_client/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13369 2024-05-18 19:50:17.000000 deltachat_rpc_client-1.139.0/src/deltachat_rpc_client/account.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10659 2024-05-18 19:50:17.000000 deltachat_rpc_client-1.139.0/src/deltachat_rpc_client/chat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7043 2024-05-18 19:50:17.000000 deltachat_rpc_client-1.139.0/src/deltachat_rpc_client/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5312 2024-05-18 19:50:17.000000 deltachat_rpc_client-1.139.0/src/deltachat_rpc_client/const.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1833 2024-05-18 19:50:17.000000 deltachat_rpc_client-1.139.0/src/deltachat_rpc_client/contact.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1538 2024-05-18 19:50:17.000000 deltachat_rpc_client-1.139.0/src/deltachat_rpc_client/deltachat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7808 2024-05-18 19:50:17.000000 deltachat_rpc_client-1.139.0/src/deltachat_rpc_client/direct_imap.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9877 2024-05-18 19:50:17.000000 deltachat_rpc_client-1.139.0/src/deltachat_rpc_client/events.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2516 2024-05-18 19:50:17.000000 deltachat_rpc_client-1.139.0/src/deltachat_rpc_client/message.py
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-18 19:50:17.000000 deltachat_rpc_client-1.139.0/src/deltachat_rpc_client/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     4059 2024-05-18 19:50:17.000000 deltachat_rpc_client-1.139.0/src/deltachat_rpc_client/pytestplugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6714 2024-05-18 19:50:17.000000 deltachat_rpc_client-1.139.0/src/deltachat_rpc_client/rpc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 19:50:26.836506 deltachat_rpc_client-1.139.0/src/deltachat_rpc_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2018 2024-05-18 19:50:26.000000 deltachat_rpc_client-1.139.0/src/deltachat_rpc_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      944 2024-05-18 19:50:26.000000 deltachat_rpc_client-1.139.0/src/deltachat_rpc_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-18 19:50:26.000000 deltachat_rpc_client-1.139.0/src/deltachat_rpc_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-05-18 19:50:26.000000 deltachat_rpc_client-1.139.0/src/deltachat_rpc_client.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-18 19:50:26.000000 deltachat_rpc_client-1.139.0/src/deltachat_rpc_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-18 19:50:26.000000 deltachat_rpc_client-1.139.0/src/deltachat_rpc_client.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 19:50:26.836506 deltachat_rpc_client-1.139.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     7581 2024-05-18 19:50:17.000000 deltachat_rpc_client-1.139.0/tests/test_chatlist_events.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24172 2024-05-18 19:50:17.000000 deltachat_rpc_client-1.139.0/tests/test_securejoin.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22129 2024-05-18 19:50:17.000000 deltachat_rpc_client-1.139.0/tests/test_something.py
+-rw-r--r--   0 runner    (1001) docker     (127)      611 2024-05-18 19:50:17.000000 deltachat_rpc_client-1.139.0/tests/test_vcard.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1995 2024-05-18 19:50:17.000000 deltachat_rpc_client-1.139.0/tests/test_webxdc.py
```

### Comparing `deltachat_rpc_client-1.138.5/LICENSE` & `deltachat_rpc_client-1.139.0/LICENSE`

 * *Files identical despite different names*

### Comparing `deltachat_rpc_client-1.138.5/PKG-INFO` & `deltachat_rpc_client-1.139.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deltachat-rpc-client
-Version: 1.138.5
+Version: 1.139.0
 Summary: Python client for Delta Chat core JSON-RPC interface
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Programming Language :: Python :: 3
```

### Comparing `deltachat_rpc_client-1.138.5/README.md` & `deltachat_rpc_client-1.139.0/README.md`

 * *Files identical despite different names*

### Comparing `deltachat_rpc_client-1.138.5/pyproject.toml` & `deltachat_rpc_client-1.139.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=45"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "deltachat-rpc-client"
-version = "1.138.5"
+version = "1.139.0"
 description = "Python client for Delta Chat core JSON-RPC interface"
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)",
     "Operating System :: POSIX :: Linux",
     "Operating System :: MacOS :: MacOS X",
```

### Comparing `deltachat_rpc_client-1.138.5/src/deltachat_rpc_client/__init__.py` & `deltachat_rpc_client-1.139.0/src/deltachat_rpc_client/__init__.py`

 * *Files identical despite different names*

### Comparing `deltachat_rpc_client-1.138.5/src/deltachat_rpc_client/_utils.py` & `deltachat_rpc_client-1.139.0/src/deltachat_rpc_client/_utils.py`

 * *Files identical despite different names*

### Comparing `deltachat_rpc_client-1.138.5/src/deltachat_rpc_client/account.py` & `deltachat_rpc_client-1.139.0/src/deltachat_rpc_client/account.py`

 * *Files identical despite different names*

### Comparing `deltachat_rpc_client-1.138.5/src/deltachat_rpc_client/chat.py` & `deltachat_rpc_client-1.139.0/src/deltachat_rpc_client/chat.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from __future__ import annotations
 
 import calendar
 from dataclasses import dataclass
+from tempfile import NamedTemporaryFile
 from typing import TYPE_CHECKING, Optional, Union
 
 from ._utils import AttrDict
 from .const import ChatVisibility, ViewType
 from .contact import Contact
 from .message import Message
 
@@ -261,7 +262,15 @@
         for loc in result:
             location = AttrDict(loc)
             location["chat"] = self
             location["contact"] = contacts.setdefault(location.contact_id, Contact(self.account, location.contact_id))
             location["message"] = Message(self.account, location.msg_id)
             locations.append(location)
         return locations
+
+    def send_contact(self, contact: Contact):
+        """Send contact to the chat."""
+        vcard = contact.make_vcard()
+        with NamedTemporaryFile(suffix=".vcard") as f:
+            f.write(vcard.encode())
+            f.flush()
+            self._rpc.send_msg(self.account.id, self.id, {"viewtype": ViewType.VCARD, "file": f.name})
```

### Comparing `deltachat_rpc_client-1.138.5/src/deltachat_rpc_client/client.py` & `deltachat_rpc_client-1.139.0/src/deltachat_rpc_client/client.py`

 * *Files identical despite different names*

### Comparing `deltachat_rpc_client-1.138.5/src/deltachat_rpc_client/const.py` & `deltachat_rpc_client-1.139.0/src/deltachat_rpc_client/const.py`

 * *Files 2% similar despite different names*

```diff
@@ -110,14 +110,15 @@
     STICKER = "Sticker"
     AUDIO = "Audio"
     VOICE = "Voice"
     VIDEO = "Video"
     FILE = "File"
     VIDEOCHAT_INVITATION = "VideochatInvitation"
     WEBXDC = "Webxdc"
+    VCARD = "Vcard"
 
 
 class SystemMessageType(str, Enum):
     """System message type."""
 
     UNKNOWN = "Unknown"
     GROUP_NAME_CHANGED = "GroupNameChanged"
```

### Comparing `deltachat_rpc_client-1.138.5/src/deltachat_rpc_client/contact.py` & `deltachat_rpc_client-1.139.0/src/deltachat_rpc_client/contact.py`

 * *Files 3% similar despite different names*

```diff
@@ -56,7 +56,10 @@
         """Create or get an existing 1:1 chat for this contact."""
         from .chat import Chat
 
         return Chat(
             self.account,
             self._rpc.create_chat_by_contact_id(self.account.id, self.id),
         )
+
+    def make_vcard(self) -> str:
+        return self._rpc.make_vcard(self.account.id, [self.id])
```

### Comparing `deltachat_rpc_client-1.138.5/src/deltachat_rpc_client/deltachat.py` & `deltachat_rpc_client-1.139.0/src/deltachat_rpc_client/deltachat.py`

 * *Files identical despite different names*

### Comparing `deltachat_rpc_client-1.138.5/src/deltachat_rpc_client/direct_imap.py` & `deltachat_rpc_client-1.139.0/src/deltachat_rpc_client/direct_imap.py`

 * *Files identical despite different names*

### Comparing `deltachat_rpc_client-1.138.5/src/deltachat_rpc_client/events.py` & `deltachat_rpc_client-1.139.0/src/deltachat_rpc_client/events.py`

 * *Files identical despite different names*

### Comparing `deltachat_rpc_client-1.138.5/src/deltachat_rpc_client/message.py` & `deltachat_rpc_client-1.139.0/src/deltachat_rpc_client/message.py`

 * *Files identical despite different names*

### Comparing `deltachat_rpc_client-1.138.5/src/deltachat_rpc_client/pytestplugin.py` & `deltachat_rpc_client-1.139.0/src/deltachat_rpc_client/pytestplugin.py`

 * *Files identical despite different names*

### Comparing `deltachat_rpc_client-1.138.5/src/deltachat_rpc_client/rpc.py` & `deltachat_rpc_client-1.139.0/src/deltachat_rpc_client/rpc.py`

 * *Files identical despite different names*

### Comparing `deltachat_rpc_client-1.138.5/src/deltachat_rpc_client.egg-info/PKG-INFO` & `deltachat_rpc_client-1.139.0/src/deltachat_rpc_client.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deltachat-rpc-client
-Version: 1.138.5
+Version: 1.139.0
 Summary: Python client for Delta Chat core JSON-RPC interface
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Programming Language :: Python :: 3
```

### Comparing `deltachat_rpc_client-1.138.5/src/deltachat_rpc_client.egg-info/SOURCES.txt` & `deltachat_rpc_client-1.139.0/src/deltachat_rpc_client.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -20,8 +20,9 @@
 src/deltachat_rpc_client.egg-info/dependency_links.txt
 src/deltachat_rpc_client.egg-info/entry_points.txt
 src/deltachat_rpc_client.egg-info/requires.txt
 src/deltachat_rpc_client.egg-info/top_level.txt
 tests/test_chatlist_events.py
 tests/test_securejoin.py
 tests/test_something.py
+tests/test_vcard.py
 tests/test_webxdc.py
```

### Comparing `deltachat_rpc_client-1.138.5/tests/test_chatlist_events.py` & `deltachat_rpc_client-1.139.0/tests/test_chatlist_events.py`

 * *Files identical despite different names*

### Comparing `deltachat_rpc_client-1.138.5/tests/test_securejoin.py` & `deltachat_rpc_client-1.139.0/tests/test_securejoin.py`

 * *Files identical despite different names*

### Comparing `deltachat_rpc_client-1.138.5/tests/test_something.py` & `deltachat_rpc_client-1.139.0/tests/test_something.py`

 * *Files identical despite different names*

### Comparing `deltachat_rpc_client-1.138.5/tests/test_webxdc.py` & `deltachat_rpc_client-1.139.0/tests/test_webxdc.py`

 * *Files identical despite different names*

