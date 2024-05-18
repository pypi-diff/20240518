# Comparing `tmp/sequence_align-0.1.1-cp37-abi3-win_amd64.whl.zip` & `tmp/sequence_align-0.1.2-cp37-abi3-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,11 @@
-Zip file size: 110645 bytes, number of entries: 10
--rw-r--r--  4.6 unx     7495 b- defN 24-May-02 14:46 sequence_align-0.1.1.dist-info/METADATA
--rw-r--r--  4.6 unx       94 b- defN 24-May-02 14:46 sequence_align-0.1.1.dist-info/WHEEL
--rw-r--r--  4.6 unx    11566 b- defN 24-May-02 14:46 sequence_align-0.1.1.dist-info/license_files/LICENSE
--rw-r--r--  4.6 unx    11566 b- defN 24-May-02 14:46 sequence_align-0.1.1.dist-info/license_files/LICENSE
--rw-r--r--  4.6 unx       59 b- defN 24-May-02 14:46 sequence_align-0.1.1.dist-info/license_files/AUTHORS.md
--rw-r--r--  4.6 unx     6792 b- defN 24-May-02 14:46 sequence_align/pairwise.py
--rw-r--r--  4.6 unx        0 b- defN 24-May-02 14:46 sequence_align/py.typed
--rw-r--r--  4.6 unx        0 b- defN 24-May-02 14:46 sequence_align/__init__.py
--rwxr-xr-x  4.6 unx   195072 b- defN 24-May-02 14:46 sequence_align/sequence_align.pyd
--rw-r--r--  4.6 unx      889 b- defN 24-May-02 14:46 sequence_align-0.1.1.dist-info/RECORD
-10 files, 233533 bytes uncompressed, 109105 bytes compressed:  53.3%
+Zip file size: 107608 bytes, number of entries: 9
+-rw-r--r--  4.6 unx     7493 b- defN 24-May-18 15:57 sequence_align-0.1.2.dist-info/METADATA
+-rw-r--r--  4.6 unx       94 b- defN 24-May-18 15:57 sequence_align-0.1.2.dist-info/WHEEL
+-rw-r--r--  4.6 unx    11566 b- defN 24-May-18 15:57 sequence_align-0.1.2.dist-info/license_files/LICENSE
+-rw-r--r--  4.6 unx       59 b- defN 24-May-18 15:57 sequence_align-0.1.2.dist-info/license_files/AUTHORS.md
+-rw-r--r--  4.6 unx     6792 b- defN 24-May-18 15:57 sequence_align/pairwise.py
+-rw-r--r--  4.6 unx        0 b- defN 24-May-18 15:57 sequence_align/py.typed
+-rw-r--r--  4.6 unx        0 b- defN 24-May-18 15:57 sequence_align/__init__.py
+-rwxr-xr-x  4.6 unx   199680 b- defN 24-May-18 15:57 sequence_align/_sequence_align.pyd
+-rw-r--r--  4.6 unx      780 b- defN 24-May-18 15:57 sequence_align-0.1.2.dist-info/RECORD
+9 files, 226464 bytes uncompressed, 106246 bytes compressed:  53.1%
```

## zipnote {}

```diff
@@ -1,31 +1,28 @@
-Filename: sequence_align-0.1.1.dist-info/METADATA
+Filename: sequence_align-0.1.2.dist-info/METADATA
 Comment: 
 
-Filename: sequence_align-0.1.1.dist-info/WHEEL
+Filename: sequence_align-0.1.2.dist-info/WHEEL
 Comment: 
 
-Filename: sequence_align-0.1.1.dist-info/license_files/LICENSE
+Filename: sequence_align-0.1.2.dist-info/license_files/LICENSE
 Comment: 
 
-Filename: sequence_align-0.1.1.dist-info/license_files/LICENSE
-Comment: 
-
-Filename: sequence_align-0.1.1.dist-info/license_files/AUTHORS.md
+Filename: sequence_align-0.1.2.dist-info/license_files/AUTHORS.md
 Comment: 
 
 Filename: sequence_align/pairwise.py
 Comment: 
 
 Filename: sequence_align/py.typed
 Comment: 
 
 Filename: sequence_align/__init__.py
 Comment: 
 
-Filename: sequence_align/sequence_align.pyd
+Filename: sequence_align/_sequence_align.pyd
 Comment: 
 
