# Comparing `tmp/nqrduck-0.0.8.tar.gz` & `tmp/nqrduck-0.0.9.tar.gz`

## Comparing `nqrduck-0.0.8.tar` & `nqrduck-0.0.9.tar`

### file list

```diff
@@ -1,64 +1,64 @@
--rw-r--r--   0        0        0      729 2020-02-02 00:00:00.000000 nqrduck-0.0.8/CHANGELOG.md
--rw-r--r--   0        0        0      711 2020-02-02 00:00:00.000000 nqrduck-0.0.8/.github/workflows/main.yml
--rw-r--r--   0        0        0      908 2020-02-02 00:00:00.000000 nqrduck-0.0.8/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0      884 2020-02-02 00:00:00.000000 nqrduck-0.0.8/.github/workflows/ubuntu-python-package.yml
--rw-r--r--   0        0        0  1509874 2020-02-02 00:00:00.000000 nqrduck-0.0.8/docs/img/ui_structure_v2.png
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 nqrduck-0.0.8/src/nqrduck/__init__.py
--rw-r--r--   0        0        0     3649 2020-02-02 00:00:00.000000 nqrduck-0.0.8/src/nqrduck/__main__.py
--rw-r--r--   0        0        0     1971 2020-02-02 00:00:00.000000 nqrduck-0.0.8/src/nqrduck/assets/animations.py
--rw-r--r--   0        0        0     7236 2020-02-02 00:00:00.000000 nqrduck-0.0.8/src/nqrduck/assets/icons.py
--rw-r--r--   0        0        0    27758 2020-02-02 00:00:00.000000 nqrduck-0.0.8/src/nqrduck/assets/animations/DuckKick_128x128.gif
--rw-r--r--   0        0        0   115443 2020-02-02 00:00:00.000000 nqrduck-0.0.8/src/nqrduck/assets/animations/DuckSleep_128x128.gif
--rw-r--r--   0        0        0      202 2020-02-02 00:00:00.000000 nqrduck-0.0.8/src/nqrduck/assets/logos/ArrowLeft_12x12.png
--rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 nqrduck-0.0.8/src/nqrduck/assets/logos/ArrowRight_12x12.png
--rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 nqrduck-0.0.8/src/nqrduck/assets/logos/Attention_16x16.png
--rw-r--r--   0        0        0      222 2020-02-02 00:00:00.000000 nqrduck-0.0.8/src/nqrduck/assets/logos/Error_16x16.png
--rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 nqrduck-0.0.8/src/nqrduck/assets/logos/Garbage_12x12.png
--rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 nqrduck-0.0.8/src/nqrduck/assets/logos/Info_16x16.png
--rw-r--r--   0        0        0     1229 2020-02-02 00:00:00.000000 nqrduck-0.0.8/src/nqrduck/assets/logos/LabMallardnbg_32x32.png
--rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 nqrduck-0.0.8/src/nqrduck/assets/logos/Load_16x16.png
--rw-r--r--   0        0        0     1019 2020-02-02 00:00:00.000000 nqrduck-0.0.8/src/nqrduck/assets/logos/Logo_64x32.png
--rw-r--r--   0        0        0     2065 2020-02-02 00:00:00.000000 nqrduck-0.0.8/src/nqrduck/assets/logos/Logo_full.png
--rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 nqrduck-0.0.8/src/nqrduck/assets/logos/New_16x16.png
--rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 nqrduck-0.0.8/src/nqrduck/assets/logos/Pen_12x12.png
--rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 nqrduck-0.0.8/src/nqrduck/assets/logos/Play_16x16.png
--rw-r--r--   0        0        0      240 2020-02-02 00:00:00.000000 nqrduck-0.0.8/src/nqrduck/assets/logos/QuestionMark_16x16.png
--rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 nqrduck-0.0.8/src/nqrduck/assets/logos/Save_16x16.png
--rw-r--r--   0        0        0      249 2020-02-02 00:00:00.000000 nqrduck-0.0.8/src/nqrduck/assets/logos/Settings_16x16.png
--rw-r--r--   0        0        0      418 2020-02-02 00:00:00.000000 nqrduck-0.0.8/src/nqrduck/assets/pulseparameters/GateOff.png
--rw-r--r--   0        0        0      453 2020-02-02 00:00:00.000000 nqrduck-0.0.8/src/nqrduck/assets/pulseparameters/GateOn.png
--rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 nqrduck-0.0.8/src/nqrduck/assets/pulseparameters/RXOff.png
--rw-r--r--   0        0        0      354 2020-02-02 00:00:00.000000 nqrduck-0.0.8/src/nqrduck/assets/pulseparameters/RXOn.png
--rw-r--r--   0        0        0      346 2020-02-02 00:00:00.000000 nqrduck-0.0.8/src/nqrduck/assets/pulseparameters/TXCustom.png
--rw-r--r--   0        0        0      356 2020-02-02 00:00:00.000000 nqrduck-0.0.8/src/nqrduck/assets/pulseparameters/TXGauss.png
--rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 nqrduck-0.0.8/src/nqrduck/assets/pulseparameters/TXOff.png
--rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 nqrduck-0.0.8/src/nqrduck/assets/pulseparameters/TXRect.png
--rw-r--r--   0        0        0      387 2020-02-02 00:00:00.000000 nqrduck-0.0.8/src/nqrduck/assets/pulseparameters/TXSinc.png
--rw-r--r--   0        0        0     2609 2020-02-02 00:00:00.000000 nqrduck-0.0.8/src/nqrduck/contrib/mplwidget.py
--rw-r--r--   0        0        0    15929 2020-02-02 00:00:00.000000 nqrduck-0.0.8/src/nqrduck/core/install_wizard.py
--rw-r--r--   0        0        0     4587 2020-02-02 00:00:00.000000 nqrduck-0.0.8/src/nqrduck/core/main_controller.py
--rw-r--r--   0        0        0     6948 2020-02-02 00:00:00.000000 nqrduck-0.0.8/src/nqrduck/core/main_model.py
--rw-r--r--   0        0        0    31514 2020-02-02 00:00:00.000000 nqrduck-0.0.8/src/nqrduck/core/main_view.py
--rw-r--r--   0        0        0     4706 2020-02-02 00:00:00.000000 nqrduck-0.0.8/src/nqrduck/core/main_window.py
--rw-r--r--   0        0        0     1077 2020-02-02 00:00:00.000000 nqrduck-0.0.8/src/nqrduck/core/resources/logo.png
--rw-r--r--   0        0        0     2919 2020-02-02 00:00:00.000000 nqrduck-0.0.8/src/nqrduck/core/resources/main_window.ui
--rw-r--r--   0        0        0    28916 2020-02-02 00:00:00.000000 nqrduck-0.0.8/src/nqrduck/core/resources/font/AsepriteFont.ttf
--rw-r--r--   0        0        0      329 2020-02-02 00:00:00.000000 nqrduck-0.0.8/src/nqrduck/core/resources/font/LICENCE
--rw-r--r--   0        0        0     7172 2020-02-02 00:00:00.000000 nqrduck-0.0.8/src/nqrduck/helpers/duckwidgets.py
--rw-r--r--   0        0        0    18853 2020-02-02 00:00:00.000000 nqrduck-0.0.8/src/nqrduck/helpers/formbuilder.py
--rw-r--r--   0        0        0    12683 2020-02-02 00:00:00.000000 nqrduck-0.0.8/src/nqrduck/helpers/functions.py
--rw-r--r--   0        0        0      741 2020-02-02 00:00:00.000000 nqrduck-0.0.8/src/nqrduck/helpers/serializer.py
--rw-r--r--   0        0        0     3307 2020-02-02 00:00:00.000000 nqrduck-0.0.8/src/nqrduck/helpers/signalprocessing.py
--rw-r--r--   0        0        0     1458 2020-02-02 00:00:00.000000 nqrduck-0.0.8/src/nqrduck/helpers/unitconverter.py
--rw-r--r--   0        0        0     3669 2020-02-02 00:00:00.000000 nqrduck-0.0.8/src/nqrduck/helpers/validators.py
--rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 nqrduck-0.0.8/src/nqrduck/module/__init__.py
--rw-r--r--   0        0        0     2716 2020-02-02 00:00:00.000000 nqrduck-0.0.8/src/nqrduck/module/module.py
--rw-r--r--   0        0        0      806 2020-02-02 00:00:00.000000 nqrduck-0.0.8/src/nqrduck/module/module_controller.py
--rw-r--r--   0        0        0     2225 2020-02-02 00:00:00.000000 nqrduck-0.0.8/src/nqrduck/module/module_model.py
--rw-r--r--   0        0        0     3103 2020-02-02 00:00:00.000000 nqrduck-0.0.8/src/nqrduck/module/module_view.py
--rw-r--r--   0        0        0     1250 2020-02-02 00:00:00.000000 nqrduck-0.0.8/tests/test_load_module.py
--rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 nqrduck-0.0.8/.gitignore
--rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 nqrduck-0.0.8/LICENSE
--rw-r--r--   0        0        0     2371 2020-02-02 00:00:00.000000 nqrduck-0.0.8/README.md
--rw-r--r--   0        0        0     1860 2020-02-02 00:00:00.000000 nqrduck-0.0.8/pyproject.toml
--rw-r--r--   0        0        0     5456 2020-02-02 00:00:00.000000 nqrduck-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 nqrduck-0.0.9/CHANGELOG.md
+-rw-r--r--   0        0        0      711 2020-02-02 00:00:00.000000 nqrduck-0.0.9/.github/workflows/main.yml
+-rw-r--r--   0        0        0      908 2020-02-02 00:00:00.000000 nqrduck-0.0.9/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0      884 2020-02-02 00:00:00.000000 nqrduck-0.0.9/.github/workflows/ubuntu-python-package.yml
+-rw-r--r--   0        0        0  1509874 2020-02-02 00:00:00.000000 nqrduck-0.0.9/docs/img/ui_structure_v2.png
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 nqrduck-0.0.9/src/nqrduck/__init__.py
+-rw-r--r--   0        0        0     3508 2020-02-02 00:00:00.000000 nqrduck-0.0.9/src/nqrduck/__main__.py
+-rw-r--r--   0        0        0     1971 2020-02-02 00:00:00.000000 nqrduck-0.0.9/src/nqrduck/assets/animations.py
+-rw-r--r--   0        0        0     7236 2020-02-02 00:00:00.000000 nqrduck-0.0.9/src/nqrduck/assets/icons.py
+-rw-r--r--   0        0        0    27758 2020-02-02 00:00:00.000000 nqrduck-0.0.9/src/nqrduck/assets/animations/DuckKick_128x128.gif
+-rw-r--r--   0        0        0   115443 2020-02-02 00:00:00.000000 nqrduck-0.0.9/src/nqrduck/assets/animations/DuckSleep_128x128.gif
+-rw-r--r--   0        0        0      202 2020-02-02 00:00:00.000000 nqrduck-0.0.9/src/nqrduck/assets/logos/ArrowLeft_12x12.png
+-rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 nqrduck-0.0.9/src/nqrduck/assets/logos/ArrowRight_12x12.png
+-rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 nqrduck-0.0.9/src/nqrduck/assets/logos/Attention_16x16.png
+-rw-r--r--   0        0        0      222 2020-02-02 00:00:00.000000 nqrduck-0.0.9/src/nqrduck/assets/logos/Error_16x16.png
+-rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 nqrduck-0.0.9/src/nqrduck/assets/logos/Garbage_12x12.png
+-rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 nqrduck-0.0.9/src/nqrduck/assets/logos/Info_16x16.png
+-rw-r--r--   0        0        0     1229 2020-02-02 00:00:00.000000 nqrduck-0.0.9/src/nqrduck/assets/logos/LabMallardnbg_32x32.png
+-rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 nqrduck-0.0.9/src/nqrduck/assets/logos/Load_16x16.png
+-rw-r--r--   0        0        0     1019 2020-02-02 00:00:00.000000 nqrduck-0.0.9/src/nqrduck/assets/logos/Logo_64x32.png
+-rw-r--r--   0        0        0     2065 2020-02-02 00:00:00.000000 nqrduck-0.0.9/src/nqrduck/assets/logos/Logo_full.png
+-rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 nqrduck-0.0.9/src/nqrduck/assets/logos/New_16x16.png
+-rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 nqrduck-0.0.9/src/nqrduck/assets/logos/Pen_12x12.png
+-rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 nqrduck-0.0.9/src/nqrduck/assets/logos/Play_16x16.png
+-rw-r--r--   0        0        0      240 2020-02-02 00:00:00.000000 nqrduck-0.0.9/src/nqrduck/assets/logos/QuestionMark_16x16.png
+-rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 nqrduck-0.0.9/src/nqrduck/assets/logos/Save_16x16.png
+-rw-r--r--   0        0        0      249 2020-02-02 00:00:00.000000 nqrduck-0.0.9/src/nqrduck/assets/logos/Settings_16x16.png
+-rw-r--r--   0        0        0      418 2020-02-02 00:00:00.000000 nqrduck-0.0.9/src/nqrduck/assets/pulseparameters/GateOff.png
+-rw-r--r--   0        0        0      453 2020-02-02 00:00:00.000000 nqrduck-0.0.9/src/nqrduck/assets/pulseparameters/GateOn.png
+-rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 nqrduck-0.0.9/src/nqrduck/assets/pulseparameters/RXOff.png
+-rw-r--r--   0        0        0      354 2020-02-02 00:00:00.000000 nqrduck-0.0.9/src/nqrduck/assets/pulseparameters/RXOn.png
+-rw-r--r--   0        0        0      346 2020-02-02 00:00:00.000000 nqrduck-0.0.9/src/nqrduck/assets/pulseparameters/TXCustom.png
+-rw-r--r--   0        0        0      356 2020-02-02 00:00:00.000000 nqrduck-0.0.9/src/nqrduck/assets/pulseparameters/TXGauss.png
+-rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 nqrduck-0.0.9/src/nqrduck/assets/pulseparameters/TXOff.png
+-rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 nqrduck-0.0.9/src/nqrduck/assets/pulseparameters/TXRect.png
+-rw-r--r--   0        0        0      387 2020-02-02 00:00:00.000000 nqrduck-0.0.9/src/nqrduck/assets/pulseparameters/TXSinc.png
+-rw-r--r--   0        0        0     2609 2020-02-02 00:00:00.000000 nqrduck-0.0.9/src/nqrduck/contrib/mplwidget.py
+-rw-r--r--   0        0        0    15929 2020-02-02 00:00:00.000000 nqrduck-0.0.9/src/nqrduck/core/install_wizard.py
+-rw-r--r--   0        0        0     4587 2020-02-02 00:00:00.000000 nqrduck-0.0.9/src/nqrduck/core/main_controller.py
+-rw-r--r--   0        0        0     6948 2020-02-02 00:00:00.000000 nqrduck-0.0.9/src/nqrduck/core/main_model.py
+-rw-r--r--   0        0        0    31833 2020-02-02 00:00:00.000000 nqrduck-0.0.9/src/nqrduck/core/main_view.py
+-rw-r--r--   0        0        0     4706 2020-02-02 00:00:00.000000 nqrduck-0.0.9/src/nqrduck/core/main_window.py
+-rw-r--r--   0        0        0     1077 2020-02-02 00:00:00.000000 nqrduck-0.0.9/src/nqrduck/core/resources/logo.png
+-rw-r--r--   0        0        0     2919 2020-02-02 00:00:00.000000 nqrduck-0.0.9/src/nqrduck/core/resources/main_window.ui
+-rw-r--r--   0        0        0    28916 2020-02-02 00:00:00.000000 nqrduck-0.0.9/src/nqrduck/core/resources/font/AsepriteFont.ttf
+-rw-r--r--   0        0        0      329 2020-02-02 00:00:00.000000 nqrduck-0.0.9/src/nqrduck/core/resources/font/LICENCE
+-rw-r--r--   0        0        0     7172 2020-02-02 00:00:00.000000 nqrduck-0.0.9/src/nqrduck/helpers/duckwidgets.py
+-rw-r--r--   0        0        0    18853 2020-02-02 00:00:00.000000 nqrduck-0.0.9/src/nqrduck/helpers/formbuilder.py
+-rw-r--r--   0        0        0    12683 2020-02-02 00:00:00.000000 nqrduck-0.0.9/src/nqrduck/helpers/functions.py
+-rw-r--r--   0        0        0      741 2020-02-02 00:00:00.000000 nqrduck-0.0.9/src/nqrduck/helpers/serializer.py
+-rw-r--r--   0        0        0     3307 2020-02-02 00:00:00.000000 nqrduck-0.0.9/src/nqrduck/helpers/signalprocessing.py
+-rw-r--r--   0        0        0     1458 2020-02-02 00:00:00.000000 nqrduck-0.0.9/src/nqrduck/helpers/unitconverter.py
+-rw-r--r--   0        0        0     3669 2020-02-02 00:00:00.000000 nqrduck-0.0.9/src/nqrduck/helpers/validators.py
+-rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 nqrduck-0.0.9/src/nqrduck/module/__init__.py
+-rw-r--r--   0        0        0     2716 2020-02-02 00:00:00.000000 nqrduck-0.0.9/src/nqrduck/module/module.py
+-rw-r--r--   0        0        0      806 2020-02-02 00:00:00.000000 nqrduck-0.0.9/src/nqrduck/module/module_controller.py
+-rw-r--r--   0        0        0     2225 2020-02-02 00:00:00.000000 nqrduck-0.0.9/src/nqrduck/module/module_model.py
+-rw-r--r--   0        0        0     3437 2020-02-02 00:00:00.000000 nqrduck-0.0.9/src/nqrduck/module/module_view.py
+-rw-r--r--   0        0        0     1250 2020-02-02 00:00:00.000000 nqrduck-0.0.9/tests/test_load_module.py
+-rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 nqrduck-0.0.9/.gitignore
+-rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 nqrduck-0.0.9/LICENSE
+-rw-r--r--   0        0        0     2371 2020-02-02 00:00:00.000000 nqrduck-0.0.9/README.md
+-rw-r--r--   0        0        0     1860 2020-02-02 00:00:00.000000 nqrduck-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0     5456 2020-02-02 00:00:00.000000 nqrduck-0.0.9/PKG-INFO
```

