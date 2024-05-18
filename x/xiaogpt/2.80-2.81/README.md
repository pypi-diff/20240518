# Comparing `tmp/xiaogpt-2.80.tar.gz` & `tmp/xiaogpt-2.81.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xiaogpt-2.80.tar", last modified: Fri May 17 04:40:21 2024, max compression
+gzip compressed data, was "xiaogpt-2.81.tar", last modified: Sat May 18 04:01:17 2024, max compression
```

## Comparing `xiaogpt-2.80.tar` & `xiaogpt-2.81.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rw-r--r--   0        0        0     1063 2024-05-17 04:40:14.908027 xiaogpt-2.80/LICENSE
--rw-r--r--   0        0        0    23909 2024-05-17 04:40:14.908027 xiaogpt-2.80/README.md
--rw-r--r--   0        0        0     3829 2024-05-17 04:40:21.132065 xiaogpt-2.80/pyproject.toml
--rw-r--r--   0        0        0        0 2024-05-17 04:40:14.908027 xiaogpt-2.80/xiaogpt/__init__.py
--rw-r--r--   0        0        0       61 2024-05-17 04:40:14.908027 xiaogpt-2.80/xiaogpt/__main__.py
--rw-r--r--   0        0        0     1160 2024-05-17 04:40:14.908027 xiaogpt-2.80/xiaogpt/bot/__init__.py
--rw-r--r--   0        0        0     1467 2024-05-17 04:40:14.908027 xiaogpt-2.80/xiaogpt/bot/base_bot.py
--rw-r--r--   0        0        0     3660 2024-05-17 04:40:14.908027 xiaogpt-2.80/xiaogpt/bot/chatgptapi_bot.py
--rw-r--r--   0        0        0     2773 2024-05-17 04:40:14.908027 xiaogpt-2.80/xiaogpt/bot/doubao_bot.py
--rw-r--r--   0        0        0     2516 2024-05-17 04:40:14.908027 xiaogpt-2.80/xiaogpt/bot/gemini_bot.py
--rw-r--r--   0        0        0     1825 2024-05-17 04:40:14.908027 xiaogpt-2.80/xiaogpt/bot/glm_bot.py
--rw-r--r--   0        0        0     1944 2024-05-17 04:40:14.908027 xiaogpt-2.80/xiaogpt/bot/langchain_bot.py
--rw-r--r--   0        0        0      708 2024-05-17 04:40:14.908027 xiaogpt-2.80/xiaogpt/bot/llama_bot.py
--rw-r--r--   0        0        0      822 2024-05-17 04:40:14.908027 xiaogpt-2.80/xiaogpt/bot/moonshot_bot.py
--rw-r--r--   0        0        0     3657 2024-05-17 04:40:14.908027 xiaogpt-2.80/xiaogpt/bot/qwen_bot.py
--rw-r--r--   0        0        0      784 2024-05-17 04:40:14.908027 xiaogpt-2.80/xiaogpt/bot/yi_bot.py
--rw-r--r--   0        0        0     5711 2024-05-17 04:40:14.908027 xiaogpt-2.80/xiaogpt/cli.py
--rw-r--r--   0        0        0     6734 2024-05-17 04:40:14.908027 xiaogpt-2.80/xiaogpt/config.py
--rw-r--r--   0        0        0     2616 2024-05-17 04:40:14.912027 xiaogpt-2.80/xiaogpt/langchain/callbacks.py
--rw-r--r--   0        0        0     1495 2024-05-17 04:40:14.912027 xiaogpt-2.80/xiaogpt/langchain/chain.py
--rw-r--r--   0        0        0     6372 2024-05-17 04:40:14.912027 xiaogpt-2.80/xiaogpt/langchain/examples/email/mail_box.py
--rw-r--r--   0        0        0     1561 2024-05-17 04:40:14.912027 xiaogpt-2.80/xiaogpt/langchain/examples/email/mail_summary_tools.py
--rw-r--r--   0        0        0      145 2024-05-17 04:40:14.912027 xiaogpt-2.80/xiaogpt/tts/__init__.py
--rw-r--r--   0        0        0     4656 2024-05-17 04:40:14.912027 xiaogpt-2.80/xiaogpt/tts/base.py
--rw-r--r--   0        0        0     1095 2024-05-17 04:40:14.912027 xiaogpt-2.80/xiaogpt/tts/mi.py
--rw-r--r--   0        0        0     1058 2024-05-17 04:40:14.912027 xiaogpt-2.80/xiaogpt/tts/tetos.py
--rw-r--r--   0        0        0     2072 2024-05-17 04:40:14.912027 xiaogpt-2.80/xiaogpt/utils.py
--rw-r--r--   0        0        0    16524 2024-05-17 04:40:14.912027 xiaogpt-2.80/xiaogpt/xiaogpt.py
--rw-r--r--   0        0        0    29638 1970-01-01 00:00:00.000000 xiaogpt-2.80/PKG-INFO
+-rw-r--r--   0        0        0     1063 2024-05-18 04:01:06.636107 xiaogpt-2.81/LICENSE
+-rw-r--r--   0        0        0    23909 2024-05-18 04:01:06.636107 xiaogpt-2.81/README.md
+-rw-r--r--   0        0        0     3829 2024-05-18 04:01:17.024246 xiaogpt-2.81/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-18 04:01:06.636107 xiaogpt-2.81/xiaogpt/__init__.py
+-rw-r--r--   0        0        0       61 2024-05-18 04:01:06.636107 xiaogpt-2.81/xiaogpt/__main__.py
+-rw-r--r--   0        0        0     1160 2024-05-18 04:01:06.636107 xiaogpt-2.81/xiaogpt/bot/__init__.py
+-rw-r--r--   0        0        0     1467 2024-05-18 04:01:06.636107 xiaogpt-2.81/xiaogpt/bot/base_bot.py
+-rw-r--r--   0        0        0     3660 2024-05-18 04:01:06.636107 xiaogpt-2.81/xiaogpt/bot/chatgptapi_bot.py
+-rw-r--r--   0        0        0     2773 2024-05-18 04:01:06.636107 xiaogpt-2.81/xiaogpt/bot/doubao_bot.py
+-rw-r--r--   0        0        0     2516 2024-05-18 04:01:06.636107 xiaogpt-2.81/xiaogpt/bot/gemini_bot.py
+-rw-r--r--   0        0        0     1825 2024-05-18 04:01:06.636107 xiaogpt-2.81/xiaogpt/bot/glm_bot.py
+-rw-r--r--   0        0        0     1944 2024-05-18 04:01:06.636107 xiaogpt-2.81/xiaogpt/bot/langchain_bot.py
+-rw-r--r--   0        0        0      708 2024-05-18 04:01:06.636107 xiaogpt-2.81/xiaogpt/bot/llama_bot.py
+-rw-r--r--   0        0        0      822 2024-05-18 04:01:06.636107 xiaogpt-2.81/xiaogpt/bot/moonshot_bot.py
+-rw-r--r--   0        0        0     3657 2024-05-18 04:01:06.636107 xiaogpt-2.81/xiaogpt/bot/qwen_bot.py
+-rw-r--r--   0        0        0      784 2024-05-18 04:01:06.636107 xiaogpt-2.81/xiaogpt/bot/yi_bot.py
+-rw-r--r--   0        0        0     5711 2024-05-18 04:01:06.636107 xiaogpt-2.81/xiaogpt/cli.py
+-rw-r--r--   0        0        0     6734 2024-05-18 04:01:06.636107 xiaogpt-2.81/xiaogpt/config.py
+-rw-r--r--   0        0        0     2616 2024-05-18 04:01:06.636107 xiaogpt-2.81/xiaogpt/langchain/callbacks.py
+-rw-r--r--   0        0        0     1495 2024-05-18 04:01:06.636107 xiaogpt-2.81/xiaogpt/langchain/chain.py
+-rw-r--r--   0        0        0     6372 2024-05-18 04:01:06.636107 xiaogpt-2.81/xiaogpt/langchain/examples/email/mail_box.py
+-rw-r--r--   0        0        0     1561 2024-05-18 04:01:06.636107 xiaogpt-2.81/xiaogpt/langchain/examples/email/mail_summary_tools.py
+-rw-r--r--   0        0        0      145 2024-05-18 04:01:06.640107 xiaogpt-2.81/xiaogpt/tts/__init__.py
+-rw-r--r--   0        0        0     4656 2024-05-18 04:01:06.640107 xiaogpt-2.81/xiaogpt/tts/base.py
+-rw-r--r--   0        0        0     1095 2024-05-18 04:01:06.640107 xiaogpt-2.81/xiaogpt/tts/mi.py
+-rw-r--r--   0        0        0     1058 2024-05-18 04:01:06.640107 xiaogpt-2.81/xiaogpt/tts/tetos.py
+-rw-r--r--   0        0        0     2072 2024-05-18 04:01:06.640107 xiaogpt-2.81/xiaogpt/utils.py
+-rw-r--r--   0        0        0    16524 2024-05-18 04:01:06.640107 xiaogpt-2.81/xiaogpt/xiaogpt.py
+-rw-r--r--   0        0        0    29638 1970-01-01 00:00:00.000000 xiaogpt-2.81/PKG-INFO
```

### Comparing `xiaogpt-2.80/LICENSE` & `xiaogpt-2.81/LICENSE`

 * *Files identical despite different names*

### Comparing `xiaogpt-2.80/README.md` & `xiaogpt-2.81/README.md`

 * *Files identical despite different names*

### Comparing `xiaogpt-2.80/pyproject.toml` & `xiaogpt-2.81/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -25,15 +25,15 @@
     "numexpr>=2.8.6",
     "dashscope>=1.10.0",
     "tetos>=0.2.1",
     "groq>=0.5.0",
     "pyyaml>=6.0.1",
 ]
 dynamic = []
