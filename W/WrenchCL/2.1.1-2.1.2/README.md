# Comparing `tmp/WrenchCL-2.1.1.tar.gz` & `tmp/WrenchCL-2.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "WrenchCL-2.1.1.tar", last modified: Fri May 17 19:55:57 2024, max compression
+gzip compressed data, was "WrenchCL-2.1.2.tar", last modified: Fri May 17 20:09:59 2024, max compression
```

## Comparing `WrenchCL-2.1.1.tar` & `WrenchCL-2.1.2.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 19:55:57.540559 WrenchCL-2.1.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1421 2024-05-17 19:55:31.000000 WrenchCL-2.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    22624 2024-05-17 19:55:57.540559 WrenchCL-2.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    21954 2024-05-17 19:55:31.000000 WrenchCL-2.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 19:55:57.536559 WrenchCL-2.1.1/WrenchCL/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 19:55:57.536559 WrenchCL-2.1.1/WrenchCL/Connect/
--rw-r--r--   0 runner    (1001) docker     (127)    10104 2024-05-17 19:55:31.000000 WrenchCL-2.1.1/WrenchCL/Connect/AwsClientHub.py
--rw-r--r--   0 runner    (1001) docker     (127)     8307 2024-05-17 19:55:31.000000 WrenchCL-2.1.1/WrenchCL/Connect/RdsServiceGateway.py
--rw-r--r--   0 runner    (1001) docker     (127)    10985 2024-05-17 19:55:31.000000 WrenchCL-2.1.1/WrenchCL/Connect/S3ServiceGateway.py
--rw-r--r--   0 runner    (1001) docker     (127)      236 2024-05-17 19:55:31.000000 WrenchCL-2.1.1/WrenchCL/Connect/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 19:55:57.536559 WrenchCL-2.1.1/WrenchCL/DataFlow/
--rw-r--r--   0 runner    (1001) docker     (127)      412 2024-05-17 19:55:31.000000 WrenchCL-2.1.1/WrenchCL/DataFlow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2954 2024-05-17 19:55:31.000000 WrenchCL-2.1.1/WrenchCL/DataFlow/build_return_json.py
--rw-r--r--   0 runner    (1001) docker     (127)     9123 2024-05-17 19:55:31.000000 WrenchCL-2.1.1/WrenchCL/DataFlow/handle_lambda_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    10837 2024-05-17 19:55:31.000000 WrenchCL-2.1.1/WrenchCL/DataFlow/trigger_dataflow_metrics.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 19:55:57.536559 WrenchCL-2.1.1/WrenchCL/Decorators/
--rw-r--r--   0 runner    (1001) docker     (127)     3656 2024-05-17 19:55:31.000000 WrenchCL-2.1.1/WrenchCL/Decorators/Retryable.py
--rw-r--r--   0 runner    (1001) docker     (127)     3116 2024-05-17 19:55:31.000000 WrenchCL-2.1.1/WrenchCL/Decorators/SingletonClass.py
--rw-r--r--   0 runner    (1001) docker     (127)     2541 2024-05-17 19:55:31.000000 WrenchCL-2.1.1/WrenchCL/Decorators/TimedMethod.py
--rw-r--r--   0 runner    (1001) docker     (127)      206 2024-05-17 19:55:31.000000 WrenchCL-2.1.1/WrenchCL/Decorators/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 19:55:57.540559 WrenchCL-2.1.1/WrenchCL/Models/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 19:55:57.540559 WrenchCL-2.1.1/WrenchCL/Models/OpenAI/
--rw-r--r--   0 runner    (1001) docker     (127)     4853 2024-05-17 19:55:31.000000 WrenchCL-2.1.1/WrenchCL/Models/OpenAI/OpenAIFactory.py
--rw-r--r--   0 runner    (1001) docker     (127)    15468 2024-05-17 19:55:31.000000 WrenchCL-2.1.1/WrenchCL/Models/OpenAI/OpenAIGateway.py
--rw-r--r--   0 runner    (1001) docker     (127)     7292 2024-05-17 19:55:31.000000 WrenchCL-2.1.1/WrenchCL/Models/OpenAI/_ConversationManager.py
--rw-r--r--   0 runner    (1001) docker     (127)     1651 2024-05-17 19:55:31.000000 WrenchCL-2.1.1/WrenchCL/Models/OpenAI/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-17 19:55:31.000000 WrenchCL-2.1.1/WrenchCL/Models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 19:55:57.540559 WrenchCL-2.1.1/WrenchCL/Tools/
--rw-r--r--   0 runner    (1001) docker     (127)     2196 2024-05-17 19:55:31.000000 WrenchCL-2.1.1/WrenchCL/Tools/Coalesce.py
--rw-r--r--   0 runner    (1001) docker     (127)     5888 2024-05-17 19:55:31.000000 WrenchCL-2.1.1/WrenchCL/Tools/DictValidator.py
--rw-r--r--   0 runner    (1001) docker     (127)     2930 2024-05-17 19:55:31.000000 WrenchCL-2.1.1/WrenchCL/Tools/FetchMetaData.py
--rw-r--r--   0 runner    (1001) docker     (127)     2360 2024-05-17 19:55:31.000000 WrenchCL-2.1.1/WrenchCL/Tools/FileTyper.py
--rw-r--r--   0 runner    (1001) docker     (127)     2485 2024-05-17 19:55:31.000000 WrenchCL-2.1.1/WrenchCL/Tools/Image2B64.py
--rw-r--r--   0 runner    (1001) docker     (127)     5414 2024-05-17 19:55:31.000000 WrenchCL-2.1.1/WrenchCL/Tools/MaybeMonad.py
--rw-r--r--   0 runner    (1001) docker     (127)    28041 2024-05-17 19:55:31.000000 WrenchCL-2.1.1/WrenchCL/Tools/WrenchLogger.py
--rw-r--r--   0 runner    (1001) docker     (127)      404 2024-05-17 19:55:31.000000 WrenchCL-2.1.1/WrenchCL/Tools/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 19:55:57.540559 WrenchCL-2.1.1/WrenchCL/_Internal/
--rw-r--r--   0 runner    (1001) docker     (127)     6964 2024-05-17 19:55:31.000000 WrenchCL-2.1.1/WrenchCL/_Internal/_ConfigurationManager.py
--rw-r--r--   0 runner    (1001) docker     (127)     4086 2024-05-17 19:55:31.000000 WrenchCL-2.1.1/WrenchCL/_Internal/_SshTunnelManager.py
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-17 19:55:31.000000 WrenchCL-2.1.1/WrenchCL/_Internal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       92 2024-05-17 19:55:31.000000 WrenchCL-2.1.1/WrenchCL/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 19:55:57.536559 WrenchCL-2.1.1/WrenchCL.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    22624 2024-05-17 19:55:57.000000 WrenchCL-2.1.1/WrenchCL.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1179 2024-05-17 19:55:57.000000 WrenchCL-2.1.1/WrenchCL.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-17 19:55:57.000000 WrenchCL-2.1.1/WrenchCL.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      227 2024-05-17 19:55:57.000000 WrenchCL-2.1.1/WrenchCL.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-17 19:55:57.000000 WrenchCL-2.1.1/WrenchCL.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-17 19:55:57.540559 WrenchCL-2.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2248 2024-05-17 19:55:56.000000 WrenchCL-2.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 20:09:59.048343 WrenchCL-2.1.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1421 2024-05-17 20:09:37.000000 WrenchCL-2.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    22877 2024-05-17 20:09:59.048343 WrenchCL-2.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    22207 2024-05-17 20:09:37.000000 WrenchCL-2.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 20:09:59.040343 WrenchCL-2.1.2/WrenchCL/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 20:09:59.044343 WrenchCL-2.1.2/WrenchCL/Connect/
+-rw-r--r--   0 runner    (1001) docker     (127)    10104 2024-05-17 20:09:37.000000 WrenchCL-2.1.2/WrenchCL/Connect/AwsClientHub.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8307 2024-05-17 20:09:37.000000 WrenchCL-2.1.2/WrenchCL/Connect/RdsServiceGateway.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10985 2024-05-17 20:09:37.000000 WrenchCL-2.1.2/WrenchCL/Connect/S3ServiceGateway.py
+-rw-r--r--   0 runner    (1001) docker     (127)      236 2024-05-17 20:09:37.000000 WrenchCL-2.1.2/WrenchCL/Connect/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 20:09:59.044343 WrenchCL-2.1.2/WrenchCL/DataFlow/
+-rw-r--r--   0 runner    (1001) docker     (127)      412 2024-05-17 20:09:37.000000 WrenchCL-2.1.2/WrenchCL/DataFlow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2954 2024-05-17 20:09:37.000000 WrenchCL-2.1.2/WrenchCL/DataFlow/build_return_json.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9123 2024-05-17 20:09:37.000000 WrenchCL-2.1.2/WrenchCL/DataFlow/handle_lambda_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10837 2024-05-17 20:09:37.000000 WrenchCL-2.1.2/WrenchCL/DataFlow/trigger_dataflow_metrics.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 20:09:59.044343 WrenchCL-2.1.2/WrenchCL/Decorators/
+-rw-r--r--   0 runner    (1001) docker     (127)     3656 2024-05-17 20:09:37.000000 WrenchCL-2.1.2/WrenchCL/Decorators/Retryable.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3116 2024-05-17 20:09:37.000000 WrenchCL-2.1.2/WrenchCL/Decorators/SingletonClass.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2541 2024-05-17 20:09:37.000000 WrenchCL-2.1.2/WrenchCL/Decorators/TimedMethod.py
+-rw-r--r--   0 runner    (1001) docker     (127)      206 2024-05-17 20:09:37.000000 WrenchCL-2.1.2/WrenchCL/Decorators/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 20:09:59.044343 WrenchCL-2.1.2/WrenchCL/Models/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 20:09:59.044343 WrenchCL-2.1.2/WrenchCL/Models/OpenAI/
+-rw-r--r--   0 runner    (1001) docker     (127)     4853 2024-05-17 20:09:37.000000 WrenchCL-2.1.2/WrenchCL/Models/OpenAI/OpenAIFactory.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15468 2024-05-17 20:09:37.000000 WrenchCL-2.1.2/WrenchCL/Models/OpenAI/OpenAIGateway.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7292 2024-05-17 20:09:37.000000 WrenchCL-2.1.2/WrenchCL/Models/OpenAI/_ConversationManager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1651 2024-05-17 20:09:37.000000 WrenchCL-2.1.2/WrenchCL/Models/OpenAI/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-17 20:09:37.000000 WrenchCL-2.1.2/WrenchCL/Models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 20:09:59.048343 WrenchCL-2.1.2/WrenchCL/Tools/
+-rw-r--r--   0 runner    (1001) docker     (127)     2196 2024-05-17 20:09:37.000000 WrenchCL-2.1.2/WrenchCL/Tools/Coalesce.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5888 2024-05-17 20:09:37.000000 WrenchCL-2.1.2/WrenchCL/Tools/DictValidator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3233 2024-05-17 20:09:37.000000 WrenchCL-2.1.2/WrenchCL/Tools/FetchMetaData.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2661 2024-05-17 20:09:37.000000 WrenchCL-2.1.2/WrenchCL/Tools/FileTyper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2485 2024-05-17 20:09:37.000000 WrenchCL-2.1.2/WrenchCL/Tools/Image2B64.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5414 2024-05-17 20:09:37.000000 WrenchCL-2.1.2/WrenchCL/Tools/MaybeMonad.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28041 2024-05-17 20:09:37.000000 WrenchCL-2.1.2/WrenchCL/Tools/WrenchLogger.py
+-rw-r--r--   0 runner    (1001) docker     (127)      404 2024-05-17 20:09:37.000000 WrenchCL-2.1.2/WrenchCL/Tools/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 20:09:59.048343 WrenchCL-2.1.2/WrenchCL/_Internal/
+-rw-r--r--   0 runner    (1001) docker     (127)     6964 2024-05-17 20:09:37.000000 WrenchCL-2.1.2/WrenchCL/_Internal/_ConfigurationManager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4086 2024-05-17 20:09:37.000000 WrenchCL-2.1.2/WrenchCL/_Internal/_SshTunnelManager.py
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-17 20:09:37.000000 WrenchCL-2.1.2/WrenchCL/_Internal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-05-17 20:09:37.000000 WrenchCL-2.1.2/WrenchCL/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 20:09:59.044343 WrenchCL-2.1.2/WrenchCL.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    22877 2024-05-17 20:09:59.000000 WrenchCL-2.1.2/WrenchCL.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1179 2024-05-17 20:09:59.000000 WrenchCL-2.1.2/WrenchCL.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-17 20:09:59.000000 WrenchCL-2.1.2/WrenchCL.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      264 2024-05-17 20:09:59.000000 WrenchCL-2.1.2/WrenchCL.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-17 20:09:59.000000 WrenchCL-2.1.2/WrenchCL.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-17 20:09:59.048343 WrenchCL-2.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1938 2024-05-17 20:09:57.000000 WrenchCL-2.1.2/setup.py
```

### Comparing `WrenchCL-2.1.1/LICENSE` & `WrenchCL-2.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `WrenchCL-2.1.1/PKG-INFO` & `WrenchCL-2.1.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: WrenchCL
-Version: 2.1.1
+Version: 2.1.2
 Summary: WrenchCL is a comprehensive library designed to facilitate seamless interactions with AWS services, OpenAI models, and various utility tools. This package aims to streamline the development process by providing robust components for database interactions, cloud storage, and AI-powered functionalities.
 Home-page: https://github.com/WrenchAI/WrenchCL
-Author: willem@wrench.ai
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
+Provides-Extra: libmagic
 License-File: LICENSE
 
 <h1 align="center">Wrench Code Library</h1>
 
 <p align="center">
     <img src="https://raw.githubusercontent.com/WrenchAI/WrenchCL/release/resources/img/logo.svg" alt="Logo" style="display: inline-block; vertical-align: middle; margin-bottom: -50px; width: 90%; max-width: 800px;">
     <a href="https://pypi.org/project/WrenchCL/" style="text-decoration: none;">
@@ -43,14 +43,26 @@
 ## Installation
 
 To install the package, simply run the following command:
 
 ```bash
 pip install WrenchCL
 ```
+Upon recieving the below error: 
+
+```bash
+ImportError: failed to find libmagic.  Check your installation
+```
+
+Install the package with the optional libmagic dependency, users can using the following command:
+
+```bash
+pip install WrenchCL[libmagic]
+```
+
 
 # User Guides
 
 Sure! Here's an updated and more detailed README that provides extensive instructions on how to use `AWSClientHub`, `RdsServiceGateway`, `S3ServiceGateway`, `ConversationManager`, `OpenAIFactory`, and `OpenAIGateway`. It also includes practical examples for the `Maybe` monad and other utility tools.
 
 ### Connecting to AWS Services
```

