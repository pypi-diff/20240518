# Comparing `tmp/gytmdl-1.7.1.tar.gz` & `tmp/gytmdl-2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gytmdl-1.7.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "gytmdl-2.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `gytmdl-1.7.1.tar` & `gytmdl-2.0.tar`

### file list

```diff
@@ -1,10 +1,12 @@
--rw-r--r--   0        0        0     1176 2023-08-22 04:12:14.567400 gytmdl-1.7.1/.github/workflows/main.yml
--rw-r--r--   0        0        0       80 2023-08-22 04:12:14.567400 gytmdl-1.7.1/.gitignore
--rw-r--r--   0        0        0     3828 2023-08-22 04:12:14.567400 gytmdl-1.7.1/README.md
--rw-r--r--   0        0        0       22 2023-08-22 04:12:14.567400 gytmdl-1.7.1/gytmdl/__init__.py
--rw-r--r--   0        0        0       28 2023-08-22 04:12:14.567400 gytmdl-1.7.1/gytmdl/__main__.py
--rw-r--r--   0        0        0     8368 2023-08-22 04:12:14.567400 gytmdl-1.7.1/gytmdl/cli.py
--rw-r--r--   0        0        0     9639 2023-08-22 04:12:14.567400 gytmdl-1.7.1/gytmdl/dl.py
--rw-r--r--   0        0        0      460 2023-08-22 04:12:14.571400 gytmdl-1.7.1/pyproject.toml
--rw-r--r--   0        0        0       24 2023-08-22 04:12:14.571400 gytmdl-1.7.1/requirements.txt
--rw-r--r--   0        0        0     4175 1970-01-01 00:00:00.000000 gytmdl-1.7.1/PKG-INFO
+-rw-r--r--   0        0        0     1176 2024-05-18 08:07:15.661003 gytmdl-2.0/.github/workflows/main.yml
+-rw-r--r--   0        0        0       80 2024-05-18 08:07:15.661003 gytmdl-2.0/.gitignore
+-rw-r--r--   0        0        0     7282 2024-05-18 08:07:15.661003 gytmdl-2.0/README.md
+-rw-r--r--   0        0        0       20 2024-05-18 08:07:15.661003 gytmdl-2.0/gytmdl/__init__.py
+-rw-r--r--   0        0        0       30 2024-05-18 08:07:15.661003 gytmdl-2.0/gytmdl/__main__.py
+-rw-r--r--   0        0        0    10067 2024-05-18 08:07:15.661003 gytmdl-2.0/gytmdl/cli.py
+-rw-r--r--   0        0        0      422 2024-05-18 08:07:15.661003 gytmdl-2.0/gytmdl/constants.py
+-rw-r--r--   0        0        0    13493 2024-05-18 08:07:15.661003 gytmdl-2.0/gytmdl/downloader.py
+-rw-r--r--   0        0        0      151 2024-05-18 08:07:15.661003 gytmdl-2.0/gytmdl/enums.py
+-rw-r--r--   0        0        0      482 2024-05-18 08:07:15.661003 gytmdl-2.0/pyproject.toml
+-rw-r--r--   0        0        0       35 2024-05-18 08:07:15.661003 gytmdl-2.0/requirements.txt
+-rw-r--r--   0        0        0     7660 1970-01-01 00:00:00.000000 gytmdl-2.0/PKG-INFO
```

### Comparing `gytmdl-1.7.1/.github/workflows/main.yml` & `gytmdl-2.0/.github/workflows/main.yml`

 * *Files identical despite different names*

