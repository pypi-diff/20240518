# Comparing `tmp/ezlocalai-0.1.8.tar.gz` & `tmp/ezlocalai-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ezlocalai-0.1.8.tar", last modified: Fri Apr 26 19:31:55 2024, max compression
+gzip compressed data, was "ezlocalai-0.1.9.tar", last modified: Mon Apr 29 12:07:16 2024, max compression
```

## Comparing `ezlocalai-0.1.8.tar` & `ezlocalai-0.1.9.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 19:31:55.334488 ezlocalai-0.1.8/
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-26 19:31:51.000000 ezlocalai-0.1.8/.dockerignore
--rw-r--r--   0 runner    (1001) docker     (127)      216 2024-04-26 19:31:51.000000 ezlocalai-0.1.8/.env
--rw-r--r--   0 runner    (1001) docker     (127)      145 2024-04-26 19:31:51.000000 ezlocalai-0.1.8/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     3201 2024-04-26 19:31:51.000000 ezlocalai-0.1.8/Docker.md
--rw-r--r--   0 runner    (1001) docker     (127)      952 2024-04-26 19:31:51.000000 ezlocalai-0.1.8/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-26 19:31:51.000000 ezlocalai-0.1.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-26 19:31:51.000000 ezlocalai-0.1.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     8790 2024-04-26 19:31:55.334488 ezlocalai-0.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    14301 2024-04-26 19:31:51.000000 ezlocalai-0.1.8/Pipes.py
--rw-r--r--   0 runner    (1001) docker     (127)     7719 2024-04-26 19:31:51.000000 ezlocalai-0.1.8/README.md
--rw-r--r--   0 runner    (1001) docker     (127)    10389 2024-04-26 19:31:51.000000 ezlocalai-0.1.8/app.py
--rw-r--r--   0 runner    (1001) docker     (127)      403 2024-04-26 19:31:51.000000 ezlocalai-0.1.8/cuda-requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1321 2024-04-26 19:31:51.000000 ezlocalai-0.1.8/cuda.Dockerfile
--rw-r--r--   0 runner    (1001) docker     (127)      123 2024-04-26 19:31:51.000000 ezlocalai-0.1.8/deepseek.ps1
--rw-r--r--   0 runner    (1001) docker     (127)     1059 2024-04-26 19:31:51.000000 ezlocalai-0.1.8/deepseek.yml
--rw-r--r--   0 runner    (1001) docker     (127)      882 2024-04-26 19:31:51.000000 ezlocalai-0.1.8/dev.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1047 2024-04-26 19:31:51.000000 ezlocalai-0.1.8/docker-compose-cuda.yml
--rw-r--r--   0 runner    (1001) docker     (127)      764 2024-04-26 19:31:51.000000 ezlocalai-0.1.8/docker-compose.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 19:31:55.330488 ezlocalai-0.1.8/ezlocalai/
--rw-r--r--   0 runner    (1001) docker     (127)     5599 2024-04-26 19:31:51.000000 ezlocalai-0.1.8/ezlocalai/CTTS.py
--rw-r--r--   0 runner    (1001) docker     (127)     2730 2024-04-26 19:31:51.000000 ezlocalai-0.1.8/ezlocalai/Embedding.py
--rw-r--r--   0 runner    (1001) docker     (127)      594 2024-04-26 19:31:51.000000 ezlocalai-0.1.8/ezlocalai/Helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1513 2024-04-26 19:31:51.000000 ezlocalai-0.1.8/ezlocalai/IMG.py
--rw-r--r--   0 runner    (1001) docker     (127)    11882 2024-04-26 19:31:51.000000 ezlocalai-0.1.8/ezlocalai/LLM.py
--rw-r--r--   0 runner    (1001) docker     (127)     3313 2024-04-26 19:31:51.000000 ezlocalai-0.1.8/ezlocalai/STT.py
--rw-r--r--   0 runner    (1001) docker     (127)     6753 2024-04-26 19:31:51.000000 ezlocalai-0.1.8/ezlocalai/VLM.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 19:31:51.000000 ezlocalai-0.1.8/ezlocalai/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3262 2024-04-26 19:31:51.000000 ezlocalai-0.1.8/ezlocalai-ngrok.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 19:31:55.334488 ezlocalai-0.1.8/ezlocalai.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     8790 2024-04-26 19:31:55.000000 ezlocalai-0.1.8/ezlocalai.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      618 2024-04-26 19:31:55.000000 ezlocalai-0.1.8/ezlocalai.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 19:31:55.000000 ezlocalai-0.1.8/ezlocalai.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      375 2024-04-26 19:31:55.000000 ezlocalai-0.1.8/ezlocalai.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-26 19:31:55.000000 ezlocalai-0.1.8/ezlocalai.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-26 19:31:51.000000 ezlocalai-0.1.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      374 2024-04-26 19:31:51.000000 ezlocalai-0.1.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-26 19:31:55.334488 ezlocalai-0.1.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      743 2024-04-26 19:31:51.000000 ezlocalai-0.1.8/setup.py
--rw-r--r--   0 runner    (1001) docker     (127)     4377 2024-04-26 19:31:51.000000 ezlocalai-0.1.8/start.ps1
--rw-r--r--   0 runner    (1001) docker     (127)  2999708 2024-04-26 19:31:51.000000 ezlocalai-0.1.8/tests.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     7350 2024-04-26 19:31:51.000000 ezlocalai-0.1.8/ui.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 12:07:16.768087 ezlocalai-0.1.9/
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-29 12:07:12.000000 ezlocalai-0.1.9/.dockerignore
+-rw-r--r--   0 runner    (1001) docker     (127)      263 2024-04-29 12:07:12.000000 ezlocalai-0.1.9/.env
+-rw-r--r--   0 runner    (1001) docker     (127)      145 2024-04-29 12:07:12.000000 ezlocalai-0.1.9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     3201 2024-04-29 12:07:12.000000 ezlocalai-0.1.9/Docker.md
+-rw-r--r--   0 runner    (1001) docker     (127)      952 2024-04-29 12:07:12.000000 ezlocalai-0.1.9/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-29 12:07:12.000000 ezlocalai-0.1.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-29 12:07:12.000000 ezlocalai-0.1.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     8868 2024-04-29 12:07:16.768087 ezlocalai-0.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    14751 2024-04-29 12:07:12.000000 ezlocalai-0.1.9/Pipes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7786 2024-04-29 12:07:12.000000 ezlocalai-0.1.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)    11973 2024-04-29 12:07:12.000000 ezlocalai-0.1.9/app.py
+-rw-r--r--   0 runner    (1001) docker     (127)      403 2024-04-29 12:07:12.000000 ezlocalai-0.1.9/cuda-requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1321 2024-04-29 12:07:12.000000 ezlocalai-0.1.9/cuda.Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-04-29 12:07:12.000000 ezlocalai-0.1.9/deepseek.ps1
+-rw-r--r--   0 runner    (1001) docker     (127)     1059 2024-04-29 12:07:12.000000 ezlocalai-0.1.9/deepseek.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      882 2024-04-29 12:07:12.000000 ezlocalai-0.1.9/dev.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1047 2024-04-29 12:07:12.000000 ezlocalai-0.1.9/docker-compose-cuda.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      764 2024-04-29 12:07:12.000000 ezlocalai-0.1.9/docker-compose.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 12:07:16.768087 ezlocalai-0.1.9/ezlocalai/
+-rw-r--r--   0 runner    (1001) docker     (127)     5599 2024-04-29 12:07:12.000000 ezlocalai-0.1.9/ezlocalai/CTTS.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2730 2024-04-29 12:07:12.000000 ezlocalai-0.1.9/ezlocalai/Embedding.py
+-rw-r--r--   0 runner    (1001) docker     (127)      594 2024-04-29 12:07:12.000000 ezlocalai-0.1.9/ezlocalai/Helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2099 2024-04-29 12:07:12.000000 ezlocalai-0.1.9/ezlocalai/IMG.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11882 2024-04-29 12:07:12.000000 ezlocalai-0.1.9/ezlocalai/LLM.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3313 2024-04-29 12:07:12.000000 ezlocalai-0.1.9/ezlocalai/STT.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6753 2024-04-29 12:07:12.000000 ezlocalai-0.1.9/ezlocalai/VLM.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 12:07:12.000000 ezlocalai-0.1.9/ezlocalai/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3486 2024-04-29 12:07:12.000000 ezlocalai-0.1.9/ezlocalai-ngrok.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 12:07:16.768087 ezlocalai-0.1.9/ezlocalai.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8868 2024-04-29 12:07:16.000000 ezlocalai-0.1.9/ezlocalai.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      618 2024-04-29 12:07:16.000000 ezlocalai-0.1.9/ezlocalai.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 12:07:16.000000 ezlocalai-0.1.9/ezlocalai.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      375 2024-04-29 12:07:16.000000 ezlocalai-0.1.9/ezlocalai.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-29 12:07:16.000000 ezlocalai-0.1.9/ezlocalai.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-29 12:07:12.000000 ezlocalai-0.1.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      374 2024-04-29 12:07:12.000000 ezlocalai-0.1.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-29 12:07:16.768087 ezlocalai-0.1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      754 2024-04-29 12:07:12.000000 ezlocalai-0.1.9/setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4377 2024-04-29 12:07:12.000000 ezlocalai-0.1.9/start.ps1
+-rw-r--r--   0 runner    (1001) docker     (127)  3000347 2024-04-29 12:07:12.000000 ezlocalai-0.1.9/tests.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     7350 2024-04-29 12:07:12.000000 ezlocalai-0.1.9/ui.py
```

### Comparing `ezlocalai-0.1.8/Docker.md` & `ezlocalai-0.1.9/Docker.md`

 * *Files identical despite different names*

### Comparing `ezlocalai-0.1.8/Dockerfile` & `ezlocalai-0.1.9/Dockerfile`

 * *Files identical despite different names*

### Comparing `ezlocalai-0.1.8/LICENSE` & `ezlocalai-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `ezlocalai-0.1.8/PKG-INFO` & `ezlocalai-0.1.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: ezlocalai
-Version: 0.1.8
-Summary: ezlocalai is an easy to set up local artificial intelligence server with OpenAI Style Endpoints.
+Version: 0.1.9
+Summary: ezlocalai is an easy to set up local multimodal artificial intelligence server with OpenAI Style Endpoints.
 Author: Josh XT
 Author-email: josh@devxt.com
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: fastapi
 Requires-Dist: uvicorn
@@ -110,15 +110,15 @@
 docker-compose up
 ```
 
 ## OpenAI Style Endpoint Usage
 
 OpenAI Style endpoints available at `http://<YOUR LOCAL IP ADDRESS>:8091/v1/` by default. Documentation can be accessed at that <http://localhost:8091> when the server is running.
 
