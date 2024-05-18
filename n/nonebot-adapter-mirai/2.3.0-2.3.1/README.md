# Comparing `tmp/nonebot_adapter_mirai-2.3.0.tar.gz` & `tmp/nonebot_adapter_mirai-2.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_adapter_mirai-2.3.0.tar", last modified: Tue May 14 16:55:11 2024, max compression
+gzip compressed data, was "nonebot_adapter_mirai-2.3.1.tar", last modified: Sat May 18 07:08:34 2024, max compression
```

## Comparing `nonebot_adapter_mirai-2.3.0.tar` & `nonebot_adapter_mirai-2.3.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0    34523 2024-05-14 16:54:46.947192 nonebot_adapter_mirai-2.3.0/LICENSE
--rw-r--r--   0        0        0     1300 2024-05-14 16:54:46.947192 nonebot_adapter_mirai-2.3.0/README.md
--rw-r--r--   0        0        0      244 2024-05-14 16:54:46.947192 nonebot_adapter_mirai-2.3.0/nonebot/adapters/mirai/__init__.py
--rw-r--r--   0        0        0    11812 2024-05-14 16:54:46.947192 nonebot_adapter_mirai-2.3.0/nonebot/adapters/mirai/adapter.py
--rw-r--r--   0        0        0    55508 2024-05-14 16:54:46.947192 nonebot_adapter_mirai-2.3.0/nonebot/adapters/mirai/bot.py
--rw-r--r--   0        0        0     1463 2024-05-14 16:54:46.947192 nonebot_adapter_mirai-2.3.0/nonebot/adapters/mirai/compat.py
--rw-r--r--   0        0        0      923 2024-05-14 16:54:46.947192 nonebot_adapter_mirai-2.3.0/nonebot/adapters/mirai/config.py
--rw-r--r--   0        0        0    30053 2024-05-14 16:54:46.947192 nonebot_adapter_mirai-2.3.0/nonebot/adapters/mirai/event.py
--rw-r--r--   0        0        0     3117 2024-05-14 16:54:46.951192 nonebot_adapter_mirai-2.3.0/nonebot/adapters/mirai/exception.py
--rw-r--r--   0        0        0    19490 2024-05-14 16:54:46.951192 nonebot_adapter_mirai-2.3.0/nonebot/adapters/mirai/message.py
--rw-r--r--   0        0        0      601 2024-05-14 16:54:46.951192 nonebot_adapter_mirai-2.3.0/nonebot/adapters/mirai/model/__init__.py
--rw-r--r--   0        0        0     1548 2024-05-14 16:54:46.951192 nonebot_adapter_mirai-2.3.0/nonebot/adapters/mirai/model/base.py
--rw-r--r--   0        0        0     2762 2024-05-14 16:54:46.951192 nonebot_adapter_mirai-2.3.0/nonebot/adapters/mirai/model/common.py
--rw-r--r--   0        0        0     8816 2024-05-14 16:54:46.951192 nonebot_adapter_mirai-2.3.0/nonebot/adapters/mirai/model/relationship.py
--rw-r--r--   0        0        0     2559 2024-05-14 16:54:46.951192 nonebot_adapter_mirai-2.3.0/nonebot/adapters/mirai/utils.py
--rw-r--r--   0        0        0     2263 2024-05-14 16:55:11.223346 nonebot_adapter_mirai-2.3.0/pyproject.toml
--rw-r--r--   0        0        0        0 2024-05-14 16:54:46.951192 nonebot_adapter_mirai-2.3.0/tests/__init__.py
--rw-r--r--   0        0        0     2259 1970-01-01 00:00:00.000000 nonebot_adapter_mirai-2.3.0/PKG-INFO
+-rw-r--r--   0        0        0    34523 2024-05-18 07:08:12.374980 nonebot_adapter_mirai-2.3.1/LICENSE
+-rw-r--r--   0        0        0     1300 2024-05-18 07:08:12.374980 nonebot_adapter_mirai-2.3.1/README.md
+-rw-r--r--   0        0        0      244 2024-05-18 07:08:12.374980 nonebot_adapter_mirai-2.3.1/nonebot/adapters/mirai/__init__.py
+-rw-r--r--   0        0        0    11812 2024-05-18 07:08:12.374980 nonebot_adapter_mirai-2.3.1/nonebot/adapters/mirai/adapter.py
+-rw-r--r--   0        0        0    55508 2024-05-18 07:08:12.374980 nonebot_adapter_mirai-2.3.1/nonebot/adapters/mirai/bot.py
+-rw-r--r--   0        0        0     1463 2024-05-18 07:08:12.374980 nonebot_adapter_mirai-2.3.1/nonebot/adapters/mirai/compat.py
+-rw-r--r--   0        0        0      923 2024-05-18 07:08:12.374980 nonebot_adapter_mirai-2.3.1/nonebot/adapters/mirai/config.py
+-rw-r--r--   0        0        0    30053 2024-05-18 07:08:12.374980 nonebot_adapter_mirai-2.3.1/nonebot/adapters/mirai/event.py
+-rw-r--r--   0        0        0     3117 2024-05-18 07:08:12.374980 nonebot_adapter_mirai-2.3.1/nonebot/adapters/mirai/exception.py
+-rw-r--r--   0        0        0    20300 2024-05-18 07:08:12.374980 nonebot_adapter_mirai-2.3.1/nonebot/adapters/mirai/message.py
+-rw-r--r--   0        0        0      601 2024-05-18 07:08:12.374980 nonebot_adapter_mirai-2.3.1/nonebot/adapters/mirai/model/__init__.py
+-rw-r--r--   0        0        0     1548 2024-05-18 07:08:12.374980 nonebot_adapter_mirai-2.3.1/nonebot/adapters/mirai/model/base.py
+-rw-r--r--   0        0        0     2762 2024-05-18 07:08:12.378980 nonebot_adapter_mirai-2.3.1/nonebot/adapters/mirai/model/common.py
+-rw-r--r--   0        0        0     8816 2024-05-18 07:08:12.378980 nonebot_adapter_mirai-2.3.1/nonebot/adapters/mirai/model/relationship.py
+-rw-r--r--   0        0        0     2559 2024-05-18 07:08:12.378980 nonebot_adapter_mirai-2.3.1/nonebot/adapters/mirai/utils.py
+-rw-r--r--   0        0        0     2263 2024-05-18 07:08:34.610996 nonebot_adapter_mirai-2.3.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-18 07:08:12.378980 nonebot_adapter_mirai-2.3.1/tests/__init__.py
+-rw-r--r--   0        0        0     2259 1970-01-01 00:00:00.000000 nonebot_adapter_mirai-2.3.1/PKG-INFO
```

### Comparing `nonebot_adapter_mirai-2.3.0/LICENSE` & `nonebot_adapter_mirai-2.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_mirai-2.3.0/README.md` & `nonebot_adapter_mirai-2.3.1/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_mirai-2.3.0/nonebot/adapters/mirai/adapter.py` & `nonebot_adapter_mirai-2.3.1/nonebot/adapters/mirai/adapter.py`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_mirai-2.3.0/nonebot/adapters/mirai/bot.py` & `nonebot_adapter_mirai-2.3.1/nonebot/adapters/mirai/bot.py`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_mirai-2.3.0/nonebot/adapters/mirai/compat.py` & `nonebot_adapter_mirai-2.3.1/nonebot/adapters/mirai/compat.py`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_mirai-2.3.0/nonebot/adapters/mirai/config.py` & `nonebot_adapter_mirai-2.3.1/nonebot/adapters/mirai/config.py`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_mirai-2.3.0/nonebot/adapters/mirai/event.py` & `nonebot_adapter_mirai-2.3.1/nonebot/adapters/mirai/event.py`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_mirai-2.3.0/nonebot/adapters/mirai/exception.py` & `nonebot_adapter_mirai-2.3.1/nonebot/adapters/mirai/exception.py`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_mirai-2.3.0/nonebot/adapters/mirai/message.py` & `nonebot_adapter_mirai-2.3.1/nonebot/adapters/mirai/message.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from io import BytesIO
 from pathlib import Path
 from base64 import b64encode
 from datetime import datetime
 from collections.abc import Iterable
 from typing_extensions import override
 from dataclasses import field, dataclass
