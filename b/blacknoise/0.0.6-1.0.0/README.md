# Comparing `tmp/blacknoise-0.0.6.tar.gz` & `tmp/blacknoise-1.0.0.tar.gz`

## Comparing `blacknoise-0.0.6.tar` & `blacknoise-1.0.0.tar`

### file list

```diff
@@ -1,17 +1,18 @@
--rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 blacknoise-0.0.6/.editorconfig
--rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 blacknoise-0.0.6/.pre-commit-config.yaml
--rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 blacknoise-0.0.6/src/blacknoise/__about__.py
--rw-r--r--   0        0        0      214 2020-02-02 00:00:00.000000 blacknoise-0.0.6/src/blacknoise/__init__.py
--rw-r--r--   0        0        0     5656 2020-02-02 00:00:00.000000 blacknoise-0.0.6/src/blacknoise/_impl.py
--rw-r--r--   0        0        0     2780 2020-02-02 00:00:00.000000 blacknoise-0.0.6/src/blacknoise/compress.py
--rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 blacknoise-0.0.6/tests/__init__.py
--rw-r--r--   0        0        0     5768 2020-02-02 00:00:00.000000 blacknoise-0.0.6/tests/test_blacknoise.py
--rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 blacknoise-0.0.6/tests/static/hello.txt
--rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 blacknoise-0.0.6/tests/static/hello.txt.gz
--rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 blacknoise-0.0.6/tests/static/hello2.txt.gz
--rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 blacknoise-0.0.6/tests/static/hello3.txt
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 blacknoise-0.0.6/.gitignore
--rw-r--r--   0        0        0     1101 2020-02-02 00:00:00.000000 blacknoise-0.0.6/LICENSE.txt
--rw-r--r--   0        0        0     3012 2020-02-02 00:00:00.000000 blacknoise-0.0.6/README.md
--rw-r--r--   0        0        0     2806 2020-02-02 00:00:00.000000 blacknoise-0.0.6/pyproject.toml
--rw-r--r--   0        0        0     3935 2020-02-02 00:00:00.000000 blacknoise-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 blacknoise-1.0.0/.editorconfig
+-rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 blacknoise-1.0.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 blacknoise-1.0.0/CHANGELOG.md
+-rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 blacknoise-1.0.0/src/blacknoise/__about__.py
+-rw-r--r--   0        0        0      214 2020-02-02 00:00:00.000000 blacknoise-1.0.0/src/blacknoise/__init__.py
+-rw-r--r--   0        0        0     5656 2020-02-02 00:00:00.000000 blacknoise-1.0.0/src/blacknoise/_impl.py
+-rw-r--r--   0        0        0     2608 2020-02-02 00:00:00.000000 blacknoise-1.0.0/src/blacknoise/compress.py
+-rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 blacknoise-1.0.0/tests/__init__.py
+-rw-r--r--   0        0        0     5768 2020-02-02 00:00:00.000000 blacknoise-1.0.0/tests/test_blacknoise.py
+-rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 blacknoise-1.0.0/tests/static/hello.txt
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 blacknoise-1.0.0/tests/static/hello.txt.gz
+-rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 blacknoise-1.0.0/tests/static/hello2.txt.gz
+-rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 blacknoise-1.0.0/tests/static/hello3.txt
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 blacknoise-1.0.0/.gitignore
+-rw-r--r--   0        0        0     1101 2020-02-02 00:00:00.000000 blacknoise-1.0.0/LICENSE.txt
+-rw-r--r--   0        0        0     3181 2020-02-02 00:00:00.000000 blacknoise-1.0.0/README.md
+-rw-r--r--   0        0        0     2827 2020-02-02 00:00:00.000000 blacknoise-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0     4104 2020-02-02 00:00:00.000000 blacknoise-1.0.0/PKG-INFO
```

### Comparing `blacknoise-0.0.6/.pre-commit-config.yaml` & `blacknoise-1.0.0/.pre-commit-config.yaml`

 * *Files 3% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 exclude: ".yarn/|yarn.lock|\\.min\\.(css|js)$"
 repos:
   - repo: https://github.com/pre-commit/pre-commit-hooks
