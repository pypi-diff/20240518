# Comparing `tmp/nonebot_plugin_nai3_bot-0.0.1.tar.gz` & `tmp/nonebot_plugin_nai3_bot-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_nai3_bot-0.0.1.tar", max compression
+gzip compressed data, was "nonebot_plugin_nai3_bot-0.0.2.tar", max compression
```

## Comparing `nonebot_plugin_nai3_bot-0.0.1.tar` & `nonebot_plugin_nai3_bot-0.0.2.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     2556 2024-05-18 17:55:30.949231 nonebot_plugin_nai3_bot-0.0.1/README.md
--rw-r--r--   0        0        0     6148 2023-06-10 13:04:05.827943 nonebot_plugin_nai3_bot-0.0.1/nonebot_plugin_nai3_bot/.DS_Store
--rw-r--r--   0        0        0    11728 2024-05-18 17:54:56.091036 nonebot_plugin_nai3_bot-0.0.1/nonebot_plugin_nai3_bot/__init__.py
--rw-r--r--   0        0        0      624 2024-05-18 17:43:00.932701 nonebot_plugin_nai3_bot-0.0.1/nonebot_plugin_nai3_bot/config.py
--rw-r--r--   0        0        0      621 2024-05-18 17:25:19.038827 nonebot_plugin_nai3_bot-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     3429 1970-01-01 00:00:00.000000 nonebot_plugin_nai3_bot-0.0.1/setup.py
--rw-r--r--   0        0        0     3330 1970-01-01 00:00:00.000000 nonebot_plugin_nai3_bot-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     2716 2024-05-18 18:12:40.986423 nonebot_plugin_nai3_bot-0.0.2/README.md
+-rw-r--r--   0        0        0     6148 2024-05-18 18:12:40.996971 nonebot_plugin_nai3_bot-0.0.2/nonebot_plugin_nai3_bot/.DS_Store
+-rw-r--r--   0        0        0    11728 2024-05-18 18:12:40.997303 nonebot_plugin_nai3_bot-0.0.2/nonebot_plugin_nai3_bot/__init__.py
+-rw-r--r--   0        0        0      624 2024-05-18 18:12:40.997504 nonebot_plugin_nai3_bot-0.0.2/nonebot_plugin_nai3_bot/config.py
+-rw-r--r--   0        0        0      639 2024-05-18 18:13:46.377339 nonebot_plugin_nai3_bot-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     3617 1970-01-01 00:00:00.000000 nonebot_plugin_nai3_bot-0.0.2/setup.py
+-rw-r--r--   0        0        0     3530 1970-01-01 00:00:00.000000 nonebot_plugin_nai3_bot-0.0.2/PKG-INFO
```

### Comparing `nonebot_plugin_nai3_bot-0.0.1/README.md` & `nonebot_plugin_nai3_bot-0.0.2/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -53,11 +53,13 @@
 # 使用方法
 - **  聊天内容/绘图需求      （**是触发与Bot对话的关键字）
 - 记忆清除 清除当前用户的聊天记录
 
 # 可能存在的问题
 - 由于调教prompt的原因，机器人可能会偶尔出错，此时继续和TA对话或者是使用记忆清除命令重新开始对话即可。
 - 注意语言大模型的token消耗量
+- 插件目前没有实现绘图排队功能，所以请避免较多用户同时使用绘图功能。
 
 # TODO
 - [ ] 添加用户自定义人格功能
 - [ ] 代理支持
