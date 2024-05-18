# Comparing `tmp/galaxy-language-server-0.8.0.tar.gz` & `tmp/galaxy-language-server-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "galaxy-language-server-0.8.0.tar", last modified: Sun Oct  2 13:38:40 2022, max compression
+gzip compressed data, was "galaxy-language-server-0.9.0.tar", last modified: Thu Oct 20 19:07:40 2022, max compression
```

## Comparing `galaxy-language-server-0.8.0.tar` & `galaxy-language-server-0.9.0.tar`

### file list

```diff
@@ -1,61 +1,61 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-02 13:38:40.038088 galaxy-language-server-0.8.0/
--rw-r--r--   0 runner    (1001) docker     (121)    13397 2022-10-02 13:38:40.038088 galaxy-language-server-0.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2998 2022-10-02 13:38:31.000000 galaxy-language-server-0.8.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-02 13:38:40.034088 galaxy-language-server-0.8.0/galaxy_language_server.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    13397 2022-10-02 13:38:39.000000 galaxy-language-server-0.8.0/galaxy_language_server.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1636 2022-10-02 13:38:39.000000 galaxy-language-server-0.8.0/galaxy_language_server.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-02 13:38:39.000000 galaxy-language-server-0.8.0/galaxy_language_server.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       82 2022-10-02 13:38:39.000000 galaxy-language-server-0.8.0/galaxy_language_server.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        9 2022-10-02 13:38:39.000000 galaxy-language-server-0.8.0/galaxy_language_server.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-02 13:38:40.034088 galaxy-language-server-0.8.0/galaxyls/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-02 13:38:31.000000 galaxy-language-server-0.8.0/galaxyls/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      815 2022-10-02 13:38:31.000000 galaxy-language-server-0.8.0/galaxyls/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)      779 2022-10-02 13:38:31.000000 galaxy-language-server-0.8.0/galaxyls/config.py
--rw-r--r--   0 runner    (1001) docker     (121)      638 2022-10-02 13:38:31.000000 galaxy-language-server-0.8.0/galaxyls/constants.py
--rw-r--r--   0 runner    (1001) docker     (121)    12212 2022-10-02 13:38:31.000000 galaxy-language-server-0.8.0/galaxyls/server.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-02 13:38:40.034088 galaxy-language-server-0.8.0/galaxyls/services/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-02 13:38:31.000000 galaxy-language-server-0.8.0/galaxyls/services/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    10372 2022-10-02 13:38:31.000000 galaxy-language-server-0.8.0/galaxyls/services/completion.py
--rw-r--r--   0 runner    (1001) docker     (121)     9028 2022-10-02 13:38:31.000000 galaxy-language-server-0.8.0/galaxyls/services/context.py
--rw-r--r--   0 runner    (1001) docker     (121)     1845 2022-10-02 13:38:31.000000 galaxy-language-server-0.8.0/galaxyls/services/definitions.py
--rw-r--r--   0 runner    (1001) docker     (121)     1481 2022-10-02 13:38:31.000000 galaxy-language-server-0.8.0/galaxyls/services/format.py
--rw-r--r--   0 runner    (1001) docker     (121)     7450 2022-10-02 13:38:31.000000 galaxy-language-server-0.8.0/galaxyls/services/language.py
--rw-r--r--   0 runner    (1001) docker     (121)     1302 2022-10-02 13:38:31.000000 galaxy-language-server-0.8.0/galaxyls/services/macros.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-02 13:38:40.038088 galaxy-language-server-0.8.0/galaxyls/services/tools/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-02 13:38:31.000000 galaxy-language-server-0.8.0/galaxyls/services/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1877 2022-10-02 13:38:31.000000 galaxy-language-server-0.8.0/galaxyls/services/tools/common.py
--rw-r--r--   0 runner    (1001) docker     (121)     1281 2022-10-02 13:38:31.000000 galaxy-language-server-0.8.0/galaxyls/services/tools/constants.py
--rw-r--r--   0 runner    (1001) docker     (121)     8412 2022-10-02 13:38:31.000000 galaxy-language-server-0.8.0/galaxyls/services/tools/document.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-02 13:38:40.038088 galaxy-language-server-0.8.0/galaxyls/services/tools/generators/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-02 13:38:31.000000 galaxy-language-server-0.8.0/galaxyls/services/tools/generators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    10637 2022-10-02 13:38:31.000000 galaxy-language-server-0.8.0/galaxyls/services/tools/generators/command.py
--rw-r--r--   0 runner    (1001) docker     (121)     4691 2022-10-02 13:38:31.000000 galaxy-language-server-0.8.0/galaxyls/services/tools/generators/snippets.py
--rw-r--r--   0 runner    (1001) docker     (121)    15626 2022-10-02 13:38:31.000000 galaxy-language-server-0.8.0/galaxyls/services/tools/generators/tests.py
--rw-r--r--   0 runner    (1001) docker     (121)     8636 2022-10-02 13:38:31.000000 galaxy-language-server-0.8.0/galaxyls/services/tools/inputs.py
--rw-r--r--   0 runner    (1001) docker     (121)     2868 2022-10-02 13:38:31.000000 galaxy-language-server-0.8.0/galaxyls/services/tools/iuc.py
--rw-r--r--   0 runner    (1001) docker     (121)     1734 2022-10-02 13:38:31.000000 galaxy-language-server-0.8.0/galaxyls/services/tools/linting.py
--rw-r--r--   0 runner    (1001) docker     (121)     7498 2022-10-02 13:38:31.000000 galaxy-language-server-0.8.0/galaxyls/services/tools/macros.py
--rw-r--r--   0 runner    (1001) docker     (121)    14750 2022-10-02 13:38:31.000000 galaxy-language-server-0.8.0/galaxyls/services/tools/refactor.py
--rw-r--r--   0 runner    (1001) docker     (121)     2402 2022-10-02 13:38:31.000000 galaxy-language-server-0.8.0/galaxyls/services/tools/testing.py
--rw-r--r--   0 runner    (1001) docker     (121)     1972 2022-10-02 13:38:31.000000 galaxy-language-server-0.8.0/galaxyls/services/validation.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-02 13:38:40.038088 galaxy-language-server-0.8.0/galaxyls/services/xml/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-02 13:38:31.000000 galaxy-language-server-0.8.0/galaxyls/services/xml/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      691 2022-10-02 13:38:31.000000 galaxy-language-server-0.8.0/galaxyls/services/xml/constants.py
--rw-r--r--   0 runner    (1001) docker     (121)    11682 2022-10-02 13:38:31.000000 galaxy-language-server-0.8.0/galaxyls/services/xml/document.py
--rw-r--r--   0 runner    (1001) docker     (121)    16208 2022-10-02 13:38:31.000000 galaxy-language-server-0.8.0/galaxyls/services/xml/nodes.py
--rw-r--r--   0 runner    (1001) docker     (121)    10129 2022-10-02 13:38:31.000000 galaxy-language-server-0.8.0/galaxyls/services/xml/parser.py
--rw-r--r--   0 runner    (1001) docker     (121)    11972 2022-10-02 13:38:31.000000 galaxy-language-server-0.8.0/galaxyls/services/xml/scanner.py
--rw-r--r--   0 runner    (1001) docker     (121)     1461 2022-10-02 13:38:31.000000 galaxy-language-server-0.8.0/galaxyls/services/xml/types.py
--rw-r--r--   0 runner    (1001) docker     (121)     6684 2022-10-02 13:38:31.000000 galaxy-language-server-0.8.0/galaxyls/services/xml/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-02 13:38:40.038088 galaxy-language-server-0.8.0/galaxyls/services/xsd/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-02 13:38:31.000000 galaxy-language-server-0.8.0/galaxyls/services/xsd/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      993 2022-10-02 13:38:31.000000 galaxy-language-server-0.8.0/galaxyls/services/xsd/constants.py
--rw-r--r--   0 runner    (1001) docker     (121)     8590 2022-10-02 13:38:31.000000 galaxy-language-server-0.8.0/galaxyls/services/xsd/parser.py
--rw-r--r--   0 runner    (1001) docker     (121)     2217 2022-10-02 13:38:31.000000 galaxy-language-server-0.8.0/galaxyls/services/xsd/service.py
--rw-r--r--   0 runner    (1001) docker     (121)     6382 2022-10-02 13:38:31.000000 galaxy-language-server-0.8.0/galaxyls/services/xsd/types.py
--rw-r--r--   0 runner    (1001) docker     (121)     8838 2022-10-02 13:38:31.000000 galaxy-language-server-0.8.0/galaxyls/services/xsd/validation.py
--rw-r--r--   0 runner    (1001) docker     (121)     2672 2022-10-02 13:38:31.000000 galaxy-language-server-0.8.0/galaxyls/types.py
--rw-r--r--   0 runner    (1001) docker     (121)     1161 2022-10-02 13:38:31.000000 galaxy-language-server-0.8.0/galaxyls/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)      223 2022-10-02 13:38:31.000000 galaxy-language-server-0.8.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-10-02 13:38:40.038088 galaxy-language-server-0.8.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1667 2022-10-02 13:38:31.000000 galaxy-language-server-0.8.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-20 19:07:40.068320 galaxy-language-server-0.9.0/
+-rw-r--r--   0 runner    (1001) docker     (121)    13776 2022-10-20 19:07:40.068320 galaxy-language-server-0.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     2998 2022-10-20 19:07:24.000000 galaxy-language-server-0.9.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-20 19:07:40.064320 galaxy-language-server-0.9.0/galaxy_language_server.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)    13776 2022-10-20 19:07:39.000000 galaxy-language-server-0.9.0/galaxy_language_server.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     1636 2022-10-20 19:07:40.000000 galaxy-language-server-0.9.0/galaxy_language_server.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-20 19:07:39.000000 galaxy-language-server-0.9.0/galaxy_language_server.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       82 2022-10-20 19:07:39.000000 galaxy-language-server-0.9.0/galaxy_language_server.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        9 2022-10-20 19:07:39.000000 galaxy-language-server-0.9.0/galaxy_language_server.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-20 19:07:40.064320 galaxy-language-server-0.9.0/galaxyls/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-20 19:07:24.000000 galaxy-language-server-0.9.0/galaxyls/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      815 2022-10-20 19:07:24.000000 galaxy-language-server-0.9.0/galaxyls/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      779 2022-10-20 19:07:24.000000 galaxy-language-server-0.9.0/galaxyls/config.py
+-rw-r--r--   0 runner    (1001) docker     (121)      638 2022-10-20 19:07:24.000000 galaxy-language-server-0.9.0/galaxyls/constants.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12212 2022-10-20 19:07:24.000000 galaxy-language-server-0.9.0/galaxyls/server.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-20 19:07:40.068320 galaxy-language-server-0.9.0/galaxyls/services/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-20 19:07:24.000000 galaxy-language-server-0.9.0/galaxyls/services/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10372 2022-10-20 19:07:24.000000 galaxy-language-server-0.9.0/galaxyls/services/completion.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9028 2022-10-20 19:07:24.000000 galaxy-language-server-0.9.0/galaxyls/services/context.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1845 2022-10-20 19:07:24.000000 galaxy-language-server-0.9.0/galaxyls/services/definitions.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1481 2022-10-20 19:07:24.000000 galaxy-language-server-0.9.0/galaxyls/services/format.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7450 2022-10-20 19:07:24.000000 galaxy-language-server-0.9.0/galaxyls/services/language.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1302 2022-10-20 19:07:24.000000 galaxy-language-server-0.9.0/galaxyls/services/macros.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-20 19:07:40.068320 galaxy-language-server-0.9.0/galaxyls/services/tools/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-20 19:07:24.000000 galaxy-language-server-0.9.0/galaxyls/services/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1877 2022-10-20 19:07:24.000000 galaxy-language-server-0.9.0/galaxyls/services/tools/common.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1281 2022-10-20 19:07:24.000000 galaxy-language-server-0.9.0/galaxyls/services/tools/constants.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8412 2022-10-20 19:07:24.000000 galaxy-language-server-0.9.0/galaxyls/services/tools/document.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-20 19:07:40.068320 galaxy-language-server-0.9.0/galaxyls/services/tools/generators/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-20 19:07:24.000000 galaxy-language-server-0.9.0/galaxyls/services/tools/generators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10637 2022-10-20 19:07:24.000000 galaxy-language-server-0.9.0/galaxyls/services/tools/generators/command.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4691 2022-10-20 19:07:24.000000 galaxy-language-server-0.9.0/galaxyls/services/tools/generators/snippets.py
+-rw-r--r--   0 runner    (1001) docker     (121)    15626 2022-10-20 19:07:24.000000 galaxy-language-server-0.9.0/galaxyls/services/tools/generators/tests.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8636 2022-10-20 19:07:24.000000 galaxy-language-server-0.9.0/galaxyls/services/tools/inputs.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2868 2022-10-20 19:07:24.000000 galaxy-language-server-0.9.0/galaxyls/services/tools/iuc.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1734 2022-10-20 19:07:24.000000 galaxy-language-server-0.9.0/galaxyls/services/tools/linting.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7498 2022-10-20 19:07:24.000000 galaxy-language-server-0.9.0/galaxyls/services/tools/macros.py
+-rw-r--r--   0 runner    (1001) docker     (121)    14750 2022-10-20 19:07:24.000000 galaxy-language-server-0.9.0/galaxyls/services/tools/refactor.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2402 2022-10-20 19:07:24.000000 galaxy-language-server-0.9.0/galaxyls/services/tools/testing.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1972 2022-10-20 19:07:24.000000 galaxy-language-server-0.9.0/galaxyls/services/validation.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-20 19:07:40.068320 galaxy-language-server-0.9.0/galaxyls/services/xml/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-20 19:07:24.000000 galaxy-language-server-0.9.0/galaxyls/services/xml/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      691 2022-10-20 19:07:24.000000 galaxy-language-server-0.9.0/galaxyls/services/xml/constants.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11682 2022-10-20 19:07:24.000000 galaxy-language-server-0.9.0/galaxyls/services/xml/document.py
+-rw-r--r--   0 runner    (1001) docker     (121)    16208 2022-10-20 19:07:24.000000 galaxy-language-server-0.9.0/galaxyls/services/xml/nodes.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10129 2022-10-20 19:07:24.000000 galaxy-language-server-0.9.0/galaxyls/services/xml/parser.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11972 2022-10-20 19:07:24.000000 galaxy-language-server-0.9.0/galaxyls/services/xml/scanner.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1461 2022-10-20 19:07:24.000000 galaxy-language-server-0.9.0/galaxyls/services/xml/types.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6684 2022-10-20 19:07:24.000000 galaxy-language-server-0.9.0/galaxyls/services/xml/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-20 19:07:40.068320 galaxy-language-server-0.9.0/galaxyls/services/xsd/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-20 19:07:24.000000 galaxy-language-server-0.9.0/galaxyls/services/xsd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      993 2022-10-20 19:07:24.000000 galaxy-language-server-0.9.0/galaxyls/services/xsd/constants.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8590 2022-10-20 19:07:24.000000 galaxy-language-server-0.9.0/galaxyls/services/xsd/parser.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2217 2022-10-20 19:07:24.000000 galaxy-language-server-0.9.0/galaxyls/services/xsd/service.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6382 2022-10-20 19:07:24.000000 galaxy-language-server-0.9.0/galaxyls/services/xsd/types.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8838 2022-10-20 19:07:24.000000 galaxy-language-server-0.9.0/galaxyls/services/xsd/validation.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2672 2022-10-20 19:07:24.000000 galaxy-language-server-0.9.0/galaxyls/types.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1161 2022-10-20 19:07:24.000000 galaxy-language-server-0.9.0/galaxyls/utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)      223 2022-10-20 19:07:24.000000 galaxy-language-server-0.9.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-10-20 19:07:40.068320 galaxy-language-server-0.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     1667 2022-10-20 19:07:24.000000 galaxy-language-server-0.9.0/setup.py
```

### Comparing `galaxy-language-server-0.8.0/PKG-INFO` & `galaxy-language-server-0.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: galaxy-language-server
-Version: 0.8.0
+Version: 0.9.0
 Summary: A language server for Galaxy (https://galaxyproject.org) tool wrappers
 Home-page: https://github.com/davelopez/galaxy-language-server/tree/main/server
 Author: David López
 Author-email: davelopez7391@gmail.com
 License: Apache License 2.0
 Description: # Galaxy Language Server
         
@@ -75,14 +75,24 @@
         ```
         INFO:pygls.server:Starting server on 127.0.0.1:2087
         INFO:pygls.server:Shutting down the server
         INFO:pygls.server:Closing the event loop.
         ```
         # Galaxy Language Server Changelog
         
+        ## [0.9.0] - 2022-10-20
+        
+        ### Added
+        
+        - New setting to silently install the language server ([#210](https://github.com/galaxyproject/galaxy-language-server/pull/210)).
+        
+        ### Changed
+        
+        - Code quality: fix e2e tests for linting ([#211](https://github.com/galaxyproject/galaxy-language-server/pull/211)).
+        
         ## [0.8.0] - 2022-10-02
         
         ### Added
         
         - Full Galaxy tool linting integration ([#204](https://github.com/galaxyproject/galaxy-language-server/pull/204)).
         
         ### Changed
```

### Comparing `galaxy-language-server-0.8.0/README.md` & `galaxy-language-server-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `galaxy-language-server-0.8.0/galaxy_language_server.egg-info/PKG-INFO` & `galaxy-language-server-0.9.0/galaxy_language_server.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: galaxy-language-server
-Version: 0.8.0
+Version: 0.9.0
 Summary: A language server for Galaxy (https://galaxyproject.org) tool wrappers
 Home-page: https://github.com/davelopez/galaxy-language-server/tree/main/server
 Author: David López
 Author-email: davelopez7391@gmail.com
 License: Apache License 2.0
 Description: # Galaxy Language Server
         
@@ -75,14 +75,24 @@
         ```
         INFO:pygls.server:Starting server on 127.0.0.1:2087
         INFO:pygls.server:Shutting down the server
         INFO:pygls.server:Closing the event loop.
         ```
         # Galaxy Language Server Changelog
         
+        ## [0.9.0] - 2022-10-20
+        
+        ### Added
+        
+        - New setting to silently install the language server ([#210](https://github.com/galaxyproject/galaxy-language-server/pull/210)).
+        
+        ### Changed
+        
+        - Code quality: fix e2e tests for linting ([#211](https://github.com/galaxyproject/galaxy-language-server/pull/211)).
+        
         ## [0.8.0] - 2022-10-02
         
         ### Added
         
         - Full Galaxy tool linting integration ([#204](https://github.com/galaxyproject/galaxy-language-server/pull/204)).
         
         ### Changed
```

### Comparing `galaxy-language-server-0.8.0/galaxy_language_server.egg-info/SOURCES.txt` & `galaxy-language-server-0.9.0/galaxy_language_server.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `galaxy-language-server-0.8.0/galaxyls/__main__.py` & `galaxy-language-server-0.9.0/galaxyls/__main__.py`

 * *Files identical despite different names*

### Comparing `galaxy-language-server-0.8.0/galaxyls/config.py` & `galaxy-language-server-0.9.0/galaxyls/config.py`

 * *Files identical despite different names*

### Comparing `galaxy-language-server-0.8.0/galaxyls/constants.py` & `galaxy-language-server-0.9.0/galaxyls/constants.py`

 * *Files identical despite different names*

### Comparing `galaxy-language-server-0.8.0/galaxyls/server.py` & `galaxy-language-server-0.9.0/galaxyls/server.py`

 * *Files identical despite different names*

### Comparing `galaxy-language-server-0.8.0/galaxyls/services/completion.py` & `galaxy-language-server-0.9.0/galaxyls/services/completion.py`

 * *Files identical despite different names*

### Comparing `galaxy-language-server-0.8.0/galaxyls/services/context.py` & `galaxy-language-server-0.9.0/galaxyls/services/context.py`

 * *Files identical despite different names*

### Comparing `galaxy-language-server-0.8.0/galaxyls/services/definitions.py` & `galaxy-language-server-0.9.0/galaxyls/services/definitions.py`

 * *Files identical despite different names*

### Comparing `galaxy-language-server-0.8.0/galaxyls/services/format.py` & `galaxy-language-server-0.9.0/galaxyls/services/format.py`

 * *Files identical despite different names*

### Comparing `galaxy-language-server-0.8.0/galaxyls/services/language.py` & `galaxy-language-server-0.9.0/galaxyls/services/language.py`

 * *Files identical despite different names*

### Comparing `galaxy-language-server-0.8.0/galaxyls/services/macros.py` & `galaxy-language-server-0.9.0/galaxyls/services/macros.py`

 * *Files identical despite different names*

### Comparing `galaxy-language-server-0.8.0/galaxyls/services/tools/common.py` & `galaxy-language-server-0.9.0/galaxyls/services/tools/common.py`

 * *Files identical despite different names*

### Comparing `galaxy-language-server-0.8.0/galaxyls/services/tools/constants.py` & `galaxy-language-server-0.9.0/galaxyls/services/tools/constants.py`

 * *Files identical despite different names*

### Comparing `galaxy-language-server-0.8.0/galaxyls/services/tools/document.py` & `galaxy-language-server-0.9.0/galaxyls/services/tools/document.py`

 * *Files identical despite different names*

### Comparing `galaxy-language-server-0.8.0/galaxyls/services/tools/generators/command.py` & `galaxy-language-server-0.9.0/galaxyls/services/tools/generators/command.py`

 * *Files identical despite different names*

### Comparing `galaxy-language-server-0.8.0/galaxyls/services/tools/generators/snippets.py` & `galaxy-language-server-0.9.0/galaxyls/services/tools/generators/snippets.py`

 * *Files identical despite different names*

### Comparing `galaxy-language-server-0.8.0/galaxyls/services/tools/generators/tests.py` & `galaxy-language-server-0.9.0/galaxyls/services/tools/generators/tests.py`

 * *Files identical despite different names*

### Comparing `galaxy-language-server-0.8.0/galaxyls/services/tools/inputs.py` & `galaxy-language-server-0.9.0/galaxyls/services/tools/inputs.py`

 * *Files identical despite different names*

### Comparing `galaxy-language-server-0.8.0/galaxyls/services/tools/iuc.py` & `galaxy-language-server-0.9.0/galaxyls/services/tools/iuc.py`

 * *Files identical despite different names*

### Comparing `galaxy-language-server-0.8.0/galaxyls/services/tools/linting.py` & `galaxy-language-server-0.9.0/galaxyls/services/tools/linting.py`

 * *Files identical despite different names*

### Comparing `galaxy-language-server-0.8.0/galaxyls/services/tools/macros.py` & `galaxy-language-server-0.9.0/galaxyls/services/tools/macros.py`

 * *Files identical despite different names*

### Comparing `galaxy-language-server-0.8.0/galaxyls/services/tools/refactor.py` & `galaxy-language-server-0.9.0/galaxyls/services/tools/refactor.py`

 * *Files identical despite different names*

### Comparing `galaxy-language-server-0.8.0/galaxyls/services/tools/testing.py` & `galaxy-language-server-0.9.0/galaxyls/services/tools/testing.py`

 * *Files identical despite different names*

### Comparing `galaxy-language-server-0.8.0/galaxyls/services/validation.py` & `galaxy-language-server-0.9.0/galaxyls/services/validation.py`

 * *Files identical despite different names*

### Comparing `galaxy-language-server-0.8.0/galaxyls/services/xml/constants.py` & `galaxy-language-server-0.9.0/galaxyls/services/xml/constants.py`

 * *Files identical despite different names*

### Comparing `galaxy-language-server-0.8.0/galaxyls/services/xml/document.py` & `galaxy-language-server-0.9.0/galaxyls/services/xml/document.py`

 * *Files identical despite different names*

### Comparing `galaxy-language-server-0.8.0/galaxyls/services/xml/nodes.py` & `galaxy-language-server-0.9.0/galaxyls/services/xml/nodes.py`

 * *Files identical despite different names*

### Comparing `galaxy-language-server-0.8.0/galaxyls/services/xml/parser.py` & `galaxy-language-server-0.9.0/galaxyls/services/xml/parser.py`

 * *Files identical despite different names*

### Comparing `galaxy-language-server-0.8.0/galaxyls/services/xml/scanner.py` & `galaxy-language-server-0.9.0/galaxyls/services/xml/scanner.py`

 * *Files identical despite different names*

### Comparing `galaxy-language-server-0.8.0/galaxyls/services/xml/types.py` & `galaxy-language-server-0.9.0/galaxyls/services/xml/types.py`

 * *Files identical despite different names*

### Comparing `galaxy-language-server-0.8.0/galaxyls/services/xml/utils.py` & `galaxy-language-server-0.9.0/galaxyls/services/xml/utils.py`

 * *Files identical despite different names*

### Comparing `galaxy-language-server-0.8.0/galaxyls/services/xsd/constants.py` & `galaxy-language-server-0.9.0/galaxyls/services/xsd/constants.py`

 * *Files identical despite different names*

### Comparing `galaxy-language-server-0.8.0/galaxyls/services/xsd/parser.py` & `galaxy-language-server-0.9.0/galaxyls/services/xsd/parser.py`

 * *Files identical despite different names*

### Comparing `galaxy-language-server-0.8.0/galaxyls/services/xsd/service.py` & `galaxy-language-server-0.9.0/galaxyls/services/xsd/service.py`

 * *Files identical despite different names*

### Comparing `galaxy-language-server-0.8.0/galaxyls/services/xsd/types.py` & `galaxy-language-server-0.9.0/galaxyls/services/xsd/types.py`

 * *Files identical despite different names*

### Comparing `galaxy-language-server-0.8.0/galaxyls/services/xsd/validation.py` & `galaxy-language-server-0.9.0/galaxyls/services/xsd/validation.py`

 * *Files identical despite different names*

### Comparing `galaxy-language-server-0.8.0/galaxyls/types.py` & `galaxy-language-server-0.9.0/galaxyls/types.py`

 * *Files identical despite different names*

### Comparing `galaxy-language-server-0.8.0/galaxyls/utils.py` & `galaxy-language-server-0.9.0/galaxyls/utils.py`

 * *Files identical despite different names*

### Comparing `galaxy-language-server-0.8.0/setup.py` & `galaxy-language-server-0.9.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 from setuptools import (
     find_packages,
     setup,
 )
 
 PACKAGE_NAME = "galaxy-language-server"
-VERSION = "0.8.0"
+VERSION = "0.9.0"
 AUTHOR = "David López"
 AUTHOR_EMAIL = "davelopez7391@gmail.com"
 DESCRIPTION = "A language server for Galaxy (https://galaxyproject.org) tool wrappers"
 KEYWORDS = ["galaxy", "python", "language server"]
 LICENSE = "Apache License 2.0"
 URL = "https://github.com/davelopez/galaxy-language-server/tree/main/server"
```

