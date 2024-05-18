# Comparing `tmp/textlong-0.1.3.tar.gz` & `tmp/textlong-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "textlong-0.1.3.tar", max compression
+gzip compressed data, was "textlong-0.1.4.tar", max compression
```

## Comparing `textlong-0.1.3.tar` & `textlong-0.1.4.tar`

### file list

```diff
@@ -1,31 +1,34 @@
--rw-r--r--   0        0        0     1066 2024-05-17 12:44:59.600013 textlong-0.1.3/LICENSE
--rw-r--r--   0        0        0     1072 2024-05-17 15:09:50.760904 textlong-0.1.3/README.md
--rw-r--r--   0        0        0      880 2024-05-17 15:05:28.320169 textlong-0.1.3/pyproject.toml
--rw-r--r--   0        0        0        0 2024-05-17 12:44:59.600533 textlong-0.1.3/textlong/.pypirc
--rw-r--r--   0        0        0      848 2024-05-17 14:19:13.587368 textlong-0.1.3/textlong/__init__.py
--rw-r--r--   0        0        0       22 2024-05-17 15:05:01.865502 textlong-0.1.3/textlong/__version__.py
--rw-r--r--   0        0        0        0 2024-05-17 12:44:59.601026 textlong-0.1.3/textlong/agents/__init__.py
--rw-r--r--   0        0        0     2722 2024-05-17 12:44:59.601163 textlong-0.1.3/textlong/agents/base.py
--rw-r--r--   0        0        0     7036 2024-05-17 12:44:59.601410 textlong-0.1.3/textlong/agents/prompt.py
--rw-r--r--   0        0        0     4988 2024-05-17 12:44:59.601632 textlong-0.1.3/textlong/ai.py
--rw-r--r--   0        0        0     6780 2024-05-17 12:44:59.601940 textlong-0.1.3/textlong/base.py
--rw-r--r--   0        0        0     2442 2024-05-17 12:44:59.602176 textlong-0.1.3/textlong/command.py
--rw-r--r--   0        0        0        0 2024-05-17 12:44:59.602426 textlong-0.1.3/textlong/document_loaders/__init__.py
--rw-r--r--   0        0        0     8955 2024-05-17 12:44:59.602748 textlong-0.1.3/textlong/document_loaders/base.py
--rw-r--r--   0        0        0       57 2024-05-17 12:44:59.602930 textlong-0.1.3/textlong/langgraph/__init__.py
--rw-r--r--   0        0        0     5269 2024-05-17 12:44:59.603160 textlong-0.1.3/textlong/langgraph/tools_calling.py
--rw-r--r--   0        0        0       77 2024-05-17 12:44:59.603326 textlong-0.1.3/textlong/memory/__init__.py
--rw-r--r--   0        0        0    10213 2024-05-17 12:44:59.603589 textlong-0.1.3/textlong/memory/base.py
--rw-r--r--   0        0        0     3839 2024-05-17 12:44:59.603829 textlong-0.1.3/textlong/memory/history.py
--rw-r--r--   0        0        0     3131 2024-05-17 12:44:59.603975 textlong-0.1.3/textlong/memory/memory_manager.py
--rw-r--r--   0        0        0     9410 2024-05-17 14:58:44.781290 textlong-0.1.3/textlong/node.py
--rw-r--r--   0        0        0      936 2024-05-17 12:44:59.604351 textlong-0.1.3/textlong/prompts/main.py
--rw-r--r--   0        0        0     3314 2024-05-17 12:44:59.604491 textlong-0.1.3/textlong/prompts/task_prompt.py
--rw-r--r--   0        0        0      385 2024-05-17 12:44:59.604603 textlong-0.1.3/textlong/prompts/translate.py
--rw-r--r--   0        0        0        0 2024-05-17 12:44:59.604711 textlong-0.1.3/textlong/retrievers/__init__.py
--rw-r--r--   0        0        0     2999 2024-05-17 12:44:59.604917 textlong-0.1.3/textlong/retrievers/base.py
--rw-r--r--   0        0        0     3141 2024-05-17 13:56:55.783580 textlong-0.1.3/textlong/serialize.py
--rw-r--r--   0        0        0     1949 2024-05-17 12:44:59.605319 textlong-0.1.3/textlong/state.py
--rw-r--r--   0        0        0     2406 2024-05-17 12:44:59.605464 textlong-0.1.3/textlong/task.py
--rw-r--r--   0        0        0     2003 2024-05-17 15:01:02.849565 textlong-0.1.3/textlong/tree.py
--rw-r--r--   0        0        0     1973 1970-01-01 00:00:00.000000 textlong-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1066 2024-05-17 12:44:59.600013 textlong-0.1.4/LICENSE
+-rw-r--r--   0        0        0     1592 2024-05-18 06:03:25.955655 textlong-0.1.4/README.md
+-rw-r--r--   0        0        0      880 2024-05-18 06:06:21.730057 textlong-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-17 12:44:59.600533 textlong-0.1.4/textlong/.pypirc
+-rw-r--r--   0        0        0      340 2024-05-18 02:21:59.329892 textlong-0.1.4/textlong/__init__.py
+-rw-r--r--   0        0        0       22 2024-05-18 06:06:13.007213 textlong-0.1.4/textlong/__version__.py
+-rw-r--r--   0        0        0        0 2024-05-17 12:44:59.601026 textlong-0.1.4/textlong/agents/__init__.py
+-rw-r--r--   0        0        0     2722 2024-05-17 12:44:59.601163 textlong-0.1.4/textlong/agents/base.py
+-rw-r--r--   0        0        0     7036 2024-05-17 12:44:59.601410 textlong-0.1.4/textlong/agents/prompt.py
+-rw-r--r--   0        0        0     2370 2024-05-18 02:24:33.016543 textlong-0.1.4/textlong/ai.py
+-rw-r--r--   0        0        0     6780 2024-05-17 12:44:59.601940 textlong-0.1.4/textlong/base.py
+-rw-r--r--   0        0        0     2511 2024-05-18 03:48:42.318437 textlong-0.1.4/textlong/command.py
+-rw-r--r--   0        0        0        0 2024-05-18 02:40:06.723540 textlong-0.1.4/textlong/docs/__init__.py
+-rw-r--r--   0        0        0     3557 2024-05-18 03:57:52.669524 textlong-0.1.4/textlong/docs/writing_help.py
+-rw-r--r--   0        0        0        0 2024-05-17 12:44:59.602426 textlong-0.1.4/textlong/document_loaders/__init__.py
+-rw-r--r--   0        0        0     8955 2024-05-17 12:44:59.602748 textlong-0.1.4/textlong/document_loaders/base.py
+-rw-r--r--   0        0        0       57 2024-05-17 12:44:59.602930 textlong-0.1.4/textlong/langgraph/__init__.py
+-rw-r--r--   0        0        0     5269 2024-05-17 12:44:59.603160 textlong-0.1.4/textlong/langgraph/tools_calling.py
+-rw-r--r--   0        0        0       77 2024-05-17 12:44:59.603326 textlong-0.1.4/textlong/memory/__init__.py
+-rw-r--r--   0        0        0    10213 2024-05-17 12:44:59.603589 textlong-0.1.4/textlong/memory/base.py
+-rw-r--r--   0        0        0     3839 2024-05-17 12:44:59.603829 textlong-0.1.4/textlong/memory/history.py
+-rw-r--r--   0        0        0     3131 2024-05-17 12:44:59.603975 textlong-0.1.4/textlong/memory/memory_manager.py
+-rw-r--r--   0        0        0     9577 2024-05-18 02:23:07.746469 textlong-0.1.4/textlong/node.py
+-rw-r--r--   0        0        0      121 2024-05-18 02:19:48.770966 textlong-0.1.4/textlong/prompts/__init__.py
+-rw-r--r--   0        0        0      936 2024-05-17 12:44:59.604351 textlong-0.1.4/textlong/prompts/main.py
+-rw-r--r--   0        0        0      385 2024-05-17 12:44:59.604603 textlong-0.1.4/textlong/prompts/translate.py
+-rw-r--r--   0        0        0     6442 2024-05-18 03:59:57.327185 textlong-0.1.4/textlong/prompts/writing_prompt.py
+-rw-r--r--   0        0        0        0 2024-05-17 12:44:59.604711 textlong-0.1.4/textlong/retrievers/__init__.py
+-rw-r--r--   0        0        0     2999 2024-05-17 12:44:59.604917 textlong-0.1.4/textlong/retrievers/base.py
+-rw-r--r--   0        0        0     3139 2024-05-18 01:20:13.147651 textlong-0.1.4/textlong/serialize.py
+-rw-r--r--   0        0        0     1949 2024-05-17 12:44:59.605319 textlong-0.1.4/textlong/state.py
+-rw-r--r--   0        0        0     2026 2024-05-17 15:18:37.918040 textlong-0.1.4/textlong/tree.py
+-rw-r--r--   0        0        0     2438 2024-05-18 03:33:05.691759 textlong-0.1.4/textlong/writing.py
+-rw-r--r--   0        0        0     2493 1970-01-01 00:00:00.000000 textlong-0.1.4/PKG-INFO
```

### Comparing `textlong-0.1.3/LICENSE` & `textlong-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `textlong-0.1.3/pyproject.toml` & `textlong-0.1.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "textlong"
-version = "0.1.3"
+version = "0.1.4"
 description = "A framework designed to produce long-texts with GPT or other large language models."
 authors = ["arcstep <43801@qq.com>"]
 homepage = "https://github.com/arcstep/textlong"
 repository = "https://github.com/arcstep/textlong.git"
 license = "MIT"
 readme = "README.md"
```

