# Comparing `tmp/neon-audio-1.5.2a5.tar.gz` & `tmp/neon-audio-1.5.2a6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neon-audio-1.5.2a5.tar", last modified: Wed May  8 22:07:34 2024, max compression
+gzip compressed data, was "neon-audio-1.5.2a6.tar", last modified: Fri May 17 23:23:05 2024, max compression
```

## Comparing `neon-audio-1.5.2a5.tar` & `neon-audio-1.5.2a6.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 22:07:34.946669 neon-audio-1.5.2a5/
--rw-r--r--   0 runner    (1001) docker     (127)     1634 2024-05-08 22:07:30.000000 neon-audio-1.5.2a5/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)     1695 2024-05-08 22:07:34.946669 neon-audio-1.5.2a5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1304 2024-05-08 22:07:30.000000 neon-audio-1.5.2a5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 22:07:34.946669 neon-audio-1.5.2a5/neon_audio/
--rw-r--r--   0 runner    (1001) docker     (127)     1831 2024-05-08 22:07:30.000000 neon-audio-1.5.2a5/neon_audio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3463 2024-05-08 22:07:30.000000 neon-audio-1.5.2a5/neon_audio/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5615 2024-05-08 22:07:30.000000 neon-audio-1.5.2a5/neon_audio/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     8556 2024-05-08 22:07:30.000000 neon-audio-1.5.2a5/neon_audio/service.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 22:07:34.946669 neon-audio-1.5.2a5/neon_audio/tts/
--rw-r--r--   0 runner    (1001) docker     (127)     3049 2024-05-08 22:07:30.000000 neon-audio-1.5.2a5/neon_audio/tts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    19086 2024-05-08 22:07:30.000000 neon-audio-1.5.2a5/neon_audio/tts/neon.py
--rw-r--r--   0 runner    (1001) docker     (127)     5166 2024-05-08 22:07:30.000000 neon-audio-1.5.2a5/neon_audio/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 22:07:34.946669 neon-audio-1.5.2a5/neon_audio.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1695 2024-05-08 22:07:34.000000 neon-audio-1.5.2a5/neon_audio.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      515 2024-05-08 22:07:34.000000 neon-audio-1.5.2a5/neon_audio.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 22:07:34.000000 neon-audio-1.5.2a5/neon_audio.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      123 2024-05-08 22:07:34.000000 neon-audio-1.5.2a5/neon_audio.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      454 2024-05-08 22:07:34.000000 neon-audio-1.5.2a5/neon_audio.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-08 22:07:34.000000 neon-audio-1.5.2a5/neon_audio.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 22:07:34.000000 neon-audio-1.5.2a5/neon_audio.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-08 22:07:34.946669 neon-audio-1.5.2a5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3987 2024-05-08 22:07:30.000000 neon-audio-1.5.2a5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 22:07:34.946669 neon-audio-1.5.2a5/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1831 2024-05-08 22:07:30.000000 neon-audio-1.5.2a5/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10747 2024-05-08 22:07:30.000000 neon-audio-1.5.2a5/tests/api_method_tests.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 22:07:34.946669 neon-audio-1.5.2a5/tests/test_objects/
--rw-r--r--   0 runner    (1001) docker     (127)     2562 2024-05-08 22:07:30.000000 neon-audio-1.5.2a5/tests/test_objects/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9846 2024-05-08 22:07:30.000000 neon-audio-1.5.2a5/tests/unit_tests.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 23:23:05.515546 neon-audio-1.5.2a6/
+-rw-r--r--   0 runner    (1001) docker     (127)     1634 2024-05-17 23:23:02.000000 neon-audio-1.5.2a6/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1695 2024-05-17 23:23:05.515546 neon-audio-1.5.2a6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1304 2024-05-17 23:23:02.000000 neon-audio-1.5.2a6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 23:23:05.511546 neon-audio-1.5.2a6/neon_audio/
+-rw-r--r--   0 runner    (1001) docker     (127)     1831 2024-05-17 23:23:02.000000 neon-audio-1.5.2a6/neon_audio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3463 2024-05-17 23:23:02.000000 neon-audio-1.5.2a6/neon_audio/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5615 2024-05-17 23:23:02.000000 neon-audio-1.5.2a6/neon_audio/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8556 2024-05-17 23:23:02.000000 neon-audio-1.5.2a6/neon_audio/service.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 23:23:05.515546 neon-audio-1.5.2a6/neon_audio/tts/
+-rw-r--r--   0 runner    (1001) docker     (127)     3049 2024-05-17 23:23:02.000000 neon-audio-1.5.2a6/neon_audio/tts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19086 2024-05-17 23:23:02.000000 neon-audio-1.5.2a6/neon_audio/tts/neon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5166 2024-05-17 23:23:02.000000 neon-audio-1.5.2a6/neon_audio/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 23:23:05.515546 neon-audio-1.5.2a6/neon_audio.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1695 2024-05-17 23:23:05.000000 neon-audio-1.5.2a6/neon_audio.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      515 2024-05-17 23:23:05.000000 neon-audio-1.5.2a6/neon_audio.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-17 23:23:05.000000 neon-audio-1.5.2a6/neon_audio.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-05-17 23:23:05.000000 neon-audio-1.5.2a6/neon_audio.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      465 2024-05-17 23:23:05.000000 neon-audio-1.5.2a6/neon_audio.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-17 23:23:05.000000 neon-audio-1.5.2a6/neon_audio.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-17 23:23:05.000000 neon-audio-1.5.2a6/neon_audio.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-17 23:23:05.515546 neon-audio-1.5.2a6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3987 2024-05-17 23:23:02.000000 neon-audio-1.5.2a6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 23:23:05.515546 neon-audio-1.5.2a6/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1831 2024-05-17 23:23:02.000000 neon-audio-1.5.2a6/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10747 2024-05-17 23:23:02.000000 neon-audio-1.5.2a6/tests/api_method_tests.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 23:23:05.515546 neon-audio-1.5.2a6/tests/test_objects/
+-rw-r--r--   0 runner    (1001) docker     (127)     2562 2024-05-17 23:23:02.000000 neon-audio-1.5.2a6/tests/test_objects/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9846 2024-05-17 23:23:02.000000 neon-audio-1.5.2a6/tests/unit_tests.py
```

### Comparing `neon-audio-1.5.2a5/LICENSE.md` & `neon-audio-1.5.2a6/LICENSE.md`

 * *Files identical despite different names*

### Comparing `neon-audio-1.5.2a5/PKG-INFO` & `neon-audio-1.5.2a6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neon-audio
-Version: 1.5.2a5
+Version: 1.5.2a6
 Summary: Neon Audio Module
 Home-page: https://github.com/NeonGeckoCom/neon_audio
 Author: Neongecko
 Author-email: developers@neon.ai
 License: BSD-3-Clause
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `neon-audio-1.5.2a5/README.md` & `neon-audio-1.5.2a6/README.md`

 * *Files identical despite different names*

