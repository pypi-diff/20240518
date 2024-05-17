# Comparing `tmp/cartesia-0.0.5rc1.tar.gz` & `tmp/cartesia-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cartesia-0.0.5rc1.tar", last modified: Fri Mar 29 17:20:16 2024, max compression
+gzip compressed data, was "cartesia-0.0.6.tar", last modified: Fri May 17 23:40:18 2024, max compression
```

## Comparing `cartesia-0.0.5rc1.tar` & `cartesia-0.0.6.tar`

### file list

```diff
@@ -1,18 +1,19 @@
-drwxrwxr-x   0 arjun    (243000073) arjun    (243000073)        0 2024-03-29 17:20:16.347590 cartesia-0.0.5rc1/
--rw-r--r--   0 arjun    (243000073) arjun    (243000073)     4863 2024-03-29 17:20:16.344946 cartesia-0.0.5rc1/PKG-INFO
--rw-rw-r--   0 arjun    (243000073) arjun    (243000073)     3475 2024-03-29 05:01:08.000000 cartesia-0.0.5rc1/README.md
-drwxrwxr-x   0 arjun    (243000073) arjun    (243000073)        0 2024-03-29 17:20:16.302987 cartesia-0.0.5rc1/cartesia/
--rw-rw-r--   0 arjun    (243000073) arjun    (243000073)       64 2024-03-26 14:49:34.000000 cartesia-0.0.5rc1/cartesia/__init__.py
--rw-rw-r--   0 arjun    (243000073) arjun    (243000073)    20543 2024-03-29 05:01:08.000000 cartesia-0.0.5rc1/cartesia/tts.py
--rw-rw-r--   0 arjun    (243000073) arjun    (243000073)       25 2024-03-29 17:19:56.000000 cartesia-0.0.5rc1/cartesia/version.py
-drwxrwxr-x   0 arjun    (243000073) arjun    (243000073)        0 2024-03-29 17:20:16.348418 cartesia-0.0.5rc1/cartesia.egg-info/
--rw-r--r--   0 arjun    (243000073) arjun    (243000073)     4863 2024-03-29 17:20:16.000000 cartesia-0.0.5rc1/cartesia.egg-info/PKG-INFO
--rw-rw-r--   0 arjun    (243000073) arjun    (243000073)      267 2024-03-29 17:20:16.000000 cartesia-0.0.5rc1/cartesia.egg-info/SOURCES.txt
--rw-rw-r--   0 arjun    (243000073) arjun    (243000073)        1 2024-03-29 17:20:16.000000 cartesia-0.0.5rc1/cartesia.egg-info/dependency_links.txt
--rw-rw-r--   0 arjun    (243000073) arjun    (243000073)      317 2024-03-29 17:20:16.000000 cartesia-0.0.5rc1/cartesia.egg-info/requires.txt
--rw-rw-r--   0 arjun    (243000073) arjun    (243000073)        9 2024-03-29 17:20:16.000000 cartesia-0.0.5rc1/cartesia.egg-info/top_level.txt
--rw-rw-r--   0 arjun    (243000073) arjun    (243000073)      213 2024-03-16 15:51:29.000000 cartesia-0.0.5rc1/pyproject.toml
--rw-rw-r--   0 arjun    (243000073) arjun    (243000073)       38 2024-03-29 17:20:16.347737 cartesia-0.0.5rc1/setup.cfg
--rw-rw-r--   0 arjun    (243000073) arjun    (243000073)     9207 2024-03-29 15:37:33.000000 cartesia-0.0.5rc1/setup.py
-drwxrwxr-x   0 arjun    (243000073) arjun    (243000073)        0 2024-03-29 17:20:16.349650 cartesia-0.0.5rc1/tests/
--rw-rw-r--   0 arjun    (243000073) arjun    (243000073)     7510 2024-03-29 05:01:08.000000 cartesia-0.0.5rc1/tests/test_tts.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 23:40:18.810603 cartesia-0.0.6/
+-rw-r--r--   0 runner    (1001) docker     (127)     5416 2024-05-17 23:40:18.810603 cartesia-0.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4967 2024-05-17 23:39:52.000000 cartesia-0.0.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 23:40:18.810603 cartesia-0.0.6/cartesia/
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-05-17 23:39:52.000000 cartesia-0.0.6/cartesia/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26734 2024-05-17 23:39:52.000000 cartesia-0.0.6/cartesia/tts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3024 2024-05-17 23:39:52.000000 cartesia-0.0.6/cartesia/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-17 23:39:52.000000 cartesia-0.0.6/cartesia/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 23:40:18.810603 cartesia-0.0.6/cartesia.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5416 2024-05-17 23:40:18.000000 cartesia-0.0.6/cartesia.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-05-17 23:40:18.000000 cartesia-0.0.6/cartesia.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-17 23:40:18.000000 cartesia-0.0.6/cartesia.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      173 2024-05-17 23:40:18.000000 cartesia-0.0.6/cartesia.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-17 23:40:18.000000 cartesia-0.0.6/cartesia.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1702 2024-05-17 23:39:52.000000 cartesia-0.0.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-17 23:40:18.810603 cartesia-0.0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     9241 2024-05-17 23:39:52.000000 cartesia-0.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 23:40:18.810603 cartesia-0.0.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    10533 2024-05-17 23:39:52.000000 cartesia-0.0.6/tests/test_tts.py
```

### Comparing `cartesia-0.0.5rc1/PKG-INFO` & `cartesia-0.0.6/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,46 +1,7 @@
-Metadata-Version: 2.1
-Name: cartesia
-Version: 0.0.5rc1
-Summary: The official Python library for the Cartesia API.
-Home-page: 
-Author: Cartesia, Inc.
-Author-email: support@cartesia.ai
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
-Requires-Python: >=3.8.0
-Description-Content-Type: text/markdown
-Requires-Dist: aiohttp
-Requires-Dist: httpx
-Requires-Dist: pytest-asyncio
-Requires-Dist: requests
-Requires-Dist: websockets
-Provides-Extra: dev
-Requires-Dist: pre-commit; extra == "dev"
-Requires-Dist: docformatter; extra == "dev"
-Requires-Dist: black==24.1.1; extra == "dev"
-Requires-Dist: isort==5.13.2; extra == "dev"
-Requires-Dist: flake8==7.0.0; extra == "dev"
-Requires-Dist: flake8-bugbear==24.2.6; extra == "dev"
-Requires-Dist: pytest>=8.0.2; extra == "dev"
-Requires-Dist: pytest-cov>=4.1.0; extra == "dev"
-Requires-Dist: twine; extra == "dev"
-Provides-Extra: all
-Requires-Dist: pre-commit; extra == "all"
-Requires-Dist: docformatter; extra == "all"
-Requires-Dist: black==24.1.1; extra == "all"
-Requires-Dist: isort==5.13.2; extra == "all"
-Requires-Dist: flake8==7.0.0; extra == "all"
-Requires-Dist: flake8-bugbear==24.2.6; extra == "all"
-Requires-Dist: pytest>=8.0.2; extra == "all"
-Requires-Dist: pytest-cov>=4.1.0; extra == "all"
-Requires-Dist: twine; extra == "all"
-
-
 # Cartesia Python API Library
 The official Cartesia Python library which provides convenient access to the Cartesia REST and Websocket API from any Python 3.8+ application.
 
 **Note:** This API is still in alpha. Please expect breaking changes and report any issues you encounter.
 
 ## Installation
 ```bash
@@ -56,21 +17,22 @@
 import pyaudio
 import os
 
 client = CartesiaTTS(api_key=os.environ.get("CARTESIA_API_KEY"))
 voices = client.get_voices()
 voice = client.get_voice_embedding(voice_id=voices["Graham"]["id"])
 transcript = "Hello! Welcome to Cartesia"
+model_id = "genial-planet-1346" # (Optional) We'll specify a default if you don't have a specific model in mind
 
 p = pyaudio.PyAudio()
 
 stream = None
 
 # Generate and stream audio
-for output in client.generate(transcript=transcript, voice=voice, stream=True):
+for output in client.generate(transcript=transcript, voice=voice, model_id=model_id, stream=True):
     buffer = output["audio"]
     rate = output["sampling_rate"]
 
     if not stream:
         stream = p.open(format=pyaudio.paFloat32,
                         channels=1,
                         rate=rate,
@@ -80,64 +42,108 @@
     stream.write(buffer)
 
 stream.stop_stream()
 stream.close()
 p.terminate()
 ```
 
