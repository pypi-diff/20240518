# Comparing `tmp/llm_axe-1.0.9.tar.gz` & `tmp/llm_axe-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llm_axe-1.0.9.tar", last modified: Fri May 17 13:38:27 2024, max compression
+gzip compressed data, was "llm_axe-1.1.0.tar", last modified: Sat May 18 16:20:25 2024, max compression
```

## Comparing `llm_axe-1.0.9.tar` & `llm_axe-1.1.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-05-17 13:38:27.817139 llm_axe-1.0.9/
--rw-rw-rw-   0        0        0     3914 2024-05-17 13:38:27.816638 llm_axe-1.0.9/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-17 13:38:27.788139 llm_axe-1.0.9/llm_axe/
--rw-rw-rw-   0        0        0       67 2024-04-22 04:52:11.000000 llm_axe-1.0.9/llm_axe/__init__.py
--rw-rw-rw-   0        0        0    21505 2024-05-17 04:58:22.000000 llm_axe-1.0.9/llm_axe/agents.py
--rw-rw-rw-   0        0        0     6047 2024-05-17 05:18:31.000000 llm_axe-1.0.9/llm_axe/core.py
--rw-rw-rw-   0        0        0      581 2024-05-04 16:21:13.000000 llm_axe-1.0.9/llm_axe/models.py
--rw-rw-rw-   0        0        0     8161 2024-05-17 05:27:31.000000 llm_axe-1.0.9/llm_axe/system_prompts.yaml
-drwxrwxrwx   0        0        0        0 2024-05-17 13:38:27.815638 llm_axe-1.0.9/llm_axe.egg-info/
--rw-rw-rw-   0        0        0     3914 2024-05-17 13:38:27.000000 llm_axe-1.0.9/llm_axe.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      262 2024-05-17 13:38:27.000000 llm_axe-1.0.9/llm_axe.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-17 13:38:27.000000 llm_axe-1.0.9/llm_axe.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      118 2024-05-17 13:38:27.000000 llm_axe-1.0.9/llm_axe.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-05-17 13:38:27.000000 llm_axe-1.0.9/llm_axe.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-17 13:38:27.817139 llm_axe-1.0.9/setup.cfg
--rw-rw-rw-   0        0        0     4619 2024-05-17 13:37:47.000000 llm_axe-1.0.9/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-18 16:20:25.194175 llm_axe-1.1.0/
+-rw-rw-rw-   0        0        0     3914 2024-05-18 16:20:25.193673 llm_axe-1.1.0/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-18 16:20:25.178674 llm_axe-1.1.0/llm_axe/
+-rw-rw-rw-   0        0        0       67 2024-04-22 04:52:11.000000 llm_axe-1.1.0/llm_axe/__init__.py
+-rw-rw-rw-   0        0        0    26131 2024-05-18 16:12:16.000000 llm_axe-1.1.0/llm_axe/agents.py
+-rw-rw-rw-   0        0        0     6172 2024-05-18 05:39:43.000000 llm_axe-1.1.0/llm_axe/core.py
+-rw-rw-rw-   0        0        0      640 2024-05-18 05:10:13.000000 llm_axe-1.1.0/llm_axe/models.py
+-rw-rw-rw-   0        0        0     9070 2024-05-18 16:01:16.000000 llm_axe-1.1.0/llm_axe/system_prompts.yaml
+drwxrwxrwx   0        0        0        0 2024-05-18 16:20:25.192673 llm_axe-1.1.0/llm_axe.egg-info/
+-rw-rw-rw-   0        0        0     3914 2024-05-18 16:20:25.000000 llm_axe-1.1.0/llm_axe.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      262 2024-05-18 16:20:25.000000 llm_axe-1.1.0/llm_axe.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-18 16:20:25.000000 llm_axe-1.1.0/llm_axe.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      118 2024-05-18 16:20:25.000000 llm_axe-1.1.0/llm_axe.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-05-18 16:20:25.000000 llm_axe-1.1.0/llm_axe.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-18 16:20:25.194175 llm_axe-1.1.0/setup.cfg
+-rw-rw-rw-   0        0        0     4619 2024-05-18 16:19:51.000000 llm_axe-1.1.0/setup.py
```

### Comparing `llm_axe-1.0.9/PKG-INFO` & `llm_axe-1.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llm_axe
-Version: 1.0.9
+Version: 1.1.0
 Summary: A toolkit for quickly implementing llm powered functionalities.
 Author: Emir Sahin
 Author-email: emirsah122@gmail.com
 License: MIT
 Keywords: python,llm axe,llm toolkit,local llm,local llm internet,function caller llm,ollama
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `llm_axe-1.0.9/llm_axe/agents.py` & `llm_axe-1.1.0/llm_axe/agents.py`

 * *Files 11% similar despite different names*

