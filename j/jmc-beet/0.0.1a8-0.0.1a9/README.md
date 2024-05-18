# Comparing `tmp/jmc-beet-0.0.1a8.tar.gz` & `tmp/jmc-beet-0.0.1a9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jmc-beet-0.0.1a8.tar", last modified: Thu Sep 28 05:32:48 2023, max compression
+gzip compressed data, was "jmc-beet-0.0.1a9.tar", last modified: Sat May 18 19:30:45 2024, max compression
```

## Comparing `jmc-beet-0.0.1a8.tar` & `jmc-beet-0.0.1a9.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-09-28 05:32:48.407374 jmc-beet-0.0.1a8/
--rw-rw-rw-   0        0        0      895 2023-09-28 05:32:48.405371 jmc-beet-0.0.1a8/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-09-28 05:32:48.394949 jmc-beet-0.0.1a8/jmc_beet.egg-info/
--rw-rw-rw-   0        0        0      895 2023-09-28 05:32:47.000000 jmc-beet-0.0.1a8/jmc_beet.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      260 2023-09-28 05:32:48.000000 jmc-beet-0.0.1a8/jmc_beet.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-09-28 05:32:47.000000 jmc-beet-0.0.1a8/jmc_beet.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       50 2023-09-28 05:32:47.000000 jmc-beet-0.0.1a8/jmc_beet.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       17 2023-09-28 05:32:47.000000 jmc-beet-0.0.1a8/jmc_beet.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-09-28 05:32:47.000000 jmc-beet-0.0.1a8/jmc_beet.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-09-28 05:32:48.402865 jmc-beet-0.0.1a8/jmcbeet/
--rw-rw-rw-   0        0        0     3326 2023-09-28 05:30:45.000000 jmc-beet-0.0.1a8/jmcbeet/__init__.py
--rw-rw-rw-   0        0        0     1870 2023-09-14 09:31:33.000000 jmc-beet-0.0.1a8/jmcbeet/__main__.py
--rw-rw-rw-   0        0        0       28 2023-09-28 05:32:25.000000 jmc-beet-0.0.1a8/jmcbeet/config.py
--rw-rw-rw-   0        0        0       42 2023-09-28 05:32:48.407374 jmc-beet-0.0.1a8/setup.cfg
--rw-rw-rw-   0        0        0     1534 2023-09-14 09:08:19.000000 jmc-beet-0.0.1a8/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-18 19:30:45.307227 jmc-beet-0.0.1a9/
+-rw-rw-rw-   0        0        0      895 2024-05-18 19:30:45.305351 jmc-beet-0.0.1a9/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-18 19:30:45.292607 jmc-beet-0.0.1a9/jmc_beet.egg-info/
+-rw-rw-rw-   0        0        0      895 2024-05-18 19:30:44.000000 jmc-beet-0.0.1a9/jmc_beet.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      260 2024-05-18 19:30:44.000000 jmc-beet-0.0.1a9/jmc_beet.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-18 19:30:44.000000 jmc-beet-0.0.1a9/jmc_beet.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       50 2024-05-18 19:30:44.000000 jmc-beet-0.0.1a9/jmc_beet.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       17 2024-05-18 19:30:44.000000 jmc-beet-0.0.1a9/jmc_beet.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-05-18 19:30:44.000000 jmc-beet-0.0.1a9/jmc_beet.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-18 19:30:45.301705 jmc-beet-0.0.1a9/jmcbeet/
+-rw-rw-rw-   0        0        0     3328 2024-05-18 19:26:47.000000 jmc-beet-0.0.1a9/jmcbeet/__init__.py
+-rw-rw-rw-   0        0        0     1870 2023-09-14 09:31:33.000000 jmc-beet-0.0.1a9/jmcbeet/__main__.py
+-rw-rw-rw-   0        0        0       28 2024-05-18 19:30:28.000000 jmc-beet-0.0.1a9/jmcbeet/config.py
+-rw-rw-rw-   0        0        0       42 2024-05-18 19:30:45.308240 jmc-beet-0.0.1a9/setup.cfg
+-rw-rw-rw-   0        0        0     1534 2023-09-14 09:08:19.000000 jmc-beet-0.0.1a9/setup.py
```

### Comparing `jmc-beet-0.0.1a8/PKG-INFO` & `jmc-beet-0.0.1a9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jmc-beet
-Version: 0.0.1a8
+Version: 0.0.1a9
 Summary: A Beet plugin that act as an adapter for JMC
 Author: WingedSeal
 Author-email: firm09719@gmail.com
 License: MIT License
 Project-URL: Documentation, https://jmc.wingedseal.com/
 Project-URL: Repository, https://github.com/WingedSeal/jmc-beet
 Keywords: python,minecraft,mcfunction,datapack,compiler,beet
```

### Comparing `jmc-beet-0.0.1a8/jmc_beet.egg-info/PKG-INFO` & `jmc-beet-0.0.1a9/jmc_beet.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jmc-beet
-Version: 0.0.1a8
+Version: 0.0.1a9
 Summary: A Beet plugin that act as an adapter for JMC
 Author: WingedSeal
 Author-email: firm09719@gmail.com
 License: MIT License
 Project-URL: Documentation, https://jmc.wingedseal.com/
 Project-URL: Repository, https://github.com/WingedSeal/jmc-beet
 Keywords: python,minecraft,mcfunction,datapack,compiler,beet
```

### Comparing `jmc-beet-0.0.1a8/jmcbeet/__init__.py` & `jmc-beet-0.0.1a9/jmcbeet/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -93,15 +93,15 @@
     for key, value in DEFAULT_JMC_TXT.items():
         jmc_txt[key] = ctx.meta["jmc"].get(key, value)
 
     try:
         jmc_pack = PyJMC(
             namespace,
             description="",
-            pack_format="-1",
+            pack_format="9999",
             target=file_path,
             jmc_txt=jmc_txt)
     except JMC_EXCEPTIONS as error:
         print("JMC-Warning | JMC Error has occured")
         print(type(error).__name__)
         print(error)
         return
```

### Comparing `jmc-beet-0.0.1a8/jmcbeet/__main__.py` & `jmc-beet-0.0.1a9/jmcbeet/__main__.py`

 * *Files identical despite different names*

### Comparing `jmc-beet-0.0.1a8/setup.py` & `jmc-beet-0.0.1a9/setup.py`

 * *Files identical despite different names*

