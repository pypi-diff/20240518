# Comparing `tmp/xplainable_client-1.2.2.post1.tar.gz` & `tmp/xplainable-client-1.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xplainable_client-1.2.2.post1.tar", last modified: Fri May 17 03:17:43 2024, max compression
+gzip compressed data, was "xplainable-client-1.2.4.tar", last modified: Sat May 18 01:38:24 2024, max compression
```

## Comparing `xplainable_client-1.2.2.post1.tar` & `xplainable-client-1.2.4.tar`

### file list

```diff
@@ -1,36 +1,39 @@
-drwxr-xr-x   0 jtuppack   (501) staff       (20)        0 2024-05-17 03:17:43.753728 xplainable_client-1.2.2.post1/
--rw-r--r--   0 jtuppack   (501) staff       (20)     4703 2024-05-17 03:17:43.753497 xplainable_client-1.2.2.post1/PKG-INFO
--rw-r--r--   0 jtuppack   (501) staff       (20)     3924 2024-02-21 21:39:20.000000 xplainable_client-1.2.2.post1/README.md
--rw-r--r--   0 jtuppack   (501) staff       (20)      849 2024-05-17 03:17:17.000000 xplainable_client-1.2.2.post1/pyproject.toml
--rw-r--r--   0 jtuppack   (501) staff       (20)       38 2024-05-17 03:17:43.753773 xplainable_client-1.2.2.post1/setup.cfg
-drwxr-xr-x   0 jtuppack   (501) staff       (20)        0 2024-05-17 03:17:43.746352 xplainable_client-1.2.2.post1/xplainable_client/
-drwxr-xr-x   0 jtuppack   (501) staff       (20)        0 2024-05-17 03:17:43.750822 xplainable_client-1.2.2.post1/xplainable_client/client/
--rw-r--r--   0 jtuppack   (501) staff       (20)     1099 2024-05-17 03:09:19.000000 xplainable_client-1.2.2.post1/xplainable_client/client/__init__.py
--rw-r--r--   0 jtuppack   (501) staff       (20)      123 2024-05-16 09:16:42.000000 xplainable_client-1.2.2.post1/xplainable_client/client/_client_cog_base.py
--rw-r--r--   0 jtuppack   (501) staff       (20)     7352 2024-05-17 03:09:19.000000 xplainable_client-1.2.2.post1/xplainable_client/client/_collections.py
--rw-r--r--   0 jtuppack   (501) staff       (20)     1245 2024-05-16 09:16:42.000000 xplainable_client-1.2.2.post1/xplainable_client/client/_datasets.py
--rw-r--r--   0 jtuppack   (501) staff       (20)    14623 2024-05-17 03:09:19.000000 xplainable_client-1.2.2.post1/xplainable_client/client/_deployments.py
--rw-r--r--   0 jtuppack   (501) staff       (20)     1218 2024-05-17 03:09:19.000000 xplainable_client-1.2.2.post1/xplainable_client/client/_gpt.py
--rw-r--r--   0 jtuppack   (501) staff       (20)     1235 2024-05-17 03:09:19.000000 xplainable_client-1.2.2.post1/xplainable_client/client/_inference.py
--rw-r--r--   0 jtuppack   (501) staff       (20)     8265 2024-05-17 03:09:19.000000 xplainable_client-1.2.2.post1/xplainable_client/client/_misc.py
--rw-r--r--   0 jtuppack   (501) staff       (20)    17225 2024-05-17 03:09:19.000000 xplainable_client-1.2.2.post1/xplainable_client/client/_models.py
--rw-r--r--   0 jtuppack   (501) staff       (20)     9344 2024-05-17 03:09:19.000000 xplainable_client-1.2.2.post1/xplainable_client/client/_preprocessing.py
--rw-r--r--   0 jtuppack   (501) staff       (20)     4051 2024-05-17 03:09:19.000000 xplainable_client-1.2.2.post1/xplainable_client/client/_session.py
-drwxr-xr-x   0 jtuppack   (501) staff       (20)        0 2024-05-17 03:17:43.751002 xplainable_client-1.2.2.post1/xplainable_client/models/
--rw-r--r--   0 jtuppack   (501) staff       (20)     4057 2024-03-04 22:40:48.000000 xplainable_client-1.2.2.post1/xplainable_client/models/ebm.py
-drwxr-xr-x   0 jtuppack   (501) staff       (20)        0 2024-05-17 03:17:43.751469 xplainable_client-1.2.2.post1/xplainable_client/tests/
--rw-r--r--   0 jtuppack   (501) staff       (20)      270 2024-05-17 03:09:19.000000 xplainable_client-1.2.2.post1/xplainable_client/tests/test_model.py
--rw-r--r--   0 jtuppack   (501) staff       (20)      184 2024-05-17 03:09:19.000000 xplainable_client-1.2.2.post1/xplainable_client/tests/test_test.py
-drwxr-xr-x   0 jtuppack   (501) staff       (20)        0 2024-05-17 03:17:43.752795 xplainable_client-1.2.2.post1/xplainable_client/utils/
--rw-r--r--   0 jtuppack   (501) staff       (20)        0 2024-02-12 08:30:29.000000 xplainable_client-1.2.2.post1/xplainable_client/utils/__init__.py
--rw-r--r--   0 jtuppack   (501) staff       (20)     1291 2024-02-11 21:43:09.000000 xplainable_client-1.2.2.post1/xplainable_client/utils/encoders.py
--rw-r--r--   0 jtuppack   (501) staff       (20)      218 2024-05-17 03:09:19.000000 xplainable_client-1.2.2.post1/xplainable_client/utils/exceptions.py
--rw-r--r--   0 jtuppack   (501) staff       (20)      980 2024-02-11 21:45:45.000000 xplainable_client-1.2.2.post1/xplainable_client/utils/helpers.py
--rw-r--r--   0 jtuppack   (501) staff       (20)     6426 2024-02-12 08:36:49.000000 xplainable_client-1.2.2.post1/xplainable_client/utils/metrics.py
--rw-r--r--   0 jtuppack   (501) staff       (20)     3042 2024-02-11 21:51:47.000000 xplainable_client-1.2.2.post1/xplainable_client/utils/model_parsers.py
-drwxr-xr-x   0 jtuppack   (501) staff       (20)        0 2024-05-17 03:17:43.753186 xplainable_client-1.2.2.post1/xplainable_client.egg-info/
--rw-r--r--   0 jtuppack   (501) staff       (20)     4703 2024-05-17 03:17:43.000000 xplainable_client-1.2.2.post1/xplainable_client.egg-info/PKG-INFO
--rw-r--r--   0 jtuppack   (501) staff       (20)      980 2024-05-17 03:17:43.000000 xplainable_client-1.2.2.post1/xplainable_client.egg-info/SOURCES.txt
--rw-r--r--   0 jtuppack   (501) staff       (20)        1 2024-05-17 03:17:43.000000 xplainable_client-1.2.2.post1/xplainable_client.egg-info/dependency_links.txt
--rw-r--r--   0 jtuppack   (501) staff       (20)      130 2024-05-17 03:17:43.000000 xplainable_client-1.2.2.post1/xplainable_client.egg-info/requires.txt
--rw-r--r--   0 jtuppack   (501) staff       (20)       29 2024-05-17 03:17:43.000000 xplainable_client-1.2.2.post1/xplainable_client.egg-info/top_level.txt
+drwxr-xr-x   0 jtuppack   (501) staff       (20)        0 2024-05-18 01:38:24.200857 xplainable-client-1.2.4/
+-rw-r--r--   0 jtuppack   (501) staff       (20)    34523 2024-05-18 01:38:20.000000 xplainable-client-1.2.4/LICENSE
+-rw-r--r--   0 jtuppack   (501) staff       (20)    44573 2024-05-18 01:38:24.200489 xplainable-client-1.2.4/PKG-INFO
+-rw-r--r--   0 jtuppack   (501) staff       (20)     3924 2024-02-21 21:39:20.000000 xplainable-client-1.2.4/README.md
+-rw-r--r--   0 jtuppack   (501) staff       (20)      852 2024-05-17 23:15:50.000000 xplainable-client-1.2.4/pyproject.toml
+-rw-r--r--   0 jtuppack   (501) staff       (20)       38 2024-05-18 01:38:24.200912 xplainable-client-1.2.4/setup.cfg
+-rw-r--r--   0 jtuppack   (501) staff       (20)      822 2024-05-18 01:38:20.000000 xplainable-client-1.2.4/setup.py
+drwxr-xr-x   0 jtuppack   (501) staff       (20)        0 2024-05-18 01:38:24.195128 xplainable-client-1.2.4/tests/
+-rw-r--r--   0 jtuppack   (501) staff       (20)      270 2024-05-18 01:38:20.000000 xplainable-client-1.2.4/tests/test_model.py
+-rw-r--r--   0 jtuppack   (501) staff       (20)      184 2024-05-18 01:38:20.000000 xplainable-client-1.2.4/tests/test_test.py
+drwxr-xr-x   0 jtuppack   (501) staff       (20)        0 2024-05-18 01:38:24.195239 xplainable-client-1.2.4/xplainable_client/
+-rw-r--r--   0 jtuppack   (501) staff       (20)       27 2024-05-17 23:15:50.000000 xplainable-client-1.2.4/xplainable_client/__init__.py
+drwxr-xr-x   0 jtuppack   (501) staff       (20)        0 2024-05-18 01:38:24.199033 xplainable-client-1.2.4/xplainable_client/client/
+-rw-r--r--   0 jtuppack   (501) staff       (20)      946 2024-05-17 23:15:50.000000 xplainable-client-1.2.4/xplainable_client/client/__init__.py
+-rw-r--r--   0 jtuppack   (501) staff       (20)      123 2024-05-16 09:16:42.000000 xplainable-client-1.2.4/xplainable_client/client/_client_cog_base.py
+-rw-r--r--   0 jtuppack   (501) staff       (20)     7324 2024-05-17 23:15:50.000000 xplainable-client-1.2.4/xplainable_client/client/_collections.py
+-rw-r--r--   0 jtuppack   (501) staff       (20)     1245 2024-05-16 09:16:42.000000 xplainable-client-1.2.4/xplainable_client/client/_datasets.py
+-rw-r--r--   0 jtuppack   (501) staff       (20)    14605 2024-05-17 23:15:50.000000 xplainable-client-1.2.4/xplainable_client/client/_deployments.py
+-rw-r--r--   0 jtuppack   (501) staff       (20)     1218 2024-05-17 03:09:19.000000 xplainable-client-1.2.4/xplainable_client/client/_gpt.py
+-rw-r--r--   0 jtuppack   (501) staff       (20)     1236 2024-05-17 23:15:50.000000 xplainable-client-1.2.4/xplainable_client/client/_inference.py
+-rw-r--r--   0 jtuppack   (501) staff       (20)     7982 2024-05-17 23:15:50.000000 xplainable-client-1.2.4/xplainable_client/client/_misc.py
+-rw-r--r--   0 jtuppack   (501) staff       (20)    20834 2024-05-17 23:17:59.000000 xplainable-client-1.2.4/xplainable_client/client/_models.py
+-rw-r--r--   0 jtuppack   (501) staff       (20)     9359 2024-05-17 23:15:50.000000 xplainable-client-1.2.4/xplainable_client/client/_preprocessing.py
+-rw-r--r--   0 jtuppack   (501) staff       (20)     4020 2024-05-17 23:15:50.000000 xplainable-client-1.2.4/xplainable_client/client/_session.py
+drwxr-xr-x   0 jtuppack   (501) staff       (20)        0 2024-05-18 01:38:24.199734 xplainable-client-1.2.4/xplainable_client/client/utils/
+-rw-r--r--   0 jtuppack   (501) staff       (20)      122 2024-05-17 23:15:50.000000 xplainable-client-1.2.4/xplainable_client/client/utils/__init__.py
+-rw-r--r--   0 jtuppack   (501) staff       (20)     1291 2024-05-17 23:15:50.000000 xplainable-client-1.2.4/xplainable_client/client/utils/encoders.py
+-rw-r--r--   0 jtuppack   (501) staff       (20)      961 2024-05-17 23:15:50.000000 xplainable-client-1.2.4/xplainable_client/client/utils/helpers.py
+-rw-r--r--   0 jtuppack   (501) staff       (20)     6416 2024-05-17 23:15:50.000000 xplainable-client-1.2.4/xplainable_client/client/utils/metrics.py
+-rw-r--r--   0 jtuppack   (501) staff       (20)     3042 2024-05-17 23:15:50.000000 xplainable-client-1.2.4/xplainable_client/client/utils/model_parsers.py
+-rw-r--r--   0 jtuppack   (501) staff       (20)    10432 2024-05-17 23:15:50.000000 xplainable-client-1.2.4/xplainable_client/client/utils/scanner.py
+drwxr-xr-x   0 jtuppack   (501) staff       (20)        0 2024-05-18 01:38:24.199850 xplainable-client-1.2.4/xplainable_client/models/
+-rw-r--r--   0 jtuppack   (501) staff       (20)     4057 2024-03-04 22:40:48.000000 xplainable-client-1.2.4/xplainable_client/models/ebm.py
+drwxr-xr-x   0 jtuppack   (501) staff       (20)        0 2024-05-18 01:38:24.197328 xplainable-client-1.2.4/xplainable_client.egg-info/
+-rw-r--r--   0 jtuppack   (501) staff       (20)    44573 2024-05-18 01:38:24.000000 xplainable-client-1.2.4/xplainable_client.egg-info/PKG-INFO
+-rw-r--r--   0 jtuppack   (501) staff       (20)     1030 2024-05-18 01:38:24.000000 xplainable-client-1.2.4/xplainable_client.egg-info/SOURCES.txt
+-rw-r--r--   0 jtuppack   (501) staff       (20)        1 2024-05-18 01:38:24.000000 xplainable-client-1.2.4/xplainable_client.egg-info/dependency_links.txt
+-rw-r--r--   0 jtuppack   (501) staff       (20)      135 2024-05-18 01:38:24.000000 xplainable-client-1.2.4/xplainable_client.egg-info/requires.txt
+-rw-r--r--   0 jtuppack   (501) staff       (20)       24 2024-05-18 01:38:24.000000 xplainable-client-1.2.4/xplainable_client.egg-info/top_level.txt
```

### Comparing `xplainable_client-1.2.2.post1/PKG-INFO` & `xplainable-client-1.2.4/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,29 +1,7 @@
-Metadata-Version: 2.1
-Name: xplainable-client
-Version: 1.2.2.post1
-Summary: The client for persisting and deploying models to Xplainable cloud.
-Author-email: xplainable pty ltd <contact@xplainable.io>
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-Requires-Dist: ipywidgets==8.0.6
-Requires-Dist: numpy==1.21.1
-Requires-Dist: pandas>=1.5.2
-Requires-Dist: pyperclip==1.8.2
-Requires-Dist: Requests==2.31.0
-Requires-Dist: scikit_learn
-Requires-Dist: setuptools
-Requires-Dist: urllib3==2.2.0
-Requires-Dist: xplainable
-
 
 <div align="center">
 <img src="https://raw.githubusercontent.com/xplainable/xplainable/main/docs/assets/logo/xplainable-logo.png">
 <h1 align="center">xplainable</h1>
 <h3 align="center">Real-time explainable machine learning for business optimisation</h3>
     
 **Xplainable** makes tabular machine learning transparent, fair, and actionable.
