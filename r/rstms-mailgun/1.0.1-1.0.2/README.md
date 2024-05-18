# Comparing `tmp/rstms_mailgun-1.0.1.tar.gz` & `tmp/rstms_mailgun-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rstms_mailgun-1.0.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "rstms_mailgun-1.0.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `rstms_mailgun-1.0.1.tar` & `rstms_mailgun-1.0.2.tar`

### file list

```diff
@@ -1,40 +1,40 @@
--rw-r--r--   0        0        0      380 2024-04-27 07:20:32.114641 rstms_mailgun-1.0.1/.bumpversion.cfg
--rw-r--r--   0        0        0     1338 2024-04-27 02:57:20.583637 rstms_mailgun-1.0.1/.gitignore
--rw-r--r--   0        0        0     1071 2024-04-27 02:57:20.579637 rstms_mailgun-1.0.1/LICENSE
--rw-r--r--   0        0        0      539 2024-04-27 02:57:20.579637 rstms_mailgun-1.0.1/Makefile
--rw-r--r--   0        0        0      660 2024-04-27 02:57:20.595637 rstms_mailgun-1.0.1/README.md
--rw-r--r--   0        0        0        6 2024-04-27 07:20:32.114641 rstms_mailgun-1.0.1/VERSION
--rw-r--r--   0        0        0      614 2024-04-27 02:57:20.663637 rstms_mailgun-1.0.1/docs/Makefile
--rw-r--r--   0        0        0       91 2024-04-27 02:57:20.675636 rstms_mailgun-1.0.1/docs/cli.rst
--rwxr-xr-x   0        0        0     4921 2024-04-27 02:57:20.675636 rstms_mailgun-1.0.1/docs/conf.py
--rw-r--r--   0        0        0       33 2024-04-27 02:57:20.675636 rstms_mailgun-1.0.1/docs/contributing.rst
--rw-r--r--   0        0        0      297 2024-04-27 02:57:20.659637 rstms_mailgun-1.0.1/docs/index.rst
--rw-r--r--   0        0        0     1150 2024-04-27 02:57:20.667636 rstms_mailgun-1.0.1/docs/installation.rst
--rw-r--r--   0        0        0      775 2024-04-27 02:57:20.659637 rstms_mailgun-1.0.1/docs/make.bat
--rw-r--r--   0        0        0       27 2024-04-27 02:57:20.655637 rstms_mailgun-1.0.1/docs/readme.rst
--rw-r--r--   0        0        0      431 2024-04-27 02:57:20.615637 rstms_mailgun-1.0.1/make/browser.mk
--rw-r--r--   0        0        0      694 2024-04-27 02:57:20.627637 rstms_mailgun-1.0.1/make/clean.mk
--rw-r--r--   0        0        0     3808 2024-04-27 02:57:20.623637 rstms_mailgun-1.0.1/make/common.mk
--rw-r--r--   0        0        0      477 2024-04-27 02:57:20.619637 rstms_mailgun-1.0.1/make/depends.mk
--rw-r--r--   0        0        0      441 2024-04-27 02:57:20.611637 rstms_mailgun-1.0.1/make/dist.mk
--rw-r--r--   0        0        0      719 2024-04-27 02:57:20.603637 rstms_mailgun-1.0.1/make/docs.mk
--rw-r--r--   0        0        0      610 2024-04-27 02:57:20.599637 rstms_mailgun-1.0.1/make/lint.mk
--rw-r--r--   0        0        0     1214 2024-04-27 02:57:20.607637 rstms_mailgun-1.0.1/make/publish.mk
--rw-r--r--   0        0        0      517 2024-04-27 02:57:20.611637 rstms_mailgun-1.0.1/make/release.mk
--rw-r--r--   0        0        0      502 2024-04-27 02:57:20.607637 rstms_mailgun-1.0.1/make/requirements.mk
--rw-r--r--   0        0        0      947 2024-04-27 02:57:20.603637 rstms_mailgun-1.0.1/make/test.mk
--rw-r--r--   0        0        0     1610 2024-04-27 02:57:20.615637 rstms_mailgun-1.0.1/make/version.mk
--rw-r--r--   0        0        0     1137 2024-04-27 07:20:32.114641 rstms_mailgun-1.0.1/pyproject.toml
--rw-r--r--   0        0        0      231 2024-04-27 02:57:20.547638 rstms_mailgun-1.0.1/pytest.ini
--rw-r--r--   0        0        0       97 2024-04-27 07:20:31.858644 rstms_mailgun-1.0.1/requirements-dev.txt
--rw-r--r--   0        0        0       47 2024-04-27 07:20:31.958643 rstms_mailgun-1.0.1/requirements-docs.txt
--rw-r--r--   0        0        0       15 2024-04-27 07:20:31.774645 rstms_mailgun-1.0.1/requirements.txt
--rw-r--r--   0        0        0      214 2024-04-27 03:15:02.887230 rstms_mailgun-1.0.1/rstms_mailgun/__init__.py
--rw-r--r--   0        0        0     8707 2024-04-27 07:16:28.097282 rstms_mailgun-1.0.1/rstms_mailgun/cli.py
--rw-r--r--   0        0        0     1067 2024-04-27 02:57:20.651637 rstms_mailgun-1.0.1/rstms_mailgun/exception_handler.py
--rw-r--r--   0        0        0     1092 2024-04-27 03:15:02.915229 rstms_mailgun-1.0.1/rstms_mailgun/shell.py
--rw-r--r--   0        0        0      127 2024-04-27 07:20:32.114641 rstms_mailgun-1.0.1/rstms_mailgun/version.py
--rw-r--r--   0        0        0       43 2024-04-27 02:57:20.631637 rstms_mailgun-1.0.1/tests/__init__.py
--rw-r--r--   0        0        0     2255 2024-04-27 03:15:02.935229 rstms_mailgun-1.0.1/tests/test_cli.py
--rw-r--r--   0        0        0      429 2024-04-27 02:57:20.551638 rstms_mailgun-1.0.1/tox.ini
--rw-r--r--   0        0        0     1864 1970-01-01 00:00:00.000000 rstms_mailgun-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0      380 2024-05-18 17:01:57.987206 rstms_mailgun-1.0.2/.bumpversion.cfg
+-rw-r--r--   0        0        0     1344 2024-05-18 17:01:39.323410 rstms_mailgun-1.0.2/.gitignore
+-rw-r--r--   0        0        0     1071 2024-04-27 02:57:20.579637 rstms_mailgun-1.0.2/LICENSE
+-rw-r--r--   0        0        0      539 2024-04-27 02:57:20.579637 rstms_mailgun-1.0.2/Makefile
+-rw-r--r--   0        0        0      660 2024-04-27 02:57:20.595637 rstms_mailgun-1.0.2/README.md
+-rw-r--r--   0        0        0        6 2024-05-18 17:01:57.987206 rstms_mailgun-1.0.2/VERSION
+-rw-r--r--   0        0        0      614 2024-04-27 02:57:20.663637 rstms_mailgun-1.0.2/docs/Makefile
+-rw-r--r--   0        0        0       91 2024-04-27 02:57:20.675636 rstms_mailgun-1.0.2/docs/cli.rst
+-rwxr-xr-x   0        0        0     4921 2024-04-27 02:57:20.675636 rstms_mailgun-1.0.2/docs/conf.py
+-rw-r--r--   0        0        0       33 2024-04-27 02:57:20.675636 rstms_mailgun-1.0.2/docs/contributing.rst
+-rw-r--r--   0        0        0      297 2024-04-27 02:57:20.659637 rstms_mailgun-1.0.2/docs/index.rst
+-rw-r--r--   0        0        0     1150 2024-04-27 02:57:20.667636 rstms_mailgun-1.0.2/docs/installation.rst
+-rw-r--r--   0        0        0      775 2024-04-27 02:57:20.659637 rstms_mailgun-1.0.2/docs/make.bat
+-rw-r--r--   0        0        0       27 2024-04-27 02:57:20.655637 rstms_mailgun-1.0.2/docs/readme.rst
+-rw-r--r--   0        0        0      431 2024-04-27 02:57:20.615637 rstms_mailgun-1.0.2/make/browser.mk
+-rw-r--r--   0        0        0      694 2024-04-27 02:57:20.627637 rstms_mailgun-1.0.2/make/clean.mk
+-rw-r--r--   0        0        0     3808 2024-04-27 02:57:20.623637 rstms_mailgun-1.0.2/make/common.mk
+-rw-r--r--   0        0        0      477 2024-04-27 02:57:20.619637 rstms_mailgun-1.0.2/make/depends.mk
+-rw-r--r--   0        0        0      441 2024-04-27 02:57:20.611637 rstms_mailgun-1.0.2/make/dist.mk
+-rw-r--r--   0        0        0      719 2024-04-27 02:57:20.603637 rstms_mailgun-1.0.2/make/docs.mk
+-rw-r--r--   0        0        0      610 2024-04-27 02:57:20.599637 rstms_mailgun-1.0.2/make/lint.mk
+-rw-r--r--   0        0        0     1214 2024-04-27 02:57:20.607637 rstms_mailgun-1.0.2/make/publish.mk
+-rw-r--r--   0        0        0      517 2024-04-27 02:57:20.611637 rstms_mailgun-1.0.2/make/release.mk
+-rw-r--r--   0        0        0      502 2024-04-27 02:57:20.607637 rstms_mailgun-1.0.2/make/requirements.mk
+-rw-r--r--   0        0        0      947 2024-04-27 02:57:20.603637 rstms_mailgun-1.0.2/make/test.mk
+-rw-r--r--   0        0        0     1610 2024-04-27 02:57:20.615637 rstms_mailgun-1.0.2/make/version.mk
+-rw-r--r--   0        0        0     1137 2024-05-18 17:01:57.987206 rstms_mailgun-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0      231 2024-04-27 02:57:20.547638 rstms_mailgun-1.0.2/pytest.ini
+-rw-r--r--   0        0        0       97 2024-05-18 17:01:57.831207 rstms_mailgun-1.0.2/requirements-dev.txt
+-rw-r--r--   0        0        0       47 2024-05-18 17:01:57.883207 rstms_mailgun-1.0.2/requirements-docs.txt
+-rw-r--r--   0        0        0       15 2024-05-18 17:01:57.775208 rstms_mailgun-1.0.2/requirements.txt
+-rw-r--r--   0        0        0      214 2024-04-27 03:15:02.887230 rstms_mailgun-1.0.2/rstms_mailgun/__init__.py
+-rw-r--r--   0        0        0    16057 2024-05-18 16:51:44.889906 rstms_mailgun-1.0.2/rstms_mailgun/cli.py
+-rw-r--r--   0        0        0     1067 2024-04-27 02:57:20.651637 rstms_mailgun-1.0.2/rstms_mailgun/exception_handler.py
+-rw-r--r--   0        0        0     1092 2024-04-27 03:15:02.915229 rstms_mailgun-1.0.2/rstms_mailgun/shell.py
+-rw-r--r--   0        0        0      127 2024-05-18 17:01:57.987206 rstms_mailgun-1.0.2/rstms_mailgun/version.py
+-rw-r--r--   0        0        0       43 2024-04-27 02:57:20.631637 rstms_mailgun-1.0.2/tests/__init__.py
+-rw-r--r--   0        0        0     2255 2024-04-27 03:15:02.935229 rstms_mailgun-1.0.2/tests/test_cli.py
+-rw-r--r--   0        0        0      429 2024-04-27 02:57:20.551638 rstms_mailgun-1.0.2/tox.ini
+-rw-r--r--   0        0        0     1864 1970-01-01 00:00:00.000000 rstms_mailgun-1.0.2/PKG-INFO
```

