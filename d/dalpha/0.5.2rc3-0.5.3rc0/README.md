# Comparing `tmp/dalpha-0.5.2rc3.tar.gz` & `tmp/dalpha-0.5.3rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dalpha-0.5.2rc3.tar", max compression
+gzip compressed data, was "dalpha-0.5.3rc0.tar", max compression
```

## Comparing `dalpha-0.5.2rc3.tar` & `dalpha-0.5.3rc0.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0      578 2023-12-18 04:10:26.318635 dalpha-0.5.2rc3/README.md
--rw-r--r--   0        0        0     2077 2024-05-16 07:16:07.976796 dalpha-0.5.2rc3/dalpha/__init__.py
--rw-r--r--   0        0        0     8282 2024-05-16 17:41:28.081119 dalpha-0.5.2rc3/dalpha/agent.py
--rw-r--r--   0        0        0     7019 2024-05-10 10:54:52.512416 dalpha-0.5.2rc3/dalpha/backend_cli.py
--rw-r--r--   0        0        0      555 2024-05-08 06:25:10.211719 dalpha-0.5.2rc3/dalpha/cobra_cls.py
--rw-r--r--   0        0        0      573 2024-02-28 08:10:55.063883 dalpha-0.5.2rc3/dalpha/context.py
--rw-r--r--   0        0        0     3036 2024-05-02 07:23:00.795089 dalpha-0.5.2rc3/dalpha/data_update_cls.py
--rw-r--r--   0        0        0      940 2024-05-02 07:23:00.795089 dalpha-0.5.2rc3/dalpha/dto.py
--rw-r--r--   0        0        0      616 2024-05-16 07:16:07.980796 dalpha-0.5.2rc3/dalpha/exception.py
--rw-r--r--   0        0        0     5954 2024-05-16 07:16:07.980796 dalpha-0.5.2rc3/dalpha/inference_cls.py
--rw-r--r--   0        0        0      233 2024-03-25 02:37:47.094337 dalpha-0.5.2rc3/dalpha/kafka_cli.py
--rw-r--r--   0        0        0     1861 2024-03-11 02:52:37.986799 dalpha-0.5.2rc3/dalpha/logging/__init__.py
--rw-r--r--   0        0        0      229 2024-02-28 08:10:55.063883 dalpha-0.5.2rc3/dalpha/logging/events.py
--rw-r--r--   0        0        0     1116 2024-02-28 08:10:55.063883 dalpha-0.5.2rc3/dalpha/logging/log_formatter.py
--rw-r--r--   0        0        0     1817 2024-02-28 08:10:55.063883 dalpha-0.5.2rc3/dalpha/logging/utils.py
--rw-r--r--   0        0        0     6687 2024-05-16 17:41:28.081119 dalpha-0.5.2rc3/dalpha/message_consumer.py
--rw-r--r--   0        0        0     1703 2024-05-10 10:54:52.512416 dalpha-0.5.2rc3/dalpha/openai_cls.py
--rw-r--r--   0        0        0     6079 2024-05-02 07:23:00.795089 dalpha-0.5.2rc3/dalpha/redis_cli.py
--rw-r--r--   0        0        0     1886 2024-05-02 07:23:00.795089 dalpha-0.5.2rc3/dalpha/redis_cls.py
--rw-r--r--   0        0        0      776 2024-05-10 10:54:52.512416 dalpha-0.5.2rc3/dalpha/request.py
--rw-r--r--   0        0        0     2689 2024-05-10 10:54:52.512416 dalpha-0.5.2rc3/dalpha/s3.py
--rw-r--r--   0        0        0      497 2024-02-28 08:10:55.063883 dalpha-0.5.2rc3/dalpha/signal_handler.py
--rw-r--r--   0        0        0      767 2024-05-10 10:54:52.512416 dalpha-0.5.2rc3/dalpha/slack.py
--rw-r--r--   0        0        0     2355 2024-05-10 10:54:52.512416 dalpha-0.5.2rc3/dalpha/update_agent.py
--rw-r--r--   0        0        0      952 2024-05-16 17:41:28.081119 dalpha-0.5.2rc3/pyproject.toml
--rw-r--r--   0        0        0     1362 1970-01-01 00:00:00.000000 dalpha-0.5.2rc3/PKG-INFO
+-rw-r--r--   0        0        0      578 2023-12-18 04:10:26.318635 dalpha-0.5.3rc0/README.md
+-rw-r--r--   0        0        0     2077 2024-05-16 07:16:07.976796 dalpha-0.5.3rc0/dalpha/__init__.py
+-rw-r--r--   0        0        0     8282 2024-05-16 17:41:28.081119 dalpha-0.5.3rc0/dalpha/agent.py
+-rw-r--r--   0        0        0     7019 2024-05-10 10:54:52.512416 dalpha-0.5.3rc0/dalpha/backend_cli.py
+-rw-r--r--   0        0        0      555 2024-05-08 06:25:10.211719 dalpha-0.5.3rc0/dalpha/cobra_cls.py
+-rw-r--r--   0        0        0      573 2024-02-28 08:10:55.063883 dalpha-0.5.3rc0/dalpha/context.py
+-rw-r--r--   0        0        0     3036 2024-05-02 07:23:00.795089 dalpha-0.5.3rc0/dalpha/data_update_cls.py
+-rw-r--r--   0        0        0      940 2024-05-02 07:23:00.795089 dalpha-0.5.3rc0/dalpha/dto.py
+-rw-r--r--   0        0        0      616 2024-05-16 07:16:07.980796 dalpha-0.5.3rc0/dalpha/exception.py
+-rw-r--r--   0        0        0     6000 2024-05-18 12:36:17.240345 dalpha-0.5.3rc0/dalpha/inference_cls.py
+-rw-r--r--   0        0        0      233 2024-03-25 02:37:47.094337 dalpha-0.5.3rc0/dalpha/kafka_cli.py
+-rw-r--r--   0        0        0     1861 2024-03-11 02:52:37.986799 dalpha-0.5.3rc0/dalpha/logging/__init__.py
+-rw-r--r--   0        0        0      229 2024-02-28 08:10:55.063883 dalpha-0.5.3rc0/dalpha/logging/events.py
+-rw-r--r--   0        0        0     1116 2024-02-28 08:10:55.063883 dalpha-0.5.3rc0/dalpha/logging/log_formatter.py
+-rw-r--r--   0        0        0     1817 2024-02-28 08:10:55.063883 dalpha-0.5.3rc0/dalpha/logging/utils.py
+-rw-r--r--   0        0        0     6687 2024-05-16 17:41:28.081119 dalpha-0.5.3rc0/dalpha/message_consumer.py
+-rw-r--r--   0        0        0     1703 2024-05-10 10:54:52.512416 dalpha-0.5.3rc0/dalpha/openai_cls.py
+-rw-r--r--   0        0        0     6079 2024-05-02 07:23:00.795089 dalpha-0.5.3rc0/dalpha/redis_cli.py
+-rw-r--r--   0        0        0     1886 2024-05-02 07:23:00.795089 dalpha-0.5.3rc0/dalpha/redis_cls.py
+-rw-r--r--   0        0        0      776 2024-05-10 10:54:52.512416 dalpha-0.5.3rc0/dalpha/request.py
+-rw-r--r--   0        0        0     2689 2024-05-10 10:54:52.512416 dalpha-0.5.3rc0/dalpha/s3.py
+-rw-r--r--   0        0        0      497 2024-02-28 08:10:55.063883 dalpha-0.5.3rc0/dalpha/signal_handler.py
+-rw-r--r--   0        0        0      767 2024-05-10 10:54:52.512416 dalpha-0.5.3rc0/dalpha/slack.py
+-rw-r--r--   0        0        0     2355 2024-05-10 10:54:52.512416 dalpha-0.5.3rc0/dalpha/update_agent.py
+-rw-r--r--   0        0        0      952 2024-05-18 12:36:17.240345 dalpha-0.5.3rc0/pyproject.toml
+-rw-r--r--   0        0        0     1362 1970-01-01 00:00:00.000000 dalpha-0.5.3rc0/PKG-INFO
```

### Comparing `dalpha-0.5.2rc3/README.md` & `dalpha-0.5.3rc0/README.md`

 * *Files identical despite different names*

### Comparing `dalpha-0.5.2rc3/dalpha/__init__.py` & `dalpha-0.5.3rc0/dalpha/__init__.py`

 * *Files identical despite different names*

### Comparing `dalpha-0.5.2rc3/dalpha/agent.py` & `dalpha-0.5.3rc0/dalpha/agent.py`

 * *Files identical despite different names*

### Comparing `dalpha-0.5.2rc3/dalpha/backend_cli.py` & `dalpha-0.5.3rc0/dalpha/backend_cli.py`

 * *Files identical despite different names*

### Comparing `dalpha-0.5.2rc3/dalpha/cobra_cls.py` & `dalpha-0.5.3rc0/dalpha/cobra_cls.py`

 * *Files identical despite different names*

### Comparing `dalpha-0.5.2rc3/dalpha/context.py` & `dalpha-0.5.3rc0/dalpha/context.py`

 * *Files identical despite different names*

### Comparing `dalpha-0.5.2rc3/dalpha/data_update_cls.py` & `dalpha-0.5.3rc0/dalpha/data_update_cls.py`

 * *Files identical despite different names*

### Comparing `dalpha-0.5.2rc3/dalpha/dto.py` & `dalpha-0.5.3rc0/dalpha/dto.py`

 * *Files identical despite different names*

### Comparing `dalpha-0.5.2rc3/dalpha/exception.py` & `dalpha-0.5.3rc0/dalpha/exception.py`

 * *Files identical despite different names*

### Comparing `dalpha-0.5.2rc3/dalpha/inference_cls.py` & `dalpha-0.5.3rc0/dalpha/inference_cls.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 from dalpha.message_consumer import EvaluateItem
 
 
 class DalphaAI:
     def __init__(
         self,
         api_id: int,
-        inference: Callable[[Dict, EvaluateItem], InferenceResult],
+        inference: Callable[[Dict, EvaluateItem, bool], InferenceResult],
         load_globals: Callable[[], Dict],
         mock_file: Optional[str],
         mocks_file: Optional[str],
     ):
         self.wait_flag = True
 
         self.agent = Agent(api_id=api_id)
