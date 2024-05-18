# Comparing `tmp/ctrip-app-ui-0.4.8.tar.gz` & `tmp/ctrip-app-ui-0.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ctrip-app-ui-0.4.8.tar", last modified: Sat May 18 08:54:53 2024, max compression
+gzip compressed data, was "ctrip-app-ui-0.4.9.tar", last modified: Sat May 18 14:21:24 2024, max compression
```

## Comparing `ctrip-app-ui-0.4.8.tar` & `ctrip-app-ui-0.4.9.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxrwx   0        0        0        0 2024-05-18 08:54:53.307423 ctrip-app-ui-0.4.8/
--rw-rw-rw-   0        0        0    11558 2024-04-24 09:02:35.000000 ctrip-app-ui-0.4.8/LICENSE
--rw-rw-rw-   0        0        0      474 2024-05-18 08:54:53.305397 ctrip-app-ui-0.4.8/PKG-INFO
--rw-rw-rw-   0        0        0       47 2024-04-24 09:02:35.000000 ctrip-app-ui-0.4.8/README.md
-drwxrwxrwx   0        0        0        0 2024-05-18 08:54:53.278471 ctrip-app-ui-0.4.8/capp_ui/
--rw-rw-rw-   0        0        0      470 2024-04-24 09:06:21.000000 ctrip-app-ui-0.4.8/capp_ui/__init__.py
--rw-rw-rw-   0        0        0      736 2024-05-06 07:02:29.000000 ctrip-app-ui-0.4.8/capp_ui/config.py
--rw-rw-rw-   0        0        0     4060 2024-05-07 16:57:27.000000 ctrip-app-ui-0.4.8/capp_ui/date_extend.py
--rw-rw-rw-   0        0        0     1664 2024-05-09 13:31:21.000000 ctrip-app-ui-0.4.8/capp_ui/device.py
--rw-rw-rw-   0        0        0     1391 2024-04-25 08:27:58.000000 ctrip-app-ui-0.4.8/capp_ui/dir.py
--rw-rw-rw-   0        0        0    80683 2024-05-18 08:52:06.000000 ctrip-app-ui-0.4.8/capp_ui/domain_service.py
--rw-rw-rw-   0        0        0      613 2024-04-24 15:31:00.000000 ctrip-app-ui-0.4.8/capp_ui/fee.py
--rw-rw-rw-   0        0        0     4653 2024-05-18 04:20:17.000000 ctrip-app-ui-0.4.8/capp_ui/libs.py
--rw-rw-rw-   0        0        0    24821 2024-05-13 17:15:14.000000 ctrip-app-ui-0.4.8/capp_ui/mobile_terminals.py
--rw-rw-rw-   0        0        0     1719 2024-04-28 16:15:39.000000 ctrip-app-ui-0.4.8/capp_ui/platforms.py
--rw-rw-rw-   0        0        0      765 2024-04-28 16:02:26.000000 ctrip-app-ui-0.4.8/capp_ui/test.py
--rw-rw-rw-   0        0        0     5486 2024-05-11 03:13:30.000000 ctrip-app-ui-0.4.8/capp_ui/utils.py
--rw-rw-rw-   0        0        0     3023 2024-05-11 03:13:43.000000 ctrip-app-ui-0.4.8/capp_ui/validators.py
-drwxrwxrwx   0        0        0        0 2024-05-18 08:54:53.304400 ctrip-app-ui-0.4.8/ctrip_app_ui.egg-info/
--rw-rw-rw-   0        0        0      474 2024-05-18 08:54:52.000000 ctrip-app-ui-0.4.8/ctrip_app_ui.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      460 2024-05-18 08:54:52.000000 ctrip-app-ui-0.4.8/ctrip_app_ui.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-18 08:54:52.000000 ctrip-app-ui-0.4.8/ctrip_app_ui.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       30 2024-05-18 08:54:52.000000 ctrip-app-ui-0.4.8/ctrip_app_ui.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-05-18 08:54:52.000000 ctrip-app-ui-0.4.8/ctrip_app_ui.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-18 08:54:53.307423 ctrip-app-ui-0.4.8/setup.cfg
--rw-rw-rw-   0        0        0     1087 2024-05-18 08:54:38.000000 ctrip-app-ui-0.4.8/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-18 14:21:24.890128 ctrip-app-ui-0.4.9/
+-rw-rw-rw-   0        0        0    11558 2024-04-24 09:02:35.000000 ctrip-app-ui-0.4.9/LICENSE
+-rw-rw-rw-   0        0        0      474 2024-05-18 14:21:24.888132 ctrip-app-ui-0.4.9/PKG-INFO
+-rw-rw-rw-   0        0        0       47 2024-04-24 09:02:35.000000 ctrip-app-ui-0.4.9/README.md
+drwxrwxrwx   0        0        0        0 2024-05-18 14:21:24.861188 ctrip-app-ui-0.4.9/capp_ui/
+-rw-rw-rw-   0        0        0      470 2024-04-24 09:06:21.000000 ctrip-app-ui-0.4.9/capp_ui/__init__.py
+-rw-rw-rw-   0        0        0      736 2024-05-06 07:02:29.000000 ctrip-app-ui-0.4.9/capp_ui/config.py
+-rw-rw-rw-   0        0        0     4060 2024-05-07 16:57:27.000000 ctrip-app-ui-0.4.9/capp_ui/date_extend.py
+-rw-rw-rw-   0        0        0     1664 2024-05-09 13:31:21.000000 ctrip-app-ui-0.4.9/capp_ui/device.py
+-rw-rw-rw-   0        0        0     1391 2024-04-25 08:27:58.000000 ctrip-app-ui-0.4.9/capp_ui/dir.py
+-rw-rw-rw-   0        0        0    44529 2024-05-18 14:20:01.000000 ctrip-app-ui-0.4.9/capp_ui/domain_service.py
+-rw-rw-rw-   0        0        0      613 2024-04-24 15:31:00.000000 ctrip-app-ui-0.4.9/capp_ui/fee.py
+-rw-rw-rw-   0        0        0     5408 2024-05-18 11:39:51.000000 ctrip-app-ui-0.4.9/capp_ui/libs.py
+-rw-rw-rw-   0        0        0    24821 2024-05-13 17:15:14.000000 ctrip-app-ui-0.4.9/capp_ui/mobile_terminals.py
+-rw-rw-rw-   0        0        0     1719 2024-04-28 16:15:39.000000 ctrip-app-ui-0.4.9/capp_ui/platforms.py
+-rw-rw-rw-   0        0        0      765 2024-04-28 16:02:26.000000 ctrip-app-ui-0.4.9/capp_ui/test.py
+-rw-rw-rw-   0        0        0     5486 2024-05-11 03:13:30.000000 ctrip-app-ui-0.4.9/capp_ui/utils.py
+-rw-rw-rw-   0        0        0     3023 2024-05-11 03:13:43.000000 ctrip-app-ui-0.4.9/capp_ui/validators.py
+drwxrwxrwx   0        0        0        0 2024-05-18 14:21:24.886140 ctrip-app-ui-0.4.9/ctrip_app_ui.egg-info/
+-rw-rw-rw-   0        0        0      474 2024-05-18 14:21:24.000000 ctrip-app-ui-0.4.9/ctrip_app_ui.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      460 2024-05-18 14:21:24.000000 ctrip-app-ui-0.4.9/ctrip_app_ui.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-18 14:21:24.000000 ctrip-app-ui-0.4.9/ctrip_app_ui.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       30 2024-05-18 14:21:24.000000 ctrip-app-ui-0.4.9/ctrip_app_ui.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-05-18 14:21:24.000000 ctrip-app-ui-0.4.9/ctrip_app_ui.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-18 14:21:24.890128 ctrip-app-ui-0.4.9/setup.cfg
+-rw-rw-rw-   0        0        0     1087 2024-05-18 14:21:17.000000 ctrip-app-ui-0.4.9/setup.py
```

### Comparing `ctrip-app-ui-0.4.8/LICENSE` & `ctrip-app-ui-0.4.9/LICENSE`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.4.8/capp_ui/config.py` & `ctrip-app-ui-0.4.9/capp_ui/config.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.4.8/capp_ui/date_extend.py` & `ctrip-app-ui-0.4.9/capp_ui/date_extend.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.4.8/capp_ui/device.py` & `ctrip-app-ui-0.4.9/capp_ui/device.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.4.8/capp_ui/dir.py` & `ctrip-app-ui-0.4.9/capp_ui/dir.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.4.8/capp_ui/domain_service.py` & `ctrip-app-ui-0.4.9/capp_ui/domain_service.py`

 * *Files 24% similar despite different names*

