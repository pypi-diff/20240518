# Comparing `tmp/txm_sandbox-0.3.1.tar.gz` & `tmp/txm_sandbox-0.3.1.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "txm_sandbox-0.3.1.tar", last modified: Wed May 15 04:02:48 2024, max compression
+gzip compressed data, was "txm_sandbox-0.3.1.post1.tar", last modified: Sat May 18 02:17:05 2024, max compression
```

## Comparing `txm_sandbox-0.3.1.tar` & `txm_sandbox-0.3.1.post1.tar`

### file list

```diff
@@ -1,100 +1,100 @@
-drwxr-xr-x   0 xianghui   (501) staff       (20)        0 2024-05-15 04:02:48.038593 txm_sandbox-0.3.1/
--rw-rw-r--   0 xianghui   (501) staff       (20)     1070 2024-04-27 23:21:56.000000 txm_sandbox-0.3.1/LICENSE
--rw-rw-r--   0 xianghui   (501) staff       (20)      203 2024-05-09 00:28:45.000000 txm_sandbox-0.3.1/MANIFEST.in
--rw-r--r--   0 xianghui   (501) staff       (20)      706 2024-05-15 04:02:48.038407 txm_sandbox-0.3.1/PKG-INFO
--rw-rw-r--   0 xianghui   (501) staff       (20)     1964 2024-05-09 00:35:34.000000 txm_sandbox-0.3.1/README.md
--rwxrwxr-x   0 xianghui   (501) staff       (20)     2565 2024-04-27 23:21:56.000000 txm_sandbox-0.3.1/TXM_GUI2.ipynb
--rw-r--r--   0 xianghui   (501) staff       (20)       38 2024-05-15 04:02:48.038633 txm_sandbox-0.3.1/setup.cfg
--rw-rw-r--   0 xianghui   (501) staff       (20)     1124 2024-05-15 04:00:27.000000 txm_sandbox-0.3.1/setup.py
-drwxr-xr-x   0 xianghui   (501) staff       (20)        0 2024-05-15 04:02:48.010140 txm_sandbox-0.3.1/txm_sandbox/
--rw-rw-r--   0 xianghui   (501) staff       (20)      181 2024-04-28 16:42:36.000000 txm_sandbox-0.3.1/txm_sandbox/__init__.py
-drwxr-xr-x   0 xianghui   (501) staff       (20)        0 2024-05-15 04:02:48.012446 txm_sandbox-0.3.1/txm_sandbox/config/
--rw-rw-r--   0 xianghui   (501) staff       (20)     5092 2024-04-28 16:42:36.000000 txm_sandbox-0.3.1/txm_sandbox/config/XANES2D_GUI_config.json
--rw-rw-r--   0 xianghui   (501) staff       (20)      107 2024-04-28 16:42:36.000000 txm_sandbox-0.3.1/txm_sandbox/config/__init__.py
--rw-rw-r--   0 xianghui   (501) staff       (20)       45 2024-04-28 16:42:36.000000 txm_sandbox-0.3.1/txm_sandbox/config/analysis_tool_gui_cfg.json
--rw-rw-r--   0 xianghui   (501) staff       (20)      497 2024-04-28 16:42:36.000000 txm_sandbox-0.3.1/txm_sandbox/config/io_tomo_h5_data_structure.json
--rw-rw-r--   0 xianghui   (501) staff       (20)      500 2024-04-28 16:42:36.000000 txm_sandbox-0.3.1/txm_sandbox/config/io_xanes2D_h5_data_structure.json
--rw-rw-r--   0 xianghui   (501) staff       (20)      616 2024-04-28 16:42:36.000000 txm_sandbox-0.3.1/txm_sandbox/config/io_xanes3D_h5_data_structure.json
-drwxr-xr-x   0 xianghui   (501) staff       (20)        0 2024-05-15 04:02:48.013733 txm_sandbox-0.3.1/txm_sandbox/dicts/
--rw-rw-r--   0 xianghui   (501) staff       (20)      107 2024-04-28 16:42:36.000000 txm_sandbox-0.3.1/txm_sandbox/dicts/__init__.py
--rw-rw-r--   0 xianghui   (501) staff       (20)     3848 2024-04-28 16:42:36.000000 txm_sandbox-0.3.1/txm_sandbox/dicts/config_dict.py
--rw-rw-r--   0 xianghui   (501) staff       (20)    61110 2024-04-28 16:42:36.000000 txm_sandbox-0.3.1/txm_sandbox/dicts/customized_struct_dict.py
--rw-rw-r--   0 xianghui   (501) staff       (20)      755 2024-04-28 16:42:36.000000 txm_sandbox-0.3.1/txm_sandbox/dicts/sklearn_opt_dict.py
--rw-rw-r--   0 xianghui   (501) staff       (20)      583 2024-04-28 16:42:36.000000 txm_sandbox-0.3.1/txm_sandbox/dicts/xanes_analysis_dict.py
-drwxr-xr-x   0 xianghui   (501) staff       (20)        0 2024-05-15 04:02:48.014142 txm_sandbox-0.3.1/txm_sandbox/external/
--rw-rw-r--   0 xianghui   (501) staff       (20)      107 2024-04-28 16:42:36.000000 txm_sandbox-0.3.1/txm_sandbox/external/__init__.py
--rw-rw-r--   0 xianghui   (501) staff       (20)      253 2024-04-28 16:42:36.000000 txm_sandbox-0.3.1/txm_sandbox/external/user_io.py
-drwxr-xr-x   0 xianghui   (501) staff       (20)        0 2024-05-15 04:02:48.021615 txm_sandbox-0.3.1/txm_sandbox/gui/
--rw-rw-r--   0 xianghui   (501) staff       (20)      107 2024-04-28 16:42:36.000000 txm_sandbox-0.3.1/txm_sandbox/gui/__init__.py
--rw-rw-r--   0 xianghui   (501) staff       (20)    32500 2024-04-28 16:42:36.000000 txm_sandbox-0.3.1/txm_sandbox/gui/conv_data_gui.py
--rw-rw-r--   0 xianghui   (501) staff       (20)    74137 2024-04-28 16:42:36.000000 txm_sandbox-0.3.1/txm_sandbox/gui/gen_algn_gui.py
--rw-rw-r--   0 xianghui   (501) staff       (20)    79148 2024-05-12 04:56:04.000000 txm_sandbox-0.3.1/txm_sandbox/gui/gui_components.py
--rw-rw-r--   0 xianghui   (501) staff       (20)    36752 2024-04-28 16:42:36.000000 txm_sandbox-0.3.1/txm_sandbox/gui/io_config_gui.py
--rw-rw-r--   0 xianghui   (501) staff       (20)    15709 2024-04-28 16:42:36.000000 txm_sandbox-0.3.1/txm_sandbox/gui/main_gui.py
--rw-rw-r--   0 xianghui   (501) staff       (20)      795 2024-04-28 16:42:36.000000 txm_sandbox-0.3.1/txm_sandbox/gui/misc_gui.py
--rw-rw-r--   0 xianghui   (501) staff       (20)   169879 2024-04-28 16:42:36.000000 txm_sandbox-0.3.1/txm_sandbox/gui/tomo_gui.py
--rw-rw-r--   0 xianghui   (501) staff       (20)   204783 2024-04-28 16:42:36.000000 txm_sandbox-0.3.1/txm_sandbox/gui/xanes2D_gui.py
--rw-rw-r--   0 xianghui   (501) staff       (20)   202060 2024-04-28 16:42:36.000000 txm_sandbox-0.3.1/txm_sandbox/gui/xanes3D_gui.py
--rw-rw-r--   0 xianghui   (501) staff       (20)    91679 2024-04-28 16:42:36.000000 txm_sandbox-0.3.1/txm_sandbox/gui/xanes_analysis_gui.py
--rw-rw-r--   0 xianghui   (501) staff       (20)   203257 2024-04-28 16:42:36.000000 txm_sandbox-0.3.1/txm_sandbox/gui/xanes_fitting_gui.py
-drwxr-xr-x   0 xianghui   (501) staff       (20)        0 2024-05-15 04:02:48.022312 txm_sandbox-0.3.1/txm_sandbox/napari_gui/
--rw-rw-r--   0 xianghui   (501) staff       (20)      181 2024-05-14 04:58:24.000000 txm_sandbox-0.3.1/txm_sandbox/napari_gui/__init__.py
-drwxr-xr-x   0 xianghui   (501) staff       (20)        0 2024-05-15 04:02:48.024216 txm_sandbox-0.3.1/txm_sandbox/napari_gui/configs/
--rw-rw-r--   0 xianghui   (501) staff       (20)      181 2024-05-14 04:58:24.000000 txm_sandbox-0.3.1/txm_sandbox/napari_gui/configs/__init__.py
--rw-rw-r--   0 xianghui   (501) staff       (20)      979 2024-05-14 04:58:24.000000 txm_sandbox-0.3.1/txm_sandbox/napari_gui/configs/txm_simple_gui_script_cfg.json
--rw-rw-r--   0 xianghui   (501) staff       (20)      957 2024-05-14 04:58:24.000000 txm_sandbox-0.3.1/txm_sandbox/napari_gui/configs/xanes2d_image_autoreg_cfg.json
--rw-rw-r--   0 xianghui   (501) staff       (20)      899 2024-05-14 04:58:24.000000 txm_sandbox-0.3.1/txm_sandbox/napari_gui/configs/xanes3d_tomo_autocent_cfg.json
--rw-rw-r--   0 xianghui   (501) staff       (20)     2389 2024-05-14 04:58:24.000000 txm_sandbox-0.3.1/txm_sandbox/napari_gui/configs/xanes3d_tomo_template_cfg.json
--rw-rw-r--   0 xianghui   (501) staff       (20)     1362 2024-05-14 04:58:24.000000 txm_sandbox-0.3.1/txm_sandbox/napari_gui/configs/xanes_proc_data_struct_cfg.json
-drwxr-xr-x   0 xianghui   (501) staff       (20)        0 2024-05-15 04:02:48.024576 txm_sandbox-0.3.1/txm_sandbox/napari_gui/dicts/
--rw-rw-r--   0 xianghui   (501) staff       (20)      181 2024-05-14 04:58:24.000000 txm_sandbox-0.3.1/txm_sandbox/napari_gui/dicts/__init__.py
--rw-r--r--   0 xianghui   (501) staff       (20)     8853 2024-05-14 04:58:24.000000 txm_sandbox-0.3.1/txm_sandbox/napari_gui/dicts/data_struct_dict.py
-drwxr-xr-x   0 xianghui   (501) staff       (20)        0 2024-05-15 04:02:48.028228 txm_sandbox-0.3.1/txm_sandbox/napari_gui/guis/
--rw-rw-r--   0 xianghui   (501) staff       (20)      106 2024-05-14 04:58:24.000000 txm_sandbox-0.3.1/txm_sandbox/napari_gui/guis/__init__.py
--rw-rw-r--   0 xianghui   (501) staff       (20)    16170 2024-05-14 04:58:24.000000 txm_sandbox-0.3.1/txm_sandbox/napari_gui/guis/appl_mask_gui.py
--rw-rw-r--   0 xianghui   (501) staff       (20)     9799 2024-05-14 04:58:24.000000 txm_sandbox-0.3.1/txm_sandbox/napari_gui/guis/convert_data_gui.py
--rw-r--r--   0 xianghui   (501) staff       (20)     3929 2024-05-14 04:58:24.000000 txm_sandbox-0.3.1/txm_sandbox/napari_gui/guis/extra_io_gui.py
--rw-r--r--   0 xianghui   (501) staff       (20)    32957 2024-05-14 07:59:24.000000 txm_sandbox-0.3.1/txm_sandbox/napari_gui/guis/tomo_gui.py
--rw-r--r--   0 xianghui   (501) staff       (20)    24243 2024-05-14 04:58:24.000000 txm_sandbox-0.3.1/txm_sandbox/napari_gui/guis/xanes_fit_gui.py
--rw-r--r--   0 xianghui   (501) staff       (20)    67247 2024-05-15 03:58:02.000000 txm_sandbox-0.3.1/txm_sandbox/napari_gui/guis/xanes_reg_gui.py
--rw-rw-r--   0 xianghui   (501) staff       (20)    16157 2024-05-14 04:58:24.000000 txm_sandbox-0.3.1/txm_sandbox/napari_gui/guis/xanes_vis_gui.py
-drwxr-xr-x   0 xianghui   (501) staff       (20)        0 2024-05-15 04:02:48.030167 txm_sandbox-0.3.1/txm_sandbox/napari_gui/scripts/
--rw-rw-r--   0 xianghui   (501) staff       (20)      107 2024-05-14 04:58:24.000000 txm_sandbox-0.3.1/txm_sandbox/napari_gui/scripts/__init__.py
--rw-rw-r--   0 xianghui   (501) staff       (20)     4223 2024-05-14 05:10:46.000000 txm_sandbox-0.3.1/txm_sandbox/napari_gui/scripts/aps_xanes2d_image_autoreg_cmd.py
--rw-rw-r--   0 xianghui   (501) staff       (20)      650 2024-05-14 04:58:24.000000 txm_sandbox-0.3.1/txm_sandbox/napari_gui/scripts/tomo_batch_recon_cmd.py
--rw-rw-r--   0 xianghui   (501) staff       (20)      599 2024-05-14 04:58:24.000000 txm_sandbox-0.3.1/txm_sandbox/napari_gui/scripts/tomo_recon_cmd.py
--rw-rw-r--   0 xianghui   (501) staff       (20)    15251 2024-05-14 04:58:24.000000 txm_sandbox-0.3.1/txm_sandbox/napari_gui/scripts/xanes2D_fit_cmd.py
--rw-rw-r--   0 xianghui   (501) staff       (20)     2441 2024-05-14 04:58:24.000000 txm_sandbox-0.3.1/txm_sandbox/napari_gui/scripts/xanes2d_image_autoreg_cmd.py
--rw-rw-r--   0 xianghui   (501) staff       (20)    16610 2024-05-14 04:58:24.000000 txm_sandbox-0.3.1/txm_sandbox/napari_gui/scripts/xanes3D_fit_cmd.py
--rw-rw-r--   0 xianghui   (501) staff       (20)     1197 2024-05-14 04:58:24.000000 txm_sandbox-0.3.1/txm_sandbox/napari_gui/scripts/xanes3d_tomo_autocent_cmd.py
--rw-r--r--   0 xianghui   (501) staff       (20)     2029 2024-05-14 04:58:24.000000 txm_sandbox-0.3.1/txm_sandbox/napari_gui/scripts/xnaes2d_image_autoreg_cmd.py
--rw-r--r--   0 xianghui   (501) staff       (20)     1533 2024-05-14 04:58:24.000000 txm_sandbox-0.3.1/txm_sandbox/napari_gui/txm_gui.py
-drwxr-xr-x   0 xianghui   (501) staff       (20)        0 2024-05-15 04:02:48.031206 txm_sandbox-0.3.1/txm_sandbox/napari_gui/utils/
--rw-rw-r--   0 xianghui   (501) staff       (20)      181 2024-05-14 04:58:24.000000 txm_sandbox-0.3.1/txm_sandbox/napari_gui/utils/__init__.py
--rw-r--r--   0 xianghui   (501) staff       (20)     5157 2024-05-14 04:58:24.000000 txm_sandbox-0.3.1/txm_sandbox/napari_gui/utils/ext_io_lib.py
--rw-rw-r--   0 xianghui   (501) staff       (20)     1264 2024-05-14 04:58:24.000000 txm_sandbox-0.3.1/txm_sandbox/napari_gui/utils/io.py
--rw-r--r--   0 xianghui   (501) staff       (20)    10590 2024-05-14 04:58:24.000000 txm_sandbox-0.3.1/txm_sandbox/napari_gui/utils/misc.py
-drwxr-xr-x   0 xianghui   (501) staff       (20)        0 2024-05-15 04:02:48.031756 txm_sandbox-0.3.1/txm_sandbox/tmp/
--rw-rw-r--   0 xianghui   (501) staff       (20)      107 2024-04-28 16:42:36.000000 txm_sandbox-0.3.1/txm_sandbox/tmp/__init__.py
--rw-rw-r--   0 xianghui   (501) staff       (20)       69 2024-04-28 16:42:36.000000 txm_sandbox-0.3.1/txm_sandbox/tmp/readme.txt
-drwxr-xr-x   0 xianghui   (501) staff       (20)        0 2024-05-15 04:02:48.037845 txm_sandbox-0.3.1/txm_sandbox/utils/
--rw-rw-r--   0 xianghui   (501) staff       (20)      107 2024-04-28 16:42:36.000000 txm_sandbox-0.3.1/txm_sandbox/utils/__init__.py
--rw-rw-r--   0 xianghui   (501) staff       (20)    16672 2024-04-28 16:42:36.000000 txm_sandbox-0.3.1/txm_sandbox/utils/io.py
--rw-rw-r--   0 xianghui   (501) staff       (20)    14410 2024-04-28 16:42:36.000000 txm_sandbox-0.3.1/txm_sandbox/utils/lineshapes.py
--rwxrwxr-x   0 xianghui   (501) staff       (20)     4246 2024-04-28 16:42:36.000000 txm_sandbox-0.3.1/txm_sandbox/utils/misc.py
--rw-rw-r--   0 xianghui   (501) staff       (20)     1439 2024-04-28 16:42:36.000000 txm_sandbox-0.3.1/txm_sandbox/utils/plotlib.py
--rw-rw-r--   0 xianghui   (501) staff       (20)    61837 2024-04-28 16:42:36.000000 txm_sandbox-0.3.1/txm_sandbox/utils/reg_algs.py
--rw-rw-r--   0 xianghui   (501) staff       (20)    70498 2024-04-28 16:42:36.000000 txm_sandbox-0.3.1/txm_sandbox/utils/tomo_recon_tools.py
--rw-rw-r--   0 xianghui   (501) staff       (20)    41021 2024-04-28 16:42:36.000000 txm_sandbox-0.3.1/txm_sandbox/utils/xanes_analysis.py
--rw-rw-r--   0 xianghui   (501) staff       (20)     2342 2024-04-28 16:42:36.000000 txm_sandbox-0.3.1/txm_sandbox/utils/xanes_image_utils.py
--rw-rw-r--   0 xianghui   (501) staff       (20)    23436 2024-04-28 16:42:36.000000 txm_sandbox-0.3.1/txm_sandbox/utils/xanes_math.py
--rw-rw-r--   0 xianghui   (501) staff       (20)     6083 2024-04-28 16:42:36.000000 txm_sandbox-0.3.1/txm_sandbox/utils/xanes_post_analysis.py
--rw-rw-r--   0 xianghui   (501) staff       (20)    84912 2024-05-14 13:37:48.000000 txm_sandbox-0.3.1/txm_sandbox/utils/xanes_regtools.py
--rw-rw-r--   0 xianghui   (501) staff       (20)     3266 2024-04-28 16:42:36.000000 txm_sandbox-0.3.1/txm_sandbox/utils/xanes_spectra_filters.py
-drwxr-xr-x   0 xianghui   (501) staff       (20)        0 2024-05-15 04:02:48.038181 txm_sandbox-0.3.1/txm_sandbox.egg-info/
--rw-r--r--   0 xianghui   (501) staff       (20)      706 2024-05-15 04:02:47.000000 txm_sandbox-0.3.1/txm_sandbox.egg-info/PKG-INFO
--rw-r--r--   0 xianghui   (501) staff       (20)     3196 2024-05-15 04:02:47.000000 txm_sandbox-0.3.1/txm_sandbox.egg-info/SOURCES.txt
--rw-r--r--   0 xianghui   (501) staff       (20)        1 2024-05-15 04:02:47.000000 txm_sandbox-0.3.1/txm_sandbox.egg-info/dependency_links.txt
--rw-r--r--   0 xianghui   (501) staff       (20)        1 2024-05-15 04:02:47.000000 txm_sandbox-0.3.1/txm_sandbox.egg-info/not-zip-safe
--rw-r--r--   0 xianghui   (501) staff       (20)      170 2024-05-15 04:02:47.000000 txm_sandbox-0.3.1/txm_sandbox.egg-info/requires.txt
--rw-r--r--   0 xianghui   (501) staff       (20)       12 2024-05-15 04:02:47.000000 txm_sandbox-0.3.1/txm_sandbox.egg-info/top_level.txt
+drwxr-xr-x   0 xianghui   (501) staff       (20)        0 2024-05-18 02:17:05.320273 txm_sandbox-0.3.1.post1/
+-rw-rw-r--   0 xianghui   (501) staff       (20)     1070 2024-04-27 23:21:56.000000 txm_sandbox-0.3.1.post1/LICENSE
+-rw-rw-r--   0 xianghui   (501) staff       (20)      203 2024-05-09 00:28:45.000000 txm_sandbox-0.3.1.post1/MANIFEST.in
+-rw-r--r--   0 xianghui   (501) staff       (20)      712 2024-05-18 02:17:05.320089 txm_sandbox-0.3.1.post1/PKG-INFO
+-rw-rw-r--   0 xianghui   (501) staff       (20)     1964 2024-05-09 00:35:34.000000 txm_sandbox-0.3.1.post1/README.md
+-rwxrwxr-x   0 xianghui   (501) staff       (20)     2565 2024-04-27 23:21:56.000000 txm_sandbox-0.3.1.post1/TXM_GUI2.ipynb
+-rw-r--r--   0 xianghui   (501) staff       (20)       38 2024-05-18 02:17:05.320318 txm_sandbox-0.3.1.post1/setup.cfg
+-rw-rw-r--   0 xianghui   (501) staff       (20)     1130 2024-05-18 02:14:38.000000 txm_sandbox-0.3.1.post1/setup.py
+drwxr-xr-x   0 xianghui   (501) staff       (20)        0 2024-05-18 02:17:05.289595 txm_sandbox-0.3.1.post1/txm_sandbox/
+-rw-rw-r--   0 xianghui   (501) staff       (20)      181 2024-04-28 16:42:36.000000 txm_sandbox-0.3.1.post1/txm_sandbox/__init__.py
+drwxr-xr-x   0 xianghui   (501) staff       (20)        0 2024-05-18 02:17:05.291864 txm_sandbox-0.3.1.post1/txm_sandbox/config/
+-rw-rw-r--   0 xianghui   (501) staff       (20)     5092 2024-04-28 16:42:36.000000 txm_sandbox-0.3.1.post1/txm_sandbox/config/XANES2D_GUI_config.json
+-rw-rw-r--   0 xianghui   (501) staff       (20)      107 2024-04-28 16:42:36.000000 txm_sandbox-0.3.1.post1/txm_sandbox/config/__init__.py
+-rw-rw-r--   0 xianghui   (501) staff       (20)       45 2024-04-28 16:42:36.000000 txm_sandbox-0.3.1.post1/txm_sandbox/config/analysis_tool_gui_cfg.json
+-rw-rw-r--   0 xianghui   (501) staff       (20)      497 2024-04-28 16:42:36.000000 txm_sandbox-0.3.1.post1/txm_sandbox/config/io_tomo_h5_data_structure.json
+-rw-rw-r--   0 xianghui   (501) staff       (20)      500 2024-04-28 16:42:36.000000 txm_sandbox-0.3.1.post1/txm_sandbox/config/io_xanes2D_h5_data_structure.json
+-rw-rw-r--   0 xianghui   (501) staff       (20)      616 2024-04-28 16:42:36.000000 txm_sandbox-0.3.1.post1/txm_sandbox/config/io_xanes3D_h5_data_structure.json
+drwxr-xr-x   0 xianghui   (501) staff       (20)        0 2024-05-18 02:17:05.293368 txm_sandbox-0.3.1.post1/txm_sandbox/dicts/
+-rw-rw-r--   0 xianghui   (501) staff       (20)      107 2024-04-28 16:42:36.000000 txm_sandbox-0.3.1.post1/txm_sandbox/dicts/__init__.py
+-rw-rw-r--   0 xianghui   (501) staff       (20)     3848 2024-04-28 16:42:36.000000 txm_sandbox-0.3.1.post1/txm_sandbox/dicts/config_dict.py
+-rw-rw-r--   0 xianghui   (501) staff       (20)    61110 2024-04-28 16:42:36.000000 txm_sandbox-0.3.1.post1/txm_sandbox/dicts/customized_struct_dict.py
+-rw-rw-r--   0 xianghui   (501) staff       (20)      755 2024-04-28 16:42:36.000000 txm_sandbox-0.3.1.post1/txm_sandbox/dicts/sklearn_opt_dict.py
+-rw-rw-r--   0 xianghui   (501) staff       (20)      583 2024-04-28 16:42:36.000000 txm_sandbox-0.3.1.post1/txm_sandbox/dicts/xanes_analysis_dict.py
+drwxr-xr-x   0 xianghui   (501) staff       (20)        0 2024-05-18 02:17:05.293799 txm_sandbox-0.3.1.post1/txm_sandbox/external/
+-rw-rw-r--   0 xianghui   (501) staff       (20)      107 2024-04-28 16:42:36.000000 txm_sandbox-0.3.1.post1/txm_sandbox/external/__init__.py
+-rw-rw-r--   0 xianghui   (501) staff       (20)      253 2024-04-28 16:42:36.000000 txm_sandbox-0.3.1.post1/txm_sandbox/external/user_io.py
+drwxr-xr-x   0 xianghui   (501) staff       (20)        0 2024-05-18 02:17:05.302309 txm_sandbox-0.3.1.post1/txm_sandbox/gui/
+-rw-rw-r--   0 xianghui   (501) staff       (20)      107 2024-04-28 16:42:36.000000 txm_sandbox-0.3.1.post1/txm_sandbox/gui/__init__.py
+-rw-rw-r--   0 xianghui   (501) staff       (20)    32500 2024-04-28 16:42:36.000000 txm_sandbox-0.3.1.post1/txm_sandbox/gui/conv_data_gui.py
+-rw-rw-r--   0 xianghui   (501) staff       (20)    74137 2024-04-28 16:42:36.000000 txm_sandbox-0.3.1.post1/txm_sandbox/gui/gen_algn_gui.py
+-rw-rw-r--   0 xianghui   (501) staff       (20)    79148 2024-05-12 04:56:04.000000 txm_sandbox-0.3.1.post1/txm_sandbox/gui/gui_components.py
+-rw-rw-r--   0 xianghui   (501) staff       (20)    36752 2024-04-28 16:42:36.000000 txm_sandbox-0.3.1.post1/txm_sandbox/gui/io_config_gui.py
+-rw-rw-r--   0 xianghui   (501) staff       (20)    15709 2024-04-28 16:42:36.000000 txm_sandbox-0.3.1.post1/txm_sandbox/gui/main_gui.py
+-rw-rw-r--   0 xianghui   (501) staff       (20)      795 2024-04-28 16:42:36.000000 txm_sandbox-0.3.1.post1/txm_sandbox/gui/misc_gui.py
+-rw-rw-r--   0 xianghui   (501) staff       (20)   169879 2024-04-28 16:42:36.000000 txm_sandbox-0.3.1.post1/txm_sandbox/gui/tomo_gui.py
+-rw-rw-r--   0 xianghui   (501) staff       (20)   204783 2024-04-28 16:42:36.000000 txm_sandbox-0.3.1.post1/txm_sandbox/gui/xanes2D_gui.py
+-rw-rw-r--   0 xianghui   (501) staff       (20)   202060 2024-04-28 16:42:36.000000 txm_sandbox-0.3.1.post1/txm_sandbox/gui/xanes3D_gui.py
+-rw-rw-r--   0 xianghui   (501) staff       (20)    91679 2024-04-28 16:42:36.000000 txm_sandbox-0.3.1.post1/txm_sandbox/gui/xanes_analysis_gui.py
+-rw-rw-r--   0 xianghui   (501) staff       (20)   203257 2024-04-28 16:42:36.000000 txm_sandbox-0.3.1.post1/txm_sandbox/gui/xanes_fitting_gui.py
+drwxr-xr-x   0 xianghui   (501) staff       (20)        0 2024-05-18 02:17:05.303271 txm_sandbox-0.3.1.post1/txm_sandbox/napari_gui/
+-rw-rw-r--   0 xianghui   (501) staff       (20)      181 2024-05-14 04:58:24.000000 txm_sandbox-0.3.1.post1/txm_sandbox/napari_gui/__init__.py
+drwxr-xr-x   0 xianghui   (501) staff       (20)        0 2024-05-18 02:17:05.304953 txm_sandbox-0.3.1.post1/txm_sandbox/napari_gui/configs/
+-rw-rw-r--   0 xianghui   (501) staff       (20)      181 2024-05-14 04:58:24.000000 txm_sandbox-0.3.1.post1/txm_sandbox/napari_gui/configs/__init__.py
+-rw-rw-r--   0 xianghui   (501) staff       (20)      979 2024-05-14 04:58:24.000000 txm_sandbox-0.3.1.post1/txm_sandbox/napari_gui/configs/txm_simple_gui_script_cfg.json
+-rw-rw-r--   0 xianghui   (501) staff       (20)      957 2024-05-14 04:58:24.000000 txm_sandbox-0.3.1.post1/txm_sandbox/napari_gui/configs/xanes2d_image_autoreg_cfg.json
+-rw-rw-r--   0 xianghui   (501) staff       (20)      899 2024-05-14 04:58:24.000000 txm_sandbox-0.3.1.post1/txm_sandbox/napari_gui/configs/xanes3d_tomo_autocent_cfg.json
+-rw-rw-r--   0 xianghui   (501) staff       (20)     2389 2024-05-14 04:58:24.000000 txm_sandbox-0.3.1.post1/txm_sandbox/napari_gui/configs/xanes3d_tomo_template_cfg.json
+-rw-rw-r--   0 xianghui   (501) staff       (20)     1362 2024-05-14 04:58:24.000000 txm_sandbox-0.3.1.post1/txm_sandbox/napari_gui/configs/xanes_proc_data_struct_cfg.json
+drwxr-xr-x   0 xianghui   (501) staff       (20)        0 2024-05-18 02:17:05.305330 txm_sandbox-0.3.1.post1/txm_sandbox/napari_gui/dicts/
+-rw-rw-r--   0 xianghui   (501) staff       (20)      181 2024-05-14 04:58:24.000000 txm_sandbox-0.3.1.post1/txm_sandbox/napari_gui/dicts/__init__.py
+-rw-r--r--   0 xianghui   (501) staff       (20)     8853 2024-05-14 04:58:24.000000 txm_sandbox-0.3.1.post1/txm_sandbox/napari_gui/dicts/data_struct_dict.py
+drwxr-xr-x   0 xianghui   (501) staff       (20)        0 2024-05-18 02:17:05.309235 txm_sandbox-0.3.1.post1/txm_sandbox/napari_gui/guis/
+-rw-rw-r--   0 xianghui   (501) staff       (20)      106 2024-05-14 04:58:24.000000 txm_sandbox-0.3.1.post1/txm_sandbox/napari_gui/guis/__init__.py
+-rw-rw-r--   0 xianghui   (501) staff       (20)    16170 2024-05-14 04:58:24.000000 txm_sandbox-0.3.1.post1/txm_sandbox/napari_gui/guis/appl_mask_gui.py
+-rw-rw-r--   0 xianghui   (501) staff       (20)     9799 2024-05-14 04:58:24.000000 txm_sandbox-0.3.1.post1/txm_sandbox/napari_gui/guis/convert_data_gui.py
+-rw-r--r--   0 xianghui   (501) staff       (20)     3929 2024-05-14 04:58:24.000000 txm_sandbox-0.3.1.post1/txm_sandbox/napari_gui/guis/extra_io_gui.py
+-rw-r--r--   0 xianghui   (501) staff       (20)    32957 2024-05-14 07:59:24.000000 txm_sandbox-0.3.1.post1/txm_sandbox/napari_gui/guis/tomo_gui.py
+-rw-r--r--   0 xianghui   (501) staff       (20)    24243 2024-05-14 04:58:24.000000 txm_sandbox-0.3.1.post1/txm_sandbox/napari_gui/guis/xanes_fit_gui.py
+-rw-r--r--   0 xianghui   (501) staff       (20)    67248 2024-05-18 02:01:00.000000 txm_sandbox-0.3.1.post1/txm_sandbox/napari_gui/guis/xanes_reg_gui.py
+-rw-rw-r--   0 xianghui   (501) staff       (20)    16157 2024-05-14 04:58:24.000000 txm_sandbox-0.3.1.post1/txm_sandbox/napari_gui/guis/xanes_vis_gui.py
+drwxr-xr-x   0 xianghui   (501) staff       (20)        0 2024-05-18 02:17:05.312505 txm_sandbox-0.3.1.post1/txm_sandbox/napari_gui/scripts/
+-rw-rw-r--   0 xianghui   (501) staff       (20)      107 2024-05-14 04:58:24.000000 txm_sandbox-0.3.1.post1/txm_sandbox/napari_gui/scripts/__init__.py
+-rw-rw-r--   0 xianghui   (501) staff       (20)     4223 2024-05-14 05:10:46.000000 txm_sandbox-0.3.1.post1/txm_sandbox/napari_gui/scripts/aps_xanes2d_image_autoreg_cmd.py
+-rw-rw-r--   0 xianghui   (501) staff       (20)      650 2024-05-14 04:58:24.000000 txm_sandbox-0.3.1.post1/txm_sandbox/napari_gui/scripts/tomo_batch_recon_cmd.py
+-rw-rw-r--   0 xianghui   (501) staff       (20)      599 2024-05-14 04:58:24.000000 txm_sandbox-0.3.1.post1/txm_sandbox/napari_gui/scripts/tomo_recon_cmd.py
+-rw-rw-r--   0 xianghui   (501) staff       (20)    15251 2024-05-14 04:58:24.000000 txm_sandbox-0.3.1.post1/txm_sandbox/napari_gui/scripts/xanes2D_fit_cmd.py
+-rw-rw-r--   0 xianghui   (501) staff       (20)     2441 2024-05-14 04:58:24.000000 txm_sandbox-0.3.1.post1/txm_sandbox/napari_gui/scripts/xanes2d_image_autoreg_cmd.py
+-rw-rw-r--   0 xianghui   (501) staff       (20)    16610 2024-05-14 04:58:24.000000 txm_sandbox-0.3.1.post1/txm_sandbox/napari_gui/scripts/xanes3D_fit_cmd.py
+-rw-rw-r--   0 xianghui   (501) staff       (20)     1197 2024-05-14 04:58:24.000000 txm_sandbox-0.3.1.post1/txm_sandbox/napari_gui/scripts/xanes3d_tomo_autocent_cmd.py
+-rw-r--r--   0 xianghui   (501) staff       (20)     2029 2024-05-14 04:58:24.000000 txm_sandbox-0.3.1.post1/txm_sandbox/napari_gui/scripts/xnaes2d_image_autoreg_cmd.py
+-rw-r--r--   0 xianghui   (501) staff       (20)     1533 2024-05-14 04:58:24.000000 txm_sandbox-0.3.1.post1/txm_sandbox/napari_gui/txm_gui.py
+drwxr-xr-x   0 xianghui   (501) staff       (20)        0 2024-05-18 02:17:05.313941 txm_sandbox-0.3.1.post1/txm_sandbox/napari_gui/utils/
+-rw-rw-r--   0 xianghui   (501) staff       (20)      181 2024-05-14 04:58:24.000000 txm_sandbox-0.3.1.post1/txm_sandbox/napari_gui/utils/__init__.py
+-rw-r--r--   0 xianghui   (501) staff       (20)     5157 2024-05-14 04:58:24.000000 txm_sandbox-0.3.1.post1/txm_sandbox/napari_gui/utils/ext_io_lib.py
+-rw-rw-r--   0 xianghui   (501) staff       (20)     1264 2024-05-14 04:58:24.000000 txm_sandbox-0.3.1.post1/txm_sandbox/napari_gui/utils/io.py
+-rw-r--r--   0 xianghui   (501) staff       (20)    10709 2024-05-16 05:38:21.000000 txm_sandbox-0.3.1.post1/txm_sandbox/napari_gui/utils/misc.py
+drwxr-xr-x   0 xianghui   (501) staff       (20)        0 2024-05-18 02:17:05.314422 txm_sandbox-0.3.1.post1/txm_sandbox/tmp/
+-rw-rw-r--   0 xianghui   (501) staff       (20)      107 2024-04-28 16:42:36.000000 txm_sandbox-0.3.1.post1/txm_sandbox/tmp/__init__.py
+-rw-rw-r--   0 xianghui   (501) staff       (20)       69 2024-04-28 16:42:36.000000 txm_sandbox-0.3.1.post1/txm_sandbox/tmp/readme.txt
+drwxr-xr-x   0 xianghui   (501) staff       (20)        0 2024-05-18 02:17:05.319569 txm_sandbox-0.3.1.post1/txm_sandbox/utils/
+-rw-rw-r--   0 xianghui   (501) staff       (20)      107 2024-04-28 16:42:36.000000 txm_sandbox-0.3.1.post1/txm_sandbox/utils/__init__.py
+-rw-rw-r--   0 xianghui   (501) staff       (20)    16672 2024-04-28 16:42:36.000000 txm_sandbox-0.3.1.post1/txm_sandbox/utils/io.py
+-rw-rw-r--   0 xianghui   (501) staff       (20)    14410 2024-04-28 16:42:36.000000 txm_sandbox-0.3.1.post1/txm_sandbox/utils/lineshapes.py
+-rwxrwxr-x   0 xianghui   (501) staff       (20)     4246 2024-04-28 16:42:36.000000 txm_sandbox-0.3.1.post1/txm_sandbox/utils/misc.py
+-rw-rw-r--   0 xianghui   (501) staff       (20)     1439 2024-04-28 16:42:36.000000 txm_sandbox-0.3.1.post1/txm_sandbox/utils/plotlib.py
+-rw-rw-r--   0 xianghui   (501) staff       (20)    61837 2024-04-28 16:42:36.000000 txm_sandbox-0.3.1.post1/txm_sandbox/utils/reg_algs.py
+-rw-rw-r--   0 xianghui   (501) staff       (20)    70498 2024-04-28 16:42:36.000000 txm_sandbox-0.3.1.post1/txm_sandbox/utils/tomo_recon_tools.py
+-rw-rw-r--   0 xianghui   (501) staff       (20)    41021 2024-04-28 16:42:36.000000 txm_sandbox-0.3.1.post1/txm_sandbox/utils/xanes_analysis.py
+-rw-rw-r--   0 xianghui   (501) staff       (20)     2342 2024-04-28 16:42:36.000000 txm_sandbox-0.3.1.post1/txm_sandbox/utils/xanes_image_utils.py
+-rw-rw-r--   0 xianghui   (501) staff       (20)    23436 2024-04-28 16:42:36.000000 txm_sandbox-0.3.1.post1/txm_sandbox/utils/xanes_math.py
+-rw-rw-r--   0 xianghui   (501) staff       (20)     6083 2024-04-28 16:42:36.000000 txm_sandbox-0.3.1.post1/txm_sandbox/utils/xanes_post_analysis.py
+-rw-rw-r--   0 xianghui   (501) staff       (20)    84740 2024-05-18 02:00:43.000000 txm_sandbox-0.3.1.post1/txm_sandbox/utils/xanes_regtools.py
+-rw-rw-r--   0 xianghui   (501) staff       (20)     3266 2024-04-28 16:42:36.000000 txm_sandbox-0.3.1.post1/txm_sandbox/utils/xanes_spectra_filters.py
+drwxr-xr-x   0 xianghui   (501) staff       (20)        0 2024-05-18 02:17:05.319881 txm_sandbox-0.3.1.post1/txm_sandbox.egg-info/
+-rw-r--r--   0 xianghui   (501) staff       (20)      712 2024-05-18 02:17:05.000000 txm_sandbox-0.3.1.post1/txm_sandbox.egg-info/PKG-INFO
+-rw-r--r--   0 xianghui   (501) staff       (20)     3196 2024-05-18 02:17:05.000000 txm_sandbox-0.3.1.post1/txm_sandbox.egg-info/SOURCES.txt
+-rw-r--r--   0 xianghui   (501) staff       (20)        1 2024-05-18 02:17:05.000000 txm_sandbox-0.3.1.post1/txm_sandbox.egg-info/dependency_links.txt
+-rw-r--r--   0 xianghui   (501) staff       (20)        1 2024-05-18 02:17:05.000000 txm_sandbox-0.3.1.post1/txm_sandbox.egg-info/not-zip-safe
+-rw-r--r--   0 xianghui   (501) staff       (20)      170 2024-05-18 02:17:05.000000 txm_sandbox-0.3.1.post1/txm_sandbox.egg-info/requires.txt
+-rw-r--r--   0 xianghui   (501) staff       (20)       12 2024-05-18 02:17:05.000000 txm_sandbox-0.3.1.post1/txm_sandbox.egg-info/top_level.txt
```

### Comparing `txm_sandbox-0.3.1/LICENSE` & `txm_sandbox-0.3.1.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `txm_sandbox-0.3.1/PKG-INFO` & `txm_sandbox-0.3.1.post1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: txm_sandbox
-Version: 0.3.1
+Version: 0.3.1.post1
 Summary: Integrated Spectro-Imaging Analysis Toolbox
 Home-page: https://github.com/xianghuix/TXM_Sandbox
 Author: Xianghui Xiao
 Author-email: xianghuix@gmail.com
 License: MIT
 License-File: LICENSE
 Requires-Dist: python>=3.11
```

