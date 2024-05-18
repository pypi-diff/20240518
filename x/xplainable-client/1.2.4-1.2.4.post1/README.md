# Comparing `tmp/xplainable-client-1.2.4.tar.gz` & `tmp/xplainable-client-1.2.4.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xplainable-client-1.2.4.tar", last modified: Sat May 18 01:38:24 2024, max compression
+gzip compressed data, was "xplainable-client-1.2.4.post1.tar", last modified: Sat May 18 01:48:20 2024, max compression
```

## Comparing `xplainable-client-1.2.4.tar` & `xplainable-client-1.2.4.post1.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 jtuppack   (501) staff       (20)        0 2024-05-18 01:38:24.200857 xplainable-client-1.2.4/
--rw-r--r--   0 jtuppack   (501) staff       (20)    34523 2024-05-18 01:38:20.000000 xplainable-client-1.2.4/LICENSE
--rw-r--r--   0 jtuppack   (501) staff       (20)    44573 2024-05-18 01:38:24.200489 xplainable-client-1.2.4/PKG-INFO
--rw-r--r--   0 jtuppack   (501) staff       (20)     3924 2024-02-21 21:39:20.000000 xplainable-client-1.2.4/README.md
--rw-r--r--   0 jtuppack   (501) staff       (20)      852 2024-05-17 23:15:50.000000 xplainable-client-1.2.4/pyproject.toml
--rw-r--r--   0 jtuppack   (501) staff       (20)       38 2024-05-18 01:38:24.200912 xplainable-client-1.2.4/setup.cfg
--rw-r--r--   0 jtuppack   (501) staff       (20)      822 2024-05-18 01:38:20.000000 xplainable-client-1.2.4/setup.py
-drwxr-xr-x   0 jtuppack   (501) staff       (20)        0 2024-05-18 01:38:24.195128 xplainable-client-1.2.4/tests/
--rw-r--r--   0 jtuppack   (501) staff       (20)      270 2024-05-18 01:38:20.000000 xplainable-client-1.2.4/tests/test_model.py
--rw-r--r--   0 jtuppack   (501) staff       (20)      184 2024-05-18 01:38:20.000000 xplainable-client-1.2.4/tests/test_test.py
-drwxr-xr-x   0 jtuppack   (501) staff       (20)        0 2024-05-18 01:38:24.195239 xplainable-client-1.2.4/xplainable_client/
--rw-r--r--   0 jtuppack   (501) staff       (20)       27 2024-05-17 23:15:50.000000 xplainable-client-1.2.4/xplainable_client/__init__.py
-drwxr-xr-x   0 jtuppack   (501) staff       (20)        0 2024-05-18 01:38:24.199033 xplainable-client-1.2.4/xplainable_client/client/
--rw-r--r--   0 jtuppack   (501) staff       (20)      946 2024-05-17 23:15:50.000000 xplainable-client-1.2.4/xplainable_client/client/__init__.py
--rw-r--r--   0 jtuppack   (501) staff       (20)      123 2024-05-16 09:16:42.000000 xplainable-client-1.2.4/xplainable_client/client/_client_cog_base.py
--rw-r--r--   0 jtuppack   (501) staff       (20)     7324 2024-05-17 23:15:50.000000 xplainable-client-1.2.4/xplainable_client/client/_collections.py
--rw-r--r--   0 jtuppack   (501) staff       (20)     1245 2024-05-16 09:16:42.000000 xplainable-client-1.2.4/xplainable_client/client/_datasets.py
--rw-r--r--   0 jtuppack   (501) staff       (20)    14605 2024-05-17 23:15:50.000000 xplainable-client-1.2.4/xplainable_client/client/_deployments.py
--rw-r--r--   0 jtuppack   (501) staff       (20)     1218 2024-05-17 03:09:19.000000 xplainable-client-1.2.4/xplainable_client/client/_gpt.py
--rw-r--r--   0 jtuppack   (501) staff       (20)     1236 2024-05-17 23:15:50.000000 xplainable-client-1.2.4/xplainable_client/client/_inference.py
--rw-r--r--   0 jtuppack   (501) staff       (20)     7982 2024-05-17 23:15:50.000000 xplainable-client-1.2.4/xplainable_client/client/_misc.py
--rw-r--r--   0 jtuppack   (501) staff       (20)    20834 2024-05-17 23:17:59.000000 xplainable-client-1.2.4/xplainable_client/client/_models.py
--rw-r--r--   0 jtuppack   (501) staff       (20)     9359 2024-05-17 23:15:50.000000 xplainable-client-1.2.4/xplainable_client/client/_preprocessing.py
--rw-r--r--   0 jtuppack   (501) staff       (20)     4020 2024-05-17 23:15:50.000000 xplainable-client-1.2.4/xplainable_client/client/_session.py
-drwxr-xr-x   0 jtuppack   (501) staff       (20)        0 2024-05-18 01:38:24.199734 xplainable-client-1.2.4/xplainable_client/client/utils/
--rw-r--r--   0 jtuppack   (501) staff       (20)      122 2024-05-17 23:15:50.000000 xplainable-client-1.2.4/xplainable_client/client/utils/__init__.py
--rw-r--r--   0 jtuppack   (501) staff       (20)     1291 2024-05-17 23:15:50.000000 xplainable-client-1.2.4/xplainable_client/client/utils/encoders.py
--rw-r--r--   0 jtuppack   (501) staff       (20)      961 2024-05-17 23:15:50.000000 xplainable-client-1.2.4/xplainable_client/client/utils/helpers.py
--rw-r--r--   0 jtuppack   (501) staff       (20)     6416 2024-05-17 23:15:50.000000 xplainable-client-1.2.4/xplainable_client/client/utils/metrics.py
--rw-r--r--   0 jtuppack   (501) staff       (20)     3042 2024-05-17 23:15:50.000000 xplainable-client-1.2.4/xplainable_client/client/utils/model_parsers.py
--rw-r--r--   0 jtuppack   (501) staff       (20)    10432 2024-05-17 23:15:50.000000 xplainable-client-1.2.4/xplainable_client/client/utils/scanner.py
-drwxr-xr-x   0 jtuppack   (501) staff       (20)        0 2024-05-18 01:38:24.199850 xplainable-client-1.2.4/xplainable_client/models/
--rw-r--r--   0 jtuppack   (501) staff       (20)     4057 2024-03-04 22:40:48.000000 xplainable-client-1.2.4/xplainable_client/models/ebm.py
-drwxr-xr-x   0 jtuppack   (501) staff       (20)        0 2024-05-18 01:38:24.197328 xplainable-client-1.2.4/xplainable_client.egg-info/
--rw-r--r--   0 jtuppack   (501) staff       (20)    44573 2024-05-18 01:38:24.000000 xplainable-client-1.2.4/xplainable_client.egg-info/PKG-INFO
--rw-r--r--   0 jtuppack   (501) staff       (20)     1030 2024-05-18 01:38:24.000000 xplainable-client-1.2.4/xplainable_client.egg-info/SOURCES.txt
--rw-r--r--   0 jtuppack   (501) staff       (20)        1 2024-05-18 01:38:24.000000 xplainable-client-1.2.4/xplainable_client.egg-info/dependency_links.txt
--rw-r--r--   0 jtuppack   (501) staff       (20)      135 2024-05-18 01:38:24.000000 xplainable-client-1.2.4/xplainable_client.egg-info/requires.txt
--rw-r--r--   0 jtuppack   (501) staff       (20)       24 2024-05-18 01:38:24.000000 xplainable-client-1.2.4/xplainable_client.egg-info/top_level.txt
+drwxr-xr-x   0 jtuppack   (501) staff       (20)        0 2024-05-18 01:48:20.120806 xplainable-client-1.2.4.post1/
+-rw-r--r--   0 jtuppack   (501) staff       (20)    34523 2024-05-18 01:38:20.000000 xplainable-client-1.2.4.post1/LICENSE
+-rw-r--r--   0 jtuppack   (501) staff       (20)    44077 2024-05-18 01:48:20.120604 xplainable-client-1.2.4.post1/PKG-INFO
+-rw-r--r--   0 jtuppack   (501) staff       (20)     3924 2024-02-21 21:39:20.000000 xplainable-client-1.2.4.post1/README.md
+-rw-r--r--   0 jtuppack   (501) staff       (20)      852 2024-05-17 23:15:50.000000 xplainable-client-1.2.4.post1/pyproject.toml
+-rw-r--r--   0 jtuppack   (501) staff       (20)       38 2024-05-18 01:48:20.120858 xplainable-client-1.2.4.post1/setup.cfg
+-rw-r--r--   0 jtuppack   (501) staff       (20)      823 2024-05-18 01:48:16.000000 xplainable-client-1.2.4.post1/setup.py
+drwxr-xr-x   0 jtuppack   (501) staff       (20)        0 2024-05-18 01:48:20.115805 xplainable-client-1.2.4.post1/tests/
+-rw-r--r--   0 jtuppack   (501) staff       (20)      270 2024-05-18 01:38:20.000000 xplainable-client-1.2.4.post1/tests/test_model.py
+-rw-r--r--   0 jtuppack   (501) staff       (20)      184 2024-05-18 01:38:20.000000 xplainable-client-1.2.4.post1/tests/test_test.py
+drwxr-xr-x   0 jtuppack   (501) staff       (20)        0 2024-05-18 01:48:20.115927 xplainable-client-1.2.4.post1/xplainable_client/
+-rw-r--r--   0 jtuppack   (501) staff       (20)       27 2024-05-17 23:15:50.000000 xplainable-client-1.2.4.post1/xplainable_client/__init__.py
+drwxr-xr-x   0 jtuppack   (501) staff       (20)        0 2024-05-18 01:48:20.118784 xplainable-client-1.2.4.post1/xplainable_client/client/
+-rw-r--r--   0 jtuppack   (501) staff       (20)      946 2024-05-17 23:15:50.000000 xplainable-client-1.2.4.post1/xplainable_client/client/__init__.py
+-rw-r--r--   0 jtuppack   (501) staff       (20)      123 2024-05-16 09:16:42.000000 xplainable-client-1.2.4.post1/xplainable_client/client/_client_cog_base.py
+-rw-r--r--   0 jtuppack   (501) staff       (20)     7324 2024-05-17 23:15:50.000000 xplainable-client-1.2.4.post1/xplainable_client/client/_collections.py
+-rw-r--r--   0 jtuppack   (501) staff       (20)     1245 2024-05-16 09:16:42.000000 xplainable-client-1.2.4.post1/xplainable_client/client/_datasets.py
+-rw-r--r--   0 jtuppack   (501) staff       (20)    14605 2024-05-17 23:15:50.000000 xplainable-client-1.2.4.post1/xplainable_client/client/_deployments.py
+-rw-r--r--   0 jtuppack   (501) staff       (20)     1218 2024-05-17 03:09:19.000000 xplainable-client-1.2.4.post1/xplainable_client/client/_gpt.py
+-rw-r--r--   0 jtuppack   (501) staff       (20)     1236 2024-05-17 23:15:50.000000 xplainable-client-1.2.4.post1/xplainable_client/client/_inference.py
+-rw-r--r--   0 jtuppack   (501) staff       (20)     7982 2024-05-17 23:15:50.000000 xplainable-client-1.2.4.post1/xplainable_client/client/_misc.py
+-rw-r--r--   0 jtuppack   (501) staff       (20)    20834 2024-05-17 23:17:59.000000 xplainable-client-1.2.4.post1/xplainable_client/client/_models.py
+-rw-r--r--   0 jtuppack   (501) staff       (20)     9359 2024-05-17 23:15:50.000000 xplainable-client-1.2.4.post1/xplainable_client/client/_preprocessing.py
+-rw-r--r--   0 jtuppack   (501) staff       (20)     4020 2024-05-17 23:15:50.000000 xplainable-client-1.2.4.post1/xplainable_client/client/_session.py
+drwxr-xr-x   0 jtuppack   (501) staff       (20)        0 2024-05-18 01:48:20.119859 xplainable-client-1.2.4.post1/xplainable_client/client/utils/
+-rw-r--r--   0 jtuppack   (501) staff       (20)      122 2024-05-17 23:15:50.000000 xplainable-client-1.2.4.post1/xplainable_client/client/utils/__init__.py
+-rw-r--r--   0 jtuppack   (501) staff       (20)     1291 2024-05-17 23:15:50.000000 xplainable-client-1.2.4.post1/xplainable_client/client/utils/encoders.py
+-rw-r--r--   0 jtuppack   (501) staff       (20)      961 2024-05-17 23:15:50.000000 xplainable-client-1.2.4.post1/xplainable_client/client/utils/helpers.py
+-rw-r--r--   0 jtuppack   (501) staff       (20)     6416 2024-05-17 23:15:50.000000 xplainable-client-1.2.4.post1/xplainable_client/client/utils/metrics.py
+-rw-r--r--   0 jtuppack   (501) staff       (20)     3042 2024-05-17 23:15:50.000000 xplainable-client-1.2.4.post1/xplainable_client/client/utils/model_parsers.py
+-rw-r--r--   0 jtuppack   (501) staff       (20)    10432 2024-05-17 23:15:50.000000 xplainable-client-1.2.4.post1/xplainable_client/client/utils/scanner.py
+drwxr-xr-x   0 jtuppack   (501) staff       (20)        0 2024-05-18 01:48:20.120150 xplainable-client-1.2.4.post1/xplainable_client/models/
+-rw-r--r--   0 jtuppack   (501) staff       (20)     4057 2024-03-04 22:40:48.000000 xplainable-client-1.2.4.post1/xplainable_client/models/ebm.py
+drwxr-xr-x   0 jtuppack   (501) staff       (20)        0 2024-05-18 01:48:20.116581 xplainable-client-1.2.4.post1/xplainable_client.egg-info/
+-rw-r--r--   0 jtuppack   (501) staff       (20)    44077 2024-05-18 01:48:20.000000 xplainable-client-1.2.4.post1/xplainable_client.egg-info/PKG-INFO
+-rw-r--r--   0 jtuppack   (501) staff       (20)     1030 2024-05-18 01:48:20.000000 xplainable-client-1.2.4.post1/xplainable_client.egg-info/SOURCES.txt
+-rw-r--r--   0 jtuppack   (501) staff       (20)        1 2024-05-18 01:48:20.000000 xplainable-client-1.2.4.post1/xplainable_client.egg-info/dependency_links.txt
+-rw-r--r--   0 jtuppack   (501) staff       (20)      135 2024-05-18 01:48:20.000000 xplainable-client-1.2.4.post1/xplainable_client.egg-info/requires.txt
+-rw-r--r--   0 jtuppack   (501) staff       (20)       18 2024-05-18 01:48:20.000000 xplainable-client-1.2.4.post1/xplainable_client.egg-info/top_level.txt
```

### Comparing `xplainable-client-1.2.4/LICENSE` & `xplainable-client-1.2.4.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `xplainable-client-1.2.4/PKG-INFO` & `xplainable-client-1.2.4.post1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 Metadata-Version: 2.1
 Name: xplainable-client
-Version: 1.2.4
+Version: 1.2.4.post1
 Summary: The client for persisting and deploying models to Xplainable cloud.
+Home-page: UNKNOWN
 Author: xplainable pty ltd
-Author-email: xplainable pty ltd <contact@xplainable.io>
+Author-email: contact@xplainable.io
 License:                     GNU AFFERO GENERAL PUBLIC LICENSE
                                Version 3, 19 November 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
          of this license document, but changing it is not allowed.
         
@@ -662,31 +663,18 @@
         specific requirements.
         
           You should also get your employer (if you work as a programmer) or school,
         if any, to sign a "copyright disclaimer" for the program, if necessary.
         For more information on this, and how to apply and follow the GNU AGPL, see
         <https://www.gnu.org/licenses/>.
         
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.11
+Platform: UNKNOWN
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: ipywidgets==8.0.6
-Requires-Dist: numpy>=1.26
-Requires-Dist: pandas>=1.5.2
-Requires-Dist: pyperclip==1.8.2
-Requires-Dist: Requests==2.31.0
-Requires-Dist: scikit_learn
-Requires-Dist: setuptools
-Requires-Dist: urllib3==2.2.0
-Requires-Dist: xplainable==1.2.4
 
 
 <div align="center">
 <img src="https://raw.githubusercontent.com/xplainable/xplainable/main/docs/assets/logo/xplainable-logo.png">
 <h1 align="center">xplainable</h1>
 <h3 align="center">Real-time explainable machine learning for business optimisation</h3>
     
@@ -798,7 +786,9 @@
 <strong>Made with ❤️ in Australia</strong>
 <br></br>
 <hr>
 &copy; copyright xplainable pty ltd
 </div>
 
 
+
+
```

