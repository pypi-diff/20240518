# Comparing `tmp/lollms_client-0.5.9.tar.gz` & `tmp/lollms_client-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lollms_client-0.5.9.tar", last modified: Wed May 15 23:09:24 2024, max compression
+gzip compressed data, was "lollms_client-0.6.0.tar", last modified: Fri May 17 23:59:03 2024, max compression
```

## Comparing `lollms_client-0.5.9.tar` & `lollms_client-0.6.0.tar`

### file list

```diff
@@ -1,23 +1,24 @@
-drwxrwxrwx   0        0        0        0 2024-05-15 23:09:24.113317 lollms_client-0.5.9/
--rw-rw-rw-   0        0        0    11558 2024-03-30 19:02:48.000000 lollms_client-0.5.9/LICENSE
--rw-rw-rw-   0        0        0     3258 2024-05-15 23:09:24.112806 lollms_client-0.5.9/PKG-INFO
--rw-rw-rw-   0        0        0     2780 2024-04-08 23:28:01.000000 lollms_client-0.5.9/README.md
-drwxrwxrwx   0        0        0        0 2024-05-15 23:09:24.096698 lollms_client-0.5.9/lollms_client/
--rw-rw-rw-   0        0        0      452 2024-05-15 22:53:01.000000 lollms_client-0.5.9/lollms_client/__init__.py
--rw-rw-rw-   0        0        0    21876 2024-03-20 22:06:25.000000 lollms_client-0.5.9/lollms_client/lollms_config.py
--rw-rw-rw-   0        0        0    20023 2024-05-07 23:05:45.000000 lollms_client-0.5.9/lollms_client/lollms_core.py
--rw-rw-rw-   0        0        0     2073 2024-04-27 17:07:34.000000 lollms_client-0.5.9/lollms_client/lollms_discussion.py
--rw-rw-rw-   0        0        0    20548 2024-04-27 23:24:03.000000 lollms_client-0.5.9/lollms_client/lollms_personality.py
--rw-rw-rw-   0        0        0    65331 2024-04-27 15:52:23.000000 lollms_client-0.5.9/lollms_client/lollms_personality_worker.py
--rw-rw-rw-   0        0        0    18863 2024-04-29 23:43:11.000000 lollms_client-0.5.9/lollms_client/lollms_tasks.py
--rw-rw-rw-   0        0        0     2170 2024-04-29 23:40:27.000000 lollms_client-0.5.9/lollms_client/lollms_types.py
--rw-rw-rw-   0        0        0     2087 2024-04-27 16:48:27.000000 lollms_client-0.5.9/lollms_client/lollms_utilities.py
--rw-rw-rw-   0        0        0     1144 2024-05-15 23:00:53.000000 lollms_client-0.5.9/lollms_client/lollms_xtts.py
-drwxrwxrwx   0        0        0        0 2024-05-15 23:09:24.112315 lollms_client-0.5.9/lollms_client.egg-info/
--rw-rw-rw-   0        0        0     3258 2024-05-15 23:09:23.000000 lollms_client-0.5.9/lollms_client.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      533 2024-05-15 23:09:24.000000 lollms_client-0.5.9/lollms_client.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-15 23:09:23.000000 lollms_client-0.5.9/lollms_client.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2024-05-15 23:09:23.000000 lollms_client-0.5.9/lollms_client.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2024-05-15 23:09:23.000000 lollms_client-0.5.9/lollms_client.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-15 23:09:24.114317 lollms_client-0.5.9/setup.cfg
--rw-rw-rw-   0        0        0      814 2024-05-15 23:09:18.000000 lollms_client-0.5.9/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-17 23:59:03.720614 lollms_client-0.6.0/
+-rw-rw-rw-   0        0        0    11558 2024-03-30 19:02:48.000000 lollms_client-0.6.0/LICENSE
+-rw-rw-rw-   0        0        0     3258 2024-05-17 23:59:03.719613 lollms_client-0.6.0/PKG-INFO
+-rw-rw-rw-   0        0        0     2780 2024-04-08 23:28:01.000000 lollms_client-0.6.0/README.md
+drwxrwxrwx   0        0        0        0 2024-05-17 23:59:03.682445 lollms_client-0.6.0/lollms_client/
+-rw-rw-rw-   0        0        0      518 2024-05-17 22:54:10.000000 lollms_client-0.6.0/lollms_client/__init__.py
+-rw-rw-rw-   0        0        0    21876 2024-03-20 22:06:25.000000 lollms_client-0.6.0/lollms_client/lollms_config.py
+-rw-rw-rw-   0        0        0    25190 2024-05-17 23:58:03.000000 lollms_client-0.6.0/lollms_client/lollms_core.py
+-rw-rw-rw-   0        0        0     2073 2024-04-27 17:07:34.000000 lollms_client-0.6.0/lollms_client/lollms_discussion.py
+-rw-rw-rw-   0        0        0     3594 2024-05-17 23:39:04.000000 lollms_client-0.6.0/lollms_client/lollms_functions.py
+-rw-rw-rw-   0        0        0    20548 2024-04-27 23:24:03.000000 lollms_client-0.6.0/lollms_client/lollms_personality.py
+-rw-rw-rw-   0        0        0    65331 2024-04-27 15:52:23.000000 lollms_client-0.6.0/lollms_client/lollms_personality_worker.py
+-rw-rw-rw-   0        0        0    36906 2024-05-17 23:52:05.000000 lollms_client-0.6.0/lollms_client/lollms_tasks.py
+-rw-rw-rw-   0        0        0     2170 2024-04-29 23:40:27.000000 lollms_client-0.6.0/lollms_client/lollms_types.py
+-rw-rw-rw-   0        0        0     6171 2024-05-17 21:54:56.000000 lollms_client-0.6.0/lollms_client/lollms_utilities.py
+-rw-rw-rw-   0        0        0     1571 2024-05-17 22:12:33.000000 lollms_client-0.6.0/lollms_client/lollms_xtts.py
+drwxrwxrwx   0        0        0        0 2024-05-17 23:59:03.717612 lollms_client-0.6.0/lollms_client.egg-info/
+-rw-rw-rw-   0        0        0     3258 2024-05-17 23:59:03.000000 lollms_client-0.6.0/lollms_client.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      567 2024-05-17 23:59:03.000000 lollms_client-0.6.0/lollms_client.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-17 23:59:03.000000 lollms_client-0.6.0/lollms_client.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2024-05-17 23:59:03.000000 lollms_client-0.6.0/lollms_client.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2024-05-17 23:59:03.000000 lollms_client-0.6.0/lollms_client.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-17 23:59:03.720614 lollms_client-0.6.0/setup.cfg
+-rw-rw-rw-   0        0        0      814 2024-05-17 23:45:03.000000 lollms_client-0.6.0/setup.py
```

### Comparing `lollms_client-0.5.9/LICENSE` & `lollms_client-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `lollms_client-0.5.9/PKG-INFO` & `lollms_client-0.6.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lollms_client
-Version: 0.5.9
+Version: 0.6.0
 Summary: A client library for LoLLMs generate endpoint
 Home-page: https://github.com/ParisNeo/lollms_client
 Author: ParisNeo
 Author-email: parisneoai@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `lollms_client-0.5.9/README.md` & `lollms_client-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `lollms_client-0.5.9/lollms_client/lollms_config.py` & `lollms_client-0.6.0/lollms_client/lollms_config.py`

 * *Files identical despite different names*

