# Comparing `tmp/optprompt-0.4.0.tar.gz` & `tmp/optprompt-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/optprompt-0.4.0.tar", last modified: Tue Jan  7 20:42:37 2020, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `optprompt-0.4.0.tar` & `optprompt-0.5.0.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxrwxr-x   0 dylan     (1000) dylan     (1000)        0 2020-01-07 20:42:37.000000 optprompt-0.4.0/
--rw-rw-r--   0 dylan     (1000) dylan     (1000)     1446 2020-01-07 20:42:37.000000 optprompt-0.4.0/PKG-INFO
--rw-rw-r--   0 dylan     (1000) dylan     (1000)      643 2019-11-26 19:23:41.000000 optprompt-0.4.0/README.md
-drwxrwxr-x   0 dylan     (1000) dylan     (1000)        0 2020-01-07 20:42:37.000000 optprompt-0.4.0/optprompt/
--rw-rw-r--   0 dylan     (1000) dylan     (1000)       47 2019-11-13 19:18:13.000000 optprompt-0.4.0/optprompt/__init__.py
--rw-rw-r--   0 dylan     (1000) dylan     (1000)     2537 2020-01-07 20:33:35.000000 optprompt-0.4.0/optprompt/optprompt.py
-drwxrwxr-x   0 dylan     (1000) dylan     (1000)        0 2020-01-07 20:42:37.000000 optprompt-0.4.0/optprompt.egg-info/
--rw-rw-r--   0 dylan     (1000) dylan     (1000)     1446 2020-01-07 20:42:37.000000 optprompt-0.4.0/optprompt.egg-info/PKG-INFO
--rw-rw-r--   0 dylan     (1000) dylan     (1000)      227 2020-01-07 20:42:37.000000 optprompt-0.4.0/optprompt.egg-info/SOURCES.txt
--rw-rw-r--   0 dylan     (1000) dylan     (1000)        1 2020-01-07 20:42:37.000000 optprompt-0.4.0/optprompt.egg-info/dependency_links.txt
--rw-rw-r--   0 dylan     (1000) dylan     (1000)        5 2020-01-07 20:42:37.000000 optprompt-0.4.0/optprompt.egg-info/requires.txt
--rw-rw-r--   0 dylan     (1000) dylan     (1000)       10 2020-01-07 20:42:37.000000 optprompt-0.4.0/optprompt.egg-info/top_level.txt
--rw-rw-r--   0 dylan     (1000) dylan     (1000)       38 2020-01-07 20:42:37.000000 optprompt-0.4.0/setup.cfg
--rw-rw-r--   0 dylan     (1000) dylan     (1000)      947 2020-01-07 20:38:13.000000 optprompt-0.4.0/setup.py
+-rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 optprompt-0.5.0/.flake8
+-rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 optprompt-0.5.0/MANIFEST.in
+-rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 optprompt-0.5.0/requirements.txt
+-rw-r--r--   0        0        0      492 2020-02-02 00:00:00.000000 optprompt-0.5.0/.github/workflows/checks.yml
+-rw-r--r--   0        0        0      529 2020-02-02 00:00:00.000000 optprompt-0.5.0/examples/example.py
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 optprompt-0.5.0/examples/example.toml
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 optprompt-0.5.0/optprompt/__init__.py
+-rw-r--r--   0        0        0     2622 2020-02-02 00:00:00.000000 optprompt-0.5.0/optprompt/optprompt.py
+-rw-r--r--   0        0        0      999 2020-02-02 00:00:00.000000 optprompt-0.5.0/packaging/optprompt.spec
+-rw-r--r--   0        0        0     1801 2020-02-02 00:00:00.000000 optprompt-0.5.0/tests/test_optprompt.py
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 optprompt-0.5.0/.gitignore
+-rw-r--r--   0        0        0    34523 2020-02-02 00:00:00.000000 optprompt-0.5.0/LICENSE
+-rw-r--r--   0        0        0      643 2020-02-02 00:00:00.000000 optprompt-0.5.0/README.md
+-rw-r--r--   0        0        0      672 2020-02-02 00:00:00.000000 optprompt-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0     1243 2020-02-02 00:00:00.000000 optprompt-0.5.0/PKG-INFO
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `optprompt-0.4.0/README.md` & `optprompt-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `optprompt-0.4.0/optprompt/optprompt.py` & `optprompt-0.5.0/optprompt/optprompt.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,16 @@
 # -*- coding: utf-8 -*-
+
+# Copyright 2024 Dylan Stephano-Shachter
+# See LICENSE file for licensing details
+
 import argparse
 import getpass
 import os
+
 import toml
 
 
 class OptionPrompterError(Exception):
     pass
```

