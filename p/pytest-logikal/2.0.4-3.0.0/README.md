# Comparing `tmp/pytest-logikal-2.0.4.tar.gz` & `tmp/pytest_logikal-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest-logikal-2.0.4.tar", last modified: Sat Mar 30 11:03:58 2024, max compression
+gzip compressed data, was "pytest_logikal-3.0.0.tar", last modified: Sat May 18 17:00:43 2024, max compression
```

## Comparing `pytest-logikal-2.0.4.tar` & `pytest_logikal-3.0.0.tar`

### file list

```diff
@@ -1,58 +1,67 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 11:03:58.406928 pytest-logikal-2.0.4/
--rw-r--r--   0 runner    (1001) docker     (127)     1052 2024-03-30 11:03:39.000000 pytest-logikal-2.0.4/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-03-30 11:03:39.000000 pytest-logikal-2.0.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3765 2024-03-30 11:03:58.406928 pytest-logikal-2.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      280 2024-03-30 11:03:39.000000 pytest-logikal-2.0.4/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)      217 2024-03-30 11:03:39.000000 pytest-logikal-2.0.4/compose.yml
--rw-r--r--   0 runner    (1001) docker     (127)      785 2024-03-30 11:03:39.000000 pytest-logikal-2.0.4/entry_points.ini
--rw-r--r--   0 runner    (1001) docker     (127)     2862 2024-03-30 11:03:39.000000 pytest-logikal-2.0.4/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 11:03:58.402928 pytest-logikal-2.0.4/pytest_logikal/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-30 11:03:39.000000 pytest-logikal-2.0.4/pytest_logikal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2098 2024-03-30 11:03:39.000000 pytest-logikal-2.0.4/pytest_logikal/bandit.py
--rw-r--r--   0 runner    (1001) docker     (127)      181 2024-03-30 11:03:39.000000 pytest-logikal-2.0.4/pytest_logikal/bandit_config.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1805 2024-03-30 11:03:39.000000 pytest-logikal-2.0.4/pytest_logikal/black.py
--rw-r--r--   0 runner    (1001) docker     (127)    13919 2024-03-30 11:03:39.000000 pytest-logikal-2.0.4/pytest_logikal/browser.py
--rw-r--r--   0 runner    (1001) docker     (127)     2230 2024-03-30 11:03:39.000000 pytest-logikal-2.0.4/pytest_logikal/build.py
--rw-r--r--   0 runner    (1001) docker     (127)     8366 2024-03-30 11:03:39.000000 pytest-logikal-2.0.4/pytest_logikal/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     2558 2024-03-30 11:03:39.000000 pytest-logikal-2.0.4/pytest_logikal/css.py
--rw-r--r--   0 runner    (1001) docker     (127)     3757 2024-03-30 11:03:39.000000 pytest-logikal-2.0.4/pytest_logikal/css_config.yml
--rw-r--r--   0 runner    (1001) docker     (127)     4114 2024-03-30 11:03:39.000000 pytest-logikal-2.0.4/pytest_logikal/django.py
--rw-r--r--   0 runner    (1001) docker     (127)     1135 2024-03-30 11:03:39.000000 pytest-logikal-2.0.4/pytest_logikal/docs.py
--rw-r--r--   0 runner    (1001) docker     (127)     3339 2024-03-30 11:03:39.000000 pytest-logikal-2.0.4/pytest_logikal/file_checker.py
--rw-r--r--   0 runner    (1001) docker     (127)     3473 2024-03-30 11:03:39.000000 pytest-logikal-2.0.4/pytest_logikal/html.py
--rw-r--r--   0 runner    (1001) docker     (127)     2463 2024-03-30 11:03:39.000000 pytest-logikal-2.0.4/pytest_logikal/isort.py
--rw-r--r--   0 runner    (1001) docker     (127)     1993 2024-03-30 11:03:39.000000 pytest-logikal-2.0.4/pytest_logikal/js.py
--rw-r--r--   0 runner    (1001) docker     (127)     5447 2024-03-30 11:03:39.000000 pytest-logikal-2.0.4/pytest_logikal/js_config.yml
--rw-r--r--   0 runner    (1001) docker     (127)     4669 2024-03-30 11:03:39.000000 pytest-logikal-2.0.4/pytest_logikal/licenses.py
--rw-r--r--   0 runner    (1001) docker     (127)     2007 2024-03-30 11:03:39.000000 pytest-logikal-2.0.4/pytest_logikal/migration.py
--rw-r--r--   0 runner    (1001) docker     (127)    98728 2024-03-30 11:03:39.000000 pytest-logikal-2.0.4/pytest_logikal/package-lock.json
--rw-r--r--   0 runner    (1001) docker     (127)      127 2024-03-30 11:03:39.000000 pytest-logikal-2.0.4/pytest_logikal/package.json
--rw-r--r--   0 runner    (1001) docker     (127)     1801 2024-03-30 11:03:39.000000 pytest-logikal-2.0.4/pytest_logikal/plugin.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-30 11:03:39.000000 pytest-logikal-2.0.4/pytest_logikal/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     4825 2024-03-30 11:03:39.000000 pytest-logikal-2.0.4/pytest_logikal/pylint.py
--rw-r--r--   0 runner    (1001) docker     (127)     1396 2024-03-30 11:03:39.000000 pytest-logikal-2.0.4/pytest_logikal/requirements.py
--rw-r--r--   0 runner    (1001) docker     (127)     2484 2024-03-30 11:03:39.000000 pytest-logikal-2.0.4/pytest_logikal/style.py
--rw-r--r--   0 runner    (1001) docker     (127)     1390 2024-03-30 11:03:39.000000 pytest-logikal-2.0.4/pytest_logikal/svg.py
--rw-r--r--   0 runner    (1001) docker     (127)     3889 2024-03-30 11:03:39.000000 pytest-logikal-2.0.4/pytest_logikal/translations.py
--rw-r--r--   0 runner    (1001) docker     (127)     4550 2024-03-30 11:03:39.000000 pytest-logikal-2.0.4/pytest_logikal/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2586 2024-03-30 11:03:39.000000 pytest-logikal-2.0.4/pytest_logikal/validator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 11:03:58.402928 pytest-logikal-2.0.4/pytest_logikal.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3765 2024-03-30 11:03:58.000000 pytest-logikal-2.0.4/pytest_logikal.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1330 2024-03-30 11:03:58.000000 pytest-logikal-2.0.4/pytest_logikal.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-30 11:03:58.000000 pytest-logikal-2.0.4/pytest_logikal.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      785 2024-03-30 11:03:58.000000 pytest-logikal-2.0.4/pytest_logikal.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      599 2024-03-30 11:03:58.000000 pytest-logikal-2.0.4/pytest_logikal.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-03-30 11:03:58.000000 pytest-logikal-2.0.4/pytest_logikal.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 11:03:58.402928 pytest-logikal-2.0.4/requirements/
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-03-30 11:03:39.000000 pytest-logikal-2.0.4/requirements/build.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1048 2024-03-30 11:03:39.000000 pytest-logikal-2.0.4/requirements/build.txt.lock
--rw-r--r--   0 runner    (1001) docker     (127)      350 2024-03-30 11:03:39.000000 pytest-logikal-2.0.4/requirements/core.txt
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-03-30 11:03:39.000000 pytest-logikal-2.0.4/requirements/dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2869 2024-03-30 11:03:39.000000 pytest-logikal-2.0.4/requirements/dev.txt.lock
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-03-30 11:03:39.000000 pytest-logikal-2.0.4/requirements/docs.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2510 2024-03-30 11:03:39.000000 pytest-logikal-2.0.4/requirements/docs.txt.lock
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 11:03:58.402928 pytest-logikal-2.0.4/requirements/extras/
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-03-30 11:03:39.000000 pytest-logikal-2.0.4/requirements/extras/black.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-03-30 11:03:39.000000 pytest-logikal-2.0.4/requirements/extras/browser.txt
--rw-r--r--   0 runner    (1001) docker     (127)      229 2024-03-30 11:03:39.000000 pytest-logikal-2.0.4/requirements/extras/django.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-30 11:03:58.406928 pytest-logikal-2.0.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 17:00:43.371421 pytest_logikal-3.0.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1052 2024-05-18 17:00:25.000000 pytest_logikal-3.0.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-18 17:00:25.000000 pytest_logikal-3.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4014 2024-05-18 17:00:43.371421 pytest_logikal-3.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      280 2024-05-18 17:00:25.000000 pytest_logikal-3.0.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      217 2024-05-18 17:00:25.000000 pytest_logikal-3.0.0/compose.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      792 2024-05-18 17:00:25.000000 pytest_logikal-3.0.0/entry_points.ini
+-rw-r--r--   0 runner    (1001) docker     (127)     2826 2024-05-18 17:00:25.000000 pytest_logikal-3.0.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 17:00:43.367421 pytest_logikal-3.0.0/pytest_logikal/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-18 17:00:25.000000 pytest_logikal-3.0.0/pytest_logikal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2098 2024-05-18 17:00:25.000000 pytest_logikal-3.0.0/pytest_logikal/bandit.py
+-rw-r--r--   0 runner    (1001) docker     (127)      181 2024-05-18 17:00:25.000000 pytest_logikal-3.0.0/pytest_logikal/bandit_config.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1805 2024-05-18 17:00:25.000000 pytest_logikal-3.0.0/pytest_logikal/black.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 17:00:43.367421 pytest_logikal-3.0.0/pytest_logikal/browser/
+-rw-r--r--   0 runner    (1001) docker     (127)      286 2024-05-18 17:00:25.000000 pytest_logikal-3.0.0/pytest_logikal/browser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7039 2024-05-18 17:00:25.000000 pytest_logikal-3.0.0/pytest_logikal/browser/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1481 2024-05-18 17:00:25.000000 pytest_logikal-3.0.0/pytest_logikal/browser/chrome.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1533 2024-05-18 17:00:25.000000 pytest_logikal-3.0.0/pytest_logikal/browser/chromium.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1713 2024-05-18 17:00:25.000000 pytest_logikal-3.0.0/pytest_logikal/browser/edge.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3704 2024-05-18 17:00:25.000000 pytest_logikal-3.0.0/pytest_logikal/browser/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1545 2024-05-18 17:00:25.000000 pytest_logikal-3.0.0/pytest_logikal/browser/scenarios.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1192 2024-05-18 17:00:25.000000 pytest_logikal-3.0.0/pytest_logikal/browser/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2230 2024-05-18 17:00:25.000000 pytest_logikal-3.0.0/pytest_logikal/build.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7865 2024-05-18 17:00:25.000000 pytest_logikal-3.0.0/pytest_logikal/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2558 2024-05-18 17:00:25.000000 pytest_logikal-3.0.0/pytest_logikal/css.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3757 2024-05-18 17:00:25.000000 pytest_logikal-3.0.0/pytest_logikal/css_config.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     4575 2024-05-18 17:00:25.000000 pytest_logikal-3.0.0/pytest_logikal/django.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1135 2024-05-18 17:00:25.000000 pytest_logikal-3.0.0/pytest_logikal/docs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3339 2024-05-18 17:00:25.000000 pytest_logikal-3.0.0/pytest_logikal/file_checker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3473 2024-05-18 17:00:25.000000 pytest_logikal-3.0.0/pytest_logikal/html.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2463 2024-05-18 17:00:25.000000 pytest_logikal-3.0.0/pytest_logikal/isort.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1993 2024-05-18 17:00:25.000000 pytest_logikal-3.0.0/pytest_logikal/js.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5447 2024-05-18 17:00:25.000000 pytest_logikal-3.0.0/pytest_logikal/js_config.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     4768 2024-05-18 17:00:25.000000 pytest_logikal-3.0.0/pytest_logikal/licenses.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2007 2024-05-18 17:00:25.000000 pytest_logikal-3.0.0/pytest_logikal/migration.py
+-rw-r--r--   0 runner    (1001) docker     (127)      541 2024-05-18 17:00:25.000000 pytest_logikal-3.0.0/pytest_logikal/node_install.py
+-rw-r--r--   0 runner    (1001) docker     (127)    98728 2024-05-18 17:00:25.000000 pytest_logikal-3.0.0/pytest_logikal/package-lock.json
+-rw-r--r--   0 runner    (1001) docker     (127)      127 2024-05-18 17:00:25.000000 pytest_logikal-3.0.0/pytest_logikal/package.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1801 2024-05-18 17:00:25.000000 pytest_logikal-3.0.0/pytest_logikal/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-18 17:00:25.000000 pytest_logikal-3.0.0/pytest_logikal/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     4825 2024-05-18 17:00:25.000000 pytest_logikal-3.0.0/pytest_logikal/pylint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1396 2024-05-18 17:00:25.000000 pytest_logikal-3.0.0/pytest_logikal/requirements.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2484 2024-05-18 17:00:25.000000 pytest_logikal-3.0.0/pytest_logikal/style.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1390 2024-05-18 17:00:25.000000 pytest_logikal-3.0.0/pytest_logikal/svg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3889 2024-05-18 17:00:25.000000 pytest_logikal-3.0.0/pytest_logikal/translations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4810 2024-05-18 17:00:25.000000 pytest_logikal-3.0.0/pytest_logikal/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3135 2024-05-18 17:00:25.000000 pytest_logikal-3.0.0/pytest_logikal/validator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 17:00:43.371421 pytest_logikal-3.0.0/pytest_logikal.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4014 2024-05-18 17:00:43.000000 pytest_logikal-3.0.0/pytest_logikal.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1601 2024-05-18 17:00:43.000000 pytest_logikal-3.0.0/pytest_logikal.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-18 17:00:43.000000 pytest_logikal-3.0.0/pytest_logikal.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      792 2024-05-18 17:00:43.000000 pytest_logikal-3.0.0/pytest_logikal.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      673 2024-05-18 17:00:43.000000 pytest_logikal-3.0.0/pytest_logikal.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-18 17:00:43.000000 pytest_logikal-3.0.0/pytest_logikal.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 17:00:43.367421 pytest_logikal-3.0.0/requirements/
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-18 17:00:25.000000 pytest_logikal-3.0.0/requirements/build.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-05-18 17:00:25.000000 pytest_logikal-3.0.0/requirements/build.txt.lock
+-rw-r--r--   0 runner    (1001) docker     (127)      351 2024-05-18 17:00:25.000000 pytest_logikal-3.0.0/requirements/core.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-18 17:00:25.000000 pytest_logikal-3.0.0/requirements/dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2949 2024-05-18 17:00:25.000000 pytest_logikal-3.0.0/requirements/dev.txt.lock
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-05-18 17:00:25.000000 pytest_logikal-3.0.0/requirements/docs.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2550 2024-05-18 17:00:25.000000 pytest_logikal-3.0.0/requirements/docs.txt.lock
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 17:00:43.367421 pytest_logikal-3.0.0/requirements/extras/
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-18 17:00:25.000000 pytest_logikal-3.0.0/requirements/extras/black.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      169 2024-05-18 17:00:25.000000 pytest_logikal-3.0.0/requirements/extras/browser.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      229 2024-05-18 17:00:25.000000 pytest_logikal-3.0.0/requirements/extras/django.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-18 17:00:43.371421 pytest_logikal-3.0.0/setup.cfg
```

### Comparing `pytest-logikal-2.0.4/LICENSE.txt` & `pytest_logikal-3.0.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pytest-logikal-2.0.4/PKG-INFO` & `pytest_logikal-3.0.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-logikal
-Version: 2.0.4
+Version: 3.0.0
 Summary: Common testing environment
 Author-email: Logikal GmbH <contact@logikal.io>
 License: Copyright 2022 Logikal GmbH
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and
         associated documentation files (the "Software"), to deal in the Software without restriction,
         including without limitation the rights to use, copy, modify, merge, publish, distribute,
