# Comparing `tmp/elfobs-0.1.2.tar.gz` & `tmp/elfobs-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "elfobs-0.1.2.tar", max compression
+gzip compressed data, was "elfobs-0.1.3.tar", max compression
```

## Comparing `elfobs-0.1.2.tar` & `elfobs-0.1.3.tar`

### file list

```diff
@@ -1,23 +1,24 @@
--rw-r--r--   0        0        0       69 2023-10-10 14:06:36.675900 elfobs-0.1.2/README.md
--rw-r--r--   0        0        0     1093 2023-10-10 14:37:16.707905 elfobs-0.1.2/elfobs/__init__.py
--rw-r--r--   0        0        0      648 2023-10-10 14:38:16.783978 elfobs-0.1.2/elfobs/cli.py
--rw-r--r--   0        0        0     1096 2023-10-10 11:13:05.729485 elfobs-0.1.2/elfobs/display.py
--rw-r--r--   0        0        0   825872 2023-10-10 08:29:07.588211 elfobs-0.1.2/elfobs/fonts/NotoSerif-Black.ttf
--rw-r--r--   0        0        0   802780 2023-10-10 08:29:07.588211 elfobs-0.1.2/elfobs/fonts/NotoSerif-BlackItalic.ttf
--rw-r--r--   0        0        0   769364 2023-10-10 08:29:07.591545 elfobs-0.1.2/elfobs/fonts/NotoSerif-Bold.ttf
--rw-r--r--   0        0        0   777288 2023-10-10 08:29:07.591545 elfobs-0.1.2/elfobs/fonts/NotoSerif-BoldItalic.ttf
--rw-r--r--   0        0        0   752236 2023-10-10 08:29:07.591545 elfobs-0.1.2/elfobs/fonts/NotoSerif-Italic.ttf
--rw-r--r--   0        0        0   757916 2023-10-10 08:29:07.591545 elfobs-0.1.2/elfobs/fonts/NotoSerif-Light.ttf
--rw-r--r--   0        0        0   734840 2023-10-10 08:29:07.591545 elfobs-0.1.2/elfobs/fonts/NotoSerif-LightItalic.ttf
--rw-r--r--   0        0        0   767252 2023-10-10 08:29:07.591545 elfobs-0.1.2/elfobs/fonts/NotoSerif-Medium.ttf
--rw-r--r--   0        0        0   779240 2023-10-10 08:29:07.591545 elfobs-0.1.2/elfobs/fonts/NotoSerif-MediumItalic.ttf
--rw-r--r--   0        0        0   738828 2023-10-10 08:29:07.591545 elfobs-0.1.2/elfobs/fonts/NotoSerif-Regular.ttf
--rw-r--r--   0        0        0   788816 2023-10-10 08:29:07.594878 elfobs-0.1.2/elfobs/fonts/NotoSerif-Thin.ttf
--rw-r--r--   0        0        0   743868 2023-10-10 08:29:07.594878 elfobs-0.1.2/elfobs/fonts/NotoSerif-ThinItalic.ttf
--rw-r--r--   0        0        0        0 2023-10-10 08:43:18.855624 elfobs-0.1.2/elfobs/fonts/__init__.py
--rw-r--r--   0        0        0     1796 2023-10-10 11:13:35.449198 elfobs-0.1.2/elfobs/image.py
--rw-r--r--   0        0        0     1748 2023-10-12 05:16:29.792612 elfobs-0.1.2/elfobs/obs.py
--rw-r--r--   0        0        0     1122 2023-10-10 11:14:10.232195 elfobs-0.1.2/elfobs/sound.py
--rw-r--r--   0        0        0      683 2023-10-10 14:04:21.503892 elfobs-0.1.2/elfobs/video.py
--rw-r--r--   0        0        0      497 2023-10-12 15:18:59.957112 elfobs-0.1.2/pyproject.toml
--rw-r--r--   0        0        0      762 1970-01-01 00:00:00.000000 elfobs-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0       69 2023-10-10 14:06:36.675900 elfobs-0.1.3/README.md
+-rw-r--r--   0        0        0     1093 2023-10-10 14:37:16.707905 elfobs-0.1.3/elfobs/__init__.py
+-rw-r--r--   0        0        0      715 2024-05-17 22:07:22.103103 elfobs-0.1.3/elfobs/cli.py
+-rw-r--r--   0        0        0     1096 2023-10-10 11:13:05.729485 elfobs-0.1.3/elfobs/display.py
+-rw-r--r--   0        0        0   825872 2023-10-10 08:29:07.588211 elfobs-0.1.3/elfobs/fonts/NotoSerif-Black.ttf
+-rw-r--r--   0        0        0   802780 2023-10-10 08:29:07.588211 elfobs-0.1.3/elfobs/fonts/NotoSerif-BlackItalic.ttf
+-rw-r--r--   0        0        0   769364 2023-10-10 08:29:07.591545 elfobs-0.1.3/elfobs/fonts/NotoSerif-Bold.ttf
+-rw-r--r--   0        0        0   777288 2023-10-10 08:29:07.591545 elfobs-0.1.3/elfobs/fonts/NotoSerif-BoldItalic.ttf
+-rw-r--r--   0        0        0   752236 2023-10-10 08:29:07.591545 elfobs-0.1.3/elfobs/fonts/NotoSerif-Italic.ttf
+-rw-r--r--   0        0        0   757916 2023-10-10 08:29:07.591545 elfobs-0.1.3/elfobs/fonts/NotoSerif-Light.ttf
+-rw-r--r--   0        0        0   734840 2023-10-10 08:29:07.591545 elfobs-0.1.3/elfobs/fonts/NotoSerif-LightItalic.ttf
+-rw-r--r--   0        0        0   767252 2023-10-10 08:29:07.591545 elfobs-0.1.3/elfobs/fonts/NotoSerif-Medium.ttf
+-rw-r--r--   0        0        0   779240 2023-10-10 08:29:07.591545 elfobs-0.1.3/elfobs/fonts/NotoSerif-MediumItalic.ttf
+-rw-r--r--   0        0        0   738828 2023-10-10 08:29:07.591545 elfobs-0.1.3/elfobs/fonts/NotoSerif-Regular.ttf
+-rw-r--r--   0        0        0   788816 2023-10-10 08:29:07.594878 elfobs-0.1.3/elfobs/fonts/NotoSerif-Thin.ttf
+-rw-r--r--   0        0        0   743868 2023-10-10 08:29:07.594878 elfobs-0.1.3/elfobs/fonts/NotoSerif-ThinItalic.ttf
+-rw-r--r--   0        0        0        0 2023-10-10 08:43:18.855624 elfobs-0.1.3/elfobs/fonts/__init__.py
+-rw-r--r--   0        0        0     1796 2023-10-10 11:13:35.449198 elfobs-0.1.3/elfobs/image.py
+-rw-r--r--   0        0        0     1748 2024-05-17 22:10:54.757887 elfobs-0.1.3/elfobs/obs.py
+-rw-r--r--   0        0        0     2049 2024-05-17 23:48:53.265944 elfobs-0.1.3/elfobs/sched.py
+-rw-r--r--   0        0        0     1122 2023-10-10 11:14:10.232195 elfobs-0.1.3/elfobs/sound.py
+-rw-r--r--   0        0        0      683 2023-10-10 14:04:21.503892 elfobs-0.1.3/elfobs/video.py
+-rw-r--r--   0        0        0      545 2024-05-17 23:51:08.931410 elfobs-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0      857 1970-01-01 00:00:00.000000 elfobs-0.1.3/PKG-INFO
```

### Comparing `elfobs-0.1.2/elfobs/__init__.py` & `elfobs-0.1.3/elfobs/__init__.py`

 * *Files identical despite different names*

### Comparing `elfobs-0.1.2/elfobs/cli.py` & `elfobs-0.1.3/elfobs/cli.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 import typer
 
 from elfobs import OmegaConf, config, console
 from elfobs.display import app as display_app
 from elfobs.image import app as image_app
 from elfobs.obs import app as obs_app
