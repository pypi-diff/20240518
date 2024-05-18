# Comparing `tmp/PayNexus-0.2.0-py3-none-any.whl.zip` & `tmp/PayNexus-0.2.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 12547 bytes, number of entries: 8
+Zip file size: 14276 bytes, number of entries: 8
 -rw-rw-rw-  2.0 fat    14926 b- defN 24-May-17 23:25 paynexus/Colors.py
--rw-rw-rw-  2.0 fat       69 b- defN 24-May-18 05:33 paynexus/__init__.py
--rw-rw-rw-  2.0 fat    21774 b- defN 24-May-18 05:02 paynexus/main.py
--rw-rw-rw-  2.0 fat     1324 b- defN 24-May-18 05:33 PayNexus-0.2.0.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     3796 b- defN 24-May-18 05:33 PayNexus-0.2.0.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 24-May-18 05:33 PayNexus-0.2.0.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        9 b- defN 24-May-18 05:33 PayNexus-0.2.0.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      615 b- defN 24-May-18 05:33 PayNexus-0.2.0.dist-info/RECORD
-8 files, 42605 bytes uncompressed, 11481 bytes compressed:  73.1%
+-rw-rw-rw-  2.0 fat       69 b- defN 24-May-18 06:12 paynexus/__init__.py
+-rw-rw-rw-  2.0 fat    21636 b- defN 24-May-18 05:40 paynexus/main.py
+-rw-rw-rw-  2.0 fat     1324 b- defN 24-May-18 06:12 PayNexus-0.2.1.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat    10574 b- defN 24-May-18 06:12 PayNexus-0.2.1.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 24-May-18 06:12 PayNexus-0.2.1.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        9 b- defN 24-May-18 06:12 PayNexus-0.2.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      616 b- defN 24-May-18 06:12 PayNexus-0.2.1.dist-info/RECORD
+8 files, 49246 bytes uncompressed, 13210 bytes compressed:  73.2%
```

## zipnote {}

```diff
@@ -3,23 +3,23 @@
 
 Filename: paynexus/__init__.py
 Comment: 
 
 Filename: paynexus/main.py
 Comment: 
 
-Filename: PayNexus-0.2.0.dist-info/LICENSE
+Filename: PayNexus-0.2.1.dist-info/LICENSE
 Comment: 
 
-Filename: PayNexus-0.2.0.dist-info/METADATA
+Filename: PayNexus-0.2.1.dist-info/METADATA
 Comment: 
 
-Filename: PayNexus-0.2.0.dist-info/WHEEL
+Filename: PayNexus-0.2.1.dist-info/WHEEL
 Comment: 
 
-Filename: PayNexus-0.2.0.dist-info/top_level.txt
+Filename: PayNexus-0.2.1.dist-info/top_level.txt
 Comment: 
 
-Filename: PayNexus-0.2.0.dist-info/RECORD
+Filename: PayNexus-0.2.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## paynexus/__init__.py

```diff
@@ -1,4 +1,4 @@
 from .main import *
 from .Colors import *
 
-__version__ = '0.2.0'
+__version__ = '0.2.1'
```

## paynexus/main.py

```diff
@@ -77,15 +77,15 @@
     return decrypted_data
 
 
 class PayPay:
     def __init__(self, phone: str = None, password: str = None, client_uuid: str = str(uuid.uuid4()), token: str = None,
                  proxy: dict = None, session_save="./paypay_login.date", debug=False, webhook=None,
                  session_auto_save=False, session_check_interval=random.randint(3, 7),
-                 session_check_interval_delay_min=0, session_check_interval_delay_max=0):
+                 session_check_interval_delay=[0, 0]):
         self.session = requests.Session()
         self.proxy = proxy
         self.uuuid = client_uuid
         self.phone = phone
         self.pas = password
         self.debug = debug
         self.webhook = webhook
@@ -136,16 +136,15 @@
                                         proxies=self.proxy, timeout=(10, 5)).ok:
                     raise "ログインに失敗"
             except Exception as e:
                 self.color_print(f"ログイン失敗", [Color.RED])
                 raise e
         if session_auto_save:
             thread = threading.Thread(target=self.session_auto_saver, kwargs={"interval": session_check_interval,
-                                                                              "min_d": session_check_interval_delay_min,
-                                                                              "max_d": session_check_interval_delay_max})
+                                                                              "delay": session_check_interval_delay})
             thread.start()
             return
 
     def login(self, otp: str):
         otpj = {
             "scope": "SIGN_IN",
             "client_uuid": self.uuuid,
@@ -362,15 +361,16 @@
             "paymentMethodId": "106177237",
             "paymentCodeSessionId": str(uuid.uuid4()),
         }
         cpotc = self.session.post("https://www.paypay.ne.jp/app/v2/bff/createPaymentOneTimeCodeForHome",
                                   headers=headers, proxies=self.proxy, json=cpotcj)
         return cpotc.json()
 
-    def session_auto_saver(self, interval, min_d, max_d):
+    def session_auto_saver(self, interval, delay):
+        min_d, max_d = delay
         from term_printer import Color
         if self.uuuid is None:
             self.color_print(f"自動再ログイン機能はuuid(client_uuid)が指定されていないため利用できません",
                              [Color.YELLOW])
             return
         interval = interval * 60
         while True:
```

## Comparing `PayNexus-0.2.0.dist-info/LICENSE` & `PayNexus-0.2.1.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `PayNexus-0.2.0.dist-info/RECORD` & `PayNexus-0.2.1.dist-info/RECORD`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,8 @@
 paynexus/Colors.py,sha256=wa117RL7OmyxNWNhXxZGeMrUOMcG80JUUWo18B1JSpI,14926
-paynexus/__init__.py,sha256=E75DwD7Jy3Pp0zpeXBkRiM8Vp36FKxr6adqGnTbUAss,69
-paynexus/main.py,sha256=qfNLAjlOWBHMsNrjfcYMpjL2svVyuITacRnV01Q2ZAM,21774
-PayNexus-0.2.0.dist-info/LICENSE,sha256=IigZVe3wmZnBT1Jla6C72FmsnJzbG5MdBdP_AfJeXDQ,1324
-PayNexus-0.2.0.dist-info/METADATA,sha256=HGkpHYAKW2nsWkgtosjAX8p4XT3Vh-LS6S9-DGgbpNA,3796
-PayNexus-0.2.0.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-PayNexus-0.2.0.dist-info/top_level.txt,sha256=IG1-TEiS1lUSzD_9mINwssp3RTwRR2XXMoey5rqGLoo,9
-PayNexus-0.2.0.dist-info/RECORD,,
+paynexus/__init__.py,sha256=NduBWn0MVaOn6105XxWmbxGVV4kWChJgnoNutB1WB-0,69
+paynexus/main.py,sha256=aTFEElwvuy-zxFEAMnBtBbIbULBvwNZbh_XeS-za2D0,21636
+PayNexus-0.2.1.dist-info/LICENSE,sha256=IigZVe3wmZnBT1Jla6C72FmsnJzbG5MdBdP_AfJeXDQ,1324
+PayNexus-0.2.1.dist-info/METADATA,sha256=i6uTxRqpV4O9DDFGTc0i81Ny8gsekr8q3aJn0TOUHZg,10574
+PayNexus-0.2.1.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+PayNexus-0.2.1.dist-info/top_level.txt,sha256=IG1-TEiS1lUSzD_9mINwssp3RTwRR2XXMoey5rqGLoo,9
+PayNexus-0.2.1.dist-info/RECORD,,
```

