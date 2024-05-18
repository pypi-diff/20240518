# Comparing `tmp/psgspecialelements-1.0.2.5.tar.gz` & `tmp/psgspecialelements-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "psgspecialelements-1.0.2.5.tar", last modified: Wed May 10 21:45:41 2023, max compression
+gzip compressed data, was "psgspecialelements-1.0.3.tar", last modified: Sat May 18 15:56:35 2024, max compression
```

## Comparing `psgspecialelements-1.0.2.5.tar` & `psgspecialelements-1.0.3.tar`

### file list

```diff
@@ -1,17 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-05-10 21:45:41.811697 psgspecialelements-1.0.2.5/
--rw-rw-rw-   0        0        0      255 2023-05-10 21:45:41.810697 psgspecialelements-1.0.2.5/PKG-INFO
--rw-rw-rw-   0        0        0     1525 2023-04-21 00:40:07.000000 psgspecialelements-1.0.2.5/README.md
-drwxrwxrwx   0        0        0        0 2023-05-10 21:45:41.791693 psgspecialelements-1.0.2.5/config/
-drwxrwxrwx   0        0        0        0 2023-05-10 21:45:41.799695 psgspecialelements-1.0.2.5/config/img/
--rw-rw-rw-   0        0        0    16958 2023-05-10 13:46:04.000000 psgspecialelements-1.0.2.5/config/img/table_arrow9_transparent_64.ico
--rw-rw-rw-   0        0        0    34392 2023-04-06 03:13:05.000000 psgspecialelements-1.0.2.5/hash_password.py
-drwxrwxrwx   0        0        0        0 2023-05-10 21:45:41.809697 psgspecialelements-1.0.2.5/psgspecialelements.egg-info/
--rw-rw-rw-   0        0        0      255 2023-05-10 21:45:41.000000 psgspecialelements-1.0.2.5/psgspecialelements.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      354 2023-05-10 21:45:41.000000 psgspecialelements-1.0.2.5/psgspecialelements.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-10 21:45:41.000000 psgspecialelements-1.0.2.5/psgspecialelements.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       57 2023-05-10 21:45:41.000000 psgspecialelements-1.0.2.5/psgspecialelements.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       75 2023-05-10 21:45:41.000000 psgspecialelements-1.0.2.5/psgspecialelements.egg-info/requires.txt
--rw-rw-rw-   0        0        0       33 2023-05-10 21:45:41.000000 psgspecialelements-1.0.2.5/psgspecialelements.egg-info/top_level.txt
--rw-rw-rw-   0        0        0   241246 2023-05-10 21:44:14.000000 psgspecialelements-1.0.2.5/psgspecialelements.py
--rw-rw-rw-   0        0        0       42 2023-05-10 21:45:41.811697 psgspecialelements-1.0.2.5/setup.cfg
--rw-rw-rw-   0        0        0     2782 2023-05-10 21:44:30.000000 psgspecialelements-1.0.2.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-18 15:56:35.428216 psgspecialelements-1.0.3/
+-rw-rw-rw-   0        0        0      188 2024-05-18 15:56:35.427205 psgspecialelements-1.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     1543 2024-05-18 15:18:04.000000 psgspecialelements-1.0.3/README.md
+drwxrwxrwx   0        0        0        0 2024-05-18 15:56:35.388706 psgspecialelements-1.0.3/config/
+drwxrwxrwx   0        0        0        0 2024-05-18 15:56:35.409686 psgspecialelements-1.0.3/config/img/
+-rw-rw-rw-   0        0        0    16958 2024-05-18 15:18:04.000000 psgspecialelements-1.0.3/config/img/table_arrow9_transparent_64.ico
+-rw-rw-rw-   0        0        0    34392 2024-05-18 15:18:04.000000 psgspecialelements-1.0.3/hash_password.py
+drwxrwxrwx   0        0        0        0 2024-05-18 15:56:35.425696 psgspecialelements-1.0.3/psgspecialelements.egg-info/
+-rw-rw-rw-   0        0        0      188 2024-05-18 15:56:35.000000 psgspecialelements-1.0.3/psgspecialelements.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      309 2024-05-18 15:56:35.000000 psgspecialelements-1.0.3/psgspecialelements.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-18 15:56:35.000000 psgspecialelements-1.0.3/psgspecialelements.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       83 2024-05-18 15:56:35.000000 psgspecialelements-1.0.3/psgspecialelements.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       33 2024-05-18 15:56:35.000000 psgspecialelements-1.0.3/psgspecialelements.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0   239432 2024-05-18 15:18:04.000000 psgspecialelements-1.0.3/psgspecialelements.py
+-rw-rw-rw-   0        0        0       42 2024-05-18 15:56:35.428216 psgspecialelements-1.0.3/setup.cfg
+-rw-rw-rw-   0        0        0     2600 2024-05-18 15:56:11.000000 psgspecialelements-1.0.3/setup.py
```

### Comparing `psgspecialelements-1.0.2.5/README.md` & `psgspecialelements-1.0.3/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # psgspecialelemnts
 
 #### 介绍
 基于pysimplegui，扩展部分elements： SpecialTable, SpecialTableGroup, SpecailCombox
 该模块基于pysimplegui，扩展如下：
-
+# psgspecialelements
 ## class SpecialCombox(Sg.Combo)
 自定义Combo用于过滤update text_color， background_color, 因为Sg.Combo没有此option
 ## class SpecialTable(object)
 自定义table， 比SgTable可以做更多复杂的表格操作
 ## class SpecialTableGroup(SpecialTable)
 自定义TableGroup，可以同时操作多张表格，在表格间自由切换
 
