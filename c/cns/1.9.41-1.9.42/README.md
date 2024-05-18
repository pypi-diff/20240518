# Comparing `tmp/cns-1.9.41-py3-none-any.whl.zip` & `tmp/cns-1.9.42-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 963139 bytes, number of entries: 27
+Zip file size: 964548 bytes, number of entries: 27
 -rw-rw-rw-  2.0 fat   151040 b- defN 23-Sep-24 05:36 cns/DataX.cp36-win32.pyd
 -rw-rw-rw-  2.0 fat   189440 b- defN 23-Sep-24 05:36 cns/DataX.cp36-win_amd64.pyd
 -rw-rw-rw-  2.0 fat   189952 b- defN 23-Sep-24 05:36 cns/DataX.cp39-win_amd64.pyd
 -rw-rw-rw-  2.0 fat    82944 b- defN 23-Jun-02 15:12 cns/DateTimeX.cp36-win32.pyd
 -rw-rw-rw-  2.0 fat    99840 b- defN 23-Jun-02 15:11 cns/DateTimeX.cp36-win_amd64.pyd
 -rw-rw-rw-  2.0 fat    88576 b- defN 23-Jun-02 15:13 cns/DateTimeX.cp39-win_amd64.pyd
 -rw-rw-rw-  2.0 fat   117248 b- defN 23-Oct-10 13:48 cns/ExcelX.cp36-win32.pyd
@@ -15,15 +15,15 @@
 -rw-rw-rw-  2.0 fat    74240 b- defN 23-Jun-16 07:35 cns/SQLstrX.cp39-win_amd64.pyd
 -rw-rw-rw-  2.0 fat    80896 b- defN 24-Mar-25 09:33 cns/TextX.cp36-win_amd64.pyd
 -rw-rw-rw-  2.0 fat    65536 b- defN 23-Jun-23 11:02 cns/TextX.cp39-win_amd64.pyd
 -rw-rw-rw-  2.0 fat      645 b- defN 24-Apr-28 05:37 cns/__init__.py
 -rw-rw-rw-  2.0 fat    68608 b- defN 23-Aug-11 08:45 cns/cmdX.cp36-win32.pyd
 -rw-rw-rw-  2.0 fat   108032 b- defN 24-Apr-13 08:42 cns/cmdX.cp36-win_amd64.pyd
 -rw-rw-rw-  2.0 fat    89088 b- defN 23-Aug-11 08:45 cns/cmdX.cp39-win_amd64.pyd
--rw-rw-rw-  2.0 fat   136192 b- defN 24-May-17 16:05 cns/sqlX.cp36-win_amd64.pyd
+-rw-rw-rw-  2.0 fat   140288 b- defN 24-May-18 01:06 cns/sqlX.cp36-win_amd64.pyd
 -rw-rw-rw-  2.0 fat    87040 b- defN 24-Apr-29 08:37 cns/strX.cp36-win_amd64.pyd
--rw-rw-rw-  2.0 fat      473 b- defN 24-May-17 16:05 cns-1.9.41.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     2023 b- defN 24-May-17 16:05 cns-1.9.41.dist-info/METADATA
--rw-rw-rw-  2.0 fat       97 b- defN 24-May-17 16:05 cns-1.9.41.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        4 b- defN 24-May-17 16:05 cns-1.9.41.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat     2232 b- defN 24-May-17 16:05 cns-1.9.41.dist-info/RECORD
-27 files, 2187631 bytes uncompressed, 959613 bytes compressed:  56.2%
+-rw-rw-rw-  2.0 fat      473 b- defN 24-May-18 01:09 cns-1.9.42.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     2023 b- defN 24-May-18 01:09 cns-1.9.42.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       97 b- defN 24-May-18 01:09 cns-1.9.42.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        4 b- defN 24-May-18 01:09 cns-1.9.42.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat     2232 b- defN 24-May-18 01:09 cns-1.9.42.dist-info/RECORD
+27 files, 2191727 bytes uncompressed, 961022 bytes compressed:  56.2%
```

## zipnote {}

```diff
@@ -60,23 +60,23 @@
 
 Filename: cns/sqlX.cp36-win_amd64.pyd
 Comment: 
 
 Filename: cns/strX.cp36-win_amd64.pyd
 Comment: 
 
-Filename: cns-1.9.41.dist-info/LICENSE
+Filename: cns-1.9.42.dist-info/LICENSE
 Comment: 
 
