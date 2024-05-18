# Comparing `tmp/llama_index_llms_nvidia-0.1.2.tar.gz` & `tmp/llama_index_llms_nvidia-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llama_index_llms_nvidia-0.1.2.tar", max compression
+gzip compressed data, was "llama_index_llms_nvidia-0.1.3.tar", max compression
```

## Comparing `llama_index_llms_nvidia-0.1.2.tar` & `llama_index_llms_nvidia-0.1.3.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1004 2024-05-09 20:01:33.838047 llama_index_llms_nvidia-0.1.2/README.md
--rw-r--r--   0        0        0       17 2024-05-09 20:01:33.838047 llama_index_llms_nvidia-0.1.2/llama_index/llms/nvidia/BUILD
--rw-r--r--   0        0        0       70 2024-05-09 20:01:33.838047 llama_index_llms_nvidia-0.1.2/llama_index/llms/nvidia/__init__.py
--rw-r--r--   0        0        0     3440 2024-05-09 20:01:33.838047 llama_index_llms_nvidia-0.1.2/llama_index/llms/nvidia/base.py
--rw-r--r--   0        0        0      617 2024-05-09 20:01:33.838047 llama_index_llms_nvidia-0.1.2/llama_index/llms/nvidia/utils.py
--rw-r--r--   0        0        0     1738 2024-05-09 20:01:33.838047 llama_index_llms_nvidia-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     1689 1970-01-01 00:00:00.000000 llama_index_llms_nvidia-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1004 2024-05-18 16:06:55.027765 llama_index_llms_nvidia-0.1.3/README.md
+-rw-r--r--   0        0        0       17 2024-05-18 16:06:55.031765 llama_index_llms_nvidia-0.1.3/llama_index/llms/nvidia/BUILD
+-rw-r--r--   0        0        0       70 2024-05-18 16:06:55.031765 llama_index_llms_nvidia-0.1.3/llama_index/llms/nvidia/__init__.py
+-rw-r--r--   0        0        0     4363 2024-05-18 16:06:55.031765 llama_index_llms_nvidia-0.1.3/llama_index/llms/nvidia/base.py
+-rw-r--r--   0        0        0      617 2024-05-18 16:06:55.031765 llama_index_llms_nvidia-0.1.3/llama_index/llms/nvidia/utils.py
+-rw-r--r--   0        0        0     1738 2024-05-18 16:06:55.031765 llama_index_llms_nvidia-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     1689 1970-01-01 00:00:00.000000 llama_index_llms_nvidia-0.1.3/PKG-INFO
```

### Comparing `llama_index_llms_nvidia-0.1.2/README.md` & `llama_index_llms_nvidia-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `llama_index_llms_nvidia-0.1.2/llama_index/llms/nvidia/utils.py` & `llama_index_llms_nvidia-0.1.3/llama_index/llms/nvidia/utils.py`

 * *Files identical despite different names*

### Comparing `llama_index_llms_nvidia-0.1.2/pyproject.toml` & `llama_index_llms_nvidia-0.1.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 [tool.poetry]
 authors = ["Chris Alexiuk <calexiuk@nvidia.com>"]
 description = "llama-index llms nvidia api catalog integration"
 license = "MIT"
 name = "llama-index-llms-nvidia"
 packages = [{include = "llama_index/"}]
 readme = "README.md"
-version = "0.1.2"
+version = "0.1.3"
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<4.0"
 llama-index-core = "^0.10.0"
 llama-index-llms-openai = "^0.1.17"
 llama-index-llms-openai-like = "^0.1.3"
```

### Comparing `llama_index_llms_nvidia-0.1.2/PKG-INFO` & `llama_index_llms_nvidia-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llama-index-llms-nvidia
-Version: 0.1.2
+Version: 0.1.3
 Summary: llama-index llms nvidia api catalog integration
 License: MIT
 Author: Chris Alexiuk
 Author-email: calexiuk@nvidia.com
 Requires-Python: >=3.8.1,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