@@ -34,40 +34,45 @@
 Classifier: Framework :: Pytest
 Classifier: Topic :: Software Development
 Classifier: Typing :: Typed
 Requires-Python: ~=3.8
 Description-Content-Type: text/x-rst
 License-File: LICENSE.txt
 Requires-Dist: bandit==1.7.8
-Requires-Dist: coverage[toml]==7.4.4
+Requires-Dist: coverage[toml]==7.5.1
 Requires-Dist: isort[colors]==5.13.2
-Requires-Dist: mypy==1.9.0
+Requires-Dist: mypy==1.10.0
 Requires-Dist: pip-licenses==4.4.0
 Requires-Dist: pycodestyle==2.11.1
 Requires-Dist: pydocstyle[toml]==6.3.0
-Requires-Dist: pylint==3.1.0
-Requires-Dist: pytest==8.1.1
+Requires-Dist: pylint==3.2.0
+Requires-Dist: pytest==8.2.0
 Requires-Dist: pytest-cov==5.0.0
 Requires-Dist: pytest-mock==3.14.0
 Requires-Dist: pytest-mypy==0.10.3
-Requires-Dist: pytest-xdist[psutil]==3.5.0
-Requires-Dist: pillow~=10.2
+Requires-Dist: pytest-xdist[psutil]==3.6.1
+Requires-Dist: pillow~=10.3
 Requires-Dist: Pygments~=2.17
 Requires-Dist: logikal-utils~=1.0
 Requires-Dist: pyorbs~=2.1
 Requires-Dist: termcolor~=2.4
 Provides-Extra: black
