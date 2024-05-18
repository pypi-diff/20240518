# Comparing `tmp/batframes-1.0.0.7.tar.gz` & `tmp/batframes-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "batframes-1.0.0.7.tar", last modified: Wed May 10 21:55:50 2023, max compression
+gzip compressed data, was "batframes-1.0.1.tar", last modified: Sat May 18 16:57:24 2024, max compression
```

## Comparing `batframes-1.0.0.7.tar` & `batframes-1.0.1.tar`

### file list

```diff
@@ -1,31 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-05-10 21:55:50.242826 batframes-1.0.0.7/
--rw-rw-rw-   0        0        0      330 2023-05-10 21:55:50.241826 batframes-1.0.0.7/PKG-INFO
--rw-rw-rw-   0        0        0      154 2023-04-06 11:08:10.000000 batframes-1.0.0.7/README.md
--rw-rw-rw-   0        0        0     9590 2023-04-07 22:32:48.000000 batframes-1.0.0.7/bat_function_call_define.py
-drwxrwxrwx   0        0        0        0 2023-05-10 21:55:50.221821 batframes-1.0.0.7/bat_inner_module/
--rw-rw-rw-   0        0        0      227 2023-04-07 22:37:37.000000 batframes-1.0.0.7/bat_inner_module/inner_demo.py
--rw-rw-rw-   0        0        0      143 2023-04-07 15:30:40.000000 batframes-1.0.0.7/bat_inner_module/inner_demo1.py
--rw-rw-rw-   0        0        0      173 2023-04-07 10:56:05.000000 batframes-1.0.0.7/bat_inner_module/readme_for_inner.md
--rw-rw-rw-   0        0        0    68212 2023-04-08 01:59:23.000000 batframes-1.0.0.7/bat_menu_auto.py
--rw-rw-rw-   0        0        0    42908 2023-05-10 21:54:19.000000 batframes-1.0.0.7/batframe_main.py
-drwxrwxrwx   0        0        0        0 2023-05-10 21:55:50.229823 batframes-1.0.0.7/batframes.egg-info/
--rw-rw-rw-   0        0        0      330 2023-05-10 21:55:50.000000 batframes-1.0.0.7/batframes.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      636 2023-05-10 21:55:50.000000 batframes-1.0.0.7/batframes.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-10 21:55:50.000000 batframes-1.0.0.7/batframes.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       53 2023-05-10 21:55:50.000000 batframes-1.0.0.7/batframes.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      308 2023-05-10 21:55:50.000000 batframes-1.0.0.7/batframes.egg-info/requires.txt
--rw-rw-rw-   0        0        0       77 2023-05-10 21:55:50.000000 batframes-1.0.0.7/batframes.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-10 21:55:50.209819 batframes-1.0.0.7/config/
-drwxrwxrwx   0        0        0        0 2023-05-10 21:55:50.231824 batframes-1.0.0.7/config/DFTrans/
--rw-rw-rw-   0        0        0   162264 2023-04-18 13:07:06.000000 batframes-1.0.0.7/config/DFTrans/DFTrans_config.json
-drwxrwxrwx   0        0        0        0 2023-05-10 21:55:50.232824 batframes-1.0.0.7/config/batframe/
--rw-rw-rw-   0        0        0     2816 2023-04-11 01:59:57.000000 batframes-1.0.0.7/config/batframe/bat_tools_config.json
-drwxrwxrwx   0        0        0        0 2023-05-10 21:55:50.240826 batframes-1.0.0.7/config/img/
--rw-rw-rw-   0        0        0     7631 2023-04-06 08:06:16.000000 batframes-1.0.0.7/config/img/Excel.png
--rw-rw-rw-   0        0        0     1962 2023-04-06 08:06:16.000000 batframes-1.0.0.7/config/img/excel.gif
--rw-rw-rw-   0        0        0    10200 2023-04-06 08:06:16.000000 batframes-1.0.0.7/config/img/little_bear.png
--rw-rw-rw-   0        0        0    42148 2023-03-08 01:46:58.000000 batframes-1.0.0.7/config/img/table_arrow9_transparent_256.png
--rw-rw-rw-   0        0        0    16958 2023-03-08 01:46:58.000000 batframes-1.0.0.7/config/img/table_arrow9_transparent_64.ico
--rw-rw-rw-   0        0        0      585 2023-04-08 00:42:18.000000 batframes-1.0.0.7/nuitka_dependency_files.py
--rw-rw-rw-   0        0        0       42 2023-05-10 21:55:50.242826 batframes-1.0.0.7/setup.cfg
--rw-rw-rw-   0        0        0     6956 2023-05-10 21:54:48.000000 batframes-1.0.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-18 16:57:24.266991 batframes-1.0.1/
+-rw-rw-rw-   0        0        0      272 2024-05-18 16:57:24.265992 batframes-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0      154 2024-05-18 16:44:36.000000 batframes-1.0.1/README.md
+-rw-rw-rw-   0        0        0     9590 2024-05-18 16:44:36.000000 batframes-1.0.1/bat_function_call_define.py
+drwxrwxrwx   0        0        0        0 2024-05-18 16:57:24.252992 batframes-1.0.1/bat_inner_module/
+-rw-rw-rw-   0        0        0       65 2024-05-18 16:44:36.000000 batframes-1.0.1/bat_inner_module/inner_demo.py
+-rw-rw-rw-   0        0        0       67 2024-05-18 16:44:36.000000 batframes-1.0.1/bat_inner_module/inner_demo1.py
+-rw-rw-rw-   0        0        0    68212 2024-05-18 16:44:36.000000 batframes-1.0.1/bat_menu_auto.py
+-rw-rw-rw-   0        0        0    42389 2024-05-18 16:55:57.000000 batframes-1.0.1/batframe_main.py
+drwxrwxrwx   0        0        0        0 2024-05-18 16:57:24.260066 batframes-1.0.1/batframes.egg-info/
+-rw-rw-rw-   0        0        0      272 2024-05-18 16:57:24.000000 batframes-1.0.1/batframes.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      446 2024-05-18 16:57:24.000000 batframes-1.0.1/batframes.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-18 16:57:24.000000 batframes-1.0.1/batframes.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      323 2024-05-18 16:57:24.000000 batframes-1.0.1/batframes.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       77 2024-05-18 16:57:24.000000 batframes-1.0.1/batframes.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-18 16:57:24.240288 batframes-1.0.1/config/
+drwxrwxrwx   0        0        0        0 2024-05-18 16:57:24.265004 batframes-1.0.1/config/img/
+-rw-rw-rw-   0        0        0     7631 2024-05-18 16:44:36.000000 batframes-1.0.1/config/img/Excel.png
+-rw-rw-rw-   0        0        0     1962 2024-05-18 16:44:36.000000 batframes-1.0.1/config/img/excel.gif
+-rw-rw-rw-   0        0        0    10200 2024-05-18 16:44:36.000000 batframes-1.0.1/config/img/little_bear.png
+-rw-rw-rw-   0        0        0    16958 2024-05-18 16:44:36.000000 batframes-1.0.1/config/img/table_arrow9_transparent_64.ico
+-rw-rw-rw-   0        0        0      585 2024-05-18 16:44:36.000000 batframes-1.0.1/nuitka_dependency_files.py
+-rw-rw-rw-   0        0        0       42 2024-05-18 16:57:24.266991 batframes-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0     6795 2024-05-18 16:46:37.000000 batframes-1.0.1/setup.py
```

### Comparing `batframes-1.0.0.7/bat_function_call_define.py` & `batframes-1.0.1/bat_function_call_define.py`

 * *Files identical despite different names*

### Comparing `batframes-1.0.0.7/bat_menu_auto.py` & `batframes-1.0.1/bat_menu_auto.py`

 * *Files identical despite different names*

### Comparing `batframes-1.0.0.7/batframe_main.py` & `batframes-1.0.1/batframe_main.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,19 +20,15 @@
 from psgspecialelements import *
 from bat_function_call_define import cmdline_option_find, bat_function_call, dynamic_load_user_functions
 from DFTrans_main import *
 
 
 # 工具启动的整体配置文件
 sysdefaultdirectory = "./config"