```

### Comparing `xplainable_client-1.2.2.post1/pyproject.toml` & `xplainable-client-1.2.4/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "setuptools.build_meta"
 
 [tool.setuptools.packages]
 find = {} 
 
 [project]
 name = "xplainable-client"
-version = "1.2.2-1"
+version = "1.2.4"
 authors = [
   { name="xplainable pty ltd", email="contact@xplainable.io" },
 ]
 description = "The client for persisting and deploying models to Xplainable cloud."
 readme = "README.md"
 license = { file="LICENSE" }
 requires-python = ">=3.8"
@@ -22,16 +22,16 @@
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Operating System :: OS Independent"
 ]
 
 dependencies = [
 "ipywidgets==8.0.6",
-"numpy==1.21.1",
+"numpy>=1.26",
 "pandas>=1.5.2",
 "pyperclip==1.8.2",
 "Requests==2.31.0",
 "scikit_learn",
 "setuptools",
 "urllib3==2.2.0",
-"xplainable"
+"xplainable==1.2.4"
 ]
```

### Comparing `xplainable_client-1.2.2.post1/xplainable_client/client/__init__.py` & `xplainable-client-1.2.4/xplainable_client/client/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,33 +1,29 @@
-from ._datasets import *
-from functools import cached_property
-
 from ._models import *
 from ._misc import *
