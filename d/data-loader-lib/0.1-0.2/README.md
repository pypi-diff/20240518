# Comparing `tmp/data_loader_lib-0.1.tar.gz` & `tmp/data_loader_lib-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "data_loader_lib-0.1.tar", last modified: Fri May 17 18:18:25 2024, max compression
+gzip compressed data, was "data_loader_lib-0.2.tar", last modified: Sat May 18 16:30:17 2024, max compression
```

## Comparing `data_loader_lib-0.1.tar` & `data_loader_lib-0.2.tar`

### file list

```diff
@@ -1,11 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-05-17 18:18:25.251850 data_loader_lib-0.1/
--rw-rw-rw-   0        0        0      552 2024-05-17 18:18:25.249837 data_loader_lib-0.1/PKG-INFO
--rw-rw-rw-   0        0        0       42 2024-05-17 18:18:25.252839 data_loader_lib-0.1/setup.cfg
--rw-rw-rw-   0        0        0      746 2024-05-17 18:07:52.000000 data_loader_lib-0.1/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-17 18:18:25.196734 data_loader_lib-0.1/src/
-drwxrwxrwx   0        0        0        0 2024-05-17 18:18:25.247837 data_loader_lib-0.1/src/data_loader_lib.egg-info/
--rw-rw-rw-   0        0        0      552 2024-05-17 18:18:24.000000 data_loader_lib-0.1/src/data_loader_lib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      222 2024-05-17 18:18:25.000000 data_loader_lib-0.1/src/data_loader_lib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-17 18:18:24.000000 data_loader_lib-0.1/src/data_loader_lib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       58 2024-05-17 18:18:24.000000 data_loader_lib-0.1/src/data_loader_lib.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2024-05-17 18:18:24.000000 data_loader_lib-0.1/src/data_loader_lib.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-18 16:30:17.013125 data_loader_lib-0.2/
+-rw-rw-rw-   0        0        0      611 2024-05-18 16:30:17.012125 data_loader_lib-0.2/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2024-05-18 16:30:17.014124 data_loader_lib-0.2/setup.cfg
+-rw-rw-rw-   0        0        0      785 2024-05-18 16:28:28.000000 data_loader_lib-0.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-18 16:30:16.972458 data_loader_lib-0.2/src/
+drwxrwxrwx   0        0        0        0 2024-05-18 16:30:17.010125 data_loader_lib-0.2/src/data_loader_lib.egg-info/
+-rw-rw-rw-   0        0        0      611 2024-05-18 16:30:16.000000 data_loader_lib-0.2/src/data_loader_lib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      315 2024-05-18 16:30:16.000000 data_loader_lib-0.2/src/data_loader_lib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-18 16:30:16.000000 data_loader_lib-0.2/src/data_loader_lib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       83 2024-05-18 16:30:16.000000 data_loader_lib-0.2/src/data_loader_lib.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2024-05-18 16:30:16.000000 data_loader_lib-0.2/src/data_loader_lib.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-18 16:30:17.007030 data_loader_lib-0.2/tests/
+-rw-rw-rw-   0        0        0      920 2024-05-18 16:13:12.000000 data_loader_lib-0.2/tests/test_bigquery_loader.py
+-rw-rw-rw-   0        0        0     1430 2024-05-18 16:12:56.000000 data_loader_lib-0.2/tests/test_local_file_loader.py
+-rw-rw-rw-   0        0        0     1457 2024-05-18 16:13:04.000000 data_loader_lib-0.2/tests/test_sftp_file_loader.py
```

### Comparing `data_loader_lib-0.1/PKG-INFO` & `data_loader_lib-0.2/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 Metadata-Version: 2.1
 Name: data_loader_lib
-Version: 0.1
+Version: 0.2
 Summary: Librería para cargar datos desde diferentes fuentes en un DataFrame
-Home-page: http://onbotgo.com
-Author: Tu Nombre
-Author-email: reyesramirezricardoemanuel@gmail.com
+Home-page: http://example.com
+Author: Ricardo Reyes
+Author-email: reyesramirezcardoemanuel@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Requires-Dist: pandas
 Requires-Dist: paramiko
 Requires-Dist: sqlalchemy
 Requires-Dist: google-cloud-bigquery
 Requires-Dist: injector
+Requires-Dist: python-dotenv
+Requires-Dist: matplotlib
```

### Comparing `data_loader_lib-0.1/setup.py` & `data_loader_lib-0.2/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,26 +1,27 @@
-# setup.py
 from setuptools import setup, find_packages
 
 setup(
     name="data_loader_lib",
-    version="0.1",
+    version="0.2",
     packages=find_packages(where='src'),
     package_dir={'': 'src'},
     install_requires=[
         "pandas",
         "paramiko",
         "sqlalchemy",
         "google-cloud-bigquery",
-        "injector"
+        "injector",
+        "python-dotenv",
+        "matplotlib"
     ],
-    author="Tu Nombre",
-    author_email="reyesramirezricardoemanuel@gmail.com",
+    author="Ricardo Reyes",
+    author_email="reyesramirezcardoemanuel@gmail.com",
     description="Librería para cargar datos desde diferentes fuentes en un DataFrame",
-    url="http://onbotgo.com",
+    url="http://example.com",
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     python_requires='>=3.6',
 )
```

### Comparing `data_loader_lib-0.1/src/data_loader_lib.egg-info/PKG-INFO` & `data_loader_lib-0.2/src/data_loader_lib.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 Metadata-Version: 2.1
 Name: data_loader_lib
-Version: 0.1
+Version: 0.2
 Summary: Librería para cargar datos desde diferentes fuentes en un DataFrame
-Home-page: http://onbotgo.com
-Author: Tu Nombre
-Author-email: reyesramirezricardoemanuel@gmail.com
+Home-page: http://example.com
+Author: Ricardo Reyes
+Author-email: reyesramirezcardoemanuel@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Requires-Dist: pandas
 Requires-Dist: paramiko
 Requires-Dist: sqlalchemy
 Requires-Dist: google-cloud-bigquery
 Requires-Dist: injector
+Requires-Dist: python-dotenv
+Requires-Dist: matplotlib
```

