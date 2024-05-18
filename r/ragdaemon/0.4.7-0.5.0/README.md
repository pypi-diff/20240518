# Comparing `tmp/ragdaemon-0.4.7.tar.gz` & `tmp/ragdaemon-0.5.0.tar.gz`

## Comparing `ragdaemon-0.4.7.tar` & `ragdaemon-0.5.0.tar`

### file list

```diff
@@ -1,78 +1,78 @@
--rw-r--r--   0        0        0     4401 2020-02-02 00:00:00.000000 ragdaemon-0.4.7/scratch.ipynb
--rw-r--r--   0        0        0    10345 2020-02-02 00:00:00.000000 ragdaemon-0.4.7/tutorial.ipynb
--rw-r--r--   0        0        0      653 2020-02-02 00:00:00.000000 ragdaemon-0.4.7/.github/workflows/run-tests.yml
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 ragdaemon-0.4.7/ragdaemon/__init__.py
--rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 ragdaemon-0.4.7/ragdaemon/__main__.py
--rw-r--r--   0        0        0     3742 2020-02-02 00:00:00.000000 ragdaemon-0.4.7/ragdaemon/app.py
--rw-r--r--   0        0        0    11164 2020-02-02 00:00:00.000000 ragdaemon-0.4.7/ragdaemon/context.py
--rw-r--r--   0        0        0     7824 2020-02-02 00:00:00.000000 ragdaemon-0.4.7/ragdaemon/daemon.py
--rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 ragdaemon-0.4.7/ragdaemon/errors.py
--rw-r--r--   0        0        0     6974 2020-02-02 00:00:00.000000 ragdaemon-0.4.7/ragdaemon/get_paths.py
--rw-r--r--   0        0        0     1984 2020-02-02 00:00:00.000000 ragdaemon-0.4.7/ragdaemon/graph.py
--rw-r--r--   0        0        0     2938 2020-02-02 00:00:00.000000 ragdaemon-0.4.7/ragdaemon/locate.py
--rw-r--r--   0        0        0     5493 2020-02-02 00:00:00.000000 ragdaemon-0.4.7/ragdaemon/utils.py
--rw-r--r--   0        0        0      776 2020-02-02 00:00:00.000000 ragdaemon-0.4.7/ragdaemon/annotators/__init__.py
--rw-r--r--   0        0        0      752 2020-02-02 00:00:00.000000 ragdaemon-0.4.7/ragdaemon/annotators/base_annotator.py
--rw-r--r--   0        0        0    10351 2020-02-02 00:00:00.000000 ragdaemon-0.4.7/ragdaemon/annotators/call_graph.py
--rw-r--r--   0        0        0     8471 2020-02-02 00:00:00.000000 ragdaemon-0.4.7/ragdaemon/annotators/chunker.py
--rw-r--r--   0        0        0     1505 2020-02-02 00:00:00.000000 ragdaemon-0.4.7/ragdaemon/annotators/chunker_line.py
--rw-r--r--   0        0        0     6675 2020-02-02 00:00:00.000000 ragdaemon-0.4.7/ragdaemon/annotators/chunker_llm.py
--rw-r--r--   0        0        0     6889 2020-02-02 00:00:00.000000 ragdaemon-0.4.7/ragdaemon/annotators/diff.py
--rw-r--r--   0        0        0     6243 2020-02-02 00:00:00.000000 ragdaemon-0.4.7/ragdaemon/annotators/hierarchy.py
--rw-r--r--   0        0        0     3806 2020-02-02 00:00:00.000000 ragdaemon-0.4.7/ragdaemon/annotators/layout_hierarchy.py
--rw-r--r--   0        0        0    11629 2020-02-02 00:00:00.000000 ragdaemon-0.4.7/ragdaemon/annotators/summarizer.py
--rw-r--r--   0        0        0     1452 2020-02-02 00:00:00.000000 ragdaemon-0.4.7/ragdaemon/database/__init__.py
--rw-r--r--   0        0        0     5233 2020-02-02 00:00:00.000000 ragdaemon-0.4.7/ragdaemon/database/chroma_database.py
--rw-r--r--   0        0        0     2208 2020-02-02 00:00:00.000000 ragdaemon-0.4.7/ragdaemon/database/database.py
--rw-r--r--   0        0        0     3193 2020-02-02 00:00:00.000000 ragdaemon-0.4.7/ragdaemon/database/lite_database.py
--rw-r--r--   0        0        0     2001 2020-02-02 00:00:00.000000 ragdaemon-0.4.7/ragdaemon/prompts/call_graph.toml
--rw-r--r--   0        0        0     2220 2020-02-02 00:00:00.000000 ragdaemon-0.4.7/ragdaemon/prompts/chunker_llm.toml
--rw-r--r--   0        0        0     1390 2020-02-02 00:00:00.000000 ragdaemon-0.4.7/ragdaemon/prompts/locate.toml
--rw-r--r--   0        0        0     1275 2020-02-02 00:00:00.000000 ragdaemon-0.4.7/ragdaemon/prompts/summarizer/base.txt
--rw-r--r--   0        0        0     1539 2020-02-02 00:00:00.000000 ragdaemon-0.4.7/ragdaemon/prompts/summarizer/chunk.txt
--rw-r--r--   0        0        0     1954 2020-02-02 00:00:00.000000 ragdaemon-0.4.7/ragdaemon/prompts/summarizer/directory.txt
--rw-r--r--   0        0        0     1664 2020-02-02 00:00:00.000000 ragdaemon-0.4.7/ragdaemon/prompts/summarizer/file.txt
--rw-r--r--   0        0        0     1429 2020-02-02 00:00:00.000000 ragdaemon-0.4.7/ragdaemon/prompts/summarizer/root.txt
--rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 ragdaemon-0.4.7/ragdaemon/prompts/summarizer/user.txt
--rw-r--r--   0        0        0    15406 2020-02-02 00:00:00.000000 ragdaemon-0.4.7/ragdaemon/static/favicon.ico
--rw-r--r--   0        0        0     1751 2020-02-02 00:00:00.000000 ragdaemon-0.4.7/ragdaemon/static/js/controlPanel.js
--rw-r--r--   0        0        0     3129 2020-02-02 00:00:00.000000 ragdaemon-0.4.7/ragdaemon/static/js/main.js
--rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 ragdaemon-0.4.7/ragdaemon/static/js/three/camera.js
--rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 ragdaemon-0.4.7/ragdaemon/static/js/three/controls.js
--rw-r--r--   0        0        0     1098 2020-02-02 00:00:00.000000 ragdaemon-0.4.7/ragdaemon/static/js/three/edge.js
--rw-r--r--   0        0        0     4014 2020-02-02 00:00:00.000000 ragdaemon-0.4.7/ragdaemon/static/js/three/node.js
--rw-r--r--   0        0        0     1596 2020-02-02 00:00:00.000000 ragdaemon-0.4.7/ragdaemon/static/js/three/raycaster.js
--rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 ragdaemon-0.4.7/ragdaemon/static/js/three/renderer.js
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 ragdaemon-0.4.7/ragdaemon/static/js/three/scene.js
--rw-r--r--   0        0        0     2713 2020-02-02 00:00:00.000000 ragdaemon-0.4.7/ragdaemon/templates/index.html
--rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 ragdaemon-0.4.7/ragdaemon/templates/search_results.html
--rw-r--r--   0        0        0     1984 2020-02-02 00:00:00.000000 ragdaemon-0.4.7/tests/conftest.py
--rw-r--r--   0        0        0     4433 2020-02-02 00:00:00.000000 ragdaemon-0.4.7/tests/test_comments.py
--rw-r--r--   0        0        0     3173 2020-02-02 00:00:00.000000 ragdaemon-0.4.7/tests/test_context.py
--rw-r--r--   0        0        0     1170 2020-02-02 00:00:00.000000 ragdaemon-0.4.7/tests/test_daemon.py
--rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 ragdaemon-0.4.7/tests/test_database.py
--rw-r--r--   0        0        0     1862 2020-02-02 00:00:00.000000 ragdaemon-0.4.7/tests/test_get_paths.py
--rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 ragdaemon-0.4.7/tests/test_sample.py
--rw-r--r--   0        0        0     2090 2020-02-02 00:00:00.000000 ragdaemon-0.4.7/tests/annotators/test_chunker.py
--rw-r--r--   0        0        0     2193 2020-02-02 00:00:00.000000 ragdaemon-0.4.7/tests/annotators/test_chunker_llm.py
--rw-r--r--   0        0        0     3995 2020-02-02 00:00:00.000000 ragdaemon-0.4.7/tests/annotators/test_diff.py
--rw-r--r--   0        0        0     2333 2020-02-02 00:00:00.000000 ragdaemon-0.4.7/tests/annotators/test_hierarchy.py
--rw-r--r--   0        0        0     1816 2020-02-02 00:00:00.000000 ragdaemon-0.4.7/tests/annotators/test_layout_hierarchy.py
--rw-r--r--   0        0        0     5785 2020-02-02 00:00:00.000000 ragdaemon-0.4.7/tests/annotators/test_summarizer.py
--rw-r--r--   0        0        0     9048 2020-02-02 00:00:00.000000 ragdaemon-0.4.7/tests/data/chunker_graph.json
--rw-r--r--   0        0        0     1616 2020-02-02 00:00:00.000000 ragdaemon-0.4.7/tests/data/context_message.txt
--rw-r--r--   0        0        0    11144 2020-02-02 00:00:00.000000 ragdaemon-0.4.7/tests/data/diff_graph.json
--rw-r--r--   0        0        0     1291 2020-02-02 00:00:00.000000 ragdaemon-0.4.7/tests/data/hard_to_chunk.txt
--rw-r--r--   0        0        0     2854 2020-02-02 00:00:00.000000 ragdaemon-0.4.7/tests/data/hierarchy_graph.json
--rw-r--r--   0        0        0     4002 2020-02-02 00:00:00.000000 ragdaemon-0.4.7/tests/data/layout_hierarchy_graph.json
--rw-r--r--   0        0        0    14226 2020-02-02 00:00:00.000000 ragdaemon-0.4.7/tests/data/summarizer_graph.json
--rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 ragdaemon-0.4.7/tests/sample/README.md
--rw-r--r--   0        0        0      494 2020-02-02 00:00:00.000000 ragdaemon-0.4.7/tests/sample/main.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ragdaemon-0.4.7/tests/sample/src/__init__.py
--rw-r--r--   0        0        0      528 2020-02-02 00:00:00.000000 ragdaemon-0.4.7/tests/sample/src/interface.py
--rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 ragdaemon-0.4.7/tests/sample/src/operations.py
--rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 ragdaemon-0.4.7/.gitignore
--rw-r--r--   0        0        0    11340 2020-02-02 00:00:00.000000 ragdaemon-0.4.7/LICENSE
--rw-r--r--   0        0        0     2264 2020-02-02 00:00:00.000000 ragdaemon-0.4.7/README.md
--rw-r--r--   0        0        0      899 2020-02-02 00:00:00.000000 ragdaemon-0.4.7/pyproject.toml
--rw-r--r--   0        0        0     3131 2020-02-02 00:00:00.000000 ragdaemon-0.4.7/PKG-INFO
+-rw-r--r--   0        0        0  1670456 2020-02-02 00:00:00.000000 ragdaemon-0.5.0/scratch.ipynb
+-rw-r--r--   0        0        0    10345 2020-02-02 00:00:00.000000 ragdaemon-0.5.0/tutorial.ipynb
+-rw-r--r--   0        0        0      653 2020-02-02 00:00:00.000000 ragdaemon-0.5.0/.github/workflows/run-tests.yml
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 ragdaemon-0.5.0/ragdaemon/__init__.py
+-rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 ragdaemon-0.5.0/ragdaemon/__main__.py
+-rw-r--r--   0        0        0     3742 2020-02-02 00:00:00.000000 ragdaemon-0.5.0/ragdaemon/app.py
+-rw-r--r--   0        0        0    10876 2020-02-02 00:00:00.000000 ragdaemon-0.5.0/ragdaemon/context.py
+-rw-r--r--   0        0        0     7730 2020-02-02 00:00:00.000000 ragdaemon-0.5.0/ragdaemon/daemon.py
+-rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 ragdaemon-0.5.0/ragdaemon/errors.py
+-rw-r--r--   0        0        0     6974 2020-02-02 00:00:00.000000 ragdaemon-0.5.0/ragdaemon/get_paths.py
+-rw-r--r--   0        0        0     1984 2020-02-02 00:00:00.000000 ragdaemon-0.5.0/ragdaemon/graph.py
+-rw-r--r--   0        0        0     2938 2020-02-02 00:00:00.000000 ragdaemon-0.5.0/ragdaemon/locate.py
+-rw-r--r--   0        0        0     5505 2020-02-02 00:00:00.000000 ragdaemon-0.5.0/ragdaemon/utils.py
+-rw-r--r--   0        0        0      776 2020-02-02 00:00:00.000000 ragdaemon-0.5.0/ragdaemon/annotators/__init__.py
+-rw-r--r--   0        0        0      752 2020-02-02 00:00:00.000000 ragdaemon-0.5.0/ragdaemon/annotators/base_annotator.py
+-rw-r--r--   0        0        0    10582 2020-02-02 00:00:00.000000 ragdaemon-0.5.0/ragdaemon/annotators/call_graph.py
+-rw-r--r--   0        0        0     8517 2020-02-02 00:00:00.000000 ragdaemon-0.5.0/ragdaemon/annotators/chunker.py
+-rw-r--r--   0        0        0     1505 2020-02-02 00:00:00.000000 ragdaemon-0.5.0/ragdaemon/annotators/chunker_line.py
+-rw-r--r--   0        0        0     6739 2020-02-02 00:00:00.000000 ragdaemon-0.5.0/ragdaemon/annotators/chunker_llm.py
+-rw-r--r--   0        0        0     6282 2020-02-02 00:00:00.000000 ragdaemon-0.5.0/ragdaemon/annotators/diff.py
+-rw-r--r--   0        0        0     4849 2020-02-02 00:00:00.000000 ragdaemon-0.5.0/ragdaemon/annotators/hierarchy.py
+-rw-r--r--   0        0        0     3806 2020-02-02 00:00:00.000000 ragdaemon-0.5.0/ragdaemon/annotators/layout_hierarchy.py
+-rw-r--r--   0        0        0    11934 2020-02-02 00:00:00.000000 ragdaemon-0.5.0/ragdaemon/annotators/summarizer.py
+-rw-r--r--   0        0        0     1462 2020-02-02 00:00:00.000000 ragdaemon-0.5.0/ragdaemon/database/__init__.py
+-rw-r--r--   0        0        0     5819 2020-02-02 00:00:00.000000 ragdaemon-0.5.0/ragdaemon/database/chroma_database.py
+-rw-r--r--   0        0        0     2418 2020-02-02 00:00:00.000000 ragdaemon-0.5.0/ragdaemon/database/database.py
+-rw-r--r--   0        0        0     3097 2020-02-02 00:00:00.000000 ragdaemon-0.5.0/ragdaemon/database/lite_database.py
+-rw-r--r--   0        0        0     2001 2020-02-02 00:00:00.000000 ragdaemon-0.5.0/ragdaemon/prompts/call_graph.toml
+-rw-r--r--   0        0        0     2220 2020-02-02 00:00:00.000000 ragdaemon-0.5.0/ragdaemon/prompts/chunker_llm.toml
+-rw-r--r--   0        0        0     1390 2020-02-02 00:00:00.000000 ragdaemon-0.5.0/ragdaemon/prompts/locate.toml
+-rw-r--r--   0        0        0     1275 2020-02-02 00:00:00.000000 ragdaemon-0.5.0/ragdaemon/prompts/summarizer/base.txt
+-rw-r--r--   0        0        0     1539 2020-02-02 00:00:00.000000 ragdaemon-0.5.0/ragdaemon/prompts/summarizer/chunk.txt
+-rw-r--r--   0        0        0     1954 2020-02-02 00:00:00.000000 ragdaemon-0.5.0/ragdaemon/prompts/summarizer/directory.txt
+-rw-r--r--   0        0        0     1664 2020-02-02 00:00:00.000000 ragdaemon-0.5.0/ragdaemon/prompts/summarizer/file.txt
+-rw-r--r--   0        0        0     1429 2020-02-02 00:00:00.000000 ragdaemon-0.5.0/ragdaemon/prompts/summarizer/root.txt
+-rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 ragdaemon-0.5.0/ragdaemon/prompts/summarizer/user.txt
+-rw-r--r--   0        0        0    15406 2020-02-02 00:00:00.000000 ragdaemon-0.5.0/ragdaemon/static/favicon.ico
+-rw-r--r--   0        0        0     1751 2020-02-02 00:00:00.000000 ragdaemon-0.5.0/ragdaemon/static/js/controlPanel.js
+-rw-r--r--   0        0        0     3129 2020-02-02 00:00:00.000000 ragdaemon-0.5.0/ragdaemon/static/js/main.js
+-rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 ragdaemon-0.5.0/ragdaemon/static/js/three/camera.js
+-rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 ragdaemon-0.5.0/ragdaemon/static/js/three/controls.js
+-rw-r--r--   0        0        0     1098 2020-02-02 00:00:00.000000 ragdaemon-0.5.0/ragdaemon/static/js/three/edge.js
+-rw-r--r--   0        0        0     4014 2020-02-02 00:00:00.000000 ragdaemon-0.5.0/ragdaemon/static/js/three/node.js
+-rw-r--r--   0        0        0     1596 2020-02-02 00:00:00.000000 ragdaemon-0.5.0/ragdaemon/static/js/three/raycaster.js
+-rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 ragdaemon-0.5.0/ragdaemon/static/js/three/renderer.js
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 ragdaemon-0.5.0/ragdaemon/static/js/three/scene.js
+-rw-r--r--   0        0        0     2713 2020-02-02 00:00:00.000000 ragdaemon-0.5.0/ragdaemon/templates/index.html
+-rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 ragdaemon-0.5.0/ragdaemon/templates/search_results.html
+-rw-r--r--   0        0        0     1984 2020-02-02 00:00:00.000000 ragdaemon-0.5.0/tests/conftest.py
+-rw-r--r--   0        0        0     4422 2020-02-02 00:00:00.000000 ragdaemon-0.5.0/tests/test_comments.py
+-rw-r--r--   0        0        0     3146 2020-02-02 00:00:00.000000 ragdaemon-0.5.0/tests/test_context.py
+-rw-r--r--   0        0        0     1170 2020-02-02 00:00:00.000000 ragdaemon-0.5.0/tests/test_daemon.py
+-rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 ragdaemon-0.5.0/tests/test_database.py
+-rw-r--r--   0        0        0     1862 2020-02-02 00:00:00.000000 ragdaemon-0.5.0/tests/test_get_paths.py
+-rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 ragdaemon-0.5.0/tests/test_sample.py
+-rw-r--r--   0        0        0     2090 2020-02-02 00:00:00.000000 ragdaemon-0.5.0/tests/annotators/test_chunker.py
+-rw-r--r--   0        0        0     2193 2020-02-02 00:00:00.000000 ragdaemon-0.5.0/tests/annotators/test_chunker_llm.py
+-rw-r--r--   0        0        0     3984 2020-02-02 00:00:00.000000 ragdaemon-0.5.0/tests/annotators/test_diff.py
+-rw-r--r--   0        0        0     1492 2020-02-02 00:00:00.000000 ragdaemon-0.5.0/tests/annotators/test_hierarchy.py
+-rw-r--r--   0        0        0     1816 2020-02-02 00:00:00.000000 ragdaemon-0.5.0/tests/annotators/test_layout_hierarchy.py
+-rw-r--r--   0        0        0     5731 2020-02-02 00:00:00.000000 ragdaemon-0.5.0/tests/annotators/test_summarizer.py
+-rw-r--r--   0        0        0     9048 2020-02-02 00:00:00.000000 ragdaemon-0.5.0/tests/data/chunker_graph.json
+-rw-r--r--   0        0        0     1616 2020-02-02 00:00:00.000000 ragdaemon-0.5.0/tests/data/context_message.txt
+-rw-r--r--   0        0        0    11144 2020-02-02 00:00:00.000000 ragdaemon-0.5.0/tests/data/diff_graph.json
+-rw-r--r--   0        0        0     1291 2020-02-02 00:00:00.000000 ragdaemon-0.5.0/tests/data/hard_to_chunk.txt
+-rw-r--r--   0        0        0     2854 2020-02-02 00:00:00.000000 ragdaemon-0.5.0/tests/data/hierarchy_graph.json
+-rw-r--r--   0        0        0     4002 2020-02-02 00:00:00.000000 ragdaemon-0.5.0/tests/data/layout_hierarchy_graph.json
+-rw-r--r--   0        0        0    18009 2020-02-02 00:00:00.000000 ragdaemon-0.5.0/tests/data/summarizer_graph.json
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 ragdaemon-0.5.0/tests/sample/README.md
+-rw-r--r--   0        0        0      494 2020-02-02 00:00:00.000000 ragdaemon-0.5.0/tests/sample/main.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ragdaemon-0.5.0/tests/sample/src/__init__.py
+-rw-r--r--   0        0        0      528 2020-02-02 00:00:00.000000 ragdaemon-0.5.0/tests/sample/src/interface.py
+-rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 ragdaemon-0.5.0/tests/sample/src/operations.py
+-rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 ragdaemon-0.5.0/.gitignore
+-rw-r--r--   0        0        0    11340 2020-02-02 00:00:00.000000 ragdaemon-0.5.0/LICENSE
+-rw-r--r--   0        0        0     2264 2020-02-02 00:00:00.000000 ragdaemon-0.5.0/README.md
+-rw-r--r--   0        0        0      899 2020-02-02 00:00:00.000000 ragdaemon-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0     3131 2020-02-02 00:00:00.000000 ragdaemon-0.5.0/PKG-INFO
```

