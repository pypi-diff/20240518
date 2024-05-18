# Comparing `tmp/cnparser-1.5.3.tar.gz` & `tmp/cnparser-1.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cnparser-1.5.3.tar", last modified: Fri May 17 23:34:46 2024, max compression
+gzip compressed data, was "cnparser-1.5.4.tar", last modified: Sat May 18 13:43:16 2024, max compression
```

## Comparing `cnparser-1.5.3.tar` & `cnparser-1.5.4.tar`

### file list

```diff
@@ -1,26 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 23:34:46.734578 cnparser-1.5.3/
--rw-r--r--   0 runner    (1001) docker     (127)    35148 2024-05-17 23:34:37.000000 cnparser-1.5.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2972 2024-05-17 23:34:46.734578 cnparser-1.5.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2519 2024-05-17 23:34:37.000000 cnparser-1.5.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 23:34:46.730578 cnparser-1.5.3/cnparser/
--rw-r--r--   0 runner    (1001) docker     (127)      213 2024-05-17 23:34:37.000000 cnparser-1.5.3/cnparser/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 23:34:46.734578 cnparser-1.5.3/cnparser/config/
--rw-r--r--   0 runner    (1001) docker     (127)  1754761 2024-05-17 23:34:37.000000 cnparser-1.5.3/cnparser/config/eng_kana.json
--rw-r--r--   0 runner    (1001) docker     (127)     1146 2024-05-17 23:34:37.000000 cnparser-1.5.3/cnparser/config/file_id.json
--rw-r--r--   0 runner    (1001) docker     (127)      605 2024-05-17 23:34:37.000000 cnparser-1.5.3/cnparser/config/header.json
--rw-r--r--   0 runner    (1001) docker     (127)     1596 2024-05-17 23:34:37.000000 cnparser-1.5.3/cnparser/config/legal_entity.json
--rw-r--r--   0 runner    (1001) docker     (127)     3081 2024-05-17 23:34:37.000000 cnparser-1.5.3/cnparser/enrich.py
--rw-r--r--   0 runner    (1001) docker     (127)     5211 2024-05-17 23:34:37.000000 cnparser-1.5.3/cnparser/load.py
--rw-r--r--   0 runner    (1001) docker     (127)     1138 2024-05-17 23:34:37.000000 cnparser-1.5.3/cnparser/utility.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 23:34:46.734578 cnparser-1.5.3/cnparser.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2972 2024-05-17 23:34:46.000000 cnparser-1.5.3/cnparser.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      438 2024-05-17 23:34:46.000000 cnparser-1.5.3/cnparser.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-17 23:34:46.000000 cnparser-1.5.3/cnparser.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-05-17 23:34:46.000000 cnparser-1.5.3/cnparser.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-17 23:34:46.000000 cnparser-1.5.3/cnparser.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-17 23:34:46.734578 cnparser-1.5.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      675 2024-05-17 23:34:37.000000 cnparser-1.5.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 23:34:46.734578 cnparser-1.5.3/test/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 23:34:37.000000 cnparser-1.5.3/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1677 2024-05-17 23:34:37.000000 cnparser-1.5.3/test/test_enrich.py
--rw-r--r--   0 runner    (1001) docker     (127)     1427 2024-05-17 23:34:37.000000 cnparser-1.5.3/test/test_load.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 13:43:16.117541 cnparser-1.5.4/
+-rw-r--r--   0 runner    (1001) docker     (127)    35148 2024-05-18 13:43:06.000000 cnparser-1.5.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3536 2024-05-18 13:43:16.117541 cnparser-1.5.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3164 2024-05-18 13:43:06.000000 cnparser-1.5.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 13:43:16.109541 cnparser-1.5.4/cnparser/
+-rw-r--r--   0 runner    (1001) docker     (127)      213 2024-05-18 13:43:06.000000 cnparser-1.5.4/cnparser/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 13:43:16.113541 cnparser-1.5.4/cnparser/config/
+-rw-r--r--   0 runner    (1001) docker     (127)  1754761 2024-05-18 13:43:06.000000 cnparser-1.5.4/cnparser/config/eng_kana.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1146 2024-05-18 13:43:06.000000 cnparser-1.5.4/cnparser/config/file_id.json
+-rw-r--r--   0 runner    (1001) docker     (127)      605 2024-05-18 13:43:06.000000 cnparser-1.5.4/cnparser/config/header.json
+-rw-r--r--   0 runner    (1001) docker     (127)      210 2024-05-18 13:43:06.000000 cnparser-1.5.4/cnparser/config/kind.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1596 2024-05-18 13:43:06.000000 cnparser-1.5.4/cnparser/config/legal_entity.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3235 2024-05-18 13:43:06.000000 cnparser-1.5.4/cnparser/enrich.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5211 2024-05-18 13:43:06.000000 cnparser-1.5.4/cnparser/load.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1138 2024-05-18 13:43:06.000000 cnparser-1.5.4/cnparser/utility.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 13:43:16.117541 cnparser-1.5.4/cnparser.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3536 2024-05-18 13:43:16.000000 cnparser-1.5.4/cnparser.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      464 2024-05-18 13:43:16.000000 cnparser-1.5.4/cnparser.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-18 13:43:16.000000 cnparser-1.5.4/cnparser.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-18 13:43:16.000000 cnparser-1.5.4/cnparser.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-18 13:43:16.000000 cnparser-1.5.4/cnparser.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-18 13:43:16.117541 cnparser-1.5.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      618 2024-05-18 13:43:06.000000 cnparser-1.5.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 13:43:16.117541 cnparser-1.5.4/test/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-18 13:43:06.000000 cnparser-1.5.4/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2194 2024-05-18 13:43:06.000000 cnparser-1.5.4/test/test_enrich.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1427 2024-05-18 13:43:06.000000 cnparser-1.5.4/test/test_load.py
```

### Comparing `cnparser-1.5.3/LICENSE` & `cnparser-1.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `cnparser-1.5.3/PKG-INFO` & `cnparser-1.5.4/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,67 +1,61 @@
-Metadata-Version: 2.1
-Name: cnparser
-Version: 1.5.3
-Summary: cnparser is a parser library of Corporate Number Publication Site data.
-Home-page: https://github.com/new-village/cnparser
-Author: new-village
-License: GPLv3+
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: requests
-Requires-Dist: bs4
-Requires-Dist: pandas
-Requires-Dist: pykakasi
-Requires-Dist: kanjize==1.5.0
-Requires-Dist: normalize-japanese-addresses==0.0.9
-
 # cnparser  
 [![Test](https://github.com/new-village/cnparser/actions/workflows/test.yaml/badge.svg)](https://github.com/new-village/cnparser/actions/workflows/test.yaml)  
 **cnparser** is a python library for loading and enrichment [Corporate Number Publication Site](https://www.houjin-bangou.nta.go.jp/en/) data that is provided from National Tax Agency Japan. cnparser only support to parse latest data now.   
   
 ## Installation  
 ----------------------
 cnparser is available on pip installation.
-```
+```shell:
 $ python -m pip install cnparser
 ```
   
 ### GitHub Install
 Installing the latest version from GitHub:  
