# Comparing `tmp/devon_agent-0.1.6.tar.gz` & `tmp/devon_agent-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "devon_agent-0.1.6.tar", max compression
+gzip compressed data, was "devon_agent-0.1.7.tar", max compression
```

## Comparing `devon_agent-0.1.6.tar` & `devon_agent-0.1.7.tar`

### file list

```diff
@@ -1,24 +1,46 @@
--rw-r--r--   0        0        0    11357 2024-05-07 20:13:56.337461 devon_agent-0.1.6/LICENSE
--rw-r--r--   0        0        0     5540 2024-05-11 06:54:09.693598 devon_agent-0.1.6/README.md
--rw-r--r--   0        0        0      129 2024-05-10 22:03:09.786842 devon_agent-0.1.6/devon_agent/TODO
--rw-r--r--   0        0        0      794 2024-05-11 06:54:09.697598 devon_agent-0.1.6/devon_agent/__main__.py
--rw-r--r--   0        0        0    10485 2024-05-12 01:48:11.184292 devon_agent-0.1.6/devon_agent/agent.py
--rw-r--r--   0        0        0     2512 2024-05-11 06:54:09.697598 devon_agent-0.1.6/devon_agent/environment.py
--rw-r--r--   0        0        0     2195 2024-05-11 06:54:09.697598 devon_agent-0.1.6/devon_agent/model.py
--rw-r--r--   0        0        0    21113 2024-05-12 03:43:10.033955 devon_agent-0.1.6/devon_agent/prompt.py
--rw-r--r--   0        0        0     6317 2024-05-11 06:54:09.697598 devon_agent-0.1.6/devon_agent/retrieval/ast_extractor.py
--rw-r--r--   0        0        0      561 2024-05-11 06:54:09.697598 devon_agent-0.1.6/devon_agent/retrieval/ast_parser.py
--rw-r--r--   0        0        0     5222 2024-05-11 06:54:09.697598 devon_agent-0.1.6/devon_agent/retrieval/codebase_graph.py
--rw-r--r--   0        0        0      849 2024-05-11 06:54:09.697598 devon_agent-0.1.6/devon_agent/retrieval/file_discovery.py
--rw-r--r--   0        0        0     3660 2024-05-11 06:54:09.697598 devon_agent-0.1.6/devon_agent/retrieval/graph_visualization.py
--rw-r--r--   0        0        0     9059 2024-05-11 06:54:09.697598 devon_agent-0.1.6/devon_agent/retrieval/main.py
--rw-r--r--   0        0        0     6312 2024-05-12 00:28:17.089558 devon_agent-0.1.6/devon_agent/server.py
--rw-r--r--   0        0        0    15118 2024-05-12 01:47:30.552282 devon_agent-0.1.6/devon_agent/session.py
--rw-r--r--   0        0        0     4607 2024-05-11 06:54:09.697598 devon_agent-0.1.6/devon_agent/telemetry.py
--rw-r--r--   0        0        0      811 2024-05-11 06:54:09.697598 devon_agent-0.1.6/devon_agent/test/test_tools.py
--rw-r--r--   0        0        0    42596 2024-05-12 01:49:57.244432 devon_agent-0.1.6/devon_agent/tools.py
--rw-r--r--   0        0        0    29381 2024-05-11 06:54:09.697598 devon_agent-0.1.6/devon_agent/udiff.py
--rw-r--r--   0        0        0      727 2024-05-10 22:03:09.790843 devon_agent-0.1.6/devon_agent/utils.py
--rw-r--r--   0        0        0     1509 2024-05-10 22:03:09.790843 devon_agent-0.1.6/devon_agent/vgit.py
--rw-r--r--   0        0        0     1131 2024-05-12 03:43:51.754291 devon_agent-0.1.6/pyproject.toml
--rw-r--r--   0        0        0     6960 1970-01-01 00:00:00.000000 devon_agent-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-03-17 15:42:25.856965 devon_agent-0.1.7/LICENSE
+-rw-r--r--   0        0        0     5840 2024-05-18 02:03:47.403799 devon_agent-0.1.7/README.md
+-rw-r--r--   0        0        0      851 2024-05-18 02:03:47.410014 devon_agent-0.1.7/devon_agent/__main__.py
+-rw-r--r--   0        0        0    11192 2024-05-17 21:36:14.554449 devon_agent-0.1.7/devon_agent/agent.py
+-rw-r--r--   0        0        0     8999 2024-05-18 02:03:47.410538 devon_agent-0.1.7/devon_agent/agents/default/agent.py
+-rw-r--r--   0        0        0     6648 2024-05-18 02:03:47.410905 devon_agent-0.1.7/devon_agent/agents/default/anthropic_prompts.py
+-rw-r--r--   0        0        0     6841 2024-05-18 04:58:22.551556 devon_agent-0.1.7/devon_agent/agents/default/openai_prompts.py
+-rw-r--r--   0        0        0     5405 2024-05-18 02:03:47.412052 devon_agent-0.1.7/devon_agent/agents/model.py
+-rw-r--r--   0        0        0     7281 2024-05-18 02:03:47.412440 devon_agent-0.1.7/devon_agent/environment.py
+-rw-r--r--   0        0        0    30089 2024-05-17 17:40:28.549419 devon_agent-0.1.7/devon_agent/environments/swebenchenv.py
+-rw-r--r--   0        0        0     1247 2024-05-17 21:36:14.557332 devon_agent-0.1.7/devon_agent/event.py
+-rw-r--r--   0        0        0     9464 2024-05-18 01:59:15.254179 devon_agent-0.1.7/devon_agent/experimental/dspyloop.py
+-rw-r--r--   0        0        0     2800 2024-05-17 17:40:44.223838 devon_agent-0.1.7/devon_agent/model.py
+-rw-r--r--   0        0        0    21113 2024-05-17 21:36:14.558749 devon_agent-0.1.7/devon_agent/prompt.py
+-rw-r--r--   0        0        0     6317 2024-05-11 01:42:20.814775 devon_agent-0.1.7/devon_agent/retrieval/ast_extractor.py
+-rw-r--r--   0        0        0      561 2024-05-11 00:35:58.937331 devon_agent-0.1.7/devon_agent/retrieval/ast_parser.py
+-rw-r--r--   0        0        0     6430 2024-05-17 21:36:48.492247 devon_agent-0.1.7/devon_agent/retrieval/code_index.py
+-rw-r--r--   0        0        0     7207 2024-05-17 21:36:48.492590 devon_agent-0.1.7/devon_agent/retrieval/codebase_graph.py
+-rw-r--r--   0        0        0      913 2024-05-17 17:40:28.552873 devon_agent-0.1.7/devon_agent/retrieval/file_discovery.py
+-rw-r--r--   0        0        0     3660 2024-05-11 00:35:58.941798 devon_agent-0.1.7/devon_agent/retrieval/graph_visualization.py
+-rw-r--r--   0        0        0     9059 2024-05-11 01:41:30.027339 devon_agent-0.1.7/devon_agent/retrieval/main.py
+-rw-r--r--   0        0        0     6503 2024-05-18 02:03:47.413025 devon_agent-0.1.7/devon_agent/server.py
+-rw-r--r--   0        0        0    19013 2024-05-18 02:03:47.414506 devon_agent-0.1.7/devon_agent/session.py
+-rw-r--r--   0        0        0     3119 2024-05-17 17:44:26.704374 devon_agent-0.1.7/devon_agent/swebenchrun.py
+-rw-r--r--   0        0        0    21981 2024-05-17 17:43:48.274284 devon_agent-0.1.7/devon_agent/sweenvsession.py
+-rw-r--r--   0        0        0     4609 2024-05-17 17:40:28.555245 devon_agent-0.1.7/devon_agent/telemetry.py
+-rw-r--r--   0        0        0     1974 2024-05-17 17:40:28.555527 devon_agent-0.1.7/devon_agent/test/test_parse_commands.py
+-rw-r--r--   0        0        0      811 2024-05-11 01:43:13.118702 devon_agent-0.1.7/devon_agent/test/test_tools.py
+-rw-r--r--   0        0        0     3171 2024-05-17 21:36:14.559402 devon_agent-0.1.7/devon_agent/tool.py
+-rw-r--r--   0        0        0     3704 2024-05-17 17:40:28.556700 devon_agent-0.1.7/devon_agent/tools/__init__.py
+-rw-r--r--   0        0        0     5239 2024-05-17 17:40:28.557168 devon_agent-0.1.7/devon_agent/tools/codeindex.py
+-rw-r--r--   0        0        0        0 2024-05-17 17:40:28.557212 devon_agent-0.1.7/devon_agent/tools/create_file.py
+-rw-r--r--   0        0        0    20114 2024-05-17 17:40:28.557833 devon_agent-0.1.7/devon_agent/tools/editortools.py
+-rw-r--r--   0        0        0     7140 2024-05-17 17:40:28.558102 devon_agent-0.1.7/devon_agent/tools/edittools.py
+-rw-r--r--   0        0        0     8249 2024-05-17 17:40:28.558706 devon_agent-0.1.7/devon_agent/tools/filesearchtools.py
+-rw-r--r--   0        0        0    12460 2024-05-17 17:40:28.558925 devon_agent-0.1.7/devon_agent/tools/filetools.py
+-rw-r--r--   0        0        0     2467 2024-05-17 17:40:28.559131 devon_agent-0.1.7/devon_agent/tools/lifecycle.py
+-rw-r--r--   0        0        0     1097 2024-05-17 17:40:28.559319 devon_agent-0.1.7/devon_agent/tools/shelltool.py
+-rw-r--r--   0        0        0     1279 2024-05-17 17:40:28.559558 devon_agent-0.1.7/devon_agent/tools/swebenchtools.py
+-rw-r--r--   0        0        0     1413 2024-05-17 17:40:28.559746 devon_agent-0.1.7/devon_agent/tools/usertools.py
+-rw-r--r--   0        0        0     6703 2024-05-18 02:03:47.415177 devon_agent-0.1.7/devon_agent/tools/utils.py
+-rw-r--r--   0        0        0    29381 2024-05-12 05:56:27.613854 devon_agent-0.1.7/devon_agent/udiff.py
+-rw-r--r--   0        0        0      727 2024-05-10 17:13:36.835159 devon_agent-0.1.7/devon_agent/utils.py
+-rw-r--r--   0        0        0     1509 2024-05-10 17:13:36.835377 devon_agent-0.1.7/devon_agent/vgit.py
+-rw-r--r--   0        0        0     1226 2024-05-18 05:00:59.994417 devon_agent-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0     7396 1970-01-01 00:00:00.000000 devon_agent-0.1.7/PKG-INFO
```

### Comparing `devon_agent-0.1.6/LICENSE` & `devon_agent-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `devon_agent-0.1.6/README.md` & `devon_agent-0.1.7/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -8,30 +8,29 @@
   <a href="https://github.com/entropy-research/Devon/network/members"><img src="https://img.shields.io/github/forks/entropy-research/devon?style=for-the-badge&color=orange" alt="Forks"></a>
   <a href="https://github.com/entropy-research/Devon/stargazers"><img src="https://img.shields.io/github/stars/entropy-research/devon?style=for-the-badge&color=yellow" alt="Stargazers"></a>
   <a href="https://github.com/entropy-research/Devon/issues"><img src="https://img.shields.io/github/issues/entropy-research/devon?style=for-the-badge&color=red" alt="Issues"></a>
   <br/>
   <a href="https://github.com/entropy-research/Devon/blob/main/LICENSE"><img src="https://img.shields.io/github/license/entropy-research/devon?style=for-the-badge&color=blue" alt="Apache 2.0 License"></a>
   <a href="https://discord.gg/p5YpZ5vjd9"><img src="https://img.shields.io/badge/Discord-Join%20Us-purple?logo=discord&logoColor=white&style=for-the-badge" alt="Join our Discord community"></a>
   <br/>
-</div>
-
 
-> Video/GIF Coming Soon!
+https://github.com/entropy-research/Devon/assets/61808204/d42a8b9a-0211-4624-9804-d24df1d4dbf6
+</div>
 
 # Installation
 
 ## Prerequisites
 
 1. `node.js` and `npm`
 2. `pipx`, if you don't have this go [here](https://pipx.pypa.io/stable/installation/)
-3. [**Anthropic**](https://console.anthropic.com/settings/keys) API Key
+3. [**Anthropic**](https://console.anthropic.com/settings/keys) API Key or [**OpenAI**](https://platform.openai.com/api-keys) API key
 
 ## Installation commands
 
-To use, simply run:
+To install, simply run:
 
 ```bash
 curl -sSL https://raw.githubusercontent.com/entropy-research/Devon/main/install.sh | bash
 ```
 
 
 *Or to install using `pipx` + `npm`:*
@@ -42,33 +41,42 @@
 ```
 
 This installs the Python backend, and the cli command to run the tool
 
 ### Thats it! Happy building :)
 
 
