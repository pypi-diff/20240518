# Comparing `tmp/bcf_client-0.0.240418.tar.gz` & `tmp/bcf_client-0.0.240518.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bcf_client-0.0.240418.tar", last modified: Thu Apr 18 00:35:45 2024, max compression
+gzip compressed data, was "bcf_client-0.0.240518.tar", last modified: Sat May 18 00:37:30 2024, max compression
```

## Comparing `bcf_client-0.0.240418.tar` & `bcf_client-0.0.240518.tar`

### file list

```diff
@@ -1,62 +1,62 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 00:35:45.195573 bcf_client-0.0.240418/
--rw-r--r--   0 runner    (1001) docker     (127)    32473 2024-04-18 00:35:38.000000 bcf_client-0.0.240418/COPYING
--rw-r--r--   0 runner    (1001) docker     (127)     7652 2024-04-18 00:35:38.000000 bcf_client-0.0.240418/COPYING.LESSER
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-18 00:35:38.000000 bcf_client-0.0.240418/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      854 2024-04-18 00:35:45.195573 bcf_client-0.0.240418/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      170 2024-04-18 00:35:38.000000 bcf_client-0.0.240418/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     2804 2024-04-18 00:35:42.000000 bcf_client-0.0.240418/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-18 00:35:45.195573 bcf_client-0.0.240418/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-18 00:35:38.000000 bcf_client-0.0.240418/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 00:35:45.183573 bcf_client-0.0.240418/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 00:35:45.187573 bcf_client-0.0.240418/src/bcf/
--rw-r--r--   0 runner    (1001) docker     (127)      749 2024-04-18 00:35:38.000000 bcf_client-0.0.240418/src/bcf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2472 2024-04-18 00:35:38.000000 bcf_client-0.0.240418/src/bcf/bcfxml.py
--rw-r--r--   0 runner    (1001) docker     (127)     2175 2024-04-18 00:35:38.000000 bcf_client-0.0.240418/src/bcf/geometry.py
--rw-r--r--   0 runner    (1001) docker     (127)     2071 2024-04-18 00:35:38.000000 bcf_client-0.0.240418/src/bcf/inmemory_zipfile.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 00:35:38.000000 bcf_client-0.0.240418/src/bcf/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 00:35:45.187573 bcf_client-0.0.240418/src/bcf/v2/
--rw-r--r--   0 runner    (1001) docker     (127)      747 2024-04-18 00:35:38.000000 bcf_client-0.0.240418/src/bcf/v2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10384 2024-04-18 00:35:38.000000 bcf_client-0.0.240418/src/bcf/v2/bcfxml.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 00:35:45.187573 bcf_client-0.0.240418/src/bcf/v2/model/
--rw-r--r--   0 runner    (1001) docker     (127)     1478 2024-04-18 00:35:38.000000 bcf_client-0.0.240418/src/bcf/v2/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11006 2024-04-18 00:35:38.000000 bcf_client-0.0.240418/src/bcf/v2/model/markup.py
--rw-r--r--   0 runner    (1001) docker     (127)      911 2024-04-18 00:35:38.000000 bcf_client-0.0.240418/src/bcf/v2/model/project.py
--rw-r--r--   0 runner    (1001) docker     (127)      486 2024-04-18 00:35:38.000000 bcf_client-0.0.240418/src/bcf/v2/model/version.py
--rw-r--r--   0 runner    (1001) docker     (127)    10903 2024-04-18 00:35:38.000000 bcf_client-0.0.240418/src/bcf/v2/model/visinfo.py
--rw-r--r--   0 runner    (1001) docker     (127)    11768 2024-04-18 00:35:38.000000 bcf_client-0.0.240418/src/bcf/v2/topic.py
--rw-r--r--   0 runner    (1001) docker     (127)    10236 2024-04-18 00:35:38.000000 bcf_client-0.0.240418/src/bcf/v2/visinfo.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 00:35:45.191573 bcf_client-0.0.240418/src/bcf/v2/xsd/
--rw-r--r--   0 runner    (1001) docker     (127)     6661 2024-04-18 00:35:38.000000 bcf_client-0.0.240418/src/bcf/v2/xsd/markup.xsd
--rw-r--r--   0 runner    (1001) docker     (127)      669 2024-04-18 00:35:38.000000 bcf_client-0.0.240418/src/bcf/v2/xsd/project.xsd
--rw-r--r--   0 runner    (1001) docker     (127)      449 2024-04-18 00:35:38.000000 bcf_client-0.0.240418/src/bcf/v2/xsd/version.xsd
--rw-r--r--   0 runner    (1001) docker     (127)     7220 2024-04-18 00:35:38.000000 bcf_client-0.0.240418/src/bcf/v2/xsd/visinfo.xsd
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 00:35:45.191573 bcf_client-0.0.240418/src/bcf/v3/
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-18 00:35:38.000000 bcf_client-0.0.240418/src/bcf/v3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    22095 2024-04-18 00:35:38.000000 bcf_client-0.0.240418/src/bcf/v3/bcfapi.py
--rw-r--r--   0 runner    (1001) docker     (127)    10985 2024-04-18 00:35:38.000000 bcf_client-0.0.240418/src/bcf/v3/bcfxml.py
--rw-r--r--   0 runner    (1001) docker     (127)     2252 2024-04-18 00:35:38.000000 bcf_client-0.0.240418/src/bcf/v3/document.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 00:35:45.191573 bcf_client-0.0.240418/src/bcf/v3/model/
--rw-r--r--   0 runner    (1001) docker     (127)     2488 2024-04-18 00:35:38.000000 bcf_client-0.0.240418/src/bcf/v3/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1452 2024-04-18 00:35:38.000000 bcf_client-0.0.240418/src/bcf/v3/model/documents.py
--rw-r--r--   0 runner    (1001) docker     (127)     4171 2024-04-18 00:35:38.000000 bcf_client-0.0.240418/src/bcf/v3/model/extensions.py
--rw-r--r--   0 runner    (1001) docker     (127)    14877 2024-04-18 00:35:38.000000 bcf_client-0.0.240418/src/bcf/v3/model/markup.py
--rw-r--r--   0 runner    (1001) docker     (127)      841 2024-04-18 00:35:38.000000 bcf_client-0.0.240418/src/bcf/v3/model/project.py
--rw-r--r--   0 runner    (1001) docker     (127)      255 2024-04-18 00:35:38.000000 bcf_client-0.0.240418/src/bcf/v3/model/version.py
--rw-r--r--   0 runner    (1001) docker     (127)    12135 2024-04-18 00:35:38.000000 bcf_client-0.0.240418/src/bcf/v3/model/visinfo.py
--rw-r--r--   0 runner    (1001) docker     (127)     7375 2024-04-18 00:35:38.000000 bcf_client-0.0.240418/src/bcf/v3/topic.py
--rw-r--r--   0 runner    (1001) docker     (127)    10006 2024-04-18 00:35:38.000000 bcf_client-0.0.240418/src/bcf/v3/visinfo.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 00:35:45.195573 bcf_client-0.0.240418/src/bcf/v3/xsd/
--rw-r--r--   0 runner    (1001) docker     (127)     1374 2024-04-18 00:35:38.000000 bcf_client-0.0.240418/src/bcf/v3/xsd/documents.xsd
--rw-r--r--   0 runner    (1001) docker     (127)     2879 2024-04-18 00:35:38.000000 bcf_client-0.0.240418/src/bcf/v3/xsd/extensions.xsd
--rw-r--r--   0 runner    (1001) docker     (127)     8921 2024-04-18 00:35:38.000000 bcf_client-0.0.240418/src/bcf/v3/xsd/markup.xsd
--rw-r--r--   0 runner    (1001) docker     (127)      647 2024-04-18 00:35:38.000000 bcf_client-0.0.240418/src/bcf/v3/xsd/project.xsd
--rw-r--r--   0 runner    (1001) docker     (127)      546 2024-04-18 00:35:38.000000 bcf_client-0.0.240418/src/bcf/v3/xsd/shared-types.xsd
--rw-r--r--   0 runner    (1001) docker     (127)      286 2024-04-18 00:35:38.000000 bcf_client-0.0.240418/src/bcf/v3/xsd/version.xsd
--rw-r--r--   0 runner    (1001) docker     (127)    10054 2024-04-18 00:35:38.000000 bcf_client-0.0.240418/src/bcf/v3/xsd/visinfo.xsd
--rw-r--r--   0 runner    (1001) docker     (127)     2414 2024-04-18 00:35:38.000000 bcf_client-0.0.240418/src/bcf/xml_parser.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 00:35:45.195573 bcf_client-0.0.240418/src/bcf_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      854 2024-04-18 00:35:45.000000 bcf_client-0.0.240418/src/bcf_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1244 2024-04-18 00:35:45.000000 bcf_client-0.0.240418/src/bcf_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 00:35:45.000000 bcf_client-0.0.240418/src/bcf_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-18 00:35:45.000000 bcf_client-0.0.240418/src/bcf_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-04-18 00:35:45.000000 bcf_client-0.0.240418/src/bcf_client.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 00:37:30.854946 bcf_client-0.0.240518/
+-rw-r--r--   0 runner    (1001) docker     (127)    32473 2024-05-18 00:37:22.000000 bcf_client-0.0.240518/COPYING
+-rw-r--r--   0 runner    (1001) docker     (127)     7652 2024-05-18 00:37:22.000000 bcf_client-0.0.240518/COPYING.LESSER
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-05-18 00:37:22.000000 bcf_client-0.0.240518/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      860 2024-05-18 00:37:30.854946 bcf_client-0.0.240518/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      170 2024-05-18 00:37:22.000000 bcf_client-0.0.240518/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2810 2024-05-18 00:37:27.000000 bcf_client-0.0.240518/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-18 00:37:30.854946 bcf_client-0.0.240518/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-18 00:37:22.000000 bcf_client-0.0.240518/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 00:37:30.846947 bcf_client-0.0.240518/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 00:37:30.850947 bcf_client-0.0.240518/src/bcf/
+-rw-r--r--   0 runner    (1001) docker     (127)      749 2024-05-18 00:37:22.000000 bcf_client-0.0.240518/src/bcf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2472 2024-05-18 00:37:22.000000 bcf_client-0.0.240518/src/bcf/bcfxml.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2175 2024-05-18 00:37:22.000000 bcf_client-0.0.240518/src/bcf/geometry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2071 2024-05-18 00:37:22.000000 bcf_client-0.0.240518/src/bcf/inmemory_zipfile.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-18 00:37:22.000000 bcf_client-0.0.240518/src/bcf/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 00:37:30.850947 bcf_client-0.0.240518/src/bcf/v2/
+-rw-r--r--   0 runner    (1001) docker     (127)      747 2024-05-18 00:37:22.000000 bcf_client-0.0.240518/src/bcf/v2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10384 2024-05-18 00:37:22.000000 bcf_client-0.0.240518/src/bcf/v2/bcfxml.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 00:37:30.850947 bcf_client-0.0.240518/src/bcf/v2/model/
+-rw-r--r--   0 runner    (1001) docker     (127)     1478 2024-05-18 00:37:22.000000 bcf_client-0.0.240518/src/bcf/v2/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11006 2024-05-18 00:37:22.000000 bcf_client-0.0.240518/src/bcf/v2/model/markup.py
+-rw-r--r--   0 runner    (1001) docker     (127)      911 2024-05-18 00:37:22.000000 bcf_client-0.0.240518/src/bcf/v2/model/project.py
+-rw-r--r--   0 runner    (1001) docker     (127)      486 2024-05-18 00:37:22.000000 bcf_client-0.0.240518/src/bcf/v2/model/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10903 2024-05-18 00:37:22.000000 bcf_client-0.0.240518/src/bcf/v2/model/visinfo.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11768 2024-05-18 00:37:22.000000 bcf_client-0.0.240518/src/bcf/v2/topic.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10236 2024-05-18 00:37:22.000000 bcf_client-0.0.240518/src/bcf/v2/visinfo.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 00:37:30.850947 bcf_client-0.0.240518/src/bcf/v2/xsd/
+-rw-r--r--   0 runner    (1001) docker     (127)     6661 2024-05-18 00:37:22.000000 bcf_client-0.0.240518/src/bcf/v2/xsd/markup.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)      669 2024-05-18 00:37:22.000000 bcf_client-0.0.240518/src/bcf/v2/xsd/project.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)      449 2024-05-18 00:37:22.000000 bcf_client-0.0.240518/src/bcf/v2/xsd/version.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)     7220 2024-05-18 00:37:22.000000 bcf_client-0.0.240518/src/bcf/v2/xsd/visinfo.xsd
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 00:37:30.850947 bcf_client-0.0.240518/src/bcf/v3/
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-18 00:37:22.000000 bcf_client-0.0.240518/src/bcf/v3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22095 2024-05-18 00:37:22.000000 bcf_client-0.0.240518/src/bcf/v3/bcfapi.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10985 2024-05-18 00:37:22.000000 bcf_client-0.0.240518/src/bcf/v3/bcfxml.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2252 2024-05-18 00:37:22.000000 bcf_client-0.0.240518/src/bcf/v3/document.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 00:37:30.854946 bcf_client-0.0.240518/src/bcf/v3/model/
+-rw-r--r--   0 runner    (1001) docker     (127)     2488 2024-05-18 00:37:22.000000 bcf_client-0.0.240518/src/bcf/v3/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1452 2024-05-18 00:37:22.000000 bcf_client-0.0.240518/src/bcf/v3/model/documents.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4171 2024-05-18 00:37:22.000000 bcf_client-0.0.240518/src/bcf/v3/model/extensions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14877 2024-05-18 00:37:22.000000 bcf_client-0.0.240518/src/bcf/v3/model/markup.py
+-rw-r--r--   0 runner    (1001) docker     (127)      841 2024-05-18 00:37:22.000000 bcf_client-0.0.240518/src/bcf/v3/model/project.py
+-rw-r--r--   0 runner    (1001) docker     (127)      255 2024-05-18 00:37:22.000000 bcf_client-0.0.240518/src/bcf/v3/model/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12135 2024-05-18 00:37:22.000000 bcf_client-0.0.240518/src/bcf/v3/model/visinfo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7375 2024-05-18 00:37:22.000000 bcf_client-0.0.240518/src/bcf/v3/topic.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10006 2024-05-18 00:37:22.000000 bcf_client-0.0.240518/src/bcf/v3/visinfo.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 00:37:30.854946 bcf_client-0.0.240518/src/bcf/v3/xsd/
+-rw-r--r--   0 runner    (1001) docker     (127)     1374 2024-05-18 00:37:22.000000 bcf_client-0.0.240518/src/bcf/v3/xsd/documents.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)     2879 2024-05-18 00:37:22.000000 bcf_client-0.0.240518/src/bcf/v3/xsd/extensions.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)     8921 2024-05-18 00:37:22.000000 bcf_client-0.0.240518/src/bcf/v3/xsd/markup.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)      647 2024-05-18 00:37:22.000000 bcf_client-0.0.240518/src/bcf/v3/xsd/project.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)      546 2024-05-18 00:37:22.000000 bcf_client-0.0.240518/src/bcf/v3/xsd/shared-types.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)      286 2024-05-18 00:37:22.000000 bcf_client-0.0.240518/src/bcf/v3/xsd/version.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)    10054 2024-05-18 00:37:22.000000 bcf_client-0.0.240518/src/bcf/v3/xsd/visinfo.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)     2507 2024-05-18 00:37:22.000000 bcf_client-0.0.240518/src/bcf/xml_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 00:37:30.854946 bcf_client-0.0.240518/src/bcf_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      860 2024-05-18 00:37:30.000000 bcf_client-0.0.240518/src/bcf_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1244 2024-05-18 00:37:30.000000 bcf_client-0.0.240518/src/bcf_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-18 00:37:30.000000 bcf_client-0.0.240518/src/bcf_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-18 00:37:30.000000 bcf_client-0.0.240518/src/bcf_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-18 00:37:30.000000 bcf_client-0.0.240518/src/bcf_client.egg-info/top_level.txt
```

### Comparing `bcf_client-0.0.240418/COPYING` & `bcf_client-0.0.240518/COPYING`

 * *Files identical despite different names*

### Comparing `bcf_client-0.0.240418/COPYING.LESSER` & `bcf_client-0.0.240518/COPYING.LESSER`

 * *Files identical despite different names*

### Comparing `bcf_client-0.0.240418/PKG-INFO` & `bcf_client-0.0.240518/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: bcf-client
-Version: 0.0.240418
+Version: 0.0.240518
 Summary: BCF-XML file handler.
 Project-URL: Source, https://github.com/IfcOpenShell/IfcOpenShell
 Project-URL: Issues, https://github.com/IfcOpenShell/IfcOpenShell/issues
 Keywords: IFC,BCF,BIM
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Utilities
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: COPYING
 License-File: COPYING.LESSER
