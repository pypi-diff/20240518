# Comparing `tmp/livescore-api-0.0.4.tar.gz` & `tmp/livescore-api-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "livescore-api-0.0.4.tar", last modified: Fri Jun 23 12:52:30 2023, max compression
+gzip compressed data, was "livescore-api-0.0.5.tar", last modified: Sat May 18 12:14:20 2024, max compression
```

## Comparing `livescore-api-0.0.4.tar` & `livescore-api-0.0.5.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwx---   0 root         (0) everybody  (9997)        0 2023-06-23 12:52:30.126000 livescore-api-0.0.4/
--rw-rw----   0 root         (0) everybody  (9997)     1064 2023-06-13 16:33:10.000000 livescore-api-0.0.4/LICENSE
--rw-rw----   0 root         (0) everybody  (9997)     8566 2023-06-23 12:52:30.054000 livescore-api-0.0.4/PKG-INFO
--rw-rw----   0 root         (0) everybody  (9997)     7460 2023-06-23 12:51:08.000000 livescore-api-0.0.4/README.md
-drwxrwx---   0 root         (0) everybody  (9997)        0 2023-06-23 12:52:29.846000 livescore-api-0.0.4/livescore_api/
--rw-rw----   0 root         (0) everybody  (9997)      323 2023-06-23 12:50:14.000000 livescore-api-0.0.4/livescore_api/__init__.py
--rw-rw----   0 root         (0) everybody  (9997)       34 2023-06-12 02:52:21.000000 livescore-api-0.0.4/livescore_api/__main__.py
--rw-rw----   0 root         (0) everybody  (9997)     8243 2023-06-13 21:47:47.000000 livescore-api-0.0.4/livescore_api/console.py
--rw-rw----   0 root         (0) everybody  (9997)    12716 2023-06-13 22:03:30.000000 livescore-api-0.0.4/livescore_api/main.py
--rw-rw----   0 root         (0) everybody  (9997)     5186 2023-06-13 22:03:29.000000 livescore-api-0.0.4/livescore_api/predictor.py
-drwxrwx---   0 root         (0) everybody  (9997)        0 2023-06-23 12:52:30.034000 livescore-api-0.0.4/livescore_api.egg-info/
--rw-rw----   0 root         (0) everybody  (9997)     8566 2023-06-23 12:52:28.000000 livescore-api-0.0.4/livescore_api.egg-info/PKG-INFO
--rw-rw----   0 root         (0) everybody  (9997)      376 2023-06-23 12:52:29.000000 livescore-api-0.0.4/livescore_api.egg-info/SOURCES.txt
--rw-rw----   0 root         (0) everybody  (9997)        1 2023-06-23 12:52:28.000000 livescore-api-0.0.4/livescore_api.egg-info/dependency_links.txt
--rw-rw----   0 root         (0) everybody  (9997)       61 2023-06-23 12:52:28.000000 livescore-api-0.0.4/livescore_api.egg-info/entry_points.txt
--rw-rw----   0 root         (0) everybody  (9997)      109 2023-06-23 12:52:28.000000 livescore-api-0.0.4/livescore_api.egg-info/requires.txt
--rw-rw----   0 root         (0) everybody  (9997)       14 2023-06-23 12:52:28.000000 livescore-api-0.0.4/livescore_api.egg-info/top_level.txt
--rw-rw----   0 root         (0) everybody  (9997)       38 2023-06-23 12:52:30.126000 livescore-api-0.0.4/setup.cfg
--rw-rw----   0 root         (0) everybody  (9997)     1646 2023-06-23 12:51:32.000000 livescore-api-0.0.4/setup.py
+drwxr-xr-x   0 smartwa   (1000) smartwa   (1001)        0 2024-05-18 12:14:20.486602 livescore-api-0.0.5/
+-rw-r--r--   0 smartwa   (1000) smartwa   (1001)     1064 2024-05-18 12:01:13.000000 livescore-api-0.0.5/LICENSE
+-rw-r--r--   0 smartwa   (1000) smartwa   (1001)     8815 2024-05-18 12:14:20.486602 livescore-api-0.0.5/PKG-INFO
+-rw-r--r--   0 smartwa   (1000) smartwa   (1001)     7495 2024-05-18 12:01:13.000000 livescore-api-0.0.5/README.md
+drwxr-xr-x   0 smartwa   (1000) smartwa   (1001)        0 2024-05-18 12:14:20.483269 livescore-api-0.0.5/livescore_api/
+-rw-r--r--   0 smartwa   (1000) smartwa   (1001)      323 2024-05-18 12:10:03.000000 livescore-api-0.0.5/livescore_api/__init__.py
+-rw-r--r--   0 smartwa   (1000) smartwa   (1001)       34 2024-05-18 12:01:13.000000 livescore-api-0.0.5/livescore_api/__main__.py
+-rw-r--r--   0 smartwa   (1000) smartwa   (1001)     8243 2024-05-18 12:01:13.000000 livescore-api-0.0.5/livescore_api/console.py
+-rw-r--r--   0 smartwa   (1000) smartwa   (1001)    12715 2024-05-18 12:10:38.000000 livescore-api-0.0.5/livescore_api/main.py
+-rw-r--r--   0 smartwa   (1000) smartwa   (1001)     5186 2024-05-18 12:01:13.000000 livescore-api-0.0.5/livescore_api/predictor.py
+drwxr-xr-x   0 smartwa   (1000) smartwa   (1001)        0 2024-05-18 12:14:20.486602 livescore-api-0.0.5/livescore_api.egg-info/
+-rw-r--r--   0 smartwa   (1000) smartwa   (1001)     8815 2024-05-18 12:14:20.000000 livescore-api-0.0.5/livescore_api.egg-info/PKG-INFO
+-rw-r--r--   0 smartwa   (1000) smartwa   (1001)      376 2024-05-18 12:14:20.000000 livescore-api-0.0.5/livescore_api.egg-info/SOURCES.txt
+-rw-r--r--   0 smartwa   (1000) smartwa   (1001)        1 2024-05-18 12:14:20.000000 livescore-api-0.0.5/livescore_api.egg-info/dependency_links.txt
+-rw-r--r--   0 smartwa   (1000) smartwa   (1001)       61 2024-05-18 12:14:20.000000 livescore-api-0.0.5/livescore_api.egg-info/entry_points.txt
+-rw-r--r--   0 smartwa   (1000) smartwa   (1001)      109 2024-05-18 12:14:20.000000 livescore-api-0.0.5/livescore_api.egg-info/requires.txt
+-rw-r--r--   0 smartwa   (1000) smartwa   (1001)       14 2024-05-18 12:14:20.000000 livescore-api-0.0.5/livescore_api.egg-info/top_level.txt
+-rw-r--r--   0 smartwa   (1000) smartwa   (1001)       38 2024-05-18 12:14:20.486602 livescore-api-0.0.5/setup.cfg
+-rw-r--r--   0 smartwa   (1000) smartwa   (1001)     1646 2024-05-18 12:10:51.000000 livescore-api-0.0.5/setup.py
```

### Comparing `livescore-api-0.0.4/LICENSE` & `livescore-api-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `livescore-api-0.0.4/PKG-INFO` & `livescore-api-0.0.5/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: livescore-api
-Version: 0.0.4
+Version: 0.0.5
 Summary: Access and manipulate matches from Livescore.com
 Home-page: https://github.com/Simatwa/livescore-api
 Author: Smartwa
 Author-email: smartwacaleb@gmail.com
 Maintainer: Smartwa
 License: MIT
 Project-URL: Bug Report, https://github.com/Simatwa/livescore-api/issues/new
@@ -21,18 +21,25 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: argparse>=1.1
+Requires-Dist: requests>=2.0.2
+Requires-Dist: pandas>=1.3.3
+Requires-Dist: tabulate==0.9.0
+Requires-Dist: smartbetsAPI==1.3.1
+Requires-Dist: tqdm==4.65.0
+Requires-Dist: colorama==0.4.6
 
 # Livescore-api
 <p align="center">
-<a href="https://github.com/Simatwa/livescore-api"><img alt="Github" src="https://img.shields.io/static/v1?logo=github&color=blueviolet&label=Test&message=Passing"/></a>
+<a href="https://github.com/Simatwa/livescore-api/actions/workflows/python-test.yml"><img src="https://github.com/Simatwa/livescore-api/actions/workflows/python-test.yml/badge.svg" alt="Python Test"/></a>
 <a href="LICENSE"><img alt="License" src="https://img.shields.io/static/v1?logo=GPL&color=Blue&message=MIT&label=License"/></a>
 <a href="https://pypi.org/project/livescore-api"><img alt="PyPi" src="https://img.shields.io/static/v1?logo=pypi&label=Pypi&message=v0.0.4&color=green"/></a>
 <a href="https://github.com/psf/black"><img alt="Black" src="https://img.shields.io/static/v1?logo=Black&label=Code-style&message=Black"/></a>
 <a href="#"><img alt="Passing" src="https://img.shields.io/static/v1?logo=Docs&label=Docs&message=Passing&color=green"/></a>
 <a href="#"><img alt="coverage" src="https://img.shields.io/static/v1?logo=Coverage&label=Coverage&message=60%&color=yellowgreen"/></a>
 <a href="#" alt="progress"><img alt="Progress" src="https://img.shields.io/static/v1?logo=Progress&label=Progress&message=95%&color=green"/></a>
 <a href="https://pepy.tech/project/livescore-api"><img src="https://static.pepy.tech/personalized-badge/livescore-api?period=total&units=international_system&left_color=grey&right_color=orange&left_text=Downloads" alt="Downloads"></a>
```

