# Comparing `tmp/vmklib-1.9.0.tar.gz` & `tmp/vmklib-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vmklib-1.9.0.tar", last modified: Wed Jul 12 21:50:16 2023, max compression
+gzip compressed data, was "vmklib-2.0.0.tar", last modified: Thu Oct  5 19:00:10 2023, max compression
```

## Comparing `vmklib-1.9.0.tar` & `vmklib-2.0.0.tar`

### file list

```diff
@@ -1,71 +1,72 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 21:50:16.962616 vmklib-1.9.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-07-12 21:47:23.000000 vmklib-1.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    13192 2023-07-12 21:50:16.958615 vmklib-1.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10963 2023-07-12 21:47:23.000000 vmklib-1.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1244 2023-07-12 21:47:23.000000 vmklib-1.9.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-12 21:50:16.962616 vmklib-1.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      821 2023-07-12 21:47:23.000000 vmklib-1.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 21:50:16.954615 vmklib-1.9.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     4016 2023-07-12 21:47:23.000000 vmklib-1.9.0/tests/test_entry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 21:50:16.954615 vmklib-1.9.0/vmklib/
--rw-r--r--   0 runner    (1001) docker     (123)      325 2023-07-12 21:47:23.000000 vmklib-1.9.0/vmklib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      326 2023-07-12 21:47:23.000000 vmklib-1.9.0/vmklib/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8021 2023-07-12 21:47:23.000000 vmklib-1.9.0/vmklib/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 21:50:16.954615 vmklib-1.9.0/vmklib/data/
--rw-r--r--   0 runner    (1001) docker     (123)     1626 2023-07-12 21:47:23.000000 vmklib-1.9.0/vmklib/data/conf.mk
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 21:50:16.958615 vmklib-1.9.0/vmklib/data/data/
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-12 21:47:23.000000 vmklib-1.9.0/vmklib/data/data/edit_venv.txt
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 21:47:23.000000 vmklib-1.9.0/vmklib/data/data/fresh_venv.txt
--rw-r--r--   0 runner    (1001) docker     (123)      554 2023-07-12 21:47:23.000000 vmklib-1.9.0/vmklib/data/data/header.mk
--rw-r--r--   0 runner    (1001) docker     (123)      862 2023-07-12 21:47:23.000000 vmklib-1.9.0/vmklib/data/datazen.mk
--rw-r--r--   0 runner    (1001) docker     (123)      835 2023-07-12 21:47:23.000000 vmklib-1.9.0/vmklib/data/functions.mk
--rw-r--r--   0 runner    (1001) docker     (123)      790 2023-07-12 21:47:23.000000 vmklib-1.9.0/vmklib/data/grip.mk
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 21:50:16.958615 vmklib-1.9.0/vmklib/data/lib_tasks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 21:47:23.000000 vmklib-1.9.0/vmklib/data/lib_tasks/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 21:50:16.958615 vmklib-1.9.0/vmklib/data/lib_tasks/__pycache__/
--rw-r--r--   0 runner    (1001) docker     (123)     3213 2023-07-12 21:47:37.000000 vmklib-1.9.0/vmklib/data/lib_tasks/__pycache__/conf.cpython-311.pyc
--rw-r--r--   0 runner    (1001) docker     (123)     2374 2023-07-12 21:47:23.000000 vmklib-1.9.0/vmklib/data/lib_tasks/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 21:50:16.958615 vmklib-1.9.0/vmklib/data/python/
--rw-r--r--   0 runner    (1001) docker     (123)     1943 2023-07-12 21:47:23.000000 vmklib-1.9.0/vmklib/data/python/build.mk
--rw-r--r--   0 runner    (1001) docker     (123)      720 2023-07-12 21:47:23.000000 vmklib-1.9.0/vmklib/data/python/docs.mk
--rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-07-12 21:47:23.000000 vmklib-1.9.0/vmklib/data/python/pypi.mk
--rw-r--r--   0 runner    (1001) docker     (123)      608 2023-07-12 21:47:23.000000 vmklib-1.9.0/vmklib/data/python/upload.mk
--rw-r--r--   0 runner    (1001) docker     (123)     2685 2023-07-12 21:47:23.000000 vmklib-1.9.0/vmklib/data/python.mk
--rw-r--r--   0 runner    (1001) docker     (123)      789 2023-07-12 21:47:23.000000 vmklib-1.9.0/vmklib/data/time.mk
--rw-r--r--   0 runner    (1001) docker     (123)     1623 2023-07-12 21:47:23.000000 vmklib-1.9.0/vmklib/data/venv.mk
--rw-r--r--   0 runner    (1001) docker     (123)      795 2023-07-12 21:47:23.000000 vmklib-1.9.0/vmklib/data/vmklib.mk
--rw-r--r--   0 runner    (1001) docker     (123)      449 2023-07-12 21:47:23.000000 vmklib-1.9.0/vmklib/data/yaml.mk
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-12 21:47:23.000000 vmklib-1.9.0/vmklib/dev_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2004 2023-07-12 21:47:23.000000 vmklib-1.9.0/vmklib/entry.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 21:47:23.000000 vmklib-1.9.0/vmklib/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-12 21:47:23.000000 vmklib-1.9.0/vmklib/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      844 2023-07-12 21:47:23.000000 vmklib-1.9.0/vmklib/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 21:50:16.958615 vmklib-1.9.0/vmklib/tasks/
--rw-r--r--   0 runner    (1001) docker     (123)      473 2023-07-12 21:47:23.000000 vmklib-1.9.0/vmklib/tasks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      642 2023-07-12 21:47:23.000000 vmklib-1.9.0/vmklib/tasks/args.py
--rw-r--r--   0 runner    (1001) docker     (123)      653 2023-07-12 21:47:23.000000 vmklib-1.9.0/vmklib/tasks/clean.py
--rw-r--r--   0 runner    (1001) docker     (123)      861 2023-07-12 21:47:23.000000 vmklib-1.9.0/vmklib/tasks/github.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 21:50:16.958615 vmklib-1.9.0/vmklib/tasks/mixins/
--rw-r--r--   0 runner    (1001) docker     (123)      356 2023-07-12 21:47:23.000000 vmklib-1.9.0/vmklib/tasks/mixins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2510 2023-07-12 21:47:23.000000 vmklib-1.9.0/vmklib/tasks/mixins/concrete.py
--rw-r--r--   0 runner    (1001) docker     (123)     1864 2023-07-12 21:47:23.000000 vmklib-1.9.0/vmklib/tasks/mixins/curl.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 21:50:16.958615 vmklib-1.9.0/vmklib/tasks/node/
--rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-07-12 21:47:23.000000 vmklib-1.9.0/vmklib/tasks/node/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 21:50:16.958615 vmklib-1.9.0/vmklib/tasks/python/
--rw-r--r--   0 runner    (1001) docker     (123)     1724 2023-07-12 21:47:23.000000 vmklib-1.9.0/vmklib/tasks/python/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1900 2023-07-12 21:47:23.000000 vmklib-1.9.0/vmklib/tasks/python/build.py
--rw-r--r--   0 runner    (1001) docker     (123)     1467 2023-07-12 21:47:23.000000 vmklib-1.9.0/vmklib/tasks/python/datazen.py
--rw-r--r--   0 runner    (1001) docker     (123)     1938 2023-07-12 21:47:23.000000 vmklib-1.9.0/vmklib/tasks/python/docs.py
--rw-r--r--   0 runner    (1001) docker     (123)     4196 2023-07-12 21:47:23.000000 vmklib-1.9.0/vmklib/tasks/python/lint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1907 2023-07-12 21:47:23.000000 vmklib-1.9.0/vmklib/tasks/python/package.py
--rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-07-12 21:47:23.000000 vmklib-1.9.0/vmklib/tasks/python/sa.py
--rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-07-12 21:47:23.000000 vmklib-1.9.0/vmklib/tasks/python/test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-07-12 21:47:23.000000 vmklib-1.9.0/vmklib/tasks/python/yaml.py
--rw-r--r--   0 runner    (1001) docker     (123)     5001 2023-07-12 21:47:23.000000 vmklib-1.9.0/vmklib/tasks/venv.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 21:50:16.954615 vmklib-1.9.0/vmklib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13192 2023-07-12 21:50:16.000000 vmklib-1.9.0/vmklib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-07-12 21:50:16.000000 vmklib-1.9.0/vmklib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 21:50:16.000000 vmklib-1.9.0/vmklib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-12 21:50:16.000000 vmklib-1.9.0/vmklib.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-07-12 21:50:16.000000 vmklib-1.9.0/vmklib.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-12 21:50:16.000000 vmklib-1.9.0/vmklib.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-05 19:00:10.316212 vmklib-2.0.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2023-10-05 18:57:32.000000 vmklib-2.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    14055 2023-10-05 19:00:10.316212 vmklib-2.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    11310 2023-10-05 18:57:32.000000 vmklib-2.0.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1261 2023-10-05 18:57:32.000000 vmklib-2.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2023-10-05 19:00:10.316212 vmklib-2.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      807 2023-10-05 18:57:32.000000 vmklib-2.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-05 19:00:10.308212 vmklib-2.0.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     4016 2023-10-05 18:57:32.000000 vmklib-2.0.0/tests/test_entry.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-05 19:00:10.308212 vmklib-2.0.0/vmklib/
+-rw-r--r--   0 runner    (1001) docker     (127)      325 2023-10-05 18:57:32.000000 vmklib-2.0.0/vmklib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      326 2023-10-05 18:57:32.000000 vmklib-2.0.0/vmklib/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8044 2023-10-05 18:57:32.000000 vmklib-2.0.0/vmklib/app.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-05 19:00:10.308212 vmklib-2.0.0/vmklib/data/
+-rw-r--r--   0 runner    (1001) docker     (127)     1626 2023-10-05 18:57:32.000000 vmklib-2.0.0/vmklib/data/conf.mk
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-05 19:00:10.312212 vmklib-2.0.0/vmklib/data/data/
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2023-10-05 18:57:32.000000 vmklib-2.0.0/vmklib/data/data/edit_venv.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-05 18:57:32.000000 vmklib-2.0.0/vmklib/data/data/fresh_venv.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      554 2023-10-05 18:57:32.000000 vmklib-2.0.0/vmklib/data/data/header.mk
+-rw-r--r--   0 runner    (1001) docker     (127)      862 2023-10-05 18:57:32.000000 vmklib-2.0.0/vmklib/data/datazen.mk
+-rw-r--r--   0 runner    (1001) docker     (127)      835 2023-10-05 18:57:32.000000 vmklib-2.0.0/vmklib/data/functions.mk
+-rw-r--r--   0 runner    (1001) docker     (127)      790 2023-10-05 18:57:32.000000 vmklib-2.0.0/vmklib/data/grip.mk
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-05 19:00:10.312212 vmklib-2.0.0/vmklib/data/lib_tasks/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-05 18:57:32.000000 vmklib-2.0.0/vmklib/data/lib_tasks/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-05 19:00:10.312212 vmklib-2.0.0/vmklib/data/lib_tasks/__pycache__/
+-rw-r--r--   0 runner    (1001) docker     (127)     3317 2023-10-05 18:57:40.000000 vmklib-2.0.0/vmklib/data/lib_tasks/__pycache__/conf.cpython-311.pyc
+-rw-r--r--   0 runner    (1001) docker     (127)     2483 2023-10-05 18:57:32.000000 vmklib-2.0.0/vmklib/data/lib_tasks/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-05 19:00:10.312212 vmklib-2.0.0/vmklib/data/python/
+-rw-r--r--   0 runner    (1001) docker     (127)     1943 2023-10-05 18:57:32.000000 vmklib-2.0.0/vmklib/data/python/build.mk
+-rw-r--r--   0 runner    (1001) docker     (127)      720 2023-10-05 18:57:32.000000 vmklib-2.0.0/vmklib/data/python/docs.mk
+-rw-r--r--   0 runner    (1001) docker     (127)     1092 2023-10-05 18:57:32.000000 vmklib-2.0.0/vmklib/data/python/pypi.mk
+-rw-r--r--   0 runner    (1001) docker     (127)      608 2023-10-05 18:57:32.000000 vmklib-2.0.0/vmklib/data/python/upload.mk
+-rw-r--r--   0 runner    (1001) docker     (127)     2685 2023-10-05 18:57:32.000000 vmklib-2.0.0/vmklib/data/python.mk
+-rw-r--r--   0 runner    (1001) docker     (127)      789 2023-10-05 18:57:32.000000 vmklib-2.0.0/vmklib/data/time.mk
+-rw-r--r--   0 runner    (1001) docker     (127)     1623 2023-10-05 18:57:32.000000 vmklib-2.0.0/vmklib/data/venv.mk
+-rw-r--r--   0 runner    (1001) docker     (127)      795 2023-10-05 18:57:32.000000 vmklib-2.0.0/vmklib/data/vmklib.mk
+-rw-r--r--   0 runner    (1001) docker     (127)      449 2023-10-05 18:57:32.000000 vmklib-2.0.0/vmklib/data/yaml.mk
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2023-10-05 18:57:32.000000 vmklib-2.0.0/vmklib/dev_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1849 2023-10-05 18:57:32.000000 vmklib-2.0.0/vmklib/entry.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-05 18:57:32.000000 vmklib-2.0.0/vmklib/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2023-10-05 18:57:32.000000 vmklib-2.0.0/vmklib/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-05 19:00:10.312212 vmklib-2.0.0/vmklib/tasks/
+-rw-r--r--   0 runner    (1001) docker     (127)      473 2023-10-05 18:57:32.000000 vmklib-2.0.0/vmklib/tasks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      642 2023-10-05 18:57:32.000000 vmklib-2.0.0/vmklib/tasks/args.py
+-rw-r--r--   0 runner    (1001) docker     (127)      653 2023-10-05 18:57:32.000000 vmklib-2.0.0/vmklib/tasks/clean.py
+-rw-r--r--   0 runner    (1001) docker     (127)      861 2023-10-05 18:57:32.000000 vmklib-2.0.0/vmklib/tasks/github.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-05 19:00:10.312212 vmklib-2.0.0/vmklib/tasks/mixins/
+-rw-r--r--   0 runner    (1001) docker     (127)      356 2023-10-05 18:57:32.000000 vmklib-2.0.0/vmklib/tasks/mixins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2510 2023-10-05 18:57:32.000000 vmklib-2.0.0/vmklib/tasks/mixins/concrete.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1864 2023-10-05 18:57:32.000000 vmklib-2.0.0/vmklib/tasks/mixins/curl.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-05 19:00:10.312212 vmklib-2.0.0/vmklib/tasks/node/
+-rw-r--r--   0 runner    (1001) docker     (127)     1564 2023-10-05 18:57:32.000000 vmklib-2.0.0/vmklib/tasks/node/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-05 19:00:10.312212 vmklib-2.0.0/vmklib/tasks/python/
+-rw-r--r--   0 runner    (1001) docker     (127)      310 2023-10-05 18:57:32.000000 vmklib-2.0.0/vmklib/tasks/python/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1894 2023-10-05 18:57:32.000000 vmklib-2.0.0/vmklib/tasks/python/build.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1467 2023-10-05 18:57:32.000000 vmklib-2.0.0/vmklib/tasks/python/datazen.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1938 2023-10-05 18:57:32.000000 vmklib-2.0.0/vmklib/tasks/python/docs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4459 2023-10-05 18:57:32.000000 vmklib-2.0.0/vmklib/tasks/python/lint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1907 2023-10-05 18:57:32.000000 vmklib-2.0.0/vmklib/tasks/python/package.py
+-rw-r--r--   0 runner    (1001) docker     (127)      644 2023-10-05 18:57:32.000000 vmklib-2.0.0/vmklib/tasks/python/release.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1196 2023-10-05 18:57:32.000000 vmklib-2.0.0/vmklib/tasks/python/sa.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1845 2023-10-05 18:57:32.000000 vmklib-2.0.0/vmklib/tasks/python/test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1171 2023-10-05 18:57:32.000000 vmklib-2.0.0/vmklib/tasks/python/yaml.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3317 2023-10-05 18:57:32.000000 vmklib-2.0.0/vmklib/tasks/release.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5194 2023-10-05 18:57:32.000000 vmklib-2.0.0/vmklib/tasks/venv.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-05 19:00:10.308212 vmklib-2.0.0/vmklib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    14055 2023-10-05 19:00:10.000000 vmklib-2.0.0/vmklib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1441 2023-10-05 19:00:10.000000 vmklib-2.0.0/vmklib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-05 19:00:10.000000 vmklib-2.0.0/vmklib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2023-10-05 19:00:10.000000 vmklib-2.0.0/vmklib.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      141 2023-10-05 19:00:10.000000 vmklib-2.0.0/vmklib.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2023-10-05 19:00:10.000000 vmklib-2.0.0/vmklib.egg-info/top_level.txt
```

### Comparing `vmklib-1.9.0/LICENSE` & `vmklib-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `vmklib-1.9.0/PKG-INFO` & `vmklib-2.0.0/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,83 +1,41 @@
-Metadata-Version: 2.1
-Name: vmklib
-Version: 1.9.0
-Summary: Simplify project workflows by standardizing use of GNU Make.
-Home-page: https://github.com/vkottler/vmklib
-Author: Vaughn Kottler
-Author-email: Vaughn Kottler <vaughnkottler@gmail.com>
-Maintainer-email: Vaughn Kottler <vaughnkottler@gmail.com>
-License: MIT License
-        
-        Copyright (c) 2023 Vaughn Kottler
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
-        
-Keywords: workflow,tool,make
-Classifier: Topic :: Software Development :: Build Tools
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Operating System :: Microsoft :: Windows
-Classifier: Operating System :: MacOS
-Classifier: Operating System :: POSIX :: Linux
-Classifier: Operating System :: Unix
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: License :: OSI Approved :: MIT License
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-Provides-Extra: test
-License-File: LICENSE
-
 <!--
     =====================================
     generator=datazen
-    version=3.1.2
-    hash=1280d00c2447ef272e48abbae9617e0a
+    version=3.1.3
+    hash=c704961deeb1f544c94a11a7582f58d4
     =====================================
 -->
 
-# vmklib ([1.9.0](https://pypi.org/project/vmklib/))
+# vmklib ([2.0.0](https://pypi.org/project/vmklib/))
 
 [![python](https://img.shields.io/pypi/pyversions/vmklib.svg)](https://pypi.org/project/vmklib/)
 ![Build Status](https://github.com/vkottler/vmklib/workflows/Python%20Package/badge.svg)
 [![codecov](https://codecov.io/gh/vkottler/vmklib/branch/master/graphs/badge.svg?branch=master)](https://codecov.io/github/vkottler/vmklib)
 ![PyPI - Status](https://img.shields.io/pypi/status/vmklib)
 ![Dependents (via libraries.io)](https://img.shields.io/librariesio/dependents/pypi/vmklib)
 
 *Simplify project workflows by standardizing use of GNU Make.*
 
-See also: [generated documentation](https://vkottler.github.io/python/pydoc/vmklib.html)
-(created with [`pydoc`](https://docs.python.org/3/library/pydoc.html)).
+## Documentation
+
+### Generated
+
+* By [sphinx-apidoc](https://vkottler.github.io/python/sphinx/vmklib)
+(What's [`sphinx-apidoc`](https://www.sphinx-doc.org/en/master/man/sphinx-apidoc.html)?)
+* By [pydoc](https://vkottler.github.io/python/pydoc/vmklib.html)
+(What's [`pydoc`](https://docs.python.org/3/library/pydoc.html)?)
 
 ## Python Version Support
 
 This package is tested with the following Python minor versions:
 
-* [`python3.8`](https://docs.python.org/3.8/)
-* [`python3.9`](https://docs.python.org/3.9/)
 * [`python3.10`](https://docs.python.org/3.10/)
 * [`python3.11`](https://docs.python.org/3.11/)
+* [`python3.12`](https://docs.python.org/3.12/)
 
 ## Platform Support
 
 This package is tested on the following platforms:
 
 * `ubuntu-latest`
 * `macos-latest`
@@ -109,27 +67,30 @@
 * [Dependency Graph](#dependency-graph)
 
 # Command-line Options
 
 ```
 $ ./venv3.11/bin/mk -h
 
