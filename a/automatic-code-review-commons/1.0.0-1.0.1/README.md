# Comparing `tmp/automatic-code-review-commons-1.0.0.tar.gz` & `tmp/automatic-code-review-commons-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "automatic-code-review-commons-1.0.0.tar", last modified: Sat May 18 15:08:11 2024, max compression
+gzip compressed data, was "automatic-code-review-commons-1.0.1.tar", last modified: Sat May 18 15:43:13 2024, max compression
```

## Comparing `automatic-code-review-commons-1.0.0.tar` & `automatic-code-review-commons-1.0.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 kielsondasilva  (1001) kielsonzinn  (1001)        0 2024-05-18 15:08:11.702733 automatic-code-review-commons-1.0.0/
--rw-r--r--   0 kielsondasilva  (1001) kielsonzinn  (1001)      774 2024-05-18 15:08:11.702733 automatic-code-review-commons-1.0.0/PKG-INFO
--rw-r--r--   0 kielsondasilva  (1001) kielsonzinn  (1001)      197 2024-05-18 14:55:00.000000 automatic-code-review-commons-1.0.0/README.md
-drwxr-xr-x   0 kielsondasilva  (1001) kielsonzinn  (1001)        0 2024-05-18 15:08:11.698733 automatic-code-review-commons-1.0.0/automatic_code_review_commons/
--rw-r--r--   0 kielsondasilva  (1001) kielsonzinn  (1001)       33 2024-05-18 14:52:25.000000 automatic-code-review-commons-1.0.0/automatic_code_review_commons/__init__.py
--rw-r--r--   0 kielsondasilva  (1001) kielsonzinn  (1001)      149 2024-05-18 14:56:29.000000 automatic-code-review-commons-1.0.0/automatic_code_review_commons/commons.py
-drwxr-xr-x   0 kielsondasilva  (1001) kielsonzinn  (1001)        0 2024-05-18 15:08:11.702733 automatic-code-review-commons-1.0.0/automatic_code_review_commons.egg-info/
--rw-r--r--   0 kielsondasilva  (1001) kielsonzinn  (1001)      774 2024-05-18 15:08:11.000000 automatic-code-review-commons-1.0.0/automatic_code_review_commons.egg-info/PKG-INFO
--rw-r--r--   0 kielsondasilva  (1001) kielsonzinn  (1001)      313 2024-05-18 15:08:11.000000 automatic-code-review-commons-1.0.0/automatic_code_review_commons.egg-info/SOURCES.txt
--rw-r--r--   0 kielsondasilva  (1001) kielsonzinn  (1001)        1 2024-05-18 15:08:11.000000 automatic-code-review-commons-1.0.0/automatic_code_review_commons.egg-info/dependency_links.txt
--rw-r--r--   0 kielsondasilva  (1001) kielsonzinn  (1001)       30 2024-05-18 15:08:11.000000 automatic-code-review-commons-1.0.0/automatic_code_review_commons.egg-info/top_level.txt
--rw-r--r--   0 kielsondasilva  (1001) kielsonzinn  (1001)       38 2024-05-18 15:08:11.702733 automatic-code-review-commons-1.0.0/setup.cfg
--rw-r--r--   0 kielsondasilva  (1001) kielsonzinn  (1001)      721 2024-05-18 15:02:42.000000 automatic-code-review-commons-1.0.0/setup.py
+drwxr-xr-x   0 kielsondasilva  (1001) kielsonzinn  (1001)        0 2024-05-18 15:43:13.580460 automatic-code-review-commons-1.0.1/
+-rw-r--r--   0 kielsondasilva  (1001) kielsonzinn  (1001)     1082 2024-05-18 15:43:13.580460 automatic-code-review-commons-1.0.1/PKG-INFO
+-rw-r--r--   0 kielsondasilva  (1001) kielsonzinn  (1001)      505 2024-05-18 15:42:53.000000 automatic-code-review-commons-1.0.1/README.md
+drwxr-xr-x   0 kielsondasilva  (1001) kielsonzinn  (1001)        0 2024-05-18 15:43:13.580460 automatic-code-review-commons-1.0.1/automatic_code_review_commons/
+-rw-r--r--   0 kielsondasilva  (1001) kielsonzinn  (1001)       33 2024-05-18 14:52:25.000000 automatic-code-review-commons-1.0.1/automatic_code_review_commons/__init__.py
+-rw-r--r--   0 kielsondasilva  (1001) kielsonzinn  (1001)      741 2024-05-18 15:34:38.000000 automatic-code-review-commons-1.0.1/automatic_code_review_commons/commons.py
+drwxr-xr-x   0 kielsondasilva  (1001) kielsonzinn  (1001)        0 2024-05-18 15:43:13.580460 automatic-code-review-commons-1.0.1/automatic_code_review_commons.egg-info/
+-rw-r--r--   0 kielsondasilva  (1001) kielsonzinn  (1001)     1082 2024-05-18 15:43:13.000000 automatic-code-review-commons-1.0.1/automatic_code_review_commons.egg-info/PKG-INFO
+-rw-r--r--   0 kielsondasilva  (1001) kielsonzinn  (1001)      313 2024-05-18 15:43:13.000000 automatic-code-review-commons-1.0.1/automatic_code_review_commons.egg-info/SOURCES.txt
+-rw-r--r--   0 kielsondasilva  (1001) kielsonzinn  (1001)        1 2024-05-18 15:43:13.000000 automatic-code-review-commons-1.0.1/automatic_code_review_commons.egg-info/dependency_links.txt
+-rw-r--r--   0 kielsondasilva  (1001) kielsonzinn  (1001)       30 2024-05-18 15:43:13.000000 automatic-code-review-commons-1.0.1/automatic_code_review_commons.egg-info/top_level.txt
+-rw-r--r--   0 kielsondasilva  (1001) kielsonzinn  (1001)       38 2024-05-18 15:43:13.580460 automatic-code-review-commons-1.0.1/setup.cfg
+-rw-r--r--   0 kielsondasilva  (1001) kielsonzinn  (1001)      721 2024-05-18 15:36:41.000000 automatic-code-review-commons-1.0.1/setup.py
```

### Comparing `automatic-code-review-commons-1.0.0/PKG-INFO` & `automatic-code-review-commons-1.0.1/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: automatic-code-review-commons
-Version: 1.0.0
+Version: 1.0.1
 Summary: Biblioteca com funções genéricas para revisões automáticas de código do projeto ACR
 Home-page: https://github.com/automatic-code-review/automatic-code-review-commons
 Author: Kielson Zinn da Silva
 Author-email: automatic.code.review@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