#### html2text {}

```diff
@@ -1,23 +1,26 @@
-Metadata-Version: 2.1 Name: livescore-api Version: 0.0.4 Summary: Access and
+Metadata-Version: 2.1 Name: livescore-api Version: 0.0.5 Summary: Access and
 manipulate matches from Livescore.com Home-page: https://github.com/Simatwa/
 livescore-api Author: Smartwa Author-email: smartwacaleb@gmail.com Maintainer:
 Smartwa License: MIT Project-URL: Bug Report, https://github.com/Simatwa/
 livescore-api/issues/new Keywords: livescore,football,livescore-api,api
 Classifier: License :: OSI Approved :: MIT License Classifier: Development
 Status :: 4 - Beta Classifier: Intended Audience :: Developers Classifier:
 Natural Language :: English Classifier: License :: Free For Home Use
 Classifier: Intended Audience :: Customer Service Classifier: Programming
 Language :: Python Classifier: Topic :: Software Development :: Libraries ::
 Python Modules Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11 Requires-Python: >=3.8
-Description-Content-Type: text/markdown License-File: LICENSE # Livescore-api
-    _[_G_i_t_h_u_b_]_[_L_i_c_e_n_s_e_]_[_P_y_P_i_]_[_B_l_a_c_k_]_[_P_a_s_s_i_n_g_]_[_c_o_v_e_r_a_g_e_]_[_P_r_o_g_r_e_s_s_]_[_D_o_w_n_l_o_a_d_s_]
+Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
+argparse>=1.1 Requires-Dist: requests>=2.0.2 Requires-Dist: pandas>=1.3.3
+Requires-Dist: tabulate==0.9.0 Requires-Dist: smartbetsAPI==1.3.1 Requires-
+Dist: tqdm==4.65.0 Requires-Dist: colorama==0.4.6 # Livescore-api
+  _[_P_y_t_h_o_n_ _T_e_s_t_]_[_L_i_c_e_n_s_e_]_[_P_y_P_i_]_[_B_l_a_c_k_]_[_P_a_s_s_i_n_g_]_[_c_o_v_e_r_a_g_e_]_[_P_r_o_g_r_e_s_s_]_[_D_o_w_n_l_o_a_d_s_]
 **Access and manipulate football data from [Livescore](https://
 livescore.com).** ## Installation 1. From pip ```sh pip install livescore-api
 ``` 2. From source - Clone repo and install ```sh git clone https://github.com/
 Simatwa/livescore-api.git cd livescore-api pip install . ``` ## Usage - `$
 livescore-api` ### Developer docs 1. Retrieving data offline ```py from
 livescore_api import json_formatter raw_matches = open("matches.json").read()
 sorted_matches = json_formatter(raw_matches) print(sorted_matches(max=1)) """
```

### Comparing `livescore-api-0.0.4/README.md` & `livescore-api-0.0.5/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # Livescore-api
 <p align="center">
-<a href="https://github.com/Simatwa/livescore-api"><img alt="Github" src="https://img.shields.io/static/v1?logo=github&color=blueviolet&label=Test&message=Passing"/></a>
+<a href="https://github.com/Simatwa/livescore-api/actions/workflows/python-test.yml"><img src="https://github.com/Simatwa/livescore-api/actions/workflows/python-test.yml/badge.svg" alt="Python Test"/></a>
 <a href="LICENSE"><img alt="License" src="https://img.shields.io/static/v1?logo=GPL&color=Blue&message=MIT&label=License"/></a>
 <a href="https://pypi.org/project/livescore-api"><img alt="PyPi" src="https://img.shields.io/static/v1?logo=pypi&label=Pypi&message=v0.0.4&color=green"/></a>
 <a href="https://github.com/psf/black"><img alt="Black" src="https://img.shields.io/static/v1?logo=Black&label=Code-style&message=Black"/></a>
 <a href="#"><img alt="Passing" src="https://img.shields.io/static/v1?logo=Docs&label=Docs&message=Passing&color=green"/></a>
 <a href="#"><img alt="coverage" src="https://img.shields.io/static/v1?logo=Coverage&label=Coverage&message=60%&color=yellowgreen"/></a>
 <a href="#" alt="progress"><img alt="Progress" src="https://img.shields.io/static/v1?logo=Progress&label=Progress&message=95%&color=green"/></a>
 <a href="https://pepy.tech/project/livescore-api"><img src="https://static.pepy.tech/personalized-badge/livescore-api?period=total&units=international_system&left_color=grey&right_color=orange&left_text=Downloads" alt="Downloads"></a>
```

#### html2text {}

```diff
@@ -1,9 +1,9 @@
 # Livescore-api
-    _[_G_i_t_h_u_b_]_[_L_i_c_e_n_s_e_]_[_P_y_P_i_]_[_B_l_a_c_k_]_[_P_a_s_s_i_n_g_]_[_c_o_v_e_r_a_g_e_]_[_P_r_o_g_r_e_s_s_]_[_D_o_w_n_l_o_a_d_s_]
+  _[_P_y_t_h_o_n_ _T_e_s_t_]_[_L_i_c_e_n_s_e_]_[_P_y_P_i_]_[_B_l_a_c_k_]_[_P_a_s_s_i_n_g_]_[_c_o_v_e_r_a_g_e_]_[_P_r_o_g_r_e_s_s_]_[_D_o_w_n_l_o_a_d_s_]
 **Access and manipulate football data from [Livescore](https://
 livescore.com).** ## Installation 1. From pip ```sh pip install livescore-api
 ``` 2. From source - Clone repo and install ```sh git clone https://github.com/
 Simatwa/livescore-api.git cd livescore-api pip install . ``` ## Usage - `$
 livescore-api` ### Developer docs 1. Retrieving data offline ```py from
 livescore_api import json_formatter raw_matches = open("matches.json").read()
 sorted_matches = json_formatter(raw_matches) print(sorted_matches(max=1)) """
