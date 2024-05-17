# Comparing `tmp/expyre_wfl-0.1.3.tar.gz` & `tmp/expyre_wfl-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "expyre_wfl-0.1.3.tar", last modified: Thu May 16 18:11:51 2024, max compression
+gzip compressed data, was "expyre_wfl-0.1.4.tar", last modified: Fri May 17 22:13:31 2024, max compression
```

## Comparing `expyre_wfl-0.1.3.tar` & `expyre_wfl-0.1.4.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 18:11:51.555604 expyre_wfl-0.1.3/
--rw-r--r--   0 runner    (1001) docker     (127)    18092 2024-05-16 18:11:48.000000 expyre_wfl-0.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      793 2024-05-16 18:11:51.555604 expyre_wfl-0.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      650 2024-05-16 18:11:48.000000 expyre_wfl-0.1.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 18:11:51.547604 expyre_wfl-0.1.3/expyre/
--rw-r--r--   0 runner    (1001) docker     (127)       93 2024-05-16 18:11:48.000000 expyre_wfl-0.1.3/expyre/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 18:11:51.551604 expyre_wfl-0.1.3/expyre/cli/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 18:11:48.000000 expyre_wfl-0.1.3/expyre/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10585 2024-05-16 18:11:48.000000 expyre_wfl-0.1.3/expyre/cli/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     5123 2024-05-16 18:11:48.000000 expyre_wfl-0.1.3/expyre/config.py
--rw-r--r--   0 runner    (1001) docker     (127)    37501 2024-05-16 18:11:48.000000 expyre_wfl-0.1.3/expyre/func.py
--rw-r--r--   0 runner    (1001) docker     (127)     9177 2024-05-16 18:11:48.000000 expyre_wfl-0.1.3/expyre/jobsdb.py
--rw-r--r--   0 runner    (1001) docker     (127)     7243 2024-05-16 18:11:48.000000 expyre_wfl-0.1.3/expyre/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 18:11:51.551604 expyre_wfl-0.1.3/expyre/schedulers/
--rw-r--r--   0 runner    (1001) docker     (127)      250 2024-05-16 18:11:48.000000 expyre_wfl-0.1.3/expyre/schedulers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3311 2024-05-16 18:11:48.000000 expyre_wfl-0.1.3/expyre/schedulers/base.py
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-16 18:11:48.000000 expyre_wfl-0.1.3/expyre/schedulers/local.py
--rw-r--r--   0 runner    (1001) docker     (127)     7568 2024-05-16 18:11:48.000000 expyre_wfl-0.1.3/expyre/schedulers/pbs.py
--rw-r--r--   0 runner    (1001) docker     (127)     6468 2024-05-16 18:11:48.000000 expyre_wfl-0.1.3/expyre/schedulers/sge.py
--rw-r--r--   0 runner    (1001) docker     (127)     7018 2024-05-16 18:11:48.000000 expyre_wfl-0.1.3/expyre/schedulers/slurm.py
--rw-r--r--   0 runner    (1001) docker     (127)    10095 2024-05-16 18:11:48.000000 expyre_wfl-0.1.3/expyre/subprocess.py
--rw-r--r--   0 runner    (1001) docker     (127)    11372 2024-05-16 18:11:48.000000 expyre_wfl-0.1.3/expyre/system.py
--rw-r--r--   0 runner    (1001) docker     (127)     2163 2024-05-16 18:11:48.000000 expyre_wfl-0.1.3/expyre/units.py
--rw-r--r--   0 runner    (1001) docker     (127)      334 2024-05-16 18:11:48.000000 expyre_wfl-0.1.3/expyre/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 18:11:51.551604 expyre_wfl-0.1.3/expyre_wfl.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      793 2024-05-16 18:11:51.000000 expyre_wfl-0.1.3/expyre_wfl.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      820 2024-05-16 18:11:51.000000 expyre_wfl-0.1.3/expyre_wfl.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 18:11:51.000000 expyre_wfl-0.1.3/expyre_wfl.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-16 18:11:51.000000 expyre_wfl-0.1.3/expyre_wfl.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-16 18:11:51.000000 expyre_wfl-0.1.3/expyre_wfl.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-16 18:11:51.000000 expyre_wfl-0.1.3/expyre_wfl.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-16 18:11:51.555604 expyre_wfl-0.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      354 2024-05-16 18:11:48.000000 expyre_wfl-0.1.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 18:11:51.551604 expyre_wfl-0.1.3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     3690 2024-05-16 18:11:48.000000 expyre_wfl-0.1.3/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1789 2024-05-16 18:11:48.000000 expyre_wfl-0.1.3/tests/test_failures.py
--rw-r--r--   0 runner    (1001) docker     (127)    10322 2024-05-16 18:11:48.000000 expyre_wfl-0.1.3/tests/test_func.py
--rw-r--r--   0 runner    (1001) docker     (127)     3456 2024-05-16 18:11:48.000000 expyre_wfl-0.1.3/tests/test_jobsdb.py
--rw-r--r--   0 runner    (1001) docker     (127)      663 2024-05-16 18:11:48.000000 expyre_wfl-0.1.3/tests/test_remote_exception.py
--rw-r--r--   0 runner    (1001) docker     (127)     7640 2024-05-16 18:11:48.000000 expyre_wfl-0.1.3/tests/test_resources.py
--rw-r--r--   0 runner    (1001) docker     (127)     6392 2024-05-16 18:11:48.000000 expyre_wfl-0.1.3/tests/test_schedulers.py
--rw-r--r--   0 runner    (1001) docker     (127)     6428 2024-05-16 18:11:48.000000 expyre_wfl-0.1.3/tests/test_subprocess.py
--rw-r--r--   0 runner    (1001) docker     (127)     1811 2024-05-16 18:11:48.000000 expyre_wfl-0.1.3/tests/test_system.py
--rw-r--r--   0 runner    (1001) docker     (127)      919 2024-05-16 18:11:48.000000 expyre_wfl-0.1.3/tests/test_units.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 22:13:31.069098 expyre_wfl-0.1.4/
+-rw-r--r--   0 runner    (1001) docker     (127)    18092 2024-05-17 22:13:20.000000 expyre_wfl-0.1.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      793 2024-05-17 22:13:31.069098 expyre_wfl-0.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      650 2024-05-17 22:13:20.000000 expyre_wfl-0.1.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 22:13:31.061098 expyre_wfl-0.1.4/expyre/
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-05-17 22:13:20.000000 expyre_wfl-0.1.4/expyre/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 22:13:31.065098 expyre_wfl-0.1.4/expyre/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 22:13:20.000000 expyre_wfl-0.1.4/expyre/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10585 2024-05-17 22:13:20.000000 expyre_wfl-0.1.4/expyre/cli/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5123 2024-05-17 22:13:20.000000 expyre_wfl-0.1.4/expyre/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37501 2024-05-17 22:13:20.000000 expyre_wfl-0.1.4/expyre/func.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9177 2024-05-17 22:13:20.000000 expyre_wfl-0.1.4/expyre/jobsdb.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7243 2024-05-17 22:13:20.000000 expyre_wfl-0.1.4/expyre/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 22:13:31.065098 expyre_wfl-0.1.4/expyre/schedulers/
+-rw-r--r--   0 runner    (1001) docker     (127)      250 2024-05-17 22:13:20.000000 expyre_wfl-0.1.4/expyre/schedulers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3311 2024-05-17 22:13:20.000000 expyre_wfl-0.1.4/expyre/schedulers/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-17 22:13:20.000000 expyre_wfl-0.1.4/expyre/schedulers/local.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7568 2024-05-17 22:13:20.000000 expyre_wfl-0.1.4/expyre/schedulers/pbs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6468 2024-05-17 22:13:20.000000 expyre_wfl-0.1.4/expyre/schedulers/sge.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7018 2024-05-17 22:13:20.000000 expyre_wfl-0.1.4/expyre/schedulers/slurm.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10095 2024-05-17 22:13:20.000000 expyre_wfl-0.1.4/expyre/subprocess.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11372 2024-05-17 22:13:20.000000 expyre_wfl-0.1.4/expyre/system.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2163 2024-05-17 22:13:20.000000 expyre_wfl-0.1.4/expyre/units.py
+-rw-r--r--   0 runner    (1001) docker     (127)      334 2024-05-17 22:13:20.000000 expyre_wfl-0.1.4/expyre/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 22:13:31.069098 expyre_wfl-0.1.4/expyre_wfl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      793 2024-05-17 22:13:31.000000 expyre_wfl-0.1.4/expyre_wfl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      820 2024-05-17 22:13:31.000000 expyre_wfl-0.1.4/expyre_wfl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-17 22:13:31.000000 expyre_wfl-0.1.4/expyre_wfl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-17 22:13:31.000000 expyre_wfl-0.1.4/expyre_wfl.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-17 22:13:31.000000 expyre_wfl-0.1.4/expyre_wfl.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-17 22:13:31.000000 expyre_wfl-0.1.4/expyre_wfl.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-17 22:13:31.069098 expyre_wfl-0.1.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      385 2024-05-17 22:13:20.000000 expyre_wfl-0.1.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 22:13:31.065098 expyre_wfl-0.1.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     3690 2024-05-17 22:13:20.000000 expyre_wfl-0.1.4/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1789 2024-05-17 22:13:20.000000 expyre_wfl-0.1.4/tests/test_failures.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10322 2024-05-17 22:13:20.000000 expyre_wfl-0.1.4/tests/test_func.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3456 2024-05-17 22:13:20.000000 expyre_wfl-0.1.4/tests/test_jobsdb.py
+-rw-r--r--   0 runner    (1001) docker     (127)      663 2024-05-17 22:13:20.000000 expyre_wfl-0.1.4/tests/test_remote_exception.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7640 2024-05-17 22:13:20.000000 expyre_wfl-0.1.4/tests/test_resources.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6392 2024-05-17 22:13:20.000000 expyre_wfl-0.1.4/tests/test_schedulers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6428 2024-05-17 22:13:20.000000 expyre_wfl-0.1.4/tests/test_subprocess.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1811 2024-05-17 22:13:20.000000 expyre_wfl-0.1.4/tests/test_system.py
+-rw-r--r--   0 runner    (1001) docker     (127)      919 2024-05-17 22:13:20.000000 expyre_wfl-0.1.4/tests/test_units.py
```

### Comparing `expyre_wfl-0.1.3/LICENSE` & `expyre_wfl-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `expyre_wfl-0.1.3/PKG-INFO` & `expyre_wfl-0.1.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: expyre-wfl
-Version: 0.1.3
+Version: 0.1.4
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: click>=7.0
 
 ## Overview
 
 ExPyRe (EXecute PYthon REmotely) is a package for evaluating a python function via a queuing system (e.g. Sun Grid Engine, PBS or Slurm), and return the output. The only restriction is that the function needs to be pickleable.
```

