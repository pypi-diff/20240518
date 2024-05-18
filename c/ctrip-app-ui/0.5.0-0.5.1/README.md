# Comparing `tmp/ctrip-app-ui-0.5.0.tar.gz` & `tmp/ctrip-app-ui-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ctrip-app-ui-0.5.0.tar", last modified: Sat May 18 14:41:34 2024, max compression
+gzip compressed data, was "ctrip-app-ui-0.5.1.tar", last modified: Sat May 18 15:03:58 2024, max compression
```

## Comparing `ctrip-app-ui-0.5.0.tar` & `ctrip-app-ui-0.5.1.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxrwx   0        0        0        0 2024-05-18 14:41:34.143525 ctrip-app-ui-0.5.0/
--rw-rw-rw-   0        0        0    11558 2024-04-24 09:02:35.000000 ctrip-app-ui-0.5.0/LICENSE
--rw-rw-rw-   0        0        0      474 2024-05-18 14:41:34.141529 ctrip-app-ui-0.5.0/PKG-INFO
--rw-rw-rw-   0        0        0       47 2024-04-24 09:02:35.000000 ctrip-app-ui-0.5.0/README.md
-drwxrwxrwx   0        0        0        0 2024-05-18 14:41:34.114598 ctrip-app-ui-0.5.0/capp_ui/
--rw-rw-rw-   0        0        0      470 2024-04-24 09:06:21.000000 ctrip-app-ui-0.5.0/capp_ui/__init__.py
--rw-rw-rw-   0        0        0      736 2024-05-06 07:02:29.000000 ctrip-app-ui-0.5.0/capp_ui/config.py
--rw-rw-rw-   0        0        0     4060 2024-05-07 16:57:27.000000 ctrip-app-ui-0.5.0/capp_ui/date_extend.py
--rw-rw-rw-   0        0        0     1664 2024-05-09 13:31:21.000000 ctrip-app-ui-0.5.0/capp_ui/device.py
--rw-rw-rw-   0        0        0     1391 2024-04-25 08:27:58.000000 ctrip-app-ui-0.5.0/capp_ui/dir.py
--rw-rw-rw-   0        0        0    44529 2024-05-18 14:41:16.000000 ctrip-app-ui-0.5.0/capp_ui/domain_service.py
--rw-rw-rw-   0        0        0      613 2024-04-24 15:31:00.000000 ctrip-app-ui-0.5.0/capp_ui/fee.py
--rw-rw-rw-   0        0        0     5414 2024-05-18 14:39:38.000000 ctrip-app-ui-0.5.0/capp_ui/libs.py
--rw-rw-rw-   0        0        0    24821 2024-05-13 17:15:14.000000 ctrip-app-ui-0.5.0/capp_ui/mobile_terminals.py
--rw-rw-rw-   0        0        0     1719 2024-04-28 16:15:39.000000 ctrip-app-ui-0.5.0/capp_ui/platforms.py
--rw-rw-rw-   0        0        0      765 2024-04-28 16:02:26.000000 ctrip-app-ui-0.5.0/capp_ui/test.py
--rw-rw-rw-   0        0        0     5486 2024-05-11 03:13:30.000000 ctrip-app-ui-0.5.0/capp_ui/utils.py
--rw-rw-rw-   0        0        0     3023 2024-05-11 03:13:43.000000 ctrip-app-ui-0.5.0/capp_ui/validators.py
-drwxrwxrwx   0        0        0        0 2024-05-18 14:41:34.139534 ctrip-app-ui-0.5.0/ctrip_app_ui.egg-info/
--rw-rw-rw-   0        0        0      474 2024-05-18 14:41:33.000000 ctrip-app-ui-0.5.0/ctrip_app_ui.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      460 2024-05-18 14:41:33.000000 ctrip-app-ui-0.5.0/ctrip_app_ui.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-18 14:41:33.000000 ctrip-app-ui-0.5.0/ctrip_app_ui.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       30 2024-05-18 14:41:33.000000 ctrip-app-ui-0.5.0/ctrip_app_ui.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-05-18 14:41:33.000000 ctrip-app-ui-0.5.0/ctrip_app_ui.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-18 14:41:34.143525 ctrip-app-ui-0.5.0/setup.cfg
--rw-rw-rw-   0        0        0     1087 2024-05-18 14:41:30.000000 ctrip-app-ui-0.5.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-18 15:03:58.605503 ctrip-app-ui-0.5.1/
+-rw-rw-rw-   0        0        0    11558 2024-04-24 09:02:35.000000 ctrip-app-ui-0.5.1/LICENSE
+-rw-rw-rw-   0        0        0      474 2024-05-18 15:03:58.604506 ctrip-app-ui-0.5.1/PKG-INFO
+-rw-rw-rw-   0        0        0       47 2024-04-24 09:02:35.000000 ctrip-app-ui-0.5.1/README.md
+drwxrwxrwx   0        0        0        0 2024-05-18 15:03:58.577535 ctrip-app-ui-0.5.1/capp_ui/
+-rw-rw-rw-   0        0        0      470 2024-04-24 09:06:21.000000 ctrip-app-ui-0.5.1/capp_ui/__init__.py
+-rw-rw-rw-   0        0        0      736 2024-05-06 07:02:29.000000 ctrip-app-ui-0.5.1/capp_ui/config.py
+-rw-rw-rw-   0        0        0     4060 2024-05-07 16:57:27.000000 ctrip-app-ui-0.5.1/capp_ui/date_extend.py
+-rw-rw-rw-   0        0        0     1664 2024-05-09 13:31:21.000000 ctrip-app-ui-0.5.1/capp_ui/device.py
+-rw-rw-rw-   0        0        0     1391 2024-04-25 08:27:58.000000 ctrip-app-ui-0.5.1/capp_ui/dir.py
+-rw-rw-rw-   0        0        0    45770 2024-05-18 15:03:27.000000 ctrip-app-ui-0.5.1/capp_ui/domain_service.py
+-rw-rw-rw-   0        0        0      613 2024-04-24 15:31:00.000000 ctrip-app-ui-0.5.1/capp_ui/fee.py
+-rw-rw-rw-   0        0        0     5414 2024-05-18 14:39:38.000000 ctrip-app-ui-0.5.1/capp_ui/libs.py
+-rw-rw-rw-   0        0        0    24821 2024-05-13 17:15:14.000000 ctrip-app-ui-0.5.1/capp_ui/mobile_terminals.py
+-rw-rw-rw-   0        0        0     1719 2024-04-28 16:15:39.000000 ctrip-app-ui-0.5.1/capp_ui/platforms.py
+-rw-rw-rw-   0        0        0      765 2024-04-28 16:02:26.000000 ctrip-app-ui-0.5.1/capp_ui/test.py
+-rw-rw-rw-   0        0        0     5486 2024-05-11 03:13:30.000000 ctrip-app-ui-0.5.1/capp_ui/utils.py
+-rw-rw-rw-   0        0        0     3023 2024-05-11 03:13:43.000000 ctrip-app-ui-0.5.1/capp_ui/validators.py
+drwxrwxrwx   0        0        0        0 2024-05-18 15:03:58.602531 ctrip-app-ui-0.5.1/ctrip_app_ui.egg-info/
+-rw-rw-rw-   0        0        0      474 2024-05-18 15:03:58.000000 ctrip-app-ui-0.5.1/ctrip_app_ui.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      460 2024-05-18 15:03:58.000000 ctrip-app-ui-0.5.1/ctrip_app_ui.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-18 15:03:58.000000 ctrip-app-ui-0.5.1/ctrip_app_ui.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       30 2024-05-18 15:03:58.000000 ctrip-app-ui-0.5.1/ctrip_app_ui.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-05-18 15:03:58.000000 ctrip-app-ui-0.5.1/ctrip_app_ui.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-18 15:03:58.606501 ctrip-app-ui-0.5.1/setup.cfg
+-rw-rw-rw-   0        0        0     1087 2024-05-18 15:03:53.000000 ctrip-app-ui-0.5.1/setup.py
```

### Comparing `ctrip-app-ui-0.5.0/LICENSE` & `ctrip-app-ui-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.5.0/capp_ui/config.py` & `ctrip-app-ui-0.5.1/capp_ui/config.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.5.0/capp_ui/date_extend.py` & `ctrip-app-ui-0.5.1/capp_ui/date_extend.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.5.0/capp_ui/device.py` & `ctrip-app-ui-0.5.1/capp_ui/device.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.5.0/capp_ui/dir.py` & `ctrip-app-ui-0.5.1/capp_ui/dir.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.5.0/capp_ui/domain_service.py` & `ctrip-app-ui-0.5.1/capp_ui/domain_service.py`

 * *Files 1% similar despite different names*

```diff
@@ -70,34 +70,14 @@
             logger.warning("手机没有开启导航栏")
         except Exception as e:
             logger.error("导航栏元素定位失败，error: {}".format(e))
 
     @LoopFindElementObject(loop=20, action="查找主页【我的】", sleep=1)
     def get_my_home(self) -> dict:
         try:
