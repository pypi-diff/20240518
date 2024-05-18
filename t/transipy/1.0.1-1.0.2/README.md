# Comparing `tmp/transipy-1.0.1.tar.gz` & `tmp/transipy-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "transipy-1.0.1.tar", last modified: Sat May 18 07:04:01 2024, max compression
+gzip compressed data, was "transipy-1.0.2.tar", last modified: Sat May 18 07:17:20 2024, max compression
```

## Comparing `transipy-1.0.1.tar` & `transipy-1.0.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2024-05-18 07:04:01.648653 transipy-1.0.1/
--rw-r--r--   0 mac        (501) staff       (20)     1064 2024-05-17 16:46:36.000000 transipy-1.0.1/LICENSE
--rw-r--r--   0 mac        (501) staff       (20)     9630 2024-05-18 07:04:01.648502 transipy-1.0.1/PKG-INFO
--rw-r--r--   0 mac        (501) staff       (20)     9211 2024-05-18 06:40:16.000000 transipy-1.0.1/README.md
--rw-r--r--   0 mac        (501) staff       (20)       38 2024-05-18 07:04:01.648694 transipy-1.0.1/setup.cfg
--rw-r--r--   0 mac        (501) staff       (20)      957 2024-05-18 07:02:30.000000 transipy-1.0.1/setup.py
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2024-05-18 07:04:01.647642 transipy-1.0.1/transipy/
--rw-r--r--   0 mac        (501) staff       (20)       30 2024-05-18 07:03:48.000000 transipy-1.0.1/transipy/__init__.py
--rw-r--r--   0 mac        (501) staff       (20)     5422 2024-05-18 06:54:44.000000 transipy-1.0.1/transipy/main.py
--rw-r--r--   0 mac        (501) staff       (20)     5405 2024-05-18 06:40:16.000000 transipy-1.0.1/transipy/trans_helper.py
--rw-r--r--   0 mac        (501) staff       (20)     1327 2024-05-18 06:40:16.000000 transipy-1.0.1/transipy/utils.py
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2024-05-18 07:04:01.648332 transipy-1.0.1/transipy.egg-info/
--rw-r--r--   0 mac        (501) staff       (20)     9630 2024-05-18 07:04:01.000000 transipy-1.0.1/transipy.egg-info/PKG-INFO
--rw-r--r--   0 mac        (501) staff       (20)      301 2024-05-18 07:04:01.000000 transipy-1.0.1/transipy.egg-info/SOURCES.txt
--rw-r--r--   0 mac        (501) staff       (20)        1 2024-05-18 07:04:01.000000 transipy-1.0.1/transipy.egg-info/dependency_links.txt
--rw-r--r--   0 mac        (501) staff       (20)       43 2024-05-18 07:04:01.000000 transipy-1.0.1/transipy.egg-info/entry_points.txt
--rw-r--r--   0 mac        (501) staff       (20)      107 2024-05-18 07:04:01.000000 transipy-1.0.1/transipy.egg-info/requires.txt
--rw-r--r--   0 mac        (501) staff       (20)        9 2024-05-18 07:04:01.000000 transipy-1.0.1/transipy.egg-info/top_level.txt
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2024-05-18 07:17:20.322189 transipy-1.0.2/
+-rw-r--r--   0 mac        (501) staff       (20)     1064 2024-05-17 16:46:36.000000 transipy-1.0.2/LICENSE
+-rw-r--r--   0 mac        (501) staff       (20)     9465 2024-05-18 07:17:20.322037 transipy-1.0.2/PKG-INFO
+-rw-r--r--   0 mac        (501) staff       (20)     9046 2024-05-18 07:14:06.000000 transipy-1.0.2/README.md
+-rw-r--r--   0 mac        (501) staff       (20)       38 2024-05-18 07:17:20.322231 transipy-1.0.2/setup.cfg
+-rw-r--r--   0 mac        (501) staff       (20)      957 2024-05-18 07:15:23.000000 transipy-1.0.2/setup.py
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2024-05-18 07:17:20.321140 transipy-1.0.2/transipy/
+-rw-r--r--   0 mac        (501) staff       (20)       30 2024-05-18 07:03:48.000000 transipy-1.0.2/transipy/__init__.py
+-rw-r--r--   0 mac        (501) staff       (20)     5422 2024-05-18 07:04:57.000000 transipy-1.0.2/transipy/main.py
+-rw-r--r--   0 mac        (501) staff       (20)     5405 2024-05-18 06:40:16.000000 transipy-1.0.2/transipy/trans_helper.py
+-rw-r--r--   0 mac        (501) staff       (20)     1327 2024-05-18 06:40:16.000000 transipy-1.0.2/transipy/utils.py
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2024-05-18 07:17:20.321865 transipy-1.0.2/transipy.egg-info/
+-rw-r--r--   0 mac        (501) staff       (20)     9465 2024-05-18 07:17:20.000000 transipy-1.0.2/transipy.egg-info/PKG-INFO
+-rw-r--r--   0 mac        (501) staff       (20)      301 2024-05-18 07:17:20.000000 transipy-1.0.2/transipy.egg-info/SOURCES.txt
+-rw-r--r--   0 mac        (501) staff       (20)        1 2024-05-18 07:17:20.000000 transipy-1.0.2/transipy.egg-info/dependency_links.txt
+-rw-r--r--   0 mac        (501) staff       (20)       43 2024-05-18 07:17:20.000000 transipy-1.0.2/transipy.egg-info/entry_points.txt
+-rw-r--r--   0 mac        (501) staff       (20)      107 2024-05-18 07:17:20.000000 transipy-1.0.2/transipy.egg-info/requires.txt
+-rw-r--r--   0 mac        (501) staff       (20)        9 2024-05-18 07:17:20.000000 transipy-1.0.2/transipy.egg-info/top_level.txt
```

### Comparing `transipy-1.0.1/LICENSE` & `transipy-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `transipy-1.0.1/PKG-INFO` & `transipy-1.0.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: transipy
-Version: 1.0.1
+Version: 1.0.2
 Summary: Transipy is your one-stop solution for lightning-fast and accurate document translation.
 Home-page: https://github.com/NeiH4207/transipy
 Author: Hien Vu, 
 Author-email: hienvq23@gmail.com, 
 Keywords: google translate,translation,document translation,language translation
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
@@ -19,15 +19,15 @@
 
 
 
 <!-- PROJECT LOGO -->
 <br />
 <p align="center">
   <a href="https://github.com/NeiH4207/transipy">
-    <img src="images/transipy_logo.png" alt="Logo" width="80" height="80">
+    <img src="images/transipy_logo.png" alt="Logo" width="180" height="180">
   </a>
 
   <h3 align="center">Transipy: The Powerful and Fastest Document Translation Tool</h3>
 
   <p align="center">
     Transipy is your one-stop solution for lightning-fast and accurate document translation. With its parallel processing capabilities, Transipy effortlessly handles large volumes of data in various formats, including CSV, TXT, and XLSX.
     <br />
@@ -53,24 +53,21 @@
       <ul>
         <li><a href="#built-with">Built With</a></li>
       </ul>
     </li>
     <li>
       <a href="#getting-started">Getting Started</a>
       <ul>
-        <li><a href="#prerequisites">Prerequisites</a></li>
         <li><a href="#installation">Installation</a></li>
       </ul>
     </li>
     <li><a href="#usage">Usage</a></li>
-    <li><a href="#roadmap">Roadmap</a></li>
     <li><a href="#contributing">Contributing</a></li>
     <li><a href="#license">License</a></li>
     <li><a href="#contact">Contact</a></li>
-    <li><a href="#acknowledgements">Acknowledgements</a></li>
   </ol>
 </details>
 
 
 
 <!-- ABOUT THE PROJECT -->
 ## About The Project
@@ -87,15 +84,15 @@
 
 <!-- GETTING STARTED -->
 ## Getting Started
 
 This is an example of how you may give instructions on setting up your project locally.
 To get a local copy up and running follow these simple example steps.
 
-### Prerequisites
+### Installation
 
 Install the required packages using the following command:
 
 ```bash
 pip install transipy
 ```
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: transipy Version: 1.0.1 Summary: Transipy is your
+Metadata-Version: 2.1 Name: transipy Version: 1.0.2 Summary: Transipy is your
 one-stop solution for lightning-fast and accurate document translation. Home-
 page: https://github.com/NeiH4207/transipy Author: Hien Vu, Author-email:
 hienvq23@gmail.com, Keywords: google translate,translation,document
 translation,language translation Requires-Python: >=3.10 Description-Content-
 Type: text/markdown License-File: LICENSE [![MIT License][license-shield]]
 [license-url] [![LinkedIn][linkedin-shield]][linkedin-url]
                                     _[_L_o_g_o_]
@@ -14,36 +14,33 @@
                              _EE_xx_pp_ll_oo_rr_ee_ _tt_hh_ee_ _dd_oo_cc_ss_ _?Â_?»
 
                   _V_i_e_w_ _D_e_m_o Â· _R_e_p_o_r_t_ _B_u_g Â· _R_e_q_u_e_s_t_ _F_e_a_t_u_r_e
 Table of Contents
    1. _A_b_o_u_t_ _T_h_e_ _P_r_o_j_e_c_t
           o _B_u_i_l_t_ _W_i_t_h
    2. _G_e_t_t_i_n_g_ _S_t_a_r_t_e_d
-          o _P_r_e_r_e_q_u_i_s_i_t_e_s
           o _I_n_s_t_a_l_l_a_t_i_o_n
    3. _U_s_a_g_e
-   4. _R_o_a_d_m_a_p
-   5. _C_o_n_t_r_i_b_u_t_i_n_g
-   6. _L_i_c_e_n_s_e
-   7. _C_o_n_t_a_c_t
-   8. _A_c_k_n_o_w_l_e_d_g_e_m_e_n_t_s
+   4. _C_o_n_t_r_i_b_u_t_i_n_g
+   5. _L_i_c_e_n_s_e
+   6. _C_o_n_t_a_c_t
 ## About The Project Transipy is your one-stop solution for lightning-fast and
 accurate document translation. With its parallel processing capabilities,
 Transipy effortlessly handles large volumes of data in various formats,
 including CSV, TXT, and XLSX. Key Features: 1. Fastest Speed: Experience the
 fastest document translation available, thanks to Transipy's parallel
 processing techniques. 2. Versatile Format Support: Seamlessly translate your
 documents in CSV, TXT, and XLSX formats, eliminating the need for manual
 conversions. 3. High Accuracy: Trust Transipy's powerful translation engine to
 deliver precise results, ensuring your message is conveyed accurately across
 languages. Transform your document translation workflow with Transipy â the
 powerful, fast, and versatile solution you've been waiting for. ## Getting
 Started This is an example of how you may give instructions on setting up your
 project locally. To get a local copy up and running follow these simple example
-steps. ### Prerequisites Install the required packages using the following
+steps. ### Installation Install the required packages using the following
 command: ```bash pip install transipy ``` You can also install from the git
 repository: ```bash git clone git@github.com:NeiH4207/transipy.git cd transipy
 pip install -e . ``` ## Usage ```bash usage: transipy [-h] -f FILE_PATH [-
 l SEP] -s SOURCE -t TARGET [-c CHUNK_SIZE] [-o OUTPUT_FILE] [-d DICTIONARY] [--
 column COLUMN] [--skip SKIP] [--sheet SHEET] Translate text in a file
 (.csv/.txt) from source language to target language. options: -h, --help show
 this help message and exit -f FILE_PATH, --file-path FILE_PATH The source file