### Comparing `ragdaemon-0.4.7/tutorial.ipynb` & `ragdaemon-0.5.0/tutorial.ipynb`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.4.7/.github/workflows/run-tests.yml` & `ragdaemon-0.5.0/.github/workflows/run-tests.yml`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.4.7/ragdaemon/app.py` & `ragdaemon-0.5.0/ragdaemon/app.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.4.7/ragdaemon/context.py` & `ragdaemon-0.5.0/ragdaemon/context.py`

 * *Files 5% similar despite different names*

```diff
@@ -33,24 +33,23 @@
 def render_comments(comments: list[Comment]) -> str:
     return "\n".join(comment.render() for comment in comments)
 
 
 class ContextBuilder:
     """Renders items from a graph into an llm-readable string."""
 
-    def __init__(self, graph: KnowledgeGraph, db: Database, verbose: bool = False):
+    def __init__(self, graph: KnowledgeGraph, verbose: bool = False):
         self.graph = graph
-        self.db = db
         self.verbose = verbose
         self.context = dict[
             str, dict[str, Any]
         ]()  # {path: {lines, tags, document, diff}}
 
     def copy(self):
-        duplicate = ContextBuilder(self.graph, self.db, self.verbose)
+        duplicate = ContextBuilder(self.graph, self.verbose)
         duplicate.context = deepcopy(self.context)
         return duplicate
 
     def __add__(self, other: ContextBuilder) -> ContextBuilder:
         duplicate = self.copy()
         for path_str, data in other.context.items():
             if path_str not in duplicate.context:
@@ -65,28 +64,25 @@
                     )
         return duplicate
 
     def _add_path(self, path_str: str):
         """Create a new record in the context for the given path."""
         document = None
         if path_str in self.graph:
-            checksum = self.graph.nodes[path_str]["checksum"]
-            document = self.db.get(checksum)["documents"][0]
+            document = self.graph.nodes[path_str]["document"]
             if document.endswith("[TRUNCATED]"):
                 document = None
         if document is None:  # Truncated or deleted
             try:
-                # Could be an ignored file, in which case load it into graph/db
                 # TODO: Add ignored files to the graph/database
                 cwd = Path(self.graph.graph["cwd"])
                 document = get_document(path_str, cwd, type="file")
             except FileNotFoundError:
                 # Or could be deleted but have a diff
                 document = f"{path_str}\n[DELETED]"
-            checksum = hash_str(document)
         message = {
             "lines": set(),
             "tags": set(),
             "document": document,
             "diffs": set(),
             "comments": dict[int, list[Comment]](),
         }
@@ -254,16 +250,15 @@
         output = ""
         diff_str, _, _ = parse_diff_id(next(iter(ids)))
         git_command = "--git diff"
         if diff_str != "DEFAULT":
             git_command += f" {diff_str}"
         output += f"{git_command}\n"
         for id in sorted(ids):
-            checksum = self.graph.nodes[id]["checksum"]
-            document = self.db.get(checksum)["documents"][0]
+            document = self.graph.nodes[id]["document"]
             # TODO: Add line numbers
             without_git_command = "\n".join(document.split("\n")[1:])
             output += without_git_command + "\n"
         return output
 
     def to_refs(self) -> list[str]:
         """Return a list of path:interval,interval for everything in current context."""
```

