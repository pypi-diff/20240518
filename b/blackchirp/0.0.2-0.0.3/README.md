# Comparing `tmp/blackchirp-0.0.2.tar.gz` & `tmp/blackchirp-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "blackchirp-0.0.2.tar", last modified: Thu May 16 00:30:53 2024, max compression
+gzip compressed data, was "blackchirp-0.0.3.tar", last modified: Fri May 17 23:16:56 2024, max compression
```

## Comparing `blackchirp-0.0.2.tar` & `blackchirp-0.0.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 kncrabtree  (1000) users      (100)        0 2024-05-16 00:30:53.599635 blackchirp-0.0.2/
--rw-r--r--   0 kncrabtree  (1000) users      (100)     1069 2024-05-15 23:44:25.000000 blackchirp-0.0.2/LICENSE
--rw-r--r--   0 kncrabtree  (1000) users      (100)      918 2024-05-16 00:30:53.599635 blackchirp-0.0.2/PKG-INFO
--rw-r--r--   0 kncrabtree  (1000) users      (100)      451 2024-05-15 23:52:03.000000 blackchirp-0.0.2/README.md
--rw-r--r--   0 kncrabtree  (1000) users      (100)      459 2024-05-16 00:29:28.000000 blackchirp-0.0.2/pyproject.toml
--rw-r--r--   0 kncrabtree  (1000) users      (100)       38 2024-05-16 00:30:53.599635 blackchirp-0.0.2/setup.cfg
-drwxr-xr-x   0 kncrabtree  (1000) users      (100)        0 2024-05-16 00:30:53.599635 blackchirp-0.0.2/src/
-drwxr-xr-x   0 kncrabtree  (1000) users      (100)        0 2024-05-16 00:30:53.599635 blackchirp-0.0.2/src/blackchirp/
--rw-r--r--   0 kncrabtree  (1000) users      (100)      124 2024-05-15 22:44:55.000000 blackchirp-0.0.2/src/blackchirp/__init__.py
--rw-r--r--   0 kncrabtree  (1000) users      (100)     6775 2024-05-15 22:46:22.000000 blackchirp-0.0.2/src/blackchirp/bcfid.py
--rw-r--r--   0 kncrabtree  (1000) users      (100)     4716 2024-05-15 22:46:22.000000 blackchirp-0.0.2/src/blackchirp/bcftmw.py
--rw-r--r--   0 kncrabtree  (1000) users      (100)      394 2024-05-15 22:46:22.000000 blackchirp-0.0.2/src/blackchirp/bclif.py
--rw-r--r--   0 kncrabtree  (1000) users      (100)     2095 2024-05-15 22:45:27.000000 blackchirp-0.0.2/src/blackchirp/blackchirpexperiment.py
-drwxr-xr-x   0 kncrabtree  (1000) users      (100)        0 2024-05-16 00:30:53.599635 blackchirp-0.0.2/src/blackchirp.egg-info/
--rw-r--r--   0 kncrabtree  (1000) users      (100)      918 2024-05-16 00:30:53.000000 blackchirp-0.0.2/src/blackchirp.egg-info/PKG-INFO
--rw-r--r--   0 kncrabtree  (1000) users      (100)      360 2024-05-16 00:30:53.000000 blackchirp-0.0.2/src/blackchirp.egg-info/SOURCES.txt
--rw-r--r--   0 kncrabtree  (1000) users      (100)        1 2024-05-16 00:30:53.000000 blackchirp-0.0.2/src/blackchirp.egg-info/dependency_links.txt
--rw-r--r--   0 kncrabtree  (1000) users      (100)       19 2024-05-16 00:30:53.000000 blackchirp-0.0.2/src/blackchirp.egg-info/requires.txt
--rw-r--r--   0 kncrabtree  (1000) users      (100)       11 2024-05-16 00:30:53.000000 blackchirp-0.0.2/src/blackchirp.egg-info/top_level.txt
+drwxr-xr-x   0 kncrabtree  (1000) users      (100)        0 2024-05-17 23:16:56.892982 blackchirp-0.0.3/
+-rw-r--r--   0 kncrabtree  (1000) users      (100)     1069 2024-05-15 23:44:25.000000 blackchirp-0.0.3/LICENSE
+-rw-r--r--   0 kncrabtree  (1000) users      (100)      918 2024-05-17 23:16:56.892982 blackchirp-0.0.3/PKG-INFO
+-rw-r--r--   0 kncrabtree  (1000) users      (100)      451 2024-05-15 23:52:03.000000 blackchirp-0.0.3/README.md
+-rw-r--r--   0 kncrabtree  (1000) users      (100)      459 2024-05-17 23:14:05.000000 blackchirp-0.0.3/pyproject.toml
+-rw-r--r--   0 kncrabtree  (1000) users      (100)       38 2024-05-17 23:16:56.892982 blackchirp-0.0.3/setup.cfg
+drwxr-xr-x   0 kncrabtree  (1000) users      (100)        0 2024-05-17 23:16:56.889649 blackchirp-0.0.3/src/
+drwxr-xr-x   0 kncrabtree  (1000) users      (100)        0 2024-05-17 23:16:56.892982 blackchirp-0.0.3/src/blackchirp/
+-rw-r--r--   0 kncrabtree  (1000) users      (100)     1703 2024-05-16 21:28:30.000000 blackchirp-0.0.3/src/blackchirp/__init__.py
+-rw-r--r--   0 kncrabtree  (1000) users      (100)    11856 2024-05-17 23:08:17.000000 blackchirp-0.0.3/src/blackchirp/bcfid.py
+-rw-r--r--   0 kncrabtree  (1000) users      (100)     8641 2024-05-17 21:40:40.000000 blackchirp-0.0.3/src/blackchirp/bcftmw.py
+-rw-r--r--   0 kncrabtree  (1000) users      (100)      481 2024-05-16 21:41:01.000000 blackchirp-0.0.3/src/blackchirp/bclif.py
+-rw-r--r--   0 kncrabtree  (1000) users      (100)     9476 2024-05-17 23:08:15.000000 blackchirp-0.0.3/src/blackchirp/blackchirpexperiment.py
+drwxr-xr-x   0 kncrabtree  (1000) users      (100)        0 2024-05-17 23:16:56.892982 blackchirp-0.0.3/src/blackchirp.egg-info/
+-rw-r--r--   0 kncrabtree  (1000) users      (100)      918 2024-05-17 23:16:56.000000 blackchirp-0.0.3/src/blackchirp.egg-info/PKG-INFO
+-rw-r--r--   0 kncrabtree  (1000) users      (100)      360 2024-05-17 23:16:56.000000 blackchirp-0.0.3/src/blackchirp.egg-info/SOURCES.txt
+-rw-r--r--   0 kncrabtree  (1000) users      (100)        1 2024-05-17 23:16:56.000000 blackchirp-0.0.3/src/blackchirp.egg-info/dependency_links.txt
+-rw-r--r--   0 kncrabtree  (1000) users      (100)       19 2024-05-17 23:16:56.000000 blackchirp-0.0.3/src/blackchirp.egg-info/requires.txt
+-rw-r--r--   0 kncrabtree  (1000) users      (100)       11 2024-05-17 23:16:56.000000 blackchirp-0.0.3/src/blackchirp.egg-info/top_level.txt
```

### Comparing `blackchirp-0.0.2/LICENSE` & `blackchirp-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `blackchirp-0.0.2/PKG-INFO` & `blackchirp-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blackchirp
-Version: 0.0.2
+Version: 0.0.3
 Summary: Python module for blackchirp: data acquisition software for CP-FTMW spectroscopy
 Author-email: Kyle Crabtree <kncrabtree@ucdavis.edu>
 License: MIT License
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
```

### Comparing `blackchirp-0.0.2/src/blackchirp.egg-info/PKG-INFO` & `blackchirp-0.0.3/src/blackchirp.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blackchirp
-Version: 0.0.2
+Version: 0.0.3
 Summary: Python module for blackchirp: data acquisition software for CP-FTMW spectroscopy
 Author-email: Kyle Crabtree <kncrabtree@ucdavis.edu>
 License: MIT License
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
```