-For examples on how to use the server to communicate with the models, see the [Examples Jupyter Notebook](tests/tests.ipynb) once the server is running.
+For examples on how to use the server to communicate with the models, see the [Examples Jupyter Notebook](tests.ipynb) once the server is running. We also have an [example to use in Google Colab](ezlocalai-ngrok.ipynb).
 
 ## Demo UI
 
 You can access the basic demo UI at <http://localhost:8502>, or your local IP address with port 8502.
 
 ## Workflow
```

### Comparing `ezlocalai-0.1.8/Pipes.py` & `ezlocalai-0.1.9/Pipes.py`

 * *Files 6% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 
 from ezlocalai.VLM import VLM
 
 
 class Pipes:
     def __init__(self):
         load_dotenv()
+        global img_import_success
         DEFAULT_MODEL = os.getenv("DEFAULT_MODEL", "TheBloke/phi-2-dpo-GGUF")
         self.current_llm = DEFAULT_MODEL if DEFAULT_MODEL else "TheBloke/phi-2-dpo-GGUF"
         logging.info(f"[LLM] {self.current_llm} model loading. Please wait...")
         self.llm = LLM(model=self.current_llm)
         logging.info(f"[LLM] {self.current_llm} model loaded successfully.")
         self.embedder = Embedding()
         self.current_vlm = os.getenv("VISION_MODEL", "")
@@ -37,26 +38,14 @@
             try:
                 self.vlm = VLM(model=self.current_vlm)
             except Exception as e:
                 logging.error(f"[VLM] Failed to load the model: {e}")
                 self.vlm = None
         if self.vlm is not None:
             logging.info(f"[ezlocalai] Vision is enabled with {self.current_vlm}.")
-        self.img_enabled = os.getenv("IMG_ENABLED", "false").lower() == "true"
-        self.img = None
-        if self.img_enabled and img_import_success:
-            logging.info(f"[IMG] Image generation is enabled.")
-            SD_MODEL = os.getenv("SD_MODEL", "stabilityai/sdxl-turbo")
-            logging.info(f"[IMG] sdxl-turbo model loading. Please wait...")
-            try:
-                self.img = IMG(model=SD_MODEL)
-            except Exception as e:
-                logging.error(f"[IMG] Failed to load the model: {e}")
-                self.img = None
-            logging.info(f"[IMG] sdxl-turbo model loaded successfully.")
         logging.info(f"[CTTS] xttsv2_2.0.2 model loading. Please wait...")
         self.ctts = CTTS()
         logging.info(f"[CTTS] xttsv2_2.0.2 model loaded successfully.")
         self.current_stt = os.getenv("WHISPER_MODEL", "base")
         logging.info(f"[STT] {self.current_stt} model loading. Please wait...")
         self.stt = STT(model=self.current_stt)
         logging.info(f"[STT] {self.current_stt} model loaded successfully.")
@@ -67,14 +56,27 @@
         if NGROK_TOKEN:
             ngrok.set_auth_token(NGROK_TOKEN)
             public_url = ngrok.connect(8091)
             logging.info(f"[ngrok] Public Tunnel: {public_url.public_url}")
             self.local_uri = public_url.public_url
         else:
             self.local_uri = os.environ.get("EZLOCALAI_URL", "http://localhost:8091")
+        self.img_enabled = os.getenv("IMG_ENABLED", "false").lower() == "true"
+        self.img = None
+        if img_import_success:
+            logging.info(f"[IMG] Image generation is enabled.")
+            SD_MODEL = os.getenv("SD_MODEL", "")  # stabilityai/sdxl-turbo
+            if SD_MODEL:
+                logging.info(f"[IMG] {SD_MODEL} model loading. Please wait...")
+                try:
+                    self.img = IMG(model=SD_MODEL, local_uri=self.local_uri)
+                except Exception as e:
+                    logging.error(f"[IMG] Failed to load the model: {e}")
+                    self.img = None
+            logging.info(f"[IMG] {SD_MODEL} model loaded successfully.")
 
     async def pdf_to_audio(self, title, voice, pdf, chunk_size=200):
         filename = f"{title}.pdf"
         file_path = os.path.join(os.getcwd(), "outputs", filename)
         pdf = pdf.split(",")[1]
         pdf = base64.b64decode(pdf)
         with open(file_path, "wb") as pdf_file:
@@ -98,14 +100,25 @@
         audio = audio.split(",")[1]
         audio = base64.b64decode(audio)
         text = self.stt.transcribe_audio(base64_audio=audio, audio_format=audio_format)
         return await self.ctts.generate(
             text=text, voice=voice, local_uri=self.local_uri
         )
 
+    async def generate_image(self, prompt, response_format="url", size="512x512"):
+        if self.img:
+            self.img.local_uri = self.local_uri if response_format == "url" else None
+            new_image = self.img.generate(
+                prompt=prompt,
+                size=size,
+            )
+            self.img.local_uri = self.local_uri
+            return new_image
+        return ""
+
     async def get_response(self, data, completion_type="chat"):
         data["local_uri"] = self.local_uri
         images = []
         if "messages" in data:
             if isinstance(data["messages"][-1]["content"], list):
                 messages = data["messages"][-1]["content"]
                 for message in messages:
@@ -189,15 +202,15 @@
         else:
             response = self.llm.completion(**data)
         generated_image = None
         if "temperature" not in data:
             data["temperature"] = 0.5
         if "top_p" not in data:
             data["top_p"] = 0.9
-        if self.img and img_import_success:
+        if self.img_enabled and img_import_success and self.img:
             user_message = (
                 data["messages"][-1]["content"]
                 if completion_type == "chat"
                 else data["prompt"]
             )
             if isinstance(user_message, list):
                 user_message = prompt
@@ -244,17 +257,15 @@
                     f"[IMG] Image generation response: {image_generation_prompt}"
                 )
                 if "```markdown" in image_generation_prompt:
                     image_generation_prompt = image_generation_prompt.split(
                         "```markdown"
                     )[1]
                     image_generation_prompt = image_generation_prompt.split("```")[0]