### Comparing `nqrduck-0.0.8/.github/workflows/main.yml` & `nqrduck-0.0.9/.github/workflows/main.yml`

 * *Files identical despite different names*

### Comparing `nqrduck-0.0.8/.github/workflows/python-publish.yml` & `nqrduck-0.0.9/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `nqrduck-0.0.8/.github/workflows/ubuntu-python-package.yml` & `nqrduck-0.0.9/.github/workflows/ubuntu-python-package.yml`

 * *Files identical despite different names*

### Comparing `nqrduck-0.0.8/docs/img/ui_structure_v2.png` & `nqrduck-0.0.9/docs/img/ui_structure_v2.png`

 * *Files identical despite different names*

### Comparing `nqrduck-0.0.8/src/nqrduck/__main__.py` & `nqrduck-0.0.9/src/nqrduck/__main__.py`

 * *Files 5% similar despite different names*

```diff
@@ -31,20 +31,17 @@
         self._main_view = MainView(self._main_model, self._main_controller)
 
         # Wait for the splash screen to close before starting the rest of the application
         self.processEvents()
 
         # Here the modules are loaded and signals connected
         self._main_controller.load_modules(self._main_view)
-        # Get the first loaded module and set it as active
-        try:
-            self._main_model.active_module = self._main_model.loaded_modules[
-                list(self._main_model.loaded_modules.keys())[0]
-            ]
-        except IndexError:
+        
+        # Start the wizard if no modules could be loaded
+        if not self._main_model.loaded_modules:
             logger.warning("No modules loaded")
             # Start the install wizard if no modules are loaded
             self._main_view.install_wizard = DuckWizard(
                 [], self._main_view
             )
             self._main_view.install_wizard.show()
             self._main_view.install_wizard.exec()
```

