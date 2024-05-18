# Comparing `tmp/lora-modem-1.4.0.tar.gz` & `tmp/lora_modem-1.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lora-modem-1.4.0.tar", last modified: Sat Apr  6 15:22:19 2024, max compression
+gzip compressed data, was "lora_modem-1.4.1.tar", last modified: Sat May 18 14:54:47 2024, max compression
```

## Comparing `lora-modem-1.4.0.tar` & `lora_modem-1.4.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 janakj     (501) staff       (20)        0 2024-04-06 15:22:19.058203 lora-modem-1.4.0/
--rw-r--r--   0 janakj     (501) staff       (20)     1491 2024-04-06 15:21:57.000000 lora-modem-1.4.0/LICENSE
--rw-r--r--   0 janakj     (501) staff       (20)     9885 2024-04-06 15:22:19.057975 lora-modem-1.4.0/PKG-INFO
--rw-r--r--   0 janakj     (501) staff       (20)     6935 2024-04-06 15:21:57.000000 lora-modem-1.4.0/README.md
--rwxr-xr-x   0 janakj     (501) staff       (20)   214289 2024-04-06 15:21:57.000000 lora-modem-1.4.0/lora.py
-drwxr-xr-x   0 janakj     (501) staff       (20)        0 2024-04-06 15:22:19.057510 lora-modem-1.4.0/lora_modem.egg-info/
--rw-r--r--   0 janakj     (501) staff       (20)     9885 2024-04-06 15:22:19.000000 lora-modem-1.4.0/lora_modem.egg-info/PKG-INFO
--rw-r--r--   0 janakj     (501) staff       (20)      246 2024-04-06 15:22:19.000000 lora-modem-1.4.0/lora_modem.egg-info/SOURCES.txt
--rw-r--r--   0 janakj     (501) staff       (20)        1 2024-04-06 15:22:19.000000 lora-modem-1.4.0/lora_modem.egg-info/dependency_links.txt
--rw-r--r--   0 janakj     (501) staff       (20)       34 2024-04-06 15:22:19.000000 lora-modem-1.4.0/lora_modem.egg-info/entry_points.txt
--rw-r--r--   0 janakj     (501) staff       (20)      133 2024-04-06 15:22:19.000000 lora-modem-1.4.0/lora_modem.egg-info/requires.txt
--rw-r--r--   0 janakj     (501) staff       (20)        5 2024-04-06 15:22:19.000000 lora-modem-1.4.0/lora_modem.egg-info/top_level.txt
--rw-r--r--   0 janakj     (501) staff       (20)     1414 2024-04-06 15:21:57.000000 lora-modem-1.4.0/pyproject.toml
--rw-r--r--   0 janakj     (501) staff       (20)       38 2024-04-06 15:22:19.058247 lora-modem-1.4.0/setup.cfg
+drwxr-xr-x   0 janakj     (501) staff       (20)        0 2024-05-18 14:54:47.908694 lora_modem-1.4.1/
+-rw-r--r--   0 janakj     (501) staff       (20)     1491 2024-05-18 14:54:27.000000 lora_modem-1.4.1/LICENSE
+-rw-r--r--   0 janakj     (501) staff       (20)     9885 2024-05-18 14:54:47.908446 lora_modem-1.4.1/PKG-INFO
+-rw-r--r--   0 janakj     (501) staff       (20)     6935 2024-05-18 14:54:27.000000 lora_modem-1.4.1/README.md
+-rwxr-xr-x   0 janakj     (501) staff       (20)   214289 2024-05-18 14:54:27.000000 lora_modem-1.4.1/lora.py
+drwxr-xr-x   0 janakj     (501) staff       (20)        0 2024-05-18 14:54:47.908022 lora_modem-1.4.1/lora_modem.egg-info/
+-rw-r--r--   0 janakj     (501) staff       (20)     9885 2024-05-18 14:54:47.000000 lora_modem-1.4.1/lora_modem.egg-info/PKG-INFO
+-rw-r--r--   0 janakj     (501) staff       (20)      246 2024-05-18 14:54:47.000000 lora_modem-1.4.1/lora_modem.egg-info/SOURCES.txt
+-rw-r--r--   0 janakj     (501) staff       (20)        1 2024-05-18 14:54:47.000000 lora_modem-1.4.1/lora_modem.egg-info/dependency_links.txt
+-rw-r--r--   0 janakj     (501) staff       (20)       34 2024-05-18 14:54:47.000000 lora_modem-1.4.1/lora_modem.egg-info/entry_points.txt
+-rw-r--r--   0 janakj     (501) staff       (20)      133 2024-05-18 14:54:47.000000 lora_modem-1.4.1/lora_modem.egg-info/requires.txt
+-rw-r--r--   0 janakj     (501) staff       (20)        5 2024-05-18 14:54:47.000000 lora_modem-1.4.1/lora_modem.egg-info/top_level.txt
+-rw-r--r--   0 janakj     (501) staff       (20)     1414 2024-05-18 14:54:27.000000 lora_modem-1.4.1/pyproject.toml
+-rw-r--r--   0 janakj     (501) staff       (20)       38 2024-05-18 14:54:47.908728 lora_modem-1.4.1/setup.cfg
```

### Comparing `lora-modem-1.4.0/LICENSE` & `lora_modem-1.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `lora-modem-1.4.0/PKG-INFO` & `lora_modem-1.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lora-modem
-Version: 1.4.0
+Version: 1.4.1
 Summary: Python library for the Murata TypeABZ LoRaWAN modem
 Author-email: Jan Janak <jan@janakj.org>
 License: Copyright (c) 2022 Jan Janak <jan@janakj.org>
         
         Redistribution and use in source and binary forms, with or without modification,
         are permitted provided that the following conditions are met:
```

### Comparing `lora-modem-1.4.0/README.md` & `lora_modem-1.4.1/README.md`

 * *Files identical despite different names*

### Comparing `lora-modem-1.4.0/lora.py` & `lora_modem-1.4.1/lora.py`

 * *Files identical despite different names*

### Comparing `lora-modem-1.4.0/lora_modem.egg-info/PKG-INFO` & `lora_modem-1.4.1/lora_modem.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lora-modem
-Version: 1.4.0
+Version: 1.4.1
 Summary: Python library for the Murata TypeABZ LoRaWAN modem
 Author-email: Jan Janak <jan@janakj.org>
 License: Copyright (c) 2022 Jan Janak <jan@janakj.org>
         
         Redistribution and use in source and binary forms, with or without modification,
         are permitted provided that the following conditions are met:
```

### Comparing `lora-modem-1.4.0/pyproject.toml` & `lora_modem-1.4.1/pyproject.toml`

 * *Files identical despite different names*

