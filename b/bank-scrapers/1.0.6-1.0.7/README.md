# Comparing `tmp/bank_scrapers-1.0.6.tar.gz` & `tmp/bank_scrapers-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bank_scrapers-1.0.6.tar", last modified: Sat May 18 05:03:47 2024, max compression
+gzip compressed data, was "bank_scrapers-1.0.7.tar", last modified: Sat May 18 05:09:35 2024, max compression
```

## Comparing `bank_scrapers-1.0.6.tar` & `bank_scrapers-1.0.7.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxrwxr-x   0 eric      (1000) eric      (1000)        0 2024-05-18 05:03:47.950358 bank_scrapers-1.0.6/
--rw-rw-r--   0 eric      (1000) eric      (1000)     1066 2024-05-16 09:36:03.000000 bank_scrapers-1.0.6/LICENSE
--rw-r--r--   0 eric      (1000) eric      (1000)    22466 2024-05-18 05:03:47.950358 bank_scrapers-1.0.6/PKG-INFO
--rw-rw-r--   0 eric      (1000) eric      (1000)    20665 2024-05-16 09:36:03.000000 bank_scrapers-1.0.6/README.md
-drwxrwxr-x   0 eric      (1000) eric      (1000)        0 2024-05-18 05:03:47.947358 bank_scrapers-1.0.6/bank_scrapers/
--rw-rw-r--   0 eric      (1000) eric      (1000)      307 2024-05-18 05:01:51.000000 bank_scrapers-1.0.6/bank_scrapers/__init__.py
-drwxrwxr-x   0 eric      (1000) eric      (1000)        0 2024-05-18 05:03:47.948358 bank_scrapers-1.0.6/bank_scrapers/api_wrappers/
--rw-rw-r--   0 eric      (1000) eric      (1000)        0 2024-05-16 09:36:03.000000 bank_scrapers-1.0.6/bank_scrapers/api_wrappers/__init__.py
-drwxrwxr-x   0 eric      (1000) eric      (1000)        0 2024-05-18 05:03:47.948358 bank_scrapers-1.0.6/bank_scrapers/api_wrappers/kraken/
--rw-rw-r--   0 eric      (1000) eric      (1000)        0 2024-05-16 09:36:03.000000 bank_scrapers-1.0.6/bank_scrapers/api_wrappers/kraken/__init__.py
--rw-rw-r--   0 eric      (1000) eric      (1000)     2863 2024-05-16 09:36:03.000000 bank_scrapers-1.0.6/bank_scrapers/api_wrappers/kraken/driver.py
-drwxrwxr-x   0 eric      (1000) eric      (1000)        0 2024-05-18 05:03:47.948358 bank_scrapers-1.0.6/bank_scrapers/cli/
--rw-rw-r--   0 eric      (1000) eric      (1000)        0 2024-05-16 09:36:03.000000 bank_scrapers-1.0.6/bank_scrapers/cli/__init__.py
--rw-rw-r--   0 eric      (1000) eric      (1000)     9027 2024-05-16 09:36:03.000000 bank_scrapers-1.0.6/bank_scrapers/cli/cli.py
-drwxrwxr-x   0 eric      (1000) eric      (1000)        0 2024-05-18 05:03:47.948358 bank_scrapers-1.0.6/bank_scrapers/common/
--rw-rw-r--   0 eric      (1000) eric      (1000)        0 2024-05-16 09:36:03.000000 bank_scrapers-1.0.6/bank_scrapers/common/__init__.py
--rw-rw-r--   0 eric      (1000) eric      (1000)      272 2024-05-16 09:36:03.000000 bank_scrapers-1.0.6/bank_scrapers/common/log.py
-drwxrwxr-x   0 eric      (1000) eric      (1000)        0 2024-05-18 05:03:47.948358 bank_scrapers-1.0.6/bank_scrapers/scrapers/
--rw-rw-r--   0 eric      (1000) eric      (1000)        0 2024-05-16 09:36:03.000000 bank_scrapers-1.0.6/bank_scrapers/scrapers/__init__.py
-drwxrwxr-x   0 eric      (1000) eric      (1000)        0 2024-05-18 05:03:47.949358 bank_scrapers-1.0.6/bank_scrapers/scrapers/becu/
--rw-rw-r--   0 eric      (1000) eric      (1000)        0 2024-05-16 09:36:03.000000 bank_scrapers-1.0.6/bank_scrapers/scrapers/becu/__init__.py
--rw-rw-r--   0 eric      (1000) eric      (1000)     6910 2024-05-18 04:44:12.000000 bank_scrapers-1.0.6/bank_scrapers/scrapers/becu/driver.py
-drwxrwxr-x   0 eric      (1000) eric      (1000)        0 2024-05-18 05:03:47.949358 bank_scrapers-1.0.6/bank_scrapers/scrapers/chase/
--rw-rw-r--   0 eric      (1000) eric      (1000)        0 2024-05-16 09:36:03.000000 bank_scrapers-1.0.6/bank_scrapers/scrapers/chase/__init__.py
--rw-rw-r--   0 eric      (1000) eric      (1000)     9191 2024-05-16 09:36:03.000000 bank_scrapers-1.0.6/bank_scrapers/scrapers/chase/driver.py
-drwxrwxr-x   0 eric      (1000) eric      (1000)        0 2024-05-18 05:03:47.949358 bank_scrapers-1.0.6/bank_scrapers/scrapers/common/
--rw-rw-r--   0 eric      (1000) eric      (1000)        0 2024-05-16 09:36:03.000000 bank_scrapers-1.0.6/bank_scrapers/scrapers/common/__init__.py
--rw-rw-r--   0 eric      (1000) eric      (1000)     4712 2024-05-16 09:36:03.000000 bank_scrapers-1.0.6/bank_scrapers/scrapers/common/functions.py
-drwxrwxr-x   0 eric      (1000) eric      (1000)        0 2024-05-18 05:03:47.949358 bank_scrapers-1.0.6/bank_scrapers/scrapers/fidelity_netbenefits/
--rw-rw-r--   0 eric      (1000) eric      (1000)        0 2024-05-16 09:36:03.000000 bank_scrapers-1.0.6/bank_scrapers/scrapers/fidelity_netbenefits/__init__.py
--rw-rw-r--   0 eric      (1000) eric      (1000)     8335 2024-05-16 09:36:03.000000 bank_scrapers-1.0.6/bank_scrapers/scrapers/fidelity_netbenefits/driver.py
-drwxrwxr-x   0 eric      (1000) eric      (1000)        0 2024-05-18 05:03:47.949358 bank_scrapers-1.0.6/bank_scrapers/scrapers/roundpoint/
--rw-rw-r--   0 eric      (1000) eric      (1000)        0 2024-05-16 09:36:03.000000 bank_scrapers-1.0.6/bank_scrapers/scrapers/roundpoint/__init__.py
--rw-rw-r--   0 eric      (1000) eric      (1000)     8626 2024-05-16 09:36:03.000000 bank_scrapers-1.0.6/bank_scrapers/scrapers/roundpoint/driver.py
-drwxrwxr-x   0 eric      (1000) eric      (1000)        0 2024-05-18 05:03:47.949358 bank_scrapers-1.0.6/bank_scrapers/scrapers/smbc_prestia/
--rw-rw-r--   0 eric      (1000) eric      (1000)        0 2024-05-16 09:36:03.000000 bank_scrapers-1.0.6/bank_scrapers/scrapers/smbc_prestia/__init__.py
--rw-rw-r--   0 eric      (1000) eric      (1000)     4632 2024-05-16 09:36:03.000000 bank_scrapers-1.0.6/bank_scrapers/scrapers/smbc_prestia/driver.py
-drwxrwxr-x   0 eric      (1000) eric      (1000)        0 2024-05-18 05:03:47.950358 bank_scrapers-1.0.6/bank_scrapers/scrapers/uhfcu/
--rw-rw-r--   0 eric      (1000) eric      (1000)        0 2024-05-16 09:36:03.000000 bank_scrapers-1.0.6/bank_scrapers/scrapers/uhfcu/__init__.py
--rw-rw-r--   0 eric      (1000) eric      (1000)     8655 2024-05-16 09:36:03.000000 bank_scrapers-1.0.6/bank_scrapers/scrapers/uhfcu/driver.py
-drwxrwxr-x   0 eric      (1000) eric      (1000)        0 2024-05-18 05:03:47.950358 bank_scrapers-1.0.6/bank_scrapers/scrapers/vanguard/
--rw-rw-r--   0 eric      (1000) eric      (1000)        0 2024-05-16 09:36:03.000000 bank_scrapers-1.0.6/bank_scrapers/scrapers/vanguard/__init__.py
--rw-rw-r--   0 eric      (1000) eric      (1000)     7740 2024-05-16 09:36:03.000000 bank_scrapers-1.0.6/bank_scrapers/scrapers/vanguard/driver.py
-drwxrwxr-x   0 eric      (1000) eric      (1000)        0 2024-05-18 05:03:47.950358 bank_scrapers-1.0.6/bank_scrapers/scrapers/zillow/
--rw-rw-r--   0 eric      (1000) eric      (1000)        0 2024-05-16 09:36:03.000000 bank_scrapers-1.0.6/bank_scrapers/scrapers/zillow/__init__.py
--rw-rw-r--   0 eric      (1000) eric      (1000)     3457 2024-05-16 09:36:03.000000 bank_scrapers-1.0.6/bank_scrapers/scrapers/zillow/driver.py
-drwxrwxr-x   0 eric      (1000) eric      (1000)        0 2024-05-18 05:03:47.950358 bank_scrapers-1.0.6/bank_scrapers.egg-info/
--rw-r--r--   0 eric      (1000) eric      (1000)    22466 2024-05-18 05:03:47.000000 bank_scrapers-1.0.6/bank_scrapers.egg-info/PKG-INFO
--rw-rw-r--   0 eric      (1000) eric      (1000)     1347 2024-05-18 05:03:47.000000 bank_scrapers-1.0.6/bank_scrapers.egg-info/SOURCES.txt
--rw-rw-r--   0 eric      (1000) eric      (1000)        1 2024-05-18 05:03:47.000000 bank_scrapers-1.0.6/bank_scrapers.egg-info/dependency_links.txt
--rw-rw-r--   0 eric      (1000) eric      (1000)       59 2024-05-18 05:03:47.000000 bank_scrapers-1.0.6/bank_scrapers.egg-info/entry_points.txt
--rw-rw-r--   0 eric      (1000) eric      (1000)      149 2024-05-18 05:03:47.000000 bank_scrapers-1.0.6/bank_scrapers.egg-info/requires.txt
--rw-rw-r--   0 eric      (1000) eric      (1000)       14 2024-05-18 05:03:47.000000 bank_scrapers-1.0.6/bank_scrapers.egg-info/top_level.txt
--rw-rw-r--   0 eric      (1000) eric      (1000)      990 2024-05-18 05:01:51.000000 bank_scrapers-1.0.6/pyproject.toml
--rw-rw-r--   0 eric      (1000) eric      (1000)       38 2024-05-18 05:03:47.950358 bank_scrapers-1.0.6/setup.cfg
+drwxrwxr-x   0 eric      (1000) eric      (1000)        0 2024-05-18 05:09:35.372169 bank_scrapers-1.0.7/
+-rw-rw-r--   0 eric      (1000) eric      (1000)     1066 2024-05-16 09:36:03.000000 bank_scrapers-1.0.7/LICENSE
+-rw-r--r--   0 eric      (1000) eric      (1000)    22430 2024-05-18 05:09:35.372169 bank_scrapers-1.0.7/PKG-INFO
+-rw-rw-r--   0 eric      (1000) eric      (1000)    20665 2024-05-16 09:36:03.000000 bank_scrapers-1.0.7/README.md
+drwxrwxr-x   0 eric      (1000) eric      (1000)        0 2024-05-18 05:09:35.369169 bank_scrapers-1.0.7/bank_scrapers/
+-rw-rw-r--   0 eric      (1000) eric      (1000)      307 2024-05-18 05:07:40.000000 bank_scrapers-1.0.7/bank_scrapers/__init__.py
+drwxrwxr-x   0 eric      (1000) eric      (1000)        0 2024-05-18 05:09:35.370169 bank_scrapers-1.0.7/bank_scrapers/api_wrappers/
+-rw-rw-r--   0 eric      (1000) eric      (1000)        0 2024-05-16 09:36:03.000000 bank_scrapers-1.0.7/bank_scrapers/api_wrappers/__init__.py
+drwxrwxr-x   0 eric      (1000) eric      (1000)        0 2024-05-18 05:09:35.370169 bank_scrapers-1.0.7/bank_scrapers/api_wrappers/kraken/
+-rw-rw-r--   0 eric      (1000) eric      (1000)        0 2024-05-16 09:36:03.000000 bank_scrapers-1.0.7/bank_scrapers/api_wrappers/kraken/__init__.py
+-rw-rw-r--   0 eric      (1000) eric      (1000)     2863 2024-05-16 09:36:03.000000 bank_scrapers-1.0.7/bank_scrapers/api_wrappers/kraken/driver.py
+drwxrwxr-x   0 eric      (1000) eric      (1000)        0 2024-05-18 05:09:35.370169 bank_scrapers-1.0.7/bank_scrapers/cli/
+-rw-rw-r--   0 eric      (1000) eric      (1000)        0 2024-05-16 09:36:03.000000 bank_scrapers-1.0.7/bank_scrapers/cli/__init__.py
+-rw-rw-r--   0 eric      (1000) eric      (1000)     9027 2024-05-16 09:36:03.000000 bank_scrapers-1.0.7/bank_scrapers/cli/cli.py
+drwxrwxr-x   0 eric      (1000) eric      (1000)        0 2024-05-18 05:09:35.370169 bank_scrapers-1.0.7/bank_scrapers/common/
+-rw-rw-r--   0 eric      (1000) eric      (1000)        0 2024-05-16 09:36:03.000000 bank_scrapers-1.0.7/bank_scrapers/common/__init__.py
+-rw-rw-r--   0 eric      (1000) eric      (1000)      272 2024-05-16 09:36:03.000000 bank_scrapers-1.0.7/bank_scrapers/common/log.py
+drwxrwxr-x   0 eric      (1000) eric      (1000)        0 2024-05-18 05:09:35.370169 bank_scrapers-1.0.7/bank_scrapers/scrapers/
+-rw-rw-r--   0 eric      (1000) eric      (1000)        0 2024-05-16 09:36:03.000000 bank_scrapers-1.0.7/bank_scrapers/scrapers/__init__.py
+drwxrwxr-x   0 eric      (1000) eric      (1000)        0 2024-05-18 05:09:35.370169 bank_scrapers-1.0.7/bank_scrapers/scrapers/becu/
+-rw-rw-r--   0 eric      (1000) eric      (1000)        0 2024-05-16 09:36:03.000000 bank_scrapers-1.0.7/bank_scrapers/scrapers/becu/__init__.py
+-rw-rw-r--   0 eric      (1000) eric      (1000)     6910 2024-05-18 04:44:12.000000 bank_scrapers-1.0.7/bank_scrapers/scrapers/becu/driver.py
+drwxrwxr-x   0 eric      (1000) eric      (1000)        0 2024-05-18 05:09:35.370169 bank_scrapers-1.0.7/bank_scrapers/scrapers/chase/
+-rw-rw-r--   0 eric      (1000) eric      (1000)        0 2024-05-16 09:36:03.000000 bank_scrapers-1.0.7/bank_scrapers/scrapers/chase/__init__.py
+-rw-rw-r--   0 eric      (1000) eric      (1000)     9191 2024-05-16 09:36:03.000000 bank_scrapers-1.0.7/bank_scrapers/scrapers/chase/driver.py
+drwxrwxr-x   0 eric      (1000) eric      (1000)        0 2024-05-18 05:09:35.371169 bank_scrapers-1.0.7/bank_scrapers/scrapers/common/
+-rw-rw-r--   0 eric      (1000) eric      (1000)        0 2024-05-16 09:36:03.000000 bank_scrapers-1.0.7/bank_scrapers/scrapers/common/__init__.py
+-rw-rw-r--   0 eric      (1000) eric      (1000)     4712 2024-05-16 09:36:03.000000 bank_scrapers-1.0.7/bank_scrapers/scrapers/common/functions.py
+drwxrwxr-x   0 eric      (1000) eric      (1000)        0 2024-05-18 05:09:35.371169 bank_scrapers-1.0.7/bank_scrapers/scrapers/fidelity_netbenefits/
+-rw-rw-r--   0 eric      (1000) eric      (1000)        0 2024-05-16 09:36:03.000000 bank_scrapers-1.0.7/bank_scrapers/scrapers/fidelity_netbenefits/__init__.py
+-rw-rw-r--   0 eric      (1000) eric      (1000)     8335 2024-05-16 09:36:03.000000 bank_scrapers-1.0.7/bank_scrapers/scrapers/fidelity_netbenefits/driver.py
+drwxrwxr-x   0 eric      (1000) eric      (1000)        0 2024-05-18 05:09:35.371169 bank_scrapers-1.0.7/bank_scrapers/scrapers/roundpoint/
+-rw-rw-r--   0 eric      (1000) eric      (1000)        0 2024-05-16 09:36:03.000000 bank_scrapers-1.0.7/bank_scrapers/scrapers/roundpoint/__init__.py
+-rw-rw-r--   0 eric      (1000) eric      (1000)     8626 2024-05-16 09:36:03.000000 bank_scrapers-1.0.7/bank_scrapers/scrapers/roundpoint/driver.py
+drwxrwxr-x   0 eric      (1000) eric      (1000)        0 2024-05-18 05:09:35.371169 bank_scrapers-1.0.7/bank_scrapers/scrapers/smbc_prestia/
+-rw-rw-r--   0 eric      (1000) eric      (1000)        0 2024-05-16 09:36:03.000000 bank_scrapers-1.0.7/bank_scrapers/scrapers/smbc_prestia/__init__.py
+-rw-rw-r--   0 eric      (1000) eric      (1000)     4632 2024-05-16 09:36:03.000000 bank_scrapers-1.0.7/bank_scrapers/scrapers/smbc_prestia/driver.py
+drwxrwxr-x   0 eric      (1000) eric      (1000)        0 2024-05-18 05:09:35.371169 bank_scrapers-1.0.7/bank_scrapers/scrapers/uhfcu/
+-rw-rw-r--   0 eric      (1000) eric      (1000)        0 2024-05-16 09:36:03.000000 bank_scrapers-1.0.7/bank_scrapers/scrapers/uhfcu/__init__.py
+-rw-rw-r--   0 eric      (1000) eric      (1000)     8655 2024-05-16 09:36:03.000000 bank_scrapers-1.0.7/bank_scrapers/scrapers/uhfcu/driver.py
+drwxrwxr-x   0 eric      (1000) eric      (1000)        0 2024-05-18 05:09:35.371169 bank_scrapers-1.0.7/bank_scrapers/scrapers/vanguard/
+-rw-rw-r--   0 eric      (1000) eric      (1000)        0 2024-05-16 09:36:03.000000 bank_scrapers-1.0.7/bank_scrapers/scrapers/vanguard/__init__.py
+-rw-rw-r--   0 eric      (1000) eric      (1000)     7740 2024-05-16 09:36:03.000000 bank_scrapers-1.0.7/bank_scrapers/scrapers/vanguard/driver.py
+drwxrwxr-x   0 eric      (1000) eric      (1000)        0 2024-05-18 05:09:35.372169 bank_scrapers-1.0.7/bank_scrapers/scrapers/zillow/
+-rw-rw-r--   0 eric      (1000) eric      (1000)        0 2024-05-16 09:36:03.000000 bank_scrapers-1.0.7/bank_scrapers/scrapers/zillow/__init__.py
+-rw-rw-r--   0 eric      (1000) eric      (1000)     3457 2024-05-16 09:36:03.000000 bank_scrapers-1.0.7/bank_scrapers/scrapers/zillow/driver.py
+drwxrwxr-x   0 eric      (1000) eric      (1000)        0 2024-05-18 05:09:35.372169 bank_scrapers-1.0.7/bank_scrapers.egg-info/
+-rw-r--r--   0 eric      (1000) eric      (1000)    22430 2024-05-18 05:09:35.000000 bank_scrapers-1.0.7/bank_scrapers.egg-info/PKG-INFO
+-rw-rw-r--   0 eric      (1000) eric      (1000)     1347 2024-05-18 05:09:35.000000 bank_scrapers-1.0.7/bank_scrapers.egg-info/SOURCES.txt
+-rw-rw-r--   0 eric      (1000) eric      (1000)        1 2024-05-18 05:09:35.000000 bank_scrapers-1.0.7/bank_scrapers.egg-info/dependency_links.txt
+-rw-rw-r--   0 eric      (1000) eric      (1000)       59 2024-05-18 05:09:35.000000 bank_scrapers-1.0.7/bank_scrapers.egg-info/entry_points.txt
+-rw-rw-r--   0 eric      (1000) eric      (1000)      128 2024-05-18 05:09:35.000000 bank_scrapers-1.0.7/bank_scrapers.egg-info/requires.txt
+-rw-rw-r--   0 eric      (1000) eric      (1000)       14 2024-05-18 05:09:35.000000 bank_scrapers-1.0.7/bank_scrapers.egg-info/top_level.txt
+-rw-rw-r--   0 eric      (1000) eric      (1000)      962 2024-05-18 05:07:40.000000 bank_scrapers-1.0.7/pyproject.toml
+-rw-rw-r--   0 eric      (1000) eric      (1000)       38 2024-05-18 05:09:35.372169 bank_scrapers-1.0.7/setup.cfg
```

### Comparing `bank_scrapers-1.0.6/LICENSE` & `bank_scrapers-1.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `bank_scrapers-1.0.6/PKG-INFO` & `bank_scrapers-1.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bank_scrapers
-Version: 1.0.6
+Version: 1.0.7
 Summary: Library for working with bank_scrapers drivers.
 Author: Eric Bette
 License: MIT License
         
         Copyright (c) 2023 Eric Bette
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -31,15 +31,14 @@
 Requires-Dist: beautifulsoup4>=4.12.2
 Requires-Dist: pandas>=2.0.2
 Requires-Dist: requests>=2.31.0
 Requires-Dist: undetected-chromedriver>=3.5.0
 Requires-Dist: lxml>=4.9.2
 Requires-Dist: setuptools>=69.5.1
 Requires-Dist: lxml>=5.2.2
-Requires-Dist: bank_scrapers==1.0.6
 
 # Table of Contents
 <!-- START doctoc generated TOC please keep comment here to allow auto update -->
 <!-- DON'T EDIT THIS SECTION, INSTEAD RE-RUN doctoc TO UPDATE -->
 
 - [Introduction](#introduction)
 - [Getting Started](#getting-started)
```

