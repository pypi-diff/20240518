# Comparing `tmp/lycoris_lora-2.3.0.dev9.tar.gz` & `tmp/lycoris_lora-3.0.0.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lycoris_lora-2.3.0.dev9.tar", last modified: Fri May  3 14:52:43 2024, max compression
+gzip compressed data, was "lycoris_lora-3.0.0.dev1.tar", last modified: Sat May 18 10:22:41 2024, max compression
```

## Comparing `lycoris_lora-2.3.0.dev9.tar` & `lycoris_lora-3.0.0.dev1.tar`

### file list

```diff
@@ -1,58 +1,43 @@
-drwxrwxrwx   0        0        0        0 2024-05-03 14:52:43.762148 lycoris_lora-2.3.0.dev9/
--rw-rw-rw-   0        0        0    11545 2023-03-09 05:37:07.000000 lycoris_lora-2.3.0.dev9/LICENSE.md
--rw-rw-rw-   0        0        0      527 2024-05-03 14:52:43.762148 lycoris_lora-2.3.0.dev9/PKG-INFO
--rw-rw-rw-   0        0        0    11988 2024-05-03 13:57:17.000000 lycoris_lora-2.3.0.dev9/README.md
-drwxrwxrwx   0        0        0        0 2024-05-03 14:52:43.715648 lycoris_lora-2.3.0.dev9/lycoris/
--rw-rw-rw-   0        0        0      550 2024-02-05 11:33:28.000000 lycoris_lora-2.3.0.dev9/lycoris/__init__.py
--rw-rw-rw-   0        0        0     2537 2023-12-02 03:39:50.000000 lycoris_lora-2.3.0.dev9/lycoris/config.py
-drwxrwxrwx   0        0        0        0 2024-05-03 14:52:43.719152 lycoris_lora-2.3.0.dev9/lycoris/hcp/
--rw-rw-rw-   0        0        0      156 2023-12-02 03:39:50.000000 lycoris_lora-2.3.0.dev9/lycoris/hcp/__init__.py
--rw-rw-rw-   0        0        0     5329 2023-12-02 03:39:50.000000 lycoris_lora-2.3.0.dev9/lycoris/hcp/base.py
--rw-rw-rw-   0        0        0     2281 2024-02-12 10:32:01.000000 lycoris_lora-2.3.0.dev9/lycoris/hcp/diag_oft.py
--rw-rw-rw-   0        0        0     3391 2024-03-04 15:01:10.000000 lycoris_lora-2.3.0.dev9/lycoris/hcp/loha.py
--rw-rw-rw-   0        0        0     5643 2024-03-04 15:01:21.000000 lycoris_lora-2.3.0.dev9/lycoris/hcp/lokr.py
-drwxrwxrwx   0        0        0        0 2024-05-03 14:52:43.725674 lycoris_lora-2.3.0.dev9/lycoris/kohya/
--rw-rw-rw-   0        0        0    31784 2024-04-08 09:27:28.000000 lycoris_lora-2.3.0.dev9/lycoris/kohya/__init__.py
--rw-rw-rw-   0        0        0    59991 2024-02-18 06:15:40.000000 lycoris_lora-2.3.0.dev9/lycoris/kohya/model_utils.py
--rw-rw-rw-   0        0        0    61070 2023-12-02 03:39:51.000000 lycoris_lora-2.3.0.dev9/lycoris/kohya/original_unet.py
--rw-rw-rw-   0        0        0    21297 2024-02-18 06:15:40.000000 lycoris_lora-2.3.0.dev9/lycoris/kohya/sdxl_model_util.py
--rw-rw-rw-   0        0        0    42690 2023-12-02 03:39:51.000000 lycoris_lora-2.3.0.dev9/lycoris/kohya/sdxl_original_unet.py
--rw-rw-rw-   0        0        0    19901 2024-03-11 06:16:36.000000 lycoris_lora-2.3.0.dev9/lycoris/kohya/test_hyperdream.py
--rw-rw-rw-   0        0        0     1514 2023-12-02 03:39:50.000000 lycoris_lora-2.3.0.dev9/lycoris/kohya/utils.py
--rw-rw-rw-   0        0        0     1053 2024-02-05 11:33:20.000000 lycoris_lora-2.3.0.dev9/lycoris/logging.py
-drwxrwxrwx   0        0        0        0 2024-05-03 14:52:43.734186 lycoris_lora-2.3.0.dev9/lycoris/modules/
--rw-rw-rw-   0        0        0     4201 2024-05-03 13:52:01.000000 lycoris_lora-2.3.0.dev9/lycoris/modules/__init__.py
--rw-rw-rw-   0        0        0     8185 2023-12-02 03:39:50.000000 lycoris_lora-2.3.0.dev9/lycoris/modules/attention.py
--rw-rw-rw-   0        0        0     7155 2024-05-03 14:44:58.000000 lycoris_lora-2.3.0.dev9/lycoris/modules/base.py
--rw-rw-rw-   0        0        0     7938 2024-05-03 14:40:49.000000 lycoris_lora-2.3.0.dev9/lycoris/modules/boft.py
--rw-rw-rw-   0        0        0     6702 2024-05-03 14:47:33.000000 lycoris_lora-2.3.0.dev9/lycoris/modules/diag_oft.py
--rw-rw-rw-   0        0        0     4395 2024-05-03 12:40:31.000000 lycoris_lora-2.3.0.dev9/lycoris/modules/dylora.py
--rw-rw-rw-   0        0        0     4518 2024-05-03 13:36:02.000000 lycoris_lora-2.3.0.dev9/lycoris/modules/full.py
--rw-rw-rw-   0        0        0    11788 2024-04-08 09:27:20.000000 lycoris_lora-2.3.0.dev9/lycoris/modules/glokr.py
--rw-rw-rw-   0        0        0     4978 2024-04-08 09:27:20.000000 lycoris_lora-2.3.0.dev9/lycoris/modules/glora.py
-drwxrwxrwx   0        0        0        0 2024-05-03 14:52:43.735186 lycoris_lora-2.3.0.dev9/lycoris/modules/hypernet/
--rw-rw-rw-   0        0        0       79 2023-12-02 03:39:50.000000 lycoris_lora-2.3.0.dev9/lycoris/modules/hypernet/__init__.py
--rw-rw-rw-   0        0        0     8302 2023-12-02 03:39:50.000000 lycoris_lora-2.3.0.dev9/lycoris/modules/hypernet/generater.py
--rw-rw-rw-   0        0        0     8339 2024-02-18 06:15:40.000000 lycoris_lora-2.3.0.dev9/lycoris/modules/hypernet/text_encoder.py
--rw-rw-rw-   0        0        0     2078 2024-03-11 06:14:46.000000 lycoris_lora-2.3.0.dev9/lycoris/modules/ia3.py
--rw-rw-rw-   0        0        0    12663 2024-04-08 09:27:20.000000 lycoris_lora-2.3.0.dev9/lycoris/modules/lilora.py
--rw-rw-rw-   0        0        0    10800 2024-05-03 14:47:33.000000 lycoris_lora-2.3.0.dev9/lycoris/modules/locon.py
--rw-rw-rw-   0        0        0    13088 2024-05-03 14:47:00.000000 lycoris_lora-2.3.0.dev9/lycoris/modules/loha.py
--rw-rw-rw-   0        0        0    17926 2024-05-03 14:47:33.000000 lycoris_lora-2.3.0.dev9/lycoris/modules/lokr.py
--rw-rw-rw-   0        0        0     2387 2024-05-03 13:35:13.000000 lycoris_lora-2.3.0.dev9/lycoris/modules/norms.py
-drwxrwxrwx   0        0        0        0 2024-05-03 14:52:43.739696 lycoris_lora-2.3.0.dev9/lycoris/utils/
--rw-rw-rw-   0        0        0    23287 2024-03-23 07:38:25.000000 lycoris_lora-2.3.0.dev9/lycoris/utils/__init__.py
--rw-rw-rw-   0        0        0      497 2024-03-13 17:06:13.000000 lycoris_lora-2.3.0.dev9/lycoris/utils/bnb.py
--rw-rw-rw-   0        0        0     1078 2023-12-02 03:39:50.000000 lycoris_lora-2.3.0.dev9/lycoris/utils/logger.py
--rw-rw-rw-   0        0        0      190 2023-12-02 03:39:50.000000 lycoris_lora-2.3.0.dev9/lycoris/utils/preset.py
--rw-rw-rw-   0        0        0      251 2023-12-02 03:39:50.000000 lycoris_lora-2.3.0.dev9/lycoris/utils/xformers_utils.py
--rw-rw-rw-   0        0        0    18706 2024-03-16 16:01:01.000000 lycoris_lora-2.3.0.dev9/lycoris/wrapper.py
-drwxrwxrwx   0        0        0        0 2024-05-03 14:52:43.761143 lycoris_lora-2.3.0.dev9/lycoris_lora.egg-info/
--rw-rw-rw-   0        0        0      527 2024-05-03 14:52:43.000000 lycoris_lora-2.3.0.dev9/lycoris_lora.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1261 2024-05-03 14:52:43.000000 lycoris_lora-2.3.0.dev9/lycoris_lora.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-03 14:52:43.000000 lycoris_lora-2.3.0.dev9/lycoris_lora.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-11-06 13:42:23.000000 lycoris_lora-2.3.0.dev9/lycoris_lora.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       53 2024-05-03 14:52:43.000000 lycoris_lora-2.3.0.dev9/lycoris_lora.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-05-03 14:52:43.000000 lycoris_lora-2.3.0.dev9/lycoris_lora.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-03 14:52:43.763147 lycoris_lora-2.3.0.dev9/setup.cfg
--rw-rw-rw-   0        0        0      638 2024-05-03 14:52:39.000000 lycoris_lora-2.3.0.dev9/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-18 10:22:41.609679 lycoris_lora-3.0.0.dev1/
+-rw-rw-rw-   0        0        0    11545 2023-03-09 05:37:07.000000 lycoris_lora-3.0.0.dev1/LICENSE.md
+-rw-rw-rw-   0        0        0      527 2024-05-18 10:22:41.608679 lycoris_lora-3.0.0.dev1/PKG-INFO
+-rw-rw-rw-   0        0        0    12433 2024-05-15 08:22:33.000000 lycoris_lora-3.0.0.dev1/README.md
+drwxrwxrwx   0        0        0        0 2024-05-18 10:22:41.583648 lycoris_lora-3.0.0.dev1/lycoris/
+-rw-rw-rw-   0        0        0      550 2024-02-05 11:33:28.000000 lycoris_lora-3.0.0.dev1/lycoris/__init__.py
+-rw-rw-rw-   0        0        0     2537 2023-12-02 03:39:50.000000 lycoris_lora-3.0.0.dev1/lycoris/config.py
+drwxrwxrwx   0        0        0        0 2024-05-18 10:22:41.586653 lycoris_lora-3.0.0.dev1/lycoris/functional/
+-rw-rw-rw-   0        0        0      251 2024-05-17 14:23:10.000000 lycoris_lora-3.0.0.dev1/lycoris/functional/__init__.py
+-rw-rw-rw-   0        0        0     2379 2024-05-17 14:23:10.000000 lycoris_lora-3.0.0.dev1/lycoris/functional/general.py
+-rw-rw-rw-   0        0        0     3354 2024-05-17 14:23:10.000000 lycoris_lora-3.0.0.dev1/lycoris/functional/locon.py
+-rw-rw-rw-   0        0        0     5259 2024-05-17 12:55:00.000000 lycoris_lora-3.0.0.dev1/lycoris/functional/loha.py
+-rw-rw-rw-   0        0        0    31780 2024-05-18 10:06:20.000000 lycoris_lora-3.0.0.dev1/lycoris/kohya.py
+-rw-rw-rw-   0        0        0     1053 2024-02-05 11:33:20.000000 lycoris_lora-3.0.0.dev1/lycoris/logging.py
+drwxrwxrwx   0        0        0        0 2024-05-18 10:22:41.590651 lycoris_lora-3.0.0.dev1/lycoris/modules/
+-rw-rw-rw-   0        0        0     4201 2024-05-03 13:52:01.000000 lycoris_lora-3.0.0.dev1/lycoris/modules/__init__.py
+-rw-rw-rw-   0        0        0     8136 2024-05-18 09:26:28.000000 lycoris_lora-3.0.0.dev1/lycoris/modules/base.py
+-rw-rw-rw-   0        0        0     7635 2024-05-18 08:00:24.000000 lycoris_lora-3.0.0.dev1/lycoris/modules/boft.py
+-rw-rw-rw-   0        0        0     6971 2024-05-18 10:13:54.000000 lycoris_lora-3.0.0.dev1/lycoris/modules/diag_oft.py
+-rw-rw-rw-   0        0        0     4395 2024-05-03 12:40:31.000000 lycoris_lora-3.0.0.dev1/lycoris/modules/dylora.py
+-rw-rw-rw-   0        0        0     5775 2024-05-18 08:01:04.000000 lycoris_lora-3.0.0.dev1/lycoris/modules/full.py
+-rw-rw-rw-   0        0        0     7140 2024-05-18 10:13:31.000000 lycoris_lora-3.0.0.dev1/lycoris/modules/glora.py
+-rw-rw-rw-   0        0        0     2078 2024-03-11 06:14:46.000000 lycoris_lora-3.0.0.dev1/lycoris/modules/ia3.py
+-rw-rw-rw-   0        0        0    10858 2024-05-18 09:08:52.000000 lycoris_lora-3.0.0.dev1/lycoris/modules/locon.py
+-rw-rw-rw-   0        0        0    10688 2024-05-18 09:10:27.000000 lycoris_lora-3.0.0.dev1/lycoris/modules/loha.py
+-rw-rw-rw-   0        0        0    15618 2024-05-18 09:11:19.000000 lycoris_lora-3.0.0.dev1/lycoris/modules/lokr.py
+-rw-rw-rw-   0        0        0     3557 2024-05-18 09:12:34.000000 lycoris_lora-3.0.0.dev1/lycoris/modules/norms.py
+drwxrwxrwx   0        0        0        0 2024-05-18 10:22:41.594162 lycoris_lora-3.0.0.dev1/lycoris/utils/
+-rw-rw-rw-   0        0        0    23287 2024-03-23 07:38:25.000000 lycoris_lora-3.0.0.dev1/lycoris/utils/__init__.py
+-rw-rw-rw-   0        0        0      497 2024-03-13 17:06:13.000000 lycoris_lora-3.0.0.dev1/lycoris/utils/bnb.py
+-rw-rw-rw-   0        0        0     1078 2023-12-02 03:39:50.000000 lycoris_lora-3.0.0.dev1/lycoris/utils/logger.py
+-rw-rw-rw-   0        0        0      190 2023-12-02 03:39:50.000000 lycoris_lora-3.0.0.dev1/lycoris/utils/preset.py
+-rw-rw-rw-   0        0        0      251 2023-12-02 03:39:50.000000 lycoris_lora-3.0.0.dev1/lycoris/utils/xformers_utils.py
+-rw-rw-rw-   0        0        0    18779 2024-05-15 08:22:10.000000 lycoris_lora-3.0.0.dev1/lycoris/wrapper.py
+drwxrwxrwx   0        0        0        0 2024-05-18 10:22:41.608679 lycoris_lora-3.0.0.dev1/lycoris_lora.egg-info/
+-rw-rw-rw-   0        0        0      527 2024-05-18 10:22:41.000000 lycoris_lora-3.0.0.dev1/lycoris_lora.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      879 2024-05-18 10:22:41.000000 lycoris_lora-3.0.0.dev1/lycoris_lora.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-18 10:22:41.000000 lycoris_lora-3.0.0.dev1/lycoris_lora.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-11-06 13:42:23.000000 lycoris_lora-3.0.0.dev1/lycoris_lora.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       53 2024-05-18 10:22:41.000000 lycoris_lora-3.0.0.dev1/lycoris_lora.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-05-18 10:22:41.000000 lycoris_lora-3.0.0.dev1/lycoris_lora.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-18 10:22:41.609679 lycoris_lora-3.0.0.dev1/setup.cfg
+-rw-rw-rw-   0        0        0      638 2024-05-18 10:22:31.000000 lycoris_lora-3.0.0.dev1/setup.py
```

### Comparing `lycoris_lora-2.3.0.dev9/LICENSE.md` & `lycoris_lora-3.0.0.dev1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `lycoris_lora-2.3.0.dev9/PKG-INFO` & `lycoris_lora-3.0.0.dev1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lycoris_lora
-Version: 2.3.0.dev9
+Version: 3.0.0.dev1
 Summary: Lora beYond Conventional methods, Other Rank adaptation Implementations for Stable diffusion
 Home-page: https://github.com/KohakuBlueleaf/LyCORIS
 Author: Shih-Ying Yeh(KohakuBlueLeaf), Yu-Guan Hsieh, Zhidong Gao
 Author-email: apolloyeh0123@gmail.com
 Requires-Python: >=3.10
 License-File: LICENSE.md
 Requires-Dist: torch
```

