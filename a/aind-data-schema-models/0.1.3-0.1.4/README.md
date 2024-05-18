# Comparing `tmp/aind_data_schema_models-0.1.3.tar.gz` & `tmp/aind_data_schema_models-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aind_data_schema_models-0.1.3.tar", last modified: Thu May 16 22:47:38 2024, max compression
+gzip compressed data, was "aind_data_schema_models-0.1.4.tar", last modified: Sat May 18 13:22:23 2024, max compression
```

## Comparing `aind_data_schema_models-0.1.3.tar` & `aind_data_schema_models-0.1.4.tar`

### file list

```diff
@@ -1,56 +1,56 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 22:47:38.437685 aind_data_schema_models-0.1.3/
--rw-r--r--   0 runner    (1001) docker     (127)       98 2024-05-16 22:47:24.000000 aind_data_schema_models-0.1.3/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 22:47:38.429685 aind_data_schema_models-0.1.3/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 22:47:38.433685 aind_data_schema_models-0.1.3/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)      834 2024-05-16 22:47:24.000000 aind_data_schema_models-0.1.3/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (127)      595 2024-05-16 22:47:24.000000 aind_data_schema_models-0.1.3/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0 runner    (1001) docker     (127)      772 2024-05-16 22:47:24.000000 aind_data_schema_models-0.1.3/.github/ISSUE_TEMPLATE/user-story.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 22:47:38.433685 aind_data_schema_models-0.1.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     3189 2024-05-16 22:47:24.000000 aind_data_schema_models-0.1.3/.github/workflows/tag_and_publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)      660 2024-05-16 22:47:24.000000 aind_data_schema_models-0.1.3/.github/workflows/test_and_lint.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2199 2024-05-16 22:47:24.000000 aind_data_schema_models-0.1.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-05-16 22:47:24.000000 aind_data_schema_models-0.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5297 2024-05-16 22:47:38.437685 aind_data_schema_models-0.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4634 2024-05-16 22:47:24.000000 aind_data_schema_models-0.1.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 22:47:38.433685 aind_data_schema_models-0.1.3/doc_template/
--rw-r--r--   0 runner    (1001) docker     (127)      638 2024-05-16 22:47:24.000000 aind_data_schema_models-0.1.3/doc_template/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)      769 2024-05-16 22:47:24.000000 aind_data_schema_models-0.1.3/doc_template/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 22:47:38.433685 aind_data_schema_models-0.1.3/doc_template/source/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 22:47:38.433685 aind_data_schema_models-0.1.3/doc_template/source/_static/
--rw-r--r--   0 runner    (1001) docker     (127)     8733 2024-05-16 22:47:24.000000 aind_data_schema_models-0.1.3/doc_template/source/_static/dark-logo.svg
--rw-r--r--   0 runner    (1001) docker     (127)   259838 2024-05-16 22:47:24.000000 aind_data_schema_models-0.1.3/doc_template/source/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (127)     8712 2024-05-16 22:47:24.000000 aind_data_schema_models-0.1.3/doc_template/source/_static/light-logo.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1771 2024-05-16 22:47:24.000000 aind_data_schema_models-0.1.3/doc_template/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)      470 2024-05-16 22:47:24.000000 aind_data_schema_models-0.1.3/doc_template/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1411 2024-05-16 22:47:24.000000 aind_data_schema_models-0.1.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-16 22:47:38.441686 aind_data_schema_models-0.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-16 22:47:24.000000 aind_data_schema_models-0.1.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 22:47:38.429685 aind_data_schema_models-0.1.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 22:47:38.437685 aind_data_schema_models-0.1.3/src/aind_data_schema_models/
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-16 22:47:25.000000 aind_data_schema_models-0.1.3/src/aind_data_schema_models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2714 2024-05-16 22:47:24.000000 aind_data_schema_models-0.1.3/src/aind_data_schema_models/data_name_patterns.py
--rw-r--r--   0 runner    (1001) docker     (127)     3597 2024-05-16 22:47:24.000000 aind_data_schema_models-0.1.3/src/aind_data_schema_models/harp_types.py
--rw-r--r--   0 runner    (1001) docker     (127)     3522 2024-05-16 22:47:24.000000 aind_data_schema_models-0.1.3/src/aind_data_schema_models/modalities.py
--rw-r--r--   0 runner    (1001) docker     (127)    28393 2024-05-16 22:47:24.000000 aind_data_schema_models-0.1.3/src/aind_data_schema_models/organizations.py
--rw-r--r--   0 runner    (1001) docker     (127)      714 2024-05-16 22:47:24.000000 aind_data_schema_models-0.1.3/src/aind_data_schema_models/pid_names.py
--rw-r--r--   0 runner    (1001) docker     (127)     3781 2024-05-16 22:47:24.000000 aind_data_schema_models-0.1.3/src/aind_data_schema_models/platforms.py
--rw-r--r--   0 runner    (1001) docker     (127)     1948 2024-05-16 22:47:24.000000 aind_data_schema_models-0.1.3/src/aind_data_schema_models/process_names.py
--rw-r--r--   0 runner    (1001) docker     (127)     1860 2024-05-16 22:47:24.000000 aind_data_schema_models-0.1.3/src/aind_data_schema_models/registry.py
--rw-r--r--   0 runner    (1001) docker     (127)     2282 2024-05-16 22:47:24.000000 aind_data_schema_models-0.1.3/src/aind_data_schema_models/species.py
--rw-r--r--   0 runner    (1001) docker     (127)      786 2024-05-16 22:47:24.000000 aind_data_schema_models-0.1.3/src/aind_data_schema_models/specimen_procedure_types.py
--rw-r--r--   0 runner    (1001) docker     (127)     2808 2024-05-16 22:47:24.000000 aind_data_schema_models-0.1.3/src/aind_data_schema_models/units.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 22:47:38.437685 aind_data_schema_models-0.1.3/src/aind_data_schema_models.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5297 2024-05-16 22:47:38.000000 aind_data_schema_models-0.1.3/src/aind_data_schema_models.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1461 2024-05-16 22:47:38.000000 aind_data_schema_models-0.1.3/src/aind_data_schema_models.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 22:47:38.000000 aind_data_schema_models-0.1.3/src/aind_data_schema_models.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       83 2024-05-16 22:47:38.000000 aind_data_schema_models-0.1.3/src/aind_data_schema_models.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-16 22:47:38.000000 aind_data_schema_models-0.1.3/src/aind_data_schema_models.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 22:47:38.437685 aind_data_schema_models-0.1.3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      146 2024-05-16 22:47:24.000000 aind_data_schema_models-0.1.3/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4509 2024-05-16 22:47:24.000000 aind_data_schema_models-0.1.3/tests/test_data_name_patterns.py
--rw-r--r--   0 runner    (1001) docker     (127)      435 2024-05-16 22:47:24.000000 aind_data_schema_models-0.1.3/tests/test_modalities.py
--rw-r--r--   0 runner    (1001) docker     (127)     1857 2024-05-16 22:47:24.000000 aind_data_schema_models-0.1.3/tests/test_models.py
--rw-r--r--   0 runner    (1001) docker     (127)      433 2024-05-16 22:47:24.000000 aind_data_schema_models-0.1.3/tests/test_organizations.py
--rw-r--r--   0 runner    (1001) docker     (127)      437 2024-05-16 22:47:24.000000 aind_data_schema_models-0.1.3/tests/test_process_names.py
--rw-r--r--   0 runner    (1001) docker     (127)      464 2024-05-16 22:47:24.000000 aind_data_schema_models-0.1.3/tests/test_specimen_procedure_types.py
--rw-r--r--   0 runner    (1001) docker     (127)      769 2024-05-16 22:47:24.000000 aind_data_schema_models-0.1.3/tests/test_units.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 13:22:23.354024 aind_data_schema_models-0.1.4/
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-05-18 13:22:11.000000 aind_data_schema_models-0.1.4/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 13:22:23.342024 aind_data_schema_models-0.1.4/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 13:22:23.346024 aind_data_schema_models-0.1.4/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      834 2024-05-18 13:22:11.000000 aind_data_schema_models-0.1.4/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (127)      595 2024-05-18 13:22:11.000000 aind_data_schema_models-0.1.4/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0 runner    (1001) docker     (127)      772 2024-05-18 13:22:11.000000 aind_data_schema_models-0.1.4/.github/ISSUE_TEMPLATE/user-story.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 13:22:23.346024 aind_data_schema_models-0.1.4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     3189 2024-05-18 13:22:11.000000 aind_data_schema_models-0.1.4/.github/workflows/tag_and_publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      660 2024-05-18 13:22:11.000000 aind_data_schema_models-0.1.4/.github/workflows/test_and_lint.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2199 2024-05-18 13:22:11.000000 aind_data_schema_models-0.1.4/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-05-18 13:22:11.000000 aind_data_schema_models-0.1.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5297 2024-05-18 13:22:23.354024 aind_data_schema_models-0.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4634 2024-05-18 13:22:11.000000 aind_data_schema_models-0.1.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 13:22:23.346024 aind_data_schema_models-0.1.4/doc_template/
+-rw-r--r--   0 runner    (1001) docker     (127)      638 2024-05-18 13:22:11.000000 aind_data_schema_models-0.1.4/doc_template/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)      769 2024-05-18 13:22:11.000000 aind_data_schema_models-0.1.4/doc_template/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 13:22:23.346024 aind_data_schema_models-0.1.4/doc_template/source/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 13:22:23.346024 aind_data_schema_models-0.1.4/doc_template/source/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)     8733 2024-05-18 13:22:11.000000 aind_data_schema_models-0.1.4/doc_template/source/_static/dark-logo.svg
+-rw-r--r--   0 runner    (1001) docker     (127)   259838 2024-05-18 13:22:11.000000 aind_data_schema_models-0.1.4/doc_template/source/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (127)     8712 2024-05-18 13:22:11.000000 aind_data_schema_models-0.1.4/doc_template/source/_static/light-logo.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1771 2024-05-18 13:22:11.000000 aind_data_schema_models-0.1.4/doc_template/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      470 2024-05-18 13:22:11.000000 aind_data_schema_models-0.1.4/doc_template/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1411 2024-05-18 13:22:11.000000 aind_data_schema_models-0.1.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-18 13:22:23.354024 aind_data_schema_models-0.1.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-18 13:22:11.000000 aind_data_schema_models-0.1.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 13:22:23.342024 aind_data_schema_models-0.1.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 13:22:23.350024 aind_data_schema_models-0.1.4/src/aind_data_schema_models/
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-18 13:22:11.000000 aind_data_schema_models-0.1.4/src/aind_data_schema_models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2714 2024-05-18 13:22:11.000000 aind_data_schema_models-0.1.4/src/aind_data_schema_models/data_name_patterns.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3597 2024-05-18 13:22:11.000000 aind_data_schema_models-0.1.4/src/aind_data_schema_models/harp_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3522 2024-05-18 13:22:11.000000 aind_data_schema_models-0.1.4/src/aind_data_schema_models/modalities.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28864 2024-05-18 13:22:11.000000 aind_data_schema_models-0.1.4/src/aind_data_schema_models/organizations.py
+-rw-r--r--   0 runner    (1001) docker     (127)      714 2024-05-18 13:22:11.000000 aind_data_schema_models-0.1.4/src/aind_data_schema_models/pid_names.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3781 2024-05-18 13:22:11.000000 aind_data_schema_models-0.1.4/src/aind_data_schema_models/platforms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1948 2024-05-18 13:22:11.000000 aind_data_schema_models-0.1.4/src/aind_data_schema_models/process_names.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1860 2024-05-18 13:22:11.000000 aind_data_schema_models-0.1.4/src/aind_data_schema_models/registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2282 2024-05-18 13:22:11.000000 aind_data_schema_models-0.1.4/src/aind_data_schema_models/species.py
+-rw-r--r--   0 runner    (1001) docker     (127)      786 2024-05-18 13:22:11.000000 aind_data_schema_models-0.1.4/src/aind_data_schema_models/specimen_procedure_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2808 2024-05-18 13:22:11.000000 aind_data_schema_models-0.1.4/src/aind_data_schema_models/units.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 13:22:23.350024 aind_data_schema_models-0.1.4/src/aind_data_schema_models.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5297 2024-05-18 13:22:23.000000 aind_data_schema_models-0.1.4/src/aind_data_schema_models.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1461 2024-05-18 13:22:23.000000 aind_data_schema_models-0.1.4/src/aind_data_schema_models.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-18 13:22:23.000000 aind_data_schema_models-0.1.4/src/aind_data_schema_models.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-05-18 13:22:23.000000 aind_data_schema_models-0.1.4/src/aind_data_schema_models.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-18 13:22:23.000000 aind_data_schema_models-0.1.4/src/aind_data_schema_models.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 13:22:23.350024 aind_data_schema_models-0.1.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2024-05-18 13:22:11.000000 aind_data_schema_models-0.1.4/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4509 2024-05-18 13:22:11.000000 aind_data_schema_models-0.1.4/tests/test_data_name_patterns.py
+-rw-r--r--   0 runner    (1001) docker     (127)      435 2024-05-18 13:22:11.000000 aind_data_schema_models-0.1.4/tests/test_modalities.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1857 2024-05-18 13:22:11.000000 aind_data_schema_models-0.1.4/tests/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)      433 2024-05-18 13:22:11.000000 aind_data_schema_models-0.1.4/tests/test_organizations.py
+-rw-r--r--   0 runner    (1001) docker     (127)      437 2024-05-18 13:22:11.000000 aind_data_schema_models-0.1.4/tests/test_process_names.py
+-rw-r--r--   0 runner    (1001) docker     (127)      464 2024-05-18 13:22:11.000000 aind_data_schema_models-0.1.4/tests/test_specimen_procedure_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)      769 2024-05-18 13:22:11.000000 aind_data_schema_models-0.1.4/tests/test_units.py
```

### Comparing `aind_data_schema_models-0.1.3/.github/ISSUE_TEMPLATE/bug_report.md` & `aind_data_schema_models-0.1.4/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `aind_data_schema_models-0.1.3/.github/ISSUE_TEMPLATE/feature_request.md` & `aind_data_schema_models-0.1.4/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `aind_data_schema_models-0.1.3/.github/ISSUE_TEMPLATE/user-story.md` & `aind_data_schema_models-0.1.4/.github/ISSUE_TEMPLATE/user-story.md`

 * *Files identical despite different names*

### Comparing `aind_data_schema_models-0.1.3/.github/workflows/tag_and_publish.yml` & `aind_data_schema_models-0.1.4/.github/workflows/tag_and_publish.yml`

 * *Files identical despite different names*

### Comparing `aind_data_schema_models-0.1.3/.github/workflows/test_and_lint.yml` & `aind_data_schema_models-0.1.4/.github/workflows/test_and_lint.yml`

 * *Files identical despite different names*

### Comparing `aind_data_schema_models-0.1.3/.gitignore` & `aind_data_schema_models-0.1.4/.gitignore`

 * *Files identical despite different names*

### Comparing `aind_data_schema_models-0.1.3/LICENSE` & `aind_data_schema_models-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `aind_data_schema_models-0.1.3/PKG-INFO` & `aind_data_schema_models-0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aind-data-schema-models
-Version: 0.1.3
+Version: 0.1.4
 Summary: Generated from aind-library-template
 Author: Allen Institute for Neural Dynamics
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `aind_data_schema_models-0.1.3/README.md` & `aind_data_schema_models-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `aind_data_schema_models-0.1.3/doc_template/Makefile` & `aind_data_schema_models-0.1.4/doc_template/Makefile`

 * *Files identical despite different names*