-Filename: cns-1.9.41.dist-info/METADATA
+Filename: cns-1.9.42.dist-info/METADATA
 Comment: 
 
-Filename: cns-1.9.41.dist-info/WHEEL
+Filename: cns-1.9.42.dist-info/WHEEL
 Comment: 
 
-Filename: cns-1.9.41.dist-info/top_level.txt
+Filename: cns-1.9.42.dist-info/top_level.txt
 Comment: 
 
-Filename: cns-1.9.41.dist-info/RECORD
+Filename: cns-1.9.42.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `cns-1.9.41.dist-info/METADATA` & `cns-1.9.42.dist-info/METADATA`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cns
-Version: 1.9.41
+Version: 1.9.42
 Summary: cns工具包
 Home-page: https://cns.ink/example
 Author: Rambo
 Author-email: 6566666@qq.com
 License: Copyright (C) 2023 CNS. All Rights Reserved. See LICENSE for license.
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

## Comparing `cns-1.9.41.dist-info/RECORD` & `cns-1.9.42.dist-info/RECORD`

 * *Files 7% similar despite different names*

```diff
@@ -14,14 +14,14 @@
 cns/SQLstrX.cp39-win_amd64.pyd,sha256=B0wq2UBpInSyGEq6aGOvKiqwAov8_ynHtlkPnaYav8k,74240
 cns/TextX.cp36-win_amd64.pyd,sha256=PYVrQEs7reVMhs5Incl0q9IYBZDEmOdKA7EDMdKY_Q4,80896
 cns/TextX.cp39-win_amd64.pyd,sha256=tJkutc00Vya2KBtXFWGcCm0wOSt9vvAm_7cZBsB1DgE,65536
 cns/__init__.py,sha256=mMJGrPRMKFqzANkjaICV4uzkGsbJsXQ62ToQujXJr-Y,645
 cns/cmdX.cp36-win32.pyd,sha256=f4TcE849qF5PUxcmAf3uGHJwNPk0SNk9xilxDv9j7ek,68608
 cns/cmdX.cp36-win_amd64.pyd,sha256=12GapWmmQ-4PijruUOpF-SEwv5jYJOfeF0rZqrJGftg,108032
 cns/cmdX.cp39-win_amd64.pyd,sha256=8o8LoRMpTyJhvxc3bFAGJcJGW7hnKLHW5Ni-ooOvqYQ,89088
-cns/sqlX.cp36-win_amd64.pyd,sha256=VG8-WMOjK9ypH0XYqiUaMADvVfryoFD3a-7mlWaoDDA,136192
+cns/sqlX.cp36-win_amd64.pyd,sha256=-QjjqrrK-HSN4RcUyM0K_oqUhXLt9AiZjnRgZNPKTEE,140288
 cns/strX.cp36-win_amd64.pyd,sha256=379priq_uLDAF4xgTdz2DKrGi5Q5YMHX7psaPOlxZJo,87040
-cns-1.9.41.dist-info/LICENSE,sha256=OCcV9iTKhNBVidknwiPS8X-OLMdgbpsuUL9EzN6Q5zI,473
-cns-1.9.41.dist-info/METADATA,sha256=dQJ8vf7Dy35WVF3QVUxG1mDudsSds6v3KhypE9-CJEE,2023
-cns-1.9.41.dist-info/WHEEL,sha256=YUYzQ6UQdoqxXjimOitTqynltBCkwY6qlTfTh2IzqQU,97
-cns-1.9.41.dist-info/top_level.txt,sha256=oA9qczli9LkRhNJ77Ah4syjSkuiqmSaR2pTif57e9pM,4
-cns-1.9.41.dist-info/RECORD,,
+cns-1.9.42.dist-info/LICENSE,sha256=OCcV9iTKhNBVidknwiPS8X-OLMdgbpsuUL9EzN6Q5zI,473
+cns-1.9.42.dist-info/METADATA,sha256=TIdYCSgrvZ146EXkcwuQ6XqtSY_OiKBk_r87IFfIDFI,2023
+cns-1.9.42.dist-info/WHEEL,sha256=YUYzQ6UQdoqxXjimOitTqynltBCkwY6qlTfTh2IzqQU,97
+cns-1.9.42.dist-info/top_level.txt,sha256=oA9qczli9LkRhNJ77Ah4syjSkuiqmSaR2pTif57e9pM,4
+cns-1.9.42.dist-info/RECORD,,
```

