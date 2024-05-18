# Comparing `tmp/zhmiscellany-2.0.8-py3-none-any.whl.zip` & `tmp/zhmiscellany-2.0.9-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,20 +1,20 @@
-Zip file size: 20138 bytes, number of entries: 18
+Zip file size: 20142 bytes, number of entries: 18
 -rw-rw-rw-  2.0 fat      236 b- defN 24-Apr-15 13:40 zhmiscellany/__init__.py
 -rw-rw-rw-  2.0 fat     6520 b- defN 23-Dec-08 14:13 zhmiscellany/_discord_supportfuncs.py
 -rw-rw-rw-  2.0 fat      673 b- defN 23-Nov-05 00:34 zhmiscellany/_misc_supportfuncs.py
 -rw-rw-rw-  2.0 fat       81 b- defN 23-Nov-01 22:45 zhmiscellany/dict.py
 -rw-rw-rw-  2.0 fat    15608 b- defN 24-Mar-07 15:37 zhmiscellany/discord.py
 -rw-rw-rw-  2.0 fat     4256 b- defN 23-Nov-01 20:01 zhmiscellany/fileio.py
 -rw-rw-rw-  2.0 fat      338 b- defN 23-Oct-31 21:16 zhmiscellany/image.py
 -rw-rw-rw-  2.0 fat      854 b- defN 23-Nov-14 14:55 zhmiscellany/list.py
 -rw-rw-rw-  2.0 fat      632 b- defN 23-Nov-18 07:12 zhmiscellany/math.py
 -rw-rw-rw-  2.0 fat     4531 b- defN 24-Apr-15 16:39 zhmiscellany/misc.py
--rw-rw-rw-  2.0 fat     1685 b- defN 24-Apr-15 15:15 zhmiscellany/netio.py
+-rw-rw-rw-  2.0 fat     1687 b- defN 24-May-18 08:24 zhmiscellany/netio.py
 -rw-rw-rw-  2.0 fat     3795 b- defN 24-Apr-28 06:17 zhmiscellany/pipes.py
 -rw-rw-rw-  2.0 fat      761 b- defN 24-Feb-12 17:09 zhmiscellany/processing.py
 -rw-rw-rw-  2.0 fat     2412 b- defN 23-Nov-18 07:28 zhmiscellany/string.py
--rw-rw-rw-  2.0 fat    18861 b- defN 24-Apr-28 06:18 zhmiscellany-2.0.8.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 24-Apr-28 06:18 zhmiscellany-2.0.8.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       13 b- defN 24-Apr-28 06:18 zhmiscellany-2.0.8.dist-info/top_level.txt
--rw-rw-r--  2.0 fat     1441 b- defN 24-Apr-28 06:18 zhmiscellany-2.0.8.dist-info/RECORD
-18 files, 62789 bytes uncompressed, 17790 bytes compressed:  71.7%
+-rw-rw-rw-  2.0 fat    18861 b- defN 24-May-18 08:25 zhmiscellany-2.0.9.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 24-May-18 08:25 zhmiscellany-2.0.9.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       13 b- defN 24-May-18 08:25 zhmiscellany-2.0.9.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat     1441 b- defN 24-May-18 08:25 zhmiscellany-2.0.9.dist-info/RECORD
+18 files, 62791 bytes uncompressed, 17794 bytes compressed:  71.7%
```

## zipnote {}

```diff
@@ -36,20 +36,20 @@
 
 Filename: zhmiscellany/processing.py
 Comment: 
 
 Filename: zhmiscellany/string.py
 Comment: 
 
-Filename: zhmiscellany-2.0.8.dist-info/METADATA
+Filename: zhmiscellany-2.0.9.dist-info/METADATA
 Comment: 
 
-Filename: zhmiscellany-2.0.8.dist-info/WHEEL
+Filename: zhmiscellany-2.0.9.dist-info/WHEEL
 Comment: 
 
-Filename: zhmiscellany-2.0.8.dist-info/top_level.txt
+Filename: zhmiscellany-2.0.9.dist-info/top_level.txt
 Comment: 
 