### Comparing `aind_data_schema_models-0.1.3/doc_template/make.bat` & `aind_data_schema_models-0.1.4/doc_template/make.bat`

 * *Files identical despite different names*

### Comparing `aind_data_schema_models-0.1.3/doc_template/source/_static/dark-logo.svg` & `aind_data_schema_models-0.1.4/doc_template/source/_static/dark-logo.svg`

 * *Files identical despite different names*

### Comparing `aind_data_schema_models-0.1.3/doc_template/source/_static/favicon.ico` & `aind_data_schema_models-0.1.4/doc_template/source/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `aind_data_schema_models-0.1.3/doc_template/source/_static/light-logo.svg` & `aind_data_schema_models-0.1.4/doc_template/source/_static/light-logo.svg`

 * *Files identical despite different names*

### Comparing `aind_data_schema_models-0.1.3/doc_template/source/conf.py` & `aind_data_schema_models-0.1.4/doc_template/source/conf.py`

 * *Files identical despite different names*

### Comparing `aind_data_schema_models-0.1.3/pyproject.toml` & `aind_data_schema_models-0.1.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `aind_data_schema_models-0.1.3/src/aind_data_schema_models/data_name_patterns.py` & `aind_data_schema_models-0.1.4/src/aind_data_schema_models/data_name_patterns.py`

 * *Files identical despite different names*