```diff
@@ -5,33 +5,35 @@
 from llm_axe.core import AgentType, safe_read_json, generate_schema, get_yaml_prompt, internet_search, read_website, read_pdf, make_prompt, llm_has_ask
 
 
 class Agent:
     """
     Basic agent that can use premade or custom system prompts.
     """
-    def __init__(self, llm:object, agent_type:AgentType=None, additional_system_instructions:str="", custom_system_prompt:str=None):
+    def __init__(self, llm:object, agent_type:AgentType=None, additional_system_instructions:str="", custom_system_prompt:str=None, temperature:float=0.8):
         """
         Args:
             llm (object): An LLM object with an ask function.
             agent_type (AgentType, optional): The type of agent to use. Choose from AgentType enum. Defaults to None.
-            system_prompt (Agent): The name of the system prompt to use from the system_prompts.yaml file. See documentation for list.
+            additional_system_instructions (str, optional): Additional system instructions to include in the system prompt. Defaults to "".
             custom_system_prompt (any, optional): An optional string to override and use as the custom system prompt.
+            temperature (float, optional): The temperature of the LLM. Defaults to 0.8.
         """
         self.llm = llm
         self.chat_history = []
         if custom_system_prompt is None:
             if agent_type is None:
-                raise ValueError("You must provide either a system_prompt or a custom_system_prompt.")
+                raise ValueError("You must provide either a AgentType or a custom_system_prompt.")
             else:
                 self.system_prompt = get_yaml_prompt("system_prompts.yaml", agent_type.value)
         else:
             self.system_prompt = custom_system_prompt
         
         self.system_prompt = make_prompt("system", self.system_prompt.format(additional_instructions=additional_system_instructions))
+        self.temperature = temperature
 
     def get_prompt(self, question):
         """
         Get the prompt for the given question.
         Args:
             question (str): The question to get the prompt for.
         """
@@ -50,39 +52,106 @@
             return None
         
         prompts = [self.system_prompt]
         if history is not None:
             prompts.extend(history)
 
         prompts.append(make_prompt("user", prompt))
-        response = self.llm.ask(prompts)
+        response = self.llm.ask(prompts, temperature=self.temperature)
     
         self.chat_history.append(prompts[-1])
         self.chat_history.append(make_prompt("assistant", response))
         return response
 
 
+class ObjectDetectorAgent():
+    """
+    An ObjectDetectorAgent agent is used to detect objects in an image.
+    Requires a multimodal LLM.
+    """
+    def __init__(self, llm:object, temperature:float=0.3):
+        """
+        Initializes a new ObjectDetectorAgent object.
+
+        Args:
+            llm (object): A multimodal LLM object that implements the ask() method.
+            temperature (float, optional): The temperature of the LLM. Defaults to 0.3.
+        """
+        self.llm = llm
+        self.__system_prompt = make_prompt("system", get_yaml_prompt("system_prompts.yaml", "ObjectDetector"))
+        self.temperature = temperature
+
+    def detect(self, images:list, objects:list=None, detection_criteria:str=None):
+        """
+        Detects objects in an image.
+        If given a list of objects, only the objects in the list will be detected.
+        If a prompt is given instead, it will detect according to the prompt's instructions. 
+        Args:
+            images (list): The images to detect objects in. List of string paths or byte data.
+            objects (list, optional): An optional list of objects to detect. Defaults to None.
+            detection_criteria (str, optional): An opetional detection criteria to give.
+        """
+        if llm_has_ask(self.llm) is False:
+            return None
+        
+        prompts = make_prompt("user", "Detect all objects in this image", images=images)
+        detected_objects = self.llm.ask([self.__system_prompt, prompts], temperature=self.temperature)
+        prompts = self.__get_prompt(images, detected_objects, objects, detection_criteria)
+        response = self.llm.ask(prompts, format="json", temperature=0.1)
+
+        return response
+        
+    def __get_prompt(self, images:list, detected_objects:list, objects:list=None, detection_criteria:str=None):
+        """
+        Get the prompt for the given objects and detection_prompt.
+        Args:
+            images (list): The images to detect objects in. List of string paths or byte data.
+            detected_objects (list): The detected objects in the images.
+            objects (list, optional): An optional list of objects to detect. Defaults to None.
+            detection_criteria (str, optional): An opetional detection criteria to give.
+        """
+        prompt = ""
+        sys_prompt = make_prompt("system", get_yaml_prompt("system_prompts.yaml", "ObjectFilterer"))
+        if detection_criteria is None:
+            if objects is None:
+                raise ValueError("You must provide either an object list or a detection_prompt.")
+            else:
+                prompt = "Image Objects: " + detected_objects + "\n\n My list of objects I'm interested in is: " + ", ".join(objects)
+        else:
+            prompt = "Image Objects: " + detected_objects + "\n" + detection_criteria
+        prompt = make_prompt("user", prompt, images=images)
+        return [sys_prompt, prompt]
+
+
 class PythonAgent():
     """
     A PytonAgent agent is used to solve problems by writing Python code.
     It will provide code to execute and the imports used in the code.
     IMPORTANT!!: Code should ALWAYS be executed in a virtual or isolated environment.
     """
-    def __init__(self, llm:object):
+    def __init__(self, llm:object, temperature:float=0.8):
+        """
+        Initializes a new PythonAgent object.
+
+        Args:
+            llm (object): An object that implements the ask() method.
+            temperature (float, optional): The temperature of the LLM. Defaults to 0.8.
+        """
         self.llm = llm
         self.chat_history = []
         self.system_prompt = make_prompt("system", get_yaml_prompt("system_prompts.yaml", "PythonAgent"))
         self.library_extractor_prompt = make_prompt("system", get_yaml_prompt("system_prompts.yaml", "ImportExtractor"))
+        self.temperature = temperature
 
     def ask(self, prompt, history:list=None):
         """
         Ask a question based on the given prompt.
         Args:
             prompt (str): The prompt to use for the question. Will only use system_prompt if prompt is None.
-            history (list, optional): The history of the conversation. Defaults to None.
+            history (list, optional): A list of previous chat messages in openai format. Defaults to None.
         Returns:
             dict: A dictionary containing the "code" and "imports" keys.
                 "code": The code to execute. In string format. WARNING!:CODE SHOULD NEVER BE EXECUTED OUTSIDE OF A VIRTUAL OR ISOLATED ENVIRONMENT.
                 "libraries": The imports used in the code. In json list format.
         """
         if llm_has_ask(self.llm) is False:
             return None
@@ -91,56 +160,58 @@
         coder_prompts.append(self.system_prompt)
         if history is not None:
             coder_prompts.extend(history)
 
         user_prompt = make_prompt("user", prompt)
         coder_prompts.append(user_prompt)
             
-        code_response = self.llm.ask(coder_prompts)
+        code_response = self.llm.ask(coder_prompts, temperature=self.temperature)
         self.chat_history.append(user_prompt)
         self.chat_history.append(make_prompt("assistant", code_response))
 
         code = code_response.split("```")[1]
 
         # Clean up code
         if "Python" in code:
             code = code.replace("Python", "")
         
         # Extract imports