-    rev: v4.5.0
+    rev: v4.6.0
     hooks:
       - id: check-added-large-files
       - id: check-builtin-literals
       - id: check-executables-have-shebangs
       - id: check-merge-conflict
       - id: check-toml
       - id: check-yaml
       - id: detect-private-key
       - id: end-of-file-fixer
       - id: mixed-line-ending
       - id: trailing-whitespace
   - repo: https://github.com/astral-sh/ruff-pre-commit
-    rev: "v0.3.3"
+    rev: "v0.4.4"
     hooks:
       - id: ruff
       - id: ruff-format
   - repo: https://github.com/pre-commit/mirrors-prettier
     rev: v4.0.0-alpha.8
     hooks:
       - id: prettier
         entry: env PRETTIER_LEGACY_CLI=1 prettier
         types_or: [javascript, css, markdown]
         args: [--no-semi]
         exclude: "^conf/|.*\\.html$"
   - repo: https://github.com/tox-dev/pyproject-fmt
-    rev: 1.5.3
+    rev: 2.1.1
     hooks:
       - id: pyproject-fmt
   - repo: https://github.com/abravalheri/validate-pyproject
-    rev: v0.15
+    rev: v0.17
     hooks:
       - id: validate-pyproject
```

### Comparing `blacknoise-0.0.6/src/blacknoise/_impl.py` & `blacknoise-1.0.0/src/blacknoise/_impl.py`

 * *Files identical despite different names*

### Comparing `blacknoise-0.0.6/src/blacknoise/compress.py` & `blacknoise-1.0.0/src/blacknoise/compress.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 import argparse
-from concurrent.futures import ThreadPoolExecutor, wait
 import gzip
 import io
-from itertools import cycle
 import os
+from concurrent.futures import ThreadPoolExecutor
 from pathlib import Path
 
 try:
     import brotli
 except ModuleNotFoundError:  # no cov
     brotli = None
 
@@ -48,20 +47,21 @@
 )
 
 
 def _write_if_smaller(path, orig_bytes, compress_bytes, algorithm, suffix):
     orig_len = len(orig_bytes)
     compress_len = len(compress_bytes)
     if compress_len < orig_len * 0.9:
+        compress_improvement = (compress_len - orig_len) / orig_len
         print(
-            f"{path!s} has been shrinked by {algorithm} by {orig_len - compress_len} bytes to {int(100 * len(compress_bytes) / len(orig_bytes))}%"
+            f"{path!s}: {algorithm} compressed {orig_len} to {compress_len} bytes ({int(100 * compress_improvement)}%)"
         )
         Path(str(path) + suffix).write_bytes(compress_bytes)
     else:
-        print(f"{path!s} has been skipped because of missing gains")
+        print(f"{path!s}: {algorithm} didn't produce useful compression results")
 
 
 def try_gzip(path, orig_bytes):
     with io.BytesIO() as f:
         with gzip.GzipFile(
             filename="", mode="wb", fileobj=f, compresslevel=9, mtime=0
         ) as compress_file:
@@ -83,40 +83,35 @@
         orig_bytes,
         brotli.compress(orig_bytes),
         "Brotli",
         ".br",
     )
 
 
-def compress(root):
-    workers = os.cpu_count()
-    paths = [[] for _ in range(workers)]
-    paths_ = cycle(paths)
+def _compress_path(path):
+    orig_bytes = path.read_bytes()
+    try_brotli(path, orig_bytes)
+    try_gzip(path, orig_bytes)
+
 
+def _paths(root):
     for dir_, _dirs, files in os.walk(root):
         dir = Path(dir_)
         for filename in files:
             path = dir / filename
             if path.suffix not in SKIP_COMPRESS_EXTENSIONS:
-                next(paths_).append(path)
+                yield path
 
-    with ThreadPoolExecutor(max_workers=workers) as executor:
-        futures = [executor.submit(_compress_paths, p) for p in paths]
-        wait(futures)
 