```

### Comparing `transipy-1.0.1/README.md` & `transipy-1.0.2/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 
 
 <!-- PROJECT LOGO -->
 <br />
 <p align="center">
   <a href="https://github.com/NeiH4207/transipy">
-    <img src="images/transipy_logo.png" alt="Logo" width="80" height="80">
+    <img src="images/transipy_logo.png" alt="Logo" width="180" height="180">
   </a>
 
   <h3 align="center">Transipy: The Powerful and Fastest Document Translation Tool</h3>
 
   <p align="center">
     Transipy is your one-stop solution for lightning-fast and accurate document translation. With its parallel processing capabilities, Transipy effortlessly handles large volumes of data in various formats, including CSV, TXT, and XLSX.
     <br />
@@ -41,24 +41,21 @@
       <ul>
         <li><a href="#built-with">Built With</a></li>
       </ul>
     </li>
     <li>
       <a href="#getting-started">Getting Started</a>
       <ul>
-        <li><a href="#prerequisites">Prerequisites</a></li>
         <li><a href="#installation">Installation</a></li>
       </ul>
     </li>
     <li><a href="#usage">Usage</a></li>
-    <li><a href="#roadmap">Roadmap</a></li>
     <li><a href="#contributing">Contributing</a></li>
     <li><a href="#license">License</a></li>
     <li><a href="#contact">Contact</a></li>