### Comparing `rstms_mailgun-1.0.1/.gitignore` & `rstms_mailgun-1.0.2/.gitignore`

 * *Files 1% similar despite different names*

```diff
@@ -115,7 +115,8 @@
 .black
 .errors
 .flake8
 docker/VERSION
 docker/.build
 docker/*.whl
 postactivate
+notes
```

### Comparing `rstms_mailgun-1.0.1/LICENSE` & `rstms_mailgun-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `rstms_mailgun-1.0.1/Makefile` & `rstms_mailgun-1.0.2/Makefile`

 * *Files identical despite different names*

### Comparing `rstms_mailgun-1.0.1/README.md` & `rstms_mailgun-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `rstms_mailgun-1.0.1/docs/Makefile` & `rstms_mailgun-1.0.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `rstms_mailgun-1.0.1/docs/conf.py` & `rstms_mailgun-1.0.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `rstms_mailgun-1.0.1/docs/installation.rst` & `rstms_mailgun-1.0.2/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `rstms_mailgun-1.0.1/docs/make.bat` & `rstms_mailgun-1.0.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `rstms_mailgun-1.0.1/make/clean.mk` & `rstms_mailgun-1.0.2/make/clean.mk`

 * *Files identical despite different names*

### Comparing `rstms_mailgun-1.0.1/make/common.mk` & `rstms_mailgun-1.0.2/make/common.mk`

 * *Files identical despite different names*

