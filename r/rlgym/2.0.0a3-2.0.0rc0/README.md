# Comparing `tmp/rlgym-2.0.0a3.tar.gz` & `tmp/rlgym-2.0.0rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rlgym-2.0.0a3.tar", last modified: Wed Aug 23 18:42:01 2023, max compression
+gzip compressed data, was "rlgym-2.0.0rc0.tar", last modified: Sat May 18 16:57:45 2024, max compression
```

## Comparing `rlgym-2.0.0a3.tar` & `rlgym-2.0.0rc0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-08-23 18:42:01.275854 rlgym-2.0.0a3/
--rw-rw-rw-   0        0        0    10946 2021-03-04 22:29:53.000000 rlgym-2.0.0a3/LICENSE
--rw-rw-rw-   0        0        0       37 2023-08-19 16:59:10.000000 rlgym-2.0.0a3/MANIFEST.in
--rw-rw-rw-   0        0        0     2750 2023-08-23 18:42:01.272842 rlgym-2.0.0a3/PKG-INFO
--rw-rw-rw-   0        0        0     1929 2023-08-19 21:03:59.000000 rlgym-2.0.0a3/README.md
-drwxrwxrwx   0        0        0        0 2023-08-23 18:42:01.129775 rlgym-2.0.0a3/rlgym/
-drwxrwxrwx   0        0        0        0 2023-08-23 18:42:01.267843 rlgym-2.0.0a3/rlgym/version/
--rw-rw-rw-   0        0        0      132 2023-08-16 18:04:14.000000 rlgym-2.0.0a3/rlgym/version/__init__.py
--rw-rw-rw-   0        0        0     6197 2023-08-23 18:35:27.000000 rlgym-2.0.0a3/rlgym/version/version.py
-drwxrwxrwx   0        0        0        0 2023-08-23 18:42:01.261843 rlgym-2.0.0a3/rlgym.egg-info/
--rw-rw-rw-   0        0        0     2750 2023-08-23 18:42:00.000000 rlgym-2.0.0a3/rlgym.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      244 2023-08-23 18:42:01.000000 rlgym-2.0.0a3/rlgym.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-23 18:42:01.000000 rlgym-2.0.0a3/rlgym.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      220 2023-08-23 18:42:01.000000 rlgym-2.0.0a3/rlgym.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-08-23 18:42:01.000000 rlgym-2.0.0a3/rlgym.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-08-23 18:42:01.276845 rlgym-2.0.0a3/setup.cfg
--rw-rw-rw-   0        0        0     2502 2023-08-23 18:41:55.000000 rlgym-2.0.0a3/setup.json
--rw-rw-rw-   0        0        0      805 2023-08-23 18:04:36.000000 rlgym-2.0.0a3/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-18 16:57:45.398122 rlgym-2.0.0rc0/
+-rw-rw-rw-   0        0        0    10946 2021-03-04 22:29:53.000000 rlgym-2.0.0rc0/LICENSE
+-rw-rw-rw-   0        0        0       37 2023-08-19 16:59:10.000000 rlgym-2.0.0rc0/MANIFEST.in
+-rw-rw-rw-   0        0        0     2776 2024-05-18 16:57:45.398122 rlgym-2.0.0rc0/PKG-INFO
+-rw-rw-rw-   0        0        0     1954 2023-12-03 17:45:55.000000 rlgym-2.0.0rc0/README.md
+drwxrwxrwx   0        0        0        0 2024-05-18 16:57:45.381538 rlgym-2.0.0rc0/rlgym/
+drwxrwxrwx   0        0        0        0 2024-05-18 16:57:45.396121 rlgym-2.0.0rc0/rlgym/version/
+-rw-rw-rw-   0        0        0      132 2023-08-16 18:04:14.000000 rlgym-2.0.0rc0/rlgym/version/__init__.py
+-rw-rw-rw-   0        0        0     6990 2024-05-18 16:37:43.000000 rlgym-2.0.0rc0/rlgym/version/version.py
+drwxrwxrwx   0        0        0        0 2024-05-18 16:57:45.394121 rlgym-2.0.0rc0/rlgym.egg-info/
+-rw-rw-rw-   0        0        0     2776 2024-05-18 16:57:45.000000 rlgym-2.0.0rc0/rlgym.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      244 2024-05-18 16:57:45.000000 rlgym-2.0.0rc0/rlgym.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-18 16:57:45.000000 rlgym-2.0.0rc0/rlgym.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      195 2024-05-18 16:57:45.000000 rlgym-2.0.0rc0/rlgym.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2024-05-18 16:57:45.000000 rlgym-2.0.0rc0/rlgym.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-18 16:57:45.398122 rlgym-2.0.0rc0/setup.cfg
+-rw-rw-rw-   0        0        0     2497 2024-05-18 16:57:42.000000 rlgym-2.0.0rc0/setup.json
+-rw-rw-rw-   0        0        0      805 2023-08-23 18:04:36.000000 rlgym-2.0.0rc0/setup.py
```

### Comparing `rlgym-2.0.0a3/LICENSE` & `rlgym-2.0.0rc0/LICENSE`

 * *Files identical despite different names*

### Comparing `rlgym-2.0.0a3/PKG-INFO` & `rlgym-2.0.0rc0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rlgym
-Version: 2.0.0a3
+Version: 2.0.0rc0
 Summary: A python API with zero dependencies to create fully customizable environments for Reinforcement Learning projects.
 Home-page: https://rlgym.org
 Author: Lucas Emery and Matthew Allen
 Author-email: contact@rlgym.org
 License: Apache 2.0
 Project-URL: Source Code, https://github.com/lucas-emery/rocket-league-gym
 Keywords: rocket-league,gym,reinforcement-learning,rlgym
@@ -46,16 +46,16 @@
 Once the API is installed, you will need to enable the RLGym plugin from inside the Bakkesmod plugin manager. To do this, first launch the game, then press F2 to open the Bakkesmod menu. Navigate to the `plugins` tab and open the `Plugin Manager`. From there, scroll down until you find the RLGym plugin, and enable it. Close the game when this is done.
 
 
 ### Testing everything works
 RLGym is now installed! simply run ```example.py``` from our repo to ensure everything works.
 
 ## Dependency Management
-**Don't** specify this package as a dependency, this is an **instalation only** package.
+**DO NOT** specify this package as a dependency, this is an **installation only** package.
 
