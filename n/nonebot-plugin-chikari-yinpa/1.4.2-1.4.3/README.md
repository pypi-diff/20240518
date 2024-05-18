# Comparing `tmp/nonebot_plugin_chikari_yinpa-1.4.2.tar.gz` & `tmp/nonebot_plugin_chikari_yinpa-1.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_chikari_yinpa-1.4.2.tar", last modified: Thu May  2 12:33:00 2024, max compression
+gzip compressed data, was "nonebot_plugin_chikari_yinpa-1.4.3.tar", last modified: Sat May 18 04:21:24 2024, max compression
```

## Comparing `nonebot_plugin_chikari_yinpa-1.4.2.tar` & `nonebot_plugin_chikari_yinpa-1.4.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2024-05-02 12:33:00.469800 nonebot_plugin_chikari_yinpa-1.4.2/
--rw-rw-rw-   0        0        0     1065 2024-02-11 07:24:25.000000 nonebot_plugin_chikari_yinpa-1.4.2/LICENSE
--rw-rw-rw-   0        0        0     4734 2024-05-02 12:33:00.469800 nonebot_plugin_chikari_yinpa-1.4.2/PKG-INFO
--rw-rw-rw-   0        0        0     4033 2024-03-16 14:39:20.000000 nonebot_plugin_chikari_yinpa-1.4.2/README.md
-drwxrwxrwx   0        0        0        0 2024-05-02 12:33:00.461822 nonebot_plugin_chikari_yinpa-1.4.2/nonebot_plugin_chikari_yinpa/
--rw-rw-rw-   0        0        0     2835 2024-05-02 12:32:14.000000 nonebot_plugin_chikari_yinpa-1.4.2/nonebot_plugin_chikari_yinpa/__init__.py
--rw-rw-rw-   0        0        0      684 2024-02-17 04:46:31.000000 nonebot_plugin_chikari_yinpa-1.4.2/nonebot_plugin_chikari_yinpa/config.py
--rw-rw-rw-   0        0        0     6161 2024-04-30 09:36:41.000000 nonebot_plugin_chikari_yinpa-1.4.2/nonebot_plugin_chikari_yinpa/data_handles.py
--rw-rw-rw-   0        0        0    15078 2024-04-30 09:40:40.000000 nonebot_plugin_chikari_yinpa-1.4.2/nonebot_plugin_chikari_yinpa/dicts.py
--rw-rw-rw-   0        0        0    36837 2024-05-02 12:32:14.000000 nonebot_plugin_chikari_yinpa-1.4.2/nonebot_plugin_chikari_yinpa/handles.py
--rw-rw-rw-   0        0        0    27358 2024-04-30 09:41:35.000000 nonebot_plugin_chikari_yinpa-1.4.2/nonebot_plugin_chikari_yinpa/utils.py
-drwxrwxrwx   0        0        0        0 2024-05-02 12:33:00.468803 nonebot_plugin_chikari_yinpa-1.4.2/nonebot_plugin_chikari_yinpa.egg-info/
--rw-rw-rw-   0        0        0     4734 2024-05-02 12:33:00.000000 nonebot_plugin_chikari_yinpa-1.4.2/nonebot_plugin_chikari_yinpa.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      536 2024-05-02 12:33:00.000000 nonebot_plugin_chikari_yinpa-1.4.2/nonebot_plugin_chikari_yinpa.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-02 12:33:00.000000 nonebot_plugin_chikari_yinpa-1.4.2/nonebot_plugin_chikari_yinpa.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       72 2024-05-02 12:33:00.000000 nonebot_plugin_chikari_yinpa-1.4.2/nonebot_plugin_chikari_yinpa.egg-info/requires.txt
--rw-rw-rw-   0        0        0       29 2024-05-02 12:33:00.000000 nonebot_plugin_chikari_yinpa-1.4.2/nonebot_plugin_chikari_yinpa.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       85 2024-05-02 12:33:00.470798 nonebot_plugin_chikari_yinpa-1.4.2/setup.cfg
--rw-rw-rw-   0        0        0      783 2024-05-02 12:32:11.000000 nonebot_plugin_chikari_yinpa-1.4.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-18 04:21:24.654308 nonebot_plugin_chikari_yinpa-1.4.3/
+-rw-rw-rw-   0        0        0     1065 2024-02-11 07:24:25.000000 nonebot_plugin_chikari_yinpa-1.4.3/LICENSE
+-rw-rw-rw-   0        0        0     4734 2024-05-18 04:21:24.653311 nonebot_plugin_chikari_yinpa-1.4.3/PKG-INFO
+-rw-rw-rw-   0        0        0     4033 2024-03-16 14:39:20.000000 nonebot_plugin_chikari_yinpa-1.4.3/README.md
+drwxrwxrwx   0        0        0        0 2024-05-18 04:21:24.643337 nonebot_plugin_chikari_yinpa-1.4.3/nonebot_plugin_chikari_yinpa/
+-rw-rw-rw-   0        0        0     2835 2024-05-17 14:59:46.000000 nonebot_plugin_chikari_yinpa-1.4.3/nonebot_plugin_chikari_yinpa/__init__.py
+-rw-rw-rw-   0        0        0      684 2024-02-17 04:46:31.000000 nonebot_plugin_chikari_yinpa-1.4.3/nonebot_plugin_chikari_yinpa/config.py
+-rw-rw-rw-   0        0        0     6161 2024-04-30 09:36:41.000000 nonebot_plugin_chikari_yinpa-1.4.3/nonebot_plugin_chikari_yinpa/data_handles.py
+-rw-rw-rw-   0        0        0    15078 2024-04-30 09:40:40.000000 nonebot_plugin_chikari_yinpa-1.4.3/nonebot_plugin_chikari_yinpa/dicts.py
+-rw-rw-rw-   0        0        0    36839 2024-05-17 14:59:52.000000 nonebot_plugin_chikari_yinpa-1.4.3/nonebot_plugin_chikari_yinpa/handles.py
+-rw-rw-rw-   0        0        0    27358 2024-05-17 14:59:47.000000 nonebot_plugin_chikari_yinpa-1.4.3/nonebot_plugin_chikari_yinpa/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-18 04:21:24.652315 nonebot_plugin_chikari_yinpa-1.4.3/nonebot_plugin_chikari_yinpa.egg-info/
+-rw-rw-rw-   0        0        0     4734 2024-05-18 04:21:24.000000 nonebot_plugin_chikari_yinpa-1.4.3/nonebot_plugin_chikari_yinpa.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      536 2024-05-18 04:21:24.000000 nonebot_plugin_chikari_yinpa-1.4.3/nonebot_plugin_chikari_yinpa.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-18 04:21:24.000000 nonebot_plugin_chikari_yinpa-1.4.3/nonebot_plugin_chikari_yinpa.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       72 2024-05-18 04:21:24.000000 nonebot_plugin_chikari_yinpa-1.4.3/nonebot_plugin_chikari_yinpa.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       29 2024-05-18 04:21:24.000000 nonebot_plugin_chikari_yinpa-1.4.3/nonebot_plugin_chikari_yinpa.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       85 2024-05-18 04:21:24.655305 nonebot_plugin_chikari_yinpa-1.4.3/setup.cfg
+-rw-rw-rw-   0        0        0      783 2024-05-17 14:59:45.000000 nonebot_plugin_chikari_yinpa-1.4.3/setup.py
```

### Comparing `nonebot_plugin_chikari_yinpa-1.4.2/LICENSE` & `nonebot_plugin_chikari_yinpa-1.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_chikari_yinpa-1.4.2/PKG-INFO` & `nonebot_plugin_chikari_yinpa-1.4.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot_plugin_chikari_yinpa
-Version: 1.4.2
+Version: 1.4.3
 Summary: A plugin for nonebot 2
 Home-page: https://github.com/mrqx0195/nonebot_plugin_chikari_yinpa
 Author: mrqx0195
 Author-email: 2317249571@qq.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot_plugin_chikari_yinpa Version: 1.4.2