-If you are using Jupyter Notebook or JupyterLab, you can use IPython.display.Audio to play the generated audio directly in the notebook. Here's an example:
+You can also use the async client if you want to make asynchronous API calls:
+```python
+from cartesia.tts import AsyncCartesiaTTS
+import asyncio
+import pyaudio
+import os
+
+async def write_stream():
+    client = AsyncCartesiaTTS(api_key=os.environ.get("CARTESIA_API_KEY"))
+    voices = client.get_voices()
+    voice = client.get_voice_embedding(voice_id=voices["Graham"]["id"])
+    transcript = "Hello! Welcome to Cartesia"
+    model_id = "genial-planet-1346" # (Optional) We'll specify a default if you don't have a specific model in mind
+
+    p = pyaudio.PyAudio()
+
+    stream = None
+
+    # Generate and stream audio
+    async for output in await client.generate(transcript=transcript, voice=voice, model_id=model_id, stream=True):
+        buffer = output["audio"]
+        rate = output["sampling_rate"]
+
+        if not stream:
+            stream = p.open(format=pyaudio.paFloat32,
+                            channels=1,
+                            rate=rate,
+                            output=True)
+
+        # Write the audio data to the stream
+        stream.write(buffer)
+
+    stream.stop_stream()
+    stream.close()
+    p.terminate()
+
+asyncio.run(write_stream())
+```
+
+If you are using Jupyter Notebook or JupyterLab, you can use IPython.display.Audio to play the generated audio directly in the notebook.
+Additionally, in these notebook examples we show how to use the client as a context manager (though this is not required).
 
 ```python
-from cartesia.tts import CartesiaTTS
 from IPython.display import Audio
 import io
 import os
+import numpy as np
 
-client = CartesiaTTS(api_key=os.environ.get("CARTESIA_API_KEY"))
-voices = client.get_voices()
-voice = client.get_voice_embedding(voice_id=voices["Graham"]["id"])
-transcript = "Hello! Welcome to Cartesia"
+from cartesia.tts import CartesiaTTS
 
-# Create a BytesIO object to store the audio data
-audio_data = io.BytesIO()
-
-# Generate and stream audio
-for output in client.generate(transcript=transcript, voice=voice, stream=True):
-    buffer = output["audio"]
-    audio_data.write(buffer)
+with CartesiaTTS(api_key=os.environ.get("CARTESIA_API_KEY")) as client:
+    voices = client.get_voices()
+    voice = client.get_voice_embedding(voice_id=voices["Graham"]["id"])
+    transcript = "Hello! Welcome to Cartesia"
+
+    # Create a BytesIO object to store the audio data
+    audio_data = io.BytesIO()
+
+    # Generate and stream audio
+    for output in client.generate(transcript=transcript, voice=voice, stream=True):
+        buffer = output["audio"]
+        audio_data.write(buffer)
 
 # Set the cursor position to the beginning of the BytesIO object
 audio_data.seek(0)
 
 # Create an Audio object from the BytesIO data
 audio = Audio(np.frombuffer(audio_data.read(), dtype=np.float32), rate=output["sampling_rate"])
 
 # Display the Audio object
 display(audio)
 ```
 
-You can also use the async client if you want to make asynchronous API calls. The usage is very similar:
+Below is the same example using the async client:
 ```python
-from cartesia.tts import AsyncCartesiaTTS
 from IPython.display import Audio
 import io
 import os
+import numpy as np
 
-client = AsyncCartesiaTTS(api_key=os.environ.get("CARTESIA_API_KEY"))
-voices = client.get_voices()
-voice = client.get_voice_embedding(voice_id=voices["Graham"]["id"])
-transcript = "Hello! Welcome to Cartesia"
-
-# Create a BytesIO object to store the audio data
-audio_data = io.BytesIO()
+from cartesia.tts import AsyncCartesiaTTS
 
-# Generate and stream audio
-async for output in client.generate(transcript=transcript, voice=voice, stream=True):
-    buffer = output["audio"]
-    audio_data.write(buffer)
+async with AsyncCartesiaTTS(api_key=os.environ.get("CARTESIA_API_KEY")) as client:
+    voices = client.get_voices()
+    voice = client.get_voice_embedding(voice_id=voices["Graham"]["id"])
+    transcript = "Hello! Welcome to Cartesia"
+
+    # Create a BytesIO object to store the audio data
+    audio_data = io.BytesIO()
+
+    # Generate and stream audio
+    async for output in await client.generate(transcript=transcript, voice=voice, stream=True):
+        buffer = output["audio"]
+        audio_data.write(buffer)
 
 # Set the cursor position to the beginning of the BytesIO object
 audio_data.seek(0)
 
 # Create an Audio object from the BytesIO data
 audio = Audio(np.frombuffer(audio_data.read(), dtype=np.float32), rate=output["sampling_rate"])
```

### Comparing `cartesia-0.0.5rc1/cartesia/tts.py` & `cartesia-0.0.6/cartesia/tts.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,25 +1,33 @@
 import asyncio
 import base64
 import json
 import os
 import uuid
+from types import TracebackType
 from typing import Any, AsyncGenerator, Dict, Generator, List, Optional, Tuple, TypedDict, Union
 
 import aiohttp
 import httpx
+import logging
 import requests
 from websockets.sync.client import connect
 
-DEFAULT_MODEL_ID = "genial-planet-1346"
+from cartesia.utils import retry_on_connection_error, retry_on_connection_error_async
+
+DEFAULT_MODEL_ID = ""
 DEFAULT_BASE_URL = "api.cartesia.ai"
 DEFAULT_API_VERSION = "v0"
-DEFAULT_TIMEOUT = 60  # seconds
+DEFAULT_TIMEOUT = 30  # seconds
 DEFAULT_NUM_CONNECTIONS = 10  # connections per client
 
+BACKOFF_FACTOR = 1
+MAX_RETRIES = 3
+
+logger = logging.getLogger(__name__)
 
 class AudioOutput(TypedDict):
     audio: bytes
     sampling_rate: int
 
 
 Embedding = List[float]
@@ -70,15 +78,14 @@
     The client can be used to retrieve available voices, compute new voice embeddings,
     and generate speech from text.
 
     The client also supports generating audio using a websocket for lower latency.
     To enable interrupt handling along the websocket, set `experimental_ws_handle_interrupts=True`.
 
     Examples:
-
         >>> client = CartesiaTTS()
 
         # Load available voices and their metadata (excluding the embeddings).
         # Embeddings are fetched with `get_voice_embedding`. This avoids preloading
         # all of the embeddings, which can be expensive if there are a lot of voices.
         >>> voices = client.get_voices()
         >>> embedding = client.get_voice_embedding(voice_id=voices["Milo"]["id"])