+def compress(root):
+    with ThreadPoolExecutor() as executor:
+        executor.map(_compress_path, _paths(root))
     return 0
 
 
-def _compress_paths(paths):
-    for path in paths:
-        orig_bytes = path.read_bytes()
-        try_brotli(path, orig_bytes)
-        try_gzip(path, orig_bytes)
-
-
 def parse_args(args=None):
     parser = argparse.ArgumentParser()
     parser.add_argument("root", help="Path containing static files to compress")
     return parser.parse_args(args)
 
 
 if __name__ == "__main__":
```

### Comparing `blacknoise-0.0.6/tests/test_blacknoise.py` & `blacknoise-1.0.0/tests/test_blacknoise.py`

 * *Files identical despite different names*

### Comparing `blacknoise-0.0.6/LICENSE.txt` & `blacknoise-1.0.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `blacknoise-0.0.6/README.md` & `blacknoise-1.0.0/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -4,21 +4,16 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/blacknoise.svg)](https://pypi.org/project/blacknoise)
 
 blacknoise is an [ASGI](https://asgi.readthedocs.io/en/latest/) app for static
 file serving inspired by [whitenoise](https://github.com/evansd/whitenoise/)
 and following the principles of [low maintenance
 software](https://406.ch/writing/low-maintenance-software/).
 
-**This is pre-alpha software and everything is subject to change. I'm not even
-sure if blacknoise should exist at all or if the energy wouldn't be better
-spent improving whitenoise or other tools. Feedback and contributions are very
-welcome though!**
 
-
-## Using blacknoise with Django to serve static files
+## Using blacknoise to serve static files
 
 Install blacknoise into your Python environment:
 
 ```console
 pip install blacknoise
 ```
 
@@ -31,37 +26,48 @@
 
 BASE_DIR = Path(__file__).parent
 
 application = BlackNoise(get_asgi_application())
 application.add(BASE_DIR / "static", "/static")
 ```
 
+The example uses Django, but you can wrap any ASGI application.
+
 `BlackNoise` will automatically handle all paths below the prefixes added, and
 either return the files or return 404 errors if files do not exist. The files
 are added on server startup, which also means that `BlackNoise` only knows
 about files which existed at that particular point in time.
 
+`BlackNoise` doesn't watch the added folders for changes; if you add new files
+you have to restart the server, otherwise those files aren't served. It doesn't
+cache file contents though, so changes to files are directly picked up.
+
 ## Improving performance
 
 `BlackNoise` has worse performance than when using an optimized webserver such
 as nginx and others. Sometimes it doesn't matter much if the app is behind a
 caching reverse proxy or behind a content delivery network anyway. To further
 support this use case `BlackNoise` can be configured to serve media files with
 far-future expiry headers and has support for serving compressed assets.
 
