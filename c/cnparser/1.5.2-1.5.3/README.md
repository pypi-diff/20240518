# Comparing `tmp/cnparser-1.5.2.tar.gz` & `tmp/cnparser-1.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cnparser-1.5.2.tar", last modified: Thu May 16 13:58:47 2024, max compression
+gzip compressed data, was "cnparser-1.5.3.tar", last modified: Fri May 17 23:34:46 2024, max compression
```

## Comparing `cnparser-1.5.2.tar` & `cnparser-1.5.3.tar`

### file list

```diff
@@ -1,24 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:58:47.657657 cnparser-1.5.2/
--rw-r--r--   0 runner    (1001) docker     (127)    35148 2024-05-16 13:58:33.000000 cnparser-1.5.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2728 2024-05-16 13:58:47.657657 cnparser-1.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2275 2024-05-16 13:58:33.000000 cnparser-1.5.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:58:47.653657 cnparser-1.5.2/cnparser/
--rw-r--r--   0 runner    (1001) docker     (127)      218 2024-05-16 13:58:33.000000 cnparser-1.5.2/cnparser/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:58:47.657657 cnparser-1.5.2/cnparser/config/
--rw-r--r--   0 runner    (1001) docker     (127)  1754761 2024-05-16 13:58:33.000000 cnparser-1.5.2/cnparser/config/eng_kana.json
--rw-r--r--   0 runner    (1001) docker     (127)     1146 2024-05-16 13:58:33.000000 cnparser-1.5.2/cnparser/config/file_id.json
--rw-r--r--   0 runner    (1001) docker     (127)      605 2024-05-16 13:58:33.000000 cnparser-1.5.2/cnparser/config/header.json
--rw-r--r--   0 runner    (1001) docker     (127)     3307 2024-05-16 13:58:33.000000 cnparser-1.5.2/cnparser/enrich.py
--rw-r--r--   0 runner    (1001) docker     (127)     5211 2024-05-16 13:58:33.000000 cnparser-1.5.2/cnparser/load.py
--rw-r--r--   0 runner    (1001) docker     (127)     1138 2024-05-16 13:58:33.000000 cnparser-1.5.2/cnparser/utility.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:58:47.657657 cnparser-1.5.2/cnparser.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2728 2024-05-16 13:58:47.000000 cnparser-1.5.2/cnparser.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      384 2024-05-16 13:58:47.000000 cnparser-1.5.2/cnparser.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 13:58:47.000000 cnparser-1.5.2/cnparser.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-05-16 13:58:47.000000 cnparser-1.5.2/cnparser.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-16 13:58:47.000000 cnparser-1.5.2/cnparser.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-16 13:58:47.657657 cnparser-1.5.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      675 2024-05-16 13:58:33.000000 cnparser-1.5.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:58:47.657657 cnparser-1.5.2/test/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 13:58:33.000000 cnparser-1.5.2/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1427 2024-05-16 13:58:33.000000 cnparser-1.5.2/test/test_load.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 23:34:46.734578 cnparser-1.5.3/
+-rw-r--r--   0 runner    (1001) docker     (127)    35148 2024-05-17 23:34:37.000000 cnparser-1.5.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2972 2024-05-17 23:34:46.734578 cnparser-1.5.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2519 2024-05-17 23:34:37.000000 cnparser-1.5.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 23:34:46.730578 cnparser-1.5.3/cnparser/
+-rw-r--r--   0 runner    (1001) docker     (127)      213 2024-05-17 23:34:37.000000 cnparser-1.5.3/cnparser/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 23:34:46.734578 cnparser-1.5.3/cnparser/config/
+-rw-r--r--   0 runner    (1001) docker     (127)  1754761 2024-05-17 23:34:37.000000 cnparser-1.5.3/cnparser/config/eng_kana.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1146 2024-05-17 23:34:37.000000 cnparser-1.5.3/cnparser/config/file_id.json
+-rw-r--r--   0 runner    (1001) docker     (127)      605 2024-05-17 23:34:37.000000 cnparser-1.5.3/cnparser/config/header.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1596 2024-05-17 23:34:37.000000 cnparser-1.5.3/cnparser/config/legal_entity.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3081 2024-05-17 23:34:37.000000 cnparser-1.5.3/cnparser/enrich.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5211 2024-05-17 23:34:37.000000 cnparser-1.5.3/cnparser/load.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1138 2024-05-17 23:34:37.000000 cnparser-1.5.3/cnparser/utility.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 23:34:46.734578 cnparser-1.5.3/cnparser.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2972 2024-05-17 23:34:46.000000 cnparser-1.5.3/cnparser.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      438 2024-05-17 23:34:46.000000 cnparser-1.5.3/cnparser.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-17 23:34:46.000000 cnparser-1.5.3/cnparser.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-05-17 23:34:46.000000 cnparser-1.5.3/cnparser.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-17 23:34:46.000000 cnparser-1.5.3/cnparser.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-17 23:34:46.734578 cnparser-1.5.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      675 2024-05-17 23:34:37.000000 cnparser-1.5.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 23:34:46.734578 cnparser-1.5.3/test/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 23:34:37.000000 cnparser-1.5.3/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1677 2024-05-17 23:34:37.000000 cnparser-1.5.3/test/test_enrich.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1427 2024-05-17 23:34:37.000000 cnparser-1.5.3/test/test_load.py
```

### Comparing `cnparser-1.5.2/LICENSE` & `cnparser-1.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `cnparser-1.5.2/PKG-INFO` & `cnparser-1.5.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cnparser
-Version: 1.5.2
+Version: 1.5.3
 Summary: cnparser is a parser library of Corporate Number Publication Site data.
 Home-page: https://github.com/new-village/cnparser
 Author: new-village
 License: GPLv3+
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: requests
@@ -33,28 +33,35 @@
 $ python setup.py install
 ```
     
 ## Usage
 This section demonstrates how to use this library to load and process data from the National Tax Agency's [Corporate Number Publication Site](https://www.houjin-bangou.nta.go.jp/).
 
 ### Direct Data Loading
