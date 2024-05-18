# Comparing `tmp/textlong-0.1.2.tar.gz` & `tmp/textlong-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "textlong-0.1.2.tar", max compression
+gzip compressed data, was "textlong-0.1.3.tar", max compression
```

## Comparing `textlong-0.1.2.tar` & `textlong-0.1.3.tar`

### file list

```diff
@@ -1,31 +1,31 @@
--rw-r--r--   0        0        0     1066 2024-05-17 12:44:59.600013 textlong-0.1.2/LICENSE
--rw-r--r--   0        0        0      938 2024-05-17 12:53:58.250212 textlong-0.1.2/README.md
--rw-r--r--   0        0        0      880 2024-05-17 15:02:21.088990 textlong-0.1.2/pyproject.toml
--rw-r--r--   0        0        0        0 2024-05-17 12:44:59.600533 textlong-0.1.2/textlong/.pypirc
--rw-r--r--   0        0        0      848 2024-05-17 14:19:13.587368 textlong-0.1.2/textlong/__init__.py
--rw-r--r--   0        0        0       22 2024-05-17 15:02:16.813315 textlong-0.1.2/textlong/__version__.py
--rw-r--r--   0        0        0        0 2024-05-17 12:44:59.601026 textlong-0.1.2/textlong/agents/__init__.py
--rw-r--r--   0        0        0     2722 2024-05-17 12:44:59.601163 textlong-0.1.2/textlong/agents/base.py
--rw-r--r--   0        0        0     7036 2024-05-17 12:44:59.601410 textlong-0.1.2/textlong/agents/prompt.py
--rw-r--r--   0        0        0     4988 2024-05-17 12:44:59.601632 textlong-0.1.2/textlong/ai.py
--rw-r--r--   0        0        0     6780 2024-05-17 12:44:59.601940 textlong-0.1.2/textlong/base.py
--rw-r--r--   0        0        0     2442 2024-05-17 12:44:59.602176 textlong-0.1.2/textlong/command.py
--rw-r--r--   0        0        0        0 2024-05-17 12:44:59.602426 textlong-0.1.2/textlong/document_loaders/__init__.py
--rw-r--r--   0        0        0     8955 2024-05-17 12:44:59.602748 textlong-0.1.2/textlong/document_loaders/base.py
--rw-r--r--   0        0        0       57 2024-05-17 12:44:59.602930 textlong-0.1.2/textlong/langgraph/__init__.py
--rw-r--r--   0        0        0     5269 2024-05-17 12:44:59.603160 textlong-0.1.2/textlong/langgraph/tools_calling.py
--rw-r--r--   0        0        0       77 2024-05-17 12:44:59.603326 textlong-0.1.2/textlong/memory/__init__.py
--rw-r--r--   0        0        0    10213 2024-05-17 12:44:59.603589 textlong-0.1.2/textlong/memory/base.py
--rw-r--r--   0        0        0     3839 2024-05-17 12:44:59.603829 textlong-0.1.2/textlong/memory/history.py
--rw-r--r--   0        0        0     3131 2024-05-17 12:44:59.603975 textlong-0.1.2/textlong/memory/memory_manager.py
--rw-r--r--   0        0        0     9410 2024-05-17 14:58:44.781290 textlong-0.1.2/textlong/node.py
--rw-r--r--   0        0        0      936 2024-05-17 12:44:59.604351 textlong-0.1.2/textlong/prompts/main.py
--rw-r--r--   0        0        0     3314 2024-05-17 12:44:59.604491 textlong-0.1.2/textlong/prompts/task_prompt.py
--rw-r--r--   0        0        0      385 2024-05-17 12:44:59.604603 textlong-0.1.2/textlong/prompts/translate.py
--rw-r--r--   0        0        0        0 2024-05-17 12:44:59.604711 textlong-0.1.2/textlong/retrievers/__init__.py
--rw-r--r--   0        0        0     2999 2024-05-17 12:44:59.604917 textlong-0.1.2/textlong/retrievers/base.py
--rw-r--r--   0        0        0     3141 2024-05-17 13:56:55.783580 textlong-0.1.2/textlong/serialize.py
--rw-r--r--   0        0        0     1949 2024-05-17 12:44:59.605319 textlong-0.1.2/textlong/state.py
--rw-r--r--   0        0        0     2406 2024-05-17 12:44:59.605464 textlong-0.1.2/textlong/task.py
--rw-r--r--   0        0        0     2003 2024-05-17 15:01:02.849565 textlong-0.1.2/textlong/tree.py
--rw-r--r--   0        0        0     1839 1970-01-01 00:00:00.000000 textlong-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1066 2024-05-17 12:44:59.600013 textlong-0.1.3/LICENSE
+-rw-r--r--   0        0        0     1072 2024-05-17 15:09:50.760904 textlong-0.1.3/README.md
+-rw-r--r--   0        0        0      880 2024-05-17 15:05:28.320169 textlong-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-17 12:44:59.600533 textlong-0.1.3/textlong/.pypirc
+-rw-r--r--   0        0        0      848 2024-05-17 14:19:13.587368 textlong-0.1.3/textlong/__init__.py
+-rw-r--r--   0        0        0       22 2024-05-17 15:05:01.865502 textlong-0.1.3/textlong/__version__.py
+-rw-r--r--   0        0        0        0 2024-05-17 12:44:59.601026 textlong-0.1.3/textlong/agents/__init__.py
+-rw-r--r--   0        0        0     2722 2024-05-17 12:44:59.601163 textlong-0.1.3/textlong/agents/base.py
+-rw-r--r--   0        0        0     7036 2024-05-17 12:44:59.601410 textlong-0.1.3/textlong/agents/prompt.py
+-rw-r--r--   0        0        0     4988 2024-05-17 12:44:59.601632 textlong-0.1.3/textlong/ai.py
+-rw-r--r--   0        0        0     6780 2024-05-17 12:44:59.601940 textlong-0.1.3/textlong/base.py
+-rw-r--r--   0        0        0     2442 2024-05-17 12:44:59.602176 textlong-0.1.3/textlong/command.py
+-rw-r--r--   0        0        0        0 2024-05-17 12:44:59.602426 textlong-0.1.3/textlong/document_loaders/__init__.py
+-rw-r--r--   0        0        0     8955 2024-05-17 12:44:59.602748 textlong-0.1.3/textlong/document_loaders/base.py
+-rw-r--r--   0        0        0       57 2024-05-17 12:44:59.602930 textlong-0.1.3/textlong/langgraph/__init__.py
+-rw-r--r--   0        0        0     5269 2024-05-17 12:44:59.603160 textlong-0.1.3/textlong/langgraph/tools_calling.py
+-rw-r--r--   0        0        0       77 2024-05-17 12:44:59.603326 textlong-0.1.3/textlong/memory/__init__.py
+-rw-r--r--   0        0        0    10213 2024-05-17 12:44:59.603589 textlong-0.1.3/textlong/memory/base.py
+-rw-r--r--   0        0        0     3839 2024-05-17 12:44:59.603829 textlong-0.1.3/textlong/memory/history.py
+-rw-r--r--   0        0        0     3131 2024-05-17 12:44:59.603975 textlong-0.1.3/textlong/memory/memory_manager.py
+-rw-r--r--   0        0        0     9410 2024-05-17 14:58:44.781290 textlong-0.1.3/textlong/node.py
+-rw-r--r--   0        0        0      936 2024-05-17 12:44:59.604351 textlong-0.1.3/textlong/prompts/main.py
+-rw-r--r--   0        0        0     3314 2024-05-17 12:44:59.604491 textlong-0.1.3/textlong/prompts/task_prompt.py
+-rw-r--r--   0        0        0      385 2024-05-17 12:44:59.604603 textlong-0.1.3/textlong/prompts/translate.py
+-rw-r--r--   0        0        0        0 2024-05-17 12:44:59.604711 textlong-0.1.3/textlong/retrievers/__init__.py
+-rw-r--r--   0        0        0     2999 2024-05-17 12:44:59.604917 textlong-0.1.3/textlong/retrievers/base.py
+-rw-r--r--   0        0        0     3141 2024-05-17 13:56:55.783580 textlong-0.1.3/textlong/serialize.py
+-rw-r--r--   0        0        0     1949 2024-05-17 12:44:59.605319 textlong-0.1.3/textlong/state.py
+-rw-r--r--   0        0        0     2406 2024-05-17 12:44:59.605464 textlong-0.1.3/textlong/task.py
+-rw-r--r--   0        0        0     2003 2024-05-17 15:01:02.849565 textlong-0.1.3/textlong/tree.py
+-rw-r--r--   0        0        0     1973 1970-01-01 00:00:00.000000 textlong-0.1.3/PKG-INFO
```

### Comparing `textlong-0.1.2/LICENSE` & `textlong-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `textlong-0.1.2/README.md` & `textlong-0.1.3/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -16,24 +16,30 @@
 ```
 
 ## 二、结构化长文生成能力
 
 `textlong` 中提供如下结构化长文档的创作模式：
 
 - 一键直出：输入写作要求后，由AI直接创作
