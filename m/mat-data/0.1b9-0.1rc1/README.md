# Comparing `tmp/mat-data-0.1b9.tar.gz` & `tmp/mat_data-0.1rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mat-data-0.1b9.tar", last modified: Sun Dec 17 10:35:00 2023, max compression
+gzip compressed data, was "mat_data-0.1rc1.tar", last modified: Fri May 17 22:54:36 2024, max compression
```

## Comparing `mat-data-0.1b9.tar` & `mat_data-0.1rc1.tar`

### file list

```diff
@@ -1,32 +1,102 @@
-drwxr-xr-x   0 tarlisportela   (501) staff       (20)        0 2023-12-17 10:35:00.482799 mat-data-0.1b9/
--rw-r--r--   0 tarlisportela   (501) staff       (20)       86 2023-12-16 13:47:10.000000 mat-data-0.1b9/CHANGELOG.md
--rw-r--r--   0 tarlisportela   (501) staff       (20)    35129 2023-12-15 20:34:29.000000 mat-data-0.1b9/LICENSE
--rw-r--r--   0 tarlisportela   (501) staff       (20)      147 2023-12-15 20:28:19.000000 mat-data-0.1b9/MANIFEST.in
--rw-r--r--   0 tarlisportela   (501) staff       (20)   598446 2023-12-16 13:33:41.000000 mat-data-0.1b9/MAT-data-Tutorial.html
--rwx------   0 tarlisportela   (501) staff       (20)    43673 2023-12-17 04:10:42.000000 mat-data-0.1b9/MAT-data-Tutorial.ipynb
--rw-r--r--   0 tarlisportela   (501) staff       (20)     5435 2023-12-17 10:35:00.482381 mat-data-0.1b9/PKG-INFO
--rw-r--r--   0 tarlisportela   (501) staff       (20)     3165 2023-12-16 13:44:41.000000 mat-data-0.1b9/README.md
--rw-r--r--   0 tarlisportela   (501) staff       (20)      717 2023-12-16 03:29:23.000000 mat-data-0.1b9/Steps to Build.txt
-drwxr-xr-x   0 tarlisportela   (501) staff       (20)        0 2023-12-17 10:35:00.481400 mat-data-0.1b9/mat_data.egg-info/
--rw-r--r--   0 tarlisportela   (501) staff       (20)     5435 2023-12-17 10:35:00.000000 mat-data-0.1b9/mat_data.egg-info/PKG-INFO
--rw-r--r--   0 tarlisportela   (501) staff       (20)      522 2023-12-17 10:35:00.000000 mat-data-0.1b9/mat_data.egg-info/SOURCES.txt
--rw-r--r--   0 tarlisportela   (501) staff       (20)        1 2023-12-17 10:35:00.000000 mat-data-0.1b9/mat_data.egg-info/dependency_links.txt
--rw-r--r--   0 tarlisportela   (501) staff       (20)      148 2023-12-17 10:35:00.000000 mat-data-0.1b9/mat_data.egg-info/requires.txt
--rw-r--r--   0 tarlisportela   (501) staff       (20)        8 2023-12-17 10:35:00.000000 mat-data-0.1b9/mat_data.egg-info/top_level.txt
-drwxr-xr-x   0 tarlisportela   (501) staff       (20)        0 2023-12-17 10:35:00.467044 mat-data-0.1b9/matdata/
--rw-r--r--   0 tarlisportela   (501) staff       (20)    35129 2023-12-15 20:34:29.000000 mat-data-0.1b9/matdata/LICENSE
--rw-r--r--   0 tarlisportela   (501) staff       (20)     3165 2023-12-16 13:44:41.000000 mat-data-0.1b9/matdata/README.md
--rw-r--r--   0 tarlisportela   (501) staff       (20)        0 2023-12-15 20:25:37.000000 mat-data-0.1b9/matdata/__init__.py
-drwxr-xr-x   0 tarlisportela   (501) staff       (20)        0 2023-12-17 10:35:00.460065 mat-data-0.1b9/matdata/assets/
-drwxr-xr-x   0 tarlisportela   (501) staff       (20)        0 2023-12-17 10:35:00.468067 mat-data-0.1b9/matdata/assets/sample/
--rw-rw-r--   0 tarlisportela   (501) staff       (20)  7716732 2021-02-10 16:01:46.000000 mat-data-0.1b9/matdata/assets/sample/Foursquare_Sample.csv
--rw-r--r--   0 tarlisportela   (501) staff       (20)     6080 2023-12-17 04:02:29.000000 mat-data-0.1b9/matdata/datasets.py
--rw-r--r--   0 tarlisportela   (501) staff       (20)    26386 2023-12-16 17:27:28.000000 mat-data-0.1b9/matdata/generator.py
-drwxr-xr-x   0 tarlisportela   (501) staff       (20)        0 2023-12-17 10:35:00.479147 mat-data-0.1b9/matdata/inc/
--rw-r--r--   0 tarlisportela   (501) staff       (20)        0 2023-12-15 20:26:21.000000 mat-data-0.1b9/matdata/inc/__init__.py
--rw-r--r--   0 tarlisportela   (501) staff       (20)    13708 2023-12-16 17:42:48.000000 mat-data-0.1b9/matdata/inc/converter.py
--rw-r--r--   0 tarlisportela   (501) staff       (20)    52699 2023-12-16 17:28:01.000000 mat-data-0.1b9/matdata/inc/ts_io.py
--rw-r--r--   0 tarlisportela   (501) staff       (20)    34728 2023-12-17 10:34:32.000000 mat-data-0.1b9/matdata/preprocess.py
--rw-r--r--   0 tarlisportela   (501) staff       (20)     2131 2023-12-17 10:34:44.000000 mat-data-0.1b9/pyproject.toml
--rw-r--r--   0 tarlisportela   (501) staff       (20)       38 2023-12-17 10:35:00.482859 mat-data-0.1b9/setup.cfg
--rw-r--r--   0 tarlisportela   (501) staff       (20)     2340 2023-12-16 04:06:58.000000 mat-data-0.1b9/setup.py
+drwxr-xr-x   0 tarlisportela   (501) staff       (20)        0 2024-05-17 22:54:36.394972 mat_data-0.1rc1/
+-rw-r--r--   0 tarlisportela   (501) staff       (20)       86 2023-12-16 13:47:10.000000 mat_data-0.1rc1/CHANGELOG.md
+-rw-r--r--   0 tarlisportela   (501) staff       (20)    35129 2023-12-15 20:34:29.000000 mat_data-0.1rc1/LICENSE
+-rw-r--r--   0 tarlisportela   (501) staff       (20)      147 2023-12-15 20:28:19.000000 mat_data-0.1rc1/MANIFEST.in
+-rw-r--r--   0 tarlisportela   (501) staff       (20)   711915 2024-05-17 19:13:21.000000 mat_data-0.1rc1/MAT-data-Tutorial.html
+-rwx------   0 tarlisportela   (501) staff       (20)   159189 2024-05-17 19:07:25.000000 mat_data-0.1rc1/MAT-data-Tutorial.ipynb
+-rw-r--r--   0 tarlisportela   (501) staff       (20)     5678 2024-05-17 22:54:36.394764 mat_data-0.1rc1/PKG-INFO
+-rw-r--r--   0 tarlisportela   (501) staff       (20)     3304 2024-04-17 14:32:21.000000 mat_data-0.1rc1/README.md
+-rw-r--r--   0 tarlisportela   (501) staff       (20)      717 2023-12-16 03:29:23.000000 mat_data-0.1rc1/Steps to Build.txt
+drwxr-xr-x   0 tarlisportela   (501) staff       (20)        0 2024-05-17 22:54:36.358597 mat_data-0.1rc1/docs/
+-rw-r--r--   0 tarlisportela   (501) staff       (20)      638 2024-05-17 20:33:21.000000 mat_data-0.1rc1/docs/Makefile
+drwxr-xr-x   0 tarlisportela   (501) staff       (20)        0 2024-05-17 22:54:36.355018 mat_data-0.1rc1/docs/build/
+drwxr-xr-x   0 tarlisportela   (501) staff       (20)        0 2024-05-17 22:54:36.365017 mat_data-0.1rc1/docs/build/doctrees/
+-rw-r--r--   0 tarlisportela   (501) staff       (20)   125480 2024-05-17 22:43:40.000000 mat_data-0.1rc1/docs/build/doctrees/converter..doctree
+-rw-r--r--   0 tarlisportela   (501) staff       (20)   125479 2024-05-17 22:44:00.000000 mat_data-0.1rc1/docs/build/doctrees/converter.doctree
+-rw-r--r--   0 tarlisportela   (501) staff       (20)    93332 2024-05-17 22:43:41.000000 mat_data-0.1rc1/docs/build/doctrees/dataset..doctree
+-rw-r--r--   0 tarlisportela   (501) staff       (20)    93331 2024-05-17 22:44:00.000000 mat_data-0.1rc1/docs/build/doctrees/dataset.doctree
+-rw-r--r--   0 tarlisportela   (501) staff       (20)  1370204 2024-05-17 22:49:56.000000 mat_data-0.1rc1/docs/build/doctrees/environment.pickle
+-rw-r--r--   0 tarlisportela   (501) staff       (20)    69349 2024-05-17 22:43:41.000000 mat_data-0.1rc1/docs/build/doctrees/generator..doctree
+-rw-r--r--   0 tarlisportela   (501) staff       (20)    69348 2024-05-17 22:44:00.000000 mat_data-0.1rc1/docs/build/doctrees/generator.doctree
+-rw-r--r--   0 tarlisportela   (501) staff       (20)    27029 2024-05-17 22:43:41.000000 mat_data-0.1rc1/docs/build/doctrees/index..doctree
+-rw-r--r--   0 tarlisportela   (501) staff       (20)  1207885 2024-05-17 22:49:56.000000 mat_data-0.1rc1/docs/build/doctrees/index.doctree
+-rw-r--r--   0 tarlisportela   (501) staff       (20)   150235 2024-05-17 22:43:41.000000 mat_data-0.1rc1/docs/build/doctrees/preprocess..doctree
+-rw-r--r--   0 tarlisportela   (501) staff       (20)   150234 2024-05-17 22:44:00.000000 mat_data-0.1rc1/docs/build/doctrees/preprocess.doctree
+drwxr-xr-x   0 tarlisportela   (501) staff       (20)        0 2024-05-17 22:54:36.367740 mat_data-0.1rc1/docs/build/html/
+-rw-r--r--   0 tarlisportela   (501) staff       (20)      230 2024-05-17 22:49:56.000000 mat_data-0.1rc1/docs/build/html/.buildinfo
+drwxr-xr-x   0 tarlisportela   (501) staff       (20)        0 2024-05-17 22:54:36.367900 mat_data-0.1rc1/docs/build/html/_modules/
+-rw-r--r--   0 tarlisportela   (501) staff       (20)     3093 2024-05-17 22:49:56.000000 mat_data-0.1rc1/docs/build/html/_modules/index.html
+drwxr-xr-x   0 tarlisportela   (501) staff       (20)        0 2024-05-17 22:54:36.368609 mat_data-0.1rc1/docs/build/html/_modules/matdata/
+-rw-r--r--   0 tarlisportela   (501) staff       (20)    90321 2024-05-17 22:44:01.000000 mat_data-0.1rc1/docs/build/html/_modules/matdata/converter.html
+-rw-r--r--   0 tarlisportela   (501) staff       (20)    70051 2024-05-17 22:44:01.000000 mat_data-0.1rc1/docs/build/html/_modules/matdata/dataset.html
+-rw-r--r--   0 tarlisportela   (501) staff       (20)   129545 2024-05-17 22:44:01.000000 mat_data-0.1rc1/docs/build/html/_modules/matdata/generator.html
+-rw-r--r--   0 tarlisportela   (501) staff       (20)   181043 2024-05-17 22:44:01.000000 mat_data-0.1rc1/docs/build/html/_modules/matdata/preprocess.html
+drwxr-xr-x   0 tarlisportela   (501) staff       (20)        0 2024-05-17 22:54:36.369410 mat_data-0.1rc1/docs/build/html/_sources/
+-rw-r--r--   0 tarlisportela   (501) staff       (20)       66 2024-05-17 21:13:53.000000 mat_data-0.1rc1/docs/build/html/_sources/converter.rst.txt
+-rw-r--r--   0 tarlisportela   (501) staff       (20)       60 2024-05-17 21:13:51.000000 mat_data-0.1rc1/docs/build/html/_sources/dataset.rst.txt
+-rw-r--r--   0 tarlisportela   (501) staff       (20)       66 2024-05-17 21:29:32.000000 mat_data-0.1rc1/docs/build/html/_sources/generator.rst.txt
+-rw-r--r--   0 tarlisportela   (501) staff       (20)      623 2024-05-17 22:49:52.000000 mat_data-0.1rc1/docs/build/html/_sources/index.rst.txt
+-rw-r--r--   0 tarlisportela   (501) staff       (20)       77 2024-05-17 21:29:23.000000 mat_data-0.1rc1/docs/build/html/_sources/preprocess.rst.txt
+drwxr-xr-x   0 tarlisportela   (501) staff       (20)        0 2024-05-17 22:54:36.370971 mat_data-0.1rc1/docs/build/html/_static/
+-rw-r--r--   0 tarlisportela   (501) staff       (20)    11143 2024-05-17 22:49:56.000000 mat_data-0.1rc1/docs/build/html/_static/alabaster.css
+-rw-r--r--   0 tarlisportela   (501) staff       (20)    15096 2024-05-17 22:49:56.000000 mat_data-0.1rc1/docs/build/html/_static/basic.css
+-rw-r--r--   0 tarlisportela   (501) staff       (20)       42 2024-05-17 19:58:27.000000 mat_data-0.1rc1/docs/build/html/_static/custom.css
+-rw-r--r--   0 tarlisportela   (501) staff       (20)     4472 2024-05-17 19:58:27.000000 mat_data-0.1rc1/docs/build/html/_static/doctools.js
+-rw-r--r--   0 tarlisportela   (501) staff       (20)      329 2024-05-17 22:49:56.000000 mat_data-0.1rc1/docs/build/html/_static/documentation_options.js
+-rw-r--r--   0 tarlisportela   (501) staff       (20)      286 2024-05-17 19:58:27.000000 mat_data-0.1rc1/docs/build/html/_static/file.png
+-rw-r--r--   0 tarlisportela   (501) staff       (20)     4758 2024-05-17 22:49:56.000000 mat_data-0.1rc1/docs/build/html/_static/language_data.js
+-rw-r--r--   0 tarlisportela   (501) staff       (20)       90 2024-05-17 19:58:27.000000 mat_data-0.1rc1/docs/build/html/_static/minus.png
+-rw-r--r--   0 tarlisportela   (501) staff       (20)       90 2024-05-17 19:58:27.000000 mat_data-0.1rc1/docs/build/html/_static/plus.png
+-rw-r--r--   0 tarlisportela   (501) staff       (20)     5299 2024-05-17 22:49:56.000000 mat_data-0.1rc1/docs/build/html/_static/pygments.css
+-rw-r--r--   0 tarlisportela   (501) staff       (20)    20731 2024-05-17 19:58:27.000000 mat_data-0.1rc1/docs/build/html/_static/searchtools.js
+-rw-r--r--   0 tarlisportela   (501) staff       (20)     5123 2024-05-17 19:58:27.000000 mat_data-0.1rc1/docs/build/html/_static/sphinx_highlight.js
+-rw-r--r--   0 tarlisportela   (501) staff       (20)    42430 2024-05-17 22:44:00.000000 mat_data-0.1rc1/docs/build/html/converter.html
+-rw-r--r--   0 tarlisportela   (501) staff       (20)    32404 2024-05-17 22:44:01.000000 mat_data-0.1rc1/docs/build/html/dataset.html
+-rw-r--r--   0 tarlisportela   (501) staff       (20)    25016 2024-05-17 22:44:01.000000 mat_data-0.1rc1/docs/build/html/generator.html
+-rw-r--r--   0 tarlisportela   (501) staff       (20)    16351 2024-05-17 22:49:56.000000 mat_data-0.1rc1/docs/build/html/genindex.html
+-rw-r--r--   0 tarlisportela   (501) staff       (20)    20647 2024-05-17 22:49:56.000000 mat_data-0.1rc1/docs/build/html/index.html
+-rw-r--r--   0 tarlisportela   (501) staff       (20)      740 2024-05-17 22:49:56.000000 mat_data-0.1rc1/docs/build/html/objects.inv
+-rw-r--r--   0 tarlisportela   (501) staff       (20)    49486 2024-05-17 22:44:01.000000 mat_data-0.1rc1/docs/build/html/preprocess.html
+-rw-r--r--   0 tarlisportela   (501) staff       (20)     4166 2024-05-17 22:49:56.000000 mat_data-0.1rc1/docs/build/html/py-modindex.html
+-rw-r--r--   0 tarlisportela   (501) staff       (20)     3092 2024-05-17 22:49:56.000000 mat_data-0.1rc1/docs/build/html/search.html
+-rw-r--r--   0 tarlisportela   (501) staff       (20)    17329 2024-05-17 22:49:56.000000 mat_data-0.1rc1/docs/build/html/searchindex.js
+-rw-r--r--   0 tarlisportela   (501) staff       (20)      804 2024-05-17 20:33:21.000000 mat_data-0.1rc1/docs/make.bat
+drwxr-xr-x   0 tarlisportela   (501) staff       (20)        0 2024-05-17 22:54:36.371736 mat_data-0.1rc1/docs/source/
+-rw-r--r--   0 tarlisportela   (501) staff       (20)     1262 2024-05-17 22:43:49.000000 mat_data-0.1rc1/docs/source/conf.py
+-rw-r--r--   0 tarlisportela   (501) staff       (20)       66 2024-05-17 21:13:53.000000 mat_data-0.1rc1/docs/source/converter.rst
+-rw-r--r--   0 tarlisportela   (501) staff       (20)       60 2024-05-17 21:13:51.000000 mat_data-0.1rc1/docs/source/dataset.rst
+-rw-r--r--   0 tarlisportela   (501) staff       (20)       66 2024-05-17 21:29:32.000000 mat_data-0.1rc1/docs/source/generator.rst
+-rw-r--r--   0 tarlisportela   (501) staff       (20)      623 2024-05-17 22:49:52.000000 mat_data-0.1rc1/docs/source/index.rst
+-rw-r--r--   0 tarlisportela   (501) staff       (20)       77 2024-05-17 21:29:23.000000 mat_data-0.1rc1/docs/source/preprocess.rst
+drwxr-xr-x   0 tarlisportela   (501) staff       (20)        0 2024-05-17 22:54:36.393864 mat_data-0.1rc1/mat_data.egg-info/
+-rw-r--r--   0 tarlisportela   (501) staff       (20)     5678 2024-05-17 22:54:36.000000 mat_data-0.1rc1/mat_data.egg-info/PKG-INFO
+-rw-r--r--   0 tarlisportela   (501) staff       (20)     2573 2024-05-17 22:54:36.000000 mat_data-0.1rc1/mat_data.egg-info/SOURCES.txt
+-rw-r--r--   0 tarlisportela   (501) staff       (20)        1 2024-05-17 22:54:36.000000 mat_data-0.1rc1/mat_data.egg-info/dependency_links.txt
+-rw-r--r--   0 tarlisportela   (501) staff       (20)      169 2024-05-17 22:54:36.000000 mat_data-0.1rc1/mat_data.egg-info/requires.txt
+-rw-r--r--   0 tarlisportela   (501) staff       (20)        8 2024-05-17 22:54:36.000000 mat_data-0.1rc1/mat_data.egg-info/top_level.txt
+drwxr-xr-x   0 tarlisportela   (501) staff       (20)        0 2024-05-17 22:54:36.373661 mat_data-0.1rc1/matdata/
+-rw-r--r--   0 tarlisportela   (501) staff       (20)    35129 2023-12-15 20:34:29.000000 mat_data-0.1rc1/matdata/LICENSE
+-rw-r--r--   0 tarlisportela   (501) staff       (20)     3304 2024-04-17 14:32:21.000000 mat_data-0.1rc1/matdata/README.md
+-rw-r--r--   0 tarlisportela   (501) staff       (20)      770 2024-05-17 21:07:30.000000 mat_data-0.1rc1/matdata/__init__.py
+drwxr-xr-x   0 tarlisportela   (501) staff       (20)        0 2024-05-17 22:54:36.355663 mat_data-0.1rc1/matdata/assets/
+drwxr-xr-x   0 tarlisportela   (501) staff       (20)        0 2024-05-17 22:54:36.392655 mat_data-0.1rc1/matdata/assets/sample/
+-rw-rw-r--   0 tarlisportela   (501) staff       (20)  7716732 2021-02-10 16:01:46.000000 mat_data-0.1rc1/matdata/assets/sample/Foursquare_Sample.csv
+-rw-r--r--   0 tarlisportela   (501) staff       (20)  1775017 2024-05-17 19:06:55.000000 mat_data-0.1rc1/matdata/assets/sample/data.parquet
+-rw-r--r--   0 tarlisportela   (501) staff       (20)  7619562 2024-05-17 19:06:54.000000 mat_data-0.1rc1/matdata/assets/sample/joined.csv
+-rw-r--r--   0 tarlisportela   (501) staff       (20)  2283111 2024-05-17 19:06:46.000000 mat_data-0.1rc1/matdata/assets/sample/test.csv
+-rw-r--r--   0 tarlisportela   (501) staff       (20)   494642 2024-05-17 19:06:46.000000 mat_data-0.1rc1/matdata/assets/sample/test.parquet
+-rw-r--r--   0 tarlisportela   (501) staff       (20)  5336514 2024-05-17 19:06:45.000000 mat_data-0.1rc1/matdata/assets/sample/train.csv
+-rw-r--r--   0 tarlisportela   (501) staff       (20)  1075420 2024-05-17 19:06:46.000000 mat_data-0.1rc1/matdata/assets/sample/train.parquet
+-rw-r--r--   0 tarlisportela   (501) staff       (20)    23157 2024-05-17 21:32:51.000000 mat_data-0.1rc1/matdata/converter.py
+-rw-r--r--   0 tarlisportela   (501) staff       (20)    19407 2024-05-17 22:28:15.000000 mat_data-0.1rc1/matdata/dataset.py
+-rw-r--r--   0 tarlisportela   (501) staff       (20)    26560 2024-05-17 22:09:55.000000 mat_data-0.1rc1/matdata/generator.py
+drwxr-xr-x   0 tarlisportela   (501) staff       (20)        0 2024-05-17 22:54:36.393403 mat_data-0.1rc1/matdata/inc/
+-rw-r--r--   0 tarlisportela   (501) staff       (20)        0 2023-12-15 20:26:21.000000 mat_data-0.1rc1/matdata/inc/__init__.py
+-rw-r--r--   0 tarlisportela   (501) staff       (20)    54373 2024-05-17 21:34:31.000000 mat_data-0.1rc1/matdata/inc/ts_io.py
+-rw-r--r--   0 tarlisportela   (501) staff       (20)    43122 2024-05-17 22:02:14.000000 mat_data-0.1rc1/matdata/preprocess.py
+drwxr-xr-x   0 tarlisportela   (501) staff       (20)        0 2024-05-17 22:54:36.393665 mat_data-0.1rc1/matdata/util/
+-rw-r--r--   0 tarlisportela   (501) staff       (20)        0 2023-12-15 20:26:21.000000 mat_data-0.1rc1/matdata/util/__init__.py
+-rw-r--r--   0 tarlisportela   (501) staff       (20)     1384 2024-05-17 21:33:27.000000 mat_data-0.1rc1/matdata/util/movelets.py
+-rw-r--r--   0 tarlisportela   (501) staff       (20)     2179 2024-05-17 21:35:05.000000 mat_data-0.1rc1/pyproject.toml
+-rw-r--r--   0 tarlisportela   (501) staff       (20)       38 2024-05-17 22:54:36.395012 mat_data-0.1rc1/setup.cfg
+-rw-r--r--   0 tarlisportela   (501) staff       (20)     2098 2024-04-16 13:01:09.000000 mat_data-0.1rc1/setup.py
```

### Comparing `mat-data-0.1b9/LICENSE` & `mat_data-0.1rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `mat-data-0.1b9/MAT-data-Tutorial.html` & `mat_data-0.1rc1/MAT-data-Tutorial.html`

 * *Files 16% similar despite different names*

```diff
@@ -35927,1477 +35927,8569 @@
 0008c560: 733d 226a 702d 5265 6e64 6572 6564 4854  s="jp-RenderedHT
 0008c570: 4d4c 436f 6d6d 6f6e 206a 702d 5265 6e64  MLCommon jp-Rend
 0008c580: 6572 6564 4d61 726b 646f 776e 206a 702d  eredMarkdown jp-
 0008c590: 4d61 726b 646f 776e 4f75 7470 7574 2022  MarkdownOutput "
 0008c5a0: 2064 6174 612d 6d69 6d65 2d74 7970 653d   data-mime-type=
 0008c5b0: 2274 6578 742f 6d61 726b 646f 776e 223e  "text/markdown">
 0008c5c0: 0a3c 6831 2069 643d 224d 4154 2d64 6174  .<h1 id="MAT-dat
-0008c5d0: 613a 2d44 6174 612d 5072 6570 726f 6365  a:-Data-Preproce
-0008c5e0: 7373 696e 672d 666f 722d 4d75 6c74 6970  ssing-for-Multip
-0008c5f0: 6c65 2d41 7370 6563 742d 5472 616a 6563  le-Aspect-Trajec
-0008c600: 746f 7279 2d44 6174 612d 4d69 6e69 6e67  tory-Data-Mining
-0008c610: 2d25 3542 4d41 542d 546f 6f6c 732d 4672  -%5BMAT-Tools-Fr
-0008c620: 616d 6577 6f72 6b25 3544 223e 4d41 542d  amework%5D">MAT-
-0008c630: 6461 7461 3a20 4461 7461 2050 7265 7072  data: Data Prepr
-0008c640: 6f63 6573 7369 6e67 2066 6f72 204d 756c  ocessing for Mul
-0008c650: 7469 706c 6520 4173 7065 6374 2054 7261  tiple Aspect Tra
-0008c660: 6a65 6374 6f72 7920 4461 7461 204d 696e  jectory Data Min
-0008c670: 696e 6720 5b4d 4154 2d54 6f6f 6c73 2046  ing [MAT-Tools F
-0008c680: 7261 6d65 776f 726b 5d3c 6120 636c 6173  ramework]<a clas
-0008c690: 733d 2261 6e63 686f 722d 6c69 6e6b 2220  s="anchor-link" 
-0008c6a0: 6872 6566 3d22 234d 4154 2d64 6174 613a  href="#MAT-data:
-0008c6b0: 2d44 6174 612d 5072 6570 726f 6365 7373  -Data-Preprocess
-0008c6c0: 696e 672d 666f 722d 4d75 6c74 6970 6c65  ing-for-Multiple
-0008c6d0: 2d41 7370 6563 742d 5472 616a 6563 746f  -Aspect-Trajecto
-0008c6e0: 7279 2d44 6174 612d 4d69 6e69 6e67 2d25  ry-Data-Mining-%
-0008c6f0: 3542 4d41 542d 546f 6f6c 732d 4672 616d  5BMAT-Tools-Fram
-0008c700: 6577 6f72 6b25 3544 223e 2623 3138 323b  ework%5D">&#182;
-0008c710: 3c2f 613e 3c2f 6831 3e3c 703e 5361 6d70  </a></h1><p>Samp
-0008c720: 6c65 2043 6f64 6520 696e 2070 7974 686f  le Code in pytho
-0008c730: 6e20 6e6f 7465 626f 6f6b 2074 6f20 7573  n notebook to us
-0008c740: 6520 6d61 742d 6461 7461 2061 7320 6120  e mat-data as a 
-0008c750: 7079 7468 6f6e 206c 6962 7261 7279 2e3c  python library.<
-0008c760: 2f70 3e0a 3c70 3e54 6865 2070 7265 7365  /p>.<p>The prese
-0008c770: 6e74 2070 6163 6b61 6765 206f 6666 6572  nt package offer
-0008c780: 7320 6120 746f 6f6c 2c20 746f 2073 7570  s a tool, to sup
-0008c790: 706f 7274 2074 6865 2075 7365 7220 696e  port the user in
-0008c7a0: 2074 6865 2074 6173 6b20 6f66 2064 6174   the task of dat
-0008c7b0: 6120 7072 6570 726f 6365 7373 696e 6720  a preprocessing 
-0008c7c0: 6f66 206d 756c 7469 706c 6520 6173 7065  of multiple aspe
-0008c7d0: 6374 2074 7261 6a65 6374 6f72 6965 732c  ct trajectories,
-0008c7e0: 206f 7220 746f 2067 656e 6572 6174 696e   or to generatin
-0008c7f0: 6720 7379 6e74 6865 7469 6320 6461 7461  g synthetic data
-0008c800: 7365 7473 2e20 4974 2069 6e74 6567 7261  sets. It integra
-0008c810: 7465 7320 696e 746f 2061 2075 6e69 7175  tes into a uniqu
-0008c820: 6520 6672 616d 6577 6f72 6b20 666f 7220  e framework for 
-0008c830: 6d75 6c74 6970 6c65 2061 7370 6563 7473  multiple aspects
-0008c840: 2074 7261 6a65 6374 6f72 6965 7320 616e   trajectories an
-0008c850: 6420 696e 2067 656e 6572 616c 2066 6f72  d in general for
-0008c860: 206d 756c 7469 6469 6d65 6e73 696f 6e61   multidimensiona
-0008c870: 6c20 7365 7175 656e 6365 2064 6174 6120  l sequence data 
-0008c880: 6d69 6e69 6e67 206d 6574 686f 6473 2e3c  mining methods.<
-0008c890: 2f70 3e0a 3c70 3e43 7265 6174 6564 206f  /p>.<p>Created o
-0008c8a0: 6e20 4465 632c 2032 3032 330a 436f 7079  n Dec, 2023.Copy
-0008c8b0: 7269 6768 7420 2843 2920 3230 3233 2c20  right (C) 2023, 
-0008c8c0: 4c69 6365 6e73 6520 4750 4c20 5665 7273  License GPL Vers
-0008c8d0: 696f 6e20 3320 6f72 2073 7570 6572 696f  ion 3 or superio
-0008c8e0: 7220 2873 6565 204c 4943 454e 5345 2066  r (see LICENSE f
-0008c8f0: 696c 6529 3c2f 703e 0a0a 3c2f 6469 763e  ile)</p>..</div>
-0008c900: 0a3c 2f64 6976 3e0a 3c2f 6469 763e 0a3c  .</div>.</div>.<
-0008c910: 2f64 6976 3e3c 6469 7620 636c 6173 733d  /div><div class=
-0008c920: 226a 702d 4365 6c6c 206a 702d 436f 6465  "jp-Cell jp-Code
-0008c930: 4365 6c6c 206a 702d 4e6f 7465 626f 6f6b  Cell jp-Notebook
-0008c940: 2d63 656c 6c20 6a70 2d6d 6f64 2d6e 6f4f  -cell jp-mod-noO
-0008c950: 7574 7075 7473 2020 223e 0a3c 6469 7620  utputs  ">.<div 
-0008c960: 636c 6173 733d 226a 702d 4365 6c6c 2d69  class="jp-Cell-i
-0008c970: 6e70 7574 5772 6170 7065 7222 3e0a 3c64  nputWrapper">.<d
-0008c980: 6976 2063 6c61 7373 3d22 6a70 2d43 6f6c  iv class="jp-Col
-0008c990: 6c61 7073 6572 206a 702d 496e 7075 7443  lapser jp-InputC
-0008c9a0: 6f6c 6c61 7073 6572 206a 702d 4365 6c6c  ollapser jp-Cell
-0008c9b0: 2d69 6e70 7574 436f 6c6c 6170 7365 7222  -inputCollapser"
-0008c9c0: 3e0a 3c2f 6469 763e 0a3c 6469 7620 636c  >.</div>.<div cl
-0008c9d0: 6173 733d 226a 702d 496e 7075 7441 7265  ass="jp-InputAre
-0008c9e0: 6120 6a70 2d43 656c 6c2d 696e 7075 7441  a jp-Cell-inputA
-0008c9f0: 7265 6122 3e0a 3c64 6976 2063 6c61 7373  rea">.<div class
-0008ca00: 3d22 6a70 2d49 6e70 7574 5072 6f6d 7074  ="jp-InputPrompt
-0008ca10: 206a 702d 496e 7075 7441 7265 612d 7072   jp-InputArea-pr
-0008ca20: 6f6d 7074 223e 496e 266e 6273 703b 5b31  ompt">In&nbsp;[1
-0008ca30: 5d3a 3c2f 6469 763e 0a3c 6469 7620 636c  ]:</div>.<div cl
-0008ca40: 6173 733d 226a 702d 436f 6465 4d69 7272  ass="jp-CodeMirr
-0008ca50: 6f72 4564 6974 6f72 206a 702d 4564 6974  orEditor jp-Edit
-0008ca60: 6f72 206a 702d 496e 7075 7441 7265 612d  or jp-InputArea-
-0008ca70: 6564 6974 6f72 2220 6461 7461 2d74 7970  editor" data-typ
-0008ca80: 653d 2269 6e6c 696e 6522 3e0a 2020 2020  e="inline">.    
-0008ca90: 203c 6469 7620 636c 6173 733d 2243 6f64   <div class="Cod
-0008caa0: 654d 6972 726f 7220 636d 2d73 2d6a 7570  eMirror cm-s-jup
-0008cab0: 7974 6572 223e 0a3c 6469 7620 636c 6173  yter">.<div clas
-0008cac0: 733d 2220 6869 6768 6c69 6768 7420 686c  s=" highlight hl
-0008cad0: 2d69 7079 7468 6f6e 3322 3e3c 7072 653e  -ipython3"><pre>
-0008cae0: 3c73 7061 6e3e 3c2f 7370 616e 3e3c 7370  <span></span><sp
-0008caf0: 616e 2063 6c61 7373 3d22 6b6e 223e 696d  an class="kn">im
-0008cb00: 706f 7274 3c2f 7370 616e 3e20 3c73 7061  port</span> <spa
-0008cb10: 6e20 636c 6173 733d 226e 6e22 3e73 7973  n class="nn">sys
-0008cb20: 3c2f 7370 616e 3e3c 7370 616e 2063 6c61  </span><span cla
-0008cb30: 7373 3d22 6f22 3e2c 3c2f 7370 616e 3e20  ss="o">,</span> 
-0008cb40: 3c73 7061 6e20 636c 6173 733d 226e 6e22  <span class="nn"
-0008cb50: 3e6f 733c 2f73 7061 6e3e 0a0a 3c73 7061  >os</span>..<spa
-0008cb60: 6e20 636c 6173 733d 226e 223e 726f 6f74  n class="n">root
-0008cb70: 3c2f 7370 616e 3e20 2020 2020 203c 7370  </span>      <sp
-0008cb80: 616e 2063 6c61 7373 3d22 6f22 3e3d 3c2f  an class="o">=</
-0008cb90: 7370 616e 3e20 3c73 7061 6e20 636c 6173  span> <span clas
-0008cba0: 733d 226e 223e 6f73 3c2f 7370 616e 3e3c  s="n">os</span><
-0008cbb0: 7370 616e 2063 6c61 7373 3d22 6f22 3e2e  span class="o">.
-0008cbc0: 3c2f 7370 616e 3e3c 7370 616e 2063 6c61  </span><span cla
-0008cbd0: 7373 3d22 6e22 3e70 6174 683c 2f73 7061  ss="n">path</spa
-0008cbe0: 6e3e 3c73 7061 6e20 636c 6173 733d 226f  n><span class="o
-0008cbf0: 223e 2e3c 2f73 7061 6e3e 3c73 7061 6e20  ">.</span><span 
-0008cc00: 636c 6173 733d 226e 223e 6a6f 696e 3c2f  class="n">join</
-0008cc10: 7370 616e 3e3c 7370 616e 2063 6c61 7373  span><span class
-0008cc20: 3d22 7022 3e28 3c2f 7370 616e 3e3c 7370  ="p">(</span><sp
-0008cc30: 616e 2063 6c61 7373 3d22 7331 223e 2623  an class="s1">&#
-0008cc40: 3339 3b61 7574 6f6d 6174 697a 6526 2333  39;automatize&#3
-0008cc50: 393b 3c2f 7370 616e 3e3c 7370 616e 2063  9;</span><span c
-0008cc60: 6c61 7373 3d22 7022 3e2c 3c2f 7370 616e  lass="p">,</span
-0008cc70: 3e20 3c73 7061 6e20 636c 6173 733d 2273  > <span class="s
-0008cc80: 3122 3e26 2333 393b 6173 7365 7473 2623  1">&#39;assets&#
-0008cc90: 3339 3b3c 2f73 7061 6e3e 3c73 7061 6e20  39;</span><span 
-0008cca0: 636c 6173 733d 2270 223e 2c3c 2f73 7061  class="p">,</spa
-0008ccb0: 6e3e 203c 7370 616e 2063 6c61 7373 3d22  n> <span class="
-0008ccc0: 7331 223e 2623 3339 3b65 7861 6d70 6c65  s1">&#39;example
-0008ccd0: 7326 2333 393b 3c2f 7370 616e 3e3c 7370  s&#39;</span><sp
-0008cce0: 616e 2063 6c61 7373 3d22 7022 3e2c 3c2f  an class="p">,</
-0008ccf0: 7370 616e 3e20 3c73 7061 6e20 636c 6173  span> <span clas
-0008cd00: 733d 2273 3122 3e26 2333 393b 4578 616d  s="s1">&#39;Exam
-0008cd10: 706c 6526 2333 393b 3c2f 7370 616e 3e3c  ple&#39;</span><
-0008cd20: 7370 616e 2063 6c61 7373 3d22 7022 3e29  span class="p">)
-0008cd30: 3c2f 7370 616e 3e0a 0a3c 7370 616e 2063  </span>..<span c
-0008cd40: 6c61 7373 3d22 6331 223e 2320 5765 2063  lass="c1"># We c
-0008cd50: 6f6e 7369 6465 7220 7468 6973 2066 6f6c  onsider this fol
-0008cd60: 6465 7220 6f72 6761 6e69 7a61 7469 6f6e  der organization
-0008cd70: 2074 6f20 7468 6520 6578 7065 7269 6d65   to the experime
-0008cd80: 6e74 616c 2065 6e76 6972 6f6d 6e65 6e74  ntal enviromnent
-0008cd90: 3a3c 2f73 7061 6e3e 0a3c 7370 616e 2063  :</span>.<span c
-0008cda0: 6c61 7373 3d22 6e22 3e70 7267 5f70 6174  lass="n">prg_pat
-0008cdb0: 683c 2f73 7061 6e3e 2020 3c73 7061 6e20  h</span>  <span 
-0008cdc0: 636c 6173 733d 226f 223e 3d3c 2f73 7061  class="o">=</spa
-0008cdd0: 6e3e 203c 7370 616e 2063 6c61 7373 3d22  n> <span class="
-0008cde0: 6e22 3e6f 733c 2f73 7061 6e3e 3c73 7061  n">os</span><spa
-0008cdf0: 6e20 636c 6173 733d 226f 223e 2e3c 2f73  n class="o">.</s
-0008ce00: 7061 6e3e 3c73 7061 6e20 636c 6173 733d  pan><span class=
-0008ce10: 226e 223e 7061 7468 3c2f 7370 616e 3e3c  "n">path</span><
-0008ce20: 7370 616e 2063 6c61 7373 3d22 6f22 3e2e  span class="o">.
-0008ce30: 3c2f 7370 616e 3e3c 7370 616e 2063 6c61  </span><span cla
-0008ce40: 7373 3d22 6e22 3e6a 6f69 6e3c 2f73 7061  ss="n">join</spa
-0008ce50: 6e3e 3c73 7061 6e20 636c 6173 733d 2270  n><span class="p
-0008ce60: 223e 283c 2f73 7061 6e3e 3c73 7061 6e20  ">(</span><span 
-0008ce70: 636c 6173 733d 226e 223e 726f 6f74 3c2f  class="n">root</
-0008ce80: 7370 616e 3e3c 7370 616e 2063 6c61 7373  span><span class
-0008ce90: 3d22 7022 3e2c 3c2f 7370 616e 3e20 3c73  ="p">,</span> <s
-0008cea0: 7061 6e20 636c 6173 733d 2273 3122 3e26  pan class="s1">&
-0008ceb0: 2333 393b 7072 6f67 7261 6d73 2623 3339  #39;programs&#39
-0008cec0: 3b3c 2f73 7061 6e3e 3c73 7061 6e20 636c  ;</span><span cl
-0008ced0: 6173 733d 2270 223e 293c 2f73 7061 6e3e  ass="p">)</span>
-0008cee0: 0a3c 7370 616e 2063 6c61 7373 3d22 6e22  .<span class="n"
-0008cef0: 3e64 6174 615f 7061 7468 3c2f 7370 616e  >data_path</span
-0008cf00: 3e20 3c73 7061 6e20 636c 6173 733d 226f  > <span class="o
-0008cf10: 223e 3d3c 2f73 7061 6e3e 203c 7370 616e  ">=</span> <span
-0008cf20: 2063 6c61 7373 3d22 6e22 3e6f 733c 2f73   class="n">os</s
-0008cf30: 7061 6e3e 3c73 7061 6e20 636c 6173 733d  pan><span class=
-0008cf40: 226f 223e 2e3c 2f73 7061 6e3e 3c73 7061  "o">.</span><spa
-0008cf50: 6e20 636c 6173 733d 226e 223e 7061 7468  n class="n">path
-0008cf60: 3c2f 7370 616e 3e3c 7370 616e 2063 6c61  </span><span cla
-0008cf70: 7373 3d22 6f22 3e2e 3c2f 7370 616e 3e3c  ss="o">.</span><
-0008cf80: 7370 616e 2063 6c61 7373 3d22 6e22 3e6a  span class="n">j
-0008cf90: 6f69 6e3c 2f73 7061 6e3e 3c73 7061 6e20  oin</span><span 
-0008cfa0: 636c 6173 733d 2270 223e 283c 2f73 7061  class="p">(</spa
-0008cfb0: 6e3e 3c73 7061 6e20 636c 6173 733d 226e  n><span class="n
-0008cfc0: 223e 726f 6f74 3c2f 7370 616e 3e3c 7370  ">root</span><sp
-0008cfd0: 616e 2063 6c61 7373 3d22 7022 3e2c 3c2f  an class="p">,</
-0008cfe0: 7370 616e 3e20 3c73 7061 6e20 636c 6173  span> <span clas
-0008cff0: 733d 2273 3122 3e26 2333 393b 6461 7461  s="s1">&#39;data
-0008d000: 2623 3339 3b3c 2f73 7061 6e3e 3c73 7061  &#39;</span><spa
-0008d010: 6e20 636c 6173 733d 2270 223e 293c 2f73  n class="p">)</s
-0008d020: 7061 6e3e 0a3c 7370 616e 2063 6c61 7373  pan>.<span class
-0008d030: 3d22 6e22 3e72 6573 5f70 6174 683c 2f73  ="n">res_path</s
-0008d040: 7061 6e3e 2020 3c73 7061 6e20 636c 6173  pan>  <span clas
-0008d050: 733d 226f 223e 3d3c 2f73 7061 6e3e 203c  s="o">=</span> <
-0008d060: 7370 616e 2063 6c61 7373 3d22 6e22 3e6f  span class="n">o
-0008d070: 733c 2f73 7061 6e3e 3c73 7061 6e20 636c  s</span><span cl
-0008d080: 6173 733d 226f 223e 2e3c 2f73 7061 6e3e  ass="o">.</span>
-0008d090: 3c73 7061 6e20 636c 6173 733d 226e 223e  <span class="n">
-0008d0a0: 7061 7468 3c2f 7370 616e 3e3c 7370 616e  path</span><span
-0008d0b0: 2063 6c61 7373 3d22 6f22 3e2e 3c2f 7370   class="o">.</sp
-0008d0c0: 616e 3e3c 7370 616e 2063 6c61 7373 3d22  an><span class="
-0008d0d0: 6e22 3e6a 6f69 6e3c 2f73 7061 6e3e 3c73  n">join</span><s
-0008d0e0: 7061 6e20 636c 6173 733d 2270 223e 283c  pan class="p">(<
-0008d0f0: 2f73 7061 6e3e 3c73 7061 6e20 636c 6173  /span><span clas
-0008d100: 733d 226e 223e 726f 6f74 3c2f 7370 616e  s="n">root</span
-0008d110: 3e3c 7370 616e 2063 6c61 7373 3d22 7022  ><span class="p"
-0008d120: 3e2c 3c2f 7370 616e 3e20 3c73 7061 6e20  >,</span> <span 
-0008d130: 636c 6173 733d 2273 3122 3e26 2333 393b  class="s1">&#39;
-0008d140: 7265 7375 6c74 7326 2333 393b 3c2f 7370  results&#39;</sp
-0008d150: 616e 3e3c 7370 616e 2063 6c61 7373 3d22  an><span class="
-0008d160: 7022 3e29 3c2f 7370 616e 3e0a 0a3c 7370  p">)</span>..<sp
-0008d170: 616e 2063 6c61 7373 3d22 6331 223e 2320  an class="c1"># 
-0008d180: 4f52 2c20 796f 7520 6361 6e20 7573 6520  OR, you can use 
-0008d190: 7468 6520 2e6a 6172 206d 6574 686f 6420  the .jar method 
-0008d1a0: 6669 6c65 7320 696e 3a3c 2f73 7061 6e3e  files in:</span>
-0008d1b0: 0a3c 7370 616e 2063 6c61 7373 3d22 6e22  .<span class="n"
-0008d1c0: 3e70 7267 5f70 6174 683c 2f73 7061 6e3e  >prg_path</span>
-0008d1d0: 2020 3c73 7061 6e20 636c 6173 733d 226f    <span class="o
-0008d1e0: 223e 3d3c 2f73 7061 6e3e 203c 7370 616e  ">=</span> <span
-0008d1f0: 2063 6c61 7373 3d22 6e22 3e6f 733c 2f73   class="n">os</s
-0008d200: 7061 6e3e 3c73 7061 6e20 636c 6173 733d  pan><span class=
-0008d210: 226f 223e 2e3c 2f73 7061 6e3e 3c73 7061  "o">.</span><spa
-0008d220: 6e20 636c 6173 733d 226e 223e 7061 7468  n class="n">path
-0008d230: 3c2f 7370 616e 3e3c 7370 616e 2063 6c61  </span><span cla
-0008d240: 7373 3d22 6f22 3e2e 3c2f 7370 616e 3e3c  ss="o">.</span><
-0008d250: 7370 616e 2063 6c61 7373 3d22 6e22 3e6a  span class="n">j
-0008d260: 6f69 6e3c 2f73 7061 6e3e 3c73 7061 6e20  oin</span><span 
-0008d270: 636c 6173 733d 2270 223e 283c 2f73 7061  class="p">(</spa
-0008d280: 6e3e 3c73 7061 6e20 636c 6173 733d 2273  n><span class="s
-0008d290: 3122 3e26 2333 393b 6175 746f 6d61 7469  1">&#39;automati
-0008d2a0: 7a65 2623 3339 3b3c 2f73 7061 6e3e 3c73  ze&#39;</span><s
-0008d2b0: 7061 6e20 636c 6173 733d 2270 223e 2c3c  pan class="p">,<
-0008d2c0: 2f73 7061 6e3e 203c 7370 616e 2063 6c61  /span> <span cla
-0008d2d0: 7373 3d22 7331 223e 2623 3339 3b61 7373  ss="s1">&#39;ass
-0008d2e0: 6574 7326 2333 393b 3c2f 7370 616e 3e3c  ets&#39;</span><
-0008d2f0: 7370 616e 2063 6c61 7373 3d22 7022 3e2c  span class="p">,
-0008d300: 3c2f 7370 616e 3e20 3c73 7061 6e20 636c  </span> <span cl
-0008d310: 6173 733d 2273 3122 3e26 2333 393b 6d65  ass="s1">&#39;me
-0008d320: 7468 6f64 2623 3339 3b3c 2f73 7061 6e3e  thod&#39;</span>
-0008d330: 3c73 7061 6e20 636c 6173 733d 2270 223e  <span class="p">
-0008d340: 293c 2f73 7061 6e3e 0a3c 2f70 7265 3e3c  )</span>.</pre><
-0008d350: 2f64 6976 3e0a 0a20 2020 2020 3c2f 6469  /div>..     </di
-0008d360: 763e 0a3c 2f64 6976 3e0a 3c2f 6469 763e  v>.</div>.</div>
-0008d370: 0a3c 2f64 6976 3e0a 0a3c 2f64 6976 3e0a  .</div>..</div>.
-0008d380: 3c64 6976 2063 6c61 7373 3d22 6a70 2d43  <div class="jp-C
-0008d390: 656c 6c20 6a70 2d4d 6172 6b64 6f77 6e43  ell jp-MarkdownC
-0008d3a0: 656c 6c20 6a70 2d4e 6f74 6562 6f6f 6b2d  ell jp-Notebook-
-0008d3b0: 6365 6c6c 223e 0a3c 6469 7620 636c 6173  cell">.<div clas
-0008d3c0: 733d 226a 702d 4365 6c6c 2d69 6e70 7574  s="jp-Cell-input
-0008d3d0: 5772 6170 7065 7222 3e0a 3c64 6976 2063  Wrapper">.<div c
-0008d3e0: 6c61 7373 3d22 6a70 2d43 6f6c 6c61 7073  lass="jp-Collaps
-0008d3f0: 6572 206a 702d 496e 7075 7443 6f6c 6c61  er jp-InputColla
-0008d400: 7073 6572 206a 702d 4365 6c6c 2d69 6e70  pser jp-Cell-inp
-0008d410: 7574 436f 6c6c 6170 7365 7222 3e0a 3c2f  utCollapser">.</
-0008d420: 6469 763e 0a3c 6469 7620 636c 6173 733d  div>.<div class=
-0008d430: 226a 702d 496e 7075 7441 7265 6120 6a70  "jp-InputArea jp
-0008d440: 2d43 656c 6c2d 696e 7075 7441 7265 6122  -Cell-inputArea"
-0008d450: 3e3c 6469 7620 636c 6173 733d 226a 702d  ><div class="jp-
-0008d460: 496e 7075 7450 726f 6d70 7420 6a70 2d49  InputPrompt jp-I
-0008d470: 6e70 7574 4172 6561 2d70 726f 6d70 7422  nputArea-prompt"
-0008d480: 3e0a 3c2f 6469 763e 3c64 6976 2063 6c61  >.</div><div cla
-0008d490: 7373 3d22 6a70 2d52 656e 6465 7265 6448  ss="jp-RenderedH
-0008d4a0: 544d 4c43 6f6d 6d6f 6e20 6a70 2d52 656e  TMLCommon jp-Ren
-0008d4b0: 6465 7265 644d 6172 6b64 6f77 6e20 6a70  deredMarkdown jp
-0008d4c0: 2d4d 6172 6b64 6f77 6e4f 7574 7075 7420  -MarkdownOutput 
-0008d4d0: 2220 6461 7461 2d6d 696d 652d 7479 7065  " data-mime-type
-0008d4e0: 3d22 7465 7874 2f6d 6172 6b64 6f77 6e22  ="text/markdown"
-0008d4f0: 3e0a 3c68 3320 6964 3d22 312e 2d50 7265  >.<h3 id="1.-Pre
-0008d500: 2d70 726f 6365 7373 696e 672d 6461 7461  -processing-data
-0008d510: 223e 312e 2050 7265 2d70 726f 6365 7373  ">1. Pre-process
-0008d520: 696e 6720 6461 7461 3c61 2063 6c61 7373  ing data<a class
-0008d530: 3d22 616e 6368 6f72 2d6c 696e 6b22 2068  ="anchor-link" h
-0008d540: 7265 663d 2223 312e 2d50 7265 2d70 726f  ref="#1.-Pre-pro
-0008d550: 6365 7373 696e 672d 6461 7461 223e 2623  cessing-data">&#
-0008d560: 3138 323b 3c2f 613e 3c2f 6833 3e3c 703e  182;</a></h3><p>
-0008d570: 546f 2075 7365 2068 656c 7065 7273 2066  To use helpers f
-0008d580: 6f72 2064 6174 6120 7072 652d 7072 6f63  or data pre-proc
-0008d590: 6573 7369 6e67 2c20 696d 706f 7274 2066  essing, import f
-0008d5a0: 726f 6d20 7061 636b 6167 6520 3c63 6f64  rom package <cod
-0008d5b0: 653e 6d61 7464 6174 612e 7072 6570 726f  e>matdata.prepro
-0008d5c0: 6365 7373 3c2f 636f 6465 3e3a 3c2f 703e  cess</code>:</p>
-0008d5d0: 0a0a 3c2f 6469 763e 0a3c 2f64 6976 3e0a  ..</div>.</div>.
-0008d5e0: 3c2f 6469 763e 0a3c 2f64 6976 3e3c 6469  </div>.</div><di
-0008d5f0: 7620 636c 6173 733d 226a 702d 4365 6c6c  v class="jp-Cell
-0008d600: 206a 702d 436f 6465 4365 6c6c 206a 702d   jp-CodeCell jp-
-0008d610: 4e6f 7465 626f 6f6b 2d63 656c 6c20 6a70  Notebook-cell jp
-0008d620: 2d6d 6f64 2d6e 6f4f 7574 7075 7473 2020  -mod-noOutputs  
-0008d630: 223e 0a3c 6469 7620 636c 6173 733d 226a  ">.<div class="j
-0008d640: 702d 4365 6c6c 2d69 6e70 7574 5772 6170  p-Cell-inputWrap
-0008d650: 7065 7222 3e0a 3c64 6976 2063 6c61 7373  per">.<div class
-0008d660: 3d22 6a70 2d43 6f6c 6c61 7073 6572 206a  ="jp-Collapser j
-0008d670: 702d 496e 7075 7443 6f6c 6c61 7073 6572  p-InputCollapser
-0008d680: 206a 702d 4365 6c6c 2d69 6e70 7574 436f   jp-Cell-inputCo
-0008d690: 6c6c 6170 7365 7222 3e0a 3c2f 6469 763e  llapser">.</div>
-0008d6a0: 0a3c 6469 7620 636c 6173 733d 226a 702d  .<div class="jp-
-0008d6b0: 496e 7075 7441 7265 6120 6a70 2d43 656c  InputArea jp-Cel
-0008d6c0: 6c2d 696e 7075 7441 7265 6122 3e0a 3c64  l-inputArea">.<d
-0008d6d0: 6976 2063 6c61 7373 3d22 6a70 2d49 6e70  iv class="jp-Inp
-0008d6e0: 7574 5072 6f6d 7074 206a 702d 496e 7075  utPrompt jp-Inpu
-0008d6f0: 7441 7265 612d 7072 6f6d 7074 223e 496e  tArea-prompt">In
-0008d700: 266e 6273 703b 5b33 5d3a 3c2f 6469 763e  &nbsp;[3]:</div>
-0008d710: 0a3c 6469 7620 636c 6173 733d 226a 702d  .<div class="jp-
-0008d720: 436f 6465 4d69 7272 6f72 4564 6974 6f72  CodeMirrorEditor
-0008d730: 206a 702d 4564 6974 6f72 206a 702d 496e   jp-Editor jp-In
-0008d740: 7075 7441 7265 612d 6564 6974 6f72 2220  putArea-editor" 
-0008d750: 6461 7461 2d74 7970 653d 2269 6e6c 696e  data-type="inlin
-0008d760: 6522 3e0a 2020 2020 203c 6469 7620 636c  e">.     <div cl
-0008d770: 6173 733d 2243 6f64 654d 6972 726f 7220  ass="CodeMirror 
-0008d780: 636d 2d73 2d6a 7570 7974 6572 223e 0a3c  cm-s-jupyter">.<
-0008d790: 6469 7620 636c 6173 733d 2220 6869 6768  div class=" high
-0008d7a0: 6c69 6768 7420 686c 2d69 7079 7468 6f6e  light hl-ipython
-0008d7b0: 3322 3e3c 7072 653e 3c73 7061 6e3e 3c2f  3"><pre><span></
-0008d7c0: 7370 616e 3e3c 7370 616e 2063 6c61 7373  span><span class
-0008d7d0: 3d22 6b6e 223e 6672 6f6d 3c2f 7370 616e  ="kn">from</span
-0008d7e0: 3e20 3c73 7061 6e20 636c 6173 733d 226e  > <span class="n
-0008d7f0: 6e22 3e6d 6174 6461 7461 2e70 7265 7072  n">matdata.prepr
-0008d800: 6f63 6573 733c 2f73 7061 6e3e 203c 7370  ocess</span> <sp
-0008d810: 616e 2063 6c61 7373 3d22 6b6e 223e 696d  an class="kn">im
-0008d820: 706f 7274 3c2f 7370 616e 3e20 3c73 7061  port</span> <spa
-0008d830: 6e20 636c 6173 733d 226f 223e 2a3c 2f73  n class="o">*</s
-0008d840: 7061 6e3e 0a3c 2f70 7265 3e3c 2f64 6976  pan>.</pre></div
-0008d850: 3e0a 0a20 2020 2020 3c2f 6469 763e 0a3c  >..     </div>.<
-0008d860: 2f64 6976 3e0a 3c2f 6469 763e 0a3c 2f64  /div>.</div>.</d
-0008d870: 6976 3e0a 0a3c 2f64 6976 3e0a 3c64 6976  iv>..</div>.<div
-0008d880: 2063 6c61 7373 3d22 6a70 2d43 656c 6c20   class="jp-Cell 
-0008d890: 6a70 2d4d 6172 6b64 6f77 6e43 656c 6c20  jp-MarkdownCell 
-0008d8a0: 6a70 2d4e 6f74 6562 6f6f 6b2d 6365 6c6c  jp-Notebook-cell
-0008d8b0: 223e 0a3c 6469 7620 636c 6173 733d 226a  ">.<div class="j
-0008d8c0: 702d 4365 6c6c 2d69 6e70 7574 5772 6170  p-Cell-inputWrap
-0008d8d0: 7065 7222 3e0a 3c64 6976 2063 6c61 7373  per">.<div class
-0008d8e0: 3d22 6a70 2d43 6f6c 6c61 7073 6572 206a  ="jp-Collapser j
-0008d8f0: 702d 496e 7075 7443 6f6c 6c61 7073 6572  p-InputCollapser
-0008d900: 206a 702d 4365 6c6c 2d69 6e70 7574 436f   jp-Cell-inputCo
-0008d910: 6c6c 6170 7365 7222 3e0a 3c2f 6469 763e  llapser">.</div>
-0008d920: 0a3c 6469 7620 636c 6173 733d 226a 702d  .<div class="jp-
-0008d930: 496e 7075 7441 7265 6120 6a70 2d43 656c  InputArea jp-Cel
-0008d940: 6c2d 696e 7075 7441 7265 6122 3e3c 6469  l-inputArea"><di
-0008d950: 7620 636c 6173 733d 226a 702d 496e 7075  v class="jp-Inpu
-0008d960: 7450 726f 6d70 7420 6a70 2d49 6e70 7574  tPrompt jp-Input
-0008d970: 4172 6561 2d70 726f 6d70 7422 3e0a 3c2f  Area-prompt">.</
-0008d980: 6469 763e 3c64 6976 2063 6c61 7373 3d22  div><div class="
-0008d990: 6a70 2d52 656e 6465 7265 6448 544d 4c43  jp-RenderedHTMLC
-0008d9a0: 6f6d 6d6f 6e20 6a70 2d52 656e 6465 7265  ommon jp-Rendere
-0008d9b0: 644d 6172 6b64 6f77 6e20 6a70 2d4d 6172  dMarkdown jp-Mar
-0008d9c0: 6b64 6f77 6e4f 7574 7075 7420 2220 6461  kdownOutput " da
-0008d9d0: 7461 2d6d 696d 652d 7479 7065 3d22 7465  ta-mime-type="te
-0008d9e0: 7874 2f6d 6172 6b64 6f77 6e22 3e0a 3c70  xt/markdown">.<p
-0008d9f0: 3e54 6865 203c 7374 726f 6e67 3e70 7265  >The <strong>pre
-0008da00: 7072 6f63 6573 7369 6e67 3c2f 7374 726f  processing</stro
-0008da10: 6e67 3e20 6d6f 6475 6c65 2070 726f 7669  ng> module provi
-0008da20: 6465 7320 736f 6d65 2066 756e 6374 696f  des some functio
-0008da30: 6e73 2074 6f20 776f 726b 2064 6174 613a  ns to work data:
-0008da40: 3c2f 703e 0a3c 703e 4261 7369 6320 6675  </p>.<p>Basic fu
-0008da50: 6e63 7469 6f6e 733a 3c2f 703e 0a3c 756c  nctions:</p>.<ul
-0008da60: 3e0a 3c6c 693e 3c63 6f64 653e 7265 6164  >.<li><code>read
-0008da70: 4461 7461 7365 743c 2f63 6f64 653e 3a20  Dataset</code>: 
-0008da80: 6c6f 6164 2064 6174 6173 6574 7320 6173  load datasets as
-0008da90: 2070 616e 6461 7320 4461 7461 4672 616d   pandas DataFram
-0008daa0: 6520 2866 726f 6d20 2e63 7376 2c20 2e7a  e (from .csv, .z
-0008dab0: 6970 2c20 6f72 202e 7473 293c 2f6c 693e  ip, or .ts)</li>
-0008dac0: 0a3c 6c69 3e3c 636f 6465 3e70 7269 6e74  .<li><code>print
-0008dad0: 4665 6174 7572 6573 4a53 4f4e 3c2f 636f  FeaturesJSON</co
-0008dae0: 6465 3e3a 2070 7269 6e74 2061 2064 6566  de>: print a def
-0008daf0: 6175 6c74 204a 534f 4e20 6669 6c65 2064  ault JSON file d
-0008db00: 6573 6372 6970 746f 7220 666f 7220 4d6f  escriptor for Mo
-0008db10: 7665 6c65 7473 206d 6574 686f 6473 2028  velets methods (
-0008db20: 7665 7273 696f 6e20 3120 6f72 2032 293c  version 1 or 2)<
-0008db30: 2f6c 693e 0a3c 6c69 3e3c 636f 6465 3e64  /li>.<li><code>d
-0008db40: 6174 6173 6574 5374 6174 6973 7469 6373  atasetStatistics
-0008db50: 3c2f 636f 6465 3e3a 2063 616c 6375 6c61  </code>: calcula
-0008db60: 7465 7320 7374 6174 6973 7469 6373 2066  tes statistics f
-0008db70: 726f 6d20 6120 6461 7461 7365 7473 2064  rom a datasets d
-0008db80: 6174 6166 7261 6d65 2e3c 2f6c 693e 0a3c  ataframe.</li>.<
-0008db90: 2f75 6c3e 0a3c 703e 5472 6169 6e20 616e  /ul>.<p>Train an
-0008dba0: 6420 5465 7374 2073 706c 6974 2066 756e  d Test split fun
-0008dbb0: 6374 696f 6e73 3a3c 2f70 3e0a 3c75 6c3e  ctions:</p>.<ul>
-0008dbc0: 0a3c 6c69 3e3c 636f 6465 3e74 7261 696e  .<li><code>train
-0008dbd0: 416e 6454 6573 7453 706c 6974 3c2f 636f  AndTestSplit</co
-0008dbe0: 6465 3e3a 2073 706c 6974 2064 6174 6173  de>: split datas
-0008dbf0: 6574 2028 7061 6e64 6173 2044 6174 6146  et (pandas DataF
-0008dc00: 7261 6d65 2920 696e 2074 7261 696e 202f  rame) in train /
-0008dc10: 2074 6573 7420 2837 302f 3330 2520 6279   test (70/30% by
-0008dc20: 2064 6566 6175 6c74 293c 2f6c 693e 0a3c   default)</li>.<
-0008dc30: 6c69 3e3c 636f 6465 3e6b 666f 6c64 5f74  li><code>kfold_t
-0008dc40: 7261 696e 416e 6454 6573 7453 706c 6974  rainAndTestSplit
-0008dc50: 3c2f 636f 6465 3e3a 2073 706c 6974 2064  </code>: split d
-0008dc60: 6174 6173 6574 2028 7061 6e64 6173 2044  ataset (pandas D
-0008dc70: 6174 6146 7261 6d65 2920 696e 206b 2d66  ataFrame) in k-f
-0008dc80: 6f6c 6420 7472 6169 6e20 2f20 7465 7374  old train / test
-0008dc90: 2028 3830 2f32 3025 2065 6163 6820 666f   (80/20% each fo
-0008dca0: 6c64 2062 7920 6465 6661 756c 7429 3c2f  ld by default)</
-0008dcb0: 6c69 3e0a 3c6c 693e 3c63 6f64 653e 7374  li>.<li><code>st
-0008dcc0: 7261 7469 6679 3c2f 636f 6465 3e3a 2065  ratify</code>: e
-0008dcd0: 7874 7261 6374 2074 7261 6a65 6374 6f72  xtract trajector
-0008dce0: 6965 7320 6672 6f6d 2074 6865 2064 6174  ies from the dat
-0008dcf0: 6173 6574 2c20 6372 6561 7469 6e67 2061  aset, creating a
-0008dd00: 2073 7562 7365 7420 6f66 2074 6865 2064   subset of the d
-0008dd10: 6174 6120 2874 6f20 7573 6520 7768 656e  ata (to use when
-0008dd20: 2073 6d61 6c6c 6572 2064 6174 6173 6574   smaller dataset
-0008dd30: 7320 6172 6520 6e65 6564 6564 293c 2f6c  s are needed)</l
-0008dd40: 693e 0a3c 6c69 3e3c 636f 6465 3e6a 6f69  i>.<li><code>joi
-0008dd50: 6e54 7261 696e 416e 6454 6573 743c 2f63  nTrainAndTest</c
-0008dd60: 6f64 653e 3a20 6a6f 696e 7320 7468 6520  ode>: joins the 
-0008dd70: 7472 6169 6e20 616e 6420 7465 7374 2066  train and test f
-0008dd80: 696c 6573 2069 6e74 6f20 6f6e 6520 4461  iles into one Da
-0008dd90: 7461 4672 616d 652e 3c2f 6c69 3e0a 3c2f  taFrame.</li>.</
-0008dda0: 756c 3e0a 3c70 3e54 7970 6520 636f 6e76  ul>.<p>Type conv
-0008ddb0: 6572 7469 6f6e 2066 756e 6374 696f 6e73  ertion functions
-0008ddc0: 3a3c 2f70 3e0a 3c75 6c3e 0a3c 6c69 3e3c  :</p>.<ul>.<li><
-0008ddd0: 636f 6465 3e63 6f6e 7665 7274 4461 7461  code>convertData
-0008dde0: 7365 743c 2f63 6f64 653e 3a20 6465 6661  set</code>: defa
-0008ddf0: 756c 7420 666f 726d 6174 2063 6f6e 7665  ult format conve
-0008de00: 7273 696f 6e73 2e20 5265 6164 7320 7468  rsions. Reads th
-0008de10: 6520 6461 7461 7365 7420 6669 6c65 7320  e dataset files 
-0008de20: 616e 6420 7361 7665 7320 696e 202e 6373  and saves in .cs
-0008de30: 7620 616e 6420 2e7a 6970 2066 6f72 6d61  v and .zip forma
-0008de40: 7473 2c20 616c 736f 2064 6f20 6b2d 666f  ts, also do k-fo
-0008de50: 6c64 2073 706c 6974 2069 6620 6e6f 7420  ld split if not 
-0008de60: 7072 6573 656e 743c 2f6c 693e 0a3c 6c69  present</li>.<li
-0008de70: 3e3c 636f 6465 3e7a 6970 3264 663c 2f63  ><code>zip2df</c
-0008de80: 6f64 653e 3a20 636f 6e76 6572 7473 202e  ode>: converts .
-0008de90: 7a69 7020 6669 6c65 7320 616e 6420 7361  zip files and sa
-0008dea0: 7665 7320 746f 2044 6174 6146 7261 6d65  ves to DataFrame
-0008deb0: 3c2f 6c69 3e0a 3c6c 693e 3c63 6f64 653e  </li>.<li><code>
-0008dec0: 7a69 7032 6373 763c 2f63 6f64 653e 3a20  zip2csv</code>: 
-0008ded0: 636f 6e76 6572 7473 202e 7a69 7020 6669  converts .zip fi
-0008dee0: 6c65 7320 616e 6420 7361 7665 7320 746f  les and saves to
-0008def0: 202e 6373 7620 6669 6c65 733c 2f6c 693e   .csv files</li>
-0008df00: 0a3c 6c69 3e3c 636f 6465 3e64 6632 7a69  .<li><code>df2zi
-0008df10: 703c 2f63 6f64 653e 3a20 636f 6e76 6572  p</code>: conver
-0008df20: 7473 2044 6174 6146 7261 6d65 2061 6e64  ts DataFrame and
-0008df30: 2073 6176 6573 2074 6f20 2e7a 6970 2066   saves to .zip f
-0008df40: 696c 6573 3c2f 6c69 3e0a 3c6c 693e 3c63  iles</li>.<li><c
-0008df50: 6f64 653e 7a69 7032 6172 663c 2f63 6f64  ode>zip2arf</cod
-0008df60: 653e 3a20 636f 6e76 6572 7473 202e 7a69  e>: converts .zi
-0008df70: 7020 616e 6420 7361 7665 7320 746f 202e  p and saves to .
-0008df80: 6172 6620 6669 6c65 733c 2f6c 693e 0a3c  arf files</li>.<
-0008df90: 6c69 3e3c 636f 6465 3e61 6e79 3274 733c  li><code>any2ts<
-0008dfa0: 2f63 6f64 653e 3a20 636f 6e76 6572 7473  /code>: converts
-0008dfb0: 202e 7a69 7020 6f72 202e 6373 7620 6669   .zip or .csv fi
-0008dfc0: 6c65 7320 616e 6420 7361 7665 7320 746f  les and saves to
-0008dfd0: 202e 7473 2066 696c 6573 3c2f 6c69 3e0a   .ts files</li>.
-0008dfe0: 3c6c 693e 3c63 6f64 653e 7865 7332 6373  <li><code>xes2cs
-0008dff0: 763c 2f63 6f64 653e 3a20 7265 6164 7320  v</code>: reads 
-0008e000: 2e78 6573 2066 696c 6573 2061 6e64 2063  .xes files and c
-0008e010: 6f6e 7665 7274 7320 746f 2044 6174 6146  onverts to DataF
-0008e020: 7261 6d65 3c2f 6c69 3e0a 3c2f 756c 3e0a  rame</li>.</ul>.
-0008e030: 0a3c 2f64 6976 3e0a 3c2f 6469 763e 0a3c  .</div>.</div>.<
-0008e040: 2f64 6976 3e0a 3c2f 6469 763e 3c64 6976  /div>.</div><div
-0008e050: 2063 6c61 7373 3d22 6a70 2d43 656c 6c20   class="jp-Cell 
-0008e060: 6a70 2d43 6f64 6543 656c 6c20 6a70 2d4e  jp-CodeCell jp-N
-0008e070: 6f74 6562 6f6f 6b2d 6365 6c6c 2020 2022  otebook-cell   "
-0008e080: 3e0a 3c64 6976 2063 6c61 7373 3d22 6a70  >.<div class="jp
-0008e090: 2d43 656c 6c2d 696e 7075 7457 7261 7070  -Cell-inputWrapp
-0008e0a0: 6572 223e 0a3c 6469 7620 636c 6173 733d  er">.<div class=
-0008e0b0: 226a 702d 436f 6c6c 6170 7365 7220 6a70  "jp-Collapser jp
-0008e0c0: 2d49 6e70 7574 436f 6c6c 6170 7365 7220  -InputCollapser 
-0008e0d0: 6a70 2d43 656c 6c2d 696e 7075 7443 6f6c  jp-Cell-inputCol
-0008e0e0: 6c61 7073 6572 223e 0a3c 2f64 6976 3e0a  lapser">.</div>.
-0008e0f0: 3c64 6976 2063 6c61 7373 3d22 6a70 2d49  <div class="jp-I
-0008e100: 6e70 7574 4172 6561 206a 702d 4365 6c6c  nputArea jp-Cell
-0008e110: 2d69 6e70 7574 4172 6561 223e 0a3c 6469  -inputArea">.<di
-0008e120: 7620 636c 6173 733d 226a 702d 496e 7075  v class="jp-Inpu
-0008e130: 7450 726f 6d70 7420 6a70 2d49 6e70 7574  tPrompt jp-Input
-0008e140: 4172 6561 2d70 726f 6d70 7422 3e49 6e26  Area-prompt">In&
-0008e150: 6e62 7370 3b5b 3130 5d3a 3c2f 6469 763e  nbsp;[10]:</div>
-0008e160: 0a3c 6469 7620 636c 6173 733d 226a 702d  .<div class="jp-
-0008e170: 436f 6465 4d69 7272 6f72 4564 6974 6f72  CodeMirrorEditor
-0008e180: 206a 702d 4564 6974 6f72 206a 702d 496e   jp-Editor jp-In
-0008e190: 7075 7441 7265 612d 6564 6974 6f72 2220  putArea-editor" 
-0008e1a0: 6461 7461 2d74 7970 653d 2269 6e6c 696e  data-type="inlin
-0008e1b0: 6522 3e0a 2020 2020 203c 6469 7620 636c  e">.     <div cl
-0008e1c0: 6173 733d 2243 6f64 654d 6972 726f 7220  ass="CodeMirror 
-0008e1d0: 636d 2d73 2d6a 7570 7974 6572 223e 0a3c  cm-s-jupyter">.<
-0008e1e0: 6469 7620 636c 6173 733d 2220 6869 6768  div class=" high
-0008e1f0: 6c69 6768 7420 686c 2d69 7079 7468 6f6e  light hl-ipython
-0008e200: 3322 3e3c 7072 653e 3c73 7061 6e3e 3c2f  3"><pre><span></
-0008e210: 7370 616e 3e3c 7370 616e 2063 6c61 7373  span><span class
-0008e220: 3d22 6331 223e 2363 6f6c 7320 3d20 5b26  ="c1">#cols = [&
-0008e230: 2333 393b 7469 6426 2333 393b 2c26 2333  #39;tid&#39;,&#3
-0008e240: 393b 6c61 6265 6c26 2333 393b 2c26 2333  9;label&#39;,&#3
-0008e250: 393b 6c61 7426 2333 393b 2c26 2333 393b  9;lat&#39;,&#39;
-0008e260: 6c6f 6e26 2333 393b 2c26 2333 393b 6461  lon&#39;,&#39;da
-0008e270: 7926 2333 393b 2c26 2333 393b 686f 7572  y&#39;,&#39;hour
-0008e280: 2623 3339 3b2c 2623 3339 3b70 6f69 2623  &#39;,&#39;poi&#
-0008e290: 3339 3b2c 2623 3339 3b63 6174 6567 6f72  39;,&#39;categor
-0008e2a0: 7926 2333 393b 2c26 2333 393b 7072 6963  y&#39;,&#39;pric
-0008e2b0: 6526 2333 393b 2c26 2333 393b 7261 7469  e&#39;,&#39;rati
-0008e2c0: 6e67 2623 3339 3b5d 3c2f 7370 616e 3e0a  ng&#39;]</span>.
-0008e2d0: 0a3c 7370 616e 2063 6c61 7373 3d22 6e22  .<span class="n"
-0008e2e0: 3e64 663c 2f73 7061 6e3e 203c 7370 616e  >df</span> <span
-0008e2f0: 2063 6c61 7373 3d22 6f22 3e3d 3c2f 7370   class="o">=</sp
-0008e300: 616e 3e20 3c73 7061 6e20 636c 6173 733d  an> <span class=
-0008e310: 226e 223e 6a6f 696e 5472 6169 6e41 6e64  "n">joinTrainAnd
-0008e320: 5465 7374 3c2f 7370 616e 3e3c 7370 616e  Test</span><span
-0008e330: 2063 6c61 7373 3d22 7022 3e28 3c2f 7370   class="p">(</sp
-0008e340: 616e 3e3c 7370 616e 2063 6c61 7373 3d22  an><span class="
-0008e350: 6e22 3e64 6174 615f 7061 7468 3c2f 7370  n">data_path</sp
-0008e360: 616e 3e3c 7370 616e 2063 6c61 7373 3d22  an><span class="
-0008e370: 7022 3e2c 3c2f 7370 616e 3e20 3c73 7061  p">,</span> <spa
-0008e380: 6e20 636c 6173 733d 226e 223e 7472 6169  n class="n">trai
-0008e390: 6e5f 6669 6c65 3c2f 7370 616e 3e3c 7370  n_file</span><sp
-0008e3a0: 616e 2063 6c61 7373 3d22 6f22 3e3d 3c2f  an class="o">=</
-0008e3b0: 7370 616e 3e3c 7370 616e 2063 6c61 7373  span><span class
-0008e3c0: 3d22 7332 223e 2671 756f 743b 7472 6169  ="s2">&quot;trai
-0008e3d0: 6e2e 6373 7626 7175 6f74 3b3c 2f73 7061  n.csv&quot;</spa
-0008e3e0: 6e3e 3c73 7061 6e20 636c 6173 733d 2270  n><span class="p
-0008e3f0: 223e 2c3c 2f73 7061 6e3e 203c 7370 616e  ">,</span> <span
-0008e400: 2063 6c61 7373 3d22 6e22 3e74 6573 745f   class="n">test_
-0008e410: 6669 6c65 3c2f 7370 616e 3e3c 7370 616e  file</span><span
-0008e420: 2063 6c61 7373 3d22 6f22 3e3d 3c2f 7370   class="o">=</sp
-0008e430: 616e 3e3c 7370 616e 2063 6c61 7373 3d22  an><span class="
-0008e440: 7332 223e 2671 756f 743b 7465 7374 2e63  s2">&quot;test.c
-0008e450: 7376 2671 756f 743b 3c2f 7370 616e 3e3c  sv&quot;</span><
-0008e460: 7370 616e 2063 6c61 7373 3d22 7022 3e2c  span class="p">,
-0008e470: 3c2f 7370 616e 3e20 3c73 7061 6e20 636c  </span> <span cl
-0008e480: 6173 733d 226e 223e 636c 6173 735f 636f  ass="n">class_co
-0008e490: 6c3c 2f73 7061 6e3e 203c 7370 616e 2063  l</span> <span c
-0008e4a0: 6c61 7373 3d22 6f22 3e3d 3c2f 7370 616e  lass="o">=</span
-0008e4b0: 3e20 3c73 7061 6e20 636c 6173 733d 2273  > <span class="s
-0008e4c0: 3122 3e26 2333 393b 6c61 6265 6c26 2333  1">&#39;label&#3
-0008e4d0: 393b 3c2f 7370 616e 3e3c 7370 616e 2063  9;</span><span c
-0008e4e0: 6c61 7373 3d22 7022 3e29 3c2f 7370 616e  lass="p">)</span
-0008e4f0: 3e0a 3c73 7061 6e20 636c 6173 733d 226e  >.<span class="n
-0008e500: 223e 6466 3c2f 7370 616e 3e3c 7370 616e  ">df</span><span
-0008e510: 2063 6c61 7373 3d22 6f22 3e2e 3c2f 7370   class="o">.</sp
-0008e520: 616e 3e3c 7370 616e 2063 6c61 7373 3d22  an><span class="
-0008e530: 6e22 3e68 6561 643c 2f73 7061 6e3e 3c73  n">head</span><s
-0008e540: 7061 6e20 636c 6173 733d 2270 223e 2829  pan class="p">()
-0008e550: 3c2f 7370 616e 3e0a 3c2f 7072 653e 3c2f  </span>.</pre></
-0008e560: 6469 763e 0a0a 2020 2020 203c 2f64 6976  div>..     </div
-0008e570: 3e0a 3c2f 6469 763e 0a3c 2f64 6976 3e0a  >.</div>.</div>.
-0008e580: 3c2f 6469 763e 0a0a 3c64 6976 2063 6c61  </div>..<div cla
-0008e590: 7373 3d22 6a70 2d43 656c 6c2d 6f75 7470  ss="jp-Cell-outp
-0008e5a0: 7574 5772 6170 7065 7222 3e0a 3c64 6976  utWrapper">.<div
-0008e5b0: 2063 6c61 7373 3d22 6a70 2d43 6f6c 6c61   class="jp-Colla
-0008e5c0: 7073 6572 206a 702d 4f75 7470 7574 436f  pser jp-OutputCo
-0008e5d0: 6c6c 6170 7365 7220 6a70 2d43 656c 6c2d  llapser jp-Cell-
-0008e5e0: 6f75 7470 7574 436f 6c6c 6170 7365 7222  outputCollapser"
-0008e5f0: 3e0a 3c2f 6469 763e 0a0a 0a3c 6469 7620  >.</div>...<div 
-0008e600: 636c 6173 733d 226a 702d 4f75 7470 7574  class="jp-Output
-0008e610: 4172 6561 206a 702d 4365 6c6c 2d6f 7574  Area jp-Cell-out
-0008e620: 7075 7441 7265 6122 3e0a 0a3c 6469 7620  putArea">..<div 
-0008e630: 636c 6173 733d 226a 702d 4f75 7470 7574  class="jp-Output
-0008e640: 4172 6561 2d63 6869 6c64 223e 0a0a 2020  Area-child">..  
-0008e650: 2020 0a20 2020 203c 6469 7620 636c 6173    .    <div clas
-0008e660: 733d 226a 702d 4f75 7470 7574 5072 6f6d  s="jp-OutputProm
-0008e670: 7074 206a 702d 4f75 7470 7574 4172 6561  pt jp-OutputArea
-0008e680: 2d70 726f 6d70 7422 3e3c 2f64 6976 3e0a  -prompt"></div>.
-0008e690: 0a0a 3c64 6976 2063 6c61 7373 3d22 6a70  ..<div class="jp
-0008e6a0: 2d52 656e 6465 7265 6454 6578 7420 6a70  -RenderedText jp
-0008e6b0: 2d4f 7574 7075 7441 7265 612d 6f75 7470  -OutputArea-outp
-0008e6c0: 7574 2220 6461 7461 2d6d 696d 652d 7479  ut" data-mime-ty
-0008e6d0: 7065 3d22 7465 7874 2f70 6c61 696e 223e  pe="text/plain">
-0008e6e0: 0a3c 7072 653e 4a6f 696e 696e 6720 7472  .<pre>Joining tr
-0008e6f0: 6169 6e20 616e 6420 7465 7374 2064 6174  ain and test dat
-0008e700: 6120 6672 6f6d 2e2e 2e20 6175 746f 6d61  a from... automa
-0008e710: 7469 7a65 2f61 7373 6574 732f 6578 616d  tize/assets/exam
-0008e720: 706c 6573 2f45 7861 6d70 6c65 2f64 6174  ples/Example/dat
-0008e730: 610a 446f 6e65 2e0a 202d 2d2d 2d2d 2d2d  a.Done.. -------
-0008e740: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-0008e750: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-0008e760: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-0008e770: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-0008e780: 2d2d 2d2d 2d2d 2d2d 2d0a 3c2f 7072 653e  ---------.</pre>
-0008e790: 0a3c 2f64 6976 3e0a 3c2f 6469 763e 0a0a  .</div>.</div>..
-0008e7a0: 3c64 6976 2063 6c61 7373 3d22 6a70 2d4f  <div class="jp-O
-0008e7b0: 7574 7075 7441 7265 612d 6368 696c 6422  utputArea-child"
-0008e7c0: 3e0a 0a20 2020 200a 2020 2020 3c64 6976  >..    .    <div
-0008e7d0: 2063 6c61 7373 3d22 6a70 2d4f 7574 7075   class="jp-Outpu
-0008e7e0: 7450 726f 6d70 7420 6a70 2d4f 7574 7075  tPrompt jp-Outpu
-0008e7f0: 7441 7265 612d 7072 6f6d 7074 223e 4f75  tArea-prompt">Ou
-0008e800: 745b 3130 5d3a 3c2f 6469 763e 0a0a 0a0a  t[10]:</div>....
-0008e810: 3c64 6976 2063 6c61 7373 3d22 6a70 2d52  <div class="jp-R
-0008e820: 656e 6465 7265 6448 544d 4c43 6f6d 6d6f  enderedHTMLCommo
-0008e830: 6e20 6a70 2d52 656e 6465 7265 6448 544d  n jp-RenderedHTM
-0008e840: 4c20 6a70 2d4f 7574 7075 7441 7265 612d  L jp-OutputArea-
-0008e850: 6f75 7470 7574 206a 702d 4f75 7470 7574  output jp-Output
-0008e860: 4172 6561 2d65 7865 6375 7465 5265 7375  Area-executeResu
-0008e870: 6c74 2220 6461 7461 2d6d 696d 652d 7479  lt" data-mime-ty
-0008e880: 7065 3d22 7465 7874 2f68 746d 6c22 3e0a  pe="text/html">.
-0008e890: 3c64 6976 3e0a 3c73 7479 6c65 2073 636f  <div>.<style sco
-0008e8a0: 7065 643e 0a20 2020 202e 6461 7461 6672  ped>.    .datafr
-0008e8b0: 616d 6520 7462 6f64 7920 7472 2074 683a  ame tbody tr th:
-0008e8c0: 6f6e 6c79 2d6f 662d 7479 7065 207b 0a20  only-of-type {. 
-0008e8d0: 2020 2020 2020 2076 6572 7469 6361 6c2d         vertical-
-0008e8e0: 616c 6967 6e3a 206d 6964 646c 653b 0a20  align: middle;. 
-0008e8f0: 2020 207d 0a0a 2020 2020 2e64 6174 6166     }..    .dataf
-0008e900: 7261 6d65 2074 626f 6479 2074 7220 7468  rame tbody tr th
-0008e910: 207b 0a20 2020 2020 2020 2076 6572 7469   {.        verti
-0008e920: 6361 6c2d 616c 6967 6e3a 2074 6f70 3b0a  cal-align: top;.
-0008e930: 2020 2020 7d0a 0a20 2020 202e 6461 7461      }..    .data
-0008e940: 6672 616d 6520 7468 6561 6420 7468 207b  frame thead th {
-0008e950: 0a20 2020 2020 2020 2074 6578 742d 616c  .        text-al
-0008e960: 6967 6e3a 2072 6967 6874 3b0a 2020 2020  ign: right;.    
-0008e970: 7d0a 3c2f 7374 796c 653e 0a3c 7461 626c  }.</style>.<tabl
-0008e980: 6520 626f 7264 6572 3d22 3122 2063 6c61  e border="1" cla
-0008e990: 7373 3d22 6461 7461 6672 616d 6522 3e0a  ss="dataframe">.
-0008e9a0: 2020 3c74 6865 6164 3e0a 2020 2020 3c74    <thead>.    <t
-0008e9b0: 7220 7374 796c 653d 2274 6578 742d 616c  r style="text-al
-0008e9c0: 6967 6e3a 2072 6967 6874 3b22 3e0a 2020  ign: right;">.  
-0008e9d0: 2020 2020 3c74 683e 3c2f 7468 3e0a 2020      <th></th>.  
-0008e9e0: 2020 2020 3c74 683e 7469 643c 2f74 683e      <th>tid</th>
-0008e9f0: 0a20 2020 2020 203c 7468 3e6c 6174 5f6c  .      <th>lat_l
-0008ea00: 6f6e 3c2f 7468 3e0a 2020 2020 2020 3c74  on</th>.      <t
-0008ea10: 683e 686f 7572 3c2f 7468 3e0a 2020 2020  h>hour</th>.    
-0008ea20: 2020 3c74 683e 7072 6963 653c 2f74 683e    <th>price</th>
-0008ea30: 0a20 2020 2020 203c 7468 3e70 6f69 3c2f  .      <th>poi</
-0008ea40: 7468 3e0a 2020 2020 2020 3c74 683e 7765  th>.      <th>we
-0008ea50: 6174 6865 723c 2f74 683e 0a20 2020 2020  ather</th>.     
-0008ea60: 203c 7468 3e64 6179 3c2f 7468 3e0a 2020   <th>day</th>.  
-0008ea70: 2020 2020 3c74 683e 6c61 6265 6c3c 2f74      <th>label</t
-0008ea80: 683e 0a20 2020 203c 2f74 723e 0a20 203c  h>.    </tr>.  <
-0008ea90: 2f74 6865 6164 3e0a 2020 3c74 626f 6479  /thead>.  <tbody
-0008eaa0: 3e0a 2020 2020 3c74 723e 0a20 2020 2020  >.    <tr>.     
-0008eab0: 203c 7468 3e30 3c2f 7468 3e0a 2020 2020   <th>0</th>.    
-0008eac0: 2020 3c74 643e 3132 3c2f 7464 3e0a 2020    <td>12</td>.  
-0008ead0: 2020 2020 3c74 643e 302e 3020 362e 323c      <td>0.0 6.2<
-0008eae0: 2f74 643e 0a20 2020 2020 203c 7464 3e38  /td>.      <td>8
-0008eaf0: 3c2f 7464 3e0a 2020 2020 2020 3c74 643e  </td>.      <td>
-0008eb00: 2d31 3c2f 7464 3e0a 2020 2020 2020 3c74  -1</td>.      <t
-0008eb10: 643e 486f 6d65 3c2f 7464 3e0a 2020 2020  d>Home</td>.    
-0008eb20: 2020 3c74 643e 436c 6561 723c 2f74 643e    <td>Clear</td>
-0008eb30: 0a20 2020 2020 203c 7464 3e4d 6f6e 6461  .      <td>Monda
-0008eb40: 793c 2f74 643e 0a20 2020 2020 203c 7464  y</td>.      <td
-0008eb50: 3e43 6c61 7373 735f 4661 6c73 653c 2f74  >Classs_False</t
-0008eb60: 643e 0a20 2020 203c 2f74 723e 0a20 2020  d>.    </tr>.   
-0008eb70: 203c 7472 3e0a 2020 2020 2020 3c74 683e   <tr>.      <th>
-0008eb80: 313c 2f74 683e 0a20 2020 2020 203c 7464  1</th>.      <td
-0008eb90: 3e31 323c 2f74 643e 0a20 2020 2020 203c  >12</td>.      <
-0008eba0: 7464 3e30 2e38 2036 2e32 3c2f 7464 3e0a  td>0.8 6.2</td>.
-0008ebb0: 2020 2020 2020 3c74 643e 393c 2f74 643e        <td>9</td>
-0008ebc0: 0a20 2020 2020 203c 7464 3e32 3c2f 7464  .      <td>2</td
-0008ebd0: 3e0a 2020 2020 2020 3c74 643e 556e 6976  >.      <td>Univ
-0008ebe0: 6572 7369 7479 3c2f 7464 3e0a 2020 2020  ersity</td>.    
-0008ebf0: 2020 3c74 643e 436c 6f75 6473 3c2f 7464    <td>Clouds</td
-0008ec00: 3e0a 2020 2020 2020 3c74 643e 4d6f 6e64  >.      <td>Mond
-0008ec10: 6179 3c2f 7464 3e0a 2020 2020 2020 3c74  ay</td>.      <t
-0008ec20: 643e 436c 6173 7373 5f46 616c 7365 3c2f  d>Classs_False</
-0008ec30: 7464 3e0a 2020 2020 3c2f 7472 3e0a 2020  td>.    </tr>.  
-0008ec40: 2020 3c74 723e 0a20 2020 2020 203c 7468    <tr>.      <th
-0008ec50: 3e32 3c2f 7468 3e0a 2020 2020 2020 3c74  >2</th>.      <t
-0008ec60: 643e 3132 3c2f 7464 3e0a 2020 2020 2020  d>12</td>.      
-0008ec70: 3c74 643e 332e 3120 3131 3c2f 7464 3e0a  <td>3.1 11</td>.
-0008ec80: 2020 2020 2020 3c74 643e 3132 3c2f 7464        <td>12</td
-0008ec90: 3e0a 2020 2020 2020 3c74 643e 323c 2f74  >.      <td>2</t
-0008eca0: 643e 0a20 2020 2020 203c 7464 3e52 6573  d>.      <td>Res
-0008ecb0: 7461 7572 616e 743c 2f74 643e 0a20 2020  taurant</td>.   
-0008ecc0: 2020 203c 7464 3e43 6c65 6172 3c2f 7464     <td>Clear</td
-0008ecd0: 3e0a 2020 2020 2020 3c74 643e 4d6f 6e64  >.      <td>Mond
-0008ece0: 6179 3c2f 7464 3e0a 2020 2020 2020 3c74  ay</td>.      <t
-0008ecf0: 643e 436c 6173 7373 5f46 616c 7365 3c2f  d>Classs_False</
-0008ed00: 7464 3e0a 2020 2020 3c2f 7472 3e0a 2020  td>.    </tr>.  
-0008ed10: 2020 3c74 723e 0a20 2020 2020 203c 7468    <tr>.      <th
-0008ed20: 3e33 3c2f 7468 3e0a 2020 2020 2020 3c74  >3</th>.      <t
-0008ed30: 643e 3132 3c2f 7464 3e0a 2020 2020 2020  d>12</td>.      
-0008ed40: 3c74 643e 302e 3820 362e 353c 2f74 643e  <td>0.8 6.5</td>
-0008ed50: 0a20 2020 2020 203c 7464 3e31 333c 2f74  .      <td>13</t
-0008ed60: 643e 0a20 2020 2020 203c 7464 3e32 3c2f  d>.      <td>2</
-0008ed70: 7464 3e0a 2020 2020 2020 3c74 643e 556e  td>.      <td>Un
-0008ed80: 6976 6572 7369 7479 3c2f 7464 3e0a 2020  iversity</td>.  
-0008ed90: 2020 2020 3c74 643e 436c 6561 723c 2f74      <td>Clear</t
-0008eda0: 643e 0a20 2020 2020 203c 7464 3e4d 6f6e  d>.      <td>Mon
-0008edb0: 6461 793c 2f74 643e 0a20 2020 2020 203c  day</td>.      <
-0008edc0: 7464 3e43 6c61 7373 735f 4661 6c73 653c  td>Classs_False<
-0008edd0: 2f74 643e 0a20 2020 203c 2f74 723e 0a20  /td>.    </tr>. 
-0008ede0: 2020 203c 7472 3e0a 2020 2020 2020 3c74     <tr>.      <t
-0008edf0: 683e 343c 2f74 683e 0a20 2020 2020 203c  h>4</th>.      <
-0008ee00: 7464 3e31 323c 2f74 643e 0a20 2020 2020  td>12</td>.     
-0008ee10: 203c 7464 3e30 2e32 2036 2e32 3c2f 7464   <td>0.2 6.2</td
-0008ee20: 3e0a 2020 2020 2020 3c74 643e 3137 3c2f  >.      <td>17</
-0008ee30: 7464 3e0a 2020 2020 2020 3c74 643e 2d31  td>.      <td>-1
-0008ee40: 3c2f 7464 3e0a 2020 2020 2020 3c74 643e  </td>.      <td>
-0008ee50: 486f 6d65 3c2f 7464 3e0a 2020 2020 2020  Home</td>.      
-0008ee60: 3c74 643e 5261 696e 3c2f 7464 3e0a 2020  <td>Rain</td>.  
-0008ee70: 2020 2020 3c74 643e 4d6f 6e64 6179 3c2f      <td>Monday</
-0008ee80: 7464 3e0a 2020 2020 2020 3c74 643e 436c  td>.      <td>Cl
-0008ee90: 6173 7373 5f46 616c 7365 3c2f 7464 3e0a  asss_False</td>.
-0008eea0: 2020 2020 3c2f 7472 3e0a 2020 3c2f 7462      </tr>.  </tb
-0008eeb0: 6f64 793e 0a3c 2f74 6162 6c65 3e0a 3c2f  ody>.</table>.</
-0008eec0: 6469 763e 0a3c 2f64 6976 3e0a 0a3c 2f64  div>.</div>..</d
-0008eed0: 6976 3e0a 0a3c 2f64 6976 3e0a 0a3c 2f64  iv>..</div>..</d
-0008eee0: 6976 3e0a 0a3c 2f64 6976 3e0a 3c64 6976  iv>..</div>.<div
-0008eef0: 2063 6c61 7373 3d22 6a70 2d43 656c 6c20   class="jp-Cell 
-0008ef00: 6a70 2d4d 6172 6b64 6f77 6e43 656c 6c20  jp-MarkdownCell 
-0008ef10: 6a70 2d4e 6f74 6562 6f6f 6b2d 6365 6c6c  jp-Notebook-cell
-0008ef20: 223e 0a3c 6469 7620 636c 6173 733d 226a  ">.<div class="j
-0008ef30: 702d 4365 6c6c 2d69 6e70 7574 5772 6170  p-Cell-inputWrap
-0008ef40: 7065 7222 3e0a 3c64 6976 2063 6c61 7373  per">.<div class
-0008ef50: 3d22 6a70 2d43 6f6c 6c61 7073 6572 206a  ="jp-Collapser j
-0008ef60: 702d 496e 7075 7443 6f6c 6c61 7073 6572  p-InputCollapser
-0008ef70: 206a 702d 4365 6c6c 2d69 6e70 7574 436f   jp-Cell-inputCo
-0008ef80: 6c6c 6170 7365 7222 3e0a 3c2f 6469 763e  llapser">.</div>
-0008ef90: 0a3c 6469 7620 636c 6173 733d 226a 702d  .<div class="jp-
-0008efa0: 496e 7075 7441 7265 6120 6a70 2d43 656c  InputArea jp-Cel
-0008efb0: 6c2d 696e 7075 7441 7265 6122 3e3c 6469  l-inputArea"><di
-0008efc0: 7620 636c 6173 733d 226a 702d 496e 7075  v class="jp-Inpu
-0008efd0: 7450 726f 6d70 7420 6a70 2d49 6e70 7574  tPrompt jp-Input
-0008efe0: 4172 6561 2d70 726f 6d70 7422 3e0a 3c2f  Area-prompt">.</
-0008eff0: 6469 763e 3c64 6976 2063 6c61 7373 3d22  div><div class="
-0008f000: 6a70 2d52 656e 6465 7265 6448 544d 4c43  jp-RenderedHTMLC
-0008f010: 6f6d 6d6f 6e20 6a70 2d52 656e 6465 7265  ommon jp-Rendere
-0008f020: 644d 6172 6b64 6f77 6e20 6a70 2d4d 6172  dMarkdown jp-Mar
-0008f030: 6b64 6f77 6e4f 7574 7075 7420 2220 6461  kdownOutput " da
-0008f040: 7461 2d6d 696d 652d 7479 7065 3d22 7465  ta-mime-type="te
-0008f050: 7874 2f6d 6172 6b64 6f77 6e22 3e0a 3c70  xt/markdown">.<p
-0008f060: 3e54 6f20 6b2d 666f 6c64 2073 706c 6974  >To k-fold split
-0008f070: 2061 2064 6174 6173 6574 2069 6e74 6f20   a dataset into 
-0008f080: 7472 6169 6e20 616e 6420 7465 7374 3a3c  train and test:<
-0008f090: 2f70 3e0a 0a3c 2f64 6976 3e0a 3c2f 6469  /p>..</div>.</di
-0008f0a0: 763e 0a3c 2f64 6976 3e0a 3c2f 6469 763e  v>.</div>.</div>
-0008f0b0: 3c64 6976 2063 6c61 7373 3d22 6a70 2d43  <div class="jp-C
-0008f0c0: 656c 6c20 6a70 2d43 6f64 6543 656c 6c20  ell jp-CodeCell 
-0008f0d0: 6a70 2d4e 6f74 6562 6f6f 6b2d 6365 6c6c  jp-Notebook-cell
-0008f0e0: 2020 2022 3e0a 3c64 6976 2063 6c61 7373     ">.<div class
-0008f0f0: 3d22 6a70 2d43 656c 6c2d 696e 7075 7457  ="jp-Cell-inputW
-0008f100: 7261 7070 6572 223e 0a3c 6469 7620 636c  rapper">.<div cl
-0008f110: 6173 733d 226a 702d 436f 6c6c 6170 7365  ass="jp-Collapse
-0008f120: 7220 6a70 2d49 6e70 7574 436f 6c6c 6170  r jp-InputCollap
-0008f130: 7365 7220 6a70 2d43 656c 6c2d 696e 7075  ser jp-Cell-inpu
-0008f140: 7443 6f6c 6c61 7073 6572 223e 0a3c 2f64  tCollapser">.</d
-0008f150: 6976 3e0a 3c64 6976 2063 6c61 7373 3d22  iv>.<div class="
-0008f160: 6a70 2d49 6e70 7574 4172 6561 206a 702d  jp-InputArea jp-
-0008f170: 4365 6c6c 2d69 6e70 7574 4172 6561 223e  Cell-inputArea">
-0008f180: 0a3c 6469 7620 636c 6173 733d 226a 702d  .<div class="jp-
-0008f190: 496e 7075 7450 726f 6d70 7420 6a70 2d49  InputPrompt jp-I
-0008f1a0: 6e70 7574 4172 6561 2d70 726f 6d70 7422  nputArea-prompt"
-0008f1b0: 3e49 6e26 6e62 7370 3b5b 3131 5d3a 3c2f  >In&nbsp;[11]:</
-0008f1c0: 6469 763e 0a3c 6469 7620 636c 6173 733d  div>.<div class=
-0008f1d0: 226a 702d 436f 6465 4d69 7272 6f72 4564  "jp-CodeMirrorEd
-0008f1e0: 6974 6f72 206a 702d 4564 6974 6f72 206a  itor jp-Editor j
-0008f1f0: 702d 496e 7075 7441 7265 612d 6564 6974  p-InputArea-edit
-0008f200: 6f72 2220 6461 7461 2d74 7970 653d 2269  or" data-type="i
-0008f210: 6e6c 696e 6522 3e0a 2020 2020 203c 6469  nline">.     <di
-0008f220: 7620 636c 6173 733d 2243 6f64 654d 6972  v class="CodeMir
-0008f230: 726f 7220 636d 2d73 2d6a 7570 7974 6572  ror cm-s-jupyter
-0008f240: 223e 0a3c 6469 7620 636c 6173 733d 2220  ">.<div class=" 
-0008f250: 6869 6768 6c69 6768 7420 686c 2d69 7079  highlight hl-ipy
-0008f260: 7468 6f6e 3322 3e3c 7072 653e 3c73 7061  thon3"><pre><spa
-0008f270: 6e3e 3c2f 7370 616e 3e3c 7370 616e 2063  n></span><span c
-0008f280: 6c61 7373 3d22 6e22 3e6b 3c2f 7370 616e  lass="n">k</span
-0008f290: 3e20 3c73 7061 6e20 636c 6173 733d 226f  > <span class="o
-0008f2a0: 223e 3d3c 2f73 7061 6e3e 203c 7370 616e  ">=</span> <span
-0008f2b0: 2063 6c61 7373 3d22 6d69 223e 333c 2f73   class="mi">3</s
-0008f2c0: 7061 6e3e 0a0a 3c73 7061 6e20 636c 6173  pan>..<span clas
-0008f2d0: 733d 226e 223e 7472 6169 6e3c 2f73 7061  s="n">train</spa
-0008f2e0: 6e3e 3c73 7061 6e20 636c 6173 733d 2270  n><span class="p
-0008f2f0: 223e 2c3c 2f73 7061 6e3e 203c 7370 616e  ">,</span> <span
-0008f300: 2063 6c61 7373 3d22 6e22 3e74 6573 743c   class="n">test<
-0008f310: 2f73 7061 6e3e 203c 7370 616e 2063 6c61  /span> <span cla
-0008f320: 7373 3d22 6f22 3e3d 3c2f 7370 616e 3e20  ss="o">=</span> 
-0008f330: 3c73 7061 6e20 636c 6173 733d 226e 223e  <span class="n">
-0008f340: 6b66 6f6c 645f 7472 6169 6e41 6e64 5465  kfold_trainAndTe
-0008f350: 7374 5370 6c69 743c 2f73 7061 6e3e 3c73  stSplit</span><s
-0008f360: 7061 6e20 636c 6173 733d 2270 223e 283c  pan class="p">(<
-0008f370: 2f73 7061 6e3e 3c73 7061 6e20 636c 6173  /span><span clas
-0008f380: 733d 226e 223e 6461 7461 5f70 6174 683c  s="n">data_path<
-0008f390: 2f73 7061 6e3e 3c73 7061 6e20 636c 6173  /span><span clas
-0008f3a0: 733d 2270 223e 2c3c 2f73 7061 6e3e 203c  s="p">,</span> <
-0008f3b0: 7370 616e 2063 6c61 7373 3d22 6e22 3e6b  span class="n">k
-0008f3c0: 3c2f 7370 616e 3e3c 7370 616e 2063 6c61  </span><span cla
-0008f3d0: 7373 3d22 7022 3e2c 3c2f 7370 616e 3e20  ss="p">,</span> 
-0008f3e0: 3c73 7061 6e20 636c 6173 733d 226e 223e  <span class="n">
-0008f3f0: 6466 3c2f 7370 616e 3e3c 7370 616e 2063  df</span><span c
-0008f400: 6c61 7373 3d22 7022 3e2c 3c2f 7370 616e  lass="p">,</span
-0008f410: 3e20 3c73 7061 6e20 636c 6173 733d 226e  > <span class="n
-0008f420: 223e 7261 6e64 6f6d 5f6e 756d 3c2f 7370  ">random_num</sp
-0008f430: 616e 3e3c 7370 616e 2063 6c61 7373 3d22  an><span class="
-0008f440: 6f22 3e3d 3c2f 7370 616e 3e3c 7370 616e  o">=</span><span
-0008f450: 2063 6c61 7373 3d22 6d69 223e 313c 2f73   class="mi">1</s
-0008f460: 7061 6e3e 3c73 7061 6e20 636c 6173 733d  pan><span class=
-0008f470: 2270 223e 2c3c 2f73 7061 6e3e 203c 7370  "p">,</span> <sp
-0008f480: 616e 2063 6c61 7373 3d22 6e22 3e63 6c61  an class="n">cla
-0008f490: 7373 5f63 6f6c 3c2f 7370 616e 3e3c 7370  ss_col</span><sp
-0008f4a0: 616e 2063 6c61 7373 3d22 6f22 3e3d 3c2f  an class="o">=</
-0008f4b0: 7370 616e 3e3c 7370 616e 2063 6c61 7373  span><span class
-0008f4c0: 3d22 7331 223e 2623 3339 3b6c 6162 656c  ="s1">&#39;label
-0008f4d0: 2623 3339 3b3c 2f73 7061 6e3e 3c73 7061  &#39;</span><spa
-0008f4e0: 6e20 636c 6173 733d 2270 223e 293c 2f73  n class="p">)</s
-0008f4f0: 7061 6e3e 0a3c 2f70 7265 3e3c 2f64 6976  pan>.</pre></div
-0008f500: 3e0a 0a20 2020 2020 3c2f 6469 763e 0a3c  >..     </div>.<
-0008f510: 2f64 6976 3e0a 3c2f 6469 763e 0a3c 2f64  /div>.</div>.</d
-0008f520: 6976 3e0a 0a3c 6469 7620 636c 6173 733d  iv>..<div class=
-0008f530: 226a 702d 4365 6c6c 2d6f 7574 7075 7457  "jp-Cell-outputW
-0008f540: 7261 7070 6572 223e 0a3c 6469 7620 636c  rapper">.<div cl
-0008f550: 6173 733d 226a 702d 436f 6c6c 6170 7365  ass="jp-Collapse
-0008f560: 7220 6a70 2d4f 7574 7075 7443 6f6c 6c61  r jp-OutputColla
-0008f570: 7073 6572 206a 702d 4365 6c6c 2d6f 7574  pser jp-Cell-out
-0008f580: 7075 7443 6f6c 6c61 7073 6572 223e 0a3c  putCollapser">.<
-0008f590: 2f64 6976 3e0a 0a0a 3c64 6976 2063 6c61  /div>...<div cla
-0008f5a0: 7373 3d22 6a70 2d4f 7574 7075 7441 7265  ss="jp-OutputAre
-0008f5b0: 6120 6a70 2d43 656c 6c2d 6f75 7470 7574  a jp-Cell-output
-0008f5c0: 4172 6561 223e 0a0a 3c64 6976 2063 6c61  Area">..<div cla
-0008f5d0: 7373 3d22 6a70 2d4f 7574 7075 7441 7265  ss="jp-OutputAre
-0008f5e0: 612d 6368 696c 6422 3e0a 0a20 2020 200a  a-child">..    .
-0008f5f0: 2020 2020 3c64 6976 2063 6c61 7373 3d22      <div class="
-0008f600: 6a70 2d4f 7574 7075 7450 726f 6d70 7420  jp-OutputPrompt 
-0008f610: 6a70 2d4f 7574 7075 7441 7265 612d 7072  jp-OutputArea-pr
-0008f620: 6f6d 7074 223e 3c2f 6469 763e 0a0a 0a3c  ompt"></div>...<
-0008f630: 6469 7620 636c 6173 733d 226a 702d 5265  div class="jp-Re
-0008f640: 6e64 6572 6564 5465 7874 206a 702d 4f75  nderedText jp-Ou
-0008f650: 7470 7574 4172 6561 2d6f 7574 7075 7422  tputArea-output"
-0008f660: 2064 6174 612d 6d69 6d65 2d74 7970 653d   data-mime-type=
-0008f670: 2274 6578 742f 706c 6169 6e22 3e0a 3c70  "text/plain">.<p
-0008f680: 7265 3e33 2d66 6f6c 6420 7472 6169 6e20  re>3-fold train 
-0008f690: 616e 6420 7465 7374 2073 706c 6974 2069  and test split i
-0008f6a0: 6e2e 2e2e 2061 7574 6f6d 6174 697a 652f  n... automatize/
-0008f6b0: 6173 7365 7473 2f65 7861 6d70 6c65 732f  assets/examples/
-0008f6c0: 4578 616d 706c 652f 6461 7461 0a3c 2f70  Example/data.</p
-0008f6d0: 7265 3e0a 3c2f 6469 763e 0a3c 2f64 6976  re>.</div>.</div
-0008f6e0: 3e0a 0a3c 6469 7620 636c 6173 733d 226a  >..<div class="j
-0008f6f0: 702d 4f75 7470 7574 4172 6561 2d63 6869  p-OutputArea-chi
-0008f700: 6c64 223e 0a0a 2020 2020 0a20 2020 203c  ld">..    .    <
-0008f710: 6469 7620 636c 6173 733d 226a 702d 4f75  div class="jp-Ou
-0008f720: 7470 7574 5072 6f6d 7074 206a 702d 4f75  tputPrompt jp-Ou
-0008f730: 7470 7574 4172 6561 2d70 726f 6d70 7422  tputArea-prompt"
-0008f740: 3e3c 2f64 6976 3e0a 0a0a 0a0a 3c64 6976  ></div>.....<div
-0008f750: 2063 6c61 7373 3d22 6a70 2d52 656e 6465   class="jp-Rende
-0008f760: 7265 6454 6578 7420 6a70 2d4f 7574 7075  redText jp-Outpu
-0008f770: 7441 7265 612d 6f75 7470 7574 2022 2064  tArea-output " d
-0008f780: 6174 612d 6d69 6d65 2d74 7970 653d 2274  ata-mime-type="t
-0008f790: 6578 742f 706c 6169 6e22 3e0a 3c70 7265  ext/plain">.<pre
-0008f7a0: 3e53 706c 6974 696e 6720 4461 7461 3a20  >Spliting Data: 
-0008f7b0: 2020 3025 7c20 2020 2020 2020 2020 207c    0%|          |
-0008f7c0: 2030 2f32 205b 3030 3a30 3026 6c74 3b3f   0/2 [00:00&lt;?
-0008f7d0: 2c20 3f69 742f 735d 3c2f 7072 653e 0a3c  , ?it/s]</pre>.<
-0008f7e0: 2f64 6976 3e0a 0a3c 2f64 6976 3e0a 0a3c  /div>..</div>..<
-0008f7f0: 6469 7620 636c 6173 733d 226a 702d 4f75  div class="jp-Ou
-0008f800: 7470 7574 4172 6561 2d63 6869 6c64 223e  tputArea-child">
-0008f810: 0a0a 2020 2020 0a20 2020 203c 6469 7620  ..    .    <div 
-0008f820: 636c 6173 733d 226a 702d 4f75 7470 7574  class="jp-Output
-0008f830: 5072 6f6d 7074 206a 702d 4f75 7470 7574  Prompt jp-Output
-0008f840: 4172 6561 2d70 726f 6d70 7422 3e3c 2f64  Area-prompt"></d
-0008f850: 6976 3e0a 0a0a 3c64 6976 2063 6c61 7373  iv>...<div class
-0008f860: 3d22 6a70 2d52 656e 6465 7265 6454 6578  ="jp-RenderedTex
-0008f870: 7420 6a70 2d4f 7574 7075 7441 7265 612d  t jp-OutputArea-
-0008f880: 6f75 7470 7574 2220 6461 7461 2d6d 696d  output" data-mim
-0008f890: 652d 7479 7065 3d22 7465 7874 2f70 6c61  e-type="text/pla
-0008f8a0: 696e 223e 0a3c 7072 653e 446f 6e65 2e0a  in">.<pre>Done..
-0008f8b0: 5772 6974 696e 6720 6669 6c65 7320 2e2e  Writing files ..
-0008f8c0: 2e20 312f 330a 3c2f 7072 653e 0a3c 2f64  . 1/3.</pre>.</d
-0008f8d0: 6976 3e0a 3c2f 6469 763e 0a0a 3c64 6976  iv>.</div>..<div
-0008f8e0: 2063 6c61 7373 3d22 6a70 2d4f 7574 7075   class="jp-Outpu
-0008f8f0: 7441 7265 612d 6368 696c 6422 3e0a 0a20  tArea-child">.. 
-0008f900: 2020 200a 2020 2020 3c64 6976 2063 6c61     .    <div cla
-0008f910: 7373 3d22 6a70 2d4f 7574 7075 7450 726f  ss="jp-OutputPro
-0008f920: 6d70 7420 6a70 2d4f 7574 7075 7441 7265  mpt jp-OutputAre
-0008f930: 612d 7072 6f6d 7074 223e 3c2f 6469 763e  a-prompt"></div>
-0008f940: 0a0a 0a0a 0a3c 6469 7620 636c 6173 733d  .....<div class=
-0008f950: 226a 702d 5265 6e64 6572 6564 5465 7874  "jp-RenderedText
-0008f960: 206a 702d 4f75 7470 7574 4172 6561 2d6f   jp-OutputArea-o
-0008f970: 7574 7075 7420 2220 6461 7461 2d6d 696d  utput " data-mim
-0008f980: 652d 7479 7065 3d22 7465 7874 2f70 6c61  e-type="text/pla
-0008f990: 696e 223e 0a3c 7072 653e 5772 6974 696e  in">.<pre>Writin
-0008f9a0: 6720 5452 4149 4e20 2d20 5a49 507c 313a  g TRAIN - ZIP|1:
-0008f9b0: 2020 2030 257c 2020 2020 2020 2020 2020     0%|          
-0008f9c0: 7c20 302f 3720 5b30 303a 3030 266c 743b  | 0/7 [00:00&lt;
-0008f9d0: 3f2c 203f 6974 2f73 5d3c 2f70 7265 3e0a  ?, ?it/s]</pre>.
-0008f9e0: 3c2f 6469 763e 0a0a 3c2f 6469 763e 0a0a  </div>..</div>..
-0008f9f0: 3c64 6976 2063 6c61 7373 3d22 6a70 2d4f  <div class="jp-O
-0008fa00: 7574 7075 7441 7265 612d 6368 696c 6422  utputArea-child"
-0008fa10: 3e0a 0a20 2020 200a 2020 2020 3c64 6976  >..    .    <div
-0008fa20: 2063 6c61 7373 3d22 6a70 2d4f 7574 7075   class="jp-Outpu
-0008fa30: 7450 726f 6d70 7420 6a70 2d4f 7574 7075  tPrompt jp-Outpu
-0008fa40: 7441 7265 612d 7072 6f6d 7074 223e 3c2f  tArea-prompt"></
-0008fa50: 6469 763e 0a0a 0a0a 0a3c 6469 7620 636c  div>.....<div cl
-0008fa60: 6173 733d 226a 702d 5265 6e64 6572 6564  ass="jp-Rendered
-0008fa70: 5465 7874 206a 702d 4f75 7470 7574 4172  Text jp-OutputAr
-0008fa80: 6561 2d6f 7574 7075 7420 2220 6461 7461  ea-output " data
-0008fa90: 2d6d 696d 652d 7479 7065 3d22 7465 7874  -mime-type="text
-0008faa0: 2f70 6c61 696e 223e 0a3c 7072 653e 5772  /plain">.<pre>Wr
-0008fab0: 6974 696e 6720 5445 5354 2020 2d20 5a49  iting TEST  - ZI
-0008fac0: 507c 313a 2020 2030 257c 2020 2020 2020  P|1:   0%|      
-0008fad0: 2020 2020 7c20 302f 3420 5b30 303a 3030      | 0/4 [00:00
-0008fae0: 266c 743b 3f2c 203f 6974 2f73 5d3c 2f70  &lt;?, ?it/s]</p
-0008faf0: 7265 3e0a 3c2f 6469 763e 0a0a 3c2f 6469  re>.</div>..</di
-0008fb00: 763e 0a0a 3c64 6976 2063 6c61 7373 3d22  v>..<div class="
-0008fb10: 6a70 2d4f 7574 7075 7441 7265 612d 6368  jp-OutputArea-ch
-0008fb20: 696c 6422 3e0a 0a20 2020 200a 2020 2020  ild">..    .    
-0008fb30: 3c64 6976 2063 6c61 7373 3d22 6a70 2d4f  <div class="jp-O
-0008fb40: 7574 7075 7450 726f 6d70 7420 6a70 2d4f  utputPrompt jp-O
-0008fb50: 7574 7075 7441 7265 612d 7072 6f6d 7074  utputArea-prompt
-0008fb60: 223e 3c2f 6469 763e 0a0a 0a3c 6469 7620  "></div>...<div 
-0008fb70: 636c 6173 733d 226a 702d 5265 6e64 6572  class="jp-Render
-0008fb80: 6564 5465 7874 206a 702d 4f75 7470 7574  edText jp-Output
-0008fb90: 4172 6561 2d6f 7574 7075 7422 2064 6174  Area-output" dat
-0008fba0: 612d 6d69 6d65 2d74 7970 653d 2274 6578  a-mime-type="tex
-0008fbb0: 742f 706c 6169 6e22 3e0a 3c70 7265 3e57  t/plain">.<pre>W
-0008fbc0: 7269 7469 6e67 2054 5241 494e 202f 2054  riting TRAIN / T
-0008fbd0: 4553 5420 2d20 4353 567c 310a 3c2f 7072  EST - CSV|1.</pr
-0008fbe0: 653e 0a3c 2f64 6976 3e0a 3c2f 6469 763e  e>.</div>.</div>
-0008fbf0: 0a0a 3c64 6976 2063 6c61 7373 3d22 6a70  ..<div class="jp
-0008fc00: 2d4f 7574 7075 7441 7265 612d 6368 696c  -OutputArea-chil
-0008fc10: 6422 3e0a 0a20 2020 200a 2020 2020 3c64  d">..    .    <d
-0008fc20: 6976 2063 6c61 7373 3d22 6a70 2d4f 7574  iv class="jp-Out
-0008fc30: 7075 7450 726f 6d70 7420 6a70 2d4f 7574  putPrompt jp-Out
-0008fc40: 7075 7441 7265 612d 7072 6f6d 7074 223e  putArea-prompt">
-0008fc50: 3c2f 6469 763e 0a0a 0a0a 0a3c 6469 7620  </div>.....<div 
-0008fc60: 636c 6173 733d 226a 702d 5265 6e64 6572  class="jp-Render
-0008fc70: 6564 5465 7874 206a 702d 4f75 7470 7574  edText jp-Output
-0008fc80: 4172 6561 2d6f 7574 7075 7420 2220 6461  Area-output " da
-0008fc90: 7461 2d6d 696d 652d 7479 7065 3d22 7465  ta-mime-type="te
-0008fca0: 7874 2f70 6c61 696e 223e 0a3c 7072 653e  xt/plain">.<pre>
-0008fcb0: 5772 6974 696e 6720 5452 4149 4e20 2d20  Writing TRAIN - 
-0008fcc0: 4d41 547c 313a 2020 2030 257c 2020 2020  MAT|1:   0%|    
-0008fcd0: 2020 2020 2020 7c20 302f 3720 5b30 303a        | 0/7 [00:
-0008fce0: 3030 266c 743b 3f2c 203f 6974 2f73 5d3c  00&lt;?, ?it/s]<
-0008fcf0: 2f70 7265 3e0a 3c2f 6469 763e 0a0a 3c2f  /pre>.</div>..</
-0008fd00: 6469 763e 0a0a 3c64 6976 2063 6c61 7373  div>..<div class
-0008fd10: 3d22 6a70 2d4f 7574 7075 7441 7265 612d  ="jp-OutputArea-
-0008fd20: 6368 696c 6422 3e0a 0a20 2020 200a 2020  child">..    .  
-0008fd30: 2020 3c64 6976 2063 6c61 7373 3d22 6a70    <div class="jp
-0008fd40: 2d4f 7574 7075 7450 726f 6d70 7420 6a70  -OutputPrompt jp
-0008fd50: 2d4f 7574 7075 7441 7265 612d 7072 6f6d  -OutputArea-prom
-0008fd60: 7074 223e 3c2f 6469 763e 0a0a 0a0a 0a3c  pt"></div>.....<
-0008fd70: 6469 7620 636c 6173 733d 226a 702d 5265  div class="jp-Re
-0008fd80: 6e64 6572 6564 5465 7874 206a 702d 4f75  nderedText jp-Ou
-0008fd90: 7470 7574 4172 6561 2d6f 7574 7075 7420  tputArea-output 
-0008fda0: 2220 6461 7461 2d6d 696d 652d 7479 7065  " data-mime-type
-0008fdb0: 3d22 7465 7874 2f70 6c61 696e 223e 0a3c  ="text/plain">.<
-0008fdc0: 7072 653e 5772 6974 696e 6720 5445 5354  pre>Writing TEST
-0008fdd0: 2020 2d20 4d41 547c 313a 2020 2030 257c    - MAT|1:   0%|
-0008fde0: 2020 2020 2020 2020 2020 7c20 302f 3420            | 0/4 
-0008fdf0: 5b30 303a 3030 266c 743b 3f2c 203f 6974  [00:00&lt;?, ?it
-0008fe00: 2f73 5d3c 2f70 7265 3e0a 3c2f 6469 763e  /s]</pre>.</div>
-0008fe10: 0a0a 3c2f 6469 763e 0a0a 3c64 6976 2063  ..</div>..<div c
-0008fe20: 6c61 7373 3d22 6a70 2d4f 7574 7075 7441  lass="jp-OutputA
-0008fe30: 7265 612d 6368 696c 6422 3e0a 0a20 2020  rea-child">..   
-0008fe40: 200a 2020 2020 3c64 6976 2063 6c61 7373   .    <div class
-0008fe50: 3d22 6a70 2d4f 7574 7075 7450 726f 6d70  ="jp-OutputPromp
-0008fe60: 7420 6a70 2d4f 7574 7075 7441 7265 612d  t jp-OutputArea-
-0008fe70: 7072 6f6d 7074 223e 3c2f 6469 763e 0a0a  prompt"></div>..
-0008fe80: 0a3c 6469 7620 636c 6173 733d 226a 702d  .<div class="jp-
-0008fe90: 5265 6e64 6572 6564 5465 7874 206a 702d  RenderedText jp-
-0008fea0: 4f75 7470 7574 4172 6561 2d6f 7574 7075  OutputArea-outpu
-0008feb0: 7422 2064 6174 612d 6d69 6d65 2d74 7970  t" data-mime-typ
-0008fec0: 653d 2274 6578 742f 706c 6169 6e22 3e0a  e="text/plain">.
-0008fed0: 3c70 7265 3e57 7269 7469 6e67 2066 696c  <pre>Writing fil
-0008fee0: 6573 202e 2e2e 2032 2f33 0a3c 2f70 7265  es ... 2/3.</pre
-0008fef0: 3e0a 3c2f 6469 763e 0a3c 2f64 6976 3e0a  >.</div>.</div>.
-0008ff00: 0a3c 6469 7620 636c 6173 733d 226a 702d  .<div class="jp-
-0008ff10: 4f75 7470 7574 4172 6561 2d63 6869 6c64  OutputArea-child
-0008ff20: 223e 0a0a 2020 2020 0a20 2020 203c 6469  ">..    .    <di
-0008ff30: 7620 636c 6173 733d 226a 702d 4f75 7470  v class="jp-Outp
-0008ff40: 7574 5072 6f6d 7074 206a 702d 4f75 7470  utPrompt jp-Outp
-0008ff50: 7574 4172 6561 2d70 726f 6d70 7422 3e3c  utArea-prompt"><
-0008ff60: 2f64 6976 3e0a 0a0a 0a0a 3c64 6976 2063  /div>.....<div c
-0008ff70: 6c61 7373 3d22 6a70 2d52 656e 6465 7265  lass="jp-Rendere
-0008ff80: 6454 6578 7420 6a70 2d4f 7574 7075 7441  dText jp-OutputA
-0008ff90: 7265 612d 6f75 7470 7574 2022 2064 6174  rea-output " dat
-0008ffa0: 612d 6d69 6d65 2d74 7970 653d 2274 6578  a-mime-type="tex
-0008ffb0: 742f 706c 6169 6e22 3e0a 3c70 7265 3e57  t/plain">.<pre>W
-0008ffc0: 7269 7469 6e67 2054 5241 494e 202d 205a  riting TRAIN - Z
-0008ffd0: 4950 7c32 3a20 2020 3025 7c20 2020 2020  IP|2:   0%|     
-0008ffe0: 2020 2020 207c 2030 2f37 205b 3030 3a30       | 0/7 [00:0
-0008fff0: 3026 6c74 3b3f 2c20 3f69 742f 735d 3c2f  0&lt;?, ?it/s]</
-00090000: 7072 653e 0a3c 2f64 6976 3e0a 0a3c 2f64  pre>.</div>..</d
-00090010: 6976 3e0a 0a3c 6469 7620 636c 6173 733d  iv>..<div class=
-00090020: 226a 702d 4f75 7470 7574 4172 6561 2d63  "jp-OutputArea-c
-00090030: 6869 6c64 223e 0a0a 2020 2020 0a20 2020  hild">..    .   
-00090040: 203c 6469 7620 636c 6173 733d 226a 702d   <div class="jp-
-00090050: 4f75 7470 7574 5072 6f6d 7074 206a 702d  OutputPrompt jp-
-00090060: 4f75 7470 7574 4172 6561 2d70 726f 6d70  OutputArea-promp
-00090070: 7422 3e3c 2f64 6976 3e0a 0a0a 0a0a 3c64  t"></div>.....<d
-00090080: 6976 2063 6c61 7373 3d22 6a70 2d52 656e  iv class="jp-Ren
-00090090: 6465 7265 6454 6578 7420 6a70 2d4f 7574  deredText jp-Out
-000900a0: 7075 7441 7265 612d 6f75 7470 7574 2022  putArea-output "
-000900b0: 2064 6174 612d 6d69 6d65 2d74 7970 653d   data-mime-type=
-000900c0: 2274 6578 742f 706c 6169 6e22 3e0a 3c70  "text/plain">.<p
-000900d0: 7265 3e57 7269 7469 6e67 2054 4553 5420  re>Writing TEST 
-000900e0: 202d 205a 4950 7c32 3a20 2020 3025 7c20   - ZIP|2:   0%| 
-000900f0: 2020 2020 2020 2020 207c 2030 2f34 205b           | 0/4 [
-00090100: 3030 3a30 3026 6c74 3b3f 2c20 3f69 742f  00:00&lt;?, ?it/
-00090110: 735d 3c2f 7072 653e 0a3c 2f64 6976 3e0a  s]</pre>.</div>.
-00090120: 0a3c 2f64 6976 3e0a 0a3c 6469 7620 636c  .</div>..<div cl
-00090130: 6173 733d 226a 702d 4f75 7470 7574 4172  ass="jp-OutputAr
-00090140: 6561 2d63 6869 6c64 223e 0a0a 2020 2020  ea-child">..    
-00090150: 0a20 2020 203c 6469 7620 636c 6173 733d  .    <div class=
-00090160: 226a 702d 4f75 7470 7574 5072 6f6d 7074  "jp-OutputPrompt
-00090170: 206a 702d 4f75 7470 7574 4172 6561 2d70   jp-OutputArea-p
-00090180: 726f 6d70 7422 3e3c 2f64 6976 3e0a 0a0a  rompt"></div>...
-00090190: 3c64 6976 2063 6c61 7373 3d22 6a70 2d52  <div class="jp-R
-000901a0: 656e 6465 7265 6454 6578 7420 6a70 2d4f  enderedText jp-O
-000901b0: 7574 7075 7441 7265 612d 6f75 7470 7574  utputArea-output
-000901c0: 2220 6461 7461 2d6d 696d 652d 7479 7065  " data-mime-type
-000901d0: 3d22 7465 7874 2f70 6c61 696e 223e 0a3c  ="text/plain">.<
-000901e0: 7072 653e 5772 6974 696e 6720 5452 4149  pre>Writing TRAI
-000901f0: 4e20 2f20 5445 5354 202d 2043 5356 7c32  N / TEST - CSV|2
-00090200: 0a3c 2f70 7265 3e0a 3c2f 6469 763e 0a3c  .</pre>.</div>.<
-00090210: 2f64 6976 3e0a 0a3c 6469 7620 636c 6173  /div>..<div clas
-00090220: 733d 226a 702d 4f75 7470 7574 4172 6561  s="jp-OutputArea
-00090230: 2d63 6869 6c64 223e 0a0a 2020 2020 0a20  -child">..    . 
-00090240: 2020 203c 6469 7620 636c 6173 733d 226a     <div class="j
-00090250: 702d 4f75 7470 7574 5072 6f6d 7074 206a  p-OutputPrompt j
-00090260: 702d 4f75 7470 7574 4172 6561 2d70 726f  p-OutputArea-pro
-00090270: 6d70 7422 3e3c 2f64 6976 3e0a 0a0a 0a0a  mpt"></div>.....
-00090280: 3c64 6976 2063 6c61 7373 3d22 6a70 2d52  <div class="jp-R
-00090290: 656e 6465 7265 6454 6578 7420 6a70 2d4f  enderedText jp-O
-000902a0: 7574 7075 7441 7265 612d 6f75 7470 7574  utputArea-output
-000902b0: 2022 2064 6174 612d 6d69 6d65 2d74 7970   " data-mime-typ
-000902c0: 653d 2274 6578 742f 706c 6169 6e22 3e0a  e="text/plain">.
-000902d0: 3c70 7265 3e57 7269 7469 6e67 2054 5241  <pre>Writing TRA
-000902e0: 494e 202d 204d 4154 7c32 3a20 2020 3025  IN - MAT|2:   0%
-000902f0: 7c20 2020 2020 2020 2020 207c 2030 2f37  |          | 0/7
-00090300: 205b 3030 3a30 3026 6c74 3b3f 2c20 3f69   [00:00&lt;?, ?i
-00090310: 742f 735d 3c2f 7072 653e 0a3c 2f64 6976  t/s]</pre>.</div
-00090320: 3e0a 0a3c 2f64 6976 3e0a 0a3c 6469 7620  >..</div>..<div 
-00090330: 636c 6173 733d 226a 702d 4f75 7470 7574  class="jp-Output
-00090340: 4172 6561 2d63 6869 6c64 223e 0a0a 2020  Area-child">..  
-00090350: 2020 0a20 2020 203c 6469 7620 636c 6173    .    <div clas
-00090360: 733d 226a 702d 4f75 7470 7574 5072 6f6d  s="jp-OutputProm
-00090370: 7074 206a 702d 4f75 7470 7574 4172 6561  pt jp-OutputArea
-00090380: 2d70 726f 6d70 7422 3e3c 2f64 6976 3e0a  -prompt"></div>.
-00090390: 0a0a 0a0a 3c64 6976 2063 6c61 7373 3d22  ....<div class="
-000903a0: 6a70 2d52 656e 6465 7265 6454 6578 7420  jp-RenderedText 
-000903b0: 6a70 2d4f 7574 7075 7441 7265 612d 6f75  jp-OutputArea-ou
-000903c0: 7470 7574 2022 2064 6174 612d 6d69 6d65  tput " data-mime
-000903d0: 2d74 7970 653d 2274 6578 742f 706c 6169  -type="text/plai
-000903e0: 6e22 3e0a 3c70 7265 3e57 7269 7469 6e67  n">.<pre>Writing
-000903f0: 2054 4553 5420 202d 204d 4154 7c32 3a20   TEST  - MAT|2: 
-00090400: 2020 3025 7c20 2020 2020 2020 2020 207c    0%|          |
-00090410: 2030 2f34 205b 3030 3a30 3026 6c74 3b3f   0/4 [00:00&lt;?
-00090420: 2c20 3f69 742f 735d 3c2f 7072 653e 0a3c  , ?it/s]</pre>.<
-00090430: 2f64 6976 3e0a 0a3c 2f64 6976 3e0a 0a3c  /div>..</div>..<
-00090440: 6469 7620 636c 6173 733d 226a 702d 4f75  div class="jp-Ou
-00090450: 7470 7574 4172 6561 2d63 6869 6c64 223e  tputArea-child">
-00090460: 0a0a 2020 2020 0a20 2020 203c 6469 7620  ..    .    <div 
-00090470: 636c 6173 733d 226a 702d 4f75 7470 7574  class="jp-Output
-00090480: 5072 6f6d 7074 206a 702d 4f75 7470 7574  Prompt jp-Output
-00090490: 4172 6561 2d70 726f 6d70 7422 3e3c 2f64  Area-prompt"></d
-000904a0: 6976 3e0a 0a0a 3c64 6976 2063 6c61 7373  iv>...<div class
-000904b0: 3d22 6a70 2d52 656e 6465 7265 6454 6578  ="jp-RenderedTex
-000904c0: 7420 6a70 2d4f 7574 7075 7441 7265 612d  t jp-OutputArea-
-000904d0: 6f75 7470 7574 2220 6461 7461 2d6d 696d  output" data-mim
-000904e0: 652d 7479 7065 3d22 7465 7874 2f70 6c61  e-type="text/pla
-000904f0: 696e 223e 0a3c 7072 653e 5772 6974 696e  in">.<pre>Writin
-00090500: 6720 6669 6c65 7320 2e2e 2e20 332f 330a  g files ... 3/3.
-00090510: 3c2f 7072 653e 0a3c 2f64 6976 3e0a 3c2f  </pre>.</div>.</
-00090520: 6469 763e 0a0a 3c64 6976 2063 6c61 7373  div>..<div class
-00090530: 3d22 6a70 2d4f 7574 7075 7441 7265 612d  ="jp-OutputArea-
-00090540: 6368 696c 6422 3e0a 0a20 2020 200a 2020  child">..    .  
-00090550: 2020 3c64 6976 2063 6c61 7373 3d22 6a70    <div class="jp
-00090560: 2d4f 7574 7075 7450 726f 6d70 7420 6a70  -OutputPrompt jp
-00090570: 2d4f 7574 7075 7441 7265 612d 7072 6f6d  -OutputArea-prom
-00090580: 7074 223e 3c2f 6469 763e 0a0a 0a0a 0a3c  pt"></div>.....<
-00090590: 6469 7620 636c 6173 733d 226a 702d 5265  div class="jp-Re
-000905a0: 6e64 6572 6564 5465 7874 206a 702d 4f75  nderedText jp-Ou
-000905b0: 7470 7574 4172 6561 2d6f 7574 7075 7420  tputArea-output 
-000905c0: 2220 6461 7461 2d6d 696d 652d 7479 7065  " data-mime-type
-000905d0: 3d22 7465 7874 2f70 6c61 696e 223e 0a3c  ="text/plain">.<
-000905e0: 7072 653e 5772 6974 696e 6720 5452 4149  pre>Writing TRAI
-000905f0: 4e20 2d20 5a49 507c 333a 2020 2030 257c  N - ZIP|3:   0%|
-00090600: 2020 2020 2020 2020 2020 7c20 302f 3820            | 0/8 
-00090610: 5b30 303a 3030 266c 743b 3f2c 203f 6974  [00:00&lt;?, ?it
-00090620: 2f73 5d3c 2f70 7265 3e0a 3c2f 6469 763e  /s]</pre>.</div>
-00090630: 0a0a 3c2f 6469 763e 0a0a 3c64 6976 2063  ..</div>..<div c
-00090640: 6c61 7373 3d22 6a70 2d4f 7574 7075 7441  lass="jp-OutputA
-00090650: 7265 612d 6368 696c 6422 3e0a 0a20 2020  rea-child">..   
-00090660: 200a 2020 2020 3c64 6976 2063 6c61 7373   .    <div class
-00090670: 3d22 6a70 2d4f 7574 7075 7450 726f 6d70  ="jp-OutputPromp
-00090680: 7420 6a70 2d4f 7574 7075 7441 7265 612d  t jp-OutputArea-
-00090690: 7072 6f6d 7074 223e 3c2f 6469 763e 0a0a  prompt"></div>..
-000906a0: 0a0a 0a3c 6469 7620 636c 6173 733d 226a  ...<div class="j
-000906b0: 702d 5265 6e64 6572 6564 5465 7874 206a  p-RenderedText j
-000906c0: 702d 4f75 7470 7574 4172 6561 2d6f 7574  p-OutputArea-out
-000906d0: 7075 7420 2220 6461 7461 2d6d 696d 652d  put " data-mime-
-000906e0: 7479 7065 3d22 7465 7874 2f70 6c61 696e  type="text/plain
-000906f0: 223e 0a3c 7072 653e 5772 6974 696e 6720  ">.<pre>Writing 
-00090700: 5445 5354 2020 2d20 5a49 507c 333a 2020  TEST  - ZIP|3:  
-00090710: 2030 257c 2020 2020 2020 2020 2020 7c20   0%|          | 
-00090720: 302f 3320 5b30 303a 3030 266c 743b 3f2c  0/3 [00:00&lt;?,
-00090730: 203f 6974 2f73 5d3c 2f70 7265 3e0a 3c2f   ?it/s]</pre>.</
-00090740: 6469 763e 0a0a 3c2f 6469 763e 0a0a 3c64  div>..</div>..<d
-00090750: 6976 2063 6c61 7373 3d22 6a70 2d4f 7574  iv class="jp-Out
-00090760: 7075 7441 7265 612d 6368 696c 6422 3e0a  putArea-child">.
-00090770: 0a20 2020 200a 2020 2020 3c64 6976 2063  .    .    <div c
-00090780: 6c61 7373 3d22 6a70 2d4f 7574 7075 7450  lass="jp-OutputP
-00090790: 726f 6d70 7420 6a70 2d4f 7574 7075 7441  rompt jp-OutputA
-000907a0: 7265 612d 7072 6f6d 7074 223e 3c2f 6469  rea-prompt"></di
-000907b0: 763e 0a0a 0a3c 6469 7620 636c 6173 733d  v>...<div class=
-000907c0: 226a 702d 5265 6e64 6572 6564 5465 7874  "jp-RenderedText
-000907d0: 206a 702d 4f75 7470 7574 4172 6561 2d6f   jp-OutputArea-o
-000907e0: 7574 7075 7422 2064 6174 612d 6d69 6d65  utput" data-mime
-000907f0: 2d74 7970 653d 2274 6578 742f 706c 6169  -type="text/plai
-00090800: 6e22 3e0a 3c70 7265 3e57 7269 7469 6e67  n">.<pre>Writing
-00090810: 2054 5241 494e 202f 2054 4553 5420 2d20   TRAIN / TEST - 
-00090820: 4353 567c 330a 3c2f 7072 653e 0a3c 2f64  CSV|3.</pre>.</d
-00090830: 6976 3e0a 3c2f 6469 763e 0a0a 3c64 6976  iv>.</div>..<div
-00090840: 2063 6c61 7373 3d22 6a70 2d4f 7574 7075   class="jp-Outpu
-00090850: 7441 7265 612d 6368 696c 6422 3e0a 0a20  tArea-child">.. 
-00090860: 2020 200a 2020 2020 3c64 6976 2063 6c61     .    <div cla
-00090870: 7373 3d22 6a70 2d4f 7574 7075 7450 726f  ss="jp-OutputPro
-00090880: 6d70 7420 6a70 2d4f 7574 7075 7441 7265  mpt jp-OutputAre
-00090890: 612d 7072 6f6d 7074 223e 3c2f 6469 763e  a-prompt"></div>
-000908a0: 0a0a 0a0a 0a3c 6469 7620 636c 6173 733d  .....<div class=
-000908b0: 226a 702d 5265 6e64 6572 6564 5465 7874  "jp-RenderedText
-000908c0: 206a 702d 4f75 7470 7574 4172 6561 2d6f   jp-OutputArea-o
-000908d0: 7574 7075 7420 2220 6461 7461 2d6d 696d  utput " data-mim
-000908e0: 652d 7479 7065 3d22 7465 7874 2f70 6c61  e-type="text/pla
-000908f0: 696e 223e 0a3c 7072 653e 5772 6974 696e  in">.<pre>Writin
-00090900: 6720 5452 4149 4e20 2d20 4d41 547c 333a  g TRAIN - MAT|3:
-00090910: 2020 2030 257c 2020 2020 2020 2020 2020     0%|          
-00090920: 7c20 302f 3820 5b30 303a 3030 266c 743b  | 0/8 [00:00&lt;
-00090930: 3f2c 203f 6974 2f73 5d3c 2f70 7265 3e0a  ?, ?it/s]</pre>.
-00090940: 3c2f 6469 763e 0a0a 3c2f 6469 763e 0a0a  </div>..</div>..
-00090950: 3c64 6976 2063 6c61 7373 3d22 6a70 2d4f  <div class="jp-O
-00090960: 7574 7075 7441 7265 612d 6368 696c 6422  utputArea-child"
-00090970: 3e0a 0a20 2020 200a 2020 2020 3c64 6976  >..    .    <div
-00090980: 2063 6c61 7373 3d22 6a70 2d4f 7574 7075   class="jp-Outpu
-00090990: 7450 726f 6d70 7420 6a70 2d4f 7574 7075  tPrompt jp-Outpu
-000909a0: 7441 7265 612d 7072 6f6d 7074 223e 3c2f  tArea-prompt"></
-000909b0: 6469 763e 0a0a 0a0a 0a3c 6469 7620 636c  div>.....<div cl
-000909c0: 6173 733d 226a 702d 5265 6e64 6572 6564  ass="jp-Rendered
-000909d0: 5465 7874 206a 702d 4f75 7470 7574 4172  Text jp-OutputAr
-000909e0: 6561 2d6f 7574 7075 7420 2220 6461 7461  ea-output " data
-000909f0: 2d6d 696d 652d 7479 7065 3d22 7465 7874  -mime-type="text
-00090a00: 2f70 6c61 696e 223e 0a3c 7072 653e 5772  /plain">.<pre>Wr
-00090a10: 6974 696e 6720 5445 5354 2020 2d20 4d41  iting TEST  - MA
-00090a20: 547c 333a 2020 2030 257c 2020 2020 2020  T|3:   0%|      
-00090a30: 2020 2020 7c20 302f 3320 5b30 303a 3030      | 0/3 [00:00
-00090a40: 266c 743b 3f2c 203f 6974 2f73 5d3c 2f70  &lt;?, ?it/s]</p
-00090a50: 7265 3e0a 3c2f 6469 763e 0a0a 3c2f 6469  re>.</div>..</di
-00090a60: 763e 0a0a 3c64 6976 2063 6c61 7373 3d22  v>..<div class="
-00090a70: 6a70 2d4f 7574 7075 7441 7265 612d 6368  jp-OutputArea-ch
-00090a80: 696c 6422 3e0a 0a20 2020 200a 2020 2020  ild">..    .    
-00090a90: 3c64 6976 2063 6c61 7373 3d22 6a70 2d4f  <div class="jp-O
-00090aa0: 7574 7075 7450 726f 6d70 7420 6a70 2d4f  utputPrompt jp-O
-00090ab0: 7574 7075 7441 7265 612d 7072 6f6d 7074  utputArea-prompt
-00090ac0: 223e 3c2f 6469 763e 0a0a 0a3c 6469 7620  "></div>...<div 
-00090ad0: 636c 6173 733d 226a 702d 5265 6e64 6572  class="jp-Render
-00090ae0: 6564 5465 7874 206a 702d 4f75 7470 7574  edText jp-Output
-00090af0: 4172 6561 2d6f 7574 7075 7422 2064 6174  Area-output" dat
-00090b00: 612d 6d69 6d65 2d74 7970 653d 2274 6578  a-mime-type="tex
-00090b10: 742f 706c 6169 6e22 3e0a 3c70 7265 3e44  t/plain">.<pre>D
-00090b20: 6f6e 652e 0a20 2d2d 2d2d 2d2d 2d2d 2d2d  one.. ----------
-00090b30: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00090b40: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00090b50: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00090b60: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00090b70: 2d2d 2d2d 2d2d 0a3c 2f70 7265 3e0a 3c2f  ------.</pre>.</
-00090b80: 6469 763e 0a3c 2f64 6976 3e0a 0a3c 2f64  div>.</div>..</d
-00090b90: 6976 3e0a 0a3c 2f64 6976 3e0a 0a3c 2f64  iv>..</div>..</d
-00090ba0: 6976 3e0a 3c64 6976 2063 6c61 7373 3d22  iv>.<div class="
-00090bb0: 6a70 2d43 656c 6c20 6a70 2d4d 6172 6b64  jp-Cell jp-Markd
-00090bc0: 6f77 6e43 656c 6c20 6a70 2d4e 6f74 6562  ownCell jp-Noteb
-00090bd0: 6f6f 6b2d 6365 6c6c 223e 0a3c 6469 7620  ook-cell">.<div 
-00090be0: 636c 6173 733d 226a 702d 4365 6c6c 2d69  class="jp-Cell-i
-00090bf0: 6e70 7574 5772 6170 7065 7222 3e0a 3c64  nputWrapper">.<d
-00090c00: 6976 2063 6c61 7373 3d22 6a70 2d43 6f6c  iv class="jp-Col
-00090c10: 6c61 7073 6572 206a 702d 496e 7075 7443  lapser jp-InputC
-00090c20: 6f6c 6c61 7073 6572 206a 702d 4365 6c6c  ollapser jp-Cell
-00090c30: 2d69 6e70 7574 436f 6c6c 6170 7365 7222  -inputCollapser"
-00090c40: 3e0a 3c2f 6469 763e 0a3c 6469 7620 636c  >.</div>.<div cl
-00090c50: 6173 733d 226a 702d 496e 7075 7441 7265  ass="jp-InputAre
-00090c60: 6120 6a70 2d43 656c 6c2d 696e 7075 7441  a jp-Cell-inputA
-00090c70: 7265 6122 3e3c 6469 7620 636c 6173 733d  rea"><div class=
-00090c80: 226a 702d 496e 7075 7450 726f 6d70 7420  "jp-InputPrompt 
-00090c90: 6a70 2d49 6e70 7574 4172 6561 2d70 726f  jp-InputArea-pro
-00090ca0: 6d70 7422 3e0a 3c2f 6469 763e 3c64 6976  mpt">.</div><div
-00090cb0: 2063 6c61 7373 3d22 6a70 2d52 656e 6465   class="jp-Rende
-00090cc0: 7265 6448 544d 4c43 6f6d 6d6f 6e20 6a70  redHTMLCommon jp
-00090cd0: 2d52 656e 6465 7265 644d 6172 6b64 6f77  -RenderedMarkdow
-00090ce0: 6e20 6a70 2d4d 6172 6b64 6f77 6e4f 7574  n jp-MarkdownOut
-00090cf0: 7075 7420 2220 6461 7461 2d6d 696d 652d  put " data-mime-
-00090d00: 7479 7065 3d22 7465 7874 2f6d 6172 6b64  type="text/markd
-00090d10: 6f77 6e22 3e0a 3c70 3e54 6f20 636f 6e76  own">.<p>To conv
-00090d20: 6572 7420 7472 6169 6e20 616e 6420 7465  ert train and te
-00090d30: 7374 2066 726f 6d20 6f6e 6520 6176 6169  st from one avai
-00090d40: 6c61 626c 6520 666f 726d 6174 2074 6f20  lable format to 
-00090d50: 6f74 6865 7220 6465 6661 756c 7420 666f  other default fo
-00090d60: 726d 6174 7320 2843 5356 2c20 5a49 502c  rmats (CSV, ZIP,
-00090d70: 204d 4154 293a 3c2f 703e 0a0a 3c2f 6469   MAT):</p>..</di
-00090d80: 763e 0a3c 2f64 6976 3e0a 3c2f 6469 763e  v>.</div>.</div>
-00090d90: 0a3c 2f64 6976 3e3c 6469 7620 636c 6173  .</div><div clas
-00090da0: 733d 226a 702d 4365 6c6c 206a 702d 436f  s="jp-Cell jp-Co
-00090db0: 6465 4365 6c6c 206a 702d 4e6f 7465 626f  deCell jp-Notebo
-00090dc0: 6f6b 2d63 656c 6c20 2020 223e 0a3c 6469  ok-cell   ">.<di
-00090dd0: 7620 636c 6173 733d 226a 702d 4365 6c6c  v class="jp-Cell
-00090de0: 2d69 6e70 7574 5772 6170 7065 7222 3e0a  -inputWrapper">.
-00090df0: 3c64 6976 2063 6c61 7373 3d22 6a70 2d43  <div class="jp-C
-00090e00: 6f6c 6c61 7073 6572 206a 702d 496e 7075  ollapser jp-Inpu
-00090e10: 7443 6f6c 6c61 7073 6572 206a 702d 4365  tCollapser jp-Ce
-00090e20: 6c6c 2d69 6e70 7574 436f 6c6c 6170 7365  ll-inputCollapse
-00090e30: 7222 3e0a 3c2f 6469 763e 0a3c 6469 7620  r">.</div>.<div 
-00090e40: 636c 6173 733d 226a 702d 496e 7075 7441  class="jp-InputA
-00090e50: 7265 6120 6a70 2d43 656c 6c2d 696e 7075  rea jp-Cell-inpu
-00090e60: 7441 7265 6122 3e0a 3c64 6976 2063 6c61  tArea">.<div cla
-00090e70: 7373 3d22 6a70 2d49 6e70 7574 5072 6f6d  ss="jp-InputProm
-00090e80: 7074 206a 702d 496e 7075 7441 7265 612d  pt jp-InputArea-
-00090e90: 7072 6f6d 7074 223e 496e 266e 6273 703b  prompt">In&nbsp;
-00090ea0: 5b34 5d3a 3c2f 6469 763e 0a3c 6469 7620  [4]:</div>.<div 
-00090eb0: 636c 6173 733d 226a 702d 436f 6465 4d69  class="jp-CodeMi
-00090ec0: 7272 6f72 4564 6974 6f72 206a 702d 4564  rrorEditor jp-Ed
-00090ed0: 6974 6f72 206a 702d 496e 7075 7441 7265  itor jp-InputAre
-00090ee0: 612d 6564 6974 6f72 2220 6461 7461 2d74  a-editor" data-t
-00090ef0: 7970 653d 2269 6e6c 696e 6522 3e0a 2020  ype="inline">.  
-00090f00: 2020 203c 6469 7620 636c 6173 733d 2243     <div class="C
-00090f10: 6f64 654d 6972 726f 7220 636d 2d73 2d6a  odeMirror cm-s-j
-00090f20: 7570 7974 6572 223e 0a3c 6469 7620 636c  upyter">.<div cl
-00090f30: 6173 733d 2220 6869 6768 6c69 6768 7420  ass=" highlight 
-00090f40: 686c 2d69 7079 7468 6f6e 3322 3e3c 7072  hl-ipython3"><pr
-00090f50: 653e 3c73 7061 6e3e 3c2f 7370 616e 3e3c  e><span></span><
-00090f60: 7370 616e 2063 6c61 7373 3d22 6e22 3e63  span class="n">c
-00090f70: 6f6e 7665 7274 4461 7461 7365 743c 2f73  onvertDataset</s
-00090f80: 7061 6e3e 3c73 7061 6e20 636c 6173 733d  pan><span class=
-00090f90: 2270 223e 283c 2f73 7061 6e3e 3c73 7061  "p">(</span><spa
-00090fa0: 6e20 636c 6173 733d 226e 223e 6461 7461  n class="n">data
-00090fb0: 5f70 6174 683c 2f73 7061 6e3e 3c73 7061  _path</span><spa
-00090fc0: 6e20 636c 6173 733d 2270 223e 293c 2f73  n class="p">)</s
-00090fd0: 7061 6e3e 0a3c 2f70 7265 3e3c 2f64 6976  pan>.</pre></div
-00090fe0: 3e0a 0a20 2020 2020 3c2f 6469 763e 0a3c  >..     </div>.<
-00090ff0: 2f64 6976 3e0a 3c2f 6469 763e 0a3c 2f64  /div>.</div>.</d
-00091000: 6976 3e0a 0a3c 6469 7620 636c 6173 733d  iv>..<div class=
-00091010: 226a 702d 4365 6c6c 2d6f 7574 7075 7457  "jp-Cell-outputW
-00091020: 7261 7070 6572 223e 0a3c 6469 7620 636c  rapper">.<div cl
-00091030: 6173 733d 226a 702d 436f 6c6c 6170 7365  ass="jp-Collapse
-00091040: 7220 6a70 2d4f 7574 7075 7443 6f6c 6c61  r jp-OutputColla
-00091050: 7073 6572 206a 702d 4365 6c6c 2d6f 7574  pser jp-Cell-out
-00091060: 7075 7443 6f6c 6c61 7073 6572 223e 0a3c  putCollapser">.<
-00091070: 2f64 6976 3e0a 0a0a 3c64 6976 2063 6c61  /div>...<div cla
-00091080: 7373 3d22 6a70 2d4f 7574 7075 7441 7265  ss="jp-OutputAre
-00091090: 6120 6a70 2d43 656c 6c2d 6f75 7470 7574  a jp-Cell-output
-000910a0: 4172 6561 223e 0a0a 3c64 6976 2063 6c61  Area">..<div cla
-000910b0: 7373 3d22 6a70 2d4f 7574 7075 7441 7265  ss="jp-OutputAre
-000910c0: 612d 6368 696c 6422 3e0a 0a20 2020 200a  a-child">..    .
-000910d0: 2020 2020 3c64 6976 2063 6c61 7373 3d22      <div class="
-000910e0: 6a70 2d4f 7574 7075 7450 726f 6d70 7420  jp-OutputPrompt 
-000910f0: 6a70 2d4f 7574 7075 7441 7265 612d 7072  jp-OutputArea-pr
-00091100: 6f6d 7074 223e 3c2f 6469 763e 0a0a 0a0a  ompt"></div>....
-00091110: 0a3c 6469 7620 636c 6173 733d 226a 702d  .<div class="jp-
-00091120: 5265 6e64 6572 6564 5465 7874 206a 702d  RenderedText jp-
-00091130: 4f75 7470 7574 4172 6561 2d6f 7574 7075  OutputArea-outpu
-00091140: 7420 2220 6461 7461 2d6d 696d 652d 7479  t " data-mime-ty
-00091150: 7065 3d22 7465 7874 2f70 6c61 696e 223e  pe="text/plain">
-00091160: 0a3c 7072 653e 5772 6974 696e 6720 5452  .<pre>Writing TR
-00091170: 4149 4e20 2d20 5a49 507c 3a20 2020 3025  AIN - ZIP|:   0%
-00091180: 7c20 2020 2020 2020 2020 207c 2030 2f31  |          | 0/1
-00091190: 3420 5b30 303a 3030 266c 743b 3f2c 203f  4 [00:00&lt;?, ?
-000911a0: 6974 2f73 5d3c 2f70 7265 3e0a 3c2f 6469  it/s]</pre>.</di
-000911b0: 763e 0a0a 3c2f 6469 763e 0a0a 3c64 6976  v>..</div>..<div
-000911c0: 2063 6c61 7373 3d22 6a70 2d4f 7574 7075   class="jp-Outpu
-000911d0: 7441 7265 612d 6368 696c 6422 3e0a 0a20  tArea-child">.. 
-000911e0: 2020 200a 2020 2020 3c64 6976 2063 6c61     .    <div cla
-000911f0: 7373 3d22 6a70 2d4f 7574 7075 7450 726f  ss="jp-OutputPro
-00091200: 6d70 7420 6a70 2d4f 7574 7075 7441 7265  mpt jp-OutputAre
-00091210: 612d 7072 6f6d 7074 223e 3c2f 6469 763e  a-prompt"></div>
-00091220: 0a0a 0a0a 0a3c 6469 7620 636c 6173 733d  .....<div class=
-00091230: 226a 702d 5265 6e64 6572 6564 5465 7874  "jp-RenderedText
-00091240: 206a 702d 4f75 7470 7574 4172 6561 2d6f   jp-OutputArea-o
-00091250: 7574 7075 7420 2220 6461 7461 2d6d 696d  utput " data-mim
-00091260: 652d 7479 7065 3d22 7465 7874 2f70 6c61  e-type="text/pla
-00091270: 696e 223e 0a3c 7072 653e 5772 6974 696e  in">.<pre>Writin
-00091280: 6720 5445 5354 2020 2d20 5a49 507c 3a20  g TEST  - ZIP|: 
-00091290: 2020 3025 7c20 2020 2020 2020 2020 207c    0%|          |
-000912a0: 2030 2f31 3420 5b30 303a 3030 266c 743b   0/14 [00:00&lt;
-000912b0: 3f2c 203f 6974 2f73 5d3c 2f70 7265 3e0a  ?, ?it/s]</pre>.
-000912c0: 3c2f 6469 763e 0a0a 3c2f 6469 763e 0a0a  </div>..</div>..
-000912d0: 3c64 6976 2063 6c61 7373 3d22 6a70 2d4f  <div class="jp-O
-000912e0: 7574 7075 7441 7265 612d 6368 696c 6422  utputArea-child"
-000912f0: 3e0a 0a20 2020 200a 2020 2020 3c64 6976  >..    .    <div
-00091300: 2063 6c61 7373 3d22 6a70 2d4f 7574 7075   class="jp-Outpu
-00091310: 7450 726f 6d70 7420 6a70 2d4f 7574 7075  tPrompt jp-Outpu
-00091320: 7441 7265 612d 7072 6f6d 7074 223e 3c2f  tArea-prompt"></
-00091330: 6469 763e 0a0a 0a0a 0a3c 6469 7620 636c  div>.....<div cl
-00091340: 6173 733d 226a 702d 5265 6e64 6572 6564  ass="jp-Rendered
-00091350: 5465 7874 206a 702d 4f75 7470 7574 4172  Text jp-OutputAr
-00091360: 6561 2d6f 7574 7075 7420 2220 6461 7461  ea-output " data
-00091370: 2d6d 696d 652d 7479 7065 3d22 7465 7874  -mime-type="text
-00091380: 2f70 6c61 696e 223e 0a3c 7072 653e 5772  /plain">.<pre>Wr
-00091390: 6974 696e 6720 5452 4149 4e20 2d20 4d41  iting TRAIN - MA
-000913a0: 547c 3a20 2020 3025 7c20 2020 2020 2020  T|:   0%|       
-000913b0: 2020 207c 2030 2f31 3420 5b30 303a 3030     | 0/14 [00:00
-000913c0: 266c 743b 3f2c 203f 6974 2f73 5d3c 2f70  &lt;?, ?it/s]</p
-000913d0: 7265 3e0a 3c2f 6469 763e 0a0a 3c2f 6469  re>.</div>..</di
-000913e0: 763e 0a0a 3c64 6976 2063 6c61 7373 3d22  v>..<div class="
-000913f0: 6a70 2d4f 7574 7075 7441 7265 612d 6368  jp-OutputArea-ch
-00091400: 696c 6422 3e0a 0a20 2020 200a 2020 2020  ild">..    .    
-00091410: 3c64 6976 2063 6c61 7373 3d22 6a70 2d4f  <div class="jp-O
-00091420: 7574 7075 7450 726f 6d70 7420 6a70 2d4f  utputPrompt jp-O
-00091430: 7574 7075 7441 7265 612d 7072 6f6d 7074  utputArea-prompt
-00091440: 223e 3c2f 6469 763e 0a0a 0a0a 0a3c 6469  "></div>.....<di
-00091450: 7620 636c 6173 733d 226a 702d 5265 6e64  v class="jp-Rend
-00091460: 6572 6564 5465 7874 206a 702d 4f75 7470  eredText jp-Outp
-00091470: 7574 4172 6561 2d6f 7574 7075 7420 2220  utArea-output " 
-00091480: 6461 7461 2d6d 696d 652d 7479 7065 3d22  data-mime-type="
-00091490: 7465 7874 2f70 6c61 696e 223e 0a3c 7072  text/plain">.<pr
-000914a0: 653e 5772 6974 696e 6720 5445 5354 2020  e>Writing TEST  
-000914b0: 2d20 4d41 547c 3a20 2020 3025 7c20 2020  - MAT|:   0%|   
-000914c0: 2020 2020 2020 207c 2030 2f31 3420 5b30         | 0/14 [0
-000914d0: 303a 3030 266c 743b 3f2c 203f 6974 2f73  0:00&lt;?, ?it/s
-000914e0: 5d3c 2f70 7265 3e0a 3c2f 6469 763e 0a0a  ]</pre>.</div>..
-000914f0: 3c2f 6469 763e 0a0a 3c64 6976 2063 6c61  </div>..<div cla
-00091500: 7373 3d22 6a70 2d4f 7574 7075 7441 7265  ss="jp-OutputAre
-00091510: 612d 6368 696c 6422 3e0a 0a20 2020 200a  a-child">..    .
-00091520: 2020 2020 3c64 6976 2063 6c61 7373 3d22      <div class="
-00091530: 6a70 2d4f 7574 7075 7450 726f 6d70 7420  jp-OutputPrompt 
-00091540: 6a70 2d4f 7574 7075 7441 7265 612d 7072  jp-OutputArea-pr
-00091550: 6f6d 7074 223e 3c2f 6469 763e 0a0a 0a3c  ompt"></div>...<
-00091560: 6469 7620 636c 6173 733d 226a 702d 5265  div class="jp-Re
-00091570: 6e64 6572 6564 5465 7874 206a 702d 4f75  nderedText jp-Ou
-00091580: 7470 7574 4172 6561 2d6f 7574 7075 7422  tputArea-output"
-00091590: 2064 6174 612d 6d69 6d65 2d74 7970 653d   data-mime-type=
-000915a0: 2274 6578 742f 706c 6169 6e22 3e0a 3c70  "text/plain">.<p
-000915b0: 7265 3e41 6c6c 2044 6f6e 652e 0a3c 2f70  re>All Done..</p
-000915c0: 7265 3e0a 3c2f 6469 763e 0a3c 2f64 6976  re>.</div>.</div
-000915d0: 3e0a 0a3c 2f64 6976 3e0a 0a3c 2f64 6976  >..</div>..</div
-000915e0: 3e0a 0a3c 2f64 6976 3e0a 3c64 6976 2063  >..</div>.<div c
-000915f0: 6c61 7373 3d22 6a70 2d43 656c 6c20 6a70  lass="jp-Cell jp
-00091600: 2d4d 6172 6b64 6f77 6e43 656c 6c20 6a70  -MarkdownCell jp
-00091610: 2d4e 6f74 6562 6f6f 6b2d 6365 6c6c 223e  -Notebook-cell">
-00091620: 0a3c 6469 7620 636c 6173 733d 226a 702d  .<div class="jp-
-00091630: 4365 6c6c 2d69 6e70 7574 5772 6170 7065  Cell-inputWrappe
-00091640: 7222 3e0a 3c64 6976 2063 6c61 7373 3d22  r">.<div class="
-00091650: 6a70 2d43 6f6c 6c61 7073 6572 206a 702d  jp-Collapser jp-
-00091660: 496e 7075 7443 6f6c 6c61 7073 6572 206a  InputCollapser j
-00091670: 702d 4365 6c6c 2d69 6e70 7574 436f 6c6c  p-Cell-inputColl
-00091680: 6170 7365 7222 3e0a 3c2f 6469 763e 0a3c  apser">.</div>.<
-00091690: 6469 7620 636c 6173 733d 226a 702d 496e  div class="jp-In
-000916a0: 7075 7441 7265 6120 6a70 2d43 656c 6c2d  putArea jp-Cell-
-000916b0: 696e 7075 7441 7265 6122 3e3c 6469 7620  inputArea"><div 
-000916c0: 636c 6173 733d 226a 702d 496e 7075 7450  class="jp-InputP
-000916d0: 726f 6d70 7420 6a70 2d49 6e70 7574 4172  rompt jp-InputAr
-000916e0: 6561 2d70 726f 6d70 7422 3e0a 3c2f 6469  ea-prompt">.</di
-000916f0: 763e 3c64 6976 2063 6c61 7373 3d22 6a70  v><div class="jp
-00091700: 2d52 656e 6465 7265 6448 544d 4c43 6f6d  -RenderedHTMLCom
-00091710: 6d6f 6e20 6a70 2d52 656e 6465 7265 644d  mon jp-RenderedM
-00091720: 6172 6b64 6f77 6e20 6a70 2d4d 6172 6b64  arkdown jp-Markd
-00091730: 6f77 6e4f 7574 7075 7420 2220 6461 7461  ownOutput " data
-00091740: 2d6d 696d 652d 7479 7065 3d22 7465 7874  -mime-type="text
-00091750: 2f6d 6172 6b64 6f77 6e22 3e0a 3c68 3320  /markdown">.<h3 
-00091760: 6964 3d22 322e 2d53 796e 7468 6574 6963  id="2.-Synthetic
-00091770: 2d44 6174 612d 4765 6e65 7261 7469 6f6e  -Data-Generation
-00091780: 223e 322e 2053 796e 7468 6574 6963 2044  ">2. Synthetic D
-00091790: 6174 6120 4765 6e65 7261 7469 6f6e 3c61  ata Generation<a
-000917a0: 2063 6c61 7373 3d22 616e 6368 6f72 2d6c   class="anchor-l
-000917b0: 696e 6b22 2068 7265 663d 2223 322e 2d53  ink" href="#2.-S
-000917c0: 796e 7468 6574 6963 2d44 6174 612d 4765  ynthetic-Data-Ge
-000917d0: 6e65 7261 7469 6f6e 223e 2623 3138 323b  neration">&#182;
-000917e0: 3c2f 613e 3c2f 6833 3e3c 703e 544f 444f  </a></h3><p>TODO
-000917f0: 3c2f 703e 0a0a 3c2f 6469 763e 0a3c 2f64  </p>..</div>.</d
-00091800: 6976 3e0a 3c2f 6469 763e 0a3c 2f64 6976  iv>.</div>.</div
-00091810: 3e3c 6469 7620 636c 6173 733d 226a 702d  ><div class="jp-
-00091820: 4365 6c6c 206a 702d 436f 6465 4365 6c6c  Cell jp-CodeCell
-00091830: 206a 702d 4e6f 7465 626f 6f6b 2d63 656c   jp-Notebook-cel
-00091840: 6c20 6a70 2d6d 6f64 2d6e 6f4f 7574 7075  l jp-mod-noOutpu
-00091850: 7473 2020 223e 0a3c 6469 7620 636c 6173  ts  ">.<div clas
-00091860: 733d 226a 702d 4365 6c6c 2d69 6e70 7574  s="jp-Cell-input
-00091870: 5772 6170 7065 7222 3e0a 3c64 6976 2063  Wrapper">.<div c
-00091880: 6c61 7373 3d22 6a70 2d43 6f6c 6c61 7073  lass="jp-Collaps
-00091890: 6572 206a 702d 496e 7075 7443 6f6c 6c61  er jp-InputColla
-000918a0: 7073 6572 206a 702d 4365 6c6c 2d69 6e70  pser jp-Cell-inp
-000918b0: 7574 436f 6c6c 6170 7365 7222 3e0a 3c2f  utCollapser">.</
-000918c0: 6469 763e 0a3c 6469 7620 636c 6173 733d  div>.<div class=
-000918d0: 226a 702d 496e 7075 7441 7265 6120 6a70  "jp-InputArea jp
-000918e0: 2d43 656c 6c2d 696e 7075 7441 7265 6122  -Cell-inputArea"
-000918f0: 3e0a 3c64 6976 2063 6c61 7373 3d22 6a70  >.<div class="jp
-00091900: 2d49 6e70 7574 5072 6f6d 7074 206a 702d  -InputPrompt jp-
-00091910: 496e 7075 7441 7265 612d 7072 6f6d 7074  InputArea-prompt
-00091920: 223e 496e 266e 6273 703b 5b35 5d3a 3c2f  ">In&nbsp;[5]:</
-00091930: 6469 763e 0a3c 6469 7620 636c 6173 733d  div>.<div class=
-00091940: 226a 702d 436f 6465 4d69 7272 6f72 4564  "jp-CodeMirrorEd
-00091950: 6974 6f72 206a 702d 4564 6974 6f72 206a  itor jp-Editor j
-00091960: 702d 496e 7075 7441 7265 612d 6564 6974  p-InputArea-edit
-00091970: 6f72 2220 6461 7461 2d74 7970 653d 2269  or" data-type="i
-00091980: 6e6c 696e 6522 3e0a 2020 2020 203c 6469  nline">.     <di
-00091990: 7620 636c 6173 733d 2243 6f64 654d 6972  v class="CodeMir
-000919a0: 726f 7220 636d 2d73 2d6a 7570 7974 6572  ror cm-s-jupyter
-000919b0: 223e 0a3c 6469 7620 636c 6173 733d 2220  ">.<div class=" 
-000919c0: 6869 6768 6c69 6768 7420 686c 2d69 7079  highlight hl-ipy
-000919d0: 7468 6f6e 3322 3e3c 7072 653e 3c73 7061  thon3"><pre><spa
-000919e0: 6e3e 3c2f 7370 616e 3e3c 7370 616e 2063  n></span><span c
-000919f0: 6c61 7373 3d22 6b6e 223e 6672 6f6d 3c2f  lass="kn">from</
-00091a00: 7370 616e 3e20 3c73 7061 6e20 636c 6173  span> <span clas
-00091a10: 733d 226e 6e22 3e6d 6174 6461 7461 2e67  s="nn">matdata.g
-00091a20: 656e 6572 6174 6f72 3c2f 7370 616e 3e20  enerator</span> 
-00091a30: 3c73 7061 6e20 636c 6173 733d 226b 6e22  <span class="kn"
-00091a40: 3e69 6d70 6f72 743c 2f73 7061 6e3e 203c  >import</span> <
-00091a50: 7370 616e 2063 6c61 7373 3d22 6f22 3e2a  span class="o">*
-00091a60: 3c2f 7370 616e 3e0a 3c2f 7072 653e 3c2f  </span>.</pre></
-00091a70: 6469 763e 0a0a 2020 2020 203c 2f64 6976  div>..     </div
-00091a80: 3e0a 3c2f 6469 763e 0a3c 2f64 6976 3e0a  >.</div>.</div>.
-00091a90: 3c2f 6469 763e 0a0a 3c2f 6469 763e 0a3c  </div>..</div>.<
-00091aa0: 6469 7620 636c 6173 733d 226a 702d 4365  div class="jp-Ce
-00091ab0: 6c6c 206a 702d 4d61 726b 646f 776e 4365  ll jp-MarkdownCe
-00091ac0: 6c6c 206a 702d 4e6f 7465 626f 6f6b 2d63  ll jp-Notebook-c
-00091ad0: 656c 6c22 3e0a 3c64 6976 2063 6c61 7373  ell">.<div class
-00091ae0: 3d22 6a70 2d43 656c 6c2d 696e 7075 7457  ="jp-Cell-inputW
-00091af0: 7261 7070 6572 223e 0a3c 6469 7620 636c  rapper">.<div cl
-00091b00: 6173 733d 226a 702d 436f 6c6c 6170 7365  ass="jp-Collapse
-00091b10: 7220 6a70 2d49 6e70 7574 436f 6c6c 6170  r jp-InputCollap
-00091b20: 7365 7220 6a70 2d43 656c 6c2d 696e 7075  ser jp-Cell-inpu
-00091b30: 7443 6f6c 6c61 7073 6572 223e 0a3c 2f64  tCollapser">.</d
-00091b40: 6976 3e0a 3c64 6976 2063 6c61 7373 3d22  iv>.<div class="
-00091b50: 6a70 2d49 6e70 7574 4172 6561 206a 702d  jp-InputArea jp-
-00091b60: 4365 6c6c 2d69 6e70 7574 4172 6561 223e  Cell-inputArea">
-00091b70: 3c64 6976 2063 6c61 7373 3d22 6a70 2d49  <div class="jp-I
-00091b80: 6e70 7574 5072 6f6d 7074 206a 702d 496e  nputPrompt jp-In
-00091b90: 7075 7441 7265 612d 7072 6f6d 7074 223e  putArea-prompt">
-00091ba0: 0a3c 2f64 6976 3e3c 6469 7620 636c 6173  .</div><div clas
-00091bb0: 733d 226a 702d 5265 6e64 6572 6564 4854  s="jp-RenderedHT
-00091bc0: 4d4c 436f 6d6d 6f6e 206a 702d 5265 6e64  MLCommon jp-Rend
-00091bd0: 6572 6564 4d61 726b 646f 776e 206a 702d  eredMarkdown jp-
-00091be0: 4d61 726b 646f 776e 4f75 7470 7574 2022  MarkdownOutput "
-00091bf0: 2064 6174 612d 6d69 6d65 2d74 7970 653d   data-mime-type=
-00091c00: 2274 6578 742f 6d61 726b 646f 776e 223e  "text/markdown">
-00091c10: 0a3c 756c 3e0a 3c6c 693e 3c63 6f64 653e  .<ul>.<li><code>
-00091c20: 7363 616c 6572 5361 6d70 6c65 7247 656e  scalerSamplerGen
-00091c30: 6572 6174 6f72 3c2f 636f 6465 3e3a 2067  erator</code>: g
-00091c40: 656e 6572 6174 6573 2074 7261 6a65 6374  enerates traject
-00091c50: 6f72 7920 6461 7461 7365 7473 2062 6173  ory datasets bas
-00091c60: 6564 206f 6e20 7265 616c 2064 6174 6120  ed on real data 
-00091c70: 6f6e 2073 6361 6c65 2069 6e74 6572 7661  on scale interva
-00091c80: 6c73 3c2f 6c69 3e0a 3c6c 693e 3c63 6f64  ls</li>.<li><cod
-00091c90: 653e 7361 6d70 6c65 7247 656e 6572 6174  e>samplerGenerat
-00091ca0: 6f72 3c2f 636f 6465 3e3a 2067 656e 6572  or</code>: gener
-00091cb0: 6174 6520 6120 7472 616a 6563 746f 7279  ate a trajectory
-00091cc0: 2064 6174 6173 6574 2062 6173 6564 206f   dataset based o
-00091cd0: 6e20 7265 616c 2064 6174 613c 2f6c 693e  n real data</li>
-00091ce0: 0a3c 6c69 3e3c 636f 6465 3e73 6361 6c65  .<li><code>scale
-00091cf0: 7252 616e 646f 6d47 656e 6572 6174 6f72  rRandomGenerator
-00091d00: 3c2f 636f 6465 3e3a 2067 656e 6572 6174  </code>: generat
-00091d10: 6573 2074 7261 6a65 6374 6f72 7920 6461  es trajectory da
-00091d20: 7461 7365 7473 2062 6173 6564 206f 6e20  tasets based on 
-00091d30: 7261 6e64 6f6d 2064 6174 6120 6f6e 2073  random data on s
-00091d40: 6361 6c65 2069 6e74 6572 7661 6c73 3c2f  cale intervals</
-00091d50: 6c69 3e0a 3c6c 693e 3c63 6f64 653e 7261  li>.<li><code>ra
-00091d60: 6e64 6f6d 4765 6e65 7261 746f 723c 2f63  ndomGenerator</c
-00091d70: 6f64 653e 3a20 6765 6e65 7261 7465 2061  ode>: generate a
-00091d80: 2074 7261 6a65 6374 6f72 7920 6461 7461   trajectory data
-00091d90: 7365 7420 6261 7365 6420 6f6e 2072 616e  set based on ran
-00091da0: 646f 6d20 6461 7461 3c2f 6c69 3e0a 3c2f  dom data</li>.</
-00091db0: 756c 3e0a 0a3c 2f64 6976 3e0a 3c2f 6469  ul>..</div>.</di
-00091dc0: 763e 0a3c 2f64 6976 3e0a 3c2f 6469 763e  v>.</div>.</div>
-00091dd0: 3c64 6976 2063 6c61 7373 3d22 6a70 2d43  <div class="jp-C
-00091de0: 656c 6c20 6a70 2d43 6f64 6543 656c 6c20  ell jp-CodeCell 
-00091df0: 6a70 2d4e 6f74 6562 6f6f 6b2d 6365 6c6c  jp-Notebook-cell
-00091e00: 206a 702d 6d6f 642d 6e6f 4f75 7470 7574   jp-mod-noOutput
-00091e10: 7320 2022 3e0a 3c64 6976 2063 6c61 7373  s  ">.<div class
-00091e20: 3d22 6a70 2d43 656c 6c2d 696e 7075 7457  ="jp-Cell-inputW
-00091e30: 7261 7070 6572 223e 0a3c 6469 7620 636c  rapper">.<div cl
-00091e40: 6173 733d 226a 702d 436f 6c6c 6170 7365  ass="jp-Collapse
-00091e50: 7220 6a70 2d49 6e70 7574 436f 6c6c 6170  r jp-InputCollap
-00091e60: 7365 7220 6a70 2d43 656c 6c2d 696e 7075  ser jp-Cell-inpu
-00091e70: 7443 6f6c 6c61 7073 6572 223e 0a3c 2f64  tCollapser">.</d
-00091e80: 6976 3e0a 3c64 6976 2063 6c61 7373 3d22  iv>.<div class="
-00091e90: 6a70 2d49 6e70 7574 4172 6561 206a 702d  jp-InputArea jp-
-00091ea0: 4365 6c6c 2d69 6e70 7574 4172 6561 223e  Cell-inputArea">
-00091eb0: 0a3c 6469 7620 636c 6173 733d 226a 702d  .<div class="jp-
-00091ec0: 496e 7075 7450 726f 6d70 7420 6a70 2d49  InputPrompt jp-I
-00091ed0: 6e70 7574 4172 6561 2d70 726f 6d70 7422  nputArea-prompt"
-00091ee0: 3e49 6e26 6e62 7370 3b5b 266e 6273 703b  >In&nbsp;[&nbsp;
-00091ef0: 5d3a 3c2f 6469 763e 0a3c 6469 7620 636c  ]:</div>.<div cl
-00091f00: 6173 733d 226a 702d 436f 6465 4d69 7272  ass="jp-CodeMirr
-00091f10: 6f72 4564 6974 6f72 206a 702d 4564 6974  orEditor jp-Edit
-00091f20: 6f72 206a 702d 496e 7075 7441 7265 612d  or jp-InputArea-
-00091f30: 6564 6974 6f72 2220 6461 7461 2d74 7970  editor" data-typ
-00091f40: 653d 2269 6e6c 696e 6522 3e0a 2020 2020  e="inline">.    
-00091f50: 203c 6469 7620 636c 6173 733d 2243 6f64   <div class="Cod
-00091f60: 654d 6972 726f 7220 636d 2d73 2d6a 7570  eMirror cm-s-jup
-00091f70: 7974 6572 223e 0a3c 6469 7620 636c 6173  yter">.<div clas
-00091f80: 733d 2220 6869 6768 6c69 6768 7420 686c  s=" highlight hl
-00091f90: 2d69 7079 7468 6f6e 3322 3e3c 7072 653e  -ipython3"><pre>
-00091fa0: 3c73 7061 6e3e 3c2f 7370 616e 3e20 0a3c  <span></span> .<
-00091fb0: 2f70 7265 3e3c 2f64 6976 3e0a 0a20 2020  /pre></div>..   
-00091fc0: 2020 3c2f 6469 763e 0a3c 2f64 6976 3e0a    </div>.</div>.
-00091fd0: 3c2f 6469 763e 0a3c 2f64 6976 3e0a 0a3c  </div>.</div>..<
-00091fe0: 2f64 6976 3e0a 3c64 6976 2063 6c61 7373  /div>.<div class
-00091ff0: 3d22 6a70 2d43 656c 6c20 6a70 2d4d 6172  ="jp-Cell jp-Mar
-00092000: 6b64 6f77 6e43 656c 6c20 6a70 2d4e 6f74  kdownCell jp-Not
-00092010: 6562 6f6f 6b2d 6365 6c6c 223e 0a3c 6469  ebook-cell">.<di
-00092020: 7620 636c 6173 733d 226a 702d 4365 6c6c  v class="jp-Cell
-00092030: 2d69 6e70 7574 5772 6170 7065 7222 3e0a  -inputWrapper">.
-00092040: 3c64 6976 2063 6c61 7373 3d22 6a70 2d43  <div class="jp-C
-00092050: 6f6c 6c61 7073 6572 206a 702d 496e 7075  ollapser jp-Inpu
-00092060: 7443 6f6c 6c61 7073 6572 206a 702d 4365  tCollapser jp-Ce
-00092070: 6c6c 2d69 6e70 7574 436f 6c6c 6170 7365  ll-inputCollapse
-00092080: 7222 3e0a 3c2f 6469 763e 0a3c 6469 7620  r">.</div>.<div 
-00092090: 636c 6173 733d 226a 702d 496e 7075 7441  class="jp-InputA
-000920a0: 7265 6120 6a70 2d43 656c 6c2d 696e 7075  rea jp-Cell-inpu
-000920b0: 7441 7265 6122 3e3c 6469 7620 636c 6173  tArea"><div clas
-000920c0: 733d 226a 702d 496e 7075 7450 726f 6d70  s="jp-InputPromp
-000920d0: 7420 6a70 2d49 6e70 7574 4172 6561 2d70  t jp-InputArea-p
-000920e0: 726f 6d70 7422 3e0a 3c2f 6469 763e 3c64  rompt">.</div><d
-000920f0: 6976 2063 6c61 7373 3d22 6a70 2d52 656e  iv class="jp-Ren
-00092100: 6465 7265 6448 544d 4c43 6f6d 6d6f 6e20  deredHTMLCommon 
-00092110: 6a70 2d52 656e 6465 7265 644d 6172 6b64  jp-RenderedMarkd
-00092120: 6f77 6e20 6a70 2d4d 6172 6b64 6f77 6e4f  own jp-MarkdownO
-00092130: 7574 7075 7420 2220 6461 7461 2d6d 696d  utput " data-mim
-00092140: 652d 7479 7065 3d22 7465 7874 2f6d 6172  e-type="text/mar
-00092150: 6b64 6f77 6e22 3e0a 3c70 3e23 2042 7920  kdown">.<p># By 
-00092160: 5461 726c 6973 2050 6f72 7465 6c61 2028  Tarlis Portela (
-00092170: 3230 3233 293c 2f70 3e0a 0a3c 2f64 6976  2023)</p>..</div
-00092180: 3e0a 3c2f 6469 763e 0a3c 2f64 6976 3e0a  >.</div>.</div>.
-00092190: 3c2f 6469 763e 0a3c 2f62 6f64 793e 0a0a  </div>.</body>..
-000921a0: 0a0a 0a0a 0a0a 3c2f 6874 6d6c 3e0a       ......</html>.
+0008c5d0: 613a 2d44 6174 612d 4861 6e64 6c65 722d  a:-Data-Handler-
+0008c5e0: 666f 722d 4d75 6c74 6970 6c65 2d41 7370  for-Multiple-Asp
+0008c5f0: 6563 742d 5472 616a 6563 746f 7279 2d44  ect-Trajectory-D
+0008c600: 6174 612d 4d69 6e69 6e67 2d25 3542 4d41  ata-Mining-%5BMA
+0008c610: 542d 546f 6f6c 732d 4672 616d 6577 6f72  T-Tools-Framewor
+0008c620: 6b25 3544 223e 4d41 542d 6461 7461 3a20  k%5D">MAT-data: 
+0008c630: 4461 7461 2048 616e 646c 6572 2066 6f72  Data Handler for
+0008c640: 204d 756c 7469 706c 6520 4173 7065 6374   Multiple Aspect
+0008c650: 2054 7261 6a65 6374 6f72 7920 4461 7461   Trajectory Data
+0008c660: 204d 696e 696e 6720 5b4d 4154 2d54 6f6f   Mining [MAT-Too
+0008c670: 6c73 2046 7261 6d65 776f 726b 5d3c 6120  ls Framework]<a 
+0008c680: 636c 6173 733d 2261 6e63 686f 722d 6c69  class="anchor-li
+0008c690: 6e6b 2220 6872 6566 3d22 234d 4154 2d64  nk" href="#MAT-d
+0008c6a0: 6174 613a 2d44 6174 612d 4861 6e64 6c65  ata:-Data-Handle
+0008c6b0: 722d 666f 722d 4d75 6c74 6970 6c65 2d41  r-for-Multiple-A
+0008c6c0: 7370 6563 742d 5472 616a 6563 746f 7279  spect-Trajectory
+0008c6d0: 2d44 6174 612d 4d69 6e69 6e67 2d25 3542  -Data-Mining-%5B
+0008c6e0: 4d41 542d 546f 6f6c 732d 4672 616d 6577  MAT-Tools-Framew
+0008c6f0: 6f72 6b25 3544 223e 2623 3138 323b 3c2f  ork%5D">&#182;</
+0008c700: 613e 3c2f 6831 3e3c 703e 5361 6d70 6c65  a></h1><p>Sample
+0008c710: 2043 6f64 6520 696e 2070 7974 686f 6e20   Code in python 
+0008c720: 6e6f 7465 626f 6f6b 2074 6f20 7573 6520  notebook to use 
+0008c730: 6d61 742d 6461 7461 2061 7320 6120 7079  mat-data as a py
+0008c740: 7468 6f6e 206c 6962 7261 7279 2e3c 2f70  thon library.</p
+0008c750: 3e0a 3c70 3e54 6865 2070 7265 7365 6e74  >.<p>The present
+0008c760: 2070 6163 6b61 6765 206f 6666 6572 7320   package offers 
+0008c770: 6120 746f 6f6c 2c20 746f 2073 7570 706f  a tool, to suppo
+0008c780: 7274 2074 6865 2075 7365 7220 696e 2074  rt the user in t
+0008c790: 6865 2074 6173 6b20 6f66 2064 6174 6120  he task of data 
+0008c7a0: 7072 6570 726f 6365 7373 696e 6720 6f66  preprocessing of
+0008c7b0: 206d 756c 7469 706c 6520 6173 7065 6374   multiple aspect
+0008c7c0: 2074 7261 6a65 6374 6f72 6965 732c 206f   trajectories, o
+0008c7d0: 7220 746f 2067 656e 6572 6174 696e 6720  r to generating 
+0008c7e0: 7379 6e74 6865 7469 6320 6461 7461 7365  synthetic datase
+0008c7f0: 7473 2e20 4974 2069 6e74 6567 7261 7465  ts. It integrate
+0008c800: 7320 696e 746f 2061 2075 6e69 7175 6520  s into a unique 
+0008c810: 6672 616d 6577 6f72 6b20 666f 7220 6d75  framework for mu
+0008c820: 6c74 6970 6c65 2061 7370 6563 7473 2074  ltiple aspects t
+0008c830: 7261 6a65 6374 6f72 6965 7320 616e 6420  rajectories and 
+0008c840: 696e 2067 656e 6572 616c 2066 6f72 206d  in general for m
+0008c850: 756c 7469 6469 6d65 6e73 696f 6e61 6c20  ultidimensional 
+0008c860: 7365 7175 656e 6365 2064 6174 6120 6d69  sequence data mi
+0008c870: 6e69 6e67 206d 6574 686f 6473 2e3c 2f70  ning methods.</p
+0008c880: 3e0a 3c70 3e43 7265 6174 6564 206f 6e20  >.<p>Created on 
+0008c890: 4465 632c 2032 3032 330a 436f 7079 7269  Dec, 2023.Copyri
+0008c8a0: 6768 7420 2843 2920 3230 3233 2c20 4c69  ght (C) 2023, Li
+0008c8b0: 6365 6e73 6520 4750 4c20 5665 7273 696f  cense GPL Versio
+0008c8c0: 6e20 3320 6f72 2073 7570 6572 696f 7220  n 3 or superior 
+0008c8d0: 2873 6565 204c 4943 454e 5345 2066 696c  (see LICENSE fil
+0008c8e0: 6529 3c2f 703e 0a0a 3c2f 6469 763e 0a3c  e)</p>..</div>.<
+0008c8f0: 2f64 6976 3e0a 3c2f 6469 763e 0a3c 2f64  /div>.</div>.</d
+0008c900: 6976 3e3c 6469 7620 636c 6173 733d 226a  iv><div class="j
+0008c910: 702d 4365 6c6c 206a 702d 436f 6465 4365  p-Cell jp-CodeCe
+0008c920: 6c6c 206a 702d 4e6f 7465 626f 6f6b 2d63  ll jp-Notebook-c
+0008c930: 656c 6c20 6a70 2d6d 6f64 2d6e 6f4f 7574  ell jp-mod-noOut
+0008c940: 7075 7473 2020 223e 0a3c 6469 7620 636c  puts  ">.<div cl
+0008c950: 6173 733d 226a 702d 4365 6c6c 2d69 6e70  ass="jp-Cell-inp
+0008c960: 7574 5772 6170 7065 7222 3e0a 3c64 6976  utWrapper">.<div
+0008c970: 2063 6c61 7373 3d22 6a70 2d43 6f6c 6c61   class="jp-Colla
+0008c980: 7073 6572 206a 702d 496e 7075 7443 6f6c  pser jp-InputCol
+0008c990: 6c61 7073 6572 206a 702d 4365 6c6c 2d69  lapser jp-Cell-i
+0008c9a0: 6e70 7574 436f 6c6c 6170 7365 7222 3e0a  nputCollapser">.
+0008c9b0: 3c2f 6469 763e 0a3c 6469 7620 636c 6173  </div>.<div clas
+0008c9c0: 733d 226a 702d 496e 7075 7441 7265 6120  s="jp-InputArea 
+0008c9d0: 6a70 2d43 656c 6c2d 696e 7075 7441 7265  jp-Cell-inputAre
+0008c9e0: 6122 3e0a 3c64 6976 2063 6c61 7373 3d22  a">.<div class="
+0008c9f0: 6a70 2d49 6e70 7574 5072 6f6d 7074 206a  jp-InputPrompt j
+0008ca00: 702d 496e 7075 7441 7265 612d 7072 6f6d  p-InputArea-prom
+0008ca10: 7074 223e 496e 266e 6273 703b 5b26 6e62  pt">In&nbsp;[&nb
+0008ca20: 7370 3b5d 3a3c 2f64 6976 3e0a 3c64 6976  sp;]:</div>.<div
+0008ca30: 2063 6c61 7373 3d22 6a70 2d43 6f64 654d   class="jp-CodeM
+0008ca40: 6972 726f 7245 6469 746f 7220 6a70 2d45  irrorEditor jp-E
+0008ca50: 6469 746f 7220 6a70 2d49 6e70 7574 4172  ditor jp-InputAr
+0008ca60: 6561 2d65 6469 746f 7222 2064 6174 612d  ea-editor" data-
+0008ca70: 7479 7065 3d22 696e 6c69 6e65 223e 0a20  type="inline">. 
+0008ca80: 2020 2020 3c64 6976 2063 6c61 7373 3d22      <div class="
+0008ca90: 436f 6465 4d69 7272 6f72 2063 6d2d 732d  CodeMirror cm-s-
+0008caa0: 6a75 7079 7465 7222 3e0a 3c64 6976 2063  jupyter">.<div c
+0008cab0: 6c61 7373 3d22 2068 6967 686c 6967 6874  lass=" highlight
+0008cac0: 2068 6c2d 6970 7974 686f 6e33 223e 3c70   hl-ipython3"><p
+0008cad0: 7265 3e3c 7370 616e 3e3c 2f73 7061 6e3e  re><span></span>
+0008cae0: 3c73 7061 6e20 636c 6173 733d 226f 223e  <span class="o">
+0008caf0: 213c 2f73 7061 6e3e 7069 703c 7370 616e  !</span>pip<span
+0008cb00: 2063 6c61 7373 3d22 7722 3e20 3c2f 7370   class="w"> </sp
+0008cb10: 616e 3e69 6e73 7461 6c6c 3c73 7061 6e20  an>install<span 
+0008cb20: 636c 6173 733d 2277 223e 203c 2f73 7061  class="w"> </spa
+0008cb30: 6e3e 6d61 742d 6461 7461 0a3c 7370 616e  n>mat-data.<span
+0008cb40: 2063 6c61 7373 3d22 6331 223e 2321 7069   class="c1">#!pi
+0008cb50: 7020 696e 7374 616c 6c20 2d2d 7570 6772  p install --upgr
+0008cb60: 6164 6520 6d61 742d 6461 7461 3c2f 7370  ade mat-data</sp
+0008cb70: 616e 3e0a 3c2f 7072 653e 3c2f 6469 763e  an>.</pre></div>
+0008cb80: 0a0a 2020 2020 203c 2f64 6976 3e0a 3c2f  ..     </div>.</
+0008cb90: 6469 763e 0a3c 2f64 6976 3e0a 3c2f 6469  div>.</div>.</di
+0008cba0: 763e 0a0a 3c2f 6469 763e 0a3c 6469 7620  v>..</div>.<div 
+0008cbb0: 636c 6173 733d 226a 702d 4365 6c6c 206a  class="jp-Cell j
+0008cbc0: 702d 4d61 726b 646f 776e 4365 6c6c 206a  p-MarkdownCell j
+0008cbd0: 702d 4e6f 7465 626f 6f6b 2d63 656c 6c22  p-Notebook-cell"
+0008cbe0: 3e0a 3c64 6976 2063 6c61 7373 3d22 6a70  >.<div class="jp
+0008cbf0: 2d43 656c 6c2d 696e 7075 7457 7261 7070  -Cell-inputWrapp
+0008cc00: 6572 223e 0a3c 6469 7620 636c 6173 733d  er">.<div class=
+0008cc10: 226a 702d 436f 6c6c 6170 7365 7220 6a70  "jp-Collapser jp
+0008cc20: 2d49 6e70 7574 436f 6c6c 6170 7365 7220  -InputCollapser 
+0008cc30: 6a70 2d43 656c 6c2d 696e 7075 7443 6f6c  jp-Cell-inputCol
+0008cc40: 6c61 7073 6572 223e 0a3c 2f64 6976 3e0a  lapser">.</div>.
+0008cc50: 3c64 6976 2063 6c61 7373 3d22 6a70 2d49  <div class="jp-I
+0008cc60: 6e70 7574 4172 6561 206a 702d 4365 6c6c  nputArea jp-Cell
+0008cc70: 2d69 6e70 7574 4172 6561 223e 3c64 6976  -inputArea"><div
+0008cc80: 2063 6c61 7373 3d22 6a70 2d49 6e70 7574   class="jp-Input
+0008cc90: 5072 6f6d 7074 206a 702d 496e 7075 7441  Prompt jp-InputA
+0008cca0: 7265 612d 7072 6f6d 7074 223e 0a3c 2f64  rea-prompt">.</d
+0008ccb0: 6976 3e3c 6469 7620 636c 6173 733d 226a  iv><div class="j
+0008ccc0: 702d 5265 6e64 6572 6564 4854 4d4c 436f  p-RenderedHTMLCo
+0008ccd0: 6d6d 6f6e 206a 702d 5265 6e64 6572 6564  mmon jp-Rendered
+0008cce0: 4d61 726b 646f 776e 206a 702d 4d61 726b  Markdown jp-Mark
+0008ccf0: 646f 776e 4f75 7470 7574 2022 2064 6174  downOutput " dat
+0008cd00: 612d 6d69 6d65 2d74 7970 653d 2274 6578  a-mime-type="tex
+0008cd10: 742f 6d61 726b 646f 776e 223e 0a3c 6833  t/markdown">.<h3
+0008cd20: 2069 643d 2231 2e2d 5265 6164 696e 672d   id="1.-Reading-
+0008cd30: 6c6f 6361 6c2d 6461 7461 223e 312e 2052  local-data">1. R
+0008cd40: 6561 6469 6e67 206c 6f63 616c 2064 6174  eading local dat
+0008cd50: 613c 6120 636c 6173 733d 2261 6e63 686f  a<a class="ancho
+0008cd60: 722d 6c69 6e6b 2220 6872 6566 3d22 2331  r-link" href="#1
+0008cd70: 2e2d 5265 6164 696e 672d 6c6f 6361 6c2d  .-Reading-local-
+0008cd80: 6461 7461 223e 2623 3138 323b 3c2f 613e  data">&#182;</a>
+0008cd90: 3c2f 6833 3e3c 703e 5361 6d70 6c65 2063  </h3><p>Sample c
+0008cda0: 6f64 6520 666f 7220 7472 616a 6563 746f  ode for trajecto
+0008cdb0: 7279 2064 6174 6173 6574 2072 6561 6420  ry dataset read 
+0008cdc0: 6672 6f6d 206c 6f63 616c 2066 696c 6573  from local files
+0008cdd0: 3c2f 703e 0a0a 3c2f 6469 763e 0a3c 2f64  </p>..</div>.</d
+0008cde0: 6976 3e0a 3c2f 6469 763e 0a3c 2f64 6976  iv>.</div>.</div
+0008cdf0: 3e0a 3c64 6976 2063 6c61 7373 3d22 6a70  >.<div class="jp
+0008ce00: 2d43 656c 6c20 6a70 2d4d 6172 6b64 6f77  -Cell jp-Markdow
+0008ce10: 6e43 656c 6c20 6a70 2d4e 6f74 6562 6f6f  nCell jp-Noteboo
+0008ce20: 6b2d 6365 6c6c 223e 0a3c 6469 7620 636c  k-cell">.<div cl
+0008ce30: 6173 733d 226a 702d 4365 6c6c 2d69 6e70  ass="jp-Cell-inp
+0008ce40: 7574 5772 6170 7065 7222 3e0a 3c64 6976  utWrapper">.<div
+0008ce50: 2063 6c61 7373 3d22 6a70 2d43 6f6c 6c61   class="jp-Colla
+0008ce60: 7073 6572 206a 702d 496e 7075 7443 6f6c  pser jp-InputCol
+0008ce70: 6c61 7073 6572 206a 702d 4365 6c6c 2d69  lapser jp-Cell-i
+0008ce80: 6e70 7574 436f 6c6c 6170 7365 7222 3e0a  nputCollapser">.
+0008ce90: 3c2f 6469 763e 0a3c 6469 7620 636c 6173  </div>.<div clas
+0008cea0: 733d 226a 702d 496e 7075 7441 7265 6120  s="jp-InputArea 
+0008ceb0: 6a70 2d43 656c 6c2d 696e 7075 7441 7265  jp-Cell-inputAre
+0008cec0: 6122 3e3c 6469 7620 636c 6173 733d 226a  a"><div class="j
+0008ced0: 702d 496e 7075 7450 726f 6d70 7420 6a70  p-InputPrompt jp
+0008cee0: 2d49 6e70 7574 4172 6561 2d70 726f 6d70  -InputArea-promp
+0008cef0: 7422 3e0a 3c2f 6469 763e 3c64 6976 2063  t">.</div><div c
+0008cf00: 6c61 7373 3d22 6a70 2d52 656e 6465 7265  lass="jp-Rendere
+0008cf10: 6448 544d 4c43 6f6d 6d6f 6e20 6a70 2d52  dHTMLCommon jp-R
+0008cf20: 656e 6465 7265 644d 6172 6b64 6f77 6e20  enderedMarkdown 
+0008cf30: 6a70 2d4d 6172 6b64 6f77 6e4f 7574 7075  jp-MarkdownOutpu
+0008cf40: 7420 2220 6461 7461 2d6d 696d 652d 7479  t " data-mime-ty
+0008cf50: 7065 3d22 7465 7874 2f6d 6172 6b64 6f77  pe="text/markdow
+0008cf60: 6e22 3e0a 3c70 3e54 6865 2065 6173 7920  n">.<p>The easy 
+0008cf70: 7761 7920 746f 2072 6561 6420 6461 7461  way to read data
+0008cf80: 2069 7320 746f 206c 6f61 6420 6120 6373   is to load a cs
+0008cf90: 7620 6669 6c65 2069 6e20 7061 6e64 6173  v file in pandas
+0008cfa0: 2c20 7375 6368 2061 733a 3c2f 703e 0a0a  , such as:</p>..
+0008cfb0: 3c2f 6469 763e 0a3c 2f64 6976 3e0a 3c2f  </div>.</div>.</
+0008cfc0: 6469 763e 0a3c 2f64 6976 3e3c 6469 7620  div>.</div><div 
+0008cfd0: 636c 6173 733d 226a 702d 4365 6c6c 206a  class="jp-Cell j
+0008cfe0: 702d 436f 6465 4365 6c6c 206a 702d 4e6f  p-CodeCell jp-No
+0008cff0: 7465 626f 6f6b 2d63 656c 6c20 2020 223e  tebook-cell   ">
+0008d000: 0a3c 6469 7620 636c 6173 733d 226a 702d  .<div class="jp-
+0008d010: 4365 6c6c 2d69 6e70 7574 5772 6170 7065  Cell-inputWrappe
+0008d020: 7222 3e0a 3c64 6976 2063 6c61 7373 3d22  r">.<div class="
+0008d030: 6a70 2d43 6f6c 6c61 7073 6572 206a 702d  jp-Collapser jp-
+0008d040: 496e 7075 7443 6f6c 6c61 7073 6572 206a  InputCollapser j
+0008d050: 702d 4365 6c6c 2d69 6e70 7574 436f 6c6c  p-Cell-inputColl
+0008d060: 6170 7365 7222 3e0a 3c2f 6469 763e 0a3c  apser">.</div>.<
+0008d070: 6469 7620 636c 6173 733d 226a 702d 496e  div class="jp-In
+0008d080: 7075 7441 7265 6120 6a70 2d43 656c 6c2d  putArea jp-Cell-
+0008d090: 696e 7075 7441 7265 6122 3e0a 3c64 6976  inputArea">.<div
+0008d0a0: 2063 6c61 7373 3d22 6a70 2d49 6e70 7574   class="jp-Input
+0008d0b0: 5072 6f6d 7074 206a 702d 496e 7075 7441  Prompt jp-InputA
+0008d0c0: 7265 612d 7072 6f6d 7074 223e 496e 266e  rea-prompt">In&n
+0008d0d0: 6273 703b 5b38 5d3a 3c2f 6469 763e 0a3c  bsp;[8]:</div>.<
+0008d0e0: 6469 7620 636c 6173 733d 226a 702d 436f  div class="jp-Co
+0008d0f0: 6465 4d69 7272 6f72 4564 6974 6f72 206a  deMirrorEditor j
+0008d100: 702d 4564 6974 6f72 206a 702d 496e 7075  p-Editor jp-Inpu
+0008d110: 7441 7265 612d 6564 6974 6f72 2220 6461  tArea-editor" da
+0008d120: 7461 2d74 7970 653d 2269 6e6c 696e 6522  ta-type="inline"
+0008d130: 3e0a 2020 2020 203c 6469 7620 636c 6173  >.     <div clas
+0008d140: 733d 2243 6f64 654d 6972 726f 7220 636d  s="CodeMirror cm
+0008d150: 2d73 2d6a 7570 7974 6572 223e 0a3c 6469  -s-jupyter">.<di
+0008d160: 7620 636c 6173 733d 2220 6869 6768 6c69  v class=" highli
+0008d170: 6768 7420 686c 2d69 7079 7468 6f6e 3322  ght hl-ipython3"
+0008d180: 3e3c 7072 653e 3c73 7061 6e3e 3c2f 7370  ><pre><span></sp
+0008d190: 616e 3e3c 7370 616e 2063 6c61 7373 3d22  an><span class="
+0008d1a0: 6b6e 223e 696d 706f 7274 3c2f 7370 616e  kn">import</span
+0008d1b0: 3e20 3c73 7061 6e20 636c 6173 733d 226e  > <span class="n
+0008d1c0: 6e22 3e70 616e 6461 733c 2f73 7061 6e3e  n">pandas</span>
+0008d1d0: 203c 7370 616e 2063 6c61 7373 3d22 6b22   <span class="k"
+0008d1e0: 3e61 733c 2f73 7061 6e3e 203c 7370 616e  >as</span> <span
+0008d1f0: 2063 6c61 7373 3d22 6e6e 223e 7064 3c2f   class="nn">pd</
+0008d200: 7370 616e 3e0a 0a3c 7370 616e 2063 6c61  span>..<span cla
+0008d210: 7373 3d22 6e22 3e64 6174 615f 7061 7468  ss="n">data_path
+0008d220: 3c2f 7370 616e 3e20 3c73 7061 6e20 636c  </span> <span cl
+0008d230: 6173 733d 226f 223e 3d3c 2f73 7061 6e3e  ass="o">=</span>
+0008d240: 203c 7370 616e 2063 6c61 7373 3d22 7331   <span class="s1
+0008d250: 223e 2623 3339 3b6d 6174 6461 7461 2f61  ">&#39;matdata/a
+0008d260: 7373 6574 732f 7361 6d70 6c65 2623 3339  ssets/sample&#39
+0008d270: 3b3c 2f73 7061 6e3e 0a0a 3c73 7061 6e20  ;</span>..<span 
+0008d280: 636c 6173 733d 226e 223e 7064 3c2f 7370  class="n">pd</sp
+0008d290: 616e 3e3c 7370 616e 2063 6c61 7373 3d22  an><span class="
+0008d2a0: 6f22 3e2e 3c2f 7370 616e 3e3c 7370 616e  o">.</span><span
+0008d2b0: 2063 6c61 7373 3d22 6e22 3e72 6561 645f   class="n">read_
+0008d2c0: 6373 763c 2f73 7061 6e3e 3c73 7061 6e20  csv</span><span 
+0008d2d0: 636c 6173 733d 2270 223e 283c 2f73 7061  class="p">(</spa
+0008d2e0: 6e3e 3c73 7061 6e20 636c 6173 733d 226e  n><span class="n
+0008d2f0: 223e 6461 7461 5f70 6174 683c 2f73 7061  ">data_path</spa
+0008d300: 6e3e 203c 7370 616e 2063 6c61 7373 3d22  n> <span class="
+0008d310: 6f22 3e2b 3c2f 7370 616e 3e20 3c73 7061  o">+</span> <spa
+0008d320: 6e20 636c 6173 733d 2273 3122 3e26 2333  n class="s1">&#3
+0008d330: 393b 2f46 6f75 7273 7175 6172 655f 5361  9;/Foursquare_Sa
+0008d340: 6d70 6c65 2e63 7376 2623 3339 3b3c 2f73  mple.csv&#39;</s
+0008d350: 7061 6e3e 3c73 7061 6e20 636c 6173 733d  pan><span class=
+0008d360: 2270 223e 293c 2f73 7061 6e3e 0a3c 2f70  "p">)</span>.</p
+0008d370: 7265 3e3c 2f64 6976 3e0a 0a20 2020 2020  re></div>..     
+0008d380: 3c2f 6469 763e 0a3c 2f64 6976 3e0a 3c2f  </div>.</div>.</
+0008d390: 6469 763e 0a3c 2f64 6976 3e0a 0a3c 6469  div>.</div>..<di
+0008d3a0: 7620 636c 6173 733d 226a 702d 4365 6c6c  v class="jp-Cell
+0008d3b0: 2d6f 7574 7075 7457 7261 7070 6572 223e  -outputWrapper">
+0008d3c0: 0a3c 6469 7620 636c 6173 733d 226a 702d  .<div class="jp-
+0008d3d0: 436f 6c6c 6170 7365 7220 6a70 2d4f 7574  Collapser jp-Out
+0008d3e0: 7075 7443 6f6c 6c61 7073 6572 206a 702d  putCollapser jp-
+0008d3f0: 4365 6c6c 2d6f 7574 7075 7443 6f6c 6c61  Cell-outputColla
+0008d400: 7073 6572 223e 0a3c 2f64 6976 3e0a 0a0a  pser">.</div>...
+0008d410: 3c64 6976 2063 6c61 7373 3d22 6a70 2d4f  <div class="jp-O
+0008d420: 7574 7075 7441 7265 6120 6a70 2d43 656c  utputArea jp-Cel
+0008d430: 6c2d 6f75 7470 7574 4172 6561 223e 0a0a  l-outputArea">..
+0008d440: 3c64 6976 2063 6c61 7373 3d22 6a70 2d4f  <div class="jp-O
+0008d450: 7574 7075 7441 7265 612d 6368 696c 6422  utputArea-child"
+0008d460: 3e0a 0a20 2020 200a 2020 2020 3c64 6976  >..    .    <div
+0008d470: 2063 6c61 7373 3d22 6a70 2d4f 7574 7075   class="jp-Outpu
+0008d480: 7450 726f 6d70 7420 6a70 2d4f 7574 7075  tPrompt jp-Outpu
+0008d490: 7441 7265 612d 7072 6f6d 7074 223e 4f75  tArea-prompt">Ou
+0008d4a0: 745b 385d 3a3c 2f64 6976 3e0a 0a0a 0a3c  t[8]:</div>....<
+0008d4b0: 6469 7620 636c 6173 733d 226a 702d 5265  div class="jp-Re
+0008d4c0: 6e64 6572 6564 4854 4d4c 436f 6d6d 6f6e  nderedHTMLCommon
+0008d4d0: 206a 702d 5265 6e64 6572 6564 4854 4d4c   jp-RenderedHTML
+0008d4e0: 206a 702d 4f75 7470 7574 4172 6561 2d6f   jp-OutputArea-o
+0008d4f0: 7574 7075 7420 6a70 2d4f 7574 7075 7441  utput jp-OutputA
+0008d500: 7265 612d 6578 6563 7574 6552 6573 756c  rea-executeResul
+0008d510: 7422 2064 6174 612d 6d69 6d65 2d74 7970  t" data-mime-typ
+0008d520: 653d 2274 6578 742f 6874 6d6c 223e 0a3c  e="text/html">.<
+0008d530: 6469 763e 0a3c 7374 796c 6520 7363 6f70  div>.<style scop
+0008d540: 6564 3e0a 2020 2020 2e64 6174 6166 7261  ed>.    .datafra
+0008d550: 6d65 2074 626f 6479 2074 7220 7468 3a6f  me tbody tr th:o
+0008d560: 6e6c 792d 6f66 2d74 7970 6520 7b0a 2020  nly-of-type {.  
+0008d570: 2020 2020 2020 7665 7274 6963 616c 2d61        vertical-a
+0008d580: 6c69 676e 3a20 6d69 6464 6c65 3b0a 2020  lign: middle;.  
+0008d590: 2020 7d0a 0a20 2020 202e 6461 7461 6672    }..    .datafr
+0008d5a0: 616d 6520 7462 6f64 7920 7472 2074 6820  ame tbody tr th 
+0008d5b0: 7b0a 2020 2020 2020 2020 7665 7274 6963  {.        vertic
+0008d5c0: 616c 2d61 6c69 676e 3a20 746f 703b 0a20  al-align: top;. 
+0008d5d0: 2020 207d 0a0a 2020 2020 2e64 6174 6166     }..    .dataf
+0008d5e0: 7261 6d65 2074 6865 6164 2074 6820 7b0a  rame thead th {.
+0008d5f0: 2020 2020 2020 2020 7465 7874 2d61 6c69          text-ali
+0008d600: 676e 3a20 7269 6768 743b 0a20 2020 207d  gn: right;.    }
+0008d610: 0a3c 2f73 7479 6c65 3e0a 3c74 6162 6c65  .</style>.<table
+0008d620: 2062 6f72 6465 723d 2231 2220 636c 6173   border="1" clas
+0008d630: 733d 2264 6174 6166 7261 6d65 223e 0a20  s="dataframe">. 
+0008d640: 203c 7468 6561 643e 0a20 2020 203c 7472   <thead>.    <tr
+0008d650: 2073 7479 6c65 3d22 7465 7874 2d61 6c69   style="text-ali
+0008d660: 676e 3a20 7269 6768 743b 223e 0a20 2020  gn: right;">.   
+0008d670: 2020 203c 7468 3e3c 2f74 683e 0a20 2020     <th></th>.   
+0008d680: 2020 203c 7468 3e74 6964 3c2f 7468 3e0a     <th>tid</th>.
+0008d690: 2020 2020 2020 3c74 683e 6c61 745f 6c6f        <th>lat_lo
+0008d6a0: 6e3c 2f74 683e 0a20 2020 2020 203c 7468  n</th>.      <th
+0008d6b0: 3e64 6174 655f 7469 6d65 3c2f 7468 3e0a  >date_time</th>.
+0008d6c0: 2020 2020 2020 3c74 683e 7469 6d65 3c2f        <th>time</
+0008d6d0: 7468 3e0a 2020 2020 2020 3c74 683e 7261  th>.      <th>ra
+0008d6e0: 7469 6e67 3c2f 7468 3e0a 2020 2020 2020  ting</th>.      
+0008d6f0: 3c74 683e 7072 6963 653c 2f74 683e 0a20  <th>price</th>. 
+0008d700: 2020 2020 203c 7468 3e77 6561 7468 6572       <th>weather
+0008d710: 3c2f 7468 3e0a 2020 2020 2020 3c74 683e  </th>.      <th>
+0008d720: 6461 793c 2f74 683e 0a20 2020 2020 203c  day</th>.      <
+0008d730: 7468 3e72 6f6f 745f 7479 7065 3c2f 7468  th>root_type</th
+0008d740: 3e0a 2020 2020 2020 3c74 683e 7479 7065  >.      <th>type
+0008d750: 3c2f 7468 3e0a 2020 2020 3c2f 7472 3e0a  </th>.    </tr>.
+0008d760: 2020 3c2f 7468 6561 643e 0a20 203c 7462    </thead>.  <tb
+0008d770: 6f64 793e 0a20 2020 203c 7472 3e0a 2020  ody>.    <tr>.  
+0008d780: 2020 2020 3c74 683e 303c 2f74 683e 0a20      <th>0</th>. 
+0008d790: 2020 2020 203c 7464 3e31 3236 3c2f 7464       <td>126</td
+0008d7a0: 3e0a 2020 2020 2020 3c74 643e 3430 2e38  >.      <td>40.8
+0008d7b0: 3333 3136 3532 3030 3632 3234 202d 3733  331652006224 -73
+0008d7c0: 2e39 3431 3836 3033 3432 3736 3932 3c2f  .9418603427692</
+0008d7d0: 7464 3e0a 2020 2020 2020 3c74 643e 3230  td>.      <td>20
+0008d7e0: 3132 2d31 312d 3132 2030 353a 3137 3a31  12-11-12 05:17:1
+0008d7f0: 383c 2f74 643e 0a20 2020 2020 203c 7464  8</td>.      <td
+0008d800: 3e33 3137 3c2f 7464 3e0a 2020 2020 2020  >317</td>.      
+0008d810: 3c74 643e 2d31 2e30 3c2f 7464 3e0a 2020  <td>-1.0</td>.  
+0008d820: 2020 2020 3c74 643e 2d31 3c2f 7464 3e0a      <td>-1</td>.
+0008d830: 2020 2020 2020 3c74 643e 436c 6561 723c        <td>Clear<
+0008d840: 2f74 643e 0a20 2020 2020 203c 7464 3e4d  /td>.      <td>M
+0008d850: 6f6e 6461 793c 2f74 643e 0a20 2020 2020  onday</td>.     
+0008d860: 203c 7464 3e52 6573 6964 656e 6365 3c2f   <td>Residence</
+0008d870: 7464 3e0a 2020 2020 2020 3c74 643e 486f  td>.      <td>Ho
+0008d880: 6d65 2028 7072 6976 6174 6529 3c2f 7464  me (private)</td
+0008d890: 3e0a 2020 2020 3c2f 7472 3e0a 2020 2020  >.    </tr>.    
+0008d8a0: 3c74 723e 0a20 2020 2020 203c 7468 3e31  <tr>.      <th>1
+0008d8b0: 3c2f 7468 3e0a 2020 2020 2020 3c74 643e  </th>.      <td>
+0008d8c0: 3132 363c 2f74 643e 0a20 2020 2020 203c  126</td>.      <
+0008d8d0: 7464 3e34 302e 3833 3430 3937 3830 3431  td>40.8340978041
+0008d8e0: 3037 3220 2d37 332e 3934 3532 3637 3232  072 -73.94526722
+0008d8f0: 3235 3838 313c 2f74 643e 0a20 2020 2020  25881</td>.     
+0008d900: 203c 7464 3e32 3031 322d 3131 2d31 3220   <td>2012-11-12 
+0008d910: 3233 3a32 343a 3535 3c2f 7464 3e0a 2020  23:24:55</td>.  
+0008d920: 2020 2020 3c74 643e 3134 3034 3c2f 7464      <td>1404</td
+0008d930: 3e0a 2020 2020 2020 3c74 643e 382e 323c  >.      <td>8.2<
+0008d940: 2f74 643e 0a20 2020 2020 203c 7464 3e31  /td>.      <td>1
+0008d950: 3c2f 7464 3e0a 2020 2020 2020 3c74 643e  </td>.      <td>
+0008d960: 436c 6f75 6473 3c2f 7464 3e0a 2020 2020  Clouds</td>.    
+0008d970: 2020 3c74 643e 4d6f 6e64 6179 3c2f 7464    <td>Monday</td
+0008d980: 3e0a 2020 2020 2020 3c74 643e 466f 6f64  >.      <td>Food
+0008d990: 3c2f 7464 3e0a 2020 2020 2020 3c74 643e  </td>.      <td>
+0008d9a0: 4465 6c69 202f 2042 6f64 6567 613c 2f74  Deli / Bodega</t
+0008d9b0: 643e 0a20 2020 203c 2f74 723e 0a20 2020  d>.    </tr>.   
+0008d9c0: 203c 7472 3e0a 2020 2020 2020 3c74 683e   <tr>.      <th>
+0008d9d0: 323c 2f74 683e 0a20 2020 2020 203c 7464  2</th>.      <td
+0008d9e0: 3e31 3236 3c2f 7464 3e0a 2020 2020 2020  >126</td>.      
+0008d9f0: 3c74 643e 3430 2e38 3333 3136 3532 3030  <td>40.833165200
+0008da00: 3632 3234 202d 3733 2e39 3431 3836 3033  6224 -73.9418603
+0008da10: 3432 3736 3932 3c2f 7464 3e0a 2020 2020  427692</td>.    
+0008da20: 2020 3c74 643e 3230 3132 2d31 312d 3133    <td>2012-11-13
+0008da30: 2030 303a 3030 3a30 373c 2f74 643e 0a20   00:00:07</td>. 
+0008da40: 2020 2020 203c 7464 3e30 3c2f 7464 3e0a       <td>0</td>.
+0008da50: 2020 2020 2020 3c74 643e 2d31 2e30 3c2f        <td>-1.0</
+0008da60: 7464 3e0a 2020 2020 2020 3c74 643e 2d31  td>.      <td>-1
+0008da70: 3c2f 7464 3e0a 2020 2020 2020 3c74 643e  </td>.      <td>
+0008da80: 436c 6f75 6473 3c2f 7464 3e0a 2020 2020  Clouds</td>.    
+0008da90: 2020 3c74 643e 5475 6573 6461 793c 2f74    <td>Tuesday</t
+0008daa0: 643e 0a20 2020 2020 203c 7464 3e52 6573  d>.      <td>Res
+0008dab0: 6964 656e 6365 3c2f 7464 3e0a 2020 2020  idence</td>.    
+0008dac0: 2020 3c74 643e 486f 6d65 2028 7072 6976    <td>Home (priv
+0008dad0: 6174 6529 3c2f 7464 3e0a 2020 2020 3c2f  ate)</td>.    </
+0008dae0: 7472 3e0a 2020 2020 3c74 723e 0a20 2020  tr>.    <tr>.   
+0008daf0: 2020 203c 7468 3e33 3c2f 7468 3e0a 2020     <th>3</th>.  
+0008db00: 2020 2020 3c74 643e 3132 363c 2f74 643e      <td>126</td>
+0008db10: 0a20 2020 2020 203c 7464 3e34 302e 3736  .      <td>40.76
+0008db20: 3436 3935 3932 3833 3235 3420 2d37 332e  46959283254 -73.
+0008db30: 3838 3531 3937 3439 3634 3431 343c 2f74  8851974964414</t
+0008db40: 643e 0a20 2020 2020 203c 7464 3e32 3031  d>.      <td>201
+0008db50: 322d 3131 2d31 3520 3137 3a34 393a 3031  2-11-15 17:49:01
+0008db60: 3c2f 7464 3e0a 2020 2020 2020 3c74 643e  </td>.      <td>
+0008db70: 3130 3639 3c2f 7464 3e0a 2020 2020 2020  1069</td>.      
+0008db80: 3c74 643e 362e 363c 2f74 643e 0a20 2020  <td>6.6</td>.   
+0008db90: 2020 203c 7464 3e33 3c2f 7464 3e0a 2020     <td>3</td>.  
+0008dba0: 2020 2020 3c74 643e 436c 6561 723c 2f74      <td>Clear</t
+0008dbb0: 643e 0a20 2020 2020 203c 7464 3e54 6875  d>.      <td>Thu
+0008dbc0: 7273 6461 793c 2f74 643e 0a20 2020 2020  rsday</td>.     
+0008dbd0: 203c 7464 3e46 6f6f 643c 2f74 643e 0a20   <td>Food</td>. 
+0008dbe0: 2020 2020 203c 7464 3e46 7269 6564 2043       <td>Fried C
+0008dbf0: 6869 636b 656e 204a 6f69 6e74 3c2f 7464  hicken Joint</td
+0008dc00: 3e0a 2020 2020 3c2f 7472 3e0a 2020 2020  >.    </tr>.    
+0008dc10: 3c74 723e 0a20 2020 2020 203c 7468 3e34  <tr>.      <th>4
+0008dc20: 3c2f 7468 3e0a 2020 2020 2020 3c74 643e  </th>.      <td>
+0008dc30: 3132 363c 2f74 643e 0a20 2020 2020 203c  126</td>.      <
+0008dc40: 7464 3e34 302e 3736 3630 3739 3033 3736  td>40.7660790376
+0008dc50: 3832 3420 2d37 332e 3838 3335 3238 3730  824 -73.88352870
+0008dc60: 3934 3131 363c 2f74 643e 0a20 2020 2020  94116</td>.     
+0008dc70: 203c 7464 3e32 3031 322d 3131 2d31 3520   <td>2012-11-15 
+0008dc80: 3138 3a34 303a 3136 3c2f 7464 3e0a 2020  18:40:16</td>.  
+0008dc90: 2020 2020 3c74 643e 3131 3230 3c2f 7464      <td>1120</td
+0008dca0: 3e0a 2020 2020 2020 3c74 643e 2d31 2e30  >.      <td>-1.0
+0008dcb0: 3c2f 7464 3e0a 2020 2020 2020 3c74 643e  </td>.      <td>
+0008dcc0: 2d31 3c2f 7464 3e0a 2020 2020 2020 3c74  -1</td>.      <t
+0008dcd0: 643e 436c 6561 723c 2f74 643e 0a20 2020  d>Clear</td>.   
+0008dce0: 2020 203c 7464 3e54 6875 7273 6461 793c     <td>Thursday<
+0008dcf0: 2f74 643e 0a20 2020 2020 203c 7464 3e54  /td>.      <td>T
+0008dd00: 7261 7665 6c20 2661 6d70 3b20 5472 616e  ravel &amp; Tran
+0008dd10: 7370 6f72 743c 2f74 643e 0a20 2020 2020  sport</td>.     
+0008dd20: 203c 7464 3e42 7573 2053 7461 7469 6f6e   <td>Bus Station
+0008dd30: 3c2f 7464 3e0a 2020 2020 3c2f 7472 3e0a  </td>.    </tr>.
+0008dd40: 2020 2020 3c74 723e 0a20 2020 2020 203c      <tr>.      <
+0008dd50: 7468 3e2e 2e2e 3c2f 7468 3e0a 2020 2020  th>...</th>.    
+0008dd60: 2020 3c74 643e 2e2e 2e3c 2f74 643e 0a20    <td>...</td>. 
+0008dd70: 2020 2020 203c 7464 3e2e 2e2e 3c2f 7464       <td>...</td
+0008dd80: 3e0a 2020 2020 2020 3c74 643e 2e2e 2e3c  >.      <td>...<
+0008dd90: 2f74 643e 0a20 2020 2020 203c 7464 3e2e  /td>.      <td>.
+0008dda0: 2e2e 3c2f 7464 3e0a 2020 2020 2020 3c74  ..</td>.      <t
+0008ddb0: 643e 2e2e 2e3c 2f74 643e 0a20 2020 2020  d>...</td>.     
+0008ddc0: 203c 7464 3e2e 2e2e 3c2f 7464 3e0a 2020   <td>...</td>.  
+0008ddd0: 2020 2020 3c74 643e 2e2e 2e3c 2f74 643e      <td>...</td>
+0008dde0: 0a20 2020 2020 203c 7464 3e2e 2e2e 3c2f  .      <td>...</
+0008ddf0: 7464 3e0a 2020 2020 2020 3c74 643e 2e2e  td>.      <td>..
+0008de00: 2e3c 2f74 643e 0a20 2020 2020 203c 7464  .</td>.      <td
+0008de10: 3e2e 2e2e 3c2f 7464 3e0a 2020 2020 3c2f  >...</td>.    </
+0008de20: 7472 3e0a 2020 2020 3c74 723e 0a20 2020  tr>.    <tr>.   
+0008de30: 2020 203c 7468 3e36 3639 3537 3c2f 7468     <th>66957</th
+0008de40: 3e0a 2020 2020 2020 3c74 643e 3239 3536  >.      <td>2956
+0008de50: 333c 2f74 643e 0a20 2020 2020 203c 7464  3</td>.      <td
+0008de60: 3e34 302e 3730 3437 3333 3237 3839 3034  >40.704733278904
+0008de70: 3320 2d37 332e 3938 3737 3337 3839 3430  3 -73.9877378940
+0008de80: 3538 323c 2f74 643e 0a20 2020 2020 203c  582</td>.      <
+0008de90: 7464 3e32 3031 322d 3038 2d31 3020 3137  td>2012-08-10 17
+0008dea0: 3a31 373a 3337 3c2f 7464 3e0a 2020 2020  :17:37</td>.    
+0008deb0: 2020 3c74 643e 3130 3337 3c2f 7464 3e0a    <td>1037</td>.
+0008dec0: 2020 2020 2020 3c74 643e 2d31 2e30 3c2f        <td>-1.0</
+0008ded0: 7464 3e0a 2020 2020 2020 3c74 643e 2d31  td>.      <td>-1
+0008dee0: 3c2f 7464 3e0a 2020 2020 2020 3c74 643e  </td>.      <td>
+0008def0: 436c 6f75 6473 3c2f 7464 3e0a 2020 2020  Clouds</td>.    
+0008df00: 2020 3c74 643e 4672 6964 6179 3c2f 7464    <td>Friday</td
+0008df10: 3e0a 2020 2020 2020 3c74 643e 436f 6c6c  >.      <td>Coll
+0008df20: 6567 6520 2661 6d70 3b20 556e 6976 6572  ege &amp; Univer
+0008df30: 7369 7479 3c2f 7464 3e0a 2020 2020 2020  sity</td>.      
+0008df40: 3c74 643e 4765 6e65 7261 6c20 436f 6c6c  <td>General Coll
+0008df50: 6567 6520 2661 6d70 3b20 556e 6976 6572  ege &amp; Univer
+0008df60: 7369 7479 3c2f 7464 3e0a 2020 2020 3c2f  sity</td>.    </
+0008df70: 7472 3e0a 2020 2020 3c74 723e 0a20 2020  tr>.    <tr>.   
+0008df80: 2020 203c 7468 3e36 3639 3538 3c2f 7468     <th>66958</th
+0008df90: 3e0a 2020 2020 2020 3c74 643e 3239 3536  >.      <td>2956
+0008dfa0: 333c 2f74 643e 0a20 2020 2020 203c 7464  3</td>.      <td
+0008dfb0: 3e34 302e 3639 3531 3632 3733 3630 3139  >40.695162736019
+0008dfc0: 3920 2d37 332e 3939 3534 3437 3836 3931  9 -73.9954478691
+0008dfd0: 3037 323c 2f74 643e 0a20 2020 2020 203c  072</td>.      <
+0008dfe0: 7464 3e32 3031 322d 3038 2d31 3020 3230  td>2012-08-10 20
+0008dff0: 3a31 303a 3539 3c2f 7464 3e0a 2020 2020  :10:59</td>.    
+0008e000: 2020 3c74 643e 3132 3130 3c2f 7464 3e0a    <td>1210</td>.
+0008e010: 2020 2020 2020 3c74 643e 382e 303c 2f74        <td>8.0</t
+0008e020: 643e 0a20 2020 2020 203c 7464 3e32 3c2f  d>.      <td>2</
+0008e030: 7464 3e0a 2020 2020 2020 3c74 643e 436c  td>.      <td>Cl
+0008e040: 6f75 6473 3c2f 7464 3e0a 2020 2020 2020  ouds</td>.      
+0008e050: 3c74 643e 4672 6964 6179 3c2f 7464 3e0a  <td>Friday</td>.
+0008e060: 2020 2020 2020 3c74 643e 466f 6f64 3c2f        <td>Food</
+0008e070: 7464 3e0a 2020 2020 2020 3c74 643e 5468  td>.      <td>Th
+0008e080: 6169 2052 6573 7461 7572 616e 743c 2f74  ai Restaurant</t
+0008e090: 643e 0a20 2020 203c 2f74 723e 0a20 2020  d>.    </tr>.   
+0008e0a0: 203c 7472 3e0a 2020 2020 2020 3c74 683e   <tr>.      <th>
+0008e0b0: 3636 3935 393c 2f74 683e 0a20 2020 2020  66959</th>.     
+0008e0c0: 203c 7464 3e32 3935 3633 3c2f 7464 3e0a   <td>29563</td>.
+0008e0d0: 2020 2020 2020 3c74 643e 3430 2e36 3937        <td>40.697
+0008e0e0: 3830 3236 3635 3238 3232 202d 3733 2e39  8026652822 -73.9
+0008e0f0: 3934 3134 3531 3633 3033 3134 3c2f 7464  941451630314</td
+0008e100: 3e0a 2020 2020 2020 3c74 643e 3230 3132  >.      <td>2012
+0008e110: 2d30 382d 3131 2030 383a 3031 3a32 303c  -08-11 08:01:20<
+0008e120: 2f74 643e 0a20 2020 2020 203c 7464 3e34  /td>.      <td>4
+0008e130: 3831 3c2f 7464 3e0a 2020 2020 2020 3c74  81</td>.      <t
+0008e140: 643e 362e 393c 2f74 643e 0a20 2020 2020  d>6.9</td>.     
+0008e150: 203c 7464 3e2d 313c 2f74 643e 0a20 2020   <td>-1</td>.   
+0008e160: 2020 203c 7464 3e43 6c6f 7564 733c 2f74     <td>Clouds</t
+0008e170: 643e 0a20 2020 2020 203c 7464 3e53 6174  d>.      <td>Sat
+0008e180: 7572 6461 793c 2f74 643e 0a20 2020 2020  urday</td>.     
+0008e190: 203c 7464 3e4f 7574 646f 6f72 7320 2661   <td>Outdoors &a
+0008e1a0: 6d70 3b20 5265 6372 6561 7469 6f6e 3c2f  mp; Recreation</
+0008e1b0: 7464 3e0a 2020 2020 2020 3c74 643e 4779  td>.      <td>Gy
+0008e1c0: 6d3c 2f74 643e 0a20 2020 203c 2f74 723e  m</td>.    </tr>
+0008e1d0: 0a20 2020 203c 7472 3e0a 2020 2020 2020  .    <tr>.      
+0008e1e0: 3c74 683e 3636 3936 303c 2f74 683e 0a20  <th>66960</th>. 
+0008e1f0: 2020 2020 203c 7464 3e32 3935 3633 3c2f       <td>29563</
+0008e200: 7464 3e0a 2020 2020 2020 3c74 643e 3430  td>.      <td>40
+0008e210: 2e36 3934 3637 3238 3936 3735 3033 202d  .6946728967503 -
+0008e220: 3733 2e39 3934 3038 3230 3336 3038 3035  73.9940820360805
+0008e230: 3c2f 7464 3e0a 2020 2020 2020 3c74 643e  </td>.      <td>
+0008e240: 3230 3132 2d30 382d 3131 2031 333a 3339  2012-08-11 13:39
+0008e250: 3a33 393c 2f74 643e 0a20 2020 2020 203c  :39</td>.      <
+0008e260: 7464 3e38 3139 3c2f 7464 3e0a 2020 2020  td>819</td>.    
+0008e270: 2020 3c74 643e 372e 303c 2f74 643e 0a20    <td>7.0</td>. 
+0008e280: 2020 2020 203c 7464 3e31 3c2f 7464 3e0a       <td>1</td>.
+0008e290: 2020 2020 2020 3c74 643e 436c 6f75 6473        <td>Clouds
+0008e2a0: 3c2f 7464 3e0a 2020 2020 2020 3c74 643e  </td>.      <td>
+0008e2b0: 5361 7475 7264 6179 3c2f 7464 3e0a 2020  Saturday</td>.  
+0008e2c0: 2020 2020 3c74 643e 466f 6f64 3c2f 7464      <td>Food</td
+0008e2d0: 3e0a 2020 2020 2020 3c74 643e 436f 6666  >.      <td>Coff
+0008e2e0: 6565 2053 686f 703c 2f74 643e 0a20 2020  ee Shop</td>.   
+0008e2f0: 203c 2f74 723e 0a20 2020 203c 7472 3e0a   </tr>.    <tr>.
+0008e300: 2020 2020 2020 3c74 683e 3636 3936 313c        <th>66961<
+0008e310: 2f74 683e 0a20 2020 2020 203c 7464 3e32  /th>.      <td>2
+0008e320: 3935 3633 3c2f 7464 3e0a 2020 2020 2020  9563</td>.      
+0008e330: 3c74 643e 3430 2e36 3937 3830 3236 3635  <td>40.697802665
+0008e340: 3238 3232 202d 3733 2e39 3934 3134 3531  2822 -73.9941451
+0008e350: 3633 3033 3134 3c2f 7464 3e0a 2020 2020  630314</td>.    
+0008e360: 2020 3c74 643e 3230 3132 2d30 382d 3132    <td>2012-08-12
+0008e370: 2030 373a 3536 3a32 363c 2f74 643e 0a20   07:56:26</td>. 
+0008e380: 2020 2020 203c 7464 3e34 3736 3c2f 7464       <td>476</td
+0008e390: 3e0a 2020 2020 2020 3c74 643e 362e 393c  >.      <td>6.9<
+0008e3a0: 2f74 643e 0a20 2020 2020 203c 7464 3e2d  /td>.      <td>-
+0008e3b0: 313c 2f74 643e 0a20 2020 2020 203c 7464  1</td>.      <td
+0008e3c0: 3e43 6c6f 7564 733c 2f74 643e 0a20 2020  >Clouds</td>.   
+0008e3d0: 2020 203c 7464 3e53 756e 6461 793c 2f74     <td>Sunday</t
+0008e3e0: 643e 0a20 2020 2020 203c 7464 3e4f 7574  d>.      <td>Out
+0008e3f0: 646f 6f72 7320 2661 6d70 3b20 5265 6372  doors &amp; Recr
+0008e400: 6561 7469 6f6e 3c2f 7464 3e0a 2020 2020  eation</td>.    
+0008e410: 2020 3c74 643e 4779 6d3c 2f74 643e 0a20    <td>Gym</td>. 
+0008e420: 2020 203c 2f74 723e 0a20 203c 2f74 626f     </tr>.  </tbo
+0008e430: 6479 3e0a 3c2f 7461 626c 653e 0a3c 703e  dy>.</table>.<p>
+0008e440: 3636 3936 3220 726f 7773 20c3 9720 3130  66962 rows .. 10
+0008e450: 2063 6f6c 756d 6e73 3c2f 703e 0a3c 2f64   columns</p>.</d
+0008e460: 6976 3e0a 3c2f 6469 763e 0a0a 3c2f 6469  iv>.</div>..</di
+0008e470: 763e 0a0a 3c2f 6469 763e 0a0a 3c2f 6469  v>..</div>..</di
+0008e480: 763e 0a0a 3c2f 6469 763e 0a3c 6469 7620  v>..</div>.<div 
+0008e490: 636c 6173 733d 226a 702d 4365 6c6c 206a  class="jp-Cell j
+0008e4a0: 702d 4d61 726b 646f 776e 4365 6c6c 206a  p-MarkdownCell j
+0008e4b0: 702d 4e6f 7465 626f 6f6b 2d63 656c 6c22  p-Notebook-cell"
+0008e4c0: 3e0a 3c64 6976 2063 6c61 7373 3d22 6a70  >.<div class="jp
+0008e4d0: 2d43 656c 6c2d 696e 7075 7457 7261 7070  -Cell-inputWrapp
+0008e4e0: 6572 223e 0a3c 6469 7620 636c 6173 733d  er">.<div class=
+0008e4f0: 226a 702d 436f 6c6c 6170 7365 7220 6a70  "jp-Collapser jp
+0008e500: 2d49 6e70 7574 436f 6c6c 6170 7365 7220  -InputCollapser 
+0008e510: 6a70 2d43 656c 6c2d 696e 7075 7443 6f6c  jp-Cell-inputCol
+0008e520: 6c61 7073 6572 223e 0a3c 2f64 6976 3e0a  lapser">.</div>.
+0008e530: 3c64 6976 2063 6c61 7373 3d22 6a70 2d49  <div class="jp-I
+0008e540: 6e70 7574 4172 6561 206a 702d 4365 6c6c  nputArea jp-Cell
+0008e550: 2d69 6e70 7574 4172 6561 223e 3c64 6976  -inputArea"><div
+0008e560: 2063 6c61 7373 3d22 6a70 2d49 6e70 7574   class="jp-Input
+0008e570: 5072 6f6d 7074 206a 702d 496e 7075 7441  Prompt jp-InputA
+0008e580: 7265 612d 7072 6f6d 7074 223e 0a3c 2f64  rea-prompt">.</d
+0008e590: 6976 3e3c 6469 7620 636c 6173 733d 226a  iv><div class="j
+0008e5a0: 702d 5265 6e64 6572 6564 4854 4d4c 436f  p-RenderedHTMLCo
+0008e5b0: 6d6d 6f6e 206a 702d 5265 6e64 6572 6564  mmon jp-Rendered
+0008e5c0: 4d61 726b 646f 776e 206a 702d 4d61 726b  Markdown jp-Mark
+0008e5d0: 646f 776e 4f75 7470 7574 2022 2064 6174  downOutput " dat
+0008e5e0: 612d 6d69 6d65 2d74 7970 653d 2274 6578  a-mime-type="tex
+0008e5f0: 742f 6d61 726b 646f 776e 223e 0a3c 703e  t/markdown">.<p>
+0008e600: 3c63 6f64 653e 6d61 742d 6461 7461 3c2f  <code>mat-data</
+0008e610: 636f 6465 3e20 7072 6f76 6964 6573 206d  code> provides m
+0008e620: 6f64 756c 6573 2074 6f20 6861 6e64 6c65  odules to handle
+0008e630: 2064 6174 6173 6574 2072 6561 6469 6e67   dataset reading
+0008e640: 2069 6e20 7374 616e 6461 7264 2077 6179   in standard way
+0008e650: 733a 3c2f 703e 0a0a 3c2f 6469 763e 0a3c  s:</p>..</div>.<
+0008e660: 2f64 6976 3e0a 3c2f 6469 763e 0a3c 2f64  /div>.</div>.</d
+0008e670: 6976 3e0a 3c64 6976 2063 6c61 7373 3d22  iv>.<div class="
+0008e680: 6a70 2d43 656c 6c20 6a70 2d4d 6172 6b64  jp-Cell jp-Markd
+0008e690: 6f77 6e43 656c 6c20 6a70 2d4e 6f74 6562  ownCell jp-Noteb
+0008e6a0: 6f6f 6b2d 6365 6c6c 223e 0a3c 6469 7620  ook-cell">.<div 
+0008e6b0: 636c 6173 733d 226a 702d 4365 6c6c 2d69  class="jp-Cell-i
+0008e6c0: 6e70 7574 5772 6170 7065 7222 3e0a 3c64  nputWrapper">.<d
+0008e6d0: 6976 2063 6c61 7373 3d22 6a70 2d43 6f6c  iv class="jp-Col
+0008e6e0: 6c61 7073 6572 206a 702d 496e 7075 7443  lapser jp-InputC
+0008e6f0: 6f6c 6c61 7073 6572 206a 702d 4365 6c6c  ollapser jp-Cell
+0008e700: 2d69 6e70 7574 436f 6c6c 6170 7365 7222  -inputCollapser"
+0008e710: 3e0a 3c2f 6469 763e 0a3c 6469 7620 636c  >.</div>.<div cl
+0008e720: 6173 733d 226a 702d 496e 7075 7441 7265  ass="jp-InputAre
+0008e730: 6120 6a70 2d43 656c 6c2d 696e 7075 7441  a jp-Cell-inputA
+0008e740: 7265 6122 3e3c 6469 7620 636c 6173 733d  rea"><div class=
+0008e750: 226a 702d 496e 7075 7450 726f 6d70 7420  "jp-InputPrompt 
+0008e760: 6a70 2d49 6e70 7574 4172 6561 2d70 726f  jp-InputArea-pro
+0008e770: 6d70 7422 3e0a 3c2f 6469 763e 3c64 6976  mpt">.</div><div
+0008e780: 2063 6c61 7373 3d22 6a70 2d52 656e 6465   class="jp-Rende
+0008e790: 7265 6448 544d 4c43 6f6d 6d6f 6e20 6a70  redHTMLCommon jp
+0008e7a0: 2d52 656e 6465 7265 644d 6172 6b64 6f77  -RenderedMarkdow
+0008e7b0: 6e20 6a70 2d4d 6172 6b64 6f77 6e4f 7574  n jp-MarkdownOut
+0008e7c0: 7075 7420 2220 6461 7461 2d6d 696d 652d  put " data-mime-
+0008e7d0: 7479 7065 3d22 7465 7874 2f6d 6172 6b64  type="text/markd
+0008e7e0: 6f77 6e22 3e0a 0a3c 7072 653e 3c63 6f64  own">..<pre><cod
+0008e7f0: 653e 6129 2052 6561 6420 6120 6461 7461  e>a) Read a data
+0008e800: 7365 7420 6c6f 6361 6c6c 793a 0a0a 3c2f  set locally:..</
+0008e810: 636f 6465 3e3c 2f70 7265 3e0a 3c70 3e54  code></pre>.<p>T
+0008e820: 6869 7320 6973 2061 6e20 6578 616d 706c  his is an exampl
+0008e830: 6520 666f 7220 2e63 7376 2066 696c 652c  e for .csv file,
+0008e840: 2068 6f77 6576 6572 2074 6869 7320 6361   however this ca
+0008e850: 6e20 7265 6164 202e 6373 762c 202e 7061  n read .csv, .pa
+0008e860: 7271 7565 742c 202e 7a69 702c 202e 7473  rquet, .zip, .ts
+0008e870: 2c20 616e 6420 2e78 6573 2066 696c 6520  , and .xes file 
+0008e880: 666f 726d 6174 732e 3c2f 703e 0a0a 3c2f  formats.</p>..</
+0008e890: 6469 763e 0a3c 2f64 6976 3e0a 3c2f 6469  div>.</div>.</di
+0008e8a0: 763e 0a3c 2f64 6976 3e3c 6469 7620 636c  v>.</div><div cl
+0008e8b0: 6173 733d 226a 702d 4365 6c6c 206a 702d  ass="jp-Cell jp-
+0008e8c0: 436f 6465 4365 6c6c 206a 702d 4e6f 7465  CodeCell jp-Note
+0008e8d0: 626f 6f6b 2d63 656c 6c20 6a70 2d6d 6f64  book-cell jp-mod
+0008e8e0: 2d6e 6f4f 7574 7075 7473 2020 223e 0a3c  -noOutputs  ">.<
+0008e8f0: 6469 7620 636c 6173 733d 226a 702d 4365  div class="jp-Ce
+0008e900: 6c6c 2d69 6e70 7574 5772 6170 7065 7222  ll-inputWrapper"
+0008e910: 3e0a 3c64 6976 2063 6c61 7373 3d22 6a70  >.<div class="jp
+0008e920: 2d43 6f6c 6c61 7073 6572 206a 702d 496e  -Collapser jp-In
+0008e930: 7075 7443 6f6c 6c61 7073 6572 206a 702d  putCollapser jp-
+0008e940: 4365 6c6c 2d69 6e70 7574 436f 6c6c 6170  Cell-inputCollap
+0008e950: 7365 7222 3e0a 3c2f 6469 763e 0a3c 6469  ser">.</div>.<di
+0008e960: 7620 636c 6173 733d 226a 702d 496e 7075  v class="jp-Inpu
+0008e970: 7441 7265 6120 6a70 2d43 656c 6c2d 696e  tArea jp-Cell-in
+0008e980: 7075 7441 7265 6122 3e0a 3c64 6976 2063  putArea">.<div c
+0008e990: 6c61 7373 3d22 6a70 2d49 6e70 7574 5072  lass="jp-InputPr
+0008e9a0: 6f6d 7074 206a 702d 496e 7075 7441 7265  ompt jp-InputAre
+0008e9b0: 612d 7072 6f6d 7074 223e 496e 266e 6273  a-prompt">In&nbs
+0008e9c0: 703b 5b39 5d3a 3c2f 6469 763e 0a3c 6469  p;[9]:</div>.<di
+0008e9d0: 7620 636c 6173 733d 226a 702d 436f 6465  v class="jp-Code
+0008e9e0: 4d69 7272 6f72 4564 6974 6f72 206a 702d  MirrorEditor jp-
+0008e9f0: 4564 6974 6f72 206a 702d 496e 7075 7441  Editor jp-InputA
+0008ea00: 7265 612d 6564 6974 6f72 2220 6461 7461  rea-editor" data
+0008ea10: 2d74 7970 653d 2269 6e6c 696e 6522 3e0a  -type="inline">.
+0008ea20: 2020 2020 203c 6469 7620 636c 6173 733d       <div class=
+0008ea30: 2243 6f64 654d 6972 726f 7220 636d 2d73  "CodeMirror cm-s
+0008ea40: 2d6a 7570 7974 6572 223e 0a3c 6469 7620  -jupyter">.<div 
+0008ea50: 636c 6173 733d 2220 6869 6768 6c69 6768  class=" highligh
+0008ea60: 7420 686c 2d69 7079 7468 6f6e 3322 3e3c  t hl-ipython3"><
+0008ea70: 7072 653e 3c73 7061 6e3e 3c2f 7370 616e  pre><span></span
+0008ea80: 3e3c 7370 616e 2063 6c61 7373 3d22 6b6e  ><span class="kn
+0008ea90: 223e 6672 6f6d 3c2f 7370 616e 3e20 3c73  ">from</span> <s
+0008eaa0: 7061 6e20 636c 6173 733d 226e 6e22 3e6d  pan class="nn">m
+0008eab0: 6174 6461 7461 2e64 6174 6173 6574 3c2f  atdata.dataset</
+0008eac0: 7370 616e 3e20 3c73 7061 6e20 636c 6173  span> <span clas
+0008ead0: 733d 226b 6e22 3e69 6d70 6f72 743c 2f73  s="kn">import</s
+0008eae0: 7061 6e3e 203c 7370 616e 2063 6c61 7373  pan> <span class
+0008eaf0: 3d22 6f22 3e2a 3c2f 7370 616e 3e0a 3c2f  ="o">*</span>.</
+0008eb00: 7072 653e 3c2f 6469 763e 0a0a 2020 2020  pre></div>..    
+0008eb10: 203c 2f64 6976 3e0a 3c2f 6469 763e 0a3c   </div>.</div>.<
+0008eb20: 2f64 6976 3e0a 3c2f 6469 763e 0a0a 3c2f  /div>.</div>..</
+0008eb30: 6469 763e 3c64 6976 2063 6c61 7373 3d22  div><div class="
+0008eb40: 6a70 2d43 656c 6c20 6a70 2d43 6f64 6543  jp-Cell jp-CodeC
+0008eb50: 656c 6c20 6a70 2d4e 6f74 6562 6f6f 6b2d  ell jp-Notebook-
+0008eb60: 6365 6c6c 2020 2022 3e0a 3c64 6976 2063  cell   ">.<div c
+0008eb70: 6c61 7373 3d22 6a70 2d43 656c 6c2d 696e  lass="jp-Cell-in
+0008eb80: 7075 7457 7261 7070 6572 223e 0a3c 6469  putWrapper">.<di
+0008eb90: 7620 636c 6173 733d 226a 702d 436f 6c6c  v class="jp-Coll
+0008eba0: 6170 7365 7220 6a70 2d49 6e70 7574 436f  apser jp-InputCo
+0008ebb0: 6c6c 6170 7365 7220 6a70 2d43 656c 6c2d  llapser jp-Cell-
+0008ebc0: 696e 7075 7443 6f6c 6c61 7073 6572 223e  inputCollapser">
+0008ebd0: 0a3c 2f64 6976 3e0a 3c64 6976 2063 6c61  .</div>.<div cla
+0008ebe0: 7373 3d22 6a70 2d49 6e70 7574 4172 6561  ss="jp-InputArea
+0008ebf0: 206a 702d 4365 6c6c 2d69 6e70 7574 4172   jp-Cell-inputAr
+0008ec00: 6561 223e 0a3c 6469 7620 636c 6173 733d  ea">.<div class=
+0008ec10: 226a 702d 496e 7075 7450 726f 6d70 7420  "jp-InputPrompt 
+0008ec20: 6a70 2d49 6e70 7574 4172 6561 2d70 726f  jp-InputArea-pro
+0008ec30: 6d70 7422 3e49 6e26 6e62 7370 3b5b 3130  mpt">In&nbsp;[10
+0008ec40: 5d3a 3c2f 6469 763e 0a3c 6469 7620 636c  ]:</div>.<div cl
+0008ec50: 6173 733d 226a 702d 436f 6465 4d69 7272  ass="jp-CodeMirr
+0008ec60: 6f72 4564 6974 6f72 206a 702d 4564 6974  orEditor jp-Edit
+0008ec70: 6f72 206a 702d 496e 7075 7441 7265 612d  or jp-InputArea-
+0008ec80: 6564 6974 6f72 2220 6461 7461 2d74 7970  editor" data-typ
+0008ec90: 653d 2269 6e6c 696e 6522 3e0a 2020 2020  e="inline">.    
+0008eca0: 203c 6469 7620 636c 6173 733d 2243 6f64   <div class="Cod
+0008ecb0: 654d 6972 726f 7220 636d 2d73 2d6a 7570  eMirror cm-s-jup
+0008ecc0: 7974 6572 223e 0a3c 6469 7620 636c 6173  yter">.<div clas
+0008ecd0: 733d 2220 6869 6768 6c69 6768 7420 686c  s=" highlight hl
+0008ece0: 2d69 7079 7468 6f6e 3322 3e3c 7072 653e  -ipython3"><pre>
+0008ecf0: 3c73 7061 6e3e 3c2f 7370 616e 3e3c 7370  <span></span><sp
+0008ed00: 616e 2063 6c61 7373 3d22 6e22 3e64 663c  an class="n">df<
+0008ed10: 2f73 7061 6e3e 203c 7370 616e 2063 6c61  /span> <span cla
+0008ed20: 7373 3d22 6f22 3e3d 3c2f 7370 616e 3e20  ss="o">=</span> 
+0008ed30: 3c73 7061 6e20 636c 6173 733d 226e 223e  <span class="n">
+0008ed40: 7265 6164 5f64 733c 2f73 7061 6e3e 3c73  read_ds</span><s
+0008ed50: 7061 6e20 636c 6173 733d 2270 223e 283c  pan class="p">(<
+0008ed60: 2f73 7061 6e3e 3c73 7061 6e20 636c 6173  /span><span clas
+0008ed70: 733d 2273 3122 3e26 2333 393b 6d61 7464  s="s1">&#39;matd
+0008ed80: 6174 612f 6173 7365 7473 2f73 616d 706c  ata/assets/sampl
+0008ed90: 652f 466f 7572 7371 7561 7265 5f53 616d  e/Foursquare_Sam
+0008eda0: 706c 652e 6373 7626 2333 393b 3c2f 7370  ple.csv&#39;</sp
+0008edb0: 616e 3e3c 7370 616e 2063 6c61 7373 3d22  an><span class="
+0008edc0: 7022 3e29 3c2f 7370 616e 3e0a 3c73 7061  p">)</span>.<spa
+0008edd0: 6e20 636c 6173 733d 226e 223e 6466 3c2f  n class="n">df</
+0008ede0: 7370 616e 3e3c 7370 616e 2063 6c61 7373  span><span class
+0008edf0: 3d22 6f22 3e2e 3c2f 7370 616e 3e3c 7370  ="o">.</span><sp
+0008ee00: 616e 2063 6c61 7373 3d22 6e22 3e68 6561  an class="n">hea
+0008ee10: 643c 2f73 7061 6e3e 3c73 7061 6e20 636c  d</span><span cl
+0008ee20: 6173 733d 2270 223e 2829 3c2f 7370 616e  ass="p">()</span
+0008ee30: 3e0a 3c2f 7072 653e 3c2f 6469 763e 0a0a  >.</pre></div>..
+0008ee40: 2020 2020 203c 2f64 6976 3e0a 3c2f 6469       </div>.</di
+0008ee50: 763e 0a3c 2f64 6976 3e0a 3c2f 6469 763e  v>.</div>.</div>
+0008ee60: 0a0a 3c64 6976 2063 6c61 7373 3d22 6a70  ..<div class="jp
+0008ee70: 2d43 656c 6c2d 6f75 7470 7574 5772 6170  -Cell-outputWrap
+0008ee80: 7065 7222 3e0a 3c64 6976 2063 6c61 7373  per">.<div class
+0008ee90: 3d22 6a70 2d43 6f6c 6c61 7073 6572 206a  ="jp-Collapser j
+0008eea0: 702d 4f75 7470 7574 436f 6c6c 6170 7365  p-OutputCollapse
+0008eeb0: 7220 6a70 2d43 656c 6c2d 6f75 7470 7574  r jp-Cell-output
+0008eec0: 436f 6c6c 6170 7365 7222 3e0a 3c2f 6469  Collapser">.</di
+0008eed0: 763e 0a0a 0a3c 6469 7620 636c 6173 733d  v>...<div class=
+0008eee0: 226a 702d 4f75 7470 7574 4172 6561 206a  "jp-OutputArea j
+0008eef0: 702d 4365 6c6c 2d6f 7574 7075 7441 7265  p-Cell-outputAre
+0008ef00: 6122 3e0a 0a3c 6469 7620 636c 6173 733d  a">..<div class=
+0008ef10: 226a 702d 4f75 7470 7574 4172 6561 2d63  "jp-OutputArea-c
+0008ef20: 6869 6c64 223e 0a0a 2020 2020 0a20 2020  hild">..    .   
+0008ef30: 203c 6469 7620 636c 6173 733d 226a 702d   <div class="jp-
+0008ef40: 4f75 7470 7574 5072 6f6d 7074 206a 702d  OutputPrompt jp-
+0008ef50: 4f75 7470 7574 4172 6561 2d70 726f 6d70  OutputArea-promp
+0008ef60: 7422 3e4f 7574 5b31 305d 3a3c 2f64 6976  t">Out[10]:</div
+0008ef70: 3e0a 0a0a 0a3c 6469 7620 636c 6173 733d  >....<div class=
+0008ef80: 226a 702d 5265 6e64 6572 6564 4854 4d4c  "jp-RenderedHTML
+0008ef90: 436f 6d6d 6f6e 206a 702d 5265 6e64 6572  Common jp-Render
+0008efa0: 6564 4854 4d4c 206a 702d 4f75 7470 7574  edHTML jp-Output
+0008efb0: 4172 6561 2d6f 7574 7075 7420 6a70 2d4f  Area-output jp-O
+0008efc0: 7574 7075 7441 7265 612d 6578 6563 7574  utputArea-execut
+0008efd0: 6552 6573 756c 7422 2064 6174 612d 6d69  eResult" data-mi
+0008efe0: 6d65 2d74 7970 653d 2274 6578 742f 6874  me-type="text/ht
+0008eff0: 6d6c 223e 0a3c 6469 763e 0a3c 7374 796c  ml">.<div>.<styl
+0008f000: 6520 7363 6f70 6564 3e0a 2020 2020 2e64  e scoped>.    .d
+0008f010: 6174 6166 7261 6d65 2074 626f 6479 2074  ataframe tbody t
+0008f020: 7220 7468 3a6f 6e6c 792d 6f66 2d74 7970  r th:only-of-typ
+0008f030: 6520 7b0a 2020 2020 2020 2020 7665 7274  e {.        vert
+0008f040: 6963 616c 2d61 6c69 676e 3a20 6d69 6464  ical-align: midd
+0008f050: 6c65 3b0a 2020 2020 7d0a 0a20 2020 202e  le;.    }..    .
+0008f060: 6461 7461 6672 616d 6520 7462 6f64 7920  dataframe tbody 
+0008f070: 7472 2074 6820 7b0a 2020 2020 2020 2020  tr th {.        
+0008f080: 7665 7274 6963 616c 2d61 6c69 676e 3a20  vertical-align: 
+0008f090: 746f 703b 0a20 2020 207d 0a0a 2020 2020  top;.    }..    
+0008f0a0: 2e64 6174 6166 7261 6d65 2074 6865 6164  .dataframe thead
+0008f0b0: 2074 6820 7b0a 2020 2020 2020 2020 7465   th {.        te
+0008f0c0: 7874 2d61 6c69 676e 3a20 7269 6768 743b  xt-align: right;
+0008f0d0: 0a20 2020 207d 0a3c 2f73 7479 6c65 3e0a  .    }.</style>.
+0008f0e0: 3c74 6162 6c65 2062 6f72 6465 723d 2231  <table border="1
+0008f0f0: 2220 636c 6173 733d 2264 6174 6166 7261  " class="datafra
+0008f100: 6d65 223e 0a20 203c 7468 6561 643e 0a20  me">.  <thead>. 
+0008f110: 2020 203c 7472 2073 7479 6c65 3d22 7465     <tr style="te
+0008f120: 7874 2d61 6c69 676e 3a20 7269 6768 743b  xt-align: right;
+0008f130: 223e 0a20 2020 2020 203c 7468 3e3c 2f74  ">.      <th></t
+0008f140: 683e 0a20 2020 2020 203c 7468 3e6c 6174  h>.      <th>lat
+0008f150: 5f6c 6f6e 3c2f 7468 3e0a 2020 2020 2020  _lon</th>.      
+0008f160: 3c74 683e 6461 7465 5f74 696d 653c 2f74  <th>date_time</t
+0008f170: 683e 0a20 2020 2020 203c 7468 3e74 696d  h>.      <th>tim
+0008f180: 653c 2f74 683e 0a20 2020 2020 203c 7468  e</th>.      <th
+0008f190: 3e72 6174 696e 673c 2f74 683e 0a20 2020  >rating</th>.   
+0008f1a0: 2020 203c 7468 3e70 7269 6365 3c2f 7468     <th>price</th
+0008f1b0: 3e0a 2020 2020 2020 3c74 683e 7765 6174  >.      <th>weat
+0008f1c0: 6865 723c 2f74 683e 0a20 2020 2020 203c  her</th>.      <
+0008f1d0: 7468 3e64 6179 3c2f 7468 3e0a 2020 2020  th>day</th>.    
+0008f1e0: 2020 3c74 683e 726f 6f74 5f74 7970 653c    <th>root_type<
+0008f1f0: 2f74 683e 0a20 2020 2020 203c 7468 3e74  /th>.      <th>t
+0008f200: 7970 653c 2f74 683e 0a20 2020 2020 203c  ype</th>.      <
+0008f210: 7468 3e74 6964 3c2f 7468 3e0a 2020 2020  th>tid</th>.    
+0008f220: 3c2f 7472 3e0a 2020 3c2f 7468 6561 643e  </tr>.  </thead>
+0008f230: 0a20 203c 7462 6f64 793e 0a20 2020 203c  .  <tbody>.    <
+0008f240: 7472 3e0a 2020 2020 2020 3c74 683e 303c  tr>.      <th>0<
+0008f250: 2f74 683e 0a20 2020 2020 203c 7464 3e34  /th>.      <td>4
+0008f260: 302e 3833 3331 3635 3230 3036 3232 3420  0.8331652006224 
+0008f270: 2d37 332e 3934 3138 3630 3334 3237 3639  -73.941860342769
+0008f280: 323c 2f74 643e 0a20 2020 2020 203c 7464  2</td>.      <td
+0008f290: 3e32 3031 322d 3131 2d31 3220 3035 3a31  >2012-11-12 05:1
+0008f2a0: 373a 3138 3c2f 7464 3e0a 2020 2020 2020  7:18</td>.      
+0008f2b0: 3c74 643e 3331 373c 2f74 643e 0a20 2020  <td>317</td>.   
+0008f2c0: 2020 203c 7464 3e2d 312e 303c 2f74 643e     <td>-1.0</td>
+0008f2d0: 0a20 2020 2020 203c 7464 3e2d 313c 2f74  .      <td>-1</t
+0008f2e0: 643e 0a20 2020 2020 203c 7464 3e43 6c65  d>.      <td>Cle
+0008f2f0: 6172 3c2f 7464 3e0a 2020 2020 2020 3c74  ar</td>.      <t
+0008f300: 643e 4d6f 6e64 6179 3c2f 7464 3e0a 2020  d>Monday</td>.  
+0008f310: 2020 2020 3c74 643e 5265 7369 6465 6e63      <td>Residenc
+0008f320: 653c 2f74 643e 0a20 2020 2020 203c 7464  e</td>.      <td
+0008f330: 3e48 6f6d 6520 2870 7269 7661 7465 293c  >Home (private)<
+0008f340: 2f74 643e 0a20 2020 2020 203c 7464 3e31  /td>.      <td>1
+0008f350: 3236 3c2f 7464 3e0a 2020 2020 3c2f 7472  26</td>.    </tr
+0008f360: 3e0a 2020 2020 3c74 723e 0a20 2020 2020  >.    <tr>.     
+0008f370: 203c 7468 3e31 3c2f 7468 3e0a 2020 2020   <th>1</th>.    
+0008f380: 2020 3c74 643e 3430 2e38 3334 3039 3738    <td>40.8340978
+0008f390: 3034 3130 3732 202d 3733 2e39 3435 3236  041072 -73.94526
+0008f3a0: 3732 3232 3538 3831 3c2f 7464 3e0a 2020  72225881</td>.  
+0008f3b0: 2020 2020 3c74 643e 3230 3132 2d31 312d      <td>2012-11-
+0008f3c0: 3132 2032 333a 3234 3a35 353c 2f74 643e  12 23:24:55</td>
+0008f3d0: 0a20 2020 2020 203c 7464 3e31 3430 343c  .      <td>1404<
+0008f3e0: 2f74 643e 0a20 2020 2020 203c 7464 3e38  /td>.      <td>8
+0008f3f0: 2e32 3c2f 7464 3e0a 2020 2020 2020 3c74  .2</td>.      <t
+0008f400: 643e 313c 2f74 643e 0a20 2020 2020 203c  d>1</td>.      <
+0008f410: 7464 3e43 6c6f 7564 733c 2f74 643e 0a20  td>Clouds</td>. 
+0008f420: 2020 2020 203c 7464 3e4d 6f6e 6461 793c       <td>Monday<
+0008f430: 2f74 643e 0a20 2020 2020 203c 7464 3e46  /td>.      <td>F
+0008f440: 6f6f 643c 2f74 643e 0a20 2020 2020 203c  ood</td>.      <
+0008f450: 7464 3e44 656c 6920 2f20 426f 6465 6761  td>Deli / Bodega
+0008f460: 3c2f 7464 3e0a 2020 2020 2020 3c74 643e  </td>.      <td>
+0008f470: 3132 363c 2f74 643e 0a20 2020 203c 2f74  126</td>.    </t
+0008f480: 723e 0a20 2020 203c 7472 3e0a 2020 2020  r>.    <tr>.    
+0008f490: 2020 3c74 683e 323c 2f74 683e 0a20 2020    <th>2</th>.   
+0008f4a0: 2020 203c 7464 3e34 302e 3833 3331 3635     <td>40.833165
+0008f4b0: 3230 3036 3232 3420 2d37 332e 3934 3138  2006224 -73.9418
+0008f4c0: 3630 3334 3237 3639 323c 2f74 643e 0a20  603427692</td>. 
+0008f4d0: 2020 2020 203c 7464 3e32 3031 322d 3131       <td>2012-11
+0008f4e0: 2d31 3320 3030 3a30 303a 3037 3c2f 7464  -13 00:00:07</td
+0008f4f0: 3e0a 2020 2020 2020 3c74 643e 303c 2f74  >.      <td>0</t
+0008f500: 643e 0a20 2020 2020 203c 7464 3e2d 312e  d>.      <td>-1.
+0008f510: 303c 2f74 643e 0a20 2020 2020 203c 7464  0</td>.      <td
+0008f520: 3e2d 313c 2f74 643e 0a20 2020 2020 203c  >-1</td>.      <
+0008f530: 7464 3e43 6c6f 7564 733c 2f74 643e 0a20  td>Clouds</td>. 
+0008f540: 2020 2020 203c 7464 3e54 7565 7364 6179       <td>Tuesday
+0008f550: 3c2f 7464 3e0a 2020 2020 2020 3c74 643e  </td>.      <td>
+0008f560: 5265 7369 6465 6e63 653c 2f74 643e 0a20  Residence</td>. 
+0008f570: 2020 2020 203c 7464 3e48 6f6d 6520 2870       <td>Home (p
+0008f580: 7269 7661 7465 293c 2f74 643e 0a20 2020  rivate)</td>.   
+0008f590: 2020 203c 7464 3e31 3236 3c2f 7464 3e0a     <td>126</td>.
+0008f5a0: 2020 2020 3c2f 7472 3e0a 2020 2020 3c74      </tr>.    <t
+0008f5b0: 723e 0a20 2020 2020 203c 7468 3e33 3c2f  r>.      <th>3</
+0008f5c0: 7468 3e0a 2020 2020 2020 3c74 643e 3430  th>.      <td>40
+0008f5d0: 2e37 3634 3639 3539 3238 3332 3534 202d  .7646959283254 -
+0008f5e0: 3733 2e38 3835 3139 3734 3936 3434 3134  73.8851974964414
+0008f5f0: 3c2f 7464 3e0a 2020 2020 2020 3c74 643e  </td>.      <td>
+0008f600: 3230 3132 2d31 312d 3135 2031 373a 3439  2012-11-15 17:49
+0008f610: 3a30 313c 2f74 643e 0a20 2020 2020 203c  :01</td>.      <
+0008f620: 7464 3e31 3036 393c 2f74 643e 0a20 2020  td>1069</td>.   
+0008f630: 2020 203c 7464 3e36 2e36 3c2f 7464 3e0a     <td>6.6</td>.
+0008f640: 2020 2020 2020 3c74 643e 333c 2f74 643e        <td>3</td>
+0008f650: 0a20 2020 2020 203c 7464 3e43 6c65 6172  .      <td>Clear
+0008f660: 3c2f 7464 3e0a 2020 2020 2020 3c74 643e  </td>.      <td>
+0008f670: 5468 7572 7364 6179 3c2f 7464 3e0a 2020  Thursday</td>.  
+0008f680: 2020 2020 3c74 643e 466f 6f64 3c2f 7464      <td>Food</td
+0008f690: 3e0a 2020 2020 2020 3c74 643e 4672 6965  >.      <td>Frie
+0008f6a0: 6420 4368 6963 6b65 6e20 4a6f 696e 743c  d Chicken Joint<
+0008f6b0: 2f74 643e 0a20 2020 2020 203c 7464 3e31  /td>.      <td>1
+0008f6c0: 3236 3c2f 7464 3e0a 2020 2020 3c2f 7472  26</td>.    </tr
+0008f6d0: 3e0a 2020 2020 3c74 723e 0a20 2020 2020  >.    <tr>.     
+0008f6e0: 203c 7468 3e34 3c2f 7468 3e0a 2020 2020   <th>4</th>.    
+0008f6f0: 2020 3c74 643e 3430 2e37 3636 3037 3930    <td>40.7660790
+0008f700: 3337 3638 3234 202d 3733 2e38 3833 3532  376824 -73.88352
+0008f710: 3837 3039 3431 3136 3c2f 7464 3e0a 2020  87094116</td>.  
+0008f720: 2020 2020 3c74 643e 3230 3132 2d31 312d      <td>2012-11-
+0008f730: 3135 2031 383a 3430 3a31 363c 2f74 643e  15 18:40:16</td>
+0008f740: 0a20 2020 2020 203c 7464 3e31 3132 303c  .      <td>1120<
+0008f750: 2f74 643e 0a20 2020 2020 203c 7464 3e2d  /td>.      <td>-
+0008f760: 312e 303c 2f74 643e 0a20 2020 2020 203c  1.0</td>.      <
+0008f770: 7464 3e2d 313c 2f74 643e 0a20 2020 2020  td>-1</td>.     
+0008f780: 203c 7464 3e43 6c65 6172 3c2f 7464 3e0a   <td>Clear</td>.
+0008f790: 2020 2020 2020 3c74 643e 5468 7572 7364        <td>Thursd
+0008f7a0: 6179 3c2f 7464 3e0a 2020 2020 2020 3c74  ay</td>.      <t
+0008f7b0: 643e 5472 6176 656c 2026 616d 703b 2054  d>Travel &amp; T
+0008f7c0: 7261 6e73 706f 7274 3c2f 7464 3e0a 2020  ransport</td>.  
+0008f7d0: 2020 2020 3c74 643e 4275 7320 5374 6174      <td>Bus Stat
+0008f7e0: 696f 6e3c 2f74 643e 0a20 2020 2020 203c  ion</td>.      <
+0008f7f0: 7464 3e31 3236 3c2f 7464 3e0a 2020 2020  td>126</td>.    
+0008f800: 3c2f 7472 3e0a 2020 3c2f 7462 6f64 793e  </tr>.  </tbody>
+0008f810: 0a3c 2f74 6162 6c65 3e0a 3c2f 6469 763e  .</table>.</div>
+0008f820: 0a3c 2f64 6976 3e0a 0a3c 2f64 6976 3e0a  .</div>..</div>.
+0008f830: 0a3c 2f64 6976 3e0a 0a3c 2f64 6976 3e0a  .</div>..</div>.
+0008f840: 0a3c 2f64 6976 3e0a 3c64 6976 2063 6c61  .</div>.<div cla
+0008f850: 7373 3d22 6a70 2d43 656c 6c20 6a70 2d4d  ss="jp-Cell jp-M
+0008f860: 6172 6b64 6f77 6e43 656c 6c20 6a70 2d4e  arkdownCell jp-N
+0008f870: 6f74 6562 6f6f 6b2d 6365 6c6c 223e 0a3c  otebook-cell">.<
+0008f880: 6469 7620 636c 6173 733d 226a 702d 4365  div class="jp-Ce
+0008f890: 6c6c 2d69 6e70 7574 5772 6170 7065 7222  ll-inputWrapper"
+0008f8a0: 3e0a 3c64 6976 2063 6c61 7373 3d22 6a70  >.<div class="jp
+0008f8b0: 2d43 6f6c 6c61 7073 6572 206a 702d 496e  -Collapser jp-In
+0008f8c0: 7075 7443 6f6c 6c61 7073 6572 206a 702d  putCollapser jp-
+0008f8d0: 4365 6c6c 2d69 6e70 7574 436f 6c6c 6170  Cell-inputCollap
+0008f8e0: 7365 7222 3e0a 3c2f 6469 763e 0a3c 6469  ser">.</div>.<di
+0008f8f0: 7620 636c 6173 733d 226a 702d 496e 7075  v class="jp-Inpu
+0008f900: 7441 7265 6120 6a70 2d43 656c 6c2d 696e  tArea jp-Cell-in
+0008f910: 7075 7441 7265 6122 3e3c 6469 7620 636c  putArea"><div cl
+0008f920: 6173 733d 226a 702d 496e 7075 7450 726f  ass="jp-InputPro
+0008f930: 6d70 7420 6a70 2d49 6e70 7574 4172 6561  mpt jp-InputArea
+0008f940: 2d70 726f 6d70 7422 3e0a 3c2f 6469 763e  -prompt">.</div>
+0008f950: 3c64 6976 2063 6c61 7373 3d22 6a70 2d52  <div class="jp-R
+0008f960: 656e 6465 7265 6448 544d 4c43 6f6d 6d6f  enderedHTMLCommo
+0008f970: 6e20 6a70 2d52 656e 6465 7265 644d 6172  n jp-RenderedMar
+0008f980: 6b64 6f77 6e20 6a70 2d4d 6172 6b64 6f77  kdown jp-Markdow
+0008f990: 6e4f 7574 7075 7420 2220 6461 7461 2d6d  nOutput " data-m
+0008f9a0: 696d 652d 7479 7065 3d22 7465 7874 2f6d  ime-type="text/m
+0008f9b0: 6172 6b64 6f77 6e22 3e0a 3c70 3e4f 7074  arkdown">.<p>Opt
+0008f9c0: 696f 6e61 6c6c 792c 2079 6f75 2063 616e  ionally, you can
+0008f9d0: 2075 7365 2074 6865 2073 7461 6e64 6172   use the standar
+0008f9e0: 6469 7a65 6420 7265 6164 696e 672c 2077  dized reading, w
+0008f9f0: 6869 6368 2077 696c 6c20 6d61 6b65 2027  hich will make '
+0008fa00: 7469 6427 2f27 6c61 6265 6c27 206e 6f6d  tid'/'label' nom
+0008fa10: 656e 636c 6174 7572 6520 286f 7220 7265  enclature (or re
+0008fa20: 6e61 6d65 2063 6f6c 756d 6e73 2920 616e  name columns) an
+0008fa30: 6420 7769 6c6c 2073 6f72 7420 7468 6520  d will sort the 
+0008fa40: 7472 616a 6563 746f 7269 6573 3c2f 703e  trajectories</p>
+0008fa50: 0a0a 3c2f 6469 763e 0a3c 2f64 6976 3e0a  ..</div>.</div>.
+0008fa60: 3c2f 6469 763e 0a3c 2f64 6976 3e3c 6469  </div>.</div><di
+0008fa70: 7620 636c 6173 733d 226a 702d 4365 6c6c  v class="jp-Cell
+0008fa80: 206a 702d 436f 6465 4365 6c6c 206a 702d   jp-CodeCell jp-
+0008fa90: 4e6f 7465 626f 6f6b 2d63 656c 6c20 2020  Notebook-cell   
+0008faa0: 223e 0a3c 6469 7620 636c 6173 733d 226a  ">.<div class="j
+0008fab0: 702d 4365 6c6c 2d69 6e70 7574 5772 6170  p-Cell-inputWrap
+0008fac0: 7065 7222 3e0a 3c64 6976 2063 6c61 7373  per">.<div class
+0008fad0: 3d22 6a70 2d43 6f6c 6c61 7073 6572 206a  ="jp-Collapser j
+0008fae0: 702d 496e 7075 7443 6f6c 6c61 7073 6572  p-InputCollapser
+0008faf0: 206a 702d 4365 6c6c 2d69 6e70 7574 436f   jp-Cell-inputCo
+0008fb00: 6c6c 6170 7365 7222 3e0a 3c2f 6469 763e  llapser">.</div>
+0008fb10: 0a3c 6469 7620 636c 6173 733d 226a 702d  .<div class="jp-
+0008fb20: 496e 7075 7441 7265 6120 6a70 2d43 656c  InputArea jp-Cel
+0008fb30: 6c2d 696e 7075 7441 7265 6122 3e0a 3c64  l-inputArea">.<d
+0008fb40: 6976 2063 6c61 7373 3d22 6a70 2d49 6e70  iv class="jp-Inp
+0008fb50: 7574 5072 6f6d 7074 206a 702d 496e 7075  utPrompt jp-Inpu
+0008fb60: 7441 7265 612d 7072 6f6d 7074 223e 496e  tArea-prompt">In
+0008fb70: 266e 6273 703b 5b31 315d 3a3c 2f64 6976  &nbsp;[11]:</div
+0008fb80: 3e0a 3c64 6976 2063 6c61 7373 3d22 6a70  >.<div class="jp
+0008fb90: 2d43 6f64 654d 6972 726f 7245 6469 746f  -CodeMirrorEdito
+0008fba0: 7220 6a70 2d45 6469 746f 7220 6a70 2d49  r jp-Editor jp-I
+0008fbb0: 6e70 7574 4172 6561 2d65 6469 746f 7222  nputArea-editor"
+0008fbc0: 2064 6174 612d 7479 7065 3d22 696e 6c69   data-type="inli
+0008fbd0: 6e65 223e 0a20 2020 2020 3c64 6976 2063  ne">.     <div c
+0008fbe0: 6c61 7373 3d22 436f 6465 4d69 7272 6f72  lass="CodeMirror
+0008fbf0: 2063 6d2d 732d 6a75 7079 7465 7222 3e0a   cm-s-jupyter">.
+0008fc00: 3c64 6976 2063 6c61 7373 3d22 2068 6967  <div class=" hig
+0008fc10: 686c 6967 6874 2068 6c2d 6970 7974 686f  hlight hl-ipytho
+0008fc20: 6e33 223e 3c70 7265 3e3c 7370 616e 3e3c  n3"><pre><span><
+0008fc30: 2f73 7061 6e3e 3c73 7061 6e20 636c 6173  /span><span clas
+0008fc40: 733d 226e 223e 6466 3c2f 7370 616e 3e20  s="n">df</span> 
+0008fc50: 3c73 7061 6e20 636c 6173 733d 226f 223e  <span class="o">
+0008fc60: 3d3c 2f73 7061 6e3e 203c 7370 616e 2063  =</span> <span c
+0008fc70: 6c61 7373 3d22 6e22 3e72 6561 645f 6473  lass="n">read_ds
+0008fc80: 3c2f 7370 616e 3e3c 7370 616e 2063 6c61  </span><span cla
+0008fc90: 7373 3d22 7022 3e28 3c2f 7370 616e 3e3c  ss="p">(</span><
+0008fca0: 7370 616e 2063 6c61 7373 3d22 7331 223e  span class="s1">
+0008fcb0: 2623 3339 3b6d 6174 6461 7461 2f61 7373  &#39;matdata/ass
+0008fcc0: 6574 732f 7361 6d70 6c65 2f46 6f75 7273  ets/sample/Fours
+0008fcd0: 7175 6172 655f 5361 6d70 6c65 2e63 7376  quare_Sample.csv
+0008fce0: 2623 3339 3b3c 2f73 7061 6e3e 3c73 7061  &#39;</span><spa
+0008fcf0: 6e20 636c 6173 733d 2270 223e 2c3c 2f73  n class="p">,</s
+0008fd00: 7061 6e3e 203c 7370 616e 2063 6c61 7373  pan> <span class
+0008fd10: 3d22 6e22 3e74 6964 5f63 6f6c 3c2f 7370  ="n">tid_col</sp
+0008fd20: 616e 3e3c 7370 616e 2063 6c61 7373 3d22  an><span class="
+0008fd30: 6f22 3e3d 3c2f 7370 616e 3e3c 7370 616e  o">=</span><span
+0008fd40: 2063 6c61 7373 3d22 7331 223e 2623 3339   class="s1">&#39
+0008fd50: 3b74 6964 2623 3339 3b3c 2f73 7061 6e3e  ;tid&#39;</span>
+0008fd60: 3c73 7061 6e20 636c 6173 733d 2270 223e  <span class="p">
+0008fd70: 2c3c 2f73 7061 6e3e 203c 7370 616e 2063  ,</span> <span c
+0008fd80: 6c61 7373 3d22 6e22 3e63 6c61 7373 5f63  lass="n">class_c
+0008fd90: 6f6c 3c2f 7370 616e 3e3c 7370 616e 2063  ol</span><span c
+0008fda0: 6c61 7373 3d22 6f22 3e3d 3c2f 7370 616e  lass="o">=</span
+0008fdb0: 3e3c 7370 616e 2063 6c61 7373 3d22 7331  ><span class="s1
+0008fdc0: 223e 2623 3339 3b72 6f6f 745f 7479 7065  ">&#39;root_type
+0008fdd0: 2623 3339 3b3c 2f73 7061 6e3e 3c73 7061  &#39;</span><spa
+0008fde0: 6e20 636c 6173 733d 2270 223e 293c 2f73  n class="p">)</s
+0008fdf0: 7061 6e3e 0a3c 7370 616e 2063 6c61 7373  pan>.<span class
+0008fe00: 3d22 6e22 3e64 663c 2f73 7061 6e3e 3c73  ="n">df</span><s
+0008fe10: 7061 6e20 636c 6173 733d 226f 223e 2e3c  pan class="o">.<
+0008fe20: 2f73 7061 6e3e 3c73 7061 6e20 636c 6173  /span><span clas
+0008fe30: 733d 226e 223e 6865 6164 3c2f 7370 616e  s="n">head</span
+0008fe40: 3e3c 7370 616e 2063 6c61 7373 3d22 7022  ><span class="p"
+0008fe50: 3e28 293c 2f73 7061 6e3e 0a3c 2f70 7265  >()</span>.</pre
+0008fe60: 3e3c 2f64 6976 3e0a 0a20 2020 2020 3c2f  ></div>..     </
+0008fe70: 6469 763e 0a3c 2f64 6976 3e0a 3c2f 6469  div>.</div>.</di
+0008fe80: 763e 0a3c 2f64 6976 3e0a 0a3c 6469 7620  v>.</div>..<div 
+0008fe90: 636c 6173 733d 226a 702d 4365 6c6c 2d6f  class="jp-Cell-o
+0008fea0: 7574 7075 7457 7261 7070 6572 223e 0a3c  utputWrapper">.<
+0008feb0: 6469 7620 636c 6173 733d 226a 702d 436f  div class="jp-Co
+0008fec0: 6c6c 6170 7365 7220 6a70 2d4f 7574 7075  llapser jp-Outpu
+0008fed0: 7443 6f6c 6c61 7073 6572 206a 702d 4365  tCollapser jp-Ce
+0008fee0: 6c6c 2d6f 7574 7075 7443 6f6c 6c61 7073  ll-outputCollaps
+0008fef0: 6572 223e 0a3c 2f64 6976 3e0a 0a0a 3c64  er">.</div>...<d
+0008ff00: 6976 2063 6c61 7373 3d22 6a70 2d4f 7574  iv class="jp-Out
+0008ff10: 7075 7441 7265 6120 6a70 2d43 656c 6c2d  putArea jp-Cell-
+0008ff20: 6f75 7470 7574 4172 6561 223e 0a0a 3c64  outputArea">..<d
+0008ff30: 6976 2063 6c61 7373 3d22 6a70 2d4f 7574  iv class="jp-Out
+0008ff40: 7075 7441 7265 612d 6368 696c 6422 3e0a  putArea-child">.
+0008ff50: 0a20 2020 200a 2020 2020 3c64 6976 2063  .    .    <div c
+0008ff60: 6c61 7373 3d22 6a70 2d4f 7574 7075 7450  lass="jp-OutputP
+0008ff70: 726f 6d70 7420 6a70 2d4f 7574 7075 7441  rompt jp-OutputA
+0008ff80: 7265 612d 7072 6f6d 7074 223e 4f75 745b  rea-prompt">Out[
+0008ff90: 3131 5d3a 3c2f 6469 763e 0a0a 0a0a 3c64  11]:</div>....<d
+0008ffa0: 6976 2063 6c61 7373 3d22 6a70 2d52 656e  iv class="jp-Ren
+0008ffb0: 6465 7265 6448 544d 4c43 6f6d 6d6f 6e20  deredHTMLCommon 
+0008ffc0: 6a70 2d52 656e 6465 7265 6448 544d 4c20  jp-RenderedHTML 
+0008ffd0: 6a70 2d4f 7574 7075 7441 7265 612d 6f75  jp-OutputArea-ou
+0008ffe0: 7470 7574 206a 702d 4f75 7470 7574 4172  tput jp-OutputAr
+0008fff0: 6561 2d65 7865 6375 7465 5265 7375 6c74  ea-executeResult
+00090000: 2220 6461 7461 2d6d 696d 652d 7479 7065  " data-mime-type
+00090010: 3d22 7465 7874 2f68 746d 6c22 3e0a 3c64  ="text/html">.<d
+00090020: 6976 3e0a 3c73 7479 6c65 2073 636f 7065  iv>.<style scope
+00090030: 643e 0a20 2020 202e 6461 7461 6672 616d  d>.    .datafram
+00090040: 6520 7462 6f64 7920 7472 2074 683a 6f6e  e tbody tr th:on
+00090050: 6c79 2d6f 662d 7479 7065 207b 0a20 2020  ly-of-type {.   
+00090060: 2020 2020 2076 6572 7469 6361 6c2d 616c       vertical-al
+00090070: 6967 6e3a 206d 6964 646c 653b 0a20 2020  ign: middle;.   
+00090080: 207d 0a0a 2020 2020 2e64 6174 6166 7261   }..    .datafra
+00090090: 6d65 2074 626f 6479 2074 7220 7468 207b  me tbody tr th {
+000900a0: 0a20 2020 2020 2020 2076 6572 7469 6361  .        vertica
+000900b0: 6c2d 616c 6967 6e3a 2074 6f70 3b0a 2020  l-align: top;.  
+000900c0: 2020 7d0a 0a20 2020 202e 6461 7461 6672    }..    .datafr
+000900d0: 616d 6520 7468 6561 6420 7468 207b 0a20  ame thead th {. 
+000900e0: 2020 2020 2020 2074 6578 742d 616c 6967         text-alig
+000900f0: 6e3a 2072 6967 6874 3b0a 2020 2020 7d0a  n: right;.    }.
+00090100: 3c2f 7374 796c 653e 0a3c 7461 626c 6520  </style>.<table 
+00090110: 626f 7264 6572 3d22 3122 2063 6c61 7373  border="1" class
+00090120: 3d22 6461 7461 6672 616d 6522 3e0a 2020  ="dataframe">.  
+00090130: 3c74 6865 6164 3e0a 2020 2020 3c74 7220  <thead>.    <tr 
+00090140: 7374 796c 653d 2274 6578 742d 616c 6967  style="text-alig
+00090150: 6e3a 2072 6967 6874 3b22 3e0a 2020 2020  n: right;">.    
+00090160: 2020 3c74 683e 3c2f 7468 3e0a 2020 2020    <th></th>.    
+00090170: 2020 3c74 683e 6c61 745f 6c6f 6e3c 2f74    <th>lat_lon</t
+00090180: 683e 0a20 2020 2020 203c 7468 3e64 6174  h>.      <th>dat
+00090190: 655f 7469 6d65 3c2f 7468 3e0a 2020 2020  e_time</th>.    
+000901a0: 2020 3c74 683e 7469 6d65 3c2f 7468 3e0a    <th>time</th>.
+000901b0: 2020 2020 2020 3c74 683e 7261 7469 6e67        <th>rating
+000901c0: 3c2f 7468 3e0a 2020 2020 2020 3c74 683e  </th>.      <th>
+000901d0: 7072 6963 653c 2f74 683e 0a20 2020 2020  price</th>.     
+000901e0: 203c 7468 3e77 6561 7468 6572 3c2f 7468   <th>weather</th
+000901f0: 3e0a 2020 2020 2020 3c74 683e 6461 793c  >.      <th>day<
+00090200: 2f74 683e 0a20 2020 2020 203c 7468 3e74  /th>.      <th>t
+00090210: 7970 653c 2f74 683e 0a20 2020 2020 203c  ype</th>.      <
+00090220: 7468 3e74 6964 3c2f 7468 3e0a 2020 2020  th>tid</th>.    
+00090230: 2020 3c74 683e 6c61 6265 6c3c 2f74 683e    <th>label</th>
+00090240: 0a20 2020 203c 2f74 723e 0a20 203c 2f74  .    </tr>.  </t
+00090250: 6865 6164 3e0a 2020 3c74 626f 6479 3e0a  head>.  <tbody>.
+00090260: 2020 2020 3c74 723e 0a20 2020 2020 203c      <tr>.      <
+00090270: 7468 3e30 3c2f 7468 3e0a 2020 2020 2020  th>0</th>.      
+00090280: 3c74 643e 3430 2e38 3333 3136 3532 3030  <td>40.833165200
+00090290: 3632 3234 202d 3733 2e39 3431 3836 3033  6224 -73.9418603
+000902a0: 3432 3736 3932 3c2f 7464 3e0a 2020 2020  427692</td>.    
+000902b0: 2020 3c74 643e 3230 3132 2d31 312d 3132    <td>2012-11-12
+000902c0: 2030 353a 3137 3a31 383c 2f74 643e 0a20   05:17:18</td>. 
+000902d0: 2020 2020 203c 7464 3e33 3137 3c2f 7464       <td>317</td
+000902e0: 3e0a 2020 2020 2020 3c74 643e 2d31 2e30  >.      <td>-1.0
+000902f0: 3c2f 7464 3e0a 2020 2020 2020 3c74 643e  </td>.      <td>
+00090300: 2d31 3c2f 7464 3e0a 2020 2020 2020 3c74  -1</td>.      <t
+00090310: 643e 436c 6561 723c 2f74 643e 0a20 2020  d>Clear</td>.   
+00090320: 2020 203c 7464 3e4d 6f6e 6461 793c 2f74     <td>Monday</t
+00090330: 643e 0a20 2020 2020 203c 7464 3e48 6f6d  d>.      <td>Hom
+00090340: 6520 2870 7269 7661 7465 293c 2f74 643e  e (private)</td>
+00090350: 0a20 2020 2020 203c 7464 3e31 3236 3c2f  .      <td>126</
+00090360: 7464 3e0a 2020 2020 2020 3c74 643e 5265  td>.      <td>Re
+00090370: 7369 6465 6e63 653c 2f74 643e 0a20 2020  sidence</td>.   
+00090380: 203c 2f74 723e 0a20 2020 203c 7472 3e0a   </tr>.    <tr>.
+00090390: 2020 2020 2020 3c74 683e 313c 2f74 683e        <th>1</th>
+000903a0: 0a20 2020 2020 203c 7464 3e34 302e 3833  .      <td>40.83
+000903b0: 3430 3937 3830 3431 3037 3220 2d37 332e  40978041072 -73.
+000903c0: 3934 3532 3637 3232 3235 3838 313c 2f74  9452672225881</t
+000903d0: 643e 0a20 2020 2020 203c 7464 3e32 3031  d>.      <td>201
+000903e0: 322d 3131 2d31 3220 3233 3a32 343a 3535  2-11-12 23:24:55
+000903f0: 3c2f 7464 3e0a 2020 2020 2020 3c74 643e  </td>.      <td>
+00090400: 3134 3034 3c2f 7464 3e0a 2020 2020 2020  1404</td>.      
+00090410: 3c74 643e 382e 323c 2f74 643e 0a20 2020  <td>8.2</td>.   
+00090420: 2020 203c 7464 3e31 3c2f 7464 3e0a 2020     <td>1</td>.  
+00090430: 2020 2020 3c74 643e 436c 6f75 6473 3c2f      <td>Clouds</
+00090440: 7464 3e0a 2020 2020 2020 3c74 643e 4d6f  td>.      <td>Mo
+00090450: 6e64 6179 3c2f 7464 3e0a 2020 2020 2020  nday</td>.      
+00090460: 3c74 643e 4465 6c69 202f 2042 6f64 6567  <td>Deli / Bodeg
+00090470: 613c 2f74 643e 0a20 2020 2020 203c 7464  a</td>.      <td
+00090480: 3e31 3236 3c2f 7464 3e0a 2020 2020 2020  >126</td>.      
+00090490: 3c74 643e 466f 6f64 3c2f 7464 3e0a 2020  <td>Food</td>.  
+000904a0: 2020 3c2f 7472 3e0a 2020 2020 3c74 723e    </tr>.    <tr>
+000904b0: 0a20 2020 2020 203c 7468 3e32 3c2f 7468  .      <th>2</th
+000904c0: 3e0a 2020 2020 2020 3c74 643e 3430 2e38  >.      <td>40.8
+000904d0: 3333 3136 3532 3030 3632 3234 202d 3733  331652006224 -73
+000904e0: 2e39 3431 3836 3033 3432 3736 3932 3c2f  .9418603427692</
+000904f0: 7464 3e0a 2020 2020 2020 3c74 643e 3230  td>.      <td>20
+00090500: 3132 2d31 312d 3133 2030 303a 3030 3a30  12-11-13 00:00:0
+00090510: 373c 2f74 643e 0a20 2020 2020 203c 7464  7</td>.      <td
+00090520: 3e30 3c2f 7464 3e0a 2020 2020 2020 3c74  >0</td>.      <t
+00090530: 643e 2d31 2e30 3c2f 7464 3e0a 2020 2020  d>-1.0</td>.    
+00090540: 2020 3c74 643e 2d31 3c2f 7464 3e0a 2020    <td>-1</td>.  
+00090550: 2020 2020 3c74 643e 436c 6f75 6473 3c2f      <td>Clouds</
+00090560: 7464 3e0a 2020 2020 2020 3c74 643e 5475  td>.      <td>Tu
+00090570: 6573 6461 793c 2f74 643e 0a20 2020 2020  esday</td>.     
+00090580: 203c 7464 3e48 6f6d 6520 2870 7269 7661   <td>Home (priva
+00090590: 7465 293c 2f74 643e 0a20 2020 2020 203c  te)</td>.      <
+000905a0: 7464 3e31 3236 3c2f 7464 3e0a 2020 2020  td>126</td>.    
+000905b0: 2020 3c74 643e 5265 7369 6465 6e63 653c    <td>Residence<
+000905c0: 2f74 643e 0a20 2020 203c 2f74 723e 0a20  /td>.    </tr>. 
+000905d0: 2020 203c 7472 3e0a 2020 2020 2020 3c74     <tr>.      <t
+000905e0: 683e 333c 2f74 683e 0a20 2020 2020 203c  h>3</th>.      <
+000905f0: 7464 3e34 302e 3736 3436 3935 3932 3833  td>40.7646959283
+00090600: 3235 3420 2d37 332e 3838 3531 3937 3439  254 -73.88519749
+00090610: 3634 3431 343c 2f74 643e 0a20 2020 2020  64414</td>.     
+00090620: 203c 7464 3e32 3031 322d 3131 2d31 3520   <td>2012-11-15 
+00090630: 3137 3a34 393a 3031 3c2f 7464 3e0a 2020  17:49:01</td>.  
+00090640: 2020 2020 3c74 643e 3130 3639 3c2f 7464      <td>1069</td
+00090650: 3e0a 2020 2020 2020 3c74 643e 362e 363c  >.      <td>6.6<
+00090660: 2f74 643e 0a20 2020 2020 203c 7464 3e33  /td>.      <td>3
+00090670: 3c2f 7464 3e0a 2020 2020 2020 3c74 643e  </td>.      <td>
+00090680: 436c 6561 723c 2f74 643e 0a20 2020 2020  Clear</td>.     
+00090690: 203c 7464 3e54 6875 7273 6461 793c 2f74   <td>Thursday</t
+000906a0: 643e 0a20 2020 2020 203c 7464 3e46 7269  d>.      <td>Fri
+000906b0: 6564 2043 6869 636b 656e 204a 6f69 6e74  ed Chicken Joint
+000906c0: 3c2f 7464 3e0a 2020 2020 2020 3c74 643e  </td>.      <td>
+000906d0: 3132 363c 2f74 643e 0a20 2020 2020 203c  126</td>.      <
+000906e0: 7464 3e46 6f6f 643c 2f74 643e 0a20 2020  td>Food</td>.   
+000906f0: 203c 2f74 723e 0a20 2020 203c 7472 3e0a   </tr>.    <tr>.
+00090700: 2020 2020 2020 3c74 683e 343c 2f74 683e        <th>4</th>
+00090710: 0a20 2020 2020 203c 7464 3e34 302e 3736  .      <td>40.76
+00090720: 3630 3739 3033 3736 3832 3420 2d37 332e  60790376824 -73.
+00090730: 3838 3335 3238 3730 3934 3131 363c 2f74  8835287094116</t
+00090740: 643e 0a20 2020 2020 203c 7464 3e32 3031  d>.      <td>201
+00090750: 322d 3131 2d31 3520 3138 3a34 303a 3136  2-11-15 18:40:16
+00090760: 3c2f 7464 3e0a 2020 2020 2020 3c74 643e  </td>.      <td>
+00090770: 3131 3230 3c2f 7464 3e0a 2020 2020 2020  1120</td>.      
+00090780: 3c74 643e 2d31 2e30 3c2f 7464 3e0a 2020  <td>-1.0</td>.  
+00090790: 2020 2020 3c74 643e 2d31 3c2f 7464 3e0a      <td>-1</td>.
+000907a0: 2020 2020 2020 3c74 643e 436c 6561 723c        <td>Clear<
+000907b0: 2f74 643e 0a20 2020 2020 203c 7464 3e54  /td>.      <td>T
+000907c0: 6875 7273 6461 793c 2f74 643e 0a20 2020  hursday</td>.   
+000907d0: 2020 203c 7464 3e42 7573 2053 7461 7469     <td>Bus Stati
+000907e0: 6f6e 3c2f 7464 3e0a 2020 2020 2020 3c74  on</td>.      <t
+000907f0: 643e 3132 363c 2f74 643e 0a20 2020 2020  d>126</td>.     
+00090800: 203c 7464 3e54 7261 7665 6c20 2661 6d70   <td>Travel &amp
+00090810: 3b20 5472 616e 7370 6f72 743c 2f74 643e  ; Transport</td>
+00090820: 0a20 2020 203c 2f74 723e 0a20 203c 2f74  .    </tr>.  </t
+00090830: 626f 6479 3e0a 3c2f 7461 626c 653e 0a3c  body>.</table>.<
+00090840: 2f64 6976 3e0a 3c2f 6469 763e 0a0a 3c2f  /div>.</div>..</
+00090850: 6469 763e 0a0a 3c2f 6469 763e 0a0a 3c2f  div>..</div>..</
+00090860: 6469 763e 0a0a 3c2f 6469 763e 0a3c 6469  div>..</div>.<di
+00090870: 7620 636c 6173 733d 226a 702d 4365 6c6c  v class="jp-Cell
+00090880: 206a 702d 4d61 726b 646f 776e 4365 6c6c   jp-MarkdownCell
+00090890: 206a 702d 4e6f 7465 626f 6f6b 2d63 656c   jp-Notebook-cel
+000908a0: 6c22 3e0a 3c64 6976 2063 6c61 7373 3d22  l">.<div class="
+000908b0: 6a70 2d43 656c 6c2d 696e 7075 7457 7261  jp-Cell-inputWra
+000908c0: 7070 6572 223e 0a3c 6469 7620 636c 6173  pper">.<div clas
+000908d0: 733d 226a 702d 436f 6c6c 6170 7365 7220  s="jp-Collapser 
+000908e0: 6a70 2d49 6e70 7574 436f 6c6c 6170 7365  jp-InputCollapse
+000908f0: 7220 6a70 2d43 656c 6c2d 696e 7075 7443  r jp-Cell-inputC
+00090900: 6f6c 6c61 7073 6572 223e 0a3c 2f64 6976  ollapser">.</div
+00090910: 3e0a 3c64 6976 2063 6c61 7373 3d22 6a70  >.<div class="jp
+00090920: 2d49 6e70 7574 4172 6561 206a 702d 4365  -InputArea jp-Ce
+00090930: 6c6c 2d69 6e70 7574 4172 6561 223e 3c64  ll-inputArea"><d
+00090940: 6976 2063 6c61 7373 3d22 6a70 2d49 6e70  iv class="jp-Inp
+00090950: 7574 5072 6f6d 7074 206a 702d 496e 7075  utPrompt jp-Inpu
+00090960: 7441 7265 612d 7072 6f6d 7074 223e 0a3c  tArea-prompt">.<
+00090970: 2f64 6976 3e3c 6469 7620 636c 6173 733d  /div><div class=
+00090980: 226a 702d 5265 6e64 6572 6564 4854 4d4c  "jp-RenderedHTML
+00090990: 436f 6d6d 6f6e 206a 702d 5265 6e64 6572  Common jp-Render
+000909a0: 6564 4d61 726b 646f 776e 206a 702d 4d61  edMarkdown jp-Ma
+000909b0: 726b 646f 776e 4f75 7470 7574 2022 2064  rkdownOutput " d
+000909c0: 6174 612d 6d69 6d65 2d74 7970 653d 2274  ata-mime-type="t
+000909d0: 6578 742f 6d61 726b 646f 776e 223e 0a3c  ext/markdown">.<
+000909e0: 6833 2069 643d 2232 2e2d 4c6f 6164 696e  h3 id="2.-Loadin
+000909f0: 672d 5265 706f 7369 746f 7279 2d44 6174  g-Repository-Dat
+00090a00: 6122 3e32 2e20 4c6f 6164 696e 6720 5265  a">2. Loading Re
+00090a10: 706f 7369 746f 7279 2044 6174 613c 6120  pository Data<a 
+00090a20: 636c 6173 733d 2261 6e63 686f 722d 6c69  class="anchor-li
+00090a30: 6e6b 2220 6872 6566 3d22 2332 2e2d 4c6f  nk" href="#2.-Lo
+00090a40: 6164 696e 672d 5265 706f 7369 746f 7279  ading-Repository
+00090a50: 2d44 6174 6122 3e26 2331 3832 3b3c 2f61  -Data">&#182;</a
+00090a60: 3e3c 2f68 333e 3c70 3e54 6869 7320 6d6f  ></h3><p>This mo
+00090a70: 6475 6c65 206c 6f61 6473 2064 6174 6120  dule loads data 
+00090a80: 6672 6f6d 2070 7562 6c69 6320 7265 706f  from public repo
+00090a90: 7369 746f 7279 203c 6120 6872 6566 3d22  sitory <a href="
+00090aa0: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+00090ab0: 6f6d 2f6d 6174 2d61 6e61 6c79 7369 732f  om/mat-analysis/
+00090ac0: 6461 7461 7365 7473 223e 4769 743a 206d  datasets">Git: m
+00090ad0: 6174 2d61 6e61 6c79 7369 7320 6461 7461  at-analysis data
+00090ae0: 7365 7473 2028 7632 5f30 293c 2f61 3e3c  sets (v2_0)</a><
+00090af0: 2f70 3e0a 3c70 3e43 6865 636b 2074 6865  /p>.<p>Check the
+00090b00: 2047 6974 4875 6220 7265 706f 7369 746f   GitHub reposito
+00090b10: 7279 2074 6f20 7365 6520 6176 6169 6c61  ry to see availa
+00090b20: 626c 6520 6461 7461 7365 7473 2e3c 2f70  ble datasets.</p
+00090b30: 3e0a 0a3c 2f64 6976 3e0a 3c2f 6469 763e  >..</div>.</div>
+00090b40: 0a3c 2f64 6976 3e0a 3c2f 6469 763e 0a3c  .</div>.</div>.<
+00090b50: 6469 7620 636c 6173 733d 226a 702d 4365  div class="jp-Ce
+00090b60: 6c6c 206a 702d 4d61 726b 646f 776e 4365  ll jp-MarkdownCe
+00090b70: 6c6c 206a 702d 4e6f 7465 626f 6f6b 2d63  ll jp-Notebook-c
+00090b80: 656c 6c22 3e0a 3c64 6976 2063 6c61 7373  ell">.<div class
+00090b90: 3d22 6a70 2d43 656c 6c2d 696e 7075 7457  ="jp-Cell-inputW
+00090ba0: 7261 7070 6572 223e 0a3c 6469 7620 636c  rapper">.<div cl
+00090bb0: 6173 733d 226a 702d 436f 6c6c 6170 7365  ass="jp-Collapse
+00090bc0: 7220 6a70 2d49 6e70 7574 436f 6c6c 6170  r jp-InputCollap
+00090bd0: 7365 7220 6a70 2d43 656c 6c2d 696e 7075  ser jp-Cell-inpu
+00090be0: 7443 6f6c 6c61 7073 6572 223e 0a3c 2f64  tCollapser">.</d
+00090bf0: 6976 3e0a 3c64 6976 2063 6c61 7373 3d22  iv>.<div class="
+00090c00: 6a70 2d49 6e70 7574 4172 6561 206a 702d  jp-InputArea jp-
+00090c10: 4365 6c6c 2d69 6e70 7574 4172 6561 223e  Cell-inputArea">
+00090c20: 3c64 6976 2063 6c61 7373 3d22 6a70 2d49  <div class="jp-I
+00090c30: 6e70 7574 5072 6f6d 7074 206a 702d 496e  nputPrompt jp-In
+00090c40: 7075 7441 7265 612d 7072 6f6d 7074 223e  putArea-prompt">
+00090c50: 0a3c 2f64 6976 3e3c 6469 7620 636c 6173  .</div><div clas
+00090c60: 733d 226a 702d 5265 6e64 6572 6564 4854  s="jp-RenderedHT
+00090c70: 4d4c 436f 6d6d 6f6e 206a 702d 5265 6e64  MLCommon jp-Rend
+00090c80: 6572 6564 4d61 726b 646f 776e 206a 702d  eredMarkdown jp-
+00090c90: 4d61 726b 646f 776e 4f75 7470 7574 2022  MarkdownOutput "
+00090ca0: 2064 6174 612d 6d69 6d65 2d74 7970 653d   data-mime-type=
+00090cb0: 2274 6578 742f 6d61 726b 646f 776e 223e  "text/markdown">
+00090cc0: 0a3c 703e 546f 2075 7365 2068 656c 7065  .<p>To use helpe
+00090cd0: 7273 2066 6f72 2064 6174 6120 6c6f 6164  rs for data load
+00090ce0: 696e 672c 2069 6d70 6f72 7420 6672 6f6d  ing, import from
+00090cf0: 2070 6163 6b61 6765 203c 636f 6465 3e6d   package <code>m
+00090d00: 6174 6461 7461 2e64 6174 6173 6574 3c2f  atdata.dataset</
+00090d10: 636f 6465 3e3a 3c2f 703e 0a0a 3c2f 6469  code>:</p>..</di
+00090d20: 763e 0a3c 2f64 6976 3e0a 3c2f 6469 763e  v>.</div>.</div>
+00090d30: 0a3c 2f64 6976 3e3c 6469 7620 636c 6173  .</div><div clas
+00090d40: 733d 226a 702d 4365 6c6c 206a 702d 436f  s="jp-Cell jp-Co
+00090d50: 6465 4365 6c6c 206a 702d 4e6f 7465 626f  deCell jp-Notebo
+00090d60: 6f6b 2d63 656c 6c20 6a70 2d6d 6f64 2d6e  ok-cell jp-mod-n
+00090d70: 6f4f 7574 7075 7473 2020 223e 0a3c 6469  oOutputs  ">.<di
+00090d80: 7620 636c 6173 733d 226a 702d 4365 6c6c  v class="jp-Cell
+00090d90: 2d69 6e70 7574 5772 6170 7065 7222 3e0a  -inputWrapper">.
+00090da0: 3c64 6976 2063 6c61 7373 3d22 6a70 2d43  <div class="jp-C
+00090db0: 6f6c 6c61 7073 6572 206a 702d 496e 7075  ollapser jp-Inpu
+00090dc0: 7443 6f6c 6c61 7073 6572 206a 702d 4365  tCollapser jp-Ce
+00090dd0: 6c6c 2d69 6e70 7574 436f 6c6c 6170 7365  ll-inputCollapse
+00090de0: 7222 3e0a 3c2f 6469 763e 0a3c 6469 7620  r">.</div>.<div 
+00090df0: 636c 6173 733d 226a 702d 496e 7075 7441  class="jp-InputA
+00090e00: 7265 6120 6a70 2d43 656c 6c2d 696e 7075  rea jp-Cell-inpu
+00090e10: 7441 7265 6122 3e0a 3c64 6976 2063 6c61  tArea">.<div cla
+00090e20: 7373 3d22 6a70 2d49 6e70 7574 5072 6f6d  ss="jp-InputProm
+00090e30: 7074 206a 702d 496e 7075 7441 7265 612d  pt jp-InputArea-
+00090e40: 7072 6f6d 7074 223e 496e 266e 6273 703b  prompt">In&nbsp;
+00090e50: 5b31 325d 3a3c 2f64 6976 3e0a 3c64 6976  [12]:</div>.<div
+00090e60: 2063 6c61 7373 3d22 6a70 2d43 6f64 654d   class="jp-CodeM
+00090e70: 6972 726f 7245 6469 746f 7220 6a70 2d45  irrorEditor jp-E
+00090e80: 6469 746f 7220 6a70 2d49 6e70 7574 4172  ditor jp-InputAr
+00090e90: 6561 2d65 6469 746f 7222 2064 6174 612d  ea-editor" data-
+00090ea0: 7479 7065 3d22 696e 6c69 6e65 223e 0a20  type="inline">. 
+00090eb0: 2020 2020 3c64 6976 2063 6c61 7373 3d22      <div class="
+00090ec0: 436f 6465 4d69 7272 6f72 2063 6d2d 732d  CodeMirror cm-s-
+00090ed0: 6a75 7079 7465 7222 3e0a 3c64 6976 2063  jupyter">.<div c
+00090ee0: 6c61 7373 3d22 2068 6967 686c 6967 6874  lass=" highlight
+00090ef0: 2068 6c2d 6970 7974 686f 6e33 223e 3c70   hl-ipython3"><p
+00090f00: 7265 3e3c 7370 616e 3e3c 2f73 7061 6e3e  re><span></span>
+00090f10: 3c73 7061 6e20 636c 6173 733d 226b 6e22  <span class="kn"
+00090f20: 3e66 726f 6d3c 2f73 7061 6e3e 203c 7370  >from</span> <sp
+00090f30: 616e 2063 6c61 7373 3d22 6e6e 223e 6d61  an class="nn">ma
+00090f40: 7464 6174 612e 6461 7461 7365 743c 2f73  tdata.dataset</s
+00090f50: 7061 6e3e 203c 7370 616e 2063 6c61 7373  pan> <span class
+00090f60: 3d22 6b6e 223e 696d 706f 7274 3c2f 7370  ="kn">import</sp
+00090f70: 616e 3e20 3c73 7061 6e20 636c 6173 733d  an> <span class=
+00090f80: 226f 223e 2a3c 2f73 7061 6e3e 0a3c 2f70  "o">*</span>.</p
+00090f90: 7265 3e3c 2f64 6976 3e0a 0a20 2020 2020  re></div>..     
+00090fa0: 3c2f 6469 763e 0a3c 2f64 6976 3e0a 3c2f  </div>.</div>.</
+00090fb0: 6469 763e 0a3c 2f64 6976 3e0a 0a3c 2f64  div>.</div>..</d
+00090fc0: 6976 3e0a 3c64 6976 2063 6c61 7373 3d22  iv>.<div class="
+00090fd0: 6a70 2d43 656c 6c20 6a70 2d4d 6172 6b64  jp-Cell jp-Markd
+00090fe0: 6f77 6e43 656c 6c20 6a70 2d4e 6f74 6562  ownCell jp-Noteb
+00090ff0: 6f6f 6b2d 6365 6c6c 223e 0a3c 6469 7620  ook-cell">.<div 
+00091000: 636c 6173 733d 226a 702d 4365 6c6c 2d69  class="jp-Cell-i
+00091010: 6e70 7574 5772 6170 7065 7222 3e0a 3c64  nputWrapper">.<d
+00091020: 6976 2063 6c61 7373 3d22 6a70 2d43 6f6c  iv class="jp-Col
+00091030: 6c61 7073 6572 206a 702d 496e 7075 7443  lapser jp-InputC
+00091040: 6f6c 6c61 7073 6572 206a 702d 4365 6c6c  ollapser jp-Cell
+00091050: 2d69 6e70 7574 436f 6c6c 6170 7365 7222  -inputCollapser"
+00091060: 3e0a 3c2f 6469 763e 0a3c 6469 7620 636c  >.</div>.<div cl
+00091070: 6173 733d 226a 702d 496e 7075 7441 7265  ass="jp-InputAre
+00091080: 6120 6a70 2d43 656c 6c2d 696e 7075 7441  a jp-Cell-inputA
+00091090: 7265 6122 3e3c 6469 7620 636c 6173 733d  rea"><div class=
+000910a0: 226a 702d 496e 7075 7450 726f 6d70 7420  "jp-InputPrompt 
+000910b0: 6a70 2d49 6e70 7574 4172 6561 2d70 726f  jp-InputArea-pro
+000910c0: 6d70 7422 3e0a 3c2f 6469 763e 3c64 6976  mpt">.</div><div
+000910d0: 2063 6c61 7373 3d22 6a70 2d52 656e 6465   class="jp-Rende
+000910e0: 7265 6448 544d 4c43 6f6d 6d6f 6e20 6a70  redHTMLCommon jp
+000910f0: 2d52 656e 6465 7265 644d 6172 6b64 6f77  -RenderedMarkdow
+00091100: 6e20 6a70 2d4d 6172 6b64 6f77 6e4f 7574  n jp-MarkdownOut
+00091110: 7075 7420 2220 6461 7461 2d6d 696d 652d  put " data-mime-
+00091120: 7479 7065 3d22 7465 7874 2f6d 6172 6b64  type="text/markd
+00091130: 6f77 6e22 3e0a 0a3c 7072 653e 3c63 6f64  own">..<pre><cod
+00091140: 653e 6129 2046 6972 7374 2c20 796f 7520  e>a) First, you 
+00091150: 6361 6e20 6c6f 6164 2064 6174 6173 6574  can load dataset
+00091160: 7320 6279 2069 6e66 6f72 6d69 6e67 2074  s by informing t
+00091170: 6865 2063 6174 6567 6f72 7920 2870 6172  he category (par
+00091180: 656e 7420 666f 6c64 6572 2920 616e 6420  ent folder) and 
+00091190: 6461 7461 7365 7420 6e61 6d65 2028 7375  dataset name (su
+000911a0: 6266 6f6c 6465 7229 3a3c 2f63 6f64 653e  bfolder):</code>
+000911b0: 3c2f 7072 653e 0a0a 3c2f 6469 763e 0a3c  </pre>..</div>.<
+000911c0: 2f64 6976 3e0a 3c2f 6469 763e 0a3c 2f64  /div>.</div>.</d
+000911d0: 6976 3e3c 6469 7620 636c 6173 733d 226a  iv><div class="j
+000911e0: 702d 4365 6c6c 206a 702d 436f 6465 4365  p-Cell jp-CodeCe
+000911f0: 6c6c 206a 702d 4e6f 7465 626f 6f6b 2d63  ll jp-Notebook-c
+00091200: 656c 6c20 2020 223e 0a3c 6469 7620 636c  ell   ">.<div cl
+00091210: 6173 733d 226a 702d 4365 6c6c 2d69 6e70  ass="jp-Cell-inp
+00091220: 7574 5772 6170 7065 7222 3e0a 3c64 6976  utWrapper">.<div
+00091230: 2063 6c61 7373 3d22 6a70 2d43 6f6c 6c61   class="jp-Colla
+00091240: 7073 6572 206a 702d 496e 7075 7443 6f6c  pser jp-InputCol
+00091250: 6c61 7073 6572 206a 702d 4365 6c6c 2d69  lapser jp-Cell-i
+00091260: 6e70 7574 436f 6c6c 6170 7365 7222 3e0a  nputCollapser">.
+00091270: 3c2f 6469 763e 0a3c 6469 7620 636c 6173  </div>.<div clas
+00091280: 733d 226a 702d 496e 7075 7441 7265 6120  s="jp-InputArea 
+00091290: 6a70 2d43 656c 6c2d 696e 7075 7441 7265  jp-Cell-inputAre
+000912a0: 6122 3e0a 3c64 6976 2063 6c61 7373 3d22  a">.<div class="
+000912b0: 6a70 2d49 6e70 7574 5072 6f6d 7074 206a  jp-InputPrompt j
+000912c0: 702d 496e 7075 7441 7265 612d 7072 6f6d  p-InputArea-prom
+000912d0: 7074 223e 496e 266e 6273 703b 5b31 335d  pt">In&nbsp;[13]
+000912e0: 3a3c 2f64 6976 3e0a 3c64 6976 2063 6c61  :</div>.<div cla
+000912f0: 7373 3d22 6a70 2d43 6f64 654d 6972 726f  ss="jp-CodeMirro
+00091300: 7245 6469 746f 7220 6a70 2d45 6469 746f  rEditor jp-Edito
+00091310: 7220 6a70 2d49 6e70 7574 4172 6561 2d65  r jp-InputArea-e
+00091320: 6469 746f 7222 2064 6174 612d 7479 7065  ditor" data-type
+00091330: 3d22 696e 6c69 6e65 223e 0a20 2020 2020  ="inline">.     
+00091340: 3c64 6976 2063 6c61 7373 3d22 436f 6465  <div class="Code
+00091350: 4d69 7272 6f72 2063 6d2d 732d 6a75 7079  Mirror cm-s-jupy
+00091360: 7465 7222 3e0a 3c64 6976 2063 6c61 7373  ter">.<div class
+00091370: 3d22 2068 6967 686c 6967 6874 2068 6c2d  =" highlight hl-
+00091380: 6970 7974 686f 6e33 223e 3c70 7265 3e3c  ipython3"><pre><
+00091390: 7370 616e 3e3c 2f73 7061 6e3e 3c73 7061  span></span><spa
+000913a0: 6e20 636c 6173 733d 2263 3122 3e23 2064  n class="c1"># d
+000913b0: 6174 6173 6574 3d26 2333 393b 6d61 742e  ataset=&#39;mat.
+000913c0: 466f 7572 7371 7561 7265 4e59 4326 2333  FoursquareNYC&#3
+000913d0: 393b 2023 2320 3d26 6774 3b20 6461 6661  9; ## =&gt; dafa
+000913e0: 756c 743c 2f73 7061 6e3e 0a0a 3c73 7061  ult</span>..<spa
+000913f0: 6e20 636c 6173 733d 226e 223e 6466 3c2f  n class="n">df</
+00091400: 7370 616e 3e20 3c73 7061 6e20 636c 6173  span> <span clas
+00091410: 733d 226f 223e 3d3c 2f73 7061 6e3e 203c  s="o">=</span> <
+00091420: 7370 616e 2063 6c61 7373 3d22 6e22 3e6c  span class="n">l
+00091430: 6f61 645f 6473 3c2f 7370 616e 3e3c 7370  oad_ds</span><sp
+00091440: 616e 2063 6c61 7373 3d22 7022 3e28 3c2f  an class="p">(</
+00091450: 7370 616e 3e3c 7370 616e 2063 6c61 7373  span><span class
+00091460: 3d22 6e22 3e73 616d 706c 655f 7369 7a65  ="n">sample_size
+00091470: 3c2f 7370 616e 3e3c 7370 616e 2063 6c61  </span><span cla
+00091480: 7373 3d22 6f22 3e3d 3c2f 7370 616e 3e3c  ss="o">=</span><
+00091490: 7370 616e 2063 6c61 7373 3d22 6d66 223e  span class="mf">
+000914a0: 302e 3235 3c2f 7370 616e 3e3c 7370 616e  0.25</span><span
+000914b0: 2063 6c61 7373 3d22 7022 3e29 3c2f 7370   class="p">)</sp
+000914c0: 616e 3e0a 3c73 7061 6e20 636c 6173 733d  an>.<span class=
+000914d0: 226e 223e 6466 3c2f 7370 616e 3e0a 3c2f  "n">df</span>.</
+000914e0: 7072 653e 3c2f 6469 763e 0a0a 2020 2020  pre></div>..    
+000914f0: 203c 2f64 6976 3e0a 3c2f 6469 763e 0a3c   </div>.</div>.<
+00091500: 2f64 6976 3e0a 3c2f 6469 763e 0a0a 3c64  /div>.</div>..<d
+00091510: 6976 2063 6c61 7373 3d22 6a70 2d43 656c  iv class="jp-Cel
+00091520: 6c2d 6f75 7470 7574 5772 6170 7065 7222  l-outputWrapper"
+00091530: 3e0a 3c64 6976 2063 6c61 7373 3d22 6a70  >.<div class="jp
+00091540: 2d43 6f6c 6c61 7073 6572 206a 702d 4f75  -Collapser jp-Ou
+00091550: 7470 7574 436f 6c6c 6170 7365 7220 6a70  tputCollapser jp
+00091560: 2d43 656c 6c2d 6f75 7470 7574 436f 6c6c  -Cell-outputColl
+00091570: 6170 7365 7222 3e0a 3c2f 6469 763e 0a0a  apser">.</div>..
+00091580: 0a3c 6469 7620 636c 6173 733d 226a 702d  .<div class="jp-
+00091590: 4f75 7470 7574 4172 6561 206a 702d 4365  OutputArea jp-Ce
+000915a0: 6c6c 2d6f 7574 7075 7441 7265 6122 3e0a  ll-outputArea">.
+000915b0: 0a3c 6469 7620 636c 6173 733d 226a 702d  .<div class="jp-
+000915c0: 4f75 7470 7574 4172 6561 2d63 6869 6c64  OutputArea-child
+000915d0: 223e 0a0a 2020 2020 0a20 2020 203c 6469  ">..    .    <di
+000915e0: 7620 636c 6173 733d 226a 702d 4f75 7470  v class="jp-Outp
+000915f0: 7574 5072 6f6d 7074 206a 702d 4f75 7470  utPrompt jp-Outp
+00091600: 7574 4172 6561 2d70 726f 6d70 7422 3e3c  utArea-prompt"><
+00091610: 2f64 6976 3e0a 0a0a 3c64 6976 2063 6c61  /div>...<div cla
+00091620: 7373 3d22 6a70 2d52 656e 6465 7265 6454  ss="jp-RenderedT
+00091630: 6578 7420 6a70 2d4f 7574 7075 7441 7265  ext jp-OutputAre
+00091640: 612d 6f75 7470 7574 2220 6461 7461 2d6d  a-output" data-m
+00091650: 696d 652d 7479 7065 3d22 7465 7874 2f70  ime-type="text/p
+00091660: 6c61 696e 223e 0a3c 7072 653e 4c6f 6164  lain">.<pre>Load
+00091670: 696e 6720 6461 7461 7365 7420 6669 6c65  ing dataset file
+00091680: 3a20 6874 7470 733a 2f2f 6769 7468 7562  : https://github
+00091690: 2e63 6f6d 2f6d 6174 2d61 6e61 6c79 7369  .com/mat-analysi
+000916a0: 732f 6461 7461 7365 7473 2f72 6177 2f6d  s/datasets/raw/m
+000916b0: 6169 6e2f 6d61 742f 466f 7572 7371 7561  ain/mat/Foursqua
+000916c0: 7265 4e59 432f 0a3c 2f70 7265 3e0a 3c2f  reNYC/.</pre>.</
+000916d0: 6469 763e 0a3c 2f64 6976 3e0a 0a3c 6469  div>.</div>..<di
+000916e0: 7620 636c 6173 733d 226a 702d 4f75 7470  v class="jp-Outp
+000916f0: 7574 4172 6561 2d63 6869 6c64 223e 0a0a  utArea-child">..
+00091700: 2020 2020 0a20 2020 203c 6469 7620 636c      .    <div cl
+00091710: 6173 733d 226a 702d 4f75 7470 7574 5072  ass="jp-OutputPr
+00091720: 6f6d 7074 206a 702d 4f75 7470 7574 4172  ompt jp-OutputAr
+00091730: 6561 2d70 726f 6d70 7422 3e3c 2f64 6976  ea-prompt"></div
+00091740: 3e0a 0a0a 0a0a 3c64 6976 2063 6c61 7373  >.....<div class
+00091750: 3d22 6a70 2d52 656e 6465 7265 6454 6578  ="jp-RenderedTex
+00091760: 7420 6a70 2d4f 7574 7075 7441 7265 612d  t jp-OutputArea-
+00091770: 6f75 7470 7574 2022 2064 6174 612d 6d69  output " data-mi
+00091780: 6d65 2d74 7970 653d 2274 6578 742f 706c  me-type="text/pl
+00091790: 6169 6e22 3e0a 3c70 7265 3e20 2030 257c  ain">.<pre>  0%|
+000917a0: 2020 2020 2020 2020 2020 7c20 302f 3139            | 0/19
+000917b0: 3320 5b30 303a 3030 266c 743b 3f2c 203f  3 [00:00&lt;?, ?
+000917c0: 6974 2f73 5d3c 2f70 7265 3e0a 3c2f 6469  it/s]</pre>.</di
+000917d0: 763e 0a0a 3c2f 6469 763e 0a0a 3c64 6976  v>..</div>..<div
+000917e0: 2063 6c61 7373 3d22 6a70 2d4f 7574 7075   class="jp-Outpu
+000917f0: 7441 7265 612d 6368 696c 6422 3e0a 0a20  tArea-child">.. 
+00091800: 2020 200a 2020 2020 3c64 6976 2063 6c61     .    <div cla
+00091810: 7373 3d22 6a70 2d4f 7574 7075 7450 726f  ss="jp-OutputPro
+00091820: 6d70 7420 6a70 2d4f 7574 7075 7441 7265  mpt jp-OutputAre
+00091830: 612d 7072 6f6d 7074 223e 4f75 745b 3133  a-prompt">Out[13
+00091840: 5d3a 3c2f 6469 763e 0a0a 0a0a 3c64 6976  ]:</div>....<div
+00091850: 2063 6c61 7373 3d22 6a70 2d52 656e 6465   class="jp-Rende
+00091860: 7265 6448 544d 4c43 6f6d 6d6f 6e20 6a70  redHTMLCommon jp
+00091870: 2d52 656e 6465 7265 6448 544d 4c20 6a70  -RenderedHTML jp
+00091880: 2d4f 7574 7075 7441 7265 612d 6f75 7470  -OutputArea-outp
+00091890: 7574 206a 702d 4f75 7470 7574 4172 6561  ut jp-OutputArea
+000918a0: 2d65 7865 6375 7465 5265 7375 6c74 2220  -executeResult" 
+000918b0: 6461 7461 2d6d 696d 652d 7479 7065 3d22  data-mime-type="
+000918c0: 7465 7874 2f68 746d 6c22 3e0a 3c64 6976  text/html">.<div
+000918d0: 3e0a 3c73 7479 6c65 2073 636f 7065 643e  >.<style scoped>
+000918e0: 0a20 2020 202e 6461 7461 6672 616d 6520  .    .dataframe 
+000918f0: 7462 6f64 7920 7472 2074 683a 6f6e 6c79  tbody tr th:only
+00091900: 2d6f 662d 7479 7065 207b 0a20 2020 2020  -of-type {.     
+00091910: 2020 2076 6572 7469 6361 6c2d 616c 6967     vertical-alig
+00091920: 6e3a 206d 6964 646c 653b 0a20 2020 207d  n: middle;.    }
+00091930: 0a0a 2020 2020 2e64 6174 6166 7261 6d65  ..    .dataframe
+00091940: 2074 626f 6479 2074 7220 7468 207b 0a20   tbody tr th {. 
+00091950: 2020 2020 2020 2076 6572 7469 6361 6c2d         vertical-
+00091960: 616c 6967 6e3a 2074 6f70 3b0a 2020 2020  align: top;.    
+00091970: 7d0a 0a20 2020 202e 6461 7461 6672 616d  }..    .datafram
+00091980: 6520 7468 6561 6420 7468 207b 0a20 2020  e thead th {.   
+00091990: 2020 2020 2074 6578 742d 616c 6967 6e3a       text-align:
+000919a0: 2072 6967 6874 3b0a 2020 2020 7d0a 3c2f   right;.    }.</
+000919b0: 7374 796c 653e 0a3c 7461 626c 6520 626f  style>.<table bo
+000919c0: 7264 6572 3d22 3122 2063 6c61 7373 3d22  rder="1" class="
+000919d0: 6461 7461 6672 616d 6522 3e0a 2020 3c74  dataframe">.  <t
+000919e0: 6865 6164 3e0a 2020 2020 3c74 7220 7374  head>.    <tr st
+000919f0: 796c 653d 2274 6578 742d 616c 6967 6e3a  yle="text-align:
+00091a00: 2072 6967 6874 3b22 3e0a 2020 2020 2020   right;">.      
+00091a10: 3c74 683e 3c2f 7468 3e0a 2020 2020 2020  <th></th>.      
+00091a20: 3c74 683e 6c61 743c 2f74 683e 0a20 2020  <th>lat</th>.   
+00091a30: 2020 203c 7468 3e6c 6f6e 3c2f 7468 3e0a     <th>lon</th>.
+00091a40: 2020 2020 2020 3c74 683e 6461 793c 2f74        <th>day</t
+00091a50: 683e 0a20 2020 2020 203c 7468 3e68 6f75  h>.      <th>hou
+00091a60: 723c 2f74 683e 0a20 2020 2020 203c 7468  r</th>.      <th
+00091a70: 3e70 6f69 3c2f 7468 3e0a 2020 2020 2020  >poi</th>.      
+00091a80: 3c74 683e 6361 7465 676f 7279 3c2f 7468  <th>category</th
+00091a90: 3e0a 2020 2020 2020 3c74 683e 7072 6963  >.      <th>pric
+00091aa0: 653c 2f74 683e 0a20 2020 2020 203c 7468  e</th>.      <th
+00091ab0: 3e72 6174 696e 673c 2f74 683e 0a20 2020  >rating</th>.   
+00091ac0: 2020 203c 7468 3e77 6561 7468 6572 3c2f     <th>weather</
+00091ad0: 7468 3e0a 2020 2020 2020 3c74 683e 7469  th>.      <th>ti
+00091ae0: 643c 2f74 683e 0a20 2020 2020 203c 7468  d</th>.      <th
+00091af0: 3e6c 6162 656c 3c2f 7468 3e0a 2020 2020  >label</th>.    
+00091b00: 3c2f 7472 3e0a 2020 3c2f 7468 6561 643e  </tr>.  </thead>
+00091b10: 0a20 203c 7462 6f64 793e 0a20 2020 203c  .  <tbody>.    <
+00091b20: 7472 3e0a 2020 2020 2020 3c74 683e 303c  tr>.      <th>0<
+00091b30: 2f74 683e 0a20 2020 2020 203c 7464 3e34  /th>.      <td>4
+00091b40: 302e 3833 3430 3938 3c2f 7464 3e0a 2020  0.834098</td>.  
+00091b50: 2020 2020 3c74 643e 2d37 332e 3934 3532      <td>-73.9452
+00091b60: 3637 3c2f 7464 3e0a 2020 2020 2020 3c74  67</td>.      <t
+00091b70: 643e 4d6f 6e64 6179 3c2f 7464 3e0a 2020  d>Monday</td>.  
+00091b80: 2020 2020 3c74 643e 3133 3c2f 7464 3e0a      <td>13</td>.
+00091b90: 2020 2020 2020 3c74 643e 3231 3538 303c        <td>21580<
+00091ba0: 2f74 643e 0a20 2020 2020 203c 7464 3e46  /td>.      <td>F
+00091bb0: 6f6f 643c 2f74 643e 0a20 2020 2020 203c  ood</td>.      <
+00091bc0: 7464 3e31 3c2f 7464 3e0a 2020 2020 2020  td>1</td>.      
+00091bd0: 3c74 643e 382e 323c 2f74 643e 0a20 2020  <td>8.2</td>.   
+00091be0: 2020 203c 7464 3e43 6c6f 7564 733c 2f74     <td>Clouds</t
+00091bf0: 643e 0a20 2020 2020 203c 7464 3e31 3237  d>.      <td>127
+00091c00: 3c2f 7464 3e0a 2020 2020 2020 3c74 643e  </td>.      <td>
+00091c10: 363c 2f74 643e 0a20 2020 203c 2f74 723e  6</td>.    </tr>
+00091c20: 0a20 2020 203c 7472 3e0a 2020 2020 2020  .    <tr>.      
+00091c30: 3c74 683e 313c 2f74 683e 0a20 2020 2020  <th>1</th>.     
+00091c40: 203c 7464 3e34 302e 3536 3731 3936 3c2f   <td>40.567196</
+00091c50: 7464 3e0a 2020 2020 2020 3c74 643e 2d37  td>.      <td>-7
+00091c60: 332e 3838 3235 3736 3c2f 7464 3e0a 2020  3.882576</td>.  
+00091c70: 2020 2020 3c74 643e 4d6f 6e64 6179 3c2f      <td>Monday</
+00091c80: 7464 3e0a 2020 2020 2020 3c74 643e 3139  td>.      <td>19
+00091c90: 3c2f 7464 3e0a 2020 2020 2020 3c74 643e  </td>.      <td>
+00091ca0: 3233 3932 3c2f 7464 3e0a 2020 2020 2020  2392</td>.      
+00091cb0: 3c74 643e 5472 6176 656c 2026 616d 703b  <td>Travel &amp;
+00091cc0: 2054 7261 6e73 706f 7274 3c2f 7464 3e0a   Transport</td>.
+00091cd0: 2020 2020 2020 3c74 643e 2d39 3939 3c2f        <td>-999</
+00091ce0: 7464 3e0a 2020 2020 2020 3c74 643e 2d39  td>.      <td>-9
+00091cf0: 3939 2e30 3c2f 7464 3e0a 2020 2020 2020  99.0</td>.      
+00091d00: 3c74 643e 436c 6f75 6473 3c2f 7464 3e0a  <td>Clouds</td>.
+00091d10: 2020 2020 2020 3c74 643e 3132 373c 2f74        <td>127</t
+00091d20: 643e 0a20 2020 2020 203c 7464 3e36 3c2f  d>.      <td>6</
+00091d30: 7464 3e0a 2020 2020 3c2f 7472 3e0a 2020  td>.    </tr>.  
+00091d40: 2020 3c74 723e 0a20 2020 2020 203c 7468    <tr>.      <th
+00091d50: 3e32 3c2f 7468 3e0a 2020 2020 2020 3c74  >2</th>.      <t
+00091d60: 643e 3430 2e36 3839 3931 333c 2f74 643e  d>40.689913</td>
+00091d70: 0a20 2020 2020 203c 7464 3e2d 3733 2e39  .      <td>-73.9
+00091d80: 3831 3530 343c 2f74 643e 0a20 2020 2020  81504</td>.     
+00091d90: 203c 7464 3e4d 6f6e 6461 793c 2f74 643e   <td>Monday</td>
+00091da0: 0a20 2020 2020 203c 7464 3e32 333c 2f74  .      <td>23</t
+00091db0: 643e 0a20 2020 2020 203c 7464 3e33 3535  d>.      <td>355
+00091dc0: 3839 3c2f 7464 3e0a 2020 2020 2020 3c74  89</td>.      <t
+00091dd0: 643e 5472 6176 656c 2026 616d 703b 2054  d>Travel &amp; T
+00091de0: 7261 6e73 706f 7274 3c2f 7464 3e0a 2020  ransport</td>.  
+00091df0: 2020 2020 3c74 643e 2d39 3939 3c2f 7464      <td>-999</td
+00091e00: 3e0a 2020 2020 2020 3c74 643e 2d39 3939  >.      <td>-999
+00091e10: 2e30 3c2f 7464 3e0a 2020 2020 2020 3c74  .0</td>.      <t
+00091e20: 643e 436c 6f75 6473 3c2f 7464 3e0a 2020  d>Clouds</td>.  
+00091e30: 2020 2020 3c74 643e 3132 373c 2f74 643e      <td>127</td>
+00091e40: 0a20 2020 2020 203c 7464 3e36 3c2f 7464  .      <td>6</td
+00091e50: 3e0a 2020 2020 3c2f 7472 3e0a 2020 2020  >.    </tr>.    
+00091e60: 3c74 723e 0a20 2020 2020 203c 7468 3e33  <tr>.      <th>3
+00091e70: 3c2f 7468 3e0a 2020 2020 2020 3c74 643e  </th>.      <td>
+00091e80: 3430 2e37 3038 3538 383c 2f74 643e 0a20  40.708588</td>. 
+00091e90: 2020 2020 203c 7464 3e2d 3733 2e39 3931       <td>-73.991
+00091ea0: 3033 323c 2f74 643e 0a20 2020 2020 203c  032</td>.      <
+00091eb0: 7464 3e4d 6f6e 6461 793c 2f74 643e 0a20  td>Monday</td>. 
+00091ec0: 2020 2020 203c 7464 3e32 333c 2f74 643e       <td>23</td>
+00091ed0: 0a20 2020 2020 203c 7464 3e31 3836 3033  .      <td>18603
+00091ee0: 3c2f 7464 3e0a 2020 2020 2020 3c74 643e  </td>.      <td>
+00091ef0: 5472 6176 656c 2026 616d 703b 2054 7261  Travel &amp; Tra
+00091f00: 6e73 706f 7274 3c2f 7464 3e0a 2020 2020  nsport</td>.    
+00091f10: 2020 3c74 643e 2d39 3939 3c2f 7464 3e0a    <td>-999</td>.
+00091f20: 2020 2020 2020 3c74 643e 2d39 3939 2e30        <td>-999.0
+00091f30: 3c2f 7464 3e0a 2020 2020 2020 3c74 643e  </td>.      <td>
+00091f40: 436c 6f75 6473 3c2f 7464 3e0a 2020 2020  Clouds</td>.    
+00091f50: 2020 3c74 643e 3132 373c 2f74 643e 0a20    <td>127</td>. 
+00091f60: 2020 2020 203c 7464 3e36 3c2f 7464 3e0a       <td>6</td>.
+00091f70: 2020 2020 3c2f 7472 3e0a 2020 2020 3c74      </tr>.    <t
+00091f80: 723e 0a20 2020 2020 203c 7468 3e34 3c2f  r>.      <th>4</
+00091f90: 7468 3e0a 2020 2020 2020 3c74 643e 3430  th>.      <td>40
+00091fa0: 2e38 3333 3136 353c 2f74 643e 0a20 2020  .833165</td>.   
+00091fb0: 2020 203c 7464 3e2d 3733 2e39 3431 3836     <td>-73.94186
+00091fc0: 303c 2f74 643e 0a20 2020 2020 203c 7464  0</td>.      <td
+00091fd0: 3e54 7565 7364 6179 3c2f 7464 3e0a 2020  >Tuesday</td>.  
+00091fe0: 2020 2020 3c74 643e 3134 3c2f 7464 3e0a      <td>14</td>.
+00091ff0: 2020 2020 2020 3c74 643e 3336 3334 383c        <td>36348<
+00092000: 2f74 643e 0a20 2020 2020 203c 7464 3e52  /td>.      <td>R
+00092010: 6573 6964 656e 6365 3c2f 7464 3e0a 2020  esidence</td>.  
+00092020: 2020 2020 3c74 643e 2d39 3939 3c2f 7464      <td>-999</td
+00092030: 3e0a 2020 2020 2020 3c74 643e 2d39 3939  >.      <td>-999
+00092040: 2e30 3c2f 7464 3e0a 2020 2020 2020 3c74  .0</td>.      <t
+00092050: 643e 436c 6561 723c 2f74 643e 0a20 2020  d>Clear</td>.   
+00092060: 2020 203c 7464 3e31 3237 3c2f 7464 3e0a     <td>127</td>.
+00092070: 2020 2020 2020 3c74 643e 363c 2f74 643e        <td>6</td>
+00092080: 0a20 2020 203c 2f74 723e 0a20 2020 203c  .    </tr>.    <
+00092090: 7472 3e0a 2020 2020 2020 3c74 683e 2e2e  tr>.      <th>..
+000920a0: 2e3c 2f74 683e 0a20 2020 2020 203c 7464  .</th>.      <td
+000920b0: 3e2e 2e2e 3c2f 7464 3e0a 2020 2020 2020  >...</td>.      
+000920c0: 3c74 643e 2e2e 2e3c 2f74 643e 0a20 2020  <td>...</td>.   
+000920d0: 2020 203c 7464 3e2e 2e2e 3c2f 7464 3e0a     <td>...</td>.
+000920e0: 2020 2020 2020 3c74 643e 2e2e 2e3c 2f74        <td>...</t
+000920f0: 643e 0a20 2020 2020 203c 7464 3e2e 2e2e  d>.      <td>...
+00092100: 3c2f 7464 3e0a 2020 2020 2020 3c74 643e  </td>.      <td>
+00092110: 2e2e 2e3c 2f74 643e 0a20 2020 2020 203c  ...</td>.      <
+00092120: 7464 3e2e 2e2e 3c2f 7464 3e0a 2020 2020  td>...</td>.    
+00092130: 2020 3c74 643e 2e2e 2e3c 2f74 643e 0a20    <td>...</td>. 
+00092140: 2020 2020 203c 7464 3e2e 2e2e 3c2f 7464       <td>...</td
+00092150: 3e0a 2020 2020 2020 3c74 643e 2e2e 2e3c  >.      <td>...<
+00092160: 2f74 643e 0a20 2020 2020 203c 7464 3e2e  /td>.      <td>.
+00092170: 2e2e 3c2f 7464 3e0a 2020 2020 3c2f 7472  ..</td>.    </tr
+00092180: 3e0a 2020 2020 3c74 723e 0a20 2020 2020  >.    <tr>.     
+00092190: 203c 7468 3e32 3231 3138 3c2f 7468 3e0a   <th>22118</th>.
+000921a0: 2020 2020 2020 3c74 643e 3430 2e37 3034        <td>40.704
+000921b0: 3237 333c 2f74 643e 0a20 2020 2020 203c  273</td>.      <
+000921c0: 7464 3e2d 3733 2e39 3836 3735 393c 2f74  td>-73.986759</t
+000921d0: 643e 0a20 2020 2020 203c 7464 3e53 6174  d>.      <td>Sat
+000921e0: 7572 6461 793c 2f74 643e 0a20 2020 2020  urday</td>.     
+000921f0: 203c 7464 3e31 303c 2f74 643e 0a20 2020   <td>10</td>.   
+00092200: 2020 203c 7464 3e32 3534 3631 3c2f 7464     <td>25461</td
+00092210: 3e0a 2020 2020 2020 3c74 643e 4f75 7464  >.      <td>Outd
+00092220: 6f6f 7273 2026 616d 703b 2052 6563 7265  oors &amp; Recre
+00092230: 6174 696f 6e3c 2f74 643e 0a20 2020 2020  ation</td>.     
+00092240: 203c 7464 3e2d 3939 393c 2f74 643e 0a20   <td>-999</td>. 
+00092250: 2020 2020 203c 7464 3e38 2e36 3c2f 7464       <td>8.6</td
+00092260: 3e0a 2020 2020 2020 3c74 643e 436c 6561  >.      <td>Clea
+00092270: 723c 2f74 643e 0a20 2020 2020 203c 7464  r</td>.      <td
+00092280: 3e32 3935 3531 3c2f 7464 3e0a 2020 2020  >29551</td>.    
+00092290: 2020 3c74 643e 3130 3730 3c2f 7464 3e0a    <td>1070</td>.
+000922a0: 2020 2020 3c2f 7472 3e0a 2020 2020 3c74      </tr>.    <t
+000922b0: 723e 0a20 2020 2020 203c 7468 3e32 3231  r>.      <th>221
+000922c0: 3139 3c2f 7468 3e0a 2020 2020 2020 3c74  19</th>.      <t
+000922d0: 643e 3430 2e37 3034 3733 333c 2f74 643e  d>40.704733</td>
+000922e0: 0a20 2020 2020 203c 7464 3e2d 3733 2e39  .      <td>-73.9
+000922f0: 3837 3733 383c 2f74 643e 0a20 2020 2020  87738</td>.     
+00092300: 203c 7464 3e53 6174 7572 6461 793c 2f74   <td>Saturday</t
+00092310: 643e 0a20 2020 2020 203c 7464 3e31 303c  d>.      <td>10<
+00092320: 2f74 643e 0a20 2020 2020 203c 7464 3e31  /td>.      <td>1
+00092330: 3830 353c 2f74 643e 0a20 2020 2020 203c  805</td>.      <
+00092340: 7464 3e43 6f6c 6c65 6765 2026 616d 703b  td>College &amp;
+00092350: 2055 6e69 7665 7273 6974 793c 2f74 643e   University</td>
+00092360: 0a20 2020 2020 203c 7464 3e2d 3939 393c  .      <td>-999<
+00092370: 2f74 643e 0a20 2020 2020 203c 7464 3e2d  /td>.      <td>-
+00092380: 3939 392e 303c 2f74 643e 0a20 2020 2020  999.0</td>.     
+00092390: 203c 7464 3e43 6c65 6172 3c2f 7464 3e0a   <td>Clear</td>.
+000923a0: 2020 2020 2020 3c74 643e 3239 3535 313c        <td>29551<
+000923b0: 2f74 643e 0a20 2020 2020 203c 7464 3e31  /td>.      <td>1
+000923c0: 3037 303c 2f74 643e 0a20 2020 203c 2f74  070</td>.    </t
+000923d0: 723e 0a20 2020 203c 7472 3e0a 2020 2020  r>.    <tr>.    
+000923e0: 2020 3c74 683e 3232 3132 303c 2f74 683e    <th>22120</th>
+000923f0: 0a20 2020 2020 203c 7464 3e34 302e 3731  .      <td>40.71
+00092400: 3733 3533 3c2f 7464 3e0a 2020 2020 2020  7353</td>.      
+00092410: 3c74 643e 2d37 332e 3936 3033 3932 3c2f  <td>-73.960392</
+00092420: 7464 3e0a 2020 2020 2020 3c74 643e 5361  td>.      <td>Sa
+00092430: 7475 7264 6179 3c2f 7464 3e0a 2020 2020  turday</td>.    
+00092440: 2020 3c74 643e 3133 3c2f 7464 3e0a 2020    <td>13</td>.  
+00092450: 2020 2020 3c74 643e 3332 3532 333c 2f74      <td>32523</t
+00092460: 643e 0a20 2020 2020 203c 7464 3e46 6f6f  d>.      <td>Foo
+00092470: 643c 2f74 643e 0a20 2020 2020 203c 7464  d</td>.      <td
+00092480: 3e31 3c2f 7464 3e0a 2020 2020 2020 3c74  >1</td>.      <t
+00092490: 643e 392e 333c 2f74 643e 0a20 2020 2020  d>9.3</td>.     
+000924a0: 203c 7464 3e43 6c65 6172 3c2f 7464 3e0a   <td>Clear</td>.
+000924b0: 2020 2020 2020 3c74 643e 3239 3535 313c        <td>29551<
+000924c0: 2f74 643e 0a20 2020 2020 203c 7464 3e31  /td>.      <td>1
+000924d0: 3037 303c 2f74 643e 0a20 2020 203c 2f74  070</td>.    </t
+000924e0: 723e 0a20 2020 203c 7472 3e0a 2020 2020  r>.    <tr>.    
+000924f0: 2020 3c74 683e 3232 3132 313c 2f74 683e    <th>22121</th>
+00092500: 0a20 2020 2020 203c 7464 3e34 302e 3639  .      <td>40.69
+00092510: 3737 3231 3c2f 7464 3e0a 2020 2020 2020  7721</td>.      
+00092520: 3c74 643e 2d37 332e 3939 3330 3230 3c2f  <td>-73.993020</
+00092530: 7464 3e0a 2020 2020 2020 3c74 643e 5375  td>.      <td>Su
+00092540: 6e64 6179 3c2f 7464 3e0a 2020 2020 2020  nday</td>.      
+00092550: 3c74 643e 323c 2f74 643e 0a20 2020 2020  <td>2</td>.     
+00092560: 203c 7464 3e33 3632 3132 3c2f 7464 3e0a   <td>36212</td>.
+00092570: 2020 2020 2020 3c74 643e 436f 6c6c 6567        <td>Colleg
+00092580: 6520 2661 6d70 3b20 556e 6976 6572 7369  e &amp; Universi
+00092590: 7479 3c2f 7464 3e0a 2020 2020 2020 3c74  ty</td>.      <t
+000925a0: 643e 2d39 3939 3c2f 7464 3e0a 2020 2020  d>-999</td>.    
+000925b0: 2020 3c74 643e 2d39 3939 2e30 3c2f 7464    <td>-999.0</td
+000925c0: 3e0a 2020 2020 2020 3c74 643e 436c 6561  >.      <td>Clea
+000925d0: 723c 2f74 643e 0a20 2020 2020 203c 7464  r</td>.      <td
+000925e0: 3e32 3935 3531 3c2f 7464 3e0a 2020 2020  >29551</td>.    
+000925f0: 2020 3c74 643e 3130 3730 3c2f 7464 3e0a    <td>1070</td>.
+00092600: 2020 2020 3c2f 7472 3e0a 2020 2020 3c74      </tr>.    <t
+00092610: 723e 0a20 2020 2020 203c 7468 3e32 3231  r>.      <th>221
+00092620: 3232 3c2f 7468 3e0a 2020 2020 2020 3c74  22</th>.      <t
+00092630: 643e 3430 2e36 3937 3830 333c 2f74 643e  d>40.697803</td>
+00092640: 0a20 2020 2020 203c 7464 3e2d 3733 2e39  .      <td>-73.9
+00092650: 3934 3134 353c 2f74 643e 0a20 2020 2020  94145</td>.     
+00092660: 203c 7464 3e53 756e 6461 793c 2f74 643e   <td>Sunday</td>
+00092670: 0a20 2020 2020 203c 7464 3e38 3c2f 7464  .      <td>8</td
+00092680: 3e0a 2020 2020 2020 3c74 643e 3136 3435  >.      <td>1645
+00092690: 323c 2f74 643e 0a20 2020 2020 203c 7464  2</td>.      <td
+000926a0: 3e4f 7574 646f 6f72 7320 2661 6d70 3b20  >Outdoors &amp; 
+000926b0: 5265 6372 6561 7469 6f6e 3c2f 7464 3e0a  Recreation</td>.
+000926c0: 2020 2020 2020 3c74 643e 2d39 3939 3c2f        <td>-999</
+000926d0: 7464 3e0a 2020 2020 2020 3c74 643e 362e  td>.      <td>6.
+000926e0: 393c 2f74 643e 0a20 2020 2020 203c 7464  9</td>.      <td
+000926f0: 3e43 6c65 6172 3c2f 7464 3e0a 2020 2020  >Clear</td>.    
+00092700: 2020 3c74 643e 3239 3535 313c 2f74 643e    <td>29551</td>
+00092710: 0a20 2020 2020 203c 7464 3e31 3037 303c  .      <td>1070<
+00092720: 2f74 643e 0a20 2020 203c 2f74 723e 0a20  /td>.    </tr>. 
+00092730: 203c 2f74 626f 6479 3e0a 3c2f 7461 626c   </tbody>.</tabl
+00092740: 653e 0a3c 703e 3136 3433 3520 726f 7773  e>.<p>16435 rows
+00092750: 20c3 9720 3131 2063 6f6c 756d 6e73 3c2f   .. 11 columns</
+00092760: 703e 0a3c 2f64 6976 3e0a 3c2f 6469 763e  p>.</div>.</div>
+00092770: 0a0a 3c2f 6469 763e 0a0a 3c2f 6469 763e  ..</div>..</div>
+00092780: 0a0a 3c2f 6469 763e 0a0a 3c2f 6469 763e  ..</div>..</div>
+00092790: 0a3c 6469 7620 636c 6173 733d 226a 702d  .<div class="jp-
+000927a0: 4365 6c6c 206a 702d 4d61 726b 646f 776e  Cell jp-Markdown
+000927b0: 4365 6c6c 206a 702d 4e6f 7465 626f 6f6b  Cell jp-Notebook
+000927c0: 2d63 656c 6c22 3e0a 3c64 6976 2063 6c61  -cell">.<div cla
+000927d0: 7373 3d22 6a70 2d43 656c 6c2d 696e 7075  ss="jp-Cell-inpu
+000927e0: 7457 7261 7070 6572 223e 0a3c 6469 7620  tWrapper">.<div 
+000927f0: 636c 6173 733d 226a 702d 436f 6c6c 6170  class="jp-Collap
+00092800: 7365 7220 6a70 2d49 6e70 7574 436f 6c6c  ser jp-InputColl
+00092810: 6170 7365 7220 6a70 2d43 656c 6c2d 696e  apser jp-Cell-in
+00092820: 7075 7443 6f6c 6c61 7073 6572 223e 0a3c  putCollapser">.<
+00092830: 2f64 6976 3e0a 3c64 6976 2063 6c61 7373  /div>.<div class
+00092840: 3d22 6a70 2d49 6e70 7574 4172 6561 206a  ="jp-InputArea j
+00092850: 702d 4365 6c6c 2d69 6e70 7574 4172 6561  p-Cell-inputArea
+00092860: 223e 3c64 6976 2063 6c61 7373 3d22 6a70  "><div class="jp
+00092870: 2d49 6e70 7574 5072 6f6d 7074 206a 702d  -InputPrompt jp-
+00092880: 496e 7075 7441 7265 612d 7072 6f6d 7074  InputArea-prompt
+00092890: 223e 0a3c 2f64 6976 3e3c 6469 7620 636c  ">.</div><div cl
+000928a0: 6173 733d 226a 702d 5265 6e64 6572 6564  ass="jp-Rendered
+000928b0: 4854 4d4c 436f 6d6d 6f6e 206a 702d 5265  HTMLCommon jp-Re
+000928c0: 6e64 6572 6564 4d61 726b 646f 776e 206a  nderedMarkdown j
+000928d0: 702d 4d61 726b 646f 776e 4f75 7470 7574  p-MarkdownOutput
+000928e0: 2022 2064 6174 612d 6d69 6d65 2d74 7970   " data-mime-typ
+000928f0: 653d 2274 6578 742f 6d61 726b 646f 776e  e="text/markdown
+00092900: 223e 0a0a 3c70 7265 3e3c 636f 6465 3e20  ">..<pre><code> 
+00092910: 6229 2053 6563 6f6e 642c 2079 6f75 2063  b) Second, you c
+00092920: 616e 206c 6f61 6420 7468 6520 3730 2f33  an load the 70/3
+00092930: 3020 686f 6c64 206f 7574 2073 706c 6974  0 hold out split
+00092940: 2061 7661 696c 6162 6c65 2028 6279 2064   available (by d
+00092950: 6566 6175 6c74 293a 3c2f 636f 6465 3e3c  efault):</code><
+00092960: 2f70 7265 3e0a 0a3c 2f64 6976 3e0a 3c2f  /pre>..</div>.</
+00092970: 6469 763e 0a3c 2f64 6976 3e0a 3c2f 6469  div>.</div>.</di
+00092980: 763e 3c64 6976 2063 6c61 7373 3d22 6a70  v><div class="jp
+00092990: 2d43 656c 6c20 6a70 2d43 6f64 6543 656c  -Cell jp-CodeCel
+000929a0: 6c20 6a70 2d4e 6f74 6562 6f6f 6b2d 6365  l jp-Notebook-ce
+000929b0: 6c6c 2020 2022 3e0a 3c64 6976 2063 6c61  ll   ">.<div cla
+000929c0: 7373 3d22 6a70 2d43 656c 6c2d 696e 7075  ss="jp-Cell-inpu
+000929d0: 7457 7261 7070 6572 223e 0a3c 6469 7620  tWrapper">.<div 
+000929e0: 636c 6173 733d 226a 702d 436f 6c6c 6170  class="jp-Collap
+000929f0: 7365 7220 6a70 2d49 6e70 7574 436f 6c6c  ser jp-InputColl
+00092a00: 6170 7365 7220 6a70 2d43 656c 6c2d 696e  apser jp-Cell-in
+00092a10: 7075 7443 6f6c 6c61 7073 6572 223e 0a3c  putCollapser">.<
+00092a20: 2f64 6976 3e0a 3c64 6976 2063 6c61 7373  /div>.<div class
+00092a30: 3d22 6a70 2d49 6e70 7574 4172 6561 206a  ="jp-InputArea j
+00092a40: 702d 4365 6c6c 2d69 6e70 7574 4172 6561  p-Cell-inputArea
+00092a50: 223e 0a3c 6469 7620 636c 6173 733d 226a  ">.<div class="j
+00092a60: 702d 496e 7075 7450 726f 6d70 7420 6a70  p-InputPrompt jp
+00092a70: 2d49 6e70 7574 4172 6561 2d70 726f 6d70  -InputArea-promp
+00092a80: 7422 3e49 6e26 6e62 7370 3b5b 3134 5d3a  t">In&nbsp;[14]:
+00092a90: 3c2f 6469 763e 0a3c 6469 7620 636c 6173  </div>.<div clas
+00092aa0: 733d 226a 702d 436f 6465 4d69 7272 6f72  s="jp-CodeMirror
+00092ab0: 4564 6974 6f72 206a 702d 4564 6974 6f72  Editor jp-Editor
+00092ac0: 206a 702d 496e 7075 7441 7265 612d 6564   jp-InputArea-ed
+00092ad0: 6974 6f72 2220 6461 7461 2d74 7970 653d  itor" data-type=
+00092ae0: 2269 6e6c 696e 6522 3e0a 2020 2020 203c  "inline">.     <
+00092af0: 6469 7620 636c 6173 733d 2243 6f64 654d  div class="CodeM
+00092b00: 6972 726f 7220 636d 2d73 2d6a 7570 7974  irror cm-s-jupyt
+00092b10: 6572 223e 0a3c 6469 7620 636c 6173 733d  er">.<div class=
+00092b20: 2220 6869 6768 6c69 6768 7420 686c 2d69  " highlight hl-i
+00092b30: 7079 7468 6f6e 3322 3e3c 7072 653e 3c73  python3"><pre><s
+00092b40: 7061 6e3e 3c2f 7370 616e 3e3c 7370 616e  pan></span><span
+00092b50: 2063 6c61 7373 3d22 6e22 3e64 665f 7472   class="n">df_tr
+00092b60: 6169 6e3c 2f73 7061 6e3e 3c73 7061 6e20  ain</span><span 
+00092b70: 636c 6173 733d 2270 223e 2c3c 2f73 7061  class="p">,</spa
+00092b80: 6e3e 203c 7370 616e 2063 6c61 7373 3d22  n> <span class="
+00092b90: 6e22 3e64 665f 7465 7374 3c2f 7370 616e  n">df_test</span
+00092ba0: 3e20 3c73 7061 6e20 636c 6173 733d 226f  > <span class="o
+00092bb0: 223e 3d3c 2f73 7061 6e3e 203c 7370 616e  ">=</span> <span
+00092bc0: 2063 6c61 7373 3d22 6e22 3e6c 6f61 645f   class="n">load_
+00092bd0: 6473 5f68 6f6c 646f 7574 3c2f 7370 616e  ds_holdout</span
+00092be0: 3e3c 7370 616e 2063 6c61 7373 3d22 7022  ><span class="p"
+00092bf0: 3e28 293c 2f73 7061 6e3e 0a0a 3c73 7061  >()</span>..<spa
+00092c00: 6e20 636c 6173 733d 226e 6222 3e70 7269  n class="nb">pri
+00092c10: 6e74 3c2f 7370 616e 3e3c 7370 616e 2063  nt</span><span c
+00092c20: 6c61 7373 3d22 7022 3e28 3c2f 7370 616e  lass="p">(</span
+00092c30: 3e3c 7370 616e 2063 6c61 7373 3d22 6e22  ><span class="n"
+00092c40: 3e64 665f 7472 6169 6e3c 2f73 7061 6e3e  >df_train</span>
+00092c50: 3c73 7061 6e20 636c 6173 733d 226f 223e  <span class="o">
+00092c60: 2e3c 2f73 7061 6e3e 3c73 7061 6e20 636c  .</span><span cl
+00092c70: 6173 733d 226e 223e 7368 6170 653c 2f73  ass="n">shape</s
+00092c80: 7061 6e3e 3c73 7061 6e20 636c 6173 733d  pan><span class=
+00092c90: 2270 223e 2c3c 2f73 7061 6e3e 203c 7370  "p">,</span> <sp
+00092ca0: 616e 2063 6c61 7373 3d22 6e22 3e64 665f  an class="n">df_
+00092cb0: 7465 7374 3c2f 7370 616e 3e3c 7370 616e  test</span><span
+00092cc0: 2063 6c61 7373 3d22 6f22 3e2e 3c2f 7370   class="o">.</sp
+00092cd0: 616e 3e3c 7370 616e 2063 6c61 7373 3d22  an><span class="
+00092ce0: 6e22 3e73 6861 7065 3c2f 7370 616e 3e3c  n">shape</span><
+00092cf0: 7370 616e 2063 6c61 7373 3d22 7022 3e29  span class="p">)
+00092d00: 3c2f 7370 616e 3e0a 0a3c 7370 616e 2063  </span>..<span c
+00092d10: 6c61 7373 3d22 6e22 3e64 665f 7472 6169  lass="n">df_trai
+00092d20: 6e3c 2f73 7061 6e3e 0a3c 2f70 7265 3e3c  n</span>.</pre><
+00092d30: 2f64 6976 3e0a 0a20 2020 2020 3c2f 6469  /div>..     </di
+00092d40: 763e 0a3c 2f64 6976 3e0a 3c2f 6469 763e  v>.</div>.</div>
+00092d50: 0a3c 2f64 6976 3e0a 0a3c 6469 7620 636c  .</div>..<div cl
+00092d60: 6173 733d 226a 702d 4365 6c6c 2d6f 7574  ass="jp-Cell-out
+00092d70: 7075 7457 7261 7070 6572 223e 0a3c 6469  putWrapper">.<di
+00092d80: 7620 636c 6173 733d 226a 702d 436f 6c6c  v class="jp-Coll
+00092d90: 6170 7365 7220 6a70 2d4f 7574 7075 7443  apser jp-OutputC
+00092da0: 6f6c 6c61 7073 6572 206a 702d 4365 6c6c  ollapser jp-Cell
+00092db0: 2d6f 7574 7075 7443 6f6c 6c61 7073 6572  -outputCollapser
+00092dc0: 223e 0a3c 2f64 6976 3e0a 0a0a 3c64 6976  ">.</div>...<div
+00092dd0: 2063 6c61 7373 3d22 6a70 2d4f 7574 7075   class="jp-Outpu
+00092de0: 7441 7265 6120 6a70 2d43 656c 6c2d 6f75  tArea jp-Cell-ou
+00092df0: 7470 7574 4172 6561 223e 0a0a 3c64 6976  tputArea">..<div
+00092e00: 2063 6c61 7373 3d22 6a70 2d4f 7574 7075   class="jp-Outpu
+00092e10: 7441 7265 612d 6368 696c 6422 3e0a 0a20  tArea-child">.. 
+00092e20: 2020 200a 2020 2020 3c64 6976 2063 6c61     .    <div cla
+00092e30: 7373 3d22 6a70 2d4f 7574 7075 7450 726f  ss="jp-OutputPro
+00092e40: 6d70 7420 6a70 2d4f 7574 7075 7441 7265  mpt jp-OutputAre
+00092e50: 612d 7072 6f6d 7074 223e 3c2f 6469 763e  a-prompt"></div>
+00092e60: 0a0a 0a3c 6469 7620 636c 6173 733d 226a  ...<div class="j
+00092e70: 702d 5265 6e64 6572 6564 5465 7874 206a  p-RenderedText j
+00092e80: 702d 4f75 7470 7574 4172 6561 2d6f 7574  p-OutputArea-out
+00092e90: 7075 7422 2064 6174 612d 6d69 6d65 2d74  put" data-mime-t
+00092ea0: 7970 653d 2274 6578 742f 706c 6169 6e22  ype="text/plain"
+00092eb0: 3e0a 3c70 7265 3e4c 6f61 6469 6e67 2064  >.<pre>Loading d
+00092ec0: 6174 6173 6574 2066 696c 653a 2068 7474  ataset file: htt
+00092ed0: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
+00092ee0: 6d61 742d 616e 616c 7973 6973 2f64 6174  mat-analysis/dat
+00092ef0: 6173 6574 732f 7261 772f 6d61 696e 2f6d  asets/raw/main/m
+00092f00: 6174 2f46 6f75 7273 7175 6172 654e 5943  at/FoursquareNYC
+00092f10: 2f0a 3c2f 7072 653e 0a3c 2f64 6976 3e0a  /.</pre>.</div>.
+00092f20: 3c2f 6469 763e 0a0a 3c64 6976 2063 6c61  </div>..<div cla
+00092f30: 7373 3d22 6a70 2d4f 7574 7075 7441 7265  ss="jp-OutputAre
+00092f40: 612d 6368 696c 6422 3e0a 0a20 2020 200a  a-child">..    .
+00092f50: 2020 2020 3c64 6976 2063 6c61 7373 3d22      <div class="
+00092f60: 6a70 2d4f 7574 7075 7450 726f 6d70 7420  jp-OutputPrompt 
+00092f70: 6a70 2d4f 7574 7075 7441 7265 612d 7072  jp-OutputArea-pr
+00092f80: 6f6d 7074 223e 3c2f 6469 763e 0a0a 0a0a  ompt"></div>....
+00092f90: 0a3c 6469 7620 636c 6173 733d 226a 702d  .<div class="jp-
+00092fa0: 5265 6e64 6572 6564 5465 7874 206a 702d  RenderedText jp-
+00092fb0: 4f75 7470 7574 4172 6561 2d6f 7574 7075  OutputArea-outpu
+00092fc0: 7420 2220 6461 7461 2d6d 696d 652d 7479  t " data-mime-ty
+00092fd0: 7065 3d22 7465 7874 2f70 6c61 696e 223e  pe="text/plain">
+00092fe0: 0a3c 7072 653e 2020 3025 7c20 2020 2020  .<pre>  0%|     
+00092ff0: 2020 2020 207c 2030 2f31 3933 205b 3030       | 0/193 [00
+00093000: 3a30 3026 6c74 3b3f 2c20 3f69 742f 735d  :00&lt;?, ?it/s]
+00093010: 3c2f 7072 653e 0a3c 2f64 6976 3e0a 0a3c  </pre>.</div>..<
+00093020: 2f64 6976 3e0a 0a3c 6469 7620 636c 6173  /div>..<div clas
+00093030: 733d 226a 702d 4f75 7470 7574 4172 6561  s="jp-OutputArea
+00093040: 2d63 6869 6c64 223e 0a0a 2020 2020 0a20  -child">..    . 
+00093050: 2020 203c 6469 7620 636c 6173 733d 226a     <div class="j
+00093060: 702d 4f75 7470 7574 5072 6f6d 7074 206a  p-OutputPrompt j
+00093070: 702d 4f75 7470 7574 4172 6561 2d70 726f  p-OutputArea-pro
+00093080: 6d70 7422 3e3c 2f64 6976 3e0a 0a0a 3c64  mpt"></div>...<d
+00093090: 6976 2063 6c61 7373 3d22 6a70 2d52 656e  iv class="jp-Ren
+000930a0: 6465 7265 6454 6578 7420 6a70 2d4f 7574  deredText jp-Out
+000930b0: 7075 7441 7265 612d 6f75 7470 7574 2220  putArea-output" 
+000930c0: 6461 7461 2d6d 696d 652d 7479 7065 3d22  data-mime-type="
+000930d0: 7465 7874 2f70 6c61 696e 223e 0a3c 7072  text/plain">.<pr
+000930e0: 653e 2834 3637 3835 2c20 3131 2920 2832  e>(46785, 11) (2
+000930f0: 3031 3737 2c20 3131 290a 3c2f 7072 653e  0177, 11).</pre>
+00093100: 0a3c 2f64 6976 3e0a 3c2f 6469 763e 0a0a  .</div>.</div>..
+00093110: 3c64 6976 2063 6c61 7373 3d22 6a70 2d4f  <div class="jp-O
+00093120: 7574 7075 7441 7265 612d 6368 696c 6422  utputArea-child"
+00093130: 3e0a 0a20 2020 200a 2020 2020 3c64 6976  >..    .    <div
+00093140: 2063 6c61 7373 3d22 6a70 2d4f 7574 7075   class="jp-Outpu
+00093150: 7450 726f 6d70 7420 6a70 2d4f 7574 7075  tPrompt jp-Outpu
+00093160: 7441 7265 612d 7072 6f6d 7074 223e 4f75  tArea-prompt">Ou
+00093170: 745b 3134 5d3a 3c2f 6469 763e 0a0a 0a0a  t[14]:</div>....
+00093180: 3c64 6976 2063 6c61 7373 3d22 6a70 2d52  <div class="jp-R
+00093190: 656e 6465 7265 6448 544d 4c43 6f6d 6d6f  enderedHTMLCommo
+000931a0: 6e20 6a70 2d52 656e 6465 7265 6448 544d  n jp-RenderedHTM
+000931b0: 4c20 6a70 2d4f 7574 7075 7441 7265 612d  L jp-OutputArea-
+000931c0: 6f75 7470 7574 206a 702d 4f75 7470 7574  output jp-Output
+000931d0: 4172 6561 2d65 7865 6375 7465 5265 7375  Area-executeResu
+000931e0: 6c74 2220 6461 7461 2d6d 696d 652d 7479  lt" data-mime-ty
+000931f0: 7065 3d22 7465 7874 2f68 746d 6c22 3e0a  pe="text/html">.
+00093200: 3c64 6976 3e0a 3c73 7479 6c65 2073 636f  <div>.<style sco
+00093210: 7065 643e 0a20 2020 202e 6461 7461 6672  ped>.    .datafr
+00093220: 616d 6520 7462 6f64 7920 7472 2074 683a  ame tbody tr th:
+00093230: 6f6e 6c79 2d6f 662d 7479 7065 207b 0a20  only-of-type {. 
+00093240: 2020 2020 2020 2076 6572 7469 6361 6c2d         vertical-
+00093250: 616c 6967 6e3a 206d 6964 646c 653b 0a20  align: middle;. 
+00093260: 2020 207d 0a0a 2020 2020 2e64 6174 6166     }..    .dataf
+00093270: 7261 6d65 2074 626f 6479 2074 7220 7468  rame tbody tr th
+00093280: 207b 0a20 2020 2020 2020 2076 6572 7469   {.        verti
+00093290: 6361 6c2d 616c 6967 6e3a 2074 6f70 3b0a  cal-align: top;.
+000932a0: 2020 2020 7d0a 0a20 2020 202e 6461 7461      }..    .data
+000932b0: 6672 616d 6520 7468 6561 6420 7468 207b  frame thead th {
+000932c0: 0a20 2020 2020 2020 2074 6578 742d 616c  .        text-al
+000932d0: 6967 6e3a 2072 6967 6874 3b0a 2020 2020  ign: right;.    
+000932e0: 7d0a 3c2f 7374 796c 653e 0a3c 7461 626c  }.</style>.<tabl
+000932f0: 6520 626f 7264 6572 3d22 3122 2063 6c61  e border="1" cla
+00093300: 7373 3d22 6461 7461 6672 616d 6522 3e0a  ss="dataframe">.
+00093310: 2020 3c74 6865 6164 3e0a 2020 2020 3c74    <thead>.    <t
+00093320: 7220 7374 796c 653d 2274 6578 742d 616c  r style="text-al
+00093330: 6967 6e3a 2072 6967 6874 3b22 3e0a 2020  ign: right;">.  
+00093340: 2020 2020 3c74 683e 3c2f 7468 3e0a 2020      <th></th>.  
+00093350: 2020 2020 3c74 683e 6c61 743c 2f74 683e      <th>lat</th>
+00093360: 0a20 2020 2020 203c 7468 3e6c 6f6e 3c2f  .      <th>lon</
+00093370: 7468 3e0a 2020 2020 2020 3c74 683e 6461  th>.      <th>da
+00093380: 793c 2f74 683e 0a20 2020 2020 203c 7468  y</th>.      <th
+00093390: 3e68 6f75 723c 2f74 683e 0a20 2020 2020  >hour</th>.     
+000933a0: 203c 7468 3e70 6f69 3c2f 7468 3e0a 2020   <th>poi</th>.  
+000933b0: 2020 2020 3c74 683e 6361 7465 676f 7279      <th>category
+000933c0: 3c2f 7468 3e0a 2020 2020 2020 3c74 683e  </th>.      <th>
+000933d0: 7072 6963 653c 2f74 683e 0a20 2020 2020  price</th>.     
+000933e0: 203c 7468 3e72 6174 696e 673c 2f74 683e   <th>rating</th>
+000933f0: 0a20 2020 2020 203c 7468 3e77 6561 7468  .      <th>weath
+00093400: 6572 3c2f 7468 3e0a 2020 2020 2020 3c74  er</th>.      <t
+00093410: 683e 7469 643c 2f74 683e 0a20 2020 2020  h>tid</th>.     
+00093420: 203c 7468 3e6c 6162 656c 3c2f 7468 3e0a   <th>label</th>.
+00093430: 2020 2020 3c2f 7472 3e0a 2020 3c2f 7468      </tr>.  </th
+00093440: 6561 643e 0a20 203c 7462 6f64 793e 0a20  ead>.  <tbody>. 
+00093450: 2020 203c 7472 3e0a 2020 2020 2020 3c74     <tr>.      <t
+00093460: 683e 303c 2f74 683e 0a20 2020 2020 203c  h>0</th>.      <
+00093470: 7464 3e34 302e 3833 3430 3938 3c2f 7464  td>40.834098</td
+00093480: 3e0a 2020 2020 2020 3c74 643e 2d37 332e  >.      <td>-73.
+00093490: 3934 3532 3637 3c2f 7464 3e0a 2020 2020  945267</td>.    
+000934a0: 2020 3c74 643e 4d6f 6e64 6179 3c2f 7464    <td>Monday</td
+000934b0: 3e0a 2020 2020 2020 3c74 643e 3133 3c2f  >.      <td>13</
+000934c0: 7464 3e0a 2020 2020 2020 3c74 643e 3231  td>.      <td>21
+000934d0: 3538 303c 2f74 643e 0a20 2020 2020 203c  580</td>.      <
+000934e0: 7464 3e46 6f6f 643c 2f74 643e 0a20 2020  td>Food</td>.   
+000934f0: 2020 203c 7464 3e31 3c2f 7464 3e0a 2020     <td>1</td>.  
+00093500: 2020 2020 3c74 643e 382e 323c 2f74 643e      <td>8.2</td>
+00093510: 0a20 2020 2020 203c 7464 3e43 6c6f 7564  .      <td>Cloud
+00093520: 733c 2f74 643e 0a20 2020 2020 203c 7464  s</td>.      <td
+00093530: 3e31 3237 3c2f 7464 3e0a 2020 2020 2020  >127</td>.      
+00093540: 3c74 643e 363c 2f74 643e 0a20 2020 203c  <td>6</td>.    <
+00093550: 2f74 723e 0a20 2020 203c 7472 3e0a 2020  /tr>.    <tr>.  
+00093560: 2020 2020 3c74 683e 313c 2f74 683e 0a20      <th>1</th>. 
+00093570: 2020 2020 203c 7464 3e34 302e 3536 3731       <td>40.5671
+00093580: 3936 3c2f 7464 3e0a 2020 2020 2020 3c74  96</td>.      <t
+00093590: 643e 2d37 332e 3838 3235 3736 3c2f 7464  d>-73.882576</td
+000935a0: 3e0a 2020 2020 2020 3c74 643e 4d6f 6e64  >.      <td>Mond
+000935b0: 6179 3c2f 7464 3e0a 2020 2020 2020 3c74  ay</td>.      <t
+000935c0: 643e 3139 3c2f 7464 3e0a 2020 2020 2020  d>19</td>.      
+000935d0: 3c74 643e 3233 3932 3c2f 7464 3e0a 2020  <td>2392</td>.  
+000935e0: 2020 2020 3c74 643e 5472 6176 656c 2026      <td>Travel &
+000935f0: 616d 703b 2054 7261 6e73 706f 7274 3c2f  amp; Transport</
+00093600: 7464 3e0a 2020 2020 2020 3c74 643e 2d39  td>.      <td>-9
+00093610: 3939 3c2f 7464 3e0a 2020 2020 2020 3c74  99</td>.      <t
+00093620: 643e 2d39 3939 2e30 3c2f 7464 3e0a 2020  d>-999.0</td>.  
+00093630: 2020 2020 3c74 643e 436c 6f75 6473 3c2f      <td>Clouds</
+00093640: 7464 3e0a 2020 2020 2020 3c74 643e 3132  td>.      <td>12
+00093650: 373c 2f74 643e 0a20 2020 2020 203c 7464  7</td>.      <td
+00093660: 3e36 3c2f 7464 3e0a 2020 2020 3c2f 7472  >6</td>.    </tr
+00093670: 3e0a 2020 2020 3c74 723e 0a20 2020 2020  >.    <tr>.     
+00093680: 203c 7468 3e32 3c2f 7468 3e0a 2020 2020   <th>2</th>.    
+00093690: 2020 3c74 643e 3430 2e36 3839 3931 333c    <td>40.689913<
+000936a0: 2f74 643e 0a20 2020 2020 203c 7464 3e2d  /td>.      <td>-
+000936b0: 3733 2e39 3831 3530 343c 2f74 643e 0a20  73.981504</td>. 
+000936c0: 2020 2020 203c 7464 3e4d 6f6e 6461 793c       <td>Monday<
+000936d0: 2f74 643e 0a20 2020 2020 203c 7464 3e32  /td>.      <td>2
+000936e0: 333c 2f74 643e 0a20 2020 2020 203c 7464  3</td>.      <td
+000936f0: 3e33 3535 3839 3c2f 7464 3e0a 2020 2020  >35589</td>.    
+00093700: 2020 3c74 643e 5472 6176 656c 2026 616d    <td>Travel &am
+00093710: 703b 2054 7261 6e73 706f 7274 3c2f 7464  p; Transport</td
+00093720: 3e0a 2020 2020 2020 3c74 643e 2d39 3939  >.      <td>-999
+00093730: 3c2f 7464 3e0a 2020 2020 2020 3c74 643e  </td>.      <td>
+00093740: 2d39 3939 2e30 3c2f 7464 3e0a 2020 2020  -999.0</td>.    
+00093750: 2020 3c74 643e 436c 6f75 6473 3c2f 7464    <td>Clouds</td
+00093760: 3e0a 2020 2020 2020 3c74 643e 3132 373c  >.      <td>127<
+00093770: 2f74 643e 0a20 2020 2020 203c 7464 3e36  /td>.      <td>6
+00093780: 3c2f 7464 3e0a 2020 2020 3c2f 7472 3e0a  </td>.    </tr>.
+00093790: 2020 2020 3c74 723e 0a20 2020 2020 203c      <tr>.      <
+000937a0: 7468 3e33 3c2f 7468 3e0a 2020 2020 2020  th>3</th>.      
+000937b0: 3c74 643e 3430 2e37 3038 3538 383c 2f74  <td>40.708588</t
+000937c0: 643e 0a20 2020 2020 203c 7464 3e2d 3733  d>.      <td>-73
+000937d0: 2e39 3931 3033 323c 2f74 643e 0a20 2020  .991032</td>.   
+000937e0: 2020 203c 7464 3e4d 6f6e 6461 793c 2f74     <td>Monday</t
+000937f0: 643e 0a20 2020 2020 203c 7464 3e32 333c  d>.      <td>23<
+00093800: 2f74 643e 0a20 2020 2020 203c 7464 3e31  /td>.      <td>1
+00093810: 3836 3033 3c2f 7464 3e0a 2020 2020 2020  8603</td>.      
+00093820: 3c74 643e 5472 6176 656c 2026 616d 703b  <td>Travel &amp;
+00093830: 2054 7261 6e73 706f 7274 3c2f 7464 3e0a   Transport</td>.
+00093840: 2020 2020 2020 3c74 643e 2d39 3939 3c2f        <td>-999</
+00093850: 7464 3e0a 2020 2020 2020 3c74 643e 2d39  td>.      <td>-9
+00093860: 3939 2e30 3c2f 7464 3e0a 2020 2020 2020  99.0</td>.      
+00093870: 3c74 643e 436c 6f75 6473 3c2f 7464 3e0a  <td>Clouds</td>.
+00093880: 2020 2020 2020 3c74 643e 3132 373c 2f74        <td>127</t
+00093890: 643e 0a20 2020 2020 203c 7464 3e36 3c2f  d>.      <td>6</
+000938a0: 7464 3e0a 2020 2020 3c2f 7472 3e0a 2020  td>.    </tr>.  
+000938b0: 2020 3c74 723e 0a20 2020 2020 203c 7468    <tr>.      <th
+000938c0: 3e34 3c2f 7468 3e0a 2020 2020 2020 3c74  >4</th>.      <t
+000938d0: 643e 3430 2e38 3333 3136 353c 2f74 643e  d>40.833165</td>
+000938e0: 0a20 2020 2020 203c 7464 3e2d 3733 2e39  .      <td>-73.9
+000938f0: 3431 3836 303c 2f74 643e 0a20 2020 2020  41860</td>.     
+00093900: 203c 7464 3e54 7565 7364 6179 3c2f 7464   <td>Tuesday</td
+00093910: 3e0a 2020 2020 2020 3c74 643e 3134 3c2f  >.      <td>14</
+00093920: 7464 3e0a 2020 2020 2020 3c74 643e 3336  td>.      <td>36
+00093930: 3334 383c 2f74 643e 0a20 2020 2020 203c  348</td>.      <
+00093940: 7464 3e52 6573 6964 656e 6365 3c2f 7464  td>Residence</td
+00093950: 3e0a 2020 2020 2020 3c74 643e 2d39 3939  >.      <td>-999
+00093960: 3c2f 7464 3e0a 2020 2020 2020 3c74 643e  </td>.      <td>
+00093970: 2d39 3939 2e30 3c2f 7464 3e0a 2020 2020  -999.0</td>.    
+00093980: 2020 3c74 643e 436c 6561 723c 2f74 643e    <td>Clear</td>
+00093990: 0a20 2020 2020 203c 7464 3e31 3237 3c2f  .      <td>127</
+000939a0: 7464 3e0a 2020 2020 2020 3c74 643e 363c  td>.      <td>6<
+000939b0: 2f74 643e 0a20 2020 203c 2f74 723e 0a20  /td>.    </tr>. 
+000939c0: 2020 203c 7472 3e0a 2020 2020 2020 3c74     <tr>.      <t
+000939d0: 683e 2e2e 2e3c 2f74 683e 0a20 2020 2020  h>...</th>.     
+000939e0: 203c 7464 3e2e 2e2e 3c2f 7464 3e0a 2020   <td>...</td>.  
+000939f0: 2020 2020 3c74 643e 2e2e 2e3c 2f74 643e      <td>...</td>
+00093a00: 0a20 2020 2020 203c 7464 3e2e 2e2e 3c2f  .      <td>...</
+00093a10: 7464 3e0a 2020 2020 2020 3c74 643e 2e2e  td>.      <td>..
+00093a20: 2e3c 2f74 643e 0a20 2020 2020 203c 7464  .</td>.      <td
+00093a30: 3e2e 2e2e 3c2f 7464 3e0a 2020 2020 2020  >...</td>.      
+00093a40: 3c74 643e 2e2e 2e3c 2f74 643e 0a20 2020  <td>...</td>.   
+00093a50: 2020 203c 7464 3e2e 2e2e 3c2f 7464 3e0a     <td>...</td>.
+00093a60: 2020 2020 2020 3c74 643e 2e2e 2e3c 2f74        <td>...</t
+00093a70: 643e 0a20 2020 2020 203c 7464 3e2e 2e2e  d>.      <td>...
+00093a80: 3c2f 7464 3e0a 2020 2020 2020 3c74 643e  </td>.      <td>
+00093a90: 2e2e 2e3c 2f74 643e 0a20 2020 2020 203c  ...</td>.      <
+00093aa0: 7464 3e2e 2e2e 3c2f 7464 3e0a 2020 2020  td>...</td>.    
+00093ab0: 3c2f 7472 3e0a 2020 2020 3c74 723e 0a20  </tr>.    <tr>. 
+00093ac0: 2020 2020 203c 7468 3e32 3231 3438 3c2f       <th>22148</
+00093ad0: 7468 3e0a 2020 2020 2020 3c74 643e 3430  th>.      <td>40
+00093ae0: 2e37 3035 3935 333c 2f74 643e 0a20 2020  .705953</td>.   
+00093af0: 2020 203c 7464 3e2d 3733 2e39 3936 3536     <td>-73.99656
+00093b00: 383c 2f74 643e 0a20 2020 2020 203c 7464  8</td>.      <td
+00093b10: 3e53 6174 7572 6461 793c 2f74 643e 0a20  >Saturday</td>. 
+00093b20: 2020 2020 203c 7464 3e31 393c 2f74 643e       <td>19</td>
+00093b30: 0a20 2020 2020 203c 7464 3e33 3533 3038  .      <td>35308
+00093b40: 3c2f 7464 3e0a 2020 2020 2020 3c74 643e  </td>.      <td>
+00093b50: 4f75 7464 6f6f 7273 2026 616d 703b 2052  Outdoors &amp; R
+00093b60: 6563 7265 6174 696f 6e3c 2f74 643e 0a20  ecreation</td>. 
+00093b70: 2020 2020 203c 7464 3e2d 3939 393c 2f74       <td>-999</t
+00093b80: 643e 0a20 2020 2020 203c 7464 3e39 2e36  d>.      <td>9.6
+00093b90: 3c2f 7464 3e0a 2020 2020 2020 3c74 643e  </td>.      <td>
+00093ba0: 436c 6561 723c 2f74 643e 0a20 2020 2020  Clear</td>.     
+00093bb0: 203c 7464 3e32 3935 3536 3c2f 7464 3e0a   <td>29556</td>.
+00093bc0: 2020 2020 2020 3c74 643e 3130 3730 3c2f        <td>1070</
+00093bd0: 7464 3e0a 2020 2020 3c2f 7472 3e0a 2020  td>.    </tr>.  
+00093be0: 2020 3c74 723e 0a20 2020 2020 203c 7468    <tr>.      <th
+00093bf0: 3e32 3231 3439 3c2f 7468 3e0a 2020 2020  >22149</th>.    
+00093c00: 2020 3c74 643e 3430 2e36 3937 3732 313c    <td>40.697721<
+00093c10: 2f74 643e 0a20 2020 2020 203c 7464 3e2d  /td>.      <td>-
+00093c20: 3733 2e39 3933 3032 303c 2f74 643e 0a20  73.993020</td>. 
+00093c30: 2020 2020 203c 7464 3e53 6174 7572 6461       <td>Saturda
+00093c40: 793c 2f74 643e 0a20 2020 2020 203c 7464  y</td>.      <td
+00093c50: 3e32 333c 2f74 643e 0a20 2020 2020 203c  >23</td>.      <
+00093c60: 7464 3e33 3632 3132 3c2f 7464 3e0a 2020  td>36212</td>.  
+00093c70: 2020 2020 3c74 643e 436f 6c6c 6567 6520      <td>College 
+00093c80: 2661 6d70 3b20 556e 6976 6572 7369 7479  &amp; University
+00093c90: 3c2f 7464 3e0a 2020 2020 2020 3c74 643e  </td>.      <td>
+00093ca0: 2d39 3939 3c2f 7464 3e0a 2020 2020 2020  -999</td>.      
+00093cb0: 3c74 643e 2d39 3939 2e30 3c2f 7464 3e0a  <td>-999.0</td>.
+00093cc0: 2020 2020 2020 3c74 643e 436c 6561 723c        <td>Clear<
+00093cd0: 2f74 643e 0a20 2020 2020 203c 7464 3e32  /td>.      <td>2
+00093ce0: 3935 3536 3c2f 7464 3e0a 2020 2020 2020  9556</td>.      
+00093cf0: 3c74 643e 3130 3730 3c2f 7464 3e0a 2020  <td>1070</td>.  
+00093d00: 2020 3c2f 7472 3e0a 2020 2020 3c74 723e    </tr>.    <tr>
+00093d10: 0a20 2020 2020 203c 7468 3e32 3231 3530  .      <th>22150
+00093d20: 3c2f 7468 3e0a 2020 2020 2020 3c74 643e  </th>.      <td>
+00093d30: 3430 2e36 3937 3838 343c 2f74 643e 0a20  40.697884</td>. 
+00093d40: 2020 2020 203c 7464 3e2d 3733 2e39 3932       <td>-73.992
+00093d50: 3830 353c 2f74 643e 0a20 2020 2020 203c  805</td>.      <
+00093d60: 7464 3e53 756e 6461 793c 2f74 643e 0a20  td>Sunday</td>. 
+00093d70: 2020 2020 203c 7464 3e31 353c 2f74 643e       <td>15</td>
+00093d80: 0a20 2020 2020 203c 7464 3e33 3830 3930  .      <td>38090
+00093d90: 3c2f 7464 3e0a 2020 2020 2020 3c74 643e  </td>.      <td>
+00093da0: 5368 6f70 2026 616d 703b 2053 6572 7669  Shop &amp; Servi
+00093db0: 6365 3c2f 7464 3e0a 2020 2020 2020 3c74  ce</td>.      <t
+00093dc0: 643e 2d39 3939 3c2f 7464 3e0a 2020 2020  d>-999</td>.    
+00093dd0: 2020 3c74 643e 352e 323c 2f74 643e 0a20    <td>5.2</td>. 
+00093de0: 2020 2020 203c 7464 3e43 6c6f 7564 733c       <td>Clouds<
+00093df0: 2f74 643e 0a20 2020 2020 203c 7464 3e32  /td>.      <td>2
+00093e00: 3935 3536 3c2f 7464 3e0a 2020 2020 2020  9556</td>.      
+00093e10: 3c74 643e 3130 3730 3c2f 7464 3e0a 2020  <td>1070</td>.  
+00093e20: 2020 3c2f 7472 3e0a 2020 2020 3c74 723e    </tr>.    <tr>
+00093e30: 0a20 2020 2020 203c 7468 3e32 3231 3531  .      <th>22151
+00093e40: 3c2f 7468 3e0a 2020 2020 2020 3c74 643e  </th>.      <td>
+00093e50: 3430 2e36 3938 3239 313c 2f74 643e 0a20  40.698291</td>. 
+00093e60: 2020 2020 203c 7464 3e2d 3733 2e39 3936       <td>-73.996
+00093e70: 3633 323c 2f74 643e 0a20 2020 2020 203c  632</td>.      <
+00093e80: 7464 3e53 756e 6461 793c 2f74 643e 0a20  td>Sunday</td>. 
+00093e90: 2020 2020 203c 7464 3e31 383c 2f74 643e       <td>18</td>
+00093ea0: 0a20 2020 2020 203c 7464 3e33 3335 3338  .      <td>33538
+00093eb0: 3c2f 7464 3e0a 2020 2020 2020 3c74 643e  </td>.      <td>
+00093ec0: 4f75 7464 6f6f 7273 2026 616d 703b 2052  Outdoors &amp; R
+00093ed0: 6563 7265 6174 696f 6e3c 2f74 643e 0a20  ecreation</td>. 
+00093ee0: 2020 2020 203c 7464 3e2d 3939 393c 2f74       <td>-999</t
+00093ef0: 643e 0a20 2020 2020 203c 7464 3e39 2e36  d>.      <td>9.6
+00093f00: 3c2f 7464 3e0a 2020 2020 2020 3c74 643e  </td>.      <td>
+00093f10: 436c 6f75 6473 3c2f 7464 3e0a 2020 2020  Clouds</td>.    
+00093f20: 2020 3c74 643e 3239 3535 363c 2f74 643e    <td>29556</td>
+00093f30: 0a20 2020 2020 203c 7464 3e31 3037 303c  .      <td>1070<
+00093f40: 2f74 643e 0a20 2020 203c 2f74 723e 0a20  /td>.    </tr>. 
+00093f50: 2020 203c 7472 3e0a 2020 2020 2020 3c74     <tr>.      <t
+00093f60: 683e 3232 3135 323c 2f74 683e 0a20 2020  h>22152</th>.   
+00093f70: 2020 203c 7464 3e34 302e 3639 3234 3231     <td>40.692421
+00093f80: 3c2f 7464 3e0a 2020 2020 2020 3c74 643e  </td>.      <td>
+00093f90: 2d37 332e 3939 3430 3032 3c2f 7464 3e0a  -73.994002</td>.
+00093fa0: 2020 2020 2020 3c74 643e 5375 6e64 6179        <td>Sunday
+00093fb0: 3c2f 7464 3e0a 2020 2020 2020 3c74 643e  </td>.      <td>
+00093fc0: 3138 3c2f 7464 3e0a 2020 2020 2020 3c74  18</td>.      <t
+00093fd0: 643e 3239 3231 323c 2f74 643e 0a20 2020  d>29212</td>.   
+00093fe0: 2020 203c 7464 3e50 726f 6665 7373 696f     <td>Professio
+00093ff0: 6e61 6c20 2661 6d70 3b20 4f74 6865 7220  nal &amp; Other 
+00094000: 506c 6163 6573 3c2f 7464 3e0a 2020 2020  Places</td>.    
+00094010: 2020 3c74 643e 2d39 3939 3c2f 7464 3e0a    <td>-999</td>.
+00094020: 2020 2020 2020 3c74 643e 2d39 3939 2e30        <td>-999.0
+00094030: 3c2f 7464 3e0a 2020 2020 2020 3c74 643e  </td>.      <td>
+00094040: 436c 6f75 6473 3c2f 7464 3e0a 2020 2020  Clouds</td>.    
+00094050: 2020 3c74 643e 3239 3535 363c 2f74 643e    <td>29556</td>
+00094060: 0a20 2020 2020 203c 7464 3e31 3037 303c  .      <td>1070<
+00094070: 2f74 643e 0a20 2020 203c 2f74 723e 0a20  /td>.    </tr>. 
+00094080: 203c 2f74 626f 6479 3e0a 3c2f 7461 626c   </tbody>.</tabl
+00094090: 653e 0a3c 703e 3436 3738 3520 726f 7773  e>.<p>46785 rows
+000940a0: 20c3 9720 3131 2063 6f6c 756d 6e73 3c2f   .. 11 columns</
+000940b0: 703e 0a3c 2f64 6976 3e0a 3c2f 6469 763e  p>.</div>.</div>
+000940c0: 0a0a 3c2f 6469 763e 0a0a 3c2f 6469 763e  ..</div>..</div>
+000940d0: 0a0a 3c2f 6469 763e 0a0a 3c2f 6469 763e  ..</div>..</div>
+000940e0: 0a3c 6469 7620 636c 6173 733d 226a 702d  .<div class="jp-
+000940f0: 4365 6c6c 206a 702d 4d61 726b 646f 776e  Cell jp-Markdown
+00094100: 4365 6c6c 206a 702d 4e6f 7465 626f 6f6b  Cell jp-Notebook
+00094110: 2d63 656c 6c22 3e0a 3c64 6976 2063 6c61  -cell">.<div cla
+00094120: 7373 3d22 6a70 2d43 656c 6c2d 696e 7075  ss="jp-Cell-inpu
+00094130: 7457 7261 7070 6572 223e 0a3c 6469 7620  tWrapper">.<div 
+00094140: 636c 6173 733d 226a 702d 436f 6c6c 6170  class="jp-Collap
+00094150: 7365 7220 6a70 2d49 6e70 7574 436f 6c6c  ser jp-InputColl
+00094160: 6170 7365 7220 6a70 2d43 656c 6c2d 696e  apser jp-Cell-in
+00094170: 7075 7443 6f6c 6c61 7073 6572 223e 0a3c  putCollapser">.<
+00094180: 2f64 6976 3e0a 3c64 6976 2063 6c61 7373  /div>.<div class
+00094190: 3d22 6a70 2d49 6e70 7574 4172 6561 206a  ="jp-InputArea j
+000941a0: 702d 4365 6c6c 2d69 6e70 7574 4172 6561  p-Cell-inputArea
+000941b0: 223e 3c64 6976 2063 6c61 7373 3d22 6a70  "><div class="jp
+000941c0: 2d49 6e70 7574 5072 6f6d 7074 206a 702d  -InputPrompt jp-
+000941d0: 496e 7075 7441 7265 612d 7072 6f6d 7074  InputArea-prompt
+000941e0: 223e 0a3c 2f64 6976 3e3c 6469 7620 636c  ">.</div><div cl
+000941f0: 6173 733d 226a 702d 5265 6e64 6572 6564  ass="jp-Rendered
+00094200: 4854 4d4c 436f 6d6d 6f6e 206a 702d 5265  HTMLCommon jp-Re
+00094210: 6e64 6572 6564 4d61 726b 646f 776e 206a  nderedMarkdown j
+00094220: 702d 4d61 726b 646f 776e 4f75 7470 7574  p-MarkdownOutput
+00094230: 2022 2064 6174 612d 6d69 6d65 2d74 7970   " data-mime-typ
+00094240: 653d 2274 6578 742f 6d61 726b 646f 776e  e="text/markdown
+00094250: 223e 0a3c 703e 4f72 2c20 796f 7520 6361  ">.<p>Or, you ca
+00094260: 6e20 686f 6c64 206f 7574 2073 706c 6974  n hold out split
+00094270: 206f 6e20 616e 6f74 6865 7220 7072 6f70   on another prop
+00094280: 6f72 7469 6f6e 2028 3530 2520 666f 7220  ortion (50% for 
+00094290: 696e 7374 616e 6365 293a 3c2f 703e 0a0a  instance):</p>..
+000942a0: 3c2f 6469 763e 0a3c 2f64 6976 3e0a 3c2f  </div>.</div>.</
+000942b0: 6469 763e 0a3c 2f64 6976 3e3c 6469 7620  div>.</div><div 
+000942c0: 636c 6173 733d 226a 702d 4365 6c6c 206a  class="jp-Cell j
+000942d0: 702d 436f 6465 4365 6c6c 206a 702d 4e6f  p-CodeCell jp-No
+000942e0: 7465 626f 6f6b 2d63 656c 6c20 2020 223e  tebook-cell   ">
+000942f0: 0a3c 6469 7620 636c 6173 733d 226a 702d  .<div class="jp-
+00094300: 4365 6c6c 2d69 6e70 7574 5772 6170 7065  Cell-inputWrappe
+00094310: 7222 3e0a 3c64 6976 2063 6c61 7373 3d22  r">.<div class="
+00094320: 6a70 2d43 6f6c 6c61 7073 6572 206a 702d  jp-Collapser jp-
+00094330: 496e 7075 7443 6f6c 6c61 7073 6572 206a  InputCollapser j
+00094340: 702d 4365 6c6c 2d69 6e70 7574 436f 6c6c  p-Cell-inputColl
+00094350: 6170 7365 7222 3e0a 3c2f 6469 763e 0a3c  apser">.</div>.<
+00094360: 6469 7620 636c 6173 733d 226a 702d 496e  div class="jp-In
+00094370: 7075 7441 7265 6120 6a70 2d43 656c 6c2d  putArea jp-Cell-
+00094380: 696e 7075 7441 7265 6122 3e0a 3c64 6976  inputArea">.<div
+00094390: 2063 6c61 7373 3d22 6a70 2d49 6e70 7574   class="jp-Input
+000943a0: 5072 6f6d 7074 206a 702d 496e 7075 7441  Prompt jp-InputA
+000943b0: 7265 612d 7072 6f6d 7074 223e 496e 266e  rea-prompt">In&n
+000943c0: 6273 703b 5b31 355d 3a3c 2f64 6976 3e0a  bsp;[15]:</div>.
+000943d0: 3c64 6976 2063 6c61 7373 3d22 6a70 2d43  <div class="jp-C
+000943e0: 6f64 654d 6972 726f 7245 6469 746f 7220  odeMirrorEditor 
+000943f0: 6a70 2d45 6469 746f 7220 6a70 2d49 6e70  jp-Editor jp-Inp
+00094400: 7574 4172 6561 2d65 6469 746f 7222 2064  utArea-editor" d
+00094410: 6174 612d 7479 7065 3d22 696e 6c69 6e65  ata-type="inline
+00094420: 223e 0a20 2020 2020 3c64 6976 2063 6c61  ">.     <div cla
+00094430: 7373 3d22 436f 6465 4d69 7272 6f72 2063  ss="CodeMirror c
+00094440: 6d2d 732d 6a75 7079 7465 7222 3e0a 3c64  m-s-jupyter">.<d
+00094450: 6976 2063 6c61 7373 3d22 2068 6967 686c  iv class=" highl
+00094460: 6967 6874 2068 6c2d 6970 7974 686f 6e33  ight hl-ipython3
+00094470: 223e 3c70 7265 3e3c 7370 616e 3e3c 2f73  "><pre><span></s
+00094480: 7061 6e3e 3c73 7061 6e20 636c 6173 733d  pan><span class=
+00094490: 226e 223e 6466 5f74 7261 696e 3c2f 7370  "n">df_train</sp
+000944a0: 616e 3e3c 7370 616e 2063 6c61 7373 3d22  an><span class="
+000944b0: 7022 3e2c 3c2f 7370 616e 3e20 3c73 7061  p">,</span> <spa
+000944c0: 6e20 636c 6173 733d 226e 223e 6466 5f74  n class="n">df_t
+000944d0: 6573 743c 2f73 7061 6e3e 203c 7370 616e  est</span> <span
+000944e0: 2063 6c61 7373 3d22 6f22 3e3d 3c2f 7370   class="o">=</sp
+000944f0: 616e 3e20 3c73 7061 6e20 636c 6173 733d  an> <span class=
+00094500: 226e 223e 6c6f 6164 5f64 735f 686f 6c64  "n">load_ds_hold
+00094510: 6f75 743c 2f73 7061 6e3e 3c73 7061 6e20  out</span><span 
+00094520: 636c 6173 733d 2270 223e 283c 2f73 7061  class="p">(</spa
+00094530: 6e3e 3c73 7061 6e20 636c 6173 733d 226e  n><span class="n
+00094540: 223e 7472 6169 6e5f 7369 7a65 3c2f 7370  ">train_size</sp
+00094550: 616e 3e3c 7370 616e 2063 6c61 7373 3d22  an><span class="
+00094560: 6f22 3e3d 3c2f 7370 616e 3e3c 7370 616e  o">=</span><span
+00094570: 2063 6c61 7373 3d22 6d66 223e 302e 353c   class="mf">0.5<
+00094580: 2f73 7061 6e3e 3c73 7061 6e20 636c 6173  /span><span clas
+00094590: 733d 2270 223e 293c 2f73 7061 6e3e 0a0a  s="p">)</span>..
+000945a0: 3c73 7061 6e20 636c 6173 733d 2263 3122  <span class="c1"
+000945b0: 3e23 2054 6865 2073 706c 6974 2069 7320  ># The split is 
+000945c0: 636c 6173 732d 6261 6c61 6e63 6564 2c20  class-balanced, 
+000945d0: 7468 7573 2074 7261 696e 2061 6e64 2074  thus train and t
+000945e0: 6573 7420 6e75 6d62 6572 206f 6620 7472  est number of tr
+000945f0: 616a 6563 746f 7269 6573 206d 6179 206e  ajectories may n
+00094600: 6f74 2062 6520 6578 6163 746c 7920 7072  ot be exactly pr
+00094610: 6f70 6f72 7469 6f6e 616c 2e3c 2f73 7061  oportional.</spa
+00094620: 6e3e 0a3c 7370 616e 2063 6c61 7373 3d22  n>.<span class="
+00094630: 6e62 223e 7072 696e 743c 2f73 7061 6e3e  nb">print</span>
+00094640: 3c73 7061 6e20 636c 6173 733d 2270 223e  <span class="p">
+00094650: 283c 2f73 7061 6e3e 3c73 7061 6e20 636c  (</span><span cl
+00094660: 6173 733d 226e 223e 6466 5f74 7261 696e  ass="n">df_train
+00094670: 3c2f 7370 616e 3e3c 7370 616e 2063 6c61  </span><span cla
+00094680: 7373 3d22 6f22 3e2e 3c2f 7370 616e 3e3c  ss="o">.</span><
+00094690: 7370 616e 2063 6c61 7373 3d22 6e22 3e73  span class="n">s
+000946a0: 6861 7065 3c2f 7370 616e 3e3c 7370 616e  hape</span><span
+000946b0: 2063 6c61 7373 3d22 7022 3e2c 3c2f 7370   class="p">,</sp
+000946c0: 616e 3e20 3c73 7061 6e20 636c 6173 733d  an> <span class=
+000946d0: 226e 223e 6466 5f74 6573 743c 2f73 7061  "n">df_test</spa
+000946e0: 6e3e 3c73 7061 6e20 636c 6173 733d 226f  n><span class="o
+000946f0: 223e 2e3c 2f73 7061 6e3e 3c73 7061 6e20  ">.</span><span 
+00094700: 636c 6173 733d 226e 223e 7368 6170 653c  class="n">shape<
+00094710: 2f73 7061 6e3e 3c73 7061 6e20 636c 6173  /span><span clas
+00094720: 733d 2270 223e 293c 2f73 7061 6e3e 200a  s="p">)</span> .
+00094730: 0a3c 7370 616e 2063 6c61 7373 3d22 6e22  .<span class="n"
+00094740: 3e64 665f 7472 6169 6e3c 2f73 7061 6e3e  >df_train</span>
+00094750: 0a3c 2f70 7265 3e3c 2f64 6976 3e0a 0a20  .</pre></div>.. 
+00094760: 2020 2020 3c2f 6469 763e 0a3c 2f64 6976      </div>.</div
+00094770: 3e0a 3c2f 6469 763e 0a3c 2f64 6976 3e0a  >.</div>.</div>.
+00094780: 0a3c 6469 7620 636c 6173 733d 226a 702d  .<div class="jp-
+00094790: 4365 6c6c 2d6f 7574 7075 7457 7261 7070  Cell-outputWrapp
+000947a0: 6572 223e 0a3c 6469 7620 636c 6173 733d  er">.<div class=
+000947b0: 226a 702d 436f 6c6c 6170 7365 7220 6a70  "jp-Collapser jp
+000947c0: 2d4f 7574 7075 7443 6f6c 6c61 7073 6572  -OutputCollapser
+000947d0: 206a 702d 4365 6c6c 2d6f 7574 7075 7443   jp-Cell-outputC
+000947e0: 6f6c 6c61 7073 6572 223e 0a3c 2f64 6976  ollapser">.</div
+000947f0: 3e0a 0a0a 3c64 6976 2063 6c61 7373 3d22  >...<div class="
+00094800: 6a70 2d4f 7574 7075 7441 7265 6120 6a70  jp-OutputArea jp
+00094810: 2d43 656c 6c2d 6f75 7470 7574 4172 6561  -Cell-outputArea
+00094820: 223e 0a0a 3c64 6976 2063 6c61 7373 3d22  ">..<div class="
+00094830: 6a70 2d4f 7574 7075 7441 7265 612d 6368  jp-OutputArea-ch
+00094840: 696c 6422 3e0a 0a20 2020 200a 2020 2020  ild">..    .    
+00094850: 3c64 6976 2063 6c61 7373 3d22 6a70 2d4f  <div class="jp-O
+00094860: 7574 7075 7450 726f 6d70 7420 6a70 2d4f  utputPrompt jp-O
+00094870: 7574 7075 7441 7265 612d 7072 6f6d 7074  utputArea-prompt
+00094880: 223e 3c2f 6469 763e 0a0a 0a3c 6469 7620  "></div>...<div 
+00094890: 636c 6173 733d 226a 702d 5265 6e64 6572  class="jp-Render
+000948a0: 6564 5465 7874 206a 702d 4f75 7470 7574  edText jp-Output
+000948b0: 4172 6561 2d6f 7574 7075 7422 2064 6174  Area-output" dat
+000948c0: 612d 6d69 6d65 2d74 7970 653d 2274 6578  a-mime-type="tex
+000948d0: 742f 706c 6169 6e22 3e0a 3c70 7265 3e4c  t/plain">.<pre>L
+000948e0: 6f61 6469 6e67 2064 6174 6173 6574 2066  oading dataset f
+000948f0: 696c 653a 2068 7474 7073 3a2f 2f67 6974  ile: https://git
+00094900: 6875 622e 636f 6d2f 6d61 742d 616e 616c  hub.com/mat-anal
+00094910: 7973 6973 2f64 6174 6173 6574 732f 7261  ysis/datasets/ra
+00094920: 772f 6d61 696e 2f6d 6174 2f46 6f75 7273  w/main/mat/Fours
+00094930: 7175 6172 654e 5943 2f0a 3c2f 7072 653e  quareNYC/.</pre>
+00094940: 0a3c 2f64 6976 3e0a 3c2f 6469 763e 0a0a  .</div>.</div>..
+00094950: 3c64 6976 2063 6c61 7373 3d22 6a70 2d4f  <div class="jp-O
+00094960: 7574 7075 7441 7265 612d 6368 696c 6422  utputArea-child"
+00094970: 3e0a 0a20 2020 200a 2020 2020 3c64 6976  >..    .    <div
+00094980: 2063 6c61 7373 3d22 6a70 2d4f 7574 7075   class="jp-Outpu
+00094990: 7450 726f 6d70 7420 6a70 2d4f 7574 7075  tPrompt jp-Outpu
+000949a0: 7441 7265 612d 7072 6f6d 7074 223e 3c2f  tArea-prompt"></
+000949b0: 6469 763e 0a0a 0a0a 0a3c 6469 7620 636c  div>.....<div cl
+000949c0: 6173 733d 226a 702d 5265 6e64 6572 6564  ass="jp-Rendered
+000949d0: 5465 7874 206a 702d 4f75 7470 7574 4172  Text jp-OutputAr
+000949e0: 6561 2d6f 7574 7075 7420 2220 6461 7461  ea-output " data
+000949f0: 2d6d 696d 652d 7479 7065 3d22 7465 7874  -mime-type="text
+00094a00: 2f70 6c61 696e 223e 0a3c 7072 653e 2020  /plain">.<pre>  
+00094a10: 3025 7c20 2020 2020 2020 2020 207c 2030  0%|          | 0
+00094a20: 2f31 3933 205b 3030 3a30 3026 6c74 3b3f  /193 [00:00&lt;?
+00094a30: 2c20 3f69 742f 735d 3c2f 7072 653e 0a3c  , ?it/s]</pre>.<
+00094a40: 2f64 6976 3e0a 0a3c 2f64 6976 3e0a 0a3c  /div>..</div>..<
+00094a50: 6469 7620 636c 6173 733d 226a 702d 4f75  div class="jp-Ou
+00094a60: 7470 7574 4172 6561 2d63 6869 6c64 223e  tputArea-child">
+00094a70: 0a0a 2020 2020 0a20 2020 203c 6469 7620  ..    .    <div 
+00094a80: 636c 6173 733d 226a 702d 4f75 7470 7574  class="jp-Output
+00094a90: 5072 6f6d 7074 206a 702d 4f75 7470 7574  Prompt jp-Output
+00094aa0: 4172 6561 2d70 726f 6d70 7422 3e3c 2f64  Area-prompt"></d
+00094ab0: 6976 3e0a 0a0a 3c64 6976 2063 6c61 7373  iv>...<div class
+00094ac0: 3d22 6a70 2d52 656e 6465 7265 6454 6578  ="jp-RenderedTex
+00094ad0: 7420 6a70 2d4f 7574 7075 7441 7265 612d  t jp-OutputArea-
+00094ae0: 6f75 7470 7574 2220 6461 7461 2d6d 696d  output" data-mim
+00094af0: 652d 7479 7065 3d22 7465 7874 2f70 6c61  e-type="text/pla
+00094b00: 696e 223e 0a3c 7072 653e 2833 3337 3733  in">.<pre>(33773
+00094b10: 2c20 3131 2920 2833 3331 3839 2c20 3131  , 11) (33189, 11
+00094b20: 290a 3c2f 7072 653e 0a3c 2f64 6976 3e0a  ).</pre>.</div>.
+00094b30: 3c2f 6469 763e 0a0a 3c64 6976 2063 6c61  </div>..<div cla
+00094b40: 7373 3d22 6a70 2d4f 7574 7075 7441 7265  ss="jp-OutputAre
+00094b50: 612d 6368 696c 6422 3e0a 0a20 2020 200a  a-child">..    .
+00094b60: 2020 2020 3c64 6976 2063 6c61 7373 3d22      <div class="
+00094b70: 6a70 2d4f 7574 7075 7450 726f 6d70 7420  jp-OutputPrompt 
+00094b80: 6a70 2d4f 7574 7075 7441 7265 612d 7072  jp-OutputArea-pr
+00094b90: 6f6d 7074 223e 4f75 745b 3135 5d3a 3c2f  ompt">Out[15]:</
+00094ba0: 6469 763e 0a0a 0a0a 3c64 6976 2063 6c61  div>....<div cla
+00094bb0: 7373 3d22 6a70 2d52 656e 6465 7265 6448  ss="jp-RenderedH
+00094bc0: 544d 4c43 6f6d 6d6f 6e20 6a70 2d52 656e  TMLCommon jp-Ren
+00094bd0: 6465 7265 6448 544d 4c20 6a70 2d4f 7574  deredHTML jp-Out
+00094be0: 7075 7441 7265 612d 6f75 7470 7574 206a  putArea-output j
+00094bf0: 702d 4f75 7470 7574 4172 6561 2d65 7865  p-OutputArea-exe
+00094c00: 6375 7465 5265 7375 6c74 2220 6461 7461  cuteResult" data
+00094c10: 2d6d 696d 652d 7479 7065 3d22 7465 7874  -mime-type="text
+00094c20: 2f68 746d 6c22 3e0a 3c64 6976 3e0a 3c73  /html">.<div>.<s
+00094c30: 7479 6c65 2073 636f 7065 643e 0a20 2020  tyle scoped>.   
+00094c40: 202e 6461 7461 6672 616d 6520 7462 6f64   .dataframe tbod
+00094c50: 7920 7472 2074 683a 6f6e 6c79 2d6f 662d  y tr th:only-of-
+00094c60: 7479 7065 207b 0a20 2020 2020 2020 2076  type {.        v
+00094c70: 6572 7469 6361 6c2d 616c 6967 6e3a 206d  ertical-align: m
+00094c80: 6964 646c 653b 0a20 2020 207d 0a0a 2020  iddle;.    }..  
+00094c90: 2020 2e64 6174 6166 7261 6d65 2074 626f    .dataframe tbo
+00094ca0: 6479 2074 7220 7468 207b 0a20 2020 2020  dy tr th {.     
+00094cb0: 2020 2076 6572 7469 6361 6c2d 616c 6967     vertical-alig
+00094cc0: 6e3a 2074 6f70 3b0a 2020 2020 7d0a 0a20  n: top;.    }.. 
+00094cd0: 2020 202e 6461 7461 6672 616d 6520 7468     .dataframe th
+00094ce0: 6561 6420 7468 207b 0a20 2020 2020 2020  ead th {.       
+00094cf0: 2074 6578 742d 616c 6967 6e3a 2072 6967   text-align: rig
+00094d00: 6874 3b0a 2020 2020 7d0a 3c2f 7374 796c  ht;.    }.</styl
+00094d10: 653e 0a3c 7461 626c 6520 626f 7264 6572  e>.<table border
+00094d20: 3d22 3122 2063 6c61 7373 3d22 6461 7461  ="1" class="data
+00094d30: 6672 616d 6522 3e0a 2020 3c74 6865 6164  frame">.  <thead
+00094d40: 3e0a 2020 2020 3c74 7220 7374 796c 653d  >.    <tr style=
+00094d50: 2274 6578 742d 616c 6967 6e3a 2072 6967  "text-align: rig
+00094d60: 6874 3b22 3e0a 2020 2020 2020 3c74 683e  ht;">.      <th>
+00094d70: 3c2f 7468 3e0a 2020 2020 2020 3c74 683e  </th>.      <th>
+00094d80: 6c61 743c 2f74 683e 0a20 2020 2020 203c  lat</th>.      <
+00094d90: 7468 3e6c 6f6e 3c2f 7468 3e0a 2020 2020  th>lon</th>.    
+00094da0: 2020 3c74 683e 6461 793c 2f74 683e 0a20    <th>day</th>. 
+00094db0: 2020 2020 203c 7468 3e68 6f75 723c 2f74       <th>hour</t
+00094dc0: 683e 0a20 2020 2020 203c 7468 3e70 6f69  h>.      <th>poi
+00094dd0: 3c2f 7468 3e0a 2020 2020 2020 3c74 683e  </th>.      <th>
+00094de0: 6361 7465 676f 7279 3c2f 7468 3e0a 2020  category</th>.  
+00094df0: 2020 2020 3c74 683e 7072 6963 653c 2f74      <th>price</t
+00094e00: 683e 0a20 2020 2020 203c 7468 3e72 6174  h>.      <th>rat
+00094e10: 696e 673c 2f74 683e 0a20 2020 2020 203c  ing</th>.      <
+00094e20: 7468 3e77 6561 7468 6572 3c2f 7468 3e0a  th>weather</th>.
+00094e30: 2020 2020 2020 3c74 683e 7469 643c 2f74        <th>tid</t
+00094e40: 683e 0a20 2020 2020 203c 7468 3e6c 6162  h>.      <th>lab
+00094e50: 656c 3c2f 7468 3e0a 2020 2020 3c2f 7472  el</th>.    </tr
+00094e60: 3e0a 2020 3c2f 7468 6561 643e 0a20 203c  >.  </thead>.  <
+00094e70: 7462 6f64 793e 0a20 2020 203c 7472 3e0a  tbody>.    <tr>.
+00094e80: 2020 2020 2020 3c74 683e 303c 2f74 683e        <th>0</th>
+00094e90: 0a20 2020 2020 203c 7464 3e34 302e 3833  .      <td>40.83
+00094ea0: 3430 3938 3c2f 7464 3e0a 2020 2020 2020  4098</td>.      
+00094eb0: 3c74 643e 2d37 332e 3934 3532 3637 3c2f  <td>-73.945267</
+00094ec0: 7464 3e0a 2020 2020 2020 3c74 643e 4d6f  td>.      <td>Mo
+00094ed0: 6e64 6179 3c2f 7464 3e0a 2020 2020 2020  nday</td>.      
+00094ee0: 3c74 643e 3133 3c2f 7464 3e0a 2020 2020  <td>13</td>.    
+00094ef0: 2020 3c74 643e 3231 3538 303c 2f74 643e    <td>21580</td>
+00094f00: 0a20 2020 2020 203c 7464 3e46 6f6f 643c  .      <td>Food<
+00094f10: 2f74 643e 0a20 2020 2020 203c 7464 3e31  /td>.      <td>1
+00094f20: 3c2f 7464 3e0a 2020 2020 2020 3c74 643e  </td>.      <td>
+00094f30: 382e 323c 2f74 643e 0a20 2020 2020 203c  8.2</td>.      <
+00094f40: 7464 3e43 6c6f 7564 733c 2f74 643e 0a20  td>Clouds</td>. 
+00094f50: 2020 2020 203c 7464 3e31 3237 3c2f 7464       <td>127</td
+00094f60: 3e0a 2020 2020 2020 3c74 643e 363c 2f74  >.      <td>6</t
+00094f70: 643e 0a20 2020 203c 2f74 723e 0a20 2020  d>.    </tr>.   
+00094f80: 203c 7472 3e0a 2020 2020 2020 3c74 683e   <tr>.      <th>
+00094f90: 313c 2f74 683e 0a20 2020 2020 203c 7464  1</th>.      <td
+00094fa0: 3e34 302e 3536 3731 3936 3c2f 7464 3e0a  >40.567196</td>.
+00094fb0: 2020 2020 2020 3c74 643e 2d37 332e 3838        <td>-73.88
+00094fc0: 3235 3736 3c2f 7464 3e0a 2020 2020 2020  2576</td>.      
+00094fd0: 3c74 643e 4d6f 6e64 6179 3c2f 7464 3e0a  <td>Monday</td>.
+00094fe0: 2020 2020 2020 3c74 643e 3139 3c2f 7464        <td>19</td
+00094ff0: 3e0a 2020 2020 2020 3c74 643e 3233 3932  >.      <td>2392
+00095000: 3c2f 7464 3e0a 2020 2020 2020 3c74 643e  </td>.      <td>
+00095010: 5472 6176 656c 2026 616d 703b 2054 7261  Travel &amp; Tra
+00095020: 6e73 706f 7274 3c2f 7464 3e0a 2020 2020  nsport</td>.    
+00095030: 2020 3c74 643e 2d39 3939 3c2f 7464 3e0a    <td>-999</td>.
+00095040: 2020 2020 2020 3c74 643e 2d39 3939 2e30        <td>-999.0
+00095050: 3c2f 7464 3e0a 2020 2020 2020 3c74 643e  </td>.      <td>
+00095060: 436c 6f75 6473 3c2f 7464 3e0a 2020 2020  Clouds</td>.    
+00095070: 2020 3c74 643e 3132 373c 2f74 643e 0a20    <td>127</td>. 
+00095080: 2020 2020 203c 7464 3e36 3c2f 7464 3e0a       <td>6</td>.
+00095090: 2020 2020 3c2f 7472 3e0a 2020 2020 3c74      </tr>.    <t
+000950a0: 723e 0a20 2020 2020 203c 7468 3e32 3c2f  r>.      <th>2</
+000950b0: 7468 3e0a 2020 2020 2020 3c74 643e 3430  th>.      <td>40
+000950c0: 2e36 3839 3931 333c 2f74 643e 0a20 2020  .689913</td>.   
+000950d0: 2020 203c 7464 3e2d 3733 2e39 3831 3530     <td>-73.98150
+000950e0: 343c 2f74 643e 0a20 2020 2020 203c 7464  4</td>.      <td
+000950f0: 3e4d 6f6e 6461 793c 2f74 643e 0a20 2020  >Monday</td>.   
+00095100: 2020 203c 7464 3e32 333c 2f74 643e 0a20     <td>23</td>. 
+00095110: 2020 2020 203c 7464 3e33 3535 3839 3c2f       <td>35589</
+00095120: 7464 3e0a 2020 2020 2020 3c74 643e 5472  td>.      <td>Tr
+00095130: 6176 656c 2026 616d 703b 2054 7261 6e73  avel &amp; Trans
+00095140: 706f 7274 3c2f 7464 3e0a 2020 2020 2020  port</td>.      
+00095150: 3c74 643e 2d39 3939 3c2f 7464 3e0a 2020  <td>-999</td>.  
+00095160: 2020 2020 3c74 643e 2d39 3939 2e30 3c2f      <td>-999.0</
+00095170: 7464 3e0a 2020 2020 2020 3c74 643e 436c  td>.      <td>Cl
+00095180: 6f75 6473 3c2f 7464 3e0a 2020 2020 2020  ouds</td>.      
+00095190: 3c74 643e 3132 373c 2f74 643e 0a20 2020  <td>127</td>.   
+000951a0: 2020 203c 7464 3e36 3c2f 7464 3e0a 2020     <td>6</td>.  
+000951b0: 2020 3c2f 7472 3e0a 2020 2020 3c74 723e    </tr>.    <tr>
+000951c0: 0a20 2020 2020 203c 7468 3e33 3c2f 7468  .      <th>3</th
+000951d0: 3e0a 2020 2020 2020 3c74 643e 3430 2e37  >.      <td>40.7
+000951e0: 3038 3538 383c 2f74 643e 0a20 2020 2020  08588</td>.     
+000951f0: 203c 7464 3e2d 3733 2e39 3931 3033 323c   <td>-73.991032<
+00095200: 2f74 643e 0a20 2020 2020 203c 7464 3e4d  /td>.      <td>M
+00095210: 6f6e 6461 793c 2f74 643e 0a20 2020 2020  onday</td>.     
+00095220: 203c 7464 3e32 333c 2f74 643e 0a20 2020   <td>23</td>.   
+00095230: 2020 203c 7464 3e31 3836 3033 3c2f 7464     <td>18603</td
+00095240: 3e0a 2020 2020 2020 3c74 643e 5472 6176  >.      <td>Trav
+00095250: 656c 2026 616d 703b 2054 7261 6e73 706f  el &amp; Transpo
+00095260: 7274 3c2f 7464 3e0a 2020 2020 2020 3c74  rt</td>.      <t
+00095270: 643e 2d39 3939 3c2f 7464 3e0a 2020 2020  d>-999</td>.    
+00095280: 2020 3c74 643e 2d39 3939 2e30 3c2f 7464    <td>-999.0</td
+00095290: 3e0a 2020 2020 2020 3c74 643e 436c 6f75  >.      <td>Clou
+000952a0: 6473 3c2f 7464 3e0a 2020 2020 2020 3c74  ds</td>.      <t
+000952b0: 643e 3132 373c 2f74 643e 0a20 2020 2020  d>127</td>.     
+000952c0: 203c 7464 3e36 3c2f 7464 3e0a 2020 2020   <td>6</td>.    
+000952d0: 3c2f 7472 3e0a 2020 2020 3c74 723e 0a20  </tr>.    <tr>. 
+000952e0: 2020 2020 203c 7468 3e34 3c2f 7468 3e0a       <th>4</th>.
+000952f0: 2020 2020 2020 3c74 643e 3430 2e38 3333        <td>40.833
+00095300: 3136 353c 2f74 643e 0a20 2020 2020 203c  165</td>.      <
+00095310: 7464 3e2d 3733 2e39 3431 3836 303c 2f74  td>-73.941860</t
+00095320: 643e 0a20 2020 2020 203c 7464 3e54 7565  d>.      <td>Tue
+00095330: 7364 6179 3c2f 7464 3e0a 2020 2020 2020  sday</td>.      
+00095340: 3c74 643e 3134 3c2f 7464 3e0a 2020 2020  <td>14</td>.    
+00095350: 2020 3c74 643e 3336 3334 383c 2f74 643e    <td>36348</td>
+00095360: 0a20 2020 2020 203c 7464 3e52 6573 6964  .      <td>Resid
+00095370: 656e 6365 3c2f 7464 3e0a 2020 2020 2020  ence</td>.      
+00095380: 3c74 643e 2d39 3939 3c2f 7464 3e0a 2020  <td>-999</td>.  
+00095390: 2020 2020 3c74 643e 2d39 3939 2e30 3c2f      <td>-999.0</
+000953a0: 7464 3e0a 2020 2020 2020 3c74 643e 436c  td>.      <td>Cl
+000953b0: 6561 723c 2f74 643e 0a20 2020 2020 203c  ear</td>.      <
+000953c0: 7464 3e31 3237 3c2f 7464 3e0a 2020 2020  td>127</td>.    
+000953d0: 2020 3c74 643e 363c 2f74 643e 0a20 2020    <td>6</td>.   
+000953e0: 203c 2f74 723e 0a20 2020 203c 7472 3e0a   </tr>.    <tr>.
+000953f0: 2020 2020 2020 3c74 683e 2e2e 2e3c 2f74        <th>...</t
+00095400: 683e 0a20 2020 2020 203c 7464 3e2e 2e2e  h>.      <td>...
+00095410: 3c2f 7464 3e0a 2020 2020 2020 3c74 643e  </td>.      <td>
+00095420: 2e2e 2e3c 2f74 643e 0a20 2020 2020 203c  ...</td>.      <
+00095430: 7464 3e2e 2e2e 3c2f 7464 3e0a 2020 2020  td>...</td>.    
+00095440: 2020 3c74 643e 2e2e 2e3c 2f74 643e 0a20    <td>...</td>. 
+00095450: 2020 2020 203c 7464 3e2e 2e2e 3c2f 7464       <td>...</td
+00095460: 3e0a 2020 2020 2020 3c74 643e 2e2e 2e3c  >.      <td>...<
+00095470: 2f74 643e 0a20 2020 2020 203c 7464 3e2e  /td>.      <td>.
+00095480: 2e2e 3c2f 7464 3e0a 2020 2020 2020 3c74  ..</td>.      <t
+00095490: 643e 2e2e 2e3c 2f74 643e 0a20 2020 2020  d>...</td>.     
+000954a0: 203c 7464 3e2e 2e2e 3c2f 7464 3e0a 2020   <td>...</td>.  
+000954b0: 2020 2020 3c74 643e 2e2e 2e3c 2f74 643e      <td>...</td>
+000954c0: 0a20 2020 2020 203c 7464 3e2e 2e2e 3c2f  .      <td>...</
+000954d0: 7464 3e0a 2020 2020 3c2f 7472 3e0a 2020  td>.    </tr>.  
+000954e0: 2020 3c74 723e 0a20 2020 2020 203c 7468    <tr>.      <th
+000954f0: 3e32 3231 3331 3c2f 7468 3e0a 2020 2020  >22131</th>.    
+00095500: 2020 3c74 643e 3430 2e37 3034 3733 333c    <td>40.704733<
+00095510: 2f74 643e 0a20 2020 2020 203c 7464 3e2d  /td>.      <td>-
+00095520: 3733 2e39 3837 3733 383c 2f74 643e 0a20  73.987738</td>. 
+00095530: 2020 2020 203c 7464 3e54 6875 7273 6461       <td>Thursda
+00095540: 793c 2f74 643e 0a20 2020 2020 203c 7464  y</td>.      <td
+00095550: 3e31 383c 2f74 643e 0a20 2020 2020 203c  >18</td>.      <
+00095560: 7464 3e31 3830 353c 2f74 643e 0a20 2020  td>1805</td>.   
+00095570: 2020 203c 7464 3e43 6f6c 6c65 6765 2026     <td>College &
+00095580: 616d 703b 2055 6e69 7665 7273 6974 793c  amp; University<
+00095590: 2f74 643e 0a20 2020 2020 203c 7464 3e2d  /td>.      <td>-
+000955a0: 3939 393c 2f74 643e 0a20 2020 2020 203c  999</td>.      <
+000955b0: 7464 3e2d 3939 392e 303c 2f74 643e 0a20  td>-999.0</td>. 
+000955c0: 2020 2020 203c 7464 3e43 6c65 6172 3c2f       <td>Clear</
+000955d0: 7464 3e0a 2020 2020 2020 3c74 643e 3239  td>.      <td>29
+000955e0: 3535 343c 2f74 643e 0a20 2020 2020 203c  554</td>.      <
+000955f0: 7464 3e31 3037 303c 2f74 643e 0a20 2020  td>1070</td>.   
+00095600: 203c 2f74 723e 0a20 2020 203c 7472 3e0a   </tr>.    <tr>.
+00095610: 2020 2020 2020 3c74 683e 3232 3133 323c        <th>22132<
+00095620: 2f74 683e 0a20 2020 2020 203c 7464 3e34  /th>.      <td>4
+00095630: 302e 3730 3432 3733 3c2f 7464 3e0a 2020  0.704273</td>.  
+00095640: 2020 2020 3c74 643e 2d37 332e 3938 3637      <td>-73.9867
+00095650: 3539 3c2f 7464 3e0a 2020 2020 2020 3c74  59</td>.      <t
+00095660: 643e 5468 7572 7364 6179 3c2f 7464 3e0a  d>Thursday</td>.
+00095670: 2020 2020 2020 3c74 643e 3139 3c2f 7464        <td>19</td
+00095680: 3e0a 2020 2020 2020 3c74 643e 3235 3436  >.      <td>2546
+00095690: 313c 2f74 643e 0a20 2020 2020 203c 7464  1</td>.      <td
+000956a0: 3e4f 7574 646f 6f72 7320 2661 6d70 3b20  >Outdoors &amp; 
+000956b0: 5265 6372 6561 7469 6f6e 3c2f 7464 3e0a  Recreation</td>.
+000956c0: 2020 2020 2020 3c74 643e 2d39 3939 3c2f        <td>-999</
+000956d0: 7464 3e0a 2020 2020 2020 3c74 643e 382e  td>.      <td>8.
+000956e0: 363c 2f74 643e 0a20 2020 2020 203c 7464  6</td>.      <td
+000956f0: 3e43 6c65 6172 3c2f 7464 3e0a 2020 2020  >Clear</td>.    
+00095700: 2020 3c74 643e 3239 3535 343c 2f74 643e    <td>29554</td>
+00095710: 0a20 2020 2020 203c 7464 3e31 3037 303c  .      <td>1070<
+00095720: 2f74 643e 0a20 2020 203c 2f74 723e 0a20  /td>.    </tr>. 
+00095730: 2020 203c 7472 3e0a 2020 2020 2020 3c74     <tr>.      <t
+00095740: 683e 3232 3133 333c 2f74 683e 0a20 2020  h>22133</th>.   
+00095750: 2020 203c 7464 3e34 302e 3639 3738 3033     <td>40.697803
+00095760: 3c2f 7464 3e0a 2020 2020 2020 3c74 643e  </td>.      <td>
+00095770: 2d37 332e 3939 3431 3435 3c2f 7464 3e0a  -73.994145</td>.
+00095780: 2020 2020 2020 3c74 643e 4672 6964 6179        <td>Friday
+00095790: 3c2f 7464 3e0a 2020 2020 2020 3c74 643e  </td>.      <td>
+000957a0: 3130 3c2f 7464 3e0a 2020 2020 2020 3c74  10</td>.      <t
+000957b0: 643e 3136 3435 323c 2f74 643e 0a20 2020  d>16452</td>.   
+000957c0: 2020 203c 7464 3e4f 7574 646f 6f72 7320     <td>Outdoors 
+000957d0: 2661 6d70 3b20 5265 6372 6561 7469 6f6e  &amp; Recreation
+000957e0: 3c2f 7464 3e0a 2020 2020 2020 3c74 643e  </td>.      <td>
+000957f0: 2d39 3939 3c2f 7464 3e0a 2020 2020 2020  -999</td>.      
+00095800: 3c74 643e 362e 393c 2f74 643e 0a20 2020  <td>6.9</td>.   
+00095810: 2020 203c 7464 3e43 6c65 6172 3c2f 7464     <td>Clear</td
+00095820: 3e0a 2020 2020 2020 3c74 643e 3239 3535  >.      <td>2955
+00095830: 343c 2f74 643e 0a20 2020 2020 203c 7464  4</td>.      <td
+00095840: 3e31 3037 303c 2f74 643e 0a20 2020 203c  >1070</td>.    <
+00095850: 2f74 723e 0a20 2020 203c 7472 3e0a 2020  /tr>.    <tr>.  
+00095860: 2020 2020 3c74 683e 3232 3133 343c 2f74      <th>22134</t
+00095870: 683e 0a20 2020 2020 203c 7464 3e34 302e  h>.      <td>40.
+00095880: 3639 3531 3633 3c2f 7464 3e0a 2020 2020  695163</td>.    
+00095890: 2020 3c74 643e 2d37 332e 3939 3534 3438    <td>-73.995448
+000958a0: 3c2f 7464 3e0a 2020 2020 2020 3c74 643e  </td>.      <td>
+000958b0: 4672 6964 6179 3c2f 7464 3e0a 2020 2020  Friday</td>.    
+000958c0: 2020 3c74 643e 3230 3c2f 7464 3e0a 2020    <td>20</td>.  
+000958d0: 2020 2020 3c74 643e 3139 3434 3c2f 7464      <td>1944</td
+000958e0: 3e0a 2020 2020 2020 3c74 643e 466f 6f64  >.      <td>Food
+000958f0: 3c2f 7464 3e0a 2020 2020 2020 3c74 643e  </td>.      <td>
+00095900: 323c 2f74 643e 0a20 2020 2020 203c 7464  2</td>.      <td
+00095910: 3e38 2e30 3c2f 7464 3e0a 2020 2020 2020  >8.0</td>.      
+00095920: 3c74 643e 436c 6561 723c 2f74 643e 0a20  <td>Clear</td>. 
+00095930: 2020 2020 203c 7464 3e32 3935 3534 3c2f       <td>29554</
+00095940: 7464 3e0a 2020 2020 2020 3c74 643e 3130  td>.      <td>10
+00095950: 3730 3c2f 7464 3e0a 2020 2020 3c2f 7472  70</td>.    </tr
+00095960: 3e0a 2020 2020 3c74 723e 0a20 2020 2020  >.    <tr>.     
+00095970: 203c 7468 3e32 3231 3335 3c2f 7468 3e0a   <th>22135</th>.
+00095980: 2020 2020 2020 3c74 643e 3430 2e36 3934        <td>40.694
+00095990: 3637 333c 2f74 643e 0a20 2020 2020 203c  673</td>.      <
+000959a0: 7464 3e2d 3733 2e39 3934 3038 323c 2f74  td>-73.994082</t
+000959b0: 643e 0a20 2020 2020 203c 7464 3e53 6174  d>.      <td>Sat
+000959c0: 7572 6461 793c 2f74 643e 0a20 2020 2020  urday</td>.     
+000959d0: 203c 7464 3e31 333c 2f74 643e 0a20 2020   <td>13</td>.   
+000959e0: 2020 203c 7464 3e31 3632 3031 3c2f 7464     <td>16201</td
+000959f0: 3e0a 2020 2020 2020 3c74 643e 466f 6f64  >.      <td>Food
+00095a00: 3c2f 7464 3e0a 2020 2020 2020 3c74 643e  </td>.      <td>
+00095a10: 313c 2f74 643e 0a20 2020 2020 203c 7464  1</td>.      <td
+00095a20: 3e37 2e30 3c2f 7464 3e0a 2020 2020 2020  >7.0</td>.      
+00095a30: 3c74 643e 436c 6561 723c 2f74 643e 0a20  <td>Clear</td>. 
+00095a40: 2020 2020 203c 7464 3e32 3935 3534 3c2f       <td>29554</
+00095a50: 7464 3e0a 2020 2020 2020 3c74 643e 3130  td>.      <td>10
+00095a60: 3730 3c2f 7464 3e0a 2020 2020 3c2f 7472  70</td>.    </tr
+00095a70: 3e0a 2020 3c2f 7462 6f64 793e 0a3c 2f74  >.  </tbody>.</t
+00095a80: 6162 6c65 3e0a 3c70 3e33 3337 3733 2072  able>.<p>33773 r
+00095a90: 6f77 7320 c397 2031 3120 636f 6c75 6d6e  ows .. 11 column
+00095aa0: 733c 2f70 3e0a 3c2f 6469 763e 0a3c 2f64  s</p>.</div>.</d
+00095ab0: 6976 3e0a 0a3c 2f64 6976 3e0a 0a3c 2f64  iv>..</div>..</d
+00095ac0: 6976 3e0a 0a3c 2f64 6976 3e0a 0a3c 2f64  iv>..</div>..</d
+00095ad0: 6976 3e0a 3c64 6976 2063 6c61 7373 3d22  iv>.<div class="
+00095ae0: 6a70 2d43 656c 6c20 6a70 2d4d 6172 6b64  jp-Cell jp-Markd
+00095af0: 6f77 6e43 656c 6c20 6a70 2d4e 6f74 6562  ownCell jp-Noteb
+00095b00: 6f6f 6b2d 6365 6c6c 223e 0a3c 6469 7620  ook-cell">.<div 
+00095b10: 636c 6173 733d 226a 702d 4365 6c6c 2d69  class="jp-Cell-i
+00095b20: 6e70 7574 5772 6170 7065 7222 3e0a 3c64  nputWrapper">.<d
+00095b30: 6976 2063 6c61 7373 3d22 6a70 2d43 6f6c  iv class="jp-Col
+00095b40: 6c61 7073 6572 206a 702d 496e 7075 7443  lapser jp-InputC
+00095b50: 6f6c 6c61 7073 6572 206a 702d 4365 6c6c  ollapser jp-Cell
+00095b60: 2d69 6e70 7574 436f 6c6c 6170 7365 7222  -inputCollapser"
+00095b70: 3e0a 3c2f 6469 763e 0a3c 6469 7620 636c  >.</div>.<div cl
+00095b80: 6173 733d 226a 702d 496e 7075 7441 7265  ass="jp-InputAre
+00095b90: 6120 6a70 2d43 656c 6c2d 696e 7075 7441  a jp-Cell-inputA
+00095ba0: 7265 6122 3e3c 6469 7620 636c 6173 733d  rea"><div class=
+00095bb0: 226a 702d 496e 7075 7450 726f 6d70 7420  "jp-InputPrompt 
+00095bc0: 6a70 2d49 6e70 7574 4172 6561 2d70 726f  jp-InputArea-pro
+00095bd0: 6d70 7422 3e0a 3c2f 6469 763e 3c64 6976  mpt">.</div><div
+00095be0: 2063 6c61 7373 3d22 6a70 2d52 656e 6465   class="jp-Rende
+00095bf0: 7265 6448 544d 4c43 6f6d 6d6f 6e20 6a70  redHTMLCommon jp
+00095c00: 2d52 656e 6465 7265 644d 6172 6b64 6f77  -RenderedMarkdow
+00095c10: 6e20 6a70 2d4d 6172 6b64 6f77 6e4f 7574  n jp-MarkdownOut
+00095c20: 7075 7420 2220 6461 7461 2d6d 696d 652d  put " data-mime-
+00095c30: 7479 7065 3d22 7465 7874 2f6d 6172 6b64  type="text/markd
+00095c40: 6f77 6e22 3e0a 0a3c 7072 653e 3c63 6f64  own">..<pre><cod
+00095c50: 653e 6329 204f 722c 2079 6f75 2063 616e  e>c) Or, you can
+00095c60: 206c 6f61 6420 7468 6520 6b2d 666f 6c64   load the k-fold
+00095c70: 2073 706c 6974 2064 6174 6173 6574 7320   split datasets 
+00095c80: 6176 6169 6c61 626c 6520 2864 6561 6675  available (deafu
+00095c90: 6c74 206b 3d35 293a 3c2f 636f 6465 3e3c  lt k=5):</code><
+00095ca0: 2f70 7265 3e0a 0a3c 2f64 6976 3e0a 3c2f  /pre>..</div>.</
+00095cb0: 6469 763e 0a3c 2f64 6976 3e0a 3c2f 6469  div>.</div>.</di
+00095cc0: 763e 3c64 6976 2063 6c61 7373 3d22 6a70  v><div class="jp
+00095cd0: 2d43 656c 6c20 6a70 2d43 6f64 6543 656c  -Cell jp-CodeCel
+00095ce0: 6c20 6a70 2d4e 6f74 6562 6f6f 6b2d 6365  l jp-Notebook-ce
+00095cf0: 6c6c 2020 2022 3e0a 3c64 6976 2063 6c61  ll   ">.<div cla
+00095d00: 7373 3d22 6a70 2d43 656c 6c2d 696e 7075  ss="jp-Cell-inpu
+00095d10: 7457 7261 7070 6572 223e 0a3c 6469 7620  tWrapper">.<div 
+00095d20: 636c 6173 733d 226a 702d 436f 6c6c 6170  class="jp-Collap
+00095d30: 7365 7220 6a70 2d49 6e70 7574 436f 6c6c  ser jp-InputColl
+00095d40: 6170 7365 7220 6a70 2d43 656c 6c2d 696e  apser jp-Cell-in
+00095d50: 7075 7443 6f6c 6c61 7073 6572 223e 0a3c  putCollapser">.<
+00095d60: 2f64 6976 3e0a 3c64 6976 2063 6c61 7373  /div>.<div class
+00095d70: 3d22 6a70 2d49 6e70 7574 4172 6561 206a  ="jp-InputArea j
+00095d80: 702d 4365 6c6c 2d69 6e70 7574 4172 6561  p-Cell-inputArea
+00095d90: 223e 0a3c 6469 7620 636c 6173 733d 226a  ">.<div class="j
+00095da0: 702d 496e 7075 7450 726f 6d70 7420 6a70  p-InputPrompt jp
+00095db0: 2d49 6e70 7574 4172 6561 2d70 726f 6d70  -InputArea-promp
+00095dc0: 7422 3e49 6e26 6e62 7370 3b5b 3136 5d3a  t">In&nbsp;[16]:
+00095dd0: 3c2f 6469 763e 0a3c 6469 7620 636c 6173  </div>.<div clas
+00095de0: 733d 226a 702d 436f 6465 4d69 7272 6f72  s="jp-CodeMirror
+00095df0: 4564 6974 6f72 206a 702d 4564 6974 6f72  Editor jp-Editor
+00095e00: 206a 702d 496e 7075 7441 7265 612d 6564   jp-InputArea-ed
+00095e10: 6974 6f72 2220 6461 7461 2d74 7970 653d  itor" data-type=
+00095e20: 2269 6e6c 696e 6522 3e0a 2020 2020 203c  "inline">.     <
+00095e30: 6469 7620 636c 6173 733d 2243 6f64 654d  div class="CodeM
+00095e40: 6972 726f 7220 636d 2d73 2d6a 7570 7974  irror cm-s-jupyt
+00095e50: 6572 223e 0a3c 6469 7620 636c 6173 733d  er">.<div class=
+00095e60: 2220 6869 6768 6c69 6768 7420 686c 2d69  " highlight hl-i
+00095e70: 7079 7468 6f6e 3322 3e3c 7072 653e 3c73  python3"><pre><s
+00095e80: 7061 6e3e 3c2f 7370 616e 3e3c 7370 616e  pan></span><span
+00095e90: 2063 6c61 7373 3d22 6e22 3e64 665f 7472   class="n">df_tr
+00095ea0: 6169 6e3c 2f73 7061 6e3e 3c73 7061 6e20  ain</span><span 
+00095eb0: 636c 6173 733d 2270 223e 2c3c 2f73 7061  class="p">,</spa
+00095ec0: 6e3e 203c 7370 616e 2063 6c61 7373 3d22  n> <span class="
+00095ed0: 6e22 3e64 665f 7465 7374 3c2f 7370 616e  n">df_test</span
+00095ee0: 3e20 3c73 7061 6e20 636c 6173 733d 226f  > <span class="o
+00095ef0: 223e 3d3c 2f73 7061 6e3e 203c 7370 616e  ">=</span> <span
+00095f00: 2063 6c61 7373 3d22 6e22 3e6c 6f61 645f   class="n">load_
+00095f10: 6473 5f6b 666f 6c64 3c2f 7370 616e 3e3c  ds_kfold</span><
+00095f20: 7370 616e 2063 6c61 7373 3d22 7022 3e28  span class="p">(
+00095f30: 293c 2f73 7061 6e3e 0a0a 3c73 7061 6e20  )</span>..<span 
+00095f40: 636c 6173 733d 226b 223e 666f 723c 2f73  class="k">for</s
+00095f50: 7061 6e3e 203c 7370 616e 2063 6c61 7373  pan> <span class
+00095f60: 3d22 6e22 3e6b 3c2f 7370 616e 3e20 3c73  ="n">k</span> <s
+00095f70: 7061 6e20 636c 6173 733d 226f 7722 3e69  pan class="ow">i
+00095f80: 6e3c 2f73 7061 6e3e 203c 7370 616e 2063  n</span> <span c
+00095f90: 6c61 7373 3d22 6e62 223e 7261 6e67 653c  lass="nb">range<
+00095fa0: 2f73 7061 6e3e 3c73 7061 6e20 636c 6173  /span><span clas
+00095fb0: 733d 2270 223e 283c 2f73 7061 6e3e 3c73  s="p">(</span><s
+00095fc0: 7061 6e20 636c 6173 733d 226e 6222 3e6c  pan class="nb">l
+00095fd0: 656e 3c2f 7370 616e 3e3c 7370 616e 2063  en</span><span c
+00095fe0: 6c61 7373 3d22 7022 3e28 3c2f 7370 616e  lass="p">(</span
+00095ff0: 3e3c 7370 616e 2063 6c61 7373 3d22 6e22  ><span class="n"
+00096000: 3e64 665f 7472 6169 6e3c 2f73 7061 6e3e  >df_train</span>
+00096010: 3c73 7061 6e20 636c 6173 733d 2270 223e  <span class="p">
+00096020: 2929 3a3c 2f73 7061 6e3e 0a20 2020 203c  )):</span>.    <
+00096030: 7370 616e 2063 6c61 7373 3d22 6e62 223e  span class="nb">
+00096040: 7072 696e 743c 2f73 7061 6e3e 3c73 7061  print</span><spa
+00096050: 6e20 636c 6173 733d 2270 223e 283c 2f73  n class="p">(</s
+00096060: 7061 6e3e 3c73 7061 6e20 636c 6173 733d  pan><span class=
+00096070: 2273 3122 3e26 2333 393b 5368 6170 6520  "s1">&#39;Shape 
+00096080: 7472 6169 6e2f 7465 7374 3a26 2333 393b  train/test:&#39;
+00096090: 3c2f 7370 616e 3e3c 7370 616e 2063 6c61  </span><span cla
+000960a0: 7373 3d22 7022 3e2c 3c2f 7370 616e 3e20  ss="p">,</span> 
+000960b0: 3c73 7061 6e20 636c 6173 733d 226e 223e  <span class="n">
+000960c0: 6466 5f74 7261 696e 3c2f 7370 616e 3e3c  df_train</span><
+000960d0: 7370 616e 2063 6c61 7373 3d22 7022 3e5b  span class="p">[
+000960e0: 3c2f 7370 616e 3e3c 7370 616e 2063 6c61  </span><span cla
+000960f0: 7373 3d22 6e22 3e6b 3c2f 7370 616e 3e3c  ss="n">k</span><
+00096100: 7370 616e 2063 6c61 7373 3d22 7022 3e5d  span class="p">]
+00096110: 3c2f 7370 616e 3e3c 7370 616e 2063 6c61  </span><span cla
+00096120: 7373 3d22 6f22 3e2e 3c2f 7370 616e 3e3c  ss="o">.</span><
+00096130: 7370 616e 2063 6c61 7373 3d22 6e22 3e73  span class="n">s
+00096140: 6861 7065 3c2f 7370 616e 3e3c 7370 616e  hape</span><span
+00096150: 2063 6c61 7373 3d22 7022 3e2c 3c2f 7370   class="p">,</sp
+00096160: 616e 3e20 3c73 7061 6e20 636c 6173 733d  an> <span class=
+00096170: 226e 223e 6466 5f74 6573 743c 2f73 7061  "n">df_test</spa
+00096180: 6e3e 3c73 7061 6e20 636c 6173 733d 2270  n><span class="p
+00096190: 223e 5b3c 2f73 7061 6e3e 3c73 7061 6e20  ">[</span><span 
+000961a0: 636c 6173 733d 226e 223e 6b3c 2f73 7061  class="n">k</spa
+000961b0: 6e3e 3c73 7061 6e20 636c 6173 733d 2270  n><span class="p
+000961c0: 223e 5d3c 2f73 7061 6e3e 3c73 7061 6e20  ">]</span><span 
+000961d0: 636c 6173 733d 226f 223e 2e3c 2f73 7061  class="o">.</spa
+000961e0: 6e3e 3c73 7061 6e20 636c 6173 733d 226e  n><span class="n
+000961f0: 223e 7368 6170 653c 2f73 7061 6e3e 3c73  ">shape</span><s
+00096200: 7061 6e20 636c 6173 733d 2270 223e 293c  pan class="p">)<
+00096210: 2f73 7061 6e3e 0a3c 2f70 7265 3e3c 2f64  /span>.</pre></d
+00096220: 6976 3e0a 0a20 2020 2020 3c2f 6469 763e  iv>..     </div>
+00096230: 0a3c 2f64 6976 3e0a 3c2f 6469 763e 0a3c  .</div>.</div>.<
+00096240: 2f64 6976 3e0a 0a3c 6469 7620 636c 6173  /div>..<div clas
+00096250: 733d 226a 702d 4365 6c6c 2d6f 7574 7075  s="jp-Cell-outpu
+00096260: 7457 7261 7070 6572 223e 0a3c 6469 7620  tWrapper">.<div 
+00096270: 636c 6173 733d 226a 702d 436f 6c6c 6170  class="jp-Collap
+00096280: 7365 7220 6a70 2d4f 7574 7075 7443 6f6c  ser jp-OutputCol
+00096290: 6c61 7073 6572 206a 702d 4365 6c6c 2d6f  lapser jp-Cell-o
+000962a0: 7574 7075 7443 6f6c 6c61 7073 6572 223e  utputCollapser">
+000962b0: 0a3c 2f64 6976 3e0a 0a0a 3c64 6976 2063  .</div>...<div c
+000962c0: 6c61 7373 3d22 6a70 2d4f 7574 7075 7441  lass="jp-OutputA
+000962d0: 7265 6120 6a70 2d43 656c 6c2d 6f75 7470  rea jp-Cell-outp
+000962e0: 7574 4172 6561 223e 0a0a 3c64 6976 2063  utArea">..<div c
+000962f0: 6c61 7373 3d22 6a70 2d4f 7574 7075 7441  lass="jp-OutputA
+00096300: 7265 612d 6368 696c 6422 3e0a 0a20 2020  rea-child">..   
+00096310: 200a 2020 2020 3c64 6976 2063 6c61 7373   .    <div class
+00096320: 3d22 6a70 2d4f 7574 7075 7450 726f 6d70  ="jp-OutputPromp
+00096330: 7420 6a70 2d4f 7574 7075 7441 7265 612d  t jp-OutputArea-
+00096340: 7072 6f6d 7074 223e 3c2f 6469 763e 0a0a  prompt"></div>..
+00096350: 0a3c 6469 7620 636c 6173 733d 226a 702d  .<div class="jp-
+00096360: 5265 6e64 6572 6564 5465 7874 206a 702d  RenderedText jp-
+00096370: 4f75 7470 7574 4172 6561 2d6f 7574 7075  OutputArea-outpu
+00096380: 7422 2064 6174 612d 6d69 6d65 2d74 7970  t" data-mime-typ
+00096390: 653d 2274 6578 742f 706c 6169 6e22 3e0a  e="text/plain">.
+000963a0: 3c70 7265 3e4c 6f61 6469 6e67 2064 6174  <pre>Loading dat
+000963b0: 6173 6574 2066 696c 653a 2068 7474 7073  aset file: https
+000963c0: 3a2f 2f67 6974 6875 622e 636f 6d2f 6d61  ://github.com/ma
+000963d0: 742d 616e 616c 7973 6973 2f64 6174 6173  t-analysis/datas
+000963e0: 6574 732f 7261 772f 6d61 696e 2f6d 6174  ets/raw/main/mat
+000963f0: 2f46 6f75 7273 7175 6172 654e 5943 2f0a  /FoursquareNYC/.
+00096400: 3c2f 7072 653e 0a3c 2f64 6976 3e0a 3c2f  </pre>.</div>.</
+00096410: 6469 763e 0a0a 3c64 6976 2063 6c61 7373  div>..<div class
+00096420: 3d22 6a70 2d4f 7574 7075 7441 7265 612d  ="jp-OutputArea-
+00096430: 6368 696c 6422 3e0a 0a20 2020 200a 2020  child">..    .  
+00096440: 2020 3c64 6976 2063 6c61 7373 3d22 6a70    <div class="jp
+00096450: 2d4f 7574 7075 7450 726f 6d70 7420 6a70  -OutputPrompt jp
+00096460: 2d4f 7574 7075 7441 7265 612d 7072 6f6d  -OutputArea-prom
+00096470: 7074 223e 3c2f 6469 763e 0a0a 0a0a 0a3c  pt"></div>.....<
+00096480: 6469 7620 636c 6173 733d 226a 702d 5265  div class="jp-Re
+00096490: 6e64 6572 6564 5465 7874 206a 702d 4f75  nderedText jp-Ou
+000964a0: 7470 7574 4172 6561 2d6f 7574 7075 7420  tputArea-output 
+000964b0: 2220 6461 7461 2d6d 696d 652d 7479 7065  " data-mime-type
+000964c0: 3d22 7465 7874 2f70 6c61 696e 223e 0a3c  ="text/plain">.<
+000964d0: 7072 653e 5370 6c69 7469 6e67 2044 6174  pre>Spliting Dat
+000964e0: 613a 2020 2030 257c 2020 2020 2020 2020  a:   0%|        
+000964f0: 2020 7c20 302f 3139 3320 5b30 303a 3030    | 0/193 [00:00
+00096500: 266c 743b 3f2c 203f 6974 2f73 5d3c 2f70  &lt;?, ?it/s]</p
+00096510: 7265 3e0a 3c2f 6469 763e 0a0a 3c2f 6469  re>.</div>..</di
+00096520: 763e 0a0a 3c64 6976 2063 6c61 7373 3d22  v>..<div class="
+00096530: 6a70 2d4f 7574 7075 7441 7265 612d 6368  jp-OutputArea-ch
+00096540: 696c 6422 3e0a 0a20 2020 200a 2020 2020  ild">..    .    
+00096550: 3c64 6976 2063 6c61 7373 3d22 6a70 2d4f  <div class="jp-O
+00096560: 7574 7075 7450 726f 6d70 7420 6a70 2d4f  utputPrompt jp-O
+00096570: 7574 7075 7441 7265 612d 7072 6f6d 7074  utputArea-prompt
+00096580: 223e 3c2f 6469 763e 0a0a 0a3c 6469 7620  "></div>...<div 
+00096590: 636c 6173 733d 226a 702d 5265 6e64 6572  class="jp-Render
+000965a0: 6564 5465 7874 206a 702d 4f75 7470 7574  edText jp-Output
+000965b0: 4172 6561 2d6f 7574 7075 7422 2064 6174  Area-output" dat
+000965c0: 612d 6d69 6d65 2d74 7970 653d 2274 6578  a-mime-type="tex
+000965d0: 742f 706c 6169 6e22 3e0a 3c70 7265 3e53  t/plain">.<pre>S
+000965e0: 6861 7065 2074 7261 696e 2f74 6573 743a  hape train/test:
+000965f0: 2028 3531 3133 302c 2031 3129 2028 3135   (51130, 11) (15
+00096600: 3833 322c 2031 3129 0a53 6861 7065 2074  832, 11).Shape t
+00096610: 7261 696e 2f74 6573 743a 2028 3532 3637  rain/test: (5267
+00096620: 382c 2031 3129 2028 3134 3238 342c 2031  8, 11) (14284, 1
+00096630: 3129 0a53 6861 7065 2074 7261 696e 2f74  1).Shape train/t
+00096640: 6573 743a 2028 3533 3933 382c 2031 3129  est: (53938, 11)
+00096650: 2028 3133 3032 342c 2031 3129 0a53 6861   (13024, 11).Sha
+00096660: 7065 2074 7261 696e 2f74 6573 743a 2028  pe train/test: (
+00096670: 3534 3835 362c 2031 3129 2028 3132 3130  54856, 11) (1210
+00096680: 362c 2031 3129 0a53 6861 7065 2074 7261  6, 11).Shape tra
+00096690: 696e 2f74 6573 743a 2028 3535 3234 362c  in/test: (55246,
+000966a0: 2031 3129 2028 3131 3731 362c 2031 3129   11) (11716, 11)
+000966b0: 0a3c 2f70 7265 3e0a 3c2f 6469 763e 0a3c  .</pre>.</div>.<
+000966c0: 2f64 6976 3e0a 0a3c 2f64 6976 3e0a 0a3c  /div>..</div>..<
+000966d0: 2f64 6976 3e0a 0a3c 2f64 6976 3e0a 3c64  /div>..</div>.<d
+000966e0: 6976 2063 6c61 7373 3d22 6a70 2d43 656c  iv class="jp-Cel
+000966f0: 6c20 6a70 2d4d 6172 6b64 6f77 6e43 656c  l jp-MarkdownCel
+00096700: 6c20 6a70 2d4e 6f74 6562 6f6f 6b2d 6365  l jp-Notebook-ce
+00096710: 6c6c 223e 0a3c 6469 7620 636c 6173 733d  ll">.<div class=
+00096720: 226a 702d 4365 6c6c 2d69 6e70 7574 5772  "jp-Cell-inputWr
+00096730: 6170 7065 7222 3e0a 3c64 6976 2063 6c61  apper">.<div cla
+00096740: 7373 3d22 6a70 2d43 6f6c 6c61 7073 6572  ss="jp-Collapser
+00096750: 206a 702d 496e 7075 7443 6f6c 6c61 7073   jp-InputCollaps
+00096760: 6572 206a 702d 4365 6c6c 2d69 6e70 7574  er jp-Cell-input
+00096770: 436f 6c6c 6170 7365 7222 3e0a 3c2f 6469  Collapser">.</di
+00096780: 763e 0a3c 6469 7620 636c 6173 733d 226a  v>.<div class="j
+00096790: 702d 496e 7075 7441 7265 6120 6a70 2d43  p-InputArea jp-C
+000967a0: 656c 6c2d 696e 7075 7441 7265 6122 3e3c  ell-inputArea"><
+000967b0: 6469 7620 636c 6173 733d 226a 702d 496e  div class="jp-In
+000967c0: 7075 7450 726f 6d70 7420 6a70 2d49 6e70  putPrompt jp-Inp
+000967d0: 7574 4172 6561 2d70 726f 6d70 7422 3e0a  utArea-prompt">.
+000967e0: 3c2f 6469 763e 3c64 6976 2063 6c61 7373  </div><div class
+000967f0: 3d22 6a70 2d52 656e 6465 7265 6448 544d  ="jp-RenderedHTM
+00096800: 4c43 6f6d 6d6f 6e20 6a70 2d52 656e 6465  LCommon jp-Rende
+00096810: 7265 644d 6172 6b64 6f77 6e20 6a70 2d4d  redMarkdown jp-M
+00096820: 6172 6b64 6f77 6e4f 7574 7075 7420 2220  arkdownOutput " 
+00096830: 6461 7461 2d6d 696d 652d 7479 7065 3d22  data-mime-type="
+00096840: 7465 7874 2f6d 6172 6b64 6f77 6e22 3e0a  text/markdown">.
+00096850: 0a3c 7072 653e 3c63 6f64 653e 6429 2059  .<pre><code>d) Y
+00096860: 6f75 2063 616e 206c 6f61 6420 6120 6469  ou can load a di
+00096870: 6666 6572 656e 7420 6461 7461 7365 7420  fferent dataset 
+00096880: 6672 6f6d 2072 6570 6f73 6974 6f72 793a  from repository:
+00096890: 3c2f 636f 6465 3e3c 2f70 7265 3e0a 0a3c  </code></pre>..<
+000968a0: 2f64 6976 3e0a 3c2f 6469 763e 0a3c 2f64  /div>.</div>.</d
+000968b0: 6976 3e0a 3c2f 6469 763e 3c64 6976 2063  iv>.</div><div c
+000968c0: 6c61 7373 3d22 6a70 2d43 656c 6c20 6a70  lass="jp-Cell jp
+000968d0: 2d43 6f64 6543 656c 6c20 6a70 2d4e 6f74  -CodeCell jp-Not
+000968e0: 6562 6f6f 6b2d 6365 6c6c 2020 2022 3e0a  ebook-cell   ">.
+000968f0: 3c64 6976 2063 6c61 7373 3d22 6a70 2d43  <div class="jp-C
+00096900: 656c 6c2d 696e 7075 7457 7261 7070 6572  ell-inputWrapper
+00096910: 223e 0a3c 6469 7620 636c 6173 733d 226a  ">.<div class="j
+00096920: 702d 436f 6c6c 6170 7365 7220 6a70 2d49  p-Collapser jp-I
+00096930: 6e70 7574 436f 6c6c 6170 7365 7220 6a70  nputCollapser jp
+00096940: 2d43 656c 6c2d 696e 7075 7443 6f6c 6c61  -Cell-inputColla
+00096950: 7073 6572 223e 0a3c 2f64 6976 3e0a 3c64  pser">.</div>.<d
+00096960: 6976 2063 6c61 7373 3d22 6a70 2d49 6e70  iv class="jp-Inp
+00096970: 7574 4172 6561 206a 702d 4365 6c6c 2d69  utArea jp-Cell-i
+00096980: 6e70 7574 4172 6561 223e 0a3c 6469 7620  nputArea">.<div 
+00096990: 636c 6173 733d 226a 702d 496e 7075 7450  class="jp-InputP
+000969a0: 726f 6d70 7420 6a70 2d49 6e70 7574 4172  rompt jp-InputAr
+000969b0: 6561 2d70 726f 6d70 7422 3e49 6e26 6e62  ea-prompt">In&nb
+000969c0: 7370 3b5b 3137 5d3a 3c2f 6469 763e 0a3c  sp;[17]:</div>.<
+000969d0: 6469 7620 636c 6173 733d 226a 702d 436f  div class="jp-Co
+000969e0: 6465 4d69 7272 6f72 4564 6974 6f72 206a  deMirrorEditor j
+000969f0: 702d 4564 6974 6f72 206a 702d 496e 7075  p-Editor jp-Inpu
+00096a00: 7441 7265 612d 6564 6974 6f72 2220 6461  tArea-editor" da
+00096a10: 7461 2d74 7970 653d 2269 6e6c 696e 6522  ta-type="inline"
+00096a20: 3e0a 2020 2020 203c 6469 7620 636c 6173  >.     <div clas
+00096a30: 733d 2243 6f64 654d 6972 726f 7220 636d  s="CodeMirror cm
+00096a40: 2d73 2d6a 7570 7974 6572 223e 0a3c 6469  -s-jupyter">.<di
+00096a50: 7620 636c 6173 733d 2220 6869 6768 6c69  v class=" highli
+00096a60: 6768 7420 686c 2d69 7079 7468 6f6e 3322  ght hl-ipython3"
+00096a70: 3e3c 7072 653e 3c73 7061 6e3e 3c2f 7370  ><pre><span></sp
+00096a80: 616e 3e3c 7370 616e 2063 6c61 7373 3d22  an><span class="
+00096a90: 6331 223e 2320 5573 6520 7468 6520 666f  c1"># Use the fo
+00096aa0: 726d 6174 3a20 2623 3339 3b63 6174 6567  rmat: &#39;categ
+00096ab0: 6f72 792e 4461 7461 7365 744e 616d 6526  ory.DatasetName&
+00096ac0: 2333 393b 3c2f 7370 616e 3e0a 3c73 7061  #39;</span>.<spa
+00096ad0: 6e20 636c 6173 733d 226e 223e 6461 7461  n class="n">data
+00096ae0: 7365 743c 2f73 7061 6e3e 3c73 7061 6e20  set</span><span 
+00096af0: 636c 6173 733d 226f 223e 3d3c 2f73 7061  class="o">=</spa
+00096b00: 6e3e 3c73 7061 6e20 636c 6173 733d 2273  n><span class="s
+00096b10: 3122 3e26 2333 393b 7261 772e 416e 696d  1">&#39;raw.Anim
+00096b20: 616c 7326 2333 393b 3c2f 7370 616e 3e0a  als&#39;</span>.
+00096b30: 0a3c 7370 616e 2063 6c61 7373 3d22 6e22  .<span class="n"
+00096b40: 3e64 663c 2f73 7061 6e3e 203c 7370 616e  >df</span> <span
+00096b50: 2063 6c61 7373 3d22 6f22 3e3d 3c2f 7370   class="o">=</sp
+00096b60: 616e 3e20 3c73 7061 6e20 636c 6173 733d  an> <span class=
+00096b70: 226e 223e 6c6f 6164 5f64 733c 2f73 7061  "n">load_ds</spa
+00096b80: 6e3e 3c73 7061 6e20 636c 6173 733d 2270  n><span class="p
+00096b90: 223e 283c 2f73 7061 6e3e 3c73 7061 6e20  ">(</span><span 
+00096ba0: 636c 6173 733d 226e 223e 6461 7461 7365  class="n">datase
+00096bb0: 743c 2f73 7061 6e3e 3c73 7061 6e20 636c  t</span><span cl
+00096bc0: 6173 733d 2270 223e 293c 2f73 7061 6e3e  ass="p">)</span>
+00096bd0: 0a3c 7370 616e 2063 6c61 7373 3d22 6e22  .<span class="n"
+00096be0: 3e64 663c 2f73 7061 6e3e 0a3c 2f70 7265  >df</span>.</pre
+00096bf0: 3e3c 2f64 6976 3e0a 0a20 2020 2020 3c2f  ></div>..     </
+00096c00: 6469 763e 0a3c 2f64 6976 3e0a 3c2f 6469  div>.</div>.</di
+00096c10: 763e 0a3c 2f64 6976 3e0a 0a3c 6469 7620  v>.</div>..<div 
+00096c20: 636c 6173 733d 226a 702d 4365 6c6c 2d6f  class="jp-Cell-o
+00096c30: 7574 7075 7457 7261 7070 6572 223e 0a3c  utputWrapper">.<
+00096c40: 6469 7620 636c 6173 733d 226a 702d 436f  div class="jp-Co
+00096c50: 6c6c 6170 7365 7220 6a70 2d4f 7574 7075  llapser jp-Outpu
+00096c60: 7443 6f6c 6c61 7073 6572 206a 702d 4365  tCollapser jp-Ce
+00096c70: 6c6c 2d6f 7574 7075 7443 6f6c 6c61 7073  ll-outputCollaps
+00096c80: 6572 223e 0a3c 2f64 6976 3e0a 0a0a 3c64  er">.</div>...<d
+00096c90: 6976 2063 6c61 7373 3d22 6a70 2d4f 7574  iv class="jp-Out
+00096ca0: 7075 7441 7265 6120 6a70 2d43 656c 6c2d  putArea jp-Cell-
+00096cb0: 6f75 7470 7574 4172 6561 223e 0a0a 3c64  outputArea">..<d
+00096cc0: 6976 2063 6c61 7373 3d22 6a70 2d4f 7574  iv class="jp-Out
+00096cd0: 7075 7441 7265 612d 6368 696c 6422 3e0a  putArea-child">.
+00096ce0: 0a20 2020 200a 2020 2020 3c64 6976 2063  .    .    <div c
+00096cf0: 6c61 7373 3d22 6a70 2d4f 7574 7075 7450  lass="jp-OutputP
+00096d00: 726f 6d70 7420 6a70 2d4f 7574 7075 7441  rompt jp-OutputA
+00096d10: 7265 612d 7072 6f6d 7074 223e 3c2f 6469  rea-prompt"></di
+00096d20: 763e 0a0a 0a3c 6469 7620 636c 6173 733d  v>...<div class=
+00096d30: 226a 702d 5265 6e64 6572 6564 5465 7874  "jp-RenderedText
+00096d40: 206a 702d 4f75 7470 7574 4172 6561 2d6f   jp-OutputArea-o
+00096d50: 7574 7075 7422 2064 6174 612d 6d69 6d65  utput" data-mime
+00096d60: 2d74 7970 653d 2274 6578 742f 706c 6169  -type="text/plai
+00096d70: 6e22 3e0a 3c70 7265 3e4c 6f61 6469 6e67  n">.<pre>Loading
+00096d80: 2064 6174 6173 6574 2066 696c 653a 2068   dataset file: h
+00096d90: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+00096da0: 6d2f 6d61 742d 616e 616c 7973 6973 2f64  m/mat-analysis/d
+00096db0: 6174 6173 6574 732f 7261 772f 6d61 696e  atasets/raw/main
+00096dc0: 2f72 6177 2f41 6e69 6d61 6c73 2f0a 3c2f  /raw/Animals/.</
+00096dd0: 7072 653e 0a3c 2f64 6976 3e0a 3c2f 6469  pre>.</div>.</di
+00096de0: 763e 0a0a 3c64 6976 2063 6c61 7373 3d22  v>..<div class="
+00096df0: 6a70 2d4f 7574 7075 7441 7265 612d 6368  jp-OutputArea-ch
+00096e00: 696c 6422 3e0a 0a20 2020 200a 2020 2020  ild">..    .    
+00096e10: 3c64 6976 2063 6c61 7373 3d22 6a70 2d4f  <div class="jp-O
+00096e20: 7574 7075 7450 726f 6d70 7420 6a70 2d4f  utputPrompt jp-O
+00096e30: 7574 7075 7441 7265 612d 7072 6f6d 7074  utputArea-prompt
+00096e40: 223e 4f75 745b 3137 5d3a 3c2f 6469 763e  ">Out[17]:</div>
+00096e50: 0a0a 0a0a 3c64 6976 2063 6c61 7373 3d22  ....<div class="
+00096e60: 6a70 2d52 656e 6465 7265 6448 544d 4c43  jp-RenderedHTMLC
+00096e70: 6f6d 6d6f 6e20 6a70 2d52 656e 6465 7265  ommon jp-Rendere
+00096e80: 6448 544d 4c20 6a70 2d4f 7574 7075 7441  dHTML jp-OutputA
+00096e90: 7265 612d 6f75 7470 7574 206a 702d 4f75  rea-output jp-Ou
+00096ea0: 7470 7574 4172 6561 2d65 7865 6375 7465  tputArea-execute
+00096eb0: 5265 7375 6c74 2220 6461 7461 2d6d 696d  Result" data-mim
+00096ec0: 652d 7479 7065 3d22 7465 7874 2f68 746d  e-type="text/htm
+00096ed0: 6c22 3e0a 3c64 6976 3e0a 3c73 7479 6c65  l">.<div>.<style
+00096ee0: 2073 636f 7065 643e 0a20 2020 202e 6461   scoped>.    .da
+00096ef0: 7461 6672 616d 6520 7462 6f64 7920 7472  taframe tbody tr
+00096f00: 2074 683a 6f6e 6c79 2d6f 662d 7479 7065   th:only-of-type
+00096f10: 207b 0a20 2020 2020 2020 2076 6572 7469   {.        verti
+00096f20: 6361 6c2d 616c 6967 6e3a 206d 6964 646c  cal-align: middl
+00096f30: 653b 0a20 2020 207d 0a0a 2020 2020 2e64  e;.    }..    .d
+00096f40: 6174 6166 7261 6d65 2074 626f 6479 2074  ataframe tbody t
+00096f50: 7220 7468 207b 0a20 2020 2020 2020 2076  r th {.        v
+00096f60: 6572 7469 6361 6c2d 616c 6967 6e3a 2074  ertical-align: t
+00096f70: 6f70 3b0a 2020 2020 7d0a 0a20 2020 202e  op;.    }..    .
+00096f80: 6461 7461 6672 616d 6520 7468 6561 6420  dataframe thead 
+00096f90: 7468 207b 0a20 2020 2020 2020 2074 6578  th {.        tex
+00096fa0: 742d 616c 6967 6e3a 2072 6967 6874 3b0a  t-align: right;.
+00096fb0: 2020 2020 7d0a 3c2f 7374 796c 653e 0a3c      }.</style>.<
+00096fc0: 7461 626c 6520 626f 7264 6572 3d22 3122  table border="1"
+00096fd0: 2063 6c61 7373 3d22 6461 7461 6672 616d   class="datafram
+00096fe0: 6522 3e0a 2020 3c74 6865 6164 3e0a 2020  e">.  <thead>.  
+00096ff0: 2020 3c74 7220 7374 796c 653d 2274 6578    <tr style="tex
+00097000: 742d 616c 6967 6e3a 2072 6967 6874 3b22  t-align: right;"
+00097010: 3e0a 2020 2020 2020 3c74 683e 3c2f 7468  >.      <th></th
+00097020: 3e0a 2020 2020 2020 3c74 683e 7469 6d65  >.      <th>time
+00097030: 3c2f 7468 3e0a 2020 2020 2020 3c74 683e  </th>.      <th>
+00097040: 6c61 743c 2f74 683e 0a20 2020 2020 203c  lat</th>.      <
+00097050: 7468 3e6c 6f6e 3c2f 7468 3e0a 2020 2020  th>lon</th>.    
+00097060: 2020 3c74 683e 7469 643c 2f74 683e 0a20    <th>tid</th>. 
+00097070: 2020 2020 203c 7468 3e6c 6162 656c 3c2f       <th>label</
+00097080: 7468 3e0a 2020 2020 3c2f 7472 3e0a 2020  th>.    </tr>.  
+00097090: 3c2f 7468 6561 643e 0a20 203c 7462 6f64  </thead>.  <tbod
+000970a0: 793e 0a20 2020 203c 7472 3e0a 2020 2020  y>.    <tr>.    
+000970b0: 2020 3c74 683e 303c 2f74 683e 0a20 2020    <th>0</th>.   
+000970c0: 2020 203c 7464 3e30 2e30 303c 2f74 643e     <td>0.00</td>
+000970d0: 0a20 2020 2020 203c 7464 3e35 302e 3130  .      <td>50.10
+000970e0: 3636 3c2f 7464 3e0a 2020 2020 2020 3c74  66</td>.      <t
+000970f0: 643e 332e 3739 3636 353c 2f74 643e 0a20  d>3.79665</td>. 
+00097100: 2020 2020 203c 7464 3e31 3c2f 7464 3e0a       <td>1</td>.
+00097110: 2020 2020 2020 3c74 643e 443c 2f74 643e        <td>D</td>
+00097120: 0a20 2020 203c 2f74 723e 0a20 2020 203c  .    </tr>.    <
+00097130: 7472 3e0a 2020 2020 2020 3c74 683e 313c  tr>.      <th>1<
+00097140: 2f74 683e 0a20 2020 2020 203c 7464 3e34  /th>.      <td>4
+00097150: 2e33 393c 2f74 643e 0a20 2020 2020 203c  .39</td>.      <
+00097160: 7464 3e35 302e 3130 3435 3c2f 7464 3e0a  td>50.1045</td>.
+00097170: 2020 2020 2020 3c74 643e 332e 3739 3435        <td>3.7945
+00097180: 353c 2f74 643e 0a20 2020 2020 203c 7464  5</td>.      <td
+00097190: 3e31 3c2f 7464 3e0a 2020 2020 2020 3c74  >1</td>.      <t
+000971a0: 643e 443c 2f74 643e 0a20 2020 203c 2f74  d>D</td>.    </t
+000971b0: 723e 0a20 2020 203c 7472 3e0a 2020 2020  r>.    <tr>.    
+000971c0: 2020 3c74 683e 323c 2f74 683e 0a20 2020    <th>2</th>.   
+000971d0: 2020 203c 7464 3e37 2e39 303c 2f74 643e     <td>7.90</td>
+000971e0: 0a20 2020 2020 203c 7464 3e35 302e 3131  .      <td>50.11
+000971f0: 3131 3c2f 7464 3e0a 2020 2020 2020 3c74  11</td>.      <t
+00097200: 643e 332e 3739 3834 353c 2f74 643e 0a20  d>3.79845</td>. 
+00097210: 2020 2020 203c 7464 3e31 3c2f 7464 3e0a       <td>1</td>.
+00097220: 2020 2020 2020 3c74 643e 443c 2f74 643e        <td>D</td>
+00097230: 0a20 2020 203c 2f74 723e 0a20 2020 203c  .    </tr>.    <
+00097240: 7472 3e0a 2020 2020 2020 3c74 683e 333c  tr>.      <th>3<
+00097250: 2f74 683e 0a20 2020 2020 203c 7464 3e39  /th>.      <td>9
+00097260: 2e36 323c 2f74 643e 0a20 2020 2020 203c  .62</td>.      <
+00097270: 7464 3e35 302e 3130 3732 3c2f 7464 3e0a  td>50.1072</td>.
+00097280: 2020 2020 2020 3c74 643e 332e 3739 3834        <td>3.7984
+00097290: 353c 2f74 643e 0a20 2020 2020 203c 7464  5</td>.      <td
+000972a0: 3e31 3c2f 7464 3e0a 2020 2020 2020 3c74  >1</td>.      <t
+000972b0: 643e 443c 2f74 643e 0a20 2020 203c 2f74  d>D</td>.    </t
+000972c0: 723e 0a20 2020 203c 7472 3e0a 2020 2020  r>.    <tr>.    
+000972d0: 2020 3c74 683e 343c 2f74 683e 0a20 2020    <th>4</th>.   
+000972e0: 2020 203c 7464 3e31 352e 3039 3c2f 7464     <td>15.09</td
+000972f0: 3e0a 2020 2020 2020 3c74 643e 3530 2e31  >.      <td>50.1
+00097300: 3133 323c 2f74 643e 0a20 2020 2020 203c  132</td>.      <
+00097310: 7464 3e33 2e37 3939 3635 3c2f 7464 3e0a  td>3.79965</td>.
+00097320: 2020 2020 2020 3c74 643e 313c 2f74 643e        <td>1</td>
+00097330: 0a20 2020 2020 203c 7464 3e44 3c2f 7464  .      <td>D</td
+00097340: 3e0a 2020 2020 3c2f 7472 3e0a 2020 2020  >.    </tr>.    
+00097350: 3c74 723e 0a20 2020 2020 203c 7468 3e2e  <tr>.      <th>.
+00097360: 2e2e 3c2f 7468 3e0a 2020 2020 2020 3c74  ..</th>.      <t
+00097370: 643e 2e2e 2e3c 2f74 643e 0a20 2020 2020  d>...</td>.     
+00097380: 203c 7464 3e2e 2e2e 3c2f 7464 3e0a 2020   <td>...</td>.  
+00097390: 2020 2020 3c74 643e 2e2e 2e3c 2f74 643e      <td>...</td>
+000973a0: 0a20 2020 2020 203c 7464 3e2e 2e2e 3c2f  .      <td>...</
+000973b0: 7464 3e0a 2020 2020 2020 3c74 643e 2e2e  td>.      <td>..
+000973c0: 2e3c 2f74 643e 0a20 2020 203c 2f74 723e  .</td>.    </tr>
+000973d0: 0a20 2020 203c 7472 3e0a 2020 2020 2020  .    <tr>.      
+000973e0: 3c74 683e 3435 3137 3c2f 7468 3e0a 2020  <th>4517</th>.  
+000973f0: 2020 2020 3c74 643e 3235 382e 3838 3c2f      <td>258.88</
+00097400: 7464 3e0a 2020 2020 2020 3c74 643e 3530  td>.      <td>50
+00097410: 2e31 3639 363c 2f74 643e 0a20 2020 2020  .1696</td>.     
+00097420: 203c 7464 3e33 2e37 3632 3135 3c2f 7464   <td>3.76215</td
+00097430: 3e0a 2020 2020 2020 3c74 643e 3937 3c2f  >.      <td>97</
+00097440: 7464 3e0a 2020 2020 2020 3c74 643e 433c  td>.      <td>C<
+00097450: 2f74 643e 0a20 2020 203c 2f74 723e 0a20  /td>.    </tr>. 
+00097460: 2020 203c 7472 3e0a 2020 2020 2020 3c74     <tr>.      <t
+00097470: 683e 3435 3138 3c2f 7468 3e0a 2020 2020  h>4518</th>.    
+00097480: 2020 3c74 643e 3236 302e 3835 3c2f 7464    <td>260.85</td
+00097490: 3e0a 2020 2020 2020 3c74 643e 3530 2e31  >.      <td>50.1
+000974a0: 3639 333c 2f74 643e 0a20 2020 2020 203c  693</td>.      <
+000974b0: 7464 3e33 2e37 3631 3835 3c2f 7464 3e0a  td>3.76185</td>.
+000974c0: 2020 2020 2020 3c74 643e 3937 3c2f 7464        <td>97</td
+000974d0: 3e0a 2020 2020 2020 3c74 643e 433c 2f74  >.      <td>C</t
+000974e0: 643e 0a20 2020 203c 2f74 723e 0a20 2020  d>.    </tr>.   
+000974f0: 203c 7472 3e0a 2020 2020 2020 3c74 683e   <tr>.      <th>
+00097500: 3435 3139 3c2f 7468 3e0a 2020 2020 2020  4519</th>.      
+00097510: 3c74 643e 3236 322e 3830 3c2f 7464 3e0a  <td>262.80</td>.
+00097520: 2020 2020 2020 3c74 643e 3530 2e31 3639        <td>50.169
+00097530: 333c 2f74 643e 0a20 2020 2020 203c 7464  3</td>.      <td
+00097540: 3e33 2e37 3632 3435 3c2f 7464 3e0a 2020  >3.76245</td>.  
+00097550: 2020 2020 3c74 643e 3937 3c2f 7464 3e0a      <td>97</td>.
+00097560: 2020 2020 2020 3c74 643e 433c 2f74 643e        <td>C</td>
+00097570: 0a20 2020 203c 2f74 723e 0a20 2020 203c  .    </tr>.    <
+00097580: 7472 3e0a 2020 2020 2020 3c74 683e 3435  tr>.      <th>45
+00097590: 3230 3c2f 7468 3e0a 2020 2020 2020 3c74  20</th>.      <t
+000975a0: 643e 3236 342e 3639 3c2f 7464 3e0a 2020  d>264.69</td>.  
+000975b0: 2020 2020 3c74 643e 3530 2e31 3638 373c      <td>50.1687<
+000975c0: 2f74 643e 0a20 2020 2020 203c 7464 3e33  /td>.      <td>3
+000975d0: 2e37 3634 3535 3c2f 7464 3e0a 2020 2020  .76455</td>.    
+000975e0: 2020 3c74 643e 3937 3c2f 7464 3e0a 2020    <td>97</td>.  
+000975f0: 2020 2020 3c74 643e 433c 2f74 643e 0a20      <td>C</td>. 
+00097600: 2020 203c 2f74 723e 0a20 2020 203c 7472     </tr>.    <tr
+00097610: 3e0a 2020 2020 2020 3c74 683e 3435 3231  >.      <th>4521
+00097620: 3c2f 7468 3e0a 2020 2020 2020 3c74 643e  </th>.      <td>
+00097630: 3236 362e 3930 3c2f 7464 3e0a 2020 2020  266.90</td>.    
+00097640: 2020 3c74 643e 3530 2e31 3638 373c 2f74    <td>50.1687</t
+00097650: 643e 0a20 2020 2020 203c 7464 3e33 2e37  d>.      <td>3.7
+00097660: 3634 3535 3c2f 7464 3e0a 2020 2020 2020  6455</td>.      
+00097670: 3c74 643e 3937 3c2f 7464 3e0a 2020 2020  <td>97</td>.    
+00097680: 2020 3c74 643e 433c 2f74 643e 0a20 2020    <td>C</td>.   
+00097690: 203c 2f74 723e 0a20 203c 2f74 626f 6479   </tr>.  </tbody
+000976a0: 3e0a 3c2f 7461 626c 653e 0a3c 703e 3134  >.</table>.<p>14
+000976b0: 3939 3020 726f 7773 20c3 9720 3520 636f  990 rows .. 5 co
+000976c0: 6c75 6d6e 733c 2f70 3e0a 3c2f 6469 763e  lumns</p>.</div>
+000976d0: 0a3c 2f64 6976 3e0a 0a3c 2f64 6976 3e0a  .</div>..</div>.
+000976e0: 0a3c 2f64 6976 3e0a 0a3c 2f64 6976 3e0a  .</div>..</div>.
+000976f0: 0a3c 2f64 6976 3e0a 3c64 6976 2063 6c61  .</div>.<div cla
+00097700: 7373 3d22 6a70 2d43 656c 6c20 6a70 2d4d  ss="jp-Cell jp-M
+00097710: 6172 6b64 6f77 6e43 656c 6c20 6a70 2d4e  arkdownCell jp-N
+00097720: 6f74 6562 6f6f 6b2d 6365 6c6c 223e 0a3c  otebook-cell">.<
+00097730: 6469 7620 636c 6173 733d 226a 702d 4365  div class="jp-Ce
+00097740: 6c6c 2d69 6e70 7574 5772 6170 7065 7222  ll-inputWrapper"
+00097750: 3e0a 3c64 6976 2063 6c61 7373 3d22 6a70  >.<div class="jp
+00097760: 2d43 6f6c 6c61 7073 6572 206a 702d 496e  -Collapser jp-In
+00097770: 7075 7443 6f6c 6c61 7073 6572 206a 702d  putCollapser jp-
+00097780: 4365 6c6c 2d69 6e70 7574 436f 6c6c 6170  Cell-inputCollap
+00097790: 7365 7222 3e0a 3c2f 6469 763e 0a3c 6469  ser">.</div>.<di
+000977a0: 7620 636c 6173 733d 226a 702d 496e 7075  v class="jp-Inpu
+000977b0: 7441 7265 6120 6a70 2d43 656c 6c2d 696e  tArea jp-Cell-in
+000977c0: 7075 7441 7265 6122 3e3c 6469 7620 636c  putArea"><div cl
+000977d0: 6173 733d 226a 702d 496e 7075 7450 726f  ass="jp-InputPro
+000977e0: 6d70 7420 6a70 2d49 6e70 7574 4172 6561  mpt jp-InputArea
+000977f0: 2d70 726f 6d70 7422 3e0a 3c2f 6469 763e  -prompt">.</div>
+00097800: 3c64 6976 2063 6c61 7373 3d22 6a70 2d52  <div class="jp-R
+00097810: 656e 6465 7265 6448 544d 4c43 6f6d 6d6f  enderedHTMLCommo
+00097820: 6e20 6a70 2d52 656e 6465 7265 644d 6172  n jp-RenderedMar
+00097830: 6b64 6f77 6e20 6a70 2d4d 6172 6b64 6f77  kdown jp-Markdow
+00097840: 6e4f 7574 7075 7420 2220 6461 7461 2d6d  nOutput " data-m
+00097850: 696d 652d 7479 7065 3d22 7465 7874 2f6d  ime-type="text/m
+00097860: 6172 6b64 6f77 6e22 3e0a 0a3c 7072 653e  arkdown">..<pre>
+00097870: 3c63 6f64 653e 6529 2054 6f20 6765 7420  <code>e) To get 
+00097880: 6120 6675 6c6c 206c 6973 7420 6f66 2061  a full list of a
+00097890: 6e61 696c 6162 6c65 2072 6570 6f73 6974  nailable reposit
+000978a0: 6f72 6965 7320 616e 6420 6361 7465 676f  ories and catego
+000978b0: 7269 6573 3a3c 2f63 6f64 653e 3c2f 7072  ries:</code></pr
+000978c0: 653e 0a0a 3c2f 6469 763e 0a3c 2f64 6976  e>..</div>.</div
+000978d0: 3e0a 3c2f 6469 763e 0a3c 2f64 6976 3e3c  >.</div>.</div><
+000978e0: 6469 7620 636c 6173 733d 226a 702d 4365  div class="jp-Ce
+000978f0: 6c6c 206a 702d 436f 6465 4365 6c6c 206a  ll jp-CodeCell j
+00097900: 702d 4e6f 7465 626f 6f6b 2d63 656c 6c20  p-Notebook-cell 
+00097910: 2020 223e 0a3c 6469 7620 636c 6173 733d    ">.<div class=
+00097920: 226a 702d 4365 6c6c 2d69 6e70 7574 5772  "jp-Cell-inputWr
+00097930: 6170 7065 7222 3e0a 3c64 6976 2063 6c61  apper">.<div cla
+00097940: 7373 3d22 6a70 2d43 6f6c 6c61 7073 6572  ss="jp-Collapser
+00097950: 206a 702d 496e 7075 7443 6f6c 6c61 7073   jp-InputCollaps
+00097960: 6572 206a 702d 4365 6c6c 2d69 6e70 7574  er jp-Cell-input
+00097970: 436f 6c6c 6170 7365 7222 3e0a 3c2f 6469  Collapser">.</di
+00097980: 763e 0a3c 6469 7620 636c 6173 733d 226a  v>.<div class="j
+00097990: 702d 496e 7075 7441 7265 6120 6a70 2d43  p-InputArea jp-C
+000979a0: 656c 6c2d 696e 7075 7441 7265 6122 3e0a  ell-inputArea">.
+000979b0: 3c64 6976 2063 6c61 7373 3d22 6a70 2d49  <div class="jp-I
+000979c0: 6e70 7574 5072 6f6d 7074 206a 702d 496e  nputPrompt jp-In
+000979d0: 7075 7441 7265 612d 7072 6f6d 7074 223e  putArea-prompt">
+000979e0: 496e 266e 6273 703b 5b31 385d 3a3c 2f64  In&nbsp;[18]:</d
+000979f0: 6976 3e0a 3c64 6976 2063 6c61 7373 3d22  iv>.<div class="
+00097a00: 6a70 2d43 6f64 654d 6972 726f 7245 6469  jp-CodeMirrorEdi
+00097a10: 746f 7220 6a70 2d45 6469 746f 7220 6a70  tor jp-Editor jp
+00097a20: 2d49 6e70 7574 4172 6561 2d65 6469 746f  -InputArea-edito
+00097a30: 7222 2064 6174 612d 7479 7065 3d22 696e  r" data-type="in
+00097a40: 6c69 6e65 223e 0a20 2020 2020 3c64 6976  line">.     <div
+00097a50: 2063 6c61 7373 3d22 436f 6465 4d69 7272   class="CodeMirr
+00097a60: 6f72 2063 6d2d 732d 6a75 7079 7465 7222  or cm-s-jupyter"
+00097a70: 3e0a 3c64 6976 2063 6c61 7373 3d22 2068  >.<div class=" h
+00097a80: 6967 686c 6967 6874 2068 6c2d 6970 7974  ighlight hl-ipyt
+00097a90: 686f 6e33 223e 3c70 7265 3e3c 7370 616e  hon3"><pre><span
+00097aa0: 3e3c 2f73 7061 6e3e 3c73 7061 6e20 636c  ></span><span cl
+00097ab0: 6173 733d 226e 223e 7264 3c2f 7370 616e  ass="n">rd</span
+00097ac0: 3e20 3c73 7061 6e20 636c 6173 733d 226f  > <span class="o
+00097ad0: 223e 3d3c 2f73 7061 6e3e 203c 7370 616e  ">=</span> <span
+00097ae0: 2063 6c61 7373 3d22 6e22 3e72 6570 6f73   class="n">repos
+00097af0: 6974 6f72 795f 6461 7461 7365 7473 3c2f  itory_datasets</
+00097b00: 7370 616e 3e3c 7370 616e 2063 6c61 7373  span><span class
+00097b10: 3d22 7022 3e28 293c 2f73 7061 6e3e 0a0a  ="p">()</span>..
+00097b20: 3c73 7061 6e20 636c 6173 733d 226e 6222  <span class="nb"
+00097b30: 3e70 7269 6e74 3c2f 7370 616e 3e3c 7370  >print</span><sp
+00097b40: 616e 2063 6c61 7373 3d22 7022 3e28 3c2f  an class="p">(</
+00097b50: 7370 616e 3e3c 7370 616e 2063 6c61 7373  span><span class
+00097b60: 3d22 7331 223e 2623 3339 3b4d 756c 7469  ="s1">&#39;Multi
+00097b70: 706c 6520 4173 7065 6374 2054 7261 6a65  ple Aspect Traje
+00097b80: 636f 7279 2064 6174 6173 6574 733a 2623  cory datasets:&#
+00097b90: 3339 3b3c 2f73 7061 6e3e 3c73 7061 6e20  39;</span><span 
+00097ba0: 636c 6173 733d 2270 223e 2c3c 2f73 7061  class="p">,</spa
+00097bb0: 6e3e 203c 7370 616e 2063 6c61 7373 3d22  n> <span class="
+00097bc0: 6e22 3e72 643c 2f73 7061 6e3e 3c73 7061  n">rd</span><spa
+00097bd0: 6e20 636c 6173 733d 2270 223e 5b3c 2f73  n class="p">[</s
+00097be0: 7061 6e3e 3c73 7061 6e20 636c 6173 733d  pan><span class=
+00097bf0: 2273 3122 3e26 2333 393b 6d61 7426 2333  "s1">&#39;mat&#3
+00097c00: 393b 3c2f 7370 616e 3e3c 7370 616e 2063  9;</span><span c
+00097c10: 6c61 7373 3d22 7022 3e5d 293c 2f73 7061  lass="p">])</spa
+00097c20: 6e3e 0a0a 3c73 7061 6e20 636c 6173 733d  n>..<span class=
+00097c30: 226e 223e 7264 3c2f 7370 616e 3e0a 3c2f  "n">rd</span>.</
+00097c40: 7072 653e 3c2f 6469 763e 0a0a 2020 2020  pre></div>..    
+00097c50: 203c 2f64 6976 3e0a 3c2f 6469 763e 0a3c   </div>.</div>.<
+00097c60: 2f64 6976 3e0a 3c2f 6469 763e 0a0a 3c64  /div>.</div>..<d
+00097c70: 6976 2063 6c61 7373 3d22 6a70 2d43 656c  iv class="jp-Cel
+00097c80: 6c2d 6f75 7470 7574 5772 6170 7065 7222  l-outputWrapper"
+00097c90: 3e0a 3c64 6976 2063 6c61 7373 3d22 6a70  >.<div class="jp
+00097ca0: 2d43 6f6c 6c61 7073 6572 206a 702d 4f75  -Collapser jp-Ou
+00097cb0: 7470 7574 436f 6c6c 6170 7365 7220 6a70  tputCollapser jp
+00097cc0: 2d43 656c 6c2d 6f75 7470 7574 436f 6c6c  -Cell-outputColl
+00097cd0: 6170 7365 7222 3e0a 3c2f 6469 763e 0a0a  apser">.</div>..
+00097ce0: 0a3c 6469 7620 636c 6173 733d 226a 702d  .<div class="jp-
+00097cf0: 4f75 7470 7574 4172 6561 206a 702d 4365  OutputArea jp-Ce
+00097d00: 6c6c 2d6f 7574 7075 7441 7265 6122 3e0a  ll-outputArea">.
+00097d10: 0a3c 6469 7620 636c 6173 733d 226a 702d  .<div class="jp-
+00097d20: 4f75 7470 7574 4172 6561 2d63 6869 6c64  OutputArea-child
+00097d30: 223e 0a0a 2020 2020 0a20 2020 203c 6469  ">..    .    <di
+00097d40: 7620 636c 6173 733d 226a 702d 4f75 7470  v class="jp-Outp
+00097d50: 7574 5072 6f6d 7074 206a 702d 4f75 7470  utPrompt jp-Outp
+00097d60: 7574 4172 6561 2d70 726f 6d70 7422 3e3c  utArea-prompt"><
+00097d70: 2f64 6976 3e0a 0a0a 3c64 6976 2063 6c61  /div>...<div cla
+00097d80: 7373 3d22 6a70 2d52 656e 6465 7265 6454  ss="jp-RenderedT
+00097d90: 6578 7420 6a70 2d4f 7574 7075 7441 7265  ext jp-OutputAre
+00097da0: 612d 6f75 7470 7574 2220 6461 7461 2d6d  a-output" data-m
+00097db0: 696d 652d 7479 7065 3d22 7465 7874 2f70  ime-type="text/p
+00097dc0: 6c61 696e 223e 0a3c 7072 653e 4d75 6c74  lain">.<pre>Mult
+00097dd0: 6970 6c65 2041 7370 6563 7420 5472 616a  iple Aspect Traj
+00097de0: 6563 6f72 7920 6461 7461 7365 7473 3a20  ecory datasets: 
+00097df0: 5b26 2333 393b 4272 6967 6874 6b69 7465  [&#39;Brightkite
+00097e00: 2623 3339 3b2c 2026 2333 393b 466f 7572  &#39;, &#39;Four
+00097e10: 7371 7561 7265 476c 6f62 616c 2623 3339  squareGlobal&#39
+00097e20: 3b2c 2026 2333 393b 466f 7572 7371 7561  ;, &#39;Foursqua
+00097e30: 7265 4e59 4326 2333 393b 2c20 2623 3339  reNYC&#39;, &#39
+00097e40: 3b47 6f77 616c 6c61 2623 3339 3b2c 2026  ;Gowalla&#39;, &
+00097e50: 2333 393b 5765 6570 6c61 6365 7326 2333  #39;Weeplaces&#3
+00097e60: 393b 5d0a 3c2f 7072 653e 0a3c 2f64 6976  9;].</pre>.</div
+00097e70: 3e0a 3c2f 6469 763e 0a0a 3c64 6976 2063  >.</div>..<div c
+00097e80: 6c61 7373 3d22 6a70 2d4f 7574 7075 7441  lass="jp-OutputA
+00097e90: 7265 612d 6368 696c 6422 3e0a 0a20 2020  rea-child">..   
+00097ea0: 200a 2020 2020 3c64 6976 2063 6c61 7373   .    <div class
+00097eb0: 3d22 6a70 2d4f 7574 7075 7450 726f 6d70  ="jp-OutputPromp
+00097ec0: 7420 6a70 2d4f 7574 7075 7441 7265 612d  t jp-OutputArea-
+00097ed0: 7072 6f6d 7074 223e 4f75 745b 3138 5d3a  prompt">Out[18]:
+00097ee0: 3c2f 6469 763e 0a0a 0a0a 0a3c 6469 7620  </div>.....<div 
+00097ef0: 636c 6173 733d 226a 702d 5265 6e64 6572  class="jp-Render
+00097f00: 6564 5465 7874 206a 702d 4f75 7470 7574  edText jp-Output
+00097f10: 4172 6561 2d6f 7574 7075 7420 6a70 2d4f  Area-output jp-O
+00097f20: 7574 7075 7441 7265 612d 6578 6563 7574  utputArea-execut
+00097f30: 6552 6573 756c 7422 2064 6174 612d 6d69  eResult" data-mi
+00097f40: 6d65 2d74 7970 653d 2274 6578 742f 706c  me-type="text/pl
+00097f50: 6169 6e22 3e0a 3c70 7265 3e7b 2623 3339  ain">.<pre>{&#39
+00097f60: 3b6c 6f67 2623 3339 3b3a 205b 2623 3339  ;log&#39;: [&#39
+00097f70: 3b42 5049 3230 3131 2623 3339 3b2c 2026  ;BPI2011&#39;, &
+00097f80: 2333 393b 4250 4932 3031 3226 2333 393b  #39;BPI2012&#39;
+00097f90: 2c20 2623 3339 3b42 5049 3230 3135 2623  , &#39;BPI2015&#
+00097fa0: 3339 3b2c 2026 2333 393b 4250 4932 3031  39;, &#39;BPI201
+00097fb0: 3726 2333 393b 2c20 2623 3339 3b42 5049  7&#39;, &#39;BPI
+00097fc0: 3230 3138 2623 3339 3b2c 2026 2333 393b  2018&#39;, &#39;
+00097fd0: 4250 4932 3031 3926 2333 393b 5d2c 0a20  BPI2019&#39;],. 
+00097fe0: 2623 3339 3b6d 6174 2623 3339 3b3a 205b  &#39;mat&#39;: [
+00097ff0: 2623 3339 3b42 7269 6768 746b 6974 6526  &#39;Brightkite&
+00098000: 2333 393b 2c0a 2020 2623 3339 3b46 6f75  #39;,.  &#39;Fou
+00098010: 7273 7175 6172 6547 6c6f 6261 6c26 2333  rsquareGlobal&#3
+00098020: 393b 2c0a 2020 2623 3339 3b46 6f75 7273  9;,.  &#39;Fours
+00098030: 7175 6172 654e 5943 2623 3339 3b2c 0a20  quareNYC&#39;,. 
+00098040: 2026 2333 393b 476f 7761 6c6c 6126 2333   &#39;Gowalla&#3
+00098050: 393b 2c0a 2020 2623 3339 3b57 6565 706c  9;,.  &#39;Weepl
+00098060: 6163 6573 2623 3339 3b5d 2c0a 2026 2333  aces&#39;],. &#3
+00098070: 393b 6d74 7326 2333 393b 3a20 5b26 2333  9;mts&#39;: [&#3
+00098080: 393b 4163 7469 7669 7479 5265 636f 676e  9;ActivityRecogn
+00098090: 6974 696f 6e26 2333 393b 2c0a 2020 2623  ition&#39;,.  &#
+000980a0: 3339 3b41 7274 6963 756c 6172 7957 6f72  39;ArticularyWor
+000980b0: 6452 6563 6f67 6e69 7469 6f6e 2623 3339  dRecognition&#39
+000980c0: 3b2c 0a20 2026 2333 393b 4174 7269 616c  ;,.  &#39;Atrial
+000980d0: 4669 6272 696c 6c61 7469 6f6e 2623 3339  Fibrillation&#39
+000980e0: 3b2c 0a20 2026 2333 393b 4175 7374 7261  ;,.  &#39;Austra
+000980f0: 6c69 616e 5369 676e 4c61 6e67 7561 6765  lianSignLanguage
+00098100: 2623 3339 3b2c 0a20 2026 2333 393b 4261  &#39;,.  &#39;Ba
+00098110: 7369 634d 6f74 696f 6e73 2623 3339 3b2c  sicMotions&#39;,
+00098120: 0a20 2026 2333 393b 4368 6172 6163 7465  .  &#39;Characte
+00098130: 7254 7261 6a65 6374 6f72 6965 7326 2333  rTrajectories&#3
+00098140: 393b 2c0a 2020 2623 3339 3b43 7269 636b  9;,.  &#39;Crick
+00098150: 6574 2623 3339 3b2c 0a20 2026 2333 393b  et&#39;,.  &#39;
+00098160: 4475 636b 4475 636b 4765 6573 6526 2333  DuckDuckGeese&#3
+00098170: 393b 2c0a 2020 2623 3339 3b45 5269 6e67  9;,.  &#39;ERing
+00098180: 2623 3339 3b2c 0a20 2026 2333 393b 4569  &#39;,.  &#39;Ei
+00098190: 6765 6e57 6f72 6d73 2623 3339 3b2c 0a20  genWorms&#39;,. 
+000981a0: 2026 2333 393b 4570 696c 6570 7379 2623   &#39;Epilepsy&#
+000981b0: 3339 3b2c 0a20 2026 2333 393b 4574 6861  39;,.  &#39;Etha
+000981c0: 6e6f 6c43 6f6e 6365 6e74 7261 7469 6f6e  nolConcentration
+000981d0: 2623 3339 3b2c 0a20 2026 2333 393b 4661  &#39;,.  &#39;Fa
+000981e0: 6365 4465 7465 6374 696f 6e26 2333 393b  ceDetection&#39;
+000981f0: 2c0a 2020 2623 3339 3b46 6163 6965 7352  ,.  &#39;FaciesR
+00098200: 6f63 6b73 2623 3339 3b2c 0a20 2026 2333  ocks&#39;,.  &#3
+00098210: 393b 4669 6e67 6572 4d6f 7665 6d65 6e74  9;FingerMovement
+00098220: 7326 2333 393b 2c0a 2020 2623 3339 3b47  s&#39;,.  &#39;G
+00098230: 4543 434f 5761 7465 7226 2333 393b 2c0a  ECCOWater&#39;,.
+00098240: 2020 2623 3339 3b47 7261 6d6d 6174 6963    &#39;Grammatic
+00098250: 616c 4661 6369 616c 4578 7072 6573 7369  alFacialExpressi
+00098260: 6f6e 2623 3339 3b2c 0a20 2026 2333 393b  on&#39;,.  &#39;
+00098270: 4861 6e64 4d6f 7665 6d65 6e74 4469 7265  HandMovementDire
+00098280: 6374 696f 6e26 2333 393b 2c0a 2020 2623  ction&#39;,.  &#
+00098290: 3339 3b48 616e 6477 7269 7469 6e67 2623  39;Handwriting&#
+000982a0: 3339 3b2c 0a20 2026 2333 393b 4865 6172  39;,.  &#39;Hear
+000982b0: 7462 6561 7426 2333 393b 2c0a 2020 2623  tbeat&#39;,.  &#
+000982c0: 3339 3b49 6e73 6563 7457 696e 6762 6561  39;InsectWingbea
+000982d0: 7426 2333 393b 2c0a 2020 2623 3339 3b4a  t&#39;,.  &#39;J
+000982e0: 6170 616e 6573 6556 6f77 656c 7326 2333  apaneseVowels&#3
+000982f0: 393b 2c0a 2020 2623 3339 3b4c 5353 5426  9;,.  &#39;LSST&
+00098300: 2333 393b 2c0a 2020 2623 3339 3b4c 6962  #39;,.  &#39;Lib
+00098310: 7261 7326 2333 393b 2c0a 2020 2623 3339  ras&#39;,.  &#39
+00098320: 3b4d 6f74 6f72 496d 6167 6572 7926 2333  ;MotorImagery&#3
+00098330: 393b 2c0a 2020 2623 3339 3b4e 4154 4f50  9;,.  &#39;NATOP
+00098340: 5326 2333 393b 2c0a 2020 2623 3339 3b50  S&#39;,.  &#39;P
+00098350: 454d 532d 5346 2623 3339 3b2c 0a20 2026  EMS-SF&#39;,.  &
+00098360: 2333 393b 5065 6e44 6967 6974 7326 2333  #39;PenDigits&#3
+00098370: 393b 2c0a 2020 2623 3339 3b50 686f 6e65  9;,.  &#39;Phone
+00098380: 6d65 5370 6563 7472 6126 2333 393b 2c0a  meSpectra&#39;,.
+00098390: 2020 2623 3339 3b52 6163 6b65 7453 706f    &#39;RacketSpo
+000983a0: 7274 7326 2333 393b 2c0a 2020 2623 3339  rts&#39;,.  &#39
+000983b0: 3b53 656c 6652 6567 756c 6174 696f 6e53  ;SelfRegulationS
+000983c0: 4350 3126 2333 393b 2c0a 2020 2623 3339  CP1&#39;,.  &#39
+000983d0: 3b53 656c 6652 6567 756c 6174 696f 6e53  ;SelfRegulationS
+000983e0: 4350 3226 2333 393b 2c0a 2020 2623 3339  CP2&#39;,.  &#39
+000983f0: 3b53 706f 6b65 6e41 7261 6269 6344 6967  ;SpokenArabicDig
+00098400: 6974 7326 2333 393b 2c0a 2020 2623 3339  its&#39;,.  &#39
+00098410: 3b53 7461 6e64 5761 6c6b 4a75 6d70 2623  ;StandWalkJump&#
+00098420: 3339 3b2c 0a20 2026 2333 393b 5557 6176  39;,.  &#39;UWav
+00098430: 6547 6573 7475 7265 4c69 6272 6172 7926  eGestureLibrary&
+00098440: 2333 393b 5d2c 0a20 2623 3339 3b72 6177  #39;],. &#39;raw
+00098450: 2623 3339 3b3a 205b 2623 3339 3b41 6e69  &#39;: [&#39;Ani
+00098460: 6d61 6c73 2623 3339 3b2c 2026 2333 393b  mals&#39;, &#39;
+00098470: 4765 6f6c 6966 6526 2333 393b 2c20 2623  Geolife&#39;, &#
+00098480: 3339 3b47 6f54 7261 636b 2623 3339 3b2c  39;GoTrack&#39;,
+00098490: 2026 2333 393b 4875 7272 6963 616e 6573   &#39;Hurricanes
+000984a0: 2623 3339 3b2c 2026 2333 393b 5665 6869  &#39;, &#39;Vehi
+000984b0: 636c 6573 2623 3339 3b5d 2c0a 2026 2333  cles&#39;],. &#3
+000984c0: 393b 7365 7175 656e 7469 616c 2623 3339  9;sequential&#39
+000984d0: 3b3a 205b 2623 3339 3b43 6c6f 7468 696e  ;: [&#39;Clothin
+000984e0: 6741 6c69 6261 6261 2623 3339 3b2c 2026  gAlibaba&#39;, &
+000984f0: 2333 393b 5072 6f6d 6f74 6572 7326 2333  #39;Promoters&#3
+00098500: 393b 2c20 2623 3339 3b53 4a47 5326 2333  9;, &#39;SJGS&#3
+00098510: 393b 5d2c 0a20 2623 3339 3b75 7473 2623  9;],. &#39;uts&#
+00098520: 3339 3b3a 205b 2623 3339 3b41 4353 4631  39;: [&#39;ACSF1
+00098530: 2623 3339 3b2c 0a20 2026 2333 393b 4164  &#39;,.  &#39;Ad
+00098540: 6961 6326 2333 393b 2c0a 2020 2623 3339  iac&#39;,.  &#39
+00098550: 3b41 6c6c 4765 7374 7572 6557 6969 6d6f  ;AllGestureWiimo
+00098560: 7465 5826 2333 393b 2c0a 2020 2623 3339  teX&#39;,.  &#39
+00098570: 3b41 6c6c 4765 7374 7572 6557 6969 6d6f  ;AllGestureWiimo
+00098580: 7465 5926 2333 393b 2c0a 2020 2623 3339  teY&#39;,.  &#39
+00098590: 3b41 6c6c 4765 7374 7572 6557 6969 6d6f  ;AllGestureWiimo
+000985a0: 7465 5a26 2333 393b 2c0a 2020 2623 3339  teZ&#39;,.  &#39
+000985b0: 3b41 7272 6f77 4865 6164 2623 3339 3b2c  ;ArrowHead&#39;,
+000985c0: 0a20 2026 2333 393b 424d 4526 2333 393b  .  &#39;BME&#39;
+000985d0: 2c0a 2020 2623 3339 3b42 6565 6626 2333  ,.  &#39;Beef&#3
+000985e0: 393b 2c0a 2020 2623 3339 3b42 6565 746c  9;,.  &#39;Beetl
+000985f0: 6546 6c79 2623 3339 3b2c 0a20 2026 2333  eFly&#39;,.  &#3
+00098600: 393b 4269 7264 4368 6963 6b65 6e26 2333  9;BirdChicken&#3
+00098610: 393b 2c0a 2020 2623 3339 3b43 4246 2623  9;,.  &#39;CBF&#
+00098620: 3339 3b2c 0a20 2026 2333 393b 4361 7226  39;,.  &#39;Car&
+00098630: 2333 393b 2c0a 2020 2623 3339 3b43 6869  #39;,.  &#39;Chi
+00098640: 6e61 746f 776e 2623 3339 3b2c 0a20 2026  natown&#39;,.  &
+00098650: 2333 393b 4368 6c6f 7269 6e65 436f 6e63  #39;ChlorineConc
+00098660: 656e 7472 6174 696f 6e26 2333 393b 2c0a  entration&#39;,.
+00098670: 2020 2623 3339 3b43 696e 4345 4347 546f    &#39;CinCECGTo
+00098680: 7273 6f26 2333 393b 2c0a 2020 2623 3339  rso&#39;,.  &#39
+00098690: 3b43 6f66 6665 6526 2333 393b 2c0a 2020  ;Coffee&#39;,.  
+000986a0: 2623 3339 3b43 6f6d 7075 7465 7273 2623  &#39;Computers&#
+000986b0: 3339 3b2c 0a20 2026 2333 393b 4372 6963  39;,.  &#39;Cric
+000986c0: 6b65 7458 2623 3339 3b2c 0a20 2026 2333  ketX&#39;,.  &#3
+000986d0: 393b 4372 6963 6b65 7459 2623 3339 3b2c  9;CricketY&#39;,
+000986e0: 0a20 2026 2333 393b 4372 6963 6b65 745a  .  &#39;CricketZ
+000986f0: 2623 3339 3b2c 0a20 2026 2333 393b 4372  &#39;,.  &#39;Cr
+00098700: 6f70 2623 3339 3b2c 0a20 2026 2333 393b  op&#39;,.  &#39;
+00098710: 4469 6174 6f6d 5369 7a65 5265 6475 6374  DiatomSizeReduct
+00098720: 696f 6e26 2333 393b 2c0a 2020 2623 3339  ion&#39;,.  &#39
+00098730: 3b44 6973 7461 6c50 6861 6c61 6e78 4f75  ;DistalPhalanxOu
+00098740: 746c 696e 6541 6765 4772 6f75 7026 2333  tlineAgeGroup&#3
+00098750: 393b 2c0a 2020 2623 3339 3b44 6973 7461  9;,.  &#39;Dista
+00098760: 6c50 6861 6c61 6e78 4f75 746c 696e 6543  lPhalanxOutlineC
+00098770: 6f72 7265 6374 2623 3339 3b2c 0a20 2026  orrect&#39;,.  &
+00098780: 2333 393b 4469 7374 616c 5068 616c 616e  #39;DistalPhalan
+00098790: 7854 5726 2333 393b 2c0a 2020 2623 3339  xTW&#39;,.  &#39
+000987a0: 3b44 6f64 6765 724c 6f6f 7044 6179 2623  ;DodgerLoopDay&#
+000987b0: 3339 3b2c 0a20 2026 2333 393b 446f 6467  39;,.  &#39;Dodg
+000987c0: 6572 4c6f 6f70 4761 6d65 2623 3339 3b2c  erLoopGame&#39;,
+000987d0: 0a20 2026 2333 393b 446f 6467 6572 4c6f  .  &#39;DodgerLo
+000987e0: 6f70 5765 656b 656e 6426 2333 393b 2c0a  opWeekend&#39;,.
+000987f0: 2020 2623 3339 3b45 4347 3230 3026 2333    &#39;ECG200&#3
+00098800: 393b 2c0a 2020 2623 3339 3b45 4347 3530  9;,.  &#39;ECG50
+00098810: 3030 2623 3339 3b2c 0a20 2026 2333 393b  00&#39;,.  &#39;
+00098820: 4543 4746 6976 6544 6179 7326 2333 393b  ECGFiveDays&#39;
+00098830: 2c0a 2020 2623 3339 3b45 4f47 486f 7269  ,.  &#39;EOGHori
+00098840: 7a6f 6e74 616c 5369 676e 616c 2623 3339  zontalSignal&#39
+00098850: 3b2c 0a20 2026 2333 393b 454f 4756 6572  ;,.  &#39;EOGVer
+00098860: 7469 6361 6c53 6967 6e61 6c26 2333 393b  ticalSignal&#39;
+00098870: 2c0a 2020 2623 3339 3b45 6172 7468 7175  ,.  &#39;Earthqu
+00098880: 616b 6573 2623 3339 3b2c 0a20 2026 2333  akes&#39;,.  &#3
+00098890: 393b 456c 6563 7472 6963 4465 7669 6365  9;ElectricDevice
+000988a0: 7326 2333 393b 2c0a 2020 2623 3339 3b45  s&#39;,.  &#39;E
+000988b0: 7468 616e 6f6c 4c65 7665 6c26 2333 393b  thanolLevel&#39;
+000988c0: 2c0a 2020 2623 3339 3b46 6163 6541 6c6c  ,.  &#39;FaceAll
+000988d0: 2623 3339 3b2c 0a20 2026 2333 393b 4661  &#39;,.  &#39;Fa
+000988e0: 6365 466f 7572 2623 3339 3b2c 0a20 2026  ceFour&#39;,.  &
+000988f0: 2333 393b 4661 6365 7355 4352 2623 3339  #39;FacesUCR&#39
+00098900: 3b2c 0a20 2026 2333 393b 4669 6674 7957  ;,.  &#39;FiftyW
+00098910: 6f72 6473 2623 3339 3b2c 0a20 2026 2333  ords&#39;,.  &#3
+00098920: 393b 4669 7368 2623 3339 3b2c 0a20 2026  9;Fish&#39;,.  &
+00098930: 2333 393b 466f 7264 4126 2333 393b 2c0a  #39;FordA&#39;,.
+00098940: 2020 2623 3339 3b46 6f72 6442 2623 3339    &#39;FordB&#39
+00098950: 3b2c 0a20 2026 2333 393b 4672 6565 7a65  ;,.  &#39;Freeze
+00098960: 7252 6567 756c 6172 5472 6169 6e26 2333  rRegularTrain&#3
+00098970: 393b 2c0a 2020 2623 3339 3b46 7265 657a  9;,.  &#39;Freez
+00098980: 6572 536d 616c 6c54 7261 696e 2623 3339  erSmallTrain&#39
+00098990: 3b2c 0a20 2026 2333 393b 4675 6e67 6926  ;,.  &#39;Fungi&
+000989a0: 2333 393b 2c0a 2020 2623 3339 3b47 6573  #39;,.  &#39;Ges
+000989b0: 7475 7265 4d69 6441 6972 4431 2623 3339  tureMidAirD1&#39
+000989c0: 3b2c 0a20 2026 2333 393b 4765 7374 7572  ;,.  &#39;Gestur
+000989d0: 654d 6964 4169 7244 3226 2333 393b 2c0a  eMidAirD2&#39;,.
+000989e0: 2020 2623 3339 3b47 6573 7475 7265 4d69    &#39;GestureMi
+000989f0: 6441 6972 4433 2623 3339 3b2c 0a20 2026  dAirD3&#39;,.  &
+00098a00: 2333 393b 4765 7374 7572 6550 6562 626c  #39;GesturePebbl
+00098a10: 655a 3126 2333 393b 2c0a 2020 2623 3339  eZ1&#39;,.  &#39
+00098a20: 3b47 6573 7475 7265 5065 6262 6c65 5a32  ;GesturePebbleZ2
+00098a30: 2623 3339 3b2c 0a20 2026 2333 393b 4775  &#39;,.  &#39;Gu
+00098a40: 6e50 6f69 6e74 2623 3339 3b2c 0a20 2026  nPoint&#39;,.  &
+00098a50: 2333 393b 4775 6e50 6f69 6e74 4167 6553  #39;GunPointAgeS
+00098a60: 7061 6e26 2333 393b 2c0a 2020 2623 3339  pan&#39;,.  &#39
+00098a70: 3b47 756e 506f 696e 744d 616c 6556 6572  ;GunPointMaleVer
+00098a80: 7375 7346 656d 616c 6526 2333 393b 2c0a  susFemale&#39;,.
+00098a90: 2020 2623 3339 3b47 756e 506f 696e 744f    &#39;GunPointO
+00098aa0: 6c64 5665 7273 7573 596f 756e 6726 2333  ldVersusYoung&#3
+00098ab0: 393b 2c0a 2020 2623 3339 3b48 616d 2623  9;,.  &#39;Ham&#
+00098ac0: 3339 3b2c 0a20 2026 2333 393b 4861 6e64  39;,.  &#39;Hand
+00098ad0: 4f75 746c 696e 6573 2623 3339 3b2c 0a20  Outlines&#39;,. 
+00098ae0: 2026 2333 393b 4861 7074 6963 7326 2333   &#39;Haptics&#3
+00098af0: 393b 2c0a 2020 2623 3339 3b48 6572 7269  9;,.  &#39;Herri
+00098b00: 6e67 2623 3339 3b2c 0a20 2026 2333 393b  ng&#39;,.  &#39;
+00098b10: 486f 7573 6554 7765 6e74 7926 2333 393b  HouseTwenty&#39;
+00098b20: 2c0a 2020 2623 3339 3b49 6e6c 696e 6553  ,.  &#39;InlineS
+00098b30: 6b61 7465 2623 3339 3b2c 0a20 2026 2333  kate&#39;,.  &#3
+00098b40: 393b 496e 7365 6374 4550 4752 6567 756c  9;InsectEPGRegul
+00098b50: 6172 5472 6169 6e26 2333 393b 2c0a 2020  arTrain&#39;,.  
+00098b60: 2623 3339 3b49 6e73 6563 7445 5047 536d  &#39;InsectEPGSm
+00098b70: 616c 6c54 7261 696e 2623 3339 3b2c 0a20  allTrain&#39;,. 
+00098b80: 2026 2333 393b 496e 7365 6374 5769 6e67   &#39;InsectWing
+00098b90: 6265 6174 536f 756e 6426 2333 393b 2c0a  beatSound&#39;,.
+00098ba0: 2020 2623 3339 3b49 7461 6c79 506f 7765    &#39;ItalyPowe
+00098bb0: 7244 656d 616e 6426 2333 393b 2c0a 2020  rDemand&#39;,.  
+00098bc0: 2623 3339 3b4c 6172 6765 4b69 7463 6865  &#39;LargeKitche
+00098bd0: 6e41 7070 6c69 616e 6365 7326 2333 393b  nAppliances&#39;
+00098be0: 2c0a 2020 2623 3339 3b4c 6967 6874 6e69  ,.  &#39;Lightni
+00098bf0: 6e67 3226 2333 393b 2c0a 2020 2623 3339  ng2&#39;,.  &#39
+00098c00: 3b4c 6967 6874 6e69 6e67 3726 2333 393b  ;Lightning7&#39;
+00098c10: 2c0a 2020 2623 3339 3b4d 616c 6c61 7426  ,.  &#39;Mallat&
+00098c20: 2333 393b 2c0a 2020 2623 3339 3b4d 6561  #39;,.  &#39;Mea
+00098c30: 7426 2333 393b 2c0a 2020 2623 3339 3b4d  t&#39;,.  &#39;M
+00098c40: 6564 6963 616c 496d 6167 6573 2623 3339  edicalImages&#39
+00098c50: 3b2c 0a20 2026 2333 393b 4d65 6c62 6f75  ;,.  &#39;Melbou
+00098c60: 726e 6550 6564 6573 7472 6961 6e26 2333  rnePedestrian&#3
+00098c70: 393b 2c0a 2020 2623 3339 3b4d 6964 646c  9;,.  &#39;Middl
+00098c80: 6550 6861 6c61 6e78 4f75 746c 696e 6541  ePhalanxOutlineA
+00098c90: 6765 4772 6f75 7026 2333 393b 2c0a 2020  geGroup&#39;,.  
+00098ca0: 2623 3339 3b4d 6964 646c 6550 6861 6c61  &#39;MiddlePhala
+00098cb0: 6e78 4f75 746c 696e 6543 6f72 7265 6374  nxOutlineCorrect
+00098cc0: 2623 3339 3b2c 0a20 2026 2333 393b 4d69  &#39;,.  &#39;Mi
+00098cd0: 6464 6c65 5068 616c 616e 7854 5726 2333  ddlePhalanxTW&#3
+00098ce0: 393b 2c0a 2020 2623 3339 3b4d 6978 6564  9;,.  &#39;Mixed
+00098cf0: 5368 6170 6573 5265 6775 6c61 7254 7261  ShapesRegularTra
+00098d00: 696e 2623 3339 3b2c 0a20 2026 2333 393b  in&#39;,.  &#39;
+00098d10: 4d69 7865 6453 6861 7065 7353 6d61 6c6c  MixedShapesSmall
+00098d20: 5472 6169 6e26 2333 393b 2c0a 2020 2623  Train&#39;,.  &#
+00098d30: 3339 3b4d 6f74 6553 7472 6169 6e26 2333  39;MoteStrain&#3
+00098d40: 393b 2c0a 2020 2623 3339 3b4e 6f6e 496e  9;,.  &#39;NonIn
+00098d50: 7661 7369 7665 4665 7461 6c45 4347 5468  vasiveFetalECGTh
+00098d60: 6f72 6178 3126 2333 393b 2c0a 2020 2623  orax1&#39;,.  &#
+00098d70: 3339 3b4e 6f6e 496e 7661 7369 7665 4665  39;NonInvasiveFe
+00098d80: 7461 6c45 4347 5468 6f72 6178 3226 2333  talECGThorax2&#3
+00098d90: 393b 2c0a 2020 2623 3339 3b4f 5355 4c65  9;,.  &#39;OSULe
+00098da0: 6166 2623 3339 3b2c 0a20 2026 2333 393b  af&#39;,.  &#39;
+00098db0: 4f6c 6976 654f 696c 2623 3339 3b2c 0a20  OliveOil&#39;,. 
+00098dc0: 2026 2333 393b 504c 4149 4426 2333 393b   &#39;PLAID&#39;
+00098dd0: 2c0a 2020 2623 3339 3b50 6861 6c61 6e67  ,.  &#39;Phalang
+00098de0: 6573 4f75 746c 696e 6573 436f 7272 6563  esOutlinesCorrec
+00098df0: 7426 2333 393b 2c0a 2020 2623 3339 3b50  t&#39;,.  &#39;P
+00098e00: 686f 6e65 6d65 2623 3339 3b2c 0a20 2026  honeme&#39;,.  &
+00098e10: 2333 393b 5069 636b 7570 4765 7374 7572  #39;PickupGestur
+00098e20: 6557 6969 6d6f 7465 5a26 2333 393b 2c0a  eWiimoteZ&#39;,.
+00098e30: 2020 2623 3339 3b50 6967 4169 7277 6179    &#39;PigAirway
+00098e40: 5072 6573 7375 7265 2623 3339 3b2c 0a20  Pressure&#39;,. 
+00098e50: 2026 2333 393b 5069 6741 7274 5072 6573   &#39;PigArtPres
+00098e60: 7375 7265 2623 3339 3b2c 0a20 2026 2333  sure&#39;,.  &#3
+00098e70: 393b 5069 6743 5650 2623 3339 3b2c 0a20  9;PigCVP&#39;,. 
+00098e80: 2026 2333 393b 506c 616e 6526 2333 393b   &#39;Plane&#39;
+00098e90: 2c0a 2020 2623 3339 3b50 6f77 6572 436f  ,.  &#39;PowerCo
+00098ea0: 6e73 2623 3339 3b2c 0a20 2026 2333 393b  ns&#39;,.  &#39;
+00098eb0: 5072 6f78 696d 616c 5068 616c 616e 784f  ProximalPhalanxO
+00098ec0: 7574 6c69 6e65 4167 6547 726f 7570 2623  utlineAgeGroup&#
+00098ed0: 3339 3b2c 0a20 2026 2333 393b 5072 6f78  39;,.  &#39;Prox
+00098ee0: 696d 616c 5068 616c 616e 784f 7574 6c69  imalPhalanxOutli
+00098ef0: 6e65 436f 7272 6563 7426 2333 393b 2c0a  neCorrect&#39;,.
+00098f00: 2020 2623 3339 3b50 726f 7869 6d61 6c50    &#39;ProximalP
+00098f10: 6861 6c61 6e78 5457 2623 3339 3b2c 0a20  halanxTW&#39;,. 
+00098f20: 2026 2333 393b 5265 6672 6967 6572 6174   &#39;Refrigerat
+00098f30: 696f 6e44 6576 6963 6573 2623 3339 3b2c  ionDevices&#39;,
+00098f40: 0a20 2026 2333 393b 526f 636b 2623 3339  .  &#39;Rock&#39
+00098f50: 3b2c 0a20 2026 2333 393b 5363 7265 656e  ;,.  &#39;Screen
+00098f60: 5479 7065 2623 3339 3b2c 0a20 2026 2333  Type&#39;,.  &#3
+00098f70: 393b 5365 6d67 4861 6e64 4765 6e64 6572  9;SemgHandGender
+00098f80: 4368 3226 2333 393b 2c0a 2020 2623 3339  Ch2&#39;,.  &#39
+00098f90: 3b53 656d 6748 616e 644d 6f76 656d 656e  ;SemgHandMovemen
+00098fa0: 7443 6832 2623 3339 3b2c 0a20 2026 2333  tCh2&#39;,.  &#3
+00098fb0: 393b 5365 6d67 4861 6e64 5375 626a 6563  9;SemgHandSubjec
+00098fc0: 7443 6832 2623 3339 3b2c 0a20 2026 2333  tCh2&#39;,.  &#3
+00098fd0: 393b 5368 616b 6547 6573 7475 7265 5769  9;ShakeGestureWi
+00098fe0: 696d 6f74 655a 2623 3339 3b2c 0a20 2026  imoteZ&#39;,.  &
+00098ff0: 2333 393b 5368 6170 656c 6574 5369 6d26  #39;ShapeletSim&
+00099000: 2333 393b 2c0a 2020 2623 3339 3b53 6861  #39;,.  &#39;Sha
+00099010: 7065 7341 6c6c 2623 3339 3b2c 0a20 2026  pesAll&#39;,.  &
+00099020: 2333 393b 536d 616c 6c4b 6974 6368 656e  #39;SmallKitchen
+00099030: 4170 706c 6961 6e63 6573 2623 3339 3b2c  Appliances&#39;,
+00099040: 0a20 2026 2333 393b 536d 6f6f 7468 5375  .  &#39;SmoothSu
+00099050: 6273 7061 6365 2623 3339 3b2c 0a20 2026  bspace&#39;,.  &
+00099060: 2333 393b 536f 6e79 4149 424f 526f 626f  #39;SonyAIBORobo
+00099070: 7453 7572 6661 6365 3126 2333 393b 2c0a  tSurface1&#39;,.
+00099080: 2020 2623 3339 3b53 6f6e 7941 4942 4f52    &#39;SonyAIBOR
+00099090: 6f62 6f74 5375 7266 6163 6532 2623 3339  obotSurface2&#39
+000990a0: 3b2c 0a20 2026 2333 393b 5374 6172 4c69  ;,.  &#39;StarLi
+000990b0: 6768 7443 7572 7665 7326 2333 393b 2c0a  ghtCurves&#39;,.
+000990c0: 2020 2623 3339 3b53 7472 6177 6265 7272    &#39;Strawberr
+000990d0: 7926 2333 393b 2c0a 2020 2623 3339 3b53  y&#39;,.  &#39;S
+000990e0: 7765 6469 7368 4c65 6166 2623 3339 3b2c  wedishLeaf&#39;,
+000990f0: 0a20 2026 2333 393b 5379 6d62 6f6c 7326  .  &#39;Symbols&
+00099100: 2333 393b 2c0a 2020 2623 3339 3b53 796e  #39;,.  &#39;Syn
+00099110: 7468 6574 6963 436f 6e74 726f 6c26 2333  theticControl&#3
+00099120: 393b 2c0a 2020 2623 3339 3b54 6f65 5365  9;,.  &#39;ToeSe
+00099130: 676d 656e 7461 7469 6f6e 3126 2333 393b  gmentation1&#39;
+00099140: 2c0a 2020 2623 3339 3b54 6f65 5365 676d  ,.  &#39;ToeSegm
+00099150: 656e 7461 7469 6f6e 3226 2333 393b 2c0a  entation2&#39;,.
+00099160: 2020 2623 3339 3b54 7261 6365 2623 3339    &#39;Trace&#39
+00099170: 3b2c 0a20 2026 2333 393b 5477 6f4c 6561  ;,.  &#39;TwoLea
+00099180: 6445 4347 2623 3339 3b2c 0a20 2026 2333  dECG&#39;,.  &#3
+00099190: 393b 5477 6f50 6174 7465 726e 7326 2333  9;TwoPatterns&#3
+000991a0: 393b 2c0a 2020 2623 3339 3b55 4d44 2623  9;,.  &#39;UMD&#
+000991b0: 3339 3b2c 0a20 2026 2333 393b 5557 6176  39;,.  &#39;UWav
+000991c0: 6547 6573 7475 7265 4c69 6272 6172 7941  eGestureLibraryA
+000991d0: 6c6c 2623 3339 3b2c 0a20 2026 2333 393b  ll&#39;,.  &#39;
+000991e0: 5557 6176 6547 6573 7475 7265 4c69 6272  UWaveGestureLibr
+000991f0: 6172 7958 2623 3339 3b2c 0a20 2026 2333  aryX&#39;,.  &#3
+00099200: 393b 5557 6176 6547 6573 7475 7265 4c69  9;UWaveGestureLi
+00099210: 6272 6172 7959 2623 3339 3b2c 0a20 2026  braryY&#39;,.  &
+00099220: 2333 393b 5557 6176 6547 6573 7475 7265  #39;UWaveGesture
+00099230: 4c69 6272 6172 795a 2623 3339 3b2c 0a20  LibraryZ&#39;,. 
+00099240: 2026 2333 393b 5761 6665 7226 2333 393b   &#39;Wafer&#39;
+00099250: 2c0a 2020 2623 3339 3b57 696e 6526 2333  ,.  &#39;Wine&#3
+00099260: 393b 2c0a 2020 2623 3339 3b57 6f72 6453  9;,.  &#39;WordS
+00099270: 796e 6f6e 796d 7326 2333 393b 2c0a 2020  ynonyms&#39;,.  
+00099280: 2623 3339 3b57 6f72 6d73 2623 3339 3b2c  &#39;Worms&#39;,
+00099290: 0a20 2026 2333 393b 576f 726d 7354 776f  .  &#39;WormsTwo
+000992a0: 436c 6173 7326 2333 393b 2c0a 2020 2623  Class&#39;,.  &#
+000992b0: 3339 3b59 6f67 6126 2333 393b 5d7d 3c2f  39;Yoga&#39;]}</
+000992c0: 7072 653e 0a3c 2f64 6976 3e0a 0a3c 2f64  pre>.</div>..</d
+000992d0: 6976 3e0a 0a3c 2f64 6976 3e0a 0a3c 2f64  iv>..</div>..</d
+000992e0: 6976 3e0a 0a3c 2f64 6976 3e0a 3c64 6976  iv>..</div>.<div
+000992f0: 2063 6c61 7373 3d22 6a70 2d43 656c 6c20   class="jp-Cell 
+00099300: 6a70 2d4d 6172 6b64 6f77 6e43 656c 6c20  jp-MarkdownCell 
+00099310: 6a70 2d4e 6f74 6562 6f6f 6b2d 6365 6c6c  jp-Notebook-cell
+00099320: 223e 0a3c 6469 7620 636c 6173 733d 226a  ">.<div class="j
+00099330: 702d 4365 6c6c 2d69 6e70 7574 5772 6170  p-Cell-inputWrap
+00099340: 7065 7222 3e0a 3c64 6976 2063 6c61 7373  per">.<div class
+00099350: 3d22 6a70 2d43 6f6c 6c61 7073 6572 206a  ="jp-Collapser j
+00099360: 702d 496e 7075 7443 6f6c 6c61 7073 6572  p-InputCollapser
+00099370: 206a 702d 4365 6c6c 2d69 6e70 7574 436f   jp-Cell-inputCo
+00099380: 6c6c 6170 7365 7222 3e0a 3c2f 6469 763e  llapser">.</div>
+00099390: 0a3c 6469 7620 636c 6173 733d 226a 702d  .<div class="jp-
+000993a0: 496e 7075 7441 7265 6120 6a70 2d43 656c  InputArea jp-Cel
+000993b0: 6c2d 696e 7075 7441 7265 6122 3e3c 6469  l-inputArea"><di
+000993c0: 7620 636c 6173 733d 226a 702d 496e 7075  v class="jp-Inpu
+000993d0: 7450 726f 6d70 7420 6a70 2d49 6e70 7574  tPrompt jp-Input
+000993e0: 4172 6561 2d70 726f 6d70 7422 3e0a 3c2f  Area-prompt">.</
+000993f0: 6469 763e 3c64 6976 2063 6c61 7373 3d22  div><div class="
+00099400: 6a70 2d52 656e 6465 7265 6448 544d 4c43  jp-RenderedHTMLC
+00099410: 6f6d 6d6f 6e20 6a70 2d52 656e 6465 7265  ommon jp-Rendere
+00099420: 644d 6172 6b64 6f77 6e20 6a70 2d4d 6172  dMarkdown jp-Mar
+00099430: 6b64 6f77 6e4f 7574 7075 7420 2220 6461  kdownOutput " da
+00099440: 7461 2d6d 696d 652d 7479 7065 3d22 7465  ta-mime-type="te
+00099450: 7874 2f6d 6172 6b64 6f77 6e22 3e0a 3c68  xt/markdown">.<h
+00099460: 3320 6964 3d22 332e 2d50 7265 2d70 726f  3 id="3.-Pre-pro
+00099470: 6365 7373 696e 672d 6461 7461 223e 332e  cessing-data">3.
+00099480: 2050 7265 2d70 726f 6365 7373 696e 6720   Pre-processing 
+00099490: 6461 7461 3c61 2063 6c61 7373 3d22 616e  data<a class="an
+000994a0: 6368 6f72 2d6c 696e 6b22 2068 7265 663d  chor-link" href=
+000994b0: 2223 332e 2d50 7265 2d70 726f 6365 7373  "#3.-Pre-process
+000994c0: 696e 672d 6461 7461 223e 2623 3138 323b  ing-data">&#182;
+000994d0: 3c2f 613e 3c2f 6833 3e3c 703e 546f 2075  </a></h3><p>To u
+000994e0: 7365 2068 656c 7065 7273 2066 6f72 2064  se helpers for d
+000994f0: 6174 6120 7072 652d 7072 6f63 6573 7369  ata pre-processi
+00099500: 6e67 2c20 696d 706f 7274 2066 726f 6d20  ng, import from 
+00099510: 7061 636b 6167 6520 3c63 6f64 653e 6d61  package <code>ma
+00099520: 7464 6174 612e 7072 6570 726f 6365 7373  tdata.preprocess
+00099530: 3c2f 636f 6465 3e3a 3c2f 703e 0a0a 3c2f  </code>:</p>..</
+00099540: 6469 763e 0a3c 2f64 6976 3e0a 3c2f 6469  div>.</div>.</di
+00099550: 763e 0a3c 2f64 6976 3e3c 6469 7620 636c  v>.</div><div cl
+00099560: 6173 733d 226a 702d 4365 6c6c 206a 702d  ass="jp-Cell jp-
+00099570: 436f 6465 4365 6c6c 206a 702d 4e6f 7465  CodeCell jp-Note
+00099580: 626f 6f6b 2d63 656c 6c20 6a70 2d6d 6f64  book-cell jp-mod
+00099590: 2d6e 6f4f 7574 7075 7473 2020 223e 0a3c  -noOutputs  ">.<
+000995a0: 6469 7620 636c 6173 733d 226a 702d 4365  div class="jp-Ce
+000995b0: 6c6c 2d69 6e70 7574 5772 6170 7065 7222  ll-inputWrapper"
+000995c0: 3e0a 3c64 6976 2063 6c61 7373 3d22 6a70  >.<div class="jp
+000995d0: 2d43 6f6c 6c61 7073 6572 206a 702d 496e  -Collapser jp-In
+000995e0: 7075 7443 6f6c 6c61 7073 6572 206a 702d  putCollapser jp-
+000995f0: 4365 6c6c 2d69 6e70 7574 436f 6c6c 6170  Cell-inputCollap
+00099600: 7365 7222 3e0a 3c2f 6469 763e 0a3c 6469  ser">.</div>.<di
+00099610: 7620 636c 6173 733d 226a 702d 496e 7075  v class="jp-Inpu
+00099620: 7441 7265 6120 6a70 2d43 656c 6c2d 696e  tArea jp-Cell-in
+00099630: 7075 7441 7265 6122 3e0a 3c64 6976 2063  putArea">.<div c
+00099640: 6c61 7373 3d22 6a70 2d49 6e70 7574 5072  lass="jp-InputPr
+00099650: 6f6d 7074 206a 702d 496e 7075 7441 7265  ompt jp-InputAre
+00099660: 612d 7072 6f6d 7074 223e 496e 266e 6273  a-prompt">In&nbs
+00099670: 703b 5b31 395d 3a3c 2f64 6976 3e0a 3c64  p;[19]:</div>.<d
+00099680: 6976 2063 6c61 7373 3d22 6a70 2d43 6f64  iv class="jp-Cod
+00099690: 654d 6972 726f 7245 6469 746f 7220 6a70  eMirrorEditor jp
+000996a0: 2d45 6469 746f 7220 6a70 2d49 6e70 7574  -Editor jp-Input
+000996b0: 4172 6561 2d65 6469 746f 7222 2064 6174  Area-editor" dat
+000996c0: 612d 7479 7065 3d22 696e 6c69 6e65 223e  a-type="inline">
+000996d0: 0a20 2020 2020 3c64 6976 2063 6c61 7373  .     <div class
+000996e0: 3d22 436f 6465 4d69 7272 6f72 2063 6d2d  ="CodeMirror cm-
+000996f0: 732d 6a75 7079 7465 7222 3e0a 3c64 6976  s-jupyter">.<div
+00099700: 2063 6c61 7373 3d22 2068 6967 686c 6967   class=" highlig
+00099710: 6874 2068 6c2d 6970 7974 686f 6e33 223e  ht hl-ipython3">
+00099720: 3c70 7265 3e3c 7370 616e 3e3c 2f73 7061  <pre><span></spa
+00099730: 6e3e 3c73 7061 6e20 636c 6173 733d 226b  n><span class="k
+00099740: 6e22 3e66 726f 6d3c 2f73 7061 6e3e 203c  n">from</span> <
+00099750: 7370 616e 2063 6c61 7373 3d22 6e6e 223e  span class="nn">
+00099760: 6d61 7464 6174 612e 7072 6570 726f 6365  matdata.preproce
+00099770: 7373 3c2f 7370 616e 3e20 3c73 7061 6e20  ss</span> <span 
+00099780: 636c 6173 733d 226b 6e22 3e69 6d70 6f72  class="kn">impor
+00099790: 743c 2f73 7061 6e3e 203c 7370 616e 2063  t</span> <span c
+000997a0: 6c61 7373 3d22 6f22 3e2a 3c2f 7370 616e  lass="o">*</span
+000997b0: 3e0a 3c2f 7072 653e 3c2f 6469 763e 0a0a  >.</pre></div>..
+000997c0: 2020 2020 203c 2f64 6976 3e0a 3c2f 6469       </div>.</di
+000997d0: 763e 0a3c 2f64 6976 3e0a 3c2f 6469 763e  v>.</div>.</div>
+000997e0: 0a0a 3c2f 6469 763e 0a3c 6469 7620 636c  ..</div>.<div cl
+000997f0: 6173 733d 226a 702d 4365 6c6c 206a 702d  ass="jp-Cell jp-
+00099800: 4d61 726b 646f 776e 4365 6c6c 206a 702d  MarkdownCell jp-
+00099810: 4e6f 7465 626f 6f6b 2d63 656c 6c22 3e0a  Notebook-cell">.
+00099820: 3c64 6976 2063 6c61 7373 3d22 6a70 2d43  <div class="jp-C
+00099830: 656c 6c2d 696e 7075 7457 7261 7070 6572  ell-inputWrapper
+00099840: 223e 0a3c 6469 7620 636c 6173 733d 226a  ">.<div class="j
+00099850: 702d 436f 6c6c 6170 7365 7220 6a70 2d49  p-Collapser jp-I
+00099860: 6e70 7574 436f 6c6c 6170 7365 7220 6a70  nputCollapser jp
+00099870: 2d43 656c 6c2d 696e 7075 7443 6f6c 6c61  -Cell-inputColla
+00099880: 7073 6572 223e 0a3c 2f64 6976 3e0a 3c64  pser">.</div>.<d
+00099890: 6976 2063 6c61 7373 3d22 6a70 2d49 6e70  iv class="jp-Inp
+000998a0: 7574 4172 6561 206a 702d 4365 6c6c 2d69  utArea jp-Cell-i
+000998b0: 6e70 7574 4172 6561 223e 3c64 6976 2063  nputArea"><div c
+000998c0: 6c61 7373 3d22 6a70 2d49 6e70 7574 5072  lass="jp-InputPr
+000998d0: 6f6d 7074 206a 702d 496e 7075 7441 7265  ompt jp-InputAre
+000998e0: 612d 7072 6f6d 7074 223e 0a3c 2f64 6976  a-prompt">.</div
+000998f0: 3e3c 6469 7620 636c 6173 733d 226a 702d  ><div class="jp-
+00099900: 5265 6e64 6572 6564 4854 4d4c 436f 6d6d  RenderedHTMLComm
+00099910: 6f6e 206a 702d 5265 6e64 6572 6564 4d61  on jp-RenderedMa
+00099920: 726b 646f 776e 206a 702d 4d61 726b 646f  rkdown jp-Markdo
+00099930: 776e 4f75 7470 7574 2022 2064 6174 612d  wnOutput " data-
+00099940: 6d69 6d65 2d74 7970 653d 2274 6578 742f  mime-type="text/
+00099950: 6d61 726b 646f 776e 223e 0a3c 703e 5468  markdown">.<p>Th
+00099960: 6520 3c73 7472 6f6e 673e 7072 6570 726f  e <strong>prepro
+00099970: 6365 7373 3c2f 7374 726f 6e67 3e20 6d6f  cess</strong> mo
+00099980: 6475 6c65 2070 726f 7669 6465 7320 736f  dule provides so
+00099990: 6d65 2066 756e 6374 696f 6e73 2074 6f20  me functions to 
+000999a0: 776f 726b 2064 6174 613a 3c2f 703e 0a3c  work data:</p>.<
+000999b0: 703e 4261 7369 6320 6675 6e63 7469 6f6e  p>Basic function
+000999c0: 733a 3c2f 703e 0a3c 756c 3e0a 3c6c 693e  s:</p>.<ul>.<li>
+000999d0: 3c63 6f64 653e 7265 6164 4461 7461 7365  <code>readDatase
+000999e0: 743c 2f63 6f64 653e 3a20 6c6f 6164 2064  t</code>: load d
+000999f0: 6174 6173 6574 7320 6173 2070 616e 6461  atasets as panda
+00099a00: 7320 4461 7461 4672 616d 6520 2866 726f  s DataFrame (fro
+00099a10: 6d20 2e63 7376 2c20 2e70 6172 7175 6574  m .csv, .parquet
+00099a20: 2c20 2e7a 6970 2c20 2e74 7320 6f72 202e  , .zip, .ts or .
+00099a30: 7865 7329 3c2f 6c69 3e0a 3c6c 693e 3c63  xes)</li>.<li><c
+00099a40: 6f64 653e 6f72 6761 6e69 7a65 4672 616d  ode>organizeFram
+00099a50: 653c 2f63 6f64 653e 3a20 7374 616e 6461  e</code>: standa
+00099a60: 7264 697a 6520 6461 7461 2063 6f6c 756d  rdize data colum
+00099a70: 6e73 2066 6f72 2074 6865 2044 6174 6146  ns for the DataF
+00099a80: 7261 6d65 3c2f 6c69 3e0a 3c2f 756c 3e0a  rame</li>.</ul>.
+00099a90: 3c70 3e54 7261 696e 2061 6e64 2054 6573  <p>Train and Tes
+00099aa0: 7420 7370 6c69 7420 6675 6e63 7469 6f6e  t split function
+00099ab0: 733a 3c2f 703e 0a3c 756c 3e0a 3c6c 693e  s:</p>.<ul>.<li>
+00099ac0: 3c63 6f64 653e 7472 6169 6e54 6573 7453  <code>trainTestS
+00099ad0: 706c 6974 3c2f 636f 6465 3e3a 2073 706c  plit</code>: spl
+00099ae0: 6974 2064 6174 6173 6574 2028 7061 6e64  it dataset (pand
+00099af0: 6173 2044 6174 6146 7261 6d65 2920 696e  as DataFrame) in
+00099b00: 2074 7261 696e 202f 2074 6573 7420 2837   train / test (7
+00099b10: 302f 3330 2520 6279 2064 6566 6175 6c74  0/30% by default
+00099b20: 293c 2f6c 693e 0a3c 6c69 3e3c 636f 6465  )</li>.<li><code
+00099b30: 3e6b 666f 6c64 5f74 7261 696e 5465 7374  >kfold_trainTest
+00099b40: 5370 6c69 743c 2f63 6f64 653e 3a20 7370  Split</code>: sp
+00099b50: 6c69 7420 6461 7461 7365 7420 2870 616e  lit dataset (pan
+00099b60: 6461 7320 4461 7461 4672 616d 6529 2069  das DataFrame) i
+00099b70: 6e20 6b2d 666f 6c64 2074 7261 696e 202f  n k-fold train /
+00099b80: 2074 6573 7420 2835 2d66 6f6c 6420 6f66   test (5-fold of
+00099b90: 2038 302f 3230 2520 6561 6368 2066 6f6c   80/20% each fol
+00099ba0: 6420 6279 2064 6566 6175 6c74 293c 2f6c  d by default)</l
+00099bb0: 693e 0a3c 6c69 3e3c 636f 6465 3e73 7472  i>.<li><code>str
+00099bc0: 6174 6966 793c 2f63 6f64 653e 3a20 6578  atify</code>: ex
+00099bd0: 7472 6163 7420 7472 616a 6563 746f 7269  tract trajectori
+00099be0: 6573 2066 726f 6d20 7468 6520 6461 7461  es from the data
+00099bf0: 7365 742c 2072 6573 7065 6374 696e 6720  set, respecting 
+00099c00: 636c 6173 7320 6261 6c61 6e63 652c 2063  class balance, c
+00099c10: 7265 6174 696e 6720 6120 7375 6273 6574  reating a subset
+00099c20: 206f 6620 7468 6520 6461 7461 2028 746f   of the data (to
+00099c30: 2075 7365 2077 6865 6e20 736d 616c 6c65   use when smalle
+00099c40: 7220 6461 7461 7365 7473 2061 7265 206e  r datasets are n
+00099c50: 6565 6465 6429 3c2f 6c69 3e0a 3c6c 693e  eeded)</li>.<li>
+00099c60: 3c63 6f64 653e 6b6c 6162 656c 735f 7374  <code>klabels_st
+00099c70: 7261 7469 6679 3c2f 636f 6465 3e3a 206b  ratify</code>: k
+00099c80: 2d6c 6162 656c 7320 7374 6174 6966 6963  -labels statific
+00099c90: 6174 696f 6e20 2872 616e 646f 6d6c 7920  ation (randomly 
+00099ca0: 7365 6c65 6374 206b 2d6c 6162 656c 7320  select k-labels 
+00099cb0: 6672 6f6d 2074 6865 2064 6174 6173 6574  from the dataset
+00099cc0: 293c 2f6c 693e 0a3c 6c69 3e3c 636f 6465  )</li>.<li><code
+00099cd0: 3e6a 6f69 6e54 7261 696e 5465 7374 3c2f  >joinTrainTest</
+00099ce0: 636f 6465 3e3a 206a 6f69 6e73 2074 6865  code>: joins the
+00099cf0: 2073 6570 6172 6174 6564 2074 7261 696e   separated train
+00099d00: 2061 6e64 2074 6573 7420 6669 6c65 7320   and test files 
+00099d10: 696e 746f 206f 6e65 2044 6174 6146 7261  into one DataFra
+00099d20: 6d65 2e3c 2f6c 693e 0a3c 2f75 6c3e 0a3c  me.</li>.</ul>.<
+00099d30: 703e 5374 6174 6973 7469 6361 6c20 6675  p>Statistical fu
+00099d40: 6e63 7469 6f6e 733a 3c2f 703e 0a3c 756c  nctions:</p>.<ul
+00099d50: 3e0a 3c6c 693e 3c63 6f64 653e 7072 696e  >.<li><code>prin
+00099d60: 7446 6561 7475 7265 734a 534f 4e3c 2f63  tFeaturesJSON</c
+00099d70: 6f64 653e 3a20 7072 696e 7420 6120 6465  ode>: print a de
+00099d80: 6661 756c 7420 4a53 4f4e 2066 696c 6520  fault JSON file 
+00099d90: 6465 7363 7269 7074 6f72 2066 6f72 204d  descriptor for M
+00099da0: 6f76 656c 6574 7320 6d65 7468 6f64 7320  ovelets methods 
+00099db0: 2876 6572 7369 6f6e 2031 206f 7220 3229  (version 1 or 2)
+00099dc0: 3c2f 6c69 3e0a 3c6c 693e 3c63 6f64 653e  </li>.<li><code>
+00099dd0: 636f 756e 7443 6c61 7373 6573 3c2f 636f  countClasses</co
+00099de0: 6465 3e3a 2063 616c 6375 6c61 7465 7320  de>: calculates 
+00099df0: 7374 6174 6973 7469 6373 2066 726f 6d20  statistics from 
+00099e00: 6120 6461 7461 7365 7420 6461 7461 6672  a dataset datafr
+00099e10: 616d 653c 2f6c 693e 0a3c 6c69 3e3c 636f  ame</li>.<li><co
+00099e20: 6465 3e64 6656 6172 6961 6e63 653c 2f63  de>dfVariance</c
+00099e30: 6f64 653e 3a20 6361 6c63 756c 6174 6573  ode>: calculates
+00099e40: 2061 2076 6172 6961 6e63 6520 7261 6e6b   a variance rank
+00099e50: 2066 726f 6d20 6120 6461 7461 7365 7420   from a dataset 
+00099e60: 6461 7461 6672 616d 653c 2f6c 693e 0a3c  dataframe</li>.<
+00099e70: 6c69 3e3c 636f 6465 3e64 6653 7461 7473  li><code>dfStats
+00099e80: 3c2f 636f 6465 3e3a 2063 616c 6375 6c61  </code>: calcula
+00099e90: 7465 7320 6174 7472 6962 7574 6573 2073  tes attributes s
+00099ea0: 7461 7469 7374 6963 7320 6f72 6465 7265  tatistics ordere
+00099eb0: 6420 6279 2076 6172 6961 6e63 6520 6672  d by variance fr
+00099ec0: 6f6d 2061 2064 6174 6173 6574 2064 6174  om a dataset dat
+00099ed0: 6166 7261 6d65 3c2f 6c69 3e0a 3c6c 693e  aframe</li>.<li>
+00099ee0: 3c63 6f64 653e 6461 7461 7365 7453 7461  <code>datasetSta
+00099ef0: 7469 7374 6963 733c 2f63 6f64 653e 3a20  tistics</code>: 
+00099f00: 6765 6e65 7261 7465 7320 6461 7461 7365  generates datase
+00099f10: 7420 7374 6174 6973 7469 6373 2066 726f  t statistics fro
+00099f20: 6d20 6120 6461 7461 6672 616d 6520 696e  m a dataframe in
+00099f30: 206d 6172 6b64 6f77 6e20 7465 7874 2e3c   markdown text.<
+00099f40: 2f6c 693e 0a3c 2f75 6c3e 0a3c 703e 5479  /li>.</ul>.<p>Ty
+00099f50: 7065 2072 6561 6469 6e67 2066 756e 6374  pe reading funct
+00099f60: 696f 6e73 3a3c 2f70 3e0a 3c75 6c3e 0a3c  ions:</p>.<ul>.<
+00099f70: 6c69 3e3c 636f 6465 3e63 7376 3264 663c  li><code>csv2df<
+00099f80: 2f63 6f64 653e 3a20 7265 6164 7320 2e63  /code>: reads .c
+00099f90: 7376 2064 6174 6173 6574 2064 6174 6166  sv dataset dataf
+00099fa0: 7261 6d65 3c2f 6c69 3e0a 3c6c 693e 3c63  rame</li>.<li><c
+00099fb0: 6f64 653e 7061 7271 7565 7432 6466 3c2f  ode>parquet2df</
+00099fc0: 636f 6465 3e3a 2072 6561 6473 202e 7061  code>: reads .pa
+00099fd0: 7271 7565 7420 6461 7461 7365 7420 6461  rquet dataset da
+00099fe0: 7461 6672 616d 653c 2f6c 693e 0a3c 6c69  taframe</li>.<li
+00099ff0: 3e3c 636f 6465 3e7a 6970 3264 663c 2f63  ><code>zip2df</c
+0009a000: 6f64 653e 3a20 7265 6164 7320 2e7a 6970  ode>: reads .zip
+0009a010: 2064 6174 6173 6574 2064 6174 6166 7261   dataset datafra
+0009a020: 6d65 2028 7a69 7020 636f 6e74 6169 6e69  me (zip containi
+0009a030: 6e67 2074 7261 6a65 6374 6f72 7920 6373  ng trajectory cs
+0009a040: 7620 6669 6c65 7329 3c2f 6c69 3e0a 3c6c  v files)</li>.<l
+0009a050: 693e 3c63 6f64 653e 7473 3264 663c 2f63  i><code>ts2df</c
+0009a060: 6f64 653e 3a20 7265 6164 7320 2e74 7320  ode>: reads .ts 
+0009a070: 6461 7461 7365 7420 6461 7461 6672 616d  dataset datafram
+0009a080: 6520 2854 696d 6520 5365 7269 6573 2064  e (Time Series d
+0009a090: 6174 6120 666f 726d 6174 293c 2f6c 693e  ata format)</li>
+0009a0a0: 0a3c 6c69 3e3c 636f 6465 3e78 6573 3264  .<li><code>xes2d
+0009a0b0: 663c 2f63 6f64 653e 3a20 7265 6164 7320  f</code>: reads 
+0009a0c0: 2e78 6573 2064 6174 6173 6574 2064 6174  .xes dataset dat
+0009a0d0: 6166 7261 6d65 2028 6576 656e 7420 6c6f  aframe (event lo
+0009a0e0: 6720 2f20 6576 656e 7420 7374 7265 616d  g / event stream
+0009a0f0: 2066 696c 6529 3c2f 6c69 3e0a 3c6c 693e   file)</li>.<li>
+0009a100: 3c63 6f64 653e 6d61 7432 6466 3c2f 636f  <code>mat2df</co
+0009a110: 6465 3e3a 203c 656d 3e54 4f44 4f3c 2f65  de>: <em>TODO</e
+0009a120: 6d3e 2072 6561 6473 202e 6d61 7420 6461  m> reads .mat da
+0009a130: 7461 7365 7420 6461 7461 6672 616d 6520  taset dataframe 
+0009a140: 286d 756c 7469 706c 6520 6173 7065 6374  (multiple aspect
+0009a150: 2074 7261 6a65 6374 6f72 7920 7370 6563   trajectory spec
+0009a160: 6966 6963 2066 696c 6520 666f 726d 6174  ific file format
+0009a170: 293c 2f6c 693e 0a3c 2f75 6c3e 0a3c 703e  )</li>.</ul>.<p>
+0009a180: 4669 6c65 2063 6f6e 7665 7274 696f 6e20  File convertion 
+0009a190: 6675 6e63 7469 6f6e 733a 3c2f 703e 0a3c  functions:</p>.<
+0009a1a0: 756c 3e0a 3c6c 693e 3c63 6f64 653e 7a69  ul>.<li><code>zi
+0009a1b0: 7032 6373 763c 2f63 6f64 653e 3a20 636f  p2csv</code>: co
+0009a1c0: 6e76 6572 7473 202e 7a69 7020 6669 6c65  nverts .zip file
+0009a1d0: 7320 616e 6420 7361 7665 7320 746f 202e  s and saves to .
+0009a1e0: 6373 7620 6669 6c65 733c 2f6c 693e 0a3c  csv files</li>.<
+0009a1f0: 6c69 3e3c 636f 6465 3e64 6632 7a69 703c  li><code>df2zip<
+0009a200: 2f63 6f64 653e 3a20 636f 6e76 6572 7473  /code>: converts
+0009a210: 2044 6174 6146 7261 6d65 2061 6e64 2073   DataFrame and s
+0009a220: 6176 6573 2074 6f20 2e7a 6970 2066 696c  aves to .zip fil
+0009a230: 6573 3c2f 6c69 3e0a 3c6c 693e 3c63 6f64  es</li>.<li><cod
+0009a240: 653e 616e 7932 7473 3c2f 636f 6465 3e3a  e>any2ts</code>:
+0009a250: 2063 6f6e 7665 7274 7320 2e7a 6970 206f   converts .zip o
+0009a260: 7220 2e63 7376 2066 696c 6573 2061 6e64  r .csv files and
+0009a270: 2073 6176 6573 2074 6f20 2e74 7320 6669   saves to .ts fi
+0009a280: 6c65 733c 2f6c 693e 0a3c 6c69 3e3c 636f  les</li>.<li><co
+0009a290: 6465 3e78 6573 3263 7376 3c2f 636f 6465  de>xes2csv</code
+0009a2a0: 3e3a 2072 6561 6473 202e 7865 7320 6669  >: reads .xes fi
+0009a2b0: 6c65 7320 616e 6420 636f 6e76 6572 7473  les and converts
+0009a2c0: 2074 6f20 4461 7461 4672 616d 653c 2f6c   to DataFrame</l
+0009a2d0: 693e 0a3c 6c69 3e3c 636f 6465 3e63 6f6e  i>.<li><code>con
+0009a2e0: 7665 7274 4461 7461 7365 743c 2f63 6f64  vertDataset</cod
+0009a2f0: 653e 3a20 6465 6661 756c 7420 666f 726d  e>: default form
+0009a300: 6174 2063 6f6e 7665 7273 696f 6e73 2e20  at conversions. 
+0009a310: 5265 6164 7320 7468 6520 6461 7461 7365  Reads the datase
+0009a320: 7420 6669 6c65 7320 616e 6420 7361 7665  t files and save
+0009a330: 7320 696e 202e 6373 7620 616e 6420 2e7a  s in .csv and .z
+0009a340: 6970 2066 6f72 6d61 7473 2c20 616c 736f  ip formats, also
+0009a350: 2064 6f20 6b2d 666f 6c64 2073 706c 6974   do k-fold split
+0009a360: 2069 6620 6e6f 7420 7072 6573 656e 743c   if not present<
+0009a370: 2f6c 693e 0a3c 2f75 6c3e 0a0a 3c2f 6469  /li>.</ul>..</di
+0009a380: 763e 0a3c 2f64 6976 3e0a 3c2f 6469 763e  v>.</div>.</div>
+0009a390: 0a3c 2f64 6976 3e0a 3c64 6976 2063 6c61  .</div>.<div cla
+0009a3a0: 7373 3d22 6a70 2d43 656c 6c20 6a70 2d4d  ss="jp-Cell jp-M
+0009a3b0: 6172 6b64 6f77 6e43 656c 6c20 6a70 2d4e  arkdownCell jp-N
+0009a3c0: 6f74 6562 6f6f 6b2d 6365 6c6c 223e 0a3c  otebook-cell">.<
+0009a3d0: 6469 7620 636c 6173 733d 226a 702d 4365  div class="jp-Ce
+0009a3e0: 6c6c 2d69 6e70 7574 5772 6170 7065 7222  ll-inputWrapper"
+0009a3f0: 3e0a 3c64 6976 2063 6c61 7373 3d22 6a70  >.<div class="jp
+0009a400: 2d43 6f6c 6c61 7073 6572 206a 702d 496e  -Collapser jp-In
+0009a410: 7075 7443 6f6c 6c61 7073 6572 206a 702d  putCollapser jp-
+0009a420: 4365 6c6c 2d69 6e70 7574 436f 6c6c 6170  Cell-inputCollap
+0009a430: 7365 7222 3e0a 3c2f 6469 763e 0a3c 6469  ser">.</div>.<di
+0009a440: 7620 636c 6173 733d 226a 702d 496e 7075  v class="jp-Inpu
+0009a450: 7441 7265 6120 6a70 2d43 656c 6c2d 696e  tArea jp-Cell-in
+0009a460: 7075 7441 7265 6122 3e3c 6469 7620 636c  putArea"><div cl
+0009a470: 6173 733d 226a 702d 496e 7075 7450 726f  ass="jp-InputPro
+0009a480: 6d70 7420 6a70 2d49 6e70 7574 4172 6561  mpt jp-InputArea
+0009a490: 2d70 726f 6d70 7422 3e0a 3c2f 6469 763e  -prompt">.</div>
+0009a4a0: 3c64 6976 2063 6c61 7373 3d22 6a70 2d52  <div class="jp-R
+0009a4b0: 656e 6465 7265 6448 544d 4c43 6f6d 6d6f  enderedHTMLCommo
+0009a4c0: 6e20 6a70 2d52 656e 6465 7265 644d 6172  n jp-RenderedMar
+0009a4d0: 6b64 6f77 6e20 6a70 2d4d 6172 6b64 6f77  kdown jp-Markdow
+0009a4e0: 6e4f 7574 7075 7420 2220 6461 7461 2d6d  nOutput " data-m
+0009a4f0: 696d 652d 7479 7065 3d22 7465 7874 2f6d  ime-type="text/m
+0009a500: 6172 6b64 6f77 6e22 3e0a 0a3c 7072 653e  arkdown">..<pre>
+0009a510: 3c63 6f64 653e 6129 2042 6173 6963 2072  <code>a) Basic r
+0009a520: 6561 6469 6e67 2074 6865 2064 6174 612c  eading the data,
+0009a530: 2061 6e64 206f 7267 616e 697a 6174 696f   and organizatio
+0009a540: 6e3a 3c2f 636f 6465 3e3c 2f70 7265 3e0a  n:</code></pre>.
+0009a550: 0a3c 2f64 6976 3e0a 3c2f 6469 763e 0a3c  .</div>.</div>.<
+0009a560: 2f64 6976 3e0a 3c2f 6469 763e 3c64 6976  /div>.</div><div
+0009a570: 2063 6c61 7373 3d22 6a70 2d43 656c 6c20   class="jp-Cell 
+0009a580: 6a70 2d43 6f64 6543 656c 6c20 6a70 2d4e  jp-CodeCell jp-N
+0009a590: 6f74 6562 6f6f 6b2d 6365 6c6c 2020 2022  otebook-cell   "
+0009a5a0: 3e0a 3c64 6976 2063 6c61 7373 3d22 6a70  >.<div class="jp
+0009a5b0: 2d43 656c 6c2d 696e 7075 7457 7261 7070  -Cell-inputWrapp
+0009a5c0: 6572 223e 0a3c 6469 7620 636c 6173 733d  er">.<div class=
+0009a5d0: 226a 702d 436f 6c6c 6170 7365 7220 6a70  "jp-Collapser jp
+0009a5e0: 2d49 6e70 7574 436f 6c6c 6170 7365 7220  -InputCollapser 
+0009a5f0: 6a70 2d43 656c 6c2d 696e 7075 7443 6f6c  jp-Cell-inputCol
+0009a600: 6c61 7073 6572 223e 0a3c 2f64 6976 3e0a  lapser">.</div>.
+0009a610: 3c64 6976 2063 6c61 7373 3d22 6a70 2d49  <div class="jp-I
+0009a620: 6e70 7574 4172 6561 206a 702d 4365 6c6c  nputArea jp-Cell
+0009a630: 2d69 6e70 7574 4172 6561 223e 0a3c 6469  -inputArea">.<di
+0009a640: 7620 636c 6173 733d 226a 702d 496e 7075  v class="jp-Inpu
+0009a650: 7450 726f 6d70 7420 6a70 2d49 6e70 7574  tPrompt jp-Input
+0009a660: 4172 6561 2d70 726f 6d70 7422 3e49 6e26  Area-prompt">In&
+0009a670: 6e62 7370 3b5b 3230 5d3a 3c2f 6469 763e  nbsp;[20]:</div>
+0009a680: 0a3c 6469 7620 636c 6173 733d 226a 702d  .<div class="jp-
+0009a690: 436f 6465 4d69 7272 6f72 4564 6974 6f72  CodeMirrorEditor
+0009a6a0: 206a 702d 4564 6974 6f72 206a 702d 496e   jp-Editor jp-In
+0009a6b0: 7075 7441 7265 612d 6564 6974 6f72 2220  putArea-editor" 
+0009a6c0: 6461 7461 2d74 7970 653d 2269 6e6c 696e  data-type="inlin
+0009a6d0: 6522 3e0a 2020 2020 203c 6469 7620 636c  e">.     <div cl
+0009a6e0: 6173 733d 2243 6f64 654d 6972 726f 7220  ass="CodeMirror 
+0009a6f0: 636d 2d73 2d6a 7570 7974 6572 223e 0a3c  cm-s-jupyter">.<
+0009a700: 6469 7620 636c 6173 733d 2220 6869 6768  div class=" high
+0009a710: 6c69 6768 7420 686c 2d69 7079 7468 6f6e  light hl-ipython
+0009a720: 3322 3e3c 7072 653e 3c73 7061 6e3e 3c2f  3"><pre><span></
+0009a730: 7370 616e 3e3c 7370 616e 2063 6c61 7373  span><span class
+0009a740: 3d22 6e22 3e64 6174 615f 7061 7468 3c2f  ="n">data_path</
+0009a750: 7370 616e 3e20 3c73 7061 6e20 636c 6173  span> <span clas
+0009a760: 733d 226f 223e 3d3c 2f73 7061 6e3e 203c  s="o">=</span> <
+0009a770: 7370 616e 2063 6c61 7373 3d22 7331 223e  span class="s1">
+0009a780: 2623 3339 3b6d 6174 6461 7461 2f61 7373  &#39;matdata/ass
+0009a790: 6574 732f 7361 6d70 6c65 2623 3339 3b3c  ets/sample&#39;<
+0009a7a0: 2f73 7061 6e3e 0a0a 3c73 7061 6e20 636c  /span>..<span cl
+0009a7b0: 6173 733d 226e 223e 6466 3c2f 7370 616e  ass="n">df</span
+0009a7c0: 3e20 3c73 7061 6e20 636c 6173 733d 226f  > <span class="o
+0009a7d0: 223e 3d3c 2f73 7061 6e3e 203c 7370 616e  ">=</span> <span
+0009a7e0: 2063 6c61 7373 3d22 6e22 3e72 6561 6444   class="n">readD
+0009a7f0: 6174 6173 6574 3c2f 7370 616e 3e3c 7370  ataset</span><sp
+0009a800: 616e 2063 6c61 7373 3d22 7022 3e28 3c2f  an class="p">(</
+0009a810: 7370 616e 3e3c 7370 616e 2063 6c61 7373  span><span class
+0009a820: 3d22 6e22 3e64 6174 615f 7061 7468 3c2f  ="n">data_path</
+0009a830: 7370 616e 3e3c 7370 616e 2063 6c61 7373  span><span class
+0009a840: 3d22 7022 3e2c 3c2f 7370 616e 3e20 3c73  ="p">,</span> <s
+0009a850: 7061 6e20 636c 6173 733d 226e 223e 6669  pan class="n">fi
+0009a860: 6c65 3c2f 7370 616e 3e3c 7370 616e 2063  le</span><span c
+0009a870: 6c61 7373 3d22 6f22 3e3d 3c2f 7370 616e  lass="o">=</span
+0009a880: 3e3c 7370 616e 2063 6c61 7373 3d22 7331  ><span class="s1
+0009a890: 223e 2623 3339 3b46 6f75 7273 7175 6172  ">&#39;Foursquar
+0009a8a0: 655f 5361 6d70 6c65 2e63 7376 2623 3339  e_Sample.csv&#39
+0009a8b0: 3b3c 2f73 7061 6e3e 3c73 7061 6e20 636c  ;</span><span cl
+0009a8c0: 6173 733d 2270 223e 293c 2f73 7061 6e3e  ass="p">)</span>
+0009a8d0: 0a3c 7370 616e 2063 6c61 7373 3d22 6e22  .<span class="n"
+0009a8e0: 3e64 663c 2f73 7061 6e3e 3c73 7061 6e20  >df</span><span 
+0009a8f0: 636c 6173 733d 226f 223e 2e3c 2f73 7061  class="o">.</spa
+0009a900: 6e3e 3c73 7061 6e20 636c 6173 733d 226e  n><span class="n
+0009a910: 223e 6865 6164 3c2f 7370 616e 3e3c 7370  ">head</span><sp
+0009a920: 616e 2063 6c61 7373 3d22 7022 3e28 293c  an class="p">()<
+0009a930: 2f73 7061 6e3e 0a3c 2f70 7265 3e3c 2f64  /span>.</pre></d
+0009a940: 6976 3e0a 0a20 2020 2020 3c2f 6469 763e  iv>..     </div>
+0009a950: 0a3c 2f64 6976 3e0a 3c2f 6469 763e 0a3c  .</div>.</div>.<
+0009a960: 2f64 6976 3e0a 0a3c 6469 7620 636c 6173  /div>..<div clas
+0009a970: 733d 226a 702d 4365 6c6c 2d6f 7574 7075  s="jp-Cell-outpu
+0009a980: 7457 7261 7070 6572 223e 0a3c 6469 7620  tWrapper">.<div 
+0009a990: 636c 6173 733d 226a 702d 436f 6c6c 6170  class="jp-Collap
+0009a9a0: 7365 7220 6a70 2d4f 7574 7075 7443 6f6c  ser jp-OutputCol
+0009a9b0: 6c61 7073 6572 206a 702d 4365 6c6c 2d6f  lapser jp-Cell-o
+0009a9c0: 7574 7075 7443 6f6c 6c61 7073 6572 223e  utputCollapser">
+0009a9d0: 0a3c 2f64 6976 3e0a 0a0a 3c64 6976 2063  .</div>...<div c
+0009a9e0: 6c61 7373 3d22 6a70 2d4f 7574 7075 7441  lass="jp-OutputA
+0009a9f0: 7265 6120 6a70 2d43 656c 6c2d 6f75 7470  rea jp-Cell-outp
+0009aa00: 7574 4172 6561 223e 0a0a 3c64 6976 2063  utArea">..<div c
+0009aa10: 6c61 7373 3d22 6a70 2d4f 7574 7075 7441  lass="jp-OutputA
+0009aa20: 7265 612d 6368 696c 6422 3e0a 0a20 2020  rea-child">..   
+0009aa30: 200a 2020 2020 3c64 6976 2063 6c61 7373   .    <div class
+0009aa40: 3d22 6a70 2d4f 7574 7075 7450 726f 6d70  ="jp-OutputPromp
+0009aa50: 7420 6a70 2d4f 7574 7075 7441 7265 612d  t jp-OutputArea-
+0009aa60: 7072 6f6d 7074 223e 4f75 745b 3230 5d3a  prompt">Out[20]:
+0009aa70: 3c2f 6469 763e 0a0a 0a0a 3c64 6976 2063  </div>....<div c
+0009aa80: 6c61 7373 3d22 6a70 2d52 656e 6465 7265  lass="jp-Rendere
+0009aa90: 6448 544d 4c43 6f6d 6d6f 6e20 6a70 2d52  dHTMLCommon jp-R
+0009aaa0: 656e 6465 7265 6448 544d 4c20 6a70 2d4f  enderedHTML jp-O
+0009aab0: 7574 7075 7441 7265 612d 6f75 7470 7574  utputArea-output
+0009aac0: 206a 702d 4f75 7470 7574 4172 6561 2d65   jp-OutputArea-e
+0009aad0: 7865 6375 7465 5265 7375 6c74 2220 6461  xecuteResult" da
+0009aae0: 7461 2d6d 696d 652d 7479 7065 3d22 7465  ta-mime-type="te
+0009aaf0: 7874 2f68 746d 6c22 3e0a 3c64 6976 3e0a  xt/html">.<div>.
+0009ab00: 3c73 7479 6c65 2073 636f 7065 643e 0a20  <style scoped>. 
+0009ab10: 2020 202e 6461 7461 6672 616d 6520 7462     .dataframe tb
+0009ab20: 6f64 7920 7472 2074 683a 6f6e 6c79 2d6f  ody tr th:only-o
+0009ab30: 662d 7479 7065 207b 0a20 2020 2020 2020  f-type {.       
+0009ab40: 2076 6572 7469 6361 6c2d 616c 6967 6e3a   vertical-align:
+0009ab50: 206d 6964 646c 653b 0a20 2020 207d 0a0a   middle;.    }..
+0009ab60: 2020 2020 2e64 6174 6166 7261 6d65 2074      .dataframe t
+0009ab70: 626f 6479 2074 7220 7468 207b 0a20 2020  body tr th {.   
+0009ab80: 2020 2020 2076 6572 7469 6361 6c2d 616c       vertical-al
+0009ab90: 6967 6e3a 2074 6f70 3b0a 2020 2020 7d0a  ign: top;.    }.
+0009aba0: 0a20 2020 202e 6461 7461 6672 616d 6520  .    .dataframe 
+0009abb0: 7468 6561 6420 7468 207b 0a20 2020 2020  thead th {.     
+0009abc0: 2020 2074 6578 742d 616c 6967 6e3a 2072     text-align: r
+0009abd0: 6967 6874 3b0a 2020 2020 7d0a 3c2f 7374  ight;.    }.</st
+0009abe0: 796c 653e 0a3c 7461 626c 6520 626f 7264  yle>.<table bord
+0009abf0: 6572 3d22 3122 2063 6c61 7373 3d22 6461  er="1" class="da
+0009ac00: 7461 6672 616d 6522 3e0a 2020 3c74 6865  taframe">.  <the
+0009ac10: 6164 3e0a 2020 2020 3c74 7220 7374 796c  ad>.    <tr styl
+0009ac20: 653d 2274 6578 742d 616c 6967 6e3a 2072  e="text-align: r
+0009ac30: 6967 6874 3b22 3e0a 2020 2020 2020 3c74  ight;">.      <t
+0009ac40: 683e 3c2f 7468 3e0a 2020 2020 2020 3c74  h></th>.      <t
+0009ac50: 683e 7469 643c 2f74 683e 0a20 2020 2020  h>tid</th>.     
+0009ac60: 203c 7468 3e6c 6174 5f6c 6f6e 3c2f 7468   <th>lat_lon</th
+0009ac70: 3e0a 2020 2020 2020 3c74 683e 6461 7465  >.      <th>date
+0009ac80: 5f74 696d 653c 2f74 683e 0a20 2020 2020  _time</th>.     
+0009ac90: 203c 7468 3e74 696d 653c 2f74 683e 0a20   <th>time</th>. 
+0009aca0: 2020 2020 203c 7468 3e72 6174 696e 673c       <th>rating<
+0009acb0: 2f74 683e 0a20 2020 2020 203c 7468 3e70  /th>.      <th>p
+0009acc0: 7269 6365 3c2f 7468 3e0a 2020 2020 2020  rice</th>.      
+0009acd0: 3c74 683e 7765 6174 6865 723c 2f74 683e  <th>weather</th>
+0009ace0: 0a20 2020 2020 203c 7468 3e64 6179 3c2f  .      <th>day</
+0009acf0: 7468 3e0a 2020 2020 2020 3c74 683e 726f  th>.      <th>ro
+0009ad00: 6f74 5f74 7970 653c 2f74 683e 0a20 2020  ot_type</th>.   
+0009ad10: 2020 203c 7468 3e74 7970 653c 2f74 683e     <th>type</th>
+0009ad20: 0a20 2020 203c 2f74 723e 0a20 203c 2f74  .    </tr>.  </t
+0009ad30: 6865 6164 3e0a 2020 3c74 626f 6479 3e0a  head>.  <tbody>.
+0009ad40: 2020 2020 3c74 723e 0a20 2020 2020 203c      <tr>.      <
+0009ad50: 7468 3e30 3c2f 7468 3e0a 2020 2020 2020  th>0</th>.      
+0009ad60: 3c74 643e 3132 363c 2f74 643e 0a20 2020  <td>126</td>.   
+0009ad70: 2020 203c 7464 3e34 302e 3833 3331 3635     <td>40.833165
+0009ad80: 3230 3036 3232 3420 2d37 332e 3934 3138  2006224 -73.9418
+0009ad90: 3630 3334 3237 3639 323c 2f74 643e 0a20  603427692</td>. 
+0009ada0: 2020 2020 203c 7464 3e32 3031 322d 3131       <td>2012-11
+0009adb0: 2d31 3220 3035 3a31 373a 3138 3c2f 7464  -12 05:17:18</td
+0009adc0: 3e0a 2020 2020 2020 3c74 643e 3331 373c  >.      <td>317<
+0009add0: 2f74 643e 0a20 2020 2020 203c 7464 3e2d  /td>.      <td>-
+0009ade0: 312e 303c 2f74 643e 0a20 2020 2020 203c  1.0</td>.      <
+0009adf0: 7464 3e2d 313c 2f74 643e 0a20 2020 2020  td>-1</td>.     
+0009ae00: 203c 7464 3e43 6c65 6172 3c2f 7464 3e0a   <td>Clear</td>.
+0009ae10: 2020 2020 2020 3c74 643e 4d6f 6e64 6179        <td>Monday
+0009ae20: 3c2f 7464 3e0a 2020 2020 2020 3c74 643e  </td>.      <td>
+0009ae30: 5265 7369 6465 6e63 653c 2f74 643e 0a20  Residence</td>. 
+0009ae40: 2020 2020 203c 7464 3e48 6f6d 6520 2870       <td>Home (p
+0009ae50: 7269 7661 7465 293c 2f74 643e 0a20 2020  rivate)</td>.   
+0009ae60: 203c 2f74 723e 0a20 2020 203c 7472 3e0a   </tr>.    <tr>.
+0009ae70: 2020 2020 2020 3c74 683e 313c 2f74 683e        <th>1</th>
+0009ae80: 0a20 2020 2020 203c 7464 3e31 3236 3c2f  .      <td>126</
+0009ae90: 7464 3e0a 2020 2020 2020 3c74 643e 3430  td>.      <td>40
+0009aea0: 2e38 3334 3039 3738 3034 3130 3732 202d  .8340978041072 -
+0009aeb0: 3733 2e39 3435 3236 3732 3232 3538 3831  73.9452672225881
+0009aec0: 3c2f 7464 3e0a 2020 2020 2020 3c74 643e  </td>.      <td>
+0009aed0: 3230 3132 2d31 312d 3132 2032 333a 3234  2012-11-12 23:24
+0009aee0: 3a35 353c 2f74 643e 0a20 2020 2020 203c  :55</td>.      <
+0009aef0: 7464 3e31 3430 343c 2f74 643e 0a20 2020  td>1404</td>.   
+0009af00: 2020 203c 7464 3e38 2e32 3c2f 7464 3e0a     <td>8.2</td>.
+0009af10: 2020 2020 2020 3c74 643e 313c 2f74 643e        <td>1</td>
+0009af20: 0a20 2020 2020 203c 7464 3e43 6c6f 7564  .      <td>Cloud
+0009af30: 733c 2f74 643e 0a20 2020 2020 203c 7464  s</td>.      <td
+0009af40: 3e4d 6f6e 6461 793c 2f74 643e 0a20 2020  >Monday</td>.   
+0009af50: 2020 203c 7464 3e46 6f6f 643c 2f74 643e     <td>Food</td>
+0009af60: 0a20 2020 2020 203c 7464 3e44 656c 6920  .      <td>Deli 
+0009af70: 2f20 426f 6465 6761 3c2f 7464 3e0a 2020  / Bodega</td>.  
+0009af80: 2020 3c2f 7472 3e0a 2020 2020 3c74 723e    </tr>.    <tr>
+0009af90: 0a20 2020 2020 203c 7468 3e32 3c2f 7468  .      <th>2</th
+0009afa0: 3e0a 2020 2020 2020 3c74 643e 3132 363c  >.      <td>126<
+0009afb0: 2f74 643e 0a20 2020 2020 203c 7464 3e34  /td>.      <td>4
+0009afc0: 302e 3833 3331 3635 3230 3036 3232 3420  0.8331652006224 
+0009afd0: 2d37 332e 3934 3138 3630 3334 3237 3639  -73.941860342769
+0009afe0: 323c 2f74 643e 0a20 2020 2020 203c 7464  2</td>.      <td
+0009aff0: 3e32 3031 322d 3131 2d31 3320 3030 3a30  >2012-11-13 00:0
+0009b000: 303a 3037 3c2f 7464 3e0a 2020 2020 2020  0:07</td>.      
+0009b010: 3c74 643e 303c 2f74 643e 0a20 2020 2020  <td>0</td>.     
+0009b020: 203c 7464 3e2d 312e 303c 2f74 643e 0a20   <td>-1.0</td>. 
+0009b030: 2020 2020 203c 7464 3e2d 313c 2f74 643e       <td>-1</td>
+0009b040: 0a20 2020 2020 203c 7464 3e43 6c6f 7564  .      <td>Cloud
+0009b050: 733c 2f74 643e 0a20 2020 2020 203c 7464  s</td>.      <td
+0009b060: 3e54 7565 7364 6179 3c2f 7464 3e0a 2020  >Tuesday</td>.  
+0009b070: 2020 2020 3c74 643e 5265 7369 6465 6e63      <td>Residenc
+0009b080: 653c 2f74 643e 0a20 2020 2020 203c 7464  e</td>.      <td
+0009b090: 3e48 6f6d 6520 2870 7269 7661 7465 293c  >Home (private)<
+0009b0a0: 2f74 643e 0a20 2020 203c 2f74 723e 0a20  /td>.    </tr>. 
+0009b0b0: 2020 203c 7472 3e0a 2020 2020 2020 3c74     <tr>.      <t
+0009b0c0: 683e 333c 2f74 683e 0a20 2020 2020 203c  h>3</th>.      <
+0009b0d0: 7464 3e31 3236 3c2f 7464 3e0a 2020 2020  td>126</td>.    
+0009b0e0: 2020 3c74 643e 3430 2e37 3634 3639 3539    <td>40.7646959
+0009b0f0: 3238 3332 3534 202d 3733 2e38 3835 3139  283254 -73.88519
+0009b100: 3734 3936 3434 3134 3c2f 7464 3e0a 2020  74964414</td>.  
+0009b110: 2020 2020 3c74 643e 3230 3132 2d31 312d      <td>2012-11-
+0009b120: 3135 2031 373a 3439 3a30 313c 2f74 643e  15 17:49:01</td>
+0009b130: 0a20 2020 2020 203c 7464 3e31 3036 393c  .      <td>1069<
+0009b140: 2f74 643e 0a20 2020 2020 203c 7464 3e36  /td>.      <td>6
+0009b150: 2e36 3c2f 7464 3e0a 2020 2020 2020 3c74  .6</td>.      <t
+0009b160: 643e 333c 2f74 643e 0a20 2020 2020 203c  d>3</td>.      <
+0009b170: 7464 3e43 6c65 6172 3c2f 7464 3e0a 2020  td>Clear</td>.  
+0009b180: 2020 2020 3c74 643e 5468 7572 7364 6179      <td>Thursday
+0009b190: 3c2f 7464 3e0a 2020 2020 2020 3c74 643e  </td>.      <td>
+0009b1a0: 466f 6f64 3c2f 7464 3e0a 2020 2020 2020  Food</td>.      
+0009b1b0: 3c74 643e 4672 6965 6420 4368 6963 6b65  <td>Fried Chicke
+0009b1c0: 6e20 4a6f 696e 743c 2f74 643e 0a20 2020  n Joint</td>.   
+0009b1d0: 203c 2f74 723e 0a20 2020 203c 7472 3e0a   </tr>.    <tr>.
+0009b1e0: 2020 2020 2020 3c74 683e 343c 2f74 683e        <th>4</th>
+0009b1f0: 0a20 2020 2020 203c 7464 3e31 3236 3c2f  .      <td>126</
+0009b200: 7464 3e0a 2020 2020 2020 3c74 643e 3430  td>.      <td>40
+0009b210: 2e37 3636 3037 3930 3337 3638 3234 202d  .7660790376824 -
+0009b220: 3733 2e38 3833 3532 3837 3039 3431 3136  73.8835287094116
+0009b230: 3c2f 7464 3e0a 2020 2020 2020 3c74 643e  </td>.      <td>
+0009b240: 3230 3132 2d31 312d 3135 2031 383a 3430  2012-11-15 18:40
+0009b250: 3a31 363c 2f74 643e 0a20 2020 2020 203c  :16</td>.      <
+0009b260: 7464 3e31 3132 303c 2f74 643e 0a20 2020  td>1120</td>.   
+0009b270: 2020 203c 7464 3e2d 312e 303c 2f74 643e     <td>-1.0</td>
+0009b280: 0a20 2020 2020 203c 7464 3e2d 313c 2f74  .      <td>-1</t
+0009b290: 643e 0a20 2020 2020 203c 7464 3e43 6c65  d>.      <td>Cle
+0009b2a0: 6172 3c2f 7464 3e0a 2020 2020 2020 3c74  ar</td>.      <t
+0009b2b0: 643e 5468 7572 7364 6179 3c2f 7464 3e0a  d>Thursday</td>.
+0009b2c0: 2020 2020 2020 3c74 643e 5472 6176 656c        <td>Travel
+0009b2d0: 2026 616d 703b 2054 7261 6e73 706f 7274   &amp; Transport
+0009b2e0: 3c2f 7464 3e0a 2020 2020 2020 3c74 643e  </td>.      <td>
+0009b2f0: 4275 7320 5374 6174 696f 6e3c 2f74 643e  Bus Station</td>
+0009b300: 0a20 2020 203c 2f74 723e 0a20 203c 2f74  .    </tr>.  </t
+0009b310: 626f 6479 3e0a 3c2f 7461 626c 653e 0a3c  body>.</table>.<
+0009b320: 2f64 6976 3e0a 3c2f 6469 763e 0a0a 3c2f  /div>.</div>..</
+0009b330: 6469 763e 0a0a 3c2f 6469 763e 0a0a 3c2f  div>..</div>..</
+0009b340: 6469 763e 0a0a 3c2f 6469 763e 3c64 6976  div>..</div><div
+0009b350: 2063 6c61 7373 3d22 6a70 2d43 656c 6c20   class="jp-Cell 
+0009b360: 6a70 2d43 6f64 6543 656c 6c20 6a70 2d4e  jp-CodeCell jp-N
+0009b370: 6f74 6562 6f6f 6b2d 6365 6c6c 2020 2022  otebook-cell   "
+0009b380: 3e0a 3c64 6976 2063 6c61 7373 3d22 6a70  >.<div class="jp
+0009b390: 2d43 656c 6c2d 696e 7075 7457 7261 7070  -Cell-inputWrapp
+0009b3a0: 6572 223e 0a3c 6469 7620 636c 6173 733d  er">.<div class=
+0009b3b0: 226a 702d 436f 6c6c 6170 7365 7220 6a70  "jp-Collapser jp
+0009b3c0: 2d49 6e70 7574 436f 6c6c 6170 7365 7220  -InputCollapser 
+0009b3d0: 6a70 2d43 656c 6c2d 696e 7075 7443 6f6c  jp-Cell-inputCol
+0009b3e0: 6c61 7073 6572 223e 0a3c 2f64 6976 3e0a  lapser">.</div>.
+0009b3f0: 3c64 6976 2063 6c61 7373 3d22 6a70 2d49  <div class="jp-I
+0009b400: 6e70 7574 4172 6561 206a 702d 4365 6c6c  nputArea jp-Cell
+0009b410: 2d69 6e70 7574 4172 6561 223e 0a3c 6469  -inputArea">.<di
+0009b420: 7620 636c 6173 733d 226a 702d 496e 7075  v class="jp-Inpu
+0009b430: 7450 726f 6d70 7420 6a70 2d49 6e70 7574  tPrompt jp-Input
+0009b440: 4172 6561 2d70 726f 6d70 7422 3e49 6e26  Area-prompt">In&
+0009b450: 6e62 7370 3b5b 3231 5d3a 3c2f 6469 763e  nbsp;[21]:</div>
+0009b460: 0a3c 6469 7620 636c 6173 733d 226a 702d  .<div class="jp-
+0009b470: 436f 6465 4d69 7272 6f72 4564 6974 6f72  CodeMirrorEditor
+0009b480: 206a 702d 4564 6974 6f72 206a 702d 496e   jp-Editor jp-In
+0009b490: 7075 7441 7265 612d 6564 6974 6f72 2220  putArea-editor" 
+0009b4a0: 6461 7461 2d74 7970 653d 2269 6e6c 696e  data-type="inlin
+0009b4b0: 6522 3e0a 2020 2020 203c 6469 7620 636c  e">.     <div cl
+0009b4c0: 6173 733d 2243 6f64 654d 6972 726f 7220  ass="CodeMirror 
+0009b4d0: 636d 2d73 2d6a 7570 7974 6572 223e 0a3c  cm-s-jupyter">.<
+0009b4e0: 6469 7620 636c 6173 733d 2220 6869 6768  div class=" high
+0009b4f0: 6c69 6768 7420 686c 2d69 7079 7468 6f6e  light hl-ipython
+0009b500: 3322 3e3c 7072 653e 3c73 7061 6e3e 3c2f  3"><pre><span></
+0009b510: 7370 616e 3e3c 7370 616e 2063 6c61 7373  span><span class
+0009b520: 3d22 6e22 3e64 663c 2f73 7061 6e3e 3c73  ="n">df</span><s
+0009b530: 7061 6e20 636c 6173 733d 2270 223e 2c3c  pan class="p">,<
+0009b540: 2f73 7061 6e3e 203c 7370 616e 2063 6c61  /span> <span cla
+0009b550: 7373 3d22 6e22 3e73 7061 6365 5f63 6f6c  ss="n">space_col
+0009b560: 733c 2f73 7061 6e3e 3c73 7061 6e20 636c  s</span><span cl
+0009b570: 6173 733d 2270 223e 2c3c 2f73 7061 6e3e  ass="p">,</span>
+0009b580: 203c 7370 616e 2063 6c61 7373 3d22 6e22   <span class="n"
+0009b590: 3e6c 6c5f 636f 6c73 3c2f 7370 616e 3e20  >ll_cols</span> 
+0009b5a0: 3c73 7061 6e20 636c 6173 733d 226f 223e  <span class="o">
+0009b5b0: 3d3c 2f73 7061 6e3e 203c 7370 616e 2063  =</span> <span c
+0009b5c0: 6c61 7373 3d22 6e22 3e6f 7267 616e 697a  lass="n">organiz
+0009b5d0: 6546 7261 6d65 3c2f 7370 616e 3e3c 7370  eFrame</span><sp
+0009b5e0: 616e 2063 6c61 7373 3d22 7022 3e28 3c2f  an class="p">(</
+0009b5f0: 7370 616e 3e3c 7370 616e 2063 6c61 7373  span><span class
+0009b600: 3d22 6e22 3e64 663c 2f73 7061 6e3e 3c73  ="n">df</span><s
+0009b610: 7061 6e20 636c 6173 733d 2270 223e 2c3c  pan class="p">,<
+0009b620: 2f73 7061 6e3e 203c 7370 616e 2063 6c61  /span> <span cla
+0009b630: 7373 3d22 6e22 3e6d 616b 655f 7370 6174  ss="n">make_spat
+0009b640: 6961 6c73 3c2f 7370 616e 3e3c 7370 616e  ials</span><span
+0009b650: 2063 6c61 7373 3d22 6f22 3e3d 3c2f 7370   class="o">=</sp
+0009b660: 616e 3e3c 7370 616e 2063 6c61 7373 3d22  an><span class="
+0009b670: 6b63 223e 5472 7565 3c2f 7370 616e 3e3c  kc">True</span><
+0009b680: 7370 616e 2063 6c61 7373 3d22 7022 3e29  span class="p">)
+0009b690: 3c2f 7370 616e 3e0a 0a3c 7370 616e 2063  </span>..<span c
+0009b6a0: 6c61 7373 3d22 6e62 223e 7072 696e 743c  lass="nb">print<
+0009b6b0: 2f73 7061 6e3e 3c73 7061 6e20 636c 6173  /span><span clas
+0009b6c0: 733d 2270 223e 283c 2f73 7061 6e3e 3c73  s="p">(</span><s
+0009b6d0: 7061 6e20 636c 6173 733d 2273 3122 3e26  pan class="s1">&
+0009b6e0: 2333 393b 436f 6c75 6d6e 7320 7769 7468  #39;Columns with
+0009b6f0: 2073 7061 6365 3a20 2623 3339 3b3c 2f73   space: &#39;</s
+0009b700: 7061 6e3e 3c73 7061 6e20 636c 6173 733d  pan><span class=
+0009b710: 2270 223e 2c3c 2f73 7061 6e3e 203c 7370  "p">,</span> <sp
+0009b720: 616e 2063 6c61 7373 3d22 6e22 3e73 7061  an class="n">spa
+0009b730: 6365 5f63 6f6c 733c 2f73 7061 6e3e 3c73  ce_cols</span><s
+0009b740: 7061 6e20 636c 6173 733d 2270 223e 293c  pan class="p">)<
+0009b750: 2f73 7061 6e3e 0a3c 7370 616e 2063 6c61  /span>.<span cla
+0009b760: 7373 3d22 6e62 223e 7072 696e 743c 2f73  ss="nb">print</s
+0009b770: 7061 6e3e 3c73 7061 6e20 636c 6173 733d  pan><span class=
+0009b780: 2270 223e 283c 2f73 7061 6e3e 3c73 7061  "p">(</span><spa
+0009b790: 6e20 636c 6173 733d 2273 3122 3e26 2333  n class="s1">&#3
+0009b7a0: 393b 436f 6c75 6d6e 7320 7769 7468 206c  9;Columns with l
+0009b7b0: 6174 2f6c 6f6e 3a20 2623 3339 3b3c 2f73  at/lon: &#39;</s
+0009b7c0: 7061 6e3e 3c73 7061 6e20 636c 6173 733d  pan><span class=
+0009b7d0: 2270 223e 2c3c 2f73 7061 6e3e 203c 7370  "p">,</span> <sp
+0009b7e0: 616e 2063 6c61 7373 3d22 6e22 3e6c 6c5f  an class="n">ll_
+0009b7f0: 636f 6c73 3c2f 7370 616e 3e3c 7370 616e  cols</span><span
+0009b800: 2063 6c61 7373 3d22 7022 3e29 3c2f 7370   class="p">)</sp
+0009b810: 616e 3e0a 3c73 7061 6e20 636c 6173 733d  an>.<span class=
+0009b820: 226e 223e 6466 3c2f 7370 616e 3e3c 7370  "n">df</span><sp
+0009b830: 616e 2063 6c61 7373 3d22 6f22 3e2e 3c2f  an class="o">.</
+0009b840: 7370 616e 3e3c 7370 616e 2063 6c61 7373  span><span class
+0009b850: 3d22 6e22 3e68 6561 643c 2f73 7061 6e3e  ="n">head</span>
+0009b860: 3c73 7061 6e20 636c 6173 733d 2270 223e  <span class="p">
+0009b870: 2829 3c2f 7370 616e 3e0a 3c2f 7072 653e  ()</span>.</pre>
+0009b880: 3c2f 6469 763e 0a0a 2020 2020 203c 2f64  </div>..     </d
+0009b890: 6976 3e0a 3c2f 6469 763e 0a3c 2f64 6976  iv>.</div>.</div
+0009b8a0: 3e0a 3c2f 6469 763e 0a0a 3c64 6976 2063  >.</div>..<div c
+0009b8b0: 6c61 7373 3d22 6a70 2d43 656c 6c2d 6f75  lass="jp-Cell-ou
+0009b8c0: 7470 7574 5772 6170 7065 7222 3e0a 3c64  tputWrapper">.<d
+0009b8d0: 6976 2063 6c61 7373 3d22 6a70 2d43 6f6c  iv class="jp-Col
+0009b8e0: 6c61 7073 6572 206a 702d 4f75 7470 7574  lapser jp-Output
+0009b8f0: 436f 6c6c 6170 7365 7220 6a70 2d43 656c  Collapser jp-Cel
+0009b900: 6c2d 6f75 7470 7574 436f 6c6c 6170 7365  l-outputCollapse
+0009b910: 7222 3e0a 3c2f 6469 763e 0a0a 0a3c 6469  r">.</div>...<di
+0009b920: 7620 636c 6173 733d 226a 702d 4f75 7470  v class="jp-Outp
+0009b930: 7574 4172 6561 206a 702d 4365 6c6c 2d6f  utArea jp-Cell-o
+0009b940: 7574 7075 7441 7265 6122 3e0a 0a3c 6469  utputArea">..<di
+0009b950: 7620 636c 6173 733d 226a 702d 4f75 7470  v class="jp-Outp
+0009b960: 7574 4172 6561 2d63 6869 6c64 223e 0a0a  utArea-child">..
+0009b970: 2020 2020 0a20 2020 203c 6469 7620 636c      .    <div cl
+0009b980: 6173 733d 226a 702d 4f75 7470 7574 5072  ass="jp-OutputPr
+0009b990: 6f6d 7074 206a 702d 4f75 7470 7574 4172  ompt jp-OutputAr
+0009b9a0: 6561 2d70 726f 6d70 7422 3e3c 2f64 6976  ea-prompt"></div
+0009b9b0: 3e0a 0a0a 3c64 6976 2063 6c61 7373 3d22  >...<div class="
+0009b9c0: 6a70 2d52 656e 6465 7265 6454 6578 7420  jp-RenderedText 
+0009b9d0: 6a70 2d4f 7574 7075 7441 7265 612d 6f75  jp-OutputArea-ou
+0009b9e0: 7470 7574 2220 6461 7461 2d6d 696d 652d  tput" data-mime-
+0009b9f0: 7479 7065 3d22 7465 7874 2f70 6c61 696e  type="text/plain
+0009ba00: 223e 0a3c 7072 653e 436f 6c75 6d6e 7320  ">.<pre>Columns 
+0009ba10: 7769 7468 2073 7061 6365 3a20 205b 2623  with space:  [&#
+0009ba20: 3339 3b73 7061 6365 2623 3339 3b2c 2026  39;space&#39;, &
+0009ba30: 2333 393b 6461 7465 5f74 696d 6526 2333  #39;date_time&#3
+0009ba40: 393b 2c20 2623 3339 3b74 696d 6526 2333  9;, &#39;time&#3
+0009ba50: 393b 2c20 2623 3339 3b72 6174 696e 6726  9;, &#39;rating&
+0009ba60: 2333 393b 2c20 2623 3339 3b70 7269 6365  #39;, &#39;price
+0009ba70: 2623 3339 3b2c 2026 2333 393b 7765 6174  &#39;, &#39;weat
+0009ba80: 6865 7226 2333 393b 2c20 2623 3339 3b64  her&#39;, &#39;d
+0009ba90: 6179 2623 3339 3b2c 2026 2333 393b 726f  ay&#39;, &#39;ro
+0009baa0: 6f74 5f74 7970 6526 2333 393b 2c20 2623  ot_type&#39;, &#
+0009bab0: 3339 3b74 7970 6526 2333 393b 2c20 2623  39;type&#39;, &#
+0009bac0: 3339 3b74 6964 2623 3339 3b5d 0a43 6f6c  39;tid&#39;].Col
+0009bad0: 756d 6e73 2077 6974 6820 6c61 742f 6c6f  umns with lat/lo
+0009bae0: 6e3a 2020 5b26 2333 393b 6461 7465 5f74  n:  [&#39;date_t
+0009baf0: 696d 6526 2333 393b 2c20 2623 3339 3b74  ime&#39;, &#39;t
+0009bb00: 696d 6526 2333 393b 2c20 2623 3339 3b72  ime&#39;, &#39;r
+0009bb10: 6174 696e 6726 2333 393b 2c20 2623 3339  ating&#39;, &#39
+0009bb20: 3b70 7269 6365 2623 3339 3b2c 2026 2333  ;price&#39;, &#3
+0009bb30: 393b 7765 6174 6865 7226 2333 393b 2c20  9;weather&#39;, 
+0009bb40: 2623 3339 3b64 6179 2623 3339 3b2c 2026  &#39;day&#39;, &
+0009bb50: 2333 393b 726f 6f74 5f74 7970 6526 2333  #39;root_type&#3
+0009bb60: 393b 2c20 2623 3339 3b74 7970 6526 2333  9;, &#39;type&#3
+0009bb70: 393b 2c20 2623 3339 3b6c 6174 2623 3339  9;, &#39;lat&#39
+0009bb80: 3b2c 2026 2333 393b 6c6f 6e26 2333 393b  ;, &#39;lon&#39;
+0009bb90: 2c20 2623 3339 3b74 6964 2623 3339 3b5d  , &#39;tid&#39;]
+0009bba0: 0a3c 2f70 7265 3e0a 3c2f 6469 763e 0a3c  .</pre>.</div>.<
+0009bbb0: 2f64 6976 3e0a 0a3c 6469 7620 636c 6173  /div>..<div clas
+0009bbc0: 733d 226a 702d 4f75 7470 7574 4172 6561  s="jp-OutputArea
+0009bbd0: 2d63 6869 6c64 223e 0a0a 2020 2020 0a20  -child">..    . 
+0009bbe0: 2020 203c 6469 7620 636c 6173 733d 226a     <div class="j
+0009bbf0: 702d 4f75 7470 7574 5072 6f6d 7074 206a  p-OutputPrompt j
+0009bc00: 702d 4f75 7470 7574 4172 6561 2d70 726f  p-OutputArea-pro
+0009bc10: 6d70 7422 3e4f 7574 5b32 315d 3a3c 2f64  mpt">Out[21]:</d
+0009bc20: 6976 3e0a 0a0a 0a3c 6469 7620 636c 6173  iv>....<div clas
+0009bc30: 733d 226a 702d 5265 6e64 6572 6564 4854  s="jp-RenderedHT
+0009bc40: 4d4c 436f 6d6d 6f6e 206a 702d 5265 6e64  MLCommon jp-Rend
+0009bc50: 6572 6564 4854 4d4c 206a 702d 4f75 7470  eredHTML jp-Outp
+0009bc60: 7574 4172 6561 2d6f 7574 7075 7420 6a70  utArea-output jp
+0009bc70: 2d4f 7574 7075 7441 7265 612d 6578 6563  -OutputArea-exec
+0009bc80: 7574 6552 6573 756c 7422 2064 6174 612d  uteResult" data-
+0009bc90: 6d69 6d65 2d74 7970 653d 2274 6578 742f  mime-type="text/
+0009bca0: 6874 6d6c 223e 0a3c 6469 763e 0a3c 7374  html">.<div>.<st
+0009bcb0: 796c 6520 7363 6f70 6564 3e0a 2020 2020  yle scoped>.    
+0009bcc0: 2e64 6174 6166 7261 6d65 2074 626f 6479  .dataframe tbody
+0009bcd0: 2074 7220 7468 3a6f 6e6c 792d 6f66 2d74   tr th:only-of-t
+0009bce0: 7970 6520 7b0a 2020 2020 2020 2020 7665  ype {.        ve
+0009bcf0: 7274 6963 616c 2d61 6c69 676e 3a20 6d69  rtical-align: mi
+0009bd00: 6464 6c65 3b0a 2020 2020 7d0a 0a20 2020  ddle;.    }..   
+0009bd10: 202e 6461 7461 6672 616d 6520 7462 6f64   .dataframe tbod
+0009bd20: 7920 7472 2074 6820 7b0a 2020 2020 2020  y tr th {.      
+0009bd30: 2020 7665 7274 6963 616c 2d61 6c69 676e    vertical-align
+0009bd40: 3a20 746f 703b 0a20 2020 207d 0a0a 2020  : top;.    }..  
+0009bd50: 2020 2e64 6174 6166 7261 6d65 2074 6865    .dataframe the
+0009bd60: 6164 2074 6820 7b0a 2020 2020 2020 2020  ad th {.        
+0009bd70: 7465 7874 2d61 6c69 676e 3a20 7269 6768  text-align: righ
+0009bd80: 743b 0a20 2020 207d 0a3c 2f73 7479 6c65  t;.    }.</style
+0009bd90: 3e0a 3c74 6162 6c65 2062 6f72 6465 723d  >.<table border=
+0009bda0: 2231 2220 636c 6173 733d 2264 6174 6166  "1" class="dataf
+0009bdb0: 7261 6d65 223e 0a20 203c 7468 6561 643e  rame">.  <thead>
+0009bdc0: 0a20 2020 203c 7472 2073 7479 6c65 3d22  .    <tr style="
+0009bdd0: 7465 7874 2d61 6c69 676e 3a20 7269 6768  text-align: righ
+0009bde0: 743b 223e 0a20 2020 2020 203c 7468 3e3c  t;">.      <th><
+0009bdf0: 2f74 683e 0a20 2020 2020 203c 7468 3e74  /th>.      <th>t
+0009be00: 6964 3c2f 7468 3e0a 2020 2020 2020 3c74  id</th>.      <t
+0009be10: 683e 7370 6163 653c 2f74 683e 0a20 2020  h>space</th>.   
+0009be20: 2020 203c 7468 3e64 6174 655f 7469 6d65     <th>date_time
+0009be30: 3c2f 7468 3e0a 2020 2020 2020 3c74 683e  </th>.      <th>
+0009be40: 7469 6d65 3c2f 7468 3e0a 2020 2020 2020  time</th>.      
+0009be50: 3c74 683e 7261 7469 6e67 3c2f 7468 3e0a  <th>rating</th>.
+0009be60: 2020 2020 2020 3c74 683e 7072 6963 653c        <th>price<
+0009be70: 2f74 683e 0a20 2020 2020 203c 7468 3e77  /th>.      <th>w
+0009be80: 6561 7468 6572 3c2f 7468 3e0a 2020 2020  eather</th>.    
+0009be90: 2020 3c74 683e 6461 793c 2f74 683e 0a20    <th>day</th>. 
+0009bea0: 2020 2020 203c 7468 3e72 6f6f 745f 7479       <th>root_ty
+0009beb0: 7065 3c2f 7468 3e0a 2020 2020 2020 3c74  pe</th>.      <t
+0009bec0: 683e 7479 7065 3c2f 7468 3e0a 2020 2020  h>type</th>.    
+0009bed0: 2020 3c74 683e 6c61 743c 2f74 683e 0a20    <th>lat</th>. 
+0009bee0: 2020 2020 203c 7468 3e6c 6f6e 3c2f 7468       <th>lon</th
+0009bef0: 3e0a 2020 2020 3c2f 7472 3e0a 2020 3c2f  >.    </tr>.  </
+0009bf00: 7468 6561 643e 0a20 203c 7462 6f64 793e  thead>.  <tbody>
+0009bf10: 0a20 2020 203c 7472 3e0a 2020 2020 2020  .    <tr>.      
+0009bf20: 3c74 683e 303c 2f74 683e 0a20 2020 2020  <th>0</th>.     
+0009bf30: 203c 7464 3e31 3236 3c2f 7464 3e0a 2020   <td>126</td>.  
+0009bf40: 2020 2020 3c74 643e 3430 2e38 3333 3136      <td>40.83316
+0009bf50: 3532 3030 3632 3234 202d 3733 2e39 3431  52006224 -73.941
+0009bf60: 3836 3033 3432 3736 3932 3c2f 7464 3e0a  8603427692</td>.
+0009bf70: 2020 2020 2020 3c74 643e 3230 3132 2d31        <td>2012-1
+0009bf80: 312d 3132 2030 353a 3137 3a31 383c 2f74  1-12 05:17:18</t
+0009bf90: 643e 0a20 2020 2020 203c 7464 3e33 3137  d>.      <td>317
+0009bfa0: 3c2f 7464 3e0a 2020 2020 2020 3c74 643e  </td>.      <td>
+0009bfb0: 2d31 2e30 3c2f 7464 3e0a 2020 2020 2020  -1.0</td>.      
+0009bfc0: 3c74 643e 2d31 3c2f 7464 3e0a 2020 2020  <td>-1</td>.    
+0009bfd0: 2020 3c74 643e 436c 6561 723c 2f74 643e    <td>Clear</td>
+0009bfe0: 0a20 2020 2020 203c 7464 3e4d 6f6e 6461  .      <td>Monda
+0009bff0: 793c 2f74 643e 0a20 2020 2020 203c 7464  y</td>.      <td
+0009c000: 3e52 6573 6964 656e 6365 3c2f 7464 3e0a  >Residence</td>.
+0009c010: 2020 2020 2020 3c74 643e 486f 6d65 2028        <td>Home (
+0009c020: 7072 6976 6174 6529 3c2f 7464 3e0a 2020  private)</td>.  
+0009c030: 2020 2020 3c74 643e 3430 2e38 3333 3136      <td>40.83316
+0009c040: 353c 2f74 643e 0a20 2020 2020 203c 7464  5</td>.      <td
+0009c050: 3e2d 3733 2e39 3431 3836 303c 2f74 643e  >-73.941860</td>
+0009c060: 0a20 2020 203c 2f74 723e 0a20 2020 203c  .    </tr>.    <
+0009c070: 7472 3e0a 2020 2020 2020 3c74 683e 313c  tr>.      <th>1<
+0009c080: 2f74 683e 0a20 2020 2020 203c 7464 3e31  /th>.      <td>1
+0009c090: 3236 3c2f 7464 3e0a 2020 2020 2020 3c74  26</td>.      <t
+0009c0a0: 643e 3430 2e38 3334 3039 3738 3034 3130  d>40.83409780410
+0009c0b0: 3732 202d 3733 2e39 3435 3236 3732 3232  72 -73.945267222
+0009c0c0: 3538 3831 3c2f 7464 3e0a 2020 2020 2020  5881</td>.      
+0009c0d0: 3c74 643e 3230 3132 2d31 312d 3132 2032  <td>2012-11-12 2
+0009c0e0: 333a 3234 3a35 353c 2f74 643e 0a20 2020  3:24:55</td>.   
+0009c0f0: 2020 203c 7464 3e31 3430 343c 2f74 643e     <td>1404</td>
+0009c100: 0a20 2020 2020 203c 7464 3e38 2e32 3c2f  .      <td>8.2</
+0009c110: 7464 3e0a 2020 2020 2020 3c74 643e 313c  td>.      <td>1<
+0009c120: 2f74 643e 0a20 2020 2020 203c 7464 3e43  /td>.      <td>C
+0009c130: 6c6f 7564 733c 2f74 643e 0a20 2020 2020  louds</td>.     
+0009c140: 203c 7464 3e4d 6f6e 6461 793c 2f74 643e   <td>Monday</td>
+0009c150: 0a20 2020 2020 203c 7464 3e46 6f6f 643c  .      <td>Food<
+0009c160: 2f74 643e 0a20 2020 2020 203c 7464 3e44  /td>.      <td>D
+0009c170: 656c 6920 2f20 426f 6465 6761 3c2f 7464  eli / Bodega</td
+0009c180: 3e0a 2020 2020 2020 3c74 643e 3430 2e38  >.      <td>40.8
+0009c190: 3334 3039 383c 2f74 643e 0a20 2020 2020  34098</td>.     
+0009c1a0: 203c 7464 3e2d 3733 2e39 3435 3236 373c   <td>-73.945267<
+0009c1b0: 2f74 643e 0a20 2020 203c 2f74 723e 0a20  /td>.    </tr>. 
+0009c1c0: 2020 203c 7472 3e0a 2020 2020 2020 3c74     <tr>.      <t
+0009c1d0: 683e 323c 2f74 683e 0a20 2020 2020 203c  h>2</th>.      <
+0009c1e0: 7464 3e31 3236 3c2f 7464 3e0a 2020 2020  td>126</td>.    
+0009c1f0: 2020 3c74 643e 3430 2e38 3333 3136 3532    <td>40.8331652
+0009c200: 3030 3632 3234 202d 3733 2e39 3431 3836  006224 -73.94186
+0009c210: 3033 3432 3736 3932 3c2f 7464 3e0a 2020  03427692</td>.  
+0009c220: 2020 2020 3c74 643e 3230 3132 2d31 312d      <td>2012-11-
+0009c230: 3133 2030 303a 3030 3a30 373c 2f74 643e  13 00:00:07</td>
+0009c240: 0a20 2020 2020 203c 7464 3e30 3c2f 7464  .      <td>0</td
+0009c250: 3e0a 2020 2020 2020 3c74 643e 2d31 2e30  >.      <td>-1.0
+0009c260: 3c2f 7464 3e0a 2020 2020 2020 3c74 643e  </td>.      <td>
+0009c270: 2d31 3c2f 7464 3e0a 2020 2020 2020 3c74  -1</td>.      <t
+0009c280: 643e 436c 6f75 6473 3c2f 7464 3e0a 2020  d>Clouds</td>.  
+0009c290: 2020 2020 3c74 643e 5475 6573 6461 793c      <td>Tuesday<
+0009c2a0: 2f74 643e 0a20 2020 2020 203c 7464 3e52  /td>.      <td>R
+0009c2b0: 6573 6964 656e 6365 3c2f 7464 3e0a 2020  esidence</td>.  
+0009c2c0: 2020 2020 3c74 643e 486f 6d65 2028 7072      <td>Home (pr
+0009c2d0: 6976 6174 6529 3c2f 7464 3e0a 2020 2020  ivate)</td>.    
+0009c2e0: 2020 3c74 643e 3430 2e38 3333 3136 353c    <td>40.833165<
+0009c2f0: 2f74 643e 0a20 2020 2020 203c 7464 3e2d  /td>.      <td>-
+0009c300: 3733 2e39 3431 3836 303c 2f74 643e 0a20  73.941860</td>. 
+0009c310: 2020 203c 2f74 723e 0a20 2020 203c 7472     </tr>.    <tr
+0009c320: 3e0a 2020 2020 2020 3c74 683e 333c 2f74  >.      <th>3</t
+0009c330: 683e 0a20 2020 2020 203c 7464 3e31 3236  h>.      <td>126
+0009c340: 3c2f 7464 3e0a 2020 2020 2020 3c74 643e  </td>.      <td>
+0009c350: 3430 2e37 3634 3639 3539 3238 3332 3534  40.7646959283254
+0009c360: 202d 3733 2e38 3835 3139 3734 3936 3434   -73.88519749644
+0009c370: 3134 3c2f 7464 3e0a 2020 2020 2020 3c74  14</td>.      <t
+0009c380: 643e 3230 3132 2d31 312d 3135 2031 373a  d>2012-11-15 17:
+0009c390: 3439 3a30 313c 2f74 643e 0a20 2020 2020  49:01</td>.     
+0009c3a0: 203c 7464 3e31 3036 393c 2f74 643e 0a20   <td>1069</td>. 
+0009c3b0: 2020 2020 203c 7464 3e36 2e36 3c2f 7464       <td>6.6</td
+0009c3c0: 3e0a 2020 2020 2020 3c74 643e 333c 2f74  >.      <td>3</t
+0009c3d0: 643e 0a20 2020 2020 203c 7464 3e43 6c65  d>.      <td>Cle
+0009c3e0: 6172 3c2f 7464 3e0a 2020 2020 2020 3c74  ar</td>.      <t
+0009c3f0: 643e 5468 7572 7364 6179 3c2f 7464 3e0a  d>Thursday</td>.
+0009c400: 2020 2020 2020 3c74 643e 466f 6f64 3c2f        <td>Food</
+0009c410: 7464 3e0a 2020 2020 2020 3c74 643e 4672  td>.      <td>Fr
+0009c420: 6965 6420 4368 6963 6b65 6e20 4a6f 696e  ied Chicken Join
+0009c430: 743c 2f74 643e 0a20 2020 2020 203c 7464  t</td>.      <td
+0009c440: 3e34 302e 3736 3436 3936 3c2f 7464 3e0a  >40.764696</td>.
+0009c450: 2020 2020 2020 3c74 643e 2d37 332e 3838        <td>-73.88
+0009c460: 3531 3937 3c2f 7464 3e0a 2020 2020 3c2f  5197</td>.    </
+0009c470: 7472 3e0a 2020 2020 3c74 723e 0a20 2020  tr>.    <tr>.   
+0009c480: 2020 203c 7468 3e34 3c2f 7468 3e0a 2020     <th>4</th>.  
+0009c490: 2020 2020 3c74 643e 3132 363c 2f74 643e      <td>126</td>
+0009c4a0: 0a20 2020 2020 203c 7464 3e34 302e 3736  .      <td>40.76
+0009c4b0: 3630 3739 3033 3736 3832 3420 2d37 332e  60790376824 -73.
+0009c4c0: 3838 3335 3238 3730 3934 3131 363c 2f74  8835287094116</t
+0009c4d0: 643e 0a20 2020 2020 203c 7464 3e32 3031  d>.      <td>201
+0009c4e0: 322d 3131 2d31 3520 3138 3a34 303a 3136  2-11-15 18:40:16
+0009c4f0: 3c2f 7464 3e0a 2020 2020 2020 3c74 643e  </td>.      <td>
+0009c500: 3131 3230 3c2f 7464 3e0a 2020 2020 2020  1120</td>.      
+0009c510: 3c74 643e 2d31 2e30 3c2f 7464 3e0a 2020  <td>-1.0</td>.  
+0009c520: 2020 2020 3c74 643e 2d31 3c2f 7464 3e0a      <td>-1</td>.
+0009c530: 2020 2020 2020 3c74 643e 436c 6561 723c        <td>Clear<
+0009c540: 2f74 643e 0a20 2020 2020 203c 7464 3e54  /td>.      <td>T
+0009c550: 6875 7273 6461 793c 2f74 643e 0a20 2020  hursday</td>.   
+0009c560: 2020 203c 7464 3e54 7261 7665 6c20 2661     <td>Travel &a
+0009c570: 6d70 3b20 5472 616e 7370 6f72 743c 2f74  mp; Transport</t
+0009c580: 643e 0a20 2020 2020 203c 7464 3e42 7573  d>.      <td>Bus
+0009c590: 2053 7461 7469 6f6e 3c2f 7464 3e0a 2020   Station</td>.  
+0009c5a0: 2020 2020 3c74 643e 3430 2e37 3636 3037      <td>40.76607
+0009c5b0: 393c 2f74 643e 0a20 2020 2020 203c 7464  9</td>.      <td
+0009c5c0: 3e2d 3733 2e38 3833 3532 393c 2f74 643e  >-73.883529</td>
+0009c5d0: 0a20 2020 203c 2f74 723e 0a20 203c 2f74  .    </tr>.  </t
+0009c5e0: 626f 6479 3e0a 3c2f 7461 626c 653e 0a3c  body>.</table>.<
+0009c5f0: 2f64 6976 3e0a 3c2f 6469 763e 0a0a 3c2f  /div>.</div>..</
+0009c600: 6469 763e 0a0a 3c2f 6469 763e 0a0a 3c2f  div>..</div>..</
+0009c610: 6469 763e 0a0a 3c2f 6469 763e 0a3c 6469  div>..</div>.<di
+0009c620: 7620 636c 6173 733d 226a 702d 4365 6c6c  v class="jp-Cell
+0009c630: 206a 702d 4d61 726b 646f 776e 4365 6c6c   jp-MarkdownCell
+0009c640: 206a 702d 4e6f 7465 626f 6f6b 2d63 656c   jp-Notebook-cel
+0009c650: 6c22 3e0a 3c64 6976 2063 6c61 7373 3d22  l">.<div class="
+0009c660: 6a70 2d43 656c 6c2d 696e 7075 7457 7261  jp-Cell-inputWra
+0009c670: 7070 6572 223e 0a3c 6469 7620 636c 6173  pper">.<div clas
+0009c680: 733d 226a 702d 436f 6c6c 6170 7365 7220  s="jp-Collapser 
+0009c690: 6a70 2d49 6e70 7574 436f 6c6c 6170 7365  jp-InputCollapse
+0009c6a0: 7220 6a70 2d43 656c 6c2d 696e 7075 7443  r jp-Cell-inputC
+0009c6b0: 6f6c 6c61 7073 6572 223e 0a3c 2f64 6976  ollapser">.</div
+0009c6c0: 3e0a 3c64 6976 2063 6c61 7373 3d22 6a70  >.<div class="jp
+0009c6d0: 2d49 6e70 7574 4172 6561 206a 702d 4365  -InputArea jp-Ce
+0009c6e0: 6c6c 2d69 6e70 7574 4172 6561 223e 3c64  ll-inputArea"><d
+0009c6f0: 6976 2063 6c61 7373 3d22 6a70 2d49 6e70  iv class="jp-Inp
+0009c700: 7574 5072 6f6d 7074 206a 702d 496e 7075  utPrompt jp-Inpu
+0009c710: 7441 7265 612d 7072 6f6d 7074 223e 0a3c  tArea-prompt">.<
+0009c720: 2f64 6976 3e3c 6469 7620 636c 6173 733d  /div><div class=
+0009c730: 226a 702d 5265 6e64 6572 6564 4854 4d4c  "jp-RenderedHTML
+0009c740: 436f 6d6d 6f6e 206a 702d 5265 6e64 6572  Common jp-Render
+0009c750: 6564 4d61 726b 646f 776e 206a 702d 4d61  edMarkdown jp-Ma
+0009c760: 726b 646f 776e 4f75 7470 7574 2022 2064  rkdownOutput " d
+0009c770: 6174 612d 6d69 6d65 2d74 7970 653d 2274  ata-mime-type="t
+0009c780: 6578 742f 6d61 726b 646f 776e 223e 0a3c  ext/markdown">.<
+0009c790: 703e 3c73 7472 6f6e 673e 4e6f 7465 3a3c  p><strong>Note:<
+0009c7a0: 2f73 7472 6f6e 673e 2054 6f20 6265 7474  /strong> To bett
+0009c7b0: 6572 2073 7461 6e64 6172 642c 2077 6520  er standard, we 
+0009c7c0: 7265 636f 6d65 6e64 2066 6f72 2063 6c61  recomend for cla
+0009c7d0: 7373 6966 6963 6174 696f 6e20 7468 6520  ssification the 
+0009c7e0: 7573 6520 6f66 203c 636f 6465 3e70 7265  use of <code>pre
+0009c7f0: 7061 7265 5f64 733c 2f63 6f64 653e 2066  pare_ds</code> f
+0009c800: 756e 6374 696f 6e20 6672 6f6d 203c 636f  unction from <co
+0009c810: 6465 3e64 6174 6173 6574 3c2f 636f 6465  de>dataset</code
+0009c820: 3e20 6d6f 6475 6c65 2c20 6173 2079 6f75  > module, as you
+0009c830: 2063 616e 2069 6e64 6963 6174 6520 7468   can indicate th
+0009c840: 6520 636c 6173 7320 636f 6c75 6d6e 3a3c  e class column:<
+0009c850: 2f70 3e0a 0a3c 2f64 6976 3e0a 3c2f 6469  /p>..</div>.</di
+0009c860: 763e 0a3c 2f64 6976 3e0a 3c2f 6469 763e  v>.</div>.</div>
+0009c870: 3c64 6976 2063 6c61 7373 3d22 6a70 2d43  <div class="jp-C
+0009c880: 656c 6c20 6a70 2d43 6f64 6543 656c 6c20  ell jp-CodeCell 
+0009c890: 6a70 2d4e 6f74 6562 6f6f 6b2d 6365 6c6c  jp-Notebook-cell
+0009c8a0: 2020 2022 3e0a 3c64 6976 2063 6c61 7373     ">.<div class
+0009c8b0: 3d22 6a70 2d43 656c 6c2d 696e 7075 7457  ="jp-Cell-inputW
+0009c8c0: 7261 7070 6572 223e 0a3c 6469 7620 636c  rapper">.<div cl
+0009c8d0: 6173 733d 226a 702d 436f 6c6c 6170 7365  ass="jp-Collapse
+0009c8e0: 7220 6a70 2d49 6e70 7574 436f 6c6c 6170  r jp-InputCollap
+0009c8f0: 7365 7220 6a70 2d43 656c 6c2d 696e 7075  ser jp-Cell-inpu
+0009c900: 7443 6f6c 6c61 7073 6572 223e 0a3c 2f64  tCollapser">.</d
+0009c910: 6976 3e0a 3c64 6976 2063 6c61 7373 3d22  iv>.<div class="
+0009c920: 6a70 2d49 6e70 7574 4172 6561 206a 702d  jp-InputArea jp-
+0009c930: 4365 6c6c 2d69 6e70 7574 4172 6561 223e  Cell-inputArea">
+0009c940: 0a3c 6469 7620 636c 6173 733d 226a 702d  .<div class="jp-
+0009c950: 496e 7075 7450 726f 6d70 7420 6a70 2d49  InputPrompt jp-I
+0009c960: 6e70 7574 4172 6561 2d70 726f 6d70 7422  nputArea-prompt"
+0009c970: 3e49 6e26 6e62 7370 3b5b 3232 5d3a 3c2f  >In&nbsp;[22]:</
+0009c980: 6469 763e 0a3c 6469 7620 636c 6173 733d  div>.<div class=
+0009c990: 226a 702d 436f 6465 4d69 7272 6f72 4564  "jp-CodeMirrorEd
+0009c9a0: 6974 6f72 206a 702d 4564 6974 6f72 206a  itor jp-Editor j
+0009c9b0: 702d 496e 7075 7441 7265 612d 6564 6974  p-InputArea-edit
+0009c9c0: 6f72 2220 6461 7461 2d74 7970 653d 2269  or" data-type="i
+0009c9d0: 6e6c 696e 6522 3e0a 2020 2020 203c 6469  nline">.     <di
+0009c9e0: 7620 636c 6173 733d 2243 6f64 654d 6972  v class="CodeMir
+0009c9f0: 726f 7220 636d 2d73 2d6a 7570 7974 6572  ror cm-s-jupyter
+0009ca00: 223e 0a3c 6469 7620 636c 6173 733d 2220  ">.<div class=" 
+0009ca10: 6869 6768 6c69 6768 7420 686c 2d69 7079  highlight hl-ipy
+0009ca20: 7468 6f6e 3322 3e3c 7072 653e 3c73 7061  thon3"><pre><spa
+0009ca30: 6e3e 3c2f 7370 616e 3e3c 7370 616e 2063  n></span><span c
+0009ca40: 6c61 7373 3d22 6b6e 223e 6672 6f6d 3c2f  lass="kn">from</
+0009ca50: 7370 616e 3e20 3c73 7061 6e20 636c 6173  span> <span clas
+0009ca60: 733d 226e 6e22 3e6d 6174 6461 7461 2e64  s="nn">matdata.d
+0009ca70: 6174 6173 6574 3c2f 7370 616e 3e20 3c73  ataset</span> <s
+0009ca80: 7061 6e20 636c 6173 733d 226b 6e22 3e69  pan class="kn">i
+0009ca90: 6d70 6f72 743c 2f73 7061 6e3e 203c 7370  mport</span> <sp
+0009caa0: 616e 2063 6c61 7373 3d22 6e22 3e70 7265  an class="n">pre
+0009cab0: 7061 7265 5f64 733c 2f73 7061 6e3e 0a0a  pare_ds</span>..
+0009cac0: 3c73 7061 6e20 636c 6173 733d 226e 223e  <span class="n">
+0009cad0: 6466 3c2f 7370 616e 3e20 3c73 7061 6e20  df</span> <span 
+0009cae0: 636c 6173 733d 226f 223e 3d3c 2f73 7061  class="o">=</spa
+0009caf0: 6e3e 203c 7370 616e 2063 6c61 7373 3d22  n> <span class="
+0009cb00: 6e22 3e70 7265 7061 7265 5f64 733c 2f73  n">prepare_ds</s
+0009cb10: 7061 6e3e 3c73 7061 6e20 636c 6173 733d  pan><span class=
+0009cb20: 2270 223e 283c 2f73 7061 6e3e 3c73 7061  "p">(</span><spa
+0009cb30: 6e20 636c 6173 733d 226e 223e 6466 3c2f  n class="n">df</
+0009cb40: 7370 616e 3e3c 7370 616e 2063 6c61 7373  span><span class
+0009cb50: 3d22 7022 3e2c 3c2f 7370 616e 3e20 3c73  ="p">,</span> <s
+0009cb60: 7061 6e20 636c 6173 733d 226e 223e 636c  pan class="n">cl
+0009cb70: 6173 735f 636f 6c3c 2f73 7061 6e3e 3c73  ass_col</span><s
+0009cb80: 7061 6e20 636c 6173 733d 226f 223e 3d3c  pan class="o">=<
+0009cb90: 2f73 7061 6e3e 3c73 7061 6e20 636c 6173  /span><span clas
+0009cba0: 733d 2273 3122 3e26 2333 393b 726f 6f74  s="s1">&#39;root
+0009cbb0: 5f74 7970 6526 2333 393b 3c2f 7370 616e  _type&#39;</span
+0009cbc0: 3e3c 7370 616e 2063 6c61 7373 3d22 7022  ><span class="p"
+0009cbd0: 3e29 3c2f 7370 616e 3e20 3c73 7061 6e20  >)</span> <span 
+0009cbe0: 636c 6173 733d 2263 3122 3e23 2026 2333  class="c1"># &#3
+0009cbf0: 393b 726f 6f74 5f74 7970 6526 2333 393b  9;root_type&#39;
+0009cc00: 2069 7320 7468 656e 2072 656e 616d 6564   is then renamed
+0009cc10: 2026 2333 393b 6c61 6265 6c26 2333 393b   &#39;label&#39;
+0009cc20: 3c2f 7370 616e 3e0a 3c73 7061 6e20 636c  </span>.<span cl
+0009cc30: 6173 733d 226e 223e 6466 3c2f 7370 616e  ass="n">df</span
+0009cc40: 3e0a 3c2f 7072 653e 3c2f 6469 763e 0a0a  >.</pre></div>..
+0009cc50: 2020 2020 203c 2f64 6976 3e0a 3c2f 6469       </div>.</di
+0009cc60: 763e 0a3c 2f64 6976 3e0a 3c2f 6469 763e  v>.</div>.</div>
+0009cc70: 0a0a 3c64 6976 2063 6c61 7373 3d22 6a70  ..<div class="jp
+0009cc80: 2d43 656c 6c2d 6f75 7470 7574 5772 6170  -Cell-outputWrap
+0009cc90: 7065 7222 3e0a 3c64 6976 2063 6c61 7373  per">.<div class
+0009cca0: 3d22 6a70 2d43 6f6c 6c61 7073 6572 206a  ="jp-Collapser j
+0009ccb0: 702d 4f75 7470 7574 436f 6c6c 6170 7365  p-OutputCollapse
+0009ccc0: 7220 6a70 2d43 656c 6c2d 6f75 7470 7574  r jp-Cell-output
+0009ccd0: 436f 6c6c 6170 7365 7222 3e0a 3c2f 6469  Collapser">.</di
+0009cce0: 763e 0a0a 0a3c 6469 7620 636c 6173 733d  v>...<div class=
+0009ccf0: 226a 702d 4f75 7470 7574 4172 6561 206a  "jp-OutputArea j
+0009cd00: 702d 4365 6c6c 2d6f 7574 7075 7441 7265  p-Cell-outputAre
+0009cd10: 6122 3e0a 0a3c 6469 7620 636c 6173 733d  a">..<div class=
+0009cd20: 226a 702d 4f75 7470 7574 4172 6561 2d63  "jp-OutputArea-c
+0009cd30: 6869 6c64 223e 0a0a 2020 2020 0a20 2020  hild">..    .   
+0009cd40: 203c 6469 7620 636c 6173 733d 226a 702d   <div class="jp-
+0009cd50: 4f75 7470 7574 5072 6f6d 7074 206a 702d  OutputPrompt jp-
+0009cd60: 4f75 7470 7574 4172 6561 2d70 726f 6d70  OutputArea-promp
+0009cd70: 7422 3e4f 7574 5b32 325d 3a3c 2f64 6976  t">Out[22]:</div
+0009cd80: 3e0a 0a0a 0a3c 6469 7620 636c 6173 733d  >....<div class=
+0009cd90: 226a 702d 5265 6e64 6572 6564 4854 4d4c  "jp-RenderedHTML
+0009cda0: 436f 6d6d 6f6e 206a 702d 5265 6e64 6572  Common jp-Render
+0009cdb0: 6564 4854 4d4c 206a 702d 4f75 7470 7574  edHTML jp-Output
+0009cdc0: 4172 6561 2d6f 7574 7075 7420 6a70 2d4f  Area-output jp-O
+0009cdd0: 7574 7075 7441 7265 612d 6578 6563 7574  utputArea-execut
+0009cde0: 6552 6573 756c 7422 2064 6174 612d 6d69  eResult" data-mi
+0009cdf0: 6d65 2d74 7970 653d 2274 6578 742f 6874  me-type="text/ht
+0009ce00: 6d6c 223e 0a3c 6469 763e 0a3c 7374 796c  ml">.<div>.<styl
+0009ce10: 6520 7363 6f70 6564 3e0a 2020 2020 2e64  e scoped>.    .d
+0009ce20: 6174 6166 7261 6d65 2074 626f 6479 2074  ataframe tbody t
+0009ce30: 7220 7468 3a6f 6e6c 792d 6f66 2d74 7970  r th:only-of-typ
+0009ce40: 6520 7b0a 2020 2020 2020 2020 7665 7274  e {.        vert
+0009ce50: 6963 616c 2d61 6c69 676e 3a20 6d69 6464  ical-align: midd
+0009ce60: 6c65 3b0a 2020 2020 7d0a 0a20 2020 202e  le;.    }..    .
+0009ce70: 6461 7461 6672 616d 6520 7462 6f64 7920  dataframe tbody 
+0009ce80: 7472 2074 6820 7b0a 2020 2020 2020 2020  tr th {.        
+0009ce90: 7665 7274 6963 616c 2d61 6c69 676e 3a20  vertical-align: 
+0009cea0: 746f 703b 0a20 2020 207d 0a0a 2020 2020  top;.    }..    
+0009ceb0: 2e64 6174 6166 7261 6d65 2074 6865 6164  .dataframe thead
+0009cec0: 2074 6820 7b0a 2020 2020 2020 2020 7465   th {.        te
+0009ced0: 7874 2d61 6c69 676e 3a20 7269 6768 743b  xt-align: right;
+0009cee0: 0a20 2020 207d 0a3c 2f73 7479 6c65 3e0a  .    }.</style>.
+0009cef0: 3c74 6162 6c65 2062 6f72 6465 723d 2231  <table border="1
+0009cf00: 2220 636c 6173 733d 2264 6174 6166 7261  " class="datafra
+0009cf10: 6d65 223e 0a20 203c 7468 6561 643e 0a20  me">.  <thead>. 
+0009cf20: 2020 203c 7472 2073 7479 6c65 3d22 7465     <tr style="te
+0009cf30: 7874 2d61 6c69 676e 3a20 7269 6768 743b  xt-align: right;
+0009cf40: 223e 0a20 2020 2020 203c 7468 3e3c 2f74  ">.      <th></t
+0009cf50: 683e 0a20 2020 2020 203c 7468 3e64 6174  h>.      <th>dat
+0009cf60: 655f 7469 6d65 3c2f 7468 3e0a 2020 2020  e_time</th>.    
+0009cf70: 2020 3c74 683e 7469 6d65 3c2f 7468 3e0a    <th>time</th>.
+0009cf80: 2020 2020 2020 3c74 683e 7261 7469 6e67        <th>rating
+0009cf90: 3c2f 7468 3e0a 2020 2020 2020 3c74 683e  </th>.      <th>
+0009cfa0: 7072 6963 653c 2f74 683e 0a20 2020 2020  price</th>.     
+0009cfb0: 203c 7468 3e77 6561 7468 6572 3c2f 7468   <th>weather</th
+0009cfc0: 3e0a 2020 2020 2020 3c74 683e 6461 793c  >.      <th>day<
+0009cfd0: 2f74 683e 0a20 2020 2020 203c 7468 3e74  /th>.      <th>t
+0009cfe0: 7970 653c 2f74 683e 0a20 2020 2020 203c  ype</th>.      <
+0009cff0: 7468 3e6c 6174 3c2f 7468 3e0a 2020 2020  th>lat</th>.    
+0009d000: 2020 3c74 683e 6c6f 6e3c 2f74 683e 0a20    <th>lon</th>. 
+0009d010: 2020 2020 203c 7468 3e74 6964 3c2f 7468       <th>tid</th
+0009d020: 3e0a 2020 2020 2020 3c74 683e 6c61 6265  >.      <th>labe
+0009d030: 6c3c 2f74 683e 0a20 2020 203c 2f74 723e  l</th>.    </tr>
+0009d040: 0a20 203c 2f74 6865 6164 3e0a 2020 3c74  .  </thead>.  <t
+0009d050: 626f 6479 3e0a 2020 2020 3c74 723e 0a20  body>.    <tr>. 
+0009d060: 2020 2020 203c 7468 3e30 3c2f 7468 3e0a       <th>0</th>.
+0009d070: 2020 2020 2020 3c74 643e 3230 3132 2d31        <td>2012-1
+0009d080: 312d 3132 2030 353a 3137 3a31 383c 2f74  1-12 05:17:18</t
+0009d090: 643e 0a20 2020 2020 203c 7464 3e33 3137  d>.      <td>317
+0009d0a0: 3c2f 7464 3e0a 2020 2020 2020 3c74 643e  </td>.      <td>
+0009d0b0: 2d31 2e30 3c2f 7464 3e0a 2020 2020 2020  -1.0</td>.      
+0009d0c0: 3c74 643e 2d31 3c2f 7464 3e0a 2020 2020  <td>-1</td>.    
+0009d0d0: 2020 3c74 643e 436c 6561 723c 2f74 643e    <td>Clear</td>
+0009d0e0: 0a20 2020 2020 203c 7464 3e4d 6f6e 6461  .      <td>Monda
+0009d0f0: 793c 2f74 643e 0a20 2020 2020 203c 7464  y</td>.      <td
+0009d100: 3e48 6f6d 6520 2870 7269 7661 7465 293c  >Home (private)<
+0009d110: 2f74 643e 0a20 2020 2020 203c 7464 3e34  /td>.      <td>4
+0009d120: 302e 3833 3331 3635 3c2f 7464 3e0a 2020  0.833165</td>.  
+0009d130: 2020 2020 3c74 643e 2d37 332e 3934 3138      <td>-73.9418
+0009d140: 3630 3c2f 7464 3e0a 2020 2020 2020 3c74  60</td>.      <t
+0009d150: 643e 3132 363c 2f74 643e 0a20 2020 2020  d>126</td>.     
+0009d160: 203c 7464 3e52 6573 6964 656e 6365 3c2f   <td>Residence</
+0009d170: 7464 3e0a 2020 2020 3c2f 7472 3e0a 2020  td>.    </tr>.  
+0009d180: 2020 3c74 723e 0a20 2020 2020 203c 7468    <tr>.      <th
+0009d190: 3e31 3c2f 7468 3e0a 2020 2020 2020 3c74  >1</th>.      <t
+0009d1a0: 643e 3230 3132 2d31 312d 3132 2032 333a  d>2012-11-12 23:
+0009d1b0: 3234 3a35 353c 2f74 643e 0a20 2020 2020  24:55</td>.     
+0009d1c0: 203c 7464 3e31 3430 343c 2f74 643e 0a20   <td>1404</td>. 
+0009d1d0: 2020 2020 203c 7464 3e38 2e32 3c2f 7464       <td>8.2</td
+0009d1e0: 3e0a 2020 2020 2020 3c74 643e 313c 2f74  >.      <td>1</t
+0009d1f0: 643e 0a20 2020 2020 203c 7464 3e43 6c6f  d>.      <td>Clo
+0009d200: 7564 733c 2f74 643e 0a20 2020 2020 203c  uds</td>.      <
+0009d210: 7464 3e4d 6f6e 6461 793c 2f74 643e 0a20  td>Monday</td>. 
+0009d220: 2020 2020 203c 7464 3e44 656c 6920 2f20       <td>Deli / 
+0009d230: 426f 6465 6761 3c2f 7464 3e0a 2020 2020  Bodega</td>.    
+0009d240: 2020 3c74 643e 3430 2e38 3334 3039 383c    <td>40.834098<
+0009d250: 2f74 643e 0a20 2020 2020 203c 7464 3e2d  /td>.      <td>-
+0009d260: 3733 2e39 3435 3236 373c 2f74 643e 0a20  73.945267</td>. 
+0009d270: 2020 2020 203c 7464 3e31 3236 3c2f 7464       <td>126</td
+0009d280: 3e0a 2020 2020 2020 3c74 643e 466f 6f64  >.      <td>Food
+0009d290: 3c2f 7464 3e0a 2020 2020 3c2f 7472 3e0a  </td>.    </tr>.
+0009d2a0: 2020 2020 3c74 723e 0a20 2020 2020 203c      <tr>.      <
+0009d2b0: 7468 3e32 3c2f 7468 3e0a 2020 2020 2020  th>2</th>.      
+0009d2c0: 3c74 643e 3230 3132 2d31 312d 3133 2030  <td>2012-11-13 0
+0009d2d0: 303a 3030 3a30 373c 2f74 643e 0a20 2020  0:00:07</td>.   
+0009d2e0: 2020 203c 7464 3e30 3c2f 7464 3e0a 2020     <td>0</td>.  
+0009d2f0: 2020 2020 3c74 643e 2d31 2e30 3c2f 7464      <td>-1.0</td
+0009d300: 3e0a 2020 2020 2020 3c74 643e 2d31 3c2f  >.      <td>-1</
+0009d310: 7464 3e0a 2020 2020 2020 3c74 643e 436c  td>.      <td>Cl
+0009d320: 6f75 6473 3c2f 7464 3e0a 2020 2020 2020  ouds</td>.      
+0009d330: 3c74 643e 5475 6573 6461 793c 2f74 643e  <td>Tuesday</td>
+0009d340: 0a20 2020 2020 203c 7464 3e48 6f6d 6520  .      <td>Home 
+0009d350: 2870 7269 7661 7465 293c 2f74 643e 0a20  (private)</td>. 
+0009d360: 2020 2020 203c 7464 3e34 302e 3833 3331       <td>40.8331
+0009d370: 3635 3c2f 7464 3e0a 2020 2020 2020 3c74  65</td>.      <t
+0009d380: 643e 2d37 332e 3934 3138 3630 3c2f 7464  d>-73.941860</td
+0009d390: 3e0a 2020 2020 2020 3c74 643e 3132 363c  >.      <td>126<
+0009d3a0: 2f74 643e 0a20 2020 2020 203c 7464 3e52  /td>.      <td>R
+0009d3b0: 6573 6964 656e 6365 3c2f 7464 3e0a 2020  esidence</td>.  
+0009d3c0: 2020 3c2f 7472 3e0a 2020 2020 3c74 723e    </tr>.    <tr>
+0009d3d0: 0a20 2020 2020 203c 7468 3e33 3c2f 7468  .      <th>3</th
+0009d3e0: 3e0a 2020 2020 2020 3c74 643e 3230 3132  >.      <td>2012
+0009d3f0: 2d31 312d 3135 2031 373a 3439 3a30 313c  -11-15 17:49:01<
+0009d400: 2f74 643e 0a20 2020 2020 203c 7464 3e31  /td>.      <td>1
+0009d410: 3036 393c 2f74 643e 0a20 2020 2020 203c  069</td>.      <
+0009d420: 7464 3e36 2e36 3c2f 7464 3e0a 2020 2020  td>6.6</td>.    
+0009d430: 2020 3c74 643e 333c 2f74 643e 0a20 2020    <td>3</td>.   
+0009d440: 2020 203c 7464 3e43 6c65 6172 3c2f 7464     <td>Clear</td
+0009d450: 3e0a 2020 2020 2020 3c74 643e 5468 7572  >.      <td>Thur
+0009d460: 7364 6179 3c2f 7464 3e0a 2020 2020 2020  sday</td>.      
+0009d470: 3c74 643e 4672 6965 6420 4368 6963 6b65  <td>Fried Chicke
+0009d480: 6e20 4a6f 696e 743c 2f74 643e 0a20 2020  n Joint</td>.   
+0009d490: 2020 203c 7464 3e34 302e 3736 3436 3936     <td>40.764696
+0009d4a0: 3c2f 7464 3e0a 2020 2020 2020 3c74 643e  </td>.      <td>
+0009d4b0: 2d37 332e 3838 3531 3937 3c2f 7464 3e0a  -73.885197</td>.
+0009d4c0: 2020 2020 2020 3c74 643e 3132 363c 2f74        <td>126</t
+0009d4d0: 643e 0a20 2020 2020 203c 7464 3e46 6f6f  d>.      <td>Foo
+0009d4e0: 643c 2f74 643e 0a20 2020 203c 2f74 723e  d</td>.    </tr>
+0009d4f0: 0a20 2020 203c 7472 3e0a 2020 2020 2020  .    <tr>.      
+0009d500: 3c74 683e 343c 2f74 683e 0a20 2020 2020  <th>4</th>.     
+0009d510: 203c 7464 3e32 3031 322d 3131 2d31 3520   <td>2012-11-15 
+0009d520: 3138 3a34 303a 3136 3c2f 7464 3e0a 2020  18:40:16</td>.  
+0009d530: 2020 2020 3c74 643e 3131 3230 3c2f 7464      <td>1120</td
+0009d540: 3e0a 2020 2020 2020 3c74 643e 2d31 2e30  >.      <td>-1.0
+0009d550: 3c2f 7464 3e0a 2020 2020 2020 3c74 643e  </td>.      <td>
+0009d560: 2d31 3c2f 7464 3e0a 2020 2020 2020 3c74  -1</td>.      <t
+0009d570: 643e 436c 6561 723c 2f74 643e 0a20 2020  d>Clear</td>.   
+0009d580: 2020 203c 7464 3e54 6875 7273 6461 793c     <td>Thursday<
+0009d590: 2f74 643e 0a20 2020 2020 203c 7464 3e42  /td>.      <td>B
+0009d5a0: 7573 2053 7461 7469 6f6e 3c2f 7464 3e0a  us Station</td>.
+0009d5b0: 2020 2020 2020 3c74 643e 3430 2e37 3636        <td>40.766
+0009d5c0: 3037 393c 2f74 643e 0a20 2020 2020 203c  079</td>.      <
+0009d5d0: 7464 3e2d 3733 2e38 3833 3532 393c 2f74  td>-73.883529</t
+0009d5e0: 643e 0a20 2020 2020 203c 7464 3e31 3236  d>.      <td>126
+0009d5f0: 3c2f 7464 3e0a 2020 2020 2020 3c74 643e  </td>.      <td>
+0009d600: 5472 6176 656c 2026 616d 703b 2054 7261  Travel &amp; Tra
+0009d610: 6e73 706f 7274 3c2f 7464 3e0a 2020 2020  nsport</td>.    
+0009d620: 3c2f 7472 3e0a 2020 2020 3c74 723e 0a20  </tr>.    <tr>. 
+0009d630: 2020 2020 203c 7468 3e2e 2e2e 3c2f 7468       <th>...</th
+0009d640: 3e0a 2020 2020 2020 3c74 643e 2e2e 2e3c  >.      <td>...<
+0009d650: 2f74 643e 0a20 2020 2020 203c 7464 3e2e  /td>.      <td>.
+0009d660: 2e2e 3c2f 7464 3e0a 2020 2020 2020 3c74  ..</td>.      <t
+0009d670: 643e 2e2e 2e3c 2f74 643e 0a20 2020 2020  d>...</td>.     
+0009d680: 203c 7464 3e2e 2e2e 3c2f 7464 3e0a 2020   <td>...</td>.  
+0009d690: 2020 2020 3c74 643e 2e2e 2e3c 2f74 643e      <td>...</td>
+0009d6a0: 0a20 2020 2020 203c 7464 3e2e 2e2e 3c2f  .      <td>...</
+0009d6b0: 7464 3e0a 2020 2020 2020 3c74 643e 2e2e  td>.      <td>..
+0009d6c0: 2e3c 2f74 643e 0a20 2020 2020 203c 7464  .</td>.      <td
+0009d6d0: 3e2e 2e2e 3c2f 7464 3e0a 2020 2020 2020  >...</td>.      
+0009d6e0: 3c74 643e 2e2e 2e3c 2f74 643e 0a20 2020  <td>...</td>.   
+0009d6f0: 2020 203c 7464 3e2e 2e2e 3c2f 7464 3e0a     <td>...</td>.
+0009d700: 2020 2020 2020 3c74 643e 2e2e 2e3c 2f74        <td>...</t
+0009d710: 643e 0a20 2020 203c 2f74 723e 0a20 2020  d>.    </tr>.   
+0009d720: 203c 7472 3e0a 2020 2020 2020 3c74 683e   <tr>.      <th>
+0009d730: 3636 3935 373c 2f74 683e 0a20 2020 2020  66957</th>.     
+0009d740: 203c 7464 3e32 3031 322d 3038 2d31 3020   <td>2012-08-10 
+0009d750: 3137 3a31 373a 3337 3c2f 7464 3e0a 2020  17:17:37</td>.  
+0009d760: 2020 2020 3c74 643e 3130 3337 3c2f 7464      <td>1037</td
+0009d770: 3e0a 2020 2020 2020 3c74 643e 2d31 2e30  >.      <td>-1.0
+0009d780: 3c2f 7464 3e0a 2020 2020 2020 3c74 643e  </td>.      <td>
+0009d790: 2d31 3c2f 7464 3e0a 2020 2020 2020 3c74  -1</td>.      <t
+0009d7a0: 643e 436c 6f75 6473 3c2f 7464 3e0a 2020  d>Clouds</td>.  
+0009d7b0: 2020 2020 3c74 643e 4672 6964 6179 3c2f      <td>Friday</
+0009d7c0: 7464 3e0a 2020 2020 2020 3c74 643e 4765  td>.      <td>Ge
+0009d7d0: 6e65 7261 6c20 436f 6c6c 6567 6520 2661  neral College &a
+0009d7e0: 6d70 3b20 556e 6976 6572 7369 7479 3c2f  mp; University</
+0009d7f0: 7464 3e0a 2020 2020 2020 3c74 643e 3430  td>.      <td>40
+0009d800: 2e37 3034 3733 333c 2f74 643e 0a20 2020  .704733</td>.   
+0009d810: 2020 203c 7464 3e2d 3733 2e39 3837 3733     <td>-73.98773
+0009d820: 383c 2f74 643e 0a20 2020 2020 203c 7464  8</td>.      <td
+0009d830: 3e32 3935 3633 3c2f 7464 3e0a 2020 2020  >29563</td>.    
+0009d840: 2020 3c74 643e 436f 6c6c 6567 6520 2661    <td>College &a
+0009d850: 6d70 3b20 556e 6976 6572 7369 7479 3c2f  mp; University</
+0009d860: 7464 3e0a 2020 2020 3c2f 7472 3e0a 2020  td>.    </tr>.  
+0009d870: 2020 3c74 723e 0a20 2020 2020 203c 7468    <tr>.      <th
+0009d880: 3e36 3639 3538 3c2f 7468 3e0a 2020 2020  >66958</th>.    
+0009d890: 2020 3c74 643e 3230 3132 2d30 382d 3130    <td>2012-08-10
+0009d8a0: 2032 303a 3130 3a35 393c 2f74 643e 0a20   20:10:59</td>. 
+0009d8b0: 2020 2020 203c 7464 3e31 3231 303c 2f74       <td>1210</t
+0009d8c0: 643e 0a20 2020 2020 203c 7464 3e38 2e30  d>.      <td>8.0
+0009d8d0: 3c2f 7464 3e0a 2020 2020 2020 3c74 643e  </td>.      <td>
+0009d8e0: 323c 2f74 643e 0a20 2020 2020 203c 7464  2</td>.      <td
+0009d8f0: 3e43 6c6f 7564 733c 2f74 643e 0a20 2020  >Clouds</td>.   
+0009d900: 2020 203c 7464 3e46 7269 6461 793c 2f74     <td>Friday</t
+0009d910: 643e 0a20 2020 2020 203c 7464 3e54 6861  d>.      <td>Tha
+0009d920: 6920 5265 7374 6175 7261 6e74 3c2f 7464  i Restaurant</td
+0009d930: 3e0a 2020 2020 2020 3c74 643e 3430 2e36  >.      <td>40.6
+0009d940: 3935 3136 333c 2f74 643e 0a20 2020 2020  95163</td>.     
+0009d950: 203c 7464 3e2d 3733 2e39 3935 3434 383c   <td>-73.995448<
+0009d960: 2f74 643e 0a20 2020 2020 203c 7464 3e32  /td>.      <td>2
+0009d970: 3935 3633 3c2f 7464 3e0a 2020 2020 2020  9563</td>.      
+0009d980: 3c74 643e 466f 6f64 3c2f 7464 3e0a 2020  <td>Food</td>.  
+0009d990: 2020 3c2f 7472 3e0a 2020 2020 3c74 723e    </tr>.    <tr>
+0009d9a0: 0a20 2020 2020 203c 7468 3e36 3639 3539  .      <th>66959
+0009d9b0: 3c2f 7468 3e0a 2020 2020 2020 3c74 643e  </th>.      <td>
+0009d9c0: 3230 3132 2d30 382d 3131 2030 383a 3031  2012-08-11 08:01
+0009d9d0: 3a32 303c 2f74 643e 0a20 2020 2020 203c  :20</td>.      <
+0009d9e0: 7464 3e34 3831 3c2f 7464 3e0a 2020 2020  td>481</td>.    
+0009d9f0: 2020 3c74 643e 362e 393c 2f74 643e 0a20    <td>6.9</td>. 
+0009da00: 2020 2020 203c 7464 3e2d 313c 2f74 643e       <td>-1</td>
+0009da10: 0a20 2020 2020 203c 7464 3e43 6c6f 7564  .      <td>Cloud
+0009da20: 733c 2f74 643e 0a20 2020 2020 203c 7464  s</td>.      <td
+0009da30: 3e53 6174 7572 6461 793c 2f74 643e 0a20  >Saturday</td>. 
+0009da40: 2020 2020 203c 7464 3e47 796d 3c2f 7464       <td>Gym</td
+0009da50: 3e0a 2020 2020 2020 3c74 643e 3430 2e36  >.      <td>40.6
+0009da60: 3937 3830 333c 2f74 643e 0a20 2020 2020  97803</td>.     
+0009da70: 203c 7464 3e2d 3733 2e39 3934 3134 353c   <td>-73.994145<
+0009da80: 2f74 643e 0a20 2020 2020 203c 7464 3e32  /td>.      <td>2
+0009da90: 3935 3633 3c2f 7464 3e0a 2020 2020 2020  9563</td>.      
+0009daa0: 3c74 643e 4f75 7464 6f6f 7273 2026 616d  <td>Outdoors &am
+0009dab0: 703b 2052 6563 7265 6174 696f 6e3c 2f74  p; Recreation</t
+0009dac0: 643e 0a20 2020 203c 2f74 723e 0a20 2020  d>.    </tr>.   
+0009dad0: 203c 7472 3e0a 2020 2020 2020 3c74 683e   <tr>.      <th>
+0009dae0: 3636 3936 303c 2f74 683e 0a20 2020 2020  66960</th>.     
+0009daf0: 203c 7464 3e32 3031 322d 3038 2d31 3120   <td>2012-08-11 
+0009db00: 3133 3a33 393a 3339 3c2f 7464 3e0a 2020  13:39:39</td>.  
+0009db10: 2020 2020 3c74 643e 3831 393c 2f74 643e      <td>819</td>
+0009db20: 0a20 2020 2020 203c 7464 3e37 2e30 3c2f  .      <td>7.0</
+0009db30: 7464 3e0a 2020 2020 2020 3c74 643e 313c  td>.      <td>1<
+0009db40: 2f74 643e 0a20 2020 2020 203c 7464 3e43  /td>.      <td>C
+0009db50: 6c6f 7564 733c 2f74 643e 0a20 2020 2020  louds</td>.     
+0009db60: 203c 7464 3e53 6174 7572 6461 793c 2f74   <td>Saturday</t
+0009db70: 643e 0a20 2020 2020 203c 7464 3e43 6f66  d>.      <td>Cof
+0009db80: 6665 6520 5368 6f70 3c2f 7464 3e0a 2020  fee Shop</td>.  
+0009db90: 2020 2020 3c74 643e 3430 2e36 3934 3637      <td>40.69467
+0009dba0: 333c 2f74 643e 0a20 2020 2020 203c 7464  3</td>.      <td
+0009dbb0: 3e2d 3733 2e39 3934 3038 323c 2f74 643e  >-73.994082</td>
+0009dbc0: 0a20 2020 2020 203c 7464 3e32 3935 3633  .      <td>29563
+0009dbd0: 3c2f 7464 3e0a 2020 2020 2020 3c74 643e  </td>.      <td>
+0009dbe0: 466f 6f64 3c2f 7464 3e0a 2020 2020 3c2f  Food</td>.    </
+0009dbf0: 7472 3e0a 2020 2020 3c74 723e 0a20 2020  tr>.    <tr>.   
+0009dc00: 2020 203c 7468 3e36 3639 3631 3c2f 7468     <th>66961</th
+0009dc10: 3e0a 2020 2020 2020 3c74 643e 3230 3132  >.      <td>2012
+0009dc20: 2d30 382d 3132 2030 373a 3536 3a32 363c  -08-12 07:56:26<
+0009dc30: 2f74 643e 0a20 2020 2020 203c 7464 3e34  /td>.      <td>4
+0009dc40: 3736 3c2f 7464 3e0a 2020 2020 2020 3c74  76</td>.      <t
+0009dc50: 643e 362e 393c 2f74 643e 0a20 2020 2020  d>6.9</td>.     
+0009dc60: 203c 7464 3e2d 313c 2f74 643e 0a20 2020   <td>-1</td>.   
+0009dc70: 2020 203c 7464 3e43 6c6f 7564 733c 2f74     <td>Clouds</t
+0009dc80: 643e 0a20 2020 2020 203c 7464 3e53 756e  d>.      <td>Sun
+0009dc90: 6461 793c 2f74 643e 0a20 2020 2020 203c  day</td>.      <
+0009dca0: 7464 3e47 796d 3c2f 7464 3e0a 2020 2020  td>Gym</td>.    
+0009dcb0: 2020 3c74 643e 3430 2e36 3937 3830 333c    <td>40.697803<
+0009dcc0: 2f74 643e 0a20 2020 2020 203c 7464 3e2d  /td>.      <td>-
+0009dcd0: 3733 2e39 3934 3134 353c 2f74 643e 0a20  73.994145</td>. 
+0009dce0: 2020 2020 203c 7464 3e32 3935 3633 3c2f       <td>29563</
+0009dcf0: 7464 3e0a 2020 2020 2020 3c74 643e 4f75  td>.      <td>Ou
+0009dd00: 7464 6f6f 7273 2026 616d 703b 2052 6563  tdoors &amp; Rec
+0009dd10: 7265 6174 696f 6e3c 2f74 643e 0a20 2020  reation</td>.   
+0009dd20: 203c 2f74 723e 0a20 203c 2f74 626f 6479   </tr>.  </tbody
+0009dd30: 3e0a 3c2f 7461 626c 653e 0a3c 703e 3636  >.</table>.<p>66
+0009dd40: 3936 3220 726f 7773 20c3 9720 3131 2063  962 rows .. 11 c
+0009dd50: 6f6c 756d 6e73 3c2f 703e 0a3c 2f64 6976  olumns</p>.</div
+0009dd60: 3e0a 3c2f 6469 763e 0a0a 3c2f 6469 763e  >.</div>..</div>
+0009dd70: 0a0a 3c2f 6469 763e 0a0a 3c2f 6469 763e  ..</div>..</div>
+0009dd80: 0a0a 3c2f 6469 763e 0a3c 6469 7620 636c  ..</div>.<div cl
+0009dd90: 6173 733d 226a 702d 4365 6c6c 206a 702d  ass="jp-Cell jp-
+0009dda0: 4d61 726b 646f 776e 4365 6c6c 206a 702d  MarkdownCell jp-
+0009ddb0: 4e6f 7465 626f 6f6b 2d63 656c 6c22 3e0a  Notebook-cell">.
+0009ddc0: 3c64 6976 2063 6c61 7373 3d22 6a70 2d43  <div class="jp-C
+0009ddd0: 656c 6c2d 696e 7075 7457 7261 7070 6572  ell-inputWrapper
+0009dde0: 223e 0a3c 6469 7620 636c 6173 733d 226a  ">.<div class="j
+0009ddf0: 702d 436f 6c6c 6170 7365 7220 6a70 2d49  p-Collapser jp-I
+0009de00: 6e70 7574 436f 6c6c 6170 7365 7220 6a70  nputCollapser jp
+0009de10: 2d43 656c 6c2d 696e 7075 7443 6f6c 6c61  -Cell-inputColla
+0009de20: 7073 6572 223e 0a3c 2f64 6976 3e0a 3c64  pser">.</div>.<d
+0009de30: 6976 2063 6c61 7373 3d22 6a70 2d49 6e70  iv class="jp-Inp
+0009de40: 7574 4172 6561 206a 702d 4365 6c6c 2d69  utArea jp-Cell-i
+0009de50: 6e70 7574 4172 6561 223e 3c64 6976 2063  nputArea"><div c
+0009de60: 6c61 7373 3d22 6a70 2d49 6e70 7574 5072  lass="jp-InputPr
+0009de70: 6f6d 7074 206a 702d 496e 7075 7441 7265  ompt jp-InputAre
+0009de80: 612d 7072 6f6d 7074 223e 0a3c 2f64 6976  a-prompt">.</div
+0009de90: 3e3c 6469 7620 636c 6173 733d 226a 702d  ><div class="jp-
+0009dea0: 5265 6e64 6572 6564 4854 4d4c 436f 6d6d  RenderedHTMLComm
+0009deb0: 6f6e 206a 702d 5265 6e64 6572 6564 4d61  on jp-RenderedMa
+0009dec0: 726b 646f 776e 206a 702d 4d61 726b 646f  rkdown jp-Markdo
+0009ded0: 776e 4f75 7470 7574 2022 2064 6174 612d  wnOutput " data-
+0009dee0: 6d69 6d65 2d74 7970 653d 2274 6578 742f  mime-type="text/
+0009def0: 6d61 726b 646f 776e 223e 0a0a 3c70 7265  markdown">..<pre
+0009df00: 3e3c 636f 6465 3e62 2920 5472 6169 6e20  ><code>b) Train 
+0009df10: 616e 6420 7465 7374 2073 706c 6974 3a3c  and test split:<
+0009df20: 2f63 6f64 653e 3c2f 7072 653e 0a0a 3c2f  /code></pre>..</
+0009df30: 6469 763e 0a3c 2f64 6976 3e0a 3c2f 6469  div>.</div>.</di
+0009df40: 763e 0a3c 2f64 6976 3e0a 3c64 6976 2063  v>.</div>.<div c
+0009df50: 6c61 7373 3d22 6a70 2d43 656c 6c20 6a70  lass="jp-Cell jp
+0009df60: 2d4d 6172 6b64 6f77 6e43 656c 6c20 6a70  -MarkdownCell jp
+0009df70: 2d4e 6f74 6562 6f6f 6b2d 6365 6c6c 223e  -Notebook-cell">
+0009df80: 0a3c 6469 7620 636c 6173 733d 226a 702d  .<div class="jp-
+0009df90: 4365 6c6c 2d69 6e70 7574 5772 6170 7065  Cell-inputWrappe
+0009dfa0: 7222 3e0a 3c64 6976 2063 6c61 7373 3d22  r">.<div class="
+0009dfb0: 6a70 2d43 6f6c 6c61 7073 6572 206a 702d  jp-Collapser jp-
+0009dfc0: 496e 7075 7443 6f6c 6c61 7073 6572 206a  InputCollapser j
+0009dfd0: 702d 4365 6c6c 2d69 6e70 7574 436f 6c6c  p-Cell-inputColl
+0009dfe0: 6170 7365 7222 3e0a 3c2f 6469 763e 0a3c  apser">.</div>.<
+0009dff0: 6469 7620 636c 6173 733d 226a 702d 496e  div class="jp-In
+0009e000: 7075 7441 7265 6120 6a70 2d43 656c 6c2d  putArea jp-Cell-
+0009e010: 696e 7075 7441 7265 6122 3e3c 6469 7620  inputArea"><div 
+0009e020: 636c 6173 733d 226a 702d 496e 7075 7450  class="jp-InputP
+0009e030: 726f 6d70 7420 6a70 2d49 6e70 7574 4172  rompt jp-InputAr
+0009e040: 6561 2d70 726f 6d70 7422 3e0a 3c2f 6469  ea-prompt">.</di
+0009e050: 763e 3c64 6976 2063 6c61 7373 3d22 6a70  v><div class="jp
+0009e060: 2d52 656e 6465 7265 6448 544d 4c43 6f6d  -RenderedHTMLCom
+0009e070: 6d6f 6e20 6a70 2d52 656e 6465 7265 644d  mon jp-RenderedM
+0009e080: 6172 6b64 6f77 6e20 6a70 2d4d 6172 6b64  arkdown jp-Markd
+0009e090: 6f77 6e4f 7574 7075 7420 2220 6461 7461  ownOutput " data
+0009e0a0: 2d6d 696d 652d 7479 7065 3d22 7465 7874  -mime-type="text
+0009e0b0: 2f6d 6172 6b64 6f77 6e22 3e0a 3c70 3e54  /markdown">.<p>T
+0009e0c0: 6f20 686f 6c64 2d6f 7574 2073 706c 6974  o hold-out split
+0009e0d0: 2061 2064 6174 6173 6574 2069 6e74 6f20   a dataset into 
+0009e0e0: 7472 6169 6e20 616e 6420 7465 7374 2028  train and test (
+0009e0f0: 3730 2f33 3025 2062 7920 6465 6166 756c  70/30% by deaful
+0009e100: 7429 3a3c 2f70 3e0a 0a3c 2f64 6976 3e0a  t):</p>..</div>.
+0009e110: 3c2f 6469 763e 0a3c 2f64 6976 3e0a 3c2f  </div>.</div>.</
+0009e120: 6469 763e 3c64 6976 2063 6c61 7373 3d22  div><div class="
+0009e130: 6a70 2d43 656c 6c20 6a70 2d43 6f64 6543  jp-Cell jp-CodeC
+0009e140: 656c 6c20 6a70 2d4e 6f74 6562 6f6f 6b2d  ell jp-Notebook-
+0009e150: 6365 6c6c 2020 2022 3e0a 3c64 6976 2063  cell   ">.<div c
+0009e160: 6c61 7373 3d22 6a70 2d43 656c 6c2d 696e  lass="jp-Cell-in
+0009e170: 7075 7457 7261 7070 6572 223e 0a3c 6469  putWrapper">.<di
+0009e180: 7620 636c 6173 733d 226a 702d 436f 6c6c  v class="jp-Coll
+0009e190: 6170 7365 7220 6a70 2d49 6e70 7574 436f  apser jp-InputCo
+0009e1a0: 6c6c 6170 7365 7220 6a70 2d43 656c 6c2d  llapser jp-Cell-
+0009e1b0: 696e 7075 7443 6f6c 6c61 7073 6572 223e  inputCollapser">
+0009e1c0: 0a3c 2f64 6976 3e0a 3c64 6976 2063 6c61  .</div>.<div cla
+0009e1d0: 7373 3d22 6a70 2d49 6e70 7574 4172 6561  ss="jp-InputArea
+0009e1e0: 206a 702d 4365 6c6c 2d69 6e70 7574 4172   jp-Cell-inputAr
+0009e1f0: 6561 223e 0a3c 6469 7620 636c 6173 733d  ea">.<div class=
+0009e200: 226a 702d 496e 7075 7450 726f 6d70 7420  "jp-InputPrompt 
+0009e210: 6a70 2d49 6e70 7574 4172 6561 2d70 726f  jp-InputArea-pro
+0009e220: 6d70 7422 3e49 6e26 6e62 7370 3b5b 3233  mpt">In&nbsp;[23
+0009e230: 5d3a 3c2f 6469 763e 0a3c 6469 7620 636c  ]:</div>.<div cl
+0009e240: 6173 733d 226a 702d 436f 6465 4d69 7272  ass="jp-CodeMirr
+0009e250: 6f72 4564 6974 6f72 206a 702d 4564 6974  orEditor jp-Edit
+0009e260: 6f72 206a 702d 496e 7075 7441 7265 612d  or jp-InputArea-
+0009e270: 6564 6974 6f72 2220 6461 7461 2d74 7970  editor" data-typ
+0009e280: 653d 2269 6e6c 696e 6522 3e0a 2020 2020  e="inline">.    
+0009e290: 203c 6469 7620 636c 6173 733d 2243 6f64   <div class="Cod
+0009e2a0: 654d 6972 726f 7220 636d 2d73 2d6a 7570  eMirror cm-s-jup
+0009e2b0: 7974 6572 223e 0a3c 6469 7620 636c 6173  yter">.<div clas
+0009e2c0: 733d 2220 6869 6768 6c69 6768 7420 686c  s=" highlight hl
+0009e2d0: 2d69 7079 7468 6f6e 3322 3e3c 7072 653e  -ipython3"><pre>
+0009e2e0: 3c73 7061 6e3e 3c2f 7370 616e 3e3c 7370  <span></span><sp
+0009e2f0: 616e 2063 6c61 7373 3d22 6e22 3e74 7261  an class="n">tra
+0009e300: 696e 3c2f 7370 616e 3e3c 7370 616e 2063  in</span><span c
+0009e310: 6c61 7373 3d22 7022 3e2c 3c2f 7370 616e  lass="p">,</span
+0009e320: 3e20 3c73 7061 6e20 636c 6173 733d 226e  > <span class="n
+0009e330: 223e 7465 7374 3c2f 7370 616e 3e20 3c73  ">test</span> <s
+0009e340: 7061 6e20 636c 6173 733d 226f 223e 3d3c  pan class="o">=<
+0009e350: 2f73 7061 6e3e 203c 7370 616e 2063 6c61  /span> <span cla
+0009e360: 7373 3d22 6e22 3e74 7261 696e 5465 7374  ss="n">trainTest
+0009e370: 5370 6c69 743c 2f73 7061 6e3e 3c73 7061  Split</span><spa
+0009e380: 6e20 636c 6173 733d 2270 223e 283c 2f73  n class="p">(</s
+0009e390: 7061 6e3e 3c73 7061 6e20 636c 6173 733d  pan><span class=
+0009e3a0: 226e 223e 6466 3c2f 7370 616e 3e3c 7370  "n">df</span><sp
+0009e3b0: 616e 2063 6c61 7373 3d22 7022 3e2c 3c2f  an class="p">,</
+0009e3c0: 7370 616e 3e20 3c73 7061 6e20 636c 6173  span> <span clas
+0009e3d0: 733d 226e 223e 7261 6e64 6f6d 5f6e 756d  s="n">random_num
+0009e3e0: 3c2f 7370 616e 3e3c 7370 616e 2063 6c61  </span><span cla
+0009e3f0: 7373 3d22 6f22 3e3d 3c2f 7370 616e 3e3c  ss="o">=</span><
+0009e400: 7370 616e 2063 6c61 7373 3d22 6d69 223e  span class="mi">
+0009e410: 313c 2f73 7061 6e3e 3c73 7061 6e20 636c  1</span><span cl
+0009e420: 6173 733d 2270 223e 293c 2f73 7061 6e3e  ass="p">)</span>
+0009e430: 0a3c 7370 616e 2063 6c61 7373 3d22 6e22  .<span class="n"
+0009e440: 3e74 7261 696e 3c2f 7370 616e 3e3c 7370  >train</span><sp
+0009e450: 616e 2063 6c61 7373 3d22 6f22 3e2e 3c2f  an class="o">.</
+0009e460: 7370 616e 3e3c 7370 616e 2063 6c61 7373  span><span class
+0009e470: 3d22 6e22 3e68 6561 643c 2f73 7061 6e3e  ="n">head</span>
+0009e480: 3c73 7061 6e20 636c 6173 733d 2270 223e  <span class="p">
+0009e490: 2829 3c2f 7370 616e 3e0a 3c2f 7072 653e  ()</span>.</pre>
+0009e4a0: 3c2f 6469 763e 0a0a 2020 2020 203c 2f64  </div>..     </d
+0009e4b0: 6976 3e0a 3c2f 6469 763e 0a3c 2f64 6976  iv>.</div>.</div
+0009e4c0: 3e0a 3c2f 6469 763e 0a0a 3c64 6976 2063  >.</div>..<div c
+0009e4d0: 6c61 7373 3d22 6a70 2d43 656c 6c2d 6f75  lass="jp-Cell-ou
+0009e4e0: 7470 7574 5772 6170 7065 7222 3e0a 3c64  tputWrapper">.<d
+0009e4f0: 6976 2063 6c61 7373 3d22 6a70 2d43 6f6c  iv class="jp-Col
+0009e500: 6c61 7073 6572 206a 702d 4f75 7470 7574  lapser jp-Output
+0009e510: 436f 6c6c 6170 7365 7220 6a70 2d43 656c  Collapser jp-Cel
+0009e520: 6c2d 6f75 7470 7574 436f 6c6c 6170 7365  l-outputCollapse
+0009e530: 7222 3e0a 3c2f 6469 763e 0a0a 0a3c 6469  r">.</div>...<di
+0009e540: 7620 636c 6173 733d 226a 702d 4f75 7470  v class="jp-Outp
+0009e550: 7574 4172 6561 206a 702d 4365 6c6c 2d6f  utArea jp-Cell-o
+0009e560: 7574 7075 7441 7265 6122 3e0a 0a3c 6469  utputArea">..<di
+0009e570: 7620 636c 6173 733d 226a 702d 4f75 7470  v class="jp-Outp
+0009e580: 7574 4172 6561 2d63 6869 6c64 223e 0a0a  utArea-child">..
+0009e590: 2020 2020 0a20 2020 203c 6469 7620 636c      .    <div cl
+0009e5a0: 6173 733d 226a 702d 4f75 7470 7574 5072  ass="jp-OutputPr
+0009e5b0: 6f6d 7074 206a 702d 4f75 7470 7574 4172  ompt jp-OutputAr
+0009e5c0: 6561 2d70 726f 6d70 7422 3e3c 2f64 6976  ea-prompt"></div
+0009e5d0: 3e0a 0a0a 0a0a 3c64 6976 2063 6c61 7373  >.....<div class
+0009e5e0: 3d22 6a70 2d52 656e 6465 7265 6454 6578  ="jp-RenderedTex
+0009e5f0: 7420 6a70 2d4f 7574 7075 7441 7265 612d  t jp-OutputArea-
+0009e600: 6f75 7470 7574 2022 2064 6174 612d 6d69  output " data-mi
+0009e610: 6d65 2d74 7970 653d 2274 6578 742f 706c  me-type="text/pl
+0009e620: 6169 6e22 3e0a 3c70 7265 3e20 2030 257c  ain">.<pre>  0%|
+0009e630: 2020 2020 2020 2020 2020 7c20 302f 3920            | 0/9 
+0009e640: 5b30 303a 3030 266c 743b 3f2c 203f 6974  [00:00&lt;?, ?it
+0009e650: 2f73 5d3c 2f70 7265 3e0a 3c2f 6469 763e  /s]</pre>.</div>
+0009e660: 0a0a 3c2f 6469 763e 0a0a 3c64 6976 2063  ..</div>..<div c
+0009e670: 6c61 7373 3d22 6a70 2d4f 7574 7075 7441  lass="jp-OutputA
+0009e680: 7265 612d 6368 696c 6422 3e0a 0a20 2020  rea-child">..   
+0009e690: 200a 2020 2020 3c64 6976 2063 6c61 7373   .    <div class
+0009e6a0: 3d22 6a70 2d4f 7574 7075 7450 726f 6d70  ="jp-OutputPromp
+0009e6b0: 7420 6a70 2d4f 7574 7075 7441 7265 612d  t jp-OutputArea-
+0009e6c0: 7072 6f6d 7074 223e 4f75 745b 3233 5d3a  prompt">Out[23]:
+0009e6d0: 3c2f 6469 763e 0a0a 0a0a 3c64 6976 2063  </div>....<div c
+0009e6e0: 6c61 7373 3d22 6a70 2d52 656e 6465 7265  lass="jp-Rendere
+0009e6f0: 6448 544d 4c43 6f6d 6d6f 6e20 6a70 2d52  dHTMLCommon jp-R
+0009e700: 656e 6465 7265 6448 544d 4c20 6a70 2d4f  enderedHTML jp-O
+0009e710: 7574 7075 7441 7265 612d 6f75 7470 7574  utputArea-output
+0009e720: 206a 702d 4f75 7470 7574 4172 6561 2d65   jp-OutputArea-e
+0009e730: 7865 6375 7465 5265 7375 6c74 2220 6461  xecuteResult" da
+0009e740: 7461 2d6d 696d 652d 7479 7065 3d22 7465  ta-mime-type="te
+0009e750: 7874 2f68 746d 6c22 3e0a 3c64 6976 3e0a  xt/html">.<div>.
+0009e760: 3c73 7479 6c65 2073 636f 7065 643e 0a20  <style scoped>. 
+0009e770: 2020 202e 6461 7461 6672 616d 6520 7462     .dataframe tb
+0009e780: 6f64 7920 7472 2074 683a 6f6e 6c79 2d6f  ody tr th:only-o
+0009e790: 662d 7479 7065 207b 0a20 2020 2020 2020  f-type {.       
+0009e7a0: 2076 6572 7469 6361 6c2d 616c 6967 6e3a   vertical-align:
+0009e7b0: 206d 6964 646c 653b 0a20 2020 207d 0a0a   middle;.    }..
+0009e7c0: 2020 2020 2e64 6174 6166 7261 6d65 2074      .dataframe t
+0009e7d0: 626f 6479 2074 7220 7468 207b 0a20 2020  body tr th {.   
+0009e7e0: 2020 2020 2076 6572 7469 6361 6c2d 616c       vertical-al
+0009e7f0: 6967 6e3a 2074 6f70 3b0a 2020 2020 7d0a  ign: top;.    }.
+0009e800: 0a20 2020 202e 6461 7461 6672 616d 6520  .    .dataframe 
+0009e810: 7468 6561 6420 7468 207b 0a20 2020 2020  thead th {.     
+0009e820: 2020 2074 6578 742d 616c 6967 6e3a 2072     text-align: r
+0009e830: 6967 6874 3b0a 2020 2020 7d0a 3c2f 7374  ight;.    }.</st
+0009e840: 796c 653e 0a3c 7461 626c 6520 626f 7264  yle>.<table bord
+0009e850: 6572 3d22 3122 2063 6c61 7373 3d22 6461  er="1" class="da
+0009e860: 7461 6672 616d 6522 3e0a 2020 3c74 6865  taframe">.  <the
+0009e870: 6164 3e0a 2020 2020 3c74 7220 7374 796c  ad>.    <tr styl
+0009e880: 653d 2274 6578 742d 616c 6967 6e3a 2072  e="text-align: r
+0009e890: 6967 6874 3b22 3e0a 2020 2020 2020 3c74  ight;">.      <t
+0009e8a0: 683e 3c2f 7468 3e0a 2020 2020 2020 3c74  h></th>.      <t
+0009e8b0: 683e 6461 7465 5f74 696d 653c 2f74 683e  h>date_time</th>
+0009e8c0: 0a20 2020 2020 203c 7468 3e74 696d 653c  .      <th>time<
+0009e8d0: 2f74 683e 0a20 2020 2020 203c 7468 3e72  /th>.      <th>r
+0009e8e0: 6174 696e 673c 2f74 683e 0a20 2020 2020  ating</th>.     
+0009e8f0: 203c 7468 3e70 7269 6365 3c2f 7468 3e0a   <th>price</th>.
+0009e900: 2020 2020 2020 3c74 683e 7765 6174 6865        <th>weathe
+0009e910: 723c 2f74 683e 0a20 2020 2020 203c 7468  r</th>.      <th
+0009e920: 3e64 6179 3c2f 7468 3e0a 2020 2020 2020  >day</th>.      
+0009e930: 3c74 683e 7479 7065 3c2f 7468 3e0a 2020  <th>type</th>.  
+0009e940: 2020 2020 3c74 683e 6c61 743c 2f74 683e      <th>lat</th>
+0009e950: 0a20 2020 2020 203c 7468 3e6c 6f6e 3c2f  .      <th>lon</
+0009e960: 7468 3e0a 2020 2020 2020 3c74 683e 7469  th>.      <th>ti
+0009e970: 643c 2f74 683e 0a20 2020 2020 203c 7468  d</th>.      <th
+0009e980: 3e6c 6162 656c 3c2f 7468 3e0a 2020 2020  >label</th>.    
+0009e990: 3c2f 7472 3e0a 2020 3c2f 7468 6561 643e  </tr>.  </thead>
+0009e9a0: 0a20 203c 7462 6f64 793e 0a20 2020 203c  .  <tbody>.    <
+0009e9b0: 7472 3e0a 2020 2020 2020 3c74 683e 303c  tr>.      <th>0<
+0009e9c0: 2f74 683e 0a20 2020 2020 203c 7464 3e32  /th>.      <td>2
+0009e9d0: 3031 322d 3131 2d31 3220 3035 3a31 373a  012-11-12 05:17:
+0009e9e0: 3138 3c2f 7464 3e0a 2020 2020 2020 3c74  18</td>.      <t
+0009e9f0: 643e 3331 373c 2f74 643e 0a20 2020 2020  d>317</td>.     
+0009ea00: 203c 7464 3e2d 312e 303c 2f74 643e 0a20   <td>-1.0</td>. 
+0009ea10: 2020 2020 203c 7464 3e2d 313c 2f74 643e       <td>-1</td>
+0009ea20: 0a20 2020 2020 203c 7464 3e43 6c65 6172  .      <td>Clear
+0009ea30: 3c2f 7464 3e0a 2020 2020 2020 3c74 643e  </td>.      <td>
+0009ea40: 4d6f 6e64 6179 3c2f 7464 3e0a 2020 2020  Monday</td>.    
+0009ea50: 2020 3c74 643e 486f 6d65 2028 7072 6976    <td>Home (priv
+0009ea60: 6174 6529 3c2f 7464 3e0a 2020 2020 2020  ate)</td>.      
+0009ea70: 3c74 643e 3430 2e38 3333 3136 353c 2f74  <td>40.833165</t
+0009ea80: 643e 0a20 2020 2020 203c 7464 3e2d 3733  d>.      <td>-73
+0009ea90: 2e39 3431 3836 303c 2f74 643e 0a20 2020  .941860</td>.   
+0009eaa0: 2020 203c 7464 3e31 3236 3c2f 7464 3e0a     <td>126</td>.
+0009eab0: 2020 2020 2020 3c74 643e 5265 7369 6465        <td>Reside
+0009eac0: 6e63 653c 2f74 643e 0a20 2020 203c 2f74  nce</td>.    </t
+0009ead0: 723e 0a20 2020 203c 7472 3e0a 2020 2020  r>.    <tr>.    
+0009eae0: 2020 3c74 683e 313c 2f74 683e 0a20 2020    <th>1</th>.   
+0009eaf0: 2020 203c 7464 3e32 3031 322d 3131 2d31     <td>2012-11-1
+0009eb00: 3220 3233 3a32 343a 3535 3c2f 7464 3e0a  2 23:24:55</td>.
+0009eb10: 2020 2020 2020 3c74 643e 3134 3034 3c2f        <td>1404</
+0009eb20: 7464 3e0a 2020 2020 2020 3c74 643e 382e  td>.      <td>8.
+0009eb30: 323c 2f74 643e 0a20 2020 2020 203c 7464  2</td>.      <td
+0009eb40: 3e31 3c2f 7464 3e0a 2020 2020 2020 3c74  >1</td>.      <t
+0009eb50: 643e 436c 6f75 6473 3c2f 7464 3e0a 2020  d>Clouds</td>.  
+0009eb60: 2020 2020 3c74 643e 4d6f 6e64 6179 3c2f      <td>Monday</
+0009eb70: 7464 3e0a 2020 2020 2020 3c74 643e 4465  td>.      <td>De
+0009eb80: 6c69 202f 2042 6f64 6567 613c 2f74 643e  li / Bodega</td>
+0009eb90: 0a20 2020 2020 203c 7464 3e34 302e 3833  .      <td>40.83
+0009eba0: 3430 3938 3c2f 7464 3e0a 2020 2020 2020  4098</td>.      
+0009ebb0: 3c74 643e 2d37 332e 3934 3532 3637 3c2f  <td>-73.945267</
+0009ebc0: 7464 3e0a 2020 2020 2020 3c74 643e 3132  td>.      <td>12
+0009ebd0: 363c 2f74 643e 0a20 2020 2020 203c 7464  6</td>.      <td
+0009ebe0: 3e46 6f6f 643c 2f74 643e 0a20 2020 203c  >Food</td>.    <
+0009ebf0: 2f74 723e 0a20 2020 203c 7472 3e0a 2020  /tr>.    <tr>.  
+0009ec00: 2020 2020 3c74 683e 323c 2f74 683e 0a20      <th>2</th>. 
+0009ec10: 2020 2020 203c 7464 3e32 3031 322d 3131       <td>2012-11
+0009ec20: 2d31 3320 3030 3a30 303a 3037 3c2f 7464  -13 00:00:07</td
+0009ec30: 3e0a 2020 2020 2020 3c74 643e 303c 2f74  >.      <td>0</t
+0009ec40: 643e 0a20 2020 2020 203c 7464 3e2d 312e  d>.      <td>-1.
+0009ec50: 303c 2f74 643e 0a20 2020 2020 203c 7464  0</td>.      <td
+0009ec60: 3e2d 313c 2f74 643e 0a20 2020 2020 203c  >-1</td>.      <
+0009ec70: 7464 3e43 6c6f 7564 733c 2f74 643e 0a20  td>Clouds</td>. 
+0009ec80: 2020 2020 203c 7464 3e54 7565 7364 6179       <td>Tuesday
+0009ec90: 3c2f 7464 3e0a 2020 2020 2020 3c74 643e  </td>.      <td>
+0009eca0: 486f 6d65 2028 7072 6976 6174 6529 3c2f  Home (private)</
+0009ecb0: 7464 3e0a 2020 2020 2020 3c74 643e 3430  td>.      <td>40
+0009ecc0: 2e38 3333 3136 353c 2f74 643e 0a20 2020  .833165</td>.   
+0009ecd0: 2020 203c 7464 3e2d 3733 2e39 3431 3836     <td>-73.94186
+0009ece0: 303c 2f74 643e 0a20 2020 2020 203c 7464  0</td>.      <td
+0009ecf0: 3e31 3236 3c2f 7464 3e0a 2020 2020 2020  >126</td>.      
+0009ed00: 3c74 643e 5265 7369 6465 6e63 653c 2f74  <td>Residence</t
+0009ed10: 643e 0a20 2020 203c 2f74 723e 0a20 2020  d>.    </tr>.   
+0009ed20: 203c 7472 3e0a 2020 2020 2020 3c74 683e   <tr>.      <th>
+0009ed30: 333c 2f74 683e 0a20 2020 2020 203c 7464  3</th>.      <td
+0009ed40: 3e32 3031 322d 3131 2d31 3520 3137 3a34  >2012-11-15 17:4
+0009ed50: 393a 3031 3c2f 7464 3e0a 2020 2020 2020  9:01</td>.      
+0009ed60: 3c74 643e 3130 3639 3c2f 7464 3e0a 2020  <td>1069</td>.  
+0009ed70: 2020 2020 3c74 643e 362e 363c 2f74 643e      <td>6.6</td>
+0009ed80: 0a20 2020 2020 203c 7464 3e33 3c2f 7464  .      <td>3</td
+0009ed90: 3e0a 2020 2020 2020 3c74 643e 436c 6561  >.      <td>Clea
+0009eda0: 723c 2f74 643e 0a20 2020 2020 203c 7464  r</td>.      <td
+0009edb0: 3e54 6875 7273 6461 793c 2f74 643e 0a20  >Thursday</td>. 
+0009edc0: 2020 2020 203c 7464 3e46 7269 6564 2043       <td>Fried C
+0009edd0: 6869 636b 656e 204a 6f69 6e74 3c2f 7464  hicken Joint</td
+0009ede0: 3e0a 2020 2020 2020 3c74 643e 3430 2e37  >.      <td>40.7
+0009edf0: 3634 3639 363c 2f74 643e 0a20 2020 2020  64696</td>.     
+0009ee00: 203c 7464 3e2d 3733 2e38 3835 3139 373c   <td>-73.885197<
+0009ee10: 2f74 643e 0a20 2020 2020 203c 7464 3e31  /td>.      <td>1
+0009ee20: 3236 3c2f 7464 3e0a 2020 2020 2020 3c74  26</td>.      <t
+0009ee30: 643e 466f 6f64 3c2f 7464 3e0a 2020 2020  d>Food</td>.    
+0009ee40: 3c2f 7472 3e0a 2020 2020 3c74 723e 0a20  </tr>.    <tr>. 
+0009ee50: 2020 2020 203c 7468 3e34 3c2f 7468 3e0a       <th>4</th>.
+0009ee60: 2020 2020 2020 3c74 643e 3230 3132 2d31        <td>2012-1
+0009ee70: 312d 3135 2031 383a 3430 3a31 363c 2f74  1-15 18:40:16</t
+0009ee80: 643e 0a20 2020 2020 203c 7464 3e31 3132  d>.      <td>112
+0009ee90: 303c 2f74 643e 0a20 2020 2020 203c 7464  0</td>.      <td
+0009eea0: 3e2d 312e 303c 2f74 643e 0a20 2020 2020  >-1.0</td>.     
+0009eeb0: 203c 7464 3e2d 313c 2f74 643e 0a20 2020   <td>-1</td>.   
+0009eec0: 2020 203c 7464 3e43 6c65 6172 3c2f 7464     <td>Clear</td
+0009eed0: 3e0a 2020 2020 2020 3c74 643e 5468 7572  >.      <td>Thur
+0009eee0: 7364 6179 3c2f 7464 3e0a 2020 2020 2020  sday</td>.      
+0009eef0: 3c74 643e 4275 7320 5374 6174 696f 6e3c  <td>Bus Station<
+0009ef00: 2f74 643e 0a20 2020 2020 203c 7464 3e34  /td>.      <td>4
+0009ef10: 302e 3736 3630 3739 3c2f 7464 3e0a 2020  0.766079</td>.  
+0009ef20: 2020 2020 3c74 643e 2d37 332e 3838 3335      <td>-73.8835
+0009ef30: 3239 3c2f 7464 3e0a 2020 2020 2020 3c74  29</td>.      <t
+0009ef40: 643e 3132 363c 2f74 643e 0a20 2020 2020  d>126</td>.     
+0009ef50: 203c 7464 3e54 7261 7665 6c20 2661 6d70   <td>Travel &amp
+0009ef60: 3b20 5472 616e 7370 6f72 743c 2f74 643e  ; Transport</td>
+0009ef70: 0a20 2020 203c 2f74 723e 0a20 203c 2f74  .    </tr>.  </t
+0009ef80: 626f 6479 3e0a 3c2f 7461 626c 653e 0a3c  body>.</table>.<
+0009ef90: 2f64 6976 3e0a 3c2f 6469 763e 0a0a 3c2f  /div>.</div>..</
+0009efa0: 6469 763e 0a0a 3c2f 6469 763e 0a0a 3c2f  div>..</div>..</
+0009efb0: 6469 763e 0a0a 3c2f 6469 763e 0a3c 6469  div>..</div>.<di
+0009efc0: 7620 636c 6173 733d 226a 702d 4365 6c6c  v class="jp-Cell
+0009efd0: 206a 702d 4d61 726b 646f 776e 4365 6c6c   jp-MarkdownCell
+0009efe0: 206a 702d 4e6f 7465 626f 6f6b 2d63 656c   jp-Notebook-cel
+0009eff0: 6c22 3e0a 3c64 6976 2063 6c61 7373 3d22  l">.<div class="
+0009f000: 6a70 2d43 656c 6c2d 696e 7075 7457 7261  jp-Cell-inputWra
+0009f010: 7070 6572 223e 0a3c 6469 7620 636c 6173  pper">.<div clas
+0009f020: 733d 226a 702d 436f 6c6c 6170 7365 7220  s="jp-Collapser 
+0009f030: 6a70 2d49 6e70 7574 436f 6c6c 6170 7365  jp-InputCollapse
+0009f040: 7220 6a70 2d43 656c 6c2d 696e 7075 7443  r jp-Cell-inputC
+0009f050: 6f6c 6c61 7073 6572 223e 0a3c 2f64 6976  ollapser">.</div
+0009f060: 3e0a 3c64 6976 2063 6c61 7373 3d22 6a70  >.<div class="jp
+0009f070: 2d49 6e70 7574 4172 6561 206a 702d 4365  -InputArea jp-Ce
+0009f080: 6c6c 2d69 6e70 7574 4172 6561 223e 3c64  ll-inputArea"><d
+0009f090: 6976 2063 6c61 7373 3d22 6a70 2d49 6e70  iv class="jp-Inp
+0009f0a0: 7574 5072 6f6d 7074 206a 702d 496e 7075  utPrompt jp-Inpu
+0009f0b0: 7441 7265 612d 7072 6f6d 7074 223e 0a3c  tArea-prompt">.<
+0009f0c0: 2f64 6976 3e3c 6469 7620 636c 6173 733d  /div><div class=
+0009f0d0: 226a 702d 5265 6e64 6572 6564 4854 4d4c  "jp-RenderedHTML
+0009f0e0: 436f 6d6d 6f6e 206a 702d 5265 6e64 6572  Common jp-Render
+0009f0f0: 6564 4d61 726b 646f 776e 206a 702d 4d61  edMarkdown jp-Ma
+0009f100: 726b 646f 776e 4f75 7470 7574 2022 2064  rkdownOutput " d
+0009f110: 6174 612d 6d69 6d65 2d74 7970 653d 2274  ata-mime-type="t
+0009f120: 6578 742f 6d61 726b 646f 776e 223e 0a3c  ext/markdown">.<
+0009f130: 703e 4966 2079 6f75 2077 616e 7420 746f  p>If you want to
+0009f140: 2073 6176 652c 2069 6e64 6963 6174 6520   save, indicate 
+0009f150: 7468 6520 6f75 7470 7574 2066 6f72 6d61  the output forma
+0009f160: 7420 616e 6420 6461 7461 2070 6174 683a  t and data path:
+0009f170: 3c2f 703e 0a0a 3c2f 6469 763e 0a3c 2f64  </p>..</div>.</d
+0009f180: 6976 3e0a 3c2f 6469 763e 0a3c 2f64 6976  iv>.</div>.</div
+0009f190: 3e3c 6469 7620 636c 6173 733d 226a 702d  ><div class="jp-
+0009f1a0: 4365 6c6c 206a 702d 436f 6465 4365 6c6c  Cell jp-CodeCell
+0009f1b0: 206a 702d 4e6f 7465 626f 6f6b 2d63 656c   jp-Notebook-cel
+0009f1c0: 6c20 2020 223e 0a3c 6469 7620 636c 6173  l   ">.<div clas
+0009f1d0: 733d 226a 702d 4365 6c6c 2d69 6e70 7574  s="jp-Cell-input
+0009f1e0: 5772 6170 7065 7222 3e0a 3c64 6976 2063  Wrapper">.<div c
+0009f1f0: 6c61 7373 3d22 6a70 2d43 6f6c 6c61 7073  lass="jp-Collaps
+0009f200: 6572 206a 702d 496e 7075 7443 6f6c 6c61  er jp-InputColla
+0009f210: 7073 6572 206a 702d 4365 6c6c 2d69 6e70  pser jp-Cell-inp
+0009f220: 7574 436f 6c6c 6170 7365 7222 3e0a 3c2f  utCollapser">.</
+0009f230: 6469 763e 0a3c 6469 7620 636c 6173 733d  div>.<div class=
+0009f240: 226a 702d 496e 7075 7441 7265 6120 6a70  "jp-InputArea jp
+0009f250: 2d43 656c 6c2d 696e 7075 7441 7265 6122  -Cell-inputArea"
+0009f260: 3e0a 3c64 6976 2063 6c61 7373 3d22 6a70  >.<div class="jp
+0009f270: 2d49 6e70 7574 5072 6f6d 7074 206a 702d  -InputPrompt jp-
+0009f280: 496e 7075 7441 7265 612d 7072 6f6d 7074  InputArea-prompt
+0009f290: 223e 496e 266e 6273 703b 5b32 345d 3a3c  ">In&nbsp;[24]:<
+0009f2a0: 2f64 6976 3e0a 3c64 6976 2063 6c61 7373  /div>.<div class
+0009f2b0: 3d22 6a70 2d43 6f64 654d 6972 726f 7245  ="jp-CodeMirrorE
+0009f2c0: 6469 746f 7220 6a70 2d45 6469 746f 7220  ditor jp-Editor 
+0009f2d0: 6a70 2d49 6e70 7574 4172 6561 2d65 6469  jp-InputArea-edi
+0009f2e0: 746f 7222 2064 6174 612d 7479 7065 3d22  tor" data-type="
+0009f2f0: 696e 6c69 6e65 223e 0a20 2020 2020 3c64  inline">.     <d
+0009f300: 6976 2063 6c61 7373 3d22 436f 6465 4d69  iv class="CodeMi
+0009f310: 7272 6f72 2063 6d2d 732d 6a75 7079 7465  rror cm-s-jupyte
+0009f320: 7222 3e0a 3c64 6976 2063 6c61 7373 3d22  r">.<div class="
+0009f330: 2068 6967 686c 6967 6874 2068 6c2d 6970   highlight hl-ip
+0009f340: 7974 686f 6e33 223e 3c70 7265 3e3c 7370  ython3"><pre><sp
+0009f350: 616e 3e3c 2f73 7061 6e3e 3c73 7061 6e20  an></span><span 
+0009f360: 636c 6173 733d 226e 223e 7472 6169 6e54  class="n">trainT
+0009f370: 6573 7453 706c 6974 3c2f 7370 616e 3e3c  estSplit</span><
+0009f380: 7370 616e 2063 6c61 7373 3d22 7022 3e28  span class="p">(
+0009f390: 3c2f 7370 616e 3e3c 7370 616e 2063 6c61  </span><span cla
+0009f3a0: 7373 3d22 6e22 3e64 663c 2f73 7061 6e3e  ss="n">df</span>
+0009f3b0: 3c73 7061 6e20 636c 6173 733d 2270 223e  <span class="p">
+0009f3c0: 2c3c 2f73 7061 6e3e 203c 7370 616e 2063  ,</span> <span c
+0009f3d0: 6c61 7373 3d22 6e22 3e64 6174 615f 7061  lass="n">data_pa
+0009f3e0: 7468 3c2f 7370 616e 3e3c 7370 616e 2063  th</span><span c
+0009f3f0: 6c61 7373 3d22 6f22 3e3d 3c2f 7370 616e  lass="o">=</span
+0009f400: 3e3c 7370 616e 2063 6c61 7373 3d22 6e22  ><span class="n"
+0009f410: 3e64 6174 615f 7061 7468 3c2f 7370 616e  >data_path</span
+0009f420: 3e3c 7370 616e 2063 6c61 7373 3d22 7022  ><span class="p"
+0009f430: 3e2c 3c2f 7370 616e 3e20 3c73 7061 6e20  >,</span> <span 
+0009f440: 636c 6173 733d 226e 223e 6f75 7466 6f72  class="n">outfor
+0009f450: 6d61 7473 3c2f 7370 616e 3e3c 7370 616e  mats</span><span
+0009f460: 2063 6c61 7373 3d22 6f22 3e3d 3c2f 7370   class="o">=</sp
+0009f470: 616e 3e3c 7370 616e 2063 6c61 7373 3d22  an><span class="
+0009f480: 7022 3e5b 3c2f 7370 616e 3e3c 7370 616e  p">[</span><span
+0009f490: 2063 6c61 7373 3d22 7331 223e 2623 3339   class="s1">&#39
+0009f4a0: 3b63 7376 2623 3339 3b3c 2f73 7061 6e3e  ;csv&#39;</span>
+0009f4b0: 3c73 7061 6e20 636c 6173 733d 2270 223e  <span class="p">
+0009f4c0: 2c3c 2f73 7061 6e3e 203c 7370 616e 2063  ,</span> <span c
+0009f4d0: 6c61 7373 3d22 7331 223e 2623 3339 3b70  lass="s1">&#39;p
+0009f4e0: 6172 7175 6574 2623 3339 3b3c 2f73 7061  arquet&#39;</spa
+0009f4f0: 6e3e 3c73 7061 6e20 636c 6173 733d 2270  n><span class="p
+0009f500: 223e 5d29 3c2f 7370 616e 3e0a 0a3c 7370  ">])</span>..<sp
+0009f510: 616e 2063 6c61 7373 3d22 6331 223e 2320  an class="c1"># 
+0009f520: 5265 6164 696e 673a 3c2f 7370 616e 3e0a  Reading:</span>.
+0009f530: 3c73 7061 6e20 636c 6173 733d 226e 223e  <span class="n">
+0009f540: 6466 3c2f 7370 616e 3e20 3c73 7061 6e20  df</span> <span 
+0009f550: 636c 6173 733d 226f 223e 3d3c 2f73 7061  class="o">=</spa
+0009f560: 6e3e 203c 7370 616e 2063 6c61 7373 3d22  n> <span class="
+0009f570: 6e22 3e72 6561 6444 6174 6173 6574 3c2f  n">readDataset</
+0009f580: 7370 616e 3e3c 7370 616e 2063 6c61 7373  span><span class
+0009f590: 3d22 7022 3e28 3c2f 7370 616e 3e3c 7370  ="p">(</span><sp
+0009f5a0: 616e 2063 6c61 7373 3d22 6e22 3e64 6174  an class="n">dat
+0009f5b0: 615f 7061 7468 3c2f 7370 616e 3e3c 7370  a_path</span><sp
+0009f5c0: 616e 2063 6c61 7373 3d22 7022 3e2c 3c2f  an class="p">,</
+0009f5d0: 7370 616e 3e20 3c73 7061 6e20 636c 6173  span> <span clas
+0009f5e0: 733d 226e 223e 6669 6c65 3c2f 7370 616e  s="n">file</span
+0009f5f0: 3e3c 7370 616e 2063 6c61 7373 3d22 6f22  ><span class="o"
+0009f600: 3e3d 3c2f 7370 616e 3e3c 7370 616e 2063  >=</span><span c
+0009f610: 6c61 7373 3d22 7331 223e 2623 3339 3b74  lass="s1">&#39;t
+0009f620: 7261 696e 2e70 6172 7175 6574 2623 3339  rain.parquet&#39
+0009f630: 3b3c 2f73 7061 6e3e 3c73 7061 6e20 636c  ;</span><span cl
+0009f640: 6173 733d 2270 223e 293c 2f73 7061 6e3e  ass="p">)</span>
+0009f650: 0a3c 7370 616e 2063 6c61 7373 3d22 6e22  .<span class="n"
+0009f660: 3e64 663c 2f73 7061 6e3e 3c73 7061 6e20  >df</span><span 
+0009f670: 636c 6173 733d 226f 223e 2e3c 2f73 7061  class="o">.</spa
+0009f680: 6e3e 3c73 7061 6e20 636c 6173 733d 226e  n><span class="n
+0009f690: 223e 6865 6164 3c2f 7370 616e 3e3c 7370  ">head</span><sp
+0009f6a0: 616e 2063 6c61 7373 3d22 7022 3e28 293c  an class="p">()<
+0009f6b0: 2f73 7061 6e3e 0a3c 2f70 7265 3e3c 2f64  /span>.</pre></d
+0009f6c0: 6976 3e0a 0a20 2020 2020 3c2f 6469 763e  iv>..     </div>
+0009f6d0: 0a3c 2f64 6976 3e0a 3c2f 6469 763e 0a3c  .</div>.</div>.<
+0009f6e0: 2f64 6976 3e0a 0a3c 6469 7620 636c 6173  /div>..<div clas
+0009f6f0: 733d 226a 702d 4365 6c6c 2d6f 7574 7075  s="jp-Cell-outpu
+0009f700: 7457 7261 7070 6572 223e 0a3c 6469 7620  tWrapper">.<div 
+0009f710: 636c 6173 733d 226a 702d 436f 6c6c 6170  class="jp-Collap
+0009f720: 7365 7220 6a70 2d4f 7574 7075 7443 6f6c  ser jp-OutputCol
+0009f730: 6c61 7073 6572 206a 702d 4365 6c6c 2d6f  lapser jp-Cell-o
+0009f740: 7574 7075 7443 6f6c 6c61 7073 6572 223e  utputCollapser">
+0009f750: 0a3c 2f64 6976 3e0a 0a0a 3c64 6976 2063  .</div>...<div c
+0009f760: 6c61 7373 3d22 6a70 2d4f 7574 7075 7441  lass="jp-OutputA
+0009f770: 7265 6120 6a70 2d43 656c 6c2d 6f75 7470  rea jp-Cell-outp
+0009f780: 7574 4172 6561 223e 0a0a 3c64 6976 2063  utArea">..<div c
+0009f790: 6c61 7373 3d22 6a70 2d4f 7574 7075 7441  lass="jp-OutputA
+0009f7a0: 7265 612d 6368 696c 6422 3e0a 0a20 2020  rea-child">..   
+0009f7b0: 200a 2020 2020 3c64 6976 2063 6c61 7373   .    <div class
+0009f7c0: 3d22 6a70 2d4f 7574 7075 7450 726f 6d70  ="jp-OutputPromp
+0009f7d0: 7420 6a70 2d4f 7574 7075 7441 7265 612d  t jp-OutputArea-
+0009f7e0: 7072 6f6d 7074 223e 3c2f 6469 763e 0a0a  prompt"></div>..
+0009f7f0: 0a0a 0a3c 6469 7620 636c 6173 733d 226a  ...<div class="j
+0009f800: 702d 5265 6e64 6572 6564 5465 7874 206a  p-RenderedText j
+0009f810: 702d 4f75 7470 7574 4172 6561 2d6f 7574  p-OutputArea-out
+0009f820: 7075 7420 2220 6461 7461 2d6d 696d 652d  put " data-mime-
+0009f830: 7479 7065 3d22 7465 7874 2f70 6c61 696e  type="text/plain
+0009f840: 223e 0a3c 7072 653e 2020 3025 7c20 2020  ">.<pre>  0%|   
+0009f850: 2020 2020 2020 207c 2030 2f39 205b 3030         | 0/9 [00
+0009f860: 3a30 3026 6c74 3b3f 2c20 3f69 742f 735d  :00&lt;?, ?it/s]
+0009f870: 3c2f 7072 653e 0a3c 2f64 6976 3e0a 0a3c  </pre>.</div>..<
+0009f880: 2f64 6976 3e0a 0a3c 6469 7620 636c 6173  /div>..<div clas
+0009f890: 733d 226a 702d 4f75 7470 7574 4172 6561  s="jp-OutputArea
+0009f8a0: 2d63 6869 6c64 223e 0a0a 2020 2020 0a20  -child">..    . 
+0009f8b0: 2020 203c 6469 7620 636c 6173 733d 226a     <div class="j
+0009f8c0: 702d 4f75 7470 7574 5072 6f6d 7074 206a  p-OutputPrompt j
+0009f8d0: 702d 4f75 7470 7574 4172 6561 2d70 726f  p-OutputArea-pro
+0009f8e0: 6d70 7422 3e3c 2f64 6976 3e0a 0a0a 3c64  mpt"></div>...<d
+0009f8f0: 6976 2063 6c61 7373 3d22 6a70 2d52 656e  iv class="jp-Ren
+0009f900: 6465 7265 6454 6578 7420 6a70 2d4f 7574  deredText jp-Out
+0009f910: 7075 7441 7265 612d 6f75 7470 7574 2220  putArea-output" 
+0009f920: 6461 7461 2d6d 696d 652d 7479 7065 3d22  data-mime-type="
+0009f930: 7465 7874 2f70 6c61 696e 223e 0a3c 7072  text/plain">.<pr
+0009f940: 653e 5772 6974 696e 6720 2d20 4353 5620  e>Writing - CSV 
+0009f950: 7c54 5241 494e 202d 200a 5772 6974 696e  |TRAIN - .Writin
+0009f960: 6720 2d20 4353 5620 7c54 4553 5420 2d20  g - CSV |TEST - 
+0009f970: 0a57 7269 7469 6e67 202d 2050 6172 7175  .Writing - Parqu
+0009f980: 6574 207c 5452 4149 4e20 2d20 0a57 7269  et |TRAIN - .Wri
+0009f990: 7469 6e67 202d 2050 6172 7175 6574 207c  ting - Parquet |
+0009f9a0: 5445 5354 202d 200a 3c2f 7072 653e 0a3c  TEST - .</pre>.<
+0009f9b0: 2f64 6976 3e0a 3c2f 6469 763e 0a0a 3c64  /div>.</div>..<d
+0009f9c0: 6976 2063 6c61 7373 3d22 6a70 2d4f 7574  iv class="jp-Out
+0009f9d0: 7075 7441 7265 612d 6368 696c 6422 3e0a  putArea-child">.
+0009f9e0: 0a20 2020 200a 2020 2020 3c64 6976 2063  .    .    <div c
+0009f9f0: 6c61 7373 3d22 6a70 2d4f 7574 7075 7450  lass="jp-OutputP
+0009fa00: 726f 6d70 7420 6a70 2d4f 7574 7075 7441  rompt jp-OutputA
+0009fa10: 7265 612d 7072 6f6d 7074 223e 4f75 745b  rea-prompt">Out[
+0009fa20: 3234 5d3a 3c2f 6469 763e 0a0a 0a0a 3c64  24]:</div>....<d
+0009fa30: 6976 2063 6c61 7373 3d22 6a70 2d52 656e  iv class="jp-Ren
+0009fa40: 6465 7265 6448 544d 4c43 6f6d 6d6f 6e20  deredHTMLCommon 
+0009fa50: 6a70 2d52 656e 6465 7265 6448 544d 4c20  jp-RenderedHTML 
+0009fa60: 6a70 2d4f 7574 7075 7441 7265 612d 6f75  jp-OutputArea-ou
+0009fa70: 7470 7574 206a 702d 4f75 7470 7574 4172  tput jp-OutputAr
+0009fa80: 6561 2d65 7865 6375 7465 5265 7375 6c74  ea-executeResult
+0009fa90: 2220 6461 7461 2d6d 696d 652d 7479 7065  " data-mime-type
+0009faa0: 3d22 7465 7874 2f68 746d 6c22 3e0a 3c64  ="text/html">.<d
+0009fab0: 6976 3e0a 3c73 7479 6c65 2073 636f 7065  iv>.<style scope
+0009fac0: 643e 0a20 2020 202e 6461 7461 6672 616d  d>.    .datafram
+0009fad0: 6520 7462 6f64 7920 7472 2074 683a 6f6e  e tbody tr th:on
+0009fae0: 6c79 2d6f 662d 7479 7065 207b 0a20 2020  ly-of-type {.   
+0009faf0: 2020 2020 2076 6572 7469 6361 6c2d 616c       vertical-al
+0009fb00: 6967 6e3a 206d 6964 646c 653b 0a20 2020  ign: middle;.   
+0009fb10: 207d 0a0a 2020 2020 2e64 6174 6166 7261   }..    .datafra
+0009fb20: 6d65 2074 626f 6479 2074 7220 7468 207b  me tbody tr th {
+0009fb30: 0a20 2020 2020 2020 2076 6572 7469 6361  .        vertica
+0009fb40: 6c2d 616c 6967 6e3a 2074 6f70 3b0a 2020  l-align: top;.  
+0009fb50: 2020 7d0a 0a20 2020 202e 6461 7461 6672    }..    .datafr
+0009fb60: 616d 6520 7468 6561 6420 7468 207b 0a20  ame thead th {. 
+0009fb70: 2020 2020 2020 2074 6578 742d 616c 6967         text-alig
+0009fb80: 6e3a 2072 6967 6874 3b0a 2020 2020 7d0a  n: right;.    }.
+0009fb90: 3c2f 7374 796c 653e 0a3c 7461 626c 6520  </style>.<table 
+0009fba0: 626f 7264 6572 3d22 3122 2063 6c61 7373  border="1" class
+0009fbb0: 3d22 6461 7461 6672 616d 6522 3e0a 2020  ="dataframe">.  
+0009fbc0: 3c74 6865 6164 3e0a 2020 2020 3c74 7220  <thead>.    <tr 
+0009fbd0: 7374 796c 653d 2274 6578 742d 616c 6967  style="text-alig
+0009fbe0: 6e3a 2072 6967 6874 3b22 3e0a 2020 2020  n: right;">.    
+0009fbf0: 2020 3c74 683e 3c2f 7468 3e0a 2020 2020    <th></th>.    
+0009fc00: 2020 3c74 683e 6461 7465 5f74 696d 653c    <th>date_time<
+0009fc10: 2f74 683e 0a20 2020 2020 203c 7468 3e74  /th>.      <th>t
+0009fc20: 696d 653c 2f74 683e 0a20 2020 2020 203c  ime</th>.      <
+0009fc30: 7468 3e72 6174 696e 673c 2f74 683e 0a20  th>rating</th>. 
+0009fc40: 2020 2020 203c 7468 3e70 7269 6365 3c2f       <th>price</
+0009fc50: 7468 3e0a 2020 2020 2020 3c74 683e 7765  th>.      <th>we
+0009fc60: 6174 6865 723c 2f74 683e 0a20 2020 2020  ather</th>.     
+0009fc70: 203c 7468 3e64 6179 3c2f 7468 3e0a 2020   <th>day</th>.  
+0009fc80: 2020 2020 3c74 683e 7479 7065 3c2f 7468      <th>type</th
+0009fc90: 3e0a 2020 2020 2020 3c74 683e 6c61 743c  >.      <th>lat<
+0009fca0: 2f74 683e 0a20 2020 2020 203c 7468 3e6c  /th>.      <th>l
+0009fcb0: 6f6e 3c2f 7468 3e0a 2020 2020 2020 3c74  on</th>.      <t
+0009fcc0: 683e 7469 643c 2f74 683e 0a20 2020 2020  h>tid</th>.     
+0009fcd0: 203c 7468 3e6c 6162 656c 3c2f 7468 3e0a   <th>label</th>.
+0009fce0: 2020 2020 3c2f 7472 3e0a 2020 3c2f 7468      </tr>.  </th
+0009fcf0: 6561 643e 0a20 203c 7462 6f64 793e 0a20  ead>.  <tbody>. 
+0009fd00: 2020 203c 7472 3e0a 2020 2020 2020 3c74     <tr>.      <t
+0009fd10: 683e 303c 2f74 683e 0a20 2020 2020 203c  h>0</th>.      <
+0009fd20: 7464 3e32 3031 322d 3131 2d31 3220 3035  td>2012-11-12 05
+0009fd30: 3a31 373a 3138 3c2f 7464 3e0a 2020 2020  :17:18</td>.    
+0009fd40: 2020 3c74 643e 3331 373c 2f74 643e 0a20    <td>317</td>. 
+0009fd50: 2020 2020 203c 7464 3e2d 312e 303c 2f74       <td>-1.0</t
+0009fd60: 643e 0a20 2020 2020 203c 7464 3e2d 313c  d>.      <td>-1<
+0009fd70: 2f74 643e 0a20 2020 2020 203c 7464 3e43  /td>.      <td>C
+0009fd80: 6c65 6172 3c2f 7464 3e0a 2020 2020 2020  lear</td>.      
+0009fd90: 3c74 643e 4d6f 6e64 6179 3c2f 7464 3e0a  <td>Monday</td>.
+0009fda0: 2020 2020 2020 3c74 643e 486f 6d65 2028        <td>Home (
+0009fdb0: 7072 6976 6174 6529 3c2f 7464 3e0a 2020  private)</td>.  
+0009fdc0: 2020 2020 3c74 643e 3430 2e38 3333 3136      <td>40.83316
+0009fdd0: 353c 2f74 643e 0a20 2020 2020 203c 7464  5</td>.      <td
+0009fde0: 3e2d 3733 2e39 3431 3836 303c 2f74 643e  >-73.941860</td>
+0009fdf0: 0a20 2020 2020 203c 7464 3e31 3236 3c2f  .      <td>126</
+0009fe00: 7464 3e0a 2020 2020 2020 3c74 643e 5265  td>.      <td>Re
+0009fe10: 7369 6465 6e63 653c 2f74 643e 0a20 2020  sidence</td>.   
+0009fe20: 203c 2f74 723e 0a20 2020 203c 7472 3e0a   </tr>.    <tr>.
+0009fe30: 2020 2020 2020 3c74 683e 313c 2f74 683e        <th>1</th>
+0009fe40: 0a20 2020 2020 203c 7464 3e32 3031 322d  .      <td>2012-
+0009fe50: 3131 2d31 3220 3233 3a32 343a 3535 3c2f  11-12 23:24:55</
+0009fe60: 7464 3e0a 2020 2020 2020 3c74 643e 3134  td>.      <td>14
+0009fe70: 3034 3c2f 7464 3e0a 2020 2020 2020 3c74  04</td>.      <t
+0009fe80: 643e 382e 323c 2f74 643e 0a20 2020 2020  d>8.2</td>.     
+0009fe90: 203c 7464 3e31 3c2f 7464 3e0a 2020 2020   <td>1</td>.    
+0009fea0: 2020 3c74 643e 436c 6f75 6473 3c2f 7464    <td>Clouds</td
+0009feb0: 3e0a 2020 2020 2020 3c74 643e 4d6f 6e64  >.      <td>Mond
+0009fec0: 6179 3c2f 7464 3e0a 2020 2020 2020 3c74  ay</td>.      <t
+0009fed0: 643e 4465 6c69 202f 2042 6f64 6567 613c  d>Deli / Bodega<
+0009fee0: 2f74 643e 0a20 2020 2020 203c 7464 3e34  /td>.      <td>4
+0009fef0: 302e 3833 3430 3938 3c2f 7464 3e0a 2020  0.834098</td>.  
+0009ff00: 2020 2020 3c74 643e 2d37 332e 3934 3532      <td>-73.9452
+0009ff10: 3637 3c2f 7464 3e0a 2020 2020 2020 3c74  67</td>.      <t
+0009ff20: 643e 3132 363c 2f74 643e 0a20 2020 2020  d>126</td>.     
+0009ff30: 203c 7464 3e46 6f6f 643c 2f74 643e 0a20   <td>Food</td>. 
+0009ff40: 2020 203c 2f74 723e 0a20 2020 203c 7472     </tr>.    <tr
+0009ff50: 3e0a 2020 2020 2020 3c74 683e 323c 2f74  >.      <th>2</t
+0009ff60: 683e 0a20 2020 2020 203c 7464 3e32 3031  h>.      <td>201
+0009ff70: 322d 3131 2d31 3320 3030 3a30 303a 3037  2-11-13 00:00:07
+0009ff80: 3c2f 7464 3e0a 2020 2020 2020 3c74 643e  </td>.      <td>
+0009ff90: 303c 2f74 643e 0a20 2020 2020 203c 7464  0</td>.      <td
+0009ffa0: 3e2d 312e 303c 2f74 643e 0a20 2020 2020  >-1.0</td>.     
+0009ffb0: 203c 7464 3e2d 313c 2f74 643e 0a20 2020   <td>-1</td>.   
+0009ffc0: 2020 203c 7464 3e43 6c6f 7564 733c 2f74     <td>Clouds</t
+0009ffd0: 643e 0a20 2020 2020 203c 7464 3e54 7565  d>.      <td>Tue
+0009ffe0: 7364 6179 3c2f 7464 3e0a 2020 2020 2020  sday</td>.      
+0009fff0: 3c74 643e 486f 6d65 2028 7072 6976 6174  <td>Home (privat
+000a0000: 6529 3c2f 7464 3e0a 2020 2020 2020 3c74  e)</td>.      <t
+000a0010: 643e 3430 2e38 3333 3136 353c 2f74 643e  d>40.833165</td>
+000a0020: 0a20 2020 2020 203c 7464 3e2d 3733 2e39  .      <td>-73.9
+000a0030: 3431 3836 303c 2f74 643e 0a20 2020 2020  41860</td>.     
+000a0040: 203c 7464 3e31 3236 3c2f 7464 3e0a 2020   <td>126</td>.  
+000a0050: 2020 2020 3c74 643e 5265 7369 6465 6e63      <td>Residenc
+000a0060: 653c 2f74 643e 0a20 2020 203c 2f74 723e  e</td>.    </tr>
+000a0070: 0a20 2020 203c 7472 3e0a 2020 2020 2020  .    <tr>.      
+000a0080: 3c74 683e 333c 2f74 683e 0a20 2020 2020  <th>3</th>.     
+000a0090: 203c 7464 3e32 3031 322d 3131 2d31 3520   <td>2012-11-15 
+000a00a0: 3137 3a34 393a 3031 3c2f 7464 3e0a 2020  17:49:01</td>.  
+000a00b0: 2020 2020 3c74 643e 3130 3639 3c2f 7464      <td>1069</td
+000a00c0: 3e0a 2020 2020 2020 3c74 643e 362e 363c  >.      <td>6.6<
+000a00d0: 2f74 643e 0a20 2020 2020 203c 7464 3e33  /td>.      <td>3
+000a00e0: 3c2f 7464 3e0a 2020 2020 2020 3c74 643e  </td>.      <td>
+000a00f0: 436c 6561 723c 2f74 643e 0a20 2020 2020  Clear</td>.     
+000a0100: 203c 7464 3e54 6875 7273 6461 793c 2f74   <td>Thursday</t
+000a0110: 643e 0a20 2020 2020 203c 7464 3e46 7269  d>.      <td>Fri
+000a0120: 6564 2043 6869 636b 656e 204a 6f69 6e74  ed Chicken Joint
+000a0130: 3c2f 7464 3e0a 2020 2020 2020 3c74 643e  </td>.      <td>
+000a0140: 3430 2e37 3634 3639 363c 2f74 643e 0a20  40.764696</td>. 
+000a0150: 2020 2020 203c 7464 3e2d 3733 2e38 3835       <td>-73.885
+000a0160: 3139 373c 2f74 643e 0a20 2020 2020 203c  197</td>.      <
+000a0170: 7464 3e31 3236 3c2f 7464 3e0a 2020 2020  td>126</td>.    
+000a0180: 2020 3c74 643e 466f 6f64 3c2f 7464 3e0a    <td>Food</td>.
+000a0190: 2020 2020 3c2f 7472 3e0a 2020 2020 3c74      </tr>.    <t
+000a01a0: 723e 0a20 2020 2020 203c 7468 3e34 3c2f  r>.      <th>4</
+000a01b0: 7468 3e0a 2020 2020 2020 3c74 643e 3230  th>.      <td>20
+000a01c0: 3132 2d31 312d 3135 2031 383a 3430 3a31  12-11-15 18:40:1
+000a01d0: 363c 2f74 643e 0a20 2020 2020 203c 7464  6</td>.      <td
+000a01e0: 3e31 3132 303c 2f74 643e 0a20 2020 2020  >1120</td>.     
+000a01f0: 203c 7464 3e2d 312e 303c 2f74 643e 0a20   <td>-1.0</td>. 
+000a0200: 2020 2020 203c 7464 3e2d 313c 2f74 643e       <td>-1</td>
+000a0210: 0a20 2020 2020 203c 7464 3e43 6c65 6172  .      <td>Clear
+000a0220: 3c2f 7464 3e0a 2020 2020 2020 3c74 643e  </td>.      <td>
+000a0230: 5468 7572 7364 6179 3c2f 7464 3e0a 2020  Thursday</td>.  
+000a0240: 2020 2020 3c74 643e 4275 7320 5374 6174      <td>Bus Stat
+000a0250: 696f 6e3c 2f74 643e 0a20 2020 2020 203c  ion</td>.      <
+000a0260: 7464 3e34 302e 3736 3630 3739 3c2f 7464  td>40.766079</td
+000a0270: 3e0a 2020 2020 2020 3c74 643e 2d37 332e  >.      <td>-73.
+000a0280: 3838 3335 3239 3c2f 7464 3e0a 2020 2020  883529</td>.    
+000a0290: 2020 3c74 643e 3132 363c 2f74 643e 0a20    <td>126</td>. 
+000a02a0: 2020 2020 203c 7464 3e54 7261 7665 6c20       <td>Travel 
+000a02b0: 2661 6d70 3b20 5472 616e 7370 6f72 743c  &amp; Transport<
+000a02c0: 2f74 643e 0a20 2020 203c 2f74 723e 0a20  /td>.    </tr>. 
+000a02d0: 203c 2f74 626f 6479 3e0a 3c2f 7461 626c   </tbody>.</tabl
+000a02e0: 653e 0a3c 2f64 6976 3e0a 3c2f 6469 763e  e>.</div>.</div>
+000a02f0: 0a0a 3c2f 6469 763e 0a0a 3c2f 6469 763e  ..</div>..</div>
+000a0300: 0a0a 3c2f 6469 763e 0a0a 3c2f 6469 763e  ..</div>..</div>
+000a0310: 0a3c 6469 7620 636c 6173 733d 226a 702d  .<div class="jp-
+000a0320: 4365 6c6c 206a 702d 4d61 726b 646f 776e  Cell jp-Markdown
+000a0330: 4365 6c6c 206a 702d 4e6f 7465 626f 6f6b  Cell jp-Notebook
+000a0340: 2d63 656c 6c22 3e0a 3c64 6976 2063 6c61  -cell">.<div cla
+000a0350: 7373 3d22 6a70 2d43 656c 6c2d 696e 7075  ss="jp-Cell-inpu
+000a0360: 7457 7261 7070 6572 223e 0a3c 6469 7620  tWrapper">.<div 
+000a0370: 636c 6173 733d 226a 702d 436f 6c6c 6170  class="jp-Collap
+000a0380: 7365 7220 6a70 2d49 6e70 7574 436f 6c6c  ser jp-InputColl
+000a0390: 6170 7365 7220 6a70 2d43 656c 6c2d 696e  apser jp-Cell-in
+000a03a0: 7075 7443 6f6c 6c61 7073 6572 223e 0a3c  putCollapser">.<
+000a03b0: 2f64 6976 3e0a 3c64 6976 2063 6c61 7373  /div>.<div class
+000a03c0: 3d22 6a70 2d49 6e70 7574 4172 6561 206a  ="jp-InputArea j
+000a03d0: 702d 4365 6c6c 2d69 6e70 7574 4172 6561  p-Cell-inputArea
+000a03e0: 223e 3c64 6976 2063 6c61 7373 3d22 6a70  "><div class="jp
+000a03f0: 2d49 6e70 7574 5072 6f6d 7074 206a 702d  -InputPrompt jp-
+000a0400: 496e 7075 7441 7265 612d 7072 6f6d 7074  InputArea-prompt
+000a0410: 223e 0a3c 2f64 6976 3e3c 6469 7620 636c  ">.</div><div cl
+000a0420: 6173 733d 226a 702d 5265 6e64 6572 6564  ass="jp-Rendered
+000a0430: 4854 4d4c 436f 6d6d 6f6e 206a 702d 5265  HTMLCommon jp-Re
+000a0440: 6e64 6572 6564 4d61 726b 646f 776e 206a  nderedMarkdown j
+000a0450: 702d 4d61 726b 646f 776e 4f75 7470 7574  p-MarkdownOutput
+000a0460: 2022 2064 6174 612d 6d69 6d65 2d74 7970   " data-mime-typ
+000a0470: 653d 2274 6578 742f 6d61 726b 646f 776e  e="text/markdown
+000a0480: 223e 0a3c 703e 546f 206b 2d66 6f6c 6420  ">.<p>To k-fold 
+000a0490: 7370 6c69 7420 6120 6461 7461 7365 7420  split a dataset 
+000a04a0: 696e 746f 2074 7261 696e 2061 6e64 2074  into train and t
+000a04b0: 6573 743a 3c2f 703e 0a0a 3c2f 6469 763e  est:</p>..</div>
+000a04c0: 0a3c 2f64 6976 3e0a 3c2f 6469 763e 0a3c  .</div>.</div>.<
+000a04d0: 2f64 6976 3e3c 6469 7620 636c 6173 733d  /div><div class=
+000a04e0: 226a 702d 4365 6c6c 206a 702d 436f 6465  "jp-Cell jp-Code
+000a04f0: 4365 6c6c 206a 702d 4e6f 7465 626f 6f6b  Cell jp-Notebook
+000a0500: 2d63 656c 6c20 2020 223e 0a3c 6469 7620  -cell   ">.<div 
+000a0510: 636c 6173 733d 226a 702d 4365 6c6c 2d69  class="jp-Cell-i
+000a0520: 6e70 7574 5772 6170 7065 7222 3e0a 3c64  nputWrapper">.<d
+000a0530: 6976 2063 6c61 7373 3d22 6a70 2d43 6f6c  iv class="jp-Col
+000a0540: 6c61 7073 6572 206a 702d 496e 7075 7443  lapser jp-InputC
+000a0550: 6f6c 6c61 7073 6572 206a 702d 4365 6c6c  ollapser jp-Cell
+000a0560: 2d69 6e70 7574 436f 6c6c 6170 7365 7222  -inputCollapser"
+000a0570: 3e0a 3c2f 6469 763e 0a3c 6469 7620 636c  >.</div>.<div cl
+000a0580: 6173 733d 226a 702d 496e 7075 7441 7265  ass="jp-InputAre
+000a0590: 6120 6a70 2d43 656c 6c2d 696e 7075 7441  a jp-Cell-inputA
+000a05a0: 7265 6122 3e0a 3c64 6976 2063 6c61 7373  rea">.<div class
+000a05b0: 3d22 6a70 2d49 6e70 7574 5072 6f6d 7074  ="jp-InputPrompt
+000a05c0: 206a 702d 496e 7075 7441 7265 612d 7072   jp-InputArea-pr
+000a05d0: 6f6d 7074 223e 496e 266e 6273 703b 5b32  ompt">In&nbsp;[2
+000a05e0: 355d 3a3c 2f64 6976 3e0a 3c64 6976 2063  5]:</div>.<div c
+000a05f0: 6c61 7373 3d22 6a70 2d43 6f64 654d 6972  lass="jp-CodeMir
+000a0600: 726f 7245 6469 746f 7220 6a70 2d45 6469  rorEditor jp-Edi
+000a0610: 746f 7220 6a70 2d49 6e70 7574 4172 6561  tor jp-InputArea
+000a0620: 2d65 6469 746f 7222 2064 6174 612d 7479  -editor" data-ty
+000a0630: 7065 3d22 696e 6c69 6e65 223e 0a20 2020  pe="inline">.   
+000a0640: 2020 3c64 6976 2063 6c61 7373 3d22 436f    <div class="Co
+000a0650: 6465 4d69 7272 6f72 2063 6d2d 732d 6a75  deMirror cm-s-ju
+000a0660: 7079 7465 7222 3e0a 3c64 6976 2063 6c61  pyter">.<div cla
+000a0670: 7373 3d22 2068 6967 686c 6967 6874 2068  ss=" highlight h
+000a0680: 6c2d 6970 7974 686f 6e33 223e 3c70 7265  l-ipython3"><pre
+000a0690: 3e3c 7370 616e 3e3c 2f73 7061 6e3e 3c73  ><span></span><s
+000a06a0: 7061 6e20 636c 6173 733d 226e 223e 7472  pan class="n">tr
+000a06b0: 6169 6e3c 2f73 7061 6e3e 3c73 7061 6e20  ain</span><span 
+000a06c0: 636c 6173 733d 2270 223e 2c3c 2f73 7061  class="p">,</spa
+000a06d0: 6e3e 203c 7370 616e 2063 6c61 7373 3d22  n> <span class="
+000a06e0: 6e22 3e74 6573 743c 2f73 7061 6e3e 203c  n">test</span> <
+000a06f0: 7370 616e 2063 6c61 7373 3d22 6f22 3e3d  span class="o">=
+000a0700: 3c2f 7370 616e 3e20 3c73 7061 6e20 636c  </span> <span cl
+000a0710: 6173 733d 226e 223e 6b66 6f6c 645f 7472  ass="n">kfold_tr
+000a0720: 6169 6e54 6573 7453 706c 6974 3c2f 7370  ainTestSplit</sp
+000a0730: 616e 3e3c 7370 616e 2063 6c61 7373 3d22  an><span class="
+000a0740: 7022 3e28 3c2f 7370 616e 3e3c 7370 616e  p">(</span><span
+000a0750: 2063 6c61 7373 3d22 6e22 3e64 663c 2f73   class="n">df</s
+000a0760: 7061 6e3e 3c73 7061 6e20 636c 6173 733d  pan><span class=
+000a0770: 2270 223e 2c3c 2f73 7061 6e3e 203c 7370  "p">,</span> <sp
+000a0780: 616e 2063 6c61 7373 3d22 6e22 3e6b 3c2f  an class="n">k</
+000a0790: 7370 616e 3e3c 7370 616e 2063 6c61 7373  span><span class
+000a07a0: 3d22 6f22 3e3d 3c2f 7370 616e 3e3c 7370  ="o">=</span><sp
+000a07b0: 616e 2063 6c61 7373 3d22 6d69 223e 333c  an class="mi">3<
+000a07c0: 2f73 7061 6e3e 3c73 7061 6e20 636c 6173  /span><span clas
+000a07d0: 733d 2270 223e 293c 2f73 7061 6e3e 0a0a  s="p">)</span>..
+000a07e0: 3c73 7061 6e20 636c 6173 733d 226b 223e  <span class="k">
+000a07f0: 666f 723c 2f73 7061 6e3e 203c 7370 616e  for</span> <span
+000a0800: 2063 6c61 7373 3d22 6e22 3e6b 3c2f 7370   class="n">k</sp
+000a0810: 616e 3e20 3c73 7061 6e20 636c 6173 733d  an> <span class=
+000a0820: 226f 7722 3e69 6e3c 2f73 7061 6e3e 203c  "ow">in</span> <
+000a0830: 7370 616e 2063 6c61 7373 3d22 6e62 223e  span class="nb">
+000a0840: 7261 6e67 653c 2f73 7061 6e3e 3c73 7061  range</span><spa
+000a0850: 6e20 636c 6173 733d 2270 223e 283c 2f73  n class="p">(</s
+000a0860: 7061 6e3e 3c73 7061 6e20 636c 6173 733d  pan><span class=
+000a0870: 226e 6222 3e6c 656e 3c2f 7370 616e 3e3c  "nb">len</span><
+000a0880: 7370 616e 2063 6c61 7373 3d22 7022 3e28  span class="p">(
+000a0890: 3c2f 7370 616e 3e3c 7370 616e 2063 6c61  </span><span cla
+000a08a0: 7373 3d22 6e22 3e74 7261 696e 3c2f 7370  ss="n">train</sp
+000a08b0: 616e 3e3c 7370 616e 2063 6c61 7373 3d22  an><span class="
+000a08c0: 7022 3e29 293a 3c2f 7370 616e 3e0a 2020  p">)):</span>.  
+000a08d0: 2020 3c73 7061 6e20 636c 6173 733d 226e    <span class="n
+000a08e0: 6222 3e70 7269 6e74 3c2f 7370 616e 3e3c  b">print</span><
+000a08f0: 7370 616e 2063 6c61 7373 3d22 7022 3e28  span class="p">(
+000a0900: 3c2f 7370 616e 3e3c 7370 616e 2063 6c61  </span><span cla
+000a0910: 7373 3d22 7331 223e 2623 3339 3b53 6861  ss="s1">&#39;Sha
+000a0920: 7065 2074 7261 696e 2f74 6573 743a 2623  pe train/test:&#
+000a0930: 3339 3b3c 2f73 7061 6e3e 3c73 7061 6e20  39;</span><span 
+000a0940: 636c 6173 733d 2270 223e 2c3c 2f73 7061  class="p">,</spa
+000a0950: 6e3e 203c 7370 616e 2063 6c61 7373 3d22  n> <span class="
+000a0960: 6e22 3e74 7261 696e 3c2f 7370 616e 3e3c  n">train</span><
+000a0970: 7370 616e 2063 6c61 7373 3d22 7022 3e5b  span class="p">[
+000a0980: 3c2f 7370 616e 3e3c 7370 616e 2063 6c61  </span><span cla
+000a0990: 7373 3d22 6e22 3e6b 3c2f 7370 616e 3e3c  ss="n">k</span><
+000a09a0: 7370 616e 2063 6c61 7373 3d22 7022 3e5d  span class="p">]
+000a09b0: 3c2f 7370 616e 3e3c 7370 616e 2063 6c61  </span><span cla
+000a09c0: 7373 3d22 6f22 3e2e 3c2f 7370 616e 3e3c  ss="o">.</span><
+000a09d0: 7370 616e 2063 6c61 7373 3d22 6e22 3e73  span class="n">s
+000a09e0: 6861 7065 3c2f 7370 616e 3e3c 7370 616e  hape</span><span
+000a09f0: 2063 6c61 7373 3d22 7022 3e2c 3c2f 7370   class="p">,</sp
+000a0a00: 616e 3e20 3c73 7061 6e20 636c 6173 733d  an> <span class=
+000a0a10: 226e 223e 7465 7374 3c2f 7370 616e 3e3c  "n">test</span><
+000a0a20: 7370 616e 2063 6c61 7373 3d22 7022 3e5b  span class="p">[
+000a0a30: 3c2f 7370 616e 3e3c 7370 616e 2063 6c61  </span><span cla
+000a0a40: 7373 3d22 6e22 3e6b 3c2f 7370 616e 3e3c  ss="n">k</span><
+000a0a50: 7370 616e 2063 6c61 7373 3d22 7022 3e5d  span class="p">]
+000a0a60: 3c2f 7370 616e 3e3c 7370 616e 2063 6c61  </span><span cla
+000a0a70: 7373 3d22 6f22 3e2e 3c2f 7370 616e 3e3c  ss="o">.</span><
+000a0a80: 7370 616e 2063 6c61 7373 3d22 6e22 3e73  span class="n">s
+000a0a90: 6861 7065 3c2f 7370 616e 3e3c 7370 616e  hape</span><span
+000a0aa0: 2063 6c61 7373 3d22 7022 3e29 3c2f 7370   class="p">)</sp
+000a0ab0: 616e 3e0a 3c2f 7072 653e 3c2f 6469 763e  an>.</pre></div>
+000a0ac0: 0a0a 2020 2020 203c 2f64 6976 3e0a 3c2f  ..     </div>.</
+000a0ad0: 6469 763e 0a3c 2f64 6976 3e0a 3c2f 6469  div>.</div>.</di
+000a0ae0: 763e 0a0a 3c64 6976 2063 6c61 7373 3d22  v>..<div class="
+000a0af0: 6a70 2d43 656c 6c2d 6f75 7470 7574 5772  jp-Cell-outputWr
+000a0b00: 6170 7065 7222 3e0a 3c64 6976 2063 6c61  apper">.<div cla
+000a0b10: 7373 3d22 6a70 2d43 6f6c 6c61 7073 6572  ss="jp-Collapser
+000a0b20: 206a 702d 4f75 7470 7574 436f 6c6c 6170   jp-OutputCollap
+000a0b30: 7365 7220 6a70 2d43 656c 6c2d 6f75 7470  ser jp-Cell-outp
+000a0b40: 7574 436f 6c6c 6170 7365 7222 3e0a 3c2f  utCollapser">.</
+000a0b50: 6469 763e 0a0a 0a3c 6469 7620 636c 6173  div>...<div clas
+000a0b60: 733d 226a 702d 4f75 7470 7574 4172 6561  s="jp-OutputArea
+000a0b70: 206a 702d 4365 6c6c 2d6f 7574 7075 7441   jp-Cell-outputA
+000a0b80: 7265 6122 3e0a 0a3c 6469 7620 636c 6173  rea">..<div clas
+000a0b90: 733d 226a 702d 4f75 7470 7574 4172 6561  s="jp-OutputArea
+000a0ba0: 2d63 6869 6c64 223e 0a0a 2020 2020 0a20  -child">..    . 
+000a0bb0: 2020 203c 6469 7620 636c 6173 733d 226a     <div class="j
+000a0bc0: 702d 4f75 7470 7574 5072 6f6d 7074 206a  p-OutputPrompt j
+000a0bd0: 702d 4f75 7470 7574 4172 6561 2d70 726f  p-OutputArea-pro
+000a0be0: 6d70 7422 3e3c 2f64 6976 3e0a 0a0a 0a0a  mpt"></div>.....
+000a0bf0: 3c64 6976 2063 6c61 7373 3d22 6a70 2d52  <div class="jp-R
+000a0c00: 656e 6465 7265 6454 6578 7420 6a70 2d4f  enderedText jp-O
+000a0c10: 7574 7075 7441 7265 612d 6f75 7470 7574  utputArea-output
+000a0c20: 2022 2064 6174 612d 6d69 6d65 2d74 7970   " data-mime-typ
+000a0c30: 653d 2274 6578 742f 706c 6169 6e22 3e0a  e="text/plain">.
+000a0c40: 3c70 7265 3e53 706c 6974 696e 6720 4461  <pre>Spliting Da
+000a0c50: 7461 3a20 2020 3025 7c20 2020 2020 2020  ta:   0%|       
+000a0c60: 2020 207c 2030 2f31 3020 5b30 303a 3030     | 0/10 [00:00
+000a0c70: 266c 743b 3f2c 203f 6974 2f73 5d3c 2f70  &lt;?, ?it/s]</p
+000a0c80: 7265 3e0a 3c2f 6469 763e 0a0a 3c2f 6469  re>.</div>..</di
+000a0c90: 763e 0a0a 3c64 6976 2063 6c61 7373 3d22  v>..<div class="
+000a0ca0: 6a70 2d4f 7574 7075 7441 7265 612d 6368  jp-OutputArea-ch
+000a0cb0: 696c 6422 3e0a 0a20 2020 200a 2020 2020  ild">..    .    
+000a0cc0: 3c64 6976 2063 6c61 7373 3d22 6a70 2d4f  <div class="jp-O
+000a0cd0: 7574 7075 7450 726f 6d70 7420 6a70 2d4f  utputPrompt jp-O
+000a0ce0: 7574 7075 7441 7265 612d 7072 6f6d 7074  utputArea-prompt
+000a0cf0: 223e 3c2f 6469 763e 0a0a 0a3c 6469 7620  "></div>...<div 
+000a0d00: 636c 6173 733d 226a 702d 5265 6e64 6572  class="jp-Render
+000a0d10: 6564 5465 7874 206a 702d 4f75 7470 7574  edText jp-Output
+000a0d20: 4172 6561 2d6f 7574 7075 7422 2064 6174  Area-output" dat
+000a0d30: 612d 6d69 6d65 2d74 7970 653d 2274 6578  a-mime-type="tex
+000a0d40: 742f 706c 6169 6e22 3e0a 3c70 7265 3e53  t/plain">.<pre>S
+000a0d50: 6861 7065 2074 7261 696e 2f74 6573 743a  hape train/test:
+000a0d60: 2028 3137 3436 3336 2c20 3131 2920 2838   (174636, 11) (8
+000a0d70: 3639 3639 2c20 3131 290a 5368 6170 6520  6969, 11).Shape 
+000a0d80: 7472 6169 6e2f 7465 7374 3a20 2831 3735  train/test: (175
+000a0d90: 3731 352c 2031 3129 2028 3835 3839 302c  715, 11) (85890,
+000a0da0: 2031 3129 0a53 6861 7065 2074 7261 696e   11).Shape train
+000a0db0: 2f74 6573 743a 2028 3137 3238 3539 2c20  /test: (172859, 
+000a0dc0: 3131 2920 2838 3837 3436 2c20 3131 290a  11) (88746, 11).
+000a0dd0: 3c2f 7072 653e 0a3c 2f64 6976 3e0a 3c2f  </pre>.</div>.</
+000a0de0: 6469 763e 0a0a 3c2f 6469 763e 0a0a 3c2f  div>..</div>..</
+000a0df0: 6469 763e 0a0a 3c2f 6469 763e 0a3c 6469  div>..</div>.<di
+000a0e00: 7620 636c 6173 733d 226a 702d 4365 6c6c  v class="jp-Cell
+000a0e10: 206a 702d 4d61 726b 646f 776e 4365 6c6c   jp-MarkdownCell
+000a0e20: 206a 702d 4e6f 7465 626f 6f6b 2d63 656c   jp-Notebook-cel
+000a0e30: 6c22 3e0a 3c64 6976 2063 6c61 7373 3d22  l">.<div class="
+000a0e40: 6a70 2d43 656c 6c2d 696e 7075 7457 7261  jp-Cell-inputWra
+000a0e50: 7070 6572 223e 0a3c 6469 7620 636c 6173  pper">.<div clas
+000a0e60: 733d 226a 702d 436f 6c6c 6170 7365 7220  s="jp-Collapser 
+000a0e70: 6a70 2d49 6e70 7574 436f 6c6c 6170 7365  jp-InputCollapse
+000a0e80: 7220 6a70 2d43 656c 6c2d 696e 7075 7443  r jp-Cell-inputC
+000a0e90: 6f6c 6c61 7073 6572 223e 0a3c 2f64 6976  ollapser">.</div
+000a0ea0: 3e0a 3c64 6976 2063 6c61 7373 3d22 6a70  >.<div class="jp
+000a0eb0: 2d49 6e70 7574 4172 6561 206a 702d 4365  -InputArea jp-Ce
+000a0ec0: 6c6c 2d69 6e70 7574 4172 6561 223e 3c64  ll-inputArea"><d
+000a0ed0: 6976 2063 6c61 7373 3d22 6a70 2d49 6e70  iv class="jp-Inp
+000a0ee0: 7574 5072 6f6d 7074 206a 702d 496e 7075  utPrompt jp-Inpu
+000a0ef0: 7441 7265 612d 7072 6f6d 7074 223e 0a3c  tArea-prompt">.<
+000a0f00: 2f64 6976 3e3c 6469 7620 636c 6173 733d  /div><div class=
+000a0f10: 226a 702d 5265 6e64 6572 6564 4854 4d4c  "jp-RenderedHTML
+000a0f20: 436f 6d6d 6f6e 206a 702d 5265 6e64 6572  Common jp-Render
+000a0f30: 6564 4d61 726b 646f 776e 206a 702d 4d61  edMarkdown jp-Ma
+000a0f40: 726b 646f 776e 4f75 7470 7574 2022 2064  rkdownOutput " d
+000a0f50: 6174 612d 6d69 6d65 2d74 7970 653d 2274  ata-mime-type="t
+000a0f60: 6578 742f 6d61 726b 646f 776e 223e 0a0a  ext/markdown">..
+000a0f70: 3c70 7265 3e3c 636f 6465 3e63 2920 5374  <pre><code>c) St
+000a0f80: 7261 7469 6679 696e 6720 7468 6520 6461  ratifying the da
+000a0f90: 7461 2028 6578 616d 706c 6520 746f 2067  ta (example to g
+000a0fa0: 6574 2035 3025 206f 6620 7468 6520 6461  et 50% of the da
+000a0fb0: 7461 7365 7429 3a3c 2f63 6f64 653e 3c2f  taset):</code></
+000a0fc0: 7072 653e 0a0a 3c2f 6469 763e 0a3c 2f64  pre>..</div>.</d
+000a0fd0: 6976 3e0a 3c2f 6469 763e 0a3c 2f64 6976  iv>.</div>.</div
+000a0fe0: 3e3c 6469 7620 636c 6173 733d 226a 702d  ><div class="jp-
+000a0ff0: 4365 6c6c 206a 702d 436f 6465 4365 6c6c  Cell jp-CodeCell
+000a1000: 206a 702d 4e6f 7465 626f 6f6b 2d63 656c   jp-Notebook-cel
+000a1010: 6c20 2020 223e 0a3c 6469 7620 636c 6173  l   ">.<div clas
+000a1020: 733d 226a 702d 4365 6c6c 2d69 6e70 7574  s="jp-Cell-input
+000a1030: 5772 6170 7065 7222 3e0a 3c64 6976 2063  Wrapper">.<div c
+000a1040: 6c61 7373 3d22 6a70 2d43 6f6c 6c61 7073  lass="jp-Collaps
+000a1050: 6572 206a 702d 496e 7075 7443 6f6c 6c61  er jp-InputColla
+000a1060: 7073 6572 206a 702d 4365 6c6c 2d69 6e70  pser jp-Cell-inp
+000a1070: 7574 436f 6c6c 6170 7365 7222 3e0a 3c2f  utCollapser">.</
+000a1080: 6469 763e 0a3c 6469 7620 636c 6173 733d  div>.<div class=
+000a1090: 226a 702d 496e 7075 7441 7265 6120 6a70  "jp-InputArea jp
+000a10a0: 2d43 656c 6c2d 696e 7075 7441 7265 6122  -Cell-inputArea"
+000a10b0: 3e0a 3c64 6976 2063 6c61 7373 3d22 6a70  >.<div class="jp
+000a10c0: 2d49 6e70 7574 5072 6f6d 7074 206a 702d  -InputPrompt jp-
+000a10d0: 496e 7075 7441 7265 612d 7072 6f6d 7074  InputArea-prompt
+000a10e0: 223e 496e 266e 6273 703b 5b32 365d 3a3c  ">In&nbsp;[26]:<
+000a10f0: 2f64 6976 3e0a 3c64 6976 2063 6c61 7373  /div>.<div class
+000a1100: 3d22 6a70 2d43 6f64 654d 6972 726f 7245  ="jp-CodeMirrorE
+000a1110: 6469 746f 7220 6a70 2d45 6469 746f 7220  ditor jp-Editor 
+000a1120: 6a70 2d49 6e70 7574 4172 6561 2d65 6469  jp-InputArea-edi
+000a1130: 746f 7222 2064 6174 612d 7479 7065 3d22  tor" data-type="
+000a1140: 696e 6c69 6e65 223e 0a20 2020 2020 3c64  inline">.     <d
+000a1150: 6976 2063 6c61 7373 3d22 436f 6465 4d69  iv class="CodeMi
+000a1160: 7272 6f72 2063 6d2d 732d 6a75 7079 7465  rror cm-s-jupyte
+000a1170: 7222 3e0a 3c64 6976 2063 6c61 7373 3d22  r">.<div class="
+000a1180: 2068 6967 686c 6967 6874 2068 6c2d 6970   highlight hl-ip
+000a1190: 7974 686f 6e33 223e 3c70 7265 3e3c 7370  ython3"><pre><sp
+000a11a0: 616e 3e3c 2f73 7061 6e3e 3c73 7061 6e20  an></span><span 
+000a11b0: 636c 6173 733d 226e 223e 7472 6169 6e3c  class="n">train<
+000a11c0: 2f73 7061 6e3e 3c73 7061 6e20 636c 6173  /span><span clas
+000a11d0: 733d 2270 223e 2c3c 2f73 7061 6e3e 203c  s="p">,</span> <
+000a11e0: 7370 616e 2063 6c61 7373 3d22 6e22 3e74  span class="n">t
+000a11f0: 6573 743c 2f73 7061 6e3e 203c 7370 616e  est</span> <span
+000a1200: 2063 6c61 7373 3d22 6f22 3e3d 3c2f 7370   class="o">=</sp
+000a1210: 616e 3e20 3c73 7061 6e20 636c 6173 733d  an> <span class=
+000a1220: 226e 223e 7374 7261 7469 6679 3c2f 7370  "n">stratify</sp
+000a1230: 616e 3e3c 7370 616e 2063 6c61 7373 3d22  an><span class="
+000a1240: 7022 3e28 3c2f 7370 616e 3e3c 7370 616e  p">(</span><span
+000a1250: 2063 6c61 7373 3d22 6e22 3e64 663c 2f73   class="n">df</s
+000a1260: 7061 6e3e 3c73 7061 6e20 636c 6173 733d  pan><span class=
+000a1270: 2270 223e 2c3c 2f73 7061 6e3e 203c 7370  "p">,</span> <sp
+000a1280: 616e 2063 6c61 7373 3d22 6e22 3e73 616d  an class="n">sam
+000a1290: 706c 655f 7369 7a65 3c2f 7370 616e 3e3c  ple_size</span><
+000a12a0: 7370 616e 2063 6c61 7373 3d22 6f22 3e3d  span class="o">=
+000a12b0: 3c2f 7370 616e 3e3c 7370 616e 2063 6c61  </span><span cla
+000a12c0: 7373 3d22 6d66 223e 302e 353c 2f73 7061  ss="mf">0.5</spa
+000a12d0: 6e3e 3c73 7061 6e20 636c 6173 733d 2270  n><span class="p
+000a12e0: 223e 293c 2f73 7061 6e3e 0a0a 3c73 7061  ">)</span>..<spa
+000a12f0: 6e20 636c 6173 733d 226e 6222 3e70 7269  n class="nb">pri
+000a1300: 6e74 3c2f 7370 616e 3e3c 7370 616e 2063  nt</span><span c
+000a1310: 6c61 7373 3d22 7022 3e28 3c2f 7370 616e  lass="p">(</span
+000a1320: 3e3c 7370 616e 2063 6c61 7373 3d22 7331  ><span class="s1
+000a1330: 223e 2623 3339 3b53 6861 7065 2074 7261  ">&#39;Shape tra
+000a1340: 696e 2f74 6573 743a 2623 3339 3b3c 2f73  in/test:&#39;</s
+000a1350: 7061 6e3e 3c73 7061 6e20 636c 6173 733d  pan><span class=
+000a1360: 2270 223e 2c3c 2f73 7061 6e3e 203c 7370  "p">,</span> <sp
+000a1370: 616e 2063 6c61 7373 3d22 6e22 3e74 7261  an class="n">tra
+000a1380: 696e 3c2f 7370 616e 3e3c 7370 616e 2063  in</span><span c
+000a1390: 6c61 7373 3d22 6f22 3e2e 3c2f 7370 616e  lass="o">.</span
+000a13a0: 3e3c 7370 616e 2063 6c61 7373 3d22 6e22  ><span class="n"
+000a13b0: 3e73 6861 7065 3c2f 7370 616e 3e3c 7370  >shape</span><sp
+000a13c0: 616e 2063 6c61 7373 3d22 7022 3e2c 3c2f  an class="p">,</
+000a13d0: 7370 616e 3e20 3c73 7061 6e20 636c 6173  span> <span clas
+000a13e0: 733d 226e 223e 7465 7374 3c2f 7370 616e  s="n">test</span
+000a13f0: 3e3c 7370 616e 2063 6c61 7373 3d22 6f22  ><span class="o"
+000a1400: 3e2e 3c2f 7370 616e 3e3c 7370 616e 2063  >.</span><span c
+000a1410: 6c61 7373 3d22 6e22 3e73 6861 7065 3c2f  lass="n">shape</
+000a1420: 7370 616e 3e3c 7370 616e 2063 6c61 7373  span><span class
+000a1430: 3d22 7022 3e29 3c2f 7370 616e 3e0a 3c73  ="p">)</span>.<s
+000a1440: 7061 6e20 636c 6173 733d 226e 223e 7472  pan class="n">tr
+000a1450: 6169 6e3c 2f73 7061 6e3e 3c73 7061 6e20  ain</span><span 
+000a1460: 636c 6173 733d 226f 223e 2e3c 2f73 7061  class="o">.</spa
+000a1470: 6e3e 3c73 7061 6e20 636c 6173 733d 226e  n><span class="n
+000a1480: 223e 6865 6164 3c2f 7370 616e 3e3c 7370  ">head</span><sp
+000a1490: 616e 2063 6c61 7373 3d22 7022 3e28 293c  an class="p">()<
+000a14a0: 2f73 7061 6e3e 0a3c 2f70 7265 3e3c 2f64  /span>.</pre></d
+000a14b0: 6976 3e0a 0a20 2020 2020 3c2f 6469 763e  iv>..     </div>
+000a14c0: 0a3c 2f64 6976 3e0a 3c2f 6469 763e 0a3c  .</div>.</div>.<
+000a14d0: 2f64 6976 3e0a 0a3c 6469 7620 636c 6173  /div>..<div clas
+000a14e0: 733d 226a 702d 4365 6c6c 2d6f 7574 7075  s="jp-Cell-outpu
+000a14f0: 7457 7261 7070 6572 223e 0a3c 6469 7620  tWrapper">.<div 
+000a1500: 636c 6173 733d 226a 702d 436f 6c6c 6170  class="jp-Collap
+000a1510: 7365 7220 6a70 2d4f 7574 7075 7443 6f6c  ser jp-OutputCol
+000a1520: 6c61 7073 6572 206a 702d 4365 6c6c 2d6f  lapser jp-Cell-o
+000a1530: 7574 7075 7443 6f6c 6c61 7073 6572 223e  utputCollapser">
+000a1540: 0a3c 2f64 6976 3e0a 0a0a 3c64 6976 2063  .</div>...<div c
+000a1550: 6c61 7373 3d22 6a70 2d4f 7574 7075 7441  lass="jp-OutputA
+000a1560: 7265 6120 6a70 2d43 656c 6c2d 6f75 7470  rea jp-Cell-outp
+000a1570: 7574 4172 6561 223e 0a0a 3c64 6976 2063  utArea">..<div c
+000a1580: 6c61 7373 3d22 6a70 2d4f 7574 7075 7441  lass="jp-OutputA
+000a1590: 7265 612d 6368 696c 6422 3e0a 0a20 2020  rea-child">..   
+000a15a0: 200a 2020 2020 3c64 6976 2063 6c61 7373   .    <div class
+000a15b0: 3d22 6a70 2d4f 7574 7075 7450 726f 6d70  ="jp-OutputPromp
+000a15c0: 7420 6a70 2d4f 7574 7075 7441 7265 612d  t jp-OutputArea-
+000a15d0: 7072 6f6d 7074 223e 3c2f 6469 763e 0a0a  prompt"></div>..
+000a15e0: 0a0a 0a3c 6469 7620 636c 6173 733d 226a  ...<div class="j
+000a15f0: 702d 5265 6e64 6572 6564 5465 7874 206a  p-RenderedText j
+000a1600: 702d 4f75 7470 7574 4172 6561 2d6f 7574  p-OutputArea-out
+000a1610: 7075 7420 2220 6461 7461 2d6d 696d 652d  put " data-mime-
+000a1620: 7479 7065 3d22 7465 7874 2f70 6c61 696e  type="text/plain
+000a1630: 223e 0a3c 7072 653e 2020 3025 7c20 2020  ">.<pre>  0%|   
+000a1640: 2020 2020 2020 207c 2030 2f39 205b 3030         | 0/9 [00
+000a1650: 3a30 3026 6c74 3b3f 2c20 3f69 742f 735d  :00&lt;?, ?it/s]
+000a1660: 3c2f 7072 653e 0a3c 2f64 6976 3e0a 0a3c  </pre>.</div>..<
+000a1670: 2f64 6976 3e0a 0a3c 6469 7620 636c 6173  /div>..<div clas
+000a1680: 733d 226a 702d 4f75 7470 7574 4172 6561  s="jp-OutputArea
+000a1690: 2d63 6869 6c64 223e 0a0a 2020 2020 0a20  -child">..    . 
+000a16a0: 2020 203c 6469 7620 636c 6173 733d 226a     <div class="j
+000a16b0: 702d 4f75 7470 7574 5072 6f6d 7074 206a  p-OutputPrompt j
+000a16c0: 702d 4f75 7470 7574 4172 6561 2d70 726f  p-OutputArea-pro
+000a16d0: 6d70 7422 3e3c 2f64 6976 3e0a 0a0a 0a0a  mpt"></div>.....
+000a16e0: 3c64 6976 2063 6c61 7373 3d22 6a70 2d52  <div class="jp-R
+000a16f0: 656e 6465 7265 6454 6578 7420 6a70 2d4f  enderedText jp-O
+000a1700: 7574 7075 7441 7265 612d 6f75 7470 7574  utputArea-output
+000a1710: 2022 2064 6174 612d 6d69 6d65 2d74 7970   " data-mime-typ
+000a1720: 653d 2274 6578 742f 706c 6169 6e22 3e0a  e="text/plain">.
+000a1730: 3c70 7265 3e20 2030 257c 2020 2020 2020  <pre>  0%|      
+000a1740: 2020 2020 7c20 302f 3920 5b30 303a 3030      | 0/9 [00:00
+000a1750: 266c 743b 3f2c 203f 6974 2f73 5d3c 2f70  &lt;?, ?it/s]</p
+000a1760: 7265 3e0a 3c2f 6469 763e 0a0a 3c2f 6469  re>.</div>..</di
+000a1770: 763e 0a0a 3c64 6976 2063 6c61 7373 3d22  v>..<div class="
+000a1780: 6a70 2d4f 7574 7075 7441 7265 612d 6368  jp-OutputArea-ch
+000a1790: 696c 6422 3e0a 0a20 2020 200a 2020 2020  ild">..    .    
+000a17a0: 3c64 6976 2063 6c61 7373 3d22 6a70 2d4f  <div class="jp-O
+000a17b0: 7574 7075 7450 726f 6d70 7420 6a70 2d4f  utputPrompt jp-O
+000a17c0: 7574 7075 7441 7265 612d 7072 6f6d 7074  utputArea-prompt
+000a17d0: 223e 3c2f 6469 763e 0a0a 0a3c 6469 7620  "></div>...<div 
+000a17e0: 636c 6173 733d 226a 702d 5265 6e64 6572  class="jp-Render
+000a17f0: 6564 5465 7874 206a 702d 4f75 7470 7574  edText jp-Output
+000a1800: 4172 6561 2d6f 7574 7075 7422 2064 6174  Area-output" dat
+000a1810: 612d 6d69 6d65 2d74 7970 653d 2274 6578  a-mime-type="tex
+000a1820: 742f 706c 6169 6e22 3e0a 3c70 7265 3e53  t/plain">.<pre>S
+000a1830: 6861 7065 2074 7261 696e 2f74 6573 743a  hape train/test:
+000a1840: 2028 3136 3433 322c 2031 3129 2028 3731   (16432, 11) (71
+000a1850: 3036 2c20 3131 290a 3c2f 7072 653e 0a3c  06, 11).</pre>.<
+000a1860: 2f64 6976 3e0a 3c2f 6469 763e 0a0a 3c64  /div>.</div>..<d
+000a1870: 6976 2063 6c61 7373 3d22 6a70 2d4f 7574  iv class="jp-Out
+000a1880: 7075 7441 7265 612d 6368 696c 6422 3e0a  putArea-child">.
+000a1890: 0a20 2020 200a 2020 2020 3c64 6976 2063  .    .    <div c
+000a18a0: 6c61 7373 3d22 6a70 2d4f 7574 7075 7450  lass="jp-OutputP
+000a18b0: 726f 6d70 7420 6a70 2d4f 7574 7075 7441  rompt jp-OutputA
+000a18c0: 7265 612d 7072 6f6d 7074 223e 4f75 745b  rea-prompt">Out[
+000a18d0: 3236 5d3a 3c2f 6469 763e 0a0a 0a0a 3c64  26]:</div>....<d
+000a18e0: 6976 2063 6c61 7373 3d22 6a70 2d52 656e  iv class="jp-Ren
+000a18f0: 6465 7265 6448 544d 4c43 6f6d 6d6f 6e20  deredHTMLCommon 
+000a1900: 6a70 2d52 656e 6465 7265 6448 544d 4c20  jp-RenderedHTML 
+000a1910: 6a70 2d4f 7574 7075 7441 7265 612d 6f75  jp-OutputArea-ou
+000a1920: 7470 7574 206a 702d 4f75 7470 7574 4172  tput jp-OutputAr
+000a1930: 6561 2d65 7865 6375 7465 5265 7375 6c74  ea-executeResult
+000a1940: 2220 6461 7461 2d6d 696d 652d 7479 7065  " data-mime-type
+000a1950: 3d22 7465 7874 2f68 746d 6c22 3e0a 3c64  ="text/html">.<d
+000a1960: 6976 3e0a 3c73 7479 6c65 2073 636f 7065  iv>.<style scope
+000a1970: 643e 0a20 2020 202e 6461 7461 6672 616d  d>.    .datafram
+000a1980: 6520 7462 6f64 7920 7472 2074 683a 6f6e  e tbody tr th:on
+000a1990: 6c79 2d6f 662d 7479 7065 207b 0a20 2020  ly-of-type {.   
+000a19a0: 2020 2020 2076 6572 7469 6361 6c2d 616c       vertical-al
+000a19b0: 6967 6e3a 206d 6964 646c 653b 0a20 2020  ign: middle;.   
+000a19c0: 207d 0a0a 2020 2020 2e64 6174 6166 7261   }..    .datafra
+000a19d0: 6d65 2074 626f 6479 2074 7220 7468 207b  me tbody tr th {
+000a19e0: 0a20 2020 2020 2020 2076 6572 7469 6361  .        vertica
+000a19f0: 6c2d 616c 6967 6e3a 2074 6f70 3b0a 2020  l-align: top;.  
+000a1a00: 2020 7d0a 0a20 2020 202e 6461 7461 6672    }..    .datafr
+000a1a10: 616d 6520 7468 6561 6420 7468 207b 0a20  ame thead th {. 
+000a1a20: 2020 2020 2020 2074 6578 742d 616c 6967         text-alig
+000a1a30: 6e3a 2072 6967 6874 3b0a 2020 2020 7d0a  n: right;.    }.
+000a1a40: 3c2f 7374 796c 653e 0a3c 7461 626c 6520  </style>.<table 
+000a1a50: 626f 7264 6572 3d22 3122 2063 6c61 7373  border="1" class
+000a1a60: 3d22 6461 7461 6672 616d 6522 3e0a 2020  ="dataframe">.  
+000a1a70: 3c74 6865 6164 3e0a 2020 2020 3c74 7220  <thead>.    <tr 
+000a1a80: 7374 796c 653d 2274 6578 742d 616c 6967  style="text-alig
+000a1a90: 6e3a 2072 6967 6874 3b22 3e0a 2020 2020  n: right;">.    
+000a1aa0: 2020 3c74 683e 3c2f 7468 3e0a 2020 2020    <th></th>.    
+000a1ab0: 2020 3c74 683e 6461 7465 5f74 696d 653c    <th>date_time<
+000a1ac0: 2f74 683e 0a20 2020 2020 203c 7468 3e74  /th>.      <th>t
+000a1ad0: 696d 653c 2f74 683e 0a20 2020 2020 203c  ime</th>.      <
+000a1ae0: 7468 3e72 6174 696e 673c 2f74 683e 0a20  th>rating</th>. 
+000a1af0: 2020 2020 203c 7468 3e70 7269 6365 3c2f       <th>price</
+000a1b00: 7468 3e0a 2020 2020 2020 3c74 683e 7765  th>.      <th>we
+000a1b10: 6174 6865 723c 2f74 683e 0a20 2020 2020  ather</th>.     
+000a1b20: 203c 7468 3e64 6179 3c2f 7468 3e0a 2020   <th>day</th>.  
+000a1b30: 2020 2020 3c74 683e 7479 7065 3c2f 7468      <th>type</th
+000a1b40: 3e0a 2020 2020 2020 3c74 683e 6c61 743c  >.      <th>lat<
+000a1b50: 2f74 683e 0a20 2020 2020 203c 7468 3e6c  /th>.      <th>l
+000a1b60: 6f6e 3c2f 7468 3e0a 2020 2020 2020 3c74  on</th>.      <t
+000a1b70: 683e 7469 643c 2f74 683e 0a20 2020 2020  h>tid</th>.     
+000a1b80: 203c 7468 3e6c 6162 656c 3c2f 7468 3e0a   <th>label</th>.
+000a1b90: 2020 2020 3c2f 7472 3e0a 2020 3c2f 7468      </tr>.  </th
+000a1ba0: 6561 643e 0a20 203c 7462 6f64 793e 0a20  ead>.  <tbody>. 
+000a1bb0: 2020 203c 7472 3e0a 2020 2020 2020 3c74     <tr>.      <t
+000a1bc0: 683e 303c 2f74 683e 0a20 2020 2020 203c  h>0</th>.      <
+000a1bd0: 7464 3e32 3031 322d 3131 2d31 3220 3035  td>2012-11-12 05
+000a1be0: 3a31 373a 3138 3c2f 7464 3e0a 2020 2020  :17:18</td>.    
+000a1bf0: 2020 3c74 643e 3331 373c 2f74 643e 0a20    <td>317</td>. 
+000a1c00: 2020 2020 203c 7464 3e2d 312e 303c 2f74       <td>-1.0</t
+000a1c10: 643e 0a20 2020 2020 203c 7464 3e2d 313c  d>.      <td>-1<
+000a1c20: 2f74 643e 0a20 2020 2020 203c 7464 3e43  /td>.      <td>C
+000a1c30: 6c65 6172 3c2f 7464 3e0a 2020 2020 2020  lear</td>.      
+000a1c40: 3c74 643e 4d6f 6e64 6179 3c2f 7464 3e0a  <td>Monday</td>.
+000a1c50: 2020 2020 2020 3c74 643e 486f 6d65 2028        <td>Home (
+000a1c60: 7072 6976 6174 6529 3c2f 7464 3e0a 2020  private)</td>.  
+000a1c70: 2020 2020 3c74 643e 3430 2e38 3333 3136      <td>40.83316
+000a1c80: 353c 2f74 643e 0a20 2020 2020 203c 7464  5</td>.      <td
+000a1c90: 3e2d 3733 2e39 3431 3836 303c 2f74 643e  >-73.941860</td>
+000a1ca0: 0a20 2020 2020 203c 7464 3e31 3236 3c2f  .      <td>126</
+000a1cb0: 7464 3e0a 2020 2020 2020 3c74 643e 5265  td>.      <td>Re
+000a1cc0: 7369 6465 6e63 653c 2f74 643e 0a20 2020  sidence</td>.   
+000a1cd0: 203c 2f74 723e 0a20 2020 203c 7472 3e0a   </tr>.    <tr>.
+000a1ce0: 2020 2020 2020 3c74 683e 313c 2f74 683e        <th>1</th>
+000a1cf0: 0a20 2020 2020 203c 7464 3e32 3031 322d  .      <td>2012-
+000a1d00: 3131 2d31 3220 3233 3a32 343a 3535 3c2f  11-12 23:24:55</
+000a1d10: 7464 3e0a 2020 2020 2020 3c74 643e 3134  td>.      <td>14
+000a1d20: 3034 3c2f 7464 3e0a 2020 2020 2020 3c74  04</td>.      <t
+000a1d30: 643e 382e 323c 2f74 643e 0a20 2020 2020  d>8.2</td>.     
+000a1d40: 203c 7464 3e31 3c2f 7464 3e0a 2020 2020   <td>1</td>.    
+000a1d50: 2020 3c74 643e 436c 6f75 6473 3c2f 7464    <td>Clouds</td
+000a1d60: 3e0a 2020 2020 2020 3c74 643e 4d6f 6e64  >.      <td>Mond
+000a1d70: 6179 3c2f 7464 3e0a 2020 2020 2020 3c74  ay</td>.      <t
+000a1d80: 643e 4465 6c69 202f 2042 6f64 6567 613c  d>Deli / Bodega<
+000a1d90: 2f74 643e 0a20 2020 2020 203c 7464 3e34  /td>.      <td>4
+000a1da0: 302e 3833 3430 3938 3c2f 7464 3e0a 2020  0.834098</td>.  
+000a1db0: 2020 2020 3c74 643e 2d37 332e 3934 3532      <td>-73.9452
+000a1dc0: 3637 3c2f 7464 3e0a 2020 2020 2020 3c74  67</td>.      <t
+000a1dd0: 643e 3132 363c 2f74 643e 0a20 2020 2020  d>126</td>.     
+000a1de0: 203c 7464 3e46 6f6f 643c 2f74 643e 0a20   <td>Food</td>. 
+000a1df0: 2020 203c 2f74 723e 0a20 2020 203c 7472     </tr>.    <tr
+000a1e00: 3e0a 2020 2020 2020 3c74 683e 323c 2f74  >.      <th>2</t
+000a1e10: 683e 0a20 2020 2020 203c 7464 3e32 3031  h>.      <td>201
+000a1e20: 322d 3131 2d31 3320 3030 3a30 303a 3037  2-11-13 00:00:07
+000a1e30: 3c2f 7464 3e0a 2020 2020 2020 3c74 643e  </td>.      <td>
+000a1e40: 303c 2f74 643e 0a20 2020 2020 203c 7464  0</td>.      <td
+000a1e50: 3e2d 312e 303c 2f74 643e 0a20 2020 2020  >-1.0</td>.     
+000a1e60: 203c 7464 3e2d 313c 2f74 643e 0a20 2020   <td>-1</td>.   
+000a1e70: 2020 203c 7464 3e43 6c6f 7564 733c 2f74     <td>Clouds</t
+000a1e80: 643e 0a20 2020 2020 203c 7464 3e54 7565  d>.      <td>Tue
+000a1e90: 7364 6179 3c2f 7464 3e0a 2020 2020 2020  sday</td>.      
+000a1ea0: 3c74 643e 486f 6d65 2028 7072 6976 6174  <td>Home (privat
+000a1eb0: 6529 3c2f 7464 3e0a 2020 2020 2020 3c74  e)</td>.      <t
+000a1ec0: 643e 3430 2e38 3333 3136 353c 2f74 643e  d>40.833165</td>
+000a1ed0: 0a20 2020 2020 203c 7464 3e2d 3733 2e39  .      <td>-73.9
+000a1ee0: 3431 3836 303c 2f74 643e 0a20 2020 2020  41860</td>.     
+000a1ef0: 203c 7464 3e31 3236 3c2f 7464 3e0a 2020   <td>126</td>.  
+000a1f00: 2020 2020 3c74 643e 5265 7369 6465 6e63      <td>Residenc
+000a1f10: 653c 2f74 643e 0a20 2020 203c 2f74 723e  e</td>.    </tr>
+000a1f20: 0a20 2020 203c 7472 3e0a 2020 2020 2020  .    <tr>.      
+000a1f30: 3c74 683e 333c 2f74 683e 0a20 2020 2020  <th>3</th>.     
+000a1f40: 203c 7464 3e32 3031 322d 3131 2d31 3520   <td>2012-11-15 
+000a1f50: 3137 3a34 393a 3031 3c2f 7464 3e0a 2020  17:49:01</td>.  
+000a1f60: 2020 2020 3c74 643e 3130 3639 3c2f 7464      <td>1069</td
+000a1f70: 3e0a 2020 2020 2020 3c74 643e 362e 363c  >.      <td>6.6<
+000a1f80: 2f74 643e 0a20 2020 2020 203c 7464 3e33  /td>.      <td>3
+000a1f90: 3c2f 7464 3e0a 2020 2020 2020 3c74 643e  </td>.      <td>
+000a1fa0: 436c 6561 723c 2f74 643e 0a20 2020 2020  Clear</td>.     
+000a1fb0: 203c 7464 3e54 6875 7273 6461 793c 2f74   <td>Thursday</t
+000a1fc0: 643e 0a20 2020 2020 203c 7464 3e46 7269  d>.      <td>Fri
+000a1fd0: 6564 2043 6869 636b 656e 204a 6f69 6e74  ed Chicken Joint
+000a1fe0: 3c2f 7464 3e0a 2020 2020 2020 3c74 643e  </td>.      <td>
+000a1ff0: 3430 2e37 3634 3639 363c 2f74 643e 0a20  40.764696</td>. 
+000a2000: 2020 2020 203c 7464 3e2d 3733 2e38 3835       <td>-73.885
+000a2010: 3139 373c 2f74 643e 0a20 2020 2020 203c  197</td>.      <
+000a2020: 7464 3e31 3236 3c2f 7464 3e0a 2020 2020  td>126</td>.    
+000a2030: 2020 3c74 643e 466f 6f64 3c2f 7464 3e0a    <td>Food</td>.
+000a2040: 2020 2020 3c2f 7472 3e0a 2020 2020 3c74      </tr>.    <t
+000a2050: 723e 0a20 2020 2020 203c 7468 3e34 3c2f  r>.      <th>4</
+000a2060: 7468 3e0a 2020 2020 2020 3c74 643e 3230  th>.      <td>20
+000a2070: 3132 2d31 312d 3135 2031 383a 3430 3a31  12-11-15 18:40:1
+000a2080: 363c 2f74 643e 0a20 2020 2020 203c 7464  6</td>.      <td
+000a2090: 3e31 3132 303c 2f74 643e 0a20 2020 2020  >1120</td>.     
+000a20a0: 203c 7464 3e2d 312e 303c 2f74 643e 0a20   <td>-1.0</td>. 
+000a20b0: 2020 2020 203c 7464 3e2d 313c 2f74 643e       <td>-1</td>
+000a20c0: 0a20 2020 2020 203c 7464 3e43 6c65 6172  .      <td>Clear
+000a20d0: 3c2f 7464 3e0a 2020 2020 2020 3c74 643e  </td>.      <td>
+000a20e0: 5468 7572 7364 6179 3c2f 7464 3e0a 2020  Thursday</td>.  
+000a20f0: 2020 2020 3c74 643e 4275 7320 5374 6174      <td>Bus Stat
+000a2100: 696f 6e3c 2f74 643e 0a20 2020 2020 203c  ion</td>.      <
+000a2110: 7464 3e34 302e 3736 3630 3739 3c2f 7464  td>40.766079</td
+000a2120: 3e0a 2020 2020 2020 3c74 643e 2d37 332e  >.      <td>-73.
+000a2130: 3838 3335 3239 3c2f 7464 3e0a 2020 2020  883529</td>.    
+000a2140: 2020 3c74 643e 3132 363c 2f74 643e 0a20    <td>126</td>. 
+000a2150: 2020 2020 203c 7464 3e54 7261 7665 6c20       <td>Travel 
+000a2160: 2661 6d70 3b20 5472 616e 7370 6f72 743c  &amp; Transport<
+000a2170: 2f74 643e 0a20 2020 203c 2f74 723e 0a20  /td>.    </tr>. 
+000a2180: 203c 2f74 626f 6479 3e0a 3c2f 7461 626c   </tbody>.</tabl
+000a2190: 653e 0a3c 2f64 6976 3e0a 3c2f 6469 763e  e>.</div>.</div>
+000a21a0: 0a0a 3c2f 6469 763e 0a0a 3c2f 6469 763e  ..</div>..</div>
+000a21b0: 0a0a 3c2f 6469 763e 0a0a 3c2f 6469 763e  ..</div>..</div>
+000a21c0: 0a3c 6469 7620 636c 6173 733d 226a 702d  .<div class="jp-
+000a21d0: 4365 6c6c 206a 702d 4d61 726b 646f 776e  Cell jp-Markdown
+000a21e0: 4365 6c6c 206a 702d 4e6f 7465 626f 6f6b  Cell jp-Notebook
+000a21f0: 2d63 656c 6c22 3e0a 3c64 6976 2063 6c61  -cell">.<div cla
+000a2200: 7373 3d22 6a70 2d43 656c 6c2d 696e 7075  ss="jp-Cell-inpu
+000a2210: 7457 7261 7070 6572 223e 0a3c 6469 7620  tWrapper">.<div 
+000a2220: 636c 6173 733d 226a 702d 436f 6c6c 6170  class="jp-Collap
+000a2230: 7365 7220 6a70 2d49 6e70 7574 436f 6c6c  ser jp-InputColl
+000a2240: 6170 7365 7220 6a70 2d43 656c 6c2d 696e  apser jp-Cell-in
+000a2250: 7075 7443 6f6c 6c61 7073 6572 223e 0a3c  putCollapser">.<
+000a2260: 2f64 6976 3e0a 3c64 6976 2063 6c61 7373  /div>.<div class
+000a2270: 3d22 6a70 2d49 6e70 7574 4172 6561 206a  ="jp-InputArea j
+000a2280: 702d 4365 6c6c 2d69 6e70 7574 4172 6561  p-Cell-inputArea
+000a2290: 223e 3c64 6976 2063 6c61 7373 3d22 6a70  "><div class="jp
+000a22a0: 2d49 6e70 7574 5072 6f6d 7074 206a 702d  -InputPrompt jp-
+000a22b0: 496e 7075 7441 7265 612d 7072 6f6d 7074  InputArea-prompt
+000a22c0: 223e 0a3c 2f64 6976 3e3c 6469 7620 636c  ">.</div><div cl
+000a22d0: 6173 733d 226a 702d 5265 6e64 6572 6564  ass="jp-Rendered
+000a22e0: 4854 4d4c 436f 6d6d 6f6e 206a 702d 5265  HTMLCommon jp-Re
+000a22f0: 6e64 6572 6564 4d61 726b 646f 776e 206a  nderedMarkdown j
+000a2300: 702d 4d61 726b 646f 776e 4f75 7470 7574  p-MarkdownOutput
+000a2310: 2022 2064 6174 612d 6d69 6d65 2d74 7970   " data-mime-typ
+000a2320: 653d 2274 6578 742f 6d61 726b 646f 776e  e="text/markdown
+000a2330: 223e 0a3c 703e 6b2d 466f 6c64 2053 7472  ">.<p>k-Fold Str
+000a2340: 6174 6966 7969 6e67 2074 6865 2064 6174  atifying the dat
+000a2350: 6120 2865 7861 6d70 6c65 2074 6f20 6765  a (example to ge
+000a2360: 7420 3530 2520 6f66 2074 6865 2064 6174  t 50% of the dat
+000a2370: 6173 6574 2069 6e20 332d 666f 6c64 7329  aset in 3-folds)
+000a2380: 3a3c 2f70 3e0a 0a3c 2f64 6976 3e0a 3c2f  :</p>..</div>.</
+000a2390: 6469 763e 0a3c 2f64 6976 3e0a 3c2f 6469  div>.</div>.</di
+000a23a0: 763e 3c64 6976 2063 6c61 7373 3d22 6a70  v><div class="jp
+000a23b0: 2d43 656c 6c20 6a70 2d43 6f64 6543 656c  -Cell jp-CodeCel
+000a23c0: 6c20 6a70 2d4e 6f74 6562 6f6f 6b2d 6365  l jp-Notebook-ce
+000a23d0: 6c6c 2020 2022 3e0a 3c64 6976 2063 6c61  ll   ">.<div cla
+000a23e0: 7373 3d22 6a70 2d43 656c 6c2d 696e 7075  ss="jp-Cell-inpu
+000a23f0: 7457 7261 7070 6572 223e 0a3c 6469 7620  tWrapper">.<div 
+000a2400: 636c 6173 733d 226a 702d 436f 6c6c 6170  class="jp-Collap
+000a2410: 7365 7220 6a70 2d49 6e70 7574 436f 6c6c  ser jp-InputColl
+000a2420: 6170 7365 7220 6a70 2d43 656c 6c2d 696e  apser jp-Cell-in
+000a2430: 7075 7443 6f6c 6c61 7073 6572 223e 0a3c  putCollapser">.<
+000a2440: 2f64 6976 3e0a 3c64 6976 2063 6c61 7373  /div>.<div class
+000a2450: 3d22 6a70 2d49 6e70 7574 4172 6561 206a  ="jp-InputArea j
+000a2460: 702d 4365 6c6c 2d69 6e70 7574 4172 6561  p-Cell-inputArea
+000a2470: 223e 0a3c 6469 7620 636c 6173 733d 226a  ">.<div class="j
+000a2480: 702d 496e 7075 7450 726f 6d70 7420 6a70  p-InputPrompt jp
+000a2490: 2d49 6e70 7574 4172 6561 2d70 726f 6d70  -InputArea-promp
+000a24a0: 7422 3e49 6e26 6e62 7370 3b5b 3237 5d3a  t">In&nbsp;[27]:
+000a24b0: 3c2f 6469 763e 0a3c 6469 7620 636c 6173  </div>.<div clas
+000a24c0: 733d 226a 702d 436f 6465 4d69 7272 6f72  s="jp-CodeMirror
+000a24d0: 4564 6974 6f72 206a 702d 4564 6974 6f72  Editor jp-Editor
+000a24e0: 206a 702d 496e 7075 7441 7265 612d 6564   jp-InputArea-ed
+000a24f0: 6974 6f72 2220 6461 7461 2d74 7970 653d  itor" data-type=
+000a2500: 2269 6e6c 696e 6522 3e0a 2020 2020 203c  "inline">.     <
+000a2510: 6469 7620 636c 6173 733d 2243 6f64 654d  div class="CodeM
+000a2520: 6972 726f 7220 636d 2d73 2d6a 7570 7974  irror cm-s-jupyt
+000a2530: 6572 223e 0a3c 6469 7620 636c 6173 733d  er">.<div class=
+000a2540: 2220 6869 6768 6c69 6768 7420 686c 2d69  " highlight hl-i
+000a2550: 7079 7468 6f6e 3322 3e3c 7072 653e 3c73  python3"><pre><s
+000a2560: 7061 6e3e 3c2f 7370 616e 3e3c 7370 616e  pan></span><span
+000a2570: 2063 6c61 7373 3d22 6e22 3e74 7261 696e   class="n">train
+000a2580: 3c2f 7370 616e 3e3c 7370 616e 2063 6c61  </span><span cla
+000a2590: 7373 3d22 7022 3e2c 3c2f 7370 616e 3e20  ss="p">,</span> 
+000a25a0: 3c73 7061 6e20 636c 6173 733d 226e 223e  <span class="n">
+000a25b0: 7465 7374 3c2f 7370 616e 3e20 3c73 7061  test</span> <spa
+000a25c0: 6e20 636c 6173 733d 226f 223e 3d3c 2f73  n class="o">=</s
+000a25d0: 7061 6e3e 203c 7370 616e 2063 6c61 7373  pan> <span class
+000a25e0: 3d22 6e22 3e6b 6c61 6265 6c73 5f73 7472  ="n">klabels_str
+000a25f0: 6174 6966 793c 2f73 7061 6e3e 3c73 7061  atify</span><spa
+000a2600: 6e20 636c 6173 733d 2270 223e 283c 2f73  n class="p">(</s
+000a2610: 7061 6e3e 3c73 7061 6e20 636c 6173 733d  pan><span class=
+000a2620: 226e 223e 6466 3c2f 7370 616e 3e3c 7370  "n">df</span><sp
+000a2630: 616e 2063 6c61 7373 3d22 7022 3e2c 3c2f  an class="p">,</
+000a2640: 7370 616e 3e20 3c73 7061 6e20 636c 6173  span> <span clas
+000a2650: 733d 226e 223e 6b6c 3c2f 7370 616e 3e3c  s="n">kl</span><
+000a2660: 7370 616e 2063 6c61 7373 3d22 6f22 3e3d  span class="o">=
+000a2670: 3c2f 7370 616e 3e3c 7370 616e 2063 6c61  </span><span cla
+000a2680: 7373 3d22 6d69 223e 353c 2f73 7061 6e3e  ss="mi">5</span>
+000a2690: 3c73 7061 6e20 636c 6173 733d 2270 223e  <span class="p">
+000a26a0: 293c 2f73 7061 6e3e 0a0a 3c73 7061 6e20  )</span>..<span 
+000a26b0: 636c 6173 733d 226e 6222 3e70 7269 6e74  class="nb">print
+000a26c0: 3c2f 7370 616e 3e3c 7370 616e 2063 6c61  </span><span cla
+000a26d0: 7373 3d22 7022 3e28 3c2f 7370 616e 3e3c  ss="p">(</span><
+000a26e0: 7370 616e 2063 6c61 7373 3d22 7331 223e  span class="s1">
+000a26f0: 2623 3339 3b53 6861 7065 2074 7261 696e  &#39;Shape train
+000a2700: 2f74 6573 743a 2623 3339 3b3c 2f73 7061  /test:&#39;</spa
+000a2710: 6e3e 3c73 7061 6e20 636c 6173 733d 2270  n><span class="p
+000a2720: 223e 2c3c 2f73 7061 6e3e 203c 7370 616e  ">,</span> <span
+000a2730: 2063 6c61 7373 3d22 6e22 3e74 7261 696e   class="n">train
+000a2740: 3c2f 7370 616e 3e3c 7370 616e 2063 6c61  </span><span cla
+000a2750: 7373 3d22 6f22 3e2e 3c2f 7370 616e 3e3c  ss="o">.</span><
+000a2760: 7370 616e 2063 6c61 7373 3d22 6e22 3e73  span class="n">s
+000a2770: 6861 7065 3c2f 7370 616e 3e3c 7370 616e  hape</span><span
+000a2780: 2063 6c61 7373 3d22 7022 3e2c 3c2f 7370   class="p">,</sp
+000a2790: 616e 3e20 3c73 7061 6e20 636c 6173 733d  an> <span class=
+000a27a0: 226e 223e 7465 7374 3c2f 7370 616e 3e3c  "n">test</span><
+000a27b0: 7370 616e 2063 6c61 7373 3d22 6f22 3e2e  span class="o">.
+000a27c0: 3c2f 7370 616e 3e3c 7370 616e 2063 6c61  </span><span cla
+000a27d0: 7373 3d22 6e22 3e73 6861 7065 3c2f 7370  ss="n">shape</sp
+000a27e0: 616e 3e3c 7370 616e 2063 6c61 7373 3d22  an><span class="
+000a27f0: 7022 3e29 3c2f 7370 616e 3e0a 0a0a 3c73  p">)</span>...<s
+000a2800: 7061 6e20 636c 6173 733d 226e 6222 3e70  pan class="nb">p
+000a2810: 7269 6e74 3c2f 7370 616e 3e3c 7370 616e  rint</span><span
+000a2820: 2063 6c61 7373 3d22 7022 3e28 3c2f 7370   class="p">(</sp
+000a2830: 616e 3e3c 7370 616e 2063 6c61 7373 3d22  an><span class="
+000a2840: 7331 223e 2623 3339 3b4c 6162 656c 7320  s1">&#39;Labels 
+000a2850: 6265 666f 7265 3a26 2333 393b 3c2f 7370  before:&#39;</sp
+000a2860: 616e 3e3c 7370 616e 2063 6c61 7373 3d22  an><span class="
+000a2870: 7022 3e2c 3c2f 7370 616e 3e20 3c73 7061  p">,</span> <spa
+000a2880: 6e20 636c 6173 733d 226e 223e 6466 3c2f  n class="n">df</
+000a2890: 7370 616e 3e3c 7370 616e 2063 6c61 7373  span><span class
+000a28a0: 3d22 6f22 3e2e 3c2f 7370 616e 3e3c 7370  ="o">.</span><sp
+000a28b0: 616e 2063 6c61 7373 3d22 6e22 3e6c 6162  an class="n">lab
+000a28c0: 656c 3c2f 7370 616e 3e3c 7370 616e 2063  el</span><span c
+000a28d0: 6c61 7373 3d22 6f22 3e2e 3c2f 7370 616e  lass="o">.</span
+000a28e0: 3e3c 7370 616e 2063 6c61 7373 3d22 6e22  ><span class="n"
+000a28f0: 3e75 6e69 7175 653c 2f73 7061 6e3e 3c73  >unique</span><s
+000a2900: 7061 6e20 636c 6173 733d 2270 223e 2829  pan class="p">()
+000a2910: 293c 2f73 7061 6e3e 0a3c 7370 616e 2063  )</span>.<span c
+000a2920: 6c61 7373 3d22 6e62 223e 7072 696e 743c  lass="nb">print<
+000a2930: 2f73 7061 6e3e 3c73 7061 6e20 636c 6173  /span><span clas
+000a2940: 733d 2270 223e 283c 2f73 7061 6e3e 3c73  s="p">(</span><s
+000a2950: 7061 6e20 636c 6173 733d 2273 3122 3e26  pan class="s1">&
+000a2960: 2333 393b 4c61 6265 6c73 2061 6674 6572  #39;Labels after
+000a2970: 3a26 2333 393b 3c2f 7370 616e 3e3c 7370  :&#39;</span><sp
+000a2980: 616e 2063 6c61 7373 3d22 7022 3e2c 3c2f  an class="p">,</
+000a2990: 7370 616e 3e20 3c73 7061 6e20 636c 6173  span> <span clas
+000a29a0: 733d 226e 223e 7472 6169 6e3c 2f73 7061  s="n">train</spa
+000a29b0: 6e3e 3c73 7061 6e20 636c 6173 733d 226f  n><span class="o
+000a29c0: 223e 2e3c 2f73 7061 6e3e 3c73 7061 6e20  ">.</span><span 
+000a29d0: 636c 6173 733d 226e 223e 6c61 6265 6c3c  class="n">label<
+000a29e0: 2f73 7061 6e3e 3c73 7061 6e20 636c 6173  /span><span clas
+000a29f0: 733d 226f 223e 2e3c 2f73 7061 6e3e 3c73  s="o">.</span><s
+000a2a00: 7061 6e20 636c 6173 733d 226e 223e 756e  pan class="n">un
+000a2a10: 6971 7565 3c2f 7370 616e 3e3c 7370 616e  ique</span><span
+000a2a20: 2063 6c61 7373 3d22 7022 3e28 2929 3c2f   class="p">())</
+000a2a30: 7370 616e 3e0a 3c2f 7072 653e 3c2f 6469  span>.</pre></di
+000a2a40: 763e 0a0a 2020 2020 203c 2f64 6976 3e0a  v>..     </div>.
+000a2a50: 3c2f 6469 763e 0a3c 2f64 6976 3e0a 3c2f  </div>.</div>.</
+000a2a60: 6469 763e 0a0a 3c64 6976 2063 6c61 7373  div>..<div class
+000a2a70: 3d22 6a70 2d43 656c 6c2d 6f75 7470 7574  ="jp-Cell-output
+000a2a80: 5772 6170 7065 7222 3e0a 3c64 6976 2063  Wrapper">.<div c
+000a2a90: 6c61 7373 3d22 6a70 2d43 6f6c 6c61 7073  lass="jp-Collaps
+000a2aa0: 6572 206a 702d 4f75 7470 7574 436f 6c6c  er jp-OutputColl
+000a2ab0: 6170 7365 7220 6a70 2d43 656c 6c2d 6f75  apser jp-Cell-ou
+000a2ac0: 7470 7574 436f 6c6c 6170 7365 7222 3e0a  tputCollapser">.
+000a2ad0: 3c2f 6469 763e 0a0a 0a3c 6469 7620 636c  </div>...<div cl
+000a2ae0: 6173 733d 226a 702d 4f75 7470 7574 4172  ass="jp-OutputAr
+000a2af0: 6561 206a 702d 4365 6c6c 2d6f 7574 7075  ea jp-Cell-outpu
+000a2b00: 7441 7265 6122 3e0a 0a3c 6469 7620 636c  tArea">..<div cl
+000a2b10: 6173 733d 226a 702d 4f75 7470 7574 4172  ass="jp-OutputAr
+000a2b20: 6561 2d63 6869 6c64 223e 0a0a 2020 2020  ea-child">..    
+000a2b30: 0a20 2020 203c 6469 7620 636c 6173 733d  .    <div class=
+000a2b40: 226a 702d 4f75 7470 7574 5072 6f6d 7074  "jp-OutputPrompt
+000a2b50: 206a 702d 4f75 7470 7574 4172 6561 2d70   jp-OutputArea-p
+000a2b60: 726f 6d70 7422 3e3c 2f64 6976 3e0a 0a0a  rompt"></div>...
+000a2b70: 0a0a 3c64 6976 2063 6c61 7373 3d22 6a70  ..<div class="jp
+000a2b80: 2d52 656e 6465 7265 6454 6578 7420 6a70  -RenderedText jp
+000a2b90: 2d4f 7574 7075 7441 7265 612d 6f75 7470  -OutputArea-outp
+000a2ba0: 7574 2022 2064 6174 612d 6d69 6d65 2d74  ut " data-mime-t
+000a2bb0: 7970 653d 2274 6578 742f 706c 6169 6e22  ype="text/plain"
+000a2bc0: 3e0a 3c70 7265 3e20 2030 257c 2020 2020  >.<pre>  0%|    
+000a2bd0: 2020 2020 2020 7c20 302f 3520 5b30 303a        | 0/5 [00:
+000a2be0: 3030 266c 743b 3f2c 203f 6974 2f73 5d3c  00&lt;?, ?it/s]<
+000a2bf0: 2f70 7265 3e0a 3c2f 6469 763e 0a0a 3c2f  /pre>.</div>..</
+000a2c00: 6469 763e 0a0a 3c64 6976 2063 6c61 7373  div>..<div class
+000a2c10: 3d22 6a70 2d4f 7574 7075 7441 7265 612d  ="jp-OutputArea-
+000a2c20: 6368 696c 6422 3e0a 0a20 2020 200a 2020  child">..    .  
+000a2c30: 2020 3c64 6976 2063 6c61 7373 3d22 6a70    <div class="jp
+000a2c40: 2d4f 7574 7075 7450 726f 6d70 7420 6a70  -OutputPrompt jp
+000a2c50: 2d4f 7574 7075 7441 7265 612d 7072 6f6d  -OutputArea-prom
+000a2c60: 7074 223e 3c2f 6469 763e 0a0a 0a3c 6469  pt"></div>...<di
+000a2c70: 7620 636c 6173 733d 226a 702d 5265 6e64  v class="jp-Rend
+000a2c80: 6572 6564 5465 7874 206a 702d 4f75 7470  eredText jp-Outp
+000a2c90: 7574 4172 6561 2d6f 7574 7075 7422 2064  utArea-output" d
+000a2ca0: 6174 612d 6d69 6d65 2d74 7970 653d 2274  ata-mime-type="t
+000a2cb0: 6578 742f 706c 6169 6e22 3e0a 3c70 7265  ext/plain">.<pre
+000a2cc0: 3e53 6861 7065 2074 7261 696e 2f74 6573  >Shape train/tes
+000a2cd0: 743a 2028 3235 3832 342c 2031 3129 2028  t: (25824, 11) (
+000a2ce0: 3131 3730 342c 2031 3129 0a4c 6162 656c  11704, 11).Label
+000a2cf0: 7320 6265 666f 7265 3a20 5b26 2333 393b  s before: [&#39;
+000a2d00: 5265 7369 6465 6e63 6526 2333 393b 2026  Residence&#39; &
+000a2d10: 2333 393b 466f 6f64 2623 3339 3b20 2623  #39;Food&#39; &#
+000a2d20: 3339 3b54 7261 7665 6c20 2661 6d70 3b20  39;Travel &amp; 
+000a2d30: 5472 616e 7370 6f72 7426 2333 393b 2026  Transport&#39; &
+000a2d40: 2333 393b 5072 6f66 6573 7369 6f6e 616c  #39;Professional
+000a2d50: 2026 616d 703b 204f 7468 6572 2050 6c61   &amp; Other Pla
+000a2d60: 6365 7326 2333 393b 0a20 2623 3339 3b53  ces&#39;. &#39;S
+000a2d70: 686f 7020 2661 6d70 3b20 5365 7276 6963  hop &amp; Servic
+000a2d80: 6526 2333 393b 2026 2333 393b 4f75 7464  e&#39; &#39;Outd
+000a2d90: 6f6f 7273 2026 616d 703b 2052 6563 7265  oors &amp; Recre
+000a2da0: 6174 696f 6e26 2333 393b 2026 2333 393b  ation&#39; &#39;
+000a2db0: 436f 6c6c 6567 6520 2661 6d70 3b20 556e  College &amp; Un
+000a2dc0: 6976 6572 7369 7479 2623 3339 3b0a 2026  iversity&#39;. &
+000a2dd0: 2333 393b 4172 7473 2026 616d 703b 2045  #39;Arts &amp; E
+000a2de0: 6e74 6572 7461 696e 6d65 6e74 2623 3339  ntertainment&#39
+000a2df0: 3b20 2623 3339 3b4e 6967 6874 6c69 6665  ; &#39;Nightlife
+000a2e00: 2053 706f 7426 2333 393b 2026 2333 393b   Spot&#39; &#39;
+000a2e10: 4576 656e 7426 2333 393b 5d0a 4c61 6265  Event&#39;].Labe
+000a2e20: 6c73 2061 6674 6572 3a20 5b26 2333 393b  ls after: [&#39;
+000a2e30: 5265 7369 6465 6e63 6526 2333 393b 2026  Residence&#39; &
+000a2e40: 2333 393b 466f 6f64 2623 3339 3b20 2623  #39;Food&#39; &#
+000a2e50: 3339 3b54 7261 7665 6c20 2661 6d70 3b20  39;Travel &amp; 
+000a2e60: 5472 616e 7370 6f72 7426 2333 393b 2026  Transport&#39; &
+000a2e70: 2333 393b 5072 6f66 6573 7369 6f6e 616c  #39;Professional
+000a2e80: 2026 616d 703b 204f 7468 6572 2050 6c61   &amp; Other Pla
+000a2e90: 6365 7326 2333 393b 0a20 2623 3339 3b53  ces&#39;. &#39;S
+000a2ea0: 686f 7020 2661 6d70 3b20 5365 7276 6963  hop &amp; Servic
+000a2eb0: 6526 2333 393b 5d0a 3c2f 7072 653e 0a3c  e&#39;].</pre>.<
+000a2ec0: 2f64 6976 3e0a 3c2f 6469 763e 0a0a 3c2f  /div>.</div>..</
+000a2ed0: 6469 763e 0a0a 3c2f 6469 763e 0a0a 3c2f  div>..</div>..</
+000a2ee0: 6469 763e 0a3c 6469 7620 636c 6173 733d  div>.<div class=
+000a2ef0: 226a 702d 4365 6c6c 206a 702d 4d61 726b  "jp-Cell jp-Mark
+000a2f00: 646f 776e 4365 6c6c 206a 702d 4e6f 7465  downCell jp-Note
+000a2f10: 626f 6f6b 2d63 656c 6c22 3e0a 3c64 6976  book-cell">.<div
+000a2f20: 2063 6c61 7373 3d22 6a70 2d43 656c 6c2d   class="jp-Cell-
+000a2f30: 696e 7075 7457 7261 7070 6572 223e 0a3c  inputWrapper">.<
+000a2f40: 6469 7620 636c 6173 733d 226a 702d 436f  div class="jp-Co
+000a2f50: 6c6c 6170 7365 7220 6a70 2d49 6e70 7574  llapser jp-Input
+000a2f60: 436f 6c6c 6170 7365 7220 6a70 2d43 656c  Collapser jp-Cel
+000a2f70: 6c2d 696e 7075 7443 6f6c 6c61 7073 6572  l-inputCollapser
+000a2f80: 223e 0a3c 2f64 6976 3e0a 3c64 6976 2063  ">.</div>.<div c
+000a2f90: 6c61 7373 3d22 6a70 2d49 6e70 7574 4172  lass="jp-InputAr
+000a2fa0: 6561 206a 702d 4365 6c6c 2d69 6e70 7574  ea jp-Cell-input
+000a2fb0: 4172 6561 223e 3c64 6976 2063 6c61 7373  Area"><div class
+000a2fc0: 3d22 6a70 2d49 6e70 7574 5072 6f6d 7074  ="jp-InputPrompt
+000a2fd0: 206a 702d 496e 7075 7441 7265 612d 7072   jp-InputArea-pr
+000a2fe0: 6f6d 7074 223e 0a3c 2f64 6976 3e3c 6469  ompt">.</div><di
+000a2ff0: 7620 636c 6173 733d 226a 702d 5265 6e64  v class="jp-Rend
+000a3000: 6572 6564 4854 4d4c 436f 6d6d 6f6e 206a  eredHTMLCommon j
+000a3010: 702d 5265 6e64 6572 6564 4d61 726b 646f  p-RenderedMarkdo
+000a3020: 776e 206a 702d 4d61 726b 646f 776e 4f75  wn jp-MarkdownOu
+000a3030: 7470 7574 2022 2064 6174 612d 6d69 6d65  tput " data-mime
+000a3040: 2d74 7970 653d 2274 6578 742f 6d61 726b  -type="text/mark
+000a3050: 646f 776e 223e 0a0a 3c70 7265 3e3c 636f  down">..<pre><co
+000a3060: 6465 3e64 2920 4a6f 696e 696e 6720 7472  de>d) Joining tr
+000a3070: 6169 6e20 616e 6420 7465 7374 2066 696c  ain and test fil
+000a3080: 6573 3a3c 2f63 6f64 653e 3c2f 7072 653e  es:</code></pre>
+000a3090: 0a0a 3c2f 6469 763e 0a3c 2f64 6976 3e0a  ..</div>.</div>.
+000a30a0: 3c2f 6469 763e 0a3c 2f64 6976 3e3c 6469  </div>.</div><di
+000a30b0: 7620 636c 6173 733d 226a 702d 4365 6c6c  v class="jp-Cell
+000a30c0: 206a 702d 436f 6465 4365 6c6c 206a 702d   jp-CodeCell jp-
+000a30d0: 4e6f 7465 626f 6f6b 2d63 656c 6c20 2020  Notebook-cell   
+000a30e0: 223e 0a3c 6469 7620 636c 6173 733d 226a  ">.<div class="j
+000a30f0: 702d 4365 6c6c 2d69 6e70 7574 5772 6170  p-Cell-inputWrap
+000a3100: 7065 7222 3e0a 3c64 6976 2063 6c61 7373  per">.<div class
+000a3110: 3d22 6a70 2d43 6f6c 6c61 7073 6572 206a  ="jp-Collapser j
+000a3120: 702d 496e 7075 7443 6f6c 6c61 7073 6572  p-InputCollapser
+000a3130: 206a 702d 4365 6c6c 2d69 6e70 7574 436f   jp-Cell-inputCo
+000a3140: 6c6c 6170 7365 7222 3e0a 3c2f 6469 763e  llapser">.</div>
+000a3150: 0a3c 6469 7620 636c 6173 733d 226a 702d  .<div class="jp-
+000a3160: 496e 7075 7441 7265 6120 6a70 2d43 656c  InputArea jp-Cel
+000a3170: 6c2d 696e 7075 7441 7265 6122 3e0a 3c64  l-inputArea">.<d
+000a3180: 6976 2063 6c61 7373 3d22 6a70 2d49 6e70  iv class="jp-Inp
+000a3190: 7574 5072 6f6d 7074 206a 702d 496e 7075  utPrompt jp-Inpu
+000a31a0: 7441 7265 612d 7072 6f6d 7074 223e 496e  tArea-prompt">In
+000a31b0: 266e 6273 703b 5b32 385d 3a3c 2f64 6976  &nbsp;[28]:</div
+000a31c0: 3e0a 3c64 6976 2063 6c61 7373 3d22 6a70  >.<div class="jp
+000a31d0: 2d43 6f64 654d 6972 726f 7245 6469 746f  -CodeMirrorEdito
+000a31e0: 7220 6a70 2d45 6469 746f 7220 6a70 2d49  r jp-Editor jp-I
+000a31f0: 6e70 7574 4172 6561 2d65 6469 746f 7222  nputArea-editor"
+000a3200: 2064 6174 612d 7479 7065 3d22 696e 6c69   data-type="inli
+000a3210: 6e65 223e 0a20 2020 2020 3c64 6976 2063  ne">.     <div c
+000a3220: 6c61 7373 3d22 436f 6465 4d69 7272 6f72  lass="CodeMirror
+000a3230: 2063 6d2d 732d 6a75 7079 7465 7222 3e0a   cm-s-jupyter">.
+000a3240: 3c64 6976 2063 6c61 7373 3d22 2068 6967  <div class=" hig
+000a3250: 686c 6967 6874 2068 6c2d 6970 7974 686f  hlight hl-ipytho
+000a3260: 6e33 223e 3c70 7265 3e3c 7370 616e 3e3c  n3"><pre><span><
+000a3270: 2f73 7061 6e3e 3c73 7061 6e20 636c 6173  /span><span clas
+000a3280: 733d 226e 223e 6466 3c2f 7370 616e 3e20  s="n">df</span> 
+000a3290: 3c73 7061 6e20 636c 6173 733d 226f 223e  <span class="o">
+000a32a0: 3d3c 2f73 7061 6e3e 203c 7370 616e 2063  =</span> <span c
+000a32b0: 6c61 7373 3d22 6e22 3e6a 6f69 6e54 7261  lass="n">joinTra
+000a32c0: 696e 5465 7374 3c2f 7370 616e 3e3c 7370  inTest</span><sp
+000a32d0: 616e 2063 6c61 7373 3d22 7022 3e28 3c2f  an class="p">(</
+000a32e0: 7370 616e 3e3c 7370 616e 2063 6c61 7373  span><span class
+000a32f0: 3d22 6e22 3e64 6174 615f 7061 7468 3c2f  ="n">data_path</
+000a3300: 7370 616e 3e3c 7370 616e 2063 6c61 7373  span><span class
+000a3310: 3d22 7022 3e2c 3c2f 7370 616e 3e20 3c73  ="p">,</span> <s
+000a3320: 7061 6e20 636c 6173 733d 226e 223e 7472  pan class="n">tr
+000a3330: 6169 6e5f 6669 6c65 3c2f 7370 616e 3e3c  ain_file</span><
+000a3340: 7370 616e 2063 6c61 7373 3d22 6f22 3e3d  span class="o">=
+000a3350: 3c2f 7370 616e 3e3c 7370 616e 2063 6c61  </span><span cla
+000a3360: 7373 3d22 7332 223e 2671 756f 743b 7472  ss="s2">&quot;tr
+000a3370: 6169 6e2e 6373 7626 7175 6f74 3b3c 2f73  ain.csv&quot;</s
+000a3380: 7061 6e3e 3c73 7061 6e20 636c 6173 733d  pan><span class=
+000a3390: 2270 223e 2c3c 2f73 7061 6e3e 203c 7370  "p">,</span> <sp
+000a33a0: 616e 2063 6c61 7373 3d22 6e22 3e74 6573  an class="n">tes
+000a33b0: 745f 6669 6c65 3c2f 7370 616e 3e3c 7370  t_file</span><sp
+000a33c0: 616e 2063 6c61 7373 3d22 6f22 3e3d 3c2f  an class="o">=</
+000a33d0: 7370 616e 3e3c 7370 616e 2063 6c61 7373  span><span class
+000a33e0: 3d22 7332 223e 2671 756f 743b 7465 7374  ="s2">&quot;test
+000a33f0: 2e63 7376 2671 756f 743b 3c2f 7370 616e  .csv&quot;</span
+000a3400: 3e3c 7370 616e 2063 6c61 7373 3d22 7022  ><span class="p"
+000a3410: 3e2c 3c2f 7370 616e 3e20 3c73 7061 6e20  >,</span> <span 
+000a3420: 636c 6173 733d 226e 223e 746f 5f66 696c  class="n">to_fil
+000a3430: 653c 2f73 7061 6e3e 3c73 7061 6e20 636c  e</span><span cl
+000a3440: 6173 733d 226f 223e 3d3c 2f73 7061 6e3e  ass="o">=</span>
+000a3450: 3c73 7061 6e20 636c 6173 733d 226b 6322  <span class="kc"
+000a3460: 3e54 7275 653c 2f73 7061 6e3e 3c73 7061  >True</span><spa
+000a3470: 6e20 636c 6173 733d 2270 223e 293c 2f73  n class="p">)</s
+000a3480: 7061 6e3e 203c 7370 616e 2063 6c61 7373  pan> <span class
+000a3490: 3d22 6331 223e 2320 5361 7665 7320 2623  ="c1"># Saves &#
+000a34a0: 3339 3b6a 6f69 6e65 642e 6373 7626 2333  39;joined.csv&#3
+000a34b0: 393b 2066 696c 653c 2f73 7061 6e3e 0a0a  9; file</span>..
+000a34c0: 3c73 7061 6e20 636c 6173 733d 226e 223e  <span class="n">
+000a34d0: 6466 3c2f 7370 616e 3e3c 7370 616e 2063  df</span><span c
+000a34e0: 6c61 7373 3d22 6f22 3e2e 3c2f 7370 616e  lass="o">.</span
+000a34f0: 3e3c 7370 616e 2063 6c61 7373 3d22 6e22  ><span class="n"
+000a3500: 3e68 6561 643c 2f73 7061 6e3e 3c73 7061  >head</span><spa
+000a3510: 6e20 636c 6173 733d 2270 223e 2829 3c2f  n class="p">()</
+000a3520: 7370 616e 3e0a 3c2f 7072 653e 3c2f 6469  span>.</pre></di
+000a3530: 763e 0a0a 2020 2020 203c 2f64 6976 3e0a  v>..     </div>.
+000a3540: 3c2f 6469 763e 0a3c 2f64 6976 3e0a 3c2f  </div>.</div>.</
+000a3550: 6469 763e 0a0a 3c64 6976 2063 6c61 7373  div>..<div class
+000a3560: 3d22 6a70 2d43 656c 6c2d 6f75 7470 7574  ="jp-Cell-output
+000a3570: 5772 6170 7065 7222 3e0a 3c64 6976 2063  Wrapper">.<div c
+000a3580: 6c61 7373 3d22 6a70 2d43 6f6c 6c61 7073  lass="jp-Collaps
+000a3590: 6572 206a 702d 4f75 7470 7574 436f 6c6c  er jp-OutputColl
+000a35a0: 6170 7365 7220 6a70 2d43 656c 6c2d 6f75  apser jp-Cell-ou
+000a35b0: 7470 7574 436f 6c6c 6170 7365 7222 3e0a  tputCollapser">.
+000a35c0: 3c2f 6469 763e 0a0a 0a3c 6469 7620 636c  </div>...<div cl
+000a35d0: 6173 733d 226a 702d 4f75 7470 7574 4172  ass="jp-OutputAr
+000a35e0: 6561 206a 702d 4365 6c6c 2d6f 7574 7075  ea jp-Cell-outpu
+000a35f0: 7441 7265 6122 3e0a 0a3c 6469 7620 636c  tArea">..<div cl
+000a3600: 6173 733d 226a 702d 4f75 7470 7574 4172  ass="jp-OutputAr
+000a3610: 6561 2d63 6869 6c64 223e 0a0a 2020 2020  ea-child">..    
+000a3620: 0a20 2020 203c 6469 7620 636c 6173 733d  .    <div class=
+000a3630: 226a 702d 4f75 7470 7574 5072 6f6d 7074  "jp-OutputPrompt
+000a3640: 206a 702d 4f75 7470 7574 4172 6561 2d70   jp-OutputArea-p
+000a3650: 726f 6d70 7422 3e3c 2f64 6976 3e0a 0a0a  rompt"></div>...
+000a3660: 3c64 6976 2063 6c61 7373 3d22 6a70 2d52  <div class="jp-R
+000a3670: 656e 6465 7265 6454 6578 7420 6a70 2d4f  enderedText jp-O
+000a3680: 7574 7075 7441 7265 612d 6f75 7470 7574  utputArea-output
+000a3690: 2220 6461 7461 2d6d 696d 652d 7479 7065  " data-mime-type
+000a36a0: 3d22 7465 7874 2f70 6c61 696e 223e 0a3c  ="text/plain">.<
+000a36b0: 7072 653e 4a6f 696e 696e 6720 7472 6169  pre>Joining trai
+000a36c0: 6e20 616e 6420 7465 7374 2064 6174 6120  n and test data 
+000a36d0: 6672 6f6d 2e2e 2e20 6d61 7464 6174 612f  from... matdata/
+000a36e0: 6173 7365 7473 2f73 616d 706c 650a 5361  assets/sample.Sa
+000a36f0: 7669 6e67 206a 6f69 6e65 6420 6461 7461  ving joined data
+000a3700: 7365 7420 6173 3a20 6d61 7464 6174 612f  set as: matdata/
+000a3710: 6173 7365 7473 2f73 616d 706c 652f 6a6f  assets/sample/jo
+000a3720: 696e 6564 2e63 7376 0a44 6f6e 652e 0a20  ined.csv.Done.. 
+000a3730: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000a3740: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000a3750: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000a3760: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000a3770: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000a3780: 0a3c 2f70 7265 3e0a 3c2f 6469 763e 0a3c  .</pre>.</div>.<
+000a3790: 2f64 6976 3e0a 0a3c 6469 7620 636c 6173  /div>..<div clas
+000a37a0: 733d 226a 702d 4f75 7470 7574 4172 6561  s="jp-OutputArea
+000a37b0: 2d63 6869 6c64 223e 0a0a 2020 2020 0a20  -child">..    . 
+000a37c0: 2020 203c 6469 7620 636c 6173 733d 226a     <div class="j
+000a37d0: 702d 4f75 7470 7574 5072 6f6d 7074 206a  p-OutputPrompt j
+000a37e0: 702d 4f75 7470 7574 4172 6561 2d70 726f  p-OutputArea-pro
+000a37f0: 6d70 7422 3e4f 7574 5b32 385d 3a3c 2f64  mpt">Out[28]:</d
+000a3800: 6976 3e0a 0a0a 0a3c 6469 7620 636c 6173  iv>....<div clas
+000a3810: 733d 226a 702d 5265 6e64 6572 6564 4854  s="jp-RenderedHT
+000a3820: 4d4c 436f 6d6d 6f6e 206a 702d 5265 6e64  MLCommon jp-Rend
+000a3830: 6572 6564 4854 4d4c 206a 702d 4f75 7470  eredHTML jp-Outp
+000a3840: 7574 4172 6561 2d6f 7574 7075 7420 6a70  utArea-output jp
+000a3850: 2d4f 7574 7075 7441 7265 612d 6578 6563  -OutputArea-exec
+000a3860: 7574 6552 6573 756c 7422 2064 6174 612d  uteResult" data-
+000a3870: 6d69 6d65 2d74 7970 653d 2274 6578 742f  mime-type="text/
+000a3880: 6874 6d6c 223e 0a3c 6469 763e 0a3c 7374  html">.<div>.<st
+000a3890: 796c 6520 7363 6f70 6564 3e0a 2020 2020  yle scoped>.    
+000a38a0: 2e64 6174 6166 7261 6d65 2074 626f 6479  .dataframe tbody
+000a38b0: 2074 7220 7468 3a6f 6e6c 792d 6f66 2d74   tr th:only-of-t
+000a38c0: 7970 6520 7b0a 2020 2020 2020 2020 7665  ype {.        ve
+000a38d0: 7274 6963 616c 2d61 6c69 676e 3a20 6d69  rtical-align: mi
+000a38e0: 6464 6c65 3b0a 2020 2020 7d0a 0a20 2020  ddle;.    }..   
+000a38f0: 202e 6461 7461 6672 616d 6520 7462 6f64   .dataframe tbod
+000a3900: 7920 7472 2074 6820 7b0a 2020 2020 2020  y tr th {.      
+000a3910: 2020 7665 7274 6963 616c 2d61 6c69 676e    vertical-align
+000a3920: 3a20 746f 703b 0a20 2020 207d 0a0a 2020  : top;.    }..  
+000a3930: 2020 2e64 6174 6166 7261 6d65 2074 6865    .dataframe the
+000a3940: 6164 2074 6820 7b0a 2020 2020 2020 2020  ad th {.        
+000a3950: 7465 7874 2d61 6c69 676e 3a20 7269 6768  text-align: righ
+000a3960: 743b 0a20 2020 207d 0a3c 2f73 7479 6c65  t;.    }.</style
+000a3970: 3e0a 3c74 6162 6c65 2062 6f72 6465 723d  >.<table border=
+000a3980: 2231 2220 636c 6173 733d 2264 6174 6166  "1" class="dataf
+000a3990: 7261 6d65 223e 0a20 203c 7468 6561 643e  rame">.  <thead>
+000a39a0: 0a20 2020 203c 7472 2073 7479 6c65 3d22  .    <tr style="
+000a39b0: 7465 7874 2d61 6c69 676e 3a20 7269 6768  text-align: righ
+000a39c0: 743b 223e 0a20 2020 2020 203c 7468 3e3c  t;">.      <th><
+000a39d0: 2f74 683e 0a20 2020 2020 203c 7468 3e64  /th>.      <th>d
+000a39e0: 6174 655f 7469 6d65 3c2f 7468 3e0a 2020  ate_time</th>.  
+000a39f0: 2020 2020 3c74 683e 7469 6d65 3c2f 7468      <th>time</th
+000a3a00: 3e0a 2020 2020 2020 3c74 683e 7261 7469  >.      <th>rati
+000a3a10: 6e67 3c2f 7468 3e0a 2020 2020 2020 3c74  ng</th>.      <t
+000a3a20: 683e 7072 6963 653c 2f74 683e 0a20 2020  h>price</th>.   
+000a3a30: 2020 203c 7468 3e77 6561 7468 6572 3c2f     <th>weather</
+000a3a40: 7468 3e0a 2020 2020 2020 3c74 683e 6461  th>.      <th>da
+000a3a50: 793c 2f74 683e 0a20 2020 2020 203c 7468  y</th>.      <th
+000a3a60: 3e74 7970 653c 2f74 683e 0a20 2020 2020  >type</th>.     
+000a3a70: 203c 7468 3e6c 6174 3c2f 7468 3e0a 2020   <th>lat</th>.  
+000a3a80: 2020 2020 3c74 683e 6c6f 6e3c 2f74 683e      <th>lon</th>
+000a3a90: 0a20 2020 2020 203c 7468 3e74 6964 3c2f  .      <th>tid</
+000a3aa0: 7468 3e0a 2020 2020 2020 3c74 683e 6c61  th>.      <th>la
+000a3ab0: 6265 6c3c 2f74 683e 0a20 2020 203c 2f74  bel</th>.    </t
+000a3ac0: 723e 0a20 203c 2f74 6865 6164 3e0a 2020  r>.  </thead>.  
+000a3ad0: 3c74 626f 6479 3e0a 2020 2020 3c74 723e  <tbody>.    <tr>
+000a3ae0: 0a20 2020 2020 203c 7468 3e30 3c2f 7468  .      <th>0</th
+000a3af0: 3e0a 2020 2020 2020 3c74 643e 3230 3132  >.      <td>2012
+000a3b00: 2d31 312d 3132 2030 353a 3137 3a31 383c  -11-12 05:17:18<
+000a3b10: 2f74 643e 0a20 2020 2020 203c 7464 3e33  /td>.      <td>3
+000a3b20: 3137 3c2f 7464 3e0a 2020 2020 2020 3c74  17</td>.      <t
+000a3b30: 643e 2d31 2e30 3c2f 7464 3e0a 2020 2020  d>-1.0</td>.    
+000a3b40: 2020 3c74 643e 2d31 3c2f 7464 3e0a 2020    <td>-1</td>.  
+000a3b50: 2020 2020 3c74 643e 436c 6561 723c 2f74      <td>Clear</t
+000a3b60: 643e 0a20 2020 2020 203c 7464 3e4d 6f6e  d>.      <td>Mon
+000a3b70: 6461 793c 2f74 643e 0a20 2020 2020 203c  day</td>.      <
+000a3b80: 7464 3e48 6f6d 6520 2870 7269 7661 7465  td>Home (private
+000a3b90: 293c 2f74 643e 0a20 2020 2020 203c 7464  )</td>.      <td
+000a3ba0: 3e34 302e 3833 3331 3635 3c2f 7464 3e0a  >40.833165</td>.
+000a3bb0: 2020 2020 2020 3c74 643e 2d37 332e 3934        <td>-73.94
+000a3bc0: 3138 3630 3c2f 7464 3e0a 2020 2020 2020  1860</td>.      
+000a3bd0: 3c74 643e 3132 363c 2f74 643e 0a20 2020  <td>126</td>.   
+000a3be0: 2020 203c 7464 3e52 6573 6964 656e 6365     <td>Residence
+000a3bf0: 3c2f 7464 3e0a 2020 2020 3c2f 7472 3e0a  </td>.    </tr>.
+000a3c00: 2020 2020 3c74 723e 0a20 2020 2020 203c      <tr>.      <
+000a3c10: 7468 3e31 3c2f 7468 3e0a 2020 2020 2020  th>1</th>.      
+000a3c20: 3c74 643e 3230 3132 2d31 312d 3132 2032  <td>2012-11-12 2
+000a3c30: 333a 3234 3a35 353c 2f74 643e 0a20 2020  3:24:55</td>.   
+000a3c40: 2020 203c 7464 3e31 3430 343c 2f74 643e     <td>1404</td>
+000a3c50: 0a20 2020 2020 203c 7464 3e38 2e32 3c2f  .      <td>8.2</
+000a3c60: 7464 3e0a 2020 2020 2020 3c74 643e 313c  td>.      <td>1<
+000a3c70: 2f74 643e 0a20 2020 2020 203c 7464 3e43  /td>.      <td>C
+000a3c80: 6c6f 7564 733c 2f74 643e 0a20 2020 2020  louds</td>.     
+000a3c90: 203c 7464 3e4d 6f6e 6461 793c 2f74 643e   <td>Monday</td>
+000a3ca0: 0a20 2020 2020 203c 7464 3e44 656c 6920  .      <td>Deli 
+000a3cb0: 2f20 426f 6465 6761 3c2f 7464 3e0a 2020  / Bodega</td>.  
+000a3cc0: 2020 2020 3c74 643e 3430 2e38 3334 3039      <td>40.83409
+000a3cd0: 383c 2f74 643e 0a20 2020 2020 203c 7464  8</td>.      <td
+000a3ce0: 3e2d 3733 2e39 3435 3236 373c 2f74 643e  >-73.945267</td>
+000a3cf0: 0a20 2020 2020 203c 7464 3e31 3236 3c2f  .      <td>126</
+000a3d00: 7464 3e0a 2020 2020 2020 3c74 643e 466f  td>.      <td>Fo
+000a3d10: 6f64 3c2f 7464 3e0a 2020 2020 3c2f 7472  od</td>.    </tr
+000a3d20: 3e0a 2020 2020 3c74 723e 0a20 2020 2020  >.    <tr>.     
+000a3d30: 203c 7468 3e32 3c2f 7468 3e0a 2020 2020   <th>2</th>.    
+000a3d40: 2020 3c74 643e 3230 3132 2d31 312d 3133    <td>2012-11-13
+000a3d50: 2030 303a 3030 3a30 373c 2f74 643e 0a20   00:00:07</td>. 
+000a3d60: 2020 2020 203c 7464 3e30 3c2f 7464 3e0a       <td>0</td>.
+000a3d70: 2020 2020 2020 3c74 643e 2d31 2e30 3c2f        <td>-1.0</
+000a3d80: 7464 3e0a 2020 2020 2020 3c74 643e 2d31  td>.      <td>-1
+000a3d90: 3c2f 7464 3e0a 2020 2020 2020 3c74 643e  </td>.      <td>
+000a3da0: 436c 6f75 6473 3c2f 7464 3e0a 2020 2020  Clouds</td>.    
+000a3db0: 2020 3c74 643e 5475 6573 6461 793c 2f74    <td>Tuesday</t
+000a3dc0: 643e 0a20 2020 2020 203c 7464 3e48 6f6d  d>.      <td>Hom
+000a3dd0: 6520 2870 7269 7661 7465 293c 2f74 643e  e (private)</td>
+000a3de0: 0a20 2020 2020 203c 7464 3e34 302e 3833  .      <td>40.83
+000a3df0: 3331 3635 3c2f 7464 3e0a 2020 2020 2020  3165</td>.      
+000a3e00: 3c74 643e 2d37 332e 3934 3138 3630 3c2f  <td>-73.941860</
+000a3e10: 7464 3e0a 2020 2020 2020 3c74 643e 3132  td>.      <td>12
+000a3e20: 363c 2f74 643e 0a20 2020 2020 203c 7464  6</td>.      <td
+000a3e30: 3e52 6573 6964 656e 6365 3c2f 7464 3e0a  >Residence</td>.
+000a3e40: 2020 2020 3c2f 7472 3e0a 2020 2020 3c74      </tr>.    <t
+000a3e50: 723e 0a20 2020 2020 203c 7468 3e33 3c2f  r>.      <th>3</
+000a3e60: 7468 3e0a 2020 2020 2020 3c74 643e 3230  th>.      <td>20
+000a3e70: 3132 2d31 312d 3135 2031 373a 3439 3a30  12-11-15 17:49:0
+000a3e80: 313c 2f74 643e 0a20 2020 2020 203c 7464  1</td>.      <td
+000a3e90: 3e31 3036 393c 2f74 643e 0a20 2020 2020  >1069</td>.     
+000a3ea0: 203c 7464 3e36 2e36 3c2f 7464 3e0a 2020   <td>6.6</td>.  
+000a3eb0: 2020 2020 3c74 643e 333c 2f74 643e 0a20      <td>3</td>. 
+000a3ec0: 2020 2020 203c 7464 3e43 6c65 6172 3c2f       <td>Clear</
+000a3ed0: 7464 3e0a 2020 2020 2020 3c74 643e 5468  td>.      <td>Th
+000a3ee0: 7572 7364 6179 3c2f 7464 3e0a 2020 2020  ursday</td>.    
+000a3ef0: 2020 3c74 643e 4672 6965 6420 4368 6963    <td>Fried Chic
+000a3f00: 6b65 6e20 4a6f 696e 743c 2f74 643e 0a20  ken Joint</td>. 
+000a3f10: 2020 2020 203c 7464 3e34 302e 3736 3436       <td>40.7646
+000a3f20: 3936 3c2f 7464 3e0a 2020 2020 2020 3c74  96</td>.      <t
+000a3f30: 643e 2d37 332e 3838 3531 3937 3c2f 7464  d>-73.885197</td
+000a3f40: 3e0a 2020 2020 2020 3c74 643e 3132 363c  >.      <td>126<
+000a3f50: 2f74 643e 0a20 2020 2020 203c 7464 3e46  /td>.      <td>F
+000a3f60: 6f6f 643c 2f74 643e 0a20 2020 203c 2f74  ood</td>.    </t
+000a3f70: 723e 0a20 2020 203c 7472 3e0a 2020 2020  r>.    <tr>.    
+000a3f80: 2020 3c74 683e 343c 2f74 683e 0a20 2020    <th>4</th>.   
+000a3f90: 2020 203c 7464 3e32 3031 322d 3131 2d31     <td>2012-11-1
+000a3fa0: 3520 3138 3a34 303a 3136 3c2f 7464 3e0a  5 18:40:16</td>.
+000a3fb0: 2020 2020 2020 3c74 643e 3131 3230 3c2f        <td>1120</
+000a3fc0: 7464 3e0a 2020 2020 2020 3c74 643e 2d31  td>.      <td>-1
+000a3fd0: 2e30 3c2f 7464 3e0a 2020 2020 2020 3c74  .0</td>.      <t
+000a3fe0: 643e 2d31 3c2f 7464 3e0a 2020 2020 2020  d>-1</td>.      
+000a3ff0: 3c74 643e 436c 6561 723c 2f74 643e 0a20  <td>Clear</td>. 
+000a4000: 2020 2020 203c 7464 3e54 6875 7273 6461       <td>Thursda
+000a4010: 793c 2f74 643e 0a20 2020 2020 203c 7464  y</td>.      <td
+000a4020: 3e42 7573 2053 7461 7469 6f6e 3c2f 7464  >Bus Station</td
+000a4030: 3e0a 2020 2020 2020 3c74 643e 3430 2e37  >.      <td>40.7
+000a4040: 3636 3037 393c 2f74 643e 0a20 2020 2020  66079</td>.     
+000a4050: 203c 7464 3e2d 3733 2e38 3833 3532 393c   <td>-73.883529<
+000a4060: 2f74 643e 0a20 2020 2020 203c 7464 3e31  /td>.      <td>1
+000a4070: 3236 3c2f 7464 3e0a 2020 2020 2020 3c74  26</td>.      <t
+000a4080: 643e 5472 6176 656c 2026 616d 703b 2054  d>Travel &amp; T
+000a4090: 7261 6e73 706f 7274 3c2f 7464 3e0a 2020  ransport</td>.  
+000a40a0: 2020 3c2f 7472 3e0a 2020 3c2f 7462 6f64    </tr>.  </tbod
+000a40b0: 793e 0a3c 2f74 6162 6c65 3e0a 3c2f 6469  y>.</table>.</di
+000a40c0: 763e 0a3c 2f64 6976 3e0a 0a3c 2f64 6976  v>.</div>..</div
+000a40d0: 3e0a 0a3c 2f64 6976 3e0a 0a3c 2f64 6976  >..</div>..</div
+000a40e0: 3e0a 0a3c 2f64 6976 3e0a 3c64 6976 2063  >..</div>.<div c
+000a40f0: 6c61 7373 3d22 6a70 2d43 656c 6c20 6a70  lass="jp-Cell jp
+000a4100: 2d4d 6172 6b64 6f77 6e43 656c 6c20 6a70  -MarkdownCell jp
+000a4110: 2d4e 6f74 6562 6f6f 6b2d 6365 6c6c 223e  -Notebook-cell">
+000a4120: 0a3c 6469 7620 636c 6173 733d 226a 702d  .<div class="jp-
+000a4130: 4365 6c6c 2d69 6e70 7574 5772 6170 7065  Cell-inputWrappe
+000a4140: 7222 3e0a 3c64 6976 2063 6c61 7373 3d22  r">.<div class="
+000a4150: 6a70 2d43 6f6c 6c61 7073 6572 206a 702d  jp-Collapser jp-
+000a4160: 496e 7075 7443 6f6c 6c61 7073 6572 206a  InputCollapser j
+000a4170: 702d 4365 6c6c 2d69 6e70 7574 436f 6c6c  p-Cell-inputColl
+000a4180: 6170 7365 7222 3e0a 3c2f 6469 763e 0a3c  apser">.</div>.<
+000a4190: 6469 7620 636c 6173 733d 226a 702d 496e  div class="jp-In
+000a41a0: 7075 7441 7265 6120 6a70 2d43 656c 6c2d  putArea jp-Cell-
+000a41b0: 696e 7075 7441 7265 6122 3e3c 6469 7620  inputArea"><div 
+000a41c0: 636c 6173 733d 226a 702d 496e 7075 7450  class="jp-InputP
+000a41d0: 726f 6d70 7420 6a70 2d49 6e70 7574 4172  rompt jp-InputAr
+000a41e0: 6561 2d70 726f 6d70 7422 3e0a 3c2f 6469  ea-prompt">.</di
+000a41f0: 763e 3c64 6976 2063 6c61 7373 3d22 6a70  v><div class="jp
+000a4200: 2d52 656e 6465 7265 6448 544d 4c43 6f6d  -RenderedHTMLCom
+000a4210: 6d6f 6e20 6a70 2d52 656e 6465 7265 644d  mon jp-RenderedM
+000a4220: 6172 6b64 6f77 6e20 6a70 2d4d 6172 6b64  arkdown jp-Markd
+000a4230: 6f77 6e4f 7574 7075 7420 2220 6461 7461  ownOutput " data
+000a4240: 2d6d 696d 652d 7479 7065 3d22 7465 7874  -mime-type="text
+000a4250: 2f6d 6172 6b64 6f77 6e22 3e0a 3c70 3e3c  /markdown">.<p><
+000a4260: 7374 726f 6e67 3e4e 6f74 653a 3c2f 7374  strong>Note:</st
+000a4270: 726f 6e67 3e20 5765 2073 7461 6e64 6172  rong> We standar
+000a4280: 6469 7a65 6420 616c 6c20 7265 706f 7369  dized all reposi
+000a4290: 746f 7279 2064 6174 6173 6574 7320 6279  tory datasets by
+000a42a0: 2063 7265 6174 696e 6720 6120 3c63 6f64   creating a <cod
+000a42b0: 653e 6461 7461 2e70 6172 7175 6574 3c2f  e>data.parquet</
+000a42c0: 636f 6465 3e20 6669 6c65 2077 6974 6820  code> file with 
+000a42d0: 3c63 6f64 653e 6e70 2e4e 614e 3c2f 636f  <code>np.NaN</co
+000a42e0: 6465 3e20 6173 206d 6973 7369 6e67 2076  de> as missing v
+000a42f0: 616c 7565 732c 2061 7320 6578 616d 706c  alues, as exampl
+000a4300: 653a 3c2f 703e 0a0a 3c2f 6469 763e 0a3c  e:</p>..</div>.<
+000a4310: 2f64 6976 3e0a 3c2f 6469 763e 0a3c 2f64  /div>.</div>.</d
+000a4320: 6976 3e3c 6469 7620 636c 6173 733d 226a  iv><div class="j
+000a4330: 702d 4365 6c6c 206a 702d 436f 6465 4365  p-Cell jp-CodeCe
+000a4340: 6c6c 206a 702d 4e6f 7465 626f 6f6b 2d63  ll jp-Notebook-c
+000a4350: 656c 6c20 2020 223e 0a3c 6469 7620 636c  ell   ">.<div cl
+000a4360: 6173 733d 226a 702d 4365 6c6c 2d69 6e70  ass="jp-Cell-inp
+000a4370: 7574 5772 6170 7065 7222 3e0a 3c64 6976  utWrapper">.<div
+000a4380: 2063 6c61 7373 3d22 6a70 2d43 6f6c 6c61   class="jp-Colla
+000a4390: 7073 6572 206a 702d 496e 7075 7443 6f6c  pser jp-InputCol
+000a43a0: 6c61 7073 6572 206a 702d 4365 6c6c 2d69  lapser jp-Cell-i
+000a43b0: 6e70 7574 436f 6c6c 6170 7365 7222 3e0a  nputCollapser">.
+000a43c0: 3c2f 6469 763e 0a3c 6469 7620 636c 6173  </div>.<div clas
+000a43d0: 733d 226a 702d 496e 7075 7441 7265 6120  s="jp-InputArea 
+000a43e0: 6a70 2d43 656c 6c2d 696e 7075 7441 7265  jp-Cell-inputAre
+000a43f0: 6122 3e0a 3c64 6976 2063 6c61 7373 3d22  a">.<div class="
+000a4400: 6a70 2d49 6e70 7574 5072 6f6d 7074 206a  jp-InputPrompt j
+000a4410: 702d 496e 7075 7441 7265 612d 7072 6f6d  p-InputArea-prom
+000a4420: 7074 223e 496e 266e 6273 703b 5b32 395d  pt">In&nbsp;[29]
+000a4430: 3a3c 2f64 6976 3e0a 3c64 6976 2063 6c61  :</div>.<div cla
+000a4440: 7373 3d22 6a70 2d43 6f64 654d 6972 726f  ss="jp-CodeMirro
+000a4450: 7245 6469 746f 7220 6a70 2d45 6469 746f  rEditor jp-Edito
+000a4460: 7220 6a70 2d49 6e70 7574 4172 6561 2d65  r jp-InputArea-e
+000a4470: 6469 746f 7222 2064 6174 612d 7479 7065  ditor" data-type
+000a4480: 3d22 696e 6c69 6e65 223e 0a20 2020 2020  ="inline">.     
+000a4490: 3c64 6976 2063 6c61 7373 3d22 436f 6465  <div class="Code
+000a44a0: 4d69 7272 6f72 2063 6d2d 732d 6a75 7079  Mirror cm-s-jupy
+000a44b0: 7465 7222 3e0a 3c64 6976 2063 6c61 7373  ter">.<div class
+000a44c0: 3d22 2068 6967 686c 6967 6874 2068 6c2d  =" highlight hl-
+000a44d0: 6970 7974 686f 6e33 223e 3c70 7265 3e3c  ipython3"><pre><
+000a44e0: 7370 616e 3e3c 2f73 7061 6e3e 3c73 7061  span></span><spa
+000a44f0: 6e20 636c 6173 733d 226b 6e22 3e66 726f  n class="kn">fro
+000a4500: 6d3c 2f73 7061 6e3e 203c 7370 616e 2063  m</span> <span c
+000a4510: 6c61 7373 3d22 6e6e 223e 6d61 7464 6174  lass="nn">matdat
+000a4520: 612e 7072 6570 726f 6365 7373 3c2f 7370  a.preprocess</sp
+000a4530: 616e 3e20 3c73 7061 6e20 636c 6173 733d  an> <span class=
+000a4540: 226b 6e22 3e69 6d70 6f72 743c 2f73 7061  "kn">import</spa
+000a4550: 6e3e 203c 7370 616e 2063 6c61 7373 3d22  n> <span class="
+000a4560: 6f22 3e2a 3c2f 7370 616e 3e0a 3c73 7061  o">*</span>.<spa
+000a4570: 6e20 636c 6173 733d 226b 6e22 3e66 726f  n class="kn">fro
+000a4580: 6d3c 2f73 7061 6e3e 203c 7370 616e 2063  m</span> <span c
+000a4590: 6c61 7373 3d22 6e6e 223e 6d61 7464 6174  lass="nn">matdat
+000a45a0: 612e 6461 7461 7365 743c 2f73 7061 6e3e  a.dataset</span>
+000a45b0: 203c 7370 616e 2063 6c61 7373 3d22 6b6e   <span class="kn
+000a45c0: 223e 696d 706f 7274 3c2f 7370 616e 3e20  ">import</span> 
+000a45d0: 3c73 7061 6e20 636c 6173 733d 226e 223e  <span class="n">
+000a45e0: 7072 6570 6172 655f 6473 3c2f 7370 616e  prepare_ds</span
+000a45f0: 3e0a 3c73 7061 6e20 636c 6173 733d 226b  >.<span class="k
+000a4600: 6e22 3e69 6d70 6f72 743c 2f73 7061 6e3e  n">import</span>
+000a4610: 203c 7370 616e 2063 6c61 7373 3d22 6e6e   <span class="nn
+000a4620: 223e 6e75 6d70 793c 2f73 7061 6e3e 203c  ">numpy</span> <
+000a4630: 7370 616e 2063 6c61 7373 3d22 6b22 3e61  span class="k">a
+000a4640: 733c 2f73 7061 6e3e 203c 7370 616e 2063  s</span> <span c
+000a4650: 6c61 7373 3d22 6e6e 223e 6e70 3c2f 7370  lass="nn">np</sp
+000a4660: 616e 3e0a 0a3c 7370 616e 2063 6c61 7373  an>..<span class
+000a4670: 3d22 6e22 3e64 6174 615f 7061 7468 3c2f  ="n">data_path</
+000a4680: 7370 616e 3e20 3c73 7061 6e20 636c 6173  span> <span clas
+000a4690: 733d 226f 223e 3d3c 2f73 7061 6e3e 203c  s="o">=</span> <
+000a46a0: 7370 616e 2063 6c61 7373 3d22 7331 223e  span class="s1">
+000a46b0: 2623 3339 3b6d 6174 6461 7461 2f61 7373  &#39;matdata/ass
+000a46c0: 6574 732f 7361 6d70 6c65 2623 3339 3b3c  ets/sample&#39;<
+000a46d0: 2f73 7061 6e3e 0a0a 3c73 7061 6e20 636c  /span>..<span cl
+000a46e0: 6173 733d 226e 223e 6466 3c2f 7370 616e  ass="n">df</span
+000a46f0: 3e3c 7370 616e 2063 6c61 7373 3d22 6f22  ><span class="o"
+000a4700: 3e2e 3c2f 7370 616e 3e3c 7370 616e 2063  >.</span><span c
+000a4710: 6c61 7373 3d22 6e22 3e72 6570 6c61 6365  lass="n">replace
+000a4720: 3c2f 7370 616e 3e3c 7370 616e 2063 6c61  </span><span cla
+000a4730: 7373 3d22 7022 3e28 3c2f 7370 616e 3e3c  ss="p">(</span><
+000a4740: 7370 616e 2063 6c61 7373 3d22 7331 223e  span class="s1">
+000a4750: 2623 3339 3b3f 2623 3339 3b3c 2f73 7061  &#39;?&#39;</spa
+000a4760: 6e3e 3c73 7061 6e20 636c 6173 733d 2270  n><span class="p
+000a4770: 223e 2c3c 2f73 7061 6e3e 203c 7370 616e  ">,</span> <span
+000a4780: 2063 6c61 7373 3d22 6e22 3e6e 703c 2f73   class="n">np</s
+000a4790: 7061 6e3e 3c73 7061 6e20 636c 6173 733d  pan><span class=
+000a47a0: 226f 223e 2e3c 2f73 7061 6e3e 3c73 7061  "o">.</span><spa
+000a47b0: 6e20 636c 6173 733d 226e 223e 4e61 4e3c  n class="n">NaN<
+000a47c0: 2f73 7061 6e3e 3c73 7061 6e20 636c 6173  /span><span clas
+000a47d0: 733d 2270 223e 2c3c 2f73 7061 6e3e 203c  s="p">,</span> <
+000a47e0: 7370 616e 2063 6c61 7373 3d22 6e22 3e69  span class="n">i
+000a47f0: 6e70 6c61 6365 3c2f 7370 616e 3e3c 7370  nplace</span><sp
+000a4800: 616e 2063 6c61 7373 3d22 6f22 3e3d 3c2f  an class="o">=</
+000a4810: 7370 616e 3e3c 7370 616e 2063 6c61 7373  span><span class
+000a4820: 3d22 6b63 223e 5472 7565 3c2f 7370 616e  ="kc">True</span
+000a4830: 3e3c 7370 616e 2063 6c61 7373 3d22 7022  ><span class="p"
+000a4840: 3e29 3c2f 7370 616e 3e0a 0a3c 7370 616e  >)</span>..<span
+000a4850: 2063 6c61 7373 3d22 6e22 3e64 663c 2f73   class="n">df</s
+000a4860: 7061 6e3e 203c 7370 616e 2063 6c61 7373  pan> <span class
+000a4870: 3d22 6f22 3e3d 3c2f 7370 616e 3e20 3c73  ="o">=</span> <s
+000a4880: 7061 6e20 636c 6173 733d 226e 223e 7072  pan class="n">pr
+000a4890: 6570 6172 655f 6473 3c2f 7370 616e 3e3c  epare_ds</span><
+000a48a0: 7370 616e 2063 6c61 7373 3d22 7022 3e28  span class="p">(
+000a48b0: 3c2f 7370 616e 3e3c 7370 616e 2063 6c61  </span><span cla
+000a48c0: 7373 3d22 6e22 3e64 663c 2f73 7061 6e3e  ss="n">df</span>
+000a48d0: 3c73 7061 6e20 636c 6173 733d 2270 223e  <span class="p">
+000a48e0: 293c 2f73 7061 6e3e 0a0a 3c73 7061 6e20  )</span>..<span 
+000a48f0: 636c 6173 733d 226e 223e 6466 3270 6172  class="n">df2par
+000a4900: 7175 6574 3c2f 7370 616e 3e3c 7370 616e  quet</span><span
+000a4910: 2063 6c61 7373 3d22 7022 3e28 3c2f 7370   class="p">(</sp
+000a4920: 616e 3e3c 7370 616e 2063 6c61 7373 3d22  an><span class="
+000a4930: 6e22 3e64 663c 2f73 7061 6e3e 3c73 7061  n">df</span><spa
+000a4940: 6e20 636c 6173 733d 2270 223e 2c3c 2f73  n class="p">,</s
+000a4950: 7061 6e3e 203c 7370 616e 2063 6c61 7373  pan> <span class
+000a4960: 3d22 6e22 3e64 6174 615f 7061 7468 3c2f  ="n">data_path</
+000a4970: 7370 616e 3e3c 7370 616e 2063 6c61 7373  span><span class
+000a4980: 3d22 7022 3e2c 3c2f 7370 616e 3e20 3c73  ="p">,</span> <s
+000a4990: 7061 6e20 636c 6173 733d 2273 3122 3e26  pan class="s1">&
+000a49a0: 2333 393b 6461 7461 2623 3339 3b3c 2f73  #39;data&#39;</s
+000a49b0: 7061 6e3e 3c73 7061 6e20 636c 6173 733d  pan><span class=
+000a49c0: 2270 223e 293c 2f73 7061 6e3e 0a3c 2f70  "p">)</span>.</p
+000a49d0: 7265 3e3c 2f64 6976 3e0a 0a20 2020 2020  re></div>..     
+000a49e0: 3c2f 6469 763e 0a3c 2f64 6976 3e0a 3c2f  </div>.</div>.</
+000a49f0: 6469 763e 0a3c 2f64 6976 3e0a 0a3c 6469  div>.</div>..<di
+000a4a00: 7620 636c 6173 733d 226a 702d 4365 6c6c  v class="jp-Cell
+000a4a10: 2d6f 7574 7075 7457 7261 7070 6572 223e  -outputWrapper">
+000a4a20: 0a3c 6469 7620 636c 6173 733d 226a 702d  .<div class="jp-
+000a4a30: 436f 6c6c 6170 7365 7220 6a70 2d4f 7574  Collapser jp-Out
+000a4a40: 7075 7443 6f6c 6c61 7073 6572 206a 702d  putCollapser jp-
+000a4a50: 4365 6c6c 2d6f 7574 7075 7443 6f6c 6c61  Cell-outputColla
+000a4a60: 7073 6572 223e 0a3c 2f64 6976 3e0a 0a0a  pser">.</div>...
+000a4a70: 3c64 6976 2063 6c61 7373 3d22 6a70 2d4f  <div class="jp-O
+000a4a80: 7574 7075 7441 7265 6120 6a70 2d43 656c  utputArea jp-Cel
+000a4a90: 6c2d 6f75 7470 7574 4172 6561 223e 0a0a  l-outputArea">..
+000a4aa0: 3c64 6976 2063 6c61 7373 3d22 6a70 2d4f  <div class="jp-O
+000a4ab0: 7574 7075 7441 7265 612d 6368 696c 6422  utputArea-child"
+000a4ac0: 3e0a 0a20 2020 200a 2020 2020 3c64 6976  >..    .    <div
+000a4ad0: 2063 6c61 7373 3d22 6a70 2d4f 7574 7075   class="jp-Outpu
+000a4ae0: 7450 726f 6d70 7420 6a70 2d4f 7574 7075  tPrompt jp-Outpu
+000a4af0: 7441 7265 612d 7072 6f6d 7074 223e 3c2f  tArea-prompt"></
+000a4b00: 6469 763e 0a0a 0a3c 6469 7620 636c 6173  div>...<div clas
+000a4b10: 733d 226a 702d 5265 6e64 6572 6564 5465  s="jp-RenderedTe
+000a4b20: 7874 206a 702d 4f75 7470 7574 4172 6561  xt jp-OutputArea
+000a4b30: 2d6f 7574 7075 7422 2064 6174 612d 6d69  -output" data-mi
+000a4b40: 6d65 2d74 7970 653d 2274 6578 742f 706c  me-type="text/pl
+000a4b50: 6169 6e22 3e0a 3c70 7265 3e53 6176 696e  ain">.<pre>Savin
+000a4b60: 6720 6461 7461 7365 7420 6173 3a20 6d61  g dataset as: ma
+000a4b70: 7464 6174 612f 6173 7365 7473 2f73 616d  tdata/assets/sam
+000a4b80: 706c 652f 6461 7461 2e70 6172 7175 6574  ple/data.parquet
+000a4b90: 0a44 6f6e 652e 0a20 2d2d 2d2d 2d2d 2d2d  .Done.. --------
+000a4ba0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000a4bb0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000a4bc0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000a4bd0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000a4be0: 2d2d 2d2d 2d2d 2d2d 0a3c 2f70 7265 3e0a  --------.</pre>.
+000a4bf0: 3c2f 6469 763e 0a3c 2f64 6976 3e0a 0a3c  </div>.</div>..<
+000a4c00: 6469 7620 636c 6173 733d 226a 702d 4f75  div class="jp-Ou
+000a4c10: 7470 7574 4172 6561 2d63 6869 6c64 223e  tputArea-child">
+000a4c20: 0a0a 2020 2020 0a20 2020 203c 6469 7620  ..    .    <div 
+000a4c30: 636c 6173 733d 226a 702d 4f75 7470 7574  class="jp-Output
+000a4c40: 5072 6f6d 7074 206a 702d 4f75 7470 7574  Prompt jp-Output
+000a4c50: 4172 6561 2d70 726f 6d70 7422 3e4f 7574  Area-prompt">Out
+000a4c60: 5b32 395d 3a3c 2f64 6976 3e0a 0a0a 0a3c  [29]:</div>....<
+000a4c70: 6469 7620 636c 6173 733d 226a 702d 5265  div class="jp-Re
+000a4c80: 6e64 6572 6564 4854 4d4c 436f 6d6d 6f6e  nderedHTMLCommon
+000a4c90: 206a 702d 5265 6e64 6572 6564 4854 4d4c   jp-RenderedHTML
+000a4ca0: 206a 702d 4f75 7470 7574 4172 6561 2d6f   jp-OutputArea-o
+000a4cb0: 7574 7075 7420 6a70 2d4f 7574 7075 7441  utput jp-OutputA
+000a4cc0: 7265 612d 6578 6563 7574 6552 6573 756c  rea-executeResul
+000a4cd0: 7422 2064 6174 612d 6d69 6d65 2d74 7970  t" data-mime-typ
+000a4ce0: 653d 2274 6578 742f 6874 6d6c 223e 0a3c  e="text/html">.<
+000a4cf0: 6469 763e 0a3c 7374 796c 6520 7363 6f70  div>.<style scop
+000a4d00: 6564 3e0a 2020 2020 2e64 6174 6166 7261  ed>.    .datafra
+000a4d10: 6d65 2074 626f 6479 2074 7220 7468 3a6f  me tbody tr th:o
+000a4d20: 6e6c 792d 6f66 2d74 7970 6520 7b0a 2020  nly-of-type {.  
+000a4d30: 2020 2020 2020 7665 7274 6963 616c 2d61        vertical-a
+000a4d40: 6c69 676e 3a20 6d69 6464 6c65 3b0a 2020  lign: middle;.  
+000a4d50: 2020 7d0a 0a20 2020 202e 6461 7461 6672    }..    .datafr
+000a4d60: 616d 6520 7462 6f64 7920 7472 2074 6820  ame tbody tr th 
+000a4d70: 7b0a 2020 2020 2020 2020 7665 7274 6963  {.        vertic
+000a4d80: 616c 2d61 6c69 676e 3a20 746f 703b 0a20  al-align: top;. 
+000a4d90: 2020 207d 0a0a 2020 2020 2e64 6174 6166     }..    .dataf
+000a4da0: 7261 6d65 2074 6865 6164 2074 6820 7b0a  rame thead th {.
+000a4db0: 2020 2020 2020 2020 7465 7874 2d61 6c69          text-ali
+000a4dc0: 676e 3a20 7269 6768 743b 0a20 2020 207d  gn: right;.    }
+000a4dd0: 0a3c 2f73 7479 6c65 3e0a 3c74 6162 6c65  .</style>.<table
+000a4de0: 2062 6f72 6465 723d 2231 2220 636c 6173   border="1" clas
+000a4df0: 733d 2264 6174 6166 7261 6d65 223e 0a20  s="dataframe">. 
+000a4e00: 203c 7468 6561 643e 0a20 2020 203c 7472   <thead>.    <tr
+000a4e10: 2073 7479 6c65 3d22 7465 7874 2d61 6c69   style="text-ali
+000a4e20: 676e 3a20 7269 6768 743b 223e 0a20 2020  gn: right;">.   
+000a4e30: 2020 203c 7468 3e3c 2f74 683e 0a20 2020     <th></th>.   
+000a4e40: 2020 203c 7468 3e64 6174 655f 7469 6d65     <th>date_time
+000a4e50: 3c2f 7468 3e0a 2020 2020 2020 3c74 683e  </th>.      <th>
+000a4e60: 7469 6d65 3c2f 7468 3e0a 2020 2020 2020  time</th>.      
+000a4e70: 3c74 683e 7261 7469 6e67 3c2f 7468 3e0a  <th>rating</th>.
+000a4e80: 2020 2020 2020 3c74 683e 7072 6963 653c        <th>price<
+000a4e90: 2f74 683e 0a20 2020 2020 203c 7468 3e77  /th>.      <th>w
+000a4ea0: 6561 7468 6572 3c2f 7468 3e0a 2020 2020  eather</th>.    
+000a4eb0: 2020 3c74 683e 6461 793c 2f74 683e 0a20    <th>day</th>. 
+000a4ec0: 2020 2020 203c 7468 3e74 7970 653c 2f74       <th>type</t
+000a4ed0: 683e 0a20 2020 2020 203c 7468 3e6c 6174  h>.      <th>lat
+000a4ee0: 3c2f 7468 3e0a 2020 2020 2020 3c74 683e  </th>.      <th>
+000a4ef0: 6c6f 6e3c 2f74 683e 0a20 2020 2020 203c  lon</th>.      <
+000a4f00: 7468 3e6c 6162 656c 3c2f 7468 3e0a 2020  th>label</th>.  
+000a4f10: 2020 2020 3c74 683e 7469 643c 2f74 683e      <th>tid</th>
+000a4f20: 0a20 2020 203c 2f74 723e 0a20 203c 2f74  .    </tr>.  </t
+000a4f30: 6865 6164 3e0a 2020 3c74 626f 6479 3e0a  head>.  <tbody>.
+000a4f40: 2020 2020 3c74 723e 0a20 2020 2020 203c      <tr>.      <
+000a4f50: 7468 3e30 3c2f 7468 3e0a 2020 2020 2020  th>0</th>.      
+000a4f60: 3c74 643e 3230 3132 2d31 312d 3132 2030  <td>2012-11-12 0
+000a4f70: 353a 3137 3a31 383c 2f74 643e 0a20 2020  5:17:18</td>.   
+000a4f80: 2020 203c 7464 3e33 3137 3c2f 7464 3e0a     <td>317</td>.
+000a4f90: 2020 2020 2020 3c74 643e 2d31 2e30 3c2f        <td>-1.0</
+000a4fa0: 7464 3e0a 2020 2020 2020 3c74 643e 2d31  td>.      <td>-1
+000a4fb0: 3c2f 7464 3e0a 2020 2020 2020 3c74 643e  </td>.      <td>
+000a4fc0: 436c 6561 723c 2f74 643e 0a20 2020 2020  Clear</td>.     
+000a4fd0: 203c 7464 3e4d 6f6e 6461 793c 2f74 643e   <td>Monday</td>
+000a4fe0: 0a20 2020 2020 203c 7464 3e48 6f6d 6520  .      <td>Home 
+000a4ff0: 2870 7269 7661 7465 293c 2f74 643e 0a20  (private)</td>. 
+000a5000: 2020 2020 203c 7464 3e34 302e 3833 3331       <td>40.8331
+000a5010: 3635 3c2f 7464 3e0a 2020 2020 2020 3c74  65</td>.      <t
+000a5020: 643e 2d37 332e 3934 3138 3630 3c2f 7464  d>-73.941860</td
+000a5030: 3e0a 2020 2020 2020 3c74 643e 5265 7369  >.      <td>Resi
+000a5040: 6465 6e63 653c 2f74 643e 0a20 2020 2020  dence</td>.     
+000a5050: 203c 7464 3e31 3236 3c2f 7464 3e0a 2020   <td>126</td>.  
+000a5060: 2020 3c2f 7472 3e0a 2020 2020 3c74 723e    </tr>.    <tr>
+000a5070: 0a20 2020 2020 203c 7468 3e31 3c2f 7468  .      <th>1</th
+000a5080: 3e0a 2020 2020 2020 3c74 643e 3230 3132  >.      <td>2012
+000a5090: 2d31 312d 3132 2032 333a 3234 3a35 353c  -11-12 23:24:55<
+000a50a0: 2f74 643e 0a20 2020 2020 203c 7464 3e31  /td>.      <td>1
+000a50b0: 3430 343c 2f74 643e 0a20 2020 2020 203c  404</td>.      <
+000a50c0: 7464 3e38 2e32 3c2f 7464 3e0a 2020 2020  td>8.2</td>.    
+000a50d0: 2020 3c74 643e 313c 2f74 643e 0a20 2020    <td>1</td>.   
+000a50e0: 2020 203c 7464 3e43 6c6f 7564 733c 2f74     <td>Clouds</t
+000a50f0: 643e 0a20 2020 2020 203c 7464 3e4d 6f6e  d>.      <td>Mon
+000a5100: 6461 793c 2f74 643e 0a20 2020 2020 203c  day</td>.      <
+000a5110: 7464 3e44 656c 6920 2f20 426f 6465 6761  td>Deli / Bodega
+000a5120: 3c2f 7464 3e0a 2020 2020 2020 3c74 643e  </td>.      <td>
+000a5130: 3430 2e38 3334 3039 383c 2f74 643e 0a20  40.834098</td>. 
+000a5140: 2020 2020 203c 7464 3e2d 3733 2e39 3435       <td>-73.945
+000a5150: 3236 373c 2f74 643e 0a20 2020 2020 203c  267</td>.      <
+000a5160: 7464 3e46 6f6f 643c 2f74 643e 0a20 2020  td>Food</td>.   
+000a5170: 2020 203c 7464 3e31 3236 3c2f 7464 3e0a     <td>126</td>.
+000a5180: 2020 2020 3c2f 7472 3e0a 2020 2020 3c74      </tr>.    <t
+000a5190: 723e 0a20 2020 2020 203c 7468 3e32 3c2f  r>.      <th>2</
+000a51a0: 7468 3e0a 2020 2020 2020 3c74 643e 3230  th>.      <td>20
+000a51b0: 3132 2d31 312d 3133 2030 303a 3030 3a30  12-11-13 00:00:0
+000a51c0: 373c 2f74 643e 0a20 2020 2020 203c 7464  7</td>.      <td
+000a51d0: 3e30 3c2f 7464 3e0a 2020 2020 2020 3c74  >0</td>.      <t
+000a51e0: 643e 2d31 2e30 3c2f 7464 3e0a 2020 2020  d>-1.0</td>.    
+000a51f0: 2020 3c74 643e 2d31 3c2f 7464 3e0a 2020    <td>-1</td>.  
+000a5200: 2020 2020 3c74 643e 436c 6f75 6473 3c2f      <td>Clouds</
+000a5210: 7464 3e0a 2020 2020 2020 3c74 643e 5475  td>.      <td>Tu
+000a5220: 6573 6461 793c 2f74 643e 0a20 2020 2020  esday</td>.     
+000a5230: 203c 7464 3e48 6f6d 6520 2870 7269 7661   <td>Home (priva
+000a5240: 7465 293c 2f74 643e 0a20 2020 2020 203c  te)</td>.      <
+000a5250: 7464 3e34 302e 3833 3331 3635 3c2f 7464  td>40.833165</td
+000a5260: 3e0a 2020 2020 2020 3c74 643e 2d37 332e  >.      <td>-73.
+000a5270: 3934 3138 3630 3c2f 7464 3e0a 2020 2020  941860</td>.    
+000a5280: 2020 3c74 643e 5265 7369 6465 6e63 653c    <td>Residence<
+000a5290: 2f74 643e 0a20 2020 2020 203c 7464 3e31  /td>.      <td>1
+000a52a0: 3236 3c2f 7464 3e0a 2020 2020 3c2f 7472  26</td>.    </tr
+000a52b0: 3e0a 2020 2020 3c74 723e 0a20 2020 2020  >.    <tr>.     
+000a52c0: 203c 7468 3e33 3c2f 7468 3e0a 2020 2020   <th>3</th>.    
+000a52d0: 2020 3c74 643e 3230 3132 2d31 312d 3135    <td>2012-11-15
+000a52e0: 2031 373a 3439 3a30 313c 2f74 643e 0a20   17:49:01</td>. 
+000a52f0: 2020 2020 203c 7464 3e31 3036 393c 2f74       <td>1069</t
+000a5300: 643e 0a20 2020 2020 203c 7464 3e36 2e36  d>.      <td>6.6
+000a5310: 3c2f 7464 3e0a 2020 2020 2020 3c74 643e  </td>.      <td>
+000a5320: 333c 2f74 643e 0a20 2020 2020 203c 7464  3</td>.      <td
+000a5330: 3e43 6c65 6172 3c2f 7464 3e0a 2020 2020  >Clear</td>.    
+000a5340: 2020 3c74 643e 5468 7572 7364 6179 3c2f    <td>Thursday</
+000a5350: 7464 3e0a 2020 2020 2020 3c74 643e 4672  td>.      <td>Fr
+000a5360: 6965 6420 4368 6963 6b65 6e20 4a6f 696e  ied Chicken Join
+000a5370: 743c 2f74 643e 0a20 2020 2020 203c 7464  t</td>.      <td
+000a5380: 3e34 302e 3736 3436 3936 3c2f 7464 3e0a  >40.764696</td>.
+000a5390: 2020 2020 2020 3c74 643e 2d37 332e 3838        <td>-73.88
+000a53a0: 3531 3937 3c2f 7464 3e0a 2020 2020 2020  5197</td>.      
+000a53b0: 3c74 643e 466f 6f64 3c2f 7464 3e0a 2020  <td>Food</td>.  
+000a53c0: 2020 2020 3c74 643e 3132 363c 2f74 643e      <td>126</td>
+000a53d0: 0a20 2020 203c 2f74 723e 0a20 2020 203c  .    </tr>.    <
+000a53e0: 7472 3e0a 2020 2020 2020 3c74 683e 343c  tr>.      <th>4<
+000a53f0: 2f74 683e 0a20 2020 2020 203c 7464 3e32  /th>.      <td>2
+000a5400: 3031 322d 3131 2d31 3520 3138 3a34 303a  012-11-15 18:40:
+000a5410: 3136 3c2f 7464 3e0a 2020 2020 2020 3c74  16</td>.      <t
+000a5420: 643e 3131 3230 3c2f 7464 3e0a 2020 2020  d>1120</td>.    
+000a5430: 2020 3c74 643e 2d31 2e30 3c2f 7464 3e0a    <td>-1.0</td>.
+000a5440: 2020 2020 2020 3c74 643e 2d31 3c2f 7464        <td>-1</td
+000a5450: 3e0a 2020 2020 2020 3c74 643e 436c 6561  >.      <td>Clea
+000a5460: 723c 2f74 643e 0a20 2020 2020 203c 7464  r</td>.      <td
+000a5470: 3e54 6875 7273 6461 793c 2f74 643e 0a20  >Thursday</td>. 
+000a5480: 2020 2020 203c 7464 3e42 7573 2053 7461       <td>Bus Sta
+000a5490: 7469 6f6e 3c2f 7464 3e0a 2020 2020 2020  tion</td>.      
+000a54a0: 3c74 643e 3430 2e37 3636 3037 393c 2f74  <td>40.766079</t
+000a54b0: 643e 0a20 2020 2020 203c 7464 3e2d 3733  d>.      <td>-73
+000a54c0: 2e38 3833 3532 393c 2f74 643e 0a20 2020  .883529</td>.   
+000a54d0: 2020 203c 7464 3e54 7261 7665 6c20 2661     <td>Travel &a
+000a54e0: 6d70 3b20 5472 616e 7370 6f72 743c 2f74  mp; Transport</t
+000a54f0: 643e 0a20 2020 2020 203c 7464 3e31 3236  d>.      <td>126
+000a5500: 3c2f 7464 3e0a 2020 2020 3c2f 7472 3e0a  </td>.    </tr>.
+000a5510: 2020 2020 3c74 723e 0a20 2020 2020 203c      <tr>.      <
+000a5520: 7468 3e2e 2e2e 3c2f 7468 3e0a 2020 2020  th>...</th>.    
+000a5530: 2020 3c74 643e 2e2e 2e3c 2f74 643e 0a20    <td>...</td>. 
+000a5540: 2020 2020 203c 7464 3e2e 2e2e 3c2f 7464       <td>...</td
+000a5550: 3e0a 2020 2020 2020 3c74 643e 2e2e 2e3c  >.      <td>...<
+000a5560: 2f74 643e 0a20 2020 2020 203c 7464 3e2e  /td>.      <td>.
+000a5570: 2e2e 3c2f 7464 3e0a 2020 2020 2020 3c74  ..</td>.      <t
+000a5580: 643e 2e2e 2e3c 2f74 643e 0a20 2020 2020  d>...</td>.     
+000a5590: 203c 7464 3e2e 2e2e 3c2f 7464 3e0a 2020   <td>...</td>.  
+000a55a0: 2020 2020 3c74 643e 2e2e 2e3c 2f74 643e      <td>...</td>
+000a55b0: 0a20 2020 2020 203c 7464 3e2e 2e2e 3c2f  .      <td>...</
+000a55c0: 7464 3e0a 2020 2020 2020 3c74 643e 2e2e  td>.      <td>..
+000a55d0: 2e3c 2f74 643e 0a20 2020 2020 203c 7464  .</td>.      <td
+000a55e0: 3e2e 2e2e 3c2f 7464 3e0a 2020 2020 2020  >...</td>.      
+000a55f0: 3c74 643e 2e2e 2e3c 2f74 643e 0a20 2020  <td>...</td>.   
+000a5600: 203c 2f74 723e 0a20 2020 203c 7472 3e0a   </tr>.    <tr>.
+000a5610: 2020 2020 2020 3c74 683e 3230 3038 303c        <th>20080<
+000a5620: 2f74 683e 0a20 2020 2020 203c 7464 3e32  /th>.      <td>2
+000a5630: 3031 322d 3038 2d31 3020 3137 3a31 373a  012-08-10 17:17:
+000a5640: 3337 3c2f 7464 3e0a 2020 2020 2020 3c74  37</td>.      <t
+000a5650: 643e 3130 3337 3c2f 7464 3e0a 2020 2020  d>1037</td>.    
+000a5660: 2020 3c74 643e 2d31 2e30 3c2f 7464 3e0a    <td>-1.0</td>.
+000a5670: 2020 2020 2020 3c74 643e 2d31 3c2f 7464        <td>-1</td
+000a5680: 3e0a 2020 2020 2020 3c74 643e 436c 6f75  >.      <td>Clou
+000a5690: 6473 3c2f 7464 3e0a 2020 2020 2020 3c74  ds</td>.      <t
+000a56a0: 643e 4672 6964 6179 3c2f 7464 3e0a 2020  d>Friday</td>.  
+000a56b0: 2020 2020 3c74 643e 4765 6e65 7261 6c20      <td>General 
+000a56c0: 436f 6c6c 6567 6520 2661 6d70 3b20 556e  College &amp; Un
+000a56d0: 6976 6572 7369 7479 3c2f 7464 3e0a 2020  iversity</td>.  
+000a56e0: 2020 2020 3c74 643e 3430 2e37 3034 3733      <td>40.70473
+000a56f0: 333c 2f74 643e 0a20 2020 2020 203c 7464  3</td>.      <td
+000a5700: 3e2d 3733 2e39 3837 3733 383c 2f74 643e  >-73.987738</td>
+000a5710: 0a20 2020 2020 203c 7464 3e43 6f6c 6c65  .      <td>Colle
+000a5720: 6765 2026 616d 703b 2055 6e69 7665 7273  ge &amp; Univers
+000a5730: 6974 793c 2f74 643e 0a20 2020 2020 203c  ity</td>.      <
+000a5740: 7464 3e32 3935 3633 3c2f 7464 3e0a 2020  td>29563</td>.  
+000a5750: 2020 3c2f 7472 3e0a 2020 2020 3c74 723e    </tr>.    <tr>
+000a5760: 0a20 2020 2020 203c 7468 3e32 3030 3831  .      <th>20081
+000a5770: 3c2f 7468 3e0a 2020 2020 2020 3c74 643e  </th>.      <td>
+000a5780: 3230 3132 2d30 382d 3130 2032 303a 3130  2012-08-10 20:10
+000a5790: 3a35 393c 2f74 643e 0a20 2020 2020 203c  :59</td>.      <
+000a57a0: 7464 3e31 3231 303c 2f74 643e 0a20 2020  td>1210</td>.   
+000a57b0: 2020 203c 7464 3e38 2e30 3c2f 7464 3e0a     <td>8.0</td>.
+000a57c0: 2020 2020 2020 3c74 643e 323c 2f74 643e        <td>2</td>
+000a57d0: 0a20 2020 2020 203c 7464 3e43 6c6f 7564  .      <td>Cloud
+000a57e0: 733c 2f74 643e 0a20 2020 2020 203c 7464  s</td>.      <td
+000a57f0: 3e46 7269 6461 793c 2f74 643e 0a20 2020  >Friday</td>.   
+000a5800: 2020 203c 7464 3e54 6861 6920 5265 7374     <td>Thai Rest
+000a5810: 6175 7261 6e74 3c2f 7464 3e0a 2020 2020  aurant</td>.    
+000a5820: 2020 3c74 643e 3430 2e36 3935 3136 333c    <td>40.695163<
+000a5830: 2f74 643e 0a20 2020 2020 203c 7464 3e2d  /td>.      <td>-
+000a5840: 3733 2e39 3935 3434 383c 2f74 643e 0a20  73.995448</td>. 
+000a5850: 2020 2020 203c 7464 3e46 6f6f 643c 2f74       <td>Food</t
+000a5860: 643e 0a20 2020 2020 203c 7464 3e32 3935  d>.      <td>295
+000a5870: 3633 3c2f 7464 3e0a 2020 2020 3c2f 7472  63</td>.    </tr
+000a5880: 3e0a 2020 2020 3c74 723e 0a20 2020 2020  >.    <tr>.     
+000a5890: 203c 7468 3e32 3030 3832 3c2f 7468 3e0a   <th>20082</th>.
+000a58a0: 2020 2020 2020 3c74 643e 3230 3132 2d30        <td>2012-0
+000a58b0: 382d 3131 2030 383a 3031 3a32 303c 2f74  8-11 08:01:20</t
+000a58c0: 643e 0a20 2020 2020 203c 7464 3e34 3831  d>.      <td>481
+000a58d0: 3c2f 7464 3e0a 2020 2020 2020 3c74 643e  </td>.      <td>
+000a58e0: 362e 393c 2f74 643e 0a20 2020 2020 203c  6.9</td>.      <
+000a58f0: 7464 3e2d 313c 2f74 643e 0a20 2020 2020  td>-1</td>.     
+000a5900: 203c 7464 3e43 6c6f 7564 733c 2f74 643e   <td>Clouds</td>
+000a5910: 0a20 2020 2020 203c 7464 3e53 6174 7572  .      <td>Satur
+000a5920: 6461 793c 2f74 643e 0a20 2020 2020 203c  day</td>.      <
+000a5930: 7464 3e47 796d 3c2f 7464 3e0a 2020 2020  td>Gym</td>.    
+000a5940: 2020 3c74 643e 3430 2e36 3937 3830 333c    <td>40.697803<
+000a5950: 2f74 643e 0a20 2020 2020 203c 7464 3e2d  /td>.      <td>-
+000a5960: 3733 2e39 3934 3134 353c 2f74 643e 0a20  73.994145</td>. 
+000a5970: 2020 2020 203c 7464 3e4f 7574 646f 6f72       <td>Outdoor
+000a5980: 7320 2661 6d70 3b20 5265 6372 6561 7469  s &amp; Recreati
+000a5990: 6f6e 3c2f 7464 3e0a 2020 2020 2020 3c74  on</td>.      <t
+000a59a0: 643e 3239 3536 333c 2f74 643e 0a20 2020  d>29563</td>.   
+000a59b0: 203c 2f74 723e 0a20 2020 203c 7472 3e0a   </tr>.    <tr>.
+000a59c0: 2020 2020 2020 3c74 683e 3230 3038 333c        <th>20083<
+000a59d0: 2f74 683e 0a20 2020 2020 203c 7464 3e32  /th>.      <td>2
+000a59e0: 3031 322d 3038 2d31 3120 3133 3a33 393a  012-08-11 13:39:
+000a59f0: 3339 3c2f 7464 3e0a 2020 2020 2020 3c74  39</td>.      <t
+000a5a00: 643e 3831 393c 2f74 643e 0a20 2020 2020  d>819</td>.     
+000a5a10: 203c 7464 3e37 2e30 3c2f 7464 3e0a 2020   <td>7.0</td>.  
+000a5a20: 2020 2020 3c74 643e 313c 2f74 643e 0a20      <td>1</td>. 
+000a5a30: 2020 2020 203c 7464 3e43 6c6f 7564 733c       <td>Clouds<
+000a5a40: 2f74 643e 0a20 2020 2020 203c 7464 3e53  /td>.      <td>S
+000a5a50: 6174 7572 6461 793c 2f74 643e 0a20 2020  aturday</td>.   
+000a5a60: 2020 203c 7464 3e43 6f66 6665 6520 5368     <td>Coffee Sh
+000a5a70: 6f70 3c2f 7464 3e0a 2020 2020 2020 3c74  op</td>.      <t
+000a5a80: 643e 3430 2e36 3934 3637 333c 2f74 643e  d>40.694673</td>
+000a5a90: 0a20 2020 2020 203c 7464 3e2d 3733 2e39  .      <td>-73.9
+000a5aa0: 3934 3038 323c 2f74 643e 0a20 2020 2020  94082</td>.     
+000a5ab0: 203c 7464 3e46 6f6f 643c 2f74 643e 0a20   <td>Food</td>. 
+000a5ac0: 2020 2020 203c 7464 3e32 3935 3633 3c2f       <td>29563</
+000a5ad0: 7464 3e0a 2020 2020 3c2f 7472 3e0a 2020  td>.    </tr>.  
+000a5ae0: 2020 3c74 723e 0a20 2020 2020 203c 7468    <tr>.      <th
+000a5af0: 3e32 3030 3834 3c2f 7468 3e0a 2020 2020  >20084</th>.    
+000a5b00: 2020 3c74 643e 3230 3132 2d30 382d 3132    <td>2012-08-12
+000a5b10: 2030 373a 3536 3a32 363c 2f74 643e 0a20   07:56:26</td>. 
+000a5b20: 2020 2020 203c 7464 3e34 3736 3c2f 7464       <td>476</td
+000a5b30: 3e0a 2020 2020 2020 3c74 643e 362e 393c  >.      <td>6.9<
+000a5b40: 2f74 643e 0a20 2020 2020 203c 7464 3e2d  /td>.      <td>-
+000a5b50: 313c 2f74 643e 0a20 2020 2020 203c 7464  1</td>.      <td
+000a5b60: 3e43 6c6f 7564 733c 2f74 643e 0a20 2020  >Clouds</td>.   
+000a5b70: 2020 203c 7464 3e53 756e 6461 793c 2f74     <td>Sunday</t
+000a5b80: 643e 0a20 2020 2020 203c 7464 3e47 796d  d>.      <td>Gym
+000a5b90: 3c2f 7464 3e0a 2020 2020 2020 3c74 643e  </td>.      <td>
+000a5ba0: 3430 2e36 3937 3830 333c 2f74 643e 0a20  40.697803</td>. 
+000a5bb0: 2020 2020 203c 7464 3e2d 3733 2e39 3934       <td>-73.994
+000a5bc0: 3134 353c 2f74 643e 0a20 2020 2020 203c  145</td>.      <
+000a5bd0: 7464 3e4f 7574 646f 6f72 7320 2661 6d70  td>Outdoors &amp
+000a5be0: 3b20 5265 6372 6561 7469 6f6e 3c2f 7464  ; Recreation</td
+000a5bf0: 3e0a 2020 2020 2020 3c74 643e 3239 3536  >.      <td>2956
+000a5c00: 333c 2f74 643e 0a20 2020 203c 2f74 723e  3</td>.    </tr>
+000a5c10: 0a20 203c 2f74 626f 6479 3e0a 3c2f 7461  .  </tbody>.</ta
+000a5c20: 626c 653e 0a3c 703e 3636 3936 3220 726f  ble>.<p>66962 ro
+000a5c30: 7773 20c3 9720 3131 2063 6f6c 756d 6e73  ws .. 11 columns
+000a5c40: 3c2f 703e 0a3c 2f64 6976 3e0a 3c2f 6469  </p>.</div>.</di
+000a5c50: 763e 0a0a 3c2f 6469 763e 0a0a 3c2f 6469  v>..</div>..</di
+000a5c60: 763e 0a0a 3c2f 6469 763e 0a0a 3c2f 6469  v>..</div>..</di
+000a5c70: 763e 0a3c 6469 7620 636c 6173 733d 226a  v>.<div class="j
+000a5c80: 702d 4365 6c6c 206a 702d 4d61 726b 646f  p-Cell jp-Markdo
+000a5c90: 776e 4365 6c6c 206a 702d 4e6f 7465 626f  wnCell jp-Notebo
+000a5ca0: 6f6b 2d63 656c 6c22 3e0a 3c64 6976 2063  ok-cell">.<div c
+000a5cb0: 6c61 7373 3d22 6a70 2d43 656c 6c2d 696e  lass="jp-Cell-in
+000a5cc0: 7075 7457 7261 7070 6572 223e 0a3c 6469  putWrapper">.<di
+000a5cd0: 7620 636c 6173 733d 226a 702d 436f 6c6c  v class="jp-Coll
+000a5ce0: 6170 7365 7220 6a70 2d49 6e70 7574 436f  apser jp-InputCo
+000a5cf0: 6c6c 6170 7365 7220 6a70 2d43 656c 6c2d  llapser jp-Cell-
+000a5d00: 696e 7075 7443 6f6c 6c61 7073 6572 223e  inputCollapser">
+000a5d10: 0a3c 2f64 6976 3e0a 3c64 6976 2063 6c61  .</div>.<div cla
+000a5d20: 7373 3d22 6a70 2d49 6e70 7574 4172 6561  ss="jp-InputArea
+000a5d30: 206a 702d 4365 6c6c 2d69 6e70 7574 4172   jp-Cell-inputAr
+000a5d40: 6561 223e 3c64 6976 2063 6c61 7373 3d22  ea"><div class="
+000a5d50: 6a70 2d49 6e70 7574 5072 6f6d 7074 206a  jp-InputPrompt j
+000a5d60: 702d 496e 7075 7441 7265 612d 7072 6f6d  p-InputArea-prom
+000a5d70: 7074 223e 0a3c 2f64 6976 3e3c 6469 7620  pt">.</div><div 
+000a5d80: 636c 6173 733d 226a 702d 5265 6e64 6572  class="jp-Render
+000a5d90: 6564 4854 4d4c 436f 6d6d 6f6e 206a 702d  edHTMLCommon jp-
+000a5da0: 5265 6e64 6572 6564 4d61 726b 646f 776e  RenderedMarkdown
+000a5db0: 206a 702d 4d61 726b 646f 776e 4f75 7470   jp-MarkdownOutp
+000a5dc0: 7574 2022 2064 6174 612d 6d69 6d65 2d74  ut " data-mime-t
+000a5dd0: 7970 653d 2274 6578 742f 6d61 726b 646f  ype="text/markdo
+000a5de0: 776e 223e 0a3c 6833 2069 643d 2234 2e2d  wn">.<h3 id="4.-
+000a5df0: 5379 6e74 6865 7469 632d 4461 7461 2d47  Synthetic-Data-G
+000a5e00: 656e 6572 6174 696f 6e22 3e34 2e20 5379  eneration">4. Sy
+000a5e10: 6e74 6865 7469 6320 4461 7461 2047 656e  nthetic Data Gen
+000a5e20: 6572 6174 696f 6e3c 6120 636c 6173 733d  eration<a class=
+000a5e30: 2261 6e63 686f 722d 6c69 6e6b 2220 6872  "anchor-link" hr
+000a5e40: 6566 3d22 2334 2e2d 5379 6e74 6865 7469  ef="#4.-Syntheti
+000a5e50: 632d 4461 7461 2d47 656e 6572 6174 696f  c-Data-Generatio
+000a5e60: 6e22 3e26 2331 3832 3b3c 2f61 3e3c 2f68  n">&#182;</a></h
+000a5e70: 333e 3c70 3e54 4f44 4f3c 2f70 3e0a 0a3c  3><p>TODO</p>..<
+000a5e80: 2f64 6976 3e0a 3c2f 6469 763e 0a3c 2f64  /div>.</div>.</d
+000a5e90: 6976 3e0a 3c2f 6469 763e 3c64 6976 2063  iv>.</div><div c
+000a5ea0: 6c61 7373 3d22 6a70 2d43 656c 6c20 6a70  lass="jp-Cell jp
+000a5eb0: 2d43 6f64 6543 656c 6c20 6a70 2d4e 6f74  -CodeCell jp-Not
+000a5ec0: 6562 6f6f 6b2d 6365 6c6c 206a 702d 6d6f  ebook-cell jp-mo
+000a5ed0: 642d 6e6f 4f75 7470 7574 7320 2022 3e0a  d-noOutputs  ">.
+000a5ee0: 3c64 6976 2063 6c61 7373 3d22 6a70 2d43  <div class="jp-C
+000a5ef0: 656c 6c2d 696e 7075 7457 7261 7070 6572  ell-inputWrapper
+000a5f00: 223e 0a3c 6469 7620 636c 6173 733d 226a  ">.<div class="j
+000a5f10: 702d 436f 6c6c 6170 7365 7220 6a70 2d49  p-Collapser jp-I
+000a5f20: 6e70 7574 436f 6c6c 6170 7365 7220 6a70  nputCollapser jp
+000a5f30: 2d43 656c 6c2d 696e 7075 7443 6f6c 6c61  -Cell-inputColla
+000a5f40: 7073 6572 223e 0a3c 2f64 6976 3e0a 3c64  pser">.</div>.<d
+000a5f50: 6976 2063 6c61 7373 3d22 6a70 2d49 6e70  iv class="jp-Inp
+000a5f60: 7574 4172 6561 206a 702d 4365 6c6c 2d69  utArea jp-Cell-i
+000a5f70: 6e70 7574 4172 6561 223e 0a3c 6469 7620  nputArea">.<div 
+000a5f80: 636c 6173 733d 226a 702d 496e 7075 7450  class="jp-InputP
+000a5f90: 726f 6d70 7420 6a70 2d49 6e70 7574 4172  rompt jp-InputAr
+000a5fa0: 6561 2d70 726f 6d70 7422 3e49 6e26 6e62  ea-prompt">In&nb
+000a5fb0: 7370 3b5b 315d 3a3c 2f64 6976 3e0a 3c64  sp;[1]:</div>.<d
+000a5fc0: 6976 2063 6c61 7373 3d22 6a70 2d43 6f64  iv class="jp-Cod
+000a5fd0: 654d 6972 726f 7245 6469 746f 7220 6a70  eMirrorEditor jp
+000a5fe0: 2d45 6469 746f 7220 6a70 2d49 6e70 7574  -Editor jp-Input
+000a5ff0: 4172 6561 2d65 6469 746f 7222 2064 6174  Area-editor" dat
+000a6000: 612d 7479 7065 3d22 696e 6c69 6e65 223e  a-type="inline">
+000a6010: 0a20 2020 2020 3c64 6976 2063 6c61 7373  .     <div class
+000a6020: 3d22 436f 6465 4d69 7272 6f72 2063 6d2d  ="CodeMirror cm-
+000a6030: 732d 6a75 7079 7465 7222 3e0a 3c64 6976  s-jupyter">.<div
+000a6040: 2063 6c61 7373 3d22 2068 6967 686c 6967   class=" highlig
+000a6050: 6874 2068 6c2d 6970 7974 686f 6e33 223e  ht hl-ipython3">
+000a6060: 3c70 7265 3e3c 7370 616e 3e3c 2f73 7061  <pre><span></spa
+000a6070: 6e3e 3c73 7061 6e20 636c 6173 733d 226b  n><span class="k
+000a6080: 6e22 3e66 726f 6d3c 2f73 7061 6e3e 203c  n">from</span> <
+000a6090: 7370 616e 2063 6c61 7373 3d22 6e6e 223e  span class="nn">
+000a60a0: 6d61 7464 6174 612e 6765 6e65 7261 746f  matdata.generato
+000a60b0: 723c 2f73 7061 6e3e 203c 7370 616e 2063  r</span> <span c
+000a60c0: 6c61 7373 3d22 6b6e 223e 696d 706f 7274  lass="kn">import
+000a60d0: 3c2f 7370 616e 3e20 3c73 7061 6e20 636c  </span> <span cl
+000a60e0: 6173 733d 226f 223e 2a3c 2f73 7061 6e3e  ass="o">*</span>
+000a60f0: 0a3c 2f70 7265 3e3c 2f64 6976 3e0a 0a20  .</pre></div>.. 
+000a6100: 2020 2020 3c2f 6469 763e 0a3c 2f64 6976      </div>.</div
+000a6110: 3e0a 3c2f 6469 763e 0a3c 2f64 6976 3e0a  >.</div>.</div>.
+000a6120: 0a3c 2f64 6976 3e0a 3c64 6976 2063 6c61  .</div>.<div cla
+000a6130: 7373 3d22 6a70 2d43 656c 6c20 6a70 2d4d  ss="jp-Cell jp-M
+000a6140: 6172 6b64 6f77 6e43 656c 6c20 6a70 2d4e  arkdownCell jp-N
+000a6150: 6f74 6562 6f6f 6b2d 6365 6c6c 223e 0a3c  otebook-cell">.<
+000a6160: 6469 7620 636c 6173 733d 226a 702d 4365  div class="jp-Ce
+000a6170: 6c6c 2d69 6e70 7574 5772 6170 7065 7222  ll-inputWrapper"
+000a6180: 3e0a 3c64 6976 2063 6c61 7373 3d22 6a70  >.<div class="jp
+000a6190: 2d43 6f6c 6c61 7073 6572 206a 702d 496e  -Collapser jp-In
+000a61a0: 7075 7443 6f6c 6c61 7073 6572 206a 702d  putCollapser jp-
+000a61b0: 4365 6c6c 2d69 6e70 7574 436f 6c6c 6170  Cell-inputCollap
+000a61c0: 7365 7222 3e0a 3c2f 6469 763e 0a3c 6469  ser">.</div>.<di
+000a61d0: 7620 636c 6173 733d 226a 702d 496e 7075  v class="jp-Inpu
+000a61e0: 7441 7265 6120 6a70 2d43 656c 6c2d 696e  tArea jp-Cell-in
+000a61f0: 7075 7441 7265 6122 3e3c 6469 7620 636c  putArea"><div cl
+000a6200: 6173 733d 226a 702d 496e 7075 7450 726f  ass="jp-InputPro
+000a6210: 6d70 7420 6a70 2d49 6e70 7574 4172 6561  mpt jp-InputArea
+000a6220: 2d70 726f 6d70 7422 3e0a 3c2f 6469 763e  -prompt">.</div>
+000a6230: 3c64 6976 2063 6c61 7373 3d22 6a70 2d52  <div class="jp-R
+000a6240: 656e 6465 7265 6448 544d 4c43 6f6d 6d6f  enderedHTMLCommo
+000a6250: 6e20 6a70 2d52 656e 6465 7265 644d 6172  n jp-RenderedMar
+000a6260: 6b64 6f77 6e20 6a70 2d4d 6172 6b64 6f77  kdown jp-Markdow
+000a6270: 6e4f 7574 7075 7420 2220 6461 7461 2d6d  nOutput " data-m
+000a6280: 696d 652d 7479 7065 3d22 7465 7874 2f6d  ime-type="text/m
+000a6290: 6172 6b64 6f77 6e22 3e0a 3c75 6c3e 0a3c  arkdown">.<ul>.<
+000a62a0: 6c69 3e3c 636f 6465 3e73 6361 6c65 7253  li><code>scalerS
+000a62b0: 616d 706c 6572 4765 6e65 7261 746f 723c  amplerGenerator<
+000a62c0: 2f63 6f64 653e 3a20 6765 6e65 7261 7465  /code>: generate
+000a62d0: 7320 7472 616a 6563 746f 7279 2064 6174  s trajectory dat
+000a62e0: 6173 6574 7320 6261 7365 6420 6f6e 2072  asets based on r
+000a62f0: 6561 6c20 6461 7461 206f 6e20 7363 616c  eal data on scal
+000a6300: 6520 696e 7465 7276 616c 733c 2f6c 693e  e intervals</li>
+000a6310: 0a3c 6c69 3e3c 636f 6465 3e73 616d 706c  .<li><code>sampl
+000a6320: 6572 4765 6e65 7261 746f 723c 2f63 6f64  erGenerator</cod
+000a6330: 653e 3a20 6765 6e65 7261 7465 2061 2074  e>: generate a t
+000a6340: 7261 6a65 6374 6f72 7920 6461 7461 7365  rajectory datase
+000a6350: 7420 6261 7365 6420 6f6e 2072 6561 6c20  t based on real 
+000a6360: 6461 7461 3c2f 6c69 3e0a 3c6c 693e 3c63  data</li>.<li><c
+000a6370: 6f64 653e 7363 616c 6572 5261 6e64 6f6d  ode>scalerRandom
+000a6380: 4765 6e65 7261 746f 723c 2f63 6f64 653e  Generator</code>
+000a6390: 3a20 6765 6e65 7261 7465 7320 7472 616a  : generates traj
+000a63a0: 6563 746f 7279 2064 6174 6173 6574 7320  ectory datasets 
+000a63b0: 6261 7365 6420 6f6e 2072 616e 646f 6d20  based on random 
+000a63c0: 6461 7461 206f 6e20 7363 616c 6520 696e  data on scale in
+000a63d0: 7465 7276 616c 733c 2f6c 693e 0a3c 6c69  tervals</li>.<li
+000a63e0: 3e3c 636f 6465 3e72 616e 646f 6d47 656e  ><code>randomGen
+000a63f0: 6572 6174 6f72 3c2f 636f 6465 3e3a 2067  erator</code>: g
+000a6400: 656e 6572 6174 6520 6120 7472 616a 6563  enerate a trajec
+000a6410: 746f 7279 2064 6174 6173 6574 2062 6173  tory dataset bas
+000a6420: 6564 206f 6e20 7261 6e64 6f6d 2064 6174  ed on random dat
+000a6430: 613c 2f6c 693e 0a3c 2f75 6c3e 0a0a 3c2f  a</li>.</ul>..</
+000a6440: 6469 763e 0a3c 2f64 6976 3e0a 3c2f 6469  div>.</div>.</di
+000a6450: 763e 0a3c 2f64 6976 3e0a 3c64 6976 2063  v>.</div>.<div c
+000a6460: 6c61 7373 3d22 6a70 2d43 656c 6c20 6a70  lass="jp-Cell jp
+000a6470: 2d4d 6172 6b64 6f77 6e43 656c 6c20 6a70  -MarkdownCell jp
+000a6480: 2d4e 6f74 6562 6f6f 6b2d 6365 6c6c 223e  -Notebook-cell">
+000a6490: 0a3c 6469 7620 636c 6173 733d 226a 702d  .<div class="jp-
+000a64a0: 4365 6c6c 2d69 6e70 7574 5772 6170 7065  Cell-inputWrappe
+000a64b0: 7222 3e0a 3c64 6976 2063 6c61 7373 3d22  r">.<div class="
+000a64c0: 6a70 2d43 6f6c 6c61 7073 6572 206a 702d  jp-Collapser jp-
+000a64d0: 496e 7075 7443 6f6c 6c61 7073 6572 206a  InputCollapser j
+000a64e0: 702d 4365 6c6c 2d69 6e70 7574 436f 6c6c  p-Cell-inputColl
+000a64f0: 6170 7365 7222 3e0a 3c2f 6469 763e 0a3c  apser">.</div>.<
+000a6500: 6469 7620 636c 6173 733d 226a 702d 496e  div class="jp-In
+000a6510: 7075 7441 7265 6120 6a70 2d43 656c 6c2d  putArea jp-Cell-
+000a6520: 696e 7075 7441 7265 6122 3e3c 6469 7620  inputArea"><div 
+000a6530: 636c 6173 733d 226a 702d 496e 7075 7450  class="jp-InputP
+000a6540: 726f 6d70 7420 6a70 2d49 6e70 7574 4172  rompt jp-InputAr
+000a6550: 6561 2d70 726f 6d70 7422 3e0a 3c2f 6469  ea-prompt">.</di
+000a6560: 763e 3c64 6976 2063 6c61 7373 3d22 6a70  v><div class="jp
+000a6570: 2d52 656e 6465 7265 6448 544d 4c43 6f6d  -RenderedHTMLCom
+000a6580: 6d6f 6e20 6a70 2d52 656e 6465 7265 644d  mon jp-RenderedM
+000a6590: 6172 6b64 6f77 6e20 6a70 2d4d 6172 6b64  arkdown jp-Markd
+000a65a0: 6f77 6e4f 7574 7075 7420 2220 6461 7461  ownOutput " data
+000a65b0: 2d6d 696d 652d 7479 7065 3d22 7465 7874  -mime-type="text
+000a65c0: 2f6d 6172 6b64 6f77 6e22 3e0a 0a3c 7072  /markdown">..<pr
+000a65d0: 653e 3c63 6f64 653e 6129 2054 6f20 6765  e><code>a) To ge
+000a65e0: 6e65 7261 7465 2061 2073 616d 706c 6520  nerate a sample 
+000a65f0: 6461 7461 7365 7420 2864 6566 6175 6c74  dataset (default
+000a6600: 2063 6f6e 6669 6729 3a3c 2f63 6f64 653e   config):</code>
+000a6610: 3c2f 7072 653e 0a0a 3c2f 6469 763e 0a3c  </pre>..</div>.<
+000a6620: 2f64 6976 3e0a 3c2f 6469 763e 0a3c 2f64  /div>.</div>.</d
+000a6630: 6976 3e3c 6469 7620 636c 6173 733d 226a  iv><div class="j
+000a6640: 702d 4365 6c6c 206a 702d 436f 6465 4365  p-Cell jp-CodeCe
+000a6650: 6c6c 206a 702d 4e6f 7465 626f 6f6b 2d63  ll jp-Notebook-c
+000a6660: 656c 6c20 2020 223e 0a3c 6469 7620 636c  ell   ">.<div cl
+000a6670: 6173 733d 226a 702d 4365 6c6c 2d69 6e70  ass="jp-Cell-inp
+000a6680: 7574 5772 6170 7065 7222 3e0a 3c64 6976  utWrapper">.<div
+000a6690: 2063 6c61 7373 3d22 6a70 2d43 6f6c 6c61   class="jp-Colla
+000a66a0: 7073 6572 206a 702d 496e 7075 7443 6f6c  pser jp-InputCol
+000a66b0: 6c61 7073 6572 206a 702d 4365 6c6c 2d69  lapser jp-Cell-i
+000a66c0: 6e70 7574 436f 6c6c 6170 7365 7222 3e0a  nputCollapser">.
+000a66d0: 3c2f 6469 763e 0a3c 6469 7620 636c 6173  </div>.<div clas
+000a66e0: 733d 226a 702d 496e 7075 7441 7265 6120  s="jp-InputArea 
+000a66f0: 6a70 2d43 656c 6c2d 696e 7075 7441 7265  jp-Cell-inputAre
+000a6700: 6122 3e0a 3c64 6976 2063 6c61 7373 3d22  a">.<div class="
+000a6710: 6a70 2d49 6e70 7574 5072 6f6d 7074 206a  jp-InputPrompt j
+000a6720: 702d 496e 7075 7441 7265 612d 7072 6f6d  p-InputArea-prom
+000a6730: 7074 223e 496e 266e 6273 703b 5b32 5d3a  pt">In&nbsp;[2]:
+000a6740: 3c2f 6469 763e 0a3c 6469 7620 636c 6173  </div>.<div clas
+000a6750: 733d 226a 702d 436f 6465 4d69 7272 6f72  s="jp-CodeMirror
+000a6760: 4564 6974 6f72 206a 702d 4564 6974 6f72  Editor jp-Editor
+000a6770: 206a 702d 496e 7075 7441 7265 612d 6564   jp-InputArea-ed
+000a6780: 6974 6f72 2220 6461 7461 2d74 7970 653d  itor" data-type=
+000a6790: 2269 6e6c 696e 6522 3e0a 2020 2020 203c  "inline">.     <
+000a67a0: 6469 7620 636c 6173 733d 2243 6f64 654d  div class="CodeM
+000a67b0: 6972 726f 7220 636d 2d73 2d6a 7570 7974  irror cm-s-jupyt
+000a67c0: 6572 223e 0a3c 6469 7620 636c 6173 733d  er">.<div class=
+000a67d0: 2220 6869 6768 6c69 6768 7420 686c 2d69  " highlight hl-i
+000a67e0: 7079 7468 6f6e 3322 3e3c 7072 653e 3c73  python3"><pre><s
+000a67f0: 7061 6e3e 3c2f 7370 616e 3e3c 7370 616e  pan></span><span
+000a6800: 2063 6c61 7373 3d22 6e22 3e73 616d 706c   class="n">sampl
+000a6810: 6572 4765 6e65 7261 746f 723c 2f73 7061  erGenerator</spa
+000a6820: 6e3e 3c73 7061 6e20 636c 6173 733d 2270  n><span class="p
+000a6830: 223e 2829 3c2f 7370 616e 3e0a 3c2f 7072  ">()</span>.</pr
+000a6840: 653e 3c2f 6469 763e 0a0a 2020 2020 203c  e></div>..     <
+000a6850: 2f64 6976 3e0a 3c2f 6469 763e 0a3c 2f64  /div>.</div>.</d
+000a6860: 6976 3e0a 3c2f 6469 763e 0a0a 3c64 6976  iv>.</div>..<div
+000a6870: 2063 6c61 7373 3d22 6a70 2d43 656c 6c2d   class="jp-Cell-
+000a6880: 6f75 7470 7574 5772 6170 7065 7222 3e0a  outputWrapper">.
+000a6890: 3c64 6976 2063 6c61 7373 3d22 6a70 2d43  <div class="jp-C
+000a68a0: 6f6c 6c61 7073 6572 206a 702d 4f75 7470  ollapser jp-Outp
+000a68b0: 7574 436f 6c6c 6170 7365 7220 6a70 2d43  utCollapser jp-C
+000a68c0: 656c 6c2d 6f75 7470 7574 436f 6c6c 6170  ell-outputCollap
+000a68d0: 7365 7222 3e0a 3c2f 6469 763e 0a0a 0a3c  ser">.</div>...<
+000a68e0: 6469 7620 636c 6173 733d 226a 702d 4f75  div class="jp-Ou
+000a68f0: 7470 7574 4172 6561 206a 702d 4365 6c6c  tputArea jp-Cell
+000a6900: 2d6f 7574 7075 7441 7265 6122 3e0a 0a3c  -outputArea">..<
+000a6910: 6469 7620 636c 6173 733d 226a 702d 4f75  div class="jp-Ou
+000a6920: 7470 7574 4172 6561 2d63 6869 6c64 223e  tputArea-child">
+000a6930: 0a0a 2020 2020 0a20 2020 203c 6469 7620  ..    .    <div 
+000a6940: 636c 6173 733d 226a 702d 4f75 7470 7574  class="jp-Output
+000a6950: 5072 6f6d 7074 206a 702d 4f75 7470 7574  Prompt jp-Output
+000a6960: 4172 6561 2d70 726f 6d70 7422 3e4f 7574  Area-prompt">Out
+000a6970: 5b32 5d3a 3c2f 6469 763e 0a0a 0a0a 3c64  [2]:</div>....<d
+000a6980: 6976 2063 6c61 7373 3d22 6a70 2d52 656e  iv class="jp-Ren
+000a6990: 6465 7265 6448 544d 4c43 6f6d 6d6f 6e20  deredHTMLCommon 
+000a69a0: 6a70 2d52 656e 6465 7265 6448 544d 4c20  jp-RenderedHTML 
+000a69b0: 6a70 2d4f 7574 7075 7441 7265 612d 6f75  jp-OutputArea-ou
+000a69c0: 7470 7574 206a 702d 4f75 7470 7574 4172  tput jp-OutputAr
+000a69d0: 6561 2d65 7865 6375 7465 5265 7375 6c74  ea-executeResult
+000a69e0: 2220 6461 7461 2d6d 696d 652d 7479 7065  " data-mime-type
+000a69f0: 3d22 7465 7874 2f68 746d 6c22 3e0a 3c64  ="text/html">.<d
+000a6a00: 6976 3e0a 3c73 7479 6c65 2073 636f 7065  iv>.<style scope
+000a6a10: 643e 0a20 2020 202e 6461 7461 6672 616d  d>.    .datafram
+000a6a20: 6520 7462 6f64 7920 7472 2074 683a 6f6e  e tbody tr th:on
+000a6a30: 6c79 2d6f 662d 7479 7065 207b 0a20 2020  ly-of-type {.   
+000a6a40: 2020 2020 2076 6572 7469 6361 6c2d 616c       vertical-al
+000a6a50: 6967 6e3a 206d 6964 646c 653b 0a20 2020  ign: middle;.   
+000a6a60: 207d 0a0a 2020 2020 2e64 6174 6166 7261   }..    .datafra
+000a6a70: 6d65 2074 626f 6479 2074 7220 7468 207b  me tbody tr th {
+000a6a80: 0a20 2020 2020 2020 2076 6572 7469 6361  .        vertica
+000a6a90: 6c2d 616c 6967 6e3a 2074 6f70 3b0a 2020  l-align: top;.  
+000a6aa0: 2020 7d0a 0a20 2020 202e 6461 7461 6672    }..    .datafr
+000a6ab0: 616d 6520 7468 6561 6420 7468 207b 0a20  ame thead th {. 
+000a6ac0: 2020 2020 2020 2074 6578 742d 616c 6967         text-alig
+000a6ad0: 6e3a 2072 6967 6874 3b0a 2020 2020 7d0a  n: right;.    }.
+000a6ae0: 3c2f 7374 796c 653e 0a3c 7461 626c 6520  </style>.<table 
+000a6af0: 626f 7264 6572 3d22 3122 2063 6c61 7373  border="1" class
+000a6b00: 3d22 6461 7461 6672 616d 6522 3e0a 2020  ="dataframe">.  
+000a6b10: 3c74 6865 6164 3e0a 2020 2020 3c74 7220  <thead>.    <tr 
+000a6b20: 7374 796c 653d 2274 6578 742d 616c 6967  style="text-alig
+000a6b30: 6e3a 2072 6967 6874 3b22 3e0a 2020 2020  n: right;">.    
+000a6b40: 2020 3c74 683e 3c2f 7468 3e0a 2020 2020    <th></th>.    
+000a6b50: 2020 3c74 683e 7469 643c 2f74 683e 0a20    <th>tid</th>. 
+000a6b60: 2020 2020 203c 7468 3e73 7061 6365 3c2f       <th>space</
+000a6b70: 7468 3e0a 2020 2020 2020 3c74 683e 7469  th>.      <th>ti
+000a6b80: 6d65 3c2f 7468 3e0a 2020 2020 2020 3c74  me</th>.      <t
+000a6b90: 683e 6461 793c 2f74 683e 0a20 2020 2020  h>day</th>.     
+000a6ba0: 203c 7468 3e72 6174 696e 673c 2f74 683e   <th>rating</th>
+000a6bb0: 0a20 2020 2020 203c 7468 3e70 7269 6365  .      <th>price
+000a6bc0: 3c2f 7468 3e0a 2020 2020 2020 3c74 683e  </th>.      <th>
+000a6bd0: 7765 6174 6865 723c 2f74 683e 0a20 2020  weather</th>.   
+000a6be0: 2020 203c 7468 3e72 6f6f 745f 7479 7065     <th>root_type
+000a6bf0: 3c2f 7468 3e0a 2020 2020 2020 3c74 683e  </th>.      <th>
+000a6c00: 7479 7065 3c2f 7468 3e0a 2020 2020 2020  type</th>.      
+000a6c10: 3c74 683e 6c61 6265 6c3c 2f74 683e 0a20  <th>label</th>. 
+000a6c20: 2020 203c 2f74 723e 0a20 203c 2f74 6865     </tr>.  </the
+000a6c30: 6164 3e0a 2020 3c74 626f 6479 3e0a 2020  ad>.  <tbody>.  
+000a6c40: 2020 3c74 723e 0a20 2020 2020 203c 7468    <tr>.      <th
+000a6c50: 3e30 3c2f 7468 3e0a 2020 2020 2020 3c74  >0</th>.      <t
+000a6c60: 643e 313c 2f74 643e 0a20 2020 2020 203c  d>1</td>.      <
+000a6c70: 7464 3e34 302e 3734 3239 3639 3233 3832  td>40.7429692382
+000a6c80: 3238 3620 2d37 332e 3838 3237 3636 3936  286 -73.88276696
+000a6c90: 3230 3531 343c 2f74 643e 0a20 2020 2020  20514</td>.     
+000a6ca0: 203c 7464 3e34 3437 3c2f 7464 3e0a 2020   <td>447</td>.  
+000a6cb0: 2020 2020 3c74 643e 4d6f 6e64 6179 3c2f      <td>Monday</
+000a6cc0: 7464 3e0a 2020 2020 2020 3c74 643e 362e  td>.      <td>6.
+000a6cd0: 313c 2f74 643e 0a20 2020 2020 203c 7464  1</td>.      <td
+000a6ce0: 3e2d 313c 2f74 643e 0a20 2020 2020 203c  >-1</td>.      <
+000a6cf0: 7464 3e43 6c6f 7564 733c 2f74 643e 0a20  td>Clouds</td>. 
+000a6d00: 2020 2020 203c 7464 3e53 686f 7020 2661       <td>Shop &a
+000a6d10: 6d70 3b20 5365 7276 6963 653c 2f74 643e  mp; Service</td>
+000a6d20: 0a20 2020 2020 203c 7464 3e53 7570 6572  .      <td>Super
+000a6d30: 6d61 726b 6574 3c2f 7464 3e0a 2020 2020  market</td>.    
+000a6d40: 2020 3c74 643e 4331 3c2f 7464 3e0a 2020    <td>C1</td>.  
+000a6d50: 2020 3c2f 7472 3e0a 2020 2020 3c74 723e    </tr>.    <tr>
+000a6d60: 0a20 2020 2020 203c 7468 3e31 3c2f 7468  .      <th>1</th
+000a6d70: 3e0a 2020 2020 2020 3c74 643e 313c 2f74  >.      <td>1</t
+000a6d80: 643e 0a20 2020 2020 203c 7464 3e34 302e  d>.      <td>40.
+000a6d90: 3836 3130 3738 3535 3139 3437 3220 2d37  8610785519472 -7
+000a6da0: 332e 3933 3031 3033 3730 3736 3331 353c  3.9301037076315<
+000a6db0: 2f74 643e 0a20 2020 2020 203c 7464 3e34  /td>.      <td>4
+000a6dc0: 3836 3c2f 7464 3e0a 2020 2020 2020 3c74  86</td>.      <t
+000a6dd0: 643e 4d6f 6e64 6179 3c2f 7464 3e0a 2020  d>Monday</td>.  
+000a6de0: 2020 2020 3c74 643e 2d31 2e30 3c2f 7464      <td>-1.0</td
+000a6df0: 3e0a 2020 2020 2020 3c74 643e 2d31 3c2f  >.      <td>-1</
+000a6e00: 7464 3e0a 2020 2020 2020 3c74 643e 436c  td>.      <td>Cl
+000a6e10: 6f75 6473 3c2f 7464 3e0a 2020 2020 2020  ouds</td>.      
+000a6e20: 3c74 643e 5265 7369 6465 6e63 653c 2f74  <td>Residence</t
+000a6e30: 643e 0a20 2020 2020 203c 7464 3e48 6f6d  d>.      <td>Hom
+000a6e40: 6520 2870 7269 7661 7465 293c 2f74 643e  e (private)</td>
+000a6e50: 0a20 2020 2020 203c 7464 3e43 313c 2f74  .      <td>C1</t
+000a6e60: 643e 0a20 2020 203c 2f74 723e 0a20 2020  d>.    </tr>.   
+000a6e70: 203c 7472 3e0a 2020 2020 2020 3c74 683e   <tr>.      <th>
+000a6e80: 323c 2f74 683e 0a20 2020 2020 203c 7464  2</th>.      <td
+000a6e90: 3e31 3c2f 7464 3e0a 2020 2020 2020 3c74  >1</td>.      <t
+000a6ea0: 643e 3430 2e35 3737 3435 3535 3831 3230  d>40.57745558120
+000a6eb0: 3835 202d 3733 2e39 3831 3234 3639 3438  85 -73.981246948
+000a6ec0: 3234 3232 3c2f 7464 3e0a 2020 2020 2020  2422</td>.      
+000a6ed0: 3c74 643e 3635 333c 2f74 643e 0a20 2020  <td>653</td>.   
+000a6ee0: 2020 203c 7464 3e4d 6f6e 6461 793c 2f74     <td>Monday</t
+000a6ef0: 643e 0a20 2020 2020 203c 7464 3e2d 312e  d>.      <td>-1.
+000a6f00: 303c 2f74 643e 0a20 2020 2020 203c 7464  0</td>.      <td
+000a6f10: 3e2d 313c 2f74 643e 0a20 2020 2020 203c  >-1</td>.      <
+000a6f20: 7464 3e43 6c65 6172 3c2f 7464 3e0a 2020  td>Clear</td>.  
+000a6f30: 2020 2020 3c74 643e 5472 6176 656c 2026      <td>Travel &
+000a6f40: 616d 703b 2054 7261 6e73 706f 7274 3c2f  amp; Transport</
+000a6f50: 7464 3e0a 2020 2020 2020 3c74 643e 4d65  td>.      <td>Me
+000a6f60: 7472 6f20 5374 6174 696f 6e3c 2f74 643e  tro Station</td>
+000a6f70: 0a20 2020 2020 203c 7464 3e43 313c 2f74  .      <td>C1</t
+000a6f80: 643e 0a20 2020 203c 2f74 723e 0a20 2020  d>.    </tr>.   
+000a6f90: 203c 7472 3e0a 2020 2020 2020 3c74 683e   <tr>.      <th>
+000a6fa0: 333c 2f74 683e 0a20 2020 2020 203c 7464  3</th>.      <td
+000a6fb0: 3e31 3c2f 7464 3e0a 2020 2020 2020 3c74  >1</td>.      <t
+000a6fc0: 643e 3430 2e38 3131 3433 3831 3532 3239  d>40.81143815229
+000a6fd0: 3535 202d 3734 2e30 3637 3739 3634 3638  55 -74.067796468
+000a6fe0: 3733 3437 3c2f 7464 3e0a 2020 2020 2020  7347</td>.      
+000a6ff0: 3c74 643e 3730 313c 2f74 643e 0a20 2020  <td>701</td>.   
+000a7000: 2020 203c 7464 3e4d 6f6e 6461 793c 2f74     <td>Monday</t
+000a7010: 643e 0a20 2020 2020 203c 7464 3e36 2e38  d>.      <td>6.8
+000a7020: 3c2f 7464 3e0a 2020 2020 2020 3c74 643e  </td>.      <td>
+000a7030: 2d31 3c2f 7464 3e0a 2020 2020 2020 3c74  -1</td>.      <t
+000a7040: 643e 5261 696e 3c2f 7464 3e0a 2020 2020  d>Rain</td>.    
+000a7050: 2020 3c74 643e 4172 7473 2026 616d 703b    <td>Arts &amp;
+000a7060: 2045 6e74 6572 7461 696e 6d65 6e74 3c2f   Entertainment</
+000a7070: 7464 3e0a 2020 2020 2020 3c74 643e 5374  td>.      <td>St
+000a7080: 6164 6975 6d3c 2f74 643e 0a20 2020 2020  adium</td>.     
+000a7090: 203c 7464 3e43 313c 2f74 643e 0a20 2020   <td>C1</td>.   
+000a70a0: 203c 2f74 723e 0a20 2020 203c 7472 3e0a   </tr>.    <tr>.
+000a70b0: 2020 2020 2020 3c74 683e 343c 2f74 683e        <th>4</th>
+000a70c0: 0a20 2020 2020 203c 7464 3e31 3c2f 7464  .      <td>1</td
+000a70d0: 3e0a 2020 2020 2020 3c74 643e 3430 2e37  >.      <td>40.7
+000a70e0: 3831 3138 3434 3336 3439 3736 202d 3733  811844364976 -73
+000a70f0: 2e39 3733 3230 3330 3933 3030 3635 3c2f  .9732030930065</
+000a7100: 7464 3e0a 2020 2020 2020 3c74 643e 3735  td>.      <td>75
+000a7110: 383c 2f74 643e 0a20 2020 2020 203c 7464  8</td>.      <td
+000a7120: 3e4d 6f6e 6461 793c 2f74 643e 0a20 2020  >Monday</td>.   
+000a7130: 2020 203c 7464 3e39 2e34 3c2f 7464 3e0a     <td>9.4</td>.
+000a7140: 2020 2020 2020 3c74 643e 2d31 3c2f 7464        <td>-1</td
+000a7150: 3e0a 2020 2020 2020 3c74 643e 436c 6561  >.      <td>Clea
+000a7160: 723c 2f74 643e 0a20 2020 2020 203c 7464  r</td>.      <td
+000a7170: 3e41 7274 7320 2661 6d70 3b20 456e 7465  >Arts &amp; Ente
+000a7180: 7274 6169 6e6d 656e 743c 2f74 643e 0a20  rtainment</td>. 
+000a7190: 2020 2020 203c 7464 3e53 6369 656e 6365       <td>Science
+000a71a0: 204d 7573 6575 6d3c 2f74 643e 0a20 2020   Museum</td>.   
+000a71b0: 2020 203c 7464 3e43 313c 2f74 643e 0a20     <td>C1</td>. 
+000a71c0: 2020 203c 2f74 723e 0a20 2020 203c 7472     </tr>.    <tr
+000a71d0: 3e0a 2020 2020 2020 3c74 683e 2e2e 2e3c  >.      <th>...<
+000a71e0: 2f74 683e 0a20 2020 2020 203c 7464 3e2e  /th>.      <td>.
+000a71f0: 2e2e 3c2f 7464 3e0a 2020 2020 2020 3c74  ..</td>.      <t
+000a7200: 643e 2e2e 2e3c 2f74 643e 0a20 2020 2020  d>...</td>.     
+000a7210: 203c 7464 3e2e 2e2e 3c2f 7464 3e0a 2020   <td>...</td>.  
+000a7220: 2020 2020 3c74 643e 2e2e 2e3c 2f74 643e      <td>...</td>
+000a7230: 0a20 2020 2020 203c 7464 3e2e 2e2e 3c2f  .      <td>...</
+000a7240: 7464 3e0a 2020 2020 2020 3c74 643e 2e2e  td>.      <td>..
+000a7250: 2e3c 2f74 643e 0a20 2020 2020 203c 7464  .</td>.      <td
+000a7260: 3e2e 2e2e 3c2f 7464 3e0a 2020 2020 2020  >...</td>.      
+000a7270: 3c74 643e 2e2e 2e3c 2f74 643e 0a20 2020  <td>...</td>.   
+000a7280: 2020 203c 7464 3e2e 2e2e 3c2f 7464 3e0a     <td>...</td>.
+000a7290: 2020 2020 2020 3c74 643e 2e2e 2e3c 2f74        <td>...</t
+000a72a0: 643e 0a20 2020 203c 2f74 723e 0a20 2020  d>.    </tr>.   
+000a72b0: 203c 7472 3e0a 2020 2020 2020 3c74 683e   <tr>.      <th>
+000a72c0: 3439 353c 2f74 683e 0a20 2020 2020 203c  495</th>.      <
+000a72d0: 7464 3e31 303c 2f74 643e 0a20 2020 2020  td>10</td>.     
+000a72e0: 203c 7464 3e34 302e 3736 3338 3838 3537   <td>40.76388857
+000a72f0: 3131 3137 3920 2d37 342e 3032 3333 3832  11179 -74.023382
+000a7300: 3138 3038 3335 323c 2f74 643e 0a20 2020  1808352</td>.   
+000a7310: 2020 203c 7464 3e31 3338 353c 2f74 643e     <td>1385</td>
+000a7320: 0a20 2020 2020 203c 7464 3e53 6174 7572  .      <td>Satur
+000a7330: 6461 793c 2f74 643e 0a20 2020 2020 203c  day</td>.      <
+000a7340: 7464 3e2d 312e 303c 2f74 643e 0a20 2020  td>-1.0</td>.   
+000a7350: 2020 203c 7464 3e2d 313c 2f74 643e 0a20     <td>-1</td>. 
+000a7360: 2020 2020 203c 7464 3e43 6c6f 7564 733c       <td>Clouds<
+000a7370: 2f74 643e 0a20 2020 2020 203c 7464 3e54  /td>.      <td>T
+000a7380: 7261 7665 6c20 2661 6d70 3b20 5472 616e  ravel &amp; Tran
+000a7390: 7370 6f72 743c 2f74 643e 0a20 2020 2020  sport</td>.     
+000a73a0: 203c 7464 3e42 6f72 6465 7220 4372 6f73   <td>Border Cros
+000a73b0: 7369 6e67 3c2f 7464 3e0a 2020 2020 2020  sing</td>.      
+000a73c0: 3c74 643e 4331 3c2f 7464 3e0a 2020 2020  <td>C1</td>.    
+000a73d0: 3c2f 7472 3e0a 2020 2020 3c74 723e 0a20  </tr>.    <tr>. 
+000a73e0: 2020 2020 203c 7468 3e34 3936 3c2f 7468       <th>496</th
+000a73f0: 3e0a 2020 2020 2020 3c74 643e 3130 3c2f  >.      <td>10</
+000a7400: 7464 3e0a 2020 2020 2020 3c74 643e 3430  td>.      <td>40
+000a7410: 2e36 3839 3134 3431 3334 3532 3135 202d  .6891441345215 -
+000a7420: 3733 2e39 3330 3332 3037 3339 3734 3631  73.9303207397461
+000a7430: 3c2f 7464 3e0a 2020 2020 2020 3c74 643e  </td>.      <td>
+000a7440: 3337 393c 2f74 643e 0a20 2020 2020 203c  379</td>.      <
+000a7450: 7464 3e53 756e 6461 793c 2f74 643e 0a20  td>Sunday</td>. 
+000a7460: 2020 2020 203c 7464 3e2d 312e 303c 2f74       <td>-1.0</t
+000a7470: 643e 0a20 2020 2020 203c 7464 3e31 3c2f  d>.      <td>1</
+000a7480: 7464 3e0a 2020 2020 2020 3c74 643e 436c  td>.      <td>Cl
+000a7490: 6f75 6473 3c2f 7464 3e0a 2020 2020 2020  ouds</td>.      
+000a74a0: 3c74 643e 466f 6f64 3c2f 7464 3e0a 2020  <td>Food</td>.  
+000a74b0: 2020 2020 3c74 643e 4465 6c69 202f 2042      <td>Deli / B
+000a74c0: 6f64 6567 613c 2f74 643e 0a20 2020 2020  odega</td>.     
+000a74d0: 203c 7464 3e43 313c 2f74 643e 0a20 2020   <td>C1</td>.   
+000a74e0: 203c 2f74 723e 0a20 2020 203c 7472 3e0a   </tr>.    <tr>.
+000a74f0: 2020 2020 2020 3c74 683e 3439 373c 2f74        <th>497</t
+000a7500: 683e 0a20 2020 2020 203c 7464 3e31 303c  h>.      <td>10<
+000a7510: 2f74 643e 0a20 2020 2020 203c 7464 3e34  /td>.      <td>4
+000a7520: 302e 3737 3034 3730 3335 3030 3030 3020  0.7704703500000 
+000a7530: 2d37 342e 3032 3831 3833 3134 3030 3030  -74.028183140000
+000a7540: 303c 2f74 643e 0a20 2020 2020 203c 7464  0</td>.      <td
+000a7550: 3e35 3437 3c2f 7464 3e0a 2020 2020 2020  >547</td>.      
+000a7560: 3c74 643e 5375 6e64 6179 3c2f 7464 3e0a  <td>Sunday</td>.
+000a7570: 2020 2020 2020 3c74 643e 2d31 2e30 3c2f        <td>-1.0</
+000a7580: 7464 3e0a 2020 2020 2020 3c74 643e 2d31  td>.      <td>-1
+000a7590: 3c2f 7464 3e0a 2020 2020 2020 3c74 643e  </td>.      <td>
+000a75a0: 436c 6561 723c 2f74 643e 0a20 2020 2020  Clear</td>.     
+000a75b0: 203c 7464 3e50 726f 6665 7373 696f 6e61   <td>Professiona
+000a75c0: 6c20 2661 6d70 3b20 4f74 6865 7220 506c  l &amp; Other Pl
+000a75d0: 6163 6573 3c2f 7464 3e0a 2020 2020 2020  aces</td>.      
+000a75e0: 3c74 643e 506f 7374 204f 6666 6963 653c  <td>Post Office<
+000a75f0: 2f74 643e 0a20 2020 2020 203c 7464 3e43  /td>.      <td>C
+000a7600: 313c 2f74 643e 0a20 2020 203c 2f74 723e  1</td>.    </tr>
+000a7610: 0a20 2020 203c 7472 3e0a 2020 2020 2020  .    <tr>.      
+000a7620: 3c74 683e 3439 383c 2f74 683e 0a20 2020  <th>498</th>.   
+000a7630: 2020 203c 7464 3e31 303c 2f74 643e 0a20     <td>10</td>. 
+000a7640: 2020 2020 203c 7464 3e34 302e 3737 3734       <td>40.7774
+000a7650: 3737 3339 3232 3038 3720 2d37 332e 3831  773922087 -73.81
+000a7660: 3436 3732 3537 3535 3634 333c 2f74 643e  46725755643</td>
+000a7670: 0a20 2020 2020 203c 7464 3e37 3833 3c2f  .      <td>783</
+000a7680: 7464 3e0a 2020 2020 2020 3c74 643e 5375  td>.      <td>Su
+000a7690: 6e64 6179 3c2f 7464 3e0a 2020 2020 2020  nday</td>.      
+000a76a0: 3c74 643e 2d31 2e30 3c2f 7464 3e0a 2020  <td>-1.0</td>.  
+000a76b0: 2020 2020 3c74 643e 2d31 3c2f 7464 3e0a      <td>-1</td>.
+000a76c0: 2020 2020 2020 3c74 643e 436c 6561 723c        <td>Clear<
+000a76d0: 2f74 643e 0a20 2020 2020 203c 7464 3e53  /td>.      <td>S
+000a76e0: 686f 7020 2661 6d70 3b20 5365 7276 6963  hop &amp; Servic
+000a76f0: 653c 2f74 643e 0a20 2020 2020 203c 7464  e</td>.      <td
+000a7700: 3e43 616e 6479 2053 746f 7265 3c2f 7464  >Candy Store</td
+000a7710: 3e0a 2020 2020 2020 3c74 643e 4331 3c2f  >.      <td>C1</
+000a7720: 7464 3e0a 2020 2020 3c2f 7472 3e0a 2020  td>.    </tr>.  
+000a7730: 2020 3c74 723e 0a20 2020 2020 203c 7468    <tr>.      <th
+000a7740: 3e34 3939 3c2f 7468 3e0a 2020 2020 2020  >499</th>.      
+000a7750: 3c74 643e 3130 3c2f 7464 3e0a 2020 2020  <td>10</td>.    
+000a7760: 2020 3c74 643e 3430 2e38 3333 3136 3532    <td>40.8331652
+000a7770: 3030 3632 3234 202d 3733 2e39 3431 3836  006224 -73.94186
+000a7780: 3033 3432 3736 3932 3c2f 7464 3e0a 2020  03427692</td>.  
+000a7790: 2020 2020 3c74 643e 3130 3333 3c2f 7464      <td>1033</td
+000a77a0: 3e0a 2020 2020 2020 3c74 643e 5375 6e64  >.      <td>Sund
+000a77b0: 6179 3c2f 7464 3e0a 2020 2020 2020 3c74  ay</td>.      <t
+000a77c0: 643e 2d31 2e30 3c2f 7464 3e0a 2020 2020  d>-1.0</td>.    
+000a77d0: 2020 3c74 643e 2d31 3c2f 7464 3e0a 2020    <td>-1</td>.  
+000a77e0: 2020 2020 3c74 643e 436c 6f75 6473 3c2f      <td>Clouds</
+000a77f0: 7464 3e0a 2020 2020 2020 3c74 643e 5265  td>.      <td>Re
+000a7800: 7369 6465 6e63 653c 2f74 643e 0a20 2020  sidence</td>.   
+000a7810: 2020 203c 7464 3e48 6f6d 6520 2870 7269     <td>Home (pri
+000a7820: 7661 7465 293c 2f74 643e 0a20 2020 2020  vate)</td>.     
+000a7830: 203c 7464 3e43 313c 2f74 643e 0a20 2020   <td>C1</td>.   
+000a7840: 203c 2f74 723e 0a20 203c 2f74 626f 6479   </tr>.  </tbody
+000a7850: 3e0a 3c2f 7461 626c 653e 0a3c 703e 3530  >.</table>.<p>50
+000a7860: 3020 726f 7773 20c3 9720 3130 2063 6f6c  0 rows .. 10 col
+000a7870: 756d 6e73 3c2f 703e 0a3c 2f64 6976 3e0a  umns</p>.</div>.
+000a7880: 3c2f 6469 763e 0a0a 3c2f 6469 763e 0a0a  </div>..</div>..
+000a7890: 3c2f 6469 763e 0a0a 3c2f 6469 763e 0a0a  </div>..</div>..
+000a78a0: 3c2f 6469 763e 0a3c 6469 7620 636c 6173  </div>.<div clas
+000a78b0: 733d 226a 702d 4365 6c6c 206a 702d 4d61  s="jp-Cell jp-Ma
+000a78c0: 726b 646f 776e 4365 6c6c 206a 702d 4e6f  rkdownCell jp-No
+000a78d0: 7465 626f 6f6b 2d63 656c 6c22 3e0a 3c64  tebook-cell">.<d
+000a78e0: 6976 2063 6c61 7373 3d22 6a70 2d43 656c  iv class="jp-Cel
+000a78f0: 6c2d 696e 7075 7457 7261 7070 6572 223e  l-inputWrapper">
+000a7900: 0a3c 6469 7620 636c 6173 733d 226a 702d  .<div class="jp-
+000a7910: 436f 6c6c 6170 7365 7220 6a70 2d49 6e70  Collapser jp-Inp
+000a7920: 7574 436f 6c6c 6170 7365 7220 6a70 2d43  utCollapser jp-C
+000a7930: 656c 6c2d 696e 7075 7443 6f6c 6c61 7073  ell-inputCollaps
+000a7940: 6572 223e 0a3c 2f64 6976 3e0a 3c64 6976  er">.</div>.<div
+000a7950: 2063 6c61 7373 3d22 6a70 2d49 6e70 7574   class="jp-Input
+000a7960: 4172 6561 206a 702d 4365 6c6c 2d69 6e70  Area jp-Cell-inp
+000a7970: 7574 4172 6561 223e 3c64 6976 2063 6c61  utArea"><div cla
+000a7980: 7373 3d22 6a70 2d49 6e70 7574 5072 6f6d  ss="jp-InputProm
+000a7990: 7074 206a 702d 496e 7075 7441 7265 612d  pt jp-InputArea-
+000a79a0: 7072 6f6d 7074 223e 0a3c 2f64 6976 3e3c  prompt">.</div><
+000a79b0: 6469 7620 636c 6173 733d 226a 702d 5265  div class="jp-Re
+000a79c0: 6e64 6572 6564 4854 4d4c 436f 6d6d 6f6e  nderedHTMLCommon
+000a79d0: 206a 702d 5265 6e64 6572 6564 4d61 726b   jp-RenderedMark
+000a79e0: 646f 776e 206a 702d 4d61 726b 646f 776e  down jp-Markdown
+000a79f0: 4f75 7470 7574 2022 2064 6174 612d 6d69  Output " data-mi
+000a7a00: 6d65 2d74 7970 653d 2274 6578 742f 6d61  me-type="text/ma
+000a7a10: 726b 646f 776e 223e 0a3c 703e 546f 2073  rkdown">.<p>To s
+000a7a20: 7065 6369 6679 2074 6865 2073 796e 7468  pecify the synth
+000a7a30: 6574 6963 2064 6174 6173 6574 2070 6172  etic dataset par
+000a7a40: 616d 6574 6572 733a 3c2f 703e 0a0a 3c2f  ameters:</p>..</
+000a7a50: 6469 763e 0a3c 2f64 6976 3e0a 3c2f 6469  div>.</div>.</di
+000a7a60: 763e 0a3c 2f64 6976 3e3c 6469 7620 636c  v>.</div><div cl
+000a7a70: 6173 733d 226a 702d 4365 6c6c 206a 702d  ass="jp-Cell jp-
+000a7a80: 436f 6465 4365 6c6c 206a 702d 4e6f 7465  CodeCell jp-Note
+000a7a90: 626f 6f6b 2d63 656c 6c20 2020 223e 0a3c  book-cell   ">.<
+000a7aa0: 6469 7620 636c 6173 733d 226a 702d 4365  div class="jp-Ce
+000a7ab0: 6c6c 2d69 6e70 7574 5772 6170 7065 7222  ll-inputWrapper"
+000a7ac0: 3e0a 3c64 6976 2063 6c61 7373 3d22 6a70  >.<div class="jp
+000a7ad0: 2d43 6f6c 6c61 7073 6572 206a 702d 496e  -Collapser jp-In
+000a7ae0: 7075 7443 6f6c 6c61 7073 6572 206a 702d  putCollapser jp-
+000a7af0: 4365 6c6c 2d69 6e70 7574 436f 6c6c 6170  Cell-inputCollap
+000a7b00: 7365 7222 3e0a 3c2f 6469 763e 0a3c 6469  ser">.</div>.<di
+000a7b10: 7620 636c 6173 733d 226a 702d 496e 7075  v class="jp-Inpu
+000a7b20: 7441 7265 6120 6a70 2d43 656c 6c2d 696e  tArea jp-Cell-in
+000a7b30: 7075 7441 7265 6122 3e0a 3c64 6976 2063  putArea">.<div c
+000a7b40: 6c61 7373 3d22 6a70 2d49 6e70 7574 5072  lass="jp-InputPr
+000a7b50: 6f6d 7074 206a 702d 496e 7075 7441 7265  ompt jp-InputAre
+000a7b60: 612d 7072 6f6d 7074 223e 496e 266e 6273  a-prompt">In&nbs
+000a7b70: 703b 5b33 5d3a 3c2f 6469 763e 0a3c 6469  p;[3]:</div>.<di
+000a7b80: 7620 636c 6173 733d 226a 702d 436f 6465  v class="jp-Code
+000a7b90: 4d69 7272 6f72 4564 6974 6f72 206a 702d  MirrorEditor jp-
+000a7ba0: 4564 6974 6f72 206a 702d 496e 7075 7441  Editor jp-InputA
+000a7bb0: 7265 612d 6564 6974 6f72 2220 6461 7461  rea-editor" data
+000a7bc0: 2d74 7970 653d 2269 6e6c 696e 6522 3e0a  -type="inline">.
+000a7bd0: 2020 2020 203c 6469 7620 636c 6173 733d       <div class=
+000a7be0: 2243 6f64 654d 6972 726f 7220 636d 2d73  "CodeMirror cm-s
+000a7bf0: 2d6a 7570 7974 6572 223e 0a3c 6469 7620  -jupyter">.<div 
+000a7c00: 636c 6173 733d 2220 6869 6768 6c69 6768  class=" highligh
+000a7c10: 7420 686c 2d69 7079 7468 6f6e 3322 3e3c  t hl-ipython3"><
+000a7c20: 7072 653e 3c73 7061 6e3e 3c2f 7370 616e  pre><span></span
+000a7c30: 3e3c 7370 616e 2063 6c61 7373 3d22 6e22  ><span class="n"
+000a7c40: 3e4e 3c2f 7370 616e 3e3c 7370 616e 2063  >N</span><span c
+000a7c50: 6c61 7373 3d22 6f22 3e3d 3c2f 7370 616e  lass="o">=</span
+000a7c60: 3e3c 7370 616e 2063 6c61 7373 3d22 6d69  ><span class="mi
+000a7c70: 223e 3130 3c2f 7370 616e 3e20 3c73 7061  ">10</span> <spa
+000a7c80: 6e20 636c 6173 733d 2263 3122 3e23 204e  n class="c1"># N
+000a7c90: 756d 6265 7220 6f66 2074 7261 6a65 6374  umber of traject
+000a7ca0: 6f72 6965 733c 2f73 7061 6e3e 0a3c 7370  ories</span>.<sp
+000a7cb0: 616e 2063 6c61 7373 3d22 6e22 3e4d 3c2f  an class="n">M</
+000a7cc0: 7370 616e 3e3c 7370 616e 2063 6c61 7373  span><span class
+000a7cd0: 3d22 6f22 3e3d 3c2f 7370 616e 3e3c 7370  ="o">=</span><sp
+000a7ce0: 616e 2063 6c61 7373 3d22 6d69 223e 3530  an class="mi">50
+000a7cf0: 3c2f 7370 616e 3e20 3c73 7061 6e20 636c  </span> <span cl
+000a7d00: 6173 733d 2263 3122 3e23 204e 756d 6265  ass="c1"># Numbe
+000a7d10: 7220 6f66 2070 6f69 6e74 7320 6279 2074  r of points by t
+000a7d20: 7261 6a65 6374 6f72 793c 2f73 7061 6e3e  rajectory</span>
+000a7d30: 0a3c 7370 616e 2063 6c61 7373 3d22 6e22  .<span class="n"
+000a7d40: 3e43 3c2f 7370 616e 3e3c 7370 616e 2063  >C</span><span c
+000a7d50: 6c61 7373 3d22 6f22 3e3d 3c2f 7370 616e  lass="o">=</span
+000a7d60: 3e3c 7370 616e 2063 6c61 7373 3d22 6d69  ><span class="mi
+000a7d70: 223e 333c 2f73 7061 6e3e 2020 3c73 7061  ">3</span>  <spa
+000a7d80: 6e20 636c 6173 733d 2263 3122 3e23 204e  n class="c1"># N
+000a7d90: 756d 6265 7220 6f66 2063 6c61 7373 6573  umber of classes
+000a7da0: 2028 4331 2074 6f20 436e 293c 2f73 7061   (C1 to Cn)</spa
+000a7db0: 6e3e 0a3c 7370 616e 2063 6c61 7373 3d22  n>.<span class="
+000a7dc0: 6e22 3e73 616d 706c 6572 4765 6e65 7261  n">samplerGenera
+000a7dd0: 746f 723c 2f73 7061 6e3e 3c73 7061 6e20  tor</span><span 
+000a7de0: 636c 6173 733d 2270 223e 283c 2f73 7061  class="p">(</spa
+000a7df0: 6e3e 3c73 7061 6e20 636c 6173 733d 226e  n><span class="n
+000a7e00: 223e 4e3c 2f73 7061 6e3e 3c73 7061 6e20  ">N</span><span 
+000a7e10: 636c 6173 733d 2270 223e 2c3c 2f73 7061  class="p">,</spa
+000a7e20: 6e3e 203c 7370 616e 2063 6c61 7373 3d22  n> <span class="
+000a7e30: 6e22 3e4d 3c2f 7370 616e 3e3c 7370 616e  n">M</span><span
+000a7e40: 2063 6c61 7373 3d22 7022 3e2c 3c2f 7370   class="p">,</sp
+000a7e50: 616e 3e20 3c73 7061 6e20 636c 6173 733d  an> <span class=
+000a7e60: 226e 223e 433c 2f73 7061 6e3e 3c73 7061  "n">C</span><spa
+000a7e70: 6e20 636c 6173 733d 2270 223e 293c 2f73  n class="p">)</s
+000a7e80: 7061 6e3e 0a3c 2f70 7265 3e3c 2f64 6976  pan>.</pre></div
+000a7e90: 3e0a 0a20 2020 2020 3c2f 6469 763e 0a3c  >..     </div>.<
+000a7ea0: 2f64 6976 3e0a 3c2f 6469 763e 0a3c 2f64  /div>.</div>.</d
+000a7eb0: 6976 3e0a 0a3c 6469 7620 636c 6173 733d  iv>..<div class=
+000a7ec0: 226a 702d 4365 6c6c 2d6f 7574 7075 7457  "jp-Cell-outputW
+000a7ed0: 7261 7070 6572 223e 0a3c 6469 7620 636c  rapper">.<div cl
+000a7ee0: 6173 733d 226a 702d 436f 6c6c 6170 7365  ass="jp-Collapse
+000a7ef0: 7220 6a70 2d4f 7574 7075 7443 6f6c 6c61  r jp-OutputColla
+000a7f00: 7073 6572 206a 702d 4365 6c6c 2d6f 7574  pser jp-Cell-out
+000a7f10: 7075 7443 6f6c 6c61 7073 6572 223e 0a3c  putCollapser">.<
+000a7f20: 2f64 6976 3e0a 0a0a 3c64 6976 2063 6c61  /div>...<div cla
+000a7f30: 7373 3d22 6a70 2d4f 7574 7075 7441 7265  ss="jp-OutputAre
+000a7f40: 6120 6a70 2d43 656c 6c2d 6f75 7470 7574  a jp-Cell-output
+000a7f50: 4172 6561 223e 0a0a 3c64 6976 2063 6c61  Area">..<div cla
+000a7f60: 7373 3d22 6a70 2d4f 7574 7075 7441 7265  ss="jp-OutputAre
+000a7f70: 612d 6368 696c 6422 3e0a 0a20 2020 200a  a-child">..    .
+000a7f80: 2020 2020 3c64 6976 2063 6c61 7373 3d22      <div class="
+000a7f90: 6a70 2d4f 7574 7075 7450 726f 6d70 7420  jp-OutputPrompt 
+000a7fa0: 6a70 2d4f 7574 7075 7441 7265 612d 7072  jp-OutputArea-pr
+000a7fb0: 6f6d 7074 223e 4f75 745b 335d 3a3c 2f64  ompt">Out[3]:</d
+000a7fc0: 6976 3e0a 0a0a 0a3c 6469 7620 636c 6173  iv>....<div clas
+000a7fd0: 733d 226a 702d 5265 6e64 6572 6564 4854  s="jp-RenderedHT
+000a7fe0: 4d4c 436f 6d6d 6f6e 206a 702d 5265 6e64  MLCommon jp-Rend
+000a7ff0: 6572 6564 4854 4d4c 206a 702d 4f75 7470  eredHTML jp-Outp
+000a8000: 7574 4172 6561 2d6f 7574 7075 7420 6a70  utArea-output jp
+000a8010: 2d4f 7574 7075 7441 7265 612d 6578 6563  -OutputArea-exec
+000a8020: 7574 6552 6573 756c 7422 2064 6174 612d  uteResult" data-
+000a8030: 6d69 6d65 2d74 7970 653d 2274 6578 742f  mime-type="text/
+000a8040: 6874 6d6c 223e 0a3c 6469 763e 0a3c 7374  html">.<div>.<st
+000a8050: 796c 6520 7363 6f70 6564 3e0a 2020 2020  yle scoped>.    
+000a8060: 2e64 6174 6166 7261 6d65 2074 626f 6479  .dataframe tbody
+000a8070: 2074 7220 7468 3a6f 6e6c 792d 6f66 2d74   tr th:only-of-t
+000a8080: 7970 6520 7b0a 2020 2020 2020 2020 7665  ype {.        ve
+000a8090: 7274 6963 616c 2d61 6c69 676e 3a20 6d69  rtical-align: mi
+000a80a0: 6464 6c65 3b0a 2020 2020 7d0a 0a20 2020  ddle;.    }..   
+000a80b0: 202e 6461 7461 6672 616d 6520 7462 6f64   .dataframe tbod
+000a80c0: 7920 7472 2074 6820 7b0a 2020 2020 2020  y tr th {.      
+000a80d0: 2020 7665 7274 6963 616c 2d61 6c69 676e    vertical-align
+000a80e0: 3a20 746f 703b 0a20 2020 207d 0a0a 2020  : top;.    }..  
+000a80f0: 2020 2e64 6174 6166 7261 6d65 2074 6865    .dataframe the
+000a8100: 6164 2074 6820 7b0a 2020 2020 2020 2020  ad th {.        
+000a8110: 7465 7874 2d61 6c69 676e 3a20 7269 6768  text-align: righ
+000a8120: 743b 0a20 2020 207d 0a3c 2f73 7479 6c65  t;.    }.</style
+000a8130: 3e0a 3c74 6162 6c65 2062 6f72 6465 723d  >.<table border=
+000a8140: 2231 2220 636c 6173 733d 2264 6174 6166  "1" class="dataf
+000a8150: 7261 6d65 223e 0a20 203c 7468 6561 643e  rame">.  <thead>
+000a8160: 0a20 2020 203c 7472 2073 7479 6c65 3d22  .    <tr style="
+000a8170: 7465 7874 2d61 6c69 676e 3a20 7269 6768  text-align: righ
+000a8180: 743b 223e 0a20 2020 2020 203c 7468 3e3c  t;">.      <th><
+000a8190: 2f74 683e 0a20 2020 2020 203c 7468 3e74  /th>.      <th>t
+000a81a0: 6964 3c2f 7468 3e0a 2020 2020 2020 3c74  id</th>.      <t
+000a81b0: 683e 7370 6163 653c 2f74 683e 0a20 2020  h>space</th>.   
+000a81c0: 2020 203c 7468 3e74 696d 653c 2f74 683e     <th>time</th>
+000a81d0: 0a20 2020 2020 203c 7468 3e64 6179 3c2f  .      <th>day</
+000a81e0: 7468 3e0a 2020 2020 2020 3c74 683e 7261  th>.      <th>ra
+000a81f0: 7469 6e67 3c2f 7468 3e0a 2020 2020 2020  ting</th>.      
+000a8200: 3c74 683e 7072 6963 653c 2f74 683e 0a20  <th>price</th>. 
+000a8210: 2020 2020 203c 7468 3e77 6561 7468 6572       <th>weather
+000a8220: 3c2f 7468 3e0a 2020 2020 2020 3c74 683e  </th>.      <th>
+000a8230: 726f 6f74 5f74 7970 653c 2f74 683e 0a20  root_type</th>. 
+000a8240: 2020 2020 203c 7468 3e74 7970 653c 2f74       <th>type</t
+000a8250: 683e 0a20 2020 2020 203c 7468 3e6c 6162  h>.      <th>lab
+000a8260: 656c 3c2f 7468 3e0a 2020 2020 3c2f 7472  el</th>.    </tr
+000a8270: 3e0a 2020 3c2f 7468 6561 643e 0a20 203c  >.  </thead>.  <
+000a8280: 7462 6f64 793e 0a20 2020 203c 7472 3e0a  tbody>.    <tr>.
+000a8290: 2020 2020 2020 3c74 683e 303c 2f74 683e        <th>0</th>
+000a82a0: 0a20 2020 2020 203c 7464 3e31 3c2f 7464  .      <td>1</td
+000a82b0: 3e0a 2020 2020 2020 3c74 643e 3430 2e37  >.      <td>40.7
+000a82c0: 3432 3936 3932 3338 3232 3836 202d 3733  429692382286 -73
+000a82d0: 2e38 3832 3736 3639 3632 3035 3134 3c2f  .8827669620514</
+000a82e0: 7464 3e0a 2020 2020 2020 3c74 643e 3434  td>.      <td>44
+000a82f0: 373c 2f74 643e 0a20 2020 2020 203c 7464  7</td>.      <td
+000a8300: 3e4d 6f6e 6461 793c 2f74 643e 0a20 2020  >Monday</td>.   
+000a8310: 2020 203c 7464 3e36 2e31 3c2f 7464 3e0a     <td>6.1</td>.
+000a8320: 2020 2020 2020 3c74 643e 2d31 3c2f 7464        <td>-1</td
+000a8330: 3e0a 2020 2020 2020 3c74 643e 436c 6f75  >.      <td>Clou
+000a8340: 6473 3c2f 7464 3e0a 2020 2020 2020 3c74  ds</td>.      <t
+000a8350: 643e 5368 6f70 2026 616d 703b 2053 6572  d>Shop &amp; Ser
+000a8360: 7669 6365 3c2f 7464 3e0a 2020 2020 2020  vice</td>.      
+000a8370: 3c74 643e 5375 7065 726d 6172 6b65 743c  <td>Supermarket<
+000a8380: 2f74 643e 0a20 2020 2020 203c 7464 3e43  /td>.      <td>C
+000a8390: 313c 2f74 643e 0a20 2020 203c 2f74 723e  1</td>.    </tr>
+000a83a0: 0a20 2020 203c 7472 3e0a 2020 2020 2020  .    <tr>.      
+000a83b0: 3c74 683e 313c 2f74 683e 0a20 2020 2020  <th>1</th>.     
+000a83c0: 203c 7464 3e31 3c2f 7464 3e0a 2020 2020   <td>1</td>.    
+000a83d0: 2020 3c74 643e 3430 2e38 3631 3037 3835    <td>40.8610785
+000a83e0: 3531 3934 3732 202d 3733 2e39 3330 3130  519472 -73.93010
+000a83f0: 3337 3037 3633 3135 3c2f 7464 3e0a 2020  37076315</td>.  
+000a8400: 2020 2020 3c74 643e 3438 363c 2f74 643e      <td>486</td>
+000a8410: 0a20 2020 2020 203c 7464 3e4d 6f6e 6461  .      <td>Monda
+000a8420: 793c 2f74 643e 0a20 2020 2020 203c 7464  y</td>.      <td
+000a8430: 3e2d 312e 303c 2f74 643e 0a20 2020 2020  >-1.0</td>.     
+000a8440: 203c 7464 3e2d 313c 2f74 643e 0a20 2020   <td>-1</td>.   
+000a8450: 2020 203c 7464 3e43 6c6f 7564 733c 2f74     <td>Clouds</t
+000a8460: 643e 0a20 2020 2020 203c 7464 3e52 6573  d>.      <td>Res
+000a8470: 6964 656e 6365 3c2f 7464 3e0a 2020 2020  idence</td>.    
+000a8480: 2020 3c74 643e 486f 6d65 2028 7072 6976    <td>Home (priv
+000a8490: 6174 6529 3c2f 7464 3e0a 2020 2020 2020  ate)</td>.      
+000a84a0: 3c74 643e 4331 3c2f 7464 3e0a 2020 2020  <td>C1</td>.    
+000a84b0: 3c2f 7472 3e0a 2020 2020 3c74 723e 0a20  </tr>.    <tr>. 
+000a84c0: 2020 2020 203c 7468 3e32 3c2f 7468 3e0a       <th>2</th>.
+000a84d0: 2020 2020 2020 3c74 643e 313c 2f74 643e        <td>1</td>
+000a84e0: 0a20 2020 2020 203c 7464 3e34 302e 3537  .      <td>40.57
+000a84f0: 3734 3535 3538 3132 3038 3520 2d37 332e  74555812085 -73.
+000a8500: 3938 3132 3436 3934 3832 3432 323c 2f74  9812469482422</t
+000a8510: 643e 0a20 2020 2020 203c 7464 3e36 3533  d>.      <td>653
+000a8520: 3c2f 7464 3e0a 2020 2020 2020 3c74 643e  </td>.      <td>
+000a8530: 4d6f 6e64 6179 3c2f 7464 3e0a 2020 2020  Monday</td>.    
+000a8540: 2020 3c74 643e 2d31 2e30 3c2f 7464 3e0a    <td>-1.0</td>.
+000a8550: 2020 2020 2020 3c74 643e 2d31 3c2f 7464        <td>-1</td
+000a8560: 3e0a 2020 2020 2020 3c74 643e 436c 6561  >.      <td>Clea
+000a8570: 723c 2f74 643e 0a20 2020 2020 203c 7464  r</td>.      <td
+000a8580: 3e54 7261 7665 6c20 2661 6d70 3b20 5472  >Travel &amp; Tr
+000a8590: 616e 7370 6f72 743c 2f74 643e 0a20 2020  ansport</td>.   
+000a85a0: 2020 203c 7464 3e4d 6574 726f 2053 7461     <td>Metro Sta
+000a85b0: 7469 6f6e 3c2f 7464 3e0a 2020 2020 2020  tion</td>.      
+000a85c0: 3c74 643e 4331 3c2f 7464 3e0a 2020 2020  <td>C1</td>.    
+000a85d0: 3c2f 7472 3e0a 2020 2020 3c74 723e 0a20  </tr>.    <tr>. 
+000a85e0: 2020 2020 203c 7468 3e33 3c2f 7468 3e0a       <th>3</th>.
+000a85f0: 2020 2020 2020 3c74 643e 313c 2f74 643e        <td>1</td>
+000a8600: 0a20 2020 2020 203c 7464 3e34 302e 3831  .      <td>40.81
+000a8610: 3134 3338 3135 3232 3935 3520 2d37 342e  14381522955 -74.
+000a8620: 3036 3737 3936 3436 3837 3334 373c 2f74  0677964687347</t
+000a8630: 643e 0a20 2020 2020 203c 7464 3e37 3031  d>.      <td>701
+000a8640: 3c2f 7464 3e0a 2020 2020 2020 3c74 643e  </td>.      <td>
+000a8650: 4d6f 6e64 6179 3c2f 7464 3e0a 2020 2020  Monday</td>.    
+000a8660: 2020 3c74 643e 362e 383c 2f74 643e 0a20    <td>6.8</td>. 
+000a8670: 2020 2020 203c 7464 3e2d 313c 2f74 643e       <td>-1</td>
+000a8680: 0a20 2020 2020 203c 7464 3e52 6169 6e3c  .      <td>Rain<
+000a8690: 2f74 643e 0a20 2020 2020 203c 7464 3e41  /td>.      <td>A
+000a86a0: 7274 7320 2661 6d70 3b20 456e 7465 7274  rts &amp; Entert
+000a86b0: 6169 6e6d 656e 743c 2f74 643e 0a20 2020  ainment</td>.   
+000a86c0: 2020 203c 7464 3e53 7461 6469 756d 3c2f     <td>Stadium</
+000a86d0: 7464 3e0a 2020 2020 2020 3c74 643e 4331  td>.      <td>C1
+000a86e0: 3c2f 7464 3e0a 2020 2020 3c2f 7472 3e0a  </td>.    </tr>.
+000a86f0: 2020 2020 3c74 723e 0a20 2020 2020 203c      <tr>.      <
+000a8700: 7468 3e34 3c2f 7468 3e0a 2020 2020 2020  th>4</th>.      
+000a8710: 3c74 643e 313c 2f74 643e 0a20 2020 2020  <td>1</td>.     
+000a8720: 203c 7464 3e34 302e 3738 3131 3834 3433   <td>40.78118443
+000a8730: 3634 3937 3620 2d37 332e 3937 3332 3033  64976 -73.973203
+000a8740: 3039 3330 3036 353c 2f74 643e 0a20 2020  0930065</td>.   
+000a8750: 2020 203c 7464 3e37 3538 3c2f 7464 3e0a     <td>758</td>.
+000a8760: 2020 2020 2020 3c74 643e 4d6f 6e64 6179        <td>Monday
+000a8770: 3c2f 7464 3e0a 2020 2020 2020 3c74 643e  </td>.      <td>
+000a8780: 392e 343c 2f74 643e 0a20 2020 2020 203c  9.4</td>.      <
+000a8790: 7464 3e2d 313c 2f74 643e 0a20 2020 2020  td>-1</td>.     
+000a87a0: 203c 7464 3e43 6c65 6172 3c2f 7464 3e0a   <td>Clear</td>.
+000a87b0: 2020 2020 2020 3c74 643e 4172 7473 2026        <td>Arts &
+000a87c0: 616d 703b 2045 6e74 6572 7461 696e 6d65  amp; Entertainme
+000a87d0: 6e74 3c2f 7464 3e0a 2020 2020 2020 3c74  nt</td>.      <t
+000a87e0: 643e 5363 6965 6e63 6520 4d75 7365 756d  d>Science Museum
+000a87f0: 3c2f 7464 3e0a 2020 2020 2020 3c74 643e  </td>.      <td>
+000a8800: 4331 3c2f 7464 3e0a 2020 2020 3c2f 7472  C1</td>.    </tr
+000a8810: 3e0a 2020 2020 3c74 723e 0a20 2020 2020  >.    <tr>.     
+000a8820: 203c 7468 3e2e 2e2e 3c2f 7468 3e0a 2020   <th>...</th>.  
+000a8830: 2020 2020 3c74 643e 2e2e 2e3c 2f74 643e      <td>...</td>
+000a8840: 0a20 2020 2020 203c 7464 3e2e 2e2e 3c2f  .      <td>...</
+000a8850: 7464 3e0a 2020 2020 2020 3c74 643e 2e2e  td>.      <td>..
+000a8860: 2e3c 2f74 643e 0a20 2020 2020 203c 7464  .</td>.      <td
+000a8870: 3e2e 2e2e 3c2f 7464 3e0a 2020 2020 2020  >...</td>.      
+000a8880: 3c74 643e 2e2e 2e3c 2f74 643e 0a20 2020  <td>...</td>.   
+000a8890: 2020 203c 7464 3e2e 2e2e 3c2f 7464 3e0a     <td>...</td>.
+000a88a0: 2020 2020 2020 3c74 643e 2e2e 2e3c 2f74        <td>...</t
+000a88b0: 643e 0a20 2020 2020 203c 7464 3e2e 2e2e  d>.      <td>...
+000a88c0: 3c2f 7464 3e0a 2020 2020 2020 3c74 643e  </td>.      <td>
+000a88d0: 2e2e 2e3c 2f74 643e 0a20 2020 2020 203c  ...</td>.      <
+000a88e0: 7464 3e2e 2e2e 3c2f 7464 3e0a 2020 2020  td>...</td>.    
+000a88f0: 3c2f 7472 3e0a 2020 2020 3c74 723e 0a20  </tr>.    <tr>. 
+000a8900: 2020 2020 203c 7468 3e34 3935 3c2f 7468       <th>495</th
+000a8910: 3e0a 2020 2020 2020 3c74 643e 3131 3c2f  >.      <td>11</
+000a8920: 7464 3e0a 2020 2020 2020 3c74 643e 3430  td>.      <td>40
+000a8930: 2e37 3633 3838 3835 3731 3131 3739 202d  .7638885711179 -
+000a8940: 3734 2e30 3233 3338 3231 3830 3833 3532  74.0233821808352
+000a8950: 3c2f 7464 3e0a 2020 2020 2020 3c74 643e  </td>.      <td>
+000a8960: 3133 3835 3c2f 7464 3e0a 2020 2020 2020  1385</td>.      
+000a8970: 3c74 643e 5361 7475 7264 6179 3c2f 7464  <td>Saturday</td
+000a8980: 3e0a 2020 2020 2020 3c74 643e 2d31 2e30  >.      <td>-1.0
+000a8990: 3c2f 7464 3e0a 2020 2020 2020 3c74 643e  </td>.      <td>
+000a89a0: 2d31 3c2f 7464 3e0a 2020 2020 2020 3c74  -1</td>.      <t
+000a89b0: 643e 436c 6f75 6473 3c2f 7464 3e0a 2020  d>Clouds</td>.  
+000a89c0: 2020 2020 3c74 643e 5472 6176 656c 2026      <td>Travel &
+000a89d0: 616d 703b 2054 7261 6e73 706f 7274 3c2f  amp; Transport</
+000a89e0: 7464 3e0a 2020 2020 2020 3c74 643e 426f  td>.      <td>Bo
+000a89f0: 7264 6572 2043 726f 7373 696e 673c 2f74  rder Crossing</t
+000a8a00: 643e 0a20 2020 2020 203c 7464 3e43 333c  d>.      <td>C3<
+000a8a10: 2f74 643e 0a20 2020 203c 2f74 723e 0a20  /td>.    </tr>. 
+000a8a20: 2020 203c 7472 3e0a 2020 2020 2020 3c74     <tr>.      <t
+000a8a30: 683e 3439 363c 2f74 683e 0a20 2020 2020  h>496</th>.     
+000a8a40: 203c 7464 3e31 313c 2f74 643e 0a20 2020   <td>11</td>.   
+000a8a50: 2020 203c 7464 3e34 302e 3638 3931 3434     <td>40.689144
+000a8a60: 3133 3435 3231 3520 2d37 332e 3933 3033  1345215 -73.9303
+000a8a70: 3230 3733 3937 3436 313c 2f74 643e 0a20  207397461</td>. 
+000a8a80: 2020 2020 203c 7464 3e33 3739 3c2f 7464       <td>379</td
+000a8a90: 3e0a 2020 2020 2020 3c74 643e 5375 6e64  >.      <td>Sund
+000a8aa0: 6179 3c2f 7464 3e0a 2020 2020 2020 3c74  ay</td>.      <t
+000a8ab0: 643e 2d31 2e30 3c2f 7464 3e0a 2020 2020  d>-1.0</td>.    
+000a8ac0: 2020 3c74 643e 313c 2f74 643e 0a20 2020    <td>1</td>.   
+000a8ad0: 2020 203c 7464 3e43 6c6f 7564 733c 2f74     <td>Clouds</t
+000a8ae0: 643e 0a20 2020 2020 203c 7464 3e46 6f6f  d>.      <td>Foo
+000a8af0: 643c 2f74 643e 0a20 2020 2020 203c 7464  d</td>.      <td
+000a8b00: 3e44 656c 6920 2f20 426f 6465 6761 3c2f  >Deli / Bodega</
+000a8b10: 7464 3e0a 2020 2020 2020 3c74 643e 4333  td>.      <td>C3
+000a8b20: 3c2f 7464 3e0a 2020 2020 3c2f 7472 3e0a  </td>.    </tr>.
+000a8b30: 2020 2020 3c74 723e 0a20 2020 2020 203c      <tr>.      <
+000a8b40: 7468 3e34 3937 3c2f 7468 3e0a 2020 2020  th>497</th>.    
+000a8b50: 2020 3c74 643e 3131 3c2f 7464 3e0a 2020    <td>11</td>.  
+000a8b60: 2020 2020 3c74 643e 3430 2e37 3730 3437      <td>40.77047
+000a8b70: 3033 3530 3030 3030 202d 3734 2e30 3238  03500000 -74.028
+000a8b80: 3138 3331 3430 3030 3030 3c2f 7464 3e0a  1831400000</td>.
+000a8b90: 2020 2020 2020 3c74 643e 3534 373c 2f74        <td>547</t
+000a8ba0: 643e 0a20 2020 2020 203c 7464 3e53 756e  d>.      <td>Sun
+000a8bb0: 6461 793c 2f74 643e 0a20 2020 2020 203c  day</td>.      <
+000a8bc0: 7464 3e2d 312e 303c 2f74 643e 0a20 2020  td>-1.0</td>.   
+000a8bd0: 2020 203c 7464 3e2d 313c 2f74 643e 0a20     <td>-1</td>. 
+000a8be0: 2020 2020 203c 7464 3e43 6c65 6172 3c2f       <td>Clear</
+000a8bf0: 7464 3e0a 2020 2020 2020 3c74 643e 5072  td>.      <td>Pr
+000a8c00: 6f66 6573 7369 6f6e 616c 2026 616d 703b  ofessional &amp;
+000a8c10: 204f 7468 6572 2050 6c61 6365 733c 2f74   Other Places</t
+000a8c20: 643e 0a20 2020 2020 203c 7464 3e50 6f73  d>.      <td>Pos
+000a8c30: 7420 4f66 6669 6365 3c2f 7464 3e0a 2020  t Office</td>.  
+000a8c40: 2020 2020 3c74 643e 4333 3c2f 7464 3e0a      <td>C3</td>.
+000a8c50: 2020 2020 3c2f 7472 3e0a 2020 2020 3c74      </tr>.    <t
+000a8c60: 723e 0a20 2020 2020 203c 7468 3e34 3938  r>.      <th>498
+000a8c70: 3c2f 7468 3e0a 2020 2020 2020 3c74 643e  </th>.      <td>
+000a8c80: 3131 3c2f 7464 3e0a 2020 2020 2020 3c74  11</td>.      <t
+000a8c90: 643e 3430 2e37 3737 3437 3733 3932 3230  d>40.77747739220
+000a8ca0: 3837 202d 3733 2e38 3134 3637 3235 3735  87 -73.814672575
+000a8cb0: 3536 3433 3c2f 7464 3e0a 2020 2020 2020  5643</td>.      
+000a8cc0: 3c74 643e 3738 333c 2f74 643e 0a20 2020  <td>783</td>.   
+000a8cd0: 2020 203c 7464 3e53 756e 6461 793c 2f74     <td>Sunday</t
+000a8ce0: 643e 0a20 2020 2020 203c 7464 3e2d 312e  d>.      <td>-1.
+000a8cf0: 303c 2f74 643e 0a20 2020 2020 203c 7464  0</td>.      <td
+000a8d00: 3e2d 313c 2f74 643e 0a20 2020 2020 203c  >-1</td>.      <
+000a8d10: 7464 3e43 6c65 6172 3c2f 7464 3e0a 2020  td>Clear</td>.  
+000a8d20: 2020 2020 3c74 643e 5368 6f70 2026 616d      <td>Shop &am
+000a8d30: 703b 2053 6572 7669 6365 3c2f 7464 3e0a  p; Service</td>.
+000a8d40: 2020 2020 2020 3c74 643e 4361 6e64 7920        <td>Candy 
+000a8d50: 5374 6f72 653c 2f74 643e 0a20 2020 2020  Store</td>.     
+000a8d60: 203c 7464 3e43 333c 2f74 643e 0a20 2020   <td>C3</td>.   
+000a8d70: 203c 2f74 723e 0a20 2020 203c 7472 3e0a   </tr>.    <tr>.
+000a8d80: 2020 2020 2020 3c74 683e 3439 393c 2f74        <th>499</t
+000a8d90: 683e 0a20 2020 2020 203c 7464 3e31 313c  h>.      <td>11<
+000a8da0: 2f74 643e 0a20 2020 2020 203c 7464 3e34  /td>.      <td>4
+000a8db0: 302e 3833 3331 3635 3230 3036 3232 3420  0.8331652006224 
+000a8dc0: 2d37 332e 3934 3138 3630 3334 3237 3639  -73.941860342769
+000a8dd0: 323c 2f74 643e 0a20 2020 2020 203c 7464  2</td>.      <td
+000a8de0: 3e31 3033 333c 2f74 643e 0a20 2020 2020  >1033</td>.     
+000a8df0: 203c 7464 3e53 756e 6461 793c 2f74 643e   <td>Sunday</td>
+000a8e00: 0a20 2020 2020 203c 7464 3e2d 312e 303c  .      <td>-1.0<
+000a8e10: 2f74 643e 0a20 2020 2020 203c 7464 3e2d  /td>.      <td>-
+000a8e20: 313c 2f74 643e 0a20 2020 2020 203c 7464  1</td>.      <td
+000a8e30: 3e43 6c6f 7564 733c 2f74 643e 0a20 2020  >Clouds</td>.   
+000a8e40: 2020 203c 7464 3e52 6573 6964 656e 6365     <td>Residence
+000a8e50: 3c2f 7464 3e0a 2020 2020 2020 3c74 643e  </td>.      <td>
+000a8e60: 486f 6d65 2028 7072 6976 6174 6529 3c2f  Home (private)</
+000a8e70: 7464 3e0a 2020 2020 2020 3c74 643e 4333  td>.      <td>C3
+000a8e80: 3c2f 7464 3e0a 2020 2020 3c2f 7472 3e0a  </td>.    </tr>.
+000a8e90: 2020 3c2f 7462 6f64 793e 0a3c 2f74 6162    </tbody>.</tab
+000a8ea0: 6c65 3e0a 3c70 3e35 3030 2072 6f77 7320  le>.<p>500 rows 
+000a8eb0: c397 2031 3020 636f 6c75 6d6e 733c 2f70  .. 10 columns</p
+000a8ec0: 3e0a 3c2f 6469 763e 0a3c 2f64 6976 3e0a  >.</div>.</div>.
+000a8ed0: 0a3c 2f64 6976 3e0a 0a3c 2f64 6976 3e0a  .</div>..</div>.
+000a8ee0: 0a3c 2f64 6976 3e0a 0a3c 2f64 6976 3e0a  .</div>..</div>.
+000a8ef0: 3c64 6976 2063 6c61 7373 3d22 6a70 2d43  <div class="jp-C
+000a8f00: 656c 6c20 6a70 2d4d 6172 6b64 6f77 6e43  ell jp-MarkdownC
+000a8f10: 656c 6c20 6a70 2d4e 6f74 6562 6f6f 6b2d  ell jp-Notebook-
+000a8f20: 6365 6c6c 223e 0a3c 6469 7620 636c 6173  cell">.<div clas
+000a8f30: 733d 226a 702d 4365 6c6c 2d69 6e70 7574  s="jp-Cell-input
+000a8f40: 5772 6170 7065 7222 3e0a 3c64 6976 2063  Wrapper">.<div c
+000a8f50: 6c61 7373 3d22 6a70 2d43 6f6c 6c61 7073  lass="jp-Collaps
+000a8f60: 6572 206a 702d 496e 7075 7443 6f6c 6c61  er jp-InputColla
+000a8f70: 7073 6572 206a 702d 4365 6c6c 2d69 6e70  pser jp-Cell-inp
+000a8f80: 7574 436f 6c6c 6170 7365 7222 3e0a 3c2f  utCollapser">.</
+000a8f90: 6469 763e 0a3c 6469 7620 636c 6173 733d  div>.<div class=
+000a8fa0: 226a 702d 496e 7075 7441 7265 6120 6a70  "jp-InputArea jp
+000a8fb0: 2d43 656c 6c2d 696e 7075 7441 7265 6122  -Cell-inputArea"
+000a8fc0: 3e3c 6469 7620 636c 6173 733d 226a 702d  ><div class="jp-
+000a8fd0: 496e 7075 7450 726f 6d70 7420 6a70 2d49  InputPrompt jp-I
+000a8fe0: 6e70 7574 4172 6561 2d70 726f 6d70 7422  nputArea-prompt"
+000a8ff0: 3e0a 3c2f 6469 763e 3c64 6976 2063 6c61  >.</div><div cla
+000a9000: 7373 3d22 6a70 2d52 656e 6465 7265 6448  ss="jp-RenderedH
+000a9010: 544d 4c43 6f6d 6d6f 6e20 6a70 2d52 656e  TMLCommon jp-Ren
+000a9020: 6465 7265 644d 6172 6b64 6f77 6e20 6a70  deredMarkdown jp
+000a9030: 2d4d 6172 6b64 6f77 6e4f 7574 7075 7420  -MarkdownOutput 
+000a9040: 2220 6461 7461 2d6d 696d 652d 7479 7065  " data-mime-type
+000a9050: 3d22 7465 7874 2f6d 6172 6b64 6f77 6e22  ="text/markdown"
+000a9060: 3e0a 0a3c 7072 653e 3c63 6f64 653e 6229  >..<pre><code>b)
+000a9070: 2054 6f20 6765 6e65 7261 7465 2061 2073   To generate a s
+000a9080: 6574 206f 6620 7361 6d70 6c65 2064 6174  et of sample dat
+000a9090: 6173 6574 733a 0a0a 3c2f 636f 6465 3e3c  asets:..</code><
+000a90a0: 2f70 7265 3e0a 3c70 3e43 7265 6174 6573  /pre>.<p>Creates
+000a90b0: 2061 6e64 2073 6176 6520 6461 7461 7365   and save datase
+000a90c0: 7420 6669 6c65 7320 2869 6e63 6c75 6469  t files (includi
+000a90d0: 6e67 206d 6f76 656c 6574 7320 6a73 6f6e  ng movelets json
+000a90e0: 2064 6573 6372 6970 746f 7220 6669 6c65   descriptor file
+000a90f0: 292e 2047 656e 6572 6174 6573 2073 616d  ). Generates sam
+000a9100: 706c 6520 6461 7461 7365 7473 2069 6e20  ple datasets in 
+000a9110: 6120 696e 6372 6561 7369 6e67 206c 6f67  a increasing log
+000a9120: 2073 6361 6c65 2066 6f72 2065 6163 6820   scale for each 
+000a9130: 7061 7261 6d65 7465 722e 2049 7420 7573  parameter. It us
+000a9140: 6573 2074 6865 206d 6964 646c 6520 7661  es the middle va
+000a9150: 6c75 6520 666f 7220 7468 6520 6f74 6865  lue for the othe
+000a9160: 7220 636f 6e66 6967 7572 6174 696f 6e73  r configurations
+000a9170: 3c2f 703e 0a0a 3c2f 6469 763e 0a3c 2f64  </p>..</div>.</d
+000a9180: 6976 3e0a 3c2f 6469 763e 0a3c 2f64 6976  iv>.</div>.</div
+000a9190: 3e3c 6469 7620 636c 6173 733d 226a 702d  ><div class="jp-
+000a91a0: 4365 6c6c 206a 702d 436f 6465 4365 6c6c  Cell jp-CodeCell
+000a91b0: 206a 702d 4e6f 7465 626f 6f6b 2d63 656c   jp-Notebook-cel
+000a91c0: 6c20 2020 223e 0a3c 6469 7620 636c 6173  l   ">.<div clas
+000a91d0: 733d 226a 702d 4365 6c6c 2d69 6e70 7574  s="jp-Cell-input
+000a91e0: 5772 6170 7065 7222 3e0a 3c64 6976 2063  Wrapper">.<div c
+000a91f0: 6c61 7373 3d22 6a70 2d43 6f6c 6c61 7073  lass="jp-Collaps
+000a9200: 6572 206a 702d 496e 7075 7443 6f6c 6c61  er jp-InputColla
+000a9210: 7073 6572 206a 702d 4365 6c6c 2d69 6e70  pser jp-Cell-inp
+000a9220: 7574 436f 6c6c 6170 7365 7222 3e0a 3c2f  utCollapser">.</
+000a9230: 6469 763e 0a3c 6469 7620 636c 6173 733d  div>.<div class=
+000a9240: 226a 702d 496e 7075 7441 7265 6120 6a70  "jp-InputArea jp
+000a9250: 2d43 656c 6c2d 696e 7075 7441 7265 6122  -Cell-inputArea"
+000a9260: 3e0a 3c64 6976 2063 6c61 7373 3d22 6a70  >.<div class="jp
+000a9270: 2d49 6e70 7574 5072 6f6d 7074 206a 702d  -InputPrompt jp-
+000a9280: 496e 7075 7441 7265 612d 7072 6f6d 7074  InputArea-prompt
+000a9290: 223e 496e 266e 6273 703b 5b34 5d3a 3c2f  ">In&nbsp;[4]:</
+000a92a0: 6469 763e 0a3c 6469 7620 636c 6173 733d  div>.<div class=
+000a92b0: 226a 702d 436f 6465 4d69 7272 6f72 4564  "jp-CodeMirrorEd
+000a92c0: 6974 6f72 206a 702d 4564 6974 6f72 206a  itor jp-Editor j
+000a92d0: 702d 496e 7075 7441 7265 612d 6564 6974  p-InputArea-edit
+000a92e0: 6f72 2220 6461 7461 2d74 7970 653d 2269  or" data-type="i
+000a92f0: 6e6c 696e 6522 3e0a 2020 2020 203c 6469  nline">.     <di
+000a9300: 7620 636c 6173 733d 2243 6f64 654d 6972  v class="CodeMir
+000a9310: 726f 7220 636d 2d73 2d6a 7570 7974 6572  ror cm-s-jupyter
+000a9320: 223e 0a3c 6469 7620 636c 6173 733d 2220  ">.<div class=" 
+000a9330: 6869 6768 6c69 6768 7420 686c 2d69 7079  highlight hl-ipy
+000a9340: 7468 6f6e 3322 3e3c 7072 653e 3c73 7061  thon3"><pre><spa
+000a9350: 6e3e 3c2f 7370 616e 3e3c 7370 616e 2063  n></span><span c
+000a9360: 6c61 7373 3d22 6e22 3e64 6174 615f 7061  lass="n">data_pa
+000a9370: 7468 3c2f 7370 616e 3e20 3c73 7061 6e20  th</span> <span 
+000a9380: 636c 6173 733d 226f 223e 3d3c 2f73 7061  class="o">=</spa
+000a9390: 6e3e 203c 7370 616e 2063 6c61 7373 3d22  n> <span class="
+000a93a0: 7331 223e 2623 3339 3b6d 6174 6461 7461  s1">&#39;matdata
+000a93b0: 2f61 7373 6574 732f 7361 6d70 6c65 2f73  /assets/sample/s
+000a93c0: 616d 706c 6573 2623 3339 3b3c 2f73 7061  amples&#39;</spa
+000a93d0: 6e3e 0a0a 3c73 7061 6e20 636c 6173 733d  n>..<span class=
+000a93e0: 226e 223e 4e73 3c2f 7370 616e 3e3c 7370  "n">Ns</span><sp
+000a93f0: 616e 2063 6c61 7373 3d22 6f22 3e3d 3c2f  an class="o">=</
+000a9400: 7370 616e 3e3c 7370 616e 2063 6c61 7373  span><span class
+000a9410: 3d22 7022 3e5b 3c2f 7370 616e 3e3c 7370  ="p">[</span><sp
+000a9420: 616e 2063 6c61 7373 3d22 6d69 223e 3130  an class="mi">10
+000a9430: 303c 2f73 7061 6e3e 3c73 7061 6e20 636c  0</span><span cl
+000a9440: 6173 733d 2270 223e 2c3c 2f73 7061 6e3e  ass="p">,</span>
+000a9450: 203c 7370 616e 2063 6c61 7373 3d22 6d69   <span class="mi
+000a9460: 223e 333c 2f73 7061 6e3e 3c73 7061 6e20  ">3</span><span 
+000a9470: 636c 6173 733d 2270 223e 5d3c 2f73 7061  class="p">]</spa
+000a9480: 6e3e 2020 203c 7370 616e 2063 6c61 7373  n>   <span class
+000a9490: 3d22 6331 223e 2320 4d69 6e2e 206e 756d  ="c1"># Min. num
+000a94a0: 6265 7220 6f66 2074 7261 6a65 6374 6f72  ber of trajector
+000a94b0: 6965 733a 2031 3030 2c20 3320 7363 616c  ies: 100, 3 scal
+000a94c0: 6573 2028 6279 206c 6f67 2069 6e63 7265  es (by log incre
+000a94d0: 6d65 6e74 2920 203c 2f73 7061 6e3e 0a3c  ment)  </span>.<
+000a94e0: 7370 616e 2063 6c61 7373 3d22 6e22 3e4d  span class="n">M
+000a94f0: 733c 2f73 7061 6e3e 3c73 7061 6e20 636c  s</span><span cl
+000a9500: 6173 733d 226f 223e 3d3c 2f73 7061 6e3e  ass="o">=</span>
+000a9510: 3c73 7061 6e20 636c 6173 733d 2270 223e  <span class="p">
+000a9520: 5b3c 2f73 7061 6e3e 3c73 7061 6e20 636c  [</span><span cl
+000a9530: 6173 733d 226d 6922 3e31 303c 2f73 7061  ass="mi">10</spa
+000a9540: 6e3e 3c73 7061 6e20 636c 6173 733d 2270  n><span class="p
+000a9550: 223e 2c3c 2f73 7061 6e3e 2020 3c73 7061  ">,</span>  <spa
+000a9560: 6e20 636c 6173 733d 226d 6922 3e33 3c2f  n class="mi">3</
+000a9570: 7370 616e 3e3c 7370 616e 2063 6c61 7373  span><span class
+000a9580: 3d22 7022 3e5d 3c2f 7370 616e 3e20 2020  ="p">]</span>   
+000a9590: 3c73 7061 6e20 636c 6173 733d 2263 3122  <span class="c1"
+000a95a0: 3e23 204d 696e 2e20 6e75 6d62 6572 206f  ># Min. number o
+000a95b0: 6620 706f 696e 7473 3a20 3130 2c20 3320  f points: 10, 3 
+000a95c0: 7363 616c 6573 2028 6279 206c 6f67 2069  scales (by log i
+000a95d0: 6e63 7265 6d65 6e74 293c 2f73 7061 6e3e  ncrement)</span>
+000a95e0: 0a3c 7370 616e 2063 6c61 7373 3d22 6e22  .<span class="n"
+000a95f0: 3e4c 733c 2f73 7061 6e3e 3c73 7061 6e20  >Ls</span><span 
+000a9600: 636c 6173 733d 226f 223e 3d3c 2f73 7061  class="o">=</spa
+000a9610: 6e3e 3c73 7061 6e20 636c 6173 733d 2270  n><span class="p
+000a9620: 223e 5b3c 2f73 7061 6e3e 3c73 7061 6e20  ">[</span><span 
+000a9630: 636c 6173 733d 226d 6922 3e38 3c2f 7370  class="mi">8</sp
+000a9640: 616e 3e3c 7370 616e 2063 6c61 7373 3d22  an><span class="
+000a9650: 7022 3e2c 3c2f 7370 616e 3e20 2020 3c73  p">,</span>   <s
+000a9660: 7061 6e20 636c 6173 733d 226d 6922 3e33  pan class="mi">3
+000a9670: 3c2f 7370 616e 3e3c 7370 616e 2063 6c61  </span><span cla
+000a9680: 7373 3d22 7022 3e5d 3c2f 7370 616e 3e20  ss="p">]</span> 
+000a9690: 2020 3c73 7061 6e20 636c 6173 733d 2263    <span class="c
+000a96a0: 3122 3e23 204d 696e 2e20 6e75 6d62 6572  1"># Min. number
+000a96b0: 206f 6620 6174 7472 6962 7574 6573 3a20   of attributes: 
+000a96c0: 382c 2033 2073 6361 6c65 7320 2862 7920  8, 3 scales (by 
+000a96d0: 6c6f 6720 696e 6372 656d 656e 7429 3c2f  log increment)</
+000a96e0: 7370 616e 3e0a 3c73 7061 6e20 636c 6173  span>.<span clas
+000a96f0: 733d 226e 223e 4373 3c2f 7370 616e 3e3c  s="n">Cs</span><
+000a9700: 7370 616e 2063 6c61 7373 3d22 6f22 3e3d  span class="o">=
+000a9710: 3c2f 7370 616e 3e3c 7370 616e 2063 6c61  </span><span cla
+000a9720: 7373 3d22 7022 3e5b 3c2f 7370 616e 3e3c  ss="p">[</span><
+000a9730: 7370 616e 2063 6c61 7373 3d22 6d69 223e  span class="mi">
+000a9740: 323c 2f73 7061 6e3e 3c73 7061 6e20 636c  2</span><span cl
+000a9750: 6173 733d 2270 223e 2c3c 2f73 7061 6e3e  ass="p">,</span>
+000a9760: 2020 203c 7370 616e 2063 6c61 7373 3d22     <span class="
+000a9770: 6d69 223e 333c 2f73 7061 6e3e 3c73 7061  mi">3</span><spa
+000a9780: 6e20 636c 6173 733d 2270 223e 5d3c 2f73  n class="p">]</s
+000a9790: 7061 6e3e 2020 203c 7370 616e 2063 6c61  pan>   <span cla
+000a97a0: 7373 3d22 6331 223e 2320 4d69 6e2e 206e  ss="c1"># Min. n
+000a97b0: 756d 6265 7220 6f66 206c 6162 656c 733a  umber of labels:
+000a97c0: 2032 2c20 3320 7363 616c 6573 2028 6279   2, 3 scales (by
+000a97d0: 206c 6f67 2069 6e63 7265 6d65 6e74 293c   log increment)<
+000a97e0: 2f73 7061 6e3e 0a0a 3c73 7061 6e20 636c  /span>..<span cl
+000a97f0: 6173 733d 226e 223e 7363 616c 6572 5361  ass="n">scalerSa
+000a9800: 6d70 6c65 7247 656e 6572 6174 6f72 3c2f  mplerGenerator</
+000a9810: 7370 616e 3e3c 7370 616e 2063 6c61 7373  span><span class
+000a9820: 3d22 7022 3e28 3c2f 7370 616e 3e3c 7370  ="p">(</span><sp
+000a9830: 616e 2063 6c61 7373 3d22 6e22 3e4e 733c  an class="n">Ns<
+000a9840: 2f73 7061 6e3e 3c73 7061 6e20 636c 6173  /span><span clas
+000a9850: 733d 2270 223e 2c3c 2f73 7061 6e3e 203c  s="p">,</span> <
+000a9860: 7370 616e 2063 6c61 7373 3d22 6e22 3e4d  span class="n">M
+000a9870: 733c 2f73 7061 6e3e 3c73 7061 6e20 636c  s</span><span cl
+000a9880: 6173 733d 2270 223e 2c3c 2f73 7061 6e3e  ass="p">,</span>
+000a9890: 203c 7370 616e 2063 6c61 7373 3d22 6e22   <span class="n"
+000a98a0: 3e4c 733c 2f73 7061 6e3e 3c73 7061 6e20  >Ls</span><span 
+000a98b0: 636c 6173 733d 2270 223e 2c3c 2f73 7061  class="p">,</spa
+000a98c0: 6e3e 203c 7370 616e 2063 6c61 7373 3d22  n> <span class="
+000a98d0: 6e22 3e43 733c 2f73 7061 6e3e 3c73 7061  n">Cs</span><spa
+000a98e0: 6e20 636c 6173 733d 2270 223e 2c3c 2f73  n class="p">,</s
+000a98f0: 7061 6e3e 203c 7370 616e 2063 6c61 7373  pan> <span class
+000a9900: 3d22 6e22 3e73 6176 655f 746f 3c2f 7370  ="n">save_to</sp
+000a9910: 616e 3e3c 7370 616e 2063 6c61 7373 3d22  an><span class="
+000a9920: 6f22 3e3d 3c2f 7370 616e 3e3c 7370 616e  o">=</span><span
+000a9930: 2063 6c61 7373 3d22 6e22 3e64 6174 615f   class="n">data_
+000a9940: 7061 7468 3c2f 7370 616e 3e3c 7370 616e  path</span><span
+000a9950: 2063 6c61 7373 3d22 7022 3e29 3c2f 7370   class="p">)</sp
+000a9960: 616e 3e0a 3c2f 7072 653e 3c2f 6469 763e  an>.</pre></div>
+000a9970: 0a0a 2020 2020 203c 2f64 6976 3e0a 3c2f  ..     </div>.</
+000a9980: 6469 763e 0a3c 2f64 6976 3e0a 3c2f 6469  div>.</div>.</di
+000a9990: 763e 0a0a 3c64 6976 2063 6c61 7373 3d22  v>..<div class="
+000a99a0: 6a70 2d43 656c 6c2d 6f75 7470 7574 5772  jp-Cell-outputWr
+000a99b0: 6170 7065 7222 3e0a 3c64 6976 2063 6c61  apper">.<div cla
+000a99c0: 7373 3d22 6a70 2d43 6f6c 6c61 7073 6572  ss="jp-Collapser
+000a99d0: 206a 702d 4f75 7470 7574 436f 6c6c 6170   jp-OutputCollap
+000a99e0: 7365 7220 6a70 2d43 656c 6c2d 6f75 7470  ser jp-Cell-outp
+000a99f0: 7574 436f 6c6c 6170 7365 7222 3e0a 3c2f  utCollapser">.</
+000a9a00: 6469 763e 0a0a 0a3c 6469 7620 636c 6173  div>...<div clas
+000a9a10: 733d 226a 702d 4f75 7470 7574 4172 6561  s="jp-OutputArea
+000a9a20: 206a 702d 4365 6c6c 2d6f 7574 7075 7441   jp-Cell-outputA
+000a9a30: 7265 6122 3e0a 0a3c 6469 7620 636c 6173  rea">..<div clas
+000a9a40: 733d 226a 702d 4f75 7470 7574 4172 6561  s="jp-OutputArea
+000a9a50: 2d63 6869 6c64 223e 0a0a 2020 2020 0a20  -child">..    . 
+000a9a60: 2020 203c 6469 7620 636c 6173 733d 226a     <div class="j
+000a9a70: 702d 4f75 7470 7574 5072 6f6d 7074 206a  p-OutputPrompt j
+000a9a80: 702d 4f75 7470 7574 4172 6561 2d70 726f  p-OutputArea-pro
+000a9a90: 6d70 7422 3e3c 2f64 6976 3e0a 0a0a 0a0a  mpt"></div>.....
+000a9aa0: 3c64 6976 2063 6c61 7373 3d22 6a70 2d52  <div class="jp-R
+000a9ab0: 656e 6465 7265 6454 6578 7420 6a70 2d4f  enderedText jp-O
+000a9ac0: 7574 7075 7441 7265 612d 6f75 7470 7574  utputArea-output
+000a9ad0: 2022 2064 6174 612d 6d69 6d65 2d74 7970   " data-mime-typ
+000a9ae0: 653d 2274 6578 742f 706c 6169 6e22 3e0a  e="text/plain">.
+000a9af0: 3c70 7265 3e20 2030 257c 2020 2020 2020  <pre>  0%|      
+000a9b00: 2020 2020 7c20 302f 3132 205b 3030 3a30      | 0/12 [00:0
+000a9b10: 3026 6c74 3b3f 2c20 3f69 742f 735d 3c2f  0&lt;?, ?it/s]</
+000a9b20: 7072 653e 0a3c 2f64 6976 3e0a 0a3c 2f64  pre>.</div>..</d
+000a9b30: 6976 3e0a 0a3c 6469 7620 636c 6173 733d  iv>..<div class=
+000a9b40: 226a 702d 4f75 7470 7574 4172 6561 2d63  "jp-OutputArea-c
+000a9b50: 6869 6c64 223e 0a0a 2020 2020 0a20 2020  hild">..    .   
+000a9b60: 203c 6469 7620 636c 6173 733d 226a 702d   <div class="jp-
+000a9b70: 4f75 7470 7574 5072 6f6d 7074 206a 702d  OutputPrompt jp-
+000a9b80: 4f75 7470 7574 4172 6561 2d70 726f 6d70  OutputArea-promp
+000a9b90: 7422 3e3c 2f64 6976 3e0a 0a0a 3c64 6976  t"></div>...<div
+000a9ba0: 2063 6c61 7373 3d22 6a70 2d52 656e 6465   class="jp-Rende
+000a9bb0: 7265 6454 6578 7420 6a70 2d4f 7574 7075  redText jp-Outpu
+000a9bc0: 7441 7265 612d 6f75 7470 7574 2220 6461  tArea-output" da
+000a9bd0: 7461 2d6d 696d 652d 7479 7065 3d22 7465  ta-mime-type="te
+000a9be0: 7874 2f70 6c61 696e 223e 0a3c 7072 653e  xt/plain">.<pre>
+000a9bf0: 4e20 3a3a 2066 6978 2e20 7661 6c75 653a  N :: fix. value:
+000a9c00: 2009 2032 3030 2009 7363 616c 653a 0920   . 200 .scale:. 
+000a9c10: 5b31 3030 2c20 3230 302c 2034 3030 5d0a  [100, 200, 400].
+000a9c20: 4d20 3a3a 2066 6978 2e20 7661 6c75 653a  M :: fix. value:
+000a9c30: 2009 2032 3020 0973 6361 6c65 3a09 205b   . 20 .scale:. [
+000a9c40: 3130 2c20 3230 2c20 3430 5d0a 4c20 3a3a  10, 20, 40].L ::
+000a9c50: 2066 6978 2e20 7661 6c75 653a 2009 2038   fix. value: . 8
+000a9c60: 2009 7363 616c 653a 0920 5b38 2c20 3136   .scale:. [8, 16
+000a9c70: 2c20 3332 5d0a 4320 3a3a 2066 6978 2e20  , 32].C :: fix. 
+000a9c80: 7661 6c75 653a 2009 2034 2009 7363 616c  value: . 4 .scal
+000a9c90: 653a 0920 5b32 2c20 342c 2038 5d0a 5772  e:. [2, 4, 8].Wr
+000a9ca0: 6974 696e 6720 2d20 4353 5620 7c0a 5772  iting - CSV |.Wr
+000a9cb0: 6974 696e 6720 2d20 4353 5620 7c0a 5772  iting - CSV |.Wr
+000a9cc0: 6974 696e 6720 2d20 4353 5620 7c0a 5772  iting - CSV |.Wr
+000a9cd0: 6974 696e 6720 2d20 4353 5620 7c0a 5772  iting - CSV |.Wr
+000a9ce0: 6974 696e 6720 2d20 4353 5620 7c0a 5772  iting - CSV |.Wr
+000a9cf0: 6974 696e 6720 2d20 4353 5620 7c0a 5772  iting - CSV |.Wr
+000a9d00: 6974 696e 6720 2d20 4353 5620 7c0a 5772  iting - CSV |.Wr
+000a9d10: 6974 696e 6720 2d20 4353 5620 7c0a 5772  iting - CSV |.Wr
+000a9d20: 6974 696e 6720 2d20 4353 5620 7c0a 3c2f  iting - CSV |.</
+000a9d30: 7072 653e 0a3c 2f64 6976 3e0a 3c2f 6469  pre>.</div>.</di
+000a9d40: 763e 0a0a 3c2f 6469 763e 0a0a 3c2f 6469  v>..</div>..</di
+000a9d50: 763e 0a0a 3c2f 6469 763e 0a3c 6469 7620  v>..</div>.<div 
+000a9d60: 636c 6173 733d 226a 702d 4365 6c6c 206a  class="jp-Cell j
+000a9d70: 702d 4d61 726b 646f 776e 4365 6c6c 206a  p-MarkdownCell j
+000a9d80: 702d 4e6f 7465 626f 6f6b 2d63 656c 6c22  p-Notebook-cell"
+000a9d90: 3e0a 3c64 6976 2063 6c61 7373 3d22 6a70  >.<div class="jp
+000a9da0: 2d43 656c 6c2d 696e 7075 7457 7261 7070  -Cell-inputWrapp
+000a9db0: 6572 223e 0a3c 6469 7620 636c 6173 733d  er">.<div class=
+000a9dc0: 226a 702d 436f 6c6c 6170 7365 7220 6a70  "jp-Collapser jp
+000a9dd0: 2d49 6e70 7574 436f 6c6c 6170 7365 7220  -InputCollapser 
+000a9de0: 6a70 2d43 656c 6c2d 696e 7075 7443 6f6c  jp-Cell-inputCol
+000a9df0: 6c61 7073 6572 223e 0a3c 2f64 6976 3e0a  lapser">.</div>.
+000a9e00: 3c64 6976 2063 6c61 7373 3d22 6a70 2d49  <div class="jp-I
+000a9e10: 6e70 7574 4172 6561 206a 702d 4365 6c6c  nputArea jp-Cell
+000a9e20: 2d69 6e70 7574 4172 6561 223e 3c64 6976  -inputArea"><div
+000a9e30: 2063 6c61 7373 3d22 6a70 2d49 6e70 7574   class="jp-Input
+000a9e40: 5072 6f6d 7074 206a 702d 496e 7075 7441  Prompt jp-InputA
+000a9e50: 7265 612d 7072 6f6d 7074 223e 0a3c 2f64  rea-prompt">.</d
+000a9e60: 6976 3e3c 6469 7620 636c 6173 733d 226a  iv><div class="j
+000a9e70: 702d 5265 6e64 6572 6564 4854 4d4c 436f  p-RenderedHTMLCo
+000a9e80: 6d6d 6f6e 206a 702d 5265 6e64 6572 6564  mmon jp-Rendered
+000a9e90: 4d61 726b 646f 776e 206a 702d 4d61 726b  Markdown jp-Mark
+000a9ea0: 646f 776e 4f75 7470 7574 2022 2064 6174  downOutput " dat
+000a9eb0: 612d 6d69 6d65 2d74 7970 653d 2274 6578  a-mime-type="tex
+000a9ec0: 742f 6d61 726b 646f 776e 223e 0a0a 3c70  t/markdown">..<p
+000a9ed0: 7265 3e3c 636f 6465 3e63 2920 546f 2067  re><code>c) To g
+000a9ee0: 656e 6572 6174 6520 6120 7261 6e64 6f6d  enerate a random
+000a9ef0: 2064 6174 6173 6574 2028 6465 6661 756c   dataset (defaul
+000a9f00: 7420 636f 6e66 6967 293a 3c2f 636f 6465  t config):</code
+000a9f10: 3e3c 2f70 7265 3e0a 0a3c 2f64 6976 3e0a  ></pre>..</div>.
+000a9f20: 3c2f 6469 763e 0a3c 2f64 6976 3e0a 3c2f  </div>.</div>.</
+000a9f30: 6469 763e 3c64 6976 2063 6c61 7373 3d22  div><div class="
+000a9f40: 6a70 2d43 656c 6c20 6a70 2d43 6f64 6543  jp-Cell jp-CodeC
+000a9f50: 656c 6c20 6a70 2d4e 6f74 6562 6f6f 6b2d  ell jp-Notebook-
+000a9f60: 6365 6c6c 2020 2022 3e0a 3c64 6976 2063  cell   ">.<div c
+000a9f70: 6c61 7373 3d22 6a70 2d43 656c 6c2d 696e  lass="jp-Cell-in
+000a9f80: 7075 7457 7261 7070 6572 223e 0a3c 6469  putWrapper">.<di
+000a9f90: 7620 636c 6173 733d 226a 702d 436f 6c6c  v class="jp-Coll
+000a9fa0: 6170 7365 7220 6a70 2d49 6e70 7574 436f  apser jp-InputCo
+000a9fb0: 6c6c 6170 7365 7220 6a70 2d43 656c 6c2d  llapser jp-Cell-
+000a9fc0: 696e 7075 7443 6f6c 6c61 7073 6572 223e  inputCollapser">
+000a9fd0: 0a3c 2f64 6976 3e0a 3c64 6976 2063 6c61  .</div>.<div cla
+000a9fe0: 7373 3d22 6a70 2d49 6e70 7574 4172 6561  ss="jp-InputArea
+000a9ff0: 206a 702d 4365 6c6c 2d69 6e70 7574 4172   jp-Cell-inputAr
+000aa000: 6561 223e 0a3c 6469 7620 636c 6173 733d  ea">.<div class=
+000aa010: 226a 702d 496e 7075 7450 726f 6d70 7420  "jp-InputPrompt 
+000aa020: 6a70 2d49 6e70 7574 4172 6561 2d70 726f  jp-InputArea-pro
+000aa030: 6d70 7422 3e49 6e26 6e62 7370 3b5b 355d  mpt">In&nbsp;[5]
+000aa040: 3a3c 2f64 6976 3e0a 3c64 6976 2063 6c61  :</div>.<div cla
+000aa050: 7373 3d22 6a70 2d43 6f64 654d 6972 726f  ss="jp-CodeMirro
+000aa060: 7245 6469 746f 7220 6a70 2d45 6469 746f  rEditor jp-Edito
+000aa070: 7220 6a70 2d49 6e70 7574 4172 6561 2d65  r jp-InputArea-e
+000aa080: 6469 746f 7222 2064 6174 612d 7479 7065  ditor" data-type
+000aa090: 3d22 696e 6c69 6e65 223e 0a20 2020 2020  ="inline">.     
+000aa0a0: 3c64 6976 2063 6c61 7373 3d22 436f 6465  <div class="Code
+000aa0b0: 4d69 7272 6f72 2063 6d2d 732d 6a75 7079  Mirror cm-s-jupy
+000aa0c0: 7465 7222 3e0a 3c64 6976 2063 6c61 7373  ter">.<div class
+000aa0d0: 3d22 2068 6967 686c 6967 6874 2068 6c2d  =" highlight hl-
+000aa0e0: 6970 7974 686f 6e33 223e 3c70 7265 3e3c  ipython3"><pre><
+000aa0f0: 7370 616e 3e3c 2f73 7061 6e3e 3c73 7061  span></span><spa
+000aa100: 6e20 636c 6173 733d 226e 223e 7261 6e64  n class="n">rand
+000aa110: 6f6d 4765 6e65 7261 746f 723c 2f73 7061  omGenerator</spa
+000aa120: 6e3e 3c73 7061 6e20 636c 6173 733d 2270  n><span class="p
+000aa130: 223e 2829 3c2f 7370 616e 3e0a 3c2f 7072  ">()</span>.</pr
+000aa140: 653e 3c2f 6469 763e 0a0a 2020 2020 203c  e></div>..     <
+000aa150: 2f64 6976 3e0a 3c2f 6469 763e 0a3c 2f64  /div>.</div>.</d
+000aa160: 6976 3e0a 3c2f 6469 763e 0a0a 3c64 6976  iv>.</div>..<div
+000aa170: 2063 6c61 7373 3d22 6a70 2d43 656c 6c2d   class="jp-Cell-
+000aa180: 6f75 7470 7574 5772 6170 7065 7222 3e0a  outputWrapper">.
+000aa190: 3c64 6976 2063 6c61 7373 3d22 6a70 2d43  <div class="jp-C
+000aa1a0: 6f6c 6c61 7073 6572 206a 702d 4f75 7470  ollapser jp-Outp
+000aa1b0: 7574 436f 6c6c 6170 7365 7220 6a70 2d43  utCollapser jp-C
+000aa1c0: 656c 6c2d 6f75 7470 7574 436f 6c6c 6170  ell-outputCollap
+000aa1d0: 7365 7222 3e0a 3c2f 6469 763e 0a0a 0a3c  ser">.</div>...<
+000aa1e0: 6469 7620 636c 6173 733d 226a 702d 4f75  div class="jp-Ou
+000aa1f0: 7470 7574 4172 6561 206a 702d 4365 6c6c  tputArea jp-Cell
+000aa200: 2d6f 7574 7075 7441 7265 6122 3e0a 0a3c  -outputArea">..<
+000aa210: 6469 7620 636c 6173 733d 226a 702d 4f75  div class="jp-Ou
+000aa220: 7470 7574 4172 6561 2d63 6869 6c64 223e  tputArea-child">
+000aa230: 0a0a 2020 2020 0a20 2020 203c 6469 7620  ..    .    <div 
+000aa240: 636c 6173 733d 226a 702d 4f75 7470 7574  class="jp-Output
+000aa250: 5072 6f6d 7074 206a 702d 4f75 7470 7574  Prompt jp-Output
+000aa260: 4172 6561 2d70 726f 6d70 7422 3e4f 7574  Area-prompt">Out
+000aa270: 5b35 5d3a 3c2f 6469 763e 0a0a 0a0a 3c64  [5]:</div>....<d
+000aa280: 6976 2063 6c61 7373 3d22 6a70 2d52 656e  iv class="jp-Ren
+000aa290: 6465 7265 6448 544d 4c43 6f6d 6d6f 6e20  deredHTMLCommon 
+000aa2a0: 6a70 2d52 656e 6465 7265 6448 544d 4c20  jp-RenderedHTML 
+000aa2b0: 6a70 2d4f 7574 7075 7441 7265 612d 6f75  jp-OutputArea-ou
+000aa2c0: 7470 7574 206a 702d 4f75 7470 7574 4172  tput jp-OutputAr
+000aa2d0: 6561 2d65 7865 6375 7465 5265 7375 6c74  ea-executeResult
+000aa2e0: 2220 6461 7461 2d6d 696d 652d 7479 7065  " data-mime-type
+000aa2f0: 3d22 7465 7874 2f68 746d 6c22 3e0a 3c64  ="text/html">.<d
+000aa300: 6976 3e0a 3c73 7479 6c65 2073 636f 7065  iv>.<style scope
+000aa310: 643e 0a20 2020 202e 6461 7461 6672 616d  d>.    .datafram
+000aa320: 6520 7462 6f64 7920 7472 2074 683a 6f6e  e tbody tr th:on
+000aa330: 6c79 2d6f 662d 7479 7065 207b 0a20 2020  ly-of-type {.   
+000aa340: 2020 2020 2076 6572 7469 6361 6c2d 616c       vertical-al
+000aa350: 6967 6e3a 206d 6964 646c 653b 0a20 2020  ign: middle;.   
+000aa360: 207d 0a0a 2020 2020 2e64 6174 6166 7261   }..    .datafra
+000aa370: 6d65 2074 626f 6479 2074 7220 7468 207b  me tbody tr th {
+000aa380: 0a20 2020 2020 2020 2076 6572 7469 6361  .        vertica
+000aa390: 6c2d 616c 6967 6e3a 2074 6f70 3b0a 2020  l-align: top;.  
+000aa3a0: 2020 7d0a 0a20 2020 202e 6461 7461 6672    }..    .datafr
+000aa3b0: 616d 6520 7468 6561 6420 7468 207b 0a20  ame thead th {. 
+000aa3c0: 2020 2020 2020 2074 6578 742d 616c 6967         text-alig
+000aa3d0: 6e3a 2072 6967 6874 3b0a 2020 2020 7d0a  n: right;.    }.
+000aa3e0: 3c2f 7374 796c 653e 0a3c 7461 626c 6520  </style>.<table 
+000aa3f0: 626f 7264 6572 3d22 3122 2063 6c61 7373  border="1" class
+000aa400: 3d22 6461 7461 6672 616d 6522 3e0a 2020  ="dataframe">.  
+000aa410: 3c74 6865 6164 3e0a 2020 2020 3c74 7220  <thead>.    <tr 
+000aa420: 7374 796c 653d 2274 6578 742d 616c 6967  style="text-alig
+000aa430: 6e3a 2072 6967 6874 3b22 3e0a 2020 2020  n: right;">.    
+000aa440: 2020 3c74 683e 3c2f 7468 3e0a 2020 2020    <th></th>.    
+000aa450: 2020 3c74 683e 7469 643c 2f74 683e 0a20    <th>tid</th>. 
+000aa460: 2020 2020 203c 7468 3e61 315f 7370 6163       <th>a1_spac
+000aa470: 653c 2f74 683e 0a20 2020 2020 203c 7468  e</th>.      <th
+000aa480: 3e61 325f 7469 6d65 3c2f 7468 3e0a 2020  >a2_time</th>.  
+000aa490: 2020 2020 3c74 683e 6133 5f6e 313c 2f74      <th>a3_n1</t
+000aa4a0: 683e 0a20 2020 2020 203c 7468 3e61 345f  h>.      <th>a4_
+000aa4b0: 6e32 3c2f 7468 3e0a 2020 2020 2020 3c74  n2</th>.      <t
+000aa4c0: 683e 6135 5f6e 6f6d 696e 616c 3c2f 7468  h>a5_nominal</th
+000aa4d0: 3e0a 2020 2020 2020 3c74 683e 6136 5f64  >.      <th>a6_d
+000aa4e0: 6179 3c2f 7468 3e0a 2020 2020 2020 3c74  ay</th>.      <t
+000aa4f0: 683e 6137 5f77 6561 7468 6572 3c2f 7468  h>a7_weather</th
+000aa500: 3e0a 2020 2020 2020 3c74 683e 6138 5f63  >.      <th>a8_c
+000aa510: 6174 6567 6f72 793c 2f74 683e 0a20 2020  ategory</th>.   
+000aa520: 2020 203c 7468 3e61 395f 7370 6163 653c     <th>a9_space<
+000aa530: 2f74 683e 0a20 2020 2020 203c 7468 3e61  /th>.      <th>a
+000aa540: 3130 5f74 696d 653c 2f74 683e 0a20 2020  10_time</th>.   
+000aa550: 2020 203c 7468 3e6c 6162 656c 3c2f 7468     <th>label</th
+000aa560: 3e0a 2020 2020 3c2f 7472 3e0a 2020 3c2f  >.    </tr>.  </
+000aa570: 7468 6561 643e 0a20 203c 7462 6f64 793e  thead>.  <tbody>
+000aa580: 0a20 2020 203c 7472 3e0a 2020 2020 2020  .    <tr>.      
+000aa590: 3c74 683e 303c 2f74 683e 0a20 2020 2020  <th>0</th>.     
+000aa5a0: 203c 7464 3e31 3c2f 7464 3e0a 2020 2020   <td>1</td>.    
+000aa5b0: 2020 3c74 643e 3133 342e 3520 3834 382e    <td>134.5 848.
+000aa5c0: 3238 3c2f 7464 3e0a 2020 2020 2020 3c74  28</td>.      <t
+000aa5d0: 643e 3131 343c 2f74 643e 0a20 2020 2020  d>114</td>.     
+000aa5e0: 203c 7464 3e39 3439 3c2f 7464 3e0a 2020   <td>949</td>.  
+000aa5f0: 2020 2020 3c74 643e 3937 362e 3938 3c2f      <td>976.98</
+000aa600: 7464 3e0a 2020 2020 2020 3c74 643e 5058  td>.      <td>PX
+000aa610: 3c2f 7464 3e0a 2020 2020 2020 3c74 643e  </td>.      <td>
+000aa620: 5475 6573 6461 793c 2f74 643e 0a20 2020  Tuesday</td>.   
+000aa630: 2020 203c 7464 3e43 6c6f 7564 733c 2f74     <td>Clouds</t
+000aa640: 643e 0a20 2020 2020 203c 7464 3e4f 7574  d>.      <td>Out
+000aa650: 646f 6f72 7320 2661 6d70 3b20 5265 6372  doors &amp; Recr
+000aa660: 6561 7469 6f6e 3c2f 7464 3e0a 2020 2020  eation</td>.    
+000aa670: 2020 3c74 643e 3130 312e 3034 2037 3738    <td>101.04 778
+000aa680: 2e35 323c 2f74 643e 0a20 2020 2020 203c  .52</td>.      <
+000aa690: 7464 3e31 3131 343c 2f74 643e 0a20 2020  td>1114</td>.   
+000aa6a0: 2020 203c 7464 3e43 313c 2f74 643e 0a20     <td>C1</td>. 
+000aa6b0: 2020 203c 2f74 723e 0a20 2020 203c 7472     </tr>.    <tr
+000aa6c0: 3e0a 2020 2020 2020 3c74 683e 313c 2f74  >.      <th>1</t
+000aa6d0: 683e 0a20 2020 2020 203c 7464 3e31 3c2f  h>.      <td>1</
+000aa6e0: 7464 3e0a 2020 2020 2020 3c74 643e 3736  td>.      <td>76
+000aa6f0: 342e 3534 2032 3535 2e33 323c 2f74 643e  4.54 255.32</td>
+000aa700: 0a20 2020 2020 203c 7464 3e39 3835 3c2f  .      <td>985</
+000aa710: 7464 3e0a 2020 2020 2020 3c74 643e 2d36  td>.      <td>-6
+000aa720: 3536 3c2f 7464 3e0a 2020 2020 2020 3c74  56</td>.      <t
+000aa730: 643e 3633 302e 3737 3c2f 7464 3e0a 2020  d>630.77</td>.  
+000aa740: 2020 2020 3c74 643e 484b 3c2f 7464 3e0a      <td>HK</td>.
+000aa750: 2020 2020 2020 3c74 643e 5361 7475 7264        <td>Saturd
+000aa760: 6179 3c2f 7464 3e0a 2020 2020 2020 3c74  ay</td>.      <t
+000aa770: 643e 436c 6f75 6473 3c2f 7464 3e0a 2020  d>Clouds</td>.  
+000aa780: 2020 2020 3c74 643e 5368 6f70 2026 616d      <td>Shop &am
+000aa790: 703b 2053 6572 7669 6365 3c2f 7464 3e0a  p; Service</td>.
+000aa7a0: 2020 2020 2020 3c74 643e 3332 382e 3432        <td>328.42
+000aa7b0: 2035 3039 2e37 383c 2f74 643e 0a20 2020   509.78</td>.   
+000aa7c0: 2020 203c 7464 3e38 333c 2f74 643e 0a20     <td>83</td>. 
+000aa7d0: 2020 2020 203c 7464 3e43 313c 2f74 643e       <td>C1</td>
+000aa7e0: 0a20 2020 203c 2f74 723e 0a20 2020 203c  .    </tr>.    <
+000aa7f0: 7472 3e0a 2020 2020 2020 3c74 683e 323c  tr>.      <th>2<
+000aa800: 2f74 683e 0a20 2020 2020 203c 7464 3e31  /th>.      <td>1
+000aa810: 3c2f 7464 3e0a 2020 2020 2020 3c74 643e  </td>.      <td>
+000aa820: 3439 352e 3933 2034 3439 2e39 343c 2f74  495.93 449.94</t
+000aa830: 643e 0a20 2020 2020 203c 7464 3e37 3436  d>.      <td>746
+000aa840: 3c2f 7464 3e0a 2020 2020 2020 3c74 643e  </td>.      <td>
+000aa850: 3334 343c 2f74 643e 0a20 2020 2020 203c  344</td>.      <
+000aa860: 7464 3e36 3935 2e30 353c 2f74 643e 0a20  td>695.05</td>. 
+000aa870: 2020 2020 203c 7464 3e4a 4d3c 2f74 643e       <td>JM</td>
+000aa880: 0a20 2020 2020 203c 7464 3e53 6174 7572  .      <td>Satur
+000aa890: 6461 793c 2f74 643e 0a20 2020 2020 203c  day</td>.      <
+000aa8a0: 7464 3e52 6169 6e3c 2f74 643e 0a20 2020  td>Rain</td>.   
+000aa8b0: 2020 203c 7464 3e54 7261 7665 6c20 2661     <td>Travel &a
+000aa8c0: 6d70 3b20 5472 616e 7370 6f72 743c 2f74  mp; Transport</t
+000aa8d0: 643e 0a20 2020 2020 203c 7464 3e36 3635  d>.      <td>665
+000aa8e0: 2e39 3120 3137 392e 3735 3c2f 7464 3e0a  .91 179.75</td>.
+000aa8f0: 2020 2020 2020 3c74 643e 3130 3733 3c2f        <td>1073</
+000aa900: 7464 3e0a 2020 2020 2020 3c74 643e 4331  td>.      <td>C1
+000aa910: 3c2f 7464 3e0a 2020 2020 3c2f 7472 3e0a  </td>.    </tr>.
+000aa920: 2020 2020 3c74 723e 0a20 2020 2020 203c      <tr>.      <
+000aa930: 7468 3e33 3c2f 7468 3e0a 2020 2020 2020  th>3</th>.      
+000aa940: 3c74 643e 313c 2f74 643e 0a20 2020 2020  <td>1</td>.     
+000aa950: 203c 7464 3e36 3532 2e32 3420 3738 392e   <td>652.24 789.
+000aa960: 3531 3c2f 7464 3e0a 2020 2020 2020 3c74  51</td>.      <t
+000aa970: 643e 3131 3637 3c2f 7464 3e0a 2020 2020  d>1167</td>.    
+000aa980: 2020 3c74 643e 2d34 3432 3c2f 7464 3e0a    <td>-442</td>.
+000aa990: 2020 2020 2020 3c74 643e 3435 302e 3835        <td>450.85
+000aa9a0: 3c2f 7464 3e0a 2020 2020 2020 3c74 643e  </td>.      <td>
+000aa9b0: 5a4f 3c2f 7464 3e0a 2020 2020 2020 3c74  ZO</td>.      <t
+000aa9c0: 643e 5765 646e 6573 6461 793c 2f74 643e  d>Wednesday</td>
+000aa9d0: 0a20 2020 2020 203c 7464 3e55 6e6b 6e6f  .      <td>Unkno
+000aa9e0: 776e 3c2f 7464 3e0a 2020 2020 2020 3c74  wn</td>.      <t
+000aa9f0: 643e 4e69 6768 746c 6966 6520 5370 6f74  d>Nightlife Spot
+000aaa00: 3c2f 7464 3e0a 2020 2020 2020 3c74 643e  </td>.      <td>
+000aaa10: 3134 392e 3731 2031 3431 2e36 383c 2f74  149.71 141.68</t
+000aaa20: 643e 0a20 2020 2020 203c 7464 3e31 3835  d>.      <td>185
+000aaa30: 3c2f 7464 3e0a 2020 2020 2020 3c74 643e  </td>.      <td>
+000aaa40: 4331 3c2f 7464 3e0a 2020 2020 3c2f 7472  C1</td>.    </tr
+000aaa50: 3e0a 2020 2020 3c74 723e 0a20 2020 2020  >.    <tr>.     
+000aaa60: 203c 7468 3e34 3c2f 7468 3e0a 2020 2020   <th>4</th>.    
+000aaa70: 2020 3c74 643e 313c 2f74 643e 0a20 2020    <td>1</td>.   
+000aaa80: 2020 203c 7464 3e39 332e 3935 2032 382e     <td>93.95 28.
+000aaa90: 3338 3c2f 7464 3e0a 2020 2020 2020 3c74  38</td>.      <t
+000aaaa0: 643e 3131 3335 3c2f 7464 3e0a 2020 2020  d>1135</td>.    
+000aaab0: 2020 3c74 643e 3332 373c 2f74 643e 0a20    <td>327</td>. 
+000aaac0: 2020 2020 203c 7464 3e35 3233 2e39 303c       <td>523.90<
+000aaad0: 2f74 643e 0a20 2020 2020 203c 7464 3e43  /td>.      <td>C
+000aaae0: 553c 2f74 643e 0a20 2020 2020 203c 7464  U</td>.      <td
+000aaaf0: 3e4d 6f6e 6461 793c 2f74 643e 0a20 2020  >Monday</td>.   
+000aab00: 2020 203c 7464 3e43 6c6f 7564 733c 2f74     <td>Clouds</t
+000aab10: 643e 0a20 2020 2020 203c 7464 3e50 726f  d>.      <td>Pro
+000aab20: 6665 7373 696f 6e61 6c20 2661 6d70 3b20  fessional &amp; 
+000aab30: 4f74 6865 7220 506c 6163 6573 3c2f 7464  Other Places</td
+000aab40: 3e0a 2020 2020 2020 3c74 643e 3836 362e  >.      <td>866.
+000aab50: 3431 2033 3035 2e39 333c 2f74 643e 0a20  41 305.93</td>. 
+000aab60: 2020 2020 203c 7464 3e35 3232 3c2f 7464       <td>522</td
+000aab70: 3e0a 2020 2020 2020 3c74 643e 4331 3c2f  >.      <td>C1</
+000aab80: 7464 3e0a 2020 2020 3c2f 7472 3e0a 2020  td>.    </tr>.  
+000aab90: 2020 3c74 723e 0a20 2020 2020 203c 7468    <tr>.      <th
+000aaba0: 3e2e 2e2e 3c2f 7468 3e0a 2020 2020 2020  >...</th>.      
+000aabb0: 3c74 643e 2e2e 2e3c 2f74 643e 0a20 2020  <td>...</td>.   
+000aabc0: 2020 203c 7464 3e2e 2e2e 3c2f 7464 3e0a     <td>...</td>.
+000aabd0: 2020 2020 2020 3c74 643e 2e2e 2e3c 2f74        <td>...</t
+000aabe0: 643e 0a20 2020 2020 203c 7464 3e2e 2e2e  d>.      <td>...
+000aabf0: 3c2f 7464 3e0a 2020 2020 2020 3c74 643e  </td>.      <td>
+000aac00: 2e2e 2e3c 2f74 643e 0a20 2020 2020 203c  ...</td>.      <
+000aac10: 7464 3e2e 2e2e 3c2f 7464 3e0a 2020 2020  td>...</td>.    
+000aac20: 2020 3c74 643e 2e2e 2e3c 2f74 643e 0a20    <td>...</td>. 
+000aac30: 2020 2020 203c 7464 3e2e 2e2e 3c2f 7464       <td>...</td
+000aac40: 3e0a 2020 2020 2020 3c74 643e 2e2e 2e3c  >.      <td>...<
+000aac50: 2f74 643e 0a20 2020 2020 203c 7464 3e2e  /td>.      <td>.
+000aac60: 2e2e 3c2f 7464 3e0a 2020 2020 2020 3c74  ..</td>.      <t
+000aac70: 643e 2e2e 2e3c 2f74 643e 0a20 2020 2020  d>...</td>.     
+000aac80: 203c 7464 3e2e 2e2e 3c2f 7464 3e0a 2020   <td>...</td>.  
+000aac90: 2020 3c2f 7472 3e0a 2020 2020 3c74 723e    </tr>.    <tr>
+000aaca0: 0a20 2020 2020 203c 7468 3e34 3935 3c2f  .      <th>495</
+000aacb0: 7468 3e0a 2020 2020 2020 3c74 643e 3130  th>.      <td>10
+000aacc0: 3c2f 7464 3e0a 2020 2020 2020 3c74 643e  </td>.      <td>
+000aacd0: 3634 372e 3936 2033 3030 2e35 3c2f 7464  647.96 300.5</td
+000aace0: 3e0a 2020 2020 2020 3c74 643e 3132 3035  >.      <td>1205
+000aacf0: 3c2f 7464 3e0a 2020 2020 2020 3c74 643e  </td>.      <td>
+000aad00: 3536 313c 2f74 643e 0a20 2020 2020 203c  561</td>.      <
+000aad10: 7464 3e38 3139 2e31 323c 2f74 643e 0a20  td>819.12</td>. 
+000aad20: 2020 2020 203c 7464 3e41 4352 3c2f 7464       <td>ACR</td
+000aad30: 3e0a 2020 2020 2020 3c74 643e 5361 7475  >.      <td>Satu
+000aad40: 7264 6179 3c2f 7464 3e0a 2020 2020 2020  rday</td>.      
+000aad50: 3c74 643e 5261 696e 3c2f 7464 3e0a 2020  <td>Rain</td>.  
+000aad60: 2020 2020 3c74 643e 4172 7473 2026 616d      <td>Arts &am
+000aad70: 703b 2045 6e74 6572 7461 696e 6d65 6e74  p; Entertainment
+000aad80: 3c2f 7464 3e0a 2020 2020 2020 3c74 643e  </td>.      <td>
+000aad90: 3531 352e 3936 2039 3535 2e36 363c 2f74  515.96 955.66</t
+000aada0: 643e 0a20 2020 2020 203c 7464 3e36 3334  d>.      <td>634
+000aadb0: 3c2f 7464 3e0a 2020 2020 2020 3c74 643e  </td>.      <td>
+000aadc0: 4331 303c 2f74 643e 0a20 2020 203c 2f74  C10</td>.    </t
+000aadd0: 723e 0a20 2020 203c 7472 3e0a 2020 2020  r>.    <tr>.    
+000aade0: 2020 3c74 683e 3439 363c 2f74 683e 0a20    <th>496</th>. 
+000aadf0: 2020 2020 203c 7464 3e31 303c 2f74 643e       <td>10</td>
+000aae00: 0a20 2020 2020 203c 7464 3e37 3739 2e32  .      <td>779.2
+000aae10: 3620 3933 332e 3631 3c2f 7464 3e0a 2020  6 933.61</td>.  
+000aae20: 2020 2020 3c74 643e 3438 353c 2f74 643e      <td>485</td>
+000aae30: 0a20 2020 2020 203c 7464 3e31 3231 3c2f  .      <td>121</
+000aae40: 7464 3e0a 2020 2020 2020 3c74 643e 3734  td>.      <td>74
+000aae50: 352e 3332 3c2f 7464 3e0a 2020 2020 2020  5.32</td>.      
+000aae60: 3c74 643e 4149 5a3c 2f74 643e 0a20 2020  <td>AIZ</td>.   
+000aae70: 2020 203c 7464 3e54 7565 7364 6179 3c2f     <td>Tuesday</
+000aae80: 7464 3e0a 2020 2020 2020 3c74 643e 5261  td>.      <td>Ra
+000aae90: 696e 3c2f 7464 3e0a 2020 2020 2020 3c74  in</td>.      <t
+000aaea0: 643e 4f75 7464 6f6f 7273 2026 616d 703b  d>Outdoors &amp;
+000aaeb0: 2052 6563 7265 6174 696f 6e3c 2f74 643e   Recreation</td>
+000aaec0: 0a20 2020 2020 203c 7464 3e33 3737 2e38  .      <td>377.8
+000aaed0: 3320 3236 332e 3133 3c2f 7464 3e0a 2020  3 263.13</td>.  
+000aaee0: 2020 2020 3c74 643e 3433 353c 2f74 643e      <td>435</td>
+000aaef0: 0a20 2020 2020 203c 7464 3e43 3130 3c2f  .      <td>C10</
+000aaf00: 7464 3e0a 2020 2020 3c2f 7472 3e0a 2020  td>.    </tr>.  
+000aaf10: 2020 3c74 723e 0a20 2020 2020 203c 7468    <tr>.      <th
+000aaf20: 3e34 3937 3c2f 7468 3e0a 2020 2020 2020  >497</th>.      
+000aaf30: 3c74 643e 3130 3c2f 7464 3e0a 2020 2020  <td>10</td>.    
+000aaf40: 2020 3c74 643e 3339 382e 3320 3534 352e    <td>398.3 545.
+000aaf50: 3139 3c2f 7464 3e0a 2020 2020 2020 3c74  19</td>.      <t
+000aaf60: 643e 3430 363c 2f74 643e 0a20 2020 2020  d>406</td>.     
+000aaf70: 203c 7464 3e2d 3234 383c 2f74 643e 0a20   <td>-248</td>. 
+000aaf80: 2020 2020 203c 7464 3e31 3830 2e38 393c       <td>180.89<
+000aaf90: 2f74 643e 0a20 2020 2020 203c 7464 3e59  /td>.      <td>Y
+000aafa0: 483c 2f74 643e 0a20 2020 2020 203c 7464  H</td>.      <td
+000aafb0: 3e4d 6f6e 6461 793c 2f74 643e 0a20 2020  >Monday</td>.   
+000aafc0: 2020 203c 7464 3e46 6f67 3c2f 7464 3e0a     <td>Fog</td>.
+000aafd0: 2020 2020 2020 3c74 643e 4576 656e 743c        <td>Event<
+000aafe0: 2f74 643e 0a20 2020 2020 203c 7464 3e34  /td>.      <td>4
+000aaff0: 3538 2e32 3720 3636 352e 3436 3c2f 7464  58.27 665.46</td
+000ab000: 3e0a 2020 2020 2020 3c74 643e 3837 343c  >.      <td>874<
+000ab010: 2f74 643e 0a20 2020 2020 203c 7464 3e43  /td>.      <td>C
+000ab020: 3130 3c2f 7464 3e0a 2020 2020 3c2f 7472  10</td>.    </tr
+000ab030: 3e0a 2020 2020 3c74 723e 0a20 2020 2020  >.    <tr>.     
+000ab040: 203c 7468 3e34 3938 3c2f 7468 3e0a 2020   <th>498</th>.  
+000ab050: 2020 2020 3c74 643e 3130 3c2f 7464 3e0a      <td>10</td>.
+000ab060: 2020 2020 2020 3c74 643e 3133 332e 3532        <td>133.52
+000ab070: 2036 3035 2e30 323c 2f74 643e 0a20 2020   605.02</td>.   
+000ab080: 2020 203c 7464 3e36 323c 2f74 643e 0a20     <td>62</td>. 
+000ab090: 2020 2020 203c 7464 3e2d 3438 353c 2f74       <td>-485</t
+000ab0a0: 643e 0a20 2020 2020 203c 7464 3e38 3930  d>.      <td>890
+000ab0b0: 2e34 323c 2f74 643e 0a20 2020 2020 203c  .42</td>.      <
+000ab0c0: 7464 3e44 493c 2f74 643e 0a20 2020 2020  td>DI</td>.     
+000ab0d0: 203c 7464 3e54 6875 7273 6461 793c 2f74   <td>Thursday</t
+000ab0e0: 643e 0a20 2020 2020 203c 7464 3e43 6c6f  d>.      <td>Clo
+000ab0f0: 7564 733c 2f74 643e 0a20 2020 2020 203c  uds</td>.      <
+000ab100: 7464 3e52 6573 6964 656e 6365 3c2f 7464  td>Residence</td
+000ab110: 3e0a 2020 2020 2020 3c74 643e 3236 332e  >.      <td>263.
+000ab120: 3933 2039 3434 2e38 3c2f 7464 3e0a 2020  93 944.8</td>.  
+000ab130: 2020 2020 3c74 643e 3131 3431 3c2f 7464      <td>1141</td
+000ab140: 3e0a 2020 2020 2020 3c74 643e 4331 303c  >.      <td>C10<
+000ab150: 2f74 643e 0a20 2020 203c 2f74 723e 0a20  /td>.    </tr>. 
+000ab160: 2020 203c 7472 3e0a 2020 2020 2020 3c74     <tr>.      <t
+000ab170: 683e 3439 393c 2f74 683e 0a20 2020 2020  h>499</th>.     
+000ab180: 203c 7464 3e31 303c 2f74 643e 0a20 2020   <td>10</td>.   
+000ab190: 2020 203c 7464 3e33 3837 2e34 3920 3130     <td>387.49 10
+000ab1a0: 362e 3132 3c2f 7464 3e0a 2020 2020 2020  6.12</td>.      
+000ab1b0: 3c74 643e 3433 353c 2f74 643e 0a20 2020  <td>435</td>.   
+000ab1c0: 2020 203c 7464 3e38 3337 3c2f 7464 3e0a     <td>837</td>.
+000ab1d0: 2020 2020 2020 3c74 643e 3339 382e 3133        <td>398.13
+000ab1e0: 3c2f 7464 3e0a 2020 2020 2020 3c74 643e  </td>.      <td>
+000ab1f0: 4143 4d3c 2f74 643e 0a20 2020 2020 203c  ACM</td>.      <
+000ab200: 7464 3e54 7565 7364 6179 3c2f 7464 3e0a  td>Tuesday</td>.
+000ab210: 2020 2020 2020 3c74 643e 5261 696e 3c2f        <td>Rain</
+000ab220: 7464 3e0a 2020 2020 2020 3c74 643e 5265  td>.      <td>Re
+000ab230: 7369 6465 6e63 653c 2f74 643e 0a20 2020  sidence</td>.   
+000ab240: 2020 203c 7464 3e39 3136 2e34 3620 3738     <td>916.46 78
+000ab250: 352e 3133 3c2f 7464 3e0a 2020 2020 2020  5.13</td>.      
+000ab260: 3c74 643e 3131 3938 3c2f 7464 3e0a 2020  <td>1198</td>.  
+000ab270: 2020 2020 3c74 643e 4331 303c 2f74 643e      <td>C10</td>
+000ab280: 0a20 2020 203c 2f74 723e 0a20 203c 2f74  .    </tr>.  </t
+000ab290: 626f 6479 3e0a 3c2f 7461 626c 653e 0a3c  body>.</table>.<
+000ab2a0: 703e 3530 3020 726f 7773 20c3 9720 3132  p>500 rows .. 12
+000ab2b0: 2063 6f6c 756d 6e73 3c2f 703e 0a3c 2f64   columns</p>.</d
+000ab2c0: 6976 3e0a 3c2f 6469 763e 0a0a 3c2f 6469  iv>.</div>..</di
+000ab2d0: 763e 0a0a 3c2f 6469 763e 0a0a 3c2f 6469  v>..</div>..</di
+000ab2e0: 763e 0a0a 3c2f 6469 763e 0a3c 6469 7620  v>..</div>.<div 
+000ab2f0: 636c 6173 733d 226a 702d 4365 6c6c 206a  class="jp-Cell j
+000ab300: 702d 4d61 726b 646f 776e 4365 6c6c 206a  p-MarkdownCell j
+000ab310: 702d 4e6f 7465 626f 6f6b 2d63 656c 6c22  p-Notebook-cell"
+000ab320: 3e0a 3c64 6976 2063 6c61 7373 3d22 6a70  >.<div class="jp
+000ab330: 2d43 656c 6c2d 696e 7075 7457 7261 7070  -Cell-inputWrapp
+000ab340: 6572 223e 0a3c 6469 7620 636c 6173 733d  er">.<div class=
+000ab350: 226a 702d 436f 6c6c 6170 7365 7220 6a70  "jp-Collapser jp
+000ab360: 2d49 6e70 7574 436f 6c6c 6170 7365 7220  -InputCollapser 
+000ab370: 6a70 2d43 656c 6c2d 696e 7075 7443 6f6c  jp-Cell-inputCol
+000ab380: 6c61 7073 6572 223e 0a3c 2f64 6976 3e0a  lapser">.</div>.
+000ab390: 3c64 6976 2063 6c61 7373 3d22 6a70 2d49  <div class="jp-I
+000ab3a0: 6e70 7574 4172 6561 206a 702d 4365 6c6c  nputArea jp-Cell
+000ab3b0: 2d69 6e70 7574 4172 6561 223e 3c64 6976  -inputArea"><div
+000ab3c0: 2063 6c61 7373 3d22 6a70 2d49 6e70 7574   class="jp-Input
+000ab3d0: 5072 6f6d 7074 206a 702d 496e 7075 7441  Prompt jp-InputA
+000ab3e0: 7265 612d 7072 6f6d 7074 223e 0a3c 2f64  rea-prompt">.</d
+000ab3f0: 6976 3e3c 6469 7620 636c 6173 733d 226a  iv><div class="j
+000ab400: 702d 5265 6e64 6572 6564 4854 4d4c 436f  p-RenderedHTMLCo
+000ab410: 6d6d 6f6e 206a 702d 5265 6e64 6572 6564  mmon jp-Rendered
+000ab420: 4d61 726b 646f 776e 206a 702d 4d61 726b  Markdown jp-Mark
+000ab430: 646f 776e 4f75 7470 7574 2022 2064 6174  downOutput " dat
+000ab440: 612d 6d69 6d65 2d74 7970 653d 2274 6578  a-mime-type="tex
+000ab450: 742f 6d61 726b 646f 776e 223e 0a3c 703e  t/markdown">.<p>
+000ab460: 546f 2073 7065 6369 6679 2074 6865 2073  To specify the s
+000ab470: 796e 7468 6574 6963 2072 616e 646f 6d20  ynthetic random 
+000ab480: 6461 7461 7365 7420 7061 7261 6d65 7465  dataset paramete
+000ab490: 7273 3a3c 2f70 3e0a 0a3c 2f64 6976 3e0a  rs:</p>..</div>.
+000ab4a0: 3c2f 6469 763e 0a3c 2f64 6976 3e0a 3c2f  </div>.</div>.</
+000ab4b0: 6469 763e 3c64 6976 2063 6c61 7373 3d22  div><div class="
+000ab4c0: 6a70 2d43 656c 6c20 6a70 2d43 6f64 6543  jp-Cell jp-CodeC
+000ab4d0: 656c 6c20 6a70 2d4e 6f74 6562 6f6f 6b2d  ell jp-Notebook-
+000ab4e0: 6365 6c6c 2020 2022 3e0a 3c64 6976 2063  cell   ">.<div c
+000ab4f0: 6c61 7373 3d22 6a70 2d43 656c 6c2d 696e  lass="jp-Cell-in
+000ab500: 7075 7457 7261 7070 6572 223e 0a3c 6469  putWrapper">.<di
+000ab510: 7620 636c 6173 733d 226a 702d 436f 6c6c  v class="jp-Coll
+000ab520: 6170 7365 7220 6a70 2d49 6e70 7574 436f  apser jp-InputCo
+000ab530: 6c6c 6170 7365 7220 6a70 2d43 656c 6c2d  llapser jp-Cell-
+000ab540: 696e 7075 7443 6f6c 6c61 7073 6572 223e  inputCollapser">
+000ab550: 0a3c 2f64 6976 3e0a 3c64 6976 2063 6c61  .</div>.<div cla
+000ab560: 7373 3d22 6a70 2d49 6e70 7574 4172 6561  ss="jp-InputArea
+000ab570: 206a 702d 4365 6c6c 2d69 6e70 7574 4172   jp-Cell-inputAr
+000ab580: 6561 223e 0a3c 6469 7620 636c 6173 733d  ea">.<div class=
+000ab590: 226a 702d 496e 7075 7450 726f 6d70 7420  "jp-InputPrompt 
+000ab5a0: 6a70 2d49 6e70 7574 4172 6561 2d70 726f  jp-InputArea-pro
+000ab5b0: 6d70 7422 3e49 6e26 6e62 7370 3b5b 365d  mpt">In&nbsp;[6]
+000ab5c0: 3a3c 2f64 6976 3e0a 3c64 6976 2063 6c61  :</div>.<div cla
+000ab5d0: 7373 3d22 6a70 2d43 6f64 654d 6972 726f  ss="jp-CodeMirro
+000ab5e0: 7245 6469 746f 7220 6a70 2d45 6469 746f  rEditor jp-Edito
+000ab5f0: 7220 6a70 2d49 6e70 7574 4172 6561 2d65  r jp-InputArea-e
+000ab600: 6469 746f 7222 2064 6174 612d 7479 7065  ditor" data-type
+000ab610: 3d22 696e 6c69 6e65 223e 0a20 2020 2020  ="inline">.     
+000ab620: 3c64 6976 2063 6c61 7373 3d22 436f 6465  <div class="Code
+000ab630: 4d69 7272 6f72 2063 6d2d 732d 6a75 7079  Mirror cm-s-jupy
+000ab640: 7465 7222 3e0a 3c64 6976 2063 6c61 7373  ter">.<div class
+000ab650: 3d22 2068 6967 686c 6967 6874 2068 6c2d  =" highlight hl-
+000ab660: 6970 7974 686f 6e33 223e 3c70 7265 3e3c  ipython3"><pre><
+000ab670: 7370 616e 3e3c 2f73 7061 6e3e 3c73 7061  span></span><spa
+000ab680: 6e20 636c 6173 733d 226e 223e 4e3c 2f73  n class="n">N</s
+000ab690: 7061 6e3e 3c73 7061 6e20 636c 6173 733d  pan><span class=
+000ab6a0: 226f 223e 3d3c 2f73 7061 6e3e 3c73 7061  "o">=</span><spa
+000ab6b0: 6e20 636c 6173 733d 226d 6922 3e31 303c  n class="mi">10<
+000ab6c0: 2f73 7061 6e3e 203c 7370 616e 2063 6c61  /span> <span cla
+000ab6d0: 7373 3d22 6331 223e 2320 4e75 6d62 6572  ss="c1"># Number
+000ab6e0: 206f 6620 7472 616a 6563 746f 7269 6573   of trajectories
+000ab6f0: 3c2f 7370 616e 3e0a 3c73 7061 6e20 636c  </span>.<span cl
+000ab700: 6173 733d 226e 223e 4d3c 2f73 7061 6e3e  ass="n">M</span>
+000ab710: 3c73 7061 6e20 636c 6173 733d 226f 223e  <span class="o">
+000ab720: 3d3c 2f73 7061 6e3e 3c73 7061 6e20 636c  =</span><span cl
+000ab730: 6173 733d 226d 6922 3e35 303c 2f73 7061  ass="mi">50</spa
+000ab740: 6e3e 203c 7370 616e 2063 6c61 7373 3d22  n> <span class="
+000ab750: 6331 223e 2320 4e75 6d62 6572 206f 6620  c1"># Number of 
+000ab760: 706f 696e 7473 2062 7920 7472 616a 6563  points by trajec
+000ab770: 746f 7279 3c2f 7370 616e 3e0a 3c73 7061  tory</span>.<spa
+000ab780: 6e20 636c 6173 733d 226e 223e 4c3c 2f73  n class="n">L</s
+000ab790: 7061 6e3e 3c73 7061 6e20 636c 6173 733d  pan><span class=
+000ab7a0: 226f 223e 3d3c 2f73 7061 6e3e 3c73 7061  "o">=</span><spa
+000ab7b0: 6e20 636c 6173 733d 226d 6922 3e31 303c  n class="mi">10<
+000ab7c0: 2f73 7061 6e3e 203c 7370 616e 2063 6c61  /span> <span cla
+000ab7d0: 7373 3d22 6331 223e 2320 4e75 6d62 6572  ss="c1"># Number
+000ab7e0: 206f 6620 6174 7472 6962 7574 6573 3c2f   of attributes</
+000ab7f0: 7370 616e 3e0a 3c73 7061 6e20 636c 6173  span>.<span clas
+000ab800: 733d 226e 223e 433c 2f73 7061 6e3e 3c73  s="n">C</span><s
+000ab810: 7061 6e20 636c 6173 733d 226f 223e 3d3c  pan class="o">=<
+000ab820: 2f73 7061 6e3e 3c73 7061 6e20 636c 6173  /span><span clas
+000ab830: 733d 226d 6922 3e33 3c2f 7370 616e 3e20  s="mi">3</span> 
+000ab840: 203c 7370 616e 2063 6c61 7373 3d22 6331   <span class="c1
+000ab850: 223e 2320 4e75 6d62 6572 206f 6620 636c  "># Number of cl
+000ab860: 6173 7365 7320 2843 3120 746f 2043 6e29  asses (C1 to Cn)
+000ab870: 3c2f 7370 616e 3e0a 3c73 7061 6e20 636c  </span>.<span cl
+000ab880: 6173 733d 226e 223e 7261 6e64 6f6d 4765  ass="n">randomGe
+000ab890: 6e65 7261 746f 723c 2f73 7061 6e3e 3c73  nerator</span><s
+000ab8a0: 7061 6e20 636c 6173 733d 2270 223e 283c  pan class="p">(<
+000ab8b0: 2f73 7061 6e3e 3c73 7061 6e20 636c 6173  /span><span clas
+000ab8c0: 733d 226e 223e 4e3c 2f73 7061 6e3e 3c73  s="n">N</span><s
+000ab8d0: 7061 6e20 636c 6173 733d 2270 223e 2c3c  pan class="p">,<
+000ab8e0: 2f73 7061 6e3e 203c 7370 616e 2063 6c61  /span> <span cla
+000ab8f0: 7373 3d22 6e22 3e4d 3c2f 7370 616e 3e3c  ss="n">M</span><
+000ab900: 7370 616e 2063 6c61 7373 3d22 7022 3e2c  span class="p">,
+000ab910: 3c2f 7370 616e 3e20 3c73 7061 6e20 636c  </span> <span cl
+000ab920: 6173 733d 226e 223e 4c3c 2f73 7061 6e3e  ass="n">L</span>
+000ab930: 3c73 7061 6e20 636c 6173 733d 2270 223e  <span class="p">
+000ab940: 2c3c 2f73 7061 6e3e 203c 7370 616e 2063  ,</span> <span c
+000ab950: 6c61 7373 3d22 6e22 3e43 3c2f 7370 616e  lass="n">C</span
+000ab960: 3e3c 7370 616e 2063 6c61 7373 3d22 7022  ><span class="p"
+000ab970: 3e29 3c2f 7370 616e 3e0a 3c2f 7072 653e  >)</span>.</pre>
+000ab980: 3c2f 6469 763e 0a0a 2020 2020 203c 2f64  </div>..     </d
+000ab990: 6976 3e0a 3c2f 6469 763e 0a3c 2f64 6976  iv>.</div>.</div
+000ab9a0: 3e0a 3c2f 6469 763e 0a0a 3c64 6976 2063  >.</div>..<div c
+000ab9b0: 6c61 7373 3d22 6a70 2d43 656c 6c2d 6f75  lass="jp-Cell-ou
+000ab9c0: 7470 7574 5772 6170 7065 7222 3e0a 3c64  tputWrapper">.<d
+000ab9d0: 6976 2063 6c61 7373 3d22 6a70 2d43 6f6c  iv class="jp-Col
+000ab9e0: 6c61 7073 6572 206a 702d 4f75 7470 7574  lapser jp-Output
+000ab9f0: 436f 6c6c 6170 7365 7220 6a70 2d43 656c  Collapser jp-Cel
+000aba00: 6c2d 6f75 7470 7574 436f 6c6c 6170 7365  l-outputCollapse
+000aba10: 7222 3e0a 3c2f 6469 763e 0a0a 0a3c 6469  r">.</div>...<di
+000aba20: 7620 636c 6173 733d 226a 702d 4f75 7470  v class="jp-Outp
+000aba30: 7574 4172 6561 206a 702d 4365 6c6c 2d6f  utArea jp-Cell-o
+000aba40: 7574 7075 7441 7265 6122 3e0a 0a3c 6469  utputArea">..<di
+000aba50: 7620 636c 6173 733d 226a 702d 4f75 7470  v class="jp-Outp
+000aba60: 7574 4172 6561 2d63 6869 6c64 223e 0a0a  utArea-child">..
+000aba70: 2020 2020 0a20 2020 203c 6469 7620 636c      .    <div cl
+000aba80: 6173 733d 226a 702d 4f75 7470 7574 5072  ass="jp-OutputPr
+000aba90: 6f6d 7074 206a 702d 4f75 7470 7574 4172  ompt jp-OutputAr
+000abaa0: 6561 2d70 726f 6d70 7422 3e4f 7574 5b36  ea-prompt">Out[6
+000abab0: 5d3a 3c2f 6469 763e 0a0a 0a0a 3c64 6976  ]:</div>....<div
+000abac0: 2063 6c61 7373 3d22 6a70 2d52 656e 6465   class="jp-Rende
+000abad0: 7265 6448 544d 4c43 6f6d 6d6f 6e20 6a70  redHTMLCommon jp
+000abae0: 2d52 656e 6465 7265 6448 544d 4c20 6a70  -RenderedHTML jp
+000abaf0: 2d4f 7574 7075 7441 7265 612d 6f75 7470  -OutputArea-outp
+000abb00: 7574 206a 702d 4f75 7470 7574 4172 6561  ut jp-OutputArea
+000abb10: 2d65 7865 6375 7465 5265 7375 6c74 2220  -executeResult" 
+000abb20: 6461 7461 2d6d 696d 652d 7479 7065 3d22  data-mime-type="
+000abb30: 7465 7874 2f68 746d 6c22 3e0a 3c64 6976  text/html">.<div
+000abb40: 3e0a 3c73 7479 6c65 2073 636f 7065 643e  >.<style scoped>
+000abb50: 0a20 2020 202e 6461 7461 6672 616d 6520  .    .dataframe 
+000abb60: 7462 6f64 7920 7472 2074 683a 6f6e 6c79  tbody tr th:only
+000abb70: 2d6f 662d 7479 7065 207b 0a20 2020 2020  -of-type {.     
+000abb80: 2020 2076 6572 7469 6361 6c2d 616c 6967     vertical-alig
+000abb90: 6e3a 206d 6964 646c 653b 0a20 2020 207d  n: middle;.    }
+000abba0: 0a0a 2020 2020 2e64 6174 6166 7261 6d65  ..    .dataframe
+000abbb0: 2074 626f 6479 2074 7220 7468 207b 0a20   tbody tr th {. 
+000abbc0: 2020 2020 2020 2076 6572 7469 6361 6c2d         vertical-
+000abbd0: 616c 6967 6e3a 2074 6f70 3b0a 2020 2020  align: top;.    
+000abbe0: 7d0a 0a20 2020 202e 6461 7461 6672 616d  }..    .datafram
+000abbf0: 6520 7468 6561 6420 7468 207b 0a20 2020  e thead th {.   
+000abc00: 2020 2020 2074 6578 742d 616c 6967 6e3a       text-align:
+000abc10: 2072 6967 6874 3b0a 2020 2020 7d0a 3c2f   right;.    }.</
+000abc20: 7374 796c 653e 0a3c 7461 626c 6520 626f  style>.<table bo
+000abc30: 7264 6572 3d22 3122 2063 6c61 7373 3d22  rder="1" class="
+000abc40: 6461 7461 6672 616d 6522 3e0a 2020 3c74  dataframe">.  <t
+000abc50: 6865 6164 3e0a 2020 2020 3c74 7220 7374  head>.    <tr st
+000abc60: 796c 653d 2274 6578 742d 616c 6967 6e3a  yle="text-align:
+000abc70: 2072 6967 6874 3b22 3e0a 2020 2020 2020   right;">.      
+000abc80: 3c74 683e 3c2f 7468 3e0a 2020 2020 2020  <th></th>.      
+000abc90: 3c74 683e 7469 643c 2f74 683e 0a20 2020  <th>tid</th>.   
+000abca0: 2020 203c 7468 3e61 315f 7370 6163 653c     <th>a1_space<
+000abcb0: 2f74 683e 0a20 2020 2020 203c 7468 3e61  /th>.      <th>a
+000abcc0: 325f 7469 6d65 3c2f 7468 3e0a 2020 2020  2_time</th>.    
+000abcd0: 2020 3c74 683e 6133 5f6e 313c 2f74 683e    <th>a3_n1</th>
+000abce0: 0a20 2020 2020 203c 7468 3e61 345f 6e32  .      <th>a4_n2
+000abcf0: 3c2f 7468 3e0a 2020 2020 2020 3c74 683e  </th>.      <th>
+000abd00: 6135 5f6e 6f6d 696e 616c 3c2f 7468 3e0a  a5_nominal</th>.
+000abd10: 2020 2020 2020 3c74 683e 6136 5f64 6179        <th>a6_day
+000abd20: 3c2f 7468 3e0a 2020 2020 2020 3c74 683e  </th>.      <th>
+000abd30: 6137 5f77 6561 7468 6572 3c2f 7468 3e0a  a7_weather</th>.
+000abd40: 2020 2020 2020 3c74 683e 6138 5f63 6174        <th>a8_cat
+000abd50: 6567 6f72 793c 2f74 683e 0a20 2020 2020  egory</th>.     
+000abd60: 203c 7468 3e61 395f 7370 6163 653c 2f74   <th>a9_space</t
+000abd70: 683e 0a20 2020 2020 203c 7468 3e61 3130  h>.      <th>a10
+000abd80: 5f74 696d 653c 2f74 683e 0a20 2020 2020  _time</th>.     
+000abd90: 203c 7468 3e6c 6162 656c 3c2f 7468 3e0a   <th>label</th>.
+000abda0: 2020 2020 3c2f 7472 3e0a 2020 3c2f 7468      </tr>.  </th
+000abdb0: 6561 643e 0a20 203c 7462 6f64 793e 0a20  ead>.  <tbody>. 
+000abdc0: 2020 203c 7472 3e0a 2020 2020 2020 3c74     <tr>.      <t
+000abdd0: 683e 303c 2f74 683e 0a20 2020 2020 203c  h>0</th>.      <
+000abde0: 7464 3e31 3c2f 7464 3e0a 2020 2020 2020  td>1</td>.      
+000abdf0: 3c74 643e 3133 342e 3520 3834 382e 3238  <td>134.5 848.28
+000abe00: 3c2f 7464 3e0a 2020 2020 2020 3c74 643e  </td>.      <td>
+000abe10: 3131 343c 2f74 643e 0a20 2020 2020 203c  114</td>.      <
+000abe20: 7464 3e39 3439 3c2f 7464 3e0a 2020 2020  td>949</td>.    
+000abe30: 2020 3c74 643e 3937 362e 3938 3c2f 7464    <td>976.98</td
+000abe40: 3e0a 2020 2020 2020 3c74 643e 5058 3c2f  >.      <td>PX</
+000abe50: 7464 3e0a 2020 2020 2020 3c74 643e 5475  td>.      <td>Tu
+000abe60: 6573 6461 793c 2f74 643e 0a20 2020 2020  esday</td>.     
+000abe70: 203c 7464 3e43 6c6f 7564 733c 2f74 643e   <td>Clouds</td>
+000abe80: 0a20 2020 2020 203c 7464 3e4f 7574 646f  .      <td>Outdo
+000abe90: 6f72 7320 2661 6d70 3b20 5265 6372 6561  ors &amp; Recrea
+000abea0: 7469 6f6e 3c2f 7464 3e0a 2020 2020 2020  tion</td>.      
+000abeb0: 3c74 643e 3130 312e 3034 2037 3738 2e35  <td>101.04 778.5
+000abec0: 323c 2f74 643e 0a20 2020 2020 203c 7464  2</td>.      <td
+000abed0: 3e31 3131 343c 2f74 643e 0a20 2020 2020  >1114</td>.     
+000abee0: 203c 7464 3e43 313c 2f74 643e 0a20 2020   <td>C1</td>.   
+000abef0: 203c 2f74 723e 0a20 2020 203c 7472 3e0a   </tr>.    <tr>.
+000abf00: 2020 2020 2020 3c74 683e 313c 2f74 683e        <th>1</th>
+000abf10: 0a20 2020 2020 203c 7464 3e31 3c2f 7464  .      <td>1</td
+000abf20: 3e0a 2020 2020 2020 3c74 643e 3736 342e  >.      <td>764.
+000abf30: 3534 2032 3535 2e33 323c 2f74 643e 0a20  54 255.32</td>. 
+000abf40: 2020 2020 203c 7464 3e39 3835 3c2f 7464       <td>985</td
+000abf50: 3e0a 2020 2020 2020 3c74 643e 2d36 3536  >.      <td>-656
+000abf60: 3c2f 7464 3e0a 2020 2020 2020 3c74 643e  </td>.      <td>
+000abf70: 3633 302e 3737 3c2f 7464 3e0a 2020 2020  630.77</td>.    
+000abf80: 2020 3c74 643e 484b 3c2f 7464 3e0a 2020    <td>HK</td>.  
+000abf90: 2020 2020 3c74 643e 5361 7475 7264 6179      <td>Saturday
+000abfa0: 3c2f 7464 3e0a 2020 2020 2020 3c74 643e  </td>.      <td>
+000abfb0: 436c 6f75 6473 3c2f 7464 3e0a 2020 2020  Clouds</td>.    
+000abfc0: 2020 3c74 643e 5368 6f70 2026 616d 703b    <td>Shop &amp;
+000abfd0: 2053 6572 7669 6365 3c2f 7464 3e0a 2020   Service</td>.  
+000abfe0: 2020 2020 3c74 643e 3332 382e 3432 2035      <td>328.42 5
+000abff0: 3039 2e37 383c 2f74 643e 0a20 2020 2020  09.78</td>.     
+000ac000: 203c 7464 3e38 333c 2f74 643e 0a20 2020   <td>83</td>.   
+000ac010: 2020 203c 7464 3e43 313c 2f74 643e 0a20     <td>C1</td>. 
+000ac020: 2020 203c 2f74 723e 0a20 2020 203c 7472     </tr>.    <tr
+000ac030: 3e0a 2020 2020 2020 3c74 683e 323c 2f74  >.      <th>2</t
+000ac040: 683e 0a20 2020 2020 203c 7464 3e31 3c2f  h>.      <td>1</
+000ac050: 7464 3e0a 2020 2020 2020 3c74 643e 3439  td>.      <td>49
+000ac060: 352e 3933 2034 3439 2e39 343c 2f74 643e  5.93 449.94</td>
+000ac070: 0a20 2020 2020 203c 7464 3e37 3436 3c2f  .      <td>746</
+000ac080: 7464 3e0a 2020 2020 2020 3c74 643e 3334  td>.      <td>34
+000ac090: 343c 2f74 643e 0a20 2020 2020 203c 7464  4</td>.      <td
+000ac0a0: 3e36 3935 2e30 353c 2f74 643e 0a20 2020  >695.05</td>.   
+000ac0b0: 2020 203c 7464 3e4a 4d3c 2f74 643e 0a20     <td>JM</td>. 
+000ac0c0: 2020 2020 203c 7464 3e53 6174 7572 6461       <td>Saturda
+000ac0d0: 793c 2f74 643e 0a20 2020 2020 203c 7464  y</td>.      <td
+000ac0e0: 3e52 6169 6e3c 2f74 643e 0a20 2020 2020  >Rain</td>.     
+000ac0f0: 203c 7464 3e54 7261 7665 6c20 2661 6d70   <td>Travel &amp
+000ac100: 3b20 5472 616e 7370 6f72 743c 2f74 643e  ; Transport</td>
+000ac110: 0a20 2020 2020 203c 7464 3e36 3635 2e39  .      <td>665.9
+000ac120: 3120 3137 392e 3735 3c2f 7464 3e0a 2020  1 179.75</td>.  
+000ac130: 2020 2020 3c74 643e 3130 3733 3c2f 7464      <td>1073</td
+000ac140: 3e0a 2020 2020 2020 3c74 643e 4331 3c2f  >.      <td>C1</
+000ac150: 7464 3e0a 2020 2020 3c2f 7472 3e0a 2020  td>.    </tr>.  
+000ac160: 2020 3c74 723e 0a20 2020 2020 203c 7468    <tr>.      <th
+000ac170: 3e33 3c2f 7468 3e0a 2020 2020 2020 3c74  >3</th>.      <t
+000ac180: 643e 313c 2f74 643e 0a20 2020 2020 203c  d>1</td>.      <
+000ac190: 7464 3e36 3532 2e32 3420 3738 392e 3531  td>652.24 789.51
+000ac1a0: 3c2f 7464 3e0a 2020 2020 2020 3c74 643e  </td>.      <td>
+000ac1b0: 3131 3637 3c2f 7464 3e0a 2020 2020 2020  1167</td>.      
+000ac1c0: 3c74 643e 2d34 3432 3c2f 7464 3e0a 2020  <td>-442</td>.  
+000ac1d0: 2020 2020 3c74 643e 3435 302e 3835 3c2f      <td>450.85</
+000ac1e0: 7464 3e0a 2020 2020 2020 3c74 643e 5a4f  td>.      <td>ZO
+000ac1f0: 3c2f 7464 3e0a 2020 2020 2020 3c74 643e  </td>.      <td>
+000ac200: 5765 646e 6573 6461 793c 2f74 643e 0a20  Wednesday</td>. 
+000ac210: 2020 2020 203c 7464 3e55 6e6b 6e6f 776e       <td>Unknown
+000ac220: 3c2f 7464 3e0a 2020 2020 2020 3c74 643e  </td>.      <td>
+000ac230: 4e69 6768 746c 6966 6520 5370 6f74 3c2f  Nightlife Spot</
+000ac240: 7464 3e0a 2020 2020 2020 3c74 643e 3134  td>.      <td>14
+000ac250: 392e 3731 2031 3431 2e36 383c 2f74 643e  9.71 141.68</td>
+000ac260: 0a20 2020 2020 203c 7464 3e31 3835 3c2f  .      <td>185</
+000ac270: 7464 3e0a 2020 2020 2020 3c74 643e 4331  td>.      <td>C1
+000ac280: 3c2f 7464 3e0a 2020 2020 3c2f 7472 3e0a  </td>.    </tr>.
+000ac290: 2020 2020 3c74 723e 0a20 2020 2020 203c      <tr>.      <
+000ac2a0: 7468 3e34 3c2f 7468 3e0a 2020 2020 2020  th>4</th>.      
+000ac2b0: 3c74 643e 313c 2f74 643e 0a20 2020 2020  <td>1</td>.     
+000ac2c0: 203c 7464 3e39 332e 3935 2032 382e 3338   <td>93.95 28.38
+000ac2d0: 3c2f 7464 3e0a 2020 2020 2020 3c74 643e  </td>.      <td>
+000ac2e0: 3131 3335 3c2f 7464 3e0a 2020 2020 2020  1135</td>.      
+000ac2f0: 3c74 643e 3332 373c 2f74 643e 0a20 2020  <td>327</td>.   
+000ac300: 2020 203c 7464 3e35 3233 2e39 303c 2f74     <td>523.90</t
+000ac310: 643e 0a20 2020 2020 203c 7464 3e43 553c  d>.      <td>CU<
+000ac320: 2f74 643e 0a20 2020 2020 203c 7464 3e4d  /td>.      <td>M
+000ac330: 6f6e 6461 793c 2f74 643e 0a20 2020 2020  onday</td>.     
+000ac340: 203c 7464 3e43 6c6f 7564 733c 2f74 643e   <td>Clouds</td>
+000ac350: 0a20 2020 2020 203c 7464 3e50 726f 6665  .      <td>Profe
+000ac360: 7373 696f 6e61 6c20 2661 6d70 3b20 4f74  ssional &amp; Ot
+000ac370: 6865 7220 506c 6163 6573 3c2f 7464 3e0a  her Places</td>.
+000ac380: 2020 2020 2020 3c74 643e 3836 362e 3431        <td>866.41
+000ac390: 2033 3035 2e39 333c 2f74 643e 0a20 2020   305.93</td>.   
+000ac3a0: 2020 203c 7464 3e35 3232 3c2f 7464 3e0a     <td>522</td>.
+000ac3b0: 2020 2020 2020 3c74 643e 4331 3c2f 7464        <td>C1</td
+000ac3c0: 3e0a 2020 2020 3c2f 7472 3e0a 2020 2020  >.    </tr>.    
+000ac3d0: 3c74 723e 0a20 2020 2020 203c 7468 3e2e  <tr>.      <th>.
+000ac3e0: 2e2e 3c2f 7468 3e0a 2020 2020 2020 3c74  ..</th>.      <t
+000ac3f0: 643e 2e2e 2e3c 2f74 643e 0a20 2020 2020  d>...</td>.     
+000ac400: 203c 7464 3e2e 2e2e 3c2f 7464 3e0a 2020   <td>...</td>.  
+000ac410: 2020 2020 3c74 643e 2e2e 2e3c 2f74 643e      <td>...</td>
+000ac420: 0a20 2020 2020 203c 7464 3e2e 2e2e 3c2f  .      <td>...</
+000ac430: 7464 3e0a 2020 2020 2020 3c74 643e 2e2e  td>.      <td>..
+000ac440: 2e3c 2f74 643e 0a20 2020 2020 203c 7464  .</td>.      <td
+000ac450: 3e2e 2e2e 3c2f 7464 3e0a 2020 2020 2020  >...</td>.      
+000ac460: 3c74 643e 2e2e 2e3c 2f74 643e 0a20 2020  <td>...</td>.   
+000ac470: 2020 203c 7464 3e2e 2e2e 3c2f 7464 3e0a     <td>...</td>.
+000ac480: 2020 2020 2020 3c74 643e 2e2e 2e3c 2f74        <td>...</t
+000ac490: 643e 0a20 2020 2020 203c 7464 3e2e 2e2e  d>.      <td>...
+000ac4a0: 3c2f 7464 3e0a 2020 2020 2020 3c74 643e  </td>.      <td>
+000ac4b0: 2e2e 2e3c 2f74 643e 0a20 2020 2020 203c  ...</td>.      <
+000ac4c0: 7464 3e2e 2e2e 3c2f 7464 3e0a 2020 2020  td>...</td>.    
+000ac4d0: 3c2f 7472 3e0a 2020 2020 3c74 723e 0a20  </tr>.    <tr>. 
+000ac4e0: 2020 2020 203c 7468 3e34 3935 3c2f 7468       <th>495</th
+000ac4f0: 3e0a 2020 2020 2020 3c74 643e 3131 3c2f  >.      <td>11</
+000ac500: 7464 3e0a 2020 2020 2020 3c74 643e 3634  td>.      <td>64
+000ac510: 372e 3936 2033 3030 2e35 3c2f 7464 3e0a  7.96 300.5</td>.
+000ac520: 2020 2020 2020 3c74 643e 3132 3035 3c2f        <td>1205</
+000ac530: 7464 3e0a 2020 2020 2020 3c74 643e 3536  td>.      <td>56
+000ac540: 313c 2f74 643e 0a20 2020 2020 203c 7464  1</td>.      <td
+000ac550: 3e38 3139 2e31 323c 2f74 643e 0a20 2020  >819.12</td>.   
+000ac560: 2020 203c 7464 3e41 4352 3c2f 7464 3e0a     <td>ACR</td>.
+000ac570: 2020 2020 2020 3c74 643e 5361 7475 7264        <td>Saturd
+000ac580: 6179 3c2f 7464 3e0a 2020 2020 2020 3c74  ay</td>.      <t
+000ac590: 643e 5261 696e 3c2f 7464 3e0a 2020 2020  d>Rain</td>.    
+000ac5a0: 2020 3c74 643e 4172 7473 2026 616d 703b    <td>Arts &amp;
+000ac5b0: 2045 6e74 6572 7461 696e 6d65 6e74 3c2f   Entertainment</
+000ac5c0: 7464 3e0a 2020 2020 2020 3c74 643e 3531  td>.      <td>51
+000ac5d0: 352e 3936 2039 3535 2e36 363c 2f74 643e  5.96 955.66</td>
+000ac5e0: 0a20 2020 2020 203c 7464 3e36 3334 3c2f  .      <td>634</
+000ac5f0: 7464 3e0a 2020 2020 2020 3c74 643e 4333  td>.      <td>C3
+000ac600: 3c2f 7464 3e0a 2020 2020 3c2f 7472 3e0a  </td>.    </tr>.
+000ac610: 2020 2020 3c74 723e 0a20 2020 2020 203c      <tr>.      <
+000ac620: 7468 3e34 3936 3c2f 7468 3e0a 2020 2020  th>496</th>.    
+000ac630: 2020 3c74 643e 3131 3c2f 7464 3e0a 2020    <td>11</td>.  
+000ac640: 2020 2020 3c74 643e 3737 392e 3236 2039      <td>779.26 9
+000ac650: 3333 2e36 313c 2f74 643e 0a20 2020 2020  33.61</td>.     
+000ac660: 203c 7464 3e34 3835 3c2f 7464 3e0a 2020   <td>485</td>.  
+000ac670: 2020 2020 3c74 643e 3132 313c 2f74 643e      <td>121</td>
+000ac680: 0a20 2020 2020 203c 7464 3e37 3435 2e33  .      <td>745.3
+000ac690: 323c 2f74 643e 0a20 2020 2020 203c 7464  2</td>.      <td
+000ac6a0: 3e41 495a 3c2f 7464 3e0a 2020 2020 2020  >AIZ</td>.      
+000ac6b0: 3c74 643e 5475 6573 6461 793c 2f74 643e  <td>Tuesday</td>
+000ac6c0: 0a20 2020 2020 203c 7464 3e52 6169 6e3c  .      <td>Rain<
+000ac6d0: 2f74 643e 0a20 2020 2020 203c 7464 3e4f  /td>.      <td>O
+000ac6e0: 7574 646f 6f72 7320 2661 6d70 3b20 5265  utdoors &amp; Re
+000ac6f0: 6372 6561 7469 6f6e 3c2f 7464 3e0a 2020  creation</td>.  
+000ac700: 2020 2020 3c74 643e 3337 372e 3833 2032      <td>377.83 2
+000ac710: 3633 2e31 333c 2f74 643e 0a20 2020 2020  63.13</td>.     
+000ac720: 203c 7464 3e34 3335 3c2f 7464 3e0a 2020   <td>435</td>.  
+000ac730: 2020 2020 3c74 643e 4333 3c2f 7464 3e0a      <td>C3</td>.
+000ac740: 2020 2020 3c2f 7472 3e0a 2020 2020 3c74      </tr>.    <t
+000ac750: 723e 0a20 2020 2020 203c 7468 3e34 3937  r>.      <th>497
+000ac760: 3c2f 7468 3e0a 2020 2020 2020 3c74 643e  </th>.      <td>
+000ac770: 3131 3c2f 7464 3e0a 2020 2020 2020 3c74  11</td>.      <t
+000ac780: 643e 3339 382e 3320 3534 352e 3139 3c2f  d>398.3 545.19</
+000ac790: 7464 3e0a 2020 2020 2020 3c74 643e 3430  td>.      <td>40
+000ac7a0: 363c 2f74 643e 0a20 2020 2020 203c 7464  6</td>.      <td
+000ac7b0: 3e2d 3234 383c 2f74 643e 0a20 2020 2020  >-248</td>.     
+000ac7c0: 203c 7464 3e31 3830 2e38 393c 2f74 643e   <td>180.89</td>
+000ac7d0: 0a20 2020 2020 203c 7464 3e59 483c 2f74  .      <td>YH</t
+000ac7e0: 643e 0a20 2020 2020 203c 7464 3e4d 6f6e  d>.      <td>Mon
+000ac7f0: 6461 793c 2f74 643e 0a20 2020 2020 203c  day</td>.      <
+000ac800: 7464 3e46 6f67 3c2f 7464 3e0a 2020 2020  td>Fog</td>.    
+000ac810: 2020 3c74 643e 4576 656e 743c 2f74 643e    <td>Event</td>
+000ac820: 0a20 2020 2020 203c 7464 3e34 3538 2e32  .      <td>458.2
+000ac830: 3720 3636 352e 3436 3c2f 7464 3e0a 2020  7 665.46</td>.  
+000ac840: 2020 2020 3c74 643e 3837 343c 2f74 643e      <td>874</td>
+000ac850: 0a20 2020 2020 203c 7464 3e43 333c 2f74  .      <td>C3</t
+000ac860: 643e 0a20 2020 203c 2f74 723e 0a20 2020  d>.    </tr>.   
+000ac870: 203c 7472 3e0a 2020 2020 2020 3c74 683e   <tr>.      <th>
+000ac880: 3439 383c 2f74 683e 0a20 2020 2020 203c  498</th>.      <
+000ac890: 7464 3e31 313c 2f74 643e 0a20 2020 2020  td>11</td>.     
+000ac8a0: 203c 7464 3e31 3333 2e35 3220 3630 352e   <td>133.52 605.
+000ac8b0: 3032 3c2f 7464 3e0a 2020 2020 2020 3c74  02</td>.      <t
+000ac8c0: 643e 3632 3c2f 7464 3e0a 2020 2020 2020  d>62</td>.      
+000ac8d0: 3c74 643e 2d34 3835 3c2f 7464 3e0a 2020  <td>-485</td>.  
+000ac8e0: 2020 2020 3c74 643e 3839 302e 3432 3c2f      <td>890.42</
+000ac8f0: 7464 3e0a 2020 2020 2020 3c74 643e 4449  td>.      <td>DI
+000ac900: 3c2f 7464 3e0a 2020 2020 2020 3c74 643e  </td>.      <td>
+000ac910: 5468 7572 7364 6179 3c2f 7464 3e0a 2020  Thursday</td>.  
+000ac920: 2020 2020 3c74 643e 436c 6f75 6473 3c2f      <td>Clouds</
+000ac930: 7464 3e0a 2020 2020 2020 3c74 643e 5265  td>.      <td>Re
+000ac940: 7369 6465 6e63 653c 2f74 643e 0a20 2020  sidence</td>.   
+000ac950: 2020 203c 7464 3e32 3633 2e39 3320 3934     <td>263.93 94
+000ac960: 342e 383c 2f74 643e 0a20 2020 2020 203c  4.8</td>.      <
+000ac970: 7464 3e31 3134 313c 2f74 643e 0a20 2020  td>1141</td>.   
+000ac980: 2020 203c 7464 3e43 333c 2f74 643e 0a20     <td>C3</td>. 
+000ac990: 2020 203c 2f74 723e 0a20 2020 203c 7472     </tr>.    <tr
+000ac9a0: 3e0a 2020 2020 2020 3c74 683e 3439 393c  >.      <th>499<
+000ac9b0: 2f74 683e 0a20 2020 2020 203c 7464 3e31  /th>.      <td>1
+000ac9c0: 313c 2f74 643e 0a20 2020 2020 203c 7464  1</td>.      <td
+000ac9d0: 3e33 3837 2e34 3920 3130 362e 3132 3c2f  >387.49 106.12</
+000ac9e0: 7464 3e0a 2020 2020 2020 3c74 643e 3433  td>.      <td>43
+000ac9f0: 353c 2f74 643e 0a20 2020 2020 203c 7464  5</td>.      <td
+000aca00: 3e38 3337 3c2f 7464 3e0a 2020 2020 2020  >837</td>.      
+000aca10: 3c74 643e 3339 382e 3133 3c2f 7464 3e0a  <td>398.13</td>.
+000aca20: 2020 2020 2020 3c74 643e 4143 4d3c 2f74        <td>ACM</t
+000aca30: 643e 0a20 2020 2020 203c 7464 3e54 7565  d>.      <td>Tue
+000aca40: 7364 6179 3c2f 7464 3e0a 2020 2020 2020  sday</td>.      
+000aca50: 3c74 643e 5261 696e 3c2f 7464 3e0a 2020  <td>Rain</td>.  
+000aca60: 2020 2020 3c74 643e 5265 7369 6465 6e63      <td>Residenc
+000aca70: 653c 2f74 643e 0a20 2020 2020 203c 7464  e</td>.      <td
+000aca80: 3e39 3136 2e34 3620 3738 352e 3133 3c2f  >916.46 785.13</
+000aca90: 7464 3e0a 2020 2020 2020 3c74 643e 3131  td>.      <td>11
+000acaa0: 3938 3c2f 7464 3e0a 2020 2020 2020 3c74  98</td>.      <t
+000acab0: 643e 4333 3c2f 7464 3e0a 2020 2020 3c2f  d>C3</td>.    </
+000acac0: 7472 3e0a 2020 3c2f 7462 6f64 793e 0a3c  tr>.  </tbody>.<
+000acad0: 2f74 6162 6c65 3e0a 3c70 3e35 3030 2072  /table>.<p>500 r
+000acae0: 6f77 7320 c397 2031 3220 636f 6c75 6d6e  ows .. 12 column
+000acaf0: 733c 2f70 3e0a 3c2f 6469 763e 0a3c 2f64  s</p>.</div>.</d
+000acb00: 6976 3e0a 0a3c 2f64 6976 3e0a 0a3c 2f64  iv>..</div>..</d
+000acb10: 6976 3e0a 0a3c 2f64 6976 3e0a 0a3c 2f64  iv>..</div>..</d
+000acb20: 6976 3e0a 3c64 6976 2063 6c61 7373 3d22  iv>.<div class="
+000acb30: 6a70 2d43 656c 6c20 6a70 2d4d 6172 6b64  jp-Cell jp-Markd
+000acb40: 6f77 6e43 656c 6c20 6a70 2d4e 6f74 6562  ownCell jp-Noteb
+000acb50: 6f6f 6b2d 6365 6c6c 223e 0a3c 6469 7620  ook-cell">.<div 
+000acb60: 636c 6173 733d 226a 702d 4365 6c6c 2d69  class="jp-Cell-i
+000acb70: 6e70 7574 5772 6170 7065 7222 3e0a 3c64  nputWrapper">.<d
+000acb80: 6976 2063 6c61 7373 3d22 6a70 2d43 6f6c  iv class="jp-Col
+000acb90: 6c61 7073 6572 206a 702d 496e 7075 7443  lapser jp-InputC
+000acba0: 6f6c 6c61 7073 6572 206a 702d 4365 6c6c  ollapser jp-Cell
+000acbb0: 2d69 6e70 7574 436f 6c6c 6170 7365 7222  -inputCollapser"
+000acbc0: 3e0a 3c2f 6469 763e 0a3c 6469 7620 636c  >.</div>.<div cl
+000acbd0: 6173 733d 226a 702d 496e 7075 7441 7265  ass="jp-InputAre
+000acbe0: 6120 6a70 2d43 656c 6c2d 696e 7075 7441  a jp-Cell-inputA
+000acbf0: 7265 6122 3e3c 6469 7620 636c 6173 733d  rea"><div class=
+000acc00: 226a 702d 496e 7075 7450 726f 6d70 7420  "jp-InputPrompt 
+000acc10: 6a70 2d49 6e70 7574 4172 6561 2d70 726f  jp-InputArea-pro
+000acc20: 6d70 7422 3e0a 3c2f 6469 763e 3c64 6976  mpt">.</div><div
+000acc30: 2063 6c61 7373 3d22 6a70 2d52 656e 6465   class="jp-Rende
+000acc40: 7265 6448 544d 4c43 6f6d 6d6f 6e20 6a70  redHTMLCommon jp
+000acc50: 2d52 656e 6465 7265 644d 6172 6b64 6f77  -RenderedMarkdow
+000acc60: 6e20 6a70 2d4d 6172 6b64 6f77 6e4f 7574  n jp-MarkdownOut
+000acc70: 7075 7420 2220 6461 7461 2d6d 696d 652d  put " data-mime-
+000acc80: 7479 7065 3d22 7465 7874 2f6d 6172 6b64  type="text/markd
+000acc90: 6f77 6e22 3e0a 0a3c 7072 653e 3c63 6f64  own">..<pre><cod
+000acca0: 653e 6429 2054 6f20 6765 6e65 7261 7465  e>d) To generate
+000accb0: 2061 2073 6574 206f 6620 7261 6e64 6f6d   a set of random
+000accc0: 2064 6174 6173 6574 733a 0a0a 3c2f 636f   datasets:..</co
+000accd0: 6465 3e3c 2f70 7265 3e0a 3c70 3e43 7265  de></pre>.<p>Cre
+000acce0: 6174 6573 2061 6e64 2073 6176 6520 6461  ates and save da
+000accf0: 7461 7365 7420 6669 6c65 7320 2869 6e63  taset files (inc
+000acd00: 6c75 6469 6e67 206d 6f76 656c 6574 7320  luding movelets 
+000acd10: 6a73 6f6e 2064 6573 6372 6970 746f 7220  json descriptor 
+000acd20: 6669 6c65 292e 2047 656e 6572 6174 6573  file). Generates
+000acd30: 2072 616e 646f 6d69 6320 6461 7461 7365   randomic datase
+000acd40: 7473 2069 6e20 6120 696e 6372 6561 7369  ts in a increasi
+000acd50: 6e67 206c 6f67 2073 6361 6c65 2066 6f72  ng log scale for
+000acd60: 2065 6163 6820 7061 7261 6d65 7465 722e   each parameter.
+000acd70: 2049 7420 7573 6573 2074 6865 206d 6964   It uses the mid
+000acd80: 646c 6520 7661 6c75 6520 666f 7220 7468  dle value for th
+000acd90: 6520 6f74 6865 7220 636f 6e66 6967 7572  e other configur
+000acda0: 6174 696f 6e73 3c2f 703e 0a0a 3c2f 6469  ations</p>..</di
+000acdb0: 763e 0a3c 2f64 6976 3e0a 3c2f 6469 763e  v>.</div>.</div>
+000acdc0: 0a3c 2f64 6976 3e3c 6469 7620 636c 6173  .</div><div clas
+000acdd0: 733d 226a 702d 4365 6c6c 206a 702d 436f  s="jp-Cell jp-Co
+000acde0: 6465 4365 6c6c 206a 702d 4e6f 7465 626f  deCell jp-Notebo
+000acdf0: 6f6b 2d63 656c 6c20 2020 223e 0a3c 6469  ok-cell   ">.<di
+000ace00: 7620 636c 6173 733d 226a 702d 4365 6c6c  v class="jp-Cell
+000ace10: 2d69 6e70 7574 5772 6170 7065 7222 3e0a  -inputWrapper">.
+000ace20: 3c64 6976 2063 6c61 7373 3d22 6a70 2d43  <div class="jp-C
+000ace30: 6f6c 6c61 7073 6572 206a 702d 496e 7075  ollapser jp-Inpu
+000ace40: 7443 6f6c 6c61 7073 6572 206a 702d 4365  tCollapser jp-Ce
+000ace50: 6c6c 2d69 6e70 7574 436f 6c6c 6170 7365  ll-inputCollapse
+000ace60: 7222 3e0a 3c2f 6469 763e 0a3c 6469 7620  r">.</div>.<div 
+000ace70: 636c 6173 733d 226a 702d 496e 7075 7441  class="jp-InputA
+000ace80: 7265 6120 6a70 2d43 656c 6c2d 696e 7075  rea jp-Cell-inpu
+000ace90: 7441 7265 6122 3e0a 3c64 6976 2063 6c61  tArea">.<div cla
+000acea0: 7373 3d22 6a70 2d49 6e70 7574 5072 6f6d  ss="jp-InputProm
+000aceb0: 7074 206a 702d 496e 7075 7441 7265 612d  pt jp-InputArea-
+000acec0: 7072 6f6d 7074 223e 496e 266e 6273 703b  prompt">In&nbsp;
+000aced0: 5b37 5d3a 3c2f 6469 763e 0a3c 6469 7620  [7]:</div>.<div 
+000acee0: 636c 6173 733d 226a 702d 436f 6465 4d69  class="jp-CodeMi
+000acef0: 7272 6f72 4564 6974 6f72 206a 702d 4564  rrorEditor jp-Ed
+000acf00: 6974 6f72 206a 702d 496e 7075 7441 7265  itor jp-InputAre
+000acf10: 612d 6564 6974 6f72 2220 6461 7461 2d74  a-editor" data-t
+000acf20: 7970 653d 2269 6e6c 696e 6522 3e0a 2020  ype="inline">.  
+000acf30: 2020 203c 6469 7620 636c 6173 733d 2243     <div class="C
+000acf40: 6f64 654d 6972 726f 7220 636d 2d73 2d6a  odeMirror cm-s-j
+000acf50: 7570 7974 6572 223e 0a3c 6469 7620 636c  upyter">.<div cl
+000acf60: 6173 733d 2220 6869 6768 6c69 6768 7420  ass=" highlight 
+000acf70: 686c 2d69 7079 7468 6f6e 3322 3e3c 7072  hl-ipython3"><pr
+000acf80: 653e 3c73 7061 6e3e 3c2f 7370 616e 3e3c  e><span></span><
+000acf90: 7370 616e 2063 6c61 7373 3d22 6e22 3e64  span class="n">d
+000acfa0: 6174 615f 7061 7468 3c2f 7370 616e 3e20  ata_path</span> 
+000acfb0: 3c73 7061 6e20 636c 6173 733d 226f 223e  <span class="o">
+000acfc0: 3d3c 2f73 7061 6e3e 203c 7370 616e 2063  =</span> <span c
+000acfd0: 6c61 7373 3d22 7331 223e 2623 3339 3b6d  lass="s1">&#39;m
+000acfe0: 6174 6461 7461 2f61 7373 6574 732f 7361  atdata/assets/sa
+000acff0: 6d70 6c65 2f72 616e 646f 6d26 2333 393b  mple/random&#39;
+000ad000: 3c2f 7370 616e 3e0a 0a3c 7370 616e 2063  </span>..<span c
+000ad010: 6c61 7373 3d22 6e22 3e4e 733c 2f73 7061  lass="n">Ns</spa
+000ad020: 6e3e 3c73 7061 6e20 636c 6173 733d 226f  n><span class="o
+000ad030: 223e 3d3c 2f73 7061 6e3e 3c73 7061 6e20  ">=</span><span 
+000ad040: 636c 6173 733d 2270 223e 5b3c 2f73 7061  class="p">[</spa
+000ad050: 6e3e 3c73 7061 6e20 636c 6173 733d 226d  n><span class="m
+000ad060: 6922 3e31 3030 3c2f 7370 616e 3e3c 7370  i">100</span><sp
+000ad070: 616e 2063 6c61 7373 3d22 7022 3e2c 3c2f  an class="p">,</
+000ad080: 7370 616e 3e20 3c73 7061 6e20 636c 6173  span> <span clas
+000ad090: 733d 226d 6922 3e33 3c2f 7370 616e 3e3c  s="mi">3</span><
+000ad0a0: 7370 616e 2063 6c61 7373 3d22 7022 3e5d  span class="p">]
+000ad0b0: 3c2f 7370 616e 3e20 2020 3c73 7061 6e20  </span>   <span 
+000ad0c0: 636c 6173 733d 2263 3122 3e23 204d 696e  class="c1"># Min
+000ad0d0: 2e20 6e75 6d62 6572 206f 6620 7472 616a  . number of traj
+000ad0e0: 6563 746f 7269 6573 3a20 3130 302c 2033  ectories: 100, 3
+000ad0f0: 2073 6361 6c65 7320 2862 7920 6c6f 6720   scales (by log 
+000ad100: 696e 6372 656d 656e 7429 2020 3c2f 7370  increment)  </sp
+000ad110: 616e 3e0a 3c73 7061 6e20 636c 6173 733d  an>.<span class=
+000ad120: 226e 223e 4d73 3c2f 7370 616e 3e3c 7370  "n">Ms</span><sp
+000ad130: 616e 2063 6c61 7373 3d22 6f22 3e3d 3c2f  an class="o">=</
+000ad140: 7370 616e 3e3c 7370 616e 2063 6c61 7373  span><span class
+000ad150: 3d22 7022 3e5b 3c2f 7370 616e 3e3c 7370  ="p">[</span><sp
+000ad160: 616e 2063 6c61 7373 3d22 6d69 223e 3130  an class="mi">10
+000ad170: 3c2f 7370 616e 3e3c 7370 616e 2063 6c61  </span><span cla
+000ad180: 7373 3d22 7022 3e2c 3c2f 7370 616e 3e20  ss="p">,</span> 
+000ad190: 203c 7370 616e 2063 6c61 7373 3d22 6d69   <span class="mi
+000ad1a0: 223e 333c 2f73 7061 6e3e 3c73 7061 6e20  ">3</span><span 
+000ad1b0: 636c 6173 733d 2270 223e 5d3c 2f73 7061  class="p">]</spa
+000ad1c0: 6e3e 2020 203c 7370 616e 2063 6c61 7373  n>   <span class
+000ad1d0: 3d22 6331 223e 2320 4d69 6e2e 206e 756d  ="c1"># Min. num
+000ad1e0: 6265 7220 6f66 2070 6f69 6e74 733a 2031  ber of points: 1
+000ad1f0: 302c 2033 2073 6361 6c65 7320 2862 7920  0, 3 scales (by 
+000ad200: 6c6f 6720 696e 6372 656d 656e 7429 3c2f  log increment)</
+000ad210: 7370 616e 3e0a 3c73 7061 6e20 636c 6173  span>.<span clas
+000ad220: 733d 226e 223e 4c73 3c2f 7370 616e 3e3c  s="n">Ls</span><
+000ad230: 7370 616e 2063 6c61 7373 3d22 6f22 3e3d  span class="o">=
+000ad240: 3c2f 7370 616e 3e3c 7370 616e 2063 6c61  </span><span cla
+000ad250: 7373 3d22 7022 3e5b 3c2f 7370 616e 3e3c  ss="p">[</span><
+000ad260: 7370 616e 2063 6c61 7373 3d22 6d69 223e  span class="mi">
+000ad270: 383c 2f73 7061 6e3e 3c73 7061 6e20 636c  8</span><span cl
+000ad280: 6173 733d 2270 223e 2c3c 2f73 7061 6e3e  ass="p">,</span>
+000ad290: 2020 203c 7370 616e 2063 6c61 7373 3d22     <span class="
+000ad2a0: 6d69 223e 333c 2f73 7061 6e3e 3c73 7061  mi">3</span><spa
+000ad2b0: 6e20 636c 6173 733d 2270 223e 5d3c 2f73  n class="p">]</s
+000ad2c0: 7061 6e3e 2020 203c 7370 616e 2063 6c61  pan>   <span cla
+000ad2d0: 7373 3d22 6331 223e 2320 4d69 6e2e 206e  ss="c1"># Min. n
+000ad2e0: 756d 6265 7220 6f66 2061 7474 7269 6275  umber of attribu
+000ad2f0: 7465 733a 2038 2c20 3320 7363 616c 6573  tes: 8, 3 scales
+000ad300: 2028 6279 206c 6f67 2069 6e63 7265 6d65   (by log increme
+000ad310: 6e74 293c 2f73 7061 6e3e 0a3c 7370 616e  nt)</span>.<span
+000ad320: 2063 6c61 7373 3d22 6e22 3e43 733c 2f73   class="n">Cs</s
+000ad330: 7061 6e3e 3c73 7061 6e20 636c 6173 733d  pan><span class=
+000ad340: 226f 223e 3d3c 2f73 7061 6e3e 3c73 7061  "o">=</span><spa
+000ad350: 6e20 636c 6173 733d 2270 223e 5b3c 2f73  n class="p">[</s
+000ad360: 7061 6e3e 3c73 7061 6e20 636c 6173 733d  pan><span class=
+000ad370: 226d 6922 3e32 3c2f 7370 616e 3e3c 7370  "mi">2</span><sp
+000ad380: 616e 2063 6c61 7373 3d22 7022 3e2c 3c2f  an class="p">,</
+000ad390: 7370 616e 3e20 2020 3c73 7061 6e20 636c  span>   <span cl
+000ad3a0: 6173 733d 226d 6922 3e33 3c2f 7370 616e  ass="mi">3</span
+000ad3b0: 3e3c 7370 616e 2063 6c61 7373 3d22 7022  ><span class="p"
+000ad3c0: 3e5d 3c2f 7370 616e 3e20 2020 3c73 7061  >]</span>   <spa
+000ad3d0: 6e20 636c 6173 733d 2263 3122 3e23 204d  n class="c1"># M
+000ad3e0: 696e 2e20 6e75 6d62 6572 206f 6620 6c61  in. number of la
+000ad3f0: 6265 6c73 3a20 322c 2033 2073 6361 6c65  bels: 2, 3 scale
+000ad400: 7320 2862 7920 6c6f 6720 696e 6372 656d  s (by log increm
+000ad410: 656e 7429 3c2f 7370 616e 3e0a 0a3c 7370  ent)</span>..<sp
+000ad420: 616e 2063 6c61 7373 3d22 6e22 3e73 6361  an class="n">sca
+000ad430: 6c65 7252 616e 646f 6d47 656e 6572 6174  lerRandomGenerat
+000ad440: 6f72 3c2f 7370 616e 3e3c 7370 616e 2063  or</span><span c
+000ad450: 6c61 7373 3d22 7022 3e28 3c2f 7370 616e  lass="p">(</span
+000ad460: 3e3c 7370 616e 2063 6c61 7373 3d22 6e22  ><span class="n"
+000ad470: 3e4e 733c 2f73 7061 6e3e 3c73 7061 6e20  >Ns</span><span 
+000ad480: 636c 6173 733d 2270 223e 2c3c 2f73 7061  class="p">,</spa
+000ad490: 6e3e 203c 7370 616e 2063 6c61 7373 3d22  n> <span class="
+000ad4a0: 6e22 3e4d 733c 2f73 7061 6e3e 3c73 7061  n">Ms</span><spa
+000ad4b0: 6e20 636c 6173 733d 2270 223e 2c3c 2f73  n class="p">,</s
+000ad4c0: 7061 6e3e 203c 7370 616e 2063 6c61 7373  pan> <span class
+000ad4d0: 3d22 6e22 3e4c 733c 2f73 7061 6e3e 3c73  ="n">Ls</span><s
+000ad4e0: 7061 6e20 636c 6173 733d 2270 223e 2c3c  pan class="p">,<
+000ad4f0: 2f73 7061 6e3e 203c 7370 616e 2063 6c61  /span> <span cla
+000ad500: 7373 3d22 6e22 3e43 733c 2f73 7061 6e3e  ss="n">Cs</span>
+000ad510: 3c73 7061 6e20 636c 6173 733d 2270 223e  <span class="p">
+000ad520: 2c3c 2f73 7061 6e3e 203c 7370 616e 2063  ,</span> <span c
+000ad530: 6c61 7373 3d22 6e22 3e73 6176 655f 746f  lass="n">save_to
+000ad540: 3c2f 7370 616e 3e3c 7370 616e 2063 6c61  </span><span cla
+000ad550: 7373 3d22 6f22 3e3d 3c2f 7370 616e 3e3c  ss="o">=</span><
+000ad560: 7370 616e 2063 6c61 7373 3d22 6e22 3e64  span class="n">d
+000ad570: 6174 615f 7061 7468 3c2f 7370 616e 3e3c  ata_path</span><
+000ad580: 7370 616e 2063 6c61 7373 3d22 7022 3e29  span class="p">)
+000ad590: 3c2f 7370 616e 3e0a 3c2f 7072 653e 3c2f  </span>.</pre></
+000ad5a0: 6469 763e 0a0a 2020 2020 203c 2f64 6976  div>..     </div
+000ad5b0: 3e0a 3c2f 6469 763e 0a3c 2f64 6976 3e0a  >.</div>.</div>.
+000ad5c0: 3c2f 6469 763e 0a0a 3c64 6976 2063 6c61  </div>..<div cla
+000ad5d0: 7373 3d22 6a70 2d43 656c 6c2d 6f75 7470  ss="jp-Cell-outp
+000ad5e0: 7574 5772 6170 7065 7222 3e0a 3c64 6976  utWrapper">.<div
+000ad5f0: 2063 6c61 7373 3d22 6a70 2d43 6f6c 6c61   class="jp-Colla
+000ad600: 7073 6572 206a 702d 4f75 7470 7574 436f  pser jp-OutputCo
+000ad610: 6c6c 6170 7365 7220 6a70 2d43 656c 6c2d  llapser jp-Cell-
+000ad620: 6f75 7470 7574 436f 6c6c 6170 7365 7222  outputCollapser"
+000ad630: 3e0a 3c2f 6469 763e 0a0a 0a3c 6469 7620  >.</div>...<div 
+000ad640: 636c 6173 733d 226a 702d 4f75 7470 7574  class="jp-Output
+000ad650: 4172 6561 206a 702d 4365 6c6c 2d6f 7574  Area jp-Cell-out
+000ad660: 7075 7441 7265 6122 3e0a 0a3c 6469 7620  putArea">..<div 
+000ad670: 636c 6173 733d 226a 702d 4f75 7470 7574  class="jp-Output
+000ad680: 4172 6561 2d63 6869 6c64 223e 0a0a 2020  Area-child">..  
+000ad690: 2020 0a20 2020 203c 6469 7620 636c 6173    .    <div clas
+000ad6a0: 733d 226a 702d 4f75 7470 7574 5072 6f6d  s="jp-OutputProm
+000ad6b0: 7074 206a 702d 4f75 7470 7574 4172 6561  pt jp-OutputArea
+000ad6c0: 2d70 726f 6d70 7422 3e3c 2f64 6976 3e0a  -prompt"></div>.
+000ad6d0: 0a0a 0a0a 3c64 6976 2063 6c61 7373 3d22  ....<div class="
+000ad6e0: 6a70 2d52 656e 6465 7265 6454 6578 7420  jp-RenderedText 
+000ad6f0: 6a70 2d4f 7574 7075 7441 7265 612d 6f75  jp-OutputArea-ou
+000ad700: 7470 7574 2022 2064 6174 612d 6d69 6d65  tput " data-mime
+000ad710: 2d74 7970 653d 2274 6578 742f 706c 6169  -type="text/plai
+000ad720: 6e22 3e0a 3c70 7265 3e20 2030 257c 2020  n">.<pre>  0%|  
+000ad730: 2020 2020 2020 2020 7c20 302f 3132 205b          | 0/12 [
+000ad740: 3030 3a30 3026 6c74 3b3f 2c20 3f69 742f  00:00&lt;?, ?it/
+000ad750: 735d 3c2f 7072 653e 0a3c 2f64 6976 3e0a  s]</pre>.</div>.
+000ad760: 0a3c 2f64 6976 3e0a 0a3c 6469 7620 636c  .</div>..<div cl
+000ad770: 6173 733d 226a 702d 4f75 7470 7574 4172  ass="jp-OutputAr
+000ad780: 6561 2d63 6869 6c64 223e 0a0a 2020 2020  ea-child">..    
+000ad790: 0a20 2020 203c 6469 7620 636c 6173 733d  .    <div class=
+000ad7a0: 226a 702d 4f75 7470 7574 5072 6f6d 7074  "jp-OutputPrompt
+000ad7b0: 206a 702d 4f75 7470 7574 4172 6561 2d70   jp-OutputArea-p
+000ad7c0: 726f 6d70 7422 3e3c 2f64 6976 3e0a 0a0a  rompt"></div>...
+000ad7d0: 3c64 6976 2063 6c61 7373 3d22 6a70 2d52  <div class="jp-R
+000ad7e0: 656e 6465 7265 6454 6578 7420 6a70 2d4f  enderedText jp-O
+000ad7f0: 7574 7075 7441 7265 612d 6f75 7470 7574  utputArea-output
+000ad800: 2220 6461 7461 2d6d 696d 652d 7479 7065  " data-mime-type
+000ad810: 3d22 7465 7874 2f70 6c61 696e 223e 0a3c  ="text/plain">.<
+000ad820: 7072 653e 4e20 3a3a 2066 6978 2e20 7661  pre>N :: fix. va
+000ad830: 6c75 653a 2009 2032 3030 2009 7363 616c  lue: . 200 .scal
+000ad840: 653a 0920 5b31 3030 2c20 3230 302c 2034  e:. [100, 200, 4
+000ad850: 3030 5d0a 4d20 3a3a 2066 6978 2e20 7661  00].M :: fix. va
+000ad860: 6c75 653a 2009 2032 3020 0973 6361 6c65  lue: . 20 .scale
+000ad870: 3a09 205b 3130 2c20 3230 2c20 3430 5d0a  :. [10, 20, 40].
+000ad880: 4c20 3a3a 2066 6978 2e20 7661 6c75 653a  L :: fix. value:
+000ad890: 2009 2038 2009 7363 616c 653a 0920 5b38   . 8 .scale:. [8
+000ad8a0: 2c20 3136 2c20 3332 5d0a 4320 3a3a 2066  , 16, 32].C :: f
+000ad8b0: 6978 2e20 7661 6c75 653a 2009 2034 2009  ix. value: . 4 .
+000ad8c0: 7363 616c 653a 0920 5b32 2c20 342c 2038  scale:. [2, 4, 8
+000ad8d0: 5d0a 5772 6974 696e 6720 2d20 4353 5620  ].Writing - CSV 
+000ad8e0: 7c0a 5772 6974 696e 6720 2d20 4353 5620  |.Writing - CSV 
+000ad8f0: 7c0a 5772 6974 696e 6720 2d20 4353 5620  |.Writing - CSV 
+000ad900: 7c0a 5772 6974 696e 6720 2d20 4353 5620  |.Writing - CSV 
+000ad910: 7c0a 5772 6974 696e 6720 2d20 4353 5620  |.Writing - CSV 
+000ad920: 7c0a 5772 6974 696e 6720 2d20 4353 5620  |.Writing - CSV 
+000ad930: 7c0a 5772 6974 696e 6720 2d20 4353 5620  |.Writing - CSV 
+000ad940: 7c0a 5772 6974 696e 6720 2d20 4353 5620  |.Writing - CSV 
+000ad950: 7c0a 5772 6974 696e 6720 2d20 4353 5620  |.Writing - CSV 
+000ad960: 7c0a 3c2f 7072 653e 0a3c 2f64 6976 3e0a  |.</pre>.</div>.
+000ad970: 3c2f 6469 763e 0a0a 3c2f 6469 763e 0a0a  </div>..</div>..
+000ad980: 3c2f 6469 763e 0a0a 3c2f 6469 763e 0a3c  </div>..</div>.<
+000ad990: 6469 7620 636c 6173 733d 226a 702d 4365  div class="jp-Ce
+000ad9a0: 6c6c 206a 702d 4d61 726b 646f 776e 4365  ll jp-MarkdownCe
+000ad9b0: 6c6c 206a 702d 4e6f 7465 626f 6f6b 2d63  ll jp-Notebook-c
+000ad9c0: 656c 6c22 3e0a 3c64 6976 2063 6c61 7373  ell">.<div class
+000ad9d0: 3d22 6a70 2d43 656c 6c2d 696e 7075 7457  ="jp-Cell-inputW
+000ad9e0: 7261 7070 6572 223e 0a3c 6469 7620 636c  rapper">.<div cl
+000ad9f0: 6173 733d 226a 702d 436f 6c6c 6170 7365  ass="jp-Collapse
+000ada00: 7220 6a70 2d49 6e70 7574 436f 6c6c 6170  r jp-InputCollap
+000ada10: 7365 7220 6a70 2d43 656c 6c2d 696e 7075  ser jp-Cell-inpu
+000ada20: 7443 6f6c 6c61 7073 6572 223e 0a3c 2f64  tCollapser">.</d
+000ada30: 6976 3e0a 3c64 6976 2063 6c61 7373 3d22  iv>.<div class="
+000ada40: 6a70 2d49 6e70 7574 4172 6561 206a 702d  jp-InputArea jp-
+000ada50: 4365 6c6c 2d69 6e70 7574 4172 6561 223e  Cell-inputArea">
+000ada60: 3c64 6976 2063 6c61 7373 3d22 6a70 2d49  <div class="jp-I
+000ada70: 6e70 7574 5072 6f6d 7074 206a 702d 496e  nputPrompt jp-In
+000ada80: 7075 7441 7265 612d 7072 6f6d 7074 223e  putArea-prompt">
+000ada90: 0a3c 2f64 6976 3e3c 6469 7620 636c 6173  .</div><div clas
+000adaa0: 733d 226a 702d 5265 6e64 6572 6564 4854  s="jp-RenderedHT
+000adab0: 4d4c 436f 6d6d 6f6e 206a 702d 5265 6e64  MLCommon jp-Rend
+000adac0: 6572 6564 4d61 726b 646f 776e 206a 702d  eredMarkdown jp-
+000adad0: 4d61 726b 646f 776e 4f75 7470 7574 2022  MarkdownOutput "
+000adae0: 2064 6174 612d 6d69 6d65 2d74 7970 653d   data-mime-type=
+000adaf0: 2274 6578 742f 6d61 726b 646f 776e 223e  "text/markdown">
+000adb00: 0a3c 6872 3e0a 0a3c 2f64 6976 3e0a 3c2f  .<hr>..</div>.</
+000adb10: 6469 763e 0a3c 2f64 6976 3e0a 3c2f 6469  div>.</div>.</di
+000adb20: 763e 0a3c 6469 7620 636c 6173 733d 226a  v>.<div class="j
+000adb30: 702d 4365 6c6c 206a 702d 4d61 726b 646f  p-Cell jp-Markdo
+000adb40: 776e 4365 6c6c 206a 702d 4e6f 7465 626f  wnCell jp-Notebo
+000adb50: 6f6b 2d63 656c 6c22 3e0a 3c64 6976 2063  ok-cell">.<div c
+000adb60: 6c61 7373 3d22 6a70 2d43 656c 6c2d 696e  lass="jp-Cell-in
+000adb70: 7075 7457 7261 7070 6572 223e 0a3c 6469  putWrapper">.<di
+000adb80: 7620 636c 6173 733d 226a 702d 436f 6c6c  v class="jp-Coll
+000adb90: 6170 7365 7220 6a70 2d49 6e70 7574 436f  apser jp-InputCo
+000adba0: 6c6c 6170 7365 7220 6a70 2d43 656c 6c2d  llapser jp-Cell-
+000adbb0: 696e 7075 7443 6f6c 6c61 7073 6572 223e  inputCollapser">
+000adbc0: 0a3c 2f64 6976 3e0a 3c64 6976 2063 6c61  .</div>.<div cla
+000adbd0: 7373 3d22 6a70 2d49 6e70 7574 4172 6561  ss="jp-InputArea
+000adbe0: 206a 702d 4365 6c6c 2d69 6e70 7574 4172   jp-Cell-inputAr
+000adbf0: 6561 223e 3c64 6976 2063 6c61 7373 3d22  ea"><div class="
+000adc00: 6a70 2d49 6e70 7574 5072 6f6d 7074 206a  jp-InputPrompt j
+000adc10: 702d 496e 7075 7441 7265 612d 7072 6f6d  p-InputArea-prom
+000adc20: 7074 223e 0a3c 2f64 6976 3e3c 6469 7620  pt">.</div><div 
+000adc30: 636c 6173 733d 226a 702d 5265 6e64 6572  class="jp-Render
+000adc40: 6564 4854 4d4c 436f 6d6d 6f6e 206a 702d  edHTMLCommon jp-
+000adc50: 5265 6e64 6572 6564 4d61 726b 646f 776e  RenderedMarkdown
+000adc60: 206a 702d 4d61 726b 646f 776e 4f75 7470   jp-MarkdownOutp
+000adc70: 7574 2022 2064 6174 612d 6d69 6d65 2d74  ut " data-mime-t
+000adc80: 7970 653d 2274 6578 742f 6d61 726b 646f  ype="text/markdo
+000adc90: 776e 223e 0a3c 703e 2320 4279 2054 6172  wn">.<p># By Tar
+000adca0: 6c69 7320 506f 7274 656c 6120 2832 3032  lis Portela (202
+000adcb0: 3329 3c2f 703e 0a0a 3c2f 6469 763e 0a3c  3)</p>..</div>.<
+000adcc0: 2f64 6976 3e0a 3c2f 6469 763e 0a3c 2f64  /div>.</div>.</d
+000adcd0: 6976 3e0a 3c2f 626f 6479 3e0a 0a0a 0a0a  iv>.</body>.....
+000adce0: 0a0a 0a3c 2f68 746d 6c3e 0a              ...</html>.
```

#### html2text {}

```diff
@@ -1,119 +1,984 @@
-************ MMAATT--ddaattaa:: DDaattaa PPrreepprroocceessssiinngg ffoorr MMuullttiippllee AAssppeecctt TTrraajjeeccttoorryy DDaattaa MMiinniinngg
-[[MMAATT--TToooollss FFrraammeewwoorrkk]]_?¶ ************
+************ MMAATT--ddaattaa:: DDaattaa HHaannddlleerr ffoorr MMuullttiippllee AAssppeecctt TTrraajjeeccttoorryy DDaattaa MMiinniinngg [[MMAATT--
+TToooollss FFrraammeewwoorrkk]]_?¶ ************
 Sample Code in python notebook to use mat-data as a python library.
 The present package offers a tool, to support the user in the task of data
 preprocessing of multiple aspect trajectories, or to generating synthetic
 datasets. It integrates into a unique framework for multiple aspects
 trajectories and in general for multidimensional sequence data mining methods.
 Created on Dec, 2023 Copyright (C) 2023, License GPL Version 3 or superior (see
 LICENSE file)
-In [1]:
-import sys, os
+In [ ]:
+!pip install mat-data
+#!pip install --upgrade mat-data
+******** 11.. RReeaaddiinngg llooccaall ddaattaa_?¶ ********
+Sample code for trajectory dataset read from local files
+The easy way to read data is to load a csv file in pandas, such as:
+In [8]:
+import pandas as pd
+
+data_path = 'matdata/assets/sample'
+
+pd.read_csv(data_path + '/Foursquare_Sample.csv')
+Out[8]:
+ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ 
+|_ _ _ _ _ _|_ _ _tt_ii_dd_|_ _ _ _ _ _ _ _ _ _ll_aa_tt____ll_oo_nn_|_dd_aa_tt_ee____tt_ii_mm_ee_|_tt_ii_mm_ee_|_rr_aa_tt_ii_nn_gg_|_pp_rr_ii_cc_ee_|_ww_ee_aa_tt_hh_ee_rr_|_ _ _ _ _ _dd_aa_yy_|_ _rr_oo_oo_tt____tt_yy_pp_ee_|_ _ _ _ _ _ _tt_yy_pp_ee|
+|     |     |40.8331652006224|2012-11- |    |      |     |       |        |          |Home      |
+|00    |126  |-               |12 05:17:|317 |-1.0  |-1   |Clear  |Monday  |Residence |(private) |
+|_ _ _ _ _ _|_ _ _ _ _ _|_7_3_._9_4_1_8_6_0_3_4_2_7_6_9_2_|_1_8_ _ _ _ _ _ _ _|_ _ _ _ _|_ _ _ _ _ _ _|_ _ _ _ _ _|_ _ _ _ _ _ _ _|_ _ _ _ _ _ _ _ _|_ _ _ _ _ _ _ _ _ _ _|_ _ _ _ _ _ _ _ _ _ |
+|     |     |40.8340978041072|2012-11- |    |      |     |       |        |          |Deli /    |
+|11    |126  |-               |12 23:24:|1404|8.2   |1    |Clouds |Monday  |Food      |Bodega    |
+|_ _ _ _ _ _|_ _ _ _ _ _|_7_3_._9_4_5_2_6_7_2_2_2_5_8_8_1_|_5_5_ _ _ _ _ _ _ _|_ _ _ _ _|_ _ _ _ _ _ _|_ _ _ _ _ _|_ _ _ _ _ _ _ _|_ _ _ _ _ _ _ _ _|_ _ _ _ _ _ _ _ _ _ _|_ _ _ _ _ _ _ _ _ _ |
+|     |     |40.8331652006224|2012-11- |    |      |     |       |        |          |Home      |
+|22    |126  |-               |13 00:00:|0   |-1.0  |-1   |Clouds |Tuesday |Residence |(private) |
+|_ _ _ _ _ _|_ _ _ _ _ _|_7_3_._9_4_1_8_6_0_3_4_2_7_6_9_2_|_0_7_ _ _ _ _ _ _ _|_ _ _ _ _|_ _ _ _ _ _ _|_ _ _ _ _ _|_ _ _ _ _ _ _ _|_ _ _ _ _ _ _ _ _|_ _ _ _ _ _ _ _ _ _ _|_ _ _ _ _ _ _ _ _ _ |
+|     |     |40.7646959283254|2012-11- |    |      |     |       |        |          |Fried     |
+|33    |126  |-               |15 17:49:|1069|6.6   |3    |Clear  |Thursday|Food      |Chicken   |
+|_ _ _ _ _ _|_ _ _ _ _ _|_7_3_._8_8_5_1_9_7_4_9_6_4_4_1_4_|_0_1_ _ _ _ _ _ _ _|_ _ _ _ _|_ _ _ _ _ _ _|_ _ _ _ _ _|_ _ _ _ _ _ _ _|_ _ _ _ _ _ _ _ _|_ _ _ _ _ _ _ _ _ _ _|_J_o_i_n_t_ _ _ _ _ |
+|     |     |40.7660790376824|2012-11- |    |      |     |       |        |Travel &  |Bus       |
+|44    |126  |-               |15 18:40:|1120|-1.0  |-1   |Clear  |Thursday|Transport |Station   |
+|_ _ _ _ _ _|_ _ _ _ _ _|_7_3_._8_8_3_5_2_8_7_0_9_4_1_1_6_|_1_6_ _ _ _ _ _ _ _|_ _ _ _ _|_ _ _ _ _ _ _|_ _ _ _ _ _|_ _ _ _ _ _ _ _|_ _ _ _ _ _ _ _ _|_ _ _ _ _ _ _ _ _ _ _|_ _ _ _ _ _ _ _ _ _ |
+|_.._.._.._ _ _|_._._._ _ _|_._._._ _ _ _ _ _ _ _ _ _ _ _ _ _|_._._._ _ _ _ _ _ _|_._._._ _|_._._._ _ _ _|_._._._ _ _|_._._._ _ _ _ _|_._._._ _ _ _ _ _|_._._._ _ _ _ _ _ _ _|_._._._ _ _ _ _ _ _ |
+|     |     |40.7047332789043|2012-08- |    |      |     |       |        |College & |General   |
+|6666995577|29563|-               |10 17:17:|1037|-1.0  |-1   |Clouds |Friday  |University|College & |
+|_ _ _ _ _ _|_ _ _ _ _ _|_7_3_._9_8_7_7_3_7_8_9_4_0_5_8_2_|_3_7_ _ _ _ _ _ _ _|_ _ _ _ _|_ _ _ _ _ _ _|_ _ _ _ _ _|_ _ _ _ _ _ _ _|_ _ _ _ _ _ _ _ _|_ _ _ _ _ _ _ _ _ _ _|_U_n_i_v_e_r_s_i_t_y|
+|     |     |40.6951627360199|2012-08- |    |      |     |       |        |          |Thai      |
+|6666995588|29563|-               |10 20:10:|1210|8.0   |2    |Clouds |Friday  |Food      |Restaurant|
+|_ _ _ _ _ _|_ _ _ _ _ _|_7_3_._9_9_5_4_4_7_8_6_9_1_0_7_2_|_5_9_ _ _ _ _ _ _ _|_ _ _ _ _|_ _ _ _ _ _ _|_ _ _ _ _ _|_ _ _ _ _ _ _ _|_ _ _ _ _ _ _ _ _|_ _ _ _ _ _ _ _ _ _ _|_ _ _ _ _ _ _ _ _ _ |
+|     |     |40.6978026652822|2012-08- |    |      |     |       |        |Outdoors &|          |
+|6666995599|29563|-               |11 08:01:|481 |6.9   |-1   |Clouds |Saturday|Recreation|Gym       |
+|_ _ _ _ _ _|_ _ _ _ _ _|_7_3_._9_9_4_1_4_5_1_6_3_0_3_1_4_|_2_0_ _ _ _ _ _ _ _|_ _ _ _ _|_ _ _ _ _ _ _|_ _ _ _ _ _|_ _ _ _ _ _ _ _|_ _ _ _ _ _ _ _ _|_ _ _ _ _ _ _ _ _ _ _|_ _ _ _ _ _ _ _ _ _ |
+|     |     |40.6946728967503|2012-08- |    |      |     |       |        |          |Coffee    |
+|6666996600|29563|-               |11 13:39:|819 |7.0   |1    |Clouds |Saturday|Food      |Shop      |
+|_ _ _ _ _ _|_ _ _ _ _ _|_7_3_._9_9_4_0_8_2_0_3_6_0_8_0_5_|_3_9_ _ _ _ _ _ _ _|_ _ _ _ _|_ _ _ _ _ _ _|_ _ _ _ _ _|_ _ _ _ _ _ _ _|_ _ _ _ _ _ _ _ _|_ _ _ _ _ _ _ _ _ _ _|_ _ _ _ _ _ _ _ _ _ |
+|     |     |40.6978026652822|2012-08- |    |      |     |       |        |Outdoors &|          |
+|6666996611|29563|-               |12 07:56:|476 |6.9   |-1   |Clouds |Sunday  |Recreation|Gym       |
+|_ _ _ _ _ _|_ _ _ _ _ _|_7_3_._9_9_4_1_4_5_1_6_3_0_3_1_4_|_2_6_ _ _ _ _ _ _ _|_ _ _ _ _|_ _ _ _ _ _ _|_ _ _ _ _ _|_ _ _ _ _ _ _ _|_ _ _ _ _ _ _ _ _|_ _ _ _ _ _ _ _ _ _ _|_ _ _ _ _ _ _ _ _ _ |
+66962 rows × 10 columns
+mat-data provides modules to handle dataset reading in standard ways:
+a) Read a dataset locally:
+
+This is an example for .csv file, however this can read .csv, .parquet, .zip,
+.ts, and .xes file formats.
+In [9]:
+from matdata.dataset import *
+In [10]:
+df = read_ds('matdata/assets/sample/Foursquare_Sample.csv')
+df.head()
+Out[10]:
+ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ 
+|_ _|_ _ _ _ _ _ _ _ _ _ll_aa_tt____ll_oo_nn_|_dd_aa_tt_ee____tt_ii_mm_ee_|_tt_ii_mm_ee_|_rr_aa_tt_ii_nn_gg_|_pp_rr_ii_cc_ee_|_ww_ee_aa_tt_hh_ee_rr_|_ _ _ _ _ _dd_aa_yy_|_rr_oo_oo_tt____tt_yy_pp_ee_|_ _ _ _ _ _tt_yy_pp_ee_|_tt_ii_dd|
+| |40.8331652006224|2012-11- |    |      |     |       |        |         |Home     |   |
+|00|-               |12 05:17:|317 |-1.0  |-1   |Clear  |Monday  |Residence|(private)|126|
+|_ _|_7_3_._9_4_1_8_6_0_3_4_2_7_6_9_2_|_1_8_ _ _ _ _ _ _ _|_ _ _ _ _|_ _ _ _ _ _ _|_ _ _ _ _ _|_ _ _ _ _ _ _ _|_ _ _ _ _ _ _ _ _|_ _ _ _ _ _ _ _ _ _|_ _ _ _ _ _ _ _ _ _|_ _ _ |
+| |40.8340978041072|2012-11- |    |      |     |       |        |         |Deli /   |   |
+|11|-               |12 23:24:|1404|8.2   |1    |Clouds |Monday  |Food     |Bodega   |126|
+|_ _|_7_3_._9_4_5_2_6_7_2_2_2_5_8_8_1_|_5_5_ _ _ _ _ _ _ _|_ _ _ _ _|_ _ _ _ _ _ _|_ _ _ _ _ _|_ _ _ _ _ _ _ _|_ _ _ _ _ _ _ _ _|_ _ _ _ _ _ _ _ _ _|_ _ _ _ _ _ _ _ _ _|_ _ _ |
+| |40.8331652006224|2012-11- |    |      |     |       |        |         |Home     |   |
+|22|-               |13 00:00:|0   |-1.0  |-1   |Clouds |Tuesday |Residence|(private)|126|
+|_ _|_7_3_._9_4_1_8_6_0_3_4_2_7_6_9_2_|_0_7_ _ _ _ _ _ _ _|_ _ _ _ _|_ _ _ _ _ _ _|_ _ _ _ _ _|_ _ _ _ _ _ _ _|_ _ _ _ _ _ _ _ _|_ _ _ _ _ _ _ _ _ _|_ _ _ _ _ _ _ _ _ _|_ _ _ |
+| |40.7646959283254|2012-11- |    |      |     |       |        |         |Fried    |   |
+|33|-               |15 17:49:|1069|6.6   |3    |Clear  |Thursday|Food     |Chicken  |126|
+|_ _|_7_3_._8_8_5_1_9_7_4_9_6_4_4_1_4_|_0_1_ _ _ _ _ _ _ _|_ _ _ _ _|_ _ _ _ _ _ _|_ _ _ _ _ _|_ _ _ _ _ _ _ _|_ _ _ _ _ _ _ _ _|_ _ _ _ _ _ _ _ _ _|_J_o_i_n_t_ _ _ _ _|_ _ _ |
+| |40.7660790376824|2012-11- |    |      |     |       |        |Travel & |Bus      |   |
+|44|-               |15 18:40:|1120|-1.0  |-1   |Clear  |Thursday|Transport|Station  |126|
+|_ _|_7_3_._8_8_3_5_2_8_7_0_9_4_1_1_6_|_1_6_ _ _ _ _ _ _ _|_ _ _ _ _|_ _ _ _ _ _ _|_ _ _ _ _ _|_ _ _ _ _ _ _ _|_ _ _ _ _ _ _ _ _|_ _ _ _ _ _ _ _ _ _|_ _ _ _ _ _ _ _ _ _|_ _ _ |
+Optionally, you can use the standardized reading, which will make 'tid'/'label'
+nomenclature (or rename columns) and will sort the trajectories
+In [11]:
+df = read_ds('matdata/assets/sample/Foursquare_Sample.csv', tid_col='tid',
+class_col='root_type')
+df.head()
+Out[11]:
+ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ 
+|_ _|_ _ _ _ _ _ _ _ _ _ll_aa_tt____ll_oo_nn_|_dd_aa_tt_ee____tt_ii_mm_ee_|_tt_ii_mm_ee_|_rr_aa_tt_ii_nn_gg_|_pp_rr_ii_cc_ee_|_ww_ee_aa_tt_hh_ee_rr_|_ _ _ _ _ _dd_aa_yy_|_ _ _ _ _ _tt_yy_pp_ee_|_tt_ii_dd_|_ _ _ _ _ll_aa_bb_ee_ll|
+| |40.8331652006224|2012-11- |    |      |     |       |        |Home     |   |         |
+|00|-               |12 05:17:|317 |-1.0  |-1   |Clear  |Monday  |(private)|126|Residence|
+|_ _|_7_3_._9_4_1_8_6_0_3_4_2_7_6_9_2_|_1_8_ _ _ _ _ _ _ _|_ _ _ _ _|_ _ _ _ _ _ _|_ _ _ _ _ _|_ _ _ _ _ _ _ _|_ _ _ _ _ _ _ _ _|_ _ _ _ _ _ _ _ _ _|_ _ _ _|_ _ _ _ _ _ _ _ _ |
+| |40.8340978041072|2012-11- |    |      |     |       |        |Deli /   |   |         |
+|11|-               |12 23:24:|1404|8.2   |1    |Clouds |Monday  |Bodega   |126|Food     |
+|_ _|_7_3_._9_4_5_2_6_7_2_2_2_5_8_8_1_|_5_5_ _ _ _ _ _ _ _|_ _ _ _ _|_ _ _ _ _ _ _|_ _ _ _ _ _|_ _ _ _ _ _ _ _|_ _ _ _ _ _ _ _ _|_ _ _ _ _ _ _ _ _ _|_ _ _ _|_ _ _ _ _ _ _ _ _ |
+| |40.8331652006224|2012-11- |    |      |     |       |        |Home     |   |         |
+|22|-               |13 00:00:|0   |-1.0  |-1   |Clouds |Tuesday |(private)|126|Residence|
+|_ _|_7_3_._9_4_1_8_6_0_3_4_2_7_6_9_2_|_0_7_ _ _ _ _ _ _ _|_ _ _ _ _|_ _ _ _ _ _ _|_ _ _ _ _ _|_ _ _ _ _ _ _ _|_ _ _ _ _ _ _ _ _|_ _ _ _ _ _ _ _ _ _|_ _ _ _|_ _ _ _ _ _ _ _ _ |
+| |40.7646959283254|2012-11- |    |      |     |       |        |Fried    |   |         |
+|33|-               |15 17:49:|1069|6.6   |3    |Clear  |Thursday|Chicken  |126|Food     |
+|_ _|_7_3_._8_8_5_1_9_7_4_9_6_4_4_1_4_|_0_1_ _ _ _ _ _ _ _|_ _ _ _ _|_ _ _ _ _ _ _|_ _ _ _ _ _|_ _ _ _ _ _ _ _|_ _ _ _ _ _ _ _ _|_J_o_i_n_t_ _ _ _ _|_ _ _ _|_ _ _ _ _ _ _ _ _ |
+| |40.7660790376824|2012-11- |    |      |     |       |        |Bus      |   |Travel & |
+|44|-               |15 18:40:|1120|-1.0  |-1   |Clear  |Thursday|Station  |126|Transport|
+|_ _|_7_3_._8_8_3_5_2_8_7_0_9_4_1_1_6_|_1_6_ _ _ _ _ _ _ _|_ _ _ _ _|_ _ _ _ _ _ _|_ _ _ _ _ _|_ _ _ _ _ _ _ _|_ _ _ _ _ _ _ _ _|_ _ _ _ _ _ _ _ _ _|_ _ _ _|_ _ _ _ _ _ _ _ _ |
+******** 22.. LLooaaddiinngg RReeppoossiittoorryy DDaattaa_?¶ ********
+This module loads data from public repository _G_i_t_:_ _m_a_t_-_a_n_a_l_y_s_i_s_ _d_a_t_a_s_e_t_s_ _(_v_2___0_)
+Check the GitHub repository to see available datasets.
+To use helpers for data loading, import from package matdata.dataset:
+In [12]:
+from matdata.dataset import *
+a) First, you can load datasets by informing the category (parent folder) and
+dataset name (subfolder):
+In [13]:
+# dataset='mat.FoursquareNYC' ## => dafault
+
+df = load_ds(sample_size=0.25)
+df
+Loading dataset file: https://github.com/mat-analysis/datasets/raw/main/mat/
+FoursquareNYC/
+  0%|          | 0/193 [00:00<?, ?it/s]
+Out[13]:
+ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ 
+|_ _ _ _ _ _|_ _ _ _ _ _ _ll_aa_tt_|_ _ _ _ _ _ _ll_oo_nn_|_ _ _ _ _ _dd_aa_yy_|_hh_oo_uu_rr_|_ _ _pp_oo_ii_|_ _ _cc_aa_tt_ee_gg_oo_rr_yy_|_pp_rr_ii_cc_ee_|_rr_aa_tt_ii_nn_gg_|_ww_ee_aa_tt_hh_ee_rr_|_ _ _tt_ii_dd_|_ll_aa_bb_ee_ll|
+|00    |40.834098|-        |Monday  |13  |21580|Food      |1    |8.2   |Clouds |127  |6    |
+|_ _ _ _ _ _|_ _ _ _ _ _ _ _ _ _|_7_3_._9_4_5_2_6_7_|_ _ _ _ _ _ _ _ _|_ _ _ _ _|_ _ _ _ _ _|_ _ _ _ _ _ _ _ _ _ _|_ _ _ _ _ _|_ _ _ _ _ _ _|_ _ _ _ _ _ _ _|_ _ _ _ _ _|_ _ _ _ _ |
+|11    |40.567196|-        |Monday  |19  |2392 |Travel &  |-999 |-999.0|Clouds |127  |6    |
+|_ _ _ _ _ _|_ _ _ _ _ _ _ _ _ _|_7_3_._8_8_2_5_7_6_|_ _ _ _ _ _ _ _ _|_ _ _ _ _|_ _ _ _ _ _|_T_r_a_n_s_p_o_r_t_ _|_ _ _ _ _ _|_ _ _ _ _ _ _|_ _ _ _ _ _ _ _|_ _ _ _ _ _|_ _ _ _ _ |
+|22    |40.689913|-        |Monday  |23  |35589|Travel &  |-999 |-999.0|Clouds |127  |6    |
+|_ _ _ _ _ _|_ _ _ _ _ _ _ _ _ _|_7_3_._9_8_1_5_0_4_|_ _ _ _ _ _ _ _ _|_ _ _ _ _|_ _ _ _ _ _|_T_r_a_n_s_p_o_r_t_ _|_ _ _ _ _ _|_ _ _ _ _ _ _|_ _ _ _ _ _ _ _|_ _ _ _ _ _|_ _ _ _ _ |
+|33    |40.708588|-        |Monday  |23  |18603|Travel &  |-999 |-999.0|Clouds |127  |6    |
+|_ _ _ _ _ _|_ _ _ _ _ _ _ _ _ _|_7_3_._9_9_1_0_3_2_|_ _ _ _ _ _ _ _ _|_ _ _ _ _|_ _ _ _ _ _|_T_r_a_n_s_p_o_r_t_ _|_ _ _ _ _ _|_ _ _ _ _ _ _|_ _ _ _ _ _ _ _|_ _ _ _ _ _|_ _ _ _ _ |
+|44    |40.833165|-        |Tuesday |14  |36348|Residence |-999 |-999.0|Clear  |127  |6    |
+|_ _ _ _ _ _|_ _ _ _ _ _ _ _ _ _|_7_3_._9_4_1_8_6_0_|_ _ _ _ _ _ _ _ _|_ _ _ _ _|_ _ _ _ _ _|_ _ _ _ _ _ _ _ _ _ _|_ _ _ _ _ _|_ _ _ _ _ _ _|_ _ _ _ _ _ _ _|_ _ _ _ _ _|_ _ _ _ _ |
+|_.._.._.._ _ _|_._._._ _ _ _ _ _ _|_._._._ _ _ _ _ _ _|_._._._ _ _ _ _ _|_._._._ _|_._._._ _ _|_._._._ _ _ _ _ _ _ _|_._._._ _ _|_._._._ _ _ _|_._._._ _ _ _ _|_._._._ _ _|_._._._ _ |
+|2222111188|40.704273|-        |Saturday|10  |25461|Outdoors &|-999 |8.6   |Clear  |29551|1070 |
+|_ _ _ _ _ _|_ _ _ _ _ _ _ _ _ _|_7_3_._9_8_6_7_5_9_|_ _ _ _ _ _ _ _ _|_ _ _ _ _|_ _ _ _ _ _|_R_e_c_r_e_a_t_i_o_n_|_ _ _ _ _ _|_ _ _ _ _ _ _|_ _ _ _ _ _ _ _|_ _ _ _ _ _|_ _ _ _ _ |
+|2222111199|40.704733|-        |Saturday|10  |1805 |College & |-999 |-999.0|Clear  |29551|1070 |
+|_ _ _ _ _ _|_ _ _ _ _ _ _ _ _ _|_7_3_._9_8_7_7_3_8_|_ _ _ _ _ _ _ _ _|_ _ _ _ _|_ _ _ _ _ _|_U_n_i_v_e_r_s_i_t_y_|_ _ _ _ _ _|_ _ _ _ _ _ _|_ _ _ _ _ _ _ _|_ _ _ _ _ _|_ _ _ _ _ |
+|2222112200|40.717353|-        |Saturday|13  |32523|Food      |1    |9.3   |Clear  |29551|1070 |
+|_ _ _ _ _ _|_ _ _ _ _ _ _ _ _ _|_7_3_._9_6_0_3_9_2_|_ _ _ _ _ _ _ _ _|_ _ _ _ _|_ _ _ _ _ _|_ _ _ _ _ _ _ _ _ _ _|_ _ _ _ _ _|_ _ _ _ _ _ _|_ _ _ _ _ _ _ _|_ _ _ _ _ _|_ _ _ _ _ |
+|2222112211|40.697721|-        |Sunday  |2   |36212|College & |-999 |-999.0|Clear  |29551|1070 |
+|_ _ _ _ _ _|_ _ _ _ _ _ _ _ _ _|_7_3_._9_9_3_0_2_0_|_ _ _ _ _ _ _ _ _|_ _ _ _ _|_ _ _ _ _ _|_U_n_i_v_e_r_s_i_t_y_|_ _ _ _ _ _|_ _ _ _ _ _ _|_ _ _ _ _ _ _ _|_ _ _ _ _ _|_ _ _ _ _ |
+|2222112222|40.697803|-        |Sunday  |8   |16452|Outdoors &|-999 |6.9   |Clear  |29551|1070 |
+|_ _ _ _ _ _|_ _ _ _ _ _ _ _ _ _|_7_3_._9_9_4_1_4_5_|_ _ _ _ _ _ _ _ _|_ _ _ _ _|_ _ _ _ _ _|_R_e_c_r_e_a_t_i_o_n_|_ _ _ _ _ _|_ _ _ _ _ _ _|_ _ _ _ _ _ _ _|_ _ _ _ _ _|_ _ _ _ _ |
+16435 rows × 11 columns
+ b) Second, you can load the 70/30 hold out split available (by default):
+In [14]:
+df_train, df_test = load_ds_holdout()
+
+print(df_train.shape, df_test.shape)
+
+df_train
+Loading dataset file: https://github.com/mat-analysis/datasets/raw/main/mat/
+FoursquareNYC/
+  0%|          | 0/193 [00:00<?, ?it/s]
+(46785, 11) (20177, 11)
+Out[14]:
+ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ 
+|_ _ _ _ _ _|_ _ _ _ _ _ _ll_aa_tt_|_ _ _ _ _ _ _ll_oo_nn_|_ _ _ _ _ _dd_aa_yy_|_hh_oo_uu_rr_|_ _ _pp_oo_ii_|_ _ _ _ _cc_aa_tt_ee_gg_oo_rr_yy_|_pp_rr_ii_cc_ee_|_rr_aa_tt_ii_nn_gg_|_ww_ee_aa_tt_hh_ee_rr_|_ _ _tt_ii_dd_|_ll_aa_bb_ee_ll|
+|00    |40.834098|-        |Monday  |13  |21580|Food        |1    |8.2   |Clouds |127  |6    |
+|_ _ _ _ _ _|_ _ _ _ _ _ _ _ _ _|_7_3_._9_4_5_2_6_7_|_ _ _ _ _ _ _ _ _|_ _ _ _ _|_ _ _ _ _ _|_ _ _ _ _ _ _ _ _ _ _ _ _|_ _ _ _ _ _|_ _ _ _ _ _ _|_ _ _ _ _ _ _ _|_ _ _ _ _ _|_ _ _ _ _ |
+|11    |40.567196|-        |Monday  |19  |2392 |Travel &    |-999 |-999.0|Clouds |127  |6    |
+|_ _ _ _ _ _|_ _ _ _ _ _ _ _ _ _|_7_3_._8_8_2_5_7_6_|_ _ _ _ _ _ _ _ _|_ _ _ _ _|_ _ _ _ _ _|_T_r_a_n_s_p_o_r_t_ _ _ _|_ _ _ _ _ _|_ _ _ _ _ _ _|_ _ _ _ _ _ _ _|_ _ _ _ _ _|_ _ _ _ _ |
+|22    |40.689913|-        |Monday  |23  |35589|Travel &    |-999 |-999.0|Clouds |127  |6    |
+|_ _ _ _ _ _|_ _ _ _ _ _ _ _ _ _|_7_3_._9_8_1_5_0_4_|_ _ _ _ _ _ _ _ _|_ _ _ _ _|_ _ _ _ _ _|_T_r_a_n_s_p_o_r_t_ _ _ _|_ _ _ _ _ _|_ _ _ _ _ _ _|_ _ _ _ _ _ _ _|_ _ _ _ _ _|_ _ _ _ _ |
+|33    |40.708588|-        |Monday  |23  |18603|Travel &    |-999 |-999.0|Clouds |127  |6    |
+|_ _ _ _ _ _|_ _ _ _ _ _ _ _ _ _|_7_3_._9_9_1_0_3_2_|_ _ _ _ _ _ _ _ _|_ _ _ _ _|_ _ _ _ _ _|_T_r_a_n_s_p_o_r_t_ _ _ _|_ _ _ _ _ _|_ _ _ _ _ _ _|_ _ _ _ _ _ _ _|_ _ _ _ _ _|_ _ _ _ _ |
+|44    |40.833165|-        |Tuesday |14  |36348|Residence   |-999 |-999.0|Clear  |127  |6    |
+|_ _ _ _ _ _|_ _ _ _ _ _ _ _ _ _|_7_3_._9_4_1_8_6_0_|_ _ _ _ _ _ _ _ _|_ _ _ _ _|_ _ _ _ _ _|_ _ _ _ _ _ _ _ _ _ _ _ _|_ _ _ _ _ _|_ _ _ _ _ _ _|_ _ _ _ _ _ _ _|_ _ _ _ _ _|_ _ _ _ _ |
+|_.._.._.._ _ _|_._._._ _ _ _ _ _ _|_._._._ _ _ _ _ _ _|_._._._ _ _ _ _ _|_._._._ _|_._._._ _ _|_._._._ _ _ _ _ _ _ _ _ _|_._._._ _ _|_._._._ _ _ _|_._._._ _ _ _ _|_._._._ _ _|_._._._ _ |
+|2222114488|40.705953|-        |Saturday|19  |35308|Outdoors &  |-999 |9.6   |Clear  |29556|1070 |
+|_ _ _ _ _ _|_ _ _ _ _ _ _ _ _ _|_7_3_._9_9_6_5_6_8_|_ _ _ _ _ _ _ _ _|_ _ _ _ _|_ _ _ _ _ _|_R_e_c_r_e_a_t_i_o_n_ _ _|_ _ _ _ _ _|_ _ _ _ _ _ _|_ _ _ _ _ _ _ _|_ _ _ _ _ _|_ _ _ _ _ |
+|2222114499|40.697721|-        |Saturday|23  |36212|College &   |-999 |-999.0|Clear  |29556|1070 |
+|_ _ _ _ _ _|_ _ _ _ _ _ _ _ _ _|_7_3_._9_9_3_0_2_0_|_ _ _ _ _ _ _ _ _|_ _ _ _ _|_ _ _ _ _ _|_U_n_i_v_e_r_s_i_t_y_ _ _|_ _ _ _ _ _|_ _ _ _ _ _ _|_ _ _ _ _ _ _ _|_ _ _ _ _ _|_ _ _ _ _ |
+|2222115500|40.697884|-        |Sunday  |15  |38090|Shop &      |-999 |5.2   |Clouds |29556|1070 |
+|_ _ _ _ _ _|_ _ _ _ _ _ _ _ _ _|_7_3_._9_9_2_8_0_5_|_ _ _ _ _ _ _ _ _|_ _ _ _ _|_ _ _ _ _ _|_S_e_r_v_i_c_e_ _ _ _ _ _|_ _ _ _ _ _|_ _ _ _ _ _ _|_ _ _ _ _ _ _ _|_ _ _ _ _ _|_ _ _ _ _ |
+|2222115511|40.698291|-        |Sunday  |18  |33538|Outdoors &  |-999 |9.6   |Clouds |29556|1070 |
+|_ _ _ _ _ _|_ _ _ _ _ _ _ _ _ _|_7_3_._9_9_6_6_3_2_|_ _ _ _ _ _ _ _ _|_ _ _ _ _|_ _ _ _ _ _|_R_e_c_r_e_a_t_i_o_n_ _ _|_ _ _ _ _ _|_ _ _ _ _ _ _|_ _ _ _ _ _ _ _|_ _ _ _ _ _|_ _ _ _ _ |
+|     |         |-        |        |    |     |Professional|     |      |       |     |     |
+|2222115522|40.692421|73.994002|Sunday  |18  |29212|& Other     |-999 |-999.0|Clouds |29556|1070 |
+|_ _ _ _ _ _|_ _ _ _ _ _ _ _ _ _|_ _ _ _ _ _ _ _ _ _|_ _ _ _ _ _ _ _ _|_ _ _ _ _|_ _ _ _ _ _|_P_l_a_c_e_s_ _ _ _ _ _ _|_ _ _ _ _ _|_ _ _ _ _ _ _|_ _ _ _ _ _ _ _|_ _ _ _ _ _|_ _ _ _ _ |
+46785 rows × 11 columns
+Or, you can hold out split on another proportion (50% for instance):
+In [15]:
+df_train, df_test = load_ds_holdout(train_size=0.5)
+
+# The split is class-balanced, thus train and test number of trajectories may
+not be exactly proportional.
+print(df_train.shape, df_test.shape)
+
+df_train
+Loading dataset file: https://github.com/mat-analysis/datasets/raw/main/mat/
+FoursquareNYC/
+  0%|          | 0/193 [00:00<?, ?it/s]
+(33773, 11) (33189, 11)
+Out[15]:
+ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ 
+|_ _ _ _ _ _|_ _ _ _ _ _ _ll_aa_tt_|_ _ _ _ _ _ _ll_oo_nn_|_ _ _ _ _ _dd_aa_yy_|_hh_oo_uu_rr_|_ _ _pp_oo_ii_|_ _ _cc_aa_tt_ee_gg_oo_rr_yy_|_pp_rr_ii_cc_ee_|_rr_aa_tt_ii_nn_gg_|_ww_ee_aa_tt_hh_ee_rr_|_ _ _tt_ii_dd_|_ll_aa_bb_ee_ll|
+|00    |40.834098|-        |Monday  |13  |21580|Food      |1    |8.2   |Clouds |127  |6    |
+|_ _ _ _ _ _|_ _ _ _ _ _ _ _ _ _|_7_3_._9_4_5_2_6_7_|_ _ _ _ _ _ _ _ _|_ _ _ _ _|_ _ _ _ _ _|_ _ _ _ _ _ _ _ _ _ _|_ _ _ _ _ _|_ _ _ _ _ _ _|_ _ _ _ _ _ _ _|_ _ _ _ _ _|_ _ _ _ _ |
+|11    |40.567196|-        |Monday  |19  |2392 |Travel &  |-999 |-999.0|Clouds |127  |6    |
+|_ _ _ _ _ _|_ _ _ _ _ _ _ _ _ _|_7_3_._8_8_2_5_7_6_|_ _ _ _ _ _ _ _ _|_ _ _ _ _|_ _ _ _ _ _|_T_r_a_n_s_p_o_r_t_ _|_ _ _ _ _ _|_ _ _ _ _ _ _|_ _ _ _ _ _ _ _|_ _ _ _ _ _|_ _ _ _ _ |
+|22    |40.689913|-        |Monday  |23  |35589|Travel &  |-999 |-999.0|Clouds |127  |6    |
+|_ _ _ _ _ _|_ _ _ _ _ _ _ _ _ _|_7_3_._9_8_1_5_0_4_|_ _ _ _ _ _ _ _ _|_ _ _ _ _|_ _ _ _ _ _|_T_r_a_n_s_p_o_r_t_ _|_ _ _ _ _ _|_ _ _ _ _ _ _|_ _ _ _ _ _ _ _|_ _ _ _ _ _|_ _ _ _ _ |
+|33    |40.708588|-        |Monday  |23  |18603|Travel &  |-999 |-999.0|Clouds |127  |6    |
+|_ _ _ _ _ _|_ _ _ _ _ _ _ _ _ _|_7_3_._9_9_1_0_3_2_|_ _ _ _ _ _ _ _ _|_ _ _ _ _|_ _ _ _ _ _|_T_r_a_n_s_p_o_r_t_ _|_ _ _ _ _ _|_ _ _ _ _ _ _|_ _ _ _ _ _ _ _|_ _ _ _ _ _|_ _ _ _ _ |
+|44    |40.833165|-        |Tuesday |14  |36348|Residence |-999 |-999.0|Clear  |127  |6    |
+|_ _ _ _ _ _|_ _ _ _ _ _ _ _ _ _|_7_3_._9_4_1_8_6_0_|_ _ _ _ _ _ _ _ _|_ _ _ _ _|_ _ _ _ _ _|_ _ _ _ _ _ _ _ _ _ _|_ _ _ _ _ _|_ _ _ _ _ _ _|_ _ _ _ _ _ _ _|_ _ _ _ _ _|_ _ _ _ _ |
+|_.._.._.._ _ _|_._._._ _ _ _ _ _ _|_._._._ _ _ _ _ _ _|_._._._ _ _ _ _ _|_._._._ _|_._._._ _ _|_._._._ _ _ _ _ _ _ _|_._._._ _ _|_._._._ _ _ _|_._._._ _ _ _ _|_._._._ _ _|_._._._ _ |
+|2222113311|40.704733|-        |Thursday|18  |1805 |College & |-999 |-999.0|Clear  |29554|1070 |
+|_ _ _ _ _ _|_ _ _ _ _ _ _ _ _ _|_7_3_._9_8_7_7_3_8_|_ _ _ _ _ _ _ _ _|_ _ _ _ _|_ _ _ _ _ _|_U_n_i_v_e_r_s_i_t_y_|_ _ _ _ _ _|_ _ _ _ _ _ _|_ _ _ _ _ _ _ _|_ _ _ _ _ _|_ _ _ _ _ |
+|2222113322|40.704273|-        |Thursday|19  |25461|Outdoors &|-999 |8.6   |Clear  |29554|1070 |
+|_ _ _ _ _ _|_ _ _ _ _ _ _ _ _ _|_7_3_._9_8_6_7_5_9_|_ _ _ _ _ _ _ _ _|_ _ _ _ _|_ _ _ _ _ _|_R_e_c_r_e_a_t_i_o_n_|_ _ _ _ _ _|_ _ _ _ _ _ _|_ _ _ _ _ _ _ _|_ _ _ _ _ _|_ _ _ _ _ |
+|2222113333|40.697803|-        |Friday  |10  |16452|Outdoors &|-999 |6.9   |Clear  |29554|1070 |
+|_ _ _ _ _ _|_ _ _ _ _ _ _ _ _ _|_7_3_._9_9_4_1_4_5_|_ _ _ _ _ _ _ _ _|_ _ _ _ _|_ _ _ _ _ _|_R_e_c_r_e_a_t_i_o_n_|_ _ _ _ _ _|_ _ _ _ _ _ _|_ _ _ _ _ _ _ _|_ _ _ _ _ _|_ _ _ _ _ |
+|2222113344|40.695163|-        |Friday  |20  |1944 |Food      |2    |8.0   |Clear  |29554|1070 |
+|_ _ _ _ _ _|_ _ _ _ _ _ _ _ _ _|_7_3_._9_9_5_4_4_8_|_ _ _ _ _ _ _ _ _|_ _ _ _ _|_ _ _ _ _ _|_ _ _ _ _ _ _ _ _ _ _|_ _ _ _ _ _|_ _ _ _ _ _ _|_ _ _ _ _ _ _ _|_ _ _ _ _ _|_ _ _ _ _ |
+|2222113355|40.694673|-        |Saturday|13  |16201|Food      |1    |7.0   |Clear  |29554|1070 |
+|_ _ _ _ _ _|_ _ _ _ _ _ _ _ _ _|_7_3_._9_9_4_0_8_2_|_ _ _ _ _ _ _ _ _|_ _ _ _ _|_ _ _ _ _ _|_ _ _ _ _ _ _ _ _ _ _|_ _ _ _ _ _|_ _ _ _ _ _ _|_ _ _ _ _ _ _ _|_ _ _ _ _ _|_ _ _ _ _ |
+33773 rows × 11 columns
+c) Or, you can load the k-fold split datasets available (deafult k=5):
+In [16]:
+df_train, df_test = load_ds_kfold()
 
-root      = os.path.join('automatize', 'assets', 'examples', 'Example')
+for k in range(len(df_train)):
+    print('Shape train/test:', df_train[k].shape, df_test[k].shape)
+Loading dataset file: https://github.com/mat-analysis/datasets/raw/main/mat/
+FoursquareNYC/
+Spliting Data:   0%|          | 0/193 [00:00<?, ?it/s]
+Shape train/test: (51130, 11) (15832, 11)
+Shape train/test: (52678, 11) (14284, 11)
+Shape train/test: (53938, 11) (13024, 11)
+Shape train/test: (54856, 11) (12106, 11)
+Shape train/test: (55246, 11) (11716, 11)
+d) You can load a different dataset from repository:
+In [17]:
+# Use the format: 'category.DatasetName'
+dataset='raw.Animals'
 
-# We consider this folder organization to the experimental enviromnent:
-prg_path  = os.path.join(root, 'programs')
-data_path = os.path.join(root, 'data')
-res_path  = os.path.join(root, 'results')
-
-# OR, you can use the .jar method files in:
-prg_path  = os.path.join('automatize', 'assets', 'method')
-******** 11.. PPrree--pprroocceessssiinngg ddaattaa_?¶ ********
+df = load_ds(dataset)
+df
+Loading dataset file: https://github.com/mat-analysis/datasets/raw/main/raw/
+Animals/
+Out[17]:
+ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ 
+|_ _ _ _ _|_ _ _tt_ii_mm_ee_|_ _ _ _ _ll_aa_tt_|_ _ _ _ _ll_oo_nn_|_tt_ii_dd_|_ll_aa_bb_ee_ll|
+|_00_ _ _ _|_0_._0_0_ _ _|_5_0_._1_0_6_6_|_3_._7_9_6_6_5_|_1_ _ _|_D_ _ _ _ |
+|_11_ _ _ _|_4_._3_9_ _ _|_5_0_._1_0_4_5_|_3_._7_9_4_5_5_|_1_ _ _|_D_ _ _ _ |
+|_22_ _ _ _|_7_._9_0_ _ _|_5_0_._1_1_1_1_|_3_._7_9_8_4_5_|_1_ _ _|_D_ _ _ _ |
+|_33_ _ _ _|_9_._6_2_ _ _|_5_0_._1_0_7_2_|_3_._7_9_8_4_5_|_1_ _ _|_D_ _ _ _ |
+|_44_ _ _ _|_1_5_._0_9_ _|_5_0_._1_1_3_2_|_3_._7_9_9_6_5_|_1_ _ _|_D_ _ _ _ |
+|_.._.._.._ _|_._._._ _ _ _|_._._._ _ _ _ _|_._._._ _ _ _ _|_._._._|_._._._ _ |
+|_44_55_11_77_|_2_5_8_._8_8_|_5_0_._1_6_9_6_|_3_._7_6_2_1_5_|_9_7_ _|_C_ _ _ _ |
+|_44_55_11_88_|_2_6_0_._8_5_|_5_0_._1_6_9_3_|_3_._7_6_1_8_5_|_9_7_ _|_C_ _ _ _ |
+|_44_55_11_99_|_2_6_2_._8_0_|_5_0_._1_6_9_3_|_3_._7_6_2_4_5_|_9_7_ _|_C_ _ _ _ |
+|_44_55_22_00_|_2_6_4_._6_9_|_5_0_._1_6_8_7_|_3_._7_6_4_5_5_|_9_7_ _|_C_ _ _ _ |
+|_44_55_22_11_|_2_6_6_._9_0_|_5_0_._1_6_8_7_|_3_._7_6_4_5_5_|_9_7_ _|_C_ _ _ _ |
+14990 rows × 5 columns
+e) To get a full list of anailable repositories and categories:
+In [18]:
+rd = repository_datasets()
+
+print('Multiple Aspect Trajecory datasets:', rd['mat'])
+
+rd
+Multiple Aspect Trajecory datasets: ['Brightkite', 'FoursquareGlobal',
+'FoursquareNYC', 'Gowalla', 'Weeplaces']
+Out[18]:
+{'log': ['BPI2011', 'BPI2012', 'BPI2015', 'BPI2017', 'BPI2018', 'BPI2019'],
+ 'mat': ['Brightkite',
+  'FoursquareGlobal',
+  'FoursquareNYC',
+  'Gowalla',
+  'Weeplaces'],
+ 'mts': ['ActivityRecognition',
+  'ArticularyWordRecognition',
+  'AtrialFibrillation',
+  'AustralianSignLanguage',
+  'BasicMotions',
+  'CharacterTrajectories',
+  'Cricket',
+  'DuckDuckGeese',
+  'ERing',
+  'EigenWorms',
+  'Epilepsy',
+  'EthanolConcentration',
+  'FaceDetection',
+  'FaciesRocks',
+  'FingerMovements',
+  'GECCOWater',
+  'GrammaticalFacialExpression',
+  'HandMovementDirection',
+  'Handwriting',
+  'Heartbeat',
+  'InsectWingbeat',
+  'JapaneseVowels',
+  'LSST',
+  'Libras',
+  'MotorImagery',
+  'NATOPS',
+  'PEMS-SF',
+  'PenDigits',
+  'PhonemeSpectra',
+  'RacketSports',
+  'SelfRegulationSCP1',
+  'SelfRegulationSCP2',
+  'SpokenArabicDigits',
+  'StandWalkJump',
+  'UWaveGestureLibrary'],
+ 'raw': ['Animals', 'Geolife', 'GoTrack', 'Hurricanes', 'Vehicles'],
+ 'sequential': ['ClothingAlibaba', 'Promoters', 'SJGS'],
+ 'uts': ['ACSF1',
+  'Adiac',
+  'AllGestureWiimoteX',
+  'AllGestureWiimoteY',
+  'AllGestureWiimoteZ',
+  'ArrowHead',
+  'BME',
+  'Beef',
+  'BeetleFly',
+  'BirdChicken',
+  'CBF',
+  'Car',
+  'Chinatown',
+  'ChlorineConcentration',
+  'CinCECGTorso',
+  'Coffee',
+  'Computers',
+  'CricketX',
+  'CricketY',
+  'CricketZ',
+  'Crop',
+  'DiatomSizeReduction',
+  'DistalPhalanxOutlineAgeGroup',
+  'DistalPhalanxOutlineCorrect',
+  'DistalPhalanxTW',
+  'DodgerLoopDay',
+  'DodgerLoopGame',
+  'DodgerLoopWeekend',
+  'ECG200',
+  'ECG5000',
+  'ECGFiveDays',
+  'EOGHorizontalSignal',
+  'EOGVerticalSignal',
+  'Earthquakes',
+  'ElectricDevices',
+  'EthanolLevel',
+  'FaceAll',
+  'FaceFour',
+  'FacesUCR',
+  'FiftyWords',
+  'Fish',
+  'FordA',
+  'FordB',
+  'FreezerRegularTrain',
+  'FreezerSmallTrain',
+  'Fungi',
+  'GestureMidAirD1',
+  'GestureMidAirD2',
+  'GestureMidAirD3',
+  'GesturePebbleZ1',
+  'GesturePebbleZ2',
+  'GunPoint',
+  'GunPointAgeSpan',
+  'GunPointMaleVersusFemale',
+  'GunPointOldVersusYoung',
+  'Ham',
+  'HandOutlines',
+  'Haptics',
+  'Herring',
+  'HouseTwenty',
+  'InlineSkate',
+  'InsectEPGRegularTrain',
+  'InsectEPGSmallTrain',
+  'InsectWingbeatSound',
+  'ItalyPowerDemand',
+  'LargeKitchenAppliances',
+  'Lightning2',
+  'Lightning7',
+  'Mallat',
+  'Meat',
+  'MedicalImages',
+  'MelbournePedestrian',
+  'MiddlePhalanxOutlineAgeGroup',
+  'MiddlePhalanxOutlineCorrect',
+  'MiddlePhalanxTW',
+  'MixedShapesRegularTrain',
+  'MixedShapesSmallTrain',
+  'MoteStrain',
+  'NonInvasiveFetalECGThorax1',
+  'NonInvasiveFetalECGThorax2',
+  'OSULeaf',
+  'OliveOil',
+  'PLAID',
+  'PhalangesOutlinesCorrect',
+  'Phoneme',
+  'PickupGestureWiimoteZ',
+  'PigAirwayPressure',
+  'PigArtPressure',
+  'PigCVP',
+  'Plane',
+  'PowerCons',
+  'ProximalPhalanxOutlineAgeGroup',
+  'ProximalPhalanxOutlineCorrect',
+  'ProximalPhalanxTW',
+  'RefrigerationDevices',
+  'Rock',
+  'ScreenType',
+  'SemgHandGenderCh2',
+  'SemgHandMovementCh2',
+  'SemgHandSubjectCh2',
+  'ShakeGestureWiimoteZ',
+  'ShapeletSim',
+  'ShapesAll',
+  'SmallKitchenAppliances',
+  'SmoothSubspace',
+  'SonyAIBORobotSurface1',
+  'SonyAIBORobotSurface2',
+  'StarLightCurves',
+  'Strawberry',
+  'SwedishLeaf',
+  'Symbols',
+  'SyntheticControl',
+  'ToeSegmentation1',
+  'ToeSegmentation2',
+  'Trace',
+  'TwoLeadECG',
+  'TwoPatterns',
+  'UMD',
+  'UWaveGestureLibraryAll',
+  'UWaveGestureLibraryX',
+  'UWaveGestureLibraryY',
+  'UWaveGestureLibraryZ',
+  'Wafer',
+  'Wine',
+  'WordSynonyms',
+  'Worms',
+  'WormsTwoClass',
+  'Yoga']}
+******** 33.. PPrree--pprroocceessssiinngg ddaattaa_?¶ ********
 To use helpers for data pre-processing, import from package matdata.preprocess:
-In [3]:
+In [19]:
 from matdata.preprocess import *
-The pprreepprroocceessssiinngg module provides some functions to work data:
+The pprreepprroocceessss module provides some functions to work data:
 Basic functions:
-    * readDataset: load datasets as pandas DataFrame (from .csv, .zip, or .ts)
+    * readDataset: load datasets as pandas DataFrame (from .csv, .parquet,
+      .zip, .ts or .xes)
+    * organizeFrame: standardize data columns for the DataFrame
+Train and Test split functions:
+    * trainTestSplit: split dataset (pandas DataFrame) in train / test (70/30%
+      by default)
+    * kfold_trainTestSplit: split dataset (pandas DataFrame) in k-fold train /
+      test (5-fold of 80/20% each fold by default)
+    * stratify: extract trajectories from the dataset, respecting class
+      balance, creating a subset of the data (to use when smaller datasets are
+      needed)
+    * klabels_stratify: k-labels statification (randomly select k-labels from
+      the dataset)
+    * joinTrainTest: joins the separated train and test files into one
+      DataFrame.
+Statistical functions:
     * printFeaturesJSON: print a default JSON file descriptor for Movelets
       methods (version 1 or 2)
-    * datasetStatistics: calculates statistics from a datasets dataframe.
-Train and Test split functions:
-    * trainAndTestSplit: split dataset (pandas DataFrame) in train / test (70/
-      30% by default)
-    * kfold_trainAndTestSplit: split dataset (pandas DataFrame) in k-fold train
-      / test (80/20% each fold by default)
-    * stratify: extract trajectories from the dataset, creating a subset of the
-      data (to use when smaller datasets are needed)
-    * joinTrainAndTest: joins the train and test files into one DataFrame.
-Type convertion functions:
-    * convertDataset: default format conversions. Reads the dataset files and
-      saves in .csv and .zip formats, also do k-fold split if not present
-    * zip2df: converts .zip files and saves to DataFrame
+    * countClasses: calculates statistics from a dataset dataframe
+    * dfVariance: calculates a variance rank from a dataset dataframe
+    * dfStats: calculates attributes statistics ordered by variance from a
+      dataset dataframe
+    * datasetStatistics: generates dataset statistics from a dataframe in
+      markdown text.
+Type reading functions:
+    * csv2df: reads .csv dataset dataframe
+    * parquet2df: reads .parquet dataset dataframe
+    * zip2df: reads .zip dataset dataframe (zip containing trajectory csv
+      files)
+    * ts2df: reads .ts dataset dataframe (Time Series data format)
+    * xes2df: reads .xes dataset dataframe (event log / event stream file)
+    * mat2df: TTOODDOO reads .mat dataset dataframe (multiple aspect trajectory
+      specific file format)
+File convertion functions:
     * zip2csv: converts .zip files and saves to .csv files
     * df2zip: converts DataFrame and saves to .zip files
-    * zip2arf: converts .zip and saves to .arf files
     * any2ts: converts .zip or .csv files and saves to .ts files
     * xes2csv: reads .xes files and converts to DataFrame
-In [10]:
-#cols =
-['tid','label','lat','lon','day','hour','poi','category','price','rating']
+    * convertDataset: default format conversions. Reads the dataset files and
+      saves in .csv and .zip formats, also do k-fold split if not present
+a) Basic reading the data, and organization:
+In [20]:
+data_path = 'matdata/assets/sample'
+
+df = readDataset(data_path, file='Foursquare_Sample.csv')
+df.head()
+Out[20]:
+ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ 
+|_ _|_tt_ii_dd_|_ _ _ _ _ _ _ _ _ _ll_aa_tt____ll_oo_nn_|_dd_aa_tt_ee____tt_ii_mm_ee_|_tt_ii_mm_ee_|_rr_aa_tt_ii_nn_gg_|_pp_rr_ii_cc_ee_|_ww_ee_aa_tt_hh_ee_rr_|_ _ _ _ _ _dd_aa_yy_|_rr_oo_oo_tt____tt_yy_pp_ee_|_ _ _ _ _ _tt_yy_pp_ee|
+| |   |40.8331652006224|2012-11- |    |      |     |       |        |         |Home     |
+|00|126|-               |12 05:17:|317 |-1.0  |-1   |Clear  |Monday  |Residence|(private)|
+|_ _|_ _ _ _|_7_3_._9_4_1_8_6_0_3_4_2_7_6_9_2_|_1_8_ _ _ _ _ _ _ _|_ _ _ _ _|_ _ _ _ _ _ _|_ _ _ _ _ _|_ _ _ _ _ _ _ _|_ _ _ _ _ _ _ _ _|_ _ _ _ _ _ _ _ _ _|_ _ _ _ _ _ _ _ _ |
+| |   |40.8340978041072|2012-11- |    |      |     |       |        |         |Deli /   |
+|11|126|-               |12 23:24:|1404|8.2   |1    |Clouds |Monday  |Food     |Bodega   |
+|_ _|_ _ _ _|_7_3_._9_4_5_2_6_7_2_2_2_5_8_8_1_|_5_5_ _ _ _ _ _ _ _|_ _ _ _ _|_ _ _ _ _ _ _|_ _ _ _ _ _|_ _ _ _ _ _ _ _|_ _ _ _ _ _ _ _ _|_ _ _ _ _ _ _ _ _ _|_ _ _ _ _ _ _ _ _ |
+| |   |40.8331652006224|2012-11- |    |      |     |       |        |         |Home     |
+|22|126|-               |13 00:00:|0   |-1.0  |-1   |Clouds |Tuesday |Residence|(private)|
+|_ _|_ _ _ _|_7_3_._9_4_1_8_6_0_3_4_2_7_6_9_2_|_0_7_ _ _ _ _ _ _ _|_ _ _ _ _|_ _ _ _ _ _ _|_ _ _ _ _ _|_ _ _ _ _ _ _ _|_ _ _ _ _ _ _ _ _|_ _ _ _ _ _ _ _ _ _|_ _ _ _ _ _ _ _ _ |
+| |   |40.7646959283254|2012-11- |    |      |     |       |        |         |Fried    |
+|33|126|-               |15 17:49:|1069|6.6   |3    |Clear  |Thursday|Food     |Chicken  |
+|_ _|_ _ _ _|_7_3_._8_8_5_1_9_7_4_9_6_4_4_1_4_|_0_1_ _ _ _ _ _ _ _|_ _ _ _ _|_ _ _ _ _ _ _|_ _ _ _ _ _|_ _ _ _ _ _ _ _|_ _ _ _ _ _ _ _ _|_ _ _ _ _ _ _ _ _ _|_J_o_i_n_t_ _ _ _ |
+| |   |40.7660790376824|2012-11- |    |      |     |       |        |Travel & |Bus      |
+|44|126|-               |15 18:40:|1120|-1.0  |-1   |Clear  |Thursday|Transport|Station  |
+|_ _|_ _ _ _|_7_3_._8_8_3_5_2_8_7_0_9_4_1_1_6_|_1_6_ _ _ _ _ _ _ _|_ _ _ _ _|_ _ _ _ _ _ _|_ _ _ _ _ _|_ _ _ _ _ _ _ _|_ _ _ _ _ _ _ _ _|_ _ _ _ _ _ _ _ _ _|_ _ _ _ _ _ _ _ _ |
+In [21]:
+df, space_cols, ll_cols = organizeFrame(df, make_spatials=True)
+
+print('Columns with space: ', space_cols)
+print('Columns with lat/lon: ', ll_cols)
+df.head()
+Columns with space:  ['space', 'date_time', 'time', 'rating', 'price',
+'weather', 'day', 'root_type', 'type', 'tid']
+Columns with lat/lon:  ['date_time', 'time', 'rating', 'price', 'weather',
+'day', 'root_type', 'type', 'lat', 'lon', 'tid']
+Out[21]:
+ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ 
+|_ _|_tt_ii_dd_|_ _ _ _ _ _ _ _ _ _ _ _ss_pp_aa_cc_ee_|_dd_aa_tt_ee____tt_ii_mm_ee_|_tt_ii_mm_ee_|_rr_aa_tt_ii_nn_gg_|_pp_rr_ii_cc_ee_|_ww_ee_aa_tt_hh_ee_rr_|_ _ _ _ _ _dd_aa_yy_|_rr_oo_oo_tt____tt_yy_pp_ee_|_ _ _ _ _ _tt_yy_pp_ee_|_ _ _ _ _ _ _ll_aa_tt_|_ _ _ _ _ _ _ll_oo_nn|
+| |   |40.8331652006224|2012-11- |    |      |     |       |        |         |Home     |         |-        |
+|00|126|-               |12 05:17:|317 |-1.0  |-1   |Clear  |Monday  |Residence|(private)|40.833165|73.941860|
+|_ _|_ _ _ _|_7_3_._9_4_1_8_6_0_3_4_2_7_6_9_2_|_1_8_ _ _ _ _ _ _ _|_ _ _ _ _|_ _ _ _ _ _ _|_ _ _ _ _ _|_ _ _ _ _ _ _ _|_ _ _ _ _ _ _ _ _|_ _ _ _ _ _ _ _ _ _|_ _ _ _ _ _ _ _ _ _|_ _ _ _ _ _ _ _ _ _|_ _ _ _ _ _ _ _ _ |
+| |   |40.8340978041072|2012-11- |    |      |     |       |        |         |Deli /   |         |-        |
+|11|126|-               |12 23:24:|1404|8.2   |1    |Clouds |Monday  |Food     |Bodega   |40.834098|73.945267|
+|_ _|_ _ _ _|_7_3_._9_4_5_2_6_7_2_2_2_5_8_8_1_|_5_5_ _ _ _ _ _ _ _|_ _ _ _ _|_ _ _ _ _ _ _|_ _ _ _ _ _|_ _ _ _ _ _ _ _|_ _ _ _ _ _ _ _ _|_ _ _ _ _ _ _ _ _ _|_ _ _ _ _ _ _ _ _ _|_ _ _ _ _ _ _ _ _ _|_ _ _ _ _ _ _ _ _ |
+| |   |40.8331652006224|2012-11- |    |      |     |       |        |         |Home     |         |-        |
+|22|126|-               |13 00:00:|0   |-1.0  |-1   |Clouds |Tuesday |Residence|(private)|40.833165|73.941860|
+|_ _|_ _ _ _|_7_3_._9_4_1_8_6_0_3_4_2_7_6_9_2_|_0_7_ _ _ _ _ _ _ _|_ _ _ _ _|_ _ _ _ _ _ _|_ _ _ _ _ _|_ _ _ _ _ _ _ _|_ _ _ _ _ _ _ _ _|_ _ _ _ _ _ _ _ _ _|_ _ _ _ _ _ _ _ _ _|_ _ _ _ _ _ _ _ _ _|_ _ _ _ _ _ _ _ _ |
+| |   |40.7646959283254|2012-11- |    |      |     |       |        |         |Fried    |         |-        |
+|33|126|-               |15 17:49:|1069|6.6   |3    |Clear  |Thursday|Food     |Chicken  |40.764696|73.885197|
+|_ _|_ _ _ _|_7_3_._8_8_5_1_9_7_4_9_6_4_4_1_4_|_0_1_ _ _ _ _ _ _ _|_ _ _ _ _|_ _ _ _ _ _ _|_ _ _ _ _ _|_ _ _ _ _ _ _ _|_ _ _ _ _ _ _ _ _|_ _ _ _ _ _ _ _ _ _|_J_o_i_n_t_ _ _ _ _|_ _ _ _ _ _ _ _ _ _|_ _ _ _ _ _ _ _ _ |
+| |   |40.7660790376824|2012-11- |    |      |     |       |        |Travel & |Bus      |         |-        |
+|44|126|-               |15 18:40:|1120|-1.0  |-1   |Clear  |Thursday|Transport|Station  |40.766079|73.883529|
+|_ _|_ _ _ _|_7_3_._8_8_3_5_2_8_7_0_9_4_1_1_6_|_1_6_ _ _ _ _ _ _ _|_ _ _ _ _|_ _ _ _ _ _ _|_ _ _ _ _ _|_ _ _ _ _ _ _ _|_ _ _ _ _ _ _ _ _|_ _ _ _ _ _ _ _ _ _|_ _ _ _ _ _ _ _ _ _|_ _ _ _ _ _ _ _ _ _|_ _ _ _ _ _ _ _ _ |
+NNoottee:: To better standard, we recomend for classification the use of prepare_ds
+function from dataset module, as you can indicate the class column:
+In [22]:
+from matdata.dataset import prepare_ds
 
-df = joinTrainAndTest(data_path, train_file="train.csv", test_file="test.csv",
-class_col = 'label')
+df = prepare_ds(df, class_col='root_type') # 'root_type' is then renamed
+'label'
+df
+Out[22]:
+ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ 
+|_ _ _ _ _ _|_dd_aa_tt_ee____tt_ii_mm_ee_|_tt_ii_mm_ee_|_rr_aa_tt_ii_nn_gg_|_pp_rr_ii_cc_ee_|_ww_ee_aa_tt_hh_ee_rr_|_ _ _ _ _ _dd_aa_yy_|_ _ _ _ _ _ _tt_yy_pp_ee_|_ _ _ _ _ _ _ll_aa_tt_|_ _ _ _ _ _ _ll_oo_nn_|_ _ _tt_ii_dd_|_ _ _ _ _ _ll_aa_bb_ee_ll|
+|     |2012-11- |    |      |     |       |        |Home      |         |-        |     |          |
+|00    |12 05:17:|317 |-1.0  |-1   |Clear  |Monday  |(private) |40.833165|73.941860|126  |Residence |
+|_ _ _ _ _ _|_1_8_ _ _ _ _ _ _ _|_ _ _ _ _|_ _ _ _ _ _ _|_ _ _ _ _ _|_ _ _ _ _ _ _ _|_ _ _ _ _ _ _ _ _|_ _ _ _ _ _ _ _ _ _ _|_ _ _ _ _ _ _ _ _ _|_ _ _ _ _ _ _ _ _ _|_ _ _ _ _ _|_ _ _ _ _ _ _ _ _ _ |
+|     |2012-11- |    |      |     |       |        |Deli /    |         |-        |     |          |
+|11    |12 23:24:|1404|8.2   |1    |Clouds |Monday  |Bodega    |40.834098|73.945267|126  |Food      |
+|_ _ _ _ _ _|_5_5_ _ _ _ _ _ _ _|_ _ _ _ _|_ _ _ _ _ _ _|_ _ _ _ _ _|_ _ _ _ _ _ _ _|_ _ _ _ _ _ _ _ _|_ _ _ _ _ _ _ _ _ _ _|_ _ _ _ _ _ _ _ _ _|_ _ _ _ _ _ _ _ _ _|_ _ _ _ _ _|_ _ _ _ _ _ _ _ _ _ |
+|     |2012-11- |    |      |     |       |        |Home      |         |-        |     |          |
+|22    |13 00:00:|0   |-1.0  |-1   |Clouds |Tuesday |(private) |40.833165|73.941860|126  |Residence |
+|_ _ _ _ _ _|_0_7_ _ _ _ _ _ _ _|_ _ _ _ _|_ _ _ _ _ _ _|_ _ _ _ _ _|_ _ _ _ _ _ _ _|_ _ _ _ _ _ _ _ _|_ _ _ _ _ _ _ _ _ _ _|_ _ _ _ _ _ _ _ _ _|_ _ _ _ _ _ _ _ _ _|_ _ _ _ _ _|_ _ _ _ _ _ _ _ _ _ |
+|     |2012-11- |    |      |     |       |        |Fried     |         |-        |     |          |
+|33    |15 17:49:|1069|6.6   |3    |Clear  |Thursday|Chicken   |40.764696|73.885197|126  |Food      |
+|_ _ _ _ _ _|_0_1_ _ _ _ _ _ _ _|_ _ _ _ _|_ _ _ _ _ _ _|_ _ _ _ _ _|_ _ _ _ _ _ _ _|_ _ _ _ _ _ _ _ _|_J_o_i_n_t_ _ _ _ _ _|_ _ _ _ _ _ _ _ _ _|_ _ _ _ _ _ _ _ _ _|_ _ _ _ _ _|_ _ _ _ _ _ _ _ _ _ |
+|     |2012-11- |    |      |     |       |        |Bus       |         |-        |     |Travel &  |
+|44    |15 18:40:|1120|-1.0  |-1   |Clear  |Thursday|Station   |40.766079|73.883529|126  |Transport |
+|_ _ _ _ _ _|_1_6_ _ _ _ _ _ _ _|_ _ _ _ _|_ _ _ _ _ _ _|_ _ _ _ _ _|_ _ _ _ _ _ _ _|_ _ _ _ _ _ _ _ _|_ _ _ _ _ _ _ _ _ _ _|_ _ _ _ _ _ _ _ _ _|_ _ _ _ _ _ _ _ _ _|_ _ _ _ _ _|_ _ _ _ _ _ _ _ _ _ |
+|_.._.._.._ _ _|_._._._ _ _ _ _ _ _|_._._._ _|_._._._ _ _ _|_._._._ _ _|_._._._ _ _ _ _|_._._._ _ _ _ _ _|_._._._ _ _ _ _ _ _ _|_._._._ _ _ _ _ _ _|_._._._ _ _ _ _ _ _|_._._._ _ _|_._._._ _ _ _ _ _ _ |
+|     |2012-08- |    |      |     |       |        |General   |         |-        |     |College & |
+|6666995577|10 17:17:|1037|-1.0  |-1   |Clouds |Friday  |College & |40.704733|73.987738|29563|University|
+|_ _ _ _ _ _|_3_7_ _ _ _ _ _ _ _|_ _ _ _ _|_ _ _ _ _ _ _|_ _ _ _ _ _|_ _ _ _ _ _ _ _|_ _ _ _ _ _ _ _ _|_U_n_i_v_e_r_s_i_t_y_|_ _ _ _ _ _ _ _ _ _|_ _ _ _ _ _ _ _ _ _|_ _ _ _ _ _|_ _ _ _ _ _ _ _ _ _ |
+|     |2012-08- |    |      |     |       |        |Thai      |         |-        |     |          |
+|6666995588|10 20:10:|1210|8.0   |2    |Clouds |Friday  |Restaurant|40.695163|73.995448|29563|Food      |
+|_ _ _ _ _ _|_5_9_ _ _ _ _ _ _ _|_ _ _ _ _|_ _ _ _ _ _ _|_ _ _ _ _ _|_ _ _ _ _ _ _ _|_ _ _ _ _ _ _ _ _|_ _ _ _ _ _ _ _ _ _ _|_ _ _ _ _ _ _ _ _ _|_ _ _ _ _ _ _ _ _ _|_ _ _ _ _ _|_ _ _ _ _ _ _ _ _ _ |
+|     |2012-08- |    |      |     |       |        |          |         |-        |     |Outdoors &|
+|6666995599|11 08:01:|481 |6.9   |-1   |Clouds |Saturday|Gym       |40.697803|73.994145|29563|Recreation|
+|_ _ _ _ _ _|_2_0_ _ _ _ _ _ _ _|_ _ _ _ _|_ _ _ _ _ _ _|_ _ _ _ _ _|_ _ _ _ _ _ _ _|_ _ _ _ _ _ _ _ _|_ _ _ _ _ _ _ _ _ _ _|_ _ _ _ _ _ _ _ _ _|_ _ _ _ _ _ _ _ _ _|_ _ _ _ _ _|_ _ _ _ _ _ _ _ _ _ |
+|     |2012-08- |    |      |     |       |        |Coffee    |         |-        |     |          |
+|6666996600|11 13:39:|819 |7.0   |1    |Clouds |Saturday|Shop      |40.694673|73.994082|29563|Food      |
+|_ _ _ _ _ _|_3_9_ _ _ _ _ _ _ _|_ _ _ _ _|_ _ _ _ _ _ _|_ _ _ _ _ _|_ _ _ _ _ _ _ _|_ _ _ _ _ _ _ _ _|_ _ _ _ _ _ _ _ _ _ _|_ _ _ _ _ _ _ _ _ _|_ _ _ _ _ _ _ _ _ _|_ _ _ _ _ _|_ _ _ _ _ _ _ _ _ _ |
+|     |2012-08- |    |      |     |       |        |          |         |-        |     |Outdoors &|
+|6666996611|12 07:56:|476 |6.9   |-1   |Clouds |Sunday  |Gym       |40.697803|73.994145|29563|Recreation|
+|_ _ _ _ _ _|_2_6_ _ _ _ _ _ _ _|_ _ _ _ _|_ _ _ _ _ _ _|_ _ _ _ _ _|_ _ _ _ _ _ _ _|_ _ _ _ _ _ _ _ _|_ _ _ _ _ _ _ _ _ _ _|_ _ _ _ _ _ _ _ _ _|_ _ _ _ _ _ _ _ _ _|_ _ _ _ _ _|_ _ _ _ _ _ _ _ _ _ |
+66962 rows × 11 columns
+b) Train and test split:
+To hold-out split a dataset into train and test (70/30% by deafult):
+In [23]:
+train, test = trainTestSplit(df, random_num=1)
+train.head()
+  0%|          | 0/9 [00:00<?, ?it/s]
+Out[23]:
+ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ 
+|_ _|_dd_aa_tt_ee____tt_ii_mm_ee_|_tt_ii_mm_ee_|_rr_aa_tt_ii_nn_gg_|_pp_rr_ii_cc_ee_|_ww_ee_aa_tt_hh_ee_rr_|_ _ _ _ _ _dd_aa_yy_|_ _ _ _ _ _tt_yy_pp_ee_|_ _ _ _ _ _ _ll_aa_tt_|_ _ _ _ _ _ _ll_oo_nn_|_tt_ii_dd_|_ _ _ _ _ll_aa_bb_ee_ll|
+| |2012-11- |    |      |     |       |        |Home     |         |-        |   |         |
+|00|12 05:17:|317 |-1.0  |-1   |Clear  |Monday  |(private)|40.833165|73.941860|126|Residence|
+|_ _|_1_8_ _ _ _ _ _ _ _|_ _ _ _ _|_ _ _ _ _ _ _|_ _ _ _ _ _|_ _ _ _ _ _ _ _|_ _ _ _ _ _ _ _ _|_ _ _ _ _ _ _ _ _ _|_ _ _ _ _ _ _ _ _ _|_ _ _ _ _ _ _ _ _ _|_ _ _ _|_ _ _ _ _ _ _ _ _ |
+| |2012-11- |    |      |     |       |        |Deli /   |         |-        |   |         |
+|11|12 23:24:|1404|8.2   |1    |Clouds |Monday  |Bodega   |40.834098|73.945267|126|Food     |
+|_ _|_5_5_ _ _ _ _ _ _ _|_ _ _ _ _|_ _ _ _ _ _ _|_ _ _ _ _ _|_ _ _ _ _ _ _ _|_ _ _ _ _ _ _ _ _|_ _ _ _ _ _ _ _ _ _|_ _ _ _ _ _ _ _ _ _|_ _ _ _ _ _ _ _ _ _|_ _ _ _|_ _ _ _ _ _ _ _ _ |
+| |2012-11- |    |      |     |       |        |Home     |         |-        |   |         |
+|22|13 00:00:|0   |-1.0  |-1   |Clouds |Tuesday |(private)|40.833165|73.941860|126|Residence|
+|_ _|_0_7_ _ _ _ _ _ _ _|_ _ _ _ _|_ _ _ _ _ _ _|_ _ _ _ _ _|_ _ _ _ _ _ _ _|_ _ _ _ _ _ _ _ _|_ _ _ _ _ _ _ _ _ _|_ _ _ _ _ _ _ _ _ _|_ _ _ _ _ _ _ _ _ _|_ _ _ _|_ _ _ _ _ _ _ _ _ |
+| |2012-11- |    |      |     |       |        |Fried    |         |-        |   |         |
+|33|15 17:49:|1069|6.6   |3    |Clear  |Thursday|Chicken  |40.764696|73.885197|126|Food     |
+|_ _|_0_1_ _ _ _ _ _ _ _|_ _ _ _ _|_ _ _ _ _ _ _|_ _ _ _ _ _|_ _ _ _ _ _ _ _|_ _ _ _ _ _ _ _ _|_J_o_i_n_t_ _ _ _ _|_ _ _ _ _ _ _ _ _ _|_ _ _ _ _ _ _ _ _ _|_ _ _ _|_ _ _ _ _ _ _ _ _ |
+| |2012-11- |    |      |     |       |        |Bus      |         |-        |   |Travel & |
+|44|15 18:40:|1120|-1.0  |-1   |Clear  |Thursday|Station  |40.766079|73.883529|126|Transport|
+|_ _|_1_6_ _ _ _ _ _ _ _|_ _ _ _ _|_ _ _ _ _ _ _|_ _ _ _ _ _|_ _ _ _ _ _ _ _|_ _ _ _ _ _ _ _ _|_ _ _ _ _ _ _ _ _ _|_ _ _ _ _ _ _ _ _ _|_ _ _ _ _ _ _ _ _ _|_ _ _ _|_ _ _ _ _ _ _ _ _ |
+If you want to save, indicate the output format and data path:
+In [24]:
+trainTestSplit(df, data_path=data_path, outformats=['csv', 'parquet'])
+
+# Reading:
+df = readDataset(data_path, file='train.parquet')
 df.head()
-Joining train and test data from... automatize/assets/examples/Example/data
+  0%|          | 0/9 [00:00<?, ?it/s]
+Writing - CSV |TRAIN -
+Writing - CSV |TEST -
+Writing - Parquet |TRAIN -
+Writing - Parquet |TEST -
+Out[24]:
+ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ 
+|_ _|_dd_aa_tt_ee____tt_ii_mm_ee_|_tt_ii_mm_ee_|_rr_aa_tt_ii_nn_gg_|_pp_rr_ii_cc_ee_|_ww_ee_aa_tt_hh_ee_rr_|_ _ _ _ _ _dd_aa_yy_|_ _ _ _ _ _tt_yy_pp_ee_|_ _ _ _ _ _ _ll_aa_tt_|_ _ _ _ _ _ _ll_oo_nn_|_tt_ii_dd_|_ _ _ _ _ll_aa_bb_ee_ll|
+| |2012-11- |    |      |     |       |        |Home     |         |-        |   |         |
+|00|12 05:17:|317 |-1.0  |-1   |Clear  |Monday  |(private)|40.833165|73.941860|126|Residence|
+|_ _|_1_8_ _ _ _ _ _ _ _|_ _ _ _ _|_ _ _ _ _ _ _|_ _ _ _ _ _|_ _ _ _ _ _ _ _|_ _ _ _ _ _ _ _ _|_ _ _ _ _ _ _ _ _ _|_ _ _ _ _ _ _ _ _ _|_ _ _ _ _ _ _ _ _ _|_ _ _ _|_ _ _ _ _ _ _ _ _ |
+| |2012-11- |    |      |     |       |        |Deli /   |         |-        |   |         |
+|11|12 23:24:|1404|8.2   |1    |Clouds |Monday  |Bodega   |40.834098|73.945267|126|Food     |
+|_ _|_5_5_ _ _ _ _ _ _ _|_ _ _ _ _|_ _ _ _ _ _ _|_ _ _ _ _ _|_ _ _ _ _ _ _ _|_ _ _ _ _ _ _ _ _|_ _ _ _ _ _ _ _ _ _|_ _ _ _ _ _ _ _ _ _|_ _ _ _ _ _ _ _ _ _|_ _ _ _|_ _ _ _ _ _ _ _ _ |
+| |2012-11- |    |      |     |       |        |Home     |         |-        |   |         |
+|22|13 00:00:|0   |-1.0  |-1   |Clouds |Tuesday |(private)|40.833165|73.941860|126|Residence|
+|_ _|_0_7_ _ _ _ _ _ _ _|_ _ _ _ _|_ _ _ _ _ _ _|_ _ _ _ _ _|_ _ _ _ _ _ _ _|_ _ _ _ _ _ _ _ _|_ _ _ _ _ _ _ _ _ _|_ _ _ _ _ _ _ _ _ _|_ _ _ _ _ _ _ _ _ _|_ _ _ _|_ _ _ _ _ _ _ _ _ |
+| |2012-11- |    |      |     |       |        |Fried    |         |-        |   |         |
+|33|15 17:49:|1069|6.6   |3    |Clear  |Thursday|Chicken  |40.764696|73.885197|126|Food     |
+|_ _|_0_1_ _ _ _ _ _ _ _|_ _ _ _ _|_ _ _ _ _ _ _|_ _ _ _ _ _|_ _ _ _ _ _ _ _|_ _ _ _ _ _ _ _ _|_J_o_i_n_t_ _ _ _ _|_ _ _ _ _ _ _ _ _ _|_ _ _ _ _ _ _ _ _ _|_ _ _ _|_ _ _ _ _ _ _ _ _ |
+| |2012-11- |    |      |     |       |        |Bus      |         |-        |   |Travel & |
+|44|15 18:40:|1120|-1.0  |-1   |Clear  |Thursday|Station  |40.766079|73.883529|126|Transport|
+|_ _|_1_6_ _ _ _ _ _ _ _|_ _ _ _ _|_ _ _ _ _ _ _|_ _ _ _ _ _|_ _ _ _ _ _ _ _|_ _ _ _ _ _ _ _ _|_ _ _ _ _ _ _ _ _ _|_ _ _ _ _ _ _ _ _ _|_ _ _ _ _ _ _ _ _ _|_ _ _ _|_ _ _ _ _ _ _ _ _ |
+To k-fold split a dataset into train and test:
+In [25]:
+train, test = kfold_trainTestSplit(df, k=3)
+
+for k in range(len(train)):
+    print('Shape train/test:', train[k].shape, test[k].shape)
+Spliting Data:   0%|          | 0/10 [00:00<?, ?it/s]
+Shape train/test: (174636, 11) (86969, 11)
+Shape train/test: (175715, 11) (85890, 11)
+Shape train/test: (172859, 11) (88746, 11)
+c) Stratifying the data (example to get 50% of the dataset):
+In [26]:
+train, test = stratify(df, sample_size=0.5)
+
+print('Shape train/test:', train.shape, test.shape)
+train.head()
+  0%|          | 0/9 [00:00<?, ?it/s]
+  0%|          | 0/9 [00:00<?, ?it/s]
+Shape train/test: (16432, 11) (7106, 11)
+Out[26]:
+ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ 
+|_ _|_dd_aa_tt_ee____tt_ii_mm_ee_|_tt_ii_mm_ee_|_rr_aa_tt_ii_nn_gg_|_pp_rr_ii_cc_ee_|_ww_ee_aa_tt_hh_ee_rr_|_ _ _ _ _ _dd_aa_yy_|_ _ _ _ _ _tt_yy_pp_ee_|_ _ _ _ _ _ _ll_aa_tt_|_ _ _ _ _ _ _ll_oo_nn_|_tt_ii_dd_|_ _ _ _ _ll_aa_bb_ee_ll|
+| |2012-11- |    |      |     |       |        |Home     |         |-        |   |         |
+|00|12 05:17:|317 |-1.0  |-1   |Clear  |Monday  |(private)|40.833165|73.941860|126|Residence|
+|_ _|_1_8_ _ _ _ _ _ _ _|_ _ _ _ _|_ _ _ _ _ _ _|_ _ _ _ _ _|_ _ _ _ _ _ _ _|_ _ _ _ _ _ _ _ _|_ _ _ _ _ _ _ _ _ _|_ _ _ _ _ _ _ _ _ _|_ _ _ _ _ _ _ _ _ _|_ _ _ _|_ _ _ _ _ _ _ _ _ |
+| |2012-11- |    |      |     |       |        |Deli /   |         |-        |   |         |
+|11|12 23:24:|1404|8.2   |1    |Clouds |Monday  |Bodega   |40.834098|73.945267|126|Food     |
+|_ _|_5_5_ _ _ _ _ _ _ _|_ _ _ _ _|_ _ _ _ _ _ _|_ _ _ _ _ _|_ _ _ _ _ _ _ _|_ _ _ _ _ _ _ _ _|_ _ _ _ _ _ _ _ _ _|_ _ _ _ _ _ _ _ _ _|_ _ _ _ _ _ _ _ _ _|_ _ _ _|_ _ _ _ _ _ _ _ _ |
+| |2012-11- |    |      |     |       |        |Home     |         |-        |   |         |
+|22|13 00:00:|0   |-1.0  |-1   |Clouds |Tuesday |(private)|40.833165|73.941860|126|Residence|
+|_ _|_0_7_ _ _ _ _ _ _ _|_ _ _ _ _|_ _ _ _ _ _ _|_ _ _ _ _ _|_ _ _ _ _ _ _ _|_ _ _ _ _ _ _ _ _|_ _ _ _ _ _ _ _ _ _|_ _ _ _ _ _ _ _ _ _|_ _ _ _ _ _ _ _ _ _|_ _ _ _|_ _ _ _ _ _ _ _ _ |
+| |2012-11- |    |      |     |       |        |Fried    |         |-        |   |         |
+|33|15 17:49:|1069|6.6   |3    |Clear  |Thursday|Chicken  |40.764696|73.885197|126|Food     |
+|_ _|_0_1_ _ _ _ _ _ _ _|_ _ _ _ _|_ _ _ _ _ _ _|_ _ _ _ _ _|_ _ _ _ _ _ _ _|_ _ _ _ _ _ _ _ _|_J_o_i_n_t_ _ _ _ _|_ _ _ _ _ _ _ _ _ _|_ _ _ _ _ _ _ _ _ _|_ _ _ _|_ _ _ _ _ _ _ _ _ |
+| |2012-11- |    |      |     |       |        |Bus      |         |-        |   |Travel & |
+|44|15 18:40:|1120|-1.0  |-1   |Clear  |Thursday|Station  |40.766079|73.883529|126|Transport|
+|_ _|_1_6_ _ _ _ _ _ _ _|_ _ _ _ _|_ _ _ _ _ _ _|_ _ _ _ _ _|_ _ _ _ _ _ _ _|_ _ _ _ _ _ _ _ _|_ _ _ _ _ _ _ _ _ _|_ _ _ _ _ _ _ _ _ _|_ _ _ _ _ _ _ _ _ _|_ _ _ _|_ _ _ _ _ _ _ _ _ |
+k-Fold Stratifying the data (example to get 50% of the dataset in 3-folds):
+In [27]:
+train, test = klabels_stratify(df, kl=5)
+
+print('Shape train/test:', train.shape, test.shape)
+
+
+print('Labels before:', df.label.unique())
+print('Labels after:', train.label.unique())
+  0%|          | 0/5 [00:00<?, ?it/s]
+Shape train/test: (25824, 11) (11704, 11)
+Labels before: ['Residence' 'Food' 'Travel & Transport' 'Professional & Other
+Places'
+ 'Shop & Service' 'Outdoors & Recreation' 'College & University'
+ 'Arts & Entertainment' 'Nightlife Spot' 'Event']
+Labels after: ['Residence' 'Food' 'Travel & Transport' 'Professional & Other
+Places'
+ 'Shop & Service']
+d) Joining train and test files:
+In [28]:
+df = joinTrainTest(data_path, train_file="train.csv", test_file="test.csv",
+to_file=True) # Saves 'joined.csv' file
+
+df.head()
+Joining train and test data from... matdata/assets/sample
+Saving joined dataset as: matdata/assets/sample/joined.csv
 Done.
  ------------------------------------------------------------------------------
 --
-Out[10]:
- _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ 
-|_ _|_tt_ii_dd_|_ll_aa_tt____ll_oo_nn_|_hh_oo_uu_rr_|_pp_rr_ii_cc_ee_|_ _ _ _ _ _ _ _pp_oo_ii_|_ww_ee_aa_tt_hh_ee_rr_|_ _ _ _dd_aa_yy_|_ _ _ _ _ _ _ _ll_aa_bb_ee_ll|
-|_00_|_1_2_ _|_0_._0_ _6_._2_|_8_ _ _ _|_-_1_ _ _ _|_H_o_m_e_ _ _ _ _ _ _|_C_l_e_a_r_ _ _|_M_o_n_d_a_y_|_C_l_a_s_s_s___F_a_l_s_e|
-|_11_|_1_2_ _|_0_._8_ _6_._2_|_9_ _ _ _|_2_ _ _ _ _|_U_n_i_v_e_r_s_i_t_y_|_C_l_o_u_d_s_ _|_M_o_n_d_a_y_|_C_l_a_s_s_s___F_a_l_s_e|
-|_22_|_1_2_ _|_3_._1_ _1_1_ _|_1_2_ _ _|_2_ _ _ _ _|_R_e_s_t_a_u_r_a_n_t_|_C_l_e_a_r_ _ _|_M_o_n_d_a_y_|_C_l_a_s_s_s___F_a_l_s_e|
-|_33_|_1_2_ _|_0_._8_ _6_._5_|_1_3_ _ _|_2_ _ _ _ _|_U_n_i_v_e_r_s_i_t_y_|_C_l_e_a_r_ _ _|_M_o_n_d_a_y_|_C_l_a_s_s_s___F_a_l_s_e|
-|_44_|_1_2_ _|_0_._2_ _6_._2_|_1_7_ _ _|_-_1_ _ _ _|_H_o_m_e_ _ _ _ _ _ _|_R_a_i_n_ _ _ _|_M_o_n_d_a_y_|_C_l_a_s_s_s___F_a_l_s_e|
-To k-fold split a dataset into train and test:
-In [11]:
-k = 3
+Out[28]:
+ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ 
+|_ _|_dd_aa_tt_ee____tt_ii_mm_ee_|_tt_ii_mm_ee_|_rr_aa_tt_ii_nn_gg_|_pp_rr_ii_cc_ee_|_ww_ee_aa_tt_hh_ee_rr_|_ _ _ _ _ _dd_aa_yy_|_ _ _ _ _ _tt_yy_pp_ee_|_ _ _ _ _ _ _ll_aa_tt_|_ _ _ _ _ _ _ll_oo_nn_|_tt_ii_dd_|_ _ _ _ _ll_aa_bb_ee_ll|
+| |2012-11- |    |      |     |       |        |Home     |         |-        |   |         |
+|00|12 05:17:|317 |-1.0  |-1   |Clear  |Monday  |(private)|40.833165|73.941860|126|Residence|
+|_ _|_1_8_ _ _ _ _ _ _ _|_ _ _ _ _|_ _ _ _ _ _ _|_ _ _ _ _ _|_ _ _ _ _ _ _ _|_ _ _ _ _ _ _ _ _|_ _ _ _ _ _ _ _ _ _|_ _ _ _ _ _ _ _ _ _|_ _ _ _ _ _ _ _ _ _|_ _ _ _|_ _ _ _ _ _ _ _ _ |
+| |2012-11- |    |      |     |       |        |Deli /   |         |-        |   |         |
+|11|12 23:24:|1404|8.2   |1    |Clouds |Monday  |Bodega   |40.834098|73.945267|126|Food     |
+|_ _|_5_5_ _ _ _ _ _ _ _|_ _ _ _ _|_ _ _ _ _ _ _|_ _ _ _ _ _|_ _ _ _ _ _ _ _|_ _ _ _ _ _ _ _ _|_ _ _ _ _ _ _ _ _ _|_ _ _ _ _ _ _ _ _ _|_ _ _ _ _ _ _ _ _ _|_ _ _ _|_ _ _ _ _ _ _ _ _ |
+| |2012-11- |    |      |     |       |        |Home     |         |-        |   |         |
+|22|13 00:00:|0   |-1.0  |-1   |Clouds |Tuesday |(private)|40.833165|73.941860|126|Residence|
+|_ _|_0_7_ _ _ _ _ _ _ _|_ _ _ _ _|_ _ _ _ _ _ _|_ _ _ _ _ _|_ _ _ _ _ _ _ _|_ _ _ _ _ _ _ _ _|_ _ _ _ _ _ _ _ _ _|_ _ _ _ _ _ _ _ _ _|_ _ _ _ _ _ _ _ _ _|_ _ _ _|_ _ _ _ _ _ _ _ _ |
+| |2012-11- |    |      |     |       |        |Fried    |         |-        |   |         |
+|33|15 17:49:|1069|6.6   |3    |Clear  |Thursday|Chicken  |40.764696|73.885197|126|Food     |
+|_ _|_0_1_ _ _ _ _ _ _ _|_ _ _ _ _|_ _ _ _ _ _ _|_ _ _ _ _ _|_ _ _ _ _ _ _ _|_ _ _ _ _ _ _ _ _|_J_o_i_n_t_ _ _ _ _|_ _ _ _ _ _ _ _ _ _|_ _ _ _ _ _ _ _ _ _|_ _ _ _|_ _ _ _ _ _ _ _ _ |
+| |2012-11- |    |      |     |       |        |Bus      |         |-        |   |Travel & |
+|44|15 18:40:|1120|-1.0  |-1   |Clear  |Thursday|Station  |40.766079|73.883529|126|Transport|
+|_ _|_1_6_ _ _ _ _ _ _ _|_ _ _ _ _|_ _ _ _ _ _ _|_ _ _ _ _ _|_ _ _ _ _ _ _ _|_ _ _ _ _ _ _ _ _|_ _ _ _ _ _ _ _ _ _|_ _ _ _ _ _ _ _ _ _|_ _ _ _ _ _ _ _ _ _|_ _ _ _|_ _ _ _ _ _ _ _ _ |
+NNoottee:: We standardized all repository datasets by creating a data.parquet file
+with np.NaN as missing values, as example:
+In [29]:
+from matdata.preprocess import *
+from matdata.dataset import prepare_ds
+import numpy as np
 
-train, test = kfold_trainAndTestSplit(data_path, k, df, random_num=1,
-class_col='label')
-3-fold train and test split in... automatize/assets/examples/Example/data
-Spliting Data:   0%|          | 0/2 [00:00<?, ?it/s]
-Done.
-Writing files ... 1/3
-Writing TRAIN - ZIP|1:   0%|          | 0/7 [00:00<?, ?it/s]
-Writing TEST  - ZIP|1:   0%|          | 0/4 [00:00<?, ?it/s]
-Writing TRAIN / TEST - CSV|1
-Writing TRAIN - MAT|1:   0%|          | 0/7 [00:00<?, ?it/s]
-Writing TEST  - MAT|1:   0%|          | 0/4 [00:00<?, ?it/s]
-Writing files ... 2/3
-Writing TRAIN - ZIP|2:   0%|          | 0/7 [00:00<?, ?it/s]
-Writing TEST  - ZIP|2:   0%|          | 0/4 [00:00<?, ?it/s]
-Writing TRAIN / TEST - CSV|2
-Writing TRAIN - MAT|2:   0%|          | 0/7 [00:00<?, ?it/s]
-Writing TEST  - MAT|2:   0%|          | 0/4 [00:00<?, ?it/s]
-Writing files ... 3/3
-Writing TRAIN - ZIP|3:   0%|          | 0/8 [00:00<?, ?it/s]
-Writing TEST  - ZIP|3:   0%|          | 0/3 [00:00<?, ?it/s]
-Writing TRAIN / TEST - CSV|3
-Writing TRAIN - MAT|3:   0%|          | 0/8 [00:00<?, ?it/s]
-Writing TEST  - MAT|3:   0%|          | 0/3 [00:00<?, ?it/s]
+data_path = 'matdata/assets/sample'
+
+df.replace('?', np.NaN, inplace=True)
+
+df = prepare_ds(df)
+
+df2parquet(df, data_path, 'data')
+Saving dataset as: matdata/assets/sample/data.parquet
 Done.
  ------------------------------------------------------------------------------
 --
-To convert train and test from one available format to other default formats
-(CSV, ZIP, MAT):
-In [4]:
-convertDataset(data_path)
-Writing TRAIN - ZIP|:   0%|          | 0/14 [00:00<?, ?it/s]
-Writing TEST  - ZIP|:   0%|          | 0/14 [00:00<?, ?it/s]
-Writing TRAIN - MAT|:   0%|          | 0/14 [00:00<?, ?it/s]
-Writing TEST  - MAT|:   0%|          | 0/14 [00:00<?, ?it/s]
-All Done.
-******** 22.. SSyynntthheettiicc DDaattaa GGeenneerraattiioonn_?¶ ********
+Out[29]:
+ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ 
+|_ _ _ _ _ _|_dd_aa_tt_ee____tt_ii_mm_ee_|_tt_ii_mm_ee_|_rr_aa_tt_ii_nn_gg_|_pp_rr_ii_cc_ee_|_ww_ee_aa_tt_hh_ee_rr_|_ _ _ _ _ _dd_aa_yy_|_ _ _ _ _ _ _tt_yy_pp_ee_|_ _ _ _ _ _ _ll_aa_tt_|_ _ _ _ _ _ _ll_oo_nn_|_ _ _ _ _ _ll_aa_bb_ee_ll_|_ _ _tt_ii_dd|
+|     |2012-11- |    |      |     |       |        |Home      |         |-        |          |     |
+|00    |12 05:17:|317 |-1.0  |-1   |Clear  |Monday  |(private) |40.833165|73.941860|Residence |126  |
+|_ _ _ _ _ _|_1_8_ _ _ _ _ _ _ _|_ _ _ _ _|_ _ _ _ _ _ _|_ _ _ _ _ _|_ _ _ _ _ _ _ _|_ _ _ _ _ _ _ _ _|_ _ _ _ _ _ _ _ _ _ _|_ _ _ _ _ _ _ _ _ _|_ _ _ _ _ _ _ _ _ _|_ _ _ _ _ _ _ _ _ _ _|_ _ _ _ _ |
+|     |2012-11- |    |      |     |       |        |Deli /    |         |-        |          |     |
+|11    |12 23:24:|1404|8.2   |1    |Clouds |Monday  |Bodega    |40.834098|73.945267|Food      |126  |
+|_ _ _ _ _ _|_5_5_ _ _ _ _ _ _ _|_ _ _ _ _|_ _ _ _ _ _ _|_ _ _ _ _ _|_ _ _ _ _ _ _ _|_ _ _ _ _ _ _ _ _|_ _ _ _ _ _ _ _ _ _ _|_ _ _ _ _ _ _ _ _ _|_ _ _ _ _ _ _ _ _ _|_ _ _ _ _ _ _ _ _ _ _|_ _ _ _ _ |
+|     |2012-11- |    |      |     |       |        |Home      |         |-        |          |     |
+|22    |13 00:00:|0   |-1.0  |-1   |Clouds |Tuesday |(private) |40.833165|73.941860|Residence |126  |
+|_ _ _ _ _ _|_0_7_ _ _ _ _ _ _ _|_ _ _ _ _|_ _ _ _ _ _ _|_ _ _ _ _ _|_ _ _ _ _ _ _ _|_ _ _ _ _ _ _ _ _|_ _ _ _ _ _ _ _ _ _ _|_ _ _ _ _ _ _ _ _ _|_ _ _ _ _ _ _ _ _ _|_ _ _ _ _ _ _ _ _ _ _|_ _ _ _ _ |
+|     |2012-11- |    |      |     |       |        |Fried     |         |-        |          |     |
+|33    |15 17:49:|1069|6.6   |3    |Clear  |Thursday|Chicken   |40.764696|73.885197|Food      |126  |
+|_ _ _ _ _ _|_0_1_ _ _ _ _ _ _ _|_ _ _ _ _|_ _ _ _ _ _ _|_ _ _ _ _ _|_ _ _ _ _ _ _ _|_ _ _ _ _ _ _ _ _|_J_o_i_n_t_ _ _ _ _ _|_ _ _ _ _ _ _ _ _ _|_ _ _ _ _ _ _ _ _ _|_ _ _ _ _ _ _ _ _ _ _|_ _ _ _ _ |
+|     |2012-11- |    |      |     |       |        |Bus       |         |-        |Travel &  |     |
+|44    |15 18:40:|1120|-1.0  |-1   |Clear  |Thursday|Station   |40.766079|73.883529|Transport |126  |
+|_ _ _ _ _ _|_1_6_ _ _ _ _ _ _ _|_ _ _ _ _|_ _ _ _ _ _ _|_ _ _ _ _ _|_ _ _ _ _ _ _ _|_ _ _ _ _ _ _ _ _|_ _ _ _ _ _ _ _ _ _ _|_ _ _ _ _ _ _ _ _ _|_ _ _ _ _ _ _ _ _ _|_ _ _ _ _ _ _ _ _ _ _|_ _ _ _ _ |
+|_.._.._.._ _ _|_._._._ _ _ _ _ _ _|_._._._ _|_._._._ _ _ _|_._._._ _ _|_._._._ _ _ _ _|_._._._ _ _ _ _ _|_._._._ _ _ _ _ _ _ _|_._._._ _ _ _ _ _ _|_._._._ _ _ _ _ _ _|_._._._ _ _ _ _ _ _ _|_._._._ _ |
+|     |2012-08- |    |      |     |       |        |General   |         |-        |College & |     |
+|2200008800|10 17:17:|1037|-1.0  |-1   |Clouds |Friday  |College & |40.704733|73.987738|University|29563|
+|_ _ _ _ _ _|_3_7_ _ _ _ _ _ _ _|_ _ _ _ _|_ _ _ _ _ _ _|_ _ _ _ _ _|_ _ _ _ _ _ _ _|_ _ _ _ _ _ _ _ _|_U_n_i_v_e_r_s_i_t_y_|_ _ _ _ _ _ _ _ _ _|_ _ _ _ _ _ _ _ _ _|_ _ _ _ _ _ _ _ _ _ _|_ _ _ _ _ |
+|     |2012-08- |    |      |     |       |        |Thai      |         |-        |          |     |
+|2200008811|10 20:10:|1210|8.0   |2    |Clouds |Friday  |Restaurant|40.695163|73.995448|Food      |29563|
+|_ _ _ _ _ _|_5_9_ _ _ _ _ _ _ _|_ _ _ _ _|_ _ _ _ _ _ _|_ _ _ _ _ _|_ _ _ _ _ _ _ _|_ _ _ _ _ _ _ _ _|_ _ _ _ _ _ _ _ _ _ _|_ _ _ _ _ _ _ _ _ _|_ _ _ _ _ _ _ _ _ _|_ _ _ _ _ _ _ _ _ _ _|_ _ _ _ _ |
+|     |2012-08- |    |      |     |       |        |          |         |-        |Outdoors &|     |
+|2200008822|11 08:01:|481 |6.9   |-1   |Clouds |Saturday|Gym       |40.697803|73.994145|Recreation|29563|
+|_ _ _ _ _ _|_2_0_ _ _ _ _ _ _ _|_ _ _ _ _|_ _ _ _ _ _ _|_ _ _ _ _ _|_ _ _ _ _ _ _ _|_ _ _ _ _ _ _ _ _|_ _ _ _ _ _ _ _ _ _ _|_ _ _ _ _ _ _ _ _ _|_ _ _ _ _ _ _ _ _ _|_ _ _ _ _ _ _ _ _ _ _|_ _ _ _ _ |
+|     |2012-08- |    |      |     |       |        |Coffee    |         |-        |          |     |
+|2200008833|11 13:39:|819 |7.0   |1    |Clouds |Saturday|Shop      |40.694673|73.994082|Food      |29563|
+|_ _ _ _ _ _|_3_9_ _ _ _ _ _ _ _|_ _ _ _ _|_ _ _ _ _ _ _|_ _ _ _ _ _|_ _ _ _ _ _ _ _|_ _ _ _ _ _ _ _ _|_ _ _ _ _ _ _ _ _ _ _|_ _ _ _ _ _ _ _ _ _|_ _ _ _ _ _ _ _ _ _|_ _ _ _ _ _ _ _ _ _ _|_ _ _ _ _ |
+|     |2012-08- |    |      |     |       |        |          |         |-        |Outdoors &|     |
+|2200008844|12 07:56:|476 |6.9   |-1   |Clouds |Sunday  |Gym       |40.697803|73.994145|Recreation|29563|
+|_ _ _ _ _ _|_2_6_ _ _ _ _ _ _ _|_ _ _ _ _|_ _ _ _ _ _ _|_ _ _ _ _ _|_ _ _ _ _ _ _ _|_ _ _ _ _ _ _ _ _|_ _ _ _ _ _ _ _ _ _ _|_ _ _ _ _ _ _ _ _ _|_ _ _ _ _ _ _ _ _ _|_ _ _ _ _ _ _ _ _ _ _|_ _ _ _ _ |
+66962 rows × 11 columns
+******** 44.. SSyynntthheettiicc DDaattaa GGeenneerraattiioonn_?¶ ********
 TODO
-In [5]:
+In [1]:
 from matdata.generator import *
     * scalerSamplerGenerator: generates trajectory datasets based on real data
       on scale intervals
     * samplerGenerator: generate a trajectory dataset based on real data
     * scalerRandomGenerator: generates trajectory datasets based on random data
       on scale intervals
     * randomGenerator: generate a trajectory dataset based on random data
-In [ ]:
+a) To generate a sample dataset (default config):
+In [2]:
+samplerGenerator()
+Out[2]:
+ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ 
+|_ _ _ _|_tt_ii_dd_|_ _ _ _ _ _ _ _ _ _ _ _ss_pp_aa_cc_ee_|_tt_ii_mm_ee_|_ _ _ _ _ _dd_aa_yy_|_rr_aa_tt_ii_nn_gg_|_pp_rr_ii_cc_ee_|_ww_ee_aa_tt_hh_ee_rr_|_ _ _ _ _rr_oo_oo_tt____tt_yy_pp_ee_|_ _ _ _ _ _ _ _tt_yy_pp_ee_|_ll_aa_bb_ee_ll|
+|   |   |40.7429692382286|    |        |      |     |       |Shop &       |           |     |
+|00  |1  |-               |447 |Monday  |6.1   |-1   |Clouds |Service      |Supermarket|C1   |
+|_ _ _ _|_ _ _ _|_7_3_._8_8_2_7_6_6_9_6_2_0_5_1_4_|_ _ _ _ _|_ _ _ _ _ _ _ _ _|_ _ _ _ _ _ _|_ _ _ _ _ _|_ _ _ _ _ _ _ _|_ _ _ _ _ _ _ _ _ _ _ _ _ _|_ _ _ _ _ _ _ _ _ _ _ _|_ _ _ _ _ |
+|   |   |40.8610785519472|    |        |      |     |       |             |Home       |     |
+|11  |1  |-               |486 |Monday  |-1.0  |-1   |Clouds |Residence    |(private)  |C1   |
+|_ _ _ _|_ _ _ _|_7_3_._9_3_0_1_0_3_7_0_7_6_3_1_5_|_ _ _ _ _|_ _ _ _ _ _ _ _ _|_ _ _ _ _ _ _|_ _ _ _ _ _|_ _ _ _ _ _ _ _|_ _ _ _ _ _ _ _ _ _ _ _ _ _|_ _ _ _ _ _ _ _ _ _ _ _|_ _ _ _ _ |
+|   |   |40.5774555812085|    |        |      |     |       |Travel &     |Metro      |     |
+|22  |1  |-               |653 |Monday  |-1.0  |-1   |Clear  |Transport    |Station    |C1   |
+|_ _ _ _|_ _ _ _|_7_3_._9_8_1_2_4_6_9_4_8_2_4_2_2_|_ _ _ _ _|_ _ _ _ _ _ _ _ _|_ _ _ _ _ _ _|_ _ _ _ _ _|_ _ _ _ _ _ _ _|_ _ _ _ _ _ _ _ _ _ _ _ _ _|_ _ _ _ _ _ _ _ _ _ _ _|_ _ _ _ _ |
+|   |   |40.8114381522955|    |        |      |     |       |Arts &       |           |     |
+|33  |1  |-               |701 |Monday  |6.8   |-1   |Rain   |Entertainment|Stadium    |C1   |
+|_ _ _ _|_ _ _ _|_7_4_._0_6_7_7_9_6_4_6_8_7_3_4_7_|_ _ _ _ _|_ _ _ _ _ _ _ _ _|_ _ _ _ _ _ _|_ _ _ _ _ _|_ _ _ _ _ _ _ _|_ _ _ _ _ _ _ _ _ _ _ _ _ _|_ _ _ _ _ _ _ _ _ _ _ _|_ _ _ _ _ |
+|   |   |40.7811844364976|    |        |      |     |       |Arts &       |Science    |     |
+|44  |1  |-               |758 |Monday  |9.4   |-1   |Clear  |Entertainment|Museum     |C1   |
+|_ _ _ _|_ _ _ _|_7_3_._9_7_3_2_0_3_0_9_3_0_0_6_5_|_ _ _ _ _|_ _ _ _ _ _ _ _ _|_ _ _ _ _ _ _|_ _ _ _ _ _|_ _ _ _ _ _ _ _|_ _ _ _ _ _ _ _ _ _ _ _ _ _|_ _ _ _ _ _ _ _ _ _ _ _|_ _ _ _ _ |
+|_.._.._.._|_._._._|_._._._ _ _ _ _ _ _ _ _ _ _ _ _ _|_._._._ _|_._._._ _ _ _ _ _|_._._._ _ _ _|_._._._ _ _|_._._._ _ _ _ _|_._._._ _ _ _ _ _ _ _ _ _ _|_._._._ _ _ _ _ _ _ _ _|_._._._ _ |
+|   |   |40.7638885711179|    |        |      |     |       |Travel &     |Border     |     |
+|449955|10 |-               |1385|Saturday|-1.0  |-1   |Clouds |Transport    |Crossing   |C1   |
+|_ _ _ _|_ _ _ _|_7_4_._0_2_3_3_8_2_1_8_0_8_3_5_2_|_ _ _ _ _|_ _ _ _ _ _ _ _ _|_ _ _ _ _ _ _|_ _ _ _ _ _|_ _ _ _ _ _ _ _|_ _ _ _ _ _ _ _ _ _ _ _ _ _|_ _ _ _ _ _ _ _ _ _ _ _|_ _ _ _ _ |
+|   |   |40.6891441345215|    |        |      |     |       |             |Deli /     |     |
+|449966|10 |-               |379 |Sunday  |-1.0  |1    |Clouds |Food         |Bodega     |C1   |
+|_ _ _ _|_ _ _ _|_7_3_._9_3_0_3_2_0_7_3_9_7_4_6_1_|_ _ _ _ _|_ _ _ _ _ _ _ _ _|_ _ _ _ _ _ _|_ _ _ _ _ _|_ _ _ _ _ _ _ _|_ _ _ _ _ _ _ _ _ _ _ _ _ _|_ _ _ _ _ _ _ _ _ _ _ _|_ _ _ _ _ |
+|   |   |40.7704703500000|    |        |      |     |       |Professional |           |     |
+|449977|10 |-               |547 |Sunday  |-1.0  |-1   |Clear  |& Other      |Post Office|C1   |
+|_ _ _ _|_ _ _ _|_7_4_._0_2_8_1_8_3_1_4_0_0_0_0_0_|_ _ _ _ _|_ _ _ _ _ _ _ _ _|_ _ _ _ _ _ _|_ _ _ _ _ _|_ _ _ _ _ _ _ _|_P_l_a_c_e_s_ _ _ _ _ _ _ _|_ _ _ _ _ _ _ _ _ _ _ _|_ _ _ _ _ |
+|   |   |40.7774773922087|    |        |      |     |       |Shop &       |           |     |
+|449988|10 |-               |783 |Sunday  |-1.0  |-1   |Clear  |Service      |Candy Store|C1   |
+|_ _ _ _|_ _ _ _|_7_3_._8_1_4_6_7_2_5_7_5_5_6_4_3_|_ _ _ _ _|_ _ _ _ _ _ _ _ _|_ _ _ _ _ _ _|_ _ _ _ _ _|_ _ _ _ _ _ _ _|_ _ _ _ _ _ _ _ _ _ _ _ _ _|_ _ _ _ _ _ _ _ _ _ _ _|_ _ _ _ _ |
+|   |   |40.8331652006224|    |        |      |     |       |             |Home       |     |
+|449999|10 |-               |1033|Sunday  |-1.0  |-1   |Clouds |Residence    |(private)  |C1   |
+|_ _ _ _|_ _ _ _|_7_3_._9_4_1_8_6_0_3_4_2_7_6_9_2_|_ _ _ _ _|_ _ _ _ _ _ _ _ _|_ _ _ _ _ _ _|_ _ _ _ _ _|_ _ _ _ _ _ _ _|_ _ _ _ _ _ _ _ _ _ _ _ _ _|_ _ _ _ _ _ _ _ _ _ _ _|_ _ _ _ _ |
+500 rows × 10 columns
+To specify the synthetic dataset parameters:
+In [3]:
+N=10 # Number of trajectories
+M=50 # Number of points by trajectory
+C=3  # Number of classes (C1 to Cn)
+samplerGenerator(N, M, C)
+Out[3]:
+ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ 
+|_ _ _ _|_tt_ii_dd_|_ _ _ _ _ _ _ _ _ _ _ _ss_pp_aa_cc_ee_|_tt_ii_mm_ee_|_ _ _ _ _ _dd_aa_yy_|_rr_aa_tt_ii_nn_gg_|_pp_rr_ii_cc_ee_|_ww_ee_aa_tt_hh_ee_rr_|_ _ _ _ _rr_oo_oo_tt____tt_yy_pp_ee_|_ _ _ _ _ _ _ _tt_yy_pp_ee_|_ll_aa_bb_ee_ll|
+|   |   |40.7429692382286|    |        |      |     |       |Shop &       |           |     |
+|00  |1  |-               |447 |Monday  |6.1   |-1   |Clouds |Service      |Supermarket|C1   |
+|_ _ _ _|_ _ _ _|_7_3_._8_8_2_7_6_6_9_6_2_0_5_1_4_|_ _ _ _ _|_ _ _ _ _ _ _ _ _|_ _ _ _ _ _ _|_ _ _ _ _ _|_ _ _ _ _ _ _ _|_ _ _ _ _ _ _ _ _ _ _ _ _ _|_ _ _ _ _ _ _ _ _ _ _ _|_ _ _ _ _ |
+|   |   |40.8610785519472|    |        |      |     |       |             |Home       |     |
+|11  |1  |-               |486 |Monday  |-1.0  |-1   |Clouds |Residence    |(private)  |C1   |
+|_ _ _ _|_ _ _ _|_7_3_._9_3_0_1_0_3_7_0_7_6_3_1_5_|_ _ _ _ _|_ _ _ _ _ _ _ _ _|_ _ _ _ _ _ _|_ _ _ _ _ _|_ _ _ _ _ _ _ _|_ _ _ _ _ _ _ _ _ _ _ _ _ _|_ _ _ _ _ _ _ _ _ _ _ _|_ _ _ _ _ |
+|   |   |40.5774555812085|    |        |      |     |       |Travel &     |Metro      |     |
+|22  |1  |-               |653 |Monday  |-1.0  |-1   |Clear  |Transport    |Station    |C1   |
+|_ _ _ _|_ _ _ _|_7_3_._9_8_1_2_4_6_9_4_8_2_4_2_2_|_ _ _ _ _|_ _ _ _ _ _ _ _ _|_ _ _ _ _ _ _|_ _ _ _ _ _|_ _ _ _ _ _ _ _|_ _ _ _ _ _ _ _ _ _ _ _ _ _|_ _ _ _ _ _ _ _ _ _ _ _|_ _ _ _ _ |
+|   |   |40.8114381522955|    |        |      |     |       |Arts &       |           |     |
+|33  |1  |-               |701 |Monday  |6.8   |-1   |Rain   |Entertainment|Stadium    |C1   |
+|_ _ _ _|_ _ _ _|_7_4_._0_6_7_7_9_6_4_6_8_7_3_4_7_|_ _ _ _ _|_ _ _ _ _ _ _ _ _|_ _ _ _ _ _ _|_ _ _ _ _ _|_ _ _ _ _ _ _ _|_ _ _ _ _ _ _ _ _ _ _ _ _ _|_ _ _ _ _ _ _ _ _ _ _ _|_ _ _ _ _ |
+|   |   |40.7811844364976|    |        |      |     |       |Arts &       |Science    |     |
+|44  |1  |-               |758 |Monday  |9.4   |-1   |Clear  |Entertainment|Museum     |C1   |
+|_ _ _ _|_ _ _ _|_7_3_._9_7_3_2_0_3_0_9_3_0_0_6_5_|_ _ _ _ _|_ _ _ _ _ _ _ _ _|_ _ _ _ _ _ _|_ _ _ _ _ _|_ _ _ _ _ _ _ _|_ _ _ _ _ _ _ _ _ _ _ _ _ _|_ _ _ _ _ _ _ _ _ _ _ _|_ _ _ _ _ |
+|_.._.._.._|_._._._|_._._._ _ _ _ _ _ _ _ _ _ _ _ _ _|_._._._ _|_._._._ _ _ _ _ _|_._._._ _ _ _|_._._._ _ _|_._._._ _ _ _ _|_._._._ _ _ _ _ _ _ _ _ _ _|_._._._ _ _ _ _ _ _ _ _|_._._._ _ |
+|   |   |40.7638885711179|    |        |      |     |       |Travel &     |Border     |     |
+|449955|11 |-               |1385|Saturday|-1.0  |-1   |Clouds |Transport    |Crossing   |C3   |
+|_ _ _ _|_ _ _ _|_7_4_._0_2_3_3_8_2_1_8_0_8_3_5_2_|_ _ _ _ _|_ _ _ _ _ _ _ _ _|_ _ _ _ _ _ _|_ _ _ _ _ _|_ _ _ _ _ _ _ _|_ _ _ _ _ _ _ _ _ _ _ _ _ _|_ _ _ _ _ _ _ _ _ _ _ _|_ _ _ _ _ |
+|   |   |40.6891441345215|    |        |      |     |       |             |Deli /     |     |
+|449966|11 |-               |379 |Sunday  |-1.0  |1    |Clouds |Food         |Bodega     |C3   |
+|_ _ _ _|_ _ _ _|_7_3_._9_3_0_3_2_0_7_3_9_7_4_6_1_|_ _ _ _ _|_ _ _ _ _ _ _ _ _|_ _ _ _ _ _ _|_ _ _ _ _ _|_ _ _ _ _ _ _ _|_ _ _ _ _ _ _ _ _ _ _ _ _ _|_ _ _ _ _ _ _ _ _ _ _ _|_ _ _ _ _ |
+|   |   |40.7704703500000|    |        |      |     |       |Professional |           |     |
+|449977|11 |-               |547 |Sunday  |-1.0  |-1   |Clear  |& Other      |Post Office|C3   |
+|_ _ _ _|_ _ _ _|_7_4_._0_2_8_1_8_3_1_4_0_0_0_0_0_|_ _ _ _ _|_ _ _ _ _ _ _ _ _|_ _ _ _ _ _ _|_ _ _ _ _ _|_ _ _ _ _ _ _ _|_P_l_a_c_e_s_ _ _ _ _ _ _ _|_ _ _ _ _ _ _ _ _ _ _ _|_ _ _ _ _ |
+|   |   |40.7774773922087|    |        |      |     |       |Shop &       |           |     |
+|449988|11 |-               |783 |Sunday  |-1.0  |-1   |Clear  |Service      |Candy Store|C3   |
+|_ _ _ _|_ _ _ _|_7_3_._8_1_4_6_7_2_5_7_5_5_6_4_3_|_ _ _ _ _|_ _ _ _ _ _ _ _ _|_ _ _ _ _ _ _|_ _ _ _ _ _|_ _ _ _ _ _ _ _|_ _ _ _ _ _ _ _ _ _ _ _ _ _|_ _ _ _ _ _ _ _ _ _ _ _|_ _ _ _ _ |
+|   |   |40.8331652006224|    |        |      |     |       |             |Home       |     |
+|449999|11 |-               |1033|Sunday  |-1.0  |-1   |Clouds |Residence    |(private)  |C3   |
+|_ _ _ _|_ _ _ _|_7_3_._9_4_1_8_6_0_3_4_2_7_6_9_2_|_ _ _ _ _|_ _ _ _ _ _ _ _ _|_ _ _ _ _ _ _|_ _ _ _ _ _|_ _ _ _ _ _ _ _|_ _ _ _ _ _ _ _ _ _ _ _ _ _|_ _ _ _ _ _ _ _ _ _ _ _|_ _ _ _ _ |
+500 rows × 10 columns
+b) To generate a set of sample datasets:
+
+Creates and save dataset files (including movelets json descriptor file).
+Generates sample datasets in a increasing log scale for each parameter. It uses
+the middle value for the other configurations
+In [4]:
+data_path = 'matdata/assets/sample/samples'
+
+Ns=[100, 3]   # Min. number of trajectories: 100, 3 scales (by log increment)
+Ms=[10,  3]   # Min. number of points: 10, 3 scales (by log increment)
+Ls=[8,   3]   # Min. number of attributes: 8, 3 scales (by log increment)
+Cs=[2,   3]   # Min. number of labels: 2, 3 scales (by log increment)
+
+scalerSamplerGenerator(Ns, Ms, Ls, Cs, save_to=data_path)
+  0%|          | 0/12 [00:00<?, ?it/s]
+N :: fix. value: 	 200 	scale:	 [100, 200, 400]
+M :: fix. value: 	 20 	scale:	 [10, 20, 40]
+L :: fix. value: 	 8 	scale:	 [8, 16, 32]
+C :: fix. value: 	 4 	scale:	 [2, 4, 8]
+Writing - CSV |
+Writing - CSV |
+Writing - CSV |
+Writing - CSV |
+Writing - CSV |
+Writing - CSV |
+Writing - CSV |
+Writing - CSV |
+Writing - CSV |
+c) To generate a random dataset (default config):
+In [5]:
+randomGenerator()
+Out[5]:
+ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ 
+|_ _ _ _|_tt_ii_dd_|_aa_11____ss_pp_aa_cc_ee_|_aa_22____tt_ii_mm_ee_|_aa_33____nn_11_|_ _aa_44____nn_22_|_aa_55____nn_oo_mm_ii_nn_aa_ll_|_ _ _ _aa_66____dd_aa_yy_|_aa_77____ww_ee_aa_tt_hh_ee_rr_|_ _ _aa_88____cc_aa_tt_ee_gg_oo_rr_yy_|_aa_99____ss_pp_aa_cc_ee_|_aa_11_00____tt_ii_mm_ee_|_ll_aa_bb_ee_ll|
+|00  |1  |134.5   |114    |949  |976.98|PX        |Tuesday  |Clouds    |Outdoors &   |101.04  |1114    |C1   |
+|_ _ _ _|_ _ _ _|_8_4_8_._2_8_ _ _|_ _ _ _ _ _ _ _|_ _ _ _ _ _|_ _ _ _ _ _ _|_ _ _ _ _ _ _ _ _ _ _|_ _ _ _ _ _ _ _ _ _|_ _ _ _ _ _ _ _ _ _ _|_R_e_c_r_e_a_t_i_o_n_ _ _ _|_7_7_8_._5_2_ _ _|_ _ _ _ _ _ _ _ _|_ _ _ _ _ |
+|11  |1  |764.54  |985    |-656 |630.77|HK        |Saturday |Clouds    |Shop &       |328.42  |83      |C1   |
+|_ _ _ _|_ _ _ _|_2_5_5_._3_2_ _ _|_ _ _ _ _ _ _ _|_ _ _ _ _ _|_ _ _ _ _ _ _|_ _ _ _ _ _ _ _ _ _ _|_ _ _ _ _ _ _ _ _ _|_ _ _ _ _ _ _ _ _ _ _|_S_e_r_v_i_c_e_ _ _ _ _ _ _|_5_0_9_._7_8_ _ _|_ _ _ _ _ _ _ _ _|_ _ _ _ _ |
+|22  |1  |495.93  |746    |344  |695.05|JM        |Saturday |Rain      |Travel &     |665.91  |1073    |C1   |
+|_ _ _ _|_ _ _ _|_4_4_9_._9_4_ _ _|_ _ _ _ _ _ _ _|_ _ _ _ _ _|_ _ _ _ _ _ _|_ _ _ _ _ _ _ _ _ _ _|_ _ _ _ _ _ _ _ _ _|_ _ _ _ _ _ _ _ _ _ _|_T_r_a_n_s_p_o_r_t_ _ _ _ _|_1_7_9_._7_5_ _ _|_ _ _ _ _ _ _ _ _|_ _ _ _ _ |
+|33  |1  |652.24  |1167   |-442 |450.85|ZO        |Wednesday|Unknown   |Nightlife    |149.71  |185     |C1   |
+|_ _ _ _|_ _ _ _|_7_8_9_._5_1_ _ _|_ _ _ _ _ _ _ _|_ _ _ _ _ _|_ _ _ _ _ _ _|_ _ _ _ _ _ _ _ _ _ _|_ _ _ _ _ _ _ _ _ _|_ _ _ _ _ _ _ _ _ _ _|_S_p_o_t_ _ _ _ _ _ _ _ _ _|_1_4_1_._6_8_ _ _|_ _ _ _ _ _ _ _ _|_ _ _ _ _ |
+|   |   |93.95   |       |     |      |          |         |          |Professional |866.41  |        |     |
+|44  |1  |28.38   |1135   |327  |523.90|CU        |Monday   |Clouds    |& Other      |305.93  |522     |C1   |
+|_ _ _ _|_ _ _ _|_ _ _ _ _ _ _ _ _|_ _ _ _ _ _ _ _|_ _ _ _ _ _|_ _ _ _ _ _ _|_ _ _ _ _ _ _ _ _ _ _|_ _ _ _ _ _ _ _ _ _|_ _ _ _ _ _ _ _ _ _ _|_P_l_a_c_e_s_ _ _ _ _ _ _ _|_ _ _ _ _ _ _ _ _|_ _ _ _ _ _ _ _ _|_ _ _ _ _ |
+|_.._.._.._|_._._._|_._._._ _ _ _ _ _|_._._._ _ _ _ _|_._._._ _ _|_._._._ _ _ _|_._._._ _ _ _ _ _ _ _|_._._._ _ _ _ _ _ _|_._._._ _ _ _ _ _ _ _|_._._._ _ _ _ _ _ _ _ _ _ _|_._._._ _ _ _ _ _|_._._._ _ _ _ _ _|_._._._ _ |
+|449955|10 |647.96  |1205   |561  |819.12|ACR       |Saturday |Rain      |Arts &       |515.96  |634     |C10  |
+|_ _ _ _|_ _ _ _|_3_0_0_._5_ _ _ _|_ _ _ _ _ _ _ _|_ _ _ _ _ _|_ _ _ _ _ _ _|_ _ _ _ _ _ _ _ _ _ _|_ _ _ _ _ _ _ _ _ _|_ _ _ _ _ _ _ _ _ _ _|_E_n_t_e_r_t_a_i_n_m_e_n_t_|_9_5_5_._6_6_ _ _|_ _ _ _ _ _ _ _ _|_ _ _ _ _ |
+|449966|10 |779.26  |485    |121  |745.32|AIZ       |Tuesday  |Rain      |Outdoors &   |377.83  |435     |C10  |
+|_ _ _ _|_ _ _ _|_9_3_3_._6_1_ _ _|_ _ _ _ _ _ _ _|_ _ _ _ _ _|_ _ _ _ _ _ _|_ _ _ _ _ _ _ _ _ _ _|_ _ _ _ _ _ _ _ _ _|_ _ _ _ _ _ _ _ _ _ _|_R_e_c_r_e_a_t_i_o_n_ _ _ _|_2_6_3_._1_3_ _ _|_ _ _ _ _ _ _ _ _|_ _ _ _ _ |
+|449977|10 |398.3   |406    |-248 |180.89|YH        |Monday   |Fog       |Event        |458.27  |874     |C10  |
+|_ _ _ _|_ _ _ _|_5_4_5_._1_9_ _ _|_ _ _ _ _ _ _ _|_ _ _ _ _ _|_ _ _ _ _ _ _|_ _ _ _ _ _ _ _ _ _ _|_ _ _ _ _ _ _ _ _ _|_ _ _ _ _ _ _ _ _ _ _|_ _ _ _ _ _ _ _ _ _ _ _ _ _|_6_6_5_._4_6_ _ _|_ _ _ _ _ _ _ _ _|_ _ _ _ _ |
+|449988|10 |133.52  |62     |-485 |890.42|DI        |Thursday |Clouds    |Residence    |263.93  |1141    |C10  |
+|_ _ _ _|_ _ _ _|_6_0_5_._0_2_ _ _|_ _ _ _ _ _ _ _|_ _ _ _ _ _|_ _ _ _ _ _ _|_ _ _ _ _ _ _ _ _ _ _|_ _ _ _ _ _ _ _ _ _|_ _ _ _ _ _ _ _ _ _ _|_ _ _ _ _ _ _ _ _ _ _ _ _ _|_9_4_4_._8_ _ _ _|_ _ _ _ _ _ _ _ _|_ _ _ _ _ |
+|449999|10 |387.49  |435    |837  |398.13|ACM       |Tuesday  |Rain      |Residence    |916.46  |1198    |C10  |
+|_ _ _ _|_ _ _ _|_1_0_6_._1_2_ _ _|_ _ _ _ _ _ _ _|_ _ _ _ _ _|_ _ _ _ _ _ _|_ _ _ _ _ _ _ _ _ _ _|_ _ _ _ _ _ _ _ _ _|_ _ _ _ _ _ _ _ _ _ _|_ _ _ _ _ _ _ _ _ _ _ _ _ _|_7_8_5_._1_3_ _ _|_ _ _ _ _ _ _ _ _|_ _ _ _ _ |
+500 rows × 12 columns
+To specify the synthetic random dataset parameters:
+In [6]:
+N=10 # Number of trajectories
+M=50 # Number of points by trajectory
+L=10 # Number of attributes
+C=3  # Number of classes (C1 to Cn)
+randomGenerator(N, M, L, C)
+Out[6]:
+ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ 
+|_ _ _ _|_tt_ii_dd_|_aa_11____ss_pp_aa_cc_ee_|_aa_22____tt_ii_mm_ee_|_aa_33____nn_11_|_ _aa_44____nn_22_|_aa_55____nn_oo_mm_ii_nn_aa_ll_|_ _ _ _aa_66____dd_aa_yy_|_aa_77____ww_ee_aa_tt_hh_ee_rr_|_ _ _aa_88____cc_aa_tt_ee_gg_oo_rr_yy_|_aa_99____ss_pp_aa_cc_ee_|_aa_11_00____tt_ii_mm_ee_|_ll_aa_bb_ee_ll|
+|00  |1  |134.5   |114    |949  |976.98|PX        |Tuesday  |Clouds    |Outdoors &   |101.04  |1114    |C1   |
+|_ _ _ _|_ _ _ _|_8_4_8_._2_8_ _ _|_ _ _ _ _ _ _ _|_ _ _ _ _ _|_ _ _ _ _ _ _|_ _ _ _ _ _ _ _ _ _ _|_ _ _ _ _ _ _ _ _ _|_ _ _ _ _ _ _ _ _ _ _|_R_e_c_r_e_a_t_i_o_n_ _ _ _|_7_7_8_._5_2_ _ _|_ _ _ _ _ _ _ _ _|_ _ _ _ _ |
+|11  |1  |764.54  |985    |-656 |630.77|HK        |Saturday |Clouds    |Shop &       |328.42  |83      |C1   |
+|_ _ _ _|_ _ _ _|_2_5_5_._3_2_ _ _|_ _ _ _ _ _ _ _|_ _ _ _ _ _|_ _ _ _ _ _ _|_ _ _ _ _ _ _ _ _ _ _|_ _ _ _ _ _ _ _ _ _|_ _ _ _ _ _ _ _ _ _ _|_S_e_r_v_i_c_e_ _ _ _ _ _ _|_5_0_9_._7_8_ _ _|_ _ _ _ _ _ _ _ _|_ _ _ _ _ |
+|22  |1  |495.93  |746    |344  |695.05|JM        |Saturday |Rain      |Travel &     |665.91  |1073    |C1   |
+|_ _ _ _|_ _ _ _|_4_4_9_._9_4_ _ _|_ _ _ _ _ _ _ _|_ _ _ _ _ _|_ _ _ _ _ _ _|_ _ _ _ _ _ _ _ _ _ _|_ _ _ _ _ _ _ _ _ _|_ _ _ _ _ _ _ _ _ _ _|_T_r_a_n_s_p_o_r_t_ _ _ _ _|_1_7_9_._7_5_ _ _|_ _ _ _ _ _ _ _ _|_ _ _ _ _ |
+|33  |1  |652.24  |1167   |-442 |450.85|ZO        |Wednesday|Unknown   |Nightlife    |149.71  |185     |C1   |
+|_ _ _ _|_ _ _ _|_7_8_9_._5_1_ _ _|_ _ _ _ _ _ _ _|_ _ _ _ _ _|_ _ _ _ _ _ _|_ _ _ _ _ _ _ _ _ _ _|_ _ _ _ _ _ _ _ _ _|_ _ _ _ _ _ _ _ _ _ _|_S_p_o_t_ _ _ _ _ _ _ _ _ _|_1_4_1_._6_8_ _ _|_ _ _ _ _ _ _ _ _|_ _ _ _ _ |
+|   |   |93.95   |       |     |      |          |         |          |Professional |866.41  |        |     |
+|44  |1  |28.38   |1135   |327  |523.90|CU        |Monday   |Clouds    |& Other      |305.93  |522     |C1   |
+|_ _ _ _|_ _ _ _|_ _ _ _ _ _ _ _ _|_ _ _ _ _ _ _ _|_ _ _ _ _ _|_ _ _ _ _ _ _|_ _ _ _ _ _ _ _ _ _ _|_ _ _ _ _ _ _ _ _ _|_ _ _ _ _ _ _ _ _ _ _|_P_l_a_c_e_s_ _ _ _ _ _ _ _|_ _ _ _ _ _ _ _ _|_ _ _ _ _ _ _ _ _|_ _ _ _ _ |
+|_.._.._.._|_._._._|_._._._ _ _ _ _ _|_._._._ _ _ _ _|_._._._ _ _|_._._._ _ _ _|_._._._ _ _ _ _ _ _ _|_._._._ _ _ _ _ _ _|_._._._ _ _ _ _ _ _ _|_._._._ _ _ _ _ _ _ _ _ _ _|_._._._ _ _ _ _ _|_._._._ _ _ _ _ _|_._._._ _ |
+|449955|11 |647.96  |1205   |561  |819.12|ACR       |Saturday |Rain      |Arts &       |515.96  |634     |C3   |
+|_ _ _ _|_ _ _ _|_3_0_0_._5_ _ _ _|_ _ _ _ _ _ _ _|_ _ _ _ _ _|_ _ _ _ _ _ _|_ _ _ _ _ _ _ _ _ _ _|_ _ _ _ _ _ _ _ _ _|_ _ _ _ _ _ _ _ _ _ _|_E_n_t_e_r_t_a_i_n_m_e_n_t_|_9_5_5_._6_6_ _ _|_ _ _ _ _ _ _ _ _|_ _ _ _ _ |
+|449966|11 |779.26  |485    |121  |745.32|AIZ       |Tuesday  |Rain      |Outdoors &   |377.83  |435     |C3   |
+|_ _ _ _|_ _ _ _|_9_3_3_._6_1_ _ _|_ _ _ _ _ _ _ _|_ _ _ _ _ _|_ _ _ _ _ _ _|_ _ _ _ _ _ _ _ _ _ _|_ _ _ _ _ _ _ _ _ _|_ _ _ _ _ _ _ _ _ _ _|_R_e_c_r_e_a_t_i_o_n_ _ _ _|_2_6_3_._1_3_ _ _|_ _ _ _ _ _ _ _ _|_ _ _ _ _ |
+|449977|11 |398.3   |406    |-248 |180.89|YH        |Monday   |Fog       |Event        |458.27  |874     |C3   |
+|_ _ _ _|_ _ _ _|_5_4_5_._1_9_ _ _|_ _ _ _ _ _ _ _|_ _ _ _ _ _|_ _ _ _ _ _ _|_ _ _ _ _ _ _ _ _ _ _|_ _ _ _ _ _ _ _ _ _|_ _ _ _ _ _ _ _ _ _ _|_ _ _ _ _ _ _ _ _ _ _ _ _ _|_6_6_5_._4_6_ _ _|_ _ _ _ _ _ _ _ _|_ _ _ _ _ |
+|449988|11 |133.52  |62     |-485 |890.42|DI        |Thursday |Clouds    |Residence    |263.93  |1141    |C3   |
+|_ _ _ _|_ _ _ _|_6_0_5_._0_2_ _ _|_ _ _ _ _ _ _ _|_ _ _ _ _ _|_ _ _ _ _ _ _|_ _ _ _ _ _ _ _ _ _ _|_ _ _ _ _ _ _ _ _ _|_ _ _ _ _ _ _ _ _ _ _|_ _ _ _ _ _ _ _ _ _ _ _ _ _|_9_4_4_._8_ _ _ _|_ _ _ _ _ _ _ _ _|_ _ _ _ _ |
+|449999|11 |387.49  |435    |837  |398.13|ACM       |Tuesday  |Rain      |Residence    |916.46  |1198    |C3   |
+|_ _ _ _|_ _ _ _|_1_0_6_._1_2_ _ _|_ _ _ _ _ _ _ _|_ _ _ _ _ _|_ _ _ _ _ _ _|_ _ _ _ _ _ _ _ _ _ _|_ _ _ _ _ _ _ _ _ _|_ _ _ _ _ _ _ _ _ _ _|_ _ _ _ _ _ _ _ _ _ _ _ _ _|_7_8_5_._1_3_ _ _|_ _ _ _ _ _ _ _ _|_ _ _ _ _ |
+500 rows × 12 columns
+d) To generate a set of random datasets:
+
+Creates and save dataset files (including movelets json descriptor file).
+Generates randomic datasets in a increasing log scale for each parameter. It
+uses the middle value for the other configurations
+In [7]:
+data_path = 'matdata/assets/sample/random'
+
+Ns=[100, 3]   # Min. number of trajectories: 100, 3 scales (by log increment)
+Ms=[10,  3]   # Min. number of points: 10, 3 scales (by log increment)
+Ls=[8,   3]   # Min. number of attributes: 8, 3 scales (by log increment)
+Cs=[2,   3]   # Min. number of labels: 2, 3 scales (by log increment)
 
+scalerRandomGenerator(Ns, Ms, Ls, Cs, save_to=data_path)
+  0%|          | 0/12 [00:00<?, ?it/s]
+N :: fix. value: 	 200 	scale:	 [100, 200, 400]
+M :: fix. value: 	 20 	scale:	 [10, 20, 40]
+L :: fix. value: 	 8 	scale:	 [8, 16, 32]
+C :: fix. value: 	 4 	scale:	 [2, 4, 8]
+Writing - CSV |
+Writing - CSV |
+Writing - CSV |
+Writing - CSV |
+Writing - CSV |
+Writing - CSV |
+Writing - CSV |
+Writing - CSV |
+Writing - CSV |
+===============================================================================
 # By Tarlis Portela (2023)
```

### Comparing `mat-data-0.1b9/PKG-INFO` & `mat_data-0.1rc1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: mat-data
-Version: 0.1b9
+Version: 0.1rc1
 Summary: MAT-data: Data Preprocessing for Multiple Aspect Trajectory Data Mining
-Home-page: https://github.com/ttportela/mat-data
-Author: Tarlis Tortelli Portela
+Home-page: https://github.com/mat-analysis/mat-data
+Author: Tarlis Portela
 Author-email: Tarlis Tortelli Portela <tarlis@tarlis.com.br>
 Maintainer-email: Tarlis Tortelli Portela <tarlis@tarlis.com.br>
 License: GPL Version 3 or superior (see LICENSE file)
-Project-URL: Homepage, https://github.com/ttportela/mat-data
-Project-URL: Repository, https://github.com/ttportela/mat-data
-Project-URL: Documentation, https://github.com/ttportela/mat-data/blob/main/README.md
+Project-URL: Homepage, https://github.com/mat-analysis/mat-data
+Project-URL: Repository, https://github.com/mat-analysis/mat-data
+Project-URL: Documentation, https://github.com/mat-analysis/mat-data/blob/main/README.md
 Project-URL: Download, https://pypi.org/project/mat-data/#files
-Project-URL: Bug Tracker, https://github.com/ttportela/mat-data/issues
+Project-URL: Bug Tracker, https://github.com/mat-analysis/mat-data/issues
 Keywords: data-science,machine-learning,data-mining,trajectory,multiple-trajectory,trajectory-classification,preprocess
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python
 Classifier: Topic :: Software Development
 Classifier: Topic :: Scientific/Engineering
@@ -30,17 +30,19 @@
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: glob2
 Requires-Dist: numpy
 Requires-Dist: pandas
-Requires-Dist: mat-data
+Requires-Dist: mat-model
 Provides-Extra: all-extras
 Requires-Dist: geohash; extra == "all-extras"
+Requires-Dist: pyarrow; extra == "all-extras"
+Requires-Dist: fastparquet; extra == "all-extras"
 Provides-Extra: dev
 Requires-Dist: pre-commit; extra == "dev"
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: pytest-cov; extra == "dev"
 Requires-Dist: pytest-xdist; extra == "dev"
 Requires-Dist: wheel; extra == "dev"
 Provides-Extra: binder
@@ -59,15 +61,17 @@
 
 Created on Dec, 2023
 Copyright (C) 2023, License GPL Version 3 or superior (see LICENSE file)
 
 ### Main Modules
 
 - [proprocess](/proprocess.py): Methods for trajectory preprocessing;
-- [generator](/generator.py): Methods for trajectory datasets generation.
+- [generator](/generator.py): Methods for trajectory datasets generation;
+- [datasets](/datasets.py): Methods for loading trajectory datasets;
+- [converter](/converter.py): Methods for conferting dataset formats.
 
 
 ### Installation
 
 Install directly from PyPi repository, or, download from github. (python >= 3.7 required)
 
 ```bash
```

### Comparing `mat-data-0.1b9/README.md` & `mat_data-0.1rc1/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -8,15 +8,17 @@
 
 Created on Dec, 2023
 Copyright (C) 2023, License GPL Version 3 or superior (see LICENSE file)
 
 ### Main Modules
 
 - [proprocess](/proprocess.py): Methods for trajectory preprocessing;
-- [generator](/generator.py): Methods for trajectory datasets generation.
+- [generator](/generator.py): Methods for trajectory datasets generation;
+- [datasets](/datasets.py): Methods for loading trajectory datasets;
+- [converter](/converter.py): Methods for conferting dataset formats.
 
 
 ### Installation
 
 Install directly from PyPi repository, or, download from github. (python >= 3.7 required)
 
 ```bash
```

### Comparing `mat-data-0.1b9/Steps to Build.txt` & `mat_data-0.1rc1/Steps to Build.txt`

 * *Files identical despite different names*

### Comparing `mat-data-0.1b9/mat_data.egg-info/PKG-INFO` & `mat_data-0.1rc1/mat_data.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: mat-data
-Version: 0.1b9
+Version: 0.1rc1
 Summary: MAT-data: Data Preprocessing for Multiple Aspect Trajectory Data Mining
-Home-page: https://github.com/ttportela/mat-data
-Author: Tarlis Tortelli Portela
+Home-page: https://github.com/mat-analysis/mat-data
+Author: Tarlis Portela
 Author-email: Tarlis Tortelli Portela <tarlis@tarlis.com.br>
 Maintainer-email: Tarlis Tortelli Portela <tarlis@tarlis.com.br>
 License: GPL Version 3 or superior (see LICENSE file)
-Project-URL: Homepage, https://github.com/ttportela/mat-data
-Project-URL: Repository, https://github.com/ttportela/mat-data
-Project-URL: Documentation, https://github.com/ttportela/mat-data/blob/main/README.md
+Project-URL: Homepage, https://github.com/mat-analysis/mat-data
+Project-URL: Repository, https://github.com/mat-analysis/mat-data
+Project-URL: Documentation, https://github.com/mat-analysis/mat-data/blob/main/README.md
 Project-URL: Download, https://pypi.org/project/mat-data/#files
-Project-URL: Bug Tracker, https://github.com/ttportela/mat-data/issues
+Project-URL: Bug Tracker, https://github.com/mat-analysis/mat-data/issues
 Keywords: data-science,machine-learning,data-mining,trajectory,multiple-trajectory,trajectory-classification,preprocess
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python
 Classifier: Topic :: Software Development
 Classifier: Topic :: Scientific/Engineering
@@ -30,17 +30,19 @@
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: glob2
 Requires-Dist: numpy
 Requires-Dist: pandas
-Requires-Dist: mat-data
+Requires-Dist: mat-model
 Provides-Extra: all-extras
 Requires-Dist: geohash; extra == "all-extras"
+Requires-Dist: pyarrow; extra == "all-extras"
+Requires-Dist: fastparquet; extra == "all-extras"
 Provides-Extra: dev
 Requires-Dist: pre-commit; extra == "dev"
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: pytest-cov; extra == "dev"
 Requires-Dist: pytest-xdist; extra == "dev"
 Requires-Dist: wheel; extra == "dev"
 Provides-Extra: binder
@@ -59,15 +61,17 @@
 
 Created on Dec, 2023
 Copyright (C) 2023, License GPL Version 3 or superior (see LICENSE file)
 
 ### Main Modules
 
 - [proprocess](/proprocess.py): Methods for trajectory preprocessing;
-- [generator](/generator.py): Methods for trajectory datasets generation.
+- [generator](/generator.py): Methods for trajectory datasets generation;
+- [datasets](/datasets.py): Methods for loading trajectory datasets;
+- [converter](/converter.py): Methods for conferting dataset formats.
 
 
 ### Installation
 
 Install directly from PyPi repository, or, download from github. (python >= 3.7 required)
 
 ```bash
```

### Comparing `mat-data-0.1b9/matdata/LICENSE` & `mat_data-0.1rc1/matdata/LICENSE`

 * *Files identical despite different names*

### Comparing `mat-data-0.1b9/matdata/README.md` & `mat_data-0.1rc1/matdata/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -8,15 +8,17 @@
 
 Created on Dec, 2023
 Copyright (C) 2023, License GPL Version 3 or superior (see LICENSE file)
 
 ### Main Modules
 
 - [proprocess](/proprocess.py): Methods for trajectory preprocessing;
-- [generator](/generator.py): Methods for trajectory datasets generation.
+- [generator](/generator.py): Methods for trajectory datasets generation;
+- [datasets](/datasets.py): Methods for loading trajectory datasets;
+- [converter](/converter.py): Methods for conferting dataset formats.
 
 
 ### Installation
 
 Install directly from PyPi repository, or, download from github. (python >= 3.7 required)
 
 ```bash
```

### Comparing `mat-data-0.1b9/matdata/assets/sample/Foursquare_Sample.csv` & `mat_data-0.1rc1/matdata/assets/sample/Foursquare_Sample.csv`

 * *Files identical despite different names*

### Comparing `mat-data-0.1b9/matdata/generator.py` & `mat_data-0.1rc1/matdata/generator.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,85 +1,94 @@
 # -*- coding: utf-8 -*-
 """
-Multiple Aspect Trajectory Tools Framework, MAT-data: Data Preprocessing for Multiple Aspect Trajectory Data Mining
+**Multiple Aspect Trajectory Tools Framework**
+
+*MAT-data: Data Preprocessing for Multiple Aspect Trajectory Data Mining*
 
 The present application offers a tool, to support the user in the classification task of multiple aspect trajectories,
 specifically for extracting and visualizing the movelets, the parts of the trajectory that better discriminate a class.
 It integrates into a unique platform the fragmented approaches available for multiple aspects trajectories and in
 general for multidimensional sequence classification into a unique web-based and python library system. Offers both
 movelets visualization and classification methods.
 
 Created on Dec, 2023
 Copyright (C) 2023, License GPL Version 3 or superior (see LICENSE file)
 
 @author: Tarlis Portela
+
+----
+
 """
 import os
 import pandas as pd
 import numpy as np
 
 from tqdm.auto import tqdm
 
 import math
 import random
 import itertools
 
-
-from .preprocess import writeFile, featuresJSON
+from matdata.preprocess import writeFile, featuresJSON
 # --------------------------------------------------------------------------------
 def scalerSamplerGenerator(
     Ns=[100, 10],
     Ms=[10,  10],
     Ls=[8,   10],
     Cs=[2,  10],
     random_seed=1,
     fileprefix='scalability',
     fileposfix='train',
     cols_for_sampling = ['space','time','day','rating','price','weather','root_type','type'],
     save_to=None,
     base_data=None,
     save_desc_files=True,
-    outformats=['csv', 'mat']):
-    '''
-    [Function to generate trajectory datasets based on real data.]
+    outformats=['csv']):
+    """
+    Generates trajectory datasets based on real data.
+
+    Parameters:
+    -----------
+    Ns : list of int, optional
+        Parameters to scale the number of trajectories. 
+        List of 2 values: starting number, number of elements (default [100, 10])
+    Ms : list of int, optional
+        Parameters to scale the size of trajectories. 
+        List of 2 values: starting number, number of elements (default [10, 10])
+    Ls : list of int, optional
+        Parameters to scale the number of attributes (* doubles the columns). 
+        List of 2 values: starting number, number of elements (default [8, 10])
+    Cs : list of int, optional
+        Parameters to scale the number of classes. 
+        List of 2 values: starting number, number of elements (default [2, 10])
+    random_seed : int, optional
+        Random seed (default 1)
+    fileprefix : str, optional
+        Output filename prefix (default 'scalability')
+    fileposfix : str, optional
+        Output filename postfix (default 'train')
+    cols_for_sampling : list or dict, optional
+        Columns to add in the generated dataset. 
+        Default: ['space', 'time', 'day', 'rating', 'price', 'weather', 'root_type', 'type'].
+        If a dictionary is provided in the format: {'aspectName': 'type', 'aspectName': 'type'},
+        it is used when providing base_data and saving .MAT.
+    save_to : str or bool, optional
+        Destination folder to save, or False if not to save CSV files (default False)
+    base_data : DataFrame, optional
+        DataFrame of trajectories to use as a base for sampling data.
+        Default: None (uses example data)
+    save_desc_files : bool, optional
+        True if to save the .json description files, False otherwise (default True)
+    outformats : list, optional
+        Output file formats for saving (default ['csv'])
 
-    Args:
-        Ns [int, int]: 
-            Parameters to scale number of trajectories. 
-            List of 2 values: starting number, number of elements (default [100, 10])
-        Ms [int, int]: 
-            Parameters to scale size of Trajectories. 
-            List of 2 values: starting number, number of elements (default [10, 10])
-        Ls [int, int]: 
-            Parameters to scale number of attributes (* doubles the columns). 
-            List of 2 values: starting number, number of elements (default [8, 10])
-        Cs [int, int]: 
-            Parameters to scale number of classes. 
-            List of 2 values: starting number, number of elements (default [2, 10])
-        random_seed [int]: 
-            Random Seed (default 1)
-        cols_for_sampling [list] or [dict]: 
-            Columns to add in the generated dataset (default 'lat_lon,time,day,rating,price,weather,root_type,type')
-            OR if use dictionary in the format: {'aspectName': 'type', 'aspectName': 'type'} when broviding base_data and saving .MAT
-        save_to [str, bool]: 
-            Destination folder to save or False, if not to save csv file (default False)
-        fileprefix [str]: 
-            Output filename prefix (default 'sample')
-        fileposfix [str]: 
-            Output filename postfix (default 'train')
-        base_data [DataFrame]: 
-            DataFrame of trajectoris to use as base for sampling data (default 'assets/examples/Foursquare_Example.csv')
-        save_desc_files [bool]: 
-            True if to save the .json description files or False, if not to save (default True)
-        outformats [list]:
-            Output file formats for saving (default ['csv', 'mat'])
-    
     Returns:
-        [pandas.DataFrame] the generated dataset
-    '''
+    --------
+    None
+    """
     
     assert Ns[0] > 0, 'N > 0'
     assert Ms[0] > 0, 'M > 0'
     assert Cs[0] > 0, 'C > 0'
     assert Ls[0] > 0, 'L > 0'
     assert Ns[0] >= Cs[0], 'N >= C'
     assert save_to, 'save_to param must be set.'
@@ -98,18 +107,18 @@
     Cs = getScale(Cs[0], Cs[1])
     
     miN = getMiddleE(Ns)
     miM = getMiddleE(Ms)
     miL = len(cols_for_sampling) #getMiddleE(La)
     miC = getMiddleE(Cs)
     
-    print('N ::', 'fix. value:', 't', miN, 'tscale:t', Ns)
-    print('M ::', 'fix. value:', 't', miM, 'tscale:t', Ms)
-    print('L ::', 'fix. value:', 't', miL, 'tscale:t', La)
-    print('C ::', 'fix. value:', 't', miC, 'tscale:t', Cs)
+    print('N ::', 'fix. value:', '\t', miN, '\tscale:\t', Ns)
+    print('M ::', 'fix. value:', '\t', miM, '\tscale:\t', Ms)
+    print('L ::', 'fix. value:', '\t', miL, '\tscale:\t', La)
+    print('C ::', 'fix. value:', '\t', miC, '\tscale:\t', Cs)
     
     # 1 - Scale attributes (reshape columns), fixed trajectories, points, and classes:
     cols = cols_for_sampling.copy()
     prefix = fileprefix #+ '_L'
     for i in range(Ls[1]):        
         #if len(cols) == miL:
         #    cols_for_sampling = cols
@@ -160,42 +169,47 @@
     C=1,
     random_seed=1,
     fileprefix='sample',
     fileposfix='train',
     cols_for_sampling = ['space','time','day','rating','price','weather','root_type','type'],
     save_to=False,
     base_data=None,
-    outformats=['csv', 'mat']):
+    outformats=['csv']):
     '''
-    [Function to generate trajectories based on real data.]
+    Function to generate trajectories based on real data.
+
+    Parameters:
+    -----------
+    N : int, optional
+        Number of trajectories (default 10)
+    M : int, optional
+        Size of trajectories, number of points (default 50)
+    C : int, optional
+        Number of classes (default 1)
+    random_seed : int, optional
+        Random seed (default 1)
+    cols_for_sampling : list, optional
+        Columns to add in the generated dataset. 
+        Default: ['space', 'time', 'day', 'rating', 'price', 'weather', 'root_type', 'type'].
+    save_to : str or bool, optional
+        Destination folder to save, or False if not to save CSV files (default False)
+    fileprefix : str, optional
+        Output filename prefix (default 'sample')
+    fileposfix : str, optional
+        Output filename postfix (default 'train')
+    base_data : DataFrame, optional
+        DataFrame of trajectories to use as a base for sampling data.
+        Default: None (uses example data)
+    outformats : list, optional
+        Output file formats for saving (default ['csv'])
 
-    Args:
-        N [int]: 
-            Number of Trajectories (default 10)
-        M [int]: 
-            Size of Trajectories (default 50)
-        C [int]: 
-            Number of classes (default 1)
-        random_seed [int]: 
-            Random Seed (default 1)
-        cols_for_sampling [list]: 
-            Columns to add in the generated dataset (default 'lat_lon,time,day,rating,price,weather,root_type,type')
-        save_to [str, bool]: 
-            Destination folder to save or False, if not to save csv file (default False)
-        fileprefix [str]: 
-            Output filename prefix (default 'sample')
-        fileposfix [str]: 
-            Output filename postfix (default 'train')
-        base_data [DataFrame]: 
-            DataFrame of trajectoris to use as base for sampling data (default 'assets/examples/Foursquare_Example.csv')
-        outformats [list]:
-            Output file formats for saving (default ['csv', 'mat'])
-    
     Returns:
-        [pandas.DataFrame] the generated dataset
+    --------
+    pandas.DataFrame
+        The generated dataset.
     '''
     
     assert N > 0, 'N > 0'
     assert M > 0, 'M > 0'
     assert C > 0, 'C > 0'
     assert N >= C, 'N >= C'
     
@@ -271,48 +285,51 @@
     Cs=[2,  10],
     random_seed=1,
     fileprefix='scalability',
     fileposfix='train',
     attr_desc=None,
     save_to=None,
     save_desc_files=True,
-    outformats=['csv', 'mat']):
+    outformats=['csv']):
     '''
-    [Function to generate trajectory datasets based on random data.]
+    Function to generate trajectory datasets based on random data.
+
+    Parameters:
+    -----------
+    Ns : list of int, optional
+        Parameters to scale the number of trajectories. 
+        List of 2 values: starting number, number of elements (default [100, 10])
+    Ms : list of int, optional
+        Parameters to scale the size of trajectories. 
+        List of 2 values: starting number, number of elements (default [10, 10])
+    Ls : list of int, optional
+        Parameters to scale the number of attributes (* doubles the columns). 
+        List of 2 values: starting number, number of elements (default [8, 10])
+    Cs : list of int, optional
+        Parameters to scale the number of classes. 
+        List of 2 values: starting number, number of elements (default [2, 10])
+    random_seed : int, optional
+        Random seed (default 1)
+    attr_desc : list, optional
+        Data type intervals to generate attributes as a list of descriptive dicts.
+        Default: None (uses default types)
+    save_to : str or bool, optional
+        Destination folder to save, or False if not to save CSV files (default False)
+    fileprefix : str, optional
+        Output filename prefix (default 'sample')
+    fileposfix : str, optional
+        Output filename postfix (default 'train')
+    save_desc_files : bool, optional
+        True if to save the .json description files, False otherwise (default True)
+    outformats : list, optional
+        Output file formats for saving (default ['csv'])
 
-    Args:
-        Ns [int, int]: 
-            Parameters to scale number of trajectories. 
-            List of 2 values: starting number, number of elements (default [100, 10])
-        Ms [int, int]: 
-            Parameters to scale size of Trajectories. 
-            List of 2 values: starting number, number of elements (default [10, 10])
-        Ls [int, int]: 
-            Parameters to scale number of attributes (* doubles the columns). 
-            List of 2 values: starting number, number of elements (default [8, 10])
-        Cs [int, int]: 
-            Parameters to scale number of classes. 
-            List of 2 values: starting number, number of elements (default [2, 10])
-        random_seed [int]: 
-            Random Seed (default 1)
-        attr_desc [list]: 
-            Data type intervals to generate attributes as list of desciptive dicts (default 'default_types()')
-        save_to [str, bool]: 
-            Destination folder to save or False, if not to save csv file (default False)
-        fileprefix [str]: 
-            Output filename prefix (default 'sample')
-        fileposfix [str]: 
-            Output filename postfix (default 'train')
-        save_desc_files [bool]: 
-            True if to save the .json description files or False, if not to save (default True)
-        outformats [list]:
-            Output file formats for saving (default ['csv', 'mat'])
-    
     Returns:
-        [pandas.DataFrame] the generated dataset
+    --------
+    None
     '''
     
     assert Ns[0] > 0, 'N > 0'
     assert Ms[0] > 0, 'M > 0'
     assert Cs[0] > 0, 'C > 0'
     assert Ls[0] > 0, 'L > 0'
     assert Ns[0] >= Cs[0], 'N >= C'
@@ -330,18 +347,18 @@
     Cs = getScale(Cs[0], Cs[1])
     
     miN = getMiddleE(Ns)
     miM = getMiddleE(Ms)
     miL = Ls[0] #getMiddleE(La)
     miC = getMiddleE(Cs)
     
-    print('N ::', 'fix. value:', 't', miN, 'tscale:t', Ns)
-    print('M ::', 'fix. value:', 't', miM, 'tscale:t', Ms)
-    print('L ::', 'fix. value:', 't', miL, 'tscale:t', La)
-    print('C ::', 'fix. value:', 't', miC, 'tscale:t', Cs)
+    print('N ::', 'fix. value:', '\t', miN, '\tscale:\t', Ns)
+    print('M ::', 'fix. value:', '\t', miM, '\tscale:\t', Ms)
+    print('L ::', 'fix. value:', '\t', miL, '\tscale:\t', La)
+    print('C ::', 'fix. value:', '\t', miC, '\tscale:\t', Cs)
     
     if not attr_desc:
         attr_desc = default_types()[:Ls[0]]
     
     generators = instantiate_generators(attr_desc)
     
     # 1 - Scale attributes (reshape columns), fixed trajectories, points, and classes:
@@ -386,43 +403,47 @@
     L=10,
     C=10,
     random_seed=1,
     fileprefix='random',
     fileposfix='train',
     attr_desc=None,
     save_to=False,
-    outformats=['csv', 'mat']):
+    outformats=['csv']):
     '''
-    [Function to generate trajectories based on random data.]
+    Function to generate trajectories based on random data.
+
+    Parameters:
+    -----------
+    N : int, optional
+        Number of trajectories (default 10)
+    M : int, optional
+        Size of trajectories (default 50)
+    L : int, optional
+        Number of attributes (default 10)
+    C : int, optional
+        Number of classes (default 10)
+    random_seed : int, optional
+        Random Seed (default 1)
+    attr_desc : list of dict, optional
+        Data type intervals to generate attributes as a list of descriptive dicts.
+        Default: None (uses default types)
+        OR a list of instances of AttributeGenerator
+    save_to : str or bool, optional
+        Destination folder to save, or False if not to save CSV files (default False)
+    fileprefix : str, optional
+        Output filename prefix (default 'sample')
+    fileposfix : str, optional
+        Output filename postfix (default 'train')
+    outformats : list, optional
+        Output file formats for saving (default ['csv'])
 
-    Args:
-        N [int]: 
-            Number of Trajectories (default 10)
-        M [int]: 
-            Size of Trajectories (default 50)
-        L [int]: 
-            Number of attributes (default 10)
-        C [int]: 
-            Number of classes (default 10)
-        random_seed [int]: 
-            Random Seed (default 1)
-        attr_desc [list of dict]: 
-            Data type intervals to generate attributes as list of desciptive dicts (default 'default_types()')
-            OR a list of instances of AttributeGenerator
-        save_to [str, bool]: 
-            Destination folder to save or False, if not to save csv file (default False)
-        fileprefix [str]: 
-            Output filename prefix (default 'sample')
-        fileposfix [str]: 
-            Output filename postfix (default 'train')
-        outformats [list]:
-            Output file formats for saving (default ['csv', 'mat'])
-    
     Returns:
-        [pandas.DataFrame] the generated dataset
+    --------
+    pandas.DataFrame
+        The generated dataset.
     '''
     
     assert N > 0, 'N > 0'
     assert M > 0, 'M > 0'
     assert L > 0, 'L > 0'
     assert C > 0, 'C > 0'
     assert N >= C, 'N >= C'
@@ -471,15 +492,15 @@
         for outType in outformats:
             writeFile(save_to, new_df, filename, 'tid', 'label', list(new_df.columns), None, desc_cols, outType)
         #filename += '.csv'
         #new_df.to_csv( os.path.join(save_to, filename), index=False)
 
     return new_df
     
-    print('Not implemented.')
+#    print('Not implemented.')
 
 # --------------------------------------------------------------------------------
 def default_types():
     return [
         {'name': 'space',    'atype': 'space',    'method': 'grid_cell',    'interval': [(0.0,1000.0), (0.0,1000.0)]},
         {'name': 'time',     'atype': 'time',     'method': 'random',       'interval': [0, 1440]},
         {'name': 'n1',       'atype': 'numeric',  'method': 'random',       'interval': [-1000, 1000]},
```

### Comparing `mat-data-0.1b9/matdata/inc/ts_io.py` & `mat_data-0.1rc1/matdata/inc/ts_io.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,27 @@
 # -*- coding: utf-8 -*-
 """
-Multiple Aspect Trajectory Tools Framework, MAT-data: Data Preprocessing for Multiple Aspect Trajectory Data Mining
+**Multiple Aspect Trajectory Tools Framework**
 
-The present application offers a tool, to support the user in the classification task of multiple aspect trajectories, specifically for extracting and visualizing the movelets, the parts of the trajectory that better discriminate a class. It integrates into a unique platform the fragmented approaches available for multiple aspects trajectories and in general for multidimensional sequence classification into a unique web-based and python library system. Offers both movelets visualization and a complete configuration of classification experimental settings.
+*MAT-data: Data Preprocessing for Multiple Aspect Trajectory Data Mining*
+
+The present application offers a tool, to support the user in the classification task of multiple aspect trajectories,
+specifically for extracting and visualizing the movelets, the parts of the trajectory that better discriminate a class.
+It integrates into a unique platform the fragmented approaches available for multiple aspects trajectories and in
+general for multidimensional sequence classification into a unique web-based and python library system. Offers both
+movelets visualization and classification methods.
 
 Created on Dec, 2021
 Copyright (C) 2022, License GPL Version 3 or superior (see LICENSE file)
 
 @author: Tarlis Portela
 @author sktime package (adapted)
+
+----
+
 """
 import os
 import itertools
 import textwrap
 
 import numpy as np
 import pandas as pd
@@ -423,23 +432,32 @@
                                             )
 
                                         try:
                                             value = tuple_data[last_comma_index + 1 :]
                                             value = float(value)
 
                                         except ValueError:
-                                            raise TsFileParseException(
-                                                "dimension "
+                                            # By Tarlis:
+                                            print("dimension "
                                                 + str(this_line_num_dim + 1)
                                                 + " on line "
                                                 + str(line_num + 1)
                                                 + " contains a tuple that does "
                                                 "not have a valid numeric "
-                                                "value"
-                                            )
+                                                "value, read '"+str(value)+"' as missing.")
+                                            value = replace_missing_vals_with
+                                            #raise TsFileParseException(
+                                            #    "dimension "
+                                            #    + str(this_line_num_dim + 1)
+                                            #    + " on line "
+                                            #    + str(line_num + 1)
+                                            #    + " contains a tuple that does "
+                                            #    "not have a valid numeric "
+                                            #    "value"
+                                            #)
 
                                         # Check the type of timestamp that
                                         # we have
 
                                         timestamp = tuple_data[0:last_comma_index]
 
                                         try:
@@ -699,15 +717,30 @@
                         # Process the data for each dimension
 
                         for dim in range(0, num_dimensions):
                             dimension = dimensions[dim].strip()
 
                             if dimension:
                                 data_series = dimension.split(",")
-                                data_series = [float(i) for i in data_series]
+                                #data_series = [float(i) for i in data_series]
+                                
+                                def process(dim, value):
+                                    try:
+                                        value = float(value)
+                                    except ValueError:
+                                        # By Tarlis:
+                                        print("dimension "
+                                            + str(dim)
+                                            + " contains a tuple that does "
+                                            "not have a valid numeric "
+                                            "value, read '"+str(value)+"' as missing.")
+                                        value = replace_missing_vals_with
+                                    return value
+                                data_series = list(map(lambda i: process(dim, i), data_series))
+                                
                                 instance_list[dim].append(pd.Series(data_series))
 
                             else:
                                 instance_list[dim].append(pd.Series(dtype="object"))
 
                         if class_labels:
                             class_val_list.append(dimensions[num_dimensions].strip())
@@ -740,15 +773,17 @@
 
         x_data = pd.DataFrame(dtype=np.float32)
 
         for x in range(len(instance_list[0])):
             x_data_aux = pd.DataFrame(dtype=np.float32)
             for dim in range(len(instance_list)):
 #                 print(dim, x)
-                x_data_aux["dim" + str(dim)] = pd.Series(instance_list[dim][x])
+#                x_data_aux["dim" + str(dim)] = pd.Series(instance_list[dim][x])
+                x_data_aux = pd.concat([x_data_aux, pd.Series(instance_list[dim][x], name="dim" + str(dim))], axis=1)
+                
 
             x_data_aux["tid"] = x
             if class_labels:
                 x_data_aux["label"] = class_val_list[x]
             x_data = pd.concat([x_data, x_data_aux])
         
         x_data.reset_index(drop=True, inplace=True)
```

### Comparing `mat-data-0.1b9/matdata/preprocess.py` & `mat_data-0.1rc1/matdata/preprocess.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,76 +1,132 @@
 # -*- coding: utf-8 -*-
 """
-Multiple Aspect Trajectory Tools Framework, MAT-data: Data Preprocessing for Multiple Aspect Trajectory Data Mining
+**Multiple Aspect Trajectory Tools Framework**
+
+*MAT-data: Data Preprocessing for Multiple Aspect Trajectory Data Mining*
 
 The present application offers a tool, to support the user in the classification task of multiple aspect trajectories,
 specifically for extracting and visualizing the movelets, the parts of the trajectory that better discriminate a class.
 It integrates into a unique platform the fragmented approaches available for multiple aspects trajectories and in
 general for multidimensional sequence classification into a unique web-based and python library system. Offers both
 movelets visualization and classification methods.
 
 Created on Dec, 2023
 Copyright (C) 2023, License GPL Version 3 or superior (see LICENSE file)
 
 @author: Tarlis Portela
+
+----
+
 """
 import os
 import pandas as pd
 import numpy as np
 
+from pathlib import Path
 from tqdm.auto import tqdm
 import glob2 as glob
 import random
 
 from sklearn.model_selection import KFold, train_test_split
 
-from .inc.converter import *
+from matdata.converter import *
 #from .inc.script_def import getDescName
-#-------------------------------------------------------------------------->>
 
-def readDataset(data_path, folder=None, file='train.csv', class_col = 'label', missing='?'):
-#     from ..main import importer
+DS_FUNCTIONS = {
+    '.csv': csv2df,
+    '.parquet': parquet2df,
+    '.zip': zip2df,
+    '.mat': mat2df, #TODO
+    '.ts': ts2df,
+    '.xes': xes2df,
+}
+
+#-------------------------------------------------------------------------->>
+def readDataset(data_path, folder=None, file='train.csv', class_col='label', tid_col='tid', missing='?'):
+    """
+    Reads a dataset file (CSV format by default, 'train.csv') and returns it as a pandas DataFrame.
+
+    Parameters:
+    -----------
+    data_path : str
+        The directory path where the dataset file is located.
+    folder : str, optional
+        The subfolder within the data path where the dataset file is located.
+    file : str, optional (default='train.csv')
+        The name of the dataset file to be read.
+    class_col : str, optional (default='label')
+        The name of the column to be treated as the class/label column.
+    tid_col : str, optional (default='tid')
+        The name of the column to be used as the trajectory identifier.
+    missing : str, optional (default='?')
+        The placeholder for missing values in the dataset.
+
+    Returns:
+    --------
+    pandas.DataFrame
+        A DataFrame containing the dataset from the specified file, with trajectory identifier,
+        class label, and missing values handled as specified.
+    """
     
     if folder:
-        data_path = os.path.join(data_path, folder)
-    
-    if '.csv' in data_path or '.zip' in data_path or '.ts' in data_path:
-        url = data_path
-    elif '.csv' in file or '.zip' in file or '.ts' in file:
-        url = os.path.join(data_path, file)
+        url = os.path.join(data_path, folder)
     else:
-        url = os.path.join(data_path, file+'.csv')
+        url = data_path
+        
+    ext = Path(url).suffix
+    if '' == ext:
+        url = os.path.join(url, file)
+        
+    ext = Path(url).suffix
+    if '' == ext:
+        url = url + '.csv'
     
     url = os.path.abspath(url)
-    if '.csv' in url and os.path.exists(url):
-        df = pd.read_csv(url, na_values=missing)
-    elif ('.zip' in url and os.path.exists(url)) or ('.csv' in url and os.path.exists(url.replace('.csv', '.zip'))):
-        file = file.replace('.csv', '.zip')
-        df = zip2df(data_path, file, class_col=class_col)
-    elif '.ts' in url or os.path.exists(url.replace('train', 'TRAIN').replace('test', 'TEST').replace('.csv', '.ts')):
-        importer(['ts_io'], globals())
-        url = url.replace('train', 'TRAIN').replace('test', 'TEST').replace('.csv', '.ts')
-        df = load_from_tsfile_to_dataframe(url, replace_missing_vals_with=missing)
-#    elif '.mat' in url or os.path.exists(url.replace('.csv', '.mat')): #TODO
-#        url = url.replace('.csv', '.mat')
-#        df = mat2df(url, replace_missing_vals_with=missing)
-    else:
-        df = pd.read_csv(url, na_values=missing) # should not be used
+    ext = Path(url).suffix
+    
+    df = DS_FUNCTIONS[ext](url, class_col=class_col, tid_col=tid_col, missing=missing)
+    
     return df
 
-def organizeFrame(df, columns_order=None, tid_col='tid', class_col='label'):
-    if (set(df.columns) & set(['lat', 'lon'])) and not 'space' in df.columns:
-        df[["lat", "lon"]] = df[["lat", "lon"]].astype(str) 
-        df['space'] = df["lat"] + ' ' + df["lon"]
-        df[["lat", "lon"]] = df[["lat", "lon"]].astype(float)
+def organizeFrame(df, columns_order=None, tid_col='tid', class_col='label', make_spatials=False):
+    """
+    Organizes a DataFrame by reordering columns and optionally converting spatial columns.
+
+    Parameters:
+    -----------
+    df : pandas.DataFrame
+        The DataFrame to be organized.
+    columns_order : list of str, optional
+        A list of column names specifying the desired order of columns. If None, no reordering is performed.
+    tid_col : str, optional (default='tid')
+        The name of the column to be used as the trajectory identifier.
+    class_col : str, optional (default='label')
+        The name of the column to be treated as the class/label column.
+    make_spatials : bool, optional (default=False)
+        A flag indicating whether to convert spatial columns to both lat/lon separated or space format, which is the lat/lon concatenated in one column.
+
+    Returns:
+    --------
+    pandas.DataFrame
+        A DataFrame containing the organized data, with columns added as specified
+        and spatial columns converted if requested.
+    columns_order_zip
+        A list of the columns with space column, if present.
+    columns_order_csv
+        A list of the columns with lat/lon columns, if present.
+    """
+    
+    if make_spatials and (set(df.columns) & set(['lat', 'lon'])) and not 'space' in df.columns:
+        df.loc[:, 'space'] = df["lat"].astype(str)  + ' ' + df["lon"].astype(str) 
 
         if columns_order is not None:
             columns_order.insert(columns_order.index('lon')-1, 'space')
             
-    elif ('space' in df.columns or 'lat_lon' in df.columns) and not (set(df.columns) & set(['lat', 'lon'])):
+    elif make_spatials and ('space' in df.columns or 'lat_lon' in df.columns) and not (set(df.columns) & set(['lat', 'lon'])):
         if 'lat_lon' in df.columns:
             df.rename(columns={'lat_lon': 'space'}, inplace=True)
             if columns_order is not None:
                 columns_order[columns_order.index('lat_lon')] = 'space'
         
         ll = df['space'].str.split(" ", n = 1, expand = True) 
         df["lat"]= ll[0].astype(float)
@@ -80,60 +136,418 @@
             columns_order.insert(columns_order.index('space'), 'lat')
             columns_order.insert(columns_order.index('space')+1, 'lon')
     
     # For Columns ordering:
     if columns_order is None:
         columns_order = df.columns
             
-    columns_order = [x for x in columns_order if x not in [tid_col, class_col]]
-    columns_order = columns_order + [tid_col, class_col]
+    if class_col and class_col in df.columns:
+        columns_order = [x for x in columns_order if x not in [tid_col, class_col]]
+        columns_order = columns_order + [tid_col, class_col]
+    else:
+        columns_order = [x for x in columns_order if x not in [tid_col]]
+        columns_order = columns_order + [tid_col]
             
     columns_order_zip = [x for x in columns_order if x not in ['lat', 'lon']]
     columns_order_csv = [x for x in columns_order if x not in ['space']]
     
     return df, columns_order_zip, columns_order_csv
 
 #-------------------------------------------------------------------------->>
+def trainTestSplit(df, train_size=0.7, random_num=1, tid_col='tid', class_col='label', fileprefix='', \
+                      data_path='.', outformats=[], verbose=False, organize_columns=True):
+    """
+    Splits a DataFrame into training and testing sets, optionally organizes columns, and saves them to files.
+
+    Parameters:
+    -----------
+    df : pandas.DataFrame
+        The DataFrame to be split into training and testing sets.
+    train_size : float, optional (default=0.7)
+        The proportion of the dataset to include in the training set.
+    random_num : int, optional (default=1)
+        The random seed for reproducible results.
+    tid_col : str, optional (default='tid')
+        The name of the column to be used as the trajectory identifier.
+    class_col : str, optional (default='label')
+        The name of the column to be treated as the class/label column.
+    fileprefix : str, optional (default='')
+        The prefix to be added to the file names when saving.
+    data_path : str, optional (default='.')
+        The directory path where the output files will be saved.
+    outformats : list of str, optional
+        A list of output formats for saving the datasets (e.g., ['csv', 'parquet']).
+    verbose : bool, optional (default=False)
+        A flag indicating whether to display progress messages.
+    organize_columns : bool, optional (default=True)
+        A flag indicating whether to organize columns before saving.
+
+    Returns:
+    --------
+    train : pandas.DataFrame
+        A DataFrame containing the training set.
+    test : pandas.DataFrame
+        A DataFrame containing the testing set.
+    """
+    
+    #outformats=['zip', 'csv', 'mat']
+    if verbose:
+        print(str(train_size)+"% train and test split ... ")
+    
+    if organize_columns:
+        df, columns_order_zip, columns_order_csv = organizeFrame(df, None, tid_col, class_col)
+    else:
+        columns_order_zip = list(df.columns)
+        columns_order_csv = list(df.columns)
+    
+    train_index, test_index, _ = splitTIDs(df, train_size, random_num, tid_col, class_col, min_elements=1)
+    
+    train = df.loc[df[tid_col].isin(train_index)]
+    test  = df.loc[df[tid_col].isin(test_index)]
+    
+    # WRITE Train / Test Files
+    for outType in outformats:
+        writeFiles(data_path, fileprefix, train, test, tid_col, class_col, \
+                 columns_order_zip if outType in ['zip', 'mat'] else columns_order_csv, outformat=outType)
+
+    if verbose:
+        print("Done.")
+        print(" --------------------------------------------------------------------------------")
+    return train, test
+
+def kfold_trainTestSplit(df, k, random_num=1, tid_col='tid', class_col='label', fileprefix='', columns_order=None, ktrain=None, ktest=None, mat_columns=None, data_path='.', outformats=[], verbose=False):
+    """
+    Splits a DataFrame into k folds for k-fold cross-validation, optionally organizes columns, and saves them to files.
+
+    Parameters:
+    -----------
+    df : pandas.DataFrame
+        The DataFrame to be split into k folds.
+    k : int
+        The number of folds for cross-validation.
+    random_num : int, optional (default=1)
+        The random seed for reproducible results.
+    tid_col : str, optional (default='tid')
+        The name of the column to be used as the trajectory identifier.
+    class_col : str, optional (default='label')
+        The name of the column to be treated as the class/label column.
+    fileprefix : str, optional (default='')
+        The prefix to be added to the file names when saving, for example: 'specific_' or 'generic_'.
+    columns_order : list of str, optional
+        A list of column names specifying the desired order of columns. If None, no reordering is performed.
+    ktrain : list of pandas.DataFrame, optional
+        A list of training sets for each fold. If None, the function will split the data into training and testing sets.
+    ktest : list of pandas.DataFrame, optional
+        A list of testing sets for each fold. If None, the function will split the data into training and testing sets.
+    mat_columns : list of str, optional
+        A list of column names to be included in the .mat files, corresponding to `columns_order`.
+    data_path : str, optional (default='.')
+        The directory path where the output files will be saved.
+    outformats : list of str, optional
+        A list of output formats for saving the datasets (e.g., ['csv', 'zip', 'parquet']).
+    verbose : bool, optional (default=False)
+        A flag indicating whether to display progress messages.
+
+    Returns:
+    --------
+    ktrain : list of pandas.DataFrame
+        List of DataFrame containing the training sets.
+    ktest : list of pandas.DataFrame
+        List of DataFrame containing the testing sets.
+    """
+
+  
+    if verbose:
+        print(str(k)+"-fold train and test split ... ")
+    
+    df, columns_order_zip, columns_order_csv = organizeFrame(df, columns_order, tid_col, class_col)
+    
+    if not ktrain:
+        ktrain, ktest = splitData(df, k, random_num, tid_col, class_col)
+    elif verbose:
+        print("Train and test data provided.")
+    
+    if len(outformats) > 0:
+        for x in range(k):            
+            train_aux = ktrain[x]
+            test_aux  = ktest[x]
+
+            for outType in outformats:
+                if verbose:
+                    print("Writing", outType, "files ... " + str(x+1) +'/'+str(k))
+                path = 'run'+str(x+1)
+                if not os.path.exists(os.path.join(data_path, path)):
+                    os.makedirs(os.path.join(data_path, path))
+
+                writeFiles(data_path, os.path.join(path, fileprefix), train_aux, test_aux, tid_col, class_col, \
+                         columns_order_zip if outType in ['zip', 'mat'] else columns_order_csv, mat_columns, None, \
+                         outType, opSuff=str(x+1))
+    if verbose:
+        print("Done.")
+        print(" --------------------------------------------------------------------------------")
+    
+    return ktrain, ktest
+
+def stratify(df, sample_size=0.5, train_size=0.7, random_num=1, tid_col='tid', class_col='label', 
+             organize_columns=True, mat_columns=None, fileprefix='', outformats=[], data_path='.'):  
+    """
+    Stratifies a DataFrame by class label and splits it into training and testing sets, optionally organizes columns, and saves them to files.
+
+    Parameters:
+    -----------
+    df : pandas.DataFrame
+        The DataFrame to be stratified and split into training and testing sets.
+    sample_size : float, optional (default=0.5)
+        The proportion of the dataset to sample for stratification.
+    train_size : float, optional (default=0.7)
+        The proportion of the stratified dataset to include in the training set.
+    random_num : int, optional (default=1)
+        The random seed for reproducible results.
+    tid_col : str, optional (default='tid')
+        The name of the column to be used as the trajectory identifier.
+    class_col : str, optional (default='label')
+        The name of the column to be treated as the class/label column.
+    organize_columns : bool, optional (default=True)
+        A flag indicating whether to organize columns before saving.
+    mat_columns : list of str, optional (unused for now)
+        A list of column names to be included in the .mat files, if set to save.
+    fileprefix : str, optional (default='')
+        The prefix to be added to the file names when saving.
+    outformats : list of str, optional
+        A list of output formats for saving the datasets (e.g., ['csv', 'zip', 'parquet']).
+    data_path : str, optional (default='.')
+        The directory path where the output files will be saved.
+
+    Returns:
+    --------
+    train : pandas.DataFrame
+        A DataFrame containing the training set.
+    test : pandas.DataFrame
+        A DataFrame containing the testing set.
+    """
+    
+    train_index, _, _ = splitTIDs(df, sample_size, random_num, tid_col, class_col, min_elements=2)
+    
+    df = df.loc[df[tid_col].isin(train_index)].copy()
+    
+    train_index, test_index, _ = splitTIDs(df, train_size, random_num, tid_col, class_col, min_elements=1)
+    
+    if organize_columns:
+        df, columns_order_zip, columns_order_csv = organizeFrame(df, None, tid_col, class_col)
+    else:
+        columns_order_zip = list(df.columns)
+        columns_order_csv = list(df.columns)
+    
+    train = df.loc[df[tid_col].isin(train_index)]
+    test  = df.loc[df[tid_col].isin(test_index)]
+    
+    for outType in outformats:
+        path = 'S'+str(int(sample_size*100))
+        if not os.path.exists(os.path.join(data_path, path)):
+                os.makedirs(os.path.join(data_path, path))
+            
+        writeFiles(data_path, os.path.join(path, fileprefix), train, test, tid_col, class_col, \
+                 columns_order_zip if outType in ['zip', 'mat'] else columns_order_csv, mat_columns, None, outType, opSuff=path)
+    
+    return train, test
+    
+# TODO fix stratify:
+def kfold_stratify(df, k=10, inc=1, limit=10, random_num=1, tid_col='tid', class_col='label', fileprefix='', 
+             ktrain=None, ktest=None, organize_columns=True, mat_columns=None, data_path='.', outformats=[], ignore_ltk=True):
+   
+    print(str(k)+"-fold stratification of train and test ... ")
+    
+    if organize_columns:
+        df, columns_order_zip, columns_order_csv = organizeFrame(df, None, tid_col, class_col)
+    else:
+        columns_order_zip = list(df.columns)
+        columns_order_csv = list(df.columns)
+        
+    if not ktrain:
+        ktrain, ktest = splitData(df, k, random_num, tid_col, class_col, ignore_ltk=ignore_ltk)
+    else:
+        print("Train and test data provided.")
+    
+    for x in range(0, limit, inc):
+        
+        train_aux = ktrain[0]
+        test_aux  = ktest[0]
+        for y in range(1, x+1):
+            train_aux = pd.concat([train_aux,  ktrain[y]])
+            test_aux  = pd.concat([test_aux,   ktest[y]])
+            
+        for outType in outformats:
+            path = 'S'+str((x+1)*int(100/k))
+
+            if not os.path.exists(os.path.join(data_path, path)):
+                os.makedirs(os.path.join(data_path, path))
+            
+            writeFiles(data_path, os.path.join(path, fileprefix), train_aux, test_aux, tid_col, class_col, \
+                     columns_order_zip if outType in ['zip', 'mat'] else columns_order_csv, mat_columns, None, outType, opSuff=str(x+1))
+    print(" Done.")
+    print(" --------------------------------------------------------------------------------")
+    
+    return ktrain, ktest
+
+def klabels_stratify(df, kl=10, train_size=0.7, random_num=1, tid_col='tid', class_col='label', 
+             organize_columns=True, mat_columns=None, fileprefix='', outformats=[], data_path='.'):
+    """
+    Stratifies a DataFrame by a specified number of class labels and splits it into training and testing sets,
+    optionally organizes columns, and saves them to files.
+
+    Parameters:
+    -----------
+    df : pandas.DataFrame
+        The DataFrame to be stratified and split into training and testing sets.
+    kl : int, optional (default=10)
+        The number of class labels to stratify the DataFrame.
+    train_size : float, optional (default=0.7)
+        The proportion of the stratified dataset to include in the training set.
+    random_num : int, optional (default=1)
+        The random seed for reproducible results.
+    tid_col : str, optional (default='tid')
+        The name of the column to be used as the trajectory identifier.
+    class_col : str, optional (default='label')
+        The name of the column to be treated as the class/label column.
+    organize_columns : bool, optional (default=True)
+        A flag indicating whether to organize columns before saving.
+    mat_columns : list of str, optional (unused for now)
+        A list of column names to be included in the .mat files, if set to save.
+    fileprefix : str, optional (default='')
+        The prefix to be added to the file names when saving.
+    outformats : list of str, optional
+        A list of output formats for saving the datasets (e.g., ['csv', 'zip', 'parquet']).
+    data_path : str, optional (default='.')
+        The directory path where the output files will be saved.
+
+    Returns:
+    --------
+    train : pandas.DataFrame
+        A DataFrame containing the training set.
+    test : pandas.DataFrame
+        A DataFrame containing the testing set.
+    """
+
+    min_elements=1
+    
+    random.seed(random_num)
+    labels = df[class_col].unique()
+
+    n = min_elements if kl < min_elements else kl
+
+    labels_index = random.sample(list(labels), n)
+    df = df.loc[df[class_col].isin(labels_index)].copy()
+    
+    train_index, test_index, _ = splitTIDs(df, train_size, random_num, tid_col, class_col, min_elements=min_elements)
+    
+    if organize_columns:
+        df, columns_order_zip, columns_order_csv = organizeFrame(df, None, tid_col, class_col)
+    else:
+        columns_order_zip = list(df.columns)
+        columns_order_csv = list(df.columns)
+    
+    train = df.loc[df[tid_col].isin(train_index)]
+    test  = df.loc[df[tid_col].isin(test_index)]
+    
+    for outType in outformats:
+        path = 'L'+str(n)
+        if not os.path.exists(os.path.join(data_path, path)):
+                os.makedirs(os.path.join(data_path, path))
+                
+        writeFiles(data_path, os.path.join(path, fileprefix), train, test, tid_col, class_col, \
+                 columns_order_zip if outType in ['zip', 'mat'] else columns_order_csv, mat_columns, None, outType, opSuff=path)
+    
+    return train, test
+
+def joinTrainTest(dir_path, train_file="train.csv", test_file="test.csv", tid_col='tid', class_col = 'label', to_file=False): 
+    """
+    Joins training and testing datasets from separate files into a single DataFrame.
+
+    Parameters:
+    -----------
+    dir_path : str
+        The directory path where the training and testing files are located.
+    train_file : str, optional (default="train.csv")
+        The name of the training file to be read.
+    test_file : str, optional (default="test.csv")
+        The name of the testing file to be read.
+    tid_col : str, optional (default='tid')
+        The name of the column to be used as the trajectory identifier.
+    class_col : str, optional (default='label')
+        The name of the column to be treated as the class/label column.
+    to_file : bool, optional (default=False)
+        A flag indicating whether to save the joined DataFrame to a file, and saves the joined DataFrame to a file named 'joined.csv'.
+
+    Returns:
+    --------
+    pandas.DataFrame
+        A DataFrame containing the joined training and testing data.
+        If `to_file` is True, returns the DataFrame and saves the joined DataFrame to a file named 'joined.csv'.
+    """
+    
+    print("Joining train and test data from... " + dir_path)
+    
+    # Read datasets
+    dataset_train = readDataset(dir_path, None, train_file)
+    dataset_test  = readDataset(dir_path, None, test_file)
+    
+    dataset = pd.concat([dataset_train, dataset_test])
+    dataset.sort_values([class_col, tid_col])
+    
+    if to_file:
+        print("Saving joined dataset as: " + os.path.join(dir_path, 'joined.csv'))
+        dataset.to_csv(os.path.join(dir_path, 'joined.csv'), index=False)
+        
+    print("Done.")
+    print(" --------------------------------------------------------------------------------")
+    
+    return dataset
+
+#-------------------------------------------------------------------------->> DESCRIPTORS
 def readDsDesc(data_path, folder=None, file='train.csv', tid_col='tid', class_col='label', missing='?'):
+    # TODO Deprecated
+    
     df = readDataset(data_path, folder, file, class_col, missing)
     
     columns_order = [x for x in df.columns if x not in [tid_col, class_col]]
     df = df[columns_order + [tid_col, class_col]]
     
     if folder == None:
         folder = os.path.basename(data_path)
         data_path = os.path.dirname(data_path)
     
-#    desc = glob.glob(os.path.join(data_path, 'descriptors', \
-#                                  getDescName(os.path.basename(data_path), folder)+'_specific_hp.json'))
-#    if len(desc) > 0:
-#        attrs = readAttributes(desc[0])
-#        df.set_axis(attrs + [tid_col, class_col], axis=1, inplace=True)
-    
     return df
 
-#def readAttributes(desc_file):
-#    importer(['json'], globals())
-#    f = open(desc_file)
-#    desc = json.load(f)
-#    f.close()
-#    
-#    attrs = []
-#    for at in desc['attributes']:
-#        if at['type'].startswith('composite'):
-#            for i in ['x', 'y', 'z'] if at['type'].startswith('composite3_') else ['x', 'y']:
-#                attrs.append(at['text'].split('_')[0] + '_' + i)
-#        else:
-#            attrs.append(at['text'])
-##         attrs.append(at['text'])
-#        
-#    return attrs
-
-# --------------------------------------------------------------------------------
 def featuresJSON(df, version=1, deftype='nominal', defcomparator='equals', tid_col='tid', label_col='label', file=False):
+    """
+    Generates a JSON representation of features from a DataFrame.
+
+    Parameters:
+    -----------
+    df : pandas.DataFrame
+        The DataFrame containing the dataset.
+    version : int, optional (default=1)
+        The version number of the JSON schema (1 for MASTERMovelets format, 2 for HiPerMovelets format).
+    deftype : str, optional (default='nominal')
+        The default type of features.
+    defcomparator : str, optional (default='equals')
+        The default comparator for features.
+    tid_col : str, optional (default='tid')
+        The name of the column to be used as the trajectory identifier.
+    label_col : str, optional (default='label')
+        The name of the column to be treated as the class/label column.
+    file : bool, optional (default=False)
+        A flag indicating whether to save the JSON representation to a file.
+
+    Returns:
+    --------
+    str
+        If `file` is False, returns a str representing the features in JSON format.
+        If `file` is str, returns a str of JSON features and saves the JSON representation to a `file` param name.
+    """
     
     if isinstance(df, list):
         cols = {x: deftype for x in df}
     elif isinstance(df, dict):
         cols = df
     else:
         cols = descTypes(df)
@@ -192,16 +606,41 @@
     if file:
         file = open(file, 'w')
         print(s, file=file)
         file.close()
     else:
         print(s)
     
-#-------------------------------------------------------------------------->>
+#-------------------------------------------------------------------------->> STATISTICS
 def countClasses(data_path, folder, file='train.csv', tid_col = 'tid', class_col = 'label', markd=False):
+    """
+    Counts the occurrences of each class label in a dataset.
+
+    Parameters:
+    -----------
+    data_path : str
+        The directory path where the dataset file is located.
+    folder : str
+        The subfolder within the data path where the dataset file is located.
+    file : str, optional (default='train.csv')
+        The name of the dataset file to be read.
+    tid_col : str, optional (default='tid')
+        The name of the column to be used as the trajectory identifier.
+    class_col : str, optional (default='label')
+        The name of the column to be treated as the class/label column.
+    markd : bool, optional (default=False)
+        A flag indicating whether to print the class counts in Markdown format.
+
+    Returns:
+    --------
+    pandas.DataFrame or str
+        If `markd` is False, prins the markdown text and returns a dictionary DataFrame containing the counts of each class label in the dataset.
+        If `markd` is True, returns str markdown of the counts of each class label in the dataset.
+    """
+    
     df = readDataset(data_path, folder, file, class_col, tid_col, markd)
     return countClasses_df(df, tid_col, class_col, markd)
 
 def countClasses_df(df, tid_col = 'tid', class_col = 'label', markd=False):
     group = df.groupby([class_col, tid_col])
     df2 = group.apply(lambda x: ', '.join([str(s) for s in list(x[class_col].unique())]))
     md = "Number of Samples: " + str(len(df[tid_col].unique()))
@@ -215,14 +654,28 @@
         return md
     else:
         print(md)
         print(df2.value_counts())
         return df2.value_counts()
 
 def dfVariance(df):
+    """
+    Computes the variance for each column in a DataFrame.
+
+    Parameters:
+    -----------
+    df : pandas.DataFrame
+        The DataFrame for which variance is to be computed.
+
+    Returns:
+    --------
+    pandas.Series
+        A Series containing the variance for each column in the DataFrame.
+    """
+    
     stats=pd.DataFrame()
     dfx = df.apply(pd.to_numeric, args=['coerce'])
     #stats["Mean"]=dfx.mean(axis=0, skipna=True)
     #stats["Std.Dev"]=dfx.std(axis=0, skipna=True)
     stats["Variance"]=dfx.var(axis=0, skipna=True)
 
     dfx = df.fillna('?')
@@ -233,14 +686,29 @@
             #stats["Mean"][col] = categories[int( np.median(dfx[col].cat.codes) )]
             #stats["Std.Dev"][col] = np.std(dfx[col].cat.codes)
             stats["Variance"][col] = np.var(dfx[col].cat.codes)
     
     return stats.sort_values('Variance', ascending=False)
 
 def dfStats(df):
+    """
+    Computes summary statistics for each column in a DataFrame.
+
+    Parameters:
+    -----------
+    df : pandas.DataFrame
+        The DataFrame for which statistics are to be computed.
+
+    Returns:
+    --------
+    pandas.DataFrame
+        A DataFrame containing summary statistics for each column, including mean, standard deviation,
+        and variance. Columns are sorted by variance in descending order.
+    """
+    
     stats=pd.DataFrame()
     dfx = df.apply(pd.to_numeric, args=['coerce'])
     stats["Mean"]=dfx.mean(axis=0, skipna=True)
     stats["Std.Dev"]=dfx.std(axis=0, skipna=True)
     stats["Variance"]=dfx.var(axis=0, skipna=True)
 
     dfx = df.fillna('?')
@@ -251,16 +719,38 @@
             stats["Mean"][col] = categories[int( np.median(dfx[col].cat.codes) )]
             stats["Std.Dev"][col] = np.std(dfx[col].cat.codes)
             stats["Variance"][col] = np.var(dfx[col].cat.codes)
     
     return stats.sort_values('Variance', ascending=False)
     
 def datasetStatistics(data_path, folder, file_prefix='', tid_col = 'tid', class_col = 'label', to_file=False):
-#     from ..main import importer
-#     importer(['S'], locals())
+    """
+    Computes statistics for a dataset, including summary statistics for each column and class distribution into a markdown file format.
+
+    Parameters:
+    -----------
+    data_path : str
+        The directory path where the dataset file(s) are located.
+    folder : str
+        The subfolder within the data path where the dataset file(s) are located.
+    file_prefix : str, optional (default='')
+        The prefix to be added to the dataset file names.
+    tid_col : str, optional (default='tid')
+        The name of the column to be used as the trajectory identifier.
+    class_col : str, optional (default='label')
+        The name of the column to be treated as the class/label column.
+    to_file : bool, optional (default=False)
+        A flag indicating whether to save the statistics to a file.
+
+    Returns:
+    --------
+    dict or None
+        If `to_file` is False, prints markdown and returns a str containing the computed statistics.
+        If `to_file` is str, returns markdown str and saves the statistics to a file named as in `to_file` value.
+    """
 
     def addLine(i):
         return '\n\r' + ('&nbsp;'.join(['\n\r' for x in range(i)])) + '\n\r'
     
     train = readDsDesc(data_path, folder, file_prefix+'train.csv', tid_col, class_col, missing='NaN')
     test = readDsDesc(data_path, folder, file_prefix+'test.csv', tid_col, class_col, missing='NaN')
     
@@ -354,17 +844,16 @@
         f.write(f''+md)
         f.close()
     else:
         print('\n--------------------------------------------------------------------')
         print(md)
     return md
 
-#-------------------------------------------------------------------------->>
+#-------------------------------------------------------------------------->> HELPERS
 def splitTIDs(df, train_size=0.7, random_num=1, tid_col='tid', class_col='label', min_elements=1):
-#    importer(['S', 'random'], globals())
     train = list()
     test = list()
     
     df_ = df.groupby(tid_col).first().reset_index()[[tid_col, class_col]]
     
     def splitByLabel(label):
         nonlocal df_, train, test
@@ -380,57 +869,27 @@
         train = train + list(train_index)
         test  = test  + list(test_index)
         
     list(map(lambda label: splitByLabel(label), tqdm(df_[class_col].unique())))
     
     return train, test, df_
 
-def trainAndTestSplit(df, train_size=0.7, random_num=1, tid_col='tid', class_col='label', fileprefix='', \
-                      data_path='.', outformats=['zip', 'csv', 'mat'], verbose=False, organize_columns=True):
-#     from ..main import importer
-#    importer(['S', 'random'], globals())
-    if verbose:
-        print(str(train_size)+"% train and test split in... " + data_path)
-    
-    if organize_columns:
-        df, columns_order_zip, columns_order_csv = organizeFrame(df, None, tid_col, class_col)
-    else:
-        columns_order_zip = list(df.columns)
-        columns_order_csv = list(df.columns)
-    
-    train_index, test_index, _ = splitTIDs(df, train_size, random_num, tid_col, class_col, min_elements=1)
-    
-    train = df.loc[df[tid_col].isin(train_index)]
-    test  = df.loc[df[tid_col].isin(test_index)]
-    
-    # WRITE Train / Test Files
-    for outType in outformats:
-        writeFiles(data_path, fileprefix, train, test, tid_col, class_col, \
-                 columns_order_zip if outType in ['zip', 'mat'] else columns_order_csv, outformat=outType)
-#     write_trainAndTest(data_path, train, test, tid_col, class_col, fileprefix)
-    
-    if verbose:
-        print("Done.")
-        print(" --------------------------------------------------------------------------------")
-    return train, test
-
 def splitData(df, k, random_num, tid_col='tid', class_col='label', opLabel='Spliting Data', ignore_ltk=True):
     
     if ignore_ltk: # removes labels with less than k trajectories...
         df = dropLabelsltk(df, k, tid_col, class_col)
     
     ktrain = []
     ktest = []
     for x in range(k):
         ktrain.append( pd.DataFrame() )
         ktest.append( pd.DataFrame() )
 
-#     print("Spliting data...")
     kfold = KFold(n_splits=k, shuffle=True, random_state=random_num)
-#         for label in df[class_col].unique(): 
+
     def addData(label):
         tids = df.loc[df[class_col] == label][tid_col].unique()
         x = 0
         for train_idx, test_idx in kfold.split(tids):
             ktrain[x] = pd.concat([ktrain[x], df.loc[df[tid_col].isin(tids[train_idx])]])
             ktest[x]  = pd.concat([ktest[x],  df.loc[df[tid_col].isin(tids[test_idx])]])
             x += 1
@@ -439,234 +898,56 @@
     return ktrain, ktest
 
 def dropLabelsltk(df, k, tid_col='tid', class_col='label'):
     df_ = df.groupby(by=class_col, as_index=False).agg({tid_col: pd.Series.nunique})
     index_names = df[df[class_col].isin(df_[df_[tid_col] < k][class_col])].index
     return df.drop(index_names)
 
-def kfold_trainAndTestSplit(data_path, k, df, random_num=1, tid_col='tid', class_col='label', fileprefix='', columns_order=None, ktrain=None, ktest=None, mat_columns=None, outformats=['zip', 'csv', 'mat'], verbose=False):
-#     from ..main import importer
-#    importer(['S', 'KFold'], globals())
-    
-    print(str(k)+"-fold train and test split in... " + data_path)
-    
-    df, columns_order_zip, columns_order_csv = organizeFrame(df, columns_order, tid_col, class_col)
-    
-    if not ktrain:
-        ktrain, ktest = splitData(df, k, random_num, tid_col, class_col)
-    else:
-        print("Train and test data provided.")
-    
-#     print("Writing files...")
-    for x in range(k):            
-        train_aux = ktrain[x]
-        test_aux  = ktest[x]
-        
-        for outType in outformats:
-            print("Writing", outType, "files ... " + str(x+1) +'/'+str(k))
-            path = 'run'+str(x+1)
-            if not os.path.exists(os.path.join(data_path, path)):
-                os.makedirs(os.path.join(data_path, path))
-                
-            writeFiles(data_path, os.path.join(path, fileprefix), train_aux, test_aux, tid_col, class_col, \
-                     columns_order_zip if outType in ['zip', 'mat'] else columns_order_csv, mat_columns, None, \
-                     outType, opSuff=str(x+1))
-    print("Done.")
-    print(" --------------------------------------------------------------------------------")
-    
-    return ktrain, ktest
-
-def stratify(df, sample_size=0.5, train_size=0.7, random_num=1, tid_col='tid', class_col='label', 
-             organize_columns=True, mat_columns=None, fileprefix='', outformats=['zip', 'csv', 'mat'], data_path='.'):
-#    importer(['S', 'train_test_split'], globals())
-    
-    train_index, _, _ = splitTIDs(df, sample_size, random_num, tid_col, class_col, min_elements=2)
-    
-    df = df.loc[df[tid_col].isin(train_index)]
-    
-    train_index, test_index, _ = splitTIDs(df, train_size, random_num, tid_col, class_col, min_elements=1)
-    
-    if organize_columns:
-        df, columns_order_zip, columns_order_csv = organizeFrame(df, None, tid_col, class_col)
-    else:
-        columns_order_zip = list(df.columns)
-        columns_order_csv = list(df.columns)
-    
-    train = df.loc[df[tid_col].isin(train_index)]
-    test  = df.loc[df[tid_col].isin(test_index)]
-    
-    for outType in outformats:
-        path = 'S'+str(int(sample_size*100))
-        if not os.path.exists(os.path.join(data_path, path)):
-                os.makedirs(os.path.join(data_path, path))
-            
-        writeFiles(data_path, os.path.join(path, fileprefix), train, test, tid_col, class_col, \
-                 columns_order_zip if outType in ['zip', 'mat'] else columns_order_csv, mat_columns, None, outType, opSuff=path)
-    
-    return train, test
-    
-# TODO fix stratify:
-def kfold_stratify(data_path, df, k=10, inc=1, limit=10, random_num=1, tid_col='tid', class_col='label', fileprefix='', 
-             ktrain=None, ktest=None, organize_columns=True, mat_columns=None, outformats=['zip', 'csv', 'mat'], ignore_ltk=True):
-#    importer(['S', 'KFold'], globals())
-    
-    print(str(k)+"-fold stratification of train and test in... " + data_path)
-    
-    if organize_columns:
-        df, columns_order_zip, columns_order_csv = organizeFrame(df, None, tid_col, class_col)
-    else:
-        columns_order_zip = list(df.columns)
-        columns_order_csv = list(df.columns)
-        
-    if not ktrain:
-        ktrain, ktest = splitData(df, k, random_num, tid_col, class_col, ignore_ltk=ignore_ltk)
-    else:
-        print("Train and test data provided.")
-    
-    for x in range(0, limit, inc):
-        
-        train_aux = ktrain[0]
-        test_aux  = ktest[0]
-        for y in range(1, x+1):
-            train_aux = pd.concat([train_aux,  ktrain[y]])
-            test_aux  = pd.concat([test_aux,   ktest[y]])
-            
-        for outType in outformats:
-            path = 'S'+str((x+1)*int(100/k))
-
-            if not os.path.exists(os.path.join(data_path, path)):
-                os.makedirs(os.path.join(data_path, path))
-            
-            writeFiles(data_path, os.path.join(path, fileprefix), train_aux, test_aux, tid_col, class_col, \
-                     columns_order_zip if outType in ['zip', 'mat'] else columns_order_csv, mat_columns, None, outType, opSuff=str(x+1))
-    print(" Done.")
-    print(" --------------------------------------------------------------------------------")
-    
-    return ktrain, ktest
+def labels_extract(df, labels=[], tid_col='tid', class_col='label', organize_columns=True):
 
-def klabels_stratify(df, kl=10, train_size=0.7, random_num=1, tid_col='tid', class_col='label', 
-             organize_columns=True, mat_columns=None, fileprefix='', outformats=['zip', 'csv', 'mat'], data_path='.'):
-
-    min_elements=1
-    
-    random.seed(random_num)
-    labels = df[class_col].unique()
-
-    n = min_elements if lk < min_elements else n
-
-    labels_index = random.sample(list(labels), n)
-    df = df.loc[df[class_col].isin(labels_index)]
-    
-    train_index, test_index, _ = splitTIDs(df, train_size, random_num, tid_col, class_col, min_elements=min_elements)
+    df = df.loc[df[class_col].isin(labels)].copy()
     
     if organize_columns:
         df, columns_order_zip, columns_order_csv = organizeFrame(df, None, tid_col, class_col)
     else:
         columns_order_zip = list(df.columns)
         columns_order_csv = list(df.columns)
     
-    train = df.loc[df[tid_col].isin(train_index)]
-    test  = df.loc[df[tid_col].isin(test_index)]
-    
-    for outType in outformats:
-        path = 'L'+str(n)
-        if not os.path.exists(os.path.join(data_path, path)):
-                os.makedirs(os.path.join(data_path, path))
-                
-        writeFiles(data_path, os.path.join(path, fileprefix), train, test, tid_col, class_col, \
-                 columns_order_zip if outType in ['zip', 'mat'] else columns_order_csv, mat_columns, None, outType, opSuff=path)
-    
-    return train, test
-
-#def stratify(data_path, df, k=10, inc=1, limit=10, random_num=1, tid_col='tid', class_col='label', fileprefix='', 
-#             ktrain=None, ktest=None, organize_columns=True, mat_columns=None, outformats=['zip', 'csv', 'mat'], ignore_ltk=True):
-#    importer(['S', 'KFold'], globals())
-#    
-#    print(str(k)+"-fold stratification of train and test in... " + data_path)
-#    
-#    if organize_columns:
-#        df, columns_order_zip, columns_order_csv = organizeFrame(df, None, tid_col, class_col)
-#    else:
-#        columns_order_zip = list(df.columns)
-#        columns_order_csv = list(df.columns)
-#        
-#    if not ktrain:
-#        ktrain, ktest = splitData(df, k, random_num, tid_col, class_col, ignore_ltk=ignore_ltk)
-#    else:
-#        print("Train and test data provided.")
-#    
-#    for x in range(0, limit, inc):
-#        path = 'S'+str((x+1)*int(100/k))
-#        
-#        if not os.path.exists(os.path.join(data_path, path)):
-#            os.makedirs(os.path.join(data_path, path))
-#            
-#        train_aux = ktrain[0]
-#        test_aux  = ktest[0]
-#        for y in range(1, x+1):
-#            train_aux = pd.concat([train_aux,  ktrain[y]])
-#            test_aux  = pd.concat([test_aux,   ktest[y]])
-#            
-#        for outType in outformats:
-#            writeFiles(data_path, os.path.join(path, fileprefix), train_aux, test_aux, tid_col, class_col, \
-#                     columns_order_zip if outType in ['zip', 'mat'] else columns_order_csv, mat_columns, None, outType, opSuff=str(x+1))
-#    print(" Done.")
-#    print(" --------------------------------------------------------------------------------")
-#    
-#    return ktrain, ktest
+    return df
         
 def writeFile(data_path, df, file, tid_col, class_col, columns_order, mat_columns=None, desc_cols=None, outformat='zip', opSuff=''):
     if outformat == 'zip':
         # WRITE ZIP >> FOR MASTERMovelets:
         df2zip(data_path, df, file, tid_col, class_col, select_cols=columns_order,\
                opLabel='Writing - ZIP |' + opSuff)
         
     elif outformat == 'csv':
         print('Writing - CSV |' + opSuff)
         df[columns_order].to_csv(os.path.join(data_path, file+".csv"), index = False)
         
+    elif outformat == 'parquet':
+        print('Writing - Parquet |' + opSuff)
+        df[columns_order].to_parquet(os.path.join(data_path, file+".parquet"), index = False)
+        
     elif outformat == 'mat':
         # WRITE MAT Files >> FOR HiPerMovelets:
         df2mat(df, data_path, file, cols=columns_order, mat_cols=mat_columns, tid_col=tid_col, class_col=class_col, \
                desc_cols=desc_cols, opLabel='Writing - MAT|' + opSuff)
         
 def writeFiles(data_path, file, train, test, tid_col, class_col, columns_order, mat_columns=None, desc_cols=None, outformat='zip', opSuff=''):
     # WRITE Train
     writeFile(data_path, train, file+'train', tid_col, class_col, columns_order, mat_columns, desc_cols, 
               outformat, opSuff='TRAIN - '+opSuff)
     # WRITE Test
     writeFile(data_path, test,  file+'test',  tid_col, class_col, columns_order, mat_columns, desc_cols, 
               outformat, opSuff='TEST - '+ opSuff)
     
-#def writeFiles(data_path, file, train, test, tid_col, class_col, columns_order, mat_columns=None, outformat='zip', opSuff=''):
-#    if outformat == 'zip':
-#        # WRITE ZIP Train / Test Files >> FOR MASTERMovelets:
-#        df2zip(data_path, train, file+'train', tid_col, class_col, select_cols=columns_order,\
-#               opLabel='Writing TRAIN - ZIP|' + opSuff)
-#        df2zip(data_path, test,  file+'test', tid_col, class_col, select_cols=columns_order, \
-#               opLabel='Writing TEST  - ZIP|' + opSuff)
-#        
-#    elif outformat == 'csv':
-#        print('Writing TRAIN / TEST - CSV|' + opSuff)
-#        train[columns_order].to_csv(os.path.join(data_path, file+"train.csv"), index = False)
-#        test[ columns_order].to_csv(os.path.join(data_path, file+"test.csv"),  index = False)
-#        
-#    elif outformat == 'mat':
-#        # WRITE ZIP Train / Test Files >> FOR HiPerMovelets:
-#        df2mat(train, data_path, file+'train', cols=columns_order, mat_cols=mat_columns, tid_col=tid_col, class_col=class_col, \
-#               opLabel='Writing TRAIN - MAT|' + opSuff)
-#        df2mat(test,  data_path, file+'test', cols=columns_order, mat_cols=mat_columns, tid_col=tid_col, class_col=class_col, \
-#               opLabel='Writing TEST  - MAT|' + opSuff)
-#        
-    
+
 #-------------------------------------------------------------------------->>
-def splitframe(data, name='tid'):
-#     from ..main import importer
-#     importer(['S'], locals())
-    
+def splitframe(data, name='tid'):    
     n = data[name][0]
 
     df = pd.DataFrame(columns=data.columns)
 
     datalist = []
 
     for i in range(len(data)):
@@ -675,67 +956,19 @@
         else:
             datalist.append(df)
             df = pd.DataFrame(columns=data.columns)
             n = data[name][i]
             df = df.append(data.iloc[i])
 
     return datalist
-    
-#-------------------------------------------------------------------------->>    
-
-#-------------------------------------------------------------------------->>
-def joinTrainAndTest(dir_path, train_file="train.csv", test_file="test.csv", tid_col='tid', class_col = 'label', to_file=False):
-#     from ..main import importer
-#     importer(['S'], locals())
-    
-    print("Joining train and test data from... " + dir_path)
-    
-    # Read datasets
-    dataset_train = readDataset(dir_path, None, train_file)
-    dataset_test  = readDataset(dir_path, None, test_file)
-    
-    dataset = pd.concat([dataset_train, dataset_test])
-#     if '.csv' in train_file:
-#         print("Reading train file...")
-#         dataset_train = pd.read_csv(os.path.join(dir_path, train_file))
-#     else:
-#         print("Converting train file...")
-#         dataset_train = zip2csv(dir_path, train_file, cols, class_col)
-#     print("Done.")
-        
-#     if '.csv' in test_file:
-#         print("Reading test file...")
-#         dataset_test  = pd.read_csv(os.path.join(dir_path, test_file))
-#     else:
-#         print("Converting test file...")
-#         dataset_test = zip2csv(dir_path, test_file, cols, class_col)
-    dataset.sort_values([class_col, tid_col])
-    print("Done.")
-    
-    if to_file:
-        print("Saving joined dataset as: " + os.path.join(dir_path, 'joined.csv'))
-
-        dataset.to_csv(os.path.join(dir_path, 'joined.csv'), index=False)
-        print("Done.")
-    print(" --------------------------------------------------------------------------------")
-    
-    return dataset
 
 #--------------------------------------------------------------------------------
 def convertDataset(dir_path, k=None, cols = None, fileprefix='', tid_col='tid', class_col='label'):
     def convert_file(file, cols):
         df = readDataset(dir_path, fileprefix+file+'.csv')
-#        if os.path.exists(os.path.join(dir_path, 'specific_'+file+'.csv')):
-#            # Option 1:
-#            df = pd.read_csv(os.path.join(dir_path, 'specific_'+file+'.csv'))
-#        elif os.path.exists(os.path.join(dir_path, file+'.zip')):
-#            df = convert_zip2csv(dir_path, file, cols, class_col)
-#        else:
-##             print("File "+file+" not found, nothing to do.")
-#            raise Exception("File "+file+" not found, nothing to do.")
             
         if not cols:
             cols = list(df.columns)
         df, columns_order_zip, columns_order_csv = organizeFrame(df, cols, tid_col, class_col)
         
         outformats = []
         if not os.path.exists(os.path.join(dir_path, file+'.zip')):
@@ -759,21 +992,21 @@
     for outType in outformats:
         writeFiles(dir_path, fileprefix, df_train, df_test, tid_col, class_col, \
                  columns_order_zip if outType in ['zip', 'mat'] else columns_order_csv, None, outType, opSuff='')
     
     data = pd.concat([df_train,df_test])
 
     if k and not os.path.exists(os.path.join(dir_path, 'run1')):
-        train, test = kfold_trainAndTestSplit(dir_path, k, data, fileprefix=fileprefix, random_num=1, tid_col=tid_col, class_col=class_col, columns_order=columns_order_csv)
+        train, test = kfold_trainTestSplit(data, k, fileprefix=fileprefix, random_num=1, tid_col=tid_col, class_col=class_col, columns_order=columns_order_csv, data_path=dir_path)
         for i in range(1, k+1):
             for file in ['train', 'test']:
                 os.rename(os.path.join(dir_path, 'run'+str(i), fileprefix+file+'.zip'), 
                           os.path.join(dir_path, 'run'+str(i), file+'.zip'))
 
         if 'space' in columns_order_zip:
-            kfold_trainAndTestSplit(dir_path, k, None, random_num=1, fileprefix='raw_', tid_col=tid_col, class_col=class_col, columns_order=columns_order_csv, ktrain=train, ktest=test)
+            kfold_trainTestSplit(None, k, random_num=1, fileprefix='raw_', tid_col=tid_col, class_col=class_col, columns_order=columns_order_csv, ktrain=train, ktest=test, data_path=dir_path)
             for i in range(1, k+1):
                 for file in ['train', 'test']:
                     os.remove(os.path.join(dir_path, 'run'+str(i), 'raw_'+file+'.zip'))
     
     print("All Done.")
 #--------------------------------------------------------------------------------
```

### Comparing `mat-data-0.1b9/pyproject.toml` & `mat_data-0.1rc1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*-
 [project]
 name = "mat-data"
-version = "0.1b9"
+version = "0.1rc1"
 description = "MAT-data: Data Preprocessing for Multiple Aspect Trajectory Data Mining"
 authors = [
     {name = "Tarlis Tortelli Portela", email = "tarlis@tarlis.com.br"},
  ]
 maintainers = [
     {name = "Tarlis Tortelli Portela", email = "tarlis@tarlis.com.br"},
  ]
@@ -37,20 +37,22 @@
     "Programming Language :: Python :: 3.10",
  ]
 requires-python = ">=3.7"
 dependencies = [
     "glob2",
     "numpy",
     "pandas",
-    "mat-data",
+    "mat-model",
  ]
 
 [project.optional-dependencies]
 all_extras = [
     "geohash",
+    "pyarrow",
+    "fastparquet",
  ]
 
 dev = [
     "pre-commit",
     "pytest",
     "pytest-cov",
     "pytest-xdist",
@@ -63,19 +65,19 @@
 
 docs = [
     "jupyter",
     "numpydoc",
  ]
 
 [project.urls]
-"Homepage" = "https://github.com/ttportela/mat-data"
-"Repository" = "https://github.com/ttportela/mat-data"
-"Documentation" = "https://github.com/ttportela/mat-data/blob/main/README.md"
+"Homepage" = "https://github.com/mat-analysis/mat-data"
+"Repository" = "https://github.com/mat-analysis/mat-data"
+"Documentation" = "https://github.com/mat-analysis/mat-data/blob/main/README.md"
 "Download" = "https://pypi.org/project/mat-data/#files"
-"Bug Tracker" = "https://github.com/ttportela/mat-data/issues"
+"Bug Tracker" = "https://github.com/mat-analysis/mat-data/issues"
 
 [project.license]
 text = 'GPL Version 3 or superior (see LICENSE file)'
 
 [tool.poetry]
 include = ["CHANGELOG.md"]
```

### Comparing `mat-data-0.1b9/setup.py` & `mat_data-0.1rc1/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,16 +1,12 @@
 # -*- coding: utf-8 -*-
 """
-Multiple Aspect Trajectory Tools Framework, MAT-data: Data Preprocessing for Multiple Aspect Trajectory Data Mining
+# MAT-data: Data Preprocessing for Multiple Aspect Trajectory Data Mining
 
-The present application offers a tool, to support the user in the classification task of multiple aspect trajectories,
-specifically for extracting and visualizing the movelets, the parts of the trajectory that better discriminate a class.
-It integrates into a unique platform the fragmented approaches available for multiple aspects trajectories and in
-general for multidimensional sequence classification into a unique web-based and python library system. Offers both
-movelets visualization and classification methods.
+The present application offers a tool, to support the user in the data mining task of multiple aspect trajectories, specifically for measuring similarity of its complex data. It integrates into a unique platform the fragmented approaches available for multiple aspects trajectories and in general for multidimensional sequence classification into a unique web-based and python library system. 
 
 Created on Dec, 2023
 Copyright (C) 2023, License GPL Version 3 or superior (see LICENSE file)
 
 @author: Tarlis Portela
 """
 import setuptools
@@ -18,38 +14,37 @@
 import configparser
 config = configparser.ConfigParser()
 config.read('pyproject.toml')
 VERSION = config['project']['version'].strip('"')
 PACKAGE_NAME = config['project']['name'].strip('"')
 DEV_VERSION = "0.1b0"
 
-with open("matdata/README.md", "r", encoding="utf-8") as fh:
+with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
     
 setuptools.setup(
     name=PACKAGE_NAME,
     version=VERSION,
 #    version=DEV_VERSION,
-    author="Tarlis Tortelli Portela",
+    author="Tarlis Portela",
     author_email="tarlis@tarlis.com.br",
     description="MAT-data: Data Preprocessing for Multiple Aspect Trajectory Data Mining",
     long_description=long_description,
     long_description_content_type="text/markdown",
-    url="https://github.com/ttportela/mat-data",
+    url="https://github.com/mat-analysis/mat-data",
 #    packages=setuptools.find_packages(include=[PACKAGE_NAME, PACKAGE_NAME+'.*']),
     packages=setuptools.find_packages(),
 #    include_package_data=True,
 #    scripts=[
 #         'scripts/x.py', # For future
 #    ],
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)",
         "Operating System :: OS Independent",
         "Intended Audience :: Science/Research",
         "Topic :: Scientific/Engineering :: Artificial Intelligence",
         "Topic :: Scientific/Engineering :: Information Analysis",
-        "Topic :: Scientific/Engineering :: Visualization",
     ],
     keywords='data mining, python, trajectory classification, trajectory analysis, movelets',
     license='GPL Version 3 or superior (see LICENSE file)',
 )
```

