# Comparing `tmp/pymonit-1.4.0.tar.gz` & `tmp/pymonit-1.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymonit-1.4.0.tar", last modified: Sat May 18 17:28:05 2024, max compression
+gzip compressed data, was "pymonit-1.4.1.tar", last modified: Sat May 18 17:38:29 2024, max compression
```

## Comparing `pymonit-1.4.0.tar` & `pymonit-1.4.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 arktnld   (1000) arktnld   (1000)        0 2024-05-18 17:28:05.015844 pymonit-1.4.0/
--rw-r--r--   0 arktnld   (1000) arktnld   (1000)     1064 2024-04-22 01:06:10.000000 pymonit-1.4.0/LICENSE
--rw-r--r--   0 arktnld   (1000) arktnld   (1000)     2188 2024-05-18 17:28:05.015844 pymonit-1.4.0/PKG-INFO
--rw-r--r--   0 arktnld   (1000) arktnld   (1000)     1553 2024-05-18 17:12:03.000000 pymonit-1.4.0/README.md
-drwxr-xr-x   0 arktnld   (1000) arktnld   (1000)        0 2024-05-18 17:28:05.012511 pymonit-1.4.0/monit/
--rw-r--r--   0 arktnld   (1000) arktnld   (1000)        0 2024-04-22 01:06:10.000000 pymonit-1.4.0/monit/__init__.py
--rw-r--r--   0 arktnld   (1000) arktnld   (1000)      977 2024-05-18 17:24:00.000000 pymonit-1.4.0/monit/config.py
--rw-r--r--   0 arktnld   (1000) arktnld   (1000)      741 2024-05-18 17:23:53.000000 pymonit-1.4.0/monit/core.py
--rw-r--r--   0 arktnld   (1000) arktnld   (1000)     2013 2024-05-18 17:24:26.000000 pymonit-1.4.0/monit/func.py
--rw-r--r--   0 arktnld   (1000) arktnld   (1000)     1180 2024-05-18 17:24:34.000000 pymonit-1.4.0/monit/http.py
--rw-r--r--   0 arktnld   (1000) arktnld   (1000)      459 2024-05-18 17:24:45.000000 pymonit-1.4.0/monit/init.py
--rw-r--r--   0 arktnld   (1000) arktnld   (1000)      950 2024-05-18 17:25:03.000000 pymonit-1.4.0/monit/log2file.py
--rw-r--r--   0 arktnld   (1000) arktnld   (1000)     1698 2024-05-18 17:25:39.000000 pymonit-1.4.0/monit/logger.py
-drwxr-xr-x   0 arktnld   (1000) arktnld   (1000)        0 2024-05-18 17:28:05.015844 pymonit-1.4.0/pymonit.egg-info/
--rw-r--r--   0 arktnld   (1000) arktnld   (1000)     2188 2024-05-18 17:28:04.000000 pymonit-1.4.0/pymonit.egg-info/PKG-INFO
--rw-r--r--   0 arktnld   (1000) arktnld   (1000)      304 2024-05-18 17:28:04.000000 pymonit-1.4.0/pymonit.egg-info/SOURCES.txt
--rw-r--r--   0 arktnld   (1000) arktnld   (1000)        1 2024-05-18 17:28:04.000000 pymonit-1.4.0/pymonit.egg-info/dependency_links.txt
--rw-r--r--   0 arktnld   (1000) arktnld   (1000)       40 2024-05-18 17:28:04.000000 pymonit-1.4.0/pymonit.egg-info/requires.txt
--rw-r--r--   0 arktnld   (1000) arktnld   (1000)        6 2024-05-18 17:28:04.000000 pymonit-1.4.0/pymonit.egg-info/top_level.txt
--rw-r--r--   0 arktnld   (1000) arktnld   (1000)       38 2024-05-18 17:28:05.015844 pymonit-1.4.0/setup.cfg
--rw-r--r--   0 arktnld   (1000) arktnld   (1000)      865 2024-05-18 17:27:57.000000 pymonit-1.4.0/setup.py
+drwxr-xr-x   0 arktnld   (1000) arktnld   (1000)        0 2024-05-18 17:38:29.110113 pymonit-1.4.1/
+-rw-r--r--   0 arktnld   (1000) arktnld   (1000)     1064 2024-04-22 01:06:10.000000 pymonit-1.4.1/LICENSE
+-rw-r--r--   0 arktnld   (1000) arktnld   (1000)     2029 2024-05-18 17:38:29.110113 pymonit-1.4.1/PKG-INFO
+-rw-r--r--   0 arktnld   (1000) arktnld   (1000)     1394 2024-05-18 17:30:43.000000 pymonit-1.4.1/README.md
+drwxr-xr-x   0 arktnld   (1000) arktnld   (1000)        0 2024-05-18 17:38:29.106779 pymonit-1.4.1/monit/
+-rw-r--r--   0 arktnld   (1000) arktnld   (1000)        0 2024-04-22 01:06:10.000000 pymonit-1.4.1/monit/__init__.py
+-rw-r--r--   0 arktnld   (1000) arktnld   (1000)      977 2024-05-18 17:24:00.000000 pymonit-1.4.1/monit/config.py
+-rw-r--r--   0 arktnld   (1000) arktnld   (1000)      741 2024-05-18 17:23:53.000000 pymonit-1.4.1/monit/core.py
+-rw-r--r--   0 arktnld   (1000) arktnld   (1000)     2013 2024-05-18 17:24:26.000000 pymonit-1.4.1/monit/func.py
+-rw-r--r--   0 arktnld   (1000) arktnld   (1000)     1180 2024-05-18 17:24:34.000000 pymonit-1.4.1/monit/http.py
+-rw-r--r--   0 arktnld   (1000) arktnld   (1000)      453 2024-05-18 17:31:11.000000 pymonit-1.4.1/monit/init.py
+-rw-r--r--   0 arktnld   (1000) arktnld   (1000)      950 2024-05-18 17:25:03.000000 pymonit-1.4.1/monit/log2file.py
+-rw-r--r--   0 arktnld   (1000) arktnld   (1000)     1698 2024-05-18 17:25:39.000000 pymonit-1.4.1/monit/logger.py
+drwxr-xr-x   0 arktnld   (1000) arktnld   (1000)        0 2024-05-18 17:38:29.110113 pymonit-1.4.1/pymonit.egg-info/
+-rw-r--r--   0 arktnld   (1000) arktnld   (1000)     2029 2024-05-18 17:38:28.000000 pymonit-1.4.1/pymonit.egg-info/PKG-INFO
+-rw-r--r--   0 arktnld   (1000) arktnld   (1000)      304 2024-05-18 17:38:29.000000 pymonit-1.4.1/pymonit.egg-info/SOURCES.txt
+-rw-r--r--   0 arktnld   (1000) arktnld   (1000)        1 2024-05-18 17:38:28.000000 pymonit-1.4.1/pymonit.egg-info/dependency_links.txt
+-rw-r--r--   0 arktnld   (1000) arktnld   (1000)       40 2024-05-18 17:38:28.000000 pymonit-1.4.1/pymonit.egg-info/requires.txt
+-rw-r--r--   0 arktnld   (1000) arktnld   (1000)        6 2024-05-18 17:38:28.000000 pymonit-1.4.1/pymonit.egg-info/top_level.txt
+-rw-r--r--   0 arktnld   (1000) arktnld   (1000)       38 2024-05-18 17:38:29.110113 pymonit-1.4.1/setup.cfg
+-rw-r--r--   0 arktnld   (1000) arktnld   (1000)      865 2024-05-18 17:38:25.000000 pymonit-1.4.1/setup.py
```

### Comparing `pymonit-1.4.0/LICENSE` & `pymonit-1.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pymonit-1.4.0/PKG-INFO` & `pymonit-1.4.1/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymonit
-Version: 1.4.0
+Version: 1.4.1
 Summary: Programa de monitoramento de código python, desenvolvido para ser utilizado pelas funcionário da Agência de dados
 Home-page: https://github.com/arktnld/monit
 Author: arktnld
 Author-email: arktnld@gmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