-from typing import Union, Literal, ClassVar, Optional, TypedDict, overload
+from typing import Union, Literal, ClassVar, Optional, TypedDict, cast, overload
 
 from nonebot.adapters import Message as BaseMessage
 from nonebot.adapters import MessageSegment as BaseMessageSegment
 
 from .model import Member
 
 
@@ -139,20 +139,33 @@
                 "picture_url": picture_url,
                 "music_url": music_url,
                 "brief": brief,
             },
         )
 
     @staticmethod
-    def node(uid: int, time: datetime, name: str, message: "Message") -> "Node":
-        """合并转发消息段中的节点"""
-        return Node("node", {"uid": uid, "time": int(time.timestamp()), "name": name, "message": message})
+    def custom_node(uid: int, time: datetime, name: str, message: "Message") -> "CustomNode":
+        """合并转发消息段中的自定义节点"""
+        return CustomNode(uid, int(time.timestamp()), name, message)
 
     @staticmethod
-    def forward(nodes: list["Node"], display_strategy: Optional["DisplayStrategy"] = None) -> "Forward":
+    def id_node(id: int) -> "IdNode":
+        """合并转发消息段中的当前对话上下文消息引用节点"""
+        return IdNode(id)
+
+    @staticmethod
+    def ref_node(id: int, target: Optional[int] = None) -> "RefNode":
+        """合并转发消息段中的其他对话上下文消息引用节点"""
+        return RefNode({"id": id, "target": target})
+
+    @staticmethod
+    def forward(
+        nodes: list[Union["CustomNode", "IdNode", "RefNode"]],
+        display_strategy: Optional["DisplayStrategy"] = None,
+    ) -> "Forward":
         """合并转发消息段"""
         return Forward("forward", {"nodes": nodes, "display_strategy": display_strategy})
 
     @staticmethod
     def image(
         id: Optional[str] = None,
         url: Optional[str] = None,
@@ -497,52 +510,66 @@
     }
 
     @override
     def __str__(self):
         return "[音乐分享]"
 
 
