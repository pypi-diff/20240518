# Comparing `tmp/dftrans-2.0.2.7.tar.gz` & `tmp/dftrans-2.0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dftrans-2.0.2.7.tar", last modified: Sun Mar 17 03:14:56 2024, max compression
+gzip compressed data, was "dftrans-2.0.2.8.tar", last modified: Sat May 18 16:32:02 2024, max compression
```

## Comparing `dftrans-2.0.2.7.tar` & `dftrans-2.0.2.8.tar`

### file list

```diff
@@ -1,24 +1,22 @@
-drwxrwxrwx   0        0        0        0 2024-03-17 03:14:56.320804 dftrans-2.0.2.7/
--rw-rw-rw-   0        0        0   316590 2024-03-17 01:56:42.000000 dftrans-2.0.2.7/DFTrans_main.py
--rw-rw-rw-   0        0        0     1539 2023-05-18 01:57:46.000000 dftrans-2.0.2.7/LICENSE
--rw-rw-rw-   0        0        0      552 2024-03-17 03:14:56.319803 dftrans-2.0.2.7/PKG-INFO
--rw-rw-rw-   0        0        0     1431 2023-05-18 01:35:35.000000 dftrans-2.0.2.7/README.md
-drwxrwxrwx   0        0        0        0 2024-03-17 03:14:56.289795 dftrans-2.0.2.7/config/
-drwxrwxrwx   0        0        0        0 2024-03-17 03:14:56.305800 dftrans-2.0.2.7/config/DFTrans/
--rw-rw-rw-   0        0        0   163319 2024-03-17 01:56:42.000000 dftrans-2.0.2.7/config/DFTrans/DFTrans_config.json
-drwxrwxrwx   0        0        0        0 2024-03-17 03:14:56.308801 dftrans-2.0.2.7/config/img/
--rw-rw-rw-   0        0        0    42148 2023-05-18 01:21:37.000000 dftrans-2.0.2.7/config/img/table_arrow9_transparent_256.png
--rw-rw-rw-   0        0        0    16958 2023-05-18 01:21:37.000000 dftrans-2.0.2.7/config/img/table_arrow9_transparent_64.ico
--rw-rw-rw-   0        0        0   209243 2024-03-17 01:56:43.000000 dftrans-2.0.2.7/df_excel_define.py
--rw-rw-rw-   0        0        0     3418 2023-04-06 04:23:37.000000 dftrans-2.0.2.7/df_excel_define_user.py
--rw-rw-rw-   0        0        0    17037 2023-04-18 14:54:25.000000 dftrans-2.0.2.7/df_excel_plot.py
--rw-rw-rw-   0        0        0     7706 2023-04-18 13:30:39.000000 dftrans-2.0.2.7/df_stock_define.py
-drwxrwxrwx   0        0        0        0 2024-03-17 03:14:56.317803 dftrans-2.0.2.7/dftrans.egg-info/
--rw-rw-rw-   0        0        0      552 2024-03-17 03:14:56.000000 dftrans-2.0.2.7/dftrans.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      431 2024-03-17 03:14:56.000000 dftrans-2.0.2.7/dftrans.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-17 03:14:56.000000 dftrans-2.0.2.7/dftrans.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       55 2024-03-17 03:14:56.000000 dftrans-2.0.2.7/dftrans.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      284 2024-03-17 03:14:56.000000 dftrans-2.0.2.7/dftrans.egg-info/requires.txt
--rw-rw-rw-   0        0        0       80 2024-03-17 03:14:56.000000 dftrans-2.0.2.7/dftrans.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-03-17 03:14:56.320804 dftrans-2.0.2.7/setup.cfg
--rw-rw-rw-   0        0        0     7432 2024-03-17 02:17:38.000000 dftrans-2.0.2.7/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-18 16:32:02.626119 dftrans-2.0.2.8/
+-rw-rw-rw-   0        0        0   316590 2024-05-18 14:55:54.000000 dftrans-2.0.2.8/DFTrans_main.py
+-rw-rw-rw-   0        0        0     1539 2024-05-18 14:55:54.000000 dftrans-2.0.2.8/LICENSE
+-rw-rw-rw-   0        0        0      552 2024-05-18 16:32:02.624118 dftrans-2.0.2.8/PKG-INFO
+-rw-rw-rw-   0        0        0     1431 2024-05-18 14:55:54.000000 dftrans-2.0.2.8/README.md
+drwxrwxrwx   0        0        0        0 2024-05-18 16:32:02.508514 dftrans-2.0.2.8/config/
+drwxrwxrwx   0        0        0        0 2024-05-18 16:32:02.588577 dftrans-2.0.2.8/config/img/
+-rw-rw-rw-   0        0        0    42148 2024-05-18 14:55:54.000000 dftrans-2.0.2.8/config/img/table_arrow9_transparent_256.png
+-rw-rw-rw-   0        0        0    16958 2024-05-18 14:55:54.000000 dftrans-2.0.2.8/config/img/table_arrow9_transparent_64.ico
+-rw-rw-rw-   0        0        0   209243 2024-05-18 14:56:01.000000 dftrans-2.0.2.8/df_excel_define.py
+-rw-rw-rw-   0        0        0     3418 2024-05-18 14:56:01.000000 dftrans-2.0.2.8/df_excel_define_user.py
+-rw-rw-rw-   0        0        0    17037 2024-05-18 14:56:01.000000 dftrans-2.0.2.8/df_excel_plot.py
+-rw-rw-rw-   0        0        0     7706 2024-05-18 14:56:01.000000 dftrans-2.0.2.8/df_stock_define.py
+drwxrwxrwx   0        0        0        0 2024-05-18 16:32:02.620120 dftrans-2.0.2.8/dftrans.egg-info/
+-rw-rw-rw-   0        0        0      552 2024-05-18 16:32:02.000000 dftrans-2.0.2.8/dftrans.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      396 2024-05-18 16:32:02.000000 dftrans-2.0.2.8/dftrans.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-18 16:32:02.000000 dftrans-2.0.2.8/dftrans.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       55 2024-05-18 16:32:02.000000 dftrans-2.0.2.8/dftrans.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      299 2024-05-18 16:32:02.000000 dftrans-2.0.2.8/dftrans.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       80 2024-05-18 16:32:02.000000 dftrans-2.0.2.8/dftrans.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-18 16:32:02.627117 dftrans-2.0.2.8/setup.cfg
+-rw-rw-rw-   0        0        0     7447 2024-05-18 16:03:25.000000 dftrans-2.0.2.8/setup.py
```

### Comparing `dftrans-2.0.2.7/DFTrans_main.py` & `dftrans-2.0.2.8/DFTrans_main.py`

 * *Files identical despite different names*

### Comparing `dftrans-2.0.2.7/LICENSE` & `dftrans-2.0.2.8/LICENSE`

 * *Files identical despite different names*

### Comparing `dftrans-2.0.2.7/PKG-INFO` & `dftrans-2.0.2.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dftrans
-Version: 2.0.2.7
+Version: 2.0.2.8
 Summary: 用于批量处理excel、sql数据库表、jsonl、csv等数据源的文件，并输出到数据库表或这excel文件
 Home-page: https://gitee.com/Frank_583983716/dftrans
 Author: Frank Gong
 Author-email: 583983716@qq.com
 License: BSD
 Description-Content-Type: text/x-rst
 License-File: LICENSE
