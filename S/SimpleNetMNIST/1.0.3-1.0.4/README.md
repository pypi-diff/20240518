# Comparing `tmp/simplenetmnist-1.0.3.tar.gz` & `tmp/simplenetmnist-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simplenetmnist-1.0.3.tar", last modified: Wed May 15 12:11:07 2024, max compression
+gzip compressed data, was "simplenetmnist-1.0.4.tar", last modified: Sat May 18 13:25:59 2024, max compression
```

## Comparing `simplenetmnist-1.0.3.tar` & `simplenetmnist-1.0.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 dane      (1000) dane      (1000)        0 2024-05-15 12:11:07.395342 simplenetmnist-1.0.3/
--rw-r--r--   0 dane      (1000) dane      (1000)     1066 2024-03-16 20:05:16.000000 simplenetmnist-1.0.3/LICENSE
--rw-r--r--   0 dane      (1000) dane      (1000)     2144 2024-05-15 12:11:07.395342 simplenetmnist-1.0.3/PKG-INFO
--rw-r--r--   0 dane      (1000) dane      (1000)      219 2024-03-16 20:05:16.000000 simplenetmnist-1.0.3/README.md
-drwxr-xr-x   0 dane      (1000) dane      (1000)        0 2024-05-15 12:11:07.395342 simplenetmnist-1.0.3/SimpleNetMNIST/
--rw-r--r--   0 dane      (1000) dane      (1000)     3114 2024-03-16 20:05:16.000000 simplenetmnist-1.0.3/SimpleNetMNIST/predict.py
--rw-r--r--   0 dane      (1000) dane      (1000)     6959 2024-03-18 17:07:44.000000 simplenetmnist-1.0.3/SimpleNetMNIST/simpnet.py
--rw-r--r--   0 dane      (1000) dane      (1000)     4634 2024-03-16 20:05:16.000000 simplenetmnist-1.0.3/SimpleNetMNIST/train.py
--rw-r--r--   0 dane      (1000) dane      (1000)     1592 2024-03-16 20:05:16.000000 simplenetmnist-1.0.3/SimpleNetMNIST/utils.py
-drwxr-xr-x   0 dane      (1000) dane      (1000)        0 2024-05-15 12:11:07.395342 simplenetmnist-1.0.3/SimpleNetMNIST.egg-info/
--rw-r--r--   0 dane      (1000) dane      (1000)     2144 2024-05-15 12:11:07.000000 simplenetmnist-1.0.3/SimpleNetMNIST.egg-info/PKG-INFO
--rw-r--r--   0 dane      (1000) dane      (1000)      330 2024-05-15 12:11:07.000000 simplenetmnist-1.0.3/SimpleNetMNIST.egg-info/SOURCES.txt
--rw-r--r--   0 dane      (1000) dane      (1000)        1 2024-05-15 12:11:07.000000 simplenetmnist-1.0.3/SimpleNetMNIST.egg-info/dependency_links.txt
--rw-r--r--   0 dane      (1000) dane      (1000)       11 2024-05-15 12:11:07.000000 simplenetmnist-1.0.3/SimpleNetMNIST.egg-info/requires.txt
--rw-r--r--   0 dane      (1000) dane      (1000)       15 2024-05-15 12:11:07.000000 simplenetmnist-1.0.3/SimpleNetMNIST.egg-info/top_level.txt
--rw-r--r--   0 dane      (1000) dane      (1000)      827 2024-05-15 12:10:15.000000 simplenetmnist-1.0.3/pyproject.toml
--rw-r--r--   0 dane      (1000) dane      (1000)       38 2024-05-15 12:11:07.395342 simplenetmnist-1.0.3/setup.cfg
--rw-r--r--   0 dane      (1000) dane      (1000)      160 2024-03-16 21:53:55.000000 simplenetmnist-1.0.3/setup.py
+drwxr-xr-x   0 dane      (1000) dane      (1000)        0 2024-05-18 13:25:59.010821 simplenetmnist-1.0.4/
+-rw-r--r--   0 dane      (1000) dane      (1000)     1066 2024-03-16 20:05:16.000000 simplenetmnist-1.0.4/LICENSE
+-rw-r--r--   0 dane      (1000) dane      (1000)     2144 2024-05-18 13:25:59.010821 simplenetmnist-1.0.4/PKG-INFO
+-rw-r--r--   0 dane      (1000) dane      (1000)      219 2024-03-16 20:05:16.000000 simplenetmnist-1.0.4/README.md
+drwxr-xr-x   0 dane      (1000) dane      (1000)        0 2024-05-18 13:25:59.010821 simplenetmnist-1.0.4/SimpleNetMNIST/
+-rw-r--r--   0 dane      (1000) dane      (1000)     3114 2024-03-16 20:05:16.000000 simplenetmnist-1.0.4/SimpleNetMNIST/predict.py
+-rw-r--r--   0 dane      (1000) dane      (1000)     6959 2024-03-18 17:07:44.000000 simplenetmnist-1.0.4/SimpleNetMNIST/simpnet.py
+-rw-r--r--   0 dane      (1000) dane      (1000)     4634 2024-03-16 20:05:16.000000 simplenetmnist-1.0.4/SimpleNetMNIST/train.py
+-rw-r--r--   0 dane      (1000) dane      (1000)     1592 2024-03-16 20:05:16.000000 simplenetmnist-1.0.4/SimpleNetMNIST/utils.py
+drwxr-xr-x   0 dane      (1000) dane      (1000)        0 2024-05-18 13:25:59.010821 simplenetmnist-1.0.4/SimpleNetMNIST.egg-info/
+-rw-r--r--   0 dane      (1000) dane      (1000)     2144 2024-05-18 13:25:59.000000 simplenetmnist-1.0.4/SimpleNetMNIST.egg-info/PKG-INFO
+-rw-r--r--   0 dane      (1000) dane      (1000)      330 2024-05-18 13:25:59.000000 simplenetmnist-1.0.4/SimpleNetMNIST.egg-info/SOURCES.txt
+-rw-r--r--   0 dane      (1000) dane      (1000)        1 2024-05-18 13:25:59.000000 simplenetmnist-1.0.4/SimpleNetMNIST.egg-info/dependency_links.txt
+-rw-r--r--   0 dane      (1000) dane      (1000)       11 2024-05-18 13:25:59.000000 simplenetmnist-1.0.4/SimpleNetMNIST.egg-info/requires.txt
+-rw-r--r--   0 dane      (1000) dane      (1000)       15 2024-05-18 13:25:59.000000 simplenetmnist-1.0.4/SimpleNetMNIST.egg-info/top_level.txt
+-rw-r--r--   0 dane      (1000) dane      (1000)      827 2024-05-18 13:23:33.000000 simplenetmnist-1.0.4/pyproject.toml
+-rw-r--r--   0 dane      (1000) dane      (1000)       38 2024-05-18 13:25:59.010821 simplenetmnist-1.0.4/setup.cfg
+-rw-r--r--   0 dane      (1000) dane      (1000)      160 2024-03-16 21:53:55.000000 simplenetmnist-1.0.4/setup.py
```

### Comparing `simplenetmnist-1.0.3/LICENSE` & `simplenetmnist-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `simplenetmnist-1.0.3/PKG-INFO` & `simplenetmnist-1.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SimpleNetMNIST
-Version: 1.0.3
+Version: 1.0.4
 Summary: SimpleNetMNIST.  Based off an implementation of a simple neural network for MNIST classification in PyTorch. Created by Edward Ji (https://github.com/Edward-Ji).
 Author-email: Edward Ji <jiziao6@gmail.com>, Daniel Elliott <danelliottster@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 Edward Ji
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -26,15 +26,15 @@
         SOFTWARE.
         
 Project-URL: homepage, https://github.com/danelliottster/SimpleNetMNIST
 Keywords: pytorch,mnist,neural network
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.9
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: torch>=2.0
 
 ---
 title: SimpleNetMNSIT
 emoji: ✍️
```

