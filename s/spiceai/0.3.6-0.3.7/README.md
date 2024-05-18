# Comparing `tmp/spiceai-0.3.6.tar.gz` & `tmp/spiceai-0.3.7.tar.gz`

## Comparing `spiceai-0.3.6.tar` & `spiceai-0.3.7.tar`

### file list

```diff
@@ -1,20 +1,23 @@
--rw-r--r--   0        0        0      655 2020-02-02 00:00:00.000000 spiceai-0.3.6/.github/workflows/ruff.yml
--rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 spiceai-0.3.6/scripts/mytoml.toml
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 spiceai-0.3.6/scripts/prompt.txt
--rw-r--r--   0        0        0     5999 2020-02-02 00:00:00.000000 spiceai-0.3.6/scripts/run.py
--rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 spiceai-0.3.6/spice/__init__.py
--rw-r--r--   0        0        0      632 2020-02-02 00:00:00.000000 spiceai-0.3.6/spice/errors.py
--rw-r--r--   0        0        0     6897 2020-02-02 00:00:00.000000 spiceai-0.3.6/spice/models.py
--rw-r--r--   0        0        0     2142 2020-02-02 00:00:00.000000 spiceai-0.3.6/spice/providers.py
--rw-r--r--   0        0        0    35102 2020-02-02 00:00:00.000000 spiceai-0.3.6/spice/spice.py
--rw-r--r--   0        0        0     7622 2020-02-02 00:00:00.000000 spiceai-0.3.6/spice/spice_message.py
--rw-r--r--   0        0        0      917 2020-02-02 00:00:00.000000 spiceai-0.3.6/spice/utils.py
--rw-r--r--   0        0        0    18773 2020-02-02 00:00:00.000000 spiceai-0.3.6/spice/wrapped_clients.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 spiceai-0.3.6/tests/__init__.py
--rw-r--r--   0        0        0     3455 2020-02-02 00:00:00.000000 spiceai-0.3.6/tests/conftest.py
--rw-r--r--   0        0        0      781 2020-02-02 00:00:00.000000 spiceai-0.3.6/tests/test_spice.py
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 spiceai-0.3.6/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 spiceai-0.3.6/LICENSE
--rw-r--r--   0        0        0     5903 2020-02-02 00:00:00.000000 spiceai-0.3.6/README.md
--rw-r--r--   0        0        0      574 2020-02-02 00:00:00.000000 spiceai-0.3.6/pyproject.toml
--rw-r--r--   0        0        0     6445 2020-02-02 00:00:00.000000 spiceai-0.3.6/PKG-INFO
+-rw-r--r--   0        0        0    28786 2020-02-02 00:00:00.000000 spiceai-0.3.7/tags
+-rw-r--r--   0        0        0      655 2020-02-02 00:00:00.000000 spiceai-0.3.7/.github/workflows/ruff.yml
+-rw-r--r--   0        0        0      667 2020-02-02 00:00:00.000000 spiceai-0.3.7/.ropeproject/globalnames
+-rw-r--r--   0        0        0    89341 2020-02-02 00:00:00.000000 spiceai-0.3.7/.ropeproject/history
+-rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 spiceai-0.3.7/scripts/mytoml.toml
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 spiceai-0.3.7/scripts/prompt.txt
+-rw-r--r--   0        0        0     5999 2020-02-02 00:00:00.000000 spiceai-0.3.7/scripts/run.py
+-rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 spiceai-0.3.7/spice/__init__.py
+-rw-r--r--   0        0        0      632 2020-02-02 00:00:00.000000 spiceai-0.3.7/spice/errors.py
+-rw-r--r--   0        0        0     6897 2020-02-02 00:00:00.000000 spiceai-0.3.7/spice/models.py
+-rw-r--r--   0        0        0     2142 2020-02-02 00:00:00.000000 spiceai-0.3.7/spice/providers.py
+-rw-r--r--   0        0        0    35385 2020-02-02 00:00:00.000000 spiceai-0.3.7/spice/spice.py
+-rw-r--r--   0        0        0     7622 2020-02-02 00:00:00.000000 spiceai-0.3.7/spice/spice_message.py
+-rw-r--r--   0        0        0      917 2020-02-02 00:00:00.000000 spiceai-0.3.7/spice/utils.py
+-rw-r--r--   0        0        0    18773 2020-02-02 00:00:00.000000 spiceai-0.3.7/spice/wrapped_clients.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 spiceai-0.3.7/tests/__init__.py
+-rw-r--r--   0        0        0     3455 2020-02-02 00:00:00.000000 spiceai-0.3.7/tests/conftest.py
+-rw-r--r--   0        0        0      781 2020-02-02 00:00:00.000000 spiceai-0.3.7/tests/test_spice.py
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 spiceai-0.3.7/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 spiceai-0.3.7/LICENSE
+-rw-r--r--   0        0        0     5903 2020-02-02 00:00:00.000000 spiceai-0.3.7/README.md
+-rw-r--r--   0        0        0      574 2020-02-02 00:00:00.000000 spiceai-0.3.7/pyproject.toml
+-rw-r--r--   0        0        0     6445 2020-02-02 00:00:00.000000 spiceai-0.3.7/PKG-INFO
```