```diff
@@ -13,21 +13,19 @@
 import time
 import typing as t
 from decimal import Decimal
 from poco.proxy import UIObjectProxy
 from poco.exceptions import PocoNoSuchNodeException, PocoTargetTimeout
 
 from capp_ui.platforms import PlatformService
-from capp_ui.utils import get_ui_object_proxy_attr
 from capp_ui.config import ctrip_soft_keyboard_position
 from capp_ui.mobile_terminals import stop_app, PocoProxy
 from capp_ui.date_extend import is_later_than_current_time
 from capp_ui.dir import get_images_dir, is_exists, join_path
-from capp_ui.date_extend import get_trip_year_month_day, get_datetime_area, is_public_holiday
-from capp_ui.libs import SleepWait, LoopFindElement, LoopFindElementSubmit, logger, LoopExcute
+from capp_ui.libs import SleepWait, LoopFindElementSubmit, logger, LoopFindElementObject
 
 
 class CtripAppService(object):
     """
     携程APP
     """
     IMAGE_DIR = get_images_dir()
@@ -69,82 +67,72 @@
             navigation_bar.click()
             logger.warning("手机导航栏已被隐藏")
         except (PocoNoSuchNodeException, PocoTargetTimeout):
             logger.warning("手机没有开启导航栏")
         except Exception as e:
             logger.error("导航栏元素定位失败，error: {}".format(e))
 
-    @LoopFindElementSubmit(loop=3, action="首页")
-    def touch_home(self):
-        """进入app后，点击【首页】"""
-        file_name = join_path([get_images_dir(), "首页.png"])
-        if is_exists(file_name):
-            temp = self.device.get_cv_template(file_name=file_name)
-        else:
-            temp = (154, 2878)  # LG g7手机上对应的坐标位置，其他型号手机可能不是这个值
-        self.device.touch(v=temp)
-
-    @LoopExcute(loop=20, action="点击【我的】", sleep=1)
-    def touch_my(self) -> bool:
-        """进入app后，点击【我的】"""
+    @LoopFindElementObject(loop=20, action="查找主页【我的】", sleep=1)
+    def get_my_home(self) -> dict:
         try:
             my_button = self.device.poco(
                 type="android.widget.ImageView", name="ctrip.android.view:id/home_tab_bar_icon_iv"
             )
             if my_button.exists() is True:
-                my_button.click()
-                time.sleep(0.5)
-                my_button = self.device.poco(
-                    type="android.widget.ImageView", name="ctrip.android.view:id/home_tab_bar_icon_iv"
-                )
-                if my_button.exists() is False:
-                    return True
+                return {"element": my_button}
         except (Exception,):
             pass
         try:
-
             my_button = self.device.poco(type="android.view.ViewGroup", name="ctrip.android.view:id/a", desc="我的")
             if my_button.exists() is True:
-                my_button.click()
-                time.sleep(0.5)
-                my_button = self.device.poco(type="android.view.ViewGroup", name="ctrip.android.view:id/a", desc="我的")
-                if my_button.exists() is False:
-                    return True
+                return {"element": my_button}
+        except (Exception,):
+            pass
+        try:
+            my_button = self.device.poco(type="android.widget.TextView", name="android.widget.TextView", desc="我的")
+            if my_button.exists() is True:
+                return {"element": my_button}
         except (Exception,):
             pass
         try:
             file_name = join_path([get_images_dir(), "我的.png"])
             if is_exists(file_name):
                 temp = self.device.get_cv_template(file_name=file_name, threshold=0.9)
                 pos = self.device.exists(v=temp)
                 if pos:
-                    self.device.touch(v=pos)
-                    time.sleep(0.5)
-                    pos = self.device.exists(v=temp)
-                    if pos is False:
-                        return True
+                    return {"pos": pos}
             else:
                 # temp = (975, 2214)  # Huawei Mate 20手机上对应的坐标位置，其他型号手机可能不是这个值
                 logger.warning("文件{}，没找到".format(file_name))
         except (Exception,):
             pass
         try:
             # 手机可能处于USB弹框提示点击【仅充电】
             file_name = join_path([get_images_dir(), "仅充电.png"])
             if is_exists(file_name):
                 temp = self.device.get_cv_template(file_name=file_name, threshold=0.9)
                 pos = self.device.exists(v=temp)
                 if pos:
                     self.device.touch(v=pos)
             else:
-                # temp = (975, 2214)  # Huawei Mate 20手机上对应的坐标位置，其他型号手机可能不是这个值
+                # temp = (183, 1923)  # Huawei Mate 20手机上对应的坐标位置，其他型号手机可能不是这个值
                 logger.warning("文件{}，没找到".format(file_name))
         except (Exception,):
             pass
-        return False
+        return dict()
+
+    def touch_element(self, attr: dict, sleep: int = 1) -> None:
+        """进入app后，点击【我的】"""
+        pos = attr.get("pos")
+        element = attr.get("element")
+        if pos:
+            self.device.touch(v=pos)
+        else:
+            element.click()
+        time.sleep(sleep)
 
     @LoopFindElementSubmit(loop=1, action="设置")
     def touch_settings(self):
         """我的主页，点击【设置】"""
         setting_button = self.device.poco(type="android.widget.ImageView", name="ctrip.android.view:id/a", desc="设置")
         setting_button.click()
 
@@ -161,209 +149,202 @@
     def touch_submit_logout(self):
         """退出登录弹框，点击【确定】"""
         logout_user = self.device.poco(
             type="android.widget.TextView", name="ctrip.android.view:id/a", text="确定"
         )
         logout_user.click()
 
-    @LoopExcute(loop=20, action="点击【待付款】", sleep=1)
-    def touch_unpaid(self) -> bool:
+    @LoopFindElementObject(loop=20, action="找到我的主页【待付款】", sleep=1)
+    def get_todo_unpaid(self) -> dict:
         """进入my主页后，点击【待付款】"""
         try:
             # 待付款元素定位1
             unpaid_button = self.device.poco(
                 type="android.widget.TextView", name="ctrip.android.view:id/a", text="待付款"
             )
             if unpaid_button.exists() is True:
-                unpaid_button.click()
-                time.sleep(0.5)
-                unpaid_button = self.device.poco(
-                    type="android.widget.TextView", name="ctrip.android.view:id/a", text="待付款"
-                )
-                if unpaid_button.exists() is False:
-                    return True
+                return {"element": unpaid_button}
         except (Exception,):
             pass
         try:
             # 待付款元素定位2
             unpaid_button = self.device.poco(
                 type="android.widget.TextView", name="android.widget.TextView", text="待付款"
             )
             if unpaid_button.exists() is True:
-                unpaid_button.click()
-                time.sleep(0.5)
-                unpaid_button = self.device.poco(
-                    type="android.widget.TextView", name="android.widget.TextView", text="待付款"
-                )
-                if unpaid_button.exists() is False:
-                    return True
+                return {"element": unpaid_button}
         except (Exception,):
             pass
         try:
             file_name = join_path([get_images_dir(), "我的待办_待付款.png"])
             if is_exists(file_name):
                 temp = self.device.get_cv_template(file_name=file_name, threshold=0.9)
                 pos = self.device.exists(v=temp)
                 if pos:
-                    self.device.touch(v=pos)
-                    time.sleep(0.5)
-                    pos = self.device.exists(v=temp)
-                    if pos is False:
-                        return True
+                    return {"pos": pos}
             else:
                 # temp = (417, 947)  # Huawei Mate 20手机上对应的坐标位置，其他型号手机可能不是这个值
                 logger.warning("文件{}，没找到".format(file_name))
         except (Exception,):
             pass
-        return False
+        return dict()
 
-    @LoopExcute(loop=20, action="搜索【待支付订单】", sleep=1)
-    def search_unpaid_order(self, ctrip_order_id: str) -> bool:
-        """搜索待支付的订单，这里面有2个步骤：1，定位搜索入口，并点击进入搜索界面，2.输入搜索内容"""
+    @LoopFindElementObject(loop=20, action="订单列表-待付款页查到【搜索】", sleep=1)
+    def get_unpaid_page_search_box(self) -> dict:
         try:
             search_box = self.device.poco(
                 type="android.widget.TextView", name="android.widget.TextView", text="搜索订单"
             )
             if search_box.exists() is True:
-                search_box.click()
-                time.sleep(0.5)
-                search_box = self.device.poco(
-                    type="android.widget.EditText", name="android.widget.EditText", text="输入城市名/订单号 搜索订单"
-                )
-                if search_box.exists() is True:
-                    search_box.click()
-                    search_box.set_text(ctrip_order_id)
-                    # 模拟键盘按下回车键（keyCode为66表示回车键）
-                    self.device.keyevent(keyname="66")
-                    time.sleep(1)
-                    return True
+                return {"element": search_box}
         except (Exception,):
             pass
         try:
             file_name = join_path([get_images_dir(), "搜索订单_搜索框.png"])
             if is_exists(file_name):
                 temp = self.device.get_cv_template(file_name=file_name, threshold=0.9)
                 pos = self.device.exists(v=temp)
                 if pos:
-                    self.device.touch(v=pos)
-                    time.sleep(0.5)
-                    pos = self.device.exists(v=temp)
-                    if pos is False:
-                        self.device.text(text=ctrip_order_id, enter=True)
-                        time.sleep(1)
-                        return True
+                    return {"pos": pos}
             else:
                 # temp = (289, 168)  # Huawei Mate 20手机上对应的坐标位置，其他型号手机可能不是这个值
                 logger.warning("文件{}，没找到".format(file_name))
         except (Exception,):
             pass
         try:
             file_name = join_path([get_images_dir(), "搜索_放大镜.png"])
             if is_exists(file_name):
                 temp = self.device.get_cv_template(file_name=file_name, threshold=0.9)
                 pos = self.device.exists(v=temp)
                 if pos:
-                    self.device.touch(v=pos)
-                    time.sleep(0.5)
-                    pos = self.device.exists(v=temp)
-                    if pos is False:
-                        self.device.text(text=ctrip_order_id, enter=True)
-                        time.sleep(1)
-                        return True
+                    return {"pos": pos}
             else:
                 # temp = (896, 173)  # Huawei Mate 20手机上对应的坐标位置，其他型号手机可能不是这个值
                 logger.warning("文件{}，没找到".format(file_name))
         except (Exception,):
             pass
-        return False
 
-    @LoopFindElementSubmit(loop=3, action="列表页搜索框")
-    def touch_list_page_search_box(self):
-        """进入待付款列表页，点击【搜索框】"""
-        search_box = self.device.poco(
-            type="android.widget.TextView", name="android.widget.TextView", text="搜索订单"
-        )
-        search_box.click()
+    @LoopFindElementObject(loop=20, action="搜索页查找【搜索】", sleep=1)
+    def get_search_page_search_box(self) -> dict:
+        try:
+            search_box = self.device.poco(
+                type="android.widget.EditText", name="android.widget.EditText", text="输入城市名/订单号 搜索订单"
+            )
+            if search_box.exists() is True:
+                return {"element": search_box}
+        except (Exception,):
+            pass
+        try:
+            search_box = self.device.poco(
+                type="android.widget.EditText", name="android.widget.EditText", text="输入标题关键词/订单号"
+            )
+            if search_box.exists() is True:
+                return {"element": search_box}
+        except (Exception,):
+            pass
+        return dict()
 
-    @LoopFindElementSubmit(loop=3, action="搜索页搜索框")
-    def touch_search_page_search_box(self, ctrip_order_id: str):
-        """进入搜索页，点击【搜索框】"""
-        search_box = self.device.poco(
-            type="android.widget.EditText", name="android.widget.EditText", text="输入城市名/订单号 搜索订单"
-        )
-        search_box.click()
-        search_box.set_text(ctrip_order_id)
-        # 模拟键盘按下回车键（keyCode为66表示回车键）
-        self.device.keyevent(keyname="66")
+    def search_unpaid_order(self, attr: dict, sleep: int, ctrip_order_id: str) -> bool:
+        pos = attr.get("pos")
+        element = attr.get("element")
+        if pos:
+            self.device.touch(v=pos)
+            self.device.text(text=ctrip_order_id, enter=True)
+            time.sleep(sleep)
+            return True
+        else:
+            element.click()
+            search_box = self.get_search_page_search_box()
+            if not search_box:
+                return False
+            element = search_box.get("element")
+            element.click()
+            element.set_text(ctrip_order_id)
+            # 模拟键盘按下回车键（keyCode为66表示回车键）
+            self.device.keyevent(keyname="66")
+            time.sleep(sleep)
+            return True
 
-    @LoopExcute(loop=1, action="判断订单是否为【待支付】", sleep=1)
-    def is_exist_to_payment_at_list_page(self) -> bool:
-        """检查搜索列表界面，是否存在【待支付】状态"""
+    def get_order_status_with_order_list(self) -> str:
+        """检查搜索列表界面，获取订单的状态"""
         try:
-            is_exist = self.device.poco(type="android.widget.TextView", name="android.widget.TextView", text="去支付")
-            if is_exist.exists() is True:
-                return True
-        except (Exception,):
+            unpaid_status = self.device.poco(
+                type="android.widget.TextView", name="android.widget.TextView", text="去支付"
+            )
+            if unpaid_status.exists() is True:
+                return "待支付"
+        except (PocoNoSuchNodeException, PocoTargetTimeout, Exception):
             pass
         try:
-            is_exist = self.device.poco(type="android.widget.TextView", name="android.widget.TextView", text="待支付")
-            if is_exist.exists() is True:
-                return True
+            unpaid_status = self.device.poco(
+                type="android.widget.TextView", name="android.widget.TextView", text="待支付"
+            )
+            if unpaid_status.exists() is True:
+                return "待支付"
         except (Exception,):
             pass
         try:
             file_name = join_path([get_images_dir(), "订单状态_待支付.png"])
             if is_exists(file_name):
                 temp = self.device.get_cv_template(file_name=file_name, threshold=0.9)
                 pos = self.device.exists(v=temp)
                 if pos:
-                    return True
+                    return "待支付"
             else:
                 # temp = (1033, 381)  # Huawei Mate 20手机上对应的坐标位置，其他型号手机可能不是这个值
                 logger.warning("文件{}，没找到".format(file_name))
         except (Exception,):
             pass
-        return False
-
-    def get_order_status(self) -> str:
-        """检查搜索列表界面，获取订单的状态"""
-        status = None
-        try:
-            unpaid_status = self.device.poco(
-                type="android.widget.TextView", name="android.widget.TextView", text="去支付"
-            )
-            if unpaid_status.exists() is True:
-                status = "待支付"
-        except (PocoNoSuchNodeException, PocoTargetTimeout, Exception):
-            pass
         try:
             cancel_status = self.device.poco(
                 type="android.widget.TextView", name="android.widget.TextView", text="已取消"
             )
             if cancel_status.exists() is True:
-                status = "已取消"
+                return "已取消"
         except (PocoNoSuchNodeException, PocoTargetTimeout, Exception):
             pass
         try:
             out_ticketed_status = self.device.poco(
                 type="android.widget.TextView", name="android.widget.TextView", text="已出票"
             )
             if out_ticketed_status.exists() is True:
-                status = "已出票"
+                return "已出票"
         except (PocoNoSuchNodeException, PocoTargetTimeout, Exception):
             pass
         try:
             out_ticketed_status = self.device.poco(
                 type="android.widget.TextView", name="android.widget.TextView", text="出票中"
             )
             if out_ticketed_status.exists() is True:
-                status = "出票中"
+                return "出票中"
         except (PocoNoSuchNodeException, PocoTargetTimeout, Exception):
             pass
-        return status
+        return ""
+
+    @LoopFindElementObject(loop=20, action="从搜索结果获取【去支付】按钮", sleep=1)
+    def get_to_payment_at_list_page(self) -> dict:
+        try:
+            to_payment = self.device.poco(type="android.widget.TextView", name="android.widget.TextView", text="去支付")
+            if to_payment.exists() is True:
+                return {"element": to_payment}
+        except (Exception,):
+            pass
+        try:
+            file_name = join_path([get_images_dir(), "订单状态_待支付.png"])
+            if is_exists(file_name):
+                temp = self.device.get_cv_template(file_name=file_name, threshold=0.9)
+                pos = self.device.exists(v=temp)
+                if pos:
+                    return {"pos": pos}
+            else:
+                # temp = (1033, 513)  # Huawei Mate 20手机上对应的坐标位置，其他型号手机可能不是这个值
+                logger.warning("文件{}，没找到".format(file_name))
+        except (Exception,):
+            pass
+        return dict()
 
     def is_order_detail_page(self) -> bool:
         """是否在订单详情界面"""
         flag = False
         try:
             order_detail_page_1 = self.device.poco(
                 type="android.widget.TextView", name="浮层标题", text="出行前必读"
@@ -396,75 +377,14 @@
             if order_detail_page_4.exists() is True:
                 flag = True
         except (PocoNoSuchNodeException, PocoTargetTimeout, Exception):
             pass
         return flag
 
     @SleepWait(wait_time=1)
-    def touch_go_back_to_unpaid_list_page_by_search_page(self) -> None:
-        """从搜索界面退回到【待支付】列表页"""
-        try:
-            go_back = self.device.poco(type="android.widget.TextView", name="icon_back")
-            if go_back.exists() is True:
-                go_back.click()
-                go_back.click()
-        except (PocoNoSuchNodeException, PocoTargetTimeout):
-            pass
-        except Exception as e:
-            logger.error(e)
-
-    @SleepWait(wait_time=1)
-    def touch_go_back_to_search_page_page_by_cancel_page(self) -> None:
-        """从订单撤销页返回到订单待支付列表页"""
-        try:
-            go_back = self.device.poco(
-                type="android.view.ViewGroup", name="CusHeaderView_TouchableOpacity_leftIconWrap",
-                desc="CusHeaderView_TouchableOpacity_leftIconWrap"
-            )
-            if go_back.exists() is True:
-                go_back.click()
-        except (PocoNoSuchNodeException, PocoTargetTimeout):
-            pass
-        except Exception as e:
-            logger.error(e)
-
-    @LoopExcute(loop=3, sleep=1, action="点击【去支付】")
-    def touch_to_payment_at_list_page(self) -> bool:
-        """进入待付款列表页，点击【去支付】"""
-        try:
-            to_payment = self.device.poco(type="android.widget.TextView", name="android.widget.TextView", text="去支付")
-            if to_payment.exists() is True:
-                to_payment.click()
-                time.sleep(0.5)
-                to_payment = self.device.poco(
-                    type="android.widget.TextView", name="android.widget.TextView", text="去支付"
-                )
-                if to_payment.exists() is False:
-                    return True
-        except (Exception,):
-            pass
-        try:
-            file_name = join_path([get_images_dir(), "订单状态_待支付.png"])
-            if is_exists(file_name):
-                temp = self.device.get_cv_template(file_name=file_name, threshold=0.9)
-                pos = self.device.exists(v=temp)
-                if pos:
-                    self.device.touch(v=pos)
-                    time.sleep(0.5)
-                    pos = self.device.exists(v=temp)
-                    if pos is False:
-                        return True
-            else:
-                # temp = (1033, 513)  # Huawei Mate 20手机上对应的坐标位置，其他型号手机可能不是这个值
-                logger.warning("文件{}，没找到".format(file_name))
-        except (Exception,):
-            pass
-        return False
-
-    @SleepWait(wait_time=1)
     def is_cancel_order(self, out_total_price: str, amount_loss_limit: str, profit_cap: str, passenger_number: int,
                         discount_amount: str = None) -> tuple:
         """在订单详情页，判断是否需要取消订单"""
         flag = False
         remark = None
         try:
             is_cancel = self.device.poco(
@@ -610,453 +530,41 @@
             else:
                 # temp = (466, 173)  # Huawei Mate 20手机上对应的坐标位置，其他型号手机可能不是这个值
                 logger.warning("文件{}，没找到".format(file_name))
         except (Exception,):
             pass
         return ""
 
-    @LoopExcute(action="订单详情页点击【去支付】", loop=10, sleep=1)
-    def touch_to_payment_at_order_detail(self):
-        """在订单详情页，点击【去支付】"""
+    @LoopFindElementObject(loop=20, action="从订单详情页【去支付】按钮", sleep=1)
+    def get_to_payment_in_order_detail(self):
         try:
             to_payment = self.device.poco(type="android.widget.TextView", name="pcardLimit_Text_去支付", text="去支付")
             if to_payment.exists() is True:
-                to_payment.click()
-                time.sleep(3)
-                to_payment = self.device.poco(
-                    type="android.widget.TextView", name="pcardLimit_Text_去支付", text="去支付"
-                )
-                if to_payment.exists() is False:
-                    return True
+                return {"element": to_payment}
         except (Exception,):
             pass
         try:
             to_payment = self.device.poco(type="android.widget.TextView", name="android.widget.TextView", text="去支付")
             if to_payment.exists() is True:
-                to_payment.click()
-                time.sleep(3)
-                to_payment = self.device.poco(
-                    type="android.widget.TextView", name="android.widget.TextView", text="去支付"
-                )
-                if to_payment.exists() is False:
-                    return True
+                return {"element": to_payment}
         except (Exception,):
             pass
         try:
             file_name = join_path([get_images_dir(), "订单详情_去支付.png"])
             if is_exists(file_name):
                 temp = self.device.get_cv_template(file_name=file_name, threshold=0.9)
                 pos = self.device.exists(v=temp)
                 if pos:
-                    self.device.touch(v=pos)
-                    time.sleep(3)
-                    pos = self.device.exists(v=temp)
-                    if pos is False:
-                        return True
+                    return {"pos": pos}
             else:
                 # temp = (873, 440)  # Huawei Mate 20手机上对应的坐标位置，其他型号手机可能不是这个值
                 logger.warning("文件{}，没找到".format(file_name))
         except (Exception,):
             pass
-
-    @SleepWait(wait_time=1)
-    def touch_flight_ticket(self) -> None:
-        """进入app后，点击【首页】，点击【机票】"""
-        file_name = join_path([get_images_dir(), "机票.png"])
-        if is_exists(file_name):
-            temp = self.device.get_cv_template(file_name=file_name)
-        else:
-            temp = (445, 560)  # LG g7手机上对应的坐标位置，其他型号手机可能不是这个值
-        self.device.touch(v=temp)
-
-    @SleepWait(wait_time=1)
-    def touch_special_flight_ticket(self) -> None:
-        """进入app后，点击【首页】，点击【机票】，点击【特价机票】"""
-        file_name = join_path([get_images_dir(), "特价机票.png"])
-        if is_exists(file_name):
-            temp = self.device.get_cv_template(file_name=file_name)
-        else:
-            temp = (517, 592)  # LG g7手机上对应的坐标位置，其他型号手机可能不是这个值
-        self.device.touch(v=temp)
-
-    @SleepWait(wait_time=1)
-    def select_departure_city(self) -> None:
-        departure_city = self.device.get_po_extend(
-            type="android.widget.TextView",
-            name="ctrip.android.view:id/a",
-            textMatches_inner=r"\S+",
-            global_num=0,
-            local_num=2,
-        )[0]
-        departure_city.click()
-
-    @SleepWait(wait_time=3)
-    def enter_search_value(self, search_value: str) -> None:
-        search_box = self.device.poco(type="android.widget.EditText")
-        search_box.click()
-        search_box.set_text(search_value)
-
-    @SleepWait(wait_time=5)
-    def select_search_result_first_city(self, select_value: str):
-        search_result = self.device.get_po_extend(
-            type="android.widget.TextView",
-            name="ctrip.android.view:id/a",
-            textMatches_inner=".* {} .*".format(select_value),
-            global_num=0,
-            local_num=2,
-            touchable=False
-        )[0]
-        value = search_result.get_text().strip()
-        search_result.click()
-        logger.info("从搜索结果中，选择<{}>这条数据.".format(value))
-
-    @SleepWait(wait_time=3)
-    def sumbit_search_result(self):
-        """选择城市后，需要点击【确认】按钮"""
-        """
-        file_name = join_path([get_images_dir(), "搜索确认.png"])
-        if is_exists(file_name):
-            template = self.device.get_cv_template(file_name=file_name)
-            result = self.device.find_all(v=template)
-            temp = result[0].get("result")
-        else:
-            temp = (1273, 624) # LG g7手机上对应的坐标位置，其他型号手机可能不是这个值
-        self.device.adb_touch(v=temp)
-        """
-        search_result = self.device.get_po_extend(
-            type="android.widget.Button",
-            name="ctrip.android.view:id/a",
-            text="确认",
-            global_num=0,
-            local_num=2,
-            touchable=True,
-        )[0]
-        search_result.click()
-
-    @SleepWait(wait_time=1)
-    def select_arrive_city(self) -> None:
-        arrive_city = self.device.get_po_extend(
-            type="android.widget.TextView",
-            name="ctrip.android.view:id/a",
-            textMatches_inner=r"\S+",
-            global_num=0,
-            local_num=4,
-        )[0]
-        arrive_city.click()
-
-    @SleepWait(wait_time=1)
-    def select_trip_date(self) -> None:
-        trip_date = self.device.get_po_extend(
-            type="android.widget.TextView",
-            name="ctrip.android.view:id/a",
-            textMatches_inner="^出发.*",
-            global_num=0,
-            local_num=9,
-        )[0]
-        trip_date.click()
-
-    @SleepWait(wait_time=1)
-    def select_trip_expect_month(self, date_str: str) -> None:
-        _, trip_month, _ = get_trip_year_month_day(date_str=date_str)
-        top_month_area = self.device.get_po_extend(
-            type="android.widget.TextView",
-            name="ctrip.android.view:id/a",
-            text=trip_month,
-            touchable=False,
-            global_num=0,
-            local_num=2,
-        )[0]
-        top_month_area.click()
-
-    @SleepWait(wait_time=2)
-    def select_trip_expect_day(self, date_str: str) -> None:
-        _, _, trip_day = get_trip_year_month_day(date_str=date_str)
-        day_str = "{}_red".format(trip_day) if is_public_holiday(
-            date_str=date_str) else "{}_blue".format(trip_day)
-        file_name = join_path([get_images_dir(), "{}.png".format(day_str)])
-        logger.info("需要识别日历中的日期文件是：{}".format(file_name))
-        if is_exists(file_name):
-            # threshold 提高识别灵敏度，灵敏度太低，容易将相似的结果匹配出来
-            temp = self.device.get_cv_template(
-                file_name=file_name, threshold=0.9)
-            find_results = self.device.find_all(v=temp)
-            if isinstance(find_results, t.List) and len(find_results) > 0:
-                sorted_list = sorted(find_results, key=lambda x: (
-                    x['result'][1], x['result'][0]))
-                temp = sorted_list[0].get("result")
-            else:
-                raise ValueError(
-                    "According to the image file <{}>, no corresponding element was found".format(file_name))
-        else:
-            raise ValueError("<{}> file does not exist".format(file_name))
-        self.device.touch(v=temp)
-
-    @SleepWait(wait_time=1)
-    def touch_only_query_some_day(self) -> None:
-        """
-        点击 【预计出发日期】 界面的 【仅查询当天】 按钮
-        """
-        only_query_some_day = self.device.get_po_extend(
-            type="android.widget.Button",
-            name="ctrip.android.view:id/a",
-            text="仅查询当天",
-            global_num=0,
-            local_num=5,
-        )[0]
-        only_query_some_day.click()
-
-    @SleepWait(wait_time=8)
-    def touch_query_special(self) -> None:
-        """
-        特价机票界面，点击【查询特价】
-        """
-        query_special_flight = self.device.get_po_extend(
-            type="android.widget.Button",
-            name="ctrip.android.view:id/a",
-            text="查询特价",
-            global_num=0,
-            local_num=5,
-            touchable=True,
-        )[0]
-        query_special_flight.click()
-
-    def is_exist_flight_in_screen(self, flight: str) -> bool:
-        """
-        检索需要购买的航班是否出现在初始的屏幕中
-        """
-        logger.info("判断航班<{}>机票信息是否在初始列表当中...".format(flight))
-        in_screen = self.device.get_po(
-            type="android.widget.TextView", name="第{}航班航司信息".format(flight))
-        if in_screen.exists():
-            return True
-        else:
-            return False
-
-    def touch_flight_inland_single_list_filter(self) -> None:
-        po = self.device.get_po(type="android.widget.TextView", name="筛选")
-        if po.exists():
-            # 说明筛选入口在底部
-            logger.info("查询到的航班数量不多，筛选的按钮在UI的底部。")
-            self.__touch_flight_inland_single_list_bottom_filter()
-        else:
-            self.__touch_flight_inland_single_list_top_filter()
-
-    @SleepWait(wait_time=1)
-    def touch_clear_filter(self) -> None:
-        """
-        点击【清空】，防止缓存数据，干扰配置过滤条件，当然需要判断，【清空】按钮，是否为激活状态，未激活的情况下，按钮是灰色，无法点击
-        """
-        clear_button = self.device.get_po(
-            type="android.view.ViewGroup", name="筛选清空按钮"
-        )[0]
-        clear_button_attr = get_ui_object_proxy_attr(
-            ui_object_proxy=clear_button)
-        is_enabled = clear_button_attr.get("enabled")
-        if is_enabled is True:
-            clear_text = self.device.get_po_extend(
-                type="android.widget.TextView",
-                name="android.widget.TextView",
-                text="清空",
-                global_num=0,
-                local_num=1,
-                touchable=False,
-            )[0]
-            clear_text.click()
-
-    @SleepWait(wait_time=1)
-    def __touch_flight_inland_single_list_top_filter(self) -> None:
-        """
-        航线特价机票查询列表，点击顶部的【筛选】
-        """
-        filter1 = self.device.get_po_extend(
-            type="android.widget.TextView",
-            name="android.widget.TextView",
-            text="筛选",
-            global_num=0,
-            local_num=1,
-            touchable=False,
-        )[0]
-        filter1.click()
-
-    @SleepWait(wait_time=1)
-    def __touch_flight_inland_single_list_bottom_filter(self) -> None:
-        """
-        航线特价机票查询列表，点击底部的【筛选】
-        """
-        filter1 = self.device.get_po_extend(
-            type="android.widget.TextView",
-            name="筛选",
-            text="筛选",
-            global_num=0,
-            local_num=2,
-            touchable=False,
-        )[0]
-        filter1.click()
-
-    @SleepWait(wait_time=1)
-    def touch_filter_departure_time(self) -> None:
-        """
-        航班列表底部的筛选界面，点击【起飞时间】
-        """
-        departure_time = self.device.get_po_extend(
-            type="android.widget.TextView",
-            name="起飞时间",
-            text="起飞时间",
-            global_num=0,
-            local_num=2,
-            touchable=False,
-        )[0]
-        departure_time.click()
-
-    @SleepWait(wait_time=1)
-    def select_filter_departure_time_area(self, date_str: str) -> None:
-        """
-        选择筛选条件中的起飞时间区域，00:00~06:00,06:00~12:00,12:00~18:00,18:00~24:00
-        """
-        time_area_str = get_datetime_area(date_str=date_str)
-        time_area = self.device.get_po_extend(
-            type="android.widget.TextView",
-            # name="{}筛选控件".format(time_area_str),
-            text=time_area_str,
-            global_num=0,
-            local_num=1,
-            touchable=False,
-        )[0]
-        time_area.click()
-
-    @SleepWait(wait_time=1)
-    def touch_filter_airline(self) -> None:
-        """
-        航班列表底部的筛选界面，点击【航空公司】
-        """
-        airline = self.device.get_po_extend(
-            type="android.widget.TextView",
-            name="航空公司",
-            text="航空公司",
-            global_num=0,
-            local_num=2,
-            touchable=False,
-        )[0]
-        airline.click()
-
-    @SleepWait(wait_time=1)
-    def select_filter_airline_company(self, ac: str) -> None:
-        """
-        选择筛选条件中的航空公司
-        """
-        airline_company = self.device.get_po_extend(
-            type="android.widget.TextView",
-            name="筛选按钮{}".format(ac),
-            text=ac,
-            global_num=0,
-            local_num=2,
-            touchable=False,
-        )[0]
-        airline_company.click()
-
-    @SleepWait(wait_time=8)
-    def touch_filter_submit_button(self) -> None:
-        """
-        确认筛选条件
-        """
-        submit_button = self.device.get_po_extend(
-            type="android.widget.TextView",
-            name="筛选确定按钮文案",
-            global_num=0,
-            local_num=1,
-            touchable=False,
-        )[0]
-        submit_button.click()
-
-    @SleepWait(wait_time=5)
-    def select_special_flight(self, flight: str) -> None:
-        """
-        从特价机票列表中选择本次订单的航班
-        """
-        desc = "第{}航班航司信息".format(flight)
-        special_flight = self.device.get_po(
-            type="android.widget.TextView", name=desc)
-        if special_flight.exists():
-            abs_position = self.device.get_abs_position(element=special_flight)
-            # special_flight.click()
-            logger.info("选择：{}".format(desc))
-            self.device.touch((abs_position[0], abs_position[1] - 200))
-        else:
-            raise ValueError("当前页面没有找到", desc)
-
-    @SleepWait(wait_time=1)
-    def get_special_flight_amount(self) -> Decimal:
-        """
-        检索航班经济舱的第二条数据的金额
-        """
-        lowerest_amount_po = self.device.get_po(
-            type="android.widget.TextView", name="第2个政策成人价格金额"
-        )[0]
-        ui_object_proxy_attr = get_ui_object_proxy_attr(
-            ui_object_proxy=lowerest_amount_po)
-        text = ui_object_proxy_attr.get("text")
-        logger.info("获取到的机票最低价为：{}".format(text))
-        # 9999999999.9999999999 表示金额无限大，仅限于作为后续的比较逻辑默认值
-        return Decimal(text) if isinstance(text, str) and text.isdigit() else 9999999999.9999999999
-
-    def is_direct_booking(self) -> True:
-        """
-        在经济舱航班列表中，存在某些航班，没有【选购】按钮，点击【订】直接进入下单界面，相当于少了一次点击
-        """
-        booking = self.device.get_po(
-            type="android.widget.TextView", name="btn_book_2预订按钮", text="订")
-        if booking.exists():
-            return True
-        else:
-            return False
-
-    @SleepWait(wait_time=1)
-    def touch_direct_booking_button(self) -> None:
-        """
-        在经济舱航班列表中，存在某些航班，点击【订】直接进入下单界面
-        """
-        direct_booking_button = self.device.get_po_extend(
-            type="android.widget.TextView",
-            name="btn_book_2预订按钮",
-            text="订",
-            global_num=0,
-            local_num=2,
-            touchable=False,
-        )[0]
-        direct_booking_button.click()
-
-    @SleepWait(wait_time=1)
-    def touch_booking_the_second_button(self) -> None:
-        """
-        点击航班经济舱第二条数据中的【选购】
-        """
-        the_second_button = self.device.get_po_extend(
-            type="android.widget.TextView",
-            name="drop_book_2预订按钮",
-            text="选购",
-            global_num=0,
-            local_num=2,
-            touchable=False,
-        )[0]
-        the_second_button.click()
-
-    @SleepWait(wait_time=5)
-    def touch_ordinary_booking_button(self) -> None:
-        """
-        点击航班经济舱第二条数据中的【普通预订】
-        """
-        ordinary_booking_button = self.device.get_po_extend(
-            type="android.widget.TextView",
-            name="第2个政策选购第7个X产品预订按钮",
-            text="订",
-            global_num=0,
-            local_num=1,
-            touchable=False,
-        )[0]
-        ordinary_booking_button.click()
+        return dict()
 
     def is_need_login_with_my_page(self) -> bool:
         flag = False
         try:
             my_login = self.device.get_po(
                 type="android.widget.Button", name="ctrip.android.view:id/a", text="登录/注册"
             )
@@ -1122,322 +630,14 @@
     @LoopFindElementSubmit(loop=1, action="登录")
     def touch_login(self):
         """点击【登录】"""
         login_poco = self.device.get_po(type="android.widget.TextView", name="ctrip.android.view:id/a",
                                         text="登录")
         login_poco.click()
 
-    @LoopFindElement(loop=5)
-    # @SleepWait(wait_time=3)
-    def touch_more_passengers_button(self) -> None:
-        """
-        点击【更多乘机人】按钮
-        """
-        add_passenger_button = self.device.get_po_extend(
-            type="android.widget.TextView",
-            name="新增乘机人按钮icon",
-            global_num=0,
-            local_num=1,
-            touchable=False,
-        )[0]
-        add_passenger_button.click()
-
-    @LoopFindElement(loop=5)
-    # @SleepWait(wait_time=1)
-    def touch_add_passengers_button(self) -> None:
-        """
-        点击【新增乘机人】按钮
-        """
-        add_passenger_button = self.device.get_po_extend(
-            type="android.widget.TextView",
-            name="乘机人列表新增乘机人文案",
-            text="新增乘机人",
-            global_num=0,
-            local_num=2,
-            touchable=False,
-        )[0]
-        add_passenger_button.click()
-
-    @SleepWait(wait_time=1)
-    def enter_passenger_username(self, passenger: str) -> None:
-        """
-        录入乘客姓名
-        """
-        passenger_username = self.device.get_po_extend(
-            type="android.widget.EditText",
-            name="新增乘机人姓名框文案",
-            text="与乘机证件一致",
-            global_num=0,
-            local_num=1,
-            touchable=True,
-        )[0]
-        passenger_username.click()
-        passenger_username.set_text(passenger)
-
-    @SleepWait(wait_time=1)
-    def touch_passenger_card_type(self) -> None:
-        """
-        点击【证件类型】
-        """
-        passenger_card_type = self.device.get_po(
-            type="android.widget.TextView", name="新增乘机人证件类型文案")
-        passenger_card_type.click()
-        logger.info("点击【证件类型】")
-
-    @SleepWait(wait_time=1)
-    def select_passenger_card_type(self, card_type: str) -> None:
-        """
-        选择合适的证件类型
-        """
-        passenger_card_type = self.device.get_po(
-            type="android.widget.TextView", text=card_type)
-        passenger_card_type.click()
-        logger.info("选择【{}】".format(card_type))
-
-    @SleepWait(wait_time=1)
-    def enter_passenger_card_id(self, card_id: str) -> None:
-        """
-        录入乘客证件号码
-        """
-        passenger_card_id = self.device.get_po_extend(
-            type="android.widget.EditText",
-            name="新增乘机人证件号码文案",
-            text="请输入证件号",
-            global_num=0,
-            local_num=1,
-            touchable=True,
-        )[0]
-        passenger_card_id.click()
-        passenger_card_id.set_text(card_id)
-
-    @SleepWait(wait_time=1)
-    def enter_passenger_phone_number(self, phone: str) -> None:
-        """
-        录入乘客手机号码
-        """
-        passenger_phone_number = self.device.get_po_extend(
-            type="android.widget.EditText",
-            name="新增乘机人手机框文案",
-            global_num=0,
-            local_num=1,
-            touchable=True,
-        )[0]
-        passenger_phone_number.click()
-        passenger_phone_number.set_text(phone)
-
-    @SleepWait(wait_time=1)
-    def submit_passenger_info(self) -> None:
-        """
-        点击【完成】按钮，提交乘客信息
-        """
-        file_name = join_path([get_images_dir(), "键盘隐藏.png"])
-        self.device.hide_keyword(file_name=file_name)
-        passenger_info = self.device.get_po_extend(
-            type="android.widget.TextView",
-            name="新增乘机人完成按钮",
-            text="完成",
-            global_num=0,
-            local_num=1,
-            touchable=False,
-        )[0]
-        passenger_info.click()
-
-    @SleepWait(wait_time=3)
-    def submit_passenger_info_confirm(self) -> None:
-        """
-        点击【确认无误】按钮，提交乘客信息
-        """
-        """
-        passenger_info_confirm = self.device.get_po_extend(
-            type="android.view.ViewGroup",
-            name="android.view.ViewGroup",
-            global_num=0,
-            local_num=5,
-            touchable=True,
-        )[0]
-        passenger_info_confirm.click()
-        """
-        file_name = join_path([get_images_dir(), "乘机人信息_确认无误.png"])
-        if is_exists(file_name):
-            temp = self.device.get_cv_template(file_name=file_name)
-        else:
-            temp = (723, 1413)  # LG g7手机上对应的坐标位置，其他型号手机可能不是这个值
-        self.device.touch(v=temp)
-
-    @LoopFindElement(loop=5)
-    # @SleepWait(wait_time=1)
-    def add_passenger(self, passenger: str) -> None:
-        """
-        点击【确定】按钮，添加乘客
-        """
-        passenger_po = self.device.get_po_extend(
-            type="android.widget.TextView",
-            name="乘机人列表确定按钮",
-            text="确定",
-            global_num=0,
-            local_num=1,
-            touchable=False,
-        )[0]
-        passenger_po.click()
-        logger.info("预定特价机票，已添加乘客: <{}>".format(passenger))
-
-    @SleepWait(wait_time=1)
-    def select_insecure(self) -> None:
-        """
-        选择【无保障】航意航延组合险
-        """
-        # 先滑屏
-        self.device.quick_slide_screen(duration=0.5)
-        insecure = self.device.get_po_extend(
-            type="android.widget.TextView",
-            name="航意航延组合险无保障标题",
-            text="无保障",
-            global_num=0,
-            local_num=2,
-            touchable=False,
-        )[0]
-        insecure.click()
-
-    @SleepWait(wait_time=5)
-    def touch_fill_order_next_step(self) -> None:
-        """
-        填订单界面，点击【下一步】
-        """
-        next_step = self.device.get_po_extend(
-            type="android.widget.TextView",
-            name="下一步",
-            text="下一步",
-            global_num=0,
-            local_num=2,
-            touchable=False,
-        )[0]
-        next_step.click()
-
-    @SleepWait(wait_time=1)
-    def is_duplicate_order(self) -> str:
-        """
-        如果用户已经下单，系统会有弹框提示，下单重复了
-        """
-        duplicate_order_1 = self.device.get_po(
-            type="android.widget.TextView", text="我知道了")
-        duplicate_order_2 = self.device.get_po(type="android.widget.TextView", name="android.widget.TextView",
-                                               text="继续预订当前航班")
-        duplicate_order_3 = self.device.get_po(
-            type="android.widget.TextView", name="重复订单标题", text="行程冲突提示")
-        if duplicate_order_1.exists():
-            conflict_prompt = self.device.get_po_extend(
-                type="android.widget.TextView",
-                name="重复订单提示文案",
-                global_num=0,
-                local_num=2,
-                touchable=False,
-            )[0]
-            conflict_prompt_str = get_ui_object_proxy_attr(
-                ui_object_proxy=conflict_prompt).get("text")
-            duplicate_order_1.click()
-            return conflict_prompt_str
-        elif duplicate_order_2.exists():
-            conflict_prompt = self.device.get_po_extend(
-                type="android.widget.TextView",
-                name="android.widget.TextView",
-                global_num=0,
-                local_num=1,
-                touchable=False,
-            )[0]
-            conflict_prompt_str = get_ui_object_proxy_attr(
-                ui_object_proxy=conflict_prompt).get("text")
-            duplicate_order_2.click()
-            return conflict_prompt_str
-        elif duplicate_order_3.exists():
-            conflict_prompt = self.device.get_po_extend(
-                type="android.widget.TextView",
-                name="重复订单提示文案",
-                global_num=0,
-                local_num=3,
-                touchable=False,
-            )[0]
-            conflict_prompt_str = get_ui_object_proxy_attr(
-                ui_object_proxy=conflict_prompt).get("text")
-            self.device.touch((400, 500))  # 点击一个随机坐标，尽量靠近上半屏，相当于点击空白处，隐藏掉提示框
-            return conflict_prompt_str
-        else:
-            return ""
-
-    @SleepWait(wait_time=1)
-    def touch_select_service_no_need(self) -> None:
-        """
-        选服务界面，点击【不用了，谢谢】
-        """
-        try:
-            no_need = self.device.get_po_extend(
-                type="android.widget.TextView",
-                name="android.widget.TextView",
-                text="不用了，谢谢",
-                global_num=0,
-                local_num=1,
-                touchable=False,
-            )[0]
-            no_need.click()
-        except (PocoNoSuchNodeException, Exception):
-            pass
-
-    @SleepWait(wait_time=1)
-    def touch_to_payment(self) -> None:
-        """
-        选服务界面，点击【去支付】
-        """
-        try:
-            to_payment = self.device.get_po_extend(
-                type="android.widget.TextView",
-                name="去支付",
-                text="去支付",
-                global_num=0,
-                local_num=2,
-                touchable=False,
-            )[0]
-            to_payment.click()
-        except (PocoNoSuchNodeException, Exception):
-            pass
-
-    @SleepWait(wait_time=3)
-    def touch_insure_no(self) -> None:
-        """
-        选航空意外险界面，点击【否】
-        """
-        try:
-            no = self.device.get_po_extend(
-                type="android.widget.TextView",
-                name="android.widget.TextView",
-                text="否",
-                global_num=0,
-                local_num=1,
-                touchable=False,
-            )[0]
-            no.click()
-        except (PocoNoSuchNodeException, Exception):
-            pass
-
-    @SleepWait(wait_time=5)
-    def touch_read_agree(self) -> None:
-        """
-        我已阅读并同意，点击【同意并支付】
-        """
-        try:
-            agree = self.device.get_po_extend(
-                type="android.widget.TextView",
-                name="去支付",
-                text="同意并支付",
-                global_num=0,
-                local_num=2,
-                touchable=False,
-            )[0]
-            agree.click()
-        except (PocoNoSuchNodeException, Exception):
-            pass
-
     @SleepWait(wait_time=1)
     def touch_payment_method(self) -> None:
         """点击【换卡支付，支持境外卡】"""
         try:
             payment_method = self.device.get_po(
                 type="android.widget.TextView",
                 name="android.widget.TextView",
@@ -1447,21 +647,24 @@
             logger.info("在安全收银台界面，点击选择【换卡支付，支持境外卡】")
         except (PocoNoSuchNodeException, Exception):
             logger.warning("没有出现收银台，可以直接选择银行卡支付.")
 
     @SleepWait(wait_time=1)
     def select_payment_method(self, payment_method: str) -> None:
         """选择【xxxy银行储蓄卡(xxxx)】"""
-        method = self.device.get_po(
-            type="android.widget.TextView",
-            name="android.widget.TextView",
-            text=payment_method
-        )
-        method.click()
-        logger.info("点击选择【{}】".format(payment_method))
+        try:
+            method = self.device.get_po(
+                type="android.widget.TextView",
+                name="android.widget.TextView",
+                text=payment_method
+            )
+            method.click()
+            logger.info("点击选择【{}】".format(payment_method))
+        except (Exception,):
+            pass
 
     def select_more_payment(self) -> bool:
         """
         当【同意并支付】后，特殊情况下，会出现支付小弹框，这个时候需要先判断是否存在小框，如果存在，则切换到通用支付选择界面
         """
         flag = False
         # 这个地方容易卡卡住，采用透底的方案执行该逻辑
@@ -1508,15 +711,15 @@
                         pass
             except (Exception,):
                 pass
             # 3. 检测到小弹框， 图像识别定位特征是：【更多付款方式】
             try:
                 file_name = join_path([get_images_dir(), "更多付款方式.png"])
                 if is_exists(file_name):
-                    temp = self.device.get_cv_template(file_name=file_name)
+                    temp = self.device.get_cv_template(file_name=file_name, threshold=0.9)
                     if temp:
                         logger.warning("图像识别方式检测到有小弹框，需要点击【更多付款方式】")
                         self.device.touch(v=temp)
                         time.sleep(1)
                         temp_inner = self.device.get_cv_template(file_name=file_name)
                         if not temp_inner:
                             flag = True
@@ -1775,125 +978,7 @@
         payment_complete_button = self.device.poco(
             type="android.widget.TextView",
             name="android.widget.TextView",
             text="完成"
         )
         payment_complete_button.click()
         logger.warning("点击支付成功界面的【完成】按钮.")
-
-    @SleepWait(wait_time=1)
-    def close_coupon_dialog(self) -> None:
-        """支付完成后，会有一个优惠卷弹框，需要关闭"""
-        try:
-            coupon_dialog = self.device.get_po(
-                type="android.view.ViewGroup", name="领券弹窗关闭按钮")
-            if coupon_dialog.exists():
-                coupon_dialog.click()
-        except (PocoNoSuchNodeException, Exception):
-            logger.warning("没有出现领券弹窗关闭按钮.")
-
-    @SleepWait(wait_time=1)
-    def expand_order_detail(self) -> None:
-        """展开【详情/首页】"""
-        try:
-            file_name = join_path([get_images_dir(), "完成后的订单详情.png"])
-            if is_exists(file_name):
-                temp = self.device.get_cv_template(file_name=file_name)
-            else:
-                temp = (902, 202)  # LG g7手机上对应的坐标位置，其他型号手机可能不是这个值
-            self.device.touch(v=temp)
-            logger.info("展开【详情/首页】，接下来可以点击【查订单/开发票】")
-        except Exception as e:
-            logger.error("展开【详情/首页】元素失败，原因：{}".format(str(e)))
-
-    @SleepWait(wait_time=5)
-    def touch_order_detail(self) -> None:
-        """点击【查订单/开发票】，进入订单详情界面"""
-        try:
-            order_detail = self.device.get_po(type="android.widget.TextView", name="android.widget.TextView",
-                                              text="查订单/开发票")
-            order_detail.click()
-            logger.info("点击【查订单/开发票】，进入订单详情界面")
-        except Exception as e:
-            logger.error("点击点击【查订单/开发票】失败，原因：{}".format(str(e)))
-
-    @SleepWait(wait_time=2)
-    def close_important_trip_guidelines(self) -> None:
-        """关闭出行前必读"""
-        try:
-            read_me = self.device.get_po(type="android.widget.TextView", name="浮层标题", text="出行前必读")
-            if read_me.exists() is True:
-                # 说明出现了出行前必读，需要关闭该窗口
-                file_name = join_path([get_images_dir(), "关闭.png"])
-                if is_exists(file_name):
-                    temp = self.device.get_cv_template(file_name=file_name)
-                else:
-                    temp = (76, 367)  # Huawei Mate 20手机上对应的坐标位置，其他型号手机可能不是这个值
-                self.device.touch(v=temp)
-                logger.info("【出行前必读】小窗口，已关闭.")
-            else:
-                logger.info("【出行前必读】小窗口，不可点击")
-        except (PocoNoSuchNodeException, Exception):
-            logger.warning("没有检测到【出现前必读】小窗口弹出，可以直接进行下面的操作.")
-
-    @SleepWait(wait_time=1)
-    def touch_order_with_finish_button(self) -> None:
-        """点击支付成功界面的【完成】按钮"""
-        finish_button = self.device.get_po_extend(
-            type="android.widget.TextView",
-            name="android.widget.TextView",
-            text="完成",
-            global_num=0,
-            local_num=1,
-            touchable=False,
-        )[0]
-        logger.info("点击【完成】按钮, 关闭流程.")
-        finish_button.click()
-
-    @SleepWait(wait_time=1)
-    def get_flight_ticket_with_order_id(self) -> str:
-        """获取机票订单的id"""
-        order_id = None
-        try:
-            poco = self.device.get_po(type="android.widget.TextView", name="pricePolicy_Text_订单号")
-            order_id = poco.get_text().split("：")[-1].strip()
-        except Exception as e:
-            logger.error("获取携程订单id失败，原因：{}".format(str(e)))
-        return order_id
-
-    @SleepWait(wait_time=1)
-    def get_flight_ticket_with_itinerary_id(self) -> str:
-        """获取机票中乘客的行程单号，可能在出票中，那么就先结束流程，等待人工回填行程单号"""
-        # 滑动屏幕三次
-        for i in range(3):
-            self.device.quick_slide_screen()
-        itinerary_id = None
-        try:
-            poco = (
-                self.device.poco("android.widget.FrameLayout")
-                .offspring("android:id/content")
-                .child("ctrip.android.view:id/a")
-                .child("ctrip.android.view:id/a")
-                .offspring("android.widget.LinearLayout")
-                .offspring("android.widget.FrameLayout")
-                .child("android.view.ViewGroup")
-                .child("android.view.ViewGroup")
-                .child("android.view.ViewGroup")
-                .child("android.view.ViewGroup")
-                .child("android.view.ViewGroup")[1]
-                .offspring("PullRefreshScrollView_ScrollView")
-                .child("android.view.ViewGroup")
-                .child("android.view.ViewGroup")
-                .offspring("@contactInfo")
-                .offspring("contactInfo_Text_票号")[0]
-            )
-            if poco.exists() is True:
-                itinerary_id = poco.get_text().split("：")[-1].strip()
-        except (PocoNoSuchNodeException, Exception):
-            logger.warning("出票中，没有查找到行程单.")
-        return itinerary_id
-
-    """
-    # 为了调式方便，暂时注释
-    def __del__(self) -> None:
-        self.stop()
-    """
```

