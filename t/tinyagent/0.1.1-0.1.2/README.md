# Comparing `tmp/tinyagent-0.1.1.tar.gz` & `tmp/tinyagent-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tinyagent-0.1.1.tar", last modified: Sat May 18 16:24:26 2024, max compression
+gzip compressed data, was "tinyagent-0.1.2.tar", last modified: Sat May 18 16:44:58 2024, max compression
```

## Comparing `tinyagent-0.1.1.tar` & `tinyagent-0.1.2.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 lan        (501) wheel        (0)        0 2024-05-18 16:24:26.765694 tinyagent-0.1.1/
--rw-r--r--   0 lan        (501) wheel        (0)      789 2024-05-18 15:22:41.000000 tinyagent-0.1.1/.gitignore
--rw-r--r--   0 lan        (501) wheel        (0)     1069 2024-05-18 16:24:07.000000 tinyagent-0.1.1/LICENSE
--rw-r--r--   0 lan        (501) wheel        (0)      462 2024-05-18 16:24:26.765558 tinyagent-0.1.1/PKG-INFO
--rw-r--r--   0 lan        (501) wheel        (0)       83 2024-05-18 15:22:41.000000 tinyagent-0.1.1/README.md
--rw-r--r--   0 lan        (501) wheel        (0)    32102 2024-05-18 15:22:41.000000 tinyagent-0.1.1/poetry.lock
--rw-r--r--   0 lan        (501) wheel        (0)      303 2024-05-18 16:24:07.000000 tinyagent-0.1.1/pyproject.toml
--rw-r--r--   0 lan        (501) wheel        (0)       38 2024-05-18 16:24:26.765727 tinyagent-0.1.1/setup.cfg
--rw-r--r--   0 lan        (501) wheel        (0)      589 2024-05-18 16:24:07.000000 tinyagent-0.1.1/setup.py
-drwxr-xr-x   0 lan        (501) wheel        (0)        0 2024-05-18 16:24:26.762265 tinyagent-0.1.1/tests/
-drwxr-xr-x   0 lan        (501) wheel        (0)        0 2024-05-18 16:24:26.762404 tinyagent-0.1.1/tests/resources/
--rw-r--r--   0 lan        (501) wheel        (0)      785 2024-05-18 15:22:41.000000 tinyagent-0.1.1/tests/resources/test.jpg
--rw-r--r--   0 lan        (501) wheel        (0)     1987 2024-05-18 15:22:41.000000 tinyagent-0.1.1/tests/test_claude.py
--rw-r--r--   0 lan        (501) wheel        (0)     1991 2024-05-18 15:22:41.000000 tinyagent-0.1.1/tests/test_gpt.py
--rw-r--r--   0 lan        (501) wheel        (0)     1018 2024-05-18 15:22:41.000000 tinyagent-0.1.1/tests/test_tool.py
-drwxr-xr-x   0 lan        (501) wheel        (0)        0 2024-05-18 16:24:26.762528 tinyagent-0.1.1/tinyagent/
--rw-r--r--   0 lan        (501) wheel        (0)      562 2024-05-18 16:24:07.000000 tinyagent-0.1.1/tinyagent/__init__.py
-drwxr-xr-x   0 lan        (501) wheel        (0)        0 2024-05-18 16:24:26.763881 tinyagent-0.1.1/tinyagent/agent/
--rw-r--r--   0 lan        (501) wheel        (0)      385 2024-05-18 15:22:41.000000 tinyagent-0.1.1/tinyagent/agent/__init__.py
--rw-r--r--   0 lan        (501) wheel        (0)     4114 2024-05-18 15:22:41.000000 tinyagent-0.1.1/tinyagent/agent/base.py
-drwxr-xr-x   0 lan        (501) wheel        (0)        0 2024-05-18 16:24:26.764229 tinyagent-0.1.1/tinyagent/agent/claude/
--rw-r--r--   0 lan        (501) wheel        (0)        0 2024-05-18 16:24:07.000000 tinyagent-0.1.1/tinyagent/agent/claude/__init__..py
--rw-r--r--   0 lan        (501) wheel        (0)     9002 2024-05-18 15:22:41.000000 tinyagent-0.1.1/tinyagent/agent/claude/agent.py
--rw-r--r--   0 lan        (501) wheel        (0)     2333 2024-05-18 15:22:41.000000 tinyagent-0.1.1/tinyagent/agent/claude/client.py
-drwxr-xr-x   0 lan        (501) wheel        (0)        0 2024-05-18 16:24:26.764948 tinyagent-0.1.1/tinyagent/agent/gpt/
--rw-r--r--   0 lan        (501) wheel        (0)        0 2024-05-18 16:24:07.000000 tinyagent-0.1.1/tinyagent/agent/gpt/__init__.py
--rw-r--r--   0 lan        (501) wheel        (0)     8668 2024-05-18 16:24:07.000000 tinyagent-0.1.1/tinyagent/agent/gpt/agent.py
--rw-r--r--   0 lan        (501) wheel        (0)     2371 2024-05-18 16:24:07.000000 tinyagent-0.1.1/tinyagent/agent/gpt/client.py
--rw-r--r--   0 lan        (501) wheel        (0)     2250 2024-05-18 15:22:41.000000 tinyagent-0.1.1/tinyagent/agent/schema.py
--rw-r--r--   0 lan        (501) wheel        (0)     2328 2024-05-18 15:22:41.000000 tinyagent-0.1.1/tinyagent/agent/tools.py
--rw-r--r--   0 lan        (501) wheel        (0)      191 2024-05-18 15:22:41.000000 tinyagent-0.1.1/tinyagent/agent/utils.py
-drwxr-xr-x   0 lan        (501) wheel        (0)        0 2024-05-18 16:24:26.765377 tinyagent-0.1.1/tinyagent/common/
--rw-r--r--   0 lan        (501) wheel        (0)       73 2024-05-18 15:22:41.000000 tinyagent-0.1.1/tinyagent/common/__init__.py
--rw-r--r--   0 lan        (501) wheel        (0)      358 2024-05-18 15:22:41.000000 tinyagent-0.1.1/tinyagent/common/event.py
--rw-r--r--   0 lan        (501) wheel        (0)      107 2024-05-18 15:22:41.000000 tinyagent-0.1.1/tinyagent/common/time.py
-drwxr-xr-x   0 lan        (501) wheel        (0)        0 2024-05-18 16:24:26.763165 tinyagent-0.1.1/tinyagent.egg-info/
--rw-r--r--   0 lan        (501) wheel        (0)      462 2024-05-18 16:24:26.000000 tinyagent-0.1.1/tinyagent.egg-info/PKG-INFO
--rw-r--r--   0 lan        (501) wheel        (0)      733 2024-05-18 16:24:26.000000 tinyagent-0.1.1/tinyagent.egg-info/SOURCES.txt
--rw-r--r--   0 lan        (501) wheel        (0)        1 2024-05-18 16:24:26.000000 tinyagent-0.1.1/tinyagent.egg-info/dependency_links.txt
--rw-r--r--   0 lan        (501) wheel        (0)       33 2024-05-18 16:24:26.000000 tinyagent-0.1.1/tinyagent.egg-info/requires.txt
--rw-r--r--   0 lan        (501) wheel        (0)       10 2024-05-18 16:24:26.000000 tinyagent-0.1.1/tinyagent.egg-info/top_level.txt
+drwxr-xr-x   0 lan        (501) wheel        (0)        0 2024-05-18 16:44:58.088589 tinyagent-0.1.2/
+-rw-r--r--   0 lan        (501) wheel        (0)      789 2024-05-18 16:38:39.000000 tinyagent-0.1.2/.gitignore
+-rw-r--r--   0 lan        (501) wheel        (0)     1069 2024-05-18 16:38:39.000000 tinyagent-0.1.2/LICENSE
+-rw-r--r--   0 lan        (501) wheel        (0)      462 2024-05-18 16:44:58.088459 tinyagent-0.1.2/PKG-INFO
+-rw-r--r--   0 lan        (501) wheel        (0)       83 2024-05-18 16:38:39.000000 tinyagent-0.1.2/README.md
+-rw-r--r--   0 lan        (501) wheel        (0)    32102 2024-05-18 16:38:39.000000 tinyagent-0.1.2/poetry.lock
+-rw-r--r--   0 lan        (501) wheel        (0)      303 2024-05-18 16:44:07.000000 tinyagent-0.1.2/pyproject.toml
+-rw-r--r--   0 lan        (501) wheel        (0)       38 2024-05-18 16:44:58.088624 tinyagent-0.1.2/setup.cfg
+-rw-r--r--   0 lan        (501) wheel        (0)      589 2024-05-18 16:43:46.000000 tinyagent-0.1.2/setup.py
+drwxr-xr-x   0 lan        (501) wheel        (0)        0 2024-05-18 16:44:58.085306 tinyagent-0.1.2/tests/
+drwxr-xr-x   0 lan        (501) wheel        (0)        0 2024-05-18 16:44:58.085515 tinyagent-0.1.2/tests/resources/
+-rw-r--r--   0 lan        (501) wheel        (0)      785 2024-05-18 16:38:39.000000 tinyagent-0.1.2/tests/resources/test.jpg
+-rw-r--r--   0 lan        (501) wheel        (0)     1987 2024-05-18 16:38:39.000000 tinyagent-0.1.2/tests/test_claude.py
+-rw-r--r--   0 lan        (501) wheel        (0)     1991 2024-05-18 16:38:39.000000 tinyagent-0.1.2/tests/test_gpt.py
+-rw-r--r--   0 lan        (501) wheel        (0)     1018 2024-05-18 16:38:39.000000 tinyagent-0.1.2/tests/test_tool.py
+drwxr-xr-x   0 lan        (501) wheel        (0)        0 2024-05-18 16:44:58.085657 tinyagent-0.1.2/tinyagent/
+-rw-r--r--   0 lan        (501) wheel        (0)      562 2024-05-18 16:38:39.000000 tinyagent-0.1.2/tinyagent/__init__.py
+drwxr-xr-x   0 lan        (501) wheel        (0)        0 2024-05-18 16:44:58.087051 tinyagent-0.1.2/tinyagent/agent/
+-rw-r--r--   0 lan        (501) wheel        (0)      385 2024-05-18 16:38:39.000000 tinyagent-0.1.2/tinyagent/agent/__init__.py
+-rw-r--r--   0 lan        (501) wheel        (0)     4114 2024-05-18 16:38:39.000000 tinyagent-0.1.2/tinyagent/agent/base.py
+drwxr-xr-x   0 lan        (501) wheel        (0)        0 2024-05-18 16:44:58.087530 tinyagent-0.1.2/tinyagent/agent/claude/
+-rw-r--r--   0 lan        (501) wheel        (0)        0 2024-05-18 16:38:39.000000 tinyagent-0.1.2/tinyagent/agent/claude/__init__..py
+-rw-r--r--   0 lan        (501) wheel        (0)     9002 2024-05-18 16:38:39.000000 tinyagent-0.1.2/tinyagent/agent/claude/agent.py
+-rw-r--r--   0 lan        (501) wheel        (0)     2333 2024-05-18 16:38:39.000000 tinyagent-0.1.2/tinyagent/agent/claude/client.py
+drwxr-xr-x   0 lan        (501) wheel        (0)        0 2024-05-18 16:44:58.087874 tinyagent-0.1.2/tinyagent/agent/gpt/
+-rw-r--r--   0 lan        (501) wheel        (0)        0 2024-05-18 16:38:39.000000 tinyagent-0.1.2/tinyagent/agent/gpt/__init__.py
+-rw-r--r--   0 lan        (501) wheel        (0)     8668 2024-05-18 16:38:39.000000 tinyagent-0.1.2/tinyagent/agent/gpt/agent.py
+-rw-r--r--   0 lan        (501) wheel        (0)     2371 2024-05-18 16:38:39.000000 tinyagent-0.1.2/tinyagent/agent/gpt/client.py
+-rw-r--r--   0 lan        (501) wheel        (0)     2250 2024-05-18 16:38:39.000000 tinyagent-0.1.2/tinyagent/agent/schema.py
+-rw-r--r--   0 lan        (501) wheel        (0)     2328 2024-05-18 16:38:39.000000 tinyagent-0.1.2/tinyagent/agent/tools.py
+-rw-r--r--   0 lan        (501) wheel        (0)      191 2024-05-18 16:38:39.000000 tinyagent-0.1.2/tinyagent/agent/utils.py
+drwxr-xr-x   0 lan        (501) wheel        (0)        0 2024-05-18 16:44:58.088279 tinyagent-0.1.2/tinyagent/common/
+-rw-r--r--   0 lan        (501) wheel        (0)       73 2024-05-18 16:38:39.000000 tinyagent-0.1.2/tinyagent/common/__init__.py
+-rw-r--r--   0 lan        (501) wheel        (0)      358 2024-05-18 16:38:39.000000 tinyagent-0.1.2/tinyagent/common/event.py
+-rw-r--r--   0 lan        (501) wheel        (0)      107 2024-05-18 16:38:39.000000 tinyagent-0.1.2/tinyagent/common/time.py
+drwxr-xr-x   0 lan        (501) wheel        (0)        0 2024-05-18 16:44:58.086271 tinyagent-0.1.2/tinyagent.egg-info/
+-rw-r--r--   0 lan        (501) wheel        (0)      462 2024-05-18 16:44:57.000000 tinyagent-0.1.2/tinyagent.egg-info/PKG-INFO
+-rw-r--r--   0 lan        (501) wheel        (0)      733 2024-05-18 16:44:58.000000 tinyagent-0.1.2/tinyagent.egg-info/SOURCES.txt
+-rw-r--r--   0 lan        (501) wheel        (0)        1 2024-05-18 16:44:57.000000 tinyagent-0.1.2/tinyagent.egg-info/dependency_links.txt
+-rw-r--r--   0 lan        (501) wheel        (0)       33 2024-05-18 16:44:57.000000 tinyagent-0.1.2/tinyagent.egg-info/requires.txt
+-rw-r--r--   0 lan        (501) wheel        (0)       10 2024-05-18 16:44:57.000000 tinyagent-0.1.2/tinyagent.egg-info/top_level.txt
```

### Comparing `tinyagent-0.1.1/.gitignore` & `tinyagent-0.1.2/.gitignore`

 * *Files identical despite different names*

### Comparing `tinyagent-0.1.1/LICENSE` & `tinyagent-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `tinyagent-0.1.1/poetry.lock` & `tinyagent-0.1.2/poetry.lock`

 * *Files identical despite different names*