### Comparing `bank_scrapers-1.0.6/README.md` & `bank_scrapers-1.0.7/README.md`

 * *Files identical despite different names*

### Comparing `bank_scrapers-1.0.6/bank_scrapers/api_wrappers/kraken/driver.py` & `bank_scrapers-1.0.7/bank_scrapers/api_wrappers/kraken/driver.py`

 * *Files identical despite different names*

### Comparing `bank_scrapers-1.0.6/bank_scrapers/cli/cli.py` & `bank_scrapers-1.0.7/bank_scrapers/cli/cli.py`

 * *Files identical despite different names*

### Comparing `bank_scrapers-1.0.6/bank_scrapers/scrapers/becu/driver.py` & `bank_scrapers-1.0.7/bank_scrapers/scrapers/becu/driver.py`

 * *Files identical despite different names*

### Comparing `bank_scrapers-1.0.6/bank_scrapers/scrapers/chase/driver.py` & `bank_scrapers-1.0.7/bank_scrapers/scrapers/chase/driver.py`

 * *Files identical despite different names*

### Comparing `bank_scrapers-1.0.6/bank_scrapers/scrapers/common/functions.py` & `bank_scrapers-1.0.7/bank_scrapers/scrapers/common/functions.py`

 * *Files identical despite different names*