### Comparing `ctrip-app-ui-0.4.8/capp_ui/fee.py` & `ctrip-app-ui-0.4.9/capp_ui/fee.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.4.8/capp_ui/libs.py` & `ctrip-app-ui-0.4.9/capp_ui/libs.py`

 * *Files 16% similar despite different names*

```diff
@@ -143,7 +143,30 @@
                     break
                 sleep(self.sleep)
             if flag is False and self.loop > 2:
                 logger.warning("{}次尝试{}都失败".format(self.loop, self.action))
             return flag
 
         return wrapper
+
+
+class LoopFindElementObject(object):
+
+    def __init__(self, action: str, loop: int = 1, sleep: int = 1) -> None:
+        self.loop = loop
+        self.sleep = sleep
+        self.action = action
+
+    def __call__(self, func: Callable) -> Any:
+        def wrapper(*args, **kwargs) -> dict:
+            for i in range(self.loop):
+                if i > 0:
+                    logger.warning("尝试第{}次{}".format(i, self.action))
+                flag = func(*args, **kwargs)
+                if flag:
+                    break
+                sleep(self.sleep)
+            if self.loop > 2:
+                logger.warning("{}次尝试{}都失败".format(self.loop, self.action))
+            return dict()
+
+        return wrapper
```

### Comparing `ctrip-app-ui-0.4.8/capp_ui/mobile_terminals.py` & `ctrip-app-ui-0.4.9/capp_ui/mobile_terminals.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.4.8/capp_ui/platforms.py` & `ctrip-app-ui-0.4.9/capp_ui/platforms.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.4.8/capp_ui/test.py` & `ctrip-app-ui-0.4.9/capp_ui/test.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.4.8/capp_ui/utils.py` & `ctrip-app-ui-0.4.9/capp_ui/utils.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.4.8/capp_ui/validators.py` & `ctrip-app-ui-0.4.9/capp_ui/validators.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.4.8/setup.py` & `ctrip-app-ui-0.4.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 # Copyright ©2011-2024. Hunan xxxxxxx Company limited. All rights reserved.
 # ---------------------------------------------------------------------------------------------------------
 """
 from setuptools import setup, find_packages
 
 setup(
     name='ctrip-app-ui',
-    version='0.4.8',
+    version='0.4.9',
     description='This is my ctrip app ui package',
     long_description='This is my ctrip app ui package',
     author='ckf10000',
     author_email='ckf10000@sina.com',
     url='https://github.com/ckf10000/ctrip-app-ui',
     packages=find_packages(),
     install_requires=[
```