-Requires-Dist: black==24.3.0; extra == "black"
+Requires-Dist: black==24.4.2; extra == "black"
 Provides-Extra: browser
-Requires-Dist: selenium==4.19.0; extra == "browser"
+Requires-Dist: requests~=2.31; extra == "browser"
+Requires-Dist: types-requests~=2.31; extra == "browser"
+Requires-Dist: tqdm~=4.66; extra == "browser"
+Requires-Dist: types-tqdm~=4.66; extra == "browser"
+Requires-Dist: selenium==4.21.0; extra == "browser"
+Requires-Dist: xdg~=5.1; extra == "browser"
 Provides-Extra: django
 Requires-Dist: Babel~=2.14; extra == "django"
 Requires-Dist: Django~=4.2; extra == "django"
 Requires-Dist: django-stubs~=4.2; extra == "django"
-Requires-Dist: django-migration-linter~=5.0; extra == "django"
+Requires-Dist: django-migration-linter~=5.1; extra == "django"
 Requires-Dist: djlint==1.34.1; extra == "django"
 Requires-Dist: pylint-django==2.5.5; extra == "django"
 Requires-Dist: pytest-django==4.8.0; extra == "django"
 Requires-Dist: pytest-factoryboy==2.7.0; extra == "django"
 Requires-Dist: requests~=2.31; extra == "django"
 Requires-Dist: types-requests~=2.31; extra == "django"
 Requires-Dist: logikal-utils[docker]~=1.0; extra == "django"
```

### Comparing `pytest-logikal-2.0.4/entry_points.ini` & `pytest_logikal-3.0.0/entry_points.ini`

 * *Files 8% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 logikal_docs = pytest_logikal.docs
 logikal_isort = pytest_logikal.isort
 logikal_licenses = pytest_logikal.licenses
 logikal_pylint = pytest_logikal.pylint
 logikal_requirements = pytest_logikal.requirements
 logikal_style = pytest_logikal.style
 logikal_black = pytest_logikal.black [black]
-logikal_browser = pytest_logikal.browser [browser]
+logikal_browser = pytest_logikal.browser.plugin [browser]
 logikal_django = pytest_logikal.django [django]
 logikal_migration = pytest_logikal.migration [django]
 logikal_translations = pytest_logikal.translations [django]
 logikal_html = pytest_logikal.html [django]
 logikal_css = pytest_logikal.css [django]
 logikal_svg = pytest_logikal.svg [django]
 logikal_js = pytest_logikal.js [django]
```

### Comparing `pytest-logikal-2.0.4/pyproject.toml` & `pytest_logikal-3.0.0/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 [project.urls]
 'Documentation' = 'https://docs.logikal.io/pytest-logikal/'
 'Release notes' = 'https://github.com/logikal-io/pytest-logikal/releases'
 'Issue tracker' = 'https://github.com/logikal-io/pytest-logikal/issues'
 'Source code' = 'https://github.com/logikal-io/pytest-logikal'
 
 [tool.setuptools]
-packages = ['pytest_logikal']
+packages = ['pytest_logikal', 'pytest_logikal.browser']
 
 [tool.setuptools.dynamic]
 entry-points = {file = 'entry_points.ini'}
 dependencies = {file = 'requirements/core.txt'}
 
 [tool.setuptools.dynamic.optional-dependencies]
 black = {file = 'requirements/extras/black.txt'}
@@ -51,19 +51,14 @@
 
 [tool.pytest.ini_options]
 DJANGO_SETTINGS_MODULE = 'tests.website.settings'
 norecursedirs = [
   '*.egg', '.*', 'build', 'dist', 'node_modules',  # standard folders
   'tests/pytest_logikal/files',  # ignore files used inside plugin runs
 ]
-filterwarnings = [
-  'error',
-  # Can be removed with the next release of django-migration-linter
-  "ignore:unclosed file .* name='/dev/null':ResourceWarning",
-]
 
 [tool.mypy]
 plugins = ['mypy_django_plugin.main']  # see https://github.com/python/mypy/issues/11667
 
 [[tool.mypy.overrides]]
 ignore_missing_imports = true
 module = [
@@ -71,17 +66,19 @@
   'django_migration_linter.*',  # https://github.com/3YOURMIND/django-migration-linter/issues/238
   'factory.*',
   'pycodestyle',
   'pydocstyle',
   'xdist.*',
 ]
 
