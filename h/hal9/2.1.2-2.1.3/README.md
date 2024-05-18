# Comparing `tmp/hal9-2.1.2.tar.gz` & `tmp/hal9-2.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hal9-2.1.2.tar", max compression
+gzip compressed data, was "hal9-2.1.3.tar", max compression
```

## Comparing `hal9-2.1.2.tar` & `hal9-2.1.3.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     2951 2024-05-17 21:37:53.967241 hal9-2.1.2/README.md
--rw-r--r--   0        0        0       86 2024-05-17 21:37:53.895241 hal9-2.1.2/hal9/__init__.py
--rw-r--r--   0        0        0     1220 2024-05-17 21:37:53.895241 hal9-2.1.2/hal9/cli.py
--rw-r--r--   0        0        0      634 2024-05-17 21:37:53.895241 hal9-2.1.2/hal9/create.py
--rw-r--r--   0        0        0      574 2024-05-17 21:37:53.895241 hal9-2.1.2/hal9/deploy.py
--rw-r--r--   0        0        0      531 2024-05-17 21:37:53.895241 hal9-2.1.2/hal9/run.py
--rw-r--r--   0        0        0      352 2024-05-17 21:37:53.895241 hal9-2.1.2/hal9/targets/docker.py
--rw-r--r--   0        0        0     2021 2024-05-17 21:37:53.899241 hal9-2.1.2/hal9/targets/hal9.py
--rw-r--r--   0        0        0       42 2024-05-17 21:37:53.899241 hal9-2.1.2/hal9/templates/docker/Dockerfile
--rw-r--r--   0        0        0       38 2024-05-17 21:37:53.899241 hal9-2.1.2/hal9/templates/openai/app.py
--rw-r--r--   0        0        0      434 2024-05-17 21:37:53.899241 hal9-2.1.2/pyproject.toml
--rw-r--r--   0        0        0     3589 1970-01-01 00:00:00.000000 hal9-2.1.2/PKG-INFO
+-rw-r--r--   0        0        0     2948 2024-05-17 21:55:15.073818 hal9-2.1.3/README.md
+-rw-r--r--   0        0        0       86 2024-05-17 21:55:14.997817 hal9-2.1.3/hal9/__init__.py
+-rw-r--r--   0        0        0     1220 2024-05-17 21:55:14.997817 hal9-2.1.3/hal9/cli.py
+-rw-r--r--   0        0        0      634 2024-05-17 21:55:15.001817 hal9-2.1.3/hal9/create.py
+-rw-r--r--   0        0        0      574 2024-05-17 21:55:15.001817 hal9-2.1.3/hal9/deploy.py
+-rw-r--r--   0        0        0      531 2024-05-17 21:55:15.001817 hal9-2.1.3/hal9/run.py
+-rw-r--r--   0        0        0      352 2024-05-17 21:55:15.001817 hal9-2.1.3/hal9/targets/docker.py
+-rw-r--r--   0        0        0     2021 2024-05-17 21:55:15.001817 hal9-2.1.3/hal9/targets/hal9.py
+-rw-r--r--   0        0        0       42 2024-05-17 21:55:15.001817 hal9-2.1.3/hal9/templates/docker/Dockerfile
+-rw-r--r--   0        0        0       38 2024-05-17 21:55:15.001817 hal9-2.1.3/hal9/templates/openai/app.py
+-rw-r--r--   0        0        0      434 2024-05-17 21:55:15.001817 hal9-2.1.3/pyproject.toml
+-rw-r--r--   0        0        0     3586 1970-01-01 00:00:00.000000 hal9-2.1.3/PKG-INFO
```

### Comparing `hal9-2.1.2/README.md` & `hal9-2.1.3/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 - **Scalable:** Engineers can integrate your app with scalable technilogies (Docker, Kubernetes, etc)
 - **Powerful:** Using an OS process (stdin, stdout, files) as our app contract, enables long-running agents, multiple programming languages, and complex system dependencies.
 
 Focus on AI (RAG, fine-tuning, aligment, training) and skip engineering tasks (frontend development, backend integration, deployment, operations).
 
 ## Getting started
 
-To create and share a chatbot in seconds by running the following commands:
+Create and share a chatbot in seconds by running the following commands:
 
 ```bash
 pip install hal9
 
 hal9 create chatbot
 hal9 deploy chatbot
 ```
```

### Comparing `hal9-2.1.2/hal9/cli.py` & `hal9-2.1.3/hal9/cli.py`

 * *Files identical despite different names*

### Comparing `hal9-2.1.2/hal9/create.py` & `hal9-2.1.3/hal9/create.py`

 * *Files identical despite different names*

### Comparing `hal9-2.1.2/hal9/deploy.py` & `hal9-2.1.3/hal9/deploy.py`

 * *Files identical despite different names*

### Comparing `hal9-2.1.2/hal9/run.py` & `hal9-2.1.3/hal9/run.py`

 * *Files identical despite different names*

### Comparing `hal9-2.1.2/hal9/targets/hal9.py` & `hal9-2.1.3/hal9/targets/hal9.py`

 * *Files identical despite different names*

### Comparing `hal9-2.1.2/PKG-INFO` & `hal9-2.1.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hal9
-Version: 2.1.2
+Version: 2.1.3
 Summary: 
 Author: Javier Luraschi
 Author-email: javier@hal9.ai
 Requires-Python: >=3.8, !=2.7.*, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*, !=3.4.*, !=3.5.*, !=3.6.*, !=3.7.*
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -25,15 +25,15 @@
 - **Scalable:** Engineers can integrate your app with scalable technilogies (Docker, Kubernetes, etc)
 - **Powerful:** Using an OS process (stdin, stdout, files) as our app contract, enables long-running agents, multiple programming languages, and complex system dependencies.
 
 Focus on AI (RAG, fine-tuning, aligment, training) and skip engineering tasks (frontend development, backend integration, deployment, operations).
 
 ## Getting started
 
-To create and share a chatbot in seconds by running the following commands:
+Create and share a chatbot in seconds by running the following commands:
 
 ```bash
 pip install hal9
 
 hal9 create chatbot
 hal9 deploy chatbot
 ```
```