#### html2text {}

```diff
@@ -1,16 +1,16 @@
-Metadata-Version: 2.1 Name: WrenchCL Version: 2.1.1 Summary: WrenchCL is a
+Metadata-Version: 2.1 Name: WrenchCL Version: 2.1.2 Summary: WrenchCL is a
 comprehensive library designed to facilitate seamless interactions with AWS
 services, OpenAI models, and various utility tools. This package aims to
 streamline the development process by providing robust components for database
 interactions, cloud storage, and AI-powered functionalities. Home-page: https:/
-/github.com/WrenchAI/WrenchCL Author: willem@wrench.ai Classifier: Programming
-Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent Requires-Python: >=3.11
-Description-Content-Type: text/markdown License-File: LICENSE
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
@@ -19,25 +19,28 @@
 AWS RDS and S3 services and the `AWSClientHub`. - **Decorators**: Utility
 decorators for retry logic, singleton pattern, and method timing. - **Models**:
 _Internal for interacting with OpenAI models. - **Tools**: Miscellaneous
 utility tools such as coalescing values, file typing, image encoding, and a
 custom logger. - **DataFlow**: Response focused tools to aid in returning
 values and generating logs based on status codes. ## Installation To install
 the package, simply run the following command: ```bash pip install WrenchCL ```
-# User Guides Sure! Here's an updated and more detailed README that provides
-extensive instructions on how to use `AWSClientHub`, `RdsServiceGateway`,
-`S3ServiceGateway`, `ConversationManager`, `OpenAIFactory`, and
-`OpenAIGateway`. It also includes practical examples for the `Maybe` monad and
-other utility tools. ### Connecting to AWS Services To interact with AWS RDS
-and S3 services, follow these steps: 1. **Setup `AWSClientHub`**: ```python
-from WrenchCL.Connections import AwsClientHub # Initialize the AWSClientHub
-using an env file or keyword arguments aws_client_hub = AWSClientHub
-(env_path="path/to/your/env/file") # Alternatively, use keyword arguments or
-existing env variables # aws_client_hub = AWSClientHub
-(aws_profile='your_profile', region_name='your_region',
+Upon recieving the below error: ```bash ImportError: failed to find libmagic.
+Check your installation ``` Install the package with the optional libmagic
+dependency, users can using the following command: ```bash pip install WrenchCL
+[libmagic] ``` # User Guides Sure! Here's an updated and more detailed README
+that provides extensive instructions on how to use `AWSClientHub`,
+`RdsServiceGateway`, `S3ServiceGateway`, `ConversationManager`,
+`OpenAIFactory`, and `OpenAIGateway`. It also includes practical examples for
+the `Maybe` monad and other utility tools. ### Connecting to AWS Services To
+interact with AWS RDS and S3 services, follow these steps: 1. **Setup
+`AWSClientHub`**: ```python from WrenchCL.Connections import AwsClientHub #
+Initialize the AWSClientHub using an env file or keyword arguments
+aws_client_hub = AWSClientHub(env_path="path/to/your/env/file") #
+Alternatively, use keyword arguments or existing env variables # aws_client_hub
+= AWSClientHub(aws_profile='your_profile', region_name='your_region',
 secret_arn='your_secret_arn', ...) ``` 2. **Using `RdsServiceGateway`**:
 ```python from WrenchCL.Connections import RdsServiceGateway # Initialize
 RdsServiceGateway with the AWSClientHub instance rds_service =
 RdsServiceGateway(aws_client_hub) # Example: Fetching data from the database
 query = "SELECT * FROM your_table" data = rds_service.get_data(query) print
 (data) ``` **Methods in `RdsServiceGateway`**: - `get_data(query: str, payload:
 Optional[dict] = None, fetchall: bool = True, accepted_type: Optional[Type] =
```

### Comparing `WrenchCL-2.1.1/README.md` & `WrenchCL-2.1.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -30,14 +30,26 @@
 ## Installation
 
 To install the package, simply run the following command:
 
 ```bash
 pip install WrenchCL
 ```
+Upon recieving the below error: 
+
+```bash
+ImportError: failed to find libmagic.  Check your installation
+```
+
+Install the package with the optional libmagic dependency, users can using the following command:
+
+```bash
+pip install WrenchCL[libmagic]
+```
+
 
 # User Guides
 
 Sure! Here's an updated and more detailed README that provides extensive instructions on how to use `AWSClientHub`, `RdsServiceGateway`, `S3ServiceGateway`, `ConversationManager`, `OpenAIFactory`, and `OpenAIGateway`. It also includes practical examples for the `Maybe` monad and other utility tools.
 
 ### Connecting to AWS Services
```

#### html2text {}

```diff
@@ -10,25 +10,28 @@
 AWS RDS and S3 services and the `AWSClientHub`. - **Decorators**: Utility
 decorators for retry logic, singleton pattern, and method timing. - **Models**:
 _Internal for interacting with OpenAI models. - **Tools**: Miscellaneous
 utility tools such as coalescing values, file typing, image encoding, and a
 custom logger. - **DataFlow**: Response focused tools to aid in returning
 values and generating logs based on status codes. ## Installation To install
 the package, simply run the following command: ```bash pip install WrenchCL ```
-# User Guides Sure! Here's an updated and more detailed README that provides
-extensive instructions on how to use `AWSClientHub`, `RdsServiceGateway`,
-`S3ServiceGateway`, `ConversationManager`, `OpenAIFactory`, and
-`OpenAIGateway`. It also includes practical examples for the `Maybe` monad and
-other utility tools. ### Connecting to AWS Services To interact with AWS RDS
-and S3 services, follow these steps: 1. **Setup `AWSClientHub`**: ```python
-from WrenchCL.Connections import AwsClientHub # Initialize the AWSClientHub
-using an env file or keyword arguments aws_client_hub = AWSClientHub
-(env_path="path/to/your/env/file") # Alternatively, use keyword arguments or
-existing env variables # aws_client_hub = AWSClientHub
-(aws_profile='your_profile', region_name='your_region',
+Upon recieving the below error: ```bash ImportError: failed to find libmagic.
+Check your installation ``` Install the package with the optional libmagic
+dependency, users can using the following command: ```bash pip install WrenchCL
+[libmagic] ``` # User Guides Sure! Here's an updated and more detailed README
+that provides extensive instructions on how to use `AWSClientHub`,
+`RdsServiceGateway`, `S3ServiceGateway`, `ConversationManager`,
+`OpenAIFactory`, and `OpenAIGateway`. It also includes practical examples for
+the `Maybe` monad and other utility tools. ### Connecting to AWS Services To
+interact with AWS RDS and S3 services, follow these steps: 1. **Setup
+`AWSClientHub`**: ```python from WrenchCL.Connections import AwsClientHub #
+Initialize the AWSClientHub using an env file or keyword arguments
+aws_client_hub = AWSClientHub(env_path="path/to/your/env/file") #
+Alternatively, use keyword arguments or existing env variables # aws_client_hub
+= AWSClientHub(aws_profile='your_profile', region_name='your_region',
 secret_arn='your_secret_arn', ...) ``` 2. **Using `RdsServiceGateway`**:
 ```python from WrenchCL.Connections import RdsServiceGateway # Initialize
 RdsServiceGateway with the AWSClientHub instance rds_service =
 RdsServiceGateway(aws_client_hub) # Example: Fetching data from the database
 query = "SELECT * FROM your_table" data = rds_service.get_data(query) print
 (data) ``` **Methods in `RdsServiceGateway`**: - `get_data(query: str, payload:
 Optional[dict] = None, fetchall: bool = True, accepted_type: Optional[Type] =
```

### Comparing `WrenchCL-2.1.1/WrenchCL/Connect/AwsClientHub.py` & `WrenchCL-2.1.2/WrenchCL/Connect/AwsClientHub.py`

 * *Files identical despite different names*

### Comparing `WrenchCL-2.1.1/WrenchCL/Connect/RdsServiceGateway.py` & `WrenchCL-2.1.2/WrenchCL/Connect/RdsServiceGateway.py`

 * *Files identical despite different names*

### Comparing `WrenchCL-2.1.1/WrenchCL/Connect/S3ServiceGateway.py` & `WrenchCL-2.1.2/WrenchCL/Connect/S3ServiceGateway.py`

 * *Files identical despite different names*

### Comparing `WrenchCL-2.1.1/WrenchCL/DataFlow/build_return_json.py` & `WrenchCL-2.1.2/WrenchCL/DataFlow/build_return_json.py`

 * *Files identical despite different names*

### Comparing `WrenchCL-2.1.1/WrenchCL/DataFlow/handle_lambda_response.py` & `WrenchCL-2.1.2/WrenchCL/DataFlow/handle_lambda_response.py`

 * *Files identical despite different names*

### Comparing `WrenchCL-2.1.1/WrenchCL/DataFlow/trigger_dataflow_metrics.py` & `WrenchCL-2.1.2/WrenchCL/DataFlow/trigger_dataflow_metrics.py`

 * *Files identical despite different names*

### Comparing `WrenchCL-2.1.1/WrenchCL/Decorators/Retryable.py` & `WrenchCL-2.1.2/WrenchCL/Decorators/Retryable.py`

 * *Files identical despite different names*

### Comparing `WrenchCL-2.1.1/WrenchCL/Decorators/SingletonClass.py` & `WrenchCL-2.1.2/WrenchCL/Decorators/SingletonClass.py`

 * *Files identical despite different names*

### Comparing `WrenchCL-2.1.1/WrenchCL/Decorators/TimedMethod.py` & `WrenchCL-2.1.2/WrenchCL/Decorators/TimedMethod.py`

 * *Files identical despite different names*

### Comparing `WrenchCL-2.1.1/WrenchCL/Models/OpenAI/OpenAIFactory.py` & `WrenchCL-2.1.2/WrenchCL/Models/OpenAI/OpenAIFactory.py`

 * *Files identical despite different names*

### Comparing `WrenchCL-2.1.1/WrenchCL/Models/OpenAI/OpenAIGateway.py` & `WrenchCL-2.1.2/WrenchCL/Models/OpenAI/OpenAIGateway.py`

 * *Files identical despite different names*

### Comparing `WrenchCL-2.1.1/WrenchCL/Models/OpenAI/_ConversationManager.py` & `WrenchCL-2.1.2/WrenchCL/Models/OpenAI/_ConversationManager.py`

 * *Files identical despite different names*

### Comparing `WrenchCL-2.1.1/WrenchCL/Models/OpenAI/__init__.py` & `WrenchCL-2.1.2/WrenchCL/Models/OpenAI/__init__.py`

 * *Files identical despite different names*

### Comparing `WrenchCL-2.1.1/WrenchCL/Tools/Coalesce.py` & `WrenchCL-2.1.2/WrenchCL/Tools/Coalesce.py`

 * *Files identical despite different names*

### Comparing `WrenchCL-2.1.1/WrenchCL/Tools/DictValidator.py` & `WrenchCL-2.1.2/WrenchCL/Tools/DictValidator.py`

 * *Files identical despite different names*

### Comparing `WrenchCL-2.1.1/WrenchCL/Tools/FetchMetaData.py` & `WrenchCL-2.1.2/WrenchCL/Tools/FetchMetaData.py`

 * *Files 21% similar despite different names*

```diff
@@ -11,15 +11,25 @@
 #  All works within the Software are owned by their respective creators and are distributed by Wrench.AI.
 #
 #  For inquiries, please contact Willem van der Schans through the official Wrench.AI channels or directly via GitHub at [Kydoimos97](https://github.com/Kydoimos97).
 #
 
 import os
 import requests
-import magic
+
+try:
+    import magic
+except ImportError as e:
+    raise ImportError(
+        "Failed to import 'magic'. Please install the appropriate library. "
+        "On Windows, you can install it with:\n"
+        "pip install WrenchCL[libmagic]\n"
+        "On other platforms, ensure 'libmagic' is installed."
+    ) from e
+
 from datetime import datetime
 
 def get_metadata(file_source, is_url=True):
     """
     Get metadata of a file from a URL or file path.
 
     :param file_source: URL or file path of the file
```

### Comparing `WrenchCL-2.1.1/WrenchCL/Tools/FileTyper.py` & `WrenchCL-2.1.2/WrenchCL/Tools/FileTyper.py`

 * *Files 14% similar despite different names*

```diff
@@ -10,15 +10,23 @@
 #
 #  All works within the Software are owned by their respective creators and are distributed by Wrench.AI.
 #
 #  For inquiries, please contact Willem van der Schans through the official Wrench.AI channels or directly via GitHub at [Kydoimos97](https://github.com/Kydoimos97).
 #
 import mimetypes
 import requests
-import magic
+try:
+    import magic
+except ImportError as e:
+    raise ImportError(
+        "Failed to import 'magic'. Please install the appropriate library. "
+        "On Windows, you can install it with:\n"
+        "pip install WrenchCL[libmagic]\n"
+        "On other platforms, ensure 'libmagic' is installed."
+    ) from e
 
 
 def get_file_type(file_source, is_url=True):
     """
     Determine the file type of a file from a URL or file path.
 
     :param file_source: URL or file path of the file
```

### Comparing `WrenchCL-2.1.1/WrenchCL/Tools/Image2B64.py` & `WrenchCL-2.1.2/WrenchCL/Tools/Image2B64.py`

 * *Files identical despite different names*

### Comparing `WrenchCL-2.1.1/WrenchCL/Tools/MaybeMonad.py` & `WrenchCL-2.1.2/WrenchCL/Tools/MaybeMonad.py`

 * *Files identical despite different names*

### Comparing `WrenchCL-2.1.1/WrenchCL/Tools/WrenchLogger.py` & `WrenchCL-2.1.2/WrenchCL/Tools/WrenchLogger.py`

 * *Files identical despite different names*

### Comparing `WrenchCL-2.1.1/WrenchCL/_Internal/_ConfigurationManager.py` & `WrenchCL-2.1.2/WrenchCL/_Internal/_ConfigurationManager.py`

 * *Files identical despite different names*

### Comparing `WrenchCL-2.1.1/WrenchCL/_Internal/_SshTunnelManager.py` & `WrenchCL-2.1.2/WrenchCL/_Internal/_SshTunnelManager.py`

 * *Files identical despite different names*

### Comparing `WrenchCL-2.1.1/WrenchCL.egg-info/PKG-INFO` & `WrenchCL-2.1.2/WrenchCL.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: WrenchCL
-Version: 2.1.1
+Version: 2.1.2
 Summary: WrenchCL is a comprehensive library designed to facilitate seamless interactions with AWS services, OpenAI models, and various utility tools. This package aims to streamline the development process by providing robust components for database interactions, cloud storage, and AI-powered functionalities.
 Home-page: https://github.com/WrenchAI/WrenchCL
-Author: willem@wrench.ai
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
+Provides-Extra: libmagic
 License-File: LICENSE
 
 <h1 align="center">Wrench Code Library</h1>
 
 <p align="center">
     <img src="https://raw.githubusercontent.com/WrenchAI/WrenchCL/release/resources/img/logo.svg" alt="Logo" style="display: inline-block; vertical-align: middle; margin-bottom: -50px; width: 90%; max-width: 800px;">
     <a href="https://pypi.org/project/WrenchCL/" style="text-decoration: none;">
@@ -43,14 +43,26 @@
 ## Installation
 
 To install the package, simply run the following command:
 
 ```bash
 pip install WrenchCL
 ```
+Upon recieving the below error: 
+
+```bash
+ImportError: failed to find libmagic.  Check your installation
+```
+
+Install the package with the optional libmagic dependency, users can using the following command:
+
+```bash
+pip install WrenchCL[libmagic]
+```
+
 
 # User Guides
 
 Sure! Here's an updated and more detailed README that provides extensive instructions on how to use `AWSClientHub`, `RdsServiceGateway`, `S3ServiceGateway`, `ConversationManager`, `OpenAIFactory`, and `OpenAIGateway`. It also includes practical examples for the `Maybe` monad and other utility tools.
 
 ### Connecting to AWS Services
```

#### html2text {}

```diff
@@ -1,16 +1,16 @@
-Metadata-Version: 2.1 Name: WrenchCL Version: 2.1.1 Summary: WrenchCL is a
+Metadata-Version: 2.1 Name: WrenchCL Version: 2.1.2 Summary: WrenchCL is a
 comprehensive library designed to facilitate seamless interactions with AWS
 services, OpenAI models, and various utility tools. This package aims to
 streamline the development process by providing robust components for database
 interactions, cloud storage, and AI-powered functionalities. Home-page: https:/
-/github.com/WrenchAI/WrenchCL Author: willem@wrench.ai Classifier: Programming
-Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent Requires-Python: >=3.11
-Description-Content-Type: text/markdown License-File: LICENSE
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
@@ -19,25 +19,28 @@
 AWS RDS and S3 services and the `AWSClientHub`. - **Decorators**: Utility
 decorators for retry logic, singleton pattern, and method timing. - **Models**:
 _Internal for interacting with OpenAI models. - **Tools**: Miscellaneous
 utility tools such as coalescing values, file typing, image encoding, and a
 custom logger. - **DataFlow**: Response focused tools to aid in returning
 values and generating logs based on status codes. ## Installation To install
 the package, simply run the following command: ```bash pip install WrenchCL ```
-# User Guides Sure! Here's an updated and more detailed README that provides
-extensive instructions on how to use `AWSClientHub`, `RdsServiceGateway`,
-`S3ServiceGateway`, `ConversationManager`, `OpenAIFactory`, and
-`OpenAIGateway`. It also includes practical examples for the `Maybe` monad and
-other utility tools. ### Connecting to AWS Services To interact with AWS RDS
-and S3 services, follow these steps: 1. **Setup `AWSClientHub`**: ```python
-from WrenchCL.Connections import AwsClientHub # Initialize the AWSClientHub
-using an env file or keyword arguments aws_client_hub = AWSClientHub
-(env_path="path/to/your/env/file") # Alternatively, use keyword arguments or
-existing env variables # aws_client_hub = AWSClientHub
-(aws_profile='your_profile', region_name='your_region',
+Upon recieving the below error: ```bash ImportError: failed to find libmagic.
+Check your installation ``` Install the package with the optional libmagic
+dependency, users can using the following command: ```bash pip install WrenchCL
+[libmagic] ``` # User Guides Sure! Here's an updated and more detailed README
+that provides extensive instructions on how to use `AWSClientHub`,
+`RdsServiceGateway`, `S3ServiceGateway`, `ConversationManager`,
+`OpenAIFactory`, and `OpenAIGateway`. It also includes practical examples for
+the `Maybe` monad and other utility tools. ### Connecting to AWS Services To
+interact with AWS RDS and S3 services, follow these steps: 1. **Setup
+`AWSClientHub`**: ```python from WrenchCL.Connections import AwsClientHub #
+Initialize the AWSClientHub using an env file or keyword arguments
+aws_client_hub = AWSClientHub(env_path="path/to/your/env/file") #
+Alternatively, use keyword arguments or existing env variables # aws_client_hub
+= AWSClientHub(aws_profile='your_profile', region_name='your_region',
 secret_arn='your_secret_arn', ...) ``` 2. **Using `RdsServiceGateway`**:
 ```python from WrenchCL.Connections import RdsServiceGateway # Initialize
 RdsServiceGateway with the AWSClientHub instance rds_service =
 RdsServiceGateway(aws_client_hub) # Example: Fetching data from the database
 query = "SELECT * FROM your_table" data = rds_service.get_data(query) print
 (data) ``` **Methods in `RdsServiceGateway`**: - `get_data(query: str, payload:
 Optional[dict] = None, fetchall: bool = True, accepted_type: Optional[Type] =
```

### Comparing `WrenchCL-2.1.1/WrenchCL.egg-info/SOURCES.txt` & `WrenchCL-2.1.2/WrenchCL.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `WrenchCL-2.1.1/setup.py` & `WrenchCL-2.1.2/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 import os
 import platform
 from setuptools import setup, find_packages
 
+
 # Function to find a folder that ends with .egg-info
 def find_egg_info_folder(path='.'):
     for folder_name in os.listdir(path):
         if folder_name.endswith('.egg-info'):
             return folder_name
     return None
 
+
 # Read the long description from README.md
 with open("README.md", "r", encoding="utf-8") as f:
     long_description = f.read()
 
 # First, attempt to read the dependencies from requirements.txt in the root directory
 required = []
 requirements_path = 'requirements.txt'
@@ -24,36 +26,17 @@
     egg_info_folder = find_egg_info_folder()
     if egg_info_folder:
         requires_path = os.path.join(egg_info_folder, 'requires.txt')
         if os.path.exists(requires_path):
             with open(requires_path, "r", encoding="utf-8") as f:
                 required = f.read().splitlines()
 
-# Add a note for Windows users to install python-magic-bin if python-magic isn't found
-if platform.system() == "Windows":
-    print(
-        "Note: If you encounter issues with python-magic on Windows, please install python-magic-bin manually:\n"
-        "pip install python-magic-bin~=0.4.14"
-    )
-
-setup(
-    name='WrenchCL',
-    version='v2.1.1',
-    author='willem@wrench.ai',
-    description=(
-        'WrenchCL is a comprehensive library designed to facilitate seamless interactions with '
-        'AWS services, OpenAI models, and various utility tools. This package aims to streamline '
-        'the development process by providing robust components for database interactions, '
-        'cloud storage, and AI-powered functionalities.'
-    ),
-    long_description=long_description,
-    long_description_content_type="text/markdown",
-    url='https://github.com/WrenchAI/WrenchCL',
-    packages=find_packages(),
-    install_requires=required,
-    python_requires='>=3.11',
-    classifiers=[
-        'Programming Language :: Python :: 3',
-        'License :: OSI Approved :: MIT License',
-        'Operating System :: OS Independent',
-    ],
-)
+# Define the optional dependencies
+extras = {'libmagic': ['python-magic-bin~=0.4.14']}
+
+setup(name='WrenchCL', version='v2.1.2',
+    description='WrenchCL is a comprehensive library designed to facilitate seamless interactions with AWS services, OpenAI models, and various utility tools. This package aims to streamline the development process by providing robust components for database interactions, cloud storage, and AI-powered functionalities.',
+    long_description=long_description, long_description_content_type="text/markdown",
+    url='https://github.com/WrenchAI/WrenchCL', packages=find_packages(), install_requires=required,
+    extras_require=extras, python_requires='>=3.11',
+    classifiers=['Programming Language :: Python :: 3', 'License :: OSI Approved :: MIT License',
+        'Operating System :: OS Independent', ], )
```

