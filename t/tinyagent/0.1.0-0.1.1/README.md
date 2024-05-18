# Comparing `tmp/tinyagent-0.1.0.tar.gz` & `tmp/tinyagent-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tinyagent-0.1.0.tar", last modified: Sat May 18 15:38:05 2024, max compression
+gzip compressed data, was "tinyagent-0.1.1.tar", last modified: Sat May 18 16:24:26 2024, max compression
```

## Comparing `tinyagent-0.1.0.tar` & `tinyagent-0.1.1.tar`

### file list

```diff
@@ -1,40 +1,41 @@
-drwxr-xr-x   0 lan        (501) staff       (20)        0 2024-05-18 15:38:05.338869 tinyagent-0.1.0/
--rw-r--r--   0 lan        (501) staff       (20)      789 2024-05-18 07:09:41.000000 tinyagent-0.1.0/.gitignore
--rw-r--r--   0 lan        (501) staff       (20)     1069 2024-05-18 15:37:21.000000 tinyagent-0.1.0/LICENSE
--rw-r--r--   0 lan        (501) staff       (20)      462 2024-05-18 15:38:05.338744 tinyagent-0.1.0/PKG-INFO
--rw-r--r--   0 lan        (501) staff       (20)       83 2024-05-18 04:41:33.000000 tinyagent-0.1.0/README.md
--rw-r--r--   0 lan        (501) staff       (20)    32102 2024-05-18 04:46:25.000000 tinyagent-0.1.0/poetry.lock
--rw-r--r--   0 lan        (501) staff       (20)      303 2024-05-18 04:46:25.000000 tinyagent-0.1.0/pyproject.toml
--rw-r--r--   0 lan        (501) staff       (20)       38 2024-05-18 15:38:05.338904 tinyagent-0.1.0/setup.cfg
--rw-r--r--   0 lan        (501) staff       (20)      589 2024-05-18 15:34:54.000000 tinyagent-0.1.0/setup.py
-drwxr-xr-x   0 lan        (501) staff       (20)        0 2024-05-18 15:38:05.333914 tinyagent-0.1.0/tests/
-drwxr-xr-x   0 lan        (501) staff       (20)        0 2024-05-18 15:38:05.334185 tinyagent-0.1.0/tests/resources/
--rw-r--r--   0 lan        (501) staff       (20)      785 2024-05-18 08:00:19.000000 tinyagent-0.1.0/tests/resources/test.jpg
--rw-r--r--   0 lan        (501) staff       (20)     1987 2024-05-18 12:18:20.000000 tinyagent-0.1.0/tests/test_claude.py
--rw-r--r--   0 lan        (501) staff       (20)     1991 2024-05-18 14:56:21.000000 tinyagent-0.1.0/tests/test_gpt.py
--rw-r--r--   0 lan        (501) staff       (20)     1018 2024-05-18 10:19:39.000000 tinyagent-0.1.0/tests/test_tool.py
-drwxr-xr-x   0 lan        (501) staff       (20)        0 2024-05-18 15:38:05.334505 tinyagent-0.1.0/tinyagent/
--rw-r--r--   0 lan        (501) staff       (20)      562 2024-05-18 15:30:51.000000 tinyagent-0.1.0/tinyagent/__init__.py
-drwxr-xr-x   0 lan        (501) staff       (20)        0 2024-05-18 15:38:05.336418 tinyagent-0.1.0/tinyagent/agent/
--rw-r--r--   0 lan        (501) staff       (20)      385 2024-05-18 04:39:39.000000 tinyagent-0.1.0/tinyagent/agent/__init__.py
--rw-r--r--   0 lan        (501) staff       (20)     4114 2024-05-18 14:51:25.000000 tinyagent-0.1.0/tinyagent/agent/base.py
-drwxr-xr-x   0 lan        (501) staff       (20)        0 2024-05-18 15:38:05.337133 tinyagent-0.1.0/tinyagent/agent/claude/
--rw-r--r--   0 lan        (501) staff       (20)        0 2024-05-18 05:29:38.000000 tinyagent-0.1.0/tinyagent/agent/claude/__init_..py
--rw-r--r--   0 lan        (501) staff       (20)     9002 2024-05-18 14:08:11.000000 tinyagent-0.1.0/tinyagent/agent/claude/agent.py
--rw-r--r--   0 lan        (501) staff       (20)     2333 2024-05-18 12:49:02.000000 tinyagent-0.1.0/tinyagent/agent/claude/client.py
-drwxr-xr-x   0 lan        (501) staff       (20)        0 2024-05-18 15:38:05.337670 tinyagent-0.1.0/tinyagent/agent/gpt/
--rw-r--r--   0 lan        (501) staff       (20)     8610 2024-05-18 15:01:17.000000 tinyagent-0.1.0/tinyagent/agent/gpt/agent.py
--rw-r--r--   0 lan        (501) staff       (20)     2420 2024-05-18 15:01:24.000000 tinyagent-0.1.0/tinyagent/agent/gpt/client.py
--rw-r--r--   0 lan        (501) staff       (20)     2250 2024-05-18 14:29:27.000000 tinyagent-0.1.0/tinyagent/agent/schema.py
--rw-r--r--   0 lan        (501) staff       (20)     2328 2024-05-18 11:39:01.000000 tinyagent-0.1.0/tinyagent/agent/tools.py
--rw-r--r--   0 lan        (501) staff       (20)      191 2024-05-18 05:33:28.000000 tinyagent-0.1.0/tinyagent/agent/utils.py
-drwxr-xr-x   0 lan        (501) staff       (20)        0 2024-05-18 15:38:05.338457 tinyagent-0.1.0/tinyagent/common/
--rw-r--r--   0 lan        (501) staff       (20)       73 2024-05-18 06:36:17.000000 tinyagent-0.1.0/tinyagent/common/__init__.py
--rw-r--r--   0 lan        (501) staff       (20)      358 2024-05-18 07:53:30.000000 tinyagent-0.1.0/tinyagent/common/event.py
--rw-r--r--   0 lan        (501) staff       (20)      107 2024-05-18 05:39:07.000000 tinyagent-0.1.0/tinyagent/common/time.py
-drwxr-xr-x   0 lan        (501) staff       (20)        0 2024-05-18 15:38:05.335316 tinyagent-0.1.0/tinyagent.egg-info/
--rw-r--r--   0 lan        (501) staff       (20)      462 2024-05-18 15:38:05.000000 tinyagent-0.1.0/tinyagent.egg-info/PKG-INFO
--rw-r--r--   0 lan        (501) staff       (20)      700 2024-05-18 15:38:05.000000 tinyagent-0.1.0/tinyagent.egg-info/SOURCES.txt
--rw-r--r--   0 lan        (501) staff       (20)        1 2024-05-18 15:38:05.000000 tinyagent-0.1.0/tinyagent.egg-info/dependency_links.txt
--rw-r--r--   0 lan        (501) staff       (20)       33 2024-05-18 15:38:05.000000 tinyagent-0.1.0/tinyagent.egg-info/requires.txt
--rw-r--r--   0 lan        (501) staff       (20)       10 2024-05-18 15:38:05.000000 tinyagent-0.1.0/tinyagent.egg-info/top_level.txt
+drwxr-xr-x   0 lan        (501) wheel        (0)        0 2024-05-18 16:24:26.765694 tinyagent-0.1.1/
+-rw-r--r--   0 lan        (501) wheel        (0)      789 2024-05-18 15:22:41.000000 tinyagent-0.1.1/.gitignore
+-rw-r--r--   0 lan        (501) wheel        (0)     1069 2024-05-18 16:24:07.000000 tinyagent-0.1.1/LICENSE
+-rw-r--r--   0 lan        (501) wheel        (0)      462 2024-05-18 16:24:26.765558 tinyagent-0.1.1/PKG-INFO
+-rw-r--r--   0 lan        (501) wheel        (0)       83 2024-05-18 15:22:41.000000 tinyagent-0.1.1/README.md
+-rw-r--r--   0 lan        (501) wheel        (0)    32102 2024-05-18 15:22:41.000000 tinyagent-0.1.1/poetry.lock
+-rw-r--r--   0 lan        (501) wheel        (0)      303 2024-05-18 16:24:07.000000 tinyagent-0.1.1/pyproject.toml
+-rw-r--r--   0 lan        (501) wheel        (0)       38 2024-05-18 16:24:26.765727 tinyagent-0.1.1/setup.cfg
+-rw-r--r--   0 lan        (501) wheel        (0)      589 2024-05-18 16:24:07.000000 tinyagent-0.1.1/setup.py
+drwxr-xr-x   0 lan        (501) wheel        (0)        0 2024-05-18 16:24:26.762265 tinyagent-0.1.1/tests/
+drwxr-xr-x   0 lan        (501) wheel        (0)        0 2024-05-18 16:24:26.762404 tinyagent-0.1.1/tests/resources/
+-rw-r--r--   0 lan        (501) wheel        (0)      785 2024-05-18 15:22:41.000000 tinyagent-0.1.1/tests/resources/test.jpg
+-rw-r--r--   0 lan        (501) wheel        (0)     1987 2024-05-18 15:22:41.000000 tinyagent-0.1.1/tests/test_claude.py
+-rw-r--r--   0 lan        (501) wheel        (0)     1991 2024-05-18 15:22:41.000000 tinyagent-0.1.1/tests/test_gpt.py
+-rw-r--r--   0 lan        (501) wheel        (0)     1018 2024-05-18 15:22:41.000000 tinyagent-0.1.1/tests/test_tool.py
+drwxr-xr-x   0 lan        (501) wheel        (0)        0 2024-05-18 16:24:26.762528 tinyagent-0.1.1/tinyagent/
+-rw-r--r--   0 lan        (501) wheel        (0)      562 2024-05-18 16:24:07.000000 tinyagent-0.1.1/tinyagent/__init__.py
+drwxr-xr-x   0 lan        (501) wheel        (0)        0 2024-05-18 16:24:26.763881 tinyagent-0.1.1/tinyagent/agent/
+-rw-r--r--   0 lan        (501) wheel        (0)      385 2024-05-18 15:22:41.000000 tinyagent-0.1.1/tinyagent/agent/__init__.py
+-rw-r--r--   0 lan        (501) wheel        (0)     4114 2024-05-18 15:22:41.000000 tinyagent-0.1.1/tinyagent/agent/base.py
+drwxr-xr-x   0 lan        (501) wheel        (0)        0 2024-05-18 16:24:26.764229 tinyagent-0.1.1/tinyagent/agent/claude/
+-rw-r--r--   0 lan        (501) wheel        (0)        0 2024-05-18 16:24:07.000000 tinyagent-0.1.1/tinyagent/agent/claude/__init__..py
+-rw-r--r--   0 lan        (501) wheel        (0)     9002 2024-05-18 15:22:41.000000 tinyagent-0.1.1/tinyagent/agent/claude/agent.py
+-rw-r--r--   0 lan        (501) wheel        (0)     2333 2024-05-18 15:22:41.000000 tinyagent-0.1.1/tinyagent/agent/claude/client.py
+drwxr-xr-x   0 lan        (501) wheel        (0)        0 2024-05-18 16:24:26.764948 tinyagent-0.1.1/tinyagent/agent/gpt/
+-rw-r--r--   0 lan        (501) wheel        (0)        0 2024-05-18 16:24:07.000000 tinyagent-0.1.1/tinyagent/agent/gpt/__init__.py
+-rw-r--r--   0 lan        (501) wheel        (0)     8668 2024-05-18 16:24:07.000000 tinyagent-0.1.1/tinyagent/agent/gpt/agent.py
+-rw-r--r--   0 lan        (501) wheel        (0)     2371 2024-05-18 16:24:07.000000 tinyagent-0.1.1/tinyagent/agent/gpt/client.py
+-rw-r--r--   0 lan        (501) wheel        (0)     2250 2024-05-18 15:22:41.000000 tinyagent-0.1.1/tinyagent/agent/schema.py
+-rw-r--r--   0 lan        (501) wheel        (0)     2328 2024-05-18 15:22:41.000000 tinyagent-0.1.1/tinyagent/agent/tools.py
+-rw-r--r--   0 lan        (501) wheel        (0)      191 2024-05-18 15:22:41.000000 tinyagent-0.1.1/tinyagent/agent/utils.py
+drwxr-xr-x   0 lan        (501) wheel        (0)        0 2024-05-18 16:24:26.765377 tinyagent-0.1.1/tinyagent/common/
+-rw-r--r--   0 lan        (501) wheel        (0)       73 2024-05-18 15:22:41.000000 tinyagent-0.1.1/tinyagent/common/__init__.py
+-rw-r--r--   0 lan        (501) wheel        (0)      358 2024-05-18 15:22:41.000000 tinyagent-0.1.1/tinyagent/common/event.py
+-rw-r--r--   0 lan        (501) wheel        (0)      107 2024-05-18 15:22:41.000000 tinyagent-0.1.1/tinyagent/common/time.py
+drwxr-xr-x   0 lan        (501) wheel        (0)        0 2024-05-18 16:24:26.763165 tinyagent-0.1.1/tinyagent.egg-info/
+-rw-r--r--   0 lan        (501) wheel        (0)      462 2024-05-18 16:24:26.000000 tinyagent-0.1.1/tinyagent.egg-info/PKG-INFO
+-rw-r--r--   0 lan        (501) wheel        (0)      733 2024-05-18 16:24:26.000000 tinyagent-0.1.1/tinyagent.egg-info/SOURCES.txt
+-rw-r--r--   0 lan        (501) wheel        (0)        1 2024-05-18 16:24:26.000000 tinyagent-0.1.1/tinyagent.egg-info/dependency_links.txt
+-rw-r--r--   0 lan        (501) wheel        (0)       33 2024-05-18 16:24:26.000000 tinyagent-0.1.1/tinyagent.egg-info/requires.txt
+-rw-r--r--   0 lan        (501) wheel        (0)       10 2024-05-18 16:24:26.000000 tinyagent-0.1.1/tinyagent.egg-info/top_level.txt
```

### Comparing `tinyagent-0.1.0/.gitignore` & `tinyagent-0.1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `tinyagent-0.1.0/LICENSE` & `tinyagent-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `tinyagent-0.1.0/poetry.lock` & `tinyagent-0.1.1/poetry.lock`

 * *Files identical despite different names*

### Comparing `tinyagent-0.1.0/setup.py` & `tinyagent-0.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="tinyagent",
-    version="0.1.0",
+    version="0.1.1",
     author="y-lan",
     author_email="lanyuyang@gmail.com",
     description="A minimalistic agent framework",
     long_description=open("README.md").read(),
     url="https://github.com/y-lan/tinyagent",
     packages=find_packages(),
     install_requires=["pydantic>=2.7.1", "requests>=2.31.0"],