### Comparing `spiceai-0.3.6/.github/workflows/ruff.yml` & `spiceai-0.3.7/.github/workflows/ruff.yml`

 * *Files identical despite different names*

### Comparing `spiceai-0.3.6/scripts/run.py` & `spiceai-0.3.7/scripts/run.py`

 * *Files identical despite different names*

### Comparing `spiceai-0.3.6/spice/errors.py` & `spiceai-0.3.7/spice/errors.py`

 * *Files identical despite different names*

### Comparing `spiceai-0.3.6/spice/models.py` & `spiceai-0.3.7/spice/models.py`

 * *Files identical despite different names*

### Comparing `spiceai-0.3.6/spice/providers.py` & `spiceai-0.3.7/spice/providers.py`

 * *Files identical despite different names*

### Comparing `spiceai-0.3.6/spice/spice.py` & `spiceai-0.3.7/spice/spice.py`

 * *Files 1% similar despite different names*

```diff
@@ -201,14 +201,15 @@
     def __init__(
         self,
         default_text_model: Optional[TextModel | str] = None,
         default_embeddings_model: Optional[EmbeddingModel | str] = None,
         model_aliases: Optional[Dict[str, Model | str]] = None,
         logging_dir: Optional[Path | str] = None,
         logging_callback: Optional[Callable[[SpiceResponse, str, str], None]] = None,
+        default_temperature: Optional[float] = None,
     ):
         """
         Creates a new Spice client.
 
         Args:
             default_text_model: The default model that will be used for chat completions if no other model is given.
             Will raise an InvalidModelError if the model is not a text model.
@@ -217,14 +218,16 @@
             Will raise an InvalidModelError if the model is not an embeddings model.
 
             model_aliases: A custom model name map.
 
             logging_dir: If not None, will log all api calls to the given directory.
 
             logging_callback: If not None, will call the given function with the SpiceResponse, the name of the run, and the name of the call after every call finishes.
+
+            default_temperature: The default temperature to use for chat completions if no other temperature is given.
         """
 
         if isinstance(default_text_model, str):
             text_model = get_model_from_name(default_text_model)
         else:
             text_model = default_text_model
         if text_model and not isinstance(text_model, TextModel):
@@ -234,14 +237,15 @@
         if isinstance(default_embeddings_model, str):
             embeddings_model = get_model_from_name(default_embeddings_model)
         else:
             embeddings_model = default_embeddings_model
         if embeddings_model and not isinstance(embeddings_model, EmbeddingModel):
             raise InvalidModelError("Default embeddings model must be an embeddings model")
         self._default_embeddings_model = embeddings_model
+        self._default_temperature = default_temperature
 
         # TODO: Should we validate model aliases?
         self._model_aliases = model_aliases
 
         self._total_cost: float = 0
         self._prompts: Dict[str, str] = {}
 
@@ -346,15 +350,15 @@
             if response_format == {"type": "text"}:
                 response_format = None
 
         return SpiceCallArgs(
             model=model.name,
             messages=messages,
             stream=stream,
-            temperature=temperature,
+            temperature=self._default_temperature if temperature is None else temperature,
             max_tokens=max_tokens,
             response_format=response_format,
         )
 
     async def get_response(
         self,
         messages: Collection[SpiceMessage],
```

### Comparing `spiceai-0.3.6/spice/spice_message.py` & `spiceai-0.3.7/spice/spice_message.py`

 * *Files identical despite different names*

### Comparing `spiceai-0.3.6/spice/utils.py` & `spiceai-0.3.7/spice/utils.py`

 * *Files identical despite different names*

### Comparing `spiceai-0.3.6/spice/wrapped_clients.py` & `spiceai-0.3.7/spice/wrapped_clients.py`

 * *Files identical despite different names*

### Comparing `spiceai-0.3.6/tests/conftest.py` & `spiceai-0.3.7/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `spiceai-0.3.6/tests/test_spice.py` & `spiceai-0.3.7/tests/test_spice.py`

 * *Files identical despite different names*

### Comparing `spiceai-0.3.6/LICENSE` & `spiceai-0.3.7/LICENSE`

 * *Files identical despite different names*

### Comparing `spiceai-0.3.6/README.md` & `spiceai-0.3.7/README.md`

 * *Files identical despite different names*

### Comparing `spiceai-0.3.6/pyproject.toml` & `spiceai-0.3.7/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 [tool.hatch]
 
 [tool.hatch.build.targets.wheel]
 packages=["spice"]
 
 [project]
 name = "spiceai"
-version = "0.3.6"
+version = "0.3.7"
 license = {text = "Apache-2.0"}
 description = "A Python library for building AI-powered applications."
 readme = "README.md"
 dependencies = [
     "python-dotenv",
     "openai",
     "anthropic",
```

### Comparing `spiceai-0.3.6/PKG-INFO` & `spiceai-0.3.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: spiceai
-Version: 0.3.6
+Version: 0.3.7
 Summary: A Python library for building AI-powered applications.
 License: Apache-2.0
 License-File: LICENSE
 Requires-Dist: anthropic
 Requires-Dist: httpx
 Requires-Dist: jinja2
 Requires-Dist: openai
```