-- （其他模式正在研发中，请参考路线图说明 [路线图](https://github.com/arcstep/textlong/blob/main/roadmap.md)）
+- （其他模式正在研发中，请参考[路线图](https://github.com/arcstep/textlong/blob/main/roadmap.md)）
 
-**应用示范：**
+**使用示例：**
 
 ```python
 import os
 from dotenv import load_dotenv, find_dotenv
 load_dotenv(find_dotenv(), override=True)
 
 from textlong import WritingTask
 
 # 使用默认的智谱AI推理
 t = WritingTask()
-t.auto_write("task 给好基友写一封信, 1800字")
+t.auto_write("task 给好基友写一封信, 1800字，分4段就行")
+```
 
-t.invoke("")
+之后你可以查看生成的成果：
+```python
+# 查看创作大纲
+t.invoke("outlines")['reply']
+# 查看文本
+t.invoke("texts")['reply']
 ```
```

### Comparing `textlong-0.1.2/pyproject.toml` & `textlong-0.1.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "textlong"
-version = "0.1.2"
+version = "0.1.3"
 description = "A framework designed to produce long-texts with GPT or other large language models."
 authors = ["arcstep <43801@qq.com>"]
 homepage = "https://github.com/arcstep/textlong"
 repository = "https://github.com/arcstep/textlong.git"
 license = "MIT"
 readme = "README.md"
```

### Comparing `textlong-0.1.2/textlong/__init__.py` & `textlong-0.1.3/textlong/__init__.py`

 * *Files identical despite different names*

### Comparing `textlong-0.1.2/textlong/agents/base.py` & `textlong-0.1.3/textlong/agents/base.py`

 * *Files identical despite different names*

### Comparing `textlong-0.1.2/textlong/agents/prompt.py` & `textlong-0.1.3/textlong/agents/prompt.py`

 * *Files identical despite different names*

### Comparing `textlong-0.1.2/textlong/ai.py` & `textlong-0.1.3/textlong/ai.py`

 * *Files identical despite different names*

### Comparing `textlong-0.1.2/textlong/base.py` & `textlong-0.1.3/textlong/base.py`

 * *Files identical despite different names*

### Comparing `textlong-0.1.2/textlong/command.py` & `textlong-0.1.3/textlong/command.py`

 * *Files identical despite different names*

### Comparing `textlong-0.1.2/textlong/document_loaders/base.py` & `textlong-0.1.3/textlong/document_loaders/base.py`

 * *Files identical despite different names*

### Comparing `textlong-0.1.2/textlong/langgraph/tools_calling.py` & `textlong-0.1.3/textlong/langgraph/tools_calling.py`

 * *Files identical despite different names*

### Comparing `textlong-0.1.2/textlong/memory/base.py` & `textlong-0.1.3/textlong/memory/base.py`

 * *Files identical despite different names*

### Comparing `textlong-0.1.2/textlong/memory/history.py` & `textlong-0.1.3/textlong/memory/history.py`

 * *Files identical despite different names*

### Comparing `textlong-0.1.2/textlong/memory/memory_manager.py` & `textlong-0.1.3/textlong/memory/memory_manager.py`

 * *Files identical despite different names*

### Comparing `textlong-0.1.2/textlong/node.py` & `textlong-0.1.3/textlong/node.py`

 * *Files identical despite different names*

### Comparing `textlong-0.1.2/textlong/prompts/main.py` & `textlong-0.1.3/textlong/prompts/main.py`

 * *Files identical despite different names*

### Comparing `textlong-0.1.2/textlong/prompts/task_prompt.py` & `textlong-0.1.3/textlong/prompts/task_prompt.py`

 * *Files identical despite different names*

### Comparing `textlong-0.1.2/textlong/retrievers/base.py` & `textlong-0.1.3/textlong/retrievers/base.py`

 * *Files identical despite different names*

### Comparing `textlong-0.1.2/textlong/serialize.py` & `textlong-0.1.3/textlong/serialize.py`

 * *Files identical despite different names*

### Comparing `textlong-0.1.2/textlong/state.py` & `textlong-0.1.3/textlong/state.py`

 * *Files identical despite different names*

### Comparing `textlong-0.1.2/textlong/task.py` & `textlong-0.1.3/textlong/task.py`

 * *Files identical despite different names*

### Comparing `textlong-0.1.2/textlong/tree.py` & `textlong-0.1.3/textlong/tree.py`

 * *Files identical despite different names*

### Comparing `textlong-0.1.2/PKG-INFO` & `textlong-0.1.3/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: textlong
-Version: 0.1.2
+Version: 0.1.3
 Summary: A framework designed to produce long-texts with GPT or other large language models.
 Home-page: https://github.com/arcstep/textlong
 License: MIT
 Author: arcstep
 Author-email: 43801@qq.com
 Requires-Python: >=3.9,<3.12
 Classifier: License :: OSI Approved :: MIT License
@@ -39,24 +39,30 @@
 ```
 
 ## 二、结构化长文生成能力
 
 `textlong` 中提供如下结构化长文档的创作模式：
 
 - 一键直出：输入写作要求后，由AI直接创作
-- （其他模式正在研发中，请参考路线图说明 [路线图](https://github.com/arcstep/textlong/blob/main/roadmap.md)）
+- （其他模式正在研发中，请参考[路线图](https://github.com/arcstep/textlong/blob/main/roadmap.md)）
 
-**应用示范：**
+**使用示例：**
 
 ```python
 import os
 from dotenv import load_dotenv, find_dotenv
 load_dotenv(find_dotenv(), override=True)
 
 from textlong import WritingTask
 
 # 使用默认的智谱AI推理
 t = WritingTask()
-t.auto_write("task 给好基友写一封信, 1800字")
+t.auto_write("task 给好基友写一封信, 1800字，分4段就行")
+```
 
-t.invoke("")
+之后你可以查看生成的成果：
+```python
+# 查看创作大纲
+t.invoke("outlines")['reply']
+# 查看文本
+t.invoke("texts")['reply']
 ```
```

