# Comparing `tmp/speechtoolkit-0.0.4.tar.gz` & `tmp/speechtoolkit-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "speechtoolkit-0.0.4.tar", last modified: Sat Apr 20 21:56:40 2024, max compression
+gzip compressed data, was "speechtoolkit-0.0.5.tar", last modified: Fri May 17 22:45:48 2024, max compression
```

## Comparing `speechtoolkit-0.0.4.tar` & `speechtoolkit-0.0.5.tar`

### file list

```diff
@@ -1,34 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 21:56:40.374679 speechtoolkit-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (127)     3057 2024-04-20 21:56:40.374679 speechtoolkit-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2018 2024-04-20 21:56:36.000000 speechtoolkit-0.0.4/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-20 21:56:40.374679 speechtoolkit-0.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1043 2024-04-20 21:56:36.000000 speechtoolkit-0.0.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 21:56:40.370679 speechtoolkit-0.0.4/speechtoolkit/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 21:56:36.000000 speechtoolkit-0.0.4/speechtoolkit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 21:56:40.370679 speechtoolkit-0.0.4/speechtoolkit/asr/
--rw-r--r--   0 runner    (1001) docker     (127)      122 2024-04-20 21:56:36.000000 speechtoolkit-0.0.4/speechtoolkit/asr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2644 2024-04-20 21:56:36.000000 speechtoolkit-0.0.4/speechtoolkit/asr/distilwhisper_lib.py
--rw-r--r--   0 runner    (1001) docker     (127)     1172 2024-04-20 21:56:36.000000 speechtoolkit-0.0.4/speechtoolkit/asr/whisper_lib.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 21:56:40.370679 speechtoolkit-0.0.4/speechtoolkit/classification/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 21:56:36.000000 speechtoolkit-0.0.4/speechtoolkit/classification/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2708 2024-04-20 21:56:36.000000 speechtoolkit-0.0.4/speechtoolkit/classification/accentclassifier.py
--rw-r--r--   0 runner    (1001) docker     (127)     1363 2024-04-20 21:56:36.000000 speechtoolkit-0.0.4/speechtoolkit/classification/languageclassification.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 21:56:40.370679 speechtoolkit-0.0.4/speechtoolkit/data/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 21:56:36.000000 speechtoolkit-0.0.4/speechtoolkit/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1016 2024-04-20 21:56:36.000000 speechtoolkit-0.0.4/speechtoolkit/data/languages.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 21:56:40.374679 speechtoolkit-0.0.4/speechtoolkit/tts/
--rw-r--r--   0 runner    (1001) docker     (127)       82 2024-04-20 21:56:36.000000 speechtoolkit-0.0.4/speechtoolkit/tts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3129 2024-04-20 21:56:36.000000 speechtoolkit-0.0.4/speechtoolkit/tts/styletts2_lib.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 21:56:40.374679 speechtoolkit-0.0.4/speechtoolkit/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 21:56:36.000000 speechtoolkit-0.0.4/speechtoolkit/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      212 2024-04-20 21:56:36.000000 speechtoolkit-0.0.4/speechtoolkit/utils/device.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 21:56:40.374679 speechtoolkit-0.0.4/speechtoolkit/vc/
--rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-20 21:56:36.000000 speechtoolkit-0.0.4/speechtoolkit/vc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1390 2024-04-20 21:56:36.000000 speechtoolkit-0.0.4/speechtoolkit/vc/lvc_lib.py
--rw-r--r--   0 runner    (1001) docker     (127)     1113 2024-04-20 21:56:36.000000 speechtoolkit-0.0.4/speechtoolkit/vc/ns3vc_lib.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 21:56:40.374679 speechtoolkit-0.0.4/speechtoolkit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3057 2024-04-20 21:56:40.000000 speechtoolkit-0.0.4/speechtoolkit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      752 2024-04-20 21:56:40.000000 speechtoolkit-0.0.4/speechtoolkit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-20 21:56:40.000000 speechtoolkit-0.0.4/speechtoolkit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      212 2024-04-20 21:56:40.000000 speechtoolkit-0.0.4/speechtoolkit.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-20 21:56:40.000000 speechtoolkit-0.0.4/speechtoolkit.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 22:45:48.644855 speechtoolkit-0.0.5/
+-rw-r--r--   0 runner    (1001) docker     (127)     3045 2024-05-17 22:45:48.644855 speechtoolkit-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2006 2024-05-17 22:45:44.000000 speechtoolkit-0.0.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-17 22:45:48.644855 speechtoolkit-0.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1043 2024-05-17 22:45:44.000000 speechtoolkit-0.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 22:45:48.640855 speechtoolkit-0.0.5/speechtoolkit/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 22:45:44.000000 speechtoolkit-0.0.5/speechtoolkit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 22:45:48.640855 speechtoolkit-0.0.5/speechtoolkit/asr/
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-05-17 22:45:44.000000 speechtoolkit-0.0.5/speechtoolkit/asr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2644 2024-05-17 22:45:44.000000 speechtoolkit-0.0.5/speechtoolkit/asr/distilwhisper_lib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1172 2024-05-17 22:45:44.000000 speechtoolkit-0.0.5/speechtoolkit/asr/whisper_lib.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 22:45:48.640855 speechtoolkit-0.0.5/speechtoolkit/classification/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 22:45:44.000000 speechtoolkit-0.0.5/speechtoolkit/classification/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1363 2024-05-17 22:45:44.000000 speechtoolkit-0.0.5/speechtoolkit/classification/languageclassification.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 22:45:48.640855 speechtoolkit-0.0.5/speechtoolkit/data/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 22:45:44.000000 speechtoolkit-0.0.5/speechtoolkit/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1016 2024-05-17 22:45:44.000000 speechtoolkit-0.0.5/speechtoolkit/data/languages.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 22:45:48.640855 speechtoolkit-0.0.5/speechtoolkit/tts/
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-05-17 22:45:44.000000 speechtoolkit-0.0.5/speechtoolkit/tts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3129 2024-05-17 22:45:44.000000 speechtoolkit-0.0.5/speechtoolkit/tts/styletts2_lib.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 22:45:48.640855 speechtoolkit-0.0.5/speechtoolkit/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 22:45:44.000000 speechtoolkit-0.0.5/speechtoolkit/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      212 2024-05-17 22:45:44.000000 speechtoolkit-0.0.5/speechtoolkit/utils/device.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 22:45:48.644855 speechtoolkit-0.0.5/speechtoolkit/vc/
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-05-17 22:45:44.000000 speechtoolkit-0.0.5/speechtoolkit/vc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1390 2024-05-17 22:45:44.000000 speechtoolkit-0.0.5/speechtoolkit/vc/lvc_lib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1113 2024-05-17 22:45:44.000000 speechtoolkit-0.0.5/speechtoolkit/vc/ns3vc_lib.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 22:45:48.644855 speechtoolkit-0.0.5/speechtoolkit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3045 2024-05-17 22:45:48.000000 speechtoolkit-0.0.5/speechtoolkit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      703 2024-05-17 22:45:48.000000 speechtoolkit-0.0.5/speechtoolkit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-17 22:45:48.000000 speechtoolkit-0.0.5/speechtoolkit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      212 2024-05-17 22:45:48.000000 speechtoolkit-0.0.5/speechtoolkit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-17 22:45:48.000000 speechtoolkit-0.0.5/speechtoolkit.egg-info/top_level.txt
```

### Comparing `speechtoolkit-0.0.4/PKG-INFO` & `speechtoolkit-0.0.5/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: speechtoolkit
-Version: 0.0.4
+Version: 0.0.5
 Summary: ML for Speech presents SpeechToolkit, a unified, all-in-one toolkit for TTS, ASR, VC, & other models.
 Home-page: https://github.com/ml-for-speech/speechtoolkit
 Author: ml-for-speech
 Description-Content-Type: text/markdown
 Requires-Dist: soundfile
 Requires-Dist: librosa
 Requires-Dist: transformers