```

### Comparing `dftrans-2.0.2.7/README.md` & `dftrans-2.0.2.8/README.md`

 * *Files identical despite different names*

### Comparing `dftrans-2.0.2.7/config/img/table_arrow9_transparent_256.png` & `dftrans-2.0.2.8/config/img/table_arrow9_transparent_256.png`

 * *Files identical despite different names*

### Comparing `dftrans-2.0.2.7/config/img/table_arrow9_transparent_64.ico` & `dftrans-2.0.2.8/config/img/table_arrow9_transparent_64.ico`

 * *Files identical despite different names*

### Comparing `dftrans-2.0.2.7/df_excel_define.py` & `dftrans-2.0.2.8/df_excel_define.py`

 * *Files identical despite different names*

### Comparing `dftrans-2.0.2.7/df_excel_define_user.py` & `dftrans-2.0.2.8/df_excel_define_user.py`

 * *Files identical despite different names*

### Comparing `dftrans-2.0.2.7/df_excel_plot.py` & `dftrans-2.0.2.8/df_excel_plot.py`

 * *Files identical despite different names*

### Comparing `dftrans-2.0.2.7/df_stock_define.py` & `dftrans-2.0.2.8/df_stock_define.py`

 * *Files identical despite different names*

### Comparing `dftrans-2.0.2.7/dftrans.egg-info/PKG-INFO` & `dftrans-2.0.2.8/dftrans.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dftrans
-Version: 2.0.2.7
+Version: 2.0.2.8
 Summary: 用于批量处理excel、sql数据库表、jsonl、csv等数据源的文件，并输出到数据库表或这excel文件
 Home-page: https://gitee.com/Frank_583983716/dftrans
 Author: Frank Gong
 Author-email: 583983716@qq.com
 License: BSD
 Description-Content-Type: text/x-rst
 License-File: LICENSE
```

### Comparing `dftrans-2.0.2.7/setup.py` & `dftrans-2.0.2.8/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -79,29 +79,29 @@
             (originconfigdir, [orginconfigfile]),
         ]
     return data_files
 
 
 setup(
     name='dftrans',
-    version='2.0.2.7',
+    version='2.0.2.8',
     description='用于批量处理excel、sql数据库表、jsonl、csv等数据源的文件，并输出到数据库表或这excel文件',
     author='Frank Gong',
     author_email='583983716@qq.com',
     packages=find_packages(),        # 表示你要封装的包，find_packages用于系统自动从当前目录开始找包
     license="BSD",
     url='https://gitee.com/Frank_583983716/dftrans',
     long_description='轻量级ETL工具，用于批量处理excel、sql数据库表、jsonl、csv等数据源的文件，并输出到数据库表或excel文件，可以对相关功能进行持续扩展',
     long_description_content_type="text/x-rst",
     py_modules=['DFTrans_main', 'df_excel_define', 'df_excel_define_user', 'df_excel_plot', 'df_stock_define'],
     install_requires=['pandas~=1.5.2', 'numpy~=1.24.1', 'openpyxl', 'argparse', 'pathlib',
-                      'selenium', 'requests', 'xlrd', 'bottle', 'PySimpleGUI',
+                      'selenium', 'requests', 'xlrd', 'bottle', 'PySimpleGUI~=4.59.0',
                       'chardet', 'nuitka', 'PyQt5', 'pycryptodomex', 'datacompy',
                       'shortuuid', 'sqlalchemy==1.4.46', 'mysql-connector-python', 'ipy',
-                      'pathos', 'pymysql', 'colorlog', 'matplotlib', 'pypinyin',
+                      'pathos', 'pymysql', 'colorlog', 'matplotlib~=3.7.2', 'pypinyin',
                       'pyxlsb', 'jsonlines', 'Jinja2', 'psgspecialelements'],
     data_files=init_data_files(),
     entry_points={
         'console_scripts': [
             'dftrans = DFTrans_main:DF_Trans_main']},
     # classifiers=[
     #     # 发展时期,常见的如下
```

