# Comparing `tmp/zhihubackup-0.2.1.tar.gz` & `tmp/zhihubackup-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zhihubackup-0.2.1.tar", last modified: Thu Oct  5 07:25:12 2023, max compression
+gzip compressed data, was "zhihubackup-0.2.2.tar", last modified: Fri May 17 22:22:48 2024, max compression
```

## Comparing `zhihubackup-0.2.1.tar` & `zhihubackup-0.2.2.tar`

### file list

```diff
@@ -1,27 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-05 07:25:12.503520 zhihubackup-0.2.1/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-05 07:25:12.499520 zhihubackup-0.2.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-05 07:25:12.499520 zhihubackup-0.2.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      621 2023-10-05 07:24:58.000000 zhihubackup-0.2.1/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (127)      399 2023-10-05 07:24:58.000000 zhihubackup-0.2.1/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3078 2023-10-05 07:24:58.000000 zhihubackup-0.2.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      926 2023-10-05 07:24:58.000000 zhihubackup-0.2.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     7652 2023-10-05 07:24:58.000000 zhihubackup-0.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    10799 2023-10-05 07:25:12.503520 zhihubackup-0.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      788 2023-10-05 07:24:58.000000 zhihubackup-0.2.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       63 2023-10-05 07:24:58.000000 zhihubackup-0.2.1/example.py
--rw-r--r--   0 runner    (1001) docker     (127)     2230 2023-10-05 07:24:58.000000 zhihubackup-0.2.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-10-05 07:25:12.503520 zhihubackup-0.2.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-05 07:25:12.499520 zhihubackup-0.2.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      481 2023-10-05 07:24:58.000000 zhihubackup-0.2.1/tests/test_backup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-05 07:25:12.499520 zhihubackup-0.2.1/zhihubackup/
--rw-r--r--   0 runner    (1001) docker     (127)       69 2023-10-05 07:24:58.000000 zhihubackup-0.2.1/zhihubackup/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3366 2023-10-05 07:24:58.000000 zhihubackup-0.2.1/zhihubackup/backup.py
--rw-r--r--   0 runner    (1001) docker     (127)      239 2023-10-05 07:24:58.000000 zhihubackup-0.2.1/zhihubackup/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     5570 2023-10-05 07:24:58.000000 zhihubackup-0.2.1/zhihubackup/xzse96.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-05 07:25:12.499520 zhihubackup-0.2.1/zhihubackup.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    10799 2023-10-05 07:25:12.000000 zhihubackup-0.2.1/zhihubackup.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      455 2023-10-05 07:25:12.000000 zhihubackup-0.2.1/zhihubackup.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-05 07:25:12.000000 zhihubackup-0.2.1/zhihubackup.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-10-05 07:25:12.000000 zhihubackup-0.2.1/zhihubackup.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       61 2023-10-05 07:25:12.000000 zhihubackup-0.2.1/zhihubackup.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2023-10-05 07:25:12.000000 zhihubackup-0.2.1/zhihubackup.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 22:22:48.059993 zhihubackup-0.2.2/
+-rw-r--r--   0 runner    (1001) docker     (127)      125 2024-05-17 22:22:43.000000 zhihubackup-0.2.2/.git_archival.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-17 22:22:43.000000 zhihubackup-0.2.2/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 22:22:48.051993 zhihubackup-0.2.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 22:22:48.055993 zhihubackup-0.2.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      621 2024-05-17 22:22:43.000000 zhihubackup-0.2.2/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      457 2024-05-17 22:22:43.000000 zhihubackup-0.2.2/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3078 2024-05-17 22:22:43.000000 zhihubackup-0.2.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      838 2024-05-17 22:22:43.000000 zhihubackup-0.2.2/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     7652 2024-05-17 22:22:43.000000 zhihubackup-0.2.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    10686 2024-05-17 22:22:48.059993 zhihubackup-0.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      695 2024-05-17 22:22:43.000000 zhihubackup-0.2.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-17 22:22:43.000000 zhihubackup-0.2.2/example.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2235 2024-05-17 22:22:43.000000 zhihubackup-0.2.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-17 22:22:48.059993 zhihubackup-0.2.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 22:22:48.055993 zhihubackup-0.2.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      481 2024-05-17 22:22:43.000000 zhihubackup-0.2.2/tests/test_backup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 22:22:48.055993 zhihubackup-0.2.2/zhihubackup/
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-17 22:22:43.000000 zhihubackup-0.2.2/zhihubackup/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3534 2024-05-17 22:22:43.000000 zhihubackup-0.2.2/zhihubackup/backup.py
+-rw-r--r--   0 runner    (1001) docker     (127)      239 2024-05-17 22:22:43.000000 zhihubackup-0.2.2/zhihubackup/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5570 2024-05-17 22:22:43.000000 zhihubackup-0.2.2/zhihubackup/xzse96.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 22:22:48.055993 zhihubackup-0.2.2/zhihubackup.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    10686 2024-05-17 22:22:48.000000 zhihubackup-0.2.2/zhihubackup.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      488 2024-05-17 22:22:48.000000 zhihubackup-0.2.2/zhihubackup.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-17 22:22:48.000000 zhihubackup-0.2.2/zhihubackup.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-17 22:22:48.000000 zhihubackup-0.2.2/zhihubackup.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-17 22:22:48.000000 zhihubackup-0.2.2/zhihubackup.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-17 22:22:48.000000 zhihubackup-0.2.2/zhihubackup.egg-info/top_level.txt
```

### Comparing `zhihubackup-0.2.1/.github/workflows/release.yml` & `zhihubackup-0.2.2/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `zhihubackup-0.2.1/.gitignore` & `zhihubackup-0.2.2/.gitignore`

 * *Files identical despite different names*