-Filename: sequence_align-0.1.1.dist-info/RECORD
+Filename: sequence_align-0.1.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `sequence_align-0.1.1.dist-info/METADATA` & `sequence_align-0.1.2.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: sequence_align
-Version: 0.1.1
+Version: 0.1.2
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Rust
@@ -22,19 +22,19 @@
 Requires-Dist: pytest ; extra == 'dev'
 Requires-Dist: pytest-cov ; extra == 'dev'
 Requires-Dist: pyyaml ; extra == 'dev'
 Requires-Dist: types-psutil ; extra == 'dev'
 Requires-Dist: types-pyyaml ; extra == 'dev'
 Provides-Extra: dev
 License-File: LICENSE
-License-File: LICENSE
 License-File: AUTHORS.md
 Summary: Efficient implementations of Needleman-Wunsch and other sequence alignment algorithms in Rust with Python bindings.
 Author-email: "Kensho Technologies LLC." <sequence-align-maintainer@kensho.com>
 Maintainer-email: "Kensho Technologies LLC." <sequence-align-maintainer@kensho.com>
+License: Apache-2.0
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
 Project-URL: source, https://github.com/kensho-technologies/sequence_align
 Project-URL: Homepage, https://github.com/kensho-technologies/sequence_align
 Project-URL: Bug Tracker, https://github.com/kensho-technologies/sequence_align/issues
 
   <a href="https://github.com/kensho-technologies/sequence_align/actions?query=workflow%3A%22Tests+and+lint%22"><img src="https://github.com/kensho-technologies/sequence_align/workflows/Tests%20and%20lint/badge.svg" /></a>
```

### html2text {}

```diff
@@ -1,34 +1,34 @@
-Metadata-Version: 2.3 Name: sequence_align Version: 0.1.1 Classifier: Operating
+Metadata-Version: 2.3 Name: sequence_align Version: 0.1.2 Classifier: Operating
 System :: OS Independent Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11 Classifier: Programming
 Language :: Rust Classifier: Topic :: Scientific/Engineering :: Artificial
 Intelligence Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: Typing :: Typed Requires-Dist: bandit ; extra == 'dev' Requires-
 Dist: black ; extra == 'dev' Requires-Dist: flake8 ; extra == 'dev' Requires-
 Dist: isort >=5.0.0, <6 ; extra == 'dev' Requires-Dist: mypy ; extra == 'dev'
 Requires-Dist: psutil ; extra == 'dev' Requires-Dist: pydocstyle ; extra ==
 'dev' Requires-Dist: pylint ; extra == 'dev' Requires-Dist: pytest ; extra ==
 'dev' Requires-Dist: pytest-cov ; extra == 'dev' Requires-Dist: pyyaml ; extra
 == 'dev' Requires-Dist: types-psutil ; extra == 'dev' Requires-Dist: types-
 pyyaml ; extra == 'dev' Provides-Extra: dev License-File: LICENSE License-File:
-LICENSE License-File: AUTHORS.md Summary: Efficient implementations of
-Needleman-Wunsch and other sequence alignment algorithms in Rust with Python
-bindings. Author-email: "Kensho Technologies LLC."
+AUTHORS.md Summary: Efficient implementations of Needleman-Wunsch and other
+sequence alignment algorithms in Rust with Python bindings. Author-email:
+"Kensho Technologies LLC."
 kensho.com> Maintainer-email: "Kensho Technologies LLC."
-kensho.com> Requires-Python: >=3.7 Description-Content-Type: text/markdown;
-charset=UTF-8; variant=GFM Project-URL: source, https://github.com/kensho-
-technologies/sequence_align Project-URL: Homepage, https://github.com/kensho-
-technologies/sequence_align Project-URL: Bug Tracker, https://github.com/
-kensho-technologies/sequence_align/issues _[_h_t_t_p_s_:_/_/_g_i_t_h_u_b_._c_o_m_/_k_e_n_s_h_o_-
-_t_e_c_h_n_o_l_o_g_i_e_s_/_s_e_q_u_e_n_c_e___a_l_i_g_n_/_w_o_r_k_f_l_o_w_s_/_T_e_s_t_s_%_2_0_a_n_d_%_2_0_l_i_n_t_/_b_a_d_g_e_._s_v_g_]_[_h_t_t_p_s_:_/_/
-_c_o_d_e_c_o_v_._i_o_/_g_h_/_k_e_n_s_h_o_-_t_e_c_h_n_o_l_o_g_i_e_s_/_s_e_q_u_e_n_c_e___a_l_i_g_n_/_b_r_a_n_c_h_/_m_a_i_n_/_g_r_a_p_h_/_b_a_d_g_e_._s_v_g_]
-_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_L_i_c_e_n_s_e_-_A_p_a_c_h_e_%_2_0_2_._0_-_b_l_u_e_._s_v_g_]_[_h_t_t_p_:_/_/
+kensho.com> License: Apache-2.0 Requires-Python: >=3.7 Description-Content-
+Type: text/markdown; charset=UTF-8; variant=GFM Project-URL: source, https://
+github.com/kensho-technologies/sequence_align Project-URL: Homepage, https://
+github.com/kensho-technologies/sequence_align Project-URL: Bug Tracker, https:/
+/github.com/kensho-technologies/sequence_align/issues _[_h_t_t_p_s_:_/_/_g_i_t_h_u_b_._c_o_m_/
+_k_e_n_s_h_o_-_t_e_c_h_n_o_l_o_g_i_e_s_/_s_e_q_u_e_n_c_e___a_l_i_g_n_/_w_o_r_k_f_l_o_w_s_/_T_e_s_t_s_%_2_0_a_n_d_%_2_0_l_i_n_t_/_b_a_d_g_e_._s_v_g_]
+_[_h_t_t_p_s_:_/_/_c_o_d_e_c_o_v_._i_o_/_g_h_/_k_e_n_s_h_o_-_t_e_c_h_n_o_l_o_g_i_e_s_/_s_e_q_u_e_n_c_e___a_l_i_g_n_/_b_r_a_n_c_h_/_m_a_i_n_/_g_r_a_p_h_/
+_b_a_d_g_e_._s_v_g_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_L_i_c_e_n_s_e_-_A_p_a_c_h_e_%_2_0_2_._0_-_b_l_u_e_._s_v_g_]_[_h_t_t_p_:_/_/
 _w_w_w_._r_e_p_o_s_t_a_t_u_s_._o_r_g_/_b_a_d_g_e_s_/_l_a_t_e_s_t_/_a_c_t_i_v_e_._s_v_g_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/
 _c_o_d_e_%_2_0_s_t_y_l_e_-_b_l_a_c_k_-_0_0_0_0_0_0_._s_v_g_]# sequence_align Efficient implementations of
 [Needleman-Wunsch](https://en.wikipedia.org/wiki/
 Needleman%E2%80%93Wunsch_algorithm) and other sequence alignment algorithms
 written in Rust with Python bindings via [PyO3](https://github.com/PyO3/pyo3).
 [https://raw.githubusercontent.com/kensho-technologies/sequence_align/main/
 docs/images/sequence_align.png]
```

