# Comparing `tmp/nonebot_plugin_tsugu_bangdream_bot-0.1.3.tar.gz` & `tmp/nonebot_plugin_tsugu_bangdream_bot-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_tsugu_bangdream_bot-0.1.3.tar", last modified: Fri May 17 12:03:24 2024, max compression
+gzip compressed data, was "nonebot_plugin_tsugu_bangdream_bot-0.1.4.tar", last modified: Fri May 17 16:47:25 2024, max compression
```

## Comparing `nonebot_plugin_tsugu_bangdream_bot-0.1.3.tar` & `nonebot_plugin_tsugu_bangdream_bot-0.1.4.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1067 2024-05-17 12:03:01.749841 nonebot_plugin_tsugu_bangdream_bot-0.1.3/LICENSE
--rw-r--r--   0        0        0     6710 2024-05-17 12:03:01.749841 nonebot_plugin_tsugu_bangdream_bot-0.1.3/README.md
--rw-r--r--   0        0        0    36185 2024-05-17 12:03:01.749841 nonebot_plugin_tsugu_bangdream_bot-0.1.3/nonebot_plugin_tsugu_bangdream_bot/__init__.py
--rw-r--r--   0        0        0    13194 2024-05-17 12:03:01.749841 nonebot_plugin_tsugu_bangdream_bot-0.1.3/nonebot_plugin_tsugu_bangdream_bot/_commands.py
--rw-r--r--   0        0        0     7847 2024-05-17 12:03:01.749841 nonebot_plugin_tsugu_bangdream_bot-0.1.3/nonebot_plugin_tsugu_bangdream_bot/_utils.py
--rw-r--r--   0        0        0     1586 2024-05-17 12:03:01.749841 nonebot_plugin_tsugu_bangdream_bot-0.1.3/nonebot_plugin_tsugu_bangdream_bot/config.py
--rw-r--r--   0        0        0      569 2024-05-17 12:03:24.965947 nonebot_plugin_tsugu_bangdream_bot-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     7150 1970-01-01 00:00:00.000000 nonebot_plugin_tsugu_bangdream_bot-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1067 2024-05-17 16:47:02.686586 nonebot_plugin_tsugu_bangdream_bot-0.1.4/LICENSE
+-rw-r--r--   0        0        0     6710 2024-05-17 16:47:02.686586 nonebot_plugin_tsugu_bangdream_bot-0.1.4/README.md
+-rw-r--r--   0        0        0    36184 2024-05-17 16:47:02.686586 nonebot_plugin_tsugu_bangdream_bot-0.1.4/nonebot_plugin_tsugu_bangdream_bot/__init__.py
+-rw-r--r--   0        0        0    13193 2024-05-17 16:47:02.686586 nonebot_plugin_tsugu_bangdream_bot-0.1.4/nonebot_plugin_tsugu_bangdream_bot/_commands.py
+-rw-r--r--   0        0        0     7846 2024-05-17 16:47:02.686586 nonebot_plugin_tsugu_bangdream_bot-0.1.4/nonebot_plugin_tsugu_bangdream_bot/_utils.py
+-rw-r--r--   0        0        0     1586 2024-05-17 16:47:02.686586 nonebot_plugin_tsugu_bangdream_bot-0.1.4/nonebot_plugin_tsugu_bangdream_bot/config.py
+-rw-r--r--   0        0        0      569 2024-05-17 16:47:25.386906 nonebot_plugin_tsugu_bangdream_bot-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     7150 1970-01-01 00:00:00.000000 nonebot_plugin_tsugu_bangdream_bot-0.1.4/PKG-INFO
```

### Comparing `nonebot_plugin_tsugu_bangdream_bot-0.1.3/LICENSE` & `nonebot_plugin_tsugu_bangdream_bot-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_tsugu_bangdream_bot-0.1.3/README.md` & `nonebot_plugin_tsugu_bangdream_bot-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_tsugu_bangdream_bot-0.1.3/nonebot_plugin_tsugu_bangdream_bot/__init__.py` & `nonebot_plugin_tsugu_bangdream_bot-0.1.4/nonebot_plugin_tsugu_bangdream_bot/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -42,15 +42,15 @@
     search_character,
     switch_main_server,
     set_default_servers,
     get_card_illustration
 )
 
 import tsugu_api_async
-from tsugu_api_async._typing import _ServerId
+from tsugu_api_core._typing import _ServerId
 
 class NoSpaceExtension(Extension):
     @property
     def priority(self) -> int:
         return 10
     
     @property
```

### Comparing `nonebot_plugin_tsugu_bangdream_bot-0.1.3/nonebot_plugin_tsugu_bangdream_bot/_commands.py` & `nonebot_plugin_tsugu_bangdream_bot-0.1.4/nonebot_plugin_tsugu_bangdream_bot/_commands.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from base64 import b64decode
 from typing import List, Tuple, Union, Optional, Sequence
 
 import tsugu_api_async