-class NodeData(TypedDict):
+@dataclass
+class CustomNode:
     uid: int
     time: int
     name: str
     message: "Message"
 
+    @classmethod
+    def parse(cls, raw: dict):
+        return cls(
+            uid=raw["senderId"],
+            time=raw["time"],
+            name=raw["senderName"],
+            message=Message.from_elements(raw["messageChain"]),
+        )
+
+    def dump(self) -> dict:
+        return {
+            "senderId": self.uid,
+            "time": self.time,
+            "senderName": self.name,
+            "messageChain": self.message.to_elements(),
+        }
+
 
 @dataclass
-class Node(MessageSegment, element_type=("ForwardNode", "node")):
-    data: NodeData = field(default_factory=dict)  # type: ignore
-    __mapping__ = {
-        "uid": "senderId",
-        "time": "time",
-        "name": "senderName",
-        "message": "messageChain",
-    }
+class IdNode:
+    id: int
+
+    @classmethod
+    def parse(cls, raw: dict):
+        return cls(id=raw["messageId"])
+
+    def dump(self) -> dict:
+        return {"messageId": self.id}
+
+
+class RefData(TypedDict):
+    id: int
+    target: Optional[int]
 
-    def __post_init__(self):
-        if not isinstance(self.data["message"], Message):
-            self.data["message"] = Message.from_elements(self.data["message"])  # type: ignore
+
+@dataclass
+class RefNode:
+    ref: RefData
 
     @classmethod
     def parse(cls, raw: dict):
-        return Node(
-            "node",
-            {
-                "uid": raw["senderId"],
-                "time": raw["time"],
-                "name": raw["senderName"],
-                "message": Message.from_elements(raw["messageChain"]),
-            },
-        )
+        return cls(ref={"id": raw["messageId"], "target": raw.get("target")})
 
     def dump(self) -> dict:
-        return {
-            **{self.__mapping__.get(k, k): v for k, v in self.data.items()},
-            "messageChain": self.data["message"].to_elements(),
-        }
+        return {"messageRef": {"messageId": self.ref["id"], "target": self.ref.get("target")}}
 
 
 class DisplayStrategy(TypedDict):
     title: Optional[str]
     """卡片顶部标题"""
     brief: Optional[str]
     """消息列表预览"""
@@ -551,27 +578,33 @@
     preview: Optional[list[str]]
     """卡片消息预览 (只显示前 4 条)"""
     summary: Optional[str]
     """卡片底部摘要"""
 
 
 class ForwardData(TypedDict):