```

### Comparing `livescore-api-0.0.4/livescore_api/console.py` & `livescore-api-0.0.5/livescore_api/console.py`

 * *Files identical despite different names*

### Comparing `livescore-api-0.0.4/livescore_api/main.py` & `livescore-api-0.0.5/livescore_api/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -116,15 +116,14 @@
         resp = cls.format(df)
         if cls.chosen_format in ("xlsx", "json"):
             resp = cls.reformat_json(json.loads(resp))
         return resp
 
     @classmethod
     def format(cls, df):
-
         r"""Manipulates data to required format
         :param df: `pd.DataFrame` object
         :type df: object `pd.DataFrame`
         :rtype: Instance of `pd.DataFrame`
         """
         if cls.chosen_format == "xlsx":
             df.to_excel(cls.chosen_output + ".xlsx")
```

### Comparing `livescore-api-0.0.4/livescore_api/predictor.py` & `livescore-api-0.0.5/livescore_api/predictor.py`

 * *Files identical despite different names*

### Comparing `livescore-api-0.0.4/livescore_api.egg-info/PKG-INFO` & `livescore-api-0.0.5/livescore_api.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: livescore-api
-Version: 0.0.4
+Version: 0.0.5
 Summary: Access and manipulate matches from Livescore.com
 Home-page: https://github.com/Simatwa/livescore-api
 Author: Smartwa
 Author-email: smartwacaleb@gmail.com
 Maintainer: Smartwa
 License: MIT
 Project-URL: Bug Report, https://github.com/Simatwa/livescore-api/issues/new