### Comparing `zhihubackup-0.2.1/.pre-commit-config.yaml` & `zhihubackup-0.2.2/.pre-commit-config.yaml`

 * *Files 10% similar despite different names*

```diff
@@ -1,32 +1,29 @@
 # See https://pre-commit.com for more information
 # See https://pre-commit.com/hooks.html for more hooks
 repos:
 -   repo: https://github.com/pre-commit/pre-commit-hooks
-    rev: v4.4.0
+    rev: v4.6.0
     hooks:
     -   id: trailing-whitespace
     -   id: end-of-file-fixer
     -   id: check-yaml
     -   id: check-json
     -   id: check-added-large-files
     -   id: check-merge-conflict
     -   id: check-symlinks
     -   id: check-toml
 # Python
--   repo: https://github.com/psf/black-pre-commit-mirror
-    rev: 23.9.1
-    hooks:
-    - id: black-jupyter
 -   repo: https://github.com/astral-sh/ruff-pre-commit
     # Ruff version.
-    rev: v0.0.290
+    rev: v0.4.4
     hooks:
     - id: ruff
       args: ["--fix"]
+    - id: ruff-format
 # numpydoc
 -   repo: https://github.com/Carreau/velin
     rev: 0.0.12
     hooks:
     - id: velin
       args: ["--write"]
 # Python inside docs
```

### Comparing `zhihubackup-0.2.1/LICENSE` & `zhihubackup-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `zhihubackup-0.2.1/PKG-INFO` & `zhihubackup-0.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zhihubackup
-Version: 0.2.1
+Version: 0.2.2
 Summary: Backup your Zhihu contents before quitting Zhihu.
 Author-email: Jinzhe Zeng <jinzhe.zeng@rutgers.edu>
 License:                    GNU LESSER GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -181,32 +181,29 @@
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: requests
 Requires-Dist: tqdm
-Provides-Extra: node
-Requires-Dist: nodejs-wheel; extra == "node"
+Requires-Dist: nodejs-wheel-binaries>=20.13.1
 Provides-Extra: test
 Requires-Dist: pytest; extra == "test"
 Requires-Dist: pytest-cov; extra == "test"
 
 # 退乎前备份知乎回答：zhihubackup
 
 每个知乎答主都有退乎的梦想，但退乎前如果删光回答，则十分可惜。因此，我用Python写了60行的脚本，可以在退乎前备份自己的所有回答和文章，以免事后后悔。
 
 ## 安装
 
 ```sh
-pip install zhihubackup[node]
+pip install zhihubackup
 ```
 
