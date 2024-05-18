# Comparing `tmp/harm-analysis-1.1.1.tar.gz` & `tmp/harm_analysis-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "harm-analysis-1.1.1.tar", last modified: Mon Feb  5 13:17:01 2024, max compression
+gzip compressed data, was "harm_analysis-1.1.2.tar", last modified: Sat May 18 19:01:01 2024, max compression
```

## Comparing `harm-analysis-1.1.1.tar` & `harm_analysis-1.1.2.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 emacedo    (503) staff       (20)        0 2024-02-05 13:17:01.609514 harm-analysis-1.1.1/
--rw-r--r--   0 emacedo    (503) staff       (20)     3078 2023-12-28 15:35:10.000000 harm-analysis-1.1.1/.gitignore
--rw-r--r--   0 emacedo    (503) staff       (20)      825 2024-02-03 00:41:34.000000 harm-analysis-1.1.1/.readthedocs.yaml
--rw-r--r--   0 emacedo    (503) staff       (20)     2222 2024-02-05 13:17:01.609221 harm-analysis-1.1.1/PKG-INFO
--rw-r--r--   0 emacedo    (503) staff       (20)     1703 2024-02-03 11:55:53.000000 harm-analysis-1.1.1/README.rst
-drwxr-xr-x   0 emacedo    (503) staff       (20)        0 2024-02-05 13:17:01.604206 harm-analysis-1.1.1/docs/
--rw-r--r--   0 emacedo    (503) staff       (20)      638 2023-12-28 16:46:46.000000 harm-analysis-1.1.1/docs/Makefile
--rw-r--r--   0 emacedo    (503) staff       (20)    51951 2023-12-29 13:29:34.000000 harm-analysis-1.1.1/docs/harm_analysis_out_example.png
--rw-r--r--   0 emacedo    (503) staff       (20)      804 2023-12-28 16:46:46.000000 harm-analysis-1.1.1/docs/make.bat
--rw-r--r--   0 emacedo    (503) staff       (20)      666 2024-02-03 00:48:44.000000 harm-analysis-1.1.1/docs/requirements.txt
-drwxr-xr-x   0 emacedo    (503) staff       (20)        0 2024-02-05 13:17:01.604893 harm-analysis-1.1.1/docs/source/
--rw-r--r--   0 emacedo    (503) staff       (20)     1409 2024-02-03 00:00:39.000000 harm-analysis-1.1.1/docs/source/conf.py
--rw-r--r--   0 emacedo    (503) staff       (20)      123 2024-02-03 00:12:34.000000 harm-analysis-1.1.1/docs/source/harm_analysis.rst
--rw-r--r--   0 emacedo    (503) staff       (20)     2832 2024-02-05 13:14:05.000000 harm-analysis-1.1.1/docs/source/index.rst
-drwxr-xr-x   0 emacedo    (503) staff       (20)        0 2024-02-05 13:17:01.600916 harm-analysis-1.1.1/docs/source/tutorial/
-drwxr-xr-x   0 emacedo    (503) staff       (20)        0 2024-02-05 13:17:01.605420 harm-analysis-1.1.1/docs/source/tutorial/examples/
--rw-r--r--   0 emacedo    (503) staff       (20)      747 2024-02-05 11:53:25.000000 harm-analysis-1.1.1/docs/source/tutorial/examples/run_harm_analysis.py
--rw-r--r--   0 emacedo    (503) staff       (20)      736 2024-02-05 11:55:17.000000 harm-analysis-1.1.1/docs/source/tutorial/examples/run_shaped_noise_example.py
-drwxr-xr-x   0 emacedo    (503) staff       (20)        0 2024-02-05 13:17:01.606057 harm-analysis-1.1.1/harm_analysis/
--rw-r--r--   0 emacedo    (503) staff       (20)       30 2023-12-28 15:35:10.000000 harm-analysis-1.1.1/harm_analysis/__init__.py
--rw-r--r--   0 emacedo    (503) staff       (20)    18140 2024-02-05 13:16:02.000000 harm-analysis-1.1.1/harm_analysis/_harm_analysis.py
--rw-r--r--   0 emacedo    (503) staff       (20)     1562 2024-01-09 11:16:43.000000 harm-analysis-1.1.1/harm_analysis/cli.py
-drwxr-xr-x   0 emacedo    (503) staff       (20)        0 2024-02-05 13:17:01.608872 harm-analysis-1.1.1/harm_analysis.egg-info/
--rw-r--r--   0 emacedo    (503) staff       (20)     2222 2024-02-05 13:17:01.000000 harm-analysis-1.1.1/harm_analysis.egg-info/PKG-INFO
--rw-r--r--   0 emacedo    (503) staff       (20)      758 2024-02-05 13:17:01.000000 harm-analysis-1.1.1/harm_analysis.egg-info/SOURCES.txt
--rw-r--r--   0 emacedo    (503) staff       (20)        1 2024-02-05 13:17:01.000000 harm-analysis-1.1.1/harm_analysis.egg-info/dependency_links.txt
--rw-r--r--   0 emacedo    (503) staff       (20)       56 2024-02-05 13:17:01.000000 harm-analysis-1.1.1/harm_analysis.egg-info/entry_points.txt
--rw-r--r--   0 emacedo    (503) staff       (20)       29 2024-02-05 13:17:01.000000 harm-analysis-1.1.1/harm_analysis.egg-info/requires.txt
--rw-r--r--   0 emacedo    (503) staff       (20)       14 2024-02-05 13:17:01.000000 harm-analysis-1.1.1/harm_analysis.egg-info/top_level.txt
--rw-r--r--   0 emacedo    (503) staff       (20)      951 2024-02-03 11:53:09.000000 harm-analysis-1.1.1/pyproject.toml
--rw-r--r--   0 emacedo    (503) staff       (20)       59 2024-01-30 19:44:54.000000 harm-analysis-1.1.1/requirents.txt
--rw-r--r--   0 emacedo    (503) staff       (20)       38 2024-02-05 13:17:01.609576 harm-analysis-1.1.1/setup.cfg
-drwxr-xr-x   0 emacedo    (503) staff       (20)        0 2024-02-05 13:17:01.608359 harm-analysis-1.1.1/tests/
--rw-r--r--   0 emacedo    (503) staff       (20)        0 2023-12-28 15:35:10.000000 harm-analysis-1.1.1/tests/__init__.py
--rw-r--r--   0 emacedo    (503) staff       (20)     1020 2024-01-08 12:15:43.000000 harm-analysis-1.1.1/tests/test_cli.py
--rw-r--r--   0 emacedo    (503) staff       (20)    52180 2024-01-08 14:39:26.000000 harm-analysis-1.1.1/tests/test_data_cli.txt
--rw-r--r--   0 emacedo    (503) staff       (20)     7833 2024-02-05 11:41:44.000000 harm-analysis-1.1.1/tests/test_harm_analysis.py
--rw-r--r--   0 emacedo    (503) staff       (20)     1020 2024-01-08 12:15:56.000000 harm-analysis-1.1.1/tests/test_harm_analysis_cli.py
+drwxr-xr-x   0 emacedo    (503) staff       (20)        0 2024-05-18 19:01:01.903485 harm_analysis-1.1.2/
+-rw-r--r--   0 emacedo    (503) staff       (20)     3078 2023-12-28 15:35:10.000000 harm_analysis-1.1.2/.gitignore
+-rw-r--r--   0 emacedo    (503) staff       (20)      825 2024-02-03 00:41:34.000000 harm_analysis-1.1.2/.readthedocs.yaml
+-rw-r--r--   0 emacedo    (503) staff       (20)     2227 2024-05-18 19:01:01.903137 harm_analysis-1.1.2/PKG-INFO
+-rw-r--r--   0 emacedo    (503) staff       (20)     1703 2024-02-03 11:55:53.000000 harm_analysis-1.1.2/README.rst
+drwxr-xr-x   0 emacedo    (503) staff       (20)        0 2024-05-18 19:01:01.898274 harm_analysis-1.1.2/docs/
+-rw-r--r--   0 emacedo    (503) staff       (20)      638 2023-12-28 16:46:46.000000 harm_analysis-1.1.2/docs/Makefile
+-rw-r--r--   0 emacedo    (503) staff       (20)    51951 2023-12-29 13:29:34.000000 harm_analysis-1.1.2/docs/harm_analysis_out_example.png
+-rw-r--r--   0 emacedo    (503) staff       (20)      804 2023-12-28 16:46:46.000000 harm_analysis-1.1.2/docs/make.bat
+-rw-r--r--   0 emacedo    (503) staff       (20)      666 2024-02-03 00:48:44.000000 harm_analysis-1.1.2/docs/requirements.txt
+drwxr-xr-x   0 emacedo    (503) staff       (20)        0 2024-05-18 19:01:01.898745 harm_analysis-1.1.2/docs/source/
+-rw-r--r--   0 emacedo    (503) staff       (20)     1409 2024-02-03 00:00:39.000000 harm_analysis-1.1.2/docs/source/conf.py
+-rw-r--r--   0 emacedo    (503) staff       (20)      123 2024-02-03 00:12:34.000000 harm_analysis-1.1.2/docs/source/harm_analysis.rst
+-rw-r--r--   0 emacedo    (503) staff       (20)     2832 2024-02-05 13:14:05.000000 harm_analysis-1.1.2/docs/source/index.rst
+drwxr-xr-x   0 emacedo    (503) staff       (20)        0 2024-05-18 19:01:01.896460 harm_analysis-1.1.2/docs/source/tutorial/
+drwxr-xr-x   0 emacedo    (503) staff       (20)        0 2024-05-18 19:01:01.899335 harm_analysis-1.1.2/docs/source/tutorial/examples/
+-rw-r--r--   0 emacedo    (503) staff       (20)      747 2024-02-05 11:53:25.000000 harm_analysis-1.1.2/docs/source/tutorial/examples/run_harm_analysis.py
+-rw-r--r--   0 emacedo    (503) staff       (20)      736 2024-02-05 11:55:17.000000 harm_analysis-1.1.2/docs/source/tutorial/examples/run_shaped_noise_example.py
+drwxr-xr-x   0 emacedo    (503) staff       (20)        0 2024-05-18 19:01:01.899992 harm_analysis-1.1.2/harm_analysis/
+-rw-r--r--   0 emacedo    (503) staff       (20)       30 2023-12-28 15:35:10.000000 harm_analysis-1.1.2/harm_analysis/__init__.py
+-rw-r--r--   0 emacedo    (503) staff       (20)    18140 2024-02-05 13:16:02.000000 harm_analysis-1.1.2/harm_analysis/_harm_analysis.py
+-rw-r--r--   0 emacedo    (503) staff       (20)     1562 2024-01-09 11:16:43.000000 harm_analysis-1.1.2/harm_analysis/cli.py
+drwxr-xr-x   0 emacedo    (503) staff       (20)        0 2024-05-18 19:01:01.902663 harm_analysis-1.1.2/harm_analysis.egg-info/
+-rw-r--r--   0 emacedo    (503) staff       (20)     2227 2024-05-18 19:01:01.000000 harm_analysis-1.1.2/harm_analysis.egg-info/PKG-INFO
+-rw-r--r--   0 emacedo    (503) staff       (20)      758 2024-05-18 19:01:01.000000 harm_analysis-1.1.2/harm_analysis.egg-info/SOURCES.txt
+-rw-r--r--   0 emacedo    (503) staff       (20)        1 2024-05-18 19:01:01.000000 harm_analysis-1.1.2/harm_analysis.egg-info/dependency_links.txt
+-rw-r--r--   0 emacedo    (503) staff       (20)       56 2024-05-18 19:01:01.000000 harm_analysis-1.1.2/harm_analysis.egg-info/entry_points.txt
+-rw-r--r--   0 emacedo    (503) staff       (20)       29 2024-05-18 19:01:01.000000 harm_analysis-1.1.2/harm_analysis.egg-info/requires.txt
+-rw-r--r--   0 emacedo    (503) staff       (20)       14 2024-05-18 19:01:01.000000 harm_analysis-1.1.2/harm_analysis.egg-info/top_level.txt
+-rw-r--r--   0 emacedo    (503) staff       (20)      956 2024-05-18 18:51:06.000000 harm_analysis-1.1.2/pyproject.toml
+-rw-r--r--   0 emacedo    (503) staff       (20)       59 2024-01-30 19:44:54.000000 harm_analysis-1.1.2/requirents.txt
+-rw-r--r--   0 emacedo    (503) staff       (20)       38 2024-05-18 19:01:01.903546 harm_analysis-1.1.2/setup.cfg
+drwxr-xr-x   0 emacedo    (503) staff       (20)        0 2024-05-18 19:01:01.902333 harm_analysis-1.1.2/tests/
+-rw-r--r--   0 emacedo    (503) staff       (20)        0 2023-12-28 15:35:10.000000 harm_analysis-1.1.2/tests/__init__.py
+-rw-r--r--   0 emacedo    (503) staff       (20)     1020 2024-01-08 12:15:43.000000 harm_analysis-1.1.2/tests/test_cli.py
+-rw-r--r--   0 emacedo    (503) staff       (20)    52180 2024-01-08 14:39:26.000000 harm_analysis-1.1.2/tests/test_data_cli.txt
+-rw-r--r--   0 emacedo    (503) staff       (20)     7833 2024-02-05 11:41:44.000000 harm_analysis-1.1.2/tests/test_harm_analysis.py
+-rw-r--r--   0 emacedo    (503) staff       (20)     1020 2024-01-08 12:15:56.000000 harm_analysis-1.1.2/tests/test_harm_analysis_cli.py
```

### Comparing `harm-analysis-1.1.1/.gitignore` & `harm_analysis-1.1.2/.gitignore`

 * *Files identical despite different names*

### Comparing `harm-analysis-1.1.1/.readthedocs.yaml` & `harm_analysis-1.1.2/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `harm-analysis-1.1.1/PKG-INFO` & `harm_analysis-1.1.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: harm-analysis
-Version: 1.1.1
-Summary: A Python library for Q format representation and overflow handling.
+Version: 1.1.2
+Summary: A Python library to estimate parameters from a signal containing a tone.
 Author-email: Eric Macedo <ericsmacedo@gmail.com>
 License: MIT
 Project-URL: Documentation, https://harm-analysis.readthedocs.io/en/latest/
 Project-URL: Source Code, https://github.com/ericsmacedo/harm_analysis
 Keywords: DSP,Fixed-point,Signal-Processing,SNR
 Description-Content-Type: text/x-rst
 Requires-Dist: matplotlib
```