-                generated_image = self.img.generate(
-                    prompt=image_generation_prompt, local_uri=self.local_uri
-                )
+                generated_image = self.img.generate(prompt=image_generation_prompt)
         audio_response = None
         if "voice" in data:
             text_response = (
                 response["choices"][0]["text"]
                 if completion_type != "chat"
                 else response["choices"][0]["message"]["content"]
             )
```

### Comparing `ezlocalai-0.1.8/README.md` & `ezlocalai-0.1.9/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -73,15 +73,15 @@
 docker-compose up
 ```
 
 ## OpenAI Style Endpoint Usage
 
 OpenAI Style endpoints available at `http://<YOUR LOCAL IP ADDRESS>:8091/v1/` by default. Documentation can be accessed at that <http://localhost:8091> when the server is running.
 
-For examples on how to use the server to communicate with the models, see the [Examples Jupyter Notebook](tests/tests.ipynb) once the server is running.
+For examples on how to use the server to communicate with the models, see the [Examples Jupyter Notebook](tests.ipynb) once the server is running. We also have an [example to use in Google Colab](ezlocalai-ngrok.ipynb).
 
 ## Demo UI
 
 You can access the basic demo UI at <http://localhost:8502>, or your local IP address with port 8502.
 
 ## Workflow
```

### Comparing `ezlocalai-0.1.8/app.py` & `ezlocalai-0.1.9/app.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 from pydantic import BaseModel
 from typing import List, Dict, Union, Optional
 from Pipes import Pipes
 import base64
 import os
 import logging
 import uuid
