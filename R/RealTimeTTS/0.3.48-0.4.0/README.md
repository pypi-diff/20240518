# Comparing `tmp/RealTimeTTS-0.3.48.tar.gz` & `tmp/RealTimeTTS-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "RealTimeTTS-0.3.48.tar", last modified: Thu May 16 22:17:50 2024, max compression
+gzip compressed data, was "RealTimeTTS-0.4.0.tar", last modified: Fri May 17 22:02:55 2024, max compression
```

## Comparing `RealTimeTTS-0.3.48.tar` & `RealTimeTTS-0.4.0.tar`

### file list

```diff
@@ -1,31 +1,32 @@
-drwxrwxrwx   0        0        0        0 2024-05-16 22:17:50.356256 RealTimeTTS-0.3.48/
--rw-rw-rw-   0        0        0    19978 2024-05-16 22:17:50.355255 RealTimeTTS-0.3.48/PKG-INFO
--rw-rw-rw-   0        0        0    18860 2024-05-16 20:10:20.000000 RealTimeTTS-0.3.48/README.md
-drwxrwxrwx   0        0        0        0 2024-05-16 22:17:50.354254 RealTimeTTS-0.3.48/RealTimeTTS.egg-info/
--rw-rw-rw-   0        0        0    19978 2024-05-16 22:17:50.000000 RealTimeTTS-0.3.48/RealTimeTTS.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      768 2024-05-16 22:17:50.000000 RealTimeTTS-0.3.48/RealTimeTTS.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-16 22:17:50.000000 RealTimeTTS-0.3.48/RealTimeTTS.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      181 2024-05-16 22:17:50.000000 RealTimeTTS-0.3.48/RealTimeTTS.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2024-05-16 22:17:50.000000 RealTimeTTS-0.3.48/RealTimeTTS.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-05-16 22:17:50.337239 RealTimeTTS-0.3.48/RealtimeTTS/
--rw-rw-rw-   0        0        0      422 2023-12-28 10:50:12.000000 RealTimeTTS-0.3.48/RealtimeTTS/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-16 22:17:50.351251 RealTimeTTS-0.3.48/RealtimeTTS/engines/
--rw-rw-rw-   0        0        0      397 2023-12-28 10:50:55.000000 RealTimeTTS-0.3.48/RealtimeTTS/engines/__init__.py
--rw-rw-rw-   0        0        0     9413 2024-05-16 19:46:11.000000 RealTimeTTS-0.3.48/RealtimeTTS/engines/azure_engine.py
--rw-rw-rw-   0        0        0     4490 2023-12-01 16:58:58.000000 RealTimeTTS-0.3.48/RealtimeTTS/engines/base_engine.py
--rw-rw-rw-   0        0        0   506471 2023-11-29 16:17:54.000000 RealTimeTTS-0.3.48/RealtimeTTS/engines/chinese.json
--rw-rw-rw-   0        0        0   506653 2023-12-07 22:51:46.000000 RealTimeTTS-0.3.48/RealtimeTTS/engines/coqui_default_voice.json
--rw-rw-rw-   0        0        0    38627 2024-05-16 19:46:15.000000 RealTimeTTS-0.3.48/RealtimeTTS/engines/coqui_engine.py
--rw-rw-rw-   0        0        0    10661 2024-05-16 20:09:01.000000 RealTimeTTS-0.3.48/RealtimeTTS/engines/elevenlabs_engine.py
--rw-rw-rw-   0        0        0   505425 2023-11-17 22:30:40.000000 RealTimeTTS-0.3.48/RealtimeTTS/engines/female.json
--rw-rw-rw-   0        0        0   506653 2023-12-07 22:51:46.000000 RealTimeTTS-0.3.48/RealtimeTTS/engines/male.json
--rw-rw-rw-   0        0        0     3477 2023-12-28 10:13:43.000000 RealTimeTTS-0.3.48/RealtimeTTS/engines/openai_engine.py
--rw-rw-rw-   0        0        0     4834 2024-05-16 19:46:19.000000 RealTimeTTS-0.3.48/RealtimeTTS/engines/system_engine.py
--rw-rw-rw-   0        0        0    10657 2024-05-06 13:40:39.000000 RealTimeTTS-0.3.48/RealtimeTTS/stream_player.py
--rw-rw-rw-   0        0        0    30141 2024-05-06 13:37:11.000000 RealTimeTTS-0.3.48/RealtimeTTS/text_to_stream.py
--rw-rw-rw-   0        0        0    10179 2023-11-29 16:17:54.000000 RealTimeTTS-0.3.48/RealtimeTTS/threadsafe_generators.py
--rw-rw-rw-   0        0        0       42 2024-05-16 22:17:50.356256 RealTimeTTS-0.3.48/setup.cfg
--rw-rw-rw-   0        0        0     1295 2024-05-16 22:17:42.000000 RealTimeTTS-0.3.48/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-16 22:17:50.353253 RealTimeTTS-0.3.48/tests/
--rw-rw-rw-   0        0        0     1361 2023-11-03 15:39:11.000000 RealTimeTTS-0.3.48/tests/test_callbacks.py
--rw-rw-rw-   0        0        0      637 2024-02-21 18:39:01.000000 RealTimeTTS-0.3.48/tests/test_on_audio_chunk_callback.py
+drwxrwxrwx   0        0        0        0 2024-05-17 22:02:55.864385 RealTimeTTS-0.4.0/
+-rw-rw-rw-   0        0        0    21039 2024-05-17 22:02:55.863385 RealTimeTTS-0.4.0/PKG-INFO
+-rw-rw-rw-   0        0        0    19894 2024-05-17 21:59:46.000000 RealTimeTTS-0.4.0/README.md
+drwxrwxrwx   0        0        0        0 2024-05-17 22:02:55.862384 RealTimeTTS-0.4.0/RealTimeTTS.egg-info/
+-rw-rw-rw-   0        0        0    21039 2024-05-17 22:02:55.000000 RealTimeTTS-0.4.0/RealTimeTTS.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      803 2024-05-17 22:02:55.000000 RealTimeTTS-0.4.0/RealTimeTTS.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-17 22:02:55.000000 RealTimeTTS-0.4.0/RealTimeTTS.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      193 2024-05-17 22:02:55.000000 RealTimeTTS-0.4.0/RealTimeTTS.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2024-05-17 22:02:55.000000 RealTimeTTS-0.4.0/RealTimeTTS.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-17 22:02:55.590479 RealTimeTTS-0.4.0/RealtimeTTS/
+-rw-rw-rw-   0        0        0      466 2024-05-17 21:40:58.000000 RealTimeTTS-0.4.0/RealtimeTTS/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-17 22:02:55.812388 RealTimeTTS-0.4.0/RealtimeTTS/engines/
+-rw-rw-rw-   0        0        0      459 2024-05-17 21:41:03.000000 RealTimeTTS-0.4.0/RealtimeTTS/engines/__init__.py
+-rw-rw-rw-   0        0        0     9413 2024-05-16 19:46:11.000000 RealTimeTTS-0.4.0/RealtimeTTS/engines/azure_engine.py
+-rw-rw-rw-   0        0        0     4490 2023-12-01 16:58:58.000000 RealTimeTTS-0.4.0/RealtimeTTS/engines/base_engine.py
+-rw-rw-rw-   0        0        0   506471 2023-11-29 16:17:54.000000 RealTimeTTS-0.4.0/RealtimeTTS/engines/chinese.json
+-rw-rw-rw-   0        0        0   506653 2023-12-07 22:51:46.000000 RealTimeTTS-0.4.0/RealtimeTTS/engines/coqui_default_voice.json
+-rw-rw-rw-   0        0        0    38627 2024-05-16 19:46:15.000000 RealTimeTTS-0.4.0/RealtimeTTS/engines/coqui_engine.py
+-rw-rw-rw-   0        0        0    10661 2024-05-16 20:09:01.000000 RealTimeTTS-0.4.0/RealtimeTTS/engines/elevenlabs_engine.py
+-rw-rw-rw-   0        0        0   505425 2023-11-17 22:30:40.000000 RealTimeTTS-0.4.0/RealtimeTTS/engines/female.json
+-rw-rw-rw-   0        0        0     3878 2024-05-17 22:00:29.000000 RealTimeTTS-0.4.0/RealtimeTTS/engines/gtts_engine.py
+-rw-rw-rw-   0        0        0   506653 2023-12-07 22:51:46.000000 RealTimeTTS-0.4.0/RealtimeTTS/engines/male.json
+-rw-rw-rw-   0        0        0     3477 2023-12-28 10:13:43.000000 RealTimeTTS-0.4.0/RealtimeTTS/engines/openai_engine.py
+-rw-rw-rw-   0        0        0     4834 2024-05-17 20:58:34.000000 RealTimeTTS-0.4.0/RealtimeTTS/engines/system_engine.py
+-rw-rw-rw-   0        0        0    10657 2024-05-06 13:40:39.000000 RealTimeTTS-0.4.0/RealtimeTTS/stream_player.py
+-rw-rw-rw-   0        0        0    30141 2024-05-06 13:37:11.000000 RealTimeTTS-0.4.0/RealtimeTTS/text_to_stream.py
+-rw-rw-rw-   0        0        0    10179 2023-11-29 16:17:54.000000 RealTimeTTS-0.4.0/RealtimeTTS/threadsafe_generators.py
+-rw-rw-rw-   0        0        0       42 2024-05-17 22:02:55.864385 RealTimeTTS-0.4.0/setup.cfg
+-rw-rw-rw-   0        0        0     1294 2024-05-17 21:59:14.000000 RealTimeTTS-0.4.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-17 22:02:55.860382 RealTimeTTS-0.4.0/tests/
+-rw-rw-rw-   0        0        0     1361 2023-11-03 15:39:11.000000 RealTimeTTS-0.4.0/tests/test_callbacks.py
+-rw-rw-rw-   0        0        0      637 2024-02-21 18:39:01.000000 RealTimeTTS-0.4.0/tests/test_on_audio_chunk_callback.py
```

### Comparing `RealTimeTTS-0.3.48/PKG-INFO` & `RealTimeTTS-0.4.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: RealTimeTTS
-Version: 0.3.48
+Version: 0.4.0
 Summary: *Stream text into audio with an easy-to-use, highly configurable library delivering voice output with minimal latency.
 Home-page: https://github.com/KoljaB/RealTimeTTS
 Author: Kolja Beigel
 Author-email: kolja.beigel@web.de
 Keywords: real-time,text-to-speech,TTS,streaming,audio,voice,synthesis,sentence-segmentation,low-latency,character-streaming,dynamic feedback,audio-output,text-input,TTS-engine,audio-playback,stream-player,sentence-fragment,audio-feedback,interactive,python
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -17,14 +17,15 @@
 Requires-Dist: stream2sentence==0.2.3
 Requires-Dist: azure-cognitiveservices-speech==1.36.0
 Requires-Dist: elevenlabs==1.2.2
 Requires-Dist: TTS==0.22.0
 Requires-Dist: tqdm==4.66.2
 Requires-Dist: pydub==0.25.1
 Requires-Dist: openai==1.13.3