@@ -21,18 +21,25 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: argparse>=1.1
+Requires-Dist: requests>=2.0.2
+Requires-Dist: pandas>=1.3.3
+Requires-Dist: tabulate==0.9.0
+Requires-Dist: smartbetsAPI==1.3.1
+Requires-Dist: tqdm==4.65.0
+Requires-Dist: colorama==0.4.6
 
 # Livescore-api
 <p align="center">
-<a href="https://github.com/Simatwa/livescore-api"><img alt="Github" src="https://img.shields.io/static/v1?logo=github&color=blueviolet&label=Test&message=Passing"/></a>
+<a href="https://github.com/Simatwa/livescore-api/actions/workflows/python-test.yml"><img src="https://github.com/Simatwa/livescore-api/actions/workflows/python-test.yml/badge.svg" alt="Python Test"/></a>
 <a href="LICENSE"><img alt="License" src="https://img.shields.io/static/v1?logo=GPL&color=Blue&message=MIT&label=License"/></a>
 <a href="https://pypi.org/project/livescore-api"><img alt="PyPi" src="https://img.shields.io/static/v1?logo=pypi&label=Pypi&message=v0.0.4&color=green"/></a>
 <a href="https://github.com/psf/black"><img alt="Black" src="https://img.shields.io/static/v1?logo=Black&label=Code-style&message=Black"/></a>
 <a href="#"><img alt="Passing" src="https://img.shields.io/static/v1?logo=Docs&label=Docs&message=Passing&color=green"/></a>
 <a href="#"><img alt="coverage" src="https://img.shields.io/static/v1?logo=Coverage&label=Coverage&message=60%&color=yellowgreen"/></a>
 <a href="#" alt="progress"><img alt="Progress" src="https://img.shields.io/static/v1?logo=Progress&label=Progress&message=95%&color=green"/></a>
 <a href="https://pepy.tech/project/livescore-api"><img src="https://static.pepy.tech/personalized-badge/livescore-api?period=total&units=international_system&left_color=grey&right_color=orange&left_text=Downloads" alt="Downloads"></a>