### Comparing `ragdaemon-0.4.7/ragdaemon/daemon.py` & `ragdaemon-0.5.0/ragdaemon/daemon.py`

 * *Files 5% similar despite different names*

```diff
@@ -140,28 +140,26 @@
         n: Optional[int] = None,
         node_types: Iterable[str] = ("file", "chunk", "diff"),
     ) -> list[dict[str, Any]]:
         """Return a sorted list of nodes that match the query."""
         return self.db.query_graph(query, self.graph, n=n, node_types=node_types)
 
     def get_document(self, filename: str) -> str:
-        checksum = self.graph.nodes[filename]["checksum"]
-        document = self.db.get(checksum)["documents"][0]
-        return document
+        return self.graph.nodes[filename]["document"]
 
     def get_context(
         self,
         query: str,
         context_builder: Optional[ContextBuilder] = None,
         max_tokens: int = 8000,
         auto_tokens: int = 0,
         model: Model | str = DEFAULT_COMPLETION_MODEL,
     ) -> ContextBuilder:
         if context_builder is None:
-            context = ContextBuilder(self.graph, self.db, self.verbose)
+            context = ContextBuilder(self.graph, self.verbose)
         else:
             # TODO: Compare graph hashes, reconcile changes
             context = context_builder
         include_context_message = context.render()
         include_tokens = self.spice_client.count_tokens(include_context_message, model)
         if not auto_tokens or include_tokens >= max_tokens:
             return context
```

