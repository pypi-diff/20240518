# Comparing `tmp/WrenchCL-2.1.2.tar.gz` & `tmp/WrenchCL-2.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "WrenchCL-2.1.2.tar", last modified: Fri May 17 20:09:59 2024, max compression
+gzip compressed data, was "WrenchCL-2.1.3.tar", last modified: Sat May 18 04:48:18 2024, max compression
```

## Comparing `WrenchCL-2.1.2.tar` & `WrenchCL-2.1.3.tar`

### file list

```diff
@@ -1,49 +1,50 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 20:09:59.048343 WrenchCL-2.1.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1421 2024-05-17 20:09:37.000000 WrenchCL-2.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    22877 2024-05-17 20:09:59.048343 WrenchCL-2.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    22207 2024-05-17 20:09:37.000000 WrenchCL-2.1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 20:09:59.040343 WrenchCL-2.1.2/WrenchCL/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 20:09:59.044343 WrenchCL-2.1.2/WrenchCL/Connect/
--rw-r--r--   0 runner    (1001) docker     (127)    10104 2024-05-17 20:09:37.000000 WrenchCL-2.1.2/WrenchCL/Connect/AwsClientHub.py
--rw-r--r--   0 runner    (1001) docker     (127)     8307 2024-05-17 20:09:37.000000 WrenchCL-2.1.2/WrenchCL/Connect/RdsServiceGateway.py
--rw-r--r--   0 runner    (1001) docker     (127)    10985 2024-05-17 20:09:37.000000 WrenchCL-2.1.2/WrenchCL/Connect/S3ServiceGateway.py
--rw-r--r--   0 runner    (1001) docker     (127)      236 2024-05-17 20:09:37.000000 WrenchCL-2.1.2/WrenchCL/Connect/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 20:09:59.044343 WrenchCL-2.1.2/WrenchCL/DataFlow/
--rw-r--r--   0 runner    (1001) docker     (127)      412 2024-05-17 20:09:37.000000 WrenchCL-2.1.2/WrenchCL/DataFlow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2954 2024-05-17 20:09:37.000000 WrenchCL-2.1.2/WrenchCL/DataFlow/build_return_json.py
--rw-r--r--   0 runner    (1001) docker     (127)     9123 2024-05-17 20:09:37.000000 WrenchCL-2.1.2/WrenchCL/DataFlow/handle_lambda_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    10837 2024-05-17 20:09:37.000000 WrenchCL-2.1.2/WrenchCL/DataFlow/trigger_dataflow_metrics.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 20:09:59.044343 WrenchCL-2.1.2/WrenchCL/Decorators/
--rw-r--r--   0 runner    (1001) docker     (127)     3656 2024-05-17 20:09:37.000000 WrenchCL-2.1.2/WrenchCL/Decorators/Retryable.py
--rw-r--r--   0 runner    (1001) docker     (127)     3116 2024-05-17 20:09:37.000000 WrenchCL-2.1.2/WrenchCL/Decorators/SingletonClass.py
--rw-r--r--   0 runner    (1001) docker     (127)     2541 2024-05-17 20:09:37.000000 WrenchCL-2.1.2/WrenchCL/Decorators/TimedMethod.py
--rw-r--r--   0 runner    (1001) docker     (127)      206 2024-05-17 20:09:37.000000 WrenchCL-2.1.2/WrenchCL/Decorators/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 20:09:59.044343 WrenchCL-2.1.2/WrenchCL/Models/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 20:09:59.044343 WrenchCL-2.1.2/WrenchCL/Models/OpenAI/
--rw-r--r--   0 runner    (1001) docker     (127)     4853 2024-05-17 20:09:37.000000 WrenchCL-2.1.2/WrenchCL/Models/OpenAI/OpenAIFactory.py
--rw-r--r--   0 runner    (1001) docker     (127)    15468 2024-05-17 20:09:37.000000 WrenchCL-2.1.2/WrenchCL/Models/OpenAI/OpenAIGateway.py
--rw-r--r--   0 runner    (1001) docker     (127)     7292 2024-05-17 20:09:37.000000 WrenchCL-2.1.2/WrenchCL/Models/OpenAI/_ConversationManager.py
--rw-r--r--   0 runner    (1001) docker     (127)     1651 2024-05-17 20:09:37.000000 WrenchCL-2.1.2/WrenchCL/Models/OpenAI/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-17 20:09:37.000000 WrenchCL-2.1.2/WrenchCL/Models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 20:09:59.048343 WrenchCL-2.1.2/WrenchCL/Tools/
--rw-r--r--   0 runner    (1001) docker     (127)     2196 2024-05-17 20:09:37.000000 WrenchCL-2.1.2/WrenchCL/Tools/Coalesce.py
--rw-r--r--   0 runner    (1001) docker     (127)     5888 2024-05-17 20:09:37.000000 WrenchCL-2.1.2/WrenchCL/Tools/DictValidator.py
--rw-r--r--   0 runner    (1001) docker     (127)     3233 2024-05-17 20:09:37.000000 WrenchCL-2.1.2/WrenchCL/Tools/FetchMetaData.py
--rw-r--r--   0 runner    (1001) docker     (127)     2661 2024-05-17 20:09:37.000000 WrenchCL-2.1.2/WrenchCL/Tools/FileTyper.py
--rw-r--r--   0 runner    (1001) docker     (127)     2485 2024-05-17 20:09:37.000000 WrenchCL-2.1.2/WrenchCL/Tools/Image2B64.py
--rw-r--r--   0 runner    (1001) docker     (127)     5414 2024-05-17 20:09:37.000000 WrenchCL-2.1.2/WrenchCL/Tools/MaybeMonad.py
--rw-r--r--   0 runner    (1001) docker     (127)    28041 2024-05-17 20:09:37.000000 WrenchCL-2.1.2/WrenchCL/Tools/WrenchLogger.py
--rw-r--r--   0 runner    (1001) docker     (127)      404 2024-05-17 20:09:37.000000 WrenchCL-2.1.2/WrenchCL/Tools/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 20:09:59.048343 WrenchCL-2.1.2/WrenchCL/_Internal/
--rw-r--r--   0 runner    (1001) docker     (127)     6964 2024-05-17 20:09:37.000000 WrenchCL-2.1.2/WrenchCL/_Internal/_ConfigurationManager.py
--rw-r--r--   0 runner    (1001) docker     (127)     4086 2024-05-17 20:09:37.000000 WrenchCL-2.1.2/WrenchCL/_Internal/_SshTunnelManager.py
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-17 20:09:37.000000 WrenchCL-2.1.2/WrenchCL/_Internal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       92 2024-05-17 20:09:37.000000 WrenchCL-2.1.2/WrenchCL/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 20:09:59.044343 WrenchCL-2.1.2/WrenchCL.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    22877 2024-05-17 20:09:59.000000 WrenchCL-2.1.2/WrenchCL.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1179 2024-05-17 20:09:59.000000 WrenchCL-2.1.2/WrenchCL.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-17 20:09:59.000000 WrenchCL-2.1.2/WrenchCL.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      264 2024-05-17 20:09:59.000000 WrenchCL-2.1.2/WrenchCL.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-17 20:09:59.000000 WrenchCL-2.1.2/WrenchCL.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-17 20:09:59.048343 WrenchCL-2.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1938 2024-05-17 20:09:57.000000 WrenchCL-2.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 04:48:18.604204 WrenchCL-2.1.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1421 2024-05-18 04:47:56.000000 WrenchCL-2.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    23514 2024-05-18 04:48:18.604204 WrenchCL-2.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    22844 2024-05-18 04:47:56.000000 WrenchCL-2.1.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 04:48:18.600204 WrenchCL-2.1.3/WrenchCL/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 04:48:18.600204 WrenchCL-2.1.3/WrenchCL/Connect/
+-rw-r--r--   0 runner    (1001) docker     (127)    11060 2024-05-18 04:47:56.000000 WrenchCL-2.1.3/WrenchCL/Connect/AwsClientHub.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9226 2024-05-18 04:47:56.000000 WrenchCL-2.1.3/WrenchCL/Connect/RdsServiceGateway.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10985 2024-05-18 04:47:56.000000 WrenchCL-2.1.3/WrenchCL/Connect/S3ServiceGateway.py
+-rw-r--r--   0 runner    (1001) docker     (127)      236 2024-05-18 04:47:56.000000 WrenchCL-2.1.3/WrenchCL/Connect/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 04:48:18.604204 WrenchCL-2.1.3/WrenchCL/DataFlow/
+-rw-r--r--   0 runner    (1001) docker     (127)      412 2024-05-18 04:47:56.000000 WrenchCL-2.1.3/WrenchCL/DataFlow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2729 2024-05-18 04:47:56.000000 WrenchCL-2.1.3/WrenchCL/DataFlow/build_return_json.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10159 2024-05-18 04:47:56.000000 WrenchCL-2.1.3/WrenchCL/DataFlow/handle_lambda_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10837 2024-05-18 04:47:56.000000 WrenchCL-2.1.3/WrenchCL/DataFlow/trigger_dataflow_metrics.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 04:48:18.604204 WrenchCL-2.1.3/WrenchCL/Decorators/
+-rw-r--r--   0 runner    (1001) docker     (127)     3656 2024-05-18 04:47:56.000000 WrenchCL-2.1.3/WrenchCL/Decorators/Retryable.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3116 2024-05-18 04:47:56.000000 WrenchCL-2.1.3/WrenchCL/Decorators/SingletonClass.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2541 2024-05-18 04:47:56.000000 WrenchCL-2.1.3/WrenchCL/Decorators/TimedMethod.py
+-rw-r--r--   0 runner    (1001) docker     (127)      206 2024-05-18 04:47:56.000000 WrenchCL-2.1.3/WrenchCL/Decorators/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 04:48:18.604204 WrenchCL-2.1.3/WrenchCL/Models/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 04:48:18.604204 WrenchCL-2.1.3/WrenchCL/Models/OpenAI/
+-rw-r--r--   0 runner    (1001) docker     (127)     4856 2024-05-18 04:47:56.000000 WrenchCL-2.1.3/WrenchCL/Models/OpenAI/OpenAIFactory.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16033 2024-05-18 04:47:56.000000 WrenchCL-2.1.3/WrenchCL/Models/OpenAI/OpenAIGateway.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7292 2024-05-18 04:47:56.000000 WrenchCL-2.1.3/WrenchCL/Models/OpenAI/_ConversationManager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1651 2024-05-18 04:47:56.000000 WrenchCL-2.1.3/WrenchCL/Models/OpenAI/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-18 04:47:56.000000 WrenchCL-2.1.3/WrenchCL/Models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 04:48:18.604204 WrenchCL-2.1.3/WrenchCL/Tools/
+-rw-r--r--   0 runner    (1001) docker     (127)     2196 2024-05-18 04:47:56.000000 WrenchCL-2.1.3/WrenchCL/Tools/Coalesce.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5888 2024-05-18 04:47:56.000000 WrenchCL-2.1.3/WrenchCL/Tools/DictValidator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3279 2024-05-18 04:47:56.000000 WrenchCL-2.1.3/WrenchCL/Tools/FetchMetaData.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2707 2024-05-18 04:47:56.000000 WrenchCL-2.1.3/WrenchCL/Tools/FileTyper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2485 2024-05-18 04:47:56.000000 WrenchCL-2.1.3/WrenchCL/Tools/Image2B64.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3546 2024-05-18 04:47:56.000000 WrenchCL-2.1.3/WrenchCL/Tools/JsonSerializer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5414 2024-05-18 04:47:56.000000 WrenchCL-2.1.3/WrenchCL/Tools/MaybeMonad.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31356 2024-05-18 04:47:56.000000 WrenchCL-2.1.3/WrenchCL/Tools/WrenchLogger.py
+-rw-r--r--   0 runner    (1001) docker     (127)      471 2024-05-18 04:47:56.000000 WrenchCL-2.1.3/WrenchCL/Tools/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 04:48:18.604204 WrenchCL-2.1.3/WrenchCL/_Internal/
+-rw-r--r--   0 runner    (1001) docker     (127)     7429 2024-05-18 04:47:56.000000 WrenchCL-2.1.3/WrenchCL/_Internal/_ConfigurationManager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4086 2024-05-18 04:47:56.000000 WrenchCL-2.1.3/WrenchCL/_Internal/_SshTunnelManager.py
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-18 04:47:56.000000 WrenchCL-2.1.3/WrenchCL/_Internal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-05-18 04:47:56.000000 WrenchCL-2.1.3/WrenchCL/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 04:48:18.600204 WrenchCL-2.1.3/WrenchCL.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    23514 2024-05-18 04:48:18.000000 WrenchCL-2.1.3/WrenchCL.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1212 2024-05-18 04:48:18.000000 WrenchCL-2.1.3/WrenchCL.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-18 04:48:18.000000 WrenchCL-2.1.3/WrenchCL.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      408 2024-05-18 04:48:18.000000 WrenchCL-2.1.3/WrenchCL.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-18 04:48:18.000000 WrenchCL-2.1.3/WrenchCL.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-18 04:48:18.604204 WrenchCL-2.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1959 2024-05-18 04:48:16.000000 WrenchCL-2.1.3/setup.py
```

### Comparing `WrenchCL-2.1.2/LICENSE` & `WrenchCL-2.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `WrenchCL-2.1.2/PKG-INFO` & `WrenchCL-2.1.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: WrenchCL
-Version: 2.1.2
+Version: 2.1.3
 Summary: WrenchCL is a comprehensive library designed to facilitate seamless interactions with AWS services, OpenAI models, and various utility tools. This package aims to streamline the development process by providing robust components for database interactions, cloud storage, and AI-powered functionalities.
 Home-page: https://github.com/WrenchAI/WrenchCL
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
@@ -52,15 +52,16 @@
 ```bash
 ImportError: failed to find libmagic.  Check your installation
 ```
 
 Install the package with the optional libmagic dependency, users can using the following command:
 
 ```bash
-pip install WrenchCL[libmagic]
+1. pip uninstall python-magic -y
+2. pip install WrenchCL[libmagic]
 ```
 
 
 # User Guides
 
 Sure! Here's an updated and more detailed README that provides extensive instructions on how to use `AWSClientHub`, `RdsServiceGateway`, `S3ServiceGateway`, `ConversationManager`, `OpenAIFactory`, and `OpenAIGateway`. It also includes practical examples for the `Maybe` monad and other utility tools.
 
@@ -88,15 +89,15 @@
    # Example: Fetching data from the database
    query = "SELECT * FROM your_table"
    data = rds_service.get_data(query)
    print(data)
    ```
 
    **Methods in `RdsServiceGateway`**:
-   - `get_data(query: str, payload: Optional[dict] = None, fetchall: bool = True, accepted_type: Optional[Type] = None, none_is_ok: bool = False, accepted_length: Tuple[Optional[int], Optional[int]] = (None, None)) -> Optional[Any]`
+   - `get_data(query: str, payload: Optional[dict] = None, fetchall: bool = True, return_dict: bool = True, accepted_type: Optional[Type] = None, none_is_ok: bool = False, accepted_length: Tuple[Optional[int], Optional[int]] = (None, None)) -> Optional[Any]`
      - Fetches data from the database based on the input query and parameters.
    - `update_database(query: str, payload: Union[dict, 'pd.DataFrame'], column_order: Optional[List[str]] = None) -> None`
      - Updates the database by executing the given query with the provided payload.
 
 3. **Using `S3ServiceGateway`**:
    ```python
    from WrenchCL.Connect import S3ServiceGateway
@@ -142,36 +143,36 @@
    ```python
    from WrenchCL.Models.OpenAI import OpenAIGateway
 
    # Initialize OpenAIGateway with your OpenAI API key
    openai_gateway = OpenAIGateway(api_key="your_openai_api_key")
 
    # Example: Generating text