```

### Comparing `tinyagent-0.1.0/tests/resources/test.jpg` & `tinyagent-0.1.1/tests/resources/test.jpg`

 * *Files identical despite different names*

### Comparing `tinyagent-0.1.0/tests/test_claude.py` & `tinyagent-0.1.1/tests/test_claude.py`

 * *Files identical despite different names*

### Comparing `tinyagent-0.1.0/tests/test_gpt.py` & `tinyagent-0.1.1/tests/test_gpt.py`

 * *Files identical despite different names*

### Comparing `tinyagent-0.1.0/tests/test_tool.py` & `tinyagent-0.1.1/tests/test_tool.py`

 * *Files identical despite different names*

### Comparing `tinyagent-0.1.0/tinyagent/__init__.py` & `tinyagent-0.1.1/tinyagent/__init__.py`

 * *Files identical despite different names*

### Comparing `tinyagent-0.1.0/tinyagent/agent/base.py` & `tinyagent-0.1.1/tinyagent/agent/base.py`

 * *Files identical despite different names*

### Comparing `tinyagent-0.1.0/tinyagent/agent/claude/agent.py` & `tinyagent-0.1.1/tinyagent/agent/claude/agent.py`

 * *Files identical despite different names*

### Comparing `tinyagent-0.1.0/tinyagent/agent/claude/client.py` & `tinyagent-0.1.1/tinyagent/agent/claude/client.py`

 * *Files identical despite different names*

### Comparing `tinyagent-0.1.0/tinyagent/agent/gpt/agent.py` & `tinyagent-0.1.1/tinyagent/agent/gpt/agent.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,10 @@
 import base64
 import json