+from elfobs.sched import app as sched_app
 from elfobs.sound import app as sound_app
 from elfobs.video import app as video_app
 
 app = typer.Typer()
 app.add_typer(image_app)
 app.add_typer(sound_app)
 app.add_typer(display_app)
 app.add_typer(video_app)
 app.add_typer(obs_app)
+app.add_typer(sched_app)
 
 
 @app.callback()
 def elfobs():
     """
     El Faro OBS
     """
```

### Comparing `elfobs-0.1.2/elfobs/display.py` & `elfobs-0.1.3/elfobs/display.py`

 * *Files identical despite different names*

### Comparing `elfobs-0.1.2/elfobs/fonts/NotoSerif-Black.ttf` & `elfobs-0.1.3/elfobs/fonts/NotoSerif-Black.ttf`

 * *Files identical despite different names*

### Comparing `elfobs-0.1.2/elfobs/fonts/NotoSerif-BlackItalic.ttf` & `elfobs-0.1.3/elfobs/fonts/NotoSerif-BlackItalic.ttf`

 * *Files identical despite different names*

### Comparing `elfobs-0.1.2/elfobs/fonts/NotoSerif-Bold.ttf` & `elfobs-0.1.3/elfobs/fonts/NotoSerif-Bold.ttf`

 * *Files identical despite different names*

### Comparing `elfobs-0.1.2/elfobs/fonts/NotoSerif-BoldItalic.ttf` & `elfobs-0.1.3/elfobs/fonts/NotoSerif-BoldItalic.ttf`

 * *Files identical despite different names*

### Comparing `elfobs-0.1.2/elfobs/fonts/NotoSerif-Italic.ttf` & `elfobs-0.1.3/elfobs/fonts/NotoSerif-Italic.ttf`

 * *Files identical despite different names*

### Comparing `elfobs-0.1.2/elfobs/fonts/NotoSerif-Light.ttf` & `elfobs-0.1.3/elfobs/fonts/NotoSerif-Light.ttf`

 * *Files identical despite different names*

### Comparing `elfobs-0.1.2/elfobs/fonts/NotoSerif-LightItalic.ttf` & `elfobs-0.1.3/elfobs/fonts/NotoSerif-LightItalic.ttf`

 * *Files identical despite different names*

### Comparing `elfobs-0.1.2/elfobs/fonts/NotoSerif-Medium.ttf` & `elfobs-0.1.3/elfobs/fonts/NotoSerif-Medium.ttf`

 * *Files identical despite different names*

### Comparing `elfobs-0.1.2/elfobs/fonts/NotoSerif-MediumItalic.ttf` & `elfobs-0.1.3/elfobs/fonts/NotoSerif-MediumItalic.ttf`

 * *Files identical despite different names*

### Comparing `elfobs-0.1.2/elfobs/fonts/NotoSerif-Regular.ttf` & `elfobs-0.1.3/elfobs/fonts/NotoSerif-Regular.ttf`

 * *Files identical despite different names*

### Comparing `elfobs-0.1.2/elfobs/fonts/NotoSerif-Thin.ttf` & `elfobs-0.1.3/elfobs/fonts/NotoSerif-Thin.ttf`

 * *Files identical despite different names*

### Comparing `elfobs-0.1.2/elfobs/fonts/NotoSerif-ThinItalic.ttf` & `elfobs-0.1.3/elfobs/fonts/NotoSerif-ThinItalic.ttf`

 * *Files identical despite different names*

### Comparing `elfobs-0.1.2/elfobs/image.py` & `elfobs-0.1.3/elfobs/image.py`

 * *Files identical despite different names*

### Comparing `elfobs-0.1.2/elfobs/obs.py` & `elfobs-0.1.3/elfobs/obs.py`

 * *Files identical despite different names*

### Comparing `elfobs-0.1.2/elfobs/sound.py` & `elfobs-0.1.3/elfobs/sound.py`

 * *Files identical despite different names*

### Comparing `elfobs-0.1.2/elfobs/video.py` & `elfobs-0.1.3/elfobs/video.py`

 * *Files identical despite different names*

### Comparing `elfobs-0.1.2/PKG-INFO` & `elfobs-0.1.3/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 Metadata-Version: 2.1
 Name: elfobs
-Version: 0.1.2
+Version: 0.1.3
 Summary: 
 Author: Aldo A. Villagra B.
 Author-email: aldovillagra@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: obsws-python (>=1.6.1,<2.0.0)
 Requires-Dist: omegaconf (>=2.3.0,<3.0.0)
+Requires-Dist: pandas[all] (>=2.2.2,<3.0.0)
 Requires-Dist: pendulum (>=2.1.2,<3.0.0)
 Requires-Dist: pillow (>=10.0.1,<11.0.0)
 Requires-Dist: pyalsaaudio (>=0.10.0,<0.11.0)
 Requires-Dist: typer[all] (>=0.9.0,<0.10.0)
 Requires-Dist: v4l2py (>=2.1.0,<3.0.0)
 Description-Content-Type: text/markdown
```