### Comparing `bank_scrapers-1.0.6/bank_scrapers/scrapers/fidelity_netbenefits/driver.py` & `bank_scrapers-1.0.7/bank_scrapers/scrapers/fidelity_netbenefits/driver.py`

 * *Files identical despite different names*

### Comparing `bank_scrapers-1.0.6/bank_scrapers/scrapers/roundpoint/driver.py` & `bank_scrapers-1.0.7/bank_scrapers/scrapers/roundpoint/driver.py`

 * *Files identical despite different names*

### Comparing `bank_scrapers-1.0.6/bank_scrapers/scrapers/smbc_prestia/driver.py` & `bank_scrapers-1.0.7/bank_scrapers/scrapers/smbc_prestia/driver.py`

 * *Files identical despite different names*

### Comparing `bank_scrapers-1.0.6/bank_scrapers/scrapers/uhfcu/driver.py` & `bank_scrapers-1.0.7/bank_scrapers/scrapers/uhfcu/driver.py`

 * *Files identical despite different names*

### Comparing `bank_scrapers-1.0.6/bank_scrapers/scrapers/vanguard/driver.py` & `bank_scrapers-1.0.7/bank_scrapers/scrapers/vanguard/driver.py`

 * *Files identical despite different names*

### Comparing `bank_scrapers-1.0.6/bank_scrapers/scrapers/zillow/driver.py` & `bank_scrapers-1.0.7/bank_scrapers/scrapers/zillow/driver.py`

 * *Files identical despite different names*