### Comparing `expyre_wfl-0.1.3/README.md` & `expyre_wfl-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `expyre_wfl-0.1.3/expyre/cli/cli.py` & `expyre_wfl-0.1.4/expyre/cli/cli.py`

 * *Files identical despite different names*

### Comparing `expyre_wfl-0.1.3/expyre/config.py` & `expyre_wfl-0.1.4/expyre/config.py`

 * *Files identical despite different names*

### Comparing `expyre_wfl-0.1.3/expyre/func.py` & `expyre_wfl-0.1.4/expyre/func.py`

 * *Files identical despite different names*

### Comparing `expyre_wfl-0.1.3/expyre/jobsdb.py` & `expyre_wfl-0.1.4/expyre/jobsdb.py`

 * *Files identical despite different names*

### Comparing `expyre_wfl-0.1.3/expyre/resources.py` & `expyre_wfl-0.1.4/expyre/resources.py`

 * *Files identical despite different names*

### Comparing `expyre_wfl-0.1.3/expyre/schedulers/base.py` & `expyre_wfl-0.1.4/expyre/schedulers/base.py`

 * *Files identical despite different names*

### Comparing `expyre_wfl-0.1.3/expyre/schedulers/pbs.py` & `expyre_wfl-0.1.4/expyre/schedulers/pbs.py`

 * *Files identical despite different names*