### Comparing `aind_data_schema_models-0.1.3/src/aind_data_schema_models/harp_types.py` & `aind_data_schema_models-0.1.4/src/aind_data_schema_models/harp_types.py`

 * *Files identical despite different names*

### Comparing `aind_data_schema_models-0.1.3/src/aind_data_schema_models/modalities.py` & `aind_data_schema_models-0.1.4/src/aind_data_schema_models/modalities.py`

 * *Files identical despite different names*

### Comparing `aind_data_schema_models-0.1.3/src/aind_data_schema_models/organizations.py` & `aind_data_schema_models-0.1.4/src/aind_data_schema_models/organizations.py`

 * *Files 0% similar despite different names*

```diff
@@ -398,14 +398,23 @@
 
     name: Literal["IR Robot Co"] = "IR Robot Co"
     abbreviation: Literal[None] = Field(None)
     registry: Literal[None] = Field(None)
     registry_identifier: Literal[None] = Field(None)
 
 
+class MidwestOpticalSystems(_Organization):
+    """MidwestOpticalSystems"""
+
+    name: Literal["Midwest Optical Systems, Inc."] = "Midwest Optical Systems, Inc."
+    abbreviation: Literal["MidOpt"] = "MidOpt"
+    registry: Literal[None] = Field(None)
+    registry_identifier: Literal[None] = Field(None)
+
+
 class Mitutuyo(_Organization):
     """Mitutuyo"""
 
     name: Literal["Mitutuyo"] = "Mitutuyo"
     abbreviation: Literal[None] = Field(None)
     registry: Literal[None] = Field(None)
     registry_identifier: Literal[None] = Field(None)
@@ -750,14 +759,15 @@
     JAX = JacksonLaboratory()
     JULABO = Julabo()
     LEE = TheLeeCompany()
     LEICA = Leica()
     LG = Lg()
     LIFECANVAS = LifeCanvas()
     MEADOWLARK = MeadowlarkOptics()
+    MIDOPT = MidwestOpticalSystems()
     MIGHTY_ZAP = IRRobotCo()
     MITUTUYO = Mitutuyo()
     MKS_NEWPORT = MKSNewport()
     MPI = Mpi()
     NATIONAL_INSTRUMENTS = NationalInstruments()
     NAVITAR = Navitar()
     NEW_SCALE_TECHNOLOGIES = NewScaleTechnologies()
@@ -824,15 +834,25 @@
             TheImagingSource,
             Thorlabs,
             Vieworks,
             Other,
         ],
         Field(discriminator="name"),
     ]
-    FILTER_MANUFACTURERS = Annotated[Union[Chroma, EdmundOptics, Semrock, Thorlabs, Other], Field(discriminator="name")]
+    FILTER_MANUFACTURERS = Annotated[
+        Union[
+            Chroma,
+            EdmundOptics,
+            MidwestOpticalSystems,
+            Semrock,
+            Thorlabs,
+            Other
+        ],
+        Field(discriminator="name"),
+    ]
     LENS_MANUFACTURERS = Annotated[
         Union[
             Computar,
             EdmundOptics,
             Fujinon,
             Hamamatsu,
             InfinityPhotoOptical,
```

