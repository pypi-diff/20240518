# Comparing `tmp/bank_scrapers-1.0.7.tar.gz` & `tmp/bank_scrapers-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bank_scrapers-1.0.7.tar", last modified: Sat May 18 05:09:35 2024, max compression
+gzip compressed data, was "bank_scrapers-1.0.8.tar", last modified: Sat May 18 06:14:34 2024, max compression
```

## Comparing `bank_scrapers-1.0.7.tar` & `bank_scrapers-1.0.8.tar`

### file list

```diff
@@ -1,55 +1,57 @@
-drwxrwxr-x   0 eric      (1000) eric      (1000)        0 2024-05-18 05:09:35.372169 bank_scrapers-1.0.7/
--rw-rw-r--   0 eric      (1000) eric      (1000)     1066 2024-05-16 09:36:03.000000 bank_scrapers-1.0.7/LICENSE
--rw-r--r--   0 eric      (1000) eric      (1000)    22430 2024-05-18 05:09:35.372169 bank_scrapers-1.0.7/PKG-INFO
--rw-rw-r--   0 eric      (1000) eric      (1000)    20665 2024-05-16 09:36:03.000000 bank_scrapers-1.0.7/README.md
-drwxrwxr-x   0 eric      (1000) eric      (1000)        0 2024-05-18 05:09:35.369169 bank_scrapers-1.0.7/bank_scrapers/
--rw-rw-r--   0 eric      (1000) eric      (1000)      307 2024-05-18 05:07:40.000000 bank_scrapers-1.0.7/bank_scrapers/__init__.py
-drwxrwxr-x   0 eric      (1000) eric      (1000)        0 2024-05-18 05:09:35.370169 bank_scrapers-1.0.7/bank_scrapers/api_wrappers/
--rw-rw-r--   0 eric      (1000) eric      (1000)        0 2024-05-16 09:36:03.000000 bank_scrapers-1.0.7/bank_scrapers/api_wrappers/__init__.py
-drwxrwxr-x   0 eric      (1000) eric      (1000)        0 2024-05-18 05:09:35.370169 bank_scrapers-1.0.7/bank_scrapers/api_wrappers/kraken/
--rw-rw-r--   0 eric      (1000) eric      (1000)        0 2024-05-16 09:36:03.000000 bank_scrapers-1.0.7/bank_scrapers/api_wrappers/kraken/__init__.py
--rw-rw-r--   0 eric      (1000) eric      (1000)     2863 2024-05-16 09:36:03.000000 bank_scrapers-1.0.7/bank_scrapers/api_wrappers/kraken/driver.py
-drwxrwxr-x   0 eric      (1000) eric      (1000)        0 2024-05-18 05:09:35.370169 bank_scrapers-1.0.7/bank_scrapers/cli/
--rw-rw-r--   0 eric      (1000) eric      (1000)        0 2024-05-16 09:36:03.000000 bank_scrapers-1.0.7/bank_scrapers/cli/__init__.py
--rw-rw-r--   0 eric      (1000) eric      (1000)     9027 2024-05-16 09:36:03.000000 bank_scrapers-1.0.7/bank_scrapers/cli/cli.py
-drwxrwxr-x   0 eric      (1000) eric      (1000)        0 2024-05-18 05:09:35.370169 bank_scrapers-1.0.7/bank_scrapers/common/
--rw-rw-r--   0 eric      (1000) eric      (1000)        0 2024-05-16 09:36:03.000000 bank_scrapers-1.0.7/bank_scrapers/common/__init__.py
--rw-rw-r--   0 eric      (1000) eric      (1000)      272 2024-05-16 09:36:03.000000 bank_scrapers-1.0.7/bank_scrapers/common/log.py
-drwxrwxr-x   0 eric      (1000) eric      (1000)        0 2024-05-18 05:09:35.370169 bank_scrapers-1.0.7/bank_scrapers/scrapers/
--rw-rw-r--   0 eric      (1000) eric      (1000)        0 2024-05-16 09:36:03.000000 bank_scrapers-1.0.7/bank_scrapers/scrapers/__init__.py
-drwxrwxr-x   0 eric      (1000) eric      (1000)        0 2024-05-18 05:09:35.370169 bank_scrapers-1.0.7/bank_scrapers/scrapers/becu/
--rw-rw-r--   0 eric      (1000) eric      (1000)        0 2024-05-16 09:36:03.000000 bank_scrapers-1.0.7/bank_scrapers/scrapers/becu/__init__.py
--rw-rw-r--   0 eric      (1000) eric      (1000)     6910 2024-05-18 04:44:12.000000 bank_scrapers-1.0.7/bank_scrapers/scrapers/becu/driver.py
-drwxrwxr-x   0 eric      (1000) eric      (1000)        0 2024-05-18 05:09:35.370169 bank_scrapers-1.0.7/bank_scrapers/scrapers/chase/
--rw-rw-r--   0 eric      (1000) eric      (1000)        0 2024-05-16 09:36:03.000000 bank_scrapers-1.0.7/bank_scrapers/scrapers/chase/__init__.py
--rw-rw-r--   0 eric      (1000) eric      (1000)     9191 2024-05-16 09:36:03.000000 bank_scrapers-1.0.7/bank_scrapers/scrapers/chase/driver.py
-drwxrwxr-x   0 eric      (1000) eric      (1000)        0 2024-05-18 05:09:35.371169 bank_scrapers-1.0.7/bank_scrapers/scrapers/common/
--rw-rw-r--   0 eric      (1000) eric      (1000)        0 2024-05-16 09:36:03.000000 bank_scrapers-1.0.7/bank_scrapers/scrapers/common/__init__.py
--rw-rw-r--   0 eric      (1000) eric      (1000)     4712 2024-05-16 09:36:03.000000 bank_scrapers-1.0.7/bank_scrapers/scrapers/common/functions.py
-drwxrwxr-x   0 eric      (1000) eric      (1000)        0 2024-05-18 05:09:35.371169 bank_scrapers-1.0.7/bank_scrapers/scrapers/fidelity_netbenefits/
--rw-rw-r--   0 eric      (1000) eric      (1000)        0 2024-05-16 09:36:03.000000 bank_scrapers-1.0.7/bank_scrapers/scrapers/fidelity_netbenefits/__init__.py
--rw-rw-r--   0 eric      (1000) eric      (1000)     8335 2024-05-16 09:36:03.000000 bank_scrapers-1.0.7/bank_scrapers/scrapers/fidelity_netbenefits/driver.py
-drwxrwxr-x   0 eric      (1000) eric      (1000)        0 2024-05-18 05:09:35.371169 bank_scrapers-1.0.7/bank_scrapers/scrapers/roundpoint/
--rw-rw-r--   0 eric      (1000) eric      (1000)        0 2024-05-16 09:36:03.000000 bank_scrapers-1.0.7/bank_scrapers/scrapers/roundpoint/__init__.py
--rw-rw-r--   0 eric      (1000) eric      (1000)     8626 2024-05-16 09:36:03.000000 bank_scrapers-1.0.7/bank_scrapers/scrapers/roundpoint/driver.py
-drwxrwxr-x   0 eric      (1000) eric      (1000)        0 2024-05-18 05:09:35.371169 bank_scrapers-1.0.7/bank_scrapers/scrapers/smbc_prestia/
--rw-rw-r--   0 eric      (1000) eric      (1000)        0 2024-05-16 09:36:03.000000 bank_scrapers-1.0.7/bank_scrapers/scrapers/smbc_prestia/__init__.py
--rw-rw-r--   0 eric      (1000) eric      (1000)     4632 2024-05-16 09:36:03.000000 bank_scrapers-1.0.7/bank_scrapers/scrapers/smbc_prestia/driver.py
-drwxrwxr-x   0 eric      (1000) eric      (1000)        0 2024-05-18 05:09:35.371169 bank_scrapers-1.0.7/bank_scrapers/scrapers/uhfcu/
--rw-rw-r--   0 eric      (1000) eric      (1000)        0 2024-05-16 09:36:03.000000 bank_scrapers-1.0.7/bank_scrapers/scrapers/uhfcu/__init__.py
--rw-rw-r--   0 eric      (1000) eric      (1000)     8655 2024-05-16 09:36:03.000000 bank_scrapers-1.0.7/bank_scrapers/scrapers/uhfcu/driver.py
-drwxrwxr-x   0 eric      (1000) eric      (1000)        0 2024-05-18 05:09:35.371169 bank_scrapers-1.0.7/bank_scrapers/scrapers/vanguard/
--rw-rw-r--   0 eric      (1000) eric      (1000)        0 2024-05-16 09:36:03.000000 bank_scrapers-1.0.7/bank_scrapers/scrapers/vanguard/__init__.py
--rw-rw-r--   0 eric      (1000) eric      (1000)     7740 2024-05-16 09:36:03.000000 bank_scrapers-1.0.7/bank_scrapers/scrapers/vanguard/driver.py
-drwxrwxr-x   0 eric      (1000) eric      (1000)        0 2024-05-18 05:09:35.372169 bank_scrapers-1.0.7/bank_scrapers/scrapers/zillow/
--rw-rw-r--   0 eric      (1000) eric      (1000)        0 2024-05-16 09:36:03.000000 bank_scrapers-1.0.7/bank_scrapers/scrapers/zillow/__init__.py
--rw-rw-r--   0 eric      (1000) eric      (1000)     3457 2024-05-16 09:36:03.000000 bank_scrapers-1.0.7/bank_scrapers/scrapers/zillow/driver.py
-drwxrwxr-x   0 eric      (1000) eric      (1000)        0 2024-05-18 05:09:35.372169 bank_scrapers-1.0.7/bank_scrapers.egg-info/
--rw-r--r--   0 eric      (1000) eric      (1000)    22430 2024-05-18 05:09:35.000000 bank_scrapers-1.0.7/bank_scrapers.egg-info/PKG-INFO
--rw-rw-r--   0 eric      (1000) eric      (1000)     1347 2024-05-18 05:09:35.000000 bank_scrapers-1.0.7/bank_scrapers.egg-info/SOURCES.txt
--rw-rw-r--   0 eric      (1000) eric      (1000)        1 2024-05-18 05:09:35.000000 bank_scrapers-1.0.7/bank_scrapers.egg-info/dependency_links.txt
--rw-rw-r--   0 eric      (1000) eric      (1000)       59 2024-05-18 05:09:35.000000 bank_scrapers-1.0.7/bank_scrapers.egg-info/entry_points.txt
--rw-rw-r--   0 eric      (1000) eric      (1000)      128 2024-05-18 05:09:35.000000 bank_scrapers-1.0.7/bank_scrapers.egg-info/requires.txt
--rw-rw-r--   0 eric      (1000) eric      (1000)       14 2024-05-18 05:09:35.000000 bank_scrapers-1.0.7/bank_scrapers.egg-info/top_level.txt
--rw-rw-r--   0 eric      (1000) eric      (1000)      962 2024-05-18 05:07:40.000000 bank_scrapers-1.0.7/pyproject.toml
--rw-rw-r--   0 eric      (1000) eric      (1000)       38 2024-05-18 05:09:35.372169 bank_scrapers-1.0.7/setup.cfg
+drwxrwxr-x   0 eric      (1000) eric      (1000)        0 2024-05-18 06:14:34.342314 bank_scrapers-1.0.8/
+-rw-rw-r--   0 eric      (1000) eric      (1000)     1066 2024-05-16 09:36:03.000000 bank_scrapers-1.0.8/LICENSE
+-rw-r--r--   0 eric      (1000) eric      (1000)    22430 2024-05-18 06:14:34.342314 bank_scrapers-1.0.8/PKG-INFO
+-rw-rw-r--   0 eric      (1000) eric      (1000)    20665 2024-05-16 09:36:03.000000 bank_scrapers-1.0.8/README.md
+drwxrwxr-x   0 eric      (1000) eric      (1000)        0 2024-05-18 06:14:34.339314 bank_scrapers-1.0.8/bank_scrapers/
+-rw-rw-r--   0 eric      (1000) eric      (1000)      308 2024-05-18 06:14:30.000000 bank_scrapers-1.0.8/bank_scrapers/__init__.py
+drwxrwxr-x   0 eric      (1000) eric      (1000)        0 2024-05-18 06:14:34.340314 bank_scrapers-1.0.8/bank_scrapers/api_wrappers/
+-rw-rw-r--   0 eric      (1000) eric      (1000)        0 2024-05-16 09:36:03.000000 bank_scrapers-1.0.8/bank_scrapers/api_wrappers/__init__.py
+drwxrwxr-x   0 eric      (1000) eric      (1000)        0 2024-05-18 06:14:34.340314 bank_scrapers-1.0.8/bank_scrapers/api_wrappers/kraken/
+-rw-rw-r--   0 eric      (1000) eric      (1000)        0 2024-05-16 09:36:03.000000 bank_scrapers-1.0.8/bank_scrapers/api_wrappers/kraken/__init__.py
+-rw-rw-r--   0 eric      (1000) eric      (1000)     2863 2024-05-16 09:36:03.000000 bank_scrapers-1.0.8/bank_scrapers/api_wrappers/kraken/driver.py
+drwxrwxr-x   0 eric      (1000) eric      (1000)        0 2024-05-18 06:14:34.340314 bank_scrapers-1.0.8/bank_scrapers/cli/
+-rw-rw-r--   0 eric      (1000) eric      (1000)        0 2024-05-16 09:36:03.000000 bank_scrapers-1.0.8/bank_scrapers/cli/__init__.py
+-rw-rw-r--   0 eric      (1000) eric      (1000)     9027 2024-05-16 09:36:03.000000 bank_scrapers-1.0.8/bank_scrapers/cli/cli.py
+drwxrwxr-x   0 eric      (1000) eric      (1000)        0 2024-05-18 06:14:34.340314 bank_scrapers-1.0.8/bank_scrapers/common/
+-rw-rw-r--   0 eric      (1000) eric      (1000)        0 2024-05-16 09:36:03.000000 bank_scrapers-1.0.8/bank_scrapers/common/__init__.py
+-rw-rw-r--   0 eric      (1000) eric      (1000)     1394 2024-05-18 06:14:01.000000 bank_scrapers-1.0.8/bank_scrapers/common/functions.py
+-rw-rw-r--   0 eric      (1000) eric      (1000)      271 2024-05-18 06:09:50.000000 bank_scrapers-1.0.8/bank_scrapers/common/log.py
+-rw-rw-r--   0 eric      (1000) eric      (1000)      169 2024-05-18 06:02:00.000000 bank_scrapers-1.0.8/bank_scrapers/common/values.py
+drwxrwxr-x   0 eric      (1000) eric      (1000)        0 2024-05-18 06:14:34.340314 bank_scrapers-1.0.8/bank_scrapers/scrapers/
+-rw-rw-r--   0 eric      (1000) eric      (1000)        0 2024-05-16 09:36:03.000000 bank_scrapers-1.0.8/bank_scrapers/scrapers/__init__.py
+drwxrwxr-x   0 eric      (1000) eric      (1000)        0 2024-05-18 06:14:34.340314 bank_scrapers-1.0.8/bank_scrapers/scrapers/becu/
+-rw-rw-r--   0 eric      (1000) eric      (1000)        0 2024-05-16 09:36:03.000000 bank_scrapers-1.0.8/bank_scrapers/scrapers/becu/__init__.py
+-rw-rw-r--   0 eric      (1000) eric      (1000)     7589 2024-05-18 06:13:34.000000 bank_scrapers-1.0.8/bank_scrapers/scrapers/becu/driver.py
+drwxrwxr-x   0 eric      (1000) eric      (1000)        0 2024-05-18 06:14:34.341313 bank_scrapers-1.0.8/bank_scrapers/scrapers/chase/
+-rw-rw-r--   0 eric      (1000) eric      (1000)        0 2024-05-16 09:36:03.000000 bank_scrapers-1.0.8/bank_scrapers/scrapers/chase/__init__.py
+-rw-rw-r--   0 eric      (1000) eric      (1000)     9191 2024-05-16 09:36:03.000000 bank_scrapers-1.0.8/bank_scrapers/scrapers/chase/driver.py
+drwxrwxr-x   0 eric      (1000) eric      (1000)        0 2024-05-18 06:14:34.341313 bank_scrapers-1.0.8/bank_scrapers/scrapers/common/
+-rw-rw-r--   0 eric      (1000) eric      (1000)        0 2024-05-16 09:36:03.000000 bank_scrapers-1.0.8/bank_scrapers/scrapers/common/__init__.py
+-rw-rw-r--   0 eric      (1000) eric      (1000)     4712 2024-05-16 09:36:03.000000 bank_scrapers-1.0.8/bank_scrapers/scrapers/common/functions.py
+drwxrwxr-x   0 eric      (1000) eric      (1000)        0 2024-05-18 06:14:34.341313 bank_scrapers-1.0.8/bank_scrapers/scrapers/fidelity_netbenefits/
+-rw-rw-r--   0 eric      (1000) eric      (1000)        0 2024-05-16 09:36:03.000000 bank_scrapers-1.0.8/bank_scrapers/scrapers/fidelity_netbenefits/__init__.py
+-rw-rw-r--   0 eric      (1000) eric      (1000)     8335 2024-05-16 09:36:03.000000 bank_scrapers-1.0.8/bank_scrapers/scrapers/fidelity_netbenefits/driver.py
+drwxrwxr-x   0 eric      (1000) eric      (1000)        0 2024-05-18 06:14:34.341313 bank_scrapers-1.0.8/bank_scrapers/scrapers/roundpoint/
+-rw-rw-r--   0 eric      (1000) eric      (1000)        0 2024-05-16 09:36:03.000000 bank_scrapers-1.0.8/bank_scrapers/scrapers/roundpoint/__init__.py
+-rw-rw-r--   0 eric      (1000) eric      (1000)     8626 2024-05-16 09:36:03.000000 bank_scrapers-1.0.8/bank_scrapers/scrapers/roundpoint/driver.py
+drwxrwxr-x   0 eric      (1000) eric      (1000)        0 2024-05-18 06:14:34.341313 bank_scrapers-1.0.8/bank_scrapers/scrapers/smbc_prestia/
+-rw-rw-r--   0 eric      (1000) eric      (1000)        0 2024-05-16 09:36:03.000000 bank_scrapers-1.0.8/bank_scrapers/scrapers/smbc_prestia/__init__.py
+-rw-rw-r--   0 eric      (1000) eric      (1000)     4632 2024-05-16 09:36:03.000000 bank_scrapers-1.0.8/bank_scrapers/scrapers/smbc_prestia/driver.py
+drwxrwxr-x   0 eric      (1000) eric      (1000)        0 2024-05-18 06:14:34.341313 bank_scrapers-1.0.8/bank_scrapers/scrapers/uhfcu/
+-rw-rw-r--   0 eric      (1000) eric      (1000)        0 2024-05-16 09:36:03.000000 bank_scrapers-1.0.8/bank_scrapers/scrapers/uhfcu/__init__.py
+-rw-rw-r--   0 eric      (1000) eric      (1000)     8655 2024-05-16 09:36:03.000000 bank_scrapers-1.0.8/bank_scrapers/scrapers/uhfcu/driver.py
+drwxrwxr-x   0 eric      (1000) eric      (1000)        0 2024-05-18 06:14:34.342314 bank_scrapers-1.0.8/bank_scrapers/scrapers/vanguard/
+-rw-rw-r--   0 eric      (1000) eric      (1000)        0 2024-05-16 09:36:03.000000 bank_scrapers-1.0.8/bank_scrapers/scrapers/vanguard/__init__.py
+-rw-rw-r--   0 eric      (1000) eric      (1000)     7740 2024-05-16 09:36:03.000000 bank_scrapers-1.0.8/bank_scrapers/scrapers/vanguard/driver.py
+drwxrwxr-x   0 eric      (1000) eric      (1000)        0 2024-05-18 06:14:34.342314 bank_scrapers-1.0.8/bank_scrapers/scrapers/zillow/
+-rw-rw-r--   0 eric      (1000) eric      (1000)        0 2024-05-16 09:36:03.000000 bank_scrapers-1.0.8/bank_scrapers/scrapers/zillow/__init__.py
+-rw-rw-r--   0 eric      (1000) eric      (1000)     3457 2024-05-16 09:36:03.000000 bank_scrapers-1.0.8/bank_scrapers/scrapers/zillow/driver.py
+drwxrwxr-x   0 eric      (1000) eric      (1000)        0 2024-05-18 06:14:34.342314 bank_scrapers-1.0.8/bank_scrapers.egg-info/
+-rw-r--r--   0 eric      (1000) eric      (1000)    22430 2024-05-18 06:14:34.000000 bank_scrapers-1.0.8/bank_scrapers.egg-info/PKG-INFO
+-rw-rw-r--   0 eric      (1000) eric      (1000)     1412 2024-05-18 06:14:34.000000 bank_scrapers-1.0.8/bank_scrapers.egg-info/SOURCES.txt
+-rw-rw-r--   0 eric      (1000) eric      (1000)        1 2024-05-18 06:14:34.000000 bank_scrapers-1.0.8/bank_scrapers.egg-info/dependency_links.txt
+-rw-rw-r--   0 eric      (1000) eric      (1000)       59 2024-05-18 06:14:34.000000 bank_scrapers-1.0.8/bank_scrapers.egg-info/entry_points.txt
+-rw-rw-r--   0 eric      (1000) eric      (1000)      128 2024-05-18 06:14:34.000000 bank_scrapers-1.0.8/bank_scrapers.egg-info/requires.txt
+-rw-rw-r--   0 eric      (1000) eric      (1000)       14 2024-05-18 06:14:34.000000 bank_scrapers-1.0.8/bank_scrapers.egg-info/top_level.txt
+-rw-rw-r--   0 eric      (1000) eric      (1000)      962 2024-05-18 05:07:40.000000 bank_scrapers-1.0.8/pyproject.toml
+-rw-rw-r--   0 eric      (1000) eric      (1000)       38 2024-05-18 06:14:34.342314 bank_scrapers-1.0.8/setup.cfg
```

### Comparing `bank_scrapers-1.0.7/LICENSE` & `bank_scrapers-1.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `bank_scrapers-1.0.7/PKG-INFO` & `bank_scrapers-1.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bank_scrapers
-Version: 1.0.7
+Version: 1.0.8
 Summary: Library for working with bank_scrapers drivers.
 Author: Eric Bette
 License: MIT License
         
         Copyright (c) 2023 Eric Bette
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `bank_scrapers-1.0.7/README.md` & `bank_scrapers-1.0.8/README.md`

 * *Files identical despite different names*

### Comparing `bank_scrapers-1.0.7/bank_scrapers/api_wrappers/kraken/driver.py` & `bank_scrapers-1.0.8/bank_scrapers/api_wrappers/kraken/driver.py`

 * *Files identical despite different names*

### Comparing `bank_scrapers-1.0.7/bank_scrapers/cli/cli.py` & `bank_scrapers-1.0.8/bank_scrapers/cli/cli.py`

 * *Files identical despite different names*

### Comparing `bank_scrapers-1.0.7/bank_scrapers/scrapers/becu/driver.py` & `bank_scrapers-1.0.8/bank_scrapers/scrapers/becu/driver.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,24 +4,30 @@
 Example Usage:
 ```
 tables = get_accounts_info(username="{username}", password="{password}")
 for t in tables:
     print(t.to_string())
 ```
 """
+
 # Standard library imports
 from typing import Dict
 
 # Non-Standard Imports
 import pandas as pd
 from selenium.webdriver import Chrome
 from selenium.webdriver.common.by import By
 
 # Local Imports
 from bank_scrapers.scrapers.common.functions import *
+from bank_scrapers.common.functions import convert_to_prometheus
+
+# Institution info
+INSTITUTION: str = "BECU"
+SYMBOL: str = "USD"
 
 # Logon page
 HOMEPAGE: str = "https://onlinebanking.becu.org/BECUBankingWeb/Login.aspx"
 
 # Timeout
 TIMEOUT: int = 10
 
@@ -74,15 +80,17 @@
 
     # Drop any columns where all values are null
     table: pd.DataFrame = table.dropna(axis=1, how="all")
 
     return table
 
 
-def get_mfa_answer(driver: Chrome, wait: WebDriverWait, mfa_answers: Dict[str, str] | None = None) -> str:
+def get_mfa_answer(
+    driver: Chrome, wait: WebDriverWait, mfa_answers: Dict[str, str] | None = None
+) -> str:
     """
     Returns the answer for the MFA question or prompts the user for the answer if not provided
     :param driver: The browser application
     :param wait: WebDriverWait object for the driver
     :param mfa_answers: A dict of the MFA answers where the keys are the questions and the values are the answers
     :return: The MFA answer to input
     """
@@ -114,16 +122,20 @@
                 "https://onlinebanking.becu.org/BECUBankingWeb/Security/Challenge",
             ]
         )
     )
 
 
 def logon(
-        driver: Chrome, wait: WebDriverWait, homepage: str, username: str, password: str,
-        mfa_answers: Dict[str, str] | None = None
+    driver: Chrome,
+    wait: WebDriverWait,
+    homepage: str,
+    username: str,
+    password: str,
+    mfa_answers: Dict[str, str] | None = None,
 ) -> None:
     """
     Opens and signs on to an account
     :param driver: The browser application
     :param wait: WebDriverWait object for the driver
     :param homepage: The logon url to initially navigate
     :param username: Your username for logging in
