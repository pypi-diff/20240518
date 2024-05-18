# Comparing `tmp/ALLMDEV-1.3.2-py3-none-any.whl.zip` & `tmp/ALLMDEV-1.3.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,23 +1,24 @@
-Zip file size: 21663 bytes, number of entries: 21
+Zip file size: 25901 bytes, number of entries: 22
 -rw-rw-rw-  2.0 fat       39 b- defN 24-Apr-17 06:01 ALLMDEV/__init__.py
 -rw-rw-rw-  2.0 fat     3706 b- defN 24-May-04 14:17 ALLMDEV/agentapi.py
 -rw-rw-rw-  2.0 fat     3440 b- defN 24-Apr-27 08:48 ALLMDEV/agentchat.py
 -rw-rw-rw-  2.0 fat     4986 b- defN 24-May-11 17:03 ALLMDEV/azureagentapi.py
 -rw-rw-rw-  2.0 fat     3298 b- defN 24-May-11 16:47 ALLMDEV/azureagentchat.py
 -rw-rw-rw-  2.0 fat     2435 b- defN 24-May-11 16:47 ALLMDEV/azurecli.py
--rw-rw-rw-  2.0 fat      757 b- defN 24-May-04 08:56 ALLMDEV/cli.py
--rw-rw-rw-  2.0 fat    11849 b- defN 24-May-11 11:56 ALLMDEV/instruct.py
+-rw-rw-rw-  2.0 fat    20218 b- defN 24-May-18 11:12 ALLMDEV/backend.py
+-rw-rw-rw-  2.0 fat     3221 b- defN 24-May-15 11:30 ALLMDEV/cli.py
+-rw-rw-rw-  2.0 fat    12685 b- defN 24-May-15 08:32 ALLMDEV/instruct.py
 -rw-rw-rw-  2.0 fat     3096 b- defN 24-Apr-27 08:57 ALLMDEV/newagent.py
--rw-rw-rw-  2.0 fat     2795 b- defN 24-May-04 14:18 ALLMDEV/serve.py
--rw-rw-rw-  2.0 fat     1927 b- defN 24-May-11 17:57 ALLMDEV/studio.py
+-rw-rw-rw-  2.0 fat     1432 b- defN 24-May-15 08:34 ALLMDEV/serve.py
+-rw-rw-rw-  2.0 fat     1932 b- defN 24-May-15 12:35 ALLMDEV/studio.py
 -rw-rw-rw-  2.0 fat      683 b- defN 24-May-04 14:32 ALLMDEV/test.py
 -rw-rw-rw-  2.0 fat     3096 b- defN 24-May-05 07:54 ALLMDEV/updateagent.py
 -rw-rw-rw-  2.0 fat     4530 b- defN 24-May-11 16:47 ALLMDEV/vertexagentapi.py
--rw-rw-rw-  2.0 fat     2824 b- defN 24-May-11 13:36 ALLMDEV/vertexagentchat.py
--rw-rw-rw-  2.0 fat     2124 b- defN 24-May-11 13:27 ALLMDEV/vertexcli.py
--rw-rw-rw-  2.0 fat     5962 b- defN 24-May-11 18:07 ALLMDEV-1.3.2.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 24-May-11 18:07 ALLMDEV-1.3.2.dist-info/WHEEL
--rw-rw-rw-  2.0 fat      556 b- defN 24-May-11 18:07 ALLMDEV-1.3.2.dist-info/entry_points.txt
--rw-rw-rw-  2.0 fat        8 b- defN 24-May-11 18:07 ALLMDEV-1.3.2.dist-info/top_level.txt
--rw-rw-r--  2.0 fat     1621 b- defN 24-May-11 18:07 ALLMDEV-1.3.2.dist-info/RECORD
-21 files, 59824 bytes uncompressed, 19071 bytes compressed:  68.1%
+-rw-rw-rw-  2.0 fat     2826 b- defN 24-May-14 10:42 ALLMDEV/vertexagentchat.py
+-rw-rw-rw-  2.0 fat     2126 b- defN 24-May-14 10:42 ALLMDEV/vertexcli.py
+-rw-rw-rw-  2.0 fat     6060 b- defN 24-May-18 11:12 ALLMDEV-1.3.3.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 24-May-18 11:12 ALLMDEV-1.3.3.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat      591 b- defN 24-May-18 11:12 ALLMDEV-1.3.3.dist-info/entry_points.txt
+-rw-rw-rw-  2.0 fat        8 b- defN 24-May-18 11:12 ALLMDEV-1.3.3.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat     1698 b- defN 24-May-18 11:12 ALLMDEV-1.3.3.dist-info/RECORD
+22 files, 82198 bytes uncompressed, 23197 bytes compressed:  71.8%
```

## zipnote {}

```diff
@@ -12,14 +12,17 @@
 
 Filename: ALLMDEV/azureagentchat.py
 Comment: 
 
 Filename: ALLMDEV/azurecli.py
 Comment: 
 