+### Serving pre-compressed assets
+
 Compressing is possible by running:
 
 ```console
 python -m blacknoise.compress static/
 ```
 
 `BlackNoise` will try compress non-binary files using gzip or brotli (if the
 [Brotli](ttps://pypi.org/project/Brotli/) library is available), and will serve
 the compressed version if the compression actually results in (significantly)
-smaller files and if the client also supports it.
+smaller files and if the client also supports it. Files are compressed in
+parallel for faster completion times.
+
+### Setting far-future expiry headers
 
 Far-future expiry headers can be enabled by passing the `immutable_file_test`
 callable to the `BlackNoise` constructor:
 
 ```python
 def immutable_file_test(path):
     return True  # Enable far-future expiry headers for all files
@@ -75,8 +81,9 @@
 Maybe you want to add some other logic, for example check if the path contains
 a hash based upon the contents of the static file. Such hashes can be added by
 Django's `ManifestStaticFilesStorage` or by appropriately configuring bundlers
 such as `webpack` and others.
 
 ## License
 
-`blacknoise` is distributed under the terms of the [MIT](https://spdx.org/licenses/MIT.html) license.
+`blacknoise` is distributed under the terms of the
+[MIT](https://spdx.org/licenses/MIT.html) license.
```

### Comparing `blacknoise-0.0.6/pyproject.toml` & `blacknoise-1.0.0/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 [project]
 name = "blacknoise"
 description = ""
 readme = "README.md"
 keywords = [
 ]
-license = {text="MIT"}
+license = { text = "MIT" }
 authors = [
   { name = "Matthias Kestenholz", email = "mk@feinheit.ch" },
 ]
 requires-python = ">=3.9"
 classifiers = [
   "Development Status :: 4 - Beta",
   "Programming Language :: Python",
@@ -28,18 +28,17 @@
 ]
 dynamic = [
   "version",
 ]
 dependencies = [
   "starlette",
 ]
-[project.urls]
-Documentation = "https://github.com/matthiask/blacknoise#readme"
-Issues = "https://github.com/matthiask/blacknoise/issues"
-Source = "https://github.com/matthiask/blacknoise"
+urls.Documentation = "https://github.com/matthiask/blacknoise#readme"
+urls.Issues = "https://github.com/matthiask/blacknoise/issues"
+urls.Source = "https://github.com/matthiask/blacknoise"
 
 [tool.hatch.version]
 path = "src/blacknoise/__about__.py"
 
 [tool.hatch.envs.default]
 dependencies = [
   "brotli",
@@ -58,22 +57,26 @@
 ]
 cov = [
   "test-cov",
   "cov-report",
 ]
 
 [[tool.hatch.envs.all.matrix]]
-python = ["3.9", "3.10", "3.11", "3.12"]
+python = [
+  "3.9",
+  "3.10",
+  "3.11",
+  "3.12",
+]
 
 [tool.ruff]
-fix = true
 target-version = "py39"
 
-[tool.ruff.lint]
-select = [
+fix = true
+lint.select = [
   "ARG",
   "B",
   "C",
   "DTZ",
   "E",
   "EM",
   "F",
@@ -91,52 +94,67 @@
   "S",
   # "T",
   "TID",
   "UP",
   "W",
   "YTT",
 ]
-ignore = [
-  # Stop warning about line lengths
-  "E501",
+lint.per-file-ignores."tests/**/*" = [
+  "PLR2004",
+  "S101",
+  "TID252",
+]
+lint.unfixable = [
+  # Don't touch unused imports
+  "F401",
+]
+lint.flake8-tidy-imports.ban-relative-imports = "all"
+# Tests can use magic values, assertions, and relative imports
+lint.isort.known-first-party = [
+  "blacknoise",
+]
+lint.ignore = [
   # Allow non-abstract empty methods in abstract base classes
   "B027",
+  # Ignore complexity
+  "C901",
+  # Stop warning about line lengths
+  "E501",
   # Allow boolean positional values in function calls, like `dict.get(... True)`
   "FBT003",
+  "PLR0911",
+  "PLR0912",
+  "PLR0913",
+  "PLR0915",
   # Ignore checks for possible passwords
-  "S105", "S106", "S107",
-  # Ignore complexity
-  "C901", "PLR0911", "PLR0912", "PLR0913", "PLR0915",
-]
-unfixable = [
-  # Don't touch unused imports
-  "F401",
+  "S105",
+  "S106",
+  "S107",
 ]
 
-[tool.ruff.lint.isort]
-known-first-party = ["blacknoise"]
-
-[tool.ruff.lint.flake8-tidy-imports]
-ban-relative-imports = "all"
-
-[tool.ruff.lint.per-file-ignores]
-# Tests can use magic values, assertions, and relative imports
-"tests/**/*" = ["PLR2004", "S101", "TID252"]
-
 [tool.coverage.run]
-source_pkgs = ["blacknoise", "tests"]
+source_pkgs = [
+  "blacknoise",
+  "tests",
+]
 branch = true
 parallel = true
 omit = [
   "src/blacknoise/__about__.py",
 ]
 
 [tool.coverage.paths]
-blacknoise = ["src/blacknoise", "*/blacknoise/src/blacknoise"]
-tests = ["tests", "*/blacknoise/tests"]
+blacknoise = [
+  "src/blacknoise",
+  "*/blacknoise/src/blacknoise",
+]
+tests = [
+  "tests",
+  "*/blacknoise/tests",
+]
 
 [tool.coverage.report]
 exclude_lines = [
   "no cov",
   "if __name__ == .__main__.:",
   "if TYPE_CHECKING:",
 ]
```

### Comparing `blacknoise-0.0.6/PKG-INFO` & `blacknoise-1.0.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: blacknoise
-Version: 0.0.6
+Version: 1.0.0
 Project-URL: Documentation, https://github.com/matthiask/blacknoise#readme
 Project-URL: Issues, https://github.com/matthiask/blacknoise/issues
 Project-URL: Source, https://github.com/matthiask/blacknoise
 Author-email: Matthias Kestenholz <mk@feinheit.ch>
 License: MIT
 License-File: LICENSE.txt
 Classifier: Development Status :: 4 - Beta
@@ -26,21 +26,16 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/blacknoise.svg)](https://pypi.org/project/blacknoise)
 
 blacknoise is an [ASGI](https://asgi.readthedocs.io/en/latest/) app for static
 file serving inspired by [whitenoise](https://github.com/evansd/whitenoise/)
 and following the principles of [low maintenance
 software](https://406.ch/writing/low-maintenance-software/).
 
-**This is pre-alpha software and everything is subject to change. I'm not even
-sure if blacknoise should exist at all or if the energy wouldn't be better
-spent improving whitenoise or other tools. Feedback and contributions are very
-welcome though!**
 
-
-## Using blacknoise with Django to serve static files
+## Using blacknoise to serve static files
 
 Install blacknoise into your Python environment:
 
 ```console
 pip install blacknoise
 ```
 
@@ -53,37 +48,48 @@
 
 BASE_DIR = Path(__file__).parent
 
 application = BlackNoise(get_asgi_application())
 application.add(BASE_DIR / "static", "/static")
 ```
 
+The example uses Django, but you can wrap any ASGI application.
+
 `BlackNoise` will automatically handle all paths below the prefixes added, and
 either return the files or return 404 errors if files do not exist. The files
 are added on server startup, which also means that `BlackNoise` only knows
 about files which existed at that particular point in time.
 
+`BlackNoise` doesn't watch the added folders for changes; if you add new files
+you have to restart the server, otherwise those files aren't served. It doesn't
+cache file contents though, so changes to files are directly picked up.
+
 ## Improving performance
 
 `BlackNoise` has worse performance than when using an optimized webserver such
 as nginx and others. Sometimes it doesn't matter much if the app is behind a
 caching reverse proxy or behind a content delivery network anyway. To further
 support this use case `BlackNoise` can be configured to serve media files with
 far-future expiry headers and has support for serving compressed assets.
 
+### Serving pre-compressed assets
+
 Compressing is possible by running:
 
 ```console
 python -m blacknoise.compress static/
 ```
 
 `BlackNoise` will try compress non-binary files using gzip or brotli (if the
 [Brotli](ttps://pypi.org/project/Brotli/) library is available), and will serve
 the compressed version if the compression actually results in (significantly)
-smaller files and if the client also supports it.
+smaller files and if the client also supports it. Files are compressed in
+parallel for faster completion times.
+
+### Setting far-future expiry headers
 
 Far-future expiry headers can be enabled by passing the `immutable_file_test`
 callable to the `BlackNoise` constructor:
 
 ```python
 def immutable_file_test(path):
     return True  # Enable far-future expiry headers for all files
@@ -97,8 +103,9 @@
 Maybe you want to add some other logic, for example check if the path contains
 a hash based upon the contents of the static file. Such hashes can be added by
 Django's `ManifestStaticFilesStorage` or by appropriately configuring bundlers
 such as `webpack` and others.
 
 ## License
 
-`blacknoise` is distributed under the terms of the [MIT](https://spdx.org/licenses/MIT.html) license.
+`blacknoise` is distributed under the terms of the
+[MIT](https://spdx.org/licenses/MIT.html) license.
```