### Comparing `neon-audio-1.5.2a5/neon_audio/__init__.py` & `neon-audio-1.5.2a6/neon_audio/__init__.py`

 * *Files identical despite different names*

### Comparing `neon-audio-1.5.2a5/neon_audio/__main__.py` & `neon-audio-1.5.2a6/neon_audio/__main__.py`

 * *Files identical despite different names*

### Comparing `neon-audio-1.5.2a5/neon_audio/cli.py` & `neon-audio-1.5.2a6/neon_audio/cli.py`

 * *Files identical despite different names*

### Comparing `neon-audio-1.5.2a5/neon_audio/service.py` & `neon-audio-1.5.2a6/neon_audio/service.py`

 * *Files identical despite different names*

### Comparing `neon-audio-1.5.2a5/neon_audio/tts/__init__.py` & `neon-audio-1.5.2a6/neon_audio/tts/__init__.py`

 * *Files identical despite different names*

### Comparing `neon-audio-1.5.2a5/neon_audio/tts/neon.py` & `neon-audio-1.5.2a6/neon_audio/tts/neon.py`

 * *Files identical despite different names*

### Comparing `neon-audio-1.5.2a5/neon_audio/utils.py` & `neon-audio-1.5.2a6/neon_audio/utils.py`

 * *Files identical despite different names*

### Comparing `neon-audio-1.5.2a5/neon_audio.egg-info/PKG-INFO` & `neon-audio-1.5.2a6/neon_audio.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neon-audio
-Version: 1.5.2a5
+Version: 1.5.2a6
 Summary: Neon Audio Module
 Home-page: https://github.com/NeonGeckoCom/neon_audio
 Author: Neongecko
 Author-email: developers@neon.ai
 License: BSD-3-Clause
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `neon-audio-1.5.2a5/neon_audio.egg-info/SOURCES.txt` & `neon-audio-1.5.2a6/neon_audio.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `neon-audio-1.5.2a5/setup.py` & `neon-audio-1.5.2a6/setup.py`

 * *Files identical despite different names*

### Comparing `neon-audio-1.5.2a5/tests/__init__.py` & `neon-audio-1.5.2a6/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `neon-audio-1.5.2a5/tests/api_method_tests.py` & `neon-audio-1.5.2a6/tests/api_method_tests.py`

 * *Files identical despite different names*

### Comparing `neon-audio-1.5.2a5/tests/test_objects/__init__.py` & `neon-audio-1.5.2a6/tests/test_objects/__init__.py`

 * *Files identical despite different names*

### Comparing `neon-audio-1.5.2a5/tests/unit_tests.py` & `neon-audio-1.5.2a6/tests/unit_tests.py`

 * *Files identical despite different names*