-```
+```shell:
 $ git clone https://github.com/new-village/cnparser
 $ cd cnparser
 $ python setup.py install
 ```
     
 ## Usage
 This section demonstrates how to use this library to load and process data from the National Tax Agency's [Corporate Number Publication Site](https://www.houjin-bangou.nta.go.jp/).
 
 ### Direct Data Loading
 To download data for a specific prefecture, use the `load` function. By passing the prefecture name as an argument, you can obtain a DataFrame containing data for that prefecture.If you wish to download data for a specific prefecture, you must specify the prefecture name in Roman characters ([list of the supported prefectures](https://github.com/new-village/cnparser/blob/main/cnparser/config/file_id.json)).  
 To execute the `load` function without specifying any arguments, data for all prefectures across Japan will be downloaded. 
-```
+```python:
 >>> import cnparser
 >>> df = cnparser.load("Shimane")
 ```
 
 ### CSV Data Loading
 If you already have a downloaded CSV file, use the `read_csv` function. By passing the file path as an argument, you can obtain a DataFrame with headers from the CSV data.
-```
+```python:
 >>> import cnparser
 >>> df = cnparser.read_csv("path/to/data.csv")
 ```
 
 ### Data Enrichment Functionality
-The `enrich` function adds a standardized furigana column `std_furigana` to the DataFrame. It processes data entry by converting `name` to furigana.
-```
+The `enrich` function standardises and transforms the values of specific fields in the loaded DataFrame. 
+```python:
 >>> import cnparser
 >>> df = cnparser.enrich(df)
 ```
 