+Metadata-Version: 2.1 Name: nonebot_plugin_chikari_yinpa Version: 1.4.3
 Summary: A plugin for nonebot 2 Home-page: https://github.com/mrqx0195/
 nonebot_plugin_chikari_yinpa Author: mrqx0195 Author-email: 2317249571@qq.com
 Classifier: Programming Language :: Python :: 3 Classifier: License :: OSI
 Approved :: MIT License Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
 pillow Requires-Dist: nonebot2>=2.2.0 Requires-Dist: nonebot-adapter-onebot
 Requires-Dist: nonebot-plugin-localstore
```

### Comparing `nonebot_plugin_chikari_yinpa-1.4.2/README.md` & `nonebot_plugin_chikari_yinpa-1.4.3/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_chikari_yinpa-1.4.2/nonebot_plugin_chikari_yinpa/__init__.py` & `nonebot_plugin_chikari_yinpa-1.4.3/nonebot_plugin_chikari_yinpa/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     usage="",
     config=Config,
     type="application",
     homepage="https://github.com/mrqx0195/nonebot_plugin_chikari_yinpa",
     supported_adapters={"~onebot.v11"}
 )
 
-__version__ = "1.4.2"
+__version__ = "1.4.3"
 
 on_yinpa_control = on_command(
     "yinpa_control",
     aliases={"银趴控制"},
     permission=SUPERUSER | GROUP_ADMIN | GROUP_OWNER,
     priority=10,
     block=False,
```

### Comparing `nonebot_plugin_chikari_yinpa-1.4.2/nonebot_plugin_chikari_yinpa/config.py` & `nonebot_plugin_chikari_yinpa-1.4.3/nonebot_plugin_chikari_yinpa/config.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_chikari_yinpa-1.4.2/nonebot_plugin_chikari_yinpa/data_handles.py` & `nonebot_plugin_chikari_yinpa-1.4.3/nonebot_plugin_chikari_yinpa/data_handles.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_chikari_yinpa-1.4.2/nonebot_plugin_chikari_yinpa/dicts.py` & `nonebot_plugin_chikari_yinpa-1.4.3/nonebot_plugin_chikari_yinpa/dicts.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_chikari_yinpa-1.4.2/nonebot_plugin_chikari_yinpa/handles.py` & `nonebot_plugin_chikari_yinpa-1.4.3/nonebot_plugin_chikari_yinpa/handles.py`

 * *Files 0% similar despite different names*

```diff
@@ -68,15 +68,15 @@
         if Utils.yinpa_user_presence_check(event.get_user_id()):
             await matcher.finish("您已加入银趴！\n如果想要重置银趴数据，请使用 /leave_yinpa 或 /离开银趴 离开银趴后再加入")
         uid: str = event.get_user_id()
         command: str = args.extract_plain_text()
         arg_list: list = command.split()
         if not len(arg_list) == 2:
             bot = get_bots()[(str)(event.self_id)]
-            name: str = await bot.call_api("get_group_member_info",group_id = event.group_id,user_id = uid)["nickname"]
+            name: str = (await bot.call_api("get_group_member_info",group_id = event.group_id,user_id = uid))["nickname"]
         else:
             name: str = arg_list[0]
         if (int)(arg_list[1]) <= 0:
             species: int = Utils.dice(7,event.get_user_id())
         else:
             if not arg_list[1].isdigit():
                 await matcher.finish("参数错误！\n种族应为一个正整数（种族编号）\n种族列表参照： /yinpa_help 种族 ")
```

### Comparing `nonebot_plugin_chikari_yinpa-1.4.2/nonebot_plugin_chikari_yinpa/utils.py` & `nonebot_plugin_chikari_yinpa-1.4.3/nonebot_plugin_chikari_yinpa/utils.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_chikari_yinpa-1.4.2/nonebot_plugin_chikari_yinpa.egg-info/PKG-INFO` & `nonebot_plugin_chikari_yinpa-1.4.3/nonebot_plugin_chikari_yinpa.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot_plugin_chikari_yinpa
-Version: 1.4.2
+Version: 1.4.3
 Summary: A plugin for nonebot 2
 Home-page: https://github.com/mrqx0195/nonebot_plugin_chikari_yinpa
 Author: mrqx0195
 Author-email: 2317249571@qq.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot_plugin_chikari_yinpa Version: 1.4.2
+Metadata-Version: 2.1 Name: nonebot_plugin_chikari_yinpa Version: 1.4.3
 Summary: A plugin for nonebot 2 Home-page: https://github.com/mrqx0195/
 nonebot_plugin_chikari_yinpa Author: mrqx0195 Author-email: 2317249571@qq.com
 Classifier: Programming Language :: Python :: 3 Classifier: License :: OSI
 Approved :: MIT License Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
 pillow Requires-Dist: nonebot2>=2.2.0 Requires-Dist: nonebot-adapter-onebot
 Requires-Dist: nonebot-plugin-localstore
```

### Comparing `nonebot_plugin_chikari_yinpa-1.4.2/nonebot_plugin_chikari_yinpa.egg-info/SOURCES.txt` & `nonebot_plugin_chikari_yinpa-1.4.3/nonebot_plugin_chikari_yinpa.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_chikari_yinpa-1.4.2/setup.py` & `nonebot_plugin_chikari_yinpa-1.4.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding='utf-8') as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="nonebot_plugin_chikari_yinpa",
-    version="1.4.2",
+    version="1.4.3",
     author="mrqx0195",
     author_email="2317249571@qq.com",
     description="A plugin for nonebot 2",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/mrqx0195/nonebot_plugin_chikari_yinpa",
     packages=setuptools.find_packages(),
```

