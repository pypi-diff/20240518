# Comparing `tmp/xss_shield-0.1.2.tar.gz` & `tmp/xss_shield-1.0.0.tar.gz`

## Comparing `xss_shield-0.1.2.tar` & `xss_shield-1.0.0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0      936 2020-02-02 00:00:00.000000 xss_shield-0.1.2/examples/example.ipynb
--rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 xss_shield-0.1.2/src/xss_shield/__init__.py
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 xss_shield-0.1.2/.gitignore
--rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 xss_shield-0.1.2/LICENSE
--rw-r--r--   0        0        0      624 2020-02-02 00:00:00.000000 xss_shield-0.1.2/README.md
--rw-r--r--   0        0        0      601 2020-02-02 00:00:00.000000 xss_shield-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     1168 2020-02-02 00:00:00.000000 xss_shield-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0      936 2020-02-02 00:00:00.000000 xss_shield-1.0.0/examples/example.ipynb
+-rw-r--r--   0        0        0      408 2020-02-02 00:00:00.000000 xss_shield-1.0.0/src/xss_shield/__init__.py
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 xss_shield-1.0.0/.gitignore
+-rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 xss_shield-1.0.0/LICENSE
+-rw-r--r--   0        0        0      768 2020-02-02 00:00:00.000000 xss_shield-1.0.0/README.md
+-rw-r--r--   0        0        0      601 2020-02-02 00:00:00.000000 xss_shield-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0     1312 2020-02-02 00:00:00.000000 xss_shield-1.0.0/PKG-INFO
```

### Comparing `xss_shield-0.1.2/examples/example.ipynb` & `xss_shield-1.0.0/examples/example.ipynb`

 * *Files identical despite different names*

### Comparing `xss_shield-0.1.2/.gitignore` & `xss_shield-1.0.0/.gitignore`

 * *Files identical despite different names*

### Comparing `xss_shield-0.1.2/LICENSE` & `xss_shield-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `xss_shield-0.1.2/pyproject.toml` & `xss_shield-1.0.0/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "xss-shield"
-version = "0.1.2"
+version = "1.0.0"
 authors = [
   { name="Gordon Zhang", email="jp20171211@163.com" },
 ]
 description = "A library used to stop your website from being attacked."
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `xss_shield-0.1.2/PKG-INFO` & `xss_shield-1.0.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: xss-shield
-Version: 0.1.2
+Version: 1.0.0
 Summary: A library used to stop your website from being attacked.
 Project-URL: Homepage, https://github.com/GordonZhang2024/xss-shield/
 Project-URL: Issues, https://github.com/GordonZhang2024/xss-shield/issues
 Author-email: Gordon Zhang <jp20171211@163.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -25,14 +25,23 @@
 ## Installing
 Type command:
 ```bash
 $ pip install xss-shield
 ```
 
 ## Usage
+Function `excape(s: str, strict=True)`
+> ## Arguments
+> s: the string to parse
+>
+> strict: if strict = False -> only replace `<script>` tag
+
+
 example:
 ```python
 import xss_shield
 
 unsafe_str = '<script>alert("Bad.");</script>'
 safe_str = xss_shield.escape(unsafe_str)
 ```
+
+
```

#### html2text {}

```diff
@@ -1,16 +1,17 @@
-Metadata-Version: 2.3 Name: xss-shield Version: 0.1.2 Summary: A library used
+Metadata-Version: 2.3 Name: xss-shield Version: 1.0.0 Summary: A library used
 to stop your website from being attacked. Project-URL: Homepage, https://
 github.com/GordonZhang2024/xss-shield/ Project-URL: Issues, https://github.com/
 GordonZhang2024/xss-shield/issues Author-email: Gordon Zhang
 163.com> License-File: LICENSE Classifier: License :: OSI Approved :: MIT
 License Classifier: Operating System :: OS Independent Classifier: Programming
 Language :: Python :: 3 Requires-Python: >=3.8 Description-Content-Type: text/
 markdown # xss-shield A Python library to prevent your website from being
 attacked. [PyPI](https://pypi.org/project/xss-shield/) ![PyPI - Downloads]
 (https://img.shields.io/pypi/dw/xss-shield) ![PyPI - Python Version](https://
 img.shields.io/pypi/pyversions/xss-shield) ![PyPI - Wheel](https://
 img.shields.io/pypi/wheel/xss-shield) ![GitHub top language](https://
 img.shields.io/github/languages/top/GordonZhang2024/xss-shield) ## Installing
-Type command: ```bash $ pip install xss-shield ``` ## Usage example: ```python
-import xss_shield unsafe_str = '
+Type command: ```bash $ pip install xss-shield ``` ## Usage Function `excape(s:
+str, strict=True)` > ## Arguments > s: the string to parse > > strict: if
+strict = False -> only replace `
 ' safe_str = xss_shield.escape(unsafe_str) ```
```