@@ -25,31 +25,20 @@
 ```
 **Atualização:**
 ```bash
 pip install -U pymonit
 ```
 **Exemplo arquivo `.monit`:**
 ```bash
-# Project info
-# Informações obrigatórias
-PROJECT=sample_project
-COMPANY=acme
-DEV=coder
-
-# Database info
-# Informações obrigatórias
-DB_USER=user
-DB_PASSWORD=p@ssw0rd
-DB_HOST=localhost
-DB_DATABASE=teste
-
-# Email info
-# Deixe em branco para desativar o envio de e-mails
-EMAIL=
-EMAIL_PASSWORD=
+PROJECT='project_name'
+COMPANY='company_name'
+DEV='coder'
+LOCATION='location_name'
+HANDLER_URL='https://example.com'
+PHONE='556199999999'
 ```
 ### Exemplo de Uso:
 
 **Utilização simples**
 ```python
 import time
```

### Comparing `pymonit-1.4.0/README.md` & `pymonit-1.4.1/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -6,31 +6,20 @@
 ```
 **Atualização:**
 ```bash
 pip install -U pymonit
 ```
 **Exemplo arquivo `.monit`:**
 ```bash
-# Project info
-# Informações obrigatórias
-PROJECT=sample_project
-COMPANY=acme
-DEV=coder
-
-# Database info
-# Informações obrigatórias
-DB_USER=user
-DB_PASSWORD=p@ssw0rd
-DB_HOST=localhost
-DB_DATABASE=teste
-
-# Email info
-# Deixe em branco para desativar o envio de e-mails
-EMAIL=
-EMAIL_PASSWORD=
+PROJECT='project_name'
+COMPANY='company_name'
+DEV='coder'
+LOCATION='location_name'
+HANDLER_URL='https://example.com'
+PHONE='556199999999'
 ```
 ### Exemplo de Uso:
 
 **Utilização simples**
 ```python
 import time
