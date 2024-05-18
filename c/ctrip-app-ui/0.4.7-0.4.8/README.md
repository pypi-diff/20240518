# Comparing `tmp/ctrip-app-ui-0.4.7.tar.gz` & `tmp/ctrip-app-ui-0.4.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ctrip-app-ui-0.4.7.tar", last modified: Tue May 14 11:51:12 2024, max compression
+gzip compressed data, was "ctrip-app-ui-0.4.8.tar", last modified: Sat May 18 08:54:53 2024, max compression
```

## Comparing `ctrip-app-ui-0.4.7.tar` & `ctrip-app-ui-0.4.8.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxrwx   0        0        0        0 2024-05-14 11:51:12.951386 ctrip-app-ui-0.4.7/
--rw-rw-rw-   0        0        0    11558 2024-04-24 09:02:35.000000 ctrip-app-ui-0.4.7/LICENSE
--rw-rw-rw-   0        0        0      474 2024-05-14 11:51:12.950388 ctrip-app-ui-0.4.7/PKG-INFO
--rw-rw-rw-   0        0        0       47 2024-04-24 09:02:35.000000 ctrip-app-ui-0.4.7/README.md
-drwxrwxrwx   0        0        0        0 2024-05-14 11:51:12.936432 ctrip-app-ui-0.4.7/capp_ui/
--rw-rw-rw-   0        0        0      470 2024-04-24 09:06:21.000000 ctrip-app-ui-0.4.7/capp_ui/__init__.py
--rw-rw-rw-   0        0        0      736 2024-05-06 07:02:29.000000 ctrip-app-ui-0.4.7/capp_ui/config.py
--rw-rw-rw-   0        0        0     4060 2024-05-07 16:57:27.000000 ctrip-app-ui-0.4.7/capp_ui/date_extend.py
--rw-rw-rw-   0        0        0     1664 2024-05-09 13:31:21.000000 ctrip-app-ui-0.4.7/capp_ui/device.py
--rw-rw-rw-   0        0        0     1391 2024-04-25 08:27:58.000000 ctrip-app-ui-0.4.7/capp_ui/dir.py
--rw-rw-rw-   0        0        0    66560 2024-05-14 11:48:09.000000 ctrip-app-ui-0.4.7/capp_ui/domain_service.py
--rw-rw-rw-   0        0        0      613 2024-04-24 15:31:00.000000 ctrip-app-ui-0.4.7/capp_ui/fee.py
--rw-rw-rw-   0        0        0     3859 2024-05-11 16:34:35.000000 ctrip-app-ui-0.4.7/capp_ui/libs.py
--rw-rw-rw-   0        0        0    24821 2024-05-13 17:15:14.000000 ctrip-app-ui-0.4.7/capp_ui/mobile_terminals.py
--rw-rw-rw-   0        0        0     1719 2024-04-28 16:15:39.000000 ctrip-app-ui-0.4.7/capp_ui/platforms.py
--rw-rw-rw-   0        0        0      765 2024-04-28 16:02:26.000000 ctrip-app-ui-0.4.7/capp_ui/test.py
--rw-rw-rw-   0        0        0     5486 2024-05-11 03:13:30.000000 ctrip-app-ui-0.4.7/capp_ui/utils.py
--rw-rw-rw-   0        0        0     3023 2024-05-11 03:13:43.000000 ctrip-app-ui-0.4.7/capp_ui/validators.py
-drwxrwxrwx   0        0        0        0 2024-05-14 11:51:12.949366 ctrip-app-ui-0.4.7/ctrip_app_ui.egg-info/
--rw-rw-rw-   0        0        0      474 2024-05-14 11:51:12.000000 ctrip-app-ui-0.4.7/ctrip_app_ui.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      460 2024-05-14 11:51:12.000000 ctrip-app-ui-0.4.7/ctrip_app_ui.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-14 11:51:12.000000 ctrip-app-ui-0.4.7/ctrip_app_ui.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       30 2024-05-14 11:51:12.000000 ctrip-app-ui-0.4.7/ctrip_app_ui.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-05-14 11:51:12.000000 ctrip-app-ui-0.4.7/ctrip_app_ui.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-14 11:51:12.952404 ctrip-app-ui-0.4.7/setup.cfg
--rw-rw-rw-   0        0        0     1087 2024-05-14 11:51:06.000000 ctrip-app-ui-0.4.7/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-18 08:54:53.307423 ctrip-app-ui-0.4.8/
+-rw-rw-rw-   0        0        0    11558 2024-04-24 09:02:35.000000 ctrip-app-ui-0.4.8/LICENSE
+-rw-rw-rw-   0        0        0      474 2024-05-18 08:54:53.305397 ctrip-app-ui-0.4.8/PKG-INFO
+-rw-rw-rw-   0        0        0       47 2024-04-24 09:02:35.000000 ctrip-app-ui-0.4.8/README.md
+drwxrwxrwx   0        0        0        0 2024-05-18 08:54:53.278471 ctrip-app-ui-0.4.8/capp_ui/
+-rw-rw-rw-   0        0        0      470 2024-04-24 09:06:21.000000 ctrip-app-ui-0.4.8/capp_ui/__init__.py
+-rw-rw-rw-   0        0        0      736 2024-05-06 07:02:29.000000 ctrip-app-ui-0.4.8/capp_ui/config.py
+-rw-rw-rw-   0        0        0     4060 2024-05-07 16:57:27.000000 ctrip-app-ui-0.4.8/capp_ui/date_extend.py
+-rw-rw-rw-   0        0        0     1664 2024-05-09 13:31:21.000000 ctrip-app-ui-0.4.8/capp_ui/device.py
+-rw-rw-rw-   0        0        0     1391 2024-04-25 08:27:58.000000 ctrip-app-ui-0.4.8/capp_ui/dir.py
+-rw-rw-rw-   0        0        0    80683 2024-05-18 08:52:06.000000 ctrip-app-ui-0.4.8/capp_ui/domain_service.py
+-rw-rw-rw-   0        0        0      613 2024-04-24 15:31:00.000000 ctrip-app-ui-0.4.8/capp_ui/fee.py
+-rw-rw-rw-   0        0        0     4653 2024-05-18 04:20:17.000000 ctrip-app-ui-0.4.8/capp_ui/libs.py
+-rw-rw-rw-   0        0        0    24821 2024-05-13 17:15:14.000000 ctrip-app-ui-0.4.8/capp_ui/mobile_terminals.py
+-rw-rw-rw-   0        0        0     1719 2024-04-28 16:15:39.000000 ctrip-app-ui-0.4.8/capp_ui/platforms.py
+-rw-rw-rw-   0        0        0      765 2024-04-28 16:02:26.000000 ctrip-app-ui-0.4.8/capp_ui/test.py
+-rw-rw-rw-   0        0        0     5486 2024-05-11 03:13:30.000000 ctrip-app-ui-0.4.8/capp_ui/utils.py
+-rw-rw-rw-   0        0        0     3023 2024-05-11 03:13:43.000000 ctrip-app-ui-0.4.8/capp_ui/validators.py
+drwxrwxrwx   0        0        0        0 2024-05-18 08:54:53.304400 ctrip-app-ui-0.4.8/ctrip_app_ui.egg-info/
+-rw-rw-rw-   0        0        0      474 2024-05-18 08:54:52.000000 ctrip-app-ui-0.4.8/ctrip_app_ui.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      460 2024-05-18 08:54:52.000000 ctrip-app-ui-0.4.8/ctrip_app_ui.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-18 08:54:52.000000 ctrip-app-ui-0.4.8/ctrip_app_ui.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       30 2024-05-18 08:54:52.000000 ctrip-app-ui-0.4.8/ctrip_app_ui.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-05-18 08:54:52.000000 ctrip-app-ui-0.4.8/ctrip_app_ui.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-18 08:54:53.307423 ctrip-app-ui-0.4.8/setup.cfg
+-rw-rw-rw-   0        0        0     1087 2024-05-18 08:54:38.000000 ctrip-app-ui-0.4.8/setup.py
```

### Comparing `ctrip-app-ui-0.4.7/LICENSE` & `ctrip-app-ui-0.4.8/LICENSE`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.4.7/capp_ui/config.py` & `ctrip-app-ui-0.4.8/capp_ui/config.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.4.7/capp_ui/date_extend.py` & `ctrip-app-ui-0.4.8/capp_ui/date_extend.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.4.7/capp_ui/device.py` & `ctrip-app-ui-0.4.8/capp_ui/device.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.4.7/capp_ui/dir.py` & `ctrip-app-ui-0.4.8/capp_ui/dir.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.4.7/capp_ui/domain_service.py` & `ctrip-app-ui-0.4.8/capp_ui/domain_service.py`

 * *Files 14% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 from capp_ui.platforms import PlatformService
 from capp_ui.utils import get_ui_object_proxy_attr
 from capp_ui.config import ctrip_soft_keyboard_position
 from capp_ui.mobile_terminals import stop_app, PocoProxy
 from capp_ui.date_extend import is_later_than_current_time
 from capp_ui.dir import get_images_dir, is_exists, join_path
 from capp_ui.date_extend import get_trip_year_month_day, get_datetime_area, is_public_holiday
