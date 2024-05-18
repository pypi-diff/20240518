# Comparing `tmp/devon_agent-0.1.7.tar.gz` & `tmp/devon_agent-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "devon_agent-0.1.7.tar", max compression
+gzip compressed data, was "devon_agent-0.1.8.tar", max compression
```

## Comparing `devon_agent-0.1.7.tar` & `devon_agent-0.1.8.tar`

### file list

```diff
@@ -1,46 +1,46 @@
--rw-r--r--   0        0        0    11357 2024-03-17 15:42:25.856965 devon_agent-0.1.7/LICENSE
--rw-r--r--   0        0        0     5840 2024-05-18 02:03:47.403799 devon_agent-0.1.7/README.md
--rw-r--r--   0        0        0      851 2024-05-18 02:03:47.410014 devon_agent-0.1.7/devon_agent/__main__.py
--rw-r--r--   0        0        0    11192 2024-05-17 21:36:14.554449 devon_agent-0.1.7/devon_agent/agent.py
--rw-r--r--   0        0        0     8999 2024-05-18 02:03:47.410538 devon_agent-0.1.7/devon_agent/agents/default/agent.py
--rw-r--r--   0        0        0     6648 2024-05-18 02:03:47.410905 devon_agent-0.1.7/devon_agent/agents/default/anthropic_prompts.py
--rw-r--r--   0        0        0     6841 2024-05-18 04:58:22.551556 devon_agent-0.1.7/devon_agent/agents/default/openai_prompts.py
--rw-r--r--   0        0        0     5405 2024-05-18 02:03:47.412052 devon_agent-0.1.7/devon_agent/agents/model.py
--rw-r--r--   0        0        0     7281 2024-05-18 02:03:47.412440 devon_agent-0.1.7/devon_agent/environment.py
--rw-r--r--   0        0        0    30089 2024-05-17 17:40:28.549419 devon_agent-0.1.7/devon_agent/environments/swebenchenv.py
--rw-r--r--   0        0        0     1247 2024-05-17 21:36:14.557332 devon_agent-0.1.7/devon_agent/event.py
--rw-r--r--   0        0        0     9464 2024-05-18 01:59:15.254179 devon_agent-0.1.7/devon_agent/experimental/dspyloop.py
--rw-r--r--   0        0        0     2800 2024-05-17 17:40:44.223838 devon_agent-0.1.7/devon_agent/model.py
--rw-r--r--   0        0        0    21113 2024-05-17 21:36:14.558749 devon_agent-0.1.7/devon_agent/prompt.py
--rw-r--r--   0        0        0     6317 2024-05-11 01:42:20.814775 devon_agent-0.1.7/devon_agent/retrieval/ast_extractor.py
--rw-r--r--   0        0        0      561 2024-05-11 00:35:58.937331 devon_agent-0.1.7/devon_agent/retrieval/ast_parser.py
--rw-r--r--   0        0        0     6430 2024-05-17 21:36:48.492247 devon_agent-0.1.7/devon_agent/retrieval/code_index.py
--rw-r--r--   0        0        0     7207 2024-05-17 21:36:48.492590 devon_agent-0.1.7/devon_agent/retrieval/codebase_graph.py
--rw-r--r--   0        0        0      913 2024-05-17 17:40:28.552873 devon_agent-0.1.7/devon_agent/retrieval/file_discovery.py
--rw-r--r--   0        0        0     3660 2024-05-11 00:35:58.941798 devon_agent-0.1.7/devon_agent/retrieval/graph_visualization.py
--rw-r--r--   0        0        0     9059 2024-05-11 01:41:30.027339 devon_agent-0.1.7/devon_agent/retrieval/main.py
--rw-r--r--   0        0        0     6503 2024-05-18 02:03:47.413025 devon_agent-0.1.7/devon_agent/server.py
--rw-r--r--   0        0        0    19013 2024-05-18 02:03:47.414506 devon_agent-0.1.7/devon_agent/session.py
--rw-r--r--   0        0        0     3119 2024-05-17 17:44:26.704374 devon_agent-0.1.7/devon_agent/swebenchrun.py
--rw-r--r--   0        0        0    21981 2024-05-17 17:43:48.274284 devon_agent-0.1.7/devon_agent/sweenvsession.py
--rw-r--r--   0        0        0     4609 2024-05-17 17:40:28.555245 devon_agent-0.1.7/devon_agent/telemetry.py
--rw-r--r--   0        0        0     1974 2024-05-17 17:40:28.555527 devon_agent-0.1.7/devon_agent/test/test_parse_commands.py
--rw-r--r--   0        0        0      811 2024-05-11 01:43:13.118702 devon_agent-0.1.7/devon_agent/test/test_tools.py
--rw-r--r--   0        0        0     3171 2024-05-17 21:36:14.559402 devon_agent-0.1.7/devon_agent/tool.py
--rw-r--r--   0        0        0     3704 2024-05-17 17:40:28.556700 devon_agent-0.1.7/devon_agent/tools/__init__.py
--rw-r--r--   0        0        0     5239 2024-05-17 17:40:28.557168 devon_agent-0.1.7/devon_agent/tools/codeindex.py
--rw-r--r--   0        0        0        0 2024-05-17 17:40:28.557212 devon_agent-0.1.7/devon_agent/tools/create_file.py
--rw-r--r--   0        0        0    20114 2024-05-17 17:40:28.557833 devon_agent-0.1.7/devon_agent/tools/editortools.py
--rw-r--r--   0        0        0     7140 2024-05-17 17:40:28.558102 devon_agent-0.1.7/devon_agent/tools/edittools.py
--rw-r--r--   0        0        0     8249 2024-05-17 17:40:28.558706 devon_agent-0.1.7/devon_agent/tools/filesearchtools.py
--rw-r--r--   0        0        0    12460 2024-05-17 17:40:28.558925 devon_agent-0.1.7/devon_agent/tools/filetools.py
--rw-r--r--   0        0        0     2467 2024-05-17 17:40:28.559131 devon_agent-0.1.7/devon_agent/tools/lifecycle.py
--rw-r--r--   0        0        0     1097 2024-05-17 17:40:28.559319 devon_agent-0.1.7/devon_agent/tools/shelltool.py
--rw-r--r--   0        0        0     1279 2024-05-17 17:40:28.559558 devon_agent-0.1.7/devon_agent/tools/swebenchtools.py
--rw-r--r--   0        0        0     1413 2024-05-17 17:40:28.559746 devon_agent-0.1.7/devon_agent/tools/usertools.py
--rw-r--r--   0        0        0     6703 2024-05-18 02:03:47.415177 devon_agent-0.1.7/devon_agent/tools/utils.py
--rw-r--r--   0        0        0    29381 2024-05-12 05:56:27.613854 devon_agent-0.1.7/devon_agent/udiff.py
--rw-r--r--   0        0        0      727 2024-05-10 17:13:36.835159 devon_agent-0.1.7/devon_agent/utils.py
--rw-r--r--   0        0        0     1509 2024-05-10 17:13:36.835377 devon_agent-0.1.7/devon_agent/vgit.py
--rw-r--r--   0        0        0     1226 2024-05-18 05:00:59.994417 devon_agent-0.1.7/pyproject.toml
--rw-r--r--   0        0        0     7396 1970-01-01 00:00:00.000000 devon_agent-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-03-17 15:42:25.856965 devon_agent-0.1.8/LICENSE
+-rw-r--r--   0        0        0     5840 2024-05-18 02:03:47.403799 devon_agent-0.1.8/README.md
+-rw-r--r--   0        0        0      851 2024-05-18 02:03:47.410014 devon_agent-0.1.8/devon_agent/__main__.py
+-rw-r--r--   0        0        0    11192 2024-05-17 21:36:14.554449 devon_agent-0.1.8/devon_agent/agent.py
+-rw-r--r--   0        0        0     8999 2024-05-18 02:03:47.410538 devon_agent-0.1.8/devon_agent/agents/default/agent.py
+-rw-r--r--   0        0        0     6648 2024-05-18 02:03:47.410905 devon_agent-0.1.8/devon_agent/agents/default/anthropic_prompts.py
+-rw-r--r--   0        0        0     6841 2024-05-18 04:58:22.551556 devon_agent-0.1.8/devon_agent/agents/default/openai_prompts.py
+-rw-r--r--   0        0        0     5405 2024-05-18 18:53:42.487001 devon_agent-0.1.8/devon_agent/agents/model.py
+-rw-r--r--   0        0        0     7281 2024-05-18 02:03:47.412440 devon_agent-0.1.8/devon_agent/environment.py
+-rw-r--r--   0        0        0    30089 2024-05-17 17:40:28.549419 devon_agent-0.1.8/devon_agent/environments/swebenchenv.py
+-rw-r--r--   0        0        0     1247 2024-05-17 21:36:14.557332 devon_agent-0.1.8/devon_agent/event.py
+-rw-r--r--   0        0        0     9464 2024-05-18 01:59:15.254179 devon_agent-0.1.8/devon_agent/experimental/dspyloop.py
+-rw-r--r--   0        0        0     2800 2024-05-17 17:40:44.223838 devon_agent-0.1.8/devon_agent/model.py
+-rw-r--r--   0        0        0    21113 2024-05-17 21:36:14.558749 devon_agent-0.1.8/devon_agent/prompt.py
+-rw-r--r--   0        0        0     6317 2024-05-11 01:42:20.814775 devon_agent-0.1.8/devon_agent/retrieval/ast_extractor.py
+-rw-r--r--   0        0        0      561 2024-05-11 00:35:58.937331 devon_agent-0.1.8/devon_agent/retrieval/ast_parser.py
+-rw-r--r--   0        0        0     6430 2024-05-17 21:36:48.492247 devon_agent-0.1.8/devon_agent/retrieval/code_index.py
+-rw-r--r--   0        0        0     7207 2024-05-17 21:36:48.492590 devon_agent-0.1.8/devon_agent/retrieval/codebase_graph.py
+-rw-r--r--   0        0        0      913 2024-05-17 17:40:28.552873 devon_agent-0.1.8/devon_agent/retrieval/file_discovery.py
+-rw-r--r--   0        0        0     3660 2024-05-11 00:35:58.941798 devon_agent-0.1.8/devon_agent/retrieval/graph_visualization.py
+-rw-r--r--   0        0        0     9059 2024-05-11 01:41:30.027339 devon_agent-0.1.8/devon_agent/retrieval/main.py
+-rw-r--r--   0        0        0     6503 2024-05-18 02:03:47.413025 devon_agent-0.1.8/devon_agent/server.py
+-rw-r--r--   0        0        0    19013 2024-05-18 02:03:47.414506 devon_agent-0.1.8/devon_agent/session.py
+-rw-r--r--   0        0        0     3119 2024-05-17 17:44:26.704374 devon_agent-0.1.8/devon_agent/swebenchrun.py
+-rw-r--r--   0        0        0    21981 2024-05-17 17:43:48.274284 devon_agent-0.1.8/devon_agent/sweenvsession.py
+-rw-r--r--   0        0        0     4609 2024-05-17 17:40:28.555245 devon_agent-0.1.8/devon_agent/telemetry.py
+-rw-r--r--   0        0        0     1974 2024-05-17 17:40:28.555527 devon_agent-0.1.8/devon_agent/test/test_parse_commands.py
+-rw-r--r--   0        0        0      811 2024-05-11 01:43:13.118702 devon_agent-0.1.8/devon_agent/test/test_tools.py
+-rw-r--r--   0        0        0     3171 2024-05-17 21:36:14.559402 devon_agent-0.1.8/devon_agent/tool.py
+-rw-r--r--   0        0        0     3704 2024-05-17 17:40:28.556700 devon_agent-0.1.8/devon_agent/tools/__init__.py
+-rw-r--r--   0        0        0     5239 2024-05-17 17:40:28.557168 devon_agent-0.1.8/devon_agent/tools/codeindex.py
+-rw-r--r--   0        0        0        0 2024-05-17 17:40:28.557212 devon_agent-0.1.8/devon_agent/tools/create_file.py
+-rw-r--r--   0        0        0    20114 2024-05-17 17:40:28.557833 devon_agent-0.1.8/devon_agent/tools/editortools.py
+-rw-r--r--   0        0        0     7140 2024-05-17 17:40:28.558102 devon_agent-0.1.8/devon_agent/tools/edittools.py
+-rw-r--r--   0        0        0     8249 2024-05-17 17:40:28.558706 devon_agent-0.1.8/devon_agent/tools/filesearchtools.py
+-rw-r--r--   0        0        0    12460 2024-05-17 17:40:28.558925 devon_agent-0.1.8/devon_agent/tools/filetools.py
+-rw-r--r--   0        0        0     2467 2024-05-17 17:40:28.559131 devon_agent-0.1.8/devon_agent/tools/lifecycle.py
+-rw-r--r--   0        0        0     1097 2024-05-17 17:40:28.559319 devon_agent-0.1.8/devon_agent/tools/shelltool.py
+-rw-r--r--   0        0        0     1279 2024-05-17 17:40:28.559558 devon_agent-0.1.8/devon_agent/tools/swebenchtools.py
+-rw-r--r--   0        0        0     1413 2024-05-17 17:40:28.559746 devon_agent-0.1.8/devon_agent/tools/usertools.py
+-rw-r--r--   0        0        0     6703 2024-05-18 02:03:47.415177 devon_agent-0.1.8/devon_agent/tools/utils.py
+-rw-r--r--   0        0        0    29381 2024-05-12 05:56:27.613854 devon_agent-0.1.8/devon_agent/udiff.py
+-rw-r--r--   0        0        0      727 2024-05-10 17:13:36.835159 devon_agent-0.1.8/devon_agent/utils.py
+-rw-r--r--   0        0        0     1509 2024-05-10 17:13:36.835377 devon_agent-0.1.8/devon_agent/vgit.py
+-rw-r--r--   0        0        0     1226 2024-05-18 16:29:00.701629 devon_agent-0.1.8/pyproject.toml
+-rw-r--r--   0        0        0     7396 1970-01-01 00:00:00.000000 devon_agent-0.1.8/PKG-INFO
```

### Comparing `devon_agent-0.1.7/LICENSE` & `devon_agent-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `devon_agent-0.1.7/README.md` & `devon_agent-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `devon_agent-0.1.7/devon_agent/__main__.py` & `devon_agent-0.1.8/devon_agent/__main__.py`

 * *Files identical despite different names*

### Comparing `devon_agent-0.1.7/devon_agent/agent.py` & `devon_agent-0.1.8/devon_agent/agent.py`

 * *Files identical despite different names*

### Comparing `devon_agent-0.1.7/devon_agent/agents/default/agent.py` & `devon_agent-0.1.8/devon_agent/agents/default/agent.py`

 * *Files identical despite different names*

### Comparing `devon_agent-0.1.7/devon_agent/agents/default/anthropic_prompts.py` & `devon_agent-0.1.8/devon_agent/agents/default/anthropic_prompts.py`

 * *Files identical despite different names*

### Comparing `devon_agent-0.1.7/devon_agent/agents/default/openai_prompts.py` & `devon_agent-0.1.8/devon_agent/agents/default/openai_prompts.py`

 * *Files identical despite different names*

### Comparing `devon_agent-0.1.7/devon_agent/agents/model.py` & `devon_agent-0.1.8/devon_agent/agents/model.py`

 * *Files identical despite different names*

### Comparing `devon_agent-0.1.7/devon_agent/environment.py` & `devon_agent-0.1.8/devon_agent/environment.py`

 * *Files identical despite different names*

### Comparing `devon_agent-0.1.7/devon_agent/environments/swebenchenv.py` & `devon_agent-0.1.8/devon_agent/environments/swebenchenv.py`

 * *Files identical despite different names*

### Comparing `devon_agent-0.1.7/devon_agent/event.py` & `devon_agent-0.1.8/devon_agent/event.py`

 * *Files identical despite different names*

### Comparing `devon_agent-0.1.7/devon_agent/experimental/dspyloop.py` & `devon_agent-0.1.8/devon_agent/experimental/dspyloop.py`

 * *Files identical despite different names*

### Comparing `devon_agent-0.1.7/devon_agent/model.py` & `devon_agent-0.1.8/devon_agent/model.py`

 * *Files identical despite different names*

### Comparing `devon_agent-0.1.7/devon_agent/prompt.py` & `devon_agent-0.1.8/devon_agent/prompt.py`

 * *Files identical despite different names*

### Comparing `devon_agent-0.1.7/devon_agent/retrieval/ast_extractor.py` & `devon_agent-0.1.8/devon_agent/retrieval/ast_extractor.py`

 * *Files identical despite different names*

### Comparing `devon_agent-0.1.7/devon_agent/retrieval/ast_parser.py` & `devon_agent-0.1.8/devon_agent/retrieval/ast_parser.py`

 * *Files identical despite different names*

### Comparing `devon_agent-0.1.7/devon_agent/retrieval/code_index.py` & `devon_agent-0.1.8/devon_agent/retrieval/code_index.py`

 * *Files identical despite different names*

### Comparing `devon_agent-0.1.7/devon_agent/retrieval/codebase_graph.py` & `devon_agent-0.1.8/devon_agent/retrieval/codebase_graph.py`

 * *Files identical despite different names*

### Comparing `devon_agent-0.1.7/devon_agent/retrieval/file_discovery.py` & `devon_agent-0.1.8/devon_agent/retrieval/file_discovery.py`

 * *Files identical despite different names*

### Comparing `devon_agent-0.1.7/devon_agent/retrieval/graph_visualization.py` & `devon_agent-0.1.8/devon_agent/retrieval/graph_visualization.py`

 * *Files identical despite different names*

### Comparing `devon_agent-0.1.7/devon_agent/retrieval/main.py` & `devon_agent-0.1.8/devon_agent/retrieval/main.py`

 * *Files identical despite different names*

### Comparing `devon_agent-0.1.7/devon_agent/server.py` & `devon_agent-0.1.8/devon_agent/server.py`

 * *Files identical despite different names*

### Comparing `devon_agent-0.1.7/devon_agent/session.py` & `devon_agent-0.1.8/devon_agent/session.py`

 * *Files identical despite different names*

### Comparing `devon_agent-0.1.7/devon_agent/swebenchrun.py` & `devon_agent-0.1.8/devon_agent/swebenchrun.py`

 * *Files identical despite different names*

### Comparing `devon_agent-0.1.7/devon_agent/sweenvsession.py` & `devon_agent-0.1.8/devon_agent/sweenvsession.py`

 * *Files identical despite different names*

### Comparing `devon_agent-0.1.7/devon_agent/telemetry.py` & `devon_agent-0.1.8/devon_agent/telemetry.py`

 * *Files identical despite different names*

### Comparing `devon_agent-0.1.7/devon_agent/test/test_parse_commands.py` & `devon_agent-0.1.8/devon_agent/test/test_parse_commands.py`

 * *Files identical despite different names*

### Comparing `devon_agent-0.1.7/devon_agent/test/test_tools.py` & `devon_agent-0.1.8/devon_agent/test/test_tools.py`

 * *Files identical despite different names*

### Comparing `devon_agent-0.1.7/devon_agent/tool.py` & `devon_agent-0.1.8/devon_agent/tool.py`

 * *Files identical despite different names*

### Comparing `devon_agent-0.1.7/devon_agent/tools/__init__.py` & `devon_agent-0.1.8/devon_agent/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `devon_agent-0.1.7/devon_agent/tools/codeindex.py` & `devon_agent-0.1.8/devon_agent/tools/codeindex.py`

 * *Files identical despite different names*