### Comparing `ragdaemon-0.4.7/ragdaemon/get_paths.py` & `ragdaemon-0.5.0/ragdaemon/get_paths.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.4.7/ragdaemon/graph.py` & `ragdaemon-0.5.0/ragdaemon/graph.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.4.7/ragdaemon/locate.py` & `ragdaemon-0.5.0/ragdaemon/locate.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.4.7/ragdaemon/utils.py` & `ragdaemon-0.5.0/ragdaemon/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import hashlib
 import re
 import subprocess
 from base64 import b64encode
 from pathlib import Path
 
 from spice import Spice
-from spice.models import GPT_4_TURBO, Model, UnknownModel
+from spice.models import GPT_4o_2024_05_13, Model, UnknownModel
 from spice.spice import get_model_from_name
 
 from ragdaemon.errors import RagdaemonError
 from ragdaemon.get_paths import get_paths_for_directory
 
 mentat_dir_path = Path.home() / ".mentat"
 
@@ -37,15 +37,15 @@
     ".ts",
     ".jsx",
     ".tsx",
     ".scss",
 ]
 
 
-DEFAULT_COMPLETION_MODEL = GPT_4_TURBO
+DEFAULT_COMPLETION_MODEL = GPT_4o_2024_05_13
 
 
 def hash_str(string: str) -> str:
     """Return the MD5 hash of the input string."""
     return hashlib.md5(string.encode()).hexdigest()
```

### Comparing `ragdaemon-0.4.7/ragdaemon/annotators/__init__.py` & `ragdaemon-0.5.0/ragdaemon/annotators/__init__.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.4.7/ragdaemon/annotators/base_annotator.py` & `ragdaemon-0.5.0/ragdaemon/annotators/base_annotator.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.4.7/ragdaemon/annotators/call_graph.py` & `ragdaemon-0.5.0/ragdaemon/annotators/call_graph.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from typing import Any, Optional
 
 from tqdm.asyncio import tqdm
 from spice import SpiceMessages
 from spice.models import TextModel
 
 from ragdaemon.annotators.base_annotator import Annotator