-# Usage
+# Running the agent
 Navigate to your project folder and open the terminal.
 
-Set your Anthropic API key as an environment variable:
+Set your Anthropic API or OpenAI API key as an environment variable:
 
 ```bash
 export ANTHROPIC_API_KEY=sk-xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx
+
+#OR
+
+export OPENAI_API_KEY=sk-xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx
 ```
 
 Then to *run*, the command is:
 ```bash
 devon
 ```
 
 It's as easy as that.
 
 > [!NOTE]
 > Don't worry, the agent will be able to only access files and folders in the directory you started it from. You can also correct it while it's performing actions.
 
+To run in *debug* mode, the command is:
+```bash
+devon --debug
+```
+
 # Features
 - Multi-file editing
 - Codebase exploration
 - Config writing
 - Test writing
 - Bug fixing
 - Architecture exploration
```

#### html2text {}

```diff
@@ -1,25 +1,30 @@
               ************ DDeevvoonn:: AAnn ooppeenn--ssoouurrccee ppaaiirr pprrooggrraammmmeerr ************
                    _[_C_o_n_t_r_i_b_u_t_o_r_s_]_[_F_o_r_k_s_]_[_S_t_a_r_g_a_z_e_r_s_]_[_I_s_s_u_e_s_]
                _[_A_p_a_c_h_e_ _2_._0_ _L_i_c_e_n_s_e_]_[_J_o_i_n_ _o_u_r_ _D_i_s_c_o_r_d_ _c_o_m_m_u_n_i_t_y_]