### Comparing `devon_agent-0.1.7/devon_agent/tools/editortools.py` & `devon_agent-0.1.8/devon_agent/tools/editortools.py`

 * *Files identical despite different names*

### Comparing `devon_agent-0.1.7/devon_agent/tools/edittools.py` & `devon_agent-0.1.8/devon_agent/tools/edittools.py`

 * *Files identical despite different names*

### Comparing `devon_agent-0.1.7/devon_agent/tools/filesearchtools.py` & `devon_agent-0.1.8/devon_agent/tools/filesearchtools.py`

 * *Files identical despite different names*

### Comparing `devon_agent-0.1.7/devon_agent/tools/filetools.py` & `devon_agent-0.1.8/devon_agent/tools/filetools.py`

 * *Files identical despite different names*

### Comparing `devon_agent-0.1.7/devon_agent/tools/lifecycle.py` & `devon_agent-0.1.8/devon_agent/tools/lifecycle.py`

 * *Files identical despite different names*

### Comparing `devon_agent-0.1.7/devon_agent/tools/shelltool.py` & `devon_agent-0.1.8/devon_agent/tools/shelltool.py`

 * *Files identical despite different names*

### Comparing `devon_agent-0.1.7/devon_agent/tools/swebenchtools.py` & `devon_agent-0.1.8/devon_agent/tools/swebenchtools.py`

 * *Files identical despite different names*