@@ -147,31 +159,34 @@
 
     # Submit
     submit: WebElement = wait_and_find_element(
         driver, wait, (By.ID, "ctlSignon_btnLogin")
     )
     submit.click()
 
-    while driver.current_url != "https://onlinebanking.becu.org/BECUBankingWeb/Accounts/Summary.aspx":
+    while (
+        driver.current_url
+        != "https://onlinebanking.becu.org/BECUBankingWeb/Accounts/Summary.aspx"
+    ):
         # Wait for redirect to landing page
         handle_redirect(wait)
 
         if (
-                driver.current_url
-                == "https://onlinebanking.becu.org/BECUBankingWeb/Invitation/Default.aspx"
+            driver.current_url
+            == "https://onlinebanking.becu.org/BECUBankingWeb/Invitation/Default.aspx"
         ):
             # Decline offer
             decline_btn: WebElement = wait_and_find_element(
                 driver, wait, (By.NAME, "ctlWorkflow$decline")
             )
             decline_btn.click()
 
         elif (
-                driver.current_url
-                == "https://onlinebanking.becu.org/BECUBankingWeb/Security/Challenge"
+            driver.current_url
+            == "https://onlinebanking.becu.org/BECUBankingWeb/Security/Challenge"
         ):
             # Get MFA answer
             mfa_answer: str = get_mfa_answer(driver, wait, mfa_answers)
 
             # Find input box and input MFA answer
             answer_input: WebElement = wait_and_find_element(
                 driver, wait, (By.ID, "challengeAnswer")
@@ -181,19 +196,22 @@
             # Find agree/submit button and click
             agree_input: WebElement = wait_and_find_element(
                 driver, wait, (By.ID, "agree-and-continue-button")
             )
             agree_input.click()
 
 
-def get_accounts_info(username: str, password: str) -> List[pd.DataFrame]:
+def get_accounts_info(
+    username: str, password: str, prometheus: bool = False
+) -> List[pd.DataFrame] | str:
     """
     Gets the accounts info for a given user/pass as a list of pandas dataframes
     :param username: Your username for logging in
     :param password: Your password for logging in
+    :param prometheus: True/False value to exporting as Prometheus-friendly exposition
     :return: A list of pandas dataframes of accounts info tables
     """
     # Get Driver config
     chrome_options: Options = get_chrome_options(CHROME_OPTIONS)
     driver: Chrome = start_chromedriver(chrome_options)
     wait: WebDriverWait = WebDriverWait(driver, TIMEOUT)
 
@@ -203,15 +221,25 @@
     tables: List[WebElement] = wait_and_find_elements(
         driver, wait, (By.CLASS_NAME, "tablesaw-stack")
     )
 
     # Process tables
     return_tables: List = list()
     for t in tables:
+        is_credit_account = any(
+            list(True for header in t.columns if "credit" in header.lower())
+        )
         table: pd.DataFrame = process_table(t)
+        table.name = "credit" if is_credit_account else "deposit"
         return_tables.append(table)
 
     # Clean up
     driver.quit()
 
+    # Convert to Prometheus exposition if flag is set
+    if prometheus:
+        return_tables: str = convert_to_prometheus(
+            return_tables, INSTITUTION, "Account", SYMBOL, "Current Balance"
+        )
+
     # Return list of pandas df
     return return_tables
```

### Comparing `bank_scrapers-1.0.7/bank_scrapers/scrapers/chase/driver.py` & `bank_scrapers-1.0.8/bank_scrapers/scrapers/chase/driver.py`

 * *Files identical despite different names*

### Comparing `bank_scrapers-1.0.7/bank_scrapers/scrapers/common/functions.py` & `bank_scrapers-1.0.8/bank_scrapers/scrapers/common/functions.py`

 * *Files identical despite different names*

### Comparing `bank_scrapers-1.0.7/bank_scrapers/scrapers/fidelity_netbenefits/driver.py` & `bank_scrapers-1.0.8/bank_scrapers/scrapers/fidelity_netbenefits/driver.py`

 * *Files identical despite different names*

### Comparing `bank_scrapers-1.0.7/bank_scrapers/scrapers/roundpoint/driver.py` & `bank_scrapers-1.0.8/bank_scrapers/scrapers/roundpoint/driver.py`

 * *Files identical despite different names*

### Comparing `bank_scrapers-1.0.7/bank_scrapers/scrapers/smbc_prestia/driver.py` & `bank_scrapers-1.0.8/bank_scrapers/scrapers/smbc_prestia/driver.py`

 * *Files identical despite different names*

### Comparing `bank_scrapers-1.0.7/bank_scrapers/scrapers/uhfcu/driver.py` & `bank_scrapers-1.0.8/bank_scrapers/scrapers/uhfcu/driver.py`

 * *Files identical despite different names*

### Comparing `bank_scrapers-1.0.7/bank_scrapers/scrapers/vanguard/driver.py` & `bank_scrapers-1.0.8/bank_scrapers/scrapers/vanguard/driver.py`

 * *Files identical despite different names*

### Comparing `bank_scrapers-1.0.7/bank_scrapers/scrapers/zillow/driver.py` & `bank_scrapers-1.0.8/bank_scrapers/scrapers/zillow/driver.py`

 * *Files identical despite different names*

### Comparing `bank_scrapers-1.0.7/bank_scrapers.egg-info/PKG-INFO` & `bank_scrapers-1.0.8/bank_scrapers.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bank_scrapers
-Version: 1.0.7
+Version: 1.0.8
 Summary: Library for working with bank_scrapers drivers.
 Author: Eric Bette
 License: MIT License
         
         Copyright (c) 2023 Eric Bette
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `bank_scrapers-1.0.7/bank_scrapers.egg-info/SOURCES.txt` & `bank_scrapers-1.0.8/bank_scrapers.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -10,15 +10,17 @@
 bank_scrapers.egg-info/top_level.txt
 bank_scrapers/api_wrappers/__init__.py
 bank_scrapers/api_wrappers/kraken/__init__.py
 bank_scrapers/api_wrappers/kraken/driver.py
 bank_scrapers/cli/__init__.py
 bank_scrapers/cli/cli.py
 bank_scrapers/common/__init__.py
+bank_scrapers/common/functions.py
 bank_scrapers/common/log.py
+bank_scrapers/common/values.py
 bank_scrapers/scrapers/__init__.py
 bank_scrapers/scrapers/becu/__init__.py
 bank_scrapers/scrapers/becu/driver.py
 bank_scrapers/scrapers/chase/__init__.py
 bank_scrapers/scrapers/chase/driver.py
 bank_scrapers/scrapers/common/__init__.py
 bank_scrapers/scrapers/common/functions.py
```

### Comparing `bank_scrapers-1.0.7/pyproject.toml` & `bank_scrapers-1.0.8/pyproject.toml`

 * *Files identical despite different names*