-Filename: zhmiscellany-2.0.8.dist-info/RECORD
+Filename: zhmiscellany-2.0.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## zhmiscellany/netio.py

```diff
@@ -27,15 +27,15 @@
         response = requests.get(url, stream=True, headers=headers)
     else:
         response = requests.get(url, stream=True)
     if response.status_code == 200:
 
         # Save the file
         with open(destination_path, 'wb') as file:
-            for chunk in response.iter_content(chunk_size=128):
+            for chunk in response.iter_content(chunk_size=2**12):
                 file.write(chunk)
 
         return destination_path
 
     else:
         raise Exception(f"Failed to download the file. Status code: {response.status_code}")
```

## Comparing `zhmiscellany-2.0.8.dist-info/METADATA` & `zhmiscellany-2.0.9.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zhmiscellany
-Version: 2.0.8
+Version: 2.0.9
 Summary: A collection of useful/interesting python libraries made by zh.
 Home-page: https://discord.gg/ThBBAuueVJ
 Author: zh
 Author-email: imnotgivingmyemailjustaddmeondiscordmydiscordisz_h_@zh.com
 Project-URL: Bug Tracker, https://github.com/zen-ham/zhmiscellany/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

## Comparing `zhmiscellany-2.0.8.dist-info/RECORD` & `zhmiscellany-2.0.9.dist-info/RECORD`

 * *Files 7% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 zhmiscellany/dict.py,sha256=0BZJ5eK-MurAHYV1OPa0jdGTr-QEWos7ZM0npb-tN9I,81
 zhmiscellany/discord.py,sha256=Re-fUdc_OA-9tzvd3VX_w7lBNvFpg3Tg5mVyIQ83IKA,15608
 zhmiscellany/fileio.py,sha256=q5noOhvPxyHxSy56sawW0X91qwHM2xuU8CYzfJN5O08,4256
 zhmiscellany/image.py,sha256=uOXFcGG1FhvNeCU7dm6DYxefh6suiL8qg8qtAVyezew,338
 zhmiscellany/list.py,sha256=2kqsscSFXEanmEdR1NuwWaf2l8nPTDUgRyrfL1snoRg,854
 zhmiscellany/math.py,sha256=v2WmHdKrwsrY08E6yUgb0nPHbTuyrljRdgUMw5uqu3U,632
 zhmiscellany/misc.py,sha256=JlibUEtNHc3nHDnlgyOE3050SIQkcMMedPK8WZookNU,4531
-zhmiscellany/netio.py,sha256=4dKBJp-fq_jnuDcwrag6kH7WZncnERPPtuCmGcdFAt0,1685
+zhmiscellany/netio.py,sha256=UiMQFsdpPx2Kst-YDxYrz_Ivsnq455LNTKQRCi-aZwY,1687
 zhmiscellany/pipes.py,sha256=PxO4aykFzC60xbTQuc66KzZYIxiW0KPebXZbncD2HcU,3795
 zhmiscellany/processing.py,sha256=pE2LVtaZwBvWgd6Xx0S_ZT0WhcKr6GtBhjAfbAflSYo,761
 zhmiscellany/string.py,sha256=2xL_rbJeiGH14k_JkXWUp-oBN30Ltl9-bZk0eHUPltA,2412
-zhmiscellany-2.0.8.dist-info/METADATA,sha256=1qJd_h06s6uGTYeDNZrHvyuv12f-vpC4icuQ1PI68EE,18861
-zhmiscellany-2.0.8.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-zhmiscellany-2.0.8.dist-info/top_level.txt,sha256=ioDtsrevCI52rTxZntMPljRIBsZs73tD0hI00HektiE,13
-zhmiscellany-2.0.8.dist-info/RECORD,,
+zhmiscellany-2.0.9.dist-info/METADATA,sha256=vGFDjFDK2s6iINdYZPtEQYoh0jssms2t7YbRtsZC1JE,18861
+zhmiscellany-2.0.9.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+zhmiscellany-2.0.9.dist-info/top_level.txt,sha256=ioDtsrevCI52rTxZntMPljRIBsZs73tD0hI00HektiE,13
+zhmiscellany-2.0.9.dist-info/RECORD,,
```