@@ -92,30 +99,28 @@
 
         # Generate audio stream
         >>> for audio_chunk in client.generate(transcript="Hello world!", voice=embedding, stream=True):
         ...     audio, sr = audio_chunk["audio"], audio_chunk["sampling_rate"]
     """
 
     def __init__(self, *, api_key: str = None, experimental_ws_handle_interrupts: bool = False):
-        """
-        Args:
-            api_key: The API key to use for authorization.
-                If not specified, the API key will be read from the environment variable
-                `CARTESIA_API_KEY`.
-            experimental_ws_handle_interrupts: Whether to handle interrupts when generating
-                audio using the websocket. This is an experimental feature and may have bugs
-                or be deprecated in the future.
+        """Args:
+        api_key: The API key to use for authorization.
+            If not specified, the API key will be read from the environment variable
+            `CARTESIA_API_KEY`.
+        experimental_ws_handle_interrupts: Whether to handle interrupts when generating
+            audio using the websocket. This is an experimental feature and may have bugs
+            or be deprecated in the future.
         """
         self.base_url = os.environ.get("CARTESIA_BASE_URL", DEFAULT_BASE_URL)
         self.api_key = api_key or os.environ.get("CARTESIA_API_KEY")
         self.api_version = os.environ.get("CARTESIA_API_VERSION", DEFAULT_API_VERSION)
         self.headers = {"X-API-Key": self.api_key, "Content-Type": "application/json"}
         self.websocket = None
         self.experimental_ws_handle_interrupts = experimental_ws_handle_interrupts
-        self.refresh_websocket()
 
     def get_voices(self, skip_embeddings: bool = True) -> Dict[str, VoiceMetadata]:
         """Returns a mapping from voice name -> voice metadata.
 
         Args:
             skip_embeddings: Whether to skip returning the embeddings.
                 It is recommended to skip if you only want to see what
@@ -140,26 +145,31 @@
                         "id": "c1d1d3a8-6f4e-4b3f-8b3e-2e1b3e1b3e1b",
                         "name": "Jane",
                 }
             >>> embedding = client.get_voice_embedding(voice_id=voices["Jane"]["id"])
             >>> audio = client.generate(transcript="Hello world!", voice=embedding)
         """
         params = {"select": "id, name, description"} if skip_embeddings else None
-        response = httpx.get(f"{self._http_url()}/voices", headers=self.headers, params=params)
+        response = httpx.get(
+            f"{self._http_url()}/voices",
+            headers=self.headers,
+            params=params,
+            timeout=DEFAULT_TIMEOUT,
+        )
 
         if not response.is_success:
             raise ValueError(f"Failed to get voices. Error: {response.text}")
 
         voices = response.json()
-        # TODO: Update the API to return the embedding as a list of floats rather than string.
-        if not skip_embeddings:
-            for voice in voices:
+        for voice in voices:
+            if "embedding" in voice and isinstance(voice["embedding"], str):
                 voice["embedding"] = json.loads(voice["embedding"])
         return {voice["name"]: voice for voice in voices}
 
+    @retry_on_connection_error(max_retries=MAX_RETRIES, backoff_factor=BACKOFF_FACTOR, logger=logger)
     def get_voice_embedding(
         self, *, voice_id: str = None, filepath: str = None, link: str = None
     ) -> Embedding:
         """Get a voice embedding from voice_id, a filepath or YouTube url.
 
         Args:
             voice_id: The voice id.
@@ -174,54 +184,51 @@
                 Only one should be specified.
         """
         if sum(bool(x) for x in (voice_id, filepath, link)) != 1:
             raise ValueError("Exactly one of `voice_id`, `filepath` or `url` should be specified.")
 
         if voice_id:
             url = f"{self._http_url()}/voices/embedding/{voice_id}"
-            response = httpx.get(url, headers=self.headers)
+            response = httpx.get(url, headers=self.headers, timeout=DEFAULT_TIMEOUT)
         elif filepath:
             url = f"{self._http_url()}/voices/clone/clip"
             files = {"clip": open(filepath, "rb")}
             headers = self.headers.copy()
             # The default content type of JSON is incorrect for file uploads
             headers.pop("Content-Type")
-            response = httpx.post(url, headers=headers, files=files)
+            response = httpx.post(url, headers=headers, files=files, timeout=DEFAULT_TIMEOUT)
         elif link:
             url = f"{self._http_url()}/voices/clone/url"
             params = {"link": link}
-            response = httpx.post(url, headers=self.headers, params=params)
+            response = httpx.post(url, headers=self.headers, params=params, timeout=DEFAULT_TIMEOUT)
 
         if not response.is_success:
             raise ValueError(
                 f"Failed to clone voice. Status Code: {response.status_code}\n"
                 f"Error: {response.text}"
             )
 
         # Handle successful response
         out = response.json()
-        if isinstance(out["embedding"], str):
-            out["embedding"] = json.loads(out["embedding"])
-        return out["embedding"]
+        embedding = out["embedding"]
+        if isinstance(embedding, str):
+            embedding = json.loads(embedding)
+        return embedding
 
     def refresh_websocket(self):
         """Refresh the websocket connection.
 
         Note:
             The connection is synchronous.
         """
-        if self.websocket and not self._is_websocket_closed():
-            self.websocket.close()
-        route = "audio/websocket"
-        if self.experimental_ws_handle_interrupts:
-            route = f"experimental/{route}"
-        self.websocket = connect(
-            f"{self._ws_url()}/{route}?api_key={self.api_key}",
-            close_timeout=None,
-        )
+        if self.websocket is None or self._is_websocket_closed():
+            route = "audio/websocket"
+            if self.experimental_ws_handle_interrupts:
+                route = f"experimental/{route}"
+            self.websocket = connect(f"{self._ws_url()}/{route}?api_key={self.api_key}")
 
     def _is_websocket_closed(self):
         return self.websocket.socket.fileno() == -1
 
     def _check_inputs(
         self, transcript: str, duration: Optional[float], chunk_time: Optional[float]
     ):
@@ -236,92 +243,112 @@
         if transcript.strip() == "":
             raise ValueError("`transcript` must be non empty")
 
     def _generate_request_body(
         self,
         *,
         transcript: str,
+        voice: Embedding,
+        model_id: str,
+        output_format: str,
         duration: int = None,
         chunk_time: float = None,
-        voice: Embedding = None,
     ) -> Dict[str, Any]:
+        """Create the request body for a stream request.
+
+        Note that anything that's not provided will use a default if available or be
+        filtered out otherwise.
         """
-        Create the request body for a stream request.
-        Note that anything that's not provided will use a default if available or be filtered out otherwise.
-        """
-        body = dict(transcript=transcript, model_id=DEFAULT_MODEL_ID, voice=voice)
+        body = dict(transcript=transcript, model_id=model_id, voice=voice)
 
         optional_body = dict(
             duration=duration,
             chunk_time=chunk_time,
-            voice=voice,
+            output_format=output_format,
         )
         body.update({k: v for k, v in optional_body.items() if v is not None})
 
         return body
 
     def generate(
         self,
         *,
         transcript: str,
+        voice: Embedding,
+        model_id: str = DEFAULT_MODEL_ID,
         duration: int = None,
         chunk_time: float = None,
-        voice: Embedding = None,
         stream: bool = False,
         websocket: bool = True,
+        output_format: str = "fp32",
     ) -> Union[AudioOutput, Generator[AudioOutput, None, None]]:
         """Generate audio from a transcript.
 
         Args:
-            transcript: The text to generate audio for.
-            duration: The maximum duration of the audio in seconds.
-            chunk_time: How long each audio segment should be in seconds.
+            transcript (str): The text to generate audio for.
+            voice (Embedding (List[float])): The voice to use for generating audio.
+            duration (int, optional): The maximum duration of the audio in seconds.
+            chunk_time (float, optional): How long each audio segment should be in seconds.
                 This should not need to be adjusted.
-            voice: The voice to use for generating audio.
-                This can either be a voice id (string) or an embedding vector (List[float]).
-            stream: Whether to stream the audio or not.
-                If ``True`` this function returns a generator.
-            websocket: Whether to use a websocket for streaming audio.
-                Using the websocket reduces latency by pre-poning the handshake.
+            stream (bool, optional): Whether to stream the audio or not.
+                If True this function returns a generator. False by default.
+            websocket (bool, optional): Whether to use a websocket for streaming audio.
+                Using the websocket reduces latency by pre-poning the handshake. True by default.
 
         Returns:
             A generator if `stream` is True, otherwise a dictionary.
             Dictionary from both generator and non-generator return types have the following keys:
                 * "audio": The audio as a bytes buffer.
                 * "sampling_rate": The sampling rate of the audio.
         """
         self._check_inputs(transcript, duration, chunk_time)
 
         body = self._generate_request_body(
-            transcript=transcript, duration=duration, chunk_time=chunk_time, voice=voice
+            transcript=transcript, 
+            voice=voice, 
+            model_id=model_id,
+            duration=duration, 
+            chunk_time=chunk_time,
+            output_format=output_format,
         )
 
         if websocket:
             generator = self._generate_ws(body)
         else:
-            generator = self._generate_http(body)
+            generator = self._generate_http_wrapper(body)
 
         if stream:
             return generator
 
         chunks = []
         sampling_rate = None
         for chunk in generator:
             if sampling_rate is None:
                 sampling_rate = chunk["sampling_rate"]
             chunks.append(chunk["audio"])
 
         return {"audio": b"".join(chunks), "sampling_rate": sampling_rate}
 
+    @retry_on_connection_error(max_retries=MAX_RETRIES, backoff_factor=BACKOFF_FACTOR, logger=logger)
+    def _generate_http_wrapper(self, body: Dict[str, Any]):
+        """Need to wrap the http generator in a function for the retry decorator to work."""
+        try:
+            for chunk in self._generate_http(body):
+                yield chunk
+        except Exception as e:
+            logger.error(f"Failed to generate audio. {e}")
+            raise e
+
     def _generate_http(self, body: Dict[str, Any]):
         response = requests.post(
-            f"{self._http_url()}/audio/stream",
+            f"{self._http_url()}/audio/sse",
             stream=True,
             data=json.dumps(body),
             headers=self.headers,
+            timeout=(DEFAULT_TIMEOUT, DEFAULT_TIMEOUT),
         )
         if not response.ok:
             raise ValueError(f"Failed to generate audio. {response.text}")
 
         buffer = ""
         for chunk_bytes in response.iter_content(chunk_size=None):
             buffer, outputs = update_buffer(buffer, chunk_bytes)
@@ -352,114 +379,219 @@
         include_context_id = bool(context_id)
         if context_id is None:
             context_id = uuid.uuid4().hex
         self.websocket.send(json.dumps({"data": body, "context_id": context_id}))
         try:
             while True:
                 response = json.loads(self.websocket.recv())
+                if "error" in response:
+                    raise RuntimeError(f"Error generating audio:\n{response['error']}")
                 if response["done"]:
                     break
 
                 yield convert_response(response, include_context_id)
 
                 if self.experimental_ws_handle_interrupts:
                     self.websocket.send(json.dumps({"context_id": context_id}))
         except GeneratorExit:
             # The exit is only called when the generator is garbage collected.
             # It may not be called directly after a break statement.
             # However, the generator will be automatically cancelled on the next request.
             if self.experimental_ws_handle_interrupts:
                 self.websocket.send(json.dumps({"context_id": context_id, "action": "cancel"}))
         except Exception as e:
+            # Close the websocket connection if an error occurs.
+            if self.websocket and not self._is_websocket_closed():
+                self.websocket.close()
             raise RuntimeError(f"Failed to generate audio. {response}") from e
+        finally:
+            # Ensure the websocket is ultimately closed.
+            if self.websocket and not self._is_websocket_closed():
+                self.websocket.close()
+
+    @retry_on_connection_error(max_retries=MAX_RETRIES, backoff_factor=BACKOFF_FACTOR, logger=logger)
+    def transcribe(self, raw_audio: Union[bytes, str]) -> str:
+        raw_audio_bytes, headers = self.prepare_audio_and_headers(raw_audio)
+        response = httpx.post(
+            f"{self._http_url()}/audio/transcriptions",
+            headers=headers,
+            files={"clip": ("input.wav", raw_audio_bytes)},
+            timeout=DEFAULT_TIMEOUT,
+        )
+
+        if not response.is_success:
+            raise ValueError(f"Failed to transcribe audio. Error: {response.text()}")
+
+        transcript = response.json()
+        return transcript["text"]
+
+
+    def prepare_audio_and_headers(
+        self, raw_audio: Union[bytes, str]
+    ) -> Tuple[bytes, Dict[str, Any]]:
+        if isinstance(raw_audio, str):
+            with open(raw_audio, "rb") as f:
+                raw_audio_bytes = f.read()
+        else:
+            raw_audio_bytes = raw_audio
+        # application/json is not the right content type for this request
+        headers = {k: v for k, v in self.headers.items() if k != "Content-Type"}
+        return raw_audio_bytes, headers
 
     def _http_url(self):
         prefix = "http" if "localhost" in self.base_url else "https"
         return f"{prefix}://{self.base_url}/{self.api_version}"
 
     def _ws_url(self):
         prefix = "ws" if "localhost" in self.base_url else "wss"
         return f"{prefix}://{self.base_url}/{self.api_version}"
 
-    def __del__(self):
-        if self.websocket.socket.fileno() > -1:
+    def close(self):
+        if self.websocket and not self._is_websocket_closed():
             self.websocket.close()
 
+    def __del__(self):
+        self.close()
+
+    def __enter__(self):
+        self.refresh_websocket()
+        return self
+
+    def __exit__(
+        self,
+        exc_type: Union[type, None],
+        exc: Union[BaseException, None],
+        exc_tb: Union[TracebackType, None],
+    ):
+        self.close()
+
 
 class AsyncCartesiaTTS(CartesiaTTS):
     def __init__(self, *, api_key: str = None, experimental_ws_handle_interrupts: bool = False):
-        self.timeout = aiohttp.ClientTimeout(total=DEFAULT_TIMEOUT)
-        self.connector = aiohttp.TCPConnector(limit=DEFAULT_NUM_CONNECTIONS)
-        self._session = aiohttp.ClientSession(timeout=self.timeout, connector=self.connector)
+        self._session = None
+        self._loop = None
         super().__init__(
             api_key=api_key, experimental_ws_handle_interrupts=experimental_ws_handle_interrupts
         )
-
-    def refresh_websocket(self):
-        pass  # do not load the websocket for the client until asynchronously when it is needed
-
-    async def _async_refresh_websocket(self):
+    
+    async def _get_session(self):
+        current_loop = asyncio.get_event_loop()
+        if self._loop is not current_loop:
+            # If the loop has changed, close the session and create a new one.
+            await self.close()
+        if self._session is None or self._session.closed:
+            timeout = aiohttp.ClientTimeout(total=DEFAULT_TIMEOUT)
+            connector = aiohttp.TCPConnector(limit=DEFAULT_NUM_CONNECTIONS)
+            self._session = aiohttp.ClientSession(
+                timeout=timeout, connector=connector
+            )
+            self._loop = current_loop
+        return self._session
+    
+    async def refresh_websocket(self):
         """Refresh the websocket connection."""
-        if self.websocket and not self._is_websocket_closed():
-            self.websocket.close()
-        route = "audio/websocket"
-        if self.experimental_ws_handle_interrupts:
-            route = f"experimental/{route}"
-        self.websocket = await self._session.ws_connect(
-            f"{self._ws_url()}/{route}?api_key={self.api_key}"
-        )
+        if self.websocket is None or self._is_websocket_closed():
+            route = "audio/websocket"
+            if self.experimental_ws_handle_interrupts:
+                route = f"experimental/{route}"
+            session = await self._get_session()
+            self.websocket = await session.ws_connect(
+                f"{self._ws_url()}/{route}?api_key={self.api_key}"
+            )
+    
+    def _is_websocket_closed(self):
+        return self.websocket.closed
+
+    async def close(self):
+        """This method closes the websocket and the session.
+        
+        It is *strongly* recommended to call this method when you are done using the client.
+        """
+        if self.websocket is not None and not self._is_websocket_closed():
+            await self.websocket.close()
+        if self._session is not None and not self._session.closed:
+            await self._session.close()
 
     async def generate(
         self,
         *,
         transcript: str,
+        voice: Embedding,
+        model_id: str = DEFAULT_MODEL_ID,
         duration: int = None,
         chunk_time: float = None,
-        voice: Embedding = None,
         stream: bool = False,
         websocket: bool = True,
+        output_format: str = "fp32"
     ) -> Union[AudioOutput, AsyncGenerator[AudioOutput, None]]:
         """Asynchronously generate audio from a transcript.
         NOTE: This overrides the non-asynchronous generate method from the base class.