-from urllib3.util.retry import Retry
 from ._session import Session
 from ._misc import Misc
 from ._models import Models
 from ._preprocessing import Preprocessing
 from ._deployments import Deployments
 from ._gpt import GPT
 from ._collections import Collections
 from ._datasets import Datasets
 from ._inference import Inference
 
 
 class Client(Misc, Models, Preprocessing, GPT, Collections, Datasets, Inference, Deployments):
 
-    def __init__(self, api_key=None, hostname='https://api.xplainable.io', silent_mode=False):
-        self.session = Session(api_key=api_key, hostname=hostname, silent_mode=silent_mode)
+    def __init__(self, api_key=None, hostname='https://api.xplainable.io'):
+        self.session = Session(api_key=api_key, hostname=hostname)
         Misc.__init__(self, self.session)
         Models.__init__(self, self.session)
         Preprocessing.__init__(self, self.session)
         Deployments.__init__(self, self.session)
         GPT.__init__(self, self.session)
         Collections.__init__(self, self.session)
         Datasets.__init__(self, self.session)
         Inference.__init__(self, self.session)
-        
+
```

### Comparing `xplainable_client-1.2.2.post1/xplainable_client/client/_collections.py` & `xplainable-client-1.2.4/xplainable_client/client/_collections.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 from ._client_cog_base import *
-from ._models import Models
 
 
 class Collections(Client_Cog):
 
     def create_collection(self, model_id: str, name: str, description: str):
         """ Creates a new collection.
         Args:
```

### Comparing `xplainable_client-1.2.2.post1/xplainable_client/client/_datasets.py` & `xplainable-client-1.2.4/xplainable_client/client/_datasets.py`

 * *Files identical despite different names*

### Comparing `xplainable_client-1.2.2.post1/xplainable_client/client/_deployments.py` & `xplainable-client-1.2.4/xplainable_client/client/_deployments.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,11 @@
-import pyperclip
 import inspect
-
-
 from ._client_cog_base import *
 
+
 class Deployments(Client_Cog):
 
 
     def deploy(
             self, model_id: str, version_id: str,
             hostname: str='https://inference.xplainable.io',
             location: str='syd', raw_output: bool=True) -> dict:
```

### Comparing `xplainable_client-1.2.2.post1/xplainable_client/client/_gpt.py` & `xplainable-client-1.2.4/xplainable_client/client/_gpt.py`

 * *Files identical despite different names*

### Comparing `xplainable_client-1.2.2.post1/xplainable_client/client/_inference.py` & `xplainable-client-1.2.4/xplainable_client/client/_inference.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from ._client_cog_base import *
 
+
 class Inference(Client_Cog):
     
     def predict(self, filename: str, model_id: str, version_id: str, threshold: float = 0.5, delimiter: str = ","):
         """ Predicts the target column of a dataset.
         Args:
             filename (str): The name of the file.
             model_id (str): The model id.
