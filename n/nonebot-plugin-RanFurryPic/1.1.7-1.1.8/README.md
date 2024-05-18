# Comparing `tmp/nonebot_plugin_ranfurrypic-1.1.7.tar.gz` & `tmp/nonebot_plugin_ranfurrypic-1.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_ranfurrypic-1.1.7.tar", last modified: Sun May 12 07:21:31 2024, max compression
+gzip compressed data, was "nonebot_plugin_ranfurrypic-1.1.8.tar", last modified: Sat May 18 12:49:25 2024, max compression
```

## Comparing `nonebot_plugin_ranfurrypic-1.1.7.tar` & `nonebot_plugin_ranfurrypic-1.1.8.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-05-12 07:21:31.656916 nonebot_plugin_ranfurrypic-1.1.7/
--rw-rw-rw-   0        0        0     1082 2024-05-12 06:57:22.000000 nonebot_plugin_ranfurrypic-1.1.7/LICENSE
--rw-rw-rw-   0        0        0     3030 2024-05-12 07:21:31.651485 nonebot_plugin_ranfurrypic-1.1.7/PKG-INFO
--rw-rw-rw-   0        0        0     2663 2024-05-12 07:18:47.000000 nonebot_plugin_ranfurrypic-1.1.7/README.md
-drwxrwxrwx   0        0        0        0 2024-05-12 07:21:31.628437 nonebot_plugin_ranfurrypic-1.1.7/nonebot_plugin_RanFurryPic/
--rw-rw-rw-   0        0        0     3131 2024-05-12 06:57:22.000000 nonebot_plugin_ranfurrypic-1.1.7/nonebot_plugin_RanFurryPic/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-12 07:21:31.648983 nonebot_plugin_ranfurrypic-1.1.7/nonebot_plugin_RanFurryPic.egg-info/
--rw-rw-rw-   0        0        0     3030 2024-05-12 07:21:31.000000 nonebot_plugin_ranfurrypic-1.1.7/nonebot_plugin_RanFurryPic.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      320 2024-05-12 07:21:31.000000 nonebot_plugin_ranfurrypic-1.1.7/nonebot_plugin_RanFurryPic.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-12 07:21:31.000000 nonebot_plugin_ranfurrypic-1.1.7/nonebot_plugin_RanFurryPic.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       38 2024-05-12 07:21:31.000000 nonebot_plugin_ranfurrypic-1.1.7/nonebot_plugin_RanFurryPic.egg-info/requires.txt
--rw-rw-rw-   0        0        0       27 2024-05-12 07:21:31.000000 nonebot_plugin_ranfurrypic-1.1.7/nonebot_plugin_RanFurryPic.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      380 2024-05-12 07:18:54.000000 nonebot_plugin_ranfurrypic-1.1.7/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-12 07:21:31.656916 nonebot_plugin_ranfurrypic-1.1.7/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-18 12:49:25.760083 nonebot_plugin_ranfurrypic-1.1.8/
+-rw-rw-rw-   0        0        0     1082 2024-05-18 12:47:00.000000 nonebot_plugin_ranfurrypic-1.1.8/LICENSE
+-rw-rw-rw-   0        0        0     3045 2024-05-18 12:49:25.755378 nonebot_plugin_ranfurrypic-1.1.8/PKG-INFO
+-rw-rw-rw-   0        0        0     2663 2024-05-18 12:47:00.000000 nonebot_plugin_ranfurrypic-1.1.8/README.md
+drwxrwxrwx   0        0        0        0 2024-05-18 12:49:25.734372 nonebot_plugin_ranfurrypic-1.1.8/nonebot_plugin_RanFurryPic/
+-rw-rw-rw-   0        0        0     3039 2024-05-18 12:47:00.000000 nonebot_plugin_ranfurrypic-1.1.8/nonebot_plugin_RanFurryPic/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-18 12:49:25.752872 nonebot_plugin_ranfurrypic-1.1.8/nonebot_plugin_RanFurryPic.egg-info/
+-rw-rw-rw-   0        0        0     3045 2024-05-18 12:49:25.000000 nonebot_plugin_ranfurrypic-1.1.8/nonebot_plugin_RanFurryPic.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      320 2024-05-18 12:49:25.000000 nonebot_plugin_ranfurrypic-1.1.8/nonebot_plugin_RanFurryPic.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-18 12:49:25.000000 nonebot_plugin_ranfurrypic-1.1.8/nonebot_plugin_RanFurryPic.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       53 2024-05-18 12:49:25.000000 nonebot_plugin_ranfurrypic-1.1.8/nonebot_plugin_RanFurryPic.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       27 2024-05-18 12:49:25.000000 nonebot_plugin_ranfurrypic-1.1.8/nonebot_plugin_RanFurryPic.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      395 2024-05-18 12:47:00.000000 nonebot_plugin_ranfurrypic-1.1.8/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-18 12:49:25.760083 nonebot_plugin_ranfurrypic-1.1.8/setup.cfg
```

### Comparing `nonebot_plugin_ranfurrypic-1.1.7/LICENSE` & `nonebot_plugin_ranfurrypic-1.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_ranfurrypic-1.1.7/PKG-INFO` & `nonebot_plugin_ranfurrypic-1.1.8/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: nonebot_plugin_RanFurryPic
-Version: 1.1.7
+Version: 1.1.8
 Summary: 基于NoneBot2进行适配的兽云随机毛图插件
 Author-email: Ekac <2396382559@qq.com>
 License: MIT
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: nonebot2
 Requires-Dist: httpx