### Comparing `simplenetmnist-1.0.3/SimpleNetMNIST/predict.py` & `simplenetmnist-1.0.4/SimpleNetMNIST/predict.py`

 * *Files identical despite different names*

### Comparing `simplenetmnist-1.0.3/SimpleNetMNIST/simpnet.py` & `simplenetmnist-1.0.4/SimpleNetMNIST/simpnet.py`

 * *Files identical despite different names*

### Comparing `simplenetmnist-1.0.3/SimpleNetMNIST/train.py` & `simplenetmnist-1.0.4/SimpleNetMNIST/train.py`

 * *Files identical despite different names*

### Comparing `simplenetmnist-1.0.3/SimpleNetMNIST/utils.py` & `simplenetmnist-1.0.4/SimpleNetMNIST/utils.py`

 * *Files identical despite different names*

### Comparing `simplenetmnist-1.0.3/SimpleNetMNIST.egg-info/PKG-INFO` & `simplenetmnist-1.0.4/SimpleNetMNIST.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SimpleNetMNIST
-Version: 1.0.3
+Version: 1.0.4
 Summary: SimpleNetMNIST.  Based off an implementation of a simple neural network for MNIST classification in PyTorch. Created by Edward Ji (https://github.com/Edward-Ji).
 Author-email: Edward Ji <jiziao6@gmail.com>, Daniel Elliott <danelliottster@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 Edward Ji
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -26,15 +26,15 @@
         SOFTWARE.
         
 Project-URL: homepage, https://github.com/danelliottster/SimpleNetMNIST
 Keywords: pytorch,mnist,neural network
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.9
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: torch>=2.0
 
 ---
 title: SimpleNetMNSIT
 emoji: ✍️
```

### Comparing `simplenetmnist-1.0.3/pyproject.toml` & `simplenetmnist-1.0.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "SimpleNetMNIST"
-version = "1.0.3"
+version = "1.0.4"
 description = "SimpleNetMNIST.  Based off an implementation of a simple neural network for MNIST classification in PyTorch. Created by Edward Ji (https://github.com/Edward-Ji)."
 authors = [ {name="Edward Ji", email="jiziao6@gmail.com"} , {name="Daniel Elliott", email="danelliottster@gmail.com"} ]
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
 ]
 keywords = ["pytorch", "mnist", "neural network"]
 license = { file="LICENSE" }
 readme = "README.md"
 dependencies = [
     "torch>=2.0"
 ]
-requires-python = ">=3.9"
+requires-python = ">=3.8"
 
 [project.urls]
 homepage = "https://github.com/danelliottster/SimpleNetMNIST"
```