## Comparing `sequence_align-0.1.1.dist-info/license_files/LICENSE` & `sequence_align-0.1.2.dist-info/license_files/LICENSE`

 * *Files identical despite different names*

## Comparing `sequence_align-0.1.1.dist-info/RECORD` & `sequence_align-0.1.2.dist-info/RECORD`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,9 @@
-sequence_align-0.1.1.dist-info/METADATA,sha256=NUkXPf4LKZ4o8QoZ6f1XDBTjD8YNY2zbX6lN9nod_JI,7495
-sequence_align-0.1.1.dist-info/WHEEL,sha256=2KdwICnFEHl2ghwQAXqeXd9gNxeAiTvogEqUIMDbYbo,94
-sequence_align-0.1.1.dist-info/license_files/LICENSE,sha256=j9q0KoZXpK8fT1GXnUEV0DfgbGQv8XIn35OREXVn920,11566
-sequence_align-0.1.1.dist-info/license_files/LICENSE,sha256=j9q0KoZXpK8fT1GXnUEV0DfgbGQv8XIn35OREXVn920,11566
-sequence_align-0.1.1.dist-info/license_files/AUTHORS.md,sha256=zgfGnnTADSip5x0UBLZc4zlz8y5MHAa7c40hrPBddqE,59
+sequence_align-0.1.2.dist-info/METADATA,sha256=K7vQKXeDaqdTpTRKTmgYTkS8sh7m99tcWPorM_N-sdY,7493
+sequence_align-0.1.2.dist-info/WHEEL,sha256=2KdwICnFEHl2ghwQAXqeXd9gNxeAiTvogEqUIMDbYbo,94
+sequence_align-0.1.2.dist-info/license_files/LICENSE,sha256=j9q0KoZXpK8fT1GXnUEV0DfgbGQv8XIn35OREXVn920,11566
+sequence_align-0.1.2.dist-info/license_files/AUTHORS.md,sha256=zgfGnnTADSip5x0UBLZc4zlz8y5MHAa7c40hrPBddqE,59
 sequence_align/pairwise.py,sha256=Mji0Easoy3nQpWD5BAwOwHnnlRu95SLjy9Cvb2IMV98,6792
 sequence_align/py.typed,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 sequence_align/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-sequence_align/sequence_align.pyd,sha256=HjlBz3kMHLjOtez02mRElgrTzwYHUYT807mQvlQ_MKE,195072
-sequence_align-0.1.1.dist-info/RECORD,,
+sequence_align/_sequence_align.pyd,sha256=rD6kJIAtqd8kNW54g_d0vtYh1ABWzXNpVcTkiFJFLL4,199680
+sequence_align-0.1.2.dist-info/RECORD,,
```