+The functions perform all processing, but it is possible to apply only specific processing by defining specific processing as an argument.
+```python:
+>>> import cnparser
+>>> df = cnparser.enrich(df, "enrich_kana" ...)
+```
+
+The processes supported by the `enrich` function are as follows:
+- `enrich_kana`: function adding a standardized furigana column `std_furigana` to the DataFrame. It processes data entry by converting `name` to kana, if `furigana` is NaN. Note that currently only kanji and katakana conversions are supported. Alphabet conversion is not supported.  
+- `enrich_kind`: function adding label of `kind` to `std_legal_entity`.  
+  
 ## Tools
 ### import_dict.py: Bilingual Emacspeak Project (BEP) Dictionary Import Tool
 This tool imports the [BEP dictionary](https://fastapi.metacpan.org/source/MASH/Lingua-JA-Yomi-0.01/lib/Lingua/JA) and generates a dictionary file for use with cnparser. It processes the bilingual mappings from English to Kana, ensuring that cnparser can accurately handle and transform data involving these language elements.
-```
+```shell:
 $ cd /home/<USER>/analysis
 $ python enrich.py <FILE_PATH>
 ```
```

### Comparing `cnparser-1.5.3/README.md` & `cnparser-1.5.4/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,51 +1,75 @@
+Metadata-Version: 2.1
+Name: cnparser
+Version: 1.5.4
+Summary: cnparser is a parser library of Corporate Number Publication Site data.
+Home-page: https://github.com/new-village/cnparser
+Author: new-village
+License: GPLv3+
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: requests
+Requires-Dist: bs4
+Requires-Dist: pandas
+Requires-Dist: pykakasi
+
 # cnparser  
 [![Test](https://github.com/new-village/cnparser/actions/workflows/test.yaml/badge.svg)](https://github.com/new-village/cnparser/actions/workflows/test.yaml)  
 **cnparser** is a python library for loading and enrichment [Corporate Number Publication Site](https://www.houjin-bangou.nta.go.jp/en/) data that is provided from National Tax Agency Japan. cnparser only support to parse latest data now.   
   
 ## Installation  
 ----------------------
 cnparser is available on pip installation.
-```
+```shell:
 $ python -m pip install cnparser
 ```
   
 ### GitHub Install
 Installing the latest version from GitHub:  
-```
+```shell:
 $ git clone https://github.com/new-village/cnparser
 $ cd cnparser
 $ python setup.py install
 ```
     
 ## Usage
 This section demonstrates how to use this library to load and process data from the National Tax Agency's [Corporate Number Publication Site](https://www.houjin-bangou.nta.go.jp/).
 
 ### Direct Data Loading
 To download data for a specific prefecture, use the `load` function. By passing the prefecture name as an argument, you can obtain a DataFrame containing data for that prefecture.If you wish to download data for a specific prefecture, you must specify the prefecture name in Roman characters ([list of the supported prefectures](https://github.com/new-village/cnparser/blob/main/cnparser/config/file_id.json)).  
 To execute the `load` function without specifying any arguments, data for all prefectures across Japan will be downloaded. 
-```
+```python:
 >>> import cnparser
 >>> df = cnparser.load("Shimane")
 ```
 
 ### CSV Data Loading
 If you already have a downloaded CSV file, use the `read_csv` function. By passing the file path as an argument, you can obtain a DataFrame with headers from the CSV data.
-```
+```python:
 >>> import cnparser
 >>> df = cnparser.read_csv("path/to/data.csv")
 ```
 
 ### Data Enrichment Functionality
-The `enrich` function adds a standardized furigana column `std_furigana` to the DataFrame. It processes data entry by converting `name` to furigana.
-```
+The `enrich` function standardises and transforms the values of specific fields in the loaded DataFrame. 
+```python:
 >>> import cnparser
 >>> df = cnparser.enrich(df)
 ```
 
+The functions perform all processing, but it is possible to apply only specific processing by defining specific processing as an argument.
+```python:
+>>> import cnparser
+>>> df = cnparser.enrich(df, "enrich_kana" ...)
+```
+
+The processes supported by the `enrich` function are as follows:
+- `enrich_kana`: function adding a standardized furigana column `std_furigana` to the DataFrame. It processes data entry by converting `name` to kana, if `furigana` is NaN. Note that currently only kanji and katakana conversions are supported. Alphabet conversion is not supported.  
+- `enrich_kind`: function adding label of `kind` to `std_legal_entity`.  
+  
 ## Tools
 ### import_dict.py: Bilingual Emacspeak Project (BEP) Dictionary Import Tool
 This tool imports the [BEP dictionary](https://fastapi.metacpan.org/source/MASH/Lingua-JA-Yomi-0.01/lib/Lingua/JA) and generates a dictionary file for use with cnparser. It processes the bilingual mappings from English to Kana, ensuring that cnparser can accurately handle and transform data involving these language elements.
-```
+```shell:
 $ cd /home/<USER>/analysis
 $ python enrich.py <FILE_PATH>
 ```
```

### Comparing `cnparser-1.5.3/cnparser/config/eng_kana.json` & `cnparser-1.5.4/cnparser/config/eng_kana.json`

 * *Files identical despite different names*

### Comparing `cnparser-1.5.3/cnparser/config/file_id.json` & `cnparser-1.5.4/cnparser/config/file_id.json`

 * *Files identical despite different names*

### Comparing `cnparser-1.5.3/cnparser/config/header.json` & `cnparser-1.5.4/cnparser/config/header.json`

 * *Files identical despite different names*

### Comparing `cnparser-1.5.3/cnparser/config/legal_entity.json` & `cnparser-1.5.4/cnparser/config/legal_entity.json`

 * *Files identical despite different names*

### Comparing `cnparser-1.5.3/cnparser/enrich.py` & `cnparser-1.5.4/cnparser/enrich.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,14 @@
+import multiprocessing as mp
 import re
-import pandas as pd
 import unicodedata
-import pykakasi
 import warnings
-import multiprocessing as mp
+
+import pandas as pd
+import pykakasi
 
 from cnparser.utility import load_config
 
 def enrich(df: pd.DataFrame, *processes) -> pd.DataFrame:
     """
     Enriches the DataFrame with additional data processing functions specified by the user.
 
@@ -84,16 +85,18 @@
     legal_entity_regex = '|'.join(map(re.escape, load_config("legal_entity")))
     cleaned_text = re.sub(legal_entity_regex, '', normalized_text)
     kks = pykakasi.kakasi()
     return "".join(item['kana'] for item in kks.convert(cleaned_text))
 
 def enrich_kind(df: pd.DataFrame) -> pd.DataFrame:
     """
-    Placeholder function for enriching DataFrame with kind data.
+    Maps the 'kind' column of the DataFrame to a standardized legal entity description.
 
     Args:
         df (pd.DataFrame): The DataFrame to be enriched.
 
     Returns:
-        pd.DataFrame: The unchanged DataFrame as no implementation is provided.
+        pd.DataFrame: The DataFrame with the 'std_legal_entity' column added, containing standardized legal entity descriptions.
     """
+    kind = load_config("kind")
+    df['std_legal_entity'] = df['kind'].map(kind)
     return df
```

### Comparing `cnparser-1.5.3/cnparser/load.py` & `cnparser-1.5.4/cnparser/load.py`

 * *Files identical despite different names*

### Comparing `cnparser-1.5.3/cnparser/utility.py` & `cnparser-1.5.4/cnparser/utility.py`

 * *Files identical despite different names*

### Comparing `cnparser-1.5.3/cnparser.egg-info/PKG-INFO` & `cnparser-1.5.4/cnparser.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,67 +1,75 @@
 Metadata-Version: 2.1
 Name: cnparser
-Version: 1.5.3
+Version: 1.5.4
 Summary: cnparser is a parser library of Corporate Number Publication Site data.
 Home-page: https://github.com/new-village/cnparser
 Author: new-village
 License: GPLv3+
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: requests
 Requires-Dist: bs4
 Requires-Dist: pandas
 Requires-Dist: pykakasi
-Requires-Dist: kanjize==1.5.0
-Requires-Dist: normalize-japanese-addresses==0.0.9
 
 # cnparser  
 [![Test](https://github.com/new-village/cnparser/actions/workflows/test.yaml/badge.svg)](https://github.com/new-village/cnparser/actions/workflows/test.yaml)  
 **cnparser** is a python library for loading and enrichment [Corporate Number Publication Site](https://www.houjin-bangou.nta.go.jp/en/) data that is provided from National Tax Agency Japan. cnparser only support to parse latest data now.   
   
 ## Installation  
 ----------------------
 cnparser is available on pip installation.
-```
+```shell:
 $ python -m pip install cnparser
 ```
   
 ### GitHub Install
 Installing the latest version from GitHub:  
-```
+```shell:
 $ git clone https://github.com/new-village/cnparser
 $ cd cnparser
 $ python setup.py install
 ```
     
 ## Usage
 This section demonstrates how to use this library to load and process data from the National Tax Agency's [Corporate Number Publication Site](https://www.houjin-bangou.nta.go.jp/).
 
 ### Direct Data Loading
 To download data for a specific prefecture, use the `load` function. By passing the prefecture name as an argument, you can obtain a DataFrame containing data for that prefecture.If you wish to download data for a specific prefecture, you must specify the prefecture name in Roman characters ([list of the supported prefectures](https://github.com/new-village/cnparser/blob/main/cnparser/config/file_id.json)).  
 To execute the `load` function without specifying any arguments, data for all prefectures across Japan will be downloaded. 
-```
+```python:
 >>> import cnparser
 >>> df = cnparser.load("Shimane")
 ```
 
 ### CSV Data Loading
 If you already have a downloaded CSV file, use the `read_csv` function. By passing the file path as an argument, you can obtain a DataFrame with headers from the CSV data.
-```
+```python:
 >>> import cnparser
 >>> df = cnparser.read_csv("path/to/data.csv")
 ```
 
 ### Data Enrichment Functionality
-The `enrich` function adds a standardized furigana column `std_furigana` to the DataFrame. It processes data entry by converting `name` to furigana.
-```
+The `enrich` function standardises and transforms the values of specific fields in the loaded DataFrame. 
+```python:
 >>> import cnparser
 >>> df = cnparser.enrich(df)
 ```
 
+The functions perform all processing, but it is possible to apply only specific processing by defining specific processing as an argument.
+```python:
+>>> import cnparser
+>>> df = cnparser.enrich(df, "enrich_kana" ...)
+```
+
+The processes supported by the `enrich` function are as follows:
+- `enrich_kana`: function adding a standardized furigana column `std_furigana` to the DataFrame. It processes data entry by converting `name` to kana, if `furigana` is NaN. Note that currently only kanji and katakana conversions are supported. Alphabet conversion is not supported.  
+- `enrich_kind`: function adding label of `kind` to `std_legal_entity`.  
+  
 ## Tools
 ### import_dict.py: Bilingual Emacspeak Project (BEP) Dictionary Import Tool
 This tool imports the [BEP dictionary](https://fastapi.metacpan.org/source/MASH/Lingua-JA-Yomi-0.01/lib/Lingua/JA) and generates a dictionary file for use with cnparser. It processes the bilingual mappings from English to Kana, ensuring that cnparser can accurately handle and transform data involving these language elements.
-```
+```shell:
 $ cd /home/<USER>/analysis
 $ python enrich.py <FILE_PATH>
 ```
```

### Comparing `cnparser-1.5.3/setup.py` & `cnparser-1.5.4/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -3,18 +3,18 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='cnparser',
-    version='1.5.3',
+    version='1.5.4',
     author='new-village',
     url='https://github.com/new-village/cnparser',
     description='cnparser is a parser library of Corporate Number Publication Site data.',
     long_description=long_description,
     long_description_content_type="text/markdown",
     license = 'GPLv3+',
-    install_requires=['requests', 'bs4', 'pandas', 'pykakasi', 'kanjize==1.5.0', 'normalize-japanese-addresses==0.0.9'],
+    install_requires=['requests', 'bs4', 'pandas', 'pykakasi'],
     packages=find_packages(),
     package_data={'': ['config/*.json']},
 )
```

### Comparing `cnparser-1.5.3/test/test_enrich.py` & `cnparser-1.5.4/test/test_enrich.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,31 +1,40 @@
 """ test_enrich.py
 """
-import unittest
 import pandas as pd
+import unittest
+from cnparser.enrich import enrich, enrich_kana, enrich_kind
 from cnparser.load import read_csv
-from cnparser.enrich import enrich, enrich_kana
 
 class TestEnrich(unittest.TestCase):
     def setUp(self):
         """Set up the test environment by loading test data from a CSV file."""
         self.df = read_csv('./test/data/31_tottori_test_20240329.csv')
 
     def test_enrich_kana(self):
         """Test the enrich_kana function to ensure it correctly adds the 'std_furigana' column."""
         result = enrich_kana(self.df.copy())
         self.assertIn('std_furigana', result.columns)
         expected_furigana = ['トットリカンイサイバンショ', 'シマダショウジ', 'souvenir', 'T&Mコンサルティング', 'HAPカンコウ']
         for i, furigana in enumerate(expected_furigana):
             self.assertEqual(result.iloc[i]['std_furigana'], furigana)
 
+    def test_enrich_kind(self):
+        """Test the enrich_kind function to ensure it correctly maps 'kind' to 'std_legal_entity'."""
+        result = enrich_kind(self.df.copy())
+        self.assertIn('std_legal_entity', result.columns)
+        expected_entities = ['National Agency', 'K.K.', 'K.K.', 'K.K.', 'Y.K.']
+        for i, entity in enumerate(expected_entities):
+            self.assertEqual(result.iloc[i]['std_legal_entity'], entity)
+
     def test_enrich_all_processes(self):
         """Test the enrich function with all processes to ensure it processes correctly."""
         result = enrich(self.df.copy())
         self.assertIn('std_furigana', result.columns)
+        self.assertIn('std_legal_entity', result.columns)
 
     def test_enrich_with_invalid_process(self):
         """Test the enrich function with an invalid process name to ensure it returns the original DataFrame unchanged and raises a warning."""
         with self.assertWarns(Warning) as warning:
             result = enrich(self.df.copy(), 'enrich_error')
             self.assertEqual(str(warning.warnings[0].message), "No valid processing functions specified in ('enrich_error',). Returning the original DataFrame unchanged.")
         pd.testing.assert_frame_equal(self.df, result)
```

### Comparing `cnparser-1.5.3/test/test_load.py` & `cnparser-1.5.4/test/test_load.py`

 * *Files identical despite different names*