```

### Comparing `pymonit-1.4.0/monit/config.py` & `pymonit-1.4.1/monit/config.py`

 * *Files identical despite different names*

### Comparing `pymonit-1.4.0/monit/core.py` & `pymonit-1.4.1/monit/core.py`

 * *Files identical despite different names*

### Comparing `pymonit-1.4.0/monit/func.py` & `pymonit-1.4.1/monit/func.py`

 * *Files identical despite different names*

### Comparing `pymonit-1.4.0/monit/http.py` & `pymonit-1.4.1/monit/http.py`

 * *Files identical despite different names*

### Comparing `pymonit-1.4.0/monit/log2file.py` & `pymonit-1.4.1/monit/log2file.py`

 * *Files identical despite different names*

### Comparing `pymonit-1.4.0/monit/logger.py` & `pymonit-1.4.1/monit/logger.py`

 * *Files identical despite different names*

### Comparing `pymonit-1.4.0/pymonit.egg-info/PKG-INFO` & `pymonit-1.4.1/pymonit.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymonit
-Version: 1.4.0
+Version: 1.4.1
 Summary: Programa de monitoramento de código python, desenvolvido para ser utilizado pelas funcionário da Agência de dados
 Home-page: https://github.com/arktnld/monit
 Author: arktnld
 Author-email: arktnld@gmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
@@ -25,31 +25,20 @@
 ```
 **Atualização:**
 ```bash
 pip install -U pymonit
 ```
 **Exemplo arquivo `.monit`:**
 ```bash
-# Project info
-# Informações obrigatórias
-PROJECT=sample_project
-COMPANY=acme
-DEV=coder
-
-# Database info
-# Informações obrigatórias
-DB_USER=user
-DB_PASSWORD=p@ssw0rd
-DB_HOST=localhost
-DB_DATABASE=teste
-
-# Email info
-# Deixe em branco para desativar o envio de e-mails
-EMAIL=
-EMAIL_PASSWORD=
+PROJECT='project_name'
+COMPANY='company_name'
+DEV='coder'
+LOCATION='location_name'
+HANDLER_URL='https://example.com'
+PHONE='556199999999'
 ```
 ### Exemplo de Uso:
 
 **Utilização simples**
 ```python
 import time
```

### Comparing `pymonit-1.4.0/setup.py` & `pymonit-1.4.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 import pathlib
 
 setup(
     name='pymonit',
-    version='1.4.0',
+    version='1.4.1',
     description='Programa de monitoramento de código python, desenvolvido para ser utilizado pelas funcionário da Agência de dados',
     long_description=pathlib.Path('README.md').read_text(),
     long_description_content_type='text/markdown',
     author='arktnld',
     author_email='arktnld@gmail.com',
     url='https://github.com/arktnld/monit',
     license='MIT',
```

