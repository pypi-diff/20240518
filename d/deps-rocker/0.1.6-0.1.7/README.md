# Comparing `tmp/deps_rocker-0.1.6.tar.gz` & `tmp/deps_rocker-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deps_rocker-0.1.6.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "deps_rocker-0.1.7.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `deps_rocker-0.1.6.tar` & `deps_rocker-0.1.7.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     7090 2024-05-17 15:16:31.637214 deps_rocker-0.1.6/README.md
--rw-r--r--   0        0        0        0 2024-05-17 15:16:31.637214 deps_rocker-0.1.6/deps_rocker/__init__.py
--rw-r--r--   0        0        0     1097 2024-05-17 15:16:31.637214 deps_rocker-0.1.6/deps_rocker/command_layer.py
--rw-r--r--   0        0        0      128 2024-05-17 15:16:31.637214 deps_rocker-0.1.6/deps_rocker/dep_rocker_cli.py
--rw-r--r--   0        0        0     6772 2024-05-17 15:16:31.637214 deps_rocker-0.1.6/deps_rocker/dependencies.py
--rw-r--r--   0        0        0      226 2024-05-17 15:16:31.637214 deps_rocker-0.1.6/deps_rocker/templates/add-apt-repository_snippet.Dockerfile
--rw-r--r--   0        0        0      205 2024-05-17 15:16:31.637214 deps_rocker-0.1.6/deps_rocker/templates/apt_snippet.Dockerfile
--rw-r--r--   0        0        0       85 2024-05-17 15:16:31.637214 deps_rocker-0.1.6/deps_rocker/templates/env_snippet.Dockerfile
--rw-r--r--   0        0        0      118 2024-05-17 15:16:31.637214 deps_rocker-0.1.6/deps_rocker/templates/pip_snippet.Dockerfile
--rw-r--r--   0        0        0      104 2024-05-17 15:16:31.637214 deps_rocker-0.1.6/deps_rocker/templates/pyproject_snippet.Dockerfile
--rw-r--r--   0        0        0       99 2024-05-17 15:16:31.637214 deps_rocker-0.1.6/deps_rocker/templates/run_snippet.Dockerfile
--rw-r--r--   0        0        0       77 2024-05-17 15:16:31.637214 deps_rocker-0.1.6/deps_rocker/templates/script_snippet.Dockerfile
--rw-r--r--   0        0        0     2292 2024-05-17 15:16:31.641214 deps_rocker-0.1.6/pyproject.toml
--rw-r--r--   0        0        0     7952 1970-01-01 00:00:00.000000 deps_rocker-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0     7139 2024-05-17 16:39:34.480766 deps_rocker-0.1.7/README.md
+-rw-r--r--   0        0        0        0 2024-05-17 16:39:34.480766 deps_rocker-0.1.7/deps_rocker/__init__.py
+-rw-r--r--   0        0        0     1097 2024-05-17 16:39:34.480766 deps_rocker-0.1.7/deps_rocker/command_layer.py
+-rw-r--r--   0        0        0      128 2024-05-17 16:39:34.480766 deps_rocker-0.1.7/deps_rocker/dep_rocker_cli.py
+-rw-r--r--   0        0        0     7392 2024-05-17 16:39:34.480766 deps_rocker-0.1.7/deps_rocker/dependencies.py
+-rw-r--r--   0        0        0      226 2024-05-17 16:39:34.480766 deps_rocker-0.1.7/deps_rocker/templates/add-apt-repository_snippet.Dockerfile
+-rw-r--r--   0        0        0      205 2024-05-17 16:39:34.480766 deps_rocker-0.1.7/deps_rocker/templates/apt_snippet.Dockerfile
+-rw-r--r--   0        0        0       85 2024-05-17 16:39:34.480766 deps_rocker-0.1.7/deps_rocker/templates/env_snippet.Dockerfile
+-rw-r--r--   0        0        0      118 2024-05-17 16:39:34.480766 deps_rocker-0.1.7/deps_rocker/templates/pip_snippet.Dockerfile
+-rw-r--r--   0        0        0      104 2024-05-17 16:39:34.480766 deps_rocker-0.1.7/deps_rocker/templates/pyproject_snippet.Dockerfile
+-rw-r--r--   0        0        0       99 2024-05-17 16:39:34.480766 deps_rocker-0.1.7/deps_rocker/templates/run_snippet.Dockerfile
+-rw-r--r--   0        0        0       77 2024-05-17 16:39:34.480766 deps_rocker-0.1.7/deps_rocker/templates/script_snippet.Dockerfile
+-rw-r--r--   0        0        0     2292 2024-05-17 16:39:34.480766 deps_rocker-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0     8001 1970-01-01 00:00:00.000000 deps_rocker-0.1.7/PKG-INFO
```

### Comparing `deps_rocker-0.1.6/README.md` & `deps_rocker-0.1.7/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,29 +1,34 @@
 # deps_rocker
 
 ## Continuous Integration Status
 
