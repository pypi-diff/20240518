# Comparing `tmp/aiconn-0.0.1.tar.gz` & `tmp/aiconn-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiconn-0.0.1.tar", last modified: Sat May 18 14:11:01 2024, max compression
+gzip compressed data, was "aiconn-0.0.2.tar", last modified: Sat May 18 14:20:32 2024, max compression
```

## Comparing `aiconn-0.0.1.tar` & `aiconn-0.0.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 mrthinh    (501) staff       (20)        0 2024-05-18 14:11:01.274025 aiconn-0.0.1/
--rw-r--r--   0 mrthinh    (501) staff       (20)      401 2024-05-18 14:11:01.273942 aiconn-0.0.1/PKG-INFO
--rw-r--r--   0 mrthinh    (501) staff       (20)       25 2024-05-18 13:40:58.000000 aiconn-0.0.1/README.md
-drwxr-xr-x   0 mrthinh    (501) staff       (20)        0 2024-05-18 14:11:01.272553 aiconn-0.0.1/aiconn/
--rw-r--r--   0 mrthinh    (501) staff       (20)       21 2024-05-18 13:41:57.000000 aiconn-0.0.1/aiconn/__init__.py
--rw-r--r--   0 mrthinh    (501) staff       (20)     8567 2024-05-18 13:53:44.000000 aiconn-0.0.1/aiconn/gemini.py
--rw-r--r--   0 mrthinh    (501) staff       (20)      210 2024-05-18 13:48:03.000000 aiconn-0.0.1/aiconn/utils.py
-drwxr-xr-x   0 mrthinh    (501) staff       (20)        0 2024-05-18 14:11:01.273698 aiconn-0.0.1/aiconn.egg-info/
--rw-r--r--   0 mrthinh    (501) staff       (20)      401 2024-05-18 14:11:01.000000 aiconn-0.0.1/aiconn.egg-info/PKG-INFO
--rw-r--r--   0 mrthinh    (501) staff       (20)      206 2024-05-18 14:11:01.000000 aiconn-0.0.1/aiconn.egg-info/SOURCES.txt
--rw-r--r--   0 mrthinh    (501) staff       (20)        1 2024-05-18 14:11:01.000000 aiconn-0.0.1/aiconn.egg-info/dependency_links.txt
--rw-r--r--   0 mrthinh    (501) staff       (20)        7 2024-05-18 14:11:01.000000 aiconn-0.0.1/aiconn.egg-info/top_level.txt
--rw-r--r--   0 mrthinh    (501) staff       (20)      150 2024-05-18 13:45:03.000000 aiconn-0.0.1/pyproject.toml
--rw-r--r--   0 mrthinh    (501) staff       (20)      474 2024-05-18 14:11:01.274283 aiconn-0.0.1/setup.cfg
+drwxr-xr-x   0 mrthinh    (501) staff       (20)        0 2024-05-18 14:20:32.567089 aiconn-0.0.2/
+-rw-r--r--   0 mrthinh    (501) staff       (20)      401 2024-05-18 14:20:32.567016 aiconn-0.0.2/PKG-INFO
+-rw-r--r--   0 mrthinh    (501) staff       (20)       25 2024-05-18 13:40:58.000000 aiconn-0.0.2/README.md
+drwxr-xr-x   0 mrthinh    (501) staff       (20)        0 2024-05-18 14:20:32.565884 aiconn-0.0.2/aiconn/
+-rw-r--r--   0 mrthinh    (501) staff       (20)       21 2024-05-18 13:41:57.000000 aiconn-0.0.2/aiconn/__init__.py
+-rw-r--r--   0 mrthinh    (501) staff       (20)     8567 2024-05-18 13:53:44.000000 aiconn-0.0.2/aiconn/gemini.py
+-rw-r--r--   0 mrthinh    (501) staff       (20)      185 2024-05-18 14:15:07.000000 aiconn-0.0.2/aiconn/utils.py
+drwxr-xr-x   0 mrthinh    (501) staff       (20)        0 2024-05-18 14:20:32.566796 aiconn-0.0.2/aiconn.egg-info/
+-rw-r--r--   0 mrthinh    (501) staff       (20)      401 2024-05-18 14:20:32.000000 aiconn-0.0.2/aiconn.egg-info/PKG-INFO
+-rw-r--r--   0 mrthinh    (501) staff       (20)      206 2024-05-18 14:20:32.000000 aiconn-0.0.2/aiconn.egg-info/SOURCES.txt
+-rw-r--r--   0 mrthinh    (501) staff       (20)        1 2024-05-18 14:20:32.000000 aiconn-0.0.2/aiconn.egg-info/dependency_links.txt
+-rw-r--r--   0 mrthinh    (501) staff       (20)        7 2024-05-18 14:20:32.000000 aiconn-0.0.2/aiconn.egg-info/top_level.txt
+-rw-r--r--   0 mrthinh    (501) staff       (20)      150 2024-05-18 13:45:03.000000 aiconn-0.0.2/pyproject.toml
+-rw-r--r--   0 mrthinh    (501) staff       (20)      474 2024-05-18 14:20:32.567328 aiconn-0.0.2/setup.cfg
```

### Comparing `aiconn-0.0.1/aiconn/gemini.py` & `aiconn-0.0.2/aiconn/gemini.py`

 * *Files identical despite different names*