```

### Comparing `xplainable_client-1.2.2.post1/xplainable_client/client/_misc.py` & `xplainable-client-1.2.4/xplainable_client/client/_misc.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,30 +1,18 @@
 """ Copyright Xplainable Pty Ltd"""
-import json
 import pandas as pd
 import inspect
 import ast
-import sys
 import xplainable
-
-import requests
-from urllib3.exceptions import HTTPError
-
-from requests.adapters import HTTPAdapter
-
-from xplainable.preprocessing.pipeline import XPipeline
-from xplainable.preprocessing import transformers as xtf
 from xplainable.utils.model_parsers import *
 from xplainable.quality.scanner import XScan
 
-from ..utils.exceptions import AuthenticationError
-from ..utils.encoders import NpEncoder, force_json_compliant
-from ..utils.metrics import evaluate_classification, evaluate_regression
+from xplainable_client.client.utils.encoders import NpEncoder
+from xplainable_client.client.utils.metrics import evaluate_classification, evaluate_regression
 
-import ipywidgets
 from ._client_cog_base import *
 
 
 class Misc(Client_Cog):
 
     @staticmethod
     def _get_xplainable_version():
```

### Comparing `xplainable_client-1.2.2.post1/xplainable_client/client/_preprocessing.py` & `xplainable-client-1.2.4/xplainable_client/client/_preprocessing.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from ._client_cog_base import *
 import pandas as pd
 import json
