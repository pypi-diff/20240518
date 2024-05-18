# Comparing `tmp/ctrip-app-ui-0.5.1.tar.gz` & `tmp/ctrip-app-ui-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ctrip-app-ui-0.5.1.tar", last modified: Sat May 18 15:03:58 2024, max compression
+gzip compressed data, was "ctrip-app-ui-0.5.2.tar", last modified: Sat May 18 15:40:32 2024, max compression
```

## Comparing `ctrip-app-ui-0.5.1.tar` & `ctrip-app-ui-0.5.2.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxrwx   0        0        0        0 2024-05-18 15:03:58.605503 ctrip-app-ui-0.5.1/
--rw-rw-rw-   0        0        0    11558 2024-04-24 09:02:35.000000 ctrip-app-ui-0.5.1/LICENSE
--rw-rw-rw-   0        0        0      474 2024-05-18 15:03:58.604506 ctrip-app-ui-0.5.1/PKG-INFO
--rw-rw-rw-   0        0        0       47 2024-04-24 09:02:35.000000 ctrip-app-ui-0.5.1/README.md
-drwxrwxrwx   0        0        0        0 2024-05-18 15:03:58.577535 ctrip-app-ui-0.5.1/capp_ui/
--rw-rw-rw-   0        0        0      470 2024-04-24 09:06:21.000000 ctrip-app-ui-0.5.1/capp_ui/__init__.py
--rw-rw-rw-   0        0        0      736 2024-05-06 07:02:29.000000 ctrip-app-ui-0.5.1/capp_ui/config.py
--rw-rw-rw-   0        0        0     4060 2024-05-07 16:57:27.000000 ctrip-app-ui-0.5.1/capp_ui/date_extend.py
--rw-rw-rw-   0        0        0     1664 2024-05-09 13:31:21.000000 ctrip-app-ui-0.5.1/capp_ui/device.py
--rw-rw-rw-   0        0        0     1391 2024-04-25 08:27:58.000000 ctrip-app-ui-0.5.1/capp_ui/dir.py
--rw-rw-rw-   0        0        0    45770 2024-05-18 15:03:27.000000 ctrip-app-ui-0.5.1/capp_ui/domain_service.py
--rw-rw-rw-   0        0        0      613 2024-04-24 15:31:00.000000 ctrip-app-ui-0.5.1/capp_ui/fee.py
--rw-rw-rw-   0        0        0     5414 2024-05-18 14:39:38.000000 ctrip-app-ui-0.5.1/capp_ui/libs.py
--rw-rw-rw-   0        0        0    24821 2024-05-13 17:15:14.000000 ctrip-app-ui-0.5.1/capp_ui/mobile_terminals.py
--rw-rw-rw-   0        0        0     1719 2024-04-28 16:15:39.000000 ctrip-app-ui-0.5.1/capp_ui/platforms.py
--rw-rw-rw-   0        0        0      765 2024-04-28 16:02:26.000000 ctrip-app-ui-0.5.1/capp_ui/test.py
--rw-rw-rw-   0        0        0     5486 2024-05-11 03:13:30.000000 ctrip-app-ui-0.5.1/capp_ui/utils.py
--rw-rw-rw-   0        0        0     3023 2024-05-11 03:13:43.000000 ctrip-app-ui-0.5.1/capp_ui/validators.py
-drwxrwxrwx   0        0        0        0 2024-05-18 15:03:58.602531 ctrip-app-ui-0.5.1/ctrip_app_ui.egg-info/
--rw-rw-rw-   0        0        0      474 2024-05-18 15:03:58.000000 ctrip-app-ui-0.5.1/ctrip_app_ui.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      460 2024-05-18 15:03:58.000000 ctrip-app-ui-0.5.1/ctrip_app_ui.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-18 15:03:58.000000 ctrip-app-ui-0.5.1/ctrip_app_ui.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       30 2024-05-18 15:03:58.000000 ctrip-app-ui-0.5.1/ctrip_app_ui.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-05-18 15:03:58.000000 ctrip-app-ui-0.5.1/ctrip_app_ui.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-18 15:03:58.606501 ctrip-app-ui-0.5.1/setup.cfg
--rw-rw-rw-   0        0        0     1087 2024-05-18 15:03:53.000000 ctrip-app-ui-0.5.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-18 15:40:32.471464 ctrip-app-ui-0.5.2/
+-rw-rw-rw-   0        0        0    11558 2024-04-24 09:02:35.000000 ctrip-app-ui-0.5.2/LICENSE
+-rw-rw-rw-   0        0        0      474 2024-05-18 15:40:32.470474 ctrip-app-ui-0.5.2/PKG-INFO
+-rw-rw-rw-   0        0        0       47 2024-04-24 09:02:35.000000 ctrip-app-ui-0.5.2/README.md
+drwxrwxrwx   0        0        0        0 2024-05-18 15:40:32.442541 ctrip-app-ui-0.5.2/capp_ui/
+-rw-rw-rw-   0        0        0      470 2024-04-24 09:06:21.000000 ctrip-app-ui-0.5.2/capp_ui/__init__.py
+-rw-rw-rw-   0        0        0      736 2024-05-06 07:02:29.000000 ctrip-app-ui-0.5.2/capp_ui/config.py
+-rw-rw-rw-   0        0        0     4060 2024-05-07 16:57:27.000000 ctrip-app-ui-0.5.2/capp_ui/date_extend.py
+-rw-rw-rw-   0        0        0     1664 2024-05-09 13:31:21.000000 ctrip-app-ui-0.5.2/capp_ui/device.py
+-rw-rw-rw-   0        0        0     1391 2024-04-25 08:27:58.000000 ctrip-app-ui-0.5.2/capp_ui/dir.py
+-rw-rw-rw-   0        0        0    44871 2024-05-18 15:39:35.000000 ctrip-app-ui-0.5.2/capp_ui/domain_service.py
+-rw-rw-rw-   0        0        0      613 2024-04-24 15:31:00.000000 ctrip-app-ui-0.5.2/capp_ui/fee.py
+-rw-rw-rw-   0        0        0     5414 2024-05-18 14:39:38.000000 ctrip-app-ui-0.5.2/capp_ui/libs.py
+-rw-rw-rw-   0        0        0    24821 2024-05-13 17:15:14.000000 ctrip-app-ui-0.5.2/capp_ui/mobile_terminals.py
+-rw-rw-rw-   0        0        0     1719 2024-04-28 16:15:39.000000 ctrip-app-ui-0.5.2/capp_ui/platforms.py
+-rw-rw-rw-   0        0        0      765 2024-04-28 16:02:26.000000 ctrip-app-ui-0.5.2/capp_ui/test.py
+-rw-rw-rw-   0        0        0     5486 2024-05-11 03:13:30.000000 ctrip-app-ui-0.5.2/capp_ui/utils.py
+-rw-rw-rw-   0        0        0     3023 2024-05-11 03:13:43.000000 ctrip-app-ui-0.5.2/capp_ui/validators.py
+drwxrwxrwx   0        0        0        0 2024-05-18 15:40:32.468473 ctrip-app-ui-0.5.2/ctrip_app_ui.egg-info/
+-rw-rw-rw-   0        0        0      474 2024-05-18 15:40:32.000000 ctrip-app-ui-0.5.2/ctrip_app_ui.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      460 2024-05-18 15:40:32.000000 ctrip-app-ui-0.5.2/ctrip_app_ui.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-18 15:40:32.000000 ctrip-app-ui-0.5.2/ctrip_app_ui.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       30 2024-05-18 15:40:32.000000 ctrip-app-ui-0.5.2/ctrip_app_ui.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-05-18 15:40:32.000000 ctrip-app-ui-0.5.2/ctrip_app_ui.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-18 15:40:32.471464 ctrip-app-ui-0.5.2/setup.cfg
+-rw-rw-rw-   0        0        0     1087 2024-05-18 15:40:29.000000 ctrip-app-ui-0.5.2/setup.py
```

### Comparing `ctrip-app-ui-0.5.1/LICENSE` & `ctrip-app-ui-0.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.5.1/capp_ui/config.py` & `ctrip-app-ui-0.5.2/capp_ui/config.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.5.1/capp_ui/date_extend.py` & `ctrip-app-ui-0.5.2/capp_ui/date_extend.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.5.1/capp_ui/device.py` & `ctrip-app-ui-0.5.2/capp_ui/device.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.5.1/capp_ui/dir.py` & `ctrip-app-ui-0.5.2/capp_ui/dir.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.5.1/capp_ui/domain_service.py` & `ctrip-app-ui-0.5.2/capp_ui/domain_service.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 from poco.exceptions import PocoNoSuchNodeException, PocoTargetTimeout
 
 from capp_ui.platforms import PlatformService
 from capp_ui.config import ctrip_soft_keyboard_position
 from capp_ui.mobile_terminals import stop_app, PocoProxy
 from capp_ui.date_extend import is_later_than_current_time
 from capp_ui.dir import get_images_dir, is_exists, join_path