-import logging
 import os
-import time
 import urllib
 
 from pydantic import BaseModel, ConfigDict
 
 from tinyagent.agent.base import BaseAgent
 from tinyagent.agent.gpt.client import OpenAIChatResponse, OpenAIClient
 from tinyagent.agent.schema import (
@@ -15,15 +13,15 @@
     ChatResponse,
     Message,
     Role,
     TextContent,
     TokenUsage,
     Tool,
 )
-from tinyagent.agent.tools import CalculatorTool, build_function_signature
+from tinyagent.agent.tools import build_function_signature
 from tinyagent.agent.utils import replace_magic_placeholders
 
 
 def _create_image_content(image_path):
     parsed = urllib.parse.urlparse(image_path)
 
     if parsed.scheme in ("http", "https"):
@@ -221,14 +219,17 @@
             temperature=temperature or self.config.temperature,
             frequency_penalty=self.config.frequency_penalty,
             top_p=self.config.top_p,
             seed=self.config.seed,
             stream=self.config.stream or stream,
         )
 
+        if self.config.json_output:
+            params["response_format"] = {"type": "json_object"}
+
         if params["stream"]:
             params["stream_options"] = dict(include_usage=True)
 
         if self.config.use_tools and self.tools:
             tools = [build_function_signature(tool) for tool in self.tools.values()]
             params["tools"] = tools
             params["tool_choice"] = "auto"