### Comparing `rstms_mailgun-1.0.1/make/docs.mk` & `rstms_mailgun-1.0.2/make/docs.mk`

 * *Files identical despite different names*

### Comparing `rstms_mailgun-1.0.1/make/lint.mk` & `rstms_mailgun-1.0.2/make/lint.mk`

 * *Files identical despite different names*

### Comparing `rstms_mailgun-1.0.1/make/publish.mk` & `rstms_mailgun-1.0.2/make/publish.mk`

 * *Files identical despite different names*

### Comparing `rstms_mailgun-1.0.1/make/release.mk` & `rstms_mailgun-1.0.2/make/release.mk`

 * *Files identical despite different names*

### Comparing `rstms_mailgun-1.0.1/make/test.mk` & `rstms_mailgun-1.0.2/make/test.mk`

 * *Files identical despite different names*

### Comparing `rstms_mailgun-1.0.1/make/version.mk` & `rstms_mailgun-1.0.2/make/version.mk`

 * *Files identical despite different names*

### Comparing `rstms_mailgun-1.0.1/pyproject.toml` & `rstms_mailgun-1.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "flit_core.buildapi"
 requires_python = ">=3.10"
 
 
 
 [project]
 name = "rstms-mailgun"
-version = "1.0.1"
+version = "1.0.2"
 authors = [{name = "Matt Krueger", email = "mkrueger@rstms.net"}]
 readme = {file = "README.md", content-type = "text/markdown"}
 license = {file = "LICENSE"}
 keywords = ["rstms_mailgun"]
 classifiers = [
   "Intended Audience :: Developers",
```

### Comparing `rstms_mailgun-1.0.1/rstms_mailgun/exception_handler.py` & `rstms_mailgun-1.0.2/rstms_mailgun/exception_handler.py`

 * *Files identical despite different names*

### Comparing `rstms_mailgun-1.0.1/rstms_mailgun/shell.py` & `rstms_mailgun-1.0.2/rstms_mailgun/shell.py`

 * *Files identical despite different names*

### Comparing `rstms_mailgun-1.0.1/tests/test_cli.py` & `rstms_mailgun-1.0.2/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `rstms_mailgun-1.0.1/PKG-INFO` & `rstms_mailgun-1.0.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rstms-mailgun
-Version: 1.0.1
+Version: 1.0.2
 Summary: Top-level package for rstms-mailgun.
 Keywords: rstms_mailgun
 Author-email: Matt Krueger <mkrueger@rstms.net>
 Description-Content-Type: text/markdown
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
```