-from capp_ui.libs import SleepWait, LoopFindElementSubmit, logger, LoopFindElementObject
+from capp_ui.libs import SleepWait, LoopFindElementSubmit, logger, LoopFindElementObject, LoopExcute
 
 
 class CtripAppService(object):
     """
     携程APP
     """
     IMAGE_DIR = get_images_dir()
@@ -305,15 +305,15 @@
             pass
         try:
             unpaid_status = self.device.poco(
                 type="android.widget.TextView", name="android.widget.TextView", text="去支付"
             )
             if unpaid_status.exists() is True:
                 return "待支付"
-        except (PocoNoSuchNodeException, PocoTargetTimeout, Exception):
+        except (Exception,):
             pass
         try:
             unpaid_status = self.device.poco(
                 type="android.widget.TextView", name="android.widget.TextView", text="待支付"
             )
             if unpaid_status.exists() is True:
                 return "待支付"
@@ -321,54 +321,54 @@
             pass
         try:
             cancel_status = self.device.poco(
                 type="android.widget.TextView", name="android.widget.TextView", text="已取消"
             )
             if cancel_status.exists() is True:
                 return "已取消"
-        except (PocoNoSuchNodeException, PocoTargetTimeout, Exception):
+        except (Exception,):
             pass
         try:
             out_ticketed_status = self.device.poco(
                 type="android.widget.TextView", name="android.widget.TextView", text="已出票"
             )
             if out_ticketed_status.exists() is True:
                 return "已出票"