-from capp_ui.libs import SleepWait, LoopFindElement, LoopFindElementSubmit, logger, LoopClickElement
+from capp_ui.libs import SleepWait, LoopFindElement, LoopFindElementSubmit, logger, LoopExcute
 
 
 class CtripAppService(object):
     """
     携程APP
     """
     IMAGE_DIR = get_images_dir()
@@ -79,19 +79,72 @@
         file_name = join_path([get_images_dir(), "首页.png"])
         if is_exists(file_name):
             temp = self.device.get_cv_template(file_name=file_name)
         else:
             temp = (154, 2878)  # LG g7手机上对应的坐标位置，其他型号手机可能不是这个值
         self.device.touch(v=temp)
 
-    @LoopFindElementSubmit(loop=2, action="我的")
-    def touch_my(self):
+    @LoopExcute(loop=20, action="点击【我的】", sleep=1)
+    def touch_my(self) -> bool:
         """进入app后，点击【我的】"""
-        my_button = self.device.poco(type="android.view.ViewGroup", name="ctrip.android.view:id/a", desc="我的")
-        my_button.click()
+        try:
+            my_button = self.device.poco(
+                type="android.widget.ImageView", name="ctrip.android.view:id/home_tab_bar_icon_iv"
+            )
+            if my_button.exists() is True:
+                my_button.click()
+                time.sleep(0.5)
+                my_button = self.device.poco(
+                    type="android.widget.ImageView", name="ctrip.android.view:id/home_tab_bar_icon_iv"
+                )
+                if my_button.exists() is False:
+                    return True
+        except (Exception,):
+            pass
+        try:
+
+            my_button = self.device.poco(type="android.view.ViewGroup", name="ctrip.android.view:id/a", desc="我的")
+            if my_button.exists() is True:
+                my_button.click()
+                time.sleep(0.5)
+                my_button = self.device.poco(type="android.view.ViewGroup", name="ctrip.android.view:id/a", desc="我的")
+                if my_button.exists() is False:
+                    return True
+        except (Exception,):
+            pass
+        try:
+            file_name = join_path([get_images_dir(), "我的.png"])
+            if is_exists(file_name):
+                temp = self.device.get_cv_template(file_name=file_name, threshold=0.9)
+                pos = self.device.exists(v=temp)
+                if pos:
+                    self.device.touch(v=pos)
+                    time.sleep(0.5)
+                    pos = self.device.exists(v=temp)
+                    if pos is False:
+                        return True
+            else:
+                # temp = (975, 2214)  # Huawei Mate 20手机上对应的坐标位置，其他型号手机可能不是这个值
+                logger.warning("文件{}，没找到".format(file_name))
+        except (Exception,):
+            pass
+        try:
+            # 手机可能处于USB弹框提示点击【仅充电】
+            file_name = join_path([get_images_dir(), "仅充电.png"])
+            if is_exists(file_name):
+                temp = self.device.get_cv_template(file_name=file_name, threshold=0.9)
+                pos = self.device.exists(v=temp)
+                if pos:
+                    self.device.touch(v=pos)
+            else:
+                # temp = (975, 2214)  # Huawei Mate 20手机上对应的坐标位置，其他型号手机可能不是这个值
+                logger.warning("文件{}，没找到".format(file_name))
+        except (Exception,):
+            pass
+        return False
 
     @LoopFindElementSubmit(loop=1, action="设置")
     def touch_settings(self):
         """我的主页，点击【设置】"""
         setting_button = self.device.poco(type="android.widget.ImageView", name="ctrip.android.view:id/a", desc="设置")
         setting_button.click()
 