-        imports = self.llm.ask([self.library_extractor_prompt, make_prompt("user", code_response)], format="json")
+        imports = self.llm.ask([self.library_extractor_prompt, make_prompt("user", code_response)], format="json", temperature=self.temperature)
         self.chat_history.append(make_prompt("assistant", imports))
         imports = safe_read_json(imports)
 
         return {"code":code, "libraries":imports}
 
 
 class DataExtractor():
     """
     A DataExtractor agent is used to extract information from given content.
     """
-    def __init__(self, llm:object, reply_as_json:bool=False, additional_system_instructions:str=""):
+    def __init__(self, llm:object, reply_as_json:bool=False, additional_system_instructions:str="", temperature:float=0.8):
         """
         Initializes a new DataExtractor.
         Args:
             llm (object): An object that implements the ask() method.
             reply_as_json (bool, optional): If True, the response will be in the format of a JSON object. Defaults to False.
             additional_system_instructions (str, optional): Additional instructions to include in the system prompt. Defaults to "".
+            temperature (float, optional): The temperature of the LLM. Defaults to 0.8.
         """
         yaml_prompt = "DataExtractorJson" if reply_as_json else "DataExtractor"
         self.system_prompt = get_yaml_prompt("system_prompts.yaml", yaml_prompt)
         self.system_prompt = make_prompt("system", self.system_prompt.format(additional_instructions=additional_system_instructions))
         self.llm = llm
         self.chat_history = []