### Comparing `lycoris_lora-2.3.0.dev9/README.md` & `lycoris_lora-3.0.0.dev1/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,43 +1,46 @@
-# LyCORIS - Lora beYond Conventional methods, Other Rank adaptation Implementations for Stable diffusion.
+# LyCORIS - Lora beYond Conventional methods, Other Rank adaptation Implementations for Stable diffusion. (ICLR'24)
 
 ![banner image](docs/images/banner.png)
 
 A project that implements different parameter-efficient fine-tuning algorithms for Stable Diffusion.
 
 This project originated from LoCon (see archive branch).
 
 **If you are interested in discussing more details, you can join [our Discord server](https://discord.gg/VtTFKrj9gJ)**
 
 [![Discord!](https://i.imgur.com/A8tOvFS.jpg)](https://discord.gg/VtTFKrj9gJ)
 
-**If you want to check more in-depth experiment results and discussions for LyCORIS, you can check our [paper](https://arxiv.org/abs/2309.14859)**
+**If you want to check more in-depth experiment results and discussions for LyCORIS, you can check our [paper](https://openreview.net/forum?id=wfzXa8e783)**
 
 ## Algorithm Overview
 
 LyCORIS currently contains LoRA (LoCon), LoHa, LoKr, (IA)^3, DyLoRA, Native fine-tuning (aka dreambooth).
 GLoRA and GLoKr are coming soon.
 Please check [List of Implemented Algorithms](docs/Algo-List.md) and [Guidelines](docs/Guidelines.md) for more details.
 
 A simple comparison of some of these methods are provided below (to be taken with a grain of salt)
 
-|                       | Full | LoRA | LoHa | LoKr low factor | LoKr high factor |
+|                       | Full | LoRA | LoHa | LoKr low factor | LoKr high factor $^+$ |
 | --------------------- | ---- | ---- | ---- | --------------- | ---------------- |
 | Fidelity              | ★   | ●   | ▲   | ◉              | ▲               |
-| Flexibility$^*$     | ★   | ●   | ◉   | ▲              | ●$^†$        |
+| Flexibility $^*$     | ★   | ●   | ◉   | ▲              | ● $^†$        |
 | Diversity             | ▲   | ◉   | ★   | ●              | ★               |
 | Size                  | ▲   | ●   | ●   | ●              | ★               |
 | Training Speed Linear | ★   | ●   | ●   | ★              | ★               |
 | Training Speed Conv   | ●   | ★   | ▲   | ●              | ●               |
 
 ★ > ◉ > ● > ▲
 [> means better and smaller size is better]
 
-$^*$ Flexibility means anything related to generating images not similar to those in the training set, and combination of multiple concepts, whether they are trained together or not
-$^†$ It may become more difficult to switch base model or combine multiple concepts in this situation
+$^+$ Usually we take `factor <= 0.5 * sqrt(dim)` as low factor and `factor >= sqrt(dim` as high factor. For example, factor<=8 for SD1.x/SD2.x/SDXL can be seen as low factor, and, factor>=16 can be seen as high factor. <br>
+$^*$ Flexibility means anything related to generating images not similar to those in the training set, and combination of multiple concepts, whether they are trained together or not <br>
+$^†$ It may become more difficult to switch base model or combine multiple concepts in this situation <br>
+
+**The actual performance may vary depending on the datasets, tasks, and hyperparameters used. It is recommended to experiment with different settings to achieve optimal results.**
 
 ## Usage
 
 ### Image Generation
 
 #### [a1111/sd-webui](https://github.com/AUTOMATIC1111/stable-diffusion-webui)
```

### Comparing `lycoris_lora-2.3.0.dev9/lycoris/__init__.py` & `lycoris_lora-3.0.0.dev1/lycoris/__init__.py`

 * *Files identical despite different names*

### Comparing `lycoris_lora-2.3.0.dev9/lycoris/config.py` & `lycoris_lora-3.0.0.dev1/lycoris/config.py`

 * *Files identical despite different names*

### Comparing `lycoris_lora-2.3.0.dev9/lycoris/kohya/__init__.py` & `lycoris_lora-3.0.0.dev1/lycoris/kohya.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,32 +6,32 @@
 
 import os
 import re
 from typing import List
 
 import torch
 
-from .utils import *
-from ..wrapper import LycorisNetwork
-from ..modules.locon import LoConModule
-from ..modules.loha import LohaModule
-from ..modules.ia3 import IA3Module
-from ..modules.lokr import LokrModule
-from ..modules.dylora import DyLoraModule
-from ..modules.glora import GLoRAModule
-from ..modules.norms import NormModule
-from ..modules.full import FullModule
-from ..modules.diag_oft import DiagOFTModule
-from ..modules.boft import ButterflyOFTModule
-from ..modules import make_module
-
-from ..config import PRESET
-from ..utils.preset import read_preset
-from ..utils import get_module, str_bool
-from ..logging import logger
+from library.train_util import *
+from .wrapper import LycorisNetwork
+from .modules.locon import LoConModule
+from .modules.loha import LohaModule
+from .modules.ia3 import IA3Module
+from .modules.lokr import LokrModule
+from .modules.dylora import DyLoraModule
+from .modules.glora import GLoRAModule
+from .modules.norms import NormModule
+from .modules.full import FullModule
+from .modules.diag_oft import DiagOFTModule
+from .modules.boft import ButterflyOFTModule
+from .modules import make_module
+
+from .config import PRESET
+from .utils.preset import read_preset
+from .utils import get_module, str_bool
+from .logging import logger
 
 
 network_module_dict = {
     "lora": LoConModule,
     "locon": LoConModule,
     "loha": LohaModule,
     "ia3": IA3Module,
```

### Comparing `lycoris_lora-2.3.0.dev9/lycoris/kohya/test_hyperdream.py` & `lycoris_lora-3.0.0.dev1/lycoris/wrapper.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,69 +1,55 @@
-# network module for kohya
-# reference:
-# https://github.com/microsoft/LoRA/blob/main/loralib/layers.py
-# https://github.com/cloneofsimo/lora/blob/master/lora_diffusion/lora.py
-# https://github.com/kohya-ss/sd-scripts/blob/main/networks/lora.py
+# General LyCORIS wrapper based on kohya-ss/sd-scripts' style
 
+import math
 import os
-import re
+import regex as re
 import sys
-from typing import List
 
 sys.setrecursionlimit(10000)
+from typing import List
 
 import torch
-import torch.utils.checkpoint as checkpoint
+import torch.nn as nn
 
-from .utils import *
-from ..wrapper import LycorisNetwork
-from ..modules.locon import LoConModule
-from ..modules.loha import LohaModule
-from ..modules.ia3 import IA3Module
-from ..modules.lokr import LokrModule
-from ..modules.dylora import DyLoraModule
-from ..modules.glora import GLoRAModule
-from ..modules.norms import NormModule
-from ..modules.full import FullModule
-from ..modules.diag_oft import DiagOFTModule
-from ..modules.boft import ButterflyOFTModule
-from ..modules import make_module
-
-from ..config import PRESET
-from ..utils.preset import read_preset
-from ..utils import get_module, str_bool
-from ..logging import logger
+from .modules.locon import LoConModule
+from .modules.loha import LohaModule
+from .modules.lokr import LokrModule
+from .modules.dylora import DyLoraModule
+from .modules.glora import GLoRAModule
+from .modules.norms import NormModule
+from .modules.full import FullModule
+from .modules.diag_oft import DiagOFTModule
+from .modules.boft import ButterflyOFTModule
+from .modules import make_module
+
+from .config import PRESET
+from .utils.preset import read_preset
+from .utils import get_module, str_bool
+from .logging import logger
 
 
 network_module_dict = {
     "lora": LoConModule,
     "locon": LoConModule,
     "loha": LohaModule,
-    "ia3": IA3Module,
     "lokr": LokrModule,
     "dylora": DyLoraModule,
     "glora": GLoRAModule,
     "full": FullModule,
     "diag-oft": DiagOFTModule,
     "boft": ButterflyOFTModule,
 }
 
 
-def create_hypernetwork(
-    multiplier,
-    network_dim,
-    network_alpha,
-    vae,
-    text_encoder,
-    unet,
-    vocab_size,
-    **kwargs,
-):
-    if network_dim is None:
-        network_dim = 4
+def create_lycoris(module, multiplier, linear_dim, linear_alpha, **kwargs):
+    if linear_dim is None:
+        linear_dim = 4  # default
+    conv_dim = int(kwargs.get("conv_dim", linear_dim) or linear_dim)
+    conv_alpha = float(kwargs.get("conv_alpha", linear_alpha) or linear_alpha)
     dropout = float(kwargs.get("dropout", 0.0) or 0.0)
     rank_dropout = float(kwargs.get("rank_dropout", 0.0) or 0.0)
     module_dropout = float(kwargs.get("module_dropout", 0.0) or 0.0)
     algo = (kwargs.get("algo", "lora") or "lora").lower()
     use_tucker = str_bool(
         not kwargs.get("disable_conv_cp", True)
         or kwargs.get("use_conv_cp", False)
@@ -71,457 +57,480 @@
         or kwargs.get("use_tucker", False)
     )
     if "disable_conv_cp" in kwargs or "use_cp" in kwargs or "use_conv_cp" in kwargs:
         logger.warning(
             "disable_conv_cp and use_cp are deprecated. Please use use_tucker instead.",
             stacklevel=2,
         )
+    use_scalar = str_bool(kwargs.get("use_scalar", False))
     block_size = int(kwargs.get("block_size", 4) or 4)
-    down_dim = int(kwargs.get("down_dim", 128) or 128)
-    up_dim = int(kwargs.get("up_dim", 64) or 64)
-    delta_iters = int(kwargs.get("delta_iters", 5) or 5)
-    decoder_blocks = int(kwargs.get("decoder_blocks", 4) or 4)
-    network_module = {
-        "lora": LoConModule,
-        "locon": LoConModule,
-    }[algo]
+    train_norm = str_bool(kwargs.get("train_norm", False))
+    constrain = float(kwargs.get("constrain", 0) or 0)
+    rescaled = str_bool(kwargs.get("rescaled", False))
+    weight_decompose = str_bool(kwargs.get("dora_wd", False))
+    full_matrix = str_bool(kwargs.get("full_matrix", False))
+    bypass_mode = str_bool(kwargs.get("bypass_mode", False))
+    unbalanced_factorization = str_bool(kwargs.get("unbalanced_factorization", False))
+
+    if unbalanced_factorization:
+        logger.info("Unbalanced factorization for LoKr is enabled")
+
+    if bypass_mode:
+        logger.info("Bypass mode is enabled")
+
+    if weight_decompose:
+        logger.info("Weight decomposition is enabled")
+
+    if full_matrix:
+        logger.info("Full matrix mode for LoKr is enabled")
+
+    if algo == "glora" and conv_dim > 0:
+        conv_dim = 0
+        logger.info("Disable conv layer for GLoRA")
+
+    preset = kwargs.get("preset", "full")
+    if preset not in PRESET:
+        preset = read_preset(preset)
+    else:
+        preset = PRESET[preset]
+    assert preset is not None
+    LycorisNetwork.apply_preset(preset)
 
     logger.info(f"Using rank adaptation algo: {algo}")
 
-    return HyperDreamNetwork(
-        text_encoder,
-        unet,
+    if (
+        (algo == "loha")
+        and not kwargs.get("no_dim_warn", False)
+        and (linear_dim > 64 or conv_dim > 64)
+    ):
+        warning_type = {"loha": "Hadamard Product representation"}
+        warning_msg = (
+            "You are not supposed to use dim>64 (64*64 = 4096, it already has enough rank)\n"
+            f"in {warning_type[algo]}!\n"
+            "Please consider use lower dim or disable this warning with --network_args no_dim_warn=True\n"
+            f"If you just want to use high dim {algo}, please consider use lower lr."
+        )
+        logger.warning(warning_msg, stacklevel=2)
+
+    network = LycorisNetwork(
+        module,
         multiplier=multiplier,
-        lora_dim=network_dim,
-        alpha=network_alpha,
-        use_tucker=use_tucker,
+        lora_dim=linear_dim,
+        conv_lora_dim=conv_dim,
+        alpha=linear_alpha,
+        conv_alpha=conv_alpha,
         dropout=dropout,
         rank_dropout=rank_dropout,
         module_dropout=module_dropout,
-        network_module=network_module,
-        down_dim=down_dim,
-        up_dim=up_dim,
-        delta_iters=delta_iters,
-        decoder_blocks=decoder_blocks,
-        vocab_size=vocab_size,
+        use_tucker=use_tucker,
+        use_scalar=use_scalar,
+        network_module=algo,
+        train_norm=train_norm,
         decompose_both=kwargs.get("decompose_both", False),
         factor=kwargs.get("factor", -1),
         block_size=block_size,
+        constrain=constrain,
+        rescaled=rescaled,
+        weight_decompose=weight_decompose,
+        full_matrix=full_matrix,
+        bypass_mode=bypass_mode,
+        unbalanced_factorization=unbalanced_factorization,
     )
 
+    if algo == "dylora":
+        # dylora didn't support scale weight norm yet
+        delattr(type(network), "apply_max_norm_regularization")
 
-class HyperDreamNetwork(torch.nn.Module):
-    """
-    HyperDreamBooth hypernetwork part
-    only train Attention right now
-    """
-
-    UNET_TARGET_REPLACE_MODULE = [
-        "Attention",
-    ]
-    UNET_TARGET_REPLACE_NAME = []
-    TEXT_ENCODER_TARGET_REPLACE_MODULE = ["CLIPAttention"]
-    LORA_PREFIX_UNET = "lora_unet"
-    LORA_PREFIX_TEXT_ENCODER = "lora_te"
+    return network
+
+
+def create_lycoris_from_weights(multiplier, file, module, weights_sd=None, **kwargs):
+    if weights_sd is None:
+        if os.path.splitext(file)[1] == ".safetensors":
+            from safetensors.torch import load_file
+
+            weights_sd = load_file(file)
+        else:
+            weights_sd = torch.load(file, map_location="cpu")
+
+    # get dim/alpha mapping
+    loras = {}
+    for key in weights_sd:
+        if "." not in key:
+            continue
+
+        lora_name = key.split(".")[0]
+        loras[lora_name] = None
+
+    for name, modules in module.named_modules():
+        lora_name = f"{LycorisNetwork.LORA_PREFIX}_{name}".replace(".", "_")
+        if lora_name in loras:
+            loras[lora_name] = modules
+
+    network = LycorisNetwork(module, init_only=True)
+    network.multiplier = multiplier
+    network.loras = []
+
+    for lora_name, orig_modules in loras.items():
+        if orig_modules is None:
+            continue
+        lyco_type, params = get_module(weights_sd, lora_name)
+        module = make_module(lyco_type, params, lora_name, orig_modules)
+        if module is not None:
+            network.loras.append(module)
+            network.algo_table[module.__class__.__name__] = (
+                network.algo_table.get(module.__class__.__name__, 0) + 1
+            )
+
+    for lora in network.loras:
+        lora.multiplier = multiplier
+
+    return network, weights_sd
+
+
+class LycorisNetwork(torch.nn.Module):
+    ENABLE_CONV = True
+    TARGET_REPLACE_MODULE = []
+    TARGET_REPLACE_NAME = []
+    LORA_PREFIX = "lycoris"
+    MODULE_ALGO_MAP = {}
+    NAME_ALGO_MAP = {}
+
+    @classmethod
+    def apply_preset(cls, preset):
+        if "enable_conv" in preset:
+            cls.ENABLE_CONV = preset["enable_conv"]
+        if "target_module" in preset:
+            cls.TARGET_REPLACE_MODULE = preset["target_module"]
+        if "target_name" in preset:
+            cls.TARGET_REPLACE_NAME = preset["target_name"]
+        if "module_algo_map" in preset:
+            cls.MODULE_ALGO_MAP = preset["module_algo_map"]
+        if "name_algo_map" in preset:
+            cls.NAME_ALGO_MAP = preset["name_algo_map"]
+        return cls
 
     def __init__(
         self,
-        text_encoder,
-        unet,
+        module: nn.Module,
         multiplier=1.0,
         lora_dim=4,
+        conv_lora_dim=4,
         alpha=1,
+        conv_alpha=1,
         use_tucker=False,
         dropout=0,
         rank_dropout=0,
         module_dropout=0,
-        network_module=LoConModule,
-        down_dim=100,
-        up_dim=50,
-        delta_iters=5,
-        decoder_blocks=4,
-        vocab_size=49408,
+        network_module: str = "locon",
+        norm_modules=NormModule,
+        train_norm=False,
+        init_only=False,
         **kwargs,
     ) -> None:
-        from ..modules.hypernet import ImgWeightGenerator, TextWeightGenerator
-
         super().__init__()
-        self.gradient_ckpt = False
+        root_kwargs = kwargs
+        if init_only:
+            self.multiplier = 1
+            self.lora_dim = 0
+            self.alpha = 1
+            self.conv_lora_dim = 0
+            self.conv_alpha = 1
+            self.dropout = 0
+            self.rank_dropout = 0
+            self.module_dropout = 0
+            self.use_tucker = False
+            self.loras = []
+            self.algo_table = {}
+            return
         self.multiplier = multiplier
         self.lora_dim = lora_dim
+
+        if not self.ENABLE_CONV:
+            conv_lora_dim = 0
+
+        self.conv_lora_dim = int(conv_lora_dim)
+        if self.conv_lora_dim and self.conv_lora_dim != self.lora_dim:
+            logger.info("Apply different lora dim for conv layer")
+            logger.info(f"Conv Dim: {conv_lora_dim}, Linear Dim: {lora_dim}")
+        elif self.conv_lora_dim == 0:
+            logger.info("Disable conv layer")
+
         self.alpha = alpha
+        self.conv_alpha = float(conv_alpha)
+        if self.conv_lora_dim and self.alpha != self.conv_alpha:
+            logger.info("Apply different alpha value for conv layer")
+            logger.info(f"Conv alpha: {conv_alpha}, Linear alpha: {alpha}")
 
         if 1 >= dropout >= 0:
             logger.info(f"Use Dropout value: {dropout}")
-        if network_module != LoConModule:
-            logger.info("HyperDreamBooth only support LoRA at this time")
-            raise NotImplementedError
-        if lora_dim * (down_dim + up_dim) > 4096:
-            logger.info(
-                "weight elements > 4096 (dim * (down_dim + up_dim)) is not recommended!"
-            )
-
         self.dropout = dropout
         self.rank_dropout = rank_dropout
         self.module_dropout = module_dropout
 
+        self.use_tucker = use_tucker
+
+        def create_single_module(
+            lora_name: str,
+            module: torch.nn.Module,
+            algo_name,
+            dim=None,
+            alpha=None,
+            use_tucker=self.use_tucker,
+            **kwargs,
+        ):
+            for k, v in root_kwargs.items():
+                if k in kwargs:
+                    continue
+                kwargs[k] = v
+
+            if train_norm and "Norm" in module.__class__.__name__:
+                return norm_modules(
+                    lora_name,
+                    module,
+                    self.multiplier,
+                    self.rank_dropout,
+                    self.module_dropout,
+                    **kwargs,
+                )
+            lora = None
+            if isinstance(module, torch.nn.Linear) and lora_dim > 0:
+                dim = dim or lora_dim
+                alpha = alpha or self.alpha
+            elif isinstance(module, torch.nn.Conv2d):
+                k_size, *_ = module.kernel_size
+                if k_size == 1 and lora_dim > 0:
+                    dim = dim or lora_dim
+                    alpha = alpha or self.alpha
+                elif conv_lora_dim > 0 or dim:
+                    dim = dim or conv_lora_dim
+                    alpha = alpha or self.conv_alpha
+                else:
+                    return None
+            else:
+                return None
+            lora = network_module_dict[algo_name](
+                lora_name,
+                module,
+                self.multiplier,
+                dim,
+                alpha,
+                self.dropout,
+                self.rank_dropout,
+                self.module_dropout,
+                use_tucker,
+                **kwargs,
+            )
+            return lora
+
+        def create_modules_(
+            prefix: str,
+            root_module: torch.nn.Module,
+            algo,
+            configs={},
+        ):
+            loras = {}
+            lora_names = []
+            for name, module in root_module.named_modules():
+                if module is root_module:
+                    continue
+                module_name = module.__class__.__name__
+                if module_name in self.MODULE_ALGO_MAP:
+                    next_config = self.MODULE_ALGO_MAP[module_name]
+                    next_algo = next_config.get("algo", algo)
+                    new_loras, new_lora_names = create_modules_(
+                        f"{prefix}_{name}", module, next_algo, next_config
+                    )
+                    for lora_name, lora in zip(new_lora_names, new_loras):
+                        if lora_name not in loras:
+                            loras[lora_name] = lora
+                            lora_names.append(lora_name)
+                    continue
+                lora_name = prefix + "." + name
+                lora_name = lora_name.replace(".", "_")
+                if lora_name in loras:
+                    continue
+
+                lora = create_single_module(lora_name, module, algo, **configs)
+                if lora is not None:
+                    loras[lora_name] = lora
+                    lora_names.append(lora_name)
+            return [loras[lora_name] for lora_name in lora_names], lora_names
+
         # create module instances
         def create_modules(
             prefix,
             root_module: torch.nn.Module,
             target_replace_modules,
             target_replace_names=[],
-        ) -> List[network_module]:
+        ) -> List:
             logger.info("Create LyCORIS Module")
             loras = []
+            next_config = {}
             for name, module in root_module.named_modules():
-                if module.__class__.__name__ in target_replace_modules:
-                    for child_name, child_module in module.named_modules():
-                        lora_name = prefix + "." + name + "." + child_name
-                        lora_name = lora_name.replace(".", "_")
-                        if child_module.__class__.__name__ == "Linear" and lora_dim > 0:
-                            lora = network_module(
-                                lora_name,
-                                child_module,
-                                self.multiplier,
-                                self.lora_dim,
-                                self.alpha,
-                                self.dropout,
-                                self.rank_dropout,
-                                self.module_dropout,
-                                use_tucker,
-                                **kwargs,
-                            )
-                        elif child_module.__class__.__name__ == "Conv2d":
-                            k_size, *_ = child_module.kernel_size
-                            if k_size == 1 and lora_dim > 0:
-                                lora = network_module(
-                                    lora_name,
-                                    child_module,
-                                    self.multiplier,
-                                    self.lora_dim,
-                                    self.alpha,
-                                    self.dropout,
-                                    self.rank_dropout,
-                                    self.module_dropout,
-                                    use_tucker,
-                                    **kwargs,
-                                )
-                            else:
-                                continue
-                        else:
-                            continue
-                        loras.append(lora)
-                elif name in target_replace_names:
+                module_name = module.__class__.__name__
+                if module_name in target_replace_modules:
+                    if module_name in self.MODULE_ALGO_MAP:
+                        next_config = self.MODULE_ALGO_MAP[module_name]
+                        algo = next_config.get("algo", network_module)
+                    else:
+                        algo = network_module
+                    loras.extend(
+                        create_modules_(f"{prefix}_{name}", module, algo, next_config)[
+                            0
+                        ]
+                    )
+                    next_config = {}
+                elif name in target_replace_names or any(
+                    re.match(t, name) for t in target_replace_names
+                ):
+                    if name in self.NAME_ALGO_MAP:
+                        next_config = self.NAME_ALGO_MAP[name]
+                        algo = next_config.get("algo", network_module)
+                    elif module_name in self.MODULE_ALGO_MAP:
+                        next_config = self.MODULE_ALGO_MAP[module_name]
+                        algo = next_config.get("algo", network_module)
+                    else:
+                        algo = network_module
                     lora_name = prefix + "." + name
                     lora_name = lora_name.replace(".", "_")
-                    if module.__class__.__name__ == "Linear" and lora_dim > 0:
-                        lora = network_module(
-                            lora_name,
-                            module,
-                            self.multiplier,
-                            self.lora_dim,
-                            self.alpha,
-                            self.dropout,
-                            self.rank_dropout,
-                            self.module_dropout,
-                            use_tucker,
-                            **kwargs,
-                        )
-                    elif module.__class__.__name__ == "Conv2d":
-                        k_size, *_ = module.kernel_size
-                        if k_size == 1 and lora_dim > 0:
-                            lora = network_module(
-                                lora_name,
-                                module,
-                                self.multiplier,
-                                self.lora_dim,
-                                self.alpha,
-                                self.dropout,
-                                self.rank_dropout,
-                                self.module_dropout,
-                                use_tucker,
-                                **kwargs,
-                            )
-                        else:
-                            continue
-                    else:
-                        continue
-                    loras.append(lora)
+                    lora = create_single_module(lora_name, module, algo, **next_config)
+                    next_config = {}
+                    if lora is not None:
+                        loras.append(lora)
             return loras
 
-        if isinstance(text_encoder, list):
-            text_encoders = text_encoder
-            use_index = True
-        else:
-            text_encoders = [text_encoder]
-            use_index = False
-
-        self.text_encoder_loras = []
-        for i, te in enumerate(text_encoders):
-            self.text_encoder_loras.extend(
-                create_modules(
-                    HyperDreamNetwork.LORA_PREFIX_TEXT_ENCODER
-                    + (f"{i+1}" if use_index else ""),
-                    te,
-                    HyperDreamNetwork.TEXT_ENCODER_TARGET_REPLACE_MODULE,
-                )
-            )
-        logger.info(
-            f"create LyCORIS for Text Encoder: "
-            f"{len(self.text_encoder_loras)} modules."
-        )
-
-        self.unet_loras = create_modules(
-            HyperDreamNetwork.LORA_PREFIX_UNET,
-            unet,
-            HyperDreamNetwork.UNET_TARGET_REPLACE_MODULE,
+        self.loras = create_modules(
+            LycorisNetwork.LORA_PREFIX,
+            module,
+            LycorisNetwork.TARGET_REPLACE_MODULE,
+            LycorisNetwork.TARGET_REPLACE_NAME,
         )
-        logger.info(f"create LyCORIS for U-Net: {len(self.unet_loras)} modules.")
+        logger.info(f"create LyCORIS: {len(self.loras)} modules.")
 
-        self.loras: list[LoConModule] = self.text_encoder_loras + self.unet_loras
-        self.img_weight_generater = ImgWeightGenerator(
-            weight_dim=(down_dim + up_dim) * lora_dim,
-            weight_num=len(self.unet_loras),
-            sample_iters=delta_iters,
-            decoder_blocks=decoder_blocks,
-        )
-        self.text_weight_generater = TextWeightGenerator(
-            weight_dim=(down_dim + up_dim) * lora_dim,
-            weight_num=len(self.text_encoder_loras),
-            sample_iters=delta_iters,
-            decoder_blocks=decoder_blocks,
-        )
-        self.split = (down_dim * lora_dim, up_dim * lora_dim)
-        self.lora_dim = lora_dim
+        algo_table = {}
+        for lora in self.loras:
+            algo_table[lora.__class__.__name__] = (
+                algo_table.get(lora.__class__.__name__, 0) + 1
+            )
+        logger.info(f"module type table: {algo_table}")
 
         self.weights_sd = None
 
         # assertion
         names = set()
-        for lora in self.text_encoder_loras + self.unet_loras:
+        for lora in self.loras:
             assert (
                 lora.lora_name not in names
             ), f"duplicated lora name: {lora.lora_name}"
             names.add(lora.lora_name)
 
-        self.checkpoint = torch.nn.Parameter(torch.tensor(0.0))
-
-        with torch.no_grad():
-            self.update_reference(
-                torch.randn(1, 3, *self.img_weight_generater.ref_size), ["test"]
-            )
-
-        # for lora in self.loras:
-        #     assert torch.all(lora.data[0]==0)
-
-    def gen_weight(self, ref_img, caption, iter=None, ensure_grad=0):
-        unet_weights = self.img_weight_generater(ref_img, iter, ensure_grad=ensure_grad)
-        unet_weights = unet_weights + self.checkpoint
-        unet_weights = [
-            i.split(self.split, dim=-1) for i in unet_weights.split(1, dim=1)
-        ]
-        text_weights = self.text_weight_generater(
-            caption, iter, ensure_grad=ensure_grad
-        )
-        text_weights = text_weights + self.checkpoint
-        text_weights = [
-            i.split(self.split, dim=-1) for i in text_weights.split(1, dim=1)
-        ]
-        return unet_weights, text_weights
-
-    def update_reference(self, ref_img, caption, iter=None):
-        # use idx for aux weight seed
-        if self.gradient_ckpt and self.training:
-            ensure_grad = torch.zeros(1, device=ref_img.device, requires_grad=True)
-            unet_weights_list, text_weights_list = checkpoint.checkpoint(
-                self.gen_weight, ref_img, caption, iter, ensure_grad
-            )
-        else:
-            unet_weights_list, text_weights_list = self.gen_weight(
-                ref_img, caption, iter
-            )
-
-        for idx, (lora, weight) in enumerate(zip(self.unet_loras, unet_weights_list)):
-            assert (
-                lora.multiplier > 0
-            ), f"multiplier must be positive: {lora.multiplier}"
-            # weight: [batch, 1, weight_dim]
-            # if weight.dim()==3:
-            #     weight = weight.squeeze(1)
-            lora.update_weights(*weight, idx)
-
-        for idx, (lora, weight) in enumerate(
-            zip(self.text_encoder_loras, text_weights_list)
-        ):
-            assert (
-                lora.multiplier > 0
-            ), f"multiplier must be positive: {lora.multiplier}"
-            # weight: [batch, 1, weight_dim]
-            # if weight.dim()==3:
-            #     weight = weight.squeeze(1)
-            lora.update_weights(*weight, idx)
-
     def set_multiplier(self, multiplier):
         self.multiplier = multiplier
-        for lora in self.text_encoder_loras + self.unet_loras:
+        for lora in self.loras:
             lora.multiplier = self.multiplier
 
     def load_weights(self, file):
         if os.path.splitext(file)[1] == ".safetensors":
             from safetensors.torch import load_file, safe_open
 
             self.weights_sd = load_file(file)
         else:
             self.weights_sd = torch.load(file, map_location="cpu")
+        missing, unexpected = self.load_state_dict(self.weights_sd, strict=False)
+        state = {}
+        if missing:
+            state["missing keys"] = missing
+        if unexpected:
+            state["unexpected keys"] = unexpected
+        return state
+
+    def apply_to(self):
+        for lora in self.loras:
+            lora.apply_to()
+            self.add_module(lora.lora_name, lora)
 
-    def apply_to(self, text_encoder, unet, apply_text_encoder=None, apply_unet=None):
         if self.weights_sd:
-            weights_has_text_encoder = weights_has_unet = False
-            for key in self.weights_sd.keys():
-                if key.startswith(HyperDreamNetwork.LORA_PREFIX_TEXT_ENCODER):
-                    weights_has_text_encoder = True
-                elif key.startswith(HyperDreamNetwork.LORA_PREFIX_UNET):
-                    weights_has_unet = True
-
-            if apply_text_encoder is None:
-                apply_text_encoder = weights_has_text_encoder
-            else:
-                assert (
-                    apply_text_encoder == weights_has_text_encoder
-                ), f"text encoder weights: {weights_has_text_encoder} but text encoder flag: {apply_text_encoder} / 重みとText Encoderのフラグが矛盾しています"
-
-            if apply_unet is None:
-                apply_unet = weights_has_unet
-            else:
-                assert (
-                    apply_unet == weights_has_unet
-                ), f"u-net weights: {weights_has_unet} but u-net flag: {apply_unet} / 重みとU-Netのフラグが矛盾しています"
-        else:
-            assert (
-                apply_text_encoder is not None and apply_unet is not None
-            ), f"internal error: flag not set"
+            # if some weights are not in state dict, it is ok because initial LoRA does nothing (lora_up is initialized by zeros)
+            info = self.load_state_dict(self.weights_sd, False)
+            logger.info(f"weights are loaded: {info}")
+
+    def is_mergeable(self):
+        return True
+
+    def restore(self):
+        for lora in self.loras:
+            lora.restore()
+
+    def merge_to(self, weight=1.0):
+        for lora in self.loras:
+            lora.merge_to(weight)
+
+    def apply_max_norm_regularization(self, max_norm_value, device):
+        key_scaled = 0
+        norms = []
+        for model in self.loras:
+            if hasattr(model, "apply_max_norm"):
+                scaled, norm = model.apply_max_norm(max_norm_value, device)
+                norms.append(norm)
+                key_scaled += scaled
 
-        if apply_text_encoder:
-            logger.info("enable LyCORIS for text encoder")
-        else:
-            self.text_encoder_loras = []
-
-        if apply_unet:
-            logger.info("enable LyCORIS for U-Net")
-        else:
-            self.unet_loras = []
+        if key_scaled == 0:
+            return key_scaled, 0, 0
 
-        for lora in self.text_encoder_loras + self.unet_loras:
-            lora.apply_to(is_hypernet=True)
+        return key_scaled, sum(norms) / len(norms), max(norms)
 
     def enable_gradient_checkpointing(self):
-        self.gradient_ckpt = True
+        # not supported
+        def make_ckpt(module):
+            if isinstance(module, torch.nn.Module):
+                module.grad_ckpt = True
+
+        self.apply(make_ckpt)
+        pass
+
+    def prepare_optimizer_params(self, lr):
+        def enumerate_params(loras):
+            params = []
+            for lora in loras:
+                params.extend(lora.parameters())
+            return params
 
-    def prepare_optimizer_params(self, text_encoder_lr, unet_lr, learning_rate):
         self.requires_grad_(True)
         all_params = []
 
-        if self.text_encoder_loras:
-            all_params.append(
-                {
-                    "params": (
-                        [
-                            p
-                            for p in self.text_weight_generater.decoder_model.parameters()
-                        ]
-                        + [
-                            p
-                            for p in self.text_weight_generater.pos_emb_proj.parameters()
-                        ]
-                        + [
-                            p
-                            for p in self.text_weight_generater.feature_proj.parameters()
-                        ]
-                        + (
-                            [
-                                p
-                                for p in self.text_weight_generater.encoder_model.parameters()
-                            ]
-                            if self.text_weight_generater.train_encoder
-                            else []
-                        )
-                    ),
-                    "lr": text_encoder_lr,
-                }
-            )
-        if self.unet_loras:
-            all_params.append(
-                {
-                    "params": (
-                        [
-                            p
-                            for p in self.img_weight_generater.decoder_model.parameters()
-                        ]
-                        + [
-                            p
-                            for p in self.img_weight_generater.pos_emb_proj.parameters()
-                        ]
-                        + [
-                            p
-                            for p in self.img_weight_generater.feature_proj.parameters()
-                        ]
-                        + (
-                            [
-                                p
-                                for p in self.img_weight_generater.encoder_model.parameters()
-                            ]
-                            if self.img_weight_generater.train_encoder
-                            else []
-                        )
-                    ),
-                    "lr": unet_lr,
-                }
-            )
+        param_data = {"params": enumerate_params(self.loras)}
+        if lr is not None:
+            param_data["lr"] = lr
+        all_params.append(param_data)
         return all_params
 
-    def prepare_grad_etc(self, text_encoder, unet):
+    def prepare_grad_etc(self, *args):
         self.requires_grad_(True)
 
-    def on_epoch_start(self, text_encoder, unet):
+    def on_epoch_start(self, *args):
         self.train()
 
-    def get_trainable_params(self):
+    def get_trainable_params(self, *args):
         return self.parameters()
 
     def save_weights(self, file, dtype, metadata):
         if metadata is not None and len(metadata) == 0:
             metadata = None
 
-        state_dict = self.img_weight_generater.state_dict()
-        if not self.img_weight_generater.train_encoder:
-            for k in self.img_weight_generater.encoder_model.state_dict().keys():
-                state_dict.pop(f"encoder_model.{k}")
-        state_dict = {f"img_weight_generater.{i}": v for i, v in state_dict.items()}
-
-        state_dict = self.text_weight_generater.state_dict()
-        if not self.text_weight_generater.train_encoder:
-            for k in self.text_weight_generater.encoder_model.state_dict().keys():
-                state_dict.pop(f"encoder_model.{k}")
-        state_dict = {f"text_weight_generater.{i}": v for i, v in state_dict.items()}
+        state_dict = self.state_dict()
 
         if dtype is not None:
             for key in list(state_dict.keys()):
                 v = state_dict[key]
                 v = v.detach().clone().to("cpu").to(dtype)
                 state_dict[key] = v
 
         if os.path.splitext(file)[1] == ".safetensors":
             from safetensors.torch import save_file
 
             # Precalculate model hashes to save time on indexing
             if metadata is None:
                 metadata = {}
-            model_hash, legacy_hash = precalculate_safetensors_hashes(
-                state_dict, metadata
-            )
-            metadata["sshs_model_hash"] = model_hash
-            metadata["sshs_legacy_hash"] = legacy_hash
-
             save_file(state_dict, file, metadata)
         else:
             torch.save(state_dict, file)
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `lycoris_lora-2.3.0.dev9/lycoris/logging.py` & `lycoris_lora-3.0.0.dev1/lycoris/logging.py`

 * *Files identical despite different names*

### Comparing `lycoris_lora-2.3.0.dev9/lycoris/modules/__init__.py` & `lycoris_lora-3.0.0.dev1/lycoris/modules/__init__.py`

 * *Files identical despite different names*

### Comparing `lycoris_lora-2.3.0.dev9/lycoris/modules/attention.py` & `lycoris_lora-3.0.0.dev1/lycoris/modules/boft.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,259 +1,232 @@
-import math
+from functools import cache
+from math import log2
 
 import torch
 import torch.nn as nn
 import torch.nn.functional as F
 
-from einops import rearrange, repeat
+from einops import rearrange
 
-from lycoris.utils import default
-from lycoris.utils.xformers_utils import XFORMERS_AVAIL, memory_efficient_attention
+from .base import LycorisBaseModule
+from ..functional import power2factorization
+from ..logging import logger
+from ..utils.bnb import LinearNF4
 
 
-class GEGLU(nn.Module):
-    def __init__(self, dim_in, dim_out):
-        super().__init__()
-        self.proj = nn.Linear(dim_in, dim_out * 2)
-
-    def forward(self, x):
-        x, gate = self.proj(x).chunk(2, dim=-1)
-        return x * F.gelu(gate)
-
-
-class FeedForward(nn.Module):
-    def __init__(self, dim, dim_out=None, mult=4, glu=False):
-        super().__init__()
-        inner_dim = int(dim * mult)
-        dim_out = default(dim_out, dim)
-        project_in = (
-            nn.Sequential(nn.Linear(dim, inner_dim), nn.GELU())
-            if not glu
-            else GEGLU(dim, inner_dim)
-        )
-
-        self.net = nn.Sequential(project_in, nn.Linear(inner_dim, dim_out))
-        # nn.init.constant_(self.net[-1].weight, 0)
-        # nn.init.constant_(self.net[-1].bias, 0)
-
-    def forward(self, x):
-        return self.net(x)
-
-
-def vanilla_attention(q, k, v, mask, scale=None):
-    if scale is None:
-        scale = math.sqrt(q.size(-1))
-    scores = torch.bmm(q, k.transpose(-1, -2)) / scale
-    if mask is not None:
-        mask = rearrange(mask, "b ... -> b (...)")
-        max_neg_value = -torch.finfo(scores.dtype).max
-        mask = repeat(mask, "b j -> (b h) j", h=q.size(-3))
-        scores = scores.masked_fill(~mask, max_neg_value)
-    p_attn = F.softmax(scores, dim=-1)
-    return torch.bmm(p_attn, v)
-
-
-MEMORY_LAYOUTS = {
-    "torch": (
-        "b n (h d) -> b h n d",
-        "b h n d -> b n (h d)",
-        lambda x: (1, x, 1, 1),
-    ),
-    "xformers": (
-        "b n (h d) -> b n h d",
-        "b n h d -> b n (h d)",
-        lambda x: (1, 1, x, 1),
-    ),
-    "vanilla": (
-        "b n (h d) -> b h n d",
-        "b h n d -> b n (h d)",
-        lambda x: (1, x, 1, 1),
-    ),
-}
-ATTN_FUNCTION = {
-    "vanilla": vanilla_attention,
-    "torch": getattr(F, "scaled_dot_product_attention", None),
-    "xformers": memory_efficient_attention,
-}
-
-
-class Attention(nn.Module):
-    """
-    Attention Class without norm and residual
-    (You need to wrap them by your self)
-    """
-
-    def __init__(
-        self,
-        in_ch,
-        context_ch=None,
-        heads=8,
-        head_ch=64,
-        self_cross=False,
-        double_attn=False,
-        single_kv_head=False,
-        attn_backend="torch",
-        cosine_attn=False,
-        qk_head_ch=-1,
-    ):
-        super().__init__()
-        if heads == -1:
-            assert in_ch % head_ch == 0
-            heads = in_ch // head_ch
-        if head_ch == -1:
-            assert in_ch % heads == 0
-            head_ch = in_ch // heads
-        if qk_head_ch == -1:
-            qk_head_ch = head_ch
-        q_ch = heads * qk_head_ch
-        k_ch = (1 if single_kv_head else heads) * qk_head_ch
-        v_ch = (1 if single_kv_head else heads) * head_ch
-        inner_ch = heads * head_ch
-        assert inner_ch == in_ch
-        use_context = context_ch is not None
-        context_ch = default(context_ch, in_ch)
-
-        if attn_backend == "xformers":
-            assert XFORMERS_AVAIL
-        if attn_backend == "torch":
-            assert torch.version.__version__ >= "2.0.0"
-
-        self.heads = heads
-        self.self_cross = self_cross
-        self.double_attn = double_attn
-        self.single_kv_head = single_kv_head
-        self.attn = ATTN_FUNCTION[attn_backend]
-        self.memory_layout = MEMORY_LAYOUTS[attn_backend]
-        self.cosine_attn = cosine_attn
-
-        if cosine_attn:
-            self.scale = nn.Parameter(
-                torch.ones(MEMORY_LAYOUTS[attn_backend][2](heads))
-            )
-        else:
-            self.scale = None
+@cache
+def log_butterfly_factorize(dim, factor, result):
+    logger.info(
+        f"Use BOFT({int(log2(result[1]))}, {result[0]//2})"
+        f" (equivalent to factor={result[0]}) "
+        f"for {dim=} and {factor=}"
+    )
 
-        self.q = nn.Linear(in_ch, q_ch, bias=False)
-        if self_cross and use_context:
-            self.k = nn.Linear(in_ch, k_ch, bias=False)
-            self.v = nn.Linear(in_ch, v_ch, bias=False)
-            self.ck = nn.Linear(context_ch, k_ch, bias=False)
-            self.cv = nn.Linear(context_ch, v_ch, bias=False)
-        else:
-            assert double_attn == False
-            self.k = nn.Linear(context_ch, k_ch, bias=False)
-            self.v = nn.Linear(context_ch, v_ch, bias=False)
 
-        if double_attn:
-            self.out = nn.Linear(inner_ch * 2, in_ch)
-        else:
-            self.out = nn.Linear(inner_ch, in_ch)
+def butterfly_factor(dimension: int, factor: int = -1) -> tuple[int, int]:
+    m, n = power2factorization(dimension, factor)
 
-    def forward(self, x: torch.Tensor, context=None, mask=None):
-        # Input Projection
-        heads = self.heads
-        q = self.q(x)
-        ck = cv = None
-        if self.self_cross:
-            k = self.k(x)
-            v = self.v(x)
-            if context is not None:
-                ck = self.ck(context)
-                cv = self.cv(context)
-                if not self.double_attn:
-                    k = torch.concat([k, ck], dim=1)
-                    v = torch.concat([v, cv], dim=1)
-        else:
-            ctx = default(context, x)
-            k = self.k(ctx)
-            v = self.v(ctx)
-
-        # Rearrange for Attention
-        q = rearrange(q, self.memory_layout[0], h=heads)
-        if self.single_kv_head:
-            k = k.unsqueeze(1)
-            v = v.unsqueeze(1)
-
-            b, _, seq, _ = k.shape
-            k = k.expand(b, heads, seq, k.size(3))
-            v = v.expand(b, heads, seq, v.size(3))
-        else:
-            k = rearrange(k, self.memory_layout[0], h=heads)
-            v = rearrange(v, self.memory_layout[0], h=heads)
+    if n == 0:
+        raise ValueError(
+            f"It is impossible to decompose {dimension} with factor {factor} under BOFT constrains."
+        )
 
-        if self.cosine_attn:
-            q = (F.normalize(q, dim=-1) * math.sqrt(q.size(-1))).to(v.dtype)
-            k = (F.normalize(k, dim=-1) * self.scale).to(v.dtype)
-            if ck is not None and self.double_attn:
-                ck = (F.normalize(ck, dim=-1) * self.scale).to(v.dtype)
-
-        # Attention
-        out = self.attn(q.contiguous(), k.contiguous(), v.contiguous(), mask)
-        out = rearrange(out, self.memory_layout[1], h=heads)
-        if self.double_attn:
-            out2 = self.attn(q.contiguous(), ck.contiguous(), cv.contiguous(), mask)
-            out2 = rearrange(out2, self.memory_layout[1], h=heads)
-            out = torch.cat([out, out2], dim=-1)
+    log_butterfly_factorize(dimension, factor, (m, n))
+    return m, n
 
-        # Output Projection
-        return self.out(out)
 
+class ButterflyOFTModule(LycorisBaseModule):
+    support_module = {
+        "linear",
+        "conv1d",
+        "conv2d",
+        "conv3d",
+    }
 
-class TransformerBlock(nn.Module):
     def __init__(
         self,
-        dim,
-        n_heads,
-        d_head,
-        context_dim=None,
-        gated_ff=True,
-        self_cross=False,
-        single_kv_head=False,
-        attn_backend="torch",
-        cosine_attn=False,
-        qk_head_ch=-1,
-        disable_self_attn=False,
-        single_attn=False,
+        lora_name,
+        org_module: nn.Module,
+        multiplier=1.0,
+        lora_dim=4,
+        alpha=1,
+        dropout=0.0,
+        rank_dropout=0.0,
+        module_dropout=0.0,
+        use_tucker=False,
+        use_scalar=False,
+        rank_dropout_scale=False,
+        constrain=0,
+        rescaled=False,
+        bypass_mode=False,
+        **kwargs,
     ):
-        super().__init__()
-        self.single_attn = single_attn
-        self.disable_self_attn = disable_self_attn or single_attn
-
-        self.norm1 = nn.LayerNorm(dim)
-        self.attn1 = Attention(
-            dim,
-            context_dim if self.disable_self_attn else None,
-            n_heads,
-            d_head,
-            self_cross,
-            single_kv_head,
-            attn_backend,
-            cosine_attn,
-            qk_head_ch,
+        super().__init__(
+            lora_name,
+            org_module,
+            multiplier,
+            dropout,
+            rank_dropout,
+            module_dropout,
+            rank_dropout_scale,
+            bypass_mode,
         )
-        if not single_attn:
-            self.norm2 = nn.LayerNorm(dim)
-            self.attn2 = Attention(
-                dim,
-                context_dim,
-                n_heads,
-                d_head,
-                self_cross,
-                single_kv_head,
-                attn_backend,
-                cosine_attn,
-                qk_head_ch,
-            )
-        self.norm3 = nn.LayerNorm(dim)
-        self.ff = FeedForward(dim, glu=gated_ff)
+        if self.module_type not in self.support_module:
+            raise ValueError(f"{self.module_type} is not supported in BOFT algo.")
 
-    def forward(self, x, context=None):
-        x = (
-            self.attn1(
-                self.norm1(x), context=context if self.disable_self_attn else None
-            )
-            + x
+        out_dim = self.dim
+        b, m_exp = butterfly_factor(out_dim, lora_dim)
+        self.block_size = b
+        self.block_num = m_exp
+        # BOFT(m, b)
+        self.boft_b = b
+        self.boft_m = sum(int(i) for i in f"{m_exp-1:b}") + 1
+        # block_num > block_size
+        self.rescaled = rescaled
+        self.constrain = constrain * out_dim
+        self.register_buffer("alpha", torch.tensor(constrain))
+        self.oft_blocks = nn.Parameter(
+            torch.zeros(self.boft_m, self.block_num, self.block_size, self.block_size)
         )
-        if not self.single_attn and (context is not None or self.attn2.self_cross):
-            x = self.attn2(self.norm2(x), context=context) + x
-        x = self.ff(self.norm3(x)) + x
-        return x
+        if rescaled:
+            self.rescale = nn.Parameter(
+                torch.ones(out_dim, *(1 for _ in range(org_module.weight.dim() - 1)))
+            )
+
+    @property
+    def I(self):
+        return torch.eye(self.block_size, device=self.device)
+
+    def get_r(self):
+        I = self.I
+        # for Q = -Q^T
+        q = self.oft_blocks - self.oft_blocks.transpose(-1, -2)
+        normed_q = q
+        # Diag OFT style constrain
+        if self.constrain > 0:
+            q_norm = torch.norm(q) + 1e-8
+            if q_norm > self.constrain:
+                normed_q = q * self.constrain / q_norm
+        # use float() to prevent unsupported type
+        r = (I + normed_q) @ (I - normed_q).float().inverse()
+        return r
+
+    def make_weight(self, scale=1, device=None, diff=False):
+        m = self.boft_m
+        b = self.boft_b
+        r_b = b // 2
+        r = self.get_r()
+        inp = self.org_weight.to(device, dtype=r.dtype)
+
+        for i in range(m):
+            bi = r[i]  # b_num, b_size, b_size
+            if i == 0:
+                # Apply multiplier/scale and rescale into first weight
+                if self.rescaled:
+                    bi = bi * self.rescale
+            bi = bi * scale - scale * self.I + (self.I if diff else 0)
+            inp = rearrange(inp, "(c g k) ... -> (c k g) ...", g=2, k=2**i * r_b)
+            inp = rearrange(inp, "(d b) ... -> d b ...", b=b)
+            inp = torch.einsum("b i j, b j ... -> b i ...", bi, inp)
+            inp = rearrange(inp, "d b ... -> (d b) ...")
+            inp = rearrange(inp, "(c k g) ... -> (c g k) ...", g=2, k=2**i * r_b)
+
+        return inp
+
+    def get_diff_weight(self, multiplier=1, shape=None, device=None):
+        diff = self.make_weight(scale=multiplier, device=device, diff=True)
+        if shape is not None:
+            diff = diff.view(shape)
+        return diff
+
+    def get_merged_weight(self, multiplier=1, shape=None, device=None):
+        diff = self.make_weight(scale=multiplier, device=device)
+        if shape is not None:
+            diff = diff.view(shape)
+        return diff, None
+
+    @torch.no_grad()
+    def apply_max_norm(self, max_norm, device=None):
+        orig_norm = self.oft_blocks.to(device).norm()
+        norm = torch.clamp(orig_norm, max_norm / 2)
+        desired = torch.clamp(norm, max=max_norm)
+        ratio = desired / norm
+
+        scaled = norm != desired
+        if scaled:
+            self.oft_blocks *= ratio
+
+        return scaled, orig_norm * ratio
+
+    def _bypass_forward(self, x, scale=1, diff=False):
+        m = self.boft_m
+        b = self.boft_b
+        r_b = b // 2
+        r = self.get_r()
+        inp = self.org_forward(x)
+
+        for i in range(m):
+            bi = r[i]  # b_num, b_size, b_size
+            if i == 0:
+                # Apply multiplier/scale and rescale into first weight
+                if self.rescaled:
+                    bi = bi * self.rescale
+            bi = bi * scale - scale * self.I + (self.I if diff else 0)
+            inp = rearrange(inp, "... (c g k) ->... (c k g)", g=2, k=2**i * r_b)
+            inp = rearrange(inp, "... (d b) -> ... d b", b=b)
+            inp = torch.einsum("b i j, ... b j -> ... b i", bi, inp)
+            inp = rearrange(inp, "... d b -> ... (d b)")
+            inp = rearrange(inp, "... (c k g) -> ... (c g k)", g=2, k=2**i * r_b)
+
+        return inp
+
+    def bypass_forward_diff(self, x, scale=1):
+        return self._bypass_forward(x, scale, diff=True)
+
+    def bypass_forward(self, x, scale=1):
+        return self._bypass_forward(x, scale, diff=False)
+
+    def forward(self, x, *args, **kwargs):
+        if self.module_dropout and self.training:
+            if torch.rand(1) < self.module_dropout:
+                return self.org_forward(x)
+        scale = self.multiplier
+
+        if self.bypass_mode:
+            return self.bypass_forward(x, scale)
+        else:
+            w = self.make_weight(scale, x.device)
+            kw_dict = self.kw_dict | {"weight": w, "bias": self.org_module[0].bias}
+            return self.op(x, **kw_dict)
+
+
+if __name__ == "__main__":
+    base = nn.Linear(128, 128).cuda()
+    boft = ButterflyOFTModule(
+        "test", base, 1, 4, 1, weight_decompose=True, factor=8
+    ).cuda()
+    print(boft)
+    test_input = torch.randn(1, 77, 128).cuda()
+    test_output = boft(test_input)
+    torch.sum(test_output).backward()
+    print(test_output.shape)
+
+    base_4bit = LinearNF4(128, 128)
+    base_4bit.load_state_dict(base.state_dict())
+    base_4bit.cuda()
+    qboft = ButterflyOFTModule(
+        "test", base_4bit, 1, 4, 1, weight_decompose=False
+    ).cuda()
+    print(qboft)
+    test_output = qboft(test_input)
+    torch.sum(test_output).backward()
+    print(test_output.shape)
+
+    base = nn.Conv2d(128, 128, 3, 1, 1)
+    boft = ButterflyOFTModule(
+        "test", base, 1, 4, 1, weight_decompose=True, use_tucker=True
+    )
+    print(boft)
+    test_input = torch.randn(1, 128, 16, 16)
+    test_output = boft(test_input)
+    torch.sum(test_output).backward()
+    print(test_output.shape)
```

### Comparing `lycoris_lora-2.3.0.dev9/lycoris/modules/base.py` & `lycoris_lora-3.0.0.dev1/lycoris/modules/base.py`

 * *Files 7% similar despite different names*

```diff
@@ -57,14 +57,15 @@
         else:
             return super().state_dict(
                 *args, destination=destination, prefix=prefix, keep_vars=keep_vars
             )
 
 
 class LycorisBaseModule(ModuleCustomSD):
+    dtype_tensor: torch.Tensor
     support_module = {}
 
     def __init__(
         self,
         lora_name,
         org_module: nn.Module,
         multiplier=1.0,
@@ -146,30 +147,53 @@
             self.op = F.group_norm
             self.group_num = org_module.num_groups
             self.dim = org_module.num_channels
             self.kw_dict = {"num_groups": org_module.num_groups, "eps": org_module.eps}
         else:
             self.module_type = "unknown"
 
+        self.register_buffer("dtype_tensor", torch.tensor(0.0), persistent=False)
+
         self.is_bnb = False
         if isinstance(org_module, QuantLinears):
             if not bypass_mode:
                 log_bypass()
             self.is_bnb = True
             bypass_mode = True
         self.bypass_mode = bypass_mode
         self.dropout = dropout
         self.rank_dropout = rank_dropout
         self.rank_dropout_scale = rank_dropout_scale
         self.module_dropout = module_dropout
 
+        ## Dropout things
+        # Since LoKr/LoHa/OFT/BOFT are hard to follow the rank_dropout definition from kohya
+        # We redefine the dropout procedure here.
+        # g(x) = WX + drop(Brank_drop(AX)) for LoCon(lora), bypass
+        # g(x) = WX + drop(ΔWX) for any algo except LoCon(lora), bypass
+        # g(x) = (W + Brank_drop(A))X for LoCon(lora), rebuid
+        # g(x) = (W + rank_drop(ΔW))X for any algo except LoCon(lora), rebuild
+        self.drop = nn.Identity() if dropout == 0.0 else nn.Dropout(dropout)
+        self.rank_drop = (
+            nn.Identity() if rank_dropout == 0.0 else nn.Dropout(rank_dropout)
+        )
+
         self.multiplier = multiplier
+        self.org_forward = org_module.forward
         self.org_module = [org_module]
 
     @property
+    def dtype(self):
+        return self.dtype_tensor.dtype
+
+    @property
+    def device(self):
+        return self.dtype_tensor.device
+
+    @property
     def org_weight(self):
         return self.org_module[0].weight
 
     @org_weight.setter
     def org_weight(self, value):
         self.org_module[0].weight.data.copy_(value)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `lycoris_lora-2.3.0.dev9/lycoris/modules/boft.py` & `lycoris_lora-3.0.0.dev1/lycoris/modules/diag_oft.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,58 +1,31 @@
 from functools import cache
-from math import log2
 
 import torch
 import torch.nn as nn
 import torch.nn.functional as F
 
 from einops import rearrange
 
 from .base import LycorisBaseModule
+from ..functional import factorization
 from ..logging import logger
 from ..utils.bnb import LinearNF4
 
 
 @cache
-def log_butterfly_factorize(dim, factor, result):
+def log_oft_factorize(dim, factor, num, bdim):
     logger.info(
-        f"Use BOFT({int(log2(result[1]))}, {result[0]//2})"
-        f" (equivalent to factor={result[0]}) "
-        f"for {dim=} and {factor=}"
+        f"Use OFT(block num: {num}, block dim: {bdim})"
+        f" (equivalent to lora_dim={num}) "
+        f"for {dim=} and lora_dim={factor=}"
     )
 
 
-def butterfly_factor(dimension: int, factor: int = -1) -> tuple[int, int]:
-    """
-    m = 2k
-    n = 2**p
-    m*n = dim
-    """
-
-    # Find the first solution and check if it is even doable
-    m = n = 0
-    while m <= factor:
-        m += 2
-        while dimension % m != 0 and m < dimension:
-            m += 2
-        if m > factor:
-            break
-        if sum(int(i) for i in f"{dimension//m:b}") == 1:
-            n = dimension // m
-
-    if n == 0:
-        raise ValueError(
-            f"It is impossible to decompose {dimension} with factor {factor} under BOFT constrains."
-        )
-
-    log_butterfly_factorize(dimension, factor, (dimension // n, n))
-    return dimension // n, n
-
-
-class ButterflyOFTModule(LycorisBaseModule):
+class DiagOFTModule(LycorisBaseModule):
     support_module = {
         "linear",
         "conv1d",
         "conv2d",
         "conv3d",
     }
 
@@ -81,74 +54,70 @@
             dropout,
             rank_dropout,
             module_dropout,
             rank_dropout_scale,
             bypass_mode,
         )
         if self.module_type not in self.support_module:
-            raise ValueError(f"{self.module_type} is not supported in BOFT algo.")
+            raise ValueError(f"{self.module_type} is not supported in Diag-OFT algo.")
 
         out_dim = self.dim
-        b, m_exp = butterfly_factor(out_dim, lora_dim)
-        self.block_size = b
-        self.block_num = m_exp
-        # BOFT(m, b)
-        self.boft_b = b
-        self.boft_m = sum(int(i) for i in f"{m_exp-1:b}") + 1
+        self.block_size, self.block_num = factorization(out_dim, lora_dim)
         # block_num > block_size
         self.rescaled = rescaled
         self.constrain = constrain * out_dim
         self.register_buffer("alpha", torch.tensor(constrain))
         self.oft_blocks = nn.Parameter(
-            torch.zeros(self.boft_m, self.block_num, self.block_size, self.block_size)
+            torch.zeros(self.block_num, self.block_size, self.block_size)
         )
         if rescaled:
             self.rescale = nn.Parameter(
                 torch.ones(out_dim, *(1 for _ in range(org_module.weight.dim() - 1)))
             )
 
+        log_oft_factorize(
+            dim=out_dim,
+            factor=lora_dim,
+            num=self.block_num,
+            bdim=self.block_size,
+        )
+
     @property
     def I(self):
-        return torch.eye(self.block_size, device=next(self.parameters()).device)
+        return torch.eye(self.block_size, device=self.device)
 
     def get_r(self):
         I = self.I
         # for Q = -Q^T
-        q = self.oft_blocks - self.oft_blocks.transpose(-1, -2)
+        q = self.oft_blocks - self.oft_blocks.transpose(1, 2)
         normed_q = q
-        # Diag OFT style constrain
         if self.constrain > 0:
             q_norm = torch.norm(q) + 1e-8
             if q_norm > self.constrain:
                 normed_q = q * self.constrain / q_norm
         # use float() to prevent unsupported type
         r = (I + normed_q) @ (I - normed_q).float().inverse()
         return r
 
     def make_weight(self, scale=1, device=None, diff=False):
-        m = self.boft_m
-        b = self.boft_b
-        r_b = b // 2
         r = self.get_r()
-        inp = self.org_weight.to(device, dtype=r.dtype)
-
-        for i in range(m):
-            bi = r[i]  # b_num, b_size, b_size
-            if i == 0:
-                # Apply multiplier/scale and rescale into first weight
-                if self.rescaled:
-                    bi = bi * self.rescale
-            bi = bi * scale - scale * self.I + (self.I if diff else 0)
-            inp = rearrange(inp, "(c g k) ... -> (c k g) ...", g=2, k=2**i * r_b)
-            inp = rearrange(inp, "(d b) ... -> d b ...", b=b)
-            inp = torch.einsum("b i j, b j ... -> b i ...", bi, inp)
-            inp = rearrange(inp, "d b ... -> (d b) ...")
-            inp = rearrange(inp, "(c k g) ... -> (c g k) ...", g=2, k=2**i * r_b)
-
-        return inp
+        _, *shape = self.org_weight.shape
+        org_weight = self.org_weight.to(device, dtype=r.dtype)
+        org_weight = org_weight.view(self.block_num, self.block_size, *shape)
+        # Init R=0, so add I on it to ensure the output of step0 is original model output
+        weight = torch.einsum(
+            "k n m, k n ... -> k m ...",
+            self.rank_drop(r * scale) - scale * self.I + (0 if diff else self.I),
+            org_weight,
+        ).view(-1, *shape)
+        if self.rescaled:
+            weight = self.rescale * weight
+            if diff:
+                weight = weight + (self.rescale - 1) * org_weight
+        return weight
 
     def get_diff_weight(self, multiplier=1, shape=None, device=None):
         diff = self.make_weight(scale=multiplier, device=device, diff=True)
         if shape is not None:
             diff = diff.view(shape)
         return diff
 
@@ -168,42 +137,44 @@
         scaled = norm != desired
         if scaled:
             self.oft_blocks *= ratio
 
         return scaled, orig_norm * ratio
 
     def _bypass_forward(self, x, scale=1, diff=False):
-        m = self.boft_m
-        b = self.boft_b
-        r_b = b // 2
         r = self.get_r()
-        inp = self.org_forward(x)
-
-        for i in range(m):
-            bi = r[i]  # b_num, b_size, b_size
-            if i == 0:
-                # Apply multiplier/scale and rescale into first weight
-                if self.rescaled:
-                    bi = bi * self.rescale
-            bi = bi * scale - scale * self.I + (self.I if diff else 0)
-            inp = rearrange(inp, "... (c g k) ->... (c k g)", g=2, k=2**i * r_b)
-            inp = rearrange(inp, "... (d b) -> ... d b", b=b)
-            inp = torch.einsum("b i j, ... b j -> ... b i", bi, inp)
-            inp = rearrange(inp, "... d b -> ... (d b)")
-            inp = rearrange(inp, "... (c k g) -> ... (c g k)", g=2, k=2**i * r_b)
-
-        return inp
+        org_out = self.org_forward(x)
+        if self.op == F.conv2d:
+            org_out = org_out.transpose(1, -1)
+        *shape, _ = org_out.shape
+        org_out = org_out.view(*shape, self.block_num, self.block_size)
+        mask = neg_mask = 1
+        if self.dropout != 0 and self.training:
+            mask = torch.ones_like(org_out)
+            mask = self.drop(mask)
+            neg_mask = torch.max(mask) - mask
+        oft_out = torch.einsum(
+            "k n m, ... k n -> ... k m",
+            r * scale * mask + (1 - scale) * self.I * neg_mask,
+            org_out,
+        )
+        if diff:
+            out = out - org_out
+        out = oft_out.view(*shape, -1)
+        if self.op == F.conv2d:
+            out = out.transpose(1, -1)
+        return out
 
     def bypass_forward_diff(self, x, scale=1):
         return self._bypass_forward(x, scale, diff=True)
 
     def bypass_forward(self, x, scale=1):
         return self._bypass_forward(x, scale, diff=False)
 
-    def forward(self, x, *args, **kwargs):
+    def forward(self, x: torch.Tensor, *args, **kwargs):
         if self.module_dropout and self.training:
             if torch.rand(1) < self.module_dropout:
                 return self.org_forward(x)
         scale = self.multiplier
 
         if self.bypass_mode:
             return self.bypass_forward(x, scale)
@@ -211,33 +182,30 @@
             w = self.make_weight(scale, x.device)
             kw_dict = self.kw_dict | {"weight": w, "bias": self.org_module[0].bias}
             return self.op(x, **kw_dict)
 
 
 if __name__ == "__main__":
     base = nn.Linear(128, 128).cuda()
-    lokr = ButterflyOFTModule("test", base, 1, 4, 1, weight_decompose=True).cuda()
-    print(lokr)
-    test_input = torch.randn(1, 128).cuda()
-    test_output = lokr(test_input)
+    doft = DiagOFTModule("test", base, 1, 4, 1, weight_decompose=True, factor=8).cuda()
+    print(doft)
+    test_input = torch.randn(1, 77, 128).cuda()
+    test_output = doft(test_input)
+    torch.sum(test_output).backward()
     print(test_output.shape)
-    print(F.mse_loss(test_output, lokr.bypass_forward(test_input)))
 
     base_4bit = LinearNF4(128, 128)
     base_4bit.load_state_dict(base.state_dict())
     base_4bit.cuda()
-    qlocon = ButterflyOFTModule(
-        "test", base_4bit, 1, 4, 1, weight_decompose=False
-    ).cuda()
-    print(qlocon)
-    test_input = torch.randn(1, 128).cuda()
-    test_output = qlocon(test_input)
+    qdoft = DiagOFTModule("test", base_4bit, 1, 4, 1, weight_decompose=False).cuda()
+    print(qdoft)
+    test_output = qdoft(test_input)
+    torch.sum(test_output).backward()
     print(test_output.shape)
 
     base = nn.Conv2d(128, 128, 3, 1, 1)
-    lokr = ButterflyOFTModule(
-        "test", base, 1, 4, 1, weight_decompose=True, use_tucker=True
-    )
-    print(lokr)
+    doft = DiagOFTModule("test", base, 1, 4, 1, weight_decompose=True, use_tucker=True)
+    print(doft)
     test_input = torch.randn(1, 128, 16, 16)
-    test_output = lokr(test_input)
+    test_output = doft(test_input)
+    torch.sum(test_output).backward()
     print(test_output.shape)
```

### Comparing `lycoris_lora-2.3.0.dev9/lycoris/modules/dylora.py` & `lycoris_lora-3.0.0.dev1/lycoris/modules/dylora.py`

 * *Files identical despite different names*

### Comparing `lycoris_lora-2.3.0.dev9/lycoris/modules/full.py` & `lycoris_lora-3.0.0.dev1/lycoris/modules/full.py`

 * *Files 20% similar despite different names*

```diff
@@ -37,23 +37,36 @@
             module_dropout,
             rank_dropout_scale,
             bypass_mode,
         )
         if self.module_type not in self.support_module:
             raise ValueError(f"{self.module_type} is not supported in Full algo.")
 
+        if self.is_bnb:
+            raise ValueError(
+                "Quant Linear is not supported and meaningless in Full algo."
+            )
+
         if self.bypass_mode:
             raise ValueError("bypass mode is not supported in Full algo.")
 
         self.weight = nn.Parameter(torch.zeros_like(org_module.weight))
         if org_module.bias is not None:
             self.bias = nn.Parameter(torch.zeros_like(org_module.bias))
         else:
             self.bias = None
 
+    @property
+    def org_weight(self):
+        return self._org_weight[0]
+
+    @org_weight.setter
+    def org_weight(self, value):
+        self.org_module[0].weight.data.copy_(value)
+
     def apply_to(self, **kwargs):
         self.org_forward = self.org_module[0].forward
         self.org_module[0].forward = self.forward
         self.weight.data.add_(self.org_module[0].weight.data)
         self._org_weight = [self.org_module[0].weight.data.cpu().clone()]
         delattr(self.org_module[0], "weight")
         if self.org_module[0].bias is not None:
@@ -81,40 +94,48 @@
     ):
         diff_weight = state_dict["diff"]
         self.weight.data.add_(diff_weight)
         if "diff_b" in state_dict:
             diff_bias = state_dict["diff_b"]
             self.bias.data.add_(diff_bias)
 
-    def make_weight(self, scale=1, device=None, original=False):
-        if original:
-            weight = self._org_weight[0].to(device, dtype=self.weight.dtype)
-            if self.org_bias is not None:
-                bias = self.org_bias[0].to(device, dtype=self.bias.dtype)
-            else:
-                bias = None
-            return weight, bias
+    def make_weight(self, scale=1, device=None):
         drop = (
             torch.rand(self.dim, device=device) > self.rank_dropout
             if self.rank_dropout and self.training
             else 1
         )
         if drop != 1 or scale != 1:
-            org_weight = self.org_module[0].weight.to(device, dtype=self.weight.dtype)
-            diff = self.weight.to(device) - org_weight
-            weight = diff * drop * scale + org_weight
-            if self.bias is not None:
-                org_bias = self.org_module[0].bias.to(device, dtype=self.bias.dtype)
-                diff_b = self.bias.to(device) - org_bias
-                bias = diff_b * drop * scale + org_bias
+            diff_w, diff_b = self.get_diff_weight(scale, device=device)
+            weight = self.org_module[0].weight + diff_w * drop
+            bias = self.org_module[0].bias + diff_b * drop
         else:
             weight = self.weight
             bias = self.bias
         return weight, bias
 
+    def get_diff_weight(self, multiplier=1, shape=None, device=None):
+        org_weight = self.org_module[0].weight.to(device, dtype=self.weight.dtype)
+        diff = self.weight.to(device) - org_weight
+        diff_b = None
+        if shape:
+            diff = diff.view(shape)
+        if self.bias is not None:
+            org_bias = self.org_module[0].bias.to(device, dtype=self.bias.dtype)
+            diff_b = self.bias.to(device) - org_bias
+        if device is not None:
+            diff = diff.to(device)
+            if self.bias is not None:
+                diff_b = diff_b.to(device)
+        if multiplier != 1:
+            diff = diff * multiplier
+            if diff_b is not None:
+                diff_b = diff_b * multiplier
+        return diff * multiplier, diff_b
+
     def get_merged_weight(self, multiplier=1, shape=None, device=None):
         weight, bias = self.make_weight(multiplier, device)
         if shape is not None:
             weight = weight.view(shape)
             if bias is not None:
                 bias = bias.view(shape[0], 1)
         return weight, bias
@@ -124,11 +145,31 @@
             self.module_dropout
             and self.training
             and torch.rand(1) < self.module_dropout
         ):
             original = True
         else:
             original = False
+        if original:
+            return self.org_forward(x)
         scale = self.multiplier
-        weight, bias = self.make_weight(scale, x.device, original=original)
+        weight, bias = self.make_weight(scale, x.device)
         kw_dict = self.kw_dict | {"weight": weight, "bias": bias}
         return self.op(x, **kw_dict)
+
+
+if __name__ == "__main__":
+    base = nn.Linear(128, 128).cuda()
+    full = FullModule("test", base, 1, 4, 1, weight_decompose=True, factor=8).cuda()
+    print(full)
+    test_input = torch.randn(1, 77, 128).cuda()
+    test_output = full(test_input)
+    torch.sum(test_output).backward()
+    print(test_output.shape)
+
+    base = nn.Conv2d(128, 128, 3, 1, 1)
+    full = FullModule("test", base, 1, 4, 1, weight_decompose=True, use_tucker=True)
+    print(full)
+    test_input = torch.randn(1, 128, 16, 16)
+    test_output = full(test_input)
+    torch.sum(test_output).backward()
+    print(test_output.shape)
```

### Comparing `lycoris_lora-2.3.0.dev9/lycoris/modules/glokr.py` & `lycoris_lora-3.0.0.dev1/lycoris/modules/locon.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,310 +1,304 @@
 import math
+from functools import cache
 
 import torch
 import torch.nn as nn
 import torch.nn.functional as F
 
-from .base import ModuleCustomSD
-
-
-def factorization(dimension: int, factor: int = -1) -> tuple[int, int]:
-    """
-    return a tuple of two value of input dimension decomposed by the number closest to factor
-    second value is higher or equal than first value.
-
-    In LoRA with Kroneckor Product, first value is a value for weight scale.
-    secon value is a value for weight.
-
-    Becuase of non-commutative property, A⊗B ≠ B⊗A. Meaning of two matrices is slightly different.
-
-    examples)
-    factor
-        -1               2                4               8               16               ...
-    127 -> 127, 1   127 -> 127, 1    127 -> 127, 1   127 -> 127, 1   127 -> 127, 1
-    128 -> 16, 8    128 -> 64, 2     128 -> 32, 4    128 -> 16, 8    128 -> 16, 8
-    250 -> 25, 10   250 -> 125, 2    250 -> 125, 2   250 -> 50, 5   250 -> 25, 10
-    360 -> 45, 8    360 -> 180, 2    360 -> 90, 4    360 -> 45, 8    360 -> 45, 8
-    512 -> 32, 16   512 -> 256, 2    512 -> 128, 4   512 -> 64, 8    512 -> 32, 16
-    1024 -> 32, 32  1024 -> 512, 2   1024 -> 256, 4  1024 -> 128, 8  1024 -> 64, 16
-    """
-
-    if factor > 0 and (dimension % factor) == 0:
-        m = factor
-        n = dimension // factor
-        return m, n
-    if factor == -1:
-        factor = dimension
-    m, n = 1, dimension
-    length = m + n
-    while m < n:
-        new_m = m + 1
-        while dimension % new_m != 0:
-            new_m += 1
-        new_n = dimension // new_m
-        if new_m + new_n > length or new_m > factor:
-            break
-        else:
-            m, n = new_m, new_n
-    if m > n:
-        n, m = m, n
-    return m, n
-
-
-def make_weight_tucker(t, wa, wb):
-    rebuild2 = torch.einsum("i j k l, i p, j r -> p r k l", t, wa, wb)  # [c, d, k1, k2]
-    return rebuild2
-
-
-def make_kron(w1, w2, scale):
-    if len(w2.shape) == 4:
-        w1 = w1.unsqueeze(2).unsqueeze(2)
-    w2 = w2.contiguous()
-    rebuild = torch.kron(w1, w2)
-
-    return rebuild * scale
-
-
-class LokrModule(ModuleCustomSD):
-    """
-    modifed from kohya-ss/sd-scripts/networks/lora:LoRAModule
-        and from KohakuBlueleaf/LyCORIS/lycoris:loha:LoHaModule
-        and from KohakuBlueleaf/LyCORIS/lycoris:locon:LoconModule
-    """
+from .base import LycorisBaseModule
+from ..functional.general import rebuild_tucker
+from ..logging import logger
+from ..utils.bnb import LinearNF4
+
+
+@cache
+def log_wd():
+    return logger.warning(
+        "Using weight_decompose=True with LoRA (DoRA) will ignore network_dropout."
+        "Only rank dropout and module dropout will be applied"
+    )
+
+
+class LoConModule(LycorisBaseModule):
+    support_module = {
+        "linear",
+        "conv1d",
+        "conv2d",
+        "conv3d",
+    }
 
     def __init__(
         self,
         lora_name,
         org_module: nn.Module,
         multiplier=1.0,
         lora_dim=4,
         alpha=1,
         dropout=0.0,
         rank_dropout=0.0,
         module_dropout=0.0,
         use_tucker=False,
-        decompose_both=False,
-        factor: int = -1,  # factorization factor
+        use_scalar=False,
         rank_dropout_scale=False,
+        weight_decompose=False,
+        bypass_mode=False,
         rs_lora=False,
         **kwargs,
     ):
         """if alpha == 0 or None, alpha is rank (no scaling)."""
-        super().__init__()
-        factor = int(factor)
-        self.lora_name = lora_name
+        super().__init__(
+            lora_name,
+            org_module,
+            multiplier,
+            dropout,
+            rank_dropout,
+            module_dropout,
+            rank_dropout_scale,
+            bypass_mode,
+        )
+        if self.module_type not in self.support_module:
+            raise ValueError(f"{self.module_type} is not supported in LoRA/LoCon algo.")
         self.lora_dim = lora_dim
         self.tucker = False
-        self.use_w1 = False
-        self.use_w2 = False
         self.rs_lora = rs_lora
 
-        self.shape = org_module.weight.shape
-        if org_module.__class__.__name__ == "Conv2d":
+        if self.module_type.startswith("conv"):
+            self.isconv = True
+            # For general LoCon
             in_dim = org_module.in_channels
             k_size = org_module.kernel_size
+            stride = org_module.stride
+            padding = org_module.padding
             out_dim = org_module.out_channels
-
-            in_m, in_n = factorization(in_dim, factor)
-            out_l, out_k = factorization(out_dim, factor)
-            shape = ((out_l, out_k), (in_m, in_n), *k_size)  # ((a, b), (c, d), *k_size)
-
             self.tucker = use_tucker and k_size != (1, 1)
-            if decompose_both and lora_dim < max(shape[0][0], shape[1][0]) / 2:
-                self.lokr_w1_a = nn.Parameter(torch.empty(shape[0][0], lora_dim))
-                self.lokr_w1_b = nn.Parameter(torch.empty(lora_dim, shape[1][0]))
-            else:
-                self.use_w1 = True
-                self.lokr_w1 = nn.Parameter(
-                    torch.empty(shape[0][0], shape[1][0])
-                )  # a*c, 1-mode
-
-            if lora_dim >= max(shape[0][1], shape[1][1]) / 2:
-                self.use_w2 = True
-                self.lokr_w2 = nn.Parameter(
-                    torch.empty(shape[0][1], shape[1][1], *k_size)
-                )
-            elif self.tucker:
-                self.lokr_t2 = nn.Parameter(
-                    torch.empty(lora_dim, lora_dim, shape[2], shape[3])
+            self.down_op = self.op
+            self.up_op = self.op
+            if use_tucker and k_size != (1, 1):
+                self.lora_down = self.module(in_dim, lora_dim, (1, 1), bias=False)
+                self.lora_mid = self.module(
+                    lora_dim, lora_dim, k_size, stride, padding, bias=False
                 )
-                self.lokr_w2_a = nn.Parameter(
-                    torch.empty(lora_dim, shape[0][1])
-                )  # b, 1-mode
-                self.lokr_w2_b = nn.Parameter(
-                    torch.empty(lora_dim, shape[1][1])
-                )  # d, 2-mode
-            else:  # Conv2d not cp
-                # bigger part. weight and LoRA. [b, dim] x [dim, d*k1*k2]
-                self.lokr_w2_a = nn.Parameter(torch.empty(shape[0][1], lora_dim))
-                self.lokr_w2_b = nn.Parameter(
-                    torch.empty(lora_dim, shape[1][1] * shape[2] * shape[3])
+                self.tucker = True
+            else:
+                self.lora_down = self.module(
+                    in_dim, lora_dim, k_size, stride, padding, bias=False
                 )
-                # w1 ⊗ (w2_a x w2_b) = (a, b)⊗((c, dim)x(dim, d*k1*k2)) = (a, b)⊗(c, d*k1*k2) = (ac, bd*k1*k2)
-
-            self.op = F.conv2d
-            self.extra_args = {
-                "stride": org_module.stride,
-                "padding": org_module.padding,
-                "dilation": org_module.dilation,
-                "groups": org_module.groups,
-            }
-
-        else:  # Linear
+            self.lora_up = self.module(lora_dim, out_dim, (1, 1), bias=False)
+        elif isinstance(org_module, nn.Linear):
+            self.isconv = False
+            self.down_op = F.linear
+            self.up_op = F.linear
             in_dim = org_module.in_features
             out_dim = org_module.out_features
+            self.lora_down = nn.Linear(in_dim, lora_dim, bias=False)
+            self.lora_up = nn.Linear(lora_dim, out_dim, bias=False)
+        else:
+            raise NotImplementedError
 
-            in_m, in_n = factorization(in_dim, factor)
-            out_l, out_k = factorization(out_dim, factor)
-            shape = (
-                (out_l, out_k),
-                (in_m, in_n),
-            )  # ((a, b), (c, d)), out_dim = a*c, in_dim = b*d
-
-            # smaller part. weight scale
-            if decompose_both and lora_dim < max(shape[0][0], shape[1][0]) / 2:
-                self.lokr_w1_a = nn.Parameter(torch.empty(shape[0][0], lora_dim))
-                self.lokr_w1_b = nn.Parameter(torch.empty(lora_dim, shape[1][0]))
-            else:
-                self.use_w1 = True
-                self.lokr_w1 = nn.Parameter(
-                    torch.empty(shape[0][0], shape[1][0])
-                )  # a*c, 1-mode
-
-            if lora_dim < max(shape[0][1], shape[1][1]) / 2:
-                # bigger part. weight and LoRA. [b, dim] x [dim, d]
-                self.lokr_w2_a = nn.Parameter(torch.empty(shape[0][1], lora_dim))
-                self.lokr_w2_b = nn.Parameter(torch.empty(lora_dim, shape[1][1]))
-                # w1 ⊗ (w2_a x w2_b) = (a, b)⊗((c, dim)x(dim, d)) = (a, b)⊗(c, d) = (ac, bd)
-            else:
-                self.use_w2 = True
-                self.lokr_w2 = nn.Parameter(torch.empty(shape[0][1], shape[1][1]))
-
-            self.op = F.linear
-            self.extra_args = {}
+        self.wd = weight_decompose
+        if self.wd:
+            org_weight: nn.Parameter = org_module.weight
+            self.dora_norm_dims = org_weight.dim() - 1
+            self.dora_scale = nn.Parameter(
+                torch.norm(
+                    org_weight.transpose(1, 0).reshape(org_weight.shape[1], -1),
+                    dim=1,
+                    keepdim=True,
+                )
+                .reshape(org_weight.shape[1], *[1] * self.dora_norm_dims)
+                .transpose(1, 0)
+            ).float()
 
-        self.dropout = dropout
         if dropout:
-            print("[WARN]LoHa/LoKr haven't implemented normal dropout yet.")
-        self.rank_dropout = rank_dropout
-        self.rank_dropout_scale = rank_dropout_scale
-        self.module_dropout = module_dropout
+            self.dropout = nn.Dropout(dropout)
+            if self.wd:
+                log_wd()
+        else:
+            self.dropout = nn.Identity()
 
-        if isinstance(alpha, torch.Tensor):
+        if type(alpha) == torch.Tensor:
             alpha = alpha.detach().float().numpy()  # without casting, bf16 causes error
         alpha = lora_dim if alpha is None or alpha == 0 else alpha
-        if self.use_w2 and self.use_w1:
-            # use scale = 1
-            alpha = lora_dim
 
         r_factor = lora_dim
         if self.rs_lora:
             r_factor = math.sqrt(r_factor)
 
         self.scale = alpha / r_factor
 
         self.register_buffer("alpha", torch.tensor(alpha))  # 定数として扱える
 
-        if self.use_w2:
-            torch.nn.init.constant_(self.lokr_w2, 0)
+        if use_scalar:
+            self.scalar = nn.Parameter(torch.tensor(0.0))
         else:
-            if self.tucker:
-                torch.nn.init.normal_(self.lokr_t2, std=0.1)
-            torch.nn.init.normal_(self.lokr_w2_a, std=1)
-            torch.nn.init.constant_(self.lokr_w2_b, 0)
-
-        if self.use_w1:
-            torch.nn.init.normal_(self.lokr_w1, std=1)
+            self.register_buffer("scalar", torch.tensor(1.0), persistent=False)
+        # same as microsoft's
+        torch.nn.init.kaiming_uniform_(self.lora_down.weight, a=math.sqrt(5))
+        if use_scalar:
+            torch.nn.init.kaiming_uniform_(self.lora_up.weight, a=math.sqrt(5))
         else:
-            torch.nn.init.normal_(self.lokr_w1_a, std=1)
-            torch.nn.init.normal_(self.lokr_w1_b, std=0.1)
-
-        self.multiplier = multiplier
-        self.org_module = [org_module]
-        weight = make_kron(
-            self.lokr_w1 if self.use_w1 else self.lokr_w1_a @ self.lokr_w1_b,
-            (
-                self.lokr_w2
-                if self.use_w2
-                else (
-                    make_weight_tucker(self.lokr_t2, self.lokr_w2_a, self.lokr_w2_b)
-                    if self.tucker
-                    else self.lokr_w2_a @ self.lokr_w2_b
-                )
-            ),
-            torch.tensor(self.multiplier * self.scale),
-        )
-        assert torch.sum(torch.isnan(weight)) == 0, "weight is nan"
+            torch.nn.init.constant_(self.lora_up.weight, 0)
+        if self.tucker:
+            torch.nn.init.kaiming_uniform_(self.lora_mid.weight, a=math.sqrt(5))
+
+    def load_weight_hook(self, module: nn.Module, incompatible_keys):
+        missing_keys = incompatible_keys.missing_keys
+        for key in missing_keys:
+            if "scalar" in key:
+                del missing_keys[missing_keys.index(key)]
+        if isinstance(self.scalar, nn.Parameter):
+            self.scalar.data.copy_(torch.ones_like(self.scalar))
+        else:
+            self.register_buffer(
+                "scalar", torch.ones_like(self.scalar), persistent=False
+            )
+
+    def make_weight(self, device=None):
+        wa = self.lora_up.weight.to(device)
+        wb = self.lora_down.weight.to(device)
+        if self.tucker:
+            t = self.lora_mid.weight.to(device)
+            wa = wa.reshape(wa.size(0), -1).transpose(0, 1)
+            wb = wb.reshape(wb.size(0), -1)
+            weight = rebuild_tucker(t, wa, wb)
+        else:
+            weight = wa.view(wa.size(0), -1) @ wb.view(wb.size(0), -1)
 
-    # Same as locon.py
-    def apply_to(self):
-        self.org_forward = self.org_module[0].forward
-        self.org_module[0].forward = self.forward
-
-    def get_weight(self, orig_weight=None):
-        weight = make_kron(
-            self.lokr_w1 if self.use_w1 else self.lokr_w1_a @ self.lokr_w1_b,
-            (
-                self.lokr_w2
-                if self.use_w2
-                else (
-                    make_weight_tucker(self.lokr_t2, self.lokr_w2_a, self.lokr_w2_b)
-                    if self.tucker
-                    else self.lokr_w2_a @ self.lokr_w2_b
-                )
-            ),
-            torch.tensor(self.scale),
-        )
-        if orig_weight is not None:
-            weight = weight.reshape(orig_weight.shape)
+        weight = weight.view(self.shape)
         if self.training and self.rank_dropout:
-            drop = (torch.rand(weight.size(0)) < self.rank_dropout).to(weight.dtype)
-            drop = drop.view(-1, *[1] * len(weight.shape[1:])).to(weight.device)
+            drop = (torch.rand(weight.size(0), device=device) > self.rank_dropout).to(
+                weight.dtype
+            )
+            drop = drop.view(-1, *[1] * len(weight.shape[1:]))
             if self.rank_dropout_scale:
                 drop /= drop.mean()
             weight *= drop
-        return weight
+
+        return weight * self.scalar
+
+    def get_diff_weight(self, multiplier=1, shape=None, device=None):
+        scale = self.scale * multiplier
+        diff = self.make_weight(device=device) * scale
+        if shape is not None:
+            diff = diff.view(shape)
+        if device is not None:
+            diff = diff.to(device)
+        return diff
+
+    def get_merged_weight(self, multiplier=1, shape=None, device=None):
+        merged = self.org_module[0].weight.data + self.get_diff_weight(
+            multiplier=multiplier, shape=shape, device=device
+        )
+        if self.wd:
+            merged = self.apply_weight_decompose(merged)
+        return merged, None
+
+    def apply_weight_decompose(self, weight):
+        weight = weight.to(self.dora_scale.dtype)
+        weight_norm = (
+            weight.transpose(0, 1)
+            .reshape(weight.shape[1], -1)
+            .norm(dim=1, keepdim=True)
+            .reshape(weight.shape[1], *[1] * self.dora_norm_dims)
+            .transpose(0, 1)
+        ) + torch.finfo(weight.dtype).eps
+
+        return weight * (self.dora_scale.to(weight.device) / weight_norm)
+
+    def custom_state_dict(self):
+        destination = {}
+        if self.wd:
+            destination["dora_scale"] = self.dora_scale
+        destination["alpha"] = self.alpha
+        destination["lora_up.weight"] = self.lora_up.weight * self.scalar
+        destination["lora_down.weight"] = self.lora_down.weight
+        if self.tucker:
+            destination["lora_mid.weight"] = self.lora_mid.weight
+        return destination
 
     @torch.no_grad()
     def apply_max_norm(self, max_norm, device=None):
-        orig_norm = self.get_weight().norm()
+        orig_norm = self.make_weight(device).norm() * self.scale
         norm = torch.clamp(orig_norm, max_norm / 2)
         desired = torch.clamp(norm, max=max_norm)
         ratio = desired.cpu() / norm.cpu()
 
         scaled = norm != desired
         if scaled:
-            modules = 4 - self.use_w1 - self.use_w2 + (not self.use_w2 and self.tucker)
-            if self.use_w1:
-                self.lokr_w1 *= ratio ** (1 / modules)
-            else:
-                self.lokr_w1_a *= ratio ** (1 / modules)
-                self.lokr_w1_b *= ratio ** (1 / modules)
+            self.scalar *= ratio
+
+        return scaled, orig_norm * ratio
 
-            if self.use_w2:
-                self.lokr_w2 *= ratio ** (1 / modules)
+    def bypass_forward_diff(self, x, scale=1):
+        if self.tucker:
+            mid = self.lora_mid(self.lora_down(x))
+        else:
+            mid = self.lora_down(x)
+
+        if self.rank_dropout and self.training:
+            drop = (
+                torch.rand(self.lora_dim, device=mid.device) > self.rank_dropout
+            ).to(mid.dtype)
+            if self.rank_dropout_scale:
+                drop /= drop.mean()
+            if (dims := len(x.shape)) == 4:
+                drop = drop.view(1, -1, 1, 1)
             else:
-                if self.tucker:
-                    self.lokr_t2 *= ratio ** (1 / modules)
-                self.lokr_w2_a *= ratio ** (1 / modules)
-                self.lokr_w2_b *= ratio ** (1 / modules)
+                drop = drop.view(*[1] * (dims - 1), -1)
+            mid = mid * drop
 
-        return scaled, orig_norm * ratio
+        return self.dropout(self.lora_up(mid) * self.scalar * self.scale * scale)
+
+    def bypass_forward(self, x, scale=1):
+        return self.org_forward(x) + self.bypass_forward_diff(x, scale=scale)
 
     def forward(self, x):
         if self.module_dropout and self.training:
             if torch.rand(1) < self.module_dropout:
-                return self.op(
-                    x,
-                    self.org_module[0].weight.data,
-                    (
-                        None
-                        if self.org_module[0].bias is None
-                        else self.org_module[0].bias.data
-                    ),
-                )
-        weight = (
-            self.org_module[0].weight.data
-            + self.get_weight(self.org_module[0].weight.data) * self.multiplier
-        )
-        bias = None if self.org_module[0].bias is None else self.org_module[0].bias.data
-        return self.op(x, weight.view(self.shape), bias, **self.extra_args)
+                return self.org_forward(x)
+        scale = self.scale * self.multiplier
+
+        dtype = self.dtype
+        if not self.bypass_mode:
+            weight = (
+                self.org_module[0].weight.data.to(dtype)
+                + self.make_weight(x.device).to(dtype) * scale
+            )
+            if self.wd:
+                weight = self.apply_weight_decompose(weight)
+            bias = (
+                None
+                if self.org_module[0].bias is None
+                else self.org_module[0].bias.data
+            )
+            return self.op(x, weight, bias, **self.kw_dict)
+        else:
+            return self.bypass_forward(x, scale=self.multiplier)
+
+
+if __name__ == "__main__":
+    base = nn.Linear(128, 128).cuda()
+    locon = LoConModule("test", base, 1, 4, 1, weight_decompose=True).cuda()
+    print(locon)
+    test_input = torch.randn(1, 128).cuda()
+    test_output = locon(test_input)
+    torch.sum(test_output).backward()
+    print(test_output.shape)
+
+    base_4bit = LinearNF4(128, 128)
+    base_4bit.load_state_dict(base.state_dict())
+    base_4bit.cuda()
+    qlocon = LoConModule("test", base_4bit, 1, 4, 1, weight_decompose=False).cuda()
+    print(qlocon)
+    test_input = torch.randn(1, 128).cuda()
+    test_output = qlocon(test_input)
+    torch.sum(test_output).backward()
+    print(test_output.shape)
+
+    base = nn.Conv2d(128, 128, 3, 1, 1)
+    locon = LoConModule("test", base, 1, 4, 1, weight_decompose=True, use_tucker=True)
+    print(locon)
+    test_input = torch.randn(1, 128, 16, 16)
+    test_output = locon(test_input)
+    torch.sum(test_output).backward()
+    print(test_output.shape)
```

### Comparing `lycoris_lora-2.3.0.dev9/lycoris/modules/ia3.py` & `lycoris_lora-3.0.0.dev1/lycoris/modules/ia3.py`

 * *Files identical despite different names*

### Comparing `lycoris_lora-2.3.0.dev9/lycoris/modules/lilora.py` & `lycoris_lora-3.0.0.dev1/lycoris/modules/lokr.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,339 +1,420 @@
 import math
 from functools import cache
 
 import torch
 import torch.nn as nn
 import torch.nn.functional as F
 
-from .base import ModuleCustomSD
+from einops import rearrange
+
+from .base import LycorisBaseModule
+from ..functional import factorization, rebuild_tucker
 from ..logging import logger
+from ..utils.bnb import LinearNF4
 
 
 @cache
-def log_wd():
-    return logger.warning(
-        "Using weight_decompose=True with LoRA (DoRA) will ignore network_dropout."
-        "Only rank dropout and module dropout will be applied"
+def logging_force_full_matrix(lora_dim, dim, factor):
+    logger.warning(
+        f"lora_dim {lora_dim} is too large for"
+        f" dim={dim} and {factor=}"
+        ", using full matrix mode."
     )
 
 
-class LiLoConModule(ModuleCustomSD):
-    """
-    modifed from kohya-ss/sd-scripts/networks/lora:LoRAModule
-    """
+def make_kron(w1, w2, scale):
+    if len(w2.shape) == 4:
+        w1 = w1.unsqueeze(2).unsqueeze(2)
+    w2 = w2.contiguous()
+    rebuild = torch.kron(w1, w2)
+
+    return rebuild * scale
+
+
+class LokrModule(LycorisBaseModule):
+    support_module = {
+        "linear",
+        "conv1d",
+        "conv2d",
+        "conv3d",
+    }
 
     def __init__(
         self,
         lora_name,
         org_module: nn.Module,
         multiplier=1.0,
         lora_dim=4,
         alpha=1,
         dropout=0.0,
         rank_dropout=0.0,
         module_dropout=0.0,
         use_tucker=False,
         use_scalar=False,
+        decompose_both=False,
+        factor: int = -1,  # factorization factor
         rank_dropout_scale=False,
         weight_decompose=False,
+        full_matrix=False,
         bypass_mode=False,
         rs_lora=False,
+        unbalanced_factorization=False,
         **kwargs,
     ):
-        """if alpha == 0 or None, alpha is rank (no scaling)."""
-        super().__init__()
-        self.lora_name = lora_name
+        super().__init__(
+            lora_name,
+            org_module,
+            multiplier,
+            dropout,
+            rank_dropout,
+            module_dropout,
+            rank_dropout_scale,
+            bypass_mode,
+        )
+        if self.module_type not in self.support_module:
+            raise ValueError(f"{self.module_type} is not supported in LoRA/LoCon algo.")
+
+        factor = int(factor)
         self.lora_dim = lora_dim
         self.tucker = False
+        self.use_w1 = False
+        self.use_w2 = False
+        self.full_matrix = full_matrix
         self.rs_lora = rs_lora
 
-        assert not (
-            bypass_mode and weight_decompose
-        ), "bypass_mode and dora_wd cannot be used together"
-
-        if isinstance(org_module, nn.Conv2d):
+        if self.module_type.startswith("conv"):
             in_dim = org_module.in_channels
             k_size = org_module.kernel_size
             out_dim = org_module.out_channels
-            self.tucker = use_tucker and k_size != (1, 1)
-            self.op = F.conv2d
-            self.extra_args = {
-                "stride": org_module.stride,
-                "padding": org_module.padding,
-                "dilation": org_module.dilation,
-                "groups": org_module.groups,
-            }
-        else:
-            in_dim = org_module.in_features
-            out_dim = org_module.out_features
-            self.op = F.linear
-            self.extra_args = {}
+            self.shape = (out_dim, in_dim, *k_size)
 
-        if isinstance(org_module, nn.Conv2d):
-            self.isconv = True
-            # For general LoCon
-            in_dim = org_module.in_channels
-            k_size = org_module.kernel_size
-            stride = org_module.stride
-            padding = org_module.padding
-            out_dim = org_module.out_channels
-            self.down_op = F.conv2d
-            self.up_op = F.conv2d
-            if use_tucker and k_size != (1, 1):
-                self.lora_down = nn.Conv2d(in_dim, lora_dim, (1, 1), bias=False)
-                self.lora_mid = nn.Conv2d(
-                    lora_dim, lora_dim, k_size, stride, padding, bias=False
-                )
-                self.tucker = True
+            in_m, in_n = factorization(in_dim, factor)
+            out_l, out_k = factorization(out_dim, factor)
+            if unbalanced_factorization:
+                out_l, out_k = out_k, out_l
+            shape = ((out_l, out_k), (in_m, in_n), *k_size)  # ((a, b), (c, d), *k_size)
+            self.tucker = use_tucker and k_size != (1, 1)
+            if (
+                decompose_both
+                and lora_dim < max(shape[0][0], shape[1][0]) / 2
+                and not self.full_matrix
+            ):
+                self.lokr_w1_a = nn.Parameter(torch.empty(shape[0][0], lora_dim))
+                self.lokr_w1_b = nn.Parameter(torch.empty(lora_dim, shape[1][0]))
             else:
-                self.lora_down = nn.Conv2d(
-                    in_dim, lora_dim, k_size, stride, padding, bias=False
+                self.use_w1 = True
+                self.lokr_w1 = nn.Parameter(
+                    torch.empty(shape[0][0], shape[1][0])
+                )  # a*c, 1-mode
+
+            if lora_dim >= max(shape[0][1], shape[1][1]) / 2 or self.full_matrix:
+                if not self.full_matrix:
+                    logging_force_full_matrix(lora_dim, max(in_dim, out_dim), factor)
+                self.use_w2 = True
+                self.lokr_w2 = nn.Parameter(
+                    torch.empty(shape[0][1], shape[1][1], *k_size)
+                )
+            elif self.tucker:
+                self.lokr_t2 = nn.Parameter(
+                    torch.empty(lora_dim, lora_dim, shape[2], shape[3])
                 )
-            self.lora_up = nn.Conv2d(lora_dim, out_dim, (1, 1), bias=False)
-        elif isinstance(org_module, nn.Linear):
-            self.isconv = False
-            self.down_op = F.linear
-            self.up_op = F.linear
+                self.lokr_w2_a = nn.Parameter(
+                    torch.empty(lora_dim, shape[0][1])
+                )  # b, 1-mode
+                self.lokr_w2_b = nn.Parameter(
+                    torch.empty(lora_dim, shape[1][1])
+                )  # d, 2-mode
+            else:  # Conv2d not tucker
+                # bigger part. weight and LoRA. [b, dim] x [dim, d*k1*k2]
+                self.lokr_w2_a = nn.Parameter(torch.empty(shape[0][1], lora_dim))
+                self.lokr_w2_b = nn.Parameter(
+                    torch.empty(
+                        lora_dim, shape[1][1] * torch.tensor(shape[2:]).prod().item()
+                    )
+                )
+                # w1 ⊗ (w2_a x w2_b) = (a, b)⊗((c, dim)x(dim, d*k1*k2)) = (a, b)⊗(c, d*k1*k2) = (ac, bd*k1*k2)
+        else:  # Linear
             in_dim = org_module.in_features
             out_dim = org_module.out_features
-            self.lora_down = nn.Linear(in_dim, lora_dim, bias=False)
-            self.lora_up = nn.Linear(lora_dim, out_dim, bias=False)
-        else:
-            raise NotImplementedError
-        self.shape = org_module.weight.shape
+            self.shape = (out_dim, in_dim)
+
+            in_m, in_n = factorization(in_dim, factor)
+            out_l, out_k = factorization(out_dim, factor)
+            if unbalanced_factorization:
+                out_l, out_k = out_k, out_l
+            shape = (
+                (out_l, out_k),
+                (in_m, in_n),
+            )  # ((a, b), (c, d)), out_dim = a*c, in_dim = b*d
+            # smaller part. weight scale
+            if decompose_both and lora_dim < max(shape[0][0], shape[1][0]) / 2:
+                self.lokr_w1_a = nn.Parameter(torch.empty(shape[0][0], lora_dim))
+                self.lokr_w1_b = nn.Parameter(torch.empty(lora_dim, shape[1][0]))
+            else:
+                self.use_w1 = True
+                self.lokr_w1 = nn.Parameter(
+                    torch.empty(shape[0][0], shape[1][0])
+                )  # a*c, 1-mode
+            if lora_dim < max(shape[0][1], shape[1][1]) / 2:
+                # bigger part. weight and LoRA. [b, dim] x [dim, d]
+                self.lokr_w2_a = nn.Parameter(torch.empty(shape[0][1], lora_dim))
+                self.lokr_w2_b = nn.Parameter(torch.empty(lora_dim, shape[1][1]))
+                # w1 ⊗ (w2_a x w2_b) = (a, b)⊗((c, dim)x(dim, d)) = (a, b)⊗(c, d) = (ac, bd)
+            else:
+                self.use_w2 = True
+                self.lokr_w2 = nn.Parameter(torch.empty(shape[0][1], shape[1][1]))
 
         self.wd = weight_decompose
         if self.wd:
             org_weight: nn.Parameter = org_module.weight
-            self.dora_mean_dim = tuple(i for i in range(org_weight.dim()) if i != 1)
+            self.dora_norm_dims = org_weight.dim() - 1
             self.dora_scale = nn.Parameter(
-                torch.mean(org_weight, dim=self.dora_mean_dim, keepdim=True)
-            )
+                torch.norm(
+                    org_weight.transpose(1, 0).reshape(org_weight.shape[1], -1),
+                    dim=1,
+                    keepdim=True,
+                )
+                .reshape(org_weight.shape[1], *[1] * self.dora_norm_dims)
+                .transpose(1, 0)
+            ).float()
 
+        self.dropout = dropout
         if dropout:
-            self.dropout = nn.Dropout(dropout)
-            if self.wd:
-                log_wd()
-        else:
-            self.dropout = nn.Identity()
+            print("[WARN]LoHa/LoKr haven't implemented normal dropout yet.")
         self.rank_dropout = rank_dropout
         self.rank_dropout_scale = rank_dropout_scale
         self.module_dropout = module_dropout
 
-        if type(alpha) == torch.Tensor:
+        if isinstance(alpha, torch.Tensor):
             alpha = alpha.detach().float().numpy()  # without casting, bf16 causes error
-
         alpha = lora_dim if alpha is None or alpha == 0 else alpha
+        if self.use_w2 and self.use_w1:
+            # use scale = 1
+            alpha = lora_dim
 
         r_factor = lora_dim
         if self.rs_lora:
             r_factor = math.sqrt(r_factor)
 
         self.scale = alpha / r_factor
 
         self.register_buffer("alpha", torch.tensor(alpha))  # 定数として扱える
 
         if use_scalar:
             self.scalar = nn.Parameter(torch.tensor(0.0))
         else:
-            self.scalar: torch.FloatTensor
-            self.register_buffer("scalar", torch.tensor(1.0), persistent=False)
-        # same as microsoft's
-        torch.nn.init.kaiming_uniform_(self.lora_down.weight, a=math.sqrt(5))
-        if use_scalar:
-            torch.nn.init.kaiming_uniform_(self.lora_up.weight, a=math.sqrt(5))
+            self.scalar = torch.tensor(1.0)
+
+        if self.use_w2:
+            if use_scalar:
+                torch.nn.init.kaiming_uniform_(self.lokr_w2, a=math.sqrt(5))
+            else:
+                torch.nn.init.constant_(self.lokr_w2, 0)
         else:
-            torch.nn.init.constant_(self.lora_up.weight, 0)
-        if self.tucker:
-            torch.nn.init.kaiming_uniform_(self.lora_mid.weight, a=math.sqrt(5))
-
-        self.multiplier = multiplier
-        self.org_module = [org_module]
-        self.org_forward = self.org_module[0].forward
+            if self.tucker:
+                torch.nn.init.kaiming_uniform_(self.lokr_t2, a=math.sqrt(5))
+            torch.nn.init.kaiming_uniform_(self.lokr_w2_a, a=math.sqrt(5))
+            if use_scalar:
+                torch.nn.init.kaiming_uniform_(self.lokr_w2_b, a=math.sqrt(5))
+            else:
+                torch.nn.init.constant_(self.lokr_w2_b, 0)
+
+        if self.use_w1:
+            torch.nn.init.kaiming_uniform_(self.lokr_w1, a=math.sqrt(5))
+        else:
+            torch.nn.init.kaiming_uniform_(self.lokr_w1_a, a=math.sqrt(5))
+            torch.nn.init.kaiming_uniform_(self.lokr_w1_b, a=math.sqrt(5))
 
     def load_weight_hook(self, module: nn.Module, incompatible_keys):
         missing_keys = incompatible_keys.missing_keys
         for key in missing_keys:
             if "scalar" in key:
                 del missing_keys[missing_keys.index(key)]
         if isinstance(self.scalar, nn.Parameter):
-            self.scalar.copy_(torch.ones_like(self.scalar))
-        else:
-            self.scalar = torch.ones_like(self.scalar)
-
-    def apply_to(self, is_hypernet=False, **kwargs):
-        self.org_forward = self.org_module[0].forward
-        if is_hypernet:
-            self.org_module[0].forward = self.hypernet_forward
+            self.scalar.data.copy_(torch.ones_like(self.scalar))
         else:
-            self.org_module[0].forward = self.forward
-
-    def restore(self):
-        self.org_module[0].forward = self.org_forward
-
-    def merge_to(self, multiplier=1.0):
-        weight = self.make_weight() * self.scale * multiplier
-        self.org_module[0].weight.data.add_(weight)
-
-    def make_weight(self, device=None):
-        wa = self.lora_up.weight.to(device)
-        wb = self.lora_down.weight.to(device)
-        if self.tucker:
-            t = self.lora_mid.weight.to(device)
-            wa = wa.squeeze(-1, -2)
-            wb = wb.squeeze(-1, -2)
-            weight = torch.einsum("i j k l, p i, j r -> p r k l", t, wa, wb)
-        else:
-            weight = wa.view(wa.size(0), -1) @ wb.view(wb.size(0), -1)
+            self.register_buffer(
+                "scalar", torch.ones_like(self.scalar), persistent=False
+            )
 
-        weight = weight.view(self.shape)
+    def get_weight(self, shape):
+        weight = make_kron(
+            self.lokr_w1 if self.use_w1 else self.lokr_w1_a @ self.lokr_w1_b,
+            (
+                self.lokr_w2
+                if self.use_w2
+                else (
+                    rebuild_tucker(self.lokr_t2, self.lokr_w2_a, self.lokr_w2_b)
+                    if self.tucker
+                    else self.lokr_w2_a @ self.lokr_w2_b
+                )
+            ),
+            torch.tensor(self.scale),
+        )
+        dtype = weight.dtype
+        if shape is not None:
+            weight = weight.view(shape)
         if self.training and self.rank_dropout:
-            drop = (torch.rand(weight.size(0)) > self.rank_dropout).to(weight.dtype)
-            drop = drop.view(-1, *[1] * len(weight.shape[1:])).to(weight.device)
+            drop = (torch.rand(weight.size(0)) > self.rank_dropout).to(dtype)
+            drop = drop.view(-1, *[1] * len(weight.shape[1:]))
             if self.rank_dropout_scale:
                 drop /= drop.mean()
             weight *= drop
+        return weight
 
-        return weight * self.scalar.to(device)
+    def get_merged_weight(self, multiplier=1, shape=None, device=None):
+        scale = self.scale * multiplier
+        diff = self.get_weight(shape) * scale
+        if device is not None:
+            diff = diff.to(device)
+        merged = self.org_module[0].weight.data + diff
+        if self.wd:
+            merged = self.apply_weight_decompose(merged)
+        return merged
 
     def apply_weight_decompose(self, weight):
-        return (
-            weight / weight.mean(dim=self.dora_mean_dim, keepdim=True) * self.dora_scale
-        )
+        weight = weight.to(self.dora_scale.dtype)
+        weight_norm = (
+            weight.transpose(0, 1)
+            .reshape(weight.shape[1], -1)
+            .norm(dim=1, keepdim=True)
+            .reshape(weight.shape[1], *[1] * self.dora_norm_dims)
+            .transpose(0, 1)
+        ) + torch.finfo(weight.dtype).eps
+
+        return weight * (self.dora_scale / weight_norm)
 
     def custom_state_dict(self):
         destination = {}
+        destination["alpha"] = self.alpha
         if self.wd:
             destination["dora_scale"] = self.dora_scale
-        destination["alpha"] = self.alpha
-        destination["lora_up.weight"] = self.lora_up.weight * self.scalar
-        destination["lora_down.weight"] = self.lora_down.weight
-        if self.tucker:
-            destination["lora_mid.weight"] = self.lora_mid.weight
+        if self.use_w1:
+            destination["lokr_w1"] = self.lokr_w1 * self.scalar
+        else:
+            destination["lokr_w1_a"] = self.lokr_w1_a * self.scalar
+            destination["lokr_w1_b"] = self.lokr_w1_b
+
+        if self.use_w2:
+            destination["lokr_w2"] = self.lokr_w2
+        else:
+            destination["lokr_w2_a"] = self.lokr_w2_a
+            destination["lokr_w2_b"] = self.lokr_w2_b
+            if self.tucker:
+                destination["lokr_t2"] = self.lokr_t2
         return destination
 
     @torch.no_grad()
     def apply_max_norm(self, max_norm, device=None):
-        orig_norm = self.make_weight(device).norm() * self.scale
+        orig_norm = self.get_weight(self.shape).norm()
         norm = torch.clamp(orig_norm, max_norm / 2)
         desired = torch.clamp(norm, max=max_norm)
         ratio = desired.cpu() / norm.cpu()
 
         scaled = norm != desired
         if scaled:
-            self.scalar *= ratio
+            modules = 4 - self.use_w1 - self.use_w2 + (not self.use_w2 and self.tucker)
+            if self.use_w1:
+                self.lokr_w1 *= ratio ** (1 / modules)
+            else:
+                self.lokr_w1_a *= ratio ** (1 / modules)
+                self.lokr_w1_b *= ratio ** (1 / modules)
+
+            if self.use_w2:
+                self.lokr_w2 *= ratio ** (1 / modules)
+            else:
+                if self.tucker:
+                    self.lokr_t2 *= ratio ** (1 / modules)
+                self.lokr_w2_a *= ratio ** (1 / modules)
+                self.lokr_w2_b *= ratio ** (1 / modules)
 
         return scaled, orig_norm * ratio
 
-    def update_weights(self, down, up, idx):
-        self.down, self.up = self.make_lightweight(down.squeeze(1), up.squeeze(1), idx)
+    def bypass_forward_diff(self, h, scale=1):
+        if len(self.shape) > 2 and self.shape[2] > 1:
+            return (
+                self.op(h, self.get_weight(self.shape), **self.kw_dict)
+                * self.multiplier
+            )
+        if self.module_type.startswith("conv"):
+            h = h.transpose(1, -1)
+        if self.use_w2:
+            ba = self.lokr_w2
+        else:
+            a = self.lokr_w2_b
+            b = self.lokr_w2_a
+        if self.use_w1:
+            c = self.lokr_w1
+        else:
+            c = self.lokr_w1_a @ self.lokr_w1_b
+        uq = c.size(1)
+
+        if self.use_w2:
+            vq = ba.size(1)
+            h_in_group = rearrange(h, "b ... (uq vq) -> b ... uq vq", uq=uq, vq=vq)
+            hb = F.linear(h_in_group, ba)
+        else:
+            vq = a.size(1)
+            h_in_group = rearrange(h, "b ... (uq vq) -> b ... uq vq", uq=uq, vq=vq)
+            ha = F.linear(h_in_group, a)
+            hb = F.linear(ha, b)
+
+        h_cross_group = hb.transpose(-1, -2)
+        hc = F.linear(h_cross_group, c)
+
+        h = rearrange(hc, "b ... vp up -> b ... (up vp)")
+        if self.module_type.startswith("conv"):
+            h = h.transpose(1, -1)
 
-    def make_lightweight(self, down, up, seed=None, down_aux=None, up_aux=None):
-        if down.dim() == 3:
-            down = down.reshape(down.size(0), self.lora_dim, -1)
-            up = up.reshape(up.size(0), -1, self.lora_dim)
-        else:
-            down = down.reshape(self.lora_dim, -1)
-            up = up.reshape(-1, self.lora_dim)
-        # print(up.shape)
-        if seed is None:
-            assert down_aux is not None and up_aux is not None
-        else:
-            rng_state = torch.get_rng_state()
-            torch.manual_seed(seed)
-            if down_aux is None or up_aux is None:
-                down_aux = torch.empty(
-                    down.size(down.dim() - 1),
-                    self.lora_down.weight.size(1),
-                    device=down.device,
-                )
-                up_aux = torch.empty(
-                    self.lora_up.weight.size(0), up.size(up.dim() - 2), device=up.device
-                )
-                nn.init.orthogonal_(down_aux)
-                nn.init.orthogonal_(up_aux)
-                # print(up_aux.shape)
-            torch.set_rng_state(rng_state)
-        if down.dim() == 3 and down.size(0) == 1:
-            down = down.squeeze(0)
-        if up.dim() == 3 and up.size(0) == 1:
-            up = up.squeeze(0)
-        down = down + 1  # avoid zero grad or slow training, give it a constant
-        return (down @ down_aux), (up_aux @ up)
-
-    def apply_lightweight(self, down, up, seed=None, down_aux=None, up_aux=None):
-        down_weight, up_weight = self.make_lightweight(down, up, seed, down_aux, up_aux)
-        self.lora_down.weight.data = down_weight
-        self.lora_up.weight.data = up_weight
-        return down_weight, up_weight
+        return self.drop(h * scale)
 
-    def hypernet_forward(self, x):
+    def bypass_forward(self, x, scale=1):
+        return self.org_forward(x) + self.bypass_forward_diff(x, scale=scale)
+
+    def forward(self, x: torch.Tensor, *args, **kwargs):
         if self.module_dropout and self.training:
             if torch.rand(1) < self.module_dropout:
                 return self.org_forward(x)
-        scale = self.scale * self.multiplier
-
-        down_weight = self.down
-        up_weight = self.up
-
-        x_batch = None
-        if down_weight.dim() == 3:
-            if x.size(0) != down_weight.size(0):
-                assert (
-                    self.isconv == False
-                ), "Convolutional hypernet with batch size mismatch is not supported"
-                x_batch = x.size(0)
-                x = x.view(down_weight.size(0), -1, *x.shape[1:])
-
-            if self.isconv:
-                mid = torch.einsum("ijk, ik... -> ij...", down_weight, x)
-            else:
-                mid = torch.einsum("ijk, i...k -> i...j", down_weight, x)
+        if self.bypass_mode:
+            return self.bypass_forward(x, self.multiplier)
         else:
-            if self.isconv:
-                weight = down_weight.unsqueeze(-1).unsqueeze(-1)
-            else:
-                weight = down_weight
-            mid = self.down_op(x, weight)
-
-        if self.rank_dropout and self.training:
-            drop = (
-                torch.rand(self.lora_dim, device=mid.device) < self.rank_dropout
-            ).to(mid.dtype)
-            if self.rank_dropout_scale:
-                drop /= drop.mean()
-            if (dims := len(x.shape)) == 4:
-                drop = drop.view(1, -1, 1, 1)
-            else:
-                drop = drop.view(*[1] * (dims - 1), -1)
-            mid = mid * drop
-
-        if up_weight.dim() == 3:
-            mid_batch = None
-            if mid.size(0) != up_weight.size(0):
-                assert (
-                    self.isconv == False
-                ), "Convolutional hypernet with batch size mismatch is not supported"
-                mid_batch = mid.size(0)
-                mid = mid.view(up_weight.size(0), -1, *mid.shape[1:])
-
-            if self.isconv:
-                up = torch.einsum("ijk, ik... -> ij...", up_weight, mid)
-            else:
-                up = torch.einsum("ijk, i...k -> i...j", up_weight, mid)
+            weight = (
+                self.org_module[0].weight.data.to(self.dtype)
+                + self.get_weight(self.shape) * self.scalar * self.multiplier
+            )
+            bias = (
+                None
+                if self.org_module[0].bias is None
+                else self.org_module[0].bias.data
+            )
 
-            if mid_batch is not None:
-                up = up.view(mid_batch, *up.shape[2:])
-        else:
-            if self.isconv:
-                weight = up_weight.unsqueeze(-1).unsqueeze(-1)
-            else:
-                weight = up_weight
-            up = self.up_op(mid, weight)
+            if self.wd:
+                weight = self.apply_weight_decompose(weight)
+            return self.op(x, weight.view(self.shape), bias, **self.kw_dict)
 
-        if x_batch is not None:
-            up = up.view(x_batch, *up.shape[2:])
 
-        org_out = self.org_forward(x)
-        # print(x.shape, org_out.shape, up.shape)
-        return org_out + self.dropout(up) * scale
+if __name__ == "__main__":
+    base = nn.Linear(128, 128).cuda()
+    lokr = LokrModule("test", base, 1, 4, 1, weight_decompose=True, factor=8).cuda()
+    print(lokr)
+    test_input = torch.randn(1, 77, 128).cuda()
+    test_output = lokr(test_input)
+    torch.sum(test_output).backward()
+    print(test_output.shape)
+
+    base_4bit = LinearNF4(128, 128)
+    base_4bit.load_state_dict(base.state_dict())
+    base_4bit.cuda()
+    qlokr = LokrModule("test", base_4bit, 1, 4, 1, weight_decompose=False).cuda()
+    print(qlokr)
+    test_output = qlokr(test_input)
+    torch.sum(test_output).backward()
+    print(test_output.shape)
+
+    base = nn.Conv2d(128, 128, 3, 1, 1)
+    lokr = LokrModule("test", base, 1, 4, 1, weight_decompose=True, use_tucker=True)
+    print(lokr)
+    test_input = torch.randn(1, 128, 16, 16)
+    test_output = lokr(test_input)
+    torch.sum(test_output).backward()
+    print(test_output.shape)
```

### Comparing `lycoris_lora-2.3.0.dev9/lycoris/utils/__init__.py` & `lycoris_lora-3.0.0.dev1/lycoris/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `lycoris_lora-2.3.0.dev9/lycoris/utils/logger.py` & `lycoris_lora-3.0.0.dev1/lycoris/utils/logger.py`

 * *Files identical despite different names*

### Comparing `lycoris_lora-2.3.0.dev9/lycoris_lora.egg-info/PKG-INFO` & `lycoris_lora-3.0.0.dev1/lycoris_lora.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lycoris_lora
-Version: 2.3.0.dev9
+Version: 3.0.0.dev1
 Summary: Lora beYond Conventional methods, Other Rank adaptation Implementations for Stable diffusion
 Home-page: https://github.com/KohakuBlueleaf/LyCORIS
 Author: Shih-Ying Yeh(KohakuBlueLeaf), Yu-Guan Hsieh, Zhidong Gao
 Author-email: apolloyeh0123@gmail.com
 Requires-Python: >=3.10
 License-File: LICENSE.md
 Requires-Dist: torch
```

### Comparing `lycoris_lora-2.3.0.dev9/setup.py` & `lycoris_lora-3.0.0.dev1/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 
 
 setup(
     name="lycoris_lora",
     packages=find_packages(),
-    version="2.3.0.dev9",
+    version="3.0.0.dev1",
     url="https://github.com/KohakuBlueleaf/LyCORIS",
     description="Lora beYond Conventional methods, Other Rank adaptation Implementations for Stable diffusion",
     author="Shih-Ying Yeh(KohakuBlueLeaf), Yu-Guan Hsieh, Zhidong Gao",
     author_email="apolloyeh0123@gmail.com",
     zip_safe=False,
     install_requires=[
         "torch",
```