-如果已安装[Node.js](https://github.com/nodejs/node)，则可以去掉`[node]`。
-
 ## 使用
 
 假如你是@贱贱，你的id是`splitter`，那么可以执行命令：
 
 ```sh
 zhihubackup splitter
 ```
```

### Comparing `zhihubackup-0.2.1/README.md` & `zhihubackup-0.2.2/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,19 +1,17 @@
 # 退乎前备份知乎回答：zhihubackup
 
 每个知乎答主都有退乎的梦想，但退乎前如果删光回答，则十分可惜。因此，我用Python写了60行的脚本，可以在退乎前备份自己的所有回答和文章，以免事后后悔。
 
 ## 安装
 
 ```sh
-pip install zhihubackup[node]
+pip install zhihubackup
 ```
 
-如果已安装[Node.js](https://github.com/nodejs/node)，则可以去掉`[node]`。
-
 ## 使用
 
 假如你是@贱贱，你的id是`splitter`，那么可以执行命令：
 
 ```sh
 zhihubackup splitter
 ```
```

### Comparing `zhihubackup-0.2.1/pyproject.toml` & `zhihubackup-0.2.2/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [build-system]
-requires = ["setuptools>=61", "setuptools_scm[toml]>=6.2"]
+requires = ["setuptools>=61", "setuptools_scm[toml]>=7"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "zhihubackup"
 dynamic = ["version"]
 description = "Backup your Zhihu contents before quitting Zhihu."
 authors = [
@@ -20,29 +20,27 @@
     "Operating System :: MacOS :: MacOS X",
     "Operating System :: Microsoft :: Windows",
     "License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)",
 ]
 dependencies = [
     "requests",
     "tqdm",
+    "nodejs-wheel-binaries>=20.13.1",
 ]
 requires-python = ">=3.7"
 readme = "README.md"
 keywords = ["zhihu"]
 
 [project.urls]
 repository = "https://github.com/njzjz/zhihubackup"
 
 [project.scripts]
 zhihubackup = "zhihubackup.cli:main"
 
 [project.optional-dependencies]
-node = [
-    "nodejs-wheel",
-]
 test = [
     "pytest",
     "pytest-cov",
 ]
 
 [tool.setuptools.packages.find]
 include = ["zhihubackup*"]
```

### Comparing `zhihubackup-0.2.1/zhihubackup/backup.py` & `zhihubackup-0.2.2/zhihubackup/backup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,31 @@
 import json
 import os
 import subprocess
 
 import requests
+from nodejs_wheel import (
+    node,
+)
 from tqdm import tqdm
 
 
 def xzse96(path: str, d_c0: str):
-    return subprocess.check_output(
-        ["node", os.path.join(__file__, "..", "xzse96.js"), path, d_c0]
+    completed_process = node(
+        [os.path.join(__file__, "..", "xzse96.js"), path, d_c0],
+        return_completed_process=True,
+        check=True,
+        stdout=subprocess.PIPE,
+        text=True,
     )
+    return completed_process.stdout
 
 
 def act_api(username):
-    return "https://www.zhihu.com/api/v3/moments/%s/activities?desktop=true" % username
+    return f"https://www.zhihu.com/api/v3/moments/{username}/activities?desktop=true"
 
 
 def get_cookie(username):
     headers = {
         "User-Agent": "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/87.0.4280.141 Safari/537.36 Edg/87.0.664.75",
     }
     r = requests.get(f"https://www.zhihu.com/people/{username}", headers=headers)
@@ -71,15 +79,15 @@
                         saved.append(str(target[saved_type]))
                     else:
                         for tt in target[saved_type]:
                             for saved_type2 in ("content", "url"):
                                 if saved_type2 in tt:
                                     saved.append(tt[saved_type2])
             with open(
-                os.path.join(username, target_type, "%s.txt" % target["id"]),
+                os.path.join(username, target_type, f"{target['id']}.txt"),
                 "w",
                 encoding="utf-8",
             ) as f:
                 f.write("\n".join(saved))
             t.update(1)
         # paging: is_end next previous
         paging = jdata["paging"]
```

### Comparing `zhihubackup-0.2.1/zhihubackup/xzse96.js` & `zhihubackup-0.2.2/zhihubackup/xzse96.js`

 * *Files identical despite different names*

### Comparing `zhihubackup-0.2.1/zhihubackup.egg-info/PKG-INFO` & `zhihubackup-0.2.2/zhihubackup.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zhihubackup
-Version: 0.2.1
+Version: 0.2.2
 Summary: Backup your Zhihu contents before quitting Zhihu.
 Author-email: Jinzhe Zeng <jinzhe.zeng@rutgers.edu>
 License:                    GNU LESSER GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -181,32 +181,29 @@
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: requests
 Requires-Dist: tqdm
-Provides-Extra: node
-Requires-Dist: nodejs-wheel; extra == "node"
+Requires-Dist: nodejs-wheel-binaries>=20.13.1
 Provides-Extra: test
 Requires-Dist: pytest; extra == "test"
 Requires-Dist: pytest-cov; extra == "test"
 
 # 退乎前备份知乎回答：zhihubackup
 
 每个知乎答主都有退乎的梦想，但退乎前如果删光回答，则十分可惜。因此，我用Python写了60行的脚本，可以在退乎前备份自己的所有回答和文章，以免事后后悔。
 
 ## 安装
 
 ```sh
-pip install zhihubackup[node]
+pip install zhihubackup
 ```
 
-如果已安装[Node.js](https://github.com/nodejs/node)，则可以去掉`[node]`。
-
 ## 使用
 
 假如你是@贱贱，你的id是`splitter`，那么可以执行命令：
 
 ```sh
 zhihubackup splitter
 ```
```