+- [ ] 支持绘图排队(NAI3只支持一次出一张图)
```

#### html2text {}

```diff
@@ -20,9 +20,11 @@
 ï¼å¯éï¼å¤§æ¨¡åä¸­è½¬æå¡åæä¾çä¸­è½¬å°å,ä½¿ç¨OpenAIå®æ¹æå¡ä¸éè¦å¡«å
 oneapi_model = "gpt-4" #
 ï¼å¯éï¼ä½¿ç¨çè¯­è¨å¤§æ¨¡å,å»ºè®®ä½¿ç¨gpt4ægpt4oæ¨¡åä»¥è¾¾å°æ´å¥½çä½éªæææ­¤é¡¹,é»è®¤ä½¿ç¨gpt-
 4æ¨¡å ``` NAI3çtokenè·åå°åæ¹æ³ï¼ ![Alt](image.png) # ä½¿ç¨æ¹æ³
 - ** èå¤©åå®¹/ç»å¾éæ± ï¼**æ¯è§¦åä¸Botå¯¹è¯çå³é®å­ï¼ -
 è®°å¿æ¸é¤ æ¸é¤å½åç¨æ·çèå¤©è®°å½ # å¯è½å­å¨çé®é¢ -
 ç±äºè°æpromptçåå ï¼æºå¨äººå¯è½ä¼å¶å°åºéï¼æ­¤æ¶ç»§ç»­åTAå¯¹è¯æèæ¯ä½¿ç¨è®°å¿æ¸é¤å½ä»¤éæ°å¼å§å¯¹è¯å³å¯ã
-- æ³¨æè¯­è¨å¤§æ¨¡åçtokenæ¶èé # TODO - [ ]
-æ·»å ç¨æ·èªå®ä¹äººæ ¼åè½ - [ ] ä»£çæ¯æ
+- æ³¨æè¯­è¨å¤§æ¨¡åçtokenæ¶èé -
+æä»¶ç®åæ²¡æå®ç°ç»å¾æéåè½ï¼æä»¥è¯·é¿åè¾å¤ç¨æ·åæ¶ä½¿ç¨ç»å¾åè½ã
+# TODO - [ ] æ·»å ç¨æ·èªå®ä¹äººæ ¼åè½ - [ ] ä»£çæ¯æ - [ ]
+æ¯æç»å¾æé(NAI3åªæ¯æä¸æ¬¡åºä¸å¼ å¾)
```