-Requires-Dist: nonebot-adapter-onebot
+Requires-Dist: nonebot-plugin-send-anything-anywhere
 
 <div align="center">
   <a href="https://v2.nonebot.dev/store"><img src="https://github.com/A-kirami/nonebot-plugin-template/blob/resources/nbp_logo.png" width="180" height="180" alt="NoneBotPluginLogo"></a>
   <br>
   <p><img src="https://github.com/A-kirami/nonebot-plugin-template/blob/resources/NoneBotPlugin.svg" width="240" alt="NoneBotPluginText"></p>
 </div>
```

#### html2text {}

```diff
@@ -1,12 +1,12 @@
-Metadata-Version: 2.1 Name: nonebot_plugin_RanFurryPic Version: 1.1.7 Summary:
+Metadata-Version: 2.1 Name: nonebot_plugin_RanFurryPic Version: 1.1.8 Summary:
 åºäºNoneBot2è¿è¡ééçå½äºéæºæ¯å¾æä»¶ Author-email: Ekac
 <2396382559@qq.com> License: MIT Requires-Python: >=3.9 Description-Content-
 Type: text/markdown License-File: LICENSE Requires-Dist: nonebot2 Requires-
-Dist: httpx Requires-Dist: nonebot-adapter-onebot
+Dist: httpx Requires-Dist: nonebot-plugin-send-anything-anywhere
                               _[_N_o_n_e_B_o_t_P_l_u_g_i_n_L_o_g_o_]
                               [NoneBotPluginText]
               # nonebot-plugin-RanFurryPic _â¨ éæºæ¯å¾ â¨_
 _[_l_i_c_e_n_s_e_]_[_p_y_p_i_][python]
 åºäºNoneBot2è¿è¡ééçå½äºéæºæ¯å¾æä»¶ ## ð ä»ç»
 å½äºå®æ¹æä»¶å¤ªå¤æï¼åè½å¤ªæï¼çä¸æï¼ä¸å¼å®¹ï¼æåæä»¶ç»æï¼
 æ¬æä»¶ä½¿ç¨å®æ¹_A_P_Iè¿è¡ç¼åï¼æ éä»¤çï¼æ éTokenï¼å³å¯ä½¿ç¨éæºæ¯å¾åè½
```

### Comparing `nonebot_plugin_ranfurrypic-1.1.7/README.md` & `nonebot_plugin_ranfurrypic-1.1.8/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_ranfurrypic-1.1.7/nonebot_plugin_RanFurryPic/__init__.py` & `nonebot_plugin_ranfurrypic-1.1.8/nonebot_plugin_RanFurryPic/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,29 +1,28 @@
-from nonebot.plugin import on_command
+from nonebot import on_command
 from nonebot import logger
-from nonebot.adapters.onebot.v11 import MessageSegment
 import httpx
-from nonebot.plugin import PluginMetadata
-from nonebot.adapters import Message
+from nonebot.plugin import PluginMetadata, inherit_supported_adapters
 from nonebot.params import CommandArg
