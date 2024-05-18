# Comparing `tmp/atooms_pp-4.0.0.tar.gz` & `tmp/atooms_pp-4.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "atooms_pp-4.0.0.tar", last modified: Sun Apr 28 20:43:57 2024, max compression
+gzip compressed data, was "atooms_pp-4.0.1.tar", last modified: Sat May 18 16:06:07 2024, max compression
```

## Comparing `atooms_pp-4.0.0.tar` & `atooms_pp-4.0.1.tar`

### file list

```diff
@@ -1,46 +1,49 @@
-drwxrwxr-x   0 coslo     (1000) coslo     (1000)        0 2024-04-28 20:43:57.438511 atooms_pp-4.0.0/
--rw-rw-r--   0 coslo     (1000) coslo     (1000)    35147 2021-11-14 11:19:34.000000 atooms_pp-4.0.0/LICENSE
--rw-r--r--   0 coslo     (1000) coslo     (1000)     4787 2024-04-28 20:43:57.438511 atooms_pp-4.0.0/PKG-INFO
--rw-rw-r--   0 coslo     (1000) coslo     (1000)     3967 2022-02-15 14:06:29.000000 atooms_pp-4.0.0/README.md
-drwxrwxr-x   0 coslo     (1000) coslo     (1000)        0 2024-04-28 20:43:57.434511 atooms_pp-4.0.0/atooms/
-drwxrwxr-x   0 coslo     (1000) coslo     (1000)        0 2024-04-28 20:43:57.438511 atooms_pp-4.0.0/atooms/postprocessing/
--rw-rw-r--   0 coslo     (1000) coslo     (1000)      723 2024-04-14 06:46:04.000000 atooms_pp-4.0.0/atooms/postprocessing/__init__.py
--rw-rw-r--   0 coslo     (1000) coslo     (1000)       22 2024-04-28 20:43:51.000000 atooms_pp-4.0.0/atooms/postprocessing/_version.py
--rw-rw-r--   0 coslo     (1000) coslo     (1000)     1682 2024-04-28 20:01:50.000000 atooms_pp-4.0.0/atooms/postprocessing/alpha2.py
--rw-rw-r--   0 coslo     (1000) coslo     (1000)    15122 2024-04-28 20:01:50.000000 atooms_pp-4.0.0/atooms/postprocessing/api.py
--rw-rw-r--   0 coslo     (1000) coslo     (1000)     5992 2024-04-28 20:01:50.000000 atooms_pp-4.0.0/atooms/postprocessing/ba.py
--rw-rw-r--   0 coslo     (1000) coslo     (1000)     4627 2024-04-28 20:01:50.000000 atooms_pp-4.0.0/atooms/postprocessing/chi4t.py
--rw-rw-r--   0 coslo     (1000) coslo     (1000)     3414 2024-04-28 17:13:10.000000 atooms_pp-4.0.0/atooms/postprocessing/cli.py
--rw-rw-r--   0 coslo     (1000) coslo     (1000)     2015 2024-04-28 17:52:29.000000 atooms_pp-4.0.0/atooms/postprocessing/core.py
--rw-rw-r--   0 coslo     (1000) coslo     (1000)    28841 2024-04-28 20:25:29.000000 atooms_pp-4.0.0/atooms/postprocessing/correlation.py
--rw-rw-r--   0 coslo     (1000) coslo     (1000)     2138 2024-04-28 20:01:50.000000 atooms_pp-4.0.0/atooms/postprocessing/filter.py
--rw-rw-r--   0 coslo     (1000) coslo     (1000)    17389 2024-04-28 20:01:50.000000 atooms_pp-4.0.0/atooms/postprocessing/fkt.py
--rw-rw-r--   0 coslo     (1000) coslo     (1000)    15598 2024-04-28 20:01:50.000000 atooms_pp-4.0.0/atooms/postprocessing/fourierspace.py
--rw-rw-r--   0 coslo     (1000) coslo     (1000)    13982 2024-04-28 20:01:50.000000 atooms_pp-4.0.0/atooms/postprocessing/gr.py
--rw-rw-r--   0 coslo     (1000) coslo     (1000)     7653 2024-04-14 06:46:04.000000 atooms_pp-4.0.0/atooms/postprocessing/helpers.py
--rw-rw-r--   0 coslo     (1000) coslo     (1000)     2941 2024-04-28 20:01:50.000000 atooms_pp-4.0.0/atooms/postprocessing/ik.py
--rw-rw-r--   0 coslo     (1000) coslo     (1000)    10529 2024-04-14 06:46:04.000000 atooms_pp-4.0.0/atooms/postprocessing/linkedcells.py
--rw-rw-r--   0 coslo     (1000) coslo     (1000)     3767 2024-04-28 20:01:50.000000 atooms_pp-4.0.0/atooms/postprocessing/msd.py
--rw-rw-r--   0 coslo     (1000) coslo     (1000)     4910 2024-04-28 20:01:50.000000 atooms_pp-4.0.0/atooms/postprocessing/partial.py
--rw-rw-r--   0 coslo     (1000) coslo     (1000)     1750 2024-04-14 06:46:04.000000 atooms_pp-4.0.0/atooms/postprocessing/progress.py
--rw-rw-r--   0 coslo     (1000) coslo     (1000)     3112 2024-04-28 20:01:50.000000 atooms_pp-4.0.0/atooms/postprocessing/qt.py
--rw-rw-r--   0 coslo     (1000) coslo     (1000)     4220 2024-04-28 20:01:50.000000 atooms_pp-4.0.0/atooms/postprocessing/s4kt.py
--rw-rw-r--   0 coslo     (1000) coslo     (1000)     1715 2024-04-28 20:01:50.000000 atooms_pp-4.0.0/atooms/postprocessing/sacf.py
--rw-rw-r--   0 coslo     (1000) coslo     (1000)    10066 2024-04-28 20:01:50.000000 atooms_pp-4.0.0/atooms/postprocessing/sk.py
--rw-rw-r--   0 coslo     (1000) coslo     (1000)     1689 2024-04-28 20:01:50.000000 atooms_pp-4.0.0/atooms/postprocessing/susceptibility.py
--rw-rw-r--   0 coslo     (1000) coslo     (1000)     1282 2024-04-28 20:01:50.000000 atooms_pp-4.0.0/atooms/postprocessing/vacf.py
-drwxrwxr-x   0 coslo     (1000) coslo     (1000)        0 2024-04-28 20:43:57.438511 atooms_pp-4.0.0/atooms_pp.egg-info/
--rw-r--r--   0 coslo     (1000) coslo     (1000)     4787 2024-04-28 20:43:57.000000 atooms_pp-4.0.0/atooms_pp.egg-info/PKG-INFO
--rw-rw-r--   0 coslo     (1000) coslo     (1000)     1081 2024-04-28 20:43:57.000000 atooms_pp-4.0.0/atooms_pp.egg-info/SOURCES.txt
--rw-rw-r--   0 coslo     (1000) coslo     (1000)        1 2024-04-28 20:43:57.000000 atooms_pp-4.0.0/atooms_pp.egg-info/dependency_links.txt
--rw-rw-r--   0 coslo     (1000) coslo     (1000)       35 2024-04-28 20:43:57.000000 atooms_pp-4.0.0/atooms_pp.egg-info/requires.txt
--rw-rw-r--   0 coslo     (1000) coslo     (1000)        7 2024-04-28 20:43:57.000000 atooms_pp-4.0.0/atooms_pp.egg-info/top_level.txt
-drwxrwxr-x   0 coslo     (1000) coslo     (1000)        0 2024-04-28 20:43:57.438511 atooms_pp-4.0.0/bin/
--rwxrwxr-x   0 coslo     (1000) coslo     (1000)     3381 2020-11-04 22:11:46.000000 atooms_pp-4.0.0/bin/pp.py
--rw-rw-r--   0 coslo     (1000) coslo     (1000)     1166 2024-04-28 20:43:51.000000 atooms_pp-4.0.0/pyproject.toml
--rw-rw-r--   0 coslo     (1000) coslo     (1000)      173 2024-04-28 20:43:57.438511 atooms_pp-4.0.0/setup.cfg
-drwxrwxr-x   0 coslo     (1000) coslo     (1000)        0 2024-04-28 20:43:57.438511 atooms_pp-4.0.0/tests/
--rw-rw-r--   0 coslo     (1000) coslo     (1000)     1031 2024-04-13 21:37:27.000000 atooms_pp-4.0.0/tests/test_api.py
--rw-rw-r--   0 coslo     (1000) coslo     (1000)      747 2024-04-13 21:37:27.000000 atooms_pp-4.0.0/tests/test_helpers.py
--rw-rw-r--   0 coslo     (1000) coslo     (1000)     1263 2024-04-13 21:37:27.000000 atooms_pp-4.0.0/tests/test_ll.py
--rw-rw-r--   0 coslo     (1000) coslo     (1000)    30919 2024-04-28 20:27:21.000000 atooms_pp-4.0.0/tests/test_pp.py
+drwxrwxr-x   0 coslo     (1000) coslo     (1000)        0 2024-05-18 16:06:07.372662 atooms_pp-4.0.1/
+-rw-rw-r--   0 coslo     (1000) coslo     (1000)    35147 2021-11-14 11:19:34.000000 atooms_pp-4.0.1/LICENSE
+-rw-rw-r--   0 coslo     (1000) coslo     (1000)       35 2024-04-30 12:10:51.000000 atooms_pp-4.0.1/MANIFEST.in
+-rw-r--r--   0 coslo     (1000) coslo     (1000)     4774 2024-05-18 16:06:07.372662 atooms_pp-4.0.1/PKG-INFO
+-rw-rw-r--   0 coslo     (1000) coslo     (1000)     3954 2024-04-30 12:19:29.000000 atooms_pp-4.0.1/README.md
+drwxrwxr-x   0 coslo     (1000) coslo     (1000)        0 2024-05-18 16:06:07.352662 atooms_pp-4.0.1/atooms/
+drwxrwxr-x   0 coslo     (1000) coslo     (1000)        0 2024-05-18 16:06:07.368662 atooms_pp-4.0.1/atooms/postprocessing/
+-rw-rw-r--   0 coslo     (1000) coslo     (1000)      723 2024-04-14 06:46:04.000000 atooms_pp-4.0.1/atooms/postprocessing/__init__.py
+-rw-rw-r--   0 coslo     (1000) coslo     (1000)       22 2024-05-18 16:06:00.000000 atooms_pp-4.0.1/atooms/postprocessing/_version.py
+-rw-rw-r--   0 coslo     (1000) coslo     (1000)     1682 2024-04-28 20:01:50.000000 atooms_pp-4.0.1/atooms/postprocessing/alpha2.py
+-rw-rw-r--   0 coslo     (1000) coslo     (1000)    15122 2024-04-28 20:01:50.000000 atooms_pp-4.0.1/atooms/postprocessing/api.py
+-rw-rw-r--   0 coslo     (1000) coslo     (1000)     5992 2024-04-28 20:01:50.000000 atooms_pp-4.0.1/atooms/postprocessing/ba.py
+-rw-rw-r--   0 coslo     (1000) coslo     (1000)     4627 2024-04-28 20:01:50.000000 atooms_pp-4.0.1/atooms/postprocessing/chi4t.py
+-rw-rw-r--   0 coslo     (1000) coslo     (1000)     3414 2024-04-28 17:13:10.000000 atooms_pp-4.0.1/atooms/postprocessing/cli.py
+-rw-rw-r--   0 coslo     (1000) coslo     (1000)     2015 2024-04-28 17:52:29.000000 atooms_pp-4.0.1/atooms/postprocessing/core.py
+-rw-rw-r--   0 coslo     (1000) coslo     (1000)    28841 2024-04-28 20:25:29.000000 atooms_pp-4.0.1/atooms/postprocessing/correlation.py
+-rw-rw-r--   0 coslo     (1000) coslo     (1000)     2138 2024-04-28 20:01:50.000000 atooms_pp-4.0.1/atooms/postprocessing/filter.py
+-rw-rw-r--   0 coslo     (1000) coslo     (1000)    17389 2024-04-28 20:01:50.000000 atooms_pp-4.0.1/atooms/postprocessing/fkt.py
+-rw-rw-r--   0 coslo     (1000) coslo     (1000)     2856 2024-03-22 13:03:56.000000 atooms_pp-4.0.1/atooms/postprocessing/fourierspace.f90
+-rw-rw-r--   0 coslo     (1000) coslo     (1000)    15598 2024-04-28 20:01:50.000000 atooms_pp-4.0.1/atooms/postprocessing/fourierspace.py
+-rw-rw-r--   0 coslo     (1000) coslo     (1000)    13982 2024-04-28 20:01:50.000000 atooms_pp-4.0.1/atooms/postprocessing/gr.py
+-rw-rw-r--   0 coslo     (1000) coslo     (1000)     7653 2024-04-14 06:46:04.000000 atooms_pp-4.0.1/atooms/postprocessing/helpers.py
+-rw-rw-r--   0 coslo     (1000) coslo     (1000)     2941 2024-04-28 20:01:50.000000 atooms_pp-4.0.1/atooms/postprocessing/ik.py
+-rw-rw-r--   0 coslo     (1000) coslo     (1000)    10529 2024-04-14 06:46:04.000000 atooms_pp-4.0.1/atooms/postprocessing/linkedcells.py
+-rw-rw-r--   0 coslo     (1000) coslo     (1000)     3767 2024-04-28 20:01:50.000000 atooms_pp-4.0.1/atooms/postprocessing/msd.py
+-rw-rw-r--   0 coslo     (1000) coslo     (1000)     4910 2024-04-28 20:01:50.000000 atooms_pp-4.0.1/atooms/postprocessing/partial.py
+-rw-rw-r--   0 coslo     (1000) coslo     (1000)     1750 2024-04-14 06:46:04.000000 atooms_pp-4.0.1/atooms/postprocessing/progress.py
+-rw-rw-r--   0 coslo     (1000) coslo     (1000)     3112 2024-04-28 20:01:50.000000 atooms_pp-4.0.1/atooms/postprocessing/qt.py
+-rw-rw-r--   0 coslo     (1000) coslo     (1000)    25144 2024-04-28 16:27:27.000000 atooms_pp-4.0.1/atooms/postprocessing/realspace.f90
+-rw-rw-r--   0 coslo     (1000) coslo     (1000)     4220 2024-04-28 20:01:50.000000 atooms_pp-4.0.1/atooms/postprocessing/s4kt.py
+-rw-rw-r--   0 coslo     (1000) coslo     (1000)     1715 2024-04-28 20:01:50.000000 atooms_pp-4.0.1/atooms/postprocessing/sacf.py
+-rw-rw-r--   0 coslo     (1000) coslo     (1000)    10066 2024-04-28 20:01:50.000000 atooms_pp-4.0.1/atooms/postprocessing/sk.py
+-rw-rw-r--   0 coslo     (1000) coslo     (1000)     1689 2024-04-28 20:01:50.000000 atooms_pp-4.0.1/atooms/postprocessing/susceptibility.py
+-rw-rw-r--   0 coslo     (1000) coslo     (1000)     1282 2024-04-28 20:01:50.000000 atooms_pp-4.0.1/atooms/postprocessing/vacf.py
+drwxrwxr-x   0 coslo     (1000) coslo     (1000)        0 2024-05-18 16:06:07.372662 atooms_pp-4.0.1/atooms_pp.egg-info/
+-rw-r--r--   0 coslo     (1000) coslo     (1000)     4774 2024-05-18 16:06:07.000000 atooms_pp-4.0.1/atooms_pp.egg-info/PKG-INFO
+-rw-rw-r--   0 coslo     (1000) coslo     (1000)     1168 2024-05-18 16:06:07.000000 atooms_pp-4.0.1/atooms_pp.egg-info/SOURCES.txt
+-rw-rw-r--   0 coslo     (1000) coslo     (1000)        1 2024-05-18 16:06:07.000000 atooms_pp-4.0.1/atooms_pp.egg-info/dependency_links.txt
+-rw-rw-r--   0 coslo     (1000) coslo     (1000)       35 2024-05-18 16:06:07.000000 atooms_pp-4.0.1/atooms_pp.egg-info/requires.txt
+-rw-rw-r--   0 coslo     (1000) coslo     (1000)        7 2024-05-18 16:06:07.000000 atooms_pp-4.0.1/atooms_pp.egg-info/top_level.txt
+drwxrwxr-x   0 coslo     (1000) coslo     (1000)        0 2024-05-18 16:06:07.368662 atooms_pp-4.0.1/bin/
+-rwxrwxr-x   0 coslo     (1000) coslo     (1000)     3381 2020-11-04 22:11:46.000000 atooms_pp-4.0.1/bin/pp.py
+-rw-rw-r--   0 coslo     (1000) coslo     (1000)     1194 2024-05-18 16:06:00.000000 atooms_pp-4.0.1/pyproject.toml
+-rw-rw-r--   0 coslo     (1000) coslo     (1000)      173 2024-05-18 16:06:07.372662 atooms_pp-4.0.1/setup.cfg
+drwxrwxr-x   0 coslo     (1000) coslo     (1000)        0 2024-05-18 16:06:07.368662 atooms_pp-4.0.1/tests/
+-rw-rw-r--   0 coslo     (1000) coslo     (1000)     1031 2024-04-13 21:37:27.000000 atooms_pp-4.0.1/tests/test_api.py
+-rw-rw-r--   0 coslo     (1000) coslo     (1000)      747 2024-04-13 21:37:27.000000 atooms_pp-4.0.1/tests/test_helpers.py
+-rw-rw-r--   0 coslo     (1000) coslo     (1000)     1263 2024-04-13 21:37:27.000000 atooms_pp-4.0.1/tests/test_ll.py
+-rw-rw-r--   0 coslo     (1000) coslo     (1000)    30919 2024-04-28 20:27:21.000000 atooms_pp-4.0.1/tests/test_pp.py
```

### Comparing `atooms_pp-4.0.0/LICENSE` & `atooms_pp-4.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `atooms_pp-4.0.0/PKG-INFO` & `atooms_pp-4.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: atooms-pp
-Version: 4.0.0
+Version: 4.0.1
 Summary: Post-processing tools for particle simulations
 Author-email: Daniele Coslovich <daniele.coslovich@umontpellier.fr>
 License: GPLv3
 Project-URL: repository, https://framagit.org/atooms/postprocessing
 Project-URL: homepage, https://framagit.org/atooms/postprocessing
 Project-URL: documentation, https://atooms.frama.io/postprocessing
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.7
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: atooms>=2
 Requires-Dist: numpy
 Requires-Dist: argh
 Requires-Dist: tqdm
@@ -23,15 +23,15 @@
 # Postprocessing
 
 [![pypi](https://img.shields.io/pypi/v/atooms-pp.svg)](https://pypi.python.org/pypi/atooms-pp/)
 [![version](https://img.shields.io/pypi/pyversions/atooms-pp.svg)](https://pypi.python.org/pypi/atooms-pp/)
 [![license](https://img.shields.io/pypi/l/atooms-pp.svg)](https://en.wikipedia.org/wiki/GNU_General_Public_License)
 [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/git/https%3A%2F%2Fframagit.org%2Fatooms%2Fpostprocessing/HEAD?labpath=docs%2Findex.ipynb)
 [![pipeline](https://framagit.org/atooms/postprocessing/badges/master/pipeline.svg)](https://framagit.org/atooms/postprocessing/badges/master/pipeline.svg)
-[![coverage report](https://framagit.org/atooms/postprocessing/badges/master/coverage.svg?job=test:f90)](https://framagit.org/atooms/postprocessing/-/commits/master)
+[![coverage report](https://framagit.org/atooms/postprocessing/badges/master/coverage.svg)](https://framagit.org/atooms/postprocessing/-/commits/master)
 
 A Python package to compute static and dynamic correlation functions from simulations of interacting particles, such as molecular dynamics or Monte Carlo simulations. Based on [atooms](https://framagit.org/atooms/atooms).
 
 ## Quick start
 
 Postprocessing works on trajectories. Any trajectory format recognized by
 [atooms](https://framagit.org/atooms/atooms.git) can be processed, for instance most "xyz" files
```