-            my_button = self.device.poco(
-                type="android.widget.ImageView", name="ctrip.android.view:id/home_tab_bar_icon_iv"
-            )
-            if my_button.exists() is True:
-                return {"element": my_button}
-        except (Exception,):
-            pass
-        try:
-            my_button = self.device.poco(type="android.view.ViewGroup", name="ctrip.android.view:id/a", desc="我的")
-            if my_button.exists() is True:
-                return {"element": my_button}
-        except (Exception,):
-            pass
-        try:
-            my_button = self.device.poco(type="android.widget.TextView", name="android.widget.TextView", desc="我的")
-            if my_button.exists() is True:
-                return {"element": my_button}
-        except (Exception,):
-            pass
-        try:
             file_name = join_path([get_images_dir(), "我的.png"])
             if is_exists(file_name):
                 temp = self.device.get_cv_template(file_name=file_name, threshold=0.9)
                 pos = self.device.exists(v=temp)
                 if pos:
                     return {"pos": pos}
             else:
@@ -114,14 +94,34 @@
                 if pos:
                     self.device.touch(v=pos)
             else:
                 # temp = (183, 1923)  # Huawei Mate 20手机上对应的坐标位置，其他型号手机可能不是这个值
                 logger.warning("文件{}，没找到".format(file_name))
         except (Exception,):
             pass
