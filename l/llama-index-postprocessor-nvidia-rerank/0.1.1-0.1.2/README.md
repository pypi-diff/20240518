# Comparing `tmp/llama_index_postprocessor_nvidia_rerank-0.1.1.tar.gz` & `tmp/llama_index_postprocessor_nvidia_rerank-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llama_index_postprocessor_nvidia_rerank-0.1.1.tar", max compression
+gzip compressed data, was "llama_index_postprocessor_nvidia_rerank-0.1.2.tar", max compression
```

## Comparing `llama_index_postprocessor_nvidia_rerank-0.1.1.tar` & `llama_index_postprocessor_nvidia_rerank-0.1.2.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     3559 2024-05-13 21:57:40.367680 llama_index_postprocessor_nvidia_rerank-0.1.1/README.md
--rw-r--r--   0        0        0       17 2024-05-13 21:57:40.367680 llama_index_postprocessor_nvidia_rerank-0.1.1/llama_index/postprocessor/nvidia_rerank/BUILD
--rw-r--r--   0        0        0       99 2024-05-13 21:57:40.367680 llama_index_postprocessor_nvidia_rerank-0.1.1/llama_index/postprocessor/nvidia_rerank/__init__.py
--rw-r--r--   0        0        0     8583 2024-05-13 21:57:40.367680 llama_index_postprocessor_nvidia_rerank-0.1.1/llama_index/postprocessor/nvidia_rerank/base.py
--rw-r--r--   0        0        0     1710 2024-05-13 21:57:40.367680 llama_index_postprocessor_nvidia_rerank-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     4139 1970-01-01 00:00:00.000000 llama_index_postprocessor_nvidia_rerank-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     3559 2024-05-18 16:06:55.051766 llama_index_postprocessor_nvidia_rerank-0.1.2/README.md
+-rw-r--r--   0        0        0       17 2024-05-18 16:06:55.051766 llama_index_postprocessor_nvidia_rerank-0.1.2/llama_index/postprocessor/nvidia_rerank/BUILD
+-rw-r--r--   0        0        0       99 2024-05-18 16:06:55.051766 llama_index_postprocessor_nvidia_rerank-0.1.2/llama_index/postprocessor/nvidia_rerank/__init__.py
+-rw-r--r--   0        0        0     9623 2024-05-18 16:06:55.051766 llama_index_postprocessor_nvidia_rerank-0.1.2/llama_index/postprocessor/nvidia_rerank/base.py
+-rw-r--r--   0        0        0     1710 2024-05-18 16:06:55.051766 llama_index_postprocessor_nvidia_rerank-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     4139 1970-01-01 00:00:00.000000 llama_index_postprocessor_nvidia_rerank-0.1.2/PKG-INFO
```

### Comparing `llama_index_postprocessor_nvidia_rerank-0.1.1/README.md` & `llama_index_postprocessor_nvidia_rerank-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `llama_index_postprocessor_nvidia_rerank-0.1.1/llama_index/postprocessor/nvidia_rerank/base.py` & `llama_index_postprocessor_nvidia_rerank-0.1.2/llama_index/postprocessor/nvidia_rerank/base.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,20 +7,27 @@
 from llama_index.core.instrumentation.events.rerank import (
     ReRankEndEvent,
     ReRankStartEvent,
 )
 from llama_index.core.postprocessor.types import BaseNodePostprocessor
 from llama_index.core.schema import MetadataMode, NodeWithScore, QueryBundle
 import requests
-
+import warnings
+from deprecated import deprecated
 from llama_index.core.base.llms.generic_utils import get_from_param_or_env
 
 
 DEFAULT_MODEL = "nv-rerank-qa-mistral-4b:1"
-DEFAULT_BASE_URL = "https://ai.api.nvidia.com/v1"
+BASE_URL = "https://ai.api.nvidia.com/v1"
+
+MODEL_ENDPOINT_MAP = {
+    DEFAULT_MODEL: BASE_URL,
+}
+
+KNOWN_URLS = list(MODEL_ENDPOINT_MAP.values())
 
 dispatcher = get_dispatcher(__name__)
 
 
 class Model(BaseModel):
     id: str
 
@@ -41,75 +48,102 @@
         description="The number of nodes to return.",
     )
     max_batch_size: Optional[int] = Field(
         default=64,
         ge=1,
         description="The maximum batch size supported by the inference server.",
     )
-    _api_key: str = PrivateAttr("API_KEY_NOT_PROVIDED")  # TODO: should be SecretStr
+    _api_key: str = PrivateAttr("NO_API_KEY_PROVIDED")  # TODO: should be SecretStr
     _mode: str = PrivateAttr("nvidia")
-    _base_url: str = PrivateAttr(DEFAULT_BASE_URL)
+    _is_hosted: bool = PrivateAttr(True)
+    _base_url: str = PrivateAttr(BASE_URL)
 
     def _set_api_key(self, nvidia_api_key: str = None, api_key: str = None) -> None:
         self._api_key = get_from_param_or_env(
             "api_key",
             nvidia_api_key or api_key,
             "NVIDIA_API_KEY",
-            "API_KEY_NOT_PROVIDED",
+            "NO_API_KEY_PROVIDED",
         )
 
     def __init__(
         self,
+        model: str = DEFAULT_MODEL,
         nvidia_api_key: Optional[str] = None,
         api_key: Optional[str] = None,
+        base_url: Optional[str] = None,
         **kwargs: Any,
     ):
-        super().__init__(**kwargs)
+        """
+        Initialize a NVIDIARerank instance.
+
+        This class provides access to a NVIDIA NIM for reranking. By default, it connects to a hosted NIM, but can be configured to connect to an on-premises NIM using the `base_url` parameter. An API key is required for hosted NIM.
 
-        self._set_api_key(nvidia_api_key, api_key)
+        Args:
+            model (str): The model to use for reranking.
+            nvidia_api_key (str, optional): The NVIDIA API key. Defaults to None.
+            api_key (str, optional): The API key. Defaults to None.
+            base_url (str, optional): The base URL of the on-premises NIM. Defaults to None.
+            **kwargs: Additional keyword arguments.
+
+        API Key:
+        - The recommended way to provide the API key is through the `NVIDIA_API_KEY` environment variable.
+        """
+        super().__init__(model=model, **kwargs)
+
+        self._base_url = base_url or MODEL_ENDPOINT_MAP.get(model, BASE_URL)
+
+        self._api_key = get_from_param_or_env(
+            "api_key",
+            nvidia_api_key or api_key,
+            "NVIDIA_API_KEY",
+            "NO_API_KEY_PROVIDED",
+        )
+
+        self._is_hosted = self._base_url in KNOWN_URLS
+
+        if self._is_hosted and self._api_key == "NO_API_KEY_PROVIDED":
+            warnings.warn(
+                "An API key is required for hosted NIM. This will become an error in 0.2.0."
+            )
 
     @property
     def available_models(self) -> List[Model]:
         """Get available models."""
-        # there is one model on ai.nvidia.com and available as a local NIM
-        ids = [DEFAULT_MODEL]
+        # all available models are in the map
+        ids = MODEL_ENDPOINT_MAP.keys()
         return [Model(id=id) for id in ids]
 
+    @deprecated(
+        version="0.1.2",
+        reason="Will be removed in 0.2. Construct with `base_url` instead.",
+    )
     def mode(
         self,
         mode: Literal["nvidia", "nim"] = "nvidia",
         *,
         base_url: Optional[str] = None,
         model: Optional[str] = None,
         api_key: Optional[str] = None,
     ) -> "NVIDIARerank":
         """
-        Change the mode.
-
-        There are two modes, "nvidia" and "nim". The "nvidia" mode is the default mode
-        and is used to interact with hosted NVIDIA NIMs. The "nim" mode is
-        used to interact with local NVIDIA NIM endpoints, which are typically hosted
-        on-premises.
-
-        For the "nvidia" mode, the "api_key" parameter is available to specify your
-        API key. If not specified, the NVIDIA_API_KEY environment variable will be used.
-
-        For the "nim" mode, the "base_url" is required and "model" is recommended. Set
-        base_url to the url of your NVIDIA NIM endpoint. For instance,
-        "https://localhost:1976/v1", it should end in "/v1". Additionally, the "model"
-        parameter must be set to the name of the model inside the NIM.
+        Deprecated: use NVIDIARerank(base_url=...) instead.
         """
         if isinstance(self, str):
             raise ValueError("Please construct the model before calling mode()")
 
-        if mode == "nim":
+        self._is_hosted = mode == "nvidia"
+
+        if not self._is_hosted:
             if not base_url:
                 raise ValueError("base_url is required for nim mode")
+        else:
+            api_key = get_from_param_or_env("api_key", api_key, "NVIDIA_API_KEY")
         if not base_url:
-            base_url = DEFAULT_BASE_URL
+            base_url = BASE_URL
 
         self._mode = mode
         if base_url:
             # TODO: change this to not require /v1 at the end. the current
             #       implementation is for consistency, but really this code
             #       should dictate which version it works with
             components = urlparse(base_url)
@@ -124,15 +158,15 @@
                 raise ValueError(
                     f"Incorrect url format, use https://host:post/v1 ending with /v1, given '{base_url}'"
                 )
             self._base_url = base_url
         if model:
             self.model = model
         if api_key:
-            self._set_api_key(api_key)
+            self._api_key = api_key
 
         return self
 
     @classmethod
     def class_name(cls) -> str:
         return "NVIDIARerank"
 
@@ -187,15 +221,15 @@
                     "passages": [
                         {"text": n.get_content(metadata_mode=MetadataMode.EMBED)}
                         for n in batch
                     ],
                 }
                 # the hosted NIM path is different from the local NIM path
                 url = self._base_url
-                if self._mode == "nvidia":
+                if self._is_hosted:
                     url += "/retrieval/nvidia/reranking"
                 else:
                     url += "/ranking"
                 response = session.post(url, headers=_headers, json=payloads)
                 response.raise_for_status()
                 # expected response format:
                 # {
```

### Comparing `llama_index_postprocessor_nvidia_rerank-0.1.1/pyproject.toml` & `llama_index_postprocessor_nvidia_rerank-0.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 [tool.poetry]
 authors = ["Your Name <you@example.com>"]
 description = "llama-index postprocessor nvidia_rerank integration"
 license = "MIT"
 name = "llama-index-postprocessor-nvidia-rerank"
 packages = [{include = "llama_index/"}]
 readme = "README.md"
-version = "0.1.1"
+version = "0.1.2"
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<4.0"
 llama-index-core = "^0.10.35"
 
 [tool.poetry.group.dev.dependencies]
 black = {extras = ["jupyter"], version = "<=23.9.1,>=23.7.0"}
```

### Comparing `llama_index_postprocessor_nvidia_rerank-0.1.1/PKG-INFO` & `llama_index_postprocessor_nvidia_rerank-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llama-index-postprocessor-nvidia-rerank
-Version: 0.1.1
+Version: 0.1.2
 Summary: llama-index postprocessor nvidia_rerank integration
 License: MIT
 Author: Your Name
 Author-email: you@example.com
 Requires-Python: >=3.8.1,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