+Filename: ALLMDEV/backend.py
+Comment: 
+
 Filename: ALLMDEV/cli.py
 Comment: 
 
 Filename: ALLMDEV/instruct.py
 Comment: 
 
 Filename: ALLMDEV/newagent.py
@@ -42,23 +45,23 @@
 
 Filename: ALLMDEV/vertexagentchat.py
 Comment: 
 
 Filename: ALLMDEV/vertexcli.py
 Comment: 
 
-Filename: ALLMDEV-1.3.2.dist-info/METADATA
+Filename: ALLMDEV-1.3.3.dist-info/METADATA
 Comment: 
 
-Filename: ALLMDEV-1.3.2.dist-info/WHEEL
+Filename: ALLMDEV-1.3.3.dist-info/WHEEL
 Comment: 
 
-Filename: ALLMDEV-1.3.2.dist-info/entry_points.txt
+Filename: ALLMDEV-1.3.3.dist-info/entry_points.txt
 Comment: 
 
-Filename: ALLMDEV-1.3.2.dist-info/top_level.txt
+Filename: ALLMDEV-1.3.3.dist-info/top_level.txt
 Comment: 
 
-Filename: ALLMDEV-1.3.2.dist-info/RECORD
+Filename: ALLMDEV-1.3.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## ALLMDEV/cli.py

```diff
@@ -1,16 +1,86 @@
 import argparse
 from .instruct import load_model, infer
+from flask import Flask, render_template, request
+from flask_socketio import SocketIO
+import time
+from flask_cors import CORS
+from concurrent.futures import ThreadPoolExecutor
+import os
+from llama_index.llms.llama_cpp import LlamaCPP
 
+
+def cli_inference(args):
+    model_path = load_model(args.name)
+    print("Starting CLI-based inference...\n")
+    infer(model_path, args.temperature, args.max_new_tokens, args.model_kwargs)
+
+def launch_ui():
+        app = Flask(__name__)
+        CORS(app, resources={r"/*": {"origins": "*"}})
+        socketio = SocketIO(app)
+
+        prompt_template = "<s>[INST] {prompt} [/INST]"
+
+        executor = ThreadPoolExecutor(max_workers=1)
+
+        @app.route('/')
+        def index():
+            return render_template('index.html')
+
+        @app.route('/send_message', methods=['POST'])
+        def send_message():
+            data = request.json
+            prompt = data['userInput']
+            modelPath = data['filePath']
+            filepath = os.path.normpath(modelPath)
+            path=filepath.replace("\\", "\\\\")
+            temperature = data['temperature']
+            useGPU = data['useGPU']
+            print('Received userInput:', prompt)
+            print('Received filePath:', path)
+            print('Received temperature:', temperature)
+            print('Received useGPU:', useGPU)
+
+            formatted_prompt = prompt_template.format(prompt=prompt)
+
+            # Initialize LLAM object with the selected model path, temperature, and GPU settings
+            llm = LlamaCPP(
+                model_path=path,
+                temperature=float(temperature),
+                max_new_tokens=512,
+                context_window=3900,
+                model_kwargs={"n_gpu_layers": 1 if useGPU else 0},
+                verbose=False,
+            )
+
+            # Perform inference and stream the generated tokens
+            response_iter = llm.stream_complete(formatted_prompt)
+            prev_token = ''
+            for response in response_iter:
+                token = response.delta
+                # new_token = token.replace(prev_token, token)
+                # if new_token:
+                print(token, end='')
+                socketio.emit('response', token)
+                # prev_token = token
+            time.sleep(0.01)
+
+
+            return None
+        socketio.run(app)
 def main():
     parser = argparse.ArgumentParser()
     parser.add_argument("--name", type=str, default="Mistral", help="Name of the model or path to the model file")
     parser.add_argument("--temperature", type=float, default=0.5, help="Temperature for sampling")
     parser.add_argument("--max_new_tokens", type=int, default=512, help="Maximum number of new tokens to generate")
     parser.add_argument("--model_kwargs", type=dict, default={"n_gpu_layers":0}, help="Arguments for the model")
+    parser.add_argument('--launch', action='store_true', help='Launch the UI for inference')
     args = parser.parse_args()
 
-    model_path = load_model(args.name)
-    infer(model_path, args.temperature, args.max_new_tokens, args.model_kwargs)
+    if args.launch:
+        launch_ui()
+    else:
+        cli_inference(args)
 
 if __name__ == "__main__":
     main()
```