### Comparing `tinyagent-0.1.1/setup.py` & `tinyagent-0.1.2/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="tinyagent",
-    version="0.1.1",
+    version="0.1.2",
     author="y-lan",
     author_email="lanyuyang@gmail.com",
     description="A minimalistic agent framework",
     long_description=open("README.md").read(),
     url="https://github.com/y-lan/tinyagent",
     packages=find_packages(),
     install_requires=["pydantic>=2.7.1", "requests>=2.31.0"],
```

### Comparing `tinyagent-0.1.1/tests/resources/test.jpg` & `tinyagent-0.1.2/tests/resources/test.jpg`

 * *Files identical despite different names*

### Comparing `tinyagent-0.1.1/tests/test_claude.py` & `tinyagent-0.1.2/tests/test_claude.py`

 * *Files identical despite different names*

### Comparing `tinyagent-0.1.1/tests/test_gpt.py` & `tinyagent-0.1.2/tests/test_gpt.py`

 * *Files identical despite different names*

### Comparing `tinyagent-0.1.1/tests/test_tool.py` & `tinyagent-0.1.2/tests/test_tool.py`

 * *Files identical despite different names*

### Comparing `tinyagent-0.1.1/tinyagent/__init__.py` & `tinyagent-0.1.2/tinyagent/__init__.py`

 * *Files identical despite different names*

### Comparing `tinyagent-0.1.1/tinyagent/agent/base.py` & `tinyagent-0.1.2/tinyagent/agent/base.py`

 * *Files identical despite different names*

### Comparing `tinyagent-0.1.1/tinyagent/agent/claude/agent.py` & `tinyagent-0.1.2/tinyagent/agent/claude/agent.py`

 * *Files identical despite different names*

### Comparing `tinyagent-0.1.1/tinyagent/agent/claude/client.py` & `tinyagent-0.1.2/tinyagent/agent/claude/client.py`

 * *Files identical despite different names*

### Comparing `tinyagent-0.1.1/tinyagent/agent/gpt/agent.py` & `tinyagent-0.1.2/tinyagent/agent/gpt/agent.py`

 * *Files identical despite different names*

### Comparing `tinyagent-0.1.1/tinyagent/agent/gpt/client.py` & `tinyagent-0.1.2/tinyagent/agent/gpt/client.py`

 * *Files identical despite different names*

### Comparing `tinyagent-0.1.1/tinyagent/agent/schema.py` & `tinyagent-0.1.2/tinyagent/agent/schema.py`

 * *Files identical despite different names*

### Comparing `tinyagent-0.1.1/tinyagent/agent/tools.py` & `tinyagent-0.1.2/tinyagent/agent/tools.py`

 * *Files identical despite different names*

### Comparing `tinyagent-0.1.1/tinyagent.egg-info/SOURCES.txt` & `tinyagent-0.1.2/tinyagent.egg-info/SOURCES.txt`

 * *Files identical despite different names*