@@ -108,39 +161,124 @@
     def touch_submit_logout(self):
         """退出登录弹框，点击【确定】"""
         logout_user = self.device.poco(
             type="android.widget.TextView", name="ctrip.android.view:id/a", text="确定"
         )
         logout_user.click()
 
+    @LoopExcute(loop=20, action="点击【待付款】", sleep=1)
     def touch_unpaid(self) -> bool:
         """进入my主页后，点击【待付款】"""
-        flag = False
         try:
             # 待付款元素定位1
-            unpaid_button_1 = self.device.poco(
+            unpaid_button = self.device.poco(
                 type="android.widget.TextView", name="ctrip.android.view:id/a", text="待付款"
             )
-            unpaid_button_1.click()
-            flag = True
-            time.sleep(1)
+            if unpaid_button.exists() is True:
+                unpaid_button.click()
+                time.sleep(0.5)
+                unpaid_button = self.device.poco(
+                    type="android.widget.TextView", name="ctrip.android.view:id/a", text="待付款"
+                )
+                if unpaid_button.exists() is False:
+                    return True
         except (Exception,):
             pass
-        if flag is False:
-            try:
-                # 待付款元素定位2
-                unpaid_button_2 = self.device.poco(
+        try:
+            # 待付款元素定位2
+            unpaid_button = self.device.poco(
+                type="android.widget.TextView", name="android.widget.TextView", text="待付款"
+            )
+            if unpaid_button.exists() is True:
+                unpaid_button.click()
+                time.sleep(0.5)
+                unpaid_button = self.device.poco(
                     type="android.widget.TextView", name="android.widget.TextView", text="待付款"
                 )
-                unpaid_button_2.click()
-                flag = True
-                time.sleep(1)
-            except (Exception,):
-                pass
-        return flag
+                if unpaid_button.exists() is False:
+                    return True
+        except (Exception,):
+            pass
+        try:
+            file_name = join_path([get_images_dir(), "我的待办_待付款.png"])
+            if is_exists(file_name):
+                temp = self.device.get_cv_template(file_name=file_name, threshold=0.9)
+                pos = self.device.exists(v=temp)
+                if pos:
+                    self.device.touch(v=pos)
+                    time.sleep(0.5)
+                    pos = self.device.exists(v=temp)
+                    if pos is False:
+                        return True
+            else:
+                # temp = (417, 947)  # Huawei Mate 20手机上对应的坐标位置，其他型号手机可能不是这个值
+                logger.warning("文件{}，没找到".format(file_name))
+        except (Exception,):
+            pass
+        return False
+
+    @LoopExcute(loop=20, action="搜索【待支付订单】", sleep=1)
+    def search_unpaid_order(self, ctrip_order_id: str) -> bool:
+        """搜索待支付的订单，这里面有2个步骤：1，定位搜索入口，并点击进入搜索界面，2.输入搜索内容"""
+        try:
+            search_box = self.device.poco(
+                type="android.widget.TextView", name="android.widget.TextView", text="搜索订单"
+            )
+            if search_box.exists() is True:
+                search_box.click()
+                time.sleep(0.5)
+                search_box = self.device.poco(
+                    type="android.widget.EditText", name="android.widget.EditText", text="输入城市名/订单号 搜索订单"
+                )
+                if search_box.exists() is True:
+                    search_box.click()
+                    search_box.set_text(ctrip_order_id)
+                    # 模拟键盘按下回车键（keyCode为66表示回车键）
+                    self.device.keyevent(keyname="66")
+                    time.sleep(1)
+                    return True
+        except (Exception,):
+            pass
+        try:
+            file_name = join_path([get_images_dir(), "搜索订单_搜索框.png"])
+            if is_exists(file_name):
+                temp = self.device.get_cv_template(file_name=file_name, threshold=0.9)
+                pos = self.device.exists(v=temp)
+                if pos:
+                    self.device.touch(v=pos)
+                    time.sleep(0.5)
+                    pos = self.device.exists(v=temp)
+                    if pos is False:
+                        self.device.text(text=ctrip_order_id, enter=True)
+                        time.sleep(1)
+                        return True
+            else:
+                # temp = (289, 168)  # Huawei Mate 20手机上对应的坐标位置，其他型号手机可能不是这个值
+                logger.warning("文件{}，没找到".format(file_name))
+        except (Exception,):
+            pass
+        try:
+            file_name = join_path([get_images_dir(), "搜索_放大镜.png"])
+            if is_exists(file_name):
+                temp = self.device.get_cv_template(file_name=file_name, threshold=0.9)
+                pos = self.device.exists(v=temp)
+                if pos:
+                    self.device.touch(v=pos)
+                    time.sleep(0.5)
+                    pos = self.device.exists(v=temp)
+                    if pos is False:
+                        self.device.text(text=ctrip_order_id, enter=True)
+                        time.sleep(1)
+                        return True
+            else:
+                # temp = (896, 173)  # Huawei Mate 20手机上对应的坐标位置，其他型号手机可能不是这个值
+                logger.warning("文件{}，没找到".format(file_name))
+        except (Exception,):
+            pass
+        return False
 
     @LoopFindElementSubmit(loop=3, action="列表页搜索框")
     def touch_list_page_search_box(self):
         """进入待付款列表页，点击【搜索框】"""
         search_box = self.device.poco(
             type="android.widget.TextView", name="android.widget.TextView", text="搜索订单"
         )
@@ -153,29 +291,43 @@
             type="android.widget.EditText", name="android.widget.EditText", text="输入城市名/订单号 搜索订单"
         )
         search_box.click()
         search_box.set_text(ctrip_order_id)
         # 模拟键盘按下回车键（keyCode为66表示回车键）
         self.device.keyevent(keyname="66")
 
-    @SleepWait(wait_time=1)
+    @LoopExcute(loop=1, action="判断订单是否为【待支付】", sleep=1)
     def is_exist_to_payment_at_list_page(self) -> bool:
-        """检查搜索列表界面，是否存在【去支付】按钮"""
-        flag = False
+        """检查搜索列表界面，是否存在【待支付】状态"""
         try:
             is_exist = self.device.poco(type="android.widget.TextView", name="android.widget.TextView", text="去支付")
             if is_exist.exists() is True:
-                flag = True
-        except (PocoNoSuchNodeException, PocoTargetTimeout):
+                return True
+        except (Exception,):
             pass
-        except Exception as e:
-            logger.error(e)
-        return flag
+        try:
+            is_exist = self.device.poco(type="android.widget.TextView", name="android.widget.TextView", text="待支付")
+            if is_exist.exists() is True:
+                return True
+        except (Exception,):
+            pass
+        try:
+            file_name = join_path([get_images_dir(), "订单状态_待支付.png"])
+            if is_exists(file_name):
+                temp = self.device.get_cv_template(file_name=file_name, threshold=0.9)
+                pos = self.device.exists(v=temp)
+                if pos:
+                    return True
+            else:
+                # temp = (1033, 381)  # Huawei Mate 20手机上对应的坐标位置，其他型号手机可能不是这个值
+                logger.warning("文件{}，没找到".format(file_name))
+        except (Exception,):
+            pass
+        return False
 
-    @SleepWait(wait_time=1)
     def get_order_status(self) -> str:
         """检查搜索列表界面，获取订单的状态"""
         status = None
         try:
             unpaid_status = self.device.poco(
                 type="android.widget.TextView", name="android.widget.TextView", text="去支付"
             )
@@ -195,14 +347,22 @@
             out_ticketed_status = self.device.poco(
                 type="android.widget.TextView", name="android.widget.TextView", text="已出票"
             )
             if out_ticketed_status.exists() is True:
                 status = "已出票"
         except (PocoNoSuchNodeException, PocoTargetTimeout, Exception):
             pass
+        try:
+            out_ticketed_status = self.device.poco(
+                type="android.widget.TextView", name="android.widget.TextView", text="出票中"
+            )
+            if out_ticketed_status.exists() is True:
+                status = "出票中"
+        except (PocoNoSuchNodeException, PocoTargetTimeout, Exception):
+            pass
         return status
 
     def is_order_detail_page(self) -> bool:
         """是否在订单详情界面"""
         flag = False
         try:
             order_detail_page_1 = self.device.poco(
@@ -263,27 +423,46 @@
             if go_back.exists() is True:
                 go_back.click()
         except (PocoNoSuchNodeException, PocoTargetTimeout):
             pass
         except Exception as e:
             logger.error(e)
 
+    @LoopExcute(loop=3, sleep=1, action="点击【去支付】")
     def touch_to_payment_at_list_page(self) -> bool:
         """进入待付款列表页，点击【去支付】"""
-        flag = False
         try:
-            search_box = self.device.poco(type="android.widget.TextView", name="android.widget.TextView", text="去支付")
-            search_box.click()
-            flag = True
-            time.sleep(1)
-        except (PocoNoSuchNodeException, PocoTargetTimeout):
+            to_payment = self.device.poco(type="android.widget.TextView", name="android.widget.TextView", text="去支付")
+            if to_payment.exists() is True:
+                to_payment.click()
+                time.sleep(0.5)
+                to_payment = self.device.poco(
+                    type="android.widget.TextView", name="android.widget.TextView", text="去支付"
+                )
+                if to_payment.exists() is False:
+                    return True
+        except (Exception,):
             pass
-        except Exception as e:
-            logger.error(e)
-        return flag
+        try:
+            file_name = join_path([get_images_dir(), "订单状态_待支付.png"])
+            if is_exists(file_name):
+                temp = self.device.get_cv_template(file_name=file_name, threshold=0.9)
+                pos = self.device.exists(v=temp)
+                if pos:
+                    self.device.touch(v=pos)
+                    time.sleep(0.5)
+                    pos = self.device.exists(v=temp)
+                    if pos is False:
+                        return True
+            else:
+                # temp = (1033, 513)  # Huawei Mate 20手机上对应的坐标位置，其他型号手机可能不是这个值
+                logger.warning("文件{}，没找到".format(file_name))
+        except (Exception,):
+            pass
+        return False
 
     @SleepWait(wait_time=1)
     def is_cancel_order(self, out_total_price: str, amount_loss_limit: str, profit_cap: str, passenger_number: int,
                         discount_amount: str = None) -> tuple:
         """在订单详情页，判断是否需要取消订单"""
         flag = False
         remark = None
@@ -363,19 +542,125 @@
     def touch_know_the_cancel_order(self):
         """确认取消后，会有一个【知道了】的小弹框"""
         submit_cancel_order = self.device.poco(
             type="android.widget.TextView", name="Button_Text_知道了", text="知道了"
         )
         submit_cancel_order.click()
 
-    @LoopFindElementSubmit(loop=1, action="详情-去支付")
+    def get_order_detail_page_order_state(self) -> str:
+        try:
+            order_detail = self.device.poco(
+                type="android.widget.TextView", name="android.widget.TextView", text="订单详情"
+            )
+            if order_detail.exists() is True:
+                try:
+                    canceled = self.device.poco(type="android.widget.TextView", name="android.widget.TextView",
+                                                text="已取消")
+                    if canceled.exists() is True:
+                        return "已取消"
+                except (Exception,):
+                    pass
+                try:
+                    to_payment = self.device.poco(
+                        type="android.widget.TextView", name="android.widget.TextView", text="去支付"
+                    )
+                    if to_payment.exists() is True:
+                        return "去支付"
+                except (Exception,):
+                    pass
+                try:
+                    to_payment = self.device.poco(
+                        type="android.widget.TextView", name="pcardLimit_Text_去支付", text="去支付"
+                    )
+                    if to_payment.exists() is True:
+                        return "去支付"
+                except (Exception,):
+                    pass
+        except (Exception,):
+            pass
+        try:
+            file_name = join_path([get_images_dir(), "订单详情.png"])
+            if is_exists(file_name):
+                temp = self.device.get_cv_template(file_name=file_name, threshold=0.9)
+                pos = self.device.exists(v=temp)
+                if pos:
+                    try:
+                        file_name = join_path([get_images_dir(), "订单详情_去支付.png"])
+                        if is_exists(file_name):
+                            temp = self.device.get_cv_template(file_name=file_name, threshold=0.9)
+                            pos = self.device.exists(v=temp)
+                            if pos:
+                                return "去支付"
+                        else:
+                            # temp = (873, 440)  # Huawei Mate 20手机上对应的坐标位置，其他型号手机可能不是这个值
+                            logger.warning("文件{}，没找到".format(file_name))
+                    except (Exception,):
+                        pass
+                    try:
+                        file_name = join_path([get_images_dir(), "订单详情_已取消.png"])
+                        if is_exists(file_name):
+                            temp = self.device.get_cv_template(file_name=file_name, threshold=0.9)
+                            pos = self.device.exists(v=temp)
+                            if pos:
+                                return "已取消"
+                        else:
+                            # temp = (166, 311)  # Huawei Mate 20手机上对应的坐标位置，其他型号手机可能不是这个值
+                            logger.warning("文件{}，没找到".format(file_name))
+                    except (Exception,):
+                        pass
+            else:
+                # temp = (466, 173)  # Huawei Mate 20手机上对应的坐标位置，其他型号手机可能不是这个值
+                logger.warning("文件{}，没找到".format(file_name))
+        except (Exception,):
+            pass
+        return ""
+
+    @LoopExcute(action="订单详情页点击【去支付】", loop=10, sleep=1)
     def touch_to_payment_at_order_detail(self):
         """在订单详情页，点击【去支付】"""
-        search_box = self.device.poco(type="android.widget.TextView", name="pcardLimit_Text_去支付", text="去支付")
-        search_box.click()
+        try:
+            to_payment = self.device.poco(type="android.widget.TextView", name="pcardLimit_Text_去支付", text="去支付")
+            if to_payment.exists() is True:
+                to_payment.click()
+                time.sleep(3)
+                to_payment = self.device.poco(
+                    type="android.widget.TextView", name="pcardLimit_Text_去支付", text="去支付"
+                )
+                if to_payment.exists() is False:
+                    return True
+        except (Exception,):
+            pass
+        try:
+            to_payment = self.device.poco(type="android.widget.TextView", name="android.widget.TextView", text="去支付")
+            if to_payment.exists() is True:
+                to_payment.click()
+                time.sleep(3)
+                to_payment = self.device.poco(
+                    type="android.widget.TextView", name="android.widget.TextView", text="去支付"
+                )
+                if to_payment.exists() is False:
+                    return True
+        except (Exception,):
+            pass
+        try:
+            file_name = join_path([get_images_dir(), "订单详情_去支付.png"])
+            if is_exists(file_name):
+                temp = self.device.get_cv_template(file_name=file_name, threshold=0.9)
+                pos = self.device.exists(v=temp)
+                if pos:
+                    self.device.touch(v=pos)
+                    time.sleep(3)
+                    pos = self.device.exists(v=temp)
+                    if pos is False:
+                        return True
+            else:
+                # temp = (873, 440)  # Huawei Mate 20手机上对应的坐标位置，其他型号手机可能不是这个值
+                logger.warning("文件{}，没找到".format(file_name))
+        except (Exception,):
+            pass
 
     @SleepWait(wait_time=1)
     def touch_flight_ticket(self) -> None:
         """进入app后，点击【首页】，点击【机票】"""
         file_name = join_path([get_images_dir(), "机票.png"])
         if is_exists(file_name):
             temp = self.device.get_cv_template(file_name=file_name)
```

### Comparing `ctrip-app-ui-0.4.7/capp_ui/fee.py` & `ctrip-app-ui-0.4.8/capp_ui/fee.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.4.7/capp_ui/libs.py` & `ctrip-app-ui-0.4.8/capp_ui/libs.py`

 * *Files 14% similar despite different names*

```diff
@@ -119,7 +119,31 @@
                     logger.error(e)
                     break
                 # 1秒钟查找一次
                 sleep(1)
             return flag
 
         return wrapper
+
+
+class LoopExcute(object):
+
+    def __init__(self, action: str, loop: int = 1, sleep: int = 1) -> None:
+        self.loop = loop
+        self.sleep = sleep
+        self.action = action
+
+    def __call__(self, func: Callable) -> Any:
+        def wrapper(*args, **kwargs) -> bool:
+            flag = False
+            for i in range(self.loop):
+                if i > 0:
+                    logger.warning("尝试第{}次{}".format(i, self.action))
+                flag = func(*args, **kwargs)
+                if flag is True:
+                    break
+                sleep(self.sleep)
+            if flag is False and self.loop > 2:
+                logger.warning("{}次尝试{}都失败".format(self.loop, self.action))
+            return flag
+
+        return wrapper
```

### Comparing `ctrip-app-ui-0.4.7/capp_ui/mobile_terminals.py` & `ctrip-app-ui-0.4.8/capp_ui/mobile_terminals.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.4.7/capp_ui/platforms.py` & `ctrip-app-ui-0.4.8/capp_ui/platforms.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.4.7/capp_ui/test.py` & `ctrip-app-ui-0.4.8/capp_ui/test.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.4.7/capp_ui/utils.py` & `ctrip-app-ui-0.4.8/capp_ui/utils.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.4.7/capp_ui/validators.py` & `ctrip-app-ui-0.4.8/capp_ui/validators.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.4.7/setup.py` & `ctrip-app-ui-0.4.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 # Copyright ©2011-2024. Hunan xxxxxxx Company limited. All rights reserved.
 # ---------------------------------------------------------------------------------------------------------
 """
 from setuptools import setup, find_packages
 
 setup(
     name='ctrip-app-ui',
-    version='0.4.7',
+    version='0.4.8',
     description='This is my ctrip app ui package',
     long_description='This is my ctrip app ui package',
     author='ckf10000',
     author_email='ckf10000@sina.com',
     url='https://github.com/ckf10000/ctrip-app-ui',
     packages=find_packages(),
     install_requires=[
```