+        self.temperature = temperature
 
     def get_prompt(self, info:str, data_points:list=[]):
         """
         Get the prompt for the given content.
         Args:
             info (str): The content to extract information from.
-            data_points (list, optional): A list of data points to extract. Defaults to None.
+            data_points (list, optional): A string list of data points to extract. Defaults to None.
         """
         prompt = '''
                 Extract information from the following content:
                 {content}
 
                 Extract the following data:
                 {data}
@@ -149,41 +220,43 @@
         return [self.system_prompt, make_prompt("user", prompt)]
     
     def ask(self, info:str, data_points:list=[]):
         """
         Ask a question based on the given content.
         Args:
             info (str): The content to extract information from.
-            data_points (list, optional): A list of data points to extract. Defaults to None.
+            data_points (list, optional): A string list of data points to extract. Defaults to None.
         """
         prompts = self.get_prompt(info, data_points)
-        resp = self.llm.ask(self.get_prompt(info, data_points))
+        resp = self.llm.ask(self.get_prompt(info, data_points), temperature=self.temperature)
         self.chat_history.append(prompts[1])
         self.chat_history.append(make_prompt("assistant", resp))
         return resp
     
 
 class PdfReader():
     """
     A PdfReader agent is used to answer questions based on information from given PDF files.
     """
 
-    def __init__(self, llm:object, additional_system_instructions:str="", custom_system_prompt:str=None):
+    def __init__(self, llm:object, additional_system_instructions:str="", custom_system_prompt:str=None, temperature:float=0.8):
         """
         Initializes a new PdfReader.
         Args:
             llm (object): An object that implements the ask() method.
             additional_system_instructions (str, optional): Additional instructions to include in the system prompt.
             custom_system_prompt (str, optional): Custom system prompt. Defaults to None.
+            temperature (float, optional): The temperature of the LLM. Defaults to 0.8.
         """
         self.chat_history = []
         self.llm = llm
         self.additional_instructions = additional_system_instructions
         self.system_prompt = get_yaml_prompt("system_prompts.yaml", "DocumentReader")
         self.custom_system_prompt = custom_system_prompt
+        self.temperature = temperature
 
 
     def ask(self, question:str, pdf_files:list, history:list=None):
         """
         Ask a question based on the given PDF files.
         Args:
             question (str): The question to ask.
@@ -197,15 +270,15 @@
         question_prompts = self.get_prompt(question, pdf_files)
         prompts.append(question_prompts[0])
 
         if history is not None:
             prompts.extend(history)
 
         prompts.append(question_prompts[1])
-        response = self.llm.ask(prompts)
+        response = self.llm.ask(prompts, temperature=self.temperature)
 
         self.chat_history.append(question_prompts[1]) # dont include the system prompt
         self.chat_history.append(make_prompt("assistant", response))
         return response
     
     def get_prompt(self, question, pdf_files:list=None):
         """
@@ -236,29 +309,31 @@
     """
     A FunctionCaller agent is used to call functions using an LLM.
     By default, premade system prompts are used, however you can provide your own if you have issues with the default.
     For best results, your function name and parameters must be given meaningful names, 
     have type annotations doc string descriptions.
     """
 
-    def __init__(self, llm:object, functions:list, additional_system_instructions:str="", custom_system_prompt:str=None):            
+    def __init__(self, llm:object, functions:list, additional_system_instructions:str="", custom_system_prompt:str=None, temperature:float=0.8):            
         """
         Initializes a new Function Caller.
 
         Args:
             llm (object, optional): An LLM object. Must have an ask method. Defaults to None.
             functions (list, optional): A list of functions. Defaults to None.
             additional_system_instructions (str, optional): Instructions in addition to the system prompt. Defaults to "".
             custom_system_prompt (str, optional): A custom system prompt. Will override the default. Defaults to None.
+            temperature (float, optional): The temperature of the LLM. Defaults to 0.8.
         """
         self.chat_history = []
         self.llm = llm
         self.functions_dict = {func.__name__: func for func in functions}
         self.additional_instructions = additional_system_instructions
         self.schema = generate_schema(functions)
+        self.temperature = temperature
 
         if custom_system_prompt is None:
             self.system_prompt = get_yaml_prompt("system_prompts.yaml", "FunctionCaller")
         else:
             self.system_prompt = custom_system_prompt
 
         self.system_prompt = make_prompt("system", self.system_prompt.format(schema=self.schema, additional_instructions=additional_system_instructions))
@@ -293,15 +368,15 @@
         question_prompts = self.get_prompt(question)
         prompts.append(question_prompts[0])
 
         if history is not None:
             prompts.extend(history)
         prompts.append(question_prompts[1])            
 
-        response = self.llm.ask(prompts, format="json")
+        response = self.llm.ask(prompts, format="json", temperature=self.temperature)
         response_json = safe_read_json(response)
 
         self.chat_history.append(question_prompts[1])
         self.chat_history.append(make_prompt("assistant", response))
 
         if response_json is None:
             return None
@@ -347,36 +422,38 @@
 
 
 class WebsiteReaderAgent:
     """
     An agent that can will read a website and answer questions based on it.
     """
 
-    def __init__(self, llm:object, additional_system_instructions:str="", custom_site_reader:callable=None):
+    def __init__(self, llm:object, additional_system_instructions:str="", custom_site_reader:callable=None, temperature:float=0.8):
         """
         Args:
             llm (object): An LLM object. Must have an ask method.
             url (str): The url of the website to read.
             additional_system_instructions (str, optional): Instructions in addition to the system prompt. Defaults to "".
             custom_site_reader (function, optional): A custom online site reader function. The site reader function must take a URL and return a string representation of the site.
+            temperature (float, optional): The temperature of the LLM. Defaults to 0.8.
         """
         self.llm = llm
         self.chat_history = []
         self.system_prompt = get_yaml_prompt("system_prompts.yaml", "WebsiteReader")
         self.additional_system_instructions = additional_system_instructions
         self.read_function = custom_site_reader if custom_site_reader else read_website
+        self.temperature = temperature
 
     def ask(self, question:str, url:str, history:list=None):
         """
         Answers the question based on the provided website.
         
         Args:
             question (str): The question to answer.
             url (str): The url of the website to read.
-            history (list, optional): The history of the conversation. Defaults to None. Added before question.
+            history (list, optional): A list of previous chat messages in openai format. Defaults to None.
         """
         if llm_has_ask(self.llm) is False:
             return None
 
         website_content = read_website(url)
         
         if website_content is None:
@@ -389,47 +466,50 @@
         prompts.append(syst_prompt)
         if history is not None:
             prompts.extend(history)
 
         user_prompt = make_prompt("user", question)
         prompts.append(user_prompt)
         
-        response = self.llm.ask(prompts)
+        response = self.llm.ask(prompts, temperature=self.temperature)
         self.chat_history.append(user_prompt)
         self.chat_history.append(make_prompt("assistant", response))
         return response
     
 
 class OnlineAgent:
     """
     An agent that has internet access. 
-    It will use the internet to try and best answer the user prompt
+    It will use the internet to try and best answer the user prompt.
     """
 
-    def __init__(self, llm:object, additional_system_instructions:str="", custom_searcher:callable=None, custom_site_reader:callable=None):
+    def __init__(self, llm:object, additional_system_instructions:str="", custom_searcher:callable=None, custom_site_reader:callable=None, temperature:float=0.8):
         """
         Args:
             llm (object): An LLM object. Must have an ask method.
             additional_system_instructions (str, optional): Instructions in addition to the system prompt. Defaults to "".
             custom_searcher (function, optional): A custom online searcher function. The searcher function must take a query and return a list of string URLS
             custom_site_reader (function, optional): A custom online site reader function. The site reader function must take a URL and return a string representation of the site.
+            temperature (float, optional): The temperature of the LLM. Defaults to 0.8.
         """
         self.llm = llm
         self.chat_history = []
         self.system_prompt = get_yaml_prompt("system_prompts.yaml", "OnlineSearcher")
         self.system_prompt = make_prompt("system", self.system_prompt.format(additional_instructions=additional_system_instructions))
         self.search_function = custom_searcher if custom_searcher else internet_search
         self.site_reader_function = custom_site_reader if custom_site_reader else read_website
+        self.temperature = temperature
 
     def search(self, prompt, history:list=None):
         """
         Searches the internet and answers the prompt based on the search results.
 
         Parameters:
             prompt (str): The prompt or question to answer.
+            history (list, optional): A list of previous chat messages in openai format. Defaults to None.
 
         Returns:
             str: The response that answers the prompt.
         """
 
         # Will first get a good search query
         # The query will be used to find relevant URLS
@@ -447,15 +527,15 @@
             url_picker_prompts.extend(history)
 
         # Use system prompt as user, since we have chat history
         url_picker_prompt = get_yaml_prompt("system_prompts.yaml", "UrlPicker")
         url_picker_prompt = make_prompt("user", url_picker_prompt.format(question=prompt, urls=search_results))
         url_picker_prompts.append(url_picker_prompt)
 
-        resp = self.llm.ask(url_picker_prompts, format="json")
+        resp = self.llm.ask(url_picker_prompts, format="json", temperature=self.temperature)
         resp_json = safe_read_json(resp)
 
         self.chat_history.append(url_picker_prompt)
         self.chat_history.append(make_prompt("assistant", resp))
 
         # Check if the response is a valid url
         url = None
@@ -485,15 +565,15 @@
         self.chat_history.append(make_prompt("assistant", response))
         
         return response
 
     def get_search_query(self, question):
         user_prompt = make_prompt("user", question)
         prompts = [self.system_prompt, user_prompt]
-        response = self.llm.ask(prompts, format="json")
+        response = self.llm.ask(prompts, format="json", temperature=self.temperature)
         response_json = safe_read_json(response)
         self.chat_history.append(prompts[1])
         self.chat_history.append(make_prompt("assistant", response))
         if response_json is not None and "search_query" in response_json:
             return response_json["search_query"]
         else:
             return None
```

### Comparing `llm_axe-1.0.9/llm_axe/core.py` & `llm_axe-1.1.0/llm_axe/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,16 +24,23 @@
 def llm_has_ask(llm):
     if not hasattr(llm, "ask"):
             warnings.warn("llm object must have an ask function! See OllamaChat class in models.py for an example.")
             return False
     return True
 
 
-def make_prompt(role:str, content:str):
-    return {"role": role, "content": content}
+def make_prompt(role:str, content:str, images:list=None):
+    args={
+        "role": role,
+        "content": content
+    }
+    if images is not None:
+        args["images"] = images
+
+    return {**args}
 
 
 def read_pdf(file):
     """
     Reads a pdf file and returns the complete text content.
     Args:
         file (str): The path to the pdf file.
```

### Comparing `llm_axe-1.0.9/llm_axe/system_prompts.yaml` & `llm_axe-1.1.0/llm_axe/system_prompts.yaml`

 * *Files 13% similar despite different names*

```diff
@@ -218,8 +218,32 @@
         Do NOT explain your response.
         
         Your response must be in json format.
 
         Example Response:
         {
             "libraries": ["library1", "library2", "library3"]
-        }
+        }
+
+ObjectDetector:
+    prompt: |
+        You are a professional object detector. 
+        Make a list of ALL objects found in images and give your reasoning as to where it is.
+        If you are uncertain about the object, then do not include it in the list.
+
+        Example Response:
+            I found these objects in the image:
+            obj1: Its next to the table
+            obj2: Its on the ground
+
+ObjectFilterer:
+    prompt: |
+        You are a professional object filterer. 
+        The user will give you objects they are interested in, and you will return ONLY those objects that are also found in the image.
+
+        Simplify the object names to one or two words MAX.
+
+        Example Information:
+        I found these objects:obj1: Its next to the table obj2: Its on the ground. There was no cat though.
+
+        Example Response:
+        {objects: ["obj1", "obj2"]}
```

### Comparing `llm_axe-1.0.9/llm_axe.egg-info/PKG-INFO` & `llm_axe-1.1.0/llm_axe.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llm-axe
-Version: 1.0.9
+Version: 1.1.0
 Summary: A toolkit for quickly implementing llm powered functionalities.
 Author: Emir Sahin
 Author-email: emirsah122@gmail.com
 License: MIT
 Keywords: python,llm axe,llm toolkit,local llm,local llm internet,function caller llm,ollama
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `llm_axe-1.0.9/setup.py` & `llm_axe-1.1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '1.0.9' 
+VERSION = '1.1.0' 
 DESCRIPTION = 'A toolkit for quickly implementing llm powered functionalities.'
 LONG_DESCRIPTION = '''
 # llm-axe 🪓
 
 <img alt="PyPI - Version" src="https://img.shields.io/pypi/v/llm-axe"> <img alt="PyPI - Downloads" src="https://img.shields.io/pypi/dm/llm-axe">
 <img alt="Static Badge" src="https://img.shields.io/badge/clones-63/month-purple"> <img alt="GitHub forks" src="https://img.shields.io/github/forks/emirsahin1/llm-axe?style=flat">
 [![Hits](https://hits.seeyoufarm.com/api/count/incr/badge.svg?url=https%3A%2F%2Fgithub.com%2Femirsahin1%2Fllm-axe&count_bg=%2379C83D&title_bg=%23555555&icon=&icon_color=%23E7E7E7&title=hits&edge_flat=false)](https://github.com/emirsahin1/llm-axe)
```