+
         Args:
-            transcript: The text to generate audio for.
-            voice: The embedding to use for generating audio.
-            options: The options to use for generating audio. See :class:`GenerateOptions`.
+            transcript (str): The text to generate audio for.
+            voice (Embedding (List[float])): The voice to use for generating audio.
+            duration (int, optional): The maximum duration of the audio in seconds.
+            chunk_time (float, optional): How long each audio segment should be in seconds.
+                This should not need to be adjusted.
+            stream (bool, optional): Whether to stream the audio or not.
+                If True this function returns a generator. False by default.
+            websocket (bool, optional): Whether to use a websocket for streaming audio.
+                Using the websocket reduces latency by pre-poning the handshake. True by default.
+
         Returns:
-            A dictionary containing the following:
-                * "audio": The audio as a 1D numpy array.
+            A generator if `stream` is True, otherwise a dictionary.
+            Dictionary from both generator and non-generator return types have the following keys:
+                * "audio": The audio as a bytes buffer.
                 * "sampling_rate": The sampling rate of the audio.
         """
+        self._check_inputs(transcript, duration, chunk_time)
+
         body = self._generate_request_body(
-            transcript=transcript, duration=duration, chunk_time=chunk_time, voice=voice
+            transcript=transcript, 
+            voice=voice,
+            model_id=model_id,
+            duration=duration, 
+            chunk_time=chunk_time,
+            output_format=output_format,
         )
 
         if websocket:
             generator = self._generate_ws(body)
         else:
-            generator = self._generate_http(body)
+            generator = self._generate_http_wrapper(body)
 
         if stream:
             return generator
 
         chunks = []
         sampling_rate = None
         async for chunk in generator:
             if sampling_rate is None:
                 sampling_rate = chunk["sampling_rate"]
             chunks.append(chunk["audio"])
 
         return {"audio": b"".join(chunks), "sampling_rate": sampling_rate}
 
+    @retry_on_connection_error_async(max_retries=MAX_RETRIES, backoff_factor=BACKOFF_FACTOR, logger=logger)
+    async def _generate_http_wrapper(self, body: Dict[str, Any]):
+        """Need to wrap the http generator in a function for the retry decorator to work."""
+        try:
+          async for chunk in self._generate_http(body):
+              yield chunk
+        except Exception as e:
+            logger.error(f"Failed to generate audio. {e}")
+            raise e
+
     async def _generate_http(self, body: Dict[str, Any]):
-        async with self._session.post(
-            f"{self._http_url()}/audio/stream", data=json.dumps(body), headers=self.headers
+        session = await self._get_session()
+        async with session.post(
+            f"{self._http_url()}/audio/sse", data=json.dumps(body), headers=self.headers
         ) as response:
-            if response.status < 200 or response.status >= 300:
-                raise ValueError(f"Failed to generate audio. {response.text}")
+            if not response.ok:
+                raise ValueError(f"Failed to generate audio. {await response.text()}")
 
             buffer = ""
             async for chunk_bytes in response.content.iter_any():
                 buffer, outputs = update_buffer(buffer, chunk_bytes)
                 for output in outputs:
                     yield output
 
@@ -474,15 +606,15 @@
     async def _generate_ws(self, body: Dict[str, Any], *, context_id: str = None):
         include_context_id = bool(context_id)
         route = "audio/websocket"
         if self.experimental_ws_handle_interrupts:
             route = f"experimental/{route}"
 
         if not self.websocket or self._is_websocket_closed():
-            await self._async_refresh_websocket()
+            await self.refresh_websocket()
 
         ws = self.websocket
         if context_id is None:
             context_id = uuid.uuid4().hex
         await ws.send_json({"data": body, "context_id": context_id})
         try:
             response = None
@@ -498,28 +630,52 @@
         except GeneratorExit:
             # The exit is only called when the generator is garbage collected.
             # It may not be called directly after a break statement.
             # However, the generator will be automatically cancelled on the next request.
             if self.experimental_ws_handle_interrupts:
                 await ws.send_json({"context_id": context_id, "action": "cancel"})
         except Exception as e:
-            raise RuntimeError(f"Failed to generate audio. {response}") from e
-
-    def _is_websocket_closed(self):
-        return self.websocket.closed
+            if self.websocket and not self._is_websocket_closed():
+                await self.websocket.close()
+            raise RuntimeError(f"Failed to generate audio. {await response.text()}") from e
+        finally:
+            # Ensure the websocket is ultimately closed.
+            if self.websocket and not self._is_websocket_closed():
+                await self.websocket.close()
+
+    async def transcribe(self, raw_audio: Union[bytes, str]) -> str:
+        raw_audio_bytes, headers = self.prepare_audio_and_headers(raw_audio)
+        data = aiohttp.FormData()
+        data.add_field("clip", raw_audio_bytes, filename="input.wav", content_type="audio/wav")
+        session = await self._get_session()
 
-    async def cleanup(self):
-        if self.websocket is not None and not self._is_websocket_closed():
-            await self.websocket.close()
-        if not self._session.closed:
-            await self._session.close()
+        async with session.post(
+            f"{self._http_url()}/audio/transcriptions", headers=headers, data=data
+        ) as response:
+            if not response.ok:
+                raise ValueError(f"Failed to transcribe audio. Error: {await response.text()}")
 
+            transcript = await response.json()
+            return transcript["text"]
+        
     def __del__(self):
         try:
             loop = asyncio.get_running_loop()
         except RuntimeError:
             loop = None
 
         if loop is None:
-            asyncio.run(self.cleanup())
+            asyncio.run(self.close())
         else:
-            loop.create_task(self.cleanup())
+            loop.create_task(self.close())
+
+    async def __aenter__(self):
+        await self.refresh_websocket()
+        return self
+
+    async def __aexit__(
+        self,
+        exc_type: Union[type, None],
+        exc: Union[BaseException, None],
+        exc_tb: Union[TracebackType, None],
+    ):
+        await self.close()
```

### Comparing `cartesia-0.0.5rc1/cartesia.egg-info/PKG-INFO` & `cartesia-0.0.6/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,44 +1,21 @@
 Metadata-Version: 2.1
 Name: cartesia
-Version: 0.0.5rc1
+Version: 0.0.6
 Summary: The official Python library for the Cartesia API.
 Home-page: 
 Author: Cartesia, Inc.
 Author-email: support@cartesia.ai
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Requires-Python: >=3.8.0
 Description-Content-Type: text/markdown
-Requires-Dist: aiohttp
-Requires-Dist: httpx
-Requires-Dist: pytest-asyncio
-Requires-Dist: requests
-Requires-Dist: websockets
 Provides-Extra: dev
-Requires-Dist: pre-commit; extra == "dev"
-Requires-Dist: docformatter; extra == "dev"
-Requires-Dist: black==24.1.1; extra == "dev"
-Requires-Dist: isort==5.13.2; extra == "dev"
-Requires-Dist: flake8==7.0.0; extra == "dev"
-Requires-Dist: flake8-bugbear==24.2.6; extra == "dev"
-Requires-Dist: pytest>=8.0.2; extra == "dev"
-Requires-Dist: pytest-cov>=4.1.0; extra == "dev"
-Requires-Dist: twine; extra == "dev"
 Provides-Extra: all
-Requires-Dist: pre-commit; extra == "all"
-Requires-Dist: docformatter; extra == "all"
-Requires-Dist: black==24.1.1; extra == "all"
-Requires-Dist: isort==5.13.2; extra == "all"
-Requires-Dist: flake8==7.0.0; extra == "all"
-Requires-Dist: flake8-bugbear==24.2.6; extra == "all"
-Requires-Dist: pytest>=8.0.2; extra == "all"
-Requires-Dist: pytest-cov>=4.1.0; extra == "all"
-Requires-Dist: twine; extra == "all"
 
 
 # Cartesia Python API Library
 The official Cartesia Python library which provides convenient access to the Cartesia REST and Websocket API from any Python 3.8+ application.
 
 **Note:** This API is still in alpha. Please expect breaking changes and report any issues you encounter.
 
@@ -56,21 +33,22 @@
 import pyaudio
 import os
 
 client = CartesiaTTS(api_key=os.environ.get("CARTESIA_API_KEY"))
 voices = client.get_voices()
 voice = client.get_voice_embedding(voice_id=voices["Graham"]["id"])
 transcript = "Hello! Welcome to Cartesia"
+model_id = "genial-planet-1346" # (Optional) We'll specify a default if you don't have a specific model in mind
 
 p = pyaudio.PyAudio()
 
 stream = None
 
 # Generate and stream audio
-for output in client.generate(transcript=transcript, voice=voice, stream=True):
+for output in client.generate(transcript=transcript, voice=voice, model_id=model_id, stream=True):
     buffer = output["audio"]
     rate = output["sampling_rate"]
 
     if not stream:
         stream = p.open(format=pyaudio.paFloat32,
                         channels=1,
                         rate=rate,
@@ -80,64 +58,108 @@
     stream.write(buffer)
 
 stream.stop_stream()
 stream.close()
 p.terminate()
 ```
 
-If you are using Jupyter Notebook or JupyterLab, you can use IPython.display.Audio to play the generated audio directly in the notebook. Here's an example:
+You can also use the async client if you want to make asynchronous API calls:
+```python
+from cartesia.tts import AsyncCartesiaTTS
+import asyncio
+import pyaudio
+import os
+
+async def write_stream():
+    client = AsyncCartesiaTTS(api_key=os.environ.get("CARTESIA_API_KEY"))
+    voices = client.get_voices()
+    voice = client.get_voice_embedding(voice_id=voices["Graham"]["id"])
+    transcript = "Hello! Welcome to Cartesia"
+    model_id = "genial-planet-1346" # (Optional) We'll specify a default if you don't have a specific model in mind
+
+    p = pyaudio.PyAudio()
+
+    stream = None
+
+    # Generate and stream audio
+    async for output in await client.generate(transcript=transcript, voice=voice, model_id=model_id, stream=True):
+        buffer = output["audio"]
+        rate = output["sampling_rate"]
+
+        if not stream:
+            stream = p.open(format=pyaudio.paFloat32,
+                            channels=1,
+                            rate=rate,
+                            output=True)
+
+        # Write the audio data to the stream
+        stream.write(buffer)
+
+    stream.stop_stream()
+    stream.close()
+    p.terminate()
+
+asyncio.run(write_stream())
+```
+
+If you are using Jupyter Notebook or JupyterLab, you can use IPython.display.Audio to play the generated audio directly in the notebook.
+Additionally, in these notebook examples we show how to use the client as a context manager (though this is not required).
 
 ```python
-from cartesia.tts import CartesiaTTS
 from IPython.display import Audio
 import io
 import os
+import numpy as np
 
-client = CartesiaTTS(api_key=os.environ.get("CARTESIA_API_KEY"))
-voices = client.get_voices()
-voice = client.get_voice_embedding(voice_id=voices["Graham"]["id"])
-transcript = "Hello! Welcome to Cartesia"
-
-# Create a BytesIO object to store the audio data
-audio_data = io.BytesIO()
+from cartesia.tts import CartesiaTTS
 
-# Generate and stream audio
-for output in client.generate(transcript=transcript, voice=voice, stream=True):
-    buffer = output["audio"]
-    audio_data.write(buffer)
+with CartesiaTTS(api_key=os.environ.get("CARTESIA_API_KEY")) as client:
+    voices = client.get_voices()
+    voice = client.get_voice_embedding(voice_id=voices["Graham"]["id"])
+    transcript = "Hello! Welcome to Cartesia"
+
+    # Create a BytesIO object to store the audio data
+    audio_data = io.BytesIO()
+
+    # Generate and stream audio
+    for output in client.generate(transcript=transcript, voice=voice, stream=True):
+        buffer = output["audio"]
+        audio_data.write(buffer)
 
 # Set the cursor position to the beginning of the BytesIO object
 audio_data.seek(0)
 
 # Create an Audio object from the BytesIO data
 audio = Audio(np.frombuffer(audio_data.read(), dtype=np.float32), rate=output["sampling_rate"])
 
 # Display the Audio object
 display(audio)
 ```
 
-You can also use the async client if you want to make asynchronous API calls. The usage is very similar:
+Below is the same example using the async client:
 ```python
-from cartesia.tts import AsyncCartesiaTTS
 from IPython.display import Audio
 import io
 import os
+import numpy as np
 
-client = AsyncCartesiaTTS(api_key=os.environ.get("CARTESIA_API_KEY"))
-voices = client.get_voices()
-voice = client.get_voice_embedding(voice_id=voices["Graham"]["id"])
-transcript = "Hello! Welcome to Cartesia"
-
-# Create a BytesIO object to store the audio data
-audio_data = io.BytesIO()
+from cartesia.tts import AsyncCartesiaTTS
 
-# Generate and stream audio
-async for output in client.generate(transcript=transcript, voice=voice, stream=True):
-    buffer = output["audio"]
-    audio_data.write(buffer)
+async with AsyncCartesiaTTS(api_key=os.environ.get("CARTESIA_API_KEY")) as client:
+    voices = client.get_voices()
+    voice = client.get_voice_embedding(voice_id=voices["Graham"]["id"])
+    transcript = "Hello! Welcome to Cartesia"
+
+    # Create a BytesIO object to store the audio data
+    audio_data = io.BytesIO()
+
+    # Generate and stream audio
+    async for output in await client.generate(transcript=transcript, voice=voice, stream=True):
+        buffer = output["audio"]
+        audio_data.write(buffer)
 
 # Set the cursor position to the beginning of the BytesIO object
 audio_data.seek(0)
 
 # Create an Audio object from the BytesIO data
 audio = Audio(np.frombuffer(audio_data.read(), dtype=np.float32), rate=output["sampling_rate"])
```

### Comparing `cartesia-0.0.5rc1/setup.py` & `cartesia-0.0.6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -114,16 +114,17 @@
         os.system("git tag v{0}".format(about["__version__"]))
         os.system("git push --tags")
 
         sys.exit()
 
 
 class BumpVersionCommand(Command):
-    """
-    To use: python setup.py bumpversion -v <version>
+    """Bump the version of the package.
+
+    To use: python setup.py bumpversion -v <version>.
 
     This command will push the new version directly and tag it.
 
     Usage:
         python setup.py bumpversion --version=1.0.1
     """