### Comparing `textlong-0.1.3/textlong/agents/base.py` & `textlong-0.1.4/textlong/agents/base.py`

 * *Files identical despite different names*

### Comparing `textlong-0.1.3/textlong/agents/prompt.py` & `textlong-0.1.4/textlong/agents/prompt.py`

 * *Files identical despite different names*

### Comparing `textlong-0.1.3/textlong/base.py` & `textlong-0.1.4/textlong/base.py`

 * *Files identical despite different names*

### Comparing `textlong-0.1.3/textlong/command.py` & `textlong-0.1.4/textlong/command.py`

 * *Files 6% similar despite different names*

```diff
@@ -24,15 +24,15 @@
         """
         从用户输入中解析指令后，直接执行。
         通常，你应该通过重载call函数来定义执行逻辑，再通过invoke函数调用。
         """
         resp = self.parse(user_said)
 
         # 打印执行的指令
-        print(resp)
+        # print(resp)
 
         if resp and resp['command'] in self.commands:
             resp['reply'] = self.call(**resp)
         else:
             NotImplementedError("用户输入不支持：", resp)            
 
         return resp
@@ -62,12 +62,13 @@
             return {"id": None, "command": None, "args": None}
 
         pattern = r'^\s*(' + '|'.join(self.commands) + r')?\s*(.*)$'
         match = re.match(pattern, user_said, re.IGNORECASE)
  
         if match:
             command, args = match.groups()
+            command = command.strip().lower() if command else None
             command = command if command and len(command) > 0 else self.default_command
             args = args if args and len(args) > 0 else None
             return {"command": command, "args": args}
         else:
             return {"command": self.default_command, "args": None}
```