@@ -128,14 +128,15 @@
         try:
             logger.info("AI inference starts...")
             inference_start_time = time.time()
 
             inference_result: InferenceResult = self.inference(
                 globals=self.globals,
                 evaluate_item=input_json,
+                use_mock = self.is_mock
             )
             inference_end_time = time.time()
             logger.info(f"AI inference is done. Time taken: {inference_end_time - inference_start_time:.2f} sec")
         except ExpectedError as expected_error:
             self.agent.validate_error(evaluate_id=eval_id, output=expected_error.error_json, mock=self.is_mock, error_code=expected_error.error_code)
             self.wait_flag = True
             return
```

### Comparing `dalpha-0.5.2rc3/dalpha/logging/__init__.py` & `dalpha-0.5.3rc0/dalpha/logging/__init__.py`

 * *Files identical despite different names*

### Comparing `dalpha-0.5.2rc3/dalpha/logging/log_formatter.py` & `dalpha-0.5.3rc0/dalpha/logging/log_formatter.py`

 * *Files identical despite different names*

### Comparing `dalpha-0.5.2rc3/dalpha/logging/utils.py` & `dalpha-0.5.3rc0/dalpha/logging/utils.py`

 * *Files identical despite different names*

### Comparing `dalpha-0.5.2rc3/dalpha/message_consumer.py` & `dalpha-0.5.3rc0/dalpha/message_consumer.py`

 * *Files identical despite different names*

### Comparing `dalpha-0.5.2rc3/dalpha/openai_cls.py` & `dalpha-0.5.3rc0/dalpha/openai_cls.py`

 * *Files identical despite different names*

### Comparing `dalpha-0.5.2rc3/dalpha/redis_cli.py` & `dalpha-0.5.3rc0/dalpha/redis_cli.py`

 * *Files identical despite different names*

### Comparing `dalpha-0.5.2rc3/dalpha/redis_cls.py` & `dalpha-0.5.3rc0/dalpha/redis_cls.py`

 * *Files identical despite different names*

### Comparing `dalpha-0.5.2rc3/dalpha/request.py` & `dalpha-0.5.3rc0/dalpha/request.py`

 * *Files identical despite different names*

### Comparing `dalpha-0.5.2rc3/dalpha/s3.py` & `dalpha-0.5.3rc0/dalpha/s3.py`

 * *Files identical despite different names*

### Comparing `dalpha-0.5.2rc3/dalpha/slack.py` & `dalpha-0.5.3rc0/dalpha/slack.py`

 * *Files identical despite different names*

### Comparing `dalpha-0.5.2rc3/dalpha/update_agent.py` & `dalpha-0.5.3rc0/dalpha/update_agent.py`

 * *Files identical despite different names*

### Comparing `dalpha-0.5.2rc3/pyproject.toml` & `dalpha-0.5.3rc0/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dalpha"
-version = "0.5.2rc3"
+version = "0.5.3rc0"
 description = ""
 authors = ["devops <devops@dalpha.so>"]
 readme = "README.md"
 packages = [{include = "dalpha"}]
 
 [tool.poetry.dependencies]
 python = "^3.8"
@@ -17,15 +17,15 @@
 pydantic = "^2.7.1"
 
 [tool.poetry.group.dev.dependencies]
 twine = "^4.0.2"
 
 [project]
 name = "dalpha"
-version = "0.5.2rc3"
+version = "0.5.3rc0"
 authors = [
   { name="Beomseok", email="beomseok.kim@dalpha.so" },
   { name="Gideok", email="gideok.kim@dalpha.so" },
 ]
 description = "Dalpha internal sdk"
 readme = "README.md"
 requires-python = ">=3.9"
```

### Comparing `dalpha-0.5.2rc3/PKG-INFO` & `dalpha-0.5.3rc0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dalpha
-Version: 0.5.2rc3
+Version: 0.5.3rc0
 Summary: 
 Author: devops
 Author-email: devops@dalpha.so
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