### Comparing `aind_data_schema_models-0.1.3/src/aind_data_schema_models/pid_names.py` & `aind_data_schema_models-0.1.4/src/aind_data_schema_models/pid_names.py`

 * *Files identical despite different names*

### Comparing `aind_data_schema_models-0.1.3/src/aind_data_schema_models/platforms.py` & `aind_data_schema_models-0.1.4/src/aind_data_schema_models/platforms.py`

 * *Files identical despite different names*

### Comparing `aind_data_schema_models-0.1.3/src/aind_data_schema_models/process_names.py` & `aind_data_schema_models-0.1.4/src/aind_data_schema_models/process_names.py`

 * *Files identical despite different names*

### Comparing `aind_data_schema_models-0.1.3/src/aind_data_schema_models/registry.py` & `aind_data_schema_models-0.1.4/src/aind_data_schema_models/registry.py`

 * *Files identical despite different names*

### Comparing `aind_data_schema_models-0.1.3/src/aind_data_schema_models/species.py` & `aind_data_schema_models-0.1.4/src/aind_data_schema_models/species.py`

 * *Files identical despite different names*

### Comparing `aind_data_schema_models-0.1.3/src/aind_data_schema_models/specimen_procedure_types.py` & `aind_data_schema_models-0.1.4/src/aind_data_schema_models/specimen_procedure_types.py`

 * *Files identical despite different names*

### Comparing `aind_data_schema_models-0.1.3/src/aind_data_schema_models/units.py` & `aind_data_schema_models-0.1.4/src/aind_data_schema_models/units.py`

 * *Files identical despite different names*

### Comparing `aind_data_schema_models-0.1.3/src/aind_data_schema_models.egg-info/PKG-INFO` & `aind_data_schema_models-0.1.4/src/aind_data_schema_models.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aind-data-schema-models
-Version: 0.1.3
+Version: 0.1.4
 Summary: Generated from aind-library-template
 Author: Allen Institute for Neural Dynamics
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `aind_data_schema_models-0.1.3/src/aind_data_schema_models.egg-info/SOURCES.txt` & `aind_data_schema_models-0.1.4/src/aind_data_schema_models.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aind_data_schema_models-0.1.3/tests/test_data_name_patterns.py` & `aind_data_schema_models-0.1.4/tests/test_data_name_patterns.py`

 * *Files identical despite different names*

### Comparing `aind_data_schema_models-0.1.3/tests/test_models.py` & `aind_data_schema_models-0.1.4/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `aind_data_schema_models-0.1.3/tests/test_units.py` & `aind_data_schema_models-0.1.4/tests/test_units.py`

 * *Files identical despite different names*