-from ..utils.helpers import get_df_delta
+from xplainable_client.client.utils import get_df_delta
 from xplainable.preprocessing.pipeline import XPipeline
 
 
 class Preprocessing(Client_Cog):
 
     def create_preprocessor_id(
         self, preprocessor_name: str, preprocessor_description: str) -> str:
```

### Comparing `xplainable_client-1.2.2.post1/xplainable_client/client/_session.py` & `xplainable-client-1.2.4/xplainable_client/client/_session.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-from ._datasets import *
-from ..utils.exceptions import *
 from functools import cached_property
 import xplainable
 import json
 from requests.adapters import HTTPAdapter
 import ipywidgets
 import sys
 from IPython.display import display
@@ -18,30 +16,31 @@
     Access models, preprocessors and user data from xplainable cloud. API keys
     can be generated at https://beta.xplainable.io.
 
     Args:
         api_key (str): A valid api key.
     """
 
-    def __init__(self, api_key=None, hostname='https://api.xplainable.io', silent_mode=False):
+    def __init__(self, api_key=None, hostname='https://api.xplainable.io'):
         if not api_key:
             raise ValueError('A valid API Key is required. Generate one from the xplainable app.')
 
         self.api_key = api_key
         self.hostname = hostname
         self._setup_session()  # Set up the session and other initialization steps
 
 
         self._ext = f"organisations/{self.user_data['organisation_id']}/teams/{self.user_data['team_id']}"
 
         # You can still use the _render_init_table here if you want to display it,
         # or you can return the data dict for a more script-friendly approach.
         data = self._gather_initialization_data()
-        if not silent_mode:
-            self._render_init_table(data)
+        # if not silent_mode:
+        #
+        #     self._render_init_table(data)
 
     @cached_property
     def user_data(self):
         """ Retrieves the user data for the active user.
         Returns:
             dict: User data
         """
@@ -49,39 +48,40 @@
             url=f'{self.hostname}/v1/client-connect',
             
         )
         if response.status_code == 200:
             return self.get_response_content(response)
 
         else:
-            raise AuthenticationError(
-                f"{response.status_code} Unauthenticated. "
-                f"{response.json()['detail']}"
+            raise Exception(
+                f"{response.status_code} Unauthenticated. {response.json()['detail']}"
             )
 
     def _setup_session(self):
         """ Set up the session with retry strategy and session headers. """
         self._session = requests.Session()
         self._session.headers['api_key'] = self.api_key
         retry_strategy = Retry(total=5, backoff_factor=1)
         adapter = HTTPAdapter(max_retries=retry_strategy)
         self._session.mount(self.hostname, adapter)
 
     def get_response_content(self, response):
+        print("get_response_content")
+        print(response)
         if response.status_code == 200:
             return json.loads(response.content)
         elif response.status_code == 401:
             err_string = "401 Unauthorised"
             content = json.loads(response.content)
             if 'detail' in content:
                 err_string = err_string + f" ({content['detail']})"
 
-            raise HTTPError(err_string)
+            raise Exception(err_string)
         else:
-            raise HTTPError(response.status_code, json.loads(response.content))
+            raise Exception(response.status_code, json.loads(response.content))
 
     def _gather_initialization_data(self):
         """ Gather data to display or return upon initialization. """
         version_info = sys.version_info
         self.python_version = f'{version_info.major}.{version_info.minor}.{version_info.micro}'
         self.xplainable_version = xplainable.__version__
```

### Comparing `xplainable_client-1.2.2.post1/xplainable_client/models/ebm.py` & `xplainable-client-1.2.4/xplainable_client/models/ebm.py`

 * *Files identical despite different names*

### Comparing `xplainable_client-1.2.2.post1/xplainable_client/utils/encoders.py` & `xplainable-client-1.2.4/xplainable_client/client/utils/encoders.py`

 * *Files identical despite different names*

### Comparing `xplainable_client-1.2.2.post1/xplainable_client/utils/helpers.py` & `xplainable-client-1.2.4/xplainable_client/client/utils/helpers.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import json
-import pandas as pd
 from .encoders import NpEncoder
 
+
 def get_df_delta(df1, df2):
     """ Gets the delta between two dataframs"""
     changed_features = [c for c in df1.columns.intersection(
         df2.columns) if not df1[c].head(10).equals(df2[c].head(10))]
 
     rows_changed = {}
     for c in changed_features:
```

### Comparing `xplainable_client-1.2.2.post1/xplainable_client/utils/metrics.py` & `xplainable-client-1.2.4/xplainable_client/client/utils/metrics.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 """ Copyright Xplainable Pty Ltd, 2023"""
 
 import numpy as np
-import pandas as pd
-from xplainable_client.utils.encoders import force_json_compliant
+from xplainable_client.client.utils.encoders import force_json_compliant
 from sklearn.metrics import (
     roc_auc_score, matthews_corrcoef, log_loss, auc, mean_absolute_error,
     mean_squared_error, r2_score, explained_variance_score,
     mean_squared_log_error, mean_absolute_percentage_error)
 
 
 def calculate_classification_metrics(tp, fp, tn, fn):
@@ -36,14 +35,15 @@
         output_data.append({
             "class": cls,
             "values": list(counts)
         })
     
     return output_data
 
+
 def calculate_regression_bins(y_true, y_pred, bin_count):
 
     # Ensure y_true and y_pred are NumPy arrays
     y_true = np.array(y_true)
     y_pred = np.array(y_pred)
 
     # Calculate the min and max of the predicted values
@@ -78,14 +78,15 @@
             "class": "pred",
             "values": pred_output
         }
     ]
     
     return output
 
+
 def evaluate_classification(y_true, y_pred):
     results = {}
     thresholds = np.linspace(0, 1, 101)
     
     # TP, FP, TN, FN at each threshold value
     metrics = []
     for threshold in thresholds:
@@ -147,14 +148,15 @@
         results["log_loss"] = np.nan
 
     # Calculates the number of predictions in each probability bin
     results["probability_bins"] = calculate_probability_bins(y_true, y_pred)
 
     return force_json_compliant(results)
 
+
 def evaluate_regression(y_true, y_pred):
     results = {
         "charts": {
             'true': list(y_true.values if len(y_true) < 10000 else y_true[:10000].values),
             'prediction': list(y_pred if len(y_pred) < 10000 else y_pred[:10000]),
         }
     }
```

### Comparing `xplainable_client-1.2.2.post1/xplainable_client/utils/model_parsers.py` & `xplainable-client-1.2.4/xplainable_client/client/utils/model_parsers.py`

 * *Files identical despite different names*

### Comparing `xplainable_client-1.2.2.post1/xplainable_client.egg-info/SOURCES.txt` & `xplainable-client-1.2.4/xplainable_client.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,14 @@
+LICENSE
 README.md
 pyproject.toml
+setup.py
+tests/test_model.py
+tests/test_test.py
+xplainable_client/__init__.py
 xplainable_client.egg-info/PKG-INFO
 xplainable_client.egg-info/SOURCES.txt
 xplainable_client.egg-info/dependency_links.txt
 xplainable_client.egg-info/requires.txt
 xplainable_client.egg-info/top_level.txt
 xplainable_client/client/__init__.py
 xplainable_client/client/_client_cog_base.py
@@ -12,16 +17,14 @@
 xplainable_client/client/_deployments.py
 xplainable_client/client/_gpt.py
 xplainable_client/client/_inference.py
 xplainable_client/client/_misc.py
 xplainable_client/client/_models.py
 xplainable_client/client/_preprocessing.py
 xplainable_client/client/_session.py
-xplainable_client/models/ebm.py
-xplainable_client/tests/test_model.py
-xplainable_client/tests/test_test.py
-xplainable_client/utils/__init__.py
-xplainable_client/utils/encoders.py
-xplainable_client/utils/exceptions.py
-xplainable_client/utils/helpers.py
-xplainable_client/utils/metrics.py
-xplainable_client/utils/model_parsers.py
+xplainable_client/client/utils/__init__.py
+xplainable_client/client/utils/encoders.py
+xplainable_client/client/utils/helpers.py
+xplainable_client/client/utils/metrics.py
+xplainable_client/client/utils/model_parsers.py
+xplainable_client/client/utils/scanner.py
+xplainable_client/models/ebm.py
```