-   response = openai_gateway.handle_text("Your prompt here")
+   response = openai_gateway.text_response("Your prompt here")
    print(response)
    ```
 
    **Methods in `OpenAIGateway`**:
-   - `handle_text(text: str, model: str = "gpt-3.5-turbo", system_prompt: Optional[str] = None, image_url: Optional[str] = None, json_mode: bool = False, **kwargs) -> Union[str, dict]`
+   - `text_response(text: str, model: str = "gpt-3.5-turbo", system_prompt: Optional[str] = None, image_url: Optional[str] = None, json_mode: bool = False,  stream : bool = False, **kwargs) -> Union[str, dict]`
      - Processes text input using the specified model and returns the response.
    - `get_embeddings(text: str, model: str = "text-embedding-3-small") -> list`
      - Retrieves embeddings for the given text using the specified model.
-   - `generate_image(prompt: str, size: str = "1024x1024", quality: str = "standard", n: int = 1) -> str`
+   - `text_to_image(prompt: str, size: str = "1024x1024", quality: str = "standard", n: int = 1) -> str`
      - Generates an image based on the provided prompt.
-   - `process_audio(audio_path: str, model: str = "whisper-1") -> str`
+   - `audio_to_text(audio_path: str, model: str = "whisper-1") -> str`
      - Processes an audio file and returns its transcription.
-   - `create_image_variation(image_path: str, n: int = 1, size: str = "1024x1024") -> str`
+   - `generate_image_variations(image_path: str, n: int = 1, size: str = "1024x1024") -> str`
      - Creates variations of an image based on the provided image path.
-   - `edit_image(image_path: str, prompt: str, mask_path: str, n: int = 1, size: str = "1024x1024") -> str`
+   - `modify_image(image_path: str, prompt: str, mask_path: str, n: int = 1, size: str = "1024x1024") -> str`
      - Edits an image based on the provided prompt and mask.
-   - `vision_query(question: str, image_path: str, **kwargs) -> dict`
+   - `image_to_text(question: str, image_path: str, **kwargs) -> dict`
      - Processes a vision query based on the provided question and image.
    - `convert_image_to_url_or_base64(image_path: str) -> str`
      - Converts an image to a URL or base64 encoded string.
-   - `initiate_conversation(initial_text: str, **kwargs)`
+   - `start_conversation(initial_text: str, **kwargs)`
      - Initiates a conversation using the provided initial text.
 
 2. **Using `OpenAIFactory`**:
    ```python
    from WrenchCL.Models.OpenAI import OpenAIFactory
 
    # Initialize OpenAIFactory with your OpenAI API key
@@ -191,14 +192,30 @@
    - `validate_response_with_gpt(initial_response: str, validation_prompt: str) -> str`
      - Uses an initial response and validates or expands upon it with a secondary GPT call.
 
 ### Utility Tools
 
 WrenchCL includes several utility tools for various purposes:
 
+Got it! Here is the section about the custom JSON serializer in the specified format:
+
+### Custom JSON Serializer
+
+- **robust_serializer**: Serializes objects not natively serializable by JSON, including `datetime`, `date`, `Decimal`, and custom objects.
+
+    ```python
+    # Usage with json_dumps
+    from datetime import datetime
+    import json
+    from WrenchCL.Tools import robust_serializer
+
+    print(json.dumps({"timestamp": datetime.now()}, default=robust_serializer))
+    # Output: {"timestamp": "2024-05-17T12:34:56.789012"}
+    ```
+
 - **validate_input_dict**: Validates the input dictionary against expected types.
   ```python
   from WrenchCL.Tools import validate_input_dict
     
   params = {
         'event': 'event_data',
         'context': 'context_data',
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: WrenchCL Version: 2.1.2 Summary: WrenchCL is a
+Metadata-Version: 2.1 Name: WrenchCL Version: 2.1.3 Summary: WrenchCL is a
 comprehensive library designed to facilitate seamless interactions with AWS
 services, OpenAI models, and various utility tools. This package aims to
 streamline the development process by providing robust components for database
 interactions, cloud storage, and AI-powered functionalities. Home-page: https:/
 /github.com/WrenchAI/WrenchCL Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License Classifier: Operating System
 :: OS Independent Requires-Python: >=3.11 Description-Content-Type: text/
@@ -21,42 +21,43 @@
 _Internal for interacting with OpenAI models. - **Tools**: Miscellaneous
 utility tools such as coalescing values, file typing, image encoding, and a
 custom logger. - **DataFlow**: Response focused tools to aid in returning
 values and generating logs based on status codes. ## Installation To install
 the package, simply run the following command: ```bash pip install WrenchCL ```
 Upon recieving the below error: ```bash ImportError: failed to find libmagic.
 Check your installation ``` Install the package with the optional libmagic
-dependency, users can using the following command: ```bash pip install WrenchCL
-[libmagic] ``` # User Guides Sure! Here's an updated and more detailed README
-that provides extensive instructions on how to use `AWSClientHub`,
-`RdsServiceGateway`, `S3ServiceGateway`, `ConversationManager`,
-`OpenAIFactory`, and `OpenAIGateway`. It also includes practical examples for
-the `Maybe` monad and other utility tools. ### Connecting to AWS Services To
-interact with AWS RDS and S3 services, follow these steps: 1. **Setup
-`AWSClientHub`**: ```python from WrenchCL.Connections import AwsClientHub #
-Initialize the AWSClientHub using an env file or keyword arguments
-aws_client_hub = AWSClientHub(env_path="path/to/your/env/file") #
+dependency, users can using the following command: ```bash 1. pip uninstall
+python-magic -y 2. pip install WrenchCL[libmagic] ``` # User Guides Sure!
+Here's an updated and more detailed README that provides extensive instructions
+on how to use `AWSClientHub`, `RdsServiceGateway`, `S3ServiceGateway`,
+`ConversationManager`, `OpenAIFactory`, and `OpenAIGateway`. It also includes
+practical examples for the `Maybe` monad and other utility tools. ###
+Connecting to AWS Services To interact with AWS RDS and S3 services, follow
+these steps: 1. **Setup `AWSClientHub`**: ```python from WrenchCL.Connections
+import AwsClientHub # Initialize the AWSClientHub using an env file or keyword
+arguments aws_client_hub = AWSClientHub(env_path="path/to/your/env/file") #
 Alternatively, use keyword arguments or existing env variables # aws_client_hub
 = AWSClientHub(aws_profile='your_profile', region_name='your_region',
 secret_arn='your_secret_arn', ...) ``` 2. **Using `RdsServiceGateway`**:
 ```python from WrenchCL.Connections import RdsServiceGateway # Initialize
 RdsServiceGateway with the AWSClientHub instance rds_service =
 RdsServiceGateway(aws_client_hub) # Example: Fetching data from the database
 query = "SELECT * FROM your_table" data = rds_service.get_data(query) print
 (data) ``` **Methods in `RdsServiceGateway`**: - `get_data(query: str, payload:
-Optional[dict] = None, fetchall: bool = True, accepted_type: Optional[Type] =
-None, none_is_ok: bool = False, accepted_length: Tuple[Optional[int], Optional
-[int]] = (None, None)) -> Optional[Any]` - Fetches data from the database based
-on the input query and parameters. - `update_database(query: str, payload:
-Union[dict, 'pd.DataFrame'], column_order: Optional[List[str]] = None) -> None`
-- Updates the database by executing the given query with the provided payload.
-3. **Using `S3ServiceGateway`**: ```python from WrenchCL.Connect import
-S3ServiceGateway # Initialize S3ServiceGateway with the AWSClientHub instance
-s3_service = S3ServiceGateway(aws_client_hub) # Example: Downloading an object
-from S3 bucket_name = "your-bucket-name" object_key = "path/to/your/object"
+Optional[dict] = None, fetchall: bool = True, return_dict: bool = True,
+accepted_type: Optional[Type] = None, none_is_ok: bool = False,
+accepted_length: Tuple[Optional[int], Optional[int]] = (None, None)) -
+> Optional[Any]` - Fetches data from the database based on the input query and
+parameters. - `update_database(query: str, payload: Union[dict,
+'pd.DataFrame'], column_order: Optional[List[str]] = None) -> None` - Updates
+the database by executing the given query with the provided payload. 3. **Using
+`S3ServiceGateway`**: ```python from WrenchCL.Connect import S3ServiceGateway #
+Initialize S3ServiceGateway with the AWSClientHub instance s3_service =
+S3ServiceGateway(aws_client_hub) # Example: Downloading an object from S3
+bucket_name = "your-bucket-name" object_key = "path/to/your/object"
 s3_service.download_object(bucket_name, object_key, "local/path/to/save") ```
 **Methods in `S3ServiceGateway`**: - `get_object(bucket_name: str, object_key:
 str) -> io.BytesIO` - Retrieves an object from S3. - `download_object
 (bucket_name: str, object_key: str, local_path: str) -> None` - Downloads an
 object from S3 to the local file system. - `get_object_headers(bucket_name:
 str, object_key: str) -> dict` - Retrieves the headers of an object in S3. -
 `upload_object(file_path: str, bucket_name: str, object_key: str) -> None` -
@@ -72,52 +73,60 @@
 an object exists in S3. - `list_objects(bucket_name: str, prefix: Optional[str]
 = None) -> list` - Lists objects in an S3 bucket. - `check_bucket_permissions
 (bucket_name: str) -> dict` - Checks the permissions of an S3 bucket. ###
 Interacting with OpenAI Models To use OpenAI models, follow these steps: 1.
 **Setup `OpenAIGateway`**: ```python from WrenchCL.Models.OpenAI import
 OpenAIGateway # Initialize OpenAIGateway with your OpenAI API key
 openai_gateway = OpenAIGateway(api_key="your_openai_api_key") # Example:
-Generating text response = openai_gateway.handle_text("Your prompt here") print
-(response) ``` **Methods in `OpenAIGateway`**: - `handle_text(text: str, model:
-str = "gpt-3.5-turbo", system_prompt: Optional[str] = None, image_url: Optional
-[str] = None, json_mode: bool = False, **kwargs) -> Union[str, dict]` -
-Processes text input using the specified model and returns the response. -
-`get_embeddings(text: str, model: str = "text-embedding-3-small") -> list` -
-Retrieves embeddings for the given text using the specified model. -
-`generate_image(prompt: str, size: str = "1024x1024", quality: str =
-"standard", n: int = 1) -> str` - Generates an image based on the provided
-prompt. - `process_audio(audio_path: str, model: str = "whisper-1") -> str` -
-Processes an audio file and returns its transcription. -
-`create_image_variation(image_path: str, n: int = 1, size: str = "1024x1024") -
-> str` - Creates variations of an image based on the provided image path. -
-`edit_image(image_path: str, prompt: str, mask_path: str, n: int = 1, size: str
-= "1024x1024") -> str` - Edits an image based on the provided prompt and mask.
-- `vision_query(question: str, image_path: str, **kwargs) -> dict` - Processes
-a vision query based on the provided question and image. -
-`convert_image_to_url_or_base64(image_path: str) -> str` - Converts an image to
-a URL or base64 encoded string. - `initiate_conversation(initial_text: str,
-**kwargs)` - Initiates a conversation using the provided initial text. 2.
-**Using `OpenAIFactory`**: ```python from WrenchCL.Models.OpenAI import
-OpenAIFactory # Initialize OpenAIFactory with your OpenAI API key
-openai_factory = OpenAIFactory(api_key="your_openai_api_key") # Example:
-Transcribing audio to text and getting embeddings audio_path = "path/to/your/
-audio/file" embeddings = openai_factory.audio_to_text_to_embeddings(audio_path)
-print(embeddings) ``` **Methods in `OpenAIFactory`**: -
-`audio_to_text_to_embeddings(audio_path: str, embedding_model: str = "text-
-embedding-3-small") -> list` - Transcribes audio to text and then generates
-embeddings for the text. - `image_to_text_to_embeddings(image_path: str,
-question: str, embedding_model: str = "text-embedding-3-small") -> list` -
-Performs a vision query to understand an image and then generates embeddings
-for the response. - `validate_response_with_gpt(initial_response: str,
-validation_prompt: str) -> str` - Uses an initial response and validates or
-expands upon it with a secondary GPT call. ### Utility Tools WrenchCL includes
-several utility tools for various purposes: - **validate_input_dict**:
-Validates the input dictionary against expected types. ```python from
-WrenchCL.Tools import validate_input_dict params = { 'event': 'event_data',
-'context': 'context_data', 'start_time': 1625256000, 'lambda_client':
+Generating text response = openai_gateway.text_response("Your prompt here")
+print(response) ``` **Methods in `OpenAIGateway`**: - `text_response(text: str,
+model: str = "gpt-3.5-turbo", system_prompt: Optional[str] = None, image_url:
+Optional[str] = None, json_mode: bool = False, stream : bool = False, **kwargs)
+-> Union[str, dict]` - Processes text input using the specified model and
+returns the response. - `get_embeddings(text: str, model: str = "text-
+embedding-3-small") -> list` - Retrieves embeddings for the given text using
+the specified model. - `text_to_image(prompt: str, size: str = "1024x1024",
+quality: str = "standard", n: int = 1) -> str` - Generates an image based on
+the provided prompt. - `audio_to_text(audio_path: str, model: str = "whisper-
+1") -> str` - Processes an audio file and returns its transcription. -
+`generate_image_variations(image_path: str, n: int = 1, size: str =
+"1024x1024") -> str` - Creates variations of an image based on the provided
+image path. - `modify_image(image_path: str, prompt: str, mask_path: str, n:
+int = 1, size: str = "1024x1024") -> str` - Edits an image based on the
+provided prompt and mask. - `image_to_text(question: str, image_path: str,
+**kwargs) -> dict` - Processes a vision query based on the provided question
+and image. - `convert_image_to_url_or_base64(image_path: str) -> str` -
+Converts an image to a URL or base64 encoded string. - `start_conversation
+(initial_text: str, **kwargs)` - Initiates a conversation using the provided
+initial text. 2. **Using `OpenAIFactory`**: ```python from
+WrenchCL.Models.OpenAI import OpenAIFactory # Initialize OpenAIFactory with
+your OpenAI API key openai_factory = OpenAIFactory
+(api_key="your_openai_api_key") # Example: Transcribing audio to text and
+getting embeddings audio_path = "path/to/your/audio/file" embeddings =
+openai_factory.audio_to_text_to_embeddings(audio_path) print(embeddings) ```
+**Methods in `OpenAIFactory`**: - `audio_to_text_to_embeddings(audio_path: str,
+embedding_model: str = "text-embedding-3-small") -> list` - Transcribes audio
+to text and then generates embeddings for the text. -
+`image_to_text_to_embeddings(image_path: str, question: str, embedding_model:
+str = "text-embedding-3-small") -> list` - Performs a vision query to
+understand an image and then generates embeddings for the response. -
+`validate_response_with_gpt(initial_response: str, validation_prompt: str) -
+> str` - Uses an initial response and validates or expands upon it with a
+secondary GPT call. ### Utility Tools WrenchCL includes several utility tools
+for various purposes: Got it! Here is the section about the custom JSON
+serializer in the specified format: ### Custom JSON Serializer -
+**robust_serializer**: Serializes objects not natively serializable by JSON,
+including `datetime`, `date`, `Decimal`, and custom objects. ```python # Usage
+with json_dumps from datetime import datetime import json from WrenchCL.Tools
+import robust_serializer print(json.dumps({"timestamp": datetime.now()},
+default=robust_serializer)) # Output: {"timestamp": "2024-05-17T12:34:
+56.789012"} ``` - **validate_input_dict**: Validates the input dictionary
+against expected types. ```python from WrenchCL.Tools import
+validate_input_dict params = { 'event': 'event_data', 'context':
+'context_data', 'start_time': 1625256000, 'lambda_client':
 'lambda_client_instance' } expected_types = { 'event': str, 'context': str,
 'start_time': (int, float), 'lambda_client': object, } validate_input_dict
 (params, expected_types) ``` - **Coalesce**: A utility function to return the
 first non-null value. ```python from WrenchCL.Tools import coalesce result =
 coalesce(None, "default_value") print(result) # Output: "default_value" ``` -
 **FileTyper**: A utility for determining file types. ```python from
 WrenchCL.Tools import get_file_type file_type = get_file_type("path/to/your/
```