### Comparing `textlong-0.1.3/textlong/document_loaders/base.py` & `textlong-0.1.4/textlong/document_loaders/base.py`

 * *Files identical despite different names*

### Comparing `textlong-0.1.3/textlong/langgraph/tools_calling.py` & `textlong-0.1.4/textlong/langgraph/tools_calling.py`

 * *Files identical despite different names*

### Comparing `textlong-0.1.3/textlong/memory/base.py` & `textlong-0.1.4/textlong/memory/base.py`

 * *Files identical despite different names*

### Comparing `textlong-0.1.3/textlong/memory/history.py` & `textlong-0.1.4/textlong/memory/history.py`

 * *Files identical despite different names*

### Comparing `textlong-0.1.3/textlong/memory/memory_manager.py` & `textlong-0.1.4/textlong/memory/memory_manager.py`

 * *Files identical despite different names*

### Comparing `textlong-0.1.3/textlong/node.py` & `textlong-0.1.4/textlong/node.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,19 @@
 from typing import Any, Dict, Iterator, List, Optional, Union
 from langchain_core.runnables import Runnable
 from langchain.prompts import ChatPromptTemplate, MessagesPlaceholder
 from langchain_core.output_parsers import JsonOutputParser
 from .serialize import ContentSerialize
 from .state import ContentState
 from .command import BaseCommand
