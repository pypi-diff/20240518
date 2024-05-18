# Comparing `tmp/tdrpa.tdcore-1.1.29-py39-none-win_amd64.whl.zip` & `tmp/tdrpa.tdcore-1.1.30-py39-none-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,22 +1,22 @@
-Zip file size: 499331 bytes, number of entries: 20
--rw-rw-rw-  2.0 fat   640000 b- defN 24-Apr-06 07:44 tdrpa/bot.exe
--rw-rw-rw-  2.0 fat   594944 b- defN 24-Apr-06 07:44 tdrpa/tdcore.cp39-win_amd64.pyd
+Zip file size: 500442 bytes, number of entries: 20
+-rw-rw-rw-  2.0 fat   640000 b- defN 24-May-17 03:46 tdrpa/bot.exe
+-rw-rw-rw-  2.0 fat   598016 b- defN 24-May-17 03:46 tdrpa/tdcore.cp39-win_amd64.pyd
 -rw-rw-rw-  2.0 fat      129 b- defN 24-Apr-06 07:32 tdrpa/tdcore/__init__.pyi
 -rw-rw-rw-  2.0 fat        0 b- defN 24-Apr-06 00:55 tdrpa/tdcore/locator/__init__.pyi
 -rw-rw-rw-  2.0 fat      265 b- defN 24-Apr-06 07:37 tdrpa/tdcore/locator/locatorWindows.pyi
 -rw-rw-rw-  2.0 fat      264 b- defN 24-Apr-06 01:35 tdrpa/tdcore/locator/tdObject.pyi
 -rw-rw-rw-  2.0 fat        0 b- defN 24-Apr-06 00:55 tdrpa/tdcore/log/__init__.pyi
 -rw-rw-rw-  2.0 fat       42 b- defN 24-Apr-06 01:29 tdrpa/tdcore/log/log.pyi
 -rw-rw-rw-  2.0 fat    11357 b- defN 23-Jan-16 01:15 tdrpa/tdcore-license/LICENSE
 -rw-rw-rw-  2.0 fat     1473 b- defN 23-Sep-05 03:08 tdrpa/tdcore-license/infi.systray/LICENSE.txt
 -rw-rw-rw-  2.0 fat     1064 b- defN 23-Sep-05 03:09 tdrpa/tdcore-license/keyboard/LICENSE.txt
 -rw-rw-rw-  2.0 fat     1548 b- defN 23-Sep-05 03:10 tdrpa/tdcore-license/psutil/LICENSE.txt
 -rw-rw-rw-  2.0 fat        0 b- defN 23-Aug-30 09:52 tdrpa/tdcore-license/pywin32/none
 -rw-rw-rw-  2.0 fat    10142 b- defN 23-Sep-05 03:11 tdrpa/tdcore-license/requests/LICENSE.txt
 -rw-rw-rw-  2.0 fat     1060 b- defN 23-Sep-05 03:12 tdrpa/tdcore-license/tzlocal/LICENSE.txt
 -rw-rw-rw-  2.0 fat    11336 b- defN 23-Sep-05 03:13 tdrpa/tdcore-license/uiautomation/LICENSE.txt
--rw-rw-rw-  2.0 fat      638 b- defN 24-Apr-06 07:44 tdrpa.tdcore-1.1.29.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 24-Apr-06 07:44 tdrpa.tdcore-1.1.29.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        6 b- defN 24-Apr-06 07:44 tdrpa.tdcore-1.1.29.dist-info/top_level.txt
--rw-rw-r--  2.0 fat     1764 b- defN 24-Apr-06 07:44 tdrpa.tdcore-1.1.29.dist-info/RECORD
-20 files, 1276124 bytes uncompressed, 496407 bytes compressed:  61.1%
+-rw-rw-rw-  2.0 fat      638 b- defN 24-May-17 03:46 tdrpa.tdcore-1.1.30.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 24-May-17 03:46 tdrpa.tdcore-1.1.30.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        6 b- defN 24-May-17 03:46 tdrpa.tdcore-1.1.30.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat     1764 b- defN 24-May-17 03:46 tdrpa.tdcore-1.1.30.dist-info/RECORD
+20 files, 1279196 bytes uncompressed, 497518 bytes compressed:  61.1%
```

## zipnote {}

```diff
@@ -42,20 +42,20 @@
 
 Filename: tdrpa/tdcore-license/tzlocal/LICENSE.txt
 Comment: 
 
 Filename: tdrpa/tdcore-license/uiautomation/LICENSE.txt
 Comment: 
 
-Filename: tdrpa.tdcore-1.1.29.dist-info/METADATA
+Filename: tdrpa.tdcore-1.1.30.dist-info/METADATA
 Comment: 
 
-Filename: tdrpa.tdcore-1.1.29.dist-info/WHEEL
+Filename: tdrpa.tdcore-1.1.30.dist-info/WHEEL
 Comment: 
 
-Filename: tdrpa.tdcore-1.1.29.dist-info/top_level.txt
+Filename: tdrpa.tdcore-1.1.30.dist-info/top_level.txt
 Comment: 
 
-Filename: tdrpa.tdcore-1.1.29.dist-info/RECORD
+Filename: tdrpa.tdcore-1.1.30.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## tdrpa/bot.exe

### objdump