@@ -13,14 +13,27 @@
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 
 # automatic-code-review-commons
 
 Biblioteca com funções genéricas para revisões automáticas de código da ferramenta ACR.
 
-## Instalação
+- [DOCS](https://github.com/automatic-code-review/docs/wiki)
+- [VERSIONS](https://pypi.org/project/automatic-code-review-commons)
+
+## Install
 
 ```sh
 pip install automatic-code-review-commons
 ```
 
+## Publish
+
+```sh
+rm -rf dist
+rm -rf build
+rm -rf automatic_code_review_commons.egg-info
+pip install setuptools wheel twine
+python setup.py sdist bdist_wheel
+twine upload dist/*
+```
```

### Comparing `automatic-code-review-commons-1.0.0/automatic_code_review_commons.egg-info/PKG-INFO` & `automatic-code-review-commons-1.0.1/automatic_code_review_commons.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: automatic-code-review-commons
-Version: 1.0.0
+Version: 1.0.1
 Summary: Biblioteca com funções genéricas para revisões automáticas de código do projeto ACR
 Home-page: https://github.com/automatic-code-review/automatic-code-review-commons
 Author: Kielson Zinn da Silva
 Author-email: automatic.code.review@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
@@ -13,14 +13,27 @@
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 
 # automatic-code-review-commons
 
 Biblioteca com funções genéricas para revisões automáticas de código da ferramenta ACR.
 
-## Instalação
+- [DOCS](https://github.com/automatic-code-review/docs/wiki)
+- [VERSIONS](https://pypi.org/project/automatic-code-review-commons)
+
+## Install
 
 ```sh
 pip install automatic-code-review-commons
 ```
 
+## Publish
+
+```sh
+rm -rf dist
+rm -rf build
+rm -rf automatic_code_review_commons.egg-info
+pip install setuptools wheel twine
+python setup.py sdist bdist_wheel
+twine upload dist/*
+```
```

### Comparing `automatic-code-review-commons-1.0.0/setup.py` & `automatic-code-review-commons-1.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='automatic-code-review-commons',
-    version='1.0.0',
+    version='1.0.1',
     packages=find_packages(),
     description='Biblioteca com funções genéricas para revisões automáticas de código do projeto ACR',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author='Kielson Zinn da Silva',
     author_email='automatic.code.review@gmail.com',
     url='https://github.com/automatic-code-review/automatic-code-review-commons',
```