+from .prompts import (
+    create_writing_help_prompt,
+    create_writing_init_prompt,
+    create_writing_todo_prompt,
+)
 from .ai import BaseAI
 import datetime
 import random
 
 class ContentNode(ContentState, ContentSerialize, BaseCommand):
     """
     树形结构的内容存储节点，段落内容保存在叶子节点，而提纲保存在children的列表中。
@@ -21,14 +26,15 @@
         words_advice: int=None,
         title: str=None,
         howto: str=None,
         summarise: str=None,
         text: str=None,
         last_ai_reply_json: Dict[str, Any]={},
         is_draft=False,
+        llm=None,
         **kwargs,
     ):
         ContentState.__init__(self)
         ContentSerialize.__init__(self, **kwargs)
 
         self.type = type
 
@@ -43,15 +49,15 @@
         # 段落
         self.summarise = summarise
         self.text = text
 
         # 最后的AI回复
         self.last_ai_reply_json = last_ai_reply_json
         self.is_draft: bool = is_draft
-        self.ai = BaseAI()
+        self.ai = BaseAI(llm)
 
     howto_commands = ["title", "words_advice", "howto"]
     result_commands = ["summarise", "text"]
     state_commands = ["state", "memory", "ok", "todo", "modi", "task"]
 
     # inherit
     @property
@@ -104,42 +110,41 @@
         return "help"
 
     def help_ai(self, task: str=None):
         """向AI询问，获得生成结果"""
 
         default_task = "有哪些命令可以使用？"
 
-        chain = self.ai.get_chain()
-        chat = self.ai.ask_ai(task or default_task, chain, return_json=False)
+        prompt = create_writing_help_prompt()
+        chat = self.ai.ask_ai(task or default_task, prompt, return_json=False)
 
         return chat
 
     def ask_ai(self, task: str=None):
         """向AI询问，获得生成结果"""
 
         default_task = "请开始。"
 
         if self.state == "init":
-            prompt = self.ai.prompt_init()
+            prompt = create_writing_init_prompt()
 
         elif self.state == "todo":
-            prompt = self.ai.prompt_todo(
+            prompt = create_writing_todo_prompt(
                 title=self.title,
                 content_type=self.type,
                 words_limit=self.words_limit,
                 words_advice=self.words_advice,
                 howto=self.howto,
                 outline_exist=self.root.get_outlines()
             )
 
         else:
             raise NotImplementedError(f"<{self.id}> 对象在状态[{self.state}]没有指定提示语模板")
 
-        chain = self.ai.get_chain(prompt)
-        json = self.ai.ask_ai(task or default_task, chain, return_json=True)
+        json = self.ai.ask_ai(task or default_task, prompt, return_json=True)
         self.last_ai_reply_json = json
         self.is_draft = True
 
         return json
 
     # 设置提示语输入
     def _cmd_set_prop(self, k: str, v: str):
@@ -185,14 +190,15 @@
                         type=type,
                         title=title,
                         howto=howto,
                         words_advice=words_advice,
                         last_ai_reply_json=item,
                         is_draft=False,
                         item_class=ContentNode,
+                        llm=self.ai.llm,
                     )
                     node.edit()
 
             elif self.type == "paragraph":
                 self.reply_json_validator(self.last_ai_reply_json, ["内容摘要", "详细内容"])
                 self.summarise = self.last_ai_reply_json["内容摘要"]
                 self.text = self.last_ai_reply_json["详细内容"]
```

### Comparing `textlong-0.1.3/textlong/prompts/main.py` & `textlong-0.1.4/textlong/prompts/main.py`

 * *Files identical despite different names*

### Comparing `textlong-0.1.3/textlong/retrievers/base.py` & `textlong-0.1.4/textlong/retrievers/base.py`

 * *Files identical despite different names*

### Comparing `textlong-0.1.3/textlong/serialize.py` & `textlong-0.1.4/textlong/serialize.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 class ContentSerialize():
     """支持序列化的属性存储结构"""
 
     def __init__(
         self,
         project_id: str=None,
         index: int=0,
-        parent: "ContentSerialize" = None,
+        parent: "ContentSerialize"=None,
         **kwargs
     ):
         """
         初始化方法
         """
         self._project_id = project_id        
         self._index = index
```

### Comparing `textlong-0.1.3/textlong/state.py` & `textlong-0.1.4/textlong/state.py`

 * *Files identical despite different names*

### Comparing `textlong-0.1.3/textlong/task.py` & `textlong-0.1.4/textlong/writing.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,17 +3,17 @@
 from .command import BaseCommand
 
 class WritingTask(BaseCommand):
     """
     长文写作任务。
     """
 
-    def __init__(self):
+    def __init__(self, llm=None):
         self.human_input = lambda x=None : x if x != None else input("\n👤: ")
-        self.tree = ContentTree()
+        self.tree = ContentTree(llm=llm)
 
     # inherit
     @property
     def default_command(self) -> str:
         return self.tree.default_command
 
     # inherit
@@ -55,15 +55,15 @@
     def repl_write(self, user_said: str = None):
         """每一步都询问"""
 
         counter = 0
         max_steps = 1e3
 
         resp = self.invoke(user_said)
-        print(resp)
+        # print(resp)
 
         while(counter < max_steps):
             counter += 1
 
             if self.tree.todo_node.is_complete:
                 resp = self.invoke("todo")
                 if resp['reply']:
@@ -72,16 +72,16 @@
                 if self.tree.todo_node.state == "init":
                     self.invoke("ok")
 
                 if not self.tree.todo_node.is_draft:
                     self.invoke("task 请继续")
             
             n = self.tree.todo_node
-            print(f'<{n.id} #{n.state}> {n.title}')
-            print(self.commands)
+            print(f'<{n.id} #{n.state}> [Title: {n.title}]')
+            # print(self.commands)
 
             user_said = self.human_input()
             resp = self.invoke(user_said)
-            print(resp)
+            # print(resp)
             if not resp or resp['reply'] == '<QUIT>':
                 print("QUIT")
                 break
```

### Comparing `textlong-0.1.3/textlong/tree.py` & `textlong-0.1.4/textlong/tree.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,20 +3,21 @@
 from .command import BaseCommand
 
 class ContentTree(BaseCommand):
     """内容管理树。"""
 
     def __init__(
         self,
-        todo_node: Optional[ContentNode] = None,
+        todo_node: Optional[ContentNode]=None,
+        llm=None,
         **kwargs
     ):
         super().__init__(**kwargs)
 
-        self.todo_node = ContentNode() if todo_node == None else todo_node
+        self.todo_node = ContentNode(llm=llm) if todo_node == None else todo_node
 
     @property
     def root(self):
         return self.todo_node.root
 
     # inherit
     @property
```

### Comparing `textlong-0.1.3/PKG-INFO` & `textlong-0.1.4/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: textlong
-Version: 0.1.3
+Version: 0.1.4
 Summary: A framework designed to produce long-texts with GPT or other large language models.
 Home-page: https://github.com/arcstep/textlong
 License: MIT
 Author: arcstep
 Author-email: 43801@qq.com
 Requires-Python: >=3.9,<3.12
 Classifier: License :: OSI Approved :: MIT License
@@ -36,33 +36,62 @@
 或者使用 poetry 安装：
 ```
 poetry add textlong@latest
 ```
 
 ## 二、结构化长文生成能力
 
-`textlong` 中提供如下结构化长文档的创作模式：
+`textlong` 中提供如下创作工具：
 
-- 一键直出：输入写作要求后，由AI直接创作
-- （其他模式正在研发中，请参考[路线图](https://github.com/arcstep/textlong/blob/main/roadmap.md)）
+- `WritingTask`：用于生成结构化长文
 
-**使用示例：**
+**1. 加载环境变量：**
 
 ```python
-import os
 from dotenv import load_dotenv, find_dotenv
 load_dotenv(find_dotenv(), override=True)
+```
+
+**2. 创建`WritingTask`实例：**
 
+```python
 from textlong import WritingTask
+from langchain_openai import ChatOpenAI
+
+task = WritingTask(llm=ChatOpenAI())
+```
+
+**3. 使用`auto_write`方法自动生成一段长文：**
 
-# 使用默认的智谱AI推理
-t = WritingTask()
-t.auto_write("task 给好基友写一封信, 1800字，分4段就行")
+```python
+task.auto_write("task 给好基友写一封信, 1800字，分4段就行")
 ```
 
-之后你可以查看生成的成果：
+**4. 使用`repl_write`方法在进入循环控制台生成一段长文：**
+
+```python
+task.repl_write("task 给好基友写一封信, 1800字，分4段就行")
+
+## ...
+## 接下来，你可以一直输入 ok 指令确认生成的内容，获得与 auto_write 类似的效果
+```
+
+**5. 你可以查看生成的提纲（也可以在repl模式中输入 outlines）：**
+
 ```python
 # 查看创作大纲
-t.invoke("outlines")['reply']
-# 查看文本
-t.invoke("texts")['reply']
+task.invoke("outlines")['reply']
+```
+
+**6. 或者查看文字成果：**
+
+```python
+task.invoke("texts")['reply']
 ```
+
+**7. 使用`invoke`方法执行`help`指令，以获得帮助:**
+
+```python
+task.invoke("help 我在repl模式中还可以做什么？")
+```
+
+
```