```diff
@@ -6,15 +6,15 @@
 Characteristics 0x22e
 	executable
 	line numbers stripped
 	symbols stripped
 	large address aware
 	debugging information removed
 
-Time/Date		Sat Apr  6 07:44:25 2024
+Time/Date		Fri May 17 03:46:25 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	2
 MinorLinkerVersion	41
 SizeOfCode		0000000000078c00
 SizeOfInitializedData	000000000009c000
 SizeOfUninitializedData	0000000000003400
 AddressOfEntryPoint	00000000000010f6
@@ -27,15 +27,15 @@
 MajorImageVersion	0
 MinorImageVersion	0
 MajorSubsystemVersion	5
 MinorSubsystemVersion	2
 Win32Version		00000000
 SizeOfImage		000a7000
 SizeOfHeaders		00000400
-CheckSum		000902ba
+CheckSum		0009d8a7
 Subsystem		00000002	(Windows GUI)
 DllCharacteristics	00000160
 					HIGH_ENTROPY_VA
 					DYNAMIC_BASE
 					NX_COMPAT
 SizeOfStackReserve	0000000000968000
 SizeOfStackCommit	0000000000001000
```

## Comparing `tdrpa.tdcore-1.1.29.dist-info/METADATA` & `tdrpa.tdcore-1.1.30.dist-info/METADATA`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tdrpa.tdcore
-Version: 1.1.29
+Version: 1.1.30
 Summary: RPA SDK for software developers. Supports Python3.7+, Windows x64
 Home-page: https://tdrpa.thingswell.cn
 Author: tdrpa
 Author-email: armstrong.wang@gmail.com
 License: Apache 2.0
 Keywords: RPA,tdRPA,uiautomation,uia
 Platform: Windows Only
```

## Comparing `tdrpa.tdcore-1.1.29.dist-info/RECORD` & `tdrpa.tdcore-1.1.30.dist-info/RECORD`

 * *Files 16% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-tdrpa/bot.exe,sha256=eEAtRVuxOjF540WmoxgJlKwSuTypH7eqEHShRc9IldI,640000
-tdrpa/tdcore.cp39-win_amd64.pyd,sha256=MLvjcGqNgqiuAyHqR36FdYTNAFoiGSuhvHPSkqjVyQU,594944
+tdrpa/bot.exe,sha256=2fRgWxDHFifOGXeJ6Vj1L5PYfF0RGt30WkSsnJjm-QA,640000
+tdrpa/tdcore.cp39-win_amd64.pyd,sha256=rbFTLhf7d5GBxSzBW3zSsSJ3iJF64v1j5m22cMUhXNw,598016
 tdrpa/tdcore/__init__.pyi,sha256=HqSPrXJTwOWqny037hFS7WQoE8tFeOfi1pz-0La1oRA,129
 tdrpa/tdcore/locator/__init__.pyi,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 tdrpa/tdcore/locator/locatorWindows.pyi,sha256=4doiswkToDtOV5MKbkuX8gC-H6jOtLeUnraQLCaaBrA,265
 tdrpa/tdcore/locator/tdObject.pyi,sha256=bL4-DFpaE17uuCuN9ksd02DzNykVceBJsPSyw3wtSpI,264
 tdrpa/tdcore/log/__init__.pyi,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 tdrpa/tdcore/log/log.pyi,sha256=s9ToZ5GiIsNUHdMGOOy1le3zA9t0uxcn-9UoPxFjHT8,42
 tdrpa/tdcore-license/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
 tdrpa/tdcore-license/infi.systray/LICENSE.txt,sha256=-9Uy-R2R7bZjSp8m31SUjOX8_6Og1laqYUB8npdzUHI,1473
 tdrpa/tdcore-license/keyboard/LICENSE.txt,sha256=Hn56SBfvVDq2tZ90AC1Xuo6N5iIeYiY_AnP447yOId8,1064
 tdrpa/tdcore-license/psutil/LICENSE.txt,sha256=uJwGOzeG4o4MCjjxkx22H-015p3SopZvvs_-4PRsjRA,1548
 tdrpa/tdcore-license/pywin32/none,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 tdrpa/tdcore-license/requests/LICENSE.txt,sha256=CeipvOyAZxBGUsFoaFqwkx54aPnIKEtm9a5u2uXxEws,10142
 tdrpa/tdcore-license/tzlocal/LICENSE.txt,sha256=2ZqyCa6xaq0sJckP_YPBqYHikP__dqQgoqsD4D8EG4w,1060
 tdrpa/tdcore-license/uiautomation/LICENSE.txt,sha256=dbcOQowi1H0PtxOlQxoO0HxUwqrfphk-OGwrkfn_Sys,11336
-tdrpa.tdcore-1.1.29.dist-info/METADATA,sha256=EPXwJbH-CO2NA83UPZfbQKk5Aa1YI6onAywcJiE9k2k,638
-tdrpa.tdcore-1.1.29.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-tdrpa.tdcore-1.1.29.dist-info/top_level.txt,sha256=S9UoqmC_cyGqKbGsBkLQPEeQLbDrWD0SRwbxPpQpyyU,6
-tdrpa.tdcore-1.1.29.dist-info/RECORD,,
+tdrpa.tdcore-1.1.30.dist-info/METADATA,sha256=fvXsRKCBZtubzJy2oy25d_6UA8To6pkErTq_9LeueUM,638
+tdrpa.tdcore-1.1.30.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+tdrpa.tdcore-1.1.30.dist-info/top_level.txt,sha256=S9UoqmC_cyGqKbGsBkLQPEeQLbDrWD0SRwbxPpQpyyU,6
+tdrpa.tdcore-1.1.30.dist-info/RECORD,,
```