```

### Comparing `cartesia-0.0.5rc1/tests/test_tts.py` & `cartesia-0.0.6/tests/test_tts.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,25 +1,28 @@
 """Test against the production Cartesia TTS API.
 
-This test suite tries to be as general as possible because different keys
-will lead to different results. Therefore, we cannot test for complete correctness
-but rather for general correctness.
+This test suite tries to be as general as possible because different keys will lead to
+different results. Therefore, we cannot test for complete correctness but rather for
+general correctness.
 """
 
+import logging
 import os
 import sys
-import uuid
+from cartesia.tts import DEFAULT_MODEL_ID, AsyncCartesiaTTS, CartesiaTTS, VoiceMetadata
 from typing import AsyncGenerator, Dict, Generator, List
 
 import pytest
 
-sys.path.append(os.path.dirname(os.path.dirname(__file__)))
-from cartesia.tts import DEFAULT_MODEL_ID, AsyncCartesiaTTS, CartesiaTTS, VoiceMetadata
+THISDIR = os.path.dirname(__file__)
+sys.path.insert(0, os.path.dirname(THISDIR))
+
+SAMPLE_VOICE = "Samantha"
 
-SAMPLE_VOICE = "Milo"
+logger = logging.getLogger(__name__)
 
 
 class _Resources:
     def __init__(self, *, client: CartesiaTTS, voices: Dict[str, VoiceMetadata]):
         self.client = client
         self.voices = voices
 