-To load data for a specific prefecture, use the `load` function. By passing the prefecture name as an argument, you can obtain a DataFrame containing data for that prefecture.
-To execute the `load` function without specifying any arguments, data for all prefectures across Japan will be loaded. If you wish to load data for a specific prefecture, you must specify the prefecture name in Roman characters ([list of the supported prefecture](https://github.com/new-village/cnparser/blob/main/cnparser/config/file_id.json)) like below: 
+To download data for a specific prefecture, use the `load` function. By passing the prefecture name as an argument, you can obtain a DataFrame containing data for that prefecture.If you wish to download data for a specific prefecture, you must specify the prefecture name in Roman characters ([list of the supported prefectures](https://github.com/new-village/cnparser/blob/main/cnparser/config/file_id.json)).  
+To execute the `load` function without specifying any arguments, data for all prefectures across Japan will be downloaded. 
 ```
 >>> import cnparser
 >>> df = cnparser.load("Shimane")
 ```
 
 ### CSV Data Loading
 If you already have a downloaded CSV file, use the `read_csv` function. By passing the file path as an argument, you can obtain a DataFrame with headers from the CSV data.
 ```
 >>> import cnparser
 >>> df = cnparser.read_csv("path/to/data.csv")
 ```
 
+### Data Enrichment Functionality
+The `enrich` function adds a standardized furigana column `std_furigana` to the DataFrame. It processes data entry by converting `name` to furigana.
+```
+>>> import cnparser
+>>> df = cnparser.enrich(df)
+```
+
 ## Tools
 ### import_dict.py: Bilingual Emacspeak Project (BEP) Dictionary Import Tool
 This tool imports the [BEP dictionary](https://fastapi.metacpan.org/source/MASH/Lingua-JA-Yomi-0.01/lib/Lingua/JA) and generates a dictionary file for use with cnparser. It processes the bilingual mappings from English to Kana, ensuring that cnparser can accurately handle and transform data involving these language elements.
 ```
 $ cd /home/<USER>/analysis
 $ python enrich.py <FILE_PATH>
 ```
```

### Comparing `cnparser-1.5.2/README.md` & `cnparser-1.5.3/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -17,28 +17,35 @@
 $ python setup.py install
 ```
     
 ## Usage
 This section demonstrates how to use this library to load and process data from the National Tax Agency's [Corporate Number Publication Site](https://www.houjin-bangou.nta.go.jp/).
 
 ### Direct Data Loading
-To load data for a specific prefecture, use the `load` function. By passing the prefecture name as an argument, you can obtain a DataFrame containing data for that prefecture.
-To execute the `load` function without specifying any arguments, data for all prefectures across Japan will be loaded. If you wish to load data for a specific prefecture, you must specify the prefecture name in Roman characters ([list of the supported prefecture](https://github.com/new-village/cnparser/blob/main/cnparser/config/file_id.json)) like below: 
+To download data for a specific prefecture, use the `load` function. By passing the prefecture name as an argument, you can obtain a DataFrame containing data for that prefecture.If you wish to download data for a specific prefecture, you must specify the prefecture name in Roman characters ([list of the supported prefectures](https://github.com/new-village/cnparser/blob/main/cnparser/config/file_id.json)).  
+To execute the `load` function without specifying any arguments, data for all prefectures across Japan will be downloaded. 
 ```
 >>> import cnparser
 >>> df = cnparser.load("Shimane")
 ```
 
 ### CSV Data Loading
 If you already have a downloaded CSV file, use the `read_csv` function. By passing the file path as an argument, you can obtain a DataFrame with headers from the CSV data.
 ```
 >>> import cnparser
 >>> df = cnparser.read_csv("path/to/data.csv")
 ```
 
+### Data Enrichment Functionality
+The `enrich` function adds a standardized furigana column `std_furigana` to the DataFrame. It processes data entry by converting `name` to furigana.
+```
+>>> import cnparser
+>>> df = cnparser.enrich(df)
+```
+
 ## Tools
 ### import_dict.py: Bilingual Emacspeak Project (BEP) Dictionary Import Tool
 This tool imports the [BEP dictionary](https://fastapi.metacpan.org/source/MASH/Lingua-JA-Yomi-0.01/lib/Lingua/JA) and generates a dictionary file for use with cnparser. It processes the bilingual mappings from English to Kana, ensuring that cnparser can accurately handle and transform data involving these language elements.
 ```
 $ cd /home/<USER>/analysis
 $ python enrich.py <FILE_PATH>
 ```
```

### Comparing `cnparser-1.5.2/cnparser/config/eng_kana.json` & `cnparser-1.5.3/cnparser/config/eng_kana.json`

 * *Files identical despite different names*

### Comparing `cnparser-1.5.2/cnparser/config/file_id.json` & `cnparser-1.5.3/cnparser/config/file_id.json`

 * *Files identical despite different names*

### Comparing `cnparser-1.5.2/cnparser/config/header.json` & `cnparser-1.5.3/cnparser/config/header.json`

 * *Files identical despite different names*

### Comparing `cnparser-1.5.2/cnparser/load.py` & `cnparser-1.5.3/cnparser/load.py`

 * *Files identical despite different names*

### Comparing `cnparser-1.5.2/cnparser/utility.py` & `cnparser-1.5.3/cnparser/utility.py`

 * *Files identical despite different names*

### Comparing `cnparser-1.5.2/cnparser.egg-info/PKG-INFO` & `cnparser-1.5.3/cnparser.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cnparser
-Version: 1.5.2
+Version: 1.5.3
 Summary: cnparser is a parser library of Corporate Number Publication Site data.
 Home-page: https://github.com/new-village/cnparser
 Author: new-village
 License: GPLv3+
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: requests
@@ -33,28 +33,35 @@
 $ python setup.py install
 ```
     
 ## Usage
 This section demonstrates how to use this library to load and process data from the National Tax Agency's [Corporate Number Publication Site](https://www.houjin-bangou.nta.go.jp/).
 
 ### Direct Data Loading
-To load data for a specific prefecture, use the `load` function. By passing the prefecture name as an argument, you can obtain a DataFrame containing data for that prefecture.
-To execute the `load` function without specifying any arguments, data for all prefectures across Japan will be loaded. If you wish to load data for a specific prefecture, you must specify the prefecture name in Roman characters ([list of the supported prefecture](https://github.com/new-village/cnparser/blob/main/cnparser/config/file_id.json)) like below: 
+To download data for a specific prefecture, use the `load` function. By passing the prefecture name as an argument, you can obtain a DataFrame containing data for that prefecture.If you wish to download data for a specific prefecture, you must specify the prefecture name in Roman characters ([list of the supported prefectures](https://github.com/new-village/cnparser/blob/main/cnparser/config/file_id.json)).  
+To execute the `load` function without specifying any arguments, data for all prefectures across Japan will be downloaded. 
 ```
 >>> import cnparser
 >>> df = cnparser.load("Shimane")
 ```
 
 ### CSV Data Loading
 If you already have a downloaded CSV file, use the `read_csv` function. By passing the file path as an argument, you can obtain a DataFrame with headers from the CSV data.
 ```
 >>> import cnparser
 >>> df = cnparser.read_csv("path/to/data.csv")
 ```
 
+### Data Enrichment Functionality
+The `enrich` function adds a standardized furigana column `std_furigana` to the DataFrame. It processes data entry by converting `name` to furigana.
+```
+>>> import cnparser
+>>> df = cnparser.enrich(df)
+```
+
 ## Tools
 ### import_dict.py: Bilingual Emacspeak Project (BEP) Dictionary Import Tool
 This tool imports the [BEP dictionary](https://fastapi.metacpan.org/source/MASH/Lingua-JA-Yomi-0.01/lib/Lingua/JA) and generates a dictionary file for use with cnparser. It processes the bilingual mappings from English to Kana, ensuring that cnparser can accurately handle and transform data involving these language elements.
 ```
 $ cd /home/<USER>/analysis
 $ python enrich.py <FILE_PATH>
 ```
```

### Comparing `cnparser-1.5.2/setup.py` & `cnparser-1.5.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='cnparser',
-    version='1.5.2',
+    version='1.5.3',
     author='new-village',
     url='https://github.com/new-village/cnparser',
     description='cnparser is a parser library of Corporate Number Publication Site data.',
     long_description=long_description,
     long_description_content_type="text/markdown",
     license = 'GPLv3+',
     install_requires=['requests', 'bs4', 'pandas', 'pykakasi', 'kanjize==1.5.0', 'normalize-japanese-addresses==0.0.9'],
```

### Comparing `cnparser-1.5.2/test/test_load.py` & `cnparser-1.5.3/test/test_load.py`

 * *Files identical despite different names*