### Comparing `bank_scrapers-1.0.6/bank_scrapers.egg-info/PKG-INFO` & `bank_scrapers-1.0.7/bank_scrapers.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bank_scrapers
-Version: 1.0.6
+Version: 1.0.7
 Summary: Library for working with bank_scrapers drivers.
 Author: Eric Bette
 License: MIT License
         
         Copyright (c) 2023 Eric Bette
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -31,15 +31,14 @@
 Requires-Dist: beautifulsoup4>=4.12.2
 Requires-Dist: pandas>=2.0.2
 Requires-Dist: requests>=2.31.0
 Requires-Dist: undetected-chromedriver>=3.5.0
 Requires-Dist: lxml>=4.9.2
 Requires-Dist: setuptools>=69.5.1
 Requires-Dist: lxml>=5.2.2
-Requires-Dist: bank_scrapers==1.0.6
 
 # Table of Contents
 <!-- START doctoc generated TOC please keep comment here to allow auto update -->
 <!-- DON'T EDIT THIS SECTION, INSTEAD RE-RUN doctoc TO UPDATE -->
 
 - [Introduction](#introduction)
 - [Getting Started](#getting-started)
```

### Comparing `bank_scrapers-1.0.6/bank_scrapers.egg-info/SOURCES.txt` & `bank_scrapers-1.0.7/bank_scrapers.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bank_scrapers-1.0.6/pyproject.toml` & `bank_scrapers-1.0.7/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -16,16 +16,15 @@
 dependencies = [
     "beautifulsoup4>=4.12.2",
     "pandas>=2.0.2",
     "requests>=2.31.0",
     "undetected-chromedriver>=3.5.0",
     "lxml>=4.9.2",
     "setuptools>=69.5.1",
-    "lxml>=5.2.2",
-    "bank_scrapers==1.0.6"
+    "lxml>=5.2.2"
 
 ]
 
 [project.urls]
 homepage = "https://github.com/eebette/bank_scrapers/tree/master"
 
 [project.scripts]
```