+from nonebot import require
+require("nonebot_plugin_saa")
+from nonebot_plugin_saa import Text, Image, MessageFactory
+
 
 __plugin_meta__ = PluginMetadata(
     name="随机毛图",
     description="基于NoneBot2进行适配的兽云随机毛图插件",
     usage="预设指令有furry、来只毛、毛毛三种指令，发送后将会调用兽云的随即图片API并返回图片及基本介绍",
 
     type="application",
-    # 发布必填，当前有效类型有：`library`（为其他插件编写提供功能），`application`（向机器人用户提供功能）。
 
     homepage="https://github.com/Ekac00/nonebot-plugin-RanFurryPic/",
     # 发布必填。
 
-    supported_adapters={"~onebot.v11"},
-    # 支持的适配器集合，其中 `~` 在此处代表前缀 `nonebot.adapters.`，其余适配器亦按此格式填写。
-    # 若插件可以保证兼容所有适配器（即仅使用基本适配器功能）可不填写，否则应该列出插件支持的适配器。
+    supported_adapters=inherit_supported_adapters("nonebot_plugin_session")
 )
 
 furry = on_command("来只毛", aliases={"毛毛", "furry"}, priority=9, block=True)
 
 async def handle_get_pic():
     headers = {
         'User-Agent': 'Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/58.0.3029.110 Safari/537.3'
@@ -53,13 +52,18 @@
         else:
             logger.error(f"请求失败！\n状态码：{pic_response.status_code}")
             return f"请求失败！\n状态码：{pic_response.status_code}"
 
     # 发送图片
     name = pic_json["picture"]["name"]
     suggest = pic_json["picture"]["suggest"]
-    return MessageSegment.image(pic_id_url) + f"好的嗷呜～\n毛毛名称：{name}\n留言：{suggest}\n图片UID:{pic_id}"
+    #return MessageSegment.image(pic_id_url) + f"好的嗷呜～\n毛毛名称：{name}\n留言：{suggest}\n图片UID:{pic_id}"
+
+    #返回参数
+    return pic_id_url, name, suggest, pic_id
 
 @furry.handle()
 async def handle_furry():
-    result = await handle_get_pic()
-    await furry.finish(result)
+    pic_id_url, name, suggest, pic_id = await handle_get_pic()
+    text = f'好的嗷呜～\n毛毛名称：{name}\n留言：{suggest}\n图片UID:{pic_id}'
+    #使用saa构建消息
+    await MessageFactory([Image(pic_id_url), Text(text)]).send()
```

### Comparing `nonebot_plugin_ranfurrypic-1.1.7/nonebot_plugin_RanFurryPic.egg-info/PKG-INFO` & `nonebot_plugin_ranfurrypic-1.1.8/nonebot_plugin_RanFurryPic.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: nonebot_plugin_RanFurryPic
-Version: 1.1.7
+Version: 1.1.8
 Summary: 基于NoneBot2进行适配的兽云随机毛图插件
 Author-email: Ekac <2396382559@qq.com>
 License: MIT
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: nonebot2
 Requires-Dist: httpx
-Requires-Dist: nonebot-adapter-onebot
+Requires-Dist: nonebot-plugin-send-anything-anywhere
 
 <div align="center">
   <a href="https://v2.nonebot.dev/store"><img src="https://github.com/A-kirami/nonebot-plugin-template/blob/resources/nbp_logo.png" width="180" height="180" alt="NoneBotPluginLogo"></a>
   <br>
   <p><img src="https://github.com/A-kirami/nonebot-plugin-template/blob/resources/NoneBotPlugin.svg" width="240" alt="NoneBotPluginText"></p>
 </div>
```

#### html2text {}

```diff
@@ -1,12 +1,12 @@
-Metadata-Version: 2.1 Name: nonebot_plugin_RanFurryPic Version: 1.1.7 Summary:
+Metadata-Version: 2.1 Name: nonebot_plugin_RanFurryPic Version: 1.1.8 Summary:
 åºäºNoneBot2è¿è¡ééçå½äºéæºæ¯å¾æä»¶ Author-email: Ekac
 <2396382559@qq.com> License: MIT Requires-Python: >=3.9 Description-Content-
 Type: text/markdown License-File: LICENSE Requires-Dist: nonebot2 Requires-
-Dist: httpx Requires-Dist: nonebot-adapter-onebot
+Dist: httpx Requires-Dist: nonebot-plugin-send-anything-anywhere
                               _[_N_o_n_e_B_o_t_P_l_u_g_i_n_L_o_g_o_]
                               [NoneBotPluginText]
               # nonebot-plugin-RanFurryPic _â¨ éæºæ¯å¾ â¨_
 _[_l_i_c_e_n_s_e_]_[_p_y_p_i_][python]
 åºäºNoneBot2è¿è¡ééçå½äºéæºæ¯å¾æä»¶ ## ð ä»ç»
 å½äºå®æ¹æä»¶å¤ªå¤æï¼åè½å¤ªæï¼çä¸æï¼ä¸å¼å®¹ï¼æåæä»¶ç»æï¼
 æ¬æä»¶ä½¿ç¨å®æ¹_A_P_Iè¿è¡ç¼åï¼æ éä»¤çï¼æ éTokenï¼å³å¯ä½¿ç¨éæºæ¯å¾åè½
```

