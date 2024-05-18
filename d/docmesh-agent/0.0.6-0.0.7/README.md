# Comparing `tmp/docmesh_agent-0.0.6.tar.gz` & `tmp/docmesh_agent-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "docmesh_agent-0.0.6.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "docmesh_agent-0.0.7.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `docmesh_agent-0.0.6.tar` & `docmesh_agent-0.0.7.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0       15 2024-05-10 12:01:09.706198 docmesh_agent-0.0.6/README.md
--rw-r--r--   0        0        0       22 2024-05-17 06:26:10.956419 docmesh_agent-0.0.6/docmesh_agent/__init__.py
--rw-r--r--   0        0        0     3757 2024-05-17 06:25:06.227662 docmesh_agent-0.0.6/docmesh_agent/agent.py
--rw-r--r--   0        0        0      136 2024-05-14 03:33:52.820396 docmesh_agent-0.0.6/docmesh_agent/embeddings/__init__.py
--rw-r--r--   0        0        0     1404 2024-05-14 03:33:17.744088 docmesh_agent-0.0.6/docmesh_agent/embeddings/embeddings.py
--rw-r--r--   0        0        0       88 2024-05-10 11:02:39.301355 docmesh_agent-0.0.6/docmesh_agent/parser/__init__.py
--rw-r--r--   0        0        0      788 2024-05-10 11:14:17.156634 docmesh_agent-0.0.6/docmesh_agent/parser/output_parser.py
--rw-r--r--   0        0        0      241 2024-05-16 11:24:43.283487 docmesh_agent-0.0.6/docmesh_agent/toolkit/__init__.py
--rw-r--r--   0        0        0      344 2024-05-16 11:24:22.979445 docmesh_agent-0.0.6/docmesh_agent/toolkit/common.py
--rw-r--r--   0        0        0      531 2024-05-10 11:17:03.765428 docmesh_agent-0.0.6/docmesh_agent/toolkit/entity.py
--rw-r--r--   0        0        0     1035 2024-05-16 03:38:06.823760 docmesh_agent-0.0.6/docmesh_agent/toolkit/paper.py
--rw-r--r--   0        0        0      625 2024-05-13 03:31:55.262732 docmesh_agent-0.0.6/docmesh_agent/toolkit/recommend.py
--rw-r--r--   0        0        0      940 2024-05-16 11:23:32.443342 docmesh_agent-0.0.6/docmesh_agent/tools/__init__.py
--rw-r--r--   0        0        0     1139 2024-05-16 10:38:39.849612 docmesh_agent-0.0.6/docmesh_agent/tools/base.py
--rw-r--r--   0        0        0      721 2024-05-17 03:08:13.917254 docmesh_agent-0.0.6/docmesh_agent/tools/common.py
--rw-r--r--   0        0        0     2021 2024-05-16 10:36:55.425382 docmesh_agent-0.0.6/docmesh_agent/tools/entity.py
--rw-r--r--   0        0        0     3936 2024-05-13 04:13:58.033801 docmesh_agent-0.0.6/docmesh_agent/tools/graph_tools.py
--rw-r--r--   0        0        0     8572 2024-05-16 10:44:03.526324 docmesh_agent-0.0.6/docmesh_agent/tools/paper.py
--rw-r--r--   0        0        0     4351 2024-05-16 11:14:29.378232 docmesh_agent-0.0.6/docmesh_agent/tools/recommend.py
--rw-r--r--   0        0        0      750 2024-05-17 06:25:49.500169 docmesh_agent-0.0.6/pyproject.toml
--rw-r--r--   0        0        0      677 1970-01-01 00:00:00.000000 docmesh_agent-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0       15 2024-05-10 12:01:09.706198 docmesh_agent-0.0.7/README.md
+-rw-r--r--   0        0        0       22 2024-05-17 11:20:58.971924 docmesh_agent-0.0.7/docmesh_agent/__init__.py
+-rw-r--r--   0        0        0     4223 2024-05-17 11:18:21.538679 docmesh_agent-0.0.7/docmesh_agent/agent.py
+-rw-r--r--   0        0        0      136 2024-05-14 03:33:52.820396 docmesh_agent-0.0.7/docmesh_agent/embeddings/__init__.py
+-rw-r--r--   0        0        0     1404 2024-05-14 03:33:17.744088 docmesh_agent-0.0.7/docmesh_agent/embeddings/embeddings.py
+-rw-r--r--   0        0        0       88 2024-05-10 11:02:39.301355 docmesh_agent-0.0.7/docmesh_agent/parser/__init__.py
+-rw-r--r--   0        0        0      788 2024-05-10 11:14:17.156634 docmesh_agent-0.0.7/docmesh_agent/parser/output_parser.py
+-rw-r--r--   0        0        0      241 2024-05-16 11:24:43.283487 docmesh_agent-0.0.7/docmesh_agent/toolkit/__init__.py
+-rw-r--r--   0        0        0      344 2024-05-16 11:24:22.979445 docmesh_agent-0.0.7/docmesh_agent/toolkit/common.py
+-rw-r--r--   0        0        0      531 2024-05-10 11:17:03.765428 docmesh_agent-0.0.7/docmesh_agent/toolkit/entity.py
+-rw-r--r--   0        0        0     1035 2024-05-16 03:38:06.823760 docmesh_agent-0.0.7/docmesh_agent/toolkit/paper.py
+-rw-r--r--   0        0        0      625 2024-05-13 03:31:55.262732 docmesh_agent-0.0.7/docmesh_agent/toolkit/recommend.py
+-rw-r--r--   0        0        0      940 2024-05-16 11:23:32.443342 docmesh_agent-0.0.7/docmesh_agent/tools/__init__.py
+-rw-r--r--   0        0        0     1139 2024-05-16 10:38:39.849612 docmesh_agent-0.0.7/docmesh_agent/tools/base.py
+-rw-r--r--   0        0        0      721 2024-05-17 03:08:13.917254 docmesh_agent-0.0.7/docmesh_agent/tools/common.py
+-rw-r--r--   0        0        0     2021 2024-05-16 10:36:55.425382 docmesh_agent-0.0.7/docmesh_agent/tools/entity.py
+-rw-r--r--   0        0        0     3936 2024-05-13 04:13:58.033801 docmesh_agent-0.0.7/docmesh_agent/tools/graph_tools.py
+-rw-r--r--   0        0        0     8572 2024-05-16 10:44:03.526324 docmesh_agent-0.0.7/docmesh_agent/tools/paper.py
+-rw-r--r--   0        0        0     4351 2024-05-16 11:14:29.378232 docmesh_agent-0.0.7/docmesh_agent/tools/recommend.py
+-rw-r--r--   0        0        0      750 2024-05-17 06:29:59.523015 docmesh_agent-0.0.7/pyproject.toml
+-rw-r--r--   0        0        0      677 1970-01-01 00:00:00.000000 docmesh_agent-0.0.7/PKG-INFO
```

### Comparing `docmesh_agent-0.0.6/docmesh_agent/agent.py` & `docmesh_agent-0.0.7/docmesh_agent/agent.py`

 * *Files 17% similar despite different names*

```diff
@@ -83,15 +83,22 @@
             if "actions" in chunk:
                 for action in chunk["actions"]:
                     msg = f"\n{TermColor.tool}[⚒︎ {action.tool}]: {action.tool_input}{TermColor.end}"
                     yield msg.encode()
             # observation
             elif "steps" in chunk:
                 for step in chunk["steps"]:
-                    msg = f"\n{TermColor.observation}[⌕ observation]: {step.observation}{TermColor.end}"
+                    # observations could be real long if encountered PDF content
+                    # so we truncate all obseravations over 2000 characters
+                    truncate_threshold = 2000
+                    if len(step.observation) > truncate_threshold:
+                        observation = f"\nbservation exceeds {truncate_threshold} characters and has been omitted...\n"
+                    else:
+                        observation = step.observation
+                    msg = f"\n{TermColor.observation}[⌕ observation]: {observation}{TermColor.end}"
                     yield msg.encode()
             # output
             elif "output" in chunk:
                 output = chunk["output"]
                 msg = f"\n{TermColor.output}[✔️ answer]: \n{output}{TermColor.end}\n"
                 yield msg.encode()
     except Exception as e:
```

### Comparing `docmesh_agent-0.0.6/docmesh_agent/embeddings/embeddings.py` & `docmesh_agent-0.0.7/docmesh_agent/embeddings/embeddings.py`

 * *Files identical despite different names*

### Comparing `docmesh_agent-0.0.6/docmesh_agent/parser/output_parser.py` & `docmesh_agent-0.0.7/docmesh_agent/parser/output_parser.py`

 * *Files identical despite different names*

### Comparing `docmesh_agent-0.0.6/docmesh_agent/toolkit/entity.py` & `docmesh_agent-0.0.7/docmesh_agent/toolkit/entity.py`

 * *Files identical despite different names*

### Comparing `docmesh_agent-0.0.6/docmesh_agent/toolkit/paper.py` & `docmesh_agent-0.0.7/docmesh_agent/toolkit/paper.py`

 * *Files identical despite different names*

### Comparing `docmesh_agent-0.0.6/docmesh_agent/toolkit/recommend.py` & `docmesh_agent-0.0.7/docmesh_agent/toolkit/recommend.py`

 * *Files identical despite different names*

### Comparing `docmesh_agent-0.0.6/docmesh_agent/tools/__init__.py` & `docmesh_agent-0.0.7/docmesh_agent/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `docmesh_agent-0.0.6/docmesh_agent/tools/base.py` & `docmesh_agent-0.0.7/docmesh_agent/tools/base.py`

 * *Files identical despite different names*

### Comparing `docmesh_agent-0.0.6/docmesh_agent/tools/common.py` & `docmesh_agent-0.0.7/docmesh_agent/tools/common.py`

 * *Files identical despite different names*

### Comparing `docmesh_agent-0.0.6/docmesh_agent/tools/entity.py` & `docmesh_agent-0.0.7/docmesh_agent/tools/entity.py`

 * *Files identical despite different names*

### Comparing `docmesh_agent-0.0.6/docmesh_agent/tools/graph_tools.py` & `docmesh_agent-0.0.7/docmesh_agent/tools/graph_tools.py`

 * *Files identical despite different names*

### Comparing `docmesh_agent-0.0.6/docmesh_agent/tools/paper.py` & `docmesh_agent-0.0.7/docmesh_agent/tools/paper.py`

 * *Files identical despite different names*

### Comparing `docmesh_agent-0.0.6/docmesh_agent/tools/recommend.py` & `docmesh_agent-0.0.7/docmesh_agent/tools/recommend.py`

 * *Files identical despite different names*

### Comparing `docmesh_agent-0.0.6/pyproject.toml` & `docmesh_agent-0.0.7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `docmesh_agent-0.0.6/PKG-INFO` & `docmesh_agent-0.0.7/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: docmesh_agent
-Version: 0.0.6
+Version: 0.0.7
 Summary: Agent helps you dig the paper connection!
 Author-email: Zhengkai Yang <kyle.yang1995@gmail.com>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