### Comparing `txm_sandbox-0.3.1/README.md` & `txm_sandbox-0.3.1.post1/README.md`

 * *Files identical despite different names*

### Comparing `txm_sandbox-0.3.1/TXM_GUI2.ipynb` & `txm_sandbox-0.3.1.post1/TXM_GUI2.ipynb`

 * *Files identical despite different names*

### Comparing `txm_sandbox-0.3.1/setup.py` & `txm_sandbox-0.3.1.post1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 @author: xiao
 """
 
 from setuptools import setup, find_packages
 
 setup(name='txm_sandbox',
-      version='0.3.1',
+      version='0.3.1.post1',
       description='Integrated Spectro-Imaging Analysis Toolbox',
       url='https://github.com/xianghuix/TXM_Sandbox',
       author='Xianghui Xiao',
       author_email='xianghuix@gmail.com',
       license='MIT',
       packages=find_packages(),
       install_requires=[
```

### Comparing `txm_sandbox-0.3.1/txm_sandbox/config/XANES2D_GUI_config.json` & `txm_sandbox-0.3.1.post1/txm_sandbox/config/XANES2D_GUI_config.json`

 * *Files identical despite different names*

### Comparing `txm_sandbox-0.3.1/txm_sandbox/config/io_xanes3D_h5_data_structure.json` & `txm_sandbox-0.3.1.post1/txm_sandbox/config/io_xanes3D_h5_data_structure.json`

 * *Files identical despite different names*

### Comparing `txm_sandbox-0.3.1/txm_sandbox/dicts/config_dict.py` & `txm_sandbox-0.3.1.post1/txm_sandbox/dicts/config_dict.py`

 * *Files identical despite different names*

### Comparing `txm_sandbox-0.3.1/txm_sandbox/dicts/customized_struct_dict.py` & `txm_sandbox-0.3.1.post1/txm_sandbox/dicts/customized_struct_dict.py`

 * *Files identical despite different names*

### Comparing `txm_sandbox-0.3.1/txm_sandbox/dicts/sklearn_opt_dict.py` & `txm_sandbox-0.3.1.post1/txm_sandbox/dicts/sklearn_opt_dict.py`

 * *Files identical despite different names*

### Comparing `txm_sandbox-0.3.1/txm_sandbox/dicts/xanes_analysis_dict.py` & `txm_sandbox-0.3.1.post1/txm_sandbox/dicts/xanes_analysis_dict.py`

 * *Files identical despite different names*

### Comparing `txm_sandbox-0.3.1/txm_sandbox/gui/conv_data_gui.py` & `txm_sandbox-0.3.1.post1/txm_sandbox/gui/conv_data_gui.py`

 * *Files identical despite different names*

### Comparing `txm_sandbox-0.3.1/txm_sandbox/gui/gen_algn_gui.py` & `txm_sandbox-0.3.1.post1/txm_sandbox/gui/gen_algn_gui.py`

 * *Files identical despite different names*

### Comparing `txm_sandbox-0.3.1/txm_sandbox/gui/gui_components.py` & `txm_sandbox-0.3.1.post1/txm_sandbox/gui/gui_components.py`

 * *Files identical despite different names*

### Comparing `txm_sandbox-0.3.1/txm_sandbox/gui/io_config_gui.py` & `txm_sandbox-0.3.1.post1/txm_sandbox/gui/io_config_gui.py`

 * *Files identical despite different names*

### Comparing `txm_sandbox-0.3.1/txm_sandbox/gui/main_gui.py` & `txm_sandbox-0.3.1.post1/txm_sandbox/gui/main_gui.py`

 * *Files identical despite different names*

### Comparing `txm_sandbox-0.3.1/txm_sandbox/gui/misc_gui.py` & `txm_sandbox-0.3.1.post1/txm_sandbox/gui/misc_gui.py`

 * *Files identical despite different names*

### Comparing `txm_sandbox-0.3.1/txm_sandbox/gui/tomo_gui.py` & `txm_sandbox-0.3.1.post1/txm_sandbox/gui/tomo_gui.py`

 * *Files identical despite different names*

### Comparing `txm_sandbox-0.3.1/txm_sandbox/gui/xanes2D_gui.py` & `txm_sandbox-0.3.1.post1/txm_sandbox/gui/xanes2D_gui.py`

 * *Files identical despite different names*

### Comparing `txm_sandbox-0.3.1/txm_sandbox/gui/xanes3D_gui.py` & `txm_sandbox-0.3.1.post1/txm_sandbox/gui/xanes3D_gui.py`

 * *Files identical despite different names*

### Comparing `txm_sandbox-0.3.1/txm_sandbox/gui/xanes_analysis_gui.py` & `txm_sandbox-0.3.1.post1/txm_sandbox/gui/xanes_analysis_gui.py`

 * *Files identical despite different names*

### Comparing `txm_sandbox-0.3.1/txm_sandbox/gui/xanes_fitting_gui.py` & `txm_sandbox-0.3.1.post1/txm_sandbox/gui/xanes_fitting_gui.py`

 * *Files identical despite different names*

### Comparing `txm_sandbox-0.3.1/txm_sandbox/napari_gui/configs/txm_simple_gui_script_cfg.json` & `txm_sandbox-0.3.1.post1/txm_sandbox/napari_gui/configs/txm_simple_gui_script_cfg.json`

 * *Files identical despite different names*

### Comparing `txm_sandbox-0.3.1/txm_sandbox/napari_gui/configs/xanes2d_image_autoreg_cfg.json` & `txm_sandbox-0.3.1.post1/txm_sandbox/napari_gui/configs/xanes2d_image_autoreg_cfg.json`

 * *Files identical despite different names*

### Comparing `txm_sandbox-0.3.1/txm_sandbox/napari_gui/configs/xanes3d_tomo_autocent_cfg.json` & `txm_sandbox-0.3.1.post1/txm_sandbox/napari_gui/configs/xanes3d_tomo_autocent_cfg.json`

 * *Files identical despite different names*

### Comparing `txm_sandbox-0.3.1/txm_sandbox/napari_gui/configs/xanes3d_tomo_template_cfg.json` & `txm_sandbox-0.3.1.post1/txm_sandbox/napari_gui/configs/xanes3d_tomo_template_cfg.json`

 * *Files identical despite different names*

### Comparing `txm_sandbox-0.3.1/txm_sandbox/napari_gui/configs/xanes_proc_data_struct_cfg.json` & `txm_sandbox-0.3.1.post1/txm_sandbox/napari_gui/configs/xanes_proc_data_struct_cfg.json`

 * *Files identical despite different names*

### Comparing `txm_sandbox-0.3.1/txm_sandbox/napari_gui/dicts/data_struct_dict.py` & `txm_sandbox-0.3.1.post1/txm_sandbox/napari_gui/dicts/data_struct_dict.py`

 * *Files identical despite different names*

### Comparing `txm_sandbox-0.3.1/txm_sandbox/napari_gui/guis/appl_mask_gui.py` & `txm_sandbox-0.3.1.post1/txm_sandbox/napari_gui/guis/appl_mask_gui.py`

 * *Files identical despite different names*

### Comparing `txm_sandbox-0.3.1/txm_sandbox/napari_gui/guis/convert_data_gui.py` & `txm_sandbox-0.3.1.post1/txm_sandbox/napari_gui/guis/convert_data_gui.py`

 * *Files identical despite different names*

### Comparing `txm_sandbox-0.3.1/txm_sandbox/napari_gui/guis/extra_io_gui.py` & `txm_sandbox-0.3.1.post1/txm_sandbox/napari_gui/guis/extra_io_gui.py`

 * *Files identical despite different names*

### Comparing `txm_sandbox-0.3.1/txm_sandbox/napari_gui/guis/tomo_gui.py` & `txm_sandbox-0.3.1.post1/txm_sandbox/napari_gui/guis/tomo_gui.py`

 * *Files identical despite different names*

### Comparing `txm_sandbox-0.3.1/txm_sandbox/napari_gui/guis/xanes_fit_gui.py` & `txm_sandbox-0.3.1.post1/txm_sandbox/napari_gui/guis/xanes_fit_gui.py`

 * *Files identical despite different names*

### Comparing `txm_sandbox-0.3.1/txm_sandbox/napari_gui/guis/xanes_reg_gui.py` & `txm_sandbox-0.3.1.post1/txm_sandbox/napari_gui/guis/xanes_reg_gui.py`

 * *Files 0% similar despite different names*

```diff
@@ -1073,14 +1073,15 @@
             )
         with open(cfg_fn, "w") as f:
             json.dump(tem, f, indent=4, separators=(",", ": "))
 
         xanes2d_image_autocent_cfg["data"]["im_id_s"] = self.rec_roiz.value[0]
         xanes2d_image_autocent_cfg["data"]["im_id_e"] = self.rec_roiz.value[1]
         xanes2d_image_autocent_cfg["data"]["im_id_fixed"] = self.ref_sli.value
+
         if self._continue_run_confirmed:
             xanes2d_image_autocent_cfg["reg_type"] = "align"
             xanes2d_image_autocent_cfg["data"]["roi"] = [
                 self.rec_roiy.value[0],
                 self.rec_roiy.value[1],
                 self.rec_roix.value[0],
                 self.rec_roix.value[1],
```

### Comparing `txm_sandbox-0.3.1/txm_sandbox/napari_gui/guis/xanes_vis_gui.py` & `txm_sandbox-0.3.1.post1/txm_sandbox/napari_gui/guis/xanes_vis_gui.py`

 * *Files identical despite different names*

### Comparing `txm_sandbox-0.3.1/txm_sandbox/napari_gui/scripts/aps_xanes2d_image_autoreg_cmd.py` & `txm_sandbox-0.3.1.post1/txm_sandbox/napari_gui/scripts/aps_xanes2d_image_autoreg_cmd.py`

 * *Files identical despite different names*

### Comparing `txm_sandbox-0.3.1/txm_sandbox/napari_gui/scripts/tomo_batch_recon_cmd.py` & `txm_sandbox-0.3.1.post1/txm_sandbox/napari_gui/scripts/tomo_batch_recon_cmd.py`

 * *Files identical despite different names*

### Comparing `txm_sandbox-0.3.1/txm_sandbox/napari_gui/scripts/tomo_recon_cmd.py` & `txm_sandbox-0.3.1.post1/txm_sandbox/napari_gui/scripts/tomo_recon_cmd.py`

 * *Files identical despite different names*

### Comparing `txm_sandbox-0.3.1/txm_sandbox/napari_gui/scripts/xanes2D_fit_cmd.py` & `txm_sandbox-0.3.1.post1/txm_sandbox/napari_gui/scripts/xanes2D_fit_cmd.py`

 * *Files identical despite different names*

### Comparing `txm_sandbox-0.3.1/txm_sandbox/napari_gui/scripts/xanes2d_image_autoreg_cmd.py` & `txm_sandbox-0.3.1.post1/txm_sandbox/napari_gui/scripts/xanes2d_image_autoreg_cmd.py`

 * *Files identical despite different names*

### Comparing `txm_sandbox-0.3.1/txm_sandbox/napari_gui/scripts/xanes3D_fit_cmd.py` & `txm_sandbox-0.3.1.post1/txm_sandbox/napari_gui/scripts/xanes3D_fit_cmd.py`

 * *Files identical despite different names*

### Comparing `txm_sandbox-0.3.1/txm_sandbox/napari_gui/scripts/xanes3d_tomo_autocent_cmd.py` & `txm_sandbox-0.3.1.post1/txm_sandbox/napari_gui/scripts/xanes3d_tomo_autocent_cmd.py`

 * *Files identical despite different names*

### Comparing `txm_sandbox-0.3.1/txm_sandbox/napari_gui/scripts/xnaes2d_image_autoreg_cmd.py` & `txm_sandbox-0.3.1.post1/txm_sandbox/napari_gui/scripts/xnaes2d_image_autoreg_cmd.py`

 * *Files identical despite different names*

### Comparing `txm_sandbox-0.3.1/txm_sandbox/napari_gui/txm_gui.py` & `txm_sandbox-0.3.1.post1/txm_sandbox/napari_gui/txm_gui.py`

 * *Files identical despite different names*

### Comparing `txm_sandbox-0.3.1/txm_sandbox/napari_gui/utils/ext_io_lib.py` & `txm_sandbox-0.3.1.post1/txm_sandbox/napari_gui/utils/ext_io_lib.py`

 * *Files identical despite different names*

### Comparing `txm_sandbox-0.3.1/txm_sandbox/napari_gui/utils/io.py` & `txm_sandbox-0.3.1.post1/txm_sandbox/napari_gui/utils/io.py`

 * *Files identical despite different names*

### Comparing `txm_sandbox-0.3.1/txm_sandbox/napari_gui/utils/misc.py` & `txm_sandbox-0.3.1.post1/txm_sandbox/napari_gui/utils/misc.py`

 * *Files 2% similar despite different names*

```diff
@@ -162,15 +162,16 @@
     if mode == "auto_cen":
         rm_gui_viewers(viewer, ["auto_cen_roi"])
         if "recon_roi" in viewer.layers:
             viewer.layers["recon_roi"].visible = False
         if "xanes_roi" in viewer.layers:
             viewer.layers["xanes_roi"].visible = False
         if gui.auto_cen_dft_roi.value:
-            dim = viewer.layers["tomo_viewer"].data.shape
+            # dim = viewer.layers["tomo_viewer"].data.shape
+            dim = viewer.layers["xanes_raw_viewer"].data.shape
             ellipse_data = [
                 [int(dim[0] * 0.5), int(dim[1] * 0.5)],
                 [int(dim[0] * 0.45), int(dim[1] * 0.45)],
             ]
             viewer.add_shapes(
                 ellipse_data,
                 shape_type="ellipse",
@@ -187,15 +188,16 @@
                 roi_coor,
                 shape_type="rectangle",
                 edge_color="green",
                 edge_width=3,
                 face_color="transparent",
                 name="auto_cen_roi",
             )
-        viewer.layers["tomo_viewer"].refresh()
+        # viewer.layers["tomo_viewer"].refresh()
+        viewer.layers["xanes_raw_viewer"].refresh()
     elif mode == "recon_roi":
         [xs, xe] = gui.rec_roix.value
         [ys, ye] = gui.rec_roiy.value
         roi_coor = [[ys, xs], [ys, xe], [ye, xe], [ye, xs]]
         rm_gui_viewers(viewer, ["recon_roi"])
         if "auto_cen_roi" in viewer.layers:
             viewer.layers["auto_cen_roi"].visible = False
```

### Comparing `txm_sandbox-0.3.1/txm_sandbox/utils/io.py` & `txm_sandbox-0.3.1.post1/txm_sandbox/utils/io.py`

 * *Files identical despite different names*

### Comparing `txm_sandbox-0.3.1/txm_sandbox/utils/lineshapes.py` & `txm_sandbox-0.3.1.post1/txm_sandbox/utils/lineshapes.py`

 * *Files identical despite different names*

### Comparing `txm_sandbox-0.3.1/txm_sandbox/utils/misc.py` & `txm_sandbox-0.3.1.post1/txm_sandbox/utils/misc.py`

 * *Files identical despite different names*

### Comparing `txm_sandbox-0.3.1/txm_sandbox/utils/plotlib.py` & `txm_sandbox-0.3.1.post1/txm_sandbox/utils/plotlib.py`

 * *Files identical despite different names*

### Comparing `txm_sandbox-0.3.1/txm_sandbox/utils/reg_algs.py` & `txm_sandbox-0.3.1.post1/txm_sandbox/utils/reg_algs.py`

 * *Files identical despite different names*

### Comparing `txm_sandbox-0.3.1/txm_sandbox/utils/tomo_recon_tools.py` & `txm_sandbox-0.3.1.post1/txm_sandbox/utils/tomo_recon_tools.py`

 * *Files identical despite different names*

### Comparing `txm_sandbox-0.3.1/txm_sandbox/utils/xanes_analysis.py` & `txm_sandbox-0.3.1.post1/txm_sandbox/utils/xanes_analysis.py`

 * *Files identical despite different names*

### Comparing `txm_sandbox-0.3.1/txm_sandbox/utils/xanes_image_utils.py` & `txm_sandbox-0.3.1.post1/txm_sandbox/utils/xanes_image_utils.py`

 * *Files identical despite different names*

### Comparing `txm_sandbox-0.3.1/txm_sandbox/utils/xanes_math.py` & `txm_sandbox-0.3.1.post1/txm_sandbox/utils/xanes_math.py`

 * *Files identical despite different names*

### Comparing `txm_sandbox-0.3.1/txm_sandbox/utils/xanes_post_analysis.py` & `txm_sandbox-0.3.1.post1/txm_sandbox/utils/xanes_post_analysis.py`

 * *Files identical despite different names*

### Comparing `txm_sandbox-0.3.1/txm_sandbox/utils/xanes_regtools.py` & `txm_sandbox-0.3.1.post1/txm_sandbox/utils/xanes_regtools.py`

 * *Files 0% similar despite different names*

```diff
@@ -120,20 +120,16 @@
 
         self.eng_list = reg_cfg["meta"]["eng_list"]
 
         if self.data_type == "3D_XANES":
             self.anchor_loc = self.xanes3D_scn_ids.index(self.im_id_fxd)
             self.data_pnts = len(self.xanes3D_scn_ids)
         else:
-            self.anchor_loc = self.xanes3D_scn_ids.index(
-                self.im_id_fxd
-            ) - self.xanes3D_scn_ids.index(self.im_id_s)
-            self.data_pnts = self.xanes3D_scn_ids.index(
-                self.im_id_e
-            ) - self.xanes3D_scn_ids.index(self.im_id_s)
+            self.anchor_loc = self.im_id_fxd - self.im_id_s
+            self.data_pnts = self.im_id_e - self.im_id_s
         self.sav_dir = str(Path(self.sav_fn).parent)
         self.ref_im = None
         self.im = None
         self.msk = None
         self.eng_dict = {}
         self.im_ids_dict = {}
```

### Comparing `txm_sandbox-0.3.1/txm_sandbox/utils/xanes_spectra_filters.py` & `txm_sandbox-0.3.1.post1/txm_sandbox/utils/xanes_spectra_filters.py`

 * *Files identical despite different names*

### Comparing `txm_sandbox-0.3.1/txm_sandbox.egg-info/PKG-INFO` & `txm_sandbox-0.3.1.post1/txm_sandbox.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: txm_sandbox
-Version: 0.3.1
+Version: 0.3.1.post1
 Summary: Integrated Spectro-Imaging Analysis Toolbox
 Home-page: https://github.com/xianghuix/TXM_Sandbox
 Author: Xianghui Xiao
 Author-email: xianghuix@gmail.com
 License: MIT
 License-File: LICENSE
 Requires-Dist: python>=3.11
```

### Comparing `txm_sandbox-0.3.1/txm_sandbox.egg-info/SOURCES.txt` & `txm_sandbox-0.3.1.post1/txm_sandbox.egg-info/SOURCES.txt`

 * *Files identical despite different names*