```

### Comparing `tinyagent-0.1.0/tinyagent/agent/gpt/client.py` & `tinyagent-0.1.1/tinyagent/agent/gpt/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 import os
 import time
 from typing import Optional
 from pydantic import BaseModel
 
 import requests
 
-from tinyagent.agent.schema import Message, Role
 
 
 class OpenAIChatResponse(BaseModel):
     id: str
     object: str
     created: int
     model: str
```

### Comparing `tinyagent-0.1.0/tinyagent/agent/schema.py` & `tinyagent-0.1.1/tinyagent/agent/schema.py`

 * *Files identical despite different names*

### Comparing `tinyagent-0.1.0/tinyagent/agent/tools.py` & `tinyagent-0.1.1/tinyagent/agent/tools.py`

 * *Files identical despite different names*

### Comparing `tinyagent-0.1.0/tinyagent.egg-info/SOURCES.txt` & `tinyagent-0.1.1/tinyagent.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -15,15 +15,16 @@
 tinyagent.egg-info/requires.txt
 tinyagent.egg-info/top_level.txt
 tinyagent/agent/__init__.py
 tinyagent/agent/base.py
 tinyagent/agent/schema.py
 tinyagent/agent/tools.py
 tinyagent/agent/utils.py
-tinyagent/agent/claude/__init_..py
+tinyagent/agent/claude/__init__..py
 tinyagent/agent/claude/agent.py
 tinyagent/agent/claude/client.py
+tinyagent/agent/gpt/__init__.py
 tinyagent/agent/gpt/agent.py
 tinyagent/agent/gpt/client.py
 tinyagent/common/__init__.py
 tinyagent/common/event.py
 tinyagent/common/time.py
```