-version = "2.80"
+version = "2.81"
 
 [project.license]
 text = "MIT"
 
 [project.urls]
 Homepage = "https://github.com/yihong0618/xiaogpt"
```

### Comparing `xiaogpt-2.80/xiaogpt/bot/__init__.py` & `xiaogpt-2.81/xiaogpt/bot/__init__.py`

 * *Files identical despite different names*

### Comparing `xiaogpt-2.80/xiaogpt/bot/base_bot.py` & `xiaogpt-2.81/xiaogpt/bot/base_bot.py`

 * *Files identical despite different names*

### Comparing `xiaogpt-2.80/xiaogpt/bot/chatgptapi_bot.py` & `xiaogpt-2.81/xiaogpt/bot/chatgptapi_bot.py`

 * *Files identical despite different names*

### Comparing `xiaogpt-2.80/xiaogpt/bot/doubao_bot.py` & `xiaogpt-2.81/xiaogpt/bot/doubao_bot.py`

 * *Files identical despite different names*

### Comparing `xiaogpt-2.80/xiaogpt/bot/gemini_bot.py` & `xiaogpt-2.81/xiaogpt/bot/gemini_bot.py`

 * *Files identical despite different names*

### Comparing `xiaogpt-2.80/xiaogpt/bot/glm_bot.py` & `xiaogpt-2.81/xiaogpt/bot/glm_bot.py`

 * *Files identical despite different names*

### Comparing `xiaogpt-2.80/xiaogpt/bot/langchain_bot.py` & `xiaogpt-2.81/xiaogpt/bot/langchain_bot.py`

 * *Files identical despite different names*

### Comparing `xiaogpt-2.80/xiaogpt/bot/llama_bot.py` & `xiaogpt-2.81/xiaogpt/bot/llama_bot.py`

 * *Files identical despite different names*

### Comparing `xiaogpt-2.80/xiaogpt/bot/moonshot_bot.py` & `xiaogpt-2.81/xiaogpt/bot/moonshot_bot.py`

 * *Files identical despite different names*

### Comparing `xiaogpt-2.80/xiaogpt/bot/qwen_bot.py` & `xiaogpt-2.81/xiaogpt/bot/qwen_bot.py`

 * *Files identical despite different names*

### Comparing `xiaogpt-2.80/xiaogpt/bot/yi_bot.py` & `xiaogpt-2.81/xiaogpt/bot/yi_bot.py`

 * *Files identical despite different names*

### Comparing `xiaogpt-2.80/xiaogpt/cli.py` & `xiaogpt-2.81/xiaogpt/cli.py`

 * *Files identical despite different names*

### Comparing `xiaogpt-2.80/xiaogpt/config.py` & `xiaogpt-2.81/xiaogpt/config.py`

 * *Files identical despite different names*

### Comparing `xiaogpt-2.80/xiaogpt/langchain/callbacks.py` & `xiaogpt-2.81/xiaogpt/langchain/callbacks.py`

 * *Files identical despite different names*

### Comparing `xiaogpt-2.80/xiaogpt/langchain/chain.py` & `xiaogpt-2.81/xiaogpt/langchain/chain.py`

 * *Files identical despite different names*

### Comparing `xiaogpt-2.80/xiaogpt/langchain/examples/email/mail_box.py` & `xiaogpt-2.81/xiaogpt/langchain/examples/email/mail_box.py`

 * *Files identical despite different names*

### Comparing `xiaogpt-2.80/xiaogpt/langchain/examples/email/mail_summary_tools.py` & `xiaogpt-2.81/xiaogpt/langchain/examples/email/mail_summary_tools.py`

 * *Files identical despite different names*

### Comparing `xiaogpt-2.80/xiaogpt/tts/base.py` & `xiaogpt-2.81/xiaogpt/tts/base.py`

 * *Files identical despite different names*

### Comparing `xiaogpt-2.80/xiaogpt/tts/mi.py` & `xiaogpt-2.81/xiaogpt/tts/mi.py`

 * *Files identical despite different names*

### Comparing `xiaogpt-2.80/xiaogpt/tts/tetos.py` & `xiaogpt-2.81/xiaogpt/tts/tetos.py`

 * *Files identical despite different names*

### Comparing `xiaogpt-2.80/xiaogpt/utils.py` & `xiaogpt-2.81/xiaogpt/utils.py`

 * *Files identical despite different names*

### Comparing `xiaogpt-2.80/xiaogpt/xiaogpt.py` & `xiaogpt-2.81/xiaogpt/xiaogpt.py`

 * *Files identical despite different names*

### Comparing `xiaogpt-2.80/PKG-INFO` & `xiaogpt-2.81/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xiaogpt
-Version: 2.80
+Version: 2.81
 Summary: Play ChatGPT or other LLM with xiaomi AI speaker
 Author-Email: yihong0618 <zouzou0208@gmail.com>
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Project-URL: Homepage, https://github.com/yihong0618/xiaogpt
```