-You should depend directly on the package you're consuming and its corresponding extras, be it 
-`rlgym-rocket-league[sim]`, `rlgym-api` or any other in particular.
+You should depend directly on the package you're consuming and its corresponding extras, e.g.
+`rlgym-rocket-league[sim]`, `rlgym-api` or whichever of our libraries your project is using.
 
 ## Usage
 For tutorials and documentation, please visit our [Wiki](https://rlgym.org/).
 
 We also provide the base RLGym API in its own [standalone package](https://pypi.org/project/rlgym-api/) with no dependencies.
```

### Comparing `rlgym-2.0.0a3/README.md` & `rlgym-2.0.0rc0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -24,16 +24,16 @@
 Once the API is installed, you will need to enable the RLGym plugin from inside the Bakkesmod plugin manager. To do this, first launch the game, then press F2 to open the Bakkesmod menu. Navigate to the `plugins` tab and open the `Plugin Manager`. From there, scroll down until you find the RLGym plugin, and enable it. Close the game when this is done.
 
 
 ### Testing everything works
 RLGym is now installed! simply run ```example.py``` from our repo to ensure everything works.
 
 ## Dependency Management
-**Don't** specify this package as a dependency, this is an **instalation only** package.
+**DO NOT** specify this package as a dependency, this is an **installation only** package.
 
-You should depend directly on the package you're consuming and its corresponding extras, be it 
-`rlgym-rocket-league[sim]`, `rlgym-api` or any other in particular.
+You should depend directly on the package you're consuming and its corresponding extras, e.g.
+`rlgym-rocket-league[sim]`, `rlgym-api` or whichever of our libraries your project is using.
 
 ## Usage
 For tutorials and documentation, please visit our [Wiki](https://rlgym.org/).
 
 We also provide the base RLGym API in its own [standalone package](https://pypi.org/project/rlgym-api/) with no dependencies.
```

### Comparing `rlgym-2.0.0a3/rlgym/version/version.py` & `rlgym-2.0.0rc0/rlgym/version/version.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,388 +1,437 @@
 00000000: 0d0a 5f5f 7665 7273 696f 6e5f 5f20 3d20  ..__version__ = 
-00000010: 2732 2e30 2e30 2d61 6c70 6861 2d33 270d  '2.0.0-alpha-3'.
-00000020: 0a0d 0a0d 0a23 2054 4f44 4f20 636f 6e73  .....# TODO cons
-00000030: 756d 6520 7375 6270 6163 6b61 6765 7320  ume subpackages 
-00000040: 696e 7374 6561 643f 0d0a 6465 6620 6765  instead?..def ge
-00000050: 745f 6375 7272 656e 745f 7265 6c65 6173  t_current_releas
-00000060: 655f 6e6f 7465 7328 293a 0d0a 2020 2020  e_notes():..    
-00000070: 6966 205f 5f76 6572 7369 6f6e 5f5f 2069  if __version__ i
-00000080: 6e20 7265 6c65 6173 655f 6e6f 7465 733a  n release_notes:
-00000090: 0d0a 2020 2020 2020 2020 7265 7475 726e  ..        return
-000000a0: 2072 656c 6561 7365 5f6e 6f74 6573 5b5f   release_notes[_
-000000b0: 5f76 6572 7369 6f6e 5f5f 5d0d 0a20 2020  _version__]..   
-000000c0: 2072 6574 7572 6e20 2727 0d0a 0d0a 0d0a   return ''......
-000000d0: 6465 6620 7072 696e 745f 6375 7272 656e  def print_curren
-000000e0: 745f 7265 6c65 6173 655f 6e6f 7465 7328  t_release_notes(
-000000f0: 293a 0d0a 2020 2020 7072 696e 7428 6622  ):..    print(f"
-00000100: 5665 7273 696f 6e20 7b5f 5f76 6572 7369  Version {__versi
-00000110: 6f6e 5f5f 7d22 290d 0a20 2020 2070 7269  on__}")..    pri
-00000120: 6e74 2867 6574 5f63 7572 7265 6e74 5f72  nt(get_current_r
-00000130: 656c 6561 7365 5f6e 6f74 6573 2829 290d  elease_notes()).
-00000140: 0a20 2020 2070 7269 6e74 2822 2229 0d0a  .    print("")..
-00000150: 0d0a 0d0a 7265 6c65 6173 655f 6e6f 7465  ....release_note
-00000160: 7320 3d20 7b0d 0a20 2020 2027 322e 302e  s = {..    '2.0.
-00000170: 302d 616c 7068 612d 3327 3a0d 0a20 2020  0-alpha-3':..   
-00000180: 2022 2222 0d0a 2020 2020 2d20 5468 6973   """..    - This
-00000190: 2076 6572 7369 6f6e 2063 6f6e 7461 696e   version contain
-000001a0: 7320 6e75 6d65 726f 7573 2075 6e74 6573  s numerous untes
-000001b0: 7465 6420 616e 6420 6272 6561 6b69 6e67  ted and breaking
-000001c0: 2063 6861 6e67 6573 2e20 5275 6e20 6174   changes. Run at
-000001d0: 2079 6f75 7220 6f77 6e20 7269 736b 2e0d   your own risk..
-000001e0: 0a20 2020 202d 2046 6978 6564 2050 7974  .    - Fixed Pyt
-000001f0: 686f 6e20 3c33 2e39 2069 6e73 7461 6c6c  hon <3.9 install
-00000200: 0d0a 2020 2020 4150 4920 6368 616e 6765  ..    API change
-00000210: 733a 0d0a 2020 2020 2020 2020 2d20 4164  s:..        - Ad
-00000220: 6465 6420 7368 6172 6564 5f69 6e66 6f20  ded shared_info 
-00000230: 7061 7261 6d20 746f 2054 7261 6e73 6974  param to Transit
-00000240: 696f 6e45 6e67 696e 6520 616e 6420 5265  ionEngine and Re
-00000250: 6e64 6572 6572 0d0a 2020 2020 2020 2020  nderer..        
-00000260: 2d20 4d6f 7665 2072 6c67 796d 2e61 7069  - Move rlgym.api
-00000270: 2e65 6e67 696e 6520 746f 2072 6c67 796d  .engine to rlgym
-00000280: 2e61 7069 2e63 6f6e 6669 670d 0a20 2020  .api.config..   
-00000290: 2052 6f63 6b65 744c 6561 6775 6520 6368   RocketLeague ch
-000002a0: 616e 6765 733a 0d0a 2020 2020 2020 2020  anges:..        
-000002b0: 2d20 5570 6461 7465 2069 6d70 6f72 7473  - Update imports
-000002c0: 2074 6f20 726c 6779 6d2e 6170 690d 0a20   to rlgym.api.. 
-000002d0: 2020 2020 2020 202d 2052 656e 616d 6520         - Rename 
-000002e0: 726c 6779 6d2e 726f 636b 6574 5f6c 6561  rlgym.rocket_lea
-000002f0: 6775 652e 656e 6769 6e65 2074 6f20 726c  gue.engine to rl
-00000300: 6779 6d2e 726f 636b 6574 5f6c 6561 6775  gym.rocket_leagu
-00000310: 652e 6170 690d 0a20 2020 2020 2020 202d  e.api..        -
-00000320: 2049 6d70 726f 7665 2065 7870 6f72 7473   Improve exports
-00000330: 2073 6f20 696d 706f 7274 7320 6172 6520   so imports are 
-00000340: 6d6f 7265 2063 6f6e 736f 6c69 6461 7465  more consolidate
-00000350: 640d 0a20 2020 2022 2222 2c0d 0a20 2020  d..    """,..   
-00000360: 2027 322e 302e 302d 616c 7068 612d 3227   '2.0.0-alpha-2'
-00000370: 3a0d 0a20 2020 2022 2222 0d0a 2020 2020  :..    """..    
-00000380: 2d20 5468 6973 2076 6572 7369 6f6e 2063  - This version c
-00000390: 6f6e 7461 696e 7320 6e75 6d65 726f 7573  ontains numerous
-000003a0: 2075 6e74 6573 7465 6420 616e 6420 706f   untested and po
-000003b0: 7465 6e74 6961 6c6c 7920 6272 6561 6b69  tentially breaki
-000003c0: 6e67 2063 6861 6e67 6573 2e20 5275 6e20  ng changes. Run 
-000003d0: 6174 2079 6f75 7220 6f77 6e20 7269 736b  at your own risk
-000003e0: 2e0d 0a20 2020 202d 2046 6978 6564 2072  ...    - Fixed r
-000003f0: 6c76 6973 6572 2d70 7920 6465 7065 6e64  lviser-py depend
-00000400: 656e 6379 2076 6572 7369 6f6e 0d0a 2020  ency version..  
-00000410: 2020 2222 222c 0d0a 2020 2020 2732 2e30    """,..    '2.0
-00000420: 2e30 2d61 6c70 6861 2d31 273a 0d0a 2020  .0-alpha-1':..  
-00000430: 2020 2222 220d 0a20 2020 202d 2054 6869    """..    - Thi
-00000440: 7320 7665 7273 696f 6e20 636f 6e74 6169  s version contai
-00000450: 6e73 206e 756d 6572 6f75 7320 756e 7465  ns numerous unte
-00000460: 7374 6564 2061 6e64 2070 6f74 656e 7469  sted and potenti
-00000470: 616c 6c79 2062 7265 616b 696e 6720 6368  ally breaking ch
-00000480: 616e 6765 732e 2052 756e 2061 7420 796f  anges. Run at yo
-00000490: 7572 206f 776e 2072 6973 6b2e 0d0a 2020  ur own risk...  
-000004a0: 2020 2d20 4c69 6674 6564 2050 7974 686f    - Lifted Pytho
-000004b0: 6e20 3c33 2e31 3020 7265 7374 7269 6374  n <3.10 restrict
-000004c0: 696f 6e0d 0a20 2020 2022 2222 2c0d 0a20  ion..    """,.. 
-000004d0: 2020 2027 322e 302e 302d 616c 7068 6127     '2.0.0-alpha'
-000004e0: 3a0d 0a20 2020 2022 2222 0d0a 2020 2020  :..    """..    
-000004f0: 2d20 5468 6973 2076 6572 7369 6f6e 2063  - This version c
-00000500: 6f6e 7461 696e 7320 6e75 6d65 726f 7573  ontains numerous
-00000510: 2075 6e74 6573 7465 6420 616e 6420 706f   untested and po
-00000520: 7465 6e74 6961 6c6c 7920 6272 6561 6b69  tentially breaki
-00000530: 6e67 2063 6861 6e67 6573 2e20 5275 6e20  ng changes. Run 
-00000540: 6174 2079 6f75 7220 6f77 6e20 7269 736b  at your own risk
-00000550: 2e0d 0a20 2020 2022 2222 2c0d 0a20 2020  ...    """,..   
-00000560: 2027 312e 322e 3227 3a0d 0a20 2020 2022   '1.2.2':..    "
-00000570: 2222 0d0a 2020 2020 2d20 4669 7865 6420  ""..    - Fixed 
-00000580: 6d61 7820 7079 7468 6f6e 2076 6572 7369  max python versi
-00000590: 6f6e 0d0a 2020 2020 2222 222c 0d0a 2020  on..    """,..  
-000005a0: 2020 2731 2e32 2e31 273a 0d0a 2020 2020    '1.2.1':..    
-000005b0: 2222 220d 0a20 2020 202d 2046 6978 6564  """..    - Fixed
-000005c0: 2065 7069 6320 7665 7273 696f 6e20 6372   epic version cr
-000005d0: 6173 6869 6e67 2069 6e73 7461 6e74 6c79  ashing instantly
-000005e0: 202d 2042 616b 6b65 730d 0a20 2020 202d   - Bakkes..    -
-000005f0: 2041 6464 6564 206d 6178 2070 7974 686f   Added max pytho
-00000600: 6e20 7665 7273 696f 6e0d 0a20 2020 202d  n version..    -
-00000610: 2041 6464 6564 2041 6374 696f 6e50 6172   Added ActionPar
-00000620: 7365 7220 746f 2075 7469 6c73 2073 7562  ser to utils sub
-00000630: 6d6f 6475 6c65 0d0a 2020 2020 2d20 5570  module..    - Up
-00000640: 6461 7465 6420 6465 6661 756c 7420 7265  dated default re
-00000650: 7761 7264 2c20 6974 206e 6f77 206d 696e  ward, it now min
-00000660: 696d 697a 6573 206c 696e 6561 7220 7665  imizes linear ve
-00000670: 6c6f 6369 7479 2069 6e73 7465 6164 206f  locity instead o
-00000680: 6620 616e 6775 6c61 720d 0a20 2020 202d  f angular..    -
-00000690: 2052 4950 2052 686f 626f 744f 6273 0d0a   RIP RhobotObs..
-000006a0: 2020 2020 2222 222c 0d0a 2020 2020 2731      """,..    '1
-000006b0: 2e32 2e30 273a 2022 2222 0d0a 2020 2020  .2.0': """..    
-000006c0: 2d20 4465 7072 6563 6174 6564 2073 656c  - Deprecated sel
-000006d0: 665f 706c 6179 2066 6c61 672c 2070 6c61  f_play flag, pla
-000006e0: 7969 6e67 2061 6761 696e 7374 2050 7379  ying against Psy
-000006f0: 6f6e 6978 2061 6765 6e74 7320 6973 206e  onix agents is n
-00000700: 6f20 6c6f 6e67 6572 2073 7570 706f 7274  o longer support
-00000710: 6564 0d0a 2020 2020 2d20 4164 6465 6420  ed..    - Added 
-00000720: 6861 735f 6a75 6d70 2074 6f20 506c 6179  has_jump to Play
-00000730: 6572 4461 7461 2c20 7768 6963 6820 6973  erData, which is
-00000740: 2075 7365 6675 6c20 746f 2064 6574 6563   useful to detec
-00000750: 7420 7768 656e 2061 2066 6c69 7020 776f  t when a flip wo
-00000760: 6e27 7420 7275 6e20 6f75 740d 0a20 2020  n't run out..   
-00000770: 202d 2041 6464 6564 2070 7265 5f73 7465   - Added pre_ste
-00000780: 7028 2920 6675 6e63 7469 6f6e 2074 6f20  p() function to 
-00000790: 4f62 7342 7569 6c64 6572 2061 6e64 2052  ObsBuilder and R
-000007a0: 6577 6172 6446 756e 6374 696f 6e2c 2075  ewardFunction, u
-000007b0: 7365 6675 6c20 666f 7220 7072 652d 6361  seful for pre-ca
-000007c0: 6c63 756c 6174 696e 6720 7374 7566 6620  lculating stuff 
-000007d0: 6561 6368 2073 7465 700d 0a20 2020 202d  each step..    -
-000007e0: 2041 6464 6564 2073 7570 706f 7274 2066   Added support f
-000007f0: 6f72 2063 6861 6e67 696e 6720 6761 6d65  or changing game
-00000800: 6d6f 6465 2077 6974 686f 7574 2072 6573  mode without res
-00000810: 7461 7274 696e 6720 524c 4779 6d2c 2073  tarting RLGym, s
-00000820: 6565 2053 7461 7465 5365 7474 6572 2e62  ee StateSetter.b
-00000830: 7569 6c64 5f77 7261 7070 6572 2829 0d0a  uild_wrapper()..
-00000840: 2020 2020 2d20 4164 6465 6420 6772 6176      - Added grav
-00000850: 6974 7920 616e 6420 626f 6f73 745f 636f  ity and boost_co
-00000860: 6e73 756d 7074 696f 6e20 636f 6e66 6967  nsumption config
-00000870: 7572 6174 696f 6e20 746f 2072 6c67 796d  uration to rlgym
-00000880: 2e6d 616b 6528 290d 0a20 2020 202d 2041  .make()..    - A
-00000890: 6464 6564 2075 7064 6174 655f 7365 7474  dded update_sett
-000008a0: 696e 6773 2829 206d 6574 686f 6420 746f  ings() method to
-000008b0: 2067 796d 2c20 666f 7220 7570 6461 7469   gym, for updati
-000008c0: 6e67 2073 6f6d 6520 7061 7274 7320 6f66  ng some parts of
-000008d0: 2074 6865 2063 6f6e 6669 6720 7769 7468   the config with
-000008e0: 6f75 7420 7265 7374 6172 7469 6e67 0d0a  out restarting..
-000008f0: 2020 2020 2d20 4164 6465 6420 6765 745f      - Added get_
-00000900: 6f62 735f 7370 6163 6528 2920 746f 204f  obs_space() to O
-00000910: 6273 4275 696c 6465 722c 2065 6e61 626c  bsBuilder, enabl
-00000920: 6573 206f 7665 7272 6964 696e 6720 524c  es overriding RL
-00000930: 4779 6d27 7320 6175 746f 6d61 7469 6320  Gym's automatic 
-00000940: 6f62 7320 7369 7a65 2064 6574 6563 7469  obs size detecti
-00000950: 6f6e 0d0a 2020 2020 2d20 4164 6465 6420  on..    - Added 
-00000960: 7261 6973 655f 6f6e 5f63 7261 7368 206f  raise_on_crash o
-00000970: 7074 696f 6e20 746f 2072 6c67 796d 2e6d  ption to rlgym.m
-00000980: 616b 6528 290d 0a20 2020 202d 2041 6464  ake()..    - Add
-00000990: 6564 2061 7574 6f5f 6d69 6e69 6d69 7a65  ed auto_minimize
-000009a0: 206f 7074 696f 6e20 746f 2072 6c67 796d   option to rlgym
-000009b0: 2e6d 616b 6528 290d 0a20 2020 202d 2041  .make()..    - A
-000009c0: 6464 6564 2062 6f6f 7374 2070 6963 6b75  dded boost picku
-000009d0: 7073 2074 6f20 6576 656e 7420 7265 7761  ps to event rewa
-000009e0: 7264 202d 2079 6164 6172 6166 0d0a 2020  rd - yadaraf..  
-000009f0: 2020 2d20 4669 7865 6420 6375 7374 6f6d    - Fixed custom
-00000a00: 2062 696e 2073 7570 706f 7274 2069 6e20   bin support in 
-00000a10: 4469 7363 7265 7465 4163 7469 6f6e 202d  DiscreteAction -
-00000a20: 204b 6169 796f 7465 6368 0d0a 2020 2020   Kaiyotech..    
-00000a30: 2d20 4669 7865 6420 6275 6720 696e 2056  - Fixed bug in V
-00000a40: 656c 6f63 6974 7942 616c 6c54 6f47 6f61  elocityBallToGoa
-00000a50: 6c52 6577 6172 6420 616e 6420 5665 6c6f  lReward and Velo
-00000a60: 6369 7479 506c 6179 6572 546f 4261 6c6c  cityPlayerToBall
-00000a70: 5265 7761 7264 0d0a 2020 2020 2d20 4669  Reward..    - Fi
-00000a80: 7865 6420 506c 6179 6572 4461 7461 2073  xed PlayerData s
-00000a90: 7472 696e 6720 7265 7072 6573 656e 7461  tring representa
-00000aa0: 7469 6f6e 202d 2043 6172 726f 740d 0a20  tion - Carrot.. 
-00000ab0: 2020 2022 2222 2c0d 0a20 2020 2027 312e     """,..    '1.
-00000ac0: 312e 3027 3a20 2222 220d 0a20 2020 202d  1.0': """..    -
-00000ad0: 2041 6464 6564 2041 6374 696f 6e50 6172   Added ActionPar
-00000ae0: 7365 7273 2c20 7768 6963 6820 616c 6c6f  sers, which allo
-00000af0: 7720 796f 7520 746f 2064 6566 696e 6520  w you to define 
-00000b00: 6375 7374 6f6d 2061 6374 696f 6e20 7370  custom action sp
-00000b10: 6163 6573 202d 204c 6f6c 6161 706b 330d  aces - Lolaapk3.
-00000b20: 0a20 2020 202d 2046 6978 6564 2071 7561  .    - Fixed qua
-00000b30: 7465 726e 696f 6e20 746f 2065 756c 6572  ternion to euler
-00000b40: 2061 6e67 6c65 2063 6f6e 7665 7273 696f   angle conversio
-00000b50: 6e20 2d20 4461 7278 6561 6c0d 0a20 2020  n - Darxeal..   
-00000b60: 202d 2049 6d70 726f 7665 6420 4465 6661   - Improved Defa
-00000b70: 756c 744f 6273 2c20 6974 206e 6f77 2068  ultObs, it now h
-00000b80: 6173 2061 6c6c 2074 6865 2073 7461 7465  as all the state
-00000b90: 2069 6e66 6f72 6d61 7469 6f6e 0d0a 2020   information..  
-00000ba0: 2020 2d20 4164 6465 6420 6f70 7469 6f6e    - Added option
-00000bb0: 616c 2070 6172 616d 6574 6572 2074 6f20  al parameter to 
-00000bc0: 7265 7475 726e 2069 6e69 7469 616c 2069  return initial i
-00000bd0: 6e66 6f20 6f62 6a65 6374 206f 6e20 656e  nfo object on en
-00000be0: 762e 7265 7365 7428 290d 0a20 2020 202d  v.reset()..    -
-00000bf0: 2046 6978 6564 2072 616e 645f 7665 6333   Fixed rand_vec3
-00000c00: 2073 6f20 7468 6520 6d61 676e 6974 7564   so the magnitud
-00000c10: 6520 6973 2061 6374 7561 6c6c 7920 7261  e is actually ra
-00000c20: 6e64 6f6d 0d0a 2020 2020 2222 222c 0d0a  ndom..    """,..
-00000c30: 2020 2020 2731 2e30 2e32 273a 2022 2222      '1.0.2': """
-00000c40: 0d0a 2020 2020 2d20 4669 7865 6420 7374  ..    - Fixed st
-00000c50: 6174 6520 7365 7474 696e 6720 6973 7375  ate setting issu
-00000c60: 6573 2028 626f 6f73 7420 7365 7474 696e  es (boost settin
-00000c70: 6720 616e 6420 7072 6563 6973 696f 6e29  g and precision)
-00000c80: 0d0a 2020 2020 2222 222c 0d0a 2020 2020  ..    """,..    
-00000c90: 2731 2e30 2e31 273a 2022 2222 0d0a 2020  '1.0.1': """..  
-00000ca0: 2020 2d20 4d69 6e6f 7220 6669 7820 666f    - Minor fix fo
-00000cb0: 7220 5261 6e64 6f6d 5374 6174 650d 0a20  r RandomState.. 
-00000cc0: 2020 2022 2222 2c0d 0a20 2020 2027 312e     """,..    '1.
-00000cd0: 302e 3027 3a20 2222 220d 0a20 2020 202d  0.0': """..    -
-00000ce0: 2041 6464 6564 2073 7461 7465 2073 6574   Added state set
-00000cf0: 7469 6e67 2c20 796f 7520 6361 6e20 6e6f  ting, you can no
-00000d00: 7720 7370 6563 6966 7920 7468 6520 696e  w specify the in
-00000d10: 6974 6961 6c20 7374 6174 6520 6f66 2065  itial state of e
-00000d20: 7069 736f 6465 7320 7669 6120 6120 5374  pisodes via a St
-00000d30: 6174 6553 6574 7465 7220 6f62 6a65 6374  ateSetter object
-00000d40: 202d 2061 6954 616e 0d0a 2020 2020 2d20   - aiTan..    - 
-00000d50: 4164 6465 6420 6c61 756e 6368 5f70 7265  Added launch_pre
-00000d60: 6665 7265 6e63 6520 746f 206d 616b 6528  ference to make(
-00000d70: 290d 0a20 2020 202d 2046 6978 6564 2045  )..    - Fixed E
-00000d80: 7069 6320 6c61 756e 6368 2062 7567 2069  pic launch bug i
-00000d90: 6e74 726f 6475 6365 6420 7769 7468 2074  ntroduced with t
-00000da0: 6865 2053 6561 736f 6e20 3420 7570 6461  he Season 4 upda
-00000db0: 7465 0d0a 2020 2020 2d20 436f 6d6d 756e  te..    - Commun
-00000dc0: 6963 6174 696f 6e20 636f 6465 2072 6566  ication code ref
-00000dd0: 6163 746f 7265 6420 746f 2069 6e63 7265  actored to incre
-00000de0: 6173 6520 7065 7266 6f72 6d61 6e63 6520  ase performance 
-00000df0: 7769 7468 206c 6f77 2074 6963 6b5f 736b  with low tick_sk
-00000e00: 6970 0d0a 2020 2020 2d20 4669 7865 6420  ip..    - Fixed 
-00000e10: 626f 6f73 7420 7061 6420 7265 7365 7420  boost pad reset 
-00000e20: 6275 6720 6f6e 2065 7069 736f 6465 2072  bug on episode r
-00000e30: 6573 6574 0d0a 2020 2020 2d20 4164 6465  eset..    - Adde
-00000e40: 6420 6465 7465 6374 696f 6e20 6d65 6368  d detection mech
-00000e50: 616e 6973 6d20 666f 7220 6768 6f73 7420  anism for ghost 
-00000e60: 6261 6c6c 2062 7567 0d0a 2020 2020 2d20  ball bug..    - 
-00000e70: 4465 6372 6561 7365 6420 7265 7175 6972  Decreased requir
-00000e80: 6564 2061 6363 6573 7320 7269 6768 7473  ed access rights
-00000e90: 2062 7920 7468 6520 4d75 6c74 6949 6e6a   by the MultiInj
-00000ea0: 6563 746f 720d 0a20 2020 2022 2222 2c0d  ector..    """,.
-00000eb0: 0a20 2020 2027 302e 362e 3027 3a20 2222  .    '0.6.0': ""
-00000ec0: 220d 0a20 2020 202d 204d 6f76 6564 2077  "..    - Moved w
-00000ed0: 7261 7070 6572 7320 616e 6420 7265 706c  rappers and repl
-00000ee0: 6179 2063 6f6e 7665 7274 6572 2074 6f20  ay converter to 
-00000ef0: 726c 6779 6d2d 746f 6f6c 7320 7061 636b  rlgym-tools pack
-00000f00: 6167 650d 0a20 2020 202d 2041 6464 6564  age..    - Added
-00000f10: 2074 6865 206f 7074 696f 6e61 6c20 6162   the optional ab
-00000f20: 696c 6974 7920 746f 2066 6f72 6365 6675  ility to forcefu
-00000f30: 6c6c 7920 7061 6765 2074 6865 2073 7061  lly page the spa
-00000f40: 776e 6564 2052 6f63 6b65 7420 4c65 6167  wned Rocket Leag
-00000f50: 7565 2069 6e73 7461 6e63 6573 2075 706f  ue instances upo
-00000f60: 6e20 6372 6561 7469 6f6e 202d 2034 3136  n creation - 416
-00000f70: 6336 3136 650d 0a20 2020 202d 2054 6865  c616e..    - The
-00000f80: 2070 6174 685f 746f 5f72 6c20 7061 7261   path_to_rl para
-00000f90: 6d20 6973 206e 6f20 6c6f 6e67 6572 2072  m is no longer r
-00000fa0: 6571 7569 7265 6420 666f 7220 7573 655f  equired for use_
-00000fb0: 696e 6a65 6374 6f72 0d0a 2020 2020 2222  injector..    ""
-00000fc0: 222c 0d0a 2020 2020 2730 2e35 2e30 273a  ",..    '0.5.0':
-00000fd0: 2022 2222 0d0a 2020 2020 2d20 5265 6d6f   """..    - Remo
-00000fe0: 7665 6420 7374 7269 6e67 2062 6173 6564  ved string based
-00000ff0: 2063 6f6e 6669 6775 7261 7469 6f6e 7320   configurations 
-00001000: 696e 2072 6c67 796d 2e6d 616b 6528 292c  in rlgym.make(),
-00001010: 2065 7665 7279 7468 696e 6720 6973 2070   everything is p
-00001020: 6173 7365 6420 6279 206b 7761 7267 7320  assed by kwargs 
-00001030: 6e6f 7720 2d20 536f 7265 6e0d 0a20 2020  now - Soren..   
-00001040: 202d 2041 6464 6564 2053 7461 626c 6542   - Added StableB
-00001050: 6173 656c 696e 6573 3320 636f 6d70 6174  aselines3 compat
-00001060: 6962 696c 6974 7920 2d20 526f 6c76 0d0a  ibility - Rolv..
-00001070: 2020 2020 2d20 5265 6661 6374 6f72 6564      - Refactored
-00001080: 2061 6e64 2065 7870 616e 6465 6420 7265   and expanded re
-00001090: 7761 7264 2066 756e 6374 696f 6e73 202d  ward functions -
-000010a0: 2052 6f6c 760d 0a20 2020 202d 2041 6464   Rolv..    - Add
-000010b0: 6564 2072 6570 6c61 7920 636f 6e76 6572  ed replay conver
-000010c0: 7465 7220 2d20 526f 6c76 0d0a 2020 2020  ter - Rolv..    
-000010d0: 2d20 4669 7865 6420 546f 7563 6842 616c  - Fixed TouchBal
-000010e0: 6c52 6577 6172 6420 6275 6720 2d20 4b65  lReward bug - Ke
-000010f0: 7669 6e0d 0a0d 0a20 2020 204e 4f54 453a  vin....    NOTE:
-00001100: 2053 6f6d 6520 6f66 2074 6865 7365 206e   Some of these n
-00001110: 6577 2074 6f6f 6c73 2028 7772 6170 7065  ew tools (wrappe
-00001120: 7273 2c20 7265 706c 6179 2063 6f6e 7665  rs, replay conve
-00001130: 7274 6572 2c20 6574 6329 2077 696c 6c20  rter, etc) will 
-00001140: 6265 206d 6f76 6564 2074 6f20 6120 6469  be moved to a di
-00001150: 6666 6572 656e 7420 7061 636b 6167 6520  fferent package 
-00001160: 696e 2074 6865 206e 6578 7420 7265 6c65  in the next rele
-00001170: 6173 650d 0a20 2020 2022 2222 2c0d 0a20  ase..    """,.. 
-00001180: 2020 2027 302e 342e 3127 3a20 2222 220d     '0.4.1': """.
-00001190: 0a20 2020 202d 2055 7064 6174 6564 2065  .    - Updated e
-000011a0: 756c 6572 2061 6e67 6c65 7320 746f 206d  uler angles to m
-000011b0: 6174 6368 2072 6c62 6f74 205b 7069 7463  atch rlbot [pitc
-000011c0: 682c 2079 6177 2c20 726f 6c6c 5d20 616e  h, yaw, roll] an
-000011d0: 6420 6164 6465 6420 6163 6365 7373 6f72  d added accessor
-000011e0: 2066 756e 6374 696f 6e73 0d0a 2020 2020   functions..    
-000011f0: 2d20 4275 6766 6978 3a20 706c 6179 6572  - Bugfix: player
-00001200: 2e69 735f 616c 6976 6520 7265 6e61 6d65  .is_alive rename
-00001210: 6420 746f 2069 735f 6465 6d6f 6564 0d0a  d to is_demoed..
-00001220: 2020 2020 2d20 4164 6465 6420 636f 6d6d      - Added comm
-00001230: 6f6e 2072 6577 6172 6473 202d 2052 6f6c  on rewards - Rol
-00001240: 760d 0a20 2020 202d 2041 6464 6564 2061  v..    - Added a
-00001250: 2072 6577 6172 6420 636f 6d62 696e 6572   reward combiner
-00001260: 202d 2043 6861 696e 736f 0d0a 2020 2020   - Chainso..    
-00001270: 2d20 4164 6465 6420 6d69 7373 696e 6720  - Added missing 
-00001280: 6b69 636b 6f66 6620 7370 6177 6e0d 0a20  kickoff spawn.. 
-00001290: 2020 202d 2046 6978 6564 2032 7632 2061     - Fixed 2v2 a
-000012a0: 6e64 2033 7633 2061 6374 696f 6e20 6465  nd 3v3 action de
-000012b0: 6c69 7665 7279 0d0a 2020 2020 2d20 4669  livery..    - Fi
-000012c0: 7865 6420 6973 7375 6520 696e 2032 7632  xed issue in 2v2
-000012d0: 2061 6e64 2033 7633 2077 6865 7265 2062   and 3v3 where b
-000012e0: 6c75 6520 626f 7473 2077 6f75 6c64 2064  lue bots would d
-000012f0: 6973 6170 7065 6172 206f 7665 7220 7469  isappear over ti
-00001300: 6d65 0d0a 2020 2020 2d20 4164 6465 6420  me..    - Added 
-00001310: 6d75 6c74 6920 696e 6a65 6374 6f72 0d0a  multi injector..
-00001320: 2020 2020 2222 222c 0d0a 2020 2020 2730      """,..    '0
-00001330: 2e34 2e30 273a 2022 2222 0d0a 2020 2020  .4.0': """..    
-00001340: 2d20 4d61 6a6f 7220 4150 4920 7265 6661  - Major API refa
-00001350: 6374 6f72 0d0a 2020 2020 2d20 4164 6465  ctor..    - Adde
-00001360: 6420 626f 6f73 7470 6164 2062 6f6f 6c65  d boostpad boole
-00001370: 616e 2061 7272 6179 2074 6f20 4761 6d65  an array to Game
-00001380: 5374 6174 650d 0a20 2020 202d 2052 4c47  State..    - RLG
-00001390: 796d 2069 7320 6e6f 7720 6261 7365 6c69  ym is now baseli
-000013a0: 6e65 7320 636f 6d70 6174 6962 6c65 0d0a  nes compatible..
-000013b0: 2020 2020 2d20 4164 6465 6420 696d 7072      - Added impr
-000013c0: 6f76 6564 2044 6566 6175 6c74 2063 6f6e  oved Default con
-000013d0: 6669 6775 7261 7469 6f6e 0d0a 2020 2020  figuration..    
-000013e0: 2222 222c 0d0a 2020 2020 2730 2e33 2e30  """,..    '0.3.0
-000013f0: 273a 2022 2222 0d0a 2020 2020 2d20 5061  ': """..    - Pa
-00001400: 7373 2069 6e69 7469 616c 2073 7461 7465  ss initial state
-00001410: 2074 6f20 656e 7620 636f 6d70 6f6e 656e   to env componen
-00001420: 7473 206f 6e20 6779 6d2e 7265 7365 7428  ts on gym.reset(
-00001430: 290d 0a20 2020 202d 2050 6173 7320 7072  )..    - Pass pr
-00001440: 6576 2061 6374 696f 6e20 746f 2072 6577  ev action to rew
-00001450: 6172 6420 666e 0d0a 2020 2020 2d20 696e  ard fn..    - in
-00001460: 666f 2072 6574 7572 6e65 6420 6672 6f6d  fo returned from
-00001470: 2067 796d 2e73 7465 7028 2920 6973 206e   gym.step() is n
-00001480: 6f77 2061 2044 6963 740d 0a20 2020 202d  ow a Dict..    -
-00001490: 2046 6978 6564 206f 6273 2073 697a 6520   Fixed obs size 
-000014a0: 6275 6720 696e 2052 686f 626f 744f 6273  bug in RhobotObs
-000014b0: 0d0a 2020 2020 2222 222c 0d0a 2020 2020  ..    """,..    
-000014c0: 2730 2e32 2e30 273a 2022 2222 0d0a 2020  '0.2.0': """..  
-000014d0: 2020 2d20 5377 6974 6368 6564 2066 726f    - Switched fro
-000014e0: 6d20 6375 7374 6f6d 5f61 7267 7320 6469  m custom_args di
-000014f0: 6374 2074 6f20 6b65 7977 6f72 6420 6172  ct to keyword ar
-00001500: 6773 2069 6e20 726c 6779 6d2e 6d61 6b65  gs in rlgym.make
-00001510: 2829 0d0a 2020 2020 2222 222c 0d0a 2020  ()..    """,..  
-00001520: 2020 2730 2e31 2e34 273a 2022 2222 0d0a    '0.1.4': """..
-00001530: 2020 2020 2d20 4779 6d20 6e6f 7720 696e      - Gym now in
-00001540: 6865 7269 7473 206f 7065 6e61 692e 6779  herits openai.gy
-00001550: 6d2e 456e 7620 2d20 4368 6169 6e73 6f0d  m.Env - Chainso.
-00001560: 0a20 2020 202d 2046 6978 6564 2062 7567  .    - Fixed bug
-00001570: 2077 6865 7265 2072 6c67 796d 2063 7261   where rlgym cra
-00001580: 7368 6564 2074 7279 696e 6720 746f 2070  shed trying to p
-00001590: 6172 7365 2074 6865 2073 7461 7465 2073  arse the state s
-000015a0: 7472 696e 6720 696e 2073 6f6d 6520 7363  tring in some sc
-000015b0: 656e 6172 696f 730d 0a20 2020 2022 2222  enarios..    """
-000015c0: 2c0d 0a20 2020 2027 302e 312e 3327 3a20  ,..    '0.1.3': 
-000015d0: 2222 220d 0a20 2020 202d 2052 656e 616d  """..    - Renam
-000015e0: 6564 2050 6879 7369 6373 4f62 6a65 6374  ed PhysicsObject
-000015f0: 2e6f 7269 656e 7461 7469 6f6e 2074 6f20  .orientation to 
-00001600: 6575 6c65 725f 616e 676c 6573 0d0a 2020  euler_angles..  
-00001610: 2020 2d20 6575 6c65 725f 616e 676c 6573    - euler_angles
-00001620: 2069 7320 6e6f 7720 6120 6675 6e63 7469   is now a functi
-00001630: 6f6e 2073 6f20 7468 6579 2061 7265 6e27  on so they aren'
-00001640: 7420 6361 6c63 756c 6174 6564 2069 6620  t calculated if 
-00001650: 6e6f 7420 6e65 6564 6564 0d0a 2020 2020  not needed..    
-00001660: 2d20 4164 6465 6420 726f 7461 7469 6f6e  - Added rotation
-00001670: 5f6d 7478 2c20 666f 7277 6172 642c 2072  _mtx, forward, r
-00001680: 6967 6874 2061 6e64 2075 7020 7665 6374  ight and up vect
-00001690: 6f72 7320 746f 2050 6879 7369 6373 4f62  ors to PhysicsOb
-000016a0: 6a65 6374 2028 6f6e 6c79 2075 7361 626c  ject (only usabl
-000016b0: 6520 666f 7220 7468 6520 6361 7229 0d0a  e for the car)..
-000016c0: 2020 2020 2d20 5265 6d6f 7665 6420 636f      - Removed co
-000016d0: 6e76 6572 7369 6f6e 2074 6f20 6e70 2061  nversion to np a
-000016e0: 7272 6179 2066 6f72 2072 6577 6172 6473  rray for rewards
-000016f0: 2061 6e64 206f 6273 6572 7661 7469 6f6e   and observation
-00001700: 730d 0a20 2020 202d 2046 6978 6564 2062  s..    - Fixed b
-00001710: 7567 2069 6e20 5268 6f62 6f74 4f62 730d  ug in RhobotObs.
-00001720: 0a20 2020 2022 2222 2c0d 0a20 2020 2027  .    """,..    '
-00001730: 302e 312e 3227 3a20 2222 220d 0a20 2020  0.1.2': """..   
-00001740: 202d 204f 6273 2061 7265 206e 6f77 206e   - Obs are now n
-00001750: 756d 7079 2061 7272 6179 730d 0a20 2020  umpy arrays..   
-00001760: 202d 2041 6464 6564 2074 7970 6573 2074   - Added types t
-00001770: 6f20 636f 7265 2063 6c61 7373 6573 2074  o core classes t
-00001780: 6f20 6d61 6b65 2063 7573 746f 6d69 7a61  o make customiza
-00001790: 7469 6f6e 2065 6173 6965 720d 0a20 2020  tion easier..   
-000017a0: 202d 2046 6978 6564 2062 616b 6b65 736d   - Fixed bakkesm
-000017b0: 6f64 2062 7567 0d0a 2020 2020 2222 222c  od bug..    """,
-000017c0: 0d0a 2020 2020 2730 2e31 2e31 273a 2022  ..    '0.1.1': "
-000017d0: 2222 0d0a 2020 2020 4164 6465 6420 6d69  ""..    Added mi
-000017e0: 7373 696e 6720 7363 6970 7920 6465 7065  ssing scipy depe
-000017f0: 6e64 656e 6379 0d0a 2020 2020 2222 222c  ndency..    """,
-00001800: 0d0a 2020 2020 2730 2e31 2e30 273a 2022  ..    '0.1.0': "
-00001810: 2222 0d0a 2020 2020 496e 6974 6961 6c20  ""..    Initial 
-00001820: 5265 6c65 6173 650d 0a20 2020 2022 2222  Release..    """
-00001830: 0d0a 7d0d 0a                             ..}..
+00000010: 2732 2e30 2e30 2d72 6327 0d0a 0d0a 0d0a  '2.0.0-rc'......
+00000020: 2320 544f 444f 2063 6f6e 7375 6d65 2073  # TODO consume s
+00000030: 7562 7061 636b 6167 6573 2069 6e73 7465  ubpackages inste
+00000040: 6164 3f0d 0a64 6566 2067 6574 5f63 7572  ad?..def get_cur
+00000050: 7265 6e74 5f72 656c 6561 7365 5f6e 6f74  rent_release_not
+00000060: 6573 2829 3a0d 0a20 2020 2069 6620 5f5f  es():..    if __
+00000070: 7665 7273 696f 6e5f 5f20 696e 2072 656c  version__ in rel
+00000080: 6561 7365 5f6e 6f74 6573 3a0d 0a20 2020  ease_notes:..   
+00000090: 2020 2020 2072 6574 7572 6e20 7265 6c65       return rele
+000000a0: 6173 655f 6e6f 7465 735b 5f5f 7665 7273  ase_notes[__vers
+000000b0: 696f 6e5f 5f5d 0d0a 2020 2020 7265 7475  ion__]..    retu
+000000c0: 726e 2027 270d 0a0d 0a0d 0a64 6566 2070  rn ''......def p
+000000d0: 7269 6e74 5f63 7572 7265 6e74 5f72 656c  rint_current_rel
+000000e0: 6561 7365 5f6e 6f74 6573 2829 3a0d 0a20  ease_notes():.. 
+000000f0: 2020 2070 7269 6e74 2866 2256 6572 7369     print(f"Versi
+00000100: 6f6e 207b 5f5f 7665 7273 696f 6e5f 5f7d  on {__version__}
+00000110: 2229 0d0a 2020 2020 7072 696e 7428 6765  ")..    print(ge
+00000120: 745f 6375 7272 656e 745f 7265 6c65 6173  t_current_releas
+00000130: 655f 6e6f 7465 7328 2929 0d0a 2020 2020  e_notes())..    
+00000140: 7072 696e 7428 2222 290d 0a0d 0a0d 0a72  print("")......r
+00000150: 656c 6561 7365 5f6e 6f74 6573 203d 207b  elease_notes = {
+00000160: 0d0a 2020 2020 2732 2e30 2e30 2d72 6327  ..    '2.0.0-rc'
+00000170: 3a0d 0a20 2020 2022 2222 0d0a 2020 2020  :..    """..    
+00000180: 4150 4920 6368 616e 6765 733a 0d0a 2020  API changes:..  
+00000190: 2020 2020 2020 2d20 4164 6465 6420 5368        - Added Sh
+000001a0: 6172 6564 496e 666f 5072 6f76 6964 6572  aredInfoProvider
+000001b0: 2041 5049 0d0a 2020 2020 2020 2020 2d20   API..        - 
+000001c0: 446f 6e65 436f 6e64 6974 696f 6e73 2061  DoneConditions a
+000001d0: 7265 206e 6f77 206f 7074 696f 6e61 6c0d  re now optional.
+000001e0: 0a20 2020 2020 2020 202d 204e 6f77 2065  .        - Now e
+000001f0: 7665 7279 2063 6f6e 6669 6720 6f62 6a65  very config obje
+00000200: 6374 2061 6c73 6f20 7265 6365 6976 6573  ct also receives
+00000210: 2074 6865 2041 6765 6e74 4944 206c 6973   the AgentID lis
+00000220: 7420 6475 7269 6e67 2072 6573 6574 0d0a  t during reset..
+00000230: 2020 2020 2020 2020 2d20 4f62 7342 7569          - ObsBui
+00000240: 6c64 6572 2061 6e64 2041 6374 696f 6e50  lder and ActionP
+00000250: 6172 7365 7220 6e6f 7720 6861 7665 2075  arser now have u
+00000260: 6e69 7175 6520 7479 7065 7320 666f 7220  nique types for 
+00000270: 7468 6569 7220 5370 6163 6554 7970 6573  their SpaceTypes
+00000280: 0d0a 2020 2020 526f 636b 6574 204c 6561  ..    Rocket Lea
+00000290: 6775 6520 6368 616e 6765 733a 0d0a 2020  gue changes:..  
+000002a0: 2020 2020 2020 2d20 5570 6461 7465 6420        - Updated 
+000002b0: 526f 636b 6574 5369 6d20 616e 6420 524c  RocketSim and RL
+000002c0: 5669 7365 7220 6465 7065 6e64 656e 6369  Viser dependenci
+000002d0: 6573 205b 5669 7278 5d0d 0a20 2020 2020  es [Virx]..     
+000002e0: 2020 202d 2041 6464 6564 2042 616c 6c20     - Added Ball 
+000002f0: 526f 744d 7478 2074 6f20 526f 636b 6574  RotMtx to Rocket
+00000300: 5369 6d20 656e 6769 6e65 2061 6e64 2052  Sim engine and R
+00000310: 4c56 6973 6572 2072 656e 6465 7265 7220  LViser renderer 
+00000320: 5b56 6972 785d 0d0a 2020 2020 2020 2020  [Virx]..        
+00000330: 2d20 4669 7865 6420 6275 6d70 2076 6963  - Fixed bump vic
+00000340: 7469 6d20 4944 2069 6e20 526f 636b 6574  tim ID in Rocket
+00000350: 5369 6d20 656e 6769 6e65 205b 4c61 6d70  Sim engine [Lamp
+00000360: 5d0d 0a20 2020 2020 2020 202d 2041 6464  ]..        - Add
+00000370: 6564 206d 6f72 6520 7573 6566 756c 2063  ed more useful c
+00000380: 6f6e 7374 616e 7473 2074 6f20 636f 6d6d  onstants to comm
+00000390: 6f6e 5f76 616c 7565 730d 0a20 2020 2020  on_values..     
+000003a0: 2020 202d 2052 656d 6f76 6564 2052 4c56     - Removed RLV
+000003b0: 6973 6572 2064 6570 656e 6465 6e63 7920  iser dependency 
+000003c0: 6672 6f6d 2073 696d 2069 6e73 7461 6c6c  from sim install
+000003d0: 0d0a 2020 2020 2020 2020 2d20 496d 7072  ..        - Impr
+000003e0: 6f76 6564 2052 6570 6561 7441 6374 696f  oved RepeatActio
+000003f0: 6e2c 2069 7420 6e6f 7720 646f 6573 6e27  n, it now doesn'
+00000400: 7420 6578 7065 6374 2079 6f75 7220 4163  t expect your Ac
+00000410: 7469 6f6e 5061 7273 6572 2074 6f20 6861  tionParser to ha
+00000420: 6e64 6c65 206d 756c 7469 706c 6520 7469  ndle multiple ti
+00000430: 636b 730d 0a20 2020 2020 2020 202d 2049  cks..        - I
+00000440: 6d70 726f 7665 6420 6465 6661 756c 7420  mproved default 
+00000450: 4f62 7353 7061 6365 2061 6e64 2041 6374  ObsSpace and Act
+00000460: 696f 6e53 7061 6365 2064 6566 696e 6974  ionSpace definit
+00000470: 696f 6e73 0d0a 2020 2020 2222 222c 0d0a  ions..    """,..
+00000480: 2020 2020 2732 2e30 2e30 2d61 6c70 6861      '2.0.0-alpha
+00000490: 2d33 273a 0d0a 2020 2020 2222 220d 0a20  -3':..    """.. 
+000004a0: 2020 202d 2054 6869 7320 7665 7273 696f     - This versio
+000004b0: 6e20 636f 6e74 6169 6e73 206e 756d 6572  n contains numer
+000004c0: 6f75 7320 756e 7465 7374 6564 2061 6e64  ous untested and
+000004d0: 2062 7265 616b 696e 6720 6368 616e 6765   breaking change
+000004e0: 732e 2052 756e 2061 7420 796f 7572 206f  s. Run at your o
+000004f0: 776e 2072 6973 6b2e 0d0a 2020 2020 2d20  wn risk...    - 
+00000500: 4669 7865 6420 5079 7468 6f6e 203c 332e  Fixed Python <3.
+00000510: 3920 696e 7374 616c 6c0d 0a20 2020 2041  9 install..    A
+00000520: 5049 2063 6861 6e67 6573 3a0d 0a20 2020  PI changes:..   
+00000530: 2020 2020 202d 2041 6464 6564 2073 6861       - Added sha
+00000540: 7265 645f 696e 666f 2070 6172 616d 2074  red_info param t
+00000550: 6f20 5472 616e 7369 7469 6f6e 456e 6769  o TransitionEngi
+00000560: 6e65 2061 6e64 2052 656e 6465 7265 720d  ne and Renderer.
+00000570: 0a20 2020 2020 2020 202d 204d 6f76 6520  .        - Move 
+00000580: 726c 6779 6d2e 6170 692e 656e 6769 6e65  rlgym.api.engine
+00000590: 2074 6f20 726c 6779 6d2e 6170 692e 636f   to rlgym.api.co
+000005a0: 6e66 6967 0d0a 2020 2020 526f 636b 6574  nfig..    Rocket
+000005b0: 4c65 6167 7565 2063 6861 6e67 6573 3a0d  League changes:.
+000005c0: 0a20 2020 2020 2020 202d 2055 7064 6174  .        - Updat
+000005d0: 6520 696d 706f 7274 7320 746f 2072 6c67  e imports to rlg
+000005e0: 796d 2e61 7069 0d0a 2020 2020 2020 2020  ym.api..        
+000005f0: 2d20 5265 6e61 6d65 2072 6c67 796d 2e72  - Rename rlgym.r
+00000600: 6f63 6b65 745f 6c65 6167 7565 2e65 6e67  ocket_league.eng
+00000610: 696e 6520 746f 2072 6c67 796d 2e72 6f63  ine to rlgym.roc
+00000620: 6b65 745f 6c65 6167 7565 2e61 7069 0d0a  ket_league.api..
+00000630: 2020 2020 2020 2020 2d20 496d 7072 6f76          - Improv
+00000640: 6520 6578 706f 7274 7320 736f 2069 6d70  e exports so imp
+00000650: 6f72 7473 2061 7265 206d 6f72 6520 636f  orts are more co
+00000660: 6e73 6f6c 6964 6174 6564 0d0a 2020 2020  nsolidated..    
+00000670: 2222 222c 0d0a 2020 2020 2732 2e30 2e30  """,..    '2.0.0
+00000680: 2d61 6c70 6861 2d32 273a 0d0a 2020 2020  -alpha-2':..    
+00000690: 2222 220d 0a20 2020 202d 2054 6869 7320  """..    - This 
+000006a0: 7665 7273 696f 6e20 636f 6e74 6169 6e73  version contains
+000006b0: 206e 756d 6572 6f75 7320 756e 7465 7374   numerous untest
+000006c0: 6564 2061 6e64 2070 6f74 656e 7469 616c  ed and potential
+000006d0: 6c79 2062 7265 616b 696e 6720 6368 616e  ly breaking chan
+000006e0: 6765 732e 2052 756e 2061 7420 796f 7572  ges. Run at your
+000006f0: 206f 776e 2072 6973 6b2e 0d0a 2020 2020   own risk...    
+00000700: 2d20 4669 7865 6420 726c 7669 7365 722d  - Fixed rlviser-
+00000710: 7079 2064 6570 656e 6465 6e63 7920 7665  py dependency ve
+00000720: 7273 696f 6e0d 0a20 2020 2022 2222 2c0d  rsion..    """,.
+00000730: 0a20 2020 2027 322e 302e 302d 616c 7068  .    '2.0.0-alph
+00000740: 612d 3127 3a0d 0a20 2020 2022 2222 0d0a  a-1':..    """..
+00000750: 2020 2020 2d20 5468 6973 2076 6572 7369      - This versi
+00000760: 6f6e 2063 6f6e 7461 696e 7320 6e75 6d65  on contains nume
+00000770: 726f 7573 2075 6e74 6573 7465 6420 616e  rous untested an
+00000780: 6420 706f 7465 6e74 6961 6c6c 7920 6272  d potentially br
+00000790: 6561 6b69 6e67 2063 6861 6e67 6573 2e20  eaking changes. 
+000007a0: 5275 6e20 6174 2079 6f75 7220 6f77 6e20  Run at your own 
+000007b0: 7269 736b 2e0d 0a20 2020 202d 204c 6966  risk...    - Lif
+000007c0: 7465 6420 5079 7468 6f6e 203c 332e 3130  ted Python <3.10
+000007d0: 2072 6573 7472 6963 7469 6f6e 0d0a 2020   restriction..  
+000007e0: 2020 2222 222c 0d0a 2020 2020 2732 2e30    """,..    '2.0
+000007f0: 2e30 2d61 6c70 6861 273a 0d0a 2020 2020  .0-alpha':..    
+00000800: 2222 220d 0a20 2020 202d 2054 6869 7320  """..    - This 
+00000810: 7665 7273 696f 6e20 636f 6e74 6169 6e73  version contains
+00000820: 206e 756d 6572 6f75 7320 756e 7465 7374   numerous untest
+00000830: 6564 2061 6e64 2070 6f74 656e 7469 616c  ed and potential
+00000840: 6c79 2062 7265 616b 696e 6720 6368 616e  ly breaking chan
+00000850: 6765 732e 2052 756e 2061 7420 796f 7572  ges. Run at your
+00000860: 206f 776e 2072 6973 6b2e 0d0a 2020 2020   own risk...    
+00000870: 2222 222c 0d0a 2020 2020 2731 2e32 2e32  """,..    '1.2.2
+00000880: 273a 0d0a 2020 2020 2222 220d 0a20 2020  ':..    """..   
+00000890: 202d 2046 6978 6564 206d 6178 2070 7974   - Fixed max pyt
+000008a0: 686f 6e20 7665 7273 696f 6e0d 0a20 2020  hon version..   
+000008b0: 2022 2222 2c0d 0a20 2020 2027 312e 322e   """,..    '1.2.
+000008c0: 3127 3a0d 0a20 2020 2022 2222 0d0a 2020  1':..    """..  
+000008d0: 2020 2d20 4669 7865 6420 6570 6963 2076    - Fixed epic v
+000008e0: 6572 7369 6f6e 2063 7261 7368 696e 6720  ersion crashing 
+000008f0: 696e 7374 616e 746c 7920 2d20 4261 6b6b  instantly - Bakk
+00000900: 6573 0d0a 2020 2020 2d20 4164 6465 6420  es..    - Added 
+00000910: 6d61 7820 7079 7468 6f6e 2076 6572 7369  max python versi
+00000920: 6f6e 0d0a 2020 2020 2d20 4164 6465 6420  on..    - Added 
+00000930: 4163 7469 6f6e 5061 7273 6572 2074 6f20  ActionParser to 
+00000940: 7574 696c 7320 7375 626d 6f64 756c 650d  utils submodule.
+00000950: 0a20 2020 202d 2055 7064 6174 6564 2064  .    - Updated d
+00000960: 6566 6175 6c74 2072 6577 6172 642c 2069  efault reward, i
+00000970: 7420 6e6f 7720 6d69 6e69 6d69 7a65 7320  t now minimizes 
+00000980: 6c69 6e65 6172 2076 656c 6f63 6974 7920  linear velocity 
+00000990: 696e 7374 6561 6420 6f66 2061 6e67 756c  instead of angul
+000009a0: 6172 0d0a 2020 2020 2d20 5249 5020 5268  ar..    - RIP Rh
+000009b0: 6f62 6f74 4f62 730d 0a20 2020 2022 2222  obotObs..    """
+000009c0: 2c0d 0a20 2020 2027 312e 322e 3027 3a20  ,..    '1.2.0': 
+000009d0: 2222 220d 0a20 2020 202d 2044 6570 7265  """..    - Depre
+000009e0: 6361 7465 6420 7365 6c66 5f70 6c61 7920  cated self_play 
+000009f0: 666c 6167 2c20 706c 6179 696e 6720 6167  flag, playing ag
+00000a00: 6169 6e73 7420 5073 796f 6e69 7820 6167  ainst Psyonix ag
+00000a10: 656e 7473 2069 7320 6e6f 206c 6f6e 6765  ents is no longe
+00000a20: 7220 7375 7070 6f72 7465 640d 0a20 2020  r supported..   
+00000a30: 202d 2041 6464 6564 2068 6173 5f6a 756d   - Added has_jum
+00000a40: 7020 746f 2050 6c61 7965 7244 6174 612c  p to PlayerData,
+00000a50: 2077 6869 6368 2069 7320 7573 6566 756c   which is useful
+00000a60: 2074 6f20 6465 7465 6374 2077 6865 6e20   to detect when 
+00000a70: 6120 666c 6970 2077 6f6e 2774 2072 756e  a flip won't run
+00000a80: 206f 7574 0d0a 2020 2020 2d20 4164 6465   out..    - Adde
+00000a90: 6420 7072 655f 7374 6570 2829 2066 756e  d pre_step() fun
+00000aa0: 6374 696f 6e20 746f 204f 6273 4275 696c  ction to ObsBuil
+00000ab0: 6465 7220 616e 6420 5265 7761 7264 4675  der and RewardFu
+00000ac0: 6e63 7469 6f6e 2c20 7573 6566 756c 2066  nction, useful f
+00000ad0: 6f72 2070 7265 2d63 616c 6375 6c61 7469  or pre-calculati
+00000ae0: 6e67 2073 7475 6666 2065 6163 6820 7374  ng stuff each st
+00000af0: 6570 0d0a 2020 2020 2d20 4164 6465 6420  ep..    - Added 
+00000b00: 7375 7070 6f72 7420 666f 7220 6368 616e  support for chan
+00000b10: 6769 6e67 2067 616d 656d 6f64 6520 7769  ging gamemode wi
+00000b20: 7468 6f75 7420 7265 7374 6172 7469 6e67  thout restarting
+00000b30: 2052 4c47 796d 2c20 7365 6520 5374 6174   RLGym, see Stat
+00000b40: 6553 6574 7465 722e 6275 696c 645f 7772  eSetter.build_wr
+00000b50: 6170 7065 7228 290d 0a20 2020 202d 2041  apper()..    - A
+00000b60: 6464 6564 2067 7261 7669 7479 2061 6e64  dded gravity and
+00000b70: 2062 6f6f 7374 5f63 6f6e 7375 6d70 7469   boost_consumpti
+00000b80: 6f6e 2063 6f6e 6669 6775 7261 7469 6f6e  on configuration
+00000b90: 2074 6f20 726c 6779 6d2e 6d61 6b65 2829   to rlgym.make()
+00000ba0: 0d0a 2020 2020 2d20 4164 6465 6420 7570  ..    - Added up
+00000bb0: 6461 7465 5f73 6574 7469 6e67 7328 2920  date_settings() 
+00000bc0: 6d65 7468 6f64 2074 6f20 6779 6d2c 2066  method to gym, f
+00000bd0: 6f72 2075 7064 6174 696e 6720 736f 6d65  or updating some
+00000be0: 2070 6172 7473 206f 6620 7468 6520 636f   parts of the co
+00000bf0: 6e66 6967 2077 6974 686f 7574 2072 6573  nfig without res
+00000c00: 7461 7274 696e 670d 0a20 2020 202d 2041  tarting..    - A
+00000c10: 6464 6564 2067 6574 5f6f 6273 5f73 7061  dded get_obs_spa
+00000c20: 6365 2829 2074 6f20 4f62 7342 7569 6c64  ce() to ObsBuild
+00000c30: 6572 2c20 656e 6162 6c65 7320 6f76 6572  er, enables over
+00000c40: 7269 6469 6e67 2052 4c47 796d 2773 2061  riding RLGym's a
+00000c50: 7574 6f6d 6174 6963 206f 6273 2073 697a  utomatic obs siz
+00000c60: 6520 6465 7465 6374 696f 6e0d 0a20 2020  e detection..   
+00000c70: 202d 2041 6464 6564 2072 6169 7365 5f6f   - Added raise_o
+00000c80: 6e5f 6372 6173 6820 6f70 7469 6f6e 2074  n_crash option t
+00000c90: 6f20 726c 6779 6d2e 6d61 6b65 2829 0d0a  o rlgym.make()..
+00000ca0: 2020 2020 2d20 4164 6465 6420 6175 746f      - Added auto
+00000cb0: 5f6d 696e 696d 697a 6520 6f70 7469 6f6e  _minimize option
+00000cc0: 2074 6f20 726c 6779 6d2e 6d61 6b65 2829   to rlgym.make()
+00000cd0: 0d0a 2020 2020 2d20 4164 6465 6420 626f  ..    - Added bo
+00000ce0: 6f73 7420 7069 636b 7570 7320 746f 2065  ost pickups to e
+00000cf0: 7665 6e74 2072 6577 6172 6420 2d20 7961  vent reward - ya
+00000d00: 6461 7261 660d 0a20 2020 202d 2046 6978  daraf..    - Fix
+00000d10: 6564 2063 7573 746f 6d20 6269 6e20 7375  ed custom bin su
+00000d20: 7070 6f72 7420 696e 2044 6973 6372 6574  pport in Discret
+00000d30: 6541 6374 696f 6e20 2d20 4b61 6979 6f74  eAction - Kaiyot
+00000d40: 6563 680d 0a20 2020 202d 2046 6978 6564  ech..    - Fixed
+00000d50: 2062 7567 2069 6e20 5665 6c6f 6369 7479   bug in Velocity
+00000d60: 4261 6c6c 546f 476f 616c 5265 7761 7264  BallToGoalReward
+00000d70: 2061 6e64 2056 656c 6f63 6974 7950 6c61   and VelocityPla
+00000d80: 7965 7254 6f42 616c 6c52 6577 6172 640d  yerToBallReward.
+00000d90: 0a20 2020 202d 2046 6978 6564 2050 6c61  .    - Fixed Pla
+00000da0: 7965 7244 6174 6120 7374 7269 6e67 2072  yerData string r
+00000db0: 6570 7265 7365 6e74 6174 696f 6e20 2d20  epresentation - 
+00000dc0: 4361 7272 6f74 0d0a 2020 2020 2222 222c  Carrot..    """,
+00000dd0: 0d0a 2020 2020 2731 2e31 2e30 273a 2022  ..    '1.1.0': "
+00000de0: 2222 0d0a 2020 2020 2d20 4164 6465 6420  ""..    - Added 
+00000df0: 4163 7469 6f6e 5061 7273 6572 732c 2077  ActionParsers, w
+00000e00: 6869 6368 2061 6c6c 6f77 2079 6f75 2074  hich allow you t
+00000e10: 6f20 6465 6669 6e65 2063 7573 746f 6d20  o define custom 
+00000e20: 6163 7469 6f6e 2073 7061 6365 7320 2d20  action spaces - 
+00000e30: 4c6f 6c61 6170 6b33 0d0a 2020 2020 2d20  Lolaapk3..    - 
+00000e40: 4669 7865 6420 7175 6174 6572 6e69 6f6e  Fixed quaternion
+00000e50: 2074 6f20 6575 6c65 7220 616e 676c 6520   to euler angle 
+00000e60: 636f 6e76 6572 7369 6f6e 202d 2044 6172  conversion - Dar
+00000e70: 7865 616c 0d0a 2020 2020 2d20 496d 7072  xeal..    - Impr
+00000e80: 6f76 6564 2044 6566 6175 6c74 4f62 732c  oved DefaultObs,
+00000e90: 2069 7420 6e6f 7720 6861 7320 616c 6c20   it now has all 
+00000ea0: 7468 6520 7374 6174 6520 696e 666f 726d  the state inform
+00000eb0: 6174 696f 6e0d 0a20 2020 202d 2041 6464  ation..    - Add
+00000ec0: 6564 206f 7074 696f 6e61 6c20 7061 7261  ed optional para
+00000ed0: 6d65 7465 7220 746f 2072 6574 7572 6e20  meter to return 
+00000ee0: 696e 6974 6961 6c20 696e 666f 206f 626a  initial info obj
+00000ef0: 6563 7420 6f6e 2065 6e76 2e72 6573 6574  ect on env.reset
+00000f00: 2829 0d0a 2020 2020 2d20 4669 7865 6420  ()..    - Fixed 
+00000f10: 7261 6e64 5f76 6563 3320 736f 2074 6865  rand_vec3 so the
+00000f20: 206d 6167 6e69 7475 6465 2069 7320 6163   magnitude is ac
+00000f30: 7475 616c 6c79 2072 616e 646f 6d0d 0a20  tually random.. 
+00000f40: 2020 2022 2222 2c0d 0a20 2020 2027 312e     """,..    '1.
+00000f50: 302e 3227 3a20 2222 220d 0a20 2020 202d  0.2': """..    -
+00000f60: 2046 6978 6564 2073 7461 7465 2073 6574   Fixed state set
+00000f70: 7469 6e67 2069 7373 7565 7320 2862 6f6f  ting issues (boo
+00000f80: 7374 2073 6574 7469 6e67 2061 6e64 2070  st setting and p
+00000f90: 7265 6369 7369 6f6e 290d 0a20 2020 2022  recision)..    "
+00000fa0: 2222 2c0d 0a20 2020 2027 312e 302e 3127  "",..    '1.0.1'
+00000fb0: 3a20 2222 220d 0a20 2020 202d 204d 696e  : """..    - Min
+00000fc0: 6f72 2066 6978 2066 6f72 2052 616e 646f  or fix for Rando
+00000fd0: 6d53 7461 7465 0d0a 2020 2020 2222 222c  mState..    """,
+00000fe0: 0d0a 2020 2020 2731 2e30 2e30 273a 2022  ..    '1.0.0': "
+00000ff0: 2222 0d0a 2020 2020 2d20 4164 6465 6420  ""..    - Added 
+00001000: 7374 6174 6520 7365 7474 696e 672c 2079  state setting, y
+00001010: 6f75 2063 616e 206e 6f77 2073 7065 6369  ou can now speci
+00001020: 6679 2074 6865 2069 6e69 7469 616c 2073  fy the initial s
+00001030: 7461 7465 206f 6620 6570 6973 6f64 6573  tate of episodes
+00001040: 2076 6961 2061 2053 7461 7465 5365 7474   via a StateSett
+00001050: 6572 206f 626a 6563 7420 2d20 6169 5461  er object - aiTa
+00001060: 6e0d 0a20 2020 202d 2041 6464 6564 206c  n..    - Added l
+00001070: 6175 6e63 685f 7072 6566 6572 656e 6365  aunch_preference
+00001080: 2074 6f20 6d61 6b65 2829 0d0a 2020 2020   to make()..    
+00001090: 2d20 4669 7865 6420 4570 6963 206c 6175  - Fixed Epic lau
+000010a0: 6e63 6820 6275 6720 696e 7472 6f64 7563  nch bug introduc
+000010b0: 6564 2077 6974 6820 7468 6520 5365 6173  ed with the Seas
+000010c0: 6f6e 2034 2075 7064 6174 650d 0a20 2020  on 4 update..   
+000010d0: 202d 2043 6f6d 6d75 6e69 6361 7469 6f6e   - Communication
+000010e0: 2063 6f64 6520 7265 6661 6374 6f72 6564   code refactored
+000010f0: 2074 6f20 696e 6372 6561 7365 2070 6572   to increase per
+00001100: 666f 726d 616e 6365 2077 6974 6820 6c6f  formance with lo
+00001110: 7720 7469 636b 5f73 6b69 700d 0a20 2020  w tick_skip..   
+00001120: 202d 2046 6978 6564 2062 6f6f 7374 2070   - Fixed boost p
+00001130: 6164 2072 6573 6574 2062 7567 206f 6e20  ad reset bug on 
+00001140: 6570 6973 6f64 6520 7265 7365 740d 0a20  episode reset.. 
+00001150: 2020 202d 2041 6464 6564 2064 6574 6563     - Added detec
+00001160: 7469 6f6e 206d 6563 6861 6e69 736d 2066  tion mechanism f
+00001170: 6f72 2067 686f 7374 2062 616c 6c20 6275  or ghost ball bu
+00001180: 670d 0a20 2020 202d 2044 6563 7265 6173  g..    - Decreas
+00001190: 6564 2072 6571 7569 7265 6420 6163 6365  ed required acce
+000011a0: 7373 2072 6967 6874 7320 6279 2074 6865  ss rights by the
+000011b0: 204d 756c 7469 496e 6a65 6374 6f72 0d0a   MultiInjector..
+000011c0: 2020 2020 2222 222c 0d0a 2020 2020 2730      """,..    '0
+000011d0: 2e36 2e30 273a 2022 2222 0d0a 2020 2020  .6.0': """..    
+000011e0: 2d20 4d6f 7665 6420 7772 6170 7065 7273  - Moved wrappers
+000011f0: 2061 6e64 2072 6570 6c61 7920 636f 6e76   and replay conv
+00001200: 6572 7465 7220 746f 2072 6c67 796d 2d74  erter to rlgym-t
+00001210: 6f6f 6c73 2070 6163 6b61 6765 0d0a 2020  ools package..  
+00001220: 2020 2d20 4164 6465 6420 7468 6520 6f70    - Added the op
+00001230: 7469 6f6e 616c 2061 6269 6c69 7479 2074  tional ability t
+00001240: 6f20 666f 7263 6566 756c 6c79 2070 6167  o forcefully pag
+00001250: 6520 7468 6520 7370 6177 6e65 6420 526f  e the spawned Ro
+00001260: 636b 6574 204c 6561 6775 6520 696e 7374  cket League inst
+00001270: 616e 6365 7320 7570 6f6e 2063 7265 6174  ances upon creat
+00001280: 696f 6e20 2d20 3431 3663 3631 3665 0d0a  ion - 416c616e..
+00001290: 2020 2020 2d20 5468 6520 7061 7468 5f74      - The path_t
+000012a0: 6f5f 726c 2070 6172 616d 2069 7320 6e6f  o_rl param is no
+000012b0: 206c 6f6e 6765 7220 7265 7175 6972 6564   longer required
+000012c0: 2066 6f72 2075 7365 5f69 6e6a 6563 746f   for use_injecto
+000012d0: 720d 0a20 2020 2022 2222 2c0d 0a20 2020  r..    """,..   
+000012e0: 2027 302e 352e 3027 3a20 2222 220d 0a20   '0.5.0': """.. 
+000012f0: 2020 202d 2052 656d 6f76 6564 2073 7472     - Removed str
+00001300: 696e 6720 6261 7365 6420 636f 6e66 6967  ing based config
+00001310: 7572 6174 696f 6e73 2069 6e20 726c 6779  urations in rlgy
+00001320: 6d2e 6d61 6b65 2829 2c20 6576 6572 7974  m.make(), everyt
+00001330: 6869 6e67 2069 7320 7061 7373 6564 2062  hing is passed b
+00001340: 7920 6b77 6172 6773 206e 6f77 202d 2053  y kwargs now - S
+00001350: 6f72 656e 0d0a 2020 2020 2d20 4164 6465  oren..    - Adde
+00001360: 6420 5374 6162 6c65 4261 7365 6c69 6e65  d StableBaseline
+00001370: 7333 2063 6f6d 7061 7469 6269 6c69 7479  s3 compatibility
+00001380: 202d 2052 6f6c 760d 0a20 2020 202d 2052   - Rolv..    - R
+00001390: 6566 6163 746f 7265 6420 616e 6420 6578  efactored and ex
+000013a0: 7061 6e64 6564 2072 6577 6172 6420 6675  panded reward fu
+000013b0: 6e63 7469 6f6e 7320 2d20 526f 6c76 0d0a  nctions - Rolv..
+000013c0: 2020 2020 2d20 4164 6465 6420 7265 706c      - Added repl
+000013d0: 6179 2063 6f6e 7665 7274 6572 202d 2052  ay converter - R
+000013e0: 6f6c 760d 0a20 2020 202d 2046 6978 6564  olv..    - Fixed
+000013f0: 2054 6f75 6368 4261 6c6c 5265 7761 7264   TouchBallReward
+00001400: 2062 7567 202d 204b 6576 696e 0d0a 0d0a   bug - Kevin....
+00001410: 2020 2020 4e4f 5445 3a20 536f 6d65 206f      NOTE: Some o
+00001420: 6620 7468 6573 6520 6e65 7720 746f 6f6c  f these new tool
+00001430: 7320 2877 7261 7070 6572 732c 2072 6570  s (wrappers, rep
+00001440: 6c61 7920 636f 6e76 6572 7465 722c 2065  lay converter, e
+00001450: 7463 2920 7769 6c6c 2062 6520 6d6f 7665  tc) will be move
+00001460: 6420 746f 2061 2064 6966 6665 7265 6e74  d to a different
+00001470: 2070 6163 6b61 6765 2069 6e20 7468 6520   package in the 
+00001480: 6e65 7874 2072 656c 6561 7365 0d0a 2020  next release..  
+00001490: 2020 2222 222c 0d0a 2020 2020 2730 2e34    """,..    '0.4
+000014a0: 2e31 273a 2022 2222 0d0a 2020 2020 2d20  .1': """..    - 
+000014b0: 5570 6461 7465 6420 6575 6c65 7220 616e  Updated euler an
+000014c0: 676c 6573 2074 6f20 6d61 7463 6820 726c  gles to match rl
+000014d0: 626f 7420 5b70 6974 6368 2c20 7961 772c  bot [pitch, yaw,
+000014e0: 2072 6f6c 6c5d 2061 6e64 2061 6464 6564   roll] and added
+000014f0: 2061 6363 6573 736f 7220 6675 6e63 7469   accessor functi
+00001500: 6f6e 730d 0a20 2020 202d 2042 7567 6669  ons..    - Bugfi
+00001510: 783a 2070 6c61 7965 722e 6973 5f61 6c69  x: player.is_ali
+00001520: 7665 2072 656e 616d 6564 2074 6f20 6973  ve renamed to is
+00001530: 5f64 656d 6f65 640d 0a20 2020 202d 2041  _demoed..    - A
+00001540: 6464 6564 2063 6f6d 6d6f 6e20 7265 7761  dded common rewa
+00001550: 7264 7320 2d20 526f 6c76 0d0a 2020 2020  rds - Rolv..    
+00001560: 2d20 4164 6465 6420 6120 7265 7761 7264  - Added a reward
+00001570: 2063 6f6d 6269 6e65 7220 2d20 4368 6169   combiner - Chai
+00001580: 6e73 6f0d 0a20 2020 202d 2041 6464 6564  nso..    - Added
+00001590: 206d 6973 7369 6e67 206b 6963 6b6f 6666   missing kickoff
+000015a0: 2073 7061 776e 0d0a 2020 2020 2d20 4669   spawn..    - Fi
+000015b0: 7865 6420 3276 3220 616e 6420 3376 3320  xed 2v2 and 3v3 
+000015c0: 6163 7469 6f6e 2064 656c 6976 6572 790d  action delivery.
+000015d0: 0a20 2020 202d 2046 6978 6564 2069 7373  .    - Fixed iss
+000015e0: 7565 2069 6e20 3276 3220 616e 6420 3376  ue in 2v2 and 3v
+000015f0: 3320 7768 6572 6520 626c 7565 2062 6f74  3 where blue bot
+00001600: 7320 776f 756c 6420 6469 7361 7070 6561  s would disappea
+00001610: 7220 6f76 6572 2074 696d 650d 0a20 2020  r over time..   
+00001620: 202d 2041 6464 6564 206d 756c 7469 2069   - Added multi i
+00001630: 6e6a 6563 746f 720d 0a20 2020 2022 2222  njector..    """
+00001640: 2c0d 0a20 2020 2027 302e 342e 3027 3a20  ,..    '0.4.0': 
+00001650: 2222 220d 0a20 2020 202d 204d 616a 6f72  """..    - Major
+00001660: 2041 5049 2072 6566 6163 746f 720d 0a20   API refactor.. 
+00001670: 2020 202d 2041 6464 6564 2062 6f6f 7374     - Added boost
+00001680: 7061 6420 626f 6f6c 6561 6e20 6172 7261  pad boolean arra
+00001690: 7920 746f 2047 616d 6553 7461 7465 0d0a  y to GameState..
+000016a0: 2020 2020 2d20 524c 4779 6d20 6973 206e      - RLGym is n
+000016b0: 6f77 2062 6173 656c 696e 6573 2063 6f6d  ow baselines com
+000016c0: 7061 7469 626c 650d 0a20 2020 202d 2041  patible..    - A
+000016d0: 6464 6564 2069 6d70 726f 7665 6420 4465  dded improved De
+000016e0: 6661 756c 7420 636f 6e66 6967 7572 6174  fault configurat
+000016f0: 696f 6e0d 0a20 2020 2022 2222 2c0d 0a20  ion..    """,.. 
+00001700: 2020 2027 302e 332e 3027 3a20 2222 220d     '0.3.0': """.
+00001710: 0a20 2020 202d 2050 6173 7320 696e 6974  .    - Pass init
+00001720: 6961 6c20 7374 6174 6520 746f 2065 6e76  ial state to env
+00001730: 2063 6f6d 706f 6e65 6e74 7320 6f6e 2067   components on g
+00001740: 796d 2e72 6573 6574 2829 0d0a 2020 2020  ym.reset()..    
+00001750: 2d20 5061 7373 2070 7265 7620 6163 7469  - Pass prev acti
+00001760: 6f6e 2074 6f20 7265 7761 7264 2066 6e0d  on to reward fn.
+00001770: 0a20 2020 202d 2069 6e66 6f20 7265 7475  .    - info retu
+00001780: 726e 6564 2066 726f 6d20 6779 6d2e 7374  rned from gym.st
+00001790: 6570 2829 2069 7320 6e6f 7720 6120 4469  ep() is now a Di
+000017a0: 6374 0d0a 2020 2020 2d20 4669 7865 6420  ct..    - Fixed 
+000017b0: 6f62 7320 7369 7a65 2062 7567 2069 6e20  obs size bug in 
+000017c0: 5268 6f62 6f74 4f62 730d 0a20 2020 2022  RhobotObs..    "
+000017d0: 2222 2c0d 0a20 2020 2027 302e 322e 3027  "",..    '0.2.0'
+000017e0: 3a20 2222 220d 0a20 2020 202d 2053 7769  : """..    - Swi
+000017f0: 7463 6865 6420 6672 6f6d 2063 7573 746f  tched from custo
+00001800: 6d5f 6172 6773 2064 6963 7420 746f 206b  m_args dict to k
+00001810: 6579 776f 7264 2061 7267 7320 696e 2072  eyword args in r
+00001820: 6c67 796d 2e6d 616b 6528 290d 0a20 2020  lgym.make()..   
+00001830: 2022 2222 2c0d 0a20 2020 2027 302e 312e   """,..    '0.1.
+00001840: 3427 3a20 2222 220d 0a20 2020 202d 2047  4': """..    - G
+00001850: 796d 206e 6f77 2069 6e68 6572 6974 7320  ym now inherits 
+00001860: 6f70 656e 6169 2e67 796d 2e45 6e76 202d  openai.gym.Env -
+00001870: 2043 6861 696e 736f 0d0a 2020 2020 2d20   Chainso..    - 
+00001880: 4669 7865 6420 6275 6720 7768 6572 6520  Fixed bug where 
+00001890: 726c 6779 6d20 6372 6173 6865 6420 7472  rlgym crashed tr
+000018a0: 7969 6e67 2074 6f20 7061 7273 6520 7468  ying to parse th
+000018b0: 6520 7374 6174 6520 7374 7269 6e67 2069  e state string i
+000018c0: 6e20 736f 6d65 2073 6365 6e61 7269 6f73  n some scenarios
+000018d0: 0d0a 2020 2020 2222 222c 0d0a 2020 2020  ..    """,..    
+000018e0: 2730 2e31 2e33 273a 2022 2222 0d0a 2020  '0.1.3': """..  
+000018f0: 2020 2d20 5265 6e61 6d65 6420 5068 7973    - Renamed Phys
+00001900: 6963 734f 626a 6563 742e 6f72 6965 6e74  icsObject.orient
+00001910: 6174 696f 6e20 746f 2065 756c 6572 5f61  ation to euler_a
+00001920: 6e67 6c65 730d 0a20 2020 202d 2065 756c  ngles..    - eul
+00001930: 6572 5f61 6e67 6c65 7320 6973 206e 6f77  er_angles is now
+00001940: 2061 2066 756e 6374 696f 6e20 736f 2074   a function so t
+00001950: 6865 7920 6172 656e 2774 2063 616c 6375  hey aren't calcu
+00001960: 6c61 7465 6420 6966 206e 6f74 206e 6565  lated if not nee
+00001970: 6465 640d 0a20 2020 202d 2041 6464 6564  ded..    - Added
+00001980: 2072 6f74 6174 696f 6e5f 6d74 782c 2066   rotation_mtx, f
+00001990: 6f72 7761 7264 2c20 7269 6768 7420 616e  orward, right an
+000019a0: 6420 7570 2076 6563 746f 7273 2074 6f20  d up vectors to 
+000019b0: 5068 7973 6963 734f 626a 6563 7420 286f  PhysicsObject (o
+000019c0: 6e6c 7920 7573 6162 6c65 2066 6f72 2074  nly usable for t
+000019d0: 6865 2063 6172 290d 0a20 2020 202d 2052  he car)..    - R
+000019e0: 656d 6f76 6564 2063 6f6e 7665 7273 696f  emoved conversio
+000019f0: 6e20 746f 206e 7020 6172 7261 7920 666f  n to np array fo
+00001a00: 7220 7265 7761 7264 7320 616e 6420 6f62  r rewards and ob
+00001a10: 7365 7276 6174 696f 6e73 0d0a 2020 2020  servations..    
+00001a20: 2d20 4669 7865 6420 6275 6720 696e 2052  - Fixed bug in R
+00001a30: 686f 626f 744f 6273 0d0a 2020 2020 2222  hobotObs..    ""
+00001a40: 222c 0d0a 2020 2020 2730 2e31 2e32 273a  ",..    '0.1.2':
+00001a50: 2022 2222 0d0a 2020 2020 2d20 4f62 7320   """..    - Obs 
+00001a60: 6172 6520 6e6f 7720 6e75 6d70 7920 6172  are now numpy ar
+00001a70: 7261 7973 0d0a 2020 2020 2d20 4164 6465  rays..    - Adde
+00001a80: 6420 7479 7065 7320 746f 2063 6f72 6520  d types to core 
+00001a90: 636c 6173 7365 7320 746f 206d 616b 6520  classes to make 
+00001aa0: 6375 7374 6f6d 697a 6174 696f 6e20 6561  customization ea
+00001ab0: 7369 6572 0d0a 2020 2020 2d20 4669 7865  sier..    - Fixe
+00001ac0: 6420 6261 6b6b 6573 6d6f 6420 6275 670d  d bakkesmod bug.
+00001ad0: 0a20 2020 2022 2222 2c0d 0a20 2020 2027  .    """,..    '
+00001ae0: 302e 312e 3127 3a20 2222 220d 0a20 2020  0.1.1': """..   
+00001af0: 2041 6464 6564 206d 6973 7369 6e67 2073   Added missing s
+00001b00: 6369 7079 2064 6570 656e 6465 6e63 790d  cipy dependency.
+00001b10: 0a20 2020 2022 2222 2c0d 0a20 2020 2027  .    """,..    '
+00001b20: 302e 312e 3027 3a20 2222 220d 0a20 2020  0.1.0': """..   
+00001b30: 2049 6e69 7469 616c 2052 656c 6561 7365   Initial Release
+00001b40: 0d0a 2020 2020 2222 220d 0a7d 0d0a       ..    """..}..
```

### Comparing `rlgym-2.0.0a3/rlgym.egg-info/PKG-INFO` & `rlgym-2.0.0rc0/rlgym.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rlgym
-Version: 2.0.0a3
+Version: 2.0.0rc0
 Summary: A python API with zero dependencies to create fully customizable environments for Reinforcement Learning projects.
 Home-page: https://rlgym.org
 Author: Lucas Emery and Matthew Allen
 Author-email: contact@rlgym.org
 License: Apache 2.0
 Project-URL: Source Code, https://github.com/lucas-emery/rocket-league-gym
 Keywords: rocket-league,gym,reinforcement-learning,rlgym
@@ -46,16 +46,16 @@
 Once the API is installed, you will need to enable the RLGym plugin from inside the Bakkesmod plugin manager. To do this, first launch the game, then press F2 to open the Bakkesmod menu. Navigate to the `plugins` tab and open the `Plugin Manager`. From there, scroll down until you find the RLGym plugin, and enable it. Close the game when this is done.
 
 
 ### Testing everything works
 RLGym is now installed! simply run ```example.py``` from our repo to ensure everything works.
 
 ## Dependency Management
-**Don't** specify this package as a dependency, this is an **instalation only** package.
+**DO NOT** specify this package as a dependency, this is an **installation only** package.
 
-You should depend directly on the package you're consuming and its corresponding extras, be it 
-`rlgym-rocket-league[sim]`, `rlgym-api` or any other in particular.
+You should depend directly on the package you're consuming and its corresponding extras, e.g.
+`rlgym-rocket-league[sim]`, `rlgym-api` or whichever of our libraries your project is using.
 
 ## Usage
 For tutorials and documentation, please visit our [Wiki](https://rlgym.org/).
 
 We also provide the base RLGym API in its own [standalone package](https://pypi.org/project/rlgym-api/) with no dependencies.
```

### Comparing `rlgym-2.0.0a3/setup.json` & `rlgym-2.0.0rc0/setup.json`

 * *Files 18% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.78125%*

 * *Differences: {"'extras_require'": "{'rl': ['rlgym-rocket-league[all] ==2.0.0-rc'], 'rl-sim': "*

 * *                     "['rlgym-rocket-league[sim] ==2.0.0-rc'], 'rl-game': "*

 * *                     "['rlgym-rocket-league[game] ==2.0.0-rc'], 'all': ['rlgym-rocket-league[all] "*

 * *                     "==2.0.0-rc']}",*

 * * "'install_requires'": "['rlgym-api ==2.0.0-rc']",*

 * * "'long_description'": '"# The Rocket League Gym\\nThis is a python API that can be used to treat '*

 * *                       'the game [Rocket League](https://www.rock […]*

```diff
@@ -1,27 +1,27 @@
 {
     "description": "A python API with zero dependencies to create fully customizable environments for Reinforcement Learning projects.",
     "extras_require": {
         "all": [
-            "rlgym-rocket-league[all] ==2.0.0-alpha-3"
+            "rlgym-rocket-league[all] ==2.0.0-rc"
         ],
         "rl": [
-            "rlgym-rocket-league[all] ==2.0.0-alpha-3"
+            "rlgym-rocket-league[all] ==2.0.0-rc"
         ],
         "rl-game": [
-            "rlgym-rocket-league[game] ==2.0.0-alpha-3"
+            "rlgym-rocket-league[game] ==2.0.0-rc"
         ],
         "rl-sim": [
-            "rlgym-rocket-league[sim] ==2.0.0-alpha-3"
+            "rlgym-rocket-league[sim] ==2.0.0-rc"
         ]
     },
     "install_requires": [
-        "rlgym-api ==2.0.0-alpha-1"
+        "rlgym-api ==2.0.0-rc"
     ],
-    "long_description": "# The Rocket League Gym\nThis is a python API that can be used to treat the game [Rocket League](https://www.rocketleague.com) as though it were an [OpenAI Gym](https://gym.openai.com)-style environment for Reinforcement Learning projects. This API must be used with the accompanying Bakkesmod plugin.\n\n## Requirements\n* A Windows 10 PC\n* Rocket League (Both Steam and Epic are supported)\n* [Bakkesmod](https://www.bakkesmod.com)\n* The RLGym plugin for Bakkesmod (It's installed automatically by pip)\n* Python between versions 3.7 and 3.9 (3.10 not supported).\n\n## Installation\nInstall the library via pip:\n```\npip install rlgym[all]  // Installs every rlgym component\n\npip install rlgym  // Installs only the api\n\npip install rlgym[rl]  // Installs all rocket league packages\n\npip install rlgym[rl-sim]  // Installs only RocketSim rocket league packages\n```\n\n### If you installed the Rocket League game distribution\nOnce the API is installed, you will need to enable the RLGym plugin from inside the Bakkesmod plugin manager. To do this, first launch the game, then press F2 to open the Bakkesmod menu. Navigate to the `plugins` tab and open the `Plugin Manager`. From there, scroll down until you find the RLGym plugin, and enable it. Close the game when this is done.\n\n\n### Testing everything works\nRLGym is now installed! simply run ```example.py``` from our repo to ensure everything works.\n\n## Dependency Management\n**Don't** specify this package as a dependency, this is an **instalation only** package.\n\nYou should depend directly on the package you're consuming and its corresponding extras, be it \n`rlgym-rocket-league[sim]`, `rlgym-api` or any other in particular.\n\n## Usage\nFor tutorials and documentation, please visit our [Wiki](https://rlgym.org/).\n\nWe also provide the base RLGym API in its own [standalone package](https://pypi.org/project/rlgym-api/) with no dependencies.\n",
+    "long_description": "# The Rocket League Gym\nThis is a python API that can be used to treat the game [Rocket League](https://www.rocketleague.com) as though it were an [OpenAI Gym](https://gym.openai.com)-style environment for Reinforcement Learning projects. This API must be used with the accompanying Bakkesmod plugin.\n\n## Requirements\n* A Windows 10 PC\n* Rocket League (Both Steam and Epic are supported)\n* [Bakkesmod](https://www.bakkesmod.com)\n* The RLGym plugin for Bakkesmod (It's installed automatically by pip)\n* Python between versions 3.7 and 3.9 (3.10 not supported).\n\n## Installation\nInstall the library via pip:\n```\npip install rlgym[all]  // Installs every rlgym component\n\npip install rlgym  // Installs only the api\n\npip install rlgym[rl]  // Installs all rocket league packages\n\npip install rlgym[rl-sim]  // Installs only RocketSim rocket league packages\n```\n\n### If you installed the Rocket League game distribution\nOnce the API is installed, you will need to enable the RLGym plugin from inside the Bakkesmod plugin manager. To do this, first launch the game, then press F2 to open the Bakkesmod menu. Navigate to the `plugins` tab and open the `Plugin Manager`. From there, scroll down until you find the RLGym plugin, and enable it. Close the game when this is done.\n\n\n### Testing everything works\nRLGym is now installed! simply run ```example.py``` from our repo to ensure everything works.\n\n## Dependency Management\n**DO NOT** specify this package as a dependency, this is an **installation only** package.\n\nYou should depend directly on the package you're consuming and its corresponding extras, e.g.\n`rlgym-rocket-league[sim]`, `rlgym-api` or whichever of our libraries your project is using.\n\n## Usage\nFor tutorials and documentation, please visit our [Wiki](https://rlgym.org/).\n\nWe also provide the base RLGym API in its own [standalone package](https://pypi.org/project/rlgym-api/) with no dependencies.\n",
     "long_description_content_type": "text/markdown",
     "name": "rlgym",
     "packages": [
         "rlgym.version"
     ],
-    "version": "2.0.0-alpha-3"
+    "version": "2.0.0-rc"
 }
```

### Comparing `rlgym-2.0.0a3/setup.py` & `rlgym-2.0.0rc0/setup.py`

 * *Files identical despite different names*

