# Comparing `tmp/camptools-0.9.2.tar.gz` & `tmp/camptools-0.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "camptools-0.9.2.tar", last modified: Thu Jan 11 09:59:50 2024, max compression
+gzip compressed data, was "camptools-0.9.3.tar", last modified: Sat May 18 12:18:17 2024, max compression
```

## Comparing `camptools-0.9.2.tar` & `camptools-0.9.3.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-11 09:59:50.293655 camptools-0.9.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-01-11 09:59:34.000000 camptools-0.9.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3850 2024-01-11 09:59:50.293655 camptools-0.9.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3395 2024-01-11 09:59:34.000000 camptools-0.9.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-11 09:59:50.289656 camptools-0.9.2/camptools/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-11 09:59:34.000000 camptools-0.9.2/camptools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2818 2024-01-11 09:59:34.000000 camptools-0.9.2/camptools/checkpoint.py
--rw-r--r--   0 runner    (1001) docker     (127)     2945 2024-01-11 09:59:34.000000 camptools-0.9.2/camptools/cmdjob.py
--rw-r--r--   0 runner    (1001) docker     (127)      711 2024-01-11 09:59:34.000000 camptools-0.9.2/camptools/conversion_unit.py
--rw-r--r--   0 runner    (1001) docker     (127)     8066 2024-01-11 09:59:34.000000 camptools-0.9.2/camptools/create_vdist.py
--rw-r--r--   0 runner    (1001) docker     (127)     1813 2024-01-11 09:59:34.000000 camptools-0.9.2/camptools/extent_sim.py
--rw-r--r--   0 runner    (1001) docker     (127)     1609 2024-01-11 09:59:34.000000 camptools-0.9.2/camptools/filesync.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-11 09:59:50.293655 camptools-0.9.2/camptools/grand/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-11 09:59:34.000000 camptools-0.9.2/camptools/grand/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4813 2024-01-11 09:59:34.000000 camptools-0.9.2/camptools/grand/mypjsub.py
--rw-r--r--   0 runner    (1001) docker     (127)     4965 2024-01-11 09:59:34.000000 camptools-0.9.2/camptools/grand/pjsub_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (127)      593 2024-01-11 09:59:34.000000 camptools-0.9.2/camptools/job_history.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-11 09:59:50.293655 camptools-0.9.2/camptools/job_scheduler/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-11 09:59:34.000000 camptools-0.9.2/camptools/job_scheduler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2861 2024-01-11 09:59:34.000000 camptools-0.9.2/camptools/job_scheduler/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     2893 2024-01-11 09:59:34.000000 camptools-0.9.2/camptools/job_scheduler/laurel.py
--rw-r--r--   0 runner    (1001) docker     (127)     2987 2024-01-11 09:59:34.000000 camptools-0.9.2/camptools/job_scheduler/sbatch_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (127)     3037 2024-01-11 09:59:34.000000 camptools-0.9.2/camptools/job_scheduler/throw_job_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (127)     1574 2024-01-11 09:59:34.000000 camptools-0.9.2/camptools/job_status.py
--rw-r--r--   0 runner    (1001) docker     (127)     4204 2024-01-11 09:59:34.000000 camptools-0.9.2/camptools/jobs.py
--rw-r--r--   0 runner    (1001) docker     (127)     1251 2024-01-11 09:59:34.000000 camptools-0.9.2/camptools/latest_job.py
--rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-01-11 09:59:34.000000 camptools-0.9.2/camptools/mymkdir.py
--rw-r--r--   0 runner    (1001) docker     (127)     2613 2024-01-11 09:59:34.000000 camptools-0.9.2/camptools/qsub_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (127)     1696 2024-01-11 09:59:34.000000 camptools-0.9.2/camptools/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-11 09:59:50.293655 camptools-0.9.2/camptools/simmanager/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-11 09:59:34.000000 camptools-0.9.2/camptools/simmanager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      460 2024-01-11 09:59:34.000000 camptools-0.9.2/camptools/simmanager/copylist.py
--rw-r--r--   0 runner    (1001) docker     (127)    12942 2024-01-11 09:59:34.000000 camptools-0.9.2/camptools/simmanager/simmanager.py
--rw-r--r--   0 runner    (1001) docker     (127)     2373 2024-01-11 09:59:34.000000 camptools-0.9.2/camptools/simmanager/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      706 2024-01-11 09:59:34.000000 camptools-0.9.2/camptools/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-11 09:59:50.293655 camptools-0.9.2/camptools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3850 2024-01-11 09:59:50.000000 camptools-0.9.2/camptools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      980 2024-01-11 09:59:50.000000 camptools-0.9.2/camptools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-11 09:59:50.000000 camptools-0.9.2/camptools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      808 2024-01-11 09:59:50.000000 camptools-0.9.2/camptools.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-01-11 09:59:50.000000 camptools-0.9.2/camptools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-01-11 09:59:50.000000 camptools-0.9.2/camptools.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-11 09:59:50.293655 camptools-0.9.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1826 2024-01-11 09:59:34.000000 camptools-0.9.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 12:18:17.046016 camptools-0.9.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-05-18 12:18:07.000000 camptools-0.9.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3850 2024-05-18 12:18:17.046016 camptools-0.9.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3395 2024-05-18 12:18:07.000000 camptools-0.9.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 12:18:17.042016 camptools-0.9.3/camptools/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-18 12:18:07.000000 camptools-0.9.3/camptools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2818 2024-05-18 12:18:07.000000 camptools-0.9.3/camptools/checkpoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2945 2024-05-18 12:18:07.000000 camptools-0.9.3/camptools/cmdjob.py
+-rw-r--r--   0 runner    (1001) docker     (127)      711 2024-05-18 12:18:07.000000 camptools-0.9.3/camptools/conversion_unit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8066 2024-05-18 12:18:07.000000 camptools-0.9.3/camptools/create_vdist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1813 2024-05-18 12:18:07.000000 camptools-0.9.3/camptools/extent_sim.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1609 2024-05-18 12:18:07.000000 camptools-0.9.3/camptools/filesync.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 12:18:17.042016 camptools-0.9.3/camptools/grand/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-18 12:18:07.000000 camptools-0.9.3/camptools/grand/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4813 2024-05-18 12:18:07.000000 camptools-0.9.3/camptools/grand/mypjsub.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4965 2024-05-18 12:18:07.000000 camptools-0.9.3/camptools/grand/pjsub_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)      593 2024-05-18 12:18:07.000000 camptools-0.9.3/camptools/job_history.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 12:18:17.042016 camptools-0.9.3/camptools/job_scheduler/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-18 12:18:07.000000 camptools-0.9.3/camptools/job_scheduler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2861 2024-05-18 12:18:07.000000 camptools-0.9.3/camptools/job_scheduler/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2893 2024-05-18 12:18:07.000000 camptools-0.9.3/camptools/job_scheduler/laurel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2987 2024-05-18 12:18:07.000000 camptools-0.9.3/camptools/job_scheduler/sbatch_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3037 2024-05-18 12:18:07.000000 camptools-0.9.3/camptools/job_scheduler/throw_job_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1574 2024-05-18 12:18:07.000000 camptools-0.9.3/camptools/job_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4275 2024-05-18 12:18:07.000000 camptools-0.9.3/camptools/jobs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2249 2024-05-18 12:18:07.000000 camptools-0.9.3/camptools/latest_job.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-05-18 12:18:07.000000 camptools-0.9.3/camptools/mymkdir.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2613 2024-05-18 12:18:07.000000 camptools-0.9.3/camptools/qsub_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1696 2024-05-18 12:18:07.000000 camptools-0.9.3/camptools/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 12:18:17.046016 camptools-0.9.3/camptools/simmanager/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-18 12:18:07.000000 camptools-0.9.3/camptools/simmanager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      460 2024-05-18 12:18:07.000000 camptools-0.9.3/camptools/simmanager/copylist.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12942 2024-05-18 12:18:07.000000 camptools-0.9.3/camptools/simmanager/simmanager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2373 2024-05-18 12:18:07.000000 camptools-0.9.3/camptools/simmanager/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      706 2024-05-18 12:18:07.000000 camptools-0.9.3/camptools/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 12:18:17.046016 camptools-0.9.3/camptools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3850 2024-05-18 12:18:17.000000 camptools-0.9.3/camptools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      980 2024-05-18 12:18:17.000000 camptools-0.9.3/camptools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-18 12:18:17.000000 camptools-0.9.3/camptools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      808 2024-05-18 12:18:17.000000 camptools-0.9.3/camptools.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-18 12:18:17.000000 camptools-0.9.3/camptools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-18 12:18:17.000000 camptools-0.9.3/camptools.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-18 12:18:17.046016 camptools-0.9.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1826 2024-05-18 12:18:07.000000 camptools-0.9.3/setup.py
```

### Comparing `camptools-0.9.2/LICENSE` & `camptools-0.9.3/LICENSE`

 * *Files identical despite different names*

### Comparing `camptools-0.9.2/PKG-INFO` & `camptools-0.9.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: camptools
-Version: 0.9.2
+Version: 0.9.3
 Summary: Tools for camphor
 Home-page: https://github.com/Nkzono99/camptools
 Author: Nkzono
 Author-email: 71783375+Nkzono99@users.noreply.github.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `camptools-0.9.2/README.md` & `camptools-0.9.3/README.md`

 * *Files identical despite different names*

