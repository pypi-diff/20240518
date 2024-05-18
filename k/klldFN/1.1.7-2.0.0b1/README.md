# Comparing `tmp/klldFN-1.1.7.tar.gz` & `tmp/klldFN-2.0.0b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "klldFN-1.1.7.tar", last modified: Fri Mar  1 20:18:06 2024, max compression
+gzip compressed data, was "klldFN-2.0.0b1.tar", last modified: Sat May 18 16:01:32 2024, max compression
```

## Comparing `klldFN-1.1.7.tar` & `klldFN-2.0.0b1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-01 20:18:06.007396 klldFN-1.1.7/
--rw-r--r--   0 runner    (1000) runner    (1000)      344 2024-03-01 20:18:06.003395 klldFN-1.1.7/PKG-INFO
--rw-r--r--   0 runner    (1000) runner    (1000)       47 2023-07-12 17:45:01.000000 klldFN-1.1.7/README.md
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-01 20:18:06.003395 klldFN-1.1.7/klldFN/
--rw-r--r--   0 runner    (1000) runner    (1000)    77363 2024-03-01 20:09:13.000000 klldFN-1.1.7/klldFN/__init__.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-01 20:18:06.003395 klldFN-1.1.7/klldFN.egg-info/
--rw-r--r--   0 runner    (1000) runner    (1000)      344 2024-03-01 20:18:05.000000 klldFN-1.1.7/klldFN.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1000) runner    (1000)      201 2024-03-01 20:18:05.000000 klldFN-1.1.7/klldFN.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1000) runner    (1000)        1 2024-03-01 20:18:05.000000 klldFN-1.1.7/klldFN.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1000) runner    (1000)      105 2024-03-01 20:18:05.000000 klldFN-1.1.7/klldFN.egg-info/requires.txt
--rw-r--r--   0 runner    (1000) runner    (1000)        7 2024-03-01 20:18:05.000000 klldFN-1.1.7/klldFN.egg-info/top_level.txt
--rw-r--r--   0 runner    (1000) runner    (1000)      471 2022-10-20 21:31:04.000000 klldFN-1.1.7/pyproject.toml
--rw-r--r--   0 runner    (1000) runner    (1000)       38 2024-03-01 20:18:06.007396 klldFN-1.1.7/setup.cfg
--rw-r--r--   0 runner    (1000) runner    (1000)      767 2024-03-01 20:10:14.000000 klldFN-1.1.7/setup.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-05-18 16:01:32.433221 klldFN-2.0.0b1/
+-rw-r--r--   0 runner    (1000) runner    (1000)     1052 2024-05-18 16:01:32.433221 klldFN-2.0.0b1/PKG-INFO
+-rw-r--r--   0 runner    (1000) runner    (1000)       64 2024-05-18 12:28:14.000000 klldFN-2.0.0b1/README.md
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-05-18 16:01:32.425220 klldFN-2.0.0b1/klldFN/
+-rw-r--r--   0 runner    (1000) runner    (1000)   134565 2024-05-18 13:15:51.000000 klldFN-2.0.0b1/klldFN/__init__.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-05-18 16:01:32.429221 klldFN-2.0.0b1/klldFN.egg-info/
+-rw-r--r--   0 runner    (1000) runner    (1000)     1052 2024-05-18 16:01:32.000000 klldFN-2.0.0b1/klldFN.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1000) runner    (1000)      201 2024-05-18 16:01:32.000000 klldFN-2.0.0b1/klldFN.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)        1 2024-05-18 16:01:32.000000 klldFN-2.0.0b1/klldFN.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)      102 2024-05-18 16:01:32.000000 klldFN-2.0.0b1/klldFN.egg-info/requires.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)        7 2024-05-18 16:01:32.000000 klldFN-2.0.0b1/klldFN.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)      494 2024-04-12 16:24:13.000000 klldFN-2.0.0b1/pyproject.toml
+-rw-r--r--   0 runner    (1000) runner    (1000)       38 2024-05-18 16:01:32.433221 klldFN-2.0.0b1/setup.cfg
+-rw-r--r--   0 runner    (1000) runner    (1000)     1248 2024-05-18 15:56:57.000000 klldFN-2.0.0b1/setup.py
```