-from ragdaemon.database import Database
+from ragdaemon.database import Database, remove_update_db_duplicates
 from ragdaemon.graph import KnowledgeGraph
 from ragdaemon.errors import RagdaemonError
 from ragdaemon.utils import (
     DEFAULT_CODE_EXTENSIONS,
     DEFAULT_COMPLETION_MODEL,
     parse_path_ref,
     semaphore,
@@ -151,21 +151,19 @@
         return calls
 
     async def get_file_call_data(
         self,
         node: str,
         data: dict,
         graph: KnowledgeGraph,
-        db: Database,
         retries: int = 1,
     ):
-        """Generate and save call data for a file node to graph and db"""
+        """Generate and save call data for a file node to graph"""
         calls = {}
-        record = db.get(data["checksum"])
-        document = record["documents"][0]
+        document = data["document"]
 
         # Insert line numbers
         lines = document.split("\n")
         file = lines[0]
         file_lines = lines[1:]
         if any(line for line in file_lines):
             file_lines = [f"{i+1}:{line}" for i, line in enumerate(file_lines)]
@@ -180,18 +178,14 @@
                         print(
                             f"Error generating call graph for {node}:\n{e}\n"
                             + f"{i-1} retries left."
                             if i > 1
                             else "Skipping."
                         )
 
-        # Save to db and graph
-        metadatas = record["metadatas"][0]
-        metadatas[self.call_field_id] = json.dumps(calls)
-        db.update(data["checksum"], metadatas=metadatas)
         data[self.call_field_id] = calls
 
     async def annotate(
         self, graph: KnowledgeGraph, db: Database, refresh: bool = False
     ) -> KnowledgeGraph:
         # Remove any existing call edges
         graph.remove_edges_from(
@@ -208,25 +202,35 @@
                 files_with_calls.append(node)
             else:
                 extension = Path(data["ref"]).suffix
                 if extension in self.call_extensions:
                     files_with_calls.append((node, data))
         # Generate/add call data for nodes that don't have it
         tasks = []
+        files_just_updated = set()
         for node, data in files_with_calls:
             if refresh or data.get(self.call_field_id, None) is None:
                 checksum = data.get("checksum")
                 if checksum is None:
                     raise RagdaemonError(f"Node {node} has no checksum.")
-                tasks.append(self.get_file_call_data(node, data, graph, db))
+                tasks.append(self.get_file_call_data(node, data, graph))
+                files_just_updated.add(node)
         if len(tasks) > 0:
             if self.verbose:
                 await tqdm.gather(*tasks, desc="Generating call graph")
             else:
                 await asyncio.gather(*tasks)
+            update_db = {"ids": [], "metadatas": []}
+            for node in files_just_updated:
+                data = graph.nodes[node]
+                update_db["ids"].append(data["checksum"])
+                metadatas = {self.call_field_id: json.dumps(data[self.call_field_id])}
+                update_db["metadatas"].append(metadatas)
+            update_db = remove_update_db_duplicates(**update_db)
+            db.update(**update_db)
 
         # Add call edges to graph. Each call should have only ONE source; if there are
         # chunks, the source is the matching chunk, otherwise it's the file.
         for file, data in files_with_calls:
             calls = data[self.call_field_id]
             if not isinstance(calls, dict):
                 calls = json.loads(calls)
@@ -240,16 +244,15 @@
                 raise RagdaemonError(f"File node {file} is missing chunks field.")
             if not isinstance(chunks, list):
                 chunks = json.loads(chunks)
             if len(chunks) == 0:
                 checksum = data.get("checksum")
                 if checksum is None:
                     raise RagdaemonError(f"File node {file} is missing checksum field.")
-                record = db.get(checksum)
-                document = record["documents"][0]
+                document = data["document"]
                 for i in range(1, len(document.split("\n")) + 1):
                     line_index[i] = file
             else:
                 for chunk in chunks:
                     _, lines = parse_path_ref(chunk["ref"])
                     if lines is None:
                         raise RagdaemonError(f"Chunk {chunk} is missing line numbers.")
```

### Comparing `ragdaemon-0.4.7/ragdaemon/annotators/chunker_line.py` & `ragdaemon-0.5.0/ragdaemon/annotators/chunker_line.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.4.7/ragdaemon/annotators/chunker_llm.py` & `ragdaemon-0.5.0/ragdaemon/annotators/chunker_llm.py`

 * *Files 5% similar despite different names*

```diff
@@ -33,18 +33,20 @@
 class ChunkerLLM(Chunker):
     name = "chunker_llm"
     chunk_field_id = "chunks_llm"
 
     def __init__(
         self,
         *args,
+        batch_size: int = 800,
         model: Optional[TextModel | str] = DEFAULT_COMPLETION_MODEL,
         **kwargs,
     ):
         super().__init__(*args, **kwargs)
+        self.batch_size = batch_size
         self.model = model
 
     async def get_llm_response(
         self,
         file: str,
         file_lines: list[str],
         last_chunk: Optional[dict[str, Any]] = None,
@@ -84,29 +86,29 @@
             if not any(chunk["id"] == last_chunk["id"] for chunk in chunks):
                 raise RagdaemonError(
                     f"Last chunk replacement ({last_chunk['id']}) not found in response."
                 )
         return chunks
 
     async def chunk_document(
-        self, document: str, batch_size: int = 1000, retries: int = 1
+        self, document: str, retries: int = 1
     ) -> list[dict[str, Any]]:
         """Parse file_lines into a list of {id, ref} chunks."""
         lines = document.split("\n")
         file = lines[0]
         file_lines = lines[1:]
         if not file_lines or not any(line for line in file_lines):
             return []
         file_lines = [f"{i+1}:{line}" for i, line in enumerate(file_lines)]
 
         # Get raw llm output: {id, start_line, end_line}
         chunks = list[dict[str, Any]]()
-        n_batches = (len(file_lines) + batch_size - 1) // batch_size
+        n_batches = (len(file_lines) + self.batch_size - 1) // self.batch_size
         for i in range(n_batches):
-            batch_lines = file_lines[i * batch_size : (i + 1) * batch_size]
+            batch_lines = file_lines[i * self.batch_size : (i + 1) * self.batch_size]
             last_chunk = chunks.pop() if chunks else None
             for j in range(retries + 1, 0, -1):
                 try:
                     _chunks = await self.get_llm_response(file, batch_lines, last_chunk)
                     chunks.extend(_chunks)
                     break
                 except RagdaemonError as e:
```

### Comparing `ragdaemon-0.4.7/ragdaemon/annotators/diff.py` & `ragdaemon-0.5.0/ragdaemon/annotators/diff.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import json
 import re
+from copy import deepcopy
 from pathlib import Path
 
 from ragdaemon.annotators.base_annotator import Annotator
 from ragdaemon.database import Database, remove_add_to_db_duplicates
 from ragdaemon.get_paths import get_git_root_for_path
 from ragdaemon.graph import KnowledgeGraph
 from ragdaemon.errors import RagdaemonError
@@ -90,90 +91,83 @@
 
         graph_nodes = {
             node
             for node, data in graph.nodes(data=True)
             if data and data.get("type") == "diff"
         }
         graph.remove_nodes_from(graph_nodes)
+
+        checksums = dict[str, str]()
         document = get_document(self.diff_args, cwd, type="diff")
         checksum = hash_str(document)
-        existing_records = db.get(checksum)
-        if refresh or len(existing_records["ids"]) == 0:
-            chunks = get_chunks_from_diff(id=self.id, diff=document)
-            data = {
-                "id": self.id,
-                "ref": self.diff_args,
-                "type": "diff",
-                "checksum": checksum,
-                "chunks": json.dumps(chunks),
-                "active": False,
-            }
-
-            # If the full diff is too long to embed, it is truncated. Anything
-            # removed will be captured in chunks.
-            document, truncate_ratio = truncate(document, db.embedding_model)
-            if truncate_ratio > 0 and self.verbose:
-                print(f"Truncated diff by {truncate_ratio:.2%}")
-            db.upsert(ids=checksum, documents=document, metadatas=data)
-        else:
-            data = existing_records["metadatas"][0]
-        data["chunks"] = json.loads(data["chunks"])
+        chunks = get_chunks_from_diff(id=self.id, diff=document)
+        data = {
+            "id": self.id,
+            "ref": self.diff_args,
+            "type": "diff",
+            "document": document,
+            "checksum": checksum,
+            "chunks": chunks,
+            "active": False,
+        }
         graph.add_node(self.id, **data)
+        checksums[self.id] = checksum
 
-        # Add chunks
-        add_to_db = {"ids": [], "documents": [], "metadatas": []}
-        edges_to_add = set()
-        for chunk_id, chunk_ref in data["chunks"].items():
+        for chunk_id, chunk_ref in chunks.items():
             document = get_document(chunk_ref, cwd, type="diff")
             chunk_checksum = hash_str(document)
-            existing_records = db.get(chunk_checksum)
-            if refresh or len(existing_records["ids"]) == 0:
-                data = {
-                    "id": chunk_id,
-                    "ref": chunk_ref,
-                    "type": "diff",
-                    "checksum": chunk_checksum,
-                    "active": False,
-                }
-                document, truncate_ratio = truncate(document, db.embedding_model)
-                if truncate_ratio > 0 and self.verbose:
-                    print(f"Truncated diff chunk {chunk_id} by {truncate_ratio:.2%}")
-                add_to_db["ids"].append(chunk_checksum)
-                add_to_db["documents"].append(document)
-                add_to_db["metadatas"].append(data)
-            else:
-                data = existing_records["metadatas"][0]
+            data = {
+                "id": chunk_id,
+                "ref": chunk_ref,
+                "type": "diff",
+                "document": document,
+                "checksum": chunk_checksum,
+                "active": False,
+            }
             graph.add_node(chunk_id, **data)
-            edges_to_add.add((self.id, chunk_id))
-            # Match file/chunk nodes in graph
-            path_ref = chunk_id.split(":", 1)[1]
-            file, lines = parse_path_ref(path_ref)
-            file_str = str(file)
-            if file_str not in graph:  # Removed files
+            graph.add_edge(self.id, chunk_id, type="diff")
+            checksums[chunk_id] = chunk_checksum
+
+            # Link it to all overlapping chunks (if file has chunks) or to the file
+            _, path, lines = parse_diff_id(chunk_id)
+            if not path:
+                continue
+            path_str = path.as_posix()
+            if path_str not in graph:  # Removed files
                 if self.verbose:
-                    print(f"File {file_str} not in graph")
+                    print(f"File {path_str} not in graph")
                 continue
-            edges_to_add.add((chunk_id, file_str))
-
-            def _link_to_successors(_node, visited=set()):
-                for successor in graph.successors(_node):
-                    if successor in visited:
-                        continue
-                    visited.add(successor)
-                    edge = (chunk_id, successor)
-                    _data = graph.nodes[successor]
-                    if _data.get("type") not in ["file", "chunk"]:
-                        continue
-                    _, _lines = parse_path_ref(_data["ref"])
-                    if lines and _lines and lines.intersection(_lines):
-                        edges_to_add.add(edge)
-                    _link_to_successors(successor, visited)
-
-            _link_to_successors(file_str)
-
-        for source, target in edges_to_add:
-            graph.add_edge(source, target, type="diff")
+            link_to = set()
+            for node, data in graph.nodes(data=True):
+                if not node.startswith(f"{path_str}:") or data.get("type") != "chunk":
+                    continue
+                _, _lines = parse_path_ref(data["ref"])
+                if lines and _lines and lines.intersection(_lines):
+                    link_to.add(node)
+            if len(link_to) == 0:
+                link_to.add(path_str)
+            for node in link_to:
+                graph.add_edge(node, chunk_id, type="link")
+
+        # Sync with remote DB
+        ids = list(set(checksums.values()))
+        response = db.get(ids=ids, include=[])
+        db_data = set(response["ids"])
+        add_to_db = {"ids": [], "documents": [], "metadatas": []}
+        for id, checksum in checksums.items():
+            if checksum in db_data:
+                continue
+            data = deepcopy(graph.nodes[id])
+            document = data.pop("document")
+            if "chunks" in data:
+                data["chunks"] = json.dumps(data["chunks"])
+            document, truncate_ratio = truncate(document, db.embedding_model)
+            if self.verbose and truncate_ratio > 0:
+                print(f"Truncated {id} by {truncate_ratio:.2%}")
+            add_to_db["ids"].append(checksum)
+            add_to_db["documents"].append(document)
+            add_to_db["metadatas"].append(data)
         if len(add_to_db["ids"]) > 0:
             add_to_db = remove_add_to_db_duplicates(**add_to_db)
-            db.upsert(**add_to_db)
+            db.add(**add_to_db)
 
         return graph
```

### Comparing `ragdaemon-0.4.7/ragdaemon/annotators/layout_hierarchy.py` & `ragdaemon-0.5.0/ragdaemon/annotators/layout_hierarchy.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.4.7/ragdaemon/annotators/summarizer.py` & `ragdaemon-0.5.0/ragdaemon/annotators/summarizer.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from spice import Spice, SpiceMessages
 from spice.models import TextModel
 from spice.spice import get_model_from_name
 from tqdm.asyncio import tqdm
 
 from ragdaemon.annotators.base_annotator import Annotator
 from ragdaemon.context import ContextBuilder
-from ragdaemon.database import Database
+from ragdaemon.database import Database, remove_update_db_duplicates
 from ragdaemon.graph import KnowledgeGraph
 from ragdaemon.errors import RagdaemonError
 from ragdaemon.utils import DEFAULT_COMPLETION_MODEL, hash_str, semaphore, truncate
 
 
 def count_leaf_nodes_any_depth(
     graph: KnowledgeGraph,
@@ -66,35 +66,34 @@
                 filetree.extend(build_filetree(graph, target, child, prefix + "  "))
     return filetree
 
 
 def get_document_and_context(
     node: str,
     graph: KnowledgeGraph,
-    db: Database,
     summary_field_id: str = "summary",
     model: Optional[TextModel] = None,
 ) -> tuple[str, str]:
     """Return the document and type-specific context for a node in the graph."""
     data = graph.nodes[node]
     if not data:
         raise RagdaemonError(f"Node {node} not found in graph")
     checksum = data.get("checksum")
     if not checksum:
         raise RagdaemonError(f"Node {node} has no checksum.")
 
     if data.get("type") == "directory":
         document = f"Directory: {node}"
     else:
-        cb = ContextBuilder(graph, db)
+        cb = ContextBuilder(graph)
         cb.add_id(node)
         document = cb.render()
 
     if data.get("type") == "chunk":
-        cb = ContextBuilder(graph, db)
+        cb = ContextBuilder(graph)
 
         # Parent chunks back to the file
         def get_hierarchical_parents(target: str, cb: ContextBuilder):
             """Recursviely select parent chunks linked by hierarchy edges."""
             for parent in graph.predecessors(target):
                 if graph.nodes[parent].get("type") != "chunk":
                     return
@@ -208,37 +207,35 @@
             if data.get("type") not in self.summarize_nodes:
                 continue
             if data.get(self.summary_field_id) is None:
                 return False
             document, context = get_document_and_context(
                 node,
                 graph,
-                db,
                 summary_field_id=self.summary_field_id,
                 model=self.model,
             )
             summary_checksum = hash_str(document + context)
             if summary_checksum != data.get(self.checksum_field_id):
                 return False
         return True
 
     async def generate_summary(
         self,
         node: str,
         graph: KnowledgeGraph,
-        db: Database,
         loading_bar: Optional[tqdm] = None,
         refresh: bool = False,
     ):
-        """Asynchronously generate summary and update graph and db"""
+        """Asynchronously generate summary and update graph"""
         if self.spice_client is None:
             raise RagdaemonError("Spice client not initialized")
 
         document, context = get_document_and_context(
-            node, graph, db, summary_field_id=self.summary_field_id, model=self.model
+            node, graph, summary_field_id=self.summary_field_id, model=self.model
         )
         summary_checksum = hash_str(document + context)
         data = graph.nodes[node]
         if (
             refresh
             or data.get(self.summary_field_id) is None
             or summary_checksum != data.get(self.checksum_field_id)
@@ -259,63 +256,68 @@
             async with semaphore:
                 response = await self.spice_client.get_response(
                     messages=messages,
                     model=self.model,
                 )
             summary = response.text
 
-            record = db.get(data["checksum"])
-            metadatas = record["metadatas"][0]
             if summary != "PASS":
-                metadatas[self.summary_field_id] = summary
                 data[self.summary_field_id] = summary
-            metadatas[self.checksum_field_id] = summary_checksum
             data[self.checksum_field_id] = summary_checksum
-            db.update(data["checksum"], metadatas=metadatas)
 
         if loading_bar is not None:
             loading_bar.update(1)
 
     async def dfs(
         self,
         node: str,
         graph: KnowledgeGraph,
-        db: Database,
         loading_bar: Optional[tqdm] = None,
         refresh: bool = False,
     ):
         """Depth-first search to generate summaries for all nodes"""
         children = [
             edge[1]
             for edge in graph.out_edges(node, data=True)
             if edge[-1].get("type") == "hierarchy"
             and graph.nodes[edge[1]].get("type") in self.summarize_nodes
         ]
         if children:
-            tasks = [
-                self.dfs(child, graph, db, loading_bar, refresh) for child in children
-            ]
+            tasks = [self.dfs(child, graph, loading_bar, refresh) for child in children]
             await asyncio.gather(*tasks)
-        await self.generate_summary(node, graph, db, loading_bar, refresh)
+        await self.generate_summary(node, graph, loading_bar, refresh)
 
     async def annotate(
         self, graph: KnowledgeGraph, db: Database, refresh: bool = False
     ) -> KnowledgeGraph:
         """Asynchronously generate or fetch summaries and add to graph/db"""
+        summaries = dict[str, str]()
+        for node, data in graph.nodes(data=True):
+            if data is not None and data.get("type") in self.summarize_nodes:
+                summaries[node] = data.get(self.checksum_field_id, "")
+
         if self.verbose:
-            n = len(
-                [
-                    node
-                    for node, data in graph.nodes(data=True)
-                    if data is not None and data.get("type") in self.summarize_nodes
-                ]
-            )
-            loading_bar = tqdm(total=n, desc="Summarizing code...")
+            loading_bar = tqdm(total=len(summaries), desc="Summarizing code...")
         else:
             loading_bar = None
 
-        await self.dfs("ROOT", graph, db, loading_bar, refresh)
+        await self.dfs("ROOT", graph, loading_bar, refresh)
+
+        update_db = {"ids": [], "metadatas": []}
+        for node, summary_checksum in summaries.items():
+            if graph.nodes[node].get(self.checksum_field_id) != summary_checksum:
+                data = graph.nodes[node]
+                update_db["ids"].append(data["checksum"])
+                update_db["metadatas"].append(
+                    {
+                        self.summary_field_id: data[self.summary_field_id],
+                        self.checksum_field_id: data[self.checksum_field_id],
+                    }
+                )
+        if len(update_db["ids"]) > 1:
+            update_db = remove_update_db_duplicates(**update_db)
+            db.update(**update_db)
 
         if loading_bar is not None:
             loading_bar.close()
 
         return graph
```

### Comparing `ragdaemon-0.4.7/ragdaemon/database/__init__.py` & `ragdaemon-0.5.0/ragdaemon/database/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,18 @@
 import os
 from pathlib import Path
 from typing import Optional
 
 from spice import Spice
-from spice.errors import SpiceError
 
-from ragdaemon.database.chroma_database import ChromaDB, remove_add_to_db_duplicates
+from ragdaemon.database.chroma_database import (
+    ChromaDB,
+    remove_add_to_db_duplicates,
+    remove_update_db_duplicates,
+)
 from ragdaemon.database.database import Database
 from ragdaemon.database.lite_database import LiteDB
 from ragdaemon.utils import mentat_dir_path
 
 DEFAULT_EMBEDDING_MODEL = "text-embedding-3-large"
```

### Comparing `ragdaemon-0.4.7/ragdaemon/database/chroma_database.py` & `ragdaemon-0.5.0/ragdaemon/database/chroma_database.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,20 +9,14 @@
 from ragdaemon import __version__
 from ragdaemon.database.database import Database
 from ragdaemon.errors import RagdaemonError
 from ragdaemon.utils import basic_auth
 
 MAX_INPUTS_PER_CALL = 2048
 
-if TYPE_CHECKING:
-    from chromadb.api.types import (
-        GetResult,
-        Metadata,
-    )
-
 
 def remove_add_to_db_duplicates(
     ids: list[str], documents: list[str], metadatas: list[dict]
 ) -> dict[str, Any]:
     seen = set()
     output = {"ids": [], "documents": [], "metadatas": []}
     for id, document, metadata in zip(ids, documents, metadatas):
@@ -30,14 +24,27 @@
             output["ids"].append(id)
             output["documents"].append(document)
             output["metadatas"].append(metadata)
             seen.add(id)
     return output
 
 
+def remove_update_db_duplicates(
+    ids: list[str], metadatas: list[dict]
+) -> dict[str, Any]:
+    seen = set()
+    output = {"ids": [], "metadatas": []}
+    for id, metadata in zip(ids, metadatas):
+        if id not in seen:
+            output["ids"].append(id)
+            output["metadatas"].append(metadata)
+            seen.add(id)
+    return output
+
+
 class ChromaDB(Database):
     def __init__(
         self,
         cwd: Path,
         db_path: Path,
         spice_client: Spice,
         embedding_model: str,
@@ -101,43 +108,48 @@
         name = f"ragdaemon-{minor_version}-{self.embedding_model}"
         self._collection = _client.get_or_create_collection(
             name=name,
             embedding_function=embedding_function,
         )
 
     def query(self, query: str, active_checksums: list[str]) -> list[dict]:
+        """
+        Since we add many different versions of each file to Chroma, we can't do a
+        straightforward query, because it'd return multiple version of the same file.
+
+        The best workaround I've found for this is using the 'active' flag in metadata.
+        The downside is that it requires 2 additional calls to the database each time:
+        one to set it, another to unset it. The extra time is negligible for local DBs
+        and hopefully not unreasonable for remote.
+
+        There's a third "extra" call to validate the active_checksums. If we don't do
+        this it will still function properly but it will print a lot of warnings.
+        """
+        valid_checksums = self._collection.get(ids=active_checksums, include=[])["ids"]
         # Flag active records
-        result: GetResult = self._collection.get(active_checksums)
-        metadatas: Optional[list[Metadata]] = result["metadatas"]
-        if not metadatas or len(metadatas) == 0:
-            return []
-        updates = {"ids": [], "metadatas": []}
-        for metadata in metadatas:
-            updates["ids"].append(metadata["checksum"])
-            updates["metadatas"].append({**metadata, "active": True})
+        updates = {
+            "ids": valid_checksums,
+            "metadatas": [{"active": True} for _ in valid_checksums],
+        }
         self._collection.update(**updates)
         # Query
         response = self._collection.query(
             query_texts=query,
             where={"active": True},
-            n_results=len(metadatas),
+            n_results=len(valid_checksums),
+            include=["distances"],
         )
         # Remove flags
-        updates["metadatas"] = [{**metadata, "active": False} for metadata in metadatas]
+        updates = {
+            "ids": valid_checksums,
+            "metadatas": [{"active": False} for _ in valid_checksums],
+        }
         self._collection.update(**updates)
-        # Parse results. Return results for the 'first query' only
-        if (
-            response is None
-            or response["metadatas"] is None
-            or response["documents"] is None
-            or response["distances"] is None
-        ):
+        if response is None or response["distances"] is None:
             return []
-        _metadatas = response["metadatas"][0]
-        _documents = response["documents"][0]
-        _distances = response["distances"][0]
+        # Parse results. Return results for the 'first query' only
         results = [
-            {**m, "document": do, "distance": di}
-            for m, do, di in zip(_metadatas, _documents, _distances)
+            {"checksum": id, "distance": distance}
+            for id, distance in zip(response["ids"][0], response["distances"][0])
         ]
         results = sorted(results, key=lambda x: x["distance"])
         return results
```

### Comparing `ragdaemon-0.4.7/ragdaemon/database/database.py` & `ragdaemon-0.5.0/ragdaemon/database/database.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from pathlib import Path
-from typing import Iterable, Optional
+from typing import Any, Iterable, Optional
 
 from ragdaemon.graph import KnowledgeGraph
 
 
 class Database:
     embedding_model: str | None = None
     _collection = None  # Collection | LiteDB
@@ -26,27 +26,32 @@
         node_types: Iterable[str] = ("file", "chunk", "diff"),
     ) -> list[dict]:
         """Return documents, metadatas and distances, sorted, for nodes in the graph.
 
         Chroma's default search covers all records, including inactive ones, so we
         manually flag the active records, query them, and then unflag them.
         """
-        active_checksums = list(
-            {
-                data["checksum"]
-                for _, data in graph.nodes(data=True)
-                if data and "checksum" in data and data["type"] in node_types
-            }
-        )
-        results = self.query(query, active_checksums)
+        checksum_index = {
+            data["checksum"]: node
+            for node, data in graph.nodes(data=True)
+            if data and "checksum" in data and data["type"] in node_types
+        }
+        response = self.query(query, list(checksum_index.keys()))
+
+        # Add (local) metadata to results
+        results = list[dict[str, Any]]()
+        for result in response:
+            node = checksum_index[result["checksum"]]
+            data = graph.nodes[node]
+            result = {**result, **data}
+            results.append(result)
 
         # Add exact-match multiplier
         for result in results:
             distance = result["distance"]
-            # Multiply by 2 if query is in the NAME
             type = result["type"]
             if type == "file":
                 name = Path(result["id"]).name
             elif type == "chunk":
                 name = result["id"].split(":")[1]
                 if "." in name:
                     name = name.split(".")[-1]
```

### Comparing `ragdaemon-0.4.7/ragdaemon/database/lite_database.py` & `ragdaemon-0.5.0/ragdaemon/database/lite_database.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,54 +1,52 @@
 from pathlib import Path
-from typing import Any
+from typing import Any, Optional
 
 from ragdaemon.database.database import Database
 
 
 class LiteDB(Database):
     def __init__(self, cwd: Path, db_path: Path):
         self.cwd = cwd
         self.db_path = db_path
         self._collection = LiteCollection()
 
     def query(self, query: str, active_checksums: list[str]) -> list[dict]:
         response = self._collection.query(query, active_checksums)
         results = [
-            {**data, "document": document, "distance": distance}
-            for data, document, distance in zip(
-                response["metadatas"][0],
-                response["documents"][0],
-                response["distances"][0],
-            )
+            {"checksum": id, "distance": distance}
+            for id, distance in zip(response["ids"][0], response["distances"][0])
         ]
         results = sorted(results, key=lambda x: x["distance"])
         return results
 
 
 class LiteCollection:
     """A fast alternative to ChromaDB for testing (and anything else).
 
     Matches the chroma Collection API except:
     - No embeddings
     - In-memory
-    - A basic hand-coded search algo
+    - Query returns all distances=1
     """
 
     def __init__(self):
         self.data = dict[str, dict[str, Any]]()  # {id: {metadatas, document}}
 
-    def get(self, ids: list[str] | str) -> dict:
+    def get(self, ids: list[str] | str, include: Optional[list[str]] = None) -> dict:
         if isinstance(ids, str):
             ids = [ids]
         output = {"ids": [], "metadatas": [], "documents": []}
         for id in ids:
             if id in self.data:
                 output["ids"].append(id)
                 output["metadatas"].append(self.data[id]["metadatas"])
                 output["documents"].append(self.data[id]["document"])
+        if include:
+            output = {k: v for k, v in output.items() if k in include or k == "ids"}
         return output
 
     def count(self) -> int:
         return len(self.data)
 
     def update(self, ids: list[str] | str, metadatas: list[dict] | dict):
         ids = [ids] if isinstance(ids, str) else ids
@@ -61,20 +59,18 @@
     def query(self, query: str, active_checksums: list[str]) -> dict[str, list[Any]]:
         # Select active/filtered records
         records = [
             {"id": k, **v} for k, v in self.data.items() if k in active_checksums
         ]
         return {
             "ids": [[r["id"] for r in records]],
-            "metadatas": [[r["metadatas"] for r in records]],
-            "documents": [[r["document"] for r in records]],
             "distances": [[1] * len(records)],
         }
 
-    def upsert(
+    def add(
         self,
         ids: list[str] | str,
         metadatas: list[dict] | dict,
         documents: list[str] | str,
     ) -> list[str]:
         ids = [ids] if isinstance(ids, str) else ids
         metadatas = [metadatas] if isinstance(metadatas, dict) else metadatas
```

### Comparing `ragdaemon-0.4.7/ragdaemon/prompts/call_graph.toml` & `ragdaemon-0.5.0/ragdaemon/prompts/call_graph.toml`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.4.7/ragdaemon/prompts/chunker_llm.toml` & `ragdaemon-0.5.0/ragdaemon/prompts/chunker_llm.toml`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.4.7/ragdaemon/prompts/locate.toml` & `ragdaemon-0.5.0/ragdaemon/prompts/locate.toml`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.4.7/ragdaemon/prompts/summarizer/base.txt` & `ragdaemon-0.5.0/ragdaemon/prompts/summarizer/base.txt`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.4.7/ragdaemon/prompts/summarizer/chunk.txt` & `ragdaemon-0.5.0/ragdaemon/prompts/summarizer/chunk.txt`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.4.7/ragdaemon/prompts/summarizer/directory.txt` & `ragdaemon-0.5.0/ragdaemon/prompts/summarizer/directory.txt`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.4.7/ragdaemon/prompts/summarizer/file.txt` & `ragdaemon-0.5.0/ragdaemon/prompts/summarizer/file.txt`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.4.7/ragdaemon/prompts/summarizer/root.txt` & `ragdaemon-0.5.0/ragdaemon/prompts/summarizer/root.txt`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.4.7/ragdaemon/static/favicon.ico` & `ragdaemon-0.5.0/ragdaemon/static/favicon.ico`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.4.7/ragdaemon/static/js/controlPanel.js` & `ragdaemon-0.5.0/ragdaemon/static/js/controlPanel.js`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.4.7/ragdaemon/static/js/main.js` & `ragdaemon-0.5.0/ragdaemon/static/js/main.js`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.4.7/ragdaemon/static/js/three/edge.js` & `ragdaemon-0.5.0/ragdaemon/static/js/three/edge.js`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.4.7/ragdaemon/static/js/three/node.js` & `ragdaemon-0.5.0/ragdaemon/static/js/three/node.js`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.4.7/ragdaemon/static/js/three/raycaster.js` & `ragdaemon-0.5.0/ragdaemon/static/js/three/raycaster.js`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.4.7/ragdaemon/templates/index.html` & `ragdaemon-0.5.0/ragdaemon/templates/index.html`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.4.7/tests/conftest.py` & `ragdaemon-0.5.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.4.7/tests/test_comments.py` & `ragdaemon-0.5.0/tests/test_comments.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 
 @pytest.mark.asyncio
 async def test_comment_render(git_history, mock_db):
     daemon = Daemon(cwd=git_history)
     await daemon.update(refresh=True)
 
-    context = ContextBuilder(daemon.graph, daemon.db)
+    context = ContextBuilder(daemon.graph)
     context.add_ref("src/operations.py")
     context.add_comment(
         "src/operations.py", {"comment": "What is this file for?"}, tags=["test-flag"]
     )
     context.add_comment(
         "src/operations.py",
         {"comment": {"author": "bot", "content": "test"}},
```

### Comparing `ragdaemon-0.4.7/tests/test_context.py` & `ragdaemon-0.5.0/tests/test_context.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,20 +4,20 @@
 
 from ragdaemon.context import ContextBuilder
 from ragdaemon.daemon import Daemon
 from ragdaemon.graph import KnowledgeGraph
 from ragdaemon.utils import get_document
 
 
-def test_daemon_render_context(cwd, mock_db):
+def test_daemon_render_context(cwd):
     path_str = Path("src/interface.py").as_posix()
     ref = path_str
 
     # Base Chunk
-    context = ContextBuilder(KnowledgeGraph(), mock_db)
+    context = ContextBuilder(KnowledgeGraph())
     context.context = {
         path_str: {
             "lines": set([1, 2, 3, 4, 15]),
             "tags": ["test-flag"],
             "document": get_document(ref, cwd),
             "diffs": set(),
             "comments": dict(),
@@ -95,15 +95,15 @@
 
 
 def test_to_refs(cwd, mock_db):
     path_str = Path("src/interface.py").as_posix()
     ref = path_str
 
     # Setup Context
-    context = ContextBuilder(KnowledgeGraph(), mock_db)
+    context = ContextBuilder(KnowledgeGraph())
     context.context = {
         path_str: {
             "lines": set([1, 2, 3, 4, 15]),
             "tags": ["test-flag"],
             "document": get_document(ref, cwd),
             "diffs": set(),
             "comments": dict(),
```

### Comparing `ragdaemon-0.4.7/tests/test_daemon.py` & `ragdaemon-0.5.0/tests/test_daemon.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.4.7/tests/test_get_paths.py` & `ragdaemon-0.5.0/tests/test_get_paths.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.4.7/tests/test_sample.py` & `ragdaemon-0.5.0/tests/test_sample.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.4.7/tests/annotators/test_chunker.py` & `ragdaemon-0.5.0/tests/annotators/test_chunker.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.4.7/tests/annotators/test_chunker_llm.py` & `ragdaemon-0.5.0/tests/annotators/test_chunker_llm.py`

 * *Files 0% similar despite different names*

```diff
@@ -33,23 +33,23 @@
 
 
 @pytest.mark.skip(reason="This test requires calling an API")
 @pytest.mark.asyncio
 async def test_chunker_llm_edge_cases(cwd, expected_chunks):
     # NOTE: TO RUN THIS YOU HAVE TO COMMENT_OUT tests/conftest.py/mock_openai_api_key
     daemon = Daemon(cwd, annotators={"hierarchy": {}})
-    chunker = ChunkerLLM(spice_client=daemon.spice_client)
+    chunker = ChunkerLLM(spice_client=daemon.spice_client, batch_size=10)
 
     # One example with all the edge cases (when batch_size = 10 lines):
     # - First batch ends mid-class, so second batch needs 'call path'
     # - Second batch ends mid-function, third batch needs to pickup where it left off
     # - Third batch is all inside one function, so needs to pass call forward.
     text = Path("tests/data/hard_to_chunk.txt").read_text()
     document = f"src/calculator.py\n{text}"
-    actual_chunks = await chunker.chunk_document(document, batch_size=10)
+    actual_chunks = await chunker.chunk_document(document)
 
     print(actual_chunks)
 
     assert len(actual_chunks) == len(expected_chunks)
     actual_chunks = sorted(actual_chunks, key=lambda x: x["ref"])
     expected_chunks = sorted(expected_chunks, key=lambda x: x["ref"])
     for actual, expected in zip(actual_chunks, expected_chunks):
```

### Comparing `ragdaemon-0.4.7/tests/annotators/test_diff.py` & `ragdaemon-0.5.0/tests/annotators/test_diff.py`

 * *Files 1% similar despite different names*

```diff
@@ -55,15 +55,15 @@
 
 @pytest.mark.asyncio
 async def test_diff_render(git_history, mock_db):
     daemon = Daemon(cwd=git_history)
     await daemon.update(refresh=True)
 
     # Only diffs
-    context = ContextBuilder(daemon.graph, daemon.db)
+    context = ContextBuilder(daemon.graph)
     context.add_diff("DEFAULT:main.py")
     context.add_diff("DEFAULT:src/operations.py:1-5")
     context.add_diff("DEFAULT:src/operations.py:8-10")
     actual = context.render(use_tags=True)
     assert (
         actual
         == """\
```

### Comparing `ragdaemon-0.4.7/tests/annotators/test_hierarchy.py` & `ragdaemon-0.5.0/tests/annotators/test_hierarchy.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,37 +1,17 @@
 import json
 from pathlib import Path
 
 from networkx.readwrite import json_graph
 import pytest
 
-from ragdaemon.annotators.hierarchy import Hierarchy, get_active_checksums
+from ragdaemon.annotators.hierarchy import Hierarchy
 from ragdaemon.graph import KnowledgeGraph
 
 
-def test_get_active_checksums(cwd, mock_db):
-    checksums = get_active_checksums(cwd, mock_db)
-    assert isinstance(checksums, dict), "Checksums is not a dict"
-    assert all(isinstance(k, Path) for k in checksums), "Keys are not all Paths"
-    assert all(
-        isinstance(v, str) for v in checksums.values()
-    ), "Values are not all strings"
-
-    hierarchy_graph = KnowledgeGraph.load("tests/data/hierarchy_graph.json")
-    expected = {
-        (node, data["checksum"])
-        for node, data in hierarchy_graph.nodes(data=True)
-        if data and "checksum" in data
-    }
-    # Replace checksums "." with "ROOT"
-    checksums[Path("ROOT")] = checksums.pop(Path("."))
-    actual = {(path.as_posix(), checksum) for path, checksum in checksums.items()}
-    assert actual == expected, "Checksums are not equal"
-
-
 def test_hierarchy_is_complete(cwd, mock_db):
     empty_graph = KnowledgeGraph()
     empty_graph.graph["cwd"] = cwd.as_posix()
     hierarchy = Hierarchy()
 
     assert not hierarchy.is_complete(
         empty_graph, mock_db
```

### Comparing `ragdaemon-0.4.7/tests/annotators/test_layout_hierarchy.py` & `ragdaemon-0.5.0/tests/annotators/test_layout_hierarchy.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.4.7/tests/annotators/test_summarizer.py` & `ragdaemon-0.5.0/tests/annotators/test_summarizer.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,12 @@
+import json
 from pathlib import Path
 
 import pytest
+from networkx.readwrite import json_graph
 
 from ragdaemon.annotators.summarizer import (
     build_filetree,
     get_document_and_context,
 )
 from ragdaemon.daemon import Daemon
 from ragdaemon.database import LiteDB
@@ -42,22 +44,21 @@
         "  src/operations.py",
     ]
 
 
 @pytest.mark.asyncio
 async def test_get_document_and_context(cwd):
     graph = KnowledgeGraph.load("tests/data/summarizer_graph.json")  # Chunk data
-    db = LiteDB(cwd=cwd, db_path=Path("."))
     for _, data in graph.nodes(data=True):
         document = get_document(data["ref"], cwd=cwd, type=data["type"])
-        db._collection.upsert(ids=data["checksum"], documents=document, metadatas=data)
+        data["document"] = document
 
     # A chunk
     document, context = get_document_and_context(
-        "src/interface.py:parse_arguments", graph, db
+        "src/interface.py:parse_arguments", graph
     )
     assert (
         document
         == """\
 src/interface.py
 ...
 5:def parse_arguments():
@@ -103,15 +104,15 @@
 18:
 19:    render_response(result)
 ...
 """
     )
 
     # A file
-    document, context = get_document_and_context("src/interface.py", graph, db)
+    document, context = get_document_and_context("src/interface.py", graph)
     assert document.startswith("src/interface.py\n")
     assert (
         context
         == """\
 <file_tree>
 .gitignore - Manage exclusions for version control by specifying files and directories that Git should ignore, while ensuring the .gitignore file itself remains tracked.
 README.md - Describe the application's experimental purpose in testing the limits of the treesitter parser.
@@ -127,15 +128,15 @@
 src/interface.py:render_response Display the result of a mathematical operation to standard output.
 src/interface.py:parse_arguments Parse command-line arguments into three components: an integer, a symbol representing a mathematical operation, and a second integer.
 </chunk_summaries>
 """
     )
 
     # A directory
-    document, context = get_document_and_context("src", graph, db)
+    document, context = get_document_and_context("src", graph)
     assert document == "Directory: src"
     assert (
         context
         == """\
 <file_tree>
 .gitignore - Manage exclusions for version control by specifying files and directories that Git should ignore, while ensuring the .gitignore file itself remains tracked.
 README.md - Describe the application's experimental purpose in testing the limits of the treesitter parser.
```

### Comparing `ragdaemon-0.4.7/tests/data/chunker_graph.json` & `ragdaemon-0.5.0/tests/data/chunker_graph.json`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.4.7/tests/data/context_message.txt` & `ragdaemon-0.5.0/tests/data/context_message.txt`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.4.7/tests/data/diff_graph.json` & `ragdaemon-0.5.0/tests/data/diff_graph.json`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.4.7/tests/data/hard_to_chunk.txt` & `ragdaemon-0.5.0/tests/data/hard_to_chunk.txt`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.4.7/tests/data/hierarchy_graph.json` & `ragdaemon-0.5.0/tests/data/hierarchy_graph.json`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.4.7/tests/data/layout_hierarchy_graph.json` & `ragdaemon-0.5.0/tests/data/layout_hierarchy_graph.json`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.4.7/tests/sample/src/interface.py` & `ragdaemon-0.5.0/tests/sample/src/interface.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.4.7/LICENSE` & `ragdaemon-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.4.7/README.md` & `ragdaemon-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.4.7/pyproject.toml` & `ragdaemon-0.5.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "hatchling.build"
 
 [tool.hatch.build.targets.wheel]
 packages=["ragdaemon"]
 
 [project]
 name = "ragdaemon"
-version = "0.4.7"
+version = "0.5.0"
 description = "Generate and render a call graph for a Python project."
 readme = "README.md"
 dependencies = [
     "chromadb==0.4.24",
     "dict2xml==1.7.5",
     "fastapi==0.109.2",
     "Jinja2==3.1.3",
```

### Comparing `ragdaemon-0.4.7/PKG-INFO` & `ragdaemon-0.5.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: ragdaemon
-Version: 0.4.7
+Version: 0.5.0
 Summary: Generate and render a call graph for a Python project.
 Project-URL: Homepage, https://github.com/AbanteAI/ragdaemon
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
```