### Comparing `lollms_client-0.5.9/lollms_client/lollms_core.py` & `lollms_client-0.6.0/lollms_client/lollms_core.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import requests
 from ascii_colors import ASCIIColors
 from lollms_client.lollms_types import MSG_TYPE
 import json
 from enum import Enum
 import tiktoken
+import base64
 
 class ELF_GENERATION_FORMAT(Enum):
     LOLLMS = 0
     OPENAI = 1
     OLLAMA = 2
     LITELLM = 2
 
@@ -78,14 +79,26 @@
 
         Returns:
             str: The detokenized text as a string.
         """
         text = self.tokenizer.decode(tokens_list)
 
         return text
+    
+    
+    def generate_with_images(self, prompt, images, n_predict=None, stream=False, temperature=0.1, top_k=50, top_p=0.95, repeat_penalty=0.8, repeat_last_n=40, seed=None, n_threads=8, service_key:str="", streaming_callback=None):
+        if self.default_generation_mode == ELF_GENERATION_FORMAT.LOLLMS:
+            return self.lollms_generate_with_images(prompt, images, self.host_address, self.model_name, -1, n_predict, stream, temperature, top_k, top_p, repeat_penalty, repeat_last_n, seed, n_threads, service_key, streaming_callback)
+        elif self.default_generation_mode == ELF_GENERATION_FORMAT.OPENAI:
+            return # To be implemented #self.openai_generate_with_images(prompt, self.host_address, self.model_name, -1, n_predict, stream, temperature, top_k, top_p, repeat_penalty, repeat_last_n, seed, n_threads, ELF_COMPLETION_FORMAT.Instruct, service_key, streaming_callback)
+        elif self.default_generation_mode == ELF_GENERATION_FORMAT.OLLAMA:
+            return # To be implemented #self.ollama_generate_with_images(prompt, self.host_address, self.model_name, -1, n_predict, stream, temperature, top_k, top_p, repeat_penalty, repeat_last_n, seed, n_threads, ELF_COMPLETION_FORMAT.Instruct, service_key, streaming_callback)
+        elif self.default_generation_mode == ELF_GENERATION_FORMAT.LITELLM:
+            return # To be implemented #self.litellm_generate_with_images(prompt, self.host_address, self.model_name, -1, n_predict, stream, temperature, top_k, top_p, repeat_penalty, repeat_last_n, seed, n_threads, ELF_COMPLETION_FORMAT.Instruct, service_key, streaming_callback)
+
 
     def generate(self, prompt, n_predict=None, stream=False, temperature=0.1, top_k=50, top_p=0.95, repeat_penalty=0.8, repeat_last_n=40, seed=None, n_threads=8, service_key:str="", streaming_callback=None):
         if self.default_generation_mode == ELF_GENERATION_FORMAT.LOLLMS:
             return self.lollms_generate(prompt, self.host_address, self.model_name, -1, n_predict, stream, temperature, top_k, top_p, repeat_penalty, repeat_last_n, seed, n_threads, service_key, streaming_callback)
         elif self.default_generation_mode == ELF_GENERATION_FORMAT.OPENAI:
             return self.openai_generate(prompt, self.host_address, self.model_name, -1, n_predict, stream, temperature, top_k, top_p, repeat_penalty, repeat_last_n, seed, n_threads, ELF_COMPLETION_FORMAT.Instruct, service_key, streaming_callback)
         elif self.default_generation_mode == ELF_GENERATION_FORMAT.OLLAMA:
@@ -138,19 +151,88 @@
             "n_threads": n_threads
         }
 
         response = requests.post(url, json=data, headers=headers, stream=stream)
         if not stream:
             if response.status_code == 200:
                 try:
-                    text = response.text.strip().replace('\"','"')
-                    if text[0]=='"':
-                        text = text[1:]
-                    if text[-1]=='"':
-                        text = text[:-1]
+                    text = response.text.strip().rstrip('!')
+                    return text
+                except Exception as ex:
+                    return {"status": False, "error": str(ex)}
+            else:
+                return {"status": False, "error": response.text}
+        else:
+            text = ""
+            if response.status_code==200:
+                try:
+                    for line in response.iter_lines():
+                        chunk = line.decode("utf-8")
+                        text += chunk
+                        if streaming_callback:
+                            streaming_callback(chunk, MSG_TYPE.MSG_TYPE_CHUNK)
+                    return text.rstrip('!')
+                except Exception as ex:
+                    return {"status": False, "error": str(ex)}
+            else:
+                return {"status": False, "error": response.text}
+            
+
+    def lollms_generate_with_images(self, prompt, images, host_address=None, model_name=None, personality=None, n_predict=None, stream=False, temperature=0.1, top_k=50, top_p=0.95, repeat_penalty=0.8, repeat_last_n=40, seed=None, n_threads=8, service_key:str="", streaming_callback=None):
+        # Set default values to instance variables if optional arguments are None
+        host_address = host_address if host_address else self.host_address
+        model_name = model_name if model_name else self.model_name
+        n_predict = n_predict if n_predict else self.n_predict
+        personality = personality if personality is not None else self.personality
+        # Set temperature, top_k, top_p, repeat_penalty, repeat_last_n, seed, n_threads to the instance variables if they are not provided or None
+        temperature = temperature if temperature is not None else self.temperature
+        top_k = top_k if top_k is not None else self.top_k
+        top_p = top_p if top_p is not None else self.top_p
+        repeat_penalty = repeat_penalty if repeat_penalty is not None else self.repeat_penalty
+        repeat_last_n = repeat_last_n if repeat_last_n is not None else self.repeat_last_n
+        seed = seed or self.seed  # Use the instance seed if not provided
+        n_threads = n_threads if n_threads else self.n_threads
+        def encode_image_to_base64(image_path):
+            with open(image_path, "rb") as image_file:
+                encoded_string = base64.b64encode(image_file.read()).decode('utf-8')
+            return encoded_string
+        # Encode images in base64
+        encoded_images = [encode_image_to_base64(image) for image in images]
+
+        url = f"{host_address}/lollms_generate_with_images"
+        if service_key!="":
+            headers = {
+                'Content-Type': 'application/json;',
+                'Authorization': f'Bearer {service_key}',
+            }
+        else:
+            headers = {
+                'Content-Type': 'application/json',
+            }
+        data = {
+            "prompt": prompt,
+            "model_name": self.model_name,
+            "personality": self.personality,
+            "n_predict": n_predict,
+            "stream": stream,
+            "temperature": self.temperature,
+            "top_k": self.top_k,
+            "top_p": self.top_p,
+            "repeat_penalty": repeat_penalty,
+            "repeat_last_n": repeat_last_n,
+            "seed": seed,
+            "n_threads": n_threads,
+            "images": encoded_images  # Add encoded images to the request payload
+        }
+
+        response = requests.post(url, json=data, headers=headers, stream=stream)
+        if not stream:
+            if response.status_code == 200:
+                try:
+                    text = response.text.rstrip('!')
                     return text
                 except Exception as ex:
                     return {"status": False, "error": str(ex)}
             else:
                 return {"status": False, "error": response.text}
         else:
             text = ""
@@ -167,14 +249,15 @@
                         text = text[:-1]
                     return text
                 except Exception as ex:
                     return {"status": False, "error": str(ex)}
             else:
                 return {"status": False, "error": response.text}
 
+
     def openai_generate(self, prompt, host_address=None, model_name=None, personality=None, n_predict=None, stream=False, temperature=0.1, top_k=50, top_p=0.95, repeat_penalty=0.8, repeat_last_n=40, seed=None, n_threads=8, completion_format:ELF_COMPLETION_FORMAT=ELF_COMPLETION_FORMAT.Instruct, service_key:str="", streaming_callback=None):
         # Set default values to instance variables if optional arguments are None
         host_address = host_address if host_address else self.host_address
         model_name = model_name if model_name else self.model_name
         n_predict = n_predict if n_predict else self.n_predict
         personality = personality if personality is not None else self.personality
         # Set temperature, top_k, top_p, repeat_penalty, repeat_last_n, seed, n_threads to the instance variables if they are not provided or None
```

### Comparing `lollms_client-0.5.9/lollms_client/lollms_discussion.py` & `lollms_client-0.6.0/lollms_client/lollms_discussion.py`

 * *Files identical despite different names*

### Comparing `lollms_client-0.5.9/lollms_client/lollms_personality.py` & `lollms_client-0.6.0/lollms_client/lollms_personality.py`

 * *Files identical despite different names*

### Comparing `lollms_client-0.5.9/lollms_client/lollms_personality_worker.py` & `lollms_client-0.6.0/lollms_client/lollms_personality_worker.py`

 * *Files identical despite different names*

### Comparing `lollms_client-0.5.9/lollms_client/lollms_types.py` & `lollms_client-0.6.0/lollms_client/lollms_types.py`

 * *Files identical despite different names*

### Comparing `lollms_client-0.5.9/lollms_client.egg-info/PKG-INFO` & `lollms_client-0.6.0/lollms_client.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lollms_client
-Version: 0.5.9
+Version: 0.6.0
 Summary: A client library for LoLLMs generate endpoint
 Home-page: https://github.com/ParisNeo/lollms_client
 Author: ParisNeo
 Author-email: parisneoai@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `lollms_client-0.5.9/lollms_client.egg-info/SOURCES.txt` & `lollms_client-0.6.0/lollms_client.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 LICENSE
 README.md
 setup.py
 lollms_client/__init__.py
 lollms_client/lollms_config.py
 lollms_client/lollms_core.py
 lollms_client/lollms_discussion.py
+lollms_client/lollms_functions.py
 lollms_client/lollms_personality.py
 lollms_client/lollms_personality_worker.py
 lollms_client/lollms_tasks.py
 lollms_client/lollms_types.py
 lollms_client/lollms_utilities.py
 lollms_client/lollms_xtts.py
 lollms_client.egg-info/PKG-INFO
```

### Comparing `lollms_client-0.5.9/setup.py` & `lollms_client-0.6.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     long_description = fh.read()
 
 with open('requirements.txt', 'r') as f:
     install_requires = f.read().splitlines()
     
 setuptools.setup(
     name="lollms_client",
-    version="0.5.9",
+    version="0.6.0",
     author="ParisNeo",
     author_email="parisneoai@gmail.com",
     description="A client library for LoLLMs generate endpoint",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/ParisNeo/lollms_client",
     packages=setuptools.find_packages(),
```