-[![Ci](https://github.com/blooop/python_template/actions/workflows/ci.yml/badge.svg?branch=main)](https://github.com/blooop/python_template/actions/workflows/ci.yml?query=branch%3Amain)
-[![Codecov](https://codecov.io/gh/blooop/python_template/branch/main/graph/badge.svg?token=Y212GW1PG6)](https://codecov.io/gh/blooop/python_template)
-[![GitHub issues](https://img.shields.io/github/issues/blooop/python_template.svg)](https://GitHub.com/blooop/python_template/issues/)
-[![GitHub pull-requests merged](https://badgen.net/github/merged-prs/blooop/python_template)](https://github.com/blooop/python_template/pulls?q=is%3Amerged)
-[![GitHub release](https://img.shields.io/github/release/blooop/python_template.svg)](https://GitHub.com/blooop/python_template/releases/)
+[![Ci](https://github.com/blooop/deps_rocker/actions/workflows/ci.yml/badge.svg?branch=main)](https://github.com/blooop/deps_rocker/actions/workflows/ci.yml?query=branch%3Amain)
+[![Codecov](https://codecov.io/gh/blooop/deps_rocker/branch/main/graph/badge.svg?token=Y212GW1PG6)](https://codecov.io/gh/blooop/deps_rocker)
+[![GitHub issues](https://img.shields.io/github/issues/blooop/deps_rocker.svg)](https://GitHub.com/blooop/deps_rocker/issues/)
+[![GitHub pull-requests merged](https://badgen.net/github/merged-prs/blooop/deps_rocker)](https://github.com/blooop/deps_rocker/pulls?q=is%3Amerged)
+[![GitHub release](https://img.shields.io/github/release/blooop/deps_rocker.svg)](https://GitHub.com/blooop/deps_rocker/releases/)
 [![License](https://img.shields.io/pypi/l/bencher)](https://opensource.org/license/mit/)
 [![Python](https://img.shields.io/badge/python-3.10-blue)](https://www.python.org/downloads/release/python-310/)
 
 ## Installation
 
 ```
 pip install deps-rocker
 ```
 
 ## Usage
 
 ```
-rocker --deps-dependencies ubuntu:22.04
+rocker --deps ubuntu:22.04
+#or
+rocker --deps "specific_pkg.deps.yaml" ubuntu:22.04
+#or
+rocker --deps "*.deps.yaml" ubuntu:22.04
+
 ```
 
 ## Motivation
 
 Docker enables easy isolation of dependencies from the host system, but it is not easy to dynamically combine docker files from separate projects into a single unified environment.
```

### Comparing `deps_rocker-0.1.6/deps_rocker/command_layer.py` & `deps_rocker-0.1.7/deps_rocker/command_layer.py`

 * *Files identical despite different names*

### Comparing `deps_rocker-0.1.6/deps_rocker/dependencies.py` & `deps_rocker-0.1.7/deps_rocker/dependencies.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,34 +3,43 @@
 import yaml
 import toml
 from rocker.extensions import RockerExtension
 from .command_layer import CommandLayer
 
 
 class Dependencies(RockerExtension):
-    name = "deps_dependencies"
+    name = "deps"
 
-    def __init__(self, pattern: str = "*deps.yaml", path: Path = None) -> None:
-        if path is None:
-            path = Path.cwd()
+    def __init__(self) -> None:
         self.deps_files = []
         self.dependencies = defaultdict(set)
         self.layers_preamble = defaultdict(CommandLayer)
         self.layers = defaultdict(CommandLayer)
         self.layers_user = defaultdict(CommandLayer)
         self.dep_group_order = defaultdict(list)
         self.empy_args = {}
         self.all_files = {}
-        self.read_dependencies(path, pattern)
+        self.parsed = False
         super().__init__()
 
     @classmethod
     def get_name(cls):
         return cls.name
 
+    def setup_deps(self, cliargs):
+        if not self.parsed:
+            if cliargs is not None:
+                file_filter = cliargs["deps"]
+                # if ".deps.yaml" not in file_filter:
+                # file_filter += ".deps.yaml"
+            else:
+                file_filter = "*.deps.yaml"
+            self.read_dependencies(Path.cwd(), file_filter)
+            self.parsed = True
+
     def read_dependencies(self, path: Path, pattern: str):
         """Recursivly load all deps.yaml and create a dictionary containing sets of each type of dependency. Each type of dependency (apt_base, apt etc) should have duplicates rejected when adding to the set"""
         for p in path.rglob(pattern):
             print(f"found {p}")
             self.deps_files.append(p)
             with open(p, "r", encoding="utf-8") as file:
                 vals = yaml.safe_load(file)
@@ -72,14 +81,15 @@
             dep_list = list(sorted(self.dependencies[key]))
             if as_list:
                 return dep_list
             return " ".join(dep_list)
         return ""
 
     def get_files(self, cliargs) -> dict:
+        """Get a dict of local filenames and content to write into them"""
         print("Getting files")
 
         self.add_file("pyproject_default", self.get_pyproject_toml_deps())
 
         all_layers = (
             list(self.layers_preamble.values())
             + list(self.layers.values())
@@ -152,23 +162,33 @@
                         pyproj_deps.extend(optional["dev"])
         return " ".join(pyproj_deps)
 
     def get_preamble(self, cliargs):
         return "\n".join([lay.to_snippet() for lay in self.layers_preamble.values()])
 
     def get_snippet(self, cliargs=None):
+        self.setup_deps(cliargs)
         return "\n".join([lay.to_snippet() for lay in self.layers.values()])
 
-    def get_user_snippet(self, cliargs):  # pylint: disable=unused-argument
+    def get_user_snippet(self, cliargs):
         """Get a dockerfile snippet to be executed after switchingto the expected USER."""
+        self.setup_deps(cliargs)
         return "\n".join([lay.to_snippet() for lay in self.layers_user.values()])
 
     @staticmethod
     def register_arguments(parser, defaults=None):
-        parser.add_argument("--deps-dependencies", action="store_true", help="install deps.yaml ")
+        # parser.add_argument("--deps", action="store_true", help="install all deps.yaml ")
+        parser.add_argument(
+            "--deps",
+            type=str,
+            nargs="?",
+            const="*.deps.yaml",
+            help="A filter to select deps.yaml files. Defaults to *.deps.yaml",
+            # default="*.deps.yaml",
+        )
 
 
 if __name__ == "__main__":
     deps = Dependencies()
     # print(deps)
 
     # scr= deps
```

### Comparing `deps_rocker-0.1.6/pyproject.toml` & `deps_rocker-0.1.7/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "deps_rocker"
-version = "0.1.6"
+version = "0.1.7"
 license = { text = "MIT" }
 
 authors = [{ name = "Austin Gregg-Smith", email = "blooop@gmail.com" }]
 description = "A rocker plugin to help installing apt and pip dependencies"
 readme = "README.md"
 
 requires-python = ">=3.10"
```

### Comparing `deps_rocker-0.1.6/PKG-INFO` & `deps_rocker-0.1.7/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deps_rocker
-Version: 0.1.6
+Version: 0.1.7
 Summary: A rocker plugin to help installing apt and pip dependencies
 Author-email: Austin Gregg-Smith <blooop@gmail.com>
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Requires-Dist: rocker
 Requires-Dist: pyyaml
 Requires-Dist: off-your-rocker
@@ -20,32 +20,37 @@
 Project-URL: Source, https://github.com/blooop/deps_rocker
 Provides-Extra: test
 
 # deps_rocker
 
 ## Continuous Integration Status
 
-[![Ci](https://github.com/blooop/python_template/actions/workflows/ci.yml/badge.svg?branch=main)](https://github.com/blooop/python_template/actions/workflows/ci.yml?query=branch%3Amain)
-[![Codecov](https://codecov.io/gh/blooop/python_template/branch/main/graph/badge.svg?token=Y212GW1PG6)](https://codecov.io/gh/blooop/python_template)
-[![GitHub issues](https://img.shields.io/github/issues/blooop/python_template.svg)](https://GitHub.com/blooop/python_template/issues/)
-[![GitHub pull-requests merged](https://badgen.net/github/merged-prs/blooop/python_template)](https://github.com/blooop/python_template/pulls?q=is%3Amerged)
-[![GitHub release](https://img.shields.io/github/release/blooop/python_template.svg)](https://GitHub.com/blooop/python_template/releases/)
+[![Ci](https://github.com/blooop/deps_rocker/actions/workflows/ci.yml/badge.svg?branch=main)](https://github.com/blooop/deps_rocker/actions/workflows/ci.yml?query=branch%3Amain)
+[![Codecov](https://codecov.io/gh/blooop/deps_rocker/branch/main/graph/badge.svg?token=Y212GW1PG6)](https://codecov.io/gh/blooop/deps_rocker)
+[![GitHub issues](https://img.shields.io/github/issues/blooop/deps_rocker.svg)](https://GitHub.com/blooop/deps_rocker/issues/)
+[![GitHub pull-requests merged](https://badgen.net/github/merged-prs/blooop/deps_rocker)](https://github.com/blooop/deps_rocker/pulls?q=is%3Amerged)
+[![GitHub release](https://img.shields.io/github/release/blooop/deps_rocker.svg)](https://GitHub.com/blooop/deps_rocker/releases/)
 [![License](https://img.shields.io/pypi/l/bencher)](https://opensource.org/license/mit/)
 [![Python](https://img.shields.io/badge/python-3.10-blue)](https://www.python.org/downloads/release/python-310/)
 
 ## Installation
 
 ```
 pip install deps-rocker
 ```
 
 ## Usage
 
 ```
-rocker --deps-dependencies ubuntu:22.04
+rocker --deps ubuntu:22.04
+#or
+rocker --deps "specific_pkg.deps.yaml" ubuntu:22.04
+#or
+rocker --deps "*.deps.yaml" ubuntu:22.04
+
 ```
 
 ## Motivation
 
 Docker enables easy isolation of dependencies from the host system, but it is not easy to dynamically combine docker files from separate projects into a single unified environment.
```