### Comparing `WrenchCL-2.1.2/README.md` & `WrenchCL-2.1.3/WrenchCL.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,20 @@
+Metadata-Version: 2.1
+Name: WrenchCL
+Version: 2.1.3
+Summary: WrenchCL is a comprehensive library designed to facilitate seamless interactions with AWS services, OpenAI models, and various utility tools. This package aims to streamline the development process by providing robust components for database interactions, cloud storage, and AI-powered functionalities.
+Home-page: https://github.com/WrenchAI/WrenchCL
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.11
+Description-Content-Type: text/markdown
+Provides-Extra: libmagic
+License-File: LICENSE
+
 <h1 align="center">Wrench Code Library</h1>
 
 <p align="center">
     <img src="https://raw.githubusercontent.com/WrenchAI/WrenchCL/release/resources/img/logo.svg" alt="Logo" style="display: inline-block; vertical-align: middle; margin-bottom: -50px; width: 90%; max-width: 800px;">
     <a href="https://pypi.org/project/WrenchCL/" style="text-decoration: none;">
         <img alt="PyPI - Version" src="https://img.shields.io/pypi/v/WrenchCL?logo=pypi&logoColor=green&color=green">
     </a>
@@ -39,15 +52,16 @@
 ```bash
 ImportError: failed to find libmagic.  Check your installation
 ```
 
 Install the package with the optional libmagic dependency, users can using the following command:
 
 ```bash
-pip install WrenchCL[libmagic]
+1. pip uninstall python-magic -y
+2. pip install WrenchCL[libmagic]
 ```
 
 
 # User Guides
 
 Sure! Here's an updated and more detailed README that provides extensive instructions on how to use `AWSClientHub`, `RdsServiceGateway`, `S3ServiceGateway`, `ConversationManager`, `OpenAIFactory`, and `OpenAIGateway`. It also includes practical examples for the `Maybe` monad and other utility tools.
 
@@ -75,15 +89,15 @@
    # Example: Fetching data from the database
    query = "SELECT * FROM your_table"
    data = rds_service.get_data(query)
    print(data)
    ```
 
    **Methods in `RdsServiceGateway`**:
-   - `get_data(query: str, payload: Optional[dict] = None, fetchall: bool = True, accepted_type: Optional[Type] = None, none_is_ok: bool = False, accepted_length: Tuple[Optional[int], Optional[int]] = (None, None)) -> Optional[Any]`
+   - `get_data(query: str, payload: Optional[dict] = None, fetchall: bool = True, return_dict: bool = True, accepted_type: Optional[Type] = None, none_is_ok: bool = False, accepted_length: Tuple[Optional[int], Optional[int]] = (None, None)) -> Optional[Any]`
      - Fetches data from the database based on the input query and parameters.
    - `update_database(query: str, payload: Union[dict, 'pd.DataFrame'], column_order: Optional[List[str]] = None) -> None`
      - Updates the database by executing the given query with the provided payload.
 
 3. **Using `S3ServiceGateway`**:
    ```python
    from WrenchCL.Connect import S3ServiceGateway
@@ -129,36 +143,36 @@
    ```python
    from WrenchCL.Models.OpenAI import OpenAIGateway
 
    # Initialize OpenAIGateway with your OpenAI API key
    openai_gateway = OpenAIGateway(api_key="your_openai_api_key")
 
    # Example: Generating text
-   response = openai_gateway.handle_text("Your prompt here")
+   response = openai_gateway.text_response("Your prompt here")
    print(response)
    ```
 
    **Methods in `OpenAIGateway`**:
-   - `handle_text(text: str, model: str = "gpt-3.5-turbo", system_prompt: Optional[str] = None, image_url: Optional[str] = None, json_mode: bool = False, **kwargs) -> Union[str, dict]`
+   - `text_response(text: str, model: str = "gpt-3.5-turbo", system_prompt: Optional[str] = None, image_url: Optional[str] = None, json_mode: bool = False,  stream : bool = False, **kwargs) -> Union[str, dict]`
      - Processes text input using the specified model and returns the response.
    - `get_embeddings(text: str, model: str = "text-embedding-3-small") -> list`
      - Retrieves embeddings for the given text using the specified model.
-   - `generate_image(prompt: str, size: str = "1024x1024", quality: str = "standard", n: int = 1) -> str`
+   - `text_to_image(prompt: str, size: str = "1024x1024", quality: str = "standard", n: int = 1) -> str`
      - Generates an image based on the provided prompt.
-   - `process_audio(audio_path: str, model: str = "whisper-1") -> str`
+   - `audio_to_text(audio_path: str, model: str = "whisper-1") -> str`
      - Processes an audio file and returns its transcription.
-   - `create_image_variation(image_path: str, n: int = 1, size: str = "1024x1024") -> str`
+   - `generate_image_variations(image_path: str, n: int = 1, size: str = "1024x1024") -> str`
      - Creates variations of an image based on the provided image path.
-   - `edit_image(image_path: str, prompt: str, mask_path: str, n: int = 1, size: str = "1024x1024") -> str`
+   - `modify_image(image_path: str, prompt: str, mask_path: str, n: int = 1, size: str = "1024x1024") -> str`
      - Edits an image based on the provided prompt and mask.
-   - `vision_query(question: str, image_path: str, **kwargs) -> dict`
+   - `image_to_text(question: str, image_path: str, **kwargs) -> dict`
      - Processes a vision query based on the provided question and image.
    - `convert_image_to_url_or_base64(image_path: str) -> str`
      - Converts an image to a URL or base64 encoded string.