## ALLMDEV/instruct.py

```diff
@@ -1,11 +1,14 @@
 from llama_index.llms.llama_cpp import LlamaCPP
 from huggingface_hub import hf_hub_download
 import os
 import shutil
+from flask import Flask, request, jsonify
+
+
 
 def load_model(model):
             model_dir = 'model'
             if not os.path.exists(model_dir):
                 os.makedirs(model_dir)
 
             model_files = [f for f in os.listdir('model') if f.endswith('.gguf')]
@@ -146,14 +149,28 @@
                     # except:
                     #     print("Kindly check input parameter to the model_load() function. The parameter should be one of the following: \"Mistral\", \"mistral\", \"Mistral_instruct\", \"mistral_instruct\", \"Llama2\", \"Llama2_chat\", or a local gguf file path on your system")
 
             return model_path
 
 
 
+model_files = [f for f in os.listdir('model') if f.endswith('.gguf')]
+model_path = load_model(model_files[0]) if model_files else None
+
+llm = LlamaCPP(
+    model_path=model_path,
+    temperature=0.1,
+    max_new_tokens=512,
+    context_window=3900,
+    model_kwargs={"n_gpu_layers": 0},
+    verbose=False,
+)
+
+
+
 def infer(model_path, temperature=0.5, max_new_tokens=512, model_kwargs={"n_gpu_layers":0}):
 
 
         # Define a prompt template
         prompt_template = "<s>[INST] {prompt} [/INST]"
         # print(model_path)
 
@@ -189,9 +206,20 @@
                 for response in response_iter:
                     print(response.delta, end="", flush=True)
 
             except KeyboardInterrupt:
                 print("\nExiting...")
                 break
 
+def api_serve():
+        user_input = request.json.get("input")
+
+        if user_input.lower() == "exit":
+            return jsonify({"response": "Exiting chat."})
+
+        prompt_template = "<s>[INST] {prompt} [/INST]"
+        prompt = prompt_template.format(prompt=user_input)
+
+        response_iter = llm.stream_complete(prompt)
+        response_text = ''.join(response.delta for response in response_iter)
 
-        
+        return jsonify({"response": response_text})
```

## ALLMDEV/serve.py