### Comparing `expyre_wfl-0.1.3/expyre/schedulers/sge.py` & `expyre_wfl-0.1.4/expyre/schedulers/sge.py`

 * *Files identical despite different names*

### Comparing `expyre_wfl-0.1.3/expyre/schedulers/slurm.py` & `expyre_wfl-0.1.4/expyre/schedulers/slurm.py`

 * *Files identical despite different names*

### Comparing `expyre_wfl-0.1.3/expyre/subprocess.py` & `expyre_wfl-0.1.4/expyre/subprocess.py`

 * *Files identical despite different names*

### Comparing `expyre_wfl-0.1.3/expyre/system.py` & `expyre_wfl-0.1.4/expyre/system.py`

 * *Files identical despite different names*

### Comparing `expyre_wfl-0.1.3/expyre/units.py` & `expyre_wfl-0.1.4/expyre/units.py`

 * *Files identical despite different names*

### Comparing `expyre_wfl-0.1.3/expyre_wfl.egg-info/PKG-INFO` & `expyre_wfl-0.1.4/expyre_wfl.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: expyre-wfl
-Version: 0.1.3
+Version: 0.1.4
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: click>=7.0
 
 ## Overview
 
 ExPyRe (EXecute PYthon REmotely) is a package for evaluating a python function via a queuing system (e.g. Sun Grid Engine, PBS or Slurm), and return the output. The only restriction is that the function needs to be pickleable.