-battoolsconfig = "config/batframe/bat_tools_config.json"
-
-BATFRAME_SYSTEM_DATA_FILES = [battoolsconfig, SYSTEM_ICON,
-                              "config/img/excel.gif", "config/img/Excel.png",
-                              "config/img/little_bear.png", "config/img/table_arrow9_transparent_256.png"]
+battoolsconfig = "./config/batframe/bat_tools_config.json"
 
 commandtypelist = []
 commandtype2valuedic = {}
 
 
 def GraphicButton(text: str, key: str, image_data):
     text = text.replace('_', ' ')
@@ -571,16 +567,20 @@
                 Sg.Text('保存日志', size=(35, 1), justification='center', font=("Helvetica", 15), relief=Sg.RELIEF_RIDGE,
                         key='_save_log_', enable_events=True, visible=True),
                 ]]
 
     # tabgroup的整体layout， 包含日志tab
     layout = [layout1, [Sg.TabGroup([
         [
-            Sg.Tab(x, [[Sg.Col(y, scrollable=True, size=(800, 500), expand_x=True,
-                               expand_y=True, size_subsample_height=1)]])
+            Sg.Tab(x, [[Sg.Col(y,
+                               scrollable=True,
+                               size=(800, 500), expand_x=True,
+                               expand_y=True,
+                               # size_subsample_height=1
+                               )]])
             for x, y in zip(list(commandtypedic.values()), commandgrouplaylist)
         ] +
         [
             Sg.Tab('日志输出', logging_layout)
         ]
     ], key='-TAB GROUP-', expand_x=True, expand_y=True)], layout2]
 
@@ -828,21 +828,14 @@
         if debugpath.is_dir():
             commanddefaultfile = os.path.join(debugpathstring, commandfile)
         else:
             commanddefaultfile = os.path.join(".", commandfile)
 
         debugswitchdefault = 'n'
 
-        # 系统初始化，判断fileprocconfig是否存在，如果不存在，尝试从系统config目录（pip，python的安装目录拷贝），系统目录也不存在则报错退出
-        # 判断本地目录是否存在fileprocconfig
-        result = sys_data_files_copy(BATFRAME_SYSTEM_DATA_FILES)
-        if result[0] is False:
-            print(result[1])
-            sys.exit(-1)
-
         # 读取配置文件
         try:
             with open(battoolsconfig, 'r', encoding='utf8') as fp:
                 configdic = json.load(fp)
                 fp.close()
         except Exception as err:
             print("读取配置文件：{}失败：{}".format(battoolsconfig, err))