-[tool.browser.settings]
-desktop-docs = {width = 1024, height = 768}
-mobile-xl = {width = 480, frame_height = 768, mobile = true}
+[tool.browser.versions]
+# See https://googlechromelabs.github.io/chrome-for-testing/#stable
+chrome = '124.0.6367.91'
+# See https://learn.microsoft.com/en-us/deployedge/microsoft-edge-relnote-stable-channel
+edge = '124.0.2478.80'
 
 [tool.isort]
 known_first_party = ['pytest_logikal']
 
 [tool.coverage.report]
 omit = [
   '/tmp/*',  # ignore temporary files created during testing
```

### Comparing `pytest-logikal-2.0.4/pytest_logikal/bandit.py` & `pytest_logikal-3.0.0/pytest_logikal/bandit.py`

 * *Files identical despite different names*

### Comparing `pytest-logikal-2.0.4/pytest_logikal/black.py` & `pytest_logikal-3.0.0/pytest_logikal/black.py`

 * *Files identical despite different names*

### Comparing `pytest-logikal-2.0.4/pytest_logikal/build.py` & `pytest_logikal-3.0.0/pytest_logikal/build.py`

 * *Files identical despite different names*

### Comparing `pytest-logikal-2.0.4/pytest_logikal/core.py` & `pytest_logikal-3.0.0/pytest_logikal/core.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 import logging
 import os
 import shutil
-import subprocess
 import sys
 from importlib.util import find_spec
 from itertools import chain
 from pathlib import Path
 from typing import Any, Callable, Dict, Iterator, List, Optional, Tuple, Union
 
 import pytest
@@ -116,34 +115,24 @@
         'log_date_format': '%Y-%m-%d %H:%M:%S',
         'log_auto_indent': 'True',
     }
     early_config.inicfg = {**ini_defaults, **early_config.inicfg}
     yield
 
 
-def install_packages(node_prefix: Optional[Path] = None) -> None:
-    node_prefix = node_prefix or Path(__file__).parent
-    if not (node_prefix / 'node_modules').exists():
-        print(colored('Installing Node.js packages', attrs=['bold']))
-        command = ['npm', 'install', '--no-save', '--prefix', str(node_prefix)]
-        subprocess.run(command, text=True, check=True)  # nosec: secure, not using untrusted input
-
-
-def pytest_configure(config: pytest.Config) -> None:
-    # Installing Node.js packages
-    if EXTRAS['django'] and not config.getoption('no_install'):
-        install_packages()
-
+def pytest_sessionstart(session: pytest.Session) -> None:
     # Clearing cache
-    if config.getoption('clear'):
+    if session.config.getoption('clear'):
         print(colored('Clearing cache', 'yellow', attrs=['bold']))
         Path('.coverage').unlink(missing_ok=True)
         shutil.rmtree('.pytest_cache', ignore_errors=True)
         shutil.rmtree('.mypy_cache', ignore_errors=True)
 
+
+def pytest_configure(config: pytest.Config) -> None:
     # Hiding information
     if not config.getoption('verbose'):
         # Hiding overly verbose debug and info log messages
         logging.getLogger('django_migration_linter').setLevel(logging.WARNING)
         logging.getLogger('docker').setLevel(logging.INFO)
         logging.getLogger('faker').setLevel(logging.INFO)
         logging.getLogger('filelock').setLevel(logging.WARNING)
```

### Comparing `pytest-logikal-2.0.4/pytest_logikal/css.py` & `pytest_logikal-3.0.0/pytest_logikal/css.py`

 * *Files identical despite different names*

### Comparing `pytest-logikal-2.0.4/pytest_logikal/css_config.yml` & `pytest_logikal-3.0.0/pytest_logikal/css_config.yml`

 * *Files identical despite different names*

### Comparing `pytest-logikal-2.0.4/pytest_logikal/django.py` & `pytest_logikal-3.0.0/pytest_logikal/django.py`

 * *Files 9% similar despite different names*

```diff
@@ -8,20 +8,31 @@
 from django.conf import settings
 from django.urls import reverse
 from django.utils import timezone as django_timezone, translation
 from factory import random as factory_random
 from mypy_django_plugin import config as mypy_django_plugin_config
 from pytest_django.live_server_helper import LiveServer
 
+from pytest_logikal.node_install import install_node_packages
 from pytest_logikal.utils import Fixture, Function
+from pytest_logikal.validator import Validator
 
 DEFAULT_RANDOM_SEED = 42
 LiveURL = Callable[[str], str]
 
 
+def pytest_sessionstart(session: pytest.Session) -> None:
+    if not session.config.getoption('no_install'):
+        install_node_packages()
+
+    if not session.config.getoption('no_css') and not session.config.getoption('no_svg'):
+        # We start the validator service here to avoid pytest's output capturing
+        Validator.start_service()
+
+
 def pytest_configure(config: pytest.Config) -> None:
     # Patching django-stubs
     def parse_toml_file(self: Any, *_args: Any, **_kwargs: Any) -> None:
         self.django_settings_module = str(config.inicfg['DJANGO_SETTINGS_MODULE'])
         self.strict_settings = True
 
     mypy_django_plugin_config.DjangoPluginConfig.parse_toml_file = parse_toml_file  # type: ignore
@@ -40,15 +51,15 @@
     """
     Set a default seed for pytest-factoryboy for deterministic testing. Automatically applied.
     """
     factory_random.reseed_random(DEFAULT_RANDOM_SEED)
 
 
 @pytest.fixture