-from tsugu_api_async._typing import _Server, _ServerId, _DifficultyText
+from tsugu_api_core._typing import _Server, _ServerId, _DifficultyText
 
 from ._utils import server_id_to_full_name
 
 async def switch_forward(user_id: str, mode: bool) -> str:
     try:
         response = await tsugu_api_async.change_user_data(
             "red",
```

### Comparing `nonebot_plugin_tsugu_bangdream_bot-0.1.3/nonebot_plugin_tsugu_bangdream_bot/_utils.py` & `nonebot_plugin_tsugu_bangdream_bot-0.1.4/nonebot_plugin_tsugu_bangdream_bot/_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from tsugu_api_async._typing import _ServerId, _ServerName
+from tsugu_api_core._typing import _ServerId, _ServerName
 
 _COMMAND_KEYWORDS = [
     '查询玩家',
     '查卡面',
     '查玩家',
     '查卡',
     '查角色',
```

### Comparing `nonebot_plugin_tsugu_bangdream_bot-0.1.3/nonebot_plugin_tsugu_bangdream_bot/config.py` & `nonebot_plugin_tsugu_bangdream_bot-0.1.4/nonebot_plugin_tsugu_bangdream_bot/config.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_tsugu_bangdream_bot-0.1.3/pyproject.toml` & `nonebot_plugin_tsugu_bangdream_bot-0.1.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 [project]
 name = "nonebot-plugin-tsugu-bangdream-bot"
-version = "0.1.3"
+version = "0.1.4"
 description = "Koishi-Plugin-Tsugu-BanGDream-Bot 的 NoneBot2 实现"
 authors = [
     { name = "WindowsSov8forUs", email = "qwertyuiop2333@hotmail.com" },
 ]
 dependencies = [
     "nonebot2>=2.2.1",
     "nonebot-plugin-alconna>=0.42.4",
-    "tsugu-api-python>=1.1.7",
+    "tsugu-api-python>=1.2.0",
     "nonebot-plugin-userinfo>=0.2.4",
 ]
 requires-python = ">=3.8"
 readme = "README.md"
 
 [project.license]
 text = "MIT"
```

### Comparing `nonebot_plugin_tsugu_bangdream_bot-0.1.3/PKG-INFO` & `nonebot_plugin_tsugu_bangdream_bot-0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-tsugu-bangdream-bot
-Version: 0.1.3
+Version: 0.1.4
 Summary: Koishi-Plugin-Tsugu-BanGDream-Bot 的 NoneBot2 实现
 Author-Email: WindowsSov8forUs <qwertyuiop2333@hotmail.com>
 License: MIT
 Requires-Python: >=3.8
 Requires-Dist: nonebot2>=2.2.1
 Requires-Dist: nonebot-plugin-alconna>=0.42.4
-Requires-Dist: tsugu-api-python>=1.1.7
+Requires-Dist: tsugu-api-python>=1.2.0
 Requires-Dist: nonebot-plugin-userinfo>=0.2.4
 Description-Content-Type: text/markdown
 
 <div align="center">
   <a href="https://v2.nonebot.dev/store"><img src="https://github.com/A-kirami/nonebot-plugin-template/blob/resources/nbp_logo.png" width="180" height="180" alt="NoneBotPluginLogo"></a>
   <br>
   <p><img src="https://github.com/A-kirami/nonebot-plugin-template/blob/resources/NoneBotPlugin.svg" width="240" alt="NoneBotPluginText"></p>
```

#### html2text {}

```diff
@@ -1,13 +1,13 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-tsugu-bangdream-bot Version: 0.1.3
+Metadata-Version: 2.1 Name: nonebot-plugin-tsugu-bangdream-bot Version: 0.1.4
 Summary: Koishi-Plugin-Tsugu-BanGDream-Bot ç NoneBot2 å®ç° Author-Email:
 WindowsSov8forUs
 hotmail.com> License: MIT Requires-Python: >=3.8 Requires-Dist: nonebot2>=2.2.1
 Requires-Dist: nonebot-plugin-alconna>=0.42.4 Requires-Dist: tsugu-api-
-python>=1.1.7 Requires-Dist: nonebot-plugin-userinfo>=0.2.4 Description-
+python>=1.2.0 Requires-Dist: nonebot-plugin-userinfo>=0.2.4 Description-
 Content-Type: text/markdown
                               _[_N_o_n_e_B_o_t_P_l_u_g_i_n_L_o_g_o_]
                               [NoneBotPluginText]
  # NoneBot-Plugin-Tsugu-BanGDream-Bot _â¨ [Koishi-Plugin-Tsugu-BanGDream-Bot]
  (https://github.com/Yamamoto-2/tsugu-bangdream-bot) ç NoneBot2 å®ç° â¨_
                        _[_l_i_c_e_n_s_e_]_[_l_i_c_e_n_s_e_]_[_p_y_p_i_][python]
 [koishi-plugin-tsugu-bangdream-bot](https://github.com/Yamamoto-2/tsugu-
```