@@ -43,8 +43,7 @@
 
 1.  使用 Readme\_XXX.md 来支持不同的语言，例如 Readme\_en.md, Readme\_zh.md
 2.  Gitee 官方博客 [blog.gitee.com](https://blog.gitee.com)
 3.  你可以 [https://gitee.com/explore](https://gitee.com/explore) 这个地址来了解 Gitee 上的优秀开源项目
 4.  [GVP](https://gitee.com/gvp) 全称是 Gitee 最有价值开源项目，是综合评定出的优秀开源项目
 5.  Gitee 官方提供的使用手册 [https://gitee.com/help](https://gitee.com/help)
 6.  Gitee 封面人物是一档用来展示 Gitee 会员风采的栏目 [https://gitee.com/gitee-stars/](https://gitee.com/gitee-stars/)
-
```

### Comparing `psgspecialelements-1.0.2.5/config/img/table_arrow9_transparent_64.ico` & `psgspecialelements-1.0.3/config/img/table_arrow9_transparent_64.ico`

 * *Files identical despite different names*

### Comparing `psgspecialelements-1.0.2.5/hash_password.py` & `psgspecialelements-1.0.3/hash_password.py`

 * *Files identical despite different names*

### Comparing `psgspecialelements-1.0.2.5/psgspecialelements.py` & `psgspecialelements-1.0.3/psgspecialelements.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,23 +3,20 @@
 import ast
 
 import PySimpleGUI as Sg
 import pandas as pd
 import numpy as np
 import copy
 import os
-import sys
-import shutil
-from pathlib import Path
 from openpyxl import load_workbook
 import inspect
 from dataclasses import dataclass
 
-SYSTEM_ICON = 'config/img/table_arrow9_transparent_64.ico'
-SYSTEM_DATA_FILES = [SYSTEM_ICON]
+SYSTEM_ICON = './config/img/table_arrow9_transparent_64.ico'
+
 INPUTFILE_SRTING_COLUMNS = '-string-columns'
 OUTPUTFILE_RENAME_KEY = '-output'
 
 # 表格tab中的最大阈值，表格数及每张表格的最大列数
 MAX_TABLE_NUMBER = 15  # 最大配置，大于18运行错误
 MAX_TABLE_SHOW_COLUMNS = 20
 
@@ -3675,115 +3672,26 @@
         """
         if attribute is None:
             return self.currenttable
         else:
             return super().get(attribute=attribute, **kwargs)
 
 
-# 根据系统配置拷贝相应的数据文件和配置文件到本地目录
-def sys_data_files_copy(sysdatafiles: list) -> list:
-    for file in sysdatafiles:
-        result = sys_config_copy(file)
-        if result[0] is False:
-            return result
-    return [True, ""]
-
-
-# 系统初始化，判断fileprocconfig是否存在，如果不存在，尝试从系统config目录（pip，python的安装目录拷贝），系统目录也不存在则报错退出
-# 判断本地目录是否存在fileprocconfig
-def sys_config_copy(localconfigfile: str) -> list:
-    if Path(localconfigfile).is_file() is False:
-        try:
-            # 组合系统配置目录对应文件
-            sysfileprocconfig = os.path.join(sys.prefix, localconfigfile)
-            if Path(sysfileprocconfig).is_file() is False:
-                print("本地配置文件：{}及系统原始配置文件{} 均不存在！".format(localconfigfile, sysfileprocconfig))
-                sys.exit(-1)
-            else:
-                # 判断本地配置目录是否存在，如果不存在则创建目录，逐层创建
-                localdir = os.path.dirname(localconfigfile)
-                if Path(localdir).is_dir() is False:
-                    os.makedirs(localdir)
-                # 拷贝系统配置文件到本地
-                shutil.copy(sysfileprocconfig, localconfigfile)
-        except Exception as err:
-            return [False, "拷贝系统原始配置到本地配置文件：{} 失败：{}".format(localconfigfile, err)]
-
-    return [True, ""]
-
-
 def main_test():
     from PySimpleGUI import THEME_CLAM, THEME_DEFAULT, THEME_ALT, THEME_CLASSIC
     Sg.set_options(ttk_theme=THEME_DEFAULT)
     dfdata1 = pd.DataFrame(
         ["数据{}-{}".format(x, y) for y in range(MAX_SPECIAL_TABLE_COLUMNS * 2)]
         for x in range(MAX_SPECIAL_TABLE_ROWS * MAX_SPECIAL_TABLE_ROWS - 10))
     dfdata2 = pd.DataFrame(
         ["测试{}-{}".format(x, y) for y in range(MAX_SPECIAL_TABLE_COLUMNS * 2)]
         for x in range(MAX_SPECIAL_TABLE_ROWS * MAX_SPECIAL_TABLE_ROWS - 10))
     dfdata3 = pd.DataFrame(
         ["新数据{}-{}".format(x, y) for y in range(MAX_SPECIAL_TABLE_COLUMNS * 2)]
         for x in range(MAX_SPECIAL_TABLE_ROWS * MAX_SPECIAL_TABLE_ROWS - 10))
-    test_parminfo = [
-    ]
-    test_column_widths = [30, 1, 8, 3, 16, 40, 1, 6, 4, 4]
-    test_visible_column_map = [True, False, True, True, True, True, False, True, True, True]
-    test_columninfodic = {
-        '命令': 'exe_unit',
-        '账号需求': 'need_password',
-        '账号类型 ': 'account_type',
-        '选项': 'cmd_option',
-        '项目描述': 'item_name',
-        '默认文件': 'file_name',
-        '文件类型': 'file_type_info',
-        '文件后缀': 'file_type',
-        '读/写': 'save_mode',
-        '可更改': 'changable'
-    }
-    test_accounttypedic = {
-        "JDE": {
-            "default_account": "f9b531805c280b9f61e0dfdd8e69c2fd",
-            "account_password": {
-            }
-        },
-        "ERP": {
-            "default_account": "f9b531805c280b9f61e0dfdd8e69c2fd",
-            "account_password": {}
-        },
-        "EAS": {
-            "default_account": "45d2a8efdea386c3b3f400c5961cf84a",
-            "account_password": {}
-        }
-    }
-    test_errdefinedic = {
-        "101": "帐号为空",
-        "102": "密码为空",
-        "103": "密码错误",
-        "104": "未知错误",
-        "201": "命令所需文件不全",
-        "202": "读取文件失败",
-        "203": "文件格式不匹配",
-        "204": "写入文件错误",
-        "205": "未选择账号"
-    }
-    test_functioncalldic = {
-        "无": "",
-    }
-    test_colvaluescale = [
-        [],  # 命令
-        ['是', '否'],  # 是否需要账号运行
-        [a for a in test_accounttypedic.keys()],  # 账号类型
-        [''] + ['-' + chr(i) for i in range(ord('a'), ord('z') + 1)],  # 命令选项
-        [],  # 项目描述
-        [],  # 默认文件
-        None,  # 文件类型,与文件后缀需要互动， 因此不允许批量更改
-        None,  # 文件后缀,与文件类型需要互动， 因此不允许批量更改
-        ['读', '写'],  # 文件为读还是写
-        ['是', '否']  # 是否可更改
-    ]
     dfdata4 = pd.DataFrame([["1", "2", "3"], ["4", "5", "6"], ['7', "8", "9"]], columns=list('abc'))
     dfdata5 = pd.DataFrame([], columns=list("ABC"))
     layoutstatic = []
     tempfuncargs = {
         "accounttypedic": test_accounttypedic,
         "functioncalldic": test_functioncalldic,
     }
@@ -3797,20 +3705,14 @@
         None,
         [],  # 菜单配置文件
         ['是', '否'],
         commandtypelist,  # 命令类型
         []  # 图标文件
     ]
 
-    # 拷贝系统文件
-    result = sys_data_files_copy(SYSTEM_DATA_FILES)
-    if result[0] is False:
-        print(result[1])
-        sys.exit(-1)
-
     tablegroupkey = '_table_group_'
     headings1 = ["数据列{}".format(x) for x in range(MAX_SPECIAL_TABLE_COLUMNS * 2)]
     headings2 = ["测试列{}".format(x) for x in range(MAX_SPECIAL_TABLE_COLUMNS * 2)]
     headings3 = ["新数据列{}".format(x) for x in range(MAX_SPECIAL_TABLE_COLUMNS * 2)]
     dfdata1.columns = headings1
     dfdata2.columns = headings2
     dfdata3.columns = headings3
@@ -3902,15 +3804,15 @@
             Sg.Text("".rjust(20)),
             Sg.Button(' 关  闭 ', k='_close_', pad=(10, 20)),
         ]
     ]
     # 拼接页面配置
     layout = layoutstatic + layouttable + layouttail
 
-    mainwindow = Sg.Window('SPECIAL TABLE 功能测试',
+    mainwindow = Sg.Window('UMD SPECIAL TABLE 功能测试',
                            layout,
                            font=SPECIAL_TABLE_DEF_FT,
                            icon=SYSTEM_ICON,
                            # return_keyboard_events=True,
                            resizable=False,
                            size=(1500, 660),
                            modal=True,
@@ -3976,9 +3878,66 @@
                 print("configwindow unknow event:{}".format(event))
             continue
 
     mainwindow.close()
 
 
 if __name__ == '__main__':
+    test_parminfo = [
+    ]
+    test_column_widths = [30, 1, 8, 3, 16, 40, 1, 6, 4, 4]
+    test_visible_column_map = [True, False, True, True, True, True, False, True, True, True]
+    test_columninfodic = {
+        '命令': 'exe_unit',
+        '账号需求': 'need_password',
+        '账号类型 ': 'account_type',
+        '选项': 'cmd_option',
+        '项目描述': 'item_name',
+        '默认文件': 'file_name',
+        '文件类型': 'file_type_info',
+        '文件后缀': 'file_type',
+        '读/写': 'save_mode',
+        '可更改': 'changable'
+    }
+    test_accounttypedic = {
+        "JDE": {
+            "default_account": "f9b531805c280b9f61e0dfdd8e69c2fd",
+            "account_password": {
+            }
+        },
+        "ERP": {
+            "default_account": "f9b531805c280b9f61e0dfdd8e69c2fd",
+            "account_password": {}
+        },
+        "EAS": {
+            "default_account": "45d2a8efdea386c3b3f400c5961cf84a",
+            "account_password": {}
+        }
+    }
+    test_errdefinedic = {
+        "101": "帐号为空",
+        "102": "密码为空",
+        "103": "密码错误",
+        "104": "未知错误",
+        "201": "命令所需文件不全",
+        "202": "读取文件失败",
+        "203": "文件格式不匹配",
+        "204": "写入文件错误",
+        "205": "未选择账号"
+    }
+    test_functioncalldic = {
+        "无": "",
+    }
+    test_colvaluescale = [
+        [],  # 命令
+        ['是', '否'],  # 是否需要账号运行
+        [a for a in test_accounttypedic.keys()],  # 账号类型
+        [''] + ['-' + chr(i) for i in range(ord('a'), ord('z') + 1)],  # 命令选项
+        [],  # 项目描述
+        [],  # 默认文件
+        None,  # 文件类型,与文件后缀需要互动， 因此不允许批量更改
+        None,  # 文件后缀,与文件类型需要互动， 因此不允许批量更改
+        ['读', '写'],  # 文件为读还是写
+        ['是', '否']  # 是否可更改
+    ]
     main_test()
```

### Comparing `psgspecialelements-1.0.2.5/setup.py` & `psgspecialelements-1.0.3/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,174 +1,163 @@
 00000000: 0d0a 6672 6f6d 2073 6574 7570 746f 6f6c  ..from setuptool
 00000010: 7320 696d 706f 7274 2073 6574 7570 2c20  s import setup, 
 00000020: 6669 6e64 5f70 6163 6b61 6765 730d 0a0d  find_packages...
 00000030: 0a73 6574 7570 280d 0a20 2020 206e 616d  .setup(..    nam
 00000040: 653d 2770 7367 7370 6563 6961 6c65 6c65  e='psgspecialele
 00000050: 6d65 6e74 7327 2c0d 0a20 2020 2076 6572  ments',..    ver
-00000060: 7369 6f6e 3d27 312e 302e 322e 3527 2c0d  sion='1.0.2.5',.
-00000070: 0a20 2020 2064 6573 6372 6970 7469 6f6e  .    description
-00000080: 3d27 7370 6563 6961 6c20 656c 656d 656e  ='special elemen
-00000090: 7473 2062 6173 6564 206f 6e20 7079 7369  ts based on pysi
-000000a0: 6d70 6c65 6775 6920 656c 656d 656e 7473  mplegui elements
-000000b0: 272c 0d0a 2020 2020 6175 7468 6f72 3d27  ',..    author='
-000000c0: 4672 616e 6b20 476f 6e67 272c 0d0a 2020  Frank Gong',..  
-000000d0: 2020 6175 7468 6f72 5f65 6d61 696c 3d27    author_email='
-000000e0: 3538 3339 3833 3731 3640 7171 2e63 6f6d  583983716@qq.com
-000000f0: 272c 0d0a 2020 2020 7061 636b 6167 6573  ',..    packages
-00000100: 3d66 696e 645f 7061 636b 6167 6573 2829  =find_packages()
-00000110: 2c20 2020 2020 2020 2023 20e8 a1a8 e7a4  ,        # .....
-00000120: bae4 bda0 e8a6 81e5 b081 e8a3 85e7 9a84  ................
-00000130: e58c 85ef bc8c 6669 6e64 5f70 6163 6b61  ......find_packa
-00000140: 6765 73e7 94a8 e4ba 8ee7 b3bb e7bb 9fe8  ges.............
-00000150: 87aa e58a a8e4 bb8e e5bd 93e5 898d e79b  ................
-00000160: aee5 bd95 e5bc 80e5 a78b e689 bee5 8c85  ................
-00000170: 0d0a 2020 2020 6c69 6365 6e73 653d 224d  ..    license="M
-00000180: 4954 222c 0d0a 2020 2020 7079 5f6d 6f64  IT",..    py_mod
-00000190: 756c 6573 3d5b 2770 7367 7370 6563 6961  ules=['psgspecia
-000001a0: 6c65 6c65 6d65 6e74 7327 2c20 2768 6173  lelements', 'has
-000001b0: 685f 7061 7373 776f 7264 275d 2c0d 0a20  h_password'],.. 
-000001c0: 2020 2069 6e73 7461 6c6c 5f72 6571 7569     install_requi
-000001d0: 7265 733d 5b27 5079 5369 6d70 6c65 4755  res=['PySimpleGU
-000001e0: 4927 2c20 2770 616e 6461 737e 3d31 2e35  I', 'pandas~=1.5
-000001f0: 2e32 272c 2027 6e75 6d70 797e 3d31 2e32  .2', 'numpy~=1.2
-00000200: 342e 3127 2c20 276f 7065 6e70 7978 6c27  4.1', 'openpyxl'
-00000210: 2c20 2764 6174 6163 6c61 7373 6573 272c  , 'dataclasses',
-00000220: 2027 7079 6372 7970 746f 646f 6d65 7827   'pycryptodomex'
-00000230: 5d2c 0d0a 2020 2020 6461 7461 5f66 696c  ],..    data_fil
-00000240: 6573 3d5b 0d0a 2020 2020 2020 2020 2827  es=[..        ('
-00000250: 636f 6e66 6967 2f69 6d67 272c 205b 2763  config/img', ['c
-00000260: 6f6e 6669 672f 696d 672f 7461 626c 655f  onfig/img/table_
-00000270: 6172 726f 7739 5f74 7261 6e73 7061 7265  arrow9_transpare
-00000280: 6e74 5f36 342e 6963 6f27 5d29 2c0d 0a20  nt_64.ico']),.. 
-00000290: 2020 2020 2020 2023 2028 2763 6f6e 6669         # ('confi
-000002a0: 6727 2c20 205b 2763 6667 2f64 6174 612e  g',  ['cfg/data.
-000002b0: 6366 6727 5d29 0d0a 2020 2020 5d2c 0d0a  cfg'])..    ],..
-000002c0: 2020 2020 7572 6c3d 2768 7474 7073 3a2f      url='https:/
-000002d0: 2f67 6974 6565 2e63 6f6d 2f46 7261 6e6b  /gitee.com/Frank
-000002e0: 5f35 3833 3938 3337 3136 2f70 7367 7370  _583983716/psgsp
-000002f0: 6563 6961 6c65 6c65 6d65 6e74 7327 2c0d  ecialelements',.
-00000300: 0a20 2020 2065 6e74 7279 5f70 6f69 6e74  .    entry_point
-00000310: 733d 7b0d 0a20 2020 2020 2020 2027 636f  s={..        'co
-00000320: 6e73 6f6c 655f 7363 7269 7074 7327 3a20  nsole_scripts': 
-00000330: 5b0d 0a20 2020 2020 2020 2020 2020 2027  [..            '
-00000340: 7073 6774 6573 7420 3d20 7073 6773 7065  psgtest = psgspe
-00000350: 6369 616c 656c 656d 656e 7473 3a6d 6169  cialelements:mai
-00000360: 6e5f 7465 7374 270d 0a20 2020 2020 2020  n_test'..       
-00000370: 205d 0d0a 2020 2020 7d0d 0a20 2020 2023   ]..    }..    #
-00000380: 2063 6c61 7373 6966 6965 7273 3d5b 0d0a   classifiers=[..
-00000390: 2020 2020 2320 2020 2020 2320 e58f 91e5      #     # ....
-000003a0: b195 e697 b6e6 9c9f 2ce5 b8b8 e8a7 81e7  ........,.......
-000003b0: 9a84 e5a6 82e4 b88b 0d0a 2020 2020 2320  ..........    # 
-000003c0: 2020 2020 2320 2020 3320 2d20 416c 7068      #   3 - Alph
-000003d0: 610d 0a20 2020 2023 2020 2020 2023 2020  a..    #     #  
-000003e0: 2034 202d 2042 6574 610d 0a20 2020 2023   4 - Beta..    #
-000003f0: 2020 2020 2023 2020 2035 202d 2050 726f       #   5 - Pro
-00000400: 6475 6374 696f 6e2f 5374 6162 6c65 0d0a  duction/Stable..
-00000410: 2020 2020 2320 2020 2020 2744 6576 656c      #     'Devel
-00000420: 6f70 6d65 6e74 2053 7461 7475 7320 3a3a  opment Status ::
-00000430: 2035 202d 2053 7461 626c 6527 2c0d 0a20   5 - Stable',.. 
-00000440: 2020 2023 2020 2020 2023 20e5 bc80 e58f     #     # .....
-00000450: 91e7 9a84 e79b aee6 a087 e794 a8e6 88b7  ................
-00000460: 0d0a 2020 2020 2320 2020 2020 2749 6e74  ..    #     'Int
-00000470: 656e 6465 6420 4175 6469 656e 6365 203a  ended Audience :
-00000480: 3a20 4465 7665 6c6f 7065 7273 272c 0d0a  : Developers',..
-00000490: 2020 2020 2320 2020 2020 2320 e5b1 9ee4      #     # ....
-000004a0: ba8e e4bb 80e4 b988 e7b1 bbe5 9e8b 0d0a  ................
-000004b0: 2020 2020 2320 2020 2020 2754 6f70 6963      #     'Topic
-000004c0: 203a 3a20 536f 6674 7761 7265 2044 6576   :: Software Dev
-000004d0: 656c 6f70 6d65 6e74 203a 3a20 546f 6f6c  elopment :: Tool
-000004e0: 7327 2c0d 0a20 2020 2023 2020 2020 2023  s',..    #     #
-000004f0: 20e8 aeb8 e58f afe8 af81 e4bf a1e6 81af   ...............
-00000500: 0d0a 2020 2020 2320 2020 2020 274c 6963  ..    #     'Lic
-00000510: 656e 7365 203a 3a20 4f53 4920 4170 7072  ense :: OSI Appr
-00000520: 6f76 6564 203a 3a20 4253 4420 4c69 6365  oved :: BSD Lice
-00000530: 6e73 6527 2c0d 0a20 2020 2023 2020 2020  nse',..    #    
-00000540: 2023 20e7 9bae e6a0 8720 5079 7468 6f6e   # ...... Python
-00000550: 20e7 8988 e69c ac0d 0a20 2020 2023 2020   ........    #  
-00000560: 2020 2027 5072 6f67 7261 6d6d 696e 6720     'Programming 
-00000570: 4c61 6e67 7561 6765 203a 3a20 5079 7468  Language :: Pyth
-00000580: 6f6e 203a 3a20 3327 2c0d 0a20 2020 2023  on :: 3',..    #
-00000590: 2020 2020 2027 5072 6f67 7261 6d6d 696e       'Programmin
-000005a0: 6720 4c61 6e67 7561 6765 203a 3a20 5079  g Language :: Py
-000005b0: 7468 6f6e 203a 3a20 332e 3627 2c0d 0a20  thon :: 3.6',.. 
-000005c0: 2020 2023 2020 2020 2027 5072 6f67 7261     #     'Progra
-000005d0: 6d6d 696e 6720 4c61 6e67 7561 6765 203a  mming Language :
-000005e0: 3a20 5079 7468 6f6e 203a 3a20 332e 3727  : Python :: 3.7'
-000005f0: 2c0d 0a20 2020 2023 2020 2020 2027 5072  ,..    #     'Pr
-00000600: 6f67 7261 6d6d 696e 6720 4c61 6e67 7561  ogramming Langua
-00000610: 6765 203a 3a20 5079 7468 6f6e 203a 3a20  ge :: Python :: 
-00000620: 332e 3827 2c0d 0a20 2020 2023 2020 2020  3.8',..    #    
-00000630: 2027 5072 6f67 7261 6d6d 696e 6720 4c61   'Programming La
-00000640: 6e67 7561 6765 203a 3a20 5079 7468 6f6e  nguage :: Python
-00000650: 203a 3a20 332e 3927 2c0d 0a20 2020 2023   :: 3.9',..    #
-00000660: 205d 0d0a 290d 0a27 2727 0d0a 6e61 6d65   ]..)..'''..name
-00000670: 203a 20e6 8993 e58c 85e5 908e e58c 85e7   : .............
-00000680: 9a84 e696 87e4 bbb6 e590 8d0d 0a76 6572  .............ver
-00000690: 7369 6f6e 203a 20e7 8988 e69c ace5 8fb7  sion : .........
-000006a0: 0d0a 6175 7468 6f72 203a 20e4 bd9c e880  ..author : .....
-000006b0: 850d 0a61 7574 686f 725f 656d 6169 6c20  ...author_email 
-000006c0: 3a20 e4bd 9ce8 8085 e79a 84e9 82ae e7ae  : ..............
-000006d0: b10d 0a70 795f 6d6f 6475 6c65 7320 3a20  ...py_modules : 
-000006e0: e8a6 81e6 8993 e58c 85e7 9a84 2e70 79e6  .............py.
-000006f0: 9687 e4bb b60d 0a70 6163 6b61 6765 733a  .......packages:
-00000700: 20e6 8993 e58c 85e7 9a84 7079 7468 6f6e   .........python
-00000710: e696 87e4 bbb6 e5a4 b90d 0a69 6e63 6c75  ...........inclu
-00000720: 6465 5f70 6163 6b61 6765 5f64 6174 6120  de_package_data 
-00000730: 3a20 e9a1 b9e7 9bae e987 8ce4 bc9a e69c  : ..............
-00000740: 89e4 b880 e4ba 9be9 9d9e 7079 e696 87e4  ..........py....
-00000750: bbb6 2ce6 af94 e5a6 8268 746d 6ce5 928c  ..,......html...
-00000760: 6a73 e7ad 892c e8bf 99e6 97b6 e580 99e5  js...,..........
-00000770: b0b1 e8a6 81e9 9da0 696e 636c 7564 655f  ........include_
-00000780: 7061 636b 6167 655f 6461 7461 20e5 928c  package_data ...
-00000790: 2070 6163 6b61 6765 5f64 6174 6120 e69d   package_data ..
-000007a0: a5e6 8c87 e5ae 9ae4 ba86 e380 8270 6163  .............pac
-000007b0: 6b61 6765 5f64 6174 613a e4b8 80e8 88ac  kage_data:......
-000007c0: e586 99e6 8890 7be2 8098 796f 7572 5f70  ......{...your_p
-000007d0: 6163 6b61 6765 5f6e 616d 65e2 8099 3a20  ackage_name...: 
-000007e0: 5be2 809c 6669 6c65 73e2 809d 5d7d 2c20  [...files...]}, 
-000007f0: 696e 636c 7564 655f 7061 636b 6167 655f  include_package_
-00000800: 6461 7461 e8bf 98e6 b2a1 e5ae 8c2c e8bf  data.........,..
-00000810: 98e9 9c80 e8a6 81e4 bfae e694 b94d 414e  .............MAN
-00000820: 4946 4553 542e 696e e696 87e4 bbb6 2e4d  IFEST.in.......M
-00000830: 414e 4946 4553 542e 696e e696 87e4 bbb6  ANIFEST.in......
-00000840: e79a 84e8 afad e6b3 95e4 b8ba 3a20 696e  ............: in
-00000850: 636c 7564 6520 7878 782f 7878 782f 7878  clude xxx/xxx/xx
-00000860: 782f 2e69 6e69 2f28 e689 80e6 9c89 e4bb  x/.ini/(........
-00000870: a52e 696e 69e7 bb93 e5b0 bee7 9a84 e696  ..ini...........
-00000880: 87e4 bbb6 2ce4 b99f e58f afe4 bba5 e79b  ....,...........
-00000890: b4e6 8ea5 e68c 87e5 ae9a e696 87e4 bbb6  ................
-000008a0: e590 8d29 0d0a 6c69 6365 6e73 6520 3a20  ...)..license : 
-000008b0: e694 afe6 8c81 e79a 84e5 bc80 e6ba 90e5  ................
-000008c0: 8d8f e8ae ae0d 0a64 6573 6372 6970 7469  .......descripti
-000008d0: 6f6e 203a 20e5 afb9 e9a1 b9e7 9bae e7ae  on : ...........
-000008e0: 80e7 9fad e79a 84e4 b880 e4b8 aae5 bda2  ................
-000008f0: e5ae b90d 0a65 7874 5f6d 6f64 756c 6573  .....ext_modules
-00000900: 203a 20e6 98af e4b8 80e4 b8aa e58c 85e5   : .............
-00000910: 90ab 4578 7465 6e73 696f 6ee5 ae9e e4be  ..Extension.....
-00000920: 8be7 9a84 e588 97e8 a1a8 2c45 7874 656e  ..........,Exten
-00000930: 7369 6f6e e79a 84e5 ae9a e4b9 89e4 b99f  sion............
-00000940: e69c 89e4 b880 e4ba 9be5 8f82 e695 b0e3  ................
-00000950: 8082 0d0a 6578 745f 7061 636b 6167 6520  ....ext_package 
-00000960: 3a20 e5ae 9ae4 b989 6578 7465 6e73 696f  : ......extensio
-00000970: 6ee7 9a84 e79b b8e5 afb9 e8b7 afe5 be84  n...............
-00000980: 0d0a 7265 7175 6972 6573 203a 20e5 ae9a  ..requires : ...
-00000990: e4b9 89e4 be9d e8b5 96e5 93aa e4ba 9be6  ................
-000009a0: a8a1 e59d 970d 0a70 726f 7669 6465 7320  .......provides 
-000009b0: 3a20 e5ae 9ae4 b989 e58f afe4 bba5 e4b8  : ..............
-000009c0: bae5 93aa e4ba 9be6 a8a1 e59d 97e6 8f90  ................
-000009d0: e4be 9be4 be9d e8b5 960d 0a64 6174 615f  ...........data_
-000009e0: 6669 6c65 7320 3ae6 8c87 e5ae 9ae5 85b6  files :.........
-000009f0: e4bb 96e7 9a84 e4b8 80e4 ba9b e696 87e4  ................
-00000a00: bbb6 28e5 a682 e985 8de7 bdae e696 87e4  ..(.............
-00000a10: bbb6 292c e8a7 84e5 ae9a e4ba 86e5 93aa  ..),............
-00000a20: e4ba 9be6 9687 e4bb b6e8 a2ab e5ae 89e8  ................
-00000a30: a385 e588 b0e5 93aa e4ba 9be7 9bae e5bd  ................
-00000a40: 95e4 b8ad e380 82e5 a682 e69e 9ce7 9bae  ................
-00000a50: e5bd 95e5 908d e698 afe7 9bb8 e5af b9e8  ................
-00000a60: b7af e5be 842c e588 99e6 98af e79b b8e5  .....,..........
-00000a70: afb9 e4ba 8e73 7973 2e70 7265 6669 78e6  .....sys.prefix.
-00000a80: 8896 7379 732e 6578 6563 5f70 7265 6669  ..sys.exec_prefi
-00000a90: 78e7 9a84 e8b7 afe5 be84 e380 82e5 a682  x...............
-00000aa0: e69e 9ce6 b2a1 e69c 89e6 8f90 e4be 9be6  ................
-00000ab0: a8a1 e69d bf2c e4bc 9ae8 a2ab e6b7 bbe5  .....,..........
-00000ac0: 8aa0 e588 b04d 414e 4946 4553 54e6 9687  .....MANIFEST...
-00000ad0: e4bb b6e4 b8ad e380 820d 0a27 2727       ...........'''
+00000060: 7369 6f6e 3d27 312e 302e 3327 2c0d 0a20  sion='1.0.3',.. 
+00000070: 2020 2064 6573 6372 6970 7469 6f6e 3d27     description='
+00000080: 7370 6563 6961 6c20 656c 656d 656e 7473  special elements
+00000090: 2062 6173 6564 206f 6e20 7079 7369 6d70   based on pysimp
+000000a0: 6c65 6775 6920 656c 656d 656e 7473 272c  legui elements',
+000000b0: 0d0a 2020 2020 6175 7468 6f72 3d27 4672  ..    author='Fr
+000000c0: 616e 6b20 476f 6e67 272c 0d0a 2020 2020  ank Gong',..    
+000000d0: 6175 7468 6f72 5f65 6d61 696c 3d27 3538  author_email='58
+000000e0: 3339 3833 3731 3640 7171 2e63 6f6d 272c  3983716@qq.com',
+000000f0: 0d0a 2020 2020 7061 636b 6167 6573 3d66  ..    packages=f
+00000100: 696e 645f 7061 636b 6167 6573 2829 2c20  ind_packages(), 
+00000110: 2020 2020 2020 2023 20e8 a1a8 e7a4 bae4         # .......
+00000120: bda0 e8a6 81e5 b081 e8a3 85e7 9a84 e58c  ................
+00000130: 85ef bc8c 6669 6e64 5f70 6163 6b61 6765  ....find_package
+00000140: 73e7 94a8 e4ba 8ee7 b3bb e7bb 9fe8 87aa  s...............
+00000150: e58a a8e4 bb8e e5bd 93e5 898d e79b aee5  ................
+00000160: bd95 e5bc 80e5 a78b e689 bee5 8c85 0d0a  ................
+00000170: 2020 2020 6c69 6365 6e73 653d 2242 5344      license="BSD
+00000180: 222c 0d0a 2020 2020 7079 5f6d 6f64 756c  ",..    py_modul
+00000190: 6573 3d5b 2770 7367 7370 6563 6961 6c65  es=['psgspeciale
+000001a0: 6c65 6d65 6e74 7327 2c20 2768 6173 685f  lements', 'hash_
+000001b0: 7061 7373 776f 7264 275d 2c0d 0a20 2020  password'],..   
+000001c0: 2069 6e73 7461 6c6c 5f72 6571 7569 7265   install_require
+000001d0: 733d 5b27 5079 5369 6d70 6c65 4755 497e  s=['PySimpleGUI~
+000001e0: 3d34 2e35 392e 3027 2c20 2770 616e 6461  =4.59.0', 'panda
+000001f0: 737e 3d31 2e35 2e32 272c 2027 6e75 6d70  s~=1.5.2', 'nump
+00000200: 797e 3d31 2e32 342e 3127 2c20 276f 7065  y~=1.24.1', 'ope
+00000210: 6e70 7978 6c27 2c20 2764 6174 6163 6c61  npyxl', 'datacla
+00000220: 7373 6573 272c 2027 7079 6372 7970 746f  sses', 'pycrypto
+00000230: 646f 6d65 7827 5d2c 0d0a 2020 2020 6461  domex'],..    da
+00000240: 7461 5f66 696c 6573 3d5b 0d0a 2020 2020  ta_files=[..    
+00000250: 2020 2020 2827 636f 6e66 6967 2f69 6d67      ('config/img
+00000260: 272c 205b 2763 6f6e 6669 672f 696d 672f  ', ['config/img/
+00000270: 7461 626c 655f 6172 726f 7739 5f74 7261  table_arrow9_tra
+00000280: 6e73 7061 7265 6e74 5f36 342e 6963 6f27  nsparent_64.ico'
+00000290: 5d29 2c0d 0a20 2020 2020 2020 2023 2028  ]),..        # (
+000002a0: 2763 6f6e 6669 6727 2c20 205b 2763 6667  'config',  ['cfg
+000002b0: 2f64 6174 612e 6366 6727 5d29 0d0a 2020  /data.cfg'])..  
+000002c0: 2020 5d2c 0d0a 2020 2020 2320 636c 6173    ],..    # clas
+000002d0: 7369 6669 6572 733d 5b0d 0a20 2020 2023  sifiers=[..    #
+000002e0: 2020 2020 2023 20e5 8f91 e5b1 95e6 97b6       # .........
+000002f0: e69c 9f2c e5b8 b8e8 a781 e79a 84e5 a682  ...,............
+00000300: e4b8 8b0d 0a20 2020 2023 2020 2020 2023  .....    #     #
+00000310: 2020 2033 202d 2041 6c70 6861 0d0a 2020     3 - Alpha..  
+00000320: 2020 2320 2020 2020 2320 2020 3420 2d20    #     #   4 - 
+00000330: 4265 7461 0d0a 2020 2020 2320 2020 2020  Beta..    #     
+00000340: 2320 2020 3520 2d20 5072 6f64 7563 7469  #   5 - Producti
+00000350: 6f6e 2f53 7461 626c 650d 0a20 2020 2023  on/Stable..    #
+00000360: 2020 2020 2027 4465 7665 6c6f 706d 656e       'Developmen
+00000370: 7420 5374 6174 7573 203a 3a20 3520 2d20  t Status :: 5 - 
+00000380: 5374 6162 6c65 272c 0d0a 2020 2020 2320  Stable',..    # 
+00000390: 2020 2020 2320 e5bc 80e5 8f91 e79a 84e7      # ..........
+000003a0: 9bae e6a0 87e7 94a8 e688 b70d 0a20 2020  .............   
+000003b0: 2023 2020 2020 2027 496e 7465 6e64 6564   #     'Intended
+000003c0: 2041 7564 6965 6e63 6520 3a3a 2044 6576   Audience :: Dev
+000003d0: 656c 6f70 6572 7327 2c0d 0a20 2020 2023  elopers',..    #
+000003e0: 2020 2020 2023 20e5 b19e e4ba 8ee4 bb80       # .........
+000003f0: e4b9 88e7 b1bb e59e 8b0d 0a20 2020 2023  ...........    #
+00000400: 2020 2020 2027 546f 7069 6320 3a3a 2053       'Topic :: S
+00000410: 6f66 7477 6172 6520 4465 7665 6c6f 706d  oftware Developm
+00000420: 656e 7420 3a3a 2054 6f6f 6c73 272c 0d0a  ent :: Tools',..
+00000430: 2020 2020 2320 2020 2020 2320 e8ae b8e5      #     # ....
+00000440: 8faf e8af 81e4 bfa1 e681 af0d 0a20 2020  .............   
+00000450: 2023 2020 2020 2027 4c69 6365 6e73 6520   #     'License 
+00000460: 3a3a 204f 5349 2041 7070 726f 7665 6420  :: OSI Approved 
+00000470: 3a3a 2042 5344 204c 6963 656e 7365 272c  :: BSD License',
+00000480: 0d0a 2020 2020 2320 2020 2020 2320 e79b  ..    #     # ..
+00000490: aee6 a087 2050 7974 686f 6e20 e789 88e6  .... Python ....
+000004a0: 9cac 0d0a 2020 2020 2320 2020 2020 2750  ....    #     'P
+000004b0: 726f 6772 616d 6d69 6e67 204c 616e 6775  rogramming Langu
+000004c0: 6167 6520 3a3a 2050 7974 686f 6e20 3a3a  age :: Python ::
+000004d0: 2033 272c 0d0a 2020 2020 2320 2020 2020   3',..    #     
+000004e0: 2750 726f 6772 616d 6d69 6e67 204c 616e  'Programming Lan
+000004f0: 6775 6167 6520 3a3a 2050 7974 686f 6e20  guage :: Python 
+00000500: 3a3a 2033 2e36 272c 0d0a 2020 2020 2320  :: 3.6',..    # 
+00000510: 2020 2020 2750 726f 6772 616d 6d69 6e67      'Programming
+00000520: 204c 616e 6775 6167 6520 3a3a 2050 7974   Language :: Pyt
+00000530: 686f 6e20 3a3a 2033 2e37 272c 0d0a 2020  hon :: 3.7',..  
+00000540: 2020 2320 2020 2020 2750 726f 6772 616d    #     'Program
+00000550: 6d69 6e67 204c 616e 6775 6167 6520 3a3a  ming Language ::
+00000560: 2050 7974 686f 6e20 3a3a 2033 2e38 272c   Python :: 3.8',
+00000570: 0d0a 2020 2020 2320 2020 2020 2750 726f  ..    #     'Pro
+00000580: 6772 616d 6d69 6e67 204c 616e 6775 6167  gramming Languag
+00000590: 6520 3a3a 2050 7974 686f 6e20 3a3a 2033  e :: Python :: 3
+000005a0: 2e39 270d 0a20 2020 2023 205d 0d0a 290d  .9'..    # ]..).
+000005b0: 0a27 2727 0d0a 6e61 6d65 203a 20e6 8993  .'''..name : ...
+000005c0: e58c 85e5 908e e58c 85e7 9a84 e696 87e4  ................
+000005d0: bbb6 e590 8d0d 0a76 6572 7369 6f6e 203a  .......version :
+000005e0: 20e7 8988 e69c ace5 8fb7 0d0a 6175 7468   ...........auth
+000005f0: 6f72 203a 20e4 bd9c e880 850d 0a61 7574  or : ........aut
+00000600: 686f 725f 656d 6169 6c20 3a20 e4bd 9ce8  hor_email : ....
+00000610: 8085 e79a 84e9 82ae e7ae b10d 0a70 795f  .............py_
+00000620: 6d6f 6475 6c65 7320 3a20 e8a6 81e6 8993  modules : ......
+00000630: e58c 85e7 9a84 2e70 79e6 9687 e4bb b60d  .......py.......
+00000640: 0a70 6163 6b61 6765 733a 20e6 8993 e58c  .packages: .....
+00000650: 85e7 9a84 7079 7468 6f6e e696 87e4 bbb6  ....python......
+00000660: e5a4 b90d 0a69 6e63 6c75 6465 5f70 6163  .....include_pac
+00000670: 6b61 6765 5f64 6174 6120 3a20 e9a1 b9e7  kage_data : ....
+00000680: 9bae e987 8ce4 bc9a e69c 89e4 b880 e4ba  ................
+00000690: 9be9 9d9e 7079 e696 87e4 bbb6 2ce6 af94  ....py......,...
+000006a0: e5a6 8268 746d 6ce5 928c 6a73 e7ad 892c  ...html...js...,
+000006b0: e8bf 99e6 97b6 e580 99e5 b0b1 e8a6 81e9  ................
+000006c0: 9da0 696e 636c 7564 655f 7061 636b 6167  ..include_packag
+000006d0: 655f 6461 7461 20e5 928c 2070 6163 6b61  e_data ... packa
+000006e0: 6765 5f64 6174 6120 e69d a5e6 8c87 e5ae  ge_data ........
+000006f0: 9ae4 ba86 e380 8270 6163 6b61 6765 5f64  .......package_d
+00000700: 6174 613a e4b8 80e8 88ac e586 99e6 8890  ata:............
+00000710: 7be2 8098 796f 7572 5f70 6163 6b61 6765  {...your_package
+00000720: 5f6e 616d 65e2 8099 3a20 5be2 809c 6669  _name...: [...fi
+00000730: 6c65 73e2 809d 5d7d 2c20 696e 636c 7564  les...]}, includ
+00000740: 655f 7061 636b 6167 655f 6461 7461 e8bf  e_package_data..
+00000750: 98e6 b2a1 e5ae 8c2c e8bf 98e9 9c80 e8a6  .......,........
+00000760: 81e4 bfae e694 b94d 414e 4946 4553 542e  .......MANIFEST.
+00000770: 696e e696 87e4 bbb6 2e4d 414e 4946 4553  in.......MANIFES
+00000780: 542e 696e e696 87e4 bbb6 e79a 84e8 afad  T.in............
+00000790: e6b3 95e4 b8ba 3a20 696e 636c 7564 6520  ......: include 
+000007a0: 7878 782f 7878 782f 7878 782f 2e69 6e69  xxx/xxx/xxx/.ini
+000007b0: 2f28 e689 80e6 9c89 e4bb a52e 696e 69e7  /(..........ini.
+000007c0: bb93 e5b0 bee7 9a84 e696 87e4 bbb6 2ce4  ..............,.
+000007d0: b99f e58f afe4 bba5 e79b b4e6 8ea5 e68c  ................
+000007e0: 87e5 ae9a e696 87e4 bbb6 e590 8d29 0d0a  .............)..
+000007f0: 6c69 6365 6e73 6520 3a20 e694 afe6 8c81  license : ......
+00000800: e79a 84e5 bc80 e6ba 90e5 8d8f e8ae ae0d  ................
+00000810: 0a64 6573 6372 6970 7469 6f6e 203a 20e5  .description : .
+00000820: afb9 e9a1 b9e7 9bae e7ae 80e7 9fad e79a  ................
+00000830: 84e4 b880 e4b8 aae5 bda2 e5ae b90d 0a65  ...............e
+00000840: 7874 5f6d 6f64 756c 6573 203a 20e6 98af  xt_modules : ...
+00000850: e4b8 80e4 b8aa e58c 85e5 90ab 4578 7465  ............Exte
+00000860: 6e73 696f 6ee5 ae9e e4be 8be7 9a84 e588  nsion...........
+00000870: 97e8 a1a8 2c45 7874 656e 7369 6f6e e79a  ....,Extension..
+00000880: 84e5 ae9a e4b9 89e4 b99f e69c 89e4 b880  ................
+00000890: e4ba 9be5 8f82 e695 b0e3 8082 0d0a 6578  ..............ex
+000008a0: 745f 7061 636b 6167 6520 3a20 e5ae 9ae4  t_package : ....
+000008b0: b989 6578 7465 6e73 696f 6ee7 9a84 e79b  ..extension.....
+000008c0: b8e5 afb9 e8b7 afe5 be84 0d0a 7265 7175  ............requ
+000008d0: 6972 6573 203a 20e5 ae9a e4b9 89e4 be9d  ires : .........
+000008e0: e8b5 96e5 93aa e4ba 9be6 a8a1 e59d 970d  ................
+000008f0: 0a70 726f 7669 6465 7320 3a20 e5ae 9ae4  .provides : ....
+00000900: b989 e58f afe4 bba5 e4b8 bae5 93aa e4ba  ................
+00000910: 9be6 a8a1 e59d 97e6 8f90 e4be 9be4 be9d  ................
+00000920: e8b5 960d 0a64 6174 615f 6669 6c65 7320  .....data_files 
+00000930: 3ae6 8c87 e5ae 9ae5 85b6 e4bb 96e7 9a84  :...............
+00000940: e4b8 80e4 ba9b e696 87e4 bbb6 28e5 a682  ............(...
+00000950: e985 8de7 bdae e696 87e4 bbb6 292c e8a7  ............),..
+00000960: 84e5 ae9a e4ba 86e5 93aa e4ba 9be6 9687  ................
+00000970: e4bb b6e8 a2ab e5ae 89e8 a385 e588 b0e5  ................
+00000980: 93aa e4ba 9be7 9bae e5bd 95e4 b8ad e380  ................
+00000990: 82e5 a682 e69e 9ce7 9bae e5bd 95e5 908d  ................
+000009a0: e698 afe7 9bb8 e5af b9e8 b7af e5be 842c  ...............,
+000009b0: e588 99e6 98af e79b b8e5 afb9 e4ba 8e73  ...............s
+000009c0: 7973 2e70 7265 6669 78e6 8896 7379 732e  ys.prefix...sys.
+000009d0: 6578 6563 5f70 7265 6669 78e7 9a84 e8b7  exec_prefix.....
+000009e0: afe5 be84 e380 82e5 a682 e69e 9ce6 b2a1  ................
+000009f0: e69c 89e6 8f90 e4be 9be6 a8a1 e69d bf2c  ...............,
+00000a00: e4bc 9ae8 a2ab e6b7 bbe5 8aa0 e588 b04d  ...............M
+00000a10: 414e 4946 4553 54e6 9687 e4bb b6e4 b8ad  ANIFEST.........
+00000a20: e380 820d 0a27 2727                      .....'''
```