-    <li><a href="#acknowledgements">Acknowledgements</a></li>
   </ol>
 </details>
 
 
 
 <!-- ABOUT THE PROJECT -->
 ## About The Project
@@ -75,15 +72,15 @@
 
 <!-- GETTING STARTED -->
 ## Getting Started
 
 This is an example of how you may give instructions on setting up your project locally.
 To get a local copy up and running follow these simple example steps.
 
-### Prerequisites
+### Installation
 
 Install the required packages using the following command:
 
 ```bash
 pip install transipy
 ```
```

#### html2text {}

```diff
@@ -9,36 +9,33 @@
                              _EE_xx_pp_ll_oo_rr_ee_ _tt_hh_ee_ _dd_oo_cc_ss_ _?Â_?»
 
                   _V_i_e_w_ _D_e_m_o Â· _R_e_p_o_r_t_ _B_u_g Â· _R_e_q_u_e_s_t_ _F_e_a_t_u_r_e
 Table of Contents
    1. _A_b_o_u_t_ _T_h_e_ _P_r_o_j_e_c_t
           o _B_u_i_l_t_ _W_i_t_h
    2. _G_e_t_t_i_n_g_ _S_t_a_r_t_e_d
-          o _P_r_e_r_e_q_u_i_s_i_t_e_s
           o _I_n_s_t_a_l_l_a_t_i_o_n
    3. _U_s_a_g_e