@@ -30,75 +33,88 @@
 
 def create_async_client():
     return AsyncCartesiaTTS(api_key=os.environ.get("CARTESIA_API_KEY"))
 
 
 @pytest.fixture(scope="session")
 def client():
+    logger.info("Creating client")
     return create_client()
 
 
 @pytest.fixture(scope="session")
-def client_with_ws_interrupt():
-    return CartesiaTTS(
-        api_key=os.environ.get("CARTESIA_API_KEY"), experimental_ws_handle_interrupts=True
-    )
-
-
-@pytest.fixture(scope="session")
 def resources(client: CartesiaTTS):
+    logger.info("Creating resources")
     voices = client.get_voices()
     voice_id = voices[SAMPLE_VOICE]["id"]
     voices[SAMPLE_VOICE]["embedding"] = client.get_voice_embedding(voice_id=voice_id)
 
     return _Resources(
         client=client,
         voices=voices,
     )
 
 
 def test_get_voices(client: CartesiaTTS):
+    logger.info("Testing get_voices")
     voices = client.get_voices()
 
     assert isinstance(voices, dict)
     assert all(isinstance(key, str) for key in voices.keys())
     ids = [voice["id"] for voice in voices.values()]
     assert len(ids) == len(set(ids)), "All ids must be unique"
     assert all(
         key == voice["name"] for key, voice in voices.items()
     ), "The key must be the same as the name"
 
 
 def test_get_voice_embedding_from_id(client: CartesiaTTS):
+    logger.info("Testing get_voice_embedding")
     voices = client.get_voices()
     voice_id = voices[SAMPLE_VOICE]["id"]
 
     client.get_voice_embedding(voice_id=voice_id)
 
 
 def test_get_voice_embedding_from_url(client: CartesiaTTS):
     url = "https://youtu.be/g2Z7Ddd573M?si=P8BM_hBqt5P8Ft6I&t=69"
-    _ = client.get_voice_embedding(link=url)
+    logger.info(f"Testing get_voice_embedding from URL {url}")
+    client.get_voice_embedding(link=url)
 
 
 @pytest.mark.parametrize("websocket", [True, False])
 def test_generate(resources: _Resources, websocket: bool):
+    logger.info("Testing generate")
     client = resources.client
     voices = resources.voices
     embedding = voices[SAMPLE_VOICE]["embedding"]
     transcript = "Hello, world!"
 
     output = client.generate(transcript=transcript, voice=embedding, websocket=websocket)
     assert output.keys() == {"audio", "sampling_rate"}
     assert isinstance(output["audio"], bytes)
     assert isinstance(output["sampling_rate"], int)
 
 
+def test_generate_with_model_id(resources: _Resources):
+    logger.info("Testing generate with model_id")
+    client = resources.client
+    voices = resources.voices
+    embedding = voices[SAMPLE_VOICE]["embedding"]
+    transcript = "Hello, world!"
+
+    output = client.generate(transcript=transcript, voice=embedding, model_id=DEFAULT_MODEL_ID)
+    assert output.keys() == {"audio", "sampling_rate"}
+    assert isinstance(output["audio"], bytes)
+    assert isinstance(output["sampling_rate"], int)
+
+
 @pytest.mark.parametrize("websocket", [True, False])
 def test_generate_stream(resources: _Resources, websocket: bool):