+        try:
+            my_button = self.device.poco(
+                type="android.widget.ImageView", name="ctrip.android.view:id/home_tab_bar_icon_iv"
+            )
+            if my_button.exists() is True:
+                return {"element": my_button}
+        except (Exception,):
+            pass
+        try:
+            my_button = self.device.poco(type="android.view.ViewGroup", name="ctrip.android.view:id/a", desc="我的")
+            if my_button.exists() is True:
+                return {"element": my_button}
+        except (Exception,):
+            pass
+        try:
+            my_button = self.device.poco(type="android.widget.TextView", name="android.widget.TextView", desc="我的")
+            if my_button.exists() is True:
+                return {"element": my_button}
+        except (Exception,):
+            pass
         return dict()
 
     def touch_element(self, attr: dict, sleep: int = 1) -> None:
         """进入app后，点击【我的】"""
         pos = attr.get("pos")
         element = attr.get("element")
         if pos:
@@ -153,14 +153,26 @@
         )
         logout_user.click()
 
     @LoopFindElementObject(loop=20, action="找到我的主页【待付款】", sleep=1)
     def get_todo_unpaid(self) -> dict:
         """进入my主页后，点击【待付款】"""
         try:
+            file_name = join_path([get_images_dir(), "我的待办_待付款.png"])
+            if is_exists(file_name):
+                temp = self.device.get_cv_template(file_name=file_name, threshold=0.9)
+                pos = self.device.exists(v=temp)
+                if pos:
+                    return {"pos": pos}
+            else:
+                # temp = (417, 947)  # Huawei Mate 20手机上对应的坐标位置，其他型号手机可能不是这个值
+                logger.warning("文件{}，没找到".format(file_name))
+        except (Exception,):
+            pass
+        try:
             # 待付款元素定位1
             unpaid_button = self.device.poco(
                 type="android.widget.TextView", name="ctrip.android.view:id/a", text="待付款"
             )
             if unpaid_button.exists() is True:
                 return {"element": unpaid_button}
         except (Exception,):