-        except (PocoNoSuchNodeException, PocoTargetTimeout, Exception):
+        except (Exception,):
             pass
         try:
             out_ticketed_status = self.device.poco(
                 type="android.widget.TextView", name="android.widget.TextView", text="出票中"
             )
             if out_ticketed_status.exists() is True:
                 return "出票中"
-        except (PocoNoSuchNodeException, PocoTargetTimeout, Exception):
+        except (Exception,):
             pass
         return ""
 
-    @LoopFindElementObject(loop=20, action="从搜索结果获取【去支付】按钮", sleep=1)
+    @LoopFindElementObject(loop=20, action="搜索结果获取【去支付】按钮", sleep=1)
     def get_to_payment_at_list_page(self) -> dict:
         try:
-            to_payment = self.device.poco(type="android.widget.TextView", name="android.widget.TextView", text="去支付")
-            if to_payment.exists() is True:
-                return {"element": to_payment}
-        except (Exception,):
-            pass
-        try:
             file_name = join_path([get_images_dir(), "订单状态_待支付.png"])
             if is_exists(file_name):
                 temp = self.device.get_cv_template(file_name=file_name, threshold=0.9)
                 pos = self.device.exists(v=temp)
                 if pos:
                     return {"pos": pos}
             else:
                 # temp = (1033, 513)  # Huawei Mate 20手机上对应的坐标位置，其他型号手机可能不是这个值
                 logger.warning("文件{}，没找到".format(file_name))
         except (Exception,):
             pass