+    logger.info("Testing generate stream")
     client = resources.client
     voices = resources.voices
     embedding = voices[SAMPLE_VOICE]["embedding"]
     transcript = "Hello, world!"
 
     generator = client.generate(
         transcript=transcript, voice=embedding, websocket=websocket, stream=True
@@ -108,118 +124,171 @@
     for output in generator:
         assert output.keys() == {"audio", "sampling_rate"}
         assert isinstance(output["audio"], bytes)
         assert isinstance(output["sampling_rate"], int)
 
 
 @pytest.mark.parametrize("websocket", [True, False])
+def test_generate_stream_context_manager(resources: _Resources, websocket: bool):
+    logger.info("Testing generate stream context manager")
+    voices = resources.voices
+    embedding = voices[SAMPLE_VOICE]["embedding"]
+    transcript = "Hello, world!"
+
+    with create_client() as client:
+        generator = client.generate(
+            transcript=transcript, voice=embedding, websocket=websocket, stream=True
+        )
+        assert isinstance(generator, Generator)
+
+        for output in generator:
+            assert output.keys() == {"audio", "sampling_rate"}
+            assert isinstance(output["audio"], bytes)
+            assert isinstance(output["sampling_rate"], int)
+
+
+def test_generate_context_manager_with_err():
+    logger.info("Testing generate context manager with error")
+    websocket = None
+    websocket_was_opened = False
+    try:
+        with create_client() as client:
+            client.refresh_websocket()
+            websocket = client.websocket
+            websocket_was_opened = websocket.socket.fileno() != -1
+            client.generate(
+                transcript=None, voice=None, websocket=True
+            )  # should throw because transcript None
+        raise RuntimeError("Expected AttributeError to be thrown")
+    except AttributeError:
+        pass
+
+    assert websocket_was_opened
+    assert websocket.socket.fileno() == -1  # check socket is now closed
+
+
+@pytest.mark.parametrize("websocket", [True, False])
 @pytest.mark.asyncio
 async def test_async_generate(resources: _Resources, websocket: bool):
+    logger.info("Testing async generate")
     voices = resources.voices
     embedding = voices[SAMPLE_VOICE]["embedding"]
     transcript = "Hello, world!"
 
     async_client = create_async_client()
-    output = await async_client.generate(
-        transcript=transcript, voice=embedding, websocket=websocket
-    )
+    try:
+        output = await async_client.generate(
+            transcript=transcript, voice=embedding, websocket=websocket
+        )
 
-    assert output.keys() == {"audio", "sampling_rate"}
-    assert isinstance(output["audio"], bytes)
-    assert isinstance(output["sampling_rate"], int)
+        assert output.keys() == {"audio", "sampling_rate"}
+        assert isinstance(output["audio"], bytes)
+        assert isinstance(output["sampling_rate"], int)
+    finally:
+        # Close the websocket
+        await async_client.close()
 
 
 @pytest.mark.parametrize("websocket", [True, False])
 @pytest.mark.asyncio
 async def test_async_generate_stream(resources: _Resources, websocket: bool):
+    logger.info(f"Testing async generate stream with websocket={websocket}")
     voices = resources.voices
     embedding = voices[SAMPLE_VOICE]["embedding"]
     transcript = "Hello, world!"
 
     async_client = create_async_client()
 
-    generator = await async_client.generate(transcript=transcript, voice=embedding, stream=True)
-    assert isinstance(generator, AsyncGenerator)
-
-    async for output in generator:
-        assert output.keys() == {"audio", "sampling_rate"}
-        assert isinstance(output["audio"], bytes)
-        assert isinstance(output["sampling_rate"], int)
+    try:
+        generator = await async_client.generate(transcript=transcript, voice=embedding, websocket=websocket, stream=True)
+        assert isinstance(generator, AsyncGenerator)
+        async for output in generator:
+            assert output.keys() == {"audio", "sampling_rate"}
+            assert isinstance(output["audio"], bytes)
+            assert isinstance(output["sampling_rate"], int)
+    finally:
+        # Close the websocket
+        await async_client.close()
 
 
-@pytest.mark.parametrize(
-    "actions",
-    [
-        ["cancel-5", None],
-        ["cancel-5", "cancel-1", None],
-        [None, "cancel-3", None],
-        [None, "cancel-1", "cancel-2"],
-    ],
-)
-def test_generate_stream_interrupt(
-    client_with_ws_interrupt: CartesiaTTS, resources: _Resources, actions: List[str]
-):
-    client = client_with_ws_interrupt
+@pytest.mark.parametrize("websocket", [True, False])
+@pytest.mark.asyncio
+async def test_async_generate_stream_context_manager(resources: _Resources, websocket: bool):
+    logger.info("Testing async generate stream context manager")
     voices = resources.voices
     embedding = voices[SAMPLE_VOICE]["embedding"]
     transcript = "Hello, world!"
 
-    context_ids = [f"test-{uuid.uuid4().hex[:6]}" for _ in range(len(actions))]
-
-    for context_id, action in zip(context_ids, actions):
-        body = dict(transcript=transcript, model_id=DEFAULT_MODEL_ID, voice=embedding)
-
-        # Parse actions to see what we should expect.
-        if action is None:
-            num_turns = None
-        elif "cancel" in action:
-            num_turns = int(action.split("-")[1])
-
-        generator = client._generate_ws(body, context_id=context_id)
-        for idx, response in enumerate(generator):
-            assert response.keys() == {"audio", "sampling_rate", "context_id"}
-            assert response["context_id"] == context_id, (
-                f"Context ID from response ({response['context_id']}) does not match "
-                f"the expected context ID ({context_id})"
-            )
-            if idx + 1 == num_turns:
-                break
+    async with create_async_client() as async_client:
+        generator = await async_client.generate(transcript=transcript, voice=embedding, stream=True)
+        assert isinstance(generator, AsyncGenerator)
+
+        async for output in generator:
+            assert output.keys() == {"audio", "sampling_rate"}
+            assert isinstance(output["audio"], bytes)
+            assert isinstance(output["sampling_rate"], int)
+
+
+@pytest.mark.asyncio
+async def test_generate_async_context_manager_with_err():
+    logger.info("Testing async generate context manager with error")
+    websocket = None
+    websocket_was_opened = False
+    try:
+        async with create_async_client() as async_client:
+            await async_client.refresh_websocket()
+            websocket = async_client.websocket
+            websocket_was_opened = not websocket.closed
+            # below should throw because transcript None
+            await async_client.generate(transcript=None, voice=None, websocket=True)
+        raise RuntimeError("Expected AttributeError to be thrown")
+    except AttributeError:
+        pass
+
+    assert websocket_was_opened
+    assert websocket.closed  # check websocket is now closed
 
 
 @pytest.mark.parametrize("chunk_time", [0.05, 0.6])
 def test_check_inputs_invalid_chunk_time(client: CartesiaTTS, chunk_time):
+    logger.info(f"Testing invalid chunk_time: {chunk_time}")
     with pytest.raises(ValueError, match="`chunk_time` must be between 0.1 and 0.5"):
         client._check_inputs("Test", None, chunk_time)
 
 
 @pytest.mark.parametrize("chunk_time", [0.1, 0.3, 0.5])
 def test_check_inputs_valid_chunk_time(client, chunk_time):
+    logger.info("Testing valid chunk_time: {chunk_time}")
     try:
         client._check_inputs("Test", None, chunk_time)
     except ValueError:
         pytest.fail("Unexpected ValueError raised")
 
 
 def test_check_inputs_duration_less_than_chunk_time(client: CartesiaTTS):
+    logger.info("Testing duration less than chunk_time")
     with pytest.raises(ValueError, match="`duration` must be greater than chunk_time"):
         client._check_inputs("Test", 0.2, 0.3)
 
 
 @pytest.mark.parametrize("duration,chunk_time", [(0.5, 0.2), (1.0, 0.5), (2.0, 0.1)])
 def test_check_inputs_valid_duration_and_chunk_time(client: CartesiaTTS, duration, chunk_time):
+    logger.info(f"Testing valid duration: {duration} and chunk_time: {chunk_time}")
     try:
         client._check_inputs("Test", duration, chunk_time)
     except ValueError:
         pytest.fail("Unexpected ValueError raised")
 
 
 def test_check_inputs_empty_transcript(client: CartesiaTTS):
+    logger.info("Testing empty transcript")
     with pytest.raises(ValueError, match="`transcript` must be non empty"):
         client._check_inputs("", None, None)
 
 
 @pytest.mark.parametrize("transcript", ["Hello", "Test transcript", "Lorem ipsum dolor sit amet"])
 def test_check_inputs_valid_transcript(client: CartesiaTTS, transcript):
+    logger.info(f"Testing valid transcript: {transcript}")
     try:
         client._check_inputs(transcript, None, None)
     except ValueError:
         pytest.fail("Unexpected ValueError raised")
```