-   4. _R_o_a_d_m_a_p
-   5. _C_o_n_t_r_i_b_u_t_i_n_g
-   6. _L_i_c_e_n_s_e
-   7. _C_o_n_t_a_c_t
-   8. _A_c_k_n_o_w_l_e_d_g_e_m_e_n_t_s
+   4. _C_o_n_t_r_i_b_u_t_i_n_g
+   5. _L_i_c_e_n_s_e
+   6. _C_o_n_t_a_c_t
 ## About The Project Transipy is your one-stop solution for lightning-fast and
 accurate document translation. With its parallel processing capabilities,
 Transipy effortlessly handles large volumes of data in various formats,
 including CSV, TXT, and XLSX. Key Features: 1. Fastest Speed: Experience the
 fastest document translation available, thanks to Transipy's parallel
 processing techniques. 2. Versatile Format Support: Seamlessly translate your
 documents in CSV, TXT, and XLSX formats, eliminating the need for manual
 conversions. 3. High Accuracy: Trust Transipy's powerful translation engine to
 deliver precise results, ensuring your message is conveyed accurately across
 languages. Transform your document translation workflow with Transipy â the
 powerful, fast, and versatile solution you've been waiting for. ## Getting
 Started This is an example of how you may give instructions on setting up your
 project locally. To get a local copy up and running follow these simple example
