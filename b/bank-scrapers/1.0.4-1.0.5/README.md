# Comparing `tmp/bank_scrapers-1.0.4.tar.gz` & `tmp/bank_scrapers-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bank_scrapers-1.0.4.tar", last modified: Tue Jun 20 11:13:08 2023, max compression
+gzip compressed data, was "bank_scrapers-1.0.5.tar", last modified: Sat May 18 04:46:39 2024, max compression
```

## Comparing `bank_scrapers-1.0.4.tar` & `bank_scrapers-1.0.5.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxrwxr-x   0 eric      (1000) eric      (1000)        0 2023-06-20 11:13:08.967790 bank_scrapers-1.0.4/
--rw-rw-r--   0 eric      (1000) eric      (1000)     1066 2023-06-18 06:33:32.000000 bank_scrapers-1.0.4/LICENSE
--rw-rw-r--   0 eric      (1000) eric      (1000)    22197 2023-06-20 11:13:08.967790 bank_scrapers-1.0.4/PKG-INFO
--rw-rw-r--   0 eric      (1000) eric      (1000)    20665 2023-06-20 11:10:36.000000 bank_scrapers-1.0.4/README.md
-drwxrwxr-x   0 eric      (1000) eric      (1000)        0 2023-06-20 11:13:08.967790 bank_scrapers-1.0.4/bank_scrapers/
--rw-rw-r--   0 eric      (1000) eric      (1000)      476 2023-06-20 11:12:39.000000 bank_scrapers-1.0.4/bank_scrapers/__init__.py
-drwxrwxr-x   0 eric      (1000) eric      (1000)        0 2023-06-20 11:13:08.967790 bank_scrapers-1.0.4/bank_scrapers/api_wrappers/
--rw-rw-r--   0 eric      (1000) eric      (1000)        0 2023-06-12 11:03:00.000000 bank_scrapers-1.0.4/bank_scrapers/api_wrappers/__init__.py
-drwxrwxr-x   0 eric      (1000) eric      (1000)        0 2023-06-20 11:13:08.967790 bank_scrapers-1.0.4/bank_scrapers/api_wrappers/kraken/
--rw-rw-r--   0 eric      (1000) eric      (1000)        0 2023-06-12 11:03:11.000000 bank_scrapers-1.0.4/bank_scrapers/api_wrappers/kraken/__init__.py
--rw-rw-r--   0 eric      (1000) eric      (1000)     2863 2023-06-17 11:54:24.000000 bank_scrapers-1.0.4/bank_scrapers/api_wrappers/kraken/driver.py
-drwxrwxr-x   0 eric      (1000) eric      (1000)        0 2023-06-20 11:13:08.967790 bank_scrapers-1.0.4/bank_scrapers/cli/
--rw-rw-r--   0 eric      (1000) eric      (1000)        0 2023-06-18 04:02:26.000000 bank_scrapers-1.0.4/bank_scrapers/cli/__init__.py
--rw-rw-r--   0 eric      (1000) eric      (1000)     9027 2023-06-18 08:52:15.000000 bank_scrapers-1.0.4/bank_scrapers/cli/cli.py
-drwxrwxr-x   0 eric      (1000) eric      (1000)        0 2023-06-20 11:13:08.967790 bank_scrapers-1.0.4/bank_scrapers/common/
--rw-rw-r--   0 eric      (1000) eric      (1000)        0 2023-06-18 04:04:49.000000 bank_scrapers-1.0.4/bank_scrapers/common/__init__.py
--rw-rw-r--   0 eric      (1000) eric      (1000)      272 2023-06-18 04:49:40.000000 bank_scrapers-1.0.4/bank_scrapers/common/log.py
-drwxrwxr-x   0 eric      (1000) eric      (1000)        0 2023-06-20 11:13:08.967790 bank_scrapers-1.0.4/bank_scrapers/scrapers/
--rw-rw-r--   0 eric      (1000) eric      (1000)        0 2023-06-11 08:17:21.000000 bank_scrapers-1.0.4/bank_scrapers/scrapers/__init__.py
-drwxrwxr-x   0 eric      (1000) eric      (1000)        0 2023-06-20 11:13:08.967790 bank_scrapers-1.0.4/bank_scrapers/scrapers/becu/
--rw-rw-r--   0 eric      (1000) eric      (1000)        0 2023-06-11 08:18:17.000000 bank_scrapers-1.0.4/bank_scrapers/scrapers/becu/__init__.py
--rw-rw-r--   0 eric      (1000) eric      (1000)     4284 2023-06-18 08:44:27.000000 bank_scrapers-1.0.4/bank_scrapers/scrapers/becu/driver.py
-drwxrwxr-x   0 eric      (1000) eric      (1000)        0 2023-06-20 11:13:08.967790 bank_scrapers-1.0.4/bank_scrapers/scrapers/chase/
--rw-rw-r--   0 eric      (1000) eric      (1000)        0 2023-06-11 08:18:17.000000 bank_scrapers-1.0.4/bank_scrapers/scrapers/chase/__init__.py
--rw-rw-r--   0 eric      (1000) eric      (1000)     9191 2023-06-19 14:19:32.000000 bank_scrapers-1.0.4/bank_scrapers/scrapers/chase/driver.py
-drwxrwxr-x   0 eric      (1000) eric      (1000)        0 2023-06-20 11:13:08.967790 bank_scrapers-1.0.4/bank_scrapers/scrapers/common/
--rw-rw-r--   0 eric      (1000) eric      (1000)        0 2023-06-11 08:48:23.000000 bank_scrapers-1.0.4/bank_scrapers/scrapers/common/__init__.py
--rw-rw-r--   0 eric      (1000) eric      (1000)     4712 2023-06-20 11:11:51.000000 bank_scrapers-1.0.4/bank_scrapers/scrapers/common/functions.py
-drwxrwxr-x   0 eric      (1000) eric      (1000)        0 2023-06-20 11:13:08.967790 bank_scrapers-1.0.4/bank_scrapers/scrapers/fidelity_netbenefits/
--rw-rw-r--   0 eric      (1000) eric      (1000)        0 2023-06-11 08:18:17.000000 bank_scrapers-1.0.4/bank_scrapers/scrapers/fidelity_netbenefits/__init__.py
--rw-rw-r--   0 eric      (1000) eric      (1000)     8335 2023-06-18 14:10:29.000000 bank_scrapers-1.0.4/bank_scrapers/scrapers/fidelity_netbenefits/driver.py
-drwxrwxr-x   0 eric      (1000) eric      (1000)        0 2023-06-20 11:13:08.967790 bank_scrapers-1.0.4/bank_scrapers/scrapers/roundpoint/
--rw-rw-r--   0 eric      (1000) eric      (1000)        0 2023-06-11 08:18:17.000000 bank_scrapers-1.0.4/bank_scrapers/scrapers/roundpoint/__init__.py
--rw-rw-r--   0 eric      (1000) eric      (1000)     8626 2023-06-18 14:25:51.000000 bank_scrapers-1.0.4/bank_scrapers/scrapers/roundpoint/driver.py
-drwxrwxr-x   0 eric      (1000) eric      (1000)        0 2023-06-20 11:13:08.967790 bank_scrapers-1.0.4/bank_scrapers/scrapers/smbc_prestia/
--rw-rw-r--   0 eric      (1000) eric      (1000)        0 2023-06-11 08:18:17.000000 bank_scrapers-1.0.4/bank_scrapers/scrapers/smbc_prestia/__init__.py
--rw-rw-r--   0 eric      (1000) eric      (1000)     4632 2023-06-20 10:44:36.000000 bank_scrapers-1.0.4/bank_scrapers/scrapers/smbc_prestia/driver.py
-drwxrwxr-x   0 eric      (1000) eric      (1000)        0 2023-06-20 11:13:08.967790 bank_scrapers-1.0.4/bank_scrapers/scrapers/uhfcu/
--rw-rw-r--   0 eric      (1000) eric      (1000)        0 2023-06-11 08:18:17.000000 bank_scrapers-1.0.4/bank_scrapers/scrapers/uhfcu/__init__.py
--rw-rw-r--   0 eric      (1000) eric      (1000)     8655 2023-06-20 10:47:15.000000 bank_scrapers-1.0.4/bank_scrapers/scrapers/uhfcu/driver.py
-drwxrwxr-x   0 eric      (1000) eric      (1000)        0 2023-06-20 11:13:08.967790 bank_scrapers-1.0.4/bank_scrapers/scrapers/vanguard/
--rw-rw-r--   0 eric      (1000) eric      (1000)        0 2023-06-11 08:18:17.000000 bank_scrapers-1.0.4/bank_scrapers/scrapers/vanguard/__init__.py
--rw-rw-r--   0 eric      (1000) eric      (1000)     7740 2023-06-20 10:47:15.000000 bank_scrapers-1.0.4/bank_scrapers/scrapers/vanguard/driver.py
-drwxrwxr-x   0 eric      (1000) eric      (1000)        0 2023-06-20 11:13:08.967790 bank_scrapers-1.0.4/bank_scrapers/scrapers/zillow/
--rw-rw-r--   0 eric      (1000) eric      (1000)        0 2023-06-11 08:18:17.000000 bank_scrapers-1.0.4/bank_scrapers/scrapers/zillow/__init__.py
--rw-rw-r--   0 eric      (1000) eric      (1000)     3457 2023-06-18 08:44:27.000000 bank_scrapers-1.0.4/bank_scrapers/scrapers/zillow/driver.py
-drwxrwxr-x   0 eric      (1000) eric      (1000)        0 2023-06-20 11:13:08.967790 bank_scrapers-1.0.4/bank_scrapers.egg-info/
--rw-rw-r--   0 eric      (1000) eric      (1000)    22197 2023-06-20 11:13:08.000000 bank_scrapers-1.0.4/bank_scrapers.egg-info/PKG-INFO
--rw-rw-r--   0 eric      (1000) eric      (1000)     1347 2023-06-20 11:13:08.000000 bank_scrapers-1.0.4/bank_scrapers.egg-info/SOURCES.txt
--rw-rw-r--   0 eric      (1000) eric      (1000)        1 2023-06-20 11:13:08.000000 bank_scrapers-1.0.4/bank_scrapers.egg-info/dependency_links.txt
--rw-rw-r--   0 eric      (1000) eric      (1000)       59 2023-06-20 11:13:08.000000 bank_scrapers-1.0.4/bank_scrapers.egg-info/entry_points.txt
--rw-rw-r--   0 eric      (1000) eric      (1000)      118 2023-06-20 11:13:08.000000 bank_scrapers-1.0.4/bank_scrapers.egg-info/requires.txt
--rw-rw-r--   0 eric      (1000) eric      (1000)       14 2023-06-20 11:13:08.000000 bank_scrapers-1.0.4/bank_scrapers.egg-info/top_level.txt
--rw-rw-r--   0 eric      (1000) eric      (1000)      945 2023-06-20 11:12:39.000000 bank_scrapers-1.0.4/pyproject.toml
--rw-rw-r--   0 eric      (1000) eric      (1000)       38 2023-06-20 11:13:08.967790 bank_scrapers-1.0.4/setup.cfg
+drwxrwxr-x   0 eric      (1000) eric      (1000)        0 2024-05-18 04:46:39.327688 bank_scrapers-1.0.5/
+-rw-rw-r--   0 eric      (1000) eric      (1000)     1066 2024-05-16 09:36:03.000000 bank_scrapers-1.0.5/LICENSE
+-rw-r--r--   0 eric      (1000) eric      (1000)    22466 2024-05-18 04:46:39.327688 bank_scrapers-1.0.5/PKG-INFO
+-rw-rw-r--   0 eric      (1000) eric      (1000)    20665 2024-05-16 09:36:03.000000 bank_scrapers-1.0.5/README.md
+drwxrwxr-x   0 eric      (1000) eric      (1000)        0 2024-05-18 04:46:39.324688 bank_scrapers-1.0.5/bank_scrapers/
+-rw-rw-r--   0 eric      (1000) eric      (1000)      307 2024-05-18 04:27:09.000000 bank_scrapers-1.0.5/bank_scrapers/__init__.py
+drwxrwxr-x   0 eric      (1000) eric      (1000)        0 2024-05-18 04:46:39.325688 bank_scrapers-1.0.5/bank_scrapers/api_wrappers/
+-rw-rw-r--   0 eric      (1000) eric      (1000)        0 2024-05-16 09:36:03.000000 bank_scrapers-1.0.5/bank_scrapers/api_wrappers/__init__.py
+drwxrwxr-x   0 eric      (1000) eric      (1000)        0 2024-05-18 04:46:39.325688 bank_scrapers-1.0.5/bank_scrapers/api_wrappers/kraken/
+-rw-rw-r--   0 eric      (1000) eric      (1000)        0 2024-05-16 09:36:03.000000 bank_scrapers-1.0.5/bank_scrapers/api_wrappers/kraken/__init__.py
+-rw-rw-r--   0 eric      (1000) eric      (1000)     2863 2024-05-16 09:36:03.000000 bank_scrapers-1.0.5/bank_scrapers/api_wrappers/kraken/driver.py
+drwxrwxr-x   0 eric      (1000) eric      (1000)        0 2024-05-18 04:46:39.325688 bank_scrapers-1.0.5/bank_scrapers/cli/
+-rw-rw-r--   0 eric      (1000) eric      (1000)        0 2024-05-16 09:36:03.000000 bank_scrapers-1.0.5/bank_scrapers/cli/__init__.py
+-rw-rw-r--   0 eric      (1000) eric      (1000)     9027 2024-05-16 09:36:03.000000 bank_scrapers-1.0.5/bank_scrapers/cli/cli.py
+drwxrwxr-x   0 eric      (1000) eric      (1000)        0 2024-05-18 04:46:39.325688 bank_scrapers-1.0.5/bank_scrapers/common/
+-rw-rw-r--   0 eric      (1000) eric      (1000)        0 2024-05-16 09:36:03.000000 bank_scrapers-1.0.5/bank_scrapers/common/__init__.py
+-rw-rw-r--   0 eric      (1000) eric      (1000)      272 2024-05-16 09:36:03.000000 bank_scrapers-1.0.5/bank_scrapers/common/log.py
+drwxrwxr-x   0 eric      (1000) eric      (1000)        0 2024-05-18 04:46:39.325688 bank_scrapers-1.0.5/bank_scrapers/scrapers/
+-rw-rw-r--   0 eric      (1000) eric      (1000)        0 2024-05-16 09:36:03.000000 bank_scrapers-1.0.5/bank_scrapers/scrapers/__init__.py
+drwxrwxr-x   0 eric      (1000) eric      (1000)        0 2024-05-18 04:46:39.326688 bank_scrapers-1.0.5/bank_scrapers/scrapers/becu/
+-rw-rw-r--   0 eric      (1000) eric      (1000)        0 2024-05-16 09:36:03.000000 bank_scrapers-1.0.5/bank_scrapers/scrapers/becu/__init__.py
+-rw-rw-r--   0 eric      (1000) eric      (1000)     6910 2024-05-18 04:44:12.000000 bank_scrapers-1.0.5/bank_scrapers/scrapers/becu/driver.py
+drwxrwxr-x   0 eric      (1000) eric      (1000)        0 2024-05-18 04:46:39.326688 bank_scrapers-1.0.5/bank_scrapers/scrapers/chase/
+-rw-rw-r--   0 eric      (1000) eric      (1000)        0 2024-05-16 09:36:03.000000 bank_scrapers-1.0.5/bank_scrapers/scrapers/chase/__init__.py
+-rw-rw-r--   0 eric      (1000) eric      (1000)     9191 2024-05-16 09:36:03.000000 bank_scrapers-1.0.5/bank_scrapers/scrapers/chase/driver.py
+drwxrwxr-x   0 eric      (1000) eric      (1000)        0 2024-05-18 04:46:39.326688 bank_scrapers-1.0.5/bank_scrapers/scrapers/common/
+-rw-rw-r--   0 eric      (1000) eric      (1000)        0 2024-05-16 09:36:03.000000 bank_scrapers-1.0.5/bank_scrapers/scrapers/common/__init__.py
+-rw-rw-r--   0 eric      (1000) eric      (1000)     4712 2024-05-16 09:36:03.000000 bank_scrapers-1.0.5/bank_scrapers/scrapers/common/functions.py
+drwxrwxr-x   0 eric      (1000) eric      (1000)        0 2024-05-18 04:46:39.326688 bank_scrapers-1.0.5/bank_scrapers/scrapers/fidelity_netbenefits/
+-rw-rw-r--   0 eric      (1000) eric      (1000)        0 2024-05-16 09:36:03.000000 bank_scrapers-1.0.5/bank_scrapers/scrapers/fidelity_netbenefits/__init__.py
+-rw-rw-r--   0 eric      (1000) eric      (1000)     8335 2024-05-16 09:36:03.000000 bank_scrapers-1.0.5/bank_scrapers/scrapers/fidelity_netbenefits/driver.py
+drwxrwxr-x   0 eric      (1000) eric      (1000)        0 2024-05-18 04:46:39.326688 bank_scrapers-1.0.5/bank_scrapers/scrapers/roundpoint/
+-rw-rw-r--   0 eric      (1000) eric      (1000)        0 2024-05-16 09:36:03.000000 bank_scrapers-1.0.5/bank_scrapers/scrapers/roundpoint/__init__.py
+-rw-rw-r--   0 eric      (1000) eric      (1000)     8626 2024-05-16 09:36:03.000000 bank_scrapers-1.0.5/bank_scrapers/scrapers/roundpoint/driver.py
+drwxrwxr-x   0 eric      (1000) eric      (1000)        0 2024-05-18 04:46:39.326688 bank_scrapers-1.0.5/bank_scrapers/scrapers/smbc_prestia/
+-rw-rw-r--   0 eric      (1000) eric      (1000)        0 2024-05-16 09:36:03.000000 bank_scrapers-1.0.5/bank_scrapers/scrapers/smbc_prestia/__init__.py
+-rw-rw-r--   0 eric      (1000) eric      (1000)     4632 2024-05-16 09:36:03.000000 bank_scrapers-1.0.5/bank_scrapers/scrapers/smbc_prestia/driver.py
+drwxrwxr-x   0 eric      (1000) eric      (1000)        0 2024-05-18 04:46:39.327688 bank_scrapers-1.0.5/bank_scrapers/scrapers/uhfcu/
+-rw-rw-r--   0 eric      (1000) eric      (1000)        0 2024-05-16 09:36:03.000000 bank_scrapers-1.0.5/bank_scrapers/scrapers/uhfcu/__init__.py
+-rw-rw-r--   0 eric      (1000) eric      (1000)     8655 2024-05-16 09:36:03.000000 bank_scrapers-1.0.5/bank_scrapers/scrapers/uhfcu/driver.py
+drwxrwxr-x   0 eric      (1000) eric      (1000)        0 2024-05-18 04:46:39.327688 bank_scrapers-1.0.5/bank_scrapers/scrapers/vanguard/
+-rw-rw-r--   0 eric      (1000) eric      (1000)        0 2024-05-16 09:36:03.000000 bank_scrapers-1.0.5/bank_scrapers/scrapers/vanguard/__init__.py
+-rw-rw-r--   0 eric      (1000) eric      (1000)     7740 2024-05-16 09:36:03.000000 bank_scrapers-1.0.5/bank_scrapers/scrapers/vanguard/driver.py
+drwxrwxr-x   0 eric      (1000) eric      (1000)        0 2024-05-18 04:46:39.327688 bank_scrapers-1.0.5/bank_scrapers/scrapers/zillow/
+-rw-rw-r--   0 eric      (1000) eric      (1000)        0 2024-05-16 09:36:03.000000 bank_scrapers-1.0.5/bank_scrapers/scrapers/zillow/__init__.py
+-rw-rw-r--   0 eric      (1000) eric      (1000)     3457 2024-05-16 09:36:03.000000 bank_scrapers-1.0.5/bank_scrapers/scrapers/zillow/driver.py
+drwxrwxr-x   0 eric      (1000) eric      (1000)        0 2024-05-18 04:46:39.327688 bank_scrapers-1.0.5/bank_scrapers.egg-info/
+-rw-r--r--   0 eric      (1000) eric      (1000)    22466 2024-05-18 04:46:39.000000 bank_scrapers-1.0.5/bank_scrapers.egg-info/PKG-INFO
+-rw-rw-r--   0 eric      (1000) eric      (1000)     1347 2024-05-18 04:46:39.000000 bank_scrapers-1.0.5/bank_scrapers.egg-info/SOURCES.txt
+-rw-rw-r--   0 eric      (1000) eric      (1000)        1 2024-05-18 04:46:39.000000 bank_scrapers-1.0.5/bank_scrapers.egg-info/dependency_links.txt
+-rw-rw-r--   0 eric      (1000) eric      (1000)       59 2024-05-18 04:46:39.000000 bank_scrapers-1.0.5/bank_scrapers.egg-info/entry_points.txt
+-rw-rw-r--   0 eric      (1000) eric      (1000)      149 2024-05-18 04:46:39.000000 bank_scrapers-1.0.5/bank_scrapers.egg-info/requires.txt
+-rw-rw-r--   0 eric      (1000) eric      (1000)       14 2024-05-18 04:46:39.000000 bank_scrapers-1.0.5/bank_scrapers.egg-info/top_level.txt
+-rw-rw-r--   0 eric      (1000) eric      (1000)      990 2024-05-16 10:49:44.000000 bank_scrapers-1.0.5/pyproject.toml
+-rw-rw-r--   0 eric      (1000) eric      (1000)       38 2024-05-18 04:46:39.327688 bank_scrapers-1.0.5/setup.cfg
```

### Comparing `bank_scrapers-1.0.4/LICENSE` & `bank_scrapers-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `bank_scrapers-1.0.4/PKG-INFO` & `bank_scrapers-1.0.5/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,38 +1,7 @@
-Metadata-Version: 2.1
-Name: bank_scrapers
-Version: 1.0.4
-Summary: Library for working with bank_scrapers drivers.
-Author: Eric Bette
-License: MIT License
-        
-        Copyright (c) 2023 Eric Bette
-        
-        Permission is hereby granted, free of charge, to any person obtaining a copy
-        of this software and associated documentation files (the "Software"), to deal
-        in the Software without restriction, including without limitation the rights
-        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-        copies of the Software, and to permit persons to whom the Software is
-        furnished to do so, subject to the following conditions:
-        
-        The above copyright notice and this permission notice shall be included in all
-        copies or substantial portions of the Software.
-        
-        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-        SOFTWARE.
-Project-URL: homepage, https://github.com/eebette/bank_scrapers/tree/master
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # Table of Contents
 <!-- START doctoc generated TOC please keep comment here to allow auto update -->
 <!-- DON'T EDIT THIS SECTION, INSTEAD RE-RUN doctoc TO UPDATE -->
 
 - [Introduction](#introduction)
 - [Getting Started](#getting-started)
   - [Installation](#installation)
@@ -714,8 +683,8 @@
 production use, nefarious or otherwise.
 
 Usage of this code is potentially against your bank's terms of service and could result in you or your IP getting
 flagged, listed, or blocked as bad actors. I don't take any responsibility for any effects this code may have on your
 bank accounts or your relationships with your banking institutions.
 
 Please don't try to learn anything about me or my life based on the banks that I've arbitrarily decided to write
-drivers for. 
+drivers for.
```