-usage: mk [-h] [--version] [-v] [-C DIR] [-p PREFIX] [-d] [-D DEFAULT]
-          [-f FILE] [-c CONFIG] [-P PROJ]
+usage: mk [-h] [--version] [-v] [-q] [--curses] [--no-uvloop] [-C DIR]
+          [-p PREFIX] [-d] [-D DEFAULT] [-f FILE] [-c CONFIG] [-P PROJ]
           [targets ...]
 
 Simplify project workflows by standardizing use of GNU Make.
 
 positional arguments:
   targets               targets to execute
 
 options:
   -h, --help            show this help message and exit
   --version             show program's version number and exit
   -v, --verbose         set to increase logging verbosity
+  -q, --quiet           set to reduce output
+  --curses              whether or not to use curses.wrapper when starting
+  --no-uvloop           whether or not to disable uvloop as event loop driver
   -C DIR, --dir DIR     execute from a specific directory
   -p PREFIX, --prefix PREFIX
                         a prefix to apply to all targets
   -d, --disable-make    whether or not to allow GNU Make target resolution
                         (default: 'False')
   -D DEFAULT, --default DEFAULT
                         default target to make if none is specified (default:
```

### Comparing `vmklib-1.9.0/README.md` & `vmklib-2.0.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,36 +1,101 @@
+Metadata-Version: 2.1
+Name: vmklib
+Version: 2.0.0
+Summary: Simplify project workflows by standardizing use of GNU Make.
+Home-page: https://github.com/vkottler/vmklib
+Author: Vaughn Kottler
+Author-email: Vaughn Kottler <vaughnkottler@gmail.com>
+Maintainer-email: Vaughn Kottler <vaughnkottler@gmail.com>
+License: MIT License
+        
+        Copyright (c) 2023 Vaughn Kottler
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
+        
+Keywords: workflow,tool,make
+Classifier: Topic :: Software Development :: Build Tools
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Classifier: Operating System :: Microsoft :: Windows
+Classifier: Operating System :: MacOS
+Classifier: Operating System :: POSIX :: Linux
+Classifier: Operating System :: Unix
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: License :: OSI Approved :: MIT License
+Requires-Python: >=3.10
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: vcorelib>=2.4.0
+Provides-Extra: test
+Requires-Dist: pylint; extra == "test"
+Requires-Dist: flake8; extra == "test"
+Requires-Dist: black; extra == "test"
+Requires-Dist: ruff; extra == "test"
+Requires-Dist: mypy; extra == "test"
+Requires-Dist: isort; extra == "test"
+Requires-Dist: yamllint; extra == "test"
+Requires-Dist: yambs; extra == "test"
+Requires-Dist: vmklib; extra == "test"
+Requires-Dist: sphinx; extra == "test"
+Requires-Dist: sphinx-book-theme; extra == "test"
+Requires-Dist: pytest-asyncio; extra == "test"
+Requires-Dist: setuptools-wrapper; extra == "test"
+
 <!--
     =====================================
     generator=datazen
-    version=3.1.2
-    hash=1280d00c2447ef272e48abbae9617e0a
+    version=3.1.3
+    hash=c704961deeb1f544c94a11a7582f58d4
     =====================================
 -->
 
-# vmklib ([1.9.0](https://pypi.org/project/vmklib/))
+# vmklib ([2.0.0](https://pypi.org/project/vmklib/))
 
 [![python](https://img.shields.io/pypi/pyversions/vmklib.svg)](https://pypi.org/project/vmklib/)
 ![Build Status](https://github.com/vkottler/vmklib/workflows/Python%20Package/badge.svg)
 [![codecov](https://codecov.io/gh/vkottler/vmklib/branch/master/graphs/badge.svg?branch=master)](https://codecov.io/github/vkottler/vmklib)
 ![PyPI - Status](https://img.shields.io/pypi/status/vmklib)
 ![Dependents (via libraries.io)](https://img.shields.io/librariesio/dependents/pypi/vmklib)
 
 *Simplify project workflows by standardizing use of GNU Make.*
 
-See also: [generated documentation](https://vkottler.github.io/python/pydoc/vmklib.html)
-(created with [`pydoc`](https://docs.python.org/3/library/pydoc.html)).
+## Documentation
+
+### Generated
+
+* By [sphinx-apidoc](https://vkottler.github.io/python/sphinx/vmklib)
+(What's [`sphinx-apidoc`](https://www.sphinx-doc.org/en/master/man/sphinx-apidoc.html)?)
+* By [pydoc](https://vkottler.github.io/python/pydoc/vmklib.html)
+(What's [`pydoc`](https://docs.python.org/3/library/pydoc.html)?)
 
 ## Python Version Support
 
 This package is tested with the following Python minor versions:
 
-* [`python3.8`](https://docs.python.org/3.8/)
-* [`python3.9`](https://docs.python.org/3.9/)
 * [`python3.10`](https://docs.python.org/3.10/)
 * [`python3.11`](https://docs.python.org/3.11/)
+* [`python3.12`](https://docs.python.org/3.12/)
 
 ## Platform Support
 
 This package is tested on the following platforms:
 
 * `ubuntu-latest`
 * `macos-latest`
@@ -62,27 +127,30 @@
 * [Dependency Graph](#dependency-graph)
 
 # Command-line Options
 
 ```
 $ ./venv3.11/bin/mk -h
 
-usage: mk [-h] [--version] [-v] [-C DIR] [-p PREFIX] [-d] [-D DEFAULT]
-          [-f FILE] [-c CONFIG] [-P PROJ]
+usage: mk [-h] [--version] [-v] [-q] [--curses] [--no-uvloop] [-C DIR]
+          [-p PREFIX] [-d] [-D DEFAULT] [-f FILE] [-c CONFIG] [-P PROJ]
           [targets ...]
 
 Simplify project workflows by standardizing use of GNU Make.
 
 positional arguments:
   targets               targets to execute
 
 options:
   -h, --help            show this help message and exit
   --version             show program's version number and exit
   -v, --verbose         set to increase logging verbosity
+  -q, --quiet           set to reduce output
+  --curses              whether or not to use curses.wrapper when starting
+  --no-uvloop           whether or not to disable uvloop as event loop driver
   -C DIR, --dir DIR     execute from a specific directory
   -p PREFIX, --prefix PREFIX
                         a prefix to apply to all targets
   -d, --disable-make    whether or not to allow GNU Make target resolution
                         (default: 'False')
   -D DEFAULT, --default DEFAULT
                         default target to make if none is specified (default:
```

### Comparing `vmklib-1.9.0/pyproject.toml` & `vmklib-2.0.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,35 +1,34 @@
 [build-system]
 requires = ["setuptools-wrapper", "trove-classifiers"]
 build-backend = "setuptools.build_meta:__legacy__"
 
 [project]
 name = "vmklib"
-version = "1.9.0"
+version = "2.0.0"
 description = "Simplify project workflows by standardizing use of GNU Make."
 readme = "README.md"
-requires-python = ">=3.8"
+requires-python = ">=3.10"
 license = {file = "LICENSE"}
 keywords = [
   "workflow",
   "tool",
   "make"
 ]
 authors = [
   {name = "Vaughn Kottler", email = "vaughnkottler@gmail.com"}
 ]
 maintainers = [
   {name = "Vaughn Kottler", email = "vaughnkottler@gmail.com"}
 ]
 classifiers = [
   "Topic :: Software Development :: Build Tools",
-  "Programming Language :: Python :: 3.8",
-  "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
+  "Programming Language :: Python :: 3.12",
   "Operating System :: Microsoft :: Windows",
   "Operating System :: MacOS",
   "Operating System :: POSIX :: Linux",
   "Operating System :: Unix",
   "Development Status :: 5 - Production/Stable",
   "License :: OSI Approved :: MIT License"
 ]
@@ -40,13 +39,17 @@
   "pylint",
   "flake8",
   "black",
   "ruff",
   "mypy",
   "isort",
   "yamllint",
+  "yambs",
+  "vmklib",
+  "sphinx",
+  "sphinx-book-theme",
   "pytest-asyncio",
   "setuptools-wrapper"
 ]
 
 [project.scripts]
 mk = "vmklib.entry:main"
```

### Comparing `vmklib-1.9.0/setup.py` & `vmklib-2.0.0/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # =====================================
 # generator=datazen
-# version=3.1.2
-# hash=c29553a5eb8c58f39d08f72dfa51d217
+# version=3.1.3
+# hash=43286ed57052c2548361d2dcdd062187
 # =====================================
 
 """
 vmklib - Package definition for distribution.
 """
 
 # third-party
@@ -24,17 +24,16 @@
 }
 pkg_info = {
     "name": PKG_NAME,
     "slug": PKG_NAME.replace("-", "_"),
     "version": VERSION,
     "description": DESCRIPTION,
     "versions": [
-        "3.8",
-        "3.9",
         "3.10",
         "3.11",
+        "3.12",
     ],
 }
 setup(
     pkg_info,
     author_info,
 )
```

### Comparing `vmklib-1.9.0/tests/test_entry.py` & `vmklib-2.0.0/tests/test_entry.py`

 * *Files identical despite different names*

### Comparing `vmklib-1.9.0/vmklib/app.py` & `vmklib-2.0.0/vmklib/app.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,21 +13,21 @@
 import subprocess
 import tempfile
 from typing import Callable, Dict, Iterator, List, Optional, Tuple, cast
 
 # third-party
 from vcorelib.dict import GenericStrDict
 from vcorelib.io import ARBITER
+from vcorelib.paths import find_file
 from vcorelib.target import Substitutions
 from vcorelib.task import TaskFailed
 from vcorelib.task.manager import TaskManager
 
 # internal
 from vmklib import PKG_NAME
-from vmklib.resources import get_resource
 
 LOG = logging.getLogger(__name__)
 DEFAULT_FILE = Path("Makefile")
 
 
 def project(path: Path, name: str = None) -> str:
     """
@@ -61,15 +61,15 @@
         data["$(PROJ)_DIR"] = cast(str, directory)
         data["MK_AUTO"] = 1
         data["$(PROJ)_MK_DIR"] = os.path.join(str(data["$(PROJ)_DIR"]), "mk")
 
         # get the path to this package's data to include our "conf.mk"
         include_strs = [
             "-include $($(PROJ)_MK_DIR)/init.mk",
-            f"include {get_resource('conf.mk')}",
+            f"include {find_file('conf.mk', package=PKG_NAME)}",
             "-include $($(PROJ)_MK_DIR)/conf.mk",
         ]
 
         for key, item in data.items():
             makefile.write(f"{key} := {item}")
             makefile.write(os.linesep)
         for line in include_strs:
@@ -102,20 +102,18 @@
     task_register: str,
     directory: Path,
     substitutions: Substitutions,
 ) -> None:
     """Load internal and external tasks to the task manager."""
 
     # register task-manager targets from this package
+    conf = find_file("lib_tasks", "conf.py", package=PKG_NAME)
+    assert conf is not None
     assert manager.script(
-        get_resource(os.path.join("lib_tasks", "conf.py")),
-        "register",
-        proj,
-        directory,
-        substitutions,
+        conf, "register", proj, directory, substitutions
     ), "Couldn't register package tasks from '{get_resource(task_register)}'!"
 
     # register task-manager targets for the project
     proj_tasks = directory.joinpath(task_register)
     if proj_tasks.is_file():
         assert manager.script(
             proj_tasks,
@@ -163,15 +161,15 @@
 def entry(args: argparse.Namespace) -> int:
     """Execute the requested task."""
 
     if not args.file.is_file():
         if args.file.name != str(DEFAULT_FILE):
             LOG.error("'%s' not found", args.file)
             return 1
-        args.file = get_resource(os.path.join("data", "header.mk"))
+        args.file = find_file("data", "header.mk", package=PKG_NAME)
 
     # Add the default target early if nothing was specified.
     if not args.targets and args.default:
         args.targets.append(args.default)
 
     # load configuration data, if configuration data is found
     substitutions, targets = get_data(args.config, args.targets, args.prefix)
```

### Comparing `vmklib-1.9.0/vmklib/data/conf.mk` & `vmklib-2.0.0/vmklib/data/conf.mk`

 * *Files identical despite different names*

### Comparing `vmklib-1.9.0/vmklib/data/data/header.mk` & `vmklib-2.0.0/vmklib/data/data/header.mk`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # =====================================
 # generator=datazen
-# version=3.1.2
+# version=3.1.3
 # hash=22a8a762623587d443724e0f1a2a9ee4
 # =====================================
 ###############################################################################
 MK_INFO := https://pypi.org/project/vmklib
 ifeq (,$(shell which mk))
 $(warning "No 'mk' in $(PATH), install 'vmklib' with 'pip' ($(MK_INFO))")
 endif
```

### Comparing `vmklib-1.9.0/vmklib/data/datazen.mk` & `vmklib-2.0.0/vmklib/data/datazen.mk`

 * *Files identical despite different names*

### Comparing `vmklib-1.9.0/vmklib/data/functions.mk` & `vmklib-2.0.0/vmklib/data/functions.mk`

 * *Files identical despite different names*

### Comparing `vmklib-1.9.0/vmklib/data/grip.mk` & `vmklib-2.0.0/vmklib/data/grip.mk`

 * *Files identical despite different names*

### Comparing `vmklib-1.9.0/vmklib/data/lib_tasks/__pycache__/conf.cpython-311.pyc` & `vmklib-2.0.0/vmklib/data/lib_tasks/__pycache__/conf.cpython-311.pyc`

 * *Files 6% similar despite different names*

#### Python bytecode

```diff
@@ -1,26 +1,26 @@
 magic:    0xa70d0d0a
-moddate:  0x6b1faf64 (Wed Jul 12 21:47:23 2023 UTC)
-files sz: 2374
+moddate:  0x1c071f65 (Thu Oct  5 18:57:32 2023 UTC)
+files sz: 2483
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 10
    flags     : 0
    code
       0x970064005a00640164026c016d025a020100640164036c036d045a0401
       00640164046c056d065a066d075a076d085a080100640164056c096d0a5a
       0a0100640164066c0b6d0c5a0c0100640164076c0d6d0e5a0f0100640164
       086c106d115a116d125a120100640164076c136d0e5a140100640164076c
       156d0e5a160100640164076c176d0e5a180100640164076c196d0e5a1a01
       00640164076c1b6d0e5a1c0100640164076c1d6d0e5a1e0100640164076c
       1f6d0e5a200100640164076c216d0e5a220100640164076c236d0e5a2401
-      000200470064098400640a6508a6030000ab0300000000000000005a2564
-      0b650c640c6526640d6502640e6504652665266602190000000000000000
-      00640f6527660a641084045a0e64115300
+      00640164076c256d0e5a2601000200470064098400640a6508a6030000ab
+      0300000000000000005a27640b650c640c6528640d6502640e6504652865
+      28660219000000000000000000640f6529660a641084045a0e64115300
      0           0 RESUME                   0
    
      1           2 LOAD_CONST               0 ('\nA module for registering package tasks.\n')
                  4 STORE_NAME               0 (__doc__)
    
      6           6 LOAD_CONST               1 (0)
                  8 LOAD_CONST               2 (('Path',))
@@ -110,80 +110,87 @@
                154 IMPORT_NAME             27 (vmklib.tasks.python.package)
                156 IMPORT_FROM             14 (register)
                158 STORE_NAME              28 (register_python_package)
                160 POP_TOP
    
     22         162 LOAD_CONST               1 (0)
                164 LOAD_CONST               7 (('register',))
-               166 IMPORT_NAME             29 (vmklib.tasks.python.sa)
+               166 IMPORT_NAME             29 (vmklib.tasks.python.release)
                168 IMPORT_FROM             14 (register)
-               170 STORE_NAME              30 (register_python_sa)
+               170 STORE_NAME              30 (register_python_release)
                172 POP_TOP
    
     23         174 LOAD_CONST               1 (0)
                176 LOAD_CONST               7 (('register',))
-               178 IMPORT_NAME             31 (vmklib.tasks.python.test)
+               178 IMPORT_NAME             31 (vmklib.tasks.python.sa)
                180 IMPORT_FROM             14 (register)
-               182 STORE_NAME              32 (register_python_test)
+               182 STORE_NAME              32 (register_python_sa)
                184 POP_TOP
    
     24         186 LOAD_CONST               1 (0)
                188 LOAD_CONST               7 (('register',))
-               190 IMPORT_NAME             33 (vmklib.tasks.python.yaml)
+               190 IMPORT_NAME             33 (vmklib.tasks.python.test)
                192 IMPORT_FROM             14 (register)
-               194 STORE_NAME              34 (register_python_yaml)
+               194 STORE_NAME              34 (register_python_test)
                196 POP_TOP
    
     25         198 LOAD_CONST               1 (0)
                200 LOAD_CONST               7 (('register',))
-               202 IMPORT_NAME             35 (vmklib.tasks.venv)
+               202 IMPORT_NAME             35 (vmklib.tasks.python.yaml)
                204 IMPORT_FROM             14 (register)
-               206 STORE_NAME              36 (register_venv)
+               206 STORE_NAME              36 (register_python_yaml)
                208 POP_TOP
    
-    28         210 PUSH_NULL
-               212 LOAD_BUILD_CLASS
-               214 LOAD_CONST               9 (<code object FailTask, file "/home/runner/work/vmklib/vmklib/vmklib/data/lib_tasks/conf.py", line 28>)
-               216 MAKE_FUNCTION            0
-               218 LOAD_CONST              10 ('FailTask')
-               220 LOAD_NAME                8 (Task)
-               222 PRECALL                  3
-               226 CALL                     3
-               236 STORE_NAME              37 (FailTask)
+    26         210 LOAD_CONST               1 (0)
+               212 LOAD_CONST               7 (('register',))
+               214 IMPORT_NAME             37 (vmklib.tasks.venv)
+               216 IMPORT_FROM             14 (register)
+               218 STORE_NAME              38 (register_venv)
+               220 POP_TOP
    
-    35         238 LOAD_CONST              11 ('manager')
+    29         222 PUSH_NULL
+               224 LOAD_BUILD_CLASS
+               226 LOAD_CONST               9 (<code object FailTask, file "/home/runner/work/vmklib/vmklib/vmklib/data/lib_tasks/conf.py", line 29>)
+               228 MAKE_FUNCTION            0
+               230 LOAD_CONST              10 ('FailTask')
+               232 LOAD_NAME                8 (Task)
+               234 PRECALL                  3
+               238 CALL                     3
+               248 STORE_NAME              39 (FailTask)
    
-    36         240 LOAD_NAME               12 (TaskManager)
+    36         250 LOAD_CONST              11 ('manager')
    
-    35         242 LOAD_CONST              12 ('project')
+    37         252 LOAD_NAME               12 (TaskManager)
    
-    37         244 LOAD_NAME               38 (str)
+    36         254 LOAD_CONST              12 ('project')
    
-    35         246 LOAD_CONST              13 ('cwd')
+    38         256 LOAD_NAME               40 (str)
    
-    38         248 LOAD_NAME                2 (Path)
+    36         258 LOAD_CONST              13 ('cwd')
    
-    35         250 LOAD_CONST              14 ('substitutions')
+    39         260 LOAD_NAME                2 (Path)
    
-    39         252 LOAD_NAME                4 (Dict)
-               254 LOAD_NAME               38 (str)
-               256 LOAD_NAME               38 (str)
-               258 BUILD_TUPLE              2
-               260 BINARY_SUBSCR
+    36         262 LOAD_CONST              14 ('substitutions')
    
-    35         270 LOAD_CONST              15 ('return')
+    40         264 LOAD_NAME                4 (Dict)
+               266 LOAD_NAME               40 (str)
+               268 LOAD_NAME               40 (str)
+               270 BUILD_TUPLE              2
+               272 BINARY_SUBSCR
    
-    40         272 LOAD_NAME               39 (bool)
+    36         282 LOAD_CONST              15 ('return')
    
-    35         274 BUILD_TUPLE             10
-               276 LOAD_CONST              16 (<code object register, file "/home/runner/work/vmklib/vmklib/vmklib/data/lib_tasks/conf.py", line 35>)
-               278 MAKE_FUNCTION            4 (annotations)
-               280 STORE_NAME              14 (register)
-               282 LOAD_CONST              17 (None)
-               284 RETURN_VALUE
+    41         284 LOAD_NAME               41 (bool)
+   
+    36         286 BUILD_TUPLE             10
+               288 LOAD_CONST              16 (<code object register, file "/home/runner/work/vmklib/vmklib/vmklib/data/lib_tasks/conf.py", line 36>)
+               290 MAKE_FUNCTION            4 (annotations)
+               292 STORE_NAME              14 (register)
+               294 LOAD_CONST              17 (None)
+               296 RETURN_VALUE
    consts
       '\nA module for registering package tasks.\n'
       0
       ('Path',)
       ('Dict',)
       ('Inbox', 'Outbox', 'Task')
       ('DictMerger',)
@@ -194,31 +201,31 @@
          argcount  : 0
          nlocals   : 0
          stacksize : 6
          flags     : 0
          code
             0x970065005a0164005a0264015a03640265046403650564046506660664
             0584045a0764065300
-          28           0 RESUME                   0
+          29           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('FailTask')
                        8 STORE_NAME               2 (__qualname__)
          
-          29          10 LOAD_CONST               1 ('A task that always fails.')
+          30          10 LOAD_CONST               1 ('A task that always fails.')
                       12 STORE_NAME               3 (__doc__)
          
-          31          14 LOAD_CONST               2 ('inbox')
+          32          14 LOAD_CONST               2 ('inbox')
                       16 LOAD_NAME                4 (Inbox)
                       18 LOAD_CONST               3 ('outbox')
                       20 LOAD_NAME                5 (Outbox)
                       22 LOAD_CONST               4 ('return')
                       24 LOAD_NAME                6 (bool)
                       26 BUILD_TUPLE              6
-                      28 LOAD_CONST               5 (<code object run, file "/home/runner/work/vmklib/vmklib/vmklib/data/lib_tasks/conf.py", line 31>)
+                      28 LOAD_CONST               5 (<code object run, file "/home/runner/work/vmklib/vmklib/vmklib/data/lib_tasks/conf.py", line 32>)
                       30 MAKE_FUNCTION            4 (annotations)
                       32 STORE_NAME               7 (run)
                       34 LOAD_CONST               6 (None)
                       36 RETURN_VALUE
          consts
             'FailTask'
             'A task that always fails.'
@@ -227,50 +234,50 @@
             'return'
             code
                argcount  : 3
                nlocals   : 5
                stacksize : 1
                flags     : 143
                code 0x4b000100970064015300
-                31           0 RETURN_GENERATOR
+                32           0 RETURN_GENERATOR
                              2 POP_TOP
                              4 RESUME                   0
                
-                32           6 LOAD_CONST               1 (False)
+                33           6 LOAD_CONST               1 (False)
                              8 RETURN_VALUE
                consts
                   None
                   False
                names      ()
                varnames   ('self', 'inbox', 'outbox', 'args', 'kwargs')
                freevars   ()
                cellvars   ()
                filename   '/home/runner/work/vmklib/vmklib/vmklib/data/lib_tasks/conf.py'
                name       'run'
-               firstlineno 31
+               firstlineno 32
                lnotab 0x0601
             None
          names      ('__name__', '__module__', '__qualname__', '__doc__', 'Inbox', 'Outbox', 'bool', 'run')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   '/home/runner/work/vmklib/vmklib/vmklib/data/lib_tasks/conf.py'
          name       'FailTask'
-         firstlineno 28
+         firstlineno 29
          lnotab 0x0a010402
       'FailTask'
       'manager'
       'project'
       'cwd'
       'substitutions'
       'return'
       code
          argcount  : 4
          nlocals   : 7
-         stacksize : 10
+         stacksize : 11
          flags     : 3
          code
             0x97007c02a00000000000000000000000000000000000000000006401a6
             010000ab0100000000000000007403000000000000000000007c02a60100
             00ab0100000000000000007405000000000000000000007c02a6010000ab
             0100000000000000007c02a0000000000000000000000000000000000000
             0000007c01a6010000ab01000000000000000064029c0464037405000000
@@ -279,146 +286,148 @@
             0000000000000000006405a6010000ab010000000000000000a6010000ab
             01000000000000000001007c00a003000000000000000000000000000000
             0000000000740b0000000000000000000064067c047c03a6030000ab0300
             00000000000000a6010000ab010000000000000000010064077d05740c00
             000000000000000000740e00000000000000000000741000000000000000
             000000741200000000000000000000741400000000000000000000741600
             000000000000000000741800000000000000000000741a00000000000000
-            000000741c00000000000000000000741e00000000000000000000660a44
-            005d127d067c05720e02007c067c007c017c027c03a6040000ab04000000
-            00000000007d058c137c055300
-          35           0 RESUME                   0
+            000000741c00000000000000000000741e00000000000000000000742000
+            000000000000000000660b44005d127d067c05720e02007c067c007c017c
+            027c03a6040000ab0400000000000000007d058c137c055300
+          36           0 RESUME                   0
          
-          47           2 LOAD_FAST                2 (cwd)
+          48           2 LOAD_FAST                2 (cwd)
                        4 LOAD_METHOD              0 (joinpath)
                       26 LOAD_CONST               1 ('build')
                       28 PRECALL                  1
                       32 CALL                     1
          
-          48          42 LOAD_GLOBAL              3 (NULL + venv_dir)
+          49          42 LOAD_GLOBAL              3 (NULL + venv_dir)
                       54 LOAD_FAST                2 (cwd)
                       56 PRECALL                  1
                       60 CALL                     1
          
-          49          70 LOAD_GLOBAL              5 (NULL + venv_bin)
+          50          70 LOAD_GLOBAL              5 (NULL + venv_bin)
                       82 LOAD_FAST                2 (cwd)
                       84 PRECALL                  1
                       88 CALL                     1
          
-          50          98 LOAD_FAST                2 (cwd)
+          51          98 LOAD_FAST                2 (cwd)
                      100 LOAD_METHOD              0 (joinpath)
                      122 LOAD_FAST                1 (project)
                      124 PRECALL                  1
                      128 CALL                     1
          
-          46         138 LOAD_CONST               2 (('build', 'venv', 'venv_bin', 'proj'))
+          47         138 LOAD_CONST               2 (('build', 'venv', 'venv_bin', 'proj'))
                      140 BUILD_CONST_KEY_MAP      4
          
-          52         142 LOAD_CONST               3 ('python')
+          53         142 LOAD_CONST               3 ('python')
                      144 LOAD_GLOBAL              5 (NULL + venv_bin)
                      156 LOAD_FAST                2 (cwd)
                      158 LOAD_CONST               3 ('python')
                      160 PRECALL                  2
                      164 CALL                     2
                      174 BUILD_MAP                1
          
-          45         176 LOAD_CONST               4 (('__dirs__', '__files__'))
+          46         176 LOAD_CONST               4 (('__dirs__', '__files__'))
                      178 BUILD_CONST_KEY_MAP      2
                      180 STORE_FAST               4 (init_data)
          
-          56         182 LOAD_FAST                0 (manager)
+          57         182 LOAD_FAST                0 (manager)
                      184 LOAD_METHOD              3 (register)
                      206 LOAD_GLOBAL              9 (NULL + FailTask)
                      218 LOAD_CONST               5 ('fail')
                      220 PRECALL                  1
                      224 CALL                     1
                      234 PRECALL                  1
                      238 CALL                     1
                      248 POP_TOP
          
-          59         250 LOAD_FAST                0 (manager)
+          60         250 LOAD_FAST                0 (manager)
                      252 LOAD_METHOD              3 (register)
                      274 LOAD_GLOBAL             11 (NULL + DictMerger)
                      286 LOAD_CONST               6 ('vmklib.init')
                      288 LOAD_FAST                4 (init_data)
                      290 LOAD_FAST                3 (substitutions)
                      292 PRECALL                  3
                      296 CALL                     3
                      306 PRECALL                  1
                      310 CALL                     1
                      320 POP_TOP
          
-          62         322 LOAD_CONST               7 (True)
+          63         322 LOAD_CONST               7 (True)
                      324 STORE_FAST               5 (result)
          
-          64         326 LOAD_GLOBAL             12 (register_venv)
+          65         326 LOAD_GLOBAL             12 (register_venv)
+         
+          66         338 LOAD_GLOBAL             14 (register_python_lint)
          
-          65         338 LOAD_GLOBAL             14 (register_python_lint)
+          67         350 LOAD_GLOBAL             16 (register_python_package)
          
-          66         350 LOAD_GLOBAL             16 (register_python_package)
+          68         362 LOAD_GLOBAL             18 (register_python_yaml)
          
-          67         362 LOAD_GLOBAL             18 (register_python_yaml)
+          69         374 LOAD_GLOBAL             20 (register_python_build)
          
-          68         374 LOAD_GLOBAL             20 (register_python_build)
+          70         386 LOAD_GLOBAL             22 (register_python_sa)
          
-          69         386 LOAD_GLOBAL             22 (register_python_sa)
+          71         398 LOAD_GLOBAL             24 (register_python_test)
          
-          70         398 LOAD_GLOBAL             24 (register_python_test)
+          72         410 LOAD_GLOBAL             26 (register_datazen)
          
-          71         410 LOAD_GLOBAL             26 (register_datazen)
+          73         422 LOAD_GLOBAL             28 (register_python_docs)
          
-          72         422 LOAD_GLOBAL             28 (register_python_docs)
+          74         434 LOAD_GLOBAL             30 (register_python_release)
          
-          73         434 LOAD_GLOBAL             30 (register_node)
+          75         446 LOAD_GLOBAL             32 (register_node)
          
-          63         446 BUILD_TUPLE             10
-                     448 GET_ITER
-                 >>  450 FOR_ITER                18 (to 488)
-                     452 STORE_FAST               6 (dep)
+          64         458 BUILD_TUPLE             11
+                     460 GET_ITER
+                 >>  462 FOR_ITER                18 (to 500)
+                     464 STORE_FAST               6 (dep)
          
-          75         454 LOAD_FAST                5 (result)
-                     456 POP_JUMP_FORWARD_IF_FALSE    14 (to 486)
+          77         466 LOAD_FAST                5 (result)
+                     468 POP_JUMP_FORWARD_IF_FALSE    14 (to 498)
          
-          76         458 PUSH_NULL
-                     460 LOAD_FAST                6 (dep)
-                     462 LOAD_FAST                0 (manager)
-                     464 LOAD_FAST                1 (project)
-                     466 LOAD_FAST                2 (cwd)
-                     468 LOAD_FAST                3 (substitutions)
-                     470 PRECALL                  4
-                     474 CALL                     4
-                     484 STORE_FAST               5 (result)
-                 >>  486 JUMP_BACKWARD           19 (to 450)
+          78         470 PUSH_NULL
+                     472 LOAD_FAST                6 (dep)
+                     474 LOAD_FAST                0 (manager)
+                     476 LOAD_FAST                1 (project)
+                     478 LOAD_FAST                2 (cwd)
+                     480 LOAD_FAST                3 (substitutions)
+                     482 PRECALL                  4
+                     486 CALL                     4
+                     496 STORE_FAST               5 (result)
+                 >>  498 JUMP_BACKWARD           19 (to 462)
          
-          78     >>  488 LOAD_FAST                5 (result)
-                     490 RETURN_VALUE
+          80     >>  500 LOAD_FAST                5 (result)
+                     502 RETURN_VALUE
          consts
             'Register package tasks to the manager.'
             'build'
             ('build', 'venv', 'venv_bin', 'proj')
             'python'
             ('__dirs__', '__files__')
             'fail'
             'vmklib.init'
             True
-         names      ('joinpath', 'venv_dir', 'venv_bin', 'register', 'FailTask', 'DictMerger', 'register_venv', 'register_python_lint', 'register_python_package', 'register_python_yaml', 'register_python_build', 'register_python_sa', 'register_python_test', 'register_datazen', 'register_python_docs', 'register_node')
+         names      ('joinpath', 'venv_dir', 'venv_bin', 'register', 'FailTask', 'DictMerger', 'register_venv', 'register_python_lint', 'register_python_package', 'register_python_yaml', 'register_python_build', 'register_python_sa', 'register_python_test', 'register_datazen', 'register_python_docs', 'register_python_release', 'register_node')
          varnames   ('manager', 'project', 'cwd', 'substitutions', 'init_data', 'result', 'dep')
          freevars   ()
          cellvars   ()
          filename   '/home/runner/work/vmklib/vmklib/vmklib/data/lib_tasks/conf.py'
          name       'register'
-         firstlineno 35
+         firstlineno 36
          lnotab
             0x020c28011c011c0128fc040622f9060b4403480304020c010c010c010c
-            010c010c010c010c010c010cf6080c04011e02
+            010c010c010c010c010c010c010cf5080d04011e02
       None
-   names      ('__doc__', 'pathlib', 'Path', 'typing', 'Dict', 'vcorelib.task', 'Inbox', 'Outbox', 'Task', 'vcorelib.task.dict.melder', 'DictMerger', 'vcorelib.task.manager', 'TaskManager', 'vmklib.tasks.node', 'register', 'register_node', 'vmklib.tasks.python', 'venv_bin', 'venv_dir', 'vmklib.tasks.python.build', 'register_python_build', 'vmklib.tasks.python.datazen', 'register_datazen', 'vmklib.tasks.python.docs', 'register_python_docs', 'vmklib.tasks.python.lint', 'register_python_lint', 'vmklib.tasks.python.package', 'register_python_package', 'vmklib.tasks.python.sa', 'register_python_sa', 'vmklib.tasks.python.test', 'register_python_test', 'vmklib.tasks.python.yaml', 'register_python_yaml', 'vmklib.tasks.venv', 'register_venv', 'FailTask', 'str', 'bool')
+   names      ('__doc__', 'pathlib', 'Path', 'typing', 'Dict', 'vcorelib.task', 'Inbox', 'Outbox', 'Task', 'vcorelib.task.dict.melder', 'DictMerger', 'vcorelib.task.manager', 'TaskManager', 'vmklib.tasks.node', 'register', 'register_node', 'vmklib.tasks.python', 'venv_bin', 'venv_dir', 'vmklib.tasks.python.build', 'register_python_build', 'vmklib.tasks.python.datazen', 'register_datazen', 'vmklib.tasks.python.docs', 'register_python_docs', 'vmklib.tasks.python.lint', 'register_python_lint', 'vmklib.tasks.python.package', 'register_python_package', 'vmklib.tasks.python.release', 'register_python_release', 'vmklib.tasks.python.sa', 'register_python_sa', 'vmklib.tasks.python.test', 'register_python_test', 'vmklib.tasks.python.yaml', 'register_python_yaml', 'vmklib.tasks.venv', 'register_venv', 'FailTask', 'str', 'bool')
    varnames   ()
    freevars   ()
    cellvars   ()
    filename   '/home/runner/work/vmklib/vmklib/vmklib/data/lib_tasks/conf.py'
    name       '<module>'
    firstlineno 1
    lnotab
       0x00ff020104050c010c0314010c010c030c0110010c010c010c010c010c
-      010c010c010c010c031c07020102ff020202fe020302fd020412fc020502
-      fb
+      010c010c010c010c010c031c07020102ff020202fe020302fd020412fc02
+      0502fb
```

### Comparing `vmklib-1.9.0/vmklib/data/lib_tasks/conf.py` & `vmklib-2.0.0/vmklib/data/lib_tasks/conf.py`

 * *Files 9% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 from vmklib.tasks.node import register as register_node
 from vmklib.tasks.python import venv_bin, venv_dir
 from vmklib.tasks.python.build import register as register_python_build
 from vmklib.tasks.python.datazen import register as register_datazen
 from vmklib.tasks.python.docs import register as register_python_docs
 from vmklib.tasks.python.lint import register as register_python_lint
 from vmklib.tasks.python.package import register as register_python_package
+from vmklib.tasks.python.release import register as register_python_release
 from vmklib.tasks.python.sa import register as register_python_sa
 from vmklib.tasks.python.test import register as register_python_test
 from vmklib.tasks.python.yaml import register as register_python_yaml
 from vmklib.tasks.venv import register as register_venv
 
 
 class FailTask(Task):
@@ -66,13 +67,14 @@
         register_python_package,
         register_python_yaml,
         register_python_build,
         register_python_sa,
         register_python_test,
         register_datazen,
         register_python_docs,
+        register_python_release,
         register_node,
     ]:
         if result:
             result = dep(manager, project, cwd, substitutions)
 
     return result
```

### Comparing `vmklib-1.9.0/vmklib/data/python/build.mk` & `vmklib-2.0.0/vmklib/data/python/build.mk`

 * *Files identical despite different names*

### Comparing `vmklib-1.9.0/vmklib/data/python/docs.mk` & `vmklib-2.0.0/vmklib/data/python/docs.mk`

 * *Files identical despite different names*

### Comparing `vmklib-1.9.0/vmklib/data/python/pypi.mk` & `vmklib-2.0.0/vmklib/data/python/pypi.mk`

 * *Files identical despite different names*

### Comparing `vmklib-1.9.0/vmklib/data/python/upload.mk` & `vmklib-2.0.0/vmklib/data/python/upload.mk`

 * *Files identical despite different names*

### Comparing `vmklib-1.9.0/vmklib/data/python.mk` & `vmklib-2.0.0/vmklib/data/python.mk`

 * *Files identical despite different names*

### Comparing `vmklib-1.9.0/vmklib/data/time.mk` & `vmklib-2.0.0/vmklib/data/time.mk`

 * *Files identical despite different names*

### Comparing `vmklib-1.9.0/vmklib/data/venv.mk` & `vmklib-2.0.0/vmklib/data/venv.mk`

 * *Files identical despite different names*

### Comparing `vmklib-1.9.0/vmklib/data/vmklib.mk` & `vmklib-2.0.0/vmklib/data/vmklib.mk`

 * *Files identical despite different names*

### Comparing `vmklib-1.9.0/vmklib/entry.py` & `vmklib-2.0.0/vmklib/entry.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 # =====================================
 # generator=datazen
-# version=3.1.2
-# hash=334b3aaa0057809fb4013ea7760483a9
+# version=3.1.3
+# hash=745689313e0947f30ccf35892bb72cd4
 # =====================================
 
 """
 This package's command-line entry-point (boilerplate).
 """
 
 # built-in
 import argparse
-import logging
 import os
 from pathlib import Path
 import sys
 from typing import List
 
+# third-party
+from vcorelib.logging import init_logging, logging_args
+
 # internal
 from vmklib import DESCRIPTION, VERSION
 from vmklib.app import add_app_args, entry
 
 
 def main(argv: List[str] = None) -> int:
     """Program entry-point."""
@@ -34,20 +36,15 @@
     # initialize argument parsing
     parser = argparse.ArgumentParser(description=DESCRIPTION)
     parser.add_argument(
         "--version",
         action="version",
         version=f"%(prog)s {VERSION}",
     )
-    parser.add_argument(
-        "-v",
-        "--verbose",
-        action="store_true",
-        help="set to increase logging verbosity",
-    )
+    logging_args(parser)
     parser.add_argument(
         "-C",
         "--dir",
         default=Path.cwd(),
         dest="dir",
         type=Path,
         help="execute from a specific directory",
@@ -59,18 +56,16 @@
     # parse arguments and execute the requested command
     try:
         args = parser.parse_args(command_args[1:])
         args.version = VERSION
         args.dir = args.dir.resolve()
 
         # initialize logging
-        log_level = logging.DEBUG if args.verbose else logging.INFO
-        logging.basicConfig(
-            level=log_level,
-            format="%(name)-36s - %(levelname)-6s - %(message)s",
+        init_logging(
+            args, default_format="%(name)-36s - %(levelname)-6s - %(message)s"
         )
 
         # change to the specified directory
         os.chdir(args.dir)
 
         # run the application
         result = entry(args)
```

### Comparing `vmklib-1.9.0/vmklib/tasks/args.py` & `vmklib-2.0.0/vmklib/tasks/args.py`

 * *Files identical despite different names*

### Comparing `vmklib-1.9.0/vmklib/tasks/clean.py` & `vmklib-2.0.0/vmklib/tasks/clean.py`

 * *Files identical despite different names*

### Comparing `vmklib-1.9.0/vmklib/tasks/github.py` & `vmklib-2.0.0/vmklib/tasks/github.py`

 * *Files identical despite different names*

### Comparing `vmklib-1.9.0/vmklib/tasks/mixins/concrete.py` & `vmklib-2.0.0/vmklib/tasks/mixins/concrete.py`

 * *Files identical despite different names*

### Comparing `vmklib-1.9.0/vmklib/tasks/mixins/curl.py` & `vmklib-2.0.0/vmklib/tasks/mixins/curl.py`

 * *Files identical despite different names*

### Comparing `vmklib-1.9.0/vmklib/tasks/node/__init__.py` & `vmklib-2.0.0/vmklib/tasks/node/__init__.py`

 * *Files identical despite different names*

### Comparing `vmklib-1.9.0/vmklib/tasks/python/build.py` & `vmklib-2.0.0/vmklib/tasks/python/build.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,19 +10,19 @@
 # third-party
 from vcorelib.task import Inbox, Outbox
 from vcorelib.task.manager import TaskManager
 from vcorelib.task.subprocess.run import SubprocessLogMixin
 
 # internal
 from vmklib.tasks.args import environ_fallback_split
-from vmklib.tasks.mixins.concrete import ConcreteBuilderMixin
+from vmklib.tasks.mixins.concrete import ConcreteOnceMixin
 from vmklib.tasks.python import PREFIX
 
 
-class PythonBuild(ConcreteBuilderMixin, SubprocessLogMixin):
+class PythonBuild(ConcreteOnceMixin, SubprocessLogMixin):
     """Build a Python package."""
 
     async def run(
         self,
         inbox: Inbox,
         outbox: Outbox,
         *args,
```

### Comparing `vmklib-1.9.0/vmklib/tasks/python/datazen.py` & `vmklib-2.0.0/vmklib/tasks/python/datazen.py`

 * *Files identical despite different names*

### Comparing `vmklib-1.9.0/vmklib/tasks/python/docs.py` & `vmklib-2.0.0/vmklib/tasks/python/docs.py`

 * *Files identical despite different names*

### Comparing `vmklib-1.9.0/vmklib/tasks/python/lint.py` & `vmklib-2.0.0/vmklib/tasks/python/lint.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 """
 
 # built-in
 from pathlib import Path
 from typing import Dict, List
 
 # third-party
+from vcorelib.platform import is_windows
 from vcorelib.task import Inbox, Outbox, Phony
 from vcorelib.task.manager import TaskManager
 from vcorelib.task.subprocess.run import SubprocessLogMixin
 
 # internal
 from vmklib.tasks.args import environ_fallback_split
 from vmklib.tasks.python import PREFIX
@@ -26,17 +27,23 @@
         """Get Python sources within a package."""
 
         sources = []
         if kwargs.get("python_lint_source_args", True):
             sources = [
                 cwd.joinpath("tests"),
                 cwd.joinpath(project),
-                cwd.joinpath("tasks"),
                 cwd.joinpath("setup.py"),
             ]
+
+            # This breaks on Windows because of symbolic linking. It's okay
+            # to lose the linting coverage for the not-unit-tested workflow
+            # code.
+            if not is_windows():
+                sources.append(cwd.joinpath("tasks"))
+
         return list(str(x) for x in filter(lambda x: x.exists(), sources))
 
     async def run(self, inbox: Inbox, outbox: Outbox, *args, **kwargs) -> bool:
         """Run a Python linter."""
 
         cwd: Path = args[0]
         project: str = args[1]
```

### Comparing `vmklib-1.9.0/vmklib/tasks/python/package.py` & `vmklib-2.0.0/vmklib/tasks/python/package.py`

 * *Files identical despite different names*

### Comparing `vmklib-1.9.0/vmklib/tasks/python/sa.py` & `vmklib-2.0.0/vmklib/tasks/python/sa.py`

 * *Files identical despite different names*

### Comparing `vmklib-1.9.0/vmklib/tasks/python/test.py` & `vmklib-2.0.0/vmklib/tasks/python/test.py`

 * *Files identical despite different names*

### Comparing `vmklib-1.9.0/vmklib/tasks/python/yaml.py` & `vmklib-2.0.0/vmklib/tasks/python/yaml.py`

 * *Files identical despite different names*

### Comparing `vmklib-1.9.0/vmklib/tasks/venv.py` & `vmklib-2.0.0/vmklib/tasks/venv.py`

 * *Files 4% similar despite different names*

```diff
@@ -60,14 +60,19 @@
         result = await self.exec(
             python_entry(kwargs.get("python_version", _python_version())),
             "-m",
             "venv",
             str(outbox["path"]),
         )
 
+        # Create a convenient symbolic link.
+        symlink = outbox["path"].with_name("venv")
+        if result and not symlink.exists():
+            symlink.symlink_to(outbox["path"].name)
+
         # Upgrade pip by default.
         if result and kwargs.get("upgrade_pip", True):
             result = await self.exec(
                 str(outbox["python"]),
                 "-m",
                 "pip",
                 "install",
```

### Comparing `vmklib-1.9.0/vmklib.egg-info/PKG-INFO` & `vmklib-2.0.0/vmklib.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vmklib
-Version: 1.9.0
+Version: 2.0.0
 Summary: Simplify project workflows by standardizing use of GNU Make.
 Home-page: https://github.com/vkottler/vmklib
 Author: Vaughn Kottler
 Author-email: Vaughn Kottler <vaughnkottler@gmail.com>
 Maintainer-email: Vaughn Kottler <vaughnkottler@gmail.com>
 License: MIT License
         
@@ -26,58 +26,76 @@
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
         
 Keywords: workflow,tool,make
 Classifier: Topic :: Software Development :: Build Tools
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: Unix
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
-Requires-Python: >=3.8
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
-Provides-Extra: test
 License-File: LICENSE
+Requires-Dist: vcorelib>=2.4.0
+Provides-Extra: test
+Requires-Dist: pylint; extra == "test"
+Requires-Dist: flake8; extra == "test"
+Requires-Dist: black; extra == "test"
+Requires-Dist: ruff; extra == "test"
+Requires-Dist: mypy; extra == "test"
+Requires-Dist: isort; extra == "test"
+Requires-Dist: yamllint; extra == "test"
+Requires-Dist: yambs; extra == "test"
+Requires-Dist: vmklib; extra == "test"
+Requires-Dist: sphinx; extra == "test"
+Requires-Dist: sphinx-book-theme; extra == "test"
+Requires-Dist: pytest-asyncio; extra == "test"
+Requires-Dist: setuptools-wrapper; extra == "test"
 
 <!--
     =====================================
     generator=datazen
-    version=3.1.2
-    hash=1280d00c2447ef272e48abbae9617e0a
+    version=3.1.3
+    hash=c704961deeb1f544c94a11a7582f58d4
     =====================================
 -->
 
-# vmklib ([1.9.0](https://pypi.org/project/vmklib/))
+# vmklib ([2.0.0](https://pypi.org/project/vmklib/))
 
 [![python](https://img.shields.io/pypi/pyversions/vmklib.svg)](https://pypi.org/project/vmklib/)
 ![Build Status](https://github.com/vkottler/vmklib/workflows/Python%20Package/badge.svg)
 [![codecov](https://codecov.io/gh/vkottler/vmklib/branch/master/graphs/badge.svg?branch=master)](https://codecov.io/github/vkottler/vmklib)
 ![PyPI - Status](https://img.shields.io/pypi/status/vmklib)
 ![Dependents (via libraries.io)](https://img.shields.io/librariesio/dependents/pypi/vmklib)
 
 *Simplify project workflows by standardizing use of GNU Make.*
 
-See also: [generated documentation](https://vkottler.github.io/python/pydoc/vmklib.html)
-(created with [`pydoc`](https://docs.python.org/3/library/pydoc.html)).
+## Documentation
+
+### Generated
+
+* By [sphinx-apidoc](https://vkottler.github.io/python/sphinx/vmklib)
+(What's [`sphinx-apidoc`](https://www.sphinx-doc.org/en/master/man/sphinx-apidoc.html)?)
+* By [pydoc](https://vkottler.github.io/python/pydoc/vmklib.html)
+(What's [`pydoc`](https://docs.python.org/3/library/pydoc.html)?)
 
 ## Python Version Support
 
 This package is tested with the following Python minor versions:
 
-* [`python3.8`](https://docs.python.org/3.8/)
-* [`python3.9`](https://docs.python.org/3.9/)
 * [`python3.10`](https://docs.python.org/3.10/)
 * [`python3.11`](https://docs.python.org/3.11/)
+* [`python3.12`](https://docs.python.org/3.12/)
 
 ## Platform Support
 
 This package is tested on the following platforms:
 
 * `ubuntu-latest`
 * `macos-latest`
@@ -109,27 +127,30 @@
 * [Dependency Graph](#dependency-graph)
 
 # Command-line Options
 
 ```
 $ ./venv3.11/bin/mk -h
 
-usage: mk [-h] [--version] [-v] [-C DIR] [-p PREFIX] [-d] [-D DEFAULT]
-          [-f FILE] [-c CONFIG] [-P PROJ]
+usage: mk [-h] [--version] [-v] [-q] [--curses] [--no-uvloop] [-C DIR]
+          [-p PREFIX] [-d] [-D DEFAULT] [-f FILE] [-c CONFIG] [-P PROJ]
           [targets ...]
 
 Simplify project workflows by standardizing use of GNU Make.
 
 positional arguments:
   targets               targets to execute
 
 options:
   -h, --help            show this help message and exit
   --version             show program's version number and exit
   -v, --verbose         set to increase logging verbosity
+  -q, --quiet           set to reduce output
+  --curses              whether or not to use curses.wrapper when starting
+  --no-uvloop           whether or not to disable uvloop as event loop driver
   -C DIR, --dir DIR     execute from a specific directory
   -p PREFIX, --prefix PREFIX
                         a prefix to apply to all targets
   -d, --disable-make    whether or not to allow GNU Make target resolution
                         (default: 'False')
   -D DEFAULT, --default DEFAULT
                         default target to make if none is specified (default:
```

### Comparing `vmklib-1.9.0/vmklib.egg-info/SOURCES.txt` & `vmklib-2.0.0/vmklib.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 vmklib/__init__.py
 vmklib/__main__.py
 vmklib/app.py
 vmklib/dev_requirements.txt
 vmklib/entry.py
 vmklib/py.typed
 vmklib/requirements.txt
-vmklib/resources.py
 vmklib.egg-info/PKG-INFO
 vmklib.egg-info/SOURCES.txt
 vmklib.egg-info/dependency_links.txt
 vmklib.egg-info/entry_points.txt
 vmklib.egg-info/requires.txt
 vmklib.egg-info/top_level.txt
 vmklib/data/conf.mk
@@ -36,21 +35,23 @@
 vmklib/data/python/docs.mk
 vmklib/data/python/pypi.mk
 vmklib/data/python/upload.mk
 vmklib/tasks/__init__.py
 vmklib/tasks/args.py
 vmklib/tasks/clean.py
 vmklib/tasks/github.py
+vmklib/tasks/release.py
 vmklib/tasks/venv.py
 vmklib/tasks/mixins/__init__.py
 vmklib/tasks/mixins/concrete.py
 vmklib/tasks/mixins/curl.py
 vmklib/tasks/node/__init__.py
 vmklib/tasks/python/__init__.py
 vmklib/tasks/python/build.py
 vmklib/tasks/python/datazen.py
 vmklib/tasks/python/docs.py
 vmklib/tasks/python/lint.py
 vmklib/tasks/python/package.py
+vmklib/tasks/python/release.py
 vmklib/tasks/python/sa.py
 vmklib/tasks/python/test.py
 vmklib/tasks/python/yaml.py
```