### Comparing `nonebot_plugin_nai3_bot-0.0.1/nonebot_plugin_nai3_bot/.DS_Store` & `nonebot_plugin_nai3_bot-0.0.2/nonebot_plugin_nai3_bot/.DS_Store`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_nai3_bot-0.0.1/nonebot_plugin_nai3_bot/__init__.py` & `nonebot_plugin_nai3_bot-0.0.2/nonebot_plugin_nai3_bot/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_nai3_bot-0.0.1/nonebot_plugin_nai3_bot/config.py` & `nonebot_plugin_nai3_bot-0.0.2/nonebot_plugin_nai3_bot/config.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_nai3_bot-0.0.1/setup.py` & `nonebot_plugin_nai3_bot-0.0.2/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,23 +4,24 @@
 packages = \
 ['nonebot_plugin_nai3_bot']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['nonebot-adapter-onebot>=2.2.1,<3.0.0',
+['Pillow>=9.1.0,<10.0.0',
+ 'nonebot-adapter-onebot>=2.2.1,<3.0.0',
  'nonebot2>=2.0.0rc3,<3.0.0',
  'openai>=1.30.1,<2.0.0']
 
 setup_kwargs = {
     'name': 'nonebot-plugin-nai3-bot',
-    'version': '0.0.1',
+    'version': '0.0.2',
     'description': '基于GPT4+NovelAI V3,Bot在将自然语言转换为NAI3提示词并绘图发送的同时,还会以自定义人格和你聊天',
-    'long_description': '<div align="center">\n  <a href="https://v2.nonebot.dev/store"><img src="https://github.com/A-kirami/nonebot-plugin-template/blob/resources/nbp_logo.png" width="180" height="180" alt="NoneBotPluginLogo"></a>\n  <br>\n  <p><img src="https://github.com/A-kirami/nonebot-plugin-template/blob/resources/NoneBotPlugin.svg" width="240" alt="NoneBotPluginText"></p>\n</div>\n\n<div align="center">\n\n# nonebot-plugin-nai3-bot\n</div>\n\n# 介绍\n- 本插件基于GPT4+NovelAI V3,Bot在将自然语言转换为NAI3提示词并绘图发送的同时以自定义人格与用户聊天。\n- 用户可以正常与指定人格（需要调教prompt,目前插件内置的人格为群友指定的BA角色天童爱丽丝）聊天。在聊天过程中可以使用自然语言描述AI绘图的需求,Bot会根据用户的聊天内容修改AI绘图所用的提示词（见效果图）,并且判断是否需要调用Novel V3模型进行绘画。如果为正常聊天则不会触发绘画功能,如果Bot判断用户有AI绘画的需求,则会调用NAI3绘图,并将图片和提示词发送到群内。\n- 每个用户和Bot有独立的聊天记录。\n\n# 效果\n![Alt](demo1.jpeg)\n\n# 安装\n* 手动安装\n  ```\n  git clone https://github.com/Alpaca4610/nonebot_plugin_nai3_bot.git\n  ```\n\n  下载完成后在bot项目的pyproject.toml文件手动添加插件：\n\n  ```\n  plugin_dirs = ["xxxxxx","xxxxxx",......,"下载完成的插件路径/nonebot-plugin-nai3-bot"]\n  ```\n* 使用 pip\n  ```\n  pip install nonebot-plugin-nai3-bot\n  ```\n# 配置文件\n\n在Bot根目录下的.env文件中追加如下内容：\n\n必填内容：\n```\nnai3_token = "xxxx"  # （必填）NovelAI的token\noneapi_key = "sk-xxxxxxxxxx"  # （必填）OpenAI官方或者是支持OneAPI的大模型中转服务商提供的KEY\n```\n\n可选内容：\n```\noneapi_url = "https://xxxxxxxxx"  # （可选）大模型中转服务商提供的中转地址,使用OpenAI官方服务不需要填写\noneapi_model = "gpt-4" # （可选）使用的语言大模型,建议使用gpt4或gpt4o模型以达到更好的体验效果此项,默认使用gpt-4模型\n```\nNAI3的token获取地址方法：\n![Alt](image.png)\n\n# 使用方法\n- **  聊天内容/绘图需求      （**是触发与Bot对话的关键字）\n- 记忆清除 清除当前用户的聊天记录\n\n# 可能存在的问题\n- 由于调教prompt的原因，机器人可能会偶尔出错，此时继续和TA对话或者是使用记忆清除命令重新开始对话即可。\n- 注意语言大模型的token消耗量\n\n# TODO\n- [ ] 添加用户自定义人格功能\n- [ ] 代理支持\n',
+    'long_description': '<div align="center">\n  <a href="https://v2.nonebot.dev/store"><img src="https://github.com/A-kirami/nonebot-plugin-template/blob/resources/nbp_logo.png" width="180" height="180" alt="NoneBotPluginLogo"></a>\n  <br>\n  <p><img src="https://github.com/A-kirami/nonebot-plugin-template/blob/resources/NoneBotPlugin.svg" width="240" alt="NoneBotPluginText"></p>\n</div>\n\n<div align="center">\n\n# nonebot-plugin-nai3-bot\n</div>\n\n# 介绍\n- 本插件基于GPT4+NovelAI V3,Bot在将自然语言转换为NAI3提示词并绘图发送的同时以自定义人格与用户聊天。\n- 用户可以正常与指定人格（需要调教prompt,目前插件内置的人格为群友指定的BA角色天童爱丽丝）聊天。在聊天过程中可以使用自然语言描述AI绘图的需求,Bot会根据用户的聊天内容修改AI绘图所用的提示词（见效果图）,并且判断是否需要调用Novel V3模型进行绘画。如果为正常聊天则不会触发绘画功能,如果Bot判断用户有AI绘画的需求,则会调用NAI3绘图,并将图片和提示词发送到群内。\n- 每个用户和Bot有独立的聊天记录。\n\n# 效果\n![Alt](demo1.jpeg)\n\n# 安装\n* 手动安装\n  ```\n  git clone https://github.com/Alpaca4610/nonebot_plugin_nai3_bot.git\n  ```\n\n  下载完成后在bot项目的pyproject.toml文件手动添加插件：\n\n  ```\n  plugin_dirs = ["xxxxxx","xxxxxx",......,"下载完成的插件路径/nonebot-plugin-nai3-bot"]\n  ```\n* 使用 pip\n  ```\n  pip install nonebot-plugin-nai3-bot\n  ```\n# 配置文件\n\n在Bot根目录下的.env文件中追加如下内容：\n\n必填内容：\n```\nnai3_token = "xxxx"  # （必填）NovelAI的token\noneapi_key = "sk-xxxxxxxxxx"  # （必填）OpenAI官方或者是支持OneAPI的大模型中转服务商提供的KEY\n```\n\n可选内容：\n```\noneapi_url = "https://xxxxxxxxx"  # （可选）大模型中转服务商提供的中转地址,使用OpenAI官方服务不需要填写\noneapi_model = "gpt-4" # （可选）使用的语言大模型,建议使用gpt4或gpt4o模型以达到更好的体验效果此项,默认使用gpt-4模型\n```\nNAI3的token获取地址方法：\n![Alt](image.png)\n\n# 使用方法\n- **  聊天内容/绘图需求      （**是触发与Bot对话的关键字）\n- 记忆清除 清除当前用户的聊天记录\n\n# 可能存在的问题\n- 由于调教prompt的原因，机器人可能会偶尔出错，此时继续和TA对话或者是使用记忆清除命令重新开始对话即可。\n- 注意语言大模型的token消耗量\n- 插件目前没有实现绘图排队功能，所以请避免较多用户同时使用绘图功能。\n\n# TODO\n- [ ] 添加用户自定义人格功能\n- [ ] 代理支持\n- [ ] 支持绘图排队(NAI3只支持一次出一张图)\n',
     'author': 'Alpaca',
     'author_email': 'alpaca@bupt.edu.cn',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
     'packages': packages,
     'package_data': package_data,
```

#### html2text {}

```diff
@@ -1,12 +1,13 @@
 # -*- coding: utf-8 -*- from setuptools import setup packages = \
 ['nonebot_plugin_nai3_bot'] package_data = \ {'': ['*']} install_requires = \
-['nonebot-adapter-onebot>=2.2.1,<3.0.0', 'nonebot2>=2.0.0rc3,<3.0.0',
-'openai>=1.30.1,<2.0.0'] setup_kwargs = { 'name': 'nonebot-plugin-nai3-bot',
-'version': '0.0.1', 'description': 'åºäºGPT4+NovelAI
+['Pillow>=9.1.0,<10.0.0', 'nonebot-adapter-onebot>=2.2.1,<3.0.0',
+'nonebot2>=2.0.0rc3,<3.0.0', 'openai>=1.30.1,<2.0.0'] setup_kwargs = { 'name':
+'nonebot-plugin-nai3-bot', 'version': '0.0.2', 'description':
+'åºäºGPT4+NovelAI
 V3,Botå¨å°èªç¶è¯­è¨è½¬æ¢ä¸ºNAI3æç¤ºè¯å¹¶ç»å¾åéçåæ¶,è¿ä¼ä»¥èªå®ä¹äººæ ¼åä½ èå¤©',
 'long_description': '
                            \n _[_N_o_n_e_B_o_t_P_l_u_g_i_n_L_o_g_o_]\n
                                       \n
                               [NoneBotPluginText]
                                       \n
 \n\n
@@ -30,13 +31,15 @@
 = "gpt-4" #
 ï¼å¯éï¼ä½¿ç¨çè¯­è¨å¤§æ¨¡å,å»ºè®®ä½¿ç¨gpt4ægpt4oæ¨¡åä»¥è¾¾å°æ´å¥½çä½éªæææ­¤é¡¹,é»è®¤ä½¿ç¨gpt-
 4æ¨¡å\n```\nNAI3çtokenè·åå°åæ¹æ³ï¼\n![Alt](image.png)\n\n#
 ä½¿ç¨æ¹æ³\n- ** èå¤©åå®¹/ç»å¾éæ±
 ï¼**æ¯è§¦åä¸Botå¯¹è¯çå³é®å­ï¼\n- è®°å¿æ¸é¤
 æ¸é¤å½åç¨æ·çèå¤©è®°å½\n\n# å¯è½å­å¨çé®é¢\n-
 ç±äºè°æpromptçåå ï¼æºå¨äººå¯è½ä¼å¶å°åºéï¼æ­¤æ¶ç»§ç»­åTAå¯¹è¯æèæ¯ä½¿ç¨è®°å¿æ¸é¤å½ä»¤éæ°å¼å§å¯¹è¯å³å¯ã\n-
-æ³¨æè¯­è¨å¤§æ¨¡åçtokenæ¶èé\n\n# TODO\n- [ ]
-æ·»å ç¨æ·èªå®ä¹äººæ ¼åè½\n- [ ] ä»£çæ¯æ\n', 'author': 'Alpaca',
+æ³¨æè¯­è¨å¤§æ¨¡åçtokenæ¶èé\n-
+æä»¶ç®åæ²¡æå®ç°ç»å¾æéåè½ï¼æä»¥è¯·é¿åè¾å¤ç¨æ·åæ¶ä½¿ç¨ç»å¾åè½ã\n\n#
+TODO\n- [ ] æ·»å ç¨æ·èªå®ä¹äººæ ¼åè½\n- [ ] ä»£çæ¯æ\n- [ ]
+æ¯æç»å¾æé(NAI3åªæ¯æä¸æ¬¡åºä¸å¼ å¾)\n', 'author': 'Alpaca',
 'author_email': 'alpaca@bupt.edu.cn', 'maintainer': 'None', 'maintainer_email':
 'None', 'url': 'None', 'packages': packages, 'package_data': package_data,
 'install_requires': install_requires, 'python_requires': '>=3.8,<4.0', } setup
 (**setup_kwargs)
```

### Comparing `nonebot_plugin_nai3_bot-0.0.1/PKG-INFO` & `nonebot_plugin_nai3_bot-0.0.2/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-nai3-bot
-Version: 0.0.1
+Version: 0.0.2
 Summary: 基于GPT4+NovelAI V3,Bot在将自然语言转换为NAI3提示词并绘图发送的同时,还会以自定义人格和你聊天
 License: MIT
 Author: Alpaca
 Author-email: alpaca@bupt.edu.cn
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: Pillow (>=9.1.0,<10.0.0)
 Requires-Dist: nonebot-adapter-onebot (>=2.2.1,<3.0.0)
 Requires-Dist: nonebot2 (>=2.0.0rc3,<3.0.0)
 Requires-Dist: openai (>=1.30.1,<2.0.0)
 Description-Content-Type: text/markdown
 
 <div align="center">
   <a href="https://v2.nonebot.dev/store"><img src="https://github.com/A-kirami/nonebot-plugin-template/blob/resources/nbp_logo.png" width="180" height="180" alt="NoneBotPluginLogo"></a>
@@ -72,12 +73,14 @@
 # 使用方法
 - **  聊天内容/绘图需求      （**是触发与Bot对话的关键字）
 - 记忆清除 清除当前用户的聊天记录
 
 # 可能存在的问题
 - 由于调教prompt的原因，机器人可能会偶尔出错，此时继续和TA对话或者是使用记忆清除命令重新开始对话即可。
 - 注意语言大模型的token消耗量
+- 插件目前没有实现绘图排队功能，所以请避免较多用户同时使用绘图功能。
 
 # TODO
 - [ ] 添加用户自定义人格功能
 - [ ] 代理支持
+- [ ] 支持绘图排队(NAI3只支持一次出一张图)
```

#### html2text {}

```diff
@@ -1,18 +1,18 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-nai3-bot Version: 0.0.1 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-nai3-bot Version: 0.0.2 Summary:
 åºäºGPT4+NovelAI
 V3,Botå¨å°èªç¶è¯­è¨è½¬æ¢ä¸ºNAI3æç¤ºè¯å¹¶ç»å¾åéçåæ¶,è¿ä¼ä»¥èªå®ä¹äººæ ¼åä½ èå¤©
 License: MIT Author: Alpaca Author-email: alpaca@bupt.edu.cn Requires-Python:
 >=3.8,<4.0 Classifier: License :: OSI Approved :: MIT License Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
-Python :: 3.11 Requires-Dist: nonebot-adapter-onebot (>=2.2.1,<3.0.0) Requires-
-Dist: nonebot2 (>=2.0.0rc3,<3.0.0) Requires-Dist: openai (>=1.30.1,<2.0.0)
-Description-Content-Type: text/markdown
+Python :: 3.11 Requires-Dist: Pillow (>=9.1.0,<10.0.0) Requires-Dist: nonebot-
+adapter-onebot (>=2.2.1,<3.0.0) Requires-Dist: nonebot2 (>=2.0.0rc3,<3.0.0)
+Requires-Dist: openai (>=1.30.1,<2.0.0) Description-Content-Type: text/markdown
                               _[_N_o_n_e_B_o_t_P_l_u_g_i_n_L_o_g_o_]
                               [NoneBotPluginText]
                            # nonebot-plugin-nai3-bot
 # ä»ç» - æ¬æä»¶åºäºGPT4+NovelAI
 V3,Botå¨å°èªç¶è¯­è¨è½¬æ¢ä¸ºNAI3æç¤ºè¯å¹¶ç»å¾åéçåæ¶ä»¥èªå®ä¹äººæ ¼ä¸ç¨æ·èå¤©ã
 -
 ç¨æ·å¯ä»¥æ­£å¸¸ä¸æå®äººæ ¼ï¼éè¦è°æprompt,ç®åæä»¶åç½®çäººæ ¼ä¸ºç¾¤åæå®çBAè§è²å¤©ç«¥ç±ä¸½ä¸ï¼èå¤©ãå¨èå¤©è¿ç¨ä¸­å¯ä»¥ä½¿ç¨èªç¶è¯­è¨æè¿°AIç»å¾çéæ±,Botä¼æ ¹æ®ç¨æ·çèå¤©åå®¹ä¿®æ¹AIç»å¾æç¨çæç¤ºè¯ï¼è§ææå¾ï¼,å¹¶ä¸å¤æ­æ¯å¦éè¦è°ç¨Novel
@@ -31,9 +31,11 @@
 ï¼å¯éï¼å¤§æ¨¡åä¸­è½¬æå¡åæä¾çä¸­è½¬å°å,ä½¿ç¨OpenAIå®æ¹æå¡ä¸éè¦å¡«å
 oneapi_model = "gpt-4" #
 ï¼å¯éï¼ä½¿ç¨çè¯­è¨å¤§æ¨¡å,å»ºè®®ä½¿ç¨gpt4ægpt4oæ¨¡åä»¥è¾¾å°æ´å¥½çä½éªæææ­¤é¡¹,é»è®¤ä½¿ç¨gpt-
 4æ¨¡å ``` NAI3çtokenè·åå°åæ¹æ³ï¼ ![Alt](image.png) # ä½¿ç¨æ¹æ³
 - ** èå¤©åå®¹/ç»å¾éæ± ï¼**æ¯è§¦åä¸Botå¯¹è¯çå³é®å­ï¼ -
 è®°å¿æ¸é¤ æ¸é¤å½åç¨æ·çèå¤©è®°å½ # å¯è½å­å¨çé®é¢ -
 ç±äºè°æpromptçåå ï¼æºå¨äººå¯è½ä¼å¶å°åºéï¼æ­¤æ¶ç»§ç»­åTAå¯¹è¯æèæ¯ä½¿ç¨è®°å¿æ¸é¤å½ä»¤éæ°å¼å§å¯¹è¯å³å¯ã
-- æ³¨æè¯­è¨å¤§æ¨¡åçtokenæ¶èé # TODO - [ ]
-æ·»å ç¨æ·èªå®ä¹äººæ ¼åè½ - [ ] ä»£çæ¯æ
+- æ³¨æè¯­è¨å¤§æ¨¡åçtokenæ¶èé -
+æä»¶ç®åæ²¡æå®ç°ç»å¾æéåè½ï¼æä»¥è¯·é¿åè¾å¤ç¨æ·åæ¶ä½¿ç¨ç»å¾åè½ã
+# TODO - [ ] æ·»å ç¨æ·èªå®ä¹äººæ ¼åè½ - [ ] ä»£çæ¯æ - [ ]
+æ¯æç»å¾æé(NAI3åªæ¯æä¸æ¬¡åºä¸å¼ å¾)
```