### Comparing `bank_scrapers-1.0.4/README.md` & `bank_scrapers-1.0.5/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,7 +1,46 @@
+Metadata-Version: 2.1
+Name: bank_scrapers
+Version: 1.0.5
+Summary: Library for working with bank_scrapers drivers.
+Author: Eric Bette
+License: MIT License
+        
+        Copyright (c) 2023 Eric Bette
+        
+        Permission is hereby granted, free of charge, to any person obtaining a copy
+        of this software and associated documentation files (the "Software"), to deal
+        in the Software without restriction, including without limitation the rights
+        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+        copies of the Software, and to permit persons to whom the Software is
+        furnished to do so, subject to the following conditions:
+        
+        The above copyright notice and this permission notice shall be included in all
+        copies or substantial portions of the Software.
+        
+        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+        SOFTWARE.
+Project-URL: homepage, https://github.com/eebette/bank_scrapers/tree/master
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: beautifulsoup4>=4.12.2
+Requires-Dist: pandas>=2.0.2
+Requires-Dist: requests>=2.31.0
+Requires-Dist: undetected-chromedriver>=3.5.0
+Requires-Dist: lxml>=4.9.2
+Requires-Dist: setuptools>=69.5.1
+Requires-Dist: lxml>=5.2.2
+Requires-Dist: bank_scrapers==1.0.4
+
 # Table of Contents
 <!-- START doctoc generated TOC please keep comment here to allow auto update -->
 <!-- DON'T EDIT THIS SECTION, INSTEAD RE-RUN doctoc TO UPDATE -->
 
 - [Introduction](#introduction)
 - [Getting Started](#getting-started)
   - [Installation](#installation)
@@ -683,8 +722,8 @@
 production use, nefarious or otherwise.
 
 Usage of this code is potentially against your bank's terms of service and could result in you or your IP getting
 flagged, listed, or blocked as bad actors. I don't take any responsibility for any effects this code may have on your
 bank accounts or your relationships with your banking institutions.
 
 Please don't try to learn anything about me or my life based on the banks that I've arbitrarily decided to write
-drivers for. 
+drivers for.
```

### Comparing `bank_scrapers-1.0.4/bank_scrapers/api_wrappers/kraken/driver.py` & `bank_scrapers-1.0.5/bank_scrapers/api_wrappers/kraken/driver.py`

 * *Files identical despite different names*

### Comparing `bank_scrapers-1.0.4/bank_scrapers/cli/cli.py` & `bank_scrapers-1.0.5/bank_scrapers/cli/cli.py`

 * *Files identical despite different names*

### Comparing `bank_scrapers-1.0.4/bank_scrapers/scrapers/becu/driver.py` & `bank_scrapers-1.0.5/bank_scrapers/scrapers/smbc_prestia/driver.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,80 +1,54 @@
 """
-This file provides the get_accounts_info() function for BECU (https://onlinebanking.becu.org)
+This file provides the get_accounts_info() function for SMBC Prestia (https://login.smbctb.co.jp)
 
 Example Usage:
 ```
 tables = get_accounts_info(username="{username}", password="{password}")
 for t in tables:
     print(t.to_string())
 ```
 """
+
+# Standard Library Imports
+
 # Non-Standard Imports
 import pandas as pd
-from selenium.webdriver import Chrome
 from selenium.webdriver.common.by import By
 
 # Local Imports
 from bank_scrapers.scrapers.common.functions import *
 
 # Logon page
-HOMEPAGE: str = "https://onlinebanking.becu.org/BECUBankingWeb/Login.aspx"
+HOMEPAGE: str = "https://login.smbctb.co.jp/ib/portal/POSNIN1prestiatop.prst?LOCALE=en_JP"
 
 # Timeout
-TIMEOUT: int = 10
+TIMEOUT: int = 15
 
 # Chrome config
-USER_AGENT: str = "Mozilla/5.0 (X11; Linux x86_64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/60.0.3112.50 Safari/537.36"
 CHROME_OPTIONS: List[str] = [
-    f"user-agent={USER_AGENT}",
     "--no-sandbox",
     "--window-size=1920,1080",
     "--headless",
     "--disable-gpu",
     "--allow-running-insecure-content",
 ]
 
 
-def get_chrome_options(arguments: List[str]) -> Options:
+def get_chrome_options(arguments: List[str]) -> ChromeOptions:
     """
     Returns Options object for a list of chrome options arguments
     :param arguments: A list of string-ified chrome arguments
     :return: Options object with chrome options set
     """
-    chrome_options: Options = Options()
+    chrome_options: ChromeOptions = ChromeOptions()
     for arg in arguments:
         chrome_options.add_argument(arg)
-    return chrome_options
-
-
-def process_table(table: WebElement) -> pd.DataFrame:
-    """
-    Processes selenium table object into a pandas dataframe
-    :param table: The selenium table object to be processed
-    :return: A post-processed pandas dataframe of the original table object
-    """
-    # Get the htmnl
-    html: str = table.get_attribute("outerHTML")
-
-    # Load into pandas
-    table: pd.DataFrame = pd.read_html(html)[0]
-
-    # Strip non-digit/decimal
-    table: pd.DataFrame = table.replace(to_replace=r"[^0-9\.]+", value="", regex=True)
 
-    # Drop the last row (totals) from the table
-    table: pd.DataFrame = table.drop(table.tail(1).index)
-
-    # Convert each column to numeric and nullify any non-cohesive data
-    table: pd.DataFrame = table.apply(pd.to_numeric, errors="coerce")
-
-    # Drop any columns where all values are null
-    table: pd.DataFrame = table.dropna(axis=1, how="all")
-
-    return table
+    return chrome_options
 
 
 def logon(
     driver: Chrome, wait: WebDriverWait, homepage: str, username: str, password: str
 ) -> None:
     """
     Opens and signs on to an account
@@ -84,61 +58,96 @@
     :param username: Your username for logging in
     :param password: Your password for logging in
     """
     # Logon Page
     driver.get(homepage)
 
     # Enter User
-    user: WebElement = wait_and_find_element(
-        driver, wait, (By.ID, "ctlSignon_txtUserID")
-    )
+    user: WebElement = wait_and_find_click_element(driver, wait, (By.ID, "dispuserId"))
     user.send_keys(username)
 
     # Enter Password
-    passwd: WebElement = wait_and_find_element(
-        driver, wait, (By.ID, "ctlSignon_txtPassword")
-    )
+    passwd: WebElement = wait_and_find_element(driver, wait, (By.ID, "disppassword"))
     passwd.send_keys(password)
 
-    # Submit
-    submit: WebElement = wait_and_find_element(
-        driver, wait, (By.ID, "ctlSignon_btnLogin")
-    )
+    # Submit credentials
+    submit: WebElement = wait_and_find_element(driver, wait, (By.LINK_TEXT, "Sign On"))
     submit.click()
 
-    # Wait for redirect to landing page
-    wait.until(
-        lambda driver: "https://onlinebanking.becu.org/BECUBankingWeb/Accounts/Summary.aspx"
-        in driver.current_url
+
+def seek_accounts_data(driver: Chrome, wait: WebDriverWait) -> WebElement:
+    """
+    Navigate the website and find the accounts data for the user
+    :param driver: The Chrome browser application
+    :param wait: WebDriverWait object for the driver
+    :return: The web element of the accounts data
+    """
+    accounts_btn: WebElement = wait_and_find_click_element(
+        driver, wait, (By.LINK_TEXT, "Accounts")
+    )
+    accounts_btn.click()
+
+    balance_btn: WebElement = wait_and_find_click_element(
+        driver, wait, (By.LINK_TEXT, "Balance Summary")
+    )
+    balance_btn.click()
+
+    table: WebElement = driver.find_element(
+        By.CSS_SELECTOR,
+        "body > form:nth-child(2) > main > div > section > div.inner > table.table.table-normal",
     )
 
+    return table
+
+
+def parse_accounts_summary(table: WebElement) -> pd.DataFrame:
+    """
+    Post-processing of the table html
+    :param table: The html input of the accounts data from the site
+    :return: A pandas dataframe of the downloaded data
+    """
+    # Create a simple dataframe from the input amount
+    html: str = table.get_attribute("outerHTML")
+    df: pd.DataFrame = pd.read_html(html)[0]
+
+    # Remove non-numeric, non-decimal characters
+    df: pd.DataFrame = df.replace(to_replace=r"[^0-9\.]+", value="", regex=True)
+
+    # Int-ify the monthly payment amount column
+    df: pd.DataFrame = df.apply(pd.to_numeric, errors="coerce")
+
+    # Drop columns where all values are null
+    df.dropna(axis=1, how="all", inplace=True)
+
+    # Return the dataframe
+    return df
+
 
 def get_accounts_info(username: str, password: str) -> List[pd.DataFrame]:
     """
     Gets the accounts info for a given user/pass as a list of pandas dataframes
     :param username: Your username for logging in
     :param password: Your password for logging in
     :return: A list of pandas dataframes of accounts info tables
     """
     # Get Driver config
-    chrome_options: Options = get_chrome_options(CHROME_OPTIONS)
+    chrome_options: ChromeOptions = get_chrome_options(CHROME_OPTIONS)
+
+    # Instantiating the Driver
     driver: Chrome = start_chromedriver(chrome_options)
     wait: WebDriverWait = WebDriverWait(driver, TIMEOUT)
 
+    # Navigate to the logon page and submit credentials
     logon(driver, wait, HOMEPAGE, username, password)
 
-    # Get data for account and credit cards
-    tables: List[WebElement] = wait_and_find_elements(
-        driver, wait, (By.CLASS_NAME, "tablesaw-stack")
-    )
+    # Navigate the site and download the accounts data
+    accounts_data: WebElement = seek_accounts_data(driver, wait)
+    accounts_data_df: pd.DataFrame = parse_accounts_summary(accounts_data)
 
     # Process tables
-    return_tables: List = list()
-    for t in tables:
-        table: pd.DataFrame = process_table(t)
-        return_tables.append(table)
+    return_tables: List[pd.DataFrame] = [accounts_data_df]
 
     # Clean up
     driver.quit()
 
     # Return list of pandas df
     return return_tables
```

### Comparing `bank_scrapers-1.0.4/bank_scrapers/scrapers/chase/driver.py` & `bank_scrapers-1.0.5/bank_scrapers/scrapers/chase/driver.py`

 * *Files identical despite different names*

### Comparing `bank_scrapers-1.0.4/bank_scrapers/scrapers/common/functions.py` & `bank_scrapers-1.0.5/bank_scrapers/scrapers/common/functions.py`

 * *Files identical despite different names*

### Comparing `bank_scrapers-1.0.4/bank_scrapers/scrapers/fidelity_netbenefits/driver.py` & `bank_scrapers-1.0.5/bank_scrapers/scrapers/fidelity_netbenefits/driver.py`

 * *Files identical despite different names*

### Comparing `bank_scrapers-1.0.4/bank_scrapers/scrapers/roundpoint/driver.py` & `bank_scrapers-1.0.5/bank_scrapers/scrapers/roundpoint/driver.py`

 * *Files identical despite different names*

### Comparing `bank_scrapers-1.0.4/bank_scrapers/scrapers/uhfcu/driver.py` & `bank_scrapers-1.0.5/bank_scrapers/scrapers/uhfcu/driver.py`

 * *Files identical despite different names*

### Comparing `bank_scrapers-1.0.4/bank_scrapers/scrapers/vanguard/driver.py` & `bank_scrapers-1.0.5/bank_scrapers/scrapers/vanguard/driver.py`

 * *Files identical despite different names*

### Comparing `bank_scrapers-1.0.4/bank_scrapers/scrapers/zillow/driver.py` & `bank_scrapers-1.0.5/bank_scrapers/scrapers/zillow/driver.py`

 * *Files identical despite different names*

### Comparing `bank_scrapers-1.0.4/bank_scrapers.egg-info/PKG-INFO` & `bank_scrapers-1.0.5/bank_scrapers.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: bank-scrapers
-Version: 1.0.4
+Name: bank_scrapers
+Version: 1.0.5
 Summary: Library for working with bank_scrapers drivers.
 Author: Eric Bette
 License: MIT License
         
         Copyright (c) 2023 Eric Bette
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -24,14 +24,22 @@
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
 Project-URL: homepage, https://github.com/eebette/bank_scrapers/tree/master
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: beautifulsoup4>=4.12.2
+Requires-Dist: pandas>=2.0.2
+Requires-Dist: requests>=2.31.0
+Requires-Dist: undetected-chromedriver>=3.5.0
+Requires-Dist: lxml>=4.9.2
+Requires-Dist: setuptools>=69.5.1
+Requires-Dist: lxml>=5.2.2
+Requires-Dist: bank_scrapers==1.0.4
 
 # Table of Contents
 <!-- START doctoc generated TOC please keep comment here to allow auto update -->
 <!-- DON'T EDIT THIS SECTION, INSTEAD RE-RUN doctoc TO UPDATE -->
 
 - [Introduction](#introduction)
 - [Getting Started](#getting-started)
```

### Comparing `bank_scrapers-1.0.4/bank_scrapers.egg-info/SOURCES.txt` & `bank_scrapers-1.0.5/bank_scrapers.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bank_scrapers-1.0.4/pyproject.toml` & `bank_scrapers-1.0.5/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -15,15 +15,18 @@
 
 dependencies = [
     "beautifulsoup4>=4.12.2",
     "pandas>=2.0.2",
     "requests>=2.31.0",
     "undetected-chromedriver>=3.5.0",
     "lxml>=4.9.2",
-    "bank_scrapers==1.0.4",
+    "setuptools>=69.5.1",
+    "lxml>=5.2.2",
+    "bank_scrapers==1.0.4"
+
 ]
 
 [project.urls]
 homepage = "https://github.com/eebette/bank_scrapers/tree/master"
 
 [project.scripts]
 bank-scrape = "bank_scrapers.cli.cli:main"
```

