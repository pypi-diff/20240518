# Comparing `tmp/nonebot_plugin_calc24-0.2.2.tar.gz` & `tmp/nonebot_plugin_calc24-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_calc24-0.2.2.tar", max compression
+gzip compressed data, was "nonebot_plugin_calc24-0.2.3.tar", max compression
```

## Comparing `nonebot_plugin_calc24-0.2.2.tar` & `nonebot_plugin_calc24-0.2.3.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1097 2024-05-17 01:11:38.482498 nonebot_plugin_calc24-0.2.2/LICENSE
--rw-r--r--   0        0        0     3822 2024-05-17 05:53:10.025890 nonebot_plugin_calc24-0.2.2/nonebot_plugin_calc24/__init__.py
--rw-r--r--   0        0        0     5303 2024-05-17 01:11:38.483619 nonebot_plugin_calc24-0.2.2/nonebot_plugin_calc24/calc24_invalid_data.json
--rw-r--r--   0        0        0     1866 2024-05-17 05:53:24.529102 nonebot_plugin_calc24-0.2.2/nonebot_plugin_calc24/xj_calc24.py
--rw-r--r--   0        0        0      701 2024-05-17 05:54:38.705697 nonebot_plugin_calc24-0.2.2/pyproject.toml
--rw-r--r--   0        0        0      175 2024-05-17 01:11:38.482498 nonebot_plugin_calc24-0.2.2/README.md
--rw-r--r--   0        0        0     1133 1970-01-01 00:00:00.000000 nonebot_plugin_calc24-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0     1097 2024-05-17 01:11:38.482498 nonebot_plugin_calc24-0.2.3/LICENSE
+-rw-r--r--   0        0        0     3811 2024-05-18 06:23:46.845160 nonebot_plugin_calc24-0.2.3/nonebot_plugin_calc24/__init__.py
+-rw-r--r--   0        0        0     5303 2024-05-17 01:11:38.483619 nonebot_plugin_calc24-0.2.3/nonebot_plugin_calc24/calc24_invalid_data.json
+-rw-r--r--   0        0        0     1866 2024-05-17 05:53:24.529102 nonebot_plugin_calc24-0.2.3/nonebot_plugin_calc24/xj_calc24.py
+-rw-r--r--   0        0        0      701 2024-05-17 06:27:33.366930 nonebot_plugin_calc24-0.2.3/pyproject.toml
+-rw-r--r--   0        0        0      592 2024-05-18 06:23:33.596723 nonebot_plugin_calc24-0.2.3/README.md
+-rw-r--r--   0        0        0     1538 1970-01-01 00:00:00.000000 nonebot_plugin_calc24-0.2.3/PKG-INFO
```

### Comparing `nonebot_plugin_calc24-0.2.2/LICENSE` & `nonebot_plugin_calc24-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_calc24-0.2.2/nonebot_plugin_calc24/__init__.py` & `nonebot_plugin_calc24-0.2.3/nonebot_plugin_calc24/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import asyncio
 from nonebot import on_command, on_message
 from nonebot.rule import to_me
 from nonebot.params import CommandArg
-from nonebot.adapters.onebot.v11 import Bot, Event
+from nonebot.adapters import Bot, Event
 from nonebot.typing import T_State 
 from nonebot.plugin import PluginMetadata
 from .xj_calc24 import xj_calc24
 class_calc24 = xj_calc24()
 __plugin_meta__ = PluginMetadata(
     name="nonebot-plugin-calc24",
     description="该插件实现的小游戏的游戏规则为一人一题。在插件启动时使用[/24点]命令启动游戏。使用加减乘除使给出的数等于24，在游戏进行时可以直接回复[退出]来退出游戏或者[换一题]来更换新的题目。如果在5分钟内未回答会自动退出。",
```

### Comparing `nonebot_plugin_calc24-0.2.2/nonebot_plugin_calc24/calc24_invalid_data.json` & `nonebot_plugin_calc24-0.2.3/nonebot_plugin_calc24/calc24_invalid_data.json`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_calc24-0.2.2/nonebot_plugin_calc24/xj_calc24.py` & `nonebot_plugin_calc24-0.2.3/nonebot_plugin_calc24/xj_calc24.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_calc24-0.2.2/pyproject.toml` & `nonebot_plugin_calc24-0.2.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nonebot-plugin-calc24"
-version = "0.2.2"
+version = "0.2.3"
 description = "A 24-point game plugin implemented using NoneBot."
 authors = ["AwAjie <139576615+ajdgg@users.noreply.github.com>"]
 license = "LICENSE"
 readme = "README.md"
 homepage = "https://github.com/ajdgg/nonebot-plugin-calc24"
 repository = "https://github.com/ajdgg/nonebot-plugin-calc24"
 documentation = "https://github.com/ajdgg/nonebot-plugin-calc24"
```