-    nodes: list[Node]
+    nodes: list[Union[CustomNode, IdNode, RefNode]]
     display_strategy: Optional[DisplayStrategy]
 
 
 @dataclass
 class Forward(MessageSegment, element_type=("Forward", "forward")):
     data: ForwardData = field(default_factory=dict)  # type: ignore
 
     __mapping__ = {"nodes": "nodeList", "display_strategy": "display"}
 
     def __post_init__(self):
-        if "nodes" in self.data and not isinstance(self.data["nodes"][0], Node):
-            self.data["nodes"] = [Node.parse(n) for n in self.data["nodes"]]  # type: ignore
+        if "nodes" in self.data and not isinstance(self.data["nodes"][0], (CustomNode, IdNode, RefNode)):
+            for index, raw in enumerate(cast(list[dict], self.data["nodes"])):
+                if "messageId" in raw:
+                    self.data["nodes"][index] = IdNode.parse(raw)
+                elif "messageRef" in raw:
+                    self.data["nodes"][index] = RefNode.parse(raw)
+                else:
+                    self.data["nodes"][index] = CustomNode.parse(raw)
 
     def dump(self) -> dict:
         return {
             **{self.__mapping__.get(k, k): v for k, v in self.data.items()},
             "nodeList": [n.dump() for n in self.data["nodes"]],
         }
```

### Comparing `nonebot_adapter_mirai-2.3.0/nonebot/adapters/mirai/model/__init__.py` & `nonebot_adapter_mirai-2.3.1/nonebot/adapters/mirai/model/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_mirai-2.3.0/nonebot/adapters/mirai/model/base.py` & `nonebot_adapter_mirai-2.3.1/nonebot/adapters/mirai/model/base.py`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_mirai-2.3.0/nonebot/adapters/mirai/model/common.py` & `nonebot_adapter_mirai-2.3.1/nonebot/adapters/mirai/model/common.py`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_mirai-2.3.0/nonebot/adapters/mirai/model/relationship.py` & `nonebot_adapter_mirai-2.3.1/nonebot/adapters/mirai/model/relationship.py`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_mirai-2.3.0/nonebot/adapters/mirai/utils.py` & `nonebot_adapter_mirai-2.3.1/nonebot/adapters/mirai/utils.py`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_mirai-2.3.0/pyproject.toml` & `nonebot_adapter_mirai-2.3.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = [
     "pdm-backend",
 ]
 build-backend = "pdm.backend"
 
 [project]
 name = "nonebot-adapter-mirai"
-version = "2.3.0"
+version = "2.3.1"
 description = "Mirai Api HTTP adapter for nonebot2"
 authors = [
     { name = "rf_tar_railt", email = "rf_tar_railt@qq.com" },
     { name = "Mix", email = "admin@yami.im" },
     { name = "yanyongyu", email = "yyy@nonebot.dev" },
 ]
 dependencies = [
```

### Comparing `nonebot_adapter_mirai-2.3.0/PKG-INFO` & `nonebot_adapter_mirai-2.3.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-adapter-mirai
-Version: 2.3.0
+Version: 2.3.1
 Summary: Mirai Api HTTP adapter for nonebot2
 Keywords: bot,qq,qqbot,mirai
 Home-page: https://nonebot.dev/
 Author-Email: rf_tar_railt <rf_tar_railt@qq.com>, Mix <admin@yami.im>, yanyongyu <yyy@nonebot.dev>
 License: AGPL-3.0-or-later
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: Robot Framework
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-adapter-mirai Version: 2.3.0 Summary: Mirai
+Metadata-Version: 2.1 Name: nonebot-adapter-mirai Version: 2.3.1 Summary: Mirai
 Api HTTP adapter for nonebot2 Keywords: bot,qq,qqbot,mirai Home-page: https://
 nonebot.dev/ Author-Email: rf_tar_railt
 qq.com>, Mix
 yami.im>, yanyongyu
 nonebot.dev> License: AGPL-3.0-or-later Classifier: Development Status :: 5 -
 Production/Stable Classifier: Framework :: Robot Framework Classifier:
 Framework :: Robot Framework :: Library Classifier: Operating System :: OS
```