-> Video/GIF Coming Soon! # Installation ## Prerequisites 1. `node.js` and `npm`
-2. `pipx`, if you don't have this go [here](https://pipx.pypa.io/stable/
-installation/) 3. [**Anthropic**](https://console.anthropic.com/settings/keys)
-API Key ## Installation commands To use, simply run: ```bash curl -sSL https://
+ https://github.com/entropy-research/Devon/assets/61808204/d42a8b9a-0211-4624-
+                               9804-d24df1d4dbf6
+# Installation ## Prerequisites 1. `node.js` and `npm` 2. `pipx`, if you don't
+have this go [here](https://pipx.pypa.io/stable/installation/) 3.
+[**Anthropic**](https://console.anthropic.com/settings/keys) API Key or
+[**OpenAI**](https://platform.openai.com/api-keys) API key ## Installation
+commands To install, simply run: ```bash curl -sSL https://
 raw.githubusercontent.com/entropy-research/Devon/main/install.sh | bash ``` *Or
 to install using `pipx` + `npm`:* ```bash pipx install devon_agent npm install
 -g devon-tui ``` This installs the Python backend, and the cli command to run
-the tool ### Thats it! Happy building :) # Usage Navigate to your project
-folder and open the terminal. Set your Anthropic API key as an environment
-variable: ```bash export ANTHROPIC_API_KEY=sk-
+the tool ### Thats it! Happy building :) # Running the agent Navigate to your
+project folder and open the terminal. Set your Anthropic API or OpenAI API key
+as an environment variable: ```bash export ANTHROPIC_API_KEY=sk-
+xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx #OR export OPENAI_API_KEY=sk-
 xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx ``` Then to *run*, the command is:
 ```bash devon ``` It's as easy as that. > [!NOTE] > Don't worry, the agent will
 be able to only access files and folders in the directory you started it from.
-You can also correct it while it's performing actions. # Features - Multi-file
-editing - Codebase exploration - Config writing - Test writing - Bug fixing -
+You can also correct it while it's performing actions. To run in *debug* mode,
+the command is: ```bash devon --debug ``` # Features - Multi-file editing -
+Codebase exploration - Config writing - Test writing - Bug fixing -
 Architecture exploration ### Limitations - Minimal functionality for non-Python
 languages - Sometimes have to specify the file where you want the change to
 happen # Progress ### This project is still super early and we would love your
 help to make it great! ### Current goals - Multi-model support - Launch plugin
 system for tool and agent builders - Create self-hostable Electron app - Set
 SOTA on [SWE-bench Lite](https://www.swebench.com/lite.html) > View our current
 thoughts on next steps [**here**](https://docs.google.com/document/d/e/2PACX-
```

### Comparing `devon_agent-0.1.6/devon_agent/agent.py` & `devon_agent-0.1.7/devon_agent/agent.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 import json
 import logging
 from dataclasses import dataclass, field
+import traceback
 from typing import Optional, Tuple
 
 from devon_agent.model import AnthropicModel, ModelArguments
 from devon_agent.prompt import (
     commands_to_command_docs,
     history_to_bash_history,
     last_user_prompt_template_v3,
     parse_response,
     system_prompt_template_v3,
 )
+from devon_agent.tools.utils import get_cwd
 
 from devon_agent.udiff import Hallucination
-from devon_agent.utils import LOGGER_NAME
+from devon_agent.utils import LOGGER_NAME, DotDict
 from tenacity import RetryError
 
 from typing import TYPE_CHECKING
 
 if TYPE_CHECKING:
     from devon_agent.session import Session
 
@@ -84,16 +86,19 @@
             args=ModelArguments(
                 model_name=self.model,
                 temperature=self.temperature,
                 api_key=self.api_key,
             )
         )
         try:
+            # print(session.state.editor)
+            # print(session.state.editor.PAGE_SIZE)
+            # print(session.state.editor.files)
             editor = self._convert_editor_to_view(
-                session.state.editor, session.state.PAGE_SIZE
+                session.state.editor.files, session.state.editor.PAGE_SIZE
             )
 
             self.chat_history.append(
                 {"role": "user", "content": observation, "agent": self.name}
             )
 
             commands = (
@@ -130,15 +135,21 @@
                 self.current_model.args.temperature += (
                     0.2 if self.current_model.args.temperature < 0.8 else 0
                 )
             else:
                 history = history_to_bash_history(self.chat_history)
 
             last_user_prompt = last_user_prompt_template_v3(
-                task, history, editor, session.environment.get_cwd(), session.base_path, self.scratchpad
+                task, history, editor, get_cwd(
+                    {
+                        "session" : session,
+                        "environment" : session.default_environment,
+                        "state" : session.state
+                    }
+                ), session.base_path, self.scratchpad
             )
 
             messages = [{"role": "user", "content": last_user_prompt}]
 
             output = self.current_model.query(messages, system_message=system_prompt)
 
             # logger.debug(
@@ -156,18 +167,18 @@
                 #     continue
 
             try:
                 thought, action, scratchpad = parse_response(output)
                 if scratchpad:
                     self.scratchpad = scratchpad
             except Exception:
-                raise ValueError(f"Multiple actions found in response: {output}")
+                raise Hallucination(f"Multiple actions found in response: {output}")
             
             if not thought or not action:
-                raise ValueError("Agent failed to follow response format instructions")
+                raise Hallucination("Agent failed to follow response format instructions")
 
             self.chat_history.append(
                 {
                     "role": "assistant",
                     "content": output,
                     "thought": thought,
                     "action": action,
@@ -187,14 +198,16 @@
 
 SCRATCHPAD: {scratchpad}
 \n\n****************\n\n\n\n""")
 
             return thought, action, output
         except KeyboardInterrupt:
             raise
+        except Hallucination as e:
+            return "hallucination","hallucination","Incorrect response format"
         except RuntimeError as e:
             session.event_log.append(
                 {
                     "type": "Error",
                     "content": str(e),
                     "producer": self.name,
                     "consumer": "none",
@@ -226,14 +239,15 @@
                 {
                     "type": "Error",
                     "content": str(e),
                     "producer": self.name,
                     "consumer": "none",
                 }
             )
+            traceback.print_exc()
             logger.error(f"Exception: {e}")
             return (
                 f"Exit due to exception: {e}",
                 "exit_error",
                 f"exit due to exception: {e}",
             )
 
@@ -278,15 +292,15 @@
 """
 
             user_prompt_template = f"""<OBSERVATION>
         {observation}
         </OBSERVATION>"""
 
             self.history.append({"role": "user", "content": user_prompt_template})
-            logger.info(self.history[-1]["content"])
+            # logger.info(self.history[-1]["content"])
             output = self.current_model.query(self.history, system_prompt_template)
 
             thought, action = parse_response(output)
 
             self.history.append({"role": "assistant", "content": output})
 
             return thought, action, output
@@ -324,14 +338,17 @@
             observations = list()
             if action == "exit":
                 done = True
 
             try:
                 # assert output.count("<COMMAND>") == 1
                 # assert output.count("<THOUGHT>") == 1
+                output, done = self.parse_command_to_function(
+                    command_string=action
+                )
                 obs, done = env.step(action, thought)
             except AssertionError as e:
                 # logger.error(output)
                 logger.error(e)
                 obs = str(e)
             except Exception as e:
                 raise e
```

### Comparing `devon_agent-0.1.6/devon_agent/prompt.py` & `devon_agent-0.1.7/devon_agent/prompt.py`

 * *Files identical despite different names*

### Comparing `devon_agent-0.1.6/devon_agent/retrieval/ast_extractor.py` & `devon_agent-0.1.7/devon_agent/retrieval/ast_extractor.py`

 * *Files identical despite different names*

### Comparing `devon_agent-0.1.6/devon_agent/retrieval/ast_parser.py` & `devon_agent-0.1.7/devon_agent/retrieval/ast_parser.py`

 * *Files identical despite different names*

### Comparing `devon_agent-0.1.6/devon_agent/retrieval/codebase_graph.py` & `devon_agent-0.1.7/devon_agent/retrieval/codebase_graph.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import json
 import networkx as nx
 
 def create_graph():
     """
     Creates a new directed graph for representing the Python codebase.
     Returns:
         nx.DiGraph: The created graph.
@@ -168,8 +169,80 @@
     Args:
         graph (nx.DiGraph): The graph to search.
         source (str): The source node.
         target (str): The target node.
     Returns:
         list: All paths from source to target.
     """
-    return list(nx.all_simple_paths(graph, source, target))
+    return list(nx.all_simple_paths(graph, source, target))
+
+
+class CodeGraph:
+
+    def __init__(self, graph=None):
+        """
+        Creates a new directed graph for representing the Python codebase.
+        Returns:
+            nx.DiGraph: The created graph.
+        """
+        if graph is not None:
+            self.graph = graph
+        else:
+            graph = nx.DiGraph(name="Python Codebase Graph")
+            graph.graph["node_attrs"] = {
+                "type": None,
+                "code": None,
+                "doc": None,
+                "location": {
+                    "file_path": None,
+                    "start_line": None,
+                    "end_line": None,
+                },
+                "dependencies": {
+                    "imports": [],
+                    "exported": [],
+                },
+            }
+            graph.graph["edge_types"] = {
+                "calls": {
+                    "ref_location": {
+                        "file_path": None,
+                        "line_number": None,
+                    }
+                },
+                "imports": {
+                    "ref_location": {
+                        "file_path": None,
+                        "line_number": None,
+                    }
+                },
+            }
+            graph.graph["total_nodes"] = 0
+            graph.graph["total_edges"] = 0
+            graph.graph["disconnected_components"] = []
+
+            self.graph : nx.DiGraph = graph
+
+    def to_json(self):
+        from networkx.readwrite import json_graph
+
+        jg = json_graph.adjacency_data(self.graph)
+        return jg
+
+    @classmethod
+    def from_json_dict(cls,json_dict):
+        from networkx.readwrite import json_graph
+
+
+        graph = json_graph.adjacency_graph(json_dict)
+        return cls(graph)
+    
+    @classmethod
+    def from_json(cls,json_str):
+        from networkx.readwrite import json_graph
+
+        jg = json.loads(json_str)
+        graph = json_graph.adjacency_graph(jg)
+        return cls(graph)
+    
+
+
```

### Comparing `devon_agent-0.1.6/devon_agent/retrieval/file_discovery.py` & `devon_agent-0.1.7/devon_agent/retrieval/file_discovery.py`

 * *Files 16% similar despite different names*

```diff
@@ -18,10 +18,11 @@
     python_files = []
     for root, dirs, files in os.walk(root_dir):
         # Remove ignored directories from the dirs list
         dirs[:] = [d for d in dirs if d not in ignore_dirs]
 
         for file in files:
             if file.endswith(".py"):
+                print(f"discovered {os.path.join(root, file)}")
                 python_files.append(os.path.join(root, file))
 
     return python_files
```

### Comparing `devon_agent-0.1.6/devon_agent/retrieval/graph_visualization.py` & `devon_agent-0.1.7/devon_agent/retrieval/graph_visualization.py`

 * *Files identical despite different names*

### Comparing `devon_agent-0.1.6/devon_agent/retrieval/main.py` & `devon_agent-0.1.7/devon_agent/retrieval/main.py`

 * *Files identical despite different names*

### Comparing `devon_agent-0.1.6/devon_agent/server.py` & `devon_agent-0.1.7/devon_agent/server.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import asyncio
 import json
 import os
 from time import sleep
 from typing import Dict, List
 
 import fastapi
-from devon_agent.agent import TaskAgent
+from devon_agent.agents.default.agent import TaskAgent
 from devon_agent.session import (
     Event,
     Session,
     SessionArguments,
 )
 from fastapi.middleware.cors import CORSMiddleware
 
@@ -32,18 +32,14 @@
 origins = [
     "http://localhost:3000",
     "http://127.0.0.1:3000",
 ]
 
 sessions: Dict[str, Session] = {}
 
-
-API_KEY = None
-
-
 app = fastapi.FastAPI()
 
 app.add_middleware(
     CORSMiddleware,
     allow_origins=origins,
     allow_credentials=True,
     allow_methods=["*"],
@@ -85,22 +81,22 @@
 @app.post("/session")
 def create_session(session: str, path: str):
     if not os.path.exists(path):
         raise fastapi.HTTPException(status_code=404, detail="Path not found")
 
     agent = TaskAgent(
         name="Devon",
-        model="claude-opus",
+        model=app.model,
         temperature=0.0,
-        api_key=API_KEY,
+        api_key=app.api_key,
     )
     sessions[session] = Session(
         SessionArguments(
             path,
-            environment="local",
+            # environment="local",
             user_input=lambda: get_user_input(session),
             name=session,
         ),
         agent,
     )
 
     return session
@@ -119,15 +115,15 @@
         Event(
             type="Task",
             content="ask user for what to do",
             producer="system",
             consumer="devon",
         )
     )
-    background_tasks.add_task(sessions[session].step_event)
+    background_tasks.add_task(sessions[session].run_event_loop)
     running_sessions.append(session)
     return session
 
 
 @app.post("/session/{session}/response")
 def create_response(session: str, response: str):
     if session not in sessions:
@@ -216,16 +212,20 @@
     port = 8000  # Default port
     if len(sys.argv) > 1:
         try:
             port = int(sys.argv[1])
         except ValueError:
             print("Warning: Invalid port number provided. Using default port 8000.")
 
-        try:
-            API_KEY = sys.argv[2]
-        except IndexError:
-            if os.environ.get("ANTHROPIC_API_KEY"):
-                api_key = os.environ.get("ANTHROPIC_API_KEY")
-            else:
-                raise ValueError("API key not provided.")
+        if os.environ.get("OPENAI_API_KEY"):
+            app.api_key = os.environ.get("OPENAI_API_KEY")
+            app.model = "gpt4-o"
+        elif os.environ.get("ANTHROPIC_API_KEY"):
+            app.api_key = os.environ.get("ANTHROPIC_API_KEY")
+            app.model = "claude-opus"
+        else:
+            raise ValueError("API key not provided.")
+
+        if os.environ.get("DEVON_MODEL"):
+            app.model = os.environ.get("DEVON_MODEL")
 
     uvicorn.run(app, host="0.0.0.0", port=port)
```

### Comparing `devon_agent-0.1.6/devon_agent/session.py` & `devon_agent-0.1.7/devon_agent/session.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,49 +1,36 @@
 import inspect
 import json
 import logging
 import os
 import traceback
 from dataclasses import dataclass
-from typing import Any, List
+from typing import Any, Dict, List, Optional
 from devon_agent.agent import TaskAgent
-from devon_agent.environment import LocalEnvironment
+from devon_agent.environment import EnvironmentModule, LocalEnvironment, UserEnvironment
 from devon_agent.telemetry import Posthog, SessionEventEvent, SessionStartEvent
+from devon_agent.tool import  ToolNotFoundException
 from devon_agent.tools import (
-    ask_user,
-    close_file,
-    create_file,
-    delete_file,
-    edit_file,
-    exit,
-    extract_signature_and_docstring,
-    find_class,
-    find_file,
-    find_function,
-    get_cwd,
-    list_dirs_recursive,
-    no_op,
-    open_file,
     parse_command,
-    real_write_diff,
-    scroll_down,
-    scroll_to_line,
-    scroll_up,
-    search_dir,
-    search_file,
-    set_task,
-    submit,
 )
+from devon_agent.tools.editortools import CreateFileTool, DeleteFileTool, OpenFileTool, ScrollDownTool, ScrollToLineTool, ScrollUpTool
+from devon_agent.tools.edittools import EditFileTool
+from devon_agent.tools.filesearchtools import FindFileTool, GetCwdTool, ListDirsRecursiveTool, SearchDirTool
+from devon_agent.tools.filetools import SearchFileTool
+from devon_agent.tools.lifecycle import NoOpTool, SubmitTool
+from devon_agent.tools.shelltool import ShellTool
+from devon_agent.tools.usertools import AskUserTool
+
 from devon_agent.utils import DotDict, Event
 
 
 @dataclass(frozen=False)
 class SessionArguments:
     path: str
-    environment: str
+    # environments: List[str]
     user_input: Any
     name: str
 
 
 """
 The Event System
 
@@ -122,46 +109,57 @@
         self.base_path = args.path
         self.event_log: List[Event] = []
         self.event_index = 0
         self.get_user_input = args.user_input
         self.telemetry_client = Posthog()
         self.name = args.name
 
-        self.state.editor = {}
+        local_environment = LocalEnvironment(args.path)
+        local_environment.register_tools({
+            "create_file" : CreateFileTool(),
+            "open_file" : OpenFileTool(),
+            "scroll_up" : ScrollUpTool(),
+            "scroll_down" : ScrollDownTool(),
+            "scroll_to_line" : ScrollToLineTool(),
+            "search_file" : SearchFileTool(),
+            "edit_file" : EditFileTool(),
+            "search_dir" : SearchDirTool(),
+            "find_file" : FindFileTool(),
+            # "list_dirs_recursive" : ListDirsRecursiveTool(),
+            "get_cwd" : GetCwdTool(),
+            "no_op" : NoOpTool(),
+            "submit" : SubmitTool(),
+            "delete_file" : DeleteFileTool(),
+        })
+        local_environment.set_default_tool(ShellTool())
+        self.default_environment = local_environment
+
+        user_environment = UserEnvironment(args.user_input)
+
+        user_environment.register_tools({
+            "ask_user" : AskUserTool(),
+        })
+
+        self.environments = {
+            "local" : local_environment,
+            "user" : user_environment,
+        }
+
+
 
         self.path = args.path
-        self.environment_type = args.environment
+        self.base_path = args.path
+        # self.environment_type = args.environment
+
+        # if args.environment == "local":
+        #     self.default_environment = LocalEnvironment(args.path)
+        # else:
+        #     raise ValueError("Unknown environment type")
+
 
-        if args.environment == "local":
-            self.environment = LocalEnvironment(args.path)
-        else:
-            raise ValueError("Unknown environment type")
-
-        self.tools = [
-            list_dirs_recursive,
-            close_file,
-            create_file,
-            open_file,
-            search_dir,
-            # find_function,
-            # find_class,
-            search_file,
-            get_cwd,
-            delete_file,
-            submit,
-            no_op,
-            scroll_up,
-            scroll_down,
-            scroll_to_line,
-            find_file,
-            ask_user,
-            exit,
-            edit_file,
-            # set_task
-        ]
 
     def to_dict(self):
         return {
             "path": self.path,
             "environment": self.environment_type,
             "event_history": [event for event in self.event_log],
             "state": self.state.to_dict(),
@@ -193,290 +191,342 @@
         instance.state = DotDict(data["state"])
         instance.state.editor = {}
         instance.event_log = data["event_history"]
         instance.environment.communicate("cd " + data["cwd"])
 
         return instance
 
-    def step(self, action: str, thought: str) -> tuple[str, bool]:
-        # parse command
-        # run command/tool
-        # return reponse as observation
-
-        if action == "exit":
-            return "Exited task", True
-
-        try:
-            return self.parse_command_to_function(command_string=action)
-        except Exception as e:
-            return e.args[0], False
+    # def step(self, action: str, thought: str) -> tuple[str, bool]:
+    #     # parse command
+    #     # run command/tool
+    #     # return reponse as observation
+
+    #     if action == "exit":
+    #         return "Exited task", True
+
+    #     try:
+    #         return self.parse_command_to_function(command_string=action)
+    #     except Exception as e:
+    #         return e.args[0], False
 
     def get_last_task(self):
         for event in self.event_log[::-1]:
             if event["type"] == "Task":
                 return event["content"]
         return "Task unspecified ask user to specify task"
-
-    def step_event(self):
-        if self.event_index == len(self.event_log):
-            return "No more events to process", True
-        event = self.event_log[self.event_index]
-        self.logger.info(f"Event: {event}")
-        self.logger.info(f"State: {self.state.editor}")
-
-        # Collect only event name and content only in case of error
-        telemetry_event = SessionEventEvent(
-            event_type=event["type"],
-            message="" if not event["type"] == "Error" else event["content"],
-        )
-        self.telemetry_client.capture(telemetry_event)
-        if event["type"] == "Error":
-            self.event_log.append(
-                {
-                    "type": "Stop",
-                    "content": "Stopped task",
-                    "producer": event["producer"],
-                    "consumer": "user",
-                }
+    
+    def run_event_loop(self):
+        event_id = 0
+        #current event
+        while True and not (event_id == len(self.event_log)):
+
+            event = self.event_log[event_id]
+
+            self.logger.info(f"Event: {event}")
+            self.logger.info(f"State: {self.state}")
+
+            # Collect only event name and content only in case of error
+            telemetry_event = SessionEventEvent(
+                event_type=event["type"],
+                message="" if not event["type"] == "Error" else event["content"],
             )
 
-        if event["type"] == "ModelRequest":
-            thought, action, output = self.agent.predict(
-                self.get_last_task(), event["content"], self
-            )
-            self.event_log.append(
-                {
-                    "type": "ModelResponse",
-                    "content": json.dumps(
-                        {"thought": thought, "action": action, "output": output}
-                    ),
-                    "producer": self.agent.name,
-                    "consumer": event["producer"],
-                }
-            )
+            self.telemetry_client.capture(telemetry_event)
 
-        if event["type"] == "ToolRequest":
-            tool_name, args = parse_command(self, event["content"])
+            if event["type"] == "Stop":
+                break
 
-            if tool_name == "ask_user":
-                self.event_log.append(
-                    {
-                        "type": "UserRequest",
-                        "content": args[0],
-                        "producer": event["producer"],
-                        "consumer": "user",
-                    }
-                )
-            elif tool_name in ["submit", "exit", "stop", "exit_error","exit_api",]:
-                self.event_log.append(
+            events = self.step_event(event)
+            self.event_log.extend(events)
+
+            event_id += 1
+            
+
+    def step_event(self, event):
+        
+        new_events = []
+        match event["type"]:
+            case "Error":
+                new_events.append(
                     {
                         "type": "Stop",
                         "content": "Stopped task",
                         "producer": event["producer"],
                         "consumer": "user",
                     }
                 )
-            elif tool_name == "set_task":
-                self.event_log.append(
-                    {
-                        "type": "Task",
-                        "content": args[0],
-                        "producer": event["producer"],
-                        "consumer": self.agent.name,
-                    }
+
+            case "ModelRequest":
+                thought, action, output = self.agent.predict(
+                    self.get_last_task(), event["content"], self
                 )
-            elif tool_name == "send_message":
-                self.event_log.append(
-                    {
-                        "type": "ModelRequest",
-                        "content": args[1],
-                        "producer": event["producer"],
-                        "consumer": args[0],
+                if action == "hallucination":
+                    new_events.append(
+                        {
+                            "type": "ModelRequest",
+                            "content": output,
+                            "producer": self.agent.name,
+                            "consumer": event["producer"],
+                        }
+                    )
+                else:
+                    new_events.append(
+                        {
+                        "type": "ModelResponse",
+                        "content": json.dumps(
+                            {"thought": thought, "action": action, "output": output}
+                        ),
+                        "producer": self.agent.name,
+                        "consumer": event["producer"],
                     }
                 )
 
-            else:
-                output, done = self.parse_command_to_function(
-                    command_string=event["content"]
-                )
-                self.event_log.append(
+            case "ToolRequest":
+                tool_name, args = event["content"]["toolname"], event["content"]["args"]
+
+                match tool_name:
+                    case "submit" | "exit" | "stop" | "exit_error" | "exit_api":
+                        new_events.append(
+                            {
+                                "type": "Stop",
+                                "content": "Stopped task",
+                                "producer": event["producer"],
+                                "consumer": "user",
+                            }
+                        )
+                    case "set_task":
+                        new_events.append(
+                            {
+                                "type": "Task",
+                                "content": args[0],
+                                "producer": event["producer"],
+                                "consumer": self.agent.name,
+                            }
+                        )
+                    case _:        
+                        try:
+
+                            toolname = event["content"]["toolname"]
+                            args = event["content"]["args"]
+                            raw_command = event["content"]["raw_command"]
+
+                            env = None
+
+                            for _env in list(self.environments.values()):
+                                if toolname in _env.tools:
+                                    env = _env
+                            
+                            if not env:
+                                raise ToolNotFoundException(toolname, self.environments)
+
+                            response = env.tools[toolname]({
+                                "environment": env,
+                                "session": self,
+                                "state": self.state,
+                                "raw_command": raw_command
+                            }, *args)
+
+
+                            new_events.append(
+                                {
+                                    "type": "ToolResponse",
+                                    "content": response,
+                                    "producer": toolname,
+                                    "consumer": event["producer"],
+                                }
+                            )
+
+                        except ToolNotFoundException as e:
+                            
+                            if not (self.default_environment and self.default_environment.default_tool):
+                                raise e
+                            
+                            try:
+                        
+                                response  = self.default_environment.default_tool({
+                                    "state" : self.state,
+                                    "environment" : self.default_environment,
+                                    "session" : self,
+                                    "raw_command" : event["content"]["raw_command"],
+                                }, event["content"]["toolname"], event["content"]["args"])
+
+                                new_events.append(
+                                    {
+                                        "type": "ToolResponse",
+                                        "content": response,
+                                        "producer": self.default_environment.name,
+                                        "consumer": event["producer"],
+                                    }
+                                )
+                            except Exception as e:
+                                self.logger.error(traceback.format_exc())
+                                self.logger.error(f"Error routing tool call: {e}")
+                                new_events.append(
+                                    {
+                                        "type": "ToolResponse",
+                                        "content": f"Error calling command, command failed with: {e.args[0] if len(e.args) > 0 else 'unknown'}",
+                                        "producer": self.default_environment.name,
+                                        "consumer": event["producer"],
+                                    }
+                                )
+                        except Exception as e:
+                            self.logger.error(traceback.format_exc())
+                            self.logger.error(f"Error routing tool call: {e}")
+                            new_events.append(
+                                {
+                                    "type": "ToolResponse",
+                                    "content": e.args[0],
+                                    "producer": self.default_environment.name,
+                                    "consumer": event["producer"],
+                                }
+                            )
+
+            case "ToolResponse":
+                new_events.append(
                     {
-                        "type": "EnvironmentRequest",
+                        "type": "ModelRequest",
                         "content": event["content"],
                         "producer": event["producer"],
-                        "consumer": self.environment.__class__.__name__,
-                    }
-                )
-                self.event_log.append(
-                    {
-                        "type": "EnvironmentResponse",
-                        "content": output,
-                        "producer": self.environment.__class__.__name__,
                         "consumer": event["consumer"],
                     }
                 )
-                self.event_log.append(
+
+            case "ModelResponse":
+                content = json.loads(event["content"])["action"]
+                toolname, args = parse_command(content)
+                new_events.append(
                     {
-                        "type": "ToolResponse",
-                        "content": output,
-                        "producer": self.environment.__class__.__name__,
+                        "type": "ToolRequest",
+                        "content": {
+                            "toolname" : toolname,
+                            "args" : args,
+                            "raw_command" : content
+                        },
+                        "producer": event["producer"],
                         "consumer": event["consumer"],
                     }
                 )
 
-        if event["type"] == "EnvironmentRequest":
-            pass
-
-        if event["type"] == "EnvironmentResponse":
-            pass
-
-        if event["type"] == "ToolResponse":
-            self.event_log.append(
-                {
-                    "type": "ModelRequest",
-                    "content": event["content"],
-                    "producer": event["producer"],
-                    "consumer": event["consumer"],
-                }
-            )
-
-        if event["type"] == "ModelResponse":
-            content = json.loads(event["content"])["action"]
-            self.event_log.append(
-                {
-                    "type": "ToolRequest",
-                    "content": content,
-                    "producer": event["producer"],
-                    "consumer": event["consumer"],
-                }
-            )
+            case "Interrupt":
+                if self.agent.interrupt:
+                    self.agent.interrupt += (
+                        "You have been interrupted, pay attention to this message "
+                        + event["content"]
+                    )
+                else:
+                    self.agent.interrupt = event["content"]
+
+            case "Task":
+                task = event["content"]
+                self.logger.info(f"Task: {task}")
+                if task is None:
+                    task = "Task unspecified ask user to specify task"
 
-        if event["type"] == "UserRequest":
-            user_input = self.get_user_input()
-            if user_input is None:
-                self.logger.info("No user input provided")
-                self.event_log.append(
+                new_events.append(
                     {
-                        "type": "Stop",
-                        "content": "No user input provided",
-                        "producer": "user",
+                        "type": "ModelRequest",
+                        "content": "",
+                        "producer": event["producer"],
                         "consumer": event["consumer"],
                     }
                 )
-                return "No user input provided", True
+            case _:
+                pass
 
-            self.event_log.append(
-                {
-                    "type": "UserResponse",
-                    "content": user_input,
-                    "producer": "user",
-                    "consumer": event["producer"],
-                }
-            )
-            self.event_log.append(
-                {
-                    "type": "ToolResponse",
-                    "content": user_input,
-                    "producer": "user",
-                    "consumer": event["producer"],
-                }
-            )
-
-        if event["type"] == "Interrupt":
-            if self.agent.interrupt:
-                self.agent.interrupt += (
-                    "You have been interrupted, pay attention to this message "
-                    + event["content"]
-                )
-            else:
-                self.agent.interrupt = event["content"]
+        return new_events
 
-        if event["type"] == "Stop":
-            return "Stopped task", True
+    # def parse_command_to_function(self, command_string) -> tuple[str, bool]:
+    #     """
+    #     Parses a command string into its function name and arguments.
+    #     """
+    #     ctx = self
+
+    #     fn_name, args = parse_command(ctx, command_string)
+    #     if fn_name in ["vim", "nano"]:
+    #         return "Interactive Commands are not allowed", False
+
+    #     if (
+    #         fn_name == "python"
+    #         and len([line for line in command_string.splitlines() if line]) != 1
+    #     ):
+    #         return "Interactive Commands are not allowed", False
+
+    #     fn_names = [fn.__name__ for fn in self.tools]
+
+    #     try:
+    #         if fn_name == "edit_file":
+    #             try:
+    #                 return real_write_diff(self, command_string), False
+    #             except Exception as e:
+    #                 ctx.logger.error(traceback.print_exc())
+    #                 raise e
+    #         elif fn_name in fn_names:
+    #             for fn in self.tools:
+    #                 if fn.__name__ == fn_name:
+    #                     return fn(ctx, *args), False
+    #         else:
+    #             # try:
+    #             output, rc = ctx.environment.communicate(fn_name + " " + " ".join(args))
+    #             if rc != 0:
+    #                 raise Exception(output)
+    #             return output, False
+    #             # except Exception as e:
+    #             #     ctx.logger.error(
+    #             #         f"Failed to execute bash command '{fn_name}': {str(e)}"
+    #             #     )
+    #             #     return "Failed to execute bash command", False
+    #     except Exception as e:
+    #         ctx.logger.error(traceback.print_exc())
+    #         return e.args[0] if len(e.args) > 0 else "Failed to execute command due to internal error", False
 
-        if event["type"] == "Task":
-            task = event["content"]
-            self.logger.info(f"Task: {task}")
-            if task is None:
-                task = "Task unspecified ask user to specify task"
-
-            self.event_log.append(
-                {
-                    "type": "ModelRequest",
-                    "content": "",
-                    "producer": event["producer"],
-                    "consumer": event["consumer"],
-                }
-            )
+    def get_available_actions(self) -> list[str]:
+        # get all tools for all environments
 
-        self.event_index += 1
-        return self.step_event()
+        tools = []
+        for env in self.environments.values():
+            tools.extend(env.tools)
 
-    def parse_command_to_function(self, command_string) -> tuple[str, bool]:
-        """
-        Parses a command string into its function name and arguments.
-        """
-        ctx = self
+        return tools
 
-        fn_name, args = parse_command(ctx, command_string)
-        if fn_name in ["vim", "nano"]:
-            return "Interactive Commands are not allowed", False
-
-        if (
-            fn_name == "python"
-            and len([line for line in command_string.splitlines() if line]) != 1
-        ):
-            return "Interactive Commands are not allowed", False
-
-        fn_names = [fn.__name__ for fn in self.tools]
-
-        try:
-            if fn_name == "edit_file":
-                try:
-                    return real_write_diff(self, command_string), False
-                except Exception as e:
-                    ctx.logger.error(traceback.print_exc())
-                    raise e
-            elif fn_name in fn_names:
-                for fn in self.tools:
-                    if fn.__name__ == fn_name:
-                        return fn(ctx, *args), False
-            else:
-                # try:
-                output, rc = ctx.environment.communicate(fn_name + " " + " ".join(args))
-                if rc != 0:
-                    raise Exception(output)
-                return output, False
-                # except Exception as e:
-                #     ctx.logger.error(
-                #         f"Failed to execute bash command '{fn_name}': {str(e)}"
-                #     )
-                #     return "Failed to execute bash command", False
-        except Exception as e:
-            ctx.logger.error(traceback.print_exc())
-            return e.args[0] if len(e.args) > 0 else "Failed to execute command due to internal error", False
 
-    def get_available_actions(self) -> list[str]:
-        return [fn.__name__ for fn in self.tools]
-
-    def generate_command_docs(self):
+    def generate_command_docs(self, format="manpage"):
         """
         Generates a dictionary of function names and their docstrings.
         """
-
-        funcs = self.tools
         docs = {}
-
-        for func in funcs:
-            name = func.__name__
-            code = inspect.getsource(func)
-            sig, docstring = extract_signature_and_docstring(code)
-            docs[name] = {"signature": sig, "docstring": docstring}
+        for env in self.environments.values():
+            for name,tool in env.tools.items():
+                signature = inspect.signature(tool.function)
+                docs[name] = {
+                    "docstring" : tool.documentation(format),
+                    "signature" : str(signature),
+                }
 
         return docs
 
+
     def enter(self):
+        print("Entering session")
+        print(self.environments)
+        for name, env in self.environments.items():
+            print("Setting up env")
+            env.setup(self)
+            for tool in env.tools.values():
+                print("Setting up tool")
+                tool.setup({
+                    "environment" : env,
+                    "session" : self,
+                    "state" : self.state,
+                })
+
         self.telemetry_client.capture(SessionStartEvent(self.name))
-        self.environment.setup()
+        
 
     def exit(self):
-        self.environment.teardown()
+        for env in self.environments.values():
+            env.teardown()
+            for tool in env.tools.values():
+                tool.setup({
+                    "environment" : env,
+                    "session" : self,
+                    "state" : self.state,
+                })
```

### Comparing `devon_agent-0.1.6/devon_agent/telemetry.py` & `devon_agent-0.1.7/devon_agent/telemetry.py`

 * *Files 0% similar despite different names*

```diff
@@ -135,15 +135,15 @@
         self.batched_events[batch_key] = batched_event
         if batched_event.batch_size >= batched_event.max_batch_size:
             self._direct_capture(batched_event)
             del self.batched_events[batch_key]
 
     def _direct_capture(self, event: ProductTelemetryEvent) -> None:
         try:
-            print(event.name)
+            # print(event.name)
             result = posthog.capture(
                 self.user_id,
                 event.name,
                 {**event.properties, **self.context},
             )
             print(result)
         except Exception as e:
```

### Comparing `devon_agent-0.1.6/devon_agent/test/test_tools.py` & `devon_agent-0.1.7/devon_agent/test/test_tools.py`

 * *Files identical despite different names*

### Comparing `devon_agent-0.1.6/devon_agent/udiff.py` & `devon_agent-0.1.7/devon_agent/udiff.py`

 * *Files identical despite different names*

### Comparing `devon_agent-0.1.6/devon_agent/utils.py` & `devon_agent-0.1.7/devon_agent/utils.py`

 * *Files identical despite different names*

### Comparing `devon_agent-0.1.6/devon_agent/vgit.py` & `devon_agent-0.1.7/devon_agent/vgit.py`

 * *Files identical despite different names*

### Comparing `devon_agent-0.1.6/pyproject.toml` & `devon_agent-0.1.7/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "devon-agent"
-version = "0.1.6"
+version = "0.1.7"
 description = ""
 authors = ["killind-dev <61808204+killind-dev@users.noreply.github.com>","mihir1003 <mihir1003@gmail.com>"]
 readme = "README.md"
 exclude = [
     "devon_tui",
 ]
 
@@ -28,17 +28,20 @@
 tenacity = "^8.2.2"
 simple-parsing = {version = "^0.1.5", optional = true}
 swebench = {version = "1.0.1", optional = true}
 gymnasium = {version = "^0.29.1", optional = true}
 datasets = {version = ">=2.14.6,<2.15.0", optional = true}
 click = "^8.1.7"
 posthog = "^3.5.0"
+litellm = "^1.37.9"
+dspy-ai = {version = "^2.4.9", optional = true}
 
 [tool.poetry.extras]
 swebench = ["swebench", "datasets", "gymnasium"]
+experimental = ["dspy-ai"]
 
 [tool.poetry.group.dev.dependencies]
 ruff = "^0.3.3"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `devon_agent-0.1.6/PKG-INFO` & `devon_agent-0.1.7/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,28 +1,31 @@
 Metadata-Version: 2.1
 Name: devon-agent
-Version: 0.1.6
+Version: 0.1.7
 Summary: 
 Author: killind-dev
 Author-email: 61808204+killind-dev@users.noreply.github.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
+Provides-Extra: experimental
 Provides-Extra: swebench
 Requires-Dist: anthropic (>=0.20.0,<0.21.0)
 Requires-Dist: astroid (>=3.1.0,<4.0.0)
 Requires-Dist: click (>=8.1.7,<9.0.0)
 Requires-Dist: datasets (>=2.14.6,<2.15.0) ; extra == "swebench"
 Requires-Dist: docker (>=7.0.0,<8.0.0)
+Requires-Dist: dspy-ai (>=2.4.9,<3.0.0) ; extra == "experimental"
 Requires-Dist: fastapi (>=0.110.3,<0.111.0)
 Requires-Dist: ghapi (>=1.0.5,<2.0.0)
 Requires-Dist: gitpython (>=3.1.42,<4.0.0)
 Requires-Dist: gymnasium (>=0.29.1,<0.30.0) ; extra == "swebench"
+Requires-Dist: litellm (>=1.37.9,<2.0.0)
 Requires-Dist: networkx (>=3.3,<4.0)
 Requires-Dist: openai (>=1.14.1,<2.0.0)
 Requires-Dist: posthog (>=3.5.0,<4.0.0)
 Requires-Dist: pydantic (>=2.5.0,<3.0.0)
 Requires-Dist: pylint (>=3.1.0,<4.0.0)
 Requires-Dist: pytest (>=8.1.1,<9.0.0)
 Requires-Dist: pytest-json-report (>=1.5.0,<2.0.0)
@@ -44,30 +47,29 @@
   <a href="https://github.com/entropy-research/Devon/network/members"><img src="https://img.shields.io/github/forks/entropy-research/devon?style=for-the-badge&color=orange" alt="Forks"></a>
   <a href="https://github.com/entropy-research/Devon/stargazers"><img src="https://img.shields.io/github/stars/entropy-research/devon?style=for-the-badge&color=yellow" alt="Stargazers"></a>
   <a href="https://github.com/entropy-research/Devon/issues"><img src="https://img.shields.io/github/issues/entropy-research/devon?style=for-the-badge&color=red" alt="Issues"></a>
   <br/>
   <a href="https://github.com/entropy-research/Devon/blob/main/LICENSE"><img src="https://img.shields.io/github/license/entropy-research/devon?style=for-the-badge&color=blue" alt="Apache 2.0 License"></a>
   <a href="https://discord.gg/p5YpZ5vjd9"><img src="https://img.shields.io/badge/Discord-Join%20Us-purple?logo=discord&logoColor=white&style=for-the-badge" alt="Join our Discord community"></a>
   <br/>
-</div>
-
 
-> Video/GIF Coming Soon!
+https://github.com/entropy-research/Devon/assets/61808204/d42a8b9a-0211-4624-9804-d24df1d4dbf6
+</div>
 
 # Installation
 
 ## Prerequisites
 
 1. `node.js` and `npm`
 2. `pipx`, if you don't have this go [here](https://pipx.pypa.io/stable/installation/)
-3. [**Anthropic**](https://console.anthropic.com/settings/keys) API Key
+3. [**Anthropic**](https://console.anthropic.com/settings/keys) API Key or [**OpenAI**](https://platform.openai.com/api-keys) API key
 
 ## Installation commands
 
-To use, simply run:
+To install, simply run:
 
 ```bash
 curl -sSL https://raw.githubusercontent.com/entropy-research/Devon/main/install.sh | bash
 ```
 
 
 *Or to install using `pipx` + `npm`:*
@@ -78,33 +80,42 @@
 ```
 
 This installs the Python backend, and the cli command to run the tool
 
 ### Thats it! Happy building :)
 
 
-# Usage
+# Running the agent
 Navigate to your project folder and open the terminal.
 
-Set your Anthropic API key as an environment variable:
+Set your Anthropic API or OpenAI API key as an environment variable:
 
 ```bash
 export ANTHROPIC_API_KEY=sk-xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx
+
+#OR
+
+export OPENAI_API_KEY=sk-xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx
 ```
 
 Then to *run*, the command is:
 ```bash
 devon
 ```
 
 It's as easy as that.
 
 > [!NOTE]
 > Don't worry, the agent will be able to only access files and folders in the directory you started it from. You can also correct it while it's performing actions.
 
+To run in *debug* mode, the command is:
+```bash
+devon --debug
+```
+
 # Features
 - Multi-file editing
 - Codebase exploration
 - Config writing
 - Test writing
 - Bug fixing
 - Architecture exploration
```

#### html2text {}

```diff
@@ -1,44 +1,51 @@
-Metadata-Version: 2.1 Name: devon-agent Version: 0.1.6 Summary: Author:
+Metadata-Version: 2.1 Name: devon-agent Version: 0.1.7 Summary: Author:
 killind-dev Author-email: 61808204+killind-dev@users.noreply.github.com
 Requires-Python: >=3.10,<4.0 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3.11 Classifier: Programming Language :: Python :: 3.12
-Provides-Extra: swebench Requires-Dist: anthropic (>=0.20.0,<0.21.0) Requires-
-Dist: astroid (>=3.1.0,<4.0.0) Requires-Dist: click (>=8.1.7,<9.0.0) Requires-
-Dist: datasets (>=2.14.6,<2.15.0) ; extra == "swebench" Requires-Dist: docker
-(>=7.0.0,<8.0.0) Requires-Dist: fastapi (>=0.110.3,<0.111.0) Requires-Dist:
-ghapi (>=1.0.5,<2.0.0) Requires-Dist: gitpython (>=3.1.42,<4.0.0) Requires-
-Dist: gymnasium (>=0.29.1,<0.30.0) ; extra == "swebench" Requires-Dist:
-networkx (>=3.3,<4.0) Requires-Dist: openai (>=1.14.1,<2.0.0) Requires-Dist:
-posthog (>=3.5.0,<4.0.0) Requires-Dist: pydantic (>=2.5.0,<3.0.0) Requires-
-Dist: pylint (>=3.1.0,<4.0.0) Requires-Dist: pytest (>=8.1.1,<9.0.0) Requires-
-Dist: pytest-json-report (>=1.5.0,<2.0.0) Requires-Dist: simple-parsing
-(>=0.1.5,<0.2.0) Requires-Dist: sqlalchemy (>=2.0.30,<3.0.0) Requires-Dist:
-swebench (==1.0.1) ; extra == "swebench" Requires-Dist: tenacity
-(>=8.2.2,<9.0.0) Requires-Dist: uvicorn (>=0.29.0,<0.30.0) Requires-Dist:
-xmltodict (>=0.13.0,<0.14.0) Description-Content-Type: text/markdown
+Provides-Extra: experimental Provides-Extra: swebench Requires-Dist: anthropic
+(>=0.20.0,<0.21.0) Requires-Dist: astroid (>=3.1.0,<4.0.0) Requires-Dist: click
+(>=8.1.7,<9.0.0) Requires-Dist: datasets (>=2.14.6,<2.15.0) ; extra ==
+"swebench" Requires-Dist: docker (>=7.0.0,<8.0.0) Requires-Dist: dspy-ai
+(>=2.4.9,<3.0.0) ; extra == "experimental" Requires-Dist: fastapi
+(>=0.110.3,<0.111.0) Requires-Dist: ghapi (>=1.0.5,<2.0.0) Requires-Dist:
+gitpython (>=3.1.42,<4.0.0) Requires-Dist: gymnasium (>=0.29.1,<0.30.0) ; extra
+== "swebench" Requires-Dist: litellm (>=1.37.9,<2.0.0) Requires-Dist: networkx
+(>=3.3,<4.0) Requires-Dist: openai (>=1.14.1,<2.0.0) Requires-Dist: posthog
+(>=3.5.0,<4.0.0) Requires-Dist: pydantic (>=2.5.0,<3.0.0) Requires-Dist: pylint
+(>=3.1.0,<4.0.0) Requires-Dist: pytest (>=8.1.1,<9.0.0) Requires-Dist: pytest-
+json-report (>=1.5.0,<2.0.0) Requires-Dist: simple-parsing (>=0.1.5,<0.2.0)
+Requires-Dist: sqlalchemy (>=2.0.30,<3.0.0) Requires-Dist: swebench (==1.0.1) ;
+extra == "swebench" Requires-Dist: tenacity (>=8.2.2,<9.0.0) Requires-Dist:
+uvicorn (>=0.29.0,<0.30.0) Requires-Dist: xmltodict (>=0.13.0,<0.14.0)
+Description-Content-Type: text/markdown
               ************ DDeevvoonn:: AAnn ooppeenn--ssoouurrccee ppaaiirr pprrooggrraammmmeerr ************
                    _[_C_o_n_t_r_i_b_u_t_o_r_s_]_[_F_o_r_k_s_]_[_S_t_a_r_g_a_z_e_r_s_]_[_I_s_s_u_e_s_]
                _[_A_p_a_c_h_e_ _2_._0_ _L_i_c_e_n_s_e_]_[_J_o_i_n_ _o_u_r_ _D_i_s_c_o_r_d_ _c_o_m_m_u_n_i_t_y_]
-> Video/GIF Coming Soon! # Installation ## Prerequisites 1. `node.js` and `npm`
-2. `pipx`, if you don't have this go [here](https://pipx.pypa.io/stable/
-installation/) 3. [**Anthropic**](https://console.anthropic.com/settings/keys)
-API Key ## Installation commands To use, simply run: ```bash curl -sSL https://
+ https://github.com/entropy-research/Devon/assets/61808204/d42a8b9a-0211-4624-
+                               9804-d24df1d4dbf6
+# Installation ## Prerequisites 1. `node.js` and `npm` 2. `pipx`, if you don't
+have this go [here](https://pipx.pypa.io/stable/installation/) 3.
+[**Anthropic**](https://console.anthropic.com/settings/keys) API Key or
+[**OpenAI**](https://platform.openai.com/api-keys) API key ## Installation
+commands To install, simply run: ```bash curl -sSL https://
 raw.githubusercontent.com/entropy-research/Devon/main/install.sh | bash ``` *Or
 to install using `pipx` + `npm`:* ```bash pipx install devon_agent npm install
 -g devon-tui ``` This installs the Python backend, and the cli command to run
-the tool ### Thats it! Happy building :) # Usage Navigate to your project
-folder and open the terminal. Set your Anthropic API key as an environment
-variable: ```bash export ANTHROPIC_API_KEY=sk-
+the tool ### Thats it! Happy building :) # Running the agent Navigate to your
+project folder and open the terminal. Set your Anthropic API or OpenAI API key
+as an environment variable: ```bash export ANTHROPIC_API_KEY=sk-
+xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx #OR export OPENAI_API_KEY=sk-
 xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx ``` Then to *run*, the command is:
 ```bash devon ``` It's as easy as that. > [!NOTE] > Don't worry, the agent will
 be able to only access files and folders in the directory you started it from.
-You can also correct it while it's performing actions. # Features - Multi-file
-editing - Codebase exploration - Config writing - Test writing - Bug fixing -
+You can also correct it while it's performing actions. To run in *debug* mode,
+the command is: ```bash devon --debug ``` # Features - Multi-file editing -
+Codebase exploration - Config writing - Test writing - Bug fixing -
 Architecture exploration ### Limitations - Minimal functionality for non-Python
 languages - Sometimes have to specify the file where you want the change to
 happen # Progress ### This project is still super early and we would love your
 help to make it great! ### Current goals - Multi-model support - Launch plugin
 system for tool and agent builders - Create self-hostable Electron app - Set
 SOTA on [SWE-bench Lite](https://www.swebench.com/lite.html) > View our current
 thoughts on next steps [**here**](https://docs.google.com/document/d/e/2PACX-
```