### Comparing `harm-analysis-1.1.1/README.rst` & `harm_analysis-1.1.2/README.rst`

 * *Files identical despite different names*

### Comparing `harm-analysis-1.1.1/docs/Makefile` & `harm_analysis-1.1.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `harm-analysis-1.1.1/docs/harm_analysis_out_example.png` & `harm_analysis-1.1.2/docs/harm_analysis_out_example.png`

 * *Files identical despite different names*

### Comparing `harm-analysis-1.1.1/docs/make.bat` & `harm_analysis-1.1.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `harm-analysis-1.1.1/docs/requirements.txt` & `harm_analysis-1.1.2/docs/requirements.txt`

 * *Files identical despite different names*

### Comparing `harm-analysis-1.1.1/docs/source/conf.py` & `harm_analysis-1.1.2/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `harm-analysis-1.1.1/docs/source/index.rst` & `harm_analysis-1.1.2/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `harm-analysis-1.1.1/docs/source/tutorial/examples/run_harm_analysis.py` & `harm_analysis-1.1.2/docs/source/tutorial/examples/run_harm_analysis.py`

 * *Files identical despite different names*

### Comparing `harm-analysis-1.1.1/docs/source/tutorial/examples/run_shaped_noise_example.py` & `harm_analysis-1.1.2/docs/source/tutorial/examples/run_shaped_noise_example.py`

 * *Files identical despite different names*

