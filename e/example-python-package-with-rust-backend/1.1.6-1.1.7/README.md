# Comparing `tmp/example_python_package_with_rust_backend-1.1.6.tar.gz` & `tmp/example_python_package_with_rust_backend-1.1.7.tar.gz`

## Comparing `example_python_package_with_rust_backend-1.1.6.tar` & `example_python_package_with_rust_backend-1.1.7.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0      379 1970-01-01 00:00:00.000000 example_python_package_with_rust_backend-1.1.6/Cargo.toml
--rw-r--r--   0      501       20     3796 2024-05-17 21:43:36.000000 example_python_package_with_rust_backend-1.1.6/.github/workflows/python-publish.yml
--rw-r--r--   0      501       20     1073 2024-05-17 21:43:36.000000 example_python_package_with_rust_backend-1.1.6/LICENSE.txt
--rw-r--r--   0      501       20      999 2024-05-17 21:43:36.000000 example_python_package_with_rust_backend-1.1.6/README.md
--rw-r--r--   0      501       20      115 2024-05-17 21:43:36.000000 example_python_package_with_rust_backend-1.1.6/examples/usage.py
--rw-r--r--   0      501       20      759 2024-05-17 21:43:36.000000 example_python_package_with_rust_backend-1.1.6/src/lib.rs
--rw-r--r--   0      501       20     7686 2024-05-17 21:43:36.000000 example_python_package_with_rust_backend-1.1.6/Cargo.lock
--rw-r--r--   0      501       20      417 2024-05-17 21:43:36.000000 example_python_package_with_rust_backend-1.1.6/pyproject.toml
--rw-r--r--   0        0        0     1384 1970-01-01 00:00:00.000000 example_python_package_with_rust_backend-1.1.6/PKG-INFO
+-rw-r--r--   0        0        0      379 1970-01-01 00:00:00.000000 example_python_package_with_rust_backend-1.1.7/Cargo.toml
+-rw-r--r--   0      501       20     3745 2024-05-17 21:51:17.000000 example_python_package_with_rust_backend-1.1.7/.github/workflows/python-publish.yml
+-rw-r--r--   0      501       20     1073 2024-05-17 21:51:17.000000 example_python_package_with_rust_backend-1.1.7/LICENSE.txt
+-rw-r--r--   0      501       20      999 2024-05-17 21:51:17.000000 example_python_package_with_rust_backend-1.1.7/README.md
+-rw-r--r--   0      501       20      115 2024-05-17 21:51:17.000000 example_python_package_with_rust_backend-1.1.7/examples/usage.py
+-rw-r--r--   0      501       20      759 2024-05-17 21:51:17.000000 example_python_package_with_rust_backend-1.1.7/src/lib.rs
+-rw-r--r--   0      501       20     7686 2024-05-17 21:51:17.000000 example_python_package_with_rust_backend-1.1.7/Cargo.lock
+-rw-r--r--   0      501       20      417 2024-05-17 21:51:17.000000 example_python_package_with_rust_backend-1.1.7/pyproject.toml
+-rw-r--r--   0        0        0     1384 1970-01-01 00:00:00.000000 example_python_package_with_rust_backend-1.1.7/PKG-INFO
```

### Comparing `example_python_package_with_rust_backend-1.1.6/.github/workflows/python-publish.yml` & `example_python_package_with_rust_backend-1.1.7/.github/workflows/python-publish.yml`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,13 @@
 # there are different ways of making a pypi package with rust
 # https://github.com/PyO3/maturin-action has examples
 name: Build and upload to PyPI
 
 on:
   workflow_dispatch:
-  pull_request:
-  push:
-    branches:
-      - main
   release:
     types:
       - published
 
 jobs:
   macos:
     # erros on Library not loaded: /usr/local/opt/gettext/lib/libintl.8.dylib
```

### Comparing `example_python_package_with_rust_backend-1.1.6/LICENSE.txt` & `example_python_package_with_rust_backend-1.1.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `example_python_package_with_rust_backend-1.1.6/README.md` & `example_python_package_with_rust_backend-1.1.7/README.md`

 * *Files identical despite different names*

### Comparing `example_python_package_with_rust_backend-1.1.6/src/lib.rs` & `example_python_package_with_rust_backend-1.1.7/src/lib.rs`

 * *Files identical despite different names*

### Comparing `example_python_package_with_rust_backend-1.1.6/Cargo.lock` & `example_python_package_with_rust_backend-1.1.7/Cargo.lock`

 * *Files identical despite different names*

### Comparing `example_python_package_with_rust_backend-1.1.6/PKG-INFO` & `example_python_package_with_rust_backend-1.1.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: example_python_package_with_rust_backend
-Version: 1.1.6
+Version: 1.1.7
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 License-File: LICENSE.txt
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
```