### Comparing `nqrduck-0.0.8/src/nqrduck/assets/animations.py` & `nqrduck-0.0.9/src/nqrduck/assets/animations.py`

 * *Files identical despite different names*

### Comparing `nqrduck-0.0.8/src/nqrduck/assets/icons.py` & `nqrduck-0.0.9/src/nqrduck/assets/icons.py`

 * *Files identical despite different names*

### Comparing `nqrduck-0.0.8/src/nqrduck/assets/animations/DuckKick_128x128.gif` & `nqrduck-0.0.9/src/nqrduck/assets/animations/DuckKick_128x128.gif`

 * *Files identical despite different names*

### Comparing `nqrduck-0.0.8/src/nqrduck/assets/animations/DuckSleep_128x128.gif` & `nqrduck-0.0.9/src/nqrduck/assets/animations/DuckSleep_128x128.gif`

 * *Files identical despite different names*

### Comparing `nqrduck-0.0.8/src/nqrduck/assets/logos/LabMallardnbg_32x32.png` & `nqrduck-0.0.9/src/nqrduck/assets/logos/LabMallardnbg_32x32.png`

 * *Files identical despite different names*

### Comparing `nqrduck-0.0.8/src/nqrduck/assets/logos/Logo_64x32.png` & `nqrduck-0.0.9/src/nqrduck/assets/logos/Logo_64x32.png`

 * *Files identical despite different names*