+        try:
+            to_payment = self.device.poco(type="android.widget.TextView", name="android.widget.TextView", text="去支付")
+            if to_payment.exists() is True:
+                return {"element": to_payment}
+        except (Exception,):
+            pass
         return dict()
 
     def is_order_detail_page(self) -> bool:
         """是否在订单详情界面"""
         flag = False
         try:
             order_detail_page_1 = self.device.poco(
@@ -401,75 +401,79 @@
             )
             if order_detail_page_4.exists() is True:
                 flag = True
         except (PocoNoSuchNodeException, PocoTargetTimeout, Exception):
             pass
         return flag
 
-    @SleepWait(wait_time=1)
+    @LoopFindElementObject(loop=20, action="订单详情页获取【支付金额】", sleep=1)
+    def get_order_amount_with_order_detail(self) -> dict:
+        try:
+            amount_text = self.device.poco(
+                type="android.widget.TextView", name="android.widget.TextView", textMatches=r"^请在\d+:\d+前支付.*"
+            )
+            if amount_text.exists() is True:
+                return {"element": amount_text}
+        except (Exception,):
+            pass
+        return dict()
+
     def is_cancel_order(self, out_total_price: str, amount_loss_limit: str, profit_cap: str, passenger_number: int,
                         discount_amount: str = None) -> tuple:
         """在订单详情页，判断是否需要取消订单"""
         flag = False
         remark = None
-        try:
-            is_cancel = self.device.poco(
-                type="android.widget.TextView", name="android.widget.TextView", textMatches=r"^请在\d+:\d+前支付.*"
-            )
-            if is_cancel.exists() is True:
-                text = is_cancel.get_text()
-                time_match = re.search(r'(\d{2}:\d{2})', text)
-                amount_match = re.search(r'¥(\d+)', text)
-                if time_match and amount_match:
-                    time_str = time_match.group(1)
-                    string = "从订单获取到的过期时间为：{}".format(time_str)
-                    minutes = 1
-                    is_later = is_later_than_current_time(time_str=time_str, minutes=minutes)
-                    if is_later is False:
-                        flag = True
-                        remark = "支付时间少于{}分钟".format(minutes)
-                        string = string + "，" + remark
-                    else:
-                        amount_str = amount_match.group(1)
-                        string = "从携程订单获取的支付金额：{}，劲旅订单总价：{}".format(amount_str, out_total_price)
-                        # 预期订单利润
-                        ex_order_profit = Decimal(out_total_price) - Decimal(amount_str)
-                        if discount_amount:
-                            # 实际订单利润
-                            ac_order_profit = ex_order_profit + Decimal(discount_amount)
-                        else:
-                            ac_order_profit = ex_order_profit
-                        # 订单利润 < 0, 存在亏钱，与亏钱的下限进行比较
-                        if ac_order_profit < 0:
-                            total = Decimal(amount_loss_limit) * passenger_number
-                            if ac_order_profit + total < 0:
-                                flag = True
-                                remark = "订单亏钱{:.2f}太多，超过订单总下限值{}(单人下限{} * {}人)".format(
-                                    abs(ac_order_profit), total, amount_loss_limit, passenger_number
-                                )
-                                logger.warning(remark)
-                        # 订单利润 >= 0, 存在毛利，与利润的上限进行比较
-                        else:
-                            total = Decimal(profit_cap) * passenger_number
-                            if ac_order_profit - total > 0:
-                                flag = True
-                                remark = "订单利润{:.2f}太高，超过订单总下限值{}(单人下限{} * {}人)".format(
-                                    ac_order_profit, total, profit_cap, passenger_number
-                                )
-                                logger.warning(remark)
-
+        attr = self.get_order_amount_with_order_detail()
+        amount_text = attr.get("element")
+        if amount_text:
+            text = amount_text.get_text()
+            time_match = re.search(r'(\d{2}:\d{2})', text)
+            amount_match = re.search(r'¥(\d+)', text)
+            if time_match and amount_match:
+                time_str = time_match.group(1)
+                string = "从订单获取到的过期时间为：{}".format(time_str)
+                minutes = 1
+                is_later = is_later_than_current_time(time_str=time_str, minutes=minutes)
+                if is_later is False:
+                    flag = True
+                    remark = "支付时间少于{}分钟".format(minutes)
+                    string = string + "，" + remark
                 else:
-                    string = "从元素的文案<{}>提取时间与金额信息有异常".format(text)
+                    amount_str = amount_match.group(1)
+                    string = "从携程订单获取的支付金额：{}，劲旅订单总价：{}".format(amount_str, out_total_price)
+                    # 预期订单利润
+                    ex_order_profit = Decimal(out_total_price) - Decimal(amount_str)
+                    if discount_amount:
+                        # 实际订单利润
+                        ac_order_profit = ex_order_profit + Decimal(discount_amount)
+                    else:
+                        ac_order_profit = ex_order_profit
+                    # 订单利润 < 0, 存在亏钱，与亏钱的下限进行比较
+                    if ac_order_profit < 0:
+                        total = Decimal(amount_loss_limit) * passenger_number
+                        if ac_order_profit + total < 0:
+                            flag = True
+                            remark = "订单亏钱{:.2f}太多，超过订单总下限值{}(单人下限{} * {}人)".format(
+                                abs(ac_order_profit), total, amount_loss_limit, passenger_number
+                            )
+                            logger.warning(remark)
+                    # 订单利润 >= 0, 存在毛利，与利润的上限进行比较
+                    else:
+                        total = Decimal(profit_cap) * passenger_number
+                        if ac_order_profit - total > 0:
+                            flag = True
+                            remark = "订单利润{:.2f}太高，超过订单总下限值{}(单人下限{} * {}人)".format(
+                                ac_order_profit, total, profit_cap, passenger_number
+                            )
+                            logger.warning(remark)
             else:
-                string = "元素定位存在异常，订单详情页没有找到订单支付金额和过期时间"
-            logger.warning(string)
-        except (PocoNoSuchNodeException, PocoTargetTimeout):
-            pass
-        except Exception as e:
-            logger.error(e)
+                string = "从元素的文案<{}>提取时间与金额信息有异常".format(text)
+        else:
+            string = "元素定位存在异常，订单详情页没有找到订单支付金额和过期时间"
+        logger.warning(string)
         return flag, remark
 
     @LoopFindElementSubmit(loop=1, action="取消订单")
     def touch_cancel_order(self):
         cancel_order = self.device.poco(
             type="android.widget.TextView", name="operateBtnList_Text_取消订单", text="取消订单"
         )
@@ -489,44 +493,14 @@
         submit_cancel_order = self.device.poco(
             type="android.widget.TextView", name="Button_Text_知道了", text="知道了"
         )
         submit_cancel_order.click()
 
     def get_order_detail_page_order_state(self) -> str:
         try:
-            order_detail = self.device.poco(
-                type="android.widget.TextView", name="android.widget.TextView", text="订单详情"
-            )
-            if order_detail.exists() is True:
-                try:
-                    canceled = self.device.poco(type="android.widget.TextView", name="android.widget.TextView",
-                                                text="已取消")
-                    if canceled.exists() is True:
-                        return "已取消"
-                except (Exception,):
-                    pass
-                try:
-                    to_payment = self.device.poco(
-                        type="android.widget.TextView", name="android.widget.TextView", text="去支付"
-                    )
-                    if to_payment.exists() is True:
-                        return "去支付"
-                except (Exception,):
-                    pass
-                try:
-                    to_payment = self.device.poco(
-                        type="android.widget.TextView", name="pcardLimit_Text_去支付", text="去支付"
-                    )
-                    if to_payment.exists() is True:
-                        return "去支付"
-                except (Exception,):
-                    pass
-        except (Exception,):
-            pass
-        try:
             file_name = join_path([get_images_dir(), "订单详情.png"])
             if is_exists(file_name):
                 temp = self.device.get_cv_template(file_name=file_name, threshold=0.9)
                 pos = self.device.exists(v=temp)
                 if pos:
                     try:
                         file_name = join_path([get_images_dir(), "订单详情_去支付.png"])
@@ -553,42 +527,72 @@
                     except (Exception,):
                         pass
             else:
                 # temp = (466, 173)  # Huawei Mate 20手机上对应的坐标位置，其他型号手机可能不是这个值
                 logger.warning("文件{}，没找到".format(file_name))
         except (Exception,):
             pass
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
         return ""
 
     @LoopFindElementObject(loop=20, action="从订单详情页【去支付】按钮", sleep=1)
     def get_to_payment_in_order_detail(self):
         try:
-            to_payment = self.device.poco(type="android.widget.TextView", name="pcardLimit_Text_去支付", text="去支付")
-            if to_payment.exists() is True:
-                return {"element": to_payment}
-        except (Exception,):
-            pass
-        try:
-            to_payment = self.device.poco(type="android.widget.TextView", name="android.widget.TextView", text="去支付")
-            if to_payment.exists() is True:
-                return {"element": to_payment}
-        except (Exception,):
-            pass
-        try:
             file_name = join_path([get_images_dir(), "订单详情_去支付.png"])
             if is_exists(file_name):
                 temp = self.device.get_cv_template(file_name=file_name, threshold=0.9)
                 pos = self.device.exists(v=temp)
                 if pos:
                     return {"pos": pos}
             else:
                 # temp = (873, 440)  # Huawei Mate 20手机上对应的坐标位置，其他型号手机可能不是这个值
                 logger.warning("文件{}，没找到".format(file_name))
         except (Exception,):
             pass
+        try:
+            to_payment = self.device.poco(type="android.widget.TextView", name="pcardLimit_Text_去支付", text="去支付")
+            if to_payment.exists() is True:
+                return {"element": to_payment}
+        except (Exception,):
+            pass
+        try:
+            to_payment = self.device.poco(type="android.widget.TextView", name="android.widget.TextView", text="去支付")
+            if to_payment.exists() is True:
+                return {"element": to_payment}
+        except (Exception,):
+            pass
         return dict()
 
     def is_need_login_with_my_page(self) -> bool:
         flag = False
         try:
             my_login = self.device.get_po(
                 type="android.widget.Button", name="ctrip.android.view:id/a", text="登录/注册"
@@ -683,81 +687,67 @@
                 text=payment_method
             )
             method.click()
             logger.info("点击选择【{}】".format(payment_method))
         except (Exception,):
             pass
 
+    @LoopExcute(action="检测是否出现支付小弹框", loop=20, sleep=1)
     def select_more_payment(self) -> bool:
         """
         当【同意并支付】后，特殊情况下，会出现支付小弹框，这个时候需要先判断是否存在小框，如果存在，则切换到通用支付选择界面
         """
-        flag = False
-        # 这个地方容易卡卡住，采用透底的方案执行该逻辑
-        for _ in range(20):
-            # 1. 检测是否到了安全收银台，安全收银台的定位特征是：【安全收银台】|【银行卡支付】
-            try:
-                safe_cash = self.device.get_po(
-                    type="android.widget.TextView", name="android.widget.TextView", text="安全收银台"
-                )
-                if safe_cash.exists() is True:
-                    flag = True
-                    time.sleep(3)
-                    break
-            except (Exception,):
-                pass
-            try:
-                bank_card_payment = self.device.get_po(
-                    type="android.widget.TextView", name="android.widget.TextView", text="银行卡支付"
-                )
-                if bank_card_payment.exists() is True:
-                    flag = True
-                    time.sleep(3)
-                    break
-            except (Exception,):
-                pass
-            # 2. 检测到小弹框， 定位特征是：【更多付款方式】
-            try:
-                more_payment_type = self.device.get_po(
-                    type="android.view.ViewGroup ", name="更多付款方式", desc="更多付款方式"
-                )
-                if more_payment_type.exists() is True:
-                    logger.warning("元素定位方式检测到有小弹框，需要点击【更多付款方式】")
-                    more_payment_type.click()
+        # 1. 检测到小弹框， 图像识别定位特征是：【更多付款方式】
+        try:
+            file_name = join_path([get_images_dir(), "更多付款方式.png"])
+            if is_exists(file_name):
+                temp = self.device.get_cv_template(file_name=file_name, threshold=0.9)
+                if temp:
+                    logger.warning("图像识别方式检测到有小弹框，需要点击【更多付款方式】")
+                    self.device.touch(v=temp)
                     time.sleep(1)