@@ -170,39 +182,19 @@
             unpaid_button = self.device.poco(
                 type="android.widget.TextView", name="android.widget.TextView", text="待付款"
             )
             if unpaid_button.exists() is True:
                 return {"element": unpaid_button}
         except (Exception,):
             pass
-        try:
-            file_name = join_path([get_images_dir(), "我的待办_待付款.png"])
-            if is_exists(file_name):
-                temp = self.device.get_cv_template(file_name=file_name, threshold=0.9)
-                pos = self.device.exists(v=temp)
-                if pos:
-                    return {"pos": pos}
-            else:
-                # temp = (417, 947)  # Huawei Mate 20手机上对应的坐标位置，其他型号手机可能不是这个值
-                logger.warning("文件{}，没找到".format(file_name))
-        except (Exception,):
-            pass
         return dict()
 
     @LoopFindElementObject(loop=20, action="订单列表-待付款页查到【搜索】", sleep=1)
     def get_unpaid_page_search_box(self) -> dict:
         try:
-            search_box = self.device.poco(
-                type="android.widget.TextView", name="android.widget.TextView", text="搜索订单"
-            )
-            if search_box.exists() is True:
-                return {"element": search_box}
-        except (Exception,):
-            pass
-        try:
             file_name = join_path([get_images_dir(), "搜索订单_搜索框.png"])
             if is_exists(file_name):
                 temp = self.device.get_cv_template(file_name=file_name, threshold=0.9)
                 pos = self.device.exists(v=temp)
                 if pos:
                     return {"pos": pos}
             else:
@@ -218,14 +210,23 @@
                 if pos:
                     return {"pos": pos}
             else:
                 # temp = (896, 173)  # Huawei Mate 20手机上对应的坐标位置，其他型号手机可能不是这个值
                 logger.warning("文件{}，没找到".format(file_name))
         except (Exception,):
             pass
+        try:
+            search_box = self.device.poco(
+                type="android.widget.TextView", name="android.widget.TextView", text="搜索订单"
+            )
+            if search_box.exists() is True:
+                return {"element": search_box}
+        except (Exception,):
+            pass
+        return dict()
 
     @LoopFindElementObject(loop=20, action="搜索页查找【搜索】", sleep=1)
     def get_search_page_search_box(self) -> dict:
         try:
             search_box = self.device.poco(
                 type="android.widget.EditText", name="android.widget.EditText", text="输入城市名/订单号 搜索订单"
             )
@@ -263,14 +264,50 @@
             self.device.keyevent(keyname="66")
             time.sleep(sleep)
             return True
 
     def get_order_status_with_order_list(self) -> str:
         """检查搜索列表界面，获取订单的状态"""
         try:
+            file_name = join_path([get_images_dir(), "订单状态_待支付.png"])
+            if is_exists(file_name):
+                temp = self.device.get_cv_template(file_name=file_name, threshold=0.9)
+                pos = self.device.exists(v=temp)
+                if pos:
+                    return "待支付"
+            else:
+                # temp = (1033, 381)  # Huawei Mate 20手机上对应的坐标位置，其他型号手机可能不是这个值
+                logger.warning("文件{}，没找到".format(file_name))
+        except (Exception,):
+            pass
+        try:
+            file_name = join_path([get_images_dir(), "订单状态_已出票.png"])
+            if is_exists(file_name):
+                temp = self.device.get_cv_template(file_name=file_name, threshold=0.9)
+                pos = self.device.exists(v=temp)
+                if pos:
+                    return "已出票"
+            else:
+                # temp = (1033, 381)  # Huawei Mate 20手机上对应的坐标位置，其他型号手机可能不是这个值
+                logger.warning("文件{}，没找到".format(file_name))
+        except (Exception,):
+            pass
+        try:
+            file_name = join_path([get_images_dir(), "订单状态_已取消.png"])
+            if is_exists(file_name):
+                temp = self.device.get_cv_template(file_name=file_name, threshold=0.9)
+                pos = self.device.exists(v=temp)
+                if pos:
+                    return "已取消"
+            else:
+                # temp = (1033, 381)  # Huawei Mate 20手机上对应的坐标位置，其他型号手机可能不是这个值
+                logger.warning("文件{}，没找到".format(file_name))
+        except (Exception,):
+            pass
+        try:
             unpaid_status = self.device.poco(
                 type="android.widget.TextView", name="android.widget.TextView", text="去支付"
             )
             if unpaid_status.exists() is True:
                 return "待支付"
         except (PocoNoSuchNodeException, PocoTargetTimeout, Exception):
             pass
@@ -279,26 +316,14 @@
                 type="android.widget.TextView", name="android.widget.TextView", text="待支付"
             )
             if unpaid_status.exists() is True:
                 return "待支付"
         except (Exception,):
             pass
         try:
-            file_name = join_path([get_images_dir(), "订单状态_待支付.png"])
-            if is_exists(file_name):
-                temp = self.device.get_cv_template(file_name=file_name, threshold=0.9)
-                pos = self.device.exists(v=temp)
-                if pos:
-                    return "待支付"
-            else:
-                # temp = (1033, 381)  # Huawei Mate 20手机上对应的坐标位置，其他型号手机可能不是这个值
-                logger.warning("文件{}，没找到".format(file_name))
-        except (Exception,):
-            pass
-        try:
             cancel_status = self.device.poco(
                 type="android.widget.TextView", name="android.widget.TextView", text="已取消"
             )
             if cancel_status.exists() is True:
                 return "已取消"
         except (PocoNoSuchNodeException, PocoTargetTimeout, Exception):
             pass
```

### Comparing `ctrip-app-ui-0.5.0/capp_ui/fee.py` & `ctrip-app-ui-0.5.1/capp_ui/fee.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.5.0/capp_ui/libs.py` & `ctrip-app-ui-0.5.1/capp_ui/libs.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.5.0/capp_ui/mobile_terminals.py` & `ctrip-app-ui-0.5.1/capp_ui/mobile_terminals.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.5.0/capp_ui/platforms.py` & `ctrip-app-ui-0.5.1/capp_ui/platforms.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.5.0/capp_ui/test.py` & `ctrip-app-ui-0.5.1/capp_ui/test.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.5.0/capp_ui/utils.py` & `ctrip-app-ui-0.5.1/capp_ui/utils.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.5.0/capp_ui/validators.py` & `ctrip-app-ui-0.5.1/capp_ui/validators.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.5.0/setup.py` & `ctrip-app-ui-0.5.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 # Copyright ©2011-2024. Hunan xxxxxxx Company limited. All rights reserved.
 # ---------------------------------------------------------------------------------------------------------
 """
 from setuptools import setup, find_packages
 
 setup(
     name='ctrip-app-ui',
-    version='0.5.0',
+    version='0.5.1',
     description='This is my ctrip app ui package',
     long_description='This is my ctrip app ui package',
     author='ckf10000',
     author_email='ckf10000@sina.com',
     url='https://github.com/ckf10000/ctrip-app-ui',
     packages=find_packages(),
     install_requires=[
```