-def live_url(live_server: LiveServer) -> LiveURL:  # noqa: D400,D402,D415,D417
+def live_url(live_server: LiveServer) -> LiveURL:  # noqa: D400, D402, D415, D417
     """
     live_url(name: str) -> str
 
     Return the path to a URL.
 
     Args:
         name: The URL pattern name.
```

### Comparing `pytest-logikal-2.0.4/pytest_logikal/docs.py` & `pytest_logikal-3.0.0/pytest_logikal/docs.py`

 * *Files identical despite different names*

### Comparing `pytest-logikal-2.0.4/pytest_logikal/file_checker.py` & `pytest_logikal-3.0.0/pytest_logikal/file_checker.py`

 * *Files identical despite different names*

### Comparing `pytest-logikal-2.0.4/pytest_logikal/html.py` & `pytest_logikal-3.0.0/pytest_logikal/html.py`

 * *Files identical despite different names*

### Comparing `pytest-logikal-2.0.4/pytest_logikal/isort.py` & `pytest_logikal-3.0.0/pytest_logikal/isort.py`

 * *Files identical despite different names*

### Comparing `pytest-logikal-2.0.4/pytest_logikal/js.py` & `pytest_logikal-3.0.0/pytest_logikal/js.py`

 * *Files identical despite different names*

### Comparing `pytest-logikal-2.0.4/pytest_logikal/js_config.yml` & `pytest_logikal-3.0.0/pytest_logikal/js_config.yml`

 * *Files identical despite different names*

### Comparing `pytest-logikal-2.0.4/pytest_logikal/licenses.py` & `pytest_logikal-3.0.0/pytest_logikal/licenses.py`

 * *Files 3% similar despite different names*

```diff
@@ -34,28 +34,29 @@
     r'^Public Domain$',
     r'^Python Software Foundation License$',
     r'^The MIT License \(MIT\)$',
     r'^The Unlicense \(Unlicense\)$',
 ]
 
 ALLOWED_PACKAGES = {
+    'django-migration-linter': r'^UNKNOWN$',  # license is Apache License 2.0, see [1]
+    'djlint': r'^GNU General Public License v3 or later \(GPLv3\+\)$',  # only used as a local tool
     'facebook-business': r'^LICENSE\.txt$',  # only used as a connector
     'facebook_business': r'^LICENSE\.txt$',  # only used as a connector
-    'djlint': r'^GNU General Public License v3 or later \(GPLv3\+\)$',  # only used as a local tool
     'html-tag-names': r'^GNU General Public License v3 or later \(GPLv3\+\)$',  # local tool
     'html-void-elements': r'^GNU General Public License v3 or later \(GPLv3\+\)$',  # local tool
-    'pkg-resources': r'^UNKNOWN$',  # caused by an Ubuntu bug, see [1]
-    'pkg_resources': r'^UNKNOWN$',  # caused by an Ubuntu bug, see [1]
     'pillow': r'^Historical Permission Notice and Disclaimer \(HPND\)$',  # license is BSD-like
+    'pkg-resources': r'^UNKNOWN$',  # caused by an Ubuntu bug, see [2]
+    'pkg_resources': r'^UNKNOWN$',  # caused by an Ubuntu bug, see [2]
     'pylint': r'^GNU General Public License v2 \(GPLv2\)$',  # only used as a local tool
     'pylint-django': r'^GNU General Public License v2 or later \(GPLv2\+\)$',  # local plugin
     'pylint-plugin-utils': r'^GNU General Public License v2 or later \(GPLv2\+\)$',  # local plugin
-    'python-lsp-jsonrpc': r'^UNKNOWN$',  # license is MIT
 }
-# [1] https://bugs.launchpad.net/ubuntu/+source/python-pip/+bug/1635463
+# [1] https://github.com/3YOURMIND/django-migration-linter/issues/290
+# [2] https://bugs.launchpad.net/ubuntu/+source/python-pip/+bug/1635463
 
 
 def pytest_addoption(parser: pytest.Parser) -> None:
     group = parser.getgroup('licenses')
     group.addoption('--licenses', action='store_true', default=False, help='run license checks')
```

### Comparing `pytest-logikal-2.0.4/pytest_logikal/migration.py` & `pytest_logikal-3.0.0/pytest_logikal/migration.py`

 * *Files identical despite different names*

### Comparing `pytest-logikal-2.0.4/pytest_logikal/package-lock.json` & `pytest_logikal-3.0.0/pytest_logikal/package-lock.json`

 * *Files identical despite different names*

### Comparing `pytest-logikal-2.0.4/pytest_logikal/plugin.py` & `pytest_logikal-3.0.0/pytest_logikal/plugin.py`

 * *Files identical despite different names*

### Comparing `pytest-logikal-2.0.4/pytest_logikal/pylint.py` & `pytest_logikal-3.0.0/pytest_logikal/pylint.py`

 * *Files identical despite different names*

### Comparing `pytest-logikal-2.0.4/pytest_logikal/requirements.py` & `pytest_logikal-3.0.0/pytest_logikal/requirements.py`

 * *Files identical despite different names*

### Comparing `pytest-logikal-2.0.4/pytest_logikal/style.py` & `pytest_logikal-3.0.0/pytest_logikal/style.py`

 * *Files identical despite different names*

### Comparing `pytest-logikal-2.0.4/pytest_logikal/svg.py` & `pytest_logikal-3.0.0/pytest_logikal/svg.py`

 * *Files identical despite different names*

### Comparing `pytest-logikal-2.0.4/pytest_logikal/translations.py` & `pytest_logikal-3.0.0/pytest_logikal/translations.py`

 * *Files identical despite different names*

### Comparing `pytest-logikal-2.0.4/pytest_logikal/utils.py` & `pytest_logikal-3.0.0/pytest_logikal/utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,78 +3,85 @@
 from io import BytesIO
 from logging import getLogger
 from operator import methodcaller
 from os import getcwd
 from pathlib import Path
 from shutil import copy
 from subprocess import run
-from tempfile import TemporaryDirectory
+from tempfile import TemporaryDirectory, mkdtemp
 from typing import Any, Callable, Dict, Generator, Optional, Type, TypeVar
 
 from logikal_utils.project import PYPROJECT
 from PIL import Image, ImageChops
 
 from pytest_logikal.core import DEFAULT_INI_OPTIONS
 
 logger = getLogger(__name__)
 
 Function = TypeVar('Function', bound=Callable[..., Any])
 Fixture = Callable[[Function], Function]
 
 
+def tmp_path(suffix: str) -> Path:
+    path = Path(mkdtemp(prefix='pytest_logikal_', suffix=f'_{suffix}'))
+    path.mkdir(parents=True, exist_ok=True)
+    logger.debug(f'Using temporary path "{path}/"')
+    return path
+
+
 def get_ini_option(name: str) -> Any:
     ini_options = PYPROJECT.get('tool', {}).get('pytest', {}).get('ini_options', {})
     default = DEFAULT_INI_OPTIONS[name]['value']
     return type(default)(ini_options.get(name, default))
 
 
 def hide_traceback(function: Function, error: Type[Exception] = AssertionError) -> Function:
     getattr(function, '__globals__')['__tracebackhide__'] = methodcaller('errisinstance', error)
     return function
 
 
 @contextmanager
 def render_template(path: Path, context: Dict[str, Any]) -> Generator[Path, None, None]:
-    with TemporaryDirectory(prefix='pytest_logikal_') as tmp_dir:
+    with TemporaryDirectory(prefix='pytest_logikal_', suffix='_template') as tmp_dir:
         rendered = path.read_text(encoding='utf-8').format(**context)
         config_path = Path(tmp_dir) / path.name
         config_path.write_text(rendered)
         yield config_path
 
 
 @hide_traceback
-def assert_image_equal(actual: bytes, expected: Path, temp_path: Path) -> None:
-    temp_actual_path = temp_path / 'actual.png'
-    temp_expected_path = temp_path / 'expected.png'
-    temp_diff_path = temp_path / 'diff.png'
+def assert_image_equal(actual: bytes, expected: Path, image_tmp_path: Path) -> None:
+    tmp_actual_path = image_tmp_path / 'actual.png'
+    tmp_expected_path = image_tmp_path / 'expected.png'
+    tmp_diff_path = image_tmp_path / 'diff.png'
 
     logger.info(f'Checking expected image in "{expected}"')
     if expected.is_file():
         with Image.open(BytesIO(actual)) as actual_image, Image.open(expected) as expected_image:
             if actual_image == expected_image:
                 logger.info('The actual image matches the expected image')
                 return
 
-            temp_actual_path.write_bytes(actual)  # saving the temporary actual image
-            copy(expected, temp_expected_path)  # saving the temporary expected image
+            tmp_actual_path.write_bytes(actual)  # saving the temporary actual image
+            copy(expected, tmp_expected_path)  # saving the temporary expected image
             diff_image = ImageChops.invert(ImageChops.difference(
                 expected_image.convert('RGB'),
                 actual_image.convert('RGB'),
             ))
-            diff_image.save(str(temp_diff_path))  # saving the temporary diff image
+            diff_image.save(str(tmp_diff_path))  # saving the temporary diff image
             save_image_prompt(
                 message='Actual image differs from the expected image',
-                source=temp_actual_path, destination=expected, difference=temp_diff_path,
+                source=tmp_actual_path, destination=expected, difference=tmp_diff_path,
             )
     else:
         logger.info('Expected image not found')
-        temp_expected_path.write_bytes(actual)  # saving the temporary actual image as expected
+        tmp_expected_path.write_bytes(actual)  # saving the temporary actual image as expected
         save_image_prompt(
             message='Expected image file does not exist',
-            source=temp_expected_path, destination=expected,
+            source=tmp_expected_path, destination=expected,
         )
 
 
 def save_image_prompt(
     message: str,
     source: Path,
     destination: Path,
```

### Comparing `pytest-logikal-2.0.4/pytest_logikal/validator.py` & `pytest_logikal-3.0.0/pytest_logikal/validator.py`

 * *Files 16% similar despite different names*

```diff
@@ -16,29 +16,50 @@
     severity: str
     extract: Optional[str]
     first_line: int
     last_line: int
 
 
 class Validator:
-    def __init__(self, service_name: str = 'validator', port: str = '8888/tcp'):
-        service = Service(name=service_name, ready_log_text='Checker service started')
-        self._validator_url = f'http://127.0.0.1:{service.container_port(port)}'
-        logger.debug(
-            f'Using HTML/CSS/SVG validator service running at {self._validator_url} '
-            f'(container: {service.container.short_id})'
-        )
+    _SERVICE_NAME = 'validator'
+    _SERVICE_PORT = '8888/tcp'
+    _service: Optional[Service] = None
+    _service_url: Optional[str] = None
+
+    @staticmethod
+    def service() -> Service:
+        if not Validator._service:
+            Validator._service = Service(
+                name=Validator._SERVICE_NAME,
+                ready_log_text='Checker service started',
+            )
+        return Validator._service
+
+    @staticmethod
+    def service_url() -> str:
+        if not Validator._service_url:
+            port = Validator.service().container_port(Validator._SERVICE_PORT)
+            Validator._service_url = f'http://127.0.0.1:{port}'
+            logger.debug(
+                f'Using HTML/CSS/SVG validator service running at {Validator._service_url} '
+                f'(container: {Validator.service().container.short_id})'
+            )
+        return Validator._service_url
+
+    @staticmethod
+    def start_service() -> None:
+        Validator.service()
 
     def errors(self, content: str, content_type: str = 'text/html') -> List[ValidationError]:
         # Checking content
         if not content:
             raise RuntimeError('Empty content')
 
         response = requests.post(
-            self._validator_url, params={'out': 'json'}, headers={'Content-Type': content_type},
+            self.service_url(), params={'out': 'json'}, headers={'Content-Type': content_type},
             data=content.encode(), timeout=10,
         )
         if response.status_code != 200:
             raise RuntimeError(f'Cannot validate content: {response}')
 
         # Parsing error messages
         source_lines = content.splitlines()
```

### Comparing `pytest-logikal-2.0.4/pytest_logikal.egg-info/PKG-INFO` & `pytest_logikal-3.0.0/pytest_logikal.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-logikal
-Version: 2.0.4
+Version: 3.0.0
 Summary: Common testing environment
 Author-email: Logikal GmbH <contact@logikal.io>
 License: Copyright 2022 Logikal GmbH
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and
         associated documentation files (the "Software"), to deal in the Software without restriction,
         including without limitation the rights to use, copy, modify, merge, publish, distribute,
@@ -34,40 +34,45 @@
 Classifier: Framework :: Pytest
 Classifier: Topic :: Software Development
 Classifier: Typing :: Typed
 Requires-Python: ~=3.8
 Description-Content-Type: text/x-rst
 License-File: LICENSE.txt
 Requires-Dist: bandit==1.7.8
-Requires-Dist: coverage[toml]==7.4.4
+Requires-Dist: coverage[toml]==7.5.1
 Requires-Dist: isort[colors]==5.13.2
-Requires-Dist: mypy==1.9.0
+Requires-Dist: mypy==1.10.0
 Requires-Dist: pip-licenses==4.4.0
 Requires-Dist: pycodestyle==2.11.1
 Requires-Dist: pydocstyle[toml]==6.3.0
-Requires-Dist: pylint==3.1.0
-Requires-Dist: pytest==8.1.1
+Requires-Dist: pylint==3.2.0
+Requires-Dist: pytest==8.2.0
 Requires-Dist: pytest-cov==5.0.0
 Requires-Dist: pytest-mock==3.14.0
 Requires-Dist: pytest-mypy==0.10.3
-Requires-Dist: pytest-xdist[psutil]==3.5.0
-Requires-Dist: pillow~=10.2
+Requires-Dist: pytest-xdist[psutil]==3.6.1
+Requires-Dist: pillow~=10.3
 Requires-Dist: Pygments~=2.17
 Requires-Dist: logikal-utils~=1.0
 Requires-Dist: pyorbs~=2.1
 Requires-Dist: termcolor~=2.4
 Provides-Extra: black
-Requires-Dist: black==24.3.0; extra == "black"
+Requires-Dist: black==24.4.2; extra == "black"
 Provides-Extra: browser
-Requires-Dist: selenium==4.19.0; extra == "browser"
+Requires-Dist: requests~=2.31; extra == "browser"
+Requires-Dist: types-requests~=2.31; extra == "browser"
+Requires-Dist: tqdm~=4.66; extra == "browser"
+Requires-Dist: types-tqdm~=4.66; extra == "browser"
+Requires-Dist: selenium==4.21.0; extra == "browser"
+Requires-Dist: xdg~=5.1; extra == "browser"
 Provides-Extra: django
 Requires-Dist: Babel~=2.14; extra == "django"
 Requires-Dist: Django~=4.2; extra == "django"
 Requires-Dist: django-stubs~=4.2; extra == "django"
-Requires-Dist: django-migration-linter~=5.0; extra == "django"
+Requires-Dist: django-migration-linter~=5.1; extra == "django"
 Requires-Dist: djlint==1.34.1; extra == "django"
 Requires-Dist: pylint-django==2.5.5; extra == "django"
 Requires-Dist: pytest-django==4.8.0; extra == "django"
 Requires-Dist: pytest-factoryboy==2.7.0; extra == "django"
 Requires-Dist: requests~=2.31; extra == "django"
 Requires-Dist: types-requests~=2.31; extra == "django"
 Requires-Dist: logikal-utils[docker]~=1.0; extra == "django"
```

### Comparing `pytest-logikal-2.0.4/pytest_logikal.egg-info/entry_points.txt` & `pytest_logikal-3.0.0/pytest_logikal.egg-info/entry_points.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [pytest11]
 logikal = pytest_logikal.core
 logikal_bandit = pytest_logikal.bandit
 logikal_black = pytest_logikal.black [black]
-logikal_browser = pytest_logikal.browser [browser]
+logikal_browser = pytest_logikal.browser.plugin [browser]
 logikal_build = pytest_logikal.build
 logikal_css = pytest_logikal.css [django]
 logikal_django = pytest_logikal.django [django]
 logikal_docs = pytest_logikal.docs
 logikal_html = pytest_logikal.html [django]
 logikal_isort = pytest_logikal.isort
 logikal_js = pytest_logikal.js [django]
```

### Comparing `pytest-logikal-2.0.4/pytest_logikal.egg-info/requires.txt` & `pytest_logikal-3.0.0/pytest_logikal.egg-info/requires.txt`

 * *Files 22% similar despite different names*

```diff
@@ -1,37 +1,42 @@
 bandit==1.7.8
-coverage[toml]==7.4.4
+coverage[toml]==7.5.1
 isort[colors]==5.13.2
-mypy==1.9.0
+mypy==1.10.0
 pip-licenses==4.4.0
 pycodestyle==2.11.1
 pydocstyle[toml]==6.3.0
-pylint==3.1.0
-pytest==8.1.1
+pylint==3.2.0
+pytest==8.2.0
 pytest-cov==5.0.0
 pytest-mock==3.14.0
 pytest-mypy==0.10.3
-pytest-xdist[psutil]==3.5.0
-pillow~=10.2
+pytest-xdist[psutil]==3.6.1
+pillow~=10.3
 Pygments~=2.17
 logikal-utils~=1.0
 pyorbs~=2.1
 termcolor~=2.4
 
 [black]
-black==24.3.0
+black==24.4.2
 
 [browser]
-selenium==4.19.0
+requests~=2.31
+types-requests~=2.31
+tqdm~=4.66
+types-tqdm~=4.66
+selenium==4.21.0
+xdg~=5.1
 
 [django]
 Babel~=2.14
 Django~=4.2
 django-stubs~=4.2
-django-migration-linter~=5.0
+django-migration-linter~=5.1
 djlint==1.34.1
 pylint-django==2.5.5
 pytest-django==4.8.0
 pytest-factoryboy==2.7.0
 requests~=2.31
 types-requests~=2.31
 logikal-utils[docker]~=1.0
```

### Comparing `pytest-logikal-2.0.4/requirements/build.txt.lock` & `pytest_logikal-3.0.0/requirements/build.txt.lock`

 * *Files 16% similar despite different names*

```diff
@@ -1,45 +1,46 @@
 ###################################################################################################
 ##
 ##  DO NOT EDIT THIS FILE.
 ##  This is a locked requirements file generated by pyorbs.
 ##
-##  Requirements hash: 3a6ca5427065a4afd7124be4d3b04a978c888c746e811b32ca0c94b7a4d4c91f
+##  Requirements hash: 8706de2163a25299dbe1d5d6f26df03b6aaaad435e67227452ee6c0b2b97aea0
 ##
 ###################################################################################################
+backports.tarfile==1.1.1
 build==1.2.1
 certifi==2024.2.2
 cffi==1.16.0
 charset-normalizer==3.3.2
-cryptography==42.0.5
+cryptography==42.0.7
 docutils==0.20.1
-idna==3.6
+idna==3.7
 importlib_metadata==7.1.0
 importlib_resources==6.4.0
-jaraco.classes==3.3.1
-jaraco.context==4.3.0
-jaraco.functools==4.0.0
+jaraco.classes==3.4.0
+jaraco.context==5.3.0
+jaraco.functools==4.0.1
 jeepney==0.8.0
-keyring==25.0.0
+keyring==25.2.1
 markdown-it-py==3.0.0
 mdurl==0.1.2
 more-itertools==10.2.0
 nh3==0.2.17
 packaging==24.0
 pip==24.0
 pkginfo==1.10.0
-pycparser==2.21
-Pygments==2.17.2
-pyproject_hooks==1.0.0
+pycparser==2.22
+Pygments==2.18.0
+pyproject_hooks==1.1.0
 readme_renderer==43.0
 requests==2.31.0
 requests-toolbelt==1.0.0
 rfc3986==2.0.0
 rich==13.7.1
 SecretStorage==3.3.3
-setuptools==69.2.0
+setuptools==69.5.1
 tomli==2.0.1
-twine==5.0.0
-typing_extensions==4.10.0
+twine==5.1.0
+typing_extensions==4.11.0
 urllib3==2.2.1
 wheel==0.43.0
-zipp==3.18.1
+zipp==3.18.2
```

### Comparing `pytest-logikal-2.0.4/requirements/dev.txt.lock` & `pytest_logikal-3.0.0/requirements/dev.txt.lock`

 * *Files 8% similar despite different names*

```diff
@@ -1,142 +1,146 @@
 ###################################################################################################
 ##
 ##  DO NOT EDIT THIS FILE.
 ##  This is a locked requirements file generated by pyorbs.
 ##
-##  Requirements hash: 8aa9c19a85fba391e252cf3b539b30ba70086df92eca466b39d8cd0426d6ca5d
+##  Requirements hash: e16b777fdd8e5cefd14494a404036eff582b427f3c9d362c4ce52831d22696d4
 ##
 ###################################################################################################
 -e .
 alabaster==0.7.13
 appdirs==1.4.4
 asgiref==3.8.1
-astroid==3.1.0
+astroid==3.2.1
 attrs==23.2.0
-Babel==2.14.0
+Babel==2.15.0
+backports.tarfile==1.1.1
 backports.zoneinfo==0.2.1
 bandit==1.7.8
-black==24.3.0
+black==24.4.2
 build==1.2.1
 certifi==2024.2.2
 cffi==1.16.0
 charset-normalizer==3.3.2
 click==8.1.7
 colorama==0.4.6
-coverage==7.4.4
-cryptography==42.0.5
+coverage==7.5.1
+cryptography==42.0.7
 cssbeautifier==1.15.1
 dill==0.3.8
-Django==4.2.11
-django-migration-linter==5.0.0
+Django==4.2.13
+django-migration-linter==5.1.0
 django-stubs==4.2.7
-django-stubs-ext==4.2.7
+django-stubs-ext==5.0.0
 djlint==1.34.1
 docker==7.0.0
 docutils==0.20.1
 EditorConfig==0.12.4
-exceptiongroup==1.2.0
-execnet==2.0.2
+exceptiongroup==1.2.1
+execnet==2.1.1
 factory-boy==3.3.0
-Faker==24.4.0
-filelock==3.13.3
+Faker==25.2.0
+filelock==3.14.0
 h11==0.14.0
 html-tag-names==0.1.2
 html-void-elements==0.1.0
-idna==3.6
+idna==3.7
 imagesize==1.4.1
 importlib_metadata==7.1.0
 importlib_resources==6.4.0
 inflection==0.5.1
 iniconfig==2.0.0
 isort==5.13.2
-jaraco.classes==3.3.1
-jaraco.context==4.3.0
-jaraco.functools==4.0.0
+jaraco.classes==3.4.0
+jaraco.context==5.3.0
+jaraco.functools==4.0.1
 jeepney==0.8.0
-Jinja2==3.1.3
+Jinja2==3.1.4
 jsbeautifier==1.15.1
-json5==0.9.24
-keyring==25.0.0
+json5==0.9.25
+keyring==25.2.1
 logikal-docs==1.1.4
 logikal-utils==1.0.1
 markdown-it-py==3.0.0
 MarkupSafe==2.1.5
 mccabe==0.7.0
 mdurl==0.1.2
 more-itertools==10.2.0
-mypy==1.9.0
+mypy==1.10.0
 mypy-extensions==1.0.0
 nh3==0.2.17
 outcome==1.3.0.post0
 packaging==23.2
 pathspec==0.12.1
 pbr==6.0.0
-pillow==10.2.0
+pillow==10.3.0
 pip==24.0
 pip-licenses==4.4.0
 pkginfo==1.10.0
-platformdirs==4.2.0
-pluggy==1.4.0
+platformdirs==4.2.2
+pluggy==1.5.0
 prettytable==3.10.0
 psutil==5.9.8
 pycodestyle==2.11.1
-pycparser==2.21
+pycparser==2.22
 pydocstyle==6.3.0
-Pygments==2.17.2
-pylint==3.1.0
+Pygments==2.18.0
+pylint==3.2.0
 pylint-django==2.5.5
 pylint-plugin-utils==0.8.2
 pyorbs==2.1.0
-pyproject_hooks==1.0.0
+pyproject_hooks==1.1.0
 PySocks==1.7.1
-pytest==8.1.1
+pytest==8.2.0
 pytest-cov==5.0.0
 pytest-django==4.8.0
 pytest-factoryboy==2.7.0
 pytest-mock==3.14.0
 pytest-mypy==0.10.3
-pytest-xdist==3.5.0
+pytest-xdist==3.6.1
 python-dateutil==2.9.0.post0
 pytz==2024.1
 PyYAML==6.0.1
 readme_renderer==43.0
 regex==2023.12.25
 requests==2.31.0
 requests-toolbelt==1.0.0
 rfc3986==2.0.0
 rich==13.7.1
 SecretStorage==3.3.3
-selenium==4.19.0
-setuptools==69.2.0
+selenium==4.21.0
+setuptools==69.5.1
 six==1.16.0
 sniffio==1.3.1
 snowballstemmer==2.2.0
 sortedcontainers==2.4.0
 Sphinx==7.1.2
 sphinx-rtd-theme==2.0.0
 sphinxcontrib-applehelp==1.0.4
 sphinxcontrib-devhelp==1.0.2
 sphinxcontrib-htmlhelp==2.0.1
 sphinxcontrib-jquery==4.1
 sphinxcontrib-jsmath==1.0.1
 sphinxcontrib-qthelp==1.0.3
 sphinxcontrib-serializinghtml==1.1.5
-sqlparse==0.4.4
+sqlparse==0.5.0
 stevedore==5.2.0
 termcolor==2.4.0
 toml==0.10.2
 tomli==2.0.1
-tomlkit==0.12.4
-tqdm==4.66.2
-trio==0.25.0
+tomli_w==1.0.0
+tomlkit==0.12.5
+tqdm==4.66.4
+trio==0.25.1
 trio-websocket==0.11.1
-twine==5.0.0
-types-pytz==2024.1.0.20240203
+twine==5.1.0
+types-pytz==2024.1.0.20240417
 types-PyYAML==6.0.12.20240311
-types-requests==2.31.0.20240311
-typing_extensions==4.10.0
+types-requests==2.31.0.20240406
+types-tqdm==4.66.0.20240417
+typing_extensions==4.11.0
 urllib3==2.2.1
 wcwidth==0.2.13
 wheel==0.43.0
 wsproto==1.2.0
-zipp==3.18.1
+xdg==5.1.1
+zipp==3.18.2
```

### Comparing `pytest-logikal-2.0.4/requirements/docs.txt.lock` & `pytest_logikal-3.0.0/requirements/docs.txt.lock`

 * *Files 10% similar despite different names*

```diff
@@ -1,123 +1,125 @@
 ###################################################################################################
 ##
 ##  DO NOT EDIT THIS FILE.
 ##  This is a locked requirements file generated by pyorbs.
 ##
-##  Requirements hash: d0e0f8d5a9932fb72fc911a08f4b18b3216541cf2ccb1890e12e6000a4625e01
+##  Requirements hash: 519a3e2a8b754a3421dbdacf6d29f65e9572b79571813a4602a86387be35784d
 ##
 ###################################################################################################
 -e .
 alabaster==0.7.13
 appdirs==1.4.4
 asgiref==3.8.1
-astroid==3.1.0
+astroid==3.2.1
 attrs==23.2.0
-Babel==2.14.0
+Babel==2.15.0
 backports.zoneinfo==0.2.1
 bandit==1.7.8
-black==24.3.0
+black==24.4.2
 certifi==2024.2.2
 charset-normalizer==3.3.2
 click==8.1.7
 colorama==0.4.6
-coverage==7.4.4
+coverage==7.5.1
 cssbeautifier==1.15.1
 dill==0.3.8
-Django==4.2.11
-django-migration-linter==5.0.0
+Django==4.2.13
+django-migration-linter==5.1.0
 django-stubs==4.2.7
-django-stubs-ext==4.2.7
+django-stubs-ext==5.0.0
 djlint==1.34.1
 docker==7.0.0
 docutils==0.20.1
 EditorConfig==0.12.4
-exceptiongroup==1.2.0
-execnet==2.0.2
+exceptiongroup==1.2.1
+execnet==2.1.1
 factory-boy==3.3.0
-Faker==24.4.0
-filelock==3.13.3
+Faker==25.2.0
+filelock==3.14.0
 h11==0.14.0
 html-tag-names==0.1.2
 html-void-elements==0.1.0
-idna==3.6
+idna==3.7
 imagesize==1.4.1
 importlib_metadata==7.1.0
 inflection==0.5.1
 iniconfig==2.0.0
 isort==5.13.2
-Jinja2==3.1.3
+Jinja2==3.1.4
 jsbeautifier==1.15.1
-json5==0.9.24
+json5==0.9.25
 logikal-docs==1.1.4
 logikal-utils==1.0.1
 markdown-it-py==3.0.0
 MarkupSafe==2.1.5
 mccabe==0.7.0
 mdurl==0.1.2
-mypy==1.9.0
+mypy==1.10.0
 mypy-extensions==1.0.0
 outcome==1.3.0.post0
 packaging==23.2
 pathspec==0.12.1
 pbr==6.0.0
-pillow==10.2.0
+pillow==10.3.0
 pip==24.0
 pip-licenses==4.4.0
-platformdirs==4.2.0
-pluggy==1.4.0
+platformdirs==4.2.2
+pluggy==1.5.0
 prettytable==3.10.0
 psutil==5.9.8
 pycodestyle==2.11.1
 pydocstyle==6.3.0
-Pygments==2.17.2
-pylint==3.1.0
+Pygments==2.18.0
+pylint==3.2.0
 pylint-django==2.5.5
 pylint-plugin-utils==0.8.2
 pyorbs==2.1.0
 PySocks==1.7.1
-pytest==8.1.1
+pytest==8.2.0
 pytest-cov==5.0.0
 pytest-django==4.8.0
 pytest-factoryboy==2.7.0
 pytest-mock==3.14.0
 pytest-mypy==0.10.3
-pytest-xdist==3.5.0
+pytest-xdist==3.6.1
 python-dateutil==2.9.0.post0
 pytz==2024.1
 PyYAML==6.0.1
 regex==2023.12.25
 requests==2.31.0
 rich==13.7.1
-selenium==4.19.0
-setuptools==69.2.0
+selenium==4.21.0
+setuptools==69.5.1
 six==1.16.0
 sniffio==1.3.1
 snowballstemmer==2.2.0
 sortedcontainers==2.4.0
 Sphinx==7.1.2
 sphinx-rtd-theme==2.0.0
 sphinxcontrib-applehelp==1.0.4
 sphinxcontrib-devhelp==1.0.2
 sphinxcontrib-htmlhelp==2.0.1
 sphinxcontrib-jquery==4.1
 sphinxcontrib-jsmath==1.0.1
 sphinxcontrib-qthelp==1.0.3
 sphinxcontrib-serializinghtml==1.1.5
-sqlparse==0.4.4
+sqlparse==0.5.0
 stevedore==5.2.0
 termcolor==2.4.0
 toml==0.10.2
 tomli==2.0.1
-tomlkit==0.12.4
-tqdm==4.66.2
-trio==0.25.0
+tomlkit==0.12.5
+tqdm==4.66.4
+trio==0.25.1
 trio-websocket==0.11.1
-types-pytz==2024.1.0.20240203
+types-pytz==2024.1.0.20240417
 types-PyYAML==6.0.12.20240311
-types-requests==2.31.0.20240311
-typing_extensions==4.10.0
+types-requests==2.31.0.20240406
+types-tqdm==4.66.0.20240417
+typing_extensions==4.11.0
 urllib3==2.2.1
 wcwidth==0.2.13
 wheel==0.43.0
 wsproto==1.2.0
-zipp==3.18.1
+xdg==5.1.1
+zipp==3.18.2
```