@@ -40,26 +40,27 @@
 
 If you prefer not to use SpeechToolkit but would like to interact with models individually and separately, please check out the [ML for Speech](https://github.com/ml-for-speech) page.
 
 ## Implemented Features
 
 - [x] Text-to-speech
   - [x] StyleTTS 2
+  - [ ] MetaVoice
+  - [ ] Parler TTS
+  - [ ] XTTS
 - [x] Voice conversion
   - [x] LVC-VC
   - [x] NaturalSpeech3 Voice Conversion
   - [ ] StyleTTS2-VC
 - [x] Automatic speech recognition
   - [x] Whisper
   - [x] Distil-Whisper
   - [ ] Canary
 - [x] Audio classification
   - [x] Language detection
-  - [x] Accent detection
-  - [ ] Large accent detection model
 
 ## Installation & Usage
 
 Documentation is available [online](https://ml-for-speech.github.io/speechtoolkit).
 
 ## Disclaimer
```

### Comparing `speechtoolkit-0.0.4/README.md` & `speechtoolkit-0.0.5/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -8,26 +8,27 @@
 
 If you prefer not to use SpeechToolkit but would like to interact with models individually and separately, please check out the [ML for Speech](https://github.com/ml-for-speech) page.
 
 ## Implemented Features
 
 - [x] Text-to-speech
   - [x] StyleTTS 2
+  - [ ] MetaVoice
+  - [ ] Parler TTS
+  - [ ] XTTS
 - [x] Voice conversion
   - [x] LVC-VC
   - [x] NaturalSpeech3 Voice Conversion
   - [ ] StyleTTS2-VC
 - [x] Automatic speech recognition
   - [x] Whisper
   - [x] Distil-Whisper
   - [ ] Canary
 - [x] Audio classification
   - [x] Language detection
-  - [x] Accent detection
-  - [ ] Large accent detection model
 
 ## Installation & Usage
 
 Documentation is available [online](https://ml-for-speech.github.io/speechtoolkit).
 
 ## Disclaimer
```

### Comparing `speechtoolkit-0.0.4/setup.py` & `speechtoolkit-0.0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 
 extra_pkgs["all"] = final
 
 with open("README.md", "r") as f:
     longdesc = f.read()
 setup(
     name="speechtoolkit",
-    version="0.0.4",
+    version="0.0.5",
     author="ml-for-speech",
     description="ML for Speech presents SpeechToolkit, a unified, all-in-one toolkit for TTS, ASR, VC, & other models.",
     long_description=longdesc,
     long_description_content_type="text/markdown",
     url="https://github.com/ml-for-speech/speechtoolkit",
     packages=find_packages(),
     install_requires=[
```

### Comparing `speechtoolkit-0.0.4/speechtoolkit/asr/distilwhisper_lib.py` & `speechtoolkit-0.0.5/speechtoolkit/asr/distilwhisper_lib.py`

 * *Files identical despite different names*

### Comparing `speechtoolkit-0.0.4/speechtoolkit/asr/whisper_lib.py` & `speechtoolkit-0.0.5/speechtoolkit/asr/whisper_lib.py`

 * *Files identical despite different names*

### Comparing `speechtoolkit-0.0.4/speechtoolkit/classification/accentclassifier.py` & `speechtoolkit-0.0.5/speechtoolkit/classification/languageclassification.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,72 +1,27 @@
 from transformers import pipeline
 from speechtoolkit.data.languages import language_codes
 from speechtoolkit.utils.device import device_map
 
-class EdAccAccentClassifierModel:
-    """
-    Use a Whisper-based accent classification model trained on the EdAcc dataset. It currently only supports English.
-
-    **Args**
-
-    device (str): The device to use. Defaults to 'auto'
-    model (str): The model ID to use on the Hugging Face Hub.
-    **kwargs: Additional arguments to pass to package
-    """
-
-    def __init__(
-        self,
-        device="auto",
-        model="ml-for-speech/accent-classification",
-        **kwargs,
-    ):
-        """
-        Initialize model.
-
-        **Args**
-
-        device (str): The device to use. Defaults to 'auto'
-        model (str): The model ID to use on the Hugging Face Hub.
-        **kwargs: Additional arguments to pass to package
-        """
-        self.pipe = pipeline("audio-classification", model, device=device_map(device))
-
-    def infer_file(self, file_path):
-        """
-        Run inference on a single file.
-
-        **Args**
-
-        file_path (str): The path of the audio to classify.
-
-        **Returns**
-
-        str: The detected accent.
-        """
-        result = self.pipe(file_path)[0]["label"]
-        if result in language_codes.keys():
-            return language_codes[result]
-        else:
-            return result
 
-class XLAccentClassifierModel:
+class WhisperLanguageClassifierModel:
     """
-    Use a Whisper-based accent classification model that is generally higher-quality than the EdAccAccentClassifierModel but is slower and more resource-intensive. It currently only supports English.
+    Use a Whisper-based language classification model.
 
     **Args**
 
     device (str): The device to use. Defaults to 'auto'
     model (str): The model ID to use on the Hugging Face Hub.
     **kwargs: Additional arguments to pass to package
     """
 
     def __init__(
         self,
         device="auto",
-        model="ml-for-speech/accent-classification-xl",
+        model="ml-for-speech/language-classification",
         **kwargs,
     ):
         """
         Initialize model.
 
         **Args**
 
@@ -82,14 +37,14 @@
 
         **Args**
 
         file_path (str): The path of the audio to classify.
 
         **Returns**
 
-        str: The detected accent.
+        str: The language ISO language code of the detected language.
         """
         result = self.pipe(file_path)[0]["label"]
         if result in language_codes.keys():
             return language_codes[result]
         else:
             return result
```

### Comparing `speechtoolkit-0.0.4/speechtoolkit/data/languages.py` & `speechtoolkit-0.0.5/speechtoolkit/data/languages.py`

 * *Files identical despite different names*

### Comparing `speechtoolkit-0.0.4/speechtoolkit/tts/styletts2_lib.py` & `speechtoolkit-0.0.5/speechtoolkit/tts/styletts2_lib.py`

 * *Files identical despite different names*

### Comparing `speechtoolkit-0.0.4/speechtoolkit/vc/lvc_lib.py` & `speechtoolkit-0.0.5/speechtoolkit/vc/lvc_lib.py`

 * *Files identical despite different names*

### Comparing `speechtoolkit-0.0.4/speechtoolkit/vc/ns3vc_lib.py` & `speechtoolkit-0.0.5/speechtoolkit/vc/ns3vc_lib.py`

 * *Files identical despite different names*

### Comparing `speechtoolkit-0.0.4/speechtoolkit.egg-info/PKG-INFO` & `speechtoolkit-0.0.5/speechtoolkit.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: speechtoolkit
-Version: 0.0.4
+Version: 0.0.5
 Summary: ML for Speech presents SpeechToolkit, a unified, all-in-one toolkit for TTS, ASR, VC, & other models.
 Home-page: https://github.com/ml-for-speech/speechtoolkit
 Author: ml-for-speech
 Description-Content-Type: text/markdown
 Requires-Dist: soundfile
 Requires-Dist: librosa
 Requires-Dist: transformers
@@ -40,26 +40,27 @@
 
 If you prefer not to use SpeechToolkit but would like to interact with models individually and separately, please check out the [ML for Speech](https://github.com/ml-for-speech) page.
 
 ## Implemented Features
 
 - [x] Text-to-speech
   - [x] StyleTTS 2
+  - [ ] MetaVoice
+  - [ ] Parler TTS
+  - [ ] XTTS
 - [x] Voice conversion
   - [x] LVC-VC
   - [x] NaturalSpeech3 Voice Conversion
   - [ ] StyleTTS2-VC
 - [x] Automatic speech recognition
   - [x] Whisper
   - [x] Distil-Whisper
   - [ ] Canary
 - [x] Audio classification
   - [x] Language detection
-  - [x] Accent detection
-  - [ ] Large accent detection model
 
 ## Installation & Usage
 
 Documentation is available [online](https://ml-for-speech.github.io/speechtoolkit).
 
 ## Disclaimer
```

### Comparing `speechtoolkit-0.0.4/speechtoolkit.egg-info/SOURCES.txt` & `speechtoolkit-0.0.5/speechtoolkit.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 speechtoolkit.egg-info/dependency_links.txt
 speechtoolkit.egg-info/requires.txt
 speechtoolkit.egg-info/top_level.txt
 speechtoolkit/asr/__init__.py
 speechtoolkit/asr/distilwhisper_lib.py
 speechtoolkit/asr/whisper_lib.py
 speechtoolkit/classification/__init__.py
-speechtoolkit/classification/accentclassifier.py
 speechtoolkit/classification/languageclassification.py
 speechtoolkit/data/__init__.py
 speechtoolkit/data/languages.py
 speechtoolkit/tts/__init__.py
 speechtoolkit/tts/styletts2_lib.py
 speechtoolkit/utils/__init__.py
 speechtoolkit/utils/device.py
```

