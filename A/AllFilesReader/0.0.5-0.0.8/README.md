# Comparing `tmp/allfilesreader-0.0.5.tar.gz` & `tmp/allfilesreader-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "allfilesreader-0.0.5.tar", last modified: Wed May 15 09:39:58 2024, max compression
+gzip compressed data, was "allfilesreader-0.0.8.tar", last modified: Wed May 15 10:07:12 2024, max compression
```

## Comparing `allfilesreader-0.0.5.tar` & `allfilesreader-0.0.8.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 09:39:58.562340 allfilesreader-0.0.5/
--rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-05-15 09:39:25.000000 allfilesreader-0.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1051 2024-05-15 09:39:58.562340 allfilesreader-0.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-05-15 09:39:25.000000 allfilesreader-0.0.5/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      219 2024-05-15 09:39:25.000000 allfilesreader-0.0.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      539 2024-05-15 09:39:58.566340 allfilesreader-0.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      852 2024-05-15 09:39:25.000000 allfilesreader-0.0.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 09:39:58.558340 allfilesreader-0.0.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 09:39:58.562340 allfilesreader-0.0.5/src/AllFilesReader.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1051 2024-05-15 09:39:58.000000 allfilesreader-0.0.5/src/AllFilesReader.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      386 2024-05-15 09:39:58.000000 allfilesreader-0.0.5/src/AllFilesReader.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 09:39:58.000000 allfilesreader-0.0.5/src/AllFilesReader.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-15 09:39:58.000000 allfilesreader-0.0.5/src/AllFilesReader.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-15 09:39:58.000000 allfilesreader-0.0.5/src/AllFilesReader.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 09:39:58.562340 allfilesreader-0.0.5/src/all_files_reader/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 09:39:25.000000 allfilesreader-0.0.5/src/all_files_reader/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4356 2024-05-15 09:39:25.000000 allfilesreader-0.0.5/src/all_files_reader/filereader_crud.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 09:39:58.562340 allfilesreader-0.0.5/src/exception/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 09:39:25.000000 allfilesreader-0.0.5/src/exception/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      118 2024-05-15 09:39:25.000000 allfilesreader-0.0.5/src/exception/exception.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 10:07:12.234093 allfilesreader-0.0.8/
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-05-15 10:06:41.000000 allfilesreader-0.0.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2563 2024-05-15 10:07:12.234093 allfilesreader-0.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1625 2024-05-15 10:06:41.000000 allfilesreader-0.0.8/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      219 2024-05-15 10:06:41.000000 allfilesreader-0.0.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      539 2024-05-15 10:07:12.234093 allfilesreader-0.0.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      877 2024-05-15 10:06:41.000000 allfilesreader-0.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 10:07:12.230093 allfilesreader-0.0.8/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 10:07:12.234093 allfilesreader-0.0.8/src/AllFilesReader.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2563 2024-05-15 10:07:12.000000 allfilesreader-0.0.8/src/AllFilesReader.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      386 2024-05-15 10:07:12.000000 allfilesreader-0.0.8/src/AllFilesReader.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 10:07:12.000000 allfilesreader-0.0.8/src/AllFilesReader.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-15 10:07:12.000000 allfilesreader-0.0.8/src/AllFilesReader.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-15 10:07:12.000000 allfilesreader-0.0.8/src/AllFilesReader.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 10:07:12.234093 allfilesreader-0.0.8/src/all_files_reader/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 10:06:41.000000 allfilesreader-0.0.8/src/all_files_reader/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4356 2024-05-15 10:06:41.000000 allfilesreader-0.0.8/src/all_files_reader/filereader_crud.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 10:07:12.234093 allfilesreader-0.0.8/src/exception/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 10:06:41.000000 allfilesreader-0.0.8/src/exception/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      118 2024-05-15 10:06:41.000000 allfilesreader-0.0.8/src/exception/exception.py
```

### Comparing `allfilesreader-0.0.5/LICENSE` & `allfilesreader-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `allfilesreader-0.0.5/setup.cfg` & `allfilesreader-0.0.8/setup.cfg`

 * *Files identical despite different names*

### Comparing `allfilesreader-0.0.5/setup.py` & `allfilesreader-0.0.8/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 from setuptools import setup, find_packages
 from typing import List
 
 with open('README.md', 'r', encoding='utf-8') as f:
     long_description = f.read()     
-   
 
-__version__ = "0.0.5"
+__version__ = "0.0.8"
 REPO_NAME = "AllFilesReaderPythonLibrary"
 PKG_NAME= "AllFilesReader"
 AUTHOR_USER_NAME = "iamdoublea"
 AUTHOR_EMAIL = "contact@aadityaseal.com"
 
 setup(
     name=PKG_NAME,
     version=__version__,
     author=AUTHOR_USER_NAME,
     author_email=AUTHOR_EMAIL,
     description="A python package to read all kinds of file with just one click",
     long_description=long_description,
-    long_description_content="text/markdown",
+    long_description_content_type="text/markdown",  # Corrected argument name
     url=f"https://github.com/{AUTHOR_USER_NAME}/{REPO_NAME}",
     project_urls={
         "Bug Tracker": f"https://github.com/{AUTHOR_USER_NAME}/{REPO_NAME}/issues"
     },
     package_dir={"": "src"},
     packages=find_packages(where="src"),
-    )
+)
```

### Comparing `allfilesreader-0.0.5/src/all_files_reader/filereader_crud.py` & `allfilesreader-0.0.8/src/all_files_reader/filereader_crud.py`

 * *Files identical despite different names*