### Comparing `atooms_pp-4.0.0/README.md` & `atooms_pp-4.0.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # Postprocessing
 
 [![pypi](https://img.shields.io/pypi/v/atooms-pp.svg)](https://pypi.python.org/pypi/atooms-pp/)
 [![version](https://img.shields.io/pypi/pyversions/atooms-pp.svg)](https://pypi.python.org/pypi/atooms-pp/)
 [![license](https://img.shields.io/pypi/l/atooms-pp.svg)](https://en.wikipedia.org/wiki/GNU_General_Public_License)
 [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/git/https%3A%2F%2Fframagit.org%2Fatooms%2Fpostprocessing/HEAD?labpath=docs%2Findex.ipynb)
 [![pipeline](https://framagit.org/atooms/postprocessing/badges/master/pipeline.svg)](https://framagit.org/atooms/postprocessing/badges/master/pipeline.svg)
-[![coverage report](https://framagit.org/atooms/postprocessing/badges/master/coverage.svg?job=test:f90)](https://framagit.org/atooms/postprocessing/-/commits/master)
+[![coverage report](https://framagit.org/atooms/postprocessing/badges/master/coverage.svg)](https://framagit.org/atooms/postprocessing/-/commits/master)
 
 A Python package to compute static and dynamic correlation functions from simulations of interacting particles, such as molecular dynamics or Monte Carlo simulations. Based on [atooms](https://framagit.org/atooms/atooms).
 
 ## Quick start
 
 Postprocessing works on trajectories. Any trajectory format recognized by
 [atooms](https://framagit.org/atooms/atooms.git) can be processed, for instance most "xyz" files
```

### Comparing `atooms_pp-4.0.0/atooms/postprocessing/__init__.py` & `atooms_pp-4.0.1/atooms/postprocessing/__init__.py`

 * *Files identical despite different names*

### Comparing `atooms_pp-4.0.0/atooms/postprocessing/alpha2.py` & `atooms_pp-4.0.1/atooms/postprocessing/alpha2.py`

 * *Files identical despite different names*

### Comparing `atooms_pp-4.0.0/atooms/postprocessing/api.py` & `atooms_pp-4.0.1/atooms/postprocessing/api.py`

 * *Files identical despite different names*

### Comparing `atooms_pp-4.0.0/atooms/postprocessing/ba.py` & `atooms_pp-4.0.1/atooms/postprocessing/ba.py`

 * *Files identical despite different names*

### Comparing `atooms_pp-4.0.0/atooms/postprocessing/chi4t.py` & `atooms_pp-4.0.1/atooms/postprocessing/chi4t.py`

 * *Files identical despite different names*

### Comparing `atooms_pp-4.0.0/atooms/postprocessing/cli.py` & `atooms_pp-4.0.1/atooms/postprocessing/cli.py`

 * *Files identical despite different names*

### Comparing `atooms_pp-4.0.0/atooms/postprocessing/core.py` & `atooms_pp-4.0.1/atooms/postprocessing/core.py`

 * *Files identical despite different names*

### Comparing `atooms_pp-4.0.0/atooms/postprocessing/correlation.py` & `atooms_pp-4.0.1/atooms/postprocessing/correlation.py`

 * *Files identical despite different names*

### Comparing `atooms_pp-4.0.0/atooms/postprocessing/filter.py` & `atooms_pp-4.0.1/atooms/postprocessing/filter.py`

 * *Files identical despite different names*

### Comparing `atooms_pp-4.0.0/atooms/postprocessing/fkt.py` & `atooms_pp-4.0.1/atooms/postprocessing/fkt.py`

 * *Files identical despite different names*

### Comparing `atooms_pp-4.0.0/atooms/postprocessing/fourierspace.py` & `atooms_pp-4.0.1/atooms/postprocessing/fourierspace.py`

 * *Files identical despite different names*

### Comparing `atooms_pp-4.0.0/atooms/postprocessing/gr.py` & `atooms_pp-4.0.1/atooms/postprocessing/gr.py`

 * *Files identical despite different names*

### Comparing `atooms_pp-4.0.0/atooms/postprocessing/helpers.py` & `atooms_pp-4.0.1/atooms/postprocessing/helpers.py`

 * *Files identical despite different names*

### Comparing `atooms_pp-4.0.0/atooms/postprocessing/ik.py` & `atooms_pp-4.0.1/atooms/postprocessing/ik.py`

 * *Files identical despite different names*

### Comparing `atooms_pp-4.0.0/atooms/postprocessing/linkedcells.py` & `atooms_pp-4.0.1/atooms/postprocessing/linkedcells.py`

 * *Files identical despite different names*

### Comparing `atooms_pp-4.0.0/atooms/postprocessing/msd.py` & `atooms_pp-4.0.1/atooms/postprocessing/msd.py`

 * *Files identical despite different names*

### Comparing `atooms_pp-4.0.0/atooms/postprocessing/partial.py` & `atooms_pp-4.0.1/atooms/postprocessing/partial.py`

 * *Files identical despite different names*

### Comparing `atooms_pp-4.0.0/atooms/postprocessing/progress.py` & `atooms_pp-4.0.1/atooms/postprocessing/progress.py`

 * *Files identical despite different names*

### Comparing `atooms_pp-4.0.0/atooms/postprocessing/qt.py` & `atooms_pp-4.0.1/atooms/postprocessing/qt.py`

 * *Files identical despite different names*

### Comparing `atooms_pp-4.0.0/atooms/postprocessing/s4kt.py` & `atooms_pp-4.0.1/atooms/postprocessing/s4kt.py`

 * *Files identical despite different names*

### Comparing `atooms_pp-4.0.0/atooms/postprocessing/sacf.py` & `atooms_pp-4.0.1/atooms/postprocessing/sacf.py`

 * *Files identical despite different names*

### Comparing `atooms_pp-4.0.0/atooms/postprocessing/sk.py` & `atooms_pp-4.0.1/atooms/postprocessing/sk.py`

 * *Files identical despite different names*

### Comparing `atooms_pp-4.0.0/atooms/postprocessing/susceptibility.py` & `atooms_pp-4.0.1/atooms/postprocessing/susceptibility.py`

 * *Files identical despite different names*

### Comparing `atooms_pp-4.0.0/atooms/postprocessing/vacf.py` & `atooms_pp-4.0.1/atooms/postprocessing/vacf.py`

 * *Files identical despite different names*

### Comparing `atooms_pp-4.0.0/atooms_pp.egg-info/PKG-INFO` & `atooms_pp-4.0.1/atooms_pp.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: atooms-pp
-Version: 4.0.0
+Version: 4.0.1
 Summary: Post-processing tools for particle simulations
 Author-email: Daniele Coslovich <daniele.coslovich@umontpellier.fr>
 License: GPLv3
 Project-URL: repository, https://framagit.org/atooms/postprocessing
 Project-URL: homepage, https://framagit.org/atooms/postprocessing
 Project-URL: documentation, https://atooms.frama.io/postprocessing
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.7
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: atooms>=2
 Requires-Dist: numpy
 Requires-Dist: argh
 Requires-Dist: tqdm
@@ -23,15 +23,15 @@
 # Postprocessing
 
 [![pypi](https://img.shields.io/pypi/v/atooms-pp.svg)](https://pypi.python.org/pypi/atooms-pp/)
 [![version](https://img.shields.io/pypi/pyversions/atooms-pp.svg)](https://pypi.python.org/pypi/atooms-pp/)
 [![license](https://img.shields.io/pypi/l/atooms-pp.svg)](https://en.wikipedia.org/wiki/GNU_General_Public_License)
 [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/git/https%3A%2F%2Fframagit.org%2Fatooms%2Fpostprocessing/HEAD?labpath=docs%2Findex.ipynb)
 [![pipeline](https://framagit.org/atooms/postprocessing/badges/master/pipeline.svg)](https://framagit.org/atooms/postprocessing/badges/master/pipeline.svg)
-[![coverage report](https://framagit.org/atooms/postprocessing/badges/master/coverage.svg?job=test:f90)](https://framagit.org/atooms/postprocessing/-/commits/master)
+[![coverage report](https://framagit.org/atooms/postprocessing/badges/master/coverage.svg)](https://framagit.org/atooms/postprocessing/-/commits/master)
 
 A Python package to compute static and dynamic correlation functions from simulations of interacting particles, such as molecular dynamics or Monte Carlo simulations. Based on [atooms](https://framagit.org/atooms/atooms).
 
 ## Quick start
 
 Postprocessing works on trajectories. Any trajectory format recognized by
 [atooms](https://framagit.org/atooms/atooms.git) can be processed, for instance most "xyz" files
```

### Comparing `atooms_pp-4.0.0/atooms_pp.egg-info/SOURCES.txt` & `atooms_pp-4.0.1/atooms_pp.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,31 +1,34 @@
 LICENSE
+MANIFEST.in
 README.md
 pyproject.toml
 setup.cfg
 atooms/postprocessing/__init__.py
 atooms/postprocessing/_version.py
 atooms/postprocessing/alpha2.py
 atooms/postprocessing/api.py
 atooms/postprocessing/ba.py
 atooms/postprocessing/chi4t.py
 atooms/postprocessing/cli.py
 atooms/postprocessing/core.py
 atooms/postprocessing/correlation.py
 atooms/postprocessing/filter.py
 atooms/postprocessing/fkt.py
+atooms/postprocessing/fourierspace.f90
 atooms/postprocessing/fourierspace.py
 atooms/postprocessing/gr.py
 atooms/postprocessing/helpers.py
 atooms/postprocessing/ik.py
 atooms/postprocessing/linkedcells.py
 atooms/postprocessing/msd.py
 atooms/postprocessing/partial.py
 atooms/postprocessing/progress.py
 atooms/postprocessing/qt.py
+atooms/postprocessing/realspace.f90
 atooms/postprocessing/s4kt.py
 atooms/postprocessing/sacf.py
 atooms/postprocessing/sk.py
 atooms/postprocessing/susceptibility.py
 atooms/postprocessing/vacf.py
 atooms_pp.egg-info/PKG-INFO
 atooms_pp.egg-info/SOURCES.txt
```

### Comparing `atooms_pp-4.0.0/bin/pp.py` & `atooms_pp-4.0.1/bin/pp.py`

 * *Files identical despite different names*

### Comparing `atooms_pp-4.0.0/pyproject.toml` & `atooms_pp-4.0.1/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [project]
 name = "atooms-pp"
 description = "Post-processing tools for particle simulations"
 readme = "README.md"
-version = "4.0.0"
+version = "4.0.1"
 authors = [
     {name = "Daniele Coslovich", email = "daniele.coslovich@umontpellier.fr"}
 ]
 requires-python = ">=3.7"
 license = {text = "GPLv3"}
 dependencies = [
     "atooms>=2",
@@ -15,15 +15,15 @@
     "tqdm",
     "f2py_jit"
 ]
 classifiers = [
     "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
     "Development Status :: 5 - Production/Stable",
     "Programming Language :: Python :: 3",
-    'Programming Language :: Python :: 3.8',
+    'Programming Language :: Python :: 3.7',
 ]
 
 
 [project.urls]
 repository = "https://framagit.org/atooms/postprocessing"
 homepage = "https://framagit.org/atooms/postprocessing"
 documentation = "https://atooms.frama.io/postprocessing"
@@ -32,14 +32,15 @@
 # [project.scripts]
 # pp = "atooms.postprocessing.cli:main"
 
 # Deprecated but still working.
 # It seems the only way to be backward compatible with scripts ending in .py
 [tool.setuptools]
 script-files = ["bin/pp.py"]
+include-package-data = true
 
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [tool.setuptools.packages.find]
 include = ["atooms.postprocessing"]
```

### Comparing `atooms_pp-4.0.0/tests/test_api.py` & `atooms_pp-4.0.1/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `atooms_pp-4.0.0/tests/test_helpers.py` & `atooms_pp-4.0.1/tests/test_helpers.py`

 * *Files identical despite different names*

### Comparing `atooms_pp-4.0.0/tests/test_ll.py` & `atooms_pp-4.0.1/tests/test_ll.py`

 * *Files identical despite different names*

### Comparing `atooms_pp-4.0.0/tests/test_pp.py` & `atooms_pp-4.0.1/tests/test_pp.py`

 * *Files identical despite different names*