-steps. ### Prerequisites Install the required packages using the following
+steps. ### Installation Install the required packages using the following
 command: ```bash pip install transipy ``` You can also install from the git
 repository: ```bash git clone git@github.com:NeiH4207/transipy.git cd transipy
 pip install -e . ``` ## Usage ```bash usage: transipy [-h] -f FILE_PATH [-
 l SEP] -s SOURCE -t TARGET [-c CHUNK_SIZE] [-o OUTPUT_FILE] [-d DICTIONARY] [--
 column COLUMN] [--skip SKIP] [--sheet SHEET] Translate text in a file
 (.csv/.txt) from source language to target language. options: -h, --help show
 this help message and exit -f FILE_PATH, --file-path FILE_PATH The source file
```

### Comparing `transipy-1.0.1/setup.py` & `transipy-1.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 long_description = (here / "README.md").read_text(encoding="utf-8")
 
 def get_requirements(path: str):
     return [l.strip() for l in open(path)]
 
 setup(
     name='transipy',
-    version='1.0.1',
+    version='1.0.2',
     description='Transipy is your one-stop solution for lightning-fast and accurate document translation.',
     long_description=long_description,
     long_description_content_type="text/markdown",
     author=', '.join(['Hien Vu', '']),
     author_email=', '.join(['hienvq23@gmail.com', '']),
     url='https://github.com/NeiH4207/transipy',
     packages=find_packages(),
```

### Comparing `transipy-1.0.1/transipy/main.py` & `transipy-1.0.2/transipy/main.py`

 * *Files identical despite different names*

### Comparing `transipy-1.0.1/transipy/trans_helper.py` & `transipy-1.0.2/transipy/trans_helper.py`

 * *Files identical despite different names*

### Comparing `transipy-1.0.1/transipy/utils.py` & `transipy-1.0.2/transipy/utils.py`

 * *Files identical despite different names*

### Comparing `transipy-1.0.1/transipy.egg-info/PKG-INFO` & `transipy-1.0.2/transipy.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: transipy
-Version: 1.0.1
+Version: 1.0.2
 Summary: Transipy is your one-stop solution for lightning-fast and accurate document translation.
 Home-page: https://github.com/NeiH4207/transipy
 Author: Hien Vu, 
 Author-email: hienvq23@gmail.com, 
 Keywords: google translate,translation,document translation,language translation
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
@@ -19,15 +19,15 @@
 
 
 
 <!-- PROJECT LOGO -->
 <br />
 <p align="center">
   <a href="https://github.com/NeiH4207/transipy">
-    <img src="images/transipy_logo.png" alt="Logo" width="80" height="80">
+    <img src="images/transipy_logo.png" alt="Logo" width="180" height="180">
   </a>
 
   <h3 align="center">Transipy: The Powerful and Fastest Document Translation Tool</h3>
 
   <p align="center">
     Transipy is your one-stop solution for lightning-fast and accurate document translation. With its parallel processing capabilities, Transipy effortlessly handles large volumes of data in various formats, including CSV, TXT, and XLSX.
     <br />
@@ -53,24 +53,21 @@
       <ul>
         <li><a href="#built-with">Built With</a></li>
       </ul>
     </li>
     <li>
       <a href="#getting-started">Getting Started</a>
       <ul>
-        <li><a href="#prerequisites">Prerequisites</a></li>
         <li><a href="#installation">Installation</a></li>
       </ul>
     </li>
     <li><a href="#usage">Usage</a></li>
-    <li><a href="#roadmap">Roadmap</a></li>
     <li><a href="#contributing">Contributing</a></li>
     <li><a href="#license">License</a></li>
     <li><a href="#contact">Contact</a></li>
-    <li><a href="#acknowledgements">Acknowledgements</a></li>
   </ol>
 </details>
 
 
 
 <!-- ABOUT THE PROJECT -->
 ## About The Project
@@ -87,15 +84,15 @@
 
 <!-- GETTING STARTED -->
 ## Getting Started
 
 This is an example of how you may give instructions on setting up your project locally.
 To get a local copy up and running follow these simple example steps.
 
-### Prerequisites
+### Installation
 
 Install the required packages using the following command:
 
 ```bash
 pip install transipy
 ```
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: transipy Version: 1.0.1 Summary: Transipy is your
+Metadata-Version: 2.1 Name: transipy Version: 1.0.2 Summary: Transipy is your
 one-stop solution for lightning-fast and accurate document translation. Home-
 page: https://github.com/NeiH4207/transipy Author: Hien Vu, Author-email:
 hienvq23@gmail.com, Keywords: google translate,translation,document
 translation,language translation Requires-Python: >=3.10 Description-Content-
 Type: text/markdown License-File: LICENSE [![MIT License][license-shield]]
 [license-url] [![LinkedIn][linkedin-shield]][linkedin-url]
                                     _[_L_o_g_o_]
@@ -14,36 +14,33 @@
                              _EE_xx_pp_ll_oo_rr_ee_ _tt_hh_ee_ _dd_oo_cc_ss_ _?Â_?»
 
                   _V_i_e_w_ _D_e_m_o Â· _R_e_p_o_r_t_ _B_u_g Â· _R_e_q_u_e_s_t_ _F_e_a_t_u_r_e
 Table of Contents
    1. _A_b_o_u_t_ _T_h_e_ _P_r_o_j_e_c_t
           o _B_u_i_l_t_ _W_i_t_h
    2. _G_e_t_t_i_n_g_ _S_t_a_r_t_e_d
-          o _P_r_e_r_e_q_u_i_s_i_t_e_s
           o _I_n_s_t_a_l_l_a_t_i_o_n
    3. _U_s_a_g_e
-   4. _R_o_a_d_m_a_p
-   5. _C_o_n_t_r_i_b_u_t_i_n_g
-   6. _L_i_c_e_n_s_e
-   7. _C_o_n_t_a_c_t
-   8. _A_c_k_n_o_w_l_e_d_g_e_m_e_n_t_s
+   4. _C_o_n_t_r_i_b_u_t_i_n_g
+   5. _L_i_c_e_n_s_e
+   6. _C_o_n_t_a_c_t
 ## About The Project Transipy is your one-stop solution for lightning-fast and
 accurate document translation. With its parallel processing capabilities,
 Transipy effortlessly handles large volumes of data in various formats,
 including CSV, TXT, and XLSX. Key Features: 1. Fastest Speed: Experience the
 fastest document translation available, thanks to Transipy's parallel
 processing techniques. 2. Versatile Format Support: Seamlessly translate your
 documents in CSV, TXT, and XLSX formats, eliminating the need for manual
 conversions. 3. High Accuracy: Trust Transipy's powerful translation engine to
 deliver precise results, ensuring your message is conveyed accurately across
 languages. Transform your document translation workflow with Transipy â the
 powerful, fast, and versatile solution you've been waiting for. ## Getting
 Started This is an example of how you may give instructions on setting up your
 project locally. To get a local copy up and running follow these simple example
-steps. ### Prerequisites Install the required packages using the following
+steps. ### Installation Install the required packages using the following
 command: ```bash pip install transipy ``` You can also install from the git
 repository: ```bash git clone git@github.com:NeiH4207/transipy.git cd transipy
 pip install -e . ``` ## Usage ```bash usage: transipy [-h] -f FILE_PATH [-
 l SEP] -s SOURCE -t TARGET [-c CHUNK_SIZE] [-o OUTPUT_FILE] [-d DICTIONARY] [--
 column COLUMN] [--skip SKIP] [--sheet SHEET] Translate text in a file
 (.csv/.txt) from source language to target language. options: -h, --help show
 this help message and exit -f FILE_PATH, --file-path FILE_PATH The source file
```