+Requires-Dist: gtts==2.5.1
 
 # RealtimeTTS
 
 *Easy to use, low-latency text-to-speech library for realtime applications*
 
 ## About the Project
 
@@ -38,41 +39,42 @@
 
 - **Low Latency**
   - almost instantaneous text-to-speech conversion
   - compatible with LLM outputs
 - **High-Quality Audio**
   - generates clear and natural-sounding speech
 - **Multiple TTS Engine Support**
-  - supports OpenAI TTS, Elevenlabs, Azure Speech Services, Coqui TTS and System TTS
+  - supports OpenAI TTS, Elevenlabs, Azure Speech Services, Coqui TTS, gTTS and System TTS
 - **Multilingual**
 - **Robust and Reliable**: 
   - ensures continuous operation with a fallback mechanism
   - switches to alternative engines in case of disruptions guaranteeing consistent performance and reliability, which is vital for critical and professional use cases
 
 > **Hint**: *check out [RealtimeSTT](https://github.com/KoljaB/RealtimeSTT), the input counterpart of this library, for speech-to-text capabilities. Together, they form a powerful realtime audio wrapper around large language models.*
 
 ## FAQ
 
 Check the [FAQ page](./FAQ.md) for answers to a lot of questions around the usage of RealtimeTTS.
 
 ## Updates
 
-Latest Version: v0.3.47 (switched to new elevenlabs api)
+Latest Version: v0.4.0 (added GTTS engine)
 
 See [release history](https://github.com/KoljaB/RealtimeTTS/releases).
 
 ## Tech Stack
 
 This library uses:
 
 - **Text-to-Speech Engines**
   - **OpenAIEngine**: OpenAI's TTS system offers 6 natural sounding voices.
   - **CoquiEngine**: High quality local neural TTS.
   - **AzureEngine**: Microsoft's leading TTS technology. 500000 chars free per month.
   - **ElevenlabsEngine**: Offer the best sounding voices available.
+  - **GTTSEngine**: Free to use and doesn't require setting up a local GPU.
   - **SystemEngine**: Native engine for quick setup.
 
 - **Sentence Boundary Detection**
   - **NLTK Sentence Tokenizer**: Uses the Natural Language Toolkit's sentence tokenizer for precise and efficient sentence segmentation.
 
 *By using "industry standard" components RealtimeTTS offers a reliable, high-end technological foundation for developing advanced voice solutions.*
 
@@ -89,26 +91,29 @@
 Installation into virtual environment with GPU support:
 
 ```bash
 python -m venv env_realtimetts
 env_realtimetts\Scripts\activate.bat
 python.exe -m pip install --upgrade pip
 pip install RealtimeTTS
-pip install torch==2.2.1+cu118 torchaudio==2.2.1 --index-url https://download.pytorch.org/whl/cu118
+pip install torch==2.3.0+cu118 torchaudio==2.3.0 --index-url https://download.pytorch.org/whl/cu118
 ```
 
 More information about [CUDA installation](#cuda-installation).
 
 ## Engine Requirements
 
 Different engines supported by RealtimeTTS have unique requirements. Ensure you fulfill these requirements based on the engine you choose.
 
 ### SystemEngine
 The `SystemEngine` works out of the box using your system's built-in TTS capabilities. No additional setup is needed.
 
+### GTTSEngine
+The `GTTSEngine` works out of the box using Google Translate's text-to-speech API. No additional setup is needed.
+
 ### OpenAIEingine
 To use the `OpenAIEngine`:
 - set environment variable OPENAI_API_KEY
 - install ffmpeg (see [CUDA installation](#cuda-installation) point 3)
 
 ### AzureEngine
 To use the `AzureEngine`, you will need:
@@ -261,25 +266,35 @@
 
 ## Requirements Explained
 
 - **Python Version**: 
   - **Required**: Python >= 3.9, < 3.12
   - **Reason**: The library depends on the GitHub library "TTS" from coqui, which requires Python versions in this range.
 
-- **requests (>=2.31.0)**: to send HTTP requests for API calls and voice list retrieval
+- **requests**: to send HTTP requests for API calls and voice list retrieval
   
-- **PyAudio (>=0.2.13)**: to create an output audio stream
+- **PyAudio**: to create an output audio stream
   
-- **stream2sentence (>=0.1.1)**: to split the incoming text stream into sentences 
+- **stream2sentence**: to split the incoming text stream into sentences 
+
+- **pyttsx3**: System text-to-speech conversion engine
 
-- **pyttsx3 (>=2.90)**: System text-to-speech conversion engine
+- **tqdm (>=4.66.2)**: to display progress bars in the command line
 
-- **azure-cognitiveservices-speech (>=1.31.0)**: Azure text-to-speech conversion engine
+- **pydub (>=0.25.1)**: to convert audio chunk formats
+
+- **azure-cognitiveservices-speech**: Azure text-to-speech conversion engine
   
-- **elevenlabs (>=0.2.24)**: Elevenlabs text-to-speech conversion engine
+- **elevenlabs**: Elevenlabs text-to-speech conversion engine
+
+- **TTS**: Coqui's XTTS text-to-speech library for high-quality local neural TTS
+
+- **openai**: to interact with OpenAI's TTS API
+
+- **gtts (>=2.5.1)**: Google translate text-to-speech conversion
 
 
 ## Configuration
 
 ### Initialization Parameters for `TextToAudioStream`
 
 When you initialize the `TextToAudioStream` class, you have various options to customize its behavior. Here are the available parameters:
@@ -462,15 +477,17 @@
     pip install networkx==2.8.8
     pip install numpy==1.24.3
     pip install requests==2.31.0
     ```
 
 ## 💖 Acknowledgements
 
-Huge shoutout to the team behind [Coqui AI](https://coqui.ai/) being the first giving us local high quality synthesis with realtime speed and even a clonable voice!
+Huge shoutout to the team behind [Coqui AI](https://coqui.ai/) - especially the brillant [Eren Gölge](https://github.com/erogol) - for being the first giving us local high quality synthesis with realtime speed and even a clonable voice!
+
+Thank you [Pierre Nicolas Durette](https://github.com/pndurette) for giving us a free tts to use without GPU using Google Translate with his gtts python library.
 
 ## Contribution
 
 Contributions are always welcome (e.g. PR to add a new engine).
 
 ## License Information
 
@@ -495,14 +512,19 @@
 - **Details**: [AzureEngine License](https://learn.microsoft.com/en-us/answers/questions/1192398/can-i-use-azure-text-to-speech-for-commercial-usag)
 
 #### SystemEngine
 - **License**: Mozilla Public License 2.0 and GNU Lesser General Public License (LGPL) version 3.0.
 - **Commercial Use**: Allowed under this license.
 - **Details**: [SystemEngine License](https://github.com/nateshmbhat/pyttsx3/blob/master/LICENSE)
 
+#### GTTSEngine
+- **License**: MIT license
+- **Commercial Use**: It's under the MIT license, so it should be possible in theory. Since it utilizes undocumented Google Translate speech functionality, some caution might be necessary.
+- **Details**: [GTTS MIT License](https://github.com/pndurette/gTTS/blob/main/LICENSE)
+
 #### OpenAIEngine
 - **License**: please read [OpenAI Terms of Use](https://openai.com/policies/terms-of-use)
 
 **Disclaimer**: This is a summarization of the licenses as understood at the time of writing. It is not legal advice. Please read and respect the licenses of the different engine providers yourself if you plan to use them in a project.
 
 ## Author
```

### Comparing `RealTimeTTS-0.3.48/README.md` & `RealTimeTTS-0.4.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -14,41 +14,42 @@
 
 - **Low Latency**
   - almost instantaneous text-to-speech conversion
   - compatible with LLM outputs
 - **High-Quality Audio**
   - generates clear and natural-sounding speech
 - **Multiple TTS Engine Support**
-  - supports OpenAI TTS, Elevenlabs, Azure Speech Services, Coqui TTS and System TTS
+  - supports OpenAI TTS, Elevenlabs, Azure Speech Services, Coqui TTS, gTTS and System TTS
 - **Multilingual**
 - **Robust and Reliable**: 
   - ensures continuous operation with a fallback mechanism
   - switches to alternative engines in case of disruptions guaranteeing consistent performance and reliability, which is vital for critical and professional use cases
 
 > **Hint**: *check out [RealtimeSTT](https://github.com/KoljaB/RealtimeSTT), the input counterpart of this library, for speech-to-text capabilities. Together, they form a powerful realtime audio wrapper around large language models.*
 
 ## FAQ
 
 Check the [FAQ page](./FAQ.md) for answers to a lot of questions around the usage of RealtimeTTS.
 
 ## Updates
 
-Latest Version: v0.3.47 (switched to new elevenlabs api)
+Latest Version: v0.4.0 (added GTTS engine)
 
 See [release history](https://github.com/KoljaB/RealtimeTTS/releases).
 
 ## Tech Stack
 
 This library uses:
 
 - **Text-to-Speech Engines**
   - **OpenAIEngine**: OpenAI's TTS system offers 6 natural sounding voices.
   - **CoquiEngine**: High quality local neural TTS.
   - **AzureEngine**: Microsoft's leading TTS technology. 500000 chars free per month.
   - **ElevenlabsEngine**: Offer the best sounding voices available.
+  - **GTTSEngine**: Free to use and doesn't require setting up a local GPU.
   - **SystemEngine**: Native engine for quick setup.
 
 - **Sentence Boundary Detection**
   - **NLTK Sentence Tokenizer**: Uses the Natural Language Toolkit's sentence tokenizer for precise and efficient sentence segmentation.
 
 *By using "industry standard" components RealtimeTTS offers a reliable, high-end technological foundation for developing advanced voice solutions.*
 
@@ -65,26 +66,29 @@
 Installation into virtual environment with GPU support:
 
 ```bash
 python -m venv env_realtimetts
 env_realtimetts\Scripts\activate.bat
 python.exe -m pip install --upgrade pip
 pip install RealtimeTTS
-pip install torch==2.2.1+cu118 torchaudio==2.2.1 --index-url https://download.pytorch.org/whl/cu118
+pip install torch==2.3.0+cu118 torchaudio==2.3.0 --index-url https://download.pytorch.org/whl/cu118
 ```
 
 More information about [CUDA installation](#cuda-installation).
 
 ## Engine Requirements
 
 Different engines supported by RealtimeTTS have unique requirements. Ensure you fulfill these requirements based on the engine you choose.
 
 ### SystemEngine
 The `SystemEngine` works out of the box using your system's built-in TTS capabilities. No additional setup is needed.
 
+### GTTSEngine
+The `GTTSEngine` works out of the box using Google Translate's text-to-speech API. No additional setup is needed.
+
 ### OpenAIEingine
 To use the `OpenAIEngine`:
 - set environment variable OPENAI_API_KEY
 - install ffmpeg (see [CUDA installation](#cuda-installation) point 3)
 
 ### AzureEngine
 To use the `AzureEngine`, you will need:
@@ -237,25 +241,35 @@
 
 ## Requirements Explained
 
 - **Python Version**: 
   - **Required**: Python >= 3.9, < 3.12
   - **Reason**: The library depends on the GitHub library "TTS" from coqui, which requires Python versions in this range.
 
-- **requests (>=2.31.0)**: to send HTTP requests for API calls and voice list retrieval
+- **requests**: to send HTTP requests for API calls and voice list retrieval
   
-- **PyAudio (>=0.2.13)**: to create an output audio stream
+- **PyAudio**: to create an output audio stream
   
-- **stream2sentence (>=0.1.1)**: to split the incoming text stream into sentences 
+- **stream2sentence**: to split the incoming text stream into sentences 
+
+- **pyttsx3**: System text-to-speech conversion engine
 
-- **pyttsx3 (>=2.90)**: System text-to-speech conversion engine
+- **tqdm (>=4.66.2)**: to display progress bars in the command line
 
-- **azure-cognitiveservices-speech (>=1.31.0)**: Azure text-to-speech conversion engine
+- **pydub (>=0.25.1)**: to convert audio chunk formats
+
+- **azure-cognitiveservices-speech**: Azure text-to-speech conversion engine
   
-- **elevenlabs (>=0.2.24)**: Elevenlabs text-to-speech conversion engine
+- **elevenlabs**: Elevenlabs text-to-speech conversion engine
+
+- **TTS**: Coqui's XTTS text-to-speech library for high-quality local neural TTS
+
+- **openai**: to interact with OpenAI's TTS API
+
+- **gtts (>=2.5.1)**: Google translate text-to-speech conversion
 
 
 ## Configuration
 
 ### Initialization Parameters for `TextToAudioStream`
 
 When you initialize the `TextToAudioStream` class, you have various options to customize its behavior. Here are the available parameters:
@@ -438,15 +452,17 @@
     pip install networkx==2.8.8
     pip install numpy==1.24.3
     pip install requests==2.31.0
     ```
 
 ## 💖 Acknowledgements
 
-Huge shoutout to the team behind [Coqui AI](https://coqui.ai/) being the first giving us local high quality synthesis with realtime speed and even a clonable voice!
+Huge shoutout to the team behind [Coqui AI](https://coqui.ai/) - especially the brillant [Eren Gölge](https://github.com/erogol) - for being the first giving us local high quality synthesis with realtime speed and even a clonable voice!
+
+Thank you [Pierre Nicolas Durette](https://github.com/pndurette) for giving us a free tts to use without GPU using Google Translate with his gtts python library.
 
 ## Contribution
 
 Contributions are always welcome (e.g. PR to add a new engine).
 
 ## License Information
 
@@ -471,14 +487,19 @@
 - **Details**: [AzureEngine License](https://learn.microsoft.com/en-us/answers/questions/1192398/can-i-use-azure-text-to-speech-for-commercial-usag)
 
 #### SystemEngine
 - **License**: Mozilla Public License 2.0 and GNU Lesser General Public License (LGPL) version 3.0.
 - **Commercial Use**: Allowed under this license.
 - **Details**: [SystemEngine License](https://github.com/nateshmbhat/pyttsx3/blob/master/LICENSE)
 
+#### GTTSEngine
+- **License**: MIT license
+- **Commercial Use**: It's under the MIT license, so it should be possible in theory. Since it utilizes undocumented Google Translate speech functionality, some caution might be necessary.
+- **Details**: [GTTS MIT License](https://github.com/pndurette/gTTS/blob/main/LICENSE)
+
 #### OpenAIEngine
 - **License**: please read [OpenAI Terms of Use](https://openai.com/policies/terms-of-use)
 
 **Disclaimer**: This is a summarization of the licenses as understood at the time of writing. It is not legal advice. Please read and respect the licenses of the different engine providers yourself if you plan to use them in a project.
 
 ## Author
```

### Comparing `RealTimeTTS-0.3.48/RealTimeTTS.egg-info/PKG-INFO` & `RealTimeTTS-0.4.0/RealTimeTTS.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: RealTimeTTS
-Version: 0.3.48
+Version: 0.4.0
 Summary: *Stream text into audio with an easy-to-use, highly configurable library delivering voice output with minimal latency.
 Home-page: https://github.com/KoljaB/RealTimeTTS
 Author: Kolja Beigel
 Author-email: kolja.beigel@web.de
 Keywords: real-time,text-to-speech,TTS,streaming,audio,voice,synthesis,sentence-segmentation,low-latency,character-streaming,dynamic feedback,audio-output,text-input,TTS-engine,audio-playback,stream-player,sentence-fragment,audio-feedback,interactive,python
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -17,14 +17,15 @@
 Requires-Dist: stream2sentence==0.2.3
 Requires-Dist: azure-cognitiveservices-speech==1.36.0
 Requires-Dist: elevenlabs==1.2.2
 Requires-Dist: TTS==0.22.0
 Requires-Dist: tqdm==4.66.2
 Requires-Dist: pydub==0.25.1
 Requires-Dist: openai==1.13.3
+Requires-Dist: gtts==2.5.1
 
 # RealtimeTTS
 
 *Easy to use, low-latency text-to-speech library for realtime applications*
 
 ## About the Project
 
@@ -38,41 +39,42 @@
 
 - **Low Latency**
   - almost instantaneous text-to-speech conversion
   - compatible with LLM outputs
 - **High-Quality Audio**
   - generates clear and natural-sounding speech
 - **Multiple TTS Engine Support**
-  - supports OpenAI TTS, Elevenlabs, Azure Speech Services, Coqui TTS and System TTS
+  - supports OpenAI TTS, Elevenlabs, Azure Speech Services, Coqui TTS, gTTS and System TTS
 - **Multilingual**
 - **Robust and Reliable**: 
   - ensures continuous operation with a fallback mechanism
   - switches to alternative engines in case of disruptions guaranteeing consistent performance and reliability, which is vital for critical and professional use cases
 
 > **Hint**: *check out [RealtimeSTT](https://github.com/KoljaB/RealtimeSTT), the input counterpart of this library, for speech-to-text capabilities. Together, they form a powerful realtime audio wrapper around large language models.*
 
 ## FAQ
 
 Check the [FAQ page](./FAQ.md) for answers to a lot of questions around the usage of RealtimeTTS.
 
 ## Updates
 
-Latest Version: v0.3.47 (switched to new elevenlabs api)
+Latest Version: v0.4.0 (added GTTS engine)
 
 See [release history](https://github.com/KoljaB/RealtimeTTS/releases).
 
 ## Tech Stack
 
 This library uses:
 
 - **Text-to-Speech Engines**
   - **OpenAIEngine**: OpenAI's TTS system offers 6 natural sounding voices.
   - **CoquiEngine**: High quality local neural TTS.
   - **AzureEngine**: Microsoft's leading TTS technology. 500000 chars free per month.
   - **ElevenlabsEngine**: Offer the best sounding voices available.
+  - **GTTSEngine**: Free to use and doesn't require setting up a local GPU.
   - **SystemEngine**: Native engine for quick setup.
 
 - **Sentence Boundary Detection**
   - **NLTK Sentence Tokenizer**: Uses the Natural Language Toolkit's sentence tokenizer for precise and efficient sentence segmentation.
 
 *By using "industry standard" components RealtimeTTS offers a reliable, high-end technological foundation for developing advanced voice solutions.*
 
@@ -89,26 +91,29 @@
 Installation into virtual environment with GPU support:
 
 ```bash
 python -m venv env_realtimetts
 env_realtimetts\Scripts\activate.bat
 python.exe -m pip install --upgrade pip
 pip install RealtimeTTS
-pip install torch==2.2.1+cu118 torchaudio==2.2.1 --index-url https://download.pytorch.org/whl/cu118
+pip install torch==2.3.0+cu118 torchaudio==2.3.0 --index-url https://download.pytorch.org/whl/cu118
 ```
 
 More information about [CUDA installation](#cuda-installation).
 
 ## Engine Requirements
 
 Different engines supported by RealtimeTTS have unique requirements. Ensure you fulfill these requirements based on the engine you choose.
 
 ### SystemEngine
 The `SystemEngine` works out of the box using your system's built-in TTS capabilities. No additional setup is needed.
 
+### GTTSEngine
+The `GTTSEngine` works out of the box using Google Translate's text-to-speech API. No additional setup is needed.
+
 ### OpenAIEingine
 To use the `OpenAIEngine`:
 - set environment variable OPENAI_API_KEY
 - install ffmpeg (see [CUDA installation](#cuda-installation) point 3)
 
 ### AzureEngine
 To use the `AzureEngine`, you will need:
@@ -261,25 +266,35 @@
 
 ## Requirements Explained
 
 - **Python Version**: 
   - **Required**: Python >= 3.9, < 3.12
   - **Reason**: The library depends on the GitHub library "TTS" from coqui, which requires Python versions in this range.
 
-- **requests (>=2.31.0)**: to send HTTP requests for API calls and voice list retrieval
+- **requests**: to send HTTP requests for API calls and voice list retrieval
   
-- **PyAudio (>=0.2.13)**: to create an output audio stream
+- **PyAudio**: to create an output audio stream
   
-- **stream2sentence (>=0.1.1)**: to split the incoming text stream into sentences 
+- **stream2sentence**: to split the incoming text stream into sentences 
+
+- **pyttsx3**: System text-to-speech conversion engine
 
-- **pyttsx3 (>=2.90)**: System text-to-speech conversion engine
+- **tqdm (>=4.66.2)**: to display progress bars in the command line
 
-- **azure-cognitiveservices-speech (>=1.31.0)**: Azure text-to-speech conversion engine
+- **pydub (>=0.25.1)**: to convert audio chunk formats
+
+- **azure-cognitiveservices-speech**: Azure text-to-speech conversion engine
   
-- **elevenlabs (>=0.2.24)**: Elevenlabs text-to-speech conversion engine
+- **elevenlabs**: Elevenlabs text-to-speech conversion engine
+
+- **TTS**: Coqui's XTTS text-to-speech library for high-quality local neural TTS
+
+- **openai**: to interact with OpenAI's TTS API
+
+- **gtts (>=2.5.1)**: Google translate text-to-speech conversion
 
 
 ## Configuration
 
 ### Initialization Parameters for `TextToAudioStream`
 
 When you initialize the `TextToAudioStream` class, you have various options to customize its behavior. Here are the available parameters:
@@ -462,15 +477,17 @@
     pip install networkx==2.8.8
     pip install numpy==1.24.3
     pip install requests==2.31.0
     ```
 
 ## 💖 Acknowledgements
 
-Huge shoutout to the team behind [Coqui AI](https://coqui.ai/) being the first giving us local high quality synthesis with realtime speed and even a clonable voice!
+Huge shoutout to the team behind [Coqui AI](https://coqui.ai/) - especially the brillant [Eren Gölge](https://github.com/erogol) - for being the first giving us local high quality synthesis with realtime speed and even a clonable voice!
+
+Thank you [Pierre Nicolas Durette](https://github.com/pndurette) for giving us a free tts to use without GPU using Google Translate with his gtts python library.
 
 ## Contribution
 
 Contributions are always welcome (e.g. PR to add a new engine).
 
 ## License Information
 
@@ -495,14 +512,19 @@
 - **Details**: [AzureEngine License](https://learn.microsoft.com/en-us/answers/questions/1192398/can-i-use-azure-text-to-speech-for-commercial-usag)
 
 #### SystemEngine
 - **License**: Mozilla Public License 2.0 and GNU Lesser General Public License (LGPL) version 3.0.
 - **Commercial Use**: Allowed under this license.
 - **Details**: [SystemEngine License](https://github.com/nateshmbhat/pyttsx3/blob/master/LICENSE)
 
+#### GTTSEngine
+- **License**: MIT license
+- **Commercial Use**: It's under the MIT license, so it should be possible in theory. Since it utilizes undocumented Google Translate speech functionality, some caution might be necessary.
+- **Details**: [GTTS MIT License](https://github.com/pndurette/gTTS/blob/main/LICENSE)
+
 #### OpenAIEngine
 - **License**: please read [OpenAI Terms of Use](https://openai.com/policies/terms-of-use)
 
 **Disclaimer**: This is a summarization of the licenses as understood at the time of writing. It is not legal advice. Please read and respect the licenses of the different engine providers yourself if you plan to use them in a project.
 
 ## Author
```

### Comparing `RealTimeTTS-0.3.48/RealTimeTTS.egg-info/SOURCES.txt` & `RealTimeTTS-0.4.0/RealTimeTTS.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -13,12 +13,13 @@
 RealtimeTTS/engines/azure_engine.py
 RealtimeTTS/engines/base_engine.py
 RealtimeTTS/engines/chinese.json
 RealtimeTTS/engines/coqui_default_voice.json
 RealtimeTTS/engines/coqui_engine.py
 RealtimeTTS/engines/elevenlabs_engine.py
 RealtimeTTS/engines/female.json
+RealtimeTTS/engines/gtts_engine.py
 RealtimeTTS/engines/male.json
 RealtimeTTS/engines/openai_engine.py
 RealtimeTTS/engines/system_engine.py
 tests/test_callbacks.py
 tests/test_on_audio_chunk_callback.py
```

### Comparing `RealTimeTTS-0.3.48/RealtimeTTS/engines/azure_engine.py` & `RealTimeTTS-0.4.0/RealtimeTTS/engines/azure_engine.py`

 * *Files identical despite different names*

### Comparing `RealTimeTTS-0.3.48/RealtimeTTS/engines/base_engine.py` & `RealTimeTTS-0.4.0/RealtimeTTS/engines/base_engine.py`

 * *Files identical despite different names*

### Comparing `RealTimeTTS-0.3.48/RealtimeTTS/engines/chinese.json` & `RealTimeTTS-0.4.0/RealtimeTTS/engines/chinese.json`

 * *Files identical despite different names*

### Comparing `RealTimeTTS-0.3.48/RealtimeTTS/engines/coqui_default_voice.json` & `RealTimeTTS-0.4.0/RealtimeTTS/engines/coqui_default_voice.json`

 * *Files identical despite different names*

### Comparing `RealTimeTTS-0.3.48/RealtimeTTS/engines/coqui_engine.py` & `RealTimeTTS-0.4.0/RealtimeTTS/engines/coqui_engine.py`

 * *Files identical despite different names*

### Comparing `RealTimeTTS-0.3.48/RealtimeTTS/engines/elevenlabs_engine.py` & `RealTimeTTS-0.4.0/RealtimeTTS/engines/elevenlabs_engine.py`

 * *Files identical despite different names*

### Comparing `RealTimeTTS-0.3.48/RealtimeTTS/engines/female.json` & `RealTimeTTS-0.4.0/RealtimeTTS/engines/female.json`

 * *Files identical despite different names*

### Comparing `RealTimeTTS-0.3.48/RealtimeTTS/engines/male.json` & `RealTimeTTS-0.4.0/RealtimeTTS/engines/male.json`

 * *Files identical despite different names*

### Comparing `RealTimeTTS-0.3.48/RealtimeTTS/engines/openai_engine.py` & `RealTimeTTS-0.4.0/RealtimeTTS/engines/openai_engine.py`

 * *Files identical despite different names*

### Comparing `RealTimeTTS-0.3.48/RealtimeTTS/engines/system_engine.py` & `RealTimeTTS-0.4.0/RealtimeTTS/engines/system_engine.py`

 * *Files identical despite different names*

### Comparing `RealTimeTTS-0.3.48/RealtimeTTS/stream_player.py` & `RealTimeTTS-0.4.0/RealtimeTTS/stream_player.py`

 * *Files identical despite different names*

### Comparing `RealTimeTTS-0.3.48/RealtimeTTS/text_to_stream.py` & `RealTimeTTS-0.4.0/RealtimeTTS/text_to_stream.py`

 * *Files identical despite different names*

### Comparing `RealTimeTTS-0.3.48/RealtimeTTS/threadsafe_generators.py` & `RealTimeTTS-0.4.0/RealtimeTTS/threadsafe_generators.py`

 * *Files identical despite different names*

### Comparing `RealTimeTTS-0.3.48/setup.py` & `RealTimeTTS-0.4.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 # Read requirements.txt
 with open('requirements.txt') as f:
     requirements = f.read().splitlines()
 
 setuptools.setup(
     name="RealTimeTTS",
-    version="0.3.48",
+    version="0.4.0",
     author="Kolja Beigel",
     author_email="kolja.beigel@web.de",
     description="*Stream text into audio with an easy-to-use, highly configurable library delivering voice output with minimal latency.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/KoljaB/RealTimeTTS",
     packages=setuptools.find_packages(),
```

### Comparing `RealTimeTTS-0.3.48/tests/test_callbacks.py` & `RealTimeTTS-0.4.0/tests/test_callbacks.py`

 * *Files identical despite different names*

### Comparing `RealTimeTTS-0.3.48/tests/test_on_audio_chunk_callback.py` & `RealTimeTTS-0.4.0/tests/test_on_audio_chunk_callback.py`

 * *Files identical despite different names*