-Requires-Dist: xsdata
+Requires-Dist: xsdata>=24.4
 Requires-Dist: numpy
 Requires-Dist: ifcopenshell
 
 # bcf
 
 A simple Python implementation of the BCF standard. Manipulation of BCF-XML is
 available via `bcfxml.py` and manipulation of BCF-API is available via
```

### Comparing `bcf_client-0.0.240418/pyproject.toml` & `bcf_client-0.0.240518/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -9,19 +9,19 @@
 name = "bcf-client"
 # author = "IfcOpenShell"
 description = "BCF-XML file handler."
 readme = "README.md"
 requires-python = ">=3.8"
 keywords = ["IFC", "BCF", "BIM"]
 dependencies = [
-    "xsdata",
+    "xsdata>=24.4",
     "numpy",
     "ifcopenshell",
 ]
-version = "0.0.240418"
+version = "0.0.240518"
 classifiers = [
     "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
     "Operating System :: OS Independent",
     "Programming Language :: Python :: 3",
     "Topic :: Scientific/Engineering",
     "Topic :: Utilities",
 ]
```

### Comparing `bcf_client-0.0.240418/src/bcf/__init__.py` & `bcf_client-0.0.240518/src/bcf/__init__.py`

 * *Files identical despite different names*

### Comparing `bcf_client-0.0.240418/src/bcf/bcfxml.py` & `bcf_client-0.0.240518/src/bcf/bcfxml.py`

 * *Files identical despite different names*

### Comparing `bcf_client-0.0.240418/src/bcf/geometry.py` & `bcf_client-0.0.240518/src/bcf/geometry.py`

 * *Files identical despite different names*

### Comparing `bcf_client-0.0.240418/src/bcf/inmemory_zipfile.py` & `bcf_client-0.0.240518/src/bcf/inmemory_zipfile.py`

 * *Files identical despite different names*

### Comparing `bcf_client-0.0.240418/src/bcf/v2/__init__.py` & `bcf_client-0.0.240518/src/bcf/v2/__init__.py`

 * *Files identical despite different names*

### Comparing `bcf_client-0.0.240418/src/bcf/v2/bcfxml.py` & `bcf_client-0.0.240518/src/bcf/v2/bcfxml.py`

 * *Files identical despite different names*

### Comparing `bcf_client-0.0.240418/src/bcf/v2/model/__init__.py` & `bcf_client-0.0.240518/src/bcf/v2/model/__init__.py`

 * *Files identical despite different names*

### Comparing `bcf_client-0.0.240418/src/bcf/v2/model/markup.py` & `bcf_client-0.0.240518/src/bcf/v2/model/markup.py`

 * *Files identical despite different names*

### Comparing `bcf_client-0.0.240418/src/bcf/v2/model/project.py` & `bcf_client-0.0.240518/src/bcf/v2/model/project.py`

 * *Files identical despite different names*

### Comparing `bcf_client-0.0.240418/src/bcf/v2/model/visinfo.py` & `bcf_client-0.0.240518/src/bcf/v2/model/visinfo.py`

 * *Files identical despite different names*

### Comparing `bcf_client-0.0.240418/src/bcf/v2/topic.py` & `bcf_client-0.0.240518/src/bcf/v2/topic.py`

 * *Files identical despite different names*

### Comparing `bcf_client-0.0.240418/src/bcf/v2/visinfo.py` & `bcf_client-0.0.240518/src/bcf/v2/visinfo.py`

 * *Files identical despite different names*

### Comparing `bcf_client-0.0.240418/src/bcf/v2/xsd/markup.xsd` & `bcf_client-0.0.240518/src/bcf/v2/xsd/markup.xsd`

 * *Files identical despite different names*

### Comparing `bcf_client-0.0.240418/src/bcf/v2/xsd/project.xsd` & `bcf_client-0.0.240518/src/bcf/v2/xsd/project.xsd`

 * *Files identical despite different names*

### Comparing `bcf_client-0.0.240418/src/bcf/v2/xsd/visinfo.xsd` & `bcf_client-0.0.240518/src/bcf/v2/xsd/visinfo.xsd`

 * *Files identical despite different names*

### Comparing `bcf_client-0.0.240418/src/bcf/v3/bcfapi.py` & `bcf_client-0.0.240518/src/bcf/v3/bcfapi.py`

 * *Files identical despite different names*

### Comparing `bcf_client-0.0.240418/src/bcf/v3/bcfxml.py` & `bcf_client-0.0.240518/src/bcf/v3/bcfxml.py`

 * *Files identical despite different names*

### Comparing `bcf_client-0.0.240418/src/bcf/v3/document.py` & `bcf_client-0.0.240518/src/bcf/v3/document.py`

 * *Files identical despite different names*

### Comparing `bcf_client-0.0.240418/src/bcf/v3/model/__init__.py` & `bcf_client-0.0.240518/src/bcf/v3/model/__init__.py`

 * *Files identical despite different names*

### Comparing `bcf_client-0.0.240418/src/bcf/v3/model/documents.py` & `bcf_client-0.0.240518/src/bcf/v3/model/documents.py`

 * *Files identical despite different names*

### Comparing `bcf_client-0.0.240418/src/bcf/v3/model/extensions.py` & `bcf_client-0.0.240518/src/bcf/v3/model/extensions.py`

 * *Files identical despite different names*

### Comparing `bcf_client-0.0.240418/src/bcf/v3/model/markup.py` & `bcf_client-0.0.240518/src/bcf/v3/model/markup.py`

 * *Files identical despite different names*

### Comparing `bcf_client-0.0.240418/src/bcf/v3/model/project.py` & `bcf_client-0.0.240518/src/bcf/v3/model/project.py`

 * *Files identical despite different names*

### Comparing `bcf_client-0.0.240418/src/bcf/v3/model/visinfo.py` & `bcf_client-0.0.240518/src/bcf/v3/model/visinfo.py`

 * *Files identical despite different names*

### Comparing `bcf_client-0.0.240418/src/bcf/v3/topic.py` & `bcf_client-0.0.240518/src/bcf/v3/topic.py`

 * *Files identical despite different names*

### Comparing `bcf_client-0.0.240418/src/bcf/v3/visinfo.py` & `bcf_client-0.0.240518/src/bcf/v3/visinfo.py`

 * *Files identical despite different names*

### Comparing `bcf_client-0.0.240418/src/bcf/v3/xsd/documents.xsd` & `bcf_client-0.0.240518/src/bcf/v3/xsd/documents.xsd`

 * *Files identical despite different names*

### Comparing `bcf_client-0.0.240418/src/bcf/v3/xsd/extensions.xsd` & `bcf_client-0.0.240518/src/bcf/v3/xsd/extensions.xsd`

 * *Files identical despite different names*

### Comparing `bcf_client-0.0.240418/src/bcf/v3/xsd/markup.xsd` & `bcf_client-0.0.240518/src/bcf/v3/xsd/markup.xsd`

 * *Files identical despite different names*

### Comparing `bcf_client-0.0.240418/src/bcf/v3/xsd/project.xsd` & `bcf_client-0.0.240518/src/bcf/v3/xsd/project.xsd`

 * *Files identical despite different names*

### Comparing `bcf_client-0.0.240418/src/bcf/v3/xsd/shared-types.xsd` & `bcf_client-0.0.240518/src/bcf/v3/xsd/shared-types.xsd`

 * *Files identical despite different names*

### Comparing `bcf_client-0.0.240418/src/bcf/v3/xsd/visinfo.xsd` & `bcf_client-0.0.240518/src/bcf/v3/xsd/visinfo.xsd`

 * *Files identical despite different names*

### Comparing `bcf_client-0.0.240418/src/bcf/xml_parser.py` & `bcf_client-0.0.240518/src/bcf/xml_parser.py`

 * *Files 11% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from xsdata.formats.dataclass.serializers import XmlSerializer
 from xsdata.formats.dataclass.serializers.config import SerializerConfig
 
 
 def build_xml_parser(context: Optional[XmlContext] = None) -> XmlParser:
     """Return a parser for an XML file."""
     parser = XmlParser(context=context or XmlContext())
-    parser.register_namespace("xs", "http://www.w3.org/2001/XMLSchema")
+    parser.register_namespace(ns_map=parser.ns_map, prefix="xs", uri="http://www.w3.org/2001/XMLSchema")
     return parser
 
 
 def build_serializer(context: Optional[XmlContext] = None) -> XmlSerializer:
     """Return a serializer for an XML file."""
     return XmlSerializer(
-        config=SerializerConfig(pretty_print=True),
+        config=SerializerConfig(indent="  "),
         context=context or XmlContext(),
     )
 
 
 T = TypeVar("T")
 
 
@@ -32,26 +32,28 @@
         """
         Parse an XML file to an object.
 
         Args:
             xml: The XML file as bytes.
             clazz: The class to parse to.
         """
+        ...
 
-    def serialize(self, obj: T, ns_map: Optional[dict[str, str]] = None) -> str:
+    def serialize(self, obj: object, ns_map: Optional[dict[str, str]] = None) -> str:
         """
         Serialize an object to XML.
 
         Args:
             obj: The object to serialize.
             ns_map: The namespace map to use.
 
         Returns:
             The XML as string.
         """
+        ...
 
 
 class XmlParserSerializer:
     """XML Parser and serializer wrapper."""
 
     def __init__(self) -> None:
         self.context = XmlContext()
@@ -64,20 +66,20 @@
 
         Args:
             xml: The XML file as bytes.
             clazz: The class to parse to.
         """
         return self.parser.from_bytes(xml, clazz)
 
-    def serialize(self, obj: T, ns_map: Optional[dict[str, str]] = None) -> str:
+    def serialize(self, obj: object, ns_map: Optional[dict[Optional[str], str]] = None) -> str:
         """
         Serialize an object to XML.
 
         Args:
             obj: The object to serialize.
             ns_map: The namespace map to use.
 
         Returns:
             The XML as string.
         """
-        ns_map = ns_map or {"xs": "http://www.w3.org/2001/XMLSchema"}
+        ns_map = ns_map or self.parser.ns_map or {"xs": "http://www.w3.org/2001/XMLSchema"}
         return self.serializer.render(obj, ns_map)
```

### Comparing `bcf_client-0.0.240418/src/bcf_client.egg-info/PKG-INFO` & `bcf_client-0.0.240518/src/bcf_client.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: bcf-client
-Version: 0.0.240418
+Version: 0.0.240518
 Summary: BCF-XML file handler.
 Project-URL: Source, https://github.com/IfcOpenShell/IfcOpenShell
 Project-URL: Issues, https://github.com/IfcOpenShell/IfcOpenShell/issues
 Keywords: IFC,BCF,BIM
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Utilities
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: COPYING
 License-File: COPYING.LESSER
-Requires-Dist: xsdata
+Requires-Dist: xsdata>=24.4
 Requires-Dist: numpy
 Requires-Dist: ifcopenshell
 
 # bcf
 
 A simple Python implementation of the BCF standard. Manipulation of BCF-XML is
 available via `bcfxml.py` and manipulation of BCF-API is available via
```

### Comparing `bcf_client-0.0.240418/src/bcf_client.egg-info/SOURCES.txt` & `bcf_client-0.0.240518/src/bcf_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