### Comparing `harm-analysis-1.1.1/harm_analysis/_harm_analysis.py` & `harm_analysis-1.1.2/harm_analysis/_harm_analysis.py`

 * *Files identical despite different names*

### Comparing `harm-analysis-1.1.1/harm_analysis/cli.py` & `harm_analysis-1.1.2/harm_analysis/cli.py`

 * *Files identical despite different names*

### Comparing `harm-analysis-1.1.1/harm_analysis.egg-info/PKG-INFO` & `harm_analysis-1.1.2/harm_analysis.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: harm-analysis
-Version: 1.1.1
-Summary: A Python library for Q format representation and overflow handling.
+Version: 1.1.2
+Summary: A Python library to estimate parameters from a signal containing a tone.
 Author-email: Eric Macedo <ericsmacedo@gmail.com>
 License: MIT
 Project-URL: Documentation, https://harm-analysis.readthedocs.io/en/latest/
 Project-URL: Source Code, https://github.com/ericsmacedo/harm_analysis
 Keywords: DSP,Fixed-point,Signal-Processing,SNR
 Description-Content-Type: text/x-rst
 Requires-Dist: matplotlib
```

### Comparing `harm-analysis-1.1.1/harm_analysis.egg-info/SOURCES.txt` & `harm_analysis-1.1.2/harm_analysis.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `harm-analysis-1.1.1/pyproject.toml` & `harm_analysis-1.1.2/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "harm-analysis"
 authors = [
     {name = 'Eric Macedo', email = 'ericsmacedo@gmail.com'}
 ]
-description = 'A Python library for Q format representation and overflow handling.'
+description = 'A Python library to estimate parameters from a signal containing a tone.'
 dynamic = ["version"] # This in conjunction with setuptools_scm, will generate the 
                       # versions dynamically
 readme = "README.rst"
 keywords = ["DSP", "Fixed-point", "Signal-Processing", "SNR"]
 license = {text = "MIT"}
 dependencies = [
     "matplotlib",
```

### Comparing `harm-analysis-1.1.1/tests/test_cli.py` & `harm_analysis-1.1.2/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `harm-analysis-1.1.1/tests/test_data_cli.txt` & `harm_analysis-1.1.2/tests/test_data_cli.txt`

 * *Files identical despite different names*

### Comparing `harm-analysis-1.1.1/tests/test_harm_analysis.py` & `harm_analysis-1.1.2/tests/test_harm_analysis.py`

 * *Files identical despite different names*

### Comparing `harm-analysis-1.1.1/tests/test_harm_analysis_cli.py` & `harm_analysis-1.1.2/tests/test_harm_analysis_cli.py`

 * *Files identical despite different names*