```

#### html2text {}

```diff
@@ -1,23 +1,26 @@
-Metadata-Version: 2.1 Name: livescore-api Version: 0.0.4 Summary: Access and
+Metadata-Version: 2.1 Name: livescore-api Version: 0.0.5 Summary: Access and
 manipulate matches from Livescore.com Home-page: https://github.com/Simatwa/
 livescore-api Author: Smartwa Author-email: smartwacaleb@gmail.com Maintainer:
 Smartwa License: MIT Project-URL: Bug Report, https://github.com/Simatwa/
 livescore-api/issues/new Keywords: livescore,football,livescore-api,api
 Classifier: License :: OSI Approved :: MIT License Classifier: Development
 Status :: 4 - Beta Classifier: Intended Audience :: Developers Classifier:
 Natural Language :: English Classifier: License :: Free For Home Use
 Classifier: Intended Audience :: Customer Service Classifier: Programming
 Language :: Python Classifier: Topic :: Software Development :: Libraries ::
 Python Modules Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11 Requires-Python: >=3.8
-Description-Content-Type: text/markdown License-File: LICENSE # Livescore-api
-    _[_G_i_t_h_u_b_]_[_L_i_c_e_n_s_e_]_[_P_y_P_i_]_[_B_l_a_c_k_]_[_P_a_s_s_i_n_g_]_[_c_o_v_e_r_a_g_e_]_[_P_r_o_g_r_e_s_s_]_[_D_o_w_n_l_o_a_d_s_]
+Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
+argparse>=1.1 Requires-Dist: requests>=2.0.2 Requires-Dist: pandas>=1.3.3
+Requires-Dist: tabulate==0.9.0 Requires-Dist: smartbetsAPI==1.3.1 Requires-
+Dist: tqdm==4.65.0 Requires-Dist: colorama==0.4.6 # Livescore-api
+  _[_P_y_t_h_o_n_ _T_e_s_t_]_[_L_i_c_e_n_s_e_]_[_P_y_P_i_]_[_B_l_a_c_k_]_[_P_a_s_s_i_n_g_]_[_c_o_v_e_r_a_g_e_]_[_P_r_o_g_r_e_s_s_]_[_D_o_w_n_l_o_a_d_s_]
 **Access and manipulate football data from [Livescore](https://
 livescore.com).** ## Installation 1. From pip ```sh pip install livescore-api
 ``` 2. From source - Clone repo and install ```sh git clone https://github.com/
 Simatwa/livescore-api.git cd livescore-api pip install . ``` ## Usage - `$
 livescore-api` ### Developer docs 1. Retrieving data offline ```py from
 livescore_api import json_formatter raw_matches = open("matches.json").read()
 sorted_matches = json_formatter(raw_matches) print(sorted_matches(max=1)) """
```

### Comparing `livescore-api-0.0.4/setup.py` & `livescore-api-0.0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup
 
-version = "0.0.4"
+version = "0.0.5"
 repo = "https://github.com/Simatwa/livescore-api"
 info = "Access and manipulate matches from Livescore.com"
 author = "Smartwa"
 
 setup(
     name="livescore-api",
     packages=["livescore_api"],
@@ -17,15 +17,15 @@
     url=repo,
     project_urls={"Bug Report": f"{repo}/issues/new"},
     install_requires=[
         "argparse>=1.1",
         "requests>=2.0.2",
         "pandas>=1.3.3",
         "tabulate==0.9.0",
-        "smartbetsAPI==1.1.4",
+        "smartbetsAPI==1.3.1",
         "tqdm==4.65.0",
         "colorama==0.4.6",
     ],
     python_requires=">=3.8",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     classifiers=[
```