### Comparing `camptools-0.9.2/camptools/checkpoint.py` & `camptools-0.9.3/camptools/checkpoint.py`

 * *Files identical despite different names*

### Comparing `camptools-0.9.2/camptools/cmdjob.py` & `camptools-0.9.3/camptools/cmdjob.py`

 * *Files identical despite different names*

### Comparing `camptools-0.9.2/camptools/conversion_unit.py` & `camptools-0.9.3/camptools/conversion_unit.py`

 * *Files identical despite different names*

### Comparing `camptools-0.9.2/camptools/create_vdist.py` & `camptools-0.9.3/camptools/create_vdist.py`

 * *Files identical despite different names*

### Comparing `camptools-0.9.2/camptools/extent_sim.py` & `camptools-0.9.3/camptools/extent_sim.py`

 * *Files identical despite different names*

### Comparing `camptools-0.9.2/camptools/filesync.py` & `camptools-0.9.3/camptools/filesync.py`

 * *Files identical despite different names*

### Comparing `camptools-0.9.2/camptools/grand/mypjsub.py` & `camptools-0.9.3/camptools/grand/mypjsub.py`

 * *Files identical despite different names*

### Comparing `camptools-0.9.2/camptools/grand/pjsub_wrapper.py` & `camptools-0.9.3/camptools/grand/pjsub_wrapper.py`

 * *Files identical despite different names*