### Comparing `nqrduck-0.0.8/src/nqrduck/assets/logos/Logo_full.png` & `nqrduck-0.0.9/src/nqrduck/assets/logos/Logo_full.png`

 * *Files identical despite different names*

### Comparing `nqrduck-0.0.8/src/nqrduck/contrib/mplwidget.py` & `nqrduck-0.0.9/src/nqrduck/contrib/mplwidget.py`

 * *Files identical despite different names*

### Comparing `nqrduck-0.0.8/src/nqrduck/core/install_wizard.py` & `nqrduck-0.0.9/src/nqrduck/core/install_wizard.py`

 * *Files identical despite different names*

### Comparing `nqrduck-0.0.8/src/nqrduck/core/main_controller.py` & `nqrduck-0.0.9/src/nqrduck/core/main_controller.py`

 * *Files identical despite different names*

### Comparing `nqrduck-0.0.8/src/nqrduck/core/main_model.py` & `nqrduck-0.0.9/src/nqrduck/core/main_model.py`

 * *Files identical despite different names*

### Comparing `nqrduck-0.0.8/src/nqrduck/core/main_view.py` & `nqrduck-0.0.9/src/nqrduck/core/main_view.py`

 * *Files 2% similar despite different names*

```diff
@@ -255,31 +255,38 @@
 
         # Copy toolbar actions
         toolboxes = self._toolbox.findChildren(QToolButton)
         self._toolbox.clear()
 
         logger.debug("Updating toolbar with new module order: %s", module_order)
 
+        # Thi is used to set the first module as the active module
+        first_module = True
         for module in module_order:
             for button in toolboxes:
                 if not button.text():
                     continue
                 try:
                     if (
                         button.text()
                         == self._main_model.loaded_modules[module].model.toolbar_name
                     ):
                         new_button = QToolButton()
                         new_button.setText(button.text())
                         # Get the slot of the button that is connected to the clicked event
                         new_button.clicked.connect(button.clicked)
                         self._toolbox.addWidget(new_button)
+                        if first_module:
+                            self._main_model.active_module = self._main_model.loaded_modules[module]
+                            first_module = False
                         break
+                   
                 except KeyError:
                     logger.info("Module %s not found in loaded modules", module)
+            
 
         # Rescale toolbar
         self._toolbox.adjustSize()
 
         self.update_mpl_parameters()
 
     def update_mpl_parameters(self) -> None:
```