-                    try:
-                        more_payment_type_inner = self.device.get_po(
-                            type="android.view.ViewGroup ", name="更多付款方式", desc="更多付款方式"
-                        )
-                        if more_payment_type_inner.exists() is False:
-                            flag = True
-                            time.sleep(3)
-                            break
-                    except (Exception,):
-                        pass
-            except (Exception,):
-                pass
-            # 3. 检测到小弹框， 图像识别定位特征是：【更多付款方式】
-            try:
-                file_name = join_path([get_images_dir(), "更多付款方式.png"])
-                if is_exists(file_name):
-                    temp = self.device.get_cv_template(file_name=file_name, threshold=0.9)
-                    if temp:
-                        logger.warning("图像识别方式检测到有小弹框，需要点击【更多付款方式】")
-                        self.device.touch(v=temp)
+                    temp_inner = self.device.get_cv_template(file_name=file_name)
+                    if not temp_inner:
                         time.sleep(1)
-                        temp_inner = self.device.get_cv_template(file_name=file_name)
-                        if not temp_inner:
-                            flag = True
-                            time.sleep(3)
-                            break
-            except (Exception,):
-                pass
-            time.sleep(1)
-        return flag
+                        return True
+        except (Exception,):
+            pass
+        # 2. 检测是否到了安全收银台，安全收银台的定位特征是：【安全收银台】|【银行卡支付】
+        try:
+            safe_cash = self.device.get_po(
+                type="android.widget.TextView", name="android.widget.TextView", text="安全收银台"
+            )
+            if safe_cash.exists() is True:
+                time.sleep(1)
+                return True
+        except (Exception,):
+            pass
+        try:
+            bank_card_payment = self.device.get_po(
+                type="android.widget.TextView", name="android.widget.TextView", text="银行卡支付"
+            )
+            if bank_card_payment.exists() is True:
+                time.sleep(1)
+                return True
+        except (Exception,):
+            pass
+        # 3. 检测到小弹框， 定位特征是：【更多付款方式】
+        try:
+            more_payment_type = self.device.get_po(
+                type="android.view.ViewGroup ", name="更多付款方式", desc="更多付款方式"
+            )
+            if more_payment_type.exists() is True:
+                logger.warning("元素定位方式检测到有小弹框，需要点击【更多付款方式】")
+                more_payment_type.click()
+                time.sleep(1)
+                return True
+        except (Exception,):
+            pass
+        time.sleep(1)
+        return False
 
     def __get_wallet_element(self) -> UIObjectProxy:
         return self.device.get_po(
             type="android.widget.TextView", name="android.widget.TextView", textMatches=r'^钱包.*'
         )
 
     @SleepWait(wait_time=1)
```

### Comparing `ctrip-app-ui-0.5.1/capp_ui/fee.py` & `ctrip-app-ui-0.5.2/capp_ui/fee.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.5.1/capp_ui/libs.py` & `ctrip-app-ui-0.5.2/capp_ui/libs.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.5.1/capp_ui/mobile_terminals.py` & `ctrip-app-ui-0.5.2/capp_ui/mobile_terminals.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.5.1/capp_ui/platforms.py` & `ctrip-app-ui-0.5.2/capp_ui/platforms.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.5.1/capp_ui/test.py` & `ctrip-app-ui-0.5.2/capp_ui/test.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.5.1/capp_ui/utils.py` & `ctrip-app-ui-0.5.2/capp_ui/utils.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.5.1/capp_ui/validators.py` & `ctrip-app-ui-0.5.2/capp_ui/validators.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.5.1/setup.py` & `ctrip-app-ui-0.5.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 # Copyright ©2011-2024. Hunan xxxxxxx Company limited. All rights reserved.
 # ---------------------------------------------------------------------------------------------------------
 """
 from setuptools import setup, find_packages
 
 setup(
     name='ctrip-app-ui',
-    version='0.5.1',
+    version='0.5.2',
     description='This is my ctrip app ui package',
     long_description='This is my ctrip app ui package',
     author='ckf10000',
     author_email='ckf10000@sina.com',
     url='https://github.com/ckf10000/ctrip-app-ui',
     packages=find_packages(),
     install_requires=[
```