```

### Comparing `batframes-1.0.0.7/config/img/Excel.png` & `batframes-1.0.1/config/img/Excel.png`

 * *Files identical despite different names*

### Comparing `batframes-1.0.0.7/config/img/excel.gif` & `batframes-1.0.1/config/img/excel.gif`

 * *Files identical despite different names*

### Comparing `batframes-1.0.0.7/config/img/little_bear.png` & `batframes-1.0.1/config/img/little_bear.png`

 * *Files identical despite different names*

### Comparing `batframes-1.0.0.7/config/img/table_arrow9_transparent_64.ico` & `batframes-1.0.1/config/img/table_arrow9_transparent_64.ico`

 * *Files identical despite different names*

### Comparing `batframes-1.0.0.7/nuitka_dependency_files.py` & `batframes-1.0.1/nuitka_dependency_files.py`

 * *Files identical despite different names*

### Comparing `batframes-1.0.0.7/setup.py` & `batframes-1.0.1/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -183,253 +183,243 @@
 00000b60: 6f6e 6669 6764 6972 2c20 5b6f 7267 696e  onfigdir, [orgin
 00000b70: 636f 6e66 6967 6669 6c65 5d29 2c0d 0a20  configfile]),.. 
 00000b80: 2020 2020 2020 205d 0d0a 2020 2020 7265         ]..    re
 00000b90: 7475 726e 2064 6174 615f 6669 6c65 730d  turn data_files.
 00000ba0: 0a0d 0a0d 0a73 6574 7570 280d 0a20 2020  .....setup(..   
 00000bb0: 206e 616d 653d 2762 6174 6672 616d 6573   name='batframes
 00000bc0: 272c 0d0a 2020 2020 7665 7273 696f 6e3d  ',..    version=
-00000bd0: 2731 2e30 2e30 2e37 272c 0d0a 2020 2020  '1.0.0.7',..    
-00000be0: 6465 7363 7269 7074 696f 6e3d 27e5 8faf  description='...
-00000bf0: e4bb a5e9 858d e7bd aee5 b086 e5a4 9ae4  ................
-00000c00: b8aa e58f afe6 89a7 e8a1 8ce6 9687 e4bb  ................
-00000c10: b6e5 928c e586 85e9 83a8 e591 bde4 bba4  ................
-00000c20: e4b8 b2e6 8ea5 e688 90e4 b880 e4b8 aae5  ................
-00000c30: ae8c e695 b4e5 91bd e4bb a4e6 89a7 e8a1  ................
-00000c40: 8ce7 9a84 e6a1 86e6 9eb6 e5b7 a5e5 85b7  ................
-00000c50: e380 82ef bc88 e591 bde4 bba4 e694 afe6  ................
-00000c60: 8c81 20e5 a49a e4b8 aa6f 7074 696f 6ee9  .. ......option.
-00000c70: 8089 e9a1 b9ef bc89 272c 0d0a 2020 2020  ........',..    
-00000c80: 6175 7468 6f72 3d27 4672 616e 6b20 476f  author='Frank Go
-00000c90: 6e67 272c 0d0a 2020 2020 6175 7468 6f72  ng',..    author
-00000ca0: 5f65 6d61 696c 3d27 3538 3339 3833 3731  _email='58398371
-00000cb0: 3640 7171 2e63 6f6d 272c 0d0a 2020 2020  6@qq.com',..    
-00000cc0: 7061 636b 6167 6573 3d66 696e 645f 7061  packages=find_pa
-00000cd0: 636b 6167 6573 2829 2c20 2020 2020 2020  ckages(),       
-00000ce0: 2023 20e8 a1a8 e7a4 bae4 bda0 e8a6 81e5   # .............
-00000cf0: b081 e8a3 85e7 9a84 e58c 85ef bc8c 6669  ..............fi
-00000d00: 6e64 5f70 6163 6b61 6765 73e7 94a8 e4ba  nd_packages.....
-00000d10: 8ee7 b3bb e7bb 9fe8 87aa e58a a8e4 bb8e  ................
-00000d20: e5bd 93e5 898d e79b aee5 bd95 e5bc 80e5  ................
-00000d30: a78b e689 bee5 8c85 0d0a 2020 2020 6c69  ..........    li
-00000d40: 6365 6e73 653d 224d 4954 222c 0d0a 2020  cense="MIT",..  
-00000d50: 2020 7079 5f6d 6f64 756c 6573 3d5b 2762    py_modules=['b
-00000d60: 6174 6672 616d 655f 6d61 696e 272c 2027  atframe_main', '
-00000d70: 6261 745f 6d65 6e75 5f61 7574 6f27 2c20  bat_menu_auto', 
-00000d80: 2762 6174 5f66 756e 6374 696f 6e5f 6361  'bat_function_ca
-00000d90: 6c6c 5f64 6566 696e 6527 2c20 276e 7569  ll_define', 'nui
-00000da0: 746b 615f 6465 7065 6e64 656e 6379 5f66  tka_dependency_f
-00000db0: 696c 6573 275d 2c0d 0a20 2020 2069 6e73  iles'],..    ins
-00000dc0: 7461 6c6c 5f72 6571 7569 7265 733d 5b27  tall_requires=['
-00000dd0: 7061 6e64 6173 7e3d 312e 352e 3227 2c20  pandas~=1.5.2', 
-00000de0: 276e 756d 7079 7e3d 312e 3234 2e31 272c  'numpy~=1.24.1',
-00000df0: 2027 6f70 656e 7079 786c 272c 2027 6172   'openpyxl', 'ar
-00000e00: 6770 6172 7365 272c 2027 7061 7468 6c69  gparse', 'pathli
-00000e10: 6227 2c0d 0a20 2020 2020 2020 2020 2020  b',..           
-00000e20: 2020 2020 2020 2020 2020 2027 7365 6c65             'sele
-00000e30: 6e69 756d 272c 2027 7265 7175 6573 7473  nium', 'requests
-00000e40: 272c 2027 786c 7264 272c 2027 626f 7474  ', 'xlrd', 'bott
-00000e50: 6c65 272c 2027 5079 5369 6d70 6c65 4755  le', 'PySimpleGU
-00000e60: 4927 2c20 2770 7265 7474 7974 6162 6c65  I', 'prettytable
-00000e70: 272c 0d0a 2020 2020 2020 2020 2020 2020  ',..            
-00000e80: 2020 2020 2020 2020 2020 2763 6861 7264            'chard
-00000e90: 6574 272c 2027 6e75 6974 6b61 272c 2027  et', 'nuitka', '
-00000ea0: 5079 5174 3527 2c20 2770 7963 7279 7074  PyQt5', 'pycrypt
-00000eb0: 6f64 6f6d 6578 272c 2027 6461 7461 636f  odomex', 'dataco
-00000ec0: 6d70 7927 2c0d 0a20 2020 2020 2020 2020  mpy',..         
-00000ed0: 2020 2020 2020 2020 2020 2020 2027 7368               'sh
-00000ee0: 6f72 7475 7569 6427 2c20 2773 716c 616c  ortuuid', 'sqlal
-00000ef0: 6368 656d 793d 3d31 2e34 2e34 3627 2c20  chemy==1.4.46', 
-00000f00: 276d 7973 716c 2d63 6f6e 6e65 6374 6f72  'mysql-connector
-00000f10: 2d70 7974 686f 6e27 2c20 2769 7079 272c  -python', 'ipy',
-00000f20: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00000f30: 2020 2020 2020 2020 2770 6174 686f 7327          'pathos'
-00000f40: 2c20 2770 796d 7973 716c 272c 2027 636f  , 'pymysql', 'co
-00000f50: 6c6f 726c 6f67 272c 2027 6d61 7470 6c6f  lorlog', 'matplo
-00000f60: 746c 6962 272c 2027 7079 7069 6e79 696e  tlib', 'pypinyin
-00000f70: 272c 2027 6273 3427 2c0d 0a20 2020 2020  ', 'bs4',..     
-00000f80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000f90: 2027 7079 786c 7362 272c 2027 6a73 6f6e   'pyxlsb', 'json
-00000fa0: 6c69 6e65 7327 2c20 274a 696e 6a61 3227  lines', 'Jinja2'
-00000fb0: 2c20 2770 7367 7370 6563 6961 6c65 6c65  , 'psgspecialele
-00000fc0: 6d65 6e74 7327 2c20 2764 6674 7261 6e73  ments', 'dftrans
-00000fd0: 275d 2c0d 0a20 2020 2070 6163 6b61 6765  '],..    package
-00000fe0: 5f64 6174 613d 7b0d 0a20 2020 2020 2020  _data={..       
-00000ff0: 2022 6261 745f 696e 6e65 725f 6d6f 6475   "bat_inner_modu
-00001000: 6c65 223a 205b 2269 6e6e 6572 5f2a 2e70  le": ["inner_*.p
-00001010: 7922 2c20 222a 2e6d 6422 5d0d 0a20 2020  y", "*.md"]..   
-00001020: 207d 2c0d 0a20 2020 2064 6174 615f 6669   },..    data_fi
-00001030: 6c65 733d 696e 6974 5f64 6174 615f 6669  les=init_data_fi
-00001040: 6c65 7328 292c 0d0a 2020 2020 7572 6c3d  les(),..    url=
-00001050: 2768 7474 7073 3a2f 2f67 6974 6565 2e63  'https://gitee.c
-00001060: 6f6d 2f46 7261 6e6b 5f35 3833 3938 3337  om/Frank_5839837
-00001070: 3136 2f62 6174 6672 616d 6573 272c 0d0a  16/batframes',..
-00001080: 2020 2020 656e 7472 795f 706f 696e 7473      entry_points
-00001090: 3d7b 0d0a 2020 2020 2020 2020 2763 6f6e  ={..        'con
-000010a0: 736f 6c65 5f73 6372 6970 7473 273a 205b  sole_scripts': [
-000010b0: 0d0a 2020 2020 2020 2020 2020 2020 2762  ..            'b
-000010c0: 6174 6672 616d 6573 203d 2062 6174 6672  atframes = batfr
-000010d0: 616d 655f 6d61 696e 3a62 6174 5f6d 6169  ame_main:bat_mai
-000010e0: 6e27 0d0a 2020 2020 2020 2020 5d0d 0a20  n'..        ].. 
-000010f0: 2020 207d 0d0a 2020 2020 2320 636c 6173     }..    # clas
-00001100: 7369 6669 6572 733d 5b0d 0a20 2020 2023  sifiers=[..    #
-00001110: 2020 2020 2023 20e5 8f91 e5b1 95e6 97b6       # .........
-00001120: e69c 9f2c e5b8 b8e8 a781 e79a 84e5 a682  ...,............
-00001130: e4b8 8b0d 0a20 2020 2023 2020 2020 2023  .....    #     #
-00001140: 2020 2033 202d 2041 6c70 6861 0d0a 2020     3 - Alpha..  
-00001150: 2020 2320 2020 2020 2320 2020 3420 2d20    #     #   4 - 
-00001160: 4265 7461 0d0a 2020 2020 2320 2020 2020  Beta..    #     
-00001170: 2320 2020 3520 2d20 5072 6f64 7563 7469  #   5 - Producti
-00001180: 6f6e 2f53 7461 626c 650d 0a20 2020 2023  on/Stable..    #
-00001190: 2020 2020 2027 4465 7665 6c6f 706d 656e       'Developmen
-000011a0: 7420 5374 6174 7573 203a 3a20 3520 2d20  t Status :: 5 - 
-000011b0: 5374 6162 6c65 272c 0d0a 2020 2020 2320  Stable',..    # 
-000011c0: 2020 2020 2320 e5bc 80e5 8f91 e79a 84e7      # ..........
-000011d0: 9bae e6a0 87e7 94a8 e688 b70d 0a20 2020  .............   
-000011e0: 2023 2020 2020 2027 496e 7465 6e64 6564   #     'Intended
-000011f0: 2041 7564 6965 6e63 6520 3a3a 2044 6576   Audience :: Dev
-00001200: 656c 6f70 6572 7327 2c0d 0a20 2020 2023  elopers',..    #
-00001210: 2020 2020 2023 20e5 b19e e4ba 8ee4 bb80       # .........
-00001220: e4b9 88e7 b1bb e59e 8b0d 0a20 2020 2023  ...........    #
-00001230: 2020 2020 2027 546f 7069 6320 3a3a 2053       'Topic :: S
-00001240: 6f66 7477 6172 6520 4465 7665 6c6f 706d  oftware Developm
-00001250: 656e 7420 3a3a 2054 6f6f 6c73 272c 0d0a  ent :: Tools',..
-00001260: 2020 2020 2320 2020 2020 2320 e8ae b8e5      #     # ....
-00001270: 8faf e8af 81e4 bfa1 e681 af0d 0a20 2020  .............   
-00001280: 2023 2020 2020 2027 4c69 6365 6e73 6520   #     'License 
-00001290: 3a3a 204f 5349 2041 7070 726f 7665 6420  :: OSI Approved 
-000012a0: 3a3a 2042 5344 204c 6963 656e 7365 272c  :: BSD License',
-000012b0: 0d0a 2020 2020 2320 2020 2020 2320 e79b  ..    #     # ..
-000012c0: aee6 a087 2050 7974 686f 6e20 e789 88e6  .... Python ....
-000012d0: 9cac 0d0a 2020 2020 2320 2020 2020 2750  ....    #     'P
-000012e0: 726f 6772 616d 6d69 6e67 204c 616e 6775  rogramming Langu
-000012f0: 6167 6520 3a3a 2050 7974 686f 6e20 3a3a  age :: Python ::
-00001300: 2033 272c 0d0a 2020 2020 2320 2020 2020   3',..    #     
-00001310: 2750 726f 6772 616d 6d69 6e67 204c 616e  'Programming Lan
-00001320: 6775 6167 6520 3a3a 2050 7974 686f 6e20  guage :: Python 
-00001330: 3a3a 2033 2e36 272c 0d0a 2020 2020 2320  :: 3.6',..    # 
-00001340: 2020 2020 2750 726f 6772 616d 6d69 6e67      'Programming
-00001350: 204c 616e 6775 6167 6520 3a3a 2050 7974   Language :: Pyt
-00001360: 686f 6e20 3a3a 2033 2e37 272c 0d0a 2020  hon :: 3.7',..  
-00001370: 2020 2320 2020 2020 2750 726f 6772 616d    #     'Program
-00001380: 6d69 6e67 204c 616e 6775 6167 6520 3a3a  ming Language ::
-00001390: 2050 7974 686f 6e20 3a3a 2033 2e38 272c   Python :: 3.8',
-000013a0: 0d0a 2020 2020 2320 2020 2020 2750 726f  ..    #     'Pro
-000013b0: 6772 616d 6d69 6e67 204c 616e 6775 6167  gramming Languag
-000013c0: 6520 3a3a 2050 7974 686f 6e20 3a3a 2033  e :: Python :: 3
-000013d0: 2e39 272c 0d0a 2020 2020 2320 5d0d 0a29  .9',..    # ]..)
-000013e0: 0d0a 2727 270d 0a6e 616d 6520 3a20 e689  ..'''..name : ..
-000013f0: 93e5 8c85 e590 8ee5 8c85 e79a 84e6 9687  ................
-00001400: e4bb b6e5 908d 0d0a 7665 7273 696f 6e20  ........version 
-00001410: 3a20 e789 88e6 9cac e58f b70d 0a61 7574  : ...........aut
-00001420: 686f 7220 3a20 e4bd 9ce8 8085 0d0a 6175  hor : ........au
-00001430: 7468 6f72 5f65 6d61 696c 203a 20e4 bd9c  thor_email : ...
-00001440: e880 85e7 9a84 e982 aee7 aeb1 0d0a 7079  ..............py
-00001450: 5f6d 6f64 756c 6573 203a 20e8 a681 e689  _modules : .....
-00001460: 93e5 8c85 e79a 842e 7079 e696 87e4 bbb6  ........py......
-00001470: 0d0a 7061 636b 6167 6573 3a20 e689 93e5  ..packages: ....
-00001480: 8c85 e79a 8470 7974 686f 6ee6 9687 e4bb  .....python.....
-00001490: b6e5 a4b9 0d0a 696e 636c 7564 655f 7061  ......include_pa
-000014a0: 636b 6167 655f 6461 7461 203a 20e9 a1b9  ckage_data : ...
-000014b0: e79b aee9 878c e4bc 9ae6 9c89 e4b8 80e4  ................
-000014c0: ba9b e99d 9e70 79e6 9687 e4bb b62c e6af  .....py......,..
-000014d0: 94e5 a682 6874 6d6c e592 8c6a 73e7 ad89  ....html...js...
-000014e0: 2ce8 bf99 e697 b6e5 8099 e5b0 b1e8 a681  ,...............
-000014f0: e99d a069 6e63 6c75 6465 5f70 6163 6b61  ...include_packa
-00001500: 6765 5f64 6174 6120 e592 8c20 7061 636b  ge_data ... pack
-00001510: 6167 655f 6461 7461 20e6 9da5 e68c 87e5  age_data .......
-00001520: ae9a e4ba 86e3 8082 7061 636b 6167 655f  ........package_
-00001530: 6461 7461 3ae4 b880 e888 ace5 8699 e688  data:...........
-00001540: 907b e280 9879 6f75 725f 7061 636b 6167  .{...your_packag
-00001550: 655f 6e61 6d65 e280 993a 205b e280 9c66  e_name...: [...f
-00001560: 696c 6573 e280 9d5d 7d2c 2069 6e63 6c75  iles...]}, inclu
-00001570: 6465 5f70 6163 6b61 6765 5f64 6174 61e8  de_package_data.
-00001580: bf98 e6b2 a1e5 ae8c 2ce8 bf98 e99c 80e8  ........,.......
-00001590: a681 e4bf aee6 94b9 4d41 4e49 4645 5354  ........MANIFEST
-000015a0: 2e69 6ee6 9687 e4bb b62e 4d41 4e49 4645  .in.......MANIFE
-000015b0: 5354 2e69 6ee6 9687 e4bb b6e7 9a84 e8af  ST.in...........
-000015c0: ade6 b395 e4b8 ba3a 2069 6e63 6c75 6465  .......: include
-000015d0: 2078 7878 2f78 7878 2f78 7878 2f2e 696e   xxx/xxx/xxx/.in
-000015e0: 692f 28e6 8980 e69c 89e4 bba5 2e69 6e69  i/(..........ini
-000015f0: e7bb 93e5 b0be e79a 84e6 9687 e4bb b62c  ...............,
-00001600: e4b9 9fe5 8faf e4bb a5e7 9bb4 e68e a5e6  ................
-00001610: 8c87 e5ae 9ae6 9687 e4bb b6e5 908d 290d  ..............).
-00001620: 0a6c 6963 656e 7365 203a 20e6 94af e68c  .license : .....
-00001630: 81e7 9a84 e5bc 80e6 ba90 e58d 8fe8 aeae  ................
-00001640: 0d0a 6465 7363 7269 7074 696f 6e20 3a20  ..description : 
-00001650: e5af b9e9 a1b9 e79b aee7 ae80 e79f ade7  ................
-00001660: 9a84 e4b8 80e4 b8aa e5bd a2e5 aeb9 0d0a  ................
-00001670: 6578 745f 6d6f 6475 6c65 7320 3a20 e698  ext_modules : ..
-00001680: afe4 b880 e4b8 aae5 8c85 e590 ab45 7874  .............Ext
-00001690: 656e 7369 6f6e e5ae 9ee4 be8b e79a 84e5  ension..........
-000016a0: 8897 e8a1 a82c 4578 7465 6e73 696f 6ee7  .....,Extension.
-000016b0: 9a84 e5ae 9ae4 b989 e4b9 9fe6 9c89 e4b8  ................
-000016c0: 80e4 ba9b e58f 82e6 95b0 e380 820d 0a65  ...............e
-000016d0: 7874 5f70 6163 6b61 6765 203a 20e5 ae9a  xt_package : ...
-000016e0: e4b9 8965 7874 656e 7369 6f6e e79a 84e7  ...extension....
-000016f0: 9bb8 e5af b9e8 b7af e5be 840d 0a72 6571  .............req
-00001700: 7569 7265 7320 3a20 e5ae 9ae4 b989 e4be  uires : ........
-00001710: 9de8 b596 e593 aae4 ba9b e6a8 a1e5 9d97  ................
-00001720: 0d0a 7072 6f76 6964 6573 203a 20e5 ae9a  ..provides : ...
-00001730: e4b9 89e5 8faf e4bb a5e4 b8ba e593 aae4  ................
-00001740: ba9b e6a8 a1e5 9d97 e68f 90e4 be9b e4be  ................
-00001750: 9de8 b596 0d0a 6461 7461 5f66 696c 6573  ......data_files
-00001760: 203a e68c 87e5 ae9a e585 b6e4 bb96 e79a   :..............
-00001770: 84e4 b880 e4ba 9be6 9687 e4bb b628 e5a6  .............(..
-00001780: 82e9 858d e7bd aee6 9687 e4bb b629 2ce8  .............),.
-00001790: a784 e5ae 9ae4 ba86 e593 aae4 ba9b e696  ................
-000017a0: 87e4 bbb6 e8a2 abe5 ae89 e8a3 85e5 88b0  ................
-000017b0: e593 aae4 ba9b e79b aee5 bd95 e4b8 ade3  ................
-000017c0: 8082 e5a6 82e6 9e9c e79b aee5 bd95 e590  ................
-000017d0: 8de6 98af e79b b8e5 afb9 e8b7 afe5 be84  ................
-000017e0: 2ce5 8899 e698 afe7 9bb8 e5af b9e4 ba8e  ,...............
-000017f0: 7379 732e 7072 6566 6978 e688 9673 7973  sys.prefix...sys
-00001800: 2e65 7865 635f 7072 6566 6978 e79a 84e8  .exec_prefix....
-00001810: b7af e5be 84e3 8082 e5a6 82e6 9e9c e6b2  ................
-00001820: a1e6 9c89 e68f 90e4 be9b e6a8 a1e6 9dbf  ................
-00001830: 2ce4 bc9a e8a2 abe6 b7bb e58a a0e5 88b0  ,...............
-00001840: 4d41 4e49 4645 5354 e696 87e4 bbb6 e4b8  MANIFEST........
-00001850: ade3 8082 0d0a 2020 2020 2320 e5b8 8ce6  ......    # ....
-00001860: 9c9b e8a2 abe6 8993 e58c 85e7 9a84 e696  ................
-00001870: 87e4 bbb6 0d0a 2020 2020 7061 636b 6167  ......    packag
-00001880: 655f 6461 7461 3d7b 0d0a 2020 2020 2020  e_data={..      
-00001890: 2020 2727 3a5b 272a 2e74 7874 275d 2c0d    '':['*.txt'],.
-000018a0: 0a20 2020 2020 2020 2027 6261 6e64 7769  .        'bandwi
-000018b0: 6474 685f 7265 706f 7274 6572 273a 5b27  dth_reporter':['
-000018c0: 2a2e 7478 7427 5d0d 0a20 2020 2020 2020  *.txt']..       
-000018d0: 2020 2020 2020 2020 7d2c 0d0a 2020 2020          },..    
-000018e0: 2320 e4b8 8de6 8993 e58c 85e6 9f90 e4ba  # ..............
-000018f0: 9be6 9687 e4bb b60d 0a20 2020 2065 7863  .........    exc
-00001900: 6c75 6465 5f70 6163 6b61 6765 5f64 6174  lude_package_dat
-00001910: 613d 7b0d 0a20 2020 2020 2020 2027 6261  a={..        'ba
-00001920: 6e64 7769 6474 685f 7265 706f 7274 6572  ndwidth_reporter
-00001930: 273a 5b27 2a2e 7478 7427 5d0d 0a20 2020  ':['*.txt']..   
-00001940: 2020 2020 200d 0a20 2020 2020 2020 200d       ..        .
-00001950: 0a20 2020 2023 20e7 94a8 e69d a5e6 94af  .    # .........
-00001960: e68c 81e8 87aa e58a a8e7 949f e688 90e8  ................
-00001970: 849a e69c acef bc8c e5ae 89e8 a385 e590  ................
-00001980: 8ee4 bc9a e887 aae5 8aa8 e794 9fe6 8890  ................
-00001990: 202f 7573 722f 6269 6e2f 666f 6f20 e79a   /usr/bin/foo ..
-000019a0: 84e5 8faf e689 a7e8 a18c e696 87e4 bbb6  ................
-000019b0: 0d0a 2020 2020 2320 e8af a5e6 9687 e4bb  ..    # ........
-000019c0: b6e5 85a5 e58f a3e6 8c87 e590 9120 666f  ............. fo
-000019d0: 6f2f 6d61 696e 2e70 7920 e79a 846d 6169  o/main.py ...mai
-000019e0: 6e20 e587 bde6 95b0 0d0a 2020 2020 656e  n ........    en
-000019f0: 7472 795f 706f 696e 7473 3d7b 0d0a 2020  try_points={..  
-00001a00: 2020 2020 2020 2763 6f6e 736f 6c65 5f73        'console_s
-00001a10: 6372 6970 7473 273a 205b 0d0a 2020 2020  cripts': [..    
-00001a20: 2020 2020 2020 2020 2766 6f6f 203d 2066          'foo = f
-00001a30: 6f6f 2e6d 6169 6e3a 6d61 696e 270d 0a20  oo.main:main'.. 
-00001a40: 2020 2020 2020 205d 0d0a 2020 2020 7d2c         ]..    },
-00001a50: 0d0a 0d0a 2020 2020 2320 e5b0 8620 6269  ....    # ... bi
-00001a60: 6e2f 666f 6f2e 7368 20e5 928c 2062 6172  n/foo.sh ... bar
-00001a70: 2e70 7920 e884 9ae6 9cac efbc 8ce7 949f  .py ............
-00001a80: e688 90e5 88b0 e7b3 bbe7 bb9f 2050 4154  ............ PAT
-00001a90: 48e4 b8ad 0d0a 2020 2020 2320 e689 a7e8  H.....    # ....
-00001aa0: a18c 2070 7974 686f 6e20 7365 7475 702e  .. python setup.
-00001ab0: 7079 2069 6e73 7461 6c6c 20e5 908e 0d0a  py install .....
-00001ac0: 2020 2020 2320 e4bc 9ae7 949f e688 9020      # ......... 
-00001ad0: e5a6 8220 2f75 7372 2f62 696e 2f66 6f6f  ... /usr/bin/foo
-00001ae0: 2e73 6820 e592 8c20 e5a6 8220 2f75 7372  .sh ... ... /usr
-00001af0: 2f62 696e 2f62 6172 2e70 790d 0a20 2020  /bin/bar.py..   
-00001b00: 2073 6372 6970 7473 3d5b 2762 696e 2f66   scripts=['bin/f
-00001b10: 6f6f 2e73 6827 2c20 2762 6172 2e70 7927  oo.sh', 'bar.py'
-00001b20: 5d0d 0a27 2727 0d0a 0d0a 0d0a            ]..'''......
+00000bd0: 2731 2e30 2e31 272c 0d0a 2020 2020 6465  '1.0.1',..    de
+00000be0: 7363 7269 7074 696f 6e3d 27e5 8faf e4bb  scription='.....
+00000bf0: a5e9 858d e7bd aee5 b086 e5a4 9ae4 b8aa  ................
+00000c00: e58f afe6 89a7 e8a1 8ce6 9687 e4bb b6e5  ................
+00000c10: 928c e586 85e9 83a8 e591 bde4 bba4 e4b8  ................
+00000c20: b2e6 8ea5 e688 90e4 b880 e4b8 aae5 ae8c  ................
+00000c30: e695 b4e5 91bd e4bb a4e6 89a7 e8a1 8ce7  ................
+00000c40: 9a84 e6a1 86e6 9eb6 e5b7 a5e5 85b7 e380  ................
+00000c50: 82ef bc88 e591 bde4 bba4 e694 afe6 8c81  ................
+00000c60: 20e5 a49a e4b8 aa6f 7074 696f 6ee9 8089   ......option...
+00000c70: e9a1 b9ef bc89 272c 0d0a 2020 2020 6175  ......',..    au
+00000c80: 7468 6f72 3d27 4672 616e 6b20 476f 6e67  thor='Frank Gong
+00000c90: 272c 0d0a 2020 2020 6175 7468 6f72 5f65  ',..    author_e
+00000ca0: 6d61 696c 3d27 3538 3339 3833 3731 3640  mail='583983716@
+00000cb0: 7171 2e63 6f6d 272c 0d0a 2020 2020 7061  qq.com',..    pa
+00000cc0: 636b 6167 6573 3d66 696e 645f 7061 636b  ckages=find_pack
+00000cd0: 6167 6573 2829 2c20 2020 2020 2020 2023  ages(),        #
+00000ce0: 20e8 a1a8 e7a4 bae4 bda0 e8a6 81e5 b081   ...............
+00000cf0: e8a3 85e7 9a84 e58c 85ef bc8c 6669 6e64  ............find
+00000d00: 5f70 6163 6b61 6765 73e7 94a8 e4ba 8ee7  _packages.......
+00000d10: b3bb e7bb 9fe8 87aa e58a a8e4 bb8e e5bd  ................
+00000d20: 93e5 898d e79b aee5 bd95 e5bc 80e5 a78b  ................
+00000d30: e689 bee5 8c85 0d0a 2020 2020 6c69 6365  ........    lice
+00000d40: 6e73 653d 2242 5344 222c 0d0a 2020 2020  nse="BSD",..    
+00000d50: 7079 5f6d 6f64 756c 6573 3d5b 2762 6174  py_modules=['bat
+00000d60: 6672 616d 655f 6d61 696e 272c 2027 6261  frame_main', 'ba
+00000d70: 745f 6d65 6e75 5f61 7574 6f27 2c20 2762  t_menu_auto', 'b
+00000d80: 6174 5f66 756e 6374 696f 6e5f 6361 6c6c  at_function_call
+00000d90: 5f64 6566 696e 6527 2c20 276e 7569 746b  _define', 'nuitk
+00000da0: 615f 6465 7065 6e64 656e 6379 5f66 696c  a_dependency_fil
+00000db0: 6573 275d 2c0d 0a20 2020 2069 6e73 7461  es'],..    insta
+00000dc0: 6c6c 5f72 6571 7569 7265 733d 5b27 7061  ll_requires=['pa
+00000dd0: 6e64 6173 7e3d 312e 352e 3227 2c20 276e  ndas~=1.5.2', 'n
+00000de0: 756d 7079 7e3d 312e 3234 2e31 272c 2027  umpy~=1.24.1', '
+00000df0: 6f70 656e 7079 786c 272c 2027 6172 6770  openpyxl', 'argp
+00000e00: 6172 7365 272c 2027 7061 7468 6c69 6227  arse', 'pathlib'
+00000e10: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
+00000e20: 2020 2020 2020 2020 2027 7365 6c65 6e69           'seleni
+00000e30: 756d 272c 2027 7265 7175 6573 7473 272c  um', 'requests',
+00000e40: 2027 786c 7264 272c 2027 626f 7474 6c65   'xlrd', 'bottle
+00000e50: 272c 2027 5079 5369 6d70 6c65 4755 497e  ', 'PySimpleGUI~
+00000e60: 3d34 2e35 392e 3027 2c20 2770 7265 7474  =4.59.0', 'prett
+00000e70: 7974 6162 6c65 272c 0d0a 2020 2020 2020  ytable',..      
+00000e80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000e90: 2763 6861 7264 6574 272c 2027 6e75 6974  'chardet', 'nuit
+00000ea0: 6b61 272c 2027 5079 5174 3527 2c20 2770  ka', 'PyQt5', 'p
+00000eb0: 7963 7279 7074 6f64 6f6d 6578 272c 2027  ycryptodomex', '
+00000ec0: 6461 7461 636f 6d70 7927 2c0d 0a20 2020  datacompy',..   
+00000ed0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000ee0: 2020 2027 7368 6f72 7475 7569 6427 2c20     'shortuuid', 
+00000ef0: 2773 716c 616c 6368 656d 793d 3d31 2e34  'sqlalchemy==1.4
+00000f00: 2e34 3627 2c20 276d 7973 716c 2d63 6f6e  .46', 'mysql-con
+00000f10: 6e65 6374 6f72 2d70 7974 686f 6e27 2c20  nector-python', 
+00000f20: 2769 7079 272c 0d0a 2020 2020 2020 2020  'ipy',..        
+00000f30: 2020 2020 2020 2020 2020 2020 2020 2770                'p
+00000f40: 6174 686f 7327 2c20 2770 796d 7973 716c  athos', 'pymysql
+00000f50: 272c 2027 636f 6c6f 726c 6f67 272c 2027  ', 'colorlog', '
+00000f60: 6d61 7470 6c6f 746c 6962 7e3d 332e 372e  matplotlib~=3.7.
+00000f70: 3227 2c20 2770 7970 696e 7969 6e27 2c20  2', 'pypinyin', 
+00000f80: 2762 7334 272c 0d0a 2020 2020 2020 2020  'bs4',..        
+00000f90: 2020 2020 2020 2020 2020 2020 2020 2770                'p
+00000fa0: 7978 6c73 6227 2c20 276a 736f 6e6c 696e  yxlsb', 'jsonlin
+00000fb0: 6573 272c 2027 4a69 6e6a 6132 272c 2027  es', 'Jinja2', '
+00000fc0: 7073 6773 7065 6369 616c 656c 656d 656e  psgspecialelemen
+00000fd0: 7473 272c 2027 4446 5472 616e 7327 5d2c  ts', 'DFTrans'],
+00000fe0: 0d0a 2020 2020 7061 636b 6167 655f 6461  ..    package_da
+00000ff0: 7461 3d7b 0d0a 2020 2020 2020 2020 2262  ta={..        "b
+00001000: 6174 5f69 6e6e 6572 5f6d 6f64 756c 6522  at_inner_module"
+00001010: 3a20 5b22 696e 6e65 725f 2a2e 7079 222c  : ["inner_*.py",
+00001020: 2022 2a2e 6d64 225d 0d0a 2020 2020 7d2c   "*.md"]..    },
+00001030: 0d0a 2020 2020 6461 7461 5f66 696c 6573  ..    data_files
+00001040: 3d69 6e69 745f 6461 7461 5f66 696c 6573  =init_data_files
+00001050: 2829 2c0d 0a20 2020 2023 2063 6c61 7373  (),..    # class
+00001060: 6966 6965 7273 3d5b 0d0a 2020 2020 2320  ifiers=[..    # 
+00001070: 2020 2020 2320 e58f 91e5 b195 e697 b6e6      # ..........
+00001080: 9c9f 2ce5 b8b8 e8a7 81e7 9a84 e5a6 82e4  ..,.............
+00001090: b88b 0d0a 2020 2020 2320 2020 2020 2320  ....    #     # 
+000010a0: 2020 3320 2d20 416c 7068 610d 0a20 2020    3 - Alpha..   
+000010b0: 2023 2020 2020 2023 2020 2034 202d 2042   #     #   4 - B
+000010c0: 6574 610d 0a20 2020 2023 2020 2020 2023  eta..    #     #
+000010d0: 2020 2035 202d 2050 726f 6475 6374 696f     5 - Productio
+000010e0: 6e2f 5374 6162 6c65 0d0a 2020 2020 2320  n/Stable..    # 
+000010f0: 2020 2020 2744 6576 656c 6f70 6d65 6e74      'Development
+00001100: 2053 7461 7475 7320 3a3a 2035 202d 2053   Status :: 5 - S
+00001110: 7461 626c 6527 2c0d 0a20 2020 2023 2020  table',..    #  
+00001120: 2020 2023 20e5 bc80 e58f 91e7 9a84 e79b     # ...........
+00001130: aee6 a087 e794 a8e6 88b7 0d0a 2020 2020  ............    
+00001140: 2320 2020 2020 2749 6e74 656e 6465 6420  #     'Intended 
+00001150: 4175 6469 656e 6365 203a 3a20 4465 7665  Audience :: Deve
+00001160: 6c6f 7065 7273 272c 0d0a 2020 2020 2320  lopers',..    # 
+00001170: 2020 2020 2320 e5b1 9ee4 ba8e e4bb 80e4      # ..........
+00001180: b988 e7b1 bbe5 9e8b 0d0a 2020 2020 2320  ..........    # 
+00001190: 2020 2020 2754 6f70 6963 203a 3a20 536f      'Topic :: So
+000011a0: 6674 7761 7265 2044 6576 656c 6f70 6d65  ftware Developme
+000011b0: 6e74 203a 3a20 546f 6f6c 7327 2c0d 0a20  nt :: Tools',.. 
+000011c0: 2020 2023 2020 2020 2023 20e8 aeb8 e58f     #     # .....
+000011d0: afe8 af81 e4bf a1e6 81af 0d0a 2020 2020  ............    
+000011e0: 2320 2020 2020 274c 6963 656e 7365 203a  #     'License :
+000011f0: 3a20 4f53 4920 4170 7072 6f76 6564 203a  : OSI Approved :
+00001200: 3a20 4253 4420 4c69 6365 6e73 6527 2c0d  : BSD License',.
+00001210: 0a20 2020 2023 2020 2020 2023 20e7 9bae  .    #     # ...
+00001220: e6a0 8720 5079 7468 6f6e 20e7 8988 e69c  ... Python .....
+00001230: ac0d 0a20 2020 2023 2020 2020 2027 5072  ...    #     'Pr
+00001240: 6f67 7261 6d6d 696e 6720 4c61 6e67 7561  ogramming Langua
+00001250: 6765 203a 3a20 5079 7468 6f6e 203a 3a20  ge :: Python :: 
+00001260: 3327 2c0d 0a20 2020 2023 2020 2020 2027  3',..    #     '
+00001270: 5072 6f67 7261 6d6d 696e 6720 4c61 6e67  Programming Lang
+00001280: 7561 6765 203a 3a20 5079 7468 6f6e 203a  uage :: Python :
+00001290: 3a20 332e 3627 2c0d 0a20 2020 2023 2020  : 3.6',..    #  
+000012a0: 2020 2027 5072 6f67 7261 6d6d 696e 6720     'Programming 
+000012b0: 4c61 6e67 7561 6765 203a 3a20 5079 7468  Language :: Pyth
+000012c0: 6f6e 203a 3a20 332e 3727 2c0d 0a20 2020  on :: 3.7',..   
+000012d0: 2023 2020 2020 2027 5072 6f67 7261 6d6d   #     'Programm
+000012e0: 696e 6720 4c61 6e67 7561 6765 203a 3a20  ing Language :: 
+000012f0: 5079 7468 6f6e 203a 3a20 332e 3827 2c0d  Python :: 3.8',.
+00001300: 0a20 2020 2023 2020 2020 2027 5072 6f67  .    #     'Prog
+00001310: 7261 6d6d 696e 6720 4c61 6e67 7561 6765  ramming Language
+00001320: 203a 3a20 5079 7468 6f6e 203a 3a20 332e   :: Python :: 3.
+00001330: 3927 2c0d 0a20 2020 2023 205d 0d0a 290d  9',..    # ]..).
+00001340: 0a27 2727 0d0a 6e61 6d65 203a 20e6 8993  .'''..name : ...
+00001350: e58c 85e5 908e e58c 85e7 9a84 e696 87e4  ................
+00001360: bbb6 e590 8d0d 0a76 6572 7369 6f6e 203a  .......version :
+00001370: 20e7 8988 e69c ace5 8fb7 0d0a 6175 7468   ...........auth
+00001380: 6f72 203a 20e4 bd9c e880 850d 0a61 7574  or : ........aut
+00001390: 686f 725f 656d 6169 6c20 3a20 e4bd 9ce8  hor_email : ....
+000013a0: 8085 e79a 84e9 82ae e7ae b10d 0a70 795f  .............py_
+000013b0: 6d6f 6475 6c65 7320 3a20 e8a6 81e6 8993  modules : ......
+000013c0: e58c 85e7 9a84 2e70 79e6 9687 e4bb b60d  .......py.......
+000013d0: 0a70 6163 6b61 6765 733a 20e6 8993 e58c  .packages: .....
+000013e0: 85e7 9a84 7079 7468 6f6e e696 87e4 bbb6  ....python......
+000013f0: e5a4 b90d 0a69 6e63 6c75 6465 5f70 6163  .....include_pac
+00001400: 6b61 6765 5f64 6174 6120 3a20 e9a1 b9e7  kage_data : ....
+00001410: 9bae e987 8ce4 bc9a e69c 89e4 b880 e4ba  ................
+00001420: 9be9 9d9e 7079 e696 87e4 bbb6 2ce6 af94  ....py......,...
+00001430: e5a6 8268 746d 6ce5 928c 6a73 e7ad 892c  ...html...js...,
+00001440: e8bf 99e6 97b6 e580 99e5 b0b1 e8a6 81e9  ................
+00001450: 9da0 696e 636c 7564 655f 7061 636b 6167  ..include_packag
+00001460: 655f 6461 7461 20e5 928c 2070 6163 6b61  e_data ... packa
+00001470: 6765 5f64 6174 6120 e69d a5e6 8c87 e5ae  ge_data ........
+00001480: 9ae4 ba86 e380 8270 6163 6b61 6765 5f64  .......package_d
+00001490: 6174 613a e4b8 80e8 88ac e586 99e6 8890  ata:............
+000014a0: 7be2 8098 796f 7572 5f70 6163 6b61 6765  {...your_package
+000014b0: 5f6e 616d 65e2 8099 3a20 5be2 809c 6669  _name...: [...fi
+000014c0: 6c65 73e2 809d 5d7d 2c20 696e 636c 7564  les...]}, includ
+000014d0: 655f 7061 636b 6167 655f 6461 7461 e8bf  e_package_data..
+000014e0: 98e6 b2a1 e5ae 8c2c e8bf 98e9 9c80 e8a6  .......,........
+000014f0: 81e4 bfae e694 b94d 414e 4946 4553 542e  .......MANIFEST.
+00001500: 696e e696 87e4 bbb6 2e4d 414e 4946 4553  in.......MANIFES
+00001510: 542e 696e e696 87e4 bbb6 e79a 84e8 afad  T.in............
+00001520: e6b3 95e4 b8ba 3a20 696e 636c 7564 6520  ......: include 
+00001530: 7878 782f 7878 782f 7878 782f 2e69 6e69  xxx/xxx/xxx/.ini
+00001540: 2f28 e689 80e6 9c89 e4bb a52e 696e 69e7  /(..........ini.
+00001550: bb93 e5b0 bee7 9a84 e696 87e4 bbb6 2ce4  ..............,.
+00001560: b99f e58f afe4 bba5 e79b b4e6 8ea5 e68c  ................
+00001570: 87e5 ae9a e696 87e4 bbb6 e590 8d29 0d0a  .............)..
+00001580: 6c69 6365 6e73 6520 3a20 e694 afe6 8c81  license : ......
+00001590: e79a 84e5 bc80 e6ba 90e5 8d8f e8ae ae0d  ................
+000015a0: 0a64 6573 6372 6970 7469 6f6e 203a 20e5  .description : .
+000015b0: afb9 e9a1 b9e7 9bae e7ae 80e7 9fad e79a  ................
+000015c0: 84e4 b880 e4b8 aae5 bda2 e5ae b90d 0a65  ...............e
+000015d0: 7874 5f6d 6f64 756c 6573 203a 20e6 98af  xt_modules : ...
+000015e0: e4b8 80e4 b8aa e58c 85e5 90ab 4578 7465  ............Exte
+000015f0: 6e73 696f 6ee5 ae9e e4be 8be7 9a84 e588  nsion...........
+00001600: 97e8 a1a8 2c45 7874 656e 7369 6f6e e79a  ....,Extension..
+00001610: 84e5 ae9a e4b9 89e4 b99f e69c 89e4 b880  ................
+00001620: e4ba 9be5 8f82 e695 b0e3 8082 0d0a 6578  ..............ex
+00001630: 745f 7061 636b 6167 6520 3a20 e5ae 9ae4  t_package : ....
+00001640: b989 6578 7465 6e73 696f 6ee7 9a84 e79b  ..extension.....
+00001650: b8e5 afb9 e8b7 afe5 be84 0d0a 7265 7175  ............requ
+00001660: 6972 6573 203a 20e5 ae9a e4b9 89e4 be9d  ires : .........
+00001670: e8b5 96e5 93aa e4ba 9be6 a8a1 e59d 970d  ................
+00001680: 0a70 726f 7669 6465 7320 3a20 e5ae 9ae4  .provides : ....
+00001690: b989 e58f afe4 bba5 e4b8 bae5 93aa e4ba  ................
+000016a0: 9be6 a8a1 e59d 97e6 8f90 e4be 9be4 be9d  ................
+000016b0: e8b5 960d 0a64 6174 615f 6669 6c65 7320  .....data_files 
+000016c0: 3ae6 8c87 e5ae 9ae5 85b6 e4bb 96e7 9a84  :...............
+000016d0: e4b8 80e4 ba9b e696 87e4 bbb6 28e5 a682  ............(...
+000016e0: e985 8de7 bdae e696 87e4 bbb6 292c e8a7  ............),..
+000016f0: 84e5 ae9a e4ba 86e5 93aa e4ba 9be6 9687  ................
+00001700: e4bb b6e8 a2ab e5ae 89e8 a385 e588 b0e5  ................
+00001710: 93aa e4ba 9be7 9bae e5bd 95e4 b8ad e380  ................
+00001720: 82e5 a682 e69e 9ce7 9bae e5bd 95e5 908d  ................
+00001730: e698 afe7 9bb8 e5af b9e8 b7af e5be 842c  ...............,
+00001740: e588 99e6 98af e79b b8e5 afb9 e4ba 8e73  ...............s
+00001750: 7973 2e70 7265 6669 78e6 8896 7379 732e  ys.prefix...sys.
+00001760: 6578 6563 5f70 7265 6669 78e7 9a84 e8b7  exec_prefix.....
+00001770: afe5 be84 e380 82e5 a682 e69e 9ce6 b2a1  ................
+00001780: e69c 89e6 8f90 e4be 9be6 a8a1 e69d bf2c  ...............,
+00001790: e4bc 9ae8 a2ab e6b7 bbe5 8aa0 e588 b04d  ...............M
+000017a0: 414e 4946 4553 54e6 9687 e4bb b6e4 b8ad  ANIFEST.........
+000017b0: e380 820d 0a20 2020 2023 20e5 b88c e69c  .....    # .....
+000017c0: 9be8 a2ab e689 93e5 8c85 e79a 84e6 9687  ................
+000017d0: e4bb b60d 0a20 2020 2070 6163 6b61 6765  .....    package
+000017e0: 5f64 6174 613d 7b0d 0a20 2020 2020 2020  _data={..       
+000017f0: 2027 273a 5b27 2a2e 7478 7427 5d2c 0d0a   '':['*.txt'],..
+00001800: 2020 2020 2020 2020 2762 616e 6477 6964          'bandwid
+00001810: 7468 5f72 6570 6f72 7465 7227 3a5b 272a  th_reporter':['*
+00001820: 2e74 7874 275d 0d0a 2020 2020 2020 2020  .txt']..        
+00001830: 2020 2020 2020 207d 2c0d 0a20 2020 2023         },..    #
+00001840: 20e4 b88d e689 93e5 8c85 e69f 90e4 ba9b   ...............
+00001850: e696 87e4 bbb6 0d0a 2020 2020 6578 636c  ........    excl
+00001860: 7564 655f 7061 636b 6167 655f 6461 7461  ude_package_data
+00001870: 3d7b 0d0a 2020 2020 2020 2020 2762 616e  ={..        'ban
+00001880: 6477 6964 7468 5f72 6570 6f72 7465 7227  dwidth_reporter'
+00001890: 3a5b 272a 2e74 7874 275d 0d0a 2020 2020  :['*.txt']..    
+000018a0: 2020 2020 0d0a 2020 2020 2020 2020 0d0a      ..        ..
+000018b0: 2020 2020 2320 e794 a8e6 9da5 e694 afe6      # ..........
+000018c0: 8c81 e887 aae5 8aa8 e794 9fe6 8890 e884  ................
+000018d0: 9ae6 9cac efbc 8ce5 ae89 e8a3 85e5 908e  ................
+000018e0: e4bc 9ae8 87aa e58a a8e7 949f e688 9020  ............... 
+000018f0: 2f75 7372 2f62 696e 2f66 6f6f 20e7 9a84  /usr/bin/foo ...
+00001900: e58f afe6 89a7 e8a1 8ce6 9687 e4bb b60d  ................
+00001910: 0a20 2020 2023 20e8 afa5 e696 87e4 bbb6  .    # .........
+00001920: e585 a5e5 8fa3 e68c 87e5 9091 2066 6f6f  ............ foo
+00001930: 2f6d 6169 6e2e 7079 20e7 9a84 6d61 696e  /main.py ...main
+00001940: 20e5 87bd e695 b00d 0a20 2020 2065 6e74   ........    ent
+00001950: 7279 5f70 6f69 6e74 733d 7b0d 0a20 2020  ry_points={..   
+00001960: 2020 2020 2027 636f 6e73 6f6c 655f 7363       'console_sc
+00001970: 7269 7074 7327 3a20 5b0d 0a20 2020 2020  ripts': [..     
+00001980: 2020 2020 2020 2027 666f 6f20 3d20 666f         'foo = fo
+00001990: 6f2e 6d61 696e 3a6d 6169 6e27 0d0a 2020  o.main:main'..  
+000019a0: 2020 2020 2020 5d0d 0a20 2020 207d 2c0d        ]..    },.
+000019b0: 0a0d 0a20 2020 2023 20e5 b086 2062 696e  ...    # ... bin
+000019c0: 2f66 6f6f 2e73 6820 e592 8c20 6261 722e  /foo.sh ... bar.
+000019d0: 7079 20e8 849a e69c acef bc8c e794 9fe6  py .............
+000019e0: 8890 e588 b0e7 b3bb e7bb 9f20 5041 5448  ........... PATH
+000019f0: e4b8 ad0d 0a20 2020 2023 20e6 89a7 e8a1  .....    # .....
+00001a00: 8c20 7079 7468 6f6e 2073 6574 7570 2e70  . python setup.p
+00001a10: 7920 696e 7374 616c 6c20 e590 8e0d 0a20  y install ..... 
+00001a20: 2020 2023 20e4 bc9a e794 9fe6 8890 20e5     # ......... .
+00001a30: a682 202f 7573 722f 6269 6e2f 666f 6f2e  .. /usr/bin/foo.
+00001a40: 7368 20e5 928c 20e5 a682 202f 7573 722f  sh ... ... /usr/
+00001a50: 6269 6e2f 6261 722e 7079 0d0a 2020 2020  bin/bar.py..    
+00001a60: 7363 7269 7074 733d 5b27 6269 6e2f 666f  scripts=['bin/fo
+00001a70: 6f2e 7368 272c 2027 6261 722e 7079 275d  o.sh', 'bar.py']
+00001a80: 0d0a 2727 270d 0a0d 0a0d 0a              ..'''......
```