### Comparing `nqrduck-0.0.8/src/nqrduck/core/main_window.py` & `nqrduck-0.0.9/src/nqrduck/core/main_window.py`

 * *Files identical despite different names*

### Comparing `nqrduck-0.0.8/src/nqrduck/core/resources/logo.png` & `nqrduck-0.0.9/src/nqrduck/core/resources/logo.png`

 * *Files identical despite different names*

### Comparing `nqrduck-0.0.8/src/nqrduck/core/resources/main_window.ui` & `nqrduck-0.0.9/src/nqrduck/core/resources/main_window.ui`

 * *Files identical despite different names*

### Comparing `nqrduck-0.0.8/src/nqrduck/core/resources/font/AsepriteFont.ttf` & `nqrduck-0.0.9/src/nqrduck/core/resources/font/AsepriteFont.ttf`

 * *Files identical despite different names*

### Comparing `nqrduck-0.0.8/src/nqrduck/helpers/duckwidgets.py` & `nqrduck-0.0.9/src/nqrduck/helpers/duckwidgets.py`

 * *Files identical despite different names*

### Comparing `nqrduck-0.0.8/src/nqrduck/helpers/formbuilder.py` & `nqrduck-0.0.9/src/nqrduck/helpers/formbuilder.py`

 * *Files identical despite different names*