### Comparing `devon_agent-0.1.7/devon_agent/tools/usertools.py` & `devon_agent-0.1.8/devon_agent/tools/usertools.py`

 * *Files identical despite different names*

### Comparing `devon_agent-0.1.7/devon_agent/tools/utils.py` & `devon_agent-0.1.8/devon_agent/tools/utils.py`

 * *Files identical despite different names*

### Comparing `devon_agent-0.1.7/devon_agent/udiff.py` & `devon_agent-0.1.8/devon_agent/udiff.py`

 * *Files identical despite different names*

### Comparing `devon_agent-0.1.7/devon_agent/utils.py` & `devon_agent-0.1.8/devon_agent/utils.py`

 * *Files identical despite different names*

### Comparing `devon_agent-0.1.7/devon_agent/vgit.py` & `devon_agent-0.1.8/devon_agent/vgit.py`

 * *Files identical despite different names*

### Comparing `devon_agent-0.1.7/pyproject.toml` & `devon_agent-0.1.8/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "devon-agent"
-version = "0.1.7"
+version = "0.1.8"
 description = ""
 authors = ["killind-dev <61808204+killind-dev@users.noreply.github.com>","mihir1003 <mihir1003@gmail.com>"]
 readme = "README.md"
 exclude = [
     "devon_tui",
 ]
```

### Comparing `devon_agent-0.1.7/PKG-INFO` & `devon_agent-0.1.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: devon-agent
-Version: 0.1.7
+Version: 0.1.8
 Summary: 
 Author: killind-dev
 Author-email: 61808204+killind-dev@users.noreply.github.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: devon-agent Version: 0.1.7 Summary: Author:
+Metadata-Version: 2.1 Name: devon-agent Version: 0.1.8 Summary: Author:
 killind-dev Author-email: 61808204+killind-dev@users.noreply.github.com
 Requires-Python: >=3.10,<4.0 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3.11 Classifier: Programming Language :: Python :: 3.12
 Provides-Extra: experimental Provides-Extra: swebench Requires-Dist: anthropic
 (>=0.20.0,<0.21.0) Requires-Dist: astroid (>=3.1.0,<4.0.0) Requires-Dist: click
 (>=8.1.7,<9.0.0) Requires-Dist: datasets (>=2.14.6,<2.15.0) ; extra ==
```