+import time
 from dotenv import load_dotenv
 
 load_dotenv()
 DEFAULT_MODEL = os.getenv("DEFAULT_MODEL", "TheBloke/phi-2-dpo-GGUF")
 WHISPER_MODEL = os.getenv("WHISPER_MODEL", "base")
 logging.basicConfig(
     level=os.environ.get("LOGLEVEL", "INFO"),
@@ -352,7 +353,62 @@
         while os.path.exists(file_path):
             file_path = os.path.join(os.getcwd(), "voices", f"{voice}-{i}.wav")
             voice_name = f"{voice}-{i}"
             i += 1
     with open(file_path, "wb") as audio_file:
         audio_file.write(await file.read())
     return {"detail": f"Voice {voice_name} has been uploaded."}
+
+
+# Image Generation endpoint
+# https://platform.openai.com/docs/api-reference/images
+
+
+class ImageCreation(BaseModel):
+    prompt: str
+    model: Optional[str] = "stabilityai/sdxl-turbo"
+    n: Optional[int] = 1
+    size: Optional[str] = "512x512"
+    quality: Optional[str] = "hd"
+    response_format: Optional[str] = "url"
+    style: Optional[str] = "natural"
+
+
+@app.post(
+    "/v1/images/generations",
+    tags=["Images"],
+    dependencies=[Depends(verify_api_key)],
+)
+async def generate_image(
+    image_creation: ImageCreation,
+    user: str = Depends(verify_api_key),
+):
+    images = []
+    if int(image_creation.n) > 1:
+        for i in range(image_creation.n):
+            image = await pipe.generate_image(
+                prompt=image_creation.prompt,
+                response_format=image_creation.response_format,
+                size=image_creation.size,
+            )
+            if image_creation.response_format == "url":
+                images.append({"url": image})
+            else:
+                images.append({"b64_json": image})
+        return {
+            "created": int(time.time()),
+            "data": images,
+        }
+    image = await pipe.generate_image(
+        prompt=image_creation.prompt,
+        response_format=image_creation.response_format,
+        size=image_creation.size,
+    )
+    if image_creation.response_format == "url":
+        return {
+            "created": int(time.time()),
+            "data": [{"url": image}],
+        }
+    return {
+        "created": int(time.time()),
+        "data": [{"b64_json": image}],
+    }
```

### Comparing `ezlocalai-0.1.8/cuda.Dockerfile` & `ezlocalai-0.1.9/cuda.Dockerfile`

 * *Files identical despite different names*

### Comparing `ezlocalai-0.1.8/deepseek.yml` & `ezlocalai-0.1.9/deepseek.yml`

 * *Files identical despite different names*

### Comparing `ezlocalai-0.1.8/dev.yml` & `ezlocalai-0.1.9/dev.yml`

 * *Files identical despite different names*

### Comparing `ezlocalai-0.1.8/docker-compose-cuda.yml` & `ezlocalai-0.1.9/docker-compose-cuda.yml`

 * *Files identical despite different names*

### Comparing `ezlocalai-0.1.8/docker-compose.yml` & `ezlocalai-0.1.9/docker-compose.yml`

 * *Files identical despite different names*

### Comparing `ezlocalai-0.1.8/ezlocalai/CTTS.py` & `ezlocalai-0.1.9/ezlocalai/CTTS.py`

 * *Files identical despite different names*

### Comparing `ezlocalai-0.1.8/ezlocalai/Embedding.py` & `ezlocalai-0.1.9/ezlocalai/Embedding.py`

 * *Files identical despite different names*

### Comparing `ezlocalai-0.1.8/ezlocalai/Helpers.py` & `ezlocalai-0.1.9/ezlocalai/Helpers.py`

 * *Files identical despite different names*

### Comparing `ezlocalai-0.1.8/ezlocalai/IMG.py` & `ezlocalai-0.1.9/ezlocalai/IMG.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,53 +1,69 @@
 import logging
 import uuid
 import torch
+from PIL import Image
 
 try:
-    from diffusers import DiffusionPipeline
+    from diffusers import DiffusionPipeline, LCMScheduler
 
     import_success = True
 except ImportError:
     logging.error(
         "Failed to import diffusers. Please install diffusers using 'pip install diffusers'"
     )
     import_success = False
 
 
 class IMG:
-    def __init__(self, model="stabilityai/sdxl-turbo"):
+    def __init__(
+        self,
+        model="stabilityai/sdxl-turbo",
+        device="cpu",
+        local_uri=None,
+    ):
         global import_success
+        self.local_uri = local_uri
         if import_success:
-            device = "cuda" if torch.cuda.is_available() else "cpu"
             pipe = DiffusionPipeline.from_pretrained(
                 model,
                 cache_dir="models",
-                torch_dtype=torch.float16,
-                variant="fp16",
+                torch_dtype=torch.float32,
+                scheduler=LCMScheduler(beta_start=0.001, beta_end=0.01),
             ).to(device)
             self.pipe = pipe
+            self.pipe.enable_attention_slicing()
             self.pipe.safety_checker = None
         else:
             self.pipe = None
 
     def generate(
         self,
         prompt,
         negative_prompt="low resolution, grainy, distorted",
         num_inference_steps=1,
         guidance_scale=0.0,
-        local_uri=None,
+        size="512x512",
     ):
         new_file_name = f"outputs/{uuid.uuid4()}.png"
         if self.pipe:
+            generator = torch.Generator(device="cpu").manual_seed(0)
             new_image = self.pipe(
                 prompt=prompt,
                 negative_prompt=negative_prompt,
                 num_inference_steps=num_inference_steps,
                 guidance_scale=guidance_scale,
+                generator=generator,
             ).images[0]
-            new_image.save(new_file_name)
-            if local_uri:
-                return f"{local_uri}/{new_file_name}"
-            return new_image
+            width, height = map(int, size.split("x"))
+            if width != 512 and height != 512:
+                upscaled_image = new_image.resize(
+                    (width, height), resample=Image.LANCZOS
+                )
+                upscaled_image.save(new_file_name)
+            else:
+                new_image.save(new_file_name)
+            if self.local_uri:
+                return f"{self.local_uri}/{new_file_name}"
+            return upscaled_image
         else:
             return None
```

### Comparing `ezlocalai-0.1.8/ezlocalai/LLM.py` & `ezlocalai-0.1.9/ezlocalai/LLM.py`

 * *Files identical despite different names*

### Comparing `ezlocalai-0.1.8/ezlocalai/STT.py` & `ezlocalai-0.1.9/ezlocalai/STT.py`

 * *Files identical despite different names*

### Comparing `ezlocalai-0.1.8/ezlocalai/VLM.py` & `ezlocalai-0.1.9/ezlocalai/VLM.py`

 * *Files identical despite different names*

### Comparing `ezlocalai-0.1.8/ezlocalai-ngrok.ipynb` & `ezlocalai-0.1.9/ezlocalai-ngrok.ipynb`

 * *Files 12% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9969429905582923%*

 * *Differences: {"'cells'": '{1: {\'source\': {insert: [(3, \'!CMAKE_ARGS="-DLLAMA_CUDA=on" FORCE_CMAKE=1 pip '*

 * *            'install llama-cpp-python\\n\')], delete: [3]}}, 2: {\'source\': {insert: [(6, "Set '*

 * *            'the `LLM_TO_USE` with the name of the model from the models list or from the [Hugging '*

 * *            'Face model directory of GGUF Quantized '*

 * *            "Models](https://huggingface.co/models?search=GGUF). You won't have to download the "*

 * *            'model, just enter its path. We will use `MaziyarPana […]*

```diff
@@ -18,42 +18,42 @@
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "!apt install -y portaudio19-dev ffmpeg libportaudio2 libasound-dev\n",
                 "!pip install -qq scipy ftfy accelerate fastapi uvicorn pydantic requests tiktoken python-dotenv beautifulsoup4 faster-whisper pydub ffmpeg TTS sounddevice pyaudio webrtcvad pyngrok pdfplumber spacy python-multipart\n",
                 "!pip install -qq diffusers[\"torch\"] transformers torch torchvision torchaudio\n",
-                "!CMAKE_ARGS=\"-DLLAMA_CUBLAS=on\" FORCE_CMAKE=1 pip install llama-cpp-python\n",
+                "!CMAKE_ARGS=\"-DLLAMA_CUDA=on\" FORCE_CMAKE=1 pip install llama-cpp-python\n",
                 "!rm -rf sample_data .config\n",
                 "!git clone https://github.com/DevXT-LLC/ezlocalai ."
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "## Start the server\n",
                 "\n",
                 "Set the `NGROK_TOKEN` to use NGROK to expose your ezlocalai server to the public with as simple as an API key. [Get your free NGROK_TOKEN here.](https://dashboard.ngrok.com/get-started/your-authtoken)\n",
                 "\n",
                 "You can see the ngrok URL in the cell output after running the cell.\n",
                 "\n",
-                "Set the `LLM_TO_USE` with the name of the model from the models list. We will use `Mistral-7B-Instruct-v0.2` for this example since it is a smaller model that can still be useful.\n"
+                "Set the `LLM_TO_USE` with the name of the model from the models list or from the [Hugging Face model directory of GGUF Quantized Models](https://huggingface.co/models?search=GGUF). You won't have to download the model, just enter its path. We will use `MaziyarPanahi/Meta-Llama-3-8B-Instruct-GGUF` for this example since it is a smaller model that can still be useful.\n"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "LLM_TO_USE = \"TheBloke/Mistral-7B-Instruct-v0.2-GGUF\"\n",
+                "LLM_TO_USE = \"MaziyarPanahi/Meta-Llama-3-8B-Instruct-GGUF\"\n",
                 "VISION_MODEL = \"deepseek-ai/deepseek-vl-1.3b-chat\"\n",
-                "GPU_LAYERS = 10\n",
-                "LLM_MAX_TOKENS = 16384\n",
+                "GPU_LAYERS = 20\n",
+                "LLM_MAX_TOKENS = 8192\n",
                 "\n",
                 "# Add your NGROK_TOKEN to your colab secrets if using Google Colab (Key logo on the left)\n",
                 "try:\n",
                 "    from google.colab import userdata\n",
                 "    NGROK_TOKEN = userdata.get('NGROK_TOKEN')\n",
                 "    if not NGROK_TOKEN:\n",
                 "        raise\n",
@@ -63,15 +63,15 @@
                 "if NGROK_TOKEN != \"Enter your ngrok token here\":\n",
                 "    with open('.env', 'r') as file:\n",
                 "        filedata = file.read()\n",
                 "    filedata = filedata.replace('NGROK_TOKEN=\\n', f'NGROK_TOKEN={NGROK_TOKEN}\\n')\n",
                 "    filedata = filedata.replace('DEFAULT_MODEL=TheBloke/phi-2-dpo-GGUF', f'DEFAULT_MODEL={LLM_TO_USE}')\n",
                 "    filedata = filedata.replace('GPU_LAYERS=0', f'GPU_LAYERS={GPU_LAYERS}')\n",
                 "    filedata = filedata.replace('LLM_MAX_TOKENS=0', f'LLM_MAX_TOKENS={LLM_MAX_TOKENS}')\n",
-                "    filedata = filedata.replace('VISION_MODEL=', f'VISION_MODEL={VISION_MODEL}')\n",
+                "    filedata = filedata.replace('VISION_MODEL=deepseek-ai/deepseek-vl-1.3b-chat', f'VISION_MODEL={VISION_MODEL}')\n",
                 "    with open('.env', 'w') as file:\n",
                 "        file.write(filedata)\n",
                 "!uvicorn app:app --host 0.0.0.0 --port 8091 --workers 1 --proxy-headers"
             ]
         }
     ],
     "metadata": {
```

### Comparing `ezlocalai-0.1.8/ezlocalai.egg-info/PKG-INFO` & `ezlocalai-0.1.9/ezlocalai.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: ezlocalai
-Version: 0.1.8
-Summary: ezlocalai is an easy to set up local artificial intelligence server with OpenAI Style Endpoints.
+Version: 0.1.9
+Summary: ezlocalai is an easy to set up local multimodal artificial intelligence server with OpenAI Style Endpoints.
 Author: Josh XT
 Author-email: josh@devxt.com
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: fastapi
 Requires-Dist: uvicorn
@@ -110,15 +110,15 @@
 docker-compose up
 ```
 
 ## OpenAI Style Endpoint Usage
 
 OpenAI Style endpoints available at `http://<YOUR LOCAL IP ADDRESS>:8091/v1/` by default. Documentation can be accessed at that <http://localhost:8091> when the server is running.
 
-For examples on how to use the server to communicate with the models, see the [Examples Jupyter Notebook](tests/tests.ipynb) once the server is running.
+For examples on how to use the server to communicate with the models, see the [Examples Jupyter Notebook](tests.ipynb) once the server is running. We also have an [example to use in Google Colab](ezlocalai-ngrok.ipynb).
 
 ## Demo UI
 
 You can access the basic demo UI at <http://localhost:8502>, or your local IP address with port 8502.
 
 ## Workflow
```

### Comparing `ezlocalai-0.1.8/ezlocalai.egg-info/SOURCES.txt` & `ezlocalai-0.1.9/ezlocalai.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ezlocalai-0.1.8/setup.py` & `ezlocalai-0.1.9/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -6,16 +6,16 @@
     long_description = f.read()
 
 with open(os.path.join(this_directory, "requirements.txt")) as f:
     requirements = f.read().splitlines()
 
 setup(
     name="ezlocalai",
-    version="0.1.8",
-    description="ezlocalai is an easy to set up local artificial intelligence server with OpenAI Style Endpoints.",
+    version="0.1.9",
+    description="ezlocalai is an easy to set up local multimodal artificial intelligence server with OpenAI Style Endpoints.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="Josh XT",
     author_email="josh@devxt.com",
     packages=find_packages(),
     python_requires=">=3.10",
     install_requires=requirements,
```

### Comparing `ezlocalai-0.1.8/start.ps1` & `ezlocalai-0.1.9/start.ps1`

 * *Files identical despite different names*

### Comparing `ezlocalai-0.1.8/tests.ipynb` & `ezlocalai-0.1.9/tests.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9895833333333333%*

 * *Differences: {"'cells'": "{insert: [(22, OrderedDict([('cell_type', 'markdown'), ('metadata', OrderedDict()), "*

 * *            "('source', ['## Generate an Image\\n'])])), (23, OrderedDict([('cell_type', 'code'), "*

 * *            "('execution_count', None), ('metadata', OrderedDict()), ('outputs', []), ('source', "*

 * *            '[\'prompt = "Generate an image of a cat."\\n\', \'response = '*

 * *            "openai.images.generate(\\n', '    prompt=prompt,\\n', '    "*

 * *            'model="stabilityai/sdxl-turbo",\\n\', \'    n=1,\\n […]*

```diff
@@ -527,14 +527,39 @@
                 "        \"voice\": \"DukeNukem\",\n",
                 "    },\n",
                 ")\n",
                 "\n",
                 "response_text = completion.choices[0].text\n",
                 "display_content(response_text)"
             ]
+        },
+        {
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
+                "## Generate an Image\n"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "prompt = \"Generate an image of a cat.\"\n",
+                "response = openai.images.generate(\n",
+                "    prompt=prompt,\n",
+                "    model=\"stabilityai/sdxl-turbo\",\n",
+                "    n=1,\n",
+                "    size=\"512x512\",\n",
+                "    response_format=\"url\",\n",
+                ")\n",
+                "image = response.data[0].url\n",
+                "display_content(image)"
+            ]
         }
     ],
     "metadata": {
         "kernelspec": {
             "display_name": "Python 3",
             "language": "python",
             "name": "python3"
```

### Comparing `ezlocalai-0.1.8/ui.py` & `ezlocalai-0.1.9/ui.py`

 * *Files identical despite different names*