### Comparing `nqrduck-0.0.8/src/nqrduck/helpers/functions.py` & `nqrduck-0.0.9/src/nqrduck/helpers/functions.py`

 * *Files identical despite different names*

### Comparing `nqrduck-0.0.8/src/nqrduck/helpers/serializer.py` & `nqrduck-0.0.9/src/nqrduck/helpers/serializer.py`

 * *Files identical despite different names*

### Comparing `nqrduck-0.0.8/src/nqrduck/helpers/signalprocessing.py` & `nqrduck-0.0.9/src/nqrduck/helpers/signalprocessing.py`

 * *Files identical despite different names*

### Comparing `nqrduck-0.0.8/src/nqrduck/helpers/unitconverter.py` & `nqrduck-0.0.9/src/nqrduck/helpers/unitconverter.py`

 * *Files identical despite different names*

### Comparing `nqrduck-0.0.8/src/nqrduck/helpers/validators.py` & `nqrduck-0.0.9/src/nqrduck/helpers/validators.py`

 * *Files identical despite different names*

### Comparing `nqrduck-0.0.8/src/nqrduck/module/module.py` & `nqrduck-0.0.9/src/nqrduck/module/module.py`

 * *Files identical despite different names*

### Comparing `nqrduck-0.0.8/src/nqrduck/module/module_controller.py` & `nqrduck-0.0.9/src/nqrduck/module/module_controller.py`

 * *Files identical despite different names*