```

### Comparing `expyre_wfl-0.1.3/expyre_wfl.egg-info/SOURCES.txt` & `expyre_wfl-0.1.4/expyre_wfl.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `expyre_wfl-0.1.3/tests/test_config.py` & `expyre_wfl-0.1.4/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `expyre_wfl-0.1.3/tests/test_failures.py` & `expyre_wfl-0.1.4/tests/test_failures.py`

 * *Files identical despite different names*

### Comparing `expyre_wfl-0.1.3/tests/test_func.py` & `expyre_wfl-0.1.4/tests/test_func.py`

 * *Files identical despite different names*

### Comparing `expyre_wfl-0.1.3/tests/test_jobsdb.py` & `expyre_wfl-0.1.4/tests/test_jobsdb.py`

 * *Files identical despite different names*

### Comparing `expyre_wfl-0.1.3/tests/test_remote_exception.py` & `expyre_wfl-0.1.4/tests/test_remote_exception.py`

 * *Files identical despite different names*

### Comparing `expyre_wfl-0.1.3/tests/test_resources.py` & `expyre_wfl-0.1.4/tests/test_resources.py`

 * *Files identical despite different names*

### Comparing `expyre_wfl-0.1.3/tests/test_schedulers.py` & `expyre_wfl-0.1.4/tests/test_schedulers.py`

 * *Files identical despite different names*

### Comparing `expyre_wfl-0.1.3/tests/test_subprocess.py` & `expyre_wfl-0.1.4/tests/test_subprocess.py`

 * *Files identical despite different names*

### Comparing `expyre_wfl-0.1.3/tests/test_system.py` & `expyre_wfl-0.1.4/tests/test_system.py`

 * *Files identical despite different names*

### Comparing `expyre_wfl-0.1.3/tests/test_units.py` & `expyre_wfl-0.1.4/tests/test_units.py`

 * *Files identical despite different names*