```diff
@@ -1,79 +1,41 @@
-from flask import Flask, request, jsonify
-from llama_index.llms.llama_cpp import LlamaCPP
-from .instruct import load_model
+from flask import Flask
+from .instruct import load_model, api_serve
 import os
+import json
 
 app = Flask(__name__)
 
-# Check if apiconfig.txt exists in the model folder
-config_file_path = os.path.join('model', 'apiconfig.txt')
-if not os.path.exists(config_file_path):
-    # Create apiconfig.txt with default values
-    with open(config_file_path, 'w') as file:
-       file.write('Host=127.0.0.1\n')
-       file.write('Port=5000\n')
-       file.write('CertFile=""\n')
-       file.write('CertKey=""\n')
-
-# Read host and port from apiconfig.txt
-if os.path.exists(config_file_path):
-    with open(config_file_path, 'r') as file:
-        for line in file:
-            key, value = line.strip().split('=')
-            if key == 'Host':
-                host = value
-            elif key == 'Port':
-                port = int(value)
-            elif key == 'CertFile':
-                cert_file = value.strip('"')
-            elif key == 'CertKey':
-                cert_key = value.strip('"')
-else:
-    print("File doesn't exist.")
-    host = '127.0.0.1'
-    port = 5000
-    cert_file = ""
-    cert_key = ""
-
-print("Host:", host)
-print("Port:", port)
-print("CertFile:", cert_file)
-print("CertKey:", cert_key)
-
-model_files = [f for f in os.listdir('model') if f.endswith('.gguf')]
-model_path = load_model(model_files[0]) if model_files else None
-
-llm = LlamaCPP(
-    model_path=model_path,
-    temperature=0.1,
-    max_new_tokens=512,
-    context_window=3900,
-    model_kwargs={"n_gpu_layers": 0},
-    verbose=False,
-)
+model_dir = "model"
+
+config = {
+    "host": "127.0.0.1",
+    "port": "5173",
+    "cert_file": "",
+    "cert_key": ""
+}
+
+file_path=os.path.join(model_dir, "apiconfig.json")
+if not os.path.exists(file_path):
+    with open(file_path, "w") as json_file:
+        json.dump(config, json_file)
 
 @app.route('/v1/chat/completions', methods=['POST'])
 def chat():
-    user_input = request.json.get("input")
-
-    if user_input.lower() == "exit":
-        return jsonify({"response": "Exiting chat."})
-
-    prompt_template = "<s>[INST] {prompt} [/INST]"
-    prompt = prompt_template.format(prompt=user_input)
-
-    response_iter = llm.stream_complete(prompt)
-    response_text = ''.join(response.delta for response in response_iter)
-
-    return jsonify({"response": response_text})
+    api_serve()
 
 def main():
+        with open(file_path, "r") as json_file:
+            config = json.load(json_file)
+            host=config["host"]
+            port=config["port"]
+            cert_file=config["cert_file"]
+            cert_key=config["cert_key"]
         if cert_file is not "" and cert_key is not "":
-            print(f"Inference is working on https://{host}:{port}/v1/chat/completions. You can configure custom host IP and port, and ssl certificate via the apiconfig.txt file available at {config_file_path}")
+            print(f"Inference is working on https://{host}:{port}/v1/chat/completions. You can configure custom host IP and port, and ssl certificate via the apiconfig.txt file available at {file_path}")
             app.run(host=host, port=port, debug=False, ssl_context=(cert_file,cert_key))
         else:
-            print(f"Inference is working on http://{host}:{port}/v1/chat/completions. You can configure custom host IP and port, and ssl certificate via the apiconfig.txt file available at {config_file_path}")
+            print(f"Inference is working on http://{host}:{port}/v1/chat/completions. You can configure custom host IP and port, and ssl certificate via the apiconfig.txt file available at {file_path}")
             app.run(host=host, port=port, debug=False)
 
 if __name__ == "__main__":
     main()
```

## ALLMDEV/studio.py