### Comparing `camptools-0.9.2/camptools/job_history.py` & `camptools-0.9.3/camptools/job_history.py`

 * *Files identical despite different names*

### Comparing `camptools-0.9.2/camptools/job_scheduler/core.py` & `camptools-0.9.3/camptools/job_scheduler/core.py`

 * *Files identical despite different names*

### Comparing `camptools-0.9.2/camptools/job_scheduler/laurel.py` & `camptools-0.9.3/camptools/job_scheduler/laurel.py`

 * *Files identical despite different names*

### Comparing `camptools-0.9.2/camptools/job_scheduler/sbatch_wrapper.py` & `camptools-0.9.3/camptools/job_scheduler/sbatch_wrapper.py`

 * *Files identical despite different names*

### Comparing `camptools-0.9.2/camptools/job_scheduler/throw_job_wrapper.py` & `camptools-0.9.3/camptools/job_scheduler/throw_job_wrapper.py`

 * *Files identical despite different names*

### Comparing `camptools-0.9.2/camptools/job_status.py` & `camptools-0.9.3/camptools/job_status.py`

 * *Files identical despite different names*

### Comparing `camptools-0.9.2/camptools/mymkdir.py` & `camptools-0.9.3/camptools/mymkdir.py`

 * *Files identical despite different names*

### Comparing `camptools-0.9.2/camptools/qsub_wrapper.py` & `camptools-0.9.3/camptools/qsub_wrapper.py`

 * *Files identical despite different names*

### Comparing `camptools-0.9.2/camptools/settings.py` & `camptools-0.9.3/camptools/settings.py`

 * *Files identical despite different names*

### Comparing `camptools-0.9.2/camptools/simmanager/simmanager.py` & `camptools-0.9.3/camptools/simmanager/simmanager.py`

 * *Files identical despite different names*

### Comparing `camptools-0.9.2/camptools/simmanager/utils.py` & `camptools-0.9.3/camptools/simmanager/utils.py`

 * *Files identical despite different names*

### Comparing `camptools-0.9.2/camptools/utils.py` & `camptools-0.9.3/camptools/utils.py`

 * *Files identical despite different names*

### Comparing `camptools-0.9.2/camptools.egg-info/PKG-INFO` & `camptools-0.9.3/camptools.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: camptools
-Version: 0.9.2
+Version: 0.9.3
 Summary: Tools for camphor
 Home-page: https://github.com/Nkzono99/camptools
 Author: Nkzono
 Author-email: 71783375+Nkzono99@users.noreply.github.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `camptools-0.9.2/camptools.egg-info/SOURCES.txt` & `camptools-0.9.3/camptools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `camptools-0.9.2/camptools.egg-info/entry_points.txt` & `camptools-0.9.3/camptools.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `camptools-0.9.2/setup.py` & `camptools-0.9.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 
 long_description = open('README.md', 'r', encoding='utf-8').read()
 
 setup(
     name="camptools",
-    version="0.9.2",
+    version="0.9.3",
     install_requires=[
         'f90nml',
     ],
     entry_points={
         'console_scripts': [
             'nmyqsub = camptools.qsub_wrapper:nmyqsub',
             'myqsub = camptools.qsub_wrapper:myqsub',
```