### Comparing `xplainable-client-1.2.4/README.md` & `xplainable-client-1.2.4.post1/README.md`

 * *Files identical despite different names*

### Comparing `xplainable-client-1.2.4/pyproject.toml` & `xplainable-client-1.2.4.post1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `xplainable-client-1.2.4/setup.py` & `xplainable-client-1.2.4.post1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,23 +4,23 @@
     description = f.read()
 
 with open("LICENSE", "r") as f:
     license = f.read()
 
 setuptools.setup(
     name="xplainable-client",
-    version="1.2.4",
+    version="1.2.4-1",
     author="xplainable pty ltd",
     author_email="contact@xplainable.io",
     packages=["xplainable_client"],
     description="The client for persisting and deploying models to Xplainable cloud.",
     long_description=description,
     long_description_content_type="text/markdown",
     license=license,
-    python_requires='>=3.11',
+    python_requires='>=3.8',
     install_requires=[
         "ipywidgets==8.0.6",
         "numpy>=1.26",
         "pandas>=1.5.2",
         "pyperclip==1.8.2",
         "Requests==2.31.0",
         "scikit_learn",
```

### Comparing `xplainable-client-1.2.4/xplainable_client/client/__init__.py` & `xplainable-client-1.2.4.post1/xplainable_client/client/__init__.py`

 * *Files identical despite different names*

### Comparing `xplainable-client-1.2.4/xplainable_client/client/_collections.py` & `xplainable-client-1.2.4.post1/xplainable_client/client/_collections.py`

 * *Files identical despite different names*

### Comparing `xplainable-client-1.2.4/xplainable_client/client/_datasets.py` & `xplainable-client-1.2.4.post1/xplainable_client/client/_datasets.py`

 * *Files identical despite different names*

### Comparing `xplainable-client-1.2.4/xplainable_client/client/_deployments.py` & `xplainable-client-1.2.4.post1/xplainable_client/client/_deployments.py`

 * *Files identical despite different names*

### Comparing `xplainable-client-1.2.4/xplainable_client/client/_gpt.py` & `xplainable-client-1.2.4.post1/xplainable_client/client/_gpt.py`

 * *Files identical despite different names*

### Comparing `xplainable-client-1.2.4/xplainable_client/client/_inference.py` & `xplainable-client-1.2.4.post1/xplainable_client/client/_inference.py`

 * *Files identical despite different names*

### Comparing `xplainable-client-1.2.4/xplainable_client/client/_misc.py` & `xplainable-client-1.2.4.post1/xplainable_client/client/_misc.py`

 * *Files identical despite different names*

### Comparing `xplainable-client-1.2.4/xplainable_client/client/_models.py` & `xplainable-client-1.2.4.post1/xplainable_client/client/_models.py`

 * *Files identical despite different names*

### Comparing `xplainable-client-1.2.4/xplainable_client/client/_preprocessing.py` & `xplainable-client-1.2.4.post1/xplainable_client/client/_preprocessing.py`

 * *Files identical despite different names*

### Comparing `xplainable-client-1.2.4/xplainable_client/client/_session.py` & `xplainable-client-1.2.4.post1/xplainable_client/client/_session.py`

 * *Files identical despite different names*

### Comparing `xplainable-client-1.2.4/xplainable_client/client/utils/encoders.py` & `xplainable-client-1.2.4.post1/xplainable_client/client/utils/encoders.py`

 * *Files identical despite different names*

### Comparing `xplainable-client-1.2.4/xplainable_client/client/utils/helpers.py` & `xplainable-client-1.2.4.post1/xplainable_client/client/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `xplainable-client-1.2.4/xplainable_client/client/utils/metrics.py` & `xplainable-client-1.2.4.post1/xplainable_client/client/utils/metrics.py`

 * *Files identical despite different names*

### Comparing `xplainable-client-1.2.4/xplainable_client/client/utils/model_parsers.py` & `xplainable-client-1.2.4.post1/xplainable_client/client/utils/model_parsers.py`

 * *Files identical despite different names*

### Comparing `xplainable-client-1.2.4/xplainable_client/client/utils/scanner.py` & `xplainable-client-1.2.4.post1/xplainable_client/client/utils/scanner.py`

 * *Files identical despite different names*

### Comparing `xplainable-client-1.2.4/xplainable_client/models/ebm.py` & `xplainable-client-1.2.4.post1/xplainable_client/models/ebm.py`

 * *Files identical despite different names*

### Comparing `xplainable-client-1.2.4/xplainable_client.egg-info/PKG-INFO` & `xplainable-client-1.2.4.post1/xplainable_client.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 Metadata-Version: 2.1
 Name: xplainable-client
-Version: 1.2.4
+Version: 1.2.4.post1
 Summary: The client for persisting and deploying models to Xplainable cloud.
+Home-page: UNKNOWN
 Author: xplainable pty ltd
-Author-email: xplainable pty ltd <contact@xplainable.io>
+Author-email: contact@xplainable.io
 License:                     GNU AFFERO GENERAL PUBLIC LICENSE
                                Version 3, 19 November 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
          of this license document, but changing it is not allowed.
         
@@ -662,31 +663,18 @@
         specific requirements.
         
           You should also get your employer (if you work as a programmer) or school,
         if any, to sign a "copyright disclaimer" for the program, if necessary.
         For more information on this, and how to apply and follow the GNU AGPL, see
         <https://www.gnu.org/licenses/>.
         
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.11
+Platform: UNKNOWN
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: ipywidgets==8.0.6
-Requires-Dist: numpy>=1.26
-Requires-Dist: pandas>=1.5.2
-Requires-Dist: pyperclip==1.8.2
-Requires-Dist: Requests==2.31.0
-Requires-Dist: scikit_learn
-Requires-Dist: setuptools
-Requires-Dist: urllib3==2.2.0
-Requires-Dist: xplainable==1.2.4
 
 
 <div align="center">
 <img src="https://raw.githubusercontent.com/xplainable/xplainable/main/docs/assets/logo/xplainable-logo.png">
 <h1 align="center">xplainable</h1>
 <h3 align="center">Real-time explainable machine learning for business optimisation</h3>
     
@@ -798,7 +786,9 @@
 <strong>Made with ❤️ in Australia</strong>
 <br></br>
 <hr>
 &copy; copyright xplainable pty ltd
 </div>
 
 
+
+
```

### Comparing `xplainable-client-1.2.4/xplainable_client.egg-info/SOURCES.txt` & `xplainable-client-1.2.4.post1/xplainable_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