### Comparing `nqrduck-0.0.8/src/nqrduck/module/module_model.py` & `nqrduck-0.0.9/src/nqrduck/module/module_model.py`

 * *Files identical despite different names*

### Comparing `nqrduck-0.0.8/src/nqrduck/module/module_view.py` & `nqrduck-0.0.9/src/nqrduck/module/module_view.py`

 * *Files 17% similar despite different names*

```diff
@@ -39,37 +39,40 @@
         """The module of the view."""
         return self._module
 
     @module.setter
     def module(self, value):
         self._module = value
 
-    class QFileManager:
+    class FileManager:
         """This class provides methods for opening and saving files.
 
         Args:
             extension (str): The extension of the files to open or save
             parent (QWidget): The parent widget of the file dialog
+            caption (str): The caption of the file dialog
         """
 
-        def __init__(self, extension, parent=None):
+        def __init__(self, extension, parent=None, caption = None):
             """Initializes the QFileManager."""
             self.extension = extension
             self.parent = parent
+            self.caption = caption
 
         def loadFileDialog(self) -> str:
             """Opens a file dialog for the user to select a file to open.
 
             Returns:
                 str: The path of the file selected by the user.
             """
             extension_name = self.extension.upper()
+            caption_string = f"{self.caption} - Open .{self.extension} " if self.caption else f"Open .{self.extension} File"
             fileName, _ = QFileDialog.getOpenFileName(
                 self.parent,
-                "QFileManager - Open File",
+                caption_string,
                 "",
                 f"{extension_name} Files (*.{self.extension});;All Files (*)",
                 options=QFileDialog.Option.DontUseNativeDialog,
             )
             if fileName:
                 return fileName
             else:
@@ -78,17 +81,18 @@
         def saveFileDialog(self) -> str:
             """Opens a file dialog for the user to select a file to save.
 
             Returns:
                 str: The path of the file selected by the user.
             """
             extension_name = self.extension.upper()
+            caption_string = f"{self.caption} - Save .{self.extension} " if self.caption else f"Save .{self.extension} File"
             fileName, _ = QFileDialog.getSaveFileName(
                 self.parent,
-                "QFileManager - Save File",
+                caption_string,
                 "",
                 f"{extension_name} Files (*.{self.extension});;All Files (*)",
                 options=QFileDialog.Option.DontUseNativeDialog,
             )
             if fileName:
                 # Append the .quack extension if not present
                 if not fileName.endswith(f".{self.extension}"):
```

### Comparing `nqrduck-0.0.8/tests/test_load_module.py` & `nqrduck-0.0.9/tests/test_load_module.py`

 * *Files identical despite different names*

### Comparing `nqrduck-0.0.8/LICENSE` & `nqrduck-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `nqrduck-0.0.8/README.md` & `nqrduck-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `nqrduck-0.0.8/pyproject.toml` & `nqrduck-0.0.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "hatchling.build"
 
 [tool.hatch.metadata]
 allow-direct-references = true
 
 [project]
 name = "nqrduck"
-version = "0.0.8"
+version = "0.0.9"
 authors = [
   { name="jupfi", email="support@nqrduck.cool" },
 ]
 
 description = "Simple Python script to interact with various python modules used for magnetic resonance spectroscopy."
 readme = "README.md"
 license = { file="LICENSE" }
```

### Comparing `nqrduck-0.0.8/PKG-INFO` & `nqrduck-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: nqrduck
-Version: 0.0.8
+Version: 0.0.9
 Summary: Simple Python script to interact with various python modules used for magnetic resonance spectroscopy.
 Project-URL: Homepage, https://nqrduck.cool
 Project-URL: Bug Tracker, https://github.com/nqrduck/nqrduck/issues
 Project-URL: Source Code, https://github.com/nqrduck/nqrduck
 Author-email: jupfi <support@nqrduck.cool>
 License: MIT License
```