-   - `initiate_conversation(initial_text: str, **kwargs)`
+   - `start_conversation(initial_text: str, **kwargs)`
      - Initiates a conversation using the provided initial text.
 
 2. **Using `OpenAIFactory`**:
    ```python
    from WrenchCL.Models.OpenAI import OpenAIFactory
 
    # Initialize OpenAIFactory with your OpenAI API key
@@ -178,14 +192,30 @@
    - `validate_response_with_gpt(initial_response: str, validation_prompt: str) -> str`
      - Uses an initial response and validates or expands upon it with a secondary GPT call.
 
 ### Utility Tools
 
 WrenchCL includes several utility tools for various purposes:
 
+Got it! Here is the section about the custom JSON serializer in the specified format:
+
+### Custom JSON Serializer
+
+- **robust_serializer**: Serializes objects not natively serializable by JSON, including `datetime`, `date`, `Decimal`, and custom objects.
+
+    ```python
+    # Usage with json_dumps
+    from datetime import datetime
+    import json
+    from WrenchCL.Tools import robust_serializer
+
+    print(json.dumps({"timestamp": datetime.now()}, default=robust_serializer))
+    # Output: {"timestamp": "2024-05-17T12:34:56.789012"}
+    ```
+
 - **validate_input_dict**: Validates the input dictionary against expected types.
   ```python
   from WrenchCL.Tools import validate_input_dict
     
   params = {
         'event': 'event_data',
         'context': 'context_data',
```

#### html2text {}

```diff
@@ -1,7 +1,16 @@
+Metadata-Version: 2.1 Name: WrenchCL Version: 2.1.3 Summary: WrenchCL is a
+comprehensive library designed to facilitate seamless interactions with AWS
+services, OpenAI models, and various utility tools. This package aims to
+streamline the development process by providing robust components for database
+interactions, cloud storage, and AI-powered functionalities. Home-page: https:/
+/github.com/WrenchAI/WrenchCL Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License Classifier: Operating System
+:: OS Independent Requires-Python: >=3.11 Description-Content-Type: text/
+markdown Provides-Extra: libmagic License-File: LICENSE
                        ************ WWrreenncchh CCooddee LLiibbrraarryy ************
     [Logo]_[_P_y_P_I_ _-_ _V_e_r_s_i_o_n_]_[_M_a_i_n_t_a_i_n_e_r_]_[_G_i_t_H_u_b_ _W_o_r_k_f_l_o_w_ _S_t_a_t_u_s_ _(_w_i_t_h_ _e_v_e_n_t_)_]
 ## Description WrenchCL is a comprehensive library designed to facilitate
 seamless interactions with AWS services, OpenAI models, and various utility
 tools. This package aims to streamline the development process by providing
 robust components for database interactions, cloud storage, and AI-powered
 functionalities. **PyPI Link:** [WrenchCL on PyPI](https://pypi.org/project/
@@ -12,42 +21,43 @@
 _Internal for interacting with OpenAI models. - **Tools**: Miscellaneous
 utility tools such as coalescing values, file typing, image encoding, and a
 custom logger. - **DataFlow**: Response focused tools to aid in returning
 values and generating logs based on status codes. ## Installation To install
 the package, simply run the following command: ```bash pip install WrenchCL ```
 Upon recieving the below error: ```bash ImportError: failed to find libmagic.
 Check your installation ``` Install the package with the optional libmagic
-dependency, users can using the following command: ```bash pip install WrenchCL
-[libmagic] ``` # User Guides Sure! Here's an updated and more detailed README
-that provides extensive instructions on how to use `AWSClientHub`,
-`RdsServiceGateway`, `S3ServiceGateway`, `ConversationManager`,
-`OpenAIFactory`, and `OpenAIGateway`. It also includes practical examples for
-the `Maybe` monad and other utility tools. ### Connecting to AWS Services To
-interact with AWS RDS and S3 services, follow these steps: 1. **Setup
-`AWSClientHub`**: ```python from WrenchCL.Connections import AwsClientHub #
-Initialize the AWSClientHub using an env file or keyword arguments
-aws_client_hub = AWSClientHub(env_path="path/to/your/env/file") #
+dependency, users can using the following command: ```bash 1. pip uninstall
+python-magic -y 2. pip install WrenchCL[libmagic] ``` # User Guides Sure!
+Here's an updated and more detailed README that provides extensive instructions
+on how to use `AWSClientHub`, `RdsServiceGateway`, `S3ServiceGateway`,
+`ConversationManager`, `OpenAIFactory`, and `OpenAIGateway`. It also includes
+practical examples for the `Maybe` monad and other utility tools. ###
+Connecting to AWS Services To interact with AWS RDS and S3 services, follow
+these steps: 1. **Setup `AWSClientHub`**: ```python from WrenchCL.Connections
+import AwsClientHub # Initialize the AWSClientHub using an env file or keyword
+arguments aws_client_hub = AWSClientHub(env_path="path/to/your/env/file") #
 Alternatively, use keyword arguments or existing env variables # aws_client_hub
 = AWSClientHub(aws_profile='your_profile', region_name='your_region',
 secret_arn='your_secret_arn', ...) ``` 2. **Using `RdsServiceGateway`**:
 ```python from WrenchCL.Connections import RdsServiceGateway # Initialize
 RdsServiceGateway with the AWSClientHub instance rds_service =
 RdsServiceGateway(aws_client_hub) # Example: Fetching data from the database
 query = "SELECT * FROM your_table" data = rds_service.get_data(query) print
 (data) ``` **Methods in `RdsServiceGateway`**: - `get_data(query: str, payload:
-Optional[dict] = None, fetchall: bool = True, accepted_type: Optional[Type] =
-None, none_is_ok: bool = False, accepted_length: Tuple[Optional[int], Optional
-[int]] = (None, None)) -> Optional[Any]` - Fetches data from the database based
-on the input query and parameters. - `update_database(query: str, payload:
-Union[dict, 'pd.DataFrame'], column_order: Optional[List[str]] = None) -> None`
-- Updates the database by executing the given query with the provided payload.
-3. **Using `S3ServiceGateway`**: ```python from WrenchCL.Connect import
-S3ServiceGateway # Initialize S3ServiceGateway with the AWSClientHub instance
-s3_service = S3ServiceGateway(aws_client_hub) # Example: Downloading an object
-from S3 bucket_name = "your-bucket-name" object_key = "path/to/your/object"
+Optional[dict] = None, fetchall: bool = True, return_dict: bool = True,
+accepted_type: Optional[Type] = None, none_is_ok: bool = False,
+accepted_length: Tuple[Optional[int], Optional[int]] = (None, None)) -
+> Optional[Any]` - Fetches data from the database based on the input query and
+parameters. - `update_database(query: str, payload: Union[dict,
+'pd.DataFrame'], column_order: Optional[List[str]] = None) -> None` - Updates
+the database by executing the given query with the provided payload. 3. **Using
+`S3ServiceGateway`**: ```python from WrenchCL.Connect import S3ServiceGateway #
+Initialize S3ServiceGateway with the AWSClientHub instance s3_service =
+S3ServiceGateway(aws_client_hub) # Example: Downloading an object from S3
+bucket_name = "your-bucket-name" object_key = "path/to/your/object"
 s3_service.download_object(bucket_name, object_key, "local/path/to/save") ```
 **Methods in `S3ServiceGateway`**: - `get_object(bucket_name: str, object_key:
 str) -> io.BytesIO` - Retrieves an object from S3. - `download_object
 (bucket_name: str, object_key: str, local_path: str) -> None` - Downloads an
 object from S3 to the local file system. - `get_object_headers(bucket_name:
 str, object_key: str) -> dict` - Retrieves the headers of an object in S3. -
 `upload_object(file_path: str, bucket_name: str, object_key: str) -> None` -
@@ -63,52 +73,60 @@
 an object exists in S3. - `list_objects(bucket_name: str, prefix: Optional[str]
 = None) -> list` - Lists objects in an S3 bucket. - `check_bucket_permissions
 (bucket_name: str) -> dict` - Checks the permissions of an S3 bucket. ###
 Interacting with OpenAI Models To use OpenAI models, follow these steps: 1.
 **Setup `OpenAIGateway`**: ```python from WrenchCL.Models.OpenAI import
 OpenAIGateway # Initialize OpenAIGateway with your OpenAI API key
 openai_gateway = OpenAIGateway(api_key="your_openai_api_key") # Example:
-Generating text response = openai_gateway.handle_text("Your prompt here") print
-(response) ``` **Methods in `OpenAIGateway`**: - `handle_text(text: str, model:
-str = "gpt-3.5-turbo", system_prompt: Optional[str] = None, image_url: Optional
-[str] = None, json_mode: bool = False, **kwargs) -> Union[str, dict]` -
-Processes text input using the specified model and returns the response. -
-`get_embeddings(text: str, model: str = "text-embedding-3-small") -> list` -
-Retrieves embeddings for the given text using the specified model. -
-`generate_image(prompt: str, size: str = "1024x1024", quality: str =
-"standard", n: int = 1) -> str` - Generates an image based on the provided
-prompt. - `process_audio(audio_path: str, model: str = "whisper-1") -> str` -
-Processes an audio file and returns its transcription. -
-`create_image_variation(image_path: str, n: int = 1, size: str = "1024x1024") -
-> str` - Creates variations of an image based on the provided image path. -
-`edit_image(image_path: str, prompt: str, mask_path: str, n: int = 1, size: str
-= "1024x1024") -> str` - Edits an image based on the provided prompt and mask.
-- `vision_query(question: str, image_path: str, **kwargs) -> dict` - Processes
-a vision query based on the provided question and image. -
-`convert_image_to_url_or_base64(image_path: str) -> str` - Converts an image to
-a URL or base64 encoded string. - `initiate_conversation(initial_text: str,
-**kwargs)` - Initiates a conversation using the provided initial text. 2.
-**Using `OpenAIFactory`**: ```python from WrenchCL.Models.OpenAI import
-OpenAIFactory # Initialize OpenAIFactory with your OpenAI API key
-openai_factory = OpenAIFactory(api_key="your_openai_api_key") # Example:
-Transcribing audio to text and getting embeddings audio_path = "path/to/your/
-audio/file" embeddings = openai_factory.audio_to_text_to_embeddings(audio_path)
-print(embeddings) ``` **Methods in `OpenAIFactory`**: -
-`audio_to_text_to_embeddings(audio_path: str, embedding_model: str = "text-
-embedding-3-small") -> list` - Transcribes audio to text and then generates
-embeddings for the text. - `image_to_text_to_embeddings(image_path: str,
-question: str, embedding_model: str = "text-embedding-3-small") -> list` -
-Performs a vision query to understand an image and then generates embeddings
-for the response. - `validate_response_with_gpt(initial_response: str,
-validation_prompt: str) -> str` - Uses an initial response and validates or
-expands upon it with a secondary GPT call. ### Utility Tools WrenchCL includes
-several utility tools for various purposes: - **validate_input_dict**:
-Validates the input dictionary against expected types. ```python from
-WrenchCL.Tools import validate_input_dict params = { 'event': 'event_data',
-'context': 'context_data', 'start_time': 1625256000, 'lambda_client':
+Generating text response = openai_gateway.text_response("Your prompt here")
+print(response) ``` **Methods in `OpenAIGateway`**: - `text_response(text: str,
+model: str = "gpt-3.5-turbo", system_prompt: Optional[str] = None, image_url:
+Optional[str] = None, json_mode: bool = False, stream : bool = False, **kwargs)
+-> Union[str, dict]` - Processes text input using the specified model and
+returns the response. - `get_embeddings(text: str, model: str = "text-
+embedding-3-small") -> list` - Retrieves embeddings for the given text using
+the specified model. - `text_to_image(prompt: str, size: str = "1024x1024",
+quality: str = "standard", n: int = 1) -> str` - Generates an image based on
+the provided prompt. - `audio_to_text(audio_path: str, model: str = "whisper-
+1") -> str` - Processes an audio file and returns its transcription. -
+`generate_image_variations(image_path: str, n: int = 1, size: str =
+"1024x1024") -> str` - Creates variations of an image based on the provided
+image path. - `modify_image(image_path: str, prompt: str, mask_path: str, n:
+int = 1, size: str = "1024x1024") -> str` - Edits an image based on the
+provided prompt and mask. - `image_to_text(question: str, image_path: str,
+**kwargs) -> dict` - Processes a vision query based on the provided question
+and image. - `convert_image_to_url_or_base64(image_path: str) -> str` -
+Converts an image to a URL or base64 encoded string. - `start_conversation
+(initial_text: str, **kwargs)` - Initiates a conversation using the provided
+initial text. 2. **Using `OpenAIFactory`**: ```python from
+WrenchCL.Models.OpenAI import OpenAIFactory # Initialize OpenAIFactory with
+your OpenAI API key openai_factory = OpenAIFactory
+(api_key="your_openai_api_key") # Example: Transcribing audio to text and
+getting embeddings audio_path = "path/to/your/audio/file" embeddings =
+openai_factory.audio_to_text_to_embeddings(audio_path) print(embeddings) ```
+**Methods in `OpenAIFactory`**: - `audio_to_text_to_embeddings(audio_path: str,
+embedding_model: str = "text-embedding-3-small") -> list` - Transcribes audio
+to text and then generates embeddings for the text. -
+`image_to_text_to_embeddings(image_path: str, question: str, embedding_model:
+str = "text-embedding-3-small") -> list` - Performs a vision query to
+understand an image and then generates embeddings for the response. -
+`validate_response_with_gpt(initial_response: str, validation_prompt: str) -
+> str` - Uses an initial response and validates or expands upon it with a
+secondary GPT call. ### Utility Tools WrenchCL includes several utility tools
+for various purposes: Got it! Here is the section about the custom JSON
+serializer in the specified format: ### Custom JSON Serializer -
+**robust_serializer**: Serializes objects not natively serializable by JSON,
+including `datetime`, `date`, `Decimal`, and custom objects. ```python # Usage
+with json_dumps from datetime import datetime import json from WrenchCL.Tools
+import robust_serializer print(json.dumps({"timestamp": datetime.now()},
+default=robust_serializer)) # Output: {"timestamp": "2024-05-17T12:34:
+56.789012"} ``` - **validate_input_dict**: Validates the input dictionary
+against expected types. ```python from WrenchCL.Tools import
+validate_input_dict params = { 'event': 'event_data', 'context':
+'context_data', 'start_time': 1625256000, 'lambda_client':
 'lambda_client_instance' } expected_types = { 'event': str, 'context': str,
 'start_time': (int, float), 'lambda_client': object, } validate_input_dict
 (params, expected_types) ``` - **Coalesce**: A utility function to return the
 first non-null value. ```python from WrenchCL.Tools import coalesce result =
 coalesce(None, "default_value") print(result) # Output: "default_value" ``` -
 **FileTyper**: A utility for determining file types. ```python from
 WrenchCL.Tools import get_file_type file_type = get_file_type("path/to/your/
```

### Comparing `WrenchCL-2.1.2/WrenchCL/Connect/AwsClientHub.py` & `WrenchCL-2.1.3/WrenchCL/Connect/AwsClientHub.py`

 * *Files 7% similar despite different names*

```diff
@@ -20,42 +20,46 @@
 from .._Internal._ConfigurationManager import _ConfigurationManager
 from .._Internal._SshTunnelManager import _SshTunnelManager
 from ..Decorators.SingletonClass import SingletonClass
 from ..Tools.WrenchLogger import logger
 from ..Tools.Coalesce import coalesce
 from mypy_boto3_s3.client import S3Client
 from mypy_boto3_rds.client import RDSClient
+from mypy_boto3_secretsmanager.client import SecretsManagerClient
+from mypy_boto3_lambda.client import LambdaClient
 
 
 @SingletonClass
 class AwsClientHub:
     """
     Manages AWS client services including RDS and S3. Ensures that client instances are created as singletons to
     maintain efficient use of resources and consistency across operations.
 
     Attributes:
-        aws_profile (str): AWS profile name used for creating sessions.
+        self.config (str): _ConfigurationManager instance
         aws_session_client (boto3.session.Session): The AWS session client for accessing various AWS services.
         db_client (object): Client for interacting with AWS RDS databases.
         s3_client (object): Client for interacting with AWS S3 storage.
         need_ssh_tunnel (bool): Indicates if an SSH tunnel is required for database connections, based on secret data.
     """
 
-    def __init__(self, env_path):
+    def __init__(self, env_path=None):
         """
         Initializes the AwsClientHub by setting up the AWS profile and fetching necessary secrets for other
         AWS service configurations.
 
         :param env_path: The path to the environment configuration file.
-        :type env_path: str
+        :type env_path: str, optional
         """
+        self.lambda_client = None
         self.config = None
         self.aws_session_client = None
         self.db_client = None
         self.s3_client = None
+        self.secret_client = None
         self.need_ssh_tunnel = False
         self.reload_config(env_path=env_path)
         self._get_secret()
         self._initialized = True
 
     def reload_config(self, env_path=None):
         """
@@ -120,26 +124,46 @@
         :Usage:
             s3_client = client_manager.get_s3_client()
         """
         if self.s3_client is None:
             self._init_s3_client()
         return self.s3_client
 
+    def get_secret_client(self):
+        """
+        Retrieves and returns an AWS Secretmanager service client instance, initializing it if not already done.
+
+        :returns: The initialized AWS Secretmanager client instance.
+        :rtype: SecretsManagerClient
+        """
+        if self.secret_client is None:
+            self.secret_client = self._init_other_client(aws_service='secretsmanager')
+        return self.secret_client
+
+    def get_lambda_client(self):
+        """
+        Retrieves and returns an AWS Lambda service client instance, initializing it if not already done.
+
+        :returns: The initialized AWS Lambda client instance.
+        :rtype: LambdaClient
+        """
+        if self.lambda_client is None:
+            self.lambda_client = self._init_other_client(aws_service='lambda')
+        return self.lambda_client
+
     def get_service_client(self, aws_service):
         """
         Retrieves and returns an AWS service client instance, initializing it if not already done.
 
         :param aws_service: The name of the AWS service.
         :type aws_service: str
 
         :returns: The initialized AWS service client instance.
         """
-        if self.s3_client is None:
-            self._init_other_client(aws_service=aws_service)
-        return self.s3_client
+        return self._init_other_client(aws_service=aws_service)
 
     def _init_rds_client(self):
         """
         Initializes the RDS client with the necessary configuration derived from the AWS secrets manager.
 
         :raises Exception: If there is an issue initializing the RDS client.
         """
@@ -203,15 +227,15 @@
 
         :param aws_service: The name of the AWS service.
         :type aws_service: str
 
         :raises Exception: If there is an issue initializing the AWS service client.
         """
         try:
-            self.other_client = self.aws_session_client.client(aws_service, region_name=self.config.region_name)
+            return self.aws_session_client.client(aws_service, region_name=self.config.region_name)
         except Exception as e:
             logger.error(f"An exception occurred when initializing connection to {aws_service}: {e}")
             raise e
 
     def _get_secret(self):
         """
         Fetches and decodes the secret configuration from AWS Secrets Manager, setting up necessary client
```

### Comparing `WrenchCL-2.1.2/WrenchCL/Connect/RdsServiceGateway.py` & `WrenchCL-2.1.3/WrenchCL/Connect/RdsServiceGateway.py`

 * *Files 18% similar despite different names*

```diff
@@ -45,47 +45,68 @@
         """
         Initializes the RdsServiceGateway by establishing a connection to the database using the AwsClientHub.
         """
         client_manager = AwsClientHub()
         self.connection = client_manager.get_db_client()
         self.config = client_manager.get_config()
 
-    def get_data(self, query: str, payload: Optional[dict] = None, fetchall: bool = True,
-                 accepted_type: Optional[Type] = None, none_is_ok: bool = False,
+    def get_data(self, query: str, payload: Optional[tuple] = None, fetchall: bool = True,
+                 return_dict: bool = True,  accepted_type: Optional[Type] = None, none_is_ok: bool = False,
                  accepted_length: Tuple[Optional[int], Optional[int]] = (None, None)) -> Optional[Any]:
         """
         Fetch data from the database based on the input query and parameters.
 
         :param query: SQL query to execute.
         :type query: str
         :param payload: Parameters to substitute into the query.
         :type payload: dict, optional
         :param fetchall: Whether to fetch all rows or just one.
         :type fetchall: bool, optional
+        :param return_dict: Whether to return a dictionary or raw dict cursor response
+        :type return_dict: bool, optional
         :param accepted_type: Expected type of the fetched data.
         :type accepted_type: Type, optional
         :param none_is_ok: If True, None can be a valid return type if no data is found.
         :type none_is_ok: bool, optional
         :param accepted_length: A tuple of the minimum and maximum allowed lengths of the data.
         :type accepted_length: Tuple[Optional[int], Optional[int]], optional
         :returns: The fetched data or None if validations fail.
         :rtype: Optional[Any]
         """
-        with self.connection as conn:
-            with conn.connection.cursor(cursor_factory=psycopg2.extras.DictCursor) as cursor:
-                cursor.execute(query, payload)
-                data = cursor.fetchall() if fetchall else cursor.fetchone()
-                cursor.close()
-        if accepted_type:
-            if self._validate_output(data, accepted_type, none_is_ok, accepted_length):
-                return data
+        logger.debug("Executing query: ", query)
+        logger.debug("With payload: ", payload)
+
+        try:
+            with self.connection as conn:
+                with conn.cursor(cursor_factory=psycopg2.extras.DictCursor) as cursor:
+                    cursor.execute(query, payload)
+                    data = cursor.fetchall() if fetchall else cursor.fetchone()
+                    logger.debug("Fetched data: ", str(data)[:100])
+                    cursor.close()
+
+            if accepted_type:
+                logger.debug("Validating output with type: %s", accepted_type)
+                if self._validate_output(data, accepted_type, none_is_ok, accepted_length):
+                    logger.debug("Output validated successfully")
+                    if return_dict:
+                        return [dict(row) for row in data] if fetchall else dict(data)
+                    else:
+                        return data
+
+                else:
+                    logger.debug("Output validation failed")
+                    return None
             else:
-                return None
-        else:
-            return data
+                if return_dict:
+                    return [dict(row) for row in data] if fetchall else dict(data)
+                else:
+                    return data
+        except Exception as e:
+            logger.error("Error executing query: ", e)
+            return None
 
     def update_database(self, query: str, payload: Union[dict, 'pd.DataFrame'],
                         column_order: Optional[List[str]] = None) -> None:
         """
         Updates the database by executing the given query with the provided payload.
 
         :param query: SQL query to execute.
@@ -95,40 +116,40 @@
         :param column_order: The order of columns to be used if the payload is a DataFrame.
         :type column_order: List[str], optional
         :returns: None
         """
         with self.connection as conn:
             if isinstance(payload, dict):
                 try:
-                    with conn.connection.cursor(cursor_factory=psycopg2.extras.DictCursor) as cursor:
+                    with conn.cursor(cursor_factory=psycopg2.extras.DictCursor) as cursor:
                         cursor.execute(query, payload)
-                        conn.connection.commit()
+                        conn.commit()
                 except Exception as e:
                     logger.error(f"Error inserting data: {str(e)}")
-                    conn.connection.rollback()
+                    conn.rollback()
             elif PANDAS_AVAILABLE and isinstance(payload, pd.DataFrame) and column_order:
                 try:
-                    with conn.connection.cursor() as cursor:
+                    with conn.cursor() as cursor:
                         data_batch = []
                         batch_counter = 1
                         total_batches = math.ceil(len(payload) / self.config.db_batch_size)
                         for index, row in payload.iterrows():
                             data_batch.append(tuple(row[col] for col in column_order))
 
                             if len(data_batch) == self.config.db_batch_size or index == len(payload) - 1:
                                 psycopg2.extras.execute_values(cursor, query, data_batch,
                                                                page_size=self.config.db_batch_size)
                                 data_batch = []
                                 logger.debug(f"Processed batch {batch_counter}/{total_batches} successfully")
                                 batch_counter += 1
 
-                        conn.connection.commit()
+                        conn.commit()
                 except Exception as e:
                     logger.error(f"Error processing batch: {str(e)}")
-                    conn.connection.rollback()
+                    conn.rollback()
             else:
                 logger.error("Invalid payload type or missing column_order for DataFrame payload.")
 
     @staticmethod
     def _validate_output(data: Any, accepted_type: Type, none_is_ok: bool = False,
                          accepted_length: Tuple[Optional[int], Optional[int]] = (None, None)) -> bool:
         """
```

### Comparing `WrenchCL-2.1.2/WrenchCL/Connect/S3ServiceGateway.py` & `WrenchCL-2.1.3/WrenchCL/Connect/S3ServiceGateway.py`

 * *Files identical despite different names*

### Comparing `WrenchCL-2.1.2/WrenchCL/DataFlow/build_return_json.py` & `WrenchCL-2.1.3/WrenchCL/DataFlow/build_return_json.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,35 +19,28 @@
 
 # Created by Jeong Kim
 # Github: https://github.com/dalmad2
 # Annotated by Willem van der Schans
 # Github: https://github.com/Kydoimos97
 
 
-def build_return_json(code, message, return_dict=None):
+def build_return_json(code, response_body):
     """
     Constructs a JSON response body with the provided status code and message, optionally including a return dictionary.
 
     Args:
         code (int): The HTTP status code to be included in the response.
-        message (str): The message to be included in the response body.
-        return_dict (dict, optional): A dictionary containing additional data to be included in the response body. Defaults to None.
+        response_body (dict): A dictionary containing data to be included in the response body. Defaults to None.
 
     Returns:
         dict: A dictionary representing the JSON response containing the status code, message, and optionally the return dictionary.
 
     Raises:
         None: No explicit exceptions are raised within this function.
     """
-    response_body = {
-        'message': message
-    }
-
-    if return_dict:
-        response_body['result'] = return_dict
 
     return {
         'statusCode': code,
         'body': json.dumps(response_body),
         'headers': {
             'Content-Type': 'application/json; charset=utf-8',
             'strict-transport-security': 'max-age=63072000; includeSubdomains; preload',
```

### Comparing `WrenchCL-2.1.2/WrenchCL/DataFlow/handle_lambda_response.py` & `WrenchCL-2.1.3/WrenchCL/DataFlow/handle_lambda_response.py`

 * *Files 5% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 from ..Tools.DictValidator import validate_input_dict
 from ..Tools.WrenchLogger import logger
 from .build_return_json import build_return_json
 from .trigger_dataflow_metrics import trigger_minimum_dataflow_metrics
 
 lambda_response = None
 
+
 class GuardedResponseTrigger(Exception):
     """Custom exception to signal early exit from the Lambda function."""
 
     def __init__(self, response):
         self.response = response
 
     def get_response(self):
@@ -33,118 +34,104 @@
         Retrieves the response associated with this exception.
 
         Returns:
             dict: The response dictionary associated with this exception.
         """
         return self.response
 
-def handle_lambda_response(code, message, params, client_id=None, entity_id=None):
+
+def handle_lambda_response(code, message, params, response_body=None, client_id=None, entity_id=None):
     """
     Handles the Lambda function response generation and logging based on the provided status code and message.
 
     Args:
         code (int): The HTTP status code to be included in the response.
         message (str): The message to be included in the response body.
         params (dict): A dictionary containing parameters required for further processing.
+        response_body (dict, optional): The json response body
         client_id (str, optional): The client ID. Defaults to None.
         entity_id (str, optional): The entity ID. Defaults to None.
 
     Raises:
         GuardedResponseTrigger: Custom exception to signal early exit from the Lambda function. If raised and not handled
                                 at the Lambda handler level, this exception will cause an immediate return with the
                                 generated response. If caught within nested calls, ensure to re-raise it as follows:
                                 `except GuardedResponseTrigger as e: raise e`
     """
     code = int(code)
-    expected_types = {
-        'event': str,
-        'context': str,
-        'start_time': (int, float),
-        'lambda_client': boto3client,
-    }
+    expected_types = {'event': str, 'context': str, 'start_time': (int, float), 'lambda_client': boto3client, }
 
     try:
         validate_input_dict(params, expected_types)
-        trigger_minimum_dataflow_metrics(
-            event=params.get('event'),
-            context=params.get('context'),
-            start_time=params.get('start_time'),
-            lambda_client=params.get('lambda_client'),
-            job_name='Model Inference Service',
-            job_type='Lambda',
-            status_code=str(code),
-            message=str(message)
-        )
+        trigger_minimum_dataflow_metrics(event=params.get('event'), context=params.get('context'),
+                                         start_time=params.get('start_time'), lambda_client=params.get('lambda_client'),
+                                         job_name='Model Inference Service', job_type='Lambda', status_code=str(code),
+                                         message=str(message))
     except Exception as e:
         logger.error(f"Failed to invoke dataflow metrics with error {e}")
 
-    custom_error_messages = {
-        700: "Generic Custom Error: A fallback error for unspecified issues.",
-        701: "Invalid Request Format: The request body does not match the expected schema.",
-        702: "Authentication Failed: Credentials provided are invalid or expired.",
-        703: "Authorization Denied: The authenticated user does not have permission to access the requested resource.",
-        704: "Resource Not Found: The requested resource does not exist or is not available.",
-        705: "Resource Locked: The resource is currently locked or in use and cannot be modified.",
-        706: "Rate Limit Exceeded: The request has exceeded the rate limit. Try again later.",
-        707: "Data Validation Failed: The provided data does not meet validation criteria.",
-        708: "Dependency Error: A failure occurred in an external service or dependency.",
-        709: "Feature Deprecated: The requested feature is no longer supported.",
-        710: "Uncaught Expected Exit Path: The Lambda has been exited in an expected manner without successfully ending.",
-
-        730: "Model Training Error: An error occurred during the training process of a machine learning model.",
-        731: "Model Not Found: The specified machine learning model could not be found.",
-        732: "Prediction Error: An Internal error occurred while making a prediction with the model.",
-        733: "Model Update Failure: Failed to update the machine learning model.",
-        734: "Invalid Model Input: The input data for the model is invalid or malformed.",
-        735: "Model Deployment Error: An error occurred while deploying the machine learning model.",
-        736: "Model Version Conflict: There is a version conflict with the machine learning model.",
-        737: "Prediction Error: Invalid prediction provided by model.",
-        738: "Data Value Error: Returned score does not satisfy constraints or expected range.",
-        740: "Lambda Invocation Error: An error occurred while invoking an AWS Lambda function.",
-        741: "Lambda Timeout: The AWS Lambda function timed out before completion.",
-        742: "Insufficient Permissions: The AWS Lambda function does not have the necessary permissions.",
-        743: "Cold Start Delay: Delay due to AWS Lambda cold start.",
-        744: "API Gateway Integration Error: An error occurred in the integration between Lambda and API Gateway.",
-        745: "Lambda Resource Limit Exceeded: The AWS Lambda function exceeded its allocated resources.",
-
-        750: "Data Retrieval Failure: Failed to retrieve data from the database or storage.",
-        751: "Data Save Failure: Failed to save data to the database or storage.",
-        752: "Data Integrity Error: The data integrity check failed.",
-        753: "Data Serialization Error: An error occurred during data serialization or deserialization.",
-        754: "Data Version Mismatch: The version of the data does not match the expected version.",
-        755: "Data Expiry Error: Attempted to access data that has expired or is no longer valid.",
-        756: "Data Encryption Error: An error occurred during data encryption or decryption.",
-        757: "Data Typing Error: An error occurred during data type coercion.",
-        758: "Data Retrieval Rejection: The requested data already exists.",
-
-        800: "Payment Required: The request cannot be processed without payment.",
-        801: "Quota Exceeded: The usage quota for the service or resource has been exceeded.",
-        802: "Duplicate Request: The same request has been received more than once.",
-        803: "Resource Conflict: The request could not be completed due to a conflict with the current state of the resource.",
-        804: "Precondition Failed: One or more conditions in the request header fields evaluated to false.",
-        805: "Validation Timeout: The validation process for the request has timed out.",
-        806: "Operation Not Allowed: The requested operation is not allowed.",
-        807: "Data Mismatch Error: The provided data does not match the expected data.",
-        808: "Partial Success: The operation was partially successful.",
-        809: "Dependent Resource Unavailable: A resource that the request depends on is not available."
-    }
+    custom_error_messages = {700: "Generic Custom Error: A fallback error for unspecified issues.",
+                             701: "Invalid Request Format: The request body does not match the expected schema.",
+                             702: "Authentication Failed: Credentials provided are invalid or expired.",
+                             703: "Authorization Denied: The authenticated user does not have permission to access the requested resource.",
+                             704: "Resource Not Found: The requested resource does not exist or is not available.",
+                             705: "Resource Locked: The resource is currently locked or in use and cannot be modified.",
+                             706: "Rate Limit Exceeded: The request has exceeded the rate limit. Try again later.",
+                             707: "Data Validation Failed: The provided data does not meet validation criteria.",
+                             708: "Dependency Error: A failure occurred in an external service or dependency.",
+                             709: "Feature Deprecated: The requested feature is no longer supported.",
+                             710: "Uncaught Expected Exit Path: The Lambda has been exited in an expected manner without successfully ending.",
+
+                             730: "Model Training Error: An error occurred during the training process of a machine learning model.",
+                             731: "Model Not Found: The specified machine learning model could not be found.",
+                             732: "Prediction Error: An Internal error occurred while making a prediction with the model.",
+                             733: "Model Update Failure: Failed to update the machine learning model.",
+                             734: "Invalid Model Input: The input data for the model is invalid or malformed.",
+                             735: "Model Deployment Error: An error occurred while deploying the machine learning model.",
+                             736: "Model Version Conflict: There is a version conflict with the machine learning model.",
+                             737: "Prediction Error: Invalid prediction provided by model.",
+                             738: "Data Value Error: Returned score does not satisfy constraints or expected range.",
+                             740: "Lambda Invocation Error: An error occurred while invoking an AWS Lambda function.",
+                             741: "Lambda Timeout: The AWS Lambda function timed out before completion.",
+                             742: "Insufficient Permissions: The AWS Lambda function does not have the necessary permissions.",
+                             743: "Cold Start Delay: Delay due to AWS Lambda cold start.",
+                             744: "API Gateway Integration Error: An error occurred in the integration between Lambda and API Gateway.",
+                             745: "Lambda Resource Limit Exceeded: The AWS Lambda function exceeded its allocated resources.",
+
+                             750: "Data Retrieval Failure: Failed to retrieve data from the database or storage.",
+                             751: "Data Save Failure: Failed to save data to the database or storage.",
+                             752: "Data Integrity Error: The data integrity check failed.",
+                             753: "Data Serialization Error: An error occurred during data serialization or deserialization.",
+                             754: "Data Version Mismatch: The version of the data does not match the expected version.",
+                             755: "Data Expiry Error: Attempted to access data that has expired or is no longer valid.",
+                             756: "Data Encryption Error: An error occurred during data encryption or decryption.",
+                             757: "Data Typing Error: An error occurred during data type coercion.",
+                             758: "Data Retrieval Rejection: The requested data already exists.",
+
+                             800: "Payment Required: The request cannot be processed without payment.",
+                             801: "Quota Exceeded: The usage quota for the service or resource has been exceeded.",
+                             802: "Duplicate Request: The same request has been received more than once.",
+                             803: "Resource Conflict: The request could not be completed due to a conflict with the current state of the resource.",
+                             804: "Precondition Failed: One or more conditions in the request header fields evaluated to false.",
+                             805: "Validation Timeout: The validation process for the request has timed out.",
+                             806: "Operation Not Allowed: The requested operation is not allowed.",
+                             807: "Data Mismatch Error: The provided data does not match the expected data.",
+                             808: "Partial Success: The operation was partially successful.",
+                             809: "Dependent Resource Unavailable: A resource that the request depends on is not available."}
 
     if code in custom_error_messages:
         logger.warning(
-            f"status code = {code} | {custom_error_messages[code]} | [Client ID: {client_id}, Entity ID: {entity_id}] | Status message: {message}"
-        )
+            f"status code = {code} | {custom_error_messages[code]} | [Client ID: {client_id}, Entity ID: {entity_id}] | Status message: {message}")
     elif 400 <= code < 500:
         logger.error(
-            f"status code = {code} | Un-Handled Exception Status Code | [Client ID: {client_id}, Entity ID: {entity_id}] | Status message: {message}"
-        )
+            f"status code = {code} | Un-Handled Exception Status Code | [Client ID: {client_id}, Entity ID: {entity_id}] | Status message: {message}")
     elif code != 200:
         logger.error(
-            f"status code = {code} | Unexpected Status Code | [Client ID: {client_id}, Entity ID: {entity_id}] | Status message: {message}"
-        )
+            f"status code = {code} | Unexpected Status Code | [Client ID: {client_id}, Entity ID: {entity_id}] | Status message: {message}")
     elif code == 200:
         logger.info(
-            f"status code = {code} | Success Status | [Client ID: {client_id}, Entity ID: {entity_id}] | Status message: {message}"
-        )
+            f"status code = {code} | Success Status | [Client ID: {client_id}, Entity ID: {entity_id}] | Status message: {message}")
 
-    response = build_return_json(code=code, message=message)
+    response = build_return_json(code=code,
+                                 response_body=dict(Message=message) if response_body is None else response_body)
     logger.context(f"Built Lambda Response: {response}")
     raise GuardedResponseTrigger(response)
```

### Comparing `WrenchCL-2.1.2/WrenchCL/DataFlow/trigger_dataflow_metrics.py` & `WrenchCL-2.1.3/WrenchCL/DataFlow/trigger_dataflow_metrics.py`

 * *Files identical despite different names*

### Comparing `WrenchCL-2.1.2/WrenchCL/Decorators/Retryable.py` & `WrenchCL-2.1.3/WrenchCL/Decorators/Retryable.py`

 * *Files identical despite different names*

### Comparing `WrenchCL-2.1.2/WrenchCL/Decorators/SingletonClass.py` & `WrenchCL-2.1.3/WrenchCL/Decorators/SingletonClass.py`

 * *Files identical despite different names*

### Comparing `WrenchCL-2.1.2/WrenchCL/Decorators/TimedMethod.py` & `WrenchCL-2.1.3/WrenchCL/Decorators/TimedMethod.py`

 * *Files identical despite different names*

### Comparing `WrenchCL-2.1.2/WrenchCL/Models/OpenAI/OpenAIFactory.py` & `WrenchCL-2.1.3/WrenchCL/Models/OpenAI/OpenAIFactory.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,15 +52,15 @@
         :param audio_path: The path to the audio file.
         :type audio_path: str
         :param embedding_model: The model to use for generating embeddings.
         :type embedding_model: str, optional
         :returns: The generated embeddings for the transcribed text.
         :rtype: list
         """
-        transcription = self.process_audio(audio_path, model="whisper-1")
+        transcription = self.audio_to_text(audio_path, model="whisper-1")
         embeddings = self.get_embeddings(transcription, model=embedding_model)
         return embeddings
 
     @TimedMethod
     def image_to_text_to_embeddings(self, image_path, question, embedding_model="text-embedding-3-small"):
         """
         Performs a vision query to understand an image and then generates embeddings for the response.
@@ -70,15 +70,15 @@
         :param question: The question to ask about the image.
         :type question: str
         :param embedding_model: The model to use for generating embeddings.
         :type embedding_model: str, optional
         :returns: The generated embeddings for the vision query response.
         :rtype: list
         """
-        vision_response = self.vision_query(question, image_path)
+        vision_response = self.image_to_text(question, image_path)
         embeddings = self.get_embeddings(vision_response, model=embedding_model)
         return embeddings
 
     @TimedMethod
     def validate_response_with_gpt(self, initial_response, validation_prompt):
         """
         Uses an initial response and validates or expands upon it with a secondary GPT call.
@@ -86,9 +86,9 @@
         :param initial_response: The initial response to validate or expand.
         :type initial_response: str
         :param validation_prompt: The prompt to use for validation or expansion.
         :type validation_prompt: str
         :returns: The validated or expanded response.
         :rtype: str
         """
-        validated_response = self.handle_text(validation_prompt + initial_response)
+        validated_response = self.text_response(validation_prompt + initial_response)
         return validated_response
```

### Comparing `WrenchCL-2.1.2/WrenchCL/Models/OpenAI/OpenAIGateway.py` & `WrenchCL-2.1.3/WrenchCL/Models/OpenAI/OpenAIGateway.py`

 * *Files 5% similar despite different names*

```diff
@@ -79,45 +79,47 @@
 
         if json_mode:
             kwargs['response_format'] = {'type': 'json_object'}
 
         if operation == "embeddings":
             return self.get_embeddings(text, **kwargs)
         elif operation == "text":
-            return self.handle_text(text, **kwargs)
+            return self.text_response(text, **kwargs)
         elif operation == 'thread' or operation == 'conversation':
-            return self.initiate_conversation(text, **kwargs)
+            return self.start_conversation(text, **kwargs)
         elif operation == "image" and text:
-            return self.generate_image(text, **kwargs)
+            return self.text_to_image(text, **kwargs)
         elif operation == "audio" and audio_path:
-            return self.process_audio(audio_path, **kwargs)
+            return self.audio_to_text(audio_path, **kwargs)
         elif operation == "edit_image" and image_path:
-            return self.edit_image(image_path, text, **kwargs)
+            return self.modify_image(image_path, text, **kwargs)
         elif operation == "create_variation" and image_path:
-            return self.create_image_variation(image_path, **kwargs)
+            return self.generate_image_variations(image_path, **kwargs)
         elif operation == "vision" and text and image_path:
-            return self.vision_query(text, image_path, **kwargs)
+            return self.image_to_text(text, image_path, **kwargs)
         else:
             raise ValueError("Invalid or insufficient parameters for requested operation.")
 
     @TimedMethod
-    def handle_text(self, text, model="gpt-3.5-turbo", system_prompt=None, image_url=None, json_mode=False, **kwargs):
+    def text_response(self, text, model="gpt-3.5-turbo", system_prompt=None, image_url=None, json_mode=False, stream=False, **kwargs):
         """
         Processes text input using the specified model and returns the response.
 
         :param text: The text input.
         :type text: str
         :param model: The model to use for text processing.
         :type model: str, optional
         :param system_prompt: A system prompt to include in the request.
         :type system_prompt: str, optional
         :param image_url: An image URL to include in the request.
         :type image_url: str, optional
         :param json_mode: If True, expects the response to be in JSON format.
         :type json_mode: bool, optional
+        :param stream: If True, stream the response as it's generated.
+        :type stream: bool, optional
         :returns: The processed text or JSON response.
         :raises ValueError: If the JSON response cannot be decoded.
         :raises InterruptedError: If the response cannot be completed due to content filters or other issues.
         :raises Exception: If an error occurs during text processing.
         """
         try:
             messages = []
@@ -127,44 +129,58 @@
 
             user_content = [{"type": "text", "text": text}]
             if image_url:
                 user_content.append({"type": "image_url", "image_url": image_url})
 
             messages.append({"role": "user", "content": user_content})
 
-            response = self.client.chat.completions.create(model=model, messages=messages,
-                                                           max_tokens=kwargs.get('max_tokens', 2500))
-            finish_reason = response.choices[0].finish_reason
-            if finish_reason == 'stop':
-                response_content = response.choices[0].message.content
-            elif finish_reason == 'length':
-                logger.warning(f"Not enough tokens available to complete message please increase max tokens | current setting = {kwargs.get('max_tokens', 2500)}")
-                response_content = response.choices[0].message.content
-            elif finish_reason == 'content_filter':
-                logger.error(f"ChatGPT does not allow processing of this content due to its content filters. Cannot return any output")
-                response_content = None
-                raise InterruptedError
+            if stream:
+                response = self.client.chat.completions.create(
+                    model=model,
+                    messages=messages,
+                    stream=True,
+                    max_tokens=kwargs.get('max_tokens', 2500)
+                )
+                return response
             else:
-                logger.error(f"LLM did not finish output due to reason {finish_reason} no output returned")
-                response_content = None
-                raise InterruptedError
-
-            if json_mode:
-                try:
-                    return json.loads(response_content)
-                except json.JSONDecodeError:
-                    logger.error("Failed to decode JSON response")
-                    raise ValueError("Invalid JSON response.")
+                response = self.client.chat.completions.create(
+                    model=model,
+                    messages=messages,
+                    max_tokens=kwargs.get('max_tokens', 2500)
+                )
+
+                finish_reason = response.choices[0].finish_reason
+                if finish_reason == 'stop':
+                    response_content = response.choices[0].message.content
+                elif finish_reason == 'length':
+                    logger.warning(f"Not enough tokens available to complete message. Please increase max tokens | current setting = {kwargs.get('max_tokens', 2500)}")
+                    response_content = response.choices[0].message.content
+                elif finish_reason == 'content_filter':
+                    logger.error("ChatGPT does not allow processing of this content due to its content filters. Cannot return any output.")
+                    response_content = None
+                    raise InterruptedError
+                else:
+                    logger.error(f"LLM did not finish output due to reason {finish_reason}. No output returned.")
+                    response_content = None
+                    raise InterruptedError
+
+                if json_mode:
+                    try:
+                        return json.loads(response_content)
+                    except json.JSONDecodeError:
+                        logger.error("Failed to decode JSON response.")
+                        raise ValueError("Invalid JSON response.")
 
-            return response_content
+                return response_content
 
         except Exception as e:
             logger.error(f"Error processing text: {str(e)}")
             raise
 
+
     @TimedMethod
     def get_embeddings(self, text, model="text-embedding-3-small"):
         """
         Retrieves embeddings for the given text using the specified model.
 
         :param text: The text input.
         :type text: str
@@ -178,15 +194,15 @@
             embeddings = response.data[0].embedding
             return embeddings
         except Exception as e:
             logger.error(f"Error getting embeddings: {str(e)}")
             raise
 
     @TimedMethod
-    def generate_image(self, prompt, size="1024x1024", quality="standard", n=1):
+    def text_to_image(self, prompt, size="1024x1024", quality="standard", n=1):
         """
         Generates an image based on the provided prompt.
 
         :param prompt: The image prompt.
         :type prompt: str
         :param size: The size of the generated image.
         :type size: str, optional
@@ -201,15 +217,15 @@
             response = self.client.images.generate(model="dall-e-3", prompt=prompt, size=size, quality=quality, n=n)
             return response.data[0].url
         except Exception as e:
             logger.error(f"Error generating image: {str(e)}")
             raise
 
     @TimedMethod
-    def process_audio(self, audio_path, model="whisper-1"):
+    def audio_to_text(self, audio_path, model="whisper-1"):
         """
         Processes an audio file and returns its transcription.
 
         :param audio_path: The path to the audio file.
         :type audio_path: str
         :param model: The model to use for audio processing.
         :type model: str, optional
@@ -225,15 +241,15 @@
                 transcript_text = transcript_text + segment_text
             return transcript_text
         except Exception as e:
             logger.error(f"Error processing audio: {str(e)}")
             raise
 
     @TimedMethod
-    def create_image_variation(self, image_path, n=1, size="1024x1024"):
+    def generate_image_variations(self, image_path, n=1, size="1024x1024"):
         """
         Creates variations of an image based on the provided image path.
 
         :param image_path: The path to the original image.
         :type image_path: str
         :param n: The number of image variations to create.
         :type n: int, optional
@@ -247,15 +263,15 @@
                 response = self.client.images.create_variation(image=image, n=n, model="dall-e-2", size=size)
             return response.data[0].url
         except Exception as e:
             logger.error(f"Error creating image variation: {str(e)}")
             raise
 
     @TimedMethod
-    def edit_image(self, image_path, prompt, mask_path, n=1, size="1024x1024"):
+    def modify_image(self, image_path, prompt, mask_path, n=1, size="1024x1024"):
         """
         Edits an image based on the provided prompt and mask.
 
         :param image_path: The path to the original image.
         :type image_path: str
         :param prompt: The prompt describing the edits.
         :type prompt: str
@@ -273,15 +289,15 @@
                 response = self.client.images.edit(model="dall-e-2", image=image, mask=mask, prompt=prompt, n=n, size=size)
             return response.data[0].url
         except Exception as e:
             logger.error(f"Error editing image: {str(e)}")
             raise
 
     @TimedMethod
-    def vision_query(self, question, image_path, **kwargs):
+    def image_to_text(self, question, image_path, **kwargs):
         """
         Processes a vision query based on the provided question and image.
 
         :param question: The question to ask.
         :type question: str
         :param image_path: The path to the image file.
         :type image_path: str
@@ -316,15 +332,15 @@
             with open(image_path, "rb") as image_file:
                 return f"data:image/jpeg;base64,{base64.b64encode(image_file.read()).decode('utf-8')}"
         except Exception as e:
             logger.error("Failed to process image for vision query")
             raise ValueError("Invalid image path or data.")
 
     @TimedMethod
-    def initiate_conversation(self, **kwargs):
+    def start_conversation(self, **kwargs):
         """
         Initiates a conversation using the provided initial text.
 
         :raises Exception: If an error occurs while initiating the conversation.
         """
         conversation_manager = ConversationManager(self.client, kwargs.get("assistant_id"))
         conversation_manager.initiate_conversation()
```

### Comparing `WrenchCL-2.1.2/WrenchCL/Models/OpenAI/_ConversationManager.py` & `WrenchCL-2.1.3/WrenchCL/Models/OpenAI/_ConversationManager.py`

 * *Files identical despite different names*

### Comparing `WrenchCL-2.1.2/WrenchCL/Models/OpenAI/__init__.py` & `WrenchCL-2.1.3/WrenchCL/Models/OpenAI/__init__.py`

 * *Files identical despite different names*

### Comparing `WrenchCL-2.1.2/WrenchCL/Tools/Coalesce.py` & `WrenchCL-2.1.3/WrenchCL/Tools/Coalesce.py`

 * *Files identical despite different names*

### Comparing `WrenchCL-2.1.2/WrenchCL/Tools/DictValidator.py` & `WrenchCL-2.1.3/WrenchCL/Tools/DictValidator.py`

 * *Files identical despite different names*

### Comparing `WrenchCL-2.1.2/WrenchCL/Tools/FetchMetaData.py` & `WrenchCL-2.1.3/WrenchCL/Tools/FetchMetaData.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,16 +17,17 @@
 import requests
 
 try:
     import magic
 except ImportError as e:
     raise ImportError(
         "Failed to import 'magic'. Please install the appropriate library. "
-        "On Windows, you can install it with:\n"
-        "pip install WrenchCL[libmagic]\n"
+        "On Windows, you can install it with:\n\n"
+        "pip uninstall python-magic -y\n"
+        "pip install WrenchCL[libmagic]\n\n"
         "On other platforms, ensure 'libmagic' is installed."
     ) from e
 
 from datetime import datetime
 
 def get_metadata(file_source, is_url=True):
     """
```

### Comparing `WrenchCL-2.1.2/WrenchCL/Tools/FileTyper.py` & `WrenchCL-2.1.3/WrenchCL/Tools/FileTyper.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,16 +15,17 @@
 import mimetypes
 import requests
 try:
     import magic
 except ImportError as e:
     raise ImportError(
         "Failed to import 'magic'. Please install the appropriate library. "
-        "On Windows, you can install it with:\n"
-        "pip install WrenchCL[libmagic]\n"
+        "On Windows, you can install it with:\n\n"
+        "pip uninstall python-magic -y\n"
+        "pip install WrenchCL[libmagic]\n\n"
         "On other platforms, ensure 'libmagic' is installed."
     ) from e
 
 
 def get_file_type(file_source, is_url=True):
     """
     Determine the file type of a file from a URL or file path.
```

### Comparing `WrenchCL-2.1.2/WrenchCL/Tools/Image2B64.py` & `WrenchCL-2.1.3/WrenchCL/Tools/Image2B64.py`

 * *Files identical despite different names*

### Comparing `WrenchCL-2.1.2/WrenchCL/Tools/MaybeMonad.py` & `WrenchCL-2.1.3/WrenchCL/Tools/MaybeMonad.py`

 * *Files identical despite different names*

### Comparing `WrenchCL-2.1.2/WrenchCL/Tools/WrenchLogger.py` & `WrenchCL-2.1.3/WrenchCL/Tools/WrenchLogger.py`

 * *Files 14% similar despite different names*

```diff
@@ -17,15 +17,16 @@
 import logging
 import os
 import random
 import string
 import sys
 import time
 import traceback
-from datetime import datetime, timedelta
+from datetime import datetime, timedelta, date
+from decimal import Decimal
 from textwrap import fill
 from typing import Any, Optional
 
 try:
     from colorama import init, Fore as ColoramaFore, Style as ColoramaStyle
 
     colorama_imported = True
@@ -249,141 +250,206 @@
 
         # Create and handle the log record
         record = self.logger.makeRecord(name=self.logger.name, level=level, fn=filepath_out, lno=line_no_out, msg=msg,
             args=None, exc_info=None, func=func_name_out, sinfo=sinfo)
         self.logger.handle(record)
 
     def _log_with_color(self, level: int, text: str, color: Optional[str] = None,
-            stack_info: Optional[bool] = False) -> None:
+                        stack_info: Optional[bool] = False) -> None:
+        indent_prefix = '  -->    '  # Custom indent prefix for new lines
+        if level <= 15:
+            text_col = ColoramaFore.LIGHTWHITE_EX
+        else:
+            text_col = ColoramaFore.WHITE
+
         if colorama_imported and color and not self.running_on_lambda:
+            # Apply color to each line and indent new lines
+            lines = text.splitlines()
+            colored_lines = [f"{lines[0]}"]
+            colored_lines += [f"{text_col}{indent_prefix}{line}{ColoramaStyle.RESET_ALL}" for line in lines[1:]]
+            text = '\n'.join(colored_lines)
             self._handlerFormat(color)
 
+        elif self.running_on_lambda:
+
+            # Join lines with a separator for AWS Lambda
+            text = " ".join(text.split())
+            self._handlerFormat()  # Use default handler format
+        else:
+            self._handlerFormat()  # Use default handler format
+
         if self.force_stack_trace and level >= 30:
             stack_info = True
-        self._log(level, text, stack_info)
 
-        if colorama_imported or self.running_on_lambda:
-            self._handlerFormat()
+        self._log(level, text, stack_info)
 
     def info(self, *args: str, stack_info: Optional[bool] = False) -> None:
         """Log information that might be helpful but isn't essential."""
-        text = ' '.join(args)
+        serialized_args = [str(self._custom_serializer(arg)) for arg in args]
+        text = ' '.join(serialized_args)
         self._log_with_color(logging.INFO, text, ColoramaFore.LIGHTGREEN_EX if colorama_imported else None, stack_info)
 
     log_info = INFO = info  # Aliases for info
 
     def context(self, *args: str, stack_info: Optional[bool] = False) -> None:
         """Log contextual information for better understanding of the flow."""
-        text = ' '.join(args)
+        serialized_args = [str(self._custom_serializer(arg)) for arg in args]
+        text = ' '.join(serialized_args)
         self._log_with_color(21, text, ColoramaFore.LIGHTMAGENTA_EX if colorama_imported else None, stack_info)
 
     log_context = CONTEXT = context  # Aliases for context
 
     def warning(self, *args: str, stack_info: Optional[bool] = False) -> None:
         """Log issues that aren't errors but might warrant investigation."""
-        text = ' '.join(args)
+        serialized_args = [str(self._custom_serializer(arg)) for arg in args]
+        text = ' '.join(serialized_args)
         self._log_with_color(logging.WARNING, text, ColoramaFore.YELLOW if colorama_imported else None, stack_info)
 
     log_warning = WARNING = warning  # Aliases for warning
 
     def HDL_WARN(self, *args: str, stack_info: Optional[bool] = False) -> None:
         """Log warnings that have been handled and do not require further action."""
-        text = ' '.join(args)
+        serialized_args = [str(self._custom_serializer(arg)) for arg in args]
+        text = ' '.join(serialized_args)
         self._log_with_color(31, text, ColoramaFore.MAGENTA if colorama_imported else None, stack_info)
 
     log_handled_warning = log_hdl_warn = HDL_WARN  # Aliases for HDL_WARN
 
     def error(self, *args: str, stack_info: Optional[bool] = False) -> None:
         """Log errors that could disrupt normal program flow."""
-        text = ' '.join(args)
+        serialized_args = [str(self._custom_serializer(arg)) for arg in args]
+        text = ' '.join(serialized_args)
         self._log_with_color(logging.ERROR, text, ColoramaFore.RED if colorama_imported else None, stack_info)
 
     log_error = ERROR = error  # Aliases for error
 
-    def data(self, data: Any, wrap_length: Optional[int] = None, max_rows: Optional[int] = None,
-            stack_info: Optional[bool] = False) -> None:
+    def data(self, data: Any, content: Optional[bool] = True, wrap_length: Optional[int] = None, max_rows: Optional[int] = None,
+            stack_info: Optional[bool] = False, indent: Optional[int] = 4) -> None:
         """Log Data in a lower contrast, handling formatting for readability."""
-        formatted_data = self._format_data(data, wrap_length, max_rows)
+        formatted_data = self._format_data(data, content, wrap_length, max_rows, indent=indent)
         self._log_with_color(41, formatted_data, ColoramaFore.LIGHTWHITE_EX if colorama_imported else None, stack_info)
 
     log_data = print_data = DATA = data
 
     def HDL_ERR(self, *args: str, stack_info: Optional[bool] = False) -> None:
         """Log errors that have been handled but still need to be reported."""
-        text = ' '.join(args)
+        serialized_args = [str(self._custom_serializer(arg)) for arg in args]
+        text = ' '.join(serialized_args)
         self._log_with_color(42, text, ColoramaFore.LIGHTMAGENTA_EX if colorama_imported else None, stack_info)
 
     log_handled_error = log_hdl_err = HDL_ERR  # Aliases for HDL_ERR
 
     def RECV_ERR(self, *args: str, stack_info: Optional[bool] = False) -> None:
         """Log errors from which the system can recover with or without manual intervention."""
-        text = ' '.join(args)
+        serialized_args = [str(self._custom_serializer(arg)) for arg in args]
+        text = ' '.join(serialized_args)
         self._log_with_color(43, text, ColoramaFore.LIGHTRED_EX if colorama_imported else None, stack_info)
 
     log_recoverable_error = log_recv_err = RECV_ERR  # Aliases for RECV_ERR
 
     def critical(self, *args: str, stack_info: Optional[bool] = False) -> None:
         """Log critical issues that require immediate attention."""
-        text = ' '.join(args)
+        serialized_args = [str(self._custom_serializer(arg)) for arg in args]
+        text = ' '.join(serialized_args)
         self._log_with_color(logging.CRITICAL, text, ColoramaFore.RED if colorama_imported else None, stack_info)
 
     log_critical = CRITICAL = critical  # Aliases for critical
 
     def debug(self, *args: str, stack_info: Optional[bool] = False) -> None:
         """Log detailed information, typically of interest only when diagnosing problems."""
-        text = ' '.join(args)
+        serialized_args = [str(self._custom_serializer(arg)) for arg in args]
+        text = ' '.join(serialized_args)
         self._log_with_color(logging.DEBUG, text, ColoramaFore.CYAN if colorama_imported else None, stack_info)
 
     log_debug = DEBUG = debug  # Aliases for debug
 
     # Formatting Methods
 
-    def _format_data(self, data, wrap_length=None, max_rows=None, color=True, stack_trace=False):
+    def _format_data(self, data, content=True, wrap_length=None, max_rows=None, color=True, stack_trace=False, indent = 4):
         """Format data for logging, applying wrapping and color formatting where applicable."""
+
+        def serialize(obj):
+            if isinstance(obj, dict):
+                return {key: serialize(value) for key, value in obj.items()}
+            elif isinstance(obj, list):
+                return [serialize(item) for item in obj]
+            elif isinstance(obj, tuple):
+                return tuple(serialize(item) for item in obj)
+            elif isinstance(obj, set):
+                return {serialize(item) for item in obj}
+            elif isinstance(obj, str):
+                return obj
+            else:
+                try:
+                    return json.loads(json.dumps(obj, default=self._custom_serializer, indent=2))
+                except TypeError:
+                    return str(obj)
+
         # Determine the prefix based on the data type
         try:
             import pandas as pd
         except ImportError:
             pd = None
 
         if isinstance(data, dict):
             prefix_str = f"DataType: {type(data).__name__} | Length: {len(data)}"
-            formatted_text = json.dumps(data, indent=4)
+            formatted_text = json.dumps(serialize(data), indent=indent, default=self._custom_serializer)
         elif pd and isinstance(data, pd.DataFrame):
             prefix_str = f"DataType: {type(data).__name__} | Shape: {data.shape[0]} rows | {data.shape[1]} columns"
             with pd.option_context('display.max_rows', max_rows, 'display.max_columns', None):
                 formatted_text = str(data)
         elif isinstance(data, (list, tuple, set)):
             prefix_str = f"DataType: {type(data).__name__} | Length: {len(data)}"
-            formatted_text = '\n'.join([str(item) for item in data])
+            formatted_text = json.dumps(serialize(data), indent=indent, default=self._custom_serializer)
         else:
             prefix_str = f"DataType: {type(data).__name__} | Length: {len(data)}"
-            formatted_text = str(data)
+            formatted_text = json.dumps(serialize(data), indent=indent, default=self._custom_serializer)
+
+        if not content:
+            formatted_text = ""
+            wrapped_text = formatted_text
+        elif wrap_length and not self.running_on_lambda:
+            def wrap_with_indent(line, wrap_length):
+                leading_whitespace = len(line) - len(line.lstrip())
+                wrapped_lines = fill(line, width=wrap_length, subsequent_indent=' ' * leading_whitespace)
+                return wrapped_lines
 
-        # Combine prefix and data, applying wrapping if specified
-        if wrap_length:
-            wrapped_text = '\n'.join([fill(line, wrap_length) for line in formatted_text.splitlines()])
+            wrapped_text = '\n'.join([wrap_with_indent(line, wrap_length) for line in formatted_text.splitlines()])
         else:
             wrapped_text = formatted_text
 
         # Add color and whitespace for visual distinction
         if colorama_imported and color and not self.running_on_lambda:
             if not stack_trace:
                 final_text = f"\n{ColoramaFore.LIGHTBLUE_EX}{prefix_str}\n{ColoramaFore.LIGHTBLACK_EX}{wrapped_text}{ColoramaFore.RESET}\n"
             else:
                 final_text = f"\n{ColoramaFore.LIGHTBLACK_EX}{wrapped_text}{ColoramaFore.RESET}\n"
         elif not self.running_on_lambda:
             final_text = f"\n\n{wrapped_text}\n"
         else:
             # In environments like AWS Lambda, where color might not be supported or desired
-            final_text = wrapped_text.replace("\n", "- - -")
+            final_text = wrapped_text
 
         return final_text
 
     @staticmethod
+    def _custom_serializer(obj):
+        """JSON serializer for objects not serializable by default JSON code"""
+        if isinstance(obj, (datetime, date)):
+            return obj.isoformat()
+        elif isinstance(obj, Decimal):
+            return float(obj)
+        elif hasattr(obj, "__dict__"):
+            return obj.__dict__
+        elif isinstance(obj, str):
+            return obj
+        else:
+            return str(obj)  # Fallback for other types
+
+    @staticmethod
     def _wrap_text(text: str, wrap_length: int) -> str:
         import textwrap
         return '\n'.join(textwrap.wrap(text, wrap_length))
 
     def _log_header(self, text: str, size: int = 80, newline: bool = True) -> None:
         """
         Logs a header text, centered and separated by dashes.
```

### Comparing `WrenchCL-2.1.2/WrenchCL/_Internal/_ConfigurationManager.py` & `WrenchCL-2.1.3/WrenchCL/_Internal/_ConfigurationManager.py`

 * *Files 18% similar despite different names*

```diff
@@ -106,19 +106,25 @@
 
         :returns: The path to the found .env file.
         :rtype: str
         :raises FileNotFoundError: If no .env file is found in the expected locations.
         """
         # Check different potential locations for the .env file
         possible_paths = [Path(__file__).resolve().parent,  # Current directory
-            Path(os.getcwd()),  # Working directory
-            Path(os.getcwd()).joinpath('Resources', 'Secrets'), Path(os.getcwd()).joinpath('resources', 'secrets')]
+                          Path(os.getcwd()),  # Working directory
+                          Path(os.getcwd()).joinpath('Resources', 'Secrets'),
+                          Path(os.getcwd()).joinpath('resources', 'secrets'),
+                          Path(os.getcwd()).parent.joinpath('Resources', 'Secrets'),
+                          Path(os.getcwd()).parent.joinpath('resources', 'secrets'),
+                          Path(os.getcwd()).parent.parent.joinpath('Resources', 'Secrets'),
+                          Path(os.getcwd()).parent.parent.joinpath('resources', 'secrets')]
 
         for base_path in possible_paths:
             env_path = base_path.joinpath('.env')
+            logger.debug('Checking Path', str(env_path))
             if env_path.exists():
                 return str(env_path)
         raise FileNotFoundError("No .env file found in expected locations.")
 
     def _init_from_kwargs(self, kwargs):
         """
         Initializes configuration values from keyword arguments.
```

### Comparing `WrenchCL-2.1.2/WrenchCL/_Internal/_SshTunnelManager.py` & `WrenchCL-2.1.3/WrenchCL/_Internal/_SshTunnelManager.py`

 * *Files identical despite different names*

### Comparing `WrenchCL-2.1.2/WrenchCL.egg-info/PKG-INFO` & `WrenchCL-2.1.3/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,7 @@
-Metadata-Version: 2.1
-Name: WrenchCL
-Version: 2.1.2
-Summary: WrenchCL is a comprehensive library designed to facilitate seamless interactions with AWS services, OpenAI models, and various utility tools. This package aims to streamline the development process by providing robust components for database interactions, cloud storage, and AI-powered functionalities.
-Home-page: https://github.com/WrenchAI/WrenchCL
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.11
-Description-Content-Type: text/markdown
-Provides-Extra: libmagic
-License-File: LICENSE
-
 <h1 align="center">Wrench Code Library</h1>
 
 <p align="center">
     <img src="https://raw.githubusercontent.com/WrenchAI/WrenchCL/release/resources/img/logo.svg" alt="Logo" style="display: inline-block; vertical-align: middle; margin-bottom: -50px; width: 90%; max-width: 800px;">
     <a href="https://pypi.org/project/WrenchCL/" style="text-decoration: none;">
         <img alt="PyPI - Version" src="https://img.shields.io/pypi/v/WrenchCL?logo=pypi&logoColor=green&color=green">
     </a>
@@ -52,15 +39,16 @@
 ```bash
 ImportError: failed to find libmagic.  Check your installation
 ```
 
 Install the package with the optional libmagic dependency, users can using the following command:
 
 ```bash
-pip install WrenchCL[libmagic]
+1. pip uninstall python-magic -y
+2. pip install WrenchCL[libmagic]
 ```
 
 
 # User Guides
 
 Sure! Here's an updated and more detailed README that provides extensive instructions on how to use `AWSClientHub`, `RdsServiceGateway`, `S3ServiceGateway`, `ConversationManager`, `OpenAIFactory`, and `OpenAIGateway`. It also includes practical examples for the `Maybe` monad and other utility tools.
 
@@ -88,15 +76,15 @@
    # Example: Fetching data from the database
    query = "SELECT * FROM your_table"
    data = rds_service.get_data(query)
    print(data)
    ```
 
    **Methods in `RdsServiceGateway`**:
-   - `get_data(query: str, payload: Optional[dict] = None, fetchall: bool = True, accepted_type: Optional[Type] = None, none_is_ok: bool = False, accepted_length: Tuple[Optional[int], Optional[int]] = (None, None)) -> Optional[Any]`
+   - `get_data(query: str, payload: Optional[dict] = None, fetchall: bool = True, return_dict: bool = True, accepted_type: Optional[Type] = None, none_is_ok: bool = False, accepted_length: Tuple[Optional[int], Optional[int]] = (None, None)) -> Optional[Any]`
      - Fetches data from the database based on the input query and parameters.
    - `update_database(query: str, payload: Union[dict, 'pd.DataFrame'], column_order: Optional[List[str]] = None) -> None`
      - Updates the database by executing the given query with the provided payload.
 
 3. **Using `S3ServiceGateway`**:
    ```python
    from WrenchCL.Connect import S3ServiceGateway
@@ -142,36 +130,36 @@
    ```python
    from WrenchCL.Models.OpenAI import OpenAIGateway
 
    # Initialize OpenAIGateway with your OpenAI API key
    openai_gateway = OpenAIGateway(api_key="your_openai_api_key")
 
    # Example: Generating text
-   response = openai_gateway.handle_text("Your prompt here")
+   response = openai_gateway.text_response("Your prompt here")
    print(response)
    ```
 
    **Methods in `OpenAIGateway`**:
-   - `handle_text(text: str, model: str = "gpt-3.5-turbo", system_prompt: Optional[str] = None, image_url: Optional[str] = None, json_mode: bool = False, **kwargs) -> Union[str, dict]`
+   - `text_response(text: str, model: str = "gpt-3.5-turbo", system_prompt: Optional[str] = None, image_url: Optional[str] = None, json_mode: bool = False,  stream : bool = False, **kwargs) -> Union[str, dict]`
      - Processes text input using the specified model and returns the response.
    - `get_embeddings(text: str, model: str = "text-embedding-3-small") -> list`
      - Retrieves embeddings for the given text using the specified model.
-   - `generate_image(prompt: str, size: str = "1024x1024", quality: str = "standard", n: int = 1) -> str`
+   - `text_to_image(prompt: str, size: str = "1024x1024", quality: str = "standard", n: int = 1) -> str`
      - Generates an image based on the provided prompt.
-   - `process_audio(audio_path: str, model: str = "whisper-1") -> str`
+   - `audio_to_text(audio_path: str, model: str = "whisper-1") -> str`
      - Processes an audio file and returns its transcription.
-   - `create_image_variation(image_path: str, n: int = 1, size: str = "1024x1024") -> str`
+   - `generate_image_variations(image_path: str, n: int = 1, size: str = "1024x1024") -> str`
      - Creates variations of an image based on the provided image path.
-   - `edit_image(image_path: str, prompt: str, mask_path: str, n: int = 1, size: str = "1024x1024") -> str`
+   - `modify_image(image_path: str, prompt: str, mask_path: str, n: int = 1, size: str = "1024x1024") -> str`
      - Edits an image based on the provided prompt and mask.
-   - `vision_query(question: str, image_path: str, **kwargs) -> dict`
+   - `image_to_text(question: str, image_path: str, **kwargs) -> dict`
      - Processes a vision query based on the provided question and image.
    - `convert_image_to_url_or_base64(image_path: str) -> str`
      - Converts an image to a URL or base64 encoded string.
-   - `initiate_conversation(initial_text: str, **kwargs)`
+   - `start_conversation(initial_text: str, **kwargs)`
      - Initiates a conversation using the provided initial text.
 
 2. **Using `OpenAIFactory`**:
    ```python
    from WrenchCL.Models.OpenAI import OpenAIFactory
 
    # Initialize OpenAIFactory with your OpenAI API key
@@ -191,14 +179,30 @@
    - `validate_response_with_gpt(initial_response: str, validation_prompt: str) -> str`
      - Uses an initial response and validates or expands upon it with a secondary GPT call.
 
 ### Utility Tools
 
 WrenchCL includes several utility tools for various purposes:
 
+Got it! Here is the section about the custom JSON serializer in the specified format:
+
+### Custom JSON Serializer
+
+- **robust_serializer**: Serializes objects not natively serializable by JSON, including `datetime`, `date`, `Decimal`, and custom objects.
+
+    ```python
+    # Usage with json_dumps
+    from datetime import datetime
+    import json
+    from WrenchCL.Tools import robust_serializer
+
+    print(json.dumps({"timestamp": datetime.now()}, default=robust_serializer))
+    # Output: {"timestamp": "2024-05-17T12:34:56.789012"}
+    ```
+
 - **validate_input_dict**: Validates the input dictionary against expected types.
   ```python
   from WrenchCL.Tools import validate_input_dict
     
   params = {
         'event': 'event_data',
         'context': 'context_data',
```

#### html2text {}

```diff
@@ -1,16 +1,7 @@
-Metadata-Version: 2.1 Name: WrenchCL Version: 2.1.2 Summary: WrenchCL is a
-comprehensive library designed to facilitate seamless interactions with AWS
-services, OpenAI models, and various utility tools. This package aims to
-streamline the development process by providing robust components for database
-interactions, cloud storage, and AI-powered functionalities. Home-page: https:/
-/github.com/WrenchAI/WrenchCL Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License Classifier: Operating System
-:: OS Independent Requires-Python: >=3.11 Description-Content-Type: text/
-markdown Provides-Extra: libmagic License-File: LICENSE
                        ************ WWrreenncchh CCooddee LLiibbrraarryy ************
     [Logo]_[_P_y_P_I_ _-_ _V_e_r_s_i_o_n_]_[_M_a_i_n_t_a_i_n_e_r_]_[_G_i_t_H_u_b_ _W_o_r_k_f_l_o_w_ _S_t_a_t_u_s_ _(_w_i_t_h_ _e_v_e_n_t_)_]
 ## Description WrenchCL is a comprehensive library designed to facilitate
 seamless interactions with AWS services, OpenAI models, and various utility
 tools. This package aims to streamline the development process by providing
 robust components for database interactions, cloud storage, and AI-powered
 functionalities. **PyPI Link:** [WrenchCL on PyPI](https://pypi.org/project/
@@ -21,42 +12,43 @@
 _Internal for interacting with OpenAI models. - **Tools**: Miscellaneous
 utility tools such as coalescing values, file typing, image encoding, and a
 custom logger. - **DataFlow**: Response focused tools to aid in returning
 values and generating logs based on status codes. ## Installation To install
 the package, simply run the following command: ```bash pip install WrenchCL ```
 Upon recieving the below error: ```bash ImportError: failed to find libmagic.
 Check your installation ``` Install the package with the optional libmagic
-dependency, users can using the following command: ```bash pip install WrenchCL
-[libmagic] ``` # User Guides Sure! Here's an updated and more detailed README
-that provides extensive instructions on how to use `AWSClientHub`,
-`RdsServiceGateway`, `S3ServiceGateway`, `ConversationManager`,
-`OpenAIFactory`, and `OpenAIGateway`. It also includes practical examples for
-the `Maybe` monad and other utility tools. ### Connecting to AWS Services To
-interact with AWS RDS and S3 services, follow these steps: 1. **Setup
-`AWSClientHub`**: ```python from WrenchCL.Connections import AwsClientHub #
-Initialize the AWSClientHub using an env file or keyword arguments
-aws_client_hub = AWSClientHub(env_path="path/to/your/env/file") #
+dependency, users can using the following command: ```bash 1. pip uninstall
+python-magic -y 2. pip install WrenchCL[libmagic] ``` # User Guides Sure!
+Here's an updated and more detailed README that provides extensive instructions
+on how to use `AWSClientHub`, `RdsServiceGateway`, `S3ServiceGateway`,
+`ConversationManager`, `OpenAIFactory`, and `OpenAIGateway`. It also includes
+practical examples for the `Maybe` monad and other utility tools. ###
+Connecting to AWS Services To interact with AWS RDS and S3 services, follow
+these steps: 1. **Setup `AWSClientHub`**: ```python from WrenchCL.Connections
+import AwsClientHub # Initialize the AWSClientHub using an env file or keyword
+arguments aws_client_hub = AWSClientHub(env_path="path/to/your/env/file") #
 Alternatively, use keyword arguments or existing env variables # aws_client_hub
 = AWSClientHub(aws_profile='your_profile', region_name='your_region',
 secret_arn='your_secret_arn', ...) ``` 2. **Using `RdsServiceGateway`**:
 ```python from WrenchCL.Connections import RdsServiceGateway # Initialize
 RdsServiceGateway with the AWSClientHub instance rds_service =
 RdsServiceGateway(aws_client_hub) # Example: Fetching data from the database
 query = "SELECT * FROM your_table" data = rds_service.get_data(query) print
 (data) ``` **Methods in `RdsServiceGateway`**: - `get_data(query: str, payload:
-Optional[dict] = None, fetchall: bool = True, accepted_type: Optional[Type] =
-None, none_is_ok: bool = False, accepted_length: Tuple[Optional[int], Optional
-[int]] = (None, None)) -> Optional[Any]` - Fetches data from the database based
-on the input query and parameters. - `update_database(query: str, payload:
-Union[dict, 'pd.DataFrame'], column_order: Optional[List[str]] = None) -> None`
-- Updates the database by executing the given query with the provided payload.
-3. **Using `S3ServiceGateway`**: ```python from WrenchCL.Connect import
-S3ServiceGateway # Initialize S3ServiceGateway with the AWSClientHub instance
-s3_service = S3ServiceGateway(aws_client_hub) # Example: Downloading an object
-from S3 bucket_name = "your-bucket-name" object_key = "path/to/your/object"
+Optional[dict] = None, fetchall: bool = True, return_dict: bool = True,
+accepted_type: Optional[Type] = None, none_is_ok: bool = False,
+accepted_length: Tuple[Optional[int], Optional[int]] = (None, None)) -
+> Optional[Any]` - Fetches data from the database based on the input query and
+parameters. - `update_database(query: str, payload: Union[dict,
+'pd.DataFrame'], column_order: Optional[List[str]] = None) -> None` - Updates
+the database by executing the given query with the provided payload. 3. **Using
+`S3ServiceGateway`**: ```python from WrenchCL.Connect import S3ServiceGateway #
+Initialize S3ServiceGateway with the AWSClientHub instance s3_service =
+S3ServiceGateway(aws_client_hub) # Example: Downloading an object from S3
+bucket_name = "your-bucket-name" object_key = "path/to/your/object"
 s3_service.download_object(bucket_name, object_key, "local/path/to/save") ```
 **Methods in `S3ServiceGateway`**: - `get_object(bucket_name: str, object_key:
 str) -> io.BytesIO` - Retrieves an object from S3. - `download_object
 (bucket_name: str, object_key: str, local_path: str) -> None` - Downloads an
 object from S3 to the local file system. - `get_object_headers(bucket_name:
 str, object_key: str) -> dict` - Retrieves the headers of an object in S3. -
 `upload_object(file_path: str, bucket_name: str, object_key: str) -> None` -
@@ -72,52 +64,60 @@
 an object exists in S3. - `list_objects(bucket_name: str, prefix: Optional[str]
 = None) -> list` - Lists objects in an S3 bucket. - `check_bucket_permissions
 (bucket_name: str) -> dict` - Checks the permissions of an S3 bucket. ###
 Interacting with OpenAI Models To use OpenAI models, follow these steps: 1.
 **Setup `OpenAIGateway`**: ```python from WrenchCL.Models.OpenAI import
 OpenAIGateway # Initialize OpenAIGateway with your OpenAI API key
 openai_gateway = OpenAIGateway(api_key="your_openai_api_key") # Example:
-Generating text response = openai_gateway.handle_text("Your prompt here") print
-(response) ``` **Methods in `OpenAIGateway`**: - `handle_text(text: str, model:
-str = "gpt-3.5-turbo", system_prompt: Optional[str] = None, image_url: Optional
-[str] = None, json_mode: bool = False, **kwargs) -> Union[str, dict]` -
-Processes text input using the specified model and returns the response. -
-`get_embeddings(text: str, model: str = "text-embedding-3-small") -> list` -
-Retrieves embeddings for the given text using the specified model. -
-`generate_image(prompt: str, size: str = "1024x1024", quality: str =
-"standard", n: int = 1) -> str` - Generates an image based on the provided
-prompt. - `process_audio(audio_path: str, model: str = "whisper-1") -> str` -
-Processes an audio file and returns its transcription. -
-`create_image_variation(image_path: str, n: int = 1, size: str = "1024x1024") -
-> str` - Creates variations of an image based on the provided image path. -
-`edit_image(image_path: str, prompt: str, mask_path: str, n: int = 1, size: str
-= "1024x1024") -> str` - Edits an image based on the provided prompt and mask.
-- `vision_query(question: str, image_path: str, **kwargs) -> dict` - Processes
-a vision query based on the provided question and image. -
-`convert_image_to_url_or_base64(image_path: str) -> str` - Converts an image to
-a URL or base64 encoded string. - `initiate_conversation(initial_text: str,
-**kwargs)` - Initiates a conversation using the provided initial text. 2.
-**Using `OpenAIFactory`**: ```python from WrenchCL.Models.OpenAI import
-OpenAIFactory # Initialize OpenAIFactory with your OpenAI API key
-openai_factory = OpenAIFactory(api_key="your_openai_api_key") # Example:
-Transcribing audio to text and getting embeddings audio_path = "path/to/your/
-audio/file" embeddings = openai_factory.audio_to_text_to_embeddings(audio_path)
-print(embeddings) ``` **Methods in `OpenAIFactory`**: -
-`audio_to_text_to_embeddings(audio_path: str, embedding_model: str = "text-
-embedding-3-small") -> list` - Transcribes audio to text and then generates
-embeddings for the text. - `image_to_text_to_embeddings(image_path: str,
-question: str, embedding_model: str = "text-embedding-3-small") -> list` -
-Performs a vision query to understand an image and then generates embeddings
-for the response. - `validate_response_with_gpt(initial_response: str,
-validation_prompt: str) -> str` - Uses an initial response and validates or
-expands upon it with a secondary GPT call. ### Utility Tools WrenchCL includes
-several utility tools for various purposes: - **validate_input_dict**:
-Validates the input dictionary against expected types. ```python from
-WrenchCL.Tools import validate_input_dict params = { 'event': 'event_data',
-'context': 'context_data', 'start_time': 1625256000, 'lambda_client':
+Generating text response = openai_gateway.text_response("Your prompt here")
+print(response) ``` **Methods in `OpenAIGateway`**: - `text_response(text: str,
+model: str = "gpt-3.5-turbo", system_prompt: Optional[str] = None, image_url:
+Optional[str] = None, json_mode: bool = False, stream : bool = False, **kwargs)
+-> Union[str, dict]` - Processes text input using the specified model and
+returns the response. - `get_embeddings(text: str, model: str = "text-
+embedding-3-small") -> list` - Retrieves embeddings for the given text using
+the specified model. - `text_to_image(prompt: str, size: str = "1024x1024",
+quality: str = "standard", n: int = 1) -> str` - Generates an image based on
+the provided prompt. - `audio_to_text(audio_path: str, model: str = "whisper-
+1") -> str` - Processes an audio file and returns its transcription. -
+`generate_image_variations(image_path: str, n: int = 1, size: str =
+"1024x1024") -> str` - Creates variations of an image based on the provided
+image path. - `modify_image(image_path: str, prompt: str, mask_path: str, n:
+int = 1, size: str = "1024x1024") -> str` - Edits an image based on the
+provided prompt and mask. - `image_to_text(question: str, image_path: str,
+**kwargs) -> dict` - Processes a vision query based on the provided question
+and image. - `convert_image_to_url_or_base64(image_path: str) -> str` -
+Converts an image to a URL or base64 encoded string. - `start_conversation
+(initial_text: str, **kwargs)` - Initiates a conversation using the provided
+initial text. 2. **Using `OpenAIFactory`**: ```python from
+WrenchCL.Models.OpenAI import OpenAIFactory # Initialize OpenAIFactory with
+your OpenAI API key openai_factory = OpenAIFactory
+(api_key="your_openai_api_key") # Example: Transcribing audio to text and
+getting embeddings audio_path = "path/to/your/audio/file" embeddings =
+openai_factory.audio_to_text_to_embeddings(audio_path) print(embeddings) ```
+**Methods in `OpenAIFactory`**: - `audio_to_text_to_embeddings(audio_path: str,
+embedding_model: str = "text-embedding-3-small") -> list` - Transcribes audio
+to text and then generates embeddings for the text. -
+`image_to_text_to_embeddings(image_path: str, question: str, embedding_model:
+str = "text-embedding-3-small") -> list` - Performs a vision query to
+understand an image and then generates embeddings for the response. -
+`validate_response_with_gpt(initial_response: str, validation_prompt: str) -
+> str` - Uses an initial response and validates or expands upon it with a
+secondary GPT call. ### Utility Tools WrenchCL includes several utility tools
+for various purposes: Got it! Here is the section about the custom JSON
+serializer in the specified format: ### Custom JSON Serializer -
+**robust_serializer**: Serializes objects not natively serializable by JSON,
+including `datetime`, `date`, `Decimal`, and custom objects. ```python # Usage
+with json_dumps from datetime import datetime import json from WrenchCL.Tools
+import robust_serializer print(json.dumps({"timestamp": datetime.now()},
+default=robust_serializer)) # Output: {"timestamp": "2024-05-17T12:34:
+56.789012"} ``` - **validate_input_dict**: Validates the input dictionary
+against expected types. ```python from WrenchCL.Tools import
+validate_input_dict params = { 'event': 'event_data', 'context':
+'context_data', 'start_time': 1625256000, 'lambda_client':
 'lambda_client_instance' } expected_types = { 'event': str, 'context': str,
 'start_time': (int, float), 'lambda_client': object, } validate_input_dict
 (params, expected_types) ``` - **Coalesce**: A utility function to return the
 first non-null value. ```python from WrenchCL.Tools import coalesce result =
 coalesce(None, "default_value") print(result) # Output: "default_value" ``` -
 **FileTyper**: A utility for determining file types. ```python from
 WrenchCL.Tools import get_file_type file_type = get_file_type("path/to/your/
```

### Comparing `WrenchCL-2.1.2/WrenchCL.egg-info/SOURCES.txt` & `WrenchCL-2.1.3/WrenchCL.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -25,13 +25,14 @@
 WrenchCL/Models/OpenAI/_ConversationManager.py
 WrenchCL/Models/OpenAI/__init__.py
 WrenchCL/Tools/Coalesce.py
 WrenchCL/Tools/DictValidator.py
 WrenchCL/Tools/FetchMetaData.py
 WrenchCL/Tools/FileTyper.py
 WrenchCL/Tools/Image2B64.py
+WrenchCL/Tools/JsonSerializer.py
 WrenchCL/Tools/MaybeMonad.py
 WrenchCL/Tools/WrenchLogger.py
 WrenchCL/Tools/__init__.py
 WrenchCL/_Internal/_ConfigurationManager.py
 WrenchCL/_Internal/_SshTunnelManager.py
 WrenchCL/_Internal/__init__.py
```

### Comparing `WrenchCL-2.1.2/setup.py` & `WrenchCL-2.1.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -29,14 +29,14 @@
         if os.path.exists(requires_path):
             with open(requires_path, "r", encoding="utf-8") as f:
                 required = f.read().splitlines()
 
 # Define the optional dependencies
 extras = {'libmagic': ['python-magic-bin~=0.4.14']}
 
-setup(name='WrenchCL', version='v2.1.2',
-    description='WrenchCL is a comprehensive library designed to facilitate seamless interactions with AWS services, OpenAI models, and various utility tools. This package aims to streamline the development process by providing robust components for database interactions, cloud storage, and AI-powered functionalities.',
-    long_description=long_description, long_description_content_type="text/markdown",
-    url='https://github.com/WrenchAI/WrenchCL', packages=find_packages(), install_requires=required,
-    extras_require=extras, python_requires='>=3.11',
-    classifiers=['Programming Language :: Python :: 3', 'License :: OSI Approved :: MIT License',
-        'Operating System :: OS Independent', ], )
+setup(name='WrenchCL', version='v2.1.3',
+      description='WrenchCL is a comprehensive library designed to facilitate seamless interactions with AWS services, OpenAI models, and various utility tools. This package aims to streamline the development process by providing robust components for database interactions, cloud storage, and AI-powered functionalities.',
+      long_description=long_description, long_description_content_type="text/markdown",
+      url='https://github.com/WrenchAI/WrenchCL', packages=find_packages(), install_requires=required,
+      extras_require=extras, python_requires='>=3.11',
+      classifiers=['Programming Language :: Python :: 3', 'License :: OSI Approved :: MIT License',
+                   'Operating System :: OS Independent', ], )
```