```diff
@@ -15,15 +15,14 @@
 executor = ThreadPoolExecutor(max_workers=1)
 
 @app.route('/')
 def index():
     return render_template('index.html')
 
 @app.route('/send_message', methods=['POST'])
-@app.route('/send_message', methods=['POST'])
 def send_message():
     data = request.json
     prompt = data['userInput']
     modelPath = data['filePath']
     filepath = os.path.normpath(modelPath)
     path=filepath.replace("\\", "\\\\")
     temperature = data['temperature']
@@ -56,11 +55,12 @@
         socketio.emit('response', token)
         # prev_token = token
     time.sleep(0.01)
 
 
     return None
 
-
+def main():
+    socketio.run(app, host='localhost', port=8080)
 
 if __name__ == '__main__':
-    socketio.run(app)
+    main()
```

## ALLMDEV/vertexagentchat.py

```diff
@@ -50,15 +50,15 @@
     parser.add_argument("--agent", type=str, default=None, help="Name of the agent to query.")
     args = parser.parse_args()
     with open(file_path, "r") as json_file:
         config = json.load(json_file)
         projectid=config["project_id"]
         region=config["region"]
         model=config["model"] 
-        print(projectid, region, model)
+        # print(projectid, region, model)
     if projectid != "" and region != "" and model != "":
     # Initialize Vertex AI
         vertexai.init(project=projectid, location=region)
         # Load the model
         multimodal_model = GenerativeModel(model_name=model)
     else:
         vertexai.init(project=args.projectid, location=args.region)
```

## ALLMDEV/vertexcli.py

```diff
@@ -37,15 +37,15 @@
 
     # if os.path.exists(file_path):
     with open(file_path, "r") as json_file:
         config = json.load(json_file)
         projectid=config["project_id"]
         region=config["region"]
         model=config["model"] 
-        print(projectid, region, model)
+        # print(projectid, region, model)
     if projectid != "" and region != "" and model != "":
     # Initialize Vertex AI
         vertexai.init(project=projectid, location=region)
         # Load the model
         multimodal_model = GenerativeModel(model_name=model)
     else:
         vertexai.init(project=args.projectid, location=args.region)
```

## Comparing `ALLMDEV-1.3.2.dist-info/METADATA` & `ALLMDEV-1.3.3.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ALLMDEV
-Version: 1.3.2
+Version: 1.3.3
 Summary: A simple and efficient python library for fast inference of GGUF Large Language Models.
 Author: All Advance AI
 Author-email: allmdev@allaai.com
 Maintainer: Soham Ghadge
 Maintainer-email: soham.ghadge@allaai.com
 Keywords: GGUF,GGUF Large Language Model,GGUF Large Language Models,GGUF Large Language Modeling,GGUF Large Language Modeling Library
 Description-Content-Type: text/markdown
@@ -161,10 +161,16 @@
 allm-run-azure --key key --version version --endpoint https://{your_endpoint}.openai.azure.com --model model_name --agent agentname
 ```
 or
 ```bash
 allm-agentapi-vertex --agent agent_name
 ```
 
+#ALLM-Enterprise
+You can launch the UI with the following command:
+```bash
+allm-launch
+```
+
 ## Supported Model names
 Llama3, Llama2, llama, llama2_chat, Llama_chat, Mistral, Mistral_instruct
```

## Comparing `ALLMDEV-1.3.2.dist-info/entry_points.txt` & `ALLMDEV-1.3.3.dist-info/entry_points.txt`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 [console_scripts]
 allm-agentapi = ALLMDEV.agentapi:main
 allm-agentapi-azure = ALLMDEV.azureagentapi:main
 allm-agentapi-vertex = ALLMDEV.vertexagentapi:main
 allm-agentchat = ALLMDEV.agentchat:main
 allm-agentchat-azure = ALLMDEV.azureagentchat:main
 allm-agentchat-vertex = ALLMDEV.vertexagentchat:main
+allm-launch = ALLMDEV.backend:main
 allm-newagent = ALLMDEV.newagent:main
 allm-run = ALLMDEV.cli:main
 allm-run-azure = ALLMDEV.azurecli:main
 allm-run-vertex = ALLMDEV.vertexcli:main
 allm-serve = ALLMDEV.serve:main
 allm-studio = ALLMDEV.studio:main
 allm-updateagent = ALLMDEV.updateagent:main
```

